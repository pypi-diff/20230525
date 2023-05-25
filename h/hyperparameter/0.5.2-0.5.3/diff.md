# Comparing `tmp/hyperparameter-0.5.2.tar.gz` & `tmp/hyperparameter-0.5.3.tar.gz`

## Comparing `hyperparameter-0.5.2.tar` & `hyperparameter-0.5.3.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0      442 1970-01-01 00:00:00.000000 hyperparameter-0.5.2/Cargo.toml
--rw-r--r--   0     1001      123      834 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0     1001      123      126 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/.github/ISSUE_TEMPLATE/custom.md
--rw-r--r--   0     1001      123      595 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0     1001      123      706 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/.github/workflows/codecov.yml
--rw-r--r--   0     1001      123      845 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/.github/workflows/mkdocs.yml
--rw-r--r--   0     1001      123     1202 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/.github/workflows/python-publish.yml
--rw-r--r--   0     1001      123     2001 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/.gitignore
--rw-r--r--   0     1001      123      356 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/.pre-commit-config.yaml
--rw-r--r--   0     1001      123     5202 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/CODE_OF_CONDUCT.md
--rw-r--r--   0     1001      123    22513 2023-05-23 05:58:25.000000 hyperparameter-0.5.2/Cargo.lock
--rw-r--r--   0     1001      123    11356 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/LICENSE
--rw-r--r--   0     1001      123     3861 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/README.md
--rw-r--r--   0     1001      123     3457 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/README.zh.md
--rw-r--r--   0     1001      123     2846 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/docs/examples/optimization.md
--rw-r--r--   0     1001      123     2868 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/docs/examples/optimization.zh.md
--rw-r--r--   0     1001      123     3861 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/docs/index.md
--rw-r--r--   0     1001      123     3457 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/docs/index.zh.md
--rw-r--r--   0     1001      123     3000 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/docs/quick_start.md
--rw-r--r--   0     1001      123     3000 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/docs/quick_start.zh.md
--rw-r--r--   0     1001      123       48 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/docs/reference.md
--rw-r--r--   0     1001      123      110 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/docs/requirements.txt
--rw-r--r--   0     1001      123     6738 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/docs/structured_parameter.md
--rw-r--r--   0     1001      123      337 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/examples/application/README.md
--rw-r--r--   0     1001      123      789 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/examples/application/app.py
--rw-r--r--   0     1001      123       46 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/examples/application/cfg.json
--rw-r--r--   0     1001      123     4733 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/examples/automl_optuna_mnist/automl_mnist.py
--rw-r--r--   0     1001      123     2047 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/examples/cpp/cxx_test.cc
--rw-r--r--   0     1001      123      271 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/examples/cpp/cxx_test.py
--rw-r--r--   0     1001      123      237 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/examples/cpp/cxx_test.sh
--rw-r--r--   0     1001      123      152 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/examples/mnist/README.md
--rw-r--r--   0     1001      123     5625 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/examples/mnist/main.py
--rw-r--r--   0     1001      123     5899 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/examples/mnist/main_with_hp.py
--rw-r--r--   0     1001      123     6202 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/examples/mnist/main_with_hp_with_mlflow.py
--rw-r--r--   0     1001      123       18 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/examples/mnist/requirements.txt
--rw-r--r--   0     1001      123     2846 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/examples/optuna/README.md
--rw-r--r--   0     1001      123      230 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/examples/optuna/example.py
--rw-r--r--   0     1001      123      527 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/examples/optuna/example_hp.py
--rw-r--r--   0     1001      123      727 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/examples/optuna/example_hp_nested.py
--rw-r--r--   0     1001      123     1650 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/examples/sparse_lr/README.md
--rw-r--r--   0     1001      123      581 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/examples/sparse_lr/example_1.py
--rw-r--r--   0     1001      123      934 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/examples/sparse_lr/example_2.py
--rw-r--r--   0     1001      123     1059 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/examples/sparse_lr/example_mlflow.py
--rw-r--r--   0     1001      123      867 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/examples/sparse_lr/model.py
--rw-r--r--   0     1001      123     1631 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/examples/storage.rs
--rw-r--r--   0     1001      123        0 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/hparam/__init__.py
--rw-r--r--   0     1001      123     3710 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/hparam/__main__.py
--rw-r--r--   0     1001      123      314 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/hyperparameter/__init__.py
--rw-r--r--   0     1001      123    17127 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/hyperparameter/api.py
--rw-r--r--   0     1001      123     7588 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/hyperparameter/hyperparameter.h
--rw-r--r--   0     1001      123      828 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/hyperparameter/loader.py
--rw-r--r--   0     1001      123     4196 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/hyperparameter/storage.py
--rw-r--r--   0     1001      123     2223 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/hyperparameter/tune.py
--rw-r--r--   0     1001      123     1249 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/mkdocs.yml
--rw-r--r--   0     1001      123      938 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/pyproject.toml
--rw-r--r--   0     1001      123     5460 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/src/entry.rs
--rw-r--r--   0     1001      123     6580 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/src/ext.rs
--rw-r--r--   0     1001      123     2038 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/src/ffi.rs
--rw-r--r--   0     1001      123      106 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/src/lib.rs
--rw-r--r--   0     1001      123     8129 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/src/storage.rs
--rw-r--r--   0     1001      123     4528 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/src/xxh.rs
--rwxr-xr-x   0     1001      123    40754 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/tests/a.out
--rw-r--r--   0     1001      123      912 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/tests/test_auto_param.py
--rw-r--r--   0     1001      123     3769 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/tests/test_param_scope.py
--rw-r--r--   0     1001      123      697 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/tests/test_param_scope_thread.py
--rw-r--r--   0     1001      123     2988 2023-05-23 05:58:15.000000 hyperparameter-0.5.2/tests/test_rust_backend.py
--rw-r--r--   0        0        0     4210 1970-01-01 00:00:00.000000 hyperparameter-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0      492 1970-01-01 00:00:00.000000 hyperparameter-0.5.3/Cargo.toml
+-rw-r--r--   0     1001      123      834 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0     1001      123      126 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/.github/ISSUE_TEMPLATE/custom.md
+-rw-r--r--   0     1001      123      595 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0     1001      123      706 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/.github/workflows/codecov.yml
+-rw-r--r--   0     1001      123      845 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/.github/workflows/mkdocs.yml
+-rw-r--r--   0     1001      123     1202 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/.github/workflows/python-publish.yml
+-rw-r--r--   0     1001      123     2001 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/.gitignore
+-rw-r--r--   0     1001      123      356 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/.pre-commit-config.yaml
+-rw-r--r--   0     1001      123     5202 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0     1001      123    24124 2023-05-25 06:08:41.000000 hyperparameter-0.5.3/Cargo.lock
+-rw-r--r--   0     1001      123    11356 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/LICENSE
+-rw-r--r--   0     1001      123     3861 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/README.md
+-rw-r--r--   0     1001      123     3457 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/README.zh.md
+-rw-r--r--   0     1001      123     2846 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/docs/examples/optimization.md
+-rw-r--r--   0     1001      123     2868 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/docs/examples/optimization.zh.md
+-rw-r--r--   0     1001      123     3861 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/docs/index.md
+-rw-r--r--   0     1001      123     3457 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/docs/index.zh.md
+-rw-r--r--   0     1001      123     3000 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/docs/quick_start.md
+-rw-r--r--   0     1001      123     3000 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/docs/quick_start.zh.md
+-rw-r--r--   0     1001      123       48 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/docs/reference.md
+-rw-r--r--   0     1001      123      110 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/docs/requirements.txt
+-rw-r--r--   0     1001      123     6738 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/docs/structured_parameter.md
+-rw-r--r--   0     1001      123      337 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/examples/application/README.md
+-rw-r--r--   0     1001      123      789 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/examples/application/app.py
+-rw-r--r--   0     1001      123       46 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/examples/application/cfg.json
+-rw-r--r--   0     1001      123     4733 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/examples/automl_optuna_mnist/automl_mnist.py
+-rw-r--r--   0     1001      123     2737 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/examples/cpp/cxx_test.cc
+-rw-r--r--   0     1001      123      433 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/examples/cpp/cxx_test.py
+-rw-r--r--   0     1001      123      237 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/examples/cpp/cxx_test.sh
+-rw-r--r--   0     1001      123      152 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/examples/mnist/README.md
+-rw-r--r--   0     1001      123     5625 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/examples/mnist/main.py
+-rw-r--r--   0     1001      123     5899 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/examples/mnist/main_with_hp.py
+-rw-r--r--   0     1001      123     6202 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/examples/mnist/main_with_hp_with_mlflow.py
+-rw-r--r--   0     1001      123       18 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/examples/mnist/requirements.txt
+-rw-r--r--   0     1001      123     2846 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/examples/optuna/README.md
+-rw-r--r--   0     1001      123      230 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/examples/optuna/example.py
+-rw-r--r--   0     1001      123      527 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/examples/optuna/example_hp.py
+-rw-r--r--   0     1001      123      727 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/examples/optuna/example_hp_nested.py
+-rw-r--r--   0     1001      123     1650 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/examples/sparse_lr/README.md
+-rw-r--r--   0     1001      123      581 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/examples/sparse_lr/example_1.py
+-rw-r--r--   0     1001      123      934 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/examples/sparse_lr/example_2.py
+-rw-r--r--   0     1001      123     1059 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/examples/sparse_lr/example_mlflow.py
+-rw-r--r--   0     1001      123      867 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/examples/sparse_lr/model.py
+-rw-r--r--   0     1001      123     1631 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/examples/storage.rs
+-rw-r--r--   0     1001      123        0 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/hparam/__init__.py
+-rw-r--r--   0     1001      123     3710 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/hparam/__main__.py
+-rw-r--r--   0     1001      123      314 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/hyperparameter/__init__.py
+-rw-r--r--   0     1001      123    17127 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/hyperparameter/api.py
+-rw-r--r--   0     1001      123     7715 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/hyperparameter/hyperparameter.h
+-rw-r--r--   0     1001      123      828 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/hyperparameter/loader.py
+-rw-r--r--   0     1001      123     4196 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/hyperparameter/storage.py
+-rw-r--r--   0     1001      123     2223 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/hyperparameter/tune.py
+-rw-r--r--   0     1001      123     1249 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/mkdocs.yml
+-rw-r--r--   0     1001      123      938 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/pyproject.toml
+-rw-r--r--   0     1001      123     6151 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/src/entry.rs
+-rw-r--r--   0     1001      123     6580 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/src/ext.rs
+-rw-r--r--   0     1001      123     2038 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/src/ffi.rs
+-rw-r--r--   0     1001      123      106 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/src/lib.rs
+-rw-r--r--   0     1001      123     8129 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/src/storage.rs
+-rw-r--r--   0     1001      123     4528 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/src/xxh.rs
+-rwxr-xr-x   0     1001      123    40754 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/tests/a.out
+-rw-r--r--   0     1001      123      912 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/tests/test_auto_param.py
+-rw-r--r--   0     1001      123     3769 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/tests/test_param_scope.py
+-rw-r--r--   0     1001      123      697 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/tests/test_param_scope_thread.py
+-rw-r--r--   0     1001      123     2988 2023-05-25 06:08:26.000000 hyperparameter-0.5.3/tests/test_rust_backend.py
+-rw-r--r--   0        0        0     4210 1970-01-01 00:00:00.000000 hyperparameter-0.5.3/PKG-INFO
```

### Comparing `hyperparameter-0.5.2/.github/ISSUE_TEMPLATE/bug_report.md` & `hyperparameter-0.5.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.2/.github/ISSUE_TEMPLATE/feature_request.md` & `hyperparameter-0.5.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.2/.github/workflows/codecov.yml` & `hyperparameter-0.5.3/.github/workflows/codecov.yml`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.2/.github/workflows/mkdocs.yml` & `hyperparameter-0.5.3/.github/workflows/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.2/.github/workflows/python-publish.yml` & `hyperparameter-0.5.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.2/.gitignore` & `hyperparameter-0.5.3/.gitignore`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.2/CODE_OF_CONDUCT.md` & `hyperparameter-0.5.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.2/Cargo.lock` & `hyperparameter-0.5.3/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -247,14 +247,15 @@
 
 [[package]]
 name = "hyperparameter"
 version = "0.5.2"
 dependencies = [
  "cxx",
  "lazy_static",
+ "phf",
  "pyo3",
  "rspec",
 ]
 
 [[package]]
 name = "ident_case"
 version = "1.0.1"
