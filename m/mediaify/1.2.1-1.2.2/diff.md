# Comparing `tmp/mediaify-1.2.1.tar.gz` & `tmp/mediaify-1.2.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mediaify-1.2.1.tar", last modified: Wed Apr 12 19:33:42 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

