# Comparing `tmp/searchkit-0.2.6.tar.gz` & `tmp/searchkit-0.2.6.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "searchkit-0.2.6.tar", last modified: Wed May 24 11:46:36 2023, max compression
+gzip compressed data, was "searchkit-0.2.6.post2.tar", last modified: Wed May 24 13:54:11 2023, max compression
```

## Comparing `searchkit-0.2.6.tar` & `searchkit-0.2.6.post2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-05-24 11:46:36.675693 searchkit-0.2.6/
--rw-rw-r--   0 user1     (1000) user1     (1000)    11357 2023-01-10 10:19:33.000000 searchkit-0.2.6/LICENSE
--rw-rw-r--   0 user1     (1000) user1     (1000)     4352 2023-05-24 11:46:36.675693 searchkit-0.2.6/PKG-INFO
--rw-rw-r--   0 user1     (1000) user1     (1000)     4144 2023-05-24 11:46:12.000000 searchkit-0.2.6/README.md
--rw-rw-r--   0 user1     (1000) user1     (1000)      734 2023-05-18 09:56:58.000000 searchkit-0.2.6/pyproject.toml
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-05-24 11:46:36.675693 searchkit-0.2.6/searchkit/
--rw-rw-r--   0 user1     (1000) user1     (1000)      121 2023-05-22 10:26:50.000000 searchkit-0.2.6/searchkit/__init__.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    29452 2023-05-24 11:46:12.000000 searchkit-0.2.6/searchkit/constraints.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      277 2023-01-29 21:35:16.000000 searchkit-0.2.6/searchkit/log.py
--rwxrwxr-x   0 user1     (1000) user1     (1000)    49277 2023-05-22 09:42:32.000000 searchkit-0.2.6/searchkit/search.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     5726 2023-05-16 10:48:26.000000 searchkit-0.2.6/searchkit/utils.py
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-05-24 11:46:36.675693 searchkit-0.2.6/searchkit.egg-info/
--rw-rw-r--   0 user1     (1000) user1     (1000)     4352 2023-05-24 11:46:36.000000 searchkit-0.2.6/searchkit.egg-info/PKG-INFO
--rw-rw-r--   0 user1     (1000) user1     (1000)      308 2023-05-24 11:46:36.000000 searchkit-0.2.6/searchkit.egg-info/SOURCES.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)        1 2023-05-24 11:46:36.000000 searchkit-0.2.6/searchkit.egg-info/dependency_links.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)       57 2023-05-24 11:46:36.000000 searchkit-0.2.6/searchkit.egg-info/requires.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)       10 2023-05-24 11:46:36.000000 searchkit-0.2.6/searchkit.egg-info/top_level.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)       38 2023-05-24 11:46:36.675693 searchkit-0.2.6/setup.cfg
--rw-rw-r--   0 user1     (1000) user1     (1000)       54 2023-01-29 21:35:16.000000 searchkit-0.2.6/setup.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-05-24 13:54:11.266769 searchkit-0.2.6.post2/
+-rw-rw-r--   0 user1     (1000) user1     (1000)    11357 2023-01-10 10:19:33.000000 searchkit-0.2.6.post2/LICENSE
+-rw-rw-r--   0 user1     (1000) user1     (1000)     4419 2023-05-24 13:54:11.266769 searchkit-0.2.6.post2/PKG-INFO
+-rw-rw-r--   0 user1     (1000) user1     (1000)     4205 2023-05-24 13:53:26.000000 searchkit-0.2.6.post2/README.md
+-rw-rw-r--   0 user1     (1000) user1     (1000)      734 2023-05-18 09:56:58.000000 searchkit-0.2.6.post2/pyproject.toml
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-05-24 13:54:11.266769 searchkit-0.2.6.post2/searchkit/
+-rw-rw-r--   0 user1     (1000) user1     (1000)      121 2023-05-22 10:26:50.000000 searchkit-0.2.6.post2/searchkit/__init__.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    29452 2023-05-24 11:46:12.000000 searchkit-0.2.6.post2/searchkit/constraints.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      277 2023-01-29 21:35:16.000000 searchkit-0.2.6.post2/searchkit/log.py
+-rwxrwxr-x   0 user1     (1000) user1     (1000)    49277 2023-05-22 09:42:32.000000 searchkit-0.2.6.post2/searchkit/search.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     5726 2023-05-16 10:48:26.000000 searchkit-0.2.6.post2/searchkit/utils.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-05-24 13:54:11.266769 searchkit-0.2.6.post2/searchkit.egg-info/
+-rw-rw-r--   0 user1     (1000) user1     (1000)     4419 2023-05-24 13:54:11.000000 searchkit-0.2.6.post2/searchkit.egg-info/PKG-INFO
+-rw-rw-r--   0 user1     (1000) user1     (1000)      308 2023-05-24 13:54:11.000000 searchkit-0.2.6.post2/searchkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)        1 2023-05-24 13:54:11.000000 searchkit-0.2.6.post2/searchkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)       57 2023-05-24 13:54:11.000000 searchkit-0.2.6.post2/searchkit.egg-info/requires.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)       10 2023-05-24 13:54:11.000000 searchkit-0.2.6.post2/searchkit.egg-info/top_level.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)       38 2023-05-24 13:54:11.266769 searchkit-0.2.6.post2/setup.cfg
+-rw-rw-r--   0 user1     (1000) user1     (1000)       54 2023-01-29 21:35:16.000000 searchkit-0.2.6.post2/setup.py
```

### Comparing `searchkit-0.2.6/LICENSE` & `searchkit-0.2.6.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `searchkit-0.2.6/PKG-INFO` & `searchkit-0.2.6.post2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchkit
-Version: 0.2.6
+Version: 0.2.6.post2
 Summary: Python library providing tools to search files in parallel.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Searchkit
 
@@ -125,28 +125,30 @@
             print(r.get(0))
 ```
 
 An example search with constraints is as follows:
 
 ```python
 from searchkit import FileSearcher, SearchDef
-from searchkit.constraints import SearchConstraintSearchSince, DateTimeMatcherBase
+from searchkit.constraints import SearchConstraintSearchSince, TimestampMatcherBase
 
-class MyDateTimeMatcher(DateTimeMatcherBase):
-    EXPRS = [r'^(?P<year>\d{4})-(?P<month>\d{2})-(?P<day>\d{2}) '
-             r'(?P<hours>\d{2}):(?P<minutes>\d{2}):(?P<seconds>\d{2})']
+class MyDateTimeMatcher(TimestampMatcherBase):
+    @property
+    def patterns(self):
+        return [r'^(?P<year>\d{4})-(?P<month>\d{2})-(?P<day>\d{2}) '
+                r'(?P<hours>\d{2}):(?P<minutes>\d{2}):(?P<seconds>\d{2})']
 
 fname = 'foo.txt'
 with open(fname, 'w') as fd:
   fd.write('2023-01-01 12:34:24 feeling cold\n')
   fd.write('2023-06-01 12:34:24 feeling hot')
 
 today = '2023-06-02 12:34:24'
 constraint = SearchConstraintSearchSince(today, None,
-                                         MyDateTimeMatcher)
+                                         ts_matcher_cls=MyDateTimeMatcher)
 fs = FileSearcher(constraint=constraint)
 fs.add(SearchDef(r'\S+ \S+ \S+ (\S+)'), fname)
 results = fs.run()
 for r in results.find_by_path(fname):
     print(r.get(1) == 'hot')
 ```
