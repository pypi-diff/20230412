# Comparing `tmp/uk_election_ids-0.7.2.tar.gz` & `tmp/uk_election_ids-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uk_election_ids-0.7.2.tar", last modified: Fri Mar 10 10:24:16 2023, max compression
+gzip compressed data, was "uk_election_ids-0.7.3.tar", last modified: Wed Apr 12 20:06:20 2023, max compression
```

## Comparing `uk_election_ids-0.7.2.tar` & `uk_election_ids-0.7.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 10:24:16.140458 uk_election_ids-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-10 10:24:05.000000 uk_election_ids-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-10 10:24:05.000000 uk_election_ids-0.7.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-03-10 10:24:16.140458 uk_election_ids-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-03-10 10:24:05.000000 uk_election_ids-0.7.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-10 10:24:16.140458 uk_election_ids-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-03-10 10:24:05.000000 uk_election_ids-0.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 10:24:16.140458 uk_election_ids-0.7.2/uk_election_ids/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 10:24:05.000000 uk_election_ids-0.7.2/uk_election_ids/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 10:24:16.140458 uk_election_ids-0.7.2/uk_election_ids/data/
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-03-10 10:24:05.000000 uk_election_ids-0.7.2/uk_election_ids/data/id_requirements.json
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-03-10 10:24:05.000000 uk_election_ids-0.7.2/uk_election_ids/data/voting_systems.json
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-03-10 10:24:05.000000 uk_election_ids-0.7.2/uk_election_ids/datapackage.py
--rw-r--r--   0 runner    (1001) docker     (123)    13894 2023-03-10 10:24:05.000000 uk_election_ids-0.7.2/uk_election_ids/election_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-03-10 10:24:05.000000 uk_election_ids-0.7.2/uk_election_ids/metadata_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-03-10 10:24:05.000000 uk_election_ids-0.7.2/uk_election_ids/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-03-10 10:24:05.000000 uk_election_ids-0.7.2/uk_election_ids/slugger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 10:24:16.140458 uk_election_ids-0.7.2/uk_election_ids.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-03-10 10:24:16.000000 uk_election_ids-0.7.2/uk_election_ids.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-03-10 10:24:16.000000 uk_election_ids-0.7.2/uk_election_ids.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 10:24:16.000000 uk_election_ids-0.7.2/uk_election_ids.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-10 10:24:16.000000 uk_election_ids-0.7.2/uk_election_ids.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-10 10:24:16.000000 uk_election_ids-0.7.2/uk_election_ids.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:06:20.256075 uk_election_ids-0.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-12 20:06:09.000000 uk_election_ids-0.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-12 20:06:09.000000 uk_election_ids-0.7.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-12 20:06:20.256075 uk_election_ids-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-12 20:06:09.000000 uk_election_ids-0.7.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 20:06:20.256075 uk_election_ids-0.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-04-12 20:06:09.000000 uk_election_ids-0.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:06:20.256075 uk_election_ids-0.7.3/uk_election_ids/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 20:06:09.000000 uk_election_ids-0.7.3/uk_election_ids/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:06:20.256075 uk_election_ids-0.7.3/uk_election_ids/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-04-12 20:06:09.000000 uk_election_ids-0.7.3/uk_election_ids/data/id_requirements.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-04-12 20:06:09.000000 uk_election_ids-0.7.3/uk_election_ids/data/voting_systems.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-04-12 20:06:09.000000 uk_election_ids-0.7.3/uk_election_ids/datapackage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13999 2023-04-12 20:06:09.000000 uk_election_ids-0.7.3/uk_election_ids/election_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-04-12 20:06:09.000000 uk_election_ids-0.7.3/uk_election_ids/metadata_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-12 20:06:09.000000 uk_election_ids-0.7.3/uk_election_ids/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-12 20:06:09.000000 uk_election_ids-0.7.3/uk_election_ids/slugger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:06:20.256075 uk_election_ids-0.7.3/uk_election_ids.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-12 20:06:20.000000 uk_election_ids-0.7.3/uk_election_ids.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-12 20:06:20.000000 uk_election_ids-0.7.3/uk_election_ids.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 20:06:20.000000 uk_election_ids-0.7.3/uk_election_ids.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-12 20:06:20.000000 uk_election_ids-0.7.3/uk_election_ids.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-12 20:06:20.000000 uk_election_ids-0.7.3/uk_election_ids.egg-info/top_level.txt
```

### Comparing `uk_election_ids-0.7.2/LICENSE` & `uk_election_ids-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `uk_election_ids-0.7.2/PKG-INFO` & `uk_election_ids-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uk_election_ids
-Version: 0.7.2
+Version: 0.7.3
 Summary: Create Democracy Club Election Identifiers
 Home-page: https://github.com/DemocracyClub/uk-election-ids/
 Author: chris48s
 License: MIT
 Project-URL: Documentation, https://democracyclub.github.io/uk-election-ids/
 Project-URL: Source, https://github.com/DemocracyClub/uk-election-ids/
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `uk_election_ids-0.7.2/README.md` & `uk_election_ids-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `uk_election_ids-0.7.2/setup.py` & `uk_election_ids-0.7.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+
 from setuptools import setup
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 
 def _get_description():
@@ -12,26 +13,33 @@
             return f.read()
     except IOError:
         return ""
 
 
 setup(
     name="uk_election_ids",
-    version="0.7.2",
+    version="0.7.3",
     author="chris48s",
     license="MIT",
     url="https://github.com/DemocracyClub/uk-election-ids/",
     packages=["uk_election_ids"],
-    package_data={'uk_election_ids':  ['data/*.json']},
+    package_data={"uk_election_ids": ["data/*.json"]},
     description="Create Democracy Club Election Identifiers",
     long_description=_get_description(),
     long_description_content_type="text/markdown",
     extras_require={
         "testing": ["coveralls"],
-        "development": ["sphinx", "sphinx_rtd_theme", "ghp-import", "pydantic"],
+        "development": [
+            "sphinx",
+            "sphinx_rtd_theme",
+            "ghp-import",
+            "pydantic",
+            "black==23.3.0",
+            "ruff==0.0.261",
+        ],
     },
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
```

