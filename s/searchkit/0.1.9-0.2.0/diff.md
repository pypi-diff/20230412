# Comparing `tmp/searchkit-0.1.9.tar.gz` & `tmp/searchkit-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "searchkit-0.1.9.tar", last modified: Fri Jan 27 18:58:57 2023, max compression
+gzip compressed data, was "searchkit-0.2.0.tar", last modified: Wed Apr 12 11:04:56 2023, max compression
```

## Comparing `searchkit-0.1.9.tar` & `searchkit-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-01-27 18:58:57.090677 searchkit-0.1.9/
--rw-rw-r--   0 user1     (1000) user1     (1000)    11357 2023-01-10 10:19:33.000000 searchkit-0.1.9/LICENSE
--rw-rw-r--   0 user1     (1000) user1     (1000)      142 2023-01-27 18:58:57.090677 searchkit-0.1.9/PKG-INFO
--rw-rw-r--   0 user1     (1000) user1     (1000)      276 2023-01-27 18:58:39.000000 searchkit-0.1.9/pyproject.toml
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-01-27 18:58:57.090677 searchkit-0.1.9/searchkit/
--rw-rw-r--   0 user1     (1000) user1     (1000)      100 2023-01-27 10:33:34.000000 searchkit-0.1.9/searchkit/__init__.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    22684 2023-01-27 10:33:34.000000 searchkit-0.1.9/searchkit/constraints.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      277 2023-01-27 16:02:47.000000 searchkit-0.1.9/searchkit/log.py
--rwxrwxr-x   0 user1     (1000) user1     (1000)    30778 2023-01-27 18:57:39.000000 searchkit-0.1.9/searchkit/search.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     2730 2023-01-24 13:08:12.000000 searchkit-0.1.9/searchkit/utils.py
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-01-27 18:58:57.090677 searchkit-0.1.9/searchkit.egg-info/
--rw-rw-r--   0 user1     (1000) user1     (1000)      142 2023-01-27 18:58:57.000000 searchkit-0.1.9/searchkit.egg-info/PKG-INFO
--rw-rw-r--   0 user1     (1000) user1     (1000)      298 2023-01-27 18:58:57.000000 searchkit-0.1.9/searchkit.egg-info/SOURCES.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)        1 2023-01-27 18:58:57.000000 searchkit-0.1.9/searchkit.egg-info/dependency_links.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)       47 2023-01-27 18:58:57.000000 searchkit-0.1.9/searchkit.egg-info/requires.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)       10 2023-01-27 18:58:57.000000 searchkit-0.1.9/searchkit.egg-info/top_level.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)       38 2023-01-27 18:58:57.090677 searchkit-0.1.9/setup.cfg
--rw-rw-r--   0 user1     (1000) user1     (1000)       54 2023-01-24 13:08:12.000000 searchkit-0.1.9/setup.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-04-12 11:04:56.827556 searchkit-0.2.0/
+-rw-rw-r--   0 user1     (1000) user1     (1000)    11357 2023-01-10 10:19:33.000000 searchkit-0.2.0/LICENSE
+-rw-rw-r--   0 user1     (1000) user1     (1000)     3103 2023-04-12 11:04:56.827556 searchkit-0.2.0/PKG-INFO
+-rw-rw-r--   0 user1     (1000) user1     (1000)     2897 2023-04-12 11:04:01.000000 searchkit-0.2.0/README.md
+-rw-rw-r--   0 user1     (1000) user1     (1000)      335 2023-04-12 11:04:37.000000 searchkit-0.2.0/pyproject.toml
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-04-12 11:04:56.827556 searchkit-0.2.0/searchkit/
+-rw-rw-r--   0 user1     (1000) user1     (1000)      100 2023-01-29 21:35:16.000000 searchkit-0.2.0/searchkit/__init__.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    22833 2023-04-11 08:53:59.000000 searchkit-0.2.0/searchkit/constraints.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      277 2023-01-29 21:35:16.000000 searchkit-0.2.0/searchkit/log.py
+-rwxrwxr-x   0 user1     (1000) user1     (1000)    43588 2023-04-12 11:04:01.000000 searchkit-0.2.0/searchkit/search.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     4406 2023-04-11 08:53:59.000000 searchkit-0.2.0/searchkit/utils.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-04-12 11:04:56.827556 searchkit-0.2.0/searchkit.egg-info/
+-rw-rw-r--   0 user1     (1000) user1     (1000)     3103 2023-04-12 11:04:56.000000 searchkit-0.2.0/searchkit.egg-info/PKG-INFO
+-rw-rw-r--   0 user1     (1000) user1     (1000)      308 2023-04-12 11:04:56.000000 searchkit-0.2.0/searchkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)        1 2023-04-12 11:04:56.000000 searchkit-0.2.0/searchkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)       57 2023-04-12 11:04:56.000000 searchkit-0.2.0/searchkit.egg-info/requires.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)       10 2023-04-12 11:04:56.000000 searchkit-0.2.0/searchkit.egg-info/top_level.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)       38 2023-04-12 11:04:56.827556 searchkit-0.2.0/setup.cfg
+-rw-rw-r--   0 user1     (1000) user1     (1000)       54 2023-01-29 21:35:16.000000 searchkit-0.2.0/setup.py
```

### Comparing `searchkit-0.1.9/LICENSE` & `searchkit-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `searchkit-0.1.9/searchkit/constraints.py` & `searchkit-0.2.0/searchkit/constraints.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,15 +211,15 @@
         self.fd = fd
         self.iterations = 0
         self._orig_pos = self.fd.tell()
         if cache_path is None:
             cache_path = tempfile.mkdtemp()
 
         self.cache = MPCache('file_markers_{}'.format(self.fname_hash),
-                             'search_constraints', tmp_dir=cache_path)
+                             'search_constraints', cache_path)
 
     @cached_property
     def fname_hash(self):
         hash = hashlib.sha256()
         hash.update(self.fd.name.encode('utf-8'))
         return hash.hexdigest()
 
@@ -310,25 +310,53 @@
 class BinarySeekSearchBase(ConstraintBase):
     """
     Provides a way to seek to a point in a file using a binary search and a
     given condition.
     """
 
     def __init__(self, allow_constraints_for_unverifiable_logs=True):
+        self.fd_info = None
         self.allow_unverifiable_logs = allow_constraints_for_unverifiable_logs
 
     @abc.abstractmethod
     def extracted_datetime(self, line):
         """
         Extract datetime from line. Returns a datetime object or None if unable
         to extract one from the line.
 
         @param line: text line to extract a datetime from.
         """
 
+    @abc.abstractproperty
+    def _since_date(self):
+        """ A datetime.datetime object representing the "since" date/time """
+
+    def _line_date_is_valid(self, extracted_datetime):
+        """
+        Validate if the given line falls within the provided constraint. In
+        this case that's whether it has a datetime that is >= to the "since"
+        date.
+        """
+        ts = extracted_datetime
+        if ts is None:
+            # log.info("s:%s: failed to extract datetime from "
+            #          "using expressions %s - assuming line is not valid",
+            #          unique_search_id, ', '.join(self.exprs))
+            return False
+
+        if ts < self._since_date:
+            # log.debug("%s < %s at (%s) i.e. False", ts, self._since_date,
+            #           line[-3:].strip())
+            return False
+
+        # log.debug("%s >= %s at (%s) i.e. True", ts, self._since_date,
+        #           line[-3:].strip())
+
+        return True
+
     def _seek_and_validate(self, datetime_obj):
         """
         Seek to position and validate. If the line at pos is valid the new
         position is returned otherwise None.
 
         NOTE: this operation is destructive and will always point to the next
               line after being called.
@@ -520,15 +548,14 @@
         @param days: override default period with number of days
         @param hours: override default period with number of hours
         """
         super().__init__(**kwargs)
         self.cache_path = cache_path
         self.date_format = '%Y-%m-%d %H:%M:%S'
         self.current_date = datetime.strptime(current_date, self.date_format)
-        self.fd_info = None
         self._line_pass = 0
         self._line_fail = 0
         self.exprs = exprs
         self.days = days
         if days:
             self.hours = 0
         else:
@@ -571,47 +598,24 @@
             log.exception("")
 
     @property
     def _is_valid(self):
         return self._since_date is not None
 
     @cached_property
-    def _since_date(self):
+    def _since_date(self):  # pylint: disable=W0236
         """
         Reflects the date from which we will start to apply searches.
         """
         if not self.current_date:
             return
 
         return self.current_date - timedelta(days=self.days,
                                              hours=self.hours or 0)
 
-    def _line_date_is_valid(self, extracted_datetime):
-        """
-        Validate if the given line falls within the provided constraint. In
-        this case that's whether it has a datetime that is >= to the "since"
-        date.
-        """
-        ts = extracted_datetime
-        if ts is None:
-            # log.info("s:%s: failed to extract datetime from "
-            #          "using expressions %s - assuming line is not valid",
-            #          unique_search_id, ', '.join(self.exprs))
-            return False
-
-        if ts < self._since_date:
-            # log.debug("%s < %s at (%s) i.e. False", ts, self._since_date,
-            #           line[-3:].strip())
-            return False
-
-        # log.debug("%s >= %s at (%s) i.e. True", ts, self._since_date,
-        #           line[-3:].strip())
-
-        return True
-
     def apply_to_line(self, line):
         if not self._is_valid:
             log.warning("c:%s unable to apply constraint to line", self.id)
             self._line_pass += 1
             return True
 
         extracted_datetime = self.extracted_datetime(line)
```

