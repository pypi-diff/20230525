# Comparing `tmp/pypendency-0.3.0.tar.gz` & `tmp/pypendency-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pypendency-0.3.0.tar", last modified: Tue Apr 18 15:56:01 2023, max compression
+gzip compressed data, was "dist/pypendency-0.4.0.tar", last modified: Thu May 25 07:25:02 2023, max compression
```

## Comparing `pypendency-0.3.0.tar` & `pypendency-0.4.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:56:01.000000 pypendency-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-04-18 15:56:01.000000 pypendency-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-04-18 15:55:47.000000 pypendency-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 15:56:01.000000 pypendency-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-18 15:55:47.000000 pypendency-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:56:01.000000 pypendency-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:56:01.000000 pypendency-0.3.0/src/pypendency/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:55:47.000000 pypendency-0.3.0/src/pypendency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-18 15:55:47.000000 pypendency-0.3.0/src/pypendency/argument.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-18 15:55:47.000000 pypendency-0.3.0/src/pypendency/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-04-18 15:55:47.000000 pypendency-0.3.0/src/pypendency/container.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-18 15:55:47.000000 pypendency-0.3.0/src/pypendency/definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-04-18 15:55:47.000000 pypendency-0.3.0/src/pypendency/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:56:01.000000 pypendency-0.3.0/src/pypendency/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:55:47.000000 pypendency-0.3.0/src/pypendency/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-18 15:55:47.000000 pypendency-0.3.0/src/pypendency/loaders/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-18 15:55:47.000000 pypendency-0.3.0/src/pypendency/loaders/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-04-18 15:55:47.000000 pypendency-0.3.0/src/pypendency/loaders/py_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-18 15:55:47.000000 pypendency-0.3.0/src/pypendency/loaders/yaml_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-18 15:55:47.000000 pypendency-0.3.0/src/pypendency/tag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:56:01.000000 pypendency-0.3.0/src/pypendency/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:55:47.000000 pypendency-0.3.0/src/pypendency/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-18 15:55:47.000000 pypendency-0.3.0/src/pypendency/types/python_loadable_module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:56:01.000000 pypendency-0.3.0/src/pypendency.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-04-18 15:56:00.000000 pypendency-0.3.0/src/pypendency.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-18 15:56:01.000000 pypendency-0.3.0/src/pypendency.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 15:56:00.000000 pypendency-0.3.0/src/pypendency.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 15:56:00.000000 pypendency-0.3.0/src/pypendency.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-18 15:56:00.000000 pypendency-0.3.0/src/pypendency.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:25:02.000000 pypendency-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-05-25 07:25:02.000000 pypendency-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-05-25 07:24:49.000000 pypendency-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 07:25:02.000000 pypendency-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-25 07:24:49.000000 pypendency-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:25:02.000000 pypendency-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:25:02.000000 pypendency-0.4.0/src/pypendency/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:24:49.000000 pypendency-0.4.0/src/pypendency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-25 07:24:49.000000 pypendency-0.4.0/src/pypendency/argument.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-25 07:24:49.000000 pypendency-0.4.0/src/pypendency/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-05-25 07:24:49.000000 pypendency-0.4.0/src/pypendency/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-25 07:24:49.000000 pypendency-0.4.0/src/pypendency/definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-25 07:24:49.000000 pypendency-0.4.0/src/pypendency/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:25:02.000000 pypendency-0.4.0/src/pypendency/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:24:49.000000 pypendency-0.4.0/src/pypendency/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-25 07:24:49.000000 pypendency-0.4.0/src/pypendency/loaders/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-25 07:24:49.000000 pypendency-0.4.0/src/pypendency/loaders/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-05-25 07:24:49.000000 pypendency-0.4.0/src/pypendency/loaders/py_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-25 07:24:49.000000 pypendency-0.4.0/src/pypendency/loaders/yaml_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-25 07:24:49.000000 pypendency-0.4.0/src/pypendency/on_container_resolved_callable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-25 07:24:49.000000 pypendency-0.4.0/src/pypendency/tag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:25:02.000000 pypendency-0.4.0/src/pypendency/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:24:49.000000 pypendency-0.4.0/src/pypendency/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-25 07:24:49.000000 pypendency-0.4.0/src/pypendency/types/python_loadable_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:25:02.000000 pypendency-0.4.0/src/pypendency.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-05-25 07:25:02.000000 pypendency-0.4.0/src/pypendency.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-25 07:25:02.000000 pypendency-0.4.0/src/pypendency.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 07:25:02.000000 pypendency-0.4.0/src/pypendency.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-25 07:25:02.000000 pypendency-0.4.0/src/pypendency.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-25 07:25:02.000000 pypendency-0.4.0/src/pypendency.egg-info/top_level.txt
```

### Comparing `pypendency-0.3.0/PKG-INFO` & `pypendency-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypendency
-Version: 0.3.0
+Version: 0.4.0
 Summary: A dependency injection tool for python
 Home-page: https://github.com/Feverup/pypendency
 Author: Fever - Platform Squad
 Author-email: platform@feverup.com
 License: MIT License
 Description: # Pypendency
         Pypendency is a dependency injection library for python >=3.7.