### Comparing `uk_election_ids-0.7.2/uk_election_ids/data/id_requirements.json` & `uk_election_ids-0.7.3/uk_election_ids/data/id_requirements.json`

 * *Files identical despite different names*

### Comparing `uk_election_ids-0.7.2/uk_election_ids/data/voting_systems.json` & `uk_election_ids-0.7.3/uk_election_ids/data/voting_systems.json`

 * *Files identical despite different names*

### Comparing `uk_election_ids-0.7.2/uk_election_ids/datapackage.py` & `uk_election_ids-0.7.3/uk_election_ids/datapackage.py`

 * *Files 17% similar despite different names*

```diff
@@ -46,16 +46,24 @@
         ],
         "can_have_orgs": False,
         "can_have_divs": True,
     },
     "gla": {
         "name": "Greater London Assembly elections",
         "subtypes": [
-            {"name": "Constituencies", "election_subtype": "c", "can_have_divs": True},
-            {"name": "Additional", "election_subtype": "a", "can_have_divs": False},
+            {
+                "name": "Constituencies",
+                "election_subtype": "c",
+                "can_have_divs": True,
+            },
+            {
+                "name": "Additional",
+                "election_subtype": "a",
+                "can_have_divs": False,
+            },
         ],
         "can_have_orgs": False,
     },
     "local": {
         "name": "Local elections",
         "subtypes": [],
         "can_have_orgs": True,
@@ -73,15 +81,15 @@
         "can_have_orgs": True,
         "can_have_divs": False,
     },
     "ref": {
         "name": "Referendum elections",
         "subtypes": [],
         "can_have_orgs": True,
-        "can_have_divs": True,
+        "can_have_divs": False,
     },
 }
 
 voting_system_data = Path(__file__).parent / "data/voting_systems.json"
 VOTING_SYSTEMS = json.load(voting_system_data.open())["voting_systems"]
 id_requirements_data = Path(__file__).parent / "data/id_requirements.json"
 ID_REQUIREMENTS = json.load(id_requirements_data.open())["id_type"]
```

### Comparing `uk_election_ids-0.7.2/uk_election_ids/election_ids.py` & `uk_election_ids-0.7.3/uk_election_ids/election_ids.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+import contextlib
 from datetime import datetime
+
 from .datapackage import ELECTION_TYPES
 from .parser import DataPackageParser
 from .slugger import slugify
 
 parser = DataPackageParser(ELECTION_TYPES)
 RULES = parser.build_rules()
 CONTEST_TYPES = ("by", "by election", "by-election", "election")
@@ -66,16 +68,15 @@
 
         return date.strftime("%Y-%m-%d")
 
     @property
     def _can_have_divs(self):
         if isinstance(self.spec.can_have_divs, (bool,)):
             return self.spec.can_have_divs