```

### Comparing `searchkit-0.2.6/README.md` & `searchkit-0.2.6.post2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -117,28 +117,30 @@
             print(r.get(0))
 ```
 
 An example search with constraints is as follows:
 
 ```python
 from searchkit import FileSearcher, SearchDef
-from searchkit.constraints import SearchConstraintSearchSince, DateTimeMatcherBase
+from searchkit.constraints import SearchConstraintSearchSince, TimestampMatcherBase
 
-class MyDateTimeMatcher(DateTimeMatcherBase):
-    EXPRS = [r'^(?P<year>\d{4})-(?P<month>\d{2})-(?P<day>\d{2}) '
-             r'(?P<hours>\d{2}):(?P<minutes>\d{2}):(?P<seconds>\d{2})']
+class MyDateTimeMatcher(TimestampMatcherBase):
+    @property
+    def patterns(self):
+        return [r'^(?P<year>\d{4})-(?P<month>\d{2})-(?P<day>\d{2}) '
+                r'(?P<hours>\d{2}):(?P<minutes>\d{2}):(?P<seconds>\d{2})']
 
 fname = 'foo.txt'
 with open(fname, 'w') as fd:
   fd.write('2023-01-01 12:34:24 feeling cold\n')
   fd.write('2023-06-01 12:34:24 feeling hot')
 
 today = '2023-06-02 12:34:24'
 constraint = SearchConstraintSearchSince(today, None,
-                                         MyDateTimeMatcher)
+                                         ts_matcher_cls=MyDateTimeMatcher)
 fs = FileSearcher(constraint=constraint)
 fs.add(SearchDef(r'\S+ \S+ \S+ (\S+)'), fname)
 results = fs.run()
 for r in results.find_by_path(fname):
     print(r.get(1) == 'hot')
 ```
```

