# Comparing `tmp/pandacolumns-0.2.7.tar.gz` & `tmp/pandacolumns-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandacolumns-0.2.7.tar", last modified: Wed Apr 12 14:33:25 2023, max compression
+gzip compressed data, was "pandacolumns-0.2.8.tar", last modified: Wed Apr 12 14:37:54 2023, max compression
```

## Comparing `pandacolumns-0.2.7.tar` & `pandacolumns-0.2.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 14:33:25.048358 pandacolumns-0.2.7/
--rw-rw-rw-   0        0        0      171 2023-04-12 14:33:25.048358 pandacolumns-0.2.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-12 14:33:25.035708 pandacolumns-0.2.7/pandacolumns/
--rw-rw-rw-   0        0        0        0 2023-04-10 21:47:47.000000 pandacolumns-0.2.7/pandacolumns/__init__.py
--rw-rw-rw-   0        0        0     1409 2023-04-12 14:33:04.000000 pandacolumns-0.2.7/pandacolumns/dynamic.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:33:25.047308 pandacolumns-0.2.7/pandacolumns.egg-info/
--rw-rw-rw-   0        0        0      171 2023-04-12 14:33:24.000000 pandacolumns-0.2.7/pandacolumns.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-04-12 14:33:24.000000 pandacolumns-0.2.7/pandacolumns.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 14:33:24.000000 pandacolumns-0.2.7/pandacolumns.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-04-12 14:33:24.000000 pandacolumns-0.2.7/pandacolumns.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-12 14:33:24.000000 pandacolumns-0.2.7/pandacolumns.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-12 14:33:25.048358 pandacolumns-0.2.7/setup.cfg
--rw-rw-rw-   0        0        0      333 2023-04-12 14:33:19.000000 pandacolumns-0.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:37:54.758637 pandacolumns-0.2.8/
+-rw-rw-rw-   0        0        0      171 2023-04-12 14:37:54.757633 pandacolumns-0.2.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-12 14:37:54.747619 pandacolumns-0.2.8/pandacolumns/
+-rw-rw-rw-   0        0        0        0 2023-04-10 21:47:47.000000 pandacolumns-0.2.8/pandacolumns/__init__.py
+-rw-rw-rw-   0        0        0     1414 2023-04-12 14:37:38.000000 pandacolumns-0.2.8/pandacolumns/dynamic.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:37:54.757633 pandacolumns-0.2.8/pandacolumns.egg-info/
+-rw-rw-rw-   0        0        0      171 2023-04-12 14:37:54.000000 pandacolumns-0.2.8/pandacolumns.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-04-12 14:37:54.000000 pandacolumns-0.2.8/pandacolumns.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 14:37:54.000000 pandacolumns-0.2.8/pandacolumns.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-04-12 14:37:54.000000 pandacolumns-0.2.8/pandacolumns.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-12 14:37:54.000000 pandacolumns-0.2.8/pandacolumns.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 14:37:54.758637 pandacolumns-0.2.8/setup.cfg
+-rw-rw-rw-   0        0        0      333 2023-04-12 14:37:48.000000 pandacolumns-0.2.8/setup.py
```

### Comparing `pandacolumns-0.2.7/pandacolumns/dynamic.py` & `pandacolumns-0.2.8/pandacolumns/dynamic.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
       description='Drop selected',
       disabled=False,
       button_style='', 
       tooltip='Submit',
       icon='')
 
   def on_submit_button_click_drop(b):
-	ipdb.set_trace()
+      ipdb.set_trace()
       selected_columns = [checkbox.description for checkbox in checkboxes if checkbox.value]
       nonlocal df
       df = df.drop(selected_columns,axis = 1)
       output_label.value = f"{len(selected_columns)} columns dropped"
 
   submit_button_drop.on_click(on_submit_button_click_drop)
   checkboxes_box = widgets.VBox(children=checkboxes)
```

