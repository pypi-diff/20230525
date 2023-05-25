# Comparing `tmp/reasoner-pydantic-4.0.5.tar.gz` & `tmp/reasoner-pydantic-4.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasoner-pydantic-4.0.5.tar", last modified: Mon May 15 15:50:32 2023, max compression
+gzip compressed data, was "reasoner-pydantic-4.0.6.tar", last modified: Thu May 25 14:35:27 2023, max compression
```

## Comparing `reasoner-pydantic-4.0.5.tar` & `reasoner-pydantic-4.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:50:32.230150 reasoner-pydantic-4.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-15 15:50:32.230150 reasoner-pydantic-4.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-05-15 15:50:28.000000 reasoner-pydantic-4.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:50:32.230150 reasoner-pydantic-4.0.5/reasoner_pydantic/
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-15 15:50:28.000000 reasoner-pydantic-4.0.5/reasoner_pydantic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-15 15:50:28.000000 reasoner-pydantic-4.0.5/reasoner_pydantic/auxgraphs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-15 15:50:28.000000 reasoner-pydantic-4.0.5/reasoner_pydantic/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-05-15 15:50:28.000000 reasoner-pydantic-4.0.5/reasoner_pydantic/kgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-05-15 15:50:28.000000 reasoner-pydantic-4.0.5/reasoner_pydantic/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-15 15:50:28.000000 reasoner-pydantic-4.0.5/reasoner_pydantic/metakg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-05-15 15:50:28.000000 reasoner-pydantic-4.0.5/reasoner_pydantic/qgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-05-15 15:50:28.000000 reasoner-pydantic-4.0.5/reasoner_pydantic/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-05-15 15:50:28.000000 reasoner-pydantic-4.0.5/reasoner_pydantic/shared.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-15 15:50:28.000000 reasoner-pydantic-4.0.5/reasoner_pydantic/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12049 2023-05-15 15:50:28.000000 reasoner-pydantic-4.0.5/reasoner_pydantic/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 15:50:32.230150 reasoner-pydantic-4.0.5/reasoner_pydantic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-15 15:50:32.000000 reasoner-pydantic-4.0.5/reasoner_pydantic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-15 15:50:32.000000 reasoner-pydantic-4.0.5/reasoner_pydantic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 15:50:32.000000 reasoner-pydantic-4.0.5/reasoner_pydantic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 15:50:32.000000 reasoner-pydantic-4.0.5/reasoner_pydantic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-15 15:50:32.000000 reasoner-pydantic-4.0.5/reasoner_pydantic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-15 15:50:32.000000 reasoner-pydantic-4.0.5/reasoner_pydantic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 15:50:32.230150 reasoner-pydantic-4.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-15 15:50:28.000000 reasoner-pydantic-4.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:35:27.026882 reasoner-pydantic-4.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-25 14:35:27.026882 reasoner-pydantic-4.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-05-25 14:35:21.000000 reasoner-pydantic-4.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:35:27.022882 reasoner-pydantic-4.0.6/reasoner_pydantic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-25 14:35:21.000000 reasoner-pydantic-4.0.6/reasoner_pydantic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-25 14:35:21.000000 reasoner-pydantic-4.0.6/reasoner_pydantic/auxgraphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-25 14:35:21.000000 reasoner-pydantic-4.0.6/reasoner_pydantic/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-05-25 14:35:21.000000 reasoner-pydantic-4.0.6/reasoner_pydantic/kgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7085 2023-05-25 14:35:21.000000 reasoner-pydantic-4.0.6/reasoner_pydantic/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-25 14:35:21.000000 reasoner-pydantic-4.0.6/reasoner_pydantic/metakg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-05-25 14:35:21.000000 reasoner-pydantic-4.0.6/reasoner_pydantic/qgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-05-25 14:35:21.000000 reasoner-pydantic-4.0.6/reasoner_pydantic/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-05-25 14:35:21.000000 reasoner-pydantic-4.0.6/reasoner_pydantic/shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-25 14:35:21.000000 reasoner-pydantic-4.0.6/reasoner_pydantic/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12049 2023-05-25 14:35:21.000000 reasoner-pydantic-4.0.6/reasoner_pydantic/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:35:27.026882 reasoner-pydantic-4.0.6/reasoner_pydantic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-25 14:35:26.000000 reasoner-pydantic-4.0.6/reasoner_pydantic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-25 14:35:27.000000 reasoner-pydantic-4.0.6/reasoner_pydantic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 14:35:26.000000 reasoner-pydantic-4.0.6/reasoner_pydantic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 14:35:26.000000 reasoner-pydantic-4.0.6/reasoner_pydantic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-25 14:35:26.000000 reasoner-pydantic-4.0.6/reasoner_pydantic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-25 14:35:26.000000 reasoner-pydantic-4.0.6/reasoner_pydantic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 14:35:27.026882 reasoner-pydantic-4.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-25 14:35:21.000000 reasoner-pydantic-4.0.6/setup.py
```

### Comparing `reasoner-pydantic-4.0.5/PKG-INFO` & `reasoner-pydantic-4.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasoner-pydantic
-Version: 4.0.5
+Version: 4.0.6
 Summary: Pydantic models for the Reasoner API data formats
 Home-page: https://github.com/TranslatorSRI/reasoner-pydantic
 Author: Kenneth Morton
 Author-email: kenny@covar.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `reasoner-pydantic-4.0.5/README.md` & `reasoner-pydantic-4.0.6/README.md`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.5/reasoner_pydantic/__init__.py` & `reasoner-pydantic-4.0.6/reasoner_pydantic/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.5/reasoner_pydantic/auxgraphs.py` & `reasoner-pydantic-4.0.6/reasoner_pydantic/auxgraphs.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.5/reasoner_pydantic/base_model.py` & `reasoner-pydantic-4.0.6/reasoner_pydantic/base_model.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.5/reasoner_pydantic/kgraph.py` & `reasoner-pydantic-4.0.6/reasoner_pydantic/kgraph.py`

 * *Files 14% similar despite different names*

```diff
@@ -61,14 +61,24 @@
 
     resource_role: ResourceRoleEnum = Field(..., title="source type")
 
     upstream_resource_ids: Optional[HashableSet[CURIE]] = Field(None, nullable=True)
 
     source_record_urls: Optional[HashableSet[str]] = Field(None, nullable=True)
 
