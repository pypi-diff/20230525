# Comparing `tmp/spdxmerge-0.1.3.tar.gz` & `tmp/spdxmerge-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spdxmerge-0.1.3.tar", last modified: Wed Apr 26 11:57:56 2023, max compression
+gzip compressed data, was "spdxmerge-0.2.0.tar", last modified: Thu May 25 13:35:23 2023, max compression
```

## Comparing `spdxmerge-0.1.3.tar` & `spdxmerge-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:57:56.518971 spdxmerge-0.1.3/
--rw-r--r--   0 root         (0) root         (0)     1091 2023-04-26 11:57:47.000000 spdxmerge-0.1.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)      388 2023-04-26 11:57:56.518971 spdxmerge-0.1.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2614 2023-04-26 11:57:47.000000 spdxmerge-0.1.3/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 11:57:56.518971 spdxmerge-0.1.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      866 2023-04-26 11:57:47.000000 spdxmerge-0.1.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:57:56.518971 spdxmerge-0.1.3/spdxmerge/
--rwxr-xr-x   0 root         (0) root         (0)     1892 2023-04-26 11:57:47.000000 spdxmerge-0.1.3/spdxmerge/SPDXMerge.py
--rwxr-xr-x   0 root         (0) root         (0)     1793 2023-04-26 11:57:47.000000 spdxmerge-0.1.3/spdxmerge/SPDXMergeLib.py
--rwxr-xr-x   0 root         (0) root         (0)     2396 2023-04-26 11:57:47.000000 spdxmerge-0.1.3/spdxmerge/SPDX_DeepMerge.py
--rwxr-xr-x   0 root         (0) root         (0)     1727 2023-04-26 11:57:47.000000 spdxmerge-0.1.3/spdxmerge/SPDX_ShallowMerge.py
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:57:47.000000 spdxmerge-0.1.3/spdxmerge/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      496 2023-04-26 11:57:47.000000 spdxmerge-0.1.3/spdxmerge/checksum.py
--rwxr-xr-x   0 root         (0) root         (0)      419 2023-04-26 11:57:47.000000 spdxmerge-0.1.3/spdxmerge/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:57:56.518971 spdxmerge-0.1.3/spdxmerge.egg-info/
--rw-r--r--   0 root         (0) root         (0)      388 2023-04-26 11:57:56.000000 spdxmerge-0.1.3/spdxmerge.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      456 2023-04-26 11:57:56.000000 spdxmerge-0.1.3/spdxmerge.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 11:57:56.000000 spdxmerge-0.1.3/spdxmerge.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-04-26 11:57:56.000000 spdxmerge-0.1.3/spdxmerge.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-04-26 11:57:56.000000 spdxmerge-0.1.3/spdxmerge.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-04-26 11:57:56.000000 spdxmerge-0.1.3/spdxmerge.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:57:56.518971 spdxmerge-0.1.3/test/
--rw-r--r--   0 root         (0) root         (0)     8136 2023-04-26 11:57:47.000000 spdxmerge-0.1.3/test/test_SPDX_DeepMerge.py
--rw-r--r--   0 root         (0) root         (0)     2832 2023-04-26 11:57:47.000000 spdxmerge-0.1.3/test/test_SPDX_ShallowMerge.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 13:35:23.733864 spdxmerge-0.2.0/
+-rw-r--r--   0 root         (0) root         (0)     1091 2023-05-25 13:35:15.000000 spdxmerge-0.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      388 2023-05-25 13:35:23.733864 spdxmerge-0.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2772 2023-05-25 13:35:15.000000 spdxmerge-0.2.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-25 13:35:23.733864 spdxmerge-0.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      866 2023-05-25 13:35:15.000000 spdxmerge-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 13:35:23.733864 spdxmerge-0.2.0/spdxmerge/
+-rwxr-xr-x   0 root         (0) root         (0)     2079 2023-05-25 13:35:15.000000 spdxmerge-0.2.0/spdxmerge/SPDXMerge.py
+-rwxr-xr-x   0 root         (0) root         (0)     1878 2023-05-25 13:35:15.000000 spdxmerge-0.2.0/spdxmerge/SPDXMergeLib.py
+-rwxr-xr-x   0 root         (0) root         (0)     2396 2023-05-25 13:35:15.000000 spdxmerge-0.2.0/spdxmerge/SPDX_DeepMerge.py
+-rwxr-xr-x   0 root         (0) root         (0)     1727 2023-05-25 13:35:15.000000 spdxmerge-0.2.0/spdxmerge/SPDX_ShallowMerge.py
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 13:35:15.000000 spdxmerge-0.2.0/spdxmerge/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      496 2023-05-25 13:35:15.000000 spdxmerge-0.2.0/spdxmerge/checksum.py
+-rwxr-xr-x   0 root         (0) root         (0)      419 2023-05-25 13:35:15.000000 spdxmerge-0.2.0/spdxmerge/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 13:35:23.733864 spdxmerge-0.2.0/spdxmerge.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      388 2023-05-25 13:35:23.000000 spdxmerge-0.2.0/spdxmerge.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      456 2023-05-25 13:35:23.000000 spdxmerge-0.2.0/spdxmerge.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 13:35:23.000000 spdxmerge-0.2.0/spdxmerge.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-05-25 13:35:23.000000 spdxmerge-0.2.0/spdxmerge.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-05-25 13:35:23.000000 spdxmerge-0.2.0/spdxmerge.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-25 13:35:23.000000 spdxmerge-0.2.0/spdxmerge.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 13:35:23.733864 spdxmerge-0.2.0/test/
+-rw-r--r--   0 root         (0) root         (0)     8136 2023-05-25 13:35:15.000000 spdxmerge-0.2.0/test/test_SPDX_DeepMerge.py
+-rw-r--r--   0 root         (0) root         (0)     2832 2023-05-25 13:35:15.000000 spdxmerge-0.2.0/test/test_SPDX_ShallowMerge.py
```

### Comparing `spdxmerge-0.1.3/LICENSE` & `spdxmerge-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spdxmerge-0.1.3/README.md` & `spdxmerge-0.2.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -21,29 +21,30 @@
 pip install -r requirements.txt
 ```
 
 Execute the command with the required inputs.
   
 ```shell
     python src/SPDXMerge --docpath <folder path of the SBOMs to be merged>
