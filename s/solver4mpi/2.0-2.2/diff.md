# Comparing `tmp/solver4mpi-2.0.tar.gz` & `tmp/solver4mpi-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solver4mpi-2.0.tar", last modified: Wed May 24 21:45:14 2023, max compression
+gzip compressed data, was "solver4mpi-2.2.tar", last modified: Thu May 25 01:21:31 2023, max compression
```

## Comparing `solver4mpi-2.0.tar` & `solver4mpi-2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-05-24 21:45:14.597399 solver4mpi-2.0/
--rw-r--r--   0 mregnier   (501) staff       (20)      226 2023-05-24 21:45:14.597068 solver4mpi-2.0/PKG-INFO
--rw-r--r--   0 mregnier   (501) staff       (20)       21 2023-05-24 10:54:28.000000 solver4mpi-2.0/README.md
--rw-r--r--   0 mregnier   (501) staff       (20)       38 2023-05-24 21:45:14.597499 solver4mpi-2.0/setup.cfg
--rw-r--r--   0 mregnier   (501) staff       (20)      718 2023-05-24 21:41:54.000000 solver4mpi-2.0/setup.py
-drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-05-24 21:45:14.591480 solver4mpi-2.0/solver4mpi/
--rw-r--r--   0 mregnier   (501) staff       (20)       55 2023-05-24 10:54:28.000000 solver4mpi-2.0/solver4mpi/__init__.py
--rw-r--r--   0 mregnier   (501) staff       (20)     2225 2023-05-24 20:33:44.000000 solver4mpi-2.0/solver4mpi/minimizer_multiprocess.py
--rw-r--r--   0 mregnier   (501) staff       (20)     1877 2023-05-24 21:37:56.000000 solver4mpi-2.0/solver4mpi/test.py
-drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-05-24 21:45:14.596657 solver4mpi-2.0/solver4mpi.egg-info/
--rw-r--r--   0 mregnier   (501) staff       (20)      226 2023-05-24 21:45:14.000000 solver4mpi-2.0/solver4mpi.egg-info/PKG-INFO
--rw-r--r--   0 mregnier   (501) staff       (20)      266 2023-05-24 21:45:14.000000 solver4mpi-2.0/solver4mpi.egg-info/SOURCES.txt
--rw-r--r--   0 mregnier   (501) staff       (20)        1 2023-05-24 21:45:14.000000 solver4mpi-2.0/solver4mpi.egg-info/dependency_links.txt
--rw-r--r--   0 mregnier   (501) staff       (20)       13 2023-05-24 21:45:14.000000 solver4mpi-2.0/solver4mpi.egg-info/requires.txt
--rw-r--r--   0 mregnier   (501) staff       (20)       11 2023-05-24 21:45:14.000000 solver4mpi-2.0/solver4mpi.egg-info/top_level.txt
+drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-05-25 01:21:31.314658 solver4mpi-2.2/
+-rw-r--r--   0 mregnier   (501) staff       (20)      226 2023-05-25 01:21:31.314292 solver4mpi-2.2/PKG-INFO
+-rw-r--r--   0 mregnier   (501) staff       (20)       21 2023-05-25 01:20:51.000000 solver4mpi-2.2/README.md
+-rw-r--r--   0 mregnier   (501) staff       (20)       38 2023-05-25 01:21:31.314780 solver4mpi-2.2/setup.cfg
+-rw-r--r--   0 mregnier   (501) staff       (20)      718 2023-05-25 01:21:22.000000 solver4mpi-2.2/setup.py
+drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-05-25 01:21:31.308509 solver4mpi-2.2/solver4mpi/
+-rw-r--r--   0 mregnier   (501) staff       (20)       55 2023-05-25 01:20:51.000000 solver4mpi-2.2/solver4mpi/__init__.py
+-rw-r--r--   0 mregnier   (501) staff       (20)     2488 2023-05-25 01:20:51.000000 solver4mpi-2.2/solver4mpi/minimizer_multiprocess.py
+-rw-r--r--   0 mregnier   (501) staff       (20)     1877 2023-05-25 01:20:51.000000 solver4mpi-2.2/solver4mpi/test.py
+drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-05-25 01:21:31.313785 solver4mpi-2.2/solver4mpi.egg-info/
+-rw-r--r--   0 mregnier   (501) staff       (20)      226 2023-05-25 01:21:31.000000 solver4mpi-2.2/solver4mpi.egg-info/PKG-INFO
+-rw-r--r--   0 mregnier   (501) staff       (20)      266 2023-05-25 01:21:31.000000 solver4mpi-2.2/solver4mpi.egg-info/SOURCES.txt
+-rw-r--r--   0 mregnier   (501) staff       (20)        1 2023-05-25 01:21:31.000000 solver4mpi-2.2/solver4mpi.egg-info/dependency_links.txt
+-rw-r--r--   0 mregnier   (501) staff       (20)       13 2023-05-25 01:21:31.000000 solver4mpi-2.2/solver4mpi.egg-info/requires.txt
+-rw-r--r--   0 mregnier   (501) staff       (20)       11 2023-05-25 01:21:31.000000 solver4mpi-2.2/solver4mpi.egg-info/top_level.txt
```

### Comparing `solver4mpi-2.0/setup.py` & `solver4mpi-2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,14 @@
     author='Mathias Regnier',
     author_email='mathias.p.regnier@gmail.com',
     # Needed to actually package something
     packages=find_packages(),
     # Needed for dependencies
     install_requires=['multiprocess'],
     # *strongly* suggested for sharing
