# Comparing `tmp/openedx-filters-1.2.0.tar.gz` & `tmp/openedx-filters-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openedx-filters-1.2.0.tar", last modified: Wed Mar  1 14:47:50 2023, max compression
+gzip compressed data, was "openedx-filters-1.3.0.tar", last modified: Thu May 25 17:56:40 2023, max compression
```

## Comparing `openedx-filters-1.2.0.tar` & `openedx-filters-1.3.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-01 14:47:50.741954 openedx-filters-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (122)     3489 2023-03-01 14:47:47.000000 openedx-filters-1.2.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-03-01 14:47:47.000000 openedx-filters-1.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-03-01 14:47:47.000000 openedx-filters-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     9565 2023-03-01 14:47:50.741954 openedx-filters-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5391 2023-03-01 14:47:47.000000 openedx-filters-1.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-01 14:47:50.737954 openedx-filters-1.2.0/openedx_filters/
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-03-01 14:47:47.000000 openedx-filters-1.2.0/openedx_filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1083 2023-03-01 14:47:47.000000 openedx-filters-1.2.0/openedx_filters/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2765 2023-03-01 14:47:47.000000 openedx-filters-1.2.0/openedx_filters/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-01 14:47:50.741954 openedx-filters-1.2.0/openedx_filters/learning/
--rw-r--r--   0 runner    (1001) docker     (122)      168 2023-03-01 14:47:47.000000 openedx-filters-1.2.0/openedx_filters/learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    20092 2023-03-01 14:47:47.000000 openedx-filters-1.2.0/openedx_filters/learning/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-01 14:47:50.741954 openedx-filters-1.2.0/openedx_filters/learning/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       75 2023-03-01 14:47:47.000000 openedx-filters-1.2.0/openedx_filters/learning/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    17716 2023-03-01 14:47:47.000000 openedx-filters-1.2.0/openedx_filters/learning/tests/test_filters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-01 14:47:50.741954 openedx-filters-1.2.0/openedx_filters/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       78 2023-03-01 14:47:47.000000 openedx-filters-1.2.0/openedx_filters/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      746 2023-03-01 14:47:47.000000 openedx-filters-1.2.0/openedx_filters/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)      942 2023-03-01 14:47:47.000000 openedx-filters-1.2.0/openedx_filters/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (122)    17309 2023-03-01 14:47:47.000000 openedx-filters-1.2.0/openedx_filters/tests/test_tooling.py
--rw-r--r--   0 runner    (1001) docker     (122)     8532 2023-03-01 14:47:47.000000 openedx-filters-1.2.0/openedx_filters/tooling.py
--rw-r--r--   0 runner    (1001) docker     (122)     1022 2023-03-01 14:47:47.000000 openedx-filters-1.2.0/openedx_filters/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-01 14:47:50.737954 openedx-filters-1.2.0/openedx_filters.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     9565 2023-03-01 14:47:50.000000 openedx-filters-1.2.0/openedx_filters.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      801 2023-03-01 14:47:50.000000 openedx-filters-1.2.0/openedx_filters.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-01 14:47:50.000000 openedx-filters-1.2.0/openedx_filters.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-01 14:47:50.000000 openedx-filters-1.2.0/openedx_filters.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-03-01 14:47:50.000000 openedx-filters-1.2.0/openedx_filters.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-03-01 14:47:50.000000 openedx-filters-1.2.0/openedx_filters.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-01 14:47:50.741954 openedx-filters-1.2.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)       75 2023-03-01 14:47:47.000000 openedx-filters-1.2.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      268 2023-03-01 14:47:50.741954 openedx-filters-1.2.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     2867 2023-03-01 14:47:47.000000 openedx-filters-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-01 14:47:50.741954 openedx-filters-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      180 2023-03-01 14:47:47.000000 openedx-filters-1.2.0/tests/test_openedx_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 17:56:40.085341 openedx-filters-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     3669 2023-05-25 17:56:34.000000 openedx-filters-1.3.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-05-25 17:56:34.000000 openedx-filters-1.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-05-25 17:56:34.000000 openedx-filters-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     9745 2023-05-25 17:56:40.085341 openedx-filters-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5391 2023-05-25 17:56:34.000000 openedx-filters-1.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 17:56:40.085341 openedx-filters-1.3.0/openedx_filters/
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-05-25 17:56:34.000000 openedx-filters-1.3.0/openedx_filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1083 2023-05-25 17:56:34.000000 openedx-filters-1.3.0/openedx_filters/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2765 2023-05-25 17:56:34.000000 openedx-filters-1.3.0/openedx_filters/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 17:56:40.085341 openedx-filters-1.3.0/openedx_filters/learning/
+-rw-r--r--   0 runner    (1001) docker     (122)      168 2023-05-25 17:56:34.000000 openedx-filters-1.3.0/openedx_filters/learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20822 2023-05-25 17:56:34.000000 openedx-filters-1.3.0/openedx_filters/learning/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 17:56:40.085341 openedx-filters-1.3.0/openedx_filters/learning/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2023-05-25 17:56:34.000000 openedx-filters-1.3.0/openedx_filters/learning/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18503 2023-05-25 17:56:34.000000 openedx-filters-1.3.0/openedx_filters/learning/tests/test_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 17:56:40.085341 openedx-filters-1.3.0/openedx_filters/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-05-25 17:56:34.000000 openedx-filters-1.3.0/openedx_filters/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      746 2023-05-25 17:56:34.000000 openedx-filters-1.3.0/openedx_filters/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      942 2023-05-25 17:56:34.000000 openedx-filters-1.3.0/openedx_filters/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17309 2023-05-25 17:56:34.000000 openedx-filters-1.3.0/openedx_filters/tests/test_tooling.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8532 2023-05-25 17:56:34.000000 openedx-filters-1.3.0/openedx_filters/tooling.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1022 2023-05-25 17:56:34.000000 openedx-filters-1.3.0/openedx_filters/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 17:56:40.085341 openedx-filters-1.3.0/openedx_filters.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     9745 2023-05-25 17:56:40.000000 openedx-filters-1.3.0/openedx_filters.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      801 2023-05-25 17:56:40.000000 openedx-filters-1.3.0/openedx_filters.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-25 17:56:40.000000 openedx-filters-1.3.0/openedx_filters.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-25 17:56:40.000000 openedx-filters-1.3.0/openedx_filters.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-05-25 17:56:40.000000 openedx-filters-1.3.0/openedx_filters.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-05-25 17:56:40.000000 openedx-filters-1.3.0/openedx_filters.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 17:56:40.085341 openedx-filters-1.3.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2023-05-25 17:56:34.000000 openedx-filters-1.3.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      268 2023-05-25 17:56:40.085341 openedx-filters-1.3.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2867 2023-05-25 17:56:34.000000 openedx-filters-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 17:56:40.085341 openedx-filters-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      180 2023-05-25 17:56:34.000000 openedx-filters-1.3.0/tests/test_openedx_filters.py
```

### Comparing `openedx-filters-1.2.0/CHANGELOG.rst` & `openedx-filters-1.3.0/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,22 @@
 
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
+[1.3.0] - 2023-05-25
+--------------------
+
+Added
+~~~~~
+
+* CourseHomeUrlCreationStarted filter added which can be used to modify the course_home_url for externally hosted courses.
+
 [1.2.0] - 2023-03-01
 --------------------
 
 Added
 ~~~~~
 
 * AccountSettingsRenderStarted filter added which can be used to modify the rendered output of the account settings page.