### Comparing `searchkit-0.1.9/searchkit/search.py` & `searchkit-0.2.0/searchkit/search.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,192 +1,305 @@
 import abc
+import concurrent.futures
 import glob
 import gzip
 import multiprocessing
 import os
 import queue
 import re
 import signal
+import subprocess
 import threading
+import time
 import uuid
 
 from functools import cached_property
-from collections import UserDict
+from collections import UserDict, UserList
 
 from searchkit.log import log
 
-RESULTS_QUEUES = {}
 RESULTS_QUEUE_TIMEOUT = 60
+MAX_QUEUE_RETRIES = 10
 
 
 class FileSearchException(Exception):
     def __init__(self, msg):
         self.msg = msg
 
 
 class SearchDefBase(object):
 
     def __init__(self, constraints=None):
+        """
+        @param constraints: an optional list of constraints to apply to
+                            results.
+        """
         self.id
         self.constraints = {c.id: c for c in constraints or {}}
 
     @cached_property
     def id(self):
-        """
-        A unique identifier for this search definition.
-        """
+        """ A unique identifier for this search definition. """
         return str(uuid.uuid4())
 
 
 class SearchDef(SearchDefBase):
 
     def __init__(self, pattern, tag=None, hint=None,
-                 store_result_contents=True, **kwargs):
+                 store_result_contents=True, field_info=None, **kwargs):
         """
-        Add a search definition.
+        Simple search definition.
 
-        @param pattern: regex pattern or list of patterns to search for
-        @param tag: optional user-friendly identifier for this search term
-        @param hint: pre-search term to speed things up
+        @param pattern: pattern or list of patterns to search for
+        @param tag: optional user-friendly identifier for this search term.
+                    This is useful for retrieving results.
+        @param hint: optional pre-search term. If provided, this is expected to
+                     match in order for the main search to be executed.
         @param store_result_contents: by default the content of a search result
                                       is saved but if it is not needed this
                                       can be set to False. This effectively
                                       makes the result True/False.
+        @param field_info: optional ResultFieldInfo object
         """
         if type(pattern) != list:
             self.patterns = [re.compile(pattern)]
         else:
             self.patterns = []
             for _pattern in pattern:
                 self.patterns.append(re.compile(_pattern))
 
         self.store_result_contents = store_result_contents
         self.tag = tag
+        self.field_info = field_info
+        self.hint = hint
         if hint:
             self.hint = re.compile(hint)
-        else:
-            self.hint = None
+
+        self.sequence_def = None
 
         # do this last
         super().__init__(**kwargs)
 
+    def link_to_sequence(self, sequence_def, tag):
+        """
+        If this search definition is part of a sequence, the parent
+        SequenceSearchDef must link itself to this object.
+
+        @param sequence_def: SequenceSearchDef object
+        @param tag: SequenceSearchDef object tag for this section def
+        """
+        self.sequence_def = sequence_def
+        self.tag = tag
+
     def run(self, line):
-        """Execute search patterns against line and return first match."""
+        """ Execute search patterns against line and return first match. """
         if self.hint:
             ret = self.hint.search(line)
             if not ret:
                 return None
 
         ret = None
         for pattern in self.patterns:
             ret = pattern.match(line)
             if ret:
-                return ret
+                break
 
         return ret
 
 
 class SequenceSearchDef(SearchDefBase):
 
     def __init__(self, start, tag, end=None, body=None, **kwargs):
         """
-        Define search for sequences. A sequence must match a start and end with
-        optional body in between. If no end defined, the sequence ends with
-        the start of the next or EOF.
+        Sequence search definition.
+
+        A sequence must match a start and end with optional body in between.
+        If no end is defined, the sequence ends with the start of the next or
+        EOF.
 
         NOTE: sequences must not overlap. This is therefore not suitable for
         finding sequences generated by parallel/concurrent tasks.
 
         @param start: SearchDef object for matching start
         @param tag: tag used to identify this sequence definition
         @param end: optional SearchDef object for matching end
         @param body: optional SearchDef object for matching body
         """
+        self.tag = tag
         self.s_start = start
         self.s_end = end
         self.s_body = body
