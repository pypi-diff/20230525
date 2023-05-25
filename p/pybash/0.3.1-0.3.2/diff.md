# Comparing `tmp/pybash-0.3.1.tar.gz` & `tmp/pybash-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybash-0.3.1.tar", max compression
+gzip compressed data, was "pybash-0.3.2.tar", max compression
```

## Comparing `pybash-0.3.1.tar` & `pybash-0.3.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1060 2023-05-21 04:39:07.620456 pybash-0.3.1/LICENSE
--rw-r--r--   0        0        0     4057 2023-05-21 04:39:07.620456 pybash-0.3.1/README.md
--rw-r--r--   0        0        0        0 2023-05-21 04:39:07.620456 pybash-0.3.1/pybash/__init__.py
--rw-r--r--   0        0        0      684 2023-05-21 04:39:07.620456 pybash-0.3.1/pybash/__main__.py
--rw-r--r--   0        0        0      531 2023-05-21 04:39:07.620456 pybash-0.3.1/pybash/hook.py
--rw-r--r--   0        0        0    15403 2023-05-21 04:39:07.620456 pybash-0.3.1/pybash/transformer.py
--rw-r--r--   0        0        0      792 2023-05-21 04:39:07.620456 pybash-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     4601 1970-01-01 00:00:00.000000 pybash-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-05-25 01:42:43.603008 pybash-0.3.2/LICENSE
+-rw-r--r--   0        0        0     4055 2023-05-25 01:42:43.603008 pybash-0.3.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-25 01:42:43.603008 pybash-0.3.2/pybash/__init__.py
+-rw-r--r--   0        0        0      684 2023-05-25 01:42:43.603008 pybash-0.3.2/pybash/__main__.py
+-rw-r--r--   0        0        0      531 2023-05-25 01:42:43.603008 pybash-0.3.2/pybash/hook.py
+-rw-r--r--   0        0        0    15560 2023-05-25 01:42:43.603008 pybash-0.3.2/pybash/transformer.py
+-rw-r--r--   0        0        0      792 2023-05-25 01:42:43.603008 pybash-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     4599 1970-01-01 00:00:00.000000 pybash-0.3.2/PKG-INFO
```

### Comparing `pybash-0.3.1/LICENSE` & `pybash-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pybash-0.3.1/README.md` & `pybash-0.3.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,168 +1,168 @@
 # PyBash
 
 ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/jaykv/pybash/python-app.yml?branch=main)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/pybash)
 ![PyPI](https://img.shields.io/pypi/v/pybash)
 ![GitHub](https://img.shields.io/github/license/jaykv/pybash)
 
-Streamline bash-command execution from python with a new syntax. It combines the simplicity of writing bash scripts with the flexibility of python. Under the hood, any line or variable assignment starting with `>` or surrounded by parentheses is transformed to python `subprocess` calls and then injected into `sys.meta_path` as an import hook. All possible thanks to the wonderful [ideas](https://github.com/aroberge/ideas) project!
+Streamline bash-command execution from python with a new syntax. It combines the simplicity of writing bash scripts with the flexibility of python. Under the hood, any line or variable assignment starting with `$` or surrounded by parentheses is transformed to python `subprocess` calls and then injected into `sys.meta_path` as an import hook. All possible thanks to the wonderful [ideas](https://github.com/aroberge/ideas) project!
 
-For security and performance reasons, PyBash will NOT execute as shell, unless explicitly specified with a `$` instead of a single `>` before the command. While running commands as shell can be convenient, it can also spawn security risks if you're not too careful. If you're curious about the transformations, look at the [unit tests](test_pybash.py) for some quick examples.
+For security and performance reasons, PyBash will NOT execute as shell, unless explicitly specified with a `>` instead of a single `$` before the command. While running commands as shell can be convenient, it can also spawn security risks if you're not too careful. If you're curious about the transformations, look at the [unit tests](test_pybash.py) for some quick examples.
 
 Note: this is a mainly experimental library.
 
 # Setup
 
 ## As standalone transformer
 `pip install pybash`
 
 
 ```python
 from pybash.transformer import transform
 
-transform(">echo hello world") # returns the python code for the bash command as string
+transform("$echo hello world") # returns the python code for the bash command as string
 ```
 
 ## As script runner
 `pip install "pybash[script]"`
 
 
 ### Example 
 ```py
 #
 text = "HELLO WORLD"
->echo f{text}
+$echo f{text}
 ```
 
 ### Run script:
 ```bash
-$ python -m pybash hello.py
+python -m pybash hello.py
 ```
 
 # Supported transforms
 
 ### 1. Simple execution with output
 ```python
->python --version
->echo \\nthis is an echo
+$python --version
+$echo \\nthis is an echo
 ```
 outputs:
 ```
 Python 3.9.15
 
 this is an echo
 ```
 
 ### 2. Set output to variable and parse
 ```python
-out = >cat test.txt
+out = $cat test.txt
 test_data = out.decode('utf-8').strip()
 print(test_data.replace("HELLO", "HOWDY"))
 ```
 outputs:
 ```
 HOWDY WORLD
 ```
 
 ### 3. Wrapped, in-line execution and parsing
 ```python
-print((>cat test.txt).decode('utf-8').strip())
+print(($cat test.txt).decode('utf-8').strip())
 ```
 outputs:
 ```
 HELLO WORLD
 ```
 
 ### 4. Redirection
 ```python
->echo "hello" >> test4.txt
+$echo "hello" >> test4.txt
 ```
 
 ### 5. Pipe chaining
 ```python
->cat test.txt | sed 's/HELLO/HOWDY/g' | sed 's/HOW/WHY/g' | sed 's/WHY/WHEN/g'
+$cat test.txt | sed 's/HELLO/HOWDY/g' | sed 's/HOW/WHY/g' | sed 's/WHY/WHEN/g'
 ```
 outputs:
 ```
 WHENDY WORLD
 ```
 
 ### 6. Redirection chaining
 ```python
->cat test.txt | sed 's/HELLO/HOWDY\\n/g' > test1.txt >> test2.txt > test3.txt
+$cat test.txt | sed 's/HELLO/HOWDY\\n/g' > test1.txt >> test2.txt > test3.txt
 ```
 
 ### 7. Chaining pipes and redirection- works in tandem!
 ```python
->cat test.txt | sed 's/HELLO/HOWDY\\n/g' > test5.txt
+$cat test.txt | sed 's/HELLO/HOWDY\\n/g' > test5.txt
 ```
 
 ### 8. Input redirection
 ```python
->sort < test.txt >> sorted_test.txt
+$sort < test.txt >> sorted_test.txt
 ```
 
 ```python
->sort < test.txt | sed 's/SORT/TEST\\n/g'
+$sort < test.txt | sed 's/SORT/TEST\\n/g'
 ```
 ### 9. Glob patterns with shell
 ```python
-$ls .github/*
+>ls .github/*
 ```
 
 ### 10. Direct interpolation
 Denoted by {{code here}}. Interpolated as direct code replace. The value/output of the variable, function call, or the expression must not include spaces.
 
 ```python
 ## GOOD
 command = "status"
 def get_option(command):
     return "-s" if command == "status" else "-v"
->git {{command}} {{get_option(command)}}
+$git {{command}} {{get_option(command)}}
 
 display_type = "labels"
->kubectl get pods --show-{{display_type}}=true
+$kubectl get pods --show-{{display_type}}=true
 
 ## BAD
 option = "-s -v"
->git status {{option}}
+$git status {{option}}
 
 options = ['-s', '-v']
->git status {{" ".join(options)}}
+$git status {{" ".join(options)}}
 
 # use dynamic interpolation
 options = {'version': '-v'}
->git status {{options['version']}}
+$git status {{options['version']}}
 ```
 
 ### 11. f-string interpolation
 Denoted by f{ any python variable, function call, or expression here }. Interpolated as f-string. The output of the variable, function call, or the expression must still not include spaces.
 
 ```python
 ## GOOD
 
 # git -h
 options = {'version': '-v', 'help': '-h'}
->git f{options['h']}
+$git f{options['h']}
 
 # kubectl get pods --show-labels -n coffee
 namespace = "coffee"
->kubectl get pods f{"--" + "-".join(['show', 'labels'])} -n f{namespace}
+$kubectl get pods f{"--" + "-".join(['show', 'labels'])} -n f{namespace}
 
 ## BAD
 option = "-s -v"
->git status f{option}
+$git status f{option}
 ```
 
 #### Also works inside methods!
 ```python
 # PYBASH DEMO #
 def cp_test():
-    >cp test.txt test_copy.txt
+    $cp test.txt test_copy.txt
 
 cp_test()
 ```
 
 # Dev
 
 #### Demo
```

### Comparing `pybash-0.3.1/pybash/__main__.py` & `pybash-0.3.2/pybash/__main__.py`

 * *Files identical despite different names*

### Comparing `pybash-0.3.1/pybash/hook.py` & `pybash-0.3.2/pybash/hook.py`

 * *Files identical despite different names*

### Comparing `pybash-0.3.1/pybash/transformer.py` & `pybash-0.3.2/pybash/transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 class InvalidInterpolation(Exception):
     pass
 
 
 class Processor:
-    command_char = ">"
+    command_char = "$"
 
     def __init__(self, token: token_utils.Token) -> None:
         self.token = token
         self.token_line = token.line
         self.parse()
 
     def parse(self) -> None:
@@ -74,15 +74,15 @@
             raise InvalidInterpolation
 
         return re.sub(r'{{(.+?)}}', r'" + \1 + "', string)
 
 
 class Shelled(Processor):
     # $ls .github/*
-    command_char = "$"
+    command_char = ">"
 
     def transform(self) -> token_utils.Token:
         command_str = " ".join(self.command)
         self.token.string = Commander.build_subprocess_str_cmd("run", command_str, shell=True) + '\n'
         return self.token
 
 
@@ -103,20 +103,21 @@
     def parse(self) -> None:
         self.parsed_line = shlex.split(self.token.line)
         self.start_index = Commander.get_start_index(self.parsed_line)
         self.command = Commander.get_bash_command(self.parsed_line, start_index=self.start_index)
 
     def transform(self) -> None:
         pipeline_command = Pipeline(self.command).parse_command(variablized=True)
+
         if pipeline_command != self.command:
             self.token.string = pipeline_command
             self.token.string += ';' if pipeline_command[-1] != ';' else ''
             self.token.string += ' '.join(self.parsed_line[: self.start_index]) + ' cmd1\n'
         else:
-            self.token.string = ' '.join(self.parsed_line[: self.start_index])
+            self.token.string = ' '.join(self.parsed_line[: self.start_index]) + ' '
             self.token.string += Commander.build_subprocess_list_cmd("check_output", self.command) + '\n'
 
 
 class Wrapped(Processor):
     # print(>cat test.txt)
     def parse(self) -> None:
         self.parsed_line = shlex.split(self.token.line)
@@ -124,15 +125,15 @@
         self.start_index = Commander.get_start_index(self.parsed_line)
         self.command = Commander.get_bash_command(self.parsed_line, start_index=self.start_index, wrapped=True)
 
     def transform(self) -> token_utils.Token:
         # shlex strips out single quotes and double quotes-- use raw_line for the code around the wrapped command
         self.token.string = (
             ' '.join(self.raw_line[: self.start_index])
-            + self.raw_line[self.start_index][: self.raw_line[self.start_index].index('>')]
+            + self.raw_line[self.start_index][: self.raw_line[self.start_index].index('$')]
         )
         self.token.string += (
             Commander.build_subprocess_list_cmd("check_output", self.command)
             + self.raw_line[-1][self.raw_line[-1].index(')') :]
             + '\n'
         )
 
@@ -325,25 +326,25 @@
         Args:
             parsed_line (list): line to parse
 
         Returns:
             int: starting index
         """
         for i, val in enumerate(parsed_line):
-            if '>' in val:
+            if '$' in val:
                 return i
 
         return 0
 
     @staticmethod
     def get_bash_command(
         parsed_line: list,
         start_index: Union[int, None] = None,
         wrapped: Union[bool, None] = None,
-        command_char: str = ">",
+        command_char: str = "$",
     ) -> list:
         """Parses line to bash command
 
         Args:
             parsed_line (list): line to parse
             start_index (int, optional): index to start parsing command from. Defaults to None.
             wrapped (bool, optional): input is surrounded by parentheses
@@ -357,14 +358,16 @@
 
         # strip everything before that index-- not part of the command
         command = parsed_line[start_index:]
 
         # > may be at the beginning or somewhere in the middle of this arg
         # examples: >ls, print(>cat => strip up to and including >
         command[0] = command[0][command[0].index(command_char) + 1 :].strip()
+        if command[0] == '':
+            del command[0]
 
         # remove everything after and including first )- not part of the command
         if wrapped:
             if ')' not in command[-1]:
                 raise SyntaxError("Missing end parentheses")
 
             command[-1] = command[-1][: command[-1].index(')')]
@@ -408,16 +411,16 @@
         if kwargs:
             for k, v in kwargs.items():
                 command += f", {k}={v}"
         command += ")"
         return command
 
 
-TOKENIZERS = {"$": Shelled, ">": Execed}
-GREEDY_TOKENIZERS = {"= >": Variablized, "(>": Wrapped}
+TOKENIZERS = {">": Shelled, "$": Execed}
+GREEDY_TOKENIZERS = {"= $": Variablized, "($": Wrapped}
 
 
 def transform(source, **_kwargs):
     """Convert >bash commands to subprocess calls"""
     new_tokens = []
     for line in token_utils.get_lines(source):
         token = token_utils.get_first(line)
@@ -439,7 +442,12 @@
             new_tokens.append(parser.token)
             continue
 
         # no match
         new_tokens.extend(line)
 
     return token_utils.untokenize(new_tokens)
+
+
+if __name__ == "__main__":
+    pyscript = transform("test = $ echo hi")
+    print(pyscript)
```

### Comparing `pybash-0.3.1/pyproject.toml` & `pybash-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PyBash"
-version = "0.3.1"
+version = "0.3.2"
 description = ">execute bash commands from python easily"
 authors = ["Jay <jay.github0@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pybash"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `pybash-0.3.1/PKG-INFO` & `pybash-0.3.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybash
-Version: 0.3.1
+Version: 0.3.2
 Summary: >execute bash commands from python easily
 Author: Jay
 Author-email: jay.github0@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -17,168 +17,168 @@
 # PyBash
 
 ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/jaykv/pybash/python-app.yml?branch=main)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/pybash)
 ![PyPI](https://img.shields.io/pypi/v/pybash)
 ![GitHub](https://img.shields.io/github/license/jaykv/pybash)
 
-Streamline bash-command execution from python with a new syntax. It combines the simplicity of writing bash scripts with the flexibility of python. Under the hood, any line or variable assignment starting with `>` or surrounded by parentheses is transformed to python `subprocess` calls and then injected into `sys.meta_path` as an import hook. All possible thanks to the wonderful [ideas](https://github.com/aroberge/ideas) project!
+Streamline bash-command execution from python with a new syntax. It combines the simplicity of writing bash scripts with the flexibility of python. Under the hood, any line or variable assignment starting with `$` or surrounded by parentheses is transformed to python `subprocess` calls and then injected into `sys.meta_path` as an import hook. All possible thanks to the wonderful [ideas](https://github.com/aroberge/ideas) project!
 
-For security and performance reasons, PyBash will NOT execute as shell, unless explicitly specified with a `$` instead of a single `>` before the command. While running commands as shell can be convenient, it can also spawn security risks if you're not too careful. If you're curious about the transformations, look at the [unit tests](test_pybash.py) for some quick examples.
+For security and performance reasons, PyBash will NOT execute as shell, unless explicitly specified with a `>` instead of a single `$` before the command. While running commands as shell can be convenient, it can also spawn security risks if you're not too careful. If you're curious about the transformations, look at the [unit tests](test_pybash.py) for some quick examples.
 
 Note: this is a mainly experimental library.
 
 # Setup
 
 ## As standalone transformer
 `pip install pybash`
 
 
 ```python
 from pybash.transformer import transform
 
-transform(">echo hello world") # returns the python code for the bash command as string
+transform("$echo hello world") # returns the python code for the bash command as string
 ```
 
 ## As script runner
 `pip install "pybash[script]"`
 
 
 ### Example 
 ```py
 #
 text = "HELLO WORLD"
->echo f{text}
+$echo f{text}
 ```
 
 ### Run script:
 ```bash
-$ python -m pybash hello.py
+python -m pybash hello.py
 ```
 
 # Supported transforms
 
 ### 1. Simple execution with output
 ```python
->python --version
->echo \\nthis is an echo
+$python --version
+$echo \\nthis is an echo
 ```
 outputs:
 ```
 Python 3.9.15
 
 this is an echo
 ```
 
 ### 2. Set output to variable and parse
 ```python
-out = >cat test.txt
+out = $cat test.txt
 test_data = out.decode('utf-8').strip()
 print(test_data.replace("HELLO", "HOWDY"))
 ```
 outputs:
 ```
 HOWDY WORLD
 ```
 
 ### 3. Wrapped, in-line execution and parsing
 ```python
-print((>cat test.txt).decode('utf-8').strip())
+print(($cat test.txt).decode('utf-8').strip())
 ```
 outputs:
 ```
 HELLO WORLD
 ```
 
 ### 4. Redirection
 ```python
->echo "hello" >> test4.txt
+$echo "hello" >> test4.txt
 ```
 
 ### 5. Pipe chaining
 ```python
->cat test.txt | sed 's/HELLO/HOWDY/g' | sed 's/HOW/WHY/g' | sed 's/WHY/WHEN/g'
+$cat test.txt | sed 's/HELLO/HOWDY/g' | sed 's/HOW/WHY/g' | sed 's/WHY/WHEN/g'
 ```
 outputs:
 ```
 WHENDY WORLD
 ```
 
 ### 6. Redirection chaining
 ```python
->cat test.txt | sed 's/HELLO/HOWDY\\n/g' > test1.txt >> test2.txt > test3.txt
+$cat test.txt | sed 's/HELLO/HOWDY\\n/g' > test1.txt >> test2.txt > test3.txt
 ```
 
 ### 7. Chaining pipes and redirection- works in tandem!
 ```python
->cat test.txt | sed 's/HELLO/HOWDY\\n/g' > test5.txt
+$cat test.txt | sed 's/HELLO/HOWDY\\n/g' > test5.txt
 ```
 
 ### 8. Input redirection
 ```python
->sort < test.txt >> sorted_test.txt
+$sort < test.txt >> sorted_test.txt
 ```
 
 ```python
->sort < test.txt | sed 's/SORT/TEST\\n/g'
+$sort < test.txt | sed 's/SORT/TEST\\n/g'
 ```
 ### 9. Glob patterns with shell
 ```python
-$ls .github/*
+>ls .github/*
 ```
 
 ### 10. Direct interpolation
 Denoted by {{code here}}. Interpolated as direct code replace. The value/output of the variable, function call, or the expression must not include spaces.
 
 ```python
 ## GOOD
 command = "status"
 def get_option(command):
     return "-s" if command == "status" else "-v"
->git {{command}} {{get_option(command)}}
+$git {{command}} {{get_option(command)}}
 
 display_type = "labels"
->kubectl get pods --show-{{display_type}}=true
+$kubectl get pods --show-{{display_type}}=true
 
 ## BAD
 option = "-s -v"
->git status {{option}}
+$git status {{option}}
 
 options = ['-s', '-v']
->git status {{" ".join(options)}}
+$git status {{" ".join(options)}}
 
 # use dynamic interpolation
 options = {'version': '-v'}
->git status {{options['version']}}
+$git status {{options['version']}}
 ```
 
 ### 11. f-string interpolation
 Denoted by f{ any python variable, function call, or expression here }. Interpolated as f-string. The output of the variable, function call, or the expression must still not include spaces.
 
 ```python
 ## GOOD
 
 # git -h
 options = {'version': '-v', 'help': '-h'}
->git f{options['h']}
+$git f{options['h']}
 
 # kubectl get pods --show-labels -n coffee
 namespace = "coffee"
->kubectl get pods f{"--" + "-".join(['show', 'labels'])} -n f{namespace}
+$kubectl get pods f{"--" + "-".join(['show', 'labels'])} -n f{namespace}
 
 ## BAD
 option = "-s -v"
->git status f{option}
+$git status f{option}
 ```
 
 #### Also works inside methods!
 ```python
 # PYBASH DEMO #
 def cp_test():
-    >cp test.txt test_copy.txt
+    $cp test.txt test_copy.txt
 
 cp_test()
 ```
 
 # Dev
 
 #### Demo
```

