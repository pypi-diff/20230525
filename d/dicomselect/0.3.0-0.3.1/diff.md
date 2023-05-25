# Comparing `tmp/dicomselect-0.3.0.tar.gz` & `tmp/dicomselect-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dicomselect-0.3.0.tar", last modified: Tue May 23 11:51:08 2023, max compression
+gzip compressed data, was "dicomselect-0.3.1.tar", last modified: Thu May 25 09:09:00 2023, max compression
```

## Comparing `dicomselect-0.3.0.tar` & `dicomselect-0.3.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 11:51:08.559170 dicomselect-0.3.0/
--rw-rw-rw-   0        0        0     1082 2023-04-26 08:15:15.000000 dicomselect-0.3.0/LICENSE
--rw-rw-rw-   0        0        0     2814 2023-05-23 11:51:08.559170 dicomselect-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     2045 2023-05-23 11:32:18.000000 dicomselect-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-23 11:51:08.527418 dicomselect-0.3.0/dicomselect/
--rw-rw-rw-   0        0        0      133 2023-05-23 11:44:09.000000 dicomselect-0.3.0/dicomselect/__init__.py
--rw-rw-rw-   0        0        0     1358 2023-05-09 08:19:32.000000 dicomselect-0.3.0/dicomselect/constants.py
--rw-rw-rw-   0        0        0    13063 2023-05-23 11:44:09.000000 dicomselect-0.3.0/dicomselect/convert.py
--rw-rw-rw-   0        0        0     9048 2023-05-23 11:44:09.000000 dicomselect-0.3.0/dicomselect/database.py
--rw-rw-rw-   0        0        0     2315 2023-05-09 15:05:34.000000 dicomselect-0.3.0/dicomselect/dicom.py
--rw-rw-rw-   0        0        0     1580 2023-05-23 11:32:18.000000 dicomselect-0.3.0/dicomselect/info.py
--rw-rw-rw-   0        0        0     6689 2023-05-09 09:17:00.000000 dicomselect-0.3.0/dicomselect/query.py
--rw-rw-rw-   0        0        0     2759 2023-05-09 09:17:00.000000 dicomselect-0.3.0/dicomselect/queryfactory.py
--rw-rw-rw-   0        0        0    15428 2023-05-23 11:32:18.000000 dicomselect-0.3.0/dicomselect/reader.py
--rw-rw-rw-   0        0        0   203115 2023-05-09 08:19:32.000000 dicomselect-0.3.0/dicomselect/tags_generated.py
-drwxrwxrwx   0        0        0        0 2023-05-23 11:51:08.543433 dicomselect-0.3.0/dicomselect.egg-info/
--rw-rw-rw-   0        0        0     2814 2023-05-23 11:51:08.000000 dicomselect-0.3.0/dicomselect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      826 2023-05-23 11:51:08.000000 dicomselect-0.3.0/dicomselect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 11:51:08.000000 dicomselect-0.3.0/dicomselect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-26 11:37:02.000000 dicomselect-0.3.0/dicomselect.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      263 2023-05-23 11:51:08.000000 dicomselect-0.3.0/dicomselect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-23 11:51:08.000000 dicomselect-0.3.0/dicomselect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      940 2023-05-23 11:51:08.574819 dicomselect-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0      669 2023-05-23 11:32:18.000000 dicomselect-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-23 11:51:08.559170 dicomselect-0.3.0/tests/
--rw-rw-rw-   0        0        0     1604 2023-05-23 11:44:09.000000 dicomselect-0.3.0/tests/test_convert.py
--rw-rw-rw-   0        0        0      903 2023-05-09 15:12:16.000000 dicomselect-0.3.0/tests/test_create.py
--rw-rw-rw-   0        0        0     2669 2023-05-09 15:11:33.000000 dicomselect-0.3.0/tests/test_select.py
--rw-rw-rw-   0        0        0      141 2023-05-09 15:06:15.000000 dicomselect-0.3.0/tests/test_version.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:09:00.420678 dicomselect-0.3.1/
+-rw-rw-rw-   0        0        0     1082 2023-04-26 08:15:15.000000 dicomselect-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0     2843 2023-05-25 09:09:00.420678 dicomselect-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2052 2023-05-25 08:23:38.000000 dicomselect-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 09:09:00.348995 dicomselect-0.3.1/dicomselect/
+-rw-rw-rw-   0        0        0      133 2023-05-25 08:23:38.000000 dicomselect-0.3.1/dicomselect/__init__.py
+-rw-rw-rw-   0        0        0     1358 2023-05-09 08:19:32.000000 dicomselect-0.3.1/dicomselect/constants.py
+-rw-rw-rw-   0        0        0    13160 2023-05-25 08:23:38.000000 dicomselect-0.3.1/dicomselect/convert.py
+-rw-rw-rw-   0        0        0     9082 2023-05-25 09:06:57.000000 dicomselect-0.3.1/dicomselect/database.py
+-rw-rw-rw-   0        0        0     2315 2023-05-25 08:23:38.000000 dicomselect-0.3.1/dicomselect/dicom.py
+-rw-rw-rw-   0        0        0     1580 2023-05-25 08:23:38.000000 dicomselect-0.3.1/dicomselect/info.py
+-rw-rw-rw-   0        0        0     6689 2023-05-25 08:23:38.000000 dicomselect-0.3.1/dicomselect/query.py
+-rw-rw-rw-   0        0        0     2759 2023-05-25 08:23:38.000000 dicomselect-0.3.1/dicomselect/queryfactory.py
+-rw-rw-rw-   0        0        0    16475 2023-05-25 09:06:57.000000 dicomselect-0.3.1/dicomselect/reader.py
+-rw-rw-rw-   0        0        0   203115 2023-05-09 08:19:32.000000 dicomselect-0.3.1/dicomselect/tags_generated.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:09:00.381799 dicomselect-0.3.1/dicomselect.egg-info/
+-rw-rw-rw-   0        0        0     2843 2023-05-25 09:09:00.000000 dicomselect-0.3.1/dicomselect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      826 2023-05-25 09:09:00.000000 dicomselect-0.3.1/dicomselect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 09:09:00.000000 dicomselect-0.3.1/dicomselect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-26 11:37:02.000000 dicomselect-0.3.1/dicomselect.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      263 2023-05-25 09:09:00.000000 dicomselect-0.3.1/dicomselect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-25 09:09:00.000000 dicomselect-0.3.1/dicomselect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      940 2023-05-25 09:09:00.422675 dicomselect-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      669 2023-05-25 08:23:38.000000 dicomselect-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:09:00.419688 dicomselect-0.3.1/tests/
+-rw-rw-rw-   0        0        0     1604 2023-05-25 08:23:38.000000 dicomselect-0.3.1/tests/test_convert.py
+-rw-rw-rw-   0        0        0      903 2023-05-25 08:23:38.000000 dicomselect-0.3.1/tests/test_create.py
+-rw-rw-rw-   0        0        0     2669 2023-05-25 08:23:38.000000 dicomselect-0.3.1/tests/test_select.py
+-rw-rw-rw-   0        0        0      141 2023-05-25 08:23:38.000000 dicomselect-0.3.1/tests/test_version.py
```

### Comparing `dicomselect-0.3.0/LICENSE` & `dicomselect-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dicomselect-0.3.0/PKG-INFO` & `dicomselect-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: dicomselect
-Version: 0.3.0
+Version: 0.3.1
+Summary: UNKNOWN
 Home-page: https://github.com/DIAGNijmegen/dicomselect
 Author: 
 Author-email: Stan.Noordman@radboudumc.nl
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/DIAGNijmegen/dicomselect
 Platform: unix
 Platform: linux
