# Comparing `tmp/TCFnetworks-0.2.2.tar.gz` & `tmp/TCFnetworks-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/TCFnetworks-0.2.2.tar", last modified: Mon Jun 29 10:33:44 2015, max compression
+gzip compressed data, was "TCFnetworks-0.3.0.tar", last modified: Thu May 25 07:11:51 2023, max compression
```

## Comparing `TCFnetworks-0.2.2.tar` & `TCFnetworks-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,28 @@
-drwxr-x---   0 frederik  (1000) frederik  (1000)        0 2015-06-29 10:33:44.000000 TCFnetworks-0.2.2/
--rw-r-----   0 frederik  (1000) frederik  (1000)      260 2015-06-29 10:33:44.000000 TCFnetworks-0.2.2/PKG-INFO
--rw-r-----   0 frederik  (1000) frederik  (1000)      577 2015-06-29 10:29:29.000000 TCFnetworks-0.2.2/setup.py
--rw-r-----   0 frederik  (1000) frederik  (1000)       40 2015-05-12 09:12:15.000000 TCFnetworks-0.2.2/setup.cfg
-drwxr-x---   0 frederik  (1000) frederik  (1000)        0 2015-06-29 10:33:44.000000 TCFnetworks-0.2.2/tcfnetworks/
--rw-r-----   0 frederik  (1000) frederik  (1000)        0 2014-06-05 13:23:01.000000 TCFnetworks-0.2.2/tcfnetworks/__init__.py
-drwxr-x---   0 frederik  (1000) frederik  (1000)        0 2015-06-29 10:33:44.000000 TCFnetworks-0.2.2/tcfnetworks/annotators/
--rw-r-----   0 frederik  (1000) frederik  (1000)     7418 2015-06-29 10:21:35.000000 TCFnetworks-0.2.2/tcfnetworks/annotators/cooccurrence.py
--rw-r-----   0 frederik  (1000) frederik  (1000)        0 2014-06-05 13:23:01.000000 TCFnetworks-0.2.2/tcfnetworks/annotators/__init__.py
--rw-r-----   0 frederik  (1000) frederik  (1000)    11017 2015-05-12 09:12:16.000000 TCFnetworks-0.2.2/tcfnetworks/annotators/dependency.py
--rw-r-----   0 frederik  (1000) frederik  (1000)     6495 2015-06-29 10:21:29.000000 TCFnetworks-0.2.2/tcfnetworks/annotators/base.py
-drwxr-x---   0 frederik  (1000) frederik  (1000)        0 2015-06-29 10:33:44.000000 TCFnetworks-0.2.2/tcfnetworks/exporters/
--rw-r-----   0 frederik  (1000) frederik  (1000)        0 2014-06-05 13:23:01.000000 TCFnetworks-0.2.2/tcfnetworks/exporters/__init__.py
-drwxr-x---   0 frederik  (1000) frederik  (1000)        0 2015-06-29 10:33:44.000000 TCFnetworks-0.2.2/tcfnetworks/exporters/data/
--rw-r-----   0 frederik  (1000) frederik  (1000)     2516 2015-05-12 09:12:16.000000 TCFnetworks-0.2.2/tcfnetworks/exporters/data/tcf2graphml.xsl
--rw-r-----   0 frederik  (1000) frederik  (1000)     2545 2014-06-05 13:23:01.000000 TCFnetworks-0.2.2/tcfnetworks/exporters/data/tcf2json.xsl
--rw-r-----   0 frederik  (1000) frederik  (1000)     1348 2015-05-12 09:12:16.000000 TCFnetworks-0.2.2/tcfnetworks/exporters/d3_json.py
--rw-r-----   0 frederik  (1000) frederik  (1000)     1417 2015-05-12 09:12:16.000000 TCFnetworks-0.2.2/tcfnetworks/exporters/graphml.py
+drwxrwxr-x   0 frederik  (1000) frederik  (1000)        0 2023-05-25 07:11:51.144517 TCFnetworks-0.3.0/
+-rw-r-----   0 frederik  (1000) frederik  (1000)    34520 2014-06-05 13:23:01.000000 TCFnetworks-0.3.0/COPYING
+-rw-rw-r--   0 frederik  (1000) frederik  (1000)      226 2023-05-25 07:11:51.144517 TCFnetworks-0.3.0/PKG-INFO
+-rw-r-----   0 frederik  (1000) frederik  (1000)     1753 2015-05-12 09:12:15.000000 TCFnetworks-0.3.0/README.md
+drwxrwxr-x   0 frederik  (1000) frederik  (1000)        0 2023-05-25 07:11:51.132517 TCFnetworks-0.3.0/TCFnetworks.egg-info/
+-rw-r-----   0 frederik  (1000) frederik  (1000)      226 2023-05-25 07:11:50.000000 TCFnetworks-0.3.0/TCFnetworks.egg-info/PKG-INFO
+-rw-r-----   0 frederik  (1000) frederik  (1000)      623 2023-05-25 07:11:51.000000 TCFnetworks-0.3.0/TCFnetworks.egg-info/SOURCES.txt
+-rw-r-----   0 frederik  (1000) frederik  (1000)        1 2023-05-25 07:11:50.000000 TCFnetworks-0.3.0/TCFnetworks.egg-info/dependency_links.txt
+-rw-r-----   0 frederik  (1000) frederik  (1000)       46 2015-07-28 16:47:59.000000 TCFnetworks-0.3.0/TCFnetworks.egg-info/pbr.json
+-rw-r-----   0 frederik  (1000) frederik  (1000)       12 2023-05-25 07:11:50.000000 TCFnetworks-0.3.0/TCFnetworks.egg-info/top_level.txt
+-rw-r-----   0 frederik  (1000) frederik  (1000)       79 2023-05-25 07:11:51.144517 TCFnetworks-0.3.0/setup.cfg
+-rw-r-----   0 frederik  (1000) frederik  (1000)      640 2023-05-25 07:03:51.000000 TCFnetworks-0.3.0/setup.py
+drwxrwxr-x   0 frederik  (1000) frederik  (1000)        0 2023-05-25 07:11:51.132517 TCFnetworks-0.3.0/tcfnetworks/
+-rw-r-----   0 frederik  (1000) frederik  (1000)        0 2014-06-05 13:23:01.000000 TCFnetworks-0.3.0/tcfnetworks/__init__.py
+drwxrwxr-x   0 frederik  (1000) frederik  (1000)        0 2023-05-25 07:11:51.136517 TCFnetworks-0.3.0/tcfnetworks/annotators/
+-rw-r-----   0 frederik  (1000) frederik  (1000)        0 2014-06-05 13:23:01.000000 TCFnetworks-0.3.0/tcfnetworks/annotators/__init__.py
+-rw-r-----   0 frederik  (1000) frederik  (1000)     6495 2015-06-29 10:21:29.000000 TCFnetworks-0.3.0/tcfnetworks/annotators/base.py
+-rw-r-----   0 frederik  (1000) frederik  (1000)     7713 2023-05-25 07:01:12.000000 TCFnetworks-0.3.0/tcfnetworks/annotators/cooccurrence.py
+-rw-r-----   0 frederik  (1000) frederik  (1000)    11017 2015-05-12 09:12:16.000000 TCFnetworks-0.3.0/tcfnetworks/annotators/dependency.py
+drwxrwxr-x   0 frederik  (1000) frederik  (1000)        0 2023-05-25 07:11:51.136517 TCFnetworks-0.3.0/tcfnetworks/exporters/
+-rw-r-----   0 frederik  (1000) frederik  (1000)        0 2014-06-05 13:23:01.000000 TCFnetworks-0.3.0/tcfnetworks/exporters/__init__.py
+-rw-rw-r--   0 frederik  (1000) frederik  (1000)     1438 2023-05-19 08:04:46.000000 TCFnetworks-0.3.0/tcfnetworks/exporters/d3_html.py
+-rw-rw-r--   0 frederik  (1000) frederik  (1000)     3111 2023-05-19 08:04:46.000000 TCFnetworks-0.3.0/tcfnetworks/exporters/d3_json.py
+drwxrwxr-x   0 frederik  (1000) frederik  (1000)        0 2023-05-25 07:11:51.144517 TCFnetworks-0.3.0/tcfnetworks/exporters/data/
+-rw-rw-r--   0 frederik  (1000) frederik  (1000)     5971 2023-05-19 08:04:46.000000 TCFnetworks-0.3.0/tcfnetworks/exporters/data/d3.html
+-rwxrwxr-x   0 frederik  (1000) frederik  (1000)   144406 2023-05-19 08:04:46.000000 TCFnetworks-0.3.0/tcfnetworks/exporters/data/d3.v3.min.js
+-rw-r-----   0 frederik  (1000) frederik  (1000)     2516 2015-05-12 09:12:16.000000 TCFnetworks-0.3.0/tcfnetworks/exporters/data/tcf2graphml.xsl
+-rw-r-----   0 frederik  (1000) frederik  (1000)     1417 2015-05-12 09:12:16.000000 TCFnetworks-0.3.0/tcfnetworks/exporters/graphml.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `TCFnetworks-0.2.2/setup.py` & `TCFnetworks-0.3.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 from distutils.core import setup
 from glob import glob
 
 setup(name='TCFnetworks',
-      version='0.2.2',
+      version='0.3.0',
       description='Python TCF network services',
       author='Frederik Elwert',
       author_email='frederik.elwert@web.de',
       url='https://github.com/SeNeReKo/TCFnetworks',
       packages=['tcfnetworks', 'tcfnetworks.annotators',
                 'tcfnetworks.exporters'],
       package_data={'tcfnetworks.exporters': ['data/tcf2graphml.xsl',
-                                              'data/tcf2json.xsl']},
-     )
+                                              'data/d3.v3.min.js',
+                                              'data/d3.html']},
+      )
```

