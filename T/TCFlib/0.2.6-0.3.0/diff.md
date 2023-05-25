# Comparing `tmp/TCFlib-0.2.6.tar.gz` & `tmp/TCFlib-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/TCFlib-0.2.6.tar", last modified: Thu Sep  6 12:41:23 2018, max compression
+gzip compressed data, was "TCFlib-0.3.0.tar", last modified: Thu May 25 07:07:34 2023, max compression
```

## Comparing `TCFlib-0.2.6.tar` & `TCFlib-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,26 @@
-drwxr-xr-x   0 frederik  (1000) frederik  (1000)        0 2018-09-06 12:41:23.000000 TCFlib-0.2.6/
--rw-r--r--   0 frederik  (1000) frederik  (1000)      405 2018-09-06 12:31:25.000000 TCFlib-0.2.6/setup.py
-drwxr-xr-x   0 frederik  (1000) frederik  (1000)        0 2018-09-06 12:41:23.000000 TCFlib-0.2.6/tcflib/
--rw-r--r--   0 frederik  (1000) frederik  (1000)        0 2018-09-05 14:20:14.000000 TCFlib-0.2.6/tcflib/__init__.py
--rwxrwxrwx   0 frederik  (1000) frederik  (1000)    17223 2014-06-17 17:56:33.000000 TCFlib-0.2.6/tcflib/tcf_alt.py
-drwxr-xr-x   0 frederik  (1000) frederik  (1000)        0 2018-09-06 12:41:23.000000 TCFlib-0.2.6/tcflib/tagsets/
--rw-r--r--   0 frederik  (1000) frederik  (1000)     1396 2018-09-05 14:20:14.000000 TCFlib-0.2.6/tcflib/tagsets/__init__.py
-drwxr-xr-x   0 frederik  (1000) frederik  (1000)        0 2018-09-06 12:41:23.000000 TCFlib-0.2.6/tcflib/tagsets/data/
--rw-r--r--   0 frederik  (1000) frederik  (1000)   223866 2018-09-05 14:20:14.000000 TCFlib-0.2.6/tcflib/tagsets/data/dc-1345.dcif
--rw-r--r--   0 frederik  (1000) frederik  (1000)     9250 2018-09-06 12:25:51.000000 TCFlib-0.2.6/tcflib/tagsets/hits.py
--rw-r--r--   0 frederik  (1000) frederik  (1000)     8105 2018-09-05 14:20:14.000000 TCFlib-0.2.6/tcflib/tagsets/base.py
--rw-r--r--   0 frederik  (1000) frederik  (1000)     2465 2018-09-05 14:20:14.000000 TCFlib-0.2.6/tcflib/tagsets/dc1345.py
--rw-r--r--   0 frederik  (1000) frederik  (1000)     5648 2018-09-05 14:20:14.000000 TCFlib-0.2.6/tcflib/tagsets/stts.py
--rw-r--r--   0 frederik  (1000) frederik  (1000)     3973 2018-09-05 14:20:14.000000 TCFlib-0.2.6/tcflib/tagsets/stein.py
--rw-r--r--   0 frederik  (1000) frederik  (1000)     6010 2018-09-05 14:20:14.000000 TCFlib-0.2.6/tcflib/tagsets/penntb.py
--rwxrwxrwx   0 frederik  (1000) frederik  (1000)     1447 2015-03-04 16:36:14.000000 TCFlib-0.2.6/tcflib/test.py
--rw-r--r--   0 frederik  (1000) frederik  (1000)    34871 2018-09-06 12:25:51.000000 TCFlib-0.2.6/tcflib/tcf.py
--rw-r--r--   0 frederik  (1000) frederik  (1000)     9184 2018-09-05 14:20:14.000000 TCFlib-0.2.6/tcflib/service.py
--rw-r--r--   0 frederik  (1000) frederik  (1000)       40 2018-09-05 14:20:14.000000 TCFlib-0.2.6/setup.cfg
--rw-r--r--   0 frederik  (1000) frederik  (1000)      241 2018-09-06 12:41:23.000000 TCFlib-0.2.6/PKG-INFO
+drwxrwxr-x   0 frederik  (1000) frederik  (1000)        0 2023-05-25 07:07:34.631400 TCFlib-0.3.0/
+-rw-r-----   0 frederik  (1000) frederik  (1000)     1084 2014-06-05 13:23:08.000000 TCFlib-0.3.0/COPYING
+-rw-rw-r--   0 frederik  (1000) frederik  (1000)      207 2023-05-25 07:07:34.631400 TCFlib-0.3.0/PKG-INFO
+-rw-r-----   0 frederik  (1000) frederik  (1000)      827 2015-05-11 14:33:30.000000 TCFlib-0.3.0/README.md
+drwxrwxr-x   0 frederik  (1000) frederik  (1000)        0 2023-05-25 07:07:34.627400 TCFlib-0.3.0/TCFlib.egg-info/
+-rw-r-----   0 frederik  (1000) frederik  (1000)      207 2023-05-25 07:07:34.000000 TCFlib-0.3.0/TCFlib.egg-info/PKG-INFO
+-rw-r-----   0 frederik  (1000) frederik  (1000)      435 2023-05-25 07:07:34.000000 TCFlib-0.3.0/TCFlib.egg-info/SOURCES.txt
+-rw-r-----   0 frederik  (1000) frederik  (1000)        1 2023-05-25 07:07:34.000000 TCFlib-0.3.0/TCFlib.egg-info/dependency_links.txt
+-rw-r-----   0 frederik  (1000) frederik  (1000)       47 2015-07-28 16:47:47.000000 TCFlib-0.3.0/TCFlib.egg-info/pbr.json
+-rw-r-----   0 frederik  (1000) frederik  (1000)        7 2023-05-25 07:07:34.000000 TCFlib-0.3.0/TCFlib.egg-info/top_level.txt
+-rw-r-----   0 frederik  (1000) frederik  (1000)       79 2023-05-25 07:07:34.631400 TCFlib-0.3.0/setup.cfg
+-rw-r--r--   0 frederik  (1000) frederik  (1000)      424 2023-05-25 07:02:37.000000 TCFlib-0.3.0/setup.py
+drwxrwxr-x   0 frederik  (1000) frederik  (1000)        0 2023-05-25 07:07:34.627400 TCFlib-0.3.0/tcflib/
+-rw-r-----   0 frederik  (1000) frederik  (1000)        0 2014-06-05 13:23:08.000000 TCFlib-0.3.0/tcflib/__init__.py
+-rw-r-----   0 frederik  (1000) frederik  (1000)     9184 2015-06-29 10:20:31.000000 TCFlib-0.3.0/tcflib/service.py
+drwxrwxr-x   0 frederik  (1000) frederik  (1000)        0 2023-05-25 07:07:34.627400 TCFlib-0.3.0/tcflib/tagsets/
+-rw-r-----   0 frederik  (1000) frederik  (1000)     1396 2014-06-05 13:23:08.000000 TCFlib-0.3.0/tcflib/tagsets/__init__.py
+-rw-r-----   0 frederik  (1000) frederik  (1000)     8105 2014-11-18 10:34:51.000000 TCFlib-0.3.0/tcflib/tagsets/base.py
+drwxrwxr-x   0 frederik  (1000) frederik  (1000)        0 2023-05-25 07:07:34.631400 TCFlib-0.3.0/tcflib/tagsets/data/
+-rw-r-----   0 frederik  (1000) frederik  (1000)   223866 2014-06-05 13:23:08.000000 TCFlib-0.3.0/tcflib/tagsets/data/dc-1345.dcif
+-rw-r-----   0 frederik  (1000) frederik  (1000)     2465 2015-07-14 08:37:52.000000 TCFlib-0.3.0/tcflib/tagsets/dc1345.py
+-rw-r--r--   0 frederik  (1000) frederik  (1000)     9385 2019-02-26 09:41:07.000000 TCFlib-0.3.0/tcflib/tagsets/hits.py
+-rw-r-----   0 frederik  (1000) frederik  (1000)     6372 2023-05-11 10:00:02.000000 TCFlib-0.3.0/tcflib/tagsets/penntb.py
+-rw-r-----   0 frederik  (1000) frederik  (1000)     3973 2014-07-28 13:56:53.000000 TCFlib-0.3.0/tcflib/tagsets/stein.py
+-rw-r-----   0 frederik  (1000) frederik  (1000)     5723 2018-12-05 09:04:11.000000 TCFlib-0.3.0/tcflib/tagsets/stts.py
+-rw-rw-r--   0 frederik  (1000) frederik  (1000)    37192 2023-05-19 14:15:25.000000 TCFlib-0.3.0/tcflib/tcf.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `TCFlib-0.2.6/tcflib/tagsets/__init__.py` & `TCFlib-0.3.0/tcflib/tagsets/__init__.py`

 * *Files identical despite different names*