@@ -84,16 +85,20 @@
 
 # Show info
 ```python
 query.info().filter("series_description").print()
 ```
 
 # Convert
+
 ```python
 from dicomselect.database import Database
+
 db = Database('/path/to/dicomselect_archive.db')
 plan = db.plan('{patient_id}/{series_description}_{patient_age}', query)
 plan.target_dir = '/path/to/target_dir'
-plan.suffix = '.mha'
+plan.extension = '.mha'
 plan.print()
 plan.execute(max_workers=4)
 ```
+
+
```

### Comparing `dicomselect-0.3.0/README.md` & `dicomselect-0.3.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -60,16 +60,18 @@
 
 # Show info
 ```python
 query.info().filter("series_description").print()
 ```
 
 # Convert
+
 ```python
 from dicomselect.database import Database
+
 db = Database('/path/to/dicomselect_archive.db')
 plan = db.plan('{patient_id}/{series_description}_{patient_age}', query)
 plan.target_dir = '/path/to/target_dir'
-plan.suffix = '.mha'
+plan.extension = '.mha'
 plan.print()
 plan.execute(max_workers=4)
 ```
```

### Comparing `dicomselect-0.3.0/dicomselect/constants.py` & `dicomselect-0.3.1/dicomselect/constants.py`

 * *Files identical despite different names*

### Comparing `dicomselect-0.3.0/dicomselect/convert.py` & `dicomselect-0.3.1/dicomselect/convert.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import os
 import re
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from enum import Enum
-from pathlib import Path, WindowsPath
-from typing import Callable, Dict, List, Optional, Tuple, Any
+from pathlib import Path
+from typing import Callable, Dict, List, Optional, Tuple, Union
 
 import SimpleITK as sitk
 from tqdm import tqdm
 from treelib import Tree
 
 from dicomselect.reader import DICOMImageReader
 