-        else:
-            return self.spec.can_have_divs[self.subtype]
+        return self.spec.can_have_divs[self.subtype]
 
     def with_subtype(self, subtype):
         """Add a subtype segment
 
         Args:
             subtype (str): May be one of ``['a', 'c', 'r']``. See the
                 `Reference Definition <https://elections.democracyclub.org.uk/reference_definition>`_.
@@ -145,65 +146,72 @@
         Raises:
             ValueError
         """
         self._validate_contest_type(contest_type)
         if contest_type.lower() in ("by", "by election", "by-election"):
             if self.election_type == "ref":
                 raise ValueError(
-                    "election_type %s may not have a by-election" % (self.election_type)
+                    "election_type %s may not have a by-election"
+                    % (self.election_type)
                 )
             self.contest_type = "by"
         return self
 
     def _validate_election_type(self, election_type):
         if election_type not in ELECTION_TYPES:
             raise ValueError(
                 "Allowed values for election_type are %s"
                 % (str(list(ELECTION_TYPES.keys())))
             )
         return True
 
     def _validate_subtype(self, subtype):
-        if isinstance(self.spec.subtypes, tuple) and subtype not in self.spec.subtypes:
+        if (
+            isinstance(self.spec.subtypes, tuple)
+            and subtype not in self.spec.subtypes
+        ):
             raise ValueError(
                 "Allowed values for subtype are %s" % (str(self.spec.subtypes))
             )
         if not self.spec.subtypes and subtype:
             raise ValueError(
                 "election_type %s may not have a subtype" % (self.election_type)
             )
         return True
 
     def _validate_organisation(self, organisation):
         if not self.spec.can_have_orgs and organisation:
             raise ValueError(
-                "election_type %s may not have an organisation" % (self.election_type)
+                "election_type %s may not have an organisation"
+                % (self.election_type)
             )
         return True
 
     def _validate_division(self, division):
         try:
             can_have_divs = self._can_have_divs
         except KeyError:
             raise ValueError(
                 "election_type %s must have a valid subtype before setting a division"
                 % (self.election_type)
             )
         if not can_have_divs and division:
             raise ValueError(
-                "election_type %s may not have a division" % (self.election_type)
+                "election_type %s may not have a division"
+                % (self.election_type)
             )
         return True
 
     def _validate_contest_type(self, contest_type):
         if not contest_type:
             return True
-        if not contest_type.lower() in CONTEST_TYPES:
+        if contest_type.lower() not in CONTEST_TYPES:
             raise ValueError(
-                "Allowed values for contest_type are %s" % (str(list(CONTEST_TYPES)))
+                "Allowed values for contest_type are %s"
+                % (str(list(CONTEST_TYPES)))
             )
         return True
 
     def _validate(self):
         # validation checks necessary to create any id
         self._validate_election_type(self.election_type)
         self._validate_organisation(self.organisation)
