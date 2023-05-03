# Comparing `tmp/charidotella-0.9.tar.gz` & `tmp/charidotella-1.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "charidotella-0.9.tar", last modified: Fri Apr 28 12:39:27 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

