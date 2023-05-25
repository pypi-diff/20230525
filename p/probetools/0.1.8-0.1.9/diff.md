# Comparing `tmp/probetools-0.1.8.tar.gz` & `tmp/probetools-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "probetools-0.1.8.tar", last modified: Sat Feb 26 05:37:24 2022, max compression
+gzip compressed data, was "probetools-0.1.9.tar", last modified: Fri Mar  4 00:57:36 2022, max compression
```

## Comparing `probetools-0.1.8.tar` & `probetools-0.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 kevinkuchinski   (501) staff       (20)        0 2022-02-26 05:37:24.587390 probetools-0.1.8/
--rwxrwxrwx   0 kevinkuchinski   (501) staff       (20)     1072 2021-11-28 06:49:11.000000 probetools-0.1.8/LICENSE
--rw-r--r--   0 kevinkuchinski   (501) staff       (20)    11865 2022-02-26 05:37:24.587250 probetools-0.1.8/PKG-INFO
--rwxrwxrwx   0 kevinkuchinski   (501) staff       (20)    11237 2022-01-11 22:38:48.000000 probetools-0.1.8/README.md
--rwxrwxrwx   0 kevinkuchinski   (501) staff       (20)      104 2021-11-08 00:22:38.000000 probetools-0.1.8/pyproject.toml
--rw-r--r--   0 kevinkuchinski   (501) staff       (20)       38 2022-02-26 05:37:24.587427 probetools-0.1.8/setup.cfg
--rwxrwxrwx   0 kevinkuchinski   (501) staff       (20)     1007 2022-02-22 20:52:44.000000 probetools-0.1.8/setup.py
-drwxr-xr-x   0 kevinkuchinski   (501) staff       (20)        0 2022-02-26 05:37:24.585914 probetools-0.1.8/src/
-drwxr-xr-x   0 kevinkuchinski   (501) staff       (20)        0 2022-02-26 05:37:24.586542 probetools-0.1.8/src/probetools/
--rwxrwxrwx   0 kevinkuchinski   (501) staff       (20)        0 2021-11-28 09:37:34.000000 probetools-0.1.8/src/probetools/__init__.py
--rwxrwxrwx   0 kevinkuchinski   (501) staff       (20)    39129 2022-02-22 23:37:44.000000 probetools-0.1.8/src/probetools/probetools_v_0_1_8.py
-drwxr-xr-x   0 kevinkuchinski   (501) staff       (20)        0 2022-02-26 05:37:24.587098 probetools-0.1.8/src/probetools.egg-info/
--rw-r--r--   0 kevinkuchinski   (501) staff       (20)    11865 2022-02-26 05:37:24.000000 probetools-0.1.8/src/probetools.egg-info/PKG-INFO
--rw-r--r--   0 kevinkuchinski   (501) staff       (20)      298 2022-02-26 05:37:24.000000 probetools-0.1.8/src/probetools.egg-info/SOURCES.txt
--rw-r--r--   0 kevinkuchinski   (501) staff       (20)        1 2022-02-26 05:37:24.000000 probetools-0.1.8/src/probetools.egg-info/dependency_links.txt
--rw-r--r--   0 kevinkuchinski   (501) staff       (20)       66 2022-02-26 05:37:24.000000 probetools-0.1.8/src/probetools.egg-info/entry_points.txt
--rw-r--r--   0 kevinkuchinski   (501) staff       (20)       11 2022-02-26 05:37:24.000000 probetools-0.1.8/src/probetools.egg-info/top_level.txt
+drwxr-xr-x   0 kevinkuchinski   (501) staff       (20)        0 2022-03-04 00:57:36.509597 probetools-0.1.9/
+-rwxrwxrwx   0 kevinkuchinski   (501) staff       (20)     1072 2021-11-28 06:49:11.000000 probetools-0.1.9/LICENSE
+-rw-r--r--   0 kevinkuchinski   (501) staff       (20)    11981 2022-03-04 00:57:36.509463 probetools-0.1.9/PKG-INFO
+-rwxrwxrwx   0 kevinkuchinski   (501) staff       (20)    11353 2022-03-04 00:52:25.000000 probetools-0.1.9/README.md
+-rwxrwxrwx   0 kevinkuchinski   (501) staff       (20)      104 2021-11-08 00:22:38.000000 probetools-0.1.9/pyproject.toml
+-rw-r--r--   0 kevinkuchinski   (501) staff       (20)       38 2022-03-04 00:57:36.509631 probetools-0.1.9/setup.cfg
+-rwxrwxrwx   0 kevinkuchinski   (501) staff       (20)     1007 2022-03-04 00:51:39.000000 probetools-0.1.9/setup.py
+drwxr-xr-x   0 kevinkuchinski   (501) staff       (20)        0 2022-03-04 00:57:36.508074 probetools-0.1.9/src/
+drwxr-xr-x   0 kevinkuchinski   (501) staff       (20)        0 2022-03-04 00:57:36.508705 probetools-0.1.9/src/probetools/
+-rwxrwxrwx   0 kevinkuchinski   (501) staff       (20)        0 2021-11-28 09:37:34.000000 probetools-0.1.9/src/probetools/__init__.py
+-rwxrwxrwx   0 kevinkuchinski   (501) staff       (20)    39785 2022-03-04 00:51:16.000000 probetools-0.1.9/src/probetools/probetools_v_0_1_9.py
+drwxr-xr-x   0 kevinkuchinski   (501) staff       (20)        0 2022-03-04 00:57:36.509288 probetools-0.1.9/src/probetools.egg-info/
+-rw-r--r--   0 kevinkuchinski   (501) staff       (20)    11981 2022-03-04 00:57:36.000000 probetools-0.1.9/src/probetools.egg-info/PKG-INFO
+-rw-r--r--   0 kevinkuchinski   (501) staff       (20)      298 2022-03-04 00:57:36.000000 probetools-0.1.9/src/probetools.egg-info/SOURCES.txt
+-rw-r--r--   0 kevinkuchinski   (501) staff       (20)        1 2022-03-04 00:57:36.000000 probetools-0.1.9/src/probetools.egg-info/dependency_links.txt
+-rw-r--r--   0 kevinkuchinski   (501) staff       (20)       66 2022-03-04 00:57:36.000000 probetools-0.1.9/src/probetools.egg-info/entry_points.txt
+-rw-r--r--   0 kevinkuchinski   (501) staff       (20)       11 2022-03-04 00:57:36.000000 probetools-0.1.9/src/probetools.egg-info/top_level.txt
```

### Comparing `probetools-0.1.8/LICENSE` & `probetools-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `probetools-0.1.8/PKG-INFO` & `probetools-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: probetools
-Version: 0.1.8
+Version: 0.1.9
 Summary: Hybridization probe design for targeted genomic sequencing of diverse and hypervariable viral taxa
 Home-page: https://github.com/kevinkuchinski/probetools
 Author: Kevin Kuchinski
 Author-email: kevin.kuchinski@bccdc.ca
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/kevinkuchinski/probetools/issues
 Platform: UNKNOWN
@@ -146,15 +146,15 @@
 <b>Optional arguments:</b>
 
      -k : minimum sub-sequence length extracted, should be same as kmer length used for making probes (default=120, min=32)
      -D : minimum probe depth threshold used to define low coverage sub-sequences (default=0, min=0)
      -L : minimum number of consecutive bases below probe depth threshold to define a low coverage sub-sequence (default=40, min=1)
 
 ## stats
-Calculate and tabulate probe coverage statistics for target sequences. Overall target space statistics are provided in output_name_summary_report.tsv and statistics for each target sequence are provided in output_name_long_report.tsv.
+Calculate and tabulate probe coverage statistics for target sequences. Overall target space statistics are provided in output_name_summary_report.tsv and statistics for each target sequence are provided in output_name_long_report.tsv. Positions with degenerate bases do not count towards probe coverage calculations if they are not covered by probes.
 
 <b>Usage example:</b>
 ```
 $ probetools stats -i <input file> -o <output dir>/<output name>
 ```
 <b>Required arguments:</b>
```