@@ -22,21 +22,21 @@
 
 def load_plan(path: os.PathLike) -> "Plan":
     """Load a conversion plan from a json file."""
     path = Path(path)
     if path.is_dir():
         path = path / 'dicomselect_conversion_plan.json'
 
-    with open(path.with_suffix('.json'), 'r') as f:
+    with open(path, 'r') as f:
         plan_json = json.load(f)
 
     converts = [Convert(**json.loads(c), columns=[], values=[]) for c in plan_json['_converts']]
     plan = Plan(plan_json['source_dir'], converts)
     plan.target_dir = plan_json['target_dir']
-    plan.suffix = plan_json['suffix']
+    plan.extension = plan_json['suffix']
     plan.overwrite_existing = plan_json['overwrite_existing']
     plan.remove_existing = plan_json['remove_existing']
 
     return plan
 
 
 class Convert:
@@ -89,99 +89,97 @@
 class Plan:
     def __init__(self, default_source_dir: Path, converts: List[Convert]):
         self._converts = converts
 
         self._remove_existing: bool = False
         self._overwrite_existing: bool = False
         self._source_dir = default_source_dir
-        self._suffix = '.mha'
+        self._extension = '.mha'
         self._target_dir: Path = None
 
         self._missing: List[Path] = []
         self._mutation: Dict[str, Tuple[Mutation, Convert]] = dict()
-        self._dirty = True
+        self._invalidated = True
 
-    def _set_dirty(self, attr: str, value):
+    def _invalidate(self, attr: str, value):
         if getattr(self, attr) != value:
-            self._dirty = True
+            self._invalidated = True
 
     @property
     def source_dir(self) -> Path:
         """
         Source directory, containing your data that is to be converted.
         """
         return self._source_dir
 
     @source_dir.setter
     def source_dir(self, value: os.PathLike):
         value = Path(value).absolute()
         assert value.exists(), NotADirectoryError(f'{value} does not exist.')
         assert value.is_dir(), NotADirectoryError(f'{value} is not a directory.')
-        self._set_dirty('source_dir', value)
+        self._invalidate('source_dir', value)
         self._source_dir = value
 
     @property
     def target_dir(self) -> Path:
         """
         Target directory, to contain the converted data.
         """
         return self._target_dir
 
     @target_dir.setter
     def target_dir(self, value: os.PathLike):
         value = Path(value).absolute()
         assert value is not None, ValueError('target_dir is not set.')
         assert not value.exists() or value.is_dir(), NotADirectoryError(f'{value} is not a directory.')
