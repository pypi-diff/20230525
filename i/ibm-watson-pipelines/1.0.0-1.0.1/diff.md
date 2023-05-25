# Comparing `tmp/ibm-watson-pipelines-1.0.0.tar.gz` & `tmp/ibm-watson-pipelines-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibm-watson-pipelines-1.0.0.tar", last modified: Thu Dec  1 08:16:01 2022, max compression
+gzip compressed data, was "/home/travis/build/AILifecycle/ibm-watson-pipelines/dist/.tmp-v1vp30ez/ibm-watson-pipelines-1.0.1.tar", last modified: Thu May 25 15:33:06 2023, max compression
```

## Comparing `ibm-watson-pipelines-1.0.0.tar` & `ibm-watson-pipelines-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 merazmus   (501) staff       (20)        0 2022-12-01 08:16:01.401739 ibm-watson-pipelines-1.0.0/
--rw-r--r--   0 merazmus   (501) staff       (20)    11358 2022-12-01 08:12:41.000000 ibm-watson-pipelines-1.0.0/LICENSE
--rw-r--r--   0 merazmus   (501) staff       (20)     8382 2022-12-01 08:16:01.401493 ibm-watson-pipelines-1.0.0/PKG-INFO
--rw-r--r--   0 merazmus   (501) staff       (20)     7826 2022-12-01 08:12:41.000000 ibm-watson-pipelines-1.0.0/README.md
-drwxr-xr-x   0 merazmus   (501) staff       (20)        0 2022-12-01 08:16:01.400244 ibm-watson-pipelines-1.0.0/ibm_watson_pipelines/
--rw-r--r--   0 merazmus   (501) staff       (20)      610 2022-12-01 08:12:41.000000 ibm-watson-pipelines-1.0.0/ibm_watson_pipelines/__init__.py
--rw-r--r--   0 merazmus   (501) staff       (20)    40454 2022-12-01 08:12:41.000000 ibm-watson-pipelines-1.0.0/ibm_watson_pipelines/client.py
--rw-r--r--   0 merazmus   (501) staff       (20)     8643 2022-12-01 08:12:41.000000 ibm-watson-pipelines-1.0.0/ibm_watson_pipelines/client_errors.py
--rw-r--r--   0 merazmus   (501) staff       (20)    26342 2022-12-01 08:12:41.000000 ibm-watson-pipelines-1.0.0/ibm_watson_pipelines/cpd_paths.py
--rw-r--r--   0 merazmus   (501) staff       (20)     7158 2022-12-01 08:12:41.000000 ibm-watson-pipelines-1.0.0/ibm_watson_pipelines/utils.py
--rw-r--r--   0 merazmus   (501) staff       (20)      327 2022-12-01 08:12:41.000000 ibm-watson-pipelines-1.0.0/ibm_watson_pipelines/version.py
-drwxr-xr-x   0 merazmus   (501) staff       (20)        0 2022-12-01 08:16:01.400919 ibm-watson-pipelines-1.0.0/ibm_watson_pipelines.egg-info/
--rw-r--r--   0 merazmus   (501) staff       (20)     8382 2022-12-01 08:16:01.000000 ibm-watson-pipelines-1.0.0/ibm_watson_pipelines.egg-info/PKG-INFO
--rw-r--r--   0 merazmus   (501) staff       (20)      531 2022-12-01 08:16:01.000000 ibm-watson-pipelines-1.0.0/ibm_watson_pipelines.egg-info/SOURCES.txt
--rw-r--r--   0 merazmus   (501) staff       (20)        1 2022-12-01 08:16:01.000000 ibm-watson-pipelines-1.0.0/ibm_watson_pipelines.egg-info/dependency_links.txt
--rw-r--r--   0 merazmus   (501) staff       (20)      147 2022-12-01 08:16:01.000000 ibm-watson-pipelines-1.0.0/ibm_watson_pipelines.egg-info/requires.txt
--rw-r--r--   0 merazmus   (501) staff       (20)       21 2022-12-01 08:16:01.000000 ibm-watson-pipelines-1.0.0/ibm_watson_pipelines.egg-info/top_level.txt
--rw-r--r--   0 merazmus   (501) staff       (20)       38 2022-12-01 08:16:01.401781 ibm-watson-pipelines-1.0.0/setup.cfg
--rw-r--r--   0 merazmus   (501) staff       (20)     1120 2022-12-01 08:14:51.000000 ibm-watson-pipelines-1.0.0/setup.py
-drwxr-xr-x   0 merazmus   (501) staff       (20)        0 2022-12-01 08:16:01.401320 ibm-watson-pipelines-1.0.0/test/
--rw-r--r--   0 merazmus   (501) staff       (20)     9595 2022-12-01 08:12:41.000000 ibm-watson-pipelines-1.0.0/test/test_cpd_path_methods.py
--rw-r--r--   0 merazmus   (501) staff       (20)     8871 2022-12-01 08:12:41.000000 ibm-watson-pipelines-1.0.0/test/test_cpd_path_parsing.py
--rw-r--r--   0 merazmus   (501) staff       (20)     3207 2022-12-01 08:12:41.000000 ibm-watson-pipelines-1.0.0/test/test_storage_client.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-25 15:33:06.925584 ibm-watson-pipelines-1.0.1/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11358 2023-05-25 15:32:18.000000 ibm-watson-pipelines-1.0.1/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8382 2023-05-25 15:33:06.925584 ibm-watson-pipelines-1.0.1/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7826 2023-05-25 15:32:18.000000 ibm-watson-pipelines-1.0.1/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-25 15:33:06.921584 ibm-watson-pipelines-1.0.1/ibm_watson_pipelines/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      610 2023-05-25 15:32:18.000000 ibm-watson-pipelines-1.0.1/ibm_watson_pipelines/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    40454 2023-05-25 15:32:18.000000 ibm-watson-pipelines-1.0.1/ibm_watson_pipelines/client.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8643 2023-05-25 15:32:18.000000 ibm-watson-pipelines-1.0.1/ibm_watson_pipelines/client_errors.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26558 2023-05-25 15:32:18.000000 ibm-watson-pipelines-1.0.1/ibm_watson_pipelines/cpd_paths.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7158 2023-05-25 15:32:18.000000 ibm-watson-pipelines-1.0.1/ibm_watson_pipelines/utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      327 2023-05-25 15:32:18.000000 ibm-watson-pipelines-1.0.1/ibm_watson_pipelines/version.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-25 15:33:06.921584 ibm-watson-pipelines-1.0.1/ibm_watson_pipelines.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8382 2023-05-25 15:33:06.000000 ibm-watson-pipelines-1.0.1/ibm_watson_pipelines.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      531 2023-05-25 15:33:06.000000 ibm-watson-pipelines-1.0.1/ibm_watson_pipelines.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-05-25 15:33:06.000000 ibm-watson-pipelines-1.0.1/ibm_watson_pipelines.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      147 2023-05-25 15:33:06.000000 ibm-watson-pipelines-1.0.1/ibm_watson_pipelines.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       21 2023-05-25 15:33:06.000000 ibm-watson-pipelines-1.0.1/ibm_watson_pipelines.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2023-05-25 15:33:06.925584 ibm-watson-pipelines-1.0.1/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1120 2023-05-25 15:32:18.000000 ibm-watson-pipelines-1.0.1/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-25 15:33:06.925584 ibm-watson-pipelines-1.0.1/test/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9595 2023-05-25 15:32:18.000000 ibm-watson-pipelines-1.0.1/test/test_cpd_path_methods.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9071 2023-05-25 15:32:18.000000 ibm-watson-pipelines-1.0.1/test/test_cpd_path_parsing.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3207 2023-05-25 15:32:18.000000 ibm-watson-pipelines-1.0.1/test/test_storage_client.py
```

### Comparing `ibm-watson-pipelines-1.0.0/LICENSE` & `ibm-watson-pipelines-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ibm-watson-pipelines-1.0.0/PKG-INFO` & `ibm-watson-pipelines-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibm-watson-pipelines
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python utilities for IBM Watson Pipelines
 Home-page: https://www.ibm.com/docs/en/cloud-paks/cp-data/4.6.x?topic=functions-watson-pipelines
 Author: Rafał Bigaj, Maksymilian Erazmus
 Author-email: rafal.bigaj@pl.ibm.com, maksymilian.erazmus1@pl.ibm.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ibm-watson-pipelines-1.0.0/README.md` & `ibm-watson-pipelines-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `ibm-watson-pipelines-1.0.0/ibm_watson_pipelines/__init__.py` & `ibm-watson-pipelines-1.0.1/ibm_watson_pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-pipelines-1.0.0/ibm_watson_pipelines/client.py` & `ibm-watson-pipelines-1.0.1/ibm_watson_pipelines/client.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-pipelines-1.0.0/ibm_watson_pipelines/client_errors.py` & `ibm-watson-pipelines-1.0.1/ibm_watson_pipelines/client_errors.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-pipelines-1.0.0/ibm_watson_pipelines/cpd_paths.py` & `ibm-watson-pipelines-1.0.1/ibm_watson_pipelines/cpd_paths.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,14 +186,15 @@
     def from_asset_type(cls: Type[Self], asset_type: str) -> Self:
         return {
             m.to_asset_type: m for m in cls.__member__
         }[asset_type]
 
 class SpecialSegmentsType(Enum):
     FILES = "files"
+    MNTS = "mnts"
 
 _ST = TypeVar('_ST', ScopeType, Union[ResourceType, SpecialAssetsType])
 
 @attr.attrs(auto_attribs=True, frozen=True, kw_only=True)
 class Segment(Generic[_ST]):
     type: _ST
     id: Optional[str] = None
@@ -235,15 +236,15 @@
     ) -> Tuple[Optional[Segment], Sequence[str]]:
         assert len(segments) > 0
 
         scope: Optional[Segment] = None
 
         # absolute paths start from "/", so the first segment is empty
         res_idx = 0
-        if segments[0] == "":
+        if segments[0] == "" and (len(segments) > 1 and segments[1] != SpecialSegmentsType.MNTS.value):
             assert len(segments) > 1
             el = segments[1]
             if ScopeType.is_member(el):
                 scope = Segment(type=ScopeType.from_string(el))
             else:
                 raise TypeError(f"Invalid CPD scope type: {segments[1]}")
 
@@ -270,14 +271,16 @@
 
         resource: Optional[Segment] = None
         file: Optional[File] = None
 
         # files/...
         if ns > 1 and segments[0] == SpecialSegmentsType.FILES.value:
             file = File(path="/".join(segments[1:]))
+        elif ns > 1 and segments[1] == SpecialSegmentsType.MNTS.value:
+            file = File(path="/".join(segments[0:]))
         # asset-123
         else:
             if ns == 1 and not has_query:
                 el = segments[0]
                 if has_scope:
                     # cannot: /spaces/abc/asset-123
                     if ResourceType.is_member(el) or SpecialAssetsType.is_member(el):
```