### Comparing `TCFnetworks-0.2.2/tcfnetworks/annotators/cooccurrence.py` & `TCFnetworks-0.3.0/tcfnetworks/annotators/cooccurrence.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 import sys
 import os
 import logging
 from itertools import combinations
 from collections import Counter
 from math import log
 
+from tqdm import tqdm
 from tcflib import tcf
 from tcflib.service import run_as_cli
 
 from tcfnetworks.annotators.base import TokenTestingWorker
 
 
 def n_grams(a, n, nofadeout=False):
@@ -53,19 +54,22 @@
     __options__ = TokenTestingWorker.__options__.copy()
     __options__.update({
         'method': 'window',  # 'window', 'sentence' or 'textspan'
         'spantype': '',
         'window': [2, 5],  # for method='window'
         'nofadeout': False,  # prevent thin connections at span borders
         'unique': False,
-        'weight': 'count',  # 'count' or 'loglikelihood'
+        'weight': 'count',  # 'count', 'llr' or 'pmi'
     })
 
     def __init__(self, **options):
         super().__init__(**options)
+        if self.options.weight in ('llr', 'pmi') and not self.options.unique:
+            logging.warning('Cooccurrence measures only work with '
+                            'unique=True.')
         try:
             self.build_graph = getattr(self,
                     'build_graph_{}'.format(self.options.method))
         except AttributeError:
             logging.error('Method "{}" is not supported.'.format(
                     self.options.method))
             sys.exit(-1)
