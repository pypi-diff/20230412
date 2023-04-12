# Comparing `tmp/MomentumX-2.6.3.tar.gz` & `tmp/MomentumX-2.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MomentumX-2.6.3.tar", last modified: Fri Mar 10 17:06:07 2023, max compression
+gzip compressed data, was "MomentumX-2.6.4.tar", last modified: Wed Apr 12 13:24:07 2023, max compression
```

## Comparing `MomentumX-2.6.3.tar` & `MomentumX-2.6.4.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-03-10 17:06:07.040301 MomentumX-2.6.3/
--rw-rw-r--   0 developer  (1000) developer  (1000)      143 2023-02-05 03:27:25.000000 MomentumX-2.6.3/.clang-format
--rw-rw-r--   0 developer  (1000) developer  (1000)       39 2023-01-04 18:56:42.000000 MomentumX-2.6.3/.dockerignore
--rw-rw-r--   0 developer  (1000) developer  (1000)       93 2023-03-02 22:42:30.000000 MomentumX-2.6.3/.gitignore
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-03-10 17:06:07.035801 MomentumX-2.6.3/.vscode/
--rw-rw-r--   0 developer  (1000) developer  (1000)      280 2023-03-02 22:42:30.000000 MomentumX-2.6.3/.vscode/settings.json
--rw-rw-r--   0 developer  (1000) developer  (1000)     1968 2023-03-09 18:12:19.000000 MomentumX-2.6.3/CMakeLists.txt
--rw-rw-r--   0 developer  (1000) developer  (1000)    35149 2022-05-19 01:23:36.000000 MomentumX-2.6.3/LICENSE
--rwxrwxr-x   0 developer  (1000) developer  (1000)     6518 2023-01-10 14:44:56.000000 MomentumX-2.6.3/Logo.png
--rw-rw-r--   0 developer  (1000) developer  (1000)     1359 2023-03-09 18:12:19.000000 MomentumX-2.6.3/Makefile
--rw-rw-r--   0 developer  (1000) developer  (1000)     7125 2023-03-10 17:06:07.040301 MomentumX-2.6.3/PKG-INFO
--rw-rw-r--   0 developer  (1000) developer  (1000)     6667 2023-03-10 16:59:42.000000 MomentumX-2.6.3/README.md
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-03-10 17:06:07.036701 MomentumX-2.6.3/examples/
--rw-rw-r--   0 developer  (1000) developer  (1000)     1675 2023-03-09 18:12:19.000000 MomentumX-2.6.3/examples/multi.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     1120 2023-03-09 18:12:19.000000 MomentumX-2.6.3/examples/stream_reader.py
--rwxrwxr-x   0 developer  (1000) developer  (1000)      865 2023-03-09 18:12:19.000000 MomentumX-2.6.3/examples/stream_writer.py
--rw-rw-r--   0 developer  (1000) developer  (1000)      736 2023-03-09 18:12:19.000000 MomentumX-2.6.3/examples/sync_reader.py
--rwxrwxr-x   0 developer  (1000) developer  (1000)      545 2023-03-09 18:12:19.000000 MomentumX-2.6.3/examples/sync_writer.py
--rw-rw-r--   0 developer  (1000) developer  (1000)      943 2023-03-09 18:12:19.000000 MomentumX-2.6.3/examples/threaded.py
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-03-10 17:06:07.039401 MomentumX-2.6.3/ext/
--rw-rw-r--   0 developer  (1000) developer  (1000)    22185 2023-03-10 16:20:18.000000 MomentumX-2.6.3/ext/binding.cpp
--rw-rw-r--   0 developer  (1000) developer  (1000)     6517 2023-03-09 18:12:19.000000 MomentumX-2.6.3/ext/buffer.cpp
--rw-rw-r--   0 developer  (1000) developer  (1000)     4214 2023-03-09 18:12:19.000000 MomentumX-2.6.3/ext/buffer.h
--rw-rw-r--   0 developer  (1000) developer  (1000)     4748 2023-03-10 15:53:52.000000 MomentumX-2.6.3/ext/context.cpp
--rw-rw-r--   0 developer  (1000) developer  (1000)     1467 2023-03-10 15:53:52.000000 MomentumX-2.6.3/ext/context.h
--rw-rw-r--   0 developer  (1000) developer  (1000)    20326 2023-03-10 15:53:52.000000 MomentumX-2.6.3/ext/stream.cpp
--rw-rw-r--   0 developer  (1000) developer  (1000)     5141 2023-03-10 15:53:52.000000 MomentumX-2.6.3/ext/stream.h
--rw-rw-r--   0 developer  (1000) developer  (1000)     9498 2023-03-09 18:12:19.000000 MomentumX-2.6.3/ext/utils.h
--rw-rw-r--   0 developer  (1000) developer  (1000)      126 2023-01-05 01:48:10.000000 MomentumX-2.6.3/pyproject.toml
--rw-rw-r--   0 developer  (1000) developer  (1000)       38 2023-03-10 17:06:07.040301 MomentumX-2.6.3/setup.cfg
--rw-rw-r--   0 developer  (1000) developer  (1000)     1023 2023-03-10 16:57:00.000000 MomentumX-2.6.3/setup.py
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-03-10 17:06:07.034001 MomentumX-2.6.3/src/
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-03-10 17:06:07.039401 MomentumX-2.6.3/src/MomentumX.egg-info/
--rw-rw-r--   0 developer  (1000) developer  (1000)     7125 2023-03-10 17:06:06.000000 MomentumX-2.6.3/src/MomentumX.egg-info/PKG-INFO
--rw-rw-r--   0 developer  (1000) developer  (1000)      644 2023-03-10 17:06:06.000000 MomentumX-2.6.3/src/MomentumX.egg-info/SOURCES.txt
--rw-rw-r--   0 developer  (1000) developer  (1000)        1 2023-03-10 17:06:06.000000 MomentumX-2.6.3/src/MomentumX.egg-info/dependency_links.txt
--rw-rw-r--   0 developer  (1000) developer  (1000)       21 2023-03-10 17:06:06.000000 MomentumX-2.6.3/src/MomentumX.egg-info/requires.txt
--rw-rw-r--   0 developer  (1000) developer  (1000)       10 2023-03-10 17:06:06.000000 MomentumX-2.6.3/src/MomentumX.egg-info/top_level.txt
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-03-10 17:06:07.040301 MomentumX-2.6.3/src/momentumx/
--rw-rw-r--   0 developer  (1000) developer  (1000)       20 2023-03-02 22:39:27.000000 MomentumX-2.6.3/src/momentumx/__init__.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     4607 2023-03-10 16:27:51.000000 MomentumX-2.6.3/src/momentumx/_mx.pyi
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-03-10 17:06:07.040301 MomentumX-2.6.3/tests/
--rw-rw-r--   0 developer  (1000) developer  (1000)    26794 2023-03-10 16:25:04.000000 MomentumX-2.6.3/tests/test_scenarios.py
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-04-12 13:24:07.301698 MomentumX-2.6.4/
+-rw-rw-r--   0 developer  (1000) developer  (1000)      143 2023-02-05 03:27:25.000000 MomentumX-2.6.4/.clang-format
+-rw-rw-r--   0 developer  (1000) developer  (1000)       39 2023-01-04 18:56:42.000000 MomentumX-2.6.4/.dockerignore
+-rw-rw-r--   0 developer  (1000) developer  (1000)       93 2023-03-02 22:42:30.000000 MomentumX-2.6.4/.gitignore
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-04-12 13:24:07.295286 MomentumX-2.6.4/.vscode/
+-rw-rw-r--   0 developer  (1000) developer  (1000)      280 2023-03-02 22:42:30.000000 MomentumX-2.6.4/.vscode/settings.json
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1968 2023-03-09 18:12:19.000000 MomentumX-2.6.4/CMakeLists.txt
+-rw-rw-r--   0 developer  (1000) developer  (1000)    35149 2022-05-19 01:23:36.000000 MomentumX-2.6.4/LICENSE
+-rwxrwxr-x   0 developer  (1000) developer  (1000)     6518 2023-01-10 14:44:56.000000 MomentumX-2.6.4/Logo.png
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1359 2023-03-09 18:12:19.000000 MomentumX-2.6.4/Makefile
+-rw-rw-r--   0 developer  (1000) developer  (1000)     7125 2023-04-12 13:24:07.301698 MomentumX-2.6.4/PKG-INFO
+-rw-rw-r--   0 developer  (1000) developer  (1000)     6667 2023-03-10 16:59:42.000000 MomentumX-2.6.4/README.md
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-04-12 13:24:07.297118 MomentumX-2.6.4/examples/
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1675 2023-03-09 18:12:19.000000 MomentumX-2.6.4/examples/multi.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1120 2023-03-09 18:12:19.000000 MomentumX-2.6.4/examples/stream_reader.py
+-rwxrwxr-x   0 developer  (1000) developer  (1000)      865 2023-03-09 18:12:19.000000 MomentumX-2.6.4/examples/stream_writer.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)      762 2023-04-12 13:12:35.000000 MomentumX-2.6.4/examples/sync_reader.py
+-rwxrwxr-x   0 developer  (1000) developer  (1000)      583 2023-04-12 13:12:35.000000 MomentumX-2.6.4/examples/sync_writer.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)      943 2023-03-09 18:12:19.000000 MomentumX-2.6.4/examples/threaded.py
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-04-12 13:24:07.298950 MomentumX-2.6.4/ext/
+-rw-rw-r--   0 developer  (1000) developer  (1000)    22185 2023-03-10 16:20:18.000000 MomentumX-2.6.4/ext/binding.cpp
+-rw-rw-r--   0 developer  (1000) developer  (1000)     6517 2023-03-09 18:12:19.000000 MomentumX-2.6.4/ext/buffer.cpp
+-rw-rw-r--   0 developer  (1000) developer  (1000)     4214 2023-03-09 18:12:19.000000 MomentumX-2.6.4/ext/buffer.h
+-rw-rw-r--   0 developer  (1000) developer  (1000)     4748 2023-03-10 15:53:52.000000 MomentumX-2.6.4/ext/context.cpp
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1467 2023-03-10 15:53:52.000000 MomentumX-2.6.4/ext/context.h
+-rw-rw-r--   0 developer  (1000) developer  (1000)    21067 2023-04-12 13:12:35.000000 MomentumX-2.6.4/ext/stream.cpp
+-rw-rw-r--   0 developer  (1000) developer  (1000)     5141 2023-03-10 15:53:52.000000 MomentumX-2.6.4/ext/stream.h
+-rw-rw-r--   0 developer  (1000) developer  (1000)     9498 2023-03-09 18:12:19.000000 MomentumX-2.6.4/ext/utils.h
+-rw-rw-r--   0 developer  (1000) developer  (1000)      126 2023-01-05 01:48:10.000000 MomentumX-2.6.4/pyproject.toml
+-rw-rw-r--   0 developer  (1000) developer  (1000)       38 2023-04-12 13:24:07.301698 MomentumX-2.6.4/setup.cfg
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1023 2023-04-12 13:13:27.000000 MomentumX-2.6.4/setup.py
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-04-12 13:24:07.290705 MomentumX-2.6.4/src/
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-04-12 13:24:07.299866 MomentumX-2.6.4/src/MomentumX.egg-info/
+-rw-rw-r--   0 developer  (1000) developer  (1000)     7125 2023-04-12 13:24:07.000000 MomentumX-2.6.4/src/MomentumX.egg-info/PKG-INFO
+-rw-rw-r--   0 developer  (1000) developer  (1000)      665 2023-04-12 13:24:07.000000 MomentumX-2.6.4/src/MomentumX.egg-info/SOURCES.txt
+-rw-rw-r--   0 developer  (1000) developer  (1000)        1 2023-04-12 13:24:07.000000 MomentumX-2.6.4/src/MomentumX.egg-info/dependency_links.txt
+-rw-rw-r--   0 developer  (1000) developer  (1000)       21 2023-04-12 13:24:07.000000 MomentumX-2.6.4/src/MomentumX.egg-info/requires.txt
+-rw-rw-r--   0 developer  (1000) developer  (1000)       10 2023-04-12 13:24:07.000000 MomentumX-2.6.4/src/MomentumX.egg-info/top_level.txt
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-04-12 13:24:07.300782 MomentumX-2.6.4/src/momentumx/
+-rw-rw-r--   0 developer  (1000) developer  (1000)       20 2023-03-02 22:39:27.000000 MomentumX-2.6.4/src/momentumx/__init__.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     4607 2023-04-12 13:16:01.000000 MomentumX-2.6.4/src/momentumx/_mx.pyi
+-rw-rw-r--   0 developer  (1000) developer  (1000)        0 2023-03-17 18:13:12.000000 MomentumX-2.6.4/src/momentumx/cli.py
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-04-12 13:24:07.300782 MomentumX-2.6.4/tests/
+-rw-rw-r--   0 developer  (1000) developer  (1000)    27378 2023-04-12 13:12:35.000000 MomentumX-2.6.4/tests/test_scenarios.py
```

### Comparing `MomentumX-2.6.3/CMakeLists.txt` & `MomentumX-2.6.4/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `MomentumX-2.6.3/LICENSE` & `MomentumX-2.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `MomentumX-2.6.3/Logo.png` & `MomentumX-2.6.4/Logo.png`

 * *Files identical despite different names*

### Comparing `MomentumX-2.6.3/Makefile` & `MomentumX-2.6.4/Makefile`

 * *Files identical despite different names*

### Comparing `MomentumX-2.6.3/PKG-INFO` & `MomentumX-2.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MomentumX
-Version: 2.6.3
+Version: 2.6.4
 Summary: Zero-copy shared memory IPC library for building complex streaming data pipelines capable of processing large datasets
 Home-page: https://github.com/captivationsoftware/MomentumX
 Author: Captivation Software, LLC
 Keywords: shm,shared memory,zero-copy,numpy,big data,scipy,pubsub,pipeline
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `MomentumX-2.6.3/README.md` & `MomentumX-2.6.4/README.md`

 * *Files identical despite different names*

