# Comparing `tmp/pycachera-3.0.0.tar.gz` & `tmp/pycachera-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycachera-3.0.0.tar", last modified: Sun Apr  2 06:44:10 2023, max compression
+gzip compressed data, was "pycachera-3.0.1.tar", last modified: Wed Apr 12 03:30:48 2023, max compression
```

## Comparing `pycachera-3.0.0.tar` & `pycachera-3.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-02 06:44:10.873275 pycachera-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1081 2023-04-02 06:43:59.000000 pycachera-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      237 2023-04-02 06:44:10.873275 pycachera-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2131 2023-04-02 06:43:59.000000 pycachera-3.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-02 06:44:10.869275 pycachera-3.0.0/pycachera/
--rw-r--r--   0 runner    (1001) docker     (122)      195 2023-04-02 06:43:59.000000 pycachera-3.0.0/pycachera/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5221 2023-04-02 06:43:59.000000 pycachera-3.0.0/pycachera/cacher.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-02 06:44:10.873275 pycachera-3.0.0/pycachera.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      237 2023-04-02 06:44:10.000000 pycachera-3.0.0/pycachera.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      232 2023-04-02 06:44:10.000000 pycachera-3.0.0/pycachera.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-02 06:44:10.000000 pycachera-3.0.0/pycachera.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-04-02 06:44:10.000000 pycachera-3.0.0/pycachera.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-02 06:44:10.000000 pycachera-3.0.0/pycachera.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-02 06:44:10.873275 pycachera-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      465 2023-04-02 06:43:59.000000 pycachera-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 03:30:48.423467 pycachera-3.0.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1081 2023-04-12 03:30:36.000000 pycachera-3.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      277 2023-04-12 03:30:48.423467 pycachera-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2270 2023-04-12 03:30:36.000000 pycachera-3.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 03:30:48.423467 pycachera-3.0.1/pycachera/
+-rw-r--r--   0 runner    (1001) docker     (122)      196 2023-04-12 03:30:36.000000 pycachera-3.0.1/pycachera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5203 2023-04-12 03:30:36.000000 pycachera-3.0.1/pycachera/cacher.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 03:30:48.423467 pycachera-3.0.1/pycachera.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      277 2023-04-12 03:30:48.000000 pycachera-3.0.1/pycachera.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      232 2023-04-12 03:30:48.000000 pycachera-3.0.1/pycachera.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-12 03:30:48.000000 pycachera-3.0.1/pycachera.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-04-12 03:30:48.000000 pycachera-3.0.1/pycachera.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-12 03:30:48.000000 pycachera-3.0.1/pycachera.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-12 03:30:48.423467 pycachera-3.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      521 2023-04-12 03:30:36.000000 pycachera-3.0.1/setup.py
```

### Comparing `pycachera-3.0.0/LICENSE` & `pycachera-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pycachera-3.0.0/README.md` & `pycachera-3.0.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -20,60 +20,72 @@
 
 ```
 from pycachera import cache
 ```
 
 For caching a function
 ```
-@cache(Cobject='function')
+@cache()
 def sum(a,b):
    return a+b
 ```
 
-For caching a class attributes
+For caching a class attributes.
 
 ```
 class Math:
    def __init__(self):
        pass
    
-   @cache(Cobject='class')
+   @cache()
    def sum(a,b):
       return a + b  
 ```
 
-For caching to a specific directory
+For caching to a specific directory.
 
 ```
-@cache(cachefolder='/home/user/scratch',Cobject='function')
+@cache(cachefolder='/home/user/scratch')
 def sum(a,b):
    return a+b
 ```
 
 For caching with a specific key
 
 ```
-@cache(cachekey='This a custom cache',Cobject='function')
+@cache(cachekey='This a custom cache')
 def sum(a,b):
    return a+b
 ```
 
 For printing the info
 
 ```
-@cache(verbose=True,Cobject='function')
+@cache(verbose=True)
 def sum(a,b):
    return a+b
 ```
 
 While debugging your script if you want to ignore the cached values you can recache
 ```
-@cache(recache=True,Cobject='function')
+@cache(recache=True)
 def sum(a,b):
    return a+b
 ```
 
+When you use cache with a class attribute, and if you want to consider some attributes of that class for caching,
+
+```
+class Math:
+   def __init__(self,c):
+       self.c = c
+   
+   @cache(extrarg=['c'])
+   def sum(a,b):
+      return a + b  
+```
+
 
 
 ## API
 
 visit [pycachera.readthedocs.io](https://pycachera.readthedocs.io/en/latest/)
```

### Comparing `pycachera-3.0.0/pycachera/cacher.py` & `pycachera-3.0.1/pycachera/cacher.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,14 @@
     This is a decorator class, used for caching functions and class attributes.
     
     Args(optional):
         :cachefolder (*str*): Folder for caching; if not found, the cache folder is set to '.cache' in the current working directory
         :extraarg (*list*): If the function is a class method, you can give the extra arguments of the class as a list just for saving the cache
         :cachekey (*str*): You can override the above method by giving a particular human readable key(str) for example: 'This is a function with fknee is 5, and alpha is 3'
         :verbose (*bool*): Just to know what's happening inside
-        :Cobject (*str*): If the function is a class method, set it to 'class', else 'function'
         :recache (*bool*): If you want to recache the function, set it to True
     
     Usage:
         >>> from pycachera import cache
         >>> @cache()
         >>> def myfunc(self, x):
         >>>     return x**2
@@ -130,18 +129,20 @@
                 a += f'{len(tag)}'
 
         return md5(a.encode()).hexdigest()
     
     def file_writer(self,name,data):
         """
         Writes data to a file
+        save the data in a pickle file
         """
         with open(name, 'wb') as writ:
             pl.dump(data, writ)
             
     def file_reader(self,name):
         """
         Reads data from a file
+        save the data in a pickle file
         """
         with open(name, 'rb') as rea:
             data = pl.load(rea)
         return data
```

