# Comparing `tmp/calcure-2.8.5.tar.gz` & `tmp/calcure-2.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calcure-2.8.5.tar", last modified: Wed Apr  5 00:51:46 2023, max compression
+gzip compressed data, was "calcure-2.8.6.tar", last modified: Wed Apr 12 05:06:50 2023, max compression
```

## Comparing `calcure-2.8.5.tar` & `calcure-2.8.6.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-04-05 00:51:46.956391 calcure-2.8.5/
--rw-r--r--   0 r         (1000) r         (1000)     1071 2023-03-01 08:49:55.000000 calcure-2.8.5/LICENSE
--rw-r--r--   0 r         (1000) r         (1000)     3908 2023-04-05 00:51:46.956391 calcure-2.8.5/PKG-INFO
--rw-r--r--   0 r         (1000) r         (1000)     3145 2023-03-02 07:55:45.000000 calcure-2.8.5/README.md
-drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-04-05 00:51:46.953058 calcure-2.8.5/calcure/
--rw-r--r--   0 r         (1000) r         (1000)    42169 2023-04-05 00:49:12.000000 calcure-2.8.5/calcure/__main__.py
--rw-r--r--   0 r         (1000) r         (1000)     2551 2023-03-02 07:54:07.000000 calcure-2.8.5/calcure/calendars.py
--rw-r--r--   0 r         (1000) r         (1000)     4162 2023-03-04 12:39:25.000000 calcure-2.8.5/calcure/colors.py
--rw-r--r--   0 r         (1000) r         (1000)    20292 2023-03-14 13:20:07.000000 calcure-2.8.5/calcure/configuration.py
--rw-r--r--   0 r         (1000) r         (1000)    22876 2023-04-05 00:48:09.000000 calcure-2.8.5/calcure/controls.py
--rw-r--r--   0 r         (1000) r         (1000)    12945 2023-03-01 12:10:25.000000 calcure-2.8.5/calcure/data.py
--rw-r--r--   0 r         (1000) r         (1000)     3564 2023-03-14 09:29:08.000000 calcure-2.8.5/calcure/dialogues.py
--rw-r--r--   0 r         (1000) r         (1000)     1071 2023-04-05 00:48:10.000000 calcure-2.8.5/calcure/errors.py
--rw-r--r--   0 r         (1000) r         (1000)     3687 2023-03-01 08:49:55.000000 calcure-2.8.5/calcure/importers.py
--rw-r--r--   0 r         (1000) r         (1000)    14438 2023-03-14 04:33:36.000000 calcure-2.8.5/calcure/loaders.py
--rw-r--r--   0 r         (1000) r         (1000)     2550 2023-03-01 08:49:55.000000 calcure-2.8.5/calcure/savers.py
--rw-r--r--   0 r         (1000) r         (1000)     4534 2023-04-05 00:48:09.000000 calcure-2.8.5/calcure/screen.py
--rw-r--r--   0 r         (1000) r         (1000)      836 2023-03-01 08:49:55.000000 calcure-2.8.5/calcure/test_async.py
--rw-r--r--   0 r         (1000) r         (1000)      463 2023-03-14 13:14:44.000000 calcure-2.8.5/calcure/test_decoration.py
-drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-04-05 00:51:46.956391 calcure-2.8.5/calcure/translations/
--rw-r--r--   0 r         (1000) r         (1000)     5562 2023-03-10 03:04:29.000000 calcure-2.8.5/calcure/translations/br.py
--rw-r--r--   0 r         (1000) r         (1000)     5026 2023-03-10 03:05:54.000000 calcure-2.8.5/calcure/translations/en.py
--rw-r--r--   0 r         (1000) r         (1000)     6015 2023-03-10 03:05:59.000000 calcure-2.8.5/calcure/translations/fr.py
--rw-r--r--   0 r         (1000) r         (1000)     6036 2023-03-10 03:04:49.000000 calcure-2.8.5/calcure/translations/it.py
--rw-r--r--   0 r         (1000) r         (1000)     7908 2023-03-10 03:06:06.000000 calcure-2.8.5/calcure/translations/ru.py
--rw-r--r--   0 r         (1000) r         (1000)     5895 2023-03-10 03:05:11.000000 calcure-2.8.5/calcure/translations/tr.py
--rw-r--r--   0 r         (1000) r         (1000)     5239 2023-03-10 03:05:22.000000 calcure-2.8.5/calcure/translations/zh.py
--rw-r--r--   0 r         (1000) r         (1000)      905 2023-03-01 08:49:55.000000 calcure-2.8.5/calcure/weather.py
-drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-04-05 00:51:46.953058 calcure-2.8.5/calcure.egg-info/
--rw-r--r--   0 r         (1000) r         (1000)     3908 2023-04-05 00:51:46.000000 calcure-2.8.5/calcure.egg-info/PKG-INFO
--rw-r--r--   0 r         (1000) r         (1000)      721 2023-04-05 00:51:46.000000 calcure-2.8.5/calcure.egg-info/SOURCES.txt
--rw-r--r--   0 r         (1000) r         (1000)        1 2023-04-05 00:51:46.000000 calcure-2.8.5/calcure.egg-info/dependency_links.txt
--rw-r--r--   0 r         (1000) r         (1000)       49 2023-04-05 00:51:46.000000 calcure-2.8.5/calcure.egg-info/entry_points.txt
--rw-r--r--   0 r         (1000) r         (1000)       23 2023-04-05 00:51:46.000000 calcure-2.8.5/calcure.egg-info/requires.txt
--rw-r--r--   0 r         (1000) r         (1000)        8 2023-04-05 00:51:46.000000 calcure-2.8.5/calcure.egg-info/top_level.txt
--rw-r--r--   0 r         (1000) r         (1000)       91 2023-03-01 08:49:55.000000 calcure-2.8.5/pyproject.toml
--rw-r--r--   0 r         (1000) r         (1000)       38 2023-04-05 00:51:46.956391 calcure-2.8.5/setup.cfg
--rw-r--r--   0 r         (1000) r         (1000)     1427 2023-03-01 08:49:55.000000 calcure-2.8.5/setup.py
+drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-04-12 05:06:50.951349 calcure-2.8.6/
+-rw-r--r--   0 r         (1000) r         (1000)     1071 2023-03-01 08:49:55.000000 calcure-2.8.6/LICENSE
+-rw-r--r--   0 r         (1000) r         (1000)     3908 2023-04-12 05:06:50.951349 calcure-2.8.6/PKG-INFO
+-rw-r--r--   0 r         (1000) r         (1000)     3145 2023-03-02 07:55:45.000000 calcure-2.8.6/README.md
+drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-04-12 05:06:50.951349 calcure-2.8.6/calcure/
+-rw-r--r--   0 r         (1000) r         (1000)    42325 2023-04-12 05:05:40.000000 calcure-2.8.6/calcure/__main__.py
+-rw-r--r--   0 r         (1000) r         (1000)     2551 2023-03-02 07:54:07.000000 calcure-2.8.6/calcure/calendars.py
+-rw-r--r--   0 r         (1000) r         (1000)     4162 2023-03-04 12:39:25.000000 calcure-2.8.6/calcure/colors.py
+-rw-r--r--   0 r         (1000) r         (1000)    20292 2023-04-12 05:05:37.000000 calcure-2.8.6/calcure/configuration.py
+-rw-r--r--   0 r         (1000) r         (1000)    22876 2023-04-12 05:05:26.000000 calcure-2.8.6/calcure/controls.py
+-rw-r--r--   0 r         (1000) r         (1000)    12945 2023-03-01 12:10:25.000000 calcure-2.8.6/calcure/data.py
+-rw-r--r--   0 r         (1000) r         (1000)     3564 2023-03-14 09:29:08.000000 calcure-2.8.6/calcure/dialogues.py
+-rw-r--r--   0 r         (1000) r         (1000)     1071 2023-04-05 00:48:10.000000 calcure-2.8.6/calcure/errors.py
+-rw-r--r--   0 r         (1000) r         (1000)     3687 2023-03-01 08:49:55.000000 calcure-2.8.6/calcure/importers.py
+-rw-r--r--   0 r         (1000) r         (1000)    14438 2023-03-14 04:33:36.000000 calcure-2.8.6/calcure/loaders.py
+-rw-r--r--   0 r         (1000) r         (1000)     2550 2023-03-01 08:49:55.000000 calcure-2.8.6/calcure/savers.py
+-rw-r--r--   0 r         (1000) r         (1000)     4534 2023-04-05 00:48:09.000000 calcure-2.8.6/calcure/screen.py
+-rw-r--r--   0 r         (1000) r         (1000)      836 2023-03-01 08:49:55.000000 calcure-2.8.6/calcure/test_async.py
+-rw-r--r--   0 r         (1000) r         (1000)      463 2023-03-14 13:14:44.000000 calcure-2.8.6/calcure/test_decoration.py
+drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-04-12 05:06:50.951349 calcure-2.8.6/calcure/translations/
+-rw-r--r--   0 r         (1000) r         (1000)     5562 2023-03-10 03:04:29.000000 calcure-2.8.6/calcure/translations/br.py
+-rw-r--r--   0 r         (1000) r         (1000)     5026 2023-03-10 03:05:54.000000 calcure-2.8.6/calcure/translations/en.py
+-rw-r--r--   0 r         (1000) r         (1000)     6015 2023-03-10 03:05:59.000000 calcure-2.8.6/calcure/translations/fr.py
+-rw-r--r--   0 r         (1000) r         (1000)     6036 2023-03-10 03:04:49.000000 calcure-2.8.6/calcure/translations/it.py
+-rw-r--r--   0 r         (1000) r         (1000)     7908 2023-03-10 03:06:06.000000 calcure-2.8.6/calcure/translations/ru.py
+-rw-r--r--   0 r         (1000) r         (1000)     5895 2023-03-10 03:05:11.000000 calcure-2.8.6/calcure/translations/tr.py
+-rw-r--r--   0 r         (1000) r         (1000)     5239 2023-03-10 03:05:22.000000 calcure-2.8.6/calcure/translations/zh.py
+-rw-r--r--   0 r         (1000) r         (1000)      905 2023-03-01 08:49:55.000000 calcure-2.8.6/calcure/weather.py
+drwxr-xr-x   0 r         (1000) r         (1000)        0 2023-04-12 05:06:50.951349 calcure-2.8.6/calcure.egg-info/
+-rw-r--r--   0 r         (1000) r         (1000)     3908 2023-04-12 05:06:50.000000 calcure-2.8.6/calcure.egg-info/PKG-INFO
+-rw-r--r--   0 r         (1000) r         (1000)      721 2023-04-12 05:06:50.000000 calcure-2.8.6/calcure.egg-info/SOURCES.txt
+-rw-r--r--   0 r         (1000) r         (1000)        1 2023-04-12 05:06:50.000000 calcure-2.8.6/calcure.egg-info/dependency_links.txt
+-rw-r--r--   0 r         (1000) r         (1000)       49 2023-04-12 05:06:50.000000 calcure-2.8.6/calcure.egg-info/entry_points.txt
+-rw-r--r--   0 r         (1000) r         (1000)       23 2023-04-12 05:06:50.000000 calcure-2.8.6/calcure.egg-info/requires.txt
+-rw-r--r--   0 r         (1000) r         (1000)        8 2023-04-12 05:06:50.000000 calcure-2.8.6/calcure.egg-info/top_level.txt
+-rw-r--r--   0 r         (1000) r         (1000)       91 2023-03-01 08:49:55.000000 calcure-2.8.6/pyproject.toml
+-rw-r--r--   0 r         (1000) r         (1000)       38 2023-04-12 05:06:50.951349 calcure-2.8.6/setup.cfg
+-rw-r--r--   0 r         (1000) r         (1000)     1427 2023-03-01 08:49:55.000000 calcure-2.8.6/setup.py
```

### Comparing `calcure-2.8.5/LICENSE` & `calcure-2.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `calcure-2.8.5/PKG-INFO` & `calcure-2.8.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calcure
-Version: 2.8.5
+Version: 2.8.6
 Summary: Modern TUI calendar and task manager
 Home-page: https://github.com/anufrievroman/calcure
 Author: Roman Anufriev
 Author-email: anufriev.roman@protonmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `calcure-2.8.5/README.md` & `calcure-2.8.6/README.md`

 * *Files identical despite different names*

### Comparing `calcure-2.8.5/calcure/__main__.py` & `calcure-2.8.6/calcure/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     from calcure.translations.tr import *
 elif cf.LANG == "zh":
     from calcure.translations.zh import *
 else:
     from calcure.translations.en import *
 
 
