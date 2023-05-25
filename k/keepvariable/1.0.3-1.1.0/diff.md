# Comparing `tmp/keepvariable-1.0.3.tar.gz` & `tmp/keepvariable-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keepvariable-1.0.3.tar", last modified: Fri Apr 21 21:41:37 2023, max compression
+gzip compressed data, was "keepvariable-1.1.0.tar", last modified: Thu May 25 15:04:02 2023, max compression
```

## Comparing `keepvariable-1.0.3.tar` & `keepvariable-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 21:41:37.069442 keepvariable-1.0.3/
--rw-rw-rw-   0        0        0     1247 2021-03-10 00:11:59.000000 keepvariable-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     2146 2023-04-21 21:41:37.068445 keepvariable-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1593 2023-04-10 03:42:53.000000 keepvariable-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 21:41:37.035533 keepvariable-1.0.3/keepvariable/
--rw-rw-rw-   0        0        0        0 2021-03-10 00:11:59.000000 keepvariable-1.0.3/keepvariable/__init__.py
--rw-rw-rw-   0        0        0     7789 2023-04-21 21:40:36.000000 keepvariable-1.0.3/keepvariable/keepvariable_core.py
--rw-rw-rw-   0        0        0      295 2021-03-10 00:11:59.000000 keepvariable-1.0.3/keepvariable/keepvariable_model.py
--rw-rw-rw-   0        0        0     1017 2023-04-21 21:27:03.000000 keepvariable-1.0.3/keepvariable/kv_redis_example.py
-drwxrwxrwx   0        0        0        0 2023-04-21 21:41:37.067448 keepvariable-1.0.3/keepvariable.egg-info/
--rw-rw-rw-   0        0        0     2146 2023-04-21 21:41:36.000000 keepvariable-1.0.3/keepvariable.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      332 2023-04-21 21:41:36.000000 keepvariable-1.0.3/keepvariable.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 21:41:36.000000 keepvariable-1.0.3/keepvariable.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-21 21:41:36.000000 keepvariable-1.0.3/keepvariable.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-21 21:41:36.000000 keepvariable-1.0.3/keepvariable.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 21:41:37.069442 keepvariable-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      800 2023-04-21 21:41:32.000000 keepvariable-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 15:04:02.235746 keepvariable-1.1.0/
+-rw-rw-rw-   0        0        0     1247 2021-03-10 00:11:59.000000 keepvariable-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     2146 2023-05-25 15:04:02.234749 keepvariable-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1593 2023-04-10 03:42:53.000000 keepvariable-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 15:04:02.211811 keepvariable-1.1.0/keepvariable/
+-rw-rw-rw-   0        0        0        0 2021-03-10 00:11:59.000000 keepvariable-1.1.0/keepvariable/__init__.py
+-rw-rw-rw-   0        0        0     9285 2023-05-25 15:03:40.000000 keepvariable-1.1.0/keepvariable/keepvariable_core.py
+-rw-rw-rw-   0        0        0      295 2021-03-10 00:11:59.000000 keepvariable-1.1.0/keepvariable/keepvariable_model.py
+-rw-rw-rw-   0        0        0     1684 2023-05-25 15:03:40.000000 keepvariable-1.1.0/keepvariable/kv_redis_example.py
+drwxrwxrwx   0        0        0        0 2023-05-25 15:04:02.233751 keepvariable-1.1.0/keepvariable.egg-info/
+-rw-rw-rw-   0        0        0     2146 2023-05-25 15:04:01.000000 keepvariable-1.1.0/keepvariable.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      332 2023-05-25 15:04:02.000000 keepvariable-1.1.0/keepvariable.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 15:04:01.000000 keepvariable-1.1.0/keepvariable.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-25 15:04:01.000000 keepvariable-1.1.0/keepvariable.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-25 15:04:01.000000 keepvariable-1.1.0/keepvariable.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-25 15:04:02.235746 keepvariable-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      800 2023-05-25 15:03:58.000000 keepvariable-1.1.0/setup.py
```

### Comparing `keepvariable-1.0.3/LICENSE` & `keepvariable-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `keepvariable-1.0.3/PKG-INFO` & `keepvariable-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keepvariable
-Version: 1.0.3
+Version: 1.1.0
 Summary: A Python package keeping the values of variables between separate runs in a seamless and effortless way.
 Home-page: https://github.com/DovaX/keepvariable
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keepvariable-1.0.3/README.md` & `keepvariable-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `keepvariable-1.0.3/keepvariable/keepvariable_core.py` & `keepvariable-1.1.0/keepvariable/keepvariable_core.py`

 * *Files 13% similar despite different names*

```diff
@@ -131,15 +131,22 @@
    
     
 class KeepVariableDummyRedisServer:
     def __init__(self,host="localhost"):
         self.host=host
         self.storage={}
         