### Comparing `MomentumX-2.6.3/examples/multi.py` & `MomentumX-2.6.4/examples/multi.py`

 * *Files identical despite different names*

### Comparing `MomentumX-2.6.3/examples/stream_reader.py` & `MomentumX-2.6.4/examples/stream_reader.py`

 * *Files identical despite different names*

### Comparing `MomentumX-2.6.3/examples/stream_writer.py` & `MomentumX-2.6.4/examples/stream_writer.py`

 * *Files identical despite different names*

### Comparing `MomentumX-2.6.3/examples/sync_reader.py` & `MomentumX-2.6.4/examples/sync_reader.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 while stream.has_next:
     string = stream.receive_string()
     if string:
         if prev_val is None:
             prev_val = int(string)
         else:
             trial = int(string)
-            assert trial == prev_val + 1, "Counter error"
+            assert trial == prev_val + 1, f"Counter error: {trial} != {prev_val+1}"
             prev_val = trial
         print("Received:", string)
     else:
         if cancel.wait(0.5):
             break
         print("Waiting for data")
 print(stream.has_next)
```

### Comparing `MomentumX-2.6.3/examples/sync_writer.py` & `MomentumX-2.6.4/examples/sync_writer.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,12 +12,15 @@
 
 stream = mx.Producer(STREAM, 100, 10, True, cancel)
 while stream.subscriber_count == 0:
     print("waiting for subscriber(s)")
     if cancel.wait(0.5):
         break
 