### Comparing `ibm-watson-pipelines-1.0.0/ibm_watson_pipelines/utils.py` & `ibm-watson-pipelines-1.0.1/ibm_watson_pipelines/utils.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-pipelines-1.0.0/ibm_watson_pipelines.egg-info/PKG-INFO` & `ibm-watson-pipelines-1.0.1/ibm_watson_pipelines.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibm-watson-pipelines
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python utilities for IBM Watson Pipelines
 Home-page: https://www.ibm.com/docs/en/cloud-paks/cp-data/4.6.x?topic=functions-watson-pipelines
 Author: Rafał Bigaj, Maksymilian Erazmus
 Author-email: rafal.bigaj@pl.ibm.com, maksymilian.erazmus1@pl.ibm.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ibm-watson-pipelines-1.0.0/ibm_watson_pipelines.egg-info/SOURCES.txt` & `ibm-watson-pipelines-1.0.1/ibm_watson_pipelines.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ibm-watson-pipelines-1.0.0/setup.py` & `ibm-watson-pipelines-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ibm-watson-pipelines",
-    version="1.0.0",
+    version="1.0.1",
     author="Rafał Bigaj, Maksymilian Erazmus",
     author_email="rafal.bigaj@pl.ibm.com, maksymilian.erazmus1@pl.ibm.com",
     description="Python utilities for IBM Watson Pipelines",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.ibm.com/docs/en/cloud-paks/cp-data/4.6.x?topic=functions-watson-pipelines",
     packages=setuptools.find_packages(),