-        self._set_dirty('target_dir', value)
+        self._invalidate('target_dir', value)
         self._target_dir = value
 
     @property
-    def suffix(self) -> str:
+    def extension(self) -> str:
         """
         The suffix defines the converted filetype. See https://simpleitk.readthedocs.io/en/master/IO.html#images
         for possible file formats to convert to.
         """
-        return self._suffix
+        return self._extension
 
-    @suffix.setter
-    def suffix(self, value: str):
+    @extension.setter
+    def extension(self, value: str):
         assert value.startswith('.'), ValueError('extension must start with a period.')
-        self._set_dirty('suffix', value)
-        self._suffix = value
+        self._invalidate('extension', value)
+        self._extension = value
 
     @property
     def remove_existing(self) -> bool:
         """
         Whether to remove any existing files in target_dir.
         """
         return self._remove_existing
 
     @remove_existing.setter
     def remove_existing(self, value: bool):
-        self._set_dirty('remove_existing', value)
+        self._invalidate('remove_existing', value)
         self._remove_existing = value
 
     @property
     def overwrite_existing(self) -> bool:
         """
         Whether to overwrite any existing files in target_dir that are the same.
         Files are considered the same if they share the same database key value and file name.
         """
         return self._overwrite_existing
 
     @overwrite_existing.setter
     def overwrite_existing(self, value: bool):
-        self._set_dirty('overwrite_existing', value)
+        self._invalidate('overwrite_existing', value)
         self._overwrite_existing = value
 
     def _update_mutations(self):
-        if not self._dirty:
+        if not self._invalidated:
             return
-        else:
-            self._dirty = False
 
         self.source_dir = self._source_dir  # performs a validation of source dir
         self.target_dir = self._target_dir  # performs a validation of target dir
 
         _dicomselect = self.target_dir / '.dicomselect'
         _dicomselect_dict = dict()
         try:
@@ -197,48 +195,51 @@
         except:
             print('.dicomselect file appears corrupt; overwrite_existing is forcibly set to True')
             self.overwrite_existing = True
             _dicomselect_dict.clear()
 
         self._mutation.clear()
         self._missing.clear()
-        for convert in tqdm(self._converts, desc=f"Preparing conversion plan..."):
+        for convert in tqdm(self._converts, desc=f"Preparing conversion plan"):
             source_exists = (self.source_dir / convert.source).exists()
-            target_exists = (self.target_dir / convert.target).with_suffix(self.suffix).exists()
+            target_exists = (self.target_dir / convert.target).with_suffix(self.extension).exists()
             if target_exists and convert.uid in _dicomselect_dict:
                 mutation_key = _dicomselect_dict[convert.uid].as_posix()
                 self._mutation[mutation_key] = (Mutation.OVERWRITE, convert)
             else:
                 i = 0
                 while True:
-                    target = f'{convert.target}_{i}{self.suffix}'
+                    target = f'{convert.target}_{i}{self.extension}'
                     if target not in self._mutation:
                         break
                     i += 1
                 mutation_key = Path(target).as_posix()
                 self._mutation[mutation_key] = (Mutation.NEW, convert)
             if not source_exists:
                 self._mutation[mutation_key] = (Mutation.MISSING, None)
                 self._missing.append(mutation_key)
 
         if self.remove_existing:
             # gather a list of files in target_dir that are not in the conversion plan
