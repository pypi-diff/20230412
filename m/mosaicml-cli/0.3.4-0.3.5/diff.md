# Comparing `tmp/mosaicml-cli-0.3.4.tar.gz` & `tmp/mosaicml_cli-0.3.5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosaicml-cli-0.3.4.tar", last modified: Fri Apr  7 22:51:48 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

