# Comparing `tmp/robocorp_log-0.1.1.tar.gz` & `tmp/robocorp_log-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_log-0.1.1.tar", max compression
+gzip compressed data, was "robocorp_log-0.2.0.tar", max compression
```

## Comparing `robocorp_log-0.1.1.tar` & `robocorp_log-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,26 @@
--rw-r--r--   0        0        0    10142 2023-05-10 17:49:39.717459 robocorp_log-0.1.1/LICENSE
--rw-r--r--   0        0        0     5471 2023-05-10 17:49:39.717459 robocorp_log-0.1.1/README.md
--rw-r--r--   0        0        0     1137 2023-05-10 17:49:39.721459 robocorp_log-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    27835 2023-05-10 17:49:39.721459 robocorp_log-0.1.1/src/robocorp/log/__init__.py
--rw-r--r--   0        0        0    13242 2023-05-10 17:49:39.721459 robocorp_log-0.1.1/src/robocorp/log/_ast_utils.py
--rw-r--r--   0        0        0     9794 2023-05-10 17:49:39.721459 robocorp_log-0.1.1/src/robocorp/log/_auto_logging_setup.py
--rw-r--r--   0        0        0     5361 2023-05-10 17:49:39.721459 robocorp_log-0.1.1/src/robocorp/log/_config.py
--rw-r--r--   0        0        0      572 2023-05-10 17:49:39.721459 robocorp_log-0.1.1/src/robocorp/log/_convert_units.py
--rw-r--r--   0        0        0    12420 2023-05-10 17:49:39.721459 robocorp_log-0.1.1/src/robocorp/log/_decoder.py
--rw-r--r--   0        0        0    49206 2023-05-10 17:50:31.613837 robocorp_log-0.1.1/src/robocorp/log/_index.py
--rw-r--r--   0        0        0    61043 2023-05-10 17:50:34.769856 robocorp_log-0.1.1/src/robocorp/log/_index_v2.py
--rw-r--r--   0        0        0     2497 2023-05-10 17:49:39.721459 robocorp_log-0.1.1/src/robocorp/log/_lifecycle_hooks.py
--rw-r--r--   0        0        0      493 2023-05-10 17:49:39.721459 robocorp_log-0.1.1/src/robocorp/log/_logger_instances.py
--rw-r--r--   0        0        0     1208 2023-05-10 17:49:39.721459 robocorp_log-0.1.1/src/robocorp/log/_null.py
--rw-r--r--   0        0        0      385 2023-05-10 17:49:39.721459 robocorp_log-0.1.1/src/robocorp/log/_obj_info_repr.py
--rw-r--r--   0        0        0    21836 2023-05-10 17:49:39.721459 robocorp_log-0.1.1/src/robocorp/log/_rewrite_ast_add_callbacks.py
--rw-r--r--   0        0        0     8900 2023-05-10 17:49:39.721459 robocorp_log-0.1.1/src/robocorp/log/_rewrite_filtering.py
--rw-r--r--   0        0        0    12453 2023-05-10 17:49:39.721459 robocorp_log-0.1.1/src/robocorp/log/_rewrite_importhook.py
--rw-r--r--   0        0        0     9706 2023-05-10 17:49:39.721459 robocorp_log-0.1.1/src/robocorp/log/_robo_logger.py
--rw-r--r--   0        0        0    55042 2023-05-10 17:49:39.721459 robocorp_log-0.1.1/src/robocorp/log/_robo_output_impl.py
--rw-r--r--   0        0        0     1436 2023-05-10 17:49:39.721459 robocorp_log-0.1.1/src/robocorp/log/_sensitive_variable_names.py
--rw-r--r--   0        0        0     1915 2023-05-10 17:49:39.721459 robocorp_log-0.1.1/src/robocorp/log/_suppress_helper.py
--rw-r--r--   0        0        0     7802 2023-05-10 17:49:39.725459 robocorp_log-0.1.1/src/robocorp/log/console.py
--rw-r--r--   0        0        0     1057 2023-05-10 17:49:39.725459 robocorp_log-0.1.1/src/robocorp/log/protocols.py
--rw-r--r--   0        0        0        0 2023-05-10 17:49:39.725459 robocorp_log-0.1.1/src/robocorp/log/py.typed
--rw-r--r--   0        0        0     7312 2023-05-10 17:49:39.725459 robocorp_log-0.1.1/src/robocorp/log/redirect.py
--rw-r--r--   0        0        0     6269 1970-01-01 00:00:00.000000 robocorp_log-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    10142 2023-05-25 10:34:59.733227 robocorp_log-0.2.0/LICENSE
+-rw-r--r--   0        0        0     5471 2023-05-25 10:34:59.733227 robocorp_log-0.2.0/README.md
+-rw-r--r--   0        0        0     1156 2023-05-25 10:34:59.741227 robocorp_log-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    27573 2023-05-25 10:34:59.741227 robocorp_log-0.2.0/src/robocorp/log/__init__.py
+-rw-r--r--   0        0        0    13242 2023-05-25 10:34:59.741227 robocorp_log-0.2.0/src/robocorp/log/_ast_utils.py
+-rw-r--r--   0        0        0     9794 2023-05-25 10:34:59.741227 robocorp_log-0.2.0/src/robocorp/log/_auto_logging_setup.py
+-rw-r--r--   0        0        0     5361 2023-05-25 10:34:59.741227 robocorp_log-0.2.0/src/robocorp/log/_config.py
+-rw-r--r--   0        0        0      572 2023-05-25 10:34:59.741227 robocorp_log-0.2.0/src/robocorp/log/_convert_units.py
+-rw-r--r--   0        0        0    12420 2023-05-25 10:34:59.741227 robocorp_log-0.2.0/src/robocorp/log/_decoder.py
+-rw-r--r--   0        0        0   442715 2023-05-25 10:35:55.303464 robocorp_log-0.2.0/src/robocorp/log/_index_v3.py
+-rw-r--r--   0        0        0     2497 2023-05-25 10:34:59.741227 robocorp_log-0.2.0/src/robocorp/log/_lifecycle_hooks.py
+-rw-r--r--   0        0        0      493 2023-05-25 10:34:59.741227 robocorp_log-0.2.0/src/robocorp/log/_logger_instances.py
+-rw-r--r--   0        0        0     1208 2023-05-25 10:34:59.741227 robocorp_log-0.2.0/src/robocorp/log/_null.py
+-rw-r--r--   0        0        0      385 2023-05-25 10:34:59.741227 robocorp_log-0.2.0/src/robocorp/log/_obj_info_repr.py
+-rw-r--r--   0        0        0    21836 2023-05-25 10:34:59.741227 robocorp_log-0.2.0/src/robocorp/log/_rewrite_ast_add_callbacks.py
+-rw-r--r--   0        0        0     8900 2023-05-25 10:34:59.741227 robocorp_log-0.2.0/src/robocorp/log/_rewrite_filtering.py
+-rw-r--r--   0        0        0    12453 2023-05-25 10:34:59.741227 robocorp_log-0.2.0/src/robocorp/log/_rewrite_importhook.py
+-rw-r--r--   0        0        0     9706 2023-05-25 10:34:59.741227 robocorp_log-0.2.0/src/robocorp/log/_robo_logger.py
+-rw-r--r--   0        0        0    54921 2023-05-25 10:34:59.741227 robocorp_log-0.2.0/src/robocorp/log/_robo_output_impl.py
+-rw-r--r--   0        0        0     1436 2023-05-25 10:34:59.741227 robocorp_log-0.2.0/src/robocorp/log/_sensitive_variable_names.py
+-rw-r--r--   0        0        0     1915 2023-05-25 10:34:59.741227 robocorp_log-0.2.0/src/robocorp/log/_suppress_helper.py
+-rw-r--r--   0        0        0     7802 2023-05-25 10:34:59.741227 robocorp_log-0.2.0/src/robocorp/log/console.py
+-rw-r--r--   0        0        0     1057 2023-05-25 10:34:59.741227 robocorp_log-0.2.0/src/robocorp/log/protocols.py
+-rw-r--r--   0        0        0        0 2023-05-25 10:34:59.741227 robocorp_log-0.2.0/src/robocorp/log/py.typed
+-rw-r--r--   0        0        0     7317 2023-05-25 10:34:59.741227 robocorp_log-0.2.0/src/robocorp/log/redirect.py
+-rw-r--r--   0        0        0     6117 1970-01-01 00:00:00.000000 robocorp_log-0.2.0/PKG-INFO
```

### Comparing `robocorp_log-0.1.1/LICENSE` & `robocorp_log-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.1.1/README.md` & `robocorp_log-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.1.1/pyproject.toml` & `robocorp_log-0.2.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "robocorp-log"
-version = "0.1.1"
+version = "0.2.0"
 description = "Automatic trace logging for Python"
 authors = [
     "Fabio Zadrozny <fabio@robocorp.com>",
 ]
 readme = "README.md"
 packages = [{include = "robocorp/log", from = "src"}]
