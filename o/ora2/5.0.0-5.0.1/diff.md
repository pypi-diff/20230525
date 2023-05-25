# Comparing `tmp/ora2-5.0.0.tar.gz` & `tmp/ora2-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ora2-5.0.0.tar", last modified: Wed Feb  1 15:47:49 2023, max compression
+gzip compressed data, was "ora2-5.0.1.tar", last modified: Thu May 25 19:16:40 2023, max compression
```

## Comparing `ora2-5.0.0.tar` & `ora2-5.0.1.tar`

### file list

```diff
@@ -1,551 +1,551 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.515404 ora2-5.0.0/
--rw-r--r--   0 runner    (1001) docker     (122)    35135 2023-02-01 15:47:43.000000 ora2-5.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      682 2023-02-01 15:47:43.000000 ora2-5.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2643 2023-02-01 15:47:49.515404 ora2-5.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2038 2023-02-01 15:47:43.000000 ora2-5.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.423403 ora2-5.0.0/openassessment/
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.423403 ora2-5.0.0/openassessment/assessment/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/assessment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5633 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/assessment/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.423403 ora2-5.0.0/openassessment/assessment/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/assessment/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    39052 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/assessment/api/peer.py
--rw-r--r--   0 runner    (1001) docker     (122)    11874 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/assessment/api/self.py
--rw-r--r--   0 runner    (1001) docker     (122)    16433 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/assessment/api/staff.py
--rw-r--r--   0 runner    (1001) docker     (122)    16864 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/assessment/api/student_training.py
--rw-r--r--   0 runner    (1001) docker     (122)    12955 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/assessment/api/teams.py
--rw-r--r--   0 runner    (1001) docker     (122)      442 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/assessment/data_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.427403 ora2-5.0.0/openassessment/assessment/errors/
--rw-r--r--   0 runner    (1001) docker     (122)      182 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/assessment/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      189 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/assessment/errors/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1117 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/assessment/errors/peer.py
--rw-r--r--   0 runner    (1001) docker     (122)      552 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/assessment/errors/self.py
--rw-r--r--   0 runner    (1001) docker     (122)      821 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/assessment/errors/staff.py
--rw-r--r--   0 runner    (1001) docker     (122)      440 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/assessment/errors/student_training.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.427403 ora2-5.0.0/openassessment/assessment/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     9361 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/assessment/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)     1333 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/assessment/migrations/0002_staffworkflow.py
--rw-r--r--   0 runner    (1001) docker     (122)      750 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/assessment/migrations/0003_expand_course_id.py
--rw-r--r--   0 runner    (1001) docker     (122)     3459 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/assessment/migrations/0004_historicalsharedfileupload_sharedfileupload.py
--rw-r--r--   0 runner    (1001) docker     (122)      618 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/assessment/migrations/0005_add_filename_to_sharedupload.py
--rw-r--r--   0 runner    (1001) docker     (122)      744 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/assessment/migrations/0006_TeamWorkflows.py
--rw-r--r--   0 runner    (1001) docker     (122)     1218 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/assessment/migrations/0007_staff_workflow_blank.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/assessment/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.427403 ora2-5.0.0/openassessment/assessment/models/
--rw-r--r--   0 runner    (1001) docker     (122)      205 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/assessment/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    32191 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/assessment/models/base.py
--rw-r--r--   0 runner    (1001) docker     (122)    22340 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/assessment/models/peer.py
--rw-r--r--   0 runner    (1001) docker     (122)     8558 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/assessment/models/staff.py
--rw-r--r--   0 runner    (1001) docker     (122)     8200 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/assessment/models/student_training.py
--rw-r--r--   0 runner    (1001) docker     (122)     4991 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/assessment/models/training.py
--rw-r--r--   0 runner    (1001) docker     (122)      163 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/assessment/score_type_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.427403 ora2-5.0.0/openassessment/assessment/serializers/
--rw-r--r--   0 runner    (1001) docker     (122)      151 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/assessment/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10553 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/assessment/serializers/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2021 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/assessment/serializers/peer.py
--rw-r--r--   0 runner    (1001) docker     (122)     6217 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/assessment/serializers/training.py
--rw-r--r--   0 runner    (1001) docker     (122)      376 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/assessment/signals.py
--rw-r--r--   0 runner    (1001) docker     (122)      265 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/assessment/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)     1873 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/assessment/views.py
--rw-r--r--   0 runner    (1001) docker     (122)    58992 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/data.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.427403 ora2-5.0.0/openassessment/fileupload/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/fileupload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    23578 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/fileupload/api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.427403 ora2-5.0.0/openassessment/fileupload/backends/
--rw-r--r--   0 runner    (1001) docker     (122)      849 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/fileupload/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5253 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/fileupload/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2411 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/fileupload/backends/django_storage.py
--rw-r--r--   0 runner    (1001) docker     (122)     4122 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/fileupload/backends/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (122)     3034 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/fileupload/backends/s3.py
--rw-r--r--   0 runner    (1001) docker     (122)     3392 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/fileupload/backends/swift.py
--rw-r--r--   0 runner    (1001) docker     (122)      740 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/fileupload/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)      412 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/fileupload/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)      498 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/fileupload/views_django_storage.py
--rw-r--r--   0 runner    (1001) docker     (122)     5105 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/fileupload/views_filesystem.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.427403 ora2-5.0.0/openassessment/locale/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.415403 ora2-5.0.0/openassessment/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.431403 ora2-5.0.0/openassessment/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    81919 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   137408 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/ar/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)    10517 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/ar/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    29332 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/ar/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.415403 ora2-5.0.0/openassessment/locale/ar_SA/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.431403 ora2-5.0.0/openassessment/locale/ar_SA/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     9218 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/ar_SA/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    28056 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/ar_SA/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.415403 ora2-5.0.0/openassessment/locale/de_DE/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.431403 ora2-5.0.0/openassessment/locale/de_DE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    64223 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/de_DE/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   124947 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/de_DE/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     8402 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/de_DE/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    27871 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/de_DE/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.415403 ora2-5.0.0/openassessment/locale/el/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.431403 ora2-5.0.0/openassessment/locale/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    35998 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/el/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   116285 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/el/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     5045 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/el/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    26850 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/el/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.415403 ora2-5.0.0/openassessment/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.431403 ora2-5.0.0/openassessment/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      382 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)    94672 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)      425 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/en/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    23724 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/en/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.415403 ora2-5.0.0/openassessment/locale/eo/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.431403 ora2-5.0.0/openassessment/locale/eo/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)   145495 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/eo/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   195906 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/eo/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)    21982 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/eo/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    38500 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/eo/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.415403 ora2-5.0.0/openassessment/locale/es_419/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.435403 ora2-5.0.0/openassessment/locale/es_419/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    81996 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/es_419/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   133250 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/es_419/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)    11545 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/es_419/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    29006 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/es_419/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.415403 ora2-5.0.0/openassessment/locale/es_AR/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.435403 ora2-5.0.0/openassessment/locale/es_AR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    11444 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/es_AR/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    28411 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/es_AR/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.415403 ora2-5.0.0/openassessment/locale/es_ES/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.435403 ora2-5.0.0/openassessment/locale/es_ES/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    82594 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/es_ES/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   133560 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/es_ES/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)    11635 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/es_ES/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    29042 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/es_ES/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.419402 ora2-5.0.0/openassessment/locale/eu_ES/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.435403 ora2-5.0.0/openassessment/locale/eu_ES/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    14552 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/eu_ES/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   100050 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/eu_ES/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     3947 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/eu_ES/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    25057 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/eu_ES/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.419402 ora2-5.0.0/openassessment/locale/fa_IR/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.435403 ora2-5.0.0/openassessment/locale/fa_IR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    92564 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/fa_IR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   142763 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/fa_IR/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)    13499 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/fa_IR/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    30711 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/fa_IR/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.419402 ora2-5.0.0/openassessment/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.435403 ora2-5.0.0/openassessment/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    81340 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   133090 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)    11874 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/fr/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    29444 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/fr/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.419402 ora2-5.0.0/openassessment/locale/fr_CA/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.435403 ora2-5.0.0/openassessment/locale/fr_CA/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    82568 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/fr_CA/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   136626 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/fr_CA/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)    11820 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/fr_CA/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    31089 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/fr_CA/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.419402 ora2-5.0.0/openassessment/locale/he/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.439403 ora2-5.0.0/openassessment/locale/he/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    48842 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/he/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   117773 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/he/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     7008 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/he/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    27047 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/he/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.419402 ora2-5.0.0/openassessment/locale/hi/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.439403 ora2-5.0.0/openassessment/locale/hi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/hi/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)    95113 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/hi/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     1753 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/hi/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    24633 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/hi/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.419402 ora2-5.0.0/openassessment/locale/id/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.439403 ora2-5.0.0/openassessment/locale/id/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    40223 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/id/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   111930 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/id/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     6748 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/id/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    26550 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/id/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.419402 ora2-5.0.0/openassessment/locale/it_IT/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.439403 ora2-5.0.0/openassessment/locale/it_IT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    81986 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/it_IT/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   132727 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/it_IT/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)    11586 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/it_IT/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    28920 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/it_IT/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.419402 ora2-5.0.0/openassessment/locale/ja_JP/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.439403 ora2-5.0.0/openassessment/locale/ja_JP/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    50706 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/ja_JP/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   118496 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/ja_JP/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     7079 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/ja_JP/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    27020 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/ja_JP/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.419402 ora2-5.0.0/openassessment/locale/ka/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.439403 ora2-5.0.0/openassessment/locale/ka/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    77213 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/ka/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   144721 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/ka/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     8953 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/ka/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    29444 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/ka/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.419402 ora2-5.0.0/openassessment/locale/lt_LT/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.443403 ora2-5.0.0/openassessment/locale/lt_LT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    19263 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/lt_LT/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   102318 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/lt_LT/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     2764 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/lt_LT/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    24738 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/lt_LT/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.419402 ora2-5.0.0/openassessment/locale/lv/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.443403 ora2-5.0.0/openassessment/locale/lv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1383 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/lv/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)    94833 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/lv/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)      962 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/lv/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    23895 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/lv/LC_MESSAGES/djangojs.po
--rw-r--r--   0 runner    (1001) docker     (122)     6039 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/messages.mo
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.419402 ora2-5.0.0/openassessment/locale/mn/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.443403 ora2-5.0.0/openassessment/locale/mn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1741 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/mn/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)    95311 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/mn/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)      559 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/mn/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    22473 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/mn/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.419402 ora2-5.0.0/openassessment/locale/nb/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.443403 ora2-5.0.0/openassessment/locale/nb/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     7793 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/nb/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)    97392 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/nb/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     6672 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/nb/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    26384 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/nb/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.419402 ora2-5.0.0/openassessment/locale/pl/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.443403 ora2-5.0.0/openassessment/locale/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    51135 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   117244 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/pl/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     6823 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/pl/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    26637 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/pl/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.419402 ora2-5.0.0/openassessment/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.443403 ora2-5.0.0/openassessment/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    32487 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   109420 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/pt_BR/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     5663 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/pt_BR/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    26740 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/pt_BR/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.419402 ora2-5.0.0/openassessment/locale/pt_PT/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.443403 ora2-5.0.0/openassessment/locale/pt_PT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    76264 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/pt_PT/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   129689 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/pt_PT/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     8209 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/pt_PT/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    27649 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/pt_PT/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.419402 ora2-5.0.0/openassessment/locale/ro/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.447403 ora2-5.0.0/openassessment/locale/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     2590 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/ro/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)    95431 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/ro/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     2234 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/ro/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    24522 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/ro/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.419402 ora2-5.0.0/openassessment/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.447403 ora2-5.0.0/openassessment/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    59971 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   128218 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     8622 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/ru/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    28603 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/ru/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.419402 ora2-5.0.0/openassessment/locale/sk/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.447403 ora2-5.0.0/openassessment/locale/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     4054 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/sk/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    25387 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/sk/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.419402 ora2-5.0.0/openassessment/locale/sq/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.447403 ora2-5.0.0/openassessment/locale/sq/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     2554 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/sq/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)    95372 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/sq/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     1106 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/sq/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    23998 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/sq/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.419402 ora2-5.0.0/openassessment/locale/sw_KE/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.447403 ora2-5.0.0/openassessment/locale/sw_KE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    43322 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/sw_KE/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   111947 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/sw_KE/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     6441 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/sw_KE/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    26486 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/sw_KE/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.419402 ora2-5.0.0/openassessment/locale/th/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.447403 ora2-5.0.0/openassessment/locale/th/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    27854 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/th/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   111076 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/th/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     4017 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/th/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    26116 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/th/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.419402 ora2-5.0.0/openassessment/locale/tr_TR/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.447403 ora2-5.0.0/openassessment/locale/tr_TR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    46765 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/tr_TR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   114799 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/tr_TR/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     9435 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/tr_TR/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    27701 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/tr_TR/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.419402 ora2-5.0.0/openassessment/locale/uk/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.451403 ora2-5.0.0/openassessment/locale/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)    96047 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     8504 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/uk/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    28734 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/uk/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.419402 ora2-5.0.0/openassessment/locale/vi/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.451403 ora2-5.0.0/openassessment/locale/vi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/vi/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)    99390 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/vi/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     2756 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/vi/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    25235 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/vi/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.419402 ora2-5.0.0/openassessment/locale/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.451403 ora2-5.0.0/openassessment/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    46566 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/zh_CN/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   112823 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/zh_CN/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     6189 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/zh_CN/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    26173 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/zh_CN/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.419402 ora2-5.0.0/openassessment/locale/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.451403 ora2-5.0.0/openassessment/locale/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    25222 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/zh_TW/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   104144 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/zh_TW/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     5023 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/zh_TW/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    25922 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/locale/zh_TW/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.451403 ora2-5.0.0/openassessment/management/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.451403 ora2-5.0.0/openassessment/management/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2422 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/management/commands/collect_ora2_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     6882 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/management/commands/create_oa_submissions.py
--rw-r--r--   0 runner    (1001) docker     (122)    17900 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/management/commands/create_oa_submissions_from_file.py
--rw-r--r--   0 runner    (1001) docker     (122)     5269 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/management/commands/upload_oa_data.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.451403 ora2-5.0.0/openassessment/runtime_imports/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/runtime_imports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1220 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/runtime_imports/classes.py
--rw-r--r--   0 runner    (1001) docker     (122)     1324 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/runtime_imports/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.451403 ora2-5.0.0/openassessment/staffgrader/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/staffgrader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      691 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/staffgrader/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.451403 ora2-5.0.0/openassessment/staffgrader/errors/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/staffgrader/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      297 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/staffgrader/errors/submission_lock.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.455403 ora2-5.0.0/openassessment/staffgrader/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)      809 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/staffgrader/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/staffgrader/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.455403 ora2-5.0.0/openassessment/staffgrader/models/
--rw-r--r--   0 runner    (1001) docker     (122)      132 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/staffgrader/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3511 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/staffgrader/models/submission_lock.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.455403 ora2-5.0.0/openassessment/staffgrader/serializers/
--rw-r--r--   0 runner    (1001) docker     (122)      474 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/staffgrader/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1751 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/staffgrader/serializers/assessments.py
--rw-r--r--   0 runner    (1001) docker     (122)     6089 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/staffgrader/serializers/submission_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     1593 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/staffgrader/serializers/submission_lock.py
--rw-r--r--   0 runner    (1001) docker     (122)    19964 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/staffgrader/staff_grader_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.419402 ora2-5.0.0/openassessment/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.455403 ora2-5.0.0/openassessment/templates/openassessmentblock/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.455403 ora2-5.0.0/openassessment/templates/openassessmentblock/edit/
--rw-r--r--   0 runner    (1001) docker     (122)     1179 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/edit/oa_edit.html
--rw-r--r--   0 runner    (1001) docker     (122)      854 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/edit/oa_edit_assessment_steps.html
--rw-r--r--   0 runner    (1001) docker     (122)    10626 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
--rw-r--r--   0 runner    (1001) docker     (122)     3932 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html
--rw-r--r--   0 runner    (1001) docker     (122)     2818 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/edit/oa_edit_header_and_validation.html
--rw-r--r--   0 runner    (1001) docker     (122)     2499 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/edit/oa_edit_option.html
--rw-r--r--   0 runner    (1001) docker     (122)     4017 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment.html
--rw-r--r--   0 runner    (1001) docker     (122)     2414 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html
--rw-r--r--   0 runner    (1001) docker     (122)     1358 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/edit/oa_edit_prompt.html
--rw-r--r--   0 runner    (1001) docker     (122)     1095 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/edit/oa_edit_prompts.html
--rw-r--r--   0 runner    (1001) docker     (122)     3437 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/edit/oa_edit_rubric.html
--rw-r--r--   0 runner    (1001) docker     (122)     2921 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/edit/oa_edit_schedule.html
--rw-r--r--   0 runner    (1001) docker     (122)      717 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment.html
--rw-r--r--   0 runner    (1001) docker     (122)     2415 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment_schedule.html
--rw-r--r--   0 runner    (1001) docker     (122)      197 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/edit/oa_edit_settings.html
--rw-r--r--   0 runner    (1001) docker     (122)      785 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/edit/oa_edit_staff_assessment.html
--rw-r--r--   0 runner    (1001) docker     (122)     2942 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/edit/oa_edit_student_training.html
--rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/edit/oa_rubric_reuse.html
--rw-r--r--   0 runner    (1001) docker     (122)     1531 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/edit/oa_training_example.html
--rw-r--r--   0 runner    (1001) docker     (122)     1174 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/edit/oa_training_example_criterion.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.459403 ora2-5.0.0/openassessment/templates/openassessmentblock/grade/
--rw-r--r--   0 runner    (1001) docker     (122)     1437 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/grade/oa_assessment_feedback.html
--rw-r--r--   0 runner    (1001) docker     (122)     1328 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/grade/oa_assessment_title.html
--rw-r--r--   0 runner    (1001) docker     (122)     2342 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/grade/oa_grade_cancelled.html
--rw-r--r--   0 runner    (1001) docker     (122)    17846 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/grade/oa_grade_complete.html
--rw-r--r--   0 runner    (1001) docker     (122)     1779 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/grade/oa_grade_incomplete.html
--rw-r--r--   0 runner    (1001) docker     (122)     1445 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/grade/oa_grade_not_started.html
--rw-r--r--   0 runner    (1001) docker     (122)     1994 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/grade/oa_grade_waiting.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.459403 ora2-5.0.0/openassessment/templates/openassessmentblock/icons/
--rw-r--r--   0 runner    (1001) docker     (122)      208 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/icons/warning_filled.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.459403 ora2-5.0.0/openassessment/templates/openassessmentblock/instructor_dashboard/
--rw-r--r--   0 runner    (1001) docker     (122)     1471 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/instructor_dashboard/oa_grade_available_responses.html
--rw-r--r--   0 runner    (1001) docker     (122)      966 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/instructor_dashboard/oa_listing.html
--rw-r--r--   0 runner    (1001) docker     (122)     1225 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/instructor_dashboard/oa_waiting_step_details.html
--rw-r--r--   0 runner    (1001) docker     (122)      454 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/instructor_dashboard/open-response-assessment-summary.underscore
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.459403 ora2-5.0.0/openassessment/templates/openassessmentblock/leaderboard/
--rw-r--r--   0 runner    (1001) docker     (122)     2008 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/leaderboard/oa_leaderboard_show.html
--rw-r--r--   0 runner    (1001) docker     (122)     1276 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/leaderboard/oa_leaderboard_waiting.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.459403 ora2-5.0.0/openassessment/templates/openassessmentblock/message/
--rw-r--r--   0 runner    (1001) docker     (122)      743 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/message/oa_message_cancelled.html
--rw-r--r--   0 runner    (1001) docker     (122)      660 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/message/oa_message_closed.html
--rw-r--r--   0 runner    (1001) docker     (122)      708 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/message/oa_message_complete.html
--rw-r--r--   0 runner    (1001) docker     (122)     4279 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/message/oa_message_incomplete.html
--rw-r--r--   0 runner    (1001) docker     (122)      653 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/message/oa_message_no_team.html
--rw-r--r--   0 runner    (1001) docker     (122)      951 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/message/oa_message_open.html
--rw-r--r--   0 runner    (1001) docker     (122)      354 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/message/oa_message_unavailable.html
--rw-r--r--   0 runner    (1001) docker     (122)     2414 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/oa_base.html
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/oa_error.html
--rw-r--r--   0 runner    (1001) docker     (122)     1026 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/oa_latex_preview.html
--rw-r--r--   0 runner    (1001) docker     (122)     6927 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/oa_rubric.html
--rw-r--r--   0 runner    (1001) docker     (122)     1519 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/oa_submission_answer.html
--rw-r--r--   0 runner    (1001) docker     (122)     2093 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/oa_team_uploaded_files.html
--rw-r--r--   0 runner    (1001) docker     (122)     2830 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/oa_uploaded_file.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.459403 ora2-5.0.0/openassessment/templates/openassessmentblock/peer/
--rw-r--r--   0 runner    (1001) docker     (122)     5758 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/peer/oa_peer_assessment.html
--rw-r--r--   0 runner    (1001) docker     (122)      709 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/peer/oa_peer_cancelled.html
--rw-r--r--   0 runner    (1001) docker     (122)     1930 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/peer/oa_peer_closed.html
--rw-r--r--   0 runner    (1001) docker     (122)     2330 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/peer/oa_peer_complete.html
--rw-r--r--   0 runner    (1001) docker     (122)     3855 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode.html
--rw-r--r--   0 runner    (1001) docker     (122)     1932 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode_waiting.html
--rw-r--r--   0 runner    (1001) docker     (122)      633 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/peer/oa_peer_unavailable.html
--rw-r--r--   0 runner    (1001) docker     (122)     1937 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/peer/oa_peer_waiting.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.459403 ora2-5.0.0/openassessment/templates/openassessmentblock/response/
--rw-r--r--   0 runner    (1001) docker     (122)    21833 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/response/oa_response.html
--rw-r--r--   0 runner    (1001) docker     (122)     2577 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/response/oa_response_cancelled.html
--rw-r--r--   0 runner    (1001) docker     (122)     1597 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/response/oa_response_closed.html
--rw-r--r--   0 runner    (1001) docker     (122)     2030 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/response/oa_response_graded.html
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/response/oa_response_studio_preview.html
--rw-r--r--   0 runner    (1001) docker     (122)     3728 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/response/oa_response_submitted.html
--rw-r--r--   0 runner    (1001) docker     (122)     1625 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/response/oa_response_team_already_submitted.html
--rw-r--r--   0 runner    (1001) docker     (122)      628 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/response/oa_response_unavailable.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.463403 ora2-5.0.0/openassessment/templates/openassessmentblock/self/
--rw-r--r--   0 runner    (1001) docker     (122)     4593 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/self/oa_self_assessment.html
--rw-r--r--   0 runner    (1001) docker     (122)      752 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/self/oa_self_cancelled.html
--rw-r--r--   0 runner    (1001) docker     (122)     1503 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/self/oa_self_closed.html
--rw-r--r--   0 runner    (1001) docker     (122)      730 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/self/oa_self_complete.html
--rw-r--r--   0 runner    (1001) docker     (122)      676 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/self/oa_self_unavailable.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.463403 ora2-5.0.0/openassessment/templates/openassessmentblock/staff/
--rw-r--r--   0 runner    (1001) docker     (122)     1707 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/staff/oa_staff_grade.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.463403 ora2-5.0.0/openassessment/templates/openassessmentblock/staff_area/
--rw-r--r--   0 runner    (1001) docker     (122)     8449 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html
--rw-r--r--   0 runner    (1001) docker     (122)      887 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners.html
--rw-r--r--   0 runner    (1001) docker     (122)     3927 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html
--rw-r--r--   0 runner    (1001) docker     (122)      407 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_count.html
--rw-r--r--   0 runner    (1001) docker     (122)     3167 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/staff_area/oa_staff_override_assessment.html
--rw-r--r--   0 runner    (1001) docker     (122)    16404 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/staff_area/oa_student_info.html
--rw-r--r--   0 runner    (1001) docker     (122)     3732 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.463403 ora2-5.0.0/openassessment/templates/openassessmentblock/student_training/
--rw-r--r--   0 runner    (1001) docker     (122)    11281 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/student_training/student_training.html
--rw-r--r--   0 runner    (1001) docker     (122)      652 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/student_training/student_training_cancelled.html
--rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/student_training/student_training_closed.html
--rw-r--r--   0 runner    (1001) docker     (122)      653 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/student_training/student_training_complete.html
--rw-r--r--   0 runner    (1001) docker     (122)     1137 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/student_training/student_training_error.html
--rw-r--r--   0 runner    (1001) docker     (122)      599 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templates/openassessmentblock/student_training/student_training_unavailable.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.463403 ora2-5.0.0/openassessment/templatetags/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      886 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/templatetags/oa_extras.py
--rw-r--r--   0 runner    (1001) docker     (122)      758 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.463403 ora2-5.0.0/openassessment/workflow/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1533 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/workflow/admin.py
--rw-r--r--   0 runner    (1001) docker     (122)    19932 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/workflow/api.py
--rw-r--r--   0 runner    (1001) docker     (122)     1589 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/workflow/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.463403 ora2-5.0.0/openassessment/workflow/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     3111 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/workflow/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)      383 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/workflow/migrations/0002_remove_django_extensions.py
--rw-r--r--   0 runner    (1001) docker     (122)      826 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/workflow/migrations/0003_TeamWorkflows.py
--rw-r--r--   0 runner    (1001) docker     (122)      412 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/workflow/migrations/0004_assessmentworkflowstep_skipped.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/workflow/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    44741 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/workflow/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     1660 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/workflow/serializers.py
--rw-r--r--   0 runner    (1001) docker     (122)     8350 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/workflow/team_api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.467403 ora2-5.0.0/openassessment/xblock/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5880 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/config_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)      914 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/course_items_listing_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)     7889 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/data_conversion.py
--rw-r--r--   0 runner    (1001) docker     (122)     6829 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/defaults.py
--rw-r--r--   0 runner    (1001) docker     (122)      622 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/editor_config.py
--rw-r--r--   0 runner    (1001) docker     (122)    30777 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/grade_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)     5837 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/leaderboard_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)     3827 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/lms_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)     1808 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/load_static.py
--rw-r--r--   0 runner    (1001) docker     (122)     9846 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/message_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)      770 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/mobile.py
--rw-r--r--   0 runner    (1001) docker     (122)     3708 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/openassesment_template_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)    51009 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/openassessmentblock.py
--rw-r--r--   0 runner    (1001) docker     (122)    14943 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/peer_assessment_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)    10329 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/resolve_dates.py
--rw-r--r--   0 runner    (1001) docker     (122)     4560 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/rubric_reuse_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)     5369 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     7825 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/self_assessment_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)    34259 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/staff_area_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)     9317 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/staff_assessment_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.423403 ora2-5.0.0/openassessment/xblock/static/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.423403 ora2-5.0.0/openassessment/xblock/static/css/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.423403 ora2-5.0.0/openassessment/xblock/static/css/lib/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.467403 ora2-5.0.0/openassessment/xblock/static/css/lib/backgrid/
--rw-r--r--   0 runner    (1001) docker     (122)     5382 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/css/lib/backgrid/backgrid.css
--rw-r--r--   0 runner    (1001) docker     (122)     4414 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/css/lib/backgrid/backgrid.min.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.503404 ora2-5.0.0/openassessment/xblock/static/dist/
--rw-r--r--   0 runner    (1001) docker     (122)     1617 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/dist/manifest.json
--rw-r--r--   0 runner    (1001) docker     (122)     1834 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/dist/openassessment-editor-textarea.2774cf3b7c8fadda4341.js
--rw-r--r--   0 runner    (1001) docker     (122)    38550 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/dist/openassessment-editor-textarea.js
--rw-r--r--   0 runner    (1001) docker     (122)     2973 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/dist/openassessment-editor-tinymce.6a6113da3309f666ccda.js
--rw-r--r--   0 runner    (1001) docker     (122)    47578 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/dist/openassessment-editor-tinymce.js
--rw-r--r--   0 runner    (1001) docker     (122)       72 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/dist/openassessment-lms.7c3203918ed22728dd89.css
--rw-r--r--   0 runner    (1001) docker     (122)  1319515 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/dist/openassessment-lms.7c3203918ed22728dd89.js
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/dist/openassessment-lms.css
--rw-r--r--   0 runner    (1001) docker     (122) 28594064 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/dist/openassessment-lms.js
--rw-r--r--   0 runner    (1001) docker     (122)   753258 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/dist/openassessment-ltr.cc6fb8c044bfe2899cd5.css
--rw-r--r--   0 runner    (1001) docker     (122)     1007 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/dist/openassessment-ltr.cc6fb8c044bfe2899cd5.js
--rw-r--r--   0 runner    (1001) docker     (122)   846937 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/dist/openassessment-ltr.css
--rw-r--r--   0 runner    (1001) docker     (122)    32672 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/dist/openassessment-ltr.js
--rw-r--r--   0 runner    (1001) docker     (122)   753287 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/dist/openassessment-rtl.55343890f44133115ca3.css
--rw-r--r--   0 runner    (1001) docker     (122)     1007 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/dist/openassessment-rtl.55343890f44133115ca3.js
--rw-r--r--   0 runner    (1001) docker     (122)   846966 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/dist/openassessment-rtl.css
--rw-r--r--   0 runner    (1001) docker     (122)    32672 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/dist/openassessment-rtl.js
--rw-r--r--   0 runner    (1001) docker     (122)   235846 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/dist/openassessment-studio.6fd5da4c0a2e58a8aba2.js
--rw-r--r--   0 runner    (1001) docker     (122)  2305380 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/dist/openassessment-studio.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.423403 ora2-5.0.0/openassessment/xblock/static/js/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.423403 ora2-5.0.0/openassessment/xblock/static/js/lib/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.507404 ora2-5.0.0/openassessment/xblock/static/js/lib/backgrid/
--rw-r--r--   0 runner    (1001) docker     (122)    87583 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/js/lib/backgrid/backgrid.js
--rw-r--r--   0 runner    (1001) docker     (122)    26169 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/js/lib/backgrid/backgrid.min.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.507404 ora2-5.0.0/openassessment/xblock/static/js/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.511404 ora2-5.0.0/openassessment/xblock/static/js/src/lms/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.511404 ora2-5.0.0/openassessment/xblock/static/js/src/lms/api/
--rw-r--r--   0 runner    (1001) docker     (122)      817 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/js/src/lms/api/waiting_step_details.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.511404 ora2-5.0.0/openassessment/xblock/static/js/src/lms/editors/
--rw-r--r--   0 runner    (1001) docker     (122)     1368 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/js/src/lms/editors/oa_editor_textarea.js
--rw-r--r--   0 runner    (1001) docker     (122)     3741 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/js/src/lms/editors/oa_editor_tinymce.js
--rw-r--r--   0 runner    (1001) docker     (122)    18084 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/js/src/lms/oa_base.js
--rw-r--r--   0 runner    (1001) docker     (122)     1878 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/js/src/lms/oa_confirmation_alert.js
--rw-r--r--   0 runner    (1001) docker     (122)    10567 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/js/src/lms/oa_course_items_listing.js
--rw-r--r--   0 runner    (1001) docker     (122)     1994 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/js/src/lms/oa_datefactory.js
--rw-r--r--   0 runner    (1001) docker     (122)     2013 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/js/src/lms/oa_file_upload.js
--rw-r--r--   0 runner    (1001) docker     (122)     8877 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/js/src/lms/oa_grade.js
--rw-r--r--   0 runner    (1001) docker     (122)     1873 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/js/src/lms/oa_leaderboard.js
--rw-r--r--   0 runner    (1001) docker     (122)      910 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/js/src/lms/oa_message.js
--rw-r--r--   0 runner    (1001) docker     (122)     9796 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/js/src/lms/oa_peer.js
--rw-r--r--   0 runner    (1001) docker     (122)     1882 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/js/src/lms/oa_prompts.js
--rw-r--r--   0 runner    (1001) docker     (122)    32621 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/js/src/lms/oa_response.js
--rw-r--r--   0 runner    (1001) docker     (122)     1860 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/js/src/lms/oa_response_editor.js
--rw-r--r--   0 runner    (1001) docker     (122)     7024 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/js/src/lms/oa_rubric.js
--rw-r--r--   0 runner    (1001) docker     (122)     5344 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/js/src/lms/oa_self.js
--rw-r--r--   0 runner    (1001) docker     (122)     1351 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/js/src/lms/oa_staff.js
--rw-r--r--   0 runner    (1001) docker     (122)    24786 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/js/src/lms/oa_staff_area.js
--rw-r--r--   0 runner    (1001) docker     (122)     5267 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/js/src/lms/oa_training.js
--rw-r--r--   0 runner    (1001) docker     (122)      400 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/js/src/lms_index.js
--rw-r--r--   0 runner    (1001) docker     (122)    26166 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/js/src/oa_server.js
--rw-r--r--   0 runner    (1001) docker     (122)      963 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/js/src/oa_shared.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.511404 ora2-5.0.0/openassessment/xblock/static/js/src/studio/
--rw-r--r--   0 runner    (1001) docker     (122)     7705 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/js/src/studio/oa_container.js
--rw-r--r--   0 runner    (1001) docker     (122)    20684 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/js/src/studio/oa_container_item.js
--rw-r--r--   0 runner    (1001) docker     (122)    12727 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/js/src/studio/oa_edit.js
--rw-r--r--   0 runner    (1001) docker     (122)    15956 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/js/src/studio/oa_edit_assessment.js
--rw-r--r--   0 runner    (1001) docker     (122)     6121 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/js/src/studio/oa_edit_assessments_steps.js
--rw-r--r--   0 runner    (1001) docker     (122)    11441 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/js/src/studio/oa_edit_fields.js
--rw-r--r--   0 runner    (1001) docker     (122)    13033 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/js/src/studio/oa_edit_listeners.js
--rw-r--r--   0 runner    (1001) docker     (122)     1282 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/js/src/studio/oa_edit_notifier.js
--rw-r--r--   0 runner    (1001) docker     (122)     3277 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/js/src/studio/oa_edit_prompts.js
--rw-r--r--   0 runner    (1001) docker     (122)    13149 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/js/src/studio/oa_edit_rubric.js
--rw-r--r--   0 runner    (1001) docker     (122)     4349 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/js/src/studio/oa_edit_schedule.js
--rw-r--r--   0 runner    (1001) docker     (122)    15272 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/js/src/studio/oa_edit_settings.js
--rw-r--r--   0 runner    (1001) docker     (122)     3746 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/js/src/studio/oa_edit_validation_alert.js
--rw-r--r--   0 runner    (1001) docker     (122)     2654 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/js/src/studio/oa_tiny_mce.js
--rw-r--r--   0 runner    (1001) docker     (122)      133 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/static/js/src/studio_index.js
--rw-r--r--   0 runner    (1001) docker     (122)    11859 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/student_training_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)    20538 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/studio_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)    42012 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/submission_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)     8743 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/team_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)     4631 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/team_workflow_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)      675 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/user_data.py
--rw-r--r--   0 runner    (1001) docker     (122)    15746 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/validation.py
--rw-r--r--   0 runner    (1001) docker     (122)     8409 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/workflow_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)    35842 2023-02-01 15:47:43.000000 ora2-5.0.0/openassessment/xblock/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.511404 ora2-5.0.0/ora2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2643 2023-02-01 15:47:49.000000 ora2-5.0.0/ora2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    23039 2023-02-01 15:47:49.000000 ora2-5.0.0/ora2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-01 15:47:49.000000 ora2-5.0.0/ora2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-02-01 15:47:49.000000 ora2-5.0.0/ora2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      289 2023-02-01 15:47:49.000000 ora2-5.0.0/ora2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-02-01 15:47:49.000000 ora2-5.0.0/ora2.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-01 15:47:49.515404 ora2-5.0.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      413 2023-02-01 15:47:43.000000 ora2-5.0.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)       40 2023-02-01 15:47:43.000000 ora2-5.0.0/requirements/ci.in
--rw-r--r--   0 runner    (1001) docker     (122)      179 2023-02-01 15:47:43.000000 ora2-5.0.0/requirements/pip-tools.in
--rw-r--r--   0 runner    (1001) docker     (122)       91 2023-02-01 15:47:43.000000 ora2-5.0.0/requirements/pip.in
--rw-r--r--   0 runner    (1001) docker     (122)      174 2023-02-01 15:47:43.000000 ora2-5.0.0/requirements/quality.in
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-02-01 15:47:43.000000 ora2-5.0.0/requirements/test-acceptance.in
--rw-r--r--   0 runner    (1001) docker     (122)      685 2023-02-01 15:47:43.000000 ora2-5.0.0/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-02-01 15:47:43.000000 ora2-5.0.0/requirements/tox.in
--rw-r--r--   0 runner    (1001) docker     (122)      318 2023-02-01 15:47:49.515404 ora2-5.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2593 2023-02-01 15:47:43.000000 ora2-5.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.452661 ora2-5.0.1/
+-rw-r--r--   0 runner    (1001) docker     (122)    35135 2023-05-25 19:16:34.000000 ora2-5.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      682 2023-05-25 19:16:34.000000 ora2-5.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2643 2023-05-25 19:16:40.452661 ora2-5.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2038 2023-05-25 19:16:34.000000 ora2-5.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.308660 ora2-5.0.1/openassessment/
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.308660 ora2-5.0.1/openassessment/assessment/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/assessment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5633 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/assessment/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.308660 ora2-5.0.1/openassessment/assessment/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/assessment/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39052 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/assessment/api/peer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11874 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/assessment/api/self.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16433 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/assessment/api/staff.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16864 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/assessment/api/student_training.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12955 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/assessment/api/teams.py
+-rw-r--r--   0 runner    (1001) docker     (122)      442 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/assessment/data_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.312660 ora2-5.0.1/openassessment/assessment/errors/
+-rw-r--r--   0 runner    (1001) docker     (122)      182 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/assessment/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      189 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/assessment/errors/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1117 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/assessment/errors/peer.py
+-rw-r--r--   0 runner    (1001) docker     (122)      552 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/assessment/errors/self.py
+-rw-r--r--   0 runner    (1001) docker     (122)      821 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/assessment/errors/staff.py
+-rw-r--r--   0 runner    (1001) docker     (122)      440 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/assessment/errors/student_training.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.312660 ora2-5.0.1/openassessment/assessment/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     9361 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/assessment/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1333 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/assessment/migrations/0002_staffworkflow.py
+-rw-r--r--   0 runner    (1001) docker     (122)      750 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/assessment/migrations/0003_expand_course_id.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3459 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/assessment/migrations/0004_historicalsharedfileupload_sharedfileupload.py
+-rw-r--r--   0 runner    (1001) docker     (122)      618 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/assessment/migrations/0005_add_filename_to_sharedupload.py
+-rw-r--r--   0 runner    (1001) docker     (122)      744 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/assessment/migrations/0006_TeamWorkflows.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1218 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/assessment/migrations/0007_staff_workflow_blank.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/assessment/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.312660 ora2-5.0.1/openassessment/assessment/models/
+-rw-r--r--   0 runner    (1001) docker     (122)      205 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/assessment/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32191 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/assessment/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22340 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/assessment/models/peer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8558 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/assessment/models/staff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8200 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/assessment/models/student_training.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4991 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/assessment/models/training.py
+-rw-r--r--   0 runner    (1001) docker     (122)      163 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/assessment/score_type_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.312660 ora2-5.0.1/openassessment/assessment/serializers/
+-rw-r--r--   0 runner    (1001) docker     (122)      151 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/assessment/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10553 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/assessment/serializers/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2021 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/assessment/serializers/peer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6217 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/assessment/serializers/training.py
+-rw-r--r--   0 runner    (1001) docker     (122)      376 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/assessment/signals.py
+-rw-r--r--   0 runner    (1001) docker     (122)      265 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/assessment/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1874 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/assessment/views.py
+-rw-r--r--   0 runner    (1001) docker     (122)    58992 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/data.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.316660 ora2-5.0.1/openassessment/fileupload/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/fileupload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23578 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/fileupload/api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.316660 ora2-5.0.1/openassessment/fileupload/backends/
+-rw-r--r--   0 runner    (1001) docker     (122)      849 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/fileupload/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5253 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/fileupload/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2411 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/fileupload/backends/django_storage.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4122 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/fileupload/backends/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3034 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/fileupload/backends/s3.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3392 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/fileupload/backends/swift.py
+-rw-r--r--   0 runner    (1001) docker     (122)      740 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/fileupload/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      412 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/fileupload/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)      498 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/fileupload/views_django_storage.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5105 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/fileupload/views_filesystem.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.316660 ora2-5.0.1/openassessment/locale/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.296660 ora2-5.0.1/openassessment/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.316660 ora2-5.0.1/openassessment/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    82260 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   137572 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)    10517 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/ar/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    29332 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/ar/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.296660 ora2-5.0.1/openassessment/locale/ar_SA/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.316660 ora2-5.0.1/openassessment/locale/ar_SA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     9218 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/ar_SA/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    28056 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/ar_SA/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.296660 ora2-5.0.1/openassessment/locale/de_DE/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.316660 ora2-5.0.1/openassessment/locale/de_DE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    64223 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/de_DE/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   124947 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/de_DE/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     8402 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/de_DE/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    27871 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/de_DE/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.296660 ora2-5.0.1/openassessment/locale/el/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.320660 ora2-5.0.1/openassessment/locale/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    35998 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/el/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   116285 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/el/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     5045 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/el/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    26850 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/el/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.296660 ora2-5.0.1/openassessment/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.320660 ora2-5.0.1/openassessment/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      382 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    94672 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)      425 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/en/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    23724 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/en/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.296660 ora2-5.0.1/openassessment/locale/eo/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.320660 ora2-5.0.1/openassessment/locale/eo/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)   145495 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/eo/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   195906 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/eo/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)    21982 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/eo/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    38500 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/eo/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.300660 ora2-5.0.1/openassessment/locale/es_419/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.320660 ora2-5.0.1/openassessment/locale/es_419/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    81996 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/es_419/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   133250 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/es_419/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)    11545 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/es_419/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    29006 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/es_419/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.300660 ora2-5.0.1/openassessment/locale/es_AR/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.320660 ora2-5.0.1/openassessment/locale/es_AR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    11444 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/es_AR/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    28411 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/es_AR/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.300660 ora2-5.0.1/openassessment/locale/es_ES/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.324660 ora2-5.0.1/openassessment/locale/es_ES/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    82594 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/es_ES/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   133560 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/es_ES/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)    11635 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/es_ES/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    29042 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/es_ES/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.300660 ora2-5.0.1/openassessment/locale/eu_ES/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.324660 ora2-5.0.1/openassessment/locale/eu_ES/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    14552 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/eu_ES/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   100050 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/eu_ES/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     3947 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/eu_ES/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    25057 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/eu_ES/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.300660 ora2-5.0.1/openassessment/locale/fa_IR/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.324660 ora2-5.0.1/openassessment/locale/fa_IR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    92564 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/fa_IR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   142763 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/fa_IR/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)    13499 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/fa_IR/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    30711 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/fa_IR/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.300660 ora2-5.0.1/openassessment/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.328660 ora2-5.0.1/openassessment/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    81340 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   133090 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)    11874 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/fr/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    29444 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/fr/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.300660 ora2-5.0.1/openassessment/locale/fr_CA/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.328660 ora2-5.0.1/openassessment/locale/fr_CA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    82568 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/fr_CA/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   136626 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/fr_CA/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)    11820 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/fr_CA/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    31089 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/fr_CA/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.300660 ora2-5.0.1/openassessment/locale/he/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.328660 ora2-5.0.1/openassessment/locale/he/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    48842 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/he/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   117773 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/he/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     7008 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/he/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    27047 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/he/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.300660 ora2-5.0.1/openassessment/locale/hi/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.332660 ora2-5.0.1/openassessment/locale/hi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/hi/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    95113 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/hi/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     1753 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/hi/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    24633 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/hi/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.300660 ora2-5.0.1/openassessment/locale/id/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.332660 ora2-5.0.1/openassessment/locale/id/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    40204 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/id/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   112010 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/id/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     6748 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/id/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    26550 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/id/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.300660 ora2-5.0.1/openassessment/locale/it_IT/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.332660 ora2-5.0.1/openassessment/locale/it_IT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    81986 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/it_IT/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   132727 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)    11586 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/it_IT/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    28920 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/it_IT/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.300660 ora2-5.0.1/openassessment/locale/ja_JP/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.336660 ora2-5.0.1/openassessment/locale/ja_JP/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    50706 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/ja_JP/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   118496 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/ja_JP/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     7079 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/ja_JP/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    27020 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/ja_JP/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.300660 ora2-5.0.1/openassessment/locale/ka/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.336660 ora2-5.0.1/openassessment/locale/ka/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    77213 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/ka/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   144721 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/ka/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     8953 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/ka/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    29444 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/ka/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.300660 ora2-5.0.1/openassessment/locale/lt_LT/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.336660 ora2-5.0.1/openassessment/locale/lt_LT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    19263 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/lt_LT/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   102318 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/lt_LT/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     2764 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/lt_LT/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    24738 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/lt_LT/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.300660 ora2-5.0.1/openassessment/locale/lv/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.340660 ora2-5.0.1/openassessment/locale/lv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1383 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/lv/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    94833 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/lv/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)      962 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/lv/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    23895 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/lv/LC_MESSAGES/djangojs.po
+-rw-r--r--   0 runner    (1001) docker     (122)     6039 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/messages.mo
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.300660 ora2-5.0.1/openassessment/locale/mn/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.340660 ora2-5.0.1/openassessment/locale/mn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1741 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/mn/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    95311 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/mn/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)      559 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/mn/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    22473 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/mn/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.300660 ora2-5.0.1/openassessment/locale/nb/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.340660 ora2-5.0.1/openassessment/locale/nb/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     7793 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/nb/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    97392 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/nb/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     6672 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/nb/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    26384 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/nb/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.300660 ora2-5.0.1/openassessment/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.340660 ora2-5.0.1/openassessment/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    51135 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   117244 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/pl/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     6823 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/pl/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    26637 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/pl/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.300660 ora2-5.0.1/openassessment/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.344660 ora2-5.0.1/openassessment/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    32487 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   109420 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/pt_BR/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     5663 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/pt_BR/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    26740 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/pt_BR/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.300660 ora2-5.0.1/openassessment/locale/pt_PT/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.344660 ora2-5.0.1/openassessment/locale/pt_PT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    81743 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/pt_PT/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   132378 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/pt_PT/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)    11556 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/pt_PT/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    29200 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/pt_PT/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.300660 ora2-5.0.1/openassessment/locale/ro/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.344660 ora2-5.0.1/openassessment/locale/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     2590 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/ro/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    95431 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/ro/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     2234 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/ro/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    24522 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/ro/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.300660 ora2-5.0.1/openassessment/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.344660 ora2-5.0.1/openassessment/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    59971 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   128218 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     8622 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/ru/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    28603 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/ru/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.300660 ora2-5.0.1/openassessment/locale/sk/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.348661 ora2-5.0.1/openassessment/locale/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     4054 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/sk/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    25387 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/sk/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.300660 ora2-5.0.1/openassessment/locale/sq/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.348661 ora2-5.0.1/openassessment/locale/sq/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     2554 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/sq/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    95372 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/sq/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     1106 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/sq/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    23998 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/sq/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.300660 ora2-5.0.1/openassessment/locale/sw_KE/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.348661 ora2-5.0.1/openassessment/locale/sw_KE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    43322 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/sw_KE/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   111947 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/sw_KE/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     6441 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/sw_KE/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    26486 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/sw_KE/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.300660 ora2-5.0.1/openassessment/locale/th/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.348661 ora2-5.0.1/openassessment/locale/th/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    27854 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/th/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   111076 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/th/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     4017 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/th/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    26116 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/th/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.300660 ora2-5.0.1/openassessment/locale/tr_TR/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.352661 ora2-5.0.1/openassessment/locale/tr_TR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    49577 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/tr_TR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   116193 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/tr_TR/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     9435 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/tr_TR/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    27701 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/tr_TR/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.300660 ora2-5.0.1/openassessment/locale/uk/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.352661 ora2-5.0.1/openassessment/locale/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    96047 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     8504 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/uk/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    28734 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/uk/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.300660 ora2-5.0.1/openassessment/locale/vi/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.352661 ora2-5.0.1/openassessment/locale/vi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/vi/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    99390 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/vi/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     2756 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/vi/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    25235 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/vi/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.300660 ora2-5.0.1/openassessment/locale/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.352661 ora2-5.0.1/openassessment/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    46566 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/zh_CN/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   112823 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/zh_CN/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     6189 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/zh_CN/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    26173 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/zh_CN/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.304660 ora2-5.0.1/openassessment/locale/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.356660 ora2-5.0.1/openassessment/locale/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    25222 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/zh_TW/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   104144 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/zh_TW/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     5023 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/zh_TW/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    25922 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/locale/zh_TW/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.356660 ora2-5.0.1/openassessment/management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.356660 ora2-5.0.1/openassessment/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2422 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/management/commands/collect_ora2_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6882 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/management/commands/create_oa_submissions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17900 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/management/commands/create_oa_submissions_from_file.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5269 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/management/commands/upload_oa_data.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.356660 ora2-5.0.1/openassessment/runtime_imports/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/runtime_imports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1220 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/runtime_imports/classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1324 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/runtime_imports/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.360661 ora2-5.0.1/openassessment/staffgrader/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/staffgrader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      691 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/staffgrader/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.360661 ora2-5.0.1/openassessment/staffgrader/errors/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/staffgrader/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/staffgrader/errors/submission_lock.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.360661 ora2-5.0.1/openassessment/staffgrader/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)      809 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/staffgrader/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/staffgrader/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.360661 ora2-5.0.1/openassessment/staffgrader/models/
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/staffgrader/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3511 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/staffgrader/models/submission_lock.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.360661 ora2-5.0.1/openassessment/staffgrader/serializers/
+-rw-r--r--   0 runner    (1001) docker     (122)      474 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/staffgrader/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1751 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/staffgrader/serializers/assessments.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6089 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/staffgrader/serializers/submission_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1593 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/staffgrader/serializers/submission_lock.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19964 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/staffgrader/staff_grader_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.304660 ora2-5.0.1/openassessment/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.364661 ora2-5.0.1/openassessment/templates/openassessmentblock/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.368661 ora2-5.0.1/openassessment/templates/openassessmentblock/edit/
+-rw-r--r--   0 runner    (1001) docker     (122)     1179 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/edit/oa_edit.html
+-rw-r--r--   0 runner    (1001) docker     (122)      854 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/edit/oa_edit_assessment_steps.html
+-rw-r--r--   0 runner    (1001) docker     (122)    10626 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3932 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2818 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/edit/oa_edit_header_and_validation.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2499 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/edit/oa_edit_option.html
+-rw-r--r--   0 runner    (1001) docker     (122)     4017 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2414 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1358 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/edit/oa_edit_prompt.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1095 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/edit/oa_edit_prompts.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3437 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/edit/oa_edit_rubric.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2921 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/edit/oa_edit_schedule.html
+-rw-r--r--   0 runner    (1001) docker     (122)      717 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2415 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment_schedule.html
+-rw-r--r--   0 runner    (1001) docker     (122)      197 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/edit/oa_edit_settings.html
+-rw-r--r--   0 runner    (1001) docker     (122)      785 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/edit/oa_edit_staff_assessment.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2942 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/edit/oa_edit_student_training.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/edit/oa_rubric_reuse.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1531 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/edit/oa_training_example.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1174 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/edit/oa_training_example_criterion.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.368661 ora2-5.0.1/openassessment/templates/openassessmentblock/grade/
+-rw-r--r--   0 runner    (1001) docker     (122)     1437 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/grade/oa_assessment_feedback.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1328 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/grade/oa_assessment_title.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2342 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/grade/oa_grade_cancelled.html
+-rw-r--r--   0 runner    (1001) docker     (122)    17846 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/grade/oa_grade_complete.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1779 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/grade/oa_grade_incomplete.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1445 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/grade/oa_grade_not_started.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1994 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/grade/oa_grade_waiting.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.368661 ora2-5.0.1/openassessment/templates/openassessmentblock/icons/
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/icons/warning_filled.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.368661 ora2-5.0.1/openassessment/templates/openassessmentblock/instructor_dashboard/
+-rw-r--r--   0 runner    (1001) docker     (122)     1471 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/instructor_dashboard/oa_grade_available_responses.html
+-rw-r--r--   0 runner    (1001) docker     (122)      966 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/instructor_dashboard/oa_listing.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1225 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/instructor_dashboard/oa_waiting_step_details.html
+-rw-r--r--   0 runner    (1001) docker     (122)      454 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/instructor_dashboard/open-response-assessment-summary.underscore
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.368661 ora2-5.0.1/openassessment/templates/openassessmentblock/leaderboard/
+-rw-r--r--   0 runner    (1001) docker     (122)     2008 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/leaderboard/oa_leaderboard_show.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1276 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/leaderboard/oa_leaderboard_waiting.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.372661 ora2-5.0.1/openassessment/templates/openassessmentblock/message/
+-rw-r--r--   0 runner    (1001) docker     (122)      743 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/message/oa_message_cancelled.html
+-rw-r--r--   0 runner    (1001) docker     (122)      660 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/message/oa_message_closed.html
+-rw-r--r--   0 runner    (1001) docker     (122)      708 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/message/oa_message_complete.html
+-rw-r--r--   0 runner    (1001) docker     (122)     4279 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/message/oa_message_incomplete.html
+-rw-r--r--   0 runner    (1001) docker     (122)      653 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/message/oa_message_no_team.html
+-rw-r--r--   0 runner    (1001) docker     (122)      951 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/message/oa_message_open.html
+-rw-r--r--   0 runner    (1001) docker     (122)      354 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/message/oa_message_unavailable.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2414 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/oa_base.html
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/oa_error.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1026 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/oa_latex_preview.html
+-rw-r--r--   0 runner    (1001) docker     (122)     6927 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/oa_rubric.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1519 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/oa_submission_answer.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2093 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/oa_team_uploaded_files.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2830 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/oa_uploaded_file.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.372661 ora2-5.0.1/openassessment/templates/openassessmentblock/peer/
+-rw-r--r--   0 runner    (1001) docker     (122)     5758 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/peer/oa_peer_assessment.html
+-rw-r--r--   0 runner    (1001) docker     (122)      709 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/peer/oa_peer_cancelled.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1930 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/peer/oa_peer_closed.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2330 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/peer/oa_peer_complete.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3855 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1932 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode_waiting.html
+-rw-r--r--   0 runner    (1001) docker     (122)      633 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/peer/oa_peer_unavailable.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1937 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/peer/oa_peer_waiting.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.380661 ora2-5.0.1/openassessment/templates/openassessmentblock/response/
+-rw-r--r--   0 runner    (1001) docker     (122)    21833 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/response/oa_response.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2577 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/response/oa_response_cancelled.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1597 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/response/oa_response_closed.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2030 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/response/oa_response_graded.html
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/response/oa_response_studio_preview.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3728 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/response/oa_response_submitted.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1625 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/response/oa_response_team_already_submitted.html
+-rw-r--r--   0 runner    (1001) docker     (122)      628 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/response/oa_response_unavailable.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.380661 ora2-5.0.1/openassessment/templates/openassessmentblock/self/
+-rw-r--r--   0 runner    (1001) docker     (122)     4593 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/self/oa_self_assessment.html
+-rw-r--r--   0 runner    (1001) docker     (122)      752 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/self/oa_self_cancelled.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1503 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/self/oa_self_closed.html
+-rw-r--r--   0 runner    (1001) docker     (122)      730 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/self/oa_self_complete.html
+-rw-r--r--   0 runner    (1001) docker     (122)      676 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/self/oa_self_unavailable.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.380661 ora2-5.0.1/openassessment/templates/openassessmentblock/staff/
+-rw-r--r--   0 runner    (1001) docker     (122)     1707 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/staff/oa_staff_grade.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.380661 ora2-5.0.1/openassessment/templates/openassessmentblock/staff_area/
+-rw-r--r--   0 runner    (1001) docker     (122)     8449 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html
+-rw-r--r--   0 runner    (1001) docker     (122)      887 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3927 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html
+-rw-r--r--   0 runner    (1001) docker     (122)      407 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_count.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3167 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/staff_area/oa_staff_override_assessment.html
+-rw-r--r--   0 runner    (1001) docker     (122)    16404 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/staff_area/oa_student_info.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3732 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.380661 ora2-5.0.1/openassessment/templates/openassessmentblock/student_training/
+-rw-r--r--   0 runner    (1001) docker     (122)    11281 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/student_training/student_training.html
+-rw-r--r--   0 runner    (1001) docker     (122)      652 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/student_training/student_training_cancelled.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/student_training/student_training_closed.html
+-rw-r--r--   0 runner    (1001) docker     (122)      653 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/student_training/student_training_complete.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1137 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/student_training/student_training_error.html
+-rw-r--r--   0 runner    (1001) docker     (122)      599 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templates/openassessmentblock/student_training/student_training_unavailable.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.384661 ora2-5.0.1/openassessment/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      886 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/templatetags/oa_extras.py
+-rw-r--r--   0 runner    (1001) docker     (122)      758 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.384661 ora2-5.0.1/openassessment/workflow/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1533 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/workflow/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19932 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/workflow/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1589 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/workflow/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.384661 ora2-5.0.1/openassessment/workflow/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     3111 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/workflow/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)      383 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/workflow/migrations/0002_remove_django_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      826 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/workflow/migrations/0003_TeamWorkflows.py
+-rw-r--r--   0 runner    (1001) docker     (122)      412 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/workflow/migrations/0004_assessmentworkflowstep_skipped.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/workflow/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    44741 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/workflow/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1660 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/workflow/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8350 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/workflow/team_api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.392661 ora2-5.0.1/openassessment/xblock/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/xblock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5880 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/xblock/config_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)      914 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/xblock/course_items_listing_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7889 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/xblock/data_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6829 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/xblock/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (122)      622 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/xblock/editor_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30777 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/xblock/grade_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5837 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/xblock/leaderboard_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3827 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/xblock/lms_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1808 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/xblock/load_static.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9846 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/xblock/message_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)      770 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/xblock/mobile.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3708 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/xblock/openassesment_template_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    51017 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/xblock/openassessmentblock.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14943 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/xblock/peer_assessment_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10329 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/xblock/resolve_dates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4560 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/xblock/rubric_reuse_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5369 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/xblock/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7825 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/xblock/self_assessment_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34259 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/xblock/staff_area_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9317 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/xblock/staff_assessment_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.304660 ora2-5.0.1/openassessment/xblock/static/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.304660 ora2-5.0.1/openassessment/xblock/static/css/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.304660 ora2-5.0.1/openassessment/xblock/static/css/lib/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.392661 ora2-5.0.1/openassessment/xblock/static/css/lib/backgrid/
+-rw-r--r--   0 runner    (1001) docker     (122)     5382 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/xblock/static/css/lib/backgrid/backgrid.css
+-rw-r--r--   0 runner    (1001) docker     (122)     4414 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/xblock/static/css/lib/backgrid/backgrid.min.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.440661 ora2-5.0.1/openassessment/xblock/static/dist/
+-rw-r--r--   0 runner    (1001) docker     (122)     1617 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/xblock/static/dist/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1834 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/xblock/static/dist/openassessment-editor-textarea.2774cf3b7c8fadda4341.js
+-rw-r--r--   0 runner    (1001) docker     (122)    38550 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/xblock/static/dist/openassessment-editor-textarea.js
+-rw-r--r--   0 runner    (1001) docker     (122)     2973 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/xblock/static/dist/openassessment-editor-tinymce.6a6113da3309f666ccda.js
+-rw-r--r--   0 runner    (1001) docker     (122)    47578 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/xblock/static/dist/openassessment-editor-tinymce.js
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/xblock/static/dist/openassessment-lms.7c3203918ed22728dd89.css
+-rw-r--r--   0 runner    (1001) docker     (122)  1319515 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/xblock/static/dist/openassessment-lms.7c3203918ed22728dd89.js
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-25 19:16:34.000000 ora2-5.0.1/openassessment/xblock/static/dist/openassessment-lms.css
+-rw-r--r--   0 runner    (1001) docker     (122) 28594064 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/static/dist/openassessment-lms.js
+-rw-r--r--   0 runner    (1001) docker     (122)   753258 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/static/dist/openassessment-ltr.cc6fb8c044bfe2899cd5.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1007 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/static/dist/openassessment-ltr.cc6fb8c044bfe2899cd5.js
+-rw-r--r--   0 runner    (1001) docker     (122)   846937 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/static/dist/openassessment-ltr.css
+-rw-r--r--   0 runner    (1001) docker     (122)    32672 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/static/dist/openassessment-ltr.js
+-rw-r--r--   0 runner    (1001) docker     (122)   753287 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/static/dist/openassessment-rtl.55343890f44133115ca3.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1007 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/static/dist/openassessment-rtl.55343890f44133115ca3.js
+-rw-r--r--   0 runner    (1001) docker     (122)   846966 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/static/dist/openassessment-rtl.css
+-rw-r--r--   0 runner    (1001) docker     (122)    32672 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/static/dist/openassessment-rtl.js
+-rw-r--r--   0 runner    (1001) docker     (122)   235846 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/static/dist/openassessment-studio.6fd5da4c0a2e58a8aba2.js
+-rw-r--r--   0 runner    (1001) docker     (122)  2305380 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/static/dist/openassessment-studio.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.304660 ora2-5.0.1/openassessment/xblock/static/js/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.304660 ora2-5.0.1/openassessment/xblock/static/js/lib/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.444661 ora2-5.0.1/openassessment/xblock/static/js/lib/backgrid/
+-rw-r--r--   0 runner    (1001) docker     (122)    87583 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/static/js/lib/backgrid/backgrid.js
+-rw-r--r--   0 runner    (1001) docker     (122)    26169 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/static/js/lib/backgrid/backgrid.min.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.444661 ora2-5.0.1/openassessment/xblock/static/js/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.444661 ora2-5.0.1/openassessment/xblock/static/js/src/lms/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.444661 ora2-5.0.1/openassessment/xblock/static/js/src/lms/api/
+-rw-r--r--   0 runner    (1001) docker     (122)      817 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/static/js/src/lms/api/waiting_step_details.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.448661 ora2-5.0.1/openassessment/xblock/static/js/src/lms/editors/
+-rw-r--r--   0 runner    (1001) docker     (122)     1368 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/static/js/src/lms/editors/oa_editor_textarea.js
+-rw-r--r--   0 runner    (1001) docker     (122)     3741 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/static/js/src/lms/editors/oa_editor_tinymce.js
+-rw-r--r--   0 runner    (1001) docker     (122)    18084 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/static/js/src/lms/oa_base.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1878 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/static/js/src/lms/oa_confirmation_alert.js
+-rw-r--r--   0 runner    (1001) docker     (122)    10567 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/static/js/src/lms/oa_course_items_listing.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1994 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/static/js/src/lms/oa_datefactory.js
+-rw-r--r--   0 runner    (1001) docker     (122)     2013 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/static/js/src/lms/oa_file_upload.js
+-rw-r--r--   0 runner    (1001) docker     (122)     8877 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/static/js/src/lms/oa_grade.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1873 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/static/js/src/lms/oa_leaderboard.js
+-rw-r--r--   0 runner    (1001) docker     (122)      910 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/static/js/src/lms/oa_message.js
+-rw-r--r--   0 runner    (1001) docker     (122)     9796 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/static/js/src/lms/oa_peer.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1882 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/static/js/src/lms/oa_prompts.js
+-rw-r--r--   0 runner    (1001) docker     (122)    32621 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/static/js/src/lms/oa_response.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1860 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/static/js/src/lms/oa_response_editor.js
+-rw-r--r--   0 runner    (1001) docker     (122)     7024 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/static/js/src/lms/oa_rubric.js
+-rw-r--r--   0 runner    (1001) docker     (122)     5344 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/static/js/src/lms/oa_self.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1351 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/static/js/src/lms/oa_staff.js
+-rw-r--r--   0 runner    (1001) docker     (122)    24786 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/static/js/src/lms/oa_staff_area.js
+-rw-r--r--   0 runner    (1001) docker     (122)     5267 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/static/js/src/lms/oa_training.js
+-rw-r--r--   0 runner    (1001) docker     (122)      400 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/static/js/src/lms_index.js
+-rw-r--r--   0 runner    (1001) docker     (122)    26166 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/static/js/src/oa_server.js
+-rw-r--r--   0 runner    (1001) docker     (122)      963 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/static/js/src/oa_shared.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.448661 ora2-5.0.1/openassessment/xblock/static/js/src/studio/
+-rw-r--r--   0 runner    (1001) docker     (122)     7705 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/static/js/src/studio/oa_container.js
+-rw-r--r--   0 runner    (1001) docker     (122)    20684 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/static/js/src/studio/oa_container_item.js
+-rw-r--r--   0 runner    (1001) docker     (122)    12727 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/static/js/src/studio/oa_edit.js
+-rw-r--r--   0 runner    (1001) docker     (122)    15956 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/static/js/src/studio/oa_edit_assessment.js
+-rw-r--r--   0 runner    (1001) docker     (122)     6121 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/static/js/src/studio/oa_edit_assessments_steps.js
+-rw-r--r--   0 runner    (1001) docker     (122)    11441 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/static/js/src/studio/oa_edit_fields.js
+-rw-r--r--   0 runner    (1001) docker     (122)    13033 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/static/js/src/studio/oa_edit_listeners.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1282 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/static/js/src/studio/oa_edit_notifier.js
+-rw-r--r--   0 runner    (1001) docker     (122)     3277 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/static/js/src/studio/oa_edit_prompts.js
+-rw-r--r--   0 runner    (1001) docker     (122)    13149 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/static/js/src/studio/oa_edit_rubric.js
+-rw-r--r--   0 runner    (1001) docker     (122)     4349 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/static/js/src/studio/oa_edit_schedule.js
+-rw-r--r--   0 runner    (1001) docker     (122)    15272 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/static/js/src/studio/oa_edit_settings.js
+-rw-r--r--   0 runner    (1001) docker     (122)     3746 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/static/js/src/studio/oa_edit_validation_alert.js
+-rw-r--r--   0 runner    (1001) docker     (122)     2654 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/static/js/src/studio/oa_tiny_mce.js
+-rw-r--r--   0 runner    (1001) docker     (122)      133 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/static/js/src/studio_index.js
+-rw-r--r--   0 runner    (1001) docker     (122)    11859 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/student_training_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20538 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/studio_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    42012 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/submission_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8743 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/team_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4631 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/team_workflow_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)      675 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/user_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15746 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/validation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8409 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/workflow_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35842 2023-05-25 19:16:35.000000 ora2-5.0.1/openassessment/xblock/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.448661 ora2-5.0.1/ora2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2643 2023-05-25 19:16:40.000000 ora2-5.0.1/ora2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    23039 2023-05-25 19:16:40.000000 ora2-5.0.1/ora2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-25 19:16:40.000000 ora2-5.0.1/ora2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-05-25 19:16:40.000000 ora2-5.0.1/ora2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      289 2023-05-25 19:16:40.000000 ora2-5.0.1/ora2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-05-25 19:16:40.000000 ora2-5.0.1/ora2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 19:16:40.452661 ora2-5.0.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      413 2023-05-25 19:16:35.000000 ora2-5.0.1/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)       40 2023-05-25 19:16:35.000000 ora2-5.0.1/requirements/ci.in
+-rw-r--r--   0 runner    (1001) docker     (122)      179 2023-05-25 19:16:35.000000 ora2-5.0.1/requirements/pip-tools.in
+-rw-r--r--   0 runner    (1001) docker     (122)       91 2023-05-25 19:16:35.000000 ora2-5.0.1/requirements/pip.in
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-05-25 19:16:35.000000 ora2-5.0.1/requirements/quality.in
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-05-25 19:16:35.000000 ora2-5.0.1/requirements/test-acceptance.in
+-rw-r--r--   0 runner    (1001) docker     (122)      685 2023-05-25 19:16:35.000000 ora2-5.0.1/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-05-25 19:16:35.000000 ora2-5.0.1/requirements/tox.in
+-rw-r--r--   0 runner    (1001) docker     (122)      318 2023-05-25 19:16:40.452661 ora2-5.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2593 2023-05-25 19:16:35.000000 ora2-5.0.1/setup.py
```

### Comparing `ora2-5.0.0/LICENSE` & `ora2-5.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/MANIFEST.in` & `ora2-5.0.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/PKG-INFO` & `ora2-5.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ora2
-Version: 5.0.0
+Version: 5.0.1
 Summary: edx-ora2
 Home-page: http://github.com/openedx/edx-ora2
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ora2-5.0.0/README.rst` & `ora2-5.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/assessment/admin.py` & `ora2-5.0.1/openassessment/assessment/admin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/assessment/api/peer.py` & `ora2-5.0.1/openassessment/assessment/api/peer.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/assessment/api/self.py` & `ora2-5.0.1/openassessment/assessment/api/self.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/assessment/api/staff.py` & `ora2-5.0.1/openassessment/assessment/api/staff.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/assessment/api/student_training.py` & `ora2-5.0.1/openassessment/assessment/api/student_training.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/assessment/api/teams.py` & `ora2-5.0.1/openassessment/assessment/api/teams.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/assessment/errors/peer.py` & `ora2-5.0.1/openassessment/assessment/errors/peer.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/assessment/errors/self.py` & `ora2-5.0.1/openassessment/assessment/errors/self.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/assessment/errors/staff.py` & `ora2-5.0.1/openassessment/assessment/errors/staff.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/assessment/migrations/0001_initial.py` & `ora2-5.0.1/openassessment/assessment/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/assessment/migrations/0002_staffworkflow.py` & `ora2-5.0.1/openassessment/assessment/migrations/0002_staffworkflow.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/assessment/migrations/0003_expand_course_id.py` & `ora2-5.0.1/openassessment/assessment/migrations/0003_expand_course_id.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/assessment/migrations/0004_historicalsharedfileupload_sharedfileupload.py` & `ora2-5.0.1/openassessment/assessment/migrations/0004_historicalsharedfileupload_sharedfileupload.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/assessment/migrations/0005_add_filename_to_sharedupload.py` & `ora2-5.0.1/openassessment/assessment/migrations/0005_add_filename_to_sharedupload.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/assessment/migrations/0006_TeamWorkflows.py` & `ora2-5.0.1/openassessment/assessment/migrations/0006_TeamWorkflows.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/assessment/migrations/0007_staff_workflow_blank.py` & `ora2-5.0.1/openassessment/assessment/migrations/0007_staff_workflow_blank.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/assessment/models/base.py` & `ora2-5.0.1/openassessment/assessment/models/base.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/assessment/models/peer.py` & `ora2-5.0.1/openassessment/assessment/models/peer.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/assessment/models/staff.py` & `ora2-5.0.1/openassessment/assessment/models/staff.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/assessment/models/student_training.py` & `ora2-5.0.1/openassessment/assessment/models/student_training.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/assessment/models/training.py` & `ora2-5.0.1/openassessment/assessment/models/training.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/assessment/serializers/base.py` & `ora2-5.0.1/openassessment/assessment/serializers/base.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/assessment/serializers/peer.py` & `ora2-5.0.1/openassessment/assessment/serializers/peer.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/assessment/serializers/training.py` & `ora2-5.0.1/openassessment/assessment/serializers/training.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/assessment/views.py` & `ora2-5.0.1/openassessment/assessment/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,20 +28,20 @@
 
     Returns:
         HttpResponse: The response object for this request. Renders a simple
             development page with all the evaluations related to the specified
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
         evaluations = []
         for submission in submissions:
             submission_evaluations = get_assessments(submission["uuid"])
             for evaluation in submission_evaluations:
                 evaluation["submission_uuid"] = submission["uuid"]
