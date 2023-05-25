# Comparing `tmp/makelove-0.0.8-py3-none-any.whl.zip` & `tmp/makelove-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,23 @@
-Zip file size: 26551 bytes, number of entries: 21
+Zip file size: 26621 bytes, number of entries: 21
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-16 23:33 makelove/__init__.py
 -rw-rw-r--  2.0 unx       35 b- defN 20-Aug-12 18:43 makelove/__main__.py
 -rw-rw-r--  2.0 unx     7696 b- defN 20-Nov-03 19:10 makelove/config.py
 -rw-r--r--  2.0 unx     1646 b- defN 20-Mar-25 21:14 makelove/filelist.py
 -rw-r--r--  2.0 unx      733 b- defN 20-Feb-20 20:05 makelove/git_ls_tree.py
 -rw-r--r--  2.0 unx      931 b- defN 20-Feb-19 19:44 makelove/hooks.py
 -rw-r--r--  2.0 unx      520 b- defN 20-Feb-10 23:42 makelove/jsonfile.py
 -rw-r--r--  2.0 unx     7232 b- defN 20-Mar-25 20:36 makelove/linux.py
 -rw-rw-r--  2.0 unx     4368 b- defN 20-Nov-03 19:11 makelove/lovejs.py
 -rw-r--r--  2.0 unx     1704 b- defN 20-Mar-25 17:31 makelove/mac.py
 -rw-rw-r--  2.0 unx     8479 b- defN 20-Aug-12 18:43 makelove/macos.py
 -rw-rw-r--  2.0 unx    12103 b- defN 20-Nov-03 19:10 makelove/makelove.py
--rw-rw-r--  2.0 unx     2476 b- defN 20-Aug-12 18:43 makelove/util.py
+-rw-rw-r--  2.0 unx     2640 b- defN 20-Nov-13 17:03 makelove/util.py
 -rw-r--r--  2.0 unx     3709 b- defN 20-Feb-17 19:27 makelove/validators.py
 -rw-rw-r--  2.0 unx     9462 b- defN 20-Aug-14 19:03 makelove/windows.py
--rw-r--r--  2.0 unx     1071 b- defN 20-Nov-03 19:19 makelove-0.0.8.dist-info/LICENSE
--rw-rw-r--  2.0 unx     7156 b- defN 20-Nov-03 19:19 makelove-0.0.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 20-Nov-03 19:19 makelove-0.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       53 b- defN 20-Nov-03 19:19 makelove-0.0.8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 20-Nov-03 19:19 makelove-0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1616 b- defN 20-Nov-03 19:19 makelove-0.0.8.dist-info/RECORD
-21 files, 71091 bytes uncompressed, 23959 bytes compressed:  66.3%
+-rw-r--r--  2.0 unx     1071 b- defN 20-Nov-13 17:14 makelove-0.0.9.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     7156 b- defN 20-Nov-13 17:14 makelove-0.0.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 20-Nov-13 17:14 makelove-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       53 b- defN 20-Nov-13 17:14 makelove-0.0.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 20-Nov-13 17:14 makelove-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1616 b- defN 20-Nov-13 17:14 makelove-0.0.9.dist-info/RECORD
+21 files, 71255 bytes uncompressed, 24029 bytes compressed:  66.3%
```

## zipnote {}

```diff
@@ -39,26 +39,26 @@
 
 Filename: makelove/validators.py
 Comment: 
 
 Filename: makelove/windows.py
 Comment: 
 
-Filename: makelove-0.0.8.dist-info/LICENSE
+Filename: makelove-0.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: makelove-0.0.8.dist-info/METADATA
+Filename: makelove-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: makelove-0.0.8.dist-info/WHEEL
+Filename: makelove-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: makelove-0.0.8.dist-info/entry_points.txt
+Filename: makelove-0.0.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: makelove-0.0.8.dist-info/top_level.txt
+Filename: makelove-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: makelove-0.0.8.dist-info/RECORD
+Filename: makelove-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## makelove/util.py

