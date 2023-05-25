# Comparing `tmp/primerJinn-0.1.3.dev1.tar.gz` & `tmp/primerJinn-0.1.5.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "primerJinn-0.1.3.dev1.tar", last modified: Tue May 23 20:34:54 2023, max compression
+gzip compressed data, was "primerJinn-0.1.5.dev1.tar", last modified: Thu May 25 18:29:24 2023, max compression
```

## Comparing `primerJinn-0.1.3.dev1.tar` & `primerJinn-0.1.5.dev1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 semiquant   (502) staff       (20)        0 2023-05-23 20:34:54.437572 primerJinn-0.1.3.dev1/
--rw-r--r--   0 semiquant   (502) staff       (20)    10988 2023-05-23 20:34:54.437273 primerJinn-0.1.3.dev1/PKG-INFO
--rw-r--r--   0 semiquant   (502) staff       (20)    10559 2023-05-23 20:30:00.000000 primerJinn-0.1.3.dev1/README.md
-drwxr-xr-x   0 semiquant   (502) staff       (20)        0 2023-05-23 20:34:54.437083 primerJinn-0.1.3.dev1/primerJinn.egg-info/
--rw-r--r--   0 semiquant   (502) staff       (20)    10988 2023-05-23 20:34:54.000000 primerJinn-0.1.3.dev1/primerJinn.egg-info/PKG-INFO
--rw-r--r--   0 semiquant   (502) staff       (20)      224 2023-05-23 20:34:54.000000 primerJinn-0.1.3.dev1/primerJinn.egg-info/SOURCES.txt
--rw-r--r--   0 semiquant   (502) staff       (20)        1 2023-05-23 20:34:54.000000 primerJinn-0.1.3.dev1/primerJinn.egg-info/dependency_links.txt
--rw-r--r--   0 semiquant   (502) staff       (20)      162 2023-05-23 20:34:54.000000 primerJinn-0.1.3.dev1/primerJinn.egg-info/entry_points.txt
--rw-r--r--   0 semiquant   (502) staff       (20)       71 2023-05-23 20:34:54.000000 primerJinn-0.1.3.dev1/primerJinn.egg-info/requires.txt
--rw-r--r--   0 semiquant   (502) staff       (20)        1 2023-05-23 20:34:54.000000 primerJinn-0.1.3.dev1/primerJinn.egg-info/top_level.txt
--rw-r--r--   0 semiquant   (502) staff       (20)       38 2023-05-23 20:34:54.437621 primerJinn-0.1.3.dev1/setup.cfg
--rw-r--r--   0 semiquant   (502) staff       (20)     1697 2023-05-23 20:34:36.000000 primerJinn-0.1.3.dev1/setup.py
+drwxr-xr-x   0 semiquant   (502) staff       (20)        0 2023-05-25 18:29:24.882906 primerJinn-0.1.5.dev1/
+-rw-r--r--   0 semiquant   (502) staff       (20)    10982 2023-05-25 18:29:24.882661 primerJinn-0.1.5.dev1/PKG-INFO
+-rw-r--r--   0 semiquant   (502) staff       (20)    10553 2023-05-24 21:35:04.000000 primerJinn-0.1.5.dev1/README.md
+drwxr-xr-x   0 semiquant   (502) staff       (20)        0 2023-05-25 18:29:24.882455 primerJinn-0.1.5.dev1/primerJinn.egg-info/
+-rw-r--r--   0 semiquant   (502) staff       (20)    10982 2023-05-25 18:29:24.000000 primerJinn-0.1.5.dev1/primerJinn.egg-info/PKG-INFO
+-rw-r--r--   0 semiquant   (502) staff       (20)      224 2023-05-25 18:29:24.000000 primerJinn-0.1.5.dev1/primerJinn.egg-info/SOURCES.txt
+-rw-r--r--   0 semiquant   (502) staff       (20)        1 2023-05-25 18:29:24.000000 primerJinn-0.1.5.dev1/primerJinn.egg-info/dependency_links.txt
+-rw-r--r--   0 semiquant   (502) staff       (20)      162 2023-05-25 18:29:24.000000 primerJinn-0.1.5.dev1/primerJinn.egg-info/entry_points.txt
+-rw-r--r--   0 semiquant   (502) staff       (20)       71 2023-05-25 18:29:24.000000 primerJinn-0.1.5.dev1/primerJinn.egg-info/requires.txt
+-rw-r--r--   0 semiquant   (502) staff       (20)        1 2023-05-25 18:29:24.000000 primerJinn-0.1.5.dev1/primerJinn.egg-info/top_level.txt
+-rw-r--r--   0 semiquant   (502) staff       (20)       38 2023-05-25 18:29:24.882957 primerJinn-0.1.5.dev1/setup.cfg
+-rw-r--r--   0 semiquant   (502) staff       (20)     1697 2023-05-23 21:36:38.000000 primerJinn-0.1.5.dev1/setup.py
```

### Comparing `primerJinn-0.1.3.dev1/PKG-INFO` & `primerJinn-0.1.5.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: primerJinn
-Version: 0.1.3.dev1
+Version: 0.1.5.dev1
 Summary: In silico PCR tool
 Home-page: https://github.com/SemiQuant/primerJinn
 Author: Jason D Limberis
 Author-email: Jason.Limberis@ucsf.edu
 License: MIT
 Keywords: PCR,in silico PCR
 Classifier: Programming Language :: Python :: 3
