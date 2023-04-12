# Comparing `tmp/sentencepiece-0.1.97.tar.gz` & `tmp/sentencepiece-0.1.98-cp39-cp39-manylinux_2_17_i686.manylinux2014_i686.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentencepiece-0.1.97.tar", last modified: Sat Aug  6 16:18:48 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

