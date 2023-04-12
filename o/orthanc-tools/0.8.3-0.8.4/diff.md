# Comparing `tmp/orthanc_tools-0.8.3.tar.gz` & `tmp/orthanc_tools-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orthanc_tools-0.8.3.tar", last modified: Tue Apr  4 12:54:14 2023, max compression
+gzip compressed data, was "orthanc_tools-0.8.4.tar", last modified: Wed Apr 12 08:49:44 2023, max compression
```

## Comparing `orthanc_tools-0.8.3.tar` & `orthanc_tools-0.8.4.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:54:14.274066 orthanc_tools-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-04-04 12:51:39.000000 orthanc_tools-0.8.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-04 12:51:39.000000 orthanc_tools-0.8.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-04-04 12:54:14.274066 orthanc_tools-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-04-04 12:51:39.000000 orthanc_tools-0.8.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:54:14.270066 orthanc_tools-0.8.3/orthanc_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-04 12:51:39.000000 orthanc_tools-0.8.3/orthanc_tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:54:14.274066 orthanc_tools-0.8.3/orthanc_tools/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-04 12:51:39.000000 orthanc_tools-0.8.3/orthanc_tools/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-04 12:51:39.000000 orthanc_tools-0.8.3/orthanc_tools/helpers/old_files_deleter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-04 12:51:39.000000 orthanc_tools-0.8.3/orthanc_tools/helpers/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-04-04 12:51:39.000000 orthanc_tools-0.8.3/orthanc_tools/helpers/time_out.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-04 12:51:39.000000 orthanc_tools-0.8.3/orthanc_tools/helpers/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:54:14.274066 orthanc_tools-0.8.3/orthanc_tools/hl7Lib/
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-04 12:51:39.000000 orthanc_tools-0.8.3/orthanc_tools/hl7Lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-04 12:51:39.000000 orthanc_tools-0.8.3/orthanc_tools/hl7Lib/hl7.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-04-04 12:51:39.000000 orthanc_tools-0.8.3/orthanc_tools/hl7Lib/hl7_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8957 2023-04-04 12:51:39.000000 orthanc_tools-0.8.3/orthanc_tools/hl7Lib/hl7_dicom_worklist_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-04 12:51:39.000000 orthanc_tools-0.8.3/orthanc_tools/hl7Lib/hl7_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-04 12:51:39.000000 orthanc_tools-0.8.3/orthanc_tools/hl7Lib/hl7_message_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-04-04 12:51:39.000000 orthanc_tools-0.8.3/orthanc_tools/hl7Lib/hl7_message_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-04-04 12:51:39.000000 orthanc_tools-0.8.3/orthanc_tools/hl7Lib/hl7_orm_worklist_msg_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-04-04 12:51:39.000000 orthanc_tools-0.8.3/orthanc_tools/hl7Lib/hl7_oru_report_msg_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-04-04 12:51:39.000000 orthanc_tools-0.8.3/orthanc_tools/hl7Lib/hl7_report_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-04-04 12:51:39.000000 orthanc_tools-0.8.3/orthanc_tools/hl7Lib/hl7_report_series_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-04-04 12:51:39.000000 orthanc_tools-0.8.3/orthanc_tools/hl7Lib/hl7_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-04-04 12:51:39.000000 orthanc_tools-0.8.3/orthanc_tools/hl7Lib/hl7_worklist_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-04-04 12:51:39.000000 orthanc_tools-0.8.3/orthanc_tools/orthanc_cloner.py
--rw-r--r--   0 runner    (1001) docker     (123)    17715 2023-04-04 12:51:39.000000 orthanc_tools-0.8.3/orthanc_tools/orthanc_comparator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-04 12:51:39.000000 orthanc_tools-0.8.3/orthanc_tools/orthanc_folder_importer.py
--rw-r--r--   0 runner    (1001) docker     (123)    17251 2023-04-04 12:51:39.000000 orthanc_tools-0.8.3/orthanc_tools/orthanc_forwarder.py
--rw-r--r--   0 runner    (1001) docker     (123)    10904 2023-04-04 12:51:39.000000 orthanc_tools-0.8.3/orthanc_tools/orthanc_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9437 2023-04-04 12:51:39.000000 orthanc_tools-0.8.3/orthanc_tools/orthanc_test_db_populator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15403 2023-04-04 12:51:39.000000 orthanc_tools-0.8.3/orthanc_tools/pacs_migrator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:54:14.274066 orthanc_tools-0.8.3/orthanc_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-04-04 12:54:14.000000 orthanc_tools-0.8.3/orthanc_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-04 12:54:14.000000 orthanc_tools-0.8.3/orthanc_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 12:54:14.000000 orthanc_tools-0.8.3/orthanc_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-04 12:54:14.000000 orthanc_tools-0.8.3/orthanc_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-04 12:54:14.000000 orthanc_tools-0.8.3/orthanc_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-04 12:51:39.000000 orthanc_tools-0.8.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-04 12:51:39.000000 orthanc_tools-0.8.3/release-notes.md
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-04 12:54:14.274066 orthanc_tools-0.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6609 2023-04-04 12:51:39.000000 orthanc_tools-0.8.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 12:54:14.274066 orthanc_tools-0.8.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    18316 2023-04-04 12:51:39.000000 orthanc_tools-0.8.3/tests/test_3_orthancs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-04-04 12:51:39.000000 orthanc_tools-0.8.3/tests/test_old_files_deleter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:49:44.216294 orthanc_tools-0.8.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-04-12 08:49:44.216294 orthanc_tools-0.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:49:44.212294 orthanc_tools-0.8.4/orthanc_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/orthanc_tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:49:44.216294 orthanc_tools-0.8.4/orthanc_tools/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/orthanc_tools/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/orthanc_tools/helpers/old_files_deleter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/orthanc_tools/helpers/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/orthanc_tools/helpers/time_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/orthanc_tools/helpers/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:49:44.216294 orthanc_tools-0.8.4/orthanc_tools/hl7Lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/orthanc_tools/hl7Lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/orthanc_tools/hl7Lib/hl7.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/orthanc_tools/hl7Lib/hl7_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8957 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/orthanc_tools/hl7Lib/hl7_dicom_worklist_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/orthanc_tools/hl7Lib/hl7_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/orthanc_tools/hl7Lib/hl7_message_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/orthanc_tools/hl7Lib/hl7_message_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/orthanc_tools/hl7Lib/hl7_orm_worklist_msg_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/orthanc_tools/hl7Lib/hl7_oru_report_msg_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/orthanc_tools/hl7Lib/hl7_report_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/orthanc_tools/hl7Lib/hl7_report_series_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/orthanc_tools/hl7Lib/hl7_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/orthanc_tools/hl7Lib/hl7_worklist_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/orthanc_tools/orthanc_cloner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17715 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/orthanc_tools/orthanc_comparator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/orthanc_tools/orthanc_folder_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17487 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/orthanc_tools/orthanc_forwarder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10904 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/orthanc_tools/orthanc_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9437 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/orthanc_tools/orthanc_test_db_populator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15403 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/orthanc_tools/pacs_migrator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:49:44.216294 orthanc_tools-0.8.4/orthanc_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-04-12 08:49:44.000000 orthanc_tools-0.8.4/orthanc_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-12 08:49:44.000000 orthanc_tools-0.8.4/orthanc_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 08:49:44.000000 orthanc_tools-0.8.4/orthanc_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-12 08:49:44.000000 orthanc_tools-0.8.4/orthanc_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-12 08:49:44.000000 orthanc_tools-0.8.4/orthanc_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/release-notes.md
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-12 08:49:44.216294 orthanc_tools-0.8.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6609 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 08:49:44.216294 orthanc_tools-0.8.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    18316 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/tests/test_3_orthancs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-04-12 08:46:59.000000 orthanc_tools-0.8.4/tests/test_old_files_deleter.py
```

### Comparing `orthanc_tools-0.8.3/LICENSE.txt` & `orthanc_tools-0.8.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.3/PKG-INFO` & `orthanc_tools-0.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orthanc_tools
-Version: 0.8.3
+Version: 0.8.4
 Summary: Python Orthanc Tools
 Home-page: https://github.com/orthanc-team/python-orthanc-tools
 Author: Orthanc Team
 Author-email: info@orthanc.team
 Project-URL: Bug Reports, https://github.com/orthanc-team/python-orthanc-tools/issues
 Project-URL: Funding, https://orthanc.team
 Project-URL: Source, https://github.com/orthanc-team/python-orthanc-tools/