-for n in range(1, 500000):
+
+n = 0
+while not cancel.is_set() and  n < 500000:
     if stream.subscriber_count == 0:
         cancel.wait(0.5)
     elif stream.send_string(str(n)):
         print(f"Sent: {n}")
+        n += 1
```

### Comparing `MomentumX-2.6.3/examples/threaded.py` & `MomentumX-2.6.4/examples/threaded.py`

 * *Files identical despite different names*

### Comparing `MomentumX-2.6.3/ext/binding.cpp` & `MomentumX-2.6.4/ext/binding.cpp`

 * *Files identical despite different names*

### Comparing `MomentumX-2.6.3/ext/buffer.cpp` & `MomentumX-2.6.4/ext/buffer.cpp`

 * *Files identical despite different names*

### Comparing `MomentumX-2.6.3/ext/buffer.h` & `MomentumX-2.6.4/ext/buffer.h`

 * *Files identical despite different names*

### Comparing `MomentumX-2.6.3/ext/context.cpp` & `MomentumX-2.6.4/ext/context.cpp`

 * *Files identical despite different names*

### Comparing `MomentumX-2.6.3/ext/context.h` & `MomentumX-2.6.4/ext/context.h`

 * *Files identical despite different names*

### Comparing `MomentumX-2.6.3/ext/stream.cpp` & `MomentumX-2.6.4/ext/stream.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -60,22 +60,33 @@
             new (_control) ControlBlock();  // placement construct into shared memory
             const auto control_lock = get_control_lock();
             _control->sync = sync;
             _control->buffer_size = buffer_size;
             _control->buffer_count = buffer_count;
             Utils::Logger::get_logger().info(std::string("Created Producer Stream (" + std::to_string((uint64_t)this) + ")"));
         } else {
-            const auto control_lock = get_control_lock();
+            auto control_lock = get_control_lock();
             if (!_control->is_ready()) {
                 throw std::runtime_error("Attempt to open stream before it is ready");
             }
             _control->subscriber_count++;
             if (_control->sync) {
-                _last_index = _control->last_sent_index;
-                _last_iteration = _control->last_sent_iteration();
+                const auto index_iterations = _control->sorted_index_iterations(control_lock);
+                if (index_iterations.size() != 0) {
+                    // If any previous iterations, set to just before the oldest still-rechable buffer
+                    const auto dec = [&](size_t idx) { return ControlBlock::wrapping_decrement(idx, _control->buffer_count); };
+                    _last_index = dec(std::get<0>(index_iterations.at(0)));     // prevous index, so next increment places us at oldest
+                    _last_iteration = std::get<1>(index_iterations.at(0)) - 1;  // value when the previous increment was created
+
+                    for (auto ii : index_iterations) {
+                        const auto idx = std::get<0>(ii);
+                        auto& bsync = _control->buffers.at(idx).buffer_sync;
+                        bsync.inc_required(control_lock);
+                    }
+                }
             }
             _subscribed = true;
 
             Utils::Logger::get_logger().info(std::string("Created Consumer Stream (" + std::to_string((uint64_t)this) + ")"));
         }
 
         // Initialize any cached variables that will remain for the duration of the stream to prevent extraneous locking...