-    def parse_saved_value(self,value):
+    def parse_saved_value(self, value, additional_params: dict = {}):
+        """Parses enterted value to json format. Certain special type values are serialized (DFs, datetimes, functions, classes).
+
+        Args:
+            value (Any): Entered value of any type (not all types can get serialized and stored however!)
+            additional_params (dict, optional): Additional parameters used for serialization, e.g. for a function variable it's 
+            code must be passed somehow --> additional_params = {'code': <function_code>}. Defaults to {}.
+        """        
         if isinstance(value,list) or isinstance(value,bool) or isinstance(value,dict):
             value=json.dumps(value)
         elif isinstance(value,pd.DataFrame):
             data=value.values.tolist()
             columns=list(value.columns)
             final_data={"columns":columns,"data":data,"object_type":"pd.DataFrame"}
             print(final_data)
@@ -148,36 +155,56 @@
             data=value.tolist()
             final_data={"data":data,"object_type":"np.ndarray"}
             value=json.dumps(final_data)
         elif isinstance(value, datetime.datetime):
             data=value.strftime("%Y-%m-%d %H:%M:%S")
             final_data = {"data": data, "object_type": "datetime.datetime"}
             value = json.dumps(final_data)
+        elif inspect.isfunction(value):
+            code = additional_params.get("code")
+            value = {"code": code, "object_type": "function"}
+            value = json.dumps(code)
+        elif inspect.isclass(value):
+            code = additional_params.get("code")
+            value = {"code": code, "object_type": "class"}
+            value = json.dumps(code)
+            
         return(value)
     
     def decode_loaded_value(self,value):
+        """Decodes value stored in redis into it's initial value.
+        For functions and classes only their code is returned --> they need to be evaluated afterwards!!!
+
+        Args:
+            value (Any): Variable value from redis
+
+        Returns:
+            Any: Parsed variable value
+        """        
         try:
             value=json.loads(value)
             if "object_type" in value and isinstance(value,dict):
                 if value["object_type"]=="pd.DataFrame":
                     df=pd.DataFrame(value["data"],columns=value["columns"])
                     return(df)
                 elif value["object_type"]=="np.ndarray":
                     array=pd.DataFrame(value["data"]).values #to ensure 64bit values in array
                     return(array)
                 elif value["object_type"] == "datetime.datetime":
                     datetime_value = datetime.datetime.strptime(value["data"],"%Y-%m-%d %H:%M:%S")
                     return datetime_value
+                elif value["object_type"] == "function" or value["object_type"] == "class":
+                    return value["code"]
             return(value)
         except json.JSONDecodeError: #if type is str, it fails to decode
             return(value)
         
         
-    def set(self,key,value):
-        value=self.parse_saved_value(value)
+    def set(self, key, value, additional_params: dict = {}):
+        value=self.parse_saved_value(value, additional_params)
         self.storage[key]=value
         return({key:value})
 
     def get(self,key):
         value=self.storage.get(key)
         decoded_value=self.decode_loaded_value(value)
         return(decoded_value)
@@ -194,16 +221,16 @@
     def kept_variables(self):
         return(self._kept_variables)
     
     @kept_variables.setter
     def kept_variables(self,kept_variables):
         return(self._kept_variables)
     
-    def set(self,key,value):
-        value=self.parse_saved_value(value)
+    def set(self,key,value, additional_params: dict = {}):
+        value=self.parse_saved_value(value, additional_params)
         result=self.redis.set(key,value)
         return(result)
         
     def get(self,key):
         value=self.redis.get(key)
         decoded_value=self.decode_loaded_value(value)
         return(decoded_value)
```

### Comparing `keepvariable-1.0.3/keepvariable.egg-info/PKG-INFO` & `keepvariable-1.1.0/keepvariable.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keepvariable
-Version: 1.0.3
+Version: 1.1.0
 Summary: A Python package keeping the values of variables between separate runs in a seamless and effortless way.
 Home-page: https://github.com/DovaX/keepvariable
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keepvariable-1.0.3/setup.py` & `keepvariable-1.1.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
     
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name='keepvariable',
-    version='1.0.3',
+    version='1.1.0',
     author='DovaX',
     author_email='dovax.ai@gmail.com',
     description='A Python package keeping the values of variables between separate runs in a seamless and effortless way.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/DovaX/keepvariable',
     packages=setuptools.find_packages(),
```

