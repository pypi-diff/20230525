# Comparing `tmp/mpipartition-1.0.4.tar.gz` & `tmp/mpipartition-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpipartition-1.0.4.tar", max compression
+gzip compressed data, was "mpipartition-1.0.5.tar", max compression
```

## Comparing `mpipartition-1.0.4.tar` & `mpipartition-1.0.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1076 2023-05-04 18:29:01.965921 mpipartition-1.0.4/LICENSE
--rw-r--r--   0        0        0     3723 2023-05-04 18:29:01.965921 mpipartition-1.0.4/README.rst
--rw-r--r--   0        0        0      274 2023-05-04 18:29:01.965921 mpipartition-1.0.4/mpipartition/__init__.py
--rw-r--r--   0        0        0     4942 2023-05-04 18:29:01.965921 mpipartition-1.0.4/mpipartition/distribute.py
--rw-r--r--   0        0        0    11687 2023-05-04 18:29:01.965921 mpipartition-1.0.4/mpipartition/exchange.py
--rw-r--r--   0        0        0     5047 2023-05-04 18:29:01.965921 mpipartition-1.0.4/mpipartition/overload.py
--rw-r--r--   0        0        0     7395 2023-05-04 18:29:01.965921 mpipartition-1.0.4/mpipartition/partition.py
--rw-r--r--   0        0        0     1291 2023-05-04 18:29:01.965921 mpipartition-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     4936 1970-01-01 00:00:00.000000 mpipartition-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-05-25 15:01:39.017501 mpipartition-1.0.5/LICENSE
+-rw-r--r--   0        0        0     3723 2023-05-25 15:01:39.017501 mpipartition-1.0.5/README.rst
+-rw-r--r--   0        0        0      274 2023-05-25 15:01:39.017501 mpipartition-1.0.5/mpipartition/__init__.py
+-rw-r--r--   0        0        0     4942 2023-05-25 15:01:39.017501 mpipartition-1.0.5/mpipartition/distribute.py
+-rw-r--r--   0        0        0    11711 2023-05-25 15:01:39.017501 mpipartition-1.0.5/mpipartition/exchange.py
+-rw-r--r--   0        0        0     5047 2023-05-25 15:01:39.017501 mpipartition-1.0.5/mpipartition/overload.py
+-rw-r--r--   0        0        0     7395 2023-05-25 15:01:39.017501 mpipartition-1.0.5/mpipartition/partition.py
+-rw-r--r--   0        0        0     1291 2023-05-25 15:01:39.017501 mpipartition-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     4936 1970-01-01 00:00:00.000000 mpipartition-1.0.5/PKG-INFO
```

### Comparing `mpipartition-1.0.4/LICENSE` & `mpipartition-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mpipartition-1.0.4/README.rst` & `mpipartition-1.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `mpipartition-1.0.4/mpipartition/distribute.py` & `mpipartition-1.0.5/mpipartition/distribute.py`

 * *Files identical despite different names*

### Comparing `mpipartition-1.0.4/mpipartition/exchange.py` & `mpipartition-1.0.5/mpipartition/exchange.py`

 * *Files 1% similar despite different names*

```diff
@@ -282,15 +282,15 @@
 
     # if we are still not able to assign all orphans, replace key or abort after
     # printing some debug messages
     if replace_notfound_key is not None and localcount_missmatch_after > 0:
         d = data_new[key]
         d[np.isin(d, missing_keys)] = replace_notfound_key
     for i in range(nranks):
-        if rank == i and localcount_missmatch_after != 0:
+        if rank == i and localcount_missmatch_after != 0 and verbose > 1:
             print(
                 f"Warning from rank {rank} in exchange: Unable to assign all "
                 f"progenitors to correct ranks (failed for "
                 f"{localcount_missmatch_after} out of {localcount_missmatch})"
             )
             print("Could not assign keys: ", missing_keys)
             print("", flush=True)
@@ -302,15 +302,15 @@
                 f"Error in exchange: Unable to assign all progenitors to correct ranks "
                 f"(tried to reassign {totalcount_missmatch}, failed for "
                 f"{totalcount_missmatch_after})",
                 file=sys.stderr,
                 flush=True,
             )
             comm.Abort()
-        else:
+        elif verbose:
             print(
                 f"Warning in exchange: Unable to assign all progenitors to correct "
                 f"ranks (tried to reassign {totalcount_missmatch}, failed for "
                 f"{totalcount_missmatch_after}), replacing missing values with "
                 f"{replace_notfound_key}",
                 flush=True,
             )
```

### Comparing `mpipartition-1.0.4/mpipartition/overload.py` & `mpipartition-1.0.5/mpipartition/overload.py`

 * *Files identical despite different names*

### Comparing `mpipartition-1.0.4/mpipartition/partition.py` & `mpipartition-1.0.5/mpipartition/partition.py`

 * *Files identical despite different names*

### Comparing `mpipartition-1.0.4/pyproject.toml` & `mpipartition-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mpipartition"
-version = "1.0.4"
+version = "1.0.5"
 description = "MPI volume decomposition and particle distribution tools"
 authors = ["Michael Buehlmann <buehlmann.michi@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/ArgonneCPAC/MPIPartition"
 repository = "https://github.com/ArgonneCPAC/MPIPartition"
 documentation = "https://argonnecpac.github.io/MPIPartition"
```

### Comparing `mpipartition-1.0.4/PKG-INFO` & `mpipartition-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpipartition
-Version: 1.0.4
+Version: 1.0.5
 Summary: MPI volume decomposition and particle distribution tools
 Home-page: https://github.com/ArgonneCPAC/MPIPartition
 License: MIT
 Keywords: MPI,mpi4py,scientific computing,parallel computing
 Author: Michael Buehlmann
 Author-email: buehlmann.michi@gmail.com
 Requires-Python: >=3.7,<4.0
```

