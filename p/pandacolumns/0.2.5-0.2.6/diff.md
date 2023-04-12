# Comparing `tmp/pandacolumns-0.2.5.tar.gz` & `tmp/pandacolumns-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandacolumns-0.2.5.tar", last modified: Wed Apr 12 14:23:19 2023, max compression
+gzip compressed data, was "pandacolumns-0.2.6.tar", last modified: Wed Apr 12 14:26:44 2023, max compression
```

## Comparing `pandacolumns-0.2.5.tar` & `pandacolumns-0.2.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 14:23:19.081064 pandacolumns-0.2.5/
--rw-rw-rw-   0        0        0      171 2023-04-12 14:23:19.081064 pandacolumns-0.2.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-12 14:23:19.069221 pandacolumns-0.2.5/pandacolumns/
--rw-rw-rw-   0        0        0        0 2023-04-10 21:47:47.000000 pandacolumns-0.2.5/pandacolumns/__init__.py
--rw-rw-rw-   0        0        0     1407 2023-04-12 14:22:22.000000 pandacolumns-0.2.5/pandacolumns/dynamic.py
-drwxrwxrwx   0        0        0        0 2023-04-12 14:23:19.080053 pandacolumns-0.2.5/pandacolumns.egg-info/
--rw-rw-rw-   0        0        0      171 2023-04-12 14:23:18.000000 pandacolumns-0.2.5/pandacolumns.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-04-12 14:23:18.000000 pandacolumns-0.2.5/pandacolumns.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 14:23:18.000000 pandacolumns-0.2.5/pandacolumns.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-04-12 14:23:18.000000 pandacolumns-0.2.5/pandacolumns.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-12 14:23:18.000000 pandacolumns-0.2.5/pandacolumns.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-12 14:23:19.081064 pandacolumns-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0      333 2023-04-12 14:22:48.000000 pandacolumns-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:26:44.787544 pandacolumns-0.2.6/
+-rw-rw-rw-   0        0        0      171 2023-04-12 14:26:44.786445 pandacolumns-0.2.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-12 14:26:44.775727 pandacolumns-0.2.6/pandacolumns/
+-rw-rw-rw-   0        0        0        0 2023-04-10 21:47:47.000000 pandacolumns-0.2.6/pandacolumns/__init__.py
+-rw-rw-rw-   0        0        0     1390 2023-04-12 14:26:26.000000 pandacolumns-0.2.6/pandacolumns/dynamic.py
+drwxrwxrwx   0        0        0        0 2023-04-12 14:26:44.785303 pandacolumns-0.2.6/pandacolumns.egg-info/
+-rw-rw-rw-   0        0        0      171 2023-04-12 14:26:44.000000 pandacolumns-0.2.6/pandacolumns.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-04-12 14:26:44.000000 pandacolumns-0.2.6/pandacolumns.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 14:26:44.000000 pandacolumns-0.2.6/pandacolumns.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-04-12 14:26:44.000000 pandacolumns-0.2.6/pandacolumns.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-12 14:26:44.000000 pandacolumns-0.2.6/pandacolumns.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 14:26:44.787544 pandacolumns-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      333 2023-04-12 14:26:39.000000 pandacolumns-0.2.6/setup.py
```

### Comparing `pandacolumns-0.2.5/pandacolumns/dynamic.py` & `pandacolumns-0.2.6/pandacolumns/dynamic.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,14 @@
       icon='')
 
   def on_submit_button_click_drop(b):
       selected_columns = [checkbox.description for checkbox in checkboxes if checkbox.value]
       nonlocal df
       df = df.drop(selected_columns,axis = 1)
       output_label.value = f"{len(selected_columns)} columns dropped"
-      return df
 
   submit_button_drop.on_click(on_submit_button_click_drop)
   checkboxes_box = widgets.VBox(children=checkboxes)
   output_label = widgets.Label(value="")
   submit_box = widgets.VBox(children=[widgets.Label(value=''),submit_button_drop,output_label])
   submit_box.layout.margin = '30px 0px 0px 20px'
   full_box = widgets.HBox(children=[checkboxes_box, submit_box])
```

