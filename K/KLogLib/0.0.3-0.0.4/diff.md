# Comparing `tmp/KLogLib-0.0.3.tar.gz` & `tmp/KLogLib-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KLogLib-0.0.3.tar", last modified: Wed Apr 12 11:02:52 2023, max compression
+gzip compressed data, was "KLogLib-0.0.4.tar", last modified: Wed Apr 12 15:12:27 2023, max compression
```

## Comparing `KLogLib-0.0.3.tar` & `KLogLib-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-12 11:02:52.547098 KLogLib-0.0.3/
-drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-12 11:02:52.546045 KLogLib-0.0.3/Handlers/
--rw-r--r--   0 javier     (501) staff       (20)        0 2023-04-12 10:31:02.000000 KLogLib-0.0.3/Handlers/__init__.py
--rw-r--r--   0 javier     (501) staff       (20)      264 2023-04-12 09:40:54.000000 KLogLib-0.0.3/Handlers/byte.py
--rw-r--r--   0 javier     (501) staff       (20)     2774 2023-04-12 09:40:54.000000 KLogLib-0.0.3/Handlers/files_handler.py
-drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-12 11:02:52.546541 KLogLib-0.0.3/KLog/
--rw-r--r--   0 javier     (501) staff       (20)     1832 2023-04-12 10:31:12.000000 KLogLib-0.0.3/KLog/KLog.py
--rw-r--r--   0 javier     (501) staff       (20)        0 2023-04-12 11:00:25.000000 KLogLib-0.0.3/KLog/__init__.py
-drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-12 11:02:52.546986 KLogLib-0.0.3/KLogLib.egg-info/
--rw-r--r--   0 javier     (501) staff       (20)      138 2023-04-12 11:02:52.000000 KLogLib-0.0.3/KLogLib.egg-info/PKG-INFO
--rw-r--r--   0 javier     (501) staff       (20)      254 2023-04-12 11:02:52.000000 KLogLib-0.0.3/KLogLib.egg-info/SOURCES.txt
--rw-r--r--   0 javier     (501) staff       (20)        1 2023-04-12 11:02:52.000000 KLogLib-0.0.3/KLogLib.egg-info/dependency_links.txt
--rw-r--r--   0 javier     (501) staff       (20)       14 2023-04-12 11:02:52.000000 KLogLib-0.0.3/KLogLib.egg-info/top_level.txt
--rw-r--r--   0 javier     (501) staff       (20)     1063 2023-04-12 09:40:54.000000 KLogLib-0.0.3/LICENSE
--rw-r--r--   0 javier     (501) staff       (20)      138 2023-04-12 11:02:52.547160 KLogLib-0.0.3/PKG-INFO
--rw-r--r--   0 javier     (501) staff       (20)       41 2023-04-12 09:40:54.000000 KLogLib-0.0.3/README.md
--rw-r--r--   0 javier     (501) staff       (20)       81 2023-04-12 11:02:52.547422 KLogLib-0.0.3/setup.cfg
--rw-r--r--   0 javier     (501) staff       (20)      740 2023-04-12 11:02:46.000000 KLogLib-0.0.3/setup.py
+drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-12 15:12:27.129362 KLogLib-0.0.4/
+drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-12 15:12:27.128508 KLogLib-0.0.4/Handlers/
+-rw-r--r--   0 javier     (501) staff       (20)        0 2023-04-12 10:31:02.000000 KLogLib-0.0.4/Handlers/__init__.py
+-rw-r--r--   0 javier     (501) staff       (20)      344 2023-04-12 14:44:01.000000 KLogLib-0.0.4/Handlers/byte.py
+-rw-r--r--   0 javier     (501) staff       (20)     3170 2023-04-12 14:46:45.000000 KLogLib-0.0.4/Handlers/files_handler.py
+drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-12 15:12:27.128754 KLogLib-0.0.4/KLog/
+-rw-r--r--   0 javier     (501) staff       (20)     1927 2023-04-12 14:45:11.000000 KLogLib-0.0.4/KLog/KLog.py
+-rw-r--r--   0 javier     (501) staff       (20)        0 2023-04-12 11:00:25.000000 KLogLib-0.0.4/KLog/__init__.py
+drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-04-12 15:12:27.129252 KLogLib-0.0.4/KLogLib.egg-info/
+-rw-r--r--   0 javier     (501) staff       (20)      138 2023-04-12 15:12:27.000000 KLogLib-0.0.4/KLogLib.egg-info/PKG-INFO
+-rw-r--r--   0 javier     (501) staff       (20)      254 2023-04-12 15:12:27.000000 KLogLib-0.0.4/KLogLib.egg-info/SOURCES.txt
+-rw-r--r--   0 javier     (501) staff       (20)        1 2023-04-12 15:12:27.000000 KLogLib-0.0.4/KLogLib.egg-info/dependency_links.txt
+-rw-r--r--   0 javier     (501) staff       (20)       14 2023-04-12 15:12:27.000000 KLogLib-0.0.4/KLogLib.egg-info/top_level.txt
+-rw-r--r--   0 javier     (501) staff       (20)     1063 2023-04-12 09:40:54.000000 KLogLib-0.0.4/LICENSE
+-rw-r--r--   0 javier     (501) staff       (20)      138 2023-04-12 15:12:27.129433 KLogLib-0.0.4/PKG-INFO
+-rw-r--r--   0 javier     (501) staff       (20)     2096 2023-04-12 15:08:39.000000 KLogLib-0.0.4/README.md
+-rw-r--r--   0 javier     (501) staff       (20)       81 2023-04-12 15:12:27.129691 KLogLib-0.0.4/setup.cfg
+-rw-r--r--   0 javier     (501) staff       (20)      740 2023-04-12 11:02:46.000000 KLogLib-0.0.4/setup.py
```

### Comparing `KLogLib-0.0.3/Handlers/files_handler.py` & `KLogLib-0.0.4/Handlers/files_handler.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,43 +4,43 @@
 from datetime import datetime
 import tempfile
 
 """
     Check if file exists
 
     Arguments:
-    file: string | "/logs/log.log"
+    file:   string  |   Log file path
 """
 def file_exists(file):
     try:
         if os.path.exists(file) == False:
             create_file(file)
         return True
     except:
         raise Exception(f"There as an error.")
 
 """
     Creates the log file and directories
 
     Arguments:
-    file: string | "/logs/log.log"
+    file:   string  |   Log file path
 """
 def create_file(file):
     try:
         os.makedirs(os.path.dirname(file), exist_ok=True)
         with open(file, "w") as f:
             f.close
     except:
         raise Exception("There was an error creating Log file and directories...")
 
 """
     Write a log line in the file.
 
     Arguments:
-    log_model: LogModel() 
+    log_model:  LogModel()  |   Object with message, debug level...
 """
 def write(log_model):
     try:
         log_file = os.path.join(log_model.folder, log_model.log_name)
         
         if(log_model.is_zip == True):
             zip_log(log_file=log_file, max_size=log_model.max_size, log_folder=log_model.folder)