```diff
@@ -69,24 +69,29 @@
 
 def get_default_love_binary_dir(version, platform):
     return os.path.join(
         appdirs.user_cache_dir("makelove"), "love-binaries", version, platform
     )
 
 
+# TOOD: Think about hard-coding a big dictionary with download links, so I can error out if I know that there is no download link
 def get_download_url(version, platform):
     # This function is intended to handle all the weird special cases and
-    # is therefore a allowed to be ugly
-    url = "https://github.com/love2d/love/releases/download/{}/".format(version)
-    if list(map(int, version.split("."))) <= [0, 8, 0]:
+    # is therefore allowed to be ugly
+
+    # Other platforms don't use this function
+    assert platform in ["win32", "win64", "macos"]
+
+    url = "https://github.com/love2d/love/releases/download/{}".format(version)
+
+    parsed_version = parse_love_version(version)
+    if parsed_version[0] <= 8:
         platform = {"win32": "win-x86", "win64": "win-x64", "macos": "macosx-ub"}[
             platform
         ]
-    elif version == "0.9.0" and platform == "macos":
+    elif parsed_version[0] == 9 or parsed_version[0] == 10:
         platform = "macosx-x64"
 
     if version == "11.0":
-        # Why? I don't know.
-        filename = "love-11.0.0-{}.zip".format(platform)
-    else:
-        filename = "love-{}-{}.zip".format(version, platform)
-    return url + filename
+        version = "11.0.0"
+
+    return "{}/love-{}-{}.zip".format(url, version, platform)
```

## Comparing `makelove-0.0.8.dist-info/LICENSE` & `makelove-0.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `makelove-0.0.8.dist-info/METADATA` & `makelove-0.0.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: makelove
-Version: 0.0.8
+Version: 0.0.9
 Summary: A packaging tool for [löve](https://love2d.org) games
 Home-page: https://github.com/pfirsich/makelove
 Author: Joel Schumacher
 Author-email: joelschum@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `makelove-0.0.8.dist-info/RECORD` & `makelove-0.0.9.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 makelove/hooks.py,sha256=LCWStGUFqQSjQ3kPOAXxHaIc6sGDhj1OQH-3_-Cqpks,931
 makelove/jsonfile.py,sha256=G8WQIyAMY0nVQ7fk6cMB8rYGSfj-IQ7i_4uz1Pp5y00,520
 makelove/linux.py,sha256=igWib3PoUxXx4Iehl4sNApmTxANpQ_gisEGRgwqqT98,7232
 makelove/lovejs.py,sha256=-l34iJDZjFjqvcNfPAwRXTsGm9TCxzlr4Uel8KEg1W4,4368
 makelove/mac.py,sha256=TjJzv41jmCttO3IrLq-BG89iMD9xmXbjBcSEgzDpABE,1704
 makelove/macos.py,sha256=Kpz_bSDitlTWmYflgk9yDID62H8VkcUS3-B0WkmOpwM,8479
 makelove/makelove.py,sha256=DUyylDCLKGJfU9aaJPcDs7MVwJCQzd1HATUs8UtRWjE,12103
-makelove/util.py,sha256=Gea4_ORp5JBDni0BaCMz-x1UdQOZna6GU4_6TF2XYN4,2476
+makelove/util.py,sha256=x3xvh9f5tHoIczkM7J7HffCFhH_mRh3Bqj0wjGlwZRM,2640
 makelove/validators.py,sha256=0ciiHv8MloUTzEYyFzvMxfnky-h3bH7Ez0I6zVZBjhs,3709
 makelove/windows.py,sha256=8QURa2g4qmCypR25LZxM0FNEv0ywkvSAy2MEZ2wpqK0,9462
-makelove-0.0.8.dist-info/LICENSE,sha256=Lwuj4j76MsgWouFRi1owmlx53BsXa-5aawQWJNqedPE,1071
-makelove-0.0.8.dist-info/METADATA,sha256=zpuxipI8PhBPmG0Qc0GKjRQgDffXhNiNjnUxQy7M2B4,7156
-makelove-0.0.8.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-makelove-0.0.8.dist-info/entry_points.txt,sha256=DTxWuDSf4ekXBAwiqHBFezsLyVXJtXEoV--ooqtwqzA,53
-makelove-0.0.8.dist-info/top_level.txt,sha256=iBzFUBh1qZydb9IfbeJy4XSel2U3bxbYHJ755naX5gw,9
-makelove-0.0.8.dist-info/RECORD,,
+makelove-0.0.9.dist-info/LICENSE,sha256=Lwuj4j76MsgWouFRi1owmlx53BsXa-5aawQWJNqedPE,1071
+makelove-0.0.9.dist-info/METADATA,sha256=vnrCL04kdpd1nGb7-ShYUqFtD-vN_XEQtohlB5TD8Aw,7156
+makelove-0.0.9.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+makelove-0.0.9.dist-info/entry_points.txt,sha256=DTxWuDSf4ekXBAwiqHBFezsLyVXJtXEoV--ooqtwqzA,53
+makelove-0.0.9.dist-info/top_level.txt,sha256=iBzFUBh1qZydb9IfbeJy4XSel2U3bxbYHJ755naX5gw,9
+makelove-0.0.9.dist-info/RECORD,,
```