-include = ["**/_index.py", "**/_index_v2.py"]
+include = ["**/_index.py", "**/_index_v2.py", "**/_index_v3.py"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: System :: Logging",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
```

### Comparing `robocorp_log-0.1.1/src/robocorp/log/__init__.py` & `robocorp_log-0.2.0/src/robocorp/log/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from .protocols import OptExcInfo, LogHTMLStyle, Status, IReadLines
 from ._suppress_helper import SuppressHelper as _SuppressHelper
 
 
 if typing.TYPE_CHECKING:
     from ._robo_logger import _RoboLogger
 
-__version__ = "0.1.1"
+__version__ = "0.2.0"
 version_info = [int(x) for x in __version__.split(".")]
 
 from . import _config
 
 # --- Make these a part of the public API.
 
 Filter = _config.Filter
@@ -68,15 +68,14 @@
 
 def critical(*message: Any) -> None:
     """
     Adds a new logging message with a critical (error) level.
 
     Args:
         message: The message which should be logged.
-        html: If True the message passed should be rendered as HTML.
 
     Example:
         critical('Failed because', obj, 'is not', expected)
 
     Note:
         Formatting converts all objects given to `str`. If you need custom
         formatting please pre-format the string.
@@ -88,15 +87,14 @@
 
 def warn(*message: Any) -> None:
     """
     Adds a new logging message with a warn level.
 
     Args:
         message: The message which should be logged.
-        html: If True the message passed should be rendered as HTML.
 
     Example:
         warn('Did not expect', obj)
 
     Note:
         Formatting converts all objects given to `str`. If you need custom
         formatting please pre-format the string.
@@ -108,15 +106,14 @@
 
 def info(*message: Any) -> None:
     """
     Adds a new logging message with an info level.
 
     Args:
         message: The message which should be logged.
-        html: If True the message passed should be rendered as HTML.
 
 
     Example:
         info('Received value', obj)
 
     Note:
         Formatting converts all objects given to `str`. If you need custom
@@ -130,15 +127,14 @@
 
 def exception(*message: Any):
     """
     Adds to the logging the exceptions that's currently raised.
 
     Args:
         message: If given an additional error message to be shown.
-        html: If True the message passed should be rendered as HTML.
     """
     if message:
         _log(Status.ERROR, message)
 
     exc_info = sys.exc_info()
     for robo_logger in _get_logger_instances():
         robo_logger.log_method_except(exc_info, unhandled=True)
@@ -599,15 +595,15 @@
         # It may be that we're in dev mode and the target should be the bundle.js
         bundle_js = log_html.parent / "bundle.js"
         if bundle_js.exists():
             txt = bundle_js.read_text(encoding="utf-8")
             i = txt.find("let chunks = [")
             j = txt.find("];", i)
 
-    assert i > 0, "Could not find the chunks in the file."
+    assert i > 0, f"Could not find the chunks in the file ({log_html})."
     assert j > 0, "Could not find the end of the chunks in the file."
 
     sub = txt[i + len("let chunks = ") : j + 1]
     # We have something as:
     # ['base64strZippedStr', 'base64strZippedStr']
     # so, at this point decode it and unzip it
     lst = literal_eval(sub)
```

### Comparing `robocorp_log-0.1.1/src/robocorp/log/_ast_utils.py` & `robocorp_log-0.2.0/src/robocorp/log/_ast_utils.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.1.1/src/robocorp/log/_auto_logging_setup.py` & `robocorp_log-0.2.0/src/robocorp/log/_auto_logging_setup.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.1.1/src/robocorp/log/_config.py` & `robocorp_log-0.2.0/src/robocorp/log/_config.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.1.1/src/robocorp/log/_convert_units.py` & `robocorp_log-0.2.0/src/robocorp/log/_convert_units.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.1.1/src/robocorp/log/_decoder.py` & `robocorp_log-0.2.0/src/robocorp/log/_decoder.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.1.1/src/robocorp/log/_lifecycle_hooks.py` & `robocorp_log-0.2.0/src/robocorp/log/_lifecycle_hooks.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.1.1/src/robocorp/log/_null.py` & `robocorp_log-0.2.0/src/robocorp/log/_null.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.1.1/src/robocorp/log/_rewrite_ast_add_callbacks.py` & `robocorp_log-0.2.0/src/robocorp/log/_rewrite_ast_add_callbacks.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.1.1/src/robocorp/log/_rewrite_filtering.py` & `robocorp_log-0.2.0/src/robocorp/log/_rewrite_filtering.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.1.1/src/robocorp/log/_rewrite_importhook.py` & `robocorp_log-0.2.0/src/robocorp/log/_rewrite_importhook.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.1.1/src/robocorp/log/_robo_logger.py` & `robocorp_log-0.2.0/src/robocorp/log/_robo_logger.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.1.1/src/robocorp/log/_robo_output_impl.py` & `robocorp_log-0.2.0/src/robocorp/log/_robo_output_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -907,22 +907,15 @@
         if log_html:
             target = os.path.abspath(log_html)
             dirname = os.path.dirname(target)
             if not os.path.exists(dirname):
                 os.makedirs(dirname, exist_ok=True)
             print(f"Robocorp Log (html): {target}")
 
-            if self._config.log_html_style == 1:
-                from robocorp.log import _index as index
-            elif self._config.log_html_style == 2:
-                from robocorp.log import _index_v2 as index
-            else:
-                raise ValueError(
-                    f"Unexpected log html style: {self._config.log_html_style}"
-                )
+            from robocorp.log import _index_v3 as index
 
             has_separate_bundle_js = "bundle.js" in index.FILE_CONTENTS
 
             for name, contents in index.FILE_CONTENTS.items():
                 if name == "index.html":
                     if has_separate_bundle_js:
                         self._write_simple(target, contents)
@@ -952,34 +945,39 @@
             assert end_of_json_parse_index > 0
             self._write_updating_sample(
                 stream, contents, return_json_parse_index, end_of_json_parse_index
             )
 
     def _write_index_updating_sample(self, target, contents):
         with open(target, "wb") as stream:
-            sample_contents_index = contents.index("getSampleContents")
-            assert sample_contents_index > 0
+            string_start = contents.index("String.raw`V 0.0.2")
+            string_end = contents.index("`", string_start + 18)
+            string_end = contents.index("}", string_end)
+
+            assert string_start > 0, f'Could not find "String.raw`V 0.0.2" in {target}.'
+            assert string_end > 0, f"Could not find the string end in {target}."
+
+            # Now, go a bit back in the string and find the `const XXX=` to also remove that.
+            i = string_start
+            found = []
+            while i > 0:
+                c = contents[i]
+                found.insert(0, c)
+
+                if "".join(found).startswith("const "):
+                    string_start = i
+                    break
+                i -= 1
 
-            return_json_parse_index = contents.index(
-                "return JSON.parse", sample_contents_index
-            )
-            assert return_json_parse_index > 0
-
-            end_of_json_parse_index = contents.index(")}}", return_json_parse_index) + 1
-            assert end_of_json_parse_index > 0
-            self._write_updating_sample(
-                stream, contents, return_json_parse_index, end_of_json_parse_index
-            )
+            self._write_updating_sample(stream, contents, string_start, string_end)
 
-    def _write_updating_sample(
-        self, stream, contents, return_json_parse_index, end_of_json_parse_index
-    ):
+    def _write_updating_sample(self, stream, contents, start_index, end_index):
         import base64
 
-        stream.write(contents[:return_json_parse_index].encode("utf-8"))
+        stream.write(contents[:start_index].encode("utf-8"))
 
         import zlib
 
         write = stream.write
         if WRITE_CONTENTS_TO_STDERR:
             stream_write = write
 
@@ -1033,8 +1031,8 @@
     offset += item.length;
 }
 
 return new TextDecoder().decode(mergedArray);
 """
         )
 