### Comparing `probetools-0.1.8/README.md` & `probetools-0.1.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -129,15 +129,15 @@
 <b>Optional arguments:</b>
 
      -k : minimum sub-sequence length extracted, should be same as kmer length used for making probes (default=120, min=32)
      -D : minimum probe depth threshold used to define low coverage sub-sequences (default=0, min=0)
      -L : minimum number of consecutive bases below probe depth threshold to define a low coverage sub-sequence (default=40, min=1)
 
 ## stats
-Calculate and tabulate probe coverage statistics for target sequences. Overall target space statistics are provided in output_name_summary_report.tsv and statistics for each target sequence are provided in output_name_long_report.tsv.
+Calculate and tabulate probe coverage statistics for target sequences. Overall target space statistics are provided in output_name_summary_report.tsv and statistics for each target sequence are provided in output_name_long_report.tsv. Positions with degenerate bases do not count towards probe coverage calculations if they are not covered by probes.
 
 <b>Usage example:</b>
 ```
 $ probetools stats -i <input file> -o <output dir>/<output name>
 ```
 <b>Required arguments:</b>
```

### Comparing `probetools-0.1.8/setup.py` & `probetools-0.1.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="probetools",
-    version="0.1.8",
+    version="0.1.9",
     author="Kevin Kuchinski",
     author_email="kevin.kuchinski@bccdc.ca",
     description="Hybridization probe design for targeted genomic sequencing of diverse and hypervariable viral taxa",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kevinkuchinski/probetools",
     project_urls={
@@ -21,11 +21,11 @@
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     python_requires=">=3.7",
     entry_points={
     'console_scripts': [
-        'probetools = probetools.probetools_v_0_1_8:main',
+        'probetools = probetools.probetools_v_0_1_9:main',
     ],
     }
 )