### Comparing `TCFlib-0.2.6/tcflib/tagsets/data/dc-1345.dcif` & `TCFlib-0.3.0/tcflib/tagsets/data/dc-1345.dcif`

 * *Files identical despite different names*

### Comparing `TCFlib-0.2.6/tcflib/tagsets/hits.py` & `TCFlib-0.3.0/tcflib/tagsets/hits.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,16 @@
         'PAVD': 'http://www.isocat.org/datcat/DC-2998',  # pronominalAdverb; Pronominaladverb, pronominaler Teil
         'PAVG': 'http://www.isocat.org/datcat/DC-2998',  # pronominalAdverb; Pronominaladverb, pronominaler Teil, generalisierend
         'PAVW': 'http://www.isocat.org/datcat/DC-2998',  # pronominalAdverb; Pronominaladverb, pronominaler Teil, interrogativ
         'PG': 'http://www.isocat.org/datcat/DC-1370',  # pronoun; Pronomen, generalisierend
         'PI': 'http://www.isocat.org/datcat/DC-1309',  # indefinitePronoun; Pronomen, indefinit
         'PPER': 'http://www.isocat.org/datcat/DC-3013',  # irreflexivePersonalPronoun; Pronomen, personal, irreflexiv
         'PRF': 'http://www.isocat.org/datcat/DC-3014',  # reflexivePersonalPronoun; Pronomen, personal, reflexiv
