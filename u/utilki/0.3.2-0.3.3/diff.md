# Comparing `tmp/utilki-0.3.2.tar.gz` & `tmp/utilki-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utilki-0.3.2.tar", max compression
+gzip compressed data, was "utilki-0.3.3.tar", max compression
```

## Comparing `utilki-0.3.2.tar` & `utilki-0.3.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1064 2023-04-07 14:14:58.660919 utilki-0.3.2/README.md
--rw-r--r--   0        0        0      525 2023-05-23 18:17:31.462863 utilki-0.3.2/pyproject.toml
--rw-r--r--   0        0        0       73 2023-04-06 19:12:02.029197 utilki-0.3.2/utilki/__init__.py
--rw-r--r--   0        0        0     2184 2023-04-28 13:17:26.918133 utilki-0.3.2/utilki/cli.py
--rw-r--r--   0        0        0     5734 2023-05-23 18:17:06.950808 utilki-0.3.2/utilki/task_mixin.py
--rw-r--r--   0        0        0     1846 2023-05-23 18:17:48.106181 utilki-0.3.2/setup.py
--rw-r--r--   0        0        0     1608 2023-05-23 18:17:48.106435 utilki-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-07 14:14:58.660919 utilki-0.3.3/README.md
+-rw-r--r--   0        0        0      525 2023-05-25 19:22:26.189250 utilki-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0       73 2023-04-06 19:12:02.029197 utilki-0.3.3/utilki/__init__.py
+-rw-r--r--   0        0        0     2184 2023-04-28 13:17:26.918133 utilki-0.3.3/utilki/cli.py
+-rw-r--r--   0        0        0     6503 2023-05-25 19:16:01.896303 utilki-0.3.3/utilki/task_mixin.py
+-rw-r--r--   0        0        0     1846 2023-05-25 19:22:33.847695 utilki-0.3.3/setup.py
+-rw-r--r--   0        0        0     1608 2023-05-25 19:22:33.847862 utilki-0.3.3/PKG-INFO
```

### Comparing `utilki-0.3.2/README.md` & `utilki-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `utilki-0.3.2/pyproject.toml` & `utilki-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "utilki"
-version = "0.3.2"
+version = "0.3.3"
 description = "A collection of useful utilities"
 readme = "README.md"
 authors = ["Khaidar Bikmaev <khaidar@bikmaev.com>"]
 
 [tool.poetry.dependencies]
 python = ">=3.7"
 click = "^8.1.3"
```

### Comparing `utilki-0.3.2/utilki/cli.py` & `utilki-0.3.3/utilki/cli.py`

 * *Files identical despite different names*

### Comparing `utilki-0.3.2/utilki/task_mixin.py` & `utilki-0.3.3/utilki/task_mixin.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from abc import abstractmethod
 import json
 import os
 from datetime import datetime
 from dataclasses import Field
 from pydantic.fields import ModelField
 from typing import (
     Any,
@@ -24,14 +25,32 @@
     List[bool],
     List[int],
     List[float],
     List[str],
 ]
 
 
+singles = [int, float, str, bool, datetime]
+lists = [List[int], List[float], List[str], List[bool]]
+options = [
+    Union[int, None],
+    Union[float, None],
+    Union[str, None],
+    Union[bool, None],
+]
+types_we_support = singles + lists + options
+
+IsDefault = bool
+
+
+def dbg(msg):
+    if False:
+        print(msg)
+
+
 class TaskMixin:
     __dataclass_fields__: ClassVar[Dict[str, Any]]
     __fields__: ClassVar[Dict[str, Any]]
 
     @classmethod
     def __init__(cls, **kwargs):
         ...
@@ -39,133 +58,156 @@
     @classmethod
     def create(cls):
         params: List[Tuple[str, Any]] = []
         if hasattr(cls, "__dataclass_fields__"):
             fields: Iterable[Field] = cls.__dataclass_fields__.values()
             for field in fields:
                 params.append((field.name, field.type))
-        if hasattr(cls, "__fields__"):
+        elif hasattr(cls, "__fields__"):
             model_fields: Iterable[ModelField] = cls.__fields__.values()
             for model_field in model_fields:
                 params.append((model_field.name, model_field.annotation))
+        else:
+            raise TypeError("Invalid type")
         task = cls(**{name: cls.parse(name, type) for name, type in params})
         return task
 
     @classmethod
-    def get_default(cls, name_) -> Defaults:
+    def get_default(cls, name_) -> Tuple[IsDefault, Defaults]:
         env_var = os.getenv(name_)
         if env_var is not None:
-            return env_var
+            dbg(f"{name_} from env: {env_var}")
+            return False, env_var
         if hasattr(cls, "__dataclass_fields__"):
             field: Field = cls.__dataclass_fields__[name_]
             result: Any = field.default