```

### Comparing `ora2-5.0.0/openassessment/data.py` & `ora2-5.0.1/openassessment/data.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/fileupload/api.py` & `ora2-5.0.1/openassessment/fileupload/api.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/fileupload/backends/__init__.py` & `ora2-5.0.1/openassessment/fileupload/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/fileupload/backends/base.py` & `ora2-5.0.1/openassessment/fileupload/backends/base.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/fileupload/backends/django_storage.py` & `ora2-5.0.1/openassessment/fileupload/backends/django_storage.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/fileupload/backends/filesystem.py` & `ora2-5.0.1/openassessment/fileupload/backends/filesystem.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/fileupload/backends/s3.py` & `ora2-5.0.1/openassessment/fileupload/backends/s3.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/fileupload/backends/swift.py` & `ora2-5.0.1/openassessment/fileupload/backends/swift.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/fileupload/exceptions.py` & `ora2-5.0.1/openassessment/fileupload/exceptions.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/fileupload/views_filesystem.py` & `ora2-5.0.1/openassessment/fileupload/views_filesystem.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/locale/ar/LC_MESSAGES/django.mo` & `ora2-5.0.1/openassessment/locale/ar/LC_MESSAGES/django.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
 "Last-Translator: Ghassan Maslamani <ghassan.maslamani@gmail.com>, 2022\n"
