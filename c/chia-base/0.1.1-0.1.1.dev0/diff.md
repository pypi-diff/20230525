# Comparing `tmp/chia_base-0.1.1.tar.gz` & `tmp/chia_base-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chia_base-0.1.1.tar", last modified: Thu May 25 21:37:35 2023, max compression
+gzip compressed data, was "chia_base-0.1.0.tar", last modified: Thu May 25 21:29:19 2023, max compression
```

## Comparing `chia_base-0.1.1.tar` & `chia_base-0.1.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      774 1985-10-26 08:20:00.000000 chia_base-0.1.1/PKG-INFO
--rw-r--r--   0        0        0      249 1985-10-26 08:20:00.000000 chia_base-0.1.1/README.md
--rw-r--r--   0        0        0     1096 1985-10-26 08:20:00.000000 chia_base-0.1.1/SConstruct
--rw-r--r--   0        0        0        0 1985-10-26 08:20:00.000000 chia_base-0.1.1/chia_base/__init__.py
--rw-r--r--   0        0        0      340 1985-10-26 08:20:00.000000 chia_base-0.1.1/chia_base/atoms/__init__.py
--rw-r--r--   0        0        0      320 1985-10-26 08:20:00.000000 chia_base-0.1.1/chia_base/atoms/hexbytes.py
--rw-r--r--   0        0        0      451 1985-10-26 08:20:00.000000 chia_base-0.1.1/chia_base/atoms/ints.py
--rw-r--r--   0        0        0      738 1985-10-26 08:20:00.000000 chia_base-0.1.1/chia_base/atoms/sized_bytes.py
--rw-r--r--   0        0        0      529 1985-10-26 08:20:00.000000 chia_base-0.1.1/chia_base/atoms/struct_stream.py
--rw-r--r--   0        0        0      198 1985-10-26 08:20:00.000000 chia_base-0.1.1/chia_base/bls12_381/__init__.py
--rw-r--r--   0        0        0     2785 1985-10-26 08:20:00.000000 chia_base-0.1.1/chia_base/bls12_381/bls_public_key.py
--rw-r--r--   0        0        0     3461 1985-10-26 08:20:00.000000 chia_base-0.1.1/chia_base/bls12_381/bls_secret_exponent.py
--rw-r--r--   0        0        0     1912 1985-10-26 08:20:00.000000 chia_base-0.1.1/chia_base/bls12_381/bls_signature.py
--rw-r--r--   0        0        0      438 1985-10-26 08:20:00.000000 chia_base-0.1.1/chia_base/bls12_381/secret_key_utils.py
--rw-r--r--   0        0        0        0 1985-10-26 08:20:00.000000 chia_base-0.1.1/chia_base/contrib/__init__.py
--rw-r--r--   0        0        0     5189 1985-10-26 08:20:00.000000 chia_base-0.1.1/chia_base/contrib/bech32m.py
--rw-r--r--   0        0        0      144 1985-10-26 08:20:00.000000 chia_base-0.1.1/chia_base/core/__init__.py
--rw-r--r--   0        0        0      495 1985-10-26 08:20:00.000000 chia_base-0.1.1/chia_base/core/coin.py
--rw-r--r--   0        0        0      319 1985-10-26 08:20:00.000000 chia_base-0.1.1/chia_base/core/coin_spend.py
--rw-r--r--   0        0        0        0 1985-10-26 08:20:00.000000 chia_base-0.1.1/chia_base/core/program.py
--rw-r--r--   0        0        0      861 1985-10-26 08:20:00.000000 chia_base-0.1.1/chia_base/core/spend_bundle.py
--rw-r--r--   0        0        0      195 1985-10-26 08:20:00.000000 chia_base-0.1.1/chia_base/core/std_hash.py
--rw-r--r--   0        0        0       61 1985-10-26 08:20:00.000000 chia_base-0.1.1/chia_base/meta/__init__.py
--rw-r--r--   0        0        0     1005 1985-10-26 08:20:00.000000 chia_base-0.1.1/chia_base/meta/make_parser.py
--rw-r--r--   0        0        0     2380 1985-10-26 08:20:00.000000 chia_base-0.1.1/chia_base/meta/make_streamer.py
--rw-r--r--   0        0        0     1282 1985-10-26 08:20:00.000000 chia_base-0.1.1/chia_base/meta/streamable.py
--rw-r--r--   0        0        0      334 1985-10-26 08:20:00.000000 chia_base-0.1.1/chia_base/meta/typing_helpers.py
--rw-r--r--   0        0        0        0 1985-10-26 08:20:00.000000 chia_base-0.1.1/chia_base/util/__init__.py
--rw-r--r--   0        0        0      751 1985-10-26 08:20:00.000000 chia_base-0.1.1/chia_base/util/bech32.py
--rw-r--r--   0        0        0      195 1985-10-26 08:20:00.000000 chia_base-0.1.1/chia_base/util/std_hash.py
--rw-r--r--   0        0        0      665 1985-10-26 08:20:00.000000 chia_base-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      779 1985-10-26 08:20:00.000000 chia_base-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      249 1985-10-26 08:20:00.000000 chia_base-0.1.0/README.md
+-rw-r--r--   0        0        0     1096 1985-10-26 08:20:00.000000 chia_base-0.1.0/SConstruct
+-rw-r--r--   0        0        0        0 1985-10-26 08:20:00.000000 chia_base-0.1.0/chia_base/__init__.py
+-rw-r--r--   0        0        0      340 1985-10-26 08:20:00.000000 chia_base-0.1.0/chia_base/atoms/__init__.py
+-rw-r--r--   0        0        0      320 1985-10-26 08:20:00.000000 chia_base-0.1.0/chia_base/atoms/hexbytes.py
+-rw-r--r--   0        0        0      451 1985-10-26 08:20:00.000000 chia_base-0.1.0/chia_base/atoms/ints.py
+-rw-r--r--   0        0        0      738 1985-10-26 08:20:00.000000 chia_base-0.1.0/chia_base/atoms/sized_bytes.py
+-rw-r--r--   0        0        0      529 1985-10-26 08:20:00.000000 chia_base-0.1.0/chia_base/atoms/struct_stream.py
+-rw-r--r--   0        0        0      198 1985-10-26 08:20:00.000000 chia_base-0.1.0/chia_base/bls12_381/__init__.py
+-rw-r--r--   0        0        0     2785 1985-10-26 08:20:00.000000 chia_base-0.1.0/chia_base/bls12_381/bls_public_key.py
+-rw-r--r--   0        0        0     3461 1985-10-26 08:20:00.000000 chia_base-0.1.0/chia_base/bls12_381/bls_secret_exponent.py
+-rw-r--r--   0        0        0     1912 1985-10-26 08:20:00.000000 chia_base-0.1.0/chia_base/bls12_381/bls_signature.py
+-rw-r--r--   0        0        0      438 1985-10-26 08:20:00.000000 chia_base-0.1.0/chia_base/bls12_381/secret_key_utils.py
+-rw-r--r--   0        0        0        0 1985-10-26 08:20:00.000000 chia_base-0.1.0/chia_base/contrib/__init__.py
+-rw-r--r--   0        0        0     5189 1985-10-26 08:20:00.000000 chia_base-0.1.0/chia_base/contrib/bech32m.py
+-rw-r--r--   0        0        0      144 1985-10-26 08:20:00.000000 chia_base-0.1.0/chia_base/core/__init__.py
+-rw-r--r--   0        0        0      495 1985-10-26 08:20:00.000000 chia_base-0.1.0/chia_base/core/coin.py
+-rw-r--r--   0        0        0      319 1985-10-26 08:20:00.000000 chia_base-0.1.0/chia_base/core/coin_spend.py
+-rw-r--r--   0        0        0        0 1985-10-26 08:20:00.000000 chia_base-0.1.0/chia_base/core/program.py
+-rw-r--r--   0        0        0      861 1985-10-26 08:20:00.000000 chia_base-0.1.0/chia_base/core/spend_bundle.py
+-rw-r--r--   0        0        0      195 1985-10-26 08:20:00.000000 chia_base-0.1.0/chia_base/core/std_hash.py
+-rw-r--r--   0        0        0       61 1985-10-26 08:20:00.000000 chia_base-0.1.0/chia_base/meta/__init__.py
+-rw-r--r--   0        0        0     1005 1985-10-26 08:20:00.000000 chia_base-0.1.0/chia_base/meta/make_parser.py
+-rw-r--r--   0        0        0     2380 1985-10-26 08:20:00.000000 chia_base-0.1.0/chia_base/meta/make_streamer.py
+-rw-r--r--   0        0        0     1282 1985-10-26 08:20:00.000000 chia_base-0.1.0/chia_base/meta/streamable.py
+-rw-r--r--   0        0        0      334 1985-10-26 08:20:00.000000 chia_base-0.1.0/chia_base/meta/typing_helpers.py
+-rw-r--r--   0        0        0        0 1985-10-26 08:20:00.000000 chia_base-0.1.0/chia_base/util/__init__.py
+-rw-r--r--   0        0        0      751 1985-10-26 08:20:00.000000 chia_base-0.1.0/chia_base/util/bech32.py
+-rw-r--r--   0        0        0      195 1985-10-26 08:20:00.000000 chia_base-0.1.0/chia_base/util/std_hash.py
+-rw-r--r--   0        0        0      665 1985-10-26 08:20:00.000000 chia_base-0.1.0/pyproject.toml
```

### Comparing `chia_base-0.1.1/PKG-INFO` & `chia_base-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chia_base
-Version: 0.1.1
+Version: 0.1.1.dev0
 Summary: Common types and simple utilities used through chia code base
 License: Apache-2.0
 Author: Richard Kiss
 Author-email: him@richardkiss.com
 Project-URL: Repository, https://github.com/richardkiss/chia_base.git
 Provides-Extra: dev
 Requires-Dist: ruff>=0.0.252; extra == 'dev'
