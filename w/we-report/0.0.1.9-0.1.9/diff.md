# Comparing `tmp/we_report-0.0.1.9-py3-none-any.whl.zip` & `tmp/we_report-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 8753 bytes, number of entries: 12
+Zip file size: 8746 bytes, number of entries: 12
 -rw-rw-rw-  2.0 fat      126 b- defN 23-Apr-20 09:46 we_report/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-21 07:41 we_report/data_type/__init__.py
 -rw-rw-rw-  2.0 fat     7440 b- defN 23-Mar-21 07:41 we_report/data_type/report_data.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-21 07:41 we_report/interface/__init__.py
 -rw-rw-rw-  2.0 fat     7307 b- defN 23-Mar-21 07:41 we_report/interface/excel_reporter.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-21 07:41 we_report/utils/__init__.py
 -rw-rw-rw-  2.0 fat      599 b- defN 23-Mar-21 07:41 we_report/utils/utils.py
--rw-rw-rw-  2.0 fat     1092 b- defN 23-Apr-20 09:47 we_report-0.0.1.9.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      778 b- defN 23-Apr-20 09:47 we_report-0.0.1.9.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-20 09:47 we_report-0.0.1.9.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 23-Apr-20 09:47 we_report-0.0.1.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      998 b- defN 23-Apr-20 09:47 we_report-0.0.1.9.dist-info/RECORD
-12 files, 18442 bytes uncompressed, 7051 bytes compressed:  61.8%
+-rw-rw-rw-  2.0 fat     1092 b- defN 23-May-09 09:30 we_report-0.1.9.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      828 b- defN 23-May-09 09:30 we_report-0.1.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-09 09:30 we_report-0.1.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 23-May-09 09:30 we_report-0.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      988 b- defN 23-May-09 09:30 we_report-0.1.9.dist-info/RECORD
+12 files, 18482 bytes uncompressed, 7064 bytes compressed:  61.8%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: we_report/utils/__init__.py
 Comment: 
 
 Filename: we_report/utils/utils.py
 Comment: 
 
-Filename: we_report-0.0.1.9.dist-info/LICENSE
+Filename: we_report-0.1.9.dist-info/LICENSE
 Comment: 
 
-Filename: we_report-0.0.1.9.dist-info/METADATA
+Filename: we_report-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: we_report-0.0.1.9.dist-info/WHEEL
+Filename: we_report-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: we_report-0.0.1.9.dist-info/top_level.txt
+Filename: we_report-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: we_report-0.0.1.9.dist-info/RECORD
+Filename: we_report-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `we_report-0.0.1.9.dist-info/LICENSE` & `we_report-0.1.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `we_report-0.0.1.9.dist-info/METADATA` & `we_report-0.1.9.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: we-report
-Version: 0.0.1.9
+Version: 0.1.9
 Summary: Wealth Engine ReportData Generator
 Home-page: http://192.168.1.7:10600/xiazeyu/we_report.git
 Author: Xia Zeyu
 Author-email: xiazeyu@wealthengine.cn
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -13,14 +13,16 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy (>=1.15)
 Requires-Dist: pandas (>=1.0.3)
 Requires-Dist: arrow (>=0.17.0)
 Requires-Dist: sqlalchemy (>=1.3.18)
 Requires-Dist: scikit-learn
+Requires-Dist: matplotlib
+Requires-Dist: xlsxwriter
 Requires-Dist: scipy
 Requires-Dist: statsmodels
 Requires-Dist: six
 
 # we_report
 
 如何通过python操纵接口，实现自动化的图文混排报告的生成。
```

## Comparing `we_report-0.0.1.9.dist-info/RECORD` & `we_report-0.1.9.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 we_report/__init__.py,sha256=9Q4Vsx44YmjZ5Ji1Wg4pmSqamVPHJTHDezLAHA37UG0,126
 we_report/data_type/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 we_report/data_type/report_data.py,sha256=nlnm3crZHLnx7_lr7lg9fKAQG0d8AS9H_Us1h3VCr0I,7440
 we_report/interface/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 we_report/interface/excel_reporter.py,sha256=nNPPDk8i3N3KVNPBpg6m_z-0nHImcPoqFhjICY8ZmPY,7307
 we_report/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 we_report/utils/utils.py,sha256=GkAJGbefPwIFypoKqMrhKiCnVNWBwRv47RtdPR0G5t0,599
-we_report-0.0.1.9.dist-info/LICENSE,sha256=unAISPdUaH8a0Vw-QIivpvGNO-x3h_irtPw7yj07b6c,1092
-we_report-0.0.1.9.dist-info/METADATA,sha256=N9J2bIIGxHAoO7q11ZDLqU4L_FT2AuiSTMuNgvhd-4g,778
-we_report-0.0.1.9.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-we_report-0.0.1.9.dist-info/top_level.txt,sha256=RZuqUTMBxg7Dc7a_DYNhzf_w_Isj1Id9mZTsDv1BzXw,10
-we_report-0.0.1.9.dist-info/RECORD,,
+we_report-0.1.9.dist-info/LICENSE,sha256=unAISPdUaH8a0Vw-QIivpvGNO-x3h_irtPw7yj07b6c,1092
+we_report-0.1.9.dist-info/METADATA,sha256=Ho2nprpWrQeWxeKOifLqhYM-CHfk05Vo02dKIB-ixiA,828
+we_report-0.1.9.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+we_report-0.1.9.dist-info/top_level.txt,sha256=RZuqUTMBxg7Dc7a_DYNhzf_w_Isj1Id9mZTsDv1BzXw,10
+we_report-0.1.9.dist-info/RECORD,,
```