```

### Comparing `pypendency-0.3.0/README.md` & `pypendency-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pypendency-0.3.0/setup.py` & `pypendency-0.4.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open('README.md', 'r') as readme:
     README = readme.read()
 
 
 setup(
     name='pypendency',
-    version='0.3.0',
+    version='0.4.0',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     author='Fever - Platform Squad',
     author_email='platform@feverup.com',
     description='A dependency injection tool for python',
     long_description=README,
     long_description_content_type='text/markdown',
```

### Comparing `pypendency-0.3.0/src/pypendency/builder.py` & `pypendency-0.4.0/src/pypendency/builder.py`

 * *Files identical despite different names*

### Comparing `pypendency-0.3.0/src/pypendency/container.py` & `pypendency-0.4.0/src/pypendency/container.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from abc import ABC, abstractmethod
 from pydoc import locate
-from typing import Any, Dict, List, Optional, Union, Set, Tuple
+from typing import Any, Dict, List, Optional, Union, Set
 
 from pypendency import exceptions
 from pypendency.argument import Argument
 from pypendency.definition import Definition
+from pypendency.on_container_resolved_callable import OnContainerResolvedCallable
 from pypendency.tag import Tag
 
 
 class AbstractContainer(ABC):
     @abstractmethod
     def set(self, identifier: str, service: object) -> None: pass
 
@@ -18,40 +19,52 @@
     @abstractmethod
     def has(self, identifier: str) -> bool: pass
 
 
 class Container(AbstractContainer):
     def __init__(self, definitions: List[Definition]):
         self._resolved = False
+        self._on_resolved_callbacks: Set[OnContainerResolvedCallable] = set()
         self._service_mapping: Dict[str, Union[None, object, Definition]] = {
             definition.identifier: definition
             for definition in definitions
         }
         self._tags_mapping: Dict[Tag, List[str]] = {}
 
     def resolve(self) -> None:
         if self.is_resolved():
             raise exceptions.ContainerAlreadyResolved()
 
         self.__populate_tags_map()
         self._resolved = True
+        self.__perform_on_resolved_callbacks()
 
     def is_resolved(self) -> bool:
         return self._resolved
 
     def __populate_tags_map(self) -> None:
         for service in self._service_mapping.values():
             if not isinstance(service, Definition):
                 continue
             for tag in service.tags:
                 self.__add_service_to_tag_group(tag, service.identifier)
 
     def __add_service_to_tag_group(self, tag: Tag, service_identifier: str) -> None:
         self._tags_mapping.setdefault(tag, set()).add(service_identifier)
 
+    def __perform_on_resolved_callbacks(self) -> None:
+        for on_resolved_callback in self._on_resolved_callbacks:
+            try:
+                on_resolved_callback()
+            except Exception as e:
+                raise exceptions.PypendencyCallbackException() from e
+
+    def add_on_resolved_callback(self, func: OnContainerResolvedCallable) -> None:
+        self._on_resolved_callbacks.add(func)
+
     def set(self, identifier: str, service: object, tags: Optional[Set[Tag]] = None) -> None:
         if self.is_resolved():
             raise exceptions.ForbiddenChangeOnResolvedContainer()
 
         if self.has(identifier):
             raise exceptions.ServiceAlreadyDefined(identifier)
```

### Comparing `pypendency-0.3.0/src/pypendency/exceptions.py` & `pypendency-0.4.0/src/pypendency/exceptions.py`

 * *Files 19% similar despite different names*

```diff
@@ -30,18 +30,21 @@
 class ServiceNotFoundFromFullyQualifiedName(Exception):
     def __init__(self, fully_qualified_name: str):
         self.fully_qualified_name = fully_qualified_name
         super().__init__(
             f"Container can't locate any class in {fully_qualified_name}"
         )
 
-
 class ServiceInstantiationFailed(Exception):
     def __init__(self, service_fqn: str) -> None:
         self.service_fqn = service_fqn
         super().__init__(f"Type {service_fqn} cannot be instantiated by the container")
 
 
 class TagNotFoundInContainer(Exception):
     def __init__(self, tag_identifier: str) -> None:
         self.tag_identifier = tag_identifier
         super().__init__(f"The tag '{tag_identifier}' does not exist in the container")
+
+class PypendencyCallbackException(Exception):
+    def __init__(self) -> None:
+        super().__init__(f"Exception on_resolved_callback")
```

### Comparing `pypendency-0.3.0/src/pypendency/loaders/exceptions.py` & `pypendency-0.4.0/src/pypendency/loaders/exceptions.py`

 * *Files identical despite different names*

### Comparing `pypendency-0.3.0/src/pypendency/loaders/py_loader.py` & `pypendency-0.4.0/src/pypendency/loaders/py_loader.py`

 * *Files identical despite different names*

### Comparing `pypendency-0.3.0/src/pypendency/loaders/yaml_loader.py` & `pypendency-0.4.0/src/pypendency/loaders/yaml_loader.py`

 * *Files identical despite different names*

### Comparing `pypendency-0.3.0/src/pypendency.egg-info/PKG-INFO` & `pypendency-0.4.0/src/pypendency.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypendency
-Version: 0.3.0
+Version: 0.4.0
 Summary: A dependency injection tool for python
 Home-page: https://github.com/Feverup/pypendency
 Author: Fever - Platform Squad
 Author-email: platform@feverup.com
 License: MIT License
 Description: # Pypendency
         Pypendency is a dependency injection library for python >=3.7.
```

### Comparing `pypendency-0.3.0/src/pypendency.egg-info/SOURCES.txt` & `pypendency-0.4.0/src/pypendency.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 setup.py
 src/pypendency/__init__.py
 src/pypendency/argument.py
 src/pypendency/builder.py
 src/pypendency/container.py
 src/pypendency/definition.py
 src/pypendency/exceptions.py
+src/pypendency/on_container_resolved_callable.py
 src/pypendency/tag.py
 src/pypendency.egg-info/PKG-INFO
 src/pypendency.egg-info/SOURCES.txt
 src/pypendency.egg-info/dependency_links.txt
 src/pypendency.egg-info/requires.txt
 src/pypendency.egg-info/top_level.txt
 src/pypendency/loaders/__init__.py
```

