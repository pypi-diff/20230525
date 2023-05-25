# Comparing `tmp/varwizard-0.2.tar.gz` & `tmp/varwizard-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "varwizard-0.2.tar", max compression
+gzip compressed data, was "varwizard-0.2.1.tar", max compression
```

## Comparing `varwizard-0.2.tar` & `varwizard-0.2.1.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0      746 2023-05-17 09:38:45.519137 varwizard-0.2/pyproject.toml
--rw-r--r--   0        0        0     2021 2023-05-17 09:39:36.088003 varwizard-0.2/readme.md
--rw-r--r--   0        0        0       82 2023-05-17 09:38:58.503358 varwizard-0.2/varwizard/__init__.py
--rw-r--r--   0        0        0       59 2023-05-17 04:28:27.343893 varwizard-0.2/varwizard/__main__.py
--rw-r--r--   0        0        0     1659 2023-05-17 06:43:28.374791 varwizard-0.2/varwizard/cli.py
--rw-r--r--   0        0        0       51 2023-05-12 16:52:19.678029 varwizard-0.2/varwizard/config/__init__.py
--rw-r--r--   0        0        0      554 2023-05-11 10:13:41.198952 varwizard-0.2/varwizard/config/prefix_tuning.py
--rw-r--r--   0        0        0        0 2023-05-11 10:13:40.654943 varwizard-0.2/varwizard/data/__init__.py
--rw-r--r--   0        0        0     2904 2023-05-17 09:17:31.229411 varwizard-0.2/varwizard/data/input_preparation.py
--rw-r--r--   0        0        0        0 2023-05-11 10:13:40.654943 varwizard-0.2/varwizard/generation/__init__.py
--rw-r--r--   0        0        0     1005 2023-05-17 08:15:49.110211 varwizard-0.2/varwizard/generation/gen.py
--rw-r--r--   0        0        0   401536 2023-05-11 10:13:40.998948 varwizard-0.2/varwizard/libs/tree-sitter/c.so
--rw-r--r--   0        0        0  4076856 2023-05-11 10:13:41.242952 varwizard-0.2/varwizard/libs/tree-sitter/c_sharp.so
--rw-r--r--   0        0        0  2300056 2023-05-11 10:13:41.446956 varwizard-0.2/varwizard/libs/tree-sitter/cpp.so
--rw-r--r--   0        0        0   246152 2023-05-11 10:13:41.190951 varwizard-0.2/varwizard/libs/tree-sitter/go.so
--rw-r--r--   0        0        0   401704 2023-05-11 10:13:41.494956 varwizard-0.2/varwizard/libs/tree-sitter/java.so
--rw-r--r--   0        0        0   354200 2023-05-11 10:13:41.458956 varwizard-0.2/varwizard/libs/tree-sitter/javascript.so
--rw-r--r--   0        0        0   785016 2023-05-11 10:13:41.490956 varwizard-0.2/varwizard/libs/tree-sitter/php.so
--rw-r--r--   0        0        0   494864 2023-05-11 10:13:41.470956 varwizard-0.2/varwizard/libs/tree-sitter/python.so
--rw-r--r--   0        0        0  2130104 2023-05-11 10:13:41.090950 varwizard-0.2/varwizard/libs/tree-sitter/ruby.so
--rw-r--r--   0        0        0   849608 2023-05-11 10:13:41.238952 varwizard-0.2/varwizard/libs/tree-sitter/rust.so
--rw-r--r--   0        0        0        0 2023-05-11 10:13:40.654943 varwizard-0.2/varwizard/models/__init__.py
--rw-r--r--   0        0        0      252 2023-05-11 10:13:41.090950 varwizard-0.2/varwizard/models/bloom.py
--rw-r--r--   0        0        0     2178 2023-05-17 09:26:23.014501 varwizard-0.2/varwizard/models/varwizard.py
--rw-r--r--   0        0        0        0 2023-05-11 10:13:40.654943 varwizard-0.2/varwizard/utils/__init__.py
--rw-r--r--   0        0        0    13556 2023-05-11 10:13:41.086950 varwizard-0.2/varwizard/utils/obfuscation.py
--rw-r--r--   0        0        0     3015 1970-01-01 00:00:00.000000 varwizard-0.2/PKG-INFO
+-rw-r--r--   0        0        0      748 2023-05-25 12:00:28.451723 varwizard-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2048 2023-05-25 12:55:16.830778 varwizard-0.2.1/readme.md
+-rw-r--r--   0        0        0       84 2023-05-25 12:30:46.711987 varwizard-0.2.1/varwizard/__init__.py
+-rw-r--r--   0        0        0       59 2023-05-17 04:28:27.343893 varwizard-0.2.1/varwizard/__main__.py
+-rw-r--r--   0        0        0     1675 2023-05-25 12:31:15.324437 varwizard-0.2.1/varwizard/cli.py
+-rw-r--r--   0        0        0       51 2023-05-12 16:52:19.678029 varwizard-0.2.1/varwizard/config/__init__.py
+-rw-r--r--   0        0        0      777 2023-05-25 12:36:46.261554 varwizard-0.2.1/varwizard/config/prefix_tuning.py
+-rw-r--r--   0        0        0        0 2023-05-11 10:13:40.654943 varwizard-0.2.1/varwizard/data/__init__.py
+-rw-r--r--   0        0        0     3250 2023-05-25 12:39:09.295726 varwizard-0.2.1/varwizard/data/input_preparation.py
+-rw-r--r--   0        0        0        0 2023-05-11 10:13:40.654943 varwizard-0.2.1/varwizard/generation/__init__.py
+-rw-r--r--   0        0        0     1305 2023-05-25 12:52:49.844575 varwizard-0.2.1/varwizard/generation/gen.py
+-rw-r--r--   0        0        0   401536 2023-05-11 10:13:40.998948 varwizard-0.2.1/varwizard/libs/tree-sitter/c.so
+-rw-r--r--   0        0        0  4076856 2023-05-11 10:13:41.242952 varwizard-0.2.1/varwizard/libs/tree-sitter/c_sharp.so
+-rw-r--r--   0        0        0  2300056 2023-05-11 10:13:41.446956 varwizard-0.2.1/varwizard/libs/tree-sitter/cpp.so
+-rw-r--r--   0        0        0   246152 2023-05-11 10:13:41.190951 varwizard-0.2.1/varwizard/libs/tree-sitter/go.so
+-rw-r--r--   0        0        0   401704 2023-05-11 10:13:41.494956 varwizard-0.2.1/varwizard/libs/tree-sitter/java.so
+-rw-r--r--   0        0        0   354200 2023-05-11 10:13:41.458956 varwizard-0.2.1/varwizard/libs/tree-sitter/javascript.so
+-rw-r--r--   0        0        0   785016 2023-05-11 10:13:41.490956 varwizard-0.2.1/varwizard/libs/tree-sitter/php.so
+-rw-r--r--   0        0        0   494864 2023-05-11 10:13:41.470956 varwizard-0.2.1/varwizard/libs/tree-sitter/python.so
+-rw-r--r--   0        0        0  2130104 2023-05-11 10:13:41.090950 varwizard-0.2.1/varwizard/libs/tree-sitter/ruby.so
+-rw-r--r--   0        0        0   849608 2023-05-11 10:13:41.238952 varwizard-0.2.1/varwizard/libs/tree-sitter/rust.so
+-rw-r--r--   0        0        0        0 2023-05-11 10:13:40.654943 varwizard-0.2.1/varwizard/models/__init__.py
+-rw-r--r--   0        0        0      252 2023-05-11 10:13:41.090950 varwizard-0.2.1/varwizard/models/bloom.py
+-rw-r--r--   0        0        0      261 2023-05-25 12:32:09.249284 varwizard-0.2.1/varwizard/models/codet5.py
+-rw-r--r--   0        0        0     2795 2023-05-25 12:42:39.214988 varwizard-0.2.1/varwizard/models/varwizard.py
+-rw-r--r--   0        0        0        0 2023-05-11 10:13:40.654943 varwizard-0.2.1/varwizard/utils/__init__.py
+-rw-r--r--   0        0        0    13556 2023-05-11 10:13:41.086950 varwizard-0.2.1/varwizard/utils/obfuscation.py
+-rw-r--r--   0        0        0     3044 1970-01-01 00:00:00.000000 varwizard-0.2.1/PKG-INFO
```

### Comparing `varwizard-0.2/pyproject.toml` & `varwizard-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "setuptools>=60",
     "wheel",
 ]
 build-backend = "setuptools.build_meta"
 [tool.poetry]
 name="varwizard"
