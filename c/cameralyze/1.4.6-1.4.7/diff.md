# Comparing `tmp/cameralyze-1.4.6.tar.gz` & `tmp/cameralyze-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cameralyze-1.4.6.tar", last modified: Tue Apr 18 07:23:58 2023, max compression
+gzip compressed data, was "cameralyze-1.4.7.tar", last modified: Thu May 25 09:45:44 2023, max compression
```

## Comparing `cameralyze-1.4.6.tar` & `cameralyze-1.4.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 ufukdag    (501) staff       (20)        0 2023-04-18 07:23:58.587673 cameralyze-1.4.6/
--rw-r--r--   0 ufukdag    (501) staff       (20)      279 2023-04-18 07:23:58.587498 cameralyze-1.4.6/PKG-INFO
--rw-r--r--   0 ufukdag    (501) staff       (20)      243 2023-03-22 09:58:11.000000 cameralyze-1.4.6/README.md
-drwxr-xr-x   0 ufukdag    (501) staff       (20)        0 2023-04-18 07:23:58.586483 cameralyze-1.4.6/cameralyze/
--rw-r--r--   0 ufukdag    (501) staff       (20)       26 2023-03-22 09:58:11.000000 cameralyze-1.4.6/cameralyze/__init__.py
--rw-r--r--   0 ufukdag    (501) staff       (20)     4473 2023-04-18 07:23:36.000000 cameralyze-1.4.6/cameralyze/model.py
-drwxr-xr-x   0 ufukdag    (501) staff       (20)        0 2023-04-18 07:23:58.587225 cameralyze-1.4.6/cameralyze.egg-info/
--rw-r--r--   0 ufukdag    (501) staff       (20)      279 2023-04-18 07:23:58.000000 cameralyze-1.4.6/cameralyze.egg-info/PKG-INFO
--rw-r--r--   0 ufukdag    (501) staff       (20)      230 2023-04-18 07:23:58.000000 cameralyze-1.4.6/cameralyze.egg-info/SOURCES.txt
--rw-r--r--   0 ufukdag    (501) staff       (20)        1 2023-04-18 07:23:58.000000 cameralyze-1.4.6/cameralyze.egg-info/dependency_links.txt
--rw-r--r--   0 ufukdag    (501) staff       (20)       33 2023-04-18 07:23:58.000000 cameralyze-1.4.6/cameralyze.egg-info/requires.txt
--rw-r--r--   0 ufukdag    (501) staff       (20)       11 2023-04-18 07:23:58.000000 cameralyze-1.4.6/cameralyze.egg-info/top_level.txt
--rw-r--r--   0 ufukdag    (501) staff       (20)       38 2023-04-18 07:23:58.587728 cameralyze-1.4.6/setup.cfg
--rw-r--r--   0 ufukdag    (501) staff       (20)      558 2023-04-18 07:23:46.000000 cameralyze-1.4.6/setup.py
+drwxr-xr-x   0 ufukdag    (501) staff       (20)        0 2023-05-25 09:45:44.015082 cameralyze-1.4.7/
+-rw-r--r--   0 ufukdag    (501) staff       (20)      279 2023-05-25 09:45:44.014899 cameralyze-1.4.7/PKG-INFO
+-rw-r--r--   0 ufukdag    (501) staff       (20)      243 2023-03-22 09:58:11.000000 cameralyze-1.4.7/README.md
+drwxr-xr-x   0 ufukdag    (501) staff       (20)        0 2023-05-25 09:45:44.013963 cameralyze-1.4.7/cameralyze/
+-rw-r--r--   0 ufukdag    (501) staff       (20)       26 2023-03-22 09:58:11.000000 cameralyze-1.4.7/cameralyze/__init__.py
+-rw-r--r--   0 ufukdag    (501) staff       (20)     4057 2023-05-25 09:44:22.000000 cameralyze-1.4.7/cameralyze/model.py
+drwxr-xr-x   0 ufukdag    (501) staff       (20)        0 2023-05-25 09:45:44.014707 cameralyze-1.4.7/cameralyze.egg-info/
+-rw-r--r--   0 ufukdag    (501) staff       (20)      279 2023-05-25 09:45:43.000000 cameralyze-1.4.7/cameralyze.egg-info/PKG-INFO
+-rw-r--r--   0 ufukdag    (501) staff       (20)      230 2023-05-25 09:45:44.000000 cameralyze-1.4.7/cameralyze.egg-info/SOURCES.txt
+-rw-r--r--   0 ufukdag    (501) staff       (20)        1 2023-05-25 09:45:43.000000 cameralyze-1.4.7/cameralyze.egg-info/dependency_links.txt
+-rw-r--r--   0 ufukdag    (501) staff       (20)       33 2023-05-25 09:45:43.000000 cameralyze-1.4.7/cameralyze.egg-info/requires.txt
+-rw-r--r--   0 ufukdag    (501) staff       (20)       11 2023-05-25 09:45:43.000000 cameralyze-1.4.7/cameralyze.egg-info/top_level.txt
+-rw-r--r--   0 ufukdag    (501) staff       (20)       38 2023-05-25 09:45:44.015150 cameralyze-1.4.7/setup.cfg
+-rw-r--r--   0 ufukdag    (501) staff       (20)      558 2023-05-25 09:45:26.000000 cameralyze-1.4.7/setup.py
```

### Comparing `cameralyze-1.4.6/cameralyze/model.py` & `cameralyze-1.4.7/cameralyze/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     def __init__(self, api_key: str = None):
         self.model = None
         self.endpoint = None
         self.background_job = None
         self.flow = None
         self.beautify = False
         self.get_response = True
