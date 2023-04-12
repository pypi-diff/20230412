# Comparing `tmp/ifd_python-6.0.tar.gz` & `tmp/ifd_python-7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ifd_python-6.0.tar", max compression
+gzip compressed data, was "ifd_python-7.0.tar", max compression
```

## Comparing `ifd_python-6.0.tar` & `ifd_python-7.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1093 2023-04-12 12:43:31.521191 ifd_python-6.0/LICENSE
--rw-r--r--   0        0        0      551 2023-04-12 12:43:31.521191 ifd_python-6.0/README.md
--rw-r--r--   0        0        0      283 2023-04-12 12:43:31.521191 ifd_python-6.0/ifd/__init__.py
--rw-r--r--   0        0        0      971 2023-04-12 12:43:31.521191 ifd_python-6.0/ifd/entities/Abstract/ADetection.py
--rw-r--r--   0        0        0       34 2023-04-12 12:43:31.521191 ifd_python-6.0/ifd/entities/Abstract/__init__.py
--rw-r--r--   0        0        0      673 2023-04-12 12:43:31.521191 ifd_python-6.0/ifd/entities/Classification.py
--rw-r--r--   0        0        0      228 2023-04-12 12:43:31.521191 ifd_python-6.0/ifd/entities/Couleur.py
--rw-r--r--   0        0        0      646 2023-04-12 12:43:31.521191 ifd_python-6.0/ifd/entities/Detection.py
--rw-r--r--   0        0        0     2089 2023-04-12 12:43:31.521191 ifd_python-6.0/ifd/entities/Image.py
--rw-r--r--   0        0        0     1453 2023-04-12 12:43:31.521191 ifd_python-6.0/ifd/entities/LogResult.py
--rw-r--r--   0        0        0      416 2023-04-12 12:43:31.521191 ifd_python-6.0/ifd/entities/Modele.py
--rw-r--r--   0        0        0      741 2023-04-12 12:43:31.521191 ifd_python-6.0/ifd/entities/OCR.py
--rw-r--r--   0        0        0      517 2023-04-12 12:43:31.521191 ifd_python-6.0/ifd/entities/RabbitMqMessage.py
--rw-r--r--   0        0        0      208 2023-04-12 12:43:31.521191 ifd_python-6.0/ifd/entities/__init__.py
--rw-r--r--   0        0        0      656 2023-04-12 12:43:31.521191 ifd_python-6.0/ifd/entities/bbox.py
--rw-r--r--   0        0        0     2162 2023-04-12 12:43:31.521191 ifd_python-6.0/ifd/repository/AmqpImageRepository.py
--rw-r--r--   0        0        0       88 2023-04-12 12:43:31.521191 ifd_python-6.0/ifd/repository/Interfaces/IImageRepository.py
--rw-r--r--   0        0        0       46 2023-04-12 12:43:31.521191 ifd_python-6.0/ifd/repository/Interfaces/__init__.py
--rw-r--r--   0        0        0      192 2023-04-12 12:43:31.521191 ifd_python-6.0/ifd/repository/MemoryImageRepository.py
--rw-r--r--   0        0        0      110 2023-04-12 12:43:31.521191 ifd_python-6.0/ifd/repository/__init__.py
--rw-r--r--   0        0        0      645 2023-04-12 15:28:49.954314 ifd_python-6.0/ifd/spec.py
--rw-r--r--   0        0        0      558 2023-04-12 12:43:31.521191 ifd_python-6.0/ifd/tools.py
--rw-r--r--   0        0        0       77 2023-04-12 12:43:31.521191 ifd_python-6.0/ifd/usecase/Interfaces/IFonction.py
--rw-r--r--   0        0        0       32 2023-04-12 12:43:31.521191 ifd_python-6.0/ifd/usecase/Interfaces/__init__.py
--rw-r--r--   0        0        0        0 2023-04-12 15:29:07.262162 ifd_python-6.0/ifd/usecase/__init__.py
--rw-r--r--   0        0        0      327 2023-04-12 15:29:16.838077 ifd_python-6.0/pyproject.toml
--rw-r--r--   0        0        0     1084 1970-01-01 00:00:00.000000 ifd_python-6.0/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-04-12 12:43:31.521191 ifd_python-7.0/LICENSE
+-rw-r--r--   0        0        0      551 2023-04-12 12:43:31.521191 ifd_python-7.0/README.md
+-rw-r--r--   0        0        0      283 2023-04-12 12:43:31.521191 ifd_python-7.0/ifd/__init__.py
+-rw-r--r--   0        0        0      971 2023-04-12 12:43:31.521191 ifd_python-7.0/ifd/entities/Abstract/ADetection.py
+-rw-r--r--   0        0        0       34 2023-04-12 12:43:31.521191 ifd_python-7.0/ifd/entities/Abstract/__init__.py
+-rw-r--r--   0        0        0      673 2023-04-12 12:43:31.521191 ifd_python-7.0/ifd/entities/Classification.py
+-rw-r--r--   0        0        0      228 2023-04-12 12:43:31.521191 ifd_python-7.0/ifd/entities/Couleur.py
+-rw-r--r--   0        0        0      646 2023-04-12 12:43:31.521191 ifd_python-7.0/ifd/entities/Detection.py
+-rw-r--r--   0        0        0     2089 2023-04-12 12:43:31.521191 ifd_python-7.0/ifd/entities/Image.py
+-rw-r--r--   0        0        0     1453 2023-04-12 12:43:31.521191 ifd_python-7.0/ifd/entities/LogResult.py
+-rw-r--r--   0        0        0      416 2023-04-12 12:43:31.521191 ifd_python-7.0/ifd/entities/Modele.py
+-rw-r--r--   0        0        0      741 2023-04-12 12:43:31.521191 ifd_python-7.0/ifd/entities/OCR.py
+-rw-r--r--   0        0        0      517 2023-04-12 12:43:31.521191 ifd_python-7.0/ifd/entities/RabbitMqMessage.py
+-rw-r--r--   0        0        0      208 2023-04-12 12:43:31.521191 ifd_python-7.0/ifd/entities/__init__.py
+-rw-r--r--   0        0        0      656 2023-04-12 12:43:31.521191 ifd_python-7.0/ifd/entities/bbox.py
+-rw-r--r--   0        0        0     2162 2023-04-12 12:43:31.521191 ifd_python-7.0/ifd/repository/AmqpImageRepository.py
+-rw-r--r--   0        0        0       88 2023-04-12 12:43:31.521191 ifd_python-7.0/ifd/repository/Interfaces/IImageRepository.py
+-rw-r--r--   0        0        0       46 2023-04-12 12:43:31.521191 ifd_python-7.0/ifd/repository/Interfaces/__init__.py
+-rw-r--r--   0        0        0      192 2023-04-12 12:43:31.521191 ifd_python-7.0/ifd/repository/MemoryImageRepository.py
+-rw-r--r--   0        0        0      110 2023-04-12 12:43:31.521191 ifd_python-7.0/ifd/repository/__init__.py
+-rw-r--r--   0        0        0      419 2023-04-12 15:32:33.076346 ifd_python-7.0/ifd/spec.py
+-rw-r--r--   0        0        0      558 2023-04-12 12:43:31.521191 ifd_python-7.0/ifd/tools.py
+-rw-r--r--   0        0        0       77 2023-04-12 12:43:31.521191 ifd_python-7.0/ifd/usecase/Interfaces/IFonction.py
+-rw-r--r--   0        0        0       32 2023-04-12 12:43:31.521191 ifd_python-7.0/ifd/usecase/Interfaces/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-12 15:32:49.088205 ifd_python-7.0/ifd/usecase/__init__.py
+-rw-r--r--   0        0        0      327 2023-04-12 15:32:58.544122 ifd_python-7.0/pyproject.toml
+-rw-r--r--   0        0        0     1084 1970-01-01 00:00:00.000000 ifd_python-7.0/PKG-INFO
```

### Comparing `ifd_python-6.0/LICENSE` & `ifd_python-7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ifd_python-6.0/README.md` & `ifd_python-7.0/README.md`

 * *Files identical despite different names*

### Comparing `ifd_python-6.0/ifd/entities/Abstract/ADetection.py` & `ifd_python-7.0/ifd/entities/Abstract/ADetection.py`

 * *Files identical despite different names*

### Comparing `ifd_python-6.0/ifd/entities/Classification.py` & `ifd_python-7.0/ifd/entities/Classification.py`

 * *Files identical despite different names*

### Comparing `ifd_python-6.0/ifd/entities/Detection.py` & `ifd_python-7.0/ifd/entities/Detection.py`

 * *Files identical despite different names*

### Comparing `ifd_python-6.0/ifd/entities/Image.py` & `ifd_python-7.0/ifd/entities/Image.py`

 * *Files identical despite different names*

### Comparing `ifd_python-6.0/ifd/entities/LogResult.py` & `ifd_python-7.0/ifd/entities/LogResult.py`

 * *Files identical despite different names*

### Comparing `ifd_python-6.0/ifd/entities/OCR.py` & `ifd_python-7.0/ifd/entities/OCR.py`

 * *Files identical despite different names*

### Comparing `ifd_python-6.0/ifd/entities/RabbitMqMessage.py` & `ifd_python-7.0/ifd/entities/RabbitMqMessage.py`

 * *Files identical despite different names*

### Comparing `ifd_python-6.0/ifd/entities/bbox.py` & `ifd_python-7.0/ifd/entities/bbox.py`

 * *Files identical despite different names*

### Comparing `ifd_python-6.0/ifd/repository/AmqpImageRepository.py` & `ifd_python-7.0/ifd/repository/AmqpImageRepository.py`

 * *Files identical despite different names*

### Comparing `ifd_python-6.0/ifd/tools.py` & `ifd_python-7.0/ifd/tools.py`

 * *Files identical despite different names*

### Comparing `ifd_python-6.0/PKG-INFO` & `ifd_python-7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifd-python
-Version: 6.0
+Version: 7.0
 Summary: 
 Author: Antonin Lemoine
 Author-email: antonin.lemoine@altitudeinfra.fr
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

