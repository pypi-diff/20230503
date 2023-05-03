# Comparing `tmp/ib_insync-0.9.82.tar.gz` & `tmp/ib_insync-0.9.9-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ib_insync-0.9.82.tar", last modified: Tue Apr 25 13:17:10 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

