# Comparing `tmp/bibtex-dblp-0.5.tar.gz` & `tmp/bibtex-dblp-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bibtex-dblp-0.5.tar", last modified: Fri Dec  6 09:54:51 2019, max compression
+gzip compressed data, was "bibtex-dblp-0.9.tar", last modified: Thu May 25 08:55:02 2023, max compression
```

## Comparing `bibtex-dblp-0.5.tar` & `bibtex-dblp-0.9.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-12-06 09:54:51.000000 bibtex-dblp-0.5/
--rw-r--r--   0 mvolk      (502) staff       (20)     2312 2019-12-06 09:54:51.000000 bibtex-dblp-0.5/PKG-INFO
--rw-r--r--   0 mvolk      (502) staff       (20)     1532 2019-12-06 09:36:29.000000 bibtex-dblp-0.5/README.md
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-12-06 09:54:51.000000 bibtex-dblp-0.5/bibtex_dblp/
--rw-r--r--   0 mvolk      (502) staff       (20)        0 2019-12-05 21:16:53.000000 bibtex-dblp-0.5/bibtex_dblp/__init__.py
--rw-r--r--   0 mvolk      (502) staff       (20)      252 2019-12-05 20:40:02.000000 bibtex-dblp-0.5/bibtex_dblp/config.py
--rw-r--r--   0 mvolk      (502) staff       (20)     2169 2019-12-05 19:55:03.000000 bibtex-dblp-0.5/bibtex_dblp/database.py
--rw-r--r--   0 mvolk      (502) staff       (20)     2260 2019-12-05 20:40:51.000000 bibtex-dblp-0.5/bibtex_dblp/dblp_api.py
--rw-r--r--   0 mvolk      (502) staff       (20)     2178 2019-12-05 20:37:23.000000 bibtex-dblp-0.5/bibtex_dblp/dblp_data.py
--rw-r--r--   0 mvolk      (502) staff       (20)     1168 2019-12-05 20:28:02.000000 bibtex-dblp-0.5/bibtex_dblp/io.py
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-12-06 09:54:51.000000 bibtex-dblp-0.5/bibtex_dblp.egg-info/
--rw-r--r--   0 mvolk      (502) staff       (20)     2312 2019-12-06 09:54:50.000000 bibtex-dblp-0.5/bibtex_dblp.egg-info/PKG-INFO
--rw-r--r--   0 mvolk      (502) staff       (20)      406 2019-12-06 09:54:51.000000 bibtex-dblp-0.5/bibtex_dblp.egg-info/SOURCES.txt
--rw-r--r--   0 mvolk      (502) staff       (20)        1 2019-12-06 09:54:50.000000 bibtex-dblp-0.5/bibtex_dblp.egg-info/dependency_links.txt
--rw-r--r--   0 mvolk      (502) staff       (20)       83 2019-12-06 09:54:50.000000 bibtex-dblp-0.5/bibtex_dblp.egg-info/entry_points.txt
--rw-r--r--   0 mvolk      (502) staff       (20)       16 2019-12-06 09:54:50.000000 bibtex-dblp-0.5/bibtex_dblp.egg-info/requires.txt
--rw-r--r--   0 mvolk      (502) staff       (20)       12 2019-12-06 09:54:50.000000 bibtex-dblp-0.5/bibtex_dblp.egg-info/top_level.txt
-drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2019-12-06 09:54:51.000000 bibtex-dblp-0.5/bin/
--rw-r--r--   0 mvolk      (502) staff       (20)     1464 2019-12-05 21:05:44.000000 bibtex-dblp-0.5/bin/convert_dblp.py
--rw-r--r--   0 mvolk      (502) staff       (20)     2805 2019-12-06 09:28:12.000000 bibtex-dblp-0.5/bin/import_dblp.py
--rw-r--r--   0 mvolk      (502) staff       (20)       38 2019-12-06 09:54:51.000000 bibtex-dblp-0.5/setup.cfg
--rw-r--r--   0 mvolk      (502) staff       (20)     1051 2019-12-06 09:54:47.000000 bibtex-dblp-0.5/setup.py
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-05-25 08:55:02.809864 bibtex-dblp-0.9/
+-rw-r--r--   0 mvolk      (502) staff       (20)    35149 2019-12-05 12:18:12.000000 bibtex-dblp-0.9/LICENSE
+-rw-r--r--   0 mvolk      (502) staff       (20)     3290 2023-05-25 08:55:02.810141 bibtex-dblp-0.9/PKG-INFO
+-rw-r--r--   0 mvolk      (502) staff       (20)     2948 2023-05-02 15:56:34.000000 bibtex-dblp-0.9/README.md
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-05-25 08:55:02.800115 bibtex-dblp-0.9/bibtex_dblp/
+-rw-r--r--   0 mvolk      (502) staff       (20)        0 2019-12-05 21:16:53.000000 bibtex-dblp-0.9/bibtex_dblp/__init__.py
+-rw-r--r--   0 mvolk      (502) staff       (20)      249 2023-05-25 08:33:30.000000 bibtex-dblp-0.9/bibtex_dblp/config.py
+-rw-r--r--   0 mvolk      (502) staff       (20)     4218 2023-05-25 08:38:06.000000 bibtex-dblp-0.9/bibtex_dblp/database.py
+-rw-r--r--   0 mvolk      (502) staff       (20)     3708 2023-05-25 08:38:06.000000 bibtex-dblp-0.9/bibtex_dblp/dblp_api.py
+-rw-r--r--   0 mvolk      (502) staff       (20)     2268 2020-02-21 11:02:13.000000 bibtex-dblp-0.9/bibtex_dblp/dblp_data.py
+-rw-r--r--   0 mvolk      (502) staff       (20)     1168 2023-04-18 13:29:38.000000 bibtex-dblp-0.9/bibtex_dblp/io.py
+-rw-r--r--   0 mvolk      (502) staff       (20)      637 2023-04-18 13:29:38.000000 bibtex-dblp-0.9/bibtex_dblp/search.py
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-05-25 08:55:02.805630 bibtex-dblp-0.9/bibtex_dblp.egg-info/
+-rw-r--r--   0 mvolk      (502) staff       (20)     3290 2023-05-25 08:55:02.000000 bibtex-dblp-0.9/bibtex_dblp.egg-info/PKG-INFO
+-rw-r--r--   0 mvolk      (502) staff       (20)      470 2023-05-25 08:55:02.000000 bibtex-dblp-0.9/bibtex_dblp.egg-info/SOURCES.txt
+-rw-r--r--   0 mvolk      (502) staff       (20)        1 2023-05-25 08:55:02.000000 bibtex-dblp-0.9/bibtex_dblp.egg-info/dependency_links.txt
+-rw-r--r--   0 mvolk      (502) staff       (20)      123 2023-05-25 08:55:02.000000 bibtex-dblp-0.9/bibtex_dblp.egg-info/entry_points.txt
+-rw-r--r--   0 mvolk      (502) staff       (20)       26 2023-05-25 08:55:02.000000 bibtex-dblp-0.9/bibtex_dblp.egg-info/requires.txt
+-rw-r--r--   0 mvolk      (502) staff       (20)       12 2023-05-25 08:55:02.000000 bibtex-dblp-0.9/bibtex_dblp.egg-info/top_level.txt
+drwxr-xr-x   0 mvolk      (502) staff       (20)        0 2023-05-25 08:55:02.808833 bibtex-dblp-0.9/bin/
+-rw-r--r--   0 mvolk      (502) staff       (20)     1545 2023-05-25 08:38:06.000000 bibtex-dblp-0.9/bin/convert_dblp.py
+-rw-r--r--   0 mvolk      (502) staff       (20)     4286 2023-05-25 08:38:07.000000 bibtex-dblp-0.9/bin/import_dblp.py
+-rw-r--r--   0 mvolk      (502) staff       (20)     4412 2023-05-25 08:38:07.000000 bibtex-dblp-0.9/bin/update_from_dblp.py
+-rw-r--r--   0 mvolk      (502) staff       (20)       97 2023-05-25 08:55:02.811511 bibtex-dblp-0.9/setup.cfg
+-rw-r--r--   0 mvolk      (502) staff       (20)     1157 2023-05-02 15:48:25.000000 bibtex-dblp-0.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `bibtex-dblp-0.5/README.md` & `bibtex-dblp-0.9/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,48 +1,70 @@
 # bibtex-dblp
+[![Build Status](https://github.com/volkm/bibtex-dblp/workflows/Build%20and%20Test/badge.svg)](https://github.com/volkm/bibtex-dblp/actions)
+[![GitHub release](https://img.shields.io/github/release/volkm/bibtex-dblp.svg)](https://github.com/volkm/bibtex-dblp/releases/)
+[![PyPi](https://img.shields.io/pypi/v/bibtex-dblp)](https://pypi.org/project/bibtex-dblp/)
+
 Create and revise bibtex entries from [DBLP](https://dblp.uni-trier.de/).
 
-# Dependencies
+## Dependencies
 - uses [pybtex](https://pybtex.org/)
 - inspired from [dblp-python](https://github.com/scholrly/dblp-python)
 
-# Installation
+## Installation
 The package can be installed from [PyPI](https://pypi.org/) with:
 ```
 pip install bibtex-dblp
 ```
 
+Manual installation is possible by cloning this repository and building the Python package:
+```
+python setup.py develop
+```
+
 
-# Usage
+## Usage
 
-# Importing new publications from DBLP
+All relevant scripts can be found in the `bin` directory.
+Every script provides information about the expected input and additional arguments via `--help`.
+
+
+### Importing new publications from DBLP
 The script `bin/import_dblp.py` searches for a new publication on DBLP and adds the corresponding bibtex entry to the bibliography.
 
 Usage:
 ```
