# Comparing `tmp/pysqueezebox-0.6.1.tar.gz` & `tmp/pysqueezebox-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysqueezebox-0.6.1.tar", last modified: Sat Oct 29 15:40:51 2022, max compression
+gzip compressed data, was "pysqueezebox-0.6.2.tar", last modified: Thu May 25 21:48:54 2023, max compression
```

## Comparing `pysqueezebox-0.6.1.tar` & `pysqueezebox-0.6.2.tar`

### file list

```diff
@@ -1,18 +1,25 @@
-drwxr-xr-x   0 rajlaud    (501) staff       (20)        0 2022-10-29 15:40:51.131906 pysqueezebox-0.6.1/
--rw-r--r--   0 rajlaud    (501) staff       (20)    11338 2021-03-13 06:31:24.000000 pysqueezebox-0.6.1/LICENSE
--rw-r--r--   0 rajlaud    (501) staff       (20)     2572 2022-10-29 15:40:51.132038 pysqueezebox-0.6.1/PKG-INFO
--rw-r--r--   0 rajlaud    (501) staff       (20)     2226 2021-03-13 06:31:24.000000 pysqueezebox-0.6.1/README.md
-drwxr-xr-x   0 rajlaud    (501) staff       (20)        0 2022-10-29 15:40:51.129670 pysqueezebox-0.6.1/pysqueezebox/
--rw-r--r--   0 rajlaud    (501) staff       (20)      981 2021-03-13 06:31:24.000000 pysqueezebox-0.6.1/pysqueezebox/__init__.py
--rw-r--r--   0 rajlaud    (501) staff       (20)      151 2021-03-13 06:31:24.000000 pysqueezebox-0.6.1/pysqueezebox/const.py
--rw-r--r--   0 rajlaud    (501) staff       (20)     3652 2021-03-13 06:31:24.000000 pysqueezebox-0.6.1/pysqueezebox/discovery.py
--rw-r--r--   0 rajlaud    (501) staff       (20)    23408 2022-10-29 14:21:46.000000 pysqueezebox-0.6.1/pysqueezebox/player.py
--rw-r--r--   0 rajlaud    (501) staff       (20)    13353 2022-10-29 15:37:13.000000 pysqueezebox-0.6.1/pysqueezebox/server.py
-drwxr-xr-x   0 rajlaud    (501) staff       (20)        0 2022-10-29 15:40:51.131572 pysqueezebox-0.6.1/pysqueezebox.egg-info/
--rw-r--r--   0 rajlaud    (501) staff       (20)     2572 2022-10-29 15:40:51.000000 pysqueezebox-0.6.1/pysqueezebox.egg-info/PKG-INFO
--rw-r--r--   0 rajlaud    (501) staff       (20)      334 2022-10-29 15:40:51.000000 pysqueezebox-0.6.1/pysqueezebox.egg-info/SOURCES.txt
--rw-r--r--   0 rajlaud    (501) staff       (20)        1 2022-10-29 15:40:51.000000 pysqueezebox-0.6.1/pysqueezebox.egg-info/dependency_links.txt
--rw-r--r--   0 rajlaud    (501) staff       (20)        8 2022-10-29 15:40:51.000000 pysqueezebox-0.6.1/pysqueezebox.egg-info/requires.txt
--rw-r--r--   0 rajlaud    (501) staff       (20)       13 2022-10-29 15:40:51.000000 pysqueezebox-0.6.1/pysqueezebox.egg-info/top_level.txt
--rw-r--r--   0 rajlaud    (501) staff       (20)      131 2022-10-29 15:40:51.132586 pysqueezebox-0.6.1/setup.cfg
--rw-r--r--   0 rajlaud    (501) staff       (20)      555 2022-10-29 15:36:38.000000 pysqueezebox-0.6.1/setup.py
+drwxr-xr-x   0 rajlaud    (501) staff       (20)        0 2023-05-25 21:48:54.016906 pysqueezebox-0.6.2/
+-rw-r--r--   0 rajlaud    (501) staff       (20)    11338 2023-05-25 20:54:54.000000 pysqueezebox-0.6.2/LICENSE
+-rw-r--r--   0 rajlaud    (501) staff       (20)     2552 2023-05-25 21:48:54.017194 pysqueezebox-0.6.2/PKG-INFO
+-rw-r--r--   0 rajlaud    (501) staff       (20)     2226 2023-05-25 20:54:54.000000 pysqueezebox-0.6.2/README.md
+drwxr-xr-x   0 rajlaud    (501) staff       (20)        0 2023-05-25 21:48:54.009246 pysqueezebox-0.6.2/pysqueezebox/
+-rw-r--r--   0 rajlaud    (501) staff       (20)      981 2023-05-25 20:54:54.000000 pysqueezebox-0.6.2/pysqueezebox/__init__.py
+-rw-r--r--   0 rajlaud    (501) staff       (20)      151 2023-05-25 20:54:54.000000 pysqueezebox-0.6.2/pysqueezebox/const.py
+-rw-r--r--   0 rajlaud    (501) staff       (20)     3652 2023-05-25 20:54:54.000000 pysqueezebox-0.6.2/pysqueezebox/discovery.py
+-rw-r--r--   0 rajlaud    (501) staff       (20)    23556 2023-05-25 21:25:21.000000 pysqueezebox-0.6.2/pysqueezebox/player.py
+-rw-r--r--   0 rajlaud    (501) staff       (20)    13353 2023-05-25 20:54:54.000000 pysqueezebox-0.6.2/pysqueezebox/server.py
+drwxr-xr-x   0 rajlaud    (501) staff       (20)        0 2023-05-25 21:48:54.011841 pysqueezebox-0.6.2/pysqueezebox.egg-info/
+-rw-r--r--   0 rajlaud    (501) staff       (20)     2552 2023-05-25 21:48:53.000000 pysqueezebox-0.6.2/pysqueezebox.egg-info/PKG-INFO
+-rw-r--r--   0 rajlaud    (501) staff       (20)      462 2023-05-25 21:48:53.000000 pysqueezebox-0.6.2/pysqueezebox.egg-info/SOURCES.txt
+-rw-r--r--   0 rajlaud    (501) staff       (20)        1 2023-05-25 21:48:53.000000 pysqueezebox-0.6.2/pysqueezebox.egg-info/dependency_links.txt
+-rw-r--r--   0 rajlaud    (501) staff       (20)       22 2023-05-25 21:48:53.000000 pysqueezebox-0.6.2/pysqueezebox.egg-info/requires.txt
+-rw-r--r--   0 rajlaud    (501) staff       (20)       19 2023-05-25 21:48:53.000000 pysqueezebox-0.6.2/pysqueezebox.egg-info/top_level.txt
+-rw-r--r--   0 rajlaud    (501) staff       (20)      131 2023-05-25 21:48:54.018183 pysqueezebox-0.6.2/setup.cfg
+-rw-r--r--   0 rajlaud    (501) staff       (20)      572 2023-05-25 21:47:05.000000 pysqueezebox-0.6.2/setup.py
+drwxr-xr-x   0 rajlaud    (501) staff       (20)        0 2023-05-25 21:48:54.016167 pysqueezebox-0.6.2/tests/
+-rw-r--r--   0 rajlaud    (501) staff       (20)        0 2023-05-25 21:31:11.000000 pysqueezebox-0.6.2/tests/__init__.py
+-rw-r--r--   0 rajlaud    (501) staff       (20)     1520 2023-05-25 20:54:54.000000 pysqueezebox-0.6.2/tests/conftest.py
+-rw-r--r--   0 rajlaud    (501) staff       (20)     1693 2023-05-25 21:37:01.000000 pysqueezebox-0.6.2/tests/test_discovery.py
+-rw-r--r--   0 rajlaud    (501) staff       (20)    18297 2023-05-25 20:54:54.000000 pysqueezebox-0.6.2/tests/test_integration.py
+-rw-r--r--   0 rajlaud    (501) staff       (20)     1987 2023-05-25 20:54:54.000000 pysqueezebox-0.6.2/tests/test_player.py
+-rw-r--r--   0 rajlaud    (501) staff       (20)     1639 2023-05-25 20:54:54.000000 pysqueezebox-0.6.2/tests/test_server.py
```

### Comparing `pysqueezebox-0.6.1/LICENSE` & `pysqueezebox-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pysqueezebox-0.6.1/PKG-INFO` & `pysqueezebox-0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pysqueezebox
-Version: 0.6.1
+Version: 0.6.2
 Summary: Asynchronous library to control Logitech Media Server
 Home-page: https://github.com/rajlaud/pysqueezebox
 Author: Raj Laud
 Author-email: raj.laud@gmail.com
 License: apache-2.0
-Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pysqueezebox - Asynchronous control of squeezeboxes
 This a library to control a Logitech Media Server asynchronously, intended for
 integration with Home Assistant.
@@ -66,9 +65,7 @@
 This allows you to retrieve the player's properties without any I/O. Remember
 to call Player.async_update() prior to retrieving properties if you want the
 most up-to-date information.
 
 ## Player() class
 Most of the useful functions are in the Player class. More documentation to
 follow, but in the meantime, the docstrings should be instructive.
-
-
```

### Comparing `pysqueezebox-0.6.1/README.md` & `pysqueezebox-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `pysqueezebox-0.6.1/pysqueezebox/__init__.py` & `pysqueezebox-0.6.2/pysqueezebox/__init__.py`

 * *Files identical despite different names*

### Comparing `pysqueezebox-0.6.1/pysqueezebox/discovery.py` & `pysqueezebox-0.6.2/pysqueezebox/discovery.py`

 * *Files identical despite different names*

### Comparing `pysqueezebox-0.6.1/pysqueezebox/player.py` & `pysqueezebox-0.6.2/pysqueezebox/player.py`

 * *Files 1% similar despite different names*

```diff
@@ -373,15 +373,19 @@
                 response.pop("playlist_loop", None)
         else:
             # no current playlist
             self._status.update({"playlist_loop": None})
 
         # preserve the playlist between updates
         self._status = {"playlist_loop": self._status.get("playlist_loop")}
-        self._status.update(response)
+        try:
+            self._status.update(response)
+        except TypeError:
+            _LOGGER.debug("Error updating status - empty response from server")
+            return False
 
         # check if any property futures have been satisfied
         property_futures = []
         interval = None
         for property_future in self._property_futures:
             if not property_future["future"].done():
                 if property_future["test"](getattr(self, property_future["prop"])):
```

