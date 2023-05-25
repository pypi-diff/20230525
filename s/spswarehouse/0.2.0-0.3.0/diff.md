# Comparing `tmp/spswarehouse-0.2.0.tar.gz` & `tmp/spswarehouse-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spswarehouse-0.2.0.tar", last modified: Wed May 17 18:23:46 2023, max compression
+gzip compressed data, was "spswarehouse-0.3.0.tar", last modified: Thu May 25 16:11:54 2023, max compression
```

## Comparing `spswarehouse-0.2.0.tar` & `spswarehouse-0.3.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 18:23:46.296330 spswarehouse-0.2.0/
--rw-rw-rw-   0        0        0    35823 2022-12-01 20:45:52.000000 spswarehouse-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      448 2022-12-01 20:45:52.000000 spswarehouse-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     8200 2023-05-17 18:23:46.295329 spswarehouse-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     7815 2022-12-01 20:45:52.000000 spswarehouse-0.2.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-17 18:23:46.296330 spswarehouse-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      744 2023-05-17 18:23:32.000000 spswarehouse-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-17 18:23:46.274335 spswarehouse-0.2.0/spswarehouse/
--rw-rw-rw-   0        0        0      561 2023-05-09 15:39:49.000000 spswarehouse-0.2.0/spswarehouse/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 18:23:46.286327 spswarehouse-0.2.0/spswarehouse/calpads/
--rw-rw-rw-   0        0        0        0 2023-05-17 18:23:32.000000 spswarehouse-0.2.0/spswarehouse/calpads/__init__.py
--rw-rw-rw-   0        0        0    36069 2023-05-17 18:23:32.000000 spswarehouse-0.2.0/spswarehouse/calpads/calpads.py
--rw-rw-rw-   0        0        0     5792 2023-05-17 18:23:32.000000 spswarehouse-0.2.0/spswarehouse/calpads/calpads_config.py
--rw-rw-rw-   0        0        0     1035 2023-05-08 23:22:00.000000 spswarehouse-0.2.0/spswarehouse/credentials.py.template
--rw-rw-rw-   0        0        0     2090 2023-05-09 15:48:20.000000 spswarehouse-0.2.0/spswarehouse/googledrive.py
--rw-rw-rw-   0        0        0     1980 2023-05-09 15:48:34.000000 spswarehouse-0.2.0/spswarehouse/googlesheets.py
--rw-rw-rw-   0        0        0     2013 2023-05-09 15:50:01.000000 spswarehouse-0.2.0/spswarehouse/googleslides.py
-drwxrwxrwx   0        0        0        0 2023-05-17 18:23:46.292328 spswarehouse-0.2.0/spswarehouse/powerschool/
--rw-rw-rw-   0        0        0        0 2023-05-08 23:11:00.000000 spswarehouse-0.2.0/spswarehouse/powerschool/__init__.py
--rw-rw-rw-   0        0        0    21622 2023-05-17 17:25:10.000000 spswarehouse-0.2.0/spswarehouse/powerschool/powerschool.py
--rw-rw-rw-   0        0        0    29877 2023-05-15 20:19:39.000000 spswarehouse-0.2.0/spswarehouse/powerschool/powerschool_calpads.py
--rw-rw-rw-   0        0        0      302 2023-05-17 18:23:32.000000 spswarehouse-0.2.0/spswarehouse/requirements.txt
--rw-rw-rw-   0        0        0     1269 2022-12-01 20:45:52.000000 spswarehouse-0.2.0/spswarehouse/table_names.py
--rw-rw-rw-   0        0        0     7809 2023-05-09 15:47:54.000000 spswarehouse-0.2.0/spswarehouse/table_utils.py
--rw-rw-rw-   0        0        0     4689 2023-05-09 15:45:39.000000 spswarehouse-0.2.0/spswarehouse/warehouse.py
-drwxrwxrwx   0        0        0        0 2023-05-17 18:23:46.281380 spswarehouse-0.2.0/spswarehouse.egg-info/
--rw-rw-rw-   0        0        0     8200 2023-05-17 18:23:45.000000 spswarehouse-0.2.0/spswarehouse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      671 2023-05-17 18:23:46.000000 spswarehouse-0.2.0/spswarehouse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 18:23:45.000000 spswarehouse-0.2.0/spswarehouse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-17 18:23:45.000000 spswarehouse-0.2.0/spswarehouse.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-25 16:11:54.461835 spswarehouse-0.3.0/
+-rw-rw-rw-   0        0        0    35823 2022-12-01 20:45:52.000000 spswarehouse-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0      448 2022-12-01 20:45:52.000000 spswarehouse-0.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     8200 2023-05-25 16:11:54.459868 spswarehouse-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7815 2022-12-01 20:45:52.000000 spswarehouse-0.3.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-25 16:11:54.461835 spswarehouse-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      744 2023-05-25 16:11:09.000000 spswarehouse-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 16:11:54.439070 spswarehouse-0.3.0/spswarehouse/
+-rw-rw-rw-   0        0        0      561 2023-05-09 15:39:49.000000 spswarehouse-0.3.0/spswarehouse/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 16:11:54.450861 spswarehouse-0.3.0/spswarehouse/calpads/
+-rw-rw-rw-   0        0        0        0 2023-05-17 18:23:32.000000 spswarehouse-0.3.0/spswarehouse/calpads/__init__.py
+-rw-rw-rw-   0        0        0    40625 2023-05-25 16:11:09.000000 spswarehouse-0.3.0/spswarehouse/calpads/calpads.py
+-rw-rw-rw-   0        0        0     6136 2023-05-25 16:11:09.000000 spswarehouse-0.3.0/spswarehouse/calpads/calpads_config.py
+-rw-rw-rw-   0        0        0     1035 2023-05-08 23:22:00.000000 spswarehouse-0.3.0/spswarehouse/credentials.py.template
+-rw-rw-rw-   0        0        0     2090 2023-05-09 15:48:20.000000 spswarehouse-0.3.0/spswarehouse/googledrive.py
+-rw-rw-rw-   0        0        0     1980 2023-05-09 15:48:34.000000 spswarehouse-0.3.0/spswarehouse/googlesheets.py
+-rw-rw-rw-   0        0        0     2013 2023-05-09 15:50:01.000000 spswarehouse-0.3.0/spswarehouse/googleslides.py
+drwxrwxrwx   0        0        0        0 2023-05-25 16:11:54.456868 spswarehouse-0.3.0/spswarehouse/powerschool/
+-rw-rw-rw-   0        0        0        0 2023-05-08 23:11:00.000000 spswarehouse-0.3.0/spswarehouse/powerschool/__init__.py
+-rw-rw-rw-   0        0        0    21622 2023-05-17 17:25:10.000000 spswarehouse-0.3.0/spswarehouse/powerschool/powerschool.py
+-rw-rw-rw-   0        0        0    29877 2023-05-15 20:19:39.000000 spswarehouse-0.3.0/spswarehouse/powerschool/powerschool_calpads.py
+-rw-rw-rw-   0        0        0      302 2023-05-17 18:23:32.000000 spswarehouse-0.3.0/spswarehouse/requirements.txt
+-rw-rw-rw-   0        0        0     1269 2022-12-01 20:45:52.000000 spswarehouse-0.3.0/spswarehouse/table_names.py
+-rw-rw-rw-   0        0        0     7809 2023-05-09 15:47:54.000000 spswarehouse-0.3.0/spswarehouse/table_utils.py
+-rw-rw-rw-   0        0        0     4689 2023-05-09 15:45:39.000000 spswarehouse-0.3.0/spswarehouse/warehouse.py
+drwxrwxrwx   0        0        0        0 2023-05-25 16:11:54.446273 spswarehouse-0.3.0/spswarehouse.egg-info/
+-rw-rw-rw-   0        0        0     8200 2023-05-25 16:11:54.000000 spswarehouse-0.3.0/spswarehouse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      671 2023-05-25 16:11:54.000000 spswarehouse-0.3.0/spswarehouse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 16:11:54.000000 spswarehouse-0.3.0/spswarehouse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-25 16:11:54.000000 spswarehouse-0.3.0/spswarehouse.egg-info/top_level.txt
```

### Comparing `spswarehouse-0.2.0/LICENSE` & `spswarehouse-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.2.0/PKG-INFO` & `spswarehouse-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spswarehouse
-Version: 0.2.0
+Version: 0.3.0
 Summary: Summit Public Schools Snowflake warehouse
 Home-page: https://github.com/SummitPublicSchools/spswarehouse
 Author: Summit Public Schools; Harry Li Consulting, LLC
 Author-email: warehouse@summitps.org
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `spswarehouse-0.2.0/README.md` & `spswarehouse-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.2.0/setup.py` & `spswarehouse-0.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="spswarehouse",
-    version="0.2.0",
+    version="0.3.0",
     author="Summit Public Schools; Harry Li Consulting, LLC",
     author_email="warehouse@summitps.org",
     description="Summit Public Schools Snowflake warehouse",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/SummitPublicSchools/spswarehouse",
     packages=setuptools.find_packages(),
```