-        self.tag = tag
+
+        # make sure section defs have tags synced with this object
+        for sd, _tag in {start: self.start_tag,
+                         end: self.end_tag,
+                         body: self.body_tag}.items():
+            if sd:
+                sd.link_to_sequence(self, _tag)
+
         self._mark = None
-        # Each section identified gets its own id. Since each file is processed
+        # Each section matched gets its own id. Since each file is processed
         # using a separate process and memory is not shared, these values must
         # be unique to avoid collisions when results are aggregated.
         self._section_id = None
+        self.completed_sections = []
         # do this last
         super().__init__(**kwargs)
 
     @property
     def start_tag(self):
-        """Tag used to identify start of section"""
+        """ Tag used to identify start of section. """
         return "{}-start".format(self.tag)
 
     @property
     def end_tag(self):
-        """Tag used to identify end of section"""
+        """ Tag used to identify end of section. """
         return "{}-end".format(self.tag)
 
     @property
     def body_tag(self):
-        """Tag used to identify body of section"""
+        """ Tag used to identify body of section. """
         return "{}-body".format(self.tag)
 
     @property
-    def section_id(self):
+    def current_section_id(self):
         """ ID of current section. A new id should be set after each
         completed section. """
         return self._section_id
 
     @property
     def started(self):
-        """Indicate a section sequence has been started."""
+        """ Indicate a section sequence has been started. """
         return self._mark == 1
 
     def start(self):
-        """Indicate that a sequence start has been detected."""
+        """ Indicate that a sequence start has been detected. """
         self._section_id = str(uuid.uuid4())
+        log.debug("sequence %s started section %s (completed=%s)",
+                  self.id, self.current_section_id,
+                  len(self.completed_sections))
         self._mark = 1
 
     def reset(self):
-        """Used to restart a section. This is used e.g. if the start
+        """ Used to restart a section. This is used e.g. if the start
         expression matches midway through a sequence (and before the end).
         """
         self._mark = 0
 
     def stop(self):
-        """Indicate that a sequence is complete."""
+        """ Indicate that a sequence is complete. """
         self._mark = 0
+        if self.current_section_id is None:
+            raise FileSearchException("sequence section id is None")
+
+        self.completed_sections.append(self.current_section_id)
+        log.debug("sequence %s stopping section %s (completed=%s)",
+                  self.id, self.current_section_id,
+                  len(self.completed_sections))
         self._section_id = str(uuid.uuid4())
 
+    def __repr__(self):
+        return ("{}: current_section={}, started={}, completed_sections={}".
+                format(self.__class__.__name__, self.current_section_id,
+                       self.started, self.completed_sections))
+
+
+class SequenceSearchResults(UserDict):
+
+    def __init__(self):
+        self.data = {}
+
+    def add(self, result):
+        id = result.sequence_def.id
+        if id in self.data:
+            self.data[id].append(result)
+        else:
+            self.data[id] = [result]
+
+    def remove(self, id):
+        if id in self.data:
+            del self.data[id]
+
 
 class SearchResultPart(object):
 
-    def __init__(self, index, value):
+    def __init__(self, index, value, field_info=None):
+        """
+        @param index: index of this result
+        @param value: value of this result
+        @param field_info: ResultFieldInfo object
+        """
         self.index = index
         self.value = value
+        if field_info:
+            self.name = field_info.index_to_name(index - 1)
+            self.value = field_info.ensure_type(self.name, value)
+        else:
+            self.name = None
 
 
-class SearchResult(object):
+class ResultFieldInfo(UserDict):
 
-    def __init__(self, linenumber, source_id, result, search_term_tag=None,
-                 section_id=None, sequence_obj_id=None, store_contents=True):
+    def __init__(self, fields):
         """
-        @param linenumber: line number that produced a match
-        @param source_id: data source id
-        @param result: python.re match object
-        @param search_term_tag: SearchDef object tag
-        @param section_id: SequenceSearchDef object section id
-        @param sequence_obj_id: SequenceSearchDef object unique id
+        @param fields: list or dictionary of field names. If a dictionary is
+                       provided, the values are expected to be functions that
+                       the field value will be cast to. In other words these
+                       should typically be standard or custom types.
         """
-        self.tag = search_term_tag
-        self.source_id = source_id
+        if type(fields) == dict:
+            self.data = fields
+        else:
+            self.data = {f: None for f in fields}
+
+    def ensure_type(self, name, value):
+        """
+        If our fields have associated type functions, cast the value to
+        its expected type.
+        """
+        if name not in self.data or self.data[name] is None:
+            return value
+
+        return self.data[name](value)
+
+    def index_to_name(self, index):
+        """ Retrieve a field name using the result group index. """
+        for i, _field in enumerate(self.data):
+            if index == i:
+                return _field
+
+        raise FileSearchException("field with index {} not found in mapping".
+                                  format(index))
+
+
+class SearchResult(UserList):
+
+    def __init__(self, linenumber, source_id, result, search_def,
+                 sequence_section_id=None):
+        """
+        @param linenumber: line number that produced a match.
+        @param source_id: data source id - resolves to a path in the
+                          SearchCatalog.
+        @param result: python.re.match object.
+        @param search_def: SearchDef object.
+        @param sequence_section_id: if this result is part of a sequence the
+                                    section ID must be provided.
+        """
+        self.data = []
         self.linenumber = linenumber
-        self._parts = {}
-        self.sequence_obj_id = sequence_obj_id
-        self.section_id = section_id
+        self.source_id = source_id
+        self.tag = search_def.tag
+        self.section_id = sequence_section_id
+        self.sequence_def = search_def.sequence_def
+        if self.sequence_def and sequence_section_id is None:
+            raise FileSearchException("sequence section result saved "
+                                      "but no section id provided")
+        self.field_info = search_def.field_info
 
-        if not store_contents:
+        if not search_def.store_result_contents:
             log.debug("store_contents is False - skipping save")
             return
 
         num_groups = len(result.groups())
         # NOTE: this does not include group(0)
         if num_groups:
             # To reduce memory footprint, don't store group(0) i.e. the whole
@@ -194,118 +307,189 @@
             for i in range(1, num_groups + 1):
                 self._add(i, result.group(i))
         else:
             log.debug("saving full search result which can lead to high "
                       "memory usage")
             self._add(0, result.group(0))
 
+    @cached_property
+    def id(self):
+        """ Unique Result ID """
+        id_string = "{}-{}-{}".format(uuid.uuid4(), self.source_id,
+                                      self.linenumber)
+        if self.sequence_def:
+            id_string = "{}-{}-{}".format(id_string,
+                                          self.sequence_def.id,
+                                          self.section_id)
+        return id_string
+
     def _add(self, index, value):
-        self._parts[index] = SearchResultPart(index, value)
+        self.data.append(SearchResultPart(index, value, self.field_info))
 
-    def get(self, index):
-        """Retrieve a result part by its index."""
-        if index not in self._parts:
-            return None
+    def get(self, field):
+        """
+        Retrieve result part value by index or name.
 