+                         --outpath <folder path where the merged file will be saved> (optional)
                          --name <product name>
                          --mergetype <0 for deep merge/1 for shallow merge>
                          --author <organization or author name>
                          --email <org/ author email>
                          --docnamespace <namespace for spdx doc>
                          --filetype <expected SBOM file format for JSON/T for Tag value>
 ```
 
 ### GitHub action
 
 ```yml
   - name: Checkout project
     uses: actions/checkout@v3
   - name: Run SPDX Merge tool to merge spdx files 
-    uses: philips-software/SPDXMerge@v0.1
+    uses: philips-software/SPDXMerge@v0.2.0
     with:
       docpath: ${{github.workspace}}/Test # path with spdx files in json
       name: sample-sbom                   # name project
       mergetype: 1                        # 0 shallow merge, 1 deep merge defaults 1
       author: "Kung Fury"                 # Author
       email: "kfury@example.com"          # email - optional
       filetype: J                         # expected SBOM format JSON/ tag value format , defaults to J
@@ -51,21 +52,24 @@
   - name: Check result
     run: cat merged-SBoM.json
 ```
 
 ### Docker image
 
 ```shell
-docker run -it --rm -v$(PWD):/code \
+docker run -it --rm \
+  -v $(PWD):/code \
+  -v $(PWD)/output/:/output \
   -e DOCPATH='/code' \
+  -e OUTPATH='/output' \
   -e NAME='' \
   -e MERGETYPE='' \
   -e AUTHOR='' \
   -e EMAIL='' \
   -e DOCNAMESPACE='' \
   -e FILETYPE='' \
-  docker.io/philipssoftware/spdxmerge:v0.1.0
+  docker.io/philipssoftware/spdxmerge:v0.2.0
 ```
 
 ## TODOs
 
 - Option for Organization, Author tag in document creation
```

