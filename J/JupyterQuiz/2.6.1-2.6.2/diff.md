# Comparing `tmp/JupyterQuiz-2.6.1.tar.gz` & `tmp/jupyterquiz-2.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JupyterQuiz-2.6.1.tar", last modified: Fri May 12 10:24:04 2023, max compression
+gzip compressed data, was "jupyterquiz-2.6.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `JupyterQuiz-2.6.1.tar` & `jupyterquiz-2.6.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1826 2023-04-21 13:04:50.495725 JupyterQuiz-2.6.1/.gitignore
--rw-r--r--   0        0        0      192 2021-07-28 14:25:39.473408 JupyterQuiz-2.6.1/CITATION.cff
--rw-r--r--   0        0        0   104165 2021-09-27 14:34:31.769801 JupyterQuiz-2.6.1/HideQuiz.ipynb
--rw-r--r--   0        0        0     1069 2021-06-15 01:46:50.000158 JupyterQuiz-2.6.1/LICENSE
--rw-r--r--   0        0        0    11048 2023-04-28 15:48:44.041844 JupyterQuiz-2.6.1/README.md
--rw-r--r--   0        0        0   205638 2021-07-01 18:38:17.320168 JupyterQuiz-2.6.1/examples/mc-example.gif
--rw-r--r--   0        0        0    43252 2021-06-25 20:33:00.341213 JupyterQuiz-2.6.1/examples/num-example.gif
--rw-r--r--   0        0        0     7318 2023-04-18 16:13:03.229164 JupyterQuiz-2.6.1/examples/questions.json
--rw-r--r--   0        0        0      661 2023-05-12 10:23:45.554586 JupyterQuiz-2.6.1/jupyterquiz/__init__.py
--rw-r--r--   0        0        0    10879 2023-05-12 10:22:00.579714 JupyterQuiz-2.6.1/jupyterquiz/dynamic.py
--rw-r--r--   0        0        0     1653 2022-07-26 16:35:36.993580 JupyterQuiz-2.6.1/jupyterquiz/helpers.js
--rw-r--r--   0        0        0     9336 2023-05-12 09:47:31.721699 JupyterQuiz-2.6.1/jupyterquiz/multiple_choice.js
--rw-r--r--   0        0        0     6127 2023-04-18 15:57:45.160248 JupyterQuiz-2.6.1/jupyterquiz/multiple_choice.py
--rw-r--r--   0        0        0     7733 2023-05-08 22:17:16.273840 JupyterQuiz-2.6.1/jupyterquiz/numeric.js
--rw-r--r--   0        0        0     6192 2023-05-12 09:47:31.722254 JupyterQuiz-2.6.1/jupyterquiz/show_questions.js
--rw-r--r--   0        0        0     2935 2023-04-28 15:09:47.356037 JupyterQuiz-2.6.1/jupyterquiz/styles.css
--rw-r--r--   0        0        0    50597 2022-07-26 16:48:14.000000 JupyterQuiz-2.6.1/preserve-responses.ipynb
--rw-r--r--   0        0        0    50955 2022-09-27 14:13:40.377681 JupyterQuiz-2.6.1/previews/github-preview.png
--rw-r--r--   0        0        0   606109 2022-09-27 14:13:43.947087 JupyterQuiz-2.6.1/previews/github-preview.psd
--rw-r--r--   0        0        0      460 2023-03-11 13:40:05.660600 JupyterQuiz-2.6.1/pyproject.toml
--rw-r--r--   0        0        0       73 2023-04-19 02:45:53.177683 JupyterQuiz-2.6.1/schema/README
--rw-r--r--   0        0        0     1313 2023-04-18 16:54:10.575668 JupyterQuiz-2.6.1/schema/mc_schema.json
--rw-r--r--   0        0        0   107746 2023-04-18 17:18:04.044650 JupyterQuiz-2.6.1/schema/mc_schema.png
--rw-r--r--   0        0        0     4420 2023-04-19 03:25:36.952218 JupyterQuiz-2.6.1/schema/mc_schema.svg
--rw-r--r--   0        0        0     2657 2021-06-15 23:02:36.000000 JupyterQuiz-2.6.1/schema/num_schema.json
--rw-r--r--   0        0        0   247118 2021-06-15 23:07:23.780896 JupyterQuiz-2.6.1/schema/num_schema.png
--rw-r--r--   0        0        0     8208 2023-04-18 17:18:53.556513 JupyterQuiz-2.6.1/schema/schema.ipynb
--rw-r--r--   0        0        0   349141 2023-04-28 15:41:36.693358 JupyterQuiz-2.6.1/test.ipynb
--rw-r--r--   0        0        0    11362 1970-01-01 00:00:00.000000 JupyterQuiz-2.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1826 2023-04-21 13:04:50.495725 jupyterquiz-2.6.2/.gitignore
+-rw-r--r--   0        0        0      192 2021-07-28 14:25:39.473408 jupyterquiz-2.6.2/CITATION.cff
+-rw-r--r--   0        0        0   104165 2023-05-25 18:35:02.178985 jupyterquiz-2.6.2/HideQuiz.ipynb
+-rw-r--r--   0        0        0     1069 2021-06-15 01:46:50.000158 jupyterquiz-2.6.2/LICENSE
+-rw-r--r--   0        0        0    12397 2023-05-25 18:42:50.469959 jupyterquiz-2.6.2/README.md
+-rw-r--r--   0        0        0   205638 2021-07-01 18:38:17.320168 jupyterquiz-2.6.2/examples/mc-example.gif
+-rw-r--r--   0        0        0    43252 2021-06-25 20:33:00.341213 jupyterquiz-2.6.2/examples/num-example.gif
+-rw-r--r--   0        0        0     7318 2023-04-18 16:13:03.229164 jupyterquiz-2.6.2/examples/questions.json
+-rw-r--r--   0        0        0      661 2023-05-25 18:42:59.048642 jupyterquiz-2.6.2/jupyterquiz/__init__.py
+-rw-r--r--   0        0        0    10879 2023-05-25 18:41:05.117384 jupyterquiz-2.6.2/jupyterquiz/dynamic.py
+-rw-r--r--   0        0        0     1653 2022-07-26 16:35:36.993580 jupyterquiz-2.6.2/jupyterquiz/helpers.js
+-rw-r--r--   0        0        0     9336 2023-05-12 09:47:31.721699 jupyterquiz-2.6.2/jupyterquiz/multiple_choice.js
+-rw-r--r--   0        0        0     6127 2023-04-18 15:57:45.160248 jupyterquiz-2.6.2/jupyterquiz/multiple_choice.py
+-rw-r--r--   0        0        0     7733 2023-05-08 22:17:16.273840 jupyterquiz-2.6.2/jupyterquiz/numeric.js
+-rw-r--r--   0        0        0     6192 2023-05-12 09:47:31.722254 jupyterquiz-2.6.2/jupyterquiz/show_questions.js
+-rw-r--r--   0        0        0     2935 2023-05-25 18:35:28.477892 jupyterquiz-2.6.2/jupyterquiz/styles.css
+-rw-r--r--   0        0        0    50597 2022-07-26 16:48:14.000000 jupyterquiz-2.6.2/preserve-responses.ipynb
+-rw-r--r--   0        0        0    50955 2022-09-27 14:13:40.377681 jupyterquiz-2.6.2/previews/github-preview.png
+-rw-r--r--   0        0        0   606109 2022-09-27 14:13:43.947087 jupyterquiz-2.6.2/previews/github-preview.psd
+-rw-r--r--   0        0        0      460 2023-03-11 13:40:05.660600 jupyterquiz-2.6.2/pyproject.toml
+-rw-r--r--   0        0        0       73 2023-04-19 02:45:53.177683 jupyterquiz-2.6.2/schema/README
+-rw-r--r--   0        0        0     1313 2023-04-18 16:54:10.575668 jupyterquiz-2.6.2/schema/mc_schema.json
+-rw-r--r--   0        0        0   107746 2023-04-18 17:18:04.044650 jupyterquiz-2.6.2/schema/mc_schema.png
+-rw-r--r--   0        0        0     4420 2023-04-19 03:25:36.952218 jupyterquiz-2.6.2/schema/mc_schema.svg
+-rw-r--r--   0        0        0     2657 2021-06-15 23:02:36.000000 jupyterquiz-2.6.2/schema/num_schema.json
+-rw-r--r--   0        0        0   247118 2021-06-15 23:07:23.780896 jupyterquiz-2.6.2/schema/num_schema.png
+-rw-r--r--   0        0        0     8208 2023-04-18 17:18:53.556513 jupyterquiz-2.6.2/schema/schema.ipynb
+-rw-r--r--   0        0        0   349141 2023-04-28 15:41:36.693358 jupyterquiz-2.6.2/test.ipynb
+-rw-r--r--   0        0        0    12711 1970-01-01 00:00:00.000000 jupyterquiz-2.6.2/PKG-INFO
```

### Comparing `JupyterQuiz-2.6.1/.gitignore` & `jupyterquiz-2.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.6.1/HideQuiz.ipynb` & `jupyterquiz-2.6.2/HideQuiz.ipynb`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.6.1/LICENSE` & `jupyterquiz-2.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.6.1/README.md` & `jupyterquiz-2.6.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -17,17 +17,25 @@
  
  **Numerical Answer Question**
  
 ![Example numerical answer question using JupyterQuiz.](https://github.com/jmshea/jupyterquiz/blob/main/examples/num-example.gif?raw=true)
 
 ---
 
-For more examples with various types of functionality, check out the Review section of Chapter 3 of the *Foundations of Data Science with Python* Jupyter Book: 
+**Examples using JupyterQuiz**
 
-[Example of JupyterQuiz in Action](https://jmshea.github.io/Foundations-of-Data-Science-with-Python/03-first-data/review.html)
+* *Foundations of Data Science with Python* book by John M. Shea. Example: [Chapter 3 Review, ](https://jmshea.github.io/Foundations-of-Data-Science-with-Python/03-first-data/review.html)
+* *Introduction to Python for Humanists* book by W.J.B. Mattingly. Example: [Section 2.2 Introduction to Data Structures, ](https://python-textbook.pythonhumanities.com/01_intro/01_02-03_data_structures.html)
+* *Groundwater I* by  P. K. Yadav, T. Reimann, and others. Example: [Lecture 1: Course Introduction/Water Cycle of ](https://vibhubatheja.github.io/GW-Book/content/background/03_basic_hydrogeology.html)
+* *Sizing and optimization of mechatronic systems* course by Marc Budinger, Scott Delbecq and Félix Pollet. Example: [Lecture 1 Quiz](https://sizinglab.github.io/sizing_course/class/Lecture1/4-quizz.html)
+* *Linux en Bioinformatique* by Thomas Denecker & Claire Toffano-Nioche. Example: [Quizz 1](https://ifb-elixirfr.github.io/LinuxEBAII/quizz_01.html) 
+* *Programmering i Kjemi (Programming in Chemistry?)* by Andreas Haraldsrud. Example: [Quiz 1: Variabler og aritmetikk](https://andreasdh.github.io/programmering-i-kjemi/docs/grunnleggende_programmering/quiz1.html)
+* *AnIML: Another Introduction to Machine Learning* by Hunter Schafer. Example: [Chapter 2: Assessing Performance](https://animlbook.com/regression/assessing_performance/index.html)
+
+If you using JupyterQuiz in a Jupyter Book or other way that is useable on the web, please clone this repository, add your information to the bulleted list in the README.md, and make a pull request for me to include a link to your use of this library.
 
 The notebook [test.ipynb](test.ipynb) shows more features but must be run on your own local Jupyter or in nbviewer -- GitHub only renders the static HTML that does not include the interactive quizzes. (If viewing on GitHub, there should be a little circle with a minus sign at the top of the file that offers you the ability to launch the notebook in nbviewer.)
 
 It currently supports two types of quiz questions:
 1. **Multiple/ Many Choice Questions:** Users are given a predefined set of choices and click on answer(s) they believe are correct.
 2. **Numerical:** Users are given a text box in which they can submit answers in decimal or fraction form.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `JupyterQuiz-2.6.1/examples/mc-example.gif` & `jupyterquiz-2.6.2/examples/mc-example.gif`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.6.1/examples/num-example.gif` & `jupyterquiz-2.6.2/examples/num-example.gif`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.6.1/examples/questions.json` & `jupyterquiz-2.6.2/examples/questions.json`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.6.1/jupyterquiz/__init__.py` & `jupyterquiz-2.6.2/jupyterquiz/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,9 +7,9 @@
 
 Created by John M. Shea, copyright 2021
 for the book Introduction to Data Science for Engineers
 
 All files in the package are distributed under the MIT License
 '''
 
-__version__ = '2.6.1'
+__version__ = '2.6.2'
 from .dynamic import display_quiz, capture_responses
```

