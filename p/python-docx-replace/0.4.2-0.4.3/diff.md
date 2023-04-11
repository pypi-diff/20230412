# Comparing `tmp/python-docx-replace-0.4.2.tar.gz` & `tmp/python-docx-replace-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-docx-replace-0.4.2.tar", last modified: Sun Jan 29 00:07:59 2023, max compression
+gzip compressed data, was "python-docx-replace-0.4.3.tar", last modified: Tue Apr 11 23:02:21 2023, max compression
```

## Comparing `python-docx-replace-0.4.2.tar` & `python-docx-replace-0.4.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 ivanbicalho   (501) staff       (20)        0 2023-01-29 00:07:59.333602 python-docx-replace-0.4.2/
--rw-r--r--   0 ivanbicalho   (501) staff       (20)     1069 2022-10-31 14:53:42.000000 python-docx-replace-0.4.2/LICENSE
--rw-r--r--   0 ivanbicalho   (501) staff       (20)     7236 2023-01-29 00:07:59.333741 python-docx-replace-0.4.2/PKG-INFO
--rw-r--r--   0 ivanbicalho   (501) staff       (20)     6758 2022-10-31 14:53:42.000000 python-docx-replace-0.4.2/README.md
--rw-r--r--   0 ivanbicalho   (501) staff       (20)       84 2022-10-31 14:53:42.000000 python-docx-replace-0.4.2/pyproject.toml
--rw-r--r--   0 ivanbicalho   (501) staff       (20)      662 2023-01-29 00:07:59.334204 python-docx-replace-0.4.2/setup.cfg
-drwxr-xr-x   0 ivanbicalho   (501) staff       (20)        0 2023-01-29 00:07:59.330717 python-docx-replace-0.4.2/src/
-drwxr-xr-x   0 ivanbicalho   (501) staff       (20)        0 2023-01-29 00:07:59.332788 python-docx-replace-0.4.2/src/python_docx_replace/
--rw-r--r--   0 ivanbicalho   (501) staff       (20)     6212 2023-01-28 23:51:05.000000 python-docx-replace-0.4.2/src/python_docx_replace/__init__.py
--rw-r--r--   0 ivanbicalho   (501) staff       (20)     3676 2022-10-31 14:53:42.000000 python-docx-replace-0.4.2/src/python_docx_replace/block_handler.py
--rw-r--r--   0 ivanbicalho   (501) staff       (20)     1161 2022-10-31 14:53:42.000000 python-docx-replace-0.4.2/src/python_docx_replace/exceptions.py
--rw-r--r--   0 ivanbicalho   (501) staff       (20)     1571 2022-10-31 14:53:42.000000 python-docx-replace-0.4.2/src/python_docx_replace/key_changer.py
--rw-r--r--   0 ivanbicalho   (501) staff       (20)     2638 2023-01-29 00:07:48.000000 python-docx-replace-0.4.2/src/python_docx_replace/paragraph.py
-drwxr-xr-x   0 ivanbicalho   (501) staff       (20)        0 2023-01-29 00:07:59.333475 python-docx-replace-0.4.2/src/python_docx_replace.egg-info/
--rw-r--r--   0 ivanbicalho   (501) staff       (20)     7236 2023-01-29 00:07:59.000000 python-docx-replace-0.4.2/src/python_docx_replace.egg-info/PKG-INFO
--rw-r--r--   0 ivanbicalho   (501) staff       (20)      467 2023-01-29 00:07:59.000000 python-docx-replace-0.4.2/src/python_docx_replace.egg-info/SOURCES.txt
--rw-r--r--   0 ivanbicalho   (501) staff       (20)        1 2023-01-29 00:07:59.000000 python-docx-replace-0.4.2/src/python_docx_replace.egg-info/dependency_links.txt
--rw-r--r--   0 ivanbicalho   (501) staff       (20)       12 2023-01-29 00:07:59.000000 python-docx-replace-0.4.2/src/python_docx_replace.egg-info/requires.txt
--rw-r--r--   0 ivanbicalho   (501) staff       (20)       20 2023-01-29 00:07:59.000000 python-docx-replace-0.4.2/src/python_docx_replace.egg-info/top_level.txt
+drwxr-xr-x   0 ivanbicalho   (501) staff       (20)        0 2023-04-11 23:02:21.055059 python-docx-replace-0.4.3/
+-rw-r--r--   0 ivanbicalho   (501) staff       (20)     1069 2022-10-31 14:53:42.000000 python-docx-replace-0.4.3/LICENSE
+-rw-r--r--   0 ivanbicalho   (501) staff       (20)     7236 2023-04-11 23:02:21.055149 python-docx-replace-0.4.3/PKG-INFO
+-rw-r--r--   0 ivanbicalho   (501) staff       (20)     6758 2022-10-31 14:53:42.000000 python-docx-replace-0.4.3/README.md
+-rw-r--r--   0 ivanbicalho   (501) staff       (20)       84 2022-10-31 14:53:42.000000 python-docx-replace-0.4.3/pyproject.toml
+-rw-r--r--   0 ivanbicalho   (501) staff       (20)      662 2023-04-11 23:02:21.055445 python-docx-replace-0.4.3/setup.cfg
+drwxr-xr-x   0 ivanbicalho   (501) staff       (20)        0 2023-04-11 23:02:21.052098 python-docx-replace-0.4.3/src/
+drwxr-xr-x   0 ivanbicalho   (501) staff       (20)        0 2023-04-11 23:02:21.053816 python-docx-replace-0.4.3/src/python_docx_replace/
+-rw-r--r--   0 ivanbicalho   (501) staff       (20)     6623 2023-04-11 23:00:27.000000 python-docx-replace-0.4.3/src/python_docx_replace/__init__.py
+-rw-r--r--   0 ivanbicalho   (501) staff       (20)     3676 2022-10-31 14:53:42.000000 python-docx-replace-0.4.3/src/python_docx_replace/block_handler.py
+-rw-r--r--   0 ivanbicalho   (501) staff       (20)     1161 2022-10-31 14:53:42.000000 python-docx-replace-0.4.3/src/python_docx_replace/exceptions.py
+-rw-r--r--   0 ivanbicalho   (501) staff       (20)     1571 2022-10-31 14:53:42.000000 python-docx-replace-0.4.3/src/python_docx_replace/key_changer.py
+-rw-r--r--   0 ivanbicalho   (501) staff       (20)     2638 2023-04-11 22:45:44.000000 python-docx-replace-0.4.3/src/python_docx_replace/paragraph.py
+drwxr-xr-x   0 ivanbicalho   (501) staff       (20)        0 2023-04-11 23:02:21.054920 python-docx-replace-0.4.3/src/python_docx_replace.egg-info/
+-rw-r--r--   0 ivanbicalho   (501) staff       (20)     7236 2023-04-11 23:02:21.000000 python-docx-replace-0.4.3/src/python_docx_replace.egg-info/PKG-INFO
+-rw-r--r--   0 ivanbicalho   (501) staff       (20)      467 2023-04-11 23:02:21.000000 python-docx-replace-0.4.3/src/python_docx_replace.egg-info/SOURCES.txt
+-rw-r--r--   0 ivanbicalho   (501) staff       (20)        1 2023-04-11 23:02:21.000000 python-docx-replace-0.4.3/src/python_docx_replace.egg-info/dependency_links.txt
+-rw-r--r--   0 ivanbicalho   (501) staff       (20)       12 2023-04-11 23:02:21.000000 python-docx-replace-0.4.3/src/python_docx_replace.egg-info/requires.txt
+-rw-r--r--   0 ivanbicalho   (501) staff       (20)       20 2023-04-11 23:02:21.000000 python-docx-replace-0.4.3/src/python_docx_replace.egg-info/top_level.txt
```

### Comparing `python-docx-replace-0.4.2/LICENSE` & `python-docx-replace-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python-docx-replace-0.4.2/PKG-INFO` & `python-docx-replace-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-docx-replace
-Version: 0.4.2
+Version: 0.4.3
 Summary: Replace words and remove blocks inside a Word document without losing format
 Home-page: https://github.com/ivanbicalho/python-docx-replace
 Author: Ivan Bicalho
 Author-email: ivanribeirob@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `python-docx-replace-0.4.2/README.md` & `python-docx-replace-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `python-docx-replace-0.4.2/setup.cfg` & `python-docx-replace-0.4.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = python-docx-replace
