# Comparing `tmp/pyglove-0.3.1.dev20230523.tar.gz` & `tmp/pyglove-0.3.1.dev20230524.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyglove-0.3.1.dev20230523.tar", last modified: Tue May 23 08:06:37 2023, max compression
+gzip compressed data, was "pyglove-0.3.1.dev20230524.tar", last modified: Wed May 24 08:06:29 2023, max compression
```

## Comparing `pyglove-0.3.1.dev20230523.tar` & `pyglove-0.3.1.dev20230524.tar`

### file list

```diff
@@ -1,194 +1,194 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:06:37.194134 pyglove-0.3.1.dev20230523/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-05-23 08:06:37.194134 pyglove-0.3.1.dev20230523/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-05-23 08:06:35.000000 pyglove-0.3.1.dev20230523/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:06:37.170134 pyglove-0.3.1.dev20230523/pyglove/
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:06:37.170134 pyglove-0.3.1.dev20230523/pyglove/core/
--rw-r--r--   0 runner    (1001) docker     (123)     8275 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:06:37.170134 pyglove-0.3.1.dev20230523/pyglove/core/detouring/
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/detouring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/detouring/class_detour.py
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/detouring/class_detour_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:06:37.174134 pyglove-0.3.1.dev20230523/pyglove/core/geno/
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/geno/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64370 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/geno/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    38561 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/geno/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/geno/categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)    18444 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/geno/categorical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/geno/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/geno/custom_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/geno/deduping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/geno/deduping_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8959 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/geno/dna_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/geno/dna_generator_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/geno/numerical.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/geno/numerical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/geno/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/geno/random_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/geno/space.py
--rw-r--r--   0 runner    (1001) docker     (123)    16554 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/geno/space_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/geno/sweeping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/geno/sweeping_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:06:37.174134 pyglove-0.3.1.dev20230523/pyglove/core/hyper/
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/hyper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7106 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/hyper/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    23216 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/hyper/categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)    13533 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/hyper/categorical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/hyper/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/hyper/custom_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/hyper/derived.py
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/hyper/derived_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22812 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/hyper/dynamic_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)    17149 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/hyper/dynamic_evaluation_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10161 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/hyper/evolvable.py
--rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/hyper/evolvable_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/hyper/iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/hyper/iter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/hyper/numerical.py
--rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/hyper/numerical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22325 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/hyper/object_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/hyper/object_template_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/logging_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:06:37.178134 pyglove-0.3.1.dev20230523/pyglove/core/object_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/object_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/object_utils/codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/object_utils/codegen_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/object_utils/common_traits.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/object_utils/common_traits_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/object_utils/docstr_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/object_utils/docstr_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/object_utils/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/object_utils/formatting_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    19754 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/object_utils/hierarchical.py
--rw-r--r--   0 runner    (1001) docker     (123)    21150 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/object_utils/hierarchical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/object_utils/missing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/object_utils/missing_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/object_utils/thread_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/object_utils/thread_local_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    18016 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/object_utils/value_location.py
--rw-r--r--   0 runner    (1001) docker     (123)    13083 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/object_utils/value_location_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:06:37.178134 pyglove-0.3.1.dev20230523/pyglove/core/patching/
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/patching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/patching/object_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/patching/object_factory_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/patching/pattern_based.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/patching/pattern_based_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16675 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/patching/rule_based.py
--rw-r--r--   0 runner    (1001) docker     (123)    17894 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/patching/rule_based_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:06:37.182134 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/
--rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    75319 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/boilerplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/boilerplate_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22447 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/class_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    21508 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/class_wrapper_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10059 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/compounding.py
--rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/compounding_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/contextual.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/contextual_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    33066 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)    58215 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/dict_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     9762 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/diff_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11911 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/flags.py
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/flags_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    23879 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/functor.py
--rw-r--r--   0 runner    (1001) docker     (123)    28989 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/functor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    27446 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/list.py
--rw-r--r--   0 runner    (1001) docker     (123)    52472 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/list_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    34428 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/object.py
--rw-r--r--   0 runner    (1001) docker     (123)    81342 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/object_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/origin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/origin_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/pure_symbolic.py
--rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/schema_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/symbolize.py
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/symbolic/symbolize_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:06:37.186134 pyglove-0.3.1.dev20230523/pyglove/core/tuning/
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/tuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/tuning/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/tuning/backend_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/tuning/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)    13832 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/tuning/local_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    17756 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/tuning/protocols.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/tuning/protocols_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12975 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/tuning/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    17552 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/tuning/sample_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:06:37.186134 pyglove-0.3.1.dev20230523/pyglove/core/typing/
--rw-r--r--   0 runner    (1001) docker     (123)    12965 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/typing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6032 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/typing/annotation_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/typing/annotation_conversion_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/typing/callable_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/typing/callable_ext_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12647 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/typing/callable_signature.py
--rw-r--r--   0 runner    (1001) docker     (123)    11000 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/typing/callable_signature_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    49538 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/typing/class_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    25636 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/typing/class_schema_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/typing/class_schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/typing/class_schema_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/typing/custom_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/typing/key_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/typing/key_specs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/typing/pytype_support.py
--rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/typing/type_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/typing/type_conversion_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/typing/typed_missing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/typing/typed_missing_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    79366 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/typing/value_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)   103891 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/core/typing/value_specs_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:06:37.186134 pyglove-0.3.1.dev20230523/pyglove/ext/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:06:37.190134 pyglove-0.3.1.dev20230523/pyglove/ext/early_stopping/
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/early_stopping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/early_stopping/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/early_stopping/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/early_stopping/step_wise.py
--rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/early_stopping/step_wise_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:06:37.190134 pyglove-0.3.1.dev20230523/pyglove/ext/evolution/
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/evolution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50090 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/evolution/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    29936 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/evolution/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/evolution/hill_climb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/evolution/hill_climb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9757 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/evolution/mutators.py
--rw-r--r--   0 runner    (1001) docker     (123)    17424 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/evolution/mutators_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8162 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/evolution/neat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/evolution/neat_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/evolution/nsga2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/evolution/nsga2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    40354 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/evolution/recombinators.py
--rw-r--r--   0 runner    (1001) docker     (123)    19290 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/evolution/recombinators_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/evolution/regularized_evolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/evolution/regularized_evolution_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/evolution/selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/evolution/selectors_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/evolution/where.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/evolution/where_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:06:37.190134 pyglove-0.3.1.dev20230523/pyglove/ext/mutfun/
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/mutfun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16703 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/mutfun/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    21312 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/mutfun/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/mutfun/basic_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    11244 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/mutfun/basic_ops_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:06:37.194134 pyglove-0.3.1.dev20230523/pyglove/ext/scalars/
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/scalars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/scalars/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/scalars/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/scalars/maths.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/scalars/maths_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/scalars/randoms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/scalars/randoms_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/scalars/step_wise.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/pyglove/ext/scalars/step_wise_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:06:37.170134 pyglove-0.3.1.dev20230523/pyglove.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-05-23 08:06:37.000000 pyglove-0.3.1.dev20230523/pyglove.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-05-23 08:06:37.000000 pyglove-0.3.1.dev20230523/pyglove.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 08:06:37.000000 pyglove-0.3.1.dev20230523/pyglove.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-23 08:06:37.000000 pyglove-0.3.1.dev20230523/pyglove.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-23 08:06:37.000000 pyglove-0.3.1.dev20230523/pyglove.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 08:06:37.194134 pyglove-0.3.1.dev20230523/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-05-23 08:06:21.000000 pyglove-0.3.1.dev20230523/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:06:29.947311 pyglove-0.3.1.dev20230524/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-05-24 08:06:29.947311 pyglove-0.3.1.dev20230524/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-05-24 08:06:27.000000 pyglove-0.3.1.dev20230524/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:06:29.927311 pyglove-0.3.1.dev20230524/pyglove/
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:06:29.931311 pyglove-0.3.1.dev20230524/pyglove/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     8379 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:06:29.931311 pyglove-0.3.1.dev20230524/pyglove/core/detouring/
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/detouring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/detouring/class_detour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/detouring/class_detour_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:06:29.931311 pyglove-0.3.1.dev20230524/pyglove/core/geno/
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/geno/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64370 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/geno/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38561 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/geno/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/geno/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18444 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/geno/categorical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/geno/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/geno/custom_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/geno/deduping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/geno/deduping_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8959 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/geno/dna_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/geno/dna_generator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/geno/numerical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/geno/numerical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/geno/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/geno/random_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/geno/space.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16554 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/geno/space_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/geno/sweeping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/geno/sweeping_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:06:29.935311 pyglove-0.3.1.dev20230524/pyglove/core/hyper/
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/hyper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7106 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/hyper/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23216 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/hyper/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13533 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/hyper/categorical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/hyper/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/hyper/custom_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/hyper/derived.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/hyper/derived_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22812 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/hyper/dynamic_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17149 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/hyper/dynamic_evaluation_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10161 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/hyper/evolvable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/hyper/evolvable_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/hyper/iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/hyper/iter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/hyper/numerical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/hyper/numerical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22325 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/hyper/object_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/hyper/object_template_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/logging_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:06:29.935311 pyglove-0.3.1.dev20230524/pyglove/core/object_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/object_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/object_utils/codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/object_utils/codegen_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/object_utils/common_traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/object_utils/common_traits_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/object_utils/docstr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/object_utils/docstr_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/object_utils/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/object_utils/formatting_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19754 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/object_utils/hierarchical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21150 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/object_utils/hierarchical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/object_utils/missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/object_utils/missing_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/object_utils/thread_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/object_utils/thread_local_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18160 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/object_utils/value_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13083 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/object_utils/value_location_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:06:29.935311 pyglove-0.3.1.dev20230524/pyglove/core/patching/
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/patching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/patching/object_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/patching/object_factory_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/patching/pattern_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/patching/pattern_based_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16675 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/patching/rule_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17894 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/patching/rule_based_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:06:29.939311 pyglove-0.3.1.dev20230524/pyglove/core/symbolic/
+-rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/symbolic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77681 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/symbolic/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/symbolic/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/symbolic/boilerplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/symbolic/boilerplate_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22447 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/symbolic/class_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21508 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/symbolic/class_wrapper_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10059 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/symbolic/compounding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/symbolic/compounding_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/symbolic/contextual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/symbolic/contextual_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34050 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/symbolic/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62550 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/symbolic/dict_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/symbolic/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9762 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/symbolic/diff_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11911 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/symbolic/flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/symbolic/flags_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23955 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/symbolic/functor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29174 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/symbolic/functor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28899 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/symbolic/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55862 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/symbolic/list_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34771 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/symbolic/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82777 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/symbolic/object_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/symbolic/origin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/symbolic/origin_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/symbolic/pure_symbolic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/symbolic/schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/symbolic/schema_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/symbolic/symbolize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/symbolic/symbolize_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:06:29.939311 pyglove-0.3.1.dev20230524/pyglove/core/tuning/
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/tuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/tuning/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/tuning/backend_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/tuning/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13832 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/tuning/local_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17756 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/tuning/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/tuning/protocols_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12975 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/tuning/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17552 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/tuning/sample_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:06:29.943311 pyglove-0.3.1.dev20230524/pyglove/core/typing/
+-rw-r--r--   0 runner    (1001) docker     (123)    12965 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/typing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6032 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/typing/annotation_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/typing/annotation_conversion_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/typing/callable_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/typing/callable_ext_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12647 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/typing/callable_signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11000 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/typing/callable_signature_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49538 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/typing/class_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25636 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/typing/class_schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/typing/class_schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/typing/class_schema_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/typing/custom_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/typing/key_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/typing/key_specs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/typing/pytype_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/typing/type_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/typing/type_conversion_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/typing/typed_missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/typing/typed_missing_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79567 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/typing/value_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   103891 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/core/typing/value_specs_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:06:29.943311 pyglove-0.3.1.dev20230524/pyglove/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/ext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:06:29.943311 pyglove-0.3.1.dev20230524/pyglove/ext/early_stopping/
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/ext/early_stopping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/ext/early_stopping/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/ext/early_stopping/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/ext/early_stopping/step_wise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/ext/early_stopping/step_wise_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:06:29.947311 pyglove-0.3.1.dev20230524/pyglove/ext/evolution/
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/ext/evolution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50090 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/ext/evolution/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29936 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/ext/evolution/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/ext/evolution/hill_climb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/ext/evolution/hill_climb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9757 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/ext/evolution/mutators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17424 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/ext/evolution/mutators_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8162 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/ext/evolution/neat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/ext/evolution/neat_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/ext/evolution/nsga2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/ext/evolution/nsga2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40354 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/ext/evolution/recombinators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19290 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/ext/evolution/recombinators_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/ext/evolution/regularized_evolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/ext/evolution/regularized_evolution_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/ext/evolution/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/ext/evolution/selectors_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/ext/evolution/where.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/ext/evolution/where_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:06:29.947311 pyglove-0.3.1.dev20230524/pyglove/ext/mutfun/
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/ext/mutfun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16703 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/ext/mutfun/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21312 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/ext/mutfun/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/ext/mutfun/basic_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11244 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/ext/mutfun/basic_ops_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:06:29.947311 pyglove-0.3.1.dev20230524/pyglove/ext/scalars/
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/ext/scalars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/ext/scalars/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/ext/scalars/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/ext/scalars/maths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/ext/scalars/maths_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/ext/scalars/randoms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/ext/scalars/randoms_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/ext/scalars/step_wise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/pyglove/ext/scalars/step_wise_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 08:06:29.927311 pyglove-0.3.1.dev20230524/pyglove.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-05-24 08:06:29.000000 pyglove-0.3.1.dev20230524/pyglove.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-05-24 08:06:29.000000 pyglove-0.3.1.dev20230524/pyglove.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 08:06:29.000000 pyglove-0.3.1.dev20230524/pyglove.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-24 08:06:29.000000 pyglove-0.3.1.dev20230524/pyglove.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-24 08:06:29.000000 pyglove-0.3.1.dev20230524/pyglove.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 08:06:29.947311 pyglove-0.3.1.dev20230524/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-05-24 08:06:13.000000 pyglove-0.3.1.dev20230524/setup.py
```

### Comparing `pyglove-0.3.1.dev20230523/LICENSE` & `pyglove-0.3.1.dev20230524/LICENSE`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/PKG-INFO` & `pyglove-0.3.1.dev20230524/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyglove
-Version: 0.3.1.dev20230523
+Version: 0.3.1.dev20230524
 Summary: PyGlove: A library for manipulating Python objects.
 Home-page: https://github.com/google/pyglove
 Author: PyGlove Authors
 Author-email: pyglove-authors@google.com
 License: Apache License 2.0
 Keywords: ai machine learning automl mutable symbolic framework meta-programming
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyglove-0.3.1.dev20230523/README.md` & `pyglove-0.3.1.dev20230524/README.md`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/__init__.py` & `pyglove-0.3.1.dev20230524/pyglove/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/__init__.py` & `pyglove-0.3.1.dev20230524/pyglove/core/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,14 +165,16 @@
 # Contextual value marker.
 ContextualValue = symbolic.ContextualValue
 ContextualGetter = symbolic.ContextualGetter
 
 # Decorator for making contextual getters.
 contextual_getter = symbolic.contextual_getter
 
