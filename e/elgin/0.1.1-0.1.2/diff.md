# Comparing `tmp/elgin-0.1.1.tar.gz` & `tmp/elgin-0.1.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elgin-0.1.1.tar", last modified: Thu May 25 15:04:47 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