-import_dblp [--query QUERY] [--out OUT] [--format {condensed,standard,crossref}]
+import_dblp [--query QUERY] [--bib BIBTEX] [--format FORMAT]
 ```
 
 If the argument `--query` is not given, the search keywords can be given directly in the terminal.
 The script then queries the DBLP API and displays the possible matches.
-The correct publication can be selected in the terminal (or `0` for abort).
-The bibtex entry of the selected publication is either appended to the given bibliography (if `--out` is provided) or displayed on the terminal.
+The correct publication number can be selected in the terminal (or `0` for abort).
+The bibtex entry of the selected publication is either appended to the given bibliography (if `--bib` is provided) or displayed on the terminal.
 
-For more options see:
-```
-import_dblp --help
-```
-
-# Converting between DBLP formats
-The script `bin/convert_dblp.py` converts the complete bibliography between different DBLP formats (condensed, standard, crossref).
+### Converting between DBLP formats
+The script `bin/convert_dblp.py` converts the complete bibliography between different DBLP formats.
 
 Usage:
 ```
-convert_dblp INPUT_BIB [--out OUTPUT_BIB] [--format {condensed,standard,crossref}]
+convert_dblp INPUT_BIB [--out OUTPUT_BIB] [--format FORMAT]
 ```
-All bibtex entries with either the field `biburl` given or a bibtex name corresponding to a DBLP id are automatically converted.
+All bibtex entries with either the field `biburl` given or a bibtex name corresponding to a DBLP id are automatically converted into the desired format.
 All other entries are left unchanged.
 
-For more options see:
+### Updating existing bibliography from DBLP
+The script `bin/update_from_dblp.py` updates the entries in an existing bibliography by looking up the information from DBLP.
+
+Usage:
 ```