-        return self._parts[index].value
+        @param field: integer index of string field name.
+        """
+        for group in self.data:
+            if type(field) == str:
+                if group.name == field:
+                    return group.value
+            else:
+                if group.index == field:
+                    return group.value
 
-    def __len__(self):
-        return len(self._parts)
+    def __getattr__(self, name):
+        if name != 'field_info':
+            if self.field_info and name in self.field_info:
+                return self.get(name)
+
+        raise AttributeError("'{}' object has no attribute '{}'".
+                             format(self.__class__.__name__, name))
 
     def __iter__(self):
-        for idx in sorted(self._parts.keys()):
-            yield self._parts[idx].value
+        """ Only return part values when iterating over this object. """
+        for part in self.data:
+            yield part.value
 
     def __repr__(self):
-        r_list = ["{}={}".format(k, v.value) for k, v in self._parts.items()]
-        return "ln:{} ".format(self.linenumber) + ", ".join(r_list)
+        r_list = ["{}='{}'".format(rp.index, rp.value) for rp in self.data]
+        return ("ln:{} {} (section={})".
+                format(self.linenumber, ", ".join(r_list),
+                       self.section_id))
 
 
-class SearchResultsCollection(object):
+class SearchResultsCollection(UserDict):
 
     def __init__(self, search_catalog):
         self.search_catalog = search_catalog
         self.reset()
 
-    def __len__(self):
-        _count = 0
-        for f in self.files:
-            _count += len(self.find_by_path(f))
-
-        return _count
-
     @property
-    def files(self):
-        return list(self._results.keys())
+    def data(self):
+        results = {}
+        for path, ids in self._results_by_path.items():
+            results[path] = [self._results_by_id[id] for id in ids]
+
+        return results
 
     def reset(self):
         self._iter_idx = 0
-        self._results = {}
+        self._results_by_path = {}
+        self._results_by_id = {}
+
+    @property
+    def files(self):
+        return list(self._results_by_path.keys())
 
     def add(self, result):
         # resolve
         path = self.search_catalog.source_id_to_path(result.source_id)
-        if path not in self._results:
-            self._results[path] = [result]
+        self._results_by_id[result.id] = result
+        if path not in self._results_by_path:
+            self._results_by_path[path] = [result.id]
         else:
-            self._results[path].append(result)
+            self._results_by_path[path].append(result.id)
 
     def find_by_path(self, path):
-        if path not in self._results:
-            return []
+        """ Return results for a given path. """
+        results = self._results_by_path.get(path, [])
+        return [self._results_by_id[id] for id in results]
+
+    def find_by_tag(self, tag, path=None):
+        """ Return results matched by tag.
+
+        @param tag: tag used to identify search results.
+        @param path: optional path used to filter results to only include those
+                     matched from a given path.
+        """
+        if path:
+            paths = [path]
+        else:
+            paths = list(self._results_by_path.keys())
 
-        return self._results[path]
+        results = []
+        for path in paths:
+            for result in self.find_by_path(path):
+                if result.tag != tag:
+                    continue
 
-    def find_by_tag(self, tag, path=None, sequence_obj_id=None):
-        """Return all result tagged with tag.
+                results.append(result)
 
-        If no path is provided tagged results from all paths are returned.
+        return results
+
+    def _get_all_sequence_results(self, path=None):
+        """ Return a list of ids for all sequence match results.
+
+        @param path: optionally filter results for a given path.
         """
         if path:
             paths = [path]
         else:
-            paths = list(self._results.keys())
+            paths = list(self._results_by_path.keys())
 
-        results = []
+        sequences = []
         for path in paths:
-            for result in self._results.get(path, []):
-                if sequence_obj_id is None:
-                    if result.tag == tag:
-                        results.append(result)
-                else:
-                    if (result.tag == tag and
-                            result.sequence_obj_id == sequence_obj_id):
-                        results.append(result)
+            for result in self.find_by_path(path):
+                if result.sequence_def is None:
+                    continue
 
-        return results
+                sequences.append(result.id)
 
-    def find_sequence_sections(self, sequence_obj, path=None):
-        """Return results of running the given sequence search.
+        return sequences
+
+    def find_sequence_by_tag(self, tag, path=None):
+        """ Find results for the sequence search(es) identified from tag.
 
-        Returns a dictionary keyed by section id where each is a list of
-        results for that section with start, body, end etc.
+        Returns a dictionary of "sections" i.e. complete sequences matched
+        using associated SequenceSearchDef objects. Each section is a list of
+        SearchResult objects representing start/body/end for that section.
+
+        @param tag: tag used to identify sequence results.
+        @param path: optionally filter results for a given path.
         """
-        _results = []
         sections = {}
-        _results += self.find_by_tag(tag=sequence_obj.start_tag, path=path,
-                                     sequence_obj_id=sequence_obj.id)
-        _results += self.find_by_tag(tag=sequence_obj.body_tag, path=path,
-                                     sequence_obj_id=sequence_obj.id)
-        _results += self.find_by_tag(tag=sequence_obj.end_tag, path=path,
-                                     sequence_obj_id=sequence_obj.id)
-        for r in _results:
-            if r.section_id in sections:
-                sections[r.section_id].append(r)
-            else:
-                sections[r.section_id] = [r]
+        for seq_obj in self.search_catalog.resolve_from_tag(tag):
+            sections.update(self.find_sequence_sections(seq_obj, path))
 
         return sections
 
-    def __iter__(self):
-        return iter(self._results.items())
+    def find_sequence_sections(self, sequence_obj, path=None):
+        """ Find results for the given sequence search.
+
+        Returns a dictionary of "sections" i.e. complete sequences matched
+        using the associated SequenceSearchDef object. Each section is a list
+        of SearchResult objects representing start/body/end for that section.
+
+        @param sequence_obj: SequenceSearch object
+        @param path: optionally filter results for a given path.
+        """
+        _results = {}
+        for r in self._get_all_sequence_results(path=path):
+            result = self._results_by_id[r]
+            s_id = result.sequence_def.id
+            if s_id != sequence_obj.id:
+                continue
+
+            section_id = result.section_id
+            if section_id not in _results:
+                _results[section_id] = []
+
+            _results[section_id].append(result)
+
+        return _results
+
+    def __len__(self):
+        """ Returns total number of search results. """
+        _count = 0
+        for f in self.files:
+            _count += len(self.find_by_path(f))
+
+        return _count
 
 
 class LogrotateLogSort(object):
 
     def __call__(self, fname):
         """
         Sort contents of a directory by passing the function as the key to a
@@ -328,24 +512,69 @@
         if len(ret.groups()) == 0:
             return 0
 
         return int(ret.group(1))
 
 
 class SearchCatalog(object):
