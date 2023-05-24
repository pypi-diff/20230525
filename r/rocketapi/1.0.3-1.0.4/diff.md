# Comparing `tmp/rocketapi-1.0.3.tar.gz` & `tmp/rocketapi-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rocketapi-1.0.3.tar", last modified: Mon Apr 17 13:29:37 2023, max compression
+gzip compressed data, was "rocketapi-1.0.4.tar", last modified: Wed May 24 22:15:25 2023, max compression
```

## Comparing `rocketapi-1.0.3.tar` & `rocketapi-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 sobolev    (501) staff       (20)        0 2023-04-17 13:29:37.359680 rocketapi-1.0.3/
--rw-r--r--   0 sobolev    (501) staff       (20)      293 2023-04-17 13:29:37.359551 rocketapi-1.0.3/PKG-INFO
--rw-r--r--   0 sobolev    (501) staff       (20)      317 2022-11-20 19:09:53.000000 rocketapi-1.0.3/README.md
--rw-r--r--   0 sobolev    (501) staff       (20)      792 2023-01-03 14:37:32.000000 rocketapi-1.0.3/pyproject.toml
-drwxr-xr-x   0 sobolev    (501) staff       (20)        0 2023-04-17 13:29:37.358811 rocketapi-1.0.3/rocketapi/
--rw-r--r--   0 sobolev    (501) staff       (20)       39 2022-10-08 15:10:45.000000 rocketapi-1.0.3/rocketapi/__init__.py
--rw-r--r--   0 sobolev    (501) staff       (20)       95 2022-10-08 15:05:42.000000 rocketapi-1.0.3/rocketapi/exceptions.py
--rw-r--r--   0 sobolev    (501) staff       (20)    18054 2023-04-17 13:23:07.000000 rocketapi-1.0.3/rocketapi/instagramapi.py
--rw-r--r--   0 sobolev    (501) staff       (20)      759 2023-04-17 13:26:36.000000 rocketapi-1.0.3/rocketapi/rocketapi.py
-drwxr-xr-x   0 sobolev    (501) staff       (20)        0 2023-04-17 13:29:37.359370 rocketapi-1.0.3/rocketapi.egg-info/
--rw-r--r--   0 sobolev    (501) staff       (20)      293 2023-04-17 13:29:37.000000 rocketapi-1.0.3/rocketapi.egg-info/PKG-INFO
--rw-r--r--   0 sobolev    (501) staff       (20)      292 2023-04-17 13:29:37.000000 rocketapi-1.0.3/rocketapi.egg-info/SOURCES.txt
--rw-r--r--   0 sobolev    (501) staff       (20)        1 2023-04-17 13:29:37.000000 rocketapi-1.0.3/rocketapi.egg-info/dependency_links.txt
--rw-r--r--   0 sobolev    (501) staff       (20)        9 2023-04-17 13:29:37.000000 rocketapi-1.0.3/rocketapi.egg-info/requires.txt
--rw-r--r--   0 sobolev    (501) staff       (20)       10 2023-04-17 13:29:37.000000 rocketapi-1.0.3/rocketapi.egg-info/top_level.txt
--rw-r--r--   0 sobolev    (501) staff       (20)       38 2023-04-17 13:29:37.359790 rocketapi-1.0.3/setup.cfg
--rw-r--r--   0 sobolev    (501) staff       (20)      414 2023-04-17 13:24:06.000000 rocketapi-1.0.3/setup.py
+drwxr-xr-x   0 sobolev    (501) staff       (20)        0 2023-05-24 22:15:25.005781 rocketapi-1.0.4/
+-rw-r--r--   0 sobolev    (501) staff       (20)      293 2023-05-24 22:15:25.005649 rocketapi-1.0.4/PKG-INFO
+-rw-r--r--   0 sobolev    (501) staff       (20)      317 2022-11-20 19:09:53.000000 rocketapi-1.0.4/README.md
+-rw-r--r--   0 sobolev    (501) staff       (20)      792 2023-01-03 14:37:32.000000 rocketapi-1.0.4/pyproject.toml
+drwxr-xr-x   0 sobolev    (501) staff       (20)        0 2023-05-24 22:15:25.004673 rocketapi-1.0.4/rocketapi/
+-rw-r--r--   0 sobolev    (501) staff       (20)       39 2022-10-08 15:10:45.000000 rocketapi-1.0.4/rocketapi/__init__.py
+-rw-r--r--   0 sobolev    (501) staff       (20)       95 2022-10-08 15:05:42.000000 rocketapi-1.0.4/rocketapi/exceptions.py
+-rw-r--r--   0 sobolev    (501) staff       (20)    18792 2023-05-24 22:14:25.000000 rocketapi-1.0.4/rocketapi/instagramapi.py
+-rw-r--r--   0 sobolev    (501) staff       (20)      759 2023-04-17 13:26:36.000000 rocketapi-1.0.4/rocketapi/rocketapi.py
+drwxr-xr-x   0 sobolev    (501) staff       (20)        0 2023-05-24 22:15:25.005459 rocketapi-1.0.4/rocketapi.egg-info/
+-rw-r--r--   0 sobolev    (501) staff       (20)      293 2023-05-24 22:15:24.000000 rocketapi-1.0.4/rocketapi.egg-info/PKG-INFO
+-rw-r--r--   0 sobolev    (501) staff       (20)      292 2023-05-24 22:15:24.000000 rocketapi-1.0.4/rocketapi.egg-info/SOURCES.txt
+-rw-r--r--   0 sobolev    (501) staff       (20)        1 2023-05-24 22:15:24.000000 rocketapi-1.0.4/rocketapi.egg-info/dependency_links.txt
+-rw-r--r--   0 sobolev    (501) staff       (20)        9 2023-05-24 22:15:24.000000 rocketapi-1.0.4/rocketapi.egg-info/requires.txt
+-rw-r--r--   0 sobolev    (501) staff       (20)       10 2023-05-24 22:15:24.000000 rocketapi-1.0.4/rocketapi.egg-info/top_level.txt
+-rw-r--r--   0 sobolev    (501) staff       (20)       38 2023-05-24 22:15:25.005898 rocketapi-1.0.4/setup.cfg
+-rw-r--r--   0 sobolev    (501) staff       (20)      414 2023-05-24 22:15:11.000000 rocketapi-1.0.4/setup.py
```

### Comparing `rocketapi-1.0.3/pyproject.toml` & `rocketapi-1.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rocketapi-1.0.3/rocketapi/instagramapi.py` & `rocketapi-1.0.4/rocketapi/instagramapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -453,14 +453,32 @@
         For more information, see documentation: https://docs.rocketapi.io/api/instagram/comment/get_likes
         """
         payload = {"id": comment_id}
         if max_id is not None:
             payload["max_id"] = max_id
         return self.request("instagram/comment/get_likes", payload)
 
+    def get_comment_replies(self, comment_id, media_id, max_id=None):
+        """
+        Retrieve comment replies by comment id and media id.
+
+        Args:
+            comment_id (int): Comment id
+            media_id (int): Media id
+            max_id (str): Use for pagination
+
+        You can use the `max_id` parameter to paginate through replies (take from the `next_max_child_cursor` field of the response).
+
+        For more information, see documentation: https://docs.rocketapi.io/api/instagram/comment/get_replies
+        """
+        payload = {"id": comment_id, "media_id": media_id}
+        if max_id is not None:
+            payload["max_id"] = max_id
+        return self.request("instagram/comment/get_replies", payload)
+
     def get_audio_media(self, audio_id, max_id=None):
         """
         Retrieve audio media by audio id.
 
         Args:
             audio_id (int): Audio id
             max_id (str): Use for pagination
```

### Comparing `rocketapi-1.0.3/rocketapi/rocketapi.py` & `rocketapi-1.0.4/rocketapi/rocketapi.py`

 * *Files identical despite different names*

