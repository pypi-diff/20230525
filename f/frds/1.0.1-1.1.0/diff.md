# Comparing `tmp/frds-1.0.1.tar.gz` & `tmp/frds-1.1.0.tar.gz`

## Comparing `frds-1.0.1.tar` & `frds-1.1.0.tar`

### file list

```diff
@@ -1,41 +1,49 @@
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 frds-1.0.1/.pylintrc
--rw-r--r--   0        0        0     3440 2020-02-02 00:00:00.000000 frds-1.0.1/mkdocs.yml
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 frds-1.0.1/.github/FUNDING.yml
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 frds-1.0.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 frds-1.0.1/.github/workflows/build-and-deploy-docs.yml
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 frds-1.0.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 frds-1.0.1/.github/workflows/test.yml
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 frds-1.0.1/docs/CNAME
--rw-r--r--   0        0        0     3952 2020-02-02 00:00:00.000000 frds-1.0.1/docs/index.md
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 frds-1.0.1/docs/measures.md
--rw-r--r--   0        0        0   143526 2020-02-02 00:00:00.000000 frds-1.0.1/docs/images/frds_icon.png
--rw-r--r--   0        0        0    58143 2020-02-02 00:00:00.000000 frds-1.0.1/docs/images/frds_icon_white.png
--rw-r--r--   0        0        0   132433 2020-02-02 00:00:00.000000 frds-1.0.1/docs/images/frds_logo.png
--rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 frds-1.0.1/docs/measures/absorption_ratio.md
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 frds-1.0.1/docs/measures/contingent_claim_analysis.md
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 frds-1.0.1/docs/measures/distress_insurance_premium.md
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 frds-1.0.1/docs/measures/marginal_expected_shortfall.md
--rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 frds-1.0.1/docs/measures/systemic_expected_shortfall.md
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 frds-1.0.1/docs/measures/z_score.md
--rw-r--r--   0        0        0   143526 2020-02-02 00:00:00.000000 frds-1.0.1/images/frds_icon.png
--rw-r--r--   0        0        0   132433 2020-02-02 00:00:00.000000 frds-1.0.1/images/frds_logo.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 frds-1.0.1/src/frds/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 frds-1.0.1/src/frds/measures/__init__.py
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 frds-1.0.1/src/frds/measures/absorption_ratio.py
--rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 frds-1.0.1/src/frds/measures/contingent_claims_analysis.py
--rw-r--r--   0        0        0     4538 2020-02-02 00:00:00.000000 frds-1.0.1/src/frds/measures/distress_insurance_premium.py
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 frds-1.0.1/src/frds/measures/marginal_expected_shortfall.py
--rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 frds-1.0.1/src/frds/measures/systemic_expected_shortfall.py
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 frds-1.0.1/src/frds/measures/z_score.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 frds-1.0.1/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 frds-1.0.1/tests/measures/__init__.py
--rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 frds-1.0.1/tests/measures/test_absorption_ratio.py
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 frds-1.0.1/tests/measures/test_distress_insurance_premium.py
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 frds-1.0.1/tests/measures/test_marginal_expected_shortfall.py
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 frds-1.0.1/tests/measures/test_systemic_expected_shortfall.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 frds-1.0.1/tests/measures/test_z_score.py
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 frds-1.0.1/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 frds-1.0.1/LICENSE
--rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 frds-1.0.1/README.md
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 frds-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     3843 2020-02-02 00:00:00.000000 frds-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 frds-1.1.0/.pylintrc
+-rw-r--r--   0        0        0     3713 2020-02-02 00:00:00.000000 frds-1.1.0/mkdocs.yml
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 frds-1.1.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 frds-1.1.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 frds-1.1.0/.github/workflows/build-and-deploy-docs.yml
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 frds-1.1.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 frds-1.1.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 frds-1.1.0/docs/CNAME
+-rw-r--r--   0        0        0     3952 2020-02-02 00:00:00.000000 frds-1.1.0/docs/index.md
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 frds-1.1.0/docs/measures.md
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 frds-1.1.0/docs/algorithms/dcc_garch.md
+-rw-r--r--   0        0        0   143526 2020-02-02 00:00:00.000000 frds-1.1.0/docs/images/frds_icon.png
+-rw-r--r--   0        0        0    58143 2020-02-02 00:00:00.000000 frds-1.1.0/docs/images/frds_icon_white.png
+-rw-r--r--   0        0        0   132433 2020-02-02 00:00:00.000000 frds-1.1.0/docs/images/frds_logo.png
+-rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 frds-1.1.0/docs/measures/absorption_ratio.md
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 frds-1.1.0/docs/measures/contingent_claim_analysis.md
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 frds-1.1.0/docs/measures/distress_insurance_premium.md
+-rw-r--r--   0        0        0     9195 2020-02-02 00:00:00.000000 frds-1.1.0/docs/measures/long_run_mes.md
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 frds-1.1.0/docs/measures/marginal_expected_shortfall.md
+-rw-r--r--   0        0        0     3824 2020-02-02 00:00:00.000000 frds-1.1.0/docs/measures/srisk.md
+-rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 frds-1.1.0/docs/measures/systemic_expected_shortfall.md
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 frds-1.1.0/docs/measures/z_score.md
+-rw-r--r--   0        0        0   143526 2020-02-02 00:00:00.000000 frds-1.1.0/images/frds_icon.png
+-rw-r--r--   0        0        0   132433 2020-02-02 00:00:00.000000 frds-1.1.0/images/frds_logo.png
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 frds-1.1.0/includes/abbreviations.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 frds-1.1.0/src/frds/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 frds-1.1.0/src/frds/algorithms/__init__.py
+-rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 frds-1.1.0/src/frds/algorithms/dcc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 frds-1.1.0/src/frds/measures/__init__.py
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 frds-1.1.0/src/frds/measures/absorption_ratio.py
+-rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 frds-1.1.0/src/frds/measures/contingent_claim_analysis.py
+-rw-r--r--   0        0        0     4538 2020-02-02 00:00:00.000000 frds-1.1.0/src/frds/measures/distress_insurance_premium.py
+-rw-r--r--   0        0        0     7137 2020-02-02 00:00:00.000000 frds-1.1.0/src/frds/measures/long_run_mes.py
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 frds-1.1.0/src/frds/measures/marginal_expected_shortfall.py
+-rw-r--r--   0        0        0     4537 2020-02-02 00:00:00.000000 frds-1.1.0/src/frds/measures/srisk.py
+-rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 frds-1.1.0/src/frds/measures/systemic_expected_shortfall.py
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 frds-1.1.0/src/frds/measures/z_score.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 frds-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 frds-1.1.0/tests/measures/__init__.py
+-rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 frds-1.1.0/tests/measures/test_absorption_ratio.py
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 frds-1.1.0/tests/measures/test_distress_insurance_premium.py
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 frds-1.1.0/tests/measures/test_marginal_expected_shortfall.py
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 frds-1.1.0/tests/measures/test_systemic_expected_shortfall.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 frds-1.1.0/tests/measures/test_z_score.py
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 frds-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 frds-1.1.0/LICENSE
+-rw-r--r--   0        0        0     3670 2020-02-02 00:00:00.000000 frds-1.1.0/README.md
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 frds-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4575 2020-02-02 00:00:00.000000 frds-1.1.0/PKG-INFO
```

