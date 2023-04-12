# Comparing `tmp/plantuml_markdown-3.8.2-py3-none-any.whl.zip` & `tmp/plantuml_markdown-3.8.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 16759 bytes, number of entries: 6
--rw-rw-r--  2.0 unx    29398 b- defN 23-Mar-06 17:02 plantuml_markdown.py
--rw-rw-r--  2.0 unx     1299 b- defN 23-Mar-06 17:04 plantuml_markdown-3.8.2.dist-info/LICENSE
--rw-rw-r--  2.0 unx    16363 b- defN 23-Mar-06 17:04 plantuml_markdown-3.8.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Mar-06 17:04 plantuml_markdown-3.8.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx       18 b- defN 23-Mar-06 17:04 plantuml_markdown-3.8.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      515 b- defN 23-Mar-06 17:04 plantuml_markdown-3.8.2.dist-info/RECORD
-6 files, 47685 bytes uncompressed, 15823 bytes compressed:  66.8%
+Zip file size: 16756 bytes, number of entries: 6
+-rw-rw-r--  2.0 unx    29396 b- defN 23-Apr-12 16:52 plantuml_markdown.py
+-rw-rw-r--  2.0 unx     1299 b- defN 23-Apr-12 16:57 plantuml_markdown-3.8.3.dist-info/LICENSE
+-rw-rw-r--  2.0 unx    16363 b- defN 23-Apr-12 16:57 plantuml_markdown-3.8.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-12 16:57 plantuml_markdown-3.8.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       18 b- defN 23-Apr-12 16:57 plantuml_markdown-3.8.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      515 b- defN 23-Apr-12 16:57 plantuml_markdown-3.8.3.dist-info/RECORD
+6 files, 47683 bytes uncompressed, 15820 bytes compressed:  66.8%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: plantuml_markdown.py
 Comment: 
 
-Filename: plantuml_markdown-3.8.2.dist-info/LICENSE
+Filename: plantuml_markdown-3.8.3.dist-info/LICENSE
 Comment: 
 
-Filename: plantuml_markdown-3.8.2.dist-info/METADATA
+Filename: plantuml_markdown-3.8.3.dist-info/METADATA
 Comment: 
 
-Filename: plantuml_markdown-3.8.2.dist-info/WHEEL
+Filename: plantuml_markdown-3.8.3.dist-info/WHEEL
 Comment: 
 
-Filename: plantuml_markdown-3.8.2.dist-info/top_level.txt
+Filename: plantuml_markdown-3.8.3.dist-info/top_level.txt
 Comment: 
 
-Filename: plantuml_markdown-3.8.2.dist-info/RECORD
+Filename: plantuml_markdown-3.8.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## plantuml_markdown.py

```diff
@@ -604,15 +604,15 @@
             'title': ["", "Tooltip for the diagram"],
             'server': ["", "PlantUML server url, for remote rendering. Defaults to '', use local command."],
             'kroki_server': ["", "Kroki server url, as alternative to 'server' for remote rendering (image maps must "
                                  "be disabled manually). Defaults to '', use PlantUML server if defined"],
             'server_include_whitelist': [[r'^[Cc]4.*$'],
                                          "List of regular expressions defining which include files are supported by "
                                          "the server. Defaults to [r'^c4.*$']"],
-            'insecure': ["False", "Disable SSL certificates verification; set to True if you server uses self-signed certificates. Defaults to False"],
+            'insecure': [False, "Disable SSL certificates verification; set to True if you server uses self-signed certificates. Defaults to False"],
             'cachedir': ["", "Directory for caching of diagrams. Defaults to '', no caching"],
             'image_maps': ["true", "Enable generation of PNG image maps, allowing to use hyperlinks with PNG images."
                                    "Defaults to true"],
             'priority': ["30", "Extension priority. Higher values means the extension is applied sooner than others. "
                                "Defaults to 30"],
             'base_dir': [".", "Base directory for external files inclusion"],
             'encoding': ["utf8", "Default character encoding for external files (default: utf8)"],
```

## Comparing `plantuml_markdown-3.8.2.dist-info/LICENSE` & `plantuml_markdown-3.8.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `plantuml_markdown-3.8.2.dist-info/METADATA` & `plantuml_markdown-3.8.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plantuml-markdown
-Version: 3.8.2
+Version: 3.8.3
 Summary: A PlantUML plugin for Markdown
 Home-page: https://github.com/mikitex70/plantuml-markdown
 Author: Michele Tessaro
 Author-email: michele.tessaro@email.it
 Keywords: Markdown,typesetting,include,plugin,extension
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
```

## Comparing `plantuml_markdown-3.8.2.dist-info/RECORD` & `plantuml_markdown-3.8.3.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,6 +1,6 @@
-plantuml_markdown.py,sha256=DljJuNvvZ9caa407_SASozb8yArDaPjYQfVZL9NddTY,29398
-plantuml_markdown-3.8.2.dist-info/LICENSE,sha256=bsJBUgOT3HznIWIHgzMSbwk7xWI0i0bptHJyUgU6Qsg,1299
-plantuml_markdown-3.8.2.dist-info/METADATA,sha256=5rffdzy_jJfpKLWeCDizHdxZI8bT-gDviTAOREDRr-g,16363
-plantuml_markdown-3.8.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-plantuml_markdown-3.8.2.dist-info/top_level.txt,sha256=-nFvHZOilZwd9Usv166IF3L2OGkr5IT7uTpQEjw2I5M,18
-plantuml_markdown-3.8.2.dist-info/RECORD,,
+plantuml_markdown.py,sha256=N39CgzmQh2LHyPu3JJdG2Si2bDBznUZY-lSOVUd9DUM,29396
+plantuml_markdown-3.8.3.dist-info/LICENSE,sha256=bsJBUgOT3HznIWIHgzMSbwk7xWI0i0bptHJyUgU6Qsg,1299
+plantuml_markdown-3.8.3.dist-info/METADATA,sha256=LOeysIs76mNGJDzJ298P_W6CISxxdw9Vik0sO9158Ik,16363
+plantuml_markdown-3.8.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+plantuml_markdown-3.8.3.dist-info/top_level.txt,sha256=-nFvHZOilZwd9Usv166IF3L2OGkr5IT7uTpQEjw2I5M,18
+plantuml_markdown-3.8.3.dist-info/RECORD,,
```