-            for root, directories, files in tqdm(os.walk(self.target_dir), desc=f"Checking existing files in {self.target_dir}..."):
+            print(f"Checking existing files in {self.target_dir}...")
+            for root, directories, files in tqdm(os.walk(self.target_dir), desc=f"Checking existing files"):
                 for fn in files:
                     filepath = (Path(root) / fn).relative_to(self.target_dir)
                     if filepath not in self._mutation and filepath.name != _dicomselect.name:
                         self._mutation[filepath.as_posix()] = (Mutation.REMOVE, None)
 
         mutation_list = list(self._mutation.items())
         for path, (mut, _) in mutation_list:
             del_overwrite = not self.overwrite_existing and mut == Mutation.OVERWRITE
             del_remove = not self.remove_existing and mut == Mutation.REMOVE
             if del_overwrite or del_remove:
                 self._mutation.pop(path)
 
+        self._invalidated = False
+
     def _tree(self) -> Tree:
         self._update_mutations()
 
         tree = Tree()
         root = tree.create_node('.', Path('.'))
         for path, (mut, _) in self._mutation.items():
             prev_parent = root
@@ -288,15 +289,15 @@
         self._update_mutations()
 
         path = Path(path)
         if path.is_dir():
             path = path / 'dicomselect_conversion_plan.json'
 
         plan = json.dumps({**self._parameters(), '_converts': self._converts}, default=self._serialize, indent=2)
-        with open(path.with_suffix('.json'), 'w') as f:
+        with open(path, 'w') as f:
             f.write(plan)
 
     def execute(self, max_workers: int = 4, postprocess_func: Optional[Callable[[sitk.Image], sitk.Image]] = None):
         """
         Execute the conversion plan.
 
         Parameters
@@ -305,27 +306,27 @@
             Max workers for the parallel process.
         postprocess_func:
             Postprocess function which takes a SimpleITK.Image and expects an output SimpleITK.Image, just prior to conversion.
         """
         self._update_mutations()
         errors = []
         _dicomselect = []
-        convert_args = (self.suffix, self.source_dir, self.target_dir, postprocess_func)
+        convert_args = (self.extension, self.source_dir, self.target_dir, postprocess_func)
 
         if not self.target_dir.exists():
             self.target_dir.mkdir(parents=True)
 
-        def _execute(path: Path, mutation: Mutation, convert: Convert):
+        def _execute(path: Path, mutation: Mutation, convert: Convert) -> Union[str, None]:
             if convert:
                 return convert.convert(*convert_args)
             elif mutation == Mutation.REMOVE:
                 os.remove(self.target_dir / path)
 
         print(f"Converting {len(self._converts)} DICOM series from {self.source_dir} to {self.target_dir}")
-        with tqdm(total=len(self._converts)) as pbar, ThreadPoolExecutor(max_workers=max_workers) as pool:
+        with tqdm(total=len(self._converts), desc=f"Converting to {self.extension}") as pbar, ThreadPoolExecutor(max_workers=max_workers) as pool:
             futures = [pool.submit(_execute, path, mut, convert) for path, (mut, convert) in self._mutation.items()]
             for future in as_completed(futures):
                 _dicomselect.append(future.result())
                 errors.append(future.exception())
                 pbar.update()
 
         with open(self.target_dir / '.dicomselect', 'w') as f:
```

### Comparing `dicomselect-0.3.0/dicomselect/database.py` & `dicomselect-0.3.1/dicomselect/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from tqdm import tqdm
 
 from dicomselect.convert import Convert, Plan
 from dicomselect.query import Query
 from dicomselect.queryfactory import QueryFactory
 from dicomselect.reader import DICOMImageReader
 
-database_version = '0.3.0'
+database_version = '0.4'
 
 
 class Database:
     def __init__(self, db_path: PathLike):
         self._db_path = Path(db_path).absolute()
         if self._db_path.is_dir() or self._db_path.suffix != '.db':
             raise IsADirectoryError('Provide a file path with as extension, .db')
@@ -72,21 +72,21 @@
         self._query_factory = QueryFactory(self._conn)
 
         return self._query_factory.create_query(None)
 
     def close(self):
         self._conn.close()
 
