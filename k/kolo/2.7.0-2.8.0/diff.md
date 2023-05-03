# Comparing `tmp/kolo-2.7.0.tar.gz` & `tmp/kolo-2.8.0-cp39-cp39-manylinux_2_17_s390x.manylinux2014_s390x.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