### Comparing `spswarehouse-0.2.0/spswarehouse/__init__.py` & `spswarehouse-0.3.0/spswarehouse/__init__.py`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.2.0/spswarehouse/calpads/calpads.py` & `spswarehouse-0.3.0/spswarehouse/calpads/calpads.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Code adapted from original code by Yusuph in the dops-calpad repo
 
 # Author: Howard Shen
-# Last Edited 5/8/2023
+# Last Edited 5/25/2023
 
 import logging
 import os
 import pandas as pd
 import tempfile
 import time
 
@@ -29,16 +29,18 @@
     
 try:
     from spswarehouse.credentials import calpads_config
 except ModuleNotFoundError:
     print("No credentials file found in spswarehouse. This could cause issues.")
 
 from spswarehouse.calpads.calpads_config import (
+    monitoring_report_base,
+    monitoring_links,
     snapshot_report_base,
-    snapshot_links
+    snapshot_links,
 )
     
 class CALPADS():
     
     def __init__(
         self,
         config=None,
@@ -572,14 +574,65 @@
             return True, error_df, warning_df
         elif error_and_warn_count == 0:
             logging.info(f"No errors or warnings for {submission_name}")
             return True, None, None
         else:
             raise RuntimeError("Impossible part of error_and_warn_count if-elif-else reached.")
 
+    def download_monitoring_report(
+        self,
+        lea,
+        academic_year,
+        report_code,
+        report_date=None,
+        download_type='csv',
+        max_wait_time=10
+    ):
+        """
+        Download a CALPADS snapshot report.
+        
+        Known issue: The download folder needs to be empty when this function is called.
+        
+        Parameters:
+        lea: The numerical value of the LEA on the CALPADS site. Find by inspecting the
+            dropdown on the CALPADS page.
+        academic_year: Integer representing the academic year that you want to check
+            (per team norms, this is the year when the school year ends)
+        submission_name: The name of the certification window. As of this edit, the
+            certification windows are Fall1, Fall2, EOY1, EOY2, EOY3, and EOY4.
+        report_code: The code for the report that you want. Should be a string in
+            the form of "#.#". Check calpads_config.py for the list of available
+            report_code + submission_name combos
+        report_date (str): An ISO format date string ('YYYY-MM-DD') indicating the 
+            desired date for the report. If None, the function will download whatever
+            the default date on the report is (usually today).
+            Note that the function only uses the month and day. (E.g., if you pass
+            academic_year=2023 and report_date="2024-10-01", the report downloaded will be
+            for October 1 of academic year 2023, which is actually "2022-10-01")
+        download_type (str): The format in which you want the download for the report.
+            Currently supports csv, excel, and pdf.
+        max_wait_time: Integer >=0 indicating the maximum number of minutes to wait
+            for the report to generate and for the download to succeed. This means
+            this function can actually take up to 2*max_wait_time to run.
+        
+        Returns:
+        string: The filepath to the downloaded file
+        """
+        url_tail = monitoring_links[report_code]
+        report_url = self.host + monitoring_report_base + url_tail
+        
+        return self._download_report(
+            lea,
+            report_url,
+            academic_year,
+            download_type,
+            max_wait_time,
+            report_date=report_date
+        )
+            
     def download_snapshot_report(
         self,
         lea,
         academic_year,
         submission_name,
         report_code,
         cert_status=None,
@@ -588,15 +641,14 @@
     ):
         """
         Download a CALPADS snapshot report.
         
         Known issue: The download folder needs to be empty when this function is called.
         
         Parameters:
-        Parameters:
         lea: The numerical value of the LEA on the CALPADS site. Find by inspecting the
             dropdown on the CALPADS page.
         academic_year: Integer representing the academic year that you want to check
             (per team norms, this is the year when the school year ends)
         submission_name: The name of the certification window. As of this edit, the
             certification windows are Fall1, Fall2, EOY1, EOY2, EOY3, and EOY4.
         report_code: The code for the report that you want. Should be a string in
@@ -611,58 +663,25 @@
         max_wait_time: Integer >=0 indicating the maximum number of minutes to wait
             for the report to generate and for the download to succeed. This means
             this function can actually take up to 2*max_wait_time to run.
         
         Returns:
         string: The filepath to the downloaded file
         """
-        
-        self._select_lea(lea)
-        
         url_tail = snapshot_links[submission_name][report_code]
-        snapshot_report_url = self.host + snapshot_report_base + url_tail
-        
-        self.driver.get(snapshot_report_url)
-        try:
-            # The Reports module is in an iframe
-            iframe = WebDriverWait(self.driver, 30).until(
-                EC.presence_of_element_located((
-                    By.XPATH,
-                    '//*[@id="reports"]/div/div/div/iframe'
-                ))
-            )
-        except TimeoutException:
-            logging.info("Failed to load report page.")
-            raise
-        
-        self.driver.switch_to.frame(iframe)
-        
-        academic_year_string = f"{academic_year-1}-{academic_year}"
-        yr = Select(self.driver.find_element(
-            By.XPATH,
-            '//*[@id="ReportViewer1_ctl08_ctl03_ddValue"]'
-        ))
-        yr.select_by_visible_text(academic_year_string)
-        self._wait_for_view_report_clickable()
-        
-        cert_status_select = Select(self.driver.find_element(
-            By.XPATH,
-            '//*[@id="ReportViewer1_ctl08_ctl07_ddValue"]'
-        ))            
-        if cert_status is None:
-            cert_status_select.select_by_value("1")
-        else:
-            cert_status.select_by_visible_text(cert_status)
-        
-        submit_button = self._wait_for_view_report_clickable()
-        submit_button.click()
+        report_url = self.host + snapshot_report_base + url_tail
         
-        self._wait_for_view_report_clickable(max_wait_time)
-        filepath = self._download_loaded_report(download_type, max_wait_time)
-        return filepath
+        return self._download_report(
+            lea,
+            report_url,
+            academic_year,
+            download_type,
+            max_wait_time,
+            cert_status=cert_status
+        )
             
     def _login_to_calpads(self, username, password):
         self.driver.get(self.host)
         try:
             WebDriverWait(self.driver, 15).until(EC.presence_of_element_located((
                 By.XPATH,
                 '/html/body/div[3]/div/form/div/div[2]/fieldset/div[4]/div/button'
@@ -720,14 +739,103 @@
         lea: The numerical value of the LEA on the CALPADS site. Find by inspecting the
             dropdown on the CALPADS page.
         """
         select = Select(self.driver.find_element(By.ID, 'org-select'))
         select.select_by_value(lea)
         WebDriverWait(self.driver, 30).until(EC.element_to_be_clickable((By.ID, 'org-select')))
 
+    def _download_report(
+        self,
+        lea,
+        url,
+        academic_year,
+        download_type,
+        max_wait_time,
+        **kwargs
+    ):
+        """
+        Helper function for downloading from the reports iframe
+        Will crash if you pass "cert_status" in kwargs but the report is not a Snapshot
+            report
+        Will also crash if you pass a value othere than None for "report_date" in kwargs
+            but the report is not an Accountability/Monitoring report
+        """
+        
+        self._select_lea(lea)
+        self.driver.get(url)
+        try:
+            # The Reports module is in an iframe
+            iframe = WebDriverWait(self.driver, 30).until(
+                EC.presence_of_element_located((
+                    By.XPATH,
+                    '//*[@id="reports"]/div/div/div/iframe'
+                ))
+            )
+        except TimeoutException:
+            logging.info("Failed to load report page.")
+            raise
+        
+        self.driver.switch_to.frame(iframe)
+        self._select_report_academic_year(academic_year)
+        
+        if "cert_status" in kwargs:
+            cert_status = kwargs["cert_status"]
+            cert_status_select = Select(self.driver.find_element(
+                By.XPATH,
+                '//*[@id="ReportViewer1_ctl08_ctl07_ddValue"]'
+            ))
+            if cert_status is None:
+                cert_status_select.select_by_value("1")
+            else:
+                cert_status.select_by_visible_text(cert_status)
+        
+        elif "report_date" in kwargs:
+            report_date = kwargs["report_date"]
+            if report_date is None:
+                pass
+            else:
+                # You need the month and day as strings without leading zeroes
+                month = str(int(report_date[5:7]))
+                day = str(int(report_date[8:10]))
+                
+                month_select = Select(self.driver.find_element(
+                    By.XPATH,
+                    '//*[@id="ReportViewer1_ctl08_ctl05_ddValue"]'
+                ))
+                month_select.select_by_value(month)
+                self._wait_for_view_report_clickable()
+                
+                day_select = Select(self.driver.find_element(
+                    By.XPATH,
+                    '//*[@id="ReportViewer1_ctl08_ctl07_ddValue"]'
+                ))
+                day_select.select_by_value(day)
+                
+        submit_button = self._wait_for_view_report_clickable()
+        submit_button.click()
+        
+        self._wait_for_view_report_clickable(max_wait_time)
+        filepath = self._download_loaded_report(download_type, max_wait_time)
+        return filepath
+        
+    def _select_report_academic_year(self, academic_year):
+        """
+        Select the given academic_year for the the reports module. Assumes the driver
+        is already clicked into the iframe. This function waits for the "View Report"
+        button to be clickable before returning.
+        """
+        academic_year_string = f"{academic_year-1}-{academic_year}"
+        yr = Select(self.driver.find_element(
+            By.XPATH,
+            '//*[@id="ReportViewer1_ctl08_ctl03_ddValue"]'
+        ))
+        yr.select_by_visible_text(academic_year_string)
+        self._wait_for_view_report_clickable()
+        
+        
     def _wait_for_view_report_clickable(self, max_attempts=3):
         """
         Check for the delay before webpage allows another change in value
         for the report request
         """
         try:
             max_attempts = int(max_attempts)
```

### Comparing `spswarehouse-0.2.0/spswarehouse/calpads/calpads_config.py` & `spswarehouse-0.3.0/spswarehouse/calpads/calpads_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,16 @@
-snapshot_report_base = "/Report/Snapshot/"
+monitoring_report_base = "/Report/Accountability/"
+monitoring_links = {
+    "15.1": "15_1_-_Cohort_Outcome_-_Counts_and_Rates",
+    "15.2": "15_2_-_Cohort_Outcome_-_Student_Details",
+    "16.7": "16_7_-_Students_with_Disabilities_-_Monitoring_Counts_ODS",
+    "16.8": "16_8_-_Students_with_Disabilities_-_Monitoring_Student_List_ODS",
+}
 
+snapshot_report_base = "/Report/Snapshot/"
 snapshot_links = {
     "Fall1": {
         "1.1": "1_1_EnrollmentPrimaryStatusbySubgroup",
         "1.2": "1_2_EnrollmentPrimaryStatusStudentList",
         "1.3": "1_3_EnrollmentPrimaryStatusDisaggregated",
         "1.4": "1_5_EnrollmentByStatusDisaggregated",
         "1.5": "1_5_EnrollmentByStatusDisaggregated",
```

### Comparing `spswarehouse-0.2.0/spswarehouse/credentials.py.template` & `spswarehouse-0.3.0/spswarehouse/credentials.py.template`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.2.0/spswarehouse/googledrive.py` & `spswarehouse-0.3.0/spswarehouse/googledrive.py`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.2.0/spswarehouse/googlesheets.py` & `spswarehouse-0.3.0/spswarehouse/googlesheets.py`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.2.0/spswarehouse/googleslides.py` & `spswarehouse-0.3.0/spswarehouse/googleslides.py`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.2.0/spswarehouse/powerschool/powerschool.py` & `spswarehouse-0.3.0/spswarehouse/powerschool/powerschool.py`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.2.0/spswarehouse/powerschool/powerschool_calpads.py` & `spswarehouse-0.3.0/spswarehouse/powerschool/powerschool_calpads.py`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.2.0/spswarehouse/table_names.py` & `spswarehouse-0.3.0/spswarehouse/table_names.py`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.2.0/spswarehouse/table_utils.py` & `spswarehouse-0.3.0/spswarehouse/table_utils.py`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.2.0/spswarehouse/warehouse.py` & `spswarehouse-0.3.0/spswarehouse/warehouse.py`

 * *Files identical despite different names*

### Comparing `spswarehouse-0.2.0/spswarehouse.egg-info/PKG-INFO` & `spswarehouse-0.3.0/spswarehouse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spswarehouse
-Version: 0.2.0
+Version: 0.3.0
 Summary: Summit Public Schools Snowflake warehouse
 Home-page: https://github.com/SummitPublicSchools/spswarehouse
 Author: Summit Public Schools; Harry Li Consulting, LLC
 Author-email: warehouse@summitps.org
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `spswarehouse-0.2.0/spswarehouse.egg-info/SOURCES.txt` & `spswarehouse-0.3.0/spswarehouse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

