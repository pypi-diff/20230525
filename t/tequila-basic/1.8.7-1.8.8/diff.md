# Comparing `tmp/tequila-basic-1.8.7.tar.gz` & `tmp/tequila-basic-1.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tequila-basic-1.8.7.tar", last modified: Fri Mar 17 08:29:35 2023, max compression
+gzip compressed data, was "tequila-basic-1.8.8.tar", last modified: Thu May 25 07:44:51 2023, max compression
```

## Comparing `tequila-basic-1.8.7.tar` & `tequila-basic-1.8.8.tar`

### file list

```diff
@@ -1,109 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 08:29:35.185701 tequila-basic-1.8.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    20749 2023-03-17 08:29:35.185701 tequila-basic-1.8.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20071 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-03-17 08:29:33.000000 tequila-basic-1.8.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-17 08:29:35.185701 tequila-basic-1.8.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 08:29:35.173701 tequila-basic-1.8.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 08:29:35.173701 tequila-basic-1.8.7/src/tequila/
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 08:29:35.173701 tequila-basic-1.8.7/src/tequila/apps/
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21757 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/apps/_unary_state_prep_impl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 08:29:35.173701 tequila-basic-1.8.7/src/tequila/apps/adapt/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/apps/adapt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19356 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/apps/adapt/adapt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 08:29:35.173701 tequila-basic-1.8.7/src/tequila/apps/krylov/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/apps/krylov/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/apps/krylov/krylov.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 08:29:35.173701 tequila-basic-1.8.7/src/tequila/apps/robustness/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/apps/robustness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/apps/robustness/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    24743 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/apps/robustness/interval.py
--rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/apps/unary_state_prep.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/autograd_imports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 08:29:35.177701 tequila-basic-1.8.7/src/tequila/circuit/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/circuit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16377 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/circuit/_gates_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)    31866 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/circuit/circuit.py
--rw-r--r--   0 runner    (1001) docker     (123)    32685 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/circuit/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)    35355 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/circuit/gates.py
--rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/circuit/gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)     8322 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/circuit/noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/circuit/pyzx.py
--rw-r--r--   0 runner    (1001) docker     (123)    15230 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/circuit/qasm.py
--rw-r--r--   0 runner    (1001) docker     (123)    10789 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/circuit/qpic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 08:29:35.177701 tequila-basic-1.8.7/src/tequila/grouping/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/grouping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19317 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/grouping/binary_rep.py
--rw-r--r--   0 runner    (1001) docker     (123)    10916 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/grouping/binary_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    63862 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/grouping/compile_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    11059 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/grouping/overlapping_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 08:29:35.177701 tequila-basic-1.8.7/src/tequila/hamiltonian/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/hamiltonian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/hamiltonian/paulis.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/hamiltonian/paulistring.py
--rw-r--r--   0 runner    (1001) docker     (123)    21401 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/hamiltonian/qubit_hamiltonian.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 08:29:35.177701 tequila-basic-1.8.7/src/tequila/ml/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10023 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/ml/interface_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/ml/ml_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/ml/utils_ml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 08:29:35.177701 tequila-basic-1.8.7/src/tequila/objective/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/objective/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/objective/braket.py
--rw-r--r--   0 runner    (1001) docker     (123)    31715 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/objective/objective.py
--rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/objective/qtensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 08:29:35.181701 tequila-basic-1.8.7/src/tequila/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/optimizers/_containers.py
--rw-r--r--   0 runner    (1001) docker     (123)    32085 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/optimizers/optimizer_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    38993 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/optimizers/optimizer_gd.py
--rw-r--r--   0 runner    (1001) docker     (123)    11313 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/optimizers/optimizer_gpyopt.py
--rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/optimizers/optimizer_phoenics.py
--rw-r--r--   0 runner    (1001) docker     (123)    18975 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/optimizers/optimizer_scipy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 08:29:35.181701 tequila-basic-1.8.7/src/tequila/quantumchemistry/
--rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/quantumchemistry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40945 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/quantumchemistry/chemistry_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     8266 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/quantumchemistry/encodings.py
--rw-r--r--   0 runner    (1001) docker     (123)    34407 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/quantumchemistry/madness_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/quantumchemistry/orbital_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    31127 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/quantumchemistry/psi4_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/quantumchemistry/pyscf_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    86149 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/quantumchemistry/qc_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 08:29:35.185701 tequila-basic-1.8.7/src/tequila/simulators/
--rwxr-xr-x   0 runner    (1001) docker     (123)        4 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/simulators/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24177 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/simulators/simulator_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    33166 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/simulators/simulator_base.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17220 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/simulators/simulator_cirq.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24240 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/simulators/simulator_pyquil.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25119 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/simulators/simulator_qibo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23429 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/simulators/simulator_qiskit.py
--rw-r--r--   0 runner    (1001) docker     (123)    15398 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/simulators/simulator_qlm.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19546 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/simulators/simulator_qulacs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      659 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/simulators/simulator_qulacs_gpu.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5220 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/simulators/simulator_symbolic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 08:29:35.185701 tequila-basic-1.8.7/src/tequila/tools/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/tools/convenience.py
--rw-r--r--   0 runner    (1001) docker     (123)    21326 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/tools/qng.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/tools/random_generators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 08:29:35.185701 tequila-basic-1.8.7/src/tequila/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5689 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/utils/bitstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/utils/joined_transformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/utils/keymap.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 08:29:35.185701 tequila-basic-1.8.7/src/tequila/wavefunction/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/wavefunction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11881 2023-03-17 08:29:22.000000 tequila-basic-1.8.7/src/tequila/wavefunction/qubit_wavefunction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 08:29:35.185701 tequila-basic-1.8.7/src/tequila_basic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20749 2023-03-17 08:29:35.000000 tequila-basic-1.8.7/src/tequila_basic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-03-17 08:29:35.000000 tequila-basic-1.8.7/src/tequila_basic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 08:29:35.000000 tequila-basic-1.8.7/src/tequila_basic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-17 08:29:35.000000 tequila-basic-1.8.7/src/tequila_basic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-17 08:29:35.000000 tequila-basic-1.8.7/src/tequila_basic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:44:51.958609 tequila-basic-1.8.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    20749 2023-05-25 07:44:51.958609 tequila-basic-1.8.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20071 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-25 07:44:50.000000 tequila-basic-1.8.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 07:44:51.958609 tequila-basic-1.8.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:44:51.942608 tequila-basic-1.8.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:44:51.942608 tequila-basic-1.8.8/src/tequila/
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:44:51.942608 tequila-basic-1.8.8/src/tequila/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21757 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/apps/_unary_state_prep_impl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:44:51.946608 tequila-basic-1.8.8/src/tequila/apps/adapt/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/apps/adapt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19356 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/apps/adapt/adapt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:44:51.946608 tequila-basic-1.8.8/src/tequila/apps/krylov/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/apps/krylov/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/apps/krylov/krylov.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:44:51.946608 tequila-basic-1.8.8/src/tequila/apps/robustness/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/apps/robustness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/apps/robustness/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24743 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/apps/robustness/interval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/apps/unary_state_prep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/autograd_imports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:44:51.946608 tequila-basic-1.8.8/src/tequila/circuit/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/circuit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16377 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/circuit/_gates_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32044 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/circuit/circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32685 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/circuit/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35355 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/circuit/gates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/circuit/gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8322 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/circuit/noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/circuit/pyzx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15230 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/circuit/qasm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10789 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/circuit/qpic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:44:51.950608 tequila-basic-1.8.8/src/tequila/grouping/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/grouping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19406 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/grouping/binary_rep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10916 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/grouping/binary_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66415 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/grouping/compile_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8968 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/grouping/ev_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32412 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/grouping/fermionic_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27685 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/grouping/fermionic_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11059 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/grouping/overlapping_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:44:51.950608 tequila-basic-1.8.8/src/tequila/hamiltonian/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/hamiltonian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/hamiltonian/paulis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/hamiltonian/paulistring.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21401 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/hamiltonian/qubit_hamiltonian.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:44:51.950608 tequila-basic-1.8.8/src/tequila/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10023 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/ml/interface_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/ml/ml_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/ml/utils_ml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:44:51.950608 tequila-basic-1.8.8/src/tequila/objective/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/objective/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/objective/braket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31763 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/objective/objective.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/objective/qtensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:44:51.950608 tequila-basic-1.8.8/src/tequila/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/optimizers/_containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32085 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/optimizers/optimizer_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38993 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/optimizers/optimizer_gd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11313 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/optimizers/optimizer_gpyopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/optimizers/optimizer_phoenics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18975 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/optimizers/optimizer_scipy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:44:51.954609 tequila-basic-1.8.8/src/tequila/quantumchemistry/
+-rw-r--r--   0 runner    (1001) docker     (123)     7349 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/quantumchemistry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40945 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/quantumchemistry/chemistry_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8266 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/quantumchemistry/encodings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34407 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/quantumchemistry/madness_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/quantumchemistry/orbital_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29918 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/quantumchemistry/psi4_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/quantumchemistry/pyscf_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86149 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/quantumchemistry/qc_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:44:51.954609 tequila-basic-1.8.8/src/tequila/simulators/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        4 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/simulators/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24177 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/simulators/simulator_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33174 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/simulators/simulator_base.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17220 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/simulators/simulator_cirq.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24240 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/simulators/simulator_pyquil.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25119 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/simulators/simulator_qibo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23429 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/simulators/simulator_qiskit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15398 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/simulators/simulator_qlm.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19546 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/simulators/simulator_qulacs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      659 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/simulators/simulator_qulacs_gpu.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5220 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/simulators/simulator_symbolic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:44:51.954609 tequila-basic-1.8.8/src/tequila/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/tools/convenience.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21326 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/tools/qng.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/tools/random_generators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:44:51.958609 tequila-basic-1.8.8/src/tequila/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5689 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/utils/bitstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/utils/joined_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/utils/keymap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:44:51.958609 tequila-basic-1.8.8/src/tequila/wavefunction/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/wavefunction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11881 2023-05-25 07:44:38.000000 tequila-basic-1.8.8/src/tequila/wavefunction/qubit_wavefunction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:44:51.958609 tequila-basic-1.8.8/src/tequila_basic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20749 2023-05-25 07:44:51.000000 tequila-basic-1.8.8/src/tequila_basic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-05-25 07:44:51.000000 tequila-basic-1.8.8/src/tequila_basic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 07:44:51.000000 tequila-basic-1.8.8/src/tequila_basic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-25 07:44:51.000000 tequila-basic-1.8.8/src/tequila_basic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-25 07:44:51.000000 tequila-basic-1.8.8/src/tequila_basic.egg-info/top_level.txt
```

### Comparing `tequila-basic-1.8.7/LICENSE` & `tequila-basic-1.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.7/PKG-INFO` & `tequila-basic-1.8.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tequila-basic
-Version: 1.8.7
+Version: 1.8.8
 Summary: A High-Level Abstraction Framework for Quantum Algorithms
 Home-page: https://github.com/tequilahub/tequila
 Author: Jakob Kottmann and Sumner Alperin-Lea and Teresa Tamayo-Mendoza and Alba Cervera-Lierta and Cyrille Lavigne and Tzu-Ching Yen and Vladyslav Verteletskyi and Philipp Schleich and Abhinav Anand and Matthias Degroote and Skylar Chaney and Maha Kesibi and Naomi Grace Curnow and Brandon Solo and Georgios Tsilimigkounakis and Claudia Zendejas-Morales and Artur F Izmaylov and Alan Aspuru-Guzik ... 
 Author-email: jakob.kottmann@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `tequila-basic-1.8.7/README.md` & `tequila-basic-1.8.8/README.md`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.7/requirements.txt` & `tequila-basic-1.8.8/requirements.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # necessary
 numpy
 scipy >= 1.5 # can in principle be smaller, we recommend >= 1.5 for consistency with our tutorials (numerical gradients mostly)
 sympy
