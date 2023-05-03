# Comparing `tmp/jaco2-3.5.tar.gz` & `tmp/jaco2-3.7-cp311-cp311-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaco2-3.5.tar", last modified: Tue May  2 21:45:42 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

