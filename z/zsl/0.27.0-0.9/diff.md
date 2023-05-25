# Comparing `tmp/zsl-0.27.0.tar.gz` & `tmp/zsl-0.9-py2-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zsl-0.27.0.tar", last modified: Thu May 25 18:08:23 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

