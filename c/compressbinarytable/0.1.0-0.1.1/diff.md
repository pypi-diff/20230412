# Comparing `tmp/compressbinarytable-0.1.0.tar.gz` & `tmp/compressbinarytable-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compressbinarytable-0.1.0.tar", max compression
+gzip compressed data, was "compressbinarytable-0.1.1.tar", max compression
```

## Comparing `compressbinarytable-0.1.0.tar` & `compressbinarytable-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      296 2023-04-12 11:43:33.290936 compressbinarytable-0.1.0/README.md
--rw-r--r--   0        0        0     7211 2023-04-12 13:14:25.968938 compressbinarytable-0.1.0/compressbinarytable/__main__.py
--rw-r--r--   0        0        0      435 2023-04-12 13:20:48.849787 compressbinarytable-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      813 1970-01-01 00:00:00.000000 compressbinarytable-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      296 2023-04-12 11:43:33.290936 compressbinarytable-0.1.1/README.md
+-rw-r--r--   0        0        0     7299 2023-04-12 13:32:21.917314 compressbinarytable-0.1.1/compressbinarytable/__main__.py
+-rw-r--r--   0        0        0      435 2023-04-12 13:32:50.493474 compressbinarytable-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      813 1970-01-01 00:00:00.000000 compressbinarytable-0.1.1/PKG-INFO
```

### Comparing `compressbinarytable-0.1.0/compressbinarytable/__main__.py` & `compressbinarytable-0.1.1/compressbinarytable/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,15 +207,17 @@
     columns = lines[0][1:]
 
     return_array = np.array(columns)
 
     return return_array 
 
 
-if __name__ == "__main__":
+def main(args):
+
+    # Main function to call from command line
 
     parser = argparse.ArgumentParser(description='Compression of Binary Mutation Tables')
 
     parser.add_argument("-c", help="Compression flag", action="store_true")
 
     parser.add_argument("-d", help="Decompression flag", action="store_true")
 
@@ -275,7 +277,11 @@
     
     else:
         print("You need to select either Compression -c or Decompression -d")
         exit()
 
 
 
+
+if __name__ == "__main__":
+
+    main(sys.argv[1:])
```

### Comparing `compressbinarytable-0.1.0/PKG-INFO` & `compressbinarytable-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compressbinarytable
-Version: 0.1.0
+Version: 0.1.1
 Summary: Compresses binary tables
 Author: Alper Yurtseven
 Author-email: alper.yurtseven@helmholtz-hips.de
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

