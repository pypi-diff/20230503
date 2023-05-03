# Comparing `tmp/bpf4-1.8.5.tar.gz` & `tmp/bpf4-1.8.6-cp39-cp39-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpf4-1.8.5.tar", last modified: Sun Apr 23 20:53:36 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

