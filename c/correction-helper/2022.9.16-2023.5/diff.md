# Comparing `tmp/correction-helper-2022.9.16.tar.gz` & `tmp/correction-helper-2023.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "correction-helper-2022.9.16.tar", last modified: Fri Sep 16 13:30:30 2022, max compression
+gzip compressed data, was "correction-helper-2023.5.tar", last modified: Thu May 25 08:29:13 2023, max compression
```

## Comparing `correction-helper-2022.9.16.tar` & `correction-helper-2023.5.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2022-09-16 13:30:30.966759 correction-helper-2022.9.16/
--rw-r--r--   0 mdk       (1000) mdk       (1000)     3429 2022-09-16 13:30:30.966759 correction-helper-2022.9.16/PKG-INFO
--rw-r--r--   0 mdk       (1000) mdk       (1000)     2824 2022-04-13 21:56:28.000000 correction-helper-2022.9.16/README.md
-drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2022-09-16 13:30:30.966759 correction-helper-2022.9.16/correction_helper.egg-info/
--rw-r--r--   0 mdk       (1000) mdk       (1000)     3429 2022-09-16 13:30:30.000000 correction-helper-2022.9.16/correction_helper.egg-info/PKG-INFO
--rw-r--r--   0 mdk       (1000) mdk       (1000)      249 2022-09-16 13:30:30.000000 correction-helper-2022.9.16/correction_helper.egg-info/SOURCES.txt
--rw-r--r--   0 mdk       (1000) mdk       (1000)        1 2022-09-16 13:30:30.000000 correction-helper-2022.9.16/correction_helper.egg-info/dependency_links.txt
--rw-r--r--   0 mdk       (1000) mdk       (1000)       27 2022-09-16 13:30:30.000000 correction-helper-2022.9.16/correction_helper.egg-info/requires.txt
--rw-r--r--   0 mdk       (1000) mdk       (1000)       18 2022-09-16 13:30:30.000000 correction-helper-2022.9.16/correction_helper.egg-info/top_level.txt
--rw-r--r--   0 mdk       (1000) mdk       (1000)    16910 2022-09-16 13:29:25.000000 correction-helper-2022.9.16/correction_helper.py
--rw-r--r--   0 mdk       (1000) mdk       (1000)      982 2022-09-02 09:29:40.000000 correction-helper-2022.9.16/pyproject.toml
--rw-r--r--   0 mdk       (1000) mdk       (1000)       38 2022-09-16 13:30:30.966759 correction-helper-2022.9.16/setup.cfg
+drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2023-05-25 08:29:13.334617 correction-helper-2023.5/
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     3426 2023-05-25 08:29:13.334617 correction-helper-2023.5/PKG-INFO
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     2824 2022-04-13 21:56:28.000000 correction-helper-2023.5/README.md
+drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2023-05-25 08:29:13.334617 correction-helper-2023.5/correction_helper.egg-info/
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     3426 2023-05-25 08:29:13.000000 correction-helper-2023.5/correction_helper.egg-info/PKG-INFO
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      300 2023-05-25 08:29:13.000000 correction-helper-2023.5/correction_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 mdk       (1000) mdk       (1000)        1 2023-05-25 08:29:13.000000 correction-helper-2023.5/correction_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 mdk       (1000) mdk       (1000)       27 2023-05-25 08:29:13.000000 correction-helper-2023.5/correction_helper.egg-info/requires.txt
+-rw-r--r--   0 mdk       (1000) mdk       (1000)       18 2023-05-25 08:29:13.000000 correction-helper-2023.5/correction_helper.egg-info/top_level.txt
+-rw-r--r--   0 mdk       (1000) mdk       (1000)    16964 2023-05-25 08:27:42.000000 correction-helper-2023.5/correction_helper.py
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      982 2022-09-02 09:29:40.000000 correction-helper-2023.5/pyproject.toml
+-rw-r--r--   0 mdk       (1000) mdk       (1000)       38 2023-05-25 08:29:13.334617 correction-helper-2023.5/setup.cfg
+drwxr-xr-x   0 mdk       (1000) mdk       (1000)        0 2023-05-25 08:29:13.334617 correction-helper-2023.5/tests/
+-rw-r--r--   0 mdk       (1000) mdk       (1000)      877 2021-02-09 22:18:51.000000 correction-helper-2023.5/tests/test_compare.py
+-rw-r--r--   0 mdk       (1000) mdk       (1000)     2067 2021-11-07 09:16:28.000000 correction-helper-2023.5/tests/test_contextmanager.py
```

### Comparing `correction-helper-2022.9.16/PKG-INFO` & `correction-helper-2023.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: correction-helper
-Version: 2022.9.16
+Version: 2023.5
 Summary: Some helpers to help writing correction bots, use by hackinscience.org.
 Author-email: Julien Palard <julien@palard.fr>
 License: MIT License
 Project-URL: Homepage, https://github.com/JulienPalard/correction-helper
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `correction-helper-2022.9.16/README.md` & `correction-helper-2023.5/README.md`

 * *Files identical despite different names*

