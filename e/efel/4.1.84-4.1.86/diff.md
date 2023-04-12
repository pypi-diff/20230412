# Comparing `tmp/efel-4.1.84.tar.gz` & `tmp/efel-4.1.86-cp311-cp311-macosx_10_9_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efel-4.1.84.tar", last modified: Tue Mar 21 12:28:32 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