@@ -33,15 +33,15 @@
 | **primer design** | N            | product_size_min   | The desired min size for the PCR product.                                                                                                                                 | 400                                     |
 | **primer design** | N            | product_size_max   | The desired max size for the PCR product.                                                                                                                                 | 800                                     |
 | **primer design** | N            | ret                | The maximum number of primer pairs to return                                                                                                                              | 100                                     |
 | **primer design** | N            | Q5                 | A boolean indicating whether to use NEB Q5 hotstart polymerase settings for primer3                                                                                       | TRUE                                    |
 | **primer design** | N            | background         | The path to the mispriming library FASTA file                                                                                                                             |                                         |
 | **primer design** | N            | ill_adapt         | Add Illumina partial adapters                                                                                                                              | FALSE                                         |
 | **primer design** | N            | clamp         | Require GC clamp                                                                                                                               | 0                                         |
-| **primer design** | N            | clamp         | Maximum allowable length of a mononucleotide repeat (poly-X) in the primer sequence                                                                                                                               | 3                                         |
+| **primer design** | N            | poly         | Maximum allowable length of a mononucleotide repeat (poly-X) in the primer sequence                                                                                                                               | 3                                         |
 | **in silico PCR** | N            | product_size_max   | Maximum length of PCR products in nucleotides.                                                                                                                            | 2000                                    |
 | **in silico PCR** | N            | req_five           | Require the 5' end of the primer to bind?                                                                                                                                 | TRUE                                    |
 
 
 ### Dependencies
 
 -   Python 3
@@ -85,15 +85,15 @@
 
 ### PCR in silico example usage
 
 ```
 PCRinSilico \
    --primer_seq ./example/primers.txt \
    --target_tm 50 \
-   --ref_fasta_file  ./example/ref.fasta
+   --input_file ./example/ref.fasta
 ```
 
 #### in_silico_PCR.tsv
 | qseq1 | qseq1_input          | qstart1 | qend1 | direction1 | mismatch1 | qseq2 | qseq2_input          | qstart2 | qend2 | direction2 | mismatch2 | binding_pos_diff | reference   | ref_region |         |
 |-------|----------------------|---------|-------|------------|-----------|-------|----------------------|---------|-------|------------|-----------|------------------|-------------|------------|---------|
 | p1    | GAGGAACACCACTAGTACCG | 1       | 20    | +          | 0         | p9    | CTCGATGACTTTACGGCCAT | 1       | 20    | -          | 0         | 655              | NC_000962.3 | 1461637    | 1460982 |
 | p2    | CATGGGATATGGAGCGATCG | 1       | 20    | +          | 0         | p10   | GGGGTCGTAGGAGATCTTGA | 1       | 20    | -          | 0         | 771              | NC_000962.3 | 491474     | 490703  |
```

### Comparing `primerJinn-0.1.3.dev1/README.md` & `primerJinn-0.1.5.dev1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 | **primer design** | N            | product_size_min   | The desired min size for the PCR product.                                                                                                                                 | 400                                     |
 | **primer design** | N            | product_size_max   | The desired max size for the PCR product.                                                                                                                                 | 800                                     |
 | **primer design** | N            | ret                | The maximum number of primer pairs to return                                                                                                                              | 100                                     |
 | **primer design** | N            | Q5                 | A boolean indicating whether to use NEB Q5 hotstart polymerase settings for primer3                                                                                       | TRUE                                    |
 | **primer design** | N            | background         | The path to the mispriming library FASTA file                                                                                                                             |                                         |
 | **primer design** | N            | ill_adapt         | Add Illumina partial adapters                                                                                                                              | FALSE                                         |
 | **primer design** | N            | clamp         | Require GC clamp                                                                                                                               | 0                                         |
-| **primer design** | N            | clamp         | Maximum allowable length of a mononucleotide repeat (poly-X) in the primer sequence                                                                                                                               | 3                                         |
+| **primer design** | N            | poly         | Maximum allowable length of a mononucleotide repeat (poly-X) in the primer sequence                                                                                                                               | 3                                         |
 | **in silico PCR** | N            | product_size_max   | Maximum length of PCR products in nucleotides.                                                                                                                            | 2000                                    |
 | **in silico PCR** | N            | req_five           | Require the 5' end of the primer to bind?                                                                                                                                 | TRUE                                    |
 
 
 ### Dependencies
 
 -   Python 3