-            return result
+            dbg(f"{name_} default: {result}")
+            return True, result
         elif hasattr(cls, "__fields__"):
             model_field: ModelField = cls.__fields__[name_]
-            return model_field.get_default()
+            default_model = model_field.get_default()
+            dbg(f"{name_} default: {default_model}")
+            return True, default_model
         else:
             raise TypeError("Invalid type")
 
     @classmethod
-    def get_date(cls, param):
-        n = [int(n) for n in param.split("-")]
-        if len(n) == 3:
-            return datetime(n[0], n[1], n[2])
-        elif len(n) == 6:
-            return datetime(n[0], n[1], n[2], n[3], n[4], n[5])
-        else:
-            raise TypeError("Invalid datetime format")
-
-    @classmethod
-    def parse_list(cls, list_str: str, type_) -> List[Any]:
-        if list_str.startswith("[") and list_str.endswith("]"):
-            return json.loads(list_str)
-        # TODO: make this a separate tuple parsing function
-        # elif list_str.startswith("(") and list_str.endswith(")"):
-        #     list_str.replace("(", "[")
-        #     list_str.replace(")", "]")
-        #     return json.loads(list_str)
-        elif "," in list_str:
-            return list(map(type_, list_str.split(",")))
-        else:
-            raise TypeError("Invalid list format")
-
-    @classmethod
-    def parse_options(cls, value, type_):
-        if value in ["None", "none", None, "null", "NULL", ""]:
-            return None
-        else:
-            return type_(value)
-
-    @classmethod
     def parse(cls, name_, type_):
-        value = cls.get_default(name_)
-        # print(f"parsing '{name_}' with type {type_} and value {value}")
+        is_default, value = cls.get_default(name_)
+        if is_default:
+            if type_ not in types_we_support:
+                raise TypeError("Invalid type")
+            if type_ != type(value) and type_ in singles:
+                raise TypeError("Invalid type")
+            if type_ in lists and not isinstance(value, list):
+                raise TypeError("Invalid type")
+            return value
+        dbg(f"parsing '{name_}' with type {type_} and value {value}")
         if isinstance(value, str):
-            if type_ == List[int]:
-                return cls.parse_list(value, int)
-            elif type_ == List[str]:
-                return cls.parse_list(value, str)
-            elif type_ == List[float]:
-                return cls.parse_list(value, float)
-            elif type_ == List[bool]:
-                return cls.parse_list(value, parse_bool)
-            elif type_ == Union[int, None]:
-                return cls.parse_options(value, int)
-            elif type_ == Union[str, None]:
-                return cls.parse_options(value, str)
-            elif type_ == Union[float, None]:
-                return cls.parse_options(value, float)
-            elif type_ == Union[bool, None]:
-                return cls.parse_options(value, parse_bool)
-            elif type_ == bool:
-                return parse_bool(value)
-            elif type_ == int:
-                return int(value)
-            elif type_ == float:
-                return float(value)
-            elif type_ == str:
-                try:
-                    res = json.loads(value)
-                    if type(res) == int:
-                        return str(res)
-                    else:
-                        return res
-                except Exception:
-                    return str(value)
-            elif type_ == datetime:
-                # FIXME actually like use proper parsing lmao
-                if value.startswith('"') and value.endswith('"'):
-                    value = value[1:-1]
-                has_t_or_colon = ":" in value or "T" in value
-                num_parts = len(value.split("-"))
-                if has_t_or_colon:
-                    value = value.replace(" ", "-")
-                    value = value.replace("T", "-")
-                    value = value.replace(":", "-")
-                    return cls.get_date(value)
-                elif num_parts == 3:
-                    return cls.get_date(value)
-                else:
-                    raise TypeError("Invalid datetime format")
+            res = parse_variations(type_, value, name_)
+            dbg(f"res: {res}, type: {type_}, actual type {type(res)}")
+            return res
         elif isinstance(value, list):
             if type_ in [List[int], List[str], List[float], List[bool]]:
                 return value
-        elif type_ == datetime:
-            if isinstance(value, datetime):
+        elif isinstance(value, datetime):
+            if type_ == datetime:
+                return value
+        elif type_ in [int, str, float, bool]:
+            if isinstance(value, type_):
                 return value
-            else:
-                raise TypeError("Invalid default value")
-        elif type_ in [bool, int, float]:
-            return value
         else:
-            print(f"parsing '{name_}' with type {type_} and value {value}")
+            dbg(f"{name_}: {type_}\n'value' {value}: {type(value)}")
             raise TypeError("Invalid type")
 
 
 def parse_bool(param):
     if param in ["True", "true", True]:
         return True
     elif param in ["False", "false", False]:
         return False
     else:
         raise TypeError("Invalid boolean format")
