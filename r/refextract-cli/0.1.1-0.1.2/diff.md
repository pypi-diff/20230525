# Comparing `tmp/refextract_cli-0.1.1.tar.gz` & `tmp/refextract_cli-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refextract_cli-0.1.1.tar", last modified: Thu Apr 27 18:17:56 2023, max compression
+gzip compressed data, was "refextract_cli-0.1.2.tar", last modified: Thu May 25 19:38:11 2023, max compression
```

## Comparing `refextract_cli-0.1.1.tar` & `refextract_cli-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 lsmeni    (1000) lsmeni    (1000)        0 2023-04-27 18:17:56.533832 refextract_cli-0.1.1/
--rw-r--r--   0 lsmeni    (1000) lsmeni    (1000)    17711 2023-04-26 21:41:12.000000 refextract_cli-0.1.1/LICENSE
--rw-r--r--   0 lsmeni    (1000) lsmeni    (1000)      761 2023-04-27 18:17:56.533832 refextract_cli-0.1.1/PKG-INFO
--rw-r--r--   0 lsmeni    (1000) lsmeni    (1000)      593 2023-04-26 22:00:54.000000 refextract_cli-0.1.1/README.md
--rw-r--r--   0 lsmeni    (1000) lsmeni    (1000)      216 2023-04-27 18:16:47.000000 refextract_cli-0.1.1/pyproject.toml
-drwxr-xr-x   0 lsmeni    (1000) lsmeni    (1000)        0 2023-04-27 18:17:56.530499 refextract_cli-0.1.1/refextract_cli/
--rw-r--r--   0 lsmeni    (1000) lsmeni    (1000)        0 2023-04-26 21:18:14.000000 refextract_cli-0.1.1/refextract_cli/__init__.py
--rwxr-xr-x   0 lsmeni    (1000) lsmeni    (1000)     7143 2023-04-27 18:13:29.000000 refextract_cli-0.1.1/refextract_cli/cli.py
-drwxr-xr-x   0 lsmeni    (1000) lsmeni    (1000)        0 2023-04-27 18:17:56.533832 refextract_cli-0.1.1/refextract_cli.egg-info/
--rw-r--r--   0 lsmeni    (1000) lsmeni    (1000)      761 2023-04-27 18:17:56.000000 refextract_cli-0.1.1/refextract_cli.egg-info/PKG-INFO
--rw-r--r--   0 lsmeni    (1000) lsmeni    (1000)      320 2023-04-27 18:17:56.000000 refextract_cli-0.1.1/refextract_cli.egg-info/SOURCES.txt
--rw-r--r--   0 lsmeni    (1000) lsmeni    (1000)        1 2023-04-27 18:17:56.000000 refextract_cli-0.1.1/refextract_cli.egg-info/dependency_links.txt
--rw-r--r--   0 lsmeni    (1000) lsmeni    (1000)       50 2023-04-27 18:17:56.000000 refextract_cli-0.1.1/refextract_cli.egg-info/entry_points.txt
--rw-r--r--   0 lsmeni    (1000) lsmeni    (1000)       31 2023-04-27 18:17:56.000000 refextract_cli-0.1.1/refextract_cli.egg-info/requires.txt
--rw-r--r--   0 lsmeni    (1000) lsmeni    (1000)       15 2023-04-27 18:17:56.000000 refextract_cli-0.1.1/refextract_cli.egg-info/top_level.txt
--rw-r--r--   0 lsmeni    (1000) lsmeni    (1000)       38 2023-04-27 18:17:56.533832 refextract_cli-0.1.1/setup.cfg
--rw-r--r--   0 lsmeni    (1000) lsmeni    (1000)      307 2023-04-26 21:47:00.000000 refextract_cli-0.1.1/setup.py
+drwxr-xr-x   0 lsmeni    (1000) lsmeni    (1000)        0 2023-05-25 19:38:11.602741 refextract_cli-0.1.2/
+-rw-r--r--   0 lsmeni    (1000) lsmeni    (1000)    17711 2023-04-26 21:41:12.000000 refextract_cli-0.1.2/LICENSE
+-rw-r--r--   0 lsmeni    (1000) lsmeni    (1000)      761 2023-05-25 19:38:11.602741 refextract_cli-0.1.2/PKG-INFO
+-rw-r--r--   0 lsmeni    (1000) lsmeni    (1000)      593 2023-04-26 22:00:54.000000 refextract_cli-0.1.2/README.md
+-rw-r--r--   0 lsmeni    (1000) lsmeni    (1000)      216 2023-05-25 19:37:58.000000 refextract_cli-0.1.2/pyproject.toml
+drwxr-xr-x   0 lsmeni    (1000) lsmeni    (1000)        0 2023-05-25 19:38:11.599407 refextract_cli-0.1.2/refextract_cli/
+-rw-r--r--   0 lsmeni    (1000) lsmeni    (1000)        0 2023-04-26 21:18:14.000000 refextract_cli-0.1.2/refextract_cli/__init__.py
+-rwxr-xr-x   0 lsmeni    (1000) lsmeni    (1000)     9400 2023-05-25 19:37:12.000000 refextract_cli-0.1.2/refextract_cli/cli.py
+drwxr-xr-x   0 lsmeni    (1000) lsmeni    (1000)        0 2023-05-25 19:38:11.602741 refextract_cli-0.1.2/refextract_cli.egg-info/
+-rw-r--r--   0 lsmeni    (1000) lsmeni    (1000)      761 2023-05-25 19:38:11.000000 refextract_cli-0.1.2/refextract_cli.egg-info/PKG-INFO
+-rw-r--r--   0 lsmeni    (1000) lsmeni    (1000)      320 2023-05-25 19:38:11.000000 refextract_cli-0.1.2/refextract_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 lsmeni    (1000) lsmeni    (1000)        1 2023-05-25 19:38:11.000000 refextract_cli-0.1.2/refextract_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 lsmeni    (1000) lsmeni    (1000)       50 2023-05-25 19:38:11.000000 refextract_cli-0.1.2/refextract_cli.egg-info/entry_points.txt
+-rw-r--r--   0 lsmeni    (1000) lsmeni    (1000)       31 2023-05-25 19:38:11.000000 refextract_cli-0.1.2/refextract_cli.egg-info/requires.txt
+-rw-r--r--   0 lsmeni    (1000) lsmeni    (1000)       15 2023-05-25 19:38:11.000000 refextract_cli-0.1.2/refextract_cli.egg-info/top_level.txt
+-rw-r--r--   0 lsmeni    (1000) lsmeni    (1000)       38 2023-05-25 19:38:11.602741 refextract_cli-0.1.2/setup.cfg
+-rw-r--r--   0 lsmeni    (1000) lsmeni    (1000)      307 2023-04-26 21:47:00.000000 refextract_cli-0.1.2/setup.py
```

### Comparing `refextract_cli-0.1.1/LICENSE` & `refextract_cli-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `refextract_cli-0.1.1/PKG-INFO` & `refextract_cli-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refextract_cli
-Version: 0.1.1
+Version: 0.1.2
 Summary: Command line interface for refextract
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ```refex```
 
 The refexence Extractor is a command-line interface (CLI) application that uses [refextract](https://github.com/inspirehep/refextract) to extract references from a PDF file. The PDF file can be open on Okular or provided as a file path or URL.
```

