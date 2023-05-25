# Comparing `tmp/llm_rs-0.2.4.tar.gz` & `tmp/llm_rs-0.2.5.tar.gz`

## Comparing `llm_rs-0.2.4.tar` & `llm_rs-0.2.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0      468 1970-01-01 00:00:00.000000 llm_rs-0.2.4/Cargo.toml
--rw-r--r--   0     1001      123      610 2023-05-24 14:12:21.000000 llm_rs-0.2.4/.github/workflows/BuildDoc.yml
--rw-r--r--   0     1001      123     2796 2023-05-24 14:12:21.000000 llm_rs-0.2.4/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      564 2023-05-24 14:12:21.000000 llm_rs-0.2.4/.github/workflows/Clippy.yml
--rw-r--r--   0     1001      123      602 2023-05-24 14:12:21.000000 llm_rs-0.2.4/.github/workflows/PublishDocs.yml
--rw-r--r--   0     1001      123     3455 2023-05-24 14:12:21.000000 llm_rs-0.2.4/.gitignore
--rw-r--r--   0     1001      123       72 2023-05-24 14:12:21.000000 llm_rs-0.2.4/.vscode/settings.json
--rw-r--r--   0     1001      123     1071 2023-05-24 14:12:21.000000 llm_rs-0.2.4/LICENSE
--rw-r--r--   0     1001      123     3053 2023-05-24 14:12:21.000000 llm_rs-0.2.4/README.md
--rw-r--r--   0     1001      123     4799 2023-05-24 14:12:21.000000 llm_rs-0.2.4/docs/docs/conversion.md
--rw-r--r--   0     1001      123     9355 2023-05-24 14:12:21.000000 llm_rs-0.2.4/docs/docs/index.md
--rw-r--r--   0     1001      123     1181 2023-05-24 14:12:21.000000 llm_rs-0.2.4/docs/mkdocs.yml
--rw-r--r--   0     1001      123       31 2023-05-24 14:12:21.000000 llm_rs-0.2.4/docs/requirements.txt
--rw-r--r--   0     1001      123      334 2023-05-24 14:12:21.000000 llm_rs-0.2.4/llm_rs/__init__.py
--rw-r--r--   0     1001      123    14929 2023-05-24 14:12:21.000000 llm_rs-0.2.4/llm_rs/auto.py
--rw-r--r--   0     1001      123     1614 2023-05-24 14:12:21.000000 llm_rs-0.2.4/llm_rs/base_model.py
--rw-r--r--   0     1001      123     1351 2023-05-24 14:12:21.000000 llm_rs-0.2.4/llm_rs/config.pyi
--rw-r--r--   0     1001      123       78 2023-05-24 14:12:21.000000 llm_rs-0.2.4/llm_rs/convert/__init__.py
--rw-r--r--   0     1001      123     2223 2023-05-24 14:12:21.000000 llm_rs-0.2.4/llm_rs/convert/auto_converter.py
--rw-r--r--   0     1001      123      199 2023-05-24 14:12:21.000000 llm_rs-0.2.4/llm_rs/convert/models/__init__.py
--rw-r--r--   0     1001      123     5581 2023-05-24 14:12:21.000000 llm_rs-0.2.4/llm_rs/convert/models/_base.py
--rw-r--r--   0     1001      123     3177 2023-05-24 14:12:21.000000 llm_rs-0.2.4/llm_rs/convert/models/bloom.py
--rw-r--r--   0     1001      123     5221 2023-05-24 14:12:21.000000 llm_rs-0.2.4/llm_rs/convert/models/gpt2.py
--rw-r--r--   0     1001      123     2032 2023-05-24 14:12:21.000000 llm_rs-0.2.4/llm_rs/convert/models/gptj.py
--rw-r--r--   0     1001      123     2138 2023-05-24 14:12:21.000000 llm_rs-0.2.4/llm_rs/convert/models/gptneox.py
--rw-r--r--   0     1001      123     6334 2023-05-24 14:12:21.000000 llm_rs-0.2.4/llm_rs/convert/models/llama.py
--rw-r--r--   0     1001      123     1893 2023-05-24 14:12:21.000000 llm_rs-0.2.4/llm_rs/convert/models/mpt.py
--rw-r--r--   0     1001      123        0 2023-05-24 14:12:21.000000 llm_rs-0.2.4/llm_rs/llm_rs.pyi
--rw-r--r--   0     1001      123      579 2023-05-24 14:12:21.000000 llm_rs-0.2.4/llm_rs/models.pyi
--rw-r--r--   0     1001      123        0 2023-05-24 14:12:21.000000 llm_rs-0.2.4/llm_rs/py.typed
--rw-r--r--   0     1001      123     2915 2023-05-24 14:12:21.000000 llm_rs-0.2.4/llm_rs/repository.py
--rw-r--r--   0     1001      123      697 2023-05-24 14:12:21.000000 llm_rs-0.2.4/llm_rs/results.pyi
--rw-r--r--   0     1001      123      978 2023-05-24 14:12:21.000000 llm_rs-0.2.4/pyproject.toml
--rw-r--r--   0     1001      123     4274 2023-05-24 14:12:21.000000 llm_rs-0.2.4/src/configs.rs
--rw-r--r--   0     1001      123     1685 2023-05-24 14:12:21.000000 llm_rs-0.2.4/src/lib.rs
--rw-r--r--   0     1001      123     9658 2023-05-24 14:12:21.000000 llm_rs-0.2.4/src/model_base.rs
--rw-r--r--   0     1001      123      300 2023-05-24 14:12:21.000000 llm_rs-0.2.4/src/models.rs
--rw-r--r--   0     1001      123     2576 2023-05-24 14:12:21.000000 llm_rs-0.2.4/src/quantize.rs
--rw-r--r--   0     1001      123     1352 2023-05-24 14:12:21.000000 llm_rs-0.2.4/src/results.rs
--rw-r--r--   0     1001      123    14030 2023-05-24 14:13:58.000000 llm_rs-0.2.4/Cargo.lock
--rw-r--r--   0        0        0     4150 1970-01-01 00:00:00.000000 llm_rs-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      468 1970-01-01 00:00:00.000000 llm_rs-0.2.5/Cargo.toml
+-rw-r--r--   0     1001      123      610 2023-05-25 09:23:18.000000 llm_rs-0.2.5/.github/workflows/BuildDoc.yml
+-rw-r--r--   0     1001      123     2796 2023-05-25 09:23:18.000000 llm_rs-0.2.5/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      564 2023-05-25 09:23:18.000000 llm_rs-0.2.5/.github/workflows/Clippy.yml
+-rw-r--r--   0     1001      123      602 2023-05-25 09:23:18.000000 llm_rs-0.2.5/.github/workflows/PublishDocs.yml
+-rw-r--r--   0     1001      123     3455 2023-05-25 09:23:18.000000 llm_rs-0.2.5/.gitignore
+-rw-r--r--   0     1001      123       72 2023-05-25 09:23:18.000000 llm_rs-0.2.5/.vscode/settings.json
+-rw-r--r--   0     1001      123     1071 2023-05-25 09:23:18.000000 llm_rs-0.2.5/LICENSE
+-rw-r--r--   0     1001      123     3053 2023-05-25 09:23:18.000000 llm_rs-0.2.5/README.md
+-rw-r--r--   0     1001      123     4799 2023-05-25 09:23:18.000000 llm_rs-0.2.5/docs/docs/conversion.md
+-rw-r--r--   0     1001      123     9355 2023-05-25 09:23:18.000000 llm_rs-0.2.5/docs/docs/index.md
+-rw-r--r--   0     1001      123     1181 2023-05-25 09:23:18.000000 llm_rs-0.2.5/docs/mkdocs.yml
+-rw-r--r--   0     1001      123       31 2023-05-25 09:23:18.000000 llm_rs-0.2.5/docs/requirements.txt
+-rw-r--r--   0     1001      123      334 2023-05-25 09:23:18.000000 llm_rs-0.2.5/llm_rs/__init__.py
+-rw-r--r--   0     1001      123    14929 2023-05-25 09:23:18.000000 llm_rs-0.2.5/llm_rs/auto.py
+-rw-r--r--   0     1001      123     1614 2023-05-25 09:23:18.000000 llm_rs-0.2.5/llm_rs/base_model.py
+-rw-r--r--   0     1001      123     1351 2023-05-25 09:23:18.000000 llm_rs-0.2.5/llm_rs/config.pyi
+-rw-r--r--   0     1001      123       78 2023-05-25 09:23:18.000000 llm_rs-0.2.5/llm_rs/convert/__init__.py
+-rw-r--r--   0     1001      123     2223 2023-05-25 09:23:18.000000 llm_rs-0.2.5/llm_rs/convert/auto_converter.py
+-rw-r--r--   0     1001      123      199 2023-05-25 09:23:18.000000 llm_rs-0.2.5/llm_rs/convert/models/__init__.py
+-rw-r--r--   0     1001      123     5581 2023-05-25 09:23:18.000000 llm_rs-0.2.5/llm_rs/convert/models/_base.py
+-rw-r--r--   0     1001      123     3177 2023-05-25 09:23:18.000000 llm_rs-0.2.5/llm_rs/convert/models/bloom.py
+-rw-r--r--   0     1001      123     5221 2023-05-25 09:23:18.000000 llm_rs-0.2.5/llm_rs/convert/models/gpt2.py
+-rw-r--r--   0     1001      123     2032 2023-05-25 09:23:18.000000 llm_rs-0.2.5/llm_rs/convert/models/gptj.py
+-rw-r--r--   0     1001      123     2138 2023-05-25 09:23:18.000000 llm_rs-0.2.5/llm_rs/convert/models/gptneox.py
+-rw-r--r--   0     1001      123     6334 2023-05-25 09:23:18.000000 llm_rs-0.2.5/llm_rs/convert/models/llama.py
+-rw-r--r--   0     1001      123     1893 2023-05-25 09:23:18.000000 llm_rs-0.2.5/llm_rs/convert/models/mpt.py
+-rw-r--r--   0     1001      123        0 2023-05-25 09:23:18.000000 llm_rs-0.2.5/llm_rs/llm_rs.pyi
+-rw-r--r--   0     1001      123      579 2023-05-25 09:23:18.000000 llm_rs-0.2.5/llm_rs/models.pyi
+-rw-r--r--   0     1001      123        0 2023-05-25 09:23:18.000000 llm_rs-0.2.5/llm_rs/py.typed
+-rw-r--r--   0     1001      123     2915 2023-05-25 09:23:18.000000 llm_rs-0.2.5/llm_rs/repository.py
+-rw-r--r--   0     1001      123      697 2023-05-25 09:23:18.000000 llm_rs-0.2.5/llm_rs/results.pyi
+-rw-r--r--   0     1001      123      978 2023-05-25 09:23:18.000000 llm_rs-0.2.5/pyproject.toml
+-rw-r--r--   0     1001      123     4274 2023-05-25 09:23:18.000000 llm_rs-0.2.5/src/configs.rs
+-rw-r--r--   0     1001      123     1685 2023-05-25 09:23:18.000000 llm_rs-0.2.5/src/lib.rs
+-rw-r--r--   0     1001      123     9617 2023-05-25 09:23:18.000000 llm_rs-0.2.5/src/model_base.rs
+-rw-r--r--   0     1001      123      300 2023-05-25 09:23:18.000000 llm_rs-0.2.5/src/models.rs
+-rw-r--r--   0     1001      123     2576 2023-05-25 09:23:18.000000 llm_rs-0.2.5/src/quantize.rs
+-rw-r--r--   0     1001      123     1352 2023-05-25 09:23:18.000000 llm_rs-0.2.5/src/results.rs
+-rw-r--r--   0     1001      123    14030 2023-05-25 09:25:18.000000 llm_rs-0.2.5/Cargo.lock
+-rw-r--r--   0        0        0     4150 1970-01-01 00:00:00.000000 llm_rs-0.2.5/PKG-INFO
```

### Comparing `llm_rs-0.2.4/.github/workflows/BuildDoc.yml` & `llm_rs-0.2.5/.github/workflows/BuildDoc.yml`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.4/.github/workflows/CI.yml` & `llm_rs-0.2.5/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.4/.github/workflows/Clippy.yml` & `llm_rs-0.2.5/.github/workflows/Clippy.yml`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.4/.github/workflows/PublishDocs.yml` & `llm_rs-0.2.5/.github/workflows/PublishDocs.yml`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.4/.gitignore` & `llm_rs-0.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.4/LICENSE` & `llm_rs-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.4/README.md` & `llm_rs-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.4/docs/docs/conversion.md` & `llm_rs-0.2.5/docs/docs/conversion.md`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.4/docs/docs/index.md` & `llm_rs-0.2.5/docs/docs/index.md`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.4/docs/mkdocs.yml` & `llm_rs-0.2.5/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.4/llm_rs/auto.py` & `llm_rs-0.2.5/llm_rs/auto.py`

 * *Files 0% similar despite different names*