-version = 0.4.2
+version = 0.4.3
 author = Ivan Bicalho
 author_email = ivanribeirob@gmail.com
 description = Replace words and remove blocks inside a Word document without losing format
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ivanbicalho/python-docx-replace
 classifiers =
```

### Comparing `python-docx-replace-0.4.2/src/python_docx_replace/__init__.py` & `python-docx-replace-0.4.3/src/python_docx_replace/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -100,30 +100,37 @@
                 if paragraph.contains(end):
                     # if the initial and end tag are in the same paragraph, treat them together
                     paragraph.replace_block(initial, end, keep_block)
                     return True  # block completed, returns
                 else:
                     # the current paragraph doesn't have the end tag
                     if paragraph.startswith(initial):
-                        # if the paragraph starts with the initial tag, we can delete the entire paragraph,
-                        # because the end tag is not here
-                        paragraph.delete()
+                        # if the paragraph starts with the initial tag, we can clear the tag if is to keep_block
+                        # otherwise we can delete the entire paragraph because the end tag is not here
+                        if keep_block:
+                            paragraph.clear_tag_and_before(initial, keep_block)
+                        else:
+                            paragraph.delete()
                         continue
                     else:
                         # if the paragraph doesn't start with the initial tag, we cannot delete the entire
                         # paragraph, we have to clear the tag and remove the content right after (if not keep_block)
                         paragraph.clear_tag_and_after(initial, keep_block)
                         continue
         else:
             # we are looking for the end tag as the initial tag was found and treated before
             if paragraph.contains(end):
                 # end tag found in this paragraph
                 if paragraph.endswith(end):