-jax
-jaxlib
-# autograd # use if jaxlib gives you trouble (e.g. on Windows), make sure jax and jaxlib are uninstalled and install autograd
+#jax
+#jaxlib
+autograd # autograd works better on OSX-ARM64 (M1 and M2) and Windows, feel free to try jax however (no big differences)
 setuptools
 pytest
 openfermion ~= 1.0 # can not be smaller than 1.0 
 #cmake # needed by #qulacs, can be removed otherwise, now in #qulacs requirements
 #qulacs < 0.5.0 # default simulator (best integration), remove if the installation gives you trouble and just install one of the other supported backend. Version restriction only for noise models, otherwise the new version is fine
 
 #optional quantum backends
```

### Comparing `tequila-basic-1.8.7/setup.py` & `tequila-basic-1.8.8/setup.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.7/src/tequila/__init__.py` & `tequila-basic-1.8.8/src/tequila/__init__.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.7/src/tequila/apps/__init__.py` & `tequila-basic-1.8.8/src/tequila/apps/__init__.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.7/src/tequila/apps/_unary_state_prep_impl.py` & `tequila-basic-1.8.8/src/tequila/apps/_unary_state_prep_impl.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.7/src/tequila/apps/adapt/adapt.py` & `tequila-basic-1.8.8/src/tequila/apps/adapt/adapt.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.7/src/tequila/apps/krylov/krylov.py` & `tequila-basic-1.8.8/src/tequila/apps/krylov/krylov.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.7/src/tequila/apps/robustness/helpers.py` & `tequila-basic-1.8.8/src/tequila/apps/robustness/helpers.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.7/src/tequila/apps/robustness/interval.py` & `tequila-basic-1.8.8/src/tequila/apps/robustness/interval.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.7/src/tequila/apps/unary_state_prep.py` & `tequila-basic-1.8.8/src/tequila/apps/unary_state_prep.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.7/src/tequila/circuit/_gates_impl.py` & `tequila-basic-1.8.8/src/tequila/circuit/_gates_impl.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.7/src/tequila/circuit/circuit.py` & `tequila-basic-1.8.8/src/tequila/circuit/circuit.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,18 @@
 
     def export_to(self, *args, **kwargs):
         """
         Export to png, pdf, qpic, tex with qpic backend
         Convenience: see src/tequila/circuit/qpic.py - export_to for more
         Parameters
         """
