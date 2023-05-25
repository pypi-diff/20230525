# Comparing `tmp/djangocms-blog-agenda-0.3.2.tar.gz` & `tmp/djangocms-blog-agenda-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangocms-blog-agenda-0.3.2.tar", last modified: Mon Apr 17 16:24:32 2023, max compression
+gzip compressed data, was "djangocms-blog-agenda-0.3.3.tar", last modified: Wed May 24 16:36:37 2023, max compression
```

## Comparing `djangocms-blog-agenda-0.3.2.tar` & `djangocms-blog-agenda-0.3.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 kapt       (501)       20        0 2023-04-17 16:24:32.961546 djangocms-blog-agenda-0.3.2/
--rw-r--r--   0 kapt       (501)       20       45 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.3.2/AUTHORS.md
--rw-r--r--   0 kapt       (501)       20     1318 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.3.2/CONTRIBUTING.md
--rw-r--r--   0 kapt       (501)       20    35149 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.3.2/LICENSE
--rw-r--r--   0 kapt       (501)       20      159 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.3.2/MANIFEST.in
--rw-r--r--   0 kapt       (501)       20     3435 2023-04-17 16:24:32.961546 djangocms-blog-agenda-0.3.2/PKG-INFO
--rw-r--r--   0 kapt       (501)       20     2682 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.3.2/README.md
-drwxr-xr-x   0 kapt       (501)       20        0 2023-04-17 16:24:32.949546 djangocms-blog-agenda-0.3.2/djangocms_blog_agenda/
--rw-r--r--   0 kapt       (501)       20        0 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.3.2/djangocms_blog_agenda/__init__.py
--rw-r--r--   0 kapt       (501)       20     1972 2023-04-04 09:28:02.000000 djangocms-blog-agenda-0.3.2/djangocms_blog_agenda/admin.py
--rw-r--r--   0 kapt       (501)       20     1746 2023-03-31 09:10:44.000000 djangocms-blog-agenda-0.3.2/djangocms_blog_agenda/apps.py
--rw-r--r--   0 kapt       (501)       20     2371 2023-04-17 16:23:15.000000 djangocms-blog-agenda-0.3.2/djangocms_blog_agenda/cms_plugins.py
-drwxr-xr-x   0 kapt       (501)       20        0 2023-04-17 16:24:32.935546 djangocms-blog-agenda-0.3.2/djangocms_blog_agenda/locale/
-drwxr-xr-x   0 kapt       (501)       20        0 2023-04-17 16:24:32.935546 djangocms-blog-agenda-0.3.2/djangocms_blog_agenda/locale/fr/
-drwxr-xr-x   0 kapt       (501)       20        0 2023-04-17 16:24:32.954546 djangocms-blog-agenda-0.3.2/djangocms_blog_agenda/locale/fr/LC_MESSAGES/
--rw-r--r--   0 kapt       (501)       20     1408 2023-04-17 15:47:03.000000 djangocms-blog-agenda-0.3.2/djangocms_blog_agenda/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 kapt       (501)       20     3040 2023-04-17 15:46:50.000000 djangocms-blog-agenda-0.3.2/djangocms_blog_agenda/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 kapt       (501)       20        0 2023-04-17 16:24:32.957546 djangocms-blog-agenda-0.3.2/djangocms_blog_agenda/migrations/
--rw-r--r--   0 kapt       (501)       20     1076 2023-03-30 10:38:48.000000 djangocms-blog-agenda-0.3.2/djangocms_blog_agenda/migrations/0001_initial.py
--rw-r--r--   0 kapt       (501)       20     1139 2023-03-30 14:50:16.000000 djangocms-blog-agenda-0.3.2/djangocms_blog_agenda/migrations/0002_auto_20230330_1359.py
--rw-r--r--   0 kapt       (501)       20        0 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.3.2/djangocms_blog_agenda/migrations/__init__.py
--rw-r--r--   0 kapt       (501)       20      765 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.3.2/djangocms_blog_agenda/misc.py
--rw-r--r--   0 kapt       (501)       20      700 2023-03-31 09:16:37.000000 djangocms-blog-agenda-0.3.2/djangocms_blog_agenda/models.py
--rw-r--r--   0 kapt       (501)       20      672 2023-04-17 13:58:19.000000 djangocms-blog-agenda-0.3.2/djangocms_blog_agenda/patched_urls.py
-drwxr-xr-x   0 kapt       (501)       20        0 2023-04-17 16:24:32.936546 djangocms-blog-agenda-0.3.2/djangocms_blog_agenda/templates/
-drwxr-xr-x   0 kapt       (501)       20        0 2023-04-17 16:24:32.961546 djangocms-blog-agenda-0.3.2/djangocms_blog_agenda/templates/djangocms_blog_agenda/
--rw-r--r--   0 kapt       (501)       20     1341 2023-03-30 10:37:22.000000 djangocms-blog-agenda-0.3.2/djangocms_blog_agenda/templates/djangocms_blog_agenda/blog_meta.html
--rw-r--r--   0 kapt       (501)       20     1742 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.3.2/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_detail.html
--rw-r--r--   0 kapt       (501)       20     1361 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.3.2/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_item.html
--rw-r--r--   0 kapt       (501)       20     1889 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.3.2/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_list.html
--rw-r--r--   0 kapt       (501)       20     1285 2023-04-17 16:22:43.000000 djangocms-blog-agenda-0.3.2/djangocms_blog_agenda/views.py
-drwxr-xr-x   0 kapt       (501)       20        0 2023-04-17 16:24:32.953546 djangocms-blog-agenda-0.3.2/djangocms_blog_agenda.egg-info/
--rw-r--r--   0 kapt       (501)       20     3435 2023-04-17 16:24:32.000000 djangocms-blog-agenda-0.3.2/djangocms_blog_agenda.egg-info/PKG-INFO
--rw-r--r--   0 kapt       (501)       20     1102 2023-04-17 16:24:32.000000 djangocms-blog-agenda-0.3.2/djangocms_blog_agenda.egg-info/SOURCES.txt
--rw-r--r--   0 kapt       (501)       20        1 2023-04-17 16:24:32.000000 djangocms-blog-agenda-0.3.2/djangocms_blog_agenda.egg-info/dependency_links.txt
--rw-r--r--   0 kapt       (501)       20       15 2023-04-17 16:24:32.000000 djangocms-blog-agenda-0.3.2/djangocms_blog_agenda.egg-info/requires.txt
--rw-r--r--   0 kapt       (501)       20       22 2023-04-17 16:24:32.000000 djangocms-blog-agenda-0.3.2/djangocms_blog_agenda.egg-info/top_level.txt
--rw-r--r--   0 kapt       (501)       20      786 2023-04-17 16:24:32.962546 djangocms-blog-agenda-0.3.2/setup.cfg
--rw-r--r--   0 kapt       (501)       20       53 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.3.2/setup.py
+drwxr-xr-x   0 kapt       (501)       20        0 2023-05-24 16:36:36.994624 djangocms-blog-agenda-0.3.3/
+-rw-r--r--   0 kapt       (501)       20       45 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.3.3/AUTHORS.md
+-rw-r--r--   0 kapt       (501)       20     1318 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.3.3/CONTRIBUTING.md
+-rw-r--r--   0 kapt       (501)       20    35149 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.3.3/LICENSE
+-rw-r--r--   0 kapt       (501)       20      159 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.3.3/MANIFEST.in
+-rw-r--r--   0 kapt       (501)       20     3435 2023-05-24 16:36:36.994624 djangocms-blog-agenda-0.3.3/PKG-INFO
+-rw-r--r--   0 kapt       (501)       20     2682 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.3.3/README.md
+drwxr-xr-x   0 kapt       (501)       20        0 2023-05-24 16:36:36.982624 djangocms-blog-agenda-0.3.3/djangocms_blog_agenda/
+-rw-r--r--   0 kapt       (501)       20        0 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.3.3/djangocms_blog_agenda/__init__.py
+-rw-r--r--   0 kapt       (501)       20     4215 2023-05-24 16:33:57.000000 djangocms-blog-agenda-0.3.3/djangocms_blog_agenda/admin.py
+-rw-r--r--   0 kapt       (501)       20     1746 2023-03-31 09:10:44.000000 djangocms-blog-agenda-0.3.3/djangocms_blog_agenda/apps.py
+-rw-r--r--   0 kapt       (501)       20     2371 2023-04-17 16:23:15.000000 djangocms-blog-agenda-0.3.3/djangocms_blog_agenda/cms_plugins.py
+drwxr-xr-x   0 kapt       (501)       20        0 2023-05-24 16:36:36.966624 djangocms-blog-agenda-0.3.3/djangocms_blog_agenda/locale/
+drwxr-xr-x   0 kapt       (501)       20        0 2023-05-24 16:36:36.967624 djangocms-blog-agenda-0.3.3/djangocms_blog_agenda/locale/fr/
+drwxr-xr-x   0 kapt       (501)       20        0 2023-05-24 16:36:36.989624 djangocms-blog-agenda-0.3.3/djangocms_blog_agenda/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 kapt       (501)       20     1690 2023-05-24 16:27:27.000000 djangocms-blog-agenda-0.3.3/djangocms_blog_agenda/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 kapt       (501)       20     3671 2023-05-24 16:27:17.000000 djangocms-blog-agenda-0.3.3/djangocms_blog_agenda/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 kapt       (501)       20        0 2023-05-24 16:36:36.991624 djangocms-blog-agenda-0.3.3/djangocms_blog_agenda/migrations/
+-rw-r--r--   0 kapt       (501)       20     1076 2023-03-30 10:38:48.000000 djangocms-blog-agenda-0.3.3/djangocms_blog_agenda/migrations/0001_initial.py
+-rw-r--r--   0 kapt       (501)       20     1139 2023-03-30 14:50:16.000000 djangocms-blog-agenda-0.3.3/djangocms_blog_agenda/migrations/0002_auto_20230330_1359.py
+-rw-r--r--   0 kapt       (501)       20        0 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.3.3/djangocms_blog_agenda/migrations/__init__.py
+-rw-r--r--   0 kapt       (501)       20      765 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.3.3/djangocms_blog_agenda/misc.py
+-rw-r--r--   0 kapt       (501)       20      700 2023-03-31 09:16:37.000000 djangocms-blog-agenda-0.3.3/djangocms_blog_agenda/models.py
+-rw-r--r--   0 kapt       (501)       20      672 2023-04-17 13:58:19.000000 djangocms-blog-agenda-0.3.3/djangocms_blog_agenda/patched_urls.py
+drwxr-xr-x   0 kapt       (501)       20        0 2023-05-24 16:36:36.970624 djangocms-blog-agenda-0.3.3/djangocms_blog_agenda/templates/
+drwxr-xr-x   0 kapt       (501)       20        0 2023-05-24 16:36:36.993624 djangocms-blog-agenda-0.3.3/djangocms_blog_agenda/templates/djangocms_blog_agenda/
+-rw-r--r--   0 kapt       (501)       20     1341 2023-03-30 10:37:22.000000 djangocms-blog-agenda-0.3.3/djangocms_blog_agenda/templates/djangocms_blog_agenda/blog_meta.html
+-rw-r--r--   0 kapt       (501)       20     1742 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.3.3/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_detail.html
+-rw-r--r--   0 kapt       (501)       20     1361 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.3.3/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_item.html
+-rw-r--r--   0 kapt       (501)       20     1889 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.3.3/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_list.html
+-rw-r--r--   0 kapt       (501)       20     1285 2023-04-17 16:22:43.000000 djangocms-blog-agenda-0.3.3/djangocms_blog_agenda/views.py
+drwxr-xr-x   0 kapt       (501)       20        0 2023-05-24 16:36:36.986624 djangocms-blog-agenda-0.3.3/djangocms_blog_agenda.egg-info/
+-rw-r--r--   0 kapt       (501)       20     3435 2023-05-24 16:36:36.000000 djangocms-blog-agenda-0.3.3/djangocms_blog_agenda.egg-info/PKG-INFO
+-rw-r--r--   0 kapt       (501)       20     1102 2023-05-24 16:36:36.000000 djangocms-blog-agenda-0.3.3/djangocms_blog_agenda.egg-info/SOURCES.txt
+-rw-r--r--   0 kapt       (501)       20        1 2023-05-24 16:36:36.000000 djangocms-blog-agenda-0.3.3/djangocms_blog_agenda.egg-info/dependency_links.txt
+-rw-r--r--   0 kapt       (501)       20       15 2023-05-24 16:36:36.000000 djangocms-blog-agenda-0.3.3/djangocms_blog_agenda.egg-info/requires.txt
+-rw-r--r--   0 kapt       (501)       20       22 2023-05-24 16:36:36.000000 djangocms-blog-agenda-0.3.3/djangocms_blog_agenda.egg-info/top_level.txt
+-rw-r--r--   0 kapt       (501)       20      786 2023-05-24 16:36:36.995624 djangocms-blog-agenda-0.3.3/setup.cfg
+-rw-r--r--   0 kapt       (501)       20       53 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.3.3/setup.py
```

### Comparing `djangocms-blog-agenda-0.3.2/CONTRIBUTING.md` & `djangocms-blog-agenda-0.3.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.3.2/LICENSE` & `djangocms-blog-agenda-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.3.2/PKG-INFO` & `djangocms-blog-agenda-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-blog-agenda
-Version: 0.3.2
+Version: 0.3.3
 Summary: Create an agenda on top of djangocms-blog!
 Home-page: https://gitlab.com/kapt/open-source/djangocms-blog-agenda
 Author: Corentin Bettiol
 Author-email: dev@kapt.mobi
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django CMS
```

### Comparing `djangocms-blog-agenda-0.3.2/README.md` & `djangocms-blog-agenda-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.3.2/djangocms_blog_agenda/apps.py` & `djangocms-blog-agenda-0.3.3/djangocms_blog_agenda/apps.py`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.3.2/djangocms_blog_agenda/cms_plugins.py` & `djangocms-blog-agenda-0.3.3/djangocms_blog_agenda/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.3.2/djangocms_blog_agenda/locale/fr/LC_MESSAGES/django.mo` & `djangocms-blog-agenda-0.3.3/djangocms_blog_agenda/locale/fr/LC_MESSAGES/django.mo`

 * *Files 26% similar despite different names*

