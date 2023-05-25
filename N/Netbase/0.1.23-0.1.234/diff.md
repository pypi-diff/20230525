# Comparing `tmp/Netbase-0.1.23.tar.gz` & `tmp/Netbase-0.1.234-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Netbase-0.1.23.tar", last modified: Thu Nov  2 11:01:05 2017, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