### Comparing `frds-1.0.1/mkdocs.yml` & `frds-1.1.0/mkdocs.yml`

 * *Files 4% similar despite different names*

```diff
@@ -15,18 +15,21 @@
 theme:
   name: material
   features:
     - navigation.tabs
     - navigation.top
     - navigation.tracking
     - navigation.indexes
-    # - navigation.sections
+    - navigation.footer
+    - navigation.sections
+    - navigation.expand
     - content.code.annotate
     - content.code.copy
     - content.code.select
+    - content.tooltips
   language: en
   palette:
     # Palette toggle for automatic mode
     - media: "(prefers-color-scheme)"
       primary: white
       accent: blue
       toggle:
@@ -65,14 +68,15 @@
   - mkdocstrings:
       handlers:
         python:
           paths: [src]
 
 # Extensions
 markdown_extensions:
+  - abbr
   - pymdownx.tabbed:
       alternate_style: true
   - attr_list
   - md_in_html
   - meta
   - admonition
   - footnotes
@@ -99,14 +103,18 @@
   - pymdownx.mark
   - pymdownx.smartsymbols
   - pymdownx.superfences
   - pymdownx.tasklist:
       custom_checkbox: true
   - pymdownx.tabbed
   - pymdownx.tilde
+  - pymdownx.snippets:
+      auto_append:
+        - includes/abbreviations.md
+
 
 extra_javascript:
   - https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.0/MathJax.js?config=TeX-MML-AM_CHTML
 
 extra:
   generator: false
   social:
@@ -116,19 +124,22 @@
       link: https://pypi.org/project/frds/
     - icon: fontawesome/solid/paper-plane
       link: mailto:mingze.gao@sydney.edu.au
 
 nav:
   - Home:
     - frds: index.md
-    - Author: https://mingze-gao.com
-  - Measures:
+    - Measures:
       - measures.md
       - Banking:
-          - Absoprtion ratio: measures/absorption_ratio.md
-          - Contingent claim analysis: measures/contingent_claim_analysis.md
-          - Distress insurance premium: measures/distress_insurance_premium.md
-          - Marginal expected shortfall: measures/marginal_expected_shortfall.md
-          - Systemic expected shortfall: measures/systemic_expected_shortfall.md
+          - Absoprtion Ratio: measures/absorption_ratio.md
+          - Contingent Claim Analysis: measures/contingent_claim_analysis.md
+          - Distress Insurance Premium: measures/distress_insurance_premium.md
+          - Long-Run MES (LRMES): measures/long_run_mes.md
+          - Marginal Expected Shortfall: measures/marginal_expected_shortfall.md
+          - SRISK: measures/srisk.md
+          - Systemic Expected Shortfall: measures/systemic_expected_shortfall.md
           - Z-score: measures/z_score.md
+    - Algorithms:
+      - DCC: algorithms/dcc_garch.md
   - Author Site: https://mingze-gao.com
```

