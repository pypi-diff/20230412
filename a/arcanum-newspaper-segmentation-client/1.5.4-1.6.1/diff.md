# Comparing `tmp/arcanum-newspaper-segmentation-client-1.5.4.tar.gz` & `tmp/arcanum-newspaper-segmentation-client-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcanum-newspaper-segmentation-client-1.5.4.tar", last modified: Fri Apr  7 19:07:39 2023, max compression
+gzip compressed data, was "arcanum-newspaper-segmentation-client-1.6.1.tar", last modified: Wed Apr 12 09:03:33 2023, max compression
```

## Comparing `arcanum-newspaper-segmentation-client-1.5.4.tar` & `arcanum-newspaper-segmentation-client-1.6.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 19:07:39.229790 arcanum-newspaper-segmentation-client-1.5.4/
--rw-rw-rw-   0        0        0     1101 2022-01-17 15:03:50.000000 arcanum-newspaper-segmentation-client-1.5.4/LICENSE
--rw-rw-rw-   0        0        0      675 2023-04-07 19:07:39.229790 arcanum-newspaper-segmentation-client-1.5.4/PKG-INFO
--rw-rw-rw-   0        0        0      156 2022-01-17 15:03:50.000000 arcanum-newspaper-segmentation-client-1.5.4/README.md
--rw-rw-rw-   0        0        0      110 2022-01-17 15:03:50.000000 arcanum-newspaper-segmentation-client-1.5.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-07 19:07:39.229790 arcanum-newspaper-segmentation-client-1.5.4/setup.cfg
--rw-rw-rw-   0        0        0      937 2023-04-07 19:07:27.000000 arcanum-newspaper-segmentation-client-1.5.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-07 19:07:39.198594 arcanum-newspaper-segmentation-client-1.5.4/src/
-drwxrwxrwx   0        0        0        0 2023-04-07 19:07:39.229790 arcanum-newspaper-segmentation-client-1.5.4/src/arcanum_newspaper_segmentation_client.egg-info/
--rw-rw-rw-   0        0        0      675 2023-04-07 19:07:39.000000 arcanum-newspaper-segmentation-client-1.5.4/src/arcanum_newspaper_segmentation_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      578 2023-04-07 19:07:39.000000 arcanum-newspaper-segmentation-client-1.5.4/src/arcanum_newspaper_segmentation_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 19:07:39.000000 arcanum-newspaper-segmentation-client-1.5.4/src/arcanum_newspaper_segmentation_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-04-07 19:07:39.000000 arcanum-newspaper-segmentation-client-1.5.4/src/arcanum_newspaper_segmentation_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       30 2023-04-07 19:07:39.000000 arcanum-newspaper-segmentation-client-1.5.4/src/arcanum_newspaper_segmentation_client.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-07 19:07:39.229790 arcanum-newspaper-segmentation-client-1.5.4/src/newspaper_segmentation_client/
--rw-rw-rw-   0        0        0    12979 2023-04-07 18:09:27.000000 arcanum-newspaper-segmentation-client-1.5.4/src/newspaper_segmentation_client/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-04-07 19:07:15.000000 arcanum-newspaper-segmentation-client-1.5.4/src/newspaper_segmentation_client/clip.py
--rw-rw-rw-   0        0        0    16873 2022-08-01 09:09:51.000000 arcanum-newspaper-segmentation-client-1.5.4/src/newspaper_segmentation_client/mets.py
--rw-rw-rw-   0        0        0     2269 2023-04-04 22:05:29.000000 arcanum-newspaper-segmentation-client-1.5.4/src/newspaper_segmentation_client/pdf.py
--rw-rw-rw-   0        0        0      704 2023-04-07 18:17:10.000000 arcanum-newspaper-segmentation-client-1.5.4/src/newspaper_segmentation_client/text.py
+drwxrwxrwx   0        0        0        0 2023-04-12 09:03:33.489916 arcanum-newspaper-segmentation-client-1.6.1/
+-rw-rw-rw-   0        0        0     1101 2022-01-17 15:03:50.000000 arcanum-newspaper-segmentation-client-1.6.1/LICENSE
+-rw-rw-rw-   0        0        0      675 2023-04-12 09:03:33.489916 arcanum-newspaper-segmentation-client-1.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0      156 2022-01-17 15:03:50.000000 arcanum-newspaper-segmentation-client-1.6.1/README.md
+-rw-rw-rw-   0        0        0      110 2022-01-17 15:03:50.000000 arcanum-newspaper-segmentation-client-1.6.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-12 09:03:33.489916 arcanum-newspaper-segmentation-client-1.6.1/setup.cfg
+-rw-rw-rw-   0        0        0      937 2023-04-12 09:03:06.000000 arcanum-newspaper-segmentation-client-1.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 09:03:33.462988 arcanum-newspaper-segmentation-client-1.6.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-12 09:03:33.483931 arcanum-newspaper-segmentation-client-1.6.1/src/arcanum_newspaper_segmentation_client.egg-info/
+-rw-rw-rw-   0        0        0      675 2023-04-12 09:03:33.000000 arcanum-newspaper-segmentation-client-1.6.1/src/arcanum_newspaper_segmentation_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      578 2023-04-12 09:03:33.000000 arcanum-newspaper-segmentation-client-1.6.1/src/arcanum_newspaper_segmentation_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 09:03:33.000000 arcanum-newspaper-segmentation-client-1.6.1/src/arcanum_newspaper_segmentation_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-04-12 09:03:33.000000 arcanum-newspaper-segmentation-client-1.6.1/src/arcanum_newspaper_segmentation_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       30 2023-04-12 09:03:33.000000 arcanum-newspaper-segmentation-client-1.6.1/src/arcanum_newspaper_segmentation_client.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 09:03:33.488919 arcanum-newspaper-segmentation-client-1.6.1/src/newspaper_segmentation_client/
+-rw-rw-rw-   0        0        0    12514 2023-04-11 20:52:20.000000 arcanum-newspaper-segmentation-client-1.6.1/src/newspaper_segmentation_client/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-04-07 19:07:15.000000 arcanum-newspaper-segmentation-client-1.6.1/src/newspaper_segmentation_client/clip.py
+-rw-rw-rw-   0        0        0    16873 2022-08-01 09:09:51.000000 arcanum-newspaper-segmentation-client-1.6.1/src/newspaper_segmentation_client/mets.py
+-rw-rw-rw-   0        0        0     2771 2023-04-11 20:46:31.000000 arcanum-newspaper-segmentation-client-1.6.1/src/newspaper_segmentation_client/pdf.py
+-rw-rw-rw-   0        0        0      704 2023-04-07 18:17:10.000000 arcanum-newspaper-segmentation-client-1.6.1/src/newspaper_segmentation_client/text.py
```

### Comparing `arcanum-newspaper-segmentation-client-1.5.4/LICENSE` & `arcanum-newspaper-segmentation-client-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `arcanum-newspaper-segmentation-client-1.5.4/PKG-INFO` & `arcanum-newspaper-segmentation-client-1.6.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcanum-newspaper-segmentation-client
-Version: 1.5.4
+Version: 1.6.1
 Summary: Client for Arcanum's Newspaper Segmentation API
 Home-page: https://www.arcanum.com/en/newspaper-segmentation/
 Author: Biszak Előd (Arcanum Ltd)
 Author-email: elod.biszak@arcanum.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `arcanum-newspaper-segmentation-client-1.5.4/setup.py` & `arcanum-newspaper-segmentation-client-1.6.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="arcanum-newspaper-segmentation-client",
