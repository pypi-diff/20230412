# Comparing `tmp/easyquery_query_builder-0.1.0.tar.gz` & `tmp/easyquery_query_builder-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyquery_query_builder-0.1.0.tar", max compression
+gzip compressed data, was "easyquery_query_builder-0.1.1.tar", max compression
```

## Comparing `easyquery_query_builder-0.1.0.tar` & `easyquery_query_builder-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0        0 2023-04-04 22:01:26.361168 easyquery_query_builder-0.1.0/easyquery_query_builder/__init__.py
--rw-r--r--   0        0        0     8310 2023-04-11 07:10:31.822646 easyquery_query_builder-0.1.0/easyquery_query_builder/queries.py
--rw-r--r--   0        0        0      505 2023-04-11 06:34:31.840150 easyquery_query_builder-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       31 2023-04-11 07:19:27.504670 easyquery_query_builder-0.1.0/README.md
--rw-r--r--   0        0        0      668 1970-01-01 00:00:00.000000 easyquery_query_builder-0.1.0/setup.py
--rw-r--r--   0        0        0      389 1970-01-01 00:00:00.000000 easyquery_query_builder-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-04 22:01:26.361168 easyquery_query_builder-0.1.1/easyquery_query_builder/__init__.py
+-rw-r--r--   0        0        0     8486 2023-04-12 08:03:07.930811 easyquery_query_builder-0.1.1/easyquery_query_builder/queries.py
+-rw-r--r--   0        0        0      505 2023-04-12 08:04:15.234451 easyquery_query_builder-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    12961 2023-04-12 08:02:13.105404 easyquery_query_builder-0.1.1/README.md
+-rw-r--r--   0        0        0    13319 1970-01-01 00:00:00.000000 easyquery_query_builder-0.1.1/PKG-INFO
```

### Comparing `easyquery_query_builder-0.1.0/easyquery_query_builder/queries.py` & `easyquery_query_builder-0.1.1/easyquery_query_builder/queries.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from easyvalid_data_validator.validator import validate_json_data
 from easyvalid_data_validator.constraints import Constraint
 
 logging.basicConfig(level=logging.INFO)
 
 class Query(ABC):
+
     @abstractmethod
     def parse(self) -> str:
         pass
 
 
 class ReadQuery:
     def __init__(self, select_="", from_="", where_="", group_by_="", having_="", order_by_=""):
@@ -55,44 +56,44 @@
                     f"{f' having {self.having_}' if self.having_ else ''}" \
                     f"{f' order by {self.order_by_}' if self.order_by_ else ''}"
         return statement
 
 
 class ReadQueryWithJoins(ReadQuery):
     """ Subclass of ReadQuery which implements joins """
-    def __init__(self, select_="", from_="", where_="", group_by_="", having_="", order_by_="", _joins=""):
+    def __init__(self, select_="", from_="", where_="", group_by_="", having_="", order_by_="", joins_=""):
         super().__init__(select_, from_, where_, group_by_, having_, order_by_)
-        self._joins: list[list[str] | str] = _joins
+        self.joins_: list[list[str] | str] = joins_
 
     def parse(self) -> str:
         """ Creates sql query expression can be extended with join statements using fields provided in instance """
 
         # validation of all fields - checks only types and types of members
         query_data = self.__dict__
         constraints = {
             "select_": {Constraint.IS_TYPE: str},
             "from_": {Constraint.IS_TYPE: str},
             "where_": {Constraint.IS_TYPE: str},
             "group_by_": {Constraint.IS_TYPE: str},
             "having_": {Constraint.IS_TYPE: str},
             "order_by_": {Constraint.IS_TYPE: str},
-            "_joins": {Constraint.IS_TYPE: list, Constraint.ARRAY_MEMBERS_TYPE: list}
+            "joins_": {Constraint.IS_TYPE: list, Constraint.ARRAY_MEMBERS_TYPE: list}
         }
         validate_json_data(query_data, constraints)
 
         # validation that force all fields to be properly structured - minimum of select and from statements, having only with group by
         s, f, w, g, h = self.select_, self.from_, self.where_, self.group_by_, self.having_
         if (s == "" and f == "") or (s != "" and f == "") or (s == "" and f != ""):
             raise ValueError("Query requirement is to have select and from statements")
 
         if h != "" and g == "":
             raise ValueError("You cannot use having block without declaring group by block")
 
         # concatenation of joins
