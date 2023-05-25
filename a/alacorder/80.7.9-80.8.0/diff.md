# Comparing `tmp/alacorder-80.7.9.tar.gz` & `tmp/alacorder-80.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.7.9.tar", max compression
+gzip compressed data, was "alacorder-80.8.0.tar", max compression
```

## Comparing `alacorder-80.7.9.tar` & `alacorder-80.8.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.7.9/LICENSE
--rw-r--r--   0        0        0     6518 2023-05-23 14:35:47.192010 alacorder-80.7.9/README.md
--rw-r--r--   0        0        0      746 2023-05-23 18:00:38.428059 alacorder-80.7.9/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-05-23 18:06:40.624148 alacorder-80.7.9/src/alacorder/.DS_Store
--rw-r--r--   0        0        0   234455 2023-05-18 23:58:39.588863 alacorder-80.7.9/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py
--rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.7.9/src/alacorder/__init__.py
--rw-r--r--   0        0        0   241502 2023-05-23 18:06:27.826136 alacorder-80.7.9/src/alacorder/__main__.py
--rw-r--r--   0        0        0   241502 2023-05-23 18:06:30.449556 alacorder-80.7.9/src/alacorder/alac.py
--rw-r--r--   0        0        0     7489 1970-01-01 00:00:00.000000 alacorder-80.7.9/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.8.0/LICENSE
+-rw-r--r--   0        0        0     6518 2023-05-23 14:35:47.192010 alacorder-80.8.0/README.md
+-rw-r--r--   0        0        0      746 2023-05-25 18:10:16.703624 alacorder-80.8.0/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-05-23 18:11:50.134411 alacorder-80.8.0/src/alacorder/.DS_Store
+-rw-r--r--   0        0        0   234455 2023-05-18 23:58:39.588863 alacorder-80.8.0/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py
+-rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.8.0/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   255361 2023-05-25 18:09:25.182499 alacorder-80.8.0/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   255361 2023-05-25 18:08:54.049754 alacorder-80.8.0/src/alacorder/alac.py
+-rw-r--r--   0        0        0     7489 1970-01-01 00:00:00.000000 alacorder-80.8.0/PKG-INFO
```

### Comparing `alacorder-80.7.9/LICENSE` & `alacorder-80.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-80.7.9/README.md` & `alacorder-80.8.0/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-80.7.9/pyproject.toml` & `alacorder-80.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "80.7.9"
+version = "80.8.0"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-80.7.9/src/alacorder/.DS_Store` & `alacorder-80.8.0/src/alacorder/.DS_Store`

 * *Files identical despite different names*

### Comparing `alacorder-80.7.9/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py` & `alacorder-80.8.0/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py`

 * *Files identical despite different names*

### Comparing `alacorder-80.7.9/src/alacorder/__main__.py` & `alacorder-80.8.0/src/alacorder/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Optional dependencies:
     pyarrow required to export summary to .xls, .xlsx,
     Google Chrome required to fetch cases from Alacourt and crawl ADOC
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.7.9"
+version = "80.8.0"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -3272,14 +3272,209 @@
         return query
     else:
         print(
             "Try again with at least one valid column header: [NAME, PARTY_TYPE, SSN, DOB, COUNTY, DIVISION, CASE_YEAR, NO_RECORDS, FILED_BEFORE, FILED_AFTER, RETRIEVED, CASES_FOUND, QUERY_COMPLETE]"
         )
         return None
 
