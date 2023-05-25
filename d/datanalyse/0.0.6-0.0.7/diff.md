# Comparing `tmp/datanalyse-0.0.6.tar.gz` & `tmp/datanalyse-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datanalyse-0.0.6.tar", last modified: Thu May 25 19:04:07 2023, max compression
+gzip compressed data, was "datanalyse-0.0.7.tar", last modified: Thu May 25 20:21:18 2023, max compression
```

## Comparing `datanalyse-0.0.6.tar` & `datanalyse-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1078 2023-05-08 10:35:18.120135 datanalyse-0.0.6/LICENSE
--rw-r--r--   0        0        0      459 2023-05-08 11:21:31.284922 datanalyse-0.0.6/README.md
--rw-r--r--   0        0        0      687 2023-05-25 19:04:07.831587 datanalyse-0.0.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-08 13:28:09.975326 datanalyse-0.0.6/src/datanalyse/__init__.py
--rw-r--r--   0        0        0        0 2023-05-05 21:03:10.188371 datanalyse-0.0.6/src/datanalyse/dataelement/__init__.py
--rw-r--r--   0        0        0     8844 2023-05-10 07:45:44.270328 datanalyse-0.0.6/src/datanalyse/dataelement/dataelement.py
--rw-r--r--   0        0        0     3492 2023-05-08 20:06:25.263720 datanalyse-0.0.6/src/datanalyse/dataelement/dfmanipulation.py
--rw-r--r--   0        0        0    32204 2023-05-10 12:53:17.678047 datanalyse-0.0.6/src/datanalyse/dataelement/formate.py
--rw-r--r--   0        0        0      362 2023-05-08 20:06:25.269023 datanalyse-0.0.6/src/datanalyse/dataelement/stoffwerte.py
--rw-r--r--   0        0        0        0 2022-11-21 14:15:44.602999 datanalyse-0.0.6/src/datanalyse/diagramme/__init__.py
--rw-r--r--   0        0        0     4753 2023-05-10 07:45:44.282229 datanalyse-0.0.6/src/datanalyse/diagramme/balken.py
--rw-r--r--   0        0        0     2863 2023-05-08 20:06:25.272554 datanalyse-0.0.6/src/datanalyse/diagramme/diagramm.py
--rw-r--r--   0        0        0     4224 2023-05-08 20:06:25.274579 datanalyse-0.0.6/src/datanalyse/diagramme/globalbewertung.py
--rw-r--r--   0        0        0     1102 2023-05-08 20:06:25.278540 datanalyse-0.0.6/src/datanalyse/diagramme/matplotlib_parameter.py
--rw-r--r--   0        0        0     3115 2023-05-10 07:45:44.288184 datanalyse-0.0.6/src/datanalyse/diagramme/zeitreihe.py
--rw-r--r--   0        0        0      703 2023-05-08 10:35:18.138208 datanalyse-0.0.6/src/datanalyse/pfade.py
--rw-r--r--   0        0        0   149819 2023-05-10 07:45:44.296614 datanalyse-0.0.6/tests/Ahlborn.xlsx
--rw-r--r--   0        0        0      331 2023-05-10 12:30:07.304385 datanalyse-0.0.6/tests/test_dataelement.py
--rw-r--r--   0        0        0     1042 1970-01-01 00:00:00.000000 datanalyse-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-05-06 19:06:32.333418 datanalyse-0.0.7/LICENSE
+-rw-r--r--   0        0        0      459 2023-05-06 20:17:48.271205 datanalyse-0.0.7/README.md
+-rw-r--r--   0        0        0      687 2023-05-25 20:21:18.495375 datanalyse-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-08 18:40:19.058776 datanalyse-0.0.7/src/datanalyse/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-06 12:49:40.254042 datanalyse-0.0.7/src/datanalyse/dataelement/__init__.py
+-rw-r--r--   0        0        0     8844 2023-05-09 19:26:05.392037 datanalyse-0.0.7/src/datanalyse/dataelement/dataelement.py
+-rw-r--r--   0        0        0     3492 2023-05-08 19:59:39.673710 datanalyse-0.0.7/src/datanalyse/dataelement/dfmanipulation.py
+-rw-r--r--   0        0        0    32002 2023-05-25 20:18:54.971395 datanalyse-0.0.7/src/datanalyse/dataelement/formate.py
+-rw-r--r--   0        0        0      362 2023-05-08 19:59:45.459719 datanalyse-0.0.7/src/datanalyse/dataelement/stoffwerte.py
+-rw-r--r--   0        0        0        0 2023-05-08 18:40:19.069280 datanalyse-0.0.7/src/datanalyse/diagramme/__init__.py
+-rw-r--r--   0        0        0     4753 2023-05-08 20:30:15.275768 datanalyse-0.0.7/src/datanalyse/diagramme/balken.py
+-rw-r--r--   0        0        0     2863 2023-05-08 19:59:19.452792 datanalyse-0.0.7/src/datanalyse/diagramme/diagramm.py
+-rw-r--r--   0        0        0     4224 2023-05-08 19:59:23.694912 datanalyse-0.0.7/src/datanalyse/diagramme/globalbewertung.py
+-rw-r--r--   0        0        0     1102 2023-05-08 19:59:25.417764 datanalyse-0.0.7/src/datanalyse/diagramme/matplotlib_parameter.py
+-rw-r--r--   0        0        0     3115 2023-05-08 20:30:59.493810 datanalyse-0.0.7/src/datanalyse/diagramme/zeitreihe.py
+-rw-r--r--   0        0        0      703 2023-04-28 12:58:07.459695 datanalyse-0.0.7/src/datanalyse/pfade.py
+-rw-r--r--   0        0        0   149819 2023-05-09 12:45:52.677187 datanalyse-0.0.7/tests/Ahlborn.xlsx
+-rw-r--r--   0        0        0      382 2023-05-25 20:20:01.734815 datanalyse-0.0.7/tests/test_dataelement.py
+-rw-r--r--   0        0        0     1042 1970-01-01 00:00:00.000000 datanalyse-0.0.7/PKG-INFO
```

### Comparing `datanalyse-0.0.6/LICENSE` & `datanalyse-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `datanalyse-0.0.6/pyproject.toml` & `datanalyse-0.0.7/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "datanalyse"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
     { name = "Maximilian Beyer", email = "maximilian.beyer@tu-dresden.de" },
 ]
 description = "A data analysis package."
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `datanalyse-0.0.6/src/datanalyse/dataelement/dataelement.py` & `datanalyse-0.0.7/src/datanalyse/dataelement/dataelement.py`

 * *Files identical despite different names*

### Comparing `datanalyse-0.0.6/src/datanalyse/dataelement/dfmanipulation.py` & `datanalyse-0.0.7/src/datanalyse/dataelement/dfmanipulation.py`

 * *Files identical despite different names*

### Comparing `datanalyse-0.0.6/src/datanalyse/dataelement/formate.py` & `datanalyse-0.0.7/src/datanalyse/dataelement/formate.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,20 +24,18 @@
     :param resample_zeitschritt: Resampling aller Daten dient der Umrechnung auf eine gemeinsame Zeitschrittweite, es werden alle zur Zeitschrittweite gehörenden Werte gemittelt
     :param nur_ergebniszeile:
     :return: formatiertes Dataelement
     """
     df = pd.read_excel(
         dataelement.pfad,
         sheet_name=0,
-        # parse_dates=[["Datum", "Zeit"]],  # Kombination von Datum und Zeit nicht mehr möglich, da kein dayfirst
+        parse_dates=[["Datum", "Zeit"]],
+        date_format=None,
     )
 
-    # Kombination von Datum und Zeit zu Zeitstempel
-    df["Datum_Zeit"] = pd.to_datetime(str(df["Datum"]) + " " + str(df["Zeit"]), dayfirst=True)
-    
     # Zeitstempel wird als Index gesetzt
     df.set_index("Datum_Zeit", inplace=True)
 
     # drop alle Spalten, bei denen absolut nichts drin steht (beugt Fehlern vor, tritt vor allem bei Sollwerten auf)
     if dropna_spalten:
         df.dropna(how="all", axis=1, inplace=True)
```

### Comparing `datanalyse-0.0.6/src/datanalyse/diagramme/balken.py` & `datanalyse-0.0.7/src/datanalyse/diagramme/balken.py`

 * *Files identical despite different names*

### Comparing `datanalyse-0.0.6/src/datanalyse/diagramme/diagramm.py` & `datanalyse-0.0.7/src/datanalyse/diagramme/diagramm.py`

 * *Files identical despite different names*

### Comparing `datanalyse-0.0.6/src/datanalyse/diagramme/globalbewertung.py` & `datanalyse-0.0.7/src/datanalyse/diagramme/globalbewertung.py`

 * *Files identical despite different names*

### Comparing `datanalyse-0.0.6/src/datanalyse/diagramme/matplotlib_parameter.py` & `datanalyse-0.0.7/src/datanalyse/diagramme/matplotlib_parameter.py`

 * *Files identical despite different names*

### Comparing `datanalyse-0.0.6/src/datanalyse/diagramme/zeitreihe.py` & `datanalyse-0.0.7/src/datanalyse/diagramme/zeitreihe.py`

 * *Files identical despite different names*

### Comparing `datanalyse-0.0.6/src/datanalyse/pfade.py` & `datanalyse-0.0.7/src/datanalyse/pfade.py`

 * *Files identical despite different names*

### Comparing `datanalyse-0.0.6/tests/Ahlborn.xlsx` & `datanalyse-0.0.7/tests/Ahlborn.xlsx`

 * *Files identical despite different names*

### Comparing `datanalyse-0.0.6/PKG-INFO` & `datanalyse-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datanalyse
-Version: 0.0.6
+Version: 0.0.7
 Summary: A data analysis package.
 Author-Email: Maximilian Beyer <maximilian.beyer@tu-dresden.de>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Project-URL: Homepage, https://github.com/MakusuB/datanalyse
 Project-URL: Bug tracker, https://github.com/MakusuB/datanalyse/issues
```

