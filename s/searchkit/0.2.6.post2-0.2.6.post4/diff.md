# Comparing `tmp/searchkit-0.2.6.post2.tar.gz` & `tmp/searchkit-0.2.6.post4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "searchkit-0.2.6.post2.tar", last modified: Wed May 24 13:54:11 2023, max compression
+gzip compressed data, was "searchkit-0.2.6.post4.tar", last modified: Thu May 25 13:52:33 2023, max compression
```

## Comparing `searchkit-0.2.6.post2.tar` & `searchkit-0.2.6.post4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-05-24 13:54:11.266769 searchkit-0.2.6.post2/
--rw-rw-r--   0 user1     (1000) user1     (1000)    11357 2023-01-10 10:19:33.000000 searchkit-0.2.6.post2/LICENSE
--rw-rw-r--   0 user1     (1000) user1     (1000)     4419 2023-05-24 13:54:11.266769 searchkit-0.2.6.post2/PKG-INFO
--rw-rw-r--   0 user1     (1000) user1     (1000)     4205 2023-05-24 13:53:26.000000 searchkit-0.2.6.post2/README.md
--rw-rw-r--   0 user1     (1000) user1     (1000)      734 2023-05-18 09:56:58.000000 searchkit-0.2.6.post2/pyproject.toml
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-05-24 13:54:11.266769 searchkit-0.2.6.post2/searchkit/
--rw-rw-r--   0 user1     (1000) user1     (1000)      121 2023-05-22 10:26:50.000000 searchkit-0.2.6.post2/searchkit/__init__.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    29452 2023-05-24 11:46:12.000000 searchkit-0.2.6.post2/searchkit/constraints.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      277 2023-01-29 21:35:16.000000 searchkit-0.2.6.post2/searchkit/log.py
--rwxrwxr-x   0 user1     (1000) user1     (1000)    49277 2023-05-22 09:42:32.000000 searchkit-0.2.6.post2/searchkit/search.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     5726 2023-05-16 10:48:26.000000 searchkit-0.2.6.post2/searchkit/utils.py
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-05-24 13:54:11.266769 searchkit-0.2.6.post2/searchkit.egg-info/
--rw-rw-r--   0 user1     (1000) user1     (1000)     4419 2023-05-24 13:54:11.000000 searchkit-0.2.6.post2/searchkit.egg-info/PKG-INFO
--rw-rw-r--   0 user1     (1000) user1     (1000)      308 2023-05-24 13:54:11.000000 searchkit-0.2.6.post2/searchkit.egg-info/SOURCES.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)        1 2023-05-24 13:54:11.000000 searchkit-0.2.6.post2/searchkit.egg-info/dependency_links.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)       57 2023-05-24 13:54:11.000000 searchkit-0.2.6.post2/searchkit.egg-info/requires.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)       10 2023-05-24 13:54:11.000000 searchkit-0.2.6.post2/searchkit.egg-info/top_level.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)       38 2023-05-24 13:54:11.266769 searchkit-0.2.6.post2/setup.cfg
--rw-rw-r--   0 user1     (1000) user1     (1000)       54 2023-01-29 21:35:16.000000 searchkit-0.2.6.post2/setup.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-05-25 13:52:33.119709 searchkit-0.2.6.post4/
+-rw-rw-r--   0 user1     (1000) user1     (1000)    11357 2023-01-10 10:19:33.000000 searchkit-0.2.6.post4/LICENSE
+-rw-rw-r--   0 user1     (1000) user1     (1000)     4419 2023-05-25 13:52:33.119709 searchkit-0.2.6.post4/PKG-INFO
+-rw-rw-r--   0 user1     (1000) user1     (1000)     4205 2023-05-24 13:53:26.000000 searchkit-0.2.6.post4/README.md
+-rw-rw-r--   0 user1     (1000) user1     (1000)      734 2023-05-18 09:56:58.000000 searchkit-0.2.6.post4/pyproject.toml
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-05-25 13:52:33.119709 searchkit-0.2.6.post4/searchkit/
+-rw-rw-r--   0 user1     (1000) user1     (1000)      121 2023-05-22 10:26:50.000000 searchkit-0.2.6.post4/searchkit/__init__.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    29452 2023-05-24 11:46:12.000000 searchkit-0.2.6.post4/searchkit/constraints.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      277 2023-01-29 21:35:16.000000 searchkit-0.2.6.post4/searchkit/log.py
+-rwxrwxr-x   0 user1     (1000) user1     (1000)    49612 2023-05-25 13:52:19.000000 searchkit-0.2.6.post4/searchkit/search.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     5726 2023-05-16 10:48:26.000000 searchkit-0.2.6.post4/searchkit/utils.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-05-25 13:52:33.119709 searchkit-0.2.6.post4/searchkit.egg-info/
+-rw-rw-r--   0 user1     (1000) user1     (1000)     4419 2023-05-25 13:52:33.000000 searchkit-0.2.6.post4/searchkit.egg-info/PKG-INFO
+-rw-rw-r--   0 user1     (1000) user1     (1000)      308 2023-05-25 13:52:33.000000 searchkit-0.2.6.post4/searchkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)        1 2023-05-25 13:52:33.000000 searchkit-0.2.6.post4/searchkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)       57 2023-05-25 13:52:33.000000 searchkit-0.2.6.post4/searchkit.egg-info/requires.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)       10 2023-05-25 13:52:33.000000 searchkit-0.2.6.post4/searchkit.egg-info/top_level.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)       38 2023-05-25 13:52:33.119709 searchkit-0.2.6.post4/setup.cfg
+-rw-rw-r--   0 user1     (1000) user1     (1000)       54 2023-01-29 21:35:16.000000 searchkit-0.2.6.post4/setup.py
```

### Comparing `searchkit-0.2.6.post2/LICENSE` & `searchkit-0.2.6.post4/LICENSE`

 * *Files identical despite different names*

### Comparing `searchkit-0.2.6.post2/PKG-INFO` & `searchkit-0.2.6.post4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchkit
-Version: 0.2.6.post2
+Version: 0.2.6.post4
 Summary: Python library providing tools to search files in parallel.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Searchkit
