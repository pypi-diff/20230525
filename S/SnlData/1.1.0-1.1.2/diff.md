# Comparing `tmp/SnlData-1.1.0.tar.gz` & `tmp/SnlData-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/SnlData-1.1.0.tar", last modified: Wed Dec  2 11:49:58 2020, max compression
+gzip compressed data, was "SnlData-1.1.2.tar", last modified: Thu May 25 16:39:17 2023, max compression
```

## Comparing `SnlData-1.1.0.tar` & `SnlData-1.1.2.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxr-xr-x   0 andreas    (501) staff       (20)        0 2020-12-02 11:49:58.765525 SnlData-1.1.0/
--rw-r--r--   0 andreas    (501) staff       (20)    11014 2020-12-02 11:49:58.765257 SnlData-1.1.0/PKG-INFO
--rw-r--r--   0 andreas    (501) staff       (20)     8499 2020-12-02 11:38:06.000000 SnlData-1.1.0/README.md
-drwxr-xr-x   0 andreas    (501) staff       (20)        0 2020-12-02 11:49:58.764224 SnlData-1.1.0/SnlData.egg-info/
--rw-r--r--   0 andreas    (501) staff       (20)    11014 2020-12-02 11:49:58.000000 SnlData-1.1.0/SnlData.egg-info/PKG-INFO
--rw-r--r--   0 andreas    (501) staff       (20)      240 2020-12-02 11:49:58.000000 SnlData-1.1.0/SnlData.egg-info/SOURCES.txt
--rw-r--r--   0 andreas    (501) staff       (20)        1 2020-12-02 11:49:58.000000 SnlData-1.1.0/SnlData.egg-info/dependency_links.txt
--rw-r--r--   0 andreas    (501) staff       (20)        1 2020-12-02 11:38:25.000000 SnlData-1.1.0/SnlData.egg-info/not-zip-safe
--rw-r--r--   0 andreas    (501) staff       (20)       17 2020-12-02 11:49:58.000000 SnlData-1.1.0/SnlData.egg-info/requires.txt
--rw-r--r--   0 andreas    (501) staff       (20)        8 2020-12-02 11:49:58.000000 SnlData-1.1.0/SnlData.egg-info/top_level.txt
--rw-r--r--   0 andreas    (501) staff       (20)       38 2020-12-02 11:49:58.765620 SnlData-1.1.0/setup.cfg
--rw-r--r--   0 andreas    (501) staff       (20)     2182 2020-12-02 11:49:40.000000 SnlData-1.1.0/setup.py
-drwxr-xr-x   0 andreas    (501) staff       (20)        0 2020-12-02 11:49:58.764765 SnlData-1.1.0/snldata/
--rw-r--r--   0 andreas    (501) staff       (20)       30 2020-12-02 11:38:06.000000 SnlData-1.1.0/snldata/__init__.py
--rw-r--r--   0 andreas    (501) staff       (20)    12674 2020-12-02 11:38:06.000000 SnlData-1.1.0/snldata/client.py
+drwxr-xr-x   0 andreas    (502) staff       (20)        0 2023-05-25 16:39:17.637145 SnlData-1.1.2/
+-rw-r--r--   0 andreas    (502) staff       (20)    35149 2023-05-25 11:44:43.000000 SnlData-1.1.2/LICENSE
+-rw-r--r--   0 andreas    (502) staff       (20)     8959 2023-05-25 16:39:17.636991 SnlData-1.1.2/PKG-INFO
+-rw-r--r--   0 andreas    (502) staff       (20)     7982 2023-05-25 14:15:22.000000 SnlData-1.1.2/README.md
+drwxr-xr-x   0 andreas    (502) staff       (20)        0 2023-05-25 16:39:17.636233 SnlData-1.1.2/SnlData.egg-info/
+-rw-r--r--   0 andreas    (502) staff       (20)     8959 2023-05-25 16:39:17.000000 SnlData-1.1.2/SnlData.egg-info/PKG-INFO
+-rw-r--r--   0 andreas    (502) staff       (20)      269 2023-05-25 16:39:17.000000 SnlData-1.1.2/SnlData.egg-info/SOURCES.txt
+-rw-r--r--   0 andreas    (502) staff       (20)        1 2023-05-25 16:39:17.000000 SnlData-1.1.2/SnlData.egg-info/dependency_links.txt
+-rw-r--r--   0 andreas    (502) staff       (20)        1 2023-05-25 16:39:17.000000 SnlData-1.1.2/SnlData.egg-info/not-zip-safe
+-rw-r--r--   0 andreas    (502) staff       (20)       17 2023-05-25 16:39:17.000000 SnlData-1.1.2/SnlData.egg-info/requires.txt
+-rw-r--r--   0 andreas    (502) staff       (20)        8 2023-05-25 16:39:17.000000 SnlData-1.1.2/SnlData.egg-info/top_level.txt
+-rw-r--r--   0 andreas    (502) staff       (20)       38 2023-05-25 16:39:17.637184 SnlData-1.1.2/setup.cfg
+-rw-r--r--   0 andreas    (502) staff       (20)     2150 2023-05-25 13:41:19.000000 SnlData-1.1.2/setup.py
+drwxr-xr-x   0 andreas    (502) staff       (20)        0 2023-05-25 16:39:17.636504 SnlData-1.1.2/snldata/
+-rw-r--r--   0 andreas    (502) staff       (20)       30 2023-05-25 11:44:43.000000 SnlData-1.1.2/snldata/__init__.py
+-rw-r--r--   0 andreas    (502) staff       (20)    13311 2023-05-25 13:37:52.000000 SnlData-1.1.2/snldata/client.py
+drwxr-xr-x   0 andreas    (502) staff       (20)        0 2023-05-25 16:39:17.636718 SnlData-1.1.2/tests/
+-rw-r--r--   0 andreas    (502) staff       (20)     4959 2023-05-25 14:18:15.000000 SnlData-1.1.2/tests/test_client.py
```

### Comparing `SnlData-1.1.0/PKG-INFO` & `SnlData-1.1.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,213 +1,191 @@
 Metadata-Version: 2.1
 Name: SnlData
-Version: 1.1.0
-Summary: A lightweight Python library for Store Norske Leksikon and Lex.dk APIs.
+Version: 1.1.2
+Summary: A lightweight Python library for Store Norske Leksikon and Lex.dk/Den Store Danske APIs.
 Home-page: https://github.com/DiFronzo/SnlData
 Author: DiFronzo
 Author-email: root@vfiles.no
 License: GPLv3
