# Comparing `tmp/edx-submissions-3.5.4.tar.gz` & `tmp/edx-submissions-3.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-submissions-3.5.4.tar", last modified: Thu Aug 18 21:15:24 2022, max compression
+gzip compressed data, was "edx-submissions-3.5.5.tar", last modified: Thu May 25 19:18:36 2023, max compression
```

## Comparing `edx-submissions-3.5.4.tar` & `edx-submissions-3.5.5.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 21:15:24.253561 edx-submissions-3.5.4/
--rw-r--r--   0 runner    (1001) docker     (121)    35136 2022-08-18 21:15:19.000000 edx-submissions-3.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      122 2022-08-18 21:15:19.000000 edx-submissions-3.5.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      746 2022-08-18 21:15:24.253561 edx-submissions-3.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1958 2022-08-18 21:15:19.000000 edx-submissions-3.5.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 21:15:24.253561 edx-submissions-3.5.4/edx_submissions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      746 2022-08-18 21:15:24.000000 edx-submissions-3.5.4/edx_submissions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1125 2022-08-18 21:15:24.000000 edx-submissions-3.5.4/edx_submissions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-18 21:15:24.000000 edx-submissions-3.5.4/edx_submissions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-08-18 21:15:24.000000 edx-submissions-3.5.4/edx_submissions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-08-18 21:15:24.000000 edx-submissions-3.5.4/edx_submissions.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 21:15:24.253561 edx-submissions-3.5.4/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)      206 2022-08-18 21:15:19.000000 edx-submissions-3.5.4/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-08-18 21:15:19.000000 edx-submissions-3.5.4/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (121)      174 2022-08-18 21:15:19.000000 edx-submissions-3.5.4/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (121)      318 2022-08-18 21:15:24.253561 edx-submissions-3.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2780 2022-08-18 21:15:19.000000 edx-submissions-3.5.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 21:15:24.253561 edx-submissions-3.5.4/submissions/
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-08-18 21:15:19.000000 edx-submissions-3.5.4/submissions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5181 2022-08-18 21:15:19.000000 edx-submissions-3.5.4/submissions/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)    39521 2022-08-18 21:15:19.000000 edx-submissions-3.5.4/submissions/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     2454 2022-08-18 21:15:19.000000 edx-submissions-3.5.4/submissions/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 21:15:24.253561 edx-submissions-3.5.4/submissions/management/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-18 21:15:19.000000 edx-submissions-3.5.4/submissions/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 21:15:24.253561 edx-submissions-3.5.4/submissions/management/commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-18 21:15:19.000000 edx-submissions-3.5.4/submissions/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6344 2022-08-18 21:15:19.000000 edx-submissions-3.5.4/submissions/management/commands/analyze_uploaded_file_sizes.py
--rw-r--r--   0 runner    (1001) docker     (121)     2828 2022-08-18 21:15:19.000000 edx-submissions-3.5.4/submissions/management/commands/update_submissions_uuids.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 21:15:24.253561 edx-submissions-3.5.4/submissions/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     3489 2022-08-18 21:15:19.000000 edx-submissions-3.5.4/submissions/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)     6745 2022-08-18 21:15:19.000000 edx-submissions-3.5.4/submissions/migrations/0001_squashed_0005_CreateTeamModel.py
--rw-r--r--   0 runner    (1001) docker     (121)      910 2022-08-18 21:15:19.000000 edx-submissions-3.5.4/submissions/migrations/0002_auto_20151119_0913.py
--rw-r--r--   0 runner    (1001) docker     (121)      658 2022-08-18 21:15:19.000000 edx-submissions-3.5.4/submissions/migrations/0002_team_submission_optional.py
--rw-r--r--   0 runner    (1001) docker     (121)      484 2022-08-18 21:15:19.000000 edx-submissions-3.5.4/submissions/migrations/0003_ensure_ascii.py
--rw-r--r--   0 runner    (1001) docker     (121)      400 2022-08-18 21:15:19.000000 edx-submissions-3.5.4/submissions/migrations/0003_submission_status.py
--rw-r--r--   0 runner    (1001) docker     (121)      375 2022-08-18 21:15:19.000000 edx-submissions-3.5.4/submissions/migrations/0004_remove_django_extensions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2379 2022-08-18 21:15:19.000000 edx-submissions-3.5.4/submissions/migrations/0005_CreateTeamModel.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-18 21:15:19.000000 edx-submissions-3.5.4/submissions/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    20261 2022-08-18 21:15:19.000000 edx-submissions-3.5.4/submissions/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     7303 2022-08-18 21:15:19.000000 edx-submissions-3.5.4/submissions/serializers.py
--rw-r--r--   0 runner    (1001) docker     (121)    18595 2022-08-18 21:15:19.000000 edx-submissions-3.5.4/submissions/team_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1468 2022-08-18 21:15:19.000000 edx-submissions-3.5.4/submissions/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:18:36.931693 edx-submissions-3.5.5/
+-rw-r--r--   0 runner    (1001) docker     (122)    35136 2023-05-25 19:18:31.000000 edx-submissions-3.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      122 2023-05-25 19:18:31.000000 edx-submissions-3.5.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      750 2023-05-25 19:18:36.931693 edx-submissions-3.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1793 2023-05-25 19:18:31.000000 edx-submissions-3.5.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:18:36.927693 edx-submissions-3.5.5/edx_submissions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      750 2023-05-25 19:18:36.000000 edx-submissions-3.5.5/edx_submissions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1125 2023-05-25 19:18:36.000000 edx-submissions-3.5.5/edx_submissions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-25 19:18:36.000000 edx-submissions-3.5.5/edx_submissions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2023-05-25 19:18:36.000000 edx-submissions-3.5.5/edx_submissions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-25 19:18:36.000000 edx-submissions-3.5.5/edx_submissions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:18:36.927693 edx-submissions-3.5.5/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      206 2023-05-25 19:18:31.000000 edx-submissions-3.5.5/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)       91 2023-05-25 19:18:31.000000 edx-submissions-3.5.5/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-05-25 19:18:31.000000 edx-submissions-3.5.5/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (122)      318 2023-05-25 19:18:36.931693 edx-submissions-3.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2784 2023-05-25 19:18:31.000000 edx-submissions-3.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:18:36.927693 edx-submissions-3.5.5/submissions/
+-rw-r--r--   0 runner    (1001) docker     (122)       71 2023-05-25 19:18:31.000000 edx-submissions-3.5.5/submissions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5181 2023-05-25 19:18:31.000000 edx-submissions-3.5.5/submissions/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39479 2023-05-25 19:18:31.000000 edx-submissions-3.5.5/submissions/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2454 2023-05-25 19:18:31.000000 edx-submissions-3.5.5/submissions/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:18:36.927693 edx-submissions-3.5.5/submissions/management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 19:18:31.000000 edx-submissions-3.5.5/submissions/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:18:36.931693 edx-submissions-3.5.5/submissions/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 19:18:31.000000 edx-submissions-3.5.5/submissions/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6344 2023-05-25 19:18:31.000000 edx-submissions-3.5.5/submissions/management/commands/analyze_uploaded_file_sizes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2828 2023-05-25 19:18:31.000000 edx-submissions-3.5.5/submissions/management/commands/update_submissions_uuids.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:18:36.931693 edx-submissions-3.5.5/submissions/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     3489 2023-05-25 19:18:31.000000 edx-submissions-3.5.5/submissions/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6745 2023-05-25 19:18:31.000000 edx-submissions-3.5.5/submissions/migrations/0001_squashed_0005_CreateTeamModel.py
+-rw-r--r--   0 runner    (1001) docker     (122)      910 2023-05-25 19:18:31.000000 edx-submissions-3.5.5/submissions/migrations/0002_auto_20151119_0913.py
+-rw-r--r--   0 runner    (1001) docker     (122)      658 2023-05-25 19:18:31.000000 edx-submissions-3.5.5/submissions/migrations/0002_team_submission_optional.py
+-rw-r--r--   0 runner    (1001) docker     (122)      484 2023-05-25 19:18:31.000000 edx-submissions-3.5.5/submissions/migrations/0003_ensure_ascii.py
+-rw-r--r--   0 runner    (1001) docker     (122)      400 2023-05-25 19:18:31.000000 edx-submissions-3.5.5/submissions/migrations/0003_submission_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)      375 2023-05-25 19:18:31.000000 edx-submissions-3.5.5/submissions/migrations/0004_remove_django_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2379 2023-05-25 19:18:31.000000 edx-submissions-3.5.5/submissions/migrations/0005_CreateTeamModel.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 19:18:31.000000 edx-submissions-3.5.5/submissions/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20313 2023-05-25 19:18:31.000000 edx-submissions-3.5.5/submissions/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7303 2023-05-25 19:18:31.000000 edx-submissions-3.5.5/submissions/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18543 2023-05-25 19:18:31.000000 edx-submissions-3.5.5/submissions/team_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1469 2023-05-25 19:18:31.000000 edx-submissions-3.5.5/submissions/views.py
```

### Comparing `edx-submissions-3.5.4/LICENSE` & `edx-submissions-3.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.5.4/PKG-INFO` & `edx-submissions-3.5.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: edx-submissions
-Version: 3.5.4
+Version: 3.5.5
 Summary: An API for creating submissions and scores.