#### msgunfmt {}

```diff
@@ -19,14 +19,17 @@
 
 msgid "Back"
 msgstr "Retour"
 
 msgid "Category"
 msgstr "Catégorie"
 
+msgid "Event dates"
+msgstr "Dates de l’événement"
+
 msgid "Event end"
 msgstr "Fin de l’événement"
 
 msgid "Event infos"
 msgstr "Informations sur l'événement"
 
 msgid "Event start"
@@ -62,18 +65,33 @@
 msgctxt "agenda_view_url"
 msgid "archives/"
 msgstr "archives/"
 
 msgid "by"
 msgstr "par"
 
+msgid "from {start_part} to {end_part}"
+msgstr "du {start_part} au {end_part}"
+
+msgid "jS"
+msgstr "j"
+
+msgid "jS F"
+msgstr "j F"
+
+msgid "jS F Y"
+msgstr "j F Y"
+
 msgid "next"
 msgstr "suivant"
 
 msgid "of"
 msgstr "sur"
 
+msgid "on {date}"
+msgstr "le {date}"
+
 msgid "previous"
 msgstr "précédent"
 
 msgid "read more"
 msgstr "lire la suite"
```

### Comparing `djangocms-blog-agenda-0.3.2/djangocms_blog_agenda/migrations/0001_initial.py` & `djangocms-blog-agenda-0.3.3/djangocms_blog_agenda/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.3.2/djangocms_blog_agenda/migrations/0002_auto_20230330_1359.py` & `djangocms-blog-agenda-0.3.3/djangocms_blog_agenda/migrations/0002_auto_20230330_1359.py`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.3.2/djangocms_blog_agenda/misc.py` & `djangocms-blog-agenda-0.3.3/djangocms_blog_agenda/misc.py`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.3.2/djangocms_blog_agenda/models.py` & `djangocms-blog-agenda-0.3.3/djangocms_blog_agenda/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.3.2/djangocms_blog_agenda/patched_urls.py` & `djangocms-blog-agenda-0.3.3/djangocms_blog_agenda/patched_urls.py`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.3.2/djangocms_blog_agenda/templates/djangocms_blog_agenda/blog_meta.html` & `djangocms-blog-agenda-0.3.3/djangocms_blog_agenda/templates/djangocms_blog_agenda/blog_meta.html`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.3.2/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_detail.html` & `djangocms-blog-agenda-0.3.3/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_detail.html`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.3.2/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_item.html` & `djangocms-blog-agenda-0.3.3/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_item.html`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.3.2/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_list.html` & `djangocms-blog-agenda-0.3.3/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_list.html`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.3.2/djangocms_blog_agenda/views.py` & `djangocms-blog-agenda-0.3.3/djangocms_blog_agenda/views.py`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.3.2/djangocms_blog_agenda.egg-info/PKG-INFO` & `djangocms-blog-agenda-0.3.3/djangocms_blog_agenda.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-blog-agenda
-Version: 0.3.2
+Version: 0.3.3
 Summary: Create an agenda on top of djangocms-blog!
 Home-page: https://gitlab.com/kapt/open-source/djangocms-blog-agenda
 Author: Corentin Bettiol
 Author-email: dev@kapt.mobi
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django CMS
```

### Comparing `djangocms-blog-agenda-0.3.2/djangocms_blog_agenda.egg-info/SOURCES.txt` & `djangocms-blog-agenda-0.3.3/djangocms_blog_agenda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.3.2/setup.cfg` & `djangocms-blog-agenda-0.3.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = djangocms-blog-agenda
-version = 0.3.2
+version = 0.3.3
 description = Create an agenda on top of djangocms-blog!
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/kapt/open-source/djangocms-blog-agenda
 author = Corentin Bettiol
 author_email = dev@kapt.mobi
 classifiers =
```

