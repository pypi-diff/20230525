# Comparing `tmp/tencirchem-0.0.1.tar.gz` & `tmp/tencirchem-2023.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tencirchem-0.0.1.tar", last modified: Wed Mar  8 07:00:46 2023, max compression
+gzip compressed data, was "tencirchem-2023.3.tar", last modified: Sun Mar 19 06:28:26 2023, max compression
```

## Comparing `tencirchem-0.0.1.tar` & `tencirchem-2023.3.tar`

### file list

```diff
@@ -1,9 +1,61 @@
-drwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2023-03-08 07:00:46.292918 tencirchem-0.0.1/
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)      117 2023-03-08 07:00:46.292918 tencirchem-0.0.1/PKG-INFO
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)       38 2023-03-08 07:00:46.293915 tencirchem-0.0.1/setup.cfg
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)      398 2023-03-08 07:00:42.000000 tencirchem-0.0.1/setup.py
-drwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        0 2023-03-08 07:00:46.291920 tencirchem-0.0.1/tencirchem.egg-info/
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)      117 2023-03-08 07:00:46.000000 tencirchem-0.0.1/tencirchem.egg-info/PKG-INFO
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)      144 2023-03-08 07:00:46.000000 tencirchem-0.0.1/tencirchem.egg-info/SOURCES.txt
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        1 2023-03-08 07:00:46.000000 tencirchem-0.0.1/tencirchem.egg-info/dependency_links.txt
--rwxrwxrwx   0 weitangli  (1000) weitangli  (1000)        1 2023-03-08 07:00:46.000000 tencirchem-0.0.1/tencirchem.egg-info/top_level.txt
+drwxr-xr-x   0 weitangli  (1000) weitangli  (1000)        0 2023-03-19 06:28:26.851030 tencirchem-2023.3/
+-rw-r--r--   0 weitangli  (1000) weitangli  (1000)     9177 2023-03-18 10:36:33.000000 tencirchem-2023.3/LICENSE
+-rw-r--r--   0 weitangli  (1000) weitangli  (1000)     3639 2023-03-19 06:28:26.850032 tencirchem-2023.3/PKG-INFO
+-rw-r--r--   0 weitangli  (1000) weitangli  (1000)     3192 2023-03-18 10:36:33.000000 tencirchem-2023.3/README.md
+-rw-r--r--   0 weitangli  (1000) weitangli  (1000)     1043 2023-03-18 10:36:33.000000 tencirchem-2023.3/pyproject.toml
+-rw-r--r--   0 weitangli  (1000) weitangli  (1000)       38 2023-03-19 06:28:26.851030 tencirchem-2023.3/setup.cfg
+-rw-r--r--   0 weitangli  (1000) weitangli  (1000)      977 2023-03-18 10:36:33.000000 tencirchem-2023.3/setup.py
+drwxr-xr-x   0 weitangli  (1000) weitangli  (1000)        0 2023-03-19 06:28:26.801829 tencirchem-2023.3/tencirchem/
+-rw-r--r--   0 weitangli  (1000) weitangli  (1000)     1461 2023-03-18 10:36:33.000000 tencirchem-2023.3/tencirchem/__init__.py
+-rw-r--r--   0 weitangli  (1000) weitangli  (1000)      343 2023-03-18 10:36:33.000000 tencirchem-2023.3/tencirchem/constants.py
+drwxr-xr-x   0 weitangli  (1000) weitangli  (1000)        0 2023-03-19 06:28:26.811553 tencirchem-2023.3/tencirchem/dynamic/
+-rw-r--r--   0 weitangli  (1000) weitangli  (1000)      276 2023-03-18 10:36:33.000000 tencirchem-2023.3/tencirchem/dynamic/__init__.py
+drwxr-xr-x   0 weitangli  (1000) weitangli  (1000)        0 2023-03-19 06:28:26.814623 tencirchem-2023.3/tencirchem/dynamic/model/
+-rw-r--r--   0 weitangli  (1000) weitangli  (1000)        0 2023-03-18 10:36:33.000000 tencirchem-2023.3/tencirchem/dynamic/model/__init__.py
+-rw-r--r--   0 weitangli  (1000) weitangli  (1000)     4476 2023-03-18 10:36:33.000000 tencirchem-2023.3/tencirchem/dynamic/model/pyrazine.py
+-rw-r--r--   0 weitangli  (1000) weitangli  (1000)      822 2023-03-18 10:36:33.000000 tencirchem-2023.3/tencirchem/dynamic/model/sbm.py
+-rw-r--r--   0 weitangli  (1000) weitangli  (1000)     4493 2023-03-18 10:36:33.000000 tencirchem-2023.3/tencirchem/dynamic/time_derivative.py
+-rw-r--r--   0 weitangli  (1000) weitangli  (1000)     7079 2023-03-18 10:36:33.000000 tencirchem-2023.3/tencirchem/dynamic/time_evolution.py
+-rw-r--r--   0 weitangli  (1000) weitangli  (1000)    11049 2023-03-18 10:36:33.000000 tencirchem-2023.3/tencirchem/dynamic/transform.py
+-rw-r--r--   0 weitangli  (1000) weitangli  (1000)     3727 2023-03-18 10:36:33.000000 tencirchem-2023.3/tencirchem/molecule.py
+drwxr-xr-x   0 weitangli  (1000) weitangli  (1000)        0 2023-03-19 06:28:26.831082 tencirchem-2023.3/tencirchem/static/
+-rw-r--r--   0 weitangli  (1000) weitangli  (1000)        0 2023-03-18 10:36:33.000000 tencirchem-2023.3/tencirchem/static/__init__.py
+-rw-r--r--   0 weitangli  (1000) weitangli  (1000)     2782 2023-03-18 10:36:33.000000 tencirchem-2023.3/tencirchem/static/ci_utils.py
+-rw-r--r--   0 weitangli  (1000) weitangli  (1000)     3286 2023-03-18 10:36:33.000000 tencirchem-2023.3/tencirchem/static/engine_hea.py
+-rw-r--r--   0 weitangli  (1000) weitangli  (1000)     6586 2023-03-18 10:36:33.000000 tencirchem-2023.3/tencirchem/static/engine_ucc.py
+-rw-r--r--   0 weitangli  (1000) weitangli  (1000)    12121 2023-03-18 10:36:33.000000 tencirchem-2023.3/tencirchem/static/evolve_civector.py
+-rw-r--r--   0 weitangli  (1000) weitangli  (1000)     4895 2023-03-18 10:36:33.000000 tencirchem-2023.3/tencirchem/static/evolve_pyscf.py
+-rw-r--r--   0 weitangli  (1000) weitangli  (1000)     3158 2023-03-18 10:36:33.000000 tencirchem-2023.3/tencirchem/static/evolve_statevector.py
+-rw-r--r--   0 weitangli  (1000) weitangli  (1000)     7038 2023-03-18 10:36:33.000000 tencirchem-2023.3/tencirchem/static/evolve_tensornetwork.py
+-rw-r--r--   0 weitangli  (1000) weitangli  (1000)     8963 2023-03-18 10:36:33.000000 tencirchem-2023.3/tencirchem/static/hamiltonian.py
+-rw-r--r--   0 weitangli  (1000) weitangli  (1000)    26150 2023-03-18 10:36:33.000000 tencirchem-2023.3/tencirchem/static/hea.py
+-rw-r--r--   0 weitangli  (1000) weitangli  (1000)     9281 2023-03-18 10:36:33.000000 tencirchem-2023.3/tencirchem/static/kupccgsd.py
+-rw-r--r--   0 weitangli  (1000) weitangli  (1000)     8264 2023-03-18 10:36:33.000000 tencirchem-2023.3/tencirchem/static/puccd.py
+-rw-r--r--   0 weitangli  (1000) weitangli  (1000)    46576 2023-03-18 10:36:33.000000 tencirchem-2023.3/tencirchem/static/ucc.py
+-rw-r--r--   0 weitangli  (1000) weitangli  (1000)     6925 2023-03-18 10:36:33.000000 tencirchem-2023.3/tencirchem/static/uccsd.py
+drwxr-xr-x   0 weitangli  (1000) weitangli  (1000)        0 2023-03-19 06:28:26.835072 tencirchem-2023.3/tencirchem/utils/
+-rw-r--r--   0 weitangli  (1000) weitangli  (1000)        0 2023-03-18 10:36:33.000000 tencirchem-2023.3/tencirchem/utils/__init__.py
+-rw-r--r--   0 weitangli  (1000) weitangli  (1000)     3038 2023-03-18 10:36:33.000000 tencirchem-2023.3/tencirchem/utils/backend.py
+-rw-r--r--   0 weitangli  (1000) weitangli  (1000)     2925 2023-03-18 10:36:33.000000 tencirchem-2023.3/tencirchem/utils/circuit.py
+-rw-r--r--   0 weitangli  (1000) weitangli  (1000)     4351 2023-03-18 10:36:33.000000 tencirchem-2023.3/tencirchem/utils/misc.py
+drwxr-xr-x   0 weitangli  (1000) weitangli  (1000)        0 2023-03-19 06:28:26.806815 tencirchem-2023.3/tencirchem.egg-info/
+-rw-r--r--   0 weitangli  (1000) weitangli  (1000)     3639 2023-03-19 06:28:26.000000 tencirchem-2023.3/tencirchem.egg-info/PKG-INFO
+-rw-r--r--   0 weitangli  (1000) weitangli  (1000)     1400 2023-03-19 06:28:26.000000 tencirchem-2023.3/tencirchem.egg-info/SOURCES.txt
+-rw-r--r--   0 weitangli  (1000) weitangli  (1000)        1 2023-03-19 06:28:26.000000 tencirchem-2023.3/tencirchem.egg-info/dependency_links.txt
+-rw-r--r--   0 weitangli  (1000) weitangli  (1000)      117 2023-03-19 06:28:26.000000 tencirchem-2023.3/tencirchem.egg-info/requires.txt
+-rw-r--r--   0 weitangli  (1000) weitangli  (1000)       17 2023-03-19 06:28:26.000000 tencirchem-2023.3/tencirchem.egg-info/top_level.txt
+drwxr-xr-x   0 weitangli  (1000) weitangli  (1000)        0 2023-03-19 06:28:26.837067 tencirchem-2023.3/tests/
+-rw-r--r--   0 weitangli  (1000) weitangli  (1000)        0 2023-03-18 10:36:32.000000 tencirchem-2023.3/tests/__init__.py
+drwxr-xr-x   0 weitangli  (1000) weitangli  (1000)        0 2023-03-19 06:28:26.841056 tencirchem-2023.3/tests/dynamics/
+-rw-r--r--   0 weitangli  (1000) weitangli  (1000)        0 2023-03-18 10:36:32.000000 tencirchem-2023.3/tests/dynamics/__init__.py
+-rw-r--r--   0 weitangli  (1000) weitangli  (1000)     1218 2023-03-18 10:36:32.000000 tencirchem-2023.3/tests/dynamics/test_dynamics.py
+-rw-r--r--   0 weitangli  (1000) weitangli  (1000)     2914 2023-03-18 10:36:32.000000 tencirchem-2023.3/tests/dynamics/test_hamiltonian.py
+-rw-r--r--   0 weitangli  (1000) weitangli  (1000)      250 2023-03-18 10:36:32.000000 tencirchem-2023.3/tests/misc.py
+drwxr-xr-x   0 weitangli  (1000) weitangli  (1000)        0 2023-03-19 06:28:26.849034 tencirchem-2023.3/tests/static/
+-rw-r--r--   0 weitangli  (1000) weitangli  (1000)        0 2023-03-18 10:36:32.000000 tencirchem-2023.3/tests/static/__init__.py
+-rw-r--r--   0 weitangli  (1000) weitangli  (1000)     3466 2023-03-18 10:36:32.000000 tencirchem-2023.3/tests/static/test_engine.py
+-rw-r--r--   0 weitangli  (1000) weitangli  (1000)     2446 2023-03-18 10:36:32.000000 tencirchem-2023.3/tests/static/test_hamiltonian.py
+-rw-r--r--   0 weitangli  (1000) weitangli  (1000)     1341 2023-03-18 12:42:47.000000 tencirchem-2023.3/tests/static/test_hea.py
+-rw-r--r--   0 weitangli  (1000) weitangli  (1000)     1335 2023-03-18 10:36:32.000000 tencirchem-2023.3/tests/static/test_molecule.py
+-rw-r--r--   0 weitangli  (1000) weitangli  (1000)     1840 2023-03-18 10:36:32.000000 tencirchem-2023.3/tests/static/test_puccd.py
+-rw-r--r--   0 weitangli  (1000) weitangli  (1000)     3524 2023-03-18 10:36:32.000000 tencirchem-2023.3/tests/static/test_static.py
```

