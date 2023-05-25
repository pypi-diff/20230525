# Comparing `tmp/geodistance-0.1.6.tar.gz` & `tmp/geodistance-0.1.7-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\geodistance-0.1.6.tar", last modified: Thu May 25 11:37:02 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

