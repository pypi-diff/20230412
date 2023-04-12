# Comparing `tmp/rosbag-tools-0.0.2.tar.gz` & `tmp/rosbag-tools-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rosbag-tools-0.0.2.tar", last modified: Sun Apr  2 19:40:14 2023, max compression
+gzip compressed data, was "rosbag-tools-0.0.3.tar", last modified: Wed Apr 12 02:35:06 2023, max compression
```

## Comparing `rosbag-tools-0.0.2.tar` & `rosbag-tools-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,28 @@
--rw-r--r--   0        0        0     3379 2023-03-17 15:49:54.782651 rosbag-tools-0.0.2/.gitignore
--rw-r--r--   0        0        0      138 2023-04-02 19:33:02.392052 rosbag-tools-0.0.2/CHANGELOG.rst
--rw-r--r--   0        0        0    35149 2023-03-17 15:52:10.448091 rosbag-tools-0.0.2/LICENSE
--rw-r--r--   0        0        0     1615 2023-04-02 16:09:03.884163 rosbag-tools-0.0.2/README.md
--rw-r--r--   0        0        0     1353 2023-04-02 16:08:15.501652 rosbag-tools-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       36 2023-03-17 18:49:09.050747 rosbag-tools-0.0.2/requirements.txt
--rw-r--r--   0        0        0       31 2023-03-17 18:52:52.111373 rosbag-tools-0.0.2/requirements/requirements-build.txt
--rw-r--r--   0        0        0       36 2023-03-17 18:49:33.386818 rosbag-tools-0.0.2/requirements/requirements-common.txt
--rw-r--r--   0        0        0       51 2023-03-17 15:44:29.037370 rosbag-tools-0.0.2/requirements/requirements-dev.txt
--rw-r--r--   0        0        0      114 2023-04-02 19:39:40.226247 rosbag-tools-0.0.2/setup.cfg
--rw-r--r--   0        0        0      162 2023-04-02 19:39:40.210247 rosbag-tools-0.0.2/src/rosbag_tools/__init__.py
--rw-r--r--   0        0        0      418 2023-04-02 17:08:41.932568 rosbag-tools-0.0.2/src/rosbag_tools/__main__.py
--rw-r--r--   0        0        0     2731 2023-04-02 16:28:13.591750 rosbag-tools-0.0.2/src/rosbag_tools/topic_compare/README.md
--rw-r--r--   0        0        0      200 2023-03-22 22:10:57.475321 rosbag-tools-0.0.2/src/rosbag_tools/topic_compare/__init__.py
--rw-r--r--   0        0        0      196 2023-04-02 16:02:31.456070 rosbag-tools-0.0.2/src/rosbag_tools/topic_compare/__main__.py
--rw-r--r--   0        0        0     1272 2023-03-22 22:41:54.727167 rosbag-tools-0.0.2/src/rosbag_tools/topic_compare/main.py
--rw-r--r--   0        0        0     8897 2023-04-02 16:11:15.356788 rosbag-tools-0.0.2/src/rosbag_tools/topic_compare/topic_comparator.py
--rw-r--r--   0        0        0     2150 2023-04-02 16:45:33.125338 rosbag-tools-0.0.2/src/rosbag_tools/topic_remove/README.md
--rw-r--r--   0        0        0      173 2023-04-02 15:57:06.998154 rosbag-tools-0.0.2/src/rosbag_tools/topic_remove/__init__.py
--rw-r--r--   0        0        0      155 2023-04-02 16:02:38.964118 rosbag-tools-0.0.2/src/rosbag_tools/topic_remove/__main__.py
--rw-r--r--   0        0        0     1321 2023-04-02 17:14:16.803923 rosbag-tools-0.0.2/src/rosbag_tools/topic_remove/main.py
--rw-r--r--   0        0        0     8077 2023-04-02 16:24:53.316259 rosbag-tools-0.0.2/src/rosbag_tools/topic_remove/topic_remover.py
--rw-r--r--   0        0        0     2848 1970-01-01 00:00:00.000000 rosbag-tools-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     3379 2023-03-17 15:49:54.782651 rosbag-tools-0.0.3/.gitignore
+-rw-r--r--   0        0        0      307 2023-04-12 02:31:41.509823 rosbag-tools-0.0.3/CHANGELOG.rst
+-rw-r--r--   0        0        0    35149 2023-03-17 15:52:10.448091 rosbag-tools-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1699 2023-04-12 02:24:50.592581 rosbag-tools-0.0.3/README.md
+-rw-r--r--   0        0        0     1353 2023-04-02 16:08:15.501652 rosbag-tools-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       36 2023-03-17 18:49:09.050747 rosbag-tools-0.0.3/requirements.txt
+-rw-r--r--   0        0        0       31 2023-03-17 18:52:52.111373 rosbag-tools-0.0.3/requirements/requirements-build.txt
+-rw-r--r--   0        0        0       36 2023-03-17 18:49:33.386818 rosbag-tools-0.0.3/requirements/requirements-common.txt
+-rw-r--r--   0        0        0       51 2023-03-17 15:44:29.037370 rosbag-tools-0.0.3/requirements/requirements-dev.txt
+-rw-r--r--   0        0        0      114 2023-04-12 02:32:32.216676 rosbag-tools-0.0.3/setup.cfg
+-rw-r--r--   0        0        0      185 2023-04-12 02:32:32.216676 rosbag-tools-0.0.3/src/rosbag_tools/__init__.py
+-rw-r--r--   0        0        0      451 2023-04-10 22:15:21.772989 rosbag-tools-0.0.3/src/rosbag_tools/__main__.py
+-rw-r--r--   0        0        0     2118 2023-04-12 02:24:02.487974 rosbag-tools-0.0.3/src/rosbag_tools/clip/README.md
+-rw-r--r--   0        0        0      149 2023-04-10 22:01:33.492666 rosbag-tools-0.0.3/src/rosbag_tools/clip/__init__.py
+-rw-r--r--   0        0        0      150 2023-04-10 22:01:50.796785 rosbag-tools-0.0.3/src/rosbag_tools/clip/__main__.py
+-rw-r--r--   0        0        0     8274 2023-04-12 02:15:13.665485 rosbag-tools-0.0.3/src/rosbag_tools/clip/clipper.py
+-rw-r--r--   0        0        0     1826 2023-04-12 01:37:38.974167 rosbag-tools-0.0.3/src/rosbag_tools/clip/main.py
+-rw-r--r--   0        0        0     2731 2023-04-02 16:28:13.591750 rosbag-tools-0.0.3/src/rosbag_tools/topic_compare/README.md
+-rw-r--r--   0        0        0      200 2023-03-22 22:10:57.475321 rosbag-tools-0.0.3/src/rosbag_tools/topic_compare/__init__.py
+-rw-r--r--   0        0        0      196 2023-04-02 16:02:31.456070 rosbag-tools-0.0.3/src/rosbag_tools/topic_compare/__main__.py
+-rw-r--r--   0        0        0     1272 2023-03-22 22:41:54.727167 rosbag-tools-0.0.3/src/rosbag_tools/topic_compare/main.py
+-rw-r--r--   0        0        0     8895 2023-04-12 01:34:24.670607 rosbag-tools-0.0.3/src/rosbag_tools/topic_compare/topic_comparator.py
+-rw-r--r--   0        0        0     2039 2023-04-05 03:10:27.560346 rosbag-tools-0.0.3/src/rosbag_tools/topic_remove/README.md
+-rw-r--r--   0        0        0      173 2023-04-02 15:57:06.998154 rosbag-tools-0.0.3/src/rosbag_tools/topic_remove/__init__.py
+-rw-r--r--   0        0        0      155 2023-04-02 16:02:38.964118 rosbag-tools-0.0.3/src/rosbag_tools/topic_remove/__main__.py
+-rw-r--r--   0        0        0     1323 2023-04-04 15:50:05.420416 rosbag-tools-0.0.3/src/rosbag_tools/topic_remove/main.py
+-rw-r--r--   0        0        0     8082 2023-04-04 15:50:29.948454 rosbag-tools-0.0.3/src/rosbag_tools/topic_remove/topic_remover.py
+-rw-r--r--   0        0        0     2932 1970-01-01 00:00:00.000000 rosbag-tools-0.0.3/PKG-INFO
```

### Comparing `rosbag-tools-0.0.2/.gitignore` & `rosbag-tools-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `rosbag-tools-0.0.2/LICENSE` & `rosbag-tools-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rosbag-tools-0.0.2/README.md` & `rosbag-tools-0.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 ```sh
 pip install rosbag-tools[plot]
 ```
 
 ## Tools
 
 * [`topic-compare`](src/rosbag_tools/topic_compare)
+* [`topic-remove`](src/rosbag_tools/topic_remove)
+* [`clip`](src/rosbag_tools/clip)
 
 ## Usage
 
 Each tool in `rosbag-tools` can be used both as a command line application and in Python code.
 
 ### Command line
```

