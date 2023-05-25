# Comparing `tmp/graph_datasets-0.1.2.tar.gz` & `tmp/graph_datasets-0.2.0.tar.gz`

## Comparing `graph_datasets-0.1.2.tar` & `graph_datasets-0.2.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/.editorconfig
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0    17935 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/.pylintrc
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/CHANGELOG.md
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/requirements-dev.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/requirements.txt
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/.github/workflows/release.yml
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/.vscode/extensions.json
--rw-r--r--   0        0        0    56106 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/configs/nb.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/demos/demo.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/docs/Makefile
--rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/docs/conf.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/docs/make.bat
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/docs/rst/data_info.rst
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/docs/rst/load_data.rst
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/docs/rst/src.utils.rst
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/docs/tpls/module.rst_t
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/docs/tpls/package.rst_t
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/docs/tpls/toc.rst_t
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/graph_datasets/__init__.py
--rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/graph_datasets/data_info.py
--rw-r--r--   0        0        0    27860 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/graph_datasets/load_data.py
--rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/graph_datasets/utils/__init__.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/scripts/build-publish.sh
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/scripts/bump.sh
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/scripts/cuda.sh
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/scripts/docs.sh
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/scripts/install-dev.sh
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/scripts/install.sh
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/scripts/nb.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/tests/test.py
--rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/LICENSE
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/README.md
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 graph_datasets-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/.editorconfig
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    17935 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/.pylintrc
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/=1.1.0
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/requirements-dev.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/requirements.txt
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/.ci/cuda.sh
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/.ci/docs.sh
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/.ci/install-dev.sh
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/.ci/install.sh
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/.ci/nb.sh
+-rw-r--r--   0        0        0    56106 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/.ci/configs/nb.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/.vscode/extensions.json
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/demos/demo.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/docs/Makefile
+-rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/docs/conf.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/docs/make.bat
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/docs/rst/data_info.rst
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/docs/rst/load_data.rst
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/docs/rst/src.utils.rst
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/docs/tpls/module.rst_t
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/docs/tpls/package.rst_t
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/docs/tpls/toc.rst_t
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/graph_datasets/__init__.py
+-rw-r--r--   0        0        0     2768 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/graph_datasets/data_info.py
+-rw-r--r--   0        0        0    28138 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/graph_datasets/load_data.py
+-rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/graph_datasets/utils/__init__.py
+-rw-r--r--   0        0        0     4880 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/graph_datasets/utils/statistics.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     5145 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/tests/statistics.py
+-rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/LICENSE
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/README.md
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 graph_datasets-0.2.0/PKG-INFO
```

### Comparing `graph_datasets-0.1.2/.pre-commit-config.yaml` & `graph_datasets-0.2.0/.pre-commit-config.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -1,53 +1,55 @@
 repos:
