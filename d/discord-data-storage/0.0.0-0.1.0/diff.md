# Comparing `tmp/discord_data_storage-0.0.0.tar.gz` & `tmp/discord_data_storage-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord_data_storage-0.0.0.tar", last modified: Sat Apr  8 22:49:34 2023, max compression
+gzip compressed data, was "discord_data_storage-0.1.0.tar", last modified: Thu May 25 04:39:09 2023, max compression
```

## Comparing `discord_data_storage-0.0.0.tar` & `discord_data_storage-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2023-04-08 22:49:34.596199 discord_data_storage-0.0.0/
--rw-rw-r--   0 joshua    (1000) joshua    (1000)      202 2023-04-08 22:49:34.596199 discord_data_storage-0.0.0/PKG-INFO
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     3472 2023-04-08 21:46:51.000000 discord_data_storage-0.0.0/README.md
-drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2023-04-08 22:49:34.596199 discord_data_storage-0.0.0/discord_data_storage/
--rw-rw-r--   0 joshua    (1000) joshua    (1000)       47 2023-04-08 21:49:13.000000 discord_data_storage-0.0.0/discord_data_storage/__init__.py
--rw-rw-r--   0 joshua    (1000) joshua    (1000)     7075 2023-04-08 21:46:47.000000 discord_data_storage-0.0.0/discord_data_storage/discord_data_storage.py
-drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2023-04-08 22:49:34.596199 discord_data_storage-0.0.0/discord_data_storage.egg-info/
--rw-rw-r--   0 joshua    (1000) joshua    (1000)      202 2023-04-08 22:49:34.000000 discord_data_storage-0.0.0/discord_data_storage.egg-info/PKG-INFO
--rw-rw-r--   0 joshua    (1000) joshua    (1000)      315 2023-04-08 22:49:34.000000 discord_data_storage-0.0.0/discord_data_storage.egg-info/SOURCES.txt
--rw-rw-r--   0 joshua    (1000) joshua    (1000)        1 2023-04-08 22:49:34.000000 discord_data_storage-0.0.0/discord_data_storage.egg-info/dependency_links.txt
--rw-rw-r--   0 joshua    (1000) joshua    (1000)       13 2023-04-08 22:49:34.000000 discord_data_storage-0.0.0/discord_data_storage.egg-info/requires.txt
--rw-rw-r--   0 joshua    (1000) joshua    (1000)       21 2023-04-08 22:49:34.000000 discord_data_storage-0.0.0/discord_data_storage.egg-info/top_level.txt
--rw-rw-r--   0 joshua    (1000) joshua    (1000)       38 2023-04-08 22:49:34.596199 discord_data_storage-0.0.0/setup.cfg
--rw-rw-r--   0 joshua    (1000) joshua    (1000)      329 2023-01-15 06:00:45.000000 discord_data_storage-0.0.0/setup.py
+drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2023-05-25 04:39:09.168362 discord_data_storage-0.1.0/
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     1065 2023-05-25 04:24:24.000000 discord_data_storage-0.1.0/LICENSE
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     4018 2023-05-25 04:39:09.168362 discord_data_storage-0.1.0/PKG-INFO
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     3753 2023-05-25 04:21:28.000000 discord_data_storage-0.1.0/README.md
+drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2023-05-25 04:39:09.164362 discord_data_storage-0.1.0/discord_data_storage/
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)       47 2023-04-08 21:49:13.000000 discord_data_storage-0.1.0/discord_data_storage/__init__.py
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     7566 2023-05-25 04:21:47.000000 discord_data_storage-0.1.0/discord_data_storage/discord_data_storage.py
+drwxrwxr-x   0 joshua    (1000) joshua    (1000)        0 2023-05-25 04:39:09.168362 discord_data_storage-0.1.0/discord_data_storage.egg-info/
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)     4018 2023-05-25 04:39:09.000000 discord_data_storage-0.1.0/discord_data_storage.egg-info/PKG-INFO
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)      323 2023-05-25 04:39:09.000000 discord_data_storage-0.1.0/discord_data_storage.egg-info/SOURCES.txt
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)        1 2023-05-25 04:39:09.000000 discord_data_storage-0.1.0/discord_data_storage.egg-info/dependency_links.txt
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)       13 2023-05-25 04:39:09.000000 discord_data_storage-0.1.0/discord_data_storage.egg-info/requires.txt
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)       21 2023-05-25 04:39:09.000000 discord_data_storage-0.1.0/discord_data_storage.egg-info/top_level.txt
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)       38 2023-05-25 04:39:09.168362 discord_data_storage-0.1.0/setup.cfg
+-rw-rw-r--   0 joshua    (1000) joshua    (1000)      518 2023-05-25 04:38:10.000000 discord_data_storage-0.1.0/setup.py
```

### Comparing `discord_data_storage-0.0.0/README.md` & `discord_data_storage-0.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -31,14 +31,20 @@
 `discord_data_storage.DataAccessor.write(data, server_id="", user_id="")` <br />
 Writes the data to the given parameters. <br />
 **Parameters:** <br />
 data - the data to write <br />
 server_id - the server id of the data to write <br />
 user_id - the user id of the data to write <br />
  <br />
+`discord_data_storage.DataAccessor.delete(server_id="", user_id="")` <br />
+Deletes the data matching the given parameters if it exists. <br />
+**Parameters:** <br />
+server_id - the server id of the data to delete <br />
+user_id - the user id of the data to delete <br />
+ <br />
 `discord_data_storage.DataAccessor.data_exists(server_id="", user_id="")` <br />
 Checks if data exists for the given parameters. <br />
 **Parameters:** <br />
 server_id - the server id of the data to check <br />
 user_id - the user id of the data to check <br />
 **Returns:** <br />
 True if the data exists, False if not <br />
```

### Comparing `discord_data_storage-0.0.0/discord_data_storage/discord_data_storage.py` & `discord_data_storage-0.1.0/discord_data_storage/discord_data_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,28 @@
 
         Optional keyword arguments:
         server_id - the server id of the data to write
         user_id - the user id of the data to write
         """
         self._write_file(json.dumps(data), server_id, user_id)
 
+    def delete(self, server_id="", user_id=""):
+        """Deletes data
+
+        Deletes the data if it exists, does nothing if it doesn't.
+        Optional keyword arguments:
+        server_id - the server id of the data to delete
+        user_id - the user id of the data to delete
+        """
+        if self.data_exists(server_id=server_id, user_id=user_id):
+            os.remove(self._get_file_path(
+                server_id=server_id,
+                user_id=user_id
+            ))
+
     def data_exists(self,  server_id="", user_id=""):
         """Checks if data exists
 
         Optional keyword arguments:
         server_id - the server id of the data to check
         user_id - the user id of the data to check
```