+# Context object for computing contextual attribute.
+GetAttributeContext = symbolic.GetAttributeContext
 
 #
 # Symbols from 'typing.py'
 #
 
 # NOTE(daiyip): we introduce 'typing' as an alias for 'schema' sub-module, since
 # it may be easier to comprehend when users use pytype.
```

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/detouring/__init__.py` & `pyglove-0.3.1.dev20230524/pyglove/core/detouring/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/detouring/class_detour.py` & `pyglove-0.3.1.dev20230524/pyglove/core/detouring/class_detour.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/detouring/class_detour_test.py` & `pyglove-0.3.1.dev20230524/pyglove/core/detouring/class_detour_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/geno/__init__.py` & `pyglove-0.3.1.dev20230524/pyglove/core/geno/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/geno/base.py` & `pyglove-0.3.1.dev20230524/pyglove/core/geno/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/geno/base_test.py` & `pyglove-0.3.1.dev20230524/pyglove/core/geno/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/geno/categorical.py` & `pyglove-0.3.1.dev20230524/pyglove/core/geno/categorical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/geno/categorical_test.py` & `pyglove-0.3.1.dev20230524/pyglove/core/geno/categorical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/geno/custom.py` & `pyglove-0.3.1.dev20230524/pyglove/core/geno/custom.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/geno/custom_test.py` & `pyglove-0.3.1.dev20230524/pyglove/core/geno/custom_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/geno/deduping.py` & `pyglove-0.3.1.dev20230524/pyglove/core/geno/deduping.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/geno/deduping_test.py` & `pyglove-0.3.1.dev20230524/pyglove/core/geno/deduping_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/geno/dna_generator.py` & `pyglove-0.3.1.dev20230524/pyglove/core/geno/dna_generator.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/geno/dna_generator_test.py` & `pyglove-0.3.1.dev20230524/pyglove/core/geno/dna_generator_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/geno/numerical.py` & `pyglove-0.3.1.dev20230524/pyglove/core/geno/numerical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/geno/numerical_test.py` & `pyglove-0.3.1.dev20230524/pyglove/core/geno/numerical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/geno/random.py` & `pyglove-0.3.1.dev20230524/pyglove/core/geno/random.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/geno/random_test.py` & `pyglove-0.3.1.dev20230524/pyglove/core/geno/random_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/geno/space.py` & `pyglove-0.3.1.dev20230524/pyglove/core/geno/space.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/geno/space_test.py` & `pyglove-0.3.1.dev20230524/pyglove/core/geno/space_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/geno/sweeping.py` & `pyglove-0.3.1.dev20230524/pyglove/core/geno/sweeping.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/geno/sweeping_test.py` & `pyglove-0.3.1.dev20230524/pyglove/core/geno/sweeping_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/hyper/__init__.py` & `pyglove-0.3.1.dev20230524/pyglove/core/hyper/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/hyper/base.py` & `pyglove-0.3.1.dev20230524/pyglove/core/hyper/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/hyper/categorical.py` & `pyglove-0.3.1.dev20230524/pyglove/core/hyper/categorical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/hyper/categorical_test.py` & `pyglove-0.3.1.dev20230524/pyglove/core/hyper/categorical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/hyper/custom.py` & `pyglove-0.3.1.dev20230524/pyglove/core/hyper/custom.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/hyper/custom_test.py` & `pyglove-0.3.1.dev20230524/pyglove/core/hyper/custom_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/hyper/derived.py` & `pyglove-0.3.1.dev20230524/pyglove/core/hyper/derived.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/hyper/derived_test.py` & `pyglove-0.3.1.dev20230524/pyglove/core/hyper/derived_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/hyper/dynamic_evaluation.py` & `pyglove-0.3.1.dev20230524/pyglove/core/hyper/dynamic_evaluation.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/hyper/dynamic_evaluation_test.py` & `pyglove-0.3.1.dev20230524/pyglove/core/hyper/dynamic_evaluation_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/hyper/evolvable.py` & `pyglove-0.3.1.dev20230524/pyglove/core/hyper/evolvable.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/hyper/evolvable_test.py` & `pyglove-0.3.1.dev20230524/pyglove/core/hyper/evolvable_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/hyper/iter.py` & `pyglove-0.3.1.dev20230524/pyglove/core/hyper/iter.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/hyper/iter_test.py` & `pyglove-0.3.1.dev20230524/pyglove/core/hyper/iter_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/hyper/numerical.py` & `pyglove-0.3.1.dev20230524/pyglove/core/hyper/numerical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/hyper/numerical_test.py` & `pyglove-0.3.1.dev20230524/pyglove/core/hyper/numerical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/hyper/object_template.py` & `pyglove-0.3.1.dev20230524/pyglove/core/hyper/object_template.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/hyper/object_template_test.py` & `pyglove-0.3.1.dev20230524/pyglove/core/hyper/object_template_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/logging.py` & `pyglove-0.3.1.dev20230524/pyglove/core/logging.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/logging_test.py` & `pyglove-0.3.1.dev20230524/pyglove/core/logging_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/object_utils/__init__.py` & `pyglove-0.3.1.dev20230524/pyglove/core/object_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/object_utils/codegen.py` & `pyglove-0.3.1.dev20230524/pyglove/core/object_utils/codegen.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/object_utils/codegen_test.py` & `pyglove-0.3.1.dev20230524/pyglove/core/object_utils/codegen_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/object_utils/common_traits.py` & `pyglove-0.3.1.dev20230524/pyglove/core/object_utils/common_traits.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/object_utils/common_traits_test.py` & `pyglove-0.3.1.dev20230524/pyglove/core/object_utils/common_traits_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/object_utils/docstr_utils.py` & `pyglove-0.3.1.dev20230524/pyglove/core/object_utils/docstr_utils.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/object_utils/docstr_utils_test.py` & `pyglove-0.3.1.dev20230524/pyglove/core/object_utils/docstr_utils_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/object_utils/formatting.py` & `pyglove-0.3.1.dev20230524/pyglove/core/object_utils/formatting.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/object_utils/formatting_test.py` & `pyglove-0.3.1.dev20230524/pyglove/core/object_utils/formatting_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/object_utils/hierarchical.py` & `pyglove-0.3.1.dev20230524/pyglove/core/object_utils/hierarchical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/object_utils/hierarchical_test.py` & `pyglove-0.3.1.dev20230524/pyglove/core/object_utils/hierarchical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/object_utils/missing.py` & `pyglove-0.3.1.dev20230524/pyglove/core/object_utils/missing.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/object_utils/missing_test.py` & `pyglove-0.3.1.dev20230524/pyglove/core/object_utils/missing_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/object_utils/thread_local.py` & `pyglove-0.3.1.dev20230524/pyglove/core/object_utils/thread_local.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/object_utils/thread_local_test.py` & `pyglove-0.3.1.dev20230524/pyglove/core/object_utils/thread_local_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/object_utils/value_location.py` & `pyglove-0.3.1.dev20230524/pyglove/core/object_utils/value_location.py`

 * *Files 1% similar despite different names*

```diff
@@ -337,14 +337,16 @@
 
     Raises:
       KeyError: Path doesn't exist in src.
     """
     if key_pos == len(self._keys):
       return src
     key = self.keys[key_pos]
+    # NOTE(daiyip): For contextual value (e.g. ``pg.ContextualValue``),
+    # `query` returns its symbolic form instead of its evaluated value.
     if hasattr(src, 'sym_getattr'):
       assert hasattr(src, 'sym_hasattr')
       if src.sym_hasattr(key):
         return self._query(key_pos + 1, src.sym_getattr(key))
     elif hasattr(src, '__getitem__'):
       if isinstance(key, int):
         if not hasattr(src, '__len__'):
```

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/object_utils/value_location_test.py` & `pyglove-0.3.1.dev20230524/pyglove/core/object_utils/value_location_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/patching/__init__.py` & `pyglove-0.3.1.dev20230524/pyglove/core/patching/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/patching/object_factory.py` & `pyglove-0.3.1.dev20230524/pyglove/core/patching/object_factory.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/patching/object_factory_test.py` & `pyglove-0.3.1.dev20230524/pyglove/core/patching/object_factory_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/patching/pattern_based.py` & `pyglove-0.3.1.dev20230524/pyglove/core/patching/pattern_based.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/patching/pattern_based_test.py` & `pyglove-0.3.1.dev20230524/pyglove/core/patching/pattern_based_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/patching/rule_based.py` & `pyglove-0.3.1.dev20230524/pyglove/core/patching/rule_based.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/patching/rule_based_test.py` & `pyglove-0.3.1.dev20230524/pyglove/core/patching/rule_based_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/symbolic/__init__.py` & `pyglove-0.3.1.dev20230524/pyglove/core/symbolic/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,14 +61,17 @@
 from pyglove.core.symbolic.flags import should_call_functors_during_init
 
 # Marker for contextual values.
 from pyglove.core.symbolic.base import ContextualValue
 from pyglove.core.symbolic.contextual import ContextualGetter
 from pyglove.core.symbolic.contextual import contextual_getter
 
+# GetAttribute context for computing contextual values.
+from pyglove.core.symbolic.base import GetAttributeContext
+
 # Symbolic types and their definition helpers.
 from pyglove.core.symbolic.base import Symbolic
 from pyglove.core.symbolic.list import List
 from pyglove.core.symbolic.dict import Dict
 
 from pyglove.core.symbolic.object import ObjectMeta
 from pyglove.core.symbolic.object import Object
```

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/symbolic/base.py` & `pyglove-0.3.1.dev20230524/pyglove/core/symbolic/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Symbolic type base."""
 
 import abc
 import copy
+import dataclasses
 import enum
 import inspect
 import json
 import re
 import sys
 import typing
 from typing import Any, Callable, Dict, Iterator, List, Optional, Tuple, Type, Union
@@ -109,14 +110,32 @@
   # Returning only the immediate matched descendants.
   IMMEDIATE = 1
 
   # Returning only the leaf matched descendants.
   LEAF = 2
 
 
+@dataclasses.dataclass
+class GetAttributeContext:
+  """The context for computing a contextual value.
+
+  Attributes:
+    key: The key of symbolic attribute to request value.
+    container: An optional symbolic object as the current container to retrieve
+      the contextual value. If None, it means that there is no further container
+      to search for. Otherwise, it is a parent in the symbolic containing chain
+      for current attempt.
+    owner: The owner of the contextual attribute.
+  """
+
+  key: Union[str, int]
+  container: Optional['Symbolic']
+  owner: 'Symbolic'
+
+
 class ContextualValue(
     pg_typing.CustomTyping,
     object_utils.JSONConvertible,
     object_utils.Formattable,
 ):
   """Base class for contextual value markers.
 
@@ -147,34 +166,41 @@
     d = pg.Dict(y=2, z=pg.Dict(a=a))
 
     # `a.y` now refers to `d.a` since `d` is in its symbolic parent chain,
     # aka. context.
     assert a.y == 2
   """
 
-  def get(self, name: str, context: 'Symbolic') -> Any:
+  def get(self, context: GetAttributeContext) -> Any:
     """Try get the contextual value for a symbolic attribute from a parent.
 
     Args:
-      name: The name of the request symbolic attribute.
-      context: A symbolic parent which represents the current context.
+      context: a `GetAttributeContext` object representing curent context.
 
     Returns:
       The value for the requested symbolic attribute from the current context.
         If ``pg.MISSING_VALUE``, it means that current symbolic parent cannot
           provide a contextual value for the attribute, so the current context
           is moved upward, until it reaches to the root of the symbolic tree.
         If a ``pg.ContextualValue`` object, it will use the new contextual
           marker returned to resolve its value from its symbolic parent chains.
     """
-    return self.value_from(name, context)
+    return self.value_from(context)
 
-  def value_from(self, name: str, context: 'Symbolic') -> Any:
+  def value_from(self, context: GetAttributeContext) -> Any:
     """Try get the contextual value for a symbolic attribute from a parent."""
-    return getattr(context, name, pg_typing.MISSING_VALUE)
+    if context.container is None:
+      return pg_typing.MISSING_VALUE
+
+    if isinstance(context.key, int):
+      if isinstance(context.container, list):
+        return context.container[context.key]
+      else:
+        return pg_typing.MISSING_VALUE
+    return getattr(context.container, context.key, pg_typing.MISSING_VALUE)
 
   def custom_apply(self, *args, **kwargs: Any) -> Tuple[bool, Any]:
     # This is to make a ``ContextualValue`` object assignable
     # to any symbolic attribute.
     return (False, self)
 
   def format(
@@ -195,14 +221,19 @@
     # have their own __eq__ logic.
     return type(other) is ContextualValue  # pylint: disable=unidiomatic-typecheck
 
   def __ne__(self, other: Any) -> bool:
     return not self.__eq__(other)
 
 
+# Value marker for raising errors if a attribute does not exist or cannot
+# be computed.
+_RAISE_IF_NOT_FOUND = (pg_typing.MISSING_VALUE,)
+
+
 class Symbolic(object_utils.JSONConvertible,
                object_utils.MaybePartial,
                object_utils.Formattable):
   """Base for all symbolic types.
 
   Symbolic types are types that provide interfaces for symbolic programming,
   based on which symbolic objects can be created. In PyGlove, there are three
@@ -213,21 +244,22 @@
       inherit :class:`pyglove.ClassWrapper`, a subclass of ``pg.Object``.
     * Symbolic functions: Defined by :class:`pyglove.Functor`.
     * Symbolic container types: Defined by :class:`pyglove.List` and
       :class:`pyglove.Dict`.
   """
 
   # Symbolic sub-types that will be set when they are defined.
-  # DictType: Type['Symbolic'] = None      # pylint: disable=invalid-name
-  # ListType: Type['Symbolic'] = None      # pylint: disable=invalid-name
+  # pylint: disable=invalid-name
 
   DictType = None
   ListType = None
   ObjectType = None
 
+  # pylint: enable=invalid-name
+
   def __init__(self,
                *,
                allow_partial: bool,
                accessor_writable: bool,
                sealed: bool,
                root_path: Optional[object_utils.KeyPath],
                init_super: bool = True):
@@ -500,22 +532,22 @@
         will start with current node.
 
     Returns:
       True if the attribute exists. Otherwise False.
     """
     getter = getter or ContextualValue()
     v = self.sym_contextual_getattr(
-        key, default=(pg_typing.MISSING_VALUE,), getter=getter, start=start
+        key, default=pg_typing.MISSING_VALUE, getter=getter, start=start
     )
-    return v != (pg_typing.MISSING_VALUE,)
+    return v != pg_typing.MISSING_VALUE
 
   def sym_contextual_getattr(
       self,
       key: Union[str, int],
-      default: Any = object_utils.MISSING_VALUE,
+      default: Any = (object_utils.MISSING_VALUE,),
       getter: Optional[ContextualValue] = None,
       start: Union[
           'Symbolic', object_utils.MissingValue
       ] = pg_typing.MISSING_VALUE,
   ) -> Any:
     """Gets a key from current object's context (symbolic parent chain).
 
@@ -538,34 +570,58 @@
     """
     getter = getter or ContextualValue()
     if start == pg_typing.MISSING_VALUE:
       current = self
     else:
       current = typing.cast(Symbolic, start)
 
-    while current is not None:
-      v = getter.get(key, current)
+    while True:
+      context = GetAttributeContext(key=key, container=current, owner=self)
+      v = getter.get(context)
       # NOTE(daiyip): when the ContextualValue value from the parent returns
       # another ContextualValue object, we should follow the new return value's
       # instruction instead of the original one.
       if isinstance(v, ContextualValue):
         getter = v
       elif v != object_utils.MISSING_VALUE:
         return v
-      current = current.sym_parent
 
-    if default != object_utils.MISSING_VALUE:
+      if current is not None:
+        current = current.sym_parent
+      else:
+        break
+
+    if default != (object_utils.MISSING_VALUE,):
       return default
     raise AttributeError(
         self._error_message(
             f'`{key}` is not found under its context '
             '(along its symbolic parent chain).'
         )
     )
 
+  def sym_value(
+      self, key: Union[str, int], default: Any = _RAISE_IF_NOT_FOUND
+  ) -> Any:
+    """Gets the value of a symbolic attribute (with resolving ContextualValue).
+
+    Args:
+      key: The key of the symbolic attribute.
+      default: The default value if the key does not exist or contextual value
+        cannot be resolved. If not specified, attribute error will be risen.
+
+    Returns:
+      The value of the symbolic attribute after resolving the
+        ``pg.ContextualValue``.
+    """
+    v = self._sym_value(key, default)
+    if v is _RAISE_IF_NOT_FOUND:
+      raise AttributeError(key)
+    return v
+
   @abc.abstractmethod
   def sym_keys(self) -> Iterator[Union[str, int]]:
     """Iterates the keys of symbolic attributes."""
 
   @abc.abstractmethod
   def sym_values(self) -> Iterator[Any]:
     """Iterates the values of symbolic attributes."""
@@ -615,14 +671,19 @@
       skip_notification: Optional[bool] = None,
       **kwargs) -> 'Symbolic':
     """Mutates the sub-nodes of current object. Please see `rebind`."""
     if callable(path_value_pairs):
       path_value_pairs = get_rebind_dict(path_value_pairs, self)
     elif path_value_pairs is None:
       path_value_pairs = {}
+    elif isinstance(path_value_pairs, Symbolic.DictType):
+      # Rebind work on symbolic form, thus we get their symbol instead of
+      # their evaluated value when building the rebind dict.
+      sd = typing.cast(Symbolic.DictType, path_value_pairs)
+      path_value_pairs = {k: v for k, v in sd.sym_items()}
     if not isinstance(path_value_pairs, dict):
       raise ValueError(
           self._error_message(
               f'Argument \'path_value_pairs\' should be a dict. '
               f'Encountered {path_value_pairs}'))
     path_value_pairs.update(kwargs)
     path_value_pairs = {object_utils.KeyPath.from_value(k): v
@@ -1115,14 +1176,28 @@
     return self.sym_clone(deep=True, memo=memo)
 
   #
   # Proteted methods to implement from subclasses
   #
 
   @abc.abstractmethod
+  def _sym_value(self, key: Union[str, int], default: Any) -> Any:
+    """Gets the value of a symbolic attribute (with resolving ContextualValue).
+
+    Args:
+      key: The key of the symbolic attribute.
+      default: The default value if the key does not exist or contextual value
+        cannot be resolved.
+
+    Returns:
+      The value of the symbolic attribute after resolving the
+        ``pg.ContextualValue``.
+    """
+
+  @abc.abstractmethod
   def _sym_rebind(
       self, path_value_pairs: Dict[object_utils.KeyPath, Any]
       ) -> List[FieldUpdate]:
     """Subclass specific rebind implementation.
 
     Args:
       path_value_pairs: A dictionary of key path to new field value.
```

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/symbolic/base_test.py` & `pyglove-0.3.1.dev20230524/pyglove/core/symbolic/base_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -101,15 +101,26 @@
 
   def test_call(self):
     @dataclasses.dataclass
     class A:
       x: int = 1
       y: int = 2
 