### Comparing `spdxmerge-0.1.3/setup.py` & `spdxmerge-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 requirements_path = os.path.join(os.path.dirname(__file__), 'requirements.txt')
 
 with open(requirements_path, "r", encoding="utf8") as f:
     required = f.read().splitlines()
 
 setup(
     name='spdxmerge',
-    version='0.1.3',
+    version='0.2.0',
     description="merges content of two/more spdx sboms",
     long_description_content_type="text/markdown",
     url="https://github.com/philips-software/SPDXMerge",
     packages=find_packages(include=['spdxmerge'], exclude=['test', '*.test', '*.test.*']),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

### Comparing `spdxmerge-0.1.3/spdxmerge/SPDXMerge.py` & `spdxmerge-0.2.0/spdxmerge/SPDXMerge.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,27 +8,28 @@
 from spdxmerge.SPDXMergeLib import create_merged_spdx_document, write_file
 from spdxmerge.utils import read_docs
 
 
 
 @click.command()
 @click.option("--docpath", prompt="Directory path", required=True, help="Directory path with SPDX files to be merged")
+@click.option("--outpath", prompt="Output directory path", required=False, prompt_required=False, help="Output directory path where merged file should be saved")
 @click.option("--name", prompt="Product Name", required=True, help="Name of product for which SBoM is created")
 @click.option("--mergetype", prompt="Shallow Merge -0 or Deep Merge-1", help="Enter 0 for shallow merge , 1 for deep merge", type=click.Choice(['0','1']), default='1')
 @click.option("--author", prompt="SBoM Author name", required=True, help="Author who is writing SBoM")
 @click.option("--email", prompt="SBoM author email address", help="Email address of the author")
 @click.option("--docnamespace", prompt="Document namespace", help="URL where document is stored or organization URL", default="https://spdx.organization.name")
 @click.option("--filetype", prompt="SBoM output file type SPDX tag value format - T or JSON - J",
               help="Enter T for SPDX tag value format, J for JSON", type=click.Choice(['T', 't', 'J','j']), default='J')
-def main(docpath, name, mergetype, author, email, docnamespace, filetype):
+def main(docpath, name, mergetype, author, email, docnamespace, filetype, outpath = None):
     """Tool provides option to merge SPDX SBoM files. Provides two options for merging,
     Shallow Merge: New SBoM is created only with external ref links to SBoM files to be merged
     Deep Merge: New SBoM file is created by appending package, relationship, license information
     """
     doc_list = read_docs(docpath)
     merge_type = "shallow" if mergetype == '0' else "deep"
     doc = create_merged_spdx_document(doc_list, docnamespace, name, author, email, merge_type)
-    write_file(doc, filetype, merge_type)
+    write_file(doc, filetype, merge_type, outpath)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `spdxmerge-0.1.3/spdxmerge/SPDXMergeLib.py` & `spdxmerge-0.2.0/spdxmerge/SPDXMergeLib.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import codecs
+import os
 from spdx.writers.json import write_document as write_json_document, InvalidDocumentError as JsonInvalidDocumentError
 from spdx.writers.tagvalue import write_document as write_tagvalue_document, InvalidDocumentError as TagvalueInvalidDocumentError
 from spdx.parsers.loggers import ErrorMessages
 from spdxmerge.SPDX_DeepMerge import SPDX_DeepMerger
 from spdxmerge.SPDX_ShallowMerge import SPDX_ShallowMerger
 
 def create_merged_spdx_document(doc_list, docnamespace, name, author, email, merge_type):
@@ -17,17 +18,19 @@
     elif merge_type == "shallow":
         merger = SPDX_ShallowMerger(doc_list, docnamespace, name, author, email)
         merger.doc_creationInfo()
         merger.doc_externalDocumentRef()
 
     return merger.get_document()
 
-def write_file(doc, filetype, merge_type):
+def write_file(doc, filetype, merge_type, outpath = None):
     result_filetype = "spdx" if filetype.lower() == "t" else "json"
     file = f"merged-SBoM-{merge_type}.{result_filetype}"
+    if outpath:
+        file = os.path.join(outpath, file)
     with codecs.open(file, mode="w", encoding="utf-8") as out:
         try:
             if result_filetype == "spdx":
                 write_tagvalue_document(doc, out)
             else:
                 write_json_document(doc, out)
         except (TagvalueInvalidDocumentError, JsonInvalidDocumentError) as e:
```

### Comparing `spdxmerge-0.1.3/spdxmerge/SPDX_DeepMerge.py` & `spdxmerge-0.2.0/spdxmerge/SPDX_DeepMerge.py`

 * *Files identical despite different names*

### Comparing `spdxmerge-0.1.3/spdxmerge/SPDX_ShallowMerge.py` & `spdxmerge-0.2.0/spdxmerge/SPDX_ShallowMerge.py`

 * *Files identical despite different names*

### Comparing `spdxmerge-0.1.3/test/test_SPDX_DeepMerge.py` & `spdxmerge-0.2.0/test/test_SPDX_DeepMerge.py`

 * *Files identical despite different names*

### Comparing `spdxmerge-0.1.3/test/test_SPDX_ShallowMerge.py` & `spdxmerge-0.2.0/test/test_SPDX_ShallowMerge.py`

 * *Files identical despite different names*

