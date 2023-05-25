# Comparing `tmp/flams-0.0.4.tar.gz` & `tmp/flams-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flams-0.0.4.tar", last modified: Tue May  9 13:13:30 2023, max compression
+gzip compressed data, was "flams-0.0.5.tar", last modified: Wed May 17 13:34:05 2023, max compression
```

## Comparing `flams-0.0.4.tar` & `flams-0.0.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 u0138113 (1031392) domain users (200513)        0 2023-05-09 13:13:30.587750 flams-0.0.4/
--rw-r--r--   0 u0138113 (1031392) domain users (200513)     1223 2023-05-09 12:23:21.000000 flams-0.0.4/LICENSE
--rw-r--r--   0 u0138113 (1031392) domain users (200513)     5783 2023-05-09 13:13:30.587750 flams-0.0.4/PKG-INFO
--rw-r--r--   0 u0138113 (1031392) domain users (200513)     5523 2023-05-09 12:23:21.000000 flams-0.0.4/README.md
-drwxr-xr-x   0 u0138113 (1031392) domain users (200513)        0 2023-05-09 13:13:30.583750 flams-0.0.4/flams/
--rw-r--r--   0 u0138113 (1031392) domain users (200513)        0 2023-05-09 12:23:21.000000 flams-0.0.4/flams/__init__.py
-drwxr-xr-x   0 u0138113 (1031392) domain users (200513)        0 2023-05-09 13:13:30.587750 flams-0.0.4/flams/databases/
--rw-r--r--   0 u0138113 (1031392) domain users (200513)        0 2023-05-09 12:23:21.000000 flams-0.0.4/flams/databases/__init__.py
--rw-r--r--   0 u0138113 (1031392) domain users (200513)     2825 2023-05-09 12:23:21.000000 flams-0.0.4/flams/databases/cplmv4.py
--rw-r--r--   0 u0138113 (1031392) domain users (200513)     8911 2023-05-09 12:23:21.000000 flams-0.0.4/flams/databases/setup.py
--rw-r--r--   0 u0138113 (1031392) domain users (200513)     3491 2023-05-09 12:23:21.000000 flams-0.0.4/flams/display.py
--rw-r--r--   0 u0138113 (1031392) domain users (200513)     2449 2023-05-09 12:23:21.000000 flams-0.0.4/flams/flams.py
--rw-r--r--   0 u0138113 (1031392) domain users (200513)    12083 2023-05-09 12:23:21.000000 flams-0.0.4/flams/input.py
--rw-r--r--   0 u0138113 (1031392) domain users (200513)    12408 2023-05-09 12:23:21.000000 flams-0.0.4/flams/run_blast.py
--rw-r--r--   0 u0138113 (1031392) domain users (200513)      960 2023-05-09 12:59:47.000000 flams-0.0.4/flams/utils.py
-drwxr-xr-x   0 u0138113 (1031392) domain users (200513)        0 2023-05-09 13:13:30.587750 flams-0.0.4/flams.egg-info/
--rw-r--r--   0 u0138113 (1031392) domain users (200513)     5783 2023-05-09 13:13:30.000000 flams-0.0.4/flams.egg-info/PKG-INFO
--rw-r--r--   0 u0138113 (1031392) domain users (200513)      403 2023-05-09 13:13:30.000000 flams-0.0.4/flams.egg-info/SOURCES.txt
--rw-r--r--   0 u0138113 (1031392) domain users (200513)        1 2023-05-09 13:13:30.000000 flams-0.0.4/flams.egg-info/dependency_links.txt
--rw-r--r--   0 u0138113 (1031392) domain users (200513)       43 2023-05-09 13:13:30.000000 flams-0.0.4/flams.egg-info/entry_points.txt
--rw-r--r--   0 u0138113 (1031392) domain users (200513)      316 2023-05-09 13:13:30.000000 flams-0.0.4/flams.egg-info/requires.txt
--rw-r--r--   0 u0138113 (1031392) domain users (200513)        6 2023-05-09 13:13:30.000000 flams-0.0.4/flams.egg-info/top_level.txt
--rw-r--r--   0 u0138113 (1031392) domain users (200513)      454 2023-05-09 13:13:22.000000 flams-0.0.4/pyproject.toml
--rw-r--r--   0 u0138113 (1031392) domain users (200513)      315 2023-05-09 12:23:21.000000 flams-0.0.4/requirements.txt
--rw-r--r--   0 u0138113 (1031392) domain users (200513)       38 2023-05-09 13:13:30.587750 flams-0.0.4/setup.cfg
+drwxr-xr-x   0 u0138113 (1031392) domain users (200513)        0 2023-05-17 13:34:05.168484 flams-0.0.5/
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)     1223 2023-05-09 12:23:21.000000 flams-0.0.5/LICENSE
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)     5783 2023-05-17 13:34:05.168484 flams-0.0.5/PKG-INFO
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)     5523 2023-05-09 12:23:21.000000 flams-0.0.5/README.md
+drwxr-xr-x   0 u0138113 (1031392) domain users (200513)        0 2023-05-17 13:34:05.168484 flams-0.0.5/flams/
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)        0 2023-05-09 12:23:21.000000 flams-0.0.5/flams/__init__.py
+drwxr-xr-x   0 u0138113 (1031392) domain users (200513)        0 2023-05-17 13:34:05.168484 flams-0.0.5/flams/databases/
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)        0 2023-05-09 12:23:21.000000 flams-0.0.5/flams/databases/__init__.py
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)     2825 2023-05-09 12:23:21.000000 flams-0.0.5/flams/databases/cplmv4.py
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)     8911 2023-05-09 12:23:21.000000 flams-0.0.5/flams/databases/setup.py
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)     3491 2023-05-09 12:23:21.000000 flams-0.0.5/flams/display.py
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)     2449 2023-05-09 12:23:21.000000 flams-0.0.5/flams/flams.py
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)    13386 2023-05-17 13:11:26.000000 flams-0.0.5/flams/input.py
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)    12408 2023-05-09 12:23:21.000000 flams-0.0.5/flams/run_blast.py
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)      960 2023-05-09 12:59:47.000000 flams-0.0.5/flams/utils.py
+drwxr-xr-x   0 u0138113 (1031392) domain users (200513)        0 2023-05-17 13:34:05.168484 flams-0.0.5/flams.egg-info/
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)     5783 2023-05-17 13:34:05.000000 flams-0.0.5/flams.egg-info/PKG-INFO
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)      403 2023-05-17 13:34:05.000000 flams-0.0.5/flams.egg-info/SOURCES.txt
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)        1 2023-05-17 13:34:05.000000 flams-0.0.5/flams.egg-info/dependency_links.txt
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)       43 2023-05-17 13:34:05.000000 flams-0.0.5/flams.egg-info/entry_points.txt
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)      316 2023-05-17 13:34:05.000000 flams-0.0.5/flams.egg-info/requires.txt
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)        6 2023-05-17 13:34:05.000000 flams-0.0.5/flams.egg-info/top_level.txt
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)      454 2023-05-17 13:32:27.000000 flams-0.0.5/pyproject.toml
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)      315 2023-05-09 12:23:21.000000 flams-0.0.5/requirements.txt
+-rw-r--r--   0 u0138113 (1031392) domain users (200513)       38 2023-05-17 13:34:05.168484 flams-0.0.5/setup.cfg
```

### Comparing `flams-0.0.4/LICENSE` & `flams-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `flams-0.0.4/PKG-INFO` & `flams-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flams
-Version: 0.0.4
+Version: 0.0.5
 Summary: Find Lysine Acylation & other Modification Sites
 Project-URL: repository, https://github.com/hannelorelongin/FLAMS
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # FLAMS: Find Lysine Acylation & other Modification Sites
```