@@ -231,19 +239,21 @@
         parts.append(self.election_type)
         parts.append(self.date)
         return ".".join(parts)
 
     def _validate_for_subtype_group_id(self):
         if not isinstance(self.spec.subtypes, tuple):
             raise ValueError(
-                "Can't create subtype id for election_type %s" % (self.election_type)
+                "Can't create subtype id for election_type %s"
+                % (self.election_type)
             )
         if isinstance(self.spec.subtypes, tuple) and not self.subtype:
             raise ValueError(
-                "Subtype must be specified for election_type %s" % (self.election_type)
+                "Subtype must be specified for election_type %s"
+                % (self.election_type)
             )
         self._validate_subtype(self.subtype)
         return True
 
     @property
     def subtype_group_id(self):
         """
@@ -258,15 +268,16 @@
         parts.append(self.date)
         return ".".join(parts)
 
     def _validate_for_organisation_group_id(self):
         # validation checks specifically relevant to creating an organisation group id
         if isinstance(self.spec.subtypes, tuple) and not self.subtype:
             raise ValueError(
-                "Subtype must be specified for election_type %s" % (self.election_type)
+                "Subtype must be specified for election_type %s"
+                % (self.election_type)
             )
         self._validate_subtype(self.subtype)
         if not self.spec.can_have_orgs:
             raise ValueError(
                 "election_type %s can not have an organisation group id"
                 % (self.election_type)
             )
@@ -293,15 +304,16 @@
         parts.append(self.date)
         return ".".join(parts)
 
     def _validate_for_ballot_id(self):
         # validation checks specifically relevant to creating a ballot id
         if isinstance(self.spec.subtypes, tuple) and not self.subtype:
             raise ValueError(
-                "Subtype must be specified for election_type %s" % (self.election_type)
+                "Subtype must be specified for election_type %s"
+                % (self.election_type)
             )
         self._validate_subtype(self.subtype)
         if self.spec.can_have_orgs and not self.organisation:
             raise ValueError(
                 "election_type %s must have an organisation in order to create a ballot id"
                 % (self.election_type)
             )
@@ -337,30 +349,24 @@
     @property
     def ids(self):
         """
         list[str]: All applicable IDs
         """
         ids = []
 
-        try:
+        with contextlib.suppress(ValueError):
             ids.append(self.election_group_id)
-        except ValueError:
-            pass
 
         if isinstance(self.spec.subtypes, tuple):
-            try:
+            with contextlib.suppress(ValueError):
                 ids.append(self.subtype_group_id)
-            except ValueError:
-                pass
 
         if self.spec.can_have_orgs:
-            try:
+            with contextlib.suppress(ValueError):
                 ids.append(self.organisation_group_id)
-            except ValueError:
-                pass
 
         try:
             if self.ballot_id not in ids:
                 ids.append(self.ballot_id)
         except ValueError:
             pass
 
@@ -417,15 +423,15 @@
         if len(id_parts) == 0:
             return builder
 
         try:
             # use the builder object to validate the remaining parts,
             # popping as we go
             if id_parts[-1] == "by":
-                contest_type = id_parts.pop(-1)
+                id_parts.pop(-1)
                 builder = builder.with_contest_type("by")
             if builder.spec.subtypes:
                 subtype = id_parts.pop(0)
                 builder = builder.with_subtype(subtype)
             if id_parts and builder.spec.can_have_orgs:
                 org = id_parts.pop(0)
                 builder = builder.with_organisation(org)
```

### Comparing `uk_election_ids-0.7.2/uk_election_ids/metadata_tools.py` & `uk_election_ids-0.7.3/uk_election_ids/metadata_tools.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,19 +10,18 @@
     Given an election ID and optional nation, match to
     a data file to get additional properties about the ID.
 
     The data file is in the election ID metadata format specified in test/data_schema.py
     """
 
     def __init__(
-            self,
-            election_id: str,
-            nation: Optional[str] = None,
+        self,
+        election_id: str,
+        nation: Optional[str] = None,
     ) -> None:
-
         self.nation = nation
         self.election_id = election_id
         self.parts = self.election_id.split(".")
         self.date = self._parse_date(self.parts[-1])
 
     DATA = {"defaults": {}}
 
@@ -35,15 +34,17 @@
         Additionally, if wildcard is empty, regex needs reduced '.' literals .
 
         i.e. 'parl.*.by' becomes the slightly more esoteric 'parl(\..*)?\.by' where:
         \. represents a literal '.', always present at the start of a wildcard
         (\..*) captures a sequence of "[any characters]."
         ? captures a group between 0-1 times
         """
-        id_part = id_part.replace("-", r"\-")  # prevent '-' from being interpreted as range indicator
+        id_part = id_part.replace(
+            "-", r"\-"
+        )  # prevent '-' from being interpreted as range indicator
         id_part = id_part.replace(".*.", r"\.(.*\.)?")
         return id_part
 
     def match_id(self):
         """
         Match the most specific key to this ID
 
@@ -54,56 +55,56 @@
             key=lambda identifier: identifier.count("."),
             reverse=True,
         )
         matched_id_pattern = None
         matched_default_value = None
 
         for id_part in ids_with_defaults:
-            pattern = re.compile(fr"""
+            pattern = re.compile(
+                rf"""
                 ^                                   # String begins with id_part
                 ({self._escape_id_part(id_part)})   # e.g. parl.*.by, local, etc. - the bit we're interested in matching
                 (\..*|$)                            # id_part is followed by '.[any characters]' or nothing
-            """, re.VERBOSE)
+            """,
+                re.VERBOSE,
+            )
 
             if bool(pattern.search(self.election_id)):
                 matched_id_pattern = id_part
                 matched_default_value = self.DATA["defaults"].get(id_part)
                 break
 
         return (matched_id_pattern, matched_default_value)
 
     def _parse_date(self, date: Optional[str]) -> datetime.date:
         if not date:
             return None
         return datetime.datetime.strptime(date, "%Y-%m-%d").date()
 
     def match_dates(self, data):