```

### Comparing `chia_base-0.1.1/SConstruct` & `chia_base-0.1.0/SConstruct`

 * *Files identical despite different names*

### Comparing `chia_base-0.1.1/chia_base/atoms/sized_bytes.py` & `chia_base-0.1.0/chia_base/atoms/sized_bytes.py`

 * *Files identical despite different names*

### Comparing `chia_base-0.1.1/chia_base/atoms/struct_stream.py` & `chia_base-0.1.0/chia_base/atoms/struct_stream.py`

 * *Files identical despite different names*

### Comparing `chia_base-0.1.1/chia_base/bls12_381/bls_public_key.py` & `chia_base-0.1.0/chia_base/bls12_381/bls_public_key.py`

 * *Files identical despite different names*

### Comparing `chia_base-0.1.1/chia_base/bls12_381/bls_secret_exponent.py` & `chia_base-0.1.0/chia_base/bls12_381/bls_secret_exponent.py`

 * *Files identical despite different names*

### Comparing `chia_base-0.1.1/chia_base/bls12_381/bls_signature.py` & `chia_base-0.1.0/chia_base/bls12_381/bls_signature.py`

 * *Files identical despite different names*

### Comparing `chia_base-0.1.1/chia_base/contrib/bech32m.py` & `chia_base-0.1.0/chia_base/contrib/bech32m.py`

 * *Files identical despite different names*

### Comparing `chia_base-0.1.1/chia_base/core/spend_bundle.py` & `chia_base-0.1.0/chia_base/core/spend_bundle.py`

 * *Files identical despite different names*

### Comparing `chia_base-0.1.1/chia_base/meta/make_parser.py` & `chia_base-0.1.0/chia_base/meta/make_parser.py`

 * *Files identical despite different names*

### Comparing `chia_base-0.1.1/chia_base/meta/make_streamer.py` & `chia_base-0.1.0/chia_base/meta/make_streamer.py`

 * *Files identical despite different names*

### Comparing `chia_base-0.1.1/chia_base/meta/streamable.py` & `chia_base-0.1.0/chia_base/meta/streamable.py`

 * *Files identical despite different names*

### Comparing `chia_base-0.1.1/chia_base/util/bech32.py` & `chia_base-0.1.0/chia_base/util/bech32.py`

 * *Files identical despite different names*

### Comparing `chia_base-0.1.1/pyproject.toml` & `chia_base-0.1.0/pyproject.toml`

 * *Files identical despite different names*