### Comparing `pysqueezebox-0.6.1/pysqueezebox/server.py` & `pysqueezebox-0.6.2/pysqueezebox/server.py`

 * *Files identical despite different names*

### Comparing `pysqueezebox-0.6.1/pysqueezebox.egg-info/PKG-INFO` & `pysqueezebox-0.6.2/pysqueezebox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pysqueezebox
-Version: 0.6.1
+Version: 0.6.2
 Summary: Asynchronous library to control Logitech Media Server
 Home-page: https://github.com/rajlaud/pysqueezebox
 Author: Raj Laud
 Author-email: raj.laud@gmail.com
 License: apache-2.0
-Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pysqueezebox - Asynchronous control of squeezeboxes
 This a library to control a Logitech Media Server asynchronously, intended for
 integration with Home Assistant.
@@ -66,9 +65,7 @@
 This allows you to retrieve the player's properties without any I/O. Remember
 to call Player.async_update() prior to retrieving properties if you want the
 most up-to-date information.
 
 ## Player() class
 Most of the useful functions are in the Player class. More documentation to
 follow, but in the meantime, the docstrings should be instructive.
-
-
```

### Comparing `pysqueezebox-0.6.1/setup.py` & `pysqueezebox-0.6.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import setuptools
 
 with open("README.md") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pysqueezebox",
-    version="0.6.1",
+    version="0.6.2",
     license="apache-2.0",
     author="Raj Laud",
     author_email="raj.laud@gmail.com",
     description="Asynchronous library to control Logitech Media Server",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rajlaud/pysqueezebox",
     packages=setuptools.find_packages(),
     python_requires=">=3.6",
-    install_requires=["aiohttp"],
+    install_requires=["aiohttp", "async-timeout"],
 )
```