### Comparing `refextract_cli-0.1.1/README.md` & `refextract_cli-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `refextract_cli-0.1.1/refextract_cli/cli.py` & `refextract_cli-0.1.2/refextract_cli/cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,75 @@
 #!/usr/bin/python3
 import refextract
 import argparse
 import urllib.parse
 import shutil
+import sqlite3
+import hashlib
+import json
 
-from rich import print
+from rich import print, traceback
+from pathlib import Path
 
 # Constants
 URL_ESCAPE_CHARACTERS = r'/:&=?~#+!$,;\'@()*[]'
+DB_PATH = Path.home() / '.config' / 'refextract' / 'references-cache.db'
+MAX_CACHE_SIZE = 200
+
+# sqlite3 cache class
+class RefCache:
+    def __init__(self, db_path):
+        self.db_path = db_path
+
+    def __enter__(self):
+        self.conn = sqlite3.connect(self.db_path)
+        self.conn.row_factory = sqlite3.Row
+        self.cursor = self.conn.cursor()
+        return self 
+
+    def __exit__(self, exc_type, exc_value, traceback):
+        self.conn.commit()
+        self.conn.close()
+
+    def get(self, checksum):
+        self.cursor.execute('SELECT * FROM pdf_refs WHERE checksum = ?', (checksum,))
+        return self.cursor.fetchone()
+
+    def insert(self, checksum, references):
+        # check if cache is full
+        self.cursor.execute('SELECT COUNT(*) FROM pdf_refs')
+        count = self.cursor.fetchone()[0]
+        if count >= MAX_CACHE_SIZE:
+            self.cursor.execute('DELETE FROM pdf_refs WHERE timestamp = (SELECT MIN(timestamp) FROM pdf_refs)')
+
+        self.cursor.execute('INSERT INTO pdf_refs (checksum, refs) VALUES (?, ?)', (checksum, references))
+
+    @staticmethod
+    def create_db(db_path):
+        Path(db_path).parent.mkdir(parents=True, exist_ok=True)
+        conn = sqlite3.connect(db_path)
+        conn.execute('CREATE TABLE IF NOT EXISTS pdf_refs (checksum TEXT PRIMARY KEY, refs TEXT, timestamp DATETIME DEFAULT CURRENT_TIMESTAMP)')
+        conn.commit()
+        conn.close()
+
+        return RefCache(db_path)
+
+# file checksum shorthand (md5)
+def file_checksum(file_path):
+    with open(file_path, 'rb') as f:
+        return hashlib.md5(f.read()).hexdigest()
+
+cache = None
+try:
+    cache = RefCache.create_db(DB_PATH)
+    print(f'Using cache database at {DB_PATH}')
+except Exception as e:
+    print("Couldn't open cache database")
+    traceback.pretty.pprint(e)
+
 
 def main():
     # Parse arguments
     parser = argparse.ArgumentParser(description='Extract references from a source or from the current opened PDF.\n Supported viewers: Okular')
 
     parser.add_argument('source', metavar='source', type=str, help='The source to extract references from. Accepts path to PDF or URL.', nargs='?')
 