+        'PTK': 'http://www.isocat.org/datcat/DC-1342',  # particle
+        'PTK*': 'http://www.isocat.org/datcat/DC-1342',  # particle
         'PTKA': 'http://www.isocat.org/datcat/DC-1922',  # comparativeParticle; Partikel bei Adjektiv oder Adverb
         'PTKANT': 'http://www.isocat.org/datcat/DC-1342',  # particle; Antwortpartikel
         'PTKNEG': 'http://www.isocat.org/datcat/DC-1894',  # negativeParticle; Negationspartikel
         'PTKVZ': 'http://www.isocat.org/datcat/DC-1342',  # particle; Verbzusatz
         'PW': 'http://www.isocat.org/datcat/DC-1321',  # interrogativePronoun; Pronomen, interrogativ
         'VAFIN': 'http://www.isocat.org/datcat/DC-1263',  # copula; Auxiliar, finit
         'VAIMP': 'http://www.isocat.org/datcat/DC-1263',  # copula; Auxiliar, Imperativ
```

### Comparing `TCFlib-0.2.6/tcflib/tagsets/base.py` & `TCFlib-0.3.0/tcflib/tagsets/base.py`

 * *Files identical despite different names*

### Comparing `TCFlib-0.2.6/tcflib/tagsets/dc1345.py` & `TCFlib-0.3.0/tcflib/tagsets/dc1345.py`

 * *Files identical despite different names*

### Comparing `TCFlib-0.2.6/tcflib/tagsets/stts.py` & `TCFlib-0.3.0/tcflib/tagsets/stts.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,15 @@
         'ITJ': 'http://www.isocat.org/datcat/DC-1318',  # interjection
         'KOKOM': 'http://www.isocat.org/datcat/DC-1922',  # comparativeParticle
         'KON': 'http://www.isocat.org/datcat/DC-1262',  # coordinatingConjunction
         'KOUI': 'http://www.isocat.org/datcat/DC-1393',  # subordinatingConjunction
         'KOUS': 'http://www.isocat.org/datcat/DC-1393',  # subordinatingConjunction
         'NE': 'http://www.isocat.org/datcat/DC-1371',  # properNoun
         'NN': 'http://www.isocat.org/datcat/DC-1333',  # noun