-convert_dblp --help
+convert_dblp INPUT_BIB [--out OUTPUT_BIB] [--format FORMAT]
 ```
+For each bibtex entry without a DBLP id, the scripts searches DBLP for a possible match.
+The user can select the correct entry from a list of possible matches and the bibliography is updated accordingly.
+Bibtex entries which already have a DBLP id are left unchanged.
+
+
+## Supported DBLP formats
+The following bibtex formats from DBLP are currently supported:
+- `condensed`: Condensed format where e.g. journals and conferences are abbreviated. Default value.
+- `standard`: Default format from DBLP.
+- `crossref`: Extensive format in which conferences have their own bibtex entry
+- `condensed_doi`: Corresponds to `condensed` but additionally includes the DOI
```

### Comparing `bibtex-dblp-0.5/bibtex_dblp/dblp_data.py` & `bibtex-dblp-0.9/bibtex_dblp/dblp_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,35 +40,38 @@
         self.year = int(json.get("year"))
         self.type = json.get("type")
         self.key = json.get("key")
         self.doi = json.get("doi")
         self.ee = json.get("ee")
         self.url = json.get("url")
         self.authors = []
-        print(json)
         authors = json.get("authors")
         if authors:
             authors = authors["author"]
             if isinstance(authors, list):
-                self.authors = [DblpAuthor(name) for name in authors]
+                self.authors = [DblpAuthor(author) for author in authors]
             else:
                 self.authors = [DblpAuthor(authors)]
 
         # Possible additional fields:
         # sub_type, mdate, authors, editors, month, journal, number, chapter, isbn, crossref, publisher, school, citations, series
 