-Home-page: http://github.com/edx/edx-submissions.git
+Home-page: http://github.com/openedx/edx-submissions.git
 Author: edX
 License: AGPL
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
```

### Comparing `edx-submissions-3.5.4/README.rst` & `edx-submissions-3.5.5/README.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,9 @@
-Part of `edX code`__.
-
-__ http://code.edx.org/
-
-.. image:: https://github.com/edx/edx-submissions/workflows/Python%20CI/badge.svg?branch=master
-    :target: https://github.com/edx/edx-submissions/actions?query=workflow%3A%22Python+CI%22
+.. image:: https://github.com/openedx/edx-submissions/workflows/Python%20CI/badge.svg?branch=master
+    :target: https://github.com/openedx/edx-submissions/actions?query=workflow%3A%22Python+CI%22
     :alt: Build status
 
 .. image:: https://coveralls.io/repos/edx/edx-submissions/badge.png?branch=master
     :target: https://coveralls.io/r/edx/edx-submissions?branch=master
     :alt: Coverage badge
 
 
@@ -61,18 +57,15 @@
 
 
 How To Contribute
 -----------------
 
 Contributions are very welcome.
 
-Please read `How To Contribute <https://github.com/edx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details.
-
-Even though it was written with ``edx-platform`` in mind, the guidelines
-should be followed for Open edX code in general.
+Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
 
 Reporting Security Issues
 -------------------------
 
 Please do not report security issues in public. Please email security@edx.org
```