```

### Comparing `orthanc_tools-0.8.3/README.md` & `orthanc_tools-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.3/orthanc_tools/__init__.py` & `orthanc_tools-0.8.4/orthanc_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.3/orthanc_tools/helpers/old_files_deleter.py` & `orthanc_tools-0.8.4/orthanc_tools/helpers/old_files_deleter.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.3/orthanc_tools/helpers/scheduler.py` & `orthanc_tools-0.8.4/orthanc_tools/helpers/scheduler.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.3/orthanc_tools/helpers/time_out.py` & `orthanc_tools-0.8.4/orthanc_tools/helpers/time_out.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.3/orthanc_tools/helpers/timer.py` & `orthanc_tools-0.8.4/orthanc_tools/helpers/timer.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.3/orthanc_tools/hl7Lib/__init__.py` & `orthanc_tools-0.8.4/orthanc_tools/hl7Lib/__init__.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.3/orthanc_tools/hl7Lib/hl7_client.py` & `orthanc_tools-0.8.4/orthanc_tools/hl7Lib/hl7_client.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.3/orthanc_tools/hl7Lib/hl7_dicom_worklist_builder.py` & `orthanc_tools-0.8.4/orthanc_tools/hl7Lib/hl7_dicom_worklist_builder.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.3/orthanc_tools/hl7Lib/hl7_error.py` & `orthanc_tools-0.8.4/orthanc_tools/hl7Lib/hl7_error.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.3/orthanc_tools/hl7Lib/hl7_message_parser.py` & `orthanc_tools-0.8.4/orthanc_tools/hl7Lib/hl7_message_parser.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.3/orthanc_tools/hl7Lib/hl7_message_validator.py` & `orthanc_tools-0.8.4/orthanc_tools/hl7Lib/hl7_message_validator.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.3/orthanc_tools/hl7Lib/hl7_orm_worklist_msg_handler.py` & `orthanc_tools-0.8.4/orthanc_tools/hl7Lib/hl7_orm_worklist_msg_handler.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.3/orthanc_tools/hl7Lib/hl7_oru_report_msg_handler.py` & `orthanc_tools-0.8.4/orthanc_tools/hl7Lib/hl7_oru_report_msg_handler.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.3/orthanc_tools/hl7Lib/hl7_report_parser.py` & `orthanc_tools-0.8.4/orthanc_tools/hl7Lib/hl7_report_parser.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.3/orthanc_tools/hl7Lib/hl7_report_series_builder.py` & `orthanc_tools-0.8.4/orthanc_tools/hl7Lib/hl7_report_series_builder.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.3/orthanc_tools/hl7Lib/hl7_server.py` & `orthanc_tools-0.8.4/orthanc_tools/hl7Lib/hl7_server.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.3/orthanc_tools/hl7Lib/hl7_worklist_parser.py` & `orthanc_tools-0.8.4/orthanc_tools/hl7Lib/hl7_worklist_parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 import typing
 # from hl7Lib import Hl7MessageParser
 from .hl7_message_parser import Hl7MessageParser
 
 
 class Hl7WorklistParser(Hl7MessageParser):
 
