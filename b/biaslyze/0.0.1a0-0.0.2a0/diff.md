# Comparing `tmp/biaslyze-0.0.1a0.tar.gz` & `tmp/biaslyze-0.0.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biaslyze-0.0.1a0.tar", max compression
+gzip compressed data, was "biaslyze-0.0.2a0.tar", max compression
```

## Comparing `biaslyze-0.0.1a0.tar` & `biaslyze-0.0.2a0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1495 2023-04-21 09:03:51.243806 biaslyze-0.0.1a0/LICENSE
--rw-r--r--   0        0        0     1760 2023-05-25 09:47:41.505257 biaslyze-0.0.1a0/README.md
--rw-r--r--   0        0        0        0 2023-03-09 11:50:10.881651 biaslyze-0.0.1a0/biaslyze/__init__.py
--rw-r--r--   0        0        0     6931 2023-05-25 09:48:01.453043 biaslyze-0.0.1a0/biaslyze/_plotting.py
--rw-r--r--   0        0        0      220 2023-05-19 13:34:56.156524 biaslyze-0.0.1a0/biaslyze/bias_detectors/__init__.py
--rw-r--r--   0        0        0    12739 2023-05-25 10:16:50.171622 biaslyze-0.0.1a0/biaslyze/bias_detectors/counterfactual_biasdetector.py
--rw-r--r--   0        0        0     5547 2023-05-25 09:48:01.425044 biaslyze-0.0.1a0/biaslyze/bias_detectors/lime_biasdetector.py
--rw-r--r--   0        0        0     1831 2023-05-19 13:34:56.156524 biaslyze-0.0.1a0/biaslyze/concept_detectors.py
--rw-r--r--   0        0        0    64680 2023-05-19 13:34:56.156524 biaslyze-0.0.1a0/biaslyze/concepts.py
--rw-r--r--   0        0        0    13052 2023-05-25 10:16:50.203622 biaslyze-0.0.1a0/biaslyze/results/counterfactual_detection_results.py
--rw-r--r--   0        0        0     4990 2023-05-25 08:34:39.793839 biaslyze-0.0.1a0/biaslyze/results/lime_detection_results.py
--rw-r--r--   0        0        0      968 2023-05-25 12:04:51.564612 biaslyze-0.0.1a0/pyproject.toml
--rw-r--r--   0        0        0     2807 1970-01-01 00:00:00.000000 biaslyze-0.0.1a0/setup.py
--rw-r--r--   0        0        0     2668 1970-01-01 00:00:00.000000 biaslyze-0.0.1a0/PKG-INFO
+-rw-r--r--   0        0        0     1495 2023-04-21 09:03:51.243806 biaslyze-0.0.2a0/LICENSE
+-rw-r--r--   0        0        0     1760 2023-05-25 09:47:41.505257 biaslyze-0.0.2a0/README.md
+-rw-r--r--   0        0        0        0 2023-03-09 11:50:10.881651 biaslyze-0.0.2a0/biaslyze/__init__.py
+-rw-r--r--   0        0        0     6931 2023-05-25 09:48:01.453043 biaslyze-0.0.2a0/biaslyze/_plotting.py
+-rw-r--r--   0        0        0      220 2023-05-19 13:34:56.156524 biaslyze-0.0.2a0/biaslyze/bias_detectors/__init__.py
+-rw-r--r--   0        0        0    12739 2023-05-25 10:16:50.171622 biaslyze-0.0.2a0/biaslyze/bias_detectors/counterfactual_biasdetector.py
+-rw-r--r--   0        0        0     5547 2023-05-25 09:48:01.425044 biaslyze-0.0.2a0/biaslyze/bias_detectors/lime_biasdetector.py
+-rw-r--r--   0        0        0     1831 2023-05-19 13:34:56.156524 biaslyze-0.0.2a0/biaslyze/concept_detectors.py
+-rw-r--r--   0        0        0    64680 2023-05-19 13:34:56.156524 biaslyze-0.0.2a0/biaslyze/concepts.py
+-rw-r--r--   0        0        0    13052 2023-05-25 10:16:50.203622 biaslyze-0.0.2a0/biaslyze/results/counterfactual_detection_results.py
+-rw-r--r--   0        0        0     4990 2023-05-25 08:34:39.793839 biaslyze-0.0.2a0/biaslyze/results/lime_detection_results.py
+-rw-r--r--   0        0        0      984 2023-05-25 12:19:20.284108 biaslyze-0.0.2a0/pyproject.toml
+-rw-r--r--   0        0        0     2807 1970-01-01 00:00:00.000000 biaslyze-0.0.2a0/setup.py
+-rw-r--r--   0        0        0     2675 1970-01-01 00:00:00.000000 biaslyze-0.0.2a0/PKG-INFO
```

### Comparing `biaslyze-0.0.1a0/LICENSE` & `biaslyze-0.0.2a0/LICENSE`

 * *Files identical despite different names*

### Comparing `biaslyze-0.0.1a0/README.md` & `biaslyze-0.0.2a0/README.md`

 * *Files identical despite different names*

### Comparing `biaslyze-0.0.1a0/biaslyze/_plotting.py` & `biaslyze-0.0.2a0/biaslyze/_plotting.py`

 * *Files identical despite different names*

### Comparing `biaslyze-0.0.1a0/biaslyze/bias_detectors/counterfactual_biasdetector.py` & `biaslyze-0.0.2a0/biaslyze/bias_detectors/counterfactual_biasdetector.py`

 * *Files identical despite different names*

### Comparing `biaslyze-0.0.1a0/biaslyze/bias_detectors/lime_biasdetector.py` & `biaslyze-0.0.2a0/biaslyze/bias_detectors/lime_biasdetector.py`

 * *Files identical despite different names*

### Comparing `biaslyze-0.0.1a0/biaslyze/concept_detectors.py` & `biaslyze-0.0.2a0/biaslyze/concept_detectors.py`

 * *Files identical despite different names*

### Comparing `biaslyze-0.0.1a0/biaslyze/concepts.py` & `biaslyze-0.0.2a0/biaslyze/concepts.py`

 * *Files identical despite different names*

### Comparing `biaslyze-0.0.1a0/biaslyze/results/counterfactual_detection_results.py` & `biaslyze-0.0.2a0/biaslyze/results/counterfactual_detection_results.py`

 * *Files identical despite different names*

### Comparing `biaslyze-0.0.1a0/biaslyze/results/lime_detection_results.py` & `biaslyze-0.0.2a0/biaslyze/results/lime_detection_results.py`

 * *Files identical despite different names*

### Comparing `biaslyze-0.0.1a0/setup.py` & `biaslyze-0.0.2a0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  'scipy==1.8.0',
  'spacy>=3.5.0,<4.0.0',
  'transformers>=4.26.1,<5.0.0',
  'umap-learn>=0.5.3,<0.6.0']
 
 setup_kwargs = {
     'name': 'biaslyze',
-    'version': '0.0.1a0',
+    'version': '0.0.2a0',
     'description': 'The NLP Bias Identification Toolkit',
     'long_description': '# biaslyze\nThe NLP Bias Identification Toolkit\n\n\n## Usage example\n\n```python\nfrom biaslyze.bias_detectors import CounterfactualBiasDetector\n\nbias_detector = CounterfactualBiasDetector()\n\n# detect bias in the model based on the given texts\n# here, clf is a scikit-learn text classification pipeline trained for a binary classification task\ndetection_res = bias_detector.process(\n    texts=texts,\n    predict_func=clf.predict_proba\n)\n\n# see a summary of the detection\ndetection_res.report()\n\n# visualize the counterfactual scores\ndetection_res.visualize_counterfactual_scores(concept="religion", top_n=10)\n```\n\nExample output:\n![](resources/hatespeech_dl_scores_religion.png)\n\n\n## Development setup\n\n- First you need to install poetry to manage your python environment: https://python-poetry.org/docs/#installation\n- Run `make install` to install the dependencies and get the spacy basemodels.\n- Now you can use `biaslyze` in your jupyter notebooks.\n\n\n### Adding concepts and keywords\n\nYou can add concepts and new keywords for existing concepts by editing [concepts.py](https://github.com/biaslyze-dev/biaslyze/blob/keyword-based-targeted-lime/biaslyze/concepts.py).\n\n## Preview/build the documentation with mkdocs\n\nTo preview the documentation run `make doc-preview`. This will launch a preview of the documentation on `http://127.0.0.1:8000/`.\nTo build the documentation html run `make doc`.\n\n\n## Run the automated tests\n\n`make test`\n\n\n## Style guide\n\nWe are using isort and black: `make style`\nFor linting we are running ruff: `make lint`\n\n## Contributing\n\nFollow the google style guide for python: https://google.github.io/styleguide/pyguide.html\n\nThis project uses black, isort and ruff to enforce style. Apply it by running `make style` and `make lint`.\n\n',
     'author': 'Tobias Sterbak',
     'author_email': 'hello@tobiassterbak.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `biaslyze-0.0.1a0/PKG-INFO` & `biaslyze-0.0.2a0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: biaslyze
-Version: 0.0.1a0
+Version: 0.0.2a0
 Summary: The NLP Bias Identification Toolkit
-License: LICENSE
+License: BSD-3-Clause
 Author: Tobias Sterbak
 Author-email: hello@tobiassterbak.com
 Requires-Python: >=3.10,<3.11
-Classifier: License :: Other/Proprietary License
+Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: bertopic (==0.13.0)
 Requires-Dist: bokeh (>=3.1.0,<4.0.0)
 Requires-Dist: eli5 (>=0.13.0,<0.14.0)
 Requires-Dist: jupyterlab (>=3.5.2,<4.0.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
```

