# Comparing `tmp/llmo-0.4.1.tar.gz` & `tmp/llmo-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmo-0.4.1.tar", last modified: Wed May 24 21:02:39 2023, max compression
+gzip compressed data, was "llmo-0.4.2.tar", last modified: Wed May 24 23:07:46 2023, max compression
```

## Comparing `llmo-0.4.1.tar` & `llmo-0.4.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11349 2023-05-21 19:33:44.704545 llmo-0.4.1/LICENSE
--rw-r--r--   0        0        0     2134 2023-05-22 08:06:19.890271 llmo-0.4.1/README.md
--rw-r--r--   0        0        0        0 2023-05-21 19:29:22.111252 llmo-0.4.1/llmo/__init__.py
--rw-r--r--   0        0        0     2961 2023-05-24 03:21:31.439301 llmo-0.4.1/llmo/cli.py
--rw-r--r--   0        0        0      122 2023-05-22 21:51:03.475865 llmo-0.4.1/llmo/constants.py
--rw-r--r--   0        0        0     9793 2023-05-23 03:53:39.625867 llmo-0.4.1/llmo/gui.py
--rw-r--r--   0        0        0      341 2023-05-23 03:17:45.469101 llmo-0.4.1/llmo/layout.css
--rw-r--r--   0        0        0     6481 2023-05-24 21:01:58.190536 llmo-0.4.1/llmo/llms.py
--rw-r--r--   0        0        0     1593 2023-05-23 04:53:16.585981 llmo-0.4.1/llmo/shell_mode.py
--rw-r--r--   0        0        0      722 2023-05-24 21:02:39.225131 llmo-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      838 2023-05-22 22:24:34.139710 llmo-0.4.1/tests/test_openai.py
--rw-r--r--   0        0        0     2510 1970-01-01 00:00:00.000000 llmo-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-05-21 19:33:44.704545 llmo-0.4.2/LICENSE
+-rw-r--r--   0        0        0     2373 2023-05-24 23:06:37.762004 llmo-0.4.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-21 19:29:22.111252 llmo-0.4.2/llmo/__init__.py
+-rw-r--r--   0        0        0     2961 2023-05-24 03:21:31.439301 llmo-0.4.2/llmo/cli.py
+-rw-r--r--   0        0        0      122 2023-05-22 21:51:03.475865 llmo-0.4.2/llmo/constants.py
+-rw-r--r--   0        0        0     9793 2023-05-23 03:53:39.625867 llmo-0.4.2/llmo/gui.py
+-rw-r--r--   0        0        0      341 2023-05-23 03:17:45.469101 llmo-0.4.2/llmo/layout.css
+-rw-r--r--   0        0        0     6481 2023-05-24 21:01:58.190536 llmo-0.4.2/llmo/llms.py
+-rw-r--r--   0        0        0     1593 2023-05-23 04:53:16.585981 llmo-0.4.2/llmo/shell_mode.py
+-rw-r--r--   0        0        0      722 2023-05-24 23:07:46.252966 llmo-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      838 2023-05-22 22:24:34.139710 llmo-0.4.2/tests/test_openai.py
+-rw-r--r--   0        0        0     2749 1970-01-01 00:00:00.000000 llmo-0.4.2/PKG-INFO
```

### Comparing `llmo-0.4.1/LICENSE` & `llmo-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `llmo-0.4.1/README.md` & `llmo-0.4.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -4,18 +4,22 @@
 - Protector
 - Worthy to be Loved
 - Helm from God
 - (**Most Importantly**) A helpful AI programming CLI tool
 
 <img src="https://github.com/knowsuchagency/llmo/blob/main/static/mascot.png?raw=true" alt="mascot" style="width: 400px; height: auto;">   
 
-The full power of GPT straight from your terminal!
+LLMO is the AI pair programming tool that meets you where you are (your terminal) 😉
 
 With the **"staging area"**, you can keep files in the context window without the hassle of copying and pasting every time you make changes to your code.
 
+## Demo
+
+https://github.com/knowsuchagency/llmo/assets/11974795/72419d64-585b-4cd5-a546-2a07de3e6f03
+
 
 ## Features
 
 - Interactive Chat: Enjoy real-time, interactive programming assistance in your terminal.
 - Staging Area: Easily add files to the AI's context to update it about your ongoing coding tasks. No need to copy and paste updates.
 - Model Customization: Choose the OpenAI model that fits your needs.
 - Personality: By default, Elmo loves to make bodybuilding references. This can be turned off through a CLI flag or environment variable.
@@ -26,18 +30,15 @@
 
 ```bash
 pipx install llmo
 ```
 
 ## Usage
 
-Here's how you can use llmo from the command line:
-
 ```bash
-# Basic usage
 llmo --help
 # you can also use the shorthand
 lm
 
 # You can pass the -s flag if you don't need the full GUI mode
 lm -s "Could you show me an example of valid json?"
 