+
+def make_fetch_queue_from_crawl(df):
+    if isinstance(df, str):
+        df = read(df)
+    df = df.select(
+        [
+            pl.col("AIS"),
+            pl.col("Name").str.extract(r', ([A-Z]+)').alias("FirstName"),
+            pl.col("Name").str.extract(r'^([A-Z]+)').alias("LastName"),
+        ]
+    )
+    return df
+
+def adoc_fetch(df=None, path=None, cf=None):
+    if cf:
+        df = read(cf['INPUTS'])
+        path = cf['OUTPUT_PATH']
+    if df:
+        if isinstance(df, str):
+            dfpath = df
+            df = read(df)
+        else:
+            dfpath = None
+    if 'Retrieved' not in df.columns:
+        df = df.select("AIS", "FirstName", "LastName")
+        df = df.with_columns(pl.lit("").alias("Retrieved"))
+    df = df.with_columns(pl.col("AIS").cast(pl.Utf8, strict=False))
+    out = pl.DataFrame()
+    driver = webdriver.Chrome()
+    for i, r in enumerate(tqdm(df.rows(named=True))):
+        if r['Retrieved'] != '' and r['Retrieved'] != None:
+            continue
+        try:
+            out = pl.concat([out, read_top_result(driver, r['AIS'], r['FirstName'], r['LastName'])])
+        except:
+            pass
+        df[i, 'Retrieved'] = datetime.now().strftime("%d-%m-%Y %H:%M:%S")
+        if dfpath and df.shape[0] > 10 and i % 10 == 0:
+            write(df, sheet_names=["adoc_progress"], path=dfpath)
+        if df.shape[0] > 10 and i % 10 == 0 and path:
+            write(out, sheet_names=["adoc"], path=path)
+    if path:
+        write(out, sheet_names=["adoc"], path=path)
+    if dfpath:
+        write(df, sheet_names=["adoc_progress"], path=dfpath)
+    return out, df
+
+def read_top_result(driver, ais, first, last):
+    driver.get("http://www.doc.state.al.us/inmatesearch")
+    ais_box = driver.find_element(by=By.NAME, value="ctl00$MainContent$txtAIS")
+    first_name_box = driver.find_element(by=By.NAME, value="ctl00$MainContent$txtFName")
+    last_name_box = driver.find_element(by=By.NAME, value="ctl00$MainContent$txtLName")
+    send_button = driver.find_element(by=By.NAME, value="ctl00$MainContent$btnSearch")
+    ais_box.send_keys(ais)
+    first_name_box.send_keys(first)
+    last_name_box.send_keys(last)
+    send_button.click()
+    urls = driver.find_elements(by=By.TAG_NAME, value="a")
+    results = []
+    for x in urls:
+        try:
+            if 'InmateResults' in x.get_attribute("ID"):
+                results += [x]
+        except:
+            pass
+    try:
+        results[0].click()
+        return read_adoc_page(driver)
+    except:
+        return pl.DataFrame()
+
+
+def filter_missing_cases(adoc_df, cases_df):
+    if isinstance(adoc_df, str):
+        adoc_df = read(adoc_df)
+    if isinstance(cases_df, str):
+        cases_df = read(cases_df)
+    if 'AllPagesText' in cases_df.columns:
+        cases_df = set(cases_df, table="cases", now=True)
+    cases_df = cases_df.with_columns(
+        pl.col("CaseNumber").str.extract(r'(\w\w-\d\d\d\d-\d\d\d\d\d\d)').alias("CaseNoFragment")
+    )
+    clist = cases_df.select("CaseNoFragment").to_series().to_list()
+    cmap = pl.DataFrame(
+        {
+            'Selection': ['94 - ARDMORE', '93 - ATHENS', '04 - AUTAUGA', '05 - BALDWIN', '06 - BARBOUR - CLAYTON', '69 - BARBOUR - EUFAULA', '89 - BERRY', '07 - BIBB', '08 - BLOUNT', '87 - BRUNDIDGE MUNICIPAL COURT', '09 - BULLOCK', '10 - BUTLER', '11 - CALHOUN', '12 - CHAMBERS', '13 - CHEROKEE', '90 - CHEROKEE', '14 - CHILTON', '15 - CHOCTAW', '16 - CLARKE', '17 - CLAY', '18 - CLEBURNE', '19 - COFFEE - ELBA', '71 - COFFEE - ENTERPRISE', '20 - COLBERT', '21 - CONECUH', '22 - COOSA', '23 - COVINGTON', '24 - CRENSHAW', '25 - CULLMAN', '26 - DALE', '27 - DALLAS', '28 - DeKALB', '29 - ELMORE', '30 - ESCAMBIA', '31 - ETOWAH', '32 - FAYETTE', '33 - FRANKLIN', '34 - GENEVA', '35 - GREENE', '36 - HALE', '37 - HENRY', '38 - HOUSTON', '39 - JACKSON', '68 - JEFFERSON - BESSEMER', '01 - JEFFERSON - BIRMINGHAM', '40 - LAMAR', '41 - LAUDERDALE', '42 - LAWRENCE', '43 - LEE', '44 - LIMESTONE', '82 - LIVINGSTON', '45 - LOWNDES', '46 - MACON', '47 - MADISON', '48 - MARENGO', '49 - MARION', '50 - MARSHALL', '92 - MILLBROOK', '02 - MOBILE', '51 - MONROE', '03 - MONTGOMERY', '52 - MORGAN', '53 - PERRY', '80 - PHENIX CITY', '54 - PICKENS', '55 - PIKE', '88 - PRATTVILLE', '56 - RANDOLPH', '57 - RUSSELL', '58 - SHELBY', '59 - ST. CLAIR - ASHVILLE', '75 - ST. CLAIR - PELL CITY', '81 - SUMITON MUNICIPAL COURT', '60 - SUMTER', '74 - TALLADEGA - SYLACAUGA', '61 - TALLADEGA - TALLADEGA', '70 - TALLAPOOSA - ALEX CITY', '62 - TALLAPOOSA - DADEVILLE', '63 - TUSCALOOSA', '64 - WALKER', '65 - WASHINGTON', '95 - WETUMPKA MUNICIPAL COURT', '66 - WILCOX', '67 - WINSTON'],
+            'CountyNumber': ['94', '93', '04', '05', '06', '69', '89', '07', '08', '87', '09', '10', '11', '12', '13', '90', '14', '15', '16', '17', '18', '19', '71', '20', '21', '22', '23', '24', '25', '26', '27', '28', '29', '30', '31', '32', '33', '34', '35', '36', '37', '38', '39', '68', '01', '40', '41', '42', '43', '44', '82', '45', '46', '47', '48', '49', '50', '92', '02', '51', '03', '52', '53', '80', '54', '55', '88', '56', '57', '58', '59', '75', '81', '60', '74', '61', '70', '62', '63', '64', '65', '95', '66', '67'],
+            'County': ['ARDMORE', 'ATHENS', 'AUTAUGA', 'BALDWIN', 'BARBOUR - CLAYTON', 'BARBOUR - EUFAULA', 'BERRY', 'BIBB', 'BLOUNT', 'BRUNDIDGE MUNICIPAL COURT', 'BULLOCK', 'BUTLER', 'CALHOUN', 'CHAMBERS', 'CHEROKEE', 'CHEROKEE', 'CHILTON', 'CHOCTAW', 'CLARKE', 'CLAY', 'CLEBURNE', 'COFFEE - ELBA', 'COFFEE - ENTERPRISE', 'COLBERT', 'CONECUH', 'COOSA', 'COVINGTON', 'CRENSHAW', 'CULLMAN', 'DALE', 'DALLAS', 'DeKALB', 'ELMORE', 'ESCAMBIA', 'ETOWAH', 'FAYETTE', 'FRANKLIN', 'GENEVA', 'GREENE', 'HALE', 'HENRY', 'HOUSTON', 'JACKSON', 'JEFFERSON - BESSEMER', 'JEFFERSON - BIRMINGHAM', 'LAMAR', 'LAUDERDALE', 'LAWRENCE', 'LEE', 'LIMESTONE', 'LIVINGSTON', 'LOWNDES', 'MACON', 'MADISON', 'MARENGO', 'MARION', 'MARSHALL', 'MILLBROOK', 'MOBILE', 'MONROE', 'MONTGOMERY', 'MORGAN', 'PERRY', 'PHENIX CITY', 'PICKENS', 'PIKE', 'PRATTVILLE', 'RANDOLPH', 'RUSSELL', 'SHELBY', 'ST. CLAIR - ASHVILLE', 'ST. CLAIR - PELL CITY', 'SUMITON MUNICIPAL COURT', 'SUMTER', 'TALLADEGA - SYLACAUGA', 'TALLADEGA - TALLADEGA', 'TALLAPOOSA - ALEX CITY', 'TALLAPOOSA - DADEVILLE', 'TUSCALOOSA', 'WALKER', 'WASHINGTON', 'WETUMPKA MUNICIPAL COURT', 'WILCOX', 'WINSTON'] 
+        }
+    )
+    adoc_df = adoc_df.join(cmap, on="County", how="left")
+    adoc_df = adoc_df.with_columns(
+        pl.concat_str(
+            [
+                pl.col("CountyNumber"),
+                pl.lit("-"),
+                pl.col("CaseNo").str.extract(r"(\w\w)"),
+                pl.lit("-"),
+                pl.col("CaseNo").str.extract(r'(\d\d\d\d)\-'),
+                pl.lit("-"),
+                pl.col("CaseNo").str.extract(r'\-(\d\d\d\d\d\d)'),
+            ]
+        ).alias("CaseNoFragment")
+    )
+    out = adoc_df.filter(pl.col("CaseNoFragment").is_in(clist).is_not())
+    out = out.filter(pl.col("CaseNoFragment").is_null().is_not())
+    return out
+
+def read_adoc_page(driver):
+    rl = driver.find_elements(by=By.TAG_NAME, value="tr")
+    alltxt = []
+    for r in rl:
+        alltxt += [r.text]
+    name = driver.find_element(by=By.ID, value="MainContent_DetailsView2_Label1").text
+    allt = pl.DataFrame({'Tables': "\n".join(alltxt)})
+    allt = allt.with_columns(pl.col("Tables").str.split("SUF"))
+    allt = allt.explode("Tables")
+    allt = allt.with_columns(pl.col("Tables").str.split("Sentences"))
+    allt = allt.explode("Tables")
+    details = allt.filter(pl.col("Tables").str.contains("Date Total Term"))
+    sentences = allt.filter(pl.col("Tables").str.contains("Sentenced"))
+    inmate = allt.filter(pl.col("Tables").str.contains("Eye Color"))
+    sentences = sentences.with_row_count()
+    details = details.with_row_count()
+    inmate = inmate.select(
+        [
+            pl.lit(name).alias("Name"),
+            pl.col("Tables").str.extract(r'AIS:\s+(\d{8})').alias("AIS"),
+            pl.col("Tables").str.extract(r'Institution: ([A-Z\s]+)').alias("Institution"
+             ),
+            pl.col("Tables").str.extract(r'Race: ([A-Z])').alias("Race"),
+            pl.col("Tables").str.extract(r'Sex: ([A-Z])').alias("Sex"),
+            pl.col("Tables").str.extract(r'Hair Color: ([A-Z]+)').alias("HairColor"),
+            pl.col("Tables").str.extract(r'Eye Color: ([A-Z]+)').alias("EyeColor"),
+            pl.col("Tables").str.extract(r'Height: (.+)').alias("Height"),
+            pl.col("Tables").str.extract(r'Weight: (\d+)').alias("Weight"),
+            pl.col("Tables").str.extract(r'Birth Year: (\d\d\d\d)').alias("BirthYear"),
+            pl.col("Tables").str.extract(r'Custody (.+)').alias("Custody")
+        ]
+    )
+    sentences = sentences.with_columns(pl.col("Tables").str.split('\n'))
+    sentences = sentences.explode("Tables")
+    sentences = sentences.filter(pl.col("Tables").str.contains("[A-Z]"))
+    sentences = sentences.filter(pl.col("Tables").str.contains("Sentenced").is_not())
+    sentences = sentences.unique()
+    sentences = sentences.select(
+        [
+            pl.col("row_nr"),
+            pl.col("Tables").str.extract(r'([^\s]+)').alias("CaseNo"),
+            pl.col("Tables").str.extract(r'(\d\d?/\d\d?/\d\d\d\d)').str.to_date('%m/%d/%Y', strict=False).alias("Sentenced"),
+            pl.col("Tables").str.extract(r'\d\d?/\d\d?/\d\d\d\d (.+?) \d+Y \d+M \d+D').alias("Offense"),
+            pl.col("Tables").str.extract(r'\d\d?/\d\d?/\d\d\d\d .+? (\d+Y \d+M \d+D)').alias("Term"),
+            pl.col("Tables").str.extract(r'\d\d?/\d\d?/\d\d\d\d .+? \d+Y \d+M \d+D (\d+)').cast(pl.Int64, strict=False).alias("SentenceJailCredit"),
+            pl.col("Tables").str.extract(r'\d\d?/\d\d?/\d\d\d\d .+? \d+Y \d+M \d+D \d+ \d* ?(C?o?n?c?u?r?r?e?n?t?)').alias("Type"),
+            pl.col("Tables").str.extract(r'\d\d?/\d\d?/\d\d\d\d .+? \d+Y \d+M \d+D \d+ \d* ?C?o?n?c?u?r?r?e?n?t? ?([A-Z]+)').alias("County")
+        ]
+    )
+    sentences = sentences.with_columns(
+        [
+            pl.when(pl.col("Type")=="C")
+            .then("")
+            .otherwise(pl.col("Type"))
+            .alias("Type"),
+            pl.when(pl.col("Type")=="C")
+            .then(pl.concat_str([pl.lit("C"),pl.col("County")]))
+            .otherwise(pl.col("County"))
+            .alias("County")
+        ]
+    )
+    details = details.with_columns(pl.col("Tables").str.split("\n"))
+    details = details.explode("Tables")
+    details = details.filter(pl.col("Tables").str.contains("Admit Date").is_not())
+    details = details.filter(pl.col("Tables").str.contains("[A-Z]"))
+    details = details.select(
+        [
+            pl.col("row_nr"),
+            pl.col("Tables").str.extract(r'^([A-Z])').alias("SUF"),
+            pl.col("Tables").str.extract(r'^[A-Z]? ?(\d\d/\d\d/\d\d\d\d)').str.to_date('%m/%d/%Y', strict=False).alias("AdmitDate"),
+            pl.col("Tables").str.extract(r'^[A-Z]? ?\d\d/\d\d/\d\d\d\d (\d+Y \d+M \d+D)').alias("TotalTerm"),
+            pl.col("Tables").str.extract(r'^[A-Z]? ?\d\d/\d\d/\d\d\d\d \d+Y \d+M \d+D (\d+Y \d+M \d+D)').alias("TimeServed"),
+            pl.col("Tables").str.extract(r'^[A-Z]? ?\d\d/\d\d/\d\d\d\d \d+Y \d+M \d+D \d+Y \d+M \d+D (\d+)').alias("JailCredit"),
+            pl.col("Tables").str.extract(r'^[A-Z]? ?\d\d/\d\d/\d\d\d\d \d+Y \d+M \d+D \d+Y \d+M \d+D \d+ ?(\d* ?D?a?y?s?\d*Y? ?\d*M? ?\d*D?)').str.replace(r'Days .+','Days').alias("GoodTimeReceived"),
+            pl.col("Tables").str.extract(r'^[A-Z]? ?\d\d/\d\d/\d\d\d\d \d+Y \d+M \d+D \d+Y \d+M \d+D \d+ ?(\d* ?D?a?y?s?\d*Y? ?\d*M? ?\d*D? ?\d* ?D?a?y?s?\d*Y? ?\d*M? ?\d*D?)').str.replace(r'^\d Days','').str.replace(r'^\d+Y \d+M \d+D','').str.replace(r'Days .+','Days').str.strip().alias("GoodTimeRevoked"),
+            pl.col("Tables").str.extract(r'^[A-Z]? ?\d\d/\d\d/\d\d\d\d \d+Y \d+M \d+D \d+Y \d+M \d+D \d+ ?\d* ?D?a?y?s?\d*Y? ?\d*M? ?\d*D? ?\d* ?D?a?y?s?\d*Y? ?\d*M? ?\d*D? (\d\d/\d\d/\d\d\d\d)').str.to_date('%m/%d/%Y', strict=False).alias("MinReleaseDate"),
+            pl.col("Tables").str.extract(r'^[A-Z]? ?\d\d/\d\d/\d\d\d\d \d+Y \d+M \d+D \d+Y \d+M \d+D \d+ ?\d* ?D?a?y?s?\d*Y? ?\d*M? ?\d*D? ?\d* ?D?a?y?s?\d*Y? ?\d*M? ?\d*D? \d\d/\d\d/\d\d\d\d (\d?\d?/?\d?\d?/?\d?\d?\d?\d?)').str.to_date('%m/%d/%Y', strict=False).alias("ParoleConsiderationDate"),
+            pl.col("Tables").str.extract(r'^[A-Z]? ?\d\d/\d\d/\d\d\d\d \d+Y \d+M \d+D \d+Y \d+M \d+D \d+ ?\d* ?D?a?y?s?\d*Y? ?\d*M? ?\d*D? ?\d* ?D?a?y?s?\d*Y? ?\d*M? ?\d*D? \d\d/\d\d/\d\d\d\d \d?\d?/?\d?\d?/?\d?\d?\d?\d? (.+)').str.strip().alias("ParoleStatus")
+        ]
+    )
+    sentences = sentences.join(details, how="left", on="row_nr")
+    sentences = sentences.with_columns(pl.lit(0).alias("Match"))
+    inmate = inmate.with_columns(pl.lit(0).alias("Match"))
+    sentences = sentences.join(inmate, how="left", on="Match").select(pl.exclude("Match", "row_nr"))
+    sentences = sentences.select("CaseNo","Name","AIS","Institution","Race","Sex","HairColor","EyeColor","Height","Weight","BirthYear","Custody","Sentenced","Offense","Term","SentenceJailCredit","Type","County","SUF","AdmitDate","TotalTerm","TimeServed","JailCredit","GoodTimeReceived","GoodTimeRevoked","MinReleaseDate","ParoleConsiderationDate","ParoleStatus")
+    return sentences
+
 def crawl_adoc(path):
     alphabet = ['A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T', 'U', 'V', 'W', 'X', 'Y', 'Z']
     print("Connecting to ADOC...")
     driver = webdriver.Chrome()
     driver.get("http://www.doc.state.al.us/inmatesearch")
     results = []
     for x in alphabet:
@@ -3802,14 +3997,15 @@
                 "RETRIEVED": [],
                 "CASES_FOUND": []
             }
     )
     return write(empty, sheet_names="query", path=path, overwrite=True)
 
 
+
 #   #   #   #      GRAPHICAL USER INTERFACE    #   #   #   #
 
 
 def loadgui():
     """
     Load PySimpleGUI tk graphical interface
     """
@@ -4527,14 +4723,42 @@
         loadgui()
 
 
 @main.command(name="start", help="Launch graphical user interface")
 def _cli_start():
     loadgui()
 
+@main.command(name="search-adoc", help="Retrieve records from ADOC Inmate Search")
+@click.option(
+    "--input-path",
+    "-query",
+    "query",
+    required=True,
+    prompt="Path to query spreadsheet",
+    help="Path to query spreadsheet",
+    type=click.Path()
+)
+@click.option(
+    "--output-path",
+    "-out",
+    "out",
+    required=True,
+    prompt="Output spreadsheet path",
+    help="Output spreadsheet path",
+    type=click.Path()
+)
+def _cli_adoc_fetch(query, out):
+    """
+    Retrieve tables from ADOC Inmate Search
+    
+    Args:
+        query (Path|DataFrame): Path to input query spreadsheet
+        out (Path): Path to output spreadsheet
+    """
+    return adoc_fetch(query, out)
 
 @main.command(name="append", help="Append one case text archive to another")
 @click.option(
     "--input-path",
     "-in",
     "in_path",
     required=True,
@@ -4570,15 +4794,15 @@
     Returns:
         DataFrame: Appended archive
     """
     arc = append_archive(in_path, out_path)
     print("Completed task.")
     return arc
 
-@main.command(name="crawl", help="Retrieve current inmates list from ADOC")
+@main.command(name="crawl-adoc", help="Retrieve current inmates list from ADOC")
 @click.option(
     "--path",
     "-out",
     "path",
     required=True,
     prompt="Output table path",
     help="Path to output table",
```

### Comparing `alacorder-80.7.9/src/alacorder/alac.py` & `alacorder-80.8.0/src/alacorder/alac.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Optional dependencies:
     pyarrow required to export summary to .xls, .xlsx,
     Google Chrome required to fetch cases from Alacourt and crawl ADOC
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.7.9"
+version = "80.8.0"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -3272,14 +3272,209 @@
         return query
     else:
         print(
             "Try again with at least one valid column header: [NAME, PARTY_TYPE, SSN, DOB, COUNTY, DIVISION, CASE_YEAR, NO_RECORDS, FILED_BEFORE, FILED_AFTER, RETRIEVED, CASES_FOUND, QUERY_COMPLETE]"
         )
         return None
 
+
+def make_fetch_queue_from_crawl(df):
+    if isinstance(df, str):
+        df = read(df)
+    df = df.select(
+        [
+            pl.col("AIS"),
+            pl.col("Name").str.extract(r', ([A-Z]+)').alias("FirstName"),
+            pl.col("Name").str.extract(r'^([A-Z]+)').alias("LastName"),
+        ]
+    )
+    return df
+
+def adoc_fetch(df=None, path=None, cf=None):
+    if cf:
+        df = read(cf['INPUTS'])
+        path = cf['OUTPUT_PATH']
+    if df:
+        if isinstance(df, str):
+            dfpath = df
+            df = read(df)
+        else:
+            dfpath = None
+    if 'Retrieved' not in df.columns:
+        df = df.select("AIS", "FirstName", "LastName")
+        df = df.with_columns(pl.lit("").alias("Retrieved"))
+    df = df.with_columns(pl.col("AIS").cast(pl.Utf8, strict=False))
+    out = pl.DataFrame()
+    driver = webdriver.Chrome()
+    for i, r in enumerate(tqdm(df.rows(named=True))):
+        if r['Retrieved'] != '' and r['Retrieved'] != None:
+            continue
+        try:
+            out = pl.concat([out, read_top_result(driver, r['AIS'], r['FirstName'], r['LastName'])])
+        except:
+            pass
+        df[i, 'Retrieved'] = datetime.now().strftime("%d-%m-%Y %H:%M:%S")
+        if dfpath and df.shape[0] > 10 and i % 10 == 0:
+            write(df, sheet_names=["adoc_progress"], path=dfpath)
+        if df.shape[0] > 10 and i % 10 == 0 and path:
+            write(out, sheet_names=["adoc"], path=path)
+    if path:
+        write(out, sheet_names=["adoc"], path=path)
+    if dfpath:
+        write(df, sheet_names=["adoc_progress"], path=dfpath)
+    return out, df
+
+def read_top_result(driver, ais, first, last):
+    driver.get("http://www.doc.state.al.us/inmatesearch")
+    ais_box = driver.find_element(by=By.NAME, value="ctl00$MainContent$txtAIS")
+    first_name_box = driver.find_element(by=By.NAME, value="ctl00$MainContent$txtFName")
+    last_name_box = driver.find_element(by=By.NAME, value="ctl00$MainContent$txtLName")
+    send_button = driver.find_element(by=By.NAME, value="ctl00$MainContent$btnSearch")
+    ais_box.send_keys(ais)
+    first_name_box.send_keys(first)
+    last_name_box.send_keys(last)
+    send_button.click()
+    urls = driver.find_elements(by=By.TAG_NAME, value="a")
+    results = []
+    for x in urls:
+        try:
+            if 'InmateResults' in x.get_attribute("ID"):
+                results += [x]
+        except:
+            pass
+    try:
+        results[0].click()
+        return read_adoc_page(driver)
+    except:
+        return pl.DataFrame()
+
+
+def filter_missing_cases(adoc_df, cases_df):
+    if isinstance(adoc_df, str):
+        adoc_df = read(adoc_df)
+    if isinstance(cases_df, str):
+        cases_df = read(cases_df)
+    if 'AllPagesText' in cases_df.columns:
+        cases_df = set(cases_df, table="cases", now=True)
+    cases_df = cases_df.with_columns(
+        pl.col("CaseNumber").str.extract(r'(\w\w-\d\d\d\d-\d\d\d\d\d\d)').alias("CaseNoFragment")
+    )
+    clist = cases_df.select("CaseNoFragment").to_series().to_list()
+    cmap = pl.DataFrame(
+        {
+            'Selection': ['94 - ARDMORE', '93 - ATHENS', '04 - AUTAUGA', '05 - BALDWIN', '06 - BARBOUR - CLAYTON', '69 - BARBOUR - EUFAULA', '89 - BERRY', '07 - BIBB', '08 - BLOUNT', '87 - BRUNDIDGE MUNICIPAL COURT', '09 - BULLOCK', '10 - BUTLER', '11 - CALHOUN', '12 - CHAMBERS', '13 - CHEROKEE', '90 - CHEROKEE', '14 - CHILTON', '15 - CHOCTAW', '16 - CLARKE', '17 - CLAY', '18 - CLEBURNE', '19 - COFFEE - ELBA', '71 - COFFEE - ENTERPRISE', '20 - COLBERT', '21 - CONECUH', '22 - COOSA', '23 - COVINGTON', '24 - CRENSHAW', '25 - CULLMAN', '26 - DALE', '27 - DALLAS', '28 - DeKALB', '29 - ELMORE', '30 - ESCAMBIA', '31 - ETOWAH', '32 - FAYETTE', '33 - FRANKLIN', '34 - GENEVA', '35 - GREENE', '36 - HALE', '37 - HENRY', '38 - HOUSTON', '39 - JACKSON', '68 - JEFFERSON - BESSEMER', '01 - JEFFERSON - BIRMINGHAM', '40 - LAMAR', '41 - LAUDERDALE', '42 - LAWRENCE', '43 - LEE', '44 - LIMESTONE', '82 - LIVINGSTON', '45 - LOWNDES', '46 - MACON', '47 - MADISON', '48 - MARENGO', '49 - MARION', '50 - MARSHALL', '92 - MILLBROOK', '02 - MOBILE', '51 - MONROE', '03 - MONTGOMERY', '52 - MORGAN', '53 - PERRY', '80 - PHENIX CITY', '54 - PICKENS', '55 - PIKE', '88 - PRATTVILLE', '56 - RANDOLPH', '57 - RUSSELL', '58 - SHELBY', '59 - ST. CLAIR - ASHVILLE', '75 - ST. CLAIR - PELL CITY', '81 - SUMITON MUNICIPAL COURT', '60 - SUMTER', '74 - TALLADEGA - SYLACAUGA', '61 - TALLADEGA - TALLADEGA', '70 - TALLAPOOSA - ALEX CITY', '62 - TALLAPOOSA - DADEVILLE', '63 - TUSCALOOSA', '64 - WALKER', '65 - WASHINGTON', '95 - WETUMPKA MUNICIPAL COURT', '66 - WILCOX', '67 - WINSTON'],
+            'CountyNumber': ['94', '93', '04', '05', '06', '69', '89', '07', '08', '87', '09', '10', '11', '12', '13', '90', '14', '15', '16', '17', '18', '19', '71', '20', '21', '22', '23', '24', '25', '26', '27', '28', '29', '30', '31', '32', '33', '34', '35', '36', '37', '38', '39', '68', '01', '40', '41', '42', '43', '44', '82', '45', '46', '47', '48', '49', '50', '92', '02', '51', '03', '52', '53', '80', '54', '55', '88', '56', '57', '58', '59', '75', '81', '60', '74', '61', '70', '62', '63', '64', '65', '95', '66', '67'],
+            'County': ['ARDMORE', 'ATHENS', 'AUTAUGA', 'BALDWIN', 'BARBOUR - CLAYTON', 'BARBOUR - EUFAULA', 'BERRY', 'BIBB', 'BLOUNT', 'BRUNDIDGE MUNICIPAL COURT', 'BULLOCK', 'BUTLER', 'CALHOUN', 'CHAMBERS', 'CHEROKEE', 'CHEROKEE', 'CHILTON', 'CHOCTAW', 'CLARKE', 'CLAY', 'CLEBURNE', 'COFFEE - ELBA', 'COFFEE - ENTERPRISE', 'COLBERT', 'CONECUH', 'COOSA', 'COVINGTON', 'CRENSHAW', 'CULLMAN', 'DALE', 'DALLAS', 'DeKALB', 'ELMORE', 'ESCAMBIA', 'ETOWAH', 'FAYETTE', 'FRANKLIN', 'GENEVA', 'GREENE', 'HALE', 'HENRY', 'HOUSTON', 'JACKSON', 'JEFFERSON - BESSEMER', 'JEFFERSON - BIRMINGHAM', 'LAMAR', 'LAUDERDALE', 'LAWRENCE', 'LEE', 'LIMESTONE', 'LIVINGSTON', 'LOWNDES', 'MACON', 'MADISON', 'MARENGO', 'MARION', 'MARSHALL', 'MILLBROOK', 'MOBILE', 'MONROE', 'MONTGOMERY', 'MORGAN', 'PERRY', 'PHENIX CITY', 'PICKENS', 'PIKE', 'PRATTVILLE', 'RANDOLPH', 'RUSSELL', 'SHELBY', 'ST. CLAIR - ASHVILLE', 'ST. CLAIR - PELL CITY', 'SUMITON MUNICIPAL COURT', 'SUMTER', 'TALLADEGA - SYLACAUGA', 'TALLADEGA - TALLADEGA', 'TALLAPOOSA - ALEX CITY', 'TALLAPOOSA - DADEVILLE', 'TUSCALOOSA', 'WALKER', 'WASHINGTON', 'WETUMPKA MUNICIPAL COURT', 'WILCOX', 'WINSTON'] 
+        }
+    )
+    adoc_df = adoc_df.join(cmap, on="County", how="left")
+    adoc_df = adoc_df.with_columns(
+        pl.concat_str(
+            [
+                pl.col("CountyNumber"),
+                pl.lit("-"),
+                pl.col("CaseNo").str.extract(r"(\w\w)"),
+                pl.lit("-"),
+                pl.col("CaseNo").str.extract(r'(\d\d\d\d)\-'),
+                pl.lit("-"),
+                pl.col("CaseNo").str.extract(r'\-(\d\d\d\d\d\d)'),
+            ]
+        ).alias("CaseNoFragment")
+    )
+    out = adoc_df.filter(pl.col("CaseNoFragment").is_in(clist).is_not())
+    out = out.filter(pl.col("CaseNoFragment").is_null().is_not())
+    return out
+
+def read_adoc_page(driver):
+    rl = driver.find_elements(by=By.TAG_NAME, value="tr")
+    alltxt = []
+    for r in rl:
+        alltxt += [r.text]
+    name = driver.find_element(by=By.ID, value="MainContent_DetailsView2_Label1").text
+    allt = pl.DataFrame({'Tables': "\n".join(alltxt)})
+    allt = allt.with_columns(pl.col("Tables").str.split("SUF"))
+    allt = allt.explode("Tables")
+    allt = allt.with_columns(pl.col("Tables").str.split("Sentences"))
+    allt = allt.explode("Tables")
+    details = allt.filter(pl.col("Tables").str.contains("Date Total Term"))
+    sentences = allt.filter(pl.col("Tables").str.contains("Sentenced"))
+    inmate = allt.filter(pl.col("Tables").str.contains("Eye Color"))
+    sentences = sentences.with_row_count()
+    details = details.with_row_count()
+    inmate = inmate.select(
+        [
+            pl.lit(name).alias("Name"),
+            pl.col("Tables").str.extract(r'AIS:\s+(\d{8})').alias("AIS"),
+            pl.col("Tables").str.extract(r'Institution: ([A-Z\s]+)').alias("Institution"
+             ),
+            pl.col("Tables").str.extract(r'Race: ([A-Z])').alias("Race"),
+            pl.col("Tables").str.extract(r'Sex: ([A-Z])').alias("Sex"),
+            pl.col("Tables").str.extract(r'Hair Color: ([A-Z]+)').alias("HairColor"),
+            pl.col("Tables").str.extract(r'Eye Color: ([A-Z]+)').alias("EyeColor"),
+            pl.col("Tables").str.extract(r'Height: (.+)').alias("Height"),
+            pl.col("Tables").str.extract(r'Weight: (\d+)').alias("Weight"),
+            pl.col("Tables").str.extract(r'Birth Year: (\d\d\d\d)').alias("BirthYear"),
+            pl.col("Tables").str.extract(r'Custody (.+)').alias("Custody")
+        ]
+    )
+    sentences = sentences.with_columns(pl.col("Tables").str.split('\n'))
+    sentences = sentences.explode("Tables")
+    sentences = sentences.filter(pl.col("Tables").str.contains("[A-Z]"))
+    sentences = sentences.filter(pl.col("Tables").str.contains("Sentenced").is_not())
+    sentences = sentences.unique()
+    sentences = sentences.select(
+        [
+            pl.col("row_nr"),
+            pl.col("Tables").str.extract(r'([^\s]+)').alias("CaseNo"),
+            pl.col("Tables").str.extract(r'(\d\d?/\d\d?/\d\d\d\d)').str.to_date('%m/%d/%Y', strict=False).alias("Sentenced"),
+            pl.col("Tables").str.extract(r'\d\d?/\d\d?/\d\d\d\d (.+?) \d+Y \d+M \d+D').alias("Offense"),
+            pl.col("Tables").str.extract(r'\d\d?/\d\d?/\d\d\d\d .+? (\d+Y \d+M \d+D)').alias("Term"),
+            pl.col("Tables").str.extract(r'\d\d?/\d\d?/\d\d\d\d .+? \d+Y \d+M \d+D (\d+)').cast(pl.Int64, strict=False).alias("SentenceJailCredit"),
+            pl.col("Tables").str.extract(r'\d\d?/\d\d?/\d\d\d\d .+? \d+Y \d+M \d+D \d+ \d* ?(C?o?n?c?u?r?r?e?n?t?)').alias("Type"),
+            pl.col("Tables").str.extract(r'\d\d?/\d\d?/\d\d\d\d .+? \d+Y \d+M \d+D \d+ \d* ?C?o?n?c?u?r?r?e?n?t? ?([A-Z]+)').alias("County")
+        ]
+    )
+    sentences = sentences.with_columns(
+        [
+            pl.when(pl.col("Type")=="C")
+            .then("")
+            .otherwise(pl.col("Type"))
+            .alias("Type"),
+            pl.when(pl.col("Type")=="C")
+            .then(pl.concat_str([pl.lit("C"),pl.col("County")]))
+            .otherwise(pl.col("County"))
+            .alias("County")
+        ]
+    )
+    details = details.with_columns(pl.col("Tables").str.split("\n"))
+    details = details.explode("Tables")
+    details = details.filter(pl.col("Tables").str.contains("Admit Date").is_not())
+    details = details.filter(pl.col("Tables").str.contains("[A-Z]"))
+    details = details.select(
+        [
+            pl.col("row_nr"),
+            pl.col("Tables").str.extract(r'^([A-Z])').alias("SUF"),
+            pl.col("Tables").str.extract(r'^[A-Z]? ?(\d\d/\d\d/\d\d\d\d)').str.to_date('%m/%d/%Y', strict=False).alias("AdmitDate"),
+            pl.col("Tables").str.extract(r'^[A-Z]? ?\d\d/\d\d/\d\d\d\d (\d+Y \d+M \d+D)').alias("TotalTerm"),
+            pl.col("Tables").str.extract(r'^[A-Z]? ?\d\d/\d\d/\d\d\d\d \d+Y \d+M \d+D (\d+Y \d+M \d+D)').alias("TimeServed"),
+            pl.col("Tables").str.extract(r'^[A-Z]? ?\d\d/\d\d/\d\d\d\d \d+Y \d+M \d+D \d+Y \d+M \d+D (\d+)').alias("JailCredit"),
+            pl.col("Tables").str.extract(r'^[A-Z]? ?\d\d/\d\d/\d\d\d\d \d+Y \d+M \d+D \d+Y \d+M \d+D \d+ ?(\d* ?D?a?y?s?\d*Y? ?\d*M? ?\d*D?)').str.replace(r'Days .+','Days').alias("GoodTimeReceived"),
+            pl.col("Tables").str.extract(r'^[A-Z]? ?\d\d/\d\d/\d\d\d\d \d+Y \d+M \d+D \d+Y \d+M \d+D \d+ ?(\d* ?D?a?y?s?\d*Y? ?\d*M? ?\d*D? ?\d* ?D?a?y?s?\d*Y? ?\d*M? ?\d*D?)').str.replace(r'^\d Days','').str.replace(r'^\d+Y \d+M \d+D','').str.replace(r'Days .+','Days').str.strip().alias("GoodTimeRevoked"),
+            pl.col("Tables").str.extract(r'^[A-Z]? ?\d\d/\d\d/\d\d\d\d \d+Y \d+M \d+D \d+Y \d+M \d+D \d+ ?\d* ?D?a?y?s?\d*Y? ?\d*M? ?\d*D? ?\d* ?D?a?y?s?\d*Y? ?\d*M? ?\d*D? (\d\d/\d\d/\d\d\d\d)').str.to_date('%m/%d/%Y', strict=False).alias("MinReleaseDate"),
+            pl.col("Tables").str.extract(r'^[A-Z]? ?\d\d/\d\d/\d\d\d\d \d+Y \d+M \d+D \d+Y \d+M \d+D \d+ ?\d* ?D?a?y?s?\d*Y? ?\d*M? ?\d*D? ?\d* ?D?a?y?s?\d*Y? ?\d*M? ?\d*D? \d\d/\d\d/\d\d\d\d (\d?\d?/?\d?\d?/?\d?\d?\d?\d?)').str.to_date('%m/%d/%Y', strict=False).alias("ParoleConsiderationDate"),
+            pl.col("Tables").str.extract(r'^[A-Z]? ?\d\d/\d\d/\d\d\d\d \d+Y \d+M \d+D \d+Y \d+M \d+D \d+ ?\d* ?D?a?y?s?\d*Y? ?\d*M? ?\d*D? ?\d* ?D?a?y?s?\d*Y? ?\d*M? ?\d*D? \d\d/\d\d/\d\d\d\d \d?\d?/?\d?\d?/?\d?\d?\d?\d? (.+)').str.strip().alias("ParoleStatus")
+        ]
+    )
+    sentences = sentences.join(details, how="left", on="row_nr")
+    sentences = sentences.with_columns(pl.lit(0).alias("Match"))
+    inmate = inmate.with_columns(pl.lit(0).alias("Match"))
+    sentences = sentences.join(inmate, how="left", on="Match").select(pl.exclude("Match", "row_nr"))
+    sentences = sentences.select("CaseNo","Name","AIS","Institution","Race","Sex","HairColor","EyeColor","Height","Weight","BirthYear","Custody","Sentenced","Offense","Term","SentenceJailCredit","Type","County","SUF","AdmitDate","TotalTerm","TimeServed","JailCredit","GoodTimeReceived","GoodTimeRevoked","MinReleaseDate","ParoleConsiderationDate","ParoleStatus")
+    return sentences
+
 def crawl_adoc(path):
     alphabet = ['A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T', 'U', 'V', 'W', 'X', 'Y', 'Z']
     print("Connecting to ADOC...")
     driver = webdriver.Chrome()
     driver.get("http://www.doc.state.al.us/inmatesearch")
     results = []
     for x in alphabet:
@@ -3802,14 +3997,15 @@
                 "RETRIEVED": [],
                 "CASES_FOUND": []
             }
     )
     return write(empty, sheet_names="query", path=path, overwrite=True)
 
 
+
 #   #   #   #      GRAPHICAL USER INTERFACE    #   #   #   #
 
 
 def loadgui():
     """
     Load PySimpleGUI tk graphical interface
     """
@@ -4527,14 +4723,42 @@
         loadgui()
 
 
 @main.command(name="start", help="Launch graphical user interface")
 def _cli_start():
     loadgui()
 
+@main.command(name="search-adoc", help="Retrieve records from ADOC Inmate Search")
+@click.option(
+    "--input-path",
+    "-query",
+    "query",
+    required=True,
+    prompt="Path to query spreadsheet",
+    help="Path to query spreadsheet",
+    type=click.Path()
+)
+@click.option(
+    "--output-path",
+    "-out",
+    "out",
+    required=True,
+    prompt="Output spreadsheet path",
+    help="Output spreadsheet path",
+    type=click.Path()
+)
+def _cli_adoc_fetch(query, out):
+    """
+    Retrieve tables from ADOC Inmate Search
+    
+    Args:
+        query (Path|DataFrame): Path to input query spreadsheet
+        out (Path): Path to output spreadsheet
+    """
+    return adoc_fetch(query, out)
 
 @main.command(name="append", help="Append one case text archive to another")
 @click.option(
     "--input-path",
     "-in",
     "in_path",
     required=True,
@@ -4570,15 +4794,15 @@
     Returns:
         DataFrame: Appended archive
     """
     arc = append_archive(in_path, out_path)
     print("Completed task.")
     return arc
 
-@main.command(name="crawl", help="Retrieve current inmates list from ADOC")
+@main.command(name="crawl-adoc", help="Retrieve current inmates list from ADOC")
 @click.option(
     "--path",
     "-out",
     "path",
     required=True,
     prompt="Output table path",
     help="Path to output table",
```

### Comparing `alacorder-80.7.9/PKG-INFO` & `alacorder-80.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 80.7.9
+Version: 80.8.0
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

