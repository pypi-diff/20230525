# Comparing `tmp/mia_api-0.0.3.tar.gz` & `tmp/mia_api-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mia_api-0.0.3.tar", last modified: Wed May 24 17:04:38 2023, max compression
+gzip compressed data, was "mia_api-0.0.4.tar", last modified: Thu May 25 20:22:36 2023, max compression
```

## Comparing `mia_api-0.0.3.tar` & `mia_api-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 gilly     (1000) gilly     (1000)        0 2023-05-24 17:04:38.336645 mia_api-0.0.3/
--rw-rw-r--   0 gilly     (1000) gilly     (1000)     1700 2023-05-24 17:04:38.336645 mia_api-0.0.3/PKG-INFO
--rwxrwxrwx   0 gilly     (1000) gilly     (1000)     1308 2023-05-24 17:02:44.000000 mia_api-0.0.3/README.md
--rwxrwxrwx   0 gilly     (1000) gilly     (1000)       85 2022-07-29 12:38:50.000000 mia_api-0.0.3/pyproject.toml
--rwxrwxrwx   0 gilly     (1000) gilly     (1000)      561 2023-05-24 17:04:38.336645 mia_api-0.0.3/setup.cfg
--rwxrwxrwx   0 gilly     (1000) gilly     (1000)      741 2023-05-24 16:58:46.000000 mia_api-0.0.3/setup.py
-drwxrwxr-x   0 gilly     (1000) gilly     (1000)        0 2023-05-24 17:04:38.336645 mia_api-0.0.3/src/
-drwxrwxr-x   0 gilly     (1000) gilly     (1000)        0 2023-05-24 17:04:38.336645 mia_api-0.0.3/src/mia_api/
--rwxrwxrwx   0 gilly     (1000) gilly     (1000)      115 2023-05-24 16:59:58.000000 mia_api-0.0.3/src/mia_api/__init__.py
--rwxrwxrwx   0 gilly     (1000) gilly     (1000)       40 2023-05-24 16:59:58.000000 mia_api-0.0.3/src/mia_api/config_file.py
--rwxrwxrwx   0 gilly     (1000) gilly     (1000)     1749 2023-05-24 16:59:58.000000 mia_api-0.0.3/src/mia_api/connect.py
--rwxrwxrwx   0 gilly     (1000) gilly     (1000)      982 2023-05-24 16:59:58.000000 mia_api-0.0.3/src/mia_api/juice.py
--rwxrwxrwx   0 gilly     (1000) gilly     (1000)    12792 2023-05-24 16:59:58.000000 mia_api-0.0.3/src/mia_api/models.py
--rwxrwxrwx   0 gilly     (1000) gilly     (1000)      374 2023-05-24 16:59:58.000000 mia_api-0.0.3/src/mia_api/utils.py
-drwxrwxr-x   0 gilly     (1000) gilly     (1000)        0 2023-05-24 17:04:38.336645 mia_api-0.0.3/src/mia_api.egg-info/
--rwxrwxrwx   0 gilly     (1000) gilly     (1000)     1700 2023-05-24 17:04:38.000000 mia_api-0.0.3/src/mia_api.egg-info/PKG-INFO
--rwxrwxrwx   0 gilly     (1000) gilly     (1000)      355 2023-05-24 17:04:38.000000 mia_api-0.0.3/src/mia_api.egg-info/SOURCES.txt
--rwxrwxrwx   0 gilly     (1000) gilly     (1000)        1 2023-05-24 17:04:38.000000 mia_api-0.0.3/src/mia_api.egg-info/dependency_links.txt
--rw-rw-r--   0 gilly     (1000) gilly     (1000)       53 2023-05-24 17:04:38.000000 mia_api-0.0.3/src/mia_api.egg-info/requires.txt
--rwxrwxrwx   0 gilly     (1000) gilly     (1000)        8 2023-05-24 17:04:38.000000 mia_api-0.0.3/src/mia_api.egg-info/top_level.txt
+drwxrwxr-x   0 gilly     (1000) gilly     (1000)        0 2023-05-25 20:22:36.000646 mia_api-0.0.4/
+-rw-rw-r--   0 gilly     (1000) gilly     (1000)     1700 2023-05-25 20:22:36.000646 mia_api-0.0.4/PKG-INFO
+-rwxrwxrwx   0 gilly     (1000) gilly     (1000)     1308 2023-05-24 17:02:44.000000 mia_api-0.0.4/README.md
+-rwxrwxrwx   0 gilly     (1000) gilly     (1000)       85 2022-07-29 12:38:50.000000 mia_api-0.0.4/pyproject.toml
+-rwxrwxrwx   0 gilly     (1000) gilly     (1000)      561 2023-05-25 20:22:36.000646 mia_api-0.0.4/setup.cfg
+-rwxrwxrwx   0 gilly     (1000) gilly     (1000)      741 2023-05-25 20:20:59.000000 mia_api-0.0.4/setup.py
+drwxrwxr-x   0 gilly     (1000) gilly     (1000)        0 2023-05-25 20:22:36.000646 mia_api-0.0.4/src/
+drwxrwxr-x   0 gilly     (1000) gilly     (1000)        0 2023-05-25 20:22:36.000646 mia_api-0.0.4/src/mia_api/
+-rwxrwxrwx   0 gilly     (1000) gilly     (1000)      115 2023-05-25 20:21:49.000000 mia_api-0.0.4/src/mia_api/__init__.py
+-rwxrwxrwx   0 gilly     (1000) gilly     (1000)       40 2023-05-25 20:21:49.000000 mia_api-0.0.4/src/mia_api/config_file.py
+-rwxrwxrwx   0 gilly     (1000) gilly     (1000)     1749 2023-05-25 20:21:49.000000 mia_api-0.0.4/src/mia_api/connect.py
+-rwxrwxrwx   0 gilly     (1000) gilly     (1000)      982 2023-05-25 20:21:49.000000 mia_api-0.0.4/src/mia_api/juice.py
+-rwxrwxrwx   0 gilly     (1000) gilly     (1000)    13328 2023-05-25 20:21:49.000000 mia_api-0.0.4/src/mia_api/models.py
+-rwxrwxrwx   0 gilly     (1000) gilly     (1000)      374 2023-05-25 20:21:49.000000 mia_api-0.0.4/src/mia_api/utils.py
+drwxrwxr-x   0 gilly     (1000) gilly     (1000)        0 2023-05-25 20:22:36.000646 mia_api-0.0.4/src/mia_api.egg-info/
+-rwxrwxrwx   0 gilly     (1000) gilly     (1000)     1700 2023-05-25 20:22:36.000000 mia_api-0.0.4/src/mia_api.egg-info/PKG-INFO
+-rwxrwxrwx   0 gilly     (1000) gilly     (1000)      355 2023-05-25 20:22:36.000000 mia_api-0.0.4/src/mia_api.egg-info/SOURCES.txt
+-rwxrwxrwx   0 gilly     (1000) gilly     (1000)        1 2023-05-25 20:22:36.000000 mia_api-0.0.4/src/mia_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 gilly     (1000) gilly     (1000)       53 2023-05-25 20:22:36.000000 mia_api-0.0.4/src/mia_api.egg-info/requires.txt
+-rwxrwxrwx   0 gilly     (1000) gilly     (1000)        8 2023-05-25 20:22:36.000000 mia_api-0.0.4/src/mia_api.egg-info/top_level.txt
```

### Comparing `mia_api-0.0.3/PKG-INFO` & `mia_api-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mia_api
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package to communicate with MIA API
 Home-page: https://github.com/meteoia-team/mia_api
 Author: MeteoIA
 Author-email: meteoia.consult@meteoia.com
 Project-URL: Bug Tracker, https://github.com/meteoia-team/mia_api/issues
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
```

### Comparing `mia_api-0.0.3/README.md` & `mia_api-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `mia_api-0.0.3/setup.cfg` & `mia_api-0.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mia_api
-version = 0.0.1
+version = 0.0.4
 author = MeteoIA
 author_email = meteoia.consult@meteoia.com
 description = A package to communicate with MIA API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/meteoia-team/mia_api
 project_urls =
```