-version="0.2"
+version="0.2.1"
 license = "Apache-2.0"
 description = "An Automated Tool for Improving Code Quality Through Variable Name Refinement with Language Models"
 readme = "readme.md"
 homepage = "https://github.com/FSoft-AI4Code/VarWizard"
 repository = "https://github.com/FSoft-AI4Code/VarWizard"
 keywords = ["variable renaming", "language models", "code quality"]
 authors = ["FSoft-AI4Code <support.aic@fpt.com>"]
```

### Comparing `varwizard-0.2/readme.md` & `varwizard-0.2.1/readme.md`

 * *Files 22% similar despite different names*

```diff
@@ -11,31 +11,32 @@
     pip install varwizard
 ```
 3. Usage
     * Command-line
     
     You can use VarWizard by running the command
 ```
-varwizard [--model-name {bloom-560m}]
+varwizard [--model-name {bloom-560m, codet5-base}]
             --input INPUT --lang {c,cpp,java,php,go,javascript,ruby,rust,python,c_sharp} 
             [--output-path OUTPUT_PATH] [--max-input-len MAX_INPUT_LEN]
             [--device DEVICE] [--penalty-alpha PENALTY_ALPHA] [--top-k TOP_K] [--max-new-tokens MAX_NEW_TOKENS]
 ```
 Details for each argument can be found by 
 ```varwizard --help```
 
 
  * Python API
+
 Another way is to Python methods.
 Here is a simple example of VarWizard.
 ```
 from varwizard import VarWizard
 