-    def plan(self, filepath: str, *queries: Query) -> Plan:
+    def plan(self, filepath_template: str, *queries: Query) -> Plan:
         """
         Prepare a conversion plan, which can convert the results of queries to MHA files.
 
         Parameters
         ----------
-        filepath: PathLike
+        filepath_template: PathLike
             Dictates the form of the directory and filename structure, omitting the suffix.
             Use braces along with column names to replace with that column value.
             Use forward slash to create a directory structure.
             (see Query.columns for a full list of available columns).
             A unique id will be appended at the end.
 
             Illegal characters will be replaced with '#'.
@@ -96,25 +96,25 @@
 
         Returns
         -------
         A conversion plan.
         """
         with self as query:
             cols = query.columns
-            requested_cols = [r.group(1) for r in re.finditer(r'{(.+?)}', filepath)]
+            requested_cols = [r.group(1) for r in re.finditer(r'{(.+?)}', filepath_template)]
             QueryFactory.check_if_exists('column', cols, *requested_cols)
 
             ids = set()
             for q in queries:
                 ids = ids.union(q._ids)
             self._conn.execute('CREATE TEMPORARY TABLE convert_ids (id INTEGER)')
             self._conn.executemany('INSERT INTO convert_ids (id) VALUES (?)', [(i,) for i in ids])
             converts_fetched = self._conn.execute(
                 f'SELECT dicomselect_uid, path, {", ".join(requested_cols)} FROM data JOIN convert_ids ON data.id = convert_ids.id').fetchall()
