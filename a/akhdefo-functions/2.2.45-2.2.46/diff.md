# Comparing `tmp/akhdefo_functions-2.2.45.tar.gz` & `tmp/akhdefo_functions-2.2.46-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akhdefo_functions-2.2.45.tar", last modified: Sun Feb 26 19:14:14 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

