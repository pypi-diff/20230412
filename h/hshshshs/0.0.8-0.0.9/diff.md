# Comparing `tmp/hshshshs-0.0.8.tar.gz` & `tmp/hshshshs-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hshshshs-0.0.8.tar", last modified: Thu Apr  6 10:28:51 2023, max compression
+gzip compressed data, was "hshshshs-0.0.9.tar", last modified: Wed Apr 12 07:24:05 2023, max compression
```

## Comparing `hshshshs-0.0.8.tar` & `hshshshs-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 10:28:51.760508 hshshshs-0.0.8/
--rw-rw-rw-   0        0        0      261 2023-04-06 10:28:51.759508 hshshshs-0.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-06 10:28:51.734528 hshshshs-0.0.8/hshshshs/
--rw-rw-rw-   0        0        0        0 2023-03-17 08:41:46.000000 hshshshs-0.0.8/hshshshs/__init__.py
--rw-rw-rw-   0        0        0     2834 2023-04-06 10:27:40.000000 hshshshs-0.0.8/hshshshs/cFunction.py
-drwxrwxrwx   0        0        0        0 2023-04-06 10:28:51.758509 hshshshs-0.0.8/hshshshs.egg-info/
--rw-rw-rw-   0        0        0      261 2023-04-06 10:28:51.000000 hshshshs-0.0.8/hshshshs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2023-04-06 10:28:51.000000 hshshshs-0.0.8/hshshshs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 10:28:51.000000 hshshshs-0.0.8/hshshshs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-06 10:28:51.000000 hshshshs-0.0.8/hshshshs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-06 10:28:51.000000 hshshshs-0.0.8/hshshshs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-06 10:28:51.760508 hshshshs-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      978 2023-04-06 10:27:10.000000 hshshshs-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 07:24:05.171918 hshshshs-0.0.9/
+-rw-rw-rw-   0        0        0      261 2023-04-12 07:24:05.170919 hshshshs-0.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-12 07:24:05.160925 hshshshs-0.0.9/hshshshs/
+-rw-rw-rw-   0        0        0        0 2023-03-17 08:41:46.000000 hshshshs-0.0.9/hshshshs/__init__.py
+-rw-rw-rw-   0        0        0     5714 2023-04-12 07:22:47.000000 hshshshs-0.0.9/hshshshs/cFunction.py
+drwxrwxrwx   0        0        0        0 2023-04-12 07:24:05.168920 hshshshs-0.0.9/hshshshs.egg-info/
+-rw-rw-rw-   0        0        0      261 2023-04-12 07:24:05.000000 hshshshs-0.0.9/hshshshs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2023-04-12 07:24:05.000000 hshshshs-0.0.9/hshshshs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 07:24:05.000000 hshshshs-0.0.9/hshshshs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-04-12 07:24:05.000000 hshshshs-0.0.9/hshshshs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-12 07:24:05.000000 hshshshs-0.0.9/hshshshs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 07:24:05.171918 hshshshs-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1005 2023-04-12 07:22:54.000000 hshshshs-0.0.9/setup.py
```

### Comparing `hshshshs-0.0.8/setup.py` & `hshshshs-0.0.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,16 +15,16 @@
                 module_name = "%(base)s.%(item)s" % vars()
             else:
                 module_name = item
             packages[module_name] = dir
             packages.update(find_packages(dir, module_name))
     return packages
 setup(  name="hshshshs",
-        version="0.0.8",
+        version="0.0.9",
         url="http://github.com/kimhansu/hshshshs",
         license="MIT",
         author="kimhansu",
         author_email="gimhansu@naver.com",
         keywords=["calendar","isoweek","listsum"],
         description="math function",
         packages=find_packages("."),
-        install_requires=["isoweek"])
+        install_requires=["isoweek","datetime","relativedelta"])
```

