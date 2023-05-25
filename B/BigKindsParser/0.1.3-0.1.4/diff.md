# Comparing `tmp/BigKindsParser-0.1.3-py3-none-any.whl.zip` & `tmp/BigKindsParser-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,11 @@
-Zip file size: 2354 bytes, number of entries: 5
--rw-r--r--  2.0 unx     1070 b- defN 23-May-25 02:17 BigKindsParser-0.1.3.dist-info/LICENSE
--rw-r--r--  2.0 unx      962 b- defN 23-May-25 02:17 BigKindsParser-0.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-25 02:17 BigKindsParser-0.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-May-25 02:17 BigKindsParser-0.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      419 b- defN 23-May-25 02:17 BigKindsParser-0.1.3.dist-info/RECORD
-5 files, 2544 bytes uncompressed, 1564 bytes compressed:  38.5%
+Zip file size: 4910 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      496 b- defN 23-May-25 02:06 BigKindsParser/__init__.py
+-rw-r--r--  2.0 unx       22 b- defN 23-May-25 02:58 BigKindsParser/_version.py
+-rw-r--r--  2.0 unx     1691 b- defN 23-May-25 01:58 BigKindsParser/preprocessing.py
+-rw-r--r--  2.0 unx     1577 b- defN 23-May-25 01:58 BigKindsParser/visualization.py
+-rw-r--r--  2.0 unx     1070 b- defN 23-May-25 02:59 BigKindsParser-0.1.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1324 b- defN 23-May-25 02:59 BigKindsParser-0.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-25 02:59 BigKindsParser-0.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-May-25 02:59 BigKindsParser-0.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      760 b- defN 23-May-25 02:59 BigKindsParser-0.1.4.dist-info/RECORD
+9 files, 7047 bytes uncompressed, 3588 bytes compressed:  49.1%
```

## zipnote {}

```diff
@@ -1,16 +1,28 @@
-Filename: BigKindsParser-0.1.3.dist-info/LICENSE
+Filename: BigKindsParser/__init__.py
 Comment: 
 
-Filename: BigKindsParser-0.1.3.dist-info/METADATA
+Filename: BigKindsParser/_version.py
 Comment: 
 
-Filename: BigKindsParser-0.1.3.dist-info/WHEEL
+Filename: BigKindsParser/preprocessing.py
 Comment: 
 
-Filename: BigKindsParser-0.1.3.dist-info/top_level.txt
+Filename: BigKindsParser/visualization.py
 Comment: 
 
-Filename: BigKindsParser-0.1.3.dist-info/RECORD
+Filename: BigKindsParser-0.1.4.dist-info/LICENSE
+Comment: 
+
+Filename: BigKindsParser-0.1.4.dist-info/METADATA
+Comment: 
+
+Filename: BigKindsParser-0.1.4.dist-info/WHEEL
+Comment: 
+
+Filename: BigKindsParser-0.1.4.dist-info/top_level.txt
+Comment: 
+
+Filename: BigKindsParser-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `BigKindsParser-0.1.3.dist-info/LICENSE` & `BigKindsParser-0.1.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `BigKindsParser-0.1.3.dist-info/METADATA` & `BigKindsParser-0.1.4.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 Metadata-Version: 2.1
 Name: BigKindsParser
-Version: 0.1.3
-Summary: Exploratory data analysis Toolkit of Python for BigKinds Data
+Version: 0.1.4
+Summary: Journalism, preprocessing-data.
 Home-page: https://github.com/sorrychoe/BigKindsParser
-Author: sorrychoe
-Author-email: cjssoote@gmail.com
+Author: Sorrychoe
 License: MIT
-Keywords: Journalism,preprocessing-data
-Requires-Python: >=3.8
+Project-URL: Source Code, https://github.com/sorrychoe/BigKindsParser
+Project-URL: Bug Tracker, https://github.com/sorrychoe/BigKindsParser/issues
+Keywords: Journalism,preprocessing-data,BigKinds
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib (>=3.5.3)
-Requires-Dist: pandas (==1.5.1)
+Requires-Dist: pandas (==1.5.2)
 Requires-Dist: wordcloud (>=1.8.2.2)
+Provides-Extra: dev
+Requires-Dist: black (<=22.12,>=19.3b0) ; extra == 'dev'
+Requires-Dist: flake8 (>=3.9) ; extra == 'dev'
+Requires-Dist: isort (>=5.7) ; extra == 'dev'
+Requires-Dist: pre-commit (>=2.13) ; extra == 'dev'
+Requires-Dist: pylint (>=2.9) ; extra == 'dev'
 
 # BigKindsParser
 
 > BigKindsParser는 한국 언론의 빅데이터 저장소인 BigKinds에서 추출한 데이터를 low-Code로 분석할 수 있게 만든 툴입니다.
 
 ## Requirements
```