-            converts = [Convert(fetched[0], fetched[1], filepath, requested_cols, fetched[2:]) for fetched in converts_fetched]
+            converts = [Convert(fetched[0], fetched[1], filepath_template, requested_cols, fetched[2:]) for fetched in converts_fetched]
 
         return Plan(self.source_dir, converts)
 
     def create(self, data_dir: PathLike, max_workers: int = 4, *additional_dicom_tags: str):
         """
         Build a database from DICOMs in subdirectories of data_dir.
```

### Comparing `dicomselect-0.3.0/dicomselect/dicom.py` & `dicomselect-0.3.1/dicomselect/dicom.py`

 * *Files identical despite different names*

### Comparing `dicomselect-0.3.0/dicomselect/info.py` & `dicomselect-0.3.1/dicomselect/info.py`

 * *Files identical despite different names*

### Comparing `dicomselect-0.3.0/dicomselect/query.py` & `dicomselect-0.3.1/dicomselect/query.py`

 * *Files identical despite different names*

### Comparing `dicomselect-0.3.0/dicomselect/queryfactory.py` & `dicomselect-0.3.1/dicomselect/queryfactory.py`

 * *Files identical despite different names*

### Comparing `dicomselect-0.3.0/dicomselect/reader.py` & `dicomselect-0.3.1/dicomselect/reader.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import tempfile
 import hashlib
 import zipfile
 from pathlib import Path
-from typing import Dict, List, Optional, Tuple, Union
+from typing import Dict, List, Optional, Tuple, Union, Iterable
 
 import SimpleITK as sitk
 import numpy as np
 import pydicom
 import pydicom.errors
 
 from dicomselect.dicom import DICOMTag, DEFAULT_DICOM_TAGS, InvalidTagError
@@ -305,15 +305,15 @@
                     tag = DICOMTag(key)
                     if tag not in self._dcm_tags:
                         metadata[tag.name] = tag.convert(ref.GetMetaData(tag.key).strip())
                 except InvalidTagError:
                     continue
 
         metadata["spacing_in_plane"] = str(ref.GetSpacing()[0:2])
-        metadata["image_direction"] = str(ref.GetDirection())
+        metadata["image_direction"] = self.get_orientation(ref.GetDirection())
 
         return metadata
 
     def _collect_metadata_pydicom(self, ds: "pydicom.dataset.Dataset") -> Dict[str, str]:
         metadata = {}
         for tag in self._dcm_tags:
             # collect metadata with DICOM names, e.g. patients_age, as keys)
@@ -325,18 +325,44 @@
                 tag = DICOMTag('|'.join([str(x).zfill(4) for x in [key.group, key.elem]]))
                 if tag not in self._dcm_tags:
                     value = self.get_pydicom_value(ds, tag.key)
                     if value is not None:
                         metadata[tag.name] = tag.convert(value)
 
         metadata["spacing_in_plane"] = str(ds.PixelSpacing[0:2])
-        metadata["image_direction"] = ''
+        metadata["image_direction"] = self.get_orientation([])
         return metadata
 
     @staticmethod
+    def get_orientation(
+            image_direction: Iterable[float],
+    ):
+        """
+        Deduce image orientation from DICOM Image Orientation (Patient) Attribute.
+        Based on https://gist.github.com/agirault/60a72bdaea4a2126ecd08912137fe641
+        and https://stackoverflow.com/questions/70645577/translate-image-orientation-into-axial-sagittal-or-coronal-plane
+        and https://stackoverflow.com/questions/69799946/simpleitk-getdirection-explained
+        """
+        if len(image_direction) != 9:
+            return "unknown"
+
+        Ax, Bx, Cx, Ay, By, Cy, Az, Bz, Cz = image_direction
+        C = (Cx, Cy, Cz)
+
+        abs_image_z = np.abs(C)
+        main_index = list(abs_image_z).index(max(abs_image_z))
+        if main_index == 0:
+            main_direction = "sagittal"
+        elif main_index == 1:
+            main_direction = "coronal"
+        else:
+            main_direction = "transverse"
+        return main_direction
+
+    @staticmethod
     def get_pydicom_value(ds: pydicom.dataset.Dataset, key: "Union[pydicom.key.BaseTag, str]") -> str:
         if isinstance(key, str):
             key = '0x' + key.replace('|', '')
         if key in ds:
             result = ds[key]
             if result.is_empty:
                 return ''
```

### Comparing `dicomselect-0.3.0/dicomselect/tags_generated.py` & `dicomselect-0.3.1/dicomselect/tags_generated.py`

 * *Files identical despite different names*

### Comparing `dicomselect-0.3.0/dicomselect.egg-info/PKG-INFO` & `dicomselect-0.3.1/dicomselect.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: dicomselect
-Version: 0.3.0
+Version: 0.3.1
+Summary: UNKNOWN
 Home-page: https://github.com/DIAGNijmegen/dicomselect
 Author: 
 Author-email: Stan.Noordman@radboudumc.nl
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/DIAGNijmegen/dicomselect
 Platform: unix
 Platform: linux
@@ -84,16 +85,20 @@
 
 # Show info
 ```python
 query.info().filter("series_description").print()
 ```
 
 # Convert
+
 ```python
 from dicomselect.database import Database
+
 db = Database('/path/to/dicomselect_archive.db')
 plan = db.plan('{patient_id}/{series_description}_{patient_age}', query)
 plan.target_dir = '/path/to/target_dir'
-plan.suffix = '.mha'
+plan.extension = '.mha'
 plan.print()
 plan.execute(max_workers=4)
 ```
+
+
```

### Comparing `dicomselect-0.3.0/dicomselect.egg-info/SOURCES.txt` & `dicomselect-0.3.1/dicomselect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dicomselect-0.3.0/setup.cfg` & `dicomselect-0.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `dicomselect-0.3.0/setup.py` & `dicomselect-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import setuptools
 
-version = '0.3.0'
+version = '0.3.1'
 
 if __name__ == '__main__':
     with open("README.md", "r", encoding="utf-8") as fh:
         long_description = fh.read()
 
     setuptools.setup(
         name='dicomselect',
```

### Comparing `dicomselect-0.3.0/tests/test_convert.py` & `dicomselect-0.3.1/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `dicomselect-0.3.0/tests/test_create.py` & `dicomselect-0.3.1/tests/test_create.py`

 * *Files identical despite different names*

### Comparing `dicomselect-0.3.0/tests/test_select.py` & `dicomselect-0.3.1/tests/test_select.py`

 * *Files identical despite different names*

