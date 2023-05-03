# Comparing `tmp/ft_package_42_jekim-0.0.1.tar.gz` & `tmp/ft_package_42_jekim-0.0.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ft_package_42_jekim-0.0.1.tar", last modified: Wed May  3 16:57:20 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