+
     def __init__(self, max_logrotate_depth=7):
         self.max_logrotate_depth = max_logrotate_depth
-        self.user_paths = {}
+        self._user_paths = {}
         self._source_ids = {}
+        self._search_tags = {}
+        self._simple_searches = {}
+        self._sequence_searches = {}
 
     def register(self, search, user_path):
-        if user_path in self.user_paths:
-            self.user_paths[user_path].append(search)
+        """
+        Register a search against a path.
+
+        The same search can be registered against more than one path.
+
+        @param search: object implemented from SearchDefBase.
+        @param user_path: directory or file path.
+        """
+        if search.tag is not None:
+            if search.tag in self._search_tags:
+                if search.id not in self._search_tags[search.tag]:
+                    log.debug("one or more search tagged '%s' has already "
+                              "been registered against path '%s'",
+                              search.tag, user_path)
+                    self._search_tags[search.tag].append(search.id)
+            else:
+                self._search_tags[search.tag] = [search.id]
+
+        if isinstance(search, SequenceSearchDef):
+            self._sequence_searches[search.id] = search
         else:
-            self.user_paths[user_path] = [search]
+            self._simple_searches[search.id] = search
+
+        if user_path in self._user_paths:
+            self._user_paths[user_path].append(search.id)
+        else:
+            self._user_paths[user_path] = [search.id]
+
+    def resolve_from_id(self, id):
+        """ Resolve search definition from unique id. """
+        if id in self._simple_searches:
+            return self._simple_searches[id]
+
+        return self._sequence_searches[id]
+
+    def resolve_from_tag(self, tag):
+        """ Resolve search definition from tag.
+
+        Returns a list of resolved searches.
+        """
+        searches = []
+        for id in self._search_tags[tag]:
+            searches.append(self.resolve_from_id(id))
+
+        return searches
 
     def _filtered_dir(self, contents, max_logrotate_depth=7):
         """ Filter contents of a directory. Directories are ignored and if any
         files look like logrotated log files they are sorted and only
         max_logrotate_depth are kept.
         """
         logrotated = {}
@@ -402,252 +631,275 @@
             log.error("source id %s already exists - trying again", s_id)
             s_id = str(uuid.uuid4())
 
         log.debug("path=%s source_id=%s", path, s_id)
         self._source_ids[s_id] = path
         return s_id
 
+    def __len__(self):
+        items = 0
+        for user_path in self._user_paths:
+            items += len(self._expand_path(user_path))
+
+        return items
+
     def __iter__(self):
-        for user_path, searches in self.user_paths.items():
+        for user_path, searches in self._user_paths.items():
             for path in self._expand_path(user_path):
                 yield {'user_path': user_path,
                        'path': path,
                        'source_id': self._get_source_id(path),
-                       'searches': searches}
+                       'searches': [self.resolve_from_id(id)
+                                    for id in searches]}
 
 
 class SearchTask(object):
 
-    def __init__(self, info, lock, constraints_manager, results_queue_id):
+    def __init__(self, info, constraints_manager, results_queue):
         self.info = info
-        self.lock = lock
         self.stats = SearchTaskStats()
         self.constraints_manager = constraints_manager
-        self.results_queue_id = results_queue_id
+        self.results_queue = results_queue
+
+    @cached_property
+    def id(self):
+        return str(uuid.uuid4())
 
     @cached_property
     def search_defs_conditional(self):
-        return [s_term for s_term in self.info['searches']
-                if s_term.constraints]
+        return [s_def for s_def in self.info['searches']
+                if s_def.constraints]
 
     @cached_property
     def search_defs(self):
-        all = {s_term: True for s_term in self.info['searches']}
-        for s_term in all:
-            if s_term in self.search_defs_conditional:
-                all[s_term] = False
+        all = {s_def: True for s_def in self.info['searches']}
+        for s_def in all:
+            if s_def in self.search_defs_conditional:
+                all[s_def] = False
 
         return all
 
     def put_result(self, result):
         self.stats['results'] += 1
-        max_tries = 10
-        _queue = RESULTS_QUEUES[self.results_queue_id]
+        max_tries = MAX_QUEUE_RETRIES
         while max_tries > 0:
             try:
-                _queue.put(result, timeout=RESULTS_QUEUE_TIMEOUT)
+                if max_tries == MAX_QUEUE_RETRIES:
+                    self.results_queue.put_nowait(result)
+                else:
+                    self.results_queue.put(result,
+                                           timeout=RESULTS_QUEUE_TIMEOUT)
+
                 break
             except queue.Full:
-                log.debug("search task queue for '%s' is full even after "
-                          "waiting %ss - trying again", self.info['path'],
-                          RESULTS_QUEUE_TIMEOUT)
+                if max_tries == MAX_QUEUE_RETRIES:
+                    msg = ("search task queue for '%s' is full - switching "
+                           "to using blocking put with timeout")
+                    log.info(msg, self.info['path'])
+                else:
+                    msg = ("search task queue for '%s' is full even after "
+                           "waiting %ss - trying again")
+                    log.warning(msg, self.info['path'],
+                                RESULTS_QUEUE_TIMEOUT)
+
                 max_tries -= 1
 
-    def _simple_search(self, s_term, line, ln):
+        if max_tries == 0:
+            log.error("exceeded max number of retries (%s) to put results "
+                      "data on the queue", MAX_QUEUE_RETRIES)
+
+    def _simple_search(self, search_def, line, ln):
+        """ Perform a simple search on line.
+
+        @param search_def: SearchDef object
+        @param line: current line (string)
+        @param ln: current line number
         """
-        Perform a simple search on line.
-        """
-        ret = s_term.run(line)
+        ret = search_def.run(line)
         if not ret:
             return
 
-        self.put_result(SearchResult(
-                            ln, self.info['source_id'], ret, s_term.tag,
-                            store_contents=s_term.store_result_contents))
+        self.put_result(SearchResult(ln, self.info['source_id'], ret,
+                                     search_def))
 
-    def _sequence_search(self, s_term, line, ln, sequence_results):
-        """
-        Perform a sequence search on line.
+    def _sequence_search(self, seq_def, line, ln, sequence_results):
+        """ Perform a sequence search on line.
+
+        @param seq_def: SequenceSearchDef object
+        @param line: current line (string)
+        @param ln: current line number
+        @param sequence_results: SequenceSearchResults object
         """
+        ret = seq_def.s_start.run(line)
         # if the ending is defined and we match a start while
         # already in a section, we start again.
