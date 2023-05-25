# Comparing `tmp/linkedinpdfextractor-1.2.2.tar.gz` & `tmp/linkedinpdfextractor-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkedinpdfextractor-1.2.2.tar", last modified: Thu May 18 11:01:42 2023, max compression
+gzip compressed data, was "linkedinpdfextractor-1.2.3.tar", last modified: Wed May 24 11:09:47 2023, max compression
```

## Comparing `linkedinpdfextractor-1.2.2.tar` & `linkedinpdfextractor-1.2.3.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-05-18 11:01:42.173090 linkedinpdfextractor-1.2.2/
--rw-r--r--   0 seshivitakula   (501) staff       (20)     8196 2023-05-05 08:33:17.000000 linkedinpdfextractor-1.2.2/.DS_Store
--rw-r--r--   0 seshivitakula   (501) staff       (20)     1809 2023-04-21 06:26:32.000000 linkedinpdfextractor-1.2.2/.gitignore
--rw-r--r--   0 seshivitakula   (501) staff       (20)       82 2023-04-21 07:18:22.000000 linkedinpdfextractor-1.2.2/AUTHORS.rst
--rw-r--r--   0 seshivitakula   (501) staff       (20)      128 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.2.2/CHANGELOG.rst
--rw-r--r--   0 seshivitakula   (501) staff       (20)    14010 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.2.2/CONTRIBUTING.rst
--rw-r--r--   0 seshivitakula   (501) staff       (20)     1078 2023-04-19 16:57:33.000000 linkedinpdfextractor-1.2.2/LICENSE.txt
--rw-r--r--   0 seshivitakula   (501) staff       (20)     1350 2023-05-18 11:01:42.173241 linkedinpdfextractor-1.2.2/PKG-INFO
--rw-r--r--   0 seshivitakula   (501) staff       (20)     1770 2023-05-16 12:16:16.000000 linkedinpdfextractor-1.2.2/README.md
--rw-r--r--   0 seshivitakula   (501) staff       (20)      840 2023-05-16 12:33:10.000000 linkedinpdfextractor-1.2.2/README.rst
-drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-05-18 11:01:42.150813 linkedinpdfextractor-1.2.2/docs/
--rw-r--r--   0 seshivitakula   (501) staff       (20)     1154 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.2.2/docs/Makefile
-drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-05-18 11:01:42.151100 linkedinpdfextractor-1.2.2/docs/_static/
--rw-r--r--   0 seshivitakula   (501) staff       (20)       18 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.2.2/docs/_static/.gitignore
--rw-r--r--   0 seshivitakula   (501) staff       (20)       41 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.2.2/docs/authors.rst
--rw-r--r--   0 seshivitakula   (501) staff       (20)       43 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.2.2/docs/changelog.rst
--rw-r--r--   0 seshivitakula   (501) staff       (20)     9807 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.2.2/docs/conf.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)       33 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.2.2/docs/contributing.rst
--rw-r--r--   0 seshivitakula   (501) staff       (20)     2373 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.2.2/docs/index.rst
--rw-r--r--   0 seshivitakula   (501) staff       (20)       67 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.2.2/docs/license.rst
--rw-r--r--   0 seshivitakula   (501) staff       (20)       39 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.2.2/docs/readme.rst
--rw-r--r--   0 seshivitakula   (501) staff       (20)      233 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.2.2/docs/requirements.txt
--rw-r--r--   0 seshivitakula   (501) staff       (20)      346 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.2.2/pyproject.toml
--rw-r--r--   0 seshivitakula   (501) staff       (20)       46 2023-04-21 06:26:32.000000 linkedinpdfextractor-1.2.2/requirements.txt
--rw-r--r--   0 seshivitakula   (501) staff       (20)     1249 2023-05-18 11:01:42.174037 linkedinpdfextractor-1.2.2/setup.cfg
--rw-r--r--   0 seshivitakula   (501) staff       (20)      723 2023-05-05 10:18:51.000000 linkedinpdfextractor-1.2.2/setup.py
-drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-05-18 11:01:42.151385 linkedinpdfextractor-1.2.2/src/
--rw-r--r--   0 seshivitakula   (501) staff       (20)     6148 2023-04-19 11:25:51.000000 linkedinpdfextractor-1.2.2/src/.DS_Store
-drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-05-18 11:01:42.153057 linkedinpdfextractor-1.2.2/src/linkedin_pdf_extractor/
--rw-r--r--   0 seshivitakula   (501) staff       (20)     6148 2023-04-19 11:27:25.000000 linkedinpdfextractor-1.2.2/src/linkedin_pdf_extractor/.DS_Store
--rw-r--r--   0 seshivitakula   (501) staff       (20)      577 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.2.2/src/linkedin_pdf_extractor/__init__.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     5774 2023-05-18 10:59:36.000000 linkedinpdfextractor-1.2.2/src/linkedin_pdf_extractor/extractor.py
-drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-05-18 11:01:42.154471 linkedinpdfextractor-1.2.2/src/linkedin_pdf_extractor/pdfstructure/
--rw-r--r--   0 seshivitakula   (501) staff       (20)        0 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.2.2/src/linkedin_pdf_extractor/pdfstructure/__init__.py
-drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-05-18 11:01:42.155964 linkedinpdfextractor-1.2.2/src/linkedin_pdf_extractor/pdfstructure/analysis/
--rw-r--r--   0 seshivitakula   (501) staff       (20)        0 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.2.2/src/linkedin_pdf_extractor/pdfstructure/analysis/__init__.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     2916 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.2.2/src/linkedin_pdf_extractor/pdfstructure/analysis/annotate.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     3691 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.2.2/src/linkedin_pdf_extractor/pdfstructure/analysis/sizemapper.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     5496 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.2.2/src/linkedin_pdf_extractor/pdfstructure/analysis/styledistribution.py
-drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-05-18 11:01:42.157340 linkedinpdfextractor-1.2.2/src/linkedin_pdf_extractor/pdfstructure/hierarchy/
--rw-r--r--   0 seshivitakula   (501) staff       (20)        0 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.2.2/src/linkedin_pdf_extractor/pdfstructure/hierarchy/__init__.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     1593 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.2.2/src/linkedin_pdf_extractor/pdfstructure/hierarchy/detectheader.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     2985 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.2.2/src/linkedin_pdf_extractor/pdfstructure/hierarchy/headercompare.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     7296 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.2.2/src/linkedin_pdf_extractor/pdfstructure/hierarchy/parser.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     2608 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.2.2/src/linkedin_pdf_extractor/pdfstructure/hierarchy/traversal.py
-drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-05-18 11:01:42.158092 linkedinpdfextractor-1.2.2/src/linkedin_pdf_extractor/pdfstructure/model/
--rw-r--r--   0 seshivitakula   (501) staff       (20)        0 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.2.2/src/linkedin_pdf_extractor/pdfstructure/model/__init__.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     4497 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.2.2/src/linkedin_pdf_extractor/pdfstructure/model/document.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     2108 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.2.2/src/linkedin_pdf_extractor/pdfstructure/model/style.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     4155 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.2.2/src/linkedin_pdf_extractor/pdfstructure/printer.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     4983 2023-04-21 06:26:32.000000 linkedinpdfextractor-1.2.2/src/linkedin_pdf_extractor/pdfstructure/source.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     4253 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.2.2/src/linkedin_pdf_extractor/pdfstructure/utils.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     4310 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.2.2/src/linkedin_pdf_extractor/skeleton.py
-drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-05-18 11:01:42.159815 linkedinpdfextractor-1.2.2/src/linkedinpdfextractor.egg-info/
--rw-r--r--   0 seshivitakula   (501) staff       (20)     1350 2023-05-18 11:01:42.000000 linkedinpdfextractor-1.2.2/src/linkedinpdfextractor.egg-info/PKG-INFO
--rw-r--r--   0 seshivitakula   (501) staff       (20)     2528 2023-05-18 11:01:42.000000 linkedinpdfextractor-1.2.2/src/linkedinpdfextractor.egg-info/SOURCES.txt
--rw-r--r--   0 seshivitakula   (501) staff       (20)        1 2023-05-18 11:01:42.000000 linkedinpdfextractor-1.2.2/src/linkedinpdfextractor.egg-info/dependency_links.txt
--rw-r--r--   0 seshivitakula   (501) staff       (20)        1 2023-04-21 07:55:27.000000 linkedinpdfextractor-1.2.2/src/linkedinpdfextractor.egg-info/not-zip-safe
--rw-r--r--   0 seshivitakula   (501) staff       (20)      101 2023-05-18 11:01:42.000000 linkedinpdfextractor-1.2.2/src/linkedinpdfextractor.egg-info/requires.txt
--rw-r--r--   0 seshivitakula   (501) staff       (20)       23 2023-05-18 11:01:42.000000 linkedinpdfextractor-1.2.2/src/linkedinpdfextractor.egg-info/top_level.txt
-drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-05-18 11:01:42.163449 linkedinpdfextractor-1.2.2/tests/
--rw-r--r--   0 seshivitakula   (501) staff       (20)     8196 2023-05-05 08:33:17.000000 linkedinpdfextractor-1.2.2/tests/.DS_Store
--rw-r--r--   0 seshivitakula   (501) staff       (20)        0 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.2.2/tests/__init__.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)      290 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.2.2/tests/conftest.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)      820 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.2.2/tests/helper.py
-drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-05-18 11:01:42.170835 linkedinpdfextractor-1.2.2/tests/resources/
--rw-r--r--   0 seshivitakula   (501) staff       (20)   143869 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.2.2/tests/resources/5648.pdf
--rw-r--r--   0 seshivitakula   (501) staff       (20)   401628 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.2.2/tests/resources/IE00BM67HT60-ATB-FS-DE-2020-2-28.pdf
--rw-r--r--   0 seshivitakula   (501) staff       (20)    18836 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.2.2/tests/resources/SameSize_BoldTitle.pdf
--rw-r--r--   0 seshivitakula   (501) staff       (20)    12108 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.2.2/tests/resources/SameSize_EnumeratedTitle.pdf
--rw-r--r--   0 seshivitakula   (501) staff       (20)    12178 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.2.2/tests/resources/SameStyleOnly.pdf
--rw-r--r--   0 seshivitakula   (501) staff       (20)    45965 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.2.2/tests/resources/interview_cheatsheet-excerpt.png
--rwxr-xr-x   0 seshivitakula   (501) staff       (20)   230787 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.2.2/tests/resources/interview_cheatsheet.pdf
--rw-r--r--   0 seshivitakula   (501) staff       (20)    32674 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.2.2/tests/resources/lorem.pdf
--rw-r--r--   0 seshivitakula   (501) staff       (20)   383508 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.2.2/tests/resources/paper.pdf
-drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-05-18 11:01:42.172808 linkedinpdfextractor-1.2.2/tests/resources/parsed/
--rw-r--r--   0 seshivitakula   (501) staff       (20)   215280 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.2.2/tests/resources/parsed/interview_cheatsheet.json
--rw-r--r--   0 seshivitakula   (501) staff       (20)    15753 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.2.2/tests/resources/parsed/interview_cheatsheet_pretty.txt
--rw-r--r--   0 seshivitakula   (501) staff       (20)    62812 2023-04-19 12:12:39.000000 linkedinpdfextractor-1.2.2/tests/resources/profile.pdf
--rw-r--r--   0 seshivitakula   (501) staff       (20)   251982 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.2.2/tests/resources/samplepptx.pdf
--rw-r--r--   0 seshivitakula   (501) staff       (20)     1398 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.2.2/tests/test_custom_use_cases.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)      656 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.2.2/tests/test_document.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     2304 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.2.2/tests/test_headercompare.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     4709 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.2.2/tests/test_hierarchy.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     3202 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.2.2/tests/test_printer.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)      597 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.2.2/tests/test_skeleton.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     4276 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.2.2/tests/test_style_analyser.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     3865 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.2.2/tests/test_traversal.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)      804 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.2.2/tests/test_utils.py
--rw-r--r--   0 seshivitakula   (501) staff       (20)     2690 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.2.2/tox.ini
+drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-05-24 11:09:47.187888 linkedinpdfextractor-1.2.3/
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     8196 2023-05-05 08:33:17.000000 linkedinpdfextractor-1.2.3/.DS_Store
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     1809 2023-04-21 06:26:32.000000 linkedinpdfextractor-1.2.3/.gitignore
+-rw-r--r--   0 seshivitakula   (501) staff       (20)       82 2023-04-21 07:18:22.000000 linkedinpdfextractor-1.2.3/AUTHORS.rst
+-rw-r--r--   0 seshivitakula   (501) staff       (20)      128 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.2.3/CHANGELOG.rst
+-rw-r--r--   0 seshivitakula   (501) staff       (20)    14010 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.2.3/CONTRIBUTING.rst
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     1078 2023-04-19 16:57:33.000000 linkedinpdfextractor-1.2.3/LICENSE.txt
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     1350 2023-05-24 11:09:47.188022 linkedinpdfextractor-1.2.3/PKG-INFO
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     1770 2023-05-16 12:16:16.000000 linkedinpdfextractor-1.2.3/README.md
+-rw-r--r--   0 seshivitakula   (501) staff       (20)      840 2023-05-16 12:33:10.000000 linkedinpdfextractor-1.2.3/README.rst
+drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-05-24 11:09:47.166551 linkedinpdfextractor-1.2.3/docs/
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     1154 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.2.3/docs/Makefile
+drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-05-24 11:09:47.166840 linkedinpdfextractor-1.2.3/docs/_static/
+-rw-r--r--   0 seshivitakula   (501) staff       (20)       18 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.2.3/docs/_static/.gitignore
+-rw-r--r--   0 seshivitakula   (501) staff       (20)       41 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.2.3/docs/authors.rst
+-rw-r--r--   0 seshivitakula   (501) staff       (20)       43 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.2.3/docs/changelog.rst
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     9807 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.2.3/docs/conf.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)       33 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.2.3/docs/contributing.rst
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     2373 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.2.3/docs/index.rst
+-rw-r--r--   0 seshivitakula   (501) staff       (20)       67 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.2.3/docs/license.rst
+-rw-r--r--   0 seshivitakula   (501) staff       (20)       39 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.2.3/docs/readme.rst
+-rw-r--r--   0 seshivitakula   (501) staff       (20)      233 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.2.3/docs/requirements.txt
+-rw-r--r--   0 seshivitakula   (501) staff       (20)      346 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.2.3/pyproject.toml
+-rw-r--r--   0 seshivitakula   (501) staff       (20)       46 2023-04-21 06:26:32.000000 linkedinpdfextractor-1.2.3/requirements.txt
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     1249 2023-05-24 11:09:47.188754 linkedinpdfextractor-1.2.3/setup.cfg
+-rw-r--r--   0 seshivitakula   (501) staff       (20)      723 2023-05-05 10:18:51.000000 linkedinpdfextractor-1.2.3/setup.py
+drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-05-24 11:09:47.167116 linkedinpdfextractor-1.2.3/src/
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     6148 2023-04-19 11:25:51.000000 linkedinpdfextractor-1.2.3/src/.DS_Store
+drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-05-24 11:09:47.168718 linkedinpdfextractor-1.2.3/src/linkedin_pdf_extractor/
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     6148 2023-04-19 11:27:25.000000 linkedinpdfextractor-1.2.3/src/linkedin_pdf_extractor/.DS_Store
+-rw-r--r--   0 seshivitakula   (501) staff       (20)      577 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.2.3/src/linkedin_pdf_extractor/__init__.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     5736 2023-05-24 11:07:11.000000 linkedinpdfextractor-1.2.3/src/linkedin_pdf_extractor/extractor.py
+drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-05-24 11:09:47.170036 linkedinpdfextractor-1.2.3/src/linkedin_pdf_extractor/pdfstructure/
+-rw-r--r--   0 seshivitakula   (501) staff       (20)        0 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.2.3/src/linkedin_pdf_extractor/pdfstructure/__init__.py
+drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-05-24 11:09:47.171523 linkedinpdfextractor-1.2.3/src/linkedin_pdf_extractor/pdfstructure/analysis/
+-rw-r--r--   0 seshivitakula   (501) staff       (20)        0 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.2.3/src/linkedin_pdf_extractor/pdfstructure/analysis/__init__.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     2916 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.2.3/src/linkedin_pdf_extractor/pdfstructure/analysis/annotate.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     3691 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.2.3/src/linkedin_pdf_extractor/pdfstructure/analysis/sizemapper.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     5496 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.2.3/src/linkedin_pdf_extractor/pdfstructure/analysis/styledistribution.py
+drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-05-24 11:09:47.172843 linkedinpdfextractor-1.2.3/src/linkedin_pdf_extractor/pdfstructure/hierarchy/
+-rw-r--r--   0 seshivitakula   (501) staff       (20)        0 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.2.3/src/linkedin_pdf_extractor/pdfstructure/hierarchy/__init__.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     1593 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.2.3/src/linkedin_pdf_extractor/pdfstructure/hierarchy/detectheader.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     2985 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.2.3/src/linkedin_pdf_extractor/pdfstructure/hierarchy/headercompare.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     7296 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.2.3/src/linkedin_pdf_extractor/pdfstructure/hierarchy/parser.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     2608 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.2.3/src/linkedin_pdf_extractor/pdfstructure/hierarchy/traversal.py
+drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-05-24 11:09:47.173626 linkedinpdfextractor-1.2.3/src/linkedin_pdf_extractor/pdfstructure/model/
+-rw-r--r--   0 seshivitakula   (501) staff       (20)        0 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.2.3/src/linkedin_pdf_extractor/pdfstructure/model/__init__.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     4497 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.2.3/src/linkedin_pdf_extractor/pdfstructure/model/document.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     2108 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.2.3/src/linkedin_pdf_extractor/pdfstructure/model/style.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     4155 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.2.3/src/linkedin_pdf_extractor/pdfstructure/printer.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     4983 2023-04-21 06:26:32.000000 linkedinpdfextractor-1.2.3/src/linkedin_pdf_extractor/pdfstructure/source.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     4253 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.2.3/src/linkedin_pdf_extractor/pdfstructure/utils.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     4310 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.2.3/src/linkedin_pdf_extractor/skeleton.py
+drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-05-24 11:09:47.175398 linkedinpdfextractor-1.2.3/src/linkedinpdfextractor.egg-info/
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     1350 2023-05-24 11:09:47.000000 linkedinpdfextractor-1.2.3/src/linkedinpdfextractor.egg-info/PKG-INFO
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     2528 2023-05-24 11:09:47.000000 linkedinpdfextractor-1.2.3/src/linkedinpdfextractor.egg-info/SOURCES.txt
+-rw-r--r--   0 seshivitakula   (501) staff       (20)        1 2023-05-24 11:09:47.000000 linkedinpdfextractor-1.2.3/src/linkedinpdfextractor.egg-info/dependency_links.txt
+-rw-r--r--   0 seshivitakula   (501) staff       (20)        1 2023-04-21 07:55:27.000000 linkedinpdfextractor-1.2.3/src/linkedinpdfextractor.egg-info/not-zip-safe
+-rw-r--r--   0 seshivitakula   (501) staff       (20)      101 2023-05-24 11:09:47.000000 linkedinpdfextractor-1.2.3/src/linkedinpdfextractor.egg-info/requires.txt
+-rw-r--r--   0 seshivitakula   (501) staff       (20)       23 2023-05-24 11:09:47.000000 linkedinpdfextractor-1.2.3/src/linkedinpdfextractor.egg-info/top_level.txt
+drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-05-24 11:09:47.178975 linkedinpdfextractor-1.2.3/tests/
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     8196 2023-05-05 08:33:17.000000 linkedinpdfextractor-1.2.3/tests/.DS_Store
+-rw-r--r--   0 seshivitakula   (501) staff       (20)        0 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.2.3/tests/__init__.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)      290 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.2.3/tests/conftest.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)      820 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.2.3/tests/helper.py
+drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-05-24 11:09:47.186056 linkedinpdfextractor-1.2.3/tests/resources/
+-rw-r--r--   0 seshivitakula   (501) staff       (20)   143869 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.2.3/tests/resources/5648.pdf
+-rw-r--r--   0 seshivitakula   (501) staff       (20)   401628 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.2.3/tests/resources/IE00BM67HT60-ATB-FS-DE-2020-2-28.pdf
+-rw-r--r--   0 seshivitakula   (501) staff       (20)    18836 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.2.3/tests/resources/SameSize_BoldTitle.pdf
+-rw-r--r--   0 seshivitakula   (501) staff       (20)    12108 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.2.3/tests/resources/SameSize_EnumeratedTitle.pdf
+-rw-r--r--   0 seshivitakula   (501) staff       (20)    12178 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.2.3/tests/resources/SameStyleOnly.pdf
+-rw-r--r--   0 seshivitakula   (501) staff       (20)    45965 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.2.3/tests/resources/interview_cheatsheet-excerpt.png
+-rwxr-xr-x   0 seshivitakula   (501) staff       (20)   230787 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.2.3/tests/resources/interview_cheatsheet.pdf
+-rw-r--r--   0 seshivitakula   (501) staff       (20)    32674 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.2.3/tests/resources/lorem.pdf
+-rw-r--r--   0 seshivitakula   (501) staff       (20)   383508 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.2.3/tests/resources/paper.pdf
+drwxr-xr-x   0 seshivitakula   (501) staff       (20)        0 2023-05-24 11:09:47.187642 linkedinpdfextractor-1.2.3/tests/resources/parsed/
+-rw-r--r--   0 seshivitakula   (501) staff       (20)   215280 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.2.3/tests/resources/parsed/interview_cheatsheet.json
+-rw-r--r--   0 seshivitakula   (501) staff       (20)    15753 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.2.3/tests/resources/parsed/interview_cheatsheet_pretty.txt
+-rw-r--r--   0 seshivitakula   (501) staff       (20)    62812 2023-04-19 12:12:39.000000 linkedinpdfextractor-1.2.3/tests/resources/profile.pdf
+-rw-r--r--   0 seshivitakula   (501) staff       (20)   251982 2023-04-17 18:56:43.000000 linkedinpdfextractor-1.2.3/tests/resources/samplepptx.pdf
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     1398 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.2.3/tests/test_custom_use_cases.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)      656 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.2.3/tests/test_document.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     2304 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.2.3/tests/test_headercompare.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     4709 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.2.3/tests/test_hierarchy.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     3202 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.2.3/tests/test_printer.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)      597 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.2.3/tests/test_skeleton.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     4276 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.2.3/tests/test_style_analyser.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     3865 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.2.3/tests/test_traversal.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)      804 2023-04-24 06:24:13.000000 linkedinpdfextractor-1.2.3/tests/test_utils.py
+-rw-r--r--   0 seshivitakula   (501) staff       (20)     2690 2023-04-19 11:23:25.000000 linkedinpdfextractor-1.2.3/tox.ini
```

### Comparing `linkedinpdfextractor-1.2.2/.DS_Store` & `linkedinpdfextractor-1.2.3/.DS_Store`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.2/.gitignore` & `linkedinpdfextractor-1.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.2/CONTRIBUTING.rst` & `linkedinpdfextractor-1.2.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.2/LICENSE.txt` & `linkedinpdfextractor-1.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.2/PKG-INFO` & `linkedinpdfextractor-1.2.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkedinpdfextractor
-Version: 1.2.2
+Version: 1.2.3
 Summary: Add a short description here!
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: Ketan Prabhu
 Author-email: ketan.prabhu@gigvistas.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `linkedinpdfextractor-1.2.2/README.md` & `linkedinpdfextractor-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.2/README.rst` & `linkedinpdfextractor-1.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.2/docs/Makefile` & `linkedinpdfextractor-1.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.2/docs/conf.py` & `linkedinpdfextractor-1.2.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.2/docs/index.rst` & `linkedinpdfextractor-1.2.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.2/setup.cfg` & `linkedinpdfextractor-1.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.2/setup.py` & `linkedinpdfextractor-1.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.2/src/.DS_Store` & `linkedinpdfextractor-1.2.3/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.2/src/linkedin_pdf_extractor/.DS_Store` & `linkedinpdfextractor-1.2.3/src/linkedin_pdf_extractor/.DS_Store`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.2/src/linkedin_pdf_extractor/__init__.py` & `linkedinpdfextractor-1.2.3/src/linkedin_pdf_extractor/__init__.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.2/src/linkedin_pdf_extractor/extractor.py` & `linkedinpdfextractor-1.2.3/src/linkedin_pdf_extractor/extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,16 +71,14 @@
 
 
 def pdf_to_json(pdfpath:str):
     parser = HierarchyParser()
     source = FileSource(pdfpath)
     document = parser.parse_pdf(source)
 
-    a = document.elements
-
     traverse(document.elements, document.elements[0].level)
     for d in Data:
         print(d)
     df = pd.DataFrame(Data)
     # print(df)
     dtoData = createData(df)
     # print("The variable, name : ", dtoData.name)
@@ -95,15 +93,15 @@
 
 def traverse(elements: List[Section], level, parent=None):
     # print(len(elements))
     for e in elements:
         if (e.heading.text == "Summary" or e.heading.text == "Contact" or
            e.heading.text == "Top Skills" or e.heading.text == "Experience" or e.heading.text == "Education"):
             parent = e.heading.text
-        # print(e).
+        # print(e.heading)
         Data.append({"level": level+1, "text": e.heading.text, "type": parent,
                     "mean_size": e.heading.style.mean_size, "max_size": e.heading.style.max_size})
         # print("Level: ", level, element)
         traverse(e.children, e.level, parent)
 
 
 def createData(data):
@@ -111,25 +109,26 @@
     summary = Summary()
     contact = Contact()
     i = 0
     for index, row in data.iterrows():
         if (row['level'] == 1 and row["mean_size"] == 26.0 and row["max_size"] == 26.0):
             user.name = row["text"]
         elif (row['level'] == 1 and row["mean_size"] == 12.0 and row["max_size"] == 12.0):
-            user.title = row["text"].split('\n')[0]
-        elif (row['level'] == 2 and row["mean_size"] == 12.0 and row["max_size"] == 12.0 and row["type"] == "Summary"):
+            user.title = ' '.join(map(str, row["text"].split('\n')[0:-1]))
+        elif (row['level'] == 2 and 11.8 < row["max_size"] < 12.5 and row["type"] == "Summary"):
             summary.description.append(row["text"])
         elif (row['level'] == 3 and row["max_size"] == 10.5 and row["type"] == "Contact"):
             contact.description = row["text"]
         elif (row['level'] == 3 and row["max_size"] == 10.5 and row["type"] == "Top Skills"):
             user.skills.append(row["text"])
-        elif(row['level'] == 2 and row["type"] == "Experience"):
+        elif(row["type"] == "Experience"):
             parseExperience(row, user)
         elif (row["type"] == "Education"):
             parseEducation(row, user)
+    
     user.summary = ' '.join(map(str, summary.description))
     
     return user
 
 def parseExperience(row, user):
     expLength = len(user.experience)
     exp = Experience() if expLength == 0 else user.experience[expLength-1]
@@ -162,9 +161,9 @@
     if (row["max_size"] == 12.0):
         edu = Education()
         edu.university = row['text']
         user.education.append(edu)
     elif(row["max_size"] == 10.5):
         user.education[eduLength-1].course += row["text"]
 
-#pdf_to_json("/home/pk/Documents/gig-banking/test_linkdin_package/profile.pdf")
+pdf_to_json("/home/pk/Documents/gig-banking/test_linkdin_package/profile.pdf")
 #pdf_to_json("/Users/rishav/Downloads/rishav_linkedin.pdf")
```