@@ -396,15 +407,15 @@
         const size_t last_sent_idx = stream->_control->last_sent_index;
         const size_t last_read_iteration = stream->_last_iteration;
         const size_t last_sent_iteration = stream->_control->buffers.at(last_sent_idx).buffer_state.iteration;
         if (last_sent_iteration == last_read_iteration) {
             return nullptr;  // TODO: block once we've caught up, instead of just bailing like we are now
         }
 
-        size_t next_idx = ControlBlock::wrapping_increment(last_read_idx, stream->_control->buffer_count);
+        size_t next_idx = inc(last_read_idx);
         size_t next_expected_iteration = last_read_iteration + 1;
 
         auto b = std::ref(stream->_control->buffers.at(next_idx));
 
         // In the simple case, the next buffer (sequentially) is used.
         // If that's not the case, we'll have to search for the next available buffer.
         // NOTE: `sync` mode requires each buffer to be used sequentially, so this is effectively a no-op in `sync` mode.
```

### Comparing `MomentumX-2.6.3/ext/stream.h` & `MomentumX-2.6.4/ext/stream.h`

 * *Files identical despite different names*

### Comparing `MomentumX-2.6.3/ext/utils.h` & `MomentumX-2.6.4/ext/utils.h`

 * *Files identical despite different names*

### Comparing `MomentumX-2.6.3/setup.py` & `MomentumX-2.6.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_packages
 from skbuild import setup
 
