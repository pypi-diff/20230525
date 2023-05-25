# Comparing `tmp/mdforest-1.4.0.tar.gz` & `tmp/mdforest-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdforest-1.4.0.tar", last modified: Fri May 19 15:53:18 2023, max compression
+gzip compressed data, was "mdforest-1.5.0.tar", last modified: Thu May 25 04:02:57 2023, max compression
```

## Comparing `mdforest-1.4.0.tar` & `mdforest-1.5.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-19 15:53:18.529044 mdforest-1.4.0/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)    11358 2023-05-11 12:19:37.000000 mdforest-1.4.0/LICENSE
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3065 2023-05-19 15:53:18.529044 mdforest-1.4.0/PKG-INFO
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2641 2023-05-19 13:52:26.000000 mdforest-1.4.0/README.rst
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-19 15:53:18.529044 mdforest-1.4.0/mdforest/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      457 2023-05-18 22:28:45.000000 mdforest-1.4.0/mdforest/__init__.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3452 2023-05-19 15:13:12.000000 mdforest-1.4.0/mdforest/mdforest.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-19 15:53:18.529044 mdforest-1.4.0/mdforest/tree/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-18 14:40:51.000000 mdforest-1.4.0/mdforest/tree/__init__.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     4199 2023-05-19 15:11:18.000000 mdforest-1.4.0/mdforest/tree/types.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     6325 2023-05-18 19:23:23.000000 mdforest-1.4.0/mdforest/treebuild.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-19 15:53:18.529044 mdforest-1.4.0/mdforest.egg-info/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3065 2023-05-19 15:53:18.000000 mdforest-1.4.0/mdforest.egg-info/PKG-INFO
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      335 2023-05-19 15:53:18.000000 mdforest-1.4.0/mdforest.egg-info/SOURCES.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        1 2023-05-19 15:53:18.000000 mdforest-1.4.0/mdforest.egg-info/dependency_links.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       43 2023-05-19 15:53:18.000000 mdforest-1.4.0/mdforest.egg-info/requires.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        9 2023-05-19 15:53:18.000000 mdforest-1.4.0/mdforest.egg-info/top_level.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-11 12:19:37.000000 mdforest-1.4.0/pyproject.toml
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       38 2023-05-19 15:53:18.529044 mdforest-1.4.0/setup.cfg
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      943 2023-05-19 15:52:26.000000 mdforest-1.4.0/setup.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-19 15:53:18.529044 mdforest-1.4.0/tests/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1196 2023-05-18 14:40:51.000000 mdforest-1.4.0/tests/test_mdtree.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-25 04:02:57.363176 mdforest-1.5.0/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)    11358 2023-05-11 02:15:26.000000 mdforest-1.5.0/LICENSE
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3016 2023-05-25 04:02:57.363176 mdforest-1.5.0/PKG-INFO
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2592 2023-05-20 13:55:14.000000 mdforest-1.5.0/README.rst
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-25 04:02:57.361176 mdforest-1.5.0/mdforest/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1068 2023-05-25 04:00:45.000000 mdforest-1.5.0/mdforest/__init__.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3255 2023-05-25 04:00:23.000000 mdforest-1.5.0/mdforest/mdforest.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-25 04:02:57.363176 mdforest-1.5.0/mdforest/tree/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-19 02:13:23.000000 mdforest-1.5.0/mdforest/tree/__init__.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3378 2023-05-25 03:54:31.000000 mdforest-1.5.0/mdforest/tree/types.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     6325 2023-05-19 02:13:23.000000 mdforest-1.5.0/mdforest/treebuild.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-25 04:02:57.362176 mdforest-1.5.0/mdforest.egg-info/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3016 2023-05-25 04:02:57.000000 mdforest-1.5.0/mdforest.egg-info/PKG-INFO
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      335 2023-05-25 04:02:57.000000 mdforest-1.5.0/mdforest.egg-info/SOURCES.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        1 2023-05-25 04:02:57.000000 mdforest-1.5.0/mdforest.egg-info/dependency_links.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       43 2023-05-25 04:02:57.000000 mdforest-1.5.0/mdforest.egg-info/requires.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        9 2023-05-25 04:02:57.000000 mdforest-1.5.0/mdforest.egg-info/top_level.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-11 02:27:02.000000 mdforest-1.5.0/pyproject.toml
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       38 2023-05-25 04:02:57.363176 mdforest-1.5.0/setup.cfg
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      918 2023-05-25 04:02:51.000000 mdforest-1.5.0/setup.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-25 04:02:57.363176 mdforest-1.5.0/tests/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1196 2023-05-19 02:13:23.000000 mdforest-1.5.0/tests/test_mdtree.py
```

### Comparing `mdforest-1.4.0/LICENSE` & `mdforest-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mdforest-1.4.0/PKG-INFO` & `mdforest-1.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 Metadata-Version: 2.1
 Name: mdforest