-
         for key, value in data.items():
             start, end = [self._parse_date(x) for x in key.split(":")]
             if not start:
                 start = datetime.date(year=1, month=1, day=1)
             if not end:
                 end = datetime.date(year=9999, month=12, day=31)
 
-            if self.date >= start:
-                if self.date < end:
-                    return value
+            if self.date >= start and self.date < end:
+                return value
         raise ValueError("No date for range")
 
 
 class VotingSystemMatcher(MetaDataMatcher):
     path = Path(__file__).parent / "data" / "voting_systems.json"
     DATA = json.load(path.open())
 
     def get_voting_system(self):
         id_part, data = self.match_id()
-        if self.nation:
-            if self.nation in data.get("nations", {}):
-                data = data["nations"][self.nation]
+        if self.nation and self.nation in data.get("nations", {}):
+            data = data["nations"][self.nation]
 
         if data.get("dates"):
             data = self.match_dates(data["dates"])
 
         default = data.get("default", None)
         if not default:
             required_keys = data.keys()
@@ -114,17 +115,16 @@
 
 class IDRequirementsMatcher(MetaDataMatcher):
     path = Path(__file__).parent / "data" / "id_requirements.json"
     DATA = json.load(path.open())
 
     def get_id_requirements(self):
         id_part, data = self.match_id()
-        if self.nation:
-            if self.nation in data.get("nations", {}):
-                data = data["nations"][self.nation]
+        if self.nation and self.nation in data.get("nations", {}):
+            data = data["nations"][self.nation]
 
         if data.get("dates"):
             data = self.match_dates(data["dates"])
 
         default = data.get("default", "")
         if default == "":
             required_keys = data.keys()
```

### Comparing `uk_election_ids-0.7.2/uk_election_ids/parser.py` & `uk_election_ids-0.7.3/uk_election_ids/parser.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from collections import namedtuple
 
-
 IdSpec = namedtuple("IdSpec", ["subtypes", "can_have_orgs", "can_have_divs"])
 
 
 class DataPackageParser:
 
     """
     Parser which uses the data in datapackage.py to build
@@ -13,34 +12,34 @@
     """
 
     def __init__(self, data):
         self.data = data
 
     def build_subtypes(self, record):
         if record["subtypes"]:
-            return tuple(subtype["election_subtype"] for subtype in record["subtypes"])
+            return tuple(
+                subtype["election_subtype"] for subtype in record["subtypes"]
+            )
         return None
 
     def build_can_have_orgs(self, record):
         if "can_have_orgs" in record:
             return record["can_have_orgs"]
-        else:
-            return {
-                subtype["election_subtype"]: subtype["can_have_orgs"]
-                for subtype in record["subtypes"]
-            }
+        return {
+            subtype["election_subtype"]: subtype["can_have_orgs"]
+            for subtype in record["subtypes"]
+        }
 
     def build_can_have_divs(self, record):
         if "can_have_divs" in record:
             return record["can_have_divs"]
-        else:
-            return {
-                subtype["election_subtype"]: subtype["can_have_divs"]
-                for subtype in record["subtypes"]
-            }
+        return {
+            subtype["election_subtype"]: subtype["can_have_divs"]
+            for subtype in record["subtypes"]
+        }
 
     def build_rules(self):
         rules = {}
         for key, record in self.data.items():
             subtypes = self.build_subtypes(record)
             can_have_orgs = self.build_can_have_orgs(record)
             can_have_divs = self.build_can_have_divs(record)
```

### Comparing `uk_election_ids-0.7.2/uk_election_ids/slugger.py` & `uk_election_ids-0.7.3/uk_election_ids/slugger.py`

 * *Files identical despite different names*

### Comparing `uk_election_ids-0.7.2/uk_election_ids.egg-info/PKG-INFO` & `uk_election_ids-0.7.3/uk_election_ids.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uk-election-ids
-Version: 0.7.2
+Version: 0.7.3
 Summary: Create Democracy Club Election Identifiers
 Home-page: https://github.com/DemocracyClub/uk-election-ids/
 Author: chris48s
 License: MIT
 Project-URL: Documentation, https://democracyclub.github.io/uk-election-ids/
 Project-URL: Source, https://github.com/DemocracyClub/uk-election-ids/
 Classifier: License :: OSI Approved :: MIT License
```

