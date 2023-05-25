# Comparing `tmp/hopic-1.61.0.tar.gz` & `tmp/hopic-1.61.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/jenkins/workspace/hopic_release_1/dist/tmp0nf7l9tz/hopic-1.61.0.tar", last modified: Mon May 22 07:41:46 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