```

### Comparing `probetools-0.1.8/src/probetools/probetools_v_0_1_8.py` & `probetools-0.1.9/src/probetools/probetools_v_0_1_9.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 
 import sys
 import subprocess
 import os
 
 
 def main():
-    version = '0.1.8'
+    version = '0.1.9'
     # Parse command line arguments
     module, args = parse_args(sys.argv, version)
     # Set path to output directory and name to append to output files
     out_path, name = os.path.split(args['-o'])
     out_path = '.' if out_path == '' else out_path
     # Make sure output directory exists
     if os.path.exists(out_path) == False and os.path.isdir(out_path) == False:
         print(f'\nERROR: Output path {out_path} does not exist.\n')
         exit(1)
     # Run top-level function for selected module
     if module == 'clusterkmers':
         print(f'\nProbeTools ClusterKmers v{version}')
         print('https://github.com/KevinKuchinski/ProbeTools\n')
-        cluster_kmers(out_path, name, args['-t'], args['-k'], args['-i'], args['-s'], args['-p'], args['-n'], args['-T'])
+        cluster_kmers(out_path, name, args['-t'], args['-k'], args['-i'], args['-s'], args['-d'], args['-p'], args['-n'], args['-T'])
     elif module == 'capture':
         print(f'\nProbeTools Capture v{version}')
         print('https://github.com/KevinKuchinski/ProbeTools\n')
         capture(out_path, name, args['-t'], args['-p'], args['-i'], args['-l'], args['-T'])
     elif module == 'getlowcov':
         print(f'\nProbeTools GetLowCov v{version}')
         print('https://github.com/KevinKuchinski/ProbeTools\n')
@@ -33,15 +33,15 @@
     elif module == 'stats':
         print(f'\nProbeTools Stats v{version}')
         print('https://github.com/KevinKuchinski/ProbeTools\n')
         stats(out_path, name, args['-i'])
     elif module == 'makeprobes':
         print(f'\nProbeTools MakeProbes v{version}')
         print('https://github.com/KevinKuchinski/ProbeTools\n')