-"Language-Team: Arabic (http://www.transifex.com/open-edx/edx-platform/"
+"Language-Team: Arabic (http://app.transifex.com/open-edx/edx-platform/"
 "language/ar/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: ar\n"
 "Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 "
 "&& n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
@@ -967,14 +967,17 @@
 
 msgid "Feedback Instructions"
 msgstr "تعليمات الآراء والملاحظات "
 
 msgid "Feedback Recorded"
 msgstr "الملاحظة المسجلة"
 
+msgid "Feedback Statements Selected"
+msgstr "تم تحديد بيانات الملاحظات"
+
 msgid "Feedback for This Criterion"
 msgstr "آراء وملاحظات حول هذا المعيار"
 
 msgid "Feedback for This Response"
 msgstr "آراء وملاحظات حول هذا الرد"
 
 msgid "Feedback saved."
@@ -1010,14 +1013,20 @@
 
 msgid "Files that were uploaded by your teammates:"
 msgstr "الملفات التي تم رفعها بواسطة زملائك في الفريق"
 
 msgid "Final Grade Details"
 msgstr "تفاصيل الدرجة النهائية"
 
+msgid "Final Score Earned"
+msgstr "النتيجة النهائية المكتسبة"
+
+msgid "Final Score Possible"
+msgstr "النتيجة النهائية ممكنة"
+
 msgid "Give this learner a grade using the problem's rubric."
 msgstr "امنح المتعلّم درجة باستخدام سُلّم تقييم المسألة"
 
 msgid "Give this team a grade using the problem's rubric."
 msgstr "امنح الفريق درجة باستخدام سُلّم تقييم المسألة"
 
 msgid "Grade Available Responses"
@@ -1352,14 +1361,17 @@
 
 msgid "Response Due Date"
 msgstr "تاريخ استحقاق الردود"
 
 msgid "Response Due Time"
 msgstr "وقت استحقاق الردود"
 
+msgid "Response Editor"
+msgstr "محرر الاستجابة"
+
 msgid "Response Score"
 msgstr "درجات الرد"
 
 msgid "Response Start Date"
 msgstr "تاريخ بداية الردود"
 
 msgid "Response Start Time"
```

### Comparing `ora2-5.0.0/openassessment/locale/ar/LC_MESSAGES/django.po` & `ora2-5.0.1/openassessment/locale/ar/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -22,18 +22,18 @@
 # shefaa abu jabel <shefaa.aj@gmail.com>, 2016-2017
 # Soha Assali <soha+transifex@qordoba.com>, 2015-2016
 # Widad El Samman <widadsamman@gmail.com>, 2015
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-01-15 13:36-0500\n"
+"POT-Creation-Date: 2023-04-30 14:36-0400\n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
 "Last-Translator: Ghassan Maslamani <ghassan.maslamani@gmail.com>, 2022\n"
-"Language-Team: Arabic (http://www.transifex.com/open-edx/edx-platform/language/ar/)\n"
+"Language-Team: Arabic (http://app.transifex.com/open-edx/edx-platform/language/ar/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: ar\n"
 "Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 && n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
 
 #: openassessment/assessment/api/student_training.py:179
@@ -135,23 +135,23 @@
 
 #: openassessment/data.py:923
 msgid "Date/Time Final Score Given"
 msgstr ""
 
 #: openassessment/data.py:924
 msgid "Final Score Earned"
-msgstr ""
+msgstr "النتيجة النهائية المكتسبة"
 
 #: openassessment/data.py:925
 msgid "Final Score Possible"
-msgstr ""
+msgstr "النتيجة النهائية ممكنة"
 
 #: openassessment/data.py:926
 msgid "Feedback Statements Selected"
-msgstr ""
+msgstr "تم تحديد بيانات الملاحظات"
 
 #: openassessment/data.py:927
 msgid "Feedback on Assessment"
 msgstr ""
 
 #: openassessment/data.py:929
 msgid "Response Files"
@@ -193,15 +193,15 @@
 msgid ""
 "Specify whether learners must include a text based response to this "
 "problem's prompt."
 msgstr "حدد ما إذا كان يجب على المتعلمين إدراج إجابة نصية لهذه المسألة."
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:25
 msgid "Response Editor"
-msgstr ""
+msgstr "محرر الاستجابة"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:33
 msgid ""
 "Select which editor learners will use to include a text based response to "
 "this problem's prompt."
 msgstr ""
```

### Comparing `ora2-5.0.0/openassessment/locale/ar/LC_MESSAGES/djangojs.mo` & `ora2-5.0.1/openassessment/locale/ar/LC_MESSAGES/djangojs.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Ghassan Maslamani <ghassan.maslamani@gmail.com>, 2021\n"
-"Language-Team: Arabic (http://www.transifex.com/open-edx/edx-platform/"
+"Language-Team: Arabic (http://app.transifex.com/open-edx/edx-platform/"
 "language/ar/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: ar\n"
 "Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 "
 "&& n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
```

### Comparing `ora2-5.0.0/openassessment/locale/ar/LC_MESSAGES/djangojs.po` & `ora2-5.0.1/openassessment/locale/ar/LC_MESSAGES/djangojs.po`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-09-13 04:00-0400\n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Ghassan Maslamani <ghassan.maslamani@gmail.com>, 2021\n"
-"Language-Team: Arabic (http://www.transifex.com/open-edx/edx-platform/language/ar/)\n"
+"Language-Team: Arabic (http://app.transifex.com/open-edx/edx-platform/language/ar/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: ar\n"
 "Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 && n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
```

### Comparing `ora2-5.0.0/openassessment/locale/ar_SA/LC_MESSAGES/djangojs.mo` & `ora2-5.0.1/openassessment/locale/ar_SA/LC_MESSAGES/djangojs.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: NELC Open edX Translation <openedx@elc.edu.sa>, 2020\n"
-"Language-Team: Arabic (Saudi Arabia) (http://www.transifex.com/open-edx/edx-"
+"Language-Team: Arabic (Saudi Arabia) (http://app.transifex.com/open-edx/edx-"
 "platform/language/ar_SA/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: ar_SA\n"
 "Plural-Forms: nplurals=6; plural=(n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 "
 "&& n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5);\n"
```

### Comparing `ora2-5.0.0/openassessment/locale/ar_SA/LC_MESSAGES/djangojs.po` & `ora2-5.0.1/openassessment/locale/ar_SA/LC_MESSAGES/djangojs.po`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-09-13 04:00-0400\n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: NELC Open edX Translation <openedx@elc.edu.sa>, 2020\n"
-"Language-Team: Arabic (Saudi Arabia) (http://www.transifex.com/open-edx/edx-platform/language/ar_SA/)\n"
+"Language-Team: Arabic (Saudi Arabia) (http://app.transifex.com/open-edx/edx-platform/language/ar_SA/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: ar_SA\n"
 "Plural-Forms: nplurals=6; plural=(n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 && n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5);\n"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
```

### Comparing `ora2-5.0.0/openassessment/locale/de_DE/LC_MESSAGES/django.mo` & `ora2-5.0.1/openassessment/locale/de_DE/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,15 +1,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
 "Last-Translator: Stefania Trabucchi <stefania.trabucchi@abstract-technology."
 "de>, 2018-2021\n"
-"Language-Team: German (Germany) (http://www.transifex.com/open-edx/edx-"
+"Language-Team: German (Germany) (http://app.transifex.com/open-edx/edx-"
 "platform/language/de_DE/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: de_DE\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `ora2-5.0.0/openassessment/locale/de_DE/LC_MESSAGES/django.po` & `ora2-5.0.1/openassessment/locale/de_DE/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -26,18 +26,18 @@
 # Tobi, 2020
 # a44cc3e9393feb16b9a6b297471280a5_cf4574c <542714ce952f7f0fa8b5f6591bf1451e_216225>, 2014
 # Андрей Поляков <polyakov.andrey@gmail.com>, 2016
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-01-15 13:36-0500\n"
+"POT-Creation-Date: 2023-04-30 14:36-0400\n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
 "Last-Translator: Stefania Trabucchi <stefania.trabucchi@abstract-technology.de>, 2018-2021\n"
-"Language-Team: German (Germany) (http://www.transifex.com/open-edx/edx-platform/language/de_DE/)\n"
+"Language-Team: German (Germany) (http://app.transifex.com/open-edx/edx-platform/language/de_DE/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: de_DE\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: openassessment/assessment/api/student_training.py:179
```

### Comparing `ora2-5.0.0/openassessment/locale/de_DE/LC_MESSAGES/djangojs.mo` & `ora2-5.0.1/openassessment/locale/de_DE/LC_MESSAGES/djangojs.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,15 +1,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Stefania Trabucchi <stefania.trabucchi@abstract-technology."
 "de>, 2020-2021\n"
-"Language-Team: German (Germany) (http://www.transifex.com/open-edx/edx-"
+"Language-Team: German (Germany) (http://app.transifex.com/open-edx/edx-"
 "platform/language/de_DE/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: de_DE\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `ora2-5.0.0/openassessment/locale/de_DE/LC_MESSAGES/djangojs.po` & `ora2-5.0.1/openassessment/locale/de_DE/LC_MESSAGES/djangojs.po`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-09-13 04:00-0400\n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Stefania Trabucchi <stefania.trabucchi@abstract-technology.de>, 2020-2021\n"
-"Language-Team: German (Germany) (http://www.transifex.com/open-edx/edx-platform/language/de_DE/)\n"
+"Language-Team: German (Germany) (http://app.transifex.com/open-edx/edx-platform/language/de_DE/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: de_DE\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
```

### Comparing `ora2-5.0.0/openassessment/locale/el/LC_MESSAGES/django.mo` & `ora2-5.0.1/openassessment/locale/el/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
 "Last-Translator: Eirini Mageiropoulou <eirmageir@yahoo.com>, 2021\n"
-"Language-Team: Greek (http://www.transifex.com/open-edx/edx-platform/"
+"Language-Team: Greek (http://app.transifex.com/open-edx/edx-platform/"
 "language/el/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: el\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `ora2-5.0.0/openassessment/locale/el/LC_MESSAGES/django.po` & `ora2-5.0.1/openassessment/locale/el/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 # SYMI PASALIDOU <simipass@hotmail.com>, 2016
 # Vassia Kouremenou <Vassiacat@hotmail.com>, 2016
 # yiannis voz <yiannisvozikis@gmail.com>, 2016
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-01-15 13:36-0500\n"
+"POT-Creation-Date: 2023-04-30 14:36-0400\n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
 "Last-Translator: Eirini Mageiropoulou <eirmageir@yahoo.com>, 2021\n"
-"Language-Team: Greek (http://www.transifex.com/open-edx/edx-platform/language/el/)\n"
+"Language-Team: Greek (http://app.transifex.com/open-edx/edx-platform/language/el/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: el\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: openassessment/assessment/api/student_training.py:179
```

### Comparing `ora2-5.0.0/openassessment/locale/el/LC_MESSAGES/djangojs.mo` & `ora2-5.0.1/openassessment/locale/el/LC_MESSAGES/djangojs.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Eirini Mageiropoulou <eirmageir@yahoo.com>, 2021\n"
-"Language-Team: Greek (http://www.transifex.com/open-edx/edx-platform/"
+"Language-Team: Greek (http://app.transifex.com/open-edx/edx-platform/"
 "language/el/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: el\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `ora2-5.0.0/openassessment/locale/el/LC_MESSAGES/djangojs.po` & `ora2-5.0.1/openassessment/locale/el/LC_MESSAGES/djangojs.po`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-09-13 04:00-0400\n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Eirini Mageiropoulou <eirmageir@yahoo.com>, 2021\n"
-"Language-Team: Greek (http://www.transifex.com/open-edx/edx-platform/language/el/)\n"
+"Language-Team: Greek (http://app.transifex.com/open-edx/edx-platform/language/el/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: el\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
```

### Comparing `ora2-5.0.0/openassessment/locale/en/LC_MESSAGES/django.po` & `ora2-5.0.1/openassessment/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/locale/en/LC_MESSAGES/djangojs.po` & `ora2-5.0.1/openassessment/locale/en/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/locale/eo/LC_MESSAGES/django.mo` & `ora2-5.0.1/openassessment/locale/eo/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/locale/eo/LC_MESSAGES/django.po` & `ora2-5.0.1/openassessment/locale/eo/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/locale/eo/LC_MESSAGES/djangojs.mo` & `ora2-5.0.1/openassessment/locale/eo/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/locale/eo/LC_MESSAGES/djangojs.po` & `ora2-5.0.1/openassessment/locale/eo/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/locale/es_419/LC_MESSAGES/django.mo` & `ora2-5.0.1/openassessment/locale/es_419/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
 "Last-Translator: Jesica Greco, 2022\n"
-"Language-Team: Spanish (Latin America) (http://www.transifex.com/open-edx/"
+"Language-Team: Spanish (Latin America) (http://app.transifex.com/open-edx/"
 "edx-platform/language/es_419/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: es_419\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? "
 "1 : 2;\n"
```

### Comparing `ora2-5.0.0/openassessment/locale/es_419/LC_MESSAGES/django.po` & `ora2-5.0.1/openassessment/locale/es_419/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -30,18 +30,18 @@
 # Ned Weitzman <nweitzman@edx.org>, 2016-2017
 # rovim <rosauravidal@gmail.com>, 2014
 # UAbierta Universidad de Chile <uabierta@u.uchile.cl>, 2015
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-01-29 13:36-0500\n"
+"POT-Creation-Date: 2023-04-23 14:36-0400\n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
 "Last-Translator: Jesica Greco, 2022\n"
-"Language-Team: Spanish (Latin America) (http://www.transifex.com/open-edx/edx-platform/language/es_419/)\n"
+"Language-Team: Spanish (Latin America) (http://app.transifex.com/open-edx/edx-platform/language/es_419/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: es_419\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 
 #: openassessment/assessment/api/student_training.py:179
```

### Comparing `ora2-5.0.0/openassessment/locale/es_419/LC_MESSAGES/djangojs.mo` & `ora2-5.0.1/openassessment/locale/es_419/LC_MESSAGES/djangojs.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Carolina De Mares <carolina.demares@edunext.co>, 2021\n"
-"Language-Team: Spanish (Latin America) (http://www.transifex.com/open-edx/"
+"Language-Team: Spanish (Latin America) (http://app.transifex.com/open-edx/"
 "edx-platform/language/es_419/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: es_419\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? "
 "1 : 2;\n"
```

### Comparing `ora2-5.0.0/openassessment/locale/es_419/LC_MESSAGES/djangojs.po` & `ora2-5.0.1/openassessment/locale/es_419/LC_MESSAGES/djangojs.po`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-09-13 04:00-0400\n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Carolina De Mares <carolina.demares@edunext.co>, 2021\n"
-"Language-Team: Spanish (Latin America) (http://www.transifex.com/open-edx/edx-platform/language/es_419/)\n"
+"Language-Team: Spanish (Latin America) (http://app.transifex.com/open-edx/edx-platform/language/es_419/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: es_419\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
```

### Comparing `ora2-5.0.0/openassessment/locale/es_AR/LC_MESSAGES/djangojs.mo` & `ora2-5.0.1/openassessment/locale/es_AR/LC_MESSAGES/djangojs.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Jesica Greco, 2023\n"
-"Language-Team: Spanish (Argentina) (http://www.transifex.com/open-edx/edx-"
+"Language-Team: Spanish (Argentina) (http://app.transifex.com/open-edx/edx-"
 "platform/language/es_AR/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: es_AR\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? "
 "1 : 2;\n"
```

### Comparing `ora2-5.0.0/openassessment/locale/es_AR/LC_MESSAGES/djangojs.po` & `ora2-5.0.1/openassessment/locale/es_AR/LC_MESSAGES/djangojs.po`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-09-13 04:00-0400\n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Jesica Greco, 2023\n"
-"Language-Team: Spanish (Argentina) (http://www.transifex.com/open-edx/edx-platform/language/es_AR/)\n"
+"Language-Team: Spanish (Argentina) (http://app.transifex.com/open-edx/edx-platform/language/es_AR/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: es_AR\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
```