-        return export_to(circuit=self, *args, **kwargs)
+        # this way we allow calling U.export_to("asd.png") instead of having to specify U.export_to(filename="asd.png")
+        if "circuit" not in kwargs:
+            kwargs["circuit"]=self
+        return export_to(*args, **kwargs)
 
     @property
     def moments(self):
         """
         Divide self into subcircuits representing layers of simultaneous gates. Attempts to minimize gate depth.
         Returns
         -------
@@ -992,8 +995,8 @@
     # see if we can use another one
     for n in range(max(active_qubits)+1):
         if n not in active_qubits:
             free_qubit = n
             break
     assert free_qubit not in active_qubits
     
-    return free_qubit
+    return free_qubit
```

### Comparing `tequila-basic-1.8.7/src/tequila/circuit/compiler.py` & `tequila-basic-1.8.8/src/tequila/circuit/compiler.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.7/src/tequila/circuit/gates.py` & `tequila-basic-1.8.8/src/tequila/circuit/gates.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.7/src/tequila/circuit/gradient.py` & `tequila-basic-1.8.8/src/tequila/circuit/gradient.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.7/src/tequila/circuit/noise.py` & `tequila-basic-1.8.8/src/tequila/circuit/noise.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.7/src/tequila/circuit/pyzx.py` & `tequila-basic-1.8.8/src/tequila/circuit/pyzx.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.7/src/tequila/circuit/qasm.py` & `tequila-basic-1.8.8/src/tequila/circuit/qasm.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.7/src/tequila/circuit/qpic.py` & `tequila-basic-1.8.8/src/tequila/circuit/qpic.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.7/src/tequila/grouping/binary_rep.py` & `tequila-basic-1.8.8/src/tequila/grouping/binary_rep.py`

 * *Files 2% similar despite different names*

```diff
@@ -242,22 +242,22 @@
         Notes
         ----------
         Return the partitioning of the hamiltonian into commuting groups.
 
         Parameters
         ----------
         options: dictionary: Dictionary containing user-defined parameters:
-            key: method, val: 'lf' (largest first), 'rlf' (recursive largest first), 'si' (sorted insertion)
-                              'osi' [overlapping sorted insertion, i.e., ICS arXiv: 2201.01471 (2022)]
+            key: method, val: 'lf' [largest first J. Chem. Phys. 152, 124114 (2020)], 'rlf' [recursive largest first J. Chem. Phys. 152, 124114 (2020)], 
+                              'si' [sorted insertion Quantum 5, 385 (2021)], 'ics' [iterative coefficient splitting npj Quantum Inf. 9, 14 (2023)]
             key: condition, val: 'fc' (fully commuting Pauli products are measured together)
                                  'qwc' (qubit-wise commuting Pauli products are measured together)
             key: cov_dict, val: Dictionary containing {(binary_tuple of pw1, binary_tuple of pw2) : Cov (pw1, pw2)}. 
-                                Only covariances for [pw1,pw2]=0 are necessary. This dictionary is necessary for osi.
+                                Only covariances for [pw1,pw2]=0 are necessary. This dictionary is necessary for ics.
                                 For other methods, if cov_dict is given, the optimal allocation of samples will be returned.
-            key: n_iter, val: integer number of iterations in osi.
+            key: n_iter, val: integer number of iterations in ics.
 
         Returns
         ----------
         List of BinaryHamiltonian's
         """
         def process_options(options):
             method = 'rlf' # Method used for Hamiltonian partitioning.
