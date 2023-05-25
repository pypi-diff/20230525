# Comparing `tmp/lifelike-1.0.6.tar.gz` & `tmp/lifelike-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifelike-1.0.6.tar", last modified: Thu May 25 17:41:21 2023, max compression
+gzip compressed data, was "lifelike-1.0.7.tar", last modified: Thu May 25 21:55:48 2023, max compression
```

## Comparing `lifelike-1.0.6.tar` & `lifelike-1.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 mustafa    (501) staff       (20)        0 2023-05-25 17:41:21.206146 lifelike-1.0.6/
--rw-r--r--   0 mustafa    (501) staff       (20)     1073 2023-05-25 17:39:04.000000 lifelike-1.0.6/LICENSE.txt
--rw-r--r--   0 mustafa    (501) staff       (20)      270 2023-05-25 17:41:21.206213 lifelike-1.0.6/PKG-INFO
--rw-r--r--   0 mustafa    (501) staff       (20)     2758 2023-05-25 17:39:04.000000 lifelike-1.0.6/README.md
-drwxr-xr-x   0 mustafa    (501) staff       (20)        0 2023-05-25 17:41:21.204331 lifelike-1.0.6/lifelike/
-drwxr-xr-x   0 mustafa    (501) staff       (20)        0 2023-05-25 17:41:21.205981 lifelike-1.0.6/lifelike/StateManager/
--rw-r--r--   0 mustafa    (501) staff       (20)        0 2023-05-25 17:39:04.000000 lifelike-1.0.6/lifelike/StateManager/__init__.py
--rw-r--r--   0 mustafa    (501) staff       (20)    15662 2023-05-25 17:39:04.000000 lifelike-1.0.6/lifelike/StateManager/base_game_tree.py
--rw-r--r--   0 mustafa    (501) staff       (20)      962 2023-05-25 17:39:04.000000 lifelike-1.0.6/lifelike/StateManager/knowledge_tree.py
--rw-r--r--   0 mustafa    (501) staff       (20)     2131 2023-05-25 17:39:04.000000 lifelike-1.0.6/lifelike/StateManager/sequence_tree.py
--rw-r--r--   0 mustafa    (501) staff       (20)        0 2023-05-25 17:39:04.000000 lifelike-1.0.6/lifelike/__init__.py
--rw-r--r--   0 mustafa    (501) staff       (20)     8371 2023-05-25 17:39:04.000000 lifelike-1.0.6/lifelike/brain.py
--rw-r--r--   0 mustafa    (501) staff       (20)      499 2023-05-25 17:39:04.000000 lifelike-1.0.6/lifelike/state.py
-drwxr-xr-x   0 mustafa    (501) staff       (20)        0 2023-05-25 17:41:21.205250 lifelike-1.0.6/lifelike.egg-info/
--rw-r--r--   0 mustafa    (501) staff       (20)      270 2023-05-25 17:41:21.000000 lifelike-1.0.6/lifelike.egg-info/PKG-INFO
--rw-r--r--   0 mustafa    (501) staff       (20)      409 2023-05-25 17:41:21.000000 lifelike-1.0.6/lifelike.egg-info/SOURCES.txt
--rw-r--r--   0 mustafa    (501) staff       (20)        1 2023-05-25 17:41:21.000000 lifelike-1.0.6/lifelike.egg-info/dependency_links.txt
--rw-r--r--   0 mustafa    (501) staff       (20)       10 2023-05-25 17:41:21.000000 lifelike-1.0.6/lifelike.egg-info/requires.txt
--rw-r--r--   0 mustafa    (501) staff       (20)        9 2023-05-25 17:41:21.000000 lifelike-1.0.6/lifelike.egg-info/top_level.txt
--rw-r--r--   0 mustafa    (501) staff       (20)       79 2023-05-25 17:41:21.206476 lifelike-1.0.6/setup.cfg
--rw-r--r--   0 mustafa    (501) staff       (20)      392 2023-05-25 17:39:04.000000 lifelike-1.0.6/setup.py
+drwxr-xr-x   0 mustafa    (501) staff       (20)        0 2023-05-25 21:55:48.640902 lifelike-1.0.7/
+-rw-r--r--   0 mustafa    (501) staff       (20)     1073 2023-05-25 21:53:12.000000 lifelike-1.0.7/LICENSE.txt
+-rw-r--r--   0 mustafa    (501) staff       (20)      270 2023-05-25 21:55:48.640971 lifelike-1.0.7/PKG-INFO
+-rw-r--r--   0 mustafa    (501) staff       (20)     2758 2023-05-25 21:53:12.000000 lifelike-1.0.7/README.md
+drwxr-xr-x   0 mustafa    (501) staff       (20)        0 2023-05-25 21:55:48.639105 lifelike-1.0.7/lifelike/
+drwxr-xr-x   0 mustafa    (501) staff       (20)        0 2023-05-25 21:55:48.640718 lifelike-1.0.7/lifelike/StateManager/
+-rw-r--r--   0 mustafa    (501) staff       (20)        0 2023-05-25 21:53:12.000000 lifelike-1.0.7/lifelike/StateManager/__init__.py
+-rw-r--r--   0 mustafa    (501) staff       (20)    15743 2023-05-25 21:53:12.000000 lifelike-1.0.7/lifelike/StateManager/base_game_tree.py
+-rw-r--r--   0 mustafa    (501) staff       (20)      962 2023-05-25 21:53:12.000000 lifelike-1.0.7/lifelike/StateManager/knowledge_tree.py
+-rw-r--r--   0 mustafa    (501) staff       (20)     2131 2023-05-25 21:53:12.000000 lifelike-1.0.7/lifelike/StateManager/sequence_tree.py
+-rw-r--r--   0 mustafa    (501) staff       (20)        0 2023-05-25 21:53:12.000000 lifelike-1.0.7/lifelike/__init__.py
+-rw-r--r--   0 mustafa    (501) staff       (20)     8371 2023-05-25 21:53:12.000000 lifelike-1.0.7/lifelike/brain.py
+-rw-r--r--   0 mustafa    (501) staff       (20)      499 2023-05-25 21:53:12.000000 lifelike-1.0.7/lifelike/state.py
+drwxr-xr-x   0 mustafa    (501) staff       (20)        0 2023-05-25 21:55:48.639983 lifelike-1.0.7/lifelike.egg-info/
+-rw-r--r--   0 mustafa    (501) staff       (20)      270 2023-05-25 21:55:48.000000 lifelike-1.0.7/lifelike.egg-info/PKG-INFO
+-rw-r--r--   0 mustafa    (501) staff       (20)      409 2023-05-25 21:55:48.000000 lifelike-1.0.7/lifelike.egg-info/SOURCES.txt
+-rw-r--r--   0 mustafa    (501) staff       (20)        1 2023-05-25 21:55:48.000000 lifelike-1.0.7/lifelike.egg-info/dependency_links.txt
+-rw-r--r--   0 mustafa    (501) staff       (20)       10 2023-05-25 21:55:48.000000 lifelike-1.0.7/lifelike.egg-info/requires.txt
+-rw-r--r--   0 mustafa    (501) staff       (20)        9 2023-05-25 21:55:48.000000 lifelike-1.0.7/lifelike.egg-info/top_level.txt
+-rw-r--r--   0 mustafa    (501) staff       (20)       79 2023-05-25 21:55:48.641235 lifelike-1.0.7/setup.cfg
+-rw-r--r--   0 mustafa    (501) staff       (20)      393 2023-05-25 21:55:42.000000 lifelike-1.0.7/setup.py
```

### Comparing `lifelike-1.0.6/LICENSE.txt` & `lifelike-1.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lifelike-1.0.6/README.md` & `lifelike-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `lifelike-1.0.6/lifelike/StateManager/base_game_tree.py` & `lifelike-1.0.7/lifelike/StateManager/base_game_tree.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
         Returns: The new embedding
         """
         if self._final:
             print("The Embedding is marked as Final. Cannot be tuned.")
             return None
 
-        new_embeddings = self.embed(prompts)
+        new_embeddings = self.embed.embed_documents(prompts)
 
         # Update weighted average
         self.embedding = numpy.average([self.embedding] + new_embeddings, 0, [self.weight]+[1]*len(prompts)).tolist()
 
         # Update weights
         self.weight += len(prompts)
         return self.embedding
@@ -147,15 +147,15 @@
         self._final = False # Final flag, determines if any change can be made to the tree
         # if flag is False, embedding_function will be used to determine embedding using document text
 
         if embedding_function is None:
             print('Tree {} was initialized in final mode'.format(name)) # TODO Final Mode might be excessive in constructor
             self._final = True # Activate Final flag
         
-        self.embed = embedding_function
+        self.embed = embedding_function # TODO Rename this, Embeddings is not a function
 
         # TODO add persistent option and metadata preset
         self.vectorstore = Chroma(name, self.embed) # Preset to Chroma TODO make this work with all vectorstore
 
         # Currently, if there are 2 ways to reach an event, a copy with a new unique id must be made
         self.node_dict = {} # id - SequenceEvent. Mostly for lookup
 
@@ -170,15 +170,15 @@
         Create GameNode and add to GameTree using add_node().
         Must be overriden if a child of GameNode is used.
         """
         if ids is None: # If id not provided, generate it
             ids = [str(uuid.uuid1()) for _ in texts]
 
         if custom_embeddings is None:
-            embeddings = self.embed(texts)
+            embeddings = self.embed.embed_documents(texts)
 
         # Text to tree. Does not allow for custom edges
         for i in range(len(texts)):
             node = GameNode(ids[i], texts[i], metadatas[i])
             edge = EdgeEmbedding(ids[i], self.embed, embeddings[i], 20) # Tunable embedding with default weight of 20
             self.add_node(node)
             self.add_edge('_', node.id, ids[i], edge)
```

### Comparing `lifelike-1.0.6/lifelike/StateManager/knowledge_tree.py` & `lifelike-1.0.7/lifelike/StateManager/knowledge_tree.py`

 * *Files identical despite different names*

### Comparing `lifelike-1.0.6/lifelike/StateManager/sequence_tree.py` & `lifelike-1.0.7/lifelike/StateManager/sequence_tree.py`

 * *Files identical despite different names*

### Comparing `lifelike-1.0.6/lifelike/brain.py` & `lifelike-1.0.7/lifelike/brain.py`

 * *Files identical despite different names*