### Comparing `edx-submissions-3.5.4/edx_submissions.egg-info/PKG-INFO` & `edx-submissions-3.5.5/edx_submissions.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: edx-submissions
-Version: 3.5.4
+Version: 3.5.5
 Summary: An API for creating submissions and scores.
-Home-page: http://github.com/edx/edx-submissions.git
+Home-page: http://github.com/openedx/edx-submissions.git
 Author: edX
 License: AGPL
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
```

### Comparing `edx-submissions-3.5.4/edx_submissions.egg-info/SOURCES.txt` & `edx-submissions-3.5.5/edx_submissions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.5.4/setup.py` & `edx-submissions-3.5.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
 setup(
     name='edx-submissions',
     version=VERSION,
     author='edX',
     description='An API for creating submissions and scores.',
     long_description="An API for creating and scoring submissions for the Open edX platform",
-    url='http://github.com/edx/edx-submissions.git',
+    url='http://github.com/openedx/edx-submissions.git',
     license='AGPL',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Framework :: Django',
         'Framework :: Django :: 3.2',
         'Framework :: Django :: 4.0',
         'Intended Audience :: Developers',
```

### Comparing `edx-submissions-3.5.4/submissions/admin.py` & `edx-submissions-3.5.5/submissions/admin.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.5.4/submissions/api.py` & `edx-submissions-3.5.5/submissions/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -790,23 +790,22 @@
     except DatabaseError as error:
         msg = (
             "Error occurred while reseting scores for"
             f" item {item_id} in course {course_id} for student {student_id}"
         )
         logger.exception(msg)
         raise SubmissionInternalError(msg) from error
-    else:
-        logger.info(
-            "Score reset for item %(item_id)s in course %(course_id)s for student %(student_id)s",
-            {
-                'item_id': item_id,
-                'course_id': course_id,
-                'student_id': student_id,
-            }
-        )
+    logger.info(
+        "Score reset for item %(item_id)s in course %(course_id)s for student %(student_id)s",
+        {
+            'item_id': item_id,
+            'course_id': course_id,
+            'student_id': student_id,
+        }
+    )
 
 
 def set_score(submission_uuid, points_earned, points_possible,
               annotation_creator=None, annotation_type=None, annotation_reason=None):
     """Set a score for a particular submission.
 
     Sets the score for a particular submission. This score is calculated
```

### Comparing `edx-submissions-3.5.4/submissions/errors.py` & `edx-submissions-3.5.5/submissions/errors.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.5.4/submissions/management/commands/analyze_uploaded_file_sizes.py` & `edx-submissions-3.5.5/submissions/management/commands/analyze_uploaded_file_sizes.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.5.4/submissions/management/commands/update_submissions_uuids.py` & `edx-submissions-3.5.5/submissions/management/commands/update_submissions_uuids.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.5.4/submissions/migrations/0001_initial.py` & `edx-submissions-3.5.5/submissions/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.5.4/submissions/migrations/0001_squashed_0005_CreateTeamModel.py` & `edx-submissions-3.5.5/submissions/migrations/0001_squashed_0005_CreateTeamModel.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.5.4/submissions/migrations/0002_auto_20151119_0913.py` & `edx-submissions-3.5.5/submissions/migrations/0002_auto_20151119_0913.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.5.4/submissions/migrations/0002_team_submission_optional.py` & `edx-submissions-3.5.5/submissions/migrations/0002_team_submission_optional.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.5.4/submissions/migrations/0005_CreateTeamModel.py` & `edx-submissions-3.5.5/submissions/migrations/0005_CreateTeamModel.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.5.4/submissions/models.py` & `edx-submissions-3.5.5/submissions/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -70,20 +70,20 @@
     item_type = models.CharField(max_length=100)
 
     def __repr__(self):
         return repr(self.student_item_dict)
 
     @property
     def student_item_dict(self):
-        return dict(
-            student_id=self.student_id,
-            course_id=self.course_id,
-            item_id=self.item_id,
-            item_type=self.item_type,
-        )
+        return {
+            "student_id": self.student_id,
+            "course_id": self.course_id,
+            "item_id": self.item_id,
+            "item_type": self.item_type,
+        }
 
     def __str__(self):
         return (
             f"({self.student_id}, {self.course_id}, "
             f"{self.item_type}, {self.item_id})"
         )
 
@@ -175,15 +175,15 @@
         Given a course_id, item_id, and team_id, return team submission for the team assignment
 
         Raises:
             - TeamSubmissionNotFoundError if there is no matching team submission
             - TeamSubmissionInternalError if there is some other error looking up the team submission.
 
         """
-        model_query_params = dict(course_id=course_id, item_id=item_id, team_id=team_id)
+        model_query_params = {"course_id": course_id, "item_id": item_id, "team_id": team_id}
         query_params_string = "course_id={course_id} item_id={item_id} team_id={team_id}".format(**model_query_params)
         try:
             # In the equivalent non-teams api call, we're filtering on student item and then getting first(),
             # which will get us the most recent active submission due to the sort order of the model.
             # However, for this model, we have a uniqueness constraint (non-db, as a signal handler)
             # that means we can only ever have one submission per team per assignment. I don't fully understand
             # the logic behind the non-teams api, but this shouldn't have to do that filter.
@@ -250,22 +250,22 @@
                 f"Attempt to get team submissions for {query_params_string} "
                 f"caused error: {exc}"
             )
             logger.error(err_msg)
             raise TeamSubmissionInternalError(err_msg) from exc
 
     def __repr__(self):