-        if s_term.s_end:
-            ret = s_term.s_start.run(line)
-            if s_term.started:
-                if ret:
-                    # reset and start again
-                    if sequence_results:
-                        del sequence_results[s_term.id]
-
-                    s_term.reset()
-                else:
-                    ret = s_term.s_end.run(line)
-        else:
-            ret = s_term.s_start.run(line)
+        if seq_def.s_end and seq_def.started:
+            if ret:
+                # reset and start again
+                sequence_results.remove(seq_def.id)
+                seq_def.reset()
+            else:
+                ret = seq_def.s_end.run(line)
 
         if ret:
-            section_id = None
-            sequence_obj_id = None
-            tag = s_term.tag
-            store_contents = True
-
-            if not s_term.started:
-                tag = s_term.start_tag
-                s_term.start()
-                section_id = s_term.section_id
+            if not seq_def.started:
+                s_term = seq_def.s_start
+                seq_def.start()
+                section_id = seq_def.current_section_id
             else:
-                tag = s_term.end_tag
-                section_id = s_term.section_id
-                s_term.stop()
+                s_term = seq_def.s_end
+                section_id = seq_def.current_section_id
+                seq_def.stop()
                 # if no end is defined then we don't bother storing
                 # the result, just complete the section and start
                 # the next.
-                if s_term.s_end is None:
-                    tag = s_term.start_tag
-                    s_term.start()
-                    section_id = s_term.section_id
-
-            sequence_obj_id = s_term.id
-            r = SearchResult(ln, self.info['source_id'], ret, tag,
-                             section_id=section_id,
-                             sequence_obj_id=sequence_obj_id,
-                             store_contents=store_contents)
-            if s_term.id not in sequence_results:
-                sequence_results[s_term.id] = [r]
-            else:
-                sequence_results[s_term.id].append(r)
-        else:
-            if s_term.started and s_term.s_body:
-                ret = s_term.s_body.run(line)
-                if ret:
-                    r = SearchResult(ln, self.info['source_id'], ret,
-                                     s_term.body_tag,
-                                     section_id=s_term.section_id,
-                                     sequence_obj_id=s_term.id)
-                    sequence_results[s_term.id].append(r)
-
-        return sequence_results
+                if seq_def.s_end is None:
+                    s_term = seq_def.s_start
+                    seq_def.start()
+                    section_id = seq_def.current_section_id
+
+            sequence_results.add(SearchResult(ln, self.info['source_id'], ret,
+                                              s_term,
+                                              sequence_section_id=section_id))
+        elif seq_def.started and seq_def.s_body:
+            section_id = seq_def.current_section_id
+            ret = seq_def.s_body.run(line)
+            if ret:
+                sequence_results.add(SearchResult(
+                                            ln, self.info['source_id'],
+                                            ret, seq_def.s_body,
+                                            sequence_section_id=section_id))
 
     def _process_sequence_results(self, sequence_results, current_ln):
         """
-        @param sequence_results: list of sequence search results
+        Perform post processing to sequence search results.
+
+        @param sequence_results: SequenceSearchResults object
         @param current_ln: number of the last line to be read from file
         """
         # If a sequence ending definition is provided and we reached EOF
         # while a sequence is started, complete the sequence if s_end
         # matches an empty string. If s_end is not defined we just go ahead
         # and complete the section.
         filter_section_id = {}
-        for s_term in self.search_defs:
-            if type(s_term) == SequenceSearchDef:
-                if s_term.started:
-                    if s_term.s_end is None:
-                        s_term.stop()
-                    else:
-                        ret = s_term.s_end.run("")
-                        if ret:
-                            section_id = s_term.section_id
-                            s_term.stop()
-                            tag = s_term.end_tag
-                            r = SearchResult(current_ln + 1,
-                                             self.info['source_id'], ret,
-                                             tag,
-                                             section_id=section_id,
-                                             sequence_obj_id=s_term.id)
-                        else:
-                            if s_term.id not in filter_section_id:
-                                filter_section_id[s_term.id] = []
+        for s_def in self.search_defs:
+            if type(s_def) != SequenceSearchDef:
+                continue
+
+            seq_def = s_def
+            if not seq_def.started:
+                continue
+
+            if seq_def.s_end is None:
+                continue
+
+            ret = seq_def.s_end.run('')
+            if ret:
+                section_id = seq_def.current_section_id
+                r = SearchResult(current_ln + 1, self.info['source_id'], ret,
+                                 seq_def.s_end, sequence_section_id=section_id)
+                sequence_results.add(r)
+            else:
+                if seq_def.id not in filter_section_id:
+                    filter_section_id[seq_def.id] = []
+
+                filter_section_id[seq_def.id].append(
+                    seq_def.current_section_id)
 
-                            filter_section_id[s_term.id].append(
-                                s_term.section_id)
+        if len(sequence_results) < 1:
+            log.debug("no sequence results to process")
+            return
 
+        log.debug("filtering sections: %s", filter_section_id)
         # Now add sequence results to main results list, excluding any
         # incomplete sections.
         for s_results in sequence_results.values():
             for r in s_results:
                 if filter_section_id:
-                    seq_id = r.sequence_obj_id
-                    if (seq_id is not None and
-                            seq_id in filter_section_id):
+                    if r.sequence_def is None:
+                        continue
+
+                    seq_id = r.sequence_def.id
+                    if seq_id in filter_section_id:
                         if r.section_id in filter_section_id[seq_id]:
                             continue
 
                 self.put_result(r)
 
     def _run_search(self, fd):
         """
         @param fd: open file descriptor
         """
         self.stats.reset()
-        sequence_results = {}
+        sequence_results = SequenceSearchResults()
         offset = self.constraints_manager.apply_global(self.info['user_path'],
                                                        fd)
         log.debug("starting search of %s (offset=%s, pos=%s)", fd.name, offset,
                   fd.tell())
         runnable = {s.id: _runnable
                     for s, _runnable in self.search_defs.items()}
+        ln = 0
         # NOTE: line numbers start at 1 hence offset + 1
         for ln, line in enumerate(fd, start=offset + 1):
             self.stats['lines_searched'] += 1
             if type(line) == bytes:
                 line = line.decode("utf-8")
 
-            for s_term in self.search_defs:
-                if not runnable[s_term.id]:
-                    if not self.constraints_manager.apply_single(s_term, line):
+            for s_def in self.search_defs:
+                if not runnable[s_def.id]:
+                    if not self.constraints_manager.apply_single(s_def, line):
                         continue
 
                     # enable from here on in
-                    runnable[s_term.id] = True
+                    runnable[s_def.id] = True
 
-                if type(s_term) == SequenceSearchDef:
-                    sequence_results = self._sequence_search(s_term, line, ln,
-                                                             sequence_results)
+                if type(s_def) == SequenceSearchDef:
+                    self._sequence_search(s_def, line, ln, sequence_results)
                 else:
-                    self._simple_search(s_term, line, ln)
-
-        if sequence_results:
-            self._process_sequence_results(sequence_results, ln)
+                    self._simple_search(s_def, line, ln)
 
