# Comparing `tmp/hive-cli-0.2.0.tar.gz` & `tmp/hive-cli-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hive-cli-0.2.0.tar", max compression
+gzip compressed data, was "hive-cli-0.2.1.tar", max compression
```

## Comparing `hive-cli-0.2.0.tar` & `hive-cli-0.2.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1075 2023-05-23 10:31:27.358998 hive-cli-0.2.0/LICENSE
--rw-r--r--   0        0        0     4153 2023-05-25 10:31:13.485950 hive-cli-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-05-22 21:00:16.991460 hive-cli-0.2.0/hive/__init__.py
--rwxr-xr-x   0        0        0     4531 2023-05-25 10:31:53.568000 hive-cli-0.2.0/hive/cli.py
--rw-r--r--   0        0        0     2056 2023-05-25 10:31:49.467745 hive-cli-0.2.0/hive/parsers.py
--rw-r--r--   0        0        0     1805 2023-05-22 22:13:30.315961 hive-cli-0.2.0/hive/spinner.py
--rw-r--r--   0        0        0      509 2023-05-25 10:33:16.242969 hive-cli-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     5059 1970-01-01 00:00:00.000000 hive-cli-0.2.0/setup.py
--rw-r--r--   0        0        0     4742 1970-01-01 00:00:00.000000 hive-cli-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-05-23 10:31:27.358998 hive-cli-0.2.1/LICENSE
+-rw-r--r--   0        0        0     4125 2023-05-25 10:34:29.517459 hive-cli-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-22 21:00:16.991460 hive-cli-0.2.1/hive/__init__.py
+-rwxr-xr-x   0        0        0     4531 2023-05-25 10:31:53.568000 hive-cli-0.2.1/hive/cli.py
+-rw-r--r--   0        0        0     2056 2023-05-25 10:31:49.467745 hive-cli-0.2.1/hive/parsers.py
+-rw-r--r--   0        0        0     1805 2023-05-22 22:13:30.315961 hive-cli-0.2.1/hive/spinner.py
+-rw-r--r--   0        0        0      509 2023-05-25 10:34:35.518710 hive-cli-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5031 1970-01-01 00:00:00.000000 hive-cli-0.2.1/setup.py
+-rw-r--r--   0        0        0     4714 1970-01-01 00:00:00.000000 hive-cli-0.2.1/PKG-INFO
```

### Comparing `hive-cli-0.2.0/LICENSE` & `hive-cli-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hive-cli-0.2.0/README.md` & `hive-cli-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <p align="center">
-  <img height="175" src="https://github.com/PPierzc/hive/blob/main/docs/logo.png" alt="Qdrant">
+  <img height="175" src="https://github.com/PPierzc/hive/blob/main/docs/logo.png" alt="Hive Logo">
 </p>
 
 <p align="center">
-    <b>Unleash the power of Hive and navigate your knowledge base like a busy bee!  🐝🔍✨</b>
+    <b>Navigate your knowledge base like a busy bee! 🐝🔍✨</b>
 </p>
 
 <p align="center">
 <a href="https://github.com/psf/black"><img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Black Code Style"></a>
 <a href="https://github.com/ppierzc/hive/blob/main/LICENSE"><img src="https://img.shields.io/badge/License-MIT-blue.svg" alt="License"></a>
 </p>
```

#### html2text {}

```diff
@@ -1,10 +1,9 @@
-                                   [Qdrant]
-  Unleash the power of Hive and navigate your knowledge base like a busy bee!
-                                  ððâ¨
+                                  [Hive Logo]
+           Navigate your knowledge base like a busy bee! ððâ¨
                          [Black_Code_Style] [License]
 ð Hive is a CLI tool for semantic searching of your knowledge base ð. It
 allows you to easily search through your collection of files and directories,
 extracting meaningful information based on your prompts. No more searching
 through haystacksâlet Hive find the golden honey! ð¯ð Embrace the buzz
 and let your knowledge thrive! ðð¡ ## Getting Started ### Installation You
 can install Hive using pip: ```shell pip install hive-cli ``` ### Initializing