### Comparing `ora2-5.0.0/openassessment/locale/es_ES/LC_MESSAGES/django.mo` & `ora2-5.0.1/openassessment/locale/es_ES/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
 "Last-Translator: Jesica Greco, 2022-2023\n"
-"Language-Team: Spanish (Spain) (http://www.transifex.com/open-edx/edx-"
+"Language-Team: Spanish (Spain) (http://app.transifex.com/open-edx/edx-"
 "platform/language/es_ES/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: es_ES\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? "
 "1 : 2;\n"
```

### Comparing `ora2-5.0.0/openassessment/locale/es_ES/LC_MESSAGES/django.po` & `ora2-5.0.1/openassessment/locale/es_ES/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -23,18 +23,18 @@
 # Sarina Canelake <sarina@tcril.org>, 2014
 # Stefania Trabucchi <stefania.trabucchi@abstract-technology.de>, 2018
 # UAMx <uamx.dev@gmail.com>, 2021-2022
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-01-29 13:36-0500\n"
+"POT-Creation-Date: 2023-04-23 14:36-0400\n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
 "Last-Translator: Jesica Greco, 2022-2023\n"
-"Language-Team: Spanish (Spain) (http://www.transifex.com/open-edx/edx-platform/language/es_ES/)\n"
+"Language-Team: Spanish (Spain) (http://app.transifex.com/open-edx/edx-platform/language/es_ES/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: es_ES\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 
 #: openassessment/assessment/api/student_training.py:179
```

### Comparing `ora2-5.0.0/openassessment/locale/es_ES/LC_MESSAGES/djangojs.mo` & `ora2-5.0.1/openassessment/locale/es_ES/LC_MESSAGES/djangojs.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Jesica Greco, 2022\n"
-"Language-Team: Spanish (Spain) (http://www.transifex.com/open-edx/edx-"
+"Language-Team: Spanish (Spain) (http://app.transifex.com/open-edx/edx-"
 "platform/language/es_ES/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: es_ES\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? "
 "1 : 2;\n"
```

### Comparing `ora2-5.0.0/openassessment/locale/es_ES/LC_MESSAGES/djangojs.po` & `ora2-5.0.1/openassessment/locale/es_ES/LC_MESSAGES/djangojs.po`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-09-13 04:00-0400\n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Jesica Greco, 2022\n"
-"Language-Team: Spanish (Spain) (http://www.transifex.com/open-edx/edx-platform/language/es_ES/)\n"
+"Language-Team: Spanish (Spain) (http://app.transifex.com/open-edx/edx-platform/language/es_ES/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: es_ES\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
```

### Comparing `ora2-5.0.0/openassessment/locale/eu_ES/LC_MESSAGES/django.mo` & `ora2-5.0.1/openassessment/locale/eu_ES/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
 "Last-Translator: Abel Camacho <abelcama@gmail.com>, 2019-2020\n"
-"Language-Team: Basque (Spain) (http://www.transifex.com/open-edx/edx-"
+"Language-Team: Basque (Spain) (http://app.transifex.com/open-edx/edx-"
 "platform/language/eu_ES/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: eu_ES\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `ora2-5.0.0/openassessment/locale/eu_ES/LC_MESSAGES/django.po` & `ora2-5.0.1/openassessment/locale/eu_ES/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 # Abel Camacho <abelcama@gmail.com>, 2019-2020
 # Abel Camacho <abelcama@gmail.com>, 2015
 # Pedro Lonbide <plonbide@gmail.com>, 2015
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-01-15 13:36-0500\n"
+"POT-Creation-Date: 2023-04-30 14:36-0400\n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
 "Last-Translator: Abel Camacho <abelcama@gmail.com>, 2019-2020\n"
-"Language-Team: Basque (Spain) (http://www.transifex.com/open-edx/edx-platform/language/eu_ES/)\n"
+"Language-Team: Basque (Spain) (http://app.transifex.com/open-edx/edx-platform/language/eu_ES/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: eu_ES\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: openassessment/assessment/api/student_training.py:179
```

### Comparing `ora2-5.0.0/openassessment/locale/eu_ES/LC_MESSAGES/djangojs.mo` & `ora2-5.0.1/openassessment/locale/eu_ES/LC_MESSAGES/djangojs.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Abel Camacho <abelcama@gmail.com>, 2017,2019-2020\n"
-"Language-Team: Basque (Spain) (http://www.transifex.com/open-edx/edx-"
+"Language-Team: Basque (Spain) (http://app.transifex.com/open-edx/edx-"
 "platform/language/eu_ES/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: eu_ES\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `ora2-5.0.0/openassessment/locale/eu_ES/LC_MESSAGES/djangojs.po` & `ora2-5.0.1/openassessment/locale/eu_ES/LC_MESSAGES/djangojs.po`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-09-13 04:00-0400\n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Abel Camacho <abelcama@gmail.com>, 2017,2019-2020\n"
-"Language-Team: Basque (Spain) (http://www.transifex.com/open-edx/edx-platform/language/eu_ES/)\n"
+"Language-Team: Basque (Spain) (http://app.transifex.com/open-edx/edx-platform/language/eu_ES/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: eu_ES\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
```

### Comparing `ora2-5.0.0/openassessment/locale/fa_IR/LC_MESSAGES/django.mo` & `ora2-5.0.1/openassessment/locale/fa_IR/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
 "Last-Translator: Somaye Joolaee, 2022\n"
-"Language-Team: Persian (Iran) (http://www.transifex.com/open-edx/edx-"
+"Language-Team: Persian (Iran) (http://app.transifex.com/open-edx/edx-"
 "platform/language/fa_IR/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: fa_IR\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
```

### Comparing `ora2-5.0.0/openassessment/locale/fa_IR/LC_MESSAGES/django.po` & `ora2-5.0.1/openassessment/locale/fa_IR/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 # Siavash Kavousi <siavash.kavousi.sk@gmail.com>, 2016
 # Sina Shirinpour <sshirinpoor@gmail.com>, 2015
 # Somaye Joolaee, 2022
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-01-15 13:36-0500\n"
+"POT-Creation-Date: 2023-04-30 14:36-0400\n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
 "Last-Translator: Somaye Joolaee, 2022\n"
-"Language-Team: Persian (Iran) (http://www.transifex.com/open-edx/edx-platform/language/fa_IR/)\n"
+"Language-Team: Persian (Iran) (http://app.transifex.com/open-edx/edx-platform/language/fa_IR/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: fa_IR\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
 #: openassessment/assessment/api/student_training.py:179
```

### Comparing `ora2-5.0.0/openassessment/locale/fa_IR/LC_MESSAGES/djangojs.mo` & `ora2-5.0.1/openassessment/locale/fa_IR/LC_MESSAGES/djangojs.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Somaye Joolaee, 2022\n"
-"Language-Team: Persian (Iran) (http://www.transifex.com/open-edx/edx-"
+"Language-Team: Persian (Iran) (http://app.transifex.com/open-edx/edx-"
 "platform/language/fa_IR/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: fa_IR\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
```

### Comparing `ora2-5.0.0/openassessment/locale/fa_IR/LC_MESSAGES/djangojs.po` & `ora2-5.0.1/openassessment/locale/fa_IR/LC_MESSAGES/djangojs.po`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-09-13 04:00-0400\n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Somaye Joolaee, 2022\n"
-"Language-Team: Persian (Iran) (http://www.transifex.com/open-edx/edx-platform/language/fa_IR/)\n"
+"Language-Team: Persian (Iran) (http://app.transifex.com/open-edx/edx-platform/language/fa_IR/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: fa_IR\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
```

### Comparing `ora2-5.0.0/openassessment/locale/fr/LC_MESSAGES/django.mo` & `ora2-5.0.1/openassessment/locale/fr/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
 "Last-Translator: alexis swyngedauw, 2022\n"
-"Language-Team: French (http://www.transifex.com/open-edx/edx-platform/"
+"Language-Team: French (http://app.transifex.com/open-edx/edx-platform/"
 "language/fr/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: fr\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
 "1000000 == 0 ? 1 : 2;\n"
```

### Comparing `ora2-5.0.0/openassessment/locale/fr/LC_MESSAGES/django.po` & `ora2-5.0.1/openassessment/locale/fr/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -40,18 +40,18 @@
 # willyedoo <willyedoo@gmail.com>, 2019
 # d6910e756eb8532754192e6021dc9f83, 2014
 # d6910e756eb8532754192e6021dc9f83, 2014
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-01-15 13:36-0500\n"
+"POT-Creation-Date: 2023-04-30 14:36-0400\n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
 "Last-Translator: alexis swyngedauw, 2022\n"
-"Language-Team: French (http://www.transifex.com/open-edx/edx-platform/language/fr/)\n"
+"Language-Team: French (http://app.transifex.com/open-edx/edx-platform/language/fr/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: fr\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 
 #: openassessment/assessment/api/student_training.py:179
```

### Comparing `ora2-5.0.0/openassessment/locale/fr/LC_MESSAGES/djangojs.mo` & `ora2-5.0.1/openassessment/locale/fr/LC_MESSAGES/djangojs.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: iderr <ibrahim@derraz.fr>, 2021-2022\n"
-"Language-Team: French (http://www.transifex.com/open-edx/edx-platform/"
+"Language-Team: French (http://app.transifex.com/open-edx/edx-platform/"
 "language/fr/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: fr\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
 "1000000 == 0 ? 1 : 2;\n"
```

### Comparing `ora2-5.0.0/openassessment/locale/fr/LC_MESSAGES/djangojs.po` & `ora2-5.0.1/openassessment/locale/fr/LC_MESSAGES/djangojs.po`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-09-13 04:00-0400\n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: iderr <ibrahim@derraz.fr>, 2021-2022\n"
-"Language-Team: French (http://www.transifex.com/open-edx/edx-platform/language/fr/)\n"
+"Language-Team: French (http://app.transifex.com/open-edx/edx-platform/language/fr/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: fr\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
```

### Comparing `ora2-5.0.0/openassessment/locale/fr_CA/LC_MESSAGES/django.mo` & `ora2-5.0.1/openassessment/locale/fr_CA/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
 "Last-Translator: Pierre Mailhot <pierre.mailhot@gmail.com>, 2016-2023\n"
-"Language-Team: French (Canada) (http://www.transifex.com/open-edx/edx-"
+"Language-Team: French (Canada) (http://app.transifex.com/open-edx/edx-"
 "platform/language/fr_CA/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: fr_CA\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
 "1000000 == 0 ? 1 : 2;\n"
```

### Comparing `ora2-5.0.0/openassessment/locale/fr_CA/LC_MESSAGES/django.po` & `ora2-5.0.1/openassessment/locale/fr_CA/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -93,18 +93,18 @@
 # d6910e756eb8532754192e6021dc9f83, 2014-2015
 # ytabaa <ytabaa@uae.ac.ma>, 2014
 # Андрей Поляков <polyakov.andrey@gmail.com>, 2016
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-01-22 13:36-0500\n"
+"POT-Creation-Date: 2023-04-16 14:36-0400\n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
 "Last-Translator: Pierre Mailhot <pierre.mailhot@gmail.com>, 2016-2023\n"
-"Language-Team: French (Canada) (http://www.transifex.com/open-edx/edx-platform/language/fr_CA/)\n"
+"Language-Team: French (Canada) (http://app.transifex.com/open-edx/edx-platform/language/fr_CA/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: fr_CA\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 
 #: openassessment/assessment/api/student_training.py:179
```

### Comparing `ora2-5.0.0/openassessment/locale/fr_CA/LC_MESSAGES/djangojs.mo` & `ora2-5.0.1/openassessment/locale/fr_CA/LC_MESSAGES/djangojs.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Pierre Mailhot <pierre.mailhot@gmail.com>, 2016,2018-2023\n"
-"Language-Team: French (Canada) (http://www.transifex.com/open-edx/edx-"
+"Language-Team: French (Canada) (http://app.transifex.com/open-edx/edx-"
 "platform/language/fr_CA/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: fr_CA\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
 "1000000 == 0 ? 1 : 2;\n"
```

### Comparing `ora2-5.0.0/openassessment/locale/fr_CA/LC_MESSAGES/djangojs.po` & `ora2-5.0.1/openassessment/locale/fr_CA/LC_MESSAGES/djangojs.po`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-09-13 04:00-0400\n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Pierre Mailhot <pierre.mailhot@gmail.com>, 2016,2018-2023\n"
-"Language-Team: French (Canada) (http://www.transifex.com/open-edx/edx-platform/language/fr_CA/)\n"
+"Language-Team: French (Canada) (http://app.transifex.com/open-edx/edx-platform/language/fr_CA/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: fr_CA\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
```

### Comparing `ora2-5.0.0/openassessment/locale/he/LC_MESSAGES/django.mo` & `ora2-5.0.1/openassessment/locale/he/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
 "Last-Translator: Hodaya Zada <hodayaz@mse.gov.il>, 2019,2021\n"
-"Language-Team: Hebrew (http://www.transifex.com/open-edx/edx-platform/"
+"Language-Team: Hebrew (http://app.transifex.com/open-edx/edx-platform/"
 "language/he/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: he\n"
 "Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n == 2 && n % "
 "1 == 0) ? 1: (n % 10 == 0 && n % 1 == 0 && n > 10) ? 2 : 3;\n"
```

### Comparing `ora2-5.0.0/openassessment/locale/he/LC_MESSAGES/django.po` & `ora2-5.0.1/openassessment/locale/he/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # qualityalltext <quality@alltext.co.il>, 2016-2017
 # Ron Rozen <Ronrozen@gmail.com>, 2016
 # Yoav Caspin <yoavc@pmo.gov.il>, 2016-2017
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-01-15 13:36-0500\n"
+"POT-Creation-Date: 2023-04-30 14:36-0400\n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
 "Last-Translator: Hodaya Zada <hodayaz@mse.gov.il>, 2019,2021\n"
-"Language-Team: Hebrew (http://www.transifex.com/open-edx/edx-platform/language/he/)\n"
+"Language-Team: Hebrew (http://app.transifex.com/open-edx/edx-platform/language/he/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: he\n"
 "Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n == 2 && n % 1 == 0) ? 1: (n % 10 == 0 && n % 1 == 0 && n > 10) ? 2 : 3;\n"
 
 #: openassessment/assessment/api/student_training.py:179
```

### Comparing `ora2-5.0.0/openassessment/locale/he/LC_MESSAGES/djangojs.mo` & `ora2-5.0.1/openassessment/locale/he/LC_MESSAGES/djangojs.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Hodaya Zada <hodayaz@mse.gov.il>, 2019\n"
-"Language-Team: Hebrew (http://www.transifex.com/open-edx/edx-platform/"
+"Language-Team: Hebrew (http://app.transifex.com/open-edx/edx-platform/"
 "language/he/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: he\n"
 "Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n == 2 && n % "
 "1 == 0) ? 1: (n % 10 == 0 && n % 1 == 0 && n > 10) ? 2 : 3;\n"
```

### Comparing `ora2-5.0.0/openassessment/locale/he/LC_MESSAGES/djangojs.po` & `ora2-5.0.1/openassessment/locale/he/LC_MESSAGES/djangojs.po`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-09-13 04:00-0400\n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Hodaya Zada <hodayaz@mse.gov.il>, 2019\n"
-"Language-Team: Hebrew (http://www.transifex.com/open-edx/edx-platform/language/he/)\n"
+"Language-Team: Hebrew (http://app.transifex.com/open-edx/edx-platform/language/he/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: he\n"
 "Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n == 2 && n % 1 == 0) ? 1: (n % 10 == 0 && n % 1 == 0 && n > 10) ? 2 : 3;\n"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
```

### Comparing `ora2-5.0.0/openassessment/locale/hi/LC_MESSAGES/django.mo` & `ora2-5.0.1/openassessment/locale/hi/LC_MESSAGES/django.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
 "Last-Translator: Manish Manish <manish@manprax.com>, 2020\n"
-"Language-Team: Hindi (http://www.transifex.com/open-edx/edx-platform/"
+"Language-Team: Hindi (http://app.transifex.com/open-edx/edx-platform/"
 "language/hi/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: hi\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `ora2-5.0.0/openassessment/locale/hi/LC_MESSAGES/django.po` & `ora2-5.0.1/openassessment/locale/hi/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 # CHANDRA SHEKHAR SHARMA <shekharsharma041@gmail.com>, 2015
 # Goutam Kumar Dey <de_kumargoutam@yahoo.co.in>, 2014
 # Manish Manish <manish@manprax.com>, 2020
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-01-15 13:36-0500\n"
+"POT-Creation-Date: 2023-04-30 14:36-0400\n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
 "Last-Translator: Manish Manish <manish@manprax.com>, 2020\n"
-"Language-Team: Hindi (http://www.transifex.com/open-edx/edx-platform/language/hi/)\n"
+"Language-Team: Hindi (http://app.transifex.com/open-edx/edx-platform/language/hi/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: hi\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: openassessment/assessment/api/student_training.py:179
```

### Comparing `ora2-5.0.0/openassessment/locale/hi/LC_MESSAGES/djangojs.mo` & `ora2-5.0.1/openassessment/locale/hi/LC_MESSAGES/djangojs.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Manish Manish <manish@manprax.com>, 2021\n"
-"Language-Team: Hindi (http://www.transifex.com/open-edx/edx-platform/"
+"Language-Team: Hindi (http://app.transifex.com/open-edx/edx-platform/"
 "language/hi/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: hi\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `ora2-5.0.0/openassessment/locale/hi/LC_MESSAGES/djangojs.po` & `ora2-5.0.1/openassessment/locale/hi/LC_MESSAGES/djangojs.po`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-09-13 04:00-0400\n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Manish Manish <manish@manprax.com>, 2021\n"
-"Language-Team: Hindi (http://www.transifex.com/open-edx/edx-platform/language/hi/)\n"
+"Language-Team: Hindi (http://app.transifex.com/open-edx/edx-platform/language/hi/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: hi\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
```

### Comparing `ora2-5.0.0/openassessment/locale/id/LC_MESSAGES/django.mo` & `ora2-5.0.1/openassessment/locale/id/LC_MESSAGES/django.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,15 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
-"Last-Translator: Stefania Trabucchi <stefania.trabucchi@abstract-technology."
-"de>, 2019\n"
-"Language-Team: Indonesian (http://www.transifex.com/open-edx/edx-platform/"
+"Last-Translator: Faizar Septiawan <faizarsangster@gmail.com>, 2023\n"
+"Language-Team: Indonesian (http://app.transifex.com/open-edx/edx-platform/"
 "language/id/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: id\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
```

### Comparing `ora2-5.0.0/openassessment/locale/id/LC_MESSAGES/django.po` & `ora2-5.0.1/openassessment/locale/id/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,27 +2,29 @@
 # edX translation file
 # Copyright (C) 2018 edX
 # This file is distributed under the GNU AFFERO GENERAL PUBLIC LICENSE.
 # 
 # Translators:
 # Aprisa Chrysantina <aprisa.chrysantina@gmail.com>, 2018-2019
 # cholif yulian <cholifyulian123@gmail.com>, 2015
+# Faizar Septiawan <faizarsangster@gmail.com>, 2023
 # Farhanah Sheets <fsheets@edx.org>, 2018
 # Firnanda srimurni kurniawan <firnanda.srimurni.k@gmail.com>, 2018
 # ichs <ichsansp@outlook.com>, 2014
 # ichs <ichsansp@outlook.com>, 2014
+# Reza Almanda <rezaalmanda27@gmail.com>, 2023
 # Stefania Trabucchi <stefania.trabucchi@abstract-technology.de>, 2019
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-01-15 13:36-0500\n"
+"POT-Creation-Date: 2023-04-30 14:36-0400\n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
-"Last-Translator: Stefania Trabucchi <stefania.trabucchi@abstract-technology.de>, 2019\n"
-"Language-Team: Indonesian (http://www.transifex.com/open-edx/edx-platform/language/id/)\n"
+"Last-Translator: Faizar Septiawan <faizarsangster@gmail.com>, 2023\n"
+"Language-Team: Indonesian (http://app.transifex.com/open-edx/edx-platform/language/id/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: id\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 #: openassessment/assessment/api/student_training.py:179
```

### Comparing `ora2-5.0.0/openassessment/locale/id/LC_MESSAGES/djangojs.mo` & `ora2-5.0.1/openassessment/locale/id/LC_MESSAGES/djangojs.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Faizar Septiawan <faizarsangster@gmail.com>, 2022\n"
-"Language-Team: Indonesian (http://www.transifex.com/open-edx/edx-platform/"
+"Language-Team: Indonesian (http://app.transifex.com/open-edx/edx-platform/"
 "language/id/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: id\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
```

### Comparing `ora2-5.0.0/openassessment/locale/id/LC_MESSAGES/djangojs.po` & `ora2-5.0.1/openassessment/locale/id/LC_MESSAGES/djangojs.po`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-09-13 04:00-0400\n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Faizar Septiawan <faizarsangster@gmail.com>, 2022\n"
-"Language-Team: Indonesian (http://www.transifex.com/open-edx/edx-platform/language/id/)\n"
+"Language-Team: Indonesian (http://app.transifex.com/open-edx/edx-platform/language/id/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: id\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
```

### Comparing `ora2-5.0.0/openassessment/locale/it_IT/LC_MESSAGES/django.mo` & `ora2-5.0.1/openassessment/locale/it_IT/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
 "Last-Translator: Diana Huang <dkh@edx.org>, 2022\n"
-"Language-Team: Italian (Italy) (http://www.transifex.com/open-edx/edx-"
+"Language-Team: Italian (Italy) (http://app.transifex.com/open-edx/edx-"
 "platform/language/it_IT/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: it_IT\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? "
 "1 : 2;\n"
```

### Comparing `ora2-5.0.0/openassessment/locale/it_IT/LC_MESSAGES/django.po` & `ora2-5.0.1/openassessment/locale/it_IT/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 # Nicola Moretto <nicolamoretto88@gmail.com>, 2014
 # Nicola Cois <nicolacois@hotmail.com>, 2014
 # Stefania Trabucchi <stefania.trabucchi@abstract-technology.de>, 2021
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-01-15 13:36-0500\n"
+"POT-Creation-Date: 2023-04-30 14:36-0400\n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
 "Last-Translator: Diana Huang <dkh@edx.org>, 2022\n"
-"Language-Team: Italian (Italy) (http://www.transifex.com/open-edx/edx-platform/language/it_IT/)\n"
+"Language-Team: Italian (Italy) (http://app.transifex.com/open-edx/edx-platform/language/it_IT/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: it_IT\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 
 #: openassessment/assessment/api/student_training.py:179
```

### Comparing `ora2-5.0.0/openassessment/locale/it_IT/LC_MESSAGES/djangojs.mo` & `ora2-5.0.1/openassessment/locale/it_IT/LC_MESSAGES/djangojs.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Domenico Casanica <domenico.casanica@sistinf.it>, 2021\n"
-"Language-Team: Italian (Italy) (http://www.transifex.com/open-edx/edx-"
+"Language-Team: Italian (Italy) (http://app.transifex.com/open-edx/edx-"
 "platform/language/it_IT/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: it_IT\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? "
 "1 : 2;\n"
```

### Comparing `ora2-5.0.0/openassessment/locale/it_IT/LC_MESSAGES/djangojs.po` & `ora2-5.0.1/openassessment/locale/it_IT/LC_MESSAGES/djangojs.po`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-09-13 04:00-0400\n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Domenico Casanica <domenico.casanica@sistinf.it>, 2021\n"
-"Language-Team: Italian (Italy) (http://www.transifex.com/open-edx/edx-platform/language/it_IT/)\n"
+"Language-Team: Italian (Italy) (http://app.transifex.com/open-edx/edx-platform/language/it_IT/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: it_IT\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
```

### Comparing `ora2-5.0.0/openassessment/locale/ja_JP/LC_MESSAGES/django.mo` & `ora2-5.0.1/openassessment/locale/ja_JP/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
 "Last-Translator: Kyoto University <edxkyotoux@gmail.com>, 2017,2019\n"
-"Language-Team: Japanese (Japan) (http://www.transifex.com/open-edx/edx-"
+"Language-Team: Japanese (Japan) (http://app.transifex.com/open-edx/edx-"
 "platform/language/ja_JP/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: ja_JP\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
```

### Comparing `ora2-5.0.0/openassessment/locale/ja_JP/LC_MESSAGES/django.po` & `ora2-5.0.1/openassessment/locale/ja_JP/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 # Takashi Nagai <ngi644@gmail.com>, 2014
 # tomoo suzuki <t.suzuki@gacco.co.jp>, 2016
 # Toshiboumi Ohta <ohta@securesky-tech.com>, 2018
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-01-15 13:36-0500\n"
+"POT-Creation-Date: 2023-04-30 14:36-0400\n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
 "Last-Translator: Kyoto University <edxkyotoux@gmail.com>, 2017,2019\n"
-"Language-Team: Japanese (Japan) (http://www.transifex.com/open-edx/edx-platform/language/ja_JP/)\n"
+"Language-Team: Japanese (Japan) (http://app.transifex.com/open-edx/edx-platform/language/ja_JP/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: ja_JP\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 #: openassessment/assessment/api/student_training.py:179
```

### Comparing `ora2-5.0.0/openassessment/locale/ja_JP/LC_MESSAGES/djangojs.mo` & `ora2-5.0.1/openassessment/locale/ja_JP/LC_MESSAGES/djangojs.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Toshiboumi Ohta <ohta@securesky-tech.com>, 2018\n"
-"Language-Team: Japanese (Japan) (http://www.transifex.com/open-edx/edx-"
+"Language-Team: Japanese (Japan) (http://app.transifex.com/open-edx/edx-"
 "platform/language/ja_JP/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: ja_JP\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
```

### Comparing `ora2-5.0.0/openassessment/locale/ja_JP/LC_MESSAGES/djangojs.po` & `ora2-5.0.1/openassessment/locale/ja_JP/LC_MESSAGES/djangojs.po`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-09-13 04:00-0400\n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Toshiboumi Ohta <ohta@securesky-tech.com>, 2018\n"
-"Language-Team: Japanese (Japan) (http://www.transifex.com/open-edx/edx-platform/language/ja_JP/)\n"
+"Language-Team: Japanese (Japan) (http://app.transifex.com/open-edx/edx-platform/language/ja_JP/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: ja_JP\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
```

### Comparing `ora2-5.0.0/openassessment/locale/ka/LC_MESSAGES/django.mo` & `ora2-5.0.1/openassessment/locale/ka/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
 "Last-Translator: Lasha Kokilashvili, 2018\n"
-"Language-Team: Georgian (http://www.transifex.com/open-edx/edx-platform/"
+"Language-Team: Georgian (http://app.transifex.com/open-edx/edx-platform/"
 "language/ka/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: ka\n"
 "Plural-Forms: nplurals=2; plural=(n!=1);\n"
```

### Comparing `ora2-5.0.0/openassessment/locale/ka/LC_MESSAGES/django.po` & `ora2-5.0.1/openassessment/locale/ka/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 # Giorgi Goderdzishvili <biggeorgian@gmail.com>, 2017
 # ketevan Kokhreidze <k.kokhreidze@gmail.com>, 2016
 # Lasha Kokilashvili, 2018
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-01-15 13:36-0500\n"
+"POT-Creation-Date: 2023-04-30 14:36-0400\n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
 "Last-Translator: Lasha Kokilashvili, 2018\n"
-"Language-Team: Georgian (http://www.transifex.com/open-edx/edx-platform/language/ka/)\n"
+"Language-Team: Georgian (http://app.transifex.com/open-edx/edx-platform/language/ka/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: ka\n"
 "Plural-Forms: nplurals=2; plural=(n!=1);\n"
 
 #: openassessment/assessment/api/student_training.py:179
```

### Comparing `ora2-5.0.0/openassessment/locale/ka/LC_MESSAGES/djangojs.mo` & `ora2-5.0.1/openassessment/locale/ka/LC_MESSAGES/djangojs.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Giorgi Goderdzishvili <biggeorgian@gmail.com>, 2016\n"
-"Language-Team: Georgian (http://www.transifex.com/open-edx/edx-platform/"
+"Language-Team: Georgian (http://app.transifex.com/open-edx/edx-platform/"
 "language/ka/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: ka\n"
 "Plural-Forms: nplurals=2; plural=(n!=1);\n"
```

### Comparing `ora2-5.0.0/openassessment/locale/ka/LC_MESSAGES/djangojs.po` & `ora2-5.0.1/openassessment/locale/ka/LC_MESSAGES/djangojs.po`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-09-13 04:00-0400\n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Giorgi Goderdzishvili <biggeorgian@gmail.com>, 2016\n"
-"Language-Team: Georgian (http://www.transifex.com/open-edx/edx-platform/language/ka/)\n"
+"Language-Team: Georgian (http://app.transifex.com/open-edx/edx-platform/language/ka/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: ka\n"
 "Plural-Forms: nplurals=2; plural=(n!=1);\n"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
```

### Comparing `ora2-5.0.0/openassessment/locale/lt_LT/LC_MESSAGES/django.mo` & `ora2-5.0.1/openassessment/locale/lt_LT/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
 "Last-Translator: Edukometrija <jolitad@mruni.eu>, 2015\n"
-"Language-Team: Lithuanian (Lithuania) (http://www.transifex.com/open-edx/edx-"
+"Language-Team: Lithuanian (Lithuania) (http://app.transifex.com/open-edx/edx-"
 "platform/language/lt_LT/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: lt_LT\n"
 "Plural-Forms: nplurals=4; plural=(n % 10 == 1 && (n % 100 > 19 || n % 100 < "
 "11) ? 0 : (n % 10 >= 2 && n % 10 <=9) && (n % 100 > 19 || n % 100 < 11) ? "
