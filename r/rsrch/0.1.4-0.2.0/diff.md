# Comparing `tmp/rsrch-0.1.4.tar.gz` & `tmp/rsrch-0.2.0.tar.gz`

## Comparing `rsrch-0.1.4.tar` & `rsrch-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 rsrch-0.1.4/.DS_Store
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 rsrch-0.1.4/requirements.txt
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 rsrch-0.1.4/examples/yitay.md
--rw-r--r--   0        0        0  2231016 2020-02-02 00:00:00.000000 rsrch-0.1.4/papers/Birdwatch:_Crowd_Wisdom_and_Bridging_Algorithms_can_Inform
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 rsrch-0.2.0/.DS_Store
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 rsrch-0.2.0/examples/yitay.md
+-rw-r--r--   0        0        0  2231016 2020-02-02 00:00:00.000000 rsrch-0.2.0/papers/Birdwatch:_Crowd_Wisdom_and_Bridging_Algorithms_can_Inform
 Understanding_and_Reduce_the_Spread_of_Misinformation.pdf
--rw-r--r--   0        0        0   704784 2020-02-02 00:00:00.000000 rsrch-0.1.4/papers/Decision_Transformer:_Reinforcement
+-rw-r--r--   0        0        0   704784 2020-02-02 00:00:00.000000 rsrch-0.2.0/papers/Decision_Transformer:_Reinforcement
 Learning_via_Sequence_Modeling.pdf
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 rsrch-0.1.4/rsrch/__about__.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 rsrch-0.1.4/rsrch/__init__.py
--rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 rsrch-0.1.4/rsrch/_src/rsrch.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 rsrch-0.1.4/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 rsrch-0.1.4/LICENSE
--rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 rsrch-0.1.4/README.md
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 rsrch-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 rsrch-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 rsrch-0.2.0/rsrch/__about__.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 rsrch-0.2.0/rsrch/__init__.py
+-rw-r--r--   0        0        0     4938 2020-02-02 00:00:00.000000 rsrch-0.2.0/rsrch/_src/labml.py
+-rw-r--r--   0        0        0     5390 2020-02-02 00:00:00.000000 rsrch-0.2.0/rsrch/_src/notion.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 rsrch-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 rsrch-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 rsrch-0.2.0/README.md
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 rsrch-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 rsrch-0.2.0/PKG-INFO
```

### Comparing `rsrch-0.1.4/.DS_Store` & `rsrch-0.2.0/.DS_Store`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 0000 0001 4275 6431 0000 1000 0000 0800  ....Bud1........
 00000010: 0000 1000 0000 0209 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 0002 0000 0000 0000 0005  ................
+00000040: 0000 0000 0000 0002 0000 0000 0000 0004  ................
 00000050: 0000 0001 0000 1000 0072 0073 496c 6f63  .........r.sIloc
 00000060: 626c 6f62 0000 0000 0000 0000 0000 0000  blob............
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -26,15 +26,15 @@
 00000190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000200: 0000 0000 0000 0000 0000 0005 0000 0006  ................
+00000200: 0000 0000 0000 0000 0000 0004 0000 0006  ................
 00000210: 0070 0061 0070 0065 0072 0073 496c 6f63  .p.a.p.e.r.sIloc
 00000220: 626c 6f62 0000 0010 0000 018b 0000 002e  blob............
 00000230: ffff ffff ffff 0000 0000 0006 0070 0061  .............p.a
 00000240: 0070 0065 0072 0073 6277 7370 626c 6f62  .p.e.r.sbwspblob
 00000250: 0000 00b8 6270 6c69 7374 3030 d601 0203  ....bplist00....
 00000260: 0405 0607 0807 080b 085d 5368 6f77 5374  .........]ShowSt
 00000270: 6174 7573 4261 725b 5368 6f77 546f 6f6c  atusBar[ShowTool
@@ -47,19 +47,19 @@
 000002e0: 1523 2f3b 525f 6b6c 6d6e 6f8a 0000 0000  .#/;R_klmno.....
 000002f0: 0000 0101 0000 0000 0000 000d 0000 0000  ................
 00000300: 0000 0000 0000 0000 0000 008b 0000 0006  ................
 00000310: 0070 0061 0070 0065 0072 0073 7653 726e  .p.a.p.e.r.svSrn
 00000320: 6c6f 6e67 0000 0001 0000 0009 0052 0045  long.........R.E
 00000330: 0041 0044 004d 0045 002e 006d 0064 496c  .A.D.M.E...m.dIl
 00000340: 6f63 626c 6f62 0000 0010 0000 0267 0000  ocblob.......g..
-00000350: 002e ffff ffff ffff 0000 0000 0010 0072  ...............r
-00000360: 0065 0071 0075 0069 0072 0065 006d 0065  .e.q.u.i.r.e.m.e
-00000370: 006e 0074 0073 002e 0074 0078 0074 496c  .n.t.s...t.x.tIl
-00000380: 6f63 626c 6f62 0000 0010 0000 0041 0000  ocblob.......A..
-00000390: 00ac ffff ffff ffff 0000 0000 0000 0000  ................
+00000350: 002e ffff ffff ffff 0000 0000 0000 0000  ................
+00000360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000400: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `rsrch-0.1.4/examples/yitay.md` & `rsrch-0.2.0/examples/yitay.md`

 * *Files identical despite different names*

### Comparing `rsrch-0.1.4/papers/Birdwatch:_Crowd_Wisdom_and_Bridging_Algorithms_can_Inform
Understanding_and_Reduce_the_Spread_of_Misinformation.pdf` & `rsrch-0.2.0/papers/Birdwatch:_Crowd_Wisdom_and_Bridging_Algorithms_can_Inform
Understanding_and_Reduce_the_Spread_of_Misinformation.pdf`

 * *Files identical despite different names*

### Comparing `rsrch-0.1.4/papers/Decision_Transformer:_Reinforcement
Learning_via_Sequence_Modeling.pdf` & `rsrch-0.2.0/papers/Decision_Transformer:_Reinforcement
Learning_via_Sequence_Modeling.pdf`

 * *Files identical despite different names*

### Comparing `rsrch-0.1.4/rsrch/_src/rsrch.py` & `rsrch-0.2.0/rsrch/_src/notion.py`

 * *Files 23% similar despite different names*

```diff
@@ -23,14 +23,33 @@
             if not url == None and url.startswith("http"):
                 papers.append((title, url, date, authors))
 
     return papers
 
 
 def download():