+        'PAV': 'http://www.isocat.org/datcat/DC-2998',  # pronominalAdverb
         'PDAT': 'http://www.isocat.org/datcat/DC-1270',  # demonstrativePronoun
         'PDS': 'http://www.isocat.org/datcat/DC-1270',  # demonstrativePronoun
         'PIAT': 'http://www.isocat.org/datcat/DC-1309',  # indefinitePronoun
         'PIDAT': 'http://www.isocat.org/datcat/DC-1309',  # indefinitePronoun
         'PIS': 'http://www.isocat.org/datcat/DC-1309',  # indefinitePronoun
         'PPER': 'http://www.isocat.org/datcat/DC-3013',  # irreflexivePersonalPronoun
         'PPOSAT': 'http://www.isocat.org/datcat/DC-1359',  # possessivePronoun
```

### Comparing `TCFlib-0.2.6/tcflib/tagsets/stein.py` & `TCFlib-0.3.0/tcflib/tagsets/stein.py`

 * *Files identical despite different names*

### Comparing `TCFlib-0.2.6/tcflib/tagsets/penntb.py` & `TCFlib-0.3.0/tcflib/tagsets/penntb.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,19 +43,23 @@
         'JJR': 'http://www.isocat.org/datcat/DC-1230',  # adjective
         'JJS': 'http://www.isocat.org/datcat/DC-1230',  # adjective
         'LS': 'http://www.isocat.org/datcat/DC-1438',  # bullet
         'MD': 'http://www.isocat.org/datcat/DC-1329',  # modal
         'NN': 'http://www.isocat.org/datcat/DC-1256',  # commonNoun
         'NNS': 'http://www.isocat.org/datcat/DC-1256',  # commonNoun
         'NP': 'http://www.isocat.org/datcat/DC-1371',  # properNoun
+        'NNP': 'http://www.isocat.org/datcat/DC-1371',  # properNoun
         'NPS': 'http://www.isocat.org/datcat/DC-1371',  # properNoun
+        'NNPS': 'http://www.isocat.org/datcat/DC-1371',  # properNoun
         'PDT': 'http://www.isocat.org/datcat/DC-1272',  # determiner FIXME
         'POS': 'http://www.isocat.org/datcat/DC-1895',  # possessiveParticle
         'PP': 'http://www.isocat.org/datcat/DC-1463',  # personalPronoun
+        'PRP': 'http://www.isocat.org/datcat/DC-1463',  # personalPronoun
         'PP$': 'http://www.isocat.org/datcat/DC-1359',  # possessivePronoun
+        'PRP$': 'http://www.isocat.org/datcat/DC-1359',  # possessivePronoun
         'RB': 'http://www.isocat.org/datcat/DC-1232',  # adverb
         'RBR': 'http://www.isocat.org/datcat/DC-1232',  # adverb
         'RBS': 'http://www.isocat.org/datcat/DC-1232',  # adverb
         'RP': 'http://www.isocat.org/datcat/DC-1917',  # particleAdverb
         'SENT': 'http://www.isocat.org/datcat/DC-2075',  # mainPunctuation
         'SYM': 'http://www.isocat.org/datcat/DC-1891',  # unclassifiedResidual FIXME
         'TO': 'http://www.isocat.org/datcat/DC-1896',  # infinitiveParticle