```diff
@@ -372,15 +372,15 @@
             logging.warning(f"Target file '{target_file}' already exists, skipping quantization")
             return target_file
         
         logging.info(f"Quantizing model '{model_file}' to '{target_file}'")
         model_type.quantize(model_file,target_file,quantization,container)
 
         metadata_file = pathlib.Path(target_file).with_suffix(".meta")
-        quantized_metadata = ModelMetadata(model=metadata.model,quantization=quantization,container=container,quantization_version=QuantizationVersions.V1)
+        quantized_metadata = ModelMetadata(model=metadata.model,quantization=quantization,container=container,quantization_version=QuantizationVersions.V2)
         quantized_metadata.add_hash(target_file)
         logging.info(f"Writing metadata file '{metadata_file}'")
         metadata_file.write_text(json.dumps(quantized_metadata.serialize()))
         logging.info(f"Finished quantizing model '{model_file}' to '{target_file}'")
         return target_file
```

### Comparing `llm_rs-0.2.4/llm_rs/base_model.py` & `llm_rs-0.2.5/llm_rs/base_model.py`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.4/llm_rs/config.pyi` & `llm_rs-0.2.5/llm_rs/config.pyi`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.4/llm_rs/convert/auto_converter.py` & `llm_rs-0.2.5/llm_rs/convert/auto_converter.py`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.4/llm_rs/convert/models/_base.py` & `llm_rs-0.2.5/llm_rs/convert/models/_base.py`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.4/llm_rs/convert/models/bloom.py` & `llm_rs-0.2.5/llm_rs/convert/models/bloom.py`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.4/llm_rs/convert/models/gpt2.py` & `llm_rs-0.2.5/llm_rs/convert/models/gpt2.py`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.4/llm_rs/convert/models/gptj.py` & `llm_rs-0.2.5/llm_rs/convert/models/gptj.py`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.4/llm_rs/convert/models/gptneox.py` & `llm_rs-0.2.5/llm_rs/convert/models/gptneox.py`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.4/llm_rs/convert/models/llama.py` & `llm_rs-0.2.5/llm_rs/convert/models/llama.py`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.4/llm_rs/convert/models/mpt.py` & `llm_rs-0.2.5/llm_rs/convert/models/mpt.py`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.4/llm_rs/models.pyi` & `llm_rs-0.2.5/llm_rs/models.pyi`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.4/llm_rs/repository.py` & `llm_rs-0.2.5/llm_rs/repository.py`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.4/llm_rs/results.pyi` & `llm_rs-0.2.5/llm_rs/results.pyi`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.4/pyproject.toml` & `llm_rs-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.4/src/configs.rs` & `llm_rs-0.2.5/src/configs.rs`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.4/src/lib.rs` & `llm_rs-0.2.5/src/lib.rs`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.4/src/model_base.rs` & `llm_rs-0.2.5/src/model_base.rs`

 * *Files 1% similar despite different names*