### Comparing `flams-0.0.4/README.md` & `flams-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `flams-0.0.4/flams/databases/cplmv4.py` & `flams-0.0.5/flams/databases/cplmv4.py`

 * *Files identical despite different names*

### Comparing `flams-0.0.4/flams/databases/setup.py` & `flams-0.0.5/flams/databases/setup.py`

 * *Files identical despite different names*

### Comparing `flams-0.0.4/flams/display.py` & `flams-0.0.5/flams/display.py`

 * *Files identical despite different names*

### Comparing `flams-0.0.4/flams/flams.py` & `flams-0.0.5/flams/flams.py`

 * *Files identical despite different names*

### Comparing `flams-0.0.4/flams/input.py` & `flams-0.0.5/flams/input.py`

 * *Files 4% similar despite different names*

```diff
@@ -139,14 +139,15 @@
         Argument parser
 
     """
     check_files_valid(args, parser)
 
     protein_file = get_protein_file(args, parser)
 
+    check_position_in_range(protein_file, args.pos)
     check_lysine(protein_file, args.pos, parser)
     check_modifications(args, parser)
     return protein_file
 
 
 def check_files_valid(args, parser):
     """
@@ -291,14 +292,51 @@
 
     """
     # user provides position in 1-based indexing system
     position_idx = position - 1
     input_seq = SeqIO.read(input, "fasta").seq
     return input_seq[position_idx] == "K"
 
+def check_position_in_range(protein_file, pos):
+    """
+    This function checks whether the user provided position is actually part of the protein.
+    If not, it returns an error.
+
+    Parameters
+    ----------
+    protein_file: fasta
+        FASTA file containing query protein
+    pos: int
+        User provided position in the query protein
+    """
+
+    if not is_within_range(pos, protein_file):
+        logging.error(
+            f"Please provide a lysine position smaller than the size " +
+            f"of your protein ({_get_length_protein(protein_file)})."
+            )
+        sys.exit()
+
+
+def is_within_range(position: int, protein_file: Path) -> bool:
+    """
+    This function assess whether the user provided position is actually part of the query protein.
+
+    Parameters
+    ----------
+    position: int
+        User provided position in the query protein
+    input: Path
+        Path to FASTA file containing query protein
+
+    """
+    # user provides position in 1-based indexing system
+    position_idx = position - 1
+    length = _get_length_protein(protein_file)
+    return position_idx < length
 
 def check_modifications(args, parser):
     """
     This function checks whether the user provided modification is part of the collection of modifications that can be queried.
     If not, it returns an error. It also transforms the aggregate modification options Ubs, Acylations, Others, and All
     to their respective collection of modifications. Finally, it removes any duplicate modification types.
 
@@ -357,7 +395,11 @@
     upper = min(len(seq), pos_idx + 3)
     prefix = "..." if lower > 0 else ""
     sufix = "..." if upper < len(seq) - 1 else ""
     pos_idx = len(prefix) + (pos_idx - lower)
     seq_row = f"{prefix}{seq[lower:upper]}{sufix}"
     pointer_row = " " * pos_idx + "^"
     return "".join(["\n", seq_row, "\n", pointer_row])
+
+def _get_length_protein(protein_file: Path) -> int:
+    prot_seq = SeqIO.read(protein_file, "fasta").seq
+    return len(prot_seq)
```

### Comparing `flams-0.0.4/flams/run_blast.py` & `flams-0.0.5/flams/run_blast.py`

 * *Files identical despite different names*

### Comparing `flams-0.0.4/flams/utils.py` & `flams-0.0.5/flams/utils.py`

 * *Files identical despite different names*

### Comparing `flams-0.0.4/flams.egg-info/PKG-INFO` & `flams-0.0.5/flams.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flams
-Version: 0.0.4
+Version: 0.0.5
 Summary: Find Lysine Acylation & other Modification Sites
 Project-URL: repository, https://github.com/hannelorelongin/FLAMS
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # FLAMS: Find Lysine Acylation & other Modification Sites
```