-model = VarWizard()
+model = VarWizard(model_name = "codet5-base")
 code = """
 static void lsp2poly ( int * var0, const int16_t * var1, int var2 ) { int var3, var4 ; var0 [ 0 ] = 0x400000 ; // 1.0 in (3.22) var0 [ 1 ] = - var1 [ 0 ] << 8 ; // *2 and (0.15) -> (3.22) for ( var3 = 2 ; var3 <= var2 ; var3 ++ ) { var0 [ var3 ] = var0 [ var3 - 2 ] ; for ( var4 = var3 ; var4 > 1 ; var4 -- ) var0 [ var4 ] -= MULL ( var0 [ var4 - 1 ], var1 [ 2 * var3 - 2 ], FRAC_BITS ) - var0 [ var4 - 2 ] ; var0 [ 1 ] -= var1 [ 2 * var3 - 2 ] << 8 ; } }"""
 print(model.make_new_code(code, 'cpp', device = 'cuda:0'))
 ```
 VarWizard produces the output
 ```
-static void lsp2poly ( int * lsp, const int16_t * lsp2, int nbits ) { int index, count ; lsp [ 0 ] = 0x400000 ; // 1.0 in (3.22) lsp [ 1 ] = - lsp2 [ 0 ] << 8 ; // *2 and (0.15) -> (3.22) for ( index = 2 ; index <= nbits ; index ++ ) { lsp [ index ] = lsp [ index - 2 ] ; for ( count = index ; count > 1 ; count -- ) lsp [ count ] -= MULL ( lsp [ count - 1 ], lsp2 [ 2 * index - 2 ], FRAC_BITS ) - lsp [ count - 2 ] ; lsp [ 1 ] -= lsp2 [ 2 * index - 2 ] << 8 ; } }
+static void lsp2poly ( int * m_poly, const int16_t * m_h, int m_n ) { int m_i, m_j ; m_poly [ 0 ] = 0x400000 ; // 1.0 in (3.22) m_poly [ 1 ] = - m_h [ 0 ] << 8 ; // *2 and (0.15) -> (3.22) for ( m_i = 2 ; m_i <= m_n ; m_i ++ ) { m_poly [ m_i ] = m_poly [ m_i - 2 ] ; for ( m_j = m_i ; m_j > 1 ; m_j -- ) m_poly [ m_j ] -= MULL ( m_poly [ m_j - 1 ], m_h [ 2 * m_i - 2 ], FRAC_BITS ) - m_poly [ m_j - 2 ] ; m_poly [ 1 ] -= m_h [ 2 * m_i - 2 ] << 8 ; } }
 ```
```

### Comparing `varwizard-0.2/varwizard/cli.py` & `varwizard-0.2.1/varwizard/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from varwizard import VarWizard
 import argparse
 import warnings
 def main():
     parser = argparse.ArgumentParser()
-    parser.add_argument('--model-name', help = 'base pretrained model', type = str, default = 'bloom-560m', choices = ['bloom-560m'])
+    parser.add_argument('--model-name', help = 'base pretrained model', type = str, default = 'bloom-560m', choices = VarWizard.__supported_models__)
     parser.add_argument('--input', type = str, required = True, help = 'input for VarWizard (a string of code or a file path)')
     parser.add_argument('--lang', type = str, required = True, help = 'the programming language of the input', choices = ['c', 'cpp', 'java', 'php', 'go', 'javascript', 'ruby', 'rust', 'python', 'c_sharp'])
     parser.add_argument('--output-path', type = str, help = 'the path of the output file if you want to save the output')
     parser.add_argument('--max-input-len', type = int, default = 400, help = 'the maximum number of input tokens (default: 400)')
     parser.add_argument('--device', type = str, default = 'cpu', help = 'used device for generating the output (default: cpu)')
     parser.add_argument('--penalty-alpha', default = 0.6, type = float, help = 'penalty-alpha of the contrastive search')
     parser.add_argument('--top-k', default = 4, type = int, help = 'top-k')
```

### Comparing `varwizard-0.2/varwizard/data/input_preparation.py` & `varwizard-0.2.1/varwizard/data/input_preparation.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,15 +15,15 @@
                     new_function_bytes = function_bytes
                 new_function_bytes = new_function_bytes[:function_root.start_byte + offset] + vmap[node_token].encode() + new_function_bytes[function_root.end_byte + offset:]
                 offset += len(vmap[node_token].encode()) - function_root.end_byte + function_root.start_byte
                 return new_function_bytes, offset
     for child in function_root.children:
         new_function_bytes, offset = beautify(child, function_bytes, vmap, new_function_bytes, offset)
     return new_function_bytes, offset
-def prepare_input(input, lang, tokenizer, max_input_len: int = 400, prompt = ' Output var0 ='):
+def prepare_input(input, lang, tokenizer, base_model_name, max_input_len: int = 400, prompt = ' Output var0 ='):
     parser = Parser()
     so_path = resource_filename('varwizard', f'libs/tree-sitter/{lang}.so')
     parser.set_language(Language(so_path, lang))
     
     bytes = input.encode()
     root = parser.parse(bytes).root_node
     code_parser = lang.replace('_', '')
@@ -40,12 +40,16 @@
         chosen_ids = list(map(idens['vars'].get, chosen_vars))
         chosen_tup = sorted(list(zip(chosen_vars, chosen_ids)), key = lambda x: x[1])
         vmap = {}
         for i, var_name in enumerate(chosen_tup):
             vmap[var_name[0]] = f'var{i}'
         new_function_bytes, _ = beautify(function_root, function_bytes, vmap)
         function_code = new_function_bytes.decode()
-        source_tokens = tokenizer.tokenize(function_code, truncation = True, max_length = max_input_len)
-        prompt_tokens = tokenizer.tokenize(prompt)
-        input_tokens = source_tokens + prompt_tokens
-        input_ids = [tokenizer.bos_token_id] + tokenizer.convert_tokens_to_ids(input_tokens)
+        if 'bloom' in base_model_name:
+            source_tokens = tokenizer.tokenize(function_code, truncation = True, max_length = max_input_len)
+            prompt_tokens = tokenizer.tokenize(prompt)
+            input_tokens = source_tokens + prompt_tokens
+            input_ids = [tokenizer.bos_token_id] + tokenizer.convert_tokens_to_ids(input_tokens)
+        elif 'codet5' in base_model_name:
+            input_tokens = tokenizer.tokenize(function_code, truncation = True, max_length = max_input_len)
+            input_ids = [tokenizer.bos_token_id] + tokenizer.convert_tokens_to_ids(input_tokens) + [tokenizer.eos_token_id]
         yield input_ids, {v: k for k, v in vmap.items()}
```

### Comparing `varwizard-0.2/varwizard/generation/gen.py` & `varwizard-0.2.1/varwizard/generation/gen.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,25 @@
-def generate(input_ids, vmap, tokenizer, model, max_new_tokens: int = 100, penalty_alpha: float = 0.6, top_k: int = 4):
+def generate(input_ids, vmap, tokenizer, model, base_model_name, max_new_tokens: int = 100, penalty_alpha: float = 0.6, top_k: int = 4):
     attention_mask = input_ids.ne(tokenizer.pad_token_id)
+    
     predictions = model.generate(input_ids = input_ids,
                                   attention_mask =  attention_mask,
                    max_new_tokens = max_new_tokens,
                    penalty_alpha = penalty_alpha,
                    top_k = top_k,
                    eos_token_id = tokenizer.eos_token_id)
     prediction = tokenizer.batch_decode(predictions.cpu().numpy())[0]
-    obfuscated_code, prediction, *_ = prediction.replace('<s>', '').replace('</s>','').split('Output')
+    if 'bloom' in base_model_name:
+        obfuscated_code, prediction, *_ = prediction.replace('<s>', '').replace('</s>','').split('Output')
+        new_code = obfuscated_code
+    elif 'codet5' in base_model_name:
+        start_pos = prediction.find('var0')
+        prediction = prediction[start_pos:].replace('</s>', '')
+        new_code = tokenizer.decode(input_ids[0]).replace('<s>', '').replace('</s>', '')
     pred_coms = prediction.split()
-    new_code = obfuscated_code
     new_vmap = {}
     for i in range(len(pred_coms) // 3):
         key, _, value = pred_coms[3 * i: 3 * i + 3]
         new_vmap[key] = value
     vmap.update(new_vmap)
     for key, value in vmap.items():
         new_code = new_code.replace(key, value)
```

### Comparing `varwizard-0.2/varwizard/libs/tree-sitter/c.so` & `varwizard-0.2.1/varwizard/libs/tree-sitter/c.so`

 * *Files identical despite different names*

### Comparing `varwizard-0.2/varwizard/libs/tree-sitter/c_sharp.so` & `varwizard-0.2.1/varwizard/libs/tree-sitter/c_sharp.so`

 * *Files identical despite different names*

### Comparing `varwizard-0.2/varwizard/libs/tree-sitter/cpp.so` & `varwizard-0.2.1/varwizard/libs/tree-sitter/cpp.so`

 * *Files identical despite different names*

### Comparing `varwizard-0.2/varwizard/libs/tree-sitter/go.so` & `varwizard-0.2.1/varwizard/libs/tree-sitter/go.so`

 * *Files identical despite different names*

### Comparing `varwizard-0.2/varwizard/libs/tree-sitter/java.so` & `varwizard-0.2.1/varwizard/libs/tree-sitter/java.so`

 * *Files identical despite different names*

### Comparing `varwizard-0.2/varwizard/libs/tree-sitter/javascript.so` & `varwizard-0.2.1/varwizard/libs/tree-sitter/javascript.so`

 * *Files identical despite different names*

### Comparing `varwizard-0.2/varwizard/libs/tree-sitter/php.so` & `varwizard-0.2.1/varwizard/libs/tree-sitter/php.so`

 * *Files identical despite different names*

### Comparing `varwizard-0.2/varwizard/libs/tree-sitter/python.so` & `varwizard-0.2.1/varwizard/libs/tree-sitter/python.so`

 * *Files identical despite different names*

### Comparing `varwizard-0.2/varwizard/libs/tree-sitter/ruby.so` & `varwizard-0.2.1/varwizard/libs/tree-sitter/ruby.so`

 * *Files identical despite different names*

### Comparing `varwizard-0.2/varwizard/libs/tree-sitter/rust.so` & `varwizard-0.2.1/varwizard/libs/tree-sitter/rust.so`

 * *Files identical despite different names*

### Comparing `varwizard-0.2/varwizard/models/varwizard.py` & `varwizard-0.2.1/varwizard/models/varwizard.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,46 +8,56 @@
 from varwizard.config import get_prefix_tuning_config
 from varwizard.data.input_preparation import prepare_input
 from varwizard.models.bloom import get_tokenizer_and_model
 from varwizard.generation.gen import generate
 
 
 def get_varwizard_model(varwizard_path = 'Fsoft-AIC/VarWizard', model_name = 'bigscience/bloom-560m'):
+	if 'bloom' in model_name:
+		from varwizard.models.bloom import get_tokenizer_and_model
+	else:
+		from varwizard.models.codet5 import get_tokenizer_and_model
+	base_model_name = model_name.split('/')[1].replace('-', '_')
 	tokenizer, model = get_tokenizer_and_model(model_name)
-	peft_config = get_prefix_tuning_config()
+	peft_config = get_prefix_tuning_config(base_model_name)
 	model = get_peft_model(model, peft_config)
-	cp_path = hf_hub_download(repo_id = varwizard_path, filename = "varwizard.tar")
+	base_model_name = model_name.split('/')[1].replace('-', '_')
+	cp_path = hf_hub_download(repo_id = varwizard_path, filename = f"varwizard_{base_model_name}.tar")
 	cp_data = torch.load(cp_path, map_location = 'cpu')
 	model.load_state_dict(cp_data, strict = False)
 	return tokenizer, model
 
 class VarWizard:
+	__supported_models__ = ['bloom-560m', 'codet5-base']
 	def __init__(self, model_name = 'bloom-560m'):
-		assert model_name in ['bloom-560m'], "this model isn't supported"
+		assert model_name in VarWizard.__supported_models__, f"this model: {model_name} isn't supported"
 		if model_name == 'bloom-560m':
 			model_name = f'bigscience/{model_name}'
-		tokenizer, model = get_varwizard_model()
+		elif model_name == 'codet5-base':
+			model_name = 'Salesforce/codet5-base'
+		tokenizer, model = get_varwizard_model(model_name = model_name)
 		self.tokenizer = tokenizer
 		self.model = model.eval()
+		self.base_model_name = model_name
 		self.prepare_input = functools.partial(prepare_input, tokenizer = tokenizer)
-		self.generate = functools.partial(generate, tokenizer = self.tokenizer, model = self.model)
+		self.generate = functools.partial(generate, base_model_name = self.base_model_name, tokenizer = self.tokenizer, model = self.model)
 	@torch.inference_mode()
 	def make_new_code(self, input, lang, output_path = None, max_input_len: int = 400, max_new_tokens: int = 100, penalty_alpha: float = 0.6, top_k: int = 4, device = 'cpu'):
 		if os.path.exists(input):
 			with open(input) as f:
 				input = f.read()
 		input = input.strip()
 		all_predictions = []
-		for input_ids, vmap in self.prepare_input(input, lang, max_input_len = max_input_len):
+		for input_ids, vmap in self.prepare_input(input, lang, base_model_name = self.base_model_name, max_input_len = max_input_len):
 			input_ids = torch.tensor(input_ids)
 			input_ids = input_ids.to(device)
 			self.model.device = device
 			self.model.to(device)
 			input_ids = input_ids.unsqueeze(0)
 			prediction = self.generate(input_ids, vmap, max_new_tokens = max_new_tokens, penalty_alpha = penalty_alpha, top_k = top_k)
 			all_predictions.append(prediction)
 		prediction = '\n'.join(all_predictions)
 		if output_path is not None:
 			with open(output_path, 'w') as f:
 				f.write(prediction)
 		return prediction
-
+
```

### Comparing `varwizard-0.2/varwizard/utils/obfuscation.py` & `varwizard-0.2.1/varwizard/utils/obfuscation.py`

 * *Files identical despite different names*

### Comparing `varwizard-0.2/PKG-INFO` & `varwizard-0.2.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: varwizard
-Version: 0.2
+Version: 0.2.1
 Summary: An Automated Tool for Improving Code Quality Through Variable Name Refinement with Language Models
 Home-page: https://github.com/FSoft-AI4Code/VarWizard
 License: Apache-2.0
 Keywords: variable renaming,language models,code quality
 Author: FSoft-AI4Code
 Author-email: support.aic@fpt.com
 Requires-Python: >=3.7
@@ -36,31 +36,32 @@
     pip install varwizard
 ```
 3. Usage
     * Command-line
     
     You can use VarWizard by running the command
 ```
-varwizard [--model-name {bloom-560m}]
+varwizard [--model-name {bloom-560m, codet5-base}]
             --input INPUT --lang {c,cpp,java,php,go,javascript,ruby,rust,python,c_sharp} 
             [--output-path OUTPUT_PATH] [--max-input-len MAX_INPUT_LEN]
             [--device DEVICE] [--penalty-alpha PENALTY_ALPHA] [--top-k TOP_K] [--max-new-tokens MAX_NEW_TOKENS]
 ```
 Details for each argument can be found by 
 ```varwizard --help```
 
 
  * Python API
+
 Another way is to Python methods.
 Here is a simple example of VarWizard.
 ```
 from varwizard import VarWizard
 
-model = VarWizard()
+model = VarWizard(model_name = "codet5-base")
 code = """
 static void lsp2poly ( int * var0, const int16_t * var1, int var2 ) { int var3, var4 ; var0 [ 0 ] = 0x400000 ; // 1.0 in (3.22) var0 [ 1 ] = - var1 [ 0 ] << 8 ; // *2 and (0.15) -> (3.22) for ( var3 = 2 ; var3 <= var2 ; var3 ++ ) { var0 [ var3 ] = var0 [ var3 - 2 ] ; for ( var4 = var3 ; var4 > 1 ; var4 -- ) var0 [ var4 ] -= MULL ( var0 [ var4 - 1 ], var1 [ 2 * var3 - 2 ], FRAC_BITS ) - var0 [ var4 - 2 ] ; var0 [ 1 ] -= var1 [ 2 * var3 - 2 ] << 8 ; } }"""
 print(model.make_new_code(code, 'cpp', device = 'cuda:0'))
 ```
 VarWizard produces the output
 ```
-static void lsp2poly ( int * lsp, const int16_t * lsp2, int nbits ) { int index, count ; lsp [ 0 ] = 0x400000 ; // 1.0 in (3.22) lsp [ 1 ] = - lsp2 [ 0 ] << 8 ; // *2 and (0.15) -> (3.22) for ( index = 2 ; index <= nbits ; index ++ ) { lsp [ index ] = lsp [ index - 2 ] ; for ( count = index ; count > 1 ; count -- ) lsp [ count ] -= MULL ( lsp [ count - 1 ], lsp2 [ 2 * index - 2 ], FRAC_BITS ) - lsp [ count - 2 ] ; lsp [ 1 ] -= lsp2 [ 2 * index - 2 ] << 8 ; } }
+static void lsp2poly ( int * m_poly, const int16_t * m_h, int m_n ) { int m_i, m_j ; m_poly [ 0 ] = 0x400000 ; // 1.0 in (3.22) m_poly [ 1 ] = - m_h [ 0 ] << 8 ; // *2 and (0.15) -> (3.22) for ( m_i = 2 ; m_i <= m_n ; m_i ++ ) { m_poly [ m_i ] = m_poly [ m_i - 2 ] ; for ( m_j = m_i ; m_j > 1 ; m_j -- ) m_poly [ m_j ] -= MULL ( m_poly [ m_j - 1 ], m_h [ 2 * m_i - 2 ], FRAC_BITS ) - m_poly [ m_j - 2 ] ; m_poly [ 1 ] -= m_h [ 2 * m_i - 2 ] << 8 ; } }
 ```
```