-    self.assertEqual(base.ContextualValue().get('x', A()), 1)
+    self.assertEqual(
+        base.ContextualValue().get(base.GetAttributeContext('x', A(), Dict())),
+        1,
+    )
+    self.assertEqual(
+        base.ContextualValue().get(base.GetAttributeContext(0, [0, 1], Dict())),
+        0,
+    )
+    self.assertEqual(
+        base.ContextualValue().get(base.GetAttributeContext(0, Dict(), Dict())),
+        pg_typing.MISSING_VALUE,
+    )
 
   def test_custom_typing(self):
     v = base.ContextualValue()
     self.assertIs(pg_typing.Int().apply(v), v)
     self.assertIs(pg_typing.Str().apply(v), v)
 
   def test_to_json(self):
```

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/symbolic/boilerplate.py` & `pyglove-0.3.1.dev20230524/pyglove/core/symbolic/boilerplate.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/symbolic/boilerplate_test.py` & `pyglove-0.3.1.dev20230524/pyglove/core/symbolic/boilerplate_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/symbolic/class_wrapper.py` & `pyglove-0.3.1.dev20230524/pyglove/core/symbolic/class_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/symbolic/class_wrapper_test.py` & `pyglove-0.3.1.dev20230524/pyglove/core/symbolic/class_wrapper_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/symbolic/compounding.py` & `pyglove-0.3.1.dev20230524/pyglove/core/symbolic/compounding.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/symbolic/compounding_test.py` & `pyglove-0.3.1.dev20230524/pyglove/core/symbolic/compounding_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/symbolic/contextual_test.py` & `pyglove-0.3.1.dev20230524/pyglove/core/symbolic/contextual_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,19 +21,21 @@
 
 
 class ContextualGetterTest(unittest.TestCase):
   """Tests for `pg.symbolic.ContextualGetter`."""
 
   def test_basics(self):
     @contextual.contextual_getter
-    def static_value(k, p, v):
-      del k, p
+    def static_value(context, v):
+      del context
       return v
 
     getter = static_value(v=1)  # pylint: disable=no-value-for-parameter
     self.assertIsInstance(getter, base.ContextualValue)
-    self.assertEqual(getter.get('x', Dict()), 1)
+    self.assertEqual(
+        getter.get(base.GetAttributeContext('x', Dict(), Dict())), 1
+    )
     self.assertEqual(base.from_json(base.to_json(getter)), getter)
 
 
 if __name__ == '__main__':
   unittest.main()
```

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/symbolic/dict.py` & `pyglove-0.3.1.dev20230524/pyglove/core/symbolic/dict.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,21 @@
 
 from pyglove.core import object_utils
 from pyglove.core import typing as pg_typing
 from pyglove.core.symbolic import base
 from pyglove.core.symbolic import flags
 
 
+# Special default value to detect missing keys in a Dict. Though its values is
+# the same as `base._RAISE_IF_NOT_FOUND`, they are different instances so
+# `pg.Dict` and `pg.Symbolic` could use their own instances to control error
+# raising separately.
+_RAISE_IF_NOT_FOUND = (pg_typing.MISSING_VALUE,)
+
+
 class Dict(dict, base.Symbolic, pg_typing.CustomTyping):
   """Symbolic dict.
 
   ``pg.Dict`` implements a dict type whose instances are symbolically
   programmable, which is a subclass of the built-in Python ``dict`` and
   a subclass of :class:`pyglove.Symbolic`.
 
@@ -198,15 +205,19 @@
     # This is useful when Dict is used as the field container of
     # pg.Object.
     self._set_raw_attr(
         '_as_object_attributes_container',
         kwargs.pop('as_object_attributes_container', False),
     )
 
-    if dict_obj is not None:
+    # We copy the symbolic form of dict values instead of their evaluated
+    # values.
+    if isinstance(dict_obj, Dict):
+      dict_obj = {k: v for k, v in dict_obj.sym_items()}
+    elif dict_obj is not None:
       dict_obj = dict(dict_obj)
 
     # NOTE(daiyip): we call __init__ of superclasses explicitly instead of
     # calling super().__init__(...) since dict.__init__ does
     # not follow super(...).__init__ fashion, which will lead to
     # Symbolic.__init__ uncalled.
     base.Symbolic.__init__(
@@ -337,24 +348,24 @@
     if self._value_spec and self._value_spec.schema:
       matched_keys, _ = self._value_spec.schema.resolve(self.keys())
       for key_spec, keys in matched_keys.items():
         field = self._value_spec.schema[key_spec]
         assert keys or isinstance(key_spec, pg_typing.NonConstKey), key_spec
         if keys:
           for key in keys:
-            v = self[key]
+            v = self.sym_getattr(key)
             if object_utils.MISSING_VALUE == v:
               missing[key] = field.value.default
             else:
               if isinstance(v, base.Symbolic):
                 missing_child = v.sym_missing(flatten=False)
                 if missing_child:
                   missing[key] = missing_child
     else:
-      for k, v in self.items():
+      for k, v in self.sym_items():
         if isinstance(v, base.Symbolic):
           missing_child = v.sym_missing(flatten=False)
           if missing_child:
             missing[k] = missing_child
     return missing
 
   def _sym_nondefault(self) -> typing.Dict[str, Any]:
@@ -363,48 +374,48 @@
     if self._value_spec and self._value_spec.schema:
       dict_schema = self._value_spec.schema
       matched_keys, unmatched_keys = dict_schema.resolve(self.keys())
       assert not unmatched_keys
       for key_spec, keys in matched_keys.items():
         value_spec = dict_schema[key_spec].value
         for key in keys:
-          v = self[key]
+          v = self.sym_getattr(key)
           child_has_non_defaults = False
           if isinstance(v, base.Symbolic):
             non_defaults_child = v.non_default_values(flatten=False)
             if non_defaults_child:
               non_defaults[key] = non_defaults_child
               child_has_non_defaults = True
           if not child_has_non_defaults and value_spec.default != v:
             non_defaults[key] = v
     else:
-      for k, v in self.items():
+      for k, v in self.sym_items():
         if isinstance(v, base.Symbolic):
           non_defaults_child = v.non_default_values(flatten=False)
           if non_defaults_child:
             non_defaults[k] = non_defaults_child
         else:
           non_defaults[k] = v
     return non_defaults
 
   def set_accessor_writable(self, writable: bool = True) -> 'Dict':
     """Sets accessor writable."""
     if self.accessor_writable == writable:
       return self
-    for v in self.values():
+    for v in self.sym_values():
       if isinstance(v, base.Symbolic):
         v.set_accessor_writable(writable)
     super().set_accessor_writable(writable)
     return self
 
   def seal(self, sealed: bool = True) -> 'Dict':
     """Seals or unseals current object from further modification."""
     if self.is_sealed == sealed:
       return self
-    for v in self.values():
+    for v in self.sym_values():
       if isinstance(v, base.Symbolic):
         v.seal(sealed)
     super().seal(sealed)
     return self
 
   def sym_attr_field(
       self, key: Union[str, int]
@@ -448,15 +459,15 @@
 
   def sym_setparent(self, parent: base.Symbolic):
     """Override set parent of Dict to handle the passing through scenario."""
     super().sym_setparent(parent)
     # NOTE(daiyip): when flag `as_object_attributes_container` is on, it sets
     # the parent of child symbolic values using its parent.
     if self._as_object_attributes_container:
-      for v in self.values():
+      for v in self.sym_values():
         if isinstance(v, base.Symbolic):
           v.sym_setparent(parent)
 
   def sym_hash(self) -> int:
     """Symbolic hashing."""
     return base.sym_hash(
         (self.__class__,
@@ -467,15 +478,15 @@
       self, key: str) -> Any:
     """Gets symbolic attribute by key."""
     return super().__getitem__(key)
 
   def _sym_clone(self, deep: bool, memo=None) -> 'Dict':
     """Override Symbolic._sym_clone."""
     source = dict()
-    for k, v in self.items():
+    for k, v in self.sym_items():
       if deep or isinstance(v, base.Symbolic):
         v = base.clone(v, deep, memo)
       source[k] = v
     return Dict(
         source,
         value_spec=self._value_spec,
         allow_partial=self._allow_partial,
@@ -489,15 +500,15 @@
 
   def _update_children_paths(
       self,
       old_path: object_utils.KeyPath,
       new_path: object_utils.KeyPath) -> None:
     """Update children paths according to root_path of current node."""
     del old_path
-    for k, v in self.items():
+    for k, v in self.sym_items():
       if isinstance(v, base.Symbolic):
         v.sym_setpath(object_utils.KeyPath(k, new_path))
 
   def _set_item_without_permission_check(  # pytype: disable=signature-mismatch  # overriding-parameter-type-checks
       self, key: str, value: Any) -> Optional[base.FieldUpdate]:
     """Set item without permission check."""
     if not isinstance(key, str):
@@ -571,26 +582,37 @@
 
   def _on_change(self, field_updates: typing.Dict[object_utils.KeyPath,
                                                   base.FieldUpdate]):
     """On change event of Dict."""
     if self._onchange_callback:
       self._onchange_callback(field_updates)
 
-  def __getitem__(self, key: str) -> Any:
-    """Get item in this Dict."""
+  def _sym_value(self, key: str, default: Any) -> Any:  # pytype: disable=signature-mismatch
+    """Evalutes a symbolic attribute with resolving contextual values."""
+    if key not in self:
+      return default
     v = super().__getitem__(key)
     if isinstance(v, base.ContextualValue):
       start = self.sym_parent
       # NOTE(daiyip): The parent of `pg.Object`'s attribute dict points to
       # the `pg.Object` instance once it's set up. Here we let the ancester
       # traversal to bypass `pg.Object` to avoid double entry, which causes
       # dead loop.
       if self._as_object_attributes_container and self.sym_parent:
         start = start.sym_parent
-      v = self.sym_contextual_getattr(key, getter=v, start=start)
+      v = self.sym_contextual_getattr(
+          key, default=default, getter=v, start=start
+      )
+    return v
+
+  def __getitem__(self, key: str) -> Any:
+    """Get item in this Dict."""
+    v = self.sym_value(key, default=_RAISE_IF_NOT_FOUND)
+    if v is _RAISE_IF_NOT_FOUND:
+      raise KeyError(key)
     return v
 
   def __setitem__(self, key: str, value: Any) -> None:
     """Set item in this Dict.
 
     Args:
       key: String key. (Please be noted that key path is not supported.)
