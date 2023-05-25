# Comparing `tmp/djangocms-blog-2.0.0b1.tar.gz` & `tmp/djangocms-blog-2.0.0b2.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/srv/dev/apps/djangocms-blog/dist/.tmp-_3i33xqi/djangocms-blog-2.0.0b1.tar", last modified: Sun May  7 19:56:19 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

