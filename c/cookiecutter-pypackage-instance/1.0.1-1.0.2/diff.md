# Comparing `tmp/cookiecutter_pypackage_instance-1.0.1.tar.gz` & `tmp/cookiecutter_pypackage_instance-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cookiecutter_pypackage_instance-1.0.1.tar", max compression
+gzip compressed data, was "cookiecutter_pypackage_instance-1.0.2.tar", max compression
```

## Comparing `cookiecutter_pypackage_instance-1.0.1.tar` & `cookiecutter_pypackage_instance-1.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1089 2023-05-21 13:28:20.029647 cookiecutter_pypackage_instance-1.0.1/LICENSE
--rw-r--r--   0        0        0     4136 2023-05-21 13:28:20.029647 cookiecutter_pypackage_instance-1.0.1/README.md
--rw-r--r--   0        0        0     4356 2023-05-21 13:28:21.025660 cookiecutter_pypackage_instance-1.0.1/pyproject.toml
--rw-r--r--   0        0        0       82 2023-05-21 13:28:20.029647 cookiecutter_pypackage_instance-1.0.1/src/cookiecutter_pypackage_instance/__init__.py
--rw-r--r--   0        0        0      417 2023-05-21 13:28:20.029647 cookiecutter_pypackage_instance-1.0.1/src/cookiecutter_pypackage_instance/cookiecutter_pypackage_instance.py
--rw-r--r--   0        0        0        0 2023-05-21 13:28:20.029647 cookiecutter_pypackage_instance-1.0.1/src/cookiecutter_pypackage_instance/py.typed
--rw-r--r--   0        0        0     5137 1970-01-01 00:00:00.000000 cookiecutter_pypackage_instance-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-05-25 16:39:04.095058 cookiecutter_pypackage_instance-1.0.2/LICENSE
+-rw-r--r--   0        0        0     4136 2023-05-25 16:39:04.095058 cookiecutter_pypackage_instance-1.0.2/README.md
+-rw-r--r--   0        0        0     4952 2023-05-25 16:39:05.019072 cookiecutter_pypackage_instance-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0       82 2023-05-25 16:39:04.095058 cookiecutter_pypackage_instance-1.0.2/src/cookiecutter_pypackage_instance/__init__.py
+-rw-r--r--   0        0        0      417 2023-05-25 16:39:04.095058 cookiecutter_pypackage_instance-1.0.2/src/cookiecutter_pypackage_instance/cookiecutter_pypackage_instance.py
+-rw-r--r--   0        0        0        0 2023-05-25 16:39:04.095058 cookiecutter_pypackage_instance-1.0.2/src/cookiecutter_pypackage_instance/py.typed
+-rw-r--r--   0        0        0     5137 1970-01-01 00:00:00.000000 cookiecutter_pypackage_instance-1.0.2/PKG-INFO
```

### Comparing `cookiecutter_pypackage_instance-1.0.1/LICENSE` & `cookiecutter_pypackage_instance-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cookiecutter_pypackage_instance-1.0.1/README.md` & `cookiecutter_pypackage_instance-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `cookiecutter_pypackage_instance-1.0.1/pyproject.toml` & `cookiecutter_pypackage_instance-1.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "cookiecutter-pypackage-instance"
-version = "1.0.1"
+version = "1.0.2"
 description = "🐍 An awesome python package by the name Cookiecutter Pypackage Instance"
 readme = "README.md"
 authors = ["Vasilis Sioros <billsioros97@gmail.com>"]
 license = "MIT"
 homepage = "https://billsioros.github.io/cookiecutter-pypackage-instance"
 repository = "https://github.com/billsioros/cookiecutter-pypackage-instance"
 keywords = []
@@ -22,18 +22,16 @@
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/billsioros/cookiecutter-pypackage-instance/issues"
 "Changelog" = "https://github.com/billsioros/cookiecutter-pypackage-instance/releases"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 python-semantic-release = "*"
-wemake-python-styleguide = "*"
-flakeheaven = "*"
 isort = "*"
 mypy = "*"
 black = "*"
 pre-commit = "*"
 poethepoet = "*"
 coverage = {extras = ["toml"], version = "*" }
 pytest = "*"
@@ -43,14 +41,15 @@
 mkdocs = "*"
 mkdocs-material = "*"
 mkdocs-minify-plugin = "*"
 mkdocs-redirects = "*"
 mkdocstrings = { extras = ["python"], version = "*" }
 mdx-truly-sane-lists = "*"
 mike = "*"
+ruff = "*"
 
 [tool.semantic_release]
 version_toml = "pyproject.toml:tool.poetry.version"
 changelog_components = "semantic_release.changelog.changelog_headers,semantic_release.changelog.compare_url"
 build_command = "python -m pip install poetry && poetry build"
 
 [tool.vulture]
@@ -59,15 +58,15 @@
 
 [tool.poe.tasks]
 clean = { cmd = "rm -rf ./**/__pycache__ dist site .pytest_cache .mypy_cache .coverage", help = "Clean up any auxiliary files" }
 format = { shell = "poetry run isort .; poetry run black .", help = "Format your codebase" }
 hooks = { cmd = "poetry run pre-commit run --all-files", help = "Run all pre-commit hooks" }
 test = { cmd = "poetry run pytest --cov=cookiecutter_pypackage_instance", help = "Run the test suite and produce a coverage report" }
 type-check = { cmd = "poetry run mypy", help = "Run static type checking on your codebase" }
-lint = { cmd = "poetry run flakeheaven lint", help = "Lint your code for errors" }
+lint = { cmd = "poetry run ruff check src", help = "Lint your code for errors" }
 docs = { shell = "python -c 'import webbrowser; webbrowser.open(\"http://127.0.0.1:8000\")'; poetry run mkdocs serve", help = "Build and serve the documentation" }
 export = { cmd = "poetry export --without-hashes --dev -o requirements.txt" }
 
 [tool.pytest.ini_options]
 addopts = "-vv --color=yes"
 log_cli = false
 log_cli_date_format = "%Y-%m-%d %H:%M:%S"
@@ -110,43 +109,54 @@
 pretty = true
 color_output = true
 show_column_numbers = true
 show_error_codes = true
 show_error_context = true
 strict = true
 
-[tool.flakeheaven]
+
+[tool.ruff]
+select = ["A", "B", "C", "D", "E", "F", "G", "I", "N", "Q", "S", "T", "W", "ANN", "ARG", "BLE", "COM", "DJ", "DTZ", "EM", "ERA", "EXE", "FBT", "ICN", "INP", "ISC", "NPY", "PD", "PGH", "PIE", "PL", "PT", "PTH", "PYI", "RET", "RSE", "RUF", "SIM", "SLF", "TCH", "TID", "TRY", "UP", "YTT"]
+ignore = []
+
+fixable = ["A", "B", "C", "D", "E", "F", "G", "I", "N", "Q", "S", "T", "W", "ANN", "ARG", "BLE", "COM", "DJ", "DTZ", "EM", "ERA", "EXE", "FBT", "ICN", "INP", "ISC", "NPY", "PD", "PGH", "PIE", "PL", "PT", "PTH", "PYI", "RET", "RSE", "RUF", "SIM", "SLF", "TCH", "TID", "TRY", "UP", "YTT"]
+unfixable = []
+
 exclude = [
-  ".git",
-  ".github",
-  ".mypy_cache",
-  ".pytest_cache",
-  ".vscode",
-  ".venv",
-  "build",
-  "dist",
-  "docs",
-  "tests",
-  "__pycache__",
-  "README.md"
+    ".bzr",
+    ".direnv",
+    ".eggs",
+    ".git",
+    ".git-rewrite",
+    ".hg",
+    ".mypy_cache",
+    ".nox",
+    ".pants.d",
+    ".pytype",
+    ".ruff_cache",
+    ".svn",
+    ".tox",
+    ".venv",
+    "__pypackages__",
+    "_build",
+    "buck-out",
+    "build",
+    "dist",
+    "node_modules",
+    "venv",
 ]
-format = "colored"
-show_source = false
-statistics = false
-docstring-convention = "google"
-
-accept_encodings = "utf-8"
-max_line_length = 99
-
-extended_default_ignore = []
-
-[tool.flakeheaven.plugins]
-"flake8-*" = ["+*"]
-mccabe = ["+*"]
-nitpick = ["+*"]
-"pep8-naming" = ["+*"]
-pycodestyle = ["+*"]
-pyflakes = ["+*"]
-"wemake-python-styleguide" = ["+*"]
+per-file-ignores = {}
+
+line-length = 99
 
-[tool.pydocstyle]
+dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
+
+target-version = "py310"
+
+[tool.ruff.mccabe]
+max-complexity = 10
+
+[tool.ruff.pydocstyle]
 convention = "google"
+
+[tool.ruff.flake8-quotes]
+docstring-quotes = "double"
```

### Comparing `cookiecutter_pypackage_instance-1.0.1/PKG-INFO` & `cookiecutter_pypackage_instance-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cookiecutter-pypackage-instance
-Version: 1.0.1
+Version: 1.0.2
 Summary: 🐍 An awesome python package by the name Cookiecutter Pypackage Instance
 Home-page: https://billsioros.github.io/cookiecutter-pypackage-instance
 License: MIT
 Author: Vasilis Sioros
 Author-email: billsioros97@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cookiecutter-pypackage-instance Version: 1.0.1
+Metadata-Version: 2.1 Name: cookiecutter-pypackage-instance Version: 1.0.2
 Summary: ð An awesome python package by the name Cookiecutter Pypackage
 Instance Home-page: https://billsioros.github.io/cookiecutter-pypackage-
 instance License: MIT Author: Vasilis Sioros Author-email:
 billsioros97@gmail.com Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
```