### Comparing `frds-1.0.1/.github/ISSUE_TEMPLATE/bug_report.md` & `frds-1.1.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `frds-1.0.1/.github/workflows/build-and-deploy-docs.yml` & `frds-1.1.0/.github/workflows/build-and-deploy-docs.yml`

 * *Files 11% similar despite different names*

```diff
@@ -9,20 +9,23 @@
   contents: write
 jobs:
   deploy:
     runs-on: ubuntu-latest
     if: github.event.repository.fork == false
     steps:
       - uses: actions/checkout@v3
+        with:
+          fetch-depth: 0
       - uses: actions/setup-python@v4
         with:
           python-version: 3.x
+      - run: echo "cache_id=$(date --utc '+%V')" >> $GITHUB_ENV
       - uses: actions/cache@v3
         with:
-          key: mkdocs-material-${{ github.ref }}
+          key: mkdocs-material-${{ env.cache_id }}
           path: .cache
           restore-keys: |
             mkdocs-material-
       - run: |
           python -m pip install --upgrade pip
           pip install git+https://${GH_TOKEN}@github.com/squidfunk/mkdocs-material-insiders.git
           pip install mkdocs-git-revision-date-localized-plugin mkdocstrings mkdocstrings-python mkdocs-minify-plugin
```

### Comparing `frds-1.0.1/.github/workflows/publish.yml` & `frds-1.1.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `frds-1.0.1/.github/workflows/test.yml` & `frds-1.1.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `frds-1.0.1/docs/index.md` & `frds-1.1.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `frds-1.0.1/docs/images/frds_icon.png` & `frds-1.1.0/docs/images/frds_icon.png`

 * *Files identical despite different names*

### Comparing `frds-1.0.1/docs/images/frds_icon_white.png` & `frds-1.1.0/docs/images/frds_icon_white.png`

 * *Files identical despite different names*

### Comparing `frds-1.0.1/docs/images/frds_logo.png` & `frds-1.1.0/docs/images/frds_logo.png`

 * *Files identical despite different names*

