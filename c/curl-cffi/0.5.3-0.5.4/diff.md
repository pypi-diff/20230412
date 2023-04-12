# Comparing `tmp/curl_cffi-0.5.3.tar.gz` & `tmp/curl_cffi-0.5.4-cp37-abi3-macosx_11_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curl_cffi-0.5.3.tar", last modified: Fri Apr  7 11:14:11 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