+    def __hash__(self) -> int:
+        return hash((self.resource_id, self.resource_role))
+
+    def update(self, other):
+        if other.upstream_resource_ids:
+            if self.upstream_resource_ids:
+                self.upstream_resource_ids.update(other.upstream_resource_ids)
+            else:
+                self.upstream_resource_ids = other.upstream_resource_ids
+
 
 class Edge(BaseModel):
     """Knowledge graph edge."""
 
     subject: CURIE = Field(
         ...,
         title="subject node id",
```

### Comparing `reasoner-pydantic-4.0.5/reasoner_pydantic/message.py` & `reasoner-pydantic-4.0.6/reasoner_pydantic/message.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,21 +43,21 @@
 
     def parse_obj(obj):
         message = parse_obj_as(Message, obj)
         qgraph = None
         kgraph = None
         results = None
         auxgraphs = None
-        if "query_graph" in obj.keys() and obj["query_graph"]:
+        if "query_graph" in obj.keys() and obj["query_graph"] is not None:
             qgraph = QueryGraph.parse_obj(obj["query_graph"])
-        if "knowledge_graph" in obj.keys() and obj["knowledge_graph"]:
+        if "knowledge_graph" in obj.keys() and obj["knowledge_graph"] is not None:
             kgraph = KnowledgeGraph.parse_obj(obj["knowledge_graph"])
-        if "results" in obj.keys() and obj["results"]:
+        if "results" in obj.keys() and obj["results"] is not None:
             results = Results.parse_obj(obj["results"])
-        if "auxiliary_graphs" in obj.keys() and obj["auxiliary_graphs"]:
+        if "auxiliary_graphs" in obj.keys() and obj["auxiliary_graphs"] is not None:
             auxgraphs = AuxiliaryGraphs.parse_obj(obj["auxiliary_graphs"])
         m = Message(
             query_graph=qgraph,
             knowledge_graph=kgraph,
             results=results,
             auxiliary_graphs=auxgraphs,
         )
```

### Comparing `reasoner-pydantic-4.0.5/reasoner_pydantic/metakg.py` & `reasoner-pydantic-4.0.6/reasoner_pydantic/metakg.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.5/reasoner_pydantic/qgraph.py` & `reasoner-pydantic-4.0.6/reasoner_pydantic/qgraph.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.5/reasoner_pydantic/results.py` & `reasoner-pydantic-4.0.6/reasoner_pydantic/results.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Results models."""
 from typing import Optional
 
 from pydantic import Field, parse_obj_as
 
 from .base_model import BaseModel
-from .utils import HashableMapping, HashableSet
+from .utils import HashableMapping, HashableSet, HashableSequence
 from .shared import Attribute, CURIE
 
 
 class EdgeBinding(BaseModel):
     """Edge binding."""
 
     id: str = Field(
@@ -64,19 +64,28 @@
                 self.score,
                 self.support_graphs,
                 self.scoring_method,
             )
         )
 
     def update(self, other):
+        for k in self.edge_bindings.keys():
+            eb = other.edge_bindings.get(k)
+            if eb:
+                self.edge_bindings[k].update(eb)
         if other.attributes:
             if self.attributes:
                 self.attributes.update(other.attributes)
             else:
                 self.attributes = other.attributes
+        if other.support_graphs:
+            if self.support_graphs:
+                self.support_graphs.update(other.support_graphs)
+            else:
+                self.support_graphs = other.support_graphs
 
 
 class NodeBinding(BaseModel):
     """Node binding."""
 
     id: CURIE = Field(
         ...,
@@ -137,14 +146,33 @@
         if "analyses" in obj.keys():
             for analysis in obj["analyses"]:
                 analyses.add(Analysis.parse_obj(analysis))
         r = Result(node_bindings=nbindings, analyses=analyses)
         result.update(r)
         return result
 
+    def combine_analyses_by_resource_id(self):
+        combine = HashableMapping[str, Analysis]()
+        analyses = HashableSequence.parse_obj([analysis for analysis in self.analyses])
+        for i, analysis in enumerate(analyses):
+            if analysis.resource_id not in combine:
+                combine[analysis.resource_id] = analysis
+            for j, analysis_to_compare in enumerate(analyses[i + 1 :]):
+                if (
+                    analysis.resource_id == analysis_to_compare.resource_id
+                    and analysis != analysis_to_compare
+                ):
+                    combine[analysis.resource_id].update(analysis_to_compare)
+
+        combined_analyses = HashableSet[Analysis]()
+        for analysis in combine.values():
+            combined_analyses.add(analysis)
+
+        self.analyses = combined_analyses
+
 
 class Results(BaseModel):
     """Results."""
 
     __root__: Optional[HashableSet[Result]]
 
     class Config:
```

### Comparing `reasoner-pydantic-4.0.5/reasoner_pydantic/shared.py` & `reasoner-pydantic-4.0.6/reasoner_pydantic/shared.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.5/reasoner_pydantic/utils.py` & `reasoner-pydantic-4.0.6/reasoner_pydantic/utils.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.5/reasoner_pydantic/workflow.py` & `reasoner-pydantic-4.0.6/reasoner_pydantic/workflow.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.5/reasoner_pydantic.egg-info/PKG-INFO` & `reasoner-pydantic-4.0.6/reasoner_pydantic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasoner-pydantic
-Version: 4.0.5
+Version: 4.0.6
 Summary: Pydantic models for the Reasoner API data formats
 Home-page: https://github.com/TranslatorSRI/reasoner-pydantic
 Author: Kenneth Morton
 Author-email: kenny@covar.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `reasoner-pydantic-4.0.5/reasoner_pydantic.egg-info/SOURCES.txt` & `reasoner-pydantic-4.0.6/reasoner_pydantic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.5/setup.py` & `reasoner-pydantic-4.0.6/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="reasoner-pydantic",
-    version="4.0.5",
+    version="4.0.6",
     author="Kenneth Morton",
     author_email="kenny@covar.com",
     url="https://github.com/TranslatorSRI/reasoner-pydantic",
     description="Pydantic models for the Reasoner API data formats",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=["reasoner_pydantic"],
```

