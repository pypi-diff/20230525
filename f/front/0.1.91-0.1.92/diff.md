# Comparing `tmp/front-0.1.91.tar.gz` & `tmp/front-0.1.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "front-0.1.91.tar", last modified: Mon May 22 22:02:18 2023, max compression
+gzip compressed data, was "front-0.1.92.tar", last modified: Thu May 25 21:40:58 2023, max compression
```

## Comparing `front-0.1.91.tar` & `front-0.1.92.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:02:18.483954 front-0.1.91/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-22 22:01:31.000000 front-0.1.91/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10360 2023-05-22 22:02:18.483954 front-0.1.91/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8392 2023-05-22 22:01:31.000000 front-0.1.91/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:02:18.479954 front-0.1.91/front/
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-22 22:01:31.000000 front-0.1.91/front/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-22 22:01:31.000000 front-0.1.91/front/app_maker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-22 22:01:31.000000 front-0.1.91/front/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    38784 2023-05-22 22:01:31.000000 front-0.1.91/front/crude.py
--rw-r--r--   0 runner    (1001) docker     (123)    17099 2023-05-22 22:01:31.000000 front-0.1.91/front/dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-22 22:01:31.000000 front-0.1.91/front/data_binding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:02:18.483954 front-0.1.91/front/elements/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-22 22:01:31.000000 front-0.1.91/front/elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13074 2023-05-22 22:02:17.000000 front-0.1.91/front/elements/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-22 22:01:31.000000 front-0.1.91/front/elements/implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-05-22 22:01:31.000000 front-0.1.91/front/elements/tree_maker_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:02:18.483954 front-0.1.91/front/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 22:01:31.000000 front-0.1.91/front/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-22 22:01:31.000000 front-0.1.91/front/examples/data_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-22 22:01:31.000000 front-0.1.91/front/examples/experimentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-22 22:01:31.000000 front-0.1.91/front/examples/issues.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-05-22 22:01:31.000000 front-0.1.91/front/examples/kaggle_front.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-22 22:01:31.000000 front-0.1.91/front/examples/pos_key_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-22 22:01:31.000000 front-0.1.91/front/examples/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-22 22:01:31.000000 front-0.1.91/front/examples/simple_ml_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-22 22:01:31.000000 front-0.1.91/front/examples/tw_data_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-05-22 22:01:31.000000 front-0.1.91/front/examples/wordle.py
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-05-22 22:01:31.000000 front-0.1.91/front/py2pydantic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:02:18.483954 front-0.1.91/front/scrap/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-22 22:01:31.000000 front-0.1.91/front/scrap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-05-22 22:01:31.000000 front-0.1.91/front/scrap/binder_proposal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-22 22:01:31.000000 front-0.1.91/front/scrap/binder_proposal_no_desc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-05-22 22:01:31.000000 front-0.1.91/front/scrap/state_proposal.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-22 22:01:31.000000 front-0.1.91/front/scrap/tw_simple_new_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-05-22 22:01:31.000000 front-0.1.91/front/spec_maker_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9254 2023-05-22 22:01:31.000000 front-0.1.91/front/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:02:18.483954 front-0.1.91/front/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 22:01:31.000000 front-0.1.91/front/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-22 22:01:31.000000 front-0.1.91/front/tests/app_identity_pydantic_output.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-22 22:01:31.000000 front-0.1.91/front/tests/app_identity_write_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-22 22:01:31.000000 front-0.1.91/front/tests/test_combos.py
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-05-22 22:01:31.000000 front-0.1.91/front/tests/test_crude.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-22 22:01:31.000000 front-0.1.91/front/tests/test_crudify_based_on_names.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-22 22:01:31.000000 front-0.1.91/front/tests/test_identity_write_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-22 22:01:31.000000 front-0.1.91/front/tests/test_py2pydantic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6318 2023-05-22 22:01:31.000000 front-0.1.91/front/tests/test_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-05-22 22:01:31.000000 front-0.1.91/front/tests/test_use_case.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-22 22:01:31.000000 front-0.1.91/front/tests/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-22 22:01:31.000000 front-0.1.91/front/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-22 22:01:31.000000 front-0.1.91/front/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    10957 2023-05-22 22:01:31.000000 front-0.1.91/front/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:02:18.479954 front-0.1.91/front.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10360 2023-05-22 22:02:18.000000 front-0.1.91/front.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-22 22:02:18.000000 front-0.1.91/front.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 22:02:18.000000 front-0.1.91/front.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 22:02:18.000000 front-0.1.91/front.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-22 22:02:18.000000 front-0.1.91/front.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-22 22:02:18.000000 front-0.1.91/front.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-22 22:02:18.483954 front-0.1.91/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-22 22:01:31.000000 front-0.1.91/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:40:57.993963 front-0.1.92/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-25 21:40:06.000000 front-0.1.92/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10360 2023-05-25 21:40:57.993963 front-0.1.92/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8392 2023-05-25 21:40:06.000000 front-0.1.92/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:40:57.989963 front-0.1.92/front/
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-25 21:40:06.000000 front-0.1.92/front/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-25 21:40:06.000000 front-0.1.92/front/app_maker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-25 21:40:06.000000 front-0.1.92/front/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38784 2023-05-25 21:40:06.000000 front-0.1.92/front/crude.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17099 2023-05-25 21:40:06.000000 front-0.1.92/front/dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-25 21:40:06.000000 front-0.1.92/front/data_binding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:40:57.989963 front-0.1.92/front/elements/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-25 21:40:06.000000 front-0.1.92/front/elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13008 2023-05-25 21:40:06.000000 front-0.1.92/front/elements/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-25 21:40:06.000000 front-0.1.92/front/elements/implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-05-25 21:40:06.000000 front-0.1.92/front/elements/tree_maker_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:40:57.993963 front-0.1.92/front/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 21:40:06.000000 front-0.1.92/front/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-25 21:40:06.000000 front-0.1.92/front/examples/data_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-25 21:40:06.000000 front-0.1.92/front/examples/experimentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-25 21:40:06.000000 front-0.1.92/front/examples/issues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-05-25 21:40:06.000000 front-0.1.92/front/examples/kaggle_front.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-25 21:40:06.000000 front-0.1.92/front/examples/pos_key_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-25 21:40:06.000000 front-0.1.92/front/examples/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-25 21:40:06.000000 front-0.1.92/front/examples/simple_ml_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-25 21:40:06.000000 front-0.1.92/front/examples/tw_data_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-05-25 21:40:06.000000 front-0.1.92/front/examples/wordle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-05-25 21:40:06.000000 front-0.1.92/front/py2pydantic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:40:57.993963 front-0.1.92/front/scrap/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-25 21:40:06.000000 front-0.1.92/front/scrap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-05-25 21:40:06.000000 front-0.1.92/front/scrap/binder_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-25 21:40:06.000000 front-0.1.92/front/scrap/binder_proposal_no_desc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-05-25 21:40:06.000000 front-0.1.92/front/scrap/state_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-25 21:40:06.000000 front-0.1.92/front/scrap/tw_simple_new_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-05-25 21:40:06.000000 front-0.1.92/front/spec_maker_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9254 2023-05-25 21:40:06.000000 front-0.1.92/front/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:40:57.993963 front-0.1.92/front/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 21:40:06.000000 front-0.1.92/front/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-25 21:40:06.000000 front-0.1.92/front/tests/app_identity_pydantic_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-25 21:40:06.000000 front-0.1.92/front/tests/app_identity_write_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-25 21:40:06.000000 front-0.1.92/front/tests/test_combos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-05-25 21:40:06.000000 front-0.1.92/front/tests/test_crude.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-25 21:40:06.000000 front-0.1.92/front/tests/test_crudify_based_on_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-25 21:40:06.000000 front-0.1.92/front/tests/test_identity_write_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-25 21:40:06.000000 front-0.1.92/front/tests/test_py2pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6318 2023-05-25 21:40:06.000000 front-0.1.92/front/tests/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-05-25 21:40:06.000000 front-0.1.92/front/tests/test_use_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-25 21:40:06.000000 front-0.1.92/front/tests/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-25 21:40:06.000000 front-0.1.92/front/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-25 21:40:06.000000 front-0.1.92/front/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10957 2023-05-25 21:40:06.000000 front-0.1.92/front/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:40:57.989963 front-0.1.92/front.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10360 2023-05-25 21:40:57.000000 front-0.1.92/front.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-25 21:40:57.000000 front-0.1.92/front.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 21:40:57.000000 front-0.1.92/front.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 21:40:57.000000 front-0.1.92/front.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-25 21:40:57.000000 front-0.1.92/front.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-25 21:40:57.000000 front-0.1.92/front.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-25 21:40:57.993963 front-0.1.92/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-25 21:40:06.000000 front-0.1.92/setup.py
```

### Comparing `front-0.1.91/LICENSE` & `front-0.1.92/LICENSE`

 * *Files identical despite different names*

### Comparing `front-0.1.91/PKG-INFO` & `front-0.1.92/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: front
-Version: 0.1.91
+Version: 0.1.92
 Summary: Getting from python objects to UIs exposing them
 Home-page: https://github.com/i2mint/front
 Author: OtoSense
 License: apache-2.0
 Description: # front
         
         [Documentation here](https://i2mint.github.io/front/)
```

### Comparing `front-0.1.91/README.md` & `front-0.1.92/README.md`

 * *Files identical despite different names*

### Comparing `front-0.1.91/front/__init__.py` & `front-0.1.92/front/__init__.py`

 * *Files identical despite different names*

### Comparing `front-0.1.91/front/app_maker.py` & `front-0.1.92/front/app_maker.py`

 * *Files identical despite different names*

### Comparing `front-0.1.91/front/base.py` & `front-0.1.92/front/base.py`

 * *Files identical despite different names*

### Comparing `front-0.1.91/front/crude.py` & `front-0.1.92/front/crude.py`

 * *Files identical despite different names*

### Comparing `front-0.1.91/front/dag.py` & `front-0.1.92/front/dag.py`

 * *Files identical despite different names*

### Comparing `front-0.1.91/front/data_binding.py` & `front-0.1.92/front/data_binding.py`

 * *Files identical despite different names*

### Comparing `front-0.1.91/front/elements/elements.py` & `front-0.1.92/front/elements/elements.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,17 +63,14 @@
     except KeyError:
         raise RuntimeError(
             f'Key "{ELEMENT_KEY}" is missing in the following element specification: {spec}'
         )
     try:
         return factory(**_spec)
     except Exception as e:
-        from i2 import Sig
-
-        print('COUCOU', Sig(factory))
         print(f'An error occurred when trying to build element {factory}')
         raise e
 
 
 def mk_input_element_specs(obj, inputs):
     def mk_input_spec(p):
         input_spec = inputs_spec.get(p.name, {})
```

### Comparing `front-0.1.91/front/elements/implementation.py` & `front-0.1.92/front/elements/implementation.py`

 * *Files identical despite different names*

### Comparing `front-0.1.91/front/elements/tree_maker_base.py` & `front-0.1.92/front/elements/tree_maker_base.py`

 * *Files identical despite different names*

### Comparing `front-0.1.91/front/examples/experimentation.py` & `front-0.1.92/front/examples/experimentation.py`

 * *Files identical despite different names*

### Comparing `front-0.1.91/front/examples/issues.py` & `front-0.1.92/front/examples/issues.py`

 * *Files identical despite different names*

### Comparing `front-0.1.91/front/examples/kaggle_front.py` & `front-0.1.92/front/examples/kaggle_front.py`

 * *Files identical despite different names*

### Comparing `front-0.1.91/front/examples/pos_key_args.py` & `front-0.1.92/front/examples/pos_key_args.py`

 * *Files identical despite different names*

### Comparing `front-0.1.91/front/examples/simple.py` & `front-0.1.92/front/examples/simple.py`

 * *Files identical despite different names*

### Comparing `front-0.1.91/front/examples/simple_ml_1.py` & `front-0.1.92/front/examples/simple_ml_1.py`

 * *Files identical despite different names*

### Comparing `front-0.1.91/front/examples/tw_data_binding.py` & `front-0.1.92/front/examples/tw_data_binding.py`

 * *Files identical despite different names*

### Comparing `front-0.1.91/front/examples/wordle.py` & `front-0.1.92/front/examples/wordle.py`

 * *Files identical despite different names*

### Comparing `front-0.1.91/front/py2pydantic.py` & `front-0.1.92/front/py2pydantic.py`

 * *Files identical despite different names*

### Comparing `front-0.1.91/front/scrap/binder_proposal.py` & `front-0.1.92/front/scrap/binder_proposal.py`

 * *Files identical despite different names*

### Comparing `front-0.1.91/front/scrap/binder_proposal_no_desc.py` & `front-0.1.92/front/scrap/binder_proposal_no_desc.py`

 * *Files identical despite different names*

### Comparing `front-0.1.91/front/scrap/state_proposal.py` & `front-0.1.92/front/scrap/state_proposal.py`

 * *Files identical despite different names*

### Comparing `front-0.1.91/front/spec_maker_base.py` & `front-0.1.92/front/spec_maker_base.py`

 * *Files identical despite different names*

### Comparing `front-0.1.91/front/state.py` & `front-0.1.92/front/state.py`

 * *Files identical despite different names*

### Comparing `front-0.1.91/front/tests/test_combos.py` & `front-0.1.92/front/tests/test_combos.py`

 * *Files identical despite different names*

### Comparing `front-0.1.91/front/tests/test_crude.py` & `front-0.1.92/front/tests/test_crude.py`

 * *Files identical despite different names*

### Comparing `front-0.1.91/front/tests/test_crudify_based_on_names.py` & `front-0.1.92/front/tests/test_crudify_based_on_names.py`

 * *Files identical despite different names*

### Comparing `front-0.1.91/front/tests/test_py2pydantic.py` & `front-0.1.92/front/tests/test_py2pydantic.py`

 * *Files identical despite different names*

### Comparing `front-0.1.91/front/tests/test_state.py` & `front-0.1.92/front/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `front-0.1.91/front/tests/test_use_case.py` & `front-0.1.92/front/tests/test_use_case.py`

 * *Files identical despite different names*

### Comparing `front-0.1.91/front/tests/util.py` & `front-0.1.92/front/tests/util.py`

 * *Files identical despite different names*

### Comparing `front-0.1.91/front/tools.py` & `front-0.1.92/front/tools.py`

 * *Files identical despite different names*

### Comparing `front-0.1.91/front/util.py` & `front-0.1.92/front/util.py`

 * *Files identical despite different names*

### Comparing `front-0.1.91/front.egg-info/PKG-INFO` & `front-0.1.92/front.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: front
-Version: 0.1.91
+Version: 0.1.92
 Summary: Getting from python objects to UIs exposing them
 Home-page: https://github.com/i2mint/front
 Author: OtoSense
 License: apache-2.0
 Description: # front
         
         [Documentation here](https://i2mint.github.io/front/)
```

### Comparing `front-0.1.91/front.egg-info/SOURCES.txt` & `front-0.1.92/front.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `front-0.1.91/setup.cfg` & `front-0.1.92/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = front
-version = 0.1.91
+version = 0.1.92
 url = https://github.com/i2mint/front
 platforms = any
 description_file = README.md
 root_url = https://github.com/i2mint/
 license = apache-2.0
 author = OtoSense
 description = Getting from python objects to UIs exposing them
```