```

### Comparing `ora2-5.0.0/openassessment/locale/lt_LT/LC_MESSAGES/django.po` & `ora2-5.0.1/openassessment/locale/lt_LT/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 # Translators:
 # Riina <ciairdabar@yahoo.com>, 2014-2015
 # Edukometrija <jolitad@mruni.eu>, 2015
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-01-15 13:36-0500\n"
+"POT-Creation-Date: 2023-04-30 14:36-0400\n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
 "Last-Translator: Edukometrija <jolitad@mruni.eu>, 2015\n"
-"Language-Team: Lithuanian (Lithuania) (http://www.transifex.com/open-edx/edx-platform/language/lt_LT/)\n"
+"Language-Team: Lithuanian (Lithuania) (http://app.transifex.com/open-edx/edx-platform/language/lt_LT/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: lt_LT\n"
 "Plural-Forms: nplurals=4; plural=(n % 10 == 1 && (n % 100 > 19 || n % 100 < 11) ? 0 : (n % 10 >= 2 && n % 10 <=9) && (n % 100 > 19 || n % 100 < 11) ? 1 : n % 1 != 0 ? 2: 3);\n"
 
 #: openassessment/assessment/api/student_training.py:179
```

### Comparing `ora2-5.0.0/openassessment/locale/lt_LT/LC_MESSAGES/djangojs.mo` & `ora2-5.0.1/openassessment/locale/lt_LT/LC_MESSAGES/djangojs.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Edukometrija <jolitad@mruni.eu>, 2015\n"
-"Language-Team: Lithuanian (Lithuania) (http://www.transifex.com/open-edx/edx-"
+"Language-Team: Lithuanian (Lithuania) (http://app.transifex.com/open-edx/edx-"
 "platform/language/lt_LT/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: lt_LT\n"
 "Plural-Forms: nplurals=4; plural=(n % 10 == 1 && (n % 100 > 19 || n % 100 < "
 "11) ? 0 : (n % 10 >= 2 && n % 10 <=9) && (n % 100 > 19 || n % 100 < 11) ? "
```

### Comparing `ora2-5.0.0/openassessment/locale/lt_LT/LC_MESSAGES/djangojs.po` & `ora2-5.0.1/openassessment/locale/lt_LT/LC_MESSAGES/djangojs.po`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-09-13 04:00-0400\n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Edukometrija <jolitad@mruni.eu>, 2015\n"
-"Language-Team: Lithuanian (Lithuania) (http://www.transifex.com/open-edx/edx-platform/language/lt_LT/)\n"
+"Language-Team: Lithuanian (Lithuania) (http://app.transifex.com/open-edx/edx-platform/language/lt_LT/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: lt_LT\n"
 "Plural-Forms: nplurals=4; plural=(n % 10 == 1 && (n % 100 > 19 || n % 100 < 11) ? 0 : (n % 10 >= 2 && n % 10 <=9) && (n % 100 > 19 || n % 100 < 11) ? 1 : n % 1 != 0 ? 2: 3);\n"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
```

### Comparing `ora2-5.0.0/openassessment/locale/lv/LC_MESSAGES/django.mo` & `ora2-5.0.1/openassessment/locale/lv/LC_MESSAGES/django.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
 "Last-Translator: Muhammad Ayub khan <ayubkhan@edx.org>\n"
-"Language-Team: Latvian (http://www.transifex.com/open-edx/edx-platform/"
+"Language-Team: Latvian (http://app.transifex.com/open-edx/edx-platform/"
 "language/lv/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: lv\n"
 "Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n != 0 ? 1 : "
 "2);\n"
```

### Comparing `ora2-5.0.0/openassessment/locale/lv/LC_MESSAGES/django.po` & `ora2-5.0.1/openassessment/locale/lv/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 # This file is distributed under the GNU AFFERO GENERAL PUBLIC LICENSE.
 # 
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-01-15 13:36-0500\n"
+"POT-Creation-Date: 2023-04-30 14:36-0400\n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
 "Last-Translator: Muhammad Ayub khan <ayubkhan@edx.org>\n"
-"Language-Team: Latvian (http://www.transifex.com/open-edx/edx-platform/language/lv/)\n"
+"Language-Team: Latvian (http://app.transifex.com/open-edx/edx-platform/language/lv/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: lv\n"
 "Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n != 0 ? 1 : 2);\n"
 
 #: openassessment/assessment/api/student_training.py:179
```

### Comparing `ora2-5.0.0/openassessment/locale/lv/LC_MESSAGES/djangojs.mo` & `ora2-5.0.1/openassessment/locale/lv/LC_MESSAGES/djangojs.mo`

 * *Files 11% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Muhammad Ayub khan <ayubkhan@edx.org>\n"
-"Language-Team: Latvian (http://www.transifex.com/open-edx/edx-platform/"
+"Language-Team: Latvian (http://app.transifex.com/open-edx/edx-platform/"
 "language/lv/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: lv\n"
 "Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n != 0 ? 1 : "
 "2);\n"
```

### Comparing `ora2-5.0.0/openassessment/locale/lv/LC_MESSAGES/djangojs.po` & `ora2-5.0.1/openassessment/locale/lv/LC_MESSAGES/djangojs.po`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-09-13 04:00-0400\n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Muhammad Ayub khan <ayubkhan@edx.org>\n"
-"Language-Team: Latvian (http://www.transifex.com/open-edx/edx-platform/language/lv/)\n"
+"Language-Team: Latvian (http://app.transifex.com/open-edx/edx-platform/language/lv/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: lv\n"
 "Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n != 0 ? 1 : 2);\n"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
```

### Comparing `ora2-5.0.0/openassessment/locale/messages.mo` & `ora2-5.0.1/openassessment/locale/messages.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/locale/mn/LC_MESSAGES/django.mo` & `ora2-5.0.1/openassessment/locale/mn/LC_MESSAGES/django.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
 "Last-Translator: Myagmarjav Enkhbileg <miigaa.lucky@gmail.com>, 2021\n"
-"Language-Team: Mongolian (http://www.transifex.com/open-edx/edx-platform/"
+"Language-Team: Mongolian (http://app.transifex.com/open-edx/edx-platform/"
 "language/mn/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: mn\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `ora2-5.0.0/openassessment/locale/mn/LC_MESSAGES/django.po` & `ora2-5.0.1/openassessment/locale/mn/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 # Jamka Sukhee <jambka.93@gmail.com>, 2021
 # Mendbayar Gantulga <mendbayar_mgo@yahoo.com>, 2021
 # Myagmarjav Enkhbileg <miigaa.lucky@gmail.com>, 2021
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-01-15 13:36-0500\n"
+"POT-Creation-Date: 2023-04-30 14:36-0400\n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
 "Last-Translator: Myagmarjav Enkhbileg <miigaa.lucky@gmail.com>, 2021\n"
-"Language-Team: Mongolian (http://www.transifex.com/open-edx/edx-platform/language/mn/)\n"
+"Language-Team: Mongolian (http://app.transifex.com/open-edx/edx-platform/language/mn/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: mn\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: openassessment/assessment/api/student_training.py:179
```

### Comparing `ora2-5.0.0/openassessment/locale/mn/LC_MESSAGES/djangojs.mo` & `ora2-5.0.1/openassessment/locale/mn/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/locale/mn/LC_MESSAGES/djangojs.po` & `ora2-5.0.1/openassessment/locale/mn/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/locale/nb/LC_MESSAGES/django.mo` & `ora2-5.0.1/openassessment/locale/nb/LC_MESSAGES/django.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
 "Last-Translator: Frode Arntsen <frode.arntsen@unit.no>, 2014,2016-2017\n"
-"Language-Team: Norwegian Bokmål (http://www.transifex.com/open-edx/edx-"
+"Language-Team: Norwegian Bokmål (http://app.transifex.com/open-edx/edx-"
 "platform/language/nb/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: nb\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `ora2-5.0.0/openassessment/locale/nb/LC_MESSAGES/django.po` & `ora2-5.0.1/openassessment/locale/nb/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 # Lene2015 <gundersen_lene@hotmail.com>, 2015
 # Joakim S. Johnson, 2016
 # Øyvind Eide <oaeide@gmail.com>, 2014
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-01-15 13:36-0500\n"
+"POT-Creation-Date: 2023-04-30 14:36-0400\n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
 "Last-Translator: Frode Arntsen <frode.arntsen@unit.no>, 2014,2016-2017\n"
-"Language-Team: Norwegian Bokmål (http://www.transifex.com/open-edx/edx-platform/language/nb/)\n"
+"Language-Team: Norwegian Bokmål (http://app.transifex.com/open-edx/edx-platform/language/nb/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: nb\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: openassessment/assessment/api/student_training.py:179
```

### Comparing `ora2-5.0.0/openassessment/locale/nb/LC_MESSAGES/djangojs.mo` & `ora2-5.0.1/openassessment/locale/nb/LC_MESSAGES/djangojs.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Frode Arntsen <frode.arntsen@unit.no>, 2018\n"
-"Language-Team: Norwegian Bokmål (http://www.transifex.com/open-edx/edx-"
+"Language-Team: Norwegian Bokmål (http://app.transifex.com/open-edx/edx-"
 "platform/language/nb/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: nb\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `ora2-5.0.0/openassessment/locale/nb/LC_MESSAGES/djangojs.po` & `ora2-5.0.1/openassessment/locale/nb/LC_MESSAGES/djangojs.po`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-09-13 04:00-0400\n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Frode Arntsen <frode.arntsen@unit.no>, 2018\n"
-"Language-Team: Norwegian Bokmål (http://www.transifex.com/open-edx/edx-platform/language/nb/)\n"
+"Language-Team: Norwegian Bokmål (http://app.transifex.com/open-edx/edx-platform/language/nb/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: nb\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
```

### Comparing `ora2-5.0.0/openassessment/locale/pl/LC_MESSAGES/django.mo` & `ora2-5.0.1/openassessment/locale/pl/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
 "Last-Translator: Klara Sielicka-Baryłka, 2022\n"
-"Language-Team: Polish (http://www.transifex.com/open-edx/edx-platform/"
+"Language-Team: Polish (http://app.transifex.com/open-edx/edx-platform/"
 "language/pl/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: pl\n"
 "Plural-Forms: nplurals=4; plural=(n==1 ? 0 : (n%10>=2 && n%10<=4) && "
 "(n%100<12 || n%100>14) ? 1 : n!=1 && (n%10>=0 && n%10<=1) || (n%10>=5 && "
```

### Comparing `ora2-5.0.0/openassessment/locale/pl/LC_MESSAGES/django.po` & `ora2-5.0.1/openassessment/locale/pl/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -20,18 +20,18 @@
 # MONIKA STEFAŃCZYK <monika_stefanczyk@wp.pl>, 2016
 # Paweł Marchewka <mamior@o2.pl>, 2014
 # Sebastian <foobarbaz@gazeta.pl>, 2014
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-01-15 13:36-0500\n"
+"POT-Creation-Date: 2023-04-30 14:36-0400\n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
 "Last-Translator: Klara Sielicka-Baryłka, 2022\n"
-"Language-Team: Polish (http://www.transifex.com/open-edx/edx-platform/language/pl/)\n"
+"Language-Team: Polish (http://app.transifex.com/open-edx/edx-platform/language/pl/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: pl\n"
 "Plural-Forms: nplurals=4; plural=(n==1 ? 0 : (n%10>=2 && n%10<=4) && (n%100<12 || n%100>14) ? 1 : n!=1 && (n%10>=0 && n%10<=1) || (n%10>=5 && n%10<=9) || (n%100>=12 && n%100<=14) ? 2 : 3);\n"
 
 #: openassessment/assessment/api/student_training.py:179
```

### Comparing `ora2-5.0.0/openassessment/locale/pl/LC_MESSAGES/djangojs.mo` & `ora2-5.0.1/openassessment/locale/pl/LC_MESSAGES/djangojs.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Magdalena Dulęba <magdalena.duleba@e-science.pl>, 2022\n"
-"Language-Team: Polish (http://www.transifex.com/open-edx/edx-platform/"
+"Language-Team: Polish (http://app.transifex.com/open-edx/edx-platform/"
 "language/pl/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: pl\n"
 "Plural-Forms: nplurals=4; plural=(n==1 ? 0 : (n%10>=2 && n%10<=4) && "
 "(n%100<12 || n%100>14) ? 1 : n!=1 && (n%10>=0 && n%10<=1) || (n%10>=5 && "
```

### Comparing `ora2-5.0.0/openassessment/locale/pl/LC_MESSAGES/djangojs.po` & `ora2-5.0.1/openassessment/locale/pl/LC_MESSAGES/djangojs.po`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-09-13 04:00-0400\n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Magdalena Dulęba <magdalena.duleba@e-science.pl>, 2022\n"
-"Language-Team: Polish (http://www.transifex.com/open-edx/edx-platform/language/pl/)\n"
+"Language-Team: Polish (http://app.transifex.com/open-edx/edx-platform/language/pl/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: pl\n"
 "Plural-Forms: nplurals=4; plural=(n==1 ? 0 : (n%10>=2 && n%10<=4) && (n%100<12 || n%100>14) ? 1 : n!=1 && (n%10>=0 && n%10<=1) || (n%10>=5 && n%10<=9) || (n%100>=12 && n%100<=14) ? 2 : 3);\n"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
```

### Comparing `ora2-5.0.0/openassessment/locale/pt_BR/LC_MESSAGES/django.mo` & `ora2-5.0.1/openassessment/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
 "Last-Translator: Emmanuel Halbout <emmanuelhalbout@neojiba.org>, 2020\n"
-"Language-Team: Portuguese (Brazil) (http://www.transifex.com/open-edx/edx-"
+"Language-Team: Portuguese (Brazil) (http://app.transifex.com/open-edx/edx-"
 "platform/language/pt_BR/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: pt_BR\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
 "1000000 == 0 ? 1 : 2;\n"
```

### Comparing `ora2-5.0.0/openassessment/locale/pt_BR/LC_MESSAGES/django.po` & `ora2-5.0.1/openassessment/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -28,18 +28,18 @@
 # Ricardo Pietrobon <pietr007@gmail.com>, 2014
 # William Bellinazo Roca <williambr_1331@hotmail.com>, 2016
 # Willian Pascoal <willianpascoal@protonmail.com>, 2016
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-01-15 13:36-0500\n"
+"POT-Creation-Date: 2023-04-30 14:36-0400\n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
 "Last-Translator: Emmanuel Halbout <emmanuelhalbout@neojiba.org>, 2020\n"
-"Language-Team: Portuguese (Brazil) (http://www.transifex.com/open-edx/edx-platform/language/pt_BR/)\n"
+"Language-Team: Portuguese (Brazil) (http://app.transifex.com/open-edx/edx-platform/language/pt_BR/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: pt_BR\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 
 #: openassessment/assessment/api/student_training.py:179
```

### Comparing `ora2-5.0.0/openassessment/locale/pt_BR/LC_MESSAGES/djangojs.mo` & `ora2-5.0.1/openassessment/locale/pt_BR/LC_MESSAGES/djangojs.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Emmanuel Halbout <emmanuelhalbout@neojiba.org>, 2020\n"
-"Language-Team: Portuguese (Brazil) (http://www.transifex.com/open-edx/edx-"
+"Language-Team: Portuguese (Brazil) (http://app.transifex.com/open-edx/edx-"
 "platform/language/pt_BR/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: pt_BR\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
 "1000000 == 0 ? 1 : 2;\n"
```

### Comparing `ora2-5.0.0/openassessment/locale/pt_BR/LC_MESSAGES/djangojs.po` & `ora2-5.0.1/openassessment/locale/pt_BR/LC_MESSAGES/djangojs.po`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-09-13 04:00-0400\n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Emmanuel Halbout <emmanuelhalbout@neojiba.org>, 2020\n"
-"Language-Team: Portuguese (Brazil) (http://www.transifex.com/open-edx/edx-platform/language/pt_BR/)\n"
+"Language-Team: Portuguese (Brazil) (http://app.transifex.com/open-edx/edx-platform/language/pt_BR/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: pt_BR\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
```

### Comparing `ora2-5.0.0/openassessment/locale/pt_PT/LC_MESSAGES/django.mo` & `ora2-5.0.1/openassessment/locale/pt_PT/LC_MESSAGES/django.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
-"Last-Translator: Nika Shahidian, 2022\n"
-"Language-Team: Portuguese (Portugal) (http://www.transifex.com/open-edx/edx-"
+"Last-Translator: Ivo Branco <ivo.branco@fccn.pt>, 2021,2023\n"
+"Language-Team: Portuguese (Portugal) (http://app.transifex.com/open-edx/edx-"
 "platform/language/pt_PT/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: pt_PT\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
 "1000000 == 0 ? 1 : 2;\n"
@@ -120,14 +120,40 @@
 "\n"
 "                                        Resposta para: %(team_name)s com "
 "%(team_usernames)s\n"
 "                                    "
 
 msgid ""
 "\n"
+"                                      You are currently on Team "
+"%(team_name)s. Since you were on Team %(previous_team_name)s\n"
+"                                      when they submitted a response to this "
+"assignment, you are seeing Team %(previous_team_name)s’s\n"
+"                                      response and will receive the same "
+"grade for this assignment as your former teammates.\n"
+"                                      You will not be part of Team "
+"%(team_name)s’s submission for this assignment and will not\n"
+"                                      receive a grade for their submission.\n"
+"                                  "
+msgstr ""
+"\n"
+"                                      Neste momento está na Equipa "
+"%(team_name)s. Visto que esteve na Equipa %(previous_team_name)s\n"
+"                                      quando submeteram uma resposta a esta "
+"tarefa, está a ver a resposta da Equipa %(previous_team_name)s\n"
+"                                      e irá receber a mesma classificação "
+"dos seus colegas anteriores.\n"
+"                                      Não irá fazer parte da submissão da "
+"Equipa %(team_name)spara esta tarefa e não irá\n"
+"                                      receber uma classificação para a "
+"submissão deles.\n"
+"                                  "
+
+msgid ""
+"\n"
 "                                    %(start_strong)sThis assignment is in "
 "progress. The self assessment step will close soon.%(end_strong)s You still "
 "need to complete the %(start_link)sself assessment%(end_link)s step.\n"
 "                                "
 msgstr ""
 "\n"
 "                                    %(start_strong)s Esta tarefa está em "
@@ -203,14 +229,29 @@
 "tarde para verificar se existem novas respostas de estudantes. Ainda "
 "necessita de concluir a etapa de %(start_link)savaliação dos "
 "pares%(end_link)s.\n"
 "                             "
 
 msgid ""
 "\n"
+"                                  Upload files and review files uploaded by "
+"you and your teammates below. Be sure to add\n"
+"                                  descriptions to your files to help your "
+"teammates identify them.\n"
+"                              "
+msgstr ""
+"\n"
+"                                  Carregue ficheiros e reveja ficheiros "
+"carregados por si e pela sua equipa abaixo. Não se esqueça de acrescentar\n"
+"                                  descrições aos seus ficheiros para ajudar "
+"os seus colegas a identificá-los.\n"
+"                              "
+
+msgid ""
+"\n"
 "                                Your submission has been cancelled by "
 "%(removed_by_username)s on %(removed_datetime)s\n"
 "                            "
 msgstr ""
 "\n"
 "O seu envio foi cancelado por %(removed_by_username)s a %(removed_datetime)s "
 
@@ -452,14 +493,29 @@
 msgstr ""
 "\n"
 "                    Ver equipa: %(team)s\n"
 "                "
 
 msgid ""
 "\n"
+"                  Learn more about team assignments here: (<a "
+"target=\"_blank\" href=\"https://support.edx.org/hc/en-us/"
+"articles/360000191067-Submit-your-"
+"response#h_01FVD8SXM9E5H2DNAG87X25ZHR\">link</a>)\n"
+"                  "
+msgstr ""
+"\n"
+"                  Saiba mais sobre as tarefas da equipa aqui: (<a "
+"target=\"_blank\" href=\"https://support.edx.org/hc/en-us/"
+"articles/360000191067-Submit-your-"
+"response#h_01FVD8SXM9E5H2DNAG87X25ZHR\">link</a>)\n"
+"                  "
+
+msgid ""
+"\n"
 "                %(start_tag)s%(title)s%(end_tag)s%(start_grade_tag)s - "
 "%(grade)s%(end_tag)s\n"
 "              "
 msgstr ""
 "\n"
 "                %(start_tag)s%(title)s%(end_tag)s%(start_grade_tag)s - "
 "%(grade)s%(end_tag)s\n"
@@ -792,14 +848,20 @@
 msgstr ""
 "Antes de começar a avaliar as respostas dos seus colegas, irá aprender a "
 "como avaliar os pares, analisando as respostas que os formadores já "
 "avaliaram. Caso selecione as mesmas opções de resposta que o formador "
 "selecionou, irá passar para a próxima etapa. Caso não selecione as mesmas "
 "opções, terá de rever a resposta e tentar novamente."
 
+msgid "Block ID"
+msgstr "Bloco ID"
+
+msgid "Block ID For this ORA:"
+msgstr "Bloco ID Para este ORA - Open Response Assessment:"
+
 msgid "Cancel"
 msgstr "Cancelar"
 
 msgid "Cancelled"
 msgstr "Cancelado"
 
 msgid ""
@@ -821,14 +883,20 @@
 msgstr ""
 "Volte mais tarde para ver se algum elemento da equipa do curso avaliou a sua "
 "resposta. Apenas receberá a sua nota após a conclusão da avaliação."
 
 msgid "Click to preview your submission in LaTeX."
 msgstr "Clique para visualizar o seu envio em LaTeX."
 
+msgid "Clone"
+msgstr "Réplica"
+
+msgid "Clone Rubric"
+msgstr "Replicar Rubrica"
+
 msgid "Close"
 msgstr "Fechar"
 
 msgid "Comments"
 msgstr "Comentários"
 
 msgid "Comments:"
@@ -836,14 +904,17 @@
 
 msgid "Compare your selections with the instructor's selections"
 msgstr "Compare as suas seleções com as seleções do formador"
 
 msgid "Complete"
 msgstr "Concluído"
 
+msgid "Complete/Overwritten"
+msgstr "Completo/Substituído"
+
 msgid "Completed"
 msgstr "Concluído"
 
 msgid ""
 "Configuration: For this step to be configured you must specify the number of "
 "peer reviews a student will be assessed with, and the number of peer a "
 "student must grade. Additional options can be specified."
@@ -915,14 +986,17 @@
 
 msgid "Dates"
 msgstr "Datas"
 
 msgid "Default Feedback Text"
 msgstr "Texto de comentários predefinido"
 
+msgid "Demo the new Grading Experience"
+msgstr "Demonstração da nova experiência de classificação"
+
 msgid "Display Name "
 msgstr "Nome Apresentado"
 
 msgid "Due Date"
 msgstr "Data limite"
 
 msgid "Due Time"
@@ -1170,14 +1244,17 @@
 
 msgid "Incomplete"
 msgstr "Incompleto"
 
 msgid "Instructions Unavailable"
 msgstr "Instruções não disponíveis"
 
+msgid "Invalid block id."
+msgstr "Bloco id inválido."
+
 msgid "Item ID"
 msgstr "Item ID"
 
 msgid "Leaderboard number is invalid."
 msgstr "O número da tabela classificativa é inválido."
 
 msgid "Learn to Assess Responses"
@@ -1243,17 +1320,26 @@
 
 msgid "Must Grade"
 msgstr "Deve Classificar"
 
 msgid "N/A"
 msgstr "N/D"
 
+msgid ""
+"No Open Response Assessment found in {course_id} with block id {block_id}"
+msgstr ""
+"Nenhuma Avaliação de Resposta Aberta encontrada em {course_id} com bloco id "
+"{block_id}"
+
 msgid "No description provided."
 msgstr "Nenhuma descrição fornecida."
 
+msgid "No other Open Response Assessments found in course"
+msgstr "Nenhumas outras Avaliações de Resposta Aberta encontradas no curso"
+
 msgid "No other learner responses are available for grading at this time."
 msgstr ""
 "Neste momento, não existe outra resposta do estudante está disponível para "
 "classificação."
 
 msgid "None"
 msgstr "Nenhum"
@@ -1266,14 +1352,28 @@
 
 msgid "Not Selected"
 msgstr "Não selecionado"
 
 msgid "Not Started"
 msgstr "Não iniciado"
 
+msgid "Not applicable"
+msgstr "Não aplicável"
+
+msgid "Not submitted"
+msgstr "Não submetido"
+
+msgid ""
+"Note: if you have a spellcheck or grammar check browser extension, try "
+"disabling, reloading, and reentering your response before submitting."
+msgstr ""
+"Nota: se tiver uma verificação ortográfica ou uma extensão de verificação "
+"gramatical do navegador, tente desactivar, recarregar, e reentrar a sua "
+"resposta antes de submeter."
+
 msgid ""
 "One team member should submit a response with the team’s shared files and a "
 "text response on behalf of the entire team."
 msgstr ""
 "Um membro da equipa deve enviar uma resposta com os ficheiros partilhados da "
 "equipa e uma resposta de texto em nome de toda a equipa."
 
@@ -1380,14 +1480,17 @@
 
 msgid "Peer Median Grade"
 msgstr "Classificação média dos pares"
 
 msgid "Peer {peer_index}"
 msgstr "Pares {peer_index}"
 
+msgid "Pending"
+msgstr "Pendente"
+
 msgid "Please enter valid reason to remove the submission."
 msgstr "Por favor, introduza um motivo válido para eliminar o envio."
 
 msgid "Please wait"
 msgstr "Por favor aguarde"
 
 msgid "Point values cannot be changed after a problem is released."
@@ -1493,20 +1596,26 @@
 
 msgid "Response Start Date"
 msgstr "Data de Início da Resposta"
 
 msgid "Response Start Time"
 msgstr "Hora de Início de Resposta"
 
+msgid "Response exceeds maximum allowed size."
+msgstr "A resposta excede o tamanho máximo permitido."
+
 msgid "Response total"
 msgstr "Total de respostas"
 
 msgid "Rubric"
 msgstr "Rúbrica"
 
+msgid "Rubric Successfully Cloned from Block ID: "
+msgstr "Rubrica Replicada com Sucesso a partir do Bloco ID: "
+
 msgid ""
 "Rubrics are made up of criteria, which usually contain one or more options. "
 "Each option has a point value. This template contains two sample criteria "
 "and their options. Replace the sample text with your own text. For more "
 "information, see the ORA documentation."
 msgstr ""
 "As rubricas são feitas de critérios, que geralmente contêm uma ou mais "
@@ -1611,14 +1720,23 @@
 "Specify the number of peer assessments that each learner must complete. "
 "Valid numbers are 1 to 99."
 msgstr ""
 "Especifique o número de avaliações por pares que cada estudante deve "
 "concluir. Os números válidos são de 1 a 99."
 
 msgid ""
+"Specify the number of top scoring responses to display after the learner has "
+"submitted a response. Valid numbers are 0 to 99. If the number is 0, the Top "
+"Responses section does not appear to learners."
+msgstr ""
+"Especificar o número de respostas de pontuação máxima a exibir após o "
+"estudante ter submetido uma resposta. Os números válidos são de 0 a 99. Se o "
+"número for 0, a secção de respostas de topo não aparece aos estudantes."
+
+msgid ""
 "Specify whether learners are able to upload files as a part of their "
 "response."
 msgstr ""
 "Especifique se os estudantes podem enviar ficheiros anexados às suas "
 "respostas."
 
 msgid ""
@@ -1751,14 +1869,17 @@
 
 msgid "Submit your assessment and review another response"
 msgstr "Submeta a sua avaliação e reveja outras respostas"
 
 msgid "Submit your response and move to the next step"
 msgstr "Envie sua resposta e transfira-a para a próxima etapa"
 
+msgid "Submitted"
+msgstr "Submetido"
+
 msgid "Submitting Feedback"
 msgstr "A enviar comentário"
 
 msgid "Successfully updated OpenAssessment XBlock"
 msgstr "Atualização bem-sucedida do OpenAssessment XBlock"
 
 msgid "Supported file types: "
@@ -2087,14 +2208,26 @@
 "To add more file extensions, select Custom File Types and enter the full "
 "list of acceptable file extensions to be included."
 msgstr ""
 "Para adicionar mais extensões de ficheiros, selecione Tipos de Ficheiros "
 "Personalizados e insira a lista completa de extensões de ficheiros "
 "aceitáveis a serem incluídas."
 
+msgid ""
+"To clone a rubric from an existing published or unpublished draft, you can "
+"search by the Block ID. Note that cloning is one-way, meaning changes made "
+"after cloning will only affect the rubric being modified, and will not "
+"modify any rubric it was cloned from."
+msgstr ""
+"Para replicar uma rubrica de um rascunho existente, quer tenha sido "
+"publicado ou não, pode pesquisar pelo Bloco ID. Note que a replicação é "
+"unidireccional, o que significa que as alterações feitas após a replicação "
+"apenas irão afetar a rubrica que está a ser modificada, e não irão modificar "
+"a rubrica a partir da qual foi replicada."
+
 msgid "To submit a response, view this component in Preview or Live mode."
 msgstr ""
 "Para enviar uma resposta, exiba este componente em modo Pré-visualização ou "
 "Tempo Real."
 
 msgid "Top Responses"
 msgstr "Respostas com Pontuação mais Elevada"
@@ -2119,20 +2252,33 @@
 
 msgid "View / Add Sample Responses"
 msgstr "Ver / Adicionar amostras de respostas"
 
 msgid "View Assignment Statistics"
 msgstr "Visualizar Estatísticas da Tarefa"
 
+msgid "View ORA in Studio"
+msgstr "Ver ORA - Open Response Assessment no Studio"
+
 msgid "View Options & Configuration"
 msgstr "Ver Opções e Configuração"
 
 msgid "View the files associated with this submission:"
 msgstr "Visualizar os ficheiros associados a este envio:"
 