@@ -284,15 +284,15 @@
             """
             Return the class that the method belongs to: One from Minimum clique cover (mcc)
             and Greedy grouping algorithms. 
             """
             if (method == 'lf' or method == 'rlf'): 
                 mc = 'mcc' 
                 if condition != "fc": raise TequilaException(f"Combination of options={{method:{method},condition:{condition}}} is not valid. E.g., lf and rlf can only return fully commuting fragments, i.e., condition=fc is necessary.")
-            elif (method == 'si' or method == 'osi'):
+            elif (method == 'si' or method == 'ics'):
                 mc = 'greedy'
             else:
                 raise TequilaException(f"There is not options={{method:{method}}}")
             return mc
 
         terms = self.binary_terms
         n = self.n_term
@@ -304,15 +304,15 @@
                 colors = largest_first(terms, n, cg)
             elif method == 'rlf':
                 colors = recursive_largest_first(terms, n, cg)
             groups = [value for key, value in colors.items()]
             result = [BinaryHamiltonian(value) for key, value in colors.items()]
         elif method_class(method, condition) == 'greedy':
             if method == 'si': groups = sorted_insertion_grouping(terms, condition)
-            if method == 'osi':
+            if method == 'ics':
                 if overlap_aux == None: raise TequilaException("Overlapping SI grouping requires a dictionary of covariances, call with options={cov_dict:X}, where X is the dictionary.")
                 o_groups = OverlappingGroups.init_from_binary_terms(terms, condition)
                 groups = o_groups.optimal_overlapping_groups(overlap_aux)
             result = [BinaryHamiltonian(group) for group in groups]
         
         if sample_suggestion:
             suggested_sample_size = get_opt_sample_size(groups, options["cov_dict"])