### Comparing `mia_api-0.0.3/setup.py` & `mia_api-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name='mia_api',
-  version='0.0.3',
+  version='0.0.4',
   author='MeteoIA',
   author_email='meteoia.consult@meteoia.com',
   description='A package to communicate with MIA API',
   long_description=long_description,
   long_description_content_type="text/markdown",
   url='https://github.com/meteoia-team/mia_api',
   project_urls = {
```

### Comparing `mia_api-0.0.3/src/mia_api/connect.py` & `mia_api-0.0.4/src/mia_api/connect.py`

 * *Files identical despite different names*

### Comparing `mia_api-0.0.3/src/mia_api/juice.py` & `mia_api-0.0.4/src/mia_api/juice.py`

 * *Files identical despite different names*

### Comparing `mia_api-0.0.3/src/mia_api/models.py` & `mia_api-0.0.4/src/mia_api/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -188,14 +188,31 @@
             [pd.DataFrame.from_dict(m, orient="index") for m in menu]
         )
         print('#' * 40)
         print(tabulate(data, tablefmt="psql"))
         print(f'JuiceBar total juices/fruits: ' + str(data.shape[0]))
         print('#' * 40)
 
+    def list_juices(
+            self):
+        """
+        Show list of Juices names within JuiceBar
+
+        :return: List[dict] with Juices names within a JuiceBar
+
+        """
+        listjuicepath = f"{APIPATH}/bars/juices/list/?barname={self.name}"
+        headers = {
+            'accept': 'application/json',
+            'Authorization': 'Bearer ' + os.getenv("MIA_API_TOKEN")
+        }
+        response = requests.request("GET", listjuicepath, headers=headers)
+        response_return(response)
+        return response.json()
+
     def get_juice(
             self,
             juice_name: str):
         """
         Retrieve a Juice within this JuiceBar, its methods can be seen
         in class MIAJuice
```

### Comparing `mia_api-0.0.3/src/mia_api.egg-info/PKG-INFO` & `mia_api-0.0.4/src/mia_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mia-api
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package to communicate with MIA API
 Home-page: https://github.com/meteoia-team/mia_api
 Author: MeteoIA
 Author-email: meteoia.consult@meteoia.com
 Project-URL: Bug Tracker, https://github.com/meteoia-team/mia_api/issues
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
```