@@ -47,26 +48,35 @@
 # from utils import add_numbers
 # result = add_numbers(5, 3)
 
 # utils.py
 # def add_numbers(a, b):
 #     return a + b
 
-lm "How can I make add_numbers return a string?" -f "main.py" -f "utils.py"
+lm "How can I make add_numbers return a string?" -f main.py -f utils.py
 ```
 
 ## Notes
 
+### Authentication
+
+This application uses the [OpenAI][openai] API.
+
+You will need to authenticate with your own API Key.
+
+### Copying Text
+
 [Textual][textual] runs the terminal in application mode. The means that you can't simply copy content as you normally would.
 In [iterm2][iterm2], you can hold down the `option` key to select text. See the documentation for your terminal emulator for more information.
 
 ## License
 
 [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0)
 
 ## Disclaimer
 
 This tool is not officially associated with OpenAI. Always follow OpenAI's use case policy when interacting with their API.
 
 [pipx]: https://github.com/pypa/pipx
 [textual]: https://textual.textualize.io/
 [iterm2]: https://iterm2.com/
+[openai]: https://openai.com/
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `llmo-0.4.1/llmo/cli.py` & `llmo-0.4.2/llmo/cli.py`

 * *Files identical despite different names*

### Comparing `llmo-0.4.1/llmo/gui.py` & `llmo-0.4.2/llmo/gui.py`

 * *Files identical despite different names*

### Comparing `llmo-0.4.1/llmo/llms.py` & `llmo-0.4.2/llmo/llms.py`

 * *Files identical despite different names*

### Comparing `llmo-0.4.1/llmo/shell_mode.py` & `llmo-0.4.2/llmo/shell_mode.py`

 * *Files identical despite different names*

### Comparing `llmo-0.4.1/tests/test_openai.py` & `llmo-0.4.2/tests/test_openai.py`

 * *Files identical despite different names*

### Comparing `llmo-0.4.1/PKG-INFO` & `llmo-0.4.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmo
-Version: 0.4.1
+Version: 0.4.2
 Summary: AI pair programmer
 Author-Email: Stephan Fitzpatrick <stephan@knowsuchagency.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/knowsuchagency/llmo
 Requires-Python: >=3.10
 Requires-Dist: textual>=0.26.0
 Requires-Dist: openai>=0.27.6
@@ -17,18 +17,22 @@
 - Protector
 - Worthy to be Loved
 - Helm from God
 - (**Most Importantly**) A helpful AI programming CLI tool
 
 <img src="https://github.com/knowsuchagency/llmo/blob/main/static/mascot.png?raw=true" alt="mascot" style="width: 400px; height: auto;">   
 
-The full power of GPT straight from your terminal!
+LLMO is the AI pair programming tool that meets you where you are (your terminal) 😉
 
 With the **"staging area"**, you can keep files in the context window without the hassle of copying and pasting every time you make changes to your code.
 
+## Demo
+
+https://github.com/knowsuchagency/llmo/assets/11974795/72419d64-585b-4cd5-a546-2a07de3e6f03
+
 
 ## Features
 
 - Interactive Chat: Enjoy real-time, interactive programming assistance in your terminal.
 - Staging Area: Easily add files to the AI's context to update it about your ongoing coding tasks. No need to copy and paste updates.
 - Model Customization: Choose the OpenAI model that fits your needs.
 - Personality: By default, Elmo loves to make bodybuilding references. This can be turned off through a CLI flag or environment variable.
@@ -39,18 +43,15 @@
 
 ```bash
 pipx install llmo
 ```
 
 ## Usage
 
-Here's how you can use llmo from the command line:
-
 ```bash
-# Basic usage
 llmo --help
 # you can also use the shorthand
 lm
 
 # You can pass the -s flag if you don't need the full GUI mode
 lm -s "Could you show me an example of valid json?"
 
@@ -60,26 +61,35 @@
 # from utils import add_numbers
 # result = add_numbers(5, 3)
 
 # utils.py
 # def add_numbers(a, b):
 #     return a + b
 
-lm "How can I make add_numbers return a string?" -f "main.py" -f "utils.py"
+lm "How can I make add_numbers return a string?" -f main.py -f utils.py
 ```
 
 ## Notes
 
+### Authentication
+
+This application uses the [OpenAI][openai] API.
+
+You will need to authenticate with your own API Key.
+
+### Copying Text
+
 [Textual][textual] runs the terminal in application mode. The means that you can't simply copy content as you normally would.
 In [iterm2][iterm2], you can hold down the `option` key to select text. See the documentation for your terminal emulator for more information.
 
 ## License
 
 [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0)
 
 ## Disclaimer
 
 This tool is not officially associated with OpenAI. Always follow OpenAI's use case policy when interacting with their API.
 
 [pipx]: https://github.com/pypa/pipx
 [textual]: https://textual.textualize.io/
 [iterm2]: https://iterm2.com/
+[openai]: https://openai.com/
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

