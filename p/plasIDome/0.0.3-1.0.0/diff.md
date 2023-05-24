# Comparing `tmp/plasIDome-0.0.3.tar.gz` & `tmp/plasIDome-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/hendrixj/Dropbox/subDrop/plasIDome/dist/.tmp-6fa0s7zm/plasIDome-0.0.3.tar", last modified: Fri Nov 25 23:04:18 2022, max compression
+gzip compressed data, was "/Users/hendrixj/Dropbox/subDrop/plasIDome/plasIDome_pypi/dist/.tmp-ucdf1_dm/plasIDome-1.0.0.tar", last modified: Wed May 24 23:38:18 2023, max compression
```

## Comparing `plasIDome-0.0.3.tar` & `plasIDome-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 hendrixj (1692218720) 1934156310        0 2022-11-25 23:04:18.497965 plasIDome-0.0.3/
--rw-r--r--   0 hendrixj (1692218720) 1934156310     1122 2022-10-08 19:49:45.000000 plasIDome-0.0.3/LICENSE
--rw-r--r--   0 hendrixj (1692218720) 1934156310       17 2022-10-10 23:15:11.000000 plasIDome-0.0.3/MANIFEST.in
--rw-r--r--   0 hendrixj (1692218720) 1934156310     3132 2022-11-25 23:04:18.498129 plasIDome-0.0.3/PKG-INFO
--rwxr--r--   0 hendrixj (1692218720) 1934156310     2645 2022-11-25 19:45:49.000000 plasIDome-0.0.3/README.md
-drwxr-xr-x   0 hendrixj (1692218720) 1934156310        0 2022-11-25 23:04:18.495429 plasIDome-0.0.3/bin/
--rw-r--r--   0 hendrixj (1692218720) 1934156310     7542 2022-11-25 23:03:24.000000 plasIDome-0.0.3/bin/plasIDome
-drwxr-xr-x   0 hendrixj (1692218720) 1934156310        0 2022-11-25 23:04:18.497637 plasIDome-0.0.3/plasIDome.egg-info/
--rw-r--r--   0 hendrixj (1692218720) 1934156310     3132 2022-11-25 23:04:18.000000 plasIDome-0.0.3/plasIDome.egg-info/PKG-INFO
--rw-r--r--   0 hendrixj (1692218720) 1934156310      226 2022-11-25 23:04:18.000000 plasIDome-0.0.3/plasIDome.egg-info/SOURCES.txt
--rw-r--r--   0 hendrixj (1692218720) 1934156310        1 2022-11-25 23:04:18.000000 plasIDome-0.0.3/plasIDome.egg-info/dependency_links.txt
--rw-r--r--   0 hendrixj (1692218720) 1934156310       10 2022-11-25 23:04:18.000000 plasIDome-0.0.3/plasIDome.egg-info/requires.txt
--rw-r--r--   0 hendrixj (1692218720) 1934156310        1 2022-11-25 23:04:18.000000 plasIDome-0.0.3/plasIDome.egg-info/top_level.txt
--rw-r--r--   0 hendrixj (1692218720) 1934156310       38 2022-11-25 23:04:18.498725 plasIDome-0.0.3/setup.cfg
--rw-r--r--   0 hendrixj (1692218720) 1934156310      800 2022-11-25 23:03:54.000000 plasIDome-0.0.3/setup.py
+drwxr-xr-x   0 hendrixj (1692218720) NATJ\Domain Users (1934156310)        0 2023-05-24 23:38:18.107432 plasIDome-1.0.0/
+-rw-r--r--   0 hendrixj (1692218720) NATJ\Domain Users (1934156310)     1122 2022-11-22 17:50:10.000000 plasIDome-1.0.0/LICENSE
+-rw-r--r--   0 hendrixj (1692218720) NATJ\Domain Users (1934156310)       17 2022-11-22 17:50:10.000000 plasIDome-1.0.0/MANIFEST.in
+-rw-r--r--   0 hendrixj (1692218720) NATJ\Domain Users (1934156310)     3132 2023-05-24 23:38:18.107584 plasIDome-1.0.0/PKG-INFO
+-rwxr--r--   0 hendrixj (1692218720) NATJ\Domain Users (1934156310)     2645 2022-11-25 19:45:49.000000 plasIDome-1.0.0/README.md
+drwxr-xr-x   0 hendrixj (1692218720) NATJ\Domain Users (1934156310)        0 2023-05-24 23:38:18.104304 plasIDome-1.0.0/bin/
+-rw-r--r--   0 hendrixj (1692218720) NATJ\Domain Users (1934156310)     8089 2023-05-24 23:33:51.000000 plasIDome-1.0.0/bin/plasIDome
+drwxr-xr-x   0 hendrixj (1692218720) NATJ\Domain Users (1934156310)        0 2023-05-24 23:38:18.107101 plasIDome-1.0.0/plasIDome.egg-info/
+-rw-r--r--   0 hendrixj (1692218720) NATJ\Domain Users (1934156310)     3132 2023-05-24 23:38:17.000000 plasIDome-1.0.0/plasIDome.egg-info/PKG-INFO
+-rw-r--r--   0 hendrixj (1692218720) NATJ\Domain Users (1934156310)      226 2023-05-24 23:38:17.000000 plasIDome-1.0.0/plasIDome.egg-info/SOURCES.txt
+-rw-r--r--   0 hendrixj (1692218720) NATJ\Domain Users (1934156310)        1 2023-05-24 23:38:17.000000 plasIDome-1.0.0/plasIDome.egg-info/dependency_links.txt
+-rw-r--r--   0 hendrixj (1692218720) NATJ\Domain Users (1934156310)       10 2023-05-24 23:38:17.000000 plasIDome-1.0.0/plasIDome.egg-info/requires.txt
+-rw-r--r--   0 hendrixj (1692218720) NATJ\Domain Users (1934156310)        1 2023-05-24 23:38:17.000000 plasIDome-1.0.0/plasIDome.egg-info/top_level.txt
+-rw-r--r--   0 hendrixj (1692218720) NATJ\Domain Users (1934156310)       38 2023-05-24 23:38:18.108139 plasIDome-1.0.0/setup.cfg
+-rw-r--r--   0 hendrixj (1692218720) NATJ\Domain Users (1934156310)      800 2023-05-24 23:37:55.000000 plasIDome-1.0.0/setup.py
```

### Comparing `plasIDome-0.0.3/LICENSE` & `plasIDome-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `plasIDome-0.0.3/PKG-INFO` & `plasIDome-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plasIDome
-Version: 0.0.3
+Version: 1.0.0
 Summary: A tool to detect plasmids and contamination in bacterial and archaeal genome assemblies
 Home-page: https://github.com/jrhendrix/plasIDome
 Author: Jo Hendrix
 Author-email: jrhendrix36@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `plasIDome-0.0.3/README.md` & `plasIDome-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `plasIDome-0.0.3/bin/plasIDome` & `plasIDome-1.0.0/bin/plasIDome`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-
 '''
 FILE:	plasIDome
 AUTHOR:	J.R. Hendrix
 URL: 	http://stronglab.org
 		https://github.com/jrhendrix/plasIDome
 DESC:	This script extracts contigs less than a certain length 
 		and aligns the sequence using blastn
@@ -161,39 +160,42 @@
 def main(program):
 	''' The main worker function to dictate processes '''
 
 	cwd = os.getcwd()
 
 	# PARSER : ROOT
 	parent_parser = argparse.ArgumentParser(prog='plasidome')
-	parent_parser.add_argument('-b', '--blastn_path', help='Path to blastn', required=True)
+	parent_parser.add_argument('-b', '--blastn_path', default="/Strong/proj/shared_code/ncbi-blast-2.10.1+/bin/blastn", help='Path to blastn')
 	parent_parser.add_argument('-f', '--fasta_input', help='Path to fasta file')
 	parent_parser.add_argument('-l', '--length', default=200000, help='Contigs shorter than this length will be tested', type=int)
 	parent_parser.add_argument('-o', '--out_directory', default="contig_assignments", help='Prefix of output directory', type=str)
 	parent_parser.add_argument('-p', '--path_to_output',  default=cwd, help='Path to output', type=str)
 	parent_parser.add_argument('-r', '--report_file', default='report', help='Name of output summary report')
 
 	args = parent_parser.parse_args()
 
+	
 	# CREATE OUTPUT STRUCTURE
 	try:
 		TOP_DIR = Dir(args.path_to_output)
 		BASEDIR = TOP_DIR.make_subdir(args.out_directory)
 	except IOError:
 		print('ERROR: could not establish output directory.')
 
 	# GET CONTIGS THAT MET LENGTH THRESHOLD
 	conDir, ccount = get_contigs(args, BASEDIR)
 
 	# ESTABLISH RAW ALIGNMENT OUTPUT TABLE
 	outTab = '/'.join((BASEDIR.path, 'alignment_results.tsv'))
 	f1 = open(outTab, 'w')
 	header = 'contig', 'staxids', 'title', 'percent_ident', 'query_coverage', 'qcovhsp', 'length', 'e_value'
-	head = '\t'.join(header)
+	head = '\t'.join(header) + '\n'
 	f1.write(head)
+	
+	notFound = 'no alignments met required parameters'
 
 	# RUN BLASTN and REPORT RESULTS
 	print(f'There are {str(ccount)} contigs to align')
 	path = args.blastn_path
 	outfmt = '6 qseqid staxids stitle pident qcovs qcovhsp length evalue'
 	count = 0
 	for file in conDir.files:
@@ -204,42 +206,64 @@
 		seqID = seqName.split('_')[0]
 
 		# call BLAST remotely
 		command = [path, '-remote', '-db', 'nr', '-query', file.path, '-outfmt', outfmt, '-perc_identity', '95', '-qcov_hsp_perc', '95', '-max_target_seqs', '5']
 		process = subprocess.run(command, capture_output=True)
 		result = process.stdout.decode("utf-8")
 		result = ''.join(('\n', result))
+		#print(len(result))
+		#print(result)
+
+		if len(result) < 2:
+			result = '\t'.join((seqName, notFound)) + '\n\n'
 
 		f1.write(result)
 
 	f1.close()
+	
 
 	# EVALUATE BLAST RESULT
 	print('Evaluating BLAST results')
 	f2 = open(outTab, 'r')
 	f2.readline() # skip header
 	sumDic = {}
 	chrom = 0
 	plasmid = 0
 	plastid = 0
 	und = 0
 	for line in f2:
-		if line == "\n":
+		line = line.strip()
+		#print('\n')
+		#print('line: ', line)
+		if len(line) == 0:
 			continue
+
 		l = line.split('\t')
+		
+
 		key = l[0]
-		taxid = str(l[1])
-		title = l[2]
 
 		if key not in sumDic:
 			sumDic[key] = {}
 			sumDic[key]['plas'] = 0
 			sumDic[key]['chrom'] = 0
 			sumDic[key]['und'] = 0
 			sumDic[key]['contam'] = 0
+			sumDic[key]['notfound'] = 0
+
+		#print(l)
+		taxid = str(l[1])
+		#print('taxid: ', taxid, notFound)
+		if taxid == notFound:
+			#print('\tmatch')
+			sumDic[key]['notfound'] += 1
+			continue
+
+
+		title = l[2]
 
 		# Counts matches to human samples
 		if taxid == "9606":				# Detect companination (limited to homo sapien)
 			sumDic[key]['contam'] += 1
 			continue
 
 		# Counts matches to plasmid samples
@@ -263,20 +287,23 @@
 	head = ''.join(('\t'.join(header), '\n'))
 	f3.write(head)
 	for key in sumDic:
 		con = sumDic[key]['contam']
 		c = sumDic[key]['chrom']
 		p = sumDic[key]['plas']
 		u = sumDic[key]['und']
+		n = sumDic[key]['notfound']
 
 		#r = c/p    # Note to check for denominator = 0
 		# Failure -> undetermined
-		if c == p & p == u & c == 0: # Novel plasmid - no hits
-			ment = 'novel'
-		if c > (p + u):
+		if n > c+p+u:
+			ment = 'no sig. hits'
+		#elif c == p & p == u & c == 0: # Novel plasmid - no hits
+		#	ment = 'novel'
+		elif c > (p + u):
 			ment = 'chromosome'
 		elif p > (c + u):
 			ment = 'plasmid'
 		else:
 			ment = 'undetermined'
 
 		#  Override if  contamination
```

### Comparing `plasIDome-0.0.3/plasIDome.egg-info/PKG-INFO` & `plasIDome-1.0.0/plasIDome.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plasIDome
-Version: 0.0.3
+Version: 1.0.0
 Summary: A tool to detect plasmids and contamination in bacterial and archaeal genome assemblies
 Home-page: https://github.com/jrhendrix/plasIDome
 Author: Jo Hendrix
 Author-email: jrhendrix36@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `plasIDome-0.0.3/setup.py` & `plasIDome-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="plasIDome",
-    version="0.0.3",
+    version="1.0.0",
     author="Jo Hendrix",
     author_email="jrhendrix36@gmail.com",
     description="A tool to detect plasmids and contamination in bacterial and archaeal genome assemblies",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jrhendrix/plasIDome",
     scripts=['bin/plasIDome'],
```