### Comparing `JupyterQuiz-2.6.1/jupyterquiz/dynamic.py` & `jupyterquiz-2.6.2/jupyterquiz/dynamic.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
     #axes.prop_cycle: cycler('color', [ '345995', 'e26d5a', '87a878', '5bc0eb', '861657'])
     fdsp_dict = {
         '--jq-multiple-choice-bg': '#345995',
         '--jq-mc-button-bg': '#fafafa',
         '--jq-mc-button-border': '#e0e0e0e0',
         '--jq-mc-button-inset-shadow': '#555555',
         '--jq-many-choice-bg': '#e26d5a',
-        '--Jq-numeric-bg': '#5bc0eb', #'#861657',
+        '--jq-numeric-bg': '#5bc0eb', #'#861657',
         '--jq-numeric-input-bg': '#c0c0c0',
         '--jq-numeric-input-label': '#101010',
         '--jq-numeric-input-shadow': '#999999',
         '--jq-incorrect-color': '#666666',
         '--jq-correct-color': '#87a878',
         '--jq-text-color': '#fafafa'
     }
```

### Comparing `JupyterQuiz-2.6.1/jupyterquiz/helpers.js` & `jupyterquiz-2.6.2/jupyterquiz/helpers.js`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.6.1/jupyterquiz/multiple_choice.js` & `jupyterquiz-2.6.2/jupyterquiz/multiple_choice.js`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.6.1/jupyterquiz/multiple_choice.py` & `jupyterquiz-2.6.2/jupyterquiz/multiple_choice.py`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.6.1/jupyterquiz/numeric.js` & `jupyterquiz-2.6.2/jupyterquiz/numeric.js`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.6.1/jupyterquiz/show_questions.js` & `jupyterquiz-2.6.2/jupyterquiz/show_questions.js`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.6.1/jupyterquiz/styles.css` & `jupyterquiz-2.6.2/jupyterquiz/styles.css`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.6.1/preserve-responses.ipynb` & `jupyterquiz-2.6.2/preserve-responses.ipynb`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.6.1/previews/github-preview.png` & `jupyterquiz-2.6.2/previews/github-preview.png`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.6.1/previews/github-preview.psd` & `jupyterquiz-2.6.2/previews/github-preview.psd`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.6.1/schema/mc_schema.json` & `jupyterquiz-2.6.2/schema/mc_schema.json`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.6.1/schema/mc_schema.png` & `jupyterquiz-2.6.2/schema/mc_schema.png`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.6.1/schema/mc_schema.svg` & `jupyterquiz-2.6.2/schema/mc_schema.svg`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.6.1/schema/num_schema.json` & `jupyterquiz-2.6.2/schema/num_schema.json`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.6.1/schema/num_schema.png` & `jupyterquiz-2.6.2/schema/num_schema.png`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.6.1/schema/schema.ipynb` & `jupyterquiz-2.6.2/schema/schema.ipynb`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.6.1/test.ipynb` & `jupyterquiz-2.6.2/test.ipynb`

 * *Files identical despite different names*