-        return repr(dict(
-            uuid=self.uuid,
-            submitted_by=self.submitted_by,
-            attempt_number=self.attempt_number,
-            submitted_at=self.submitted_at,
-            created=self.created,
-            modified=self.modified,
-        ))
+        return repr({
+            "uuid": self.uuid,
+            "submitted_by": self.submitted_by,
+            "attempt_number": self.attempt_number,
+            "submitted_at": self.submitted_at,
+            "created": self.created,
+            "modified": self.modified,
+        })
 
     def __str__(self):
         return f"Team Submission {self.uuid}"
 
     class Meta:
         app_label = "submissions"
         ordering = ["-submitted_at", "-id"]
@@ -341,22 +341,22 @@
     _objects = models.Manager()  # Don't use this unless you know and can explain why objects doesn't work for you
 
     @staticmethod
     def get_cache_key(sub_uuid):
         return f"submissions.submission.{sub_uuid}"
 
     def __repr__(self):
-        return repr(dict(
-            uuid=self.uuid,
-            student_item=self.student_item,
-            attempt_number=self.attempt_number,
-            submitted_at=self.submitted_at,
-            created_at=self.created_at,
-            answer=self.answer,
-        ))
+        return repr({
+            "uuid": self.uuid,
+            "student_item": self.student_item,
+            "attempt_number": self.attempt_number,
+            "submitted_at": self.submitted_at,
+            "created_at": self.created_at,
+            "answer": self.answer,
+        })
 
     def __str__(self):
         return f"Submission {self.uuid}"
 
     class Meta:
         app_label = "submissions"
         ordering = ["-submitted_at", "-id"]