@@ -129,18 +133,19 @@
         :returns:
             - The graph node.
 
         """
         if graph == None:
             graph = tcf.Graph(label=self.options.label,
                               weight=self.options.weight)
-        for token in tokens:
+        for token in tqdm(tokens, desc='Adding nodes'):
             graph.node_for_token(token)
-        for n_gram in n_grams(tokens, window,
-                              nofadeout=self.options.nofadeout):
+        for n_gram in tqdm(n_grams(tokens, window,
+                                   nofadeout=self.options.nofadeout),
+                           desc='Adding edges'):
             # try all combinations of words within window
             for combo in combinations(n_gram, 2):
                 try:
                     graph.edge_for_tokens(*combo, unique=self.options.unique)
                 except tcf.LoopError:
                     continue
         return graph
```

### Comparing `TCFnetworks-0.2.2/tcfnetworks/annotators/dependency.py` & `TCFnetworks-0.3.0/tcfnetworks/annotators/dependency.py`

 * *Files identical despite different names*

### Comparing `TCFnetworks-0.2.2/tcfnetworks/annotators/base.py` & `TCFnetworks-0.3.0/tcfnetworks/annotators/base.py`

 * *Files identical despite different names*

### Comparing `TCFnetworks-0.2.2/tcfnetworks/exporters/data/tcf2graphml.xsl` & `TCFnetworks-0.3.0/tcfnetworks/exporters/data/tcf2graphml.xsl`

 * *Files identical despite different names*

### Comparing `TCFnetworks-0.2.2/tcfnetworks/exporters/d3_json.py` & `TCFnetworks-0.3.0/tcfnetworks/exporters/graphml.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,32 +13,32 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 """
-JSON exporter for TCF graphs.
+GraphML exporter for TCF graphs.
 
 """
 
 import os.path
 
 from lxml import etree
 from tcflib import tcf
 from tcflib.service import ExportingWorker, run_as_cli
 
 
-class JSONWorker(ExportingWorker):
+class GraphMLWorker(ExportingWorker):
 
     def export(self):
         input_tree = self.corpus.tree
         xslt_file = os.path.join(os.path.dirname(__file__),
-                                 'data', 'tcf2json.xsl')
+                                 'data', 'tcf2graphml.xsl')
         xslt_tree = etree.parse(xslt_file)
         transform = etree.XSLT(xslt_tree)
-        output = str(transform(input_tree))
-        return output
+        output_tree = transform(input_tree)
+        return etree.tostring(output_tree, encoding='utf8', pretty_print=True)
 
 
 if __name__ == '__main__':
-    run_as_cli(JSONWorker)
+    run_as_cli(GraphMLWorker)
```