### Comparing `linkedinpdfextractor-1.2.2/src/linkedin_pdf_extractor/pdfstructure/analysis/annotate.py` & `linkedinpdfextractor-1.2.3/src/linkedin_pdf_extractor/pdfstructure/analysis/annotate.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.2/src/linkedin_pdf_extractor/pdfstructure/analysis/sizemapper.py` & `linkedinpdfextractor-1.2.3/src/linkedin_pdf_extractor/pdfstructure/analysis/sizemapper.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.2/src/linkedin_pdf_extractor/pdfstructure/analysis/styledistribution.py` & `linkedinpdfextractor-1.2.3/src/linkedin_pdf_extractor/pdfstructure/analysis/styledistribution.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.2/src/linkedin_pdf_extractor/pdfstructure/hierarchy/detectheader.py` & `linkedinpdfextractor-1.2.3/src/linkedin_pdf_extractor/pdfstructure/hierarchy/detectheader.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.2/src/linkedin_pdf_extractor/pdfstructure/hierarchy/headercompare.py` & `linkedinpdfextractor-1.2.3/src/linkedin_pdf_extractor/pdfstructure/hierarchy/headercompare.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.2/src/linkedin_pdf_extractor/pdfstructure/hierarchy/parser.py` & `linkedinpdfextractor-1.2.3/src/linkedin_pdf_extractor/pdfstructure/hierarchy/parser.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.2/src/linkedin_pdf_extractor/pdfstructure/hierarchy/traversal.py` & `linkedinpdfextractor-1.2.3/src/linkedin_pdf_extractor/pdfstructure/hierarchy/traversal.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.2/src/linkedin_pdf_extractor/pdfstructure/model/document.py` & `linkedinpdfextractor-1.2.3/src/linkedin_pdf_extractor/pdfstructure/model/document.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.2/src/linkedin_pdf_extractor/pdfstructure/model/style.py` & `linkedinpdfextractor-1.2.3/src/linkedin_pdf_extractor/pdfstructure/model/style.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.2/src/linkedin_pdf_extractor/pdfstructure/printer.py` & `linkedinpdfextractor-1.2.3/src/linkedin_pdf_extractor/pdfstructure/printer.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.2/src/linkedin_pdf_extractor/pdfstructure/source.py` & `linkedinpdfextractor-1.2.3/src/linkedin_pdf_extractor/pdfstructure/source.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.2/src/linkedin_pdf_extractor/pdfstructure/utils.py` & `linkedinpdfextractor-1.2.3/src/linkedin_pdf_extractor/pdfstructure/utils.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.2/src/linkedin_pdf_extractor/skeleton.py` & `linkedinpdfextractor-1.2.3/src/linkedin_pdf_extractor/skeleton.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.2/src/linkedinpdfextractor.egg-info/PKG-INFO` & `linkedinpdfextractor-1.2.3/src/linkedinpdfextractor.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkedinpdfextractor
-Version: 1.2.2
+Version: 1.2.3
 Summary: Add a short description here!
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: Ketan Prabhu
 Author-email: ketan.prabhu@gigvistas.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `linkedinpdfextractor-1.2.2/src/linkedinpdfextractor.egg-info/SOURCES.txt` & `linkedinpdfextractor-1.2.3/src/linkedinpdfextractor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.2/tests/.DS_Store` & `linkedinpdfextractor-1.2.3/tests/.DS_Store`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.2/tests/helper.py` & `linkedinpdfextractor-1.2.3/tests/helper.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.2/tests/resources/5648.pdf` & `linkedinpdfextractor-1.2.3/tests/resources/5648.pdf`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.2/tests/resources/IE00BM67HT60-ATB-FS-DE-2020-2-28.pdf` & `linkedinpdfextractor-1.2.3/tests/resources/IE00BM67HT60-ATB-FS-DE-2020-2-28.pdf`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.2/tests/resources/SameSize_BoldTitle.pdf` & `linkedinpdfextractor-1.2.3/tests/resources/SameSize_BoldTitle.pdf`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.2/tests/resources/SameSize_EnumeratedTitle.pdf` & `linkedinpdfextractor-1.2.3/tests/resources/SameSize_EnumeratedTitle.pdf`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.2/tests/resources/SameStyleOnly.pdf` & `linkedinpdfextractor-1.2.3/tests/resources/SameStyleOnly.pdf`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.2/tests/resources/interview_cheatsheet-excerpt.png` & `linkedinpdfextractor-1.2.3/tests/resources/interview_cheatsheet-excerpt.png`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.2/tests/resources/interview_cheatsheet.pdf` & `linkedinpdfextractor-1.2.3/tests/resources/interview_cheatsheet.pdf`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.2/tests/resources/lorem.pdf` & `linkedinpdfextractor-1.2.3/tests/resources/lorem.pdf`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.2/tests/resources/paper.pdf` & `linkedinpdfextractor-1.2.3/tests/resources/paper.pdf`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.2/tests/resources/parsed/interview_cheatsheet.json` & `linkedinpdfextractor-1.2.3/tests/resources/parsed/interview_cheatsheet.json`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.2/tests/resources/parsed/interview_cheatsheet_pretty.txt` & `linkedinpdfextractor-1.2.3/tests/resources/parsed/interview_cheatsheet_pretty.txt`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.2/tests/resources/profile.pdf` & `linkedinpdfextractor-1.2.3/tests/resources/profile.pdf`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.2/tests/resources/samplepptx.pdf` & `linkedinpdfextractor-1.2.3/tests/resources/samplepptx.pdf`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.2/tests/test_custom_use_cases.py` & `linkedinpdfextractor-1.2.3/tests/test_custom_use_cases.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.2/tests/test_document.py` & `linkedinpdfextractor-1.2.3/tests/test_document.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.2/tests/test_headercompare.py` & `linkedinpdfextractor-1.2.3/tests/test_headercompare.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.2/tests/test_hierarchy.py` & `linkedinpdfextractor-1.2.3/tests/test_hierarchy.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.2/tests/test_printer.py` & `linkedinpdfextractor-1.2.3/tests/test_printer.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.2/tests/test_skeleton.py` & `linkedinpdfextractor-1.2.3/tests/test_skeleton.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.2/tests/test_style_analyser.py` & `linkedinpdfextractor-1.2.3/tests/test_style_analyser.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.2/tests/test_traversal.py` & `linkedinpdfextractor-1.2.3/tests/test_traversal.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.2/tests/test_utils.py` & `linkedinpdfextractor-1.2.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `linkedinpdfextractor-1.2.2/tox.ini` & `linkedinpdfextractor-1.2.3/tox.ini`

 * *Files identical despite different names*

