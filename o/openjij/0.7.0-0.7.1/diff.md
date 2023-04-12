# Comparing `tmp/openjij-0.7.0.tar.gz` & `tmp/openjij-0.7.1-cp39-cp39-manylinux_2_28_aarch64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openjij-0.7.0.tar", last modified: Mon Apr 10 05:30:12 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