```

### Comparing `tequila-basic-1.8.7/src/tequila/grouping/binary_utils.py` & `tequila-basic-1.8.8/src/tequila/grouping/binary_utils.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.7/src/tequila/grouping/compile_groups.py` & `tequila-basic-1.8.8/src/tequila/grouping/compile_groups.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,89 @@
 from tequila.grouping.binary_rep import BinaryHamiltonian
+from tequila.grouping.fermionic_methods import get_fermion_wise, do_fff, do_svd
+from tequila.grouping.fermionic_functions import n_elec
+from tequila.utils import TequilaException
+from openfermion import reverse_jordan_wigner
 import tequila as tq
 import numpy as np
 import numpy.linalg as npl
 import copy
 
-
 def compile_commuting_parts(H, unitary_circuit="improved", *args, **kwargs):
     """
     Compile the commuting parts of a QubitHamiltonian
     Into a list of All-Z Hamiltonians and corresponding unitary rotations
     Parameters
     ----------
     H: the tq.QubitHamiltonian
 
     Returns
     -------
         A list of tuples containing all-Z Hamiltonian and corresponding Rotations
     """
-    if unitary_circuit is None or unitary_circuit.lower() == "improved":
-        # @ Zack
-        result, suggested_samples = _compile_commuting_parts_zb(H, *args, **kwargs)
+    if "options" in kwargs and not(kwargs["options"] is None) and "method" in kwargs["options"]:
+        method = kwargs["options"]["method"]
     else:
-        # original implementation of Thomson (T.C. Yen)
-        binary_H = BinaryHamiltonian.init_from_qubit_hamiltonian(H)
-        commuting_parts, suggested_samples = binary_H.commuting_groups(*args, **kwargs)
-        result = [cH.get_qubit_wise() for cH in commuting_parts]
-    return result, suggested_samples
+        method = "rlf"
+
+    def method_class(method):
+        if method == "lf" or method == "rlf" or method == "si" or method == "ics":
+            return "qubit"
+        elif method == "lr" or method == "fff-lr":
+            return "fermionic"
+    
+    if method_class(method) == 'qubit':
+        if unitary_circuit is None or unitary_circuit.lower() == "improved":
+            # @ Zack
+            result, suggested_samples = _compile_commuting_parts_zb(H, *args, **kwargs)
+        else:
+            # original implementation of Thomson (T.C. Yen)
+            binary_H = BinaryHamiltonian.init_from_qubit_hamiltonian(H)
+            commuting_parts, suggested_samples = binary_H.commuting_groups(*args, **kwargs)
+            result = [cH.get_qubit_wise() for cH in commuting_parts]
+        return result, suggested_samples
+    
+    elif method_class(method) == 'fermionic':
+        options = kwargs["options"]
+        if "n_el" in options:
+            n_el = int(options["n_el"])
+        elif "mol_name" in options: 
+            n_el = n_elec(options["mol_name"])
+        else:
+            raise TequilaException("Please specify either {mol_name:} or {n_el:} in the dictionary provided as the keyward argument (optimize_measurements) to function (ExpectationValue).")
+
+        if "reverse_H_transf" in options:
+            reverse_H_transf = options["reverse_H_transf"]
+        else:
+            print("Using default reverse_H_transf, i.e., reverse_jordan_wigner.")
+            reverse_H_transf = _reverse_jordan_wigner
+        
+        h_ferm = reverse_H_transf(H)
+
+        if method == 'lr':
+            u_ops, cartan_obt, cartan_tbt, suggested_samples = do_svd(h_ferm, n_el)
+            result = [get_fermion_wise(cartan_obt, u_ops[0])]
+            for i in range(len(cartan_tbt)):
+                result.append(get_fermion_wise(cartan_tbt[i], u_ops[i+1]))
+            return result, suggested_samples
+        elif method == 'fff-lr':
+            
+            all_ops, u_ops, cartan_obt, cartan_tbt, suggested_samples = do_fff(h_ferm, n_el, options=options, metric_estim=False)
+            result = [get_fermion_wise(cartan_obt, u_ops[0])]
+            for i in range(len(cartan_tbt)):
+                result.append(get_fermion_wise(cartan_tbt[i], u_ops[i+1]))
+            return result, suggested_samples
+
+def _reverse_jordan_wigner(H):
+    '''
+    Default funcion used by fermionic methods to obtain the H in the second quantized form.
+    The user can specify a different reverse function if H was obtained from the fermionic 
+    Hamiltonian using a mapping different than the JordanWigner transformation.
+    '''
+    return reverse_jordan_wigner(H.to_openfermion())
 
 def _compile_commuting_parts_zb(H, *args, **kwargs):
     # @ Zack add main function here and rest in this file
     # should return list of commuting Hamiltonians in Z-Form and Circuits
     # i.e. result = [(H,U), (H,U), ...]
 
     binary_H = BinaryHamiltonian.init_from_qubit_hamiltonian(H)