-Version: 1.4.0
+Version: 1.5.0
 Summary: A package to convert between Markdown and a forest data structure for efficient processing.
 Home-page: http://github.com/kj3moraes/mdforest
 Author: Keane Moraes
 Author-email: lordvader3002@gmail.com
 License: Apache 2.0
-Download-URL: https://github.com/kj3moraes/mdforest/archive/1.4.0.zip
+Download-URL: https://github.com/kj3moraes/mdforest/archive/1.5.0.zip
 Platform: UNKNOWN
 Classifier: Topic :: Utilities
 License-File: LICENSE
 
-.. image:: media/forest-icon.png
-   :width: 100
-
 mdforest - Markdown Forest
 ==========================
 
 A library to convert Markdown documents into tree data structures and
 vice versa. There is greater functionality available to modify, prune,
 add and delete parts of documents when there are in the MarkdownTree
 structure.
```

### Comparing `mdforest-1.4.0/README.rst` & `mdforest-1.5.0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-.. image:: media/forest-icon.png
-   :width: 100
-
 mdforest - Markdown Forest
 ==========================
 
 A library to convert Markdown documents into tree data structures and
 vice versa. There is greater functionality available to modify, prune,
 add and delete parts of documents when there are in the MarkdownTree
 structure.
```

### Comparing `mdforest-1.4.0/mdforest/mdforest.py` & `mdforest-1.5.0/mdforest/mdforest.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,68 +10,60 @@
     if currTree.depth == None:
         return TextNode(currTree.source.string, parent=parent)
     
     # Get the current header of the tree
     headerText = currTree.source.string
     currentHeaderLevel = currTree.getHeadingLevel(currTree.source)
     rootNode = HeaderNode(headerText, headerNumber=currentHeaderLevel, parent=parent)
-
+    
     for child in currTree.branches:
         if child.getHeadingLevel(child.source) == None:
-            resultNode = TextNode(child.source.string, parent=rootNode)
-            corpus = resultNode.get_corpus()
-            rootNode.append_corpus(corpus)
+            rootNode.add_child(TextNode(child.source.string, parent=rootNode))
         else:
-            resultNode = generateRootNodeFromContents(child, parent=rootNode)
-            corpus = resultNode.get_corpus()
-            rootNode.add_child(resultNode)
-            rootNode.append_corpus(corpus)
-                
+            rootNode.add_child(generateRootNodeFromContents(child, parent=rootNode))
+            
     return rootNode    
 
 def find_backlinks(input_text:str) -> list:
-    """ 
-    Function to find all backlinks in a given text.
-    """
-    
     backlinks = []
 
     # Regular expression pattern to match backlinks
     pattern = r'\[\[(.*?)\]\]'
     backlinks = re.findall(pattern, input_text)
     return backlinks
 
 def find_tags(input_text:str) -> list:
-    """
-    Function to find all tags in a given text.
-    """
-    
     tags = []
 
     # Regular expression pattern to match backlinks
     pattern = r'#([a-zA-Z0-9_]+)'
     tags = re.findall(pattern, input_text)
     return tags
 