### Comparing `frds-1.0.1/docs/measures/absorption_ratio.md` & `frds-1.1.0/docs/measures/absorption_ratio.md`

 * *Files identical despite different names*

### Comparing `frds-1.0.1/docs/measures/contingent_claim_analysis.md` & `frds-1.1.0/docs/measures/contingent_claim_analysis.md`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 ## Introduction
 
 The difference between put price and CDS price as a measure of firm's contribution to systemic risk based on [Gray and Jobst (2010)](https://ideas.repec.org/p/imf/imfwpa/2013-054.html).
 
 ## API
 
-### ::: frds.measures.contingent_claims_analysis
+### ::: frds.measures.contingent_claim_analysis
 
 ## References
 
 * [Gray and Jobst (2010)](https://ideas.repec.org/p/imf/imfwpa/2013-054.html),
     Systemic contingent claims analysis: Estimating market-implied systemic risk, *IMF Working Papers*, No 13/54.
 * [Bisias, Flood, Lo, and Valavanis (2012)](https://doi.org/10.1146/annurev-financial-110311-101754),
     A survey of systemic risk analytics, *Annual Review of Financial Economics*, 4, 255-296.
```

### Comparing `frds-1.0.1/docs/measures/distress_insurance_premium.md` & `frds-1.1.0/docs/measures/distress_insurance_premium.md`

 * *Files identical despite different names*

### Comparing `frds-1.0.1/docs/measures/marginal_expected_shortfall.md` & `frds-1.1.0/docs/measures/marginal_expected_shortfall.md`

 * *Files identical despite different names*

### Comparing `frds-1.0.1/docs/measures/systemic_expected_shortfall.md` & `frds-1.1.0/docs/measures/systemic_expected_shortfall.md`

 * *Files identical despite different names*

### Comparing `frds-1.0.1/docs/measures/z_score.md` & `frds-1.1.0/docs/measures/z_score.md`

 * *Files identical despite different names*

### Comparing `frds-1.0.1/images/frds_icon.png` & `frds-1.1.0/images/frds_icon.png`

 * *Files identical despite different names*

### Comparing `frds-1.0.1/images/frds_logo.png` & `frds-1.1.0/images/frds_logo.png`

 * *Files identical despite different names*

### Comparing `frds-1.0.1/src/frds/measures/absorption_ratio.py` & `frds-1.1.0/src/frds/measures/absorption_ratio.py`

 * *Files identical despite different names*

### Comparing `frds-1.0.1/src/frds/measures/contingent_claims_analysis.py` & `frds-1.1.0/src/frds/measures/contingent_claim_analysis.py`

 * *Files identical despite different names*

### Comparing `frds-1.0.1/src/frds/measures/distress_insurance_premium.py` & `frds-1.1.0/src/frds/measures/distress_insurance_premium.py`

 * *Files identical despite different names*

### Comparing `frds-1.0.1/src/frds/measures/marginal_expected_shortfall.py` & `frds-1.1.0/src/frds/measures/marginal_expected_shortfall.py`

 * *Files identical despite different names*

### Comparing `frds-1.0.1/src/frds/measures/systemic_expected_shortfall.py` & `frds-1.1.0/src/frds/measures/systemic_expected_shortfall.py`

 * *Files identical despite different names*

### Comparing `frds-1.0.1/src/frds/measures/z_score.py` & `frds-1.1.0/src/frds/measures/z_score.py`

 * *Files identical despite different names*

### Comparing `frds-1.0.1/tests/measures/test_absorption_ratio.py` & `frds-1.1.0/tests/measures/test_absorption_ratio.py`

 * *Files identical despite different names*

### Comparing `frds-1.0.1/tests/measures/test_distress_insurance_premium.py` & `frds-1.1.0/tests/measures/test_distress_insurance_premium.py`

 * *Files identical despite different names*

### Comparing `frds-1.0.1/tests/measures/test_marginal_expected_shortfall.py` & `frds-1.1.0/tests/measures/test_marginal_expected_shortfall.py`

 * *Files identical despite different names*

### Comparing `frds-1.0.1/tests/measures/test_systemic_expected_shortfall.py` & `frds-1.1.0/tests/measures/test_systemic_expected_shortfall.py`

 * *Files identical despite different names*

### Comparing `frds-1.0.1/.gitignore` & `frds-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `frds-1.0.1/LICENSE` & `frds-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `frds-1.0.1/README.md` & `frds-1.1.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,32 @@
+Metadata-Version: 2.1
+Name: frds
+Version: 1.1.0
+Summary: Financial Research Data Services
+Project-URL: homepage, https://github.com/mgao6767/frds
+Project-URL: documentation, https://frds.io
+Author-email: Mingze Gao <adrian.gao@outlook.com>
+License: MIT License
+License-File: LICENSE
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Intended Audience :: Financial and Insurance Industry
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Requires-Python: >=3.8
+Requires-Dist: arch
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: scipy
+Description-Content-Type: text/markdown
+
 ![frds](https://github.com/mgao6767/frds/raw/main/images/frds_logo.png)
 
 # FRDS - Financial Research Data Services
 
 ![LICENSE](https://img.shields.io/github/license/mgao6767/frds?color=blue) ![DOWNLOADS](https://img.shields.io/pypi/dm/frds?label=PyPI%20downloads) [![Test](https://github.com/mgao6767/frds/actions/workflows/test.yml/badge.svg)](https://github.com/mgao6767/frds/actions/workflows/test.yml) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 [frds](https://github.com/mgao6767/frds/) is an open-sourced Python package for computing [a collection of major academic measures](https://frds.io/measures/) used in the finance literature in a simple and straightforward way.
@@ -12,15 +37,31 @@
 pip install frds
 ```
 
 ## Note
 
 This library is still under development and breaking changes may be expected.
 
-## Built-in measures
+If there's any issue (likely), please contact me at [mingze.gao@sydney.edu.au](mailto:mingze.gao@sydney.edu.au)
+
+## Supported measures
+
+More to be added. For a complete list of supported built-in measures, please check [frds.io/measures/](https://frds.io/measures/).
+
+* [Absorption Ratio](https://frds.io/measures/absorption_ratio/)
+* [Contingent Claim Analysis](https://frds.io/measures/contingent_claim_analysis/)
+* [Distress Insurance Premium](https://frds.io/measures/distress_insurance_premium/)
+* [Long-Run MES](https://frds.io/measures/long_run_mes/)
+* [Marginal Expected Shortfall (MES)](https://frds.io/measures/marginal_expected_shortfall/)
+* [SRISK](https://frds.io/measures/srisk/)
+* [Systemic Expected Shortfall (SES)](https://frds.io/measures/systemic_expected_shortfall/)
+* [Z-score](https://frds.io/measures/z_score)
+
+
+## Examples
 
 The primary purpose of `frds` is to offer ready-to-use functions.
 
 For example, Kritzman, Li, Page, and Rigobon (2010) propose an [Absorption Ratio](https://frds.io/measures/absorption_ratio/) that measures the fraction of the total variance of a set of asset returns explained or absorbed by a fixed number of eigenvectors. It captures the extent to which markets are unified or tightly coupled.
 
 ``` python
 >>> import numpy as np
@@ -51,9 +92,7 @@
 ...         [ 0.469,  0.150, -0.658, 0.248,  1.000, -0.370],
 ...         [ 0.283,  0.053, -0.085, 0.508, -0.370,  1.000],
 ...     ]
 ... )
 >>> distress_insurance_premium.estimate(default_probabilities, correlations)       
 0.28661995758
 ```
-
-For a complete list of supported built-in measures, please check [frds.io/measures/](https://frds.io/measures/).
```

### Comparing `frds-1.0.1/pyproject.toml` & `frds-1.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "frds"
-version = "1.0.1"
+version = "1.1.0"
 authors = [
   { name="Mingze Gao", email="adrian.gao@outlook.com" },
 ]
 description = "Financial Research Data Services"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -16,14 +16,15 @@
     "Intended Audience :: Financial and Insurance Industry",
     "Intended Audience :: Education",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering :: Information Analysis",
 ]
 license = {text = "MIT License"}
 dependencies = [
+  "arch",
   "numpy",
   "pandas",
   "scipy"
 ]
 
 
 [project.urls]
```