```

### Comparing `tequila-basic-1.8.7/src/tequila/grouping/overlapping_methods.py` & `tequila-basic-1.8.8/src/tequila/grouping/overlapping_methods.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.7/src/tequila/hamiltonian/paulis.py` & `tequila-basic-1.8.8/src/tequila/hamiltonian/paulis.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.7/src/tequila/hamiltonian/qubit_hamiltonian.py` & `tequila-basic-1.8.8/src/tequila/hamiltonian/qubit_hamiltonian.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.7/src/tequila/ml/interface_torch.py` & `tequila-basic-1.8.8/src/tequila/ml/interface_torch.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.7/src/tequila/ml/ml_api.py` & `tequila-basic-1.8.8/src/tequila/ml/ml_api.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.7/src/tequila/ml/utils_ml.py` & `tequila-basic-1.8.8/src/tequila/ml/utils_ml.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.7/src/tequila/objective/braket.py` & `tequila-basic-1.8.8/src/tequila/objective/braket.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.7/src/tequila/objective/objective.py` & `tequila-basic-1.8.8/src/tequila/objective/objective.py`

 * *Files 0% similar despite different names*

```diff
@@ -981,8 +981,9 @@
     def __str__(self):
         result = ""
         for k, v in self.items():
             result += "{} : {}\n".format(str(k), str(v))
         return result
 
     def __repr__(self):