@@ -71,15 +71,15 @@
 
 ### PCR in silico example usage
 
 ```
 PCRinSilico \
    --primer_seq ./example/primers.txt \
    --target_tm 50 \
-   --ref_fasta_file  ./example/ref.fasta
+   --input_file ./example/ref.fasta
 ```
 
 #### in_silico_PCR.tsv
 | qseq1 | qseq1_input          | qstart1 | qend1 | direction1 | mismatch1 | qseq2 | qseq2_input          | qstart2 | qend2 | direction2 | mismatch2 | binding_pos_diff | reference   | ref_region |         |
 |-------|----------------------|---------|-------|------------|-----------|-------|----------------------|---------|-------|------------|-----------|------------------|-------------|------------|---------|
 | p1    | GAGGAACACCACTAGTACCG | 1       | 20    | +          | 0         | p9    | CTCGATGACTTTACGGCCAT | 1       | 20    | -          | 0         | 655              | NC_000962.3 | 1461637    | 1460982 |
 | p2    | CATGGGATATGGAGCGATCG | 1       | 20    | +          | 0         | p10   | GGGGTCGTAGGAGATCTTGA | 1       | 20    | -          | 0         | 771              | NC_000962.3 | 491474     | 490703  |
```

### Comparing `primerJinn-0.1.3.dev1/primerJinn.egg-info/PKG-INFO` & `primerJinn-0.1.5.dev1/primerJinn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: primerJinn
-Version: 0.1.3.dev1
+Version: 0.1.5.dev1
 Summary: In silico PCR tool
 Home-page: https://github.com/SemiQuant/primerJinn
 Author: Jason D Limberis
 Author-email: Jason.Limberis@ucsf.edu
 License: MIT
 Keywords: PCR,in silico PCR
 Classifier: Programming Language :: Python :: 3
@@ -33,15 +33,15 @@
 | **primer design** | N            | product_size_min   | The desired min size for the PCR product.                                                                                                                                 | 400                                     |
 | **primer design** | N            | product_size_max   | The desired max size for the PCR product.                                                                                                                                 | 800                                     |
 | **primer design** | N            | ret                | The maximum number of primer pairs to return                                                                                                                              | 100                                     |
 | **primer design** | N            | Q5                 | A boolean indicating whether to use NEB Q5 hotstart polymerase settings for primer3                                                                                       | TRUE                                    |
 | **primer design** | N            | background         | The path to the mispriming library FASTA file                                                                                                                             |                                         |
 | **primer design** | N            | ill_adapt         | Add Illumina partial adapters                                                                                                                              | FALSE                                         |
 | **primer design** | N            | clamp         | Require GC clamp                                                                                                                               | 0                                         |
-| **primer design** | N            | clamp         | Maximum allowable length of a mononucleotide repeat (poly-X) in the primer sequence                                                                                                                               | 3                                         |
+| **primer design** | N            | poly         | Maximum allowable length of a mononucleotide repeat (poly-X) in the primer sequence                                                                                                                               | 3                                         |
 | **in silico PCR** | N            | product_size_max   | Maximum length of PCR products in nucleotides.                                                                                                                            | 2000                                    |
 | **in silico PCR** | N            | req_five           | Require the 5' end of the primer to bind?                                                                                                                                 | TRUE                                    |
 
 
 ### Dependencies
 
 -   Python 3
@@ -85,15 +85,15 @@
 
 ### PCR in silico example usage
 
 ```
 PCRinSilico \
    --primer_seq ./example/primers.txt \
    --target_tm 50 \
-   --ref_fasta_file  ./example/ref.fasta
+   --input_file ./example/ref.fasta
 ```
 
 #### in_silico_PCR.tsv
 | qseq1 | qseq1_input          | qstart1 | qend1 | direction1 | mismatch1 | qseq2 | qseq2_input          | qstart2 | qend2 | direction2 | mismatch2 | binding_pos_diff | reference   | ref_region |         |
 |-------|----------------------|---------|-------|------------|-----------|-------|----------------------|---------|-------|------------|-----------|------------------|-------------|------------|---------|
 | p1    | GAGGAACACCACTAGTACCG | 1       | 20    | +          | 0         | p9    | CTCGATGACTTTACGGCCAT | 1       | 20    | -          | 0         | 655              | NC_000962.3 | 1461637    | 1460982 |
 | p2    | CATGGGATATGGAGCGATCG | 1       | 20    | +          | 0         | p10   | GGGGTCGTAGGAGATCTTGA | 1       | 20    | -          | 0         | 771              | NC_000962.3 | 491474     | 490703  |
```

### Comparing `primerJinn-0.1.3.dev1/setup.py` & `primerJinn-0.1.5.dev1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         os.system("wget https://ftp.ncbi.nlm.nih.gov/blast/executables/blast+/2.14.0/ncbi-blast-2.14.0+-x64-linux.tar.gz")
         os.system("tar -xzvf ncbi-blast-2.14.0+-x64-linux.tar.gz")
         os.system("export PATH=$PATH:%s" % os.path.abspath("$(pwd)/ncbi-blast-2.14.0+/bin"))
 
 
 setup(
     name='primerJinn',
-    version='0.1.3.dev1',
+    version='0.1.5.dev1',
     url='https://github.com/SemiQuant/primerJinn',
     install_requires=dependencies,
     description='In silico PCR tool',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Jason D Limberis',
     author_email='Jason.Limberis@ucsf.edu',
```

