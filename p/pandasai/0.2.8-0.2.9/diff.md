# Comparing `tmp/pandasai-0.2.8.tar.gz` & `tmp/pandasai-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasai-0.2.8.tar", max compression
+gzip compressed data, was "pandasai-0.2.9.tar", max compression
```

## Comparing `pandasai-0.2.8.tar` & `pandasai-0.2.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1055 2023-04-24 05:55:05.323190 pandasai-0.2.8/LICENSE
--rw-r--r--   0        0        0     5641 2023-05-07 22:56:45.170152 pandasai-0.2.8/README.md
--rw-r--r--   0        0        0     7616 2023-05-08 14:49:29.162424 pandasai-0.2.8/pandasai/__init__.py
--rw-r--r--   0        0        0      166 2023-05-08 09:22:18.023055 pandasai-0.2.8/pandasai/constants.py
--rw-r--r--   0        0        0      884 2023-05-02 20:00:39.808655 pandasai-0.2.8/pandasai/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-03 14:53:42.378883 pandasai-0.2.8/pandasai/helpers/__init__.py
--rw-r--r--   0        0        0     4646 2023-05-06 22:56:45.185822 pandasai-0.2.8/pandasai/helpers/anonymizer.py
--rw-r--r--   0        0        0     1505 2023-05-03 14:53:42.379406 pandasai-0.2.8/pandasai/helpers/notebook.py
--rw-r--r--   0        0        0        0 2023-04-30 09:49:31.456755 pandasai-0.2.8/pandasai/llm/__init__.py
--rw-r--r--   0        0        0     1493 2023-05-07 12:19:23.603585 pandasai-0.2.8/pandasai/llm/alpaca.py
--rw-r--r--   0        0        0     3539 2023-05-08 09:22:18.023356 pandasai-0.2.8/pandasai/llm/base.py
--rw-r--r--   0        0        0     1409 2023-05-07 12:19:27.955602 pandasai-0.2.8/pandasai/llm/base_hf.py
--rw-r--r--   0        0        0      505 2023-05-07 12:19:34.602219 pandasai-0.2.8/pandasai/llm/fake.py
--rw-r--r--   0        0        0      755 2023-05-06 12:44:40.587293 pandasai-0.2.8/pandasai/llm/open_assistant.py
--rw-r--r--   0        0        0     3851 2023-05-07 12:17:45.967747 pandasai-0.2.8/pandasai/llm/openai.py
--rw-r--r--   0        0        0      689 2023-05-07 10:03:05.449931 pandasai-0.2.8/pandasai/llm/starcoder.py
--rw-r--r--   0        0        0      728 2023-05-08 14:49:36.490884 pandasai-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     6450 1970-01-01 00:00:00.000000 pandasai-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-04-24 05:55:05.323190 pandasai-0.2.9/LICENSE
+-rw-r--r--   0        0        0     5641 2023-05-07 22:56:45.170152 pandasai-0.2.9/README.md
+-rw-r--r--   0        0        0     9012 2023-05-08 23:43:04.960305 pandasai-0.2.9/pandasai/__init__.py
+-rw-r--r--   0        0        0     1025 2023-05-08 23:41:52.704456 pandasai-0.2.9/pandasai/constants.py
+-rw-r--r--   0        0        0      884 2023-05-02 20:00:39.808655 pandasai-0.2.9/pandasai/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-03 14:53:42.378883 pandasai-0.2.9/pandasai/helpers/__init__.py
+-rw-r--r--   0        0        0     4646 2023-05-06 22:56:45.185822 pandasai-0.2.9/pandasai/helpers/anonymizer.py
+-rw-r--r--   0        0        0     1505 2023-05-03 14:53:42.379406 pandasai-0.2.9/pandasai/helpers/notebook.py
+-rw-r--r--   0        0        0        0 2023-04-30 09:49:31.456755 pandasai-0.2.9/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0     1493 2023-05-07 12:19:23.603585 pandasai-0.2.9/pandasai/llm/alpaca.py
+-rw-r--r--   0        0        0     3020 2023-05-08 23:41:52.704520 pandasai-0.2.9/pandasai/llm/base.py
+-rw-r--r--   0        0        0     1409 2023-05-07 12:19:27.955602 pandasai-0.2.9/pandasai/llm/base_hf.py
+-rw-r--r--   0        0        0      505 2023-05-08 23:08:22.612651 pandasai-0.2.9/pandasai/llm/fake.py
+-rw-r--r--   0        0        0      763 2023-05-08 23:40:05.209518 pandasai-0.2.9/pandasai/llm/open_assistant.py
+-rw-r--r--   0        0        0     3859 2023-05-08 23:40:53.213540 pandasai-0.2.9/pandasai/llm/openai.py
+-rw-r--r--   0        0        0      697 2023-05-08 23:39:55.732086 pandasai-0.2.9/pandasai/llm/starcoder.py
+-rw-r--r--   0        0        0      862 2023-05-08 23:49:50.082167 pandasai-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     6493 1970-01-01 00:00:00.000000 pandasai-0.2.9/PKG-INFO
```

### Comparing `pandasai-0.2.8/LICENSE` & `pandasai-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.8/README.md` & `pandasai-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.8/pandasai/__init__.py` & `pandasai-0.2.9/pandasai/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 """ PandasAI is a wrapper around a LLM to make dataframes convesational """
+import ast
 import io
 from contextlib import redirect_stdout
 from datetime import date
 from typing import Optional
 