+msgid "Waiting Step Details"
+msgstr "Detalhes da Etapa de Espera"
+
+msgid ""
+"Waiting Step details view is unavailable. This item is not configured for "
+"peer assessments."
+msgstr ""
+"A visualização dos detalhes da Etapa de Espera não está disponível. Este "
+"item não está configurado para avaliação por pares. "
+
 msgid "Waiting for Assessments"
 msgstr "A aguardar as avaliações"
 
 msgid "Waiting for a Staff Grade"
 msgstr "A aguardar pela Equipa de Classificação"
 
 msgid "Waiting for peer reviews"
@@ -2273,14 +2419,17 @@
 
 msgid "You must provide options selected in the assessment."
 msgstr "Deve disponibilizar opções selecionadas na avaliação."
 
 msgid "You must provide overall feedback in the assessment."
 msgstr "Deve fazer comentários geraois na avaliação."
 
+msgid "You must specify a block id from which to copy a rubric."
+msgstr "Deve especificar um bloco id a partir do qual copiar uma rubrica."
+
 msgid "You must submit a response before you can perform a peer assessment."
 msgstr ""
 "Deve submeter uma resposta antes de poder realizar a avaliação dos pares."
 
 msgid "You must submit a response before you can perform a self-assessment."
 msgstr "Deve submeter uma resposta antes de poder realizar uma auto-avaliação."
```

### Comparing `ora2-5.0.0/openassessment/locale/pt_PT/LC_MESSAGES/django.po` & `ora2-5.0.1/openassessment/locale/pt_PT/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,33 +4,33 @@
 # This file is distributed under the GNU AFFERO GENERAL PUBLIC LICENSE.
 # 
 # Translators:
 # Beatriz Sousa <beatriz.sousa@bridgelk.com>, 2018
 # Cátia Lopes <catia.lopes@bridgelk.com>, 2018-2019
 # Developer QUEO <developer@queo.pt>, 2017
 # Filipa Macieira <filipa.macieira@fccn.pt>, 2021
-# Ivo Branco <ivo.branco@fccn.pt>, 2021
+# Ivo Branco <ivo.branco@fccn.pt>, 2021,2023
 # 8b7f539cfdb680c92813b22b241ff5ad_86793ec, 2016
 # Manuela Silva <mmsrs@sky.com>, 2016,2018
 # Manuela Silva <mmsrs@sky.com>, 2018
 # Manuela Silva <mmsrs@sky.com>, 2016
 # MS, 2016,2018
 # Nika Shahidian, 2022
 # Rui Ribeiro <info@nau.edu.pt>, 2018-2019
 # Sarina Canelake <sarina@tcril.org>, 2021
 # Waldo Luis Ribeiro, 2016
 # Waldo Luís Ribeiro, 2016
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-01-15 13:36-0500\n"
+"POT-Creation-Date: 2023-04-16 14:36-0400\n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
-"Last-Translator: Nika Shahidian, 2022\n"
-"Language-Team: Portuguese (Portugal) (http://www.transifex.com/open-edx/edx-platform/language/pt_PT/)\n"
+"Last-Translator: Ivo Branco <ivo.branco@fccn.pt>, 2021,2023\n"
+"Language-Team: Portuguese (Portugal) (http://app.transifex.com/open-edx/edx-platform/language/pt_PT/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: pt_PT\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 
 #: openassessment/assessment/api/student_training.py:179
@@ -295,15 +295,15 @@
 msgstr " (Desativado)"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:117
 msgid ""
 "Specify the number of top scoring responses to display after the learner has"
 " submitted a response. Valid numbers are 0 to 99. If the number is 0, the "
 "Top Responses section does not appear to learners."
-msgstr ""
+msgstr "Especificar o número de respostas de pontuação máxima a exibir após o estudante ter submetido uma resposta. Os números válidos são de 0 a 99. Se o número for 0, a secção de respostas de topo não aparece aos estudantes."
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:122
 msgid "When Teams Enabled is set to true, Top Responses will be disabled."
 msgstr "Quando as equipas são definidas como verdadeiras, as respostas principais serão desativadas."
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:129
 msgid "Teams Enabled"
@@ -644,43 +644,43 @@
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_student_training.html:32
 msgid "Add Sample Response"
 msgstr "Adicionar resposta de exemplo"
 
 #: openassessment/templates/openassessmentblock/edit/oa_rubric_reuse.html:4
 msgid "Clone Rubric"
-msgstr ""
+msgstr "Replicar Rubrica"
 
 #: openassessment/templates/openassessmentblock/edit/oa_rubric_reuse.html:7
 msgid ""
 "To clone a rubric from an existing published or unpublished draft, you can "
 "search by the Block ID. Note that cloning is one-way, meaning changes made "
 "after cloning will only affect the rubric being modified, and will not "
 "modify any rubric it was cloned from."
-msgstr ""
+msgstr "Para replicar uma rubrica de um rascunho existente, quer tenha sido publicado ou não, pode pesquisar pelo Bloco ID. Note que a replicação é unidireccional, o que significa que as alterações feitas após a replicação apenas irão afetar a rubrica que está a ser modificada, e não irão modificar a rubrica a partir da qual foi replicada."
 
 #: openassessment/templates/openassessmentblock/edit/oa_rubric_reuse.html:9
 msgid "Block ID For this ORA:"
-msgstr ""
+msgstr "Bloco ID Para este ORA - Open Response Assessment:"
 
 #: openassessment/templates/openassessmentblock/edit/oa_rubric_reuse.html:19
 msgid "Block ID"
-msgstr ""
+msgstr "Bloco ID"
 
 #: openassessment/templates/openassessmentblock/edit/oa_rubric_reuse.html:21
 msgid "No other Open Response Assessments found in course"
-msgstr ""
+msgstr "Nenhumas outras Avaliações de Resposta Aberta encontradas no curso"
 
 #: openassessment/templates/openassessmentblock/edit/oa_rubric_reuse.html:31
 msgid "Clone"
-msgstr ""
+msgstr "Réplica"
 
 #: openassessment/templates/openassessmentblock/edit/oa_rubric_reuse.html:37
 msgid "Rubric Successfully Cloned from Block ID: "
-msgstr ""
+msgstr "Rubrica Replicada com Sucesso a partir do Bloco ID: "
 
 #: openassessment/templates/openassessmentblock/edit/oa_training_example.html:7
 msgid "Scored Response"
 msgstr "Resposta pontuada"
 
 #: openassessment/templates/openassessmentblock/edit/oa_training_example.html:16
 msgid "Response Score"
@@ -906,21 +906,21 @@
 
 #: openassessment/templates/openassessmentblock/instructor_dashboard/oa_listing.html:6
 msgid "Please wait"
 msgstr "Por favor aguarde"
 
 #: openassessment/templates/openassessmentblock/instructor_dashboard/oa_waiting_step_details.html:15
 msgid "Waiting Step Details"
-msgstr ""
+msgstr "Detalhes da Etapa de Espera"
 
 #: openassessment/templates/openassessmentblock/instructor_dashboard/oa_waiting_step_details.html:24
 msgid ""
 "Waiting Step details view is unavailable. This item is not configured for "
 "peer assessments."
-msgstr ""
+msgstr "A visualização dos detalhes da Etapa de Espera não está disponível. Este item não está configurado para avaliação por pares. "
 
 #: openassessment/templates/openassessmentblock/leaderboard/oa_leaderboard_show.html:20
 #, python-format
 msgid "%(num_points)s points"
 msgstr "%(num_points)s pontos"
 
 #: openassessment/templates/openassessmentblock/leaderboard/oa_leaderboard_show.html:24
@@ -1411,15 +1411,15 @@
 "\n"
 "                                      You are currently on Team %(team_name)s. Since you were on Team %(previous_team_name)s\n"
 "                                      when they submitted a response to this assignment, you are seeing Team %(previous_team_name)s’s\n"
 "                                      response and will receive the same grade for this assignment as your former teammates.\n"
 "                                      You will not be part of Team %(team_name)s’s submission for this assignment and will not\n"
 "                                      receive a grade for their submission.\n"
 "                                  "
-msgstr ""
+msgstr "\n                                      Neste momento está na Equipa %(team_name)s. Visto que esteve na Equipa %(previous_team_name)s\n                                      quando submeteram uma resposta a esta tarefa, está a ver a resposta da Equipa %(previous_team_name)s\n                                      e irá receber a mesma classificação dos seus colegas anteriores.\n                                      Não irá fazer parte da submissão da Equipa %(team_name)spara esta tarefa e não irá\n                                      receber uma classificação para a submissão deles.\n                                  "
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:221
 msgid "We could not save your progress"
 msgstr "Não foi possível guardar o seu progresso"
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:228
 msgid "Save your progress"
@@ -1435,15 +1435,15 @@
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:250
 msgid ""
 "\n"
 "                                  Upload files and review files uploaded by you and your teammates below. Be sure to add\n"
 "                                  descriptions to your files to help your teammates identify them.\n"
 "                              "
-msgstr ""
+msgstr "\n                                  Carregue ficheiros e reveja ficheiros carregados por si e pela sua equipa abaixo. Não se esqueça de acrescentar\n                                  descrições aos seus ficheiros para ajudar os seus colegas a identificá-los.\n                              "
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:258
 msgid "We could not upload files"
 msgstr "Não foi possível carregar os ficheiros"
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:264
 msgid "We could not delete files"
@@ -1499,15 +1499,15 @@
 msgstr "Um membro da equipa deve submeter em nome de toda a equipa."
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:316
 msgid ""
 "\n"
 "                  Learn more about team assignments here: (<a target=\"_blank\" href=\"https://support.edx.org/hc/en-us/articles/360000191067-Submit-your-response#h_01FVD8SXM9E5H2DNAG87X25ZHR\">link</a>)\n"
 "                  "
-msgstr ""
+msgstr "\n                  Saiba mais sobre as tarefas da equipa aqui: (<a target=\"_blank\" href=\"https://support.edx.org/hc/en-us/articles/360000191067-Submit-your-response#h_01FVD8SXM9E5H2DNAG87X25ZHR\">link</a>)\n                  "
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:324
 msgid "We could not submit your response"
 msgstr "Não foi possível submeter a sua resposta"
 
 #: openassessment/templates/openassessmentblock/response/oa_response.html:334
 msgid "Submit your response and move to the next step"
@@ -1674,19 +1674,19 @@
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:13
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:71
 msgid "View Assignment Statistics"
 msgstr "Visualizar Estatísticas da Tarefa"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:22
 msgid "Demo the new Grading Experience"
-msgstr ""
+msgstr "Demonstração da nova experiência de classificação"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:26
 msgid "View ORA in Studio"
-msgstr ""
+msgstr "Ver ORA - Open Response Assessment no Studio"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:31
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:69
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:151
 msgid "Close"
 msgstr "Fechar"
 
@@ -2323,25 +2323,25 @@
 #: openassessment/xblock/resolve_dates.py:234
 #, python-brace-format
 msgid "The start date '{start}' cannot be later than the due date '{due}'"
 msgstr "A data de início '{start}' não pode ser posterior à data limite '{due}'"
 
 #: openassessment/xblock/rubric_reuse_mixin.py:62
 msgid "You must specify a block id from which to copy a rubric."
-msgstr ""
+msgstr "Deve especificar um bloco id a partir do qual copiar uma rubrica."
 
 #: openassessment/xblock/rubric_reuse_mixin.py:66
 msgid "Invalid block id."
-msgstr ""
+msgstr "Bloco id inválido."
 
 #: openassessment/xblock/rubric_reuse_mixin.py:72
 #, python-brace-format
 msgid ""
 "No Open Response Assessment found in {course_id} with block id {block_id}"
-msgstr ""
+msgstr "Nenhuma Avaliação de Resposta Aberta encontrada em {course_id} com bloco id {block_id}"
 
 #: openassessment/xblock/self_assessment_mixin.py:142
 msgid "You must submit a response before you can perform a self-assessment."
 msgstr "Deve submeter uma resposta antes de poder realizar uma auto-avaliação."
 
 #: openassessment/xblock/self_assessment_mixin.py:165
 #: openassessment/xblock/self_assessment_mixin.py:173
@@ -2366,31 +2366,31 @@
 
 #: openassessment/xblock/staff_area_mixin.py:71
 msgid "You do not have permission to access ORA staff grading."
 msgstr "Sem permissão para aceder à classificação da equipa de ORA."
 
 #: openassessment/xblock/staff_area_mixin.py:242
 msgid "Pending"
-msgstr ""
+msgstr "Pendente"
 
 #: openassessment/xblock/staff_area_mixin.py:243
 msgid "Complete/Overwritten"
-msgstr ""
+msgstr "Completo/Substituído"
 
 #: openassessment/xblock/staff_area_mixin.py:246
 msgid "Not applicable"
-msgstr ""
+msgstr "Não aplicável"
 
 #: openassessment/xblock/staff_area_mixin.py:247
 msgid "Not submitted"
-msgstr ""
+msgstr "Não submetido"
 
 #: openassessment/xblock/staff_area_mixin.py:248
 msgid "Submitted"
-msgstr ""
+msgstr "Submetido"
 
 #: openassessment/xblock/staff_area_mixin.py:315
 msgid "Error getting learner information."
 msgstr "Erro ao obter informações do estudante."
 
 #: openassessment/xblock/staff_area_mixin.py:358
 msgid "Error loading the checked out learner response."
@@ -2521,21 +2521,21 @@
 
 #: openassessment/xblock/submission_mixin.py:145
 msgid "Multiple submissions are not allowed."
 msgstr "Várias submissões não são permitidas."
 
 #: openassessment/xblock/submission_mixin.py:178
 msgid "Response exceeds maximum allowed size."
-msgstr ""
+msgstr "A resposta excede o tamanho máximo permitido."
 
 #: openassessment/xblock/submission_mixin.py:180
 msgid ""
 "Note: if you have a spellcheck or grammar check browser extension, try "
 "disabling, reloading, and reentering your response before submitting."
-msgstr ""
+msgstr "Nota: se tiver uma verificação ortográfica ou uma extensão de verificação gramatical do navegador, tente desactivar, recarregar, e reentrar a sua resposta antes de submeter."
 
 #: openassessment/xblock/submission_mixin.py:200
 msgid "Submission cannot be empty. Please refresh the page and try again."
 msgstr "A submissão não pode ser vazia. Por favor, atualize a página e tente novamente."
 
 #: openassessment/xblock/submission_mixin.py:210
 msgid "API returned unclassified exception."
```

### Comparing `ora2-5.0.0/openassessment/locale/pt_PT/LC_MESSAGES/djangojs.po` & `ora2-5.0.1/openassessment/locale/pt_PT/LC_MESSAGES/djangojs.po`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # 
 # Translators:
 # Beatriz Magalhães <mbeatrizmagalhaes@gmail.com>, 2016
 # Beatriz Sousa <beatriz.sousa@bridgelk.com>, 2018
 # Cátia Lopes <catia.lopes@bridgelk.com>, 2018
 # Filipa Macieira <filipa.macieira@fccn.pt>, 2021
 # Filipe Boleto <fboleto@gmail.com>, 2015
+# Ivo Branco <ivo.branco@fccn.pt>, 2023
 # Luis Manuel Moreno <luis.moreno@edunext.co>, 2019
 # Manuela Silva <mmsrs@sky.com>, 2016,2018
 # Manuela Silva <mmsrs@sky.com>, 2018
 # Manuela Silva <mmsrs@sky.com>, 2016
 # MS, 2016,2018
 # Nika Shahidian, 2022
 # Nlaranjo <numicola@gmail.com>, 2014
@@ -22,16 +23,16 @@
 # Teresa Guerreiro <t.guerreiro@sapo.pt>, 2014
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-09-13 04:00-0400\n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
-"Last-Translator: Nika Shahidian, 2022\n"
-"Language-Team: Portuguese (Portugal) (http://www.transifex.com/open-edx/edx-platform/language/pt_PT/)\n"
+"Last-Translator: Ivo Branco <ivo.branco@fccn.pt>, 2023\n"
+"Language-Team: Portuguese (Portugal) (http://app.transifex.com/open-edx/edx-platform/language/pt_PT/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: pt_PT\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
@@ -147,25 +148,25 @@
 msgid "Error when looking up username"
 msgstr "Erro ao procurar o nome de utilizador"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:1
 #: openassessment/xblock/static/js/src/oa_server.js:728
 msgid "Failed to clone rubric"
-msgstr ""
+msgstr "Falha na clonagem da rubrica"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:61
 msgid "View and grade responses"
-msgstr ""
+msgstr "Ver e classificar as respostas"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:61
 msgid "Demo the new Grading Experience"
-msgstr ""
+msgstr "Demonstração da nova experiência de classificação"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:97
 msgid "Unit Name"
 msgstr "Título da Unidade"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
@@ -224,15 +225,15 @@
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:162
 msgid "Final Grade Received"
 msgstr "Nota Final Recebida"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:169
 msgid "Staff Grader"
-msgstr ""
+msgstr "Graduador de Pessoal"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:200
 msgid "List of Open Assessments is unavailable"
 msgstr "Lista de Avaliações Abertas não está disponível"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:314
@@ -250,25 +251,25 @@
 #: openassessment/xblock/static/js/src/lms/oa_course_items_listing.js:338
 msgid "Back to Full List"
 msgstr "Voltar à lista completa"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_confirmation_alert.js:5
 msgid "Confirm"
-msgstr ""
+msgstr "Confirmar"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_confirmation_alert.js:7
 msgid "Cancel"
-msgstr ""
+msgstr "Cancelar"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:339
 msgid "Your file has been deleted or path has been changed: "
-msgstr ""
+msgstr "O seu ficheiro foi eliminado ou o caminho foi alterado: "
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:366
 msgid "Status of Your Response"
 msgstr "Estado da sua Resposta"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
@@ -297,15 +298,15 @@
 #: openassessment/xblock/static/js/src/lms/oa_response.js:477
 msgid "Error"
 msgstr "Erro"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:498
 msgid "Confirm Submit Response"
-msgstr ""
+msgstr "Confirmar Submissão da Resposta"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:501
 msgid ""
 "You're about to submit your response for this assignment. After you submit "
 "this response, you can't change it or submit a new response."
 msgstr "Está prestes a submeter a sua resposta para esta tarefa. Depois de a submeter, não é possível alterá-la ou submeter uma nova resposta."
@@ -321,15 +322,15 @@
 "File upload failed: unsupported file type. Only the supported file types can"
 " be uploaded. If you have questions, please reach out to the course team."
 msgstr "Falha no carregamento do ficheiro: tipo de ficheiro não suportado. Apenas os tipos de ficheiros suportados podem ser carregados. Se tiver dúvidas, entre em contato com a equipa de curso."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:601
 msgid "The maximum number files that can be saved is "
-msgstr ""
+msgstr "O número máximo de ficheiros que podem ser guardados é "
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:673
 #: openassessment/xblock/static/js/src/lms/oa_response.js:679
 msgid "Describe "
 msgstr "Descreva "
 
@@ -342,15 +343,15 @@
 #: openassessment/xblock/static/js/src/lms/oa_response.js:693
 msgid "Thumbnail view of "
 msgstr "Visualização em miniatura de "
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:779
 msgid "Confirm Delete Uploaded File"
-msgstr ""
+msgstr "Confirmar exclusão do arquivo enviado"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_response.js:805
 msgid ""
 "Are you sure you want to delete the following file? It cannot be restored.\n"
 "File: "
 msgstr "Tem certeza de que deseja apagar o seguinte ficheiro? Não pode ser restaurado.\nFicheiro: "
@@ -379,15 +380,15 @@
 "This grade will be applied to all members of the team. Do you want to "
 "continue?"
 msgstr "Esta nota será aplicada a todos os membros da equipa. Quer continuar?"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_staff_area.js:218
 msgid "Confirm Grade Team Submission"
-msgstr ""
+msgstr "Confirme o envio da equipe de notas"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
 #: openassessment/xblock/static/js/src/lms/oa_staff_area.js:304
 msgid "Error getting the number of ungraded responses"
 msgstr "Erro ao obter o número de respostas sem classificação"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:369
@@ -407,61 +408,61 @@
 msgid ""
 "If you leave this page without submitting your peer assessment, you will "
 "lose any work you have done."
 msgstr "Caso saia desta página sem submeter o seu teste, irá perder todo o trabalho até aqui realizado."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 msgid "Refresh"
-msgstr ""
+msgstr "Atualizar"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 msgid "Username"
-msgstr ""
+msgstr "Nome de utilizador"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 msgid "Peers Assessed"
-msgstr ""
+msgstr "Colegas avaliados"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 msgid "Peer Responses Received"
-msgstr ""
+msgstr "Respostas de Colegas Recebidas"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 msgid "Time Spent On Current Step"
-msgstr ""
+msgstr "Tempo Gasto Na Etapa Atual"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 msgid "Staff assessment"
-msgstr ""
+msgstr "Avaliação da equipa"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 msgid "Grade Status"
-msgstr ""
+msgstr "Estado da Classificação"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 msgid ""
 "The \"{name}\" problem is configured to require a minimum of {min_grades} "
 "peer grades, and asks to review {min_graded} peers."
-msgstr ""
+msgstr "O problema \"{name}\" está configurado para exigir um mínimo de {min_grades} avaliações de colegas, e pede para rever {min_graded} colegas."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 msgid ""
 "There are currently {stuck_learners} learners in the waiting state, meaning "
 "they have not yet met all requirements for Peer Assessment. "
-msgstr ""
+msgstr "Existem atualmente {stuck_learners} estudantes no estado de espera, o que significa que ainda não cumpriram todos os requisitos para a Avaliação por Colegas. "
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 msgid ""
 "However, {overwritten_count} of these students have received a grade through"
 " the staff grade override tool already."
-msgstr ""
+msgstr "No entanto, {overwritten_count} destes estudantes já receberam uma classificação através da ferramenta de substituição de classificações da equipa."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 msgid "Error while fetching student data."
-msgstr ""
+msgstr "Erro ao ir buscar dados de estudantes."
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:375
 #: openassessment/xblock/static/js/src/lms/oa_base.js:343
 msgid "Unable to load"
 msgstr "Não foi possível carregar"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
@@ -503,28 +504,28 @@
 #: openassessment/xblock/static/js/src/studio/oa_container_item.js:53
 msgid "Not Selected"
 msgstr "Não Selecionado"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_rubric.js:124
 msgid "Problem cloning rubric"
-msgstr ""
+msgstr "Rúbrica de clonagem de problemas"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:100
 msgid "Criterion Added"
 msgstr "Critério Adicionado"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:102
 msgid ""
 "You have added a criterion. You will need to select an option for the "
 "criterion in the Learner Training step. To do this, click the Assessment "
 "Steps tab."
-msgstr ""
+msgstr "Adicionou um critério. Terá de selecionar uma opção para o critério na etapa de Formação do Estudante. Para o fazer, clique no separador Passos de Avaliação."
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:150
 #: openassessment/xblock/static/js/src/studio/oa_edit_listeners.js:186
 msgid "Option Deleted"
 msgstr "Opção eliminada"
 
@@ -576,24 +577,24 @@
 #: openassessment/xblock/static/js/src/studio/oa_edit_settings.js:101
 msgid "The following file types are not allowed: "
 msgstr "Os seguintes tipos de ficheiro não são permitidos: "
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit.js:183
 msgid "Save Unsuccessful"
-msgstr ""
+msgstr "Sem Sucesso ao Guardar"
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit.js:184
 msgid "Errors detected on the following tabs: "
-msgstr ""
+msgstr "Erros detetados nos seguintes separadores: "
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 msgid ""
 "This ORA has already been released. Changes will only affect learners making"
 " new submissions. Existing submissions will not be modified by this change."
-msgstr ""
+msgstr "Esta Questão de Resposta Aberta já foi divulgada. As alterações apenas irão afetar os alunos que fizerem novas submissões. As submissões existentes não serão modificadas por esta alteração."
 
 #: openassessment/xblock/static/dist/openassessment-studio.1ffb8619386559df14f9.js:32
 #: openassessment/xblock/static/js/src/studio/oa_edit.js:318
 msgid "error count: "
-msgstr ""
+msgstr "contagem de erros: "
```

### Comparing `ora2-5.0.0/openassessment/locale/ro/LC_MESSAGES/django.mo` & `ora2-5.0.1/openassessment/locale/ro/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
 "Last-Translator: Bogdan Mateescu, 2018\n"
-"Language-Team: Romanian (http://www.transifex.com/open-edx/edx-platform/"
+"Language-Team: Romanian (http://app.transifex.com/open-edx/edx-platform/"
 "language/ro/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: ro\n"
 "Plural-Forms: nplurals=3; plural=(n==1?0:(((n%100>19)||((n%100==0)&&(n!=0)))?"
 "2:1));\n"
```

### Comparing `ora2-5.0.0/openassessment/locale/ro/LC_MESSAGES/django.po` & `ora2-5.0.1/openassessment/locale/ro/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 # Pinman <bogdan.stefan@outlook.com>, 2014
 # Rares Mihai Popa <raresmihaipopa@gmail.com>, 2015
 # tyby94 <tyby04@gmail.com>, 2014
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-01-15 13:36-0500\n"
+"POT-Creation-Date: 2023-04-30 14:36-0400\n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
 "Last-Translator: Bogdan Mateescu, 2018\n"
-"Language-Team: Romanian (http://www.transifex.com/open-edx/edx-platform/language/ro/)\n"
+"Language-Team: Romanian (http://app.transifex.com/open-edx/edx-platform/language/ro/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: ro\n"
 "Plural-Forms: nplurals=3; plural=(n==1?0:(((n%100>19)||((n%100==0)&&(n!=0)))?2:1));\n"
 
 #: openassessment/assessment/api/student_training.py:179
```

### Comparing `ora2-5.0.0/openassessment/locale/ro/LC_MESSAGES/djangojs.mo` & `ora2-5.0.1/openassessment/locale/ro/LC_MESSAGES/djangojs.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Manuel, 2021\n"
-"Language-Team: Romanian (http://www.transifex.com/open-edx/edx-platform/"
+"Language-Team: Romanian (http://app.transifex.com/open-edx/edx-platform/"
 "language/ro/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: ro\n"
 "Plural-Forms: nplurals=3; plural=(n==1?0:(((n%100>19)||((n%100==0)&&(n!=0)))?"
 "2:1));\n"
```

### Comparing `ora2-5.0.0/openassessment/locale/ro/LC_MESSAGES/djangojs.po` & `ora2-5.0.1/openassessment/locale/ro/LC_MESSAGES/djangojs.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-09-13 04:00-0400\n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Manuel, 2021\n"
-"Language-Team: Romanian (http://www.transifex.com/open-edx/edx-platform/language/ro/)\n"
+"Language-Team: Romanian (http://app.transifex.com/open-edx/edx-platform/language/ro/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: ro\n"
 "Plural-Forms: nplurals=3; plural=(n==1?0:(((n%100>19)||((n%100==0)&&(n!=0)))?2:1));\n"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
```

### Comparing `ora2-5.0.0/openassessment/locale/ru/LC_MESSAGES/django.mo` & `ora2-5.0.1/openassessment/locale/ru/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
 "Last-Translator: Dmitry Broover, 2022\n"
-"Language-Team: Russian (http://www.transifex.com/open-edx/edx-platform/"
+"Language-Team: Russian (http://app.transifex.com/open-edx/edx-platform/"
 "language/ru/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: ru\n"
 "Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || "
```

### Comparing `ora2-5.0.0/openassessment/locale/ru/LC_MESSAGES/django.po` & `ora2-5.0.1/openassessment/locale/ru/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -24,18 +24,18 @@
 # YummyTranslations Edx <yummytranslations.edx@gmail.com>, 2015
 # Pavel Zamyshliaev, 2014
 # Виктор, 2022
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-01-15 13:36-0500\n"
+"POT-Creation-Date: 2023-04-30 14:36-0400\n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
 "Last-Translator: Dmitry Broover, 2022\n"
-"Language-Team: Russian (http://www.transifex.com/open-edx/edx-platform/language/ru/)\n"
+"Language-Team: Russian (http://app.transifex.com/open-edx/edx-platform/language/ru/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: ru\n"
 "Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || (n%100>=11 && n%100<=14)? 2 : 3);\n"
 
 #: openassessment/assessment/api/student_training.py:179
```

### Comparing `ora2-5.0.0/openassessment/locale/ru/LC_MESSAGES/djangojs.mo` & `ora2-5.0.1/openassessment/locale/ru/LC_MESSAGES/djangojs.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: ashed <craysy@gmail.com>, 2022\n"
-"Language-Team: Russian (http://www.transifex.com/open-edx/edx-platform/"
+"Language-Team: Russian (http://app.transifex.com/open-edx/edx-platform/"
 "language/ru/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: ru\n"
 "Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || "
```

### Comparing `ora2-5.0.0/openassessment/locale/ru/LC_MESSAGES/djangojs.po` & `ora2-5.0.1/openassessment/locale/ru/LC_MESSAGES/djangojs.po`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-09-13 04:00-0400\n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: ashed <craysy@gmail.com>, 2022\n"
-"Language-Team: Russian (http://www.transifex.com/open-edx/edx-platform/language/ru/)\n"
+"Language-Team: Russian (http://app.transifex.com/open-edx/edx-platform/language/ru/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: ru\n"
 "Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || (n%100>=11 && n%100<=14)? 2 : 3);\n"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
```

### Comparing `ora2-5.0.0/openassessment/locale/sk/LC_MESSAGES/djangojs.mo` & `ora2-5.0.1/openassessment/locale/sk/LC_MESSAGES/djangojs.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Vladimír Záhradník <vladimir@zahradnik.io>, 2015\n"
-"Language-Team: Slovak (http://www.transifex.com/open-edx/edx-platform/"
+"Language-Team: Slovak (http://app.transifex.com/open-edx/edx-platform/"
 "language/sk/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: sk\n"
 "Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n "
 ">= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