@@ -410,21 +410,21 @@
 
         """
         if self.points_possible == 0:
             return None
         return float(self.points_earned) / self.points_possible
 
     def __repr__(self):
-        return repr(dict(
-            student_item=self.student_item,
-            submission=self.submission,
-            created_at=self.created_at,
-            points_earned=self.points_earned,
-            points_possible=self.points_possible,
-        ))
+        return repr({
+            "student_item": self.student_item,
+            "submission": self.submission,
+            "created_at": self.created_at,
+            "points_earned": self.points_earned,
+            "points_possible": self.points_possible,
+        })
 
     def is_hidden(self):
         """
         By convention, a score of 0/0 is not displayed to users.
         Hidden scores are filtered by the submissions API.
 
         Returns:
```

### Comparing `edx-submissions-3.5.4/submissions/serializers.py` & `edx-submissions-3.5.5/submissions/serializers.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.5.4/submissions/team_api.py` & `edx-submissions-3.5.5/submissions/team_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,16 +175,15 @@
             logger.error(
                 "[%s] Unable to create individual submission for %s: %s",
                 log_string,
                 team_member_id,
                 str(exc)
             )
             raise exc
-        else:
-            logger.info("[%s] Created individual submission %s", log_string, individual_submission['uuid'])
+        logger.info("[%s] Created individual submission %s", log_string, individual_submission['uuid'])
 
     model_kwargs = {
         "answer": answer,
     }
     # We must serialize the model, since the existing serializer doesn't have info about the individual submissions
     model_serializer = TeamSubmissionSerializer(team_submission, context={"answer": answer})
     return model_serializer.data
@@ -447,14 +446,13 @@
             team_submission.save(update_fields=["status"])
     except (DatabaseError, SubmissionInternalError) as error:
         msg = (
             f"Error occurred while reseting scores for team submission {team_submission_uuid}"
         )
         logger.exception(msg)
         raise TeamSubmissionInternalError(msg) from error
-    else:
-        logger.info(
-            "Score reset for team submission %(team_submission_uuid)s",
-            {
-                'team_submission_uuid': team_submission_uuid,
-            }
-        )
+    logger.info(
+        "Score reset for team submission %(team_submission_uuid)s",
+        {
+            'team_submission_uuid': team_submission_uuid,
+        }
+    )
```

### Comparing `edx-submissions-3.5.4/submissions/views.py` & `edx-submissions-3.5.5/submissions/views.py`

 * *Files 15% similar despite different names*

```diff
@@ -26,20 +26,20 @@
 
     Returns:
         HttpResponse: The response object for this request. Renders a simple
             development page with all the submissions related to the specified
             student item.
 
     """
-    student_item_dict = dict(
-        course_id=course_id,
-        student_id=student_id,
-        item_id=item_id,
-    )
-    context = dict(**student_item_dict)
+    student_item_dict = {
+        "course_id": course_id,
+        "student_id": student_id,
+        "item_id": item_id,
+    }
+    context = {**student_item_dict}
     try:
         submissions = get_submissions(student_item_dict)
         context["submissions"] = submissions
     except SubmissionRequestError:
         context["error"] = "The specified student item was not found."
 
     return render(request, 'submissions.html', context)
```