```diff
@@ -195,15 +195,14 @@
                 let path = std::path::Path::new(&path);
                 let lora_paths = lora_paths
                     .map(|strings| strings.into_iter().map(std::path::PathBuf::from).collect());
                 let model_params = llm_base::ModelParameters {
                     context_size: config_to_use.context_length,
                     prefer_mmap: config_to_use.prefer_mmap,
                     lora_adapters: lora_paths.clone(),
-                    ..Default::default()
                 };
                 let llm_model: $llm_model =
                     llm_base::load(&path, model_params, None, |load_progress| {
                         if should_log {
                             llm_base::load_progress_callback_stdout(load_progress)
                         }
                     })
```

### Comparing `llm_rs-0.2.4/src/quantize.rs` & `llm_rs-0.2.5/src/quantize.rs`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     source: PathBuf,
     destination: PathBuf,
     container: ContainerType,
     quantization: QuantizationType,
 ) -> Result<(), QuantizeError> {
     let container = match container {
         ContainerType::GGML => ggml::format::SaveContainerType::Ggml,
-        ContainerType::GGJT => ggml::format::SaveContainerType::GgjtV2,
+        ContainerType::GGJT => ggml::format::SaveContainerType::GgjtV3,
     };
 
     let quantization = match quantization {
         QuantizationType::Q4_0 => Ok(ggml::Type::Q4_0),
         QuantizationType::Q4_1 => Ok(ggml::Type::Q4_1),
         QuantizationType::F16 => Err(QuantizeError::UnsupportedElementType {
             element_type: ggml::Type::F16,
```

### Comparing `llm_rs-0.2.4/src/results.rs` & `llm_rs-0.2.5/src/results.rs`

 * *Files identical despite different names*

### Comparing `llm_rs-0.2.4/Cargo.lock` & `llm_rs-0.2.5/Cargo.lock`

 * *Files 10% similar despite different names*

```diff
@@ -48,24 +48,24 @@
  "libc",
  "wasi",
 ]
 
 [[package]]
 name = "ggml"
 version = "0.1.1"
-source = "git+https://github.com/rustformers/llm.git#c51ff5d60b4177d2c75ee8483c25b2b4ee88f07e"
+source = "git+https://github.com/rustformers/llm.git#d9f59b5b3c2d1c6d663686cee49090704ef41149"
 dependencies = [
  "ggml-sys",
  "thiserror",
 ]
 
 [[package]]
 name = "ggml-sys"
 version = "0.1.1"
-source = "git+https://github.com/rustformers/llm.git#c51ff5d60b4177d2c75ee8483c25b2b4ee88f07e"
+source = "git+https://github.com/rustformers/llm.git#d9f59b5b3c2d1c6d663686cee49090704ef41149"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "half"
 version = "2.2.1"
@@ -86,30 +86,30 @@
 version = "0.2.144"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b00cc1c228a6782d0f076e7b232802e0c5689d41bb5df366f2a6b6621cfdfe1"
 
 [[package]]
 name = "llm"
 version = "0.1.1"
-source = "git+https://github.com/rustformers/llm.git#c51ff5d60b4177d2c75ee8483c25b2b4ee88f07e"
+source = "git+https://github.com/rustformers/llm.git#d9f59b5b3c2d1c6d663686cee49090704ef41149"
 dependencies = [
  "llm-base",
  "llm-bloom",
  "llm-gpt2",
  "llm-gptj",
  "llm-gptneox",
  "llm-llama",
  "llm-mpt",
  "serde",
 ]
 
 [[package]]
 name = "llm-base"
 version = "0.1.1"
-source = "git+https://github.com/rustformers/llm.git#c51ff5d60b4177d2c75ee8483c25b2b4ee88f07e"
+source = "git+https://github.com/rustformers/llm.git#d9f59b5b3c2d1c6d663686cee49090704ef41149"
 dependencies = [
  "bytemuck",
  "ggml",
  "half",
  "memmap2",
  "partial_sort",
  "rand",
@@ -117,71 +117,71 @@
  "serde_bytes",
  "thiserror",
 ]
 
 [[package]]
 name = "llm-bloom"
 version = "0.1.1"
-source = "git+https://github.com/rustformers/llm.git#c51ff5d60b4177d2c75ee8483c25b2b4ee88f07e"
+source = "git+https://github.com/rustformers/llm.git#d9f59b5b3c2d1c6d663686cee49090704ef41149"
 dependencies = [
  "bytemuck",
  "llm-base",
 ]
 
 [[package]]
 name = "llm-gpt2"
 version = "0.1.1"
-source = "git+https://github.com/rustformers/llm.git#c51ff5d60b4177d2c75ee8483c25b2b4ee88f07e"
+source = "git+https://github.com/rustformers/llm.git#d9f59b5b3c2d1c6d663686cee49090704ef41149"
 dependencies = [
  "bytemuck",
  "llm-base",
 ]
 
 [[package]]
 name = "llm-gptj"
 version = "0.1.1"
-source = "git+https://github.com/rustformers/llm.git#c51ff5d60b4177d2c75ee8483c25b2b4ee88f07e"
+source = "git+https://github.com/rustformers/llm.git#d9f59b5b3c2d1c6d663686cee49090704ef41149"
 dependencies = [
  "bytemuck",
  "llm-base",
 ]
 
 [[package]]
 name = "llm-gptneox"
 version = "0.1.1"
-source = "git+https://github.com/rustformers/llm.git#c51ff5d60b4177d2c75ee8483c25b2b4ee88f07e"
+source = "git+https://github.com/rustformers/llm.git#d9f59b5b3c2d1c6d663686cee49090704ef41149"
 dependencies = [
  "bytemuck",
  "llm-base",
  "serde",
 ]
 
 [[package]]
 name = "llm-llama"
 version = "0.1.1"
-source = "git+https://github.com/rustformers/llm.git#c51ff5d60b4177d2c75ee8483c25b2b4ee88f07e"
+source = "git+https://github.com/rustformers/llm.git#d9f59b5b3c2d1c6d663686cee49090704ef41149"
 dependencies = [
  "bytemuck",
  "llm-base",
  "rand",
  "thiserror",
 ]
 
 [[package]]
 name = "llm-mpt"
 version = "0.1.1"
-source = "git+https://github.com/rustformers/llm.git#c51ff5d60b4177d2c75ee8483c25b2b4ee88f07e"
+source = "git+https://github.com/rustformers/llm.git#d9f59b5b3c2d1c6d663686cee49090704ef41149"
 dependencies = [
  "bytemuck",
  "llm-base",
 ]
 
 [[package]]
 name = "llm-rs"
-version = "0.2.4"
+version = "0.2.5"
 dependencies = [
  "ggml",
  "llm",
  "llm-base",
  "log",
  "pyo3",
  "rand",
@@ -470,17 +470,17 @@
  "proc-macro2",
  "quote",
  "syn 2.0.16",
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

### Comparing `llm_rs-0.2.4/PKG-INFO` & `llm_rs-0.2.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-rs
-Version: 0.2.4
+Version: 0.2.5
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: blake3
 Requires-Dist: huggingface-hub >= 0.14.1
@@ -17,16 +17,16 @@
 Provides-Extra: convert
 License-File: LICENSE
 Summary: Unofficial python bindings for llm-rs. 🐍❤️🦀
 Keywords: LLM,Transformers
 Author: Lukas Kreussel
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: documentation, https://llukas22.github.io/llm-rs-python/
 Project-URL: repository, https://github.com/LLukas22/llm-rs-python
+Project-URL: documentation, https://llukas22.github.io/llm-rs-python/
 
 # llm-rs-python: Python Bindings for Rust's llm Library
 
 Welcome to `llm-rs`, an unofficial Python interface for the Rust-based [llm](https://github.com/rustformers/llm) library, made possible through [PyO3](https://github.com/PyO3/pyo3). Our package combines the convenience of Python with the performance of Rust to offer an efficient tool for your machine learning projects. 🐍❤️🦀
 
 With `llm-rs`, you can operate a variety of Large Language Models (LLMs) including LLama and GPT-NeoX directly on your CPU.
```