+        self._process_sequence_results(sequence_results, ln)
         log.debug("completed search of %s lines", self.stats['lines_searched'])
         if self.search_defs_conditional:
             msg = "constraints stats {}:".format(fd.name)
             for sd in self.search_defs_conditional:
                 if sd.constraints:
                     for c in sd.constraints.values():
                         msg += "\n  id={}: {}".format(c.id, c.stats())
 
             log.debug(msg)
 
+        log.debug("run search complete for path %s", fd.name)
         return self.stats
 
     def failed(self, exc):
         """ This should be called if the task failed to execute. """
         log.error("search task failed for path=%s with exception %s",
                   self.info['path'], exc)
 
     def execute(self):
+        stats = SearchTaskStats()
         path = self.info['path']
         if os.path.getsize(path) == 0:
             log.debug("filesearcher: zero-length file %s - skipping search",
                       path)
-            return
+            return stats
 
+        log.debug("starting execution on path %s", path)
         try:
+            # first assume compressed then plain
             with gzip.open(path, 'rb') as fd:
                 try:
                     # test if file is gzip
                     fd.read(1)
                     fd.seek(0)
-                    return self._run_search(fd)
+                    stats = self._run_search(fd)
                 except OSError:
-                    pass
-
-            with open(path, 'rb') as fd:
-                return self._run_search(fd)
+                    with open(path, 'rb') as fd:
+                        stats = self._run_search(fd)
         except UnicodeDecodeError:
             log.exception("")
             # ignore the file if it can't be decoded
             log.debug("caught UnicodeDecodeError for path %s - skipping",
                       path)
         except EOFError as e:
             log.exception("")
@@ -656,27 +908,30 @@
             raise FileSearchException(msg) from e
         except Exception as e:
             log.exception("")
             msg = ("an unexpected exception occurred while searching {} - {}".
                    format(path, e))
             raise FileSearchException(msg) from e
 
-        return SearchTaskStats()
+        log.debug("finished execution on path %s", path)
+        return stats
 
 
 class SearchTaskStats(UserDict):
 
     def __init__(self):
         self.reset()
 
     def reset(self):
         self.data = {'lines_searched': 0,
+                     'jobs_completed': 0,
+                     'total_jobs': 0,
                      'results': 0}
 
-    def combine(self, stats):
+    def update(self, stats):
         if not stats:
             return
 
         for key, val in stats.items():
             self.data[key] += val
 
     def __repr__(self):
@@ -726,20 +981,14 @@
             log.debug("no global constraint to apply to %s", fd.name)
             return offset
 
         if user_path in self.global_restrictions:
             log.debug("skipping global constraint for %s", fd.name)
             return offset
 
-        # if not os.path.isdir(os.path.join(HotSOSConfig.data_root,
-        #                                   'sos_commands')):
-        #     log.info("skipping global constraints since data_root is not a "
-        #              "sosreport therefore files may be changing")
-        #     return offset
-
         for c in self.global_constraints:
             log.debug("applying task global constraint %s to %s", c.id,
                       fd.name)
             _offset = c.apply_to_file(fd)
             if _offset is not None:
                 return _offset
 
@@ -764,15 +1013,18 @@
 class FileSearcher(SearcherBase):
 
     def __init__(self, max_parallel_tasks=8, max_logrotate_depth=7,
                  constraint=None):
         """
         @param max_parallel_tasks: max number of search tasks that can run in
                                    parallel.
-        @param max_logrotate_depth: TODO
+        @param max_logrotate_depth: used by SearchCatalog to filter logfiles
+                                    based on their name if it matches a
+                                    logrotate format and want to constrain how
+                                    much history we search.
         @param constraint: constraint to be used with this
                                    searcher that applies to all files searched.
         """
         self.max_parallel_tasks = max_parallel_tasks
         self._stats = SearchTaskStats()
         self.catalog = SearchCatalog(max_logrotate_depth)
         self.constraints_manager = SearchConstraintsManager(self.catalog)
@@ -786,17 +1038,19 @@
     def resolve_source_id(self, source_id):
         return self.catalog.source_id_to_path(source_id)
 
     def add(self, searchdef, path, allow_global_constraints=True):
         """
         Add a search definition.
 
-        @param searchdef: a SearchDef object
-        @param path: path we want to search. this can be a file, dir or glob
-        @param allow_global_constraints:
+        @param searchdef: a SearchDef or SequenceSearchDef object.
+        @param path: path we want to search. this can be a file, dir or glob.
+        @param allow_global_constraints: boolean determining whether we want
+                                         any global constraints available to be
+                                         applied to this path.
         """
         if not allow_global_constraints:
             self.constraints_manager.global_restrictions.add(path)
 
         self.catalog.register(searchdef, path)
 
     @property
@@ -813,100 +1067,183 @@
         """
         Provide stats for the last search run.
 
         @return: SearchTaskStats object
         """
         return self._stats
 
-    def _get_results(self, results, queue_id, expected=None, event=None):
-        _queue = RESULTS_QUEUES[queue_id]
+    def _get_results(self, results, queue, event, stats):
+        """
+        Collect results from all search task processes.
+
+        @param results: SearchResultsCollection object.
+        @param queue: results queue used for this search session.
+        @param event: event object used to notify this thread to stop.
+        @param stats: SearchTaskStats object
+        """
+        log.debug("fetching results from worker queues")
+
         while True:
-            if not _queue.empty():
-                results.add(_queue.get())
-            elif expected and expected > len(results):
+            if not queue.empty():
+                results.add(queue.get())
+            elif event.is_set():
+                log.debug("exiting results thread")
+                break
+            else:
+                log.debug("total %s results received, %s/%s jobs completed - "
+                          "waiting for more", len(results),
+                          stats['jobs_completed'], stats['total_jobs'])
+                # yield
+                time.sleep(0.1)
+
+        log.debug("stopped fetching results (total received=%s)", len(results))
+
+    def _purge_results(self, results, queue, expected):
+        """
+        Purge results from all search task processes.
+
+        @param results: SearchResultsCollection object.
+        @param queue: results queue used for this search session.
+        @param expected: number of results we expect to receive. this is used
+                         to do a final sweep once all search tasks are complete
+                         to ensure all results have been collected.
+        """
+        log.debug("purging results (expected=%s)", expected)
+
+        while True:
+            if not queue.empty():
+                results.add(queue.get())
+            elif expected > len(results):
                 try:
-                    r = _queue.get(timeout=RESULTS_QUEUE_TIMEOUT)
+                    r = queue.get(timeout=RESULTS_QUEUE_TIMEOUT)
                     results.add(r)
                 except queue.Empty:
-                    log.debug("timeout waiting > %s secs to receive results - "
-                              "expected=%s, actual=%s", RESULTS_QUEUE_TIMEOUT,
-                              expected, len(results))
-            elif event:
-                if event.is_set():
-                    log.debug("exiting get thread")
-                    break
+                    log.info("timeout waiting > %s secs to receive results - "
+                             "expected=%s, actual=%s", RESULTS_QUEUE_TIMEOUT,
+                             expected, len(results))
             else:
                 break
 
-    def _run(self, queue_id):
+        log.debug("stopped purging results (total received=%s)",
+                  len(results))
+
+    def _create_results_thread(self, results, queue, stats):
+        log.debug("creating results queue consumer thread")
+        event = threading.Event()
+        event.clear()
+        t = threading.Thread(target=self._get_results,
+                             args=[results, queue, event, stats])
+        return t, event
+
+    def _stop_results_thread(self, thread, event):
+        log.debug("joining/stopping queue consumer thread")
+        event.set()
+        thread.join()
+        log.debug("consumer thread stopped successfully")
+
+    def _ensure_worker_processes_killed(self):
+        """
+        For some reason it is sometimes possible to for pool termination to
+        hang indefinitely because one or more worker process fails to
+        terminate. This method ensures that all extant worker child processes
+        are killed so that pool termination is guaranteed to complete.
+        """
+        log.debug("ensuring all pool workers killed")
+        worker_pids = []
+        for child in multiprocessing.active_children():
+            if type(child) == multiprocessing.context.ForkProcess:
+                if 'ForkProcess' in child.name:
+                    worker_pids.append(child.pid)
+
+        ps_out = subprocess.check_output(['ps', '-opid', '--no-headers',
+                                          '--ppid',
+                                          str(os.getpid())], encoding='utf8')
+        child_pids = [int(line.strip()) for line in ps_out.splitlines()]
+        log.debug("process has child pids: %s", child_pids)
+        for wpid in worker_pids:
+            if int(wpid) not in child_pids:
+                log.error("worker pid %s no longer a child of this process "
+                          "(%s)", wpid, os.getpid())
+                continue
+
+            try:
+                log.debug('sending SIGKILL to worker process %s', wpid)
+                os.kill(wpid, signal.SIGILL)
+            except Exception:
+                log.debug('worker process %s already killed', wpid)
+
+    def _run(self, mgr):
         """ Run all searches.
 
+        @param mgr: multiprocessing.Manager object
         @return: SearchResultsCollection object
         """
         self.stats.reset()
         results = SearchResultsCollection(self.catalog)
-        jobs = []
-        with multiprocessing.Manager() as m:
-            lock = m.Lock()
-            event = threading.Event()
-            event.clear()
-            t = threading.Thread(target=self._get_results,
-                                 args=[results, queue_id],
-                                 kwargs={'event': event})
-            try:
-                log.debug("starting queue consumer thread")
-                t.start()
-                # make child processes ignore sigint so it can be handled here
-                orig_sigint = signal.signal(signal.SIGINT, signal.SIG_IGN)
-                num_p_tasks = self.num_parallel_tasks
-                with multiprocessing.Pool(processes=num_p_tasks) as p:
-                    # re-establish sigint
-                    signal.signal(signal.SIGINT, orig_sigint)
-                    for info in self.catalog:
-                        c_mgr = self.constraints_manager
-                        task = SearchTask(info, lock,
-                                          constraints_manager=c_mgr,
-                                          results_queue_id=queue_id)
-                        jobs.append(p.apply_async(task.execute,
-                                                  error_callback=task.failed))
-
-                    log.debug("filesearcher: syncing %s jobs", len(jobs))
-                    while len(jobs) > 0:
-                        for i, j in enumerate(jobs):
-                            j.wait(10)
-                            if j.ready():
-                                self.stats.combine(j.get())
-                                jobs.pop(i)
-
-                    log.debug("joining queue (expected=%s, remaining=%s)",
-                              self.stats['results'],
-                              self.stats['results'] - len(results))
-                    log.debug("joining queue consumer thread")
-                    event.set()
-                    t.join()
-                    t = None
-                    self._get_results(results, queue_id,
-                                      expected=self.stats['results'])
-            finally:
-                if t is not None:
-                    event.set()
-                    t.join()
+        if len(self.catalog) == 0:
+            log.debug("catalog is empty - nothing to run")
+            return results
+
+        queue = mgr.Queue()
+        results_thread, event = self._create_results_thread(results, queue,
+                                                            self.stats)
+        results_thread_started = False
+        try:
+            num_workers = self.num_parallel_tasks
+            with concurrent.futures.ProcessPoolExecutor(
+                                    max_workers=num_workers) as executor:
+                jobs = {}
+                for info in self.catalog:
+                    c_mgr = self.constraints_manager
+                    task = SearchTask(info,
+                                      constraints_manager=c_mgr,
+                                      results_queue=queue)
+                    job = executor.submit(task.execute)
+                    jobs[job] = info['path']
+                    self.stats['total_jobs'] += 1
+
+                log.debug("filesearcher: syncing %s job(s)", len(jobs))
+                results_thread.start()
+                results_thread_started = True
+                try:
+                    for future in concurrent.futures.as_completed(jobs):
+                        self.stats.update(future.result())
+                        self.stats['jobs_completed'] += 1
+                except concurrent.futures.process.BrokenProcessPool as exc:
+                    msg = ("one or more worker processes has died - "
+                           "aborting search")
+                    raise FileSearchException(msg) from exc
+
+                log.debug("all workers synced")
+                # double check nothing is running anymore
+                for job, path in jobs.items():
+                    log.debug("worker for path '%s' has state: %s", path,
+                              repr(job))
+                    if job.running():
+                        log.info("job for path '%s' still running when "
+                                 "not expected to be", path)
+
+                self._stop_results_thread(results_thread, event)
+                results_thread = None
+                log.debug("purging remaining results (expected=%s, "
+                          "remaining=%s)", self.stats['results'],
+                          self.stats['results'] - len(results))
+                self._purge_results(results, queue, self.stats['results'])
+
+                self._ensure_worker_processes_killed()
+                log.debug("terminating pool")
+        finally:
+            if results_thread is not None and results_thread_started:
+                self._stop_results_thread(results_thread, event)
 
         log.debug("filesearcher: stats=%s", self.stats)
         log.debug("filesearcher: completed (results=%s)", len(results))
         return results
 
     def run(self):
         """ Run all searches.
 
         @return: SearchResultsCollection object
         """
-        queue_id = "{}:{}".format(os.getpid(), uuid.uuid4())
-        if queue_id in RESULTS_QUEUES:
-            raise Exception("results queue already exists with id {}".
-                            format(queue_id))
-
-        RESULTS_QUEUES[queue_id] = multiprocessing.Queue()
-        try:
-            return self._run(queue_id)
-        finally:
-            del RESULTS_QUEUES[queue_id]
+        log.debug("filesearcher: starting")
+        with multiprocessing.Manager() as mgr:
+            return self._run(mgr)
```