```

### Comparing `openedx-filters-1.2.0/LICENSE.txt` & `openedx-filters-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openedx-filters-1.2.0/PKG-INFO` & `openedx-filters-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx-filters
-Version: 1.2.0
+Version: 1.3.0
 Summary: Open edX Filters from Hooks Extensions Framework (OEP-50).
 Home-page: https://github.com/openedx/openedx-filters
 Author: eduNEXT
 Author-email: technical@edunext.co
 License: AGPL 3.0
 Keywords: Python openedx
 Classifier: Development Status :: 3 - Alpha
@@ -209,14 +209,22 @@
 
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
+[1.3.0] - 2023-05-25
+--------------------
+
+Added
+~~~~~
+
+* CourseHomeUrlCreationStarted filter added which can be used to modify the course_home_url for externally hosted courses.
+
 [1.2.0] - 2023-03-01
 --------------------
 
 Added
 ~~~~~
 
 * AccountSettingsRenderStarted filter added which can be used to modify the rendered output of the account settings page.
```

### Comparing `openedx-filters-1.2.0/README.rst` & `openedx-filters-1.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `openedx-filters-1.2.0/openedx_filters/exceptions.py` & `openedx-filters-1.3.0/openedx_filters/exceptions.py`

 * *Files identical despite different names*

### Comparing `openedx-filters-1.2.0/openedx_filters/filters.py` & `openedx-filters-1.3.0/openedx_filters/filters.py`

 * *Files identical despite different names*