### Comparing `correction-helper-2022.9.16/correction_helper.egg-info/PKG-INFO` & `correction-helper-2023.5/correction_helper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: correction-helper
-Version: 2022.9.16
+Version: 2023.5
 Summary: Some helpers to help writing correction bots, use by hackinscience.org.
 Author-email: Julien Palard <julien@palard.fr>
 License: MIT License
 Project-URL: Homepage, https://github.com/JulienPalard/correction-helper
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `correction-helper-2022.9.16/correction_helper.py` & `correction-helper-2023.5/correction_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from pathlib import Path
 from textwrap import indent
 from typing import Optional, Sequence, Tuple, Union
 
 import friendly_traceback
 from friendly_traceback import exclude_file_from_traceback
 
-__version__ = "2022.9.16"
+__version__ = "2023.5"
 
 friendly_traceback.set_lang(os.environ.get("LANGUAGE", "en"))
 
 exclude_file_from_traceback(__file__)
 
 _ = gettext.translation("check", Path(__file__).parent, fallback=True).gettext
 
@@ -140,15 +140,15 @@
     return prefix + message
 
 
 @contextmanager
 def student_code(  # pylint: disable=too-many-arguments,too-many-branches
     *,
     prefix=(),
-    exception_prefix="I got an exception:",
+    exception_prefix="",
     print_allowed=True,  # pylint: disable=redefined-outer-name
     print_hook=None,
     print_prefix="Your code printed:",
     too_slow_message="Your program looks too slow, looks like an infinite loop.",
     timeout=1,
 ):
     """Execute student code under surveillance.
@@ -249,15 +249,15 @@
 
     (Then exit with an error code of 1 if the student has printed.)
     """
     message = _prepare_message(message)
 
     def print_cb(out, err):
         if err or out:
-            print(message, sep="\n\n", end="\n\n")
+            print(*message, sep="\n\n", end="\n\n")
             if err:
                 print(code(err))
             if out:
                 print(code(out))
             sys.exit(1)
 
     return print_cb
@@ -284,38 +284,37 @@
         :::text
         42
     """
     message = _prepare_message(message)
 
     def print_cb(out, err):
         if err or out:
-            print(message, sep="\n\n", end="\n\n")
+            print(*message, sep="\n\n", end="\n\n")
         if err:
             print(code(err))
         if out:
             print(code(out))
 
     return print_cb
 
 
-def print_to_admonition(
-    admonition_type="info",
-    header="Your code printed:",
-):
+def print_to_admonition(header="Your code printed:", admonition_type="info"):
     """To be used as print_hook, renders prints as a Markdown admonition.
 
     >>> with student_code(print_hook=print_to_admonition("info", "FYI it printed:")):
     ...     print(42)
     !!! info ""
 
         FYI it printed:
 
             :::text
             42
     """
+    if not isinstance(header, str):
+        header = "\n\n".join(header)
     return lambda out, err: admonition(
         admonition_type,
         header,
         code(out + "\n" + err),
     )
 
 
@@ -324,15 +323,15 @@
 
     >>> admonition("note", "Hello world.")
     !!! note ""
         Hello world.
     """
     print(f'!!! {admonition_type} "{title}"\n')
     for item in body:
-        print(indent(item, "    "), end="\n\n")
+        print(indent(item, "    "), sep="\n\n", end="\n\n")
 
 
 @dataclass
 class Section:
     """A section of friendly output."""
 
     name: str
```

### Comparing `correction-helper-2022.9.16/pyproject.toml` & `correction-helper-2023.5/pyproject.toml`

 * *Files identical despite different names*

