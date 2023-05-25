# Comparing `tmp/bentoml_core-0.1.0.tar.gz` & `tmp/bentoml_core-1.0.20.dev0.tar.gz`

## Comparing `bentoml_core-0.1.0.tar` & `bentoml_core-1.0.20.dev0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      341 1970-01-01 00:00:00.000000 bentoml_core-0.1.0/Cargo.toml
--rw-r--r--   0     1000      984     2808 2023-05-11 00:55:11.000000 bentoml_core-0.1.0/.github/workflows/CI.yml
--rw-r--r--   0     1000      984      685 2023-05-11 00:55:11.000000 bentoml_core-0.1.0/.gitignore
--rw-r--r--   0     1000      984    11347 2023-05-11 00:55:59.000000 bentoml_core-0.1.0/LICENSE
--rw-r--r--   0     1000      984      499 2023-05-11 01:07:42.000000 bentoml_core-0.1.0/README.md
--rw-r--r--   0     1000      984        0 2023-05-11 05:00:53.000000 bentoml_core-0.1.0/bentoml_core.pyi
--rw-r--r--   0     1000      984     1456 2023-05-11 00:58:15.000000 bentoml_core-0.1.0/pyproject.toml
--rw-r--r--   0     1000      984       17 2023-05-11 01:25:06.000000 bentoml_core-0.1.0/rustfmt.toml
--rw-r--r--   0     1000      984      921 2023-05-23 07:11:16.000000 bentoml_core-0.1.0/src/bentos.rs
--rw-r--r--   0     1000      984      496 2023-05-23 00:10:03.000000 bentoml_core-0.1.0/src/exceptions.rs
--rw-r--r--   0     1000      984      595 2023-05-23 00:33:51.000000 bentoml_core-0.1.0/src/lib.rs
--rw-r--r--   0     1000      984     3326 2023-05-23 01:34:22.000000 bentoml_core-0.1.0/src/tag.rs
--rw-r--r--   0     1000      984    13029 2023-05-23 07:20:21.000000 bentoml_core-0.1.0/Cargo.lock
--rw-r--r--   0        0        0     1859 1970-01-01 00:00:00.000000 bentoml_core-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      469 1970-01-01 00:00:00.000000 bentoml_core-1.0.20.dev0/Cargo.toml
+-rw-r--r--   0      501       20     2808 2023-05-25 00:20:27.000000 bentoml_core-1.0.20.dev0/.github/workflows/CI.yml
+-rw-r--r--   0      501       20      685 2023-05-25 00:20:27.000000 bentoml_core-1.0.20.dev0/.gitignore
+-rw-r--r--   0      501       20    11347 2023-05-25 00:20:27.000000 bentoml_core-1.0.20.dev0/LICENSE
+-rw-r--r--   0      501       20      499 2023-05-25 00:20:27.000000 bentoml_core-1.0.20.dev0/README.md
+-rw-r--r--   0      501       20      537 2023-05-25 00:20:27.000000 bentoml_core-1.0.20.dev0/bentoml_core.pyi
+-rw-r--r--   0      501       20     1454 2023-05-25 00:20:27.000000 bentoml_core-1.0.20.dev0/pyproject.toml
+-rw-r--r--   0      501       20       17 2023-05-25 00:20:27.000000 bentoml_core-1.0.20.dev0/rustfmt.toml
+-rw-r--r--   0      501       20      875 2023-05-25 00:20:27.000000 bentoml_core-1.0.20.dev0/src/bentos.rs
+-rw-r--r--   0      501       20      430 2023-05-25 00:20:27.000000 bentoml_core-1.0.20.dev0/src/exceptions.rs
+-rw-r--r--   0      501       20      666 2023-05-25 00:20:27.000000 bentoml_core-1.0.20.dev0/src/lib.rs
+-rw-r--r--   0      501       20     3967 2023-05-25 00:20:27.000000 bentoml_core-1.0.20.dev0/src/tag.rs
+-rw-r--r--   0      501       20    16493 2023-05-25 00:25:30.000000 bentoml_core-1.0.20.dev0/Cargo.lock
+-rw-r--r--   0        0        0     1865 1970-01-01 00:00:00.000000 bentoml_core-1.0.20.dev0/PKG-INFO
```

### Comparing `bentoml_core-0.1.0/.github/workflows/CI.yml` & `bentoml_core-1.0.20.dev0/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `bentoml_core-0.1.0/.gitignore` & `bentoml_core-1.0.20.dev0/.gitignore`

 * *Files identical despite different names*