@@ -358,14 +359,56 @@
  "libc",
  "redox_syscall",
  "smallvec",
  "windows-sys",
 ]
 
 [[package]]
+name = "phf"
+version = "0.11.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "928c6535de93548188ef63bb7c4036bd415cd8f36ad25af44b9789b2ee72a48c"
+dependencies = [
+ "phf_macros",
+ "phf_shared",
+]
+
+[[package]]
+name = "phf_generator"
+version = "0.11.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b1181c94580fa345f50f19d738aaa39c0ed30a600d95cb2d3e23f94266f14fbf"
+dependencies = [
+ "phf_shared",
+ "rand",
+]
+
+[[package]]
+name = "phf_macros"
+version = "0.11.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "92aacdc5f16768709a569e913f7451034034178b05bdc8acda226659a3dccc66"
+dependencies = [
+ "phf_generator",
+ "phf_shared",
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+]
+
+[[package]]
+name = "phf_shared"
+version = "0.11.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e1fb5f6f826b772a8d4c0394209441e7d37cbbb967ae9c7e0e8134365c9ee676"
+dependencies = [
+ "siphasher",
+]
+
+[[package]]
 name = "proc-macro-hack"
 version = "0.5.20+deprecated"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc375e1527247fe1a97d8b7156678dfe7c1af2fc075c9a4db3690ecd2a148068"
 
 [[package]]
 name = "proc-macro2"