### Comparing `rosbag-tools-0.0.2/pyproject.toml` & `rosbag-tools-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rosbag-tools-0.0.2/src/rosbag_tools/topic_compare/README.md` & `rosbag-tools-0.0.3/src/rosbag_tools/topic_compare/README.md`

 * *Files identical despite different names*

### Comparing `rosbag-tools-0.0.2/src/rosbag_tools/topic_compare/main.py` & `rosbag-tools-0.0.3/src/rosbag_tools/topic_compare/main.py`

 * *Files identical despite different names*

### Comparing `rosbag-tools-0.0.2/src/rosbag_tools/topic_compare/topic_comparator.py` & `rosbag-tools-0.0.3/src/rosbag_tools/topic_compare/topic_comparator.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         Returns:
             RosbagComparator: Instance of RosbagComparator
         """
         with open(yaml_path, "r", encoding="utf-8") as file:
             return cls.from_dict(yaml.safe_load(file))
 
     def extract_data(self) -> None:
-        """Extract all the topics cointaned in the rosbags at the path {self.folder}"""
+        """Extract all the topics contained in the rosbags in the path self.folder"""
         paths_ros1 = self.folder.glob("*.bag")
         paths_ros2 = (p.parent for p in self.folder.glob("**/*.db3"))
         paths = list(paths_ros1) + list(paths_ros2)
 
         if len(paths) == 0:
             # Empty list of paths
             raise RuntimeWarning(f"Specified folder {self.folder} contains no bagfiles")
```

### Comparing `rosbag-tools-0.0.2/src/rosbag_tools/topic_remove/README.md` & `rosbag-tools-0.0.3/src/rosbag_tools/topic_remove/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # `topic-remove`
 
 > filter out topics from a rosbag
 
 ## Use case
 
-Say you have too much topics in a rosbag (ROS1 or ROS2) and that you want to keep a copy of this rosbag without data from a specific sensor. `rosbag-tools topic-remove` will :
+Say you have too much topics in a rosbag (ROS 1 or ROS 2) and that you want to keep a copy of this rosbag without data from a specific sensor. `rosbag-tools topic-remove` will :
 
 * Filter out topics based on their name
 * Filter out topics based on [glob](https://en.wikipedia.org/wiki/Glob_(programming))-like wildcard patterns
 * Preserve your original rosbag
 
 ## Usage
 
@@ -23,39 +23,37 @@
 rosbag-tools topic-remove /path/to/rosbag -t *sensor*
 ```
 
 Here are all the CLI options of `rosbag-tools topic-remove`:
 
 ```console
 $ rosbag-tools topic-remove -h
-usage: rosbag-tools topic-remove [-h] [-o OUTBAG] [-t TOPICS [TOPICS ...]] [-f]
-                           inbag
+Usage: rosbag-tools topic-remove [OPTIONS] INBAG
 
-positional arguments:
-  inbag                 Input bag
+  Remove topics from INBAG
 
-options:
-  -h, --help            show this help message and exit
-  -o OUTBAG, --output OUTBAG, --outbag OUTBAG
-                        Filtered bag
-  -t TOPICS [TOPICS ...], --topics TOPICS [TOPICS ...]
-                        Topics to remove from the rosbag
-  -f, --force           Force output file overwriting
+  INBAG is the path to a rosbag file
+  Can be a bag in ROS 1 or in ROS 2
 
+Options:
+  -o, --output, --outbag TEXT  Filtered bag. Defaults to INBAG_filt
+  -t, --topics TEXT
+  -f, --force-overwriting      Force output file overwriting
+  -h, --help                   Show this message and exit.
 ```
 
 ### Python Code API
 
 You can also call `rosbag-tools topic-remove` directly into your Python code :
 
 ```py
 from rosbag_tools.topic_remove import BagTopicRemover
 
-data_path = "path/to/a/rosbag.bag"  # ROS1
-data_path = "path/to/a/rosbag"  # ROS2
+data_path = "path/to/a/rosbag.bag"  # ROS 1
+data_path = "path/to/a/rosbag"  # ROS 2
 topic_remover = BagTopicRemover(data_path)
 
 # Change the input bag
 topic_remover.inbag = "path/to/another/rosbag"
 
 # Remove /cmd_vel
 topic_remover.remove("/cmd_vel")
@@ -66,10 +64,10 @@
 # Remove all camera info topics
 topic_remover.remove("/*/camera_info")
 
 # Remove all topics from the IMU and from the GPS
 topic_remover.remove(("/imu/*", "/gps/*"))
 
 # Export a rosbag with all topics filtered
-topic_remover.export("path/to/save/this/filtered/rosbag.bag")  # ROS1
-topic_remover.export("path/to/save/that/filtered/rosbag")  # ROS2
+topic_remover.export("path/to/save/this/filtered/rosbag.bag")  # ROS 1
+topic_remover.export("path/to/save/that/filtered/rosbag")  # ROS 2
 ```
```

### Comparing `rosbag-tools-0.0.2/src/rosbag_tools/topic_remove/main.py` & `rosbag-tools-0.0.3/src/rosbag_tools/topic_remove/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     help="Force output file overwriting",
     is_flag=True,
 )
 def cli(inbag, outbag, topics, force):
     """Remove topics from INBAG
 
     INBAG is the path to a rosbag file