@@ -80,14 +84,15 @@
         'VVZ': 'http://www.isocat.org/datcat/DC-1400',  # mainVerb
         'WDT': 'http://www.isocat.org/datcat/DC-1272',  # determiner
         'WP': 'http://www.isocat.org/datcat/DC-1463',  # personalPronoun
         'WP$': 'http://www.isocat.org/datcat/DC-1359',  # possessivePronoun
         'WRB': 'http://www.isocat.org/datcat/DC-1232',  # adverb
         '#': 'http://www.isocat.org/datcat/DC-1891',  # unclassifiedResidual FIXME
         '$': 'http://www.isocat.org/datcat/DC-1891',  # unclassifiedResidual FIXME
+        '.': 'http://www.isocat.org/datcat/DC-2075',  # mainPunctuation
         '"': 'http://www.isocat.org/datcat/DC-2076',  # secondaryPunctuation  FIXME
         '``': 'http://www.isocat.org/datcat/DC-2076',  # secondaryPunctuation  FIXME
         "''": 'http://www.isocat.org/datcat/DC-2076',  # secondaryPunctuation  FIXME
         #'(': 'http://www.isocat.org/datcat/DC-2078',  # openPunctuation  FIXME: Not in dcif data
         #')': 'http://www.isocat.org/datcat/DC-2079',  # closePunctuation  FIXME: Not in dcif data
         '(': 'http://www.isocat.org/datcat/DC-2076',  # secondaryPunctuation  FIXME
         ')': 'http://www.isocat.org/datcat/DC-2076',  # secondaryPunctuation  FIXME
```

### Comparing `TCFlib-0.2.6/tcflib/tcf.py` & `TCFlib-0.3.0/tcflib/tcf.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 
 NS_DATA = 'http://www.dspin.de/data'
 P_DATA = '{' + NS_DATA + '}'
 NS_TEXT = 'http://www.dspin.de/data/textcorpus'
 P_TEXT = '{' + NS_TEXT + '}'
 NS = {'data': NS_DATA, 'text': NS_TEXT}
 
+UNKNOWN_LEMMAS = ['<unknown>']
 
 class AnnotationLayerBase:
     """Base class for annotation layers."""
 
     element = ''
 
     def __init__(self, initialdata=None):
@@ -463,19 +464,25 @@
         """
         The semantic unit for a token.
 
         The semantic unit can be the (disambiguated) lemma, a named entity,
         or a referenced semantic unit.
 
         """
+        def lemma_if_available(token):
+            if token.lemma and not token.lemma in UNKNOWN_LEMMAS:
+                return token.lemma
+            return token.text
+
         def disambiguate(token):
             if token.wordsenses:
-                return '{} ({})'.format(token.lemma or token.text,
+                return '{} ({})'.format(lemma_if_available(token),
                                         ', '.join(token.wordsenses))
-            return token.lemma or token.text
+            return lemma_if_available(token)
+
         tokens = None
         if self.reference:
             if self.reference.entity.extref:
                 return self.reference.entity.extref
             if self.reference.target:
                 tokens = self.reference.target.tokens
         elif self.entity:
@@ -894,14 +901,29 @@
         except NameError:
             logging.warn('The igraph package has to be installed to use the '
                          'graph annotation layer.')
             raise
         self._graph.vs['name'] = ''  # Ensure 'name' attribute is present.
         self.label = label
         self.weight = weight
+        # Calculate cooccurrence measures
+        # The actual calculation happens in `self.tcf()`, since only then
+        # the graph is complete.
+        self.supported_measures = ('llr', 'pmi')
+        if self.weight in self.supported_measures:
+            try:
+                import nltk
+                bigram_measures = nltk.collocations.BigramAssocMeasures()
+            except ImportError:
+                logging.error('NLTK needs to be installed '
+                              'for cooccurrence measures.')
+            if self.weight == 'llr':
+                self.measure = bigram_measures.likelihood_ratio
+            elif self.weight == 'pmi':
+                self.measure = bigram_measures.pmi
 
         class Edge:
             def __init__(self, edge, graph):
                 self._edge = edge
                 self._graph = graph
 
             def __getitem__(self, key):
@@ -989,28 +1011,36 @@
                 edge['weight'] += 1
                 edge['tokens'][edge_tokens] = 1
         return edge
 
     @property
     def tcf(self):
         graph = etree.Element(P_TEXT + 'graph', nsmap={None: NS_TEXT})
+        graph.attrib['weight'] = self.weight
         nodes = etree.SubElement(graph, P_TEXT + 'nodes')
         edges = etree.SubElement(graph, P_TEXT + 'edges')
         nid = 'n_{}'
         # The graph should not have multiple edges.
         if self._graph.has_multiple():
             logging.warn('Multiple edges detected. This cannot be handled '
                          'by some graph analysis applications.')
         # simplify the graph, i.e., merge
         #self._graph.simplify(combine_edges={'weight': sum,
         #                     'tokens': lambda x: list(chain.from_iterable(x))})
+        if self.weight in self.supported_measures:
+            # Since we re-calculate the weight, we copy over the counts
+            # to a new attribute.
+            self._graph.es['count'] = self._graph.es['weight']
+            n_xx = self._graph.vcount()
         for vertex in self._graph.vs:
             node = etree.SubElement(nodes, P_TEXT + 'node')
             node.text = vertex['name']
             node.set('ID', nid.format(vertex.index))
+            # Add token count
+            vertex['count'] = len(vertex['tokens'])
             for key, value in vertex.attributes().items():
                 if key == 'name':
                     continue
                 elif key == 'tokens':
                     node.set('tokenIDs',
                              ' '.join([token.id for token in value]))
                 elif isinstance(value, (list, tuple)):
@@ -1019,14 +1049,33 @@
                     node.set(key, str(value).lower())
                 else:
                     node.set(key, str(value))
         for link in self._graph.es:
             edge = etree.SubElement(edges, P_TEXT + 'edge',
                                     source=nid.format(link.source),
                                     target=nid.format(link.target))
+            if self.weight in self.supported_measures:
+                # Re-calculate weight
+                n_ii = link['count']
+                n_ix = self._graph.vs[link.source]['count']
+                n_xi = self._graph.vs[link.target]['count']
+                try:
+                    stat = self.measure(
+                        n_ii, (n_ix, n_xi), n_xx)
+                except ValueError:
+                    # Cooccurrence count might be higher than individual counts
+                    # when two occurrences of the same word appear close.
+                    # TODO: Check what the literature suggests here.
+                    logging.debug(f'Skewed values for edge {link.source}, '
+                                 f'{link.target}: '
+                                 f'{n_ii}, ({n_ix}, {n_xi}), {n_xx}')
+                    # We fix this by using the minimum.
+                    stat = self.measure(
+                        min(n_ii, n_ix, n_xi), (n_ix, n_xi), n_xx)
+                link['weight'] = stat
             for key, value in link.attributes().items():
                 if key == 'tokens':
                     for (a, b), weight in value.items():
                         etree.SubElement(edge, P_TEXT + 'tokenEdge',
                                          source=str(a.id), target=str(b.id),
                                          weight=str(weight))
                 elif isinstance(value, (list, tuple)):
```

### Comparing `TCFlib-0.2.6/tcflib/service.py` & `TCFlib-0.3.0/tcflib/service.py`

 * *Files identical despite different names*