+def find_metadata(input_text:str):
+    post = frontmatter.loads(input_text)
+    return post.metadata, post.content
+
 def mdtreeify(name:str, md:str, *args, **kwargs) -> MarkdownForest:
     """
     Converts markdown file to a MarkdownForest
     """
     
-    post = frontmatter.loads(md)
-    backlinks = find_backlinks(post.content)
-    tags = find_tags(post.content)
-    returnForest = MarkdownForest(name, metadata=post.metadata)
+    meta, cont = find_metadata(md)
+    
+    backlinks = find_backlinks(cont)
+    tags = find_tags(cont)
+    returnForest = MarkdownForest(name, metadata=meta)
     
     for backlink in backlinks:
         returnForest.add_backlink(backlink)
     for tag in tags:
         returnForest.add_tag(tag)
     
-    toc =  __TreeOfContents.fromMarkdown(post.content, *args, **kwargs)
+    toc =  __TreeOfContents.fromMarkdown(cont, *args, **kwargs)
     for tree in toc.branches:
         root = generateRootNodeFromContents(tree)
         returnForest.add_tree(MarkdownTree(root))
     
     return returnForest
     
 def convertRootToText(rootNode: Node) -> str:
@@ -87,22 +79,24 @@
         returnString += convertRootToText(child)
     
     return returnString    
         
 def convertDictToMetadata(metadata:dict) -> str:
     yaml = "---\n"
     for key, value in metadata.items():
+        print(f"{key}: {value}")
         if isinstance(value, list):
             yaml += f"{key}: \n"
             for elem in value:
                 yaml += f"  - {elem}\n"
             continue
         yaml += f"{key}: {value}\n"
     yaml += "---\n"
     return yaml
 
 def mdtextify(forest:MarkdownForest, *args, **kwargs) -> str:
+    print(forest.metadata)
     
     finalText = convertDictToMetadata(forest.metadata)
     for i, tree in enumerate(forest):
         finalText += convertRootToText(tree.get_root())
     return finalText
```

### Comparing `mdforest-1.4.0/mdforest/tree/types.py` & `mdforest-1.5.0/mdforest/tree/types.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,36 +13,28 @@
     FRACTION_PRINTABLE = 0.5
     
     def __init__(self, text:str, parent:Node=None):
         self.parent = parent
         self.text = text
         
     def __getitem__(self, index:int):
-        if index < 0 or index >= len(self.text):
-            raise IndexError("Index out of bounds")
         return self.text[index]
            
     def __str__(self):
-        return self.text
+        return self.text[0:min(10, int(self.FRACTION_PRINTABLE * len(self.text)))] + " ..."
 
     def __repr__(self) -> str:
-        return "(Text) " + self.text[0:min(10, int(self.FRACTION_PRINTABLE * len(self.text)))] + " ..."
-    
-    def get_corpus(self) -> str:
         return self.text
-    
-    def set_corpus(self, corpus:str) -> None:
-        self.text = corpus
+
 
 class HeaderNode(Node):
     
     def __init__(self, header:str, headerNumber:int=1, parent:Node=None):
         self.parent = parent
         self.header = header
-        self.corpus = "#" * headerNumber + " " + header + "\n\n"
         self.headerNumber = headerNumber
         self.children = []
         
     def __str__(self):
         return self.header
     
     def __repr__(self):
@@ -54,37 +46,24 @@
     def __iter__(self):
         for elem in self.children:
             yield elem
     
     def __getitem__(self, index:int) -> Node:
         return self.children[index]
     
-    def set_corpus(self, corpus:str) -> None:
-        self.corpus = corpus
-    
-    def get_corpus(self) -> str:
-        return self.corpus
-    
-    def append_corpus(self, corpus:str) -> None:
-        self.corpus += corpus
-    
     def get_header_level(self) -> int:
         return self.headerNumber
     
     def add_child(self, child:Node) -> None:
         self.children.append(child)
         
 class MarkdownTree:
     
     def __init__(self, root:Node):
         self.root = root