### Comparing `bentoml_core-0.1.0/LICENSE` & `bentoml_core-1.0.20.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `bentoml_core-0.1.0/pyproject.toml` & `bentoml_core-1.0.20.dev0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["maturin>=0.15,<0.16"]
+requires = ["maturin>=1.0,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "bentoml-core"
 description = "The rust core of BentoML: The Unified Model Serving Framework"
 readme = { file = "README.md", content-type = "text/markdown" }
 requires-python = ">=3.7"
```

### Comparing `bentoml_core-0.1.0/src/bentos.rs` & `bentoml_core-1.0.20.dev0/src/bentos.rs`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,40 @@
 use std::{fs::File, time::Duration};
 
 use pyo3::prelude::*;
-use zstd;
 use tar;
+use zstd;
 
-fn handle_py_signals<T: Send + 'static, E: Send + 'static, F: FnMut() -> Result<T, E> + Send + 'static>(py: Python<'_>, f: F) -> PyResult<T> where PyErr: From<E> {
-    let thread = std::thread::spawn(f);
-    loop {
-        py.check_signals()?;
-        if thread.is_finished() {
-            return Ok(thread.join().unwrap()?);
-        }
-        std::thread::sleep(Duration::from_millis(500));
-    }
+fn handle_py_signals<
+	T: Send + 'static,
+	E: Send + 'static,
+	F: FnMut() -> Result<T, E> + Send + 'static,
+>(
+	py: Python<'_>,
+	f: F,
+) -> PyResult<T>
+where
+	PyErr: From<E>,
+{
+	let thread = std::thread::spawn(f);
+	loop {
+		py.check_signals()?;
+		if thread.is_finished() {
+			return Ok(thread.join().unwrap()?);
+		}
+		std::thread::sleep(Duration::from_millis(500));
+	}
 }
 
 // TODO: convert this to take tag once bento is moved to rust.
 #[pyfunction]
 pub fn pack_bento(py: Python<'_>, path: &str, name: &str) -> PyResult<String> {
-    let out_path = format!("{}.bento", name);
-    let out_file = File::create(&out_path)?;
+	let out_path = format!("{}.bento", name);
+	let out_file = File::create(&out_path)?;
 
-    let mut tar = tar::Builder::new(zstd::Encoder::new(out_file, 3)?);
+	let mut tar = tar::Builder::new(zstd::Encoder::new(out_file, 3)?);
 
-    let path = path.to_string();
-    handle_py_signals(py, move || tar.append_dir_all("", &path))?;
+	let path = path.to_string();
+	handle_py_signals(py, move || tar.append_dir_all("", &path))?;
 
-    Ok(out_path)
-}
+	Ok(out_path)
+}
```

### Comparing `bentoml_core-0.1.0/src/lib.rs` & `bentoml_core-1.0.20.dev0/src/lib.rs`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,25 @@
-mod tag;
-mod exceptions;
 mod bentos;
+mod exceptions;
+mod tag;
 
 use pyo3::prelude::*;
 
 pub const BENTOML_VERSION: &str = env!("CARGO_PKG_VERSION");
 
 #[pymodule]
 fn bentoml_core(py: Python, m: &PyModule) -> PyResult<()> {
 	m.add_class::<tag::Tag>()?;
+	m.add_function(wrap_pyfunction!(tag::validate_tag_str, m)?)?;
 
 	let exceptions_module = PyModule::new(py, "exceptions")?;
-	exceptions_module.add("BentoMLException", py.get_type::<exceptions::BentoMLException>())?;
+	exceptions_module.add(
+		"BentoMLException",
+		py.get_type::<exceptions::BentoMLException>(),
+	)?;
 	m.add_submodule(exceptions_module)?;
 
 	let bentos_module = PyModule::new(py, "bentos")?;
 	bentos_module.add_function(wrap_pyfunction!(bentos::pack_bento, bentos_module)?)?;
 	m.add_submodule(bentos_module)?;
 
 	Ok(())
```

### Comparing `bentoml_core-0.1.0/Cargo.lock` & `bentoml_core-1.0.20.dev0/Cargo.lock`

 * *Files 15% similar despite different names*

```diff
@@ -8,27 +8,37 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "67fc08ce920c31afb70f013dcce1bfc3a3195de6a228474e45e1f145b36f8d04"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
+name = "atomic"
+version = "0.5.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c59bdb34bc650a32731b31bd8f0829cc15d24a708ee31559e0bb34f2bc320cba"
+
+[[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
 name = "bentoml-core"
-version = "0.1.0"
+version = "1.0.20-dev"
 dependencies = [
+ "data-encoding",
  "lazy_static",
+ "mac_address",
  "pyo3",
+ "rand",
  "regex",
  "tar",
+ "uuid",
  "zstd",
 ]
 
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -46,26 +56,43 @@
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
+name = "data-encoding"
+version = "2.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c2e66c9d817f1720209181c316d28635c050fa304f9c79e47a520882661b7308"
+
+[[package]]
 name = "filetime"
 version = "0.2.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5cbc844cecaee9d4443931972e1289c8ff485cb4cc2767cb03ca139ed6885153"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
+name = "getrandom"
+version = "0.2.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c85e1d9ab2eadba7e5040d4e09cbd6d072b76a557ad64e797c2cb9d4da21d7e4"
+dependencies = [
+ "cfg-if",
+ "libc",
+ "wasi",
+]
+
+[[package]]
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "jobserver"
@@ -95,29 +122,61 @@
 checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
+name = "mac_address"
+version = "1.1.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b238e3235c8382b7653c6408ed1b08dd379bdb9fdf990fb0bbae3db2cc0ae963"
+dependencies = [
+ "nix",
+ "winapi",
+]
+
+[[package]]
 name = "memchr"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
 
 [[package]]
 name = "memoffset"
+version = "0.6.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5aa361d4faea93603064a027415f07bd8e1d5c88c9fbf68bf56a285428fd79ce"
+dependencies = [
+ "autocfg",
+]
+
+[[package]]
+name = "memoffset"
 version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
+name = "nix"
+version = "0.23.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8f3790c00a0150112de0f4cd161e3d7fc4b2d8a5542ffc35f099a2562aecb35c"
+dependencies = [
+ "bitflags",
+ "cc",
+ "cfg-if",
+ "libc",
+ "memoffset 0.6.5",
+]
+
+[[package]]
 name = "once_cell"
 version = "1.17.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
 
 [[package]]
 name = "parking_lot"
@@ -145,14 +204,20 @@
 [[package]]
 name = "pkg-config"
 version = "0.3.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "26072860ba924cbfa98ea39c8c19b4dd6a4a25423dbdf219c1eca91aa0cf6964"
 
 [[package]]
+name = "ppv-lite86"
+version = "0.2.17"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
+
+[[package]]
 name = "proc-macro2"
 version = "1.0.56"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
 dependencies = [
  "unicode-ident",
 ]
@@ -162,15 +227,15 @@
 version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
- "memoffset",
+ "memoffset 0.8.0",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
@@ -223,14 +288,44 @@
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
+ "libc",
+ "rand_chacha",
+ "rand_core",
+]
+
+[[package]]
+name = "rand_chacha"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e6c10a63a0fa32252be49d21e7709d4d4baf8d231c2dbce1eaa8141b9b127d88"
+dependencies = [
+ "ppv-lite86",
+ "rand_core",
+]
+
+[[package]]
+name = "rand_core"
+version = "0.6.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ec0be4795e2f6a28069bec0b5ff3e2ac9bafc99e6a9a7dc3547996c5c816922c"
+dependencies = [
+ "getrandom",
+]
+
+[[package]]
 name = "redox_syscall"
 version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags",
 ]
@@ -301,14 +396,52 @@
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
+name = "uuid"
+version = "1.3.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "345444e32442451b267fc254ae85a209c64be56d2890e601a0c37ff0c3c5ecd2"
+dependencies = [
+ "atomic",
+ "getrandom",
+]
+
+[[package]]
+name = "wasi"
+version = "0.11.0+wasi-snapshot-preview1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
+
+[[package]]
+name = "winapi"
+version = "0.3.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
+dependencies = [
+ "winapi-i686-pc-windows-gnu",
+ "winapi-x86_64-pc-windows-gnu",
+]
+
+[[package]]
+name = "winapi-i686-pc-windows-gnu"
+version = "0.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ac3b87c63620426dd9b991e5ce0329eff545bccbbb34f3be09ff6fb6ab51b7b6"
+
+[[package]]
+name = "winapi-x86_64-pc-windows-gnu"
+version = "0.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
+
+[[package]]
 name = "windows-sys"
 version = "0.45.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
 dependencies = [
  "windows-targets 0.42.2",
 ]
```

### Comparing `bentoml_core-0.1.0/PKG-INFO` & `bentoml_core-1.0.20.dev0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bentoml-core
-Version: 0.1.0
+Version: 1.0.20.dev0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