-        make_probes(out_path, name, args['-t'], args['-b'], args['-m'], args['-c'], args['-k'], args['-i'], args['-s'], 
+        make_probes(out_path, name, args['-t'], args['-b'], args['-m'], args['-c'], args['-k'], args['-i'], args['-s'], args['-d'], 
                     args['-D'], args['-L'], args['-i'], args['-l'], args['-T'])
     elif module == 'merge':
         print(f'\nProbeTools Merge v{version}')
         print('https://github.com/KevinKuchinski/ProbeTools\n')
         merge(args['-i'], args['-I'], args['-o'])
     print('\nDone.\n')
     exit(0)
@@ -287,18 +287,18 @@
         for line in input_file:
             output_file.write(line)
     # GARBAGE COLLECTION - Delete new FASTA file after contents have been appended
     os.remove(new_fasta_path)
 
 
 ######### Top-level functions for modules ##########
-def cluster_kmers(out_path, name, targets_path, k, cluster_id, step, prev_probes_path, num_probes, threads):
+def cluster_kmers(out_path, name, targets_path, k, cluster_id, step, max_degen, prev_probes_path, num_probes, threads):
     check_input([targets_path])
     kmers_path = os.path.join(out_path, name + '_kmers.fa')
-    enum_kmers(targets_path, kmers_path, k, step)
+    enum_kmers(targets_path, kmers_path, k, step, max_degen)
     centroids_path = os.path.join(out_path, name + '_centroids.fa')
     cluster_kmers_with_VSEARCH(kmers_path, centroids_path, cluster_id, threads)
     remove_prev_probes(centroids_path, prev_probes_path)
     probe_names, probe_seqs = rank_probe_candidates(centroids_path)
     probes_path = os.path.join(out_path, name + '_probes.fa')
     potential_probes, probes_writen = write_top_probes(probe_names, probe_seqs, num_probes, probes_path, name)
     return potential_probes, probes_writen
@@ -327,15 +327,15 @@
     capture_data = load_capture_data(capture_path)
     report_path = os.path.join(out_path, name + '_summary_stats_report.tsv')
     write_summary_report(capture_data, report_path, name)
     report_path = os.path.join(out_path, name + '_long_stats_report.tsv')
     write_long_report(capture_data, report_path, name)
 
 
-def make_probes(out_path, name, targets_path, batch_size, max_probes, cov_target, k, cluster_id, step,
+def make_probes(out_path, name, targets_path, batch_size, max_probes, cov_target, k, cluster_id, step, max_degen,
                 min_depth, min_low_cov_length, min_id, min_capture_length, threads):
     check_input([targets_path])
     # Set variable for counting rounds of incremental probe design
     round_counter = 0
     # Initialize variables for panel size (# probes) and 10th percentile of panel coverage
     panel_size, panel_cov = 0, 0
     # If panel size is not specified, set max_panel_size as 1 probe larger than current panel size so loop doesn't break
@@ -357,15 +357,15 @@
         print()
         # Break design loop if no low seqs were writen
         if seqs_writen == 0:
             break
         # Make probes from target space
         num_probes = min(batch_size, max_panel_size - panel_size)
         round_name = name + f'_round_{round_counter}'
-        potential_probes, probes_writen = cluster_kmers(out_path, round_name, low_cov_path, k, cluster_id, step, final_probes_path, num_probes, threads)
+        potential_probes, probes_writen = cluster_kmers(out_path, round_name, low_cov_path, k, cluster_id, step, max_degen, final_probes_path, num_probes, threads)
         print()
         # GARBAGE COLLECTION - Delete low cov seqs
         os.remove(low_cov_path)
         # Update panel size and max panel size
         panel_size += probes_writen
         max_panel_size = panel_size + batch_size if max_probes == 'MAX' else max_probes
         # Break design loop if no potential probes or no probes writen
@@ -402,15 +402,15 @@
     capture_data = load_capture_data(capture_path)
     other_capture_data = load_capture_data(other_capture_path)
     merged_capture_data = merge_capture_results(capture_data, other_capture_data)
     write_capture_data(merged_capture_path, merged_capture_data)
 
 
 ########## clusterkmers functions ##########
-def enum_kmers(targets_path, kmers_path, k, step):
+def enum_kmers(targets_path, kmers_path, k, step, max_degen):
     print(f'Enumerating all {k}-mers in {targets_path}...')
     # Load contents of targets FASTA
     headers, seqs = load_fasta(targets_path)
     print(f' Loaded {"{:,}".format(len(seqs))} target seqs in {targets_path}...')
     # Create FASTA file for kmers output and enumerate kmers from target seqs
     with open(kmers_path, 'w') as output_file:
         target_counter = 0
@@ -419,17 +419,20 @@
             if seq == '':
                 print(f' WARNING --- Target {header} has no sequence!')
             elif len(seq) < k:
                 print(f' WARNING --- Target {header} is shorter than the desired probe length!')
             elif len(seq) >= k and seq != '':
                 target_counter += 1
                 for i in range(0, len(seq) - k + 1, step):
-                    kmer_counter += 1
-                    output_file.write(f'>kmer_{kmer_counter}\n')
-                    output_file.write(seq[i:i+k] + '\n')
+                    kmer = seq[i:i+k]
+                    num_degen = len(kmer) - sum(kmer.count(base) for base in 'ATGC')
+                    if num_degen <= max_degen:
+                        kmer_counter += 1
+                        output_file.write(f'>kmer_{kmer_counter}\n')
+                        output_file.write(kmer + '\n')
     print(f' Enumerated {"{:,}".format(kmer_counter)} k-mers from {targets_path}.')
 
 
 def cluster_kmers_with_VSEARCH(kmers_path, centroids_path, cluster_id, threads):
     print(f' Clustering k-mers at {cluster_id}% identity...')
     # Create and run terminal command for VSEARCH
     terminal_command = (f'vsearch --cluster_fast {kmers_path} --id {cluster_id / 100} --centroids {centroids_path}'
@@ -666,20 +669,36 @@
                     low_cov_start = low_cov_end
     print(f' Wrote {total_low_cov_counter} low coverage seqs from {"{:,}".format(len(capture_data))} targets.')
     seqs_writen = total_low_cov_counter
     return seqs_writen
 
 
 ########## stats functions ##########
+def calc_cov_at_depth(seq, depth, min_depth):
+    covered_bases = 0
+    total_bases = 0
+    for base, base_depth in zip(seq, depth):
+        if base_depth >= min_depth:
+            covered_bases += 1
+            total_bases += 1
+        elif base in 'ATGC':
+            total_bases += 1
+    if total_bases == 0:
+        coverage = 0
+    else:
+        coverage = covered_bases * 100 / total_bases
+    return coverage
+
+
 def calc_cov_percentiles(capture_data, percentiles=(0, 0.05, 0.1, 0.25, 0.5, 0.75, 1)):
     """Takes a capture dict and tuple of perentiles, and returns a list of those percentile
     values."""
     cov_values = []
     for header, (seq, depth) in capture_data.items():
-        cov_values.append((len(depth) - depth.count(0)) * 100 / len(depth))
+        cov_values.append(calc_cov_at_depth(seq, depth, 1))
     cov_values = sorted(cov_values)
     percentile_values = []
     for percentile in percentiles:
         values_under_percentile = (len(cov_values) - 1) * percentile
         if values_under_percentile == int(values_under_percentile):
             percentile_values.append(cov_values[int(values_under_percentile)])
         else:
@@ -741,14 +760,15 @@
         output_file.write('\t'.join(header) + '\n')
         for header, (seq, depth) in capture_data.items():
             total_ATGC = len([s for s in seq if s in 'ATGC'])
             length = len(depth)
             line = [name, header, str(length), str(total_ATGC), str(round(total_ATGC * 100 / length, 2))]
             line += [str(depth.count(d)) for d in [0, 1, 2, 3, 4]]
             line += [str(len([d for d in depth if d >= 5]))]
-            line += [str(round(len([d for d in depth if d >= dd]) * 100 / length, 1)) for dd in [1, 2, 3, 4, 5]]
+            line += [str(round(calc_cov_at_depth(seq, depth, min_depth), 1)) for min_depth in [1, 2, 3, 4, 5]]
             output_file.write('\t'.join(line) + '\n')
 
 
 ######### call main function ##########
 if __name__ == '__main__':
     main()
+
```

### Comparing `probetools-0.1.8/src/probetools.egg-info/PKG-INFO` & `probetools-0.1.9/src/probetools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: probetools
-Version: 0.1.8
+Version: 0.1.9
 Summary: Hybridization probe design for targeted genomic sequencing of diverse and hypervariable viral taxa
 Home-page: https://github.com/kevinkuchinski/probetools
 Author: Kevin Kuchinski
 Author-email: kevin.kuchinski@bccdc.ca
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/kevinkuchinski/probetools/issues
 Platform: UNKNOWN
@@ -146,15 +146,15 @@
 <b>Optional arguments:</b>
 
      -k : minimum sub-sequence length extracted, should be same as kmer length used for making probes (default=120, min=32)
      -D : minimum probe depth threshold used to define low coverage sub-sequences (default=0, min=0)
      -L : minimum number of consecutive bases below probe depth threshold to define a low coverage sub-sequence (default=40, min=1)
 
 ## stats
-Calculate and tabulate probe coverage statistics for target sequences. Overall target space statistics are provided in output_name_summary_report.tsv and statistics for each target sequence are provided in output_name_long_report.tsv.
+Calculate and tabulate probe coverage statistics for target sequences. Overall target space statistics are provided in output_name_summary_report.tsv and statistics for each target sequence are provided in output_name_long_report.tsv. Positions with degenerate bases do not count towards probe coverage calculations if they are not covered by probes.
 
 <b>Usage example:</b>
 ```
 $ probetools stats -i <input file> -o <output dir>/<output name>
 ```
 <b>Required arguments:</b>
```

