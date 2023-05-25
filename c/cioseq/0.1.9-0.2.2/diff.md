# Comparing `tmp/cioseq-0.1.9.tar.gz` & `tmp/cioseq-0.2.2-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cioseq-0.1.9.tar", last modified: Wed Mar 10 03:56:33 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