### Comparing `JupyterQuiz-2.6.1/PKG-INFO` & `jupyterquiz-2.6.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JupyterQuiz
-Version: 2.6.1
+Version: 2.6.2
 Summary: Interactive quizzes for Jupyter and Jupyter Book
 Author-email: "John M. Shea" <jshea@ieee.org>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Project-URL: home-page, https://github.com/jmshea/jupyterquiz
 
 # JupyterQuiz
@@ -26,17 +26,25 @@
  
  **Numerical Answer Question**
  
 ![Example numerical answer question using JupyterQuiz.](https://github.com/jmshea/jupyterquiz/blob/main/examples/num-example.gif?raw=true)
 
 ---
 
-For more examples with various types of functionality, check out the Review section of Chapter 3 of the *Foundations of Data Science with Python* Jupyter Book: 
+**Examples using JupyterQuiz**
 
-[Example of JupyterQuiz in Action](https://jmshea.github.io/Foundations-of-Data-Science-with-Python/03-first-data/review.html)
+* *Foundations of Data Science with Python* book by John M. Shea. Example: [Chapter 3 Review, ](https://jmshea.github.io/Foundations-of-Data-Science-with-Python/03-first-data/review.html)
+* *Introduction to Python for Humanists* book by W.J.B. Mattingly. Example: [Section 2.2 Introduction to Data Structures, ](https://python-textbook.pythonhumanities.com/01_intro/01_02-03_data_structures.html)
+* *Groundwater I* by  P. K. Yadav, T. Reimann, and others. Example: [Lecture 1: Course Introduction/Water Cycle of ](https://vibhubatheja.github.io/GW-Book/content/background/03_basic_hydrogeology.html)
+* *Sizing and optimization of mechatronic systems* course by Marc Budinger, Scott Delbecq and Félix Pollet. Example: [Lecture 1 Quiz](https://sizinglab.github.io/sizing_course/class/Lecture1/4-quizz.html)
+* *Linux en Bioinformatique* by Thomas Denecker & Claire Toffano-Nioche. Example: [Quizz 1](https://ifb-elixirfr.github.io/LinuxEBAII/quizz_01.html) 
+* *Programmering i Kjemi (Programming in Chemistry?)* by Andreas Haraldsrud. Example: [Quiz 1: Variabler og aritmetikk](https://andreasdh.github.io/programmering-i-kjemi/docs/grunnleggende_programmering/quiz1.html)
+* *AnIML: Another Introduction to Machine Learning* by Hunter Schafer. Example: [Chapter 2: Assessing Performance](https://animlbook.com/regression/assessing_performance/index.html)
+
+If you using JupyterQuiz in a Jupyter Book or other way that is useable on the web, please clone this repository, add your information to the bulleted list in the README.md, and make a pull request for me to include a link to your use of this library.
 
 The notebook [test.ipynb](test.ipynb) shows more features but must be run on your own local Jupyter or in nbviewer -- GitHub only renders the static HTML that does not include the interactive quizzes. (If viewing on GitHub, there should be a little circle with a minus sign at the top of the file that offers you the ability to launch the notebook in nbviewer.)
 
 It currently supports two types of quiz questions:
 1. **Multiple/ Many Choice Questions:** Users are given a predefined set of choices and click on answer(s) they believe are correct.
 2. **Numerical:** Users are given a text box in which they can submit answers in decimal or fraction form.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