@@ -442,14 +485,29 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f4f29d145265ec1c483c7c654450edde0bfe043d3938d6972630663356d9500"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
+name = "rand"
+version = "0.8.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "34af8d1a0e25924bc5b7c43c079c942339d8f0a8b57c39049bef581b46327404"
+dependencies = [
+ "rand_core",
+]
+
+[[package]]
+name = "rand_core"
+version = "0.6.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ec0be4795e2f6a28069bec0b5ff3e2ac9bafc99e6a9a7dc3547996c5c816922c"
+
+[[package]]
 name = "rayon"
 version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1d2df5196e37bcc87abebc0053e20787d73847bb33134a69841207dd0a47f03b"
 dependencies = [
  "either",
  "rayon-core",
@@ -565,14 +623,20 @@
 [[package]]
 name = "sha1_smol"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ae1a47186c03a32177042e55dbc5fd5aee900b8e0069a8d70fba96a9375cd012"
 
 [[package]]
+name = "siphasher"
+version = "0.3.10"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7bd3e3206899af3f8b12af284fafc038cc1dc2b41d1b89dd17297221c5d225de"
+
+[[package]]
 name = "smallvec"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
 
 [[package]]
 name = "standback"
@@ -702,17 +766,17 @@
  "quote",
  "standback",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.8"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
+checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
 
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
```

### Comparing `hyperparameter-0.5.2/LICENSE` & `hyperparameter-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.2/README.md` & `hyperparameter-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.2/README.zh.md` & `hyperparameter-0.5.3/README.zh.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.2/docs/examples/optimization.md` & `hyperparameter-0.5.3/docs/examples/optimization.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.2/docs/examples/optimization.zh.md` & `hyperparameter-0.5.3/docs/examples/optimization.zh.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.2/docs/index.md` & `hyperparameter-0.5.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.2/docs/index.zh.md` & `hyperparameter-0.5.3/docs/index.zh.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.2/docs/quick_start.md` & `hyperparameter-0.5.3/docs/quick_start.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.2/docs/quick_start.zh.md` & `hyperparameter-0.5.3/docs/quick_start.zh.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.2/docs/structured_parameter.md` & `hyperparameter-0.5.3/docs/structured_parameter.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.2/examples/application/app.py` & `hyperparameter-0.5.3/examples/application/app.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.2/examples/automl_optuna_mnist/automl_mnist.py` & `hyperparameter-0.5.3/examples/automl_optuna_mnist/automl_mnist.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.2/examples/mnist/main.py` & `hyperparameter-0.5.3/examples/mnist/main.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.2/examples/mnist/main_with_hp.py` & `hyperparameter-0.5.3/examples/mnist/main_with_hp.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.2/examples/mnist/main_with_hp_with_mlflow.py` & `hyperparameter-0.5.3/examples/mnist/main_with_hp_with_mlflow.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.2/examples/optuna/README.md` & `hyperparameter-0.5.3/examples/optuna/README.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.2/examples/optuna/example_hp.py` & `hyperparameter-0.5.3/examples/optuna/example_hp.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.2/examples/optuna/example_hp_nested.py` & `hyperparameter-0.5.3/examples/optuna/example_hp_nested.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.2/examples/sparse_lr/README.md` & `hyperparameter-0.5.3/examples/sparse_lr/README.md`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.2/examples/sparse_lr/example_1.py` & `hyperparameter-0.5.3/examples/sparse_lr/example_1.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.2/examples/sparse_lr/example_2.py` & `hyperparameter-0.5.3/examples/sparse_lr/example_2.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.2/examples/sparse_lr/example_mlflow.py` & `hyperparameter-0.5.3/examples/sparse_lr/example_mlflow.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.2/examples/sparse_lr/model.py` & `hyperparameter-0.5.3/examples/sparse_lr/model.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.2/examples/storage.rs` & `hyperparameter-0.5.3/examples/storage.rs`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.2/hparam/__main__.py` & `hyperparameter-0.5.3/hparam/__main__.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.2/hyperparameter/api.py` & `hyperparameter-0.5.3/hyperparameter/api.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.2/hyperparameter/hyperparameter.h` & `hyperparameter-0.5.3/hyperparameter/hyperparameter.h`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
     struct xxh64
     {
         static constexpr uint64_t hash(const char *p, uint64_t len, uint64_t seed = 42)
         {
             return finalize((len >= 32 ? h32bytes(p, len, seed) : seed + PRIME5) + len, p + (len & ~0x1F), len & 0x1F);
         }
-        
+
     private:
         static constexpr uint64_t PRIME1 = 11400714785074694791ULL;
         static constexpr uint64_t PRIME2 = 14029467366897019727ULL;
         static constexpr uint64_t PRIME3 = 1609587929392839161ULL;
         static constexpr uint64_t PRIME4 = 9650029242287828579ULL;
         static constexpr uint64_t PRIME5 = 2870177450012600261ULL;
 
@@ -94,118 +94,120 @@
 
     struct Hyperparameter
     {
         Storage *_storage;
         Hyperparameter() : _storage(hyper_create_storage()) {}
         ~Hyperparameter() { hyper_destory_storage(_storage); }
 
-        void enter() { storage_enter(_storage); }
-        void exit() { storage_exit(_storage); }
+        inline void enter() { storage_enter(_storage); }
+        inline void exit() { storage_exit(_storage); }
 
         template <typename T>
-        T get(uint64_t key, T def);
+        inline T get(uint64_t key, T def);
 
         template <typename T>
-        T get(const std::string &key, T def) { return get(key.c_str(), key.size(), def); }
+        inline T get(const std::string &key, T def) { return get(key.c_str(), key.size(), def); }
 
         template <typename T>
-        T get(const char *key, int keylen, T def) { return get(xxhash(key, keylen), def); }
+        inline T get(const char *key, int keylen, T def) { return get(xxhash(key, keylen), def); }
 
         template <typename T>
-        void put(const std::string &key, T val) { put(key.c_str(), val); }
+        inline void put(const std::string &key, T val) { put(key.c_str(), val); }
 
         template <typename T>
-        void put(const char *key, T val);
+        inline void put(const char *key, T val);
     };
 
-    Hyperparameter *create() { return new Hyperparameter(); }
-    std::shared_ptr<Hyperparameter> create_shared() { return std::make_shared<Hyperparameter>(); }
+    inline Hyperparameter *create() { return new Hyperparameter(); }
+    inline std::shared_ptr<Hyperparameter> create_shared() { return std::make_shared<Hyperparameter>(); }
 
     template <>
-    int64_t Hyperparameter::get<int64_t>(uint64_t key, int64_t def)
+    inline int64_t Hyperparameter::get<int64_t>(uint64_t key, int64_t def)
     {
         return storage_hget_or_i64(_storage, key, def);
     }
 
     template <>
-    int32_t Hyperparameter::get<int32_t>(uint64_t key, int32_t def)
+    inline int32_t Hyperparameter::get<int32_t>(uint64_t key, int32_t def)
     {
         return storage_hget_or_i64(_storage, key, def);
     }
 
     template <>
-    double Hyperparameter::get<double>(uint64_t key, double def)
+    inline double Hyperparameter::get<double>(uint64_t key, double def)
     {
         return storage_hget_or_f64(_storage, key, def);
     }
 
     template <>
-    bool Hyperparameter::get<bool>(uint64_t key, bool def)
+    inline bool Hyperparameter::get<bool>(uint64_t key, bool def)
     {
         return storage_hget_or_bool(_storage, key, def);
     }
 
     template <>
-    std::string Hyperparameter::get<std::string>(uint64_t key, std::string def)
+    inline std::string Hyperparameter::get<std::string>(uint64_t key, std::string def)
     {
         return std::string(storage_hget_or_str(_storage, key, def.c_str()));
     }
 
     template <>
-    const char *Hyperparameter::get<const char *>(uint64_t key, const char *def)
+    inline const char *Hyperparameter::get<const char *>(uint64_t key, const char *def)
     {
         return storage_hget_or_str(_storage, key, def);
     }
 
     template <>
-    void Hyperparameter::put<int64_t>(const char *key, int64_t val)
+    inline void Hyperparameter::put<int64_t>(const char *key, int64_t val)
     {
         return storage_put_i64(_storage, key, val);
     }
 
     template <>
-    void Hyperparameter::put<int32_t>(const char *key, int32_t val)
+    inline void Hyperparameter::put<int32_t>(const char *key, int32_t val)
     {
         return storage_put_i64(_storage, key, val);
     }
 
     template <>
-    void Hyperparameter::put<double>(const char *key, double val)
+    inline void Hyperparameter::put<double>(const char *key, double val)
     {
         return storage_put_f64(_storage, key, val);
     }
 
     template <>
-    void Hyperparameter::put<bool>(const char *key, bool val)
+    inline void Hyperparameter::put<bool>(const char *key, bool val)
     {
         return storage_put_bool(_storage, key, val);
     }
 
     template <>
-    void Hyperparameter::put<const std::string &>(const char *key, const std::string &val)
+    inline void Hyperparameter::put<const std::string &>(const char *key, const std::string &val)
     {
         return storage_put_str(_storage, key, val.c_str());
     }
 
     template <>
-    void Hyperparameter::put<const char *>(const char *key, const char *val)
+    inline void Hyperparameter::put<const char *>(const char *key, const char *val)
     {
         return storage_put_str(_storage, key, val);
     }
 
-    std::shared_ptr<hyperparameter::Hyperparameter> get_hp() {
-      static std::shared_ptr<Hyperparameter> hp;
-      if (!hp) {
-        hp = hyperparameter::create_shared();
-      }
-      return hp;
+    inline std::shared_ptr<hyperparameter::Hyperparameter> get_hp()
+    {
+        static std::shared_ptr<Hyperparameter> hp;
+        if (!hp)
+        {
+            hp = hyperparameter::create_shared();
+        }
+        return hp;
     }
 }
 
-#define GETHP hyperparameter::get_hp()  
+#define GETHP hyperparameter::get_hp()
 
 // Implicit create hyperparameter object
-#define GETPARAM(p, default_val)                                              \
-  (GETHP->get(([](){ constexpr uint64_t x = hyperparameter::xxhash(#p,sizeof(#p)-1); return x;})(), default_val))
+#define GETPARAM(p, default_val) \
+    (GETHP->get(([]() { constexpr uint64_t x = hyperparameter::xxhash(#p,sizeof(#p)-1); return x; })(), default_val))
 #define PUTPARAM(p, default_val) (GETHP->put(#p, default_val))
 
 #endif
```

### Comparing `hyperparameter-0.5.2/hyperparameter/loader.py` & `hyperparameter-0.5.3/hyperparameter/loader.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.2/hyperparameter/storage.py` & `hyperparameter-0.5.3/hyperparameter/storage.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.2/hyperparameter/tune.py` & `hyperparameter-0.5.3/hyperparameter/tune.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.2/mkdocs.yml` & `hyperparameter-0.5.3/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.2/pyproject.toml` & `hyperparameter-0.5.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=0.14,<0.15"]
 build-backend = "maturin"
 
 [project]
 name = "hyperparameter"
-version = "0.5.2"
+version = "0.5.3"
 authors = [{ name = "Reiase", email = "reiase@gmail.com" }]
 description = "A hyper-parameter library for researchers, data scientists and machine learning engineers."
 requires-python = ">=3.7"
 readme = "README.md"
 license = { text = "Apache License Version 2.0" }
 
 [tool.maturin]
```

### Comparing `hyperparameter-0.5.2/src/entry.rs` & `hyperparameter-0.5.3/src/entry.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 use std::{ffi::c_void, sync::Arc};
+use phf::phf_map;
 
 #[derive(Debug, Clone, PartialEq)]
 pub struct DeferUnsafe(pub *mut c_void, pub unsafe fn(*mut c_void));
 
 impl Drop for DeferUnsafe {
     fn drop(&mut self) {
         unsafe { self.1(self.0) }
@@ -122,23 +123,56 @@
             Value::UserDefined(_, _, _) => {
                 Err("data type not matched, `UserDefined` and str".into())
             }
         }
     }
 }
 