```

### Comparing `ora2-5.0.0/openassessment/locale/sk/LC_MESSAGES/djangojs.po` & `ora2-5.0.1/openassessment/locale/sk/LC_MESSAGES/djangojs.po`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-09-13 04:00-0400\n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Vladimír Záhradník <vladimir@zahradnik.io>, 2015\n"
-"Language-Team: Slovak (http://www.transifex.com/open-edx/edx-platform/language/sk/)\n"
+"Language-Team: Slovak (http://app.transifex.com/open-edx/edx-platform/language/sk/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: sk\n"
 "Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n >= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
```

### Comparing `ora2-5.0.0/openassessment/locale/sq/LC_MESSAGES/django.mo` & `ora2-5.0.1/openassessment/locale/sq/LC_MESSAGES/django.mo`

 * *Files 5% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
 "Last-Translator: Faton Nuha <faton11@live.com>, 2014-2016\n"
-"Language-Team: Albanian (http://www.transifex.com/open-edx/edx-platform/"
+"Language-Team: Albanian (http://app.transifex.com/open-edx/edx-platform/"
 "language/sq/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: sq\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `ora2-5.0.0/openassessment/locale/sq/LC_MESSAGES/django.po` & `ora2-5.0.1/openassessment/locale/sq/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 # 
 # Translators:
 # Faton Nuha <faton11@live.com>, 2014-2016
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-01-15 13:36-0500\n"
+"POT-Creation-Date: 2023-04-30 14:36-0400\n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
 "Last-Translator: Faton Nuha <faton11@live.com>, 2014-2016\n"
-"Language-Team: Albanian (http://www.transifex.com/open-edx/edx-platform/language/sq/)\n"
+"Language-Team: Albanian (http://app.transifex.com/open-edx/edx-platform/language/sq/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: sq\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: openassessment/assessment/api/student_training.py:179
```

### Comparing `ora2-5.0.0/openassessment/locale/sq/LC_MESSAGES/djangojs.mo` & `ora2-5.0.1/openassessment/locale/sq/LC_MESSAGES/djangojs.mo`

 * *Files 15% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Faton Nuha <faton11@live.com>, 2014,2016\n"
-"Language-Team: Albanian (http://www.transifex.com/open-edx/edx-platform/"
+"Language-Team: Albanian (http://app.transifex.com/open-edx/edx-platform/"
 "language/sq/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: sq\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `ora2-5.0.0/openassessment/locale/sq/LC_MESSAGES/djangojs.po` & `ora2-5.0.1/openassessment/locale/sq/LC_MESSAGES/djangojs.po`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-09-13 04:00-0400\n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Faton Nuha <faton11@live.com>, 2014,2016\n"
-"Language-Team: Albanian (http://www.transifex.com/open-edx/edx-platform/language/sq/)\n"
+"Language-Team: Albanian (http://app.transifex.com/open-edx/edx-platform/language/sq/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: sq\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
```

### Comparing `ora2-5.0.0/openassessment/locale/sw_KE/LC_MESSAGES/django.mo` & `ora2-5.0.1/openassessment/locale/sw_KE/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
 "Last-Translator: YAHAYA MWAVURIZI <translations_1@camara.ie>, 2017\n"
-"Language-Team: Swahili (Kenya) (http://www.transifex.com/open-edx/edx-"
+"Language-Team: Swahili (Kenya) (http://app.transifex.com/open-edx/edx-"
 "platform/language/sw_KE/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: sw_KE\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `ora2-5.0.0/openassessment/locale/sw_KE/LC_MESSAGES/django.po` & `ora2-5.0.1/openassessment/locale/sw_KE/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 # swaleh amin <mkupuofirstnameswaleh@yahoo.com>, 2016
 # swalehe manture <translations_3@camara.ie>, 2017
 # YAHAYA MWAVURIZI <translations_1@camara.ie>, 2017
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-01-15 13:36-0500\n"
+"POT-Creation-Date: 2023-04-30 14:36-0400\n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
 "Last-Translator: YAHAYA MWAVURIZI <translations_1@camara.ie>, 2017\n"
-"Language-Team: Swahili (Kenya) (http://www.transifex.com/open-edx/edx-platform/language/sw_KE/)\n"
+"Language-Team: Swahili (Kenya) (http://app.transifex.com/open-edx/edx-platform/language/sw_KE/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: sw_KE\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: openassessment/assessment/api/student_training.py:179
```

### Comparing `ora2-5.0.0/openassessment/locale/sw_KE/LC_MESSAGES/djangojs.mo` & `ora2-5.0.1/openassessment/locale/sw_KE/LC_MESSAGES/djangojs.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Innocent Masue <translations_7@camara.ie>, 2017\n"
-"Language-Team: Swahili (Kenya) (http://www.transifex.com/open-edx/edx-"
+"Language-Team: Swahili (Kenya) (http://app.transifex.com/open-edx/edx-"
 "platform/language/sw_KE/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: sw_KE\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `ora2-5.0.0/openassessment/locale/sw_KE/LC_MESSAGES/djangojs.po` & `ora2-5.0.1/openassessment/locale/sw_KE/LC_MESSAGES/djangojs.po`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-09-13 04:00-0400\n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Innocent Masue <translations_7@camara.ie>, 2017\n"
-"Language-Team: Swahili (Kenya) (http://www.transifex.com/open-edx/edx-platform/language/sw_KE/)\n"
+"Language-Team: Swahili (Kenya) (http://app.transifex.com/open-edx/edx-platform/language/sw_KE/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: sw_KE\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
```

### Comparing `ora2-5.0.0/openassessment/locale/th/LC_MESSAGES/django.mo` & `ora2-5.0.1/openassessment/locale/th/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
 "Last-Translator: Noppadol Choti <noppadol@thaicyberu.go.th>, 2019\n"
-"Language-Team: Thai (http://www.transifex.com/open-edx/edx-platform/language/"
+"Language-Team: Thai (http://app.transifex.com/open-edx/edx-platform/language/"
 "th/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: th\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
```

### Comparing `ora2-5.0.0/openassessment/locale/th/LC_MESSAGES/django.po` & `ora2-5.0.1/openassessment/locale/th/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 # ormbook ohno <ormbook@gmail.com>, 2016
 # Sira Nokyoongtong <gumaraa@gmail.com>, 2014
 # Sorathan Chaturapruek <tummykung@gmail.com>, 2015
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-01-15 13:36-0500\n"
+"POT-Creation-Date: 2023-04-30 14:36-0400\n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
 "Last-Translator: Noppadol Choti <noppadol@thaicyberu.go.th>, 2019\n"
-"Language-Team: Thai (http://www.transifex.com/open-edx/edx-platform/language/th/)\n"
+"Language-Team: Thai (http://app.transifex.com/open-edx/edx-platform/language/th/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: th\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 #: openassessment/assessment/api/student_training.py:179
```

### Comparing `ora2-5.0.0/openassessment/locale/th/LC_MESSAGES/djangojs.mo` & `ora2-5.0.1/openassessment/locale/th/LC_MESSAGES/djangojs.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Jirayu Chamamahattana <mman2x@gmail.com>, 2015\n"
-"Language-Team: Thai (http://www.transifex.com/open-edx/edx-platform/language/"
+"Language-Team: Thai (http://app.transifex.com/open-edx/edx-platform/language/"
 "th/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: th\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
```

### Comparing `ora2-5.0.0/openassessment/locale/th/LC_MESSAGES/djangojs.po` & `ora2-5.0.1/openassessment/locale/th/LC_MESSAGES/djangojs.po`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-09-13 04:00-0400\n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Jirayu Chamamahattana <mman2x@gmail.com>, 2015\n"
-"Language-Team: Thai (http://www.transifex.com/open-edx/edx-platform/language/th/)\n"
+"Language-Team: Thai (http://app.transifex.com/open-edx/edx-platform/language/th/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: th\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
```

### Comparing `ora2-5.0.0/openassessment/locale/tr_TR/LC_MESSAGES/django.mo` & `ora2-5.0.1/openassessment/locale/tr_TR/LC_MESSAGES/django.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
-"Last-Translator: Ali Işıngör <ali@artistanbul.io>, 2018-2022\n"
-"Language-Team: Turkish (Turkey) (http://www.transifex.com/open-edx/edx-"
+"Last-Translator: Ali Işıngör <ali@artistanbul.io>, 2018-2023\n"
+"Language-Team: Turkish (Turkey) (http://app.transifex.com/open-edx/edx-"
 "platform/language/tr_TR/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: tr_TR\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
@@ -519,14 +519,17 @@
 
 msgid "Criterion {number}: {label}"
 msgstr "Ölçüt {number}: {label}"
 
 msgid "Custom File Types"
 msgstr "Özel Dosya Türleri"
 
+msgid "Date/Time Final Score Given"
+msgstr "Final Notu Verilme Tarihi/Zamanı"
+
 msgid "Dates"
 msgstr "Tarih"
 
 msgid "Default Feedback Text"
 msgstr "Varsayılan Geri Bildirim Metni"
 
 msgid "Demo the new Grading Experience"
@@ -595,14 +598,30 @@
 
 msgid "Error retrieving upload URL."
 msgstr "URL yükleme alırken hata"
 
 msgid "Error updating XBlock configuration"
 msgstr "XBlock yapılandırması güncellenirken hata"
 
+msgid "Error: Text Response and File Upload Response cannot both be disabled"
+msgstr ""
+"Hata: Metin ve Dosya Yükleme yanıtlarının ikisi birden devre dışı bırakılamaz"
+
+msgid ""
+"Error: When File Upload Response is disabled, Text Response must be Required"
+msgstr ""
+"Hata: Dosya Yükleme Yanıtı devre dışı bırakıldığında, Metin Yanıtı Gerekli "
+"Olmalıdır"
+
+msgid ""
+"Error: When Text Response is disabled, File Upload Response must be Required"
+msgstr ""
+"Hata: Metin Yanıtı devre dışı bırakıldığında, Dosya Yükleme Yanıtı Gerekli "
+"Olmalıdır"
+
 msgid "Example {example_number} has a validation error: {error}"
 msgstr "Örnek {example_number} 'de bir doğrulama hatası var: {error}"
 
 msgid "Example {example_number} has an extra option for \"{criterion_name}\""
 msgstr ""
 "{example_number} numaralı örnek \"{criterion_name}\" ekstra seçeneğe sahip."
 
@@ -678,14 +697,17 @@
 
 msgid "Final Score Possible"
 msgstr "Alınabilir Final Notu"
 
 msgid "Give this learner a grade using the problem's rubric."
 msgstr "Problem rubrikini kullanarak bu öğrenciye not ver."
 
+msgid "Give this team a grade using the problem's rubric."
+msgstr "Problemin dereceli  puanlama anahtarını kullanarak bu takıma not ver."
+
 msgid "Grade Available Responses"
 msgstr "Notlandırılabilir Yanıtlar"
 
 msgid "Graded By"
 msgstr "Tarafından Notlandırıldı"
 
 msgid "I disagree with one or more of the peer assessments of my response."
@@ -727,14 +749,17 @@
 
 msgid "Incomplete"
 msgstr "Eksik"
 
 msgid "Instructions Unavailable"
 msgstr "Komutlar Ulaşılabilir Değil"
 
+msgid "Invalid block id."
+msgstr "Geçersiz block kimliği."
+
 msgid "Item ID"
 msgstr "Öğe Kimliği"
 
 msgid "Leaderboard number is invalid."
 msgstr "Afiş sayısı geçersiz."
 
 msgid "Learn to Assess Responses"
@@ -811,14 +836,22 @@
 
 msgid "Not applicable"
 msgstr "Uygulanamaz"
 
 msgid "Not submitted"
 msgstr "Gönderilmedi"
 
+msgid ""
+"Note: if you have a spellcheck or grammar check browser extension, try "
+"disabling, reloading, and reentering your response before submitting."
+msgstr ""
+"Not: Bir yazım denetimi veya dilbilgisi denetimi tarayıcı uzantınız varsa "
+"yanıtınızı göndermeden önce uzantıyı devre dışı bırakmayı, sayfayı yeniden "
+"yüklemeyi ve yeniden girmeyi deneyin."
+
 msgid "Open Response Assessment"
 msgstr "Açık Yanıt Değerlendirmesi"
 
 msgid "Option"
 msgstr "Seçenek"
 
 msgid "Option Explanation"
@@ -955,14 +988,17 @@
 
 msgid "Response Start Date"
 msgstr "Cevaplama için Başlangıç Tarihi"
 
 msgid "Response Start Time"
 msgstr "Cevaplama için Başlangıç Zamanı"
 
+msgid "Response exceeds maximum allowed size."
+msgstr "Yanıt, izin verilen maksimum boyutu aşıyor."
+
 msgid "Response total"
 msgstr "Toplam cevap"
 
 msgid "Rubric"
 msgstr "Rubrik"
 
 msgid ""
@@ -1018,25 +1054,35 @@
 
 msgid "Self Assessment Deadlines"
 msgstr "Öz Değerlendirme Son Tarihleri"
 
 msgid "Settings"
 msgstr "Ayarlar"
 
+msgid "Show Rubric During Response"
+msgstr "Yanıt Sırasında Dereceli Puanlama Anahtarını Göster"
+
 msgid "Some comments I received were inappropriate."
 msgstr "Aldığım bazı yorumlar uygunsuzdu."
 
 msgid ""
 "Specify whether learners are able to upload files as a part of their "
 "response."
 msgstr ""
 "Öğrencilerin yanıtlarının bir parçası olarak dosya yükleyip "
 "yükleyemeyeceklerini belirtin."
 
 msgid ""
+"Specify whether learners can see the rubric while they are working on their "
+"response."
+msgstr ""
+"Öğrencilerin yanıtları üzerinde çalışırken dereceli puanlama anahtarını "
+"görüp göremeyeceklerini belirtin."
+
+msgid ""
 "Specify whether learners can upload more than one file. This has no effect "
 "if File Uploads Response is set to None. This is automatically set to True "
 "for Team Assignments. "
 msgstr ""
 "Öğrencilerin birden fazla dosya yükleyip yükleyemeyeceğini belirtin. Dosya "
 "Yükleme Yanıtı None olarak ayarlanırsa bunun hiçbir etkisi yoktur. Bu, Takım "
 "Görevleri için otomatik olarak True olarak ayarlanır."
@@ -1166,19 +1212,28 @@
 msgid ""
 "The assessment type cannot be changed after the problem has been released."
 msgstr "Problem yayımlandıktan sonra değerlendirme tipi değiştirilemez."
 
 msgid "The date and time when all peer assessments must be complete."
 msgstr "Tüm akran değerlendirmelerinin tamamlanması gereken tarih ve saat."
 
+msgid "The date and time when all self assessments must be complete."
+msgstr ""
+"Tüm kendi kendine değerlendirmelerin tamamlanması gereken tarih ve saat."
+
 msgid "The date and time when learners can begin assessing peer responses."
 msgstr ""
 "Öğrencilerin akran yanıtlarını değerlendirmeye başlayabilecekleri tarih ve "
 "saat."
 
+msgid "The date and time when learners can begin assessing their responses."
+msgstr ""
+"Öğrencilerin kendi yanıtlarını değerlendirmeye başlayabilecekleri tarih ve "
+"saat."
+
 msgid "The date and time when learners can begin submitting responses."
 msgstr "Öğrencilerin cevaplarını yüklemeye başladığı zamanki tarih ve zaman."
 
 msgid "The date and time when learners can no longer submit responses."
 msgstr "Öğrencilerin artık yanıtlarını yükleyemediği tarih ve zaman."
 
 msgid "The display name for this component."
@@ -1382,14 +1437,17 @@
 
 msgid "View / Add Sample Responses"
 msgstr "Örnek Cevap Görüntüle/Ekle"
 
 msgid "View Assignment Statistics"
 msgstr "Görev İstatistiklerini Görüntüle"
 
+msgid "View ORA in Studio"
+msgstr "Studio'da ORA'yı Görüntüle"
+
 msgid "View Options & Configuration"
 msgstr "Ayarlar & Yapılandırmayı Görüntüle"
 
 msgid "View the files associated with this submission:"
 msgstr "Bu gönderimle ilişkili dosyaları göster:"
 
 msgid "Waiting Step Details"
@@ -1569,18 +1627,34 @@
 
 msgid "Your staff assessment could not be submitted."
 msgstr "Personel değerlendirmeniz gönderilemedi."
 
 msgid "Your submission has been cancelled."
 msgstr "Yüklemeniz iptal edildi."
 
+msgid ""
+"Your submission has been cancelled. You will receive a grade of zero unless "
+"course staff resets your assessment to allow you to resubmit a response."
+msgstr ""
+"Gönderiminiz iptal edildi. Ders personeli yeniden yanıt göndermenize izin "
+"vermek için değerlendirmenizi sıfırlamadığı sürece sıfır notu alacaksınız."
+
 msgid "Your submission was cancelled. "
 msgstr "Gönderiminiz iptal edildi."
 
 msgid "Your team assessment could not be submitted."
 msgstr "Takım değerlendirmeniz gönderilemedi."
 
+msgid ""
+"Your team’s submission has been cancelled. Your team will receive a grade of "
+"zero unless course staff resets your assessment to allow the team to "
+"resubmit a response."
+msgstr ""
+"Takımınızın gönderimi iptal edildi. Ders personeli, takımın yeniden yanıt "
+"göndermesine izin vermek için değerlendirmenizi sıfırlamadığı sürece "
+"takımınız sıfır notu alacaktır."
+
 msgid "options_selected must be a dictionary"
 msgstr "seçilmiş_seçenekler sözlük olmalıdır"
 
 msgid "points"
 msgstr "puan"
```

### Comparing `ora2-5.0.0/openassessment/locale/tr_TR/LC_MESSAGES/django.po` & `ora2-5.0.1/openassessment/locale/tr_TR/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # #-#-#-#-#  django.po (edx-ora2)  #-#-#-#-#
 # edX translation file
 # Copyright (C) 2018 edX
 # This file is distributed under the GNU AFFERO GENERAL PUBLIC LICENSE.
 # 
 # Translators:
 # Adem Özgür <admozgur@gmail.com>, 2015
-# Ali Işıngör <ali@artistanbul.io>, 2018-2022
+# Ali Işıngör <ali@artistanbul.io>, 2018-2023
 # ali selek <aliselek01@gmail.com>, 2015
 # Ayhan Aksoy <aksoyayhan1@gmail.com>, 2015
 # Emrah Emirtekin <eemirtekin@gmail.com>, 2015
 # 00f403b44f997af1c6042d2ed7dd6401_3a00d02 <b14bfe84763aae05bab3d218a58936aa_222192>, 2014
 # Gencay <gencayerdem@hotmail.com>, 2015
 # Hakan Şenel <hgsenel@gmail.com>, 2015
 # İlker IŞIK <m.ilkerisik@hotmail.com>, 2015
@@ -17,18 +17,18 @@
 # msare <mervesareakin@gmail.com>, 2014
 # 169685c64da20f8565d5bb4b5fa14388_0122c8a <d6cdb6a8d55668108fbee6af67afa0d1_255939>, 2015
 # Tevfik Bagcivan <tevfik.bagcivan@gmail.com>, 2016
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-01-15 13:36-0500\n"
+"POT-Creation-Date: 2023-04-23 14:36-0400\n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
-"Last-Translator: Ali Işıngör <ali@artistanbul.io>, 2018-2022\n"
-"Language-Team: Turkish (Turkey) (http://www.transifex.com/open-edx/edx-platform/language/tr_TR/)\n"
+"Last-Translator: Ali Işıngör <ali@artistanbul.io>, 2018-2023\n"
+"Language-Team: Turkish (Turkey) (http://app.transifex.com/open-edx/edx-platform/language/tr_TR/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: tr_TR\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
 #: openassessment/assessment/api/student_training.py:179
@@ -126,15 +126,15 @@
 
 #: openassessment/data.py:922
 msgid "Assessment Scored At"
 msgstr ""
 
 #: openassessment/data.py:923
 msgid "Date/Time Final Score Given"
-msgstr ""
+msgstr "Final Notu Verilme Tarihi/Zamanı"
 
 #: openassessment/data.py:924
 msgid "Final Score Earned"
 msgstr "Alınan Final Notu"
 
 #: openassessment/data.py:925
 msgid "Final Score Possible"
@@ -313,21 +313,21 @@
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:141
 msgid "Select Team-Set"
 msgstr "Takım Yapılandırması Seçin"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:155
 msgid "Show Rubric During Response"
-msgstr ""
+msgstr "Yanıt Sırasında Dereceli Puanlama Anahtarını Göster"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html:162
 msgid ""
 "Specify whether learners can see the rubric while they are working on their "
 "response."
-msgstr ""
+msgstr "Öğrencilerin yanıtları üzerinde çalışırken dereceli puanlama anahtarını görüp göremeyeceklerini belirtin."
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html:6
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info.html:122
 #: openassessment/templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html:25
 msgid "Criterion"
 msgstr "Ölçüt"
 
@@ -597,19 +597,19 @@
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment_schedule.html:5
 msgid "Self Assessment Deadlines"
 msgstr "Öz Değerlendirme Son Tarihleri"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment_schedule.html:27
 msgid "The date and time when learners can begin assessing their responses."
-msgstr ""
+msgstr "Öğrencilerin kendi yanıtlarını değerlendirmeye başlayabilecekleri tarih ve saat."
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment_schedule.html:48
 msgid "The date and time when all self assessments must be complete."
-msgstr ""
+msgstr "Tüm kendi kendine değerlendirmelerin tamamlanması gereken tarih ve saat."
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_staff_assessment.html:8
 msgid "Step: Staff Assessment"
 msgstr "Aşama: Personel Değerlendirme"
 
 #: openassessment/templates/openassessmentblock/edit/oa_edit_staff_assessment.html:12
 msgid ""
@@ -933,21 +933,21 @@
 msgstr "Bu görevin tüm adımlarını tamamladıktan sonra, kişilerden gelen en yüksek puan alan cevapları görebilirsiniz."
 
 #: openassessment/templates/openassessmentblock/message/oa_message_cancelled.html:8
 msgid ""
 "Your team’s submission has been cancelled. Your team will receive a grade of"
 " zero unless course staff resets your assessment to allow the team to "
 "resubmit a response."
-msgstr ""
+msgstr "Takımınızın gönderimi iptal edildi. Ders personeli, takımın yeniden yanıt göndermesine izin vermek için değerlendirmenizi sıfırlamadığı sürece takımınız sıfır notu alacaktır."
 
 #: openassessment/templates/openassessmentblock/message/oa_message_cancelled.html:10
 msgid ""
 "Your submission has been cancelled. You will receive a grade of zero unless "
 "course staff resets your assessment to allow you to resubmit a response."
-msgstr ""
+msgstr "Gönderiminiz iptal edildi. Ders personeli yeniden yanıt göndermenize izin vermek için değerlendirmenizi sıfırlamadığı sürece sıfır notu alacaksınız."
 
 #: openassessment/templates/openassessmentblock/message/oa_message_closed.html:8
 msgid ""
 "This task is not yet available. Check back to complete the assignment once "
 "this section has opened."
 msgstr "Bu görev henüz mevcut değil. Bu bölüm açıldığında görevi tamamlamak için tekrar kontrol edin."
 
@@ -1675,15 +1675,15 @@
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:22
 msgid "Demo the new Grading Experience"
 msgstr "Yeni Notlandırma Deneyimi demosu"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:26
 msgid "View ORA in Studio"
-msgstr ""
+msgstr "Studio'da ORA'yı Görüntüle"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:31
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:69
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html:151
 msgid "Close"
 msgstr "Kapat"
 
@@ -1739,15 +1739,15 @@
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners.html:7
 msgid "Staff Assessment"
 msgstr "Personel Değerlendirmesi"
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html:14
 msgid "Give this team a grade using the problem's rubric."
-msgstr ""
+msgstr "Problemin dereceli  puanlama anahtarını kullanarak bu takıma not ver."
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html:16
 msgid "Give this learner a grade using the problem's rubric."
 msgstr "Problem rubrikini kullanarak bu öğrenciye not ver."
 
 #: openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html:26
 #, python-format
@@ -2323,15 +2323,15 @@
 
 #: openassessment/xblock/rubric_reuse_mixin.py:62
 msgid "You must specify a block id from which to copy a rubric."
 msgstr ""
 
 #: openassessment/xblock/rubric_reuse_mixin.py:66
 msgid "Invalid block id."
-msgstr ""
+msgstr "Geçersiz block kimliği."
 
 #: openassessment/xblock/rubric_reuse_mixin.py:72
 #, python-brace-format
 msgid ""
 "No Open Response Assessment found in {course_id} with block id {block_id}"
 msgstr ""
 
@@ -2482,25 +2482,25 @@
 #: openassessment/xblock/studio_mixin.py:224
 #: openassessment/xblock/studio_mixin.py:236
 msgid "Error updating XBlock configuration"
 msgstr "XBlock yapılandırması güncellenirken hata"
 
 #: openassessment/xblock/studio_mixin.py:241
 msgid "Error: Text Response and File Upload Response cannot both be disabled"
-msgstr ""
+msgstr "Hata: Metin ve Dosya Yükleme yanıtlarının ikisi birden devre dışı bırakılamaz"
 
 #: openassessment/xblock/studio_mixin.py:245
 msgid ""
 "Error: When Text Response is disabled, File Upload Response must be Required"
-msgstr ""
+msgstr "Hata: Metin Yanıtı devre dışı bırakıldığında, Dosya Yükleme Yanıtı Gerekli Olmalıdır"
 
 #: openassessment/xblock/studio_mixin.py:248
 msgid ""
 "Error: When File Upload Response is disabled, Text Response must be Required"
-msgstr ""
+msgstr "Hata: Dosya Yükleme Yanıtı devre dışı bırakıldığında, Metin Yanıtı Gerekli Olmalıdır"
 
 #: openassessment/xblock/studio_mixin.py:272
 #, python-brace-format
 msgid "Validation error: {error}"
 msgstr "Doğrulama hatası: {error}"
 
 #: openassessment/xblock/studio_mixin.py:303
@@ -2517,21 +2517,21 @@
 
 #: openassessment/xblock/submission_mixin.py:145
 msgid "Multiple submissions are not allowed."
 msgstr "Çoklu gönderimlere izin verilmez."
 
 #: openassessment/xblock/submission_mixin.py:178
 msgid "Response exceeds maximum allowed size."
-msgstr ""
+msgstr "Yanıt, izin verilen maksimum boyutu aşıyor."
 
 #: openassessment/xblock/submission_mixin.py:180
 msgid ""
 "Note: if you have a spellcheck or grammar check browser extension, try "
 "disabling, reloading, and reentering your response before submitting."
-msgstr ""
+msgstr "Not: Bir yazım denetimi veya dilbilgisi denetimi tarayıcı uzantınız varsa yanıtınızı göndermeden önce uzantıyı devre dışı bırakmayı, sayfayı yeniden yüklemeyi ve yeniden girmeyi deneyin."
 
 #: openassessment/xblock/submission_mixin.py:200
 msgid "Submission cannot be empty. Please refresh the page and try again."
 msgstr ""
 
 #: openassessment/xblock/submission_mixin.py:210
 msgid "API returned unclassified exception."
```

### Comparing `ora2-5.0.0/openassessment/locale/tr_TR/LC_MESSAGES/djangojs.mo` & `ora2-5.0.1/openassessment/locale/tr_TR/LC_MESSAGES/djangojs.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Ali Işıngör <ali@artistanbul.io>, 2018,2020-2022\n"
-"Language-Team: Turkish (Turkey) (http://www.transifex.com/open-edx/edx-"
+"Language-Team: Turkish (Turkey) (http://app.transifex.com/open-edx/edx-"
 "platform/language/tr_TR/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: tr_TR\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
```

### Comparing `ora2-5.0.0/openassessment/locale/tr_TR/LC_MESSAGES/djangojs.po` & `ora2-5.0.1/openassessment/locale/tr_TR/LC_MESSAGES/djangojs.po`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-09-13 04:00-0400\n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Ali Işıngör <ali@artistanbul.io>, 2018,2020-2022\n"
-"Language-Team: Turkish (Turkey) (http://www.transifex.com/open-edx/edx-platform/language/tr_TR/)\n"
+"Language-Team: Turkish (Turkey) (http://app.transifex.com/open-edx/edx-platform/language/tr_TR/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: tr_TR\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
```

### Comparing `ora2-5.0.0/openassessment/locale/uk/LC_MESSAGES/django.mo` & `ora2-5.0.1/openassessment/locale/uk/LC_MESSAGES/django.mo`

 * *Files 5% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
 "Last-Translator: Danylo Shcherbak <danylo.shcherbak@raccoongang.com>, 2021\n"
-"Language-Team: Ukrainian (http://www.transifex.com/open-edx/edx-platform/"
+"Language-Team: Ukrainian (http://app.transifex.com/open-edx/edx-platform/"
 "language/uk/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: uk\n"
 "Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != "
 "11 ? 0 : n % 1 == 0 && n % 10 >= 2 && n % 10 <= 4 && (n % 100 < 12 || n % "
```

### Comparing `ora2-5.0.0/openassessment/locale/uk/LC_MESSAGES/django.po` & `ora2-5.0.1/openassessment/locale/uk/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -18,18 +18,18 @@
 # Tanya Korshun, 2014
 # Zoriana Zaiats, 2015
 # Юлия, 2015
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-01-15 13:36-0500\n"
+"POT-Creation-Date: 2023-04-30 14:36-0400\n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
 "Last-Translator: Danylo Shcherbak <danylo.shcherbak@raccoongang.com>, 2021\n"