-    version="1.5.4",
+    version="1.6.1",
     author="Biszak Előd (Arcanum Ltd)",
     author_email="elod.biszak@arcanum.com",
     description="Client for Arcanum's Newspaper Segmentation API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.arcanum.com/en/newspaper-segmentation/",
     classifiers=[
```

### Comparing `arcanum-newspaper-segmentation-client-1.5.4/src/arcanum_newspaper_segmentation_client.egg-info/PKG-INFO` & `arcanum-newspaper-segmentation-client-1.6.1/src/arcanum_newspaper_segmentation_client.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcanum-newspaper-segmentation-client
-Version: 1.5.4
+Version: 1.6.1
 Summary: Client for Arcanum's Newspaper Segmentation API
 Home-page: https://www.arcanum.com/en/newspaper-segmentation/
 Author: Biszak Előd (Arcanum Ltd)
 Author-email: elod.biszak@arcanum.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `arcanum-newspaper-segmentation-client-1.5.4/src/arcanum_newspaper_segmentation_client.egg-info/SOURCES.txt` & `arcanum-newspaper-segmentation-client-1.6.1/src/arcanum_newspaper_segmentation_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arcanum-newspaper-segmentation-client-1.5.4/src/newspaper_segmentation_client/__init__.py` & `arcanum-newspaper-segmentation-client-1.6.1/src/newspaper_segmentation_client/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 import math
 import json
 import io
 import concurrent.futures
 from typing import BinaryIO
 
 import requests
-import fitz
 import numpy as np
 from PIL import Image, ImageDraw
 
-from .pdf import render_pdf_page, extract_pdf_text_to_textract_format
-
 
 def rotate_point(matrix, point, translate=(0, 0)):
     return (matrix[0][0] * point[0] + matrix[0][1] * point[1] + translate[0],
             matrix[1][0] * point[0] + matrix[1][1] * point[1] + translate[1])
 
 
 def get_angle_from_textract_lines(image, textract_response):
@@ -285,16 +282,7 @@
 
     response = requests.get("https://api.arcanum.com/v1/newspaper-segmentation/analyze-page",
                             data=json.dumps(
                                 {"image": upload_url_response["key"], "textract_response": textract_response}),
                             headers={"x-api-key": api_key})
 
     return response.json()
-
-
-def run_newspaper_segmentation_on_pdf_page(page: fitz.Page, api_key: str):
-    image = Image.fromarray(render_pdf_page(page))
-    pdf_text = extract_pdf_text_to_textract_format(page)
-    with io.BytesIO() as image_io:
-        image.save(image_io, "JPEG")
-        image_io.seek(0)
-        return run_newspaper_segmentation_without_textract(image_io, pdf_text, api_key)
```

### Comparing `arcanum-newspaper-segmentation-client-1.5.4/src/newspaper_segmentation_client/clip.py` & `arcanum-newspaper-segmentation-client-1.6.1/src/newspaper_segmentation_client/clip.py`

 * *Files identical despite different names*

### Comparing `arcanum-newspaper-segmentation-client-1.5.4/src/newspaper_segmentation_client/mets.py` & `arcanum-newspaper-segmentation-client-1.6.1/src/newspaper_segmentation_client/mets.py`

 * *Files identical despite different names*

### Comparing `arcanum-newspaper-segmentation-client-1.5.4/src/newspaper_segmentation_client/pdf.py` & `arcanum-newspaper-segmentation-client-1.6.1/src/newspaper_segmentation_client/pdf.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 from typing import Dict, Tuple
+import io
 
+from PIL import Image
 import numpy as np
 import fitz
 
+from newspaper_segmentation_client import run_newspaper_segmentation_without_textract
+
 
 def render_pdf_page(page: fitz.Page, dpi: int = 150) -> np.ndarray:
     mat = fitz.Matrix(dpi / 72, dpi / 72)
     pix = page.get_pixmap(matrix=mat, annots=False, alpha=False)
     image = np.array(bytearray(pix.samples), dtype=np.uint8)
     return np.reshape(image, (pix.height, pix.width, 3))
 
@@ -53,7 +57,16 @@
             line_id += 1
 
     pdf_text_textract_format["Blocks"][0]["Relationships"] = [
         {"Ids": line_ids, "Type": "CHILD"}
     ]
 
     return pdf_text_textract_format
+
+
+def run_newspaper_segmentation_on_pdf_page(page: fitz.Page, api_key: str):
+    image = Image.fromarray(render_pdf_page(page))
+    pdf_text = extract_pdf_text_to_textract_format(page)
+    with io.BytesIO() as image_io:
+        image.save(image_io, "JPEG")
+        image_io.seek(0)
+        return run_newspaper_segmentation_without_textract(image_io, pdf_text, api_key)
```

### Comparing `arcanum-newspaper-segmentation-client-1.5.4/src/newspaper_segmentation_client/text.py` & `arcanum-newspaper-segmentation-client-1.6.1/src/newspaper_segmentation_client/text.py`

 * *Files identical despite different names*