+static STR2BOOL: phf::Map<&'static str, bool> = phf_map! {
+    "true" => true,
+    "True" => true,
+    "TRUE" => true,
+    "T" => true,
+    "yes" => true,
+    "y" => true,
+    "Yes" => true,
+    "YES" => true,
+    "Y" => true,
+    "on" => true,
+    "On" => true,
+    "ON" => true,
+
+    "false" => false,
+    "False" => false,
+    "FALSE" => false,
+    "F" => false,
+    "no" => false,
+    "n" => false,
+    "No" => false,
+    "NO" => false,
+    "N" => false,
+    "off" => false,
+    "Off" => false,
+    "OFF" => false,
+};
+
 impl TryFrom<Value> for bool {
     type Error = String;
 
     fn try_from(value: Value) -> Result<Self, Self::Error> {
         match value {
             Value::Empty => Err("empty value error".into()),
             Value::Int(v) => Ok(v != 0),
             Value::Float(_) => Err("data type not matched, `Float` and bool".into()),
-            Value::Text(_) => Err("data type not matched, `Text` and bool".into()),
+            Value::Text(s) => {
+                match STR2BOOL.get(&s) {
+                    Some(v) => Ok(v.clone()),
+                    None => Err("data type not matched, `Text` and bool".into()),
+                }
+            },
             Value::Boolen(v) => Ok(v),
             Value::UserDefined(_, _, _) => {
                 Err("data type not matched, `UserDefined` and str".into())
             }
         }
     }
 }