@@ -95,14 +153,22 @@
     return opened_files[choice]
 
 
 # Check the source type
 def get_references(source, sort_key=None):
     references = []
 
+    # Check cache
+    if cache:
+        checksum = file_checksum(source)
+        with cache as c:
+            cached = c.get(checksum)
+            if cached:
+                return json.loads(cached['refs'])
+
     # Handle url
     if source.startswith('http'):
         references = refextract.extract_references_from_url(source)
     # Handle file
     elif source.endswith('.pdf'):
         references = refextract.extract_references_from_file(source)
     else:
@@ -131,14 +197,20 @@
         
         k += 1
     
     # sort references
     if sort_key:
         references.sort(key=lambda k: k.get(sort_key, [''])[0])
 
+    # save to cache as json
+    if cache:
+        checksum = file_checksum(source)
+        with cache as c:
+            c.insert(checksum, json.dumps(references))
+
     return references
 
 def scholar_link(reference):
     author = ('author' in reference and ', '.join(reference['author'])) or '????'
     year = 'year' in reference and reference['year'][0] or '????'
     raw_ref = (reference['raw_ref'][0]) or '????'
     query_str = f'{raw_ref}'
```

### Comparing `refextract_cli-0.1.1/refextract_cli.egg-info/PKG-INFO` & `refextract_cli-0.1.2/refextract_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refextract-cli
-Version: 0.1.1
+Version: 0.1.2
 Summary: Command line interface for refextract
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ```refex```
 
 The refexence Extractor is a command-line interface (CLI) application that uses [refextract](https://github.com/inspirehep/refextract) to extract references from a PDF file. The PDF file can be open on Okular or provided as a file path or URL.
```