+    def cite_key(self):
+        return "DBLP:" + self.key
+
     def __str__(self):
         authors = ", ".join([str(author) for author in self.authors])
-        book = str(self.venue) + " ({})".format(self.volume if self.volume else "")
+        book = str(self.venue) + " ({})".format(self.volume) if self.volume else ""
         return "{}:\n\t{} {} {}".format(authors, self.title, book, self.year)
 
 
 class DblpAuthor:
     """
     Author in DBLP.
     """
 
-    def __init__(self, name):
-        self.name = name
+    def __init__(self, json):
+        self.name = json.get("text")
+        self.pid = json.get("pid")
 
     def __str__(self):
         return self.name
```

### Comparing `bibtex-dblp-0.5/bibtex_dblp/io.py` & `bibtex-dblp-0.9/bibtex_dblp/io.py`

 * *Files identical despite different names*

### Comparing `bibtex-dblp-0.5/bin/convert_dblp.py` & `bibtex-dblp-0.9/bin/convert_dblp.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,19 +7,23 @@
 import logging
 
 import bibtex_dblp.database
 from bibtex_dblp.dblp_api import BibFormat
 
 
 def main():
-    parser = argparse.ArgumentParser(description='Convert DBLP entries to specific format (condensed, standard, crossref).')
+    parser = argparse.ArgumentParser(
+        description='Convert DBLP entries to specific format (condensed, standard, crossref).')
 
     parser.add_argument('infile', help='Input bibtex file', type=str)
-    parser.add_argument('--out', '-o', help='Output bibtex file. If no output file is given, the input file will be overwritten.', type=str, default=None)
-    parser.add_argument('--format', '-f', help='DBLP format type to convert into', type=BibFormat, choices=list(BibFormat), default=BibFormat.condensed)
+    parser.add_argument('--out', '-o',
+                        help='Output bibtex file. If no output file is given, the input file will be overwritten.',
+                        type=str, default=None)
+    parser.add_argument('--format', '-f', help='DBLP format type to convert into', type=BibFormat,
+                        choices=list(BibFormat), default=BibFormat.condensed)
 
     parser.add_argument('--verbose', '-v', help='print more output', action="store_true")
     args = parser.parse_args()
 
     logging.basicConfig(format='%(levelname)s: %(message)s', level=logging.DEBUG if args.verbose else logging.INFO)
 
     outfile = args.infile if args.out is None else args.out
```

### Comparing `bibtex-dblp-0.5/bin/import_dblp.py` & `bibtex-dblp-0.9/bin/import_dblp.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,64 +2,99 @@
 """
 Import entry from DBLP according to given search input.
 """
 
 import argparse
 import logging
 
+import pyperclip
+
 import bibtex_dblp.config
-import bibtex_dblp.io
+import bibtex_dblp.database
 import bibtex_dblp.dblp_api
+import bibtex_dblp.io
 from bibtex_dblp.dblp_api import BibFormat
 
 
 def main():
     parser = argparse.ArgumentParser(description='Import entry from DBLP according to given search input from cli.')
 