-__version__ = "2.8.5"
+__version__ = "2.8.6"
 
 
 def read_items_from_user_arguments(screen, user_tasks, user_events, task_saver_csv, event_saver_csv):
     """Read --task and --event flags from user arguments to create new tasks or events"""
     try:
         opts, _ = getopt.getopt(sys.argv[1:], "pjhvi", ["folder=", "config=", "task=", "event="])
         for opt, arg in opts:
@@ -94,22 +94,25 @@
         number_of_characters = len(real_text)
         available_space = x_max - x
         number_of_special = text.count('\u0336')
         if number_of_characters > available_space:
             coefficient = 2 if number_of_special > 0 else 1
             text = f"{text[:(available_space - 1)*coefficient]}"
 
-        if bold and underlined:
-            self.stdscr.addstr(y, x, text, curses.color_pair(color.value) | curses.A_BOLD | curses.A_UNDERLINE)
-        elif bold and not underlined:
-            self.stdscr.addstr(y, x, text, curses.color_pair(color.value) | curses.A_BOLD)
-        elif underlined and not bold:
-            self.stdscr.addstr(y, x, text, curses.color_pair(color.value) | curses.A_UNDERLINE)
-        else:
-            self.stdscr.addstr(y, x, text, curses.color_pair(color.value))
+        try:
+            if bold and underlined:
+                self.stdscr.addstr(y, x, text, curses.color_pair(color.value) | curses.A_BOLD | curses.A_UNDERLINE)
+            elif bold and not underlined:
+                self.stdscr.addstr(y, x, text, curses.color_pair(color.value) | curses.A_BOLD)
+            elif underlined and not bold:
+                self.stdscr.addstr(y, x, text, curses.color_pair(color.value) | curses.A_UNDERLINE)
+            else:
+                self.stdscr.addstr(y, x, text, curses.color_pair(color.value))
+        except curses.error: # Fix for occasional error with large zoom (reason is unclear)
+            return
 
 
 class TaskView(View):
     """Display a single task"""
 
     def __init__(self, stdscr, y, x, task, screen):
         super().__init__(stdscr, y, x)