```

### Comparing `hyperparameter-0.5.2/src/ext.rs` & `hyperparameter-0.5.3/src/ext.rs`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.2/src/ffi.rs` & `hyperparameter-0.5.3/src/ffi.rs`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.2/src/storage.rs` & `hyperparameter-0.5.3/src/storage.rs`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.2/src/xxh.rs` & `hyperparameter-0.5.3/src/xxh.rs`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.2/tests/a.out` & `hyperparameter-0.5.3/tests/a.out`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.2/tests/test_auto_param.py` & `hyperparameter-0.5.3/tests/test_auto_param.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.2/tests/test_param_scope.py` & `hyperparameter-0.5.3/tests/test_param_scope.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.2/tests/test_param_scope_thread.py` & `hyperparameter-0.5.3/tests/test_param_scope_thread.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.2/tests/test_rust_backend.py` & `hyperparameter-0.5.3/tests/test_rust_backend.py`

 * *Files identical despite different names*

### Comparing `hyperparameter-0.5.2/PKG-INFO` & `hyperparameter-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperparameter
-Version: 0.5.2
+Version: 0.5.3
 License-File: LICENSE
 Summary: A hyper-parameter library for researchers, data scientists and machine learning engineers.
 Author-email: Reiase <reiase@gmail.com>
 License: Apache License Version 2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