-    Can be a bag in ROS1 or in ROS2
+    Can be a bag in ROS 1 or in ROS 2
     """
     inpath = Path(inbag)
     outpath = Path(outbag)
 
     rosbag_rem = BagTopicRemover(inbag)
     rosbag_rem.remove(topics)
     if outpath:
```

### Comparing `rosbag-tools-0.0.2/src/rosbag_tools/topic_remove/topic_remover.py` & `rosbag-tools-0.0.3/src/rosbag_tools/topic_remove/topic_remover.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,15 +167,15 @@
             self.delete_rosbag(outpath)
 
         # Reader / Writer classes
         Reader = self.get_reader_class(self.inbag)
         Writer = self.get_writer_class(path)
         if self._is_ros1_reader != self._is_ros1_writer:
             raise NotImplementedError(
-                "Rosbag conversion (ROS1->ROS2 / ROS2->ROS1) is not supported. "
+                "Rosbag conversion (ROS 1->ROS 2 / ROS 2->ROS 1) is not supported. "
                 "Use `rosbags` to convert your rosbag before using `rosbag-tools topic-remove`."
             )
         with Reader(self.inbag) as reader, Writer(outpath) as writer:
             conn_map = {}
             ConnectionExt = (
                 ConnectionExtRosbag1 if self._is_ros1_writer else ConnectionExtRosbag2
             )
@@ -188,15 +188,15 @@
                             conn.msgtype,
                             conn.msgdef,
                             conn.md5sum,
                             ext.callerid,
                             ext.latching,
                         )
                     else:
-                        # ROS2
+                        # ROS 2
                         conn_map[conn.id] = writer.add_connection(
                             conn.topic,
                             conn.msgtype,
                             ext.serialization_format,
                             ext.offered_qos_profiles,
                         )
```

### Comparing `rosbag-tools-0.0.2/PKG-INFO` & `rosbag-tools-0.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosbag-tools
-Version: 0.0.2
+Version: 0.0.3
 Summary: A ROS-agnostic toolbox for common rosbag operations
 Author-email: damienlarocque <phicoltan@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -47,14 +47,16 @@
 ```sh
 pip install rosbag-tools[plot]
 ```
 
 ## Tools
 
 * [`topic-compare`](src/rosbag_tools/topic_compare)
+* [`topic-remove`](src/rosbag_tools/topic_remove)
+* [`clip`](src/rosbag_tools/clip)
 
 ## Usage
 
 Each tool in `rosbag-tools` can be used both as a command line application and in Python code.
 
 ### Command line
```