-"Language-Team: Ukrainian (http://www.transifex.com/open-edx/edx-platform/language/uk/)\n"
+"Language-Team: Ukrainian (http://app.transifex.com/open-edx/edx-platform/language/uk/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: uk\n"
 "Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != 11 ? 0 : n % 1 == 0 && n % 10 >= 2 && n % 10 <= 4 && (n % 100 < 12 || n % 100 > 14) ? 1 : n % 1 == 0 && (n % 10 ==0 || (n % 10 >=5 && n % 10 <=9) || (n % 100 >=11 && n % 100 <=14 )) ? 2: 3);\n"
 
 #: openassessment/assessment/api/student_training.py:179
```

### Comparing `ora2-5.0.0/openassessment/locale/uk/LC_MESSAGES/djangojs.mo` & `ora2-5.0.1/openassessment/locale/uk/LC_MESSAGES/djangojs.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Danylo Shcherbak <danylo.shcherbak@raccoongang.com>, 2021\n"
-"Language-Team: Ukrainian (http://www.transifex.com/open-edx/edx-platform/"
+"Language-Team: Ukrainian (http://app.transifex.com/open-edx/edx-platform/"
 "language/uk/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: uk\n"
 "Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != "
 "11 ? 0 : n % 1 == 0 && n % 10 >= 2 && n % 10 <= 4 && (n % 100 < 12 || n % "
```

### Comparing `ora2-5.0.0/openassessment/locale/uk/LC_MESSAGES/djangojs.po` & `ora2-5.0.1/openassessment/locale/uk/LC_MESSAGES/djangojs.po`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-09-13 04:00-0400\n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Danylo Shcherbak <danylo.shcherbak@raccoongang.com>, 2021\n"
-"Language-Team: Ukrainian (http://www.transifex.com/open-edx/edx-platform/language/uk/)\n"
+"Language-Team: Ukrainian (http://app.transifex.com/open-edx/edx-platform/language/uk/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: uk\n"
 "Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != 11 ? 0 : n % 1 == 0 && n % 10 >= 2 && n % 10 <= 4 && (n % 100 < 12 || n % 100 > 14) ? 1 : n % 1 == 0 && (n % 10 ==0 || (n % 10 >=5 && n % 10 <=9) || (n % 100 >=11 && n % 100 <=14 )) ? 2: 3);\n"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
```

### Comparing `ora2-5.0.0/openassessment/locale/vi/LC_MESSAGES/django.mo` & `ora2-5.0.1/openassessment/locale/vi/LC_MESSAGES/django.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
 "Last-Translator: Lam Nguyen <lamnguyen.cis@gmail.com>, 2020\n"
-"Language-Team: Vietnamese (http://www.transifex.com/open-edx/edx-platform/"
+"Language-Team: Vietnamese (http://app.transifex.com/open-edx/edx-platform/"
 "language/vi/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: vi\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
```

### Comparing `ora2-5.0.0/openassessment/locale/vi/LC_MESSAGES/django.po` & `ora2-5.0.1/openassessment/locale/vi/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -23,18 +23,18 @@
 # Trần Tử Thiêng <trantuthieng26256@gmail.com>, 2014
 # Trung V. Nguyen <trung.ngvan@gmail.com>, 2015
 # Vinh Nguyen <vinhmaivy@gmail.com>, 2016
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-01-15 13:36-0500\n"
+"POT-Creation-Date: 2023-04-30 14:36-0400\n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
 "Last-Translator: Lam Nguyen <lamnguyen.cis@gmail.com>, 2020\n"
-"Language-Team: Vietnamese (http://www.transifex.com/open-edx/edx-platform/language/vi/)\n"
+"Language-Team: Vietnamese (http://app.transifex.com/open-edx/edx-platform/language/vi/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: vi\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 #: openassessment/assessment/api/student_training.py:179
```

### Comparing `ora2-5.0.0/openassessment/locale/vi/LC_MESSAGES/djangojs.mo` & `ora2-5.0.1/openassessment/locale/vi/LC_MESSAGES/djangojs.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Le Minh Tri <trilm@hihexa.com>, 2020\n"
-"Language-Team: Vietnamese (http://www.transifex.com/open-edx/edx-platform/"
+"Language-Team: Vietnamese (http://app.transifex.com/open-edx/edx-platform/"
 "language/vi/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: vi\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
```

### Comparing `ora2-5.0.0/openassessment/locale/vi/LC_MESSAGES/djangojs.po` & `ora2-5.0.1/openassessment/locale/vi/LC_MESSAGES/djangojs.po`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-09-13 04:00-0400\n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Le Minh Tri <trilm@hihexa.com>, 2020\n"
-"Language-Team: Vietnamese (http://www.transifex.com/open-edx/edx-platform/language/vi/)\n"
+"Language-Team: Vietnamese (http://app.transifex.com/open-edx/edx-platform/language/vi/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: vi\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
```

### Comparing `ora2-5.0.0/openassessment/locale/zh_CN/LC_MESSAGES/django.mo` & `ora2-5.0.1/openassessment/locale/zh_CN/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
 "Last-Translator: 亚峰 乔 <qiao_yafeng@qq.com>, 2019\n"
-"Language-Team: Chinese (China) (http://www.transifex.com/open-edx/edx-"
+"Language-Team: Chinese (China) (http://app.transifex.com/open-edx/edx-"
 "platform/language/zh_CN/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: zh_CN\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
```

### Comparing `ora2-5.0.0/openassessment/locale/zh_CN/LC_MESSAGES/django.po` & `ora2-5.0.1/openassessment/locale/zh_CN/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -35,18 +35,18 @@
 # 张太红 <zth@xjau.edu.cn>, 2014,2017
 # 汤和果 <hgtang93@163.com>, 2015
 # 竹轩 <fmyzjs@gmail.com>, 2014
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-01-15 13:36-0500\n"
+"POT-Creation-Date: 2023-04-30 14:36-0400\n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
 "Last-Translator: 亚峰 乔 <qiao_yafeng@qq.com>, 2019\n"
-"Language-Team: Chinese (China) (http://www.transifex.com/open-edx/edx-platform/language/zh_CN/)\n"
+"Language-Team: Chinese (China) (http://app.transifex.com/open-edx/edx-platform/language/zh_CN/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: zh_CN\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 #: openassessment/assessment/api/student_training.py:179
```

### Comparing `ora2-5.0.0/openassessment/locale/zh_CN/LC_MESSAGES/djangojs.mo` & `ora2-5.0.1/openassessment/locale/zh_CN/LC_MESSAGES/djangojs.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: jsgang <jsgang9@gmail.com>, 2015,2017,2021\n"
-"Language-Team: Chinese (China) (http://www.transifex.com/open-edx/edx-"
+"Language-Team: Chinese (China) (http://app.transifex.com/open-edx/edx-"
 "platform/language/zh_CN/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: zh_CN\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
```

### Comparing `ora2-5.0.0/openassessment/locale/zh_CN/LC_MESSAGES/djangojs.po` & `ora2-5.0.1/openassessment/locale/zh_CN/LC_MESSAGES/djangojs.po`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-09-13 04:00-0400\n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: jsgang <jsgang9@gmail.com>, 2015,2017,2021\n"
-"Language-Team: Chinese (China) (http://www.transifex.com/open-edx/edx-platform/language/zh_CN/)\n"
+"Language-Team: Chinese (China) (http://app.transifex.com/open-edx/edx-platform/language/zh_CN/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: zh_CN\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
```

### Comparing `ora2-5.0.0/openassessment/locale/zh_TW/LC_MESSAGES/django.mo` & `ora2-5.0.1/openassessment/locale/zh_TW/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
 "Last-Translator: 黃蕙君 <huanghc@mail.fcu.edu.tw>, 2020\n"
-"Language-Team: Chinese (Taiwan) (http://www.transifex.com/open-edx/edx-"
+"Language-Team: Chinese (Taiwan) (http://app.transifex.com/open-edx/edx-"
 "platform/language/zh_TW/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: zh_TW\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
```

### Comparing `ora2-5.0.0/openassessment/locale/zh_TW/LC_MESSAGES/django.po` & `ora2-5.0.1/openassessment/locale/zh_TW/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -25,18 +25,18 @@
 # KUN-MIN SYU <qwer20108@gmail.com>, 2014
 # 薛念林 <nlhsueh@mail.fcu.edu.tw>, 2016
 # 黃蕙君 <huanghc@mail.fcu.edu.tw>, 2020
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-01-15 13:36-0500\n"
+"POT-Creation-Date: 2023-04-30 14:36-0400\n"
 "PO-Revision-Date: 2014-06-11 13:03+0000\n"
 "Last-Translator: 黃蕙君 <huanghc@mail.fcu.edu.tw>, 2020\n"
-"Language-Team: Chinese (Taiwan) (http://www.transifex.com/open-edx/edx-platform/language/zh_TW/)\n"
+"Language-Team: Chinese (Taiwan) (http://app.transifex.com/open-edx/edx-platform/language/zh_TW/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: zh_TW\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 #: openassessment/assessment/api/student_training.py:179
```

### Comparing `ora2-5.0.0/openassessment/locale/zh_TW/LC_MESSAGES/djangojs.mo` & `ora2-5.0.1/openassessment/locale/zh_TW/LC_MESSAGES/djangojs.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,14 +1,14 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Mose Chen <mosechen@gmail.com>, 2017\n"
-"Language-Team: Chinese (Taiwan) (http://www.transifex.com/open-edx/edx-"
+"Language-Team: Chinese (Taiwan) (http://app.transifex.com/open-edx/edx-"
 "platform/language/zh_TW/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: zh_TW\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
```

### Comparing `ora2-5.0.0/openassessment/locale/zh_TW/LC_MESSAGES/djangojs.po` & `ora2-5.0.1/openassessment/locale/zh_TW/LC_MESSAGES/djangojs.po`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: edx-platform\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2022-09-13 04:00-0400\n"
 "PO-Revision-Date: 2014-06-11 13:04+0000\n"
 "Last-Translator: Mose Chen <mosechen@gmail.com>, 2017\n"
-"Language-Team: Chinese (Taiwan) (http://www.transifex.com/open-edx/edx-platform/language/zh_TW/)\n"
+"Language-Team: Chinese (Taiwan) (http://app.transifex.com/open-edx/edx-platform/language/zh_TW/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: zh_TW\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 #: openassessment/xblock/static/dist/openassessment-lms.f2ce054f8f6e20175a0f.js:8
```

### Comparing `ora2-5.0.0/openassessment/management/commands/collect_ora2_data.py` & `ora2-5.0.1/openassessment/management/commands/collect_ora2_data.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/management/commands/create_oa_submissions.py` & `ora2-5.0.1/openassessment/management/commands/create_oa_submissions.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/management/commands/create_oa_submissions_from_file.py` & `ora2-5.0.1/openassessment/management/commands/create_oa_submissions_from_file.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/management/commands/upload_oa_data.py` & `ora2-5.0.1/openassessment/management/commands/upload_oa_data.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/runtime_imports/classes.py` & `ora2-5.0.1/openassessment/runtime_imports/classes.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/runtime_imports/functions.py` & `ora2-5.0.1/openassessment/runtime_imports/functions.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/staffgrader/admin.py` & `ora2-5.0.1/openassessment/staffgrader/admin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/staffgrader/migrations/0001_initial.py` & `ora2-5.0.1/openassessment/staffgrader/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/staffgrader/models/submission_lock.py` & `ora2-5.0.1/openassessment/staffgrader/models/submission_lock.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/staffgrader/serializers/assessments.py` & `ora2-5.0.1/openassessment/staffgrader/serializers/assessments.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/staffgrader/serializers/submission_list.py` & `ora2-5.0.1/openassessment/staffgrader/serializers/submission_list.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/staffgrader/serializers/submission_lock.py` & `ora2-5.0.1/openassessment/staffgrader/serializers/submission_lock.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/staffgrader/staff_grader_mixin.py` & `ora2-5.0.1/openassessment/staffgrader/staff_grader_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/edit/oa_edit.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/edit/oa_edit.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/edit/oa_edit_assessment_steps.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/edit/oa_edit_assessment_steps.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/edit/oa_edit_header_and_validation.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/edit/oa_edit_header_and_validation.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/edit/oa_edit_option.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/edit/oa_edit_option.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/edit/oa_edit_prompt.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/edit/oa_edit_prompt.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/edit/oa_edit_prompts.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/edit/oa_edit_prompts.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/edit/oa_edit_rubric.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/edit/oa_edit_rubric.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/edit/oa_edit_schedule.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/edit/oa_edit_schedule.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment_schedule.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment_schedule.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/edit/oa_edit_staff_assessment.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/edit/oa_edit_staff_assessment.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/edit/oa_edit_student_training.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/edit/oa_edit_student_training.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/edit/oa_rubric_reuse.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/edit/oa_rubric_reuse.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/edit/oa_training_example.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/edit/oa_training_example.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/edit/oa_training_example_criterion.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/edit/oa_training_example_criterion.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/grade/oa_assessment_feedback.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/grade/oa_assessment_feedback.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/grade/oa_assessment_title.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/grade/oa_assessment_title.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/grade/oa_grade_cancelled.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/grade/oa_grade_cancelled.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/grade/oa_grade_complete.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/grade/oa_grade_complete.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/grade/oa_grade_incomplete.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/grade/oa_grade_incomplete.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/grade/oa_grade_not_started.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/grade/oa_grade_not_started.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/grade/oa_grade_waiting.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/grade/oa_grade_waiting.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/instructor_dashboard/oa_grade_available_responses.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/instructor_dashboard/oa_grade_available_responses.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/instructor_dashboard/oa_listing.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/instructor_dashboard/oa_listing.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/instructor_dashboard/oa_waiting_step_details.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/instructor_dashboard/oa_waiting_step_details.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/leaderboard/oa_leaderboard_show.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/leaderboard/oa_leaderboard_show.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/leaderboard/oa_leaderboard_waiting.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/leaderboard/oa_leaderboard_waiting.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/message/oa_message_cancelled.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/message/oa_message_cancelled.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/message/oa_message_closed.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/message/oa_message_closed.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/message/oa_message_complete.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/message/oa_message_complete.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/message/oa_message_incomplete.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/message/oa_message_incomplete.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/message/oa_message_no_team.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/message/oa_message_no_team.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/message/oa_message_open.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/message/oa_message_open.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/oa_base.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/oa_base.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/oa_latex_preview.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/oa_latex_preview.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/oa_rubric.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/oa_rubric.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/oa_submission_answer.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/oa_submission_answer.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/oa_team_uploaded_files.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/oa_team_uploaded_files.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/oa_uploaded_file.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/oa_uploaded_file.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/peer/oa_peer_assessment.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/peer/oa_peer_assessment.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/peer/oa_peer_cancelled.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/peer/oa_peer_cancelled.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/peer/oa_peer_closed.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/peer/oa_peer_closed.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/peer/oa_peer_complete.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/peer/oa_peer_complete.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode_waiting.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode_waiting.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/peer/oa_peer_unavailable.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/peer/oa_peer_unavailable.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/peer/oa_peer_waiting.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/peer/oa_peer_waiting.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/response/oa_response.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/response/oa_response.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/response/oa_response_cancelled.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/response/oa_response_cancelled.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/response/oa_response_closed.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/response/oa_response_closed.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/response/oa_response_graded.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/response/oa_response_graded.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/response/oa_response_submitted.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/response/oa_response_submitted.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/response/oa_response_team_already_submitted.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/response/oa_response_team_already_submitted.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/response/oa_response_unavailable.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/response/oa_response_unavailable.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/self/oa_self_assessment.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/self/oa_self_assessment.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/self/oa_self_cancelled.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/self/oa_self_cancelled.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/self/oa_self_closed.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/self/oa_self_closed.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/self/oa_self_complete.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/self/oa_self_complete.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/self/oa_self_unavailable.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/self/oa_self_unavailable.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/staff/oa_staff_grade.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/staff/oa_staff_grade.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/staff_area/oa_staff_override_assessment.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/staff_area/oa_staff_override_assessment.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/staff_area/oa_student_info.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/staff_area/oa_student_info.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/student_training/student_training.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/student_training/student_training.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/student_training/student_training_cancelled.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/student_training/student_training_cancelled.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/student_training/student_training_closed.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/student_training/student_training_closed.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/student_training/student_training_complete.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/student_training/student_training_complete.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/student_training/student_training_error.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/student_training/student_training_error.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templates/openassessmentblock/student_training/student_training_unavailable.html` & `ora2-5.0.1/openassessment/templates/openassessmentblock/student_training/student_training_unavailable.html`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/templatetags/oa_extras.py` & `ora2-5.0.1/openassessment/templatetags/oa_extras.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/test_utils.py` & `ora2-5.0.1/openassessment/test_utils.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/workflow/admin.py` & `ora2-5.0.1/openassessment/workflow/admin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/workflow/api.py` & `ora2-5.0.1/openassessment/workflow/api.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/workflow/errors.py` & `ora2-5.0.1/openassessment/workflow/errors.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/workflow/migrations/0001_initial.py` & `ora2-5.0.1/openassessment/workflow/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/workflow/migrations/0003_TeamWorkflows.py` & `ora2-5.0.1/openassessment/workflow/migrations/0003_TeamWorkflows.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/workflow/models.py` & `ora2-5.0.1/openassessment/workflow/models.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/workflow/serializers.py` & `ora2-5.0.1/openassessment/workflow/serializers.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/workflow/team_api.py` & `ora2-5.0.1/openassessment/workflow/team_api.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/config_mixin.py` & `ora2-5.0.1/openassessment/xblock/config_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/course_items_listing_mixin.py` & `ora2-5.0.1/openassessment/xblock/course_items_listing_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/data_conversion.py` & `ora2-5.0.1/openassessment/xblock/data_conversion.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/defaults.py` & `ora2-5.0.1/openassessment/xblock/defaults.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/editor_config.py` & `ora2-5.0.1/openassessment/xblock/editor_config.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/grade_mixin.py` & `ora2-5.0.1/openassessment/xblock/grade_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/leaderboard_mixin.py` & `ora2-5.0.1/openassessment/xblock/leaderboard_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/lms_mixin.py` & `ora2-5.0.1/openassessment/xblock/lms_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/load_static.py` & `ora2-5.0.1/openassessment/xblock/load_static.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/message_mixin.py` & `ora2-5.0.1/openassessment/xblock/message_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/mobile.py` & `ora2-5.0.1/openassessment/xblock/mobile.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/openassesment_template_mixin.py` & `ora2-5.0.1/openassessment/xblock/openassesment_template_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/openassessmentblock.py` & `ora2-5.0.1/openassessment/xblock/openassessmentblock.py`

 * *Files 1% similar despite different names*

```diff
@@ -488,20 +488,20 @@
         else:
             course_id = "edX/Enchantment_101/April_1"
             if self.scope_ids.user_id is None:
                 student_id = None
             else:
                 student_id = str(self.scope_ids.user_id)
 
-        student_item_dict = dict(
-            student_id=student_id,
-            item_id=item_id,
-            course_id=course_id,
-            item_type='openassessment'
-        )
+        student_item_dict = {
+            "student_id": student_id,
+            "item_id": item_id,
+            "course_id": course_id,
+            "item_type": 'openassessment'
+        }
         return student_item_dict
 
     def add_javascript_files(self, fragment, item):
         """
         Add all the JavaScript files from a directory to the specified fragment
         """
         if pkg_resources.resource_isdir(__name__, item):
```

### Comparing `ora2-5.0.0/openassessment/xblock/peer_assessment_mixin.py` & `ora2-5.0.1/openassessment/xblock/peer_assessment_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/resolve_dates.py` & `ora2-5.0.1/openassessment/xblock/resolve_dates.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/rubric_reuse_mixin.py` & `ora2-5.0.1/openassessment/xblock/rubric_reuse_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/schema.py` & `ora2-5.0.1/openassessment/xblock/schema.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/self_assessment_mixin.py` & `ora2-5.0.1/openassessment/xblock/self_assessment_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/staff_area_mixin.py` & `ora2-5.0.1/openassessment/xblock/staff_area_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/staff_assessment_mixin.py` & `ora2-5.0.1/openassessment/xblock/staff_assessment_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/static/css/lib/backgrid/backgrid.css` & `ora2-5.0.1/openassessment/xblock/static/css/lib/backgrid/backgrid.css`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/static/css/lib/backgrid/backgrid.min.css` & `ora2-5.0.1/openassessment/xblock/static/css/lib/backgrid/backgrid.min.css`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/static/dist/manifest.json` & `ora2-5.0.1/openassessment/xblock/static/dist/manifest.json`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/static/dist/openassessment-editor-textarea.2774cf3b7c8fadda4341.js` & `ora2-5.0.1/openassessment/xblock/static/dist/openassessment-editor-textarea.2774cf3b7c8fadda4341.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/static/dist/openassessment-editor-textarea.js` & `ora2-5.0.1/openassessment/xblock/static/dist/openassessment-editor-textarea.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/static/dist/openassessment-editor-tinymce.6a6113da3309f666ccda.js` & `ora2-5.0.1/openassessment/xblock/static/dist/openassessment-editor-tinymce.6a6113da3309f666ccda.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/static/dist/openassessment-editor-tinymce.js` & `ora2-5.0.1/openassessment/xblock/static/dist/openassessment-editor-tinymce.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/static/dist/openassessment-lms.7c3203918ed22728dd89.js` & `ora2-5.0.1/openassessment/xblock/static/dist/openassessment-lms.7c3203918ed22728dd89.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/static/dist/openassessment-lms.js` & `ora2-5.0.1/openassessment/xblock/static/dist/openassessment-lms.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/static/dist/openassessment-ltr.cc6fb8c044bfe2899cd5.css` & `ora2-5.0.1/openassessment/xblock/static/dist/openassessment-ltr.cc6fb8c044bfe2899cd5.css`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/static/dist/openassessment-ltr.cc6fb8c044bfe2899cd5.js` & `ora2-5.0.1/openassessment/xblock/static/dist/openassessment-ltr.cc6fb8c044bfe2899cd5.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/static/dist/openassessment-ltr.css` & `ora2-5.0.1/openassessment/xblock/static/dist/openassessment-ltr.css`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/static/dist/openassessment-ltr.js` & `ora2-5.0.1/openassessment/xblock/static/dist/openassessment-ltr.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/static/dist/openassessment-rtl.55343890f44133115ca3.css` & `ora2-5.0.1/openassessment/xblock/static/dist/openassessment-rtl.55343890f44133115ca3.css`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/static/dist/openassessment-rtl.55343890f44133115ca3.js` & `ora2-5.0.1/openassessment/xblock/static/dist/openassessment-rtl.55343890f44133115ca3.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/static/dist/openassessment-rtl.css` & `ora2-5.0.1/openassessment/xblock/static/dist/openassessment-rtl.css`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/static/dist/openassessment-rtl.js` & `ora2-5.0.1/openassessment/xblock/static/dist/openassessment-rtl.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/static/dist/openassessment-studio.6fd5da4c0a2e58a8aba2.js` & `ora2-5.0.1/openassessment/xblock/static/dist/openassessment-studio.6fd5da4c0a2e58a8aba2.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/static/dist/openassessment-studio.js` & `ora2-5.0.1/openassessment/xblock/static/dist/openassessment-studio.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/static/js/lib/backgrid/backgrid.js` & `ora2-5.0.1/openassessment/xblock/static/js/lib/backgrid/backgrid.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/static/js/lib/backgrid/backgrid.min.js` & `ora2-5.0.1/openassessment/xblock/static/js/lib/backgrid/backgrid.min.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/static/js/src/lms/api/waiting_step_details.js` & `ora2-5.0.1/openassessment/xblock/static/js/src/lms/api/waiting_step_details.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/static/js/src/lms/editors/oa_editor_textarea.js` & `ora2-5.0.1/openassessment/xblock/static/js/src/lms/editors/oa_editor_textarea.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/static/js/src/lms/editors/oa_editor_tinymce.js` & `ora2-5.0.1/openassessment/xblock/static/js/src/lms/editors/oa_editor_tinymce.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/static/js/src/lms/oa_base.js` & `ora2-5.0.1/openassessment/xblock/static/js/src/lms/oa_base.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/static/js/src/lms/oa_confirmation_alert.js` & `ora2-5.0.1/openassessment/xblock/static/js/src/lms/oa_confirmation_alert.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/static/js/src/lms/oa_course_items_listing.js` & `ora2-5.0.1/openassessment/xblock/static/js/src/lms/oa_course_items_listing.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/static/js/src/lms/oa_datefactory.js` & `ora2-5.0.1/openassessment/xblock/static/js/src/lms/oa_datefactory.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/static/js/src/lms/oa_file_upload.js` & `ora2-5.0.1/openassessment/xblock/static/js/src/lms/oa_file_upload.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/static/js/src/lms/oa_grade.js` & `ora2-5.0.1/openassessment/xblock/static/js/src/lms/oa_grade.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/static/js/src/lms/oa_leaderboard.js` & `ora2-5.0.1/openassessment/xblock/static/js/src/lms/oa_leaderboard.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/static/js/src/lms/oa_message.js` & `ora2-5.0.1/openassessment/xblock/static/js/src/lms/oa_message.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/static/js/src/lms/oa_peer.js` & `ora2-5.0.1/openassessment/xblock/static/js/src/lms/oa_peer.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/static/js/src/lms/oa_prompts.js` & `ora2-5.0.1/openassessment/xblock/static/js/src/lms/oa_prompts.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/static/js/src/lms/oa_response.js` & `ora2-5.0.1/openassessment/xblock/static/js/src/lms/oa_response.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/static/js/src/lms/oa_response_editor.js` & `ora2-5.0.1/openassessment/xblock/static/js/src/lms/oa_response_editor.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/static/js/src/lms/oa_rubric.js` & `ora2-5.0.1/openassessment/xblock/static/js/src/lms/oa_rubric.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/static/js/src/lms/oa_self.js` & `ora2-5.0.1/openassessment/xblock/static/js/src/lms/oa_self.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/static/js/src/lms/oa_staff.js` & `ora2-5.0.1/openassessment/xblock/static/js/src/lms/oa_staff.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/static/js/src/lms/oa_staff_area.js` & `ora2-5.0.1/openassessment/xblock/static/js/src/lms/oa_staff_area.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/static/js/src/lms/oa_training.js` & `ora2-5.0.1/openassessment/xblock/static/js/src/lms/oa_training.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/static/js/src/oa_server.js` & `ora2-5.0.1/openassessment/xblock/static/js/src/oa_server.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/static/js/src/oa_shared.js` & `ora2-5.0.1/openassessment/xblock/static/js/src/oa_shared.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/static/js/src/studio/oa_container.js` & `ora2-5.0.1/openassessment/xblock/static/js/src/studio/oa_container.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/static/js/src/studio/oa_container_item.js` & `ora2-5.0.1/openassessment/xblock/static/js/src/studio/oa_container_item.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/static/js/src/studio/oa_edit.js` & `ora2-5.0.1/openassessment/xblock/static/js/src/studio/oa_edit.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/static/js/src/studio/oa_edit_assessment.js` & `ora2-5.0.1/openassessment/xblock/static/js/src/studio/oa_edit_assessment.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/static/js/src/studio/oa_edit_assessments_steps.js` & `ora2-5.0.1/openassessment/xblock/static/js/src/studio/oa_edit_assessments_steps.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/static/js/src/studio/oa_edit_fields.js` & `ora2-5.0.1/openassessment/xblock/static/js/src/studio/oa_edit_fields.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/static/js/src/studio/oa_edit_listeners.js` & `ora2-5.0.1/openassessment/xblock/static/js/src/studio/oa_edit_listeners.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/static/js/src/studio/oa_edit_notifier.js` & `ora2-5.0.1/openassessment/xblock/static/js/src/studio/oa_edit_notifier.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/static/js/src/studio/oa_edit_prompts.js` & `ora2-5.0.1/openassessment/xblock/static/js/src/studio/oa_edit_prompts.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/static/js/src/studio/oa_edit_rubric.js` & `ora2-5.0.1/openassessment/xblock/static/js/src/studio/oa_edit_rubric.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/static/js/src/studio/oa_edit_schedule.js` & `ora2-5.0.1/openassessment/xblock/static/js/src/studio/oa_edit_schedule.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/static/js/src/studio/oa_edit_settings.js` & `ora2-5.0.1/openassessment/xblock/static/js/src/studio/oa_edit_settings.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/static/js/src/studio/oa_edit_validation_alert.js` & `ora2-5.0.1/openassessment/xblock/static/js/src/studio/oa_edit_validation_alert.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/static/js/src/studio/oa_tiny_mce.js` & `ora2-5.0.1/openassessment/xblock/static/js/src/studio/oa_tiny_mce.js`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/student_training_mixin.py` & `ora2-5.0.1/openassessment/xblock/student_training_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/studio_mixin.py` & `ora2-5.0.1/openassessment/xblock/studio_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/submission_mixin.py` & `ora2-5.0.1/openassessment/xblock/submission_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/team_mixin.py` & `ora2-5.0.1/openassessment/xblock/team_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/team_workflow_mixin.py` & `ora2-5.0.1/openassessment/xblock/team_workflow_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/user_data.py` & `ora2-5.0.1/openassessment/xblock/user_data.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/validation.py` & `ora2-5.0.1/openassessment/xblock/validation.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/workflow_mixin.py` & `ora2-5.0.1/openassessment/xblock/workflow_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/openassessment/xblock/xml.py` & `ora2-5.0.1/openassessment/xblock/xml.py`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/ora2.egg-info/PKG-INFO` & `ora2-5.0.1/ora2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ora2
-Version: 5.0.0
+Version: 5.0.1
 Summary: edx-ora2
 Home-page: http://github.com/openedx/edx-ora2
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ora2-5.0.0/ora2.egg-info/SOURCES.txt` & `ora2-5.0.1/ora2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/requirements/test.in` & `ora2-5.0.1/requirements/test.in`

 * *Files identical despite different names*

### Comparing `ora2-5.0.0/setup.py` & `ora2-5.0.1/setup.py`

 * *Files identical despite different names*