-    parser.add_argument('--query', '-q', help='The query to search for the publication. If none is given the query is obtained from CLI input.', type=str, default=None)
-    parser.add_argument('--out', '-o', help='Output bibtex file where the imported entry will be appended. If no output file is given, the bibtex is printed to the CLI.', type=str,
+    parser.add_argument('--query', '-q',
+                        help='The query to search for the publication. If none is given the query is obtained from CLI input.',
+                        type=str, default=None)
+    parser.add_argument('--bib', '-b',
+                        help='Bibtex file where the imported entry will be appended. If no bibtex file is given, the bibtex is printed to the CLI.',
+                        type=str,
                         default=None)
-    parser.add_argument('--format', '-f', help='DBLP format type to convert into.', type=BibFormat, choices=list(BibFormat), default=BibFormat.condensed)
-    parser.add_argument('--max-results', help="Maximal number of search results to display.", type=int, default=bibtex_dblp.config.MAX_SEARCH_RESULTS)
+    parser.add_argument('--format', '-f', help='DBLP format type to convert into.', type=BibFormat,
+                        choices=list(BibFormat), default=BibFormat.condensed)
+    parser.add_argument('--max-results', help="Maximal number of search results to display.", type=int,
+                        default=bibtex_dblp.config.MAX_SEARCH_RESULTS)
 
     parser.add_argument('--verbose', '-v', help='print more output', action="store_true")
     args = parser.parse_args()
 
     logging.basicConfig(format='%(levelname)s: %(message)s', level=logging.DEBUG if args.verbose else logging.INFO)
     max_search_results = args.max_results
 
+    bib = None
+    if args.bib is not None:
+        # Load bibliography
+        bib = bibtex_dblp.database.load_from_file(args.bib)
+
     if args.query:
         search_words = args.query
     else:
         search_words = bibtex_dblp.io.get_user_input("Give the publication title to search for: ")
+
     # Search for publications
+    if bib is not None:
+        # Check if publication already exists
+        bib_result = bibtex_dblp.database.search(bib, search_words)
+        if bib_result:
+            print("The bibliography already contains the following matches:")
+            for i in range(len(bib_result)):
+                print("({})\t{}".format(i + 1, bibtex_dblp.database.print_entry(bib_result[i][0])))
+            select = bibtex_dblp.io.get_user_number("Select the intended publication (0 to search online): ", 0,
+                                                    len(bib_result))
+            if select > 0:
+                selected_entry = bib_result[select - 1][0]
+                logging.info("Selected bibtex entry:\n")
+                print(bibtex_dblp.database.print_entry(selected_entry))
+                logging.info("Use '{}' to cite it.".format(selected_entry.key))
+                exit(0)
+
     search_results = bibtex_dblp.dblp_api.search_publication(search_words, max_search_results=max_search_results)
     if search_results.total_matches == 0:
         print("The search returned no matches.")
         exit(1)
 
     print("The search returned {} matches:".format(search_results.total_matches))
     if search_results.total_matches > max_search_results:
         print("Displaying only the first {} matches.".format(max_search_results))
     for i in range(len(search_results.results)):
         result = search_results.results[i]
         print("({})\t{}".format(i + 1, result.publication))
 
     # Let user select correct publication
-    select = bibtex_dblp.io.get_user_number("Select the intended publication (0 to abort): ", 0, search_results.total_matches)
+    select = bibtex_dblp.io.get_user_number("Select the intended publication (0 to abort): ", 0,
+                                            search_results.total_matches)
     if select == 0:
         print("Cancelled.")
         exit(1)
 
     publication = search_results.results[select - 1].publication
     pub_bibtex = bibtex_dblp.dblp_api.get_bibtex(publication.key, bib_format=args.format)
-    if args.out:
-        with open(args.out, "a") as f:
+    if args.bib:
+        with open(args.bib, "a") as f:
             f.write(pub_bibtex)
-        logging.info("Bibtex file appended to {}.".format(args.out))
+        logging.info("Bibtex file appended to {}.".format(args.bib))
+        pyperclip.copy(publication.cite_key())
+        logging.info("Copied cite key '{}' to clipboard.".format(publication.cite_key()))
     else:
-        logging.info("Selected bibtex entry:\n")
-        print(pub_bibtex)
+        pyperclip.copy(pub_bibtex)
+        logging.info("Selected bibtex entry:\n{}".format(pub_bibtex))
+        logging.info("Copied selected bibtex entry to clipboard.")
 
 
 if __name__ == "__main__":
     main()
```

