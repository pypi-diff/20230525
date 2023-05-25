# Comparing `tmp/clevertable-2.4.1.tar.gz` & `tmp/clevertable-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clevertable-2.4.1.tar", last modified: Wed May 24 09:39:18 2023, max compression
+gzip compressed data, was "clevertable-2.5.0.tar", last modified: Wed May 24 11:02:18 2023, max compression
```

## Comparing `clevertable-2.4.1.tar` & `clevertable-2.5.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 09:39:18.532261 clevertable-2.4.1/
--rw-rw-rw-   0        0        0     1086 2023-04-21 11:55:46.000000 clevertable-2.4.1/LICENSE
--rw-rw-rw-   0        0        0    34992 2023-05-24 09:39:18.532261 clevertable-2.4.1/PKG-INFO
--rw-rw-rw-   0        0        0    33222 2023-05-24 08:31:40.000000 clevertable-2.4.1/README.md
--rw-rw-rw-   0        0        0     1306 2023-05-24 09:38:51.000000 clevertable-2.4.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-24 09:39:18.532261 clevertable-2.4.1/setup.cfg
--rw-rw-rw-   0        0        0      230 2023-04-21 12:00:42.000000 clevertable-2.4.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-24 09:39:18.485148 clevertable-2.4.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-24 09:39:18.518753 clevertable-2.4.1/src/clevertable/
--rw-rw-rw-   0        0        0     3512 2023-05-24 08:33:41.000000 clevertable-2.4.1/src/clevertable/Binary.py
--rw-rw-rw-   0        0        0      268 2023-05-17 09:40:22.000000 clevertable-2.4.1/src/clevertable/Const.py
--rw-rw-rw-   0        0        0     3016 2023-05-24 04:34:02.000000 clevertable-2.4.1/src/clevertable/ConversionProfile.py
--rw-rw-rw-   0        0        0     3803 2023-05-09 06:20:57.000000 clevertable-2.4.1/src/clevertable/Converter.py
--rw-rw-rw-   0        0        0     4074 2023-05-24 04:34:02.000000 clevertable-2.4.1/src/clevertable/DataFrameProfile.py
--rw-rw-rw-   0        0        0      924 2023-05-03 13:32:15.000000 clevertable-2.4.1/src/clevertable/Enumerate.py
--rw-rw-rw-   0        0        0      258 2023-05-01 13:13:02.000000 clevertable-2.4.1/src/clevertable/Flatten.py
--rw-rw-rw-   0        0        0     3857 2023-05-04 10:30:56.000000 clevertable-2.4.1/src/clevertable/Float.py
--rw-rw-rw-   0        0        0      877 2023-05-01 13:05:29.000000 clevertable-2.4.1/src/clevertable/ForEach.py
--rw-rw-rw-   0        0        0     4948 2023-05-17 10:26:00.000000 clevertable-2.4.1/src/clevertable/Function.py
--rw-rw-rw-   0        0        0      211 2023-05-01 14:33:13.000000 clevertable-2.4.1/src/clevertable/Id.py
--rw-rw-rw-   0        0        0      366 2023-05-01 17:38:30.000000 clevertable-2.4.1/src/clevertable/Ignore.py
--rw-rw-rw-   0        0        0     3018 2023-05-04 06:01:53.000000 clevertable-2.4.1/src/clevertable/Infer.py
--rw-rw-rw-   0        0        0      402 2023-05-24 08:56:57.000000 clevertable-2.4.1/src/clevertable/Label.py
--rw-rw-rw-   0        0        0     3302 2023-05-04 18:08:01.000000 clevertable-2.4.1/src/clevertable/List.py
--rw-rw-rw-   0        0        0     1343 2023-05-03 09:48:28.000000 clevertable-2.4.1/src/clevertable/Map.py
--rw-rw-rw-   0        0        0     1446 2023-05-04 18:08:46.000000 clevertable-2.4.1/src/clevertable/OneHot.py
--rw-rw-rw-   0        0        0     1663 2023-05-24 09:36:41.000000 clevertable-2.4.1/src/clevertable/Parallel.py
--rw-rw-rw-   0        0        0     2872 2023-05-04 05:25:50.000000 clevertable-2.4.1/src/clevertable/Pipeline.py
--rw-rw-rw-   0        0        0     6829 2023-05-24 04:34:02.000000 clevertable-2.4.1/src/clevertable/RecordProfile.py
--rw-rw-rw-   0        0        0      835 2023-05-04 12:11:29.000000 clevertable-2.4.1/src/clevertable/Split.py
--rw-rw-rw-   0        0        0     3370 2023-05-17 10:34:53.000000 clevertable-2.4.1/src/clevertable/StrictFunction.py
--rw-rw-rw-   0        0        0      989 2023-05-04 12:12:21.000000 clevertable-2.4.1/src/clevertable/Strip.py
--rw-rw-rw-   0        0        0     1159 2023-05-17 09:23:55.000000 clevertable-2.4.1/src/clevertable/Transpose.py
--rw-rw-rw-   0        0        0     2751 2023-05-10 15:17:59.000000 clevertable-2.4.1/src/clevertable/Try.py
--rw-rw-rw-   0        0        0      716 2023-05-24 09:38:51.000000 clevertable-2.4.1/src/clevertable/__init__.py
--rw-rw-rw-   0        0        0     1271 2023-05-04 11:54:43.000000 clevertable-2.4.1/src/clevertable/__main__.py
--rw-rw-rw-   0        0        0     2664 2023-05-17 09:41:23.000000 clevertable-2.4.1/src/clevertable/_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-24 09:39:18.532261 clevertable-2.4.1/src/clevertable.egg-info/
--rw-rw-rw-   0        0        0    34992 2023-05-24 09:39:18.000000 clevertable-2.4.1/src/clevertable.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1044 2023-05-24 09:39:18.000000 clevertable-2.4.1/src/clevertable.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 09:39:18.000000 clevertable-2.4.1/src/clevertable.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-05-24 09:39:18.000000 clevertable-2.4.1/src/clevertable.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       56 2023-05-24 09:39:18.000000 clevertable-2.4.1/src/clevertable.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-24 09:39:18.000000 clevertable-2.4.1/src/clevertable.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-24 11:02:18.046694 clevertable-2.5.0/
+-rw-rw-rw-   0        0        0     1086 2023-04-21 11:55:46.000000 clevertable-2.5.0/LICENSE
+-rw-rw-rw-   0        0        0    34992 2023-05-24 11:02:18.046694 clevertable-2.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0    33222 2023-05-24 08:31:40.000000 clevertable-2.5.0/README.md
+-rw-rw-rw-   0        0        0     1306 2023-05-24 11:01:48.000000 clevertable-2.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-24 11:02:18.046694 clevertable-2.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      230 2023-04-21 12:00:42.000000 clevertable-2.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 11:02:17.983628 clevertable-2.5.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-24 11:02:18.031068 clevertable-2.5.0/src/clevertable/
+-rw-rw-rw-   0        0        0     3512 2023-05-24 08:33:41.000000 clevertable-2.5.0/src/clevertable/Binary.py
+-rw-rw-rw-   0        0        0      268 2023-05-17 09:40:22.000000 clevertable-2.5.0/src/clevertable/Const.py
+-rw-rw-rw-   0        0        0     3016 2023-05-24 04:34:02.000000 clevertable-2.5.0/src/clevertable/ConversionProfile.py
+-rw-rw-rw-   0        0        0     3803 2023-05-09 06:20:57.000000 clevertable-2.5.0/src/clevertable/Converter.py
+-rw-rw-rw-   0        0        0     4074 2023-05-24 04:34:02.000000 clevertable-2.5.0/src/clevertable/DataFrameProfile.py
+-rw-rw-rw-   0        0        0      924 2023-05-03 13:32:15.000000 clevertable-2.5.0/src/clevertable/Enumerate.py
+-rw-rw-rw-   0        0        0      258 2023-05-01 13:13:02.000000 clevertable-2.5.0/src/clevertable/Flatten.py
+-rw-rw-rw-   0        0        0     3857 2023-05-04 10:30:56.000000 clevertable-2.5.0/src/clevertable/Float.py
+-rw-rw-rw-   0        0        0      877 2023-05-01 13:05:29.000000 clevertable-2.5.0/src/clevertable/ForEach.py
+-rw-rw-rw-   0        0        0     4948 2023-05-17 10:26:00.000000 clevertable-2.5.0/src/clevertable/Function.py
+-rw-rw-rw-   0        0        0      211 2023-05-01 14:33:13.000000 clevertable-2.5.0/src/clevertable/Id.py
+-rw-rw-rw-   0        0        0      366 2023-05-01 17:38:30.000000 clevertable-2.5.0/src/clevertable/Ignore.py
+-rw-rw-rw-   0        0        0     3018 2023-05-04 06:01:53.000000 clevertable-2.5.0/src/clevertable/Infer.py
+-rw-rw-rw-   0        0        0      402 2023-05-24 08:56:57.000000 clevertable-2.5.0/src/clevertable/Label.py
+-rw-rw-rw-   0        0        0     3302 2023-05-04 18:08:01.000000 clevertable-2.5.0/src/clevertable/List.py
+-rw-rw-rw-   0        0        0     1343 2023-05-03 09:48:28.000000 clevertable-2.5.0/src/clevertable/Map.py
+-rw-rw-rw-   0        0        0     1446 2023-05-04 18:08:46.000000 clevertable-2.5.0/src/clevertable/OneHot.py
+-rw-rw-rw-   0        0        0     1663 2023-05-24 09:36:41.000000 clevertable-2.5.0/src/clevertable/Parallel.py
+-rw-rw-rw-   0        0        0     2872 2023-05-04 05:25:50.000000 clevertable-2.5.0/src/clevertable/Pipeline.py
+-rw-rw-rw-   0        0        0     7158 2023-05-24 10:58:23.000000 clevertable-2.5.0/src/clevertable/RecordProfile.py
+-rw-rw-rw-   0        0        0      835 2023-05-04 12:11:29.000000 clevertable-2.5.0/src/clevertable/Split.py
+-rw-rw-rw-   0        0        0     3370 2023-05-17 10:34:53.000000 clevertable-2.5.0/src/clevertable/StrictFunction.py
+-rw-rw-rw-   0        0        0      989 2023-05-04 12:12:21.000000 clevertable-2.5.0/src/clevertable/Strip.py
+-rw-rw-rw-   0        0        0     1159 2023-05-17 09:23:55.000000 clevertable-2.5.0/src/clevertable/Transpose.py
+-rw-rw-rw-   0        0        0     2751 2023-05-10 15:17:59.000000 clevertable-2.5.0/src/clevertable/Try.py
+-rw-rw-rw-   0        0        0      716 2023-05-24 11:01:48.000000 clevertable-2.5.0/src/clevertable/__init__.py
+-rw-rw-rw-   0        0        0     1271 2023-05-04 11:54:43.000000 clevertable-2.5.0/src/clevertable/__main__.py
+-rw-rw-rw-   0        0        0     2664 2023-05-17 09:41:23.000000 clevertable-2.5.0/src/clevertable/_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-24 11:02:18.046694 clevertable-2.5.0/src/clevertable.egg-info/
+-rw-rw-rw-   0        0        0    34992 2023-05-24 11:02:17.000000 clevertable-2.5.0/src/clevertable.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1044 2023-05-24 11:02:17.000000 clevertable-2.5.0/src/clevertable.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 11:02:17.000000 clevertable-2.5.0/src/clevertable.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-05-24 11:02:17.000000 clevertable-2.5.0/src/clevertable.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       56 2023-05-24 11:02:17.000000 clevertable-2.5.0/src/clevertable.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-24 11:02:17.000000 clevertable-2.5.0/src/clevertable.egg-info/top_level.txt
```

### Comparing `clevertable-2.4.1/LICENSE` & `clevertable-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clevertable-2.4.1/PKG-INFO` & `clevertable-2.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clevertable
-Version: 2.4.1
+Version: 2.5.0
 Summary: Low effort conversion of tabular data into numerical values.
 Author: Tom Mohr
 License: MIT License
         
         Copyright (c) 2023 Tom Mohr
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `clevertable-2.4.1/README.md` & `clevertable-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `clevertable-2.4.1/pyproject.toml` & `clevertable-2.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "clevertable"
-version = "2.4.1"
+version = "2.5.0"
 description = "Low effort conversion of tabular data into numerical values."
 readme = "README.md"
 authors = [{ name = "Tom Mohr" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -29,15 +29,15 @@
 [project.urls]
 Homepage = "https://github.com/tom-mohr/clevertable"
 
 [project.scripts]
 clevertable = "clevertable.__main__:main"
 
 [tool.bumpver]
-current_version = "2.4.1"
+current_version = "2.5.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `clevertable-2.4.1/src/clevertable/Binary.py` & `clevertable-2.5.0/src/clevertable/Binary.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.4.1/src/clevertable/ConversionProfile.py` & `clevertable-2.5.0/src/clevertable/ConversionProfile.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.4.1/src/clevertable/Converter.py` & `clevertable-2.5.0/src/clevertable/Converter.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.4.1/src/clevertable/DataFrameProfile.py` & `clevertable-2.5.0/src/clevertable/DataFrameProfile.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.4.1/src/clevertable/Enumerate.py` & `clevertable-2.5.0/src/clevertable/Enumerate.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.4.1/src/clevertable/Float.py` & `clevertable-2.5.0/src/clevertable/Float.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.4.1/src/clevertable/ForEach.py` & `clevertable-2.5.0/src/clevertable/ForEach.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.4.1/src/clevertable/Function.py` & `clevertable-2.5.0/src/clevertable/Function.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.4.1/src/clevertable/Infer.py` & `clevertable-2.5.0/src/clevertable/Infer.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.4.1/src/clevertable/List.py` & `clevertable-2.5.0/src/clevertable/List.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.4.1/src/clevertable/Map.py` & `clevertable-2.5.0/src/clevertable/Map.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.4.1/src/clevertable/OneHot.py` & `clevertable-2.5.0/src/clevertable/OneHot.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.4.1/src/clevertable/Parallel.py` & `clevertable-2.5.0/src/clevertable/Parallel.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.4.1/src/clevertable/Pipeline.py` & `clevertable-2.5.0/src/clevertable/Pipeline.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.4.1/src/clevertable/RecordProfile.py` & `clevertable-2.5.0/src/clevertable/RecordProfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,21 @@
         """
         input_record = _check_and_unpack(row)
         output_record = {}
         for key in input_record:
             if key not in self.profile:
                 raise KeyError(f"Key not present in the profile: '{key}'")
             conv = self.profile[key]
-            out_vals: list = conv.transform([input_record[key]])
+            in_vals = [input_record[key]]
+            try:
+                out_vals: list = conv.transform(in_vals)
+            except Exception as e:
+                # add helpful context to error message
+                raise ValueError(f"Key '{key}': {conv.__class__.__name__} converter"
+                                 f" raised {e.__class__.__name__} during transform: {e}") from e
             out_keys = self.keys[key]
             assert len(out_vals) == len(out_keys), \
                 f"Key '{key}': Output length of {conv.__class__.__name__} converter" \
                 f" mismatches number of labels: {len(out_vals)}!={len(out_keys)}." \
                 f"\n\tInput:\t{[input_record[key]]}" \
                 f"\n\tOutput (length {len(out_vals)}):\t{out_vals}" \
                 f"\n\tOutput Labels (length {len(out_keys)}):\t{out_keys}"
```

### Comparing `clevertable-2.4.1/src/clevertable/Split.py` & `clevertable-2.5.0/src/clevertable/Split.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.4.1/src/clevertable/StrictFunction.py` & `clevertable-2.5.0/src/clevertable/StrictFunction.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.4.1/src/clevertable/Strip.py` & `clevertable-2.5.0/src/clevertable/Strip.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.4.1/src/clevertable/Transpose.py` & `clevertable-2.5.0/src/clevertable/Transpose.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.4.1/src/clevertable/Try.py` & `clevertable-2.5.0/src/clevertable/Try.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.4.1/src/clevertable/__init__.py` & `clevertable-2.5.0/src/clevertable/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "2.4.1"
+__version__ = "2.5.0"
 
 from .Binary import Binary
 from .Const import Const
 from .ConversionProfile import ConversionProfile
 from .Converter import Converter
 from .Enumerate import Enumerate
 from .Flatten import Flatten
```

### Comparing `clevertable-2.4.1/src/clevertable/__main__.py` & `clevertable-2.5.0/src/clevertable/__main__.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.4.1/src/clevertable/_utils.py` & `clevertable-2.5.0/src/clevertable/_utils.py`

 * *Files identical despite different names*

### Comparing `clevertable-2.4.1/src/clevertable.egg-info/PKG-INFO` & `clevertable-2.5.0/src/clevertable.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clevertable
-Version: 2.4.1
+Version: 2.5.0
 Summary: Low effort conversion of tabular data into numerical values.
 Author: Tom Mohr
 License: MIT License
         
         Copyright (c) 2023 Tom Mohr
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `clevertable-2.4.1/src/clevertable.egg-info/SOURCES.txt` & `clevertable-2.5.0/src/clevertable.egg-info/SOURCES.txt`

 * *Files identical despite different names*