-        return self.__str__()
+        xdict = {k:v for k,v in self.items()}
+        return xdict.__repr__()
```

### Comparing `tequila-basic-1.8.7/src/tequila/objective/qtensor.py` & `tequila-basic-1.8.8/src/tequila/objective/qtensor.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.7/src/tequila/optimizers/__init__.py` & `tequila-basic-1.8.8/src/tequila/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.7/src/tequila/optimizers/_containers.py` & `tequila-basic-1.8.8/src/tequila/optimizers/_containers.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.7/src/tequila/optimizers/optimizer_base.py` & `tequila-basic-1.8.8/src/tequila/optimizers/optimizer_base.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.7/src/tequila/optimizers/optimizer_gd.py` & `tequila-basic-1.8.8/src/tequila/optimizers/optimizer_gd.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.7/src/tequila/optimizers/optimizer_gpyopt.py` & `tequila-basic-1.8.8/src/tequila/optimizers/optimizer_gpyopt.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.7/src/tequila/optimizers/optimizer_phoenics.py` & `tequila-basic-1.8.8/src/tequila/optimizers/optimizer_phoenics.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.7/src/tequila/optimizers/optimizer_scipy.py` & `tequila-basic-1.8.8/src/tequila/optimizers/optimizer_scipy.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.7/src/tequila/quantumchemistry/__init__.py` & `tequila-basic-1.8.8/src/tequila/quantumchemistry/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,14 +66,21 @@
     kwargs
 
     Returns
     -------
         The Fermion to Qubit Transformation (jordan-wigner, bravyi-kitaev, bravyi-kitaev-tree and whatever OpenFermion supports)
     """
 
+    # failsafe for common mistake
+    if "basis" in kwargs:
+        warnings.warn("called molecule with keyword \"basis={0}\" converting it to \"basis_set={0}\"".format(kwargs["basis"]), TequilaWarning)
+        if basis_set is not None:
+            warnings.warn("did not convert as \"basis_set={}\" was already given".format(basis_set), TequilaWarning)
+        basis_set=kwargs["basis"]
+    
     keyvals = {}
     for k, v in kwargs.items():
         if k in ParametersQC.__dict__.keys():
             keyvals[k] = v
 
     if "parameters" in kwargs:
         parameters = kwargs["parameters"]
```

### Comparing `tequila-basic-1.8.7/src/tequila/quantumchemistry/chemistry_tools.py` & `tequila-basic-1.8.8/src/tequila/quantumchemistry/chemistry_tools.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.7/src/tequila/quantumchemistry/encodings.py` & `tequila-basic-1.8.8/src/tequila/quantumchemistry/encodings.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.7/src/tequila/quantumchemistry/madness_interface.py` & `tequila-basic-1.8.8/src/tequila/quantumchemistry/madness_interface.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.7/src/tequila/quantumchemistry/orbital_optimizer.py` & `tequila-basic-1.8.8/src/tequila/quantumchemistry/orbital_optimizer.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.7/src/tequila/quantumchemistry/psi4_interface.py` & `tequila-basic-1.8.8/src/tequila/quantumchemistry/psi4_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -365,48 +365,14 @@
         # set some psi4 specific features
         self.ref_energy = hf_energy
         self.ref_wfn = self.logs['hf'].wfn
         self.irreps = irreps
 
         return super().initialize_integral_manager(*args, **kwargs)
 
-    def compute_one_body_integrals(self, ref_wfn=None):
-        if ref_wfn is None:
-            self.compute_energy(method="hf")
-            ref_wfn = self.logs['hf'].wfn
-        if ref_wfn.nirrep() != 1:
-            wfn = ref_wfn.c1_deep_copy(ref_wfn.basisset())
-        else:
-            wfn = ref_wfn
-        Ca = numpy.asarray(wfn.Ca())
-        h = wfn.H()
-        h = numpy.einsum("xy, yi -> xi", h, Ca, optimize='greedy')
-        h = numpy.einsum("xj, xi -> ji", Ca, h, optimize='greedy')
-        return h
-
-    def compute_two_body_integrals(self, ref_wfn=None, ordering='openfermion'):
-        if ref_wfn is None:
-            if 'hf' not in self.logs:
-                self.compute_energy(method="hf")
-            ref_wfn = self.logs['hf'].wfn
-
-        if ref_wfn.nirrep() != 1:
-            wfn = ref_wfn.c1_deep_copy(ref_wfn.basisset())
-        else:
-            wfn = ref_wfn
-
-        mints = psi4.core.MintsHelper(wfn.basisset())
-
-        # Molecular orbitals (coeffs)
-        Ca = wfn.Ca()
-        h = NBodyTensor(elems=numpy.asarray(mints.mo_eri(Ca, Ca, Ca, Ca)), ordering='chem')
-        # Order tensor. default: meet openfermion conventions
-        h.reorder(to=ordering)
-        return h.elems
-
     def compute_ccsd_amplitudes(self):
         return self.compute_amplitudes(method='ccsd')
 
     def _run_psi4(self, options: dict, method=None, return_wfn=True, point_group=None, filename: str = None,
                   guess_wfn=None, ref_wfn=None, ignore_active_space=False, *args, **kwargs):
         psi4.core.clean()
         psi4.core.clean_variables()
```

### Comparing `tequila-basic-1.8.7/src/tequila/quantumchemistry/pyscf_interface.py` & `tequila-basic-1.8.8/src/tequila/quantumchemistry/pyscf_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
                 point_group = kwargs["point_group"]
             else:
                 point_group = None
 
             mol = pyscf.gto.Mole()
             mol.atom = pyscf_geomstring
             mol.basis = parameters.basis_set
+            mol.charge = parameters.charge
 
             if point_group is not None:
                 if point_group.lower() != "c1":
                     mol.symmetry = True
                     mol.symmetry_subgroup = point_group
                 else:
                     mol.symmetry = False
```

### Comparing `tequila-basic-1.8.7/src/tequila/quantumchemistry/qc_base.py` & `tequila-basic-1.8.8/src/tequila/quantumchemistry/qc_base.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.7/src/tequila/simulators/simulator_api.py` & `tequila-basic-1.8.8/src/tequila/simulators/simulator_api.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.7/src/tequila/simulators/simulator_base.py` & `tequila-basic-1.8.8/src/tequila/simulators/simulator_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -841,15 +841,15 @@
         """
 
         suggested = None
         if hasattr(samples, "lower") and samples.lower()[:4] == "auto":
             if self.abstract_expectationvalue.samples is None:
                 raise TequilaException("samples='auto' requested but no samples where set in individual expectation values")
             total_samples = int(samples[5:])