+import astor
 import pandas as pd
 
-from .constants import END_CODE_TAG, START_CODE_TAG
+from .constants import (
+    END_CODE_TAG,
+    START_CODE_TAG,
+    WHITELISTED_BUILTINS,
+    WHITELISTED_LIBRARIES,
+)
 from .exceptions import LLMNotFoundError
 from .helpers.anonymizer import anonymize_dataframe_head
 from .helpers.notebook import Notebook
 from .llm.base import LLM
 
 
 # pylint: disable=too-many-instance-attributes disable=too-many-arguments
@@ -156,51 +163,86 @@
         if is_conversational_answer is None:
             is_conversational_answer = self._is_conversational_answer
         if is_conversational_answer:
             answer = self.conversational_answer(prompt, code, answer)
             self.log(f"Conversational answer: {answer}")
         return answer
 
+    def remove_unsafe_imports(self, code: str) -> str:
+        """Remove non-whitelisted imports from the code to prevent malicious code execution"""
+
+        tree = ast.parse(code)
+        new_body = [
+            node
+            for node in tree.body
+            if not (
+                isinstance(node, (ast.Import, ast.ImportFrom))
+                and any(alias.name not in WHITELISTED_LIBRARIES for alias in node.names)
+            )
+        ]
+        new_tree = ast.Module(body=new_body)
+        return astor.to_source(new_tree).strip()
+
     def run_code(
         self,
         code: str,
-        df: pd.DataFrame,  # pylint: disable=W0613 disable=C0103
+        data_frame: pd.DataFrame,
         use_error_correction_framework: bool = True,
     ) -> str:
         # pylint: disable=W0122 disable=W0123 disable=W0702:bare-except
         """Run the code in the current context and return the result"""
 
         # Redirect standard output to a StringIO buffer
         with redirect_stdout(io.StringIO()) as output:
             # Execute the code
             count = 0
-            code_to_run = code
+            code_to_run = self.remove_unsafe_imports(code)
             while count < self._max_retries:
                 try:
-                    exec(code_to_run)
+                    exec(
+                        code_to_run,
+                        {
+                            "pd": pd,
+                            "df": data_frame,
+                            "__builtins__": {
+                                "pd": pd,
+                                "df": data_frame,
+                                **{
+                                    builtin: __builtins__[builtin]
+                                    for builtin in WHITELISTED_BUILTINS
+                                },
+                            },
+                        },
+                    )
                     code = code_to_run
                     break
                 except Exception as e:  # pylint: disable=W0718 disable=C0103
                     if not use_error_correction_framework:
                         raise e
 
                     count += 1