@@ -51,34 +51,39 @@
             f.write(f"{log_model.time}\t\t{log_model.where}\t\t{log_model.severity}\t\t{log_model.msg}")
             f.write("\n")
             f.close()
     except:
         raise Exception("There was an error writing in log file...")
     
 """
+    This method get the current log stats and check if can be zipped
 
+    Arguments:
+    log_file:   string  |   Path to the current log file
+    max_size:   double  |   Max size the log file can reach
+    log_folder: string  |   Foler where the log file is located
 """
 def zip_log(log_file, max_size, log_folder):
     try:
         file_stats = os.stat(log_file)
 
         mb = Handlers.byte.b_2_mb(size=file_stats.st_size)
 
         if mb > max_size:
             create_temp_log(log_file, log_folder)
 
     except:
         raise Exception("There was an error zipping log file")
     
 """
-This method create the temp log file and zip it
+    This method create the temp log file and zip it
 
-Arguments:
-log_file: 
-log_folder: 
+    Arguments:
+    log_file:   string  |   Log name
+    log_folder: string  |   Folder to log file
 """
 def create_temp_log(log_file, log_folder):
     try:
         temp_log_file = tempfile.NamedTemporaryFile(delete=True)
 
         with open(log_file, "r") as f:
             log_file_content = f.read()
@@ -94,18 +99,18 @@
         delete_file(log_file=temp_log_file.name)
         delete_file(log_file=log_file)
 
     except:
         raise Exception("Error creating temp file")
     
 """
-This method delete the log file
+    This method delete the log file
 
-Arguments:
-temp_log_file: string | path to the temp log
+    Arguments:
+    temp_log_file:  string  |   Path to the temp log
 """
 def delete_file(log_file):
     try:
         if os.path.exists(log_file):
             os.remove(log_file)
     except:
         raise Exception("Error deleting temp log")
```

### Comparing `KLogLib-0.0.3/KLog/KLog.py` & `KLogLib-0.0.4/KLog/KLog.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,20 +25,20 @@
             return instance
         return cls._instances[cls]
     
     """
         This method initialize the log and, if not exists creates one
 
         Arguments:
-            folder: string  | Path where Log file is located
-            log_name: srting | Name of the log
-            max_size: int | Max size the log can reach (MB)
-            is_zip: bool | Flag to set if zip and save the logs or not
-            max_zip: int | Max number of zips saved in folder
-        """
+            folder:     string  |   Path where Log file is located
+            log_name:   srting  |   Name of the log
+            max_size:   int     |   Max size the log can reach (MB)
+            is_zip:     bool    |   Flag to set if zip and save the logs or not
+            max_zip:    int     |   Max number of zips saved in folder
+    """
     def __init__(self, folder='', log_name='', max_size=10, is_zip=True, max_zip=10):
         self.folder = folder
         self.log_name = log_name
         self.max_size = max_size
         self.is_zip = is_zip
         self.max_zip = max_zip
 
@@ -46,19 +46,19 @@
 
         Handlers.files_handler.file_exists(log_file)
 
     """
         This method writes one log line
     
         Arguments:
-        where: string | 
-        severity: LogSeverity(Enum) | Default value "DEBUG"
-        msg: string |
+        where:      string  |   Class/method where message calls
+        severity:   Enum    |   Default value "DEBUG"
+        msg:        string  |   Log line to print
     """
-    def write(self, where='', severity=LogSeverity.DEBUG, msg=''):
+    def write(self, where='', msg='', severity=LogSeverity.DEBUG):
         time = datetime.now()
         self.time = time
         self.where = where
         self.severity = severity.value
         self.msg = msg
 
         Handlers.files_handler.write(self)
```

### Comparing `KLogLib-0.0.3/LICENSE` & `KLogLib-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `KLogLib-0.0.3/setup.py` & `KLogLib-0.0.4/setup.py`

 * *Files identical despite different names*