-        stream.write(contents[end_of_json_parse_index:].encode("utf-8"))
+        stream.write(contents[end_index:].encode("utf-8"))
```

### Comparing `robocorp_log-0.1.1/src/robocorp/log/_sensitive_variable_names.py` & `robocorp_log-0.2.0/src/robocorp/log/_sensitive_variable_names.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.1.1/src/robocorp/log/_suppress_helper.py` & `robocorp_log-0.2.0/src/robocorp/log/_suppress_helper.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.1.1/src/robocorp/log/console.py` & `robocorp_log-0.2.0/src/robocorp/log/console.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.1.1/src/robocorp/log/protocols.py` & `robocorp_log-0.2.0/src/robocorp/log/protocols.py`

 * *Files identical despite different names*

### Comparing `robocorp_log-0.1.1/src/robocorp/log/redirect.py` & `robocorp_log-0.2.0/src/robocorp/log/redirect.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from contextlib import contextmanager, redirect_stdout, redirect_stderr
 import json
 import os
 import sys
 import traceback
-from typing import Iterator, IO, AnyStr, Iterable
+from typing import Iterator, IO, Any, AnyStr, Iterable
 from threading import RLock
 from robocorp.log import console_message
 
 
 class _IORedirector(IO[str]):
     """
     This class works to wrap a stream (stdout/stderr) with an additional redirect.
```

### Comparing `robocorp_log-0.1.1/PKG-INFO` & `robocorp_log-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 Metadata-Version: 2.1
 Name: robocorp-log
-Version: 0.1.1
+Version: 0.2.0
 Summary: Automatic trace logging for Python
 Author: Fabio Zadrozny
 Author-email: fabio@robocorp.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Logging
 Requires-Dist: tomli (>=2.0.1,<3.0.0) ; python_version < "3.11"
 Description-Content-Type: text/markdown
 
 # robocorp-log
```