-    version='2.0',
+    version='2.2',
     # The license can be anything you like
     license='',
     description='Optimized minimizer for MPI python.',
     # We will also need a readme eventually (there will be a warning)
     # long_description=open('README.txt').read(),
 )
```

### Comparing `solver4mpi-2.0/solver4mpi/minimizer_multiprocess.py` & `solver4mpi-2.2/solver4mpi/minimizer_multiprocess.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         return np.concatenate(results)
 
 class WrapperMPI:
 
     def __init__(self, comm, chi2, cpu_per_tasks, x0, method='TNC', tol=1e-3, options={}, verbose=False):
 
         #FitMultiProcessCPU.__init__(self, chi2, cpu_per_tasks, x0, method=method, tol=tol, options=options)
-
+        self.verbose = verbose
         ### MPI distribution
         self.comm = comm
         self.size = self.comm.Get_size()
         self.rank = self.comm.Get_rank()
         if verbose:
             print(f'size = {self.size} and rank = {self.rank}')
 
@@ -54,14 +54,19 @@
         
     def perform(self, index_theta):
         res = np.zeros(len(index_theta))
         index_per_process = self._split_params(index_theta)
         number_loop = len(index_per_process) // self.fit_multi_process.nb_cpu
         rest_loop = len(index_per_process) % self.fit_multi_process.nb_cpu
 
+        if self.verbose:
+            print(f'Number of loop : {number_loop}')
+            print(f'Number of rest : {rest_loop}')
+
         for iloop in range(number_loop):
             
             res[index_per_process[iloop*self.nb_cpu:(iloop+1)*self.nb_cpu]] = self.fit_multi_process.perform_cpu(list(index_per_process[iloop*self.nb_cpu:(iloop+1)*self.nb_cpu]))
-            
+            if self.verbose:
+                print(res[index_per_process[iloop*self.nb_cpu:(iloop+1)*self.nb_cpu]])
         res[index_per_process[-rest_loop:]] = self.fit_multi_process.perform_cpu(list(index_per_process[-rest_loop:]))
         
         return res
```

### Comparing `solver4mpi-2.0/solver4mpi/test.py` & `solver4mpi-2.2/solver4mpi/test.py`

 * *Files identical despite different names*

