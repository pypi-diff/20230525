# Comparing `tmp/jupyterlab_training-0.3.3.tar.gz` & `tmp/jupyterlab_training-0.3.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterlab_training-0.3.3.tar", last modified: Thu May 25 15:46:43 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

