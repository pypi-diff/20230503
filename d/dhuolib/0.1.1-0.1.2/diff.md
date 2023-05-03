# Comparing `tmp/dhuolib-0.1.1.tar.gz` & `tmp/dhuolib-0.1.2.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dhuolib-0.1.1.tar", last modified: Tue May  2 19:37:13 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

