# Comparing `tmp/pyhgl-0.1.0.tar.gz` & `tmp/pyhgl-0.2.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhgl-0.1.0.tar", last modified: Mon Oct 17 08:47:44 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