```

### Comparing `ibm-watson-pipelines-1.0.0/test/test_cpd_path_methods.py` & `ibm-watson-pipelines-1.0.1/test/test_cpd_path_methods.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-pipelines-1.0.0/test/test_cpd_path_parsing.py` & `ibm-watson-pipelines-1.0.1/test/test_cpd_path_parsing.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,7 +223,16 @@
         "cpd:///projects/4b4946f4-242e-4ed0-9c80-24ae9b48db19/files/def%ghi",
         "cpd:///projects/4b4946f4-242e-4ed0-9c80-24ae9b48db19/files/def%%ghi",
         "cpd:///projects/4b4946f4-242e-4ed0-9c80-24ae9b48db19/files/def%20%ghi",
     ]
     for path in paths:
         with pytest.raises(TypeError):
             CpdPath.from_string(path)
+
+
+def test_07_mounted_file_path():
+    paths = [
+        "/mnts/files/dir/file_name.txt"
+    ]
+    for path in paths:
+        cpd_path = CpdPath.from_string(path)
+        assert str(cpd_path) == path
```

### Comparing `ibm-watson-pipelines-1.0.0/test/test_storage_client.py` & `ibm-watson-pipelines-1.0.1/test/test_storage_client.py`

 * *Files identical despite different names*