@@ -726,15 +748,15 @@
     if value_spec:
       self.use_value_spec(value_spec, self._allow_partial)
 
   def setdefault(self, key: str, default: Any = None) -> Any:
     """Sets default as the value to key if not present."""
     value = pg_typing.MISSING_VALUE
     if key in self:
-      value = self[key]
+      value = self.sym_getattr(key)
     if value == pg_typing.MISSING_VALUE:
       self[key] = default
       value = default
     return value
 
   def update(self,
              other: Union[
@@ -761,25 +783,28 @@
       for key_spec, keys in matched_keys.items():
         # NOTE(daiyip): The key values of frozen field can safely be excluded
         # since they will be the same for a class.
         field = self._value_spec.schema[key_spec]
         if not field.frozen:
           for key in keys:
             if key not in exclude_keys:
-              value = self[key]
+              value = self.sym_getattr(key)
               if pg_typing.MISSING_VALUE == value:
                 continue
               if hide_default_values and value == field.default_value:
                 continue
               json_repr[key] = base.to_json(
                   value, hide_default_values=hide_default_values, **kwargs)
       return json_repr
     else:
-      return {k: base.to_json(v, **kwargs)
-              for k, v in self.items() if k not in exclude_keys}
+      return {
+          k: base.to_json(v, **kwargs)
+          for k, v in self.sym_items()
+          if k not in exclude_keys
+      }
 
   def custom_apply(
       self,
       path: object_utils.KeyPath,
       value_spec: pg_typing.ValueSpec,
       allow_partial: bool,
       child_transform: Optional[
@@ -837,22 +862,23 @@
     if self._value_spec and self._value_spec.schema:
       matched_keys, unmatched = self._value_spec.schema.resolve(self.keys())
       assert not unmatched
       for key_spec, keys in matched_keys.items():
         for key in keys:
           if key not in exclude_keys:
             field = self._value_spec.schema[key_spec]
-            if pg_typing.MISSING_VALUE == self[key]:
+            v = self.sym_getattr(key)
+            if pg_typing.MISSING_VALUE == v:
               if hide_missing_values:
                 continue
-            elif hide_default_values and self[key] == field.default_value:
+            elif hide_default_values and v == field.default_value:
               continue
-            field_list.append((field, key, self[key]))
+            field_list.append((field, key, v))
     else:
-      for k, v in self.items():
+      for k, v in self.sym_items():
         if k not in exclude_keys:
           field_list.append((None, k, v))
 
     open_bracket, close_bracket = object_utils.bracket_chars(bracket_type)
     if not field_list:
       return f'{cls_name}{open_bracket}{close_bracket}'
```

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/symbolic/dict_test.py` & `pyglove-0.3.1.dev20230524/pyglove/core/symbolic/dict_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import inspect
 import io
 import unittest
 
 from pyglove.core import object_utils
 from pyglove.core import typing as pg_typing
 from pyglove.core.symbolic import base
+from pyglove.core.symbolic import contextual
 from pyglove.core.symbolic import flags
 from pyglove.core.symbolic import object as pg_object
 from pyglove.core.symbolic.dict import Dict
 from pyglove.core.symbolic.list import List
 from pyglove.core.symbolic.pure_symbolic import NonDeterministic
 from pyglove.core.symbolic.pure_symbolic import PureSymbolic
 
@@ -63,14 +64,18 @@
 
     # Schematized dict.
     vs = pg_typing.Dict([('a', pg_typing.Int())])
     sd = Dict(a=1, value_spec=vs)
     self.assertIs(sd.value_spec, vs)
     self.assertEqual(sd, dict(a=1))
 
+    # Dict with contextual value
+    sd = Dict(Dict(x=base.ContextualValue()))
+    self.assertEqual(sd, dict(x=base.ContextualValue()))
+
     with self.assertRaisesRegex(
         ValueError, 'Required value is not specified.'):
       Dict(value_spec=vs)
 
     # Schematized dict with default value.
     vs = pg_typing.Dict([('a', pg_typing.Int(default=0))])
     sd = Dict(value_spec=vs)
@@ -320,20 +325,32 @@
     self.assertEqual(sd, dict(a=1))
     sd['x1'] = 2
     sd['x2'] = 3
     self.assertEqual(sd, dict(a=1, x1=2, x2=3))
     with self.assertRaisesRegex(KeyError, 'Key \'y1\' is not allowed'):
       sd['y1'] = 4
 
+    # Set item with a contextual value.
+    sd = Dict(x=1)
+    sd.x = base.ContextualValue()
+    self.assertEqual(sd.sym_getattr('x'), base.ContextualValue())
+
   def test_getitem(self):
     sd = Dict(a=1)
     self.assertEqual(sd['a'], 1)
     with self.assertRaisesRegex(KeyError, 'x'):
       _ = sd['x']
 
+    sd = Dict(x=base.ContextualValue())
+    with self.assertRaisesRegex(AttributeError, 'x'):
+      _ = sd['x']
+
+    sdd = Dict(x=Dict(foo=0), y=sd)
+    self.assertIs(sd['x'], sdd['x'])
+
   def test_delitem(self):
     # Delete an item from a schemaless dict.
     sd = Dict(a=1, b=0)
     del sd['a']
     self.assertEqual(len(sd), 1)
 
     with flags.as_sealed():
@@ -401,14 +418,25 @@
 
   def test_getattr(self):
     sd = Dict(a=1)
     self.assertEqual(sd.a, 1)
     with self.assertRaisesRegex(AttributeError, 'Attribute .* does not exist'):
       _ = sd.x
 
+    # Test contextual.
+    sd = Dict(x=base.ContextualValue())
+    with self.assertRaisesRegex(
+        AttributeError, '`x` is not found under its context'
+    ):
+      _ = sd.x
+
+    p = Dict(x=Dict(p='foo'), y=Dict(z=sd))
+    self.assertEqual(sd.x, Dict(p='foo'))
+    self.assertIs(p.x, sd.x)
+
   def test_delattr(self):
     # Delete an item from a schemaless dict.
     sd = Dict(a=1, b=0)
     del sd.a
     self.assertEqual(len(sd), 1)
     with flags.as_sealed():
       with self.assertRaisesRegex(
@@ -587,14 +615,20 @@
     self.assertEqual(sd.setdefault('a'), 0)
     with self.assertRaisesRegex(KeyError, 'Key .* is not allowed'):
       sd.setdefault('y', 1)
 
     sd = Dict.partial(value_spec=pg_typing.Dict([('a', pg_typing.Int())]))
     self.assertEqual(sd.setdefault('a', 1), 1)
 
+    sd = Dict()
+    sd.setdefault('x', base.ContextualValue())
+    self.assertEqual(sd.sym_getattr('x'), base.ContextualValue())
+    sd.setdefault('x', 1)
+    self.assertEqual(sd.sym_getattr('x'), base.ContextualValue())
+
   def test_update(self):
     sd = Dict(b=0, a=1, c=2)
     with flags.as_sealed():
       with self.assertRaisesRegex(
           base.WritePermissionError, 'Cannot rebind key .* of sealed Dict'):
         sd.update(a=1)
     sd.update({'a': MISSING_VALUE, 'b': 1, 'd': 3})
@@ -782,14 +816,29 @@
     self.assertEqual(sd.sym_getattr('x'), 1)
     self.assertIsNone(sd.sym_getattr('a', None))
     with self.assertRaisesRegex(
         AttributeError,
         '.* object has no symbolic attribute \'a\'.'):
       sd.sym_getattr('a')
 
+    sd = Dict(x=base.ContextualValue())
+    self.assertEqual(sd.sym_getattr('x'), base.ContextualValue())
+
+  def test_sym_value(self):
+    @contextual.contextual_getter
+    def static_value(context, v):
+      del context
+      return v
+
+    sd = Dict(x=1, y=static_value(v=0))  # pylint: disable=no-value-for-parameter
+    self.assertEqual(sd.sym_value('x'), 1)
+    self.assertEqual(sd.sym_value('y'), 0)
+    with self.assertRaisesRegex(AttributeError, 'z'):
+      _ = sd.sym_value('z')
+
   def test_sym_field(self):
     sd = Dict(x=1, y=Dict(z=2))
     self.assertIsNone(sd.sym_field)
 
     spec = pg_typing.Dict([
         ('x', pg_typing.Int()),
         ('y', pg_typing.Dict())
@@ -816,41 +865,56 @@
 
     sd = Dict(x=1, z=3, y=2, value_spec=pg_typing.Dict([
         (pg_typing.StrKey(), pg_typing.Int())
     ]))
     self.assertEqual(next(sd.sym_keys()), 'x')
     self.assertEqual(list(sd.sym_keys()), ['x', 'z', 'y'])
 
+    sd = Dict(x=1, y=base.ContextualValue())
+    self.assertEqual(next(sd.sym_keys()), 'x')
+    self.assertEqual(list(sd.sym_keys()), ['x', 'y'])
+
   def test_sym_values(self):
     sd = Dict(x=1, y=2)
     self.assertEqual(next(sd.sym_values()), 1)
     self.assertEqual(list(sd.sym_values()), [1, 2])
 
     sd = Dict(x=1, z=3, y=2, value_spec=pg_typing.Dict([
         (pg_typing.StrKey(), pg_typing.Int())
     ]))
     self.assertEqual(next(sd.sym_values()), 1)
     self.assertEqual(list(sd.sym_values()), [1, 3, 2])
 
+    sd = Dict(x=1, y=base.ContextualValue())
+    self.assertEqual(next(sd.sym_values()), 1)
+    self.assertEqual(list(sd.sym_values()), [1, base.ContextualValue()])
+
   def test_sym_items(self):
     sd = Dict(x=1, y=2)
     self.assertEqual(next(sd.sym_items()), ('x', 1))
     self.assertEqual(list(sd.sym_items()), [('x', 1), ('y', 2)])
 
     sd = Dict(x=1, z=3, y=2, value_spec=pg_typing.Dict([
         (pg_typing.StrKey(), pg_typing.Int())
     ]))
     self.assertEqual(next(sd.sym_items()), ('x', 1))
     self.assertEqual(list(sd.sym_items()), [('x', 1), ('z', 3), ('y', 2)])
 
+    sd = Dict(x=1, y=base.ContextualValue())
+    self.assertEqual(next(sd.sym_items()), ('x', 1))
+    self.assertEqual(
+        list(sd.sym_items()), [('x', 1), ('y', base.ContextualValue())]
+    )
+
   def test_sym_jsonify(self):
     # Refer to SerializationTest for more detailed tests.
-    sd = Dict(x=1, y=2)
+    sd = Dict(x=1, y=base.ContextualValue())
     self.assertEqual(
-        sd.sym_jsonify(), {'x': 1, 'y': 2})
+        sd.sym_jsonify(), {'x': 1, 'y': base.ContextualValue().to_json()}
+    )
 
   def test_sym_rebind(self):
     # Refer to RebindTest for more detailed tests.
     sd = Dict(x=1, y=2)
     sd.sym_rebind(x=2)
     self.assertEqual(sd, dict(x=2, y=2))
 
@@ -907,26 +971,57 @@
     # Refer to `test_missing_values` for more details.
     sd = Dict.partial(x=1, value_spec=pg_typing.Dict([
         ('x', pg_typing.Int()),
         ('y', pg_typing.Int()),
     ]))
     self.assertEqual(sd.sym_missing(), {'y': MISSING_VALUE})
 
+    # Test contextual value as the default value.
+    sd = Dict(
+        x=base.ContextualValue(),
+        value_spec=pg_typing.Dict([
+            ('x', pg_typing.Int()),
+        ]),
+    )
+    self.assertEqual(sd.sym_missing(), {})
+
   def test_sym_nondefault(self):
     # Refer to `test_non_default_values` for more details.
     sd = Dict(x=1, value_spec=pg_typing.Dict([
         ('x', pg_typing.Int(default=0)),
         ('y', pg_typing.Dict([
             ('z', pg_typing.Int(default=1))
         ])),
     ]))
     self.assertEqual(sd.sym_nondefault(), {'x': 1})
     sd.rebind({'y.z': 2}, x=0)
     self.assertEqual(sd.sym_nondefault(), {'y.z': 2})
 
+    # Test contextual value as the default value.
+    sd = Dict(
+        x=1,
+        value_spec=pg_typing.Dict([
+            ('x', pg_typing.Int(default=base.ContextualValue())),
+        ]),
+    )
+    self.assertEqual(sd.sym_nondefault(), {'x': 1})
+    sd.rebind(x=base.ContextualValue())
+    self.assertEqual(sd.sym_nondefault(), {})
+
+    # Test contextual value as the specified value.
+    sd = Dict(
+        x=base.ContextualValue(),
+        value_spec=pg_typing.Dict([
+            ('x', pg_typing.Int(default=1)),
+        ]),
+    )
+    self.assertEqual(sd.sym_nondefault(), {'x': base.ContextualValue()})
+    sd.rebind(x=1)
+    self.assertEqual(sd.sym_nondefault(), {})
+
   def test_sym_puresymbolic(self):
     self.assertFalse(Dict(x=1).sym_puresymbolic)
 
     class A(PureSymbolic):
       pass
 
     self.assertTrue(Dict(x=A()).sym_puresymbolic)
@@ -1200,14 +1295,30 @@
 
       with self.assertRaisesRegex(
           base.WritePermissionError,
           'Cannot del Dict field by attribute or key while accessor_writable '
           'is set to False.'):
         del sd['a']
 
+    # Test with contextual value.
+    @contextual.contextual_getter
+    def unresolvable(k, p):
+      del k, p
+      return pg_typing.MISSING_VALUE
+
+    sd = Dict(x=unresolvable())  # pylint: disable=no-value-for-parameter
+    sd.set_accessor_writable(False)
+    self.assertFalse(sd.sym_getattr('x').accessor_writable)
+    with self.assertRaisesRegex(
+        base.WritePermissionError,
+        'Cannot modify Dict field by attribute or key while '
+        'accessor_writable is set to False.',
+    ):
+      sd.x = 1
+
   def test_mark_missing_values(self):
     # For schemaless Dict.
     sd = Dict(x=1, y=2)
     self.assertIn('x', sd)
     self.assertIn('y', sd)
 
     # Set field to MISSING_VALUE will delete field.
@@ -1347,24 +1458,25 @@
     sd = Dict(a=Dict())
     self.assertFalse(sd.is_sealed)
     self.assertFalse(sd.a.is_sealed)
     sd.seal()
     self.assertTrue(sd.is_sealed)
     self.assertTrue(sd.a.is_sealed)
 
-  def test_contextual(self):
-    sd = Dict(x=base.ContextualValue())
-    with self.assertRaisesRegex(
-        AttributeError, '`x` is not found under its context'
-    ):
-      _ = sd.x
+    # Test with contextual value.
+    @contextual.contextual_getter
+    def unresolvable(k, p):
+      del k, p
+      return pg_typing.MISSING_VALUE
 
-    p = Dict(x=Dict(p='foo'), y=Dict(z=sd))
-    self.assertEqual(sd.x, Dict(p='foo'))
-    self.assertIs(p.x, sd.x)
+    sd = Dict(x=unresolvable())  # pylint: disable=no-value-for-parameter
+    sd.seal()
+    self.assertTrue(sd.sym_getattr('x').is_sealed)
+    sd.seal(False)
+    self.assertFalse(sd.sym_getattr('x').is_sealed)
 
 
 class RebindTest(unittest.TestCase):
   """Dedicated tests for `pg.Dict.rebind`."""
 
   def test_rebind_on_schemaless_dicts(self):
     sd = Dict(a=Dict(b=1, c=2), d=3)
@@ -1396,14 +1508,29 @@
     self.assertEqual(sd, dict(a=2, b=2, c=4))
 
     # Rebind using both update dict and kwargs.
     sd = Dict(a=1, b=2, c=3)
     sd.rebind({'a': 2, 'b': 3}, a=3, c=3)
     self.assertEqual(sd, dict(a=3, b=3, c=3))
 
+  def test_rebind_with_context_value(self):
+    sd = Dict(a=1, b=2)
+    sd.rebind(a=base.ContextualValue())
+    self.assertEqual(sd, dict(a=base.ContextualValue(), b=2))
+
+    sd = Dict(
+        a=1,
+        b=2,
+        value_spec=pg_typing.Dict(
+            [('a', pg_typing.Int()), ('b', pg_typing.Int())]
+        ),
+    )
+    sd.rebind(a=base.ContextualValue())
+    self.assertEqual(sd, dict(a=base.ContextualValue(), b=2))
+
   def test_rebind_with_typing(self):
     spec = pg_typing.Dict([
         ('a', pg_typing.Int(default=0)),
         ('b', pg_typing.Str(regex='foo.*')),
         ('c', pg_typing.Dict([
             ('x', pg_typing.Int(min_value=1, default=1)),
             ('y', pg_typing.Bool()),
@@ -1720,14 +1847,15 @@
   def test_from_json(self):
     spec = pg_typing.Dict([
         ('w', pg_typing.Str()),
         ('x', pg_typing.Int()),
         ('y', pg_typing.Str().noneable()),
         # Frozen field shall not be written.
         ('z', pg_typing.Bool(True).freeze()),
+        ('p', pg_typing.Int(default=base.ContextualValue())),
     ])
     self.assertEqual(
         base.from_json_str('{"x": 1}').use_value_spec(spec, allow_partial=True),
         Dict.partial(x=1, value_spec=spec))
 
   def test_to_json_on_regular_dict(self):
     self.assertEqual(
@@ -1921,10 +2049,20 @@
                   )
                 }
               ]
             }
           }
         }"""))
 
+  def test_noncompact_with_contextual_value(self):
+    self.assertEqual(
+        Dict(x=1, y=base.ContextualValue()).format(compact=False),
+        inspect.cleandoc("""{
+            x = 1,
+            y = ContextualValue()
+          }
+        """),
+    )
+
 
 if __name__ == '__main__':
   unittest.main()
```

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/symbolic/diff.py` & `pyglove-0.3.1.dev20230524/pyglove/core/symbolic/diff.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/symbolic/diff_test.py` & `pyglove-0.3.1.dev20230524/pyglove/core/symbolic/diff_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/symbolic/flags.py` & `pyglove-0.3.1.dev20230524/pyglove/core/symbolic/flags.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/symbolic/flags_test.py` & `pyglove-0.3.1.dev20230524/pyglove/core/symbolic/flags_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/symbolic/functor.py` & `pyglove-0.3.1.dev20230524/pyglove/core/symbolic/functor.py`

 * *Files 0% similar despite different names*

```diff
@@ -405,15 +405,19 @@
     if self.signature.has_varargs:
       prebound_varargs = keyword_args.pop(self.signature.varargs.name, None)
       varargs = varargs or prebound_varargs
       if varargs:
         list_args.extend(varargs)
 
     return_value = self._call(*list_args, **keyword_args)
-    if self.signature.return_value and flags.is_type_check_enabled():
+    if (
+        self.signature.return_value
+        and flags.is_type_check_enabled()
+        and return_value != pg_typing.MISSING_VALUE
+    ):
       return_value = self.signature.return_value.apply(
           return_value, root_path=self.sym_path + 'returns')
     if flags.is_tracking_origin() and isinstance(return_value, base.Symbolic):
       return_value.sym_setorigin(self, 'return')
     return return_value
```

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/symbolic/functor_test.py` & `pyglove-0.3.1.dev20230524/pyglove/core/symbolic/functor_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -259,15 +259,14 @@
         ('b', pg_typing.Int(max_value=10)),
         ('args', pg_typing.List(pg_typing.Int())),
         (pg_typing.StrKey(), pg_typing.Int(max_value=5))
     ], returns=pg_typing.Int(min_value=0))
     def f(a, *args, b, **kwargs):
       return a + b + sum(args) + sum(kwargs.values())
 
-    print('SIGNATURE', f.signature)
     self.assertEqual(f(1, 2, b=3)(c=4), 10)
 
     # Validate during pre-binding.
     with self.assertRaisesRegex(
         ValueError, 'Value -1 is out of range .*min=0'):
       f(-1, b=1)
 
@@ -304,14 +303,21 @@
         ValueError, 'Value 6 is out of range .*max=5'):
       f(1, b=1)(c=6)
 
     with self.assertRaisesRegex(
         ValueError, 'Value -1 is out of range .*min=0'):
       f(0, b=-1)()
 
+    # Returning pg.MISSING_VALUE will not trigger return value spec check.
+    @pg_functor(auto_typing=True)
+    def g() -> int:
+      return pg_typing.MISSING_VALUE
+
+    self.assertEqual(g()(), pg_typing.MISSING_VALUE)
+
   def test_symbolization_on_nested_containers(self):
     @pg_functor
     def f(a, b):
       del a, b
 
     x = f([], {})
     self.assertIsInstance(x.a, List)
```

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/symbolic/list.py` & `pyglove-0.3.1.dev20230524/pyglove/core/symbolic/list.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,21 @@
 from typing import Any, Callable, Dict, Iterable, Iterator, Optional, Tuple, Union
 from pyglove.core import object_utils
 from pyglove.core import typing as pg_typing
 from pyglove.core.symbolic import base
 from pyglove.core.symbolic import flags
 
 
+# Special default value to detect missing keys in a List. Though its values is
+# the same as `base._RAISE_IF_NOT_FOUND`, they are different instances so
+# `pg.List` and `pg.Symbolic` could use their own instances to control error
+# raising separately.
+_RAISE_IF_NOT_FOUND = (pg_typing.MISSING_VALUE,)
+
+
 class List(list, base.Symbolic, pg_typing.CustomTyping):
   """Symbolic list.
 
   ``pg.List`` implements a list type whose instances are symbolically
   programmable, which is a subclass of the built-in Python ``list``,
   and the subclass of ``pg.Symbolic``.
 
@@ -174,14 +181,18 @@
         root_path=root_path)
 
     self._value_spec = None
     self._onchange_callback = None
 
     list.__init__(self)
     if items:
+      # Copy the symbolic form instead of evaluated form.
+      if isinstance(items, List):
+        items = items.sym_values()
+
       for item in items:
         self._set_item_without_permission_check(len(self), item)
 
     if value_spec:
       self.use_value_spec(value_spec, allow_partial)
 
     # NOTE(daiyip): We set onchange callback at the end of init to avoid
@@ -273,33 +284,36 @@
   def sym_keys(self) -> Iterator[int]:
     """Symbolically iterates indices."""
     for i in range(len(self)):
       yield i
 
   def sym_values(self) -> Iterator[Any]:
     """Iterates the values of symbolic attributes."""
-    return iter(self)
+    for i in range(len(self)):
+      yield super().__getitem__(i)
 
   def sym_items(self) -> Iterator[Tuple[int, Any]]:
     """Iterates the (key, value) pairs of symbolic attributes."""
-    return enumerate(self)
+    for i in range(len(self)):
+      yield (i, super().__getitem__(i))
 
   def sym_hash(self) -> int:
     """Symbolically hashing."""
-    return base.sym_hash((self.__class__, tuple([
-        base.sym_hash(e) for e in self])))
+    return base.sym_hash(
+        (self.__class__, tuple([base.sym_hash(e) for e in self.sym_values()]))
+    )
 
   def _sym_getattr(self, key: int) -> Any:   # pytype: disable=signature-mismatch  # overriding-parameter-type-checks
     """Gets symbolic attribute by index."""
-    return self[key]
+    return super().__getitem__(key)
 
   def _sym_clone(self, deep: bool, memo=None) -> 'List':
     """Override Symbolic._clone."""
     source = []
-    for v in self:
+    for v in self.sym_values():
       if deep or isinstance(v, base.Symbolic):
         v = base.clone(v, deep, memo)
       source.append(v)
     return List(
         source,
         value_spec=self._value_spec,
         allow_partial=self._allow_partial,
@@ -307,15 +321,15 @@
         # NOTE(daiyip): parent and root_path are reset to empty
         # for copy object.
         root_path=None)
 
   def _sym_missing(self) -> Dict[Any, Any]:
     """Returns missing fields."""
     missing = dict()
-    for idx, elem in enumerate(self):
+    for idx, elem in self.sym_items():
       if isinstance(elem, base.Symbolic):
         missing_child = elem.sym_missing(flatten=False)
         if missing_child:
           missing[idx] = missing_child
     return missing
 
   def _sym_rebind(
@@ -336,50 +350,50 @@
     # the largest.
     updates.reverse()
     return updates
 
   def _sym_nondefault(self) -> Dict[int, Any]:
     """Returns non-default values."""
     non_defaults = dict()
-    for idx, elem in enumerate(self):
+    for idx, elem in self.sym_items():
       if isinstance(elem, base.Symbolic):
         non_defaults_child = elem.non_default_values(flatten=False)
         if non_defaults_child:
           non_defaults[idx] = non_defaults_child
       else:
         non_defaults[idx] = elem
     return non_defaults
 
   def set_accessor_writable(self, writable: bool = True) -> 'List':
     """Sets accessor writable."""
     if self.accessor_writable == writable:
       return self
-    for elem in self:
+    for elem in self.sym_values():
       if isinstance(elem, base.Symbolic):
         elem.set_accessor_writable(writable)
     super().set_accessor_writable(writable)
     return self
 
   def seal(self, sealed: bool = True) -> 'List':
     """Seal or unseal current object from further modification."""
     if self.is_sealed == sealed:
       return self
-    for elem in self:
+    for elem in self.sym_values():
       if isinstance(elem, base.Symbolic):
         elem.seal(sealed)
     super().seal(sealed)
     return self
 
   def _update_children_paths(
       self,
       old_path: object_utils.KeyPath,
       new_path: object_utils.KeyPath) -> None:
     """Update children paths according to root_path of current node."""
     del old_path
-    for idx, item in enumerate(self):
+    for idx, item in self.sym_items():
       if isinstance(item, base.Symbolic):
         item.sym_setpath(object_utils.KeyPath(idx, new_path))
 
   def _set_item_without_permission_check(  # pytype: disable=signature-mismatch  # overriding-parameter-type-checks
       self, key: int, value: Any) -> Optional[base.FieldUpdate]:
     """Set or add an item without permission check."""
     assert isinstance(key, int), key
@@ -441,61 +455,84 @@
   def _on_change(self,
                  field_updates: Dict[object_utils.KeyPath, base.FieldUpdate]):
     """On change event of List."""
     # Do nothing for now to handle changes of List.
 
     # NOTE(daiyip): Remove items that are MISSING_VALUES.
     keys_to_remove = []
-    for i, item in enumerate(self):
+    for i, item in self.sym_items():
       if pg_typing.MISSING_VALUE == item:
         keys_to_remove.append(i)
     if keys_to_remove:
       for i in reversed(keys_to_remove):
         list.__delitem__(self, i)
 
     # Update paths for children.
-    for idx, item in enumerate(self):
+    for idx, item in self.sym_items():
       if isinstance(item, base.Symbolic) and item.sym_path.key != idx:
         item.sym_setpath(object_utils.KeyPath(idx, self.sym_path))
 
     if self._onchange_callback is not None:
       self._onchange_callback(field_updates)
 
+  def _parse_slice(self, index: slice) -> Tuple[int, int, int]:
+    start = index.start if index.start is not None else 0
+    start = max(-len(self), start)
+    start = min(len(self), start)
+    if start < 0:
+      start += len(self)
+
+    stop = index.stop if index.stop is not None else len(self)
+    stop = max(-len(self), stop)
+    stop = min(len(self), stop)
+    if stop < 0:
+      stop += len(self)
+
+    step = index.step if index.step is not None else 1
+    return start, stop, step
+
+  def _sym_value(self, key: int, default: Any) -> Any:  # pytype: disable=signature-mismatch
+    try:
+      v = super().__getitem__(key)
+    except IndexError:
+      return default
+
+    def _eval(i, v):
+      if isinstance(v, base.ContextualValue):
+        return self.sym_contextual_getattr(
+            i, default=default, getter=v, start=self.sym_parent
+        )
+      return v
+
+    if isinstance(key, slice):
+      return [
+          _eval(k, v[i]) for i, k in enumerate(range(*self._parse_slice(key)))
+      ]
+    return _eval(key, v)
+
   def __getitem__(self, index) -> Any:
     """Gets the item at a given position."""
-    v = super().__getitem__(index)
-    if isinstance(v, base.ContextualValue):
-      v = self.sym_contextual_getattr(index, getter=v, start=self.sym_parent)
+    v = self.sym_value(index, _RAISE_IF_NOT_FOUND)
+    if v is _RAISE_IF_NOT_FOUND:
+      raise IndexError('list index out of range')
     return v
 
   def __setitem__(self, index, value: Any) -> None:
     """Set item in this List."""
     if base.treats_as_sealed(self):
       raise base.WritePermissionError(
           self._error_message('Cannot set item for a sealed List.'))
 
     if not base.writtable_via_accessors(self):
       raise base.WritePermissionError(
           self._error_message('Cannot modify List item by __setitem__ while '
                               'accessor_writable is set to False. '
                               'Use \'rebind\' method instead.'))
     if isinstance(index, slice):
-      start = index.start if index.start is not None else 0
-      start = max(-len(self), start)
-      start = min(len(self), start)
-      if start < 0:
-        start += len(self)
-
-      stop = index.stop if index.stop is not None else len(self)
-      stop = max(-len(self), stop)
-      stop = min(len(self), stop)
-      if stop < 0:
-        stop += len(self)
-
-      step = index.step if index.step is not None else 1
+      start, stop, step = self._parse_slice(index)
       replacements = [self._formalized_value(i, v) for i, v in enumerate(value)]
       if step < 0:
         replacements.reverse()
         step = -step
       slice_size = math.ceil((stop - start) * 1.0 / step)
       if step == 1:
         if slice_size < len(replacements):
@@ -543,15 +580,15 @@
           f'list index must be an integer. Encountered {index!r}.')
 
     if index < -len(self) or index >= len(self):
       raise IndexError(
           f'list index out of range. '
           f'Length={len(self)}, index={index}')
 
-    old_value = self[index]
+    old_value = self.sym_getattr(index)
     super().__delitem__(index)
 
     if flags.is_change_notification_enabled():
       self._notify_field_updates([
           base.FieldUpdate(
               self.sym_path + index, self,
               self._value_spec.element if self._value_spec else None,
@@ -605,23 +642,23 @@
     if flags.is_change_notification_enabled() and update:
       self._notify_field_updates([update])
 
   def pop(self, index: int = -1) -> Any:
     """Pop an item and return its value."""
     if index < -len(self) or index >= len(self):
       raise IndexError('pop index out of range')
-
+    index = (index + len(self)) % len(self)
     value = self[index]
     with flags.allow_writable_accessors(True):
       del self[index]
     return value
 
   def remove(self, value: Any) -> None:
     """Removes the first occurrence of the value."""
-    for i, item in enumerate(self):
+    for i, item in self.sym_items():
       if item == value:
         if (self._value_spec and self._value_spec.min_size == len(self)):
           raise ValueError(
               f'Cannot remove item: min size ({self._value_spec.min_size}) '
               f'is reached.')
         del self[i]
         return
@@ -632,15 +669,17 @@
       raise base.WritePermissionError('Cannot extend a sealed List.')
     other = list(other)
     if self.max_size is not None and len(self) + len(other) > self.max_size:
       raise ValueError(
           f'Cannot extend List: the number of elements '
           f'({len(self) + len(other)}) exceeds max size ({self.max_size}).')
     updates = []
-    for v in other:
+    # Extend on the symbolic form instead of the evaluated form.
+    iter_other = other.sym_values() if isinstance(other, List) else other
+    for v in iter_other:
       update = self._set_item_without_permission_check(len(self), v)
       if update is not None:
         updates.append(update)
 
     if flags.is_change_notification_enabled() and updates:
       self._notify_field_updates(updates)
 
@@ -699,15 +738,15 @@
         self._allow_partial = allow_partial
     elif isinstance(value_spec, pg_typing.List):
       self._value_spec = value_spec
     return (proceed_with_standard_apply, self)
 
   def sym_jsonify(self, **kwargs) -> object_utils.JSONValueType:
     """Converts current list to a list of plain Python objects."""
-    return [base.to_json(v, **kwargs) for v in self]
+    return [base.to_json(v, **kwargs) for v in self.sym_values()]
 
   def format(
       self,
       compact: bool = False,
       verbose: bool = True,
       root_indent: int = 0,
       *,
@@ -721,27 +760,27 @@
       return ' ' * 2 * indent + text
 
     cls_name = cls_name or ''
     open_bracket, close_bracket = object_utils.bracket_chars(bracket_type)
     s = [f'{cls_name}{open_bracket}']
     if compact:
       kv_strs = []
-      for idx, elem in enumerate(self):
+      for idx, elem in self.sym_items():
         v_str = object_utils.format(
             elem, compact, verbose, root_indent + 1,
             python_format=python_format, **kwargs)
         if python_format:
           kv_strs.append(v_str)
         else:
           kv_strs.append(f'{idx}: {v_str}')
       s.append(', '.join(kv_strs))
       s.append(close_bracket)
     else:
       if self:
-        for idx, elem in enumerate(self):
+        for idx, elem in self.sym_items():
           if idx == 0:
             s.append('\n')
           else:
             s.append(',\n')
           v_str = object_utils.format(
               elem, compact, verbose, root_indent + 1,
               python_format=python_format, **kwargs)
```

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/symbolic/list_test.py` & `pyglove-0.3.1.dev20230524/pyglove/core/symbolic/list_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,14 +55,18 @@
 
     # Schematized list.
     vs = pg_typing.List(pg_typing.Int())
     sl = List([1], value_spec=vs)
     self.assertIs(sl.value_spec, vs)
     self.assertEqual(sl, [1])
 
+    # List with contextual value.
+    sl = List(List([base.ContextualValue()]))
+    self.assertEqual(sl, [base.ContextualValue()])
+
     with self.assertRaisesRegex(
         TypeError, '.* must be a `pg.typing.List` object.'):
       List(value_spec=pg_typing.Int())
 
   def test_partial(self):
     spec = pg_typing.List(pg_typing.Dict([
         ('a', pg_typing.Int()),
@@ -259,14 +263,30 @@
 
     # Slicing.
     sl = List([0, 1, 2])
     self.assertEqual(sl[:-1], [0, 1])
     self.assertEqual(sl[1:], [1, 2])
     self.assertEqual(sl[:], [0, 1, 2])
 
+    # Context value
+    sl = List([base.ContextualValue(), 2, base.ContextualValue()])
+    with self.assertRaises(AttributeError):
+      _ = sl[0]
+
+    sl2 = List([123, sl, 456])
+    self.assertEqual(sl[0], 123)
+
+    # Slicing contextual values.
+    self.assertEqual(sl[1:], [2, 456])
+    self.assertEqual(sl[:-1], [123, 2])
+    self.assertEqual(sl[::2], [123, 456])
+    self.assertEqual(sl[::], [123, 2, 456])
+    self.assertEqual(sl[-1:0:-1], [456, 2])
+    del sl2
+
   def test_delitem(self):
     # Delete an item from a schemaless dict.
     sl = List([0])
     del sl[0]
     self.assertEqual(len(sl), 0)
 
     sl = List([0])
@@ -317,32 +337,32 @@
     sl.seal()
     with self.assertRaisesRegex(
         base.WritePermissionError, 'Cannot append element on a sealed List.'):
       sl.append(4)
 
   def test_extend(self):
     sl = List([0, 1])
-    sl.extend([2, 3])
-    self.assertEqual(sl, [0, 1, 2, 3])
+    sl.extend([2, base.ContextualValue()])
+    self.assertEqual(sl, [0, 1, 2, base.ContextualValue()])
 
     sl = List([0, 1], value_spec=pg_typing.List(pg_typing.Int(), max_size=4))
     with self.assertRaisesRegex(
         ValueError,
         'Cannot extend List: the number of elements .* exceeds max size'):
       sl.extend([2, 3, 4])
     self.assertEqual(sl, [0, 1])
     sl.seal()
     with self.assertRaisesRegex(
         base.WritePermissionError, 'Cannot extend a sealed List.'):
       sl.extend([0, 1])
 
   def test_concatenate(self):
-    sl = List([0]) + List([1])
+    sl = List([0]) + List([base.ContextualValue()])
     self.assertIsInstance(sl, List)
-    self.assertEqual(sl, [0, 1])
+    self.assertEqual(sl, [0, base.ContextualValue()])
 
     spec = pg_typing.List(pg_typing.Int(min_value=0))
     sl = List([0], value_spec=spec) + [1, 2]
     self.assertIsInstance(sl, List)
     self.assertIs(sl.value_spec, spec)
     self.assertEqual(sl, [0, 1, 2])
 
@@ -398,14 +418,19 @@
       sl.remove(2)
 
     sl = List([0, 1], value_spec=pg_typing.List(pg_typing.Int(), min_size=2))
     with self.assertRaisesRegex(
         ValueError, 'Cannot remove item: min size .* is reached'):
       sl.remove(1)
 
+    # Remove contextual value.
+    sl = List([base.ContextualValue()])
+    sl.remove(base.ContextualValue())
+    self.assertEqual(sl, [])
+
   def test_pop(self):
     sl = List([0, 1, 2])
     self.assertEqual(sl.pop(), 2)
     self.assertEqual(sl, [0, 1])
 
     sl.seal()
     with self.assertRaisesRegex(
@@ -414,14 +439,27 @@
 
     with self.assertRaisesRegex(IndexError, 'pop index out of range'):
       _ = sl.pop(5)
 
     with self.assertRaisesRegex(IndexError, 'pop index out of range'):
       _ = sl.pop(-3)
 
+    # pop with contextual value.
+    sl = List([base.ContextualValue()])
+    with self.assertRaises(AttributeError):
+      sl.pop()
+    self.assertEqual(sl, [base.ContextualValue()])
+
+    sl2 = List([23, sl, 45])
+    self.assertEqual(len(sl), 1)
+    self.assertEqual(sl[0], 23)
+    self.assertEqual(sl.pop(), 23)
+    self.assertEqual(sl, [])
+    del sl2
+
   def test_clear(self):
     sl = List([0, 1])
     sl.clear()
     self.assertEqual(len(sl), 0)
 
     sl = List([0, 1])
     with flags.as_sealed():
@@ -463,36 +501,47 @@
   def test_index(self):
     sl = List([0, 1, 2, 1])
     self.assertEqual(sl.index(1), 1)
     with self.assertRaisesRegex(
         ValueError, '3 is not in list'):
       _ = sl.index(3)
 
+    # Index of contextual value is based on its symbolic form.
+    # TODO(daiyip): revise the behavior.
+    sl = List([0, base.ContextualValue(), 1])
+    self.assertEqual(sl.index(base.ContextualValue()), 1)
+    self.assertEqual(sl.index(1), 2)
+
   def test_count(self):
-    sl = List([0, 1, 2, 1])
+    # Count of contextual value is also based on its symbolic form.
+    # TODO(daiyip): revise the behavior.
+    sl = List([0, 1, base.ContextualValue(), 2, 1, base.ContextualValue()])
     self.assertEqual(sl.count(1), 2)
     self.assertEqual(sl.count(3), 0)
+    self.assertEqual(sl.count(base.ContextualValue()), 2)
 
   def test_copy(self):
 
     class A:
       pass
 
-    sl = List([0, A(), dict(x=A()), list([A()])])
+    sl = List([base.ContextualValue(), A(), dict(x=A()), list([A()])])
     sl2 = sl.copy()
     self.assertIsInstance(sl2, List)
     self.assertEqual(sl, sl2)
     self.assertIsNot(sl, sl2)
     self.assertIs(sl[1], sl2[1])
     self.assertIsNot(sl[2], sl2[2])
     self.assertIsNot(sl[3], sl2[3])
     self.assertIs(sl[2].x, sl2[2].x)
     self.assertIs(sl[3][0], sl2[3][0])
 
-    sl = List([0], value_spec=pg_typing.List(pg_typing.Int()))
+    sl = List(
+        [base.ContextualValue()], value_spec=pg_typing.List(pg_typing.Int())
+    )
     sl2 = sl.copy()
     self.assertIs(sl.value_spec, sl2.value_spec)
 
     # Test copy.copy.
     sl = List([0, A(), dict(x=A()), list([A()])])
     sl3 = copy.copy(sl)
     self.assertIsInstance(sl3, List)
@@ -510,15 +559,15 @@
 
       def __init__(self, v):
         self.v = v
 
       def __eq__(self, other):
         return isinstance(other, B) and self.v == other.v
 
-    sl = List([0, B(1), dict(x=B(2)), list([B(3)])])
+    sl = List([base.ContextualValue(), B(1), dict(x=B(2)), list([B(3)])])
     sl4 = copy.deepcopy(sl)
     self.assertIsInstance(sl4, List)
     self.assertEqual(sl, sl4)
     self.assertIsNot(sl, sl4)
     self.assertIsNot(sl[1], sl4[1])
     self.assertIsNot(sl[2], sl4[2])
     self.assertIsNot(sl[3], sl4[3])
@@ -532,28 +581,40 @@
 
     sl.append(-1)
     sl.seal()
     with self.assertRaisesRegex(
         base.WritePermissionError, 'Cannot sort a sealed List'):
       sl.sort()
 
+    # List with contextual value cannot be sorted.
+    sl = List([0, 2, base.ContextualValue(), 3])
+    with self.assertRaises(TypeError):
+      sl.sort()
+
   def test_reverse(self):
     sl = List([0, 2, 1, 3])
     sl.reverse()
     self.assertEqual(sl, [3, 1, 2, 0])
 
     sl.seal()
     with self.assertRaisesRegex(
         base.WritePermissionError, 'Cannot reverse a sealed List'):
       sl.reverse()
 
+    # List with contextual value is reversed in its symbolic form.
+    sl = List([0, 2, base.ContextualValue(), 3])
+    sl.reverse()
+    self.assertEqual(sl, [3, base.ContextualValue(), 2, 0])
+
   def test_in(self):
-    sl = List([0, 1, 2])
+    sl = List([0, 1, base.ContextualValue()])
     self.assertIn(1, sl)
     self.assertNotIn(3, sl)
+    # In-test is based on the symbolic form.
+    self.assertIn(base.ContextualValue(), sl)
 
   def test_iter(self):
     sl = List([0, 1, 2, 3])
     self.assertEqual(list(sl), [0, 1, 2, 3])
 
   def test_non_default(self):
     sl = List([0])
@@ -629,14 +690,26 @@
     self.assertIsNone(sl.sym_getattr(1, None))
     self.assertIsNone(sl.sym_getattr('x', None))
     with self.assertRaisesRegex(
         AttributeError,
         '.* object has no symbolic attribute 1.'):
       sl.sym_getattr(1)
 
+  def test_sym_value(self):
+    @contextual.contextual_getter
+    def static_value(context, v):
+      del context
+      return v
+
+    sd = List([1, static_value(v=0)])  # pylint: disable=no-value-for-parameter
+    self.assertEqual(sd.sym_value(0), 1)
+    self.assertEqual(sd.sym_value(1), 0)
+    with self.assertRaisesRegex(AttributeError, '2'):
+      _ = sd.sym_value(2)
+
   def test_sym_field(self):
     sl = List([dict(x=[], y={})])
     self.assertIsNone(sl.sym_field)
 
     spec = pg_typing.List(pg_typing.Dict([
         ('x', pg_typing.List(pg_typing.Int())),
         ('y', pg_typing.Dict())
@@ -672,58 +745,68 @@
     sl = List([dict(x=1), dict(x=2)], value_spec=pg_typing.List(pg_typing.Dict([
         ('x', pg_typing.Int()),
         ('y', pg_typing.Int(default=0))
     ])))
     self.assertEqual(next(sl.sym_values()), dict(x=1, y=0))
     self.assertEqual(list(sl.sym_values()), [dict(x=1, y=0), dict(x=2, y=0)])
 
+    sl = List([1, base.ContextualValue()])
+    self.assertEqual(next(sl.sym_values()), 1)
+    self.assertEqual(list(sl.sym_values()), [1, base.ContextualValue()])
+
   def test_sym_items(self):
     sl = List(['a', 'b'])
     self.assertEqual(next(sl.sym_items()), (0, 'a'))
     self.assertEqual(list(sl.sym_items()), [(0, 'a'), (1, 'b')])
 
     sl = List([dict(x=1), dict(x=2)], value_spec=pg_typing.List(pg_typing.Dict([
         ('x', pg_typing.Int()),
         ('y', pg_typing.Int(default=0))
     ])))
     self.assertEqual(next(sl.sym_items()), (0, dict(x=1, y=0)))
     self.assertEqual(
         list(sl.sym_items()), [(0, dict(x=1, y=0)), (1, dict(x=2, y=0))])
 
+    sl = List([1, base.ContextualValue()])
+    self.assertEqual(next(sl.sym_items()), (0, 1))
+    self.assertEqual(
+        list(sl.sym_items()), [(0, 1), (1, base.ContextualValue())]
+    )
+
   def test_sym_jsonify(self):
     # Refer to SerializationTest for more detailed tests.
-    sl = List([0])
-    self.assertEqual(sl.sym_jsonify(), [0])
+    sl = List([0, base.ContextualValue()])
+    self.assertEqual(sl.sym_jsonify(), [0, base.ContextualValue().to_json()])
 
   def test_sym_rebind(self):
     # Refer to RebindTest for more detailed tests.
     sl = List([0, 1, 2])
-    sl.sym_rebind({
-        0: MISSING_VALUE,
-        1: 3,
-        2: Insertion(4),
-        4: 5
-    })
-    self.assertEqual(sl, [3, 4, 2, 5])
+    sl.sym_rebind(
+        {0: MISSING_VALUE, 1: 3, 2: Insertion(4), 4: base.ContextualValue()}
+    )
+    self.assertEqual(list(sl.sym_values()), [3, 4, 2, base.ContextualValue()])
 
   def test_sym_clone(self):
     class A():
       pass
 
-    sl = List([[], dict(), A()])
+    sl = List([[], dict(), A(), base.ContextualValue()])
     sl2 = sl.clone()
     self.assertEqual(sl, sl2)
     self.assertIsNot(sl, sl2)
     # Symbolic members are always copied by value.
     self.assertIsNot(sl[0], sl2[0])
     self.assertIsNot(sl[1], sl2[1])
 
     # Non-symbolic members are copied by reference.
     self.assertIs(sl[2], sl2[2])
 
+    # Contextual values are copied by symbols.
+    self.assertEqual(sl.sym_getattr(3), sl.sym_getattr(3))
+
     spec = pg_typing.List(pg_typing.Dict([
         (pg_typing.StrKey(), pg_typing.Any())
     ]))
     sl = List([Dict(x=list(), z=dict(), y=A())], value_spec=spec)
     sl2 = sl.sym_clone(deep=True)
 
     # Instances of `A` are compared by reference.
@@ -752,29 +835,37 @@
     ])))
     self.assertTrue(sl.sym_partial)
     sl.rebind({'[0].y.z': 2})
     self.assertFalse(sl.sym_partial)
 
   def test_sym_missing(self):
     # Refer to `test_missing_values` for more details.
-    sl = List.partial([dict(x=1)], value_spec=pg_typing.List(pg_typing.Dict([
-        ('x', pg_typing.Int()),
-        ('y', pg_typing.Int()),
-    ])))
+    sl = List.partial(
+        [dict(x=base.ContextualValue())],
+        value_spec=pg_typing.List(
+            pg_typing.Dict([
+                ('x', pg_typing.Int()),
+                ('y', pg_typing.Int()),
+            ])
+        ),
+    )
     self.assertEqual(sl.sym_missing(), {'[0].y': MISSING_VALUE})
 
   def test_sym_nondefault(self):
     # Refer to `test_non_default_values` for more details.
-    sl = List([dict(x=1)], value_spec=pg_typing.List(pg_typing.Dict([
-        ('x', pg_typing.Int(default=0)),
-        ('y', pg_typing.Dict([
-            ('z', pg_typing.Int(default=1))
-        ])),
-    ])))
-    self.assertEqual(sl.sym_nondefault(), {'[0].x': 1})
+    sl = List(
+        [dict(x=base.ContextualValue())],
+        value_spec=pg_typing.List(
+            pg_typing.Dict([
+                ('x', pg_typing.Int(default=0)),
+                ('y', pg_typing.Dict([('z', pg_typing.Int(default=1))])),
+            ])
+        ),
+    )
+    self.assertEqual(sl.sym_nondefault(), {'[0].x': base.ContextualValue()})
     sl.rebind({'[0].y.z': 2, '[0].x': 0})
     self.assertEqual(sl.sym_nondefault(), {'[0].y.z': 2})
 
   def test_sym_puresymbolic(self):
     self.assertFalse(List().sym_puresymbolic)
 
     class A(PureSymbolic):
@@ -1153,19 +1244,20 @@
     self.assertTrue(sl.is_sealed)
     self.assertTrue(sl[0].is_sealed)
 
   def test_contextual(self):
     # Test contextual access for schemaless list.
     # Okay: sl[1] is contextual.
     @contextual.contextual_getter
-    def redirectd_value(k, p, key):
-      del k
-      return getattr(p, key)
+    def redirected_value(context, key):
+      if context.container:
+        return getattr(context.container, key)
+      return object_utils.MISSING_VALUE
 
-    sl = List([0, redirectd_value(key='a')])  # pylint: disable=no-value-for-parameter
+    sl = List([0, redirected_value(key='a')])  # pylint: disable=no-value-for-parameter
 
     self.assertEqual(sl[0], 0)
     with self.assertRaisesRegex(
         AttributeError, '`1` is not found under its context'
     ):
       _ = sl[1]
```

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/symbolic/object.py` & `pyglove-0.3.1.dev20230524/pyglove/core/symbolic/object.py`

 * *Files 2% similar despite different names*

```diff
@@ -364,28 +364,28 @@
   @classmethod
   def _create_sym_attribute(cls, attr_name, field):
     """Customizable trait: template of single symbolic attribute."""
     return property(
         object_utils.make_function(
             attr_name,
             ['self'],
-            [f"return self._sym_attributes['{attr_name}']"],
+            [f"return self.sym_value('{attr_name}')"],
             return_type=field.value.annotation,
         )
     )
 
   @classmethod
   def _begin_annotation_inference(cls) -> None:
-    """Event that is triggered before annotation infererence begins."""
+    """Event that is triggered before annotation inference begins."""
 
   @classmethod
   def _end_annotation_inference(
       cls, fields: List[pg_typing.Field]
   ) -> List[pg_typing.Field]:
-    """Event that is triggered before annotation infererence begins."""
+    """Event that is triggered after annotation inference ends."""
     return fields
 
   #
   # Class methods.
   #
 
   @classmethod
@@ -617,24 +617,32 @@
       old_parent: Optional[base.Symbolic],
       new_parent: Optional[base.Symbolic]):
     """Event that is triggered after the symbolic parent changes."""
     del old_parent, new_parent
 
   @property
   def sym_init_args(self) -> pg_dict.Dict:
-    """Returns symbolic attributes which are the arguments for `__init__`."""
+    """Returns the symbolic attributes which are also the `__init__` args.
+
+    Returns:
+      A symbolic Dict as evaluated symbolic attributes, meaning that all
+        ``pg.ContextValue`` will be resolved.
+    """
     return self._sym_attributes
 
   def sym_hasattr(self, key: Union[str, int]) -> bool:
     """Tests if a symbolic attribute exists."""
     if key == '_sym_attributes':
       raise ValueError(
           f'{self.__class__.__name__}.__init__ should call `super().__init__`.')
-    return (isinstance(key, str)
-            and not key.startswith('_') and key in self._sym_attributes)
+    return (
+        isinstance(key, str)
+        and not key.startswith('_')
+        and key in self._sym_attributes
+    )
 
   def sym_attr_field(
       self, key: Union[str, int]
       ) -> Optional[pg_typing.Field]:
     """Returns the field definition for a symbolic attribute."""
     return self._sym_attributes.sym_attr_field(key)
 
@@ -672,29 +680,29 @@
     super().sym_setparent(parent)
     if old_parent is not parent:
       self._on_parent_change(old_parent, parent)
 
   def _sym_getattr(  # pytype: disable=signature-mismatch  # overriding-parameter-type-checks
       self, key: str) -> Any:
     """Get symbolic field by key."""
-    return self._sym_attributes[key]
+    return self._sym_attributes.sym_getattr(key)
 
   def _sym_rebind(
       self, path_value_pairs: Dict[object_utils.KeyPath, Any]
       ) -> List[base.FieldUpdate]:
     """Rebind current object using object-form members."""
     if base.treats_as_sealed(self):
       raise base.WritePermissionError(
           f'Cannot rebind a sealed {self.__class__.__name__}.')
     return self._sym_attributes._sym_rebind(path_value_pairs)  # pylint: disable=protected-access
 
   def _sym_clone(self, deep: bool, memo: Any = None) -> 'Object':
     """Copy flags."""
     kwargs = dict()
-    for k, v in self._sym_attributes.items():
+    for k, v in self._sym_attributes.sym_items():
       if deep or isinstance(v, base.Symbolic):
         v = base.clone(v, deep, memo)
       kwargs[k] = v
     return self.__class__(allow_partial=self._allow_partial,
                           sealed=self._sealed,
                           **kwargs)  # pytype: disable=not-instantiable
 
@@ -771,15 +779,18 @@
   def __getattribute__(self, name: str) -> Any:
     """Override to accomondate symbolic attributes with variable keys."""
     try:
       return super().__getattribute__(name)
     except AttributeError as error:
       if not self.allow_symbolic_attribute or not self.sym_hasattr(name):
         raise error
-      return self._sym_getattr(name)
+      return self.sym_value(name)
+
+  def _sym_value(self, key: int, default: Any) -> Any:  # pytype: disable=signature-mismatch
+    return self._sym_attributes._sym_value(key, default)  # pylint: disable=protected-access
 
   def __eq__(self, other: Any) -> bool:
     """Operator==."""
     if self.use_symbolic_comparison:
       return self.sym_eq(other)
     return super().__eq__(other)
```

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/symbolic/object_test.py` & `pyglove-0.3.1.dev20230524/pyglove/core/symbolic/object_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -568,14 +568,24 @@
         self.z = self.x + int(self.y)
 
     a = A(1)
     self.assertEqual(a.x, 1)
     self.assertTrue(a.y)      # Use default value from the field definition.
     self.assertEqual(a.z, 2)  # Non-symbolic field.
 
+    class B(Object):
+      x: int
+
+    b = B(base.ContextualValue())
+    with self.assertRaises(AttributeError):
+      _ = b.x
+
+    sd = Dict(x=1, b=b)
+    self.assertEqual(sd.b.x, 1)
+
   def test_non_default(self):
 
     @pg_members([
         ('x', pg_typing.Int()),
         ('y', pg_typing.Bool(default=True)),
         ('z', pg_typing.Dict([
             ('p', pg_typing.Float(default=1.0))
@@ -610,14 +620,21 @@
         a.missing_values(flatten=False),
         {'x': MISSING_VALUE, 'z': {'p': MISSING_VALUE}})
 
     # After rebind, the non_default_values are updated.
     a.rebind({'x': 1, 'y': MISSING_VALUE, 'z.p': 1.0})
     self.assertEqual(a.missing_values(), {})
 
+    # Test contextual value as the default value.
+    class B(Object):
+      x: int
+
+    b = B(base.ContextualValue())
+    self.assertEqual(b.sym_missing(), {})
+
   def test_sym_has(self):
 
     @pg_members([
         ('x', pg_typing.Any())
     ])
     class A(Object):
 
@@ -630,29 +647,32 @@
     self.assertTrue(a.sym_has('x.x'))
     self.assertTrue(a.sym_has(object_utils.KeyPath.parse('x.x.y')))
     self.assertTrue(a.sym_has(object_utils.KeyPath.parse('x.x.y.x')))
     self.assertFalse(a.sym_has('y'))   # `y` is not a symbolic field.
 
   def test_sym_get(self):
 
-    @pg_members([
-        ('x', pg_typing.Any())
-    ])
+    @pg_members([('x', pg_typing.Any()), ('p', pg_typing.Any().noneable())])
     class A(Object):
 
       def _on_bound(self):
         super()._on_bound()
         self.y = 1
 
-    a = A(A(dict(y=A(1))))
+    a = A(A(dict(y=A(1, p=base.ContextualValue()))), p=base.ContextualValue())
 
     self.assertIs(a.sym_get('x'), a.x)
+    self.assertIs(a.sym_get('p'), a.sym_getattr('p'))
     self.assertIs(a.sym_get('x.x'), a.x.x)
     self.assertIs(a.sym_get(object_utils.KeyPath.parse('x.x.y')), a.x.x.y)
     self.assertIs(a.sym_get(object_utils.KeyPath.parse('x.x.y.x')), a.x.x.y.x)
+    self.assertIs(
+        a.sym_get(object_utils.KeyPath.parse('x.x.y.p')),
+        a.x.x.y.sym_getattr('p'),
+    )
 
     with self.assertRaisesRegex(
         KeyError, 'Path y does not exist.'):  # `y` is not a symbolic field.
       a.sym_get('y')
 
   def test_sym_hasattr(self):
 
@@ -692,14 +712,18 @@
 
       def _on_bound(self):
         super()._on_bound()
         self.y = 1
 
     a = A(1)
     self.assertEqual(a.sym_getattr('x'), 1)
+
+    a = A(x=base.ContextualValue())
+    self.assertEqual(a.sym_getattr('x'), base.ContextualValue())
+
     with self.assertRaisesRegex(
         AttributeError, 'has no symbolic attribute \'y\''):
       _ = a.sym_getattr('y')
 
     @pg_members([
         (pg_typing.StrKey('x.*'), pg_typing.Int())
     ])
@@ -712,14 +736,30 @@
 
     self.assertEqual(b.sym_getattr('x1'), 1)
     self.assertEqual(b.sym_getattr('x2'), 2)
     with self.assertRaisesRegex(
         AttributeError, 'has no symbolic attribute \'y\''):
       _ = b.sym_getattr('y')
 
+  def test_sym_value(self):
+    @contextual.contextual_getter
+    def static_value(context, v):
+      del context
+      return v
+
+    class A(Object):
+      x: int = 1
+      y: int = static_value(v=0)  # pylint: disable=no-value-for-parameter
+
+    a = A()
+    self.assertEqual(a.sym_value('x'), 1)
+    self.assertEqual(a.sym_value('y'), 0)
+    with self.assertRaisesRegex(AttributeError, 'z'):
+      _ = a.sym_value('z')
+
   def test_sym_contextual_hasattr(self):
     class A(Object):
       x: int
       y: int = 1
       z: int = base.ContextualValue()
 
     a = A(0)
@@ -731,17 +771,18 @@
     # Custom start.
     self.assertFalse(a.sym_contextual_hasattr('x', start=a.sym_parent))
     self.assertFalse(a.sym_contextual_hasattr('y', start=a.sym_parent))
     self.assertTrue(a.sym_contextual_hasattr('z', start=a.sym_parent))
 
     # Custom getter.
     @contextual.contextual_getter
-    def redirected_value(k, p, key):
-      del k
-      return getattr(p, key)
+    def redirected_value(context, key):
+      if context.container:
+        return getattr(context.container, key)
+      return pg_typing.MISSING_VALUE
 
     getter = redirected_value(key='b')  # pylint: disable=no-value-for-parameter
     self.assertTrue(a.sym_contextual_hasattr('x', getter, start=a.sym_parent))
     self.assertTrue(a.sym_contextual_hasattr('y', getter, start=a.sym_parent))
     self.assertTrue(a.sym_contextual_hasattr('z', getter, start=a.sym_parent))
 
   def test_sym_contextual_getattr(self):
@@ -773,17 +814,18 @@
     ):
       a.sym_contextual_getattr('y', start=a.sym_parent)
 
     self.assertEqual(a.sym_contextual_getattr('z', start=a.sym_parent), 2)
 
     # Custom getter.
     @contextual.contextual_getter
-    def redirected_value(k, p, key):
-      del k
-      return getattr(p, key)
+    def redirected_value(context, key):
+      if context.container:
+        return getattr(context.container, key)
+      return pg_typing.MISSING_VALUE
 
     getter = redirected_value(key='b')  # pylint: disable=no-value-for-parameter
     self.assertEqual(
         a.sym_contextual_getattr('x', getter=getter, start=a.sym_parent), 3
     )
     self.assertEqual(
         a.sym_contextual_getattr('y', getter=getter, start=a.sym_parent), 3
@@ -1883,26 +1925,29 @@
     with self.assertRaisesRegex(
         AttributeError, '`y` is not found under its context'
     ):
       _ = a.y
 
     # Test parent contextual value with custom getter.
     @contextual.contextual_getter
-    def redirected_value(k, p, key):
-      del k
-      return getattr(p, key)
+    def redirected_value(context, key):
+      if context.container:
+        return getattr(context.container, key)
+      return pg_typing.MISSING_VALUE
 
     sd = Dict(a='bar', b=Dict(x=a, y=redirected_value(key='a')))  # pylint: disable=no-value-for-parameter
 
     # a.y is redirected to sd.a.
     self.assertEqual(a.y, 'bar')
 
     @contextual.contextual_getter
-    def immediate_attr(k, p):
-      return p.sym_getattr(k)
+    def immediate_attr(context):
+      if context.container:
+        return context.container.sym_getattr(context.key)
+      return pg_typing.MISSING_VALUE
 
     class B(Object):
       x: int = immediate_attr()  # pylint: disable=no-value-for-parameter
 
     b = B()
     sd = Dict(a='bar', b=Dict(b=b, x=redirected_value(key='a')))  # pylint: disable=no-value-for-parameter
 
@@ -1931,15 +1976,15 @@
 
     a.rebind(x=2, y=2)
     self.assertEqual(a, A(2, 2))
     self.assertEqual(a.z, 4)
 
     # Rebind using both update dict and kwargs.
     a = A(1, 2)
-    a.rebind({'x': 2}, x=3, y=3)
+    a.rebind(Dict(x=2), x=3, y=3)
     self.assertEqual(a, A(3, 3))
     self.assertEqual(a.z, 6)
 
   def test_rebind_with_typing(self):
 
     @pg_members([
         ('x', pg_typing.Int(min_value=0)),
```

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/symbolic/origin.py` & `pyglove-0.3.1.dev20230524/pyglove/core/symbolic/origin.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/symbolic/origin_test.py` & `pyglove-0.3.1.dev20230524/pyglove/core/symbolic/origin_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/symbolic/pure_symbolic.py` & `pyglove-0.3.1.dev20230524/pyglove/core/symbolic/pure_symbolic.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/symbolic/schema_utils.py` & `pyglove-0.3.1.dev20230524/pyglove/core/symbolic/schema_utils.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/symbolic/schema_utils_test.py` & `pyglove-0.3.1.dev20230524/pyglove/core/symbolic/schema_utils_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/symbolic/symbolize.py` & `pyglove-0.3.1.dev20230524/pyglove/core/symbolic/symbolize.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/symbolic/symbolize_test.py` & `pyglove-0.3.1.dev20230524/pyglove/core/symbolic/symbolize_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/tuning/__init__.py` & `pyglove-0.3.1.dev20230524/pyglove/core/tuning/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/tuning/backend.py` & `pyglove-0.3.1.dev20230524/pyglove/core/tuning/backend.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/tuning/backend_test.py` & `pyglove-0.3.1.dev20230524/pyglove/core/tuning/backend_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/tuning/early_stopping.py` & `pyglove-0.3.1.dev20230524/pyglove/core/tuning/early_stopping.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/tuning/local_backend.py` & `pyglove-0.3.1.dev20230524/pyglove/core/tuning/local_backend.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/tuning/protocols.py` & `pyglove-0.3.1.dev20230524/pyglove/core/tuning/protocols.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/tuning/protocols_test.py` & `pyglove-0.3.1.dev20230524/pyglove/core/tuning/protocols_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/tuning/sample.py` & `pyglove-0.3.1.dev20230524/pyglove/core/tuning/sample.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/tuning/sample_test.py` & `pyglove-0.3.1.dev20230524/pyglove/core/tuning/sample_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/typing/__init__.py` & `pyglove-0.3.1.dev20230524/pyglove/core/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/typing/annotation_conversion.py` & `pyglove-0.3.1.dev20230524/pyglove/core/typing/annotation_conversion.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/typing/annotation_conversion_test.py` & `pyglove-0.3.1.dev20230524/pyglove/core/typing/annotation_conversion_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/typing/callable_ext.py` & `pyglove-0.3.1.dev20230524/pyglove/core/typing/callable_ext.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/typing/callable_ext_test.py` & `pyglove-0.3.1.dev20230524/pyglove/core/typing/callable_ext_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/typing/callable_signature.py` & `pyglove-0.3.1.dev20230524/pyglove/core/typing/callable_signature.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/typing/callable_signature_test.py` & `pyglove-0.3.1.dev20230524/pyglove/core/typing/callable_signature_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/typing/class_schema.py` & `pyglove-0.3.1.dev20230524/pyglove/core/typing/class_schema.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/typing/class_schema_test.py` & `pyglove-0.3.1.dev20230524/pyglove/core/typing/class_schema_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/typing/class_schema_utils.py` & `pyglove-0.3.1.dev20230524/pyglove/core/typing/class_schema_utils.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/typing/class_schema_utils_test.py` & `pyglove-0.3.1.dev20230524/pyglove/core/typing/class_schema_utils_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/typing/custom_typing.py` & `pyglove-0.3.1.dev20230524/pyglove/core/typing/custom_typing.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/typing/key_specs.py` & `pyglove-0.3.1.dev20230524/pyglove/core/typing/key_specs.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/typing/key_specs_test.py` & `pyglove-0.3.1.dev20230524/pyglove/core/typing/key_specs_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/typing/pytype_support.py` & `pyglove-0.3.1.dev20230524/pyglove/core/typing/pytype_support.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/typing/type_conversion.py` & `pyglove-0.3.1.dev20230524/pyglove/core/typing/type_conversion.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/typing/type_conversion_test.py` & `pyglove-0.3.1.dev20230524/pyglove/core/typing/type_conversion_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/typing/typed_missing.py` & `pyglove-0.3.1.dev20230524/pyglove/core/typing/typed_missing.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/typing/typed_missing_test.py` & `pyglove-0.3.1.dev20230524/pyglove/core/typing/typed_missing_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/typing/value_specs.py` & `pyglove-0.3.1.dev20230524/pyglove/core/typing/value_specs.py`

 * *Files 0% similar despite different names*

```diff
@@ -840,18 +840,21 @@
     # available.
     set_item = getattr(value, '_set_item_without_permission_check', None)
     if set_item is None:
       def _fn(i, v):
         value[i] = v
       set_item = _fn
 
+    # NOTE(daiyip): list elements can be contextual values, thus we try
+    # to get their symbolic form instead of the evaluated form.
+    getitem = getattr(value, 'sym_getattr', value.__getitem__)
     for i, v in enumerate(value):
       v = self._element.apply(v, allow_partial, child_transform,
                               object_utils.KeyPath(i, root_path))
-      if value[i] is not v:
+      if getitem(i) is not v:
         set_item(i, v)
     return value
 
   def _validate(
       self, path: object_utils.KeyPath, value: typing.List[typing.Any]):
     """Validates applied value."""
     if len(value) < self.min_size:
```

### Comparing `pyglove-0.3.1.dev20230523/pyglove/core/typing/value_specs_test.py` & `pyglove-0.3.1.dev20230524/pyglove/core/typing/value_specs_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/ext/__init__.py` & `pyglove-0.3.1.dev20230524/pyglove/ext/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/ext/early_stopping/__init__.py` & `pyglove-0.3.1.dev20230524/pyglove/ext/early_stopping/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/ext/early_stopping/base.py` & `pyglove-0.3.1.dev20230524/pyglove/ext/early_stopping/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/ext/early_stopping/base_test.py` & `pyglove-0.3.1.dev20230524/pyglove/ext/early_stopping/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/ext/early_stopping/step_wise.py` & `pyglove-0.3.1.dev20230524/pyglove/ext/early_stopping/step_wise.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/ext/early_stopping/step_wise_test.py` & `pyglove-0.3.1.dev20230524/pyglove/ext/early_stopping/step_wise_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/ext/evolution/__init__.py` & `pyglove-0.3.1.dev20230524/pyglove/ext/evolution/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/ext/evolution/base.py` & `pyglove-0.3.1.dev20230524/pyglove/ext/evolution/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/ext/evolution/base_test.py` & `pyglove-0.3.1.dev20230524/pyglove/ext/evolution/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/ext/evolution/hill_climb.py` & `pyglove-0.3.1.dev20230524/pyglove/ext/evolution/hill_climb.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/ext/evolution/hill_climb_test.py` & `pyglove-0.3.1.dev20230524/pyglove/ext/evolution/hill_climb_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/ext/evolution/mutators.py` & `pyglove-0.3.1.dev20230524/pyglove/ext/evolution/mutators.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/ext/evolution/mutators_test.py` & `pyglove-0.3.1.dev20230524/pyglove/ext/evolution/mutators_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/ext/evolution/neat.py` & `pyglove-0.3.1.dev20230524/pyglove/ext/evolution/neat.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/ext/evolution/neat_test.py` & `pyglove-0.3.1.dev20230524/pyglove/ext/evolution/neat_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/ext/evolution/nsga2.py` & `pyglove-0.3.1.dev20230524/pyglove/ext/evolution/nsga2.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/ext/evolution/nsga2_test.py` & `pyglove-0.3.1.dev20230524/pyglove/ext/evolution/nsga2_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/ext/evolution/recombinators.py` & `pyglove-0.3.1.dev20230524/pyglove/ext/evolution/recombinators.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/ext/evolution/recombinators_test.py` & `pyglove-0.3.1.dev20230524/pyglove/ext/evolution/recombinators_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/ext/evolution/regularized_evolution.py` & `pyglove-0.3.1.dev20230524/pyglove/ext/evolution/regularized_evolution.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/ext/evolution/regularized_evolution_test.py` & `pyglove-0.3.1.dev20230524/pyglove/ext/evolution/regularized_evolution_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/ext/evolution/selectors.py` & `pyglove-0.3.1.dev20230524/pyglove/ext/evolution/selectors.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/ext/evolution/selectors_test.py` & `pyglove-0.3.1.dev20230524/pyglove/ext/evolution/selectors_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/ext/evolution/where.py` & `pyglove-0.3.1.dev20230524/pyglove/ext/evolution/where.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/ext/evolution/where_test.py` & `pyglove-0.3.1.dev20230524/pyglove/ext/evolution/where_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/ext/mutfun/__init__.py` & `pyglove-0.3.1.dev20230524/pyglove/ext/mutfun/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/ext/mutfun/base.py` & `pyglove-0.3.1.dev20230524/pyglove/ext/mutfun/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/ext/mutfun/base_test.py` & `pyglove-0.3.1.dev20230524/pyglove/ext/mutfun/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/ext/mutfun/basic_ops.py` & `pyglove-0.3.1.dev20230524/pyglove/ext/mutfun/basic_ops.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/ext/mutfun/basic_ops_test.py` & `pyglove-0.3.1.dev20230524/pyglove/ext/mutfun/basic_ops_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/ext/scalars/__init__.py` & `pyglove-0.3.1.dev20230524/pyglove/ext/scalars/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/ext/scalars/base.py` & `pyglove-0.3.1.dev20230524/pyglove/ext/scalars/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/ext/scalars/base_test.py` & `pyglove-0.3.1.dev20230524/pyglove/ext/scalars/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/ext/scalars/maths.py` & `pyglove-0.3.1.dev20230524/pyglove/ext/scalars/maths.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/ext/scalars/maths_test.py` & `pyglove-0.3.1.dev20230524/pyglove/ext/scalars/maths_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/ext/scalars/randoms.py` & `pyglove-0.3.1.dev20230524/pyglove/ext/scalars/randoms.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/ext/scalars/randoms_test.py` & `pyglove-0.3.1.dev20230524/pyglove/ext/scalars/randoms_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/ext/scalars/step_wise.py` & `pyglove-0.3.1.dev20230524/pyglove/ext/scalars/step_wise.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove/ext/scalars/step_wise_test.py` & `pyglove-0.3.1.dev20230524/pyglove/ext/scalars/step_wise_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/pyglove.egg-info/PKG-INFO` & `pyglove-0.3.1.dev20230524/pyglove.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyglove
-Version: 0.3.1.dev20230523
+Version: 0.3.1.dev20230524
 Summary: PyGlove: A library for manipulating Python objects.
 Home-page: https://github.com/google/pyglove
 Author: PyGlove Authors
 Author-email: pyglove-authors@google.com
 License: Apache License 2.0
 Keywords: ai machine learning automl mutable symbolic framework meta-programming
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyglove-0.3.1.dev20230523/pyglove.egg-info/SOURCES.txt` & `pyglove-0.3.1.dev20230524/pyglove.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230523/setup.py` & `pyglove-0.3.1.dev20230524/setup.py`

 * *Files identical despite different names*