--   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.4.0
-    hooks:
-    -   id: trailing-whitespace
-    -   id: check-added-large-files
-    -   id: check-ast
-    -   id: check-case-conflict
-    -   id: check-merge-conflict
-    -   id: check-yaml
-    -   id: end-of-file-fixer
--   repo: https://github.com/asottile/reorder_python_imports
-    rev: v3.9.0
-    hooks:
-    -   id: reorder-python-imports
--   repo: local
-    hooks:
-    -   id: black
-        name: black
-        entry: black
-        language: system
-        types: [python]
-        exclude: |
-            (?x)^(
-                docs/*
-            )$
-    -   id: yapf
-        name: yapf
-        entry: yapf -r -i
-        language: system
-        types: [python]
-        exclude: |
-            (?x)^(
-                docs/*
-            )$
-    -   id: pylint
-        name: pylint
-        entry: pylint
-        language: system
-        types: [python]
-        exclude: |
-            (?x)^(
-                docs/*
-            )$
-    -   id: mdformat
-        name: mdformat
-        entry: mdformat
-        language: system
-        types: [markdown]
-        exclude: |
-            (?x)^(
-                CHANGELOG.md
-            )$
+    # -   repo: git@github.com:pre-commit/pre-commit-hooks
+    - repo: https://github.com/pre-commit/pre-commit-hooks
+      rev: v4.4.0
+      hooks:
+          - id: trailing-whitespace
+          - id: check-added-large-files
+          - id: check-ast
+          - id: check-case-conflict
+          - id: check-merge-conflict
+          - id: check-yaml
+          - id: end-of-file-fixer
+    # -   repo: git@github.com:asottile/reorder_python_imports
+    - repo: https://github.com/asottile/reorder_python_imports
+      rev: v3.9.0
+      hooks:
+          - id: reorder-python-imports
+    - repo: local
+      hooks:
+          - id: black
+            name: black
+            entry: black
+            language: system
+            types: [python]
+            exclude: |
+                (?x)^(
+                    docs/*
+                )$
+          - id: yapf
+            name: yapf
+            entry: yapf -r -i
+            language: system
+            types: [python]
+            exclude: |
+                (?x)^(
+                    docs/*
+                )$
+          - id: pylint
+            name: pylint
+            entry: pylint
+            language: system
+            types: [python]
+            exclude: |
+                (?x)^(
+                    docs/*
+                )$
+          - id: mdformat
+            name: mdformat
+            entry: mdformat
+            language: system
+            types: [markdown]
+            exclude: |
+                (?x)^(
+                    CHANGELOG.md
+                )$
```

### Comparing `graph_datasets-0.1.2/.pylintrc` & `graph_datasets-0.2.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.1.2/CHANGELOG.md` & `graph_datasets-0.2.0/CHANGELOG.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 <!--next-version-placeholder-->
 
+## v0.2.0 (2023-05-25)
+### Feature
+* Make it optional to remove self loops or convert to a simple graph ([`b2f751a`](https://github.com/galogm/graph_datasets/commit/b2f751add66597548863671f012c4cc428bcab17))
+* Add statistics for graph homophily metrics ([`3550814`](https://github.com/galogm/graph_datasets/commit/3550814fc17341e9b9b21bbef33be3cd173b3627))
+
 ## v0.1.2 (2023-05-12)
 ### Fix
 * Load data import error ([`1d8ac40`](https://github.com/galogm/graph_datasets/commit/1d8ac4045cad4ff662cd67e7c51f7befbc1cf061))
 
 ## v0.1.1 (2023-05-12)
 ### Fix
 * Fix DGL verbose and export load_data func ([`ea77e9c`](https://github.com/galogm/graph_datasets/commit/ea77e9ce6efc3deb871a90fcf3cb461340310ba6))
```

### Comparing `graph_datasets-0.1.2/.github/workflows/release.yml` & `graph_datasets-0.2.0/.github/workflows/release.yml`

 * *Files 20% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         with:
           fetch-depth: 0
       - name: Set up Python 3.7
         uses: actions/setup-python@v2
         with:
           python-version: 3.7.16
       - name: Install dependencies
-        run: bash scripts/install-dev.sh && bash scripts/install.sh
+        run: bash .ci/install-dev.sh && bash .ci/install.sh
       - name: Release
         run: |
           git config --global user.name "github-actions"
           git config --global user.email "action@github.com"
           source .venv/bin/activate && semantic-release publish -D commit_author="github-actions <action@github.com>"
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `graph_datasets-0.1.2/configs/nb.py` & `graph_datasets-0.2.0/.ci/configs/nb.py`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.1.2/docs/Makefile` & `graph_datasets-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.1.2/docs/conf.py` & `graph_datasets-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.1.2/docs/index.rst` & `graph_datasets-0.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.1.2/docs/make.bat` & `graph_datasets-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.1.2/docs/tpls/package.rst_t` & `graph_datasets-0.2.0/docs/tpls/package.rst_t`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.1.2/graph_datasets/data_info.py` & `graph_datasets-0.2.0/graph_datasets/data_info.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,16 +26,15 @@
     "wiki_features": "1ySNspxbK-snNoAZM7oxiWGvOnTRdSyEK",  # Wiki 1.9M
     "twitch-gamer_feat": "1fA9VIIEI8N0L27MSQfcBzJgRQLvSbrvR",
     "twitch-gamer_edges": "1XLETC6dG3lVl7kDmytEJ52hvDMVdxnZ0",
 }
 
 #: Supported datasets of pyG.
 #:
-#: **NOTE**: main difference of dgl and pyG datasets
-#:
+#: NOTE: main difference of dgl and pyG datasets
 #: - dgl has self-loops while pyG removes them.
 #: - dgl row normalizes features while pyG does not.
 PYG_DATASETS = [
     "cora",
     "citeseer",
     "pubmed",
     "corafull",
@@ -66,17 +65,17 @@
     "cornell",
     "texas",
     "wisconsin",
 ]
 OGB_DATASETS = [
     "products",
     "arxiv",
-    "mag",
-    "proteins",
-    "papers100M",
+    # "mag",
+    # "proteins",
+    # "papers100M",
 ]
 #: Datasets in paper
 #: `SDCN <https://github.com/bdy9527/SDCN>`_.
 SDCN_DATASETS = [
     "dblp",
     "acm",
 ]
@@ -106,7 +105,16 @@
     "yelp-chi",
     "deezer-europe",
     "Amherst41",
     "Cornell5",
     "Johns Hopkins55",
     "Reed98",
 ]
+
+DATASETS = {
+    "pyg": PYG_DATASETS,
+    "dgl": DGL_DATASETS,
+    "ogb": OGB_DATASETS,
+    "sdcn": SDCN_DATASETS,
+    "cola": COLA_DATASETS,
+    "linkx": LINKX_DATASETS,
+}
```

### Comparing `graph_datasets-0.1.2/graph_datasets/load_data.py` & `graph_datasets-0.2.0/graph_datasets/load_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,24 +46,28 @@
 
 
 def load_data(
     dataset_name: str,
     directory: str = DEFAULT_DATA_DIR,
     verbosity: int = 0,
     source: str = "pyg",
+    rm_self_loop: bool = True,
+    to_simple: bool = True,
 ) -> Tuple[dgl.DGLGraph, torch.Tensor, int]:
     """Load graphs.
 
     Args:
         dataset_name (str): Dataset name.
         directory (str, optional): Raw dir for loading or saving. \
             Defaults to DEFAULT_DATA_DIR=os.path.abspath("./data").
         verbosity (int, optional): Output debug information. \
             The greater, the more detailed. Defaults to 0.
         source (str, optional): Source for data loading. Defaults to "pyg".
+        rm_self_loop (str, optional): Remove self loops. Defaults to True.
+        to_simple (str, optional): Convert to a simple graph with no duplicate undirected edges.
 
     Raises:
         NotImplementedError: Dataset unknown.
 
     Returns:
         Tuple[dgl.DGLGraph, torch.Tensor, int]: [graph, label, n_clusters]
 
@@ -120,16 +124,18 @@
         )
     else:
         raise NotImplementedError(
             f"{dataset_name} is not supported or source {source} is incorrect."
         )
 
     # remove self loop and turn graphs into undirected ones
-    graph = dgl.remove_self_loop(graph)
-    graph = dgl.to_bidirected(graph, copy_ndata=True)
+    if rm_self_loop:
+        graph = dgl.remove_self_loop(graph)
+    if to_simple:
+        graph = dgl.to_bidirected(graph, copy_ndata=True)
 
     # make label from 0
     uni = label.unique()
     old2new = dict(zip(uni.numpy().tolist(), list(range(len(uni)))))
     newlabel = torch.tensor(list(map(lambda x: old2new[x.item()], label)))
     graph.ndata["label"] = newlabel
```

### Comparing `graph_datasets-0.1.2/graph_datasets/utils/__init__.py` & `graph_datasets-0.2.0/graph_datasets/utils/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 from typing import Any
 from typing import Dict
 from typing import List
 
 import gdown
 from texttable import Texttable
 
+from .statistics import edge_homo
+from .statistics import node_homo
+from .statistics import statistics
+
 
 def format_value(value) -> Any:
     if f"{value}".isdecimal():
         return f"{value:,}"
     return value
```

### Comparing `graph_datasets-0.1.2/scripts/cuda.sh` & `graph_datasets-0.2.0/.ci/cuda.sh`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.1.2/scripts/install.sh` & `graph_datasets-0.2.0/.ci/install.sh`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # # install python 3.7.16 use pyenv
+# sudo apt-get install zlib1g-dev libffi-dev libreadline-dev libssl-dev libsqlite3-dev libncurses5 libncurses5-dev libncursesw5 lzma liblzma-dev libbz2-dev
 # pyenv install 3.7.16
 # pyenv local 3.7.16
 
 # create and activate virtual environment
 if [ ! -d '.venv' ]; then
     python3 -m venv .venv && echo create venv
 else
@@ -13,15 +14,17 @@
 
 # # update pip
 # python -m pip install -U pip
 
 # # torch cuda 11.3
 python -m pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu113
 
-# # dgl cuda 11.3
-python -m pip install dgl -f https://data.dgl.ai/wheels/cu113/repo.html -i https://pypi.tuna.tsinghua.edu.cn/simple/
-python -m pip install dglgo -f https://data.dgl.ai/wheels-test/repo.html -i https://pypi.tuna.tsinghua.edu.cn/simple/
-
-# # install requirements
-python -m pip install -r requirements.txt -i https://pypi.tuna.tsinghua.edu.cn/simple/
+# dgl cuda 11.3
+# add a source if prefered: -i https://pypi.tuna.tsinghua.edu.cn/simple/
+python -m pip install dgl>=1.1.0 -f https://data.dgl.ai/wheels/cu113/repo.html
+python -m pip install dglgo -f https://data.dgl.ai/wheels-test/repo.html
+
+# install requirements
+# add a source if prefered: -i https://pypi.tuna.tsinghua.edu.cn/simple/
+python -m pip install -r requirements.txt
 
 echo install requirements successfully!
```

### Comparing `graph_datasets-0.1.2/.gitignore` & `graph_datasets-0.2.0/.gitignore`

 * *Files 0% similar despite different names*

```diff
@@ -176,7 +176,8 @@
 .vscode/*
 !.vscode/extensions.json
 
 docs/_build
 docs/rst_tmp
 
 .python-version
+test.py
```

### Comparing `graph_datasets-0.1.2/LICENSE` & `graph_datasets-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.1.2/README.md` & `graph_datasets-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `graph_datasets-0.1.2/pyproject.toml` & `graph_datasets-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "graph_datasets"
-version = "0.1.2"
+version = "0.2.0"
 authors = [{ name = "galo.gm", email = "galo.gm.work@gmail.com" }]
 keywords = ["graph", "datasets"]
 description = "Load graph datasets."
 readme = "README.md"
 license = "MIT"
 requires-python = ">=3.7"
 classifiers = [
@@ -17,15 +17,15 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dependencies = [
     "torch>=1.10.2",
     "torch-geometric>=2.0.3",
     "torchaudio>=0.10.2",
     "torchvision>=0.11.3",
-    "dgl>=0.9.0",
+    "dgl>=1.1.0",
     "dglgo>=0.0.2",
     "gdown>=4.7",
     "wget>=3.2",
     "texttable>=1.6",
 ]
 
 [project.urls]
```

### Comparing `graph_datasets-0.1.2/PKG-INFO` & `graph_datasets-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: graph_datasets
-Version: 0.1.2
+Version: 0.2.0
 Summary: Load graph datasets.
 Project-URL: Homepage, https://github.com/galogm/graph_datasets
 Project-URL: Bug Tracker, https://github.com/galogm/graph_datasets/issues
 Author-email: "galo.gm" <galo.gm.work@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: datasets,graph
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
-Requires-Dist: dgl>=0.9.0
+Requires-Dist: dgl>=1.1.0
 Requires-Dist: dglgo>=0.0.2
 Requires-Dist: gdown>=4.7
 Requires-Dist: texttable>=1.6
 Requires-Dist: torch-geometric>=2.0.3
 Requires-Dist: torch>=1.10.2
 Requires-Dist: torchaudio>=0.10.2
 Requires-Dist: torchvision>=0.11.3
```