-    def __init__(self, specific_fields: dict = None):
+    def __init__(self, specific_fields: dict = None, patient_name_components_count: int = 5):
         super(Hl7WorklistParser, self).__init__()
 
+        self._patient_name_components_count = patient_name_components_count
+
         # Let's add "standards" field
         self.add_fields_definitions({
             # --- PID segment
             'PatientID': 'PID.F3.R1.C1',
             'IssuerOfPatientID': 'PID.F3.R1.C4',
             'PatientName': 'PID.F5',  # IHE recommend to use the whole Field 5 as the patient name (it's usually full of ^ that is a separator in HL7 so we must take it as is without trying to parse it !
             'PatientMotherBirthName': 'PID.F6',
@@ -31,14 +33,16 @@
             #'ScheduledProcedureStepStartDateTime': 'OBR.F27.R1.C4',
             '_scheduledProcedureStepStartDateTime': 'OBR.F27.R1.C4',
 
             # --- PV1 segment
             '_ambulatoryStatus' : 'PV1.F15',
             'ReferringPhysicianName' : 'PV1.F8',
             'ConfidentialityConstraintOnPatientDataDescription' : 'PV1.F16',
+            '_consultingDoctorPV1' : 'PV1.F9',
+            ''
 
             # --- ORC segment
             'OrderPlacerIdentifierSequence' : 'ORC.F2.R1.C1',
             'RequestedProcedureID' : 'ORC.F2.R1.C1',
             'ScheduledProcedureStepID' : 'ORC.F2.R1.C1',
             'OrderFillerIdentifierSequence' : 'ORC.F3',
             '_requestingPhysicianORC' : 'ORC.F12',
@@ -62,22 +66,23 @@
         values['Modality'] = None
         values['ReferringPhysicianName'] = None
         values['ScheduledStationAETitle'] = 'UNKNOWN'
         values['ScheduledPerformingPhysicianName'] = None
         values['ScheduledStationName'] = None
         values['ScheduledProcedureStepID'] = 'UNKNOWN'
         values['RequestedProcedureID'] = 'UNKNOWN'
+        values['SpecificCharacterSet'] = 'ASCII'
 
         # extract field the default way
         values_from_hl7 = super(Hl7WorklistParser, self).parse(hl7_message, strict = False)
 
         values.update(values_from_hl7)
 
         # keep only the first 5 components of the name according to http://dicom.nema.org/dicom/2013/output/chtml/part05/sect_6.2.html (check PN VR definition)
-        values['PatientName'] = '^'.join(values['PatientName'].split('^')[:5])
+        values['PatientName'] = '^'.join(values['PatientName'].split('^')[:self._patient_name_components_count])
 
         sex = values['_sex']
         if sex is None or sex in ['M', 'F']:
             values['PatientSex'] = sex
         elif sex in ['U']:  # unknown in HL7 -> null in Dicom
             values['PatientSex'] = None
         elif sex in ['A', 'N']:  # ambiguous or Not Applicable in HL7 -> 'other' in Dicom
@@ -109,10 +114,14 @@
             elif len(datetimeString) == 14:
                 values['ScheduledProcedureStepStartTime'] = datetimeString[8:14]
 
         if values.get('_requestingPhysicianOBR') is not None:
             values['RequestingPhysician'] = values.get('_requestingPhysicianOBR')
         elif values.get('_requestingPhysicianORC') is not None:
             values['RequestingPhysician'] = values.get('_requestingPhysicianORC')
+        elif values.get('_consultingDoctorPV1') is not None:
+            values['RequestingPhysician'] = values.get('_consultingDoctorPV1')
+
+
 
         return values
```

### Comparing `orthanc_tools-0.8.3/orthanc_tools/orthanc_cloner.py` & `orthanc_tools-0.8.4/orthanc_tools/orthanc_cloner.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.3/orthanc_tools/orthanc_comparator.py` & `orthanc_tools-0.8.4/orthanc_tools/orthanc_comparator.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.3/orthanc_tools/orthanc_folder_importer.py` & `orthanc_tools-0.8.4/orthanc_tools/orthanc_folder_importer.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.3/orthanc_tools/orthanc_forwarder.py` & `orthanc_tools-0.8.4/orthanc_tools/orthanc_forwarder.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,26 +82,24 @@
 
     def __init__(self,
                  source: OrthancApiClient,
                  destinations: List[ForwarderDestination],
                  trigger: ChangeType = ChangeType.STABLE_STUDY,
                  max_retry_count_at_startup: int = 5,
                  polling_interval_in_seconds: int = 1,
-                 worker_threads_count: int = 1,
                  instance_filter = None,    # a method to filter instances.  Signature: Filter(api_client, instance_id) -> bool (returns True to keep an instance, returns False to delete it)
                  instance_processor = None  # a method to process instances before forwarding them.  Signature: Process(api_client, instance_id)
                  ):
 
         self._source = source
         self._destinations = destinations
         self._trigger = trigger
         self._max_retry_count_at_startup = max_retry_count_at_startup
         self._polling_interval_in_seconds = polling_interval_in_seconds
         self._is_running = False
-        self._worker_threads_count = worker_threads_count
         self._execution_thread = None
         self._instance_filter = instance_filter
         self._instance_processor = instance_processor
         self._status = {}
 
     def wait_orthanc_started(self):
         retry = 0
@@ -125,41 +123,45 @@
         self.wait_orthanc_started()
 
         while True:
             self.handle_all_content()
             time.sleep(self._polling_interval_in_seconds)
 
     def handle_all_content(self):
-        if self._trigger == ChangeType.STABLE_STUDY:
-            studies_ids = self._source.studies.get_all_ids()
-            if len(studies_ids) > 0:
-                for study_id in studies_ids:
-                    self._handle_study(study_id=study_id,
-                                       api_client=self._source)
-
-        elif self._trigger == ChangeType.STABLE_SERIES:
-            series_ids = self._source.series.get_all_ids()
-            if len(series_ids) > 0:
-                for id in series_ids:
-                    self._handle_series(series_id=id,
-                                        api_client=self._source)
+        try:
+            if self._trigger == ChangeType.STABLE_STUDY:
+                studies_ids = self._source.studies.get_all_ids()
+                if len(studies_ids) > 0:
+                    for study_id in studies_ids:
+                        self._handle_study(study_id=study_id,
+                                           api_client=self._source)
+
+            elif self._trigger == ChangeType.STABLE_SERIES:
+                series_ids = self._source.series.get_all_ids()
+                if len(series_ids) > 0:
+                    for id in series_ids:
+                        self._handle_series(series_id=id,
+                                            api_client=self._source)
+                else:
+                    logger.warning(f"No series found in Orthanc at startup")
+
+            elif self._trigger == ChangeType.NEW_INSTANCE:
+                instances_ids = self._source.instances.get_all_ids()
+                if len(instances_ids) > 0:
+                    for id in instances_ids:
+                        self._handle_instance(instance_id=id,
+                                              api_client=self._source)
+                else:
+                    logger.warning(f"No series found in Orthanc at startup")
             else:
-                logger.warning(f"No series found in Orthanc at startup")
-
-        elif self._trigger == ChangeType.NEW_INSTANCE:
-            instances_ids = self._source.instances.get_all_ids()
-            if len(instances_ids) > 0:
-                for id in instances_ids:
-                    self._handle_instance(instance_id=id,
-                                          api_client=self._source)
-            else:
-                logger.warning(f"No series found in Orthanc at startup")
-        else:
-            raise NotImplementedError()
-
+                raise NotImplementedError()
+        except exceptions.ConnectionError as ex:
+            logger.info(f"Connection error while handling all content: {ex.msg}")
+        except Exception as ex:
+            logger.exception("Error while handling all content", ex)
 
     def _thread_execute(self):
         while self._is_running:
             self.handle_all_content()
             time.sleep(self._polling_interval_in_seconds)
 
     def start(self):
```

### Comparing `orthanc_tools-0.8.3/orthanc_tools/orthanc_monitor.py` & `orthanc_tools-0.8.4/orthanc_tools/orthanc_monitor.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.3/orthanc_tools/orthanc_test_db_populator.py` & `orthanc_tools-0.8.4/orthanc_tools/orthanc_test_db_populator.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.3/orthanc_tools/pacs_migrator.py` & `orthanc_tools-0.8.4/orthanc_tools/pacs_migrator.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.3/orthanc_tools.egg-info/PKG-INFO` & `orthanc_tools-0.8.4/orthanc_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orthanc-tools
-Version: 0.8.3
+Version: 0.8.4
 Summary: Python Orthanc Tools
 Home-page: https://github.com/orthanc-team/python-orthanc-tools
 Author: Orthanc Team
 Author-email: info@orthanc.team
 Project-URL: Bug Reports, https://github.com/orthanc-team/python-orthanc-tools/issues
 Project-URL: Funding, https://orthanc.team
 Project-URL: Source, https://github.com/orthanc-team/python-orthanc-tools/
```

### Comparing `orthanc_tools-0.8.3/orthanc_tools.egg-info/SOURCES.txt` & `orthanc_tools-0.8.4/orthanc_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.3/release-notes.md` & `orthanc_tools-0.8.4/release-notes.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+v 0.8.4
+=======
+
+- `OrthancForwarder`: added error logs + retry in case of ConnectionError
+- `OrthancForwarder`: removed `worker_threads_count` that was not used anymore
+
 v 0.8.3
 =======
 
 - `OrthancForwarder`: not using `OrthancMonitor` anymore
 - `OrthancForwarder`: fixed retries
 
 v 0.8.2
```

### Comparing `orthanc_tools-0.8.3/setup.py` & `orthanc_tools-0.8.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version='0.8.3',  # Required
+    version='0.8.4',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='Python Orthanc Tools',  # Optional
 
     # This is an optional longer description of your project that represents
```

### Comparing `orthanc_tools-0.8.3/tests/test_3_orthancs.py` & `orthanc_tools-0.8.4/tests/test_3_orthancs.py`

 * *Files identical despite different names*

### Comparing `orthanc_tools-0.8.3/tests/test_old_files_deleter.py` & `orthanc_tools-0.8.4/tests/test_old_files_deleter.py`

 * *Files identical despite different names*