-                    error_correcting_instruction = self._error_correct_instruction.format(
-                        today_date=date.today(),
-                        code=code,
-                        error_returned=e,
-                        START_CODE_TAG=START_CODE_TAG,
-                        END_CODE_TAG=END_CODE_TAG,
-                        question=self._original_instructions["question"],
-                        df_head=self._original_instructions["df_head"],
-                        num_rows=self._original_instructions["num_rows"],
-                        num_columns=self._original_instructions["num_columns"],
-                        rows_to_display=self._original_instructions["rows_to_display"],
+                    error_correcting_instruction = (
+                        self._error_correct_instruction.format(
+                            today_date=date.today(),
+                            code=code,
+                            error_returned=e,
+                            START_CODE_TAG=START_CODE_TAG,
+                            END_CODE_TAG=END_CODE_TAG,
+                            question=self._original_instructions["question"],
+                            df_head=self._original_instructions["df_head"],
+                            num_rows=self._original_instructions["num_rows"],
+                            num_columns=self._original_instructions["num_columns"],
+                            rows_to_display=self._original_instructions[
+                                "rows_to_display"
+                            ],
+                        )
+                    )
+                    code_to_run = self._llm.generate_code(
+                        error_correcting_instruction, ""
                     )
-                    code_to_run = self._llm.generate_code(error_correcting_instruction, "")
 
         captured_output = output.getvalue()
 
         # Evaluate the last line and return its value or the captured output
         lines = code.strip().split("\n")
         last_line = lines[-1].strip()
         if last_line.startswith("print(") and last_line.endswith(")"):
```

### Comparing `pandasai-0.2.8/pandasai/exceptions.py` & `pandasai-0.2.9/pandasai/exceptions.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.8/pandasai/helpers/anonymizer.py` & `pandasai-0.2.9/pandasai/helpers/anonymizer.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.8/pandasai/helpers/notebook.py` & `pandasai-0.2.9/pandasai/helpers/notebook.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.8/pandasai/llm/alpaca.py` & `pandasai-0.2.9/pandasai/llm/alpaca.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.8/pandasai/llm/base.py` & `pandasai-0.2.9/pandasai/llm/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 """ Base class to implement a new LLM. """
 
 import ast
 import re
 from typing import Optional
 
-import astor
-
-from ..constants import END_CODE_TAG, START_CODE_TAG, WHITELISTED_LIBRARIES
+from ..constants import END_CODE_TAG, START_CODE_TAG
 from ..exceptions import (
     APIKeyNotFoundError,
     MethodNotImplementedError,
     NoCodeFoundError,
 )
 
 
@@ -28,27 +26,14 @@
             APIKeyNotFoundError: Type has not been implemented
 
         Returns:
             str: Type of LLM a string
         """
         raise APIKeyNotFoundError("Type has not been implemented")
 
-    def _remove_imports(self, code: str) -> str:
-        tree = ast.parse(code)
-        new_body = [
-            node
-            for node in tree.body
-            if not (
-                isinstance(node, (ast.Import, ast.ImportFrom))
-                and any(alias.name in WHITELISTED_LIBRARIES for alias in node.names)
-            )
-        ]
-        new_tree = ast.Module(body=new_body)
-        return astor.to_source(new_tree).strip()
-
     def _polish_code(self, code: str) -> str:
         """
         Polish the code by removing the leading "python" or "py",  \
         removing the imports and removing trailing spaces and new lines.
 
         Args:
             code (str): Code
@@ -57,15 +42,14 @@
             str: Polished code
         """
         if re.match(r"^(python|py)", code):
             code = re.sub(r"^(python|py)", "", code)
         if re.match(r"^`.*`$", code):
             code = re.sub(r"^`(.*)`$", r"\1", code)
         code = code.strip()
-        code = self._remove_imports(code)
         return code
 
     def _is_python_code(self, string):
         try:
             ast.parse(string)
             return True
         except SyntaxError:
```

### Comparing `pandasai-0.2.8/pandasai/llm/base_hf.py` & `pandasai-0.2.9/pandasai/llm/base_hf.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.2.8/pandasai/llm/open_assistant.py` & `pandasai-0.2.9/pandasai/llm/open_assistant.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,14 @@
     _api_url: str = (
         "https://api-inference.huggingface.co/models/"
         "OpenAssistant/oasst-sft-1-pythia-12b"
     )
     _max_retries: int = 10
 
     def __init__(self, api_token: Optional[str] = None):
-        self.api_token = api_token or os.getenv("HUGGINGFACE_API_KEY")
+        self.api_token = api_token or os.getenv("HUGGINGFACE_API_KEY") or None
         if self.api_token is None:
             raise APIKeyNotFoundError("HuggingFace Hub API key is required")
 
     @property
     def type(self) -> str:
         return "open-assistant"
```

### Comparing `pandasai-0.2.8/pandasai/llm/openai.py` & `pandasai-0.2.9/pandasai/llm/openai.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     stop: Optional[str] = None
 
     def __init__(
         self,
         api_token: Optional[str] = None,
         **kwargs,
     ):
-        self.api_token = api_token or os.getenv("OPENAI_API_KEY")
+        self.api_token = api_token or os.getenv("OPENAI_API_KEY") or None
         if self.api_token is None:
             raise APIKeyNotFoundError("OpenAI API key is required")
         openai.api_key = self.api_token
 
         self._set_params(**kwargs)
 
     def _set_params(self, **kwargs):
```

### Comparing `pandasai-0.2.8/pandasai/llm/starcoder.py` & `pandasai-0.2.9/pandasai/llm/starcoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,14 @@
     """Starcoder LLM"""
 
     api_token: str
     _api_url: str = "https://api-inference.huggingface.co/models/bigcode/starcoder"
     _max_retries: int = 5
 
     def __init__(self, api_token: Optional[str] = None):
-        self.api_token = api_token or os.getenv("HUGGINGFACE_API_KEY")
+        self.api_token = api_token or os.getenv("HUGGINGFACE_API_KEY") or None
         if self.api_token is None:
             raise APIKeyNotFoundError("HuggingFace Hub API key is required")
 
     @property
     def type(self) -> str:
         return "starcoder"
```

### Comparing `pandasai-0.2.8/pyproject.toml` & `pandasai-0.2.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,40 @@
 [tool.poetry]
 name = "pandasai"
-version = "0.2.8"
+version = "0.2.9"
 description = "Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational."
 authors = ["Gabriele Venturi"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandasai"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 python-dotenv = "^1.0.0"
 pandas = "^2.0.1"
 astor = "^0.8.1"
 openai = "^0.27.5"
 ipython = "^8.13.1"
 matplotlib = "^3.7.1"
+pytest-env = "^0.8.1"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 pre-commit = "^3.2.2"
 pylint = "^2.17.3"
 pytest = "^7.3.1"
 isort = "^5.12.0"
+pytest-mock = "^3.10.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pylint]
-ignore = "tests_*"
+ignore = "tests_*"
+
+[tool.pytest.ini_options]
+env = [
+    "HUGGINGFACE_API_KEY=",
+    "OPENAI_API_KEY="
+]
```

### Comparing `pandasai-0.2.8/PKG-INFO` & `pandasai-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: pandasai
-Version: 0.2.8
+Version: 0.2.9
 Summary: Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational.
 License: MIT
 Author: Gabriele Venturi
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: astor (>=0.8.1,<0.9.0)
 Requires-Dist: ipython (>=8.13.1,<9.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: openai (>=0.27.5,<0.28.0)
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
+Requires-Dist: pytest-env (>=0.8.1,<0.9.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # PandasAI 🐼
 
 [![release](https://img.shields.io/pypi/v/pandasai?label=Release&style=flat-square)](https://pypi.org/project/pandasai/)
 [![lint](https://github.com/gventuri/pandas-ai/actions/workflows/ci.yml/badge.svg)](https://github.com/gventuri/pandas-ai/actions/workflows/ci.yml/badge.svg)
```