```

### Comparing `searchkit-0.2.6.post2/README.md` & `searchkit-0.2.6.post4/README.md`

 * *Files identical despite different names*

### Comparing `searchkit-0.2.6.post2/pyproject.toml` & `searchkit-0.2.6.post4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `searchkit-0.2.6.post2/searchkit/constraints.py` & `searchkit-0.2.6.post4/searchkit/constraints.py`

 * *Files identical despite different names*

### Comparing `searchkit-0.2.6.post2/searchkit/search.py` & `searchkit-0.2.6.post4/searchkit/search.py`

 * *Files 0% similar despite different names*

```diff
@@ -1025,15 +1025,16 @@
         stats = SearchTaskStats()
         path = self.info['path']
         if os.path.getsize(path) == 0:
             log.debug("filesearcher: zero-length file %s - skipping search",
                       path)
             return stats
 
-        log.debug("starting execution on path %s", path)
+        log.debug("starting execution on path %s (searches=%s)", path,
+                  len(self.search_defs))
         try:
             # first assume compressed then plain
             with gzip.open(path, 'rb') as fd:
                 try:
                     # test if file is gzip
                     fd.read(1)
                     fd.seek(0)
@@ -1063,28 +1064,31 @@
 
 class SearchTaskStats(UserDict):
 
     def __init__(self):
         self.reset()
 
     def reset(self):
-        self.data = {'lines_searched': 0,
+        self.data = {'searches': 0,
+                     'searches_by_job': [],
+                     'lines_searched': 0,
                      'jobs_completed': 0,
                      'total_jobs': 0,
-                     'results': 0}
+                     'results': 0,
+                     'num_deduped': 0}
 
     def update(self, stats):
         if not stats:
             return
 
         for key, val in stats.items():
             self.data[key] += val
 
     def __repr__(self):
-        return str(self.data)
+        return ', '.join([f"{k}={v}" for k, v in self.data.items()])
 
 
 class SearcherBase(abc.ABC):
 
     @abc.abstractproperty
     def files(self):
         """ Returns a list of files we will be searching. """
@@ -1397,14 +1401,18 @@
         """
         log.debug("filesearcher: starting")
         self.stats.reset()
         if len(self.catalog) == 0:
             log.debug("catalog is empty - nothing to run")
             return SearchResultsCollection(self.catalog, ResultStoreSimple())
 
+        self.stats['searches'] = sum([len(p['searches'])
+                                      for p in self.catalog])
+        self.stats['searches_by_job'] = [len(p['searches'])
+                                         for p in self.catalog]
         if len(self.files) > 1:
             log.debug("running searches (parallel=True)")
             with multiprocessing.Manager() as mgr:
                 rs = ResultStoreParallel(mgr)
                 results = SearchResultsCollection(self.catalog, rs)
                 self._run_mp(mgr, results, rs)
                 self.stats['num_deduped'] = rs.num_deduped
@@ -1412,11 +1420,9 @@
         else:
             log.debug("running searches (parallel=False)")
             rs = ResultStoreSimple()
             results = SearchResultsCollection(self.catalog, rs)
             self._run_single(results, rs)
             self.stats['num_deduped'] = rs.num_deduped
 
-        log.debug("filesearcher: stats=%s", self.stats)
-        log.debug("filesearcher: completed (results=%s, dedup=%s)",
-                  len(results), self.stats['num_deduped'])
+        log.debug("filesearcher: completed (%s)", self.stats)
         return results
```

### Comparing `searchkit-0.2.6.post2/searchkit/utils.py` & `searchkit-0.2.6.post4/searchkit/utils.py`

 * *Files identical despite different names*

### Comparing `searchkit-0.2.6.post2/searchkit.egg-info/PKG-INFO` & `searchkit-0.2.6.post4/searchkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchkit
-Version: 0.2.6.post2
+Version: 0.2.6.post4
 Summary: Python library providing tools to search files in parallel.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Searchkit
```