+
+
+def parse_options(value, type_):
+    if value in ["None", "none", None, "null", "NULL", ""]:
+        return None
+    else:
+        return type_(value)
+
+
+def parse_list(list_str: str, type_) -> List[Any]:
+    if list_str.startswith("[") and list_str.endswith("]"):
+        return json.loads(list_str)
+    # TODO: make this a separate tuple parsing function
+    # elif list_str.startswith("(") and list_str.endswith(")"):
+    #     list_str.replace("(", "[")
+    #     list_str.replace(")", "]")
+    #     return json.loads(list_str)
+    elif "," in list_str:
+        return list(map(type_, list_str.split(",")))
+    else:
+        raise ValueError("Invalid list format")
+
+
+def get_date(param: str):
+    n = [int(n) for n in param.split("-")]
+    if len(n) == 3:
+        return datetime(n[0], n[1], n[2])
+    elif len(n) == 6:
+        return datetime(n[0], n[1], n[2], n[3], n[4], n[5])
+    else:
+        raise ValueError("Invalid datetime format")
+
+
+def parse_variations(type_, value, name_):
+    dbg(f"{name_} parse_variations({type_}, {value})")
+    if type_ == List[int]:
+        return parse_list(value, int)
+    elif type_ == List[str]:
+        return parse_list(value, str)
+    elif type_ == List[float]:
+        return parse_list(value, float)
+    elif type_ == List[bool]:
+        return parse_list(value, parse_bool)
+    elif type_ == Union[int, None]:
+        return parse_options(value, int)
+    elif type_ == Union[str, None]:
+        return parse_options(value, str)
+    elif type_ == Union[float, None]:
+        return parse_options(value, float)
+    elif type_ == Union[bool, None]:
+        return parse_options(value, parse_bool)
+    elif type_ == bool:
+        return parse_bool(value)
+    elif type_ == int:
+        return int(value)
+    elif type_ == float:
+        return float(value)
+    elif type_ == str:
+        dbg(f"str: {value}")
+        try:
+            res = json.loads(value)
+            if type(res) == int:
+                dbg(f"json.loads({value})")
+                return str(res)
+            else:
+                return res
+        except Exception:
+            dbg(f"exception: {value}")
+            return str(value)
+    elif type_ == datetime:
+        # FIXME actually like use proper parsing lmao
+        if value.startswith('"') and value.endswith('"'):
+            value = value[1:-1]
+        has_t_or_colon = ":" in value or "T" in value
+        num_parts = len(value.split("-"))
+        if has_t_or_colon:
+            value = value.replace(" ", "-")
+            value = value.replace("T", "-")
+            value = value.replace(":", "-")
+            return get_date(value)
+        elif num_parts == 3:
+            return get_date(value)
+        else:
+            raise TypeError("Invalid datetime format")
```

### Comparing `utilki-0.3.2/setup.py` & `utilki-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['click>=8.1.3,<9.0.0', 'pydantic>=1.10.7,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['utilki = utilki.cli:cli']}
 
 setup_kwargs = {
     'name': 'utilki',
-    'version': '0.3.2',
+    'version': '0.3.3',
     'description': 'A collection of useful utilities',
     'long_description': '# utilki\n\n[![codecov](https://codecov.io/gh/realbikmaev/utilki/branch/main/graph/badge.svg?token=VN0UMT7O9A)](https://codecov.io/gh/realbikmaev/utilki)\n\nutils that are frequently used by me and might be useful for others\n\n## installation\n\n```bash\npip install utilki\n```\n\n## TaskMixin\n\nMixin class that adds `create()` classmethod to dataclass you define as your task params. Useful when you have a lot of container based tasks executed on remote clusters (e.g. Kubernetes, Hashicorp Nomad, etc.). It reads task params from environment variables, parses, and validates them. \n\n```python\nfrom utilki import TaskMixin\n\n@dataclass\nclass Task(TaskMixin):\n    ayy: float = 69.69\n    lmao: str = "420"\n\nos.environ["ayy"] = "42.42"\nos.environ["lmao"] = "69"\n\nt = Task.create()\nprint(f"ayy: {t.ayy}, type: {type(t.ayy)}")\n# ayy: 42.42, type: <class \'float\'>\nprint(f"lmao: {t.lmao}, type: {type(t.lmao)}")\n# lmao: 69, type: <class \'str\'>\n```\n\n## Cli\n\n### Venv\n\n```bash\n$ utilki venv 3.8.10\n$ Enter venv name: new_venv\n$ Created venv `new_venv` with Python version 3.8.10\n```',
     'author': 'Khaidar Bikmaev',
     'author_email': 'khaidar@bikmaev.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `utilki-0.3.2/PKG-INFO` & `utilki-0.3.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utilki
-Version: 0.3.2
+Version: 0.3.3
 Summary: A collection of useful utilities
 Author: Khaidar Bikmaev
 Author-email: khaidar@bikmaev.com
 Requires-Python: >=3.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
```

