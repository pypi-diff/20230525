# Comparing `tmp/pymaidol-0.1.1.tar.gz` & `tmp/pymaidol-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymaidol-0.1.1.tar", last modified: Tue May 23 13:12:13 2023, max compression
+gzip compressed data, was "pymaidol-0.1.2.tar", last modified: Thu May 25 05:41:11 2023, max compression
```

## Comparing `pymaidol-0.1.1.tar` & `pymaidol-0.1.2.tar`

### file list

```diff
@@ -1,49 +1,62 @@
-drwxrwxr-x   0 eterance  (1000) eterance  (1000)        0 2023-05-23 13:12:13.746555 pymaidol-0.1.1/
--rw-rw-r--   0 eterance  (1000) eterance  (1000)     2028 2023-05-23 13:11:17.000000 pymaidol-0.1.1/.gitignore
--rw-rw-r--   0 eterance  (1000) eterance  (1000)     1080 2023-05-23 13:11:17.000000 pymaidol-0.1.1/LICENSE
--rw-rw-r--   0 eterance  (1000) eterance  (1000)     3032 2023-05-23 13:12:13.746555 pymaidol-0.1.1/PKG-INFO
--rw-rw-r--   0 eterance  (1000) eterance  (1000)     2628 2023-05-23 13:11:17.000000 pymaidol-0.1.1/README.md
-drwxrwxr-x   0 eterance  (1000) eterance  (1000)        0 2023-05-23 13:12:13.742555 pymaidol-0.1.1/docs/
-drwxrwxr-x   0 eterance  (1000) eterance  (1000)        0 2023-05-23 13:12:13.742555 pymaidol-0.1.1/docs/zh-cn/
--rw-rw-r--   0 eterance  (1000) eterance  (1000)     2957 2023-05-23 13:11:17.000000 pymaidol-0.1.1/docs/zh-cn/语法参考.md
-drwxrwxr-x   0 eterance  (1000) eterance  (1000)        0 2023-05-23 13:12:13.742555 pymaidol-0.1.1/examples/
-drwxrwxr-x   0 eterance  (1000) eterance  (1000)        0 2023-05-23 13:12:13.742555 pymaidol-0.1.1/examples/first_template/
--rw-rw-r--   0 eterance  (1000) eterance  (1000)      473 2023-05-23 13:11:17.000000 pymaidol-0.1.1/examples/first_template/FirstTemplate.py
--rw-rw-r--   0 eterance  (1000) eterance  (1000)       79 2023-05-23 13:11:17.000000 pymaidol-0.1.1/examples/first_template/FirstTemplate.pymd
-drwxrwxr-x   0 eterance  (1000) eterance  (1000)        0 2023-05-23 13:12:13.742555 pymaidol-0.1.1/pymaidol/
--rw-rw-r--   0 eterance  (1000) eterance  (1000)      662 2023-05-23 13:11:17.000000 pymaidol-0.1.1/pymaidol/AnnotationTypeEnum.py
--rw-rw-r--   0 eterance  (1000) eterance  (1000)     3587 2023-05-23 13:11:17.000000 pymaidol-0.1.1/pymaidol/Errors.py
--rw-rw-r--   0 eterance  (1000) eterance  (1000)     5719 2023-05-23 13:11:17.000000 pymaidol-0.1.1/pymaidol/Executor.py
--rw-rw-r--   0 eterance  (1000) eterance  (1000)     3861 2023-05-23 13:11:17.000000 pymaidol-0.1.1/pymaidol/Nodes.py
--rw-rw-r--   0 eterance  (1000) eterance  (1000)    26610 2023-05-23 13:11:17.000000 pymaidol-0.1.1/pymaidol/Parser.py
--rw-rw-r--   0 eterance  (1000) eterance  (1000)      929 2023-05-23 13:11:17.000000 pymaidol-0.1.1/pymaidol/Positions.py
--rw-rw-r--   0 eterance  (1000) eterance  (1000)     3954 2023-05-23 13:11:17.000000 pymaidol-0.1.1/pymaidol/SyntaxChecker.py
--rw-rw-r--   0 eterance  (1000) eterance  (1000)     2737 2023-05-23 13:11:17.000000 pymaidol-0.1.1/pymaidol/TemplateBase.py
--rw-rw-r--   0 eterance  (1000) eterance  (1000)     7475 2023-05-23 13:11:17.000000 pymaidol-0.1.1/pymaidol/Traversers.py
--rw-rw-r--   0 eterance  (1000) eterance  (1000)        0 2023-05-23 13:11:17.000000 pymaidol-0.1.1/pymaidol/__init__.py
--rw-rw-r--   0 eterance  (1000) eterance  (1000)     1276 2023-05-23 13:11:17.000000 pymaidol-0.1.1/pymaidol/__main__.py
-drwxrwxr-x   0 eterance  (1000) eterance  (1000)        0 2023-05-23 13:12:13.746555 pymaidol-0.1.1/pymaidol/code_templates/
--rw-rw-r--   0 eterance  (1000) eterance  (1000)      294 2023-05-23 13:11:17.000000 pymaidol-0.1.1/pymaidol/code_templates/SubClassTemplate.py
--rw-rw-r--   0 eterance  (1000) eterance  (1000)      242 2023-05-23 13:11:17.000000 pymaidol-0.1.1/pymaidol/code_templates/SubClassTemplate.pymd
--rw-rw-r--   0 eterance  (1000) eterance  (1000)        0 2023-05-23 13:11:17.000000 pymaidol-0.1.1/pymaidol/code_templates/__init__.py
--rw-rw-r--   0 eterance  (1000) eterance  (1000)     1209 2023-05-23 13:11:17.000000 pymaidol-0.1.1/pymaidol/keywords.py
-drwxrwxr-x   0 eterance  (1000) eterance  (1000)        0 2023-05-23 13:12:13.746555 pymaidol-0.1.1/pymaidol.egg-info/
--rw-rw-r--   0 eterance  (1000) eterance  (1000)     3032 2023-05-23 13:12:13.000000 pymaidol-0.1.1/pymaidol.egg-info/PKG-INFO
--rw-rw-r--   0 eterance  (1000) eterance  (1000)     1086 2023-05-23 13:12:13.000000 pymaidol-0.1.1/pymaidol.egg-info/SOURCES.txt
--rw-rw-r--   0 eterance  (1000) eterance  (1000)        1 2023-05-23 13:12:13.000000 pymaidol-0.1.1/pymaidol.egg-info/dependency_links.txt
--rw-rw-r--   0 eterance  (1000) eterance  (1000)       22 2023-05-23 13:12:13.000000 pymaidol-0.1.1/pymaidol.egg-info/requires.txt
--rw-rw-r--   0 eterance  (1000) eterance  (1000)        9 2023-05-23 13:12:13.000000 pymaidol-0.1.1/pymaidol.egg-info/top_level.txt
--rw-rw-r--   0 eterance  (1000) eterance  (1000)      557 2023-05-23 13:11:44.000000 pymaidol-0.1.1/pyproject.toml
--rw-rw-r--   0 eterance  (1000) eterance  (1000)       38 2023-05-23 13:12:13.746555 pymaidol-0.1.1/setup.cfg
-drwxrwxr-x   0 eterance  (1000) eterance  (1000)        0 2023-05-23 13:12:13.746555 pymaidol-0.1.1/tests/
-drwxrwxr-x   0 eterance  (1000) eterance  (1000)        0 2023-05-23 13:12:13.746555 pymaidol-0.1.1/tests/harder_demo/
--rw-rw-r--   0 eterance  (1000) eterance  (1000)      367 2023-05-23 13:11:17.000000 pymaidol-0.1.1/tests/harder_demo/CodeLangTemplate.py
--rw-rw-r--   0 eterance  (1000) eterance  (1000)      892 2023-05-23 13:11:17.000000 pymaidol-0.1.1/tests/harder_demo/CodeLangTemplate.pymd
--rw-rw-r--   0 eterance  (1000) eterance  (1000)      472 2023-05-23 13:11:17.000000 pymaidol-0.1.1/tests/harder_demo/codelang.json
--rw-rw-r--   0 eterance  (1000) eterance  (1000)    83313 2023-05-23 13:11:17.000000 pymaidol-0.1.1/tests/harder_demo/sparc_dev_[389, 19, 141, 329, 344, 126, 59, 46, 199, 147].json
--rw-rw-r--   0 eterance  (1000) eterance  (1000)     1274 2023-05-23 13:11:17.000000 pymaidol-0.1.1/tests/harder_demo/sparc_sub_dataset.pml
--rw-rw-r--   0 eterance  (1000) eterance  (1000)      198 2023-05-23 13:11:17.000000 pymaidol-0.1.1/tests/harder_demo/sparc_sub_dataset.py
--rw-rw-r--   0 eterance  (1000) eterance  (1000)      718 2023-05-23 13:11:17.000000 pymaidol-0.1.1/tests/harder_demo/sparc_sub_dataset_pml.py
--rw-rw-r--   0 eterance  (1000) eterance  (1000)      234 2023-05-23 13:11:17.000000 pymaidol-0.1.1/tests/test_class.py
--rw-rw-r--   0 eterance  (1000) eterance  (1000)        0 2023-05-23 13:11:17.000000 pymaidol-0.1.1/tests/test_class.pymd
--rw-rw-r--   0 eterance  (1000) eterance  (1000)     1192 2023-05-23 13:11:17.000000 pymaidol-0.1.1/tests/test_everything.py
+drwxrwxr-x   0 eterance  (1000) eterance  (1000)        0 2023-05-25 05:41:11.719943 pymaidol-0.1.2/
+-rw-rw-r--   0 eterance  (1000) eterance  (1000)     2028 2023-05-23 13:11:17.000000 pymaidol-0.1.2/.gitignore
+-rw-rw-r--   0 eterance  (1000) eterance  (1000)     1080 2023-05-23 13:11:17.000000 pymaidol-0.1.2/LICENSE
+-rw-rw-r--   0 eterance  (1000) eterance  (1000)     3309 2023-05-25 05:41:11.719943 pymaidol-0.1.2/PKG-INFO
+-rw-rw-r--   0 eterance  (1000) eterance  (1000)     2905 2023-05-25 05:40:12.000000 pymaidol-0.1.2/README.md
+drwxrwxr-x   0 eterance  (1000) eterance  (1000)        0 2023-05-25 05:41:11.707943 pymaidol-0.1.2/docs/
+drwxrwxr-x   0 eterance  (1000) eterance  (1000)        0 2023-05-25 05:41:11.711943 pymaidol-0.1.2/docs/zh-cn/
+drwxrwxr-x   0 eterance  (1000) eterance  (1000)        0 2023-05-25 05:41:11.711943 pymaidol-0.1.2/docs/zh-cn/AnnotationType/
+-rw-rw-r--   0 eterance  (1000) eterance  (1000)      379 2023-05-25 05:40:12.000000 pymaidol-0.1.2/docs/zh-cn/AnnotationType/AnnotationTypeEnum枚举.md
+-rw-rw-r--   0 eterance  (1000) eterance  (1000)      907 2023-05-25 05:40:12.000000 pymaidol-0.1.2/docs/zh-cn/AnnotationType/AnnotationType模块.md
+-rw-rw-r--   0 eterance  (1000) eterance  (1000)      731 2023-05-25 05:40:12.000000 pymaidol-0.1.2/docs/zh-cn/AnnotationType/MultiLineAnnotationTypeEnum枚举.md
+-rw-rw-r--   0 eterance  (1000) eterance  (1000)      692 2023-05-25 05:40:12.000000 pymaidol-0.1.2/docs/zh-cn/AnnotationType/SingleLineAnnotationTypeEnum枚举.md
+-rw-rw-r--   0 eterance  (1000) eterance  (1000)     1469 2023-05-25 05:40:12.000000 pymaidol-0.1.2/docs/zh-cn/Position类.md
+-rw-rw-r--   0 eterance  (1000) eterance  (1000)      530 2023-05-25 05:40:12.000000 pymaidol-0.1.2/docs/zh-cn/Pymaidol_API目录.md
+-rw-rw-r--   0 eterance  (1000) eterance  (1000)     2080 2023-05-25 05:40:12.000000 pymaidol-0.1.2/docs/zh-cn/TemplateBase类.md
+-rw-rw-r--   0 eterance  (1000) eterance  (1000)     1359 2023-05-25 05:40:12.000000 pymaidol-0.1.2/docs/zh-cn/TemplateRenderer类.md
+-rw-rw-r--   0 eterance  (1000) eterance  (1000)     2957 2023-05-23 13:11:17.000000 pymaidol-0.1.2/docs/zh-cn/语法参考.md
+drwxrwxr-x   0 eterance  (1000) eterance  (1000)        0 2023-05-25 05:41:11.711943 pymaidol-0.1.2/examples/
+drwxrwxr-x   0 eterance  (1000) eterance  (1000)        0 2023-05-25 05:41:11.711943 pymaidol-0.1.2/examples/first_template/
+-rw-rw-r--   0 eterance  (1000) eterance  (1000)      714 2023-05-25 05:40:12.000000 pymaidol-0.1.2/examples/first_template/FirstTemplate.py
+-rw-rw-r--   0 eterance  (1000) eterance  (1000)       79 2023-05-23 13:11:17.000000 pymaidol-0.1.2/examples/first_template/FirstTemplate.pymd
+drwxrwxr-x   0 eterance  (1000) eterance  (1000)        0 2023-05-25 05:41:11.711943 pymaidol-0.1.2/examples/template_renderer/
+-rw-rw-r--   0 eterance  (1000) eterance  (1000)      705 2023-05-25 05:40:12.000000 pymaidol-0.1.2/examples/template_renderer/renderer_demo.py
+-rw-rw-r--   0 eterance  (1000) eterance  (1000)      118 2023-05-25 05:40:12.000000 pymaidol-0.1.2/examples/template_renderer/template.pymd
+drwxrwxr-x   0 eterance  (1000) eterance  (1000)        0 2023-05-25 05:41:11.715943 pymaidol-0.1.2/pymaidol/
+-rw-rw-r--   0 eterance  (1000) eterance  (1000)      663 2023-05-24 08:09:41.000000 pymaidol-0.1.2/pymaidol/AnnotationType.py
+-rw-rw-r--   0 eterance  (1000) eterance  (1000)     3598 2023-05-25 05:40:12.000000 pymaidol-0.1.2/pymaidol/Errors.py
+-rw-rw-r--   0 eterance  (1000) eterance  (1000)     5719 2023-05-23 13:11:17.000000 pymaidol-0.1.2/pymaidol/Executor.py
+-rw-rw-r--   0 eterance  (1000) eterance  (1000)     3857 2023-05-24 08:09:41.000000 pymaidol-0.1.2/pymaidol/Nodes.py
+-rw-rw-r--   0 eterance  (1000) eterance  (1000)    26701 2023-05-24 08:09:41.000000 pymaidol-0.1.2/pymaidol/Parser.py
+-rw-rw-r--   0 eterance  (1000) eterance  (1000)      930 2023-05-25 05:40:12.000000 pymaidol-0.1.2/pymaidol/Positions.py
+-rw-rw-r--   0 eterance  (1000) eterance  (1000)     3954 2023-05-23 13:11:17.000000 pymaidol-0.1.2/pymaidol/SyntaxChecker.py
+-rw-rw-r--   0 eterance  (1000) eterance  (1000)     2794 2023-05-25 05:40:12.000000 pymaidol-0.1.2/pymaidol/TemplateBase.py
+-rw-rw-r--   0 eterance  (1000) eterance  (1000)     1649 2023-05-25 05:40:12.000000 pymaidol-0.1.2/pymaidol/TemplateRenderer.py
+-rw-rw-r--   0 eterance  (1000) eterance  (1000)     7475 2023-05-23 13:11:17.000000 pymaidol-0.1.2/pymaidol/Traversers.py
+-rw-rw-r--   0 eterance  (1000) eterance  (1000)      436 2023-05-25 05:40:12.000000 pymaidol-0.1.2/pymaidol/__init__.py
+-rw-rw-r--   0 eterance  (1000) eterance  (1000)     1365 2023-05-24 08:16:01.000000 pymaidol-0.1.2/pymaidol/__main__.py
+drwxrwxr-x   0 eterance  (1000) eterance  (1000)        0 2023-05-25 05:41:11.715943 pymaidol-0.1.2/pymaidol/code_templates/
+-rw-rw-r--   0 eterance  (1000) eterance  (1000)      548 2023-05-24 08:09:41.000000 pymaidol-0.1.2/pymaidol/code_templates/SubClassTemplate.py
+-rw-rw-r--   0 eterance  (1000) eterance  (1000)      478 2023-05-24 08:09:41.000000 pymaidol-0.1.2/pymaidol/code_templates/SubClassTemplate.pymd
+-rw-rw-r--   0 eterance  (1000) eterance  (1000)        0 2023-05-23 13:11:17.000000 pymaidol-0.1.2/pymaidol/code_templates/__init__.py
+-rw-rw-r--   0 eterance  (1000) eterance  (1000)     1209 2023-05-23 13:11:17.000000 pymaidol-0.1.2/pymaidol/keywords.py
+drwxrwxr-x   0 eterance  (1000) eterance  (1000)        0 2023-05-25 05:41:11.715943 pymaidol-0.1.2/pymaidol.egg-info/
+-rw-rw-r--   0 eterance  (1000) eterance  (1000)     3309 2023-05-25 05:41:11.000000 pymaidol-0.1.2/pymaidol.egg-info/PKG-INFO
+-rw-rw-r--   0 eterance  (1000) eterance  (1000)     1550 2023-05-25 05:41:11.000000 pymaidol-0.1.2/pymaidol.egg-info/SOURCES.txt
+-rw-rw-r--   0 eterance  (1000) eterance  (1000)        1 2023-05-25 05:41:11.000000 pymaidol-0.1.2/pymaidol.egg-info/dependency_links.txt
+-rw-rw-r--   0 eterance  (1000) eterance  (1000)       22 2023-05-25 05:41:11.000000 pymaidol-0.1.2/pymaidol.egg-info/requires.txt
+-rw-rw-r--   0 eterance  (1000) eterance  (1000)        9 2023-05-25 05:41:11.000000 pymaidol-0.1.2/pymaidol.egg-info/top_level.txt
+-rw-rw-r--   0 eterance  (1000) eterance  (1000)      557 2023-05-24 07:32:43.000000 pymaidol-0.1.2/pyproject.toml
+-rw-rw-r--   0 eterance  (1000) eterance  (1000)       38 2023-05-25 05:41:11.719943 pymaidol-0.1.2/setup.cfg
+drwxrwxr-x   0 eterance  (1000) eterance  (1000)        0 2023-05-25 05:41:11.715943 pymaidol-0.1.2/tests/
+drwxrwxr-x   0 eterance  (1000) eterance  (1000)        0 2023-05-25 05:41:11.719943 pymaidol-0.1.2/tests/harder_demo/
+-rw-rw-r--   0 eterance  (1000) eterance  (1000)      367 2023-05-23 13:11:17.000000 pymaidol-0.1.2/tests/harder_demo/CodeLangTemplate.py
+-rw-rw-r--   0 eterance  (1000) eterance  (1000)      892 2023-05-23 13:11:17.000000 pymaidol-0.1.2/tests/harder_demo/CodeLangTemplate.pymd
+-rw-rw-r--   0 eterance  (1000) eterance  (1000)      472 2023-05-23 13:11:17.000000 pymaidol-0.1.2/tests/harder_demo/codelang.json
+-rw-rw-r--   0 eterance  (1000) eterance  (1000)    83313 2023-05-23 13:11:17.000000 pymaidol-0.1.2/tests/harder_demo/sparc_dev_[389, 19, 141, 329, 344, 126, 59, 46, 199, 147].json
+-rw-rw-r--   0 eterance  (1000) eterance  (1000)     1274 2023-05-23 13:11:17.000000 pymaidol-0.1.2/tests/harder_demo/sparc_sub_dataset.pml
+-rw-rw-r--   0 eterance  (1000) eterance  (1000)      198 2023-05-23 13:11:17.000000 pymaidol-0.1.2/tests/harder_demo/sparc_sub_dataset.py
+-rw-rw-r--   0 eterance  (1000) eterance  (1000)      718 2023-05-23 13:11:17.000000 pymaidol-0.1.2/tests/harder_demo/sparc_sub_dataset_pml.py
+-rw-rw-r--   0 eterance  (1000) eterance  (1000)      234 2023-05-23 13:11:17.000000 pymaidol-0.1.2/tests/test_class.py
+-rw-rw-r--   0 eterance  (1000) eterance  (1000)        0 2023-05-23 13:11:17.000000 pymaidol-0.1.2/tests/test_class.pymd
+-rw-rw-r--   0 eterance  (1000) eterance  (1000)     1188 2023-05-25 05:40:12.000000 pymaidol-0.1.2/tests/test_everything.py
```

### Comparing `pymaidol-0.1.1/.gitignore` & `pymaidol-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pymaidol-0.1.1/LICENSE` & `pymaidol-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pymaidol-0.1.1/PKG-INFO` & `pymaidol-0.1.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: pymaidol
-Version: 0.1.1
-Summary: A markup gramma that embed python code into text
-Author: Eterance
-Keywords: Prompt,Markup Language,NLP,AI,GPT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Pymaidol
 
 Pymaidol 是一种标记语法，用于将 Python 代码嵌入文本中，使得文本在运行时可动态更改包含的内容。
 
 与 [ProMaid](https://github.com/Eterance/ProMaid) 相比，Pymaidol 不只是单纯的将数据嵌入至模板（Template）的对应位置，还能将复杂的处理逻辑呈现在模板中，甚至可使用在模板中定义的函数对数据进行处理。
 
 ⚠**警告：Pymaidol 目前处于开发阶段，语法和一些对空白符、换行符的处理逻辑尚未确定，以后可能会被修改。强烈不建议在生产环境中使用。**
@@ -47,19 +34,24 @@
 ```
 
 ### 编写模板设计文件
 
 首先，用以下代码将 `FirstTemplate.pymd` 中的全部内容替换掉：
 
 ``` python
-from pymaidol.TemplateBase import TemplateBase
+from pymaidol import TemplateBase
+from pymaidol.AnnotationType import FULL_ANNOTATION_TYPE, AnnotationTypeEnum
 
 class FirstTemplate(TemplateBase):
-    def __init__(self, package_name:str, template: str | None = None, template_file_path: str | None = None) -> None:
-        super().__init__(template, template_file_path)
+    def __init__(self, 
+                 package_name:str, 
+                 template: str | None = None, 
+                 template_file_path: str | None = None, 
+                 supported_annotation_types: list[AnnotationTypeEnum] = FULL_ANNOTATION_TYPE) -> None:
+        super().__init__(template, template_file_path, supported_annotation_types)
         self.package_name = package_name
         
 def main():
     template = FirstTemplate("Pymaidol")
     string = template.Render({"says": "Hello World"})
     print(string)
     
@@ -82,10 +74,11 @@
 
 运行 `FirstTemplate.py`，命令行会输出以下内容：
 
 ``` bash
 Now (Tue May 23 19:21:19 2023), Say "Hello World" using Pymaidol!
 ```
 
-## 语法参考
+## 另请参阅
 
-请参阅 [Pymaidol 语法参考](docs/zh-cn//%E8%AF%AD%E6%B3%95%E5%8F%82%E8%80%83.md)
+- [Pymaidol 语法参考](docs/zh-cn/语法参考.md)
+- [Pymaidol_API目录](docs/zh-cn/Pymaidol_API%E7%9B%AE%E5%BD%95.md)
```

### Comparing `pymaidol-0.1.1/README.md` & `pymaidol-0.1.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: pymaidol
+Version: 0.1.2
+Summary: A markup gramma that embed python code into text
+Author: Eterance
+Keywords: Prompt,Markup Language,NLP,AI,GPT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Pymaidol
 
 Pymaidol 是一种标记语法，用于将 Python 代码嵌入文本中，使得文本在运行时可动态更改包含的内容。
 
 与 [ProMaid](https://github.com/Eterance/ProMaid) 相比，Pymaidol 不只是单纯的将数据嵌入至模板（Template）的对应位置，还能将复杂的处理逻辑呈现在模板中，甚至可使用在模板中定义的函数对数据进行处理。
 
 ⚠**警告：Pymaidol 目前处于开发阶段，语法和一些对空白符、换行符的处理逻辑尚未确定，以后可能会被修改。强烈不建议在生产环境中使用。**
@@ -34,19 +47,24 @@
 ```
 
 ### 编写模板设计文件
 
 首先，用以下代码将 `FirstTemplate.pymd` 中的全部内容替换掉：
 
 ``` python
-from pymaidol.TemplateBase import TemplateBase
+from pymaidol import TemplateBase
+from pymaidol.AnnotationType import FULL_ANNOTATION_TYPE, AnnotationTypeEnum
 
 class FirstTemplate(TemplateBase):
-    def __init__(self, package_name:str, template: str | None = None, template_file_path: str | None = None) -> None:
-        super().__init__(template, template_file_path)
+    def __init__(self, 
+                 package_name:str, 
+                 template: str | None = None, 
+                 template_file_path: str | None = None, 
+                 supported_annotation_types: list[AnnotationTypeEnum] = FULL_ANNOTATION_TYPE) -> None:
+        super().__init__(template, template_file_path, supported_annotation_types)
         self.package_name = package_name
         
 def main():
     template = FirstTemplate("Pymaidol")
     string = template.Render({"says": "Hello World"})
     print(string)
     
@@ -69,10 +87,11 @@
 
 运行 `FirstTemplate.py`，命令行会输出以下内容：
 
 ``` bash
 Now (Tue May 23 19:21:19 2023), Say "Hello World" using Pymaidol!
 ```
 
-## 语法参考
+## 另请参阅
 
-请参阅 [Pymaidol 语法参考](docs/zh-cn//%E8%AF%AD%E6%B3%95%E5%8F%82%E8%80%83.md)
+- [Pymaidol 语法参考](docs/zh-cn/语法参考.md)
+- [Pymaidol_API目录](docs/zh-cn/Pymaidol_API%E7%9B%AE%E5%BD%95.md)
```

### Comparing `pymaidol-0.1.1/docs/zh-cn/语法参考.md` & `pymaidol-0.1.2/docs/zh-cn/语法参考.md`

 * *Files identical despite different names*

### Comparing `pymaidol-0.1.1/pymaidol/AnnotationTypeEnum.py` & `pymaidol-0.1.2/pymaidol/AnnotationType.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     
 class MultiLineAnnotationTypeEnum(AnnotationTypeEnum):
     PythonSingleQuotation:str = "'''"    
     PythonDoubleQuotation:str = '"""'
     C:str = "/*"
     Html:str = "<!--"
     
-FullAnnotationTypes:list[AnnotationTypeEnum] = [
+FULL_ANNOTATION_TYPE:list[AnnotationTypeEnum] = [
     SingleLineAnnotationTypeEnum.Python,
     SingleLineAnnotationTypeEnum.C,
     MultiLineAnnotationTypeEnum.PythonSingleQuotation,
     MultiLineAnnotationTypeEnum.PythonDoubleQuotation,
     MultiLineAnnotationTypeEnum.C,
     MultiLineAnnotationTypeEnum.Html
 ]
```

### Comparing `pymaidol-0.1.1/pymaidol/Errors.py` & `pymaidol-0.1.2/pymaidol/Errors.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     """Base class for all PML exceptions."""
     def __init__(self, position:Position):
         self.position = position
         self.extra_detail:str = ""
         
     @property
     def Message(self):
-        return f"{self.__class__.__name__} at {self.position.FullDescription}: Error Occur\n{self.extra_detail}"
+        return f"{self.__class__.__name__} at {self.position.full_description}: Error Occur\n{self.extra_detail}"
     
     def __repr__(self) -> str:
         return self.Message
     
     def __str__(self) -> str:
         return self.Message
     
@@ -25,74 +25,74 @@
         
     @property
     def Message(self):
         if len(self.expected) == 1:
             expected_string = f'"{self.expected[0]}"'
         else:
             expected_string = f'{self.expected}'
-        return f'{self.__class__.__name__} at {self.position.FullDescription}: Expected {expected_string}, but got {self.got}\n{self.extra_detail}'
+        return f'{self.__class__.__name__} at {self.position.full_description}: Expected {expected_string}, but got {self.got}\n{self.extra_detail}'
 
 # Only use/happen in dev.
 class ImpossibleError(Exception):
     pass
 
 class MultiLineAnnotationFormatError(BaseException):
     @property
     def Message(self):
-        return f"{self.__class__.__name__} at {self.position.FullDescription}: When using multi-line annotation, the line where the terminator is located must not have any text other than the annotation."
+        return f"{self.__class__.__name__} at {self.position.full_description}: When using multi-line annotation, the line where the terminator is located must not have any text other than the annotation."
     
 class UnknownEmbedIdentifierError(BaseException):
     def __init__(self, position:Position, unknown_identifier:str):
         super().__init__(position)
         self.unknown_identifier:str = unknown_identifier
     
     @property
     def Message(self):
-        return f'{self.__class__.__name__} at {self.position.FullDescription}: Unknown "@{self.unknown_identifier}". If you want to write "@" in template, use "@@" instead.'
+        return f'{self.__class__.__name__} at {self.position.full_description}: Unknown "@{self.unknown_identifier}". If you want to write "@" in template, use "@@" instead.'
 
 class LackingConditionError(BaseException):
     @property
     def Message(self):
-        return f'{self.__class__.__name__} at {self.position.FullDescription}: Need Condition'
+        return f'{self.__class__.__name__} at {self.position.full_description}: Need Condition'
 
 class ElseExtraConditionError(BaseException):
     @property
     def Message(self):
-        return f'{self.__class__.__name__} at {self.position.FullDescription}: "else" should not have any condition'
+        return f'{self.__class__.__name__} at {self.position.full_description}: "else" should not have any condition'
     
 
 class BranchError(BaseException):
     @property
     def Message(self):
-        return f'{self.__class__.__name__} at {self.position.FullDescription}: Lacking "if" statement'
+        return f'{self.__class__.__name__} at {self.position.full_description}: Lacking "if" statement'
     
 class WrongForStatement(BaseException):
     @property
     def Message(self):
-        return f'{self.__class__.__name__} at {self.position.FullDescription}: Wrong "for" statement'
+        return f'{self.__class__.__name__} at {self.position.full_description}: Wrong "for" statement'
 
 class PythonExecutionError(BaseException):
     def __init__(self, position: Position, error:Exception):
         super().__init__(position)
         self.error:Exception = error
     
     @property
     def Message(self):
-        return f'{self.__class__.__name__} at {self.position.FullDescription}: \n{str(self.error)}'
+        return f'{self.__class__.__name__} at {self.position.full_description}: \n{str(self.error)}'
     
 class TypeException(BaseException):
     def __init__(self, position: Position, description:str):
         super().__init__(position)
         self.description = description
         
     @property
     def Message(self):
-        return f'{self.__class__.__name__} at {self.position.FullDescription}: {self.description}'
+        return f'{self.__class__.__name__} at {self.position.full_description}: {self.description}'
     
 class NameException(BaseException):
     def __init__(self, position: Position, description:str):
         super().__init__(position)
         self.description = description
         
     @property
     def Message(self):
-        return f'{self.__class__.__name__} at {self.position.FullDescription}: {self.description}'
+        return f'{self.__class__.__name__} at {self.position.full_description}: {self.description}'
```

### Comparing `pymaidol-0.1.1/pymaidol/Executor.py` & `pymaidol-0.1.2/pymaidol/Executor.py`

 * *Files identical despite different names*

### Comparing `pymaidol-0.1.1/pymaidol/Nodes.py` & `pymaidol-0.1.2/pymaidol/Nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import ABC
 from typing import Optional
 
-from pymaidol.AnnotationTypeEnum import AnnotationTypeEnum
+from pymaidol.AnnotationType import AnnotationTypeEnum
 from pymaidol.Positions import Position
 
 
 class ComponentOrRole(ABC):
     '''
     通过继承该类，实现的抽象子类可以用作其他结点类的组件类被继承。\n
     可以往实例结点中添加成员变量，或者赋予实例结点某种身份。
```

### Comparing `pymaidol-0.1.1/pymaidol/Parser.py` & `pymaidol-0.1.2/pymaidol/Parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from enum import Enum
 from typing import Optional, Union
 
-from pymaidol.AnnotationTypeEnum import (AnnotationTypeEnum, FullAnnotationTypes,
+from pymaidol.AnnotationType import (AnnotationTypeEnum, FULL_ANNOTATION_TYPE,
                                 MultiLineAnnotationTypeEnum,
                                 SingleLineAnnotationTypeEnum)
 from pymaidol.Errors import (MultiLineAnnotationFormatError, UnexpectedTokenError,
                     UnknownEmbedIdentifierError)
 from pymaidol.keywords import (KeywordsEnum, NonTerminalKeywords, TerminalKeywords,
                       TranslateKeywords2Type)
 from pymaidol.Nodes import (AnnotationNode, BaseNode, BodyComponent, CodeBlockNode,
                    EmptyNode, NonTerminalNode, ShowBlockNode, TerminalNode,
                    TextNode, VisibleRole)
 from pymaidol.Positions import Position
 from pymaidol.Traversers import PreOrderTraverser
 
 
-class Parser:    
+class Parser:
     def __init__(
         self, 
         template:str, 
         root_node:Optional[NonTerminalNode]=None, 
         start:Position = Position.Default(), 
         end:Optional[Position] = None
         ) -> None:
@@ -32,14 +32,15 @@
         self._last_line_final_char_index = -1
         self.template:str = template
         self.__used = False
         # 用于记录当前行是否有可见字符。注意：“当前行”的定义是当前 node 的 start 所在行，而不是当前字符所在行。
         self._is_line_of_current_start_has_visible_content = False
         
         self.clean_trailing_whitespaces:bool = True
+        self.supported_annotation_types:'list[AnnotationTypeEnum]' = FULL_ANNOTATION_TYPE
     
     @property
     def _current_char(self):
         return self.template[self._current_position.total]
     
     def _peek_several(self, char_count):
         end = self._current_position.total + char_count
@@ -49,36 +50,37 @@
     def _remains(self):
         return self.template[self._current_position.total+1:]
     
     @property
     def _remains_include_current_char(self):
         return self.template[self._current_position.total:]
     
-    def _detect_annotation(self, support_annotation_types:'list[AnnotationTypeEnum]'=FullAnnotationTypes):
+    def _detect_annotation(self):
         """
         检测注释类型。如果当前字符不是注释，则返回None，否则返回注释类型（注释的开始符）和注释的结束符。
         Args:
             support_annotation_types (list[AnnotationType], optional): 支持被检测的注释类型。默认为所有注释类型。
         """
-        if SingleLineAnnotationTypeEnum.Python in support_annotation_types:
+        supported_annotation_types = self.supported_annotation_types
+        if SingleLineAnnotationTypeEnum.Python in supported_annotation_types:
             if self._remains_include_current_char.startswith(SingleLineAnnotationTypeEnum.Python.value):
                 return SingleLineAnnotationTypeEnum.Python, '\n'
-        if SingleLineAnnotationTypeEnum.C in support_annotation_types:
+        if SingleLineAnnotationTypeEnum.C in supported_annotation_types:
             if self._remains_include_current_char.startswith(SingleLineAnnotationTypeEnum.C.value):
                 return SingleLineAnnotationTypeEnum.C, '\n'
-        if MultiLineAnnotationTypeEnum.PythonDoubleQuotation in support_annotation_types:
+        if MultiLineAnnotationTypeEnum.PythonDoubleQuotation in supported_annotation_types:
             if self._remains_include_current_char.startswith(MultiLineAnnotationTypeEnum.PythonDoubleQuotation.value):
                 return MultiLineAnnotationTypeEnum.PythonDoubleQuotation, '"""'
-        if MultiLineAnnotationTypeEnum.PythonSingleQuotation in support_annotation_types:
+        if MultiLineAnnotationTypeEnum.PythonSingleQuotation in supported_annotation_types:
             if self._remains_include_current_char.startswith(MultiLineAnnotationTypeEnum.PythonSingleQuotation.value):
                 return MultiLineAnnotationTypeEnum.PythonSingleQuotation, "'''"
-        if MultiLineAnnotationTypeEnum.C in support_annotation_types:
+        if MultiLineAnnotationTypeEnum.C in supported_annotation_types:
             if self._remains_include_current_char.startswith(MultiLineAnnotationTypeEnum.C.value):
                 return MultiLineAnnotationTypeEnum.C, '*/'
-        if MultiLineAnnotationTypeEnum.Html in support_annotation_types:
+        if MultiLineAnnotationTypeEnum.Html in supported_annotation_types:
             if self._remains_include_current_char.startswith(MultiLineAnnotationTypeEnum.Html.value):
                 return MultiLineAnnotationTypeEnum.Html, '-->'
         return None
     
     def _process_annotation(self, start_sign:AnnotationTypeEnum, end_sign:str):
         self._end_current_node_at_last_char()
         self._create_new_node_at_current_char(AnnotationNode, annotation_type=start_sign)
```

### Comparing `pymaidol-0.1.1/pymaidol/Positions.py` & `pymaidol-0.1.2/pymaidol/Positions.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,19 +16,19 @@
     def total(self):
         return self.__char_index_total
     
     @classmethod
     def Default(cls):
         return cls(0, 0, 0)
     
-    def copy(self):
+    def Copy(self):
         return Position(self.__line_index, self.__char_index, self.__char_index_total)
     
     def __str__(self):
         return f"{self.line_index}:{self.char_index}({self.total})"
     
     @property
-    def FullDescription(self):
+    def full_description(self):
         return f"line {self.line_index} char {self.char_index} (total {self.total})"
     
     def __repr__(self):
         return f"Position @{str(self)}"
```

### Comparing `pymaidol-0.1.1/pymaidol/SyntaxChecker.py` & `pymaidol-0.1.2/pymaidol/SyntaxChecker.py`

 * *Files identical despite different names*

### Comparing `pymaidol-0.1.1/pymaidol/TemplateBase.py` & `pymaidol-0.1.2/pymaidol/TemplateBase.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,27 +2,31 @@
 import inspect
 from abc import ABC, abstractmethod
 from typing import Any, Optional, final
 
 from pymaidol.Executor import Executor
 from pymaidol.Parser import Parser
 from pymaidol.SyntaxChecker import SyntaxChecker
+from pymaidol.TemplateRenderer import TemplateRenderer
+from pymaidol.AnnotationType import FULL_ANNOTATION_TYPE, AnnotationTypeEnum
 
 
 class TemplateBase(ABC):
     @abstractmethod
-    def __init__(self, template:Optional[str]=None, template_file_path:Optional[str]=None) -> None:  
-        self._template:str = ""
-        self._template_file_path:Optional[str] = template_file_path
+    def __init__(self, 
+                 template:Optional[str]=None, 
+                 template_file_path:Optional[str]=None,
+                 supported_annotation_types:'list[AnnotationTypeEnum]' = FULL_ANNOTATION_TYPE) -> None:
+        self.supported_annotation_types = supported_annotation_types
         self.HotReload(template, template_file_path)
-        self._rendered:Optional[str] = None
+        self._rendered:Optional[str] = None    
     
     @property
     def template(self): 
-        return self._template
+        return self._renderer.template
     
     @property
     def rendered(self): 
         '''
         模板设计文件渲染后的结果。如果初始化或热重载以来没有渲染过，则为None。
         '''
         return self._rendered    
@@ -31,27 +35,23 @@
     def HotReload(self, template:Optional[str]=None, template_file_path:Optional[str]=None):
         """ 热重载模板设计文件。如果不指定模板设计文件路径，则使用初始化时指定的模板设计文件路径或者检测到的模板设计文件路径。
 
         Args:
             template_file_path (Optional[str], optional): 模板设计文件路径. Defaults to None.
         """
         if template is not None:
-            self._template = template
+            pass
         elif template_file_path is not None:
-            self._template_file_path = template_file_path
-            self._template = self._ReadTemplate(self._template_file_path)
+            template = self._ReadTemplate(template_file_path)
         else:
             # 获取类的文件路径
             # https://stackoverflow.com/a/697395
-            self._template_file_path = inspect.getfile(self.__class__)[:-3] + ".pymd"
-            self._template = self._ReadTemplate(self._template_file_path)
-        self._rendered = None
-        self._node = Parser(self._template).Parse()
-        self._node = SyntaxChecker().Check(self._node)
-        self._executor = Executor(self._node)
+            template_file_path = inspect.getfile(self.__class__)[:-3] + ".pymd"
+            template = self._ReadTemplate(template_file_path)        
+        self._renderer = TemplateRenderer(template, self.supported_annotation_types)
     
     @final
     def _ReadTemplate(self, template_file_path)->str:
         try: 
             with open(template_file_path, "r", encoding='utf-8') as f:
                 return f.read()
         except FileNotFoundError as fex:
@@ -60,14 +60,14 @@
     
     @final
     def Render(self, inject_kwargs:Optional[dict[str, Any]] = None) -> str:
         global_vars:dict[str, Any] = {}
         local_vars = {"self": self}
         if inject_kwargs is not None:
             global_vars.update(inject_kwargs)
-        result = self._executor.Execute(global_vars, local_vars)
+        result = self._renderer.Render(local_vars, global_vars)
         self._rendered = result
         return result
     
     @final
     def TranslateToPython(self) -> str:
-        raise NotImplementedError()
+        return self._renderer.TranslateToPython()
```

### Comparing `pymaidol-0.1.1/pymaidol/Traversers.py` & `pymaidol-0.1.2/pymaidol/Traversers.py`

 * *Files identical despite different names*

### Comparing `pymaidol-0.1.1/pymaidol/__main__.py` & `pymaidol-0.1.2/pymaidol/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 
 parser = argparse.ArgumentParser()
 parser.add_argument('-n', '--name', type=str, help="the class name of the pymaidol files")
 parser.add_argument('-d', '--dir', type=str, help="the directory of the pymaidol files", default="")
 args = parser.parse_args()
 path = args.dir
+if path is not None and path.strip() != "":
+    os.makedirs(path.strip(), exist_ok=True)
 template_file_path =  os.path.join(path, f'{args.name}.pymd')
 code_file_path =  os.path.join(path, f'{args.name}.py')
 # designer file
 if os.path.exists(template_file_path):
     message = f'Fail: file "{template_file_path}" already exist'
     print(f'\033[0;31;49m{message}\033[0m')
 else:
```

### Comparing `pymaidol-0.1.1/pymaidol/keywords.py` & `pymaidol-0.1.2/pymaidol/keywords.py`

 * *Files identical despite different names*

### Comparing `pymaidol-0.1.1/pymaidol.egg-info/PKG-INFO` & `pymaidol-0.1.2/pymaidol.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymaidol
-Version: 0.1.1
+Version: 0.1.2
 Summary: A markup gramma that embed python code into text
 Author: Eterance
 Keywords: Prompt,Markup Language,NLP,AI,GPT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
@@ -47,19 +47,24 @@
 ```
 
 ### 编写模板设计文件
 
 首先，用以下代码将 `FirstTemplate.pymd` 中的全部内容替换掉：
 
 ``` python
-from pymaidol.TemplateBase import TemplateBase
+from pymaidol import TemplateBase
+from pymaidol.AnnotationType import FULL_ANNOTATION_TYPE, AnnotationTypeEnum
 
 class FirstTemplate(TemplateBase):
-    def __init__(self, package_name:str, template: str | None = None, template_file_path: str | None = None) -> None:
-        super().__init__(template, template_file_path)
+    def __init__(self, 
+                 package_name:str, 
+                 template: str | None = None, 
+                 template_file_path: str | None = None, 
+                 supported_annotation_types: list[AnnotationTypeEnum] = FULL_ANNOTATION_TYPE) -> None:
+        super().__init__(template, template_file_path, supported_annotation_types)
         self.package_name = package_name
         
 def main():
     template = FirstTemplate("Pymaidol")
     string = template.Render({"says": "Hello World"})
     print(string)
     
@@ -82,10 +87,11 @@
 
 运行 `FirstTemplate.py`，命令行会输出以下内容：
 
 ``` bash
 Now (Tue May 23 19:21:19 2023), Say "Hello World" using Pymaidol!
 ```
 
-## 语法参考
+## 另请参阅
 
-请参阅 [Pymaidol 语法参考](docs/zh-cn//%E8%AF%AD%E6%B3%95%E5%8F%82%E8%80%83.md)
+- [Pymaidol 语法参考](docs/zh-cn/语法参考.md)
+- [Pymaidol_API目录](docs/zh-cn/Pymaidol_API%E7%9B%AE%E5%BD%95.md)
```

### Comparing `pymaidol-0.1.1/pymaidol.egg-info/SOURCES.txt` & `pymaidol-0.1.2/pymaidol.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,33 @@
 .gitignore
 LICENSE
 README.md
 pyproject.toml
+docs/zh-cn/Position类.md
+docs/zh-cn/Pymaidol_API目录.md
+docs/zh-cn/TemplateBase类.md
+docs/zh-cn/TemplateRenderer类.md
 docs/zh-cn/语法参考.md
+docs/zh-cn/AnnotationType/AnnotationTypeEnum枚举.md
+docs/zh-cn/AnnotationType/AnnotationType模块.md
+docs/zh-cn/AnnotationType/MultiLineAnnotationTypeEnum枚举.md
+docs/zh-cn/AnnotationType/SingleLineAnnotationTypeEnum枚举.md
 examples/first_template/FirstTemplate.py
 examples/first_template/FirstTemplate.pymd
-pymaidol/AnnotationTypeEnum.py
+examples/template_renderer/renderer_demo.py
+examples/template_renderer/template.pymd
+pymaidol/AnnotationType.py
 pymaidol/Errors.py
 pymaidol/Executor.py
 pymaidol/Nodes.py
 pymaidol/Parser.py
 pymaidol/Positions.py
 pymaidol/SyntaxChecker.py
 pymaidol/TemplateBase.py
+pymaidol/TemplateRenderer.py
 pymaidol/Traversers.py
 pymaidol/__init__.py
 pymaidol/__main__.py
 pymaidol/keywords.py
 pymaidol.egg-info/PKG-INFO
 pymaidol.egg-info/SOURCES.txt
 pymaidol.egg-info/dependency_links.txt
```

### Comparing `pymaidol-0.1.1/pyproject.toml` & `pymaidol-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 description = "A markup gramma that embed python code into text"
 dependencies = [
   "PythonDelegate>=0.1.0",
   ]
 readme = "README.md"
 keywords= ["Prompt", "Markup Language", "NLP", "AI", "GPT"]
 requires-python = ">=3.10"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
     { name="Eterance"},
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `pymaidol-0.1.1/tests/harder_demo/CodeLangTemplate.pymd` & `pymaidol-0.1.2/tests/harder_demo/CodeLangTemplate.pymd`

 * *Files identical despite different names*

### Comparing `pymaidol-0.1.1/tests/harder_demo/sparc_dev_[389, 19, 141, 329, 344, 126, 59, 46, 199, 147].json` & `pymaidol-0.1.2/tests/harder_demo/sparc_dev_[389, 19, 141, 329, 344, 126, 59, 46, 199, 147].json`

 * *Files identical despite different names*

### Comparing `pymaidol-0.1.1/tests/harder_demo/sparc_sub_dataset.pml` & `pymaidol-0.1.2/tests/harder_demo/sparc_sub_dataset.pml`

 * *Files identical despite different names*

### Comparing `pymaidol-0.1.1/tests/harder_demo/sparc_sub_dataset_pml.py` & `pymaidol-0.1.2/tests/harder_demo/sparc_sub_dataset_pml.py`

 * *Files identical despite different names*

### Comparing `pymaidol-0.1.1/tests/test_everything.py` & `pymaidol-0.1.2/tests/test_everything.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 ROOT_DIR = os.path.join(os.path.dirname(__file__), "../")
 SRC_DIR = os.path.join(ROOT_DIR, "src")
 sys.path.append(ROOT_DIR)
 sys.path.append(SRC_DIR)
 from pymaidol.TemplateBase import TemplateBase
-from pymaidol.AnnotationTypeEnum import MultiLineAnnotationTypeEnum
+from pymaidol.AnnotationType import MultiLineAnnotationTypeEnum
 from tests.harder_demo.CodeLangTemplate import CodeLangTemplate
 
 gol = 23
 class father:
     def __init__(self) -> None:
         self.a = 1
```