### Comparing `searchkit-0.2.6/pyproject.toml` & `searchkit-0.2.6.post2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `searchkit-0.2.6/searchkit/constraints.py` & `searchkit-0.2.6.post2/searchkit/constraints.py`

 * *Files identical despite different names*

### Comparing `searchkit-0.2.6/searchkit/search.py` & `searchkit-0.2.6.post2/searchkit/search.py`

 * *Files identical despite different names*

### Comparing `searchkit-0.2.6/searchkit/utils.py` & `searchkit-0.2.6.post2/searchkit/utils.py`

 * *Files identical despite different names*

### Comparing `searchkit-0.2.6/searchkit.egg-info/PKG-INFO` & `searchkit-0.2.6.post2/searchkit.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchkit
-Version: 0.2.6
+Version: 0.2.6.post2
 Summary: Python library providing tools to search files in parallel.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Searchkit
 
@@ -125,28 +125,30 @@
             print(r.get(0))
 ```
 
 An example search with constraints is as follows:
 
 ```python
 from searchkit import FileSearcher, SearchDef
-from searchkit.constraints import SearchConstraintSearchSince, DateTimeMatcherBase
+from searchkit.constraints import SearchConstraintSearchSince, TimestampMatcherBase
 
-class MyDateTimeMatcher(DateTimeMatcherBase):
-    EXPRS = [r'^(?P<year>\d{4})-(?P<month>\d{2})-(?P<day>\d{2}) '
-             r'(?P<hours>\d{2}):(?P<minutes>\d{2}):(?P<seconds>\d{2})']
+class MyDateTimeMatcher(TimestampMatcherBase):
+    @property
+    def patterns(self):
+        return [r'^(?P<year>\d{4})-(?P<month>\d{2})-(?P<day>\d{2}) '
+                r'(?P<hours>\d{2}):(?P<minutes>\d{2}):(?P<seconds>\d{2})']
 
 fname = 'foo.txt'
 with open(fname, 'w') as fd:
   fd.write('2023-01-01 12:34:24 feeling cold\n')
   fd.write('2023-06-01 12:34:24 feeling hot')
 
 today = '2023-06-02 12:34:24'
 constraint = SearchConstraintSearchSince(today, None,
-                                         MyDateTimeMatcher)
+                                         ts_matcher_cls=MyDateTimeMatcher)
 fs = FileSearcher(constraint=constraint)
 fs.add(SearchDef(r'\S+ \S+ \S+ (\S+)'), fname)
 results = fs.run()
 for r in results.find_by_path(fname):
     print(r.get(1) == 'hot')
 ```
```