-        self.base_domain = "https://api.server.cameralyze.co"
+        self.base_domain = "https://run.plugger.ai"
         self.test_temporary_image_domain = "https://tmp.cameralyze.co"
         self.upload_url = "https://platform.api.cameralyze.com/temporary-file/generate"
         self.platform_url = "https://platform.cameralyze.co"
         self.api_key = api_key
         self.configuration = None
         
     def beautify_response(self):
@@ -44,24 +44,15 @@
         """
         Args:
             model (str): Model UUID or model alias name
         """
         self.model = model
         
         return self
-        
-    def set_flow(self, flow: str):
-        """
-        Args:
-            flow (str): Flow UUID or flow alias name
-        """
-        self.flow = flow
-        
-        return self
-        
+                
     def __get_presigned_upload_url(self, file_type: str, file_name: str) -> str:
         return requests.post(self.upload_url, json={"fileType": file_type, "fileName": file_name}).json()["data"]        
 
     def read_file(self, path: str) -> str:
         file_type = filetype.guess(path).mime
         file_name = str(uuid4())
         file = "{file_name}.{file_extension}".format(file_name=file_name, file_extension=path.split(".")[-1])
@@ -94,19 +85,16 @@
                 json["url"] = image
             elif image != None:
                 json["image"] = image
             
         if text != None:
             json["text"] = text
             
-        if self.endpoint:
-            json["applicationUuid"] = self.endpoint
-        
-        if self.background_job:
-            json["applicationUuid"] = self.background_job
+        if self.model:
+            json["itemUuid"] = self.model
         
         if self.configuration != None:
             json["configuration"] = self.configuration
 
         return json
     
     def __get_path(self) -> str:
@@ -119,15 +107,15 @@
         if self.flow:
             return self.flow
         
         return self.model
 
     def predict(self, image: Union[str, tuple] = None, text: str = None, **kwargs: Any) -> dict:
         api_call = requests.post(
-            "{base_domain}/{path}/{unique_id}".format(base_domain=self.base_domain, path=self.__get_path(), unique_id=self.__get_unique_id()),
+            self.base_domain,
             json=self.__get_json(image=image, text=text, **kwargs)
         )
 
         return api_call.json() 
 
     def show_configuration(self):
         print(
```

### Comparing `cameralyze-1.4.6/setup.py` & `cameralyze-1.4.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.4.6' 
+VERSION = '1.4.7' 
 DESCRIPTION = 'Cameralyze No-Code AI Platform'
 LONG_DESCRIPTION = 'Offical Cameralyze No-Code AI Platform package'
 
 setup(
         name="cameralyze", 
         version=VERSION,
         author="Cameralyze Inc",
```

