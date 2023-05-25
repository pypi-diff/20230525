# Comparing `tmp/dna_parser-0.2.0.tar.gz` & `tmp/dna_parser-0.2.1.tar.gz`

## Comparing `dna_parser-0.2.0.tar` & `dna_parser-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      361 1970-01-01 00:00:00.000000 dna_parser-0.2.0/Cargo.toml
--rw-r--r--   0     1001      123     1097 2023-05-24 17:21:58.000000 dna_parser-0.2.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      123     1506 2023-05-24 17:21:58.000000 dna_parser-0.2.0/.github/workflows/release.yml
--rw-r--r--   0     1001      123      685 2023-05-24 17:21:58.000000 dna_parser-0.2.0/.gitignore
--rw-r--r--   0     1001      123     1065 2023-05-24 17:21:58.000000 dna_parser-0.2.0/LICENSE
--rw-r--r--   0     1001      123     5189 2023-05-24 17:21:58.000000 dna_parser-0.2.0/README.md
--rw-r--r--   0     1001      123      396 2023-05-24 17:21:58.000000 dna_parser-0.2.0/pyproject.toml
--rw-r--r--   0     1001      123      153 2023-05-24 17:21:58.000000 dna_parser-0.2.0/python/dna_parser/__init__.py
--rw-r--r--   0     1001      123      618 2023-05-24 17:21:58.000000 dna_parser-0.2.0/python/dna_parser/call_functions.py
--rwxr-xr-x   0     1001      123      833 2023-05-24 17:22:32.000000 dna_parser-0.2.0/run-maturin-action.sh
--rw-r--r--   0     1001      123     6771 2023-05-24 17:21:58.000000 dna_parser-0.2.0/src/cross.rs
--rw-r--r--   0     1001      123     2778 2023-05-24 17:21:58.000000 dna_parser-0.2.0/src/fasta_files.rs
--rw-r--r--   0     1001      123      430 2023-05-24 17:21:58.000000 dna_parser-0.2.0/src/kmers.rs
--rw-r--r--   0     1001      123     1018 2023-05-24 17:21:58.000000 dna_parser-0.2.0/src/lib.rs
--rw-r--r--   0     1001      123     6992 2023-05-24 17:21:58.000000 dna_parser-0.2.0/src/onehot.rs
--rw-r--r--   0     1001      123     5999 2023-05-24 17:21:58.000000 dna_parser-0.2.0/src/ordinal.rs
--rw-r--r--   0     1001      123     3906 2023-05-24 17:21:58.000000 dna_parser-0.2.0/src/random_sequence.rs
--rw-r--r--   0     1001      123     3671 2023-05-24 17:21:58.000000 dna_parser-0.2.0/src/tfidf.rs
--rw-r--r--   0     1001      123     1715 2023-05-24 17:21:58.000000 dna_parser-0.2.0/src/utils/mod.rs
--rw-r--r--   0     1001      123    11845 2023-05-24 17:24:37.000000 dna_parser-0.2.0/Cargo.lock
--rw-r--r--   0        0        0     5571 1970-01-01 00:00:00.000000 dna_parser-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      361 1970-01-01 00:00:00.000000 dna_parser-0.2.1/Cargo.toml
+-rw-r--r--   0     1001      123     1097 2023-05-25 19:08:39.000000 dna_parser-0.2.1/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123     1506 2023-05-25 19:08:39.000000 dna_parser-0.2.1/.github/workflows/release.yml
+-rw-r--r--   0     1001      123      685 2023-05-25 19:08:39.000000 dna_parser-0.2.1/.gitignore
+-rw-r--r--   0     1001      123     1065 2023-05-25 19:08:39.000000 dna_parser-0.2.1/LICENSE
+-rw-r--r--   0     1001      123     5189 2023-05-25 19:08:39.000000 dna_parser-0.2.1/README.md
+-rw-r--r--   0     1001      123      396 2023-05-25 19:08:39.000000 dna_parser-0.2.1/pyproject.toml
+-rw-r--r--   0     1001      123      153 2023-05-25 19:08:39.000000 dna_parser-0.2.1/python/dna_parser/__init__.py
+-rw-r--r--   0     1001      123      618 2023-05-25 19:08:39.000000 dna_parser-0.2.1/python/dna_parser/call_functions.py
+-rwxr-xr-x   0     1001      123      833 2023-05-25 19:09:16.000000 dna_parser-0.2.1/run-maturin-action.sh
+-rw-r--r--   0     1001      123     6761 2023-05-25 19:08:39.000000 dna_parser-0.2.1/src/cross.rs
+-rw-r--r--   0     1001      123     2730 2023-05-25 19:08:39.000000 dna_parser-0.2.1/src/fasta_files.rs
+-rw-r--r--   0     1001      123      426 2023-05-25 19:08:39.000000 dna_parser-0.2.1/src/kmers.rs
+-rw-r--r--   0     1001      123     1018 2023-05-25 19:08:39.000000 dna_parser-0.2.1/src/lib.rs
+-rw-r--r--   0     1001      123     6982 2023-05-25 19:08:39.000000 dna_parser-0.2.1/src/onehot.rs
+-rw-r--r--   0     1001      123     5989 2023-05-25 19:08:39.000000 dna_parser-0.2.1/src/ordinal.rs
+-rw-r--r--   0     1001      123     3434 2023-05-25 19:08:39.000000 dna_parser-0.2.1/src/random_sequence.rs
+-rw-r--r--   0     1001      123     3616 2023-05-25 19:08:39.000000 dna_parser-0.2.1/src/tfidf.rs
+-rw-r--r--   0     1001      123     1697 2023-05-25 19:08:39.000000 dna_parser-0.2.1/src/utils/mod.rs
+-rw-r--r--   0     1001      123    11845 2023-05-25 19:08:39.000000 dna_parser-0.2.1/Cargo.lock
+-rw-r--r--   0        0        0     5571 1970-01-01 00:00:00.000000 dna_parser-0.2.1/PKG-INFO
```

### Comparing `dna_parser-0.2.0/.github/workflows/CI.yml` & `dna_parser-0.2.1/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `dna_parser-0.2.0/.github/workflows/release.yml` & `dna_parser-0.2.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dna_parser-0.2.0/.gitignore` & `dna_parser-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dna_parser-0.2.0/LICENSE` & `dna_parser-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dna_parser-0.2.0/README.md` & `dna_parser-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `dna_parser-0.2.0/python/dna_parser/call_functions.py` & `dna_parser-0.2.1/python/dna_parser/call_functions.py`

 * *Files identical despite different names*

### Comparing `dna_parser-0.2.0/run-maturin-action.sh` & `dna_parser-0.2.1/run-maturin-action.sh`

 * *Files identical despite different names*

### Comparing `dna_parser-0.2.0/src/cross.rs` & `dna_parser-0.2.1/src/cross.rs`

 * *Files 0% similar despite different names*

```diff
@@ -113,27 +113,27 @@
             encoded_sequences.push(encoding);
             
         }
     }
 
     else if pad_type== "after" && vec_length == 0 {
 
-        for seq in chunk.into_iter(){
+        for seq in chunk.iter(){
 
             let seq_len = seq.len();
             let encoding= cross_after(seq, seq_len);
             
             encoded_sequences.push(encoding);
             
         }
     }
 
     else if pad_type== "before" && vec_length == 0 {
 
-        for seq in chunk.into_iter(){
+        for seq in chunk.iter(){
 
             let seq_len = seq.len();
             let encoding= cross_before(seq, seq_len);
             
             encoded_sequences.push(encoding);
             
         }
```

### Comparing `dna_parser-0.2.0/src/fasta_files.rs` & `dna_parser-0.2.1/src/fasta_files.rs`

 * *Files 11% similar despite different names*

```diff
@@ -18,32 +18,32 @@
     let mut sequences = Vec::new();
     let mut seq= String::from("");
 
     for line in f.lines(){
 
         let line = line.expect("Unable to read line");
 
-        if line.chars().nth(0).unwrap() == '>' {
+        if line.starts_with('>') {
             
-            if seq.len() > 0 {
+            if !seq.is_empty() {
 
                 sequences.push(seq);
                 seq= String::from("");
             }
         }
 
         else {
 
             seq.push_str(line.trim());
 
         }
 
     }
 
-    if seq.len() > 0 {
+    if !seq.is_empty() {
         sequences.push(seq);
     }
 
     sequences
 
 }
 
@@ -60,15 +60,15 @@
 
     let mut metadata = Vec::new();
 
     for line in f.lines() {
 
         let line = line.expect("Unable to read line");
 
-        if line.chars().nth(0).unwrap() == '>' {
+        if line.starts_with('>') {
 
             metadata.push(line)
         }
     }
 
     metadata 
 }
@@ -89,34 +89,34 @@
     let mut metadata= String::from("");
     let mut seq= String::from("");
 
     for line in reader.lines() {
 
         let line = line.expect("Unable to read line");
 
-        if line.chars().nth(0).unwrap() == '>' {
+        if line.starts_with('>') {
 
-            if seq.len() > 0 {
+            if !seq.is_empty() {
 
                 metadata_and_seq.push((metadata, seq));
                 seq= String::from("");
             }
 
-            metadata= String::from(line);
+            metadata= line;
         }
 
         else {
 
             seq.push_str(line.trim())
 
         }
 
     }
 
-    if seq.len() > 0 {
+    if !seq.is_empty() {
 
         metadata_and_seq.push((metadata, seq));
     }
 
     metadata_and_seq
```

### Comparing `dna_parser-0.2.0/src/lib.rs` & `dna_parser-0.2.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dna_parser-0.2.0/src/onehot.rs` & `dna_parser-0.2.1/src/onehot.rs`

 * *Files 1% similar despite different names*

```diff
@@ -110,27 +110,27 @@
             encoded_sequences.push(encoding);
             
         }
     }
 
     else if pad_type== "after" && vec_length == 0 {
 
-        for seq in chunk.into_iter(){
+        for seq in chunk.iter(){
 
             let seq_len = seq.len();
             let encoding= onehot_after(seq, seq_len);
             
             encoded_sequences.push(encoding);
             
         }
     }
 
     else if pad_type== "before" && vec_length == 0 {
 
-        for seq in chunk.into_iter(){
+        for seq in chunk.iter(){
 
             let seq_len = seq.len();
             let encoding= onehot_before(seq, seq_len);
             
             encoded_sequences.push(encoding);
             
         }
```

### Comparing `dna_parser-0.2.0/src/ordinal.rs` & `dna_parser-0.2.1/src/ordinal.rs`

 * *Files 2% similar despite different names*

```diff
@@ -109,27 +109,27 @@
             encoded_sequences.push(encoding);
             
         }
     }
 
     else if pad_type== "after" && vec_length == 0 {
 
-        for seq in chunk.into_iter(){
+        for seq in chunk.iter(){
 
             let seq_len = seq.len();
             let encoding= ordinal_after(seq, seq_len);
             
             encoded_sequences.push(encoding);
             
         }
     }
 
     else if pad_type== "before" && vec_length == 0 {
 
-        for seq in chunk.into_iter(){
+        for seq in chunk.iter(){
 
             let seq_len = seq.len();
             let encoding= ordinal_before(seq, seq_len);
             
             encoded_sequences.push(encoding);
             
         }
```

### Comparing `dna_parser-0.2.0/src/random_sequence.rs` & `dna_parser-0.2.1/src/random_sequence.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 use rand::seq::IteratorRandom;
 use pyo3::prelude::*;
 use std::sync::Mutex;
 use std::thread;
 use std::sync::Arc;
-use num_cpus;
+use crate::utils;
 
 /// Returns a randomly generate string representing a DNA sequence
 fn generate_dna_seq(length: i64) -> String {
 
     const NT_DNA: &str = "atgc";
     let mut rng = rand::thread_rng();
     let mut seq= String::from("");
@@ -80,55 +80,28 @@
         _ => panic!()
 
     }
 
     vec_of_seq
 }
 
-/// Returns the number of threads to use.
-/// 
-/// if n_jobs = 0; number of threads = number of cpus
-fn check_nb_cpus(n_jobs: i16) -> usize {
-
-    let nb_cpus;
-
-    if n_jobs == 0 {
-
-        nb_cpus= num_cpus::get_physical();
-    }
-
-    else if n_jobs < 0 {
-
-       panic!("Cannot have a negative number of cpu. Use 0 to use every cpus or input the number of desired cpus")
-
-    }
-
-    else {
-
-        nb_cpus= n_jobs as usize;
-    }
-
-    nb_cpus
-}
-
-
 
 /// Returns a Vec of strings representing a sequences
 ///
 /// This functions split the sequences to generate in different threads and collects them.
 ///
 /// # Arguments
 /// * `length` - Length of the sequences to generate
 /// * `nb_of_seq` - number of sequences to generate and store in the Vec
 /// * `seq_type` - either "dna", "rna" or "aa" (for amino acid)
 /// * `n_jobs` - number of threads to use. 0 to use every cpu in your machine
 #[pyfunction]
 pub fn random_seq_rust(length: i64, nb_of_seq: i64, seq_type: &str, n_jobs: i16) -> Vec<String>{
 
-    let cpu_to_use= check_nb_cpus(n_jobs);
+    let cpu_to_use= utils::check_nb_cpus(n_jobs);
 
     let results= Arc::new(Mutex::new(Vec::new()));
 
     let mut nb_of_threads_left= cpu_to_use;
 
     let mut nb_seq_left= nb_of_seq;
 
@@ -141,28 +114,28 @@
 
             if nb_of_threads_left == 1 {
 
                 seq_per_thread = nb_seq_left;
             }
 
             else {
-                nb_seq_left = nb_seq_left - seq_per_thread;
+                nb_seq_left -= seq_per_thread;
             }
 
 
             s.spawn({ let results= results.clone(); 
                  move|| {
                 
                 let  vec_of_seq = parse_type_seq(length, seq_per_thread, seq_type );
 
                 results.lock().unwrap().push(vec_of_seq);
                  }
             });
 
-            nb_of_threads_left = nb_of_threads_left -1;
+            nb_of_threads_left -= 1;
         }
 
     });
 
     let getter= results.lock().unwrap();
 
     let mut vec_to_return= Vec::new();
```

### Comparing `dna_parser-0.2.0/src/tfidf.rs` & `dna_parser-0.2.1/src/tfidf.rs`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 use std::collections::HashMap;
 use std::collections::HashSet;
 
 // create a struct? To be completed...
 
 /// Returns a tuple containing the Hashmap mapping each word with the number of time it appears and a Vec
 /// with the order in which the words were encountered in the corpus. 
-fn map_vocabulary(corpus: &Vec<String>) -> (HashMap<&str,f64>, Vec<&str>) {
+fn map_vocabulary(corpus: &[String]) -> (HashMap<&str,f64>, Vec<&str>) {
 
     let mut map= HashMap::new();
     let mut word_order= Vec::new();
     let mut words_set= HashSet::new();
 
     for seq in corpus.iter() {
 
@@ -35,15 +35,15 @@
 
     }
 
     (map,word_order)
 }
 
 /// Maps the number of time each word appears in the genomic sequence
-fn word_counts(sequence: &String) -> HashMap<&str,f64> {
+fn word_counts(sequence: &str) -> HashMap<&str,f64> {
 
     let mut counts= HashMap::new();
 
     for word in sequence.split_whitespace(){
 
         counts.entry(word).and_modify(|counter| *counter += 1.0).or_insert(1.0);
     }
@@ -90,15 +90,15 @@
 ///
 /// # Arguments
 /// * `length` - Length of the sequences to generate
 /// * `nb_of_seq` - number of sequences to generate and store in the Vec
 /// * `seq_type` - either "dna", "rna" or "aa" for amino acid
 /// * `n_jobs` - number of threads to use. 0 to use every cpu
 #[pyfunction]
-pub fn tfidf_encoding<'pyt>(py: Python <'pyt>, corpus: Vec<String>) -> &'pyt PyArray2<f64> {
+pub fn tfidf_encoding(py: Python, corpus: Vec<String>) -> &PyArray2<f64> {
 
     let word_map= map_vocabulary(&corpus);
     let nrows= corpus.len();
     let ncols= word_map.0.len();
 
     let mut matrix =Array2::<f64>::zeros((nrows,ncols));
 
@@ -107,14 +107,11 @@
         let seq_len= seq.split_whitespace().count() as f64;
         let counts= word_counts(seq);
 
         let tfidf_vec= compute_tfidf(seq_len, counts, &word_map);
         current_row.assign(&ArrayView::from(&tfidf_vec));
         
     }
-
-    
-    let py_array= matrix.into_pyarray(py);
-    py_array
-
-    
+  
+    matrix.into_pyarray(py)
+     
 }
```

### Comparing `dna_parser-0.2.0/Cargo.lock` & `dna_parser-0.2.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "dna_parser"
-version = "0.2.0"
+version = "0.2.1"
 dependencies = [
  "itertools",
  "num_cpus",
  "numpy",
  "pyo3",
  "rand",
 ]
```

### Comparing `dna_parser-0.2.0/PKG-INFO` & `dna_parser-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dna_parser
-Version: 0.2.0
+Version: 0.2.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: numpy >= 1.16.0
 License-File: LICENSE
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