+    """
+    Downloads papers from Notion.
+
+    Returns:
+        None
+
+    Downloads papers from the Notion database.
+    Paper URLs are fetched from the table using the 'fetch_table' function.
+    The downloaded papers are saved in a 'papers' directory.
+    Existing files are skipped.
+    Prints progress information for each paper being downloaded.
+
+    Note:
+        - Requires the 'python-dotenv', 'urllib3', 'requests', and 'tqdm' libraries.
+        - 'fetch_table' function is assumed to be defined elsewhere.
+
+    Example Usage:
+        download()
+    """
     print("Downloading papers from Notion...")
     urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
     load_dotenv()
     papers = fetch_table()
 
     if not os.path.exists("papers"):
         os.mkdir("papers")
@@ -89,14 +108,35 @@
         },
     )
 
     print(f"- {title}")
 
 
 def upload(arxiv_urls):
+    """
+    Uploads papers from arXiv to Notion.
+
+    Parameters:
+        arxiv_urls (list): List of arXiv URLs or IDs.
+
+    Returns:
+        None
+
+    Connects to Notion API and uploads papers from arXiv.
+    Creates new papers in Notion, skipping existing ones.
+    Prints "Done!" when finished.
+
+    Example:
+        urls = [
+            "https://arxiv.org/abs/2105.12345",
+            "https://arxiv.org/abs/2106.67890",
+            "https://arxiv.org/pdf/2107.24680.pdf"
+        ]
+        upload(urls)
+    """
     load_dotenv()
     notion = Client(auth=os.getenv("NOTION_TOKEN"))
 
     # Extract arXiv IDs from valid URLs
     ids = []
     for url in arxiv_urls:
         if url.startswith("https://arxiv.org/abs/"):