-        self.words = root.get_corpus().split()
-        self.wordCount = len(self.words)
-        self.vocab = set(self.words)
-        self.vocabSize = len(self.vocab)
         
     def __str__(self):
         # Helper function to print the tree
         def printTree(root:Node, markerStr="+- ", levelMarkers=[]):
             returnStr = ""
             emptyStr = " " * len(markerStr)
             connectionStr = "|" + emptyStr[:-1]
@@ -104,28 +83,26 @@
         return printTree(self.root)
         
     def get_root(self):
         return self.root
     
 class MarkdownForest:
     
-    def __init__(self, documentName:str="[document]", metadata:dict=None):
+    def __init__(self, documentName:str="[document]", metadata=None):
         self.documentName = documentName
         self.metadata = metadata
         self.trees = []
-        self.treeCount   = 0
         self.backlinks = []
         self.tags = []
+        self.treeCount = 0
         
     def __str__(self):
         return f"[{self.documentName}]\n" + "\n".join(map(str, self.trees))
     
     def __getitem__(self, index:int):
-        if index < 0 or index >= self.treeCount:
-            raise IndexError("Index out of bounds")
         return self.trees[index]
     
     def __len__(self):
         return self.treeCount
 
     def get_metadata(self):
         return self.metadata
```

### Comparing `mdforest-1.4.0/mdforest/treebuild.py` & `mdforest-1.5.0/mdforest/treebuild.py`

 * *Files identical despite different names*

### Comparing `mdforest-1.4.0/mdforest.egg-info/PKG-INFO` & `mdforest-1.5.0/mdforest.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 Metadata-Version: 2.1
 Name: mdforest
-Version: 1.4.0
+Version: 1.5.0
 Summary: A package to convert between Markdown and a forest data structure for efficient processing.
 Home-page: http://github.com/kj3moraes/mdforest
 Author: Keane Moraes
 Author-email: lordvader3002@gmail.com
 License: Apache 2.0
-Download-URL: https://github.com/kj3moraes/mdforest/archive/1.4.0.zip
+Download-URL: https://github.com/kj3moraes/mdforest/archive/1.5.0.zip
 Platform: UNKNOWN
 Classifier: Topic :: Utilities
 License-File: LICENSE
 
-.. image:: media/forest-icon.png
-   :width: 100
-
 mdforest - Markdown Forest
 ==========================
 
 A library to convert Markdown documents into tree data structures and
 vice versa. There is greater functionality available to modify, prune,
 add and delete parts of documents when there are in the MarkdownTree
 structure.
```

### Comparing `mdforest-1.4.0/setup.py` & `mdforest-1.5.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 from setuptools import setup
 from setuptools.command.test import test as TestCommand
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 LONG_DESCRIPTION = (this_directory / "README.rst").read_text()
 
-VERSION = '1.4.0'
+VERSION = '1.5.0'
 DESCRIPTION = 'A package to convert between Markdown and a forest data structure for efficient processing.'
 
 setup(
     name = "mdforest",
     version = VERSION,
     author = "Keane Moraes",
     author_email = 'lordvader3002@gmail.com',
     description = DESCRIPTION,
     long_description=LONG_DESCRIPTION,
-    readme="README.rst",
     license = "Apache 2.0",
     url = "http://github.com/kj3moraes/mdforest",
     packages = ['mdforest', 'mdforest.tree'],
     tests_require = ['unittest'],
     install_requires = ['markdown', 'beautifulsoup4', 'python-frontmatter'],
     download_url = 'https://github.com/kj3moraes/mdforest/archive/%s.zip' % VERSION,
     classifiers = [
```

### Comparing `mdforest-1.4.0/tests/test_mdtree.py` & `mdforest-1.5.0/tests/test_mdtree.py`

 * *Files identical despite different names*