-__version__ = "2.6.3"
+__version__ = "2.6.4"
 
 from pathlib import Path
 long_description = (Path(__file__).parent / "README.md").read_text()
 
 setup(
     name="MomentumX",
     version=__version__,
```

### Comparing `MomentumX-2.6.3/src/MomentumX.egg-info/PKG-INFO` & `MomentumX-2.6.4/src/MomentumX.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MomentumX
-Version: 2.6.3
+Version: 2.6.4
 Summary: Zero-copy shared memory IPC library for building complex streaming data pipelines capable of processing large datasets
 Home-page: https://github.com/captivationsoftware/MomentumX
 Author: Captivation Software, LLC
 Keywords: shm,shared memory,zero-copy,numpy,big data,scipy,pubsub,pipeline
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `MomentumX-2.6.3/src/MomentumX.egg-info/SOURCES.txt` & `MomentumX-2.6.4/src/MomentumX.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -26,8 +26,9 @@
 src/MomentumX.egg-info/PKG-INFO
 src/MomentumX.egg-info/SOURCES.txt
 src/MomentumX.egg-info/dependency_links.txt
 src/MomentumX.egg-info/requires.txt
 src/MomentumX.egg-info/top_level.txt
 src/momentumx/__init__.py
 src/momentumx/_mx.pyi
+src/momentumx/cli.py
 tests/test_scenarios.py
```

### Comparing `MomentumX-2.6.3/src/momentumx/_mx.pyi` & `MomentumX-2.6.4/src/momentumx/_mx.pyi`

 * *Files identical despite different names*

### Comparing `MomentumX-2.6.3/tests/test_scenarios.py` & `MomentumX-2.6.4/tests/test_scenarios.py`

 * *Files 2% similar despite different names*

```diff
@@ -740,20 +740,33 @@
         # Verify registration can occur during a write claim
         # and the consumer will grab the oldest buffer first
         b = producer.next_to_send()
         b[0] = b'5'[0]
         consumer_2 = mx.Consumer(_STREAM_NAME)
         consumer_3 = mx.Consumer(_STREAM_NAME)
         c2_str_1st = consumer_2.receive_string(blocking=False)
-        assert not c2_str_1st # Pickup from next available
+        assert c2_str_1st == '3' # Oldest available at time of subscribe
         b.send()
-        c2_str_2nd = consumer_2.receive_string()
-        c3_str_1st = consumer_3.receive_string()
-        assert c2_str_2nd == '5'
-        assert c3_str_1st == '5' # Last sent buffer value
+        c2_str_2nd = consumer_2.receive_string(blocking=False)
+        c2_str_3rd = consumer_2.receive_string(blocking=False)
+        c2_str_4th = consumer_2.receive_string(blocking=False)
+        c3_str_1st = consumer_3.receive_string(blocking=False)
+        c3_str_2nd = consumer_3.receive_string(blocking=False)
+        c3_str_3rd = consumer_3.receive_string(blocking=False)
+        c3_str_4th = consumer_3.receive_string(blocking=False)
+        assert c2_str_2nd == '4'
+        assert c2_str_3rd == '5'
+        assert c3_str_1st == '3' # Oldest available at time of subscribe
+        assert c3_str_2nd == '4'
+        assert c3_str_3rd == '5'
+
+        assert c2_str_4th is None # No more to receive
+        assert c3_str_4th is None # No more to receive
+
+
 
 def test_register_during_sync_write_claim()->None:
     import momentumx as mx
     with timeout_event() as event:
         producer = mx.Producer(_STREAM_NAME, 20, 2, True, event)
         consumer_1 = mx.Consumer(_STREAM_NAME)
         consumer_2 = mx.Consumer(_STREAM_NAME)
```

