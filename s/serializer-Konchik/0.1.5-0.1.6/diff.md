# Comparing `tmp/serializer_Konchik-0.1.5.tar.gz` & `tmp/serializer_Konchik-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serializer_Konchik-0.1.5.tar", last modified: Wed May 24 18:01:30 2023, max compression
+gzip compressed data, was "serializer_Konchik-0.1.6.tar", last modified: Thu May 25 16:34:50 2023, max compression
```

## Comparing `serializer_Konchik-0.1.5.tar` & `serializer_Konchik-0.1.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 18:01:30.512196 serializer_Konchik-0.1.5/
--rw-rw-rw-   0        0        0      262 2023-05-24 18:01:30.512196 serializer_Konchik-0.1.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-24 18:01:30.466194 serializer_Konchik-0.1.5/serializer_Konchik/
--rw-rw-rw-   0        0        0      176 2023-05-22 17:04:23.000000 serializer_Konchik-0.1.5/serializer_Konchik/__init__.py
--rw-rw-rw-   0        0        0     2740 2023-05-24 17:05:42.000000 serializer_Konchik-0.1.5/serializer_Konchik/constants.py
--rw-rw-rw-   0        0        0      116 2023-05-24 17:50:50.000000 serializer_Konchik-0.1.5/serializer_Konchik/is_functions.py
-drwxrwxrwx   0        0        0        0 2023-05-24 18:01:30.488197 serializer_Konchik-0.1.5/serializer_Konchik/packer/
--rw-rw-rw-   0        0        0      110 2023-05-22 17:04:23.000000 serializer_Konchik-0.1.5/serializer_Konchik/packer/__init__.py
--rw-rw-rw-   0        0        0     5479 2023-05-24 17:40:53.000000 serializer_Konchik-0.1.5/serializer_Konchik/packer/packer.py
--rw-rw-rw-   0        0        0     5477 2023-05-24 17:46:20.000000 serializer_Konchik-0.1.5/serializer_Konchik/packer/unpacker.py
-drwxrwxrwx   0        0        0        0 2023-05-24 18:01:30.511210 serializer_Konchik-0.1.5/serializer_Konchik/serializer/
--rw-rw-rw-   0        0        0      226 2023-05-22 17:04:23.000000 serializer_Konchik-0.1.5/serializer_Konchik/serializer/__init__.py
--rw-rw-rw-   0        0        0     1366 2023-05-22 16:01:32.000000 serializer_Konchik-0.1.5/serializer_Konchik/serializer/base_serializer.py
--rw-rw-rw-   0        0        0     3331 2023-05-22 17:04:23.000000 serializer_Konchik-0.1.5/serializer_Konchik/serializer/json_serializer.py
--rw-rw-rw-   0        0        0      732 2023-05-22 17:04:23.000000 serializer_Konchik-0.1.5/serializer_Konchik/serializer/serializer_factory.py
--rw-rw-rw-   0        0        0     3884 2023-05-22 17:04:23.000000 serializer_Konchik-0.1.5/serializer_Konchik/serializer/xml_serializer.py
-drwxrwxrwx   0        0        0        0 2023-05-24 18:01:30.482212 serializer_Konchik-0.1.5/serializer_Konchik.egg-info/
--rw-rw-rw-   0        0        0      262 2023-05-24 18:01:30.000000 serializer_Konchik-0.1.5/serializer_Konchik.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      667 2023-05-24 18:01:30.000000 serializer_Konchik-0.1.5/serializer_Konchik.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 18:01:30.000000 serializer_Konchik-0.1.5/serializer_Konchik.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-24 18:01:30.000000 serializer_Konchik-0.1.5/serializer_Konchik.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-24 18:01:30.000000 serializer_Konchik-0.1.5/serializer_Konchik.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-24 18:01:30.512196 serializer_Konchik-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      595 2023-05-24 17:59:35.000000 serializer_Konchik-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 16:34:50.509846 serializer_Konchik-0.1.6/
+-rw-rw-rw-   0        0        0      262 2023-05-25 16:34:50.509846 serializer_Konchik-0.1.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-25 16:34:50.448479 serializer_Konchik-0.1.6/serializer_Konchik/
+-rw-rw-rw-   0        0        0      175 2023-05-25 15:46:08.000000 serializer_Konchik-0.1.6/serializer_Konchik/__init__.py
+-rw-rw-rw-   0        0        0     2740 2023-05-24 17:05:42.000000 serializer_Konchik-0.1.6/serializer_Konchik/constants.py
+-rw-rw-rw-   0        0        0      116 2023-05-24 17:50:50.000000 serializer_Konchik-0.1.6/serializer_Konchik/is_functions.py
+drwxrwxrwx   0        0        0        0 2023-05-25 16:34:50.480267 serializer_Konchik-0.1.6/serializer_Konchik/packer/
+-rw-rw-rw-   0        0        0      110 2023-05-22 17:04:23.000000 serializer_Konchik-0.1.6/serializer_Konchik/packer/__init__.py
+-rw-rw-rw-   0        0        0     5529 2023-05-25 15:29:21.000000 serializer_Konchik-0.1.6/serializer_Konchik/packer/packer.py
+-rw-rw-rw-   0        0        0     5477 2023-05-24 17:46:20.000000 serializer_Konchik-0.1.6/serializer_Konchik/packer/unpacker.py
+drwxrwxrwx   0        0        0        0 2023-05-25 16:34:50.508865 serializer_Konchik-0.1.6/serializer_Konchik/serializer/
+-rw-rw-rw-   0        0        0      225 2023-05-25 15:46:08.000000 serializer_Konchik-0.1.6/serializer_Konchik/serializer/__init__.py
+-rw-rw-rw-   0        0        0     1366 2023-05-22 16:01:32.000000 serializer_Konchik-0.1.6/serializer_Konchik/serializer/base_serializer.py
+-rw-rw-rw-   0        0        0     3330 2023-05-25 15:46:08.000000 serializer_Konchik-0.1.6/serializer_Konchik/serializer/json_serializer.py
+-rw-rw-rw-   0        0        0      728 2023-05-25 15:46:08.000000 serializer_Konchik-0.1.6/serializer_Konchik/serializer/serializer_factory.py
+-rw-rw-rw-   0        0        0     3884 2023-05-22 17:04:23.000000 serializer_Konchik-0.1.6/serializer_Konchik/serializer/xml_serializer.py
+drwxrwxrwx   0        0        0        0 2023-05-25 16:34:50.468396 serializer_Konchik-0.1.6/serializer_Konchik.egg-info/
+-rw-rw-rw-   0        0        0      262 2023-05-25 16:34:50.000000 serializer_Konchik-0.1.6/serializer_Konchik.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      667 2023-05-25 16:34:50.000000 serializer_Konchik-0.1.6/serializer_Konchik.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 16:34:50.000000 serializer_Konchik-0.1.6/serializer_Konchik.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-25 16:34:50.000000 serializer_Konchik-0.1.6/serializer_Konchik.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-25 16:34:50.000000 serializer_Konchik-0.1.6/serializer_Konchik.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-25 16:34:50.509846 serializer_Konchik-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      595 2023-05-25 16:34:14.000000 serializer_Konchik-0.1.6/setup.py
```

### Comparing `serializer_Konchik-0.1.5/serializer_Konchik/constants.py` & `serializer_Konchik-0.1.6/serializer_Konchik/constants.py`

 * *Files identical despite different names*

### Comparing `serializer_Konchik-0.1.5/serializer_Konchik/packer/packer.py` & `serializer_Konchik-0.1.6/serializer_Konchik/packer/packer.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
         Returns:
         dictionary.
         """
 
         if isinstance(obj, PRIMITIVES):
             return {TYPE: type(obj).__name__,
-                    VALUE: obj}
+                    VALUE: str(obj) if isinstance(obj, complex) else obj}
 
         if isinstance(obj, COLLECTIONS):
             if isinstance(obj, dict):
                 return {TYPE: type(obj).__name__,
                         VALUE: [[Packer.pack(key), Packer.pack(value)]
                                 for key, value in obj.items()]}
             else:
@@ -68,15 +68,15 @@
 
         if inspect.ismethod(obj):
             return {TYPE: type(obj).__name__,
                     VALUE: Packer._pack_function(obj.__func__)}
 
         return {TYPE: "object",
                 VALUE: {"__class__": Packer.pack(obj.__class__),
-                        "__vars__": {key: Packer.pack(value) for key, value in vars(obj)}}}
+                        "__vars__": {key: Packer.pack(value) for key, value in vars(obj).items()}}}
 
     @staticmethod
     def _pack_function(obj: FunctionType, cls=None):
 
         return {"__name__": obj.__name__,
                 "__globals__": Packer._pack_globals(obj, cls),
                 "__closure__": Packer.pack(obj.__closure__),
```

### Comparing `serializer_Konchik-0.1.5/serializer_Konchik/packer/unpacker.py` & `serializer_Konchik-0.1.6/serializer_Konchik/packer/unpacker.py`

 * *Files identical despite different names*

### Comparing `serializer_Konchik-0.1.5/serializer_Konchik/serializer/base_serializer.py` & `serializer_Konchik-0.1.6/serializer_Konchik/serializer/base_serializer.py`

 * *Files identical despite different names*

### Comparing `serializer_Konchik-0.1.5/serializer_Konchik/serializer/json_serializer.py` & `serializer_Konchik-0.1.6/serializer_Konchik/serializer/json_serializer.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from serializer_Konchik.serializer.base_serializer import BaseSerializer
 from serializer_Konchik.packer import Packer, Unpacker
 from ..constants import (PRIMITIVES,
                          JsonRegularExpression as Expression)
 import regex
 
 
-class JsonSerializer(BaseSerializer):
+class XmlSerializer(BaseSerializer):
 
     def dumps(self, obj: Any) -> str:
         """
         Convert an object to string of 'JSON' format.
 
         :param obj: Any python object.
         :type obj: Any