```

### Comparing `hive-cli-0.2.0/hive/cli.py` & `hive-cli-0.2.1/hive/cli.py`

 * *Files identical despite different names*

### Comparing `hive-cli-0.2.0/hive/parsers.py` & `hive-cli-0.2.1/hive/parsers.py`

 * *Files identical despite different names*

### Comparing `hive-cli-0.2.0/hive/spinner.py` & `hive-cli-0.2.1/hive/spinner.py`

 * *Files identical despite different names*

### Comparing `hive-cli-0.2.0/setup.py` & `hive-cli-0.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,17 +16,17 @@
  'typer[all]>=0.9.0,<0.10.0']
 
 entry_points = \
 {'console_scripts': ['hive = hive.cli:app']}
 
 setup_kwargs = {
     'name': 'hive-cli',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': '',
-    'long_description': '<p align="center">\n  <img height="175" src="https://github.com/PPierzc/hive/blob/main/docs/logo.png" alt="Qdrant">\n</p>\n\n<p align="center">\n    <b>Unleash the power of Hive and navigate your knowledge base like a busy bee!  🐝🔍✨</b>\n</p>\n\n<p align="center">\n<a href="https://github.com/psf/black"><img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Black Code Style"></a>\n<a href="https://github.com/ppierzc/hive/blob/main/LICENSE"><img src="https://img.shields.io/badge/License-MIT-blue.svg" alt="License"></a>\n</p>\n\n🐝 Hive is a CLI tool for semantic searching of your knowledge base 📚. It allows you to easily search through your collection of files and directories, extracting meaningful information based on your prompts.\n No more searching through haystacks—let Hive find the golden honey! 🍯🐝 Embrace the buzz and let your knowledge thrive! 🚀💡\n\n## Getting Started\n\n### Installation\nYou can install Hive using pip:\n\n```shell\npip install hive-cli\n```\n\n### Initializing Hive\nTo get started with Hive, initialize it in your project directory using the following command:\n\n```shell\nhive init\n```\nThis sets up Hive and creates the necessary configuration files to enable knowledge base searching.\n\n### Adding Files or Directories\nYou can add files or directories to your Hive knowledge base using the add command:\n\n```shell\nhive add <file_or_dir_to_add>\n```\nThis command allows Hive to index and analyze the content of the specified files or directories, making them searchable within your knowledge base.\n\n#### Supported File Types\nHive currently supports only Markdown and PDF files. Support for other file types is coming soon!\n\n### Searching the Knowledge Base\nTo perform a semantic search within your knowledge base, use the search command along with your prompt:\n\n```shell\nhive search "your prompt"\n```\nHive will analyze your prompt and match it against the indexed content, providing you with the most relevant results based on semantic similarity.\n\n#### Example Search Output\nHere\'s an example output of a search performed with Hive:\n\n```shell\nhive search "are honey bees good?"              \n\n╭─ ./data/the-problem-with-honey-bees.md ──────────────────────────────────────────────────────────────────────────────╮\n│                                                                                                                      │\n│  But think about them, we must. I used to believe that honey bees were a gateway species, and that concern over      │\n│  their health and prosperity would spill over onto native bees, benefitting them, too. While this may have happened  │\n│  in some cases, evidence is mounting that misguided enthusiasm for honey bees has likely been to the native bees’    │\n│  detriment. Beekeeping doesn’t make me feel good, anymore. In fact, quite the opposite.                              │\n│                                                                                                                      │\n╰─ Match score: 73% ───────────────────────────────────────────────────────────────────────────────────────────────────╯\n```\nThe search output displays the matched file, along with the relevant text snippet and a match score indicating the similarity between the prompt and the content.\n\n🔍 Hive makes it easy to find the information you need, saving you time and effort!\n\n## Contributing\nWe welcome contributions to Hive! Feel free to open issues and submit pull requests for any enhancements or bug fixes. Let\'s make Hive even better together! 🚀\n\n## License\nHive is licensed under the MIT License.\n\n🐝 Don\'t waste time searching, let Hive be your knowledge navigator! Start exploring your knowledge base effortlessly with Hive. Happy searching! 🚀✨',
+    'long_description': '<p align="center">\n  <img height="175" src="https://github.com/PPierzc/hive/blob/main/docs/logo.png" alt="Hive Logo">\n</p>\n\n<p align="center">\n    <b>Navigate your knowledge base like a busy bee! 🐝🔍✨</b>\n</p>\n\n<p align="center">\n<a href="https://github.com/psf/black"><img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Black Code Style"></a>\n<a href="https://github.com/ppierzc/hive/blob/main/LICENSE"><img src="https://img.shields.io/badge/License-MIT-blue.svg" alt="License"></a>\n</p>\n\n🐝 Hive is a CLI tool for semantic searching of your knowledge base 📚. It allows you to easily search through your collection of files and directories, extracting meaningful information based on your prompts.\n No more searching through haystacks—let Hive find the golden honey! 🍯🐝 Embrace the buzz and let your knowledge thrive! 🚀💡\n\n## Getting Started\n\n### Installation\nYou can install Hive using pip:\n\n```shell\npip install hive-cli\n```\n\n### Initializing Hive\nTo get started with Hive, initialize it in your project directory using the following command:\n\n```shell\nhive init\n```\nThis sets up Hive and creates the necessary configuration files to enable knowledge base searching.\n\n### Adding Files or Directories\nYou can add files or directories to your Hive knowledge base using the add command:\n\n```shell\nhive add <file_or_dir_to_add>\n```\nThis command allows Hive to index and analyze the content of the specified files or directories, making them searchable within your knowledge base.\n\n#### Supported File Types\nHive currently supports only Markdown and PDF files. Support for other file types is coming soon!\n\n### Searching the Knowledge Base\nTo perform a semantic search within your knowledge base, use the search command along with your prompt:\n\n```shell\nhive search "your prompt"\n```\nHive will analyze your prompt and match it against the indexed content, providing you with the most relevant results based on semantic similarity.\n\n#### Example Search Output\nHere\'s an example output of a search performed with Hive:\n\n```shell\nhive search "are honey bees good?"              \n\n╭─ ./data/the-problem-with-honey-bees.md ──────────────────────────────────────────────────────────────────────────────╮\n│                                                                                                                      │\n│  But think about them, we must. I used to believe that honey bees were a gateway species, and that concern over      │\n│  their health and prosperity would spill over onto native bees, benefitting them, too. While this may have happened  │\n│  in some cases, evidence is mounting that misguided enthusiasm for honey bees has likely been to the native bees’    │\n│  detriment. Beekeeping doesn’t make me feel good, anymore. In fact, quite the opposite.                              │\n│                                                                                                                      │\n╰─ Match score: 73% ───────────────────────────────────────────────────────────────────────────────────────────────────╯\n```\nThe search output displays the matched file, along with the relevant text snippet and a match score indicating the similarity between the prompt and the content.\n\n🔍 Hive makes it easy to find the information you need, saving you time and effort!\n\n## Contributing\nWe welcome contributions to Hive! Feel free to open issues and submit pull requests for any enhancements or bug fixes. Let\'s make Hive even better together! 🚀\n\n## License\nHive is licensed under the MIT License.\n\n🐝 Don\'t waste time searching, let Hive be your knowledge navigator! Start exploring your knowledge base effortlessly with Hive. Happy searching! 🚀✨',
     'author': 'paul',
     'author_email': 'ppierzc@gmail.copm',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,18 +1,17 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['hive']
 package_data = \ {'': ['*']} install_requires = \ ['Pillow>=9.5.0,<10.0.0',
 'PyPDF2>=3.0.1,<4.0.0', 'qdrant-client>=1.1.7,<2.0.0', 'sentence-
 transformers>=2.2.2,<3.0.0', 'torch>=2.0.1,<3.0.0', 'typer
 [all]>=0.9.0,<0.10.0'] entry_points = \ {'console_scripts': ['hive = hive.cli:
-app']} setup_kwargs = { 'name': 'hive-cli', 'version': '0.2.0', 'description':
+app']} setup_kwargs = { 'name': 'hive-cli', 'version': '0.2.1', 'description':
 '', 'long_description': '
-                                 \n [Qdrant]\n
+                               \n [Hive Logo]\n
 \n\n
-\n Unleash the power of Hive and navigate your knowledge base like a busy bee!
-                                 ððâ¨\n
+        \n Navigate your knowledge base like a busy bee! ððâ¨\n
 \n\n
                        \n[Black_Code_Style]\n[License]\n
 \n\nð Hive is a CLI tool for semantic searching of your knowledge base ð.
 It allows you to easily search through your collection of files and
 directories, extracting meaningful information based on your prompts.\n No more
 searching through haystacksâlet Hive find the golden honey! ð¯ð Embrace
 the buzz and let your knowledge thrive! ðð¡\n\n## Getting Started\n\n###
```

### Comparing `hive-cli-0.2.0/PKG-INFO` & `hive-cli-0.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hive-cli
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 Author: paul
 Author-email: ppierzc@gmail.copm
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -13,19 +13,19 @@
 Requires-Dist: qdrant-client (>=1.1.7,<2.0.0)
 Requires-Dist: sentence-transformers (>=2.2.2,<3.0.0)
 Requires-Dist: torch (>=2.0.1,<3.0.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 <p align="center">
-  <img height="175" src="https://github.com/PPierzc/hive/blob/main/docs/logo.png" alt="Qdrant">
+  <img height="175" src="https://github.com/PPierzc/hive/blob/main/docs/logo.png" alt="Hive Logo">
 </p>
 
 <p align="center">
-    <b>Unleash the power of Hive and navigate your knowledge base like a busy bee!  🐝🔍✨</b>
+    <b>Navigate your knowledge base like a busy bee! 🐝🔍✨</b>
 </p>
 
 <p align="center">
 <a href="https://github.com/psf/black"><img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Black Code Style"></a>
 <a href="https://github.com/ppierzc/hive/blob/main/LICENSE"><img src="https://img.shields.io/badge/License-MIT-blue.svg" alt="License"></a>
 </p>
```

#### html2text {}

```diff
@@ -1,18 +1,17 @@
-Metadata-Version: 2.1 Name: hive-cli Version: 0.2.0 Summary: Author: paul
+Metadata-Version: 2.1 Name: hive-cli Version: 0.2.1 Summary: Author: paul
 Author-email: ppierzc@gmail.copm Requires-Python: >=3.9,<3.12 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Requires-Dist: Pillow
 (>=9.5.0,<10.0.0) Requires-Dist: PyPDF2 (>=3.0.1,<4.0.0) Requires-Dist: qdrant-
 client (>=1.1.7,<2.0.0) Requires-Dist: sentence-transformers (>=2.2.2,<3.0.0)
 Requires-Dist: torch (>=2.0.1,<3.0.0) Requires-Dist: typer[all]
 (>=0.9.0,<0.10.0) Description-Content-Type: text/markdown
-                                   [Qdrant]
-  Unleash the power of Hive and navigate your knowledge base like a busy bee!
-                                  ððâ¨
+                                  [Hive Logo]
+           Navigate your knowledge base like a busy bee! ððâ¨
                          [Black_Code_Style] [License]
 ð Hive is a CLI tool for semantic searching of your knowledge base ð. It
 allows you to easily search through your collection of files and directories,
 extracting meaningful information based on your prompts. No more searching
 through haystacksâlet Hive find the golden honey! ð¯ð Embrace the buzz
 and let your knowledge thrive! ðð¡ ## Getting Started ### Installation You
 can install Hive using pip: ```shell pip install hive-cli ``` ### Initializing
```