-                    # if the paragraph ends with the end tag, we can delete the entire paragraph
-                    paragraph.delete()
+                    # if the paragraph ends with the end tag we can clear the tag if is to keep_block
+                    # otherwise we can delete the entire paragraph
+                    if keep_block:
+                        paragraph.clear_tag_and_after(end, keep_block)
+                    else:
+                        paragraph.delete()
                     return True  # block completed, returns
                 else:
                     # if the paragraph doesn't end with the end tag, we cannot delete the entire
                     # paragraph, we have to clear the tag and remove the content right before (if not keep_block)
                     paragraph.clear_tag_and_before(end, keep_block)
                     return True  # block completed, returns
             else:
```

### Comparing `python-docx-replace-0.4.2/src/python_docx_replace/block_handler.py` & `python-docx-replace-0.4.3/src/python_docx_replace/block_handler.py`

 * *Files identical despite different names*

### Comparing `python-docx-replace-0.4.2/src/python_docx_replace/exceptions.py` & `python-docx-replace-0.4.3/src/python_docx_replace/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-docx-replace-0.4.2/src/python_docx_replace/key_changer.py` & `python-docx-replace-0.4.3/src/python_docx_replace/key_changer.py`

 * *Files identical despite different names*

### Comparing `python-docx-replace-0.4.2/src/python_docx_replace/paragraph.py` & `python-docx-replace-0.4.3/src/python_docx_replace/paragraph.py`

 * *Files identical despite different names*

### Comparing `python-docx-replace-0.4.2/src/python_docx_replace.egg-info/PKG-INFO` & `python-docx-replace-0.4.3/src/python_docx_replace.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-docx-replace
-Version: 0.4.2
+Version: 0.4.3
 Summary: Replace words and remove blocks inside a Word document without losing format
 Home-page: https://github.com/ivanbicalho/python-docx-replace
 Author: Ivan Bicalho
 Author-email: ivanribeirob@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

