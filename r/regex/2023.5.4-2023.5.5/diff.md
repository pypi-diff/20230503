# Comparing `tmp/regex-2023.5.4.tar.gz` & `tmp/regex-2023.5.5-cp311-cp311-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regex-2023.5.4.tar", last modified: Tue May  2 16:43:53 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