```

### Comparing `rsrch-0.1.4/LICENSE` & `rsrch-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rsrch-0.1.4/README.md` & `rsrch-0.2.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # rsrch
-Manage your research papers from the command line. This project lets you update a Notion database with arXiv links and download PDFs of papers to your local machine.
+Manage your research papers from Python. This project lets you update a Notion database with arXiv links and download PDFs of papers to your local machine.
 
 <p align="center">
     <img width="1095" alt="image" src="https://user-images.githubusercontent.com/47067154/219932040-ab4962f8-b01e-4d94-9eba-77a155b0e933.png">
 </p>
 
 ## Installation
 1. Create an [internal integration](https://www.notion.so/help/create-integrations-with-the-notion-api) in Notion.
@@ -59,10 +59,15 @@
 
 Alternatively, you can add non-arXiv links manually to Notion.
 
 
 ## Notes
 - Uploading papers to Notion is currently only supported for arXiv links. Papers with titles that already exist in the database will not be uploaded.
 - I plan on adding support for other databases in the future, but for now it only works with Notion databases.
+- To build and release this:
+  - Make new code accessible in `src/__init__.py`
+  - Update the version in `src/__about__.py`
+  - Run `python3 -m build`
+  - Run `python3 -m twine upload dist/*`
 
 ### Resources
 - [Notion API](https://developers.notion.com/)
```

### Comparing `rsrch-0.1.4/pyproject.toml` & `rsrch-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 ]
 dependencies = [
     "arxiv==1.4.2",
     "click==8.1.3",
     "notion-client==2.0.0",
     "python-dotenv==0.21.0",
     "requests==2.28.1",
+    "rich==13.3.4",
+    "selenium==4.9.1",
     "tqdm==4.64.1",
     "urllib3==1.26.13",
 ]
 dynamic = ["version"]
 
 [project.urls]
 "Homepage" = "https://github.com/ishan0102/rsrch"
```

### Comparing `rsrch-0.1.4/PKG-INFO` & `rsrch-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: rsrch
-Version: 0.1.4
+Version: 0.2.0
 Summary: Manage your ever-growing list of research papers
 Project-URL: Homepage, https://github.com/ishan0102/rsrch
 Project-URL: Bug Tracker, https://github.com/ishan0102/rsrch/issues
 Author-email: Ishan Shah <ishan0102@utexas.edu>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: arxiv==1.4.2
 Requires-Dist: click==8.1.3
 Requires-Dist: notion-client==2.0.0
 Requires-Dist: python-dotenv==0.21.0
 Requires-Dist: requests==2.28.1
+Requires-Dist: rich==13.3.4
+Requires-Dist: selenium==4.9.1
 Requires-Dist: tqdm==4.64.1
 Requires-Dist: urllib3==1.26.13
 Description-Content-Type: text/markdown
 
 # rsrch
-Manage your research papers from the command line. This project lets you update a Notion database with arXiv links and download PDFs of papers to your local machine.
+Manage your research papers from Python. This project lets you update a Notion database with arXiv links and download PDFs of papers to your local machine.
 
 <p align="center">
     <img width="1095" alt="image" src="https://user-images.githubusercontent.com/47067154/219932040-ab4962f8-b01e-4d94-9eba-77a155b0e933.png">
 </p>
 
 ## Installation
 1. Create an [internal integration](https://www.notion.so/help/create-integrations-with-the-notion-api) in Notion.
@@ -80,10 +82,15 @@
 
 Alternatively, you can add non-arXiv links manually to Notion.
 
 
 ## Notes
 - Uploading papers to Notion is currently only supported for arXiv links. Papers with titles that already exist in the database will not be uploaded.
 - I plan on adding support for other databases in the future, but for now it only works with Notion databases.
+- To build and release this:
+  - Make new code accessible in `src/__init__.py`
+  - Update the version in `src/__about__.py`
+  - Run `python3 -m build`
+  - Run `python3 -m twine upload dist/*`
 
 ### Resources
 - [Notion API](https://developers.notion.com/)
```