-        joins_exp = " ".join([f"join {table} as {alias} on {conditions}" for table, alias, conditions in self._joins])
+        joins_exp = " ".join([f"join {table} as {alias} on {conditions}" for table, alias, conditions in self.joins_])
 
         # creation of sql query
         statement = f"{f'select {self.select_}' if self.select_ else ''}" \
                     f"{f' from {self.from_}' if self.from_ else ''}" \
                     f" {joins_exp}" \
                     f"{f' where {self.where_}' if self.where_ else ''}" \
                     f"{f' group by {self.group_by_}' if self.group_by_ else ''}" \
@@ -118,65 +119,69 @@
         return self
 
     def add_from_statement(self, new_from: str) -> Self:
         """ Ads new from statement provided by user. Basic validation of argument is performed"""
         data = {"new_from": new_from}
         constraints = {"new_from": {Constraint.IS_TYPE: str}}
         validate_json_data(data, constraints)
-        self.query.from_ = f"{new_from}"
+        self.query.from_ = new_from
         return self
 
     def add_where_statement(self, new_where: str) -> Self:
         """ Ads new where statement provided by user. Basic validation of argument is performed"""
         data = {"new_where": new_where}
         constraints = {"new_where": {Constraint.IS_TYPE: str}}
         validate_json_data(data, constraints)
-        self.query.where_ = f"{new_where}"
+        self.query.where_ = new_where
         return self
 
     def add_group_by_statement(self, new_group_by: str) -> Self:
         """ Ads new group by statement provided by user. Basic validation of argument is performed"""
         data = {"new_group_by": new_group_by}
         constraints = {"new_group_by": {Constraint.IS_TYPE: str}}
         validate_json_data(data, constraints)
-        self.query.group_by_ = f"{new_group_by}"
+        self.query.group_by_ = new_group_by
         return self
 
     def add_having_statement(self, new_having: str) -> Self:
         """ Ads new having statement provided by user. Basic validation of argument is performed"""
         data = {"new_having": new_having}
         constraints = {"new_having": {Constraint.IS_TYPE: str}}
         validate_json_data(data, constraints)
-        self.query.having_ = f"{new_having}"
+        self.query.having_ = new_having
         return self
 
     def add_order_by_statement(self, new_order_by: str) -> Self:
         """ Ads new order by statement provided by user. Basic validation of argument is performed"""
         data = {"new_order_by": new_order_by}
         constraints = {"new_order_by": {Constraint.IS_TYPE: str}}
         validate_json_data(data, constraints)
-        self.query.order_by_ = f"{new_order_by}"
+        self.query.order_by_ = new_order_by
         return self
 
     def build(self) -> ReadQuery:
         """ Builds query based on all operations that were made """
         return self.query
 
 
-class ReadQueryWithJoinBuilder(ReadQueryBuilder):
+class ReadQueryWithJoinsBuilder(ReadQueryBuilder):
     """
         Builder that is subclass of ReadQueryBuilder used to create new ReadQueriesWithJoin
         'from scratch' or modify existing ones to desired form
     """
     def __init__(self, query: Query | None = None):
         if query is None:
             self.query = ReadQueryWithJoins()
         else:
             self.query = query
 
     def add_joins_statement(self, new_joins: str) -> Self:
-        """ Ads new joins arguments provided by user. Basic validation of argument is performed"""
+        """ Ads new joins arguments provided by user: [[<table_name>, <table_alias>, <join_condition>], ...]. Basic validation of argument is performed"""
         data = {"new_joins": new_joins}
         constraints = {"new_joins": {Constraint.IS_TYPE: list, Constraint.ARRAY_MEMBERS_TYPE: list}}
         validate_json_data(data, constraints)
-        self.query._joins = new_joins
+        self.query.joins_ = new_joins
         return self
+
+    def build(self) -> ReadQueryWithJoins:
+        """ Builds query based on all operations that were made """
+        return self.query
```

