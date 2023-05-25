# Comparing `tmp/Pydule-3.3.4.tar.gz` & `tmp/Pydule-3.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pydule-3.3.4.tar", last modified: Fri May 19 06:17:48 2023, max compression
+gzip compressed data, was "Pydule-3.3.5.tar", last modified: Thu May 25 09:38:55 2023, max compression
```

## Comparing `Pydule-3.3.4.tar` & `Pydule-3.3.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 06:17:48.684229 Pydule-3.3.4/
--rw-rw-rw-   0        0        0     2547 2023-05-19 06:17:48.653219 Pydule-3.3.4/PKG-INFO
--rw-rw-rw-   0        0        0     1783 2023-05-19 06:08:01.000000 Pydule-3.3.4/README.md
--rw-rw-rw-   0        0        0       42 2023-05-19 06:17:48.684229 Pydule-3.3.4/setup.cfg
--rw-rw-rw-   0        0        0     1474 2023-05-19 06:07:38.000000 Pydule-3.3.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-19 06:17:48.434976 Pydule-3.3.4/src/
-drwxrwxrwx   0        0        0        0 2023-05-19 06:17:48.637382 Pydule-3.3.4/src/Pydule.egg-info/
--rw-rw-rw-   0        0        0     2547 2023-05-19 06:17:47.000000 Pydule-3.3.4/src/Pydule.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2023-05-19 06:17:47.000000 Pydule-3.3.4/src/Pydule.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 06:17:47.000000 Pydule-3.3.4/src/Pydule.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      237 2023-05-19 06:17:47.000000 Pydule-3.3.4/src/Pydule.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-19 06:17:47.000000 Pydule-3.3.4/src/Pydule.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    21890 2023-05-19 06:13:53.000000 Pydule-3.3.4/src/Pydule.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:38:55.685967 Pydule-3.3.5/
+-rw-rw-rw-   0        0        0     2543 2023-05-25 09:38:55.665796 Pydule-3.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1779 2023-05-25 09:27:27.000000 Pydule-3.3.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-25 09:38:55.685967 Pydule-3.3.5/setup.cfg
+-rw-rw-rw-   0        0        0     1474 2023-05-25 09:27:52.000000 Pydule-3.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 09:38:55.597077 Pydule-3.3.5/src/
+drwxrwxrwx   0        0        0        0 2023-05-25 09:38:55.661080 Pydule-3.3.5/src/Pydule.egg-info/
+-rw-rw-rw-   0        0        0     2543 2023-05-25 09:38:54.000000 Pydule-3.3.5/src/Pydule.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2023-05-25 09:38:54.000000 Pydule-3.3.5/src/Pydule.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 09:38:54.000000 Pydule-3.3.5/src/Pydule.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      237 2023-05-25 09:38:54.000000 Pydule-3.3.5/src/Pydule.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-25 09:38:54.000000 Pydule-3.3.5/src/Pydule.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    21890 2023-05-19 06:13:54.000000 Pydule-3.3.5/src/Pydule.py
```

### Comparing `Pydule-3.3.4/PKG-INFO` & `Pydule-3.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pydule
-Version: 3.3.4
+Version: 3.3.5
 Summary: Access ChatGPT,Track Location,Play Songs,Create Qrcode,Copy Text,Translate a Sentence to Other Language and more..
 Author: D.Tamil Mutharasan
 Keywords: python,PyDule,Module,Pydule,pydule,matrix,qrcode,youtube,weather,list,tuple,set,dictionary,clear,color,pick_color,open,app,search,play,mp3,song,restart,system,shutdown,date,time,text_to_speech,text,speech
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
@@ -76,15 +76,15 @@
 # to Get all Available Functions
 py.functions() 
 
 # to Open Calculator
 py.openapp('calculator')
 
 # to Copy Text
-py.copytext('Hello World')
+py.copy('Hello World')
 
 # to play mp3
 py.playmusic('PATH')
 
 # to Access ChatGPT
 from Pydule import AI
 print(AI.ChatGPT('Hi There','Your API Key'))
```

### Comparing `Pydule-3.3.4/README.md` & `Pydule-3.3.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 # to Get all Available Functions
 py.functions() 
 
 # to Open Calculator
 py.openapp('calculator')
 
 # to Copy Text
-py.copytext('Hello World')
+py.copy('Hello World')
 
 # to play mp3
 py.playmusic('PATH')
 
 # to Access ChatGPT
 from Pydule import AI
 print(AI.ChatGPT('Hi There','Your API Key'))
```

### Comparing `Pydule-3.3.4/setup.py` & `Pydule-3.3.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open('README.md','r') as fh:
 	long_description = fh.read()
 
 setup(
 	name='Pydule',
-	version='3.3.4',
+	version='3.3.5',
 	description="Access ChatGPT,Track Location,Play Songs,Create Qrcode,Copy Text,Translate a Sentence to Other Language and more..",
 	author='D.Tamil Mutharasan',
 	long_description=long_description,
 	long_description_content_type='text/markdown',
 	packages=setuptools.find_packages(),
 	keywords=['python','PyDule','Module','Pydule','pydule','matrix','qrcode','youtube','weather','list','tuple','set','dictionary','clear','color','pick_color','open','app','search','play','mp3','song','restart','system','shutdown','date','time','text_to_speech','text','speech'],
 	classifiers=[
```

### Comparing `Pydule-3.3.4/src/Pydule.egg-info/PKG-INFO` & `Pydule-3.3.5/src/Pydule.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pydule
-Version: 3.3.4
+Version: 3.3.5
 Summary: Access ChatGPT,Track Location,Play Songs,Create Qrcode,Copy Text,Translate a Sentence to Other Language and more..
 Author: D.Tamil Mutharasan
 Keywords: python,PyDule,Module,Pydule,pydule,matrix,qrcode,youtube,weather,list,tuple,set,dictionary,clear,color,pick_color,open,app,search,play,mp3,song,restart,system,shutdown,date,time,text_to_speech,text,speech
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
@@ -76,15 +76,15 @@
 # to Get all Available Functions
 py.functions() 
 
 # to Open Calculator
 py.openapp('calculator')
 
 # to Copy Text
-py.copytext('Hello World')
+py.copy('Hello World')
 
 # to play mp3
 py.playmusic('PATH')
 
 # to Access ChatGPT
 from Pydule import AI
 print(AI.ChatGPT('Hi There','Your API Key'))
```

### Comparing `Pydule-3.3.4/src/Pydule.py` & `Pydule-3.3.5/src/Pydule.py`

 * *Files identical despite different names*