### Comparing `openedx-filters-1.2.0/openedx_filters/learning/filters.py` & `openedx-filters-1.3.0/openedx_filters/learning/filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -565,7 +565,27 @@
             block (VerticalBlock): The VeriticalBlock instance which is being rendered
             fragment (web_fragments.Fragment): The web-fragment containing the rendered content of VerticalBlock
             context (dict): rendering context values like is_mobile_app, show_title..etc.,
             view (str): the rendering view. Can be either 'student_view', or 'public_view'
         """
         data = super().run_pipeline(block=block, fragment=fragment, context=context, view=view)
         return data.get("block"), data.get("fragment"), data.get("context"), data.get("view")
+
+
+class CourseHomeUrlCreationStarted(OpenEdxPublicFilter):
+    """
+    Custom class used to create filters to act on course home url creation.
+    """
+
+    filter_type = "org.openedx.learning.course.homepage.url.creation.started.v1"
+
+    @classmethod
+    def run_filter(cls, course_key, course_home_url):
+        """
+        Execute a filter with the specified signature.
+
+        Arguments:
+            course_key (CourseKey): The course key for which the home url is being requested.
+            course_home_url (String): The url string for the course home
+        """
+        data = super().run_pipeline(course_key=course_key, course_home_url=course_home_url)
+        return data.get("course_key"), data.get("course_home_url")
```

### Comparing `openedx-filters-1.2.0/openedx_filters/learning/tests/test_filters.py` & `openedx-filters-1.3.0/openedx_filters/learning/tests/test_filters.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     CertificateCreationRequested,
     CertificateRenderStarted,
     CohortAssignmentRequested,
     CohortChangeRequested,
     CourseAboutRenderStarted,
     CourseEnrollmentQuerysetRequested,
     CourseEnrollmentStarted,
+    CourseHomeUrlCreationStarted,
     CourseUnenrollmentStarted,
     DashboardRenderStarted,
     StudentLoginRequested,
     StudentRegistrationRequested,
     VerticalBlockChildRenderStarted,
     VerticalBlockRenderCompleted,
 )
@@ -540,7 +541,30 @@
             - The filter should return user and target_cohort in that order.
         """
         user, target_cohort = Mock(), Mock()
 
         result = CohortAssignmentRequested.run_filter(user, target_cohort)
 
         self.assertTupleEqual((user, target_cohort,), result)
+
+
+class TestFederatedContentFilters(TestCase):
+    """
+    Test class to verify standard behavior of the federated content filters.
+    You'll find test suites for:
+
+    - CourseHomeUrlCreationStarted
+    """
+
+    def test_course_homeurl_creation_started(self):
+        """
+        Test CourseHomeUrlCreationStarted filter behavior under normal conditions.
+
+        Expected behavior:
+            - The filter must have the signature specified.
+            - The filter should return course_key and course_home_url in that order.
+        """
+        course_key, course_home_url = Mock(), Mock()
+
+        result = CourseHomeUrlCreationStarted.run_filter(course_key, course_home_url)
+
+        self.assertTupleEqual((course_key, course_home_url,), result)
```

### Comparing `openedx-filters-1.2.0/openedx_filters/tests/test_exceptions.py` & `openedx-filters-1.3.0/openedx_filters/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `openedx-filters-1.2.0/openedx_filters/tests/test_filters.py` & `openedx-filters-1.3.0/openedx_filters/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `openedx-filters-1.2.0/openedx_filters/tests/test_tooling.py` & `openedx-filters-1.3.0/openedx_filters/tests/test_tooling.py`

 * *Files identical despite different names*

### Comparing `openedx-filters-1.2.0/openedx_filters/tooling.py` & `openedx-filters-1.3.0/openedx_filters/tooling.py`

 * *Files identical despite different names*

### Comparing `openedx-filters-1.2.0/openedx_filters/utils.py` & `openedx-filters-1.3.0/openedx_filters/utils.py`

 * *Files identical despite different names*

### Comparing `openedx-filters-1.2.0/openedx_filters.egg-info/PKG-INFO` & `openedx-filters-1.3.0/openedx_filters.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx-filters
-Version: 1.2.0
+Version: 1.3.0
 Summary: Open edX Filters from Hooks Extensions Framework (OEP-50).
 Home-page: https://github.com/openedx/openedx-filters
 Author: eduNEXT
 Author-email: technical@edunext.co
 License: AGPL 3.0
 Keywords: Python openedx
 Classifier: Development Status :: 3 - Alpha
@@ -209,14 +209,22 @@
 
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
+[1.3.0] - 2023-05-25
+--------------------
+
+Added
+~~~~~
+
+* CourseHomeUrlCreationStarted filter added which can be used to modify the course_home_url for externally hosted courses.
+
 [1.2.0] - 2023-03-01
 --------------------
 
 Added
 ~~~~~
 
 * AccountSettingsRenderStarted filter added which can be used to modify the rendered output of the account settings page.
```

### Comparing `openedx-filters-1.2.0/openedx_filters.egg-info/SOURCES.txt` & `openedx-filters-1.3.0/openedx_filters.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openedx-filters-1.2.0/setup.py` & `openedx-filters-1.3.0/setup.py`

 * *Files identical despite different names*