-Description: <p align="center">
-          <a href="https://github.com/DiFronzo/snldata"><img alt="Logo" width="500" height="300" src="https://snldata.readthedocs.io/en/latest/_static/snldata_logo.svg"></a>
-        </p>
-        <p align="center">
-          <a href="https://github.com/DiFronzo/snldata/actions"><img alt="Actions Status" src="https://github.com/DiFronzo/SnlData/workflows/Test/badge.svg"></a>
-          <a href="https://snldata.readthedocs.io/en/latest/?badge=latest"><img alt="Documentation Status" src="https://readthedocs.org/projects/snldata/badge/?version=latest"></a>
-        	<a href="https://app.fossa.com/projects/git%2Bgithub.com%2FDiFronzo%2FSnlData?ref=badge_small" alt="FOSSA Status"><img src="https://app.fossa.com/api/projects/git%2Bgithub.com%2FDiFronzo%2FSnlData.svg?type=small"/></a>
-          <a href="https://codecov.io/gh/DiFronzo/SnlData"><img alt="Coverage Status" src="https://codecov.io/gh/DiFronzo/SnlData/branch/master/graph/badge.svg"></a>
-          <a href="https://travis-ci.com/DiFronzo/SnlData"><img alt="Build Status" src="https://api.travis-ci.com/DiFronzo/SnlData.svg?branch=master"></a>	
-          <a href="https://github.com/DiFronzo/SnlData/blob/master/LICENSE"><img alt="License: MIT" src="https://snldata.readthedocs.io/en/latest/_static/license.svg"></a>
-          <a href="https://pepy.tech/project/snldata"><img alt="Downloads" src="https://pepy.tech/badge/snldata"></a>
-          <a href="https://pypi.org/project/snldata/"><img alt="PyPI" src="https://img.shields.io/pypi/v/snldata"></a>
-          <h4>A lightweight Python library for Store Norske Leksikon and Lex.dk APIs</h4>
-        </p>
-        
-        ## Installation
-        
-            pip install snldata
-        
-        ## Quick Start
-        Raw JSON
-        ```python
-        import snldata
-        
-        R = snldata.SnlSession()
-        R.search(query="fortolket programmeringsspråk", best=True) #Pick the one with the best rank
-        print(R.json)
-        
-        ```
-        Outputs: the JSON object
-        ```
-        {
-        	"title": "fortolket programmeringsspråk",
-        	"url": "http://snl.no/fortolket_programmeringsspr%C3%A5k",
-        	"subject_url": "http://snl.no/.taxonomy/3689",
-        	"subject_title": "Programmering",
-        	"xhtml_body": "\u003cdiv\u003e\r\n\u003cp\u003eprogrammeringsspråk som ikke blir kompilert til objekt- eller maskinkode, men fortolket av et eget program på vertsmaskinen.\u003c/p\u003e\r\n\u003cp\u003eFordelen med slike språk er at man kan lage programmer som kan gjøre på mange forskjellige \u003ca class=\"crossref\" href=\"https://snl.no/datamaskin\"\u003edatamaskiner\u003c/a\u003e og \u003ca class=\"crossref\" href=\"https://snl.no/operativsystem\"\u003eoperativsystemer\u003c/a\u003e uten å skreddersy dem for hver enkelt plattform.\u003c/p\u003e\r\n\u003cp\u003eEksempler på fortolkede språk:\u003c/p\u003e\r\n\u003cul\u003e\r\n\u003cli\u003e\u003ca class=\"crossref\" href=\"https://snl.no/Python_-_programmeringsspr%C3%A5k\"\u003ePython\u003c/a\u003e\u003c/li\u003e\r\n\u003cli\u003eJavascript\u003c/li\u003e\r\n\u003cli\u003e\u003ca class=\"crossref\" href=\"https://snl.no/Perl_-_IT\"\u003ePHP\u003c/a\u003e\u003c/li\u003e\r\n\u003cli\u003e\u003ca class=\"crossref\" href=\"https://snl.no/Perl_-_IT\"\u003ePerl\u003c/a\u003e\u003c/li\u003e\r\n\u003c/ul\u003e\r\n\u003c/div\u003e",
-        	"created_at": "2017-12-12T10:34:18.189+01:00",
-        	"changed_at": "2017-12-12T10:38:37.626+01:00",
-        	"license_name": "fri",
-        	"metadata_license_name": "fri",
-        	"metadata": {
-        		"lastname": "",
-        		"firstname": ""
-        	},
-        	"authors": [{
-        		"full_name": "Henrik Dvergsdal"
-        	}],
-        	"images": []
-        }
-        ```
-        ## Licenses for content from Store Norske Leksikon and Lex.dk 
-        | Licence | Description | Read more
-        | --- | --- | --- |
-        | `fri` | [Creative Commons](https://creativecommons.org/) **[CC-BY-SA-3.0](https://creativecommons.org/licenses/by-sa/3.0/)** license. Everyone is allowed to **share, use, copy and adapt** the text as long as **the author and Store norske leksikon** continues to be credited and the article retains the same free license for further use. | [Meta](https://meta.snl.no/fri_gjenbruk)
-        | `begrenset gjenbruk/begrænset genbrug` | You **can't reuse, republish, or adapt** the article without first obtaining the author's permission.| [Meta](https://meta.snl.no/begrenset_gjenbruk)
-        
-        ## Overview of sites/zones
-        ### SNL
-        |     code    |       Website       |   Note 
-        | --- | --- | --- |
-        |     `snl`     |   https://snl.no/   | Default
-        |     `nbl`     | https://nbl.snl.no/ |        
-        |     `sml`     | https://sml.snl.no/ |        
-        |     `nkl`     | https://nkl.snl.no/ |        
-        | `prototyping` |          -          | Unstable - for SNL
-        
-        ### LEX
-        |     code    |       Website       |   Note 
-        | --- | --- | --- |
-        |     `dsd`     |   https://denstoredanske.lex.dk/   | 
-        |     `dlh`     | https://dansklitteraturshistorie.lex.dk/ |        
-        |     `dbl`     | https://biografiskleksikon.lex.dk/ |        
-        |     `gtl`     | https://teaterleksikon.lex.dk/ |
-        |     `nm`     | https://mytologi.lex.dk/ |
-        |     `do`     | https://danmarksoldtid.lex.dk/ |
-        |     `sl`     | https://symbolleksikon.lex.dk/ |
-        |     `dh`     | https://danmarkshistorien.lex.dk/ |
-        |     `hob`     | https://bornelitteratur.lex.dk/ |
-        |     `pd`     | https://pattedyratlas.lex.dk/ |
-        | `prototyping-lex` |          -          | Unstable - for LEX pages
-        
-        ## Query
-        ### Easy Query
-        - Main documentation: [API-dokumentasjon](https://meta.snl.no/API-dokumentasjon)
-        
-        ```python
-        import snldata
-        
-        R = snldata.SnlSession()
-        R.search(query="Ole Ivars", best=True) #Pick the one with the best rank
-        print(R.url)
-        
-        ```
-        Outputs: `https://snl.no/Ole_Ivars`
-        
-        ```python
-        import snldata
-        
-        R = snldata.SnlSession()
-        R.search(query="Ole Ivars") #Pick the three best results
-        for val in R.json:
-            print(val["simple"] #Summery for each index
-        
-        ```
-        Outputs: 
-        ```
-        0. Ole Ivars (rank 576.6): Ole Ivars er et norsk danseband fra Hamar.
-        1. Spellemannprisen (rank 25.9): Spellemannprisen er den norske platebransjens årlige prisutdeling for å stimulere og markere plateproduksjonen i Norge.
-        2. danseband (rank 25.1): Danseband, ensemble som spiller til dans, betegner i dag vanligvis en instrumentbesetning som i pop og rock (vokal, elektrisk gitar og bass, keyboards, trommer, eventuelt også saksofon eller andre blåsere).
-        ###Explaining of the values:
-        <index of the json file> <title> (rank <rank id>): <first sentence>
-        ```
-        Pick the article you want from the example above:
-        ```python
-        R._get(1)
-        print(R.title)
-        ```
-        Outputs: `Spellemannprisen`
-        
-        ```python
-        import snldata
-        
-        R = snldata.SnlSession()
-        R.search(zone='dsd', query="Python", best=True)  #Pick the one with the best rank
-        print(R.url)
-        ```
-        Outputs: `https://denstoredanske.lex.dk/Python`
-        
-        ### Advance Query (best for prototyping api)
-        - Main documentation: [API-dokumentasjon - prototyping](https://meta.snl.no/API-dokumentasjon_-_prototyping)
-        
-        ```python
-        import snldata
-        
-        R = snldata.SnlSession()
-        R.searchV2({"encyclopedia": "snl", "query": "dr. dre", "limit": 3, "offset": 0 }, zone="prototyping", best=True)
-        print(R.title)
-        
-        ```
-        Outputs: `Dr. Dre`
-        
-        ```python
-        import snldata
-        
-        R = snldata.SnlSession()
-        R.searchV2({"encyclopedia": "snl", "query": "dr. dre", "limit": 3, "offset": 0 }, zone="prototyping")
-        i = 0
-        for val in R.json:
-            print('{}. {}: {}'.format(i, val['headword'], val["query_quality_explain"]))
-            i += 1
-        
-        ```
-        Outputs:
-        ```
-        0. Dr. Dre: The search string is equal to the article's headword and there is no further clarification
-        1. hiphop: Match on article text or part of title
-        2. Eminem: Match on article text or part of title
-        ###Explaining of the values: (the prototyping api allows you to send a lot of parametres)
-        <index of the json file> <title>: <rank as text>
-        ```
-        Pick the article you want from the example above:
-        ```python
-        R._get(1)
-        print("Title: {}, Created: {}".format(R.title, R.created_at))
-        ```
-        Outputs: `Title: hiphop, Created: 2009-02-14T05:15:20.546+01:00`
-        ### No result
-        If the API returns no results, `.json` will be given a empty list.
-        ```python
-        import snldata
-        
-        R = snldata.SnlSession()
-        R.search(zone='dsd', query="asdadasdasdad", best=True)  #Pick the one with the best rank
-        print(R.json)
-        ```
-        Outputs: `[]`
-        
-        <sup>All of the examples uses text that is [CC-BY-SA-3.0](https://creativecommons.org/licenses/by-sa/3.0). By at least one of the following authors: Henrik Dvergsdal, Jon Vidar Bergan, and Audun Kjus Aahlin. Read more about the license: [fri gjenbruk](https://meta.snl.no/fri_gjenbruk).</sup>
-        
-        ## To-do
-        - [ ] Fully support taxonomy
-        - [X] When zero results, return somthing to tell the user there is no result.
-        
-        ## Reporting Issues
-        
-        If you have suggestions, bugs or other issues specific to this library, file them [here](https://github.com/DiFronzo/SnlData/issues). Or just send me a pull request.
-        
 Keywords: API SNL DSD
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Norwegian
 Classifier: Natural Language :: Danish
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<p align="center">
+  <a href="https://github.com/DiFronzo/snldata"><img alt="Logo" width="500" height="300" src="https://snldata.readthedocs.io/en/latest/_static/snldata_logo.svg"></a>
+</p>
+<p align="center">
+  <a href="https://github.com/DiFronzo/snldata/releases" target="_blank"><img src="https://img.shields.io/badge/SnlData-1.1.2-blue" alt="SnlData version" /></a>
+  <a href="https://github.com/DiFronzo/snldata/actions"><img alt="Actions Status" src="https://github.com/DiFronzo/SnlData/actions/workflows/test.yml/badge.svg"></a>
+  <a href="https://snldata.readthedocs.io/en/latest/?badge=latest"><img alt="Documentation Status" src="https://readthedocs.org/projects/snldata/badge/?version=latest"></a>
+  <a href="https://codecov.io/gh/DiFronzo/SnlData"><img alt="Coverage Status" src="https://codecov.io/gh/DiFronzo/SnlData/branch/master/graph/badge.svg"></a>
+  <a href="https://app.travis-ci.com/DiFronzo/SnlData"><img alt="Build Status" src="https://api.travis-ci.com/DiFronzo/SnlData.svg?branch=master"></a>	
+  <a href="https://github.com/DiFronzo/SnlData/blob/master/LICENSE"><img alt="License: GPLv3" src="https://img.shields.io/badge/License-GPLv3-blue.svg"></a>
+  <a href="https://pepy.tech/project/snldata"><img alt="Downloads" src="https://pepy.tech/badge/snldata"></a>
+  <a href="https://pypi.org/project/snldata/"><img alt="PyPI" src="https://img.shields.io/pypi/v/snldata"></a>
+  <h4>A lightweight Python library for Store Norske Leksikon and Lex.dk/Den Store Danske APIs</h4>
+</p>
+
+## Installation
+
+    pip3 install snldata
+
+## Quick Start
+Raw JSON
+```python
+import snldata
+
+R = snldata.SnlSession()
+R.search(query="fortolket programmeringsspråk", best=True) #Pick the one with the best rank
+print(R.json)
+
+```
+Outputs: the JSON object
+```
+{
+	"title": "fortolket programmeringsspråk",
+	"url": "http://snl.no/fortolket_programmeringsspr%C3%A5k",
+	"subject_url": "http://snl.no/.taxonomy/3689",
+	"subject_title": "Programmering",
+	"xhtml_body": "\u003cdiv\u003e\r\n\u003cp\u003eprogrammeringsspråk som ikke blir kompilert til objekt- eller maskinkode, men fortolket av et eget program på vertsmaskinen.\u003c/p\u003e\r\n\u003cp\u003eFordelen med slike språk er at man kan lage programmer som kan gjøre på mange forskjellige \u003ca class=\"crossref\" href=\"https://snl.no/datamaskin\"\u003edatamaskiner\u003c/a\u003e og \u003ca class=\"crossref\" href=\"https://snl.no/operativsystem\"\u003eoperativsystemer\u003c/a\u003e uten å skreddersy dem for hver enkelt plattform.\u003c/p\u003e\r\n\u003cp\u003eEksempler på fortolkede språk:\u003c/p\u003e\r\n\u003cul\u003e\r\n\u003cli\u003e\u003ca class=\"crossref\" href=\"https://snl.no/Python_-_programmeringsspr%C3%A5k\"\u003ePython\u003c/a\u003e\u003c/li\u003e\r\n\u003cli\u003eJavascript\u003c/li\u003e\r\n\u003cli\u003e\u003ca class=\"crossref\" href=\"https://snl.no/Perl_-_IT\"\u003ePHP\u003c/a\u003e\u003c/li\u003e\r\n\u003cli\u003e\u003ca class=\"crossref\" href=\"https://snl.no/Perl_-_IT\"\u003ePerl\u003c/a\u003e\u003c/li\u003e\r\n\u003c/ul\u003e\r\n\u003c/div\u003e",
+	"created_at": "2017-12-12T10:34:18.189+01:00",
+	"changed_at": "2017-12-12T10:38:37.626+01:00",
+	"license_name": "fri",
+	"metadata_license_name": "fri",
+	"metadata": {
+		"lastname": "",
+		"firstname": ""
+	},
+	"authors": [{
+		"full_name": "Henrik Dvergsdal"
+	}],
+	"images": []
+}
+```
+## Licenses for content from Store Norske Leksikon and Lex.dk 
+| Licence | Description | Read more
+| --- | --- | --- |
+| `fri` | [Creative Commons](https://creativecommons.org/) **[CC-BY-SA-3.0](https://creativecommons.org/licenses/by-sa/3.0/)** license. Everyone is allowed to **share, use, copy and adapt** the text as long as **the author and Store norske leksikon** continues to be credited and the article retains the same free license for further use. | [SNL](https://meta.snl.no/fri_gjenbruk) [LEX](https://denstoredanske.lex.dk/.licenses/free)
+| `begrenset gjenbruk/begrænset genbrug` | You **can't reuse, republish, or adapt** the article without first obtaining the author's permission.| [SNL](https://meta.snl.no/begrenset_gjenbruk) [LEX](https://denstoredanske.lex.dk/.licenses/restricted)
+
+## Overview of sites/zones
+### SNL
+|     code    |       Website       |   Note 
+| --- | --- | --- |
+|     `snl`     |   https://snl.no/   | Default
+|     `nbl`     | https://nbl.snl.no/ |        
+|     `sml`     | https://sml.snl.no/ |        
+|     `nkl`     | https://nkl.snl.no/ |        
+| <s>`prototyping`</s> |          -          | <s>Unstable - for SNL</s>
+
+### LEX
+|     code    |       Website       |   Note 
+| --- | --- | --- |
+|     `dsd`     |   https://denstoredanske.lex.dk/   | 
+|     `dlh`     | https://dansklitteraturshistorie.lex.dk/ |        
+|     `dbl`     | https://biografiskleksikon.lex.dk/ |        
+|     `gtl`     | https://teaterleksikon.lex.dk/ |
+|     `nm`     | https://mytologi.lex.dk/ |
+|     `do`     | https://danmarksoldtid.lex.dk/ |
+|     `sl`     | https://symbolleksikon.lex.dk/ |
+|     `dh`     | https://danmarkshistorien.lex.dk/ |
+|     `hob`     | https://bornelitteratur.lex.dk/ |
+|     `pd`     | https://pattedyratlas.lex.dk/ |
+|     `nid`     | https://naturenidanmark.lex.dk/ |
+|     `trap`     | https://trap.lex.dk/ |
+| <s>`prototyping-lex`</s> |          -          | <s>Unstable - for LEX pages</s>
+
+## Query
+### Easy Query
+- Main documentation (SNL): [API-dokumentasjon](https://meta.snl.no/API-dokumentasjon)
+
+```python
+import snldata
+
+R = snldata.SnlSession()
+R.search(query="Ole Ivars", best=True) #Pick the one with the best rank
+print(R.url)
+
+```
+Outputs: `https://snl.no/Ole_Ivars`
+
+```python
+import snldata
+
+R = snldata.SnlSession()
+R.search(query="Ole Ivars") #Pick the three best results
+for val in R.json:
+    print(val["simple"]) #Summery for each index
+
+```
+Outputs: 
+```
+0. Ole Ivars (rank 576.6): Ole Ivars er et norsk danseband fra Hamar.
+1. Spellemannprisen (rank 25.9): Spellemannprisen er den norske platebransjens årlige prisutdeling for å stimulere og markere plateproduksjonen i Norge.
+2. danseband (rank 25.1): Danseband, ensemble som spiller til dans, betegner i dag vanligvis en instrumentbesetning som i pop og rock (vokal, elektrisk gitar og bass, keyboards, trommer, eventuelt også saksofon eller andre blåsere).
+###Explaining of the values:
+<index of the json file> <title> (rank <rank id>): <first sentence>
+```
+Pick the article you want from the example above:
+```python
+R._get(1)
+print(R.title)
+```
+Outputs: `Spellemannprisen`
+
+```python
+import snldata
+
+R = snldata.SnlSession()
+R.search(zone='dsd', query="Python", best=True)  #Pick the one with the best rank
+print(R.url)
+```
+Outputs: `https://denstoredanske.lex.dk/Python`
+
+### Advance Query (best for prototyping api)
+- Main documentation (SNL): [API-dokumentasjon - prototyping](https://meta.snl.no/API-dokumentasjon_-_prototyping)
+
+**The prototyping API endpoint has been removed as of May 2023.**
+
+### No result
+If the API returns no results, `.json` will be given a empty list.
+```python
+import snldata
+
+R = snldata.SnlSession()
+R.search(zone='dsd', query="asdadasdasdad", best=True)  #Pick the one with the best rank
+print(R.json)
+```
+Outputs: `{}`
+
+```python
+import snldata
+
+R = snldata.SnlSession()
+R.search(zone='dsd', query="jdfhdskjfhsjkdfhksdfh") #Pick the three best results, but there are none
+R._get(0)
+print(R.json)
+```
+Outputs: `{}`
+
+<sup>All of the examples uses text that is [CC-BY-SA-3.0](https://creativecommons.org/licenses/by-sa/3.0). By at least one of the following authors: Henrik Dvergsdal, Jon Vidar Bergan, and Audun Kjus Aahlin. Read more about the license: [fri gjenbruk](https://meta.snl.no/fri_gjenbruk).</sup>
+
+## To-do
+- [ ] Fully support taxonomy
+- [ ] Support for ".recent-activities" to JSON.
+- [X] When zero results, return empty dict to tell the user there is no result.
+
+## Reporting Issues
+If you have suggestions, bugs or other issues specific to this library, file them [here](https://github.com/DiFronzo/SnlData/issues). Or just send me a pull request.
```

#### html2text {}

```diff
@@ -1,17 +1,26 @@
-Metadata-Version: 2.1 Name: SnlData Version: 1.1.0 Summary: A lightweight
-Python library for Store Norske Leksikon and Lex.dk APIs. Home-page: https://
-github.com/DiFronzo/SnlData Author: DiFronzo Author-email: root@vfiles.no
-License: GPLv3 Description:
+Metadata-Version: 2.1 Name: SnlData Version: 1.1.2 Summary: A lightweight
+Python library for Store Norske Leksikon and Lex.dk/Den Store Danske APIs.
+Home-page: https://github.com/DiFronzo/SnlData Author: DiFronzo Author-email:
+root@vfiles.no License: GPLv3 Keywords: API SNL DSD Classifier: Development
+Status :: 5 - Production/Stable Classifier: Environment :: Console Classifier:
+Intended Audience :: Developers Classifier: Natural Language :: Norwegian
+Classifier: Natural Language :: Danish Classifier: License :: OSI Approved ::
+GNU General Public License v3 (GPLv3) Classifier: Operating System :: OS
+Independent Classifier: Programming Language :: Python Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3 :: Only Classifier: Topic ::
+Software Development :: Libraries :: Python Modules Requires-Python: >=3.6
+Description-Content-Type: text/markdown License-File: LICENSE
                                     [Logo]
- [Actions_Status] [Documentation_Status] [https://app.fossa.com/api/projects/
-git%2Bgithub.com%2FDiFronzo%2FSnlData.svg?type=small] [Coverage_Status] [Build
-                   Status] [License:_MIT] [Downloads] [PyPI]
-*** A lightweight Python library for Store Norske Leksikon and Lex.dk APIs ***
-## Installation pip install snldata ## Quick Start Raw JSON ```python import
+ [SnlData_version] [Actions_Status] [Documentation_Status] [Coverage_Status]
+              [Build_Status] [License:_GPLv3] [Downloads] [PyPI]
+*** A lightweight Python library for Store Norske Leksikon and Lex.dk/Den Store
+Danske APIs ***
+## Installation pip3 install snldata ## Quick Start Raw JSON ```python import
 snldata R = snldata.SnlSession() R.search(query="fortolket
 programmeringssprÃ¥k", best=True) #Pick the one with the best rank print
 (R.json) ``` Outputs: the JSON object ``` { "title": "fortolket
 programmeringssprÃ¥k", "url": "http://snl.no/
 fortolket_programmeringsspr%C3%A5k", "subject_url": "http://snl.no/.taxonomy/
 3689", "subject_title": "Programmering", "xhtml_body":
 "\u003cdiv\u003e\r\n\u003cp\u003eprogrammeringssprÃ¥k som ikke blir kompilert
@@ -35,75 +44,59 @@
 { "lastname": "", "firstname": "" }, "authors": [{ "full_name": "Henrik
 Dvergsdal" }], "images": [] } ``` ## Licenses for content from Store Norske
 Leksikon and Lex.dk | Licence | Description | Read more | --- | --- | --- | |
 `fri` | [Creative Commons](https://creativecommons.org/) **[CC-BY-SA-3.0]
 (https://creativecommons.org/licenses/by-sa/3.0/)** license. Everyone is
 allowed to **share, use, copy and adapt** the text as long as **the author and
 Store norske leksikon** continues to be credited and the article retains the
-same free license for further use. | [Meta](https://meta.snl.no/fri_gjenbruk) |
-`begrenset gjenbruk/begrÃ¦nset genbrug` | You **can't reuse, republish, or
-adapt** the article without first obtaining the author's permission.| [Meta]
-(https://meta.snl.no/begrenset_gjenbruk) ## Overview of sites/zones ### SNL |
-code | Website | Note | --- | --- | --- | | `snl` | https://snl.no/ | Default |
-`nbl` | https://nbl.snl.no/ | | `sml` | https://sml.snl.no/ | | `nkl` | https:/
-/nkl.snl.no/ | | `prototyping` | - | Unstable - for SNL ### LEX | code |
-Website | Note | --- | --- | --- | | `dsd` | https://denstoredanske.lex.dk/ | |
-`dlh` | https://dansklitteraturshistorie.lex.dk/ | | `dbl` | https://
-biografiskleksikon.lex.dk/ | | `gtl` | https://teaterleksikon.lex.dk/ | | `nm`
-| https://mytologi.lex.dk/ | | `do` | https://danmarksoldtid.lex.dk/ | | `sl` |
-https://symbolleksikon.lex.dk/ | | `dh` | https://danmarkshistorien.lex.dk/ | |
-`hob` | https://bornelitteratur.lex.dk/ | | `pd` | https://
-pattedyratlas.lex.dk/ | | `prototyping-lex` | - | Unstable - for LEX pages ##
-Query ### Easy Query - Main documentation: [API-dokumentasjon](https://
-meta.snl.no/API-dokumentasjon) ```python import snldata R = snldata.SnlSession
-() R.search(query="Ole Ivars", best=True) #Pick the one with the best rank
-print(R.url) ``` Outputs: `https://snl.no/Ole_Ivars` ```python import snldata R
-= snldata.SnlSession() R.search(query="Ole Ivars") #Pick the three best results
-for val in R.json: print(val["simple"] #Summery for each index ``` Outputs: ```
-0. Ole Ivars (rank 576.6): Ole Ivars er et norsk danseband fra Hamar. 1.
-Spellemannprisen (rank 25.9): Spellemannprisen er den norske platebransjens
-Ã¥rlige prisutdeling for Ã¥ stimulere og markere plateproduksjonen i Norge. 2.
-danseband (rank 25.1): Danseband, ensemble som spiller til dans, betegner i dag
-vanligvis en instrumentbesetning som i pop og rock (vokal, elektrisk gitar og
-bass, keyboards, trommer, eventuelt ogsÃ¥ saksofon eller andre blÃ¥sere).
+same free license for further use. | [SNL](https://meta.snl.no/fri_gjenbruk)
+[LEX](https://denstoredanske.lex.dk/.licenses/free) | `begrenset gjenbruk/
+begrÃ¦nset genbrug` | You **can't reuse, republish, or adapt** the article
+without first obtaining the author's permission.| [SNL](https://meta.snl.no/
+begrenset_gjenbruk) [LEX](https://denstoredanske.lex.dk/.licenses/restricted)
+## Overview of sites/zones ### SNL | code | Website | Note | --- | --- | --- |
+| `snl` | https://snl.no/ | Default | `nbl` | https://nbl.snl.no/ | | `sml` |
+https://sml.snl.no/ | | `nkl` | https://nkl.snl.no/ | | `prototyping` | - |
+Unstable - for SNL ### LEX | code | Website | Note | --- | --- | --- | | `dsd`
+| https://denstoredanske.lex.dk/ | | `dlh` | https://
+dansklitteraturshistorie.lex.dk/ | | `dbl` | https://biografiskleksikon.lex.dk/
+| | `gtl` | https://teaterleksikon.lex.dk/ | | `nm` | https://mytologi.lex.dk/
+| | `do` | https://danmarksoldtid.lex.dk/ | | `sl` | https://
+symbolleksikon.lex.dk/ | | `dh` | https://danmarkshistorien.lex.dk/ | | `hob` |
+https://bornelitteratur.lex.dk/ | | `pd` | https://pattedyratlas.lex.dk/ | |
+`nid` | https://naturenidanmark.lex.dk/ | | `trap` | https://trap.lex.dk/ | |
+`prototyping-lex` | - | Unstable - for LEX pages ## Query ### Easy Query - Main
+documentation (SNL): [API-dokumentasjon](https://meta.snl.no/API-dokumentasjon)
+```python import snldata R = snldata.SnlSession() R.search(query="Ole Ivars",
+best=True) #Pick the one with the best rank print(R.url) ``` Outputs: `https://
+snl.no/Ole_Ivars` ```python import snldata R = snldata.SnlSession() R.search
+(query="Ole Ivars") #Pick the three best results for val in R.json: print(val
+["simple"]) #Summery for each index ``` Outputs: ``` 0. Ole Ivars (rank 576.6):
+Ole Ivars er et norsk danseband fra Hamar. 1. Spellemannprisen (rank 25.9):
+Spellemannprisen er den norske platebransjens Ã¥rlige prisutdeling for Ã¥
+stimulere og markere plateproduksjonen i Norge. 2. danseband (rank 25.1):
+Danseband, ensemble som spiller til dans, betegner i dag vanligvis en
+instrumentbesetning som i pop og rock (vokal, elektrisk gitar og bass,
+keyboards, trommer, eventuelt ogsÃ¥ saksofon eller andre blÃ¥sere).
 ###Explaining of the values:
 ):  ``` Pick the article you want from the example above: ```python R._get(1)
 print(R.title) ``` Outputs: `Spellemannprisen` ```python import snldata R =
 snldata.SnlSession() R.search(zone='dsd', query="Python", best=True) #Pick the
 one with the best rank print(R.url) ``` Outputs: `https://
 denstoredanske.lex.dk/Python` ### Advance Query (best for prototyping api) -
-Main documentation: [API-dokumentasjon - prototyping](https://meta.snl.no/API-
-dokumentasjon_-_prototyping) ```python import snldata R = snldata.SnlSession()
-R.searchV2({"encyclopedia": "snl", "query": "dr. dre", "limit": 3, "offset": 0
-}, zone="prototyping", best=True) print(R.title) ``` Outputs: `Dr. Dre`
-```python import snldata R = snldata.SnlSession() R.searchV2({"encyclopedia":
-"snl", "query": "dr. dre", "limit": 3, "offset": 0 }, zone="prototyping") i = 0
-for val in R.json: print('{}. {}: {}'.format(i, val['headword'], val
-["query_quality_explain"])) i += 1 ``` Outputs: ``` 0. Dr. Dre: The search
-string is equal to the article's headword and there is no further clarification
-1. hiphop: Match on article text or part of title 2. Eminem: Match on article
-text or part of title ###Explaining of the values: (the prototyping api allows
-you to send a lot of parametres)
- ``` Pick the article you want from the example above: ```python R._get(1)
-print("Title: {}, Created: {}".format(R.title, R.created_at)) ``` Outputs:
-`Title: hiphop, Created: 2009-02-14T05:15:20.546+01:00` ### No result If the
-API returns no results, `.json` will be given a empty list. ```python import
-snldata R = snldata.SnlSession() R.search(zone='dsd', query="asdadasdasdad",
-best=True) #Pick the one with the best rank print(R.json) ``` Outputs: `[]` All
-of the examples uses text that is [CC-BY-SA-3.0](https://creativecommons.org/
-licenses/by-sa/3.0). By at least one of the following authors: Henrik
-Dvergsdal, Jon Vidar Bergan, and Audun Kjus Aahlin. Read more about the
-license: [fri gjenbruk](https://meta.snl.no/fri_gjenbruk). ## To-do - [ ] Fully
-support taxonomy - [X] When zero results, return somthing to tell the user
-there is no result. ## Reporting Issues If you have suggestions, bugs or other
-issues specific to this library, file them [here](https://github.com/DiFronzo/
-SnlData/issues). Or just send me a pull request. Keywords: API SNL DSD
-Platform: UNKNOWN Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: Norwegian Classifier: Natural Language ::
-Danish Classifier: License :: OSI Approved :: GNU General Public License v3
-(GPLv3) Classifier: Operating System :: OS Independent Classifier: Programming
-Language :: Python Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3 ::
-Only Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6 Description-Content-Type: text/markdown
+Main documentation (SNL): [API-dokumentasjon - prototyping](https://
+meta.snl.no/API-dokumentasjon_-_prototyping) **The prototyping API endpoint has
+been removed as of May 2023.** ### No result If the API returns no results,
+`.json` will be given a empty list. ```python import snldata R =
+snldata.SnlSession() R.search(zone='dsd', query="asdadasdasdad", best=True)
+#Pick the one with the best rank print(R.json) ``` Outputs: `{}` ```python
+import snldata R = snldata.SnlSession() R.search(zone='dsd',
+query="jdfhdskjfhsjkdfhksdfh") #Pick the three best results, but there are none
+R._get(0) print(R.json) ``` Outputs: `{}` All of the examples uses text that is
+[CC-BY-SA-3.0](https://creativecommons.org/licenses/by-sa/3.0). By at least one
+of the following authors: Henrik Dvergsdal, Jon Vidar Bergan, and Audun Kjus
+Aahlin. Read more about the license: [fri gjenbruk](https://meta.snl.no/
+fri_gjenbruk). ## To-do - [ ] Fully support taxonomy - [ ] Support for
+".recent-activities" to JSON. - [X] When zero results, return empty dict to
+tell the user there is no result. ## Reporting Issues If you have suggestions,
+bugs or other issues specific to this library, file them [here](https://
+github.com/DiFronzo/SnlData/issues). Or just send me a pull request.
```

### Comparing `SnlData-1.1.0/README.md` & `SnlData-1.1.2/SnlData.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,50 @@
+Metadata-Version: 2.1
+Name: SnlData
+Version: 1.1.2
+Summary: A lightweight Python library for Store Norske Leksikon and Lex.dk/Den Store Danske APIs.
+Home-page: https://github.com/DiFronzo/SnlData
+Author: DiFronzo
+Author-email: root@vfiles.no
+License: GPLv3
+Keywords: API SNL DSD
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: Norwegian
+Classifier: Natural Language :: Danish
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <p align="center">
   <a href="https://github.com/DiFronzo/snldata"><img alt="Logo" width="500" height="300" src="https://snldata.readthedocs.io/en/latest/_static/snldata_logo.svg"></a>
 </p>
 <p align="center">
-  <a href="https://github.com/DiFronzo/snldata/actions"><img alt="Actions Status" src="https://github.com/DiFronzo/SnlData/workflows/Test/badge.svg"></a>
+  <a href="https://github.com/DiFronzo/snldata/releases" target="_blank"><img src="https://img.shields.io/badge/SnlData-1.1.2-blue" alt="SnlData version" /></a>
+  <a href="https://github.com/DiFronzo/snldata/actions"><img alt="Actions Status" src="https://github.com/DiFronzo/SnlData/actions/workflows/test.yml/badge.svg"></a>
   <a href="https://snldata.readthedocs.io/en/latest/?badge=latest"><img alt="Documentation Status" src="https://readthedocs.org/projects/snldata/badge/?version=latest"></a>
-	<a href="https://app.fossa.com/projects/git%2Bgithub.com%2FDiFronzo%2FSnlData?ref=badge_small" alt="FOSSA Status"><img src="https://app.fossa.com/api/projects/git%2Bgithub.com%2FDiFronzo%2FSnlData.svg?type=small"/></a>
   <a href="https://codecov.io/gh/DiFronzo/SnlData"><img alt="Coverage Status" src="https://codecov.io/gh/DiFronzo/SnlData/branch/master/graph/badge.svg"></a>
-  <a href="https://travis-ci.com/DiFronzo/SnlData"><img alt="Build Status" src="https://api.travis-ci.com/DiFronzo/SnlData.svg?branch=master"></a>	
-  <a href="https://github.com/DiFronzo/SnlData/blob/master/LICENSE"><img alt="License: MIT" src="https://snldata.readthedocs.io/en/latest/_static/license.svg"></a>
+  <a href="https://app.travis-ci.com/DiFronzo/SnlData"><img alt="Build Status" src="https://api.travis-ci.com/DiFronzo/SnlData.svg?branch=master"></a>	
+  <a href="https://github.com/DiFronzo/SnlData/blob/master/LICENSE"><img alt="License: GPLv3" src="https://img.shields.io/badge/License-GPLv3-blue.svg"></a>
   <a href="https://pepy.tech/project/snldata"><img alt="Downloads" src="https://pepy.tech/badge/snldata"></a>
   <a href="https://pypi.org/project/snldata/"><img alt="PyPI" src="https://img.shields.io/pypi/v/snldata"></a>
-  <h4>A lightweight Python library for Store Norske Leksikon and Lex.dk APIs</h4>
+  <h4>A lightweight Python library for Store Norske Leksikon and Lex.dk/Den Store Danske APIs</h4>
 </p>
 
 ## Installation
 
-    pip install snldata
+    pip3 install snldata
 
 ## Quick Start
 Raw JSON
 ```python
 import snldata
 
 R = snldata.SnlSession()
@@ -48,45 +73,47 @@
 	}],
 	"images": []
 }
 ```
 ## Licenses for content from Store Norske Leksikon and Lex.dk 
 | Licence | Description | Read more
 | --- | --- | --- |
-| `fri` | [Creative Commons](https://creativecommons.org/) **[CC-BY-SA-3.0](https://creativecommons.org/licenses/by-sa/3.0/)** license. Everyone is allowed to **share, use, copy and adapt** the text as long as **the author and Store norske leksikon** continues to be credited and the article retains the same free license for further use. | [Meta](https://meta.snl.no/fri_gjenbruk)
-| `begrenset gjenbruk/begrænset genbrug` | You **can't reuse, republish, or adapt** the article without first obtaining the author's permission.| [Meta](https://meta.snl.no/begrenset_gjenbruk)
+| `fri` | [Creative Commons](https://creativecommons.org/) **[CC-BY-SA-3.0](https://creativecommons.org/licenses/by-sa/3.0/)** license. Everyone is allowed to **share, use, copy and adapt** the text as long as **the author and Store norske leksikon** continues to be credited and the article retains the same free license for further use. | [SNL](https://meta.snl.no/fri_gjenbruk) [LEX](https://denstoredanske.lex.dk/.licenses/free)
+| `begrenset gjenbruk/begrænset genbrug` | You **can't reuse, republish, or adapt** the article without first obtaining the author's permission.| [SNL](https://meta.snl.no/begrenset_gjenbruk) [LEX](https://denstoredanske.lex.dk/.licenses/restricted)
 
 ## Overview of sites/zones
 ### SNL
 |     code    |       Website       |   Note 
 | --- | --- | --- |
 |     `snl`     |   https://snl.no/   | Default
 |     `nbl`     | https://nbl.snl.no/ |        
 |     `sml`     | https://sml.snl.no/ |        
 |     `nkl`     | https://nkl.snl.no/ |        
-| `prototyping` |          -          | Unstable - for SNL
+| <s>`prototyping`</s> |          -          | <s>Unstable - for SNL</s>
 
 ### LEX
 |     code    |       Website       |   Note 
 | --- | --- | --- |
 |     `dsd`     |   https://denstoredanske.lex.dk/   | 
 |     `dlh`     | https://dansklitteraturshistorie.lex.dk/ |        
 |     `dbl`     | https://biografiskleksikon.lex.dk/ |        
 |     `gtl`     | https://teaterleksikon.lex.dk/ |
 |     `nm`     | https://mytologi.lex.dk/ |
 |     `do`     | https://danmarksoldtid.lex.dk/ |
 |     `sl`     | https://symbolleksikon.lex.dk/ |
 |     `dh`     | https://danmarkshistorien.lex.dk/ |
 |     `hob`     | https://bornelitteratur.lex.dk/ |
 |     `pd`     | https://pattedyratlas.lex.dk/ |
-| `prototyping-lex` |          -          | Unstable - for LEX pages
+|     `nid`     | https://naturenidanmark.lex.dk/ |
+|     `trap`     | https://trap.lex.dk/ |
+| <s>`prototyping-lex`</s> |          -          | <s>Unstable - for LEX pages</s>
 
 ## Query
 ### Easy Query
-- Main documentation: [API-dokumentasjon](https://meta.snl.no/API-dokumentasjon)
+- Main documentation (SNL): [API-dokumentasjon](https://meta.snl.no/API-dokumentasjon)
 
 ```python
 import snldata
 
 R = snldata.SnlSession()
 R.search(query="Ole Ivars", best=True) #Pick the one with the best rank
 print(R.url)
@@ -96,15 +123,15 @@
 
 ```python
 import snldata
 
 R = snldata.SnlSession()
 R.search(query="Ole Ivars") #Pick the three best results
 for val in R.json:
-    print(val["simple"] #Summery for each index
+    print(val["simple"]) #Summery for each index
 
 ```
 Outputs: 
 ```
 0. Ole Ivars (rank 576.6): Ole Ivars er et norsk danseband fra Hamar.
 1. Spellemannprisen (rank 25.9): Spellemannprisen er den norske platebransjens årlige prisutdeling for å stimulere og markere plateproduksjonen i Norge.
 2. danseband (rank 25.1): Danseband, ensemble som spiller til dans, betegner i dag vanligvis en instrumentbesetning som i pop og rock (vokal, elektrisk gitar og bass, keyboards, trommer, eventuelt også saksofon eller andre blåsere).
@@ -124,64 +151,41 @@
 R = snldata.SnlSession()
 R.search(zone='dsd', query="Python", best=True)  #Pick the one with the best rank
 print(R.url)
 ```
 Outputs: `https://denstoredanske.lex.dk/Python`
 
 ### Advance Query (best for prototyping api)
-- Main documentation: [API-dokumentasjon - prototyping](https://meta.snl.no/API-dokumentasjon_-_prototyping)
+- Main documentation (SNL): [API-dokumentasjon - prototyping](https://meta.snl.no/API-dokumentasjon_-_prototyping)
 
-```python
-import snldata
-
-R = snldata.SnlSession()
-R.searchV2({"encyclopedia": "snl", "query": "dr. dre", "limit": 3, "offset": 0 }, zone="prototyping", best=True)
-print(R.title)
-
-```
-Outputs: `Dr. Dre`
+**The prototyping API endpoint has been removed as of May 2023.**
 
+### No result
+If the API returns no results, `.json` will be given a empty list.
 ```python
 import snldata
 
 R = snldata.SnlSession()
-R.searchV2({"encyclopedia": "snl", "query": "dr. dre", "limit": 3, "offset": 0 }, zone="prototyping")
-i = 0
-for val in R.json:
-    print('{}. {}: {}'.format(i, val['headword'], val["query_quality_explain"]))
-    i += 1
-
-```
-Outputs:
-```
-0. Dr. Dre: The search string is equal to the article's headword and there is no further clarification
-1. hiphop: Match on article text or part of title
-2. Eminem: Match on article text or part of title
-###Explaining of the values: (the prototyping api allows you to send a lot of parametres)
-<index of the json file> <title>: <rank as text>
-```
-Pick the article you want from the example above:
-```python
-R._get(1)
-print("Title: {}, Created: {}".format(R.title, R.created_at))
+R.search(zone='dsd', query="asdadasdasdad", best=True)  #Pick the one with the best rank
+print(R.json)
 ```
-Outputs: `Title: hiphop, Created: 2009-02-14T05:15:20.546+01:00`
-### No result
-If the API returns no results, `.json` will be given a empty list.
+Outputs: `{}`
+
 ```python
 import snldata
 
 R = snldata.SnlSession()
-R.search(zone='dsd', query="asdadasdasdad", best=True)  #Pick the one with the best rank
+R.search(zone='dsd', query="jdfhdskjfhsjkdfhksdfh") #Pick the three best results, but there are none
+R._get(0)
 print(R.json)
 ```
-Outputs: `[]`
+Outputs: `{}`
 
 <sup>All of the examples uses text that is [CC-BY-SA-3.0](https://creativecommons.org/licenses/by-sa/3.0). By at least one of the following authors: Henrik Dvergsdal, Jon Vidar Bergan, and Audun Kjus Aahlin. Read more about the license: [fri gjenbruk](https://meta.snl.no/fri_gjenbruk).</sup>
 
 ## To-do
 - [ ] Fully support taxonomy
-- [X] When zero results, return somthing to tell the user there is no result.
+- [ ] Support for ".recent-activities" to JSON.
+- [X] When zero results, return empty dict to tell the user there is no result.
 
 ## Reporting Issues
-
 If you have suggestions, bugs or other issues specific to this library, file them [here](https://github.com/DiFronzo/SnlData/issues). Or just send me a pull request.
```

#### html2text {}

```diff
@@ -1,13 +1,26 @@
+Metadata-Version: 2.1 Name: SnlData Version: 1.1.2 Summary: A lightweight
+Python library for Store Norske Leksikon and Lex.dk/Den Store Danske APIs.
+Home-page: https://github.com/DiFronzo/SnlData Author: DiFronzo Author-email:
+root@vfiles.no License: GPLv3 Keywords: API SNL DSD Classifier: Development
+Status :: 5 - Production/Stable Classifier: Environment :: Console Classifier:
+Intended Audience :: Developers Classifier: Natural Language :: Norwegian
+Classifier: Natural Language :: Danish Classifier: License :: OSI Approved ::
+GNU General Public License v3 (GPLv3) Classifier: Operating System :: OS
+Independent Classifier: Programming Language :: Python Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3 :: Only Classifier: Topic ::
+Software Development :: Libraries :: Python Modules Requires-Python: >=3.6
+Description-Content-Type: text/markdown License-File: LICENSE
                                     [Logo]
- [Actions_Status] [Documentation_Status] [https://app.fossa.com/api/projects/
-git%2Bgithub.com%2FDiFronzo%2FSnlData.svg?type=small] [Coverage_Status] [Build
-                   Status] [License:_MIT] [Downloads] [PyPI]
-*** A lightweight Python library for Store Norske Leksikon and Lex.dk APIs ***
-## Installation pip install snldata ## Quick Start Raw JSON ```python import
+ [SnlData_version] [Actions_Status] [Documentation_Status] [Coverage_Status]
+              [Build_Status] [License:_GPLv3] [Downloads] [PyPI]
+*** A lightweight Python library for Store Norske Leksikon and Lex.dk/Den Store
+Danske APIs ***
+## Installation pip3 install snldata ## Quick Start Raw JSON ```python import
 snldata R = snldata.SnlSession() R.search(query="fortolket
 programmeringssprÃ¥k", best=True) #Pick the one with the best rank print
 (R.json) ``` Outputs: the JSON object ``` { "title": "fortolket
 programmeringssprÃ¥k", "url": "http://snl.no/
 fortolket_programmeringsspr%C3%A5k", "subject_url": "http://snl.no/.taxonomy/
 3689", "subject_title": "Programmering", "xhtml_body":
 "\u003cdiv\u003e\r\n\u003cp\u003eprogrammeringssprÃ¥k som ikke blir kompilert
@@ -31,65 +44,59 @@
 { "lastname": "", "firstname": "" }, "authors": [{ "full_name": "Henrik
 Dvergsdal" }], "images": [] } ``` ## Licenses for content from Store Norske
 Leksikon and Lex.dk | Licence | Description | Read more | --- | --- | --- | |
 `fri` | [Creative Commons](https://creativecommons.org/) **[CC-BY-SA-3.0]
 (https://creativecommons.org/licenses/by-sa/3.0/)** license. Everyone is
 allowed to **share, use, copy and adapt** the text as long as **the author and
 Store norske leksikon** continues to be credited and the article retains the
-same free license for further use. | [Meta](https://meta.snl.no/fri_gjenbruk) |
-`begrenset gjenbruk/begrÃ¦nset genbrug` | You **can't reuse, republish, or
-adapt** the article without first obtaining the author's permission.| [Meta]
-(https://meta.snl.no/begrenset_gjenbruk) ## Overview of sites/zones ### SNL |
-code | Website | Note | --- | --- | --- | | `snl` | https://snl.no/ | Default |
-`nbl` | https://nbl.snl.no/ | | `sml` | https://sml.snl.no/ | | `nkl` | https:/
-/nkl.snl.no/ | | `prototyping` | - | Unstable - for SNL ### LEX | code |
-Website | Note | --- | --- | --- | | `dsd` | https://denstoredanske.lex.dk/ | |
-`dlh` | https://dansklitteraturshistorie.lex.dk/ | | `dbl` | https://
-biografiskleksikon.lex.dk/ | | `gtl` | https://teaterleksikon.lex.dk/ | | `nm`
-| https://mytologi.lex.dk/ | | `do` | https://danmarksoldtid.lex.dk/ | | `sl` |
-https://symbolleksikon.lex.dk/ | | `dh` | https://danmarkshistorien.lex.dk/ | |
-`hob` | https://bornelitteratur.lex.dk/ | | `pd` | https://
-pattedyratlas.lex.dk/ | | `prototyping-lex` | - | Unstable - for LEX pages ##
-Query ### Easy Query - Main documentation: [API-dokumentasjon](https://
-meta.snl.no/API-dokumentasjon) ```python import snldata R = snldata.SnlSession
-() R.search(query="Ole Ivars", best=True) #Pick the one with the best rank
-print(R.url) ``` Outputs: `https://snl.no/Ole_Ivars` ```python import snldata R
-= snldata.SnlSession() R.search(query="Ole Ivars") #Pick the three best results
-for val in R.json: print(val["simple"] #Summery for each index ``` Outputs: ```
-0. Ole Ivars (rank 576.6): Ole Ivars er et norsk danseband fra Hamar. 1.
-Spellemannprisen (rank 25.9): Spellemannprisen er den norske platebransjens
-Ã¥rlige prisutdeling for Ã¥ stimulere og markere plateproduksjonen i Norge. 2.
-danseband (rank 25.1): Danseband, ensemble som spiller til dans, betegner i dag
-vanligvis en instrumentbesetning som i pop og rock (vokal, elektrisk gitar og
-bass, keyboards, trommer, eventuelt ogsÃ¥ saksofon eller andre blÃ¥sere).
+same free license for further use. | [SNL](https://meta.snl.no/fri_gjenbruk)
+[LEX](https://denstoredanske.lex.dk/.licenses/free) | `begrenset gjenbruk/
+begrÃ¦nset genbrug` | You **can't reuse, republish, or adapt** the article
+without first obtaining the author's permission.| [SNL](https://meta.snl.no/
+begrenset_gjenbruk) [LEX](https://denstoredanske.lex.dk/.licenses/restricted)
+## Overview of sites/zones ### SNL | code | Website | Note | --- | --- | --- |
+| `snl` | https://snl.no/ | Default | `nbl` | https://nbl.snl.no/ | | `sml` |
+https://sml.snl.no/ | | `nkl` | https://nkl.snl.no/ | | `prototyping` | - |
+Unstable - for SNL ### LEX | code | Website | Note | --- | --- | --- | | `dsd`
+| https://denstoredanske.lex.dk/ | | `dlh` | https://
+dansklitteraturshistorie.lex.dk/ | | `dbl` | https://biografiskleksikon.lex.dk/
+| | `gtl` | https://teaterleksikon.lex.dk/ | | `nm` | https://mytologi.lex.dk/
+| | `do` | https://danmarksoldtid.lex.dk/ | | `sl` | https://
+symbolleksikon.lex.dk/ | | `dh` | https://danmarkshistorien.lex.dk/ | | `hob` |
+https://bornelitteratur.lex.dk/ | | `pd` | https://pattedyratlas.lex.dk/ | |
+`nid` | https://naturenidanmark.lex.dk/ | | `trap` | https://trap.lex.dk/ | |
+`prototyping-lex` | - | Unstable - for LEX pages ## Query ### Easy Query - Main
+documentation (SNL): [API-dokumentasjon](https://meta.snl.no/API-dokumentasjon)
+```python import snldata R = snldata.SnlSession() R.search(query="Ole Ivars",
+best=True) #Pick the one with the best rank print(R.url) ``` Outputs: `https://
+snl.no/Ole_Ivars` ```python import snldata R = snldata.SnlSession() R.search
+(query="Ole Ivars") #Pick the three best results for val in R.json: print(val
+["simple"]) #Summery for each index ``` Outputs: ``` 0. Ole Ivars (rank 576.6):
+Ole Ivars er et norsk danseband fra Hamar. 1. Spellemannprisen (rank 25.9):
+Spellemannprisen er den norske platebransjens Ã¥rlige prisutdeling for Ã¥
+stimulere og markere plateproduksjonen i Norge. 2. danseband (rank 25.1):
+Danseband, ensemble som spiller til dans, betegner i dag vanligvis en
+instrumentbesetning som i pop og rock (vokal, elektrisk gitar og bass,
+keyboards, trommer, eventuelt ogsÃ¥ saksofon eller andre blÃ¥sere).
 ###Explaining of the values:
 ):  ``` Pick the article you want from the example above: ```python R._get(1)
 print(R.title) ``` Outputs: `Spellemannprisen` ```python import snldata R =
 snldata.SnlSession() R.search(zone='dsd', query="Python", best=True) #Pick the
 one with the best rank print(R.url) ``` Outputs: `https://
 denstoredanske.lex.dk/Python` ### Advance Query (best for prototyping api) -
-Main documentation: [API-dokumentasjon - prototyping](https://meta.snl.no/API-
-dokumentasjon_-_prototyping) ```python import snldata R = snldata.SnlSession()
-R.searchV2({"encyclopedia": "snl", "query": "dr. dre", "limit": 3, "offset": 0
-}, zone="prototyping", best=True) print(R.title) ``` Outputs: `Dr. Dre`
-```python import snldata R = snldata.SnlSession() R.searchV2({"encyclopedia":
-"snl", "query": "dr. dre", "limit": 3, "offset": 0 }, zone="prototyping") i = 0
-for val in R.json: print('{}. {}: {}'.format(i, val['headword'], val
-["query_quality_explain"])) i += 1 ``` Outputs: ``` 0. Dr. Dre: The search
-string is equal to the article's headword and there is no further clarification
-1. hiphop: Match on article text or part of title 2. Eminem: Match on article
-text or part of title ###Explaining of the values: (the prototyping api allows
-you to send a lot of parametres)
- ``` Pick the article you want from the example above: ```python R._get(1)
-print("Title: {}, Created: {}".format(R.title, R.created_at)) ``` Outputs:
-`Title: hiphop, Created: 2009-02-14T05:15:20.546+01:00` ### No result If the
-API returns no results, `.json` will be given a empty list. ```python import
-snldata R = snldata.SnlSession() R.search(zone='dsd', query="asdadasdasdad",
-best=True) #Pick the one with the best rank print(R.json) ``` Outputs: `[]` All
-of the examples uses text that is [CC-BY-SA-3.0](https://creativecommons.org/
-licenses/by-sa/3.0). By at least one of the following authors: Henrik
-Dvergsdal, Jon Vidar Bergan, and Audun Kjus Aahlin. Read more about the
-license: [fri gjenbruk](https://meta.snl.no/fri_gjenbruk). ## To-do - [ ] Fully
-support taxonomy - [X] When zero results, return somthing to tell the user
-there is no result. ## Reporting Issues If you have suggestions, bugs or other
-issues specific to this library, file them [here](https://github.com/DiFronzo/
-SnlData/issues). Or just send me a pull request.
+Main documentation (SNL): [API-dokumentasjon - prototyping](https://
+meta.snl.no/API-dokumentasjon_-_prototyping) **The prototyping API endpoint has
+been removed as of May 2023.** ### No result If the API returns no results,
+`.json` will be given a empty list. ```python import snldata R =
+snldata.SnlSession() R.search(zone='dsd', query="asdadasdasdad", best=True)
+#Pick the one with the best rank print(R.json) ``` Outputs: `{}` ```python
+import snldata R = snldata.SnlSession() R.search(zone='dsd',
+query="jdfhdskjfhsjkdfhksdfh") #Pick the three best results, but there are none
+R._get(0) print(R.json) ``` Outputs: `{}` All of the examples uses text that is
+[CC-BY-SA-3.0](https://creativecommons.org/licenses/by-sa/3.0). By at least one
+of the following authors: Henrik Dvergsdal, Jon Vidar Bergan, and Audun Kjus
+Aahlin. Read more about the license: [fri gjenbruk](https://meta.snl.no/
+fri_gjenbruk). ## To-do - [ ] Fully support taxonomy - [ ] Support for
+".recent-activities" to JSON. - [X] When zero results, return empty dict to
+tell the user there is no result. ## Reporting Issues If you have suggestions,
+bugs or other issues specific to this library, file them [here](https://
+github.com/DiFronzo/SnlData/issues). Or just send me a pull request.
```

### Comparing `SnlData-1.1.0/setup.py` & `SnlData-1.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 import setuptools
 import sys
 import os
 
-assert sys.version_info >= (3, 6, 0), "SnlData requires Python 3.6+"
+assert sys.version_info >= (3, 8, 0), "SnlData requires Python 3.8+"
 from pathlib import Path  # noqa E402
 
 CURRENT_DIR = Path(__file__).parent
 sys.path.insert(0, str(CURRENT_DIR))  # for setuptools.build_meta
 
 
 def get_long_description() -> str:
@@ -32,16 +32,16 @@
     opt_level = os.getenv("MYPYC_OPT_LEVEL", "3")
     ext_modules = mypycify(mypyc_targets, opt_level=opt_level)
 else:
     ext_modules = []
 
 setuptools.setup(
     name="SnlData",
-    version="1.1.0",
-    description="A lightweight Python library for Store Norske Leksikon and Lex.dk APIs.",
+    version="1.1.2",
+    description="A lightweight Python library for Store Norske Leksikon and Lex.dk/Den Store Danske APIs.",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     keywords="API SNL DSD",
     author="DiFronzo",
     author_email="root@vfiles.no",
     url="https://github.com/DiFronzo/SnlData",
     license="GPLv3",
@@ -59,14 +59,13 @@
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Natural Language :: Norwegian",
         "Natural Language :: Danish",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3 :: Only",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
 )
```

### Comparing `SnlData-1.1.0/snldata/client.py` & `SnlData-1.1.2/snldata/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 #!/usr/bin/env python3
 import requests
 import re
-from typing import Any, Dict
 
 name = "SnlData"
 api_version = 'v1'
 user_agent = "%s %s" % (name, api_version)
 
-script_version = '1.1.0'
+script_version = '1.1.2'
 
 
 class SnlSession:
     """
         Example usage:
 
             import snldata
@@ -22,39 +21,43 @@
     """
 
     PATHS = {
         'snl': 'https://snl.no/api/' + api_version + '/search',  # Store norske leksikon
         'nbl': 'https://nbl.snl.no/api/' + api_version + '/search',  # Norsk biografisk leksikon
         'sml': 'https://sml.snl.no/api/' + api_version + '/search',  # Store medisinske leksikon
         'nkl': 'https://nkl.snl.no/api/' + api_version + '/search',  # Norsk kunstnerleksikon
-        'prototyping': 'https://snl.no/.api/prototyping/search',  # UNSTABLE - SNL
+        # 'prototyping': 'https://snl.no/.api/prototyping/search',  # UNSTABLE SNL - Broken
         'dsd': 'https://denstoredanske.lex.dk/api/' + api_version + '/search',  # Den store danske
         'dlh': 'https://dansklitteraturshistorie.lex.dk/api/' + api_version + '/search',  # Dansk litteratur historie
         'dbl': 'https://biografiskleksikon.lex.dk/api/' + api_version + '/search',  # Dansk biografisk leksikon
         'gtl': 'https://teaterleksikon.lex.dk/api' + api_version + '/search',  # Gyldendals Teaterleksikon
         'nm': 'https://mytologi.lex.dk/api/' + api_version + '/search',  # Nordisk Mytologi
         'do': 'https://danmarksoldtid.lex.dk/api/' + api_version + '/search',  # Danmarks Oldtid
         'sl': 'https://symbolleksikon.lex.dk/api/' + api_version + '/search',  # Symbolleksikon
         'dh': 'https://danmarkshistorien.lex.dk/api/' + api_version + '/search',  # Danmarkshistorien
         'hob': 'https://bornelitteratur.lex.dk/api/' + api_version + '/search',  # Historien om børnelitteratur
         'pd': 'https://pattedyratlas.lex.dk/api/' + api_version + '/search',  # Dansk Pattedyratlas
-        'prototyping-lex': 'https://denstoredanske.lex.dk/.api/prototyping/search',  # UNSTABLE
+        'nid': 'https://naturenidanmark.lex.dk/api/' + api_version + '/search',  # Naturen i Danmark
+        'trap': 'https://trap.lex.dk/api/' + api_version + '/search',  # Trap Danmark
+        # 'prototyping-lex': 'https://denstoredanske.lex.dk/.api/prototyping/search',  # UNSTABLE - Broken
     }
 
     SHORT_TO_LONG = {
         'dsd': 'denstoredanske',
         'dlh': 'dansklitteraturshistorie',
         'dbl': 'biografiskleksikon',
         'gtl': 'teaterleksikon',
         'nm': 'mytologi',
         'do': 'danmarksoldtid',
         'sl': 'symbolleksikon',
         'dh': 'danmarkshistorien',
         'hob': 'bornelitteratur',
         'pd': 'pattedyratlas',
+        'nid': 'naturenidanmark',
+        'trap': 'trap'
     }
 
     QUERYQUAL = {
         0: "Match on article text or part of title",
         1: "The search string is equal to the headword, but the article \
 has a further clarification",
         2: "The search string is equal to the article's headword and there \
@@ -80,14 +83,15 @@
             It should generally be a good idea to keep sessions enabled
             for performance reasons.
         :param user_agent
             Tell Requests what program is used in the action
         """
         self.headers = {"User-Agent": user_agent}
         self.requests_timeout = requests_timeout
+        self.json = {}
 
         if isinstance(requests_session, requests.Session):
             self._S = requests_session
         else:
             if requests_session:  # Build a new session.
                 self._S = requests.Session()
             else:  # Use the Requests API module as a "session".
@@ -128,159 +132,164 @@
 
             if best:
                 self._get(0)
             else:
                 self.simple(zone)
         else:
             raise Exception(
-                "Something went wrong with the parametres!"
+                "Something went wrong with the parameters!"
             )
 
-    def searchV2(self, param: Dict[str, str], zone="snl", best=False) -> Any:
+    # Removed API
+    # def searchV2(self, param: Dict[str, str], zone="snl", best=False) -> Any:
+    #     """
+    #     Dict param: (with "prototyping")
+    #     @param encyclopedia: Begrens søket til angitt leksikon: snl, sml, nbl
+    #         eller nkl. Den samme filtreringen kan også oppnås ved gjøre søket i
+    #         et subdomene.
+    #     @type encyclopedia: str
+    #     @param query: Søketekst, f.eks. "Tog", "Edvard Munch"
+    #     @type query: str
+    #     @param limit: Maksimalt antall resultater. 1-100 er gyldige verdier,
+    #         standard er 10
+    #     @type limit: int
+    #     @param offset: Brukes for paginering av resultatene. Sett for eksempel
+    #         offset=100 for å vise søkeresultater utover de første 100.
+    #     @type offset: int
+    #     @param include_metadata: Metadata inkluderes i søkeresultatene hvis
+    #         dette parameteret settes til true
+    #     @type include_metadata: bool
+    #     @param article_type_id: Filtrer søket til å bare inkludere artikler
+    #         med angitt artikkeltype
+    #     @type article_type_id: int
+    #     @param author_id: Filtrer søket til å bare inkludere artikler av angitt
+    #          forfatter
+    #     @type author_id: int
+    #     @param author_name: Filtrer søket til å bare inkludere artikler av
+    #         forfattere med samsvarende navn
+    #     @type author_name: str
+    #     @param taxonomy_id: Filtrer søket til å bare inkludere artikler i
+    #         angitt taksonomi
+    #     @type taxonomy_id: int
+    #     @param taxonomy_title: Filtrer søket til å bare inkludere artikler i
+    #         taksonomier med samsvarende navn
+    #     @type taxonomy_title: str
+    #     @param tagsonomy_id: Filtrer søket til å bare inkludere artikler i
+    #         angitt tagsonomy
+    #     @type tagsonomy_id: int
+    #     @param tagsonomy_title: Filtrer søket til å bare inkludere artikler i
+    #         tagsonomyer med samsvarende navn
+    #     @type tagsonomy_title: str
+    #     @param char_count_min: Filtrer søket til å bare inkludere artikler med
+    #         angitt antall tegn i artikkelteksten, eller flere
+    #     @type char_count_min: int
+    #     @param char_count_max: Filtrer søket til å bare inkludere artikler med
+    #         angitt antall tegn i artikkelteksten, eller færre
+    #     @type char_count_max: int
+    #     @param media_count_min: Filtrer søket til å bare inkludere artikler med
+    #         angitt antall media-vedlegg, eller flere
+    #     @type media_count_min: int
+    #     @param media_count_max:Filtrer søket til å bare inkludere artikler med
+    #         angitt antall media-vedlegg, eller færre
+    #     @type media_count_max: int
+    #     @param version_count_min: Filtrer søket til å bare inkludere artikler
+    #         med angitt antall historiske versjoner, eller flere
+    #     @type version_count_min: int
+    #     @param version_count_max: Filtrer søket til å bare inkludere artikler
+    #         med angitt antall historiske versjoner, eller færre
+    #     @type version_count_max: int
+    #     @param license_id: Filtrer søket til å bare inkludere artikler med
+    #         angitt lisens-id (free eller restricted)
+    #     @type license_id: str
+    #     @param updated_at_or_after: Filtrer søket til å bare inkludere artikler
+    #         oppdatert på angitt tidspunkt, eller senere.
+    #         Tidspunktet angis i RFC3339-format.
+    #     @type updated_at_or_after: str (RFC3339 format)
+    #     @param updated_at_or_before: Filtrer søket til å bare inkludere
+    #         artikler oppdatert på angitt tidspunkt, eller tidligere.
+    #         Tidspunktet angis i RFC3339-format.
+    #     @type updated_at_or_before: str (RFC3339 format)
+    #     @param zone: Website used for the search
+    #     @type zone: str
+    #     @param best: To get the first and best (by query_match_quality)
+    #         result returned.
+    #     @type best: bool
+    #     :param param:
+    #     """
+    #     if (0 < param['limit'] < 101 and param['offset'] <
+    #             param['limit'] and param['query'] != "" and
+    #             zone in self.PATHS and param['encyclopedia'] in self.PATHS):
+
+    #         if param['encyclopedia'] in self.SHORT_TO_LONG: param['encyclopedia'] = self.SHORT_TO_LONG[
+    #             param['encyclopedia']]
+
+    #         self._get(param, zone)
+
+    #         if best:
+    #             self._get(0)
+    #         else:
+    #             self.simple(zone)
+    #     else:
+    #         raise Exception(
+    #             "Something went wrong with the parametres!"
+    #         )
+
+    def _store_value(self, R: requests.Response, zone: str):
         """
-        Dict param: (with "prototyping")
-        @param encyclopedia: Begrens søket til angitt leksikon: snl, sml, nbl
-            eller nkl. Den samme filtreringen kan også oppnås ved gjøre søket i
-            et subdomene.
-        @type encyclopedia: str
-        @param query: Søketekst, f.eks. "Tog", "Edvard Munch"
-        @type query: str
-        @param limit: Maksimalt antall resultater. 1-100 er gyldige verdier,
-            standard er 10
-        @type limit: int
-        @param offset: Brukes for paginering av resultatene. Sett for eksempel
-            offset=100 for å vise søkeresultater utover de første 100.
-        @type offset: int
-        @param include_metadata: Metadata inkluderes i søkeresultatene hvis
-            dette parameteret settes til true
-        @type include_metadata: bool
-        @param article_type_id: Filtrer søket til å bare inkludere artikler
-            med angitt artikkeltype
-        @type article_type_id: int
-        @param author_id: Filtrer søket til å bare inkludere artikler av angitt
-             forfatter
-        @type author_id: int
-        @param author_name: Filtrer søket til å bare inkludere artikler av
-            forfattere med samsvarende navn
-        @type author_name: str
-        @param taxonomy_id: Filtrer søket til å bare inkludere artikler i
-            angitt taksonomi
-        @type taxonomy_id: int
-        @param taxonomy_title: Filtrer søket til å bare inkludere artikler i
-            taksonomier med samsvarende navn
-        @type taxonomy_title: str
-        @param tagsonomy_id: Filtrer søket til å bare inkludere artikler i
-            angitt tagsonomy
-        @type tagsonomy_id: int
-        @param tagsonomy_title: Filtrer søket til å bare inkludere artikler i
-            tagsonomyer med samsvarende navn
-        @type tagsonomy_title: str
-        @param char_count_min: Filtrer søket til å bare inkludere artikler med
-            angitt antall tegn i artikkelteksten, eller flere
-        @type char_count_min: int
-        @param char_count_max: Filtrer søket til å bare inkludere artikler med
-            angitt antall tegn i artikkelteksten, eller færre
-        @type char_count_max: int
-        @param media_count_min: Filtrer søket til å bare inkludere artikler med
-            angitt antall media-vedlegg, eller flere
-        @type media_count_min: int
-        @param media_count_max:Filtrer søket til å bare inkludere artikler med
-            angitt antall media-vedlegg, eller færre
-        @type media_count_max: int
-        @param version_count_min: Filtrer søket til å bare inkludere artikler
-            med angitt antall historiske versjoner, eller flere
-        @type version_count_min: int
-        @param version_count_max: Filtrer søket til å bare inkludere artikler
-            med angitt antall historiske versjoner, eller færre
-        @type version_count_max: int
-        @param license_id: Filtrer søket til å bare inkludere artikler med
-            angitt lisens-id (free eller restricted)
-        @type license_id: str
-        @param updated_at_or_after: Filtrer søket til å bare inkludere artikler
-            oppdatert på angitt tidspunkt, eller senere.
-            Tidspunktet angis i RFC3339-format.
-        @type updated_at_or_after: str (RFC3339 format)
-        @param updated_at_or_before: Filtrer søket til å bare inkludere
-            artikler oppdatert på angitt tidspunkt, eller tidligere.
-            Tidspunktet angis i RFC3339-format.
-        @type updated_at_or_before: str (RFC3339 format)
+        Store API data
+        @param R: respone from API
+        @type R: requests.Response
         @param zone: Website used for the search
         @type zone: str
-        @param best: To get the first and best (by query_match_quality)
-            result returned.
-        @type best: bool
-        :param param:
         """
-        if (0 < param['limit'] < 101 and param['offset'] <
-                param['limit'] and param['query'] != "" and
-                zone in self.PATHS and param['encyclopedia'] in self.PATHS):
+        if R and R.status_code != 200:
+            raise Exception(
+                "GET was unsuccessfull ({}): {}".format(R.status_code, R.text)
+            )
 
-            if param['encyclopedia'] in self.SHORT_TO_LONG: param['encyclopedia'] = self.SHORT_TO_LONG[
-                param['encyclopedia']]
+        if hasattr(self, 'title'):
+            self.delete_var()
 
-            self._get(param, zone)
+        if R.json() != []:
+            self.json = R.json()
 
-            if best:
-                self._get(0)
-            else:
-                self.simple(zone)
-        else:
-            raise Exception(
-                "Something went wrong with the parametres!"
-            )
+        if not zone:
+            self.store_var()
 
     def _get(self, data, zone=""):
         """
         API GET
         @param data: parametres to be used or key in dict
         @type data: dict/int
         @param zone: Website used for the search
         @type zone: str
         """
         if isinstance(data, int) and isinstance(self.json, list):
-            try:
-                R = self._S.get(
-                    self.json[data]["article_url_json"], headers=self.headers)
-            except:
-                return 0  # zero results
+            R = self._S.get(
+                self.json[data]["article_url_json"], headers=self.headers)
+            self._store_value(R, zone)
         elif not isinstance(data, int):
             R = self._S.get(
                 self.PATHS[zone.lower()], params=data, headers=self.headers)
-        else:
-            raise NotImplementedError
-
-        if R.status_code != 200:
-            raise Exception(
-                "GET was unsuccessfull ({}): {}".format(R.status_code, R.text)
-            )
-
-        if hasattr(self, 'title'):
-            self.delete_var()
-
-        self.json = R.json()
-
-        if not zone:
-            self.store_var()
+            self._store_value(R, zone)
 
     def simple(self, zone=""):
         """
         Adds a entry to JSON file
         @param zone: Website used for the search (different for "prototyping")
         @type zone: str
         """
         i = 0
         for result in self.json:
             if zone == 'prototyping':
                 self.json[i].update(
-                    {'query_quality_explain':
-                         self.QUERYQUAL[result['query_match_quality']]})
+                    {'query_quality_explain': self.QUERYQUAL[result['query_match_quality']]})
             else:
                 sentence = re.search(
-                    r'^(.*?(?<!\b\w)[.?!])\s+[A-Z0-9]',
-                    result["first_two_sentences"], flags=0)
+                    r'^(.*?(?<!\b\w)[.?!])\s+[A-Z0-9]', result["first_two_sentences"], flags=0)
                 if isinstance(sentence, type(None)):
                     # Regex did not work
                     self.json[i].update(
                         {'simple': '{}. {} (rank {}): {}'.format(
                             i, result["headword"], round(result["rank"], 1),
                             result["first_two_sentences"])})
                 else:
```