```

### Comparing `serializer_Konchik-0.1.5/serializer_Konchik/serializer/serializer_factory.py` & `serializer_Konchik-0.1.6/serializer_Konchik/serializer/serializer_factory.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from serializer_Konchik.serializer.json_serializer import JsonSerializer
+from serializer_Konchik.serializer.json_serializer import XmlSerializer
 from serializer_Konchik.serializer.xml_serializer import XmlSerializer
 from ..constants import JSON, XML
 
 
 class SerializerFactory:
 
     @staticmethod
-    def create(name: str) -> JsonSerializer | XmlSerializer:
+    def create(name: str) -> XmlSerializer | XmlSerializer:
         """
         Create serializer.
 
         :param name: Serializer name.
         :type name: str
 
         :return: Serializer.
-        :rtype: JsonSerializer | XmlSerializer
+        :rtype: XmlSerializer | XmlSerializer
         """
 
         name = name.lower().strip()
 
         if name == JSON:
-            return JsonSerializer()
+            return XmlSerializer()
         elif name == XML:
             return XmlSerializer()
         else:
             raise NameError('Invalid serializer name')
```

### Comparing `serializer_Konchik-0.1.5/serializer_Konchik/serializer/xml_serializer.py` & `serializer_Konchik-0.1.6/serializer_Konchik/serializer/xml_serializer.py`

 * *Files identical despite different names*

### Comparing `serializer_Konchik-0.1.5/serializer_Konchik.egg-info/SOURCES.txt` & `serializer_Konchik-0.1.6/serializer_Konchik.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `serializer_Konchik-0.1.5/setup.py` & `serializer_Konchik-0.1.6/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Always prefer setuptools over distutils
 from setuptools import setup
 
 # This call to setup() does all the work
 setup(
     name="serializer_Konchik",
-    version="0.1.5",
+    version="0.1.6",
     description="JSON / XML serializer",
     author="Denis Konchik",
     author_email="denis.pptx@gmail.com",
     license="MIT",
     classifiers=[
         "Programming Language :: Python",
         "Operating System :: OS Independent"
```

