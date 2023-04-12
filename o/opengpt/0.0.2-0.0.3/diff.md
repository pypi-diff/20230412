# Comparing `tmp/opengpt-0.0.2.tar.gz` & `tmp/opengpt-0.0.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/data/zeljko/projects/opengpt/dist/.tmp-j11dmewh/opengpt-0.0.2.tar", last modified: Mon Apr  3 16:27:30 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