-            samples = int(self.abstract_expectationvalue.samples * total_samples)
+            samples = max(1, int(self.abstract_expectationvalue.samples * total_samples))
             suggested = samples
             # samples are not necessarily set (either the user has to set it or some functions like optimize_measurements)
  
         if suggested is not None and suggested != samples:
             warnings.warn("simulating with samples={}, but expectationvalue carries suggested samples={}\nTry calling with samples='auto-total#ofsamples'".format(samples, suggested), TequilaWarning)
 
         self.update_variables(variables)
```

### Comparing `tequila-basic-1.8.7/src/tequila/simulators/simulator_cirq.py` & `tequila-basic-1.8.8/src/tequila/simulators/simulator_cirq.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.7/src/tequila/simulators/simulator_pyquil.py` & `tequila-basic-1.8.8/src/tequila/simulators/simulator_pyquil.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.7/src/tequila/simulators/simulator_qibo.py` & `tequila-basic-1.8.8/src/tequila/simulators/simulator_qibo.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.7/src/tequila/simulators/simulator_qiskit.py` & `tequila-basic-1.8.8/src/tequila/simulators/simulator_qiskit.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.7/src/tequila/simulators/simulator_qlm.py` & `tequila-basic-1.8.8/src/tequila/simulators/simulator_qlm.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.7/src/tequila/simulators/simulator_qulacs.py` & `tequila-basic-1.8.8/src/tequila/simulators/simulator_qulacs.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.7/src/tequila/simulators/simulator_qulacs_gpu.py` & `tequila-basic-1.8.8/src/tequila/simulators/simulator_qulacs_gpu.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.7/src/tequila/simulators/simulator_symbolic.py` & `tequila-basic-1.8.8/src/tequila/simulators/simulator_symbolic.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.7/src/tequila/tools/convenience.py` & `tequila-basic-1.8.8/src/tequila/tools/convenience.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.7/src/tequila/tools/qng.py` & `tequila-basic-1.8.8/src/tequila/tools/qng.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.7/src/tequila/tools/random_generators.py` & `tequila-basic-1.8.8/src/tequila/tools/random_generators.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.7/src/tequila/utils/bitstrings.py` & `tequila-basic-1.8.8/src/tequila/utils/bitstrings.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.7/src/tequila/utils/exceptions.py` & `tequila-basic-1.8.8/src/tequila/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.7/src/tequila/utils/joined_transformation.py` & `tequila-basic-1.8.8/src/tequila/utils/joined_transformation.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.7/src/tequila/utils/keymap.py` & `tequila-basic-1.8.8/src/tequila/utils/keymap.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.7/src/tequila/utils/misc.py` & `tequila-basic-1.8.8/src/tequila/utils/misc.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.7/src/tequila/wavefunction/qubit_wavefunction.py` & `tequila-basic-1.8.8/src/tequila/wavefunction/qubit_wavefunction.py`

 * *Files identical despite different names*

### Comparing `tequila-basic-1.8.7/src/tequila_basic.egg-info/PKG-INFO` & `tequila-basic-1.8.8/src/tequila_basic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tequila-basic
-Version: 1.8.7
+Version: 1.8.8
 Summary: A High-Level Abstraction Framework for Quantum Algorithms
 Home-page: https://github.com/tequilahub/tequila
 Author: Jakob Kottmann and Sumner Alperin-Lea and Teresa Tamayo-Mendoza and Alba Cervera-Lierta and Cyrille Lavigne and Tzu-Ching Yen and Vladyslav Verteletskyi and Philipp Schleich and Abhinav Anand and Matthias Degroote and Skylar Chaney and Maha Kesibi and Naomi Grace Curnow and Brandon Solo and Georgios Tsilimigkounakis and Claudia Zendejas-Morales and Artur F Izmaylov and Alan Aspuru-Guzik ... 
 Author-email: jakob.kottmann@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `tequila-basic-1.8.7/src/tequila_basic.egg-info/SOURCES.txt` & `tequila-basic-1.8.8/src/tequila_basic.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -26,14 +26,17 @@
 src/tequila/circuit/pyzx.py
 src/tequila/circuit/qasm.py
 src/tequila/circuit/qpic.py
 src/tequila/grouping/__init__.py
 src/tequila/grouping/binary_rep.py
 src/tequila/grouping/binary_utils.py
 src/tequila/grouping/compile_groups.py
+src/tequila/grouping/ev_utils.py
+src/tequila/grouping/fermionic_functions.py
+src/tequila/grouping/fermionic_methods.py
 src/tequila/grouping/overlapping_methods.py
 src/tequila/hamiltonian/__init__.py
 src/tequila/hamiltonian/paulis.py
 src/tequila/hamiltonian/paulistring.py
 src/tequila/hamiltonian/qubit_hamiltonian.py
 src/tequila/ml/__init__.py
 src/tequila/ml/interface_torch.py
```

