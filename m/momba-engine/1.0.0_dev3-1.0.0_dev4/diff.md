# Comparing `tmp/momba_engine-1.0.0_dev3.tar.gz` & `tmp/momba_engine-1.0.0_dev4.tar.gz`

## Comparing `momba_engine-1.0.0_dev3.tar` & `momba_engine-1.0.0_dev4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      730 1970-01-01 00:00:00.000000 momba_engine-1.0.0_dev3/local_dependencies/momba-explore/Cargo.toml
--rw-r--r--   0     1001      121      210 2021-02-26 13:00:39.000000 momba_engine-1.0.0_dev3/local_dependencies/momba-explore/README.md
--rw-r--r--   0     1001      121     3464 2021-02-26 13:00:39.000000 momba_engine-1.0.0_dev3/local_dependencies/momba-explore/src/explore/actions.rs
--rw-r--r--   0     1001      121    18192 2021-02-26 13:00:39.000000 momba_engine-1.0.0_dev3/local_dependencies/momba-explore/src/explore/compiled.rs
--rw-r--r--   0     1001      121    16393 2021-02-26 13:00:39.000000 momba_engine-1.0.0_dev3/local_dependencies/momba-explore/src/explore/evaluate.rs
--rw-r--r--   0     1001      121      963 2021-02-26 13:00:39.000000 momba_engine-1.0.0_dev3/local_dependencies/momba-explore/src/explore/external.rs
--rw-r--r--   0     1001      121    17937 2021-02-26 13:00:39.000000 momba_engine-1.0.0_dev3/local_dependencies/momba-explore/src/explore/mod.rs
--rw-r--r--   0     1001      121      713 2021-02-26 13:00:39.000000 momba_engine-1.0.0_dev3/local_dependencies/momba-explore/src/lib.rs
--rw-r--r--   0     1001      121     1623 2021-02-26 13:00:39.000000 momba_engine-1.0.0_dev3/local_dependencies/momba-explore/src/model/actions.rs
--rw-r--r--   0     1001      121     3778 2021-02-26 13:00:39.000000 momba_engine-1.0.0_dev3/local_dependencies/momba-explore/src/model/expressions.rs
--rw-r--r--   0     1001      121      265 2021-02-26 13:00:39.000000 momba_engine-1.0.0_dev3/local_dependencies/momba-explore/src/model/mod.rs
--rw-r--r--   0     1001      121     4243 2021-02-26 13:00:39.000000 momba_engine-1.0.0_dev3/local_dependencies/momba-explore/src/model/network.rs
--rw-r--r--   0     1001      121      691 2021-02-26 13:00:39.000000 momba_engine-1.0.0_dev3/local_dependencies/momba-explore/src/model/references.rs
--rw-r--r--   0     1001      121      606 2021-02-26 13:00:39.000000 momba_engine-1.0.0_dev3/local_dependencies/momba-explore/src/model/types.rs
--rw-r--r--   0     1001      121    12752 2021-02-26 13:00:39.000000 momba_engine-1.0.0_dev3/local_dependencies/momba-explore/src/model/values.rs
--rw-r--r--   0     1001      121     3249 2021-02-26 13:00:39.000000 momba_engine-1.0.0_dev3/local_dependencies/momba-explore/src/simulate/mod.rs
--rw-r--r--   0     1001      121    13230 2021-02-26 13:00:39.000000 momba_engine-1.0.0_dev3/local_dependencies/momba-explore/src/time.rs
--rw-r--r--   0        0        0      474 1970-01-01 00:00:00.000000 momba_engine-1.0.0_dev3/local_dependencies/clock-zones/Cargo.toml
--rw-r--r--   0     1001      121     1074 2021-02-26 13:00:39.000000 momba_engine-1.0.0_dev3/local_dependencies/clock-zones/README.md
--rw-r--r--   0     1001      121    10638 2021-02-26 13:00:39.000000 momba_engine-1.0.0_dev3/local_dependencies/clock-zones/src/bounds.rs
--rw-r--r--   0     1001      121     2760 2021-02-26 13:00:39.000000 momba_engine-1.0.0_dev3/local_dependencies/clock-zones/src/constants.rs
--rw-r--r--   0     1001      121     2038 2021-02-26 13:00:39.000000 momba_engine-1.0.0_dev3/local_dependencies/clock-zones/src/lib.rs
--rw-r--r--   0     1001      121     2243 2021-02-26 13:00:39.000000 momba_engine-1.0.0_dev3/local_dependencies/clock-zones/src/storage.rs
--rw-r--r--   0     1001      121    13929 2021-02-26 13:00:39.000000 momba_engine-1.0.0_dev3/local_dependencies/clock-zones/src/zones.rs
--rw-r--r--   0        0        0      596 1970-01-01 00:00:00.000000 momba_engine-1.0.0_dev3/Cargo.toml
--rw-r--r--   0     1001      121       24 2021-02-26 13:00:39.000000 momba_engine-1.0.0_dev3/.gitignore
--rw-r--r--   0     1001      121      733 2021-02-26 13:00:39.000000 momba_engine-1.0.0_dev3/README.md
--rw-r--r--   0     1001      121      781 2021-02-26 13:00:39.000000 momba_engine-1.0.0_dev3/crates/README.md
--rw-r--r--   0     1001      121       64 2021-02-26 13:00:39.000000 momba_engine-1.0.0_dev3/pyproject.toml
--rw-r--r--   0     1001      121        7 2021-02-26 13:00:39.000000 momba_engine-1.0.0_dev3/rust-toolchain
--rw-r--r--   0     1001      121     7038 2021-02-26 13:00:39.000000 momba_engine-1.0.0_dev3/src/lib.rs
--rw-r--r--   0        0        0      259 1970-01-01 00:00:00.000000 momba_engine-1.0.0_dev3/PKG-INFO
+-rw-r--r--   0        0        0      474 1970-01-01 00:00:00.000000 momba_engine-1.0.0_dev4/local_dependencies/clock-zones/Cargo.toml
+-rw-r--r--   0     1001      121     1074 2021-02-26 15:00:21.000000 momba_engine-1.0.0_dev4/local_dependencies/clock-zones/README.md
+-rw-r--r--   0     1001      121    10638 2021-02-26 15:00:21.000000 momba_engine-1.0.0_dev4/local_dependencies/clock-zones/src/bounds.rs
+-rw-r--r--   0     1001      121     2760 2021-02-26 15:00:21.000000 momba_engine-1.0.0_dev4/local_dependencies/clock-zones/src/constants.rs
+-rw-r--r--   0     1001      121     2038 2021-02-26 15:00:21.000000 momba_engine-1.0.0_dev4/local_dependencies/clock-zones/src/lib.rs
+-rw-r--r--   0     1001      121     2243 2021-02-26 15:00:21.000000 momba_engine-1.0.0_dev4/local_dependencies/clock-zones/src/storage.rs
+-rw-r--r--   0     1001      121    13929 2021-02-26 15:00:21.000000 momba_engine-1.0.0_dev4/local_dependencies/clock-zones/src/zones.rs
+-rw-r--r--   0        0        0      730 1970-01-01 00:00:00.000000 momba_engine-1.0.0_dev4/local_dependencies/momba-explore/Cargo.toml
+-rw-r--r--   0     1001      121      210 2021-02-26 15:00:21.000000 momba_engine-1.0.0_dev4/local_dependencies/momba-explore/README.md
+-rw-r--r--   0     1001      121     3464 2021-02-26 15:00:21.000000 momba_engine-1.0.0_dev4/local_dependencies/momba-explore/src/explore/actions.rs
+-rw-r--r--   0     1001      121    18192 2021-02-26 15:00:21.000000 momba_engine-1.0.0_dev4/local_dependencies/momba-explore/src/explore/compiled.rs
+-rw-r--r--   0     1001      121    16393 2021-02-26 15:00:21.000000 momba_engine-1.0.0_dev4/local_dependencies/momba-explore/src/explore/evaluate.rs
+-rw-r--r--   0     1001      121      963 2021-02-26 15:00:21.000000 momba_engine-1.0.0_dev4/local_dependencies/momba-explore/src/explore/external.rs
+-rw-r--r--   0     1001      121    17937 2021-02-26 15:00:21.000000 momba_engine-1.0.0_dev4/local_dependencies/momba-explore/src/explore/mod.rs
+-rw-r--r--   0     1001      121      713 2021-02-26 15:00:21.000000 momba_engine-1.0.0_dev4/local_dependencies/momba-explore/src/lib.rs
+-rw-r--r--   0     1001      121     1623 2021-02-26 15:00:21.000000 momba_engine-1.0.0_dev4/local_dependencies/momba-explore/src/model/actions.rs
+-rw-r--r--   0     1001      121     3778 2021-02-26 15:00:21.000000 momba_engine-1.0.0_dev4/local_dependencies/momba-explore/src/model/expressions.rs
+-rw-r--r--   0     1001      121      265 2021-02-26 15:00:21.000000 momba_engine-1.0.0_dev4/local_dependencies/momba-explore/src/model/mod.rs
+-rw-r--r--   0     1001      121     4243 2021-02-26 15:00:21.000000 momba_engine-1.0.0_dev4/local_dependencies/momba-explore/src/model/network.rs
+-rw-r--r--   0     1001      121      691 2021-02-26 15:00:21.000000 momba_engine-1.0.0_dev4/local_dependencies/momba-explore/src/model/references.rs
+-rw-r--r--   0     1001      121      606 2021-02-26 15:00:21.000000 momba_engine-1.0.0_dev4/local_dependencies/momba-explore/src/model/types.rs
+-rw-r--r--   0     1001      121    12752 2021-02-26 15:00:21.000000 momba_engine-1.0.0_dev4/local_dependencies/momba-explore/src/model/values.rs
+-rw-r--r--   0     1001      121     3249 2021-02-26 15:00:21.000000 momba_engine-1.0.0_dev4/local_dependencies/momba-explore/src/simulate/mod.rs
+-rw-r--r--   0     1001      121    13230 2021-02-26 15:00:21.000000 momba_engine-1.0.0_dev4/local_dependencies/momba-explore/src/time.rs
+-rw-r--r--   0        0        0      596 1970-01-01 00:00:00.000000 momba_engine-1.0.0_dev4/Cargo.toml
+-rw-r--r--   0     1001      121       24 2021-02-26 15:00:21.000000 momba_engine-1.0.0_dev4/.gitignore
+-rw-r--r--   0     1001      121      733 2021-02-26 15:00:21.000000 momba_engine-1.0.0_dev4/README.md
+-rw-r--r--   0     1001      121      781 2021-02-26 15:00:21.000000 momba_engine-1.0.0_dev4/crates/README.md
+-rw-r--r--   0     1001      121       64 2021-02-26 15:00:21.000000 momba_engine-1.0.0_dev4/pyproject.toml
+-rw-r--r--   0     1001      121        7 2021-02-26 15:00:21.000000 momba_engine-1.0.0_dev4/rust-toolchain
+-rw-r--r--   0     1001      121     7038 2021-02-26 15:00:21.000000 momba_engine-1.0.0_dev4/src/lib.rs
+-rw-r--r--   0        0        0      259 1970-01-01 00:00:00.000000 momba_engine-1.0.0_dev4/PKG-INFO
```

### Comparing `momba_engine-1.0.0_dev3/local_dependencies/momba-explore/Cargo.toml` & `momba_engine-1.0.0_dev4/local_dependencies/momba-explore/Cargo.toml`

 * *Files identical despite different names*

### Comparing `momba_engine-1.0.0_dev3/local_dependencies/momba-explore/src/explore/actions.rs` & `momba_engine-1.0.0_dev4/local_dependencies/momba-explore/src/explore/actions.rs`

 * *Files identical despite different names*

### Comparing `momba_engine-1.0.0_dev3/local_dependencies/momba-explore/src/explore/compiled.rs` & `momba_engine-1.0.0_dev4/local_dependencies/momba-explore/src/explore/compiled.rs`

 * *Files identical despite different names*

### Comparing `momba_engine-1.0.0_dev3/local_dependencies/momba-explore/src/explore/evaluate.rs` & `momba_engine-1.0.0_dev4/local_dependencies/momba-explore/src/explore/evaluate.rs`

 * *Files identical despite different names*

### Comparing `momba_engine-1.0.0_dev3/local_dependencies/momba-explore/src/explore/external.rs` & `momba_engine-1.0.0_dev4/local_dependencies/momba-explore/src/explore/external.rs`

 * *Files identical despite different names*

### Comparing `momba_engine-1.0.0_dev3/local_dependencies/momba-explore/src/explore/mod.rs` & `momba_engine-1.0.0_dev4/local_dependencies/momba-explore/src/explore/mod.rs`

 * *Files identical despite different names*

### Comparing `momba_engine-1.0.0_dev3/local_dependencies/momba-explore/src/lib.rs` & `momba_engine-1.0.0_dev4/local_dependencies/momba-explore/src/lib.rs`

 * *Files identical despite different names*

### Comparing `momba_engine-1.0.0_dev3/local_dependencies/momba-explore/src/model/actions.rs` & `momba_engine-1.0.0_dev4/local_dependencies/momba-explore/src/model/actions.rs`

 * *Files identical despite different names*

### Comparing `momba_engine-1.0.0_dev3/local_dependencies/momba-explore/src/model/expressions.rs` & `momba_engine-1.0.0_dev4/local_dependencies/momba-explore/src/model/expressions.rs`

 * *Files identical despite different names*

### Comparing `momba_engine-1.0.0_dev3/local_dependencies/momba-explore/src/model/network.rs` & `momba_engine-1.0.0_dev4/local_dependencies/momba-explore/src/model/network.rs`

 * *Files identical despite different names*

### Comparing `momba_engine-1.0.0_dev3/local_dependencies/momba-explore/src/model/references.rs` & `momba_engine-1.0.0_dev4/local_dependencies/momba-explore/src/model/references.rs`

 * *Files identical despite different names*

### Comparing `momba_engine-1.0.0_dev3/local_dependencies/momba-explore/src/model/types.rs` & `momba_engine-1.0.0_dev4/local_dependencies/momba-explore/src/model/types.rs`

 * *Files identical despite different names*

### Comparing `momba_engine-1.0.0_dev3/local_dependencies/momba-explore/src/model/values.rs` & `momba_engine-1.0.0_dev4/local_dependencies/momba-explore/src/model/values.rs`

 * *Files identical despite different names*

### Comparing `momba_engine-1.0.0_dev3/local_dependencies/momba-explore/src/simulate/mod.rs` & `momba_engine-1.0.0_dev4/local_dependencies/momba-explore/src/simulate/mod.rs`

 * *Files identical despite different names*

### Comparing `momba_engine-1.0.0_dev3/local_dependencies/momba-explore/src/time.rs` & `momba_engine-1.0.0_dev4/local_dependencies/momba-explore/src/time.rs`

 * *Files identical despite different names*

### Comparing `momba_engine-1.0.0_dev3/local_dependencies/clock-zones/README.md` & `momba_engine-1.0.0_dev4/local_dependencies/clock-zones/README.md`

 * *Files identical despite different names*

### Comparing `momba_engine-1.0.0_dev3/local_dependencies/clock-zones/src/bounds.rs` & `momba_engine-1.0.0_dev4/local_dependencies/clock-zones/src/bounds.rs`

 * *Files identical despite different names*

### Comparing `momba_engine-1.0.0_dev3/local_dependencies/clock-zones/src/constants.rs` & `momba_engine-1.0.0_dev4/local_dependencies/clock-zones/src/constants.rs`

 * *Files identical despite different names*

### Comparing `momba_engine-1.0.0_dev3/local_dependencies/clock-zones/src/lib.rs` & `momba_engine-1.0.0_dev4/local_dependencies/clock-zones/src/lib.rs`

 * *Files identical despite different names*

### Comparing `momba_engine-1.0.0_dev3/local_dependencies/clock-zones/src/storage.rs` & `momba_engine-1.0.0_dev4/local_dependencies/clock-zones/src/storage.rs`

 * *Files identical despite different names*

### Comparing `momba_engine-1.0.0_dev3/local_dependencies/clock-zones/src/zones.rs` & `momba_engine-1.0.0_dev4/local_dependencies/clock-zones/src/zones.rs`

 * *Files identical despite different names*

### Comparing `momba_engine-1.0.0_dev3/Cargo.toml` & `momba_engine-1.0.0_dev4/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "momba_engine"
-version = "1.0.0-dev3"
+version = "1.0.0-dev4"
 authors = ["Maximilian Köhl <koehl@cs.uni-saarland.de>"]
 edition = "2018"
 description = "A Python package supercharging Momba with computing capabilities."
 repository = "https://github.com/koehlma/momba"
 license = "MIT"
 categories = ["algorithms", "data-structures", "science"]
 publish = false
```

### Comparing `momba_engine-1.0.0_dev3/README.md` & `momba_engine-1.0.0_dev4/README.md`

 * *Files identical despite different names*

### Comparing `momba_engine-1.0.0_dev3/crates/README.md` & `momba_engine-1.0.0_dev4/crates/README.md`

 * *Files identical despite different names*

### Comparing `momba_engine-1.0.0_dev3/src/lib.rs` & `momba_engine-1.0.0_dev4/src/lib.rs`

 * *Files identical despite different names*