```

### Comparing `calcure-2.8.5/calcure/calendars.py` & `calcure-2.8.6/calcure/calendars.py`

 * *Files identical despite different names*

### Comparing `calcure-2.8.5/calcure/colors.py` & `calcure-2.8.6/calcure/colors.py`

 * *Files identical despite different names*

### Comparing `calcure-2.8.5/calcure/configuration.py` & `calcure-2.8.6/calcure/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -332,15 +332,15 @@
                     self.DEFAULT_VIEW = AppState.JOURNAL
                 elif opt == '-d':
                     self.DEFAULT_VIEW = AppState.JOURNAL
                 elif opt in ('-h'):
                     self.DEFAULT_VIEW = AppState.HELP
                 elif opt in ('-v'):
                     self.DEFAULT_VIEW = AppState.EXIT
-                    print ('Calcure - version 2.8.2')
+                    print ('Calcure - version 2.8.6')
                 elif opt in ('-i'):
                     self.USE_PERSIAN_CALENDAR = True
         except getopt.GetoptError as e_message:
             logging.error("Invalid user arguments. %s", e_message)
             pass
```

### Comparing `calcure-2.8.5/calcure/controls.py` & `calcure-2.8.6/calcure/controls.py`

 * *Files identical despite different names*

### Comparing `calcure-2.8.5/calcure/data.py` & `calcure-2.8.6/calcure/data.py`

 * *Files identical despite different names*

### Comparing `calcure-2.8.5/calcure/dialogues.py` & `calcure-2.8.6/calcure/dialogues.py`

 * *Files identical despite different names*

### Comparing `calcure-2.8.5/calcure/errors.py` & `calcure-2.8.6/calcure/errors.py`

 * *Files identical despite different names*

### Comparing `calcure-2.8.5/calcure/importers.py` & `calcure-2.8.6/calcure/importers.py`

 * *Files identical despite different names*

### Comparing `calcure-2.8.5/calcure/loaders.py` & `calcure-2.8.6/calcure/loaders.py`

 * *Files identical despite different names*

### Comparing `calcure-2.8.5/calcure/savers.py` & `calcure-2.8.6/calcure/savers.py`

 * *Files identical despite different names*

### Comparing `calcure-2.8.5/calcure/screen.py` & `calcure-2.8.6/calcure/screen.py`

 * *Files identical despite different names*

### Comparing `calcure-2.8.5/calcure/test_async.py` & `calcure-2.8.6/calcure/test_async.py`

 * *Files identical despite different names*

### Comparing `calcure-2.8.5/calcure/translations/br.py` & `calcure-2.8.6/calcure/translations/br.py`

 * *Files identical despite different names*

### Comparing `calcure-2.8.5/calcure/translations/en.py` & `calcure-2.8.6/calcure/translations/en.py`

 * *Files identical despite different names*

### Comparing `calcure-2.8.5/calcure/translations/fr.py` & `calcure-2.8.6/calcure/translations/fr.py`

 * *Files identical despite different names*

### Comparing `calcure-2.8.5/calcure/translations/it.py` & `calcure-2.8.6/calcure/translations/it.py`

 * *Files identical despite different names*

### Comparing `calcure-2.8.5/calcure/translations/ru.py` & `calcure-2.8.6/calcure/translations/ru.py`

 * *Files identical despite different names*

### Comparing `calcure-2.8.5/calcure/translations/tr.py` & `calcure-2.8.6/calcure/translations/tr.py`

 * *Files identical despite different names*

### Comparing `calcure-2.8.5/calcure/translations/zh.py` & `calcure-2.8.6/calcure/translations/zh.py`

 * *Files identical despite different names*

### Comparing `calcure-2.8.5/calcure/weather.py` & `calcure-2.8.6/calcure/weather.py`

 * *Files identical despite different names*

### Comparing `calcure-2.8.5/calcure.egg-info/PKG-INFO` & `calcure-2.8.6/calcure.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calcure
-Version: 2.8.5
+Version: 2.8.6
 Summary: Modern TUI calendar and task manager
 Home-page: https://github.com/anufrievroman/calcure
 Author: Roman Anufriev
 Author-email: anufriev.roman@protonmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `calcure-2.8.5/calcure.egg-info/SOURCES.txt` & `calcure-2.8.6/calcure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `calcure-2.8.5/setup.py` & `calcure-2.8.6/setup.py`

 * *Files identical despite different names*

