# Comparing `tmp/unstructured-0.6.7.tar.gz` & `tmp/unstructured-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unstructured-0.6.7.tar", last modified: Fri May 19 17:33:22 2023, max compression
+gzip compressed data, was "unstructured-0.6.8.tar", last modified: Fri May 19 19:59:45 2023, max compression
```

## Comparing `unstructured-0.6.7.tar` & `unstructured-0.6.8.tar`

### file list

```diff
@@ -1,111 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:33:22.594192 unstructured-0.6.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-05-19 17:33:13.000000 unstructured-0.6.7/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    21203 2023-05-19 17:33:22.594192 unstructured-0.6.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16906 2023-05-19 17:33:13.000000 unstructured-0.6.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-19 17:33:22.598192 unstructured-0.6.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-05-19 17:33:14.000000 unstructured-0.6.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:33:22.582192 unstructured-0.6.7/test_unstructured/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:33:14.000000 unstructured-0.6.7/test_unstructured/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:33:22.582192 unstructured-0.6.7/test_unstructured/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:33:14.000000 unstructured-0.6.7/test_unstructured/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-19 17:33:14.000000 unstructured-0.6.7/test_unstructured/nlp/mock_nltk.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-19 17:33:14.000000 unstructured-0.6.7/test_unstructured/nlp/test_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-05-19 17:33:14.000000 unstructured-0.6.7/test_unstructured/nlp/test_tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-05-19 17:33:14.000000 unstructured-0.6.7/test_unstructured/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:33:22.582192 unstructured-0.6.7/unstructured/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:33:22.586192 unstructured-0.6.7/unstructured/cleaners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/cleaners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/cleaners/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/cleaners/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/cleaners/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:33:22.586192 unstructured-0.6.7/unstructured/documents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/documents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/documents/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/documents/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/documents/email_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    15004 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/documents/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/documents/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:33:22.586192 unstructured-0.6.7/unstructured/file_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/file_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/file_utils/exploration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/file_utils/file_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    11762 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/file_utils/filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/file_utils/google_filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/file_utils/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:33:22.586192 unstructured-0.6.7/unstructured/ingest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/ingest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:33:22.586192 unstructured-0.6.7/unstructured/ingest/connector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/ingest/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/ingest/connector/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/ingest/connector/biomed.py
--rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/ingest/connector/discord.py
--rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/ingest/connector/fsspec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/ingest/connector/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/ingest/connector/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/ingest/connector/gitlab.py
--rw-r--r--   0 runner    (1001) docker     (123)    10994 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/ingest/connector/google_drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/ingest/connector/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/ingest/connector/reddit.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/ingest/connector/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/ingest/connector/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/ingest/connector/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:33:22.586192 unstructured-0.6.7/unstructured/ingest/doc_processor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/ingest/doc_processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/ingest/doc_processor/generalized.py
--rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/ingest/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/ingest/logger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24164 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/ingest/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:33:22.586192 unstructured-0.6.7/unstructured/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:33:22.594192 unstructured-0.6.7/unstructured/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  4472047 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/nlp/english-words.txt
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/nlp/english_words.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/nlp/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/nlp/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/nlp/tokenize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:33:22.594192 unstructured-0.6.7/unstructured/partition/
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/partition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/partition/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8742 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/partition/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/partition/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/partition/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/partition/docx.py
--rw-r--r--   0 runner    (1001) docker     (123)    10023 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/partition/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/partition/epub.py
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/partition/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/partition/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/partition/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/partition/md.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/partition/msg.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/partition/odt.py
--rw-r--r--   0 runner    (1001) docker     (123)    12845 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/partition/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/partition/ppt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/partition/pptx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/partition/rtf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/partition/strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/partition/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/partition/text_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/partition/xlsx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/partition/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:33:22.594192 unstructured-0.6.7/unstructured/staging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/staging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/staging/argilla.py
--rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/staging/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/staging/baseplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/staging/datasaur.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/staging/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/staging/label_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/staging/label_studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/staging/prodigy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-19 17:33:14.000000 unstructured-0.6.7/unstructured/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 17:33:22.586192 unstructured-0.6.7/unstructured.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21203 2023-05-19 17:33:22.000000 unstructured-0.6.7/unstructured.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-19 17:33:22.000000 unstructured-0.6.7/unstructured.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 17:33:22.000000 unstructured-0.6.7/unstructured.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-19 17:33:22.000000 unstructured-0.6.7/unstructured.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-19 17:33:22.000000 unstructured-0.6.7/unstructured.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-19 17:33:22.000000 unstructured-0.6.7/unstructured.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:59:45.246387 unstructured-0.6.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-05-19 19:59:34.000000 unstructured-0.6.8/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    21212 2023-05-19 19:59:45.246387 unstructured-0.6.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16915 2023-05-19 19:59:34.000000 unstructured-0.6.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-19 19:59:45.246387 unstructured-0.6.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-05-19 19:59:34.000000 unstructured-0.6.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:59:45.234387 unstructured-0.6.8/test_unstructured/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:59:34.000000 unstructured-0.6.8/test_unstructured/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:59:45.234387 unstructured-0.6.8/test_unstructured/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:59:34.000000 unstructured-0.6.8/test_unstructured/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-19 19:59:34.000000 unstructured-0.6.8/test_unstructured/nlp/mock_nltk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-19 19:59:34.000000 unstructured-0.6.8/test_unstructured/nlp/test_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-05-19 19:59:34.000000 unstructured-0.6.8/test_unstructured/nlp/test_tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-05-19 19:59:34.000000 unstructured-0.6.8/test_unstructured/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:59:45.234387 unstructured-0.6.8/unstructured/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:59:45.234387 unstructured-0.6.8/unstructured/cleaners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/cleaners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/cleaners/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/cleaners/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/cleaners/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:59:45.234387 unstructured-0.6.8/unstructured/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/documents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/documents/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/documents/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/documents/email_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15004 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/documents/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/documents/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:59:45.234387 unstructured-0.6.8/unstructured/file_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/file_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/file_utils/exploration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/file_utils/file_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11831 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/file_utils/filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/file_utils/google_filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/file_utils/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:59:45.234387 unstructured-0.6.8/unstructured/ingest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/ingest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:59:45.238387 unstructured-0.6.8/unstructured/ingest/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/ingest/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/ingest/connector/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/ingest/connector/biomed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/ingest/connector/discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/ingest/connector/fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/ingest/connector/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/ingest/connector/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/ingest/connector/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10994 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/ingest/connector/google_drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/ingest/connector/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/ingest/connector/reddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/ingest/connector/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/ingest/connector/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/ingest/connector/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:59:45.238387 unstructured-0.6.8/unstructured/ingest/doc_processor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/ingest/doc_processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/ingest/doc_processor/generalized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/ingest/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/ingest/logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24164 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/ingest/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:59:45.238387 unstructured-0.6.8/unstructured/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:59:45.242387 unstructured-0.6.8/unstructured/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:59:34.000000 unstructured-0.6.8/unstructured/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  4472047 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/nlp/english-words.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/nlp/english_words.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/nlp/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/nlp/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/nlp/tokenize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:59:45.246387 unstructured-0.6.8/unstructured/partition/
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/partition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/partition/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8893 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/partition/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/partition/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/partition/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/partition/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/partition/docx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10023 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/partition/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/partition/epub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/partition/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/partition/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/partition/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/partition/md.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/partition/msg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/partition/odt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12845 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/partition/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/partition/ppt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/partition/pptx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/partition/rtf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/partition/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/partition/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/partition/text_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/partition/xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/partition/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:59:45.246387 unstructured-0.6.8/unstructured/staging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/staging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/staging/argilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/staging/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/staging/baseplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/staging/datasaur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/staging/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/staging/label_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/staging/label_studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/staging/prodigy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-19 19:59:35.000000 unstructured-0.6.8/unstructured/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 19:59:45.234387 unstructured-0.6.8/unstructured.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21212 2023-05-19 19:59:44.000000 unstructured-0.6.8/unstructured.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-05-19 19:59:45.000000 unstructured-0.6.8/unstructured.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 19:59:44.000000 unstructured-0.6.8/unstructured.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-19 19:59:44.000000 unstructured-0.6.8/unstructured.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-19 19:59:44.000000 unstructured-0.6.8/unstructured.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-19 19:59:44.000000 unstructured-0.6.8/unstructured.egg-info/top_level.txt
```

### Comparing `unstructured-0.6.7/LICENSE.md` & `unstructured-0.6.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/PKG-INFO` & `unstructured-0.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured
-Version: 0.6.7
+Version: 0.6.8
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
@@ -188,15 +188,15 @@
         ## :clap: Quick Tour
         
         You can run this [Colab notebook](https://colab.research.google.com/drive/1U8VCjY2-x8c6y5TYMbSFtQGlQVFHCVIW) to run the examples below.
         
         The following examples show how to get started with the `unstructured` library.
         
         You can parse **TXT**, **HTML**, **XML**, **PDF**, **EML**, **MSG**, **RTF**, **EPUB**, **DOC**, **DOCX**,
-        **XLSX**, **ODT**, **PPT**, **PPTX**, **JPG**,
+        **XLSX**, **CSV**, **ODT**, **PPT**, **PPTX**, **JPG**,
         and **PNG** documents with one line of code!
         <br></br>
         See our [documentation page](https://unstructured-io.github.io/unstructured) for a full description
         of the features in the library.
         
         ### Document Parsing
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unstructured Version: 0.6.7 Summary: A library that
+Metadata-Version: 2.1 Name: unstructured Version: 0.6.8 Summary: A library that
 prepares raw documents for downstream ML tasks. Home-page: https://github.com/
 Unstructured-IO/unstructured Author: Unstructured Technologies Author-email:
 devops@unstructuredai.io License: Apache-2.0 Description:
 **** [https://raw.githubusercontent.com/Unstructured-IO/unstructured/main/img/
                           unstructured_logo.png] ****
  ![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/
    unstructured.svg) ![https://pypi.python.org/pypi/unstructured/](https://
@@ -112,16 +112,16 @@
 since the `pre-commit` package is installed as part of `make install` mentioned
 above. Finally, if you decided to use `pre-commit` you can also uninstall the
 hooks with `pre-commit uninstall`. ## :clap: Quick Tour You can run this [Colab
 notebook](https://colab.research.google.com/drive/1U8VCjY2-
 x8c6y5TYMbSFtQGlQVFHCVIW) to run the examples below. The following examples
 show how to get started with the `unstructured` library. You can parse **TXT**,
 **HTML**, **XML**, **PDF**, **EML**, **MSG**, **RTF**, **EPUB**, **DOC**,
-**DOCX**, **XLSX**, **ODT**, **PPT**, **PPTX**, **JPG**, and **PNG** documents
-with one line of code!
+**DOCX**, **XLSX**, **CSV**, **ODT**, **PPT**, **PPTX**, **JPG**, and **PNG**
+documents with one line of code!
 See our [documentation page](https://unstructured-io.github.io/unstructured)
 for a full description of the features in the library. ### Document Parsing The
 easiest way to parse a document in unstructured is to use the `partition`
 brick. If you use `partition` brick, `unstructured` will detect the file type
 and route it to the appropriate file-specific partitioning brick. If you are
 using the `partition` brick, you may need to install additional parameters via
 `pip install unstructured[local-inference]`. Ensure you first install
```

### Comparing `unstructured-0.6.7/README.md` & `unstructured-0.6.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -180,15 +180,15 @@
 ## :clap: Quick Tour
 
 You can run this [Colab notebook](https://colab.research.google.com/drive/1U8VCjY2-x8c6y5TYMbSFtQGlQVFHCVIW) to run the examples below.
 
 The following examples show how to get started with the `unstructured` library.
 
 You can parse **TXT**, **HTML**, **XML**, **PDF**, **EML**, **MSG**, **RTF**, **EPUB**, **DOC**, **DOCX**,
-**XLSX**, **ODT**, **PPT**, **PPTX**, **JPG**,
+**XLSX**, **CSV**, **ODT**, **PPT**, **PPTX**, **JPG**,
 and **PNG** documents with one line of code!
 <br></br>
 See our [documentation page](https://unstructured-io.github.io/unstructured) for a full description
 of the features in the library.
 
 ### Document Parsing
```

#### html2text {}

```diff
@@ -108,16 +108,16 @@
 since the `pre-commit` package is installed as part of `make install` mentioned
 above. Finally, if you decided to use `pre-commit` you can also uninstall the
 hooks with `pre-commit uninstall`. ## :clap: Quick Tour You can run this [Colab
 notebook](https://colab.research.google.com/drive/1U8VCjY2-
 x8c6y5TYMbSFtQGlQVFHCVIW) to run the examples below. The following examples
 show how to get started with the `unstructured` library. You can parse **TXT**,
 **HTML**, **XML**, **PDF**, **EML**, **MSG**, **RTF**, **EPUB**, **DOC**,
-**DOCX**, **XLSX**, **ODT**, **PPT**, **PPTX**, **JPG**, and **PNG** documents
-with one line of code!
+**DOCX**, **XLSX**, **CSV**, **ODT**, **PPT**, **PPTX**, **JPG**, and **PNG**
+documents with one line of code!
 See our [documentation page](https://unstructured-io.github.io/unstructured)
 for a full description of the features in the library. ### Document Parsing The
 easiest way to parse a document in unstructured is to use the `partition`
 brick. If you use `partition` brick, `unstructured` will detect the file type
 and route it to the appropriate file-specific partitioning brick. If you are
 using the `partition` brick, you may need to install additional parameters via
 `pip install unstructured[local-inference]`. Ensure you first install
```

### Comparing `unstructured-0.6.7/setup.py` & `unstructured-0.6.8/setup.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/test_unstructured/nlp/mock_nltk.py` & `unstructured-0.6.8/test_unstructured/nlp/mock_nltk.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/test_unstructured/nlp/test_tokenize.py` & `unstructured-0.6.8/test_unstructured/nlp/test_tokenize.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/test_unstructured/test_utils.py` & `unstructured-0.6.8/test_unstructured/test_utils.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/cleaners/core.py` & `unstructured-0.6.8/unstructured/cleaners/core.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/cleaners/extract.py` & `unstructured-0.6.8/unstructured/cleaners/extract.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/cleaners/translate.py` & `unstructured-0.6.8/unstructured/cleaners/translate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/documents/base.py` & `unstructured-0.6.8/unstructured/documents/base.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/documents/elements.py` & `unstructured-0.6.8/unstructured/documents/elements.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/documents/email_elements.py` & `unstructured-0.6.8/unstructured/documents/email_elements.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/documents/html.py` & `unstructured-0.6.8/unstructured/documents/html.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/documents/xml.py` & `unstructured-0.6.8/unstructured/documents/xml.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/file_utils/exploration.py` & `unstructured-0.6.8/unstructured/file_utils/exploration.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/file_utils/file_conversion.py` & `unstructured-0.6.8/unstructured/file_utils/file_conversion.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/file_utils/filetype.py` & `unstructured-0.6.8/unstructured/file_utils/filetype.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,14 +63,15 @@
     PNG = 31
 
     # Plain Text Types
     EML = 40
     RTF = 41
     TXT = 42
     JSON = 43
+    CSV = 44
 
     # Markup Types
     HTML = 50
     XML = 51
     MD = 52
     EPUB = 53
 
@@ -88,14 +89,15 @@
 STR_TO_FILETYPE = {
     "application/pdf": FileType.PDF,
     "application/msword": FileType.DOC,
     "application/vnd.openxmlformats-officedocument.wordprocessingml.document": FileType.DOCX,
     "image/jpeg": FileType.JPG,
     "image/png": FileType.PNG,
     "text/plain": FileType.TXT,
+    "text/csv": FileType.CSV,
     "text/markdown": FileType.MD,
     "text/x-markdown": FileType.MD,
     "application/epub": FileType.EPUB,
     "application/epub+zip": FileType.EPUB,
     "application/json": FileType.JSON,
     "application/rtf": FileType.RTF,
     "text/rtf": FileType.RTF,
@@ -135,14 +137,15 @@
     ".xls": FileType.XLS,
     ".ppt": FileType.PPT,
     ".rtf": FileType.RTF,
     ".json": FileType.JSON,
     ".epub": FileType.EPUB,
     ".msg": FileType.MSG,
     ".odt": FileType.ODT,
+    ".csv": FileType.CSV,
     None: FileType.UNK,
 }
 
 
 def detect_filetype(
     filename: Optional[str] = None,
     content_type: Optional[str] = None,
```

### Comparing `unstructured-0.6.7/unstructured/file_utils/metadata.py` & `unstructured-0.6.8/unstructured/file_utils/metadata.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/ingest/connector/azure.py` & `unstructured-0.6.8/unstructured/ingest/connector/azure.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/ingest/connector/biomed.py` & `unstructured-0.6.8/unstructured/ingest/connector/biomed.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/ingest/connector/discord.py` & `unstructured-0.6.8/unstructured/ingest/connector/discord.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/ingest/connector/fsspec.py` & `unstructured-0.6.8/unstructured/ingest/connector/fsspec.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/ingest/connector/git.py` & `unstructured-0.6.8/unstructured/ingest/connector/git.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/ingest/connector/github.py` & `unstructured-0.6.8/unstructured/ingest/connector/github.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/ingest/connector/gitlab.py` & `unstructured-0.6.8/unstructured/ingest/connector/gitlab.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/ingest/connector/google_drive.py` & `unstructured-0.6.8/unstructured/ingest/connector/google_drive.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/ingest/connector/local.py` & `unstructured-0.6.8/unstructured/ingest/connector/local.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/ingest/connector/reddit.py` & `unstructured-0.6.8/unstructured/ingest/connector/reddit.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/ingest/connector/s3.py` & `unstructured-0.6.8/unstructured/ingest/connector/s3.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/ingest/connector/slack.py` & `unstructured-0.6.8/unstructured/ingest/connector/slack.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/ingest/connector/wikipedia.py` & `unstructured-0.6.8/unstructured/ingest/connector/wikipedia.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/ingest/doc_processor/generalized.py` & `unstructured-0.6.8/unstructured/ingest/doc_processor/generalized.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/ingest/interfaces.py` & `unstructured-0.6.8/unstructured/ingest/interfaces.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/ingest/main.py` & `unstructured-0.6.8/unstructured/ingest/main.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/nlp/english-words.txt` & `unstructured-0.6.8/unstructured/nlp/english-words.txt`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/nlp/english_words.py` & `unstructured-0.6.8/unstructured/nlp/english_words.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/nlp/patterns.py` & `unstructured-0.6.8/unstructured/nlp/patterns.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/nlp/tokenize.py` & `unstructured-0.6.8/unstructured/nlp/tokenize.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/partition/__init__.py` & `unstructured-0.6.8/unstructured/partition/__init__.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/partition/api.py` & `unstructured-0.6.8/unstructured/partition/api.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/partition/auto.py` & `unstructured-0.6.8/unstructured/partition/auto.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     FILETYPE_TO_MIMETYPE,
     STR_TO_FILETYPE,
     FileType,
     detect_filetype,
 )
 from unstructured.logger import logger
 from unstructured.partition.common import exactly_one
+from unstructured.partition.csv import partition_csv
 from unstructured.partition.doc import partition_doc
 from unstructured.partition.docx import partition_docx
 from unstructured.partition.email import partition_email
 from unstructured.partition.epub import partition_epub
 from unstructured.partition.html import partition_html
 from unstructured.partition.image import partition_image
 from unstructured.partition.json import partition_json
@@ -194,14 +195,16 @@
             file=file,
             include_page_breaks=include_page_breaks,
         )
     elif filetype == FileType.JSON:
         elements = partition_json(filename=filename, file=file)
     elif filetype == FileType.XLSX:
         elements = partition_xlsx(filename=filename, file=file)
+    elif filetype == FileType.CSV:
+        elements = partition_csv(filename=filename, file=file)
     else:
         msg = "Invalid file" if not filename else f"Invalid file {filename}"
         raise ValueError(f"{msg}. The {filetype} file type is not supported in partition.")
 
     for element in elements:
         element.metadata.url = url
         if content_type is not None:
```

### Comparing `unstructured-0.6.7/unstructured/partition/common.py` & `unstructured-0.6.8/unstructured/partition/common.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/partition/doc.py` & `unstructured-0.6.8/unstructured/partition/doc.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/partition/docx.py` & `unstructured-0.6.8/unstructured/partition/docx.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/partition/email.py` & `unstructured-0.6.8/unstructured/partition/email.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/partition/epub.py` & `unstructured-0.6.8/unstructured/partition/epub.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/partition/html.py` & `unstructured-0.6.8/unstructured/partition/html.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/partition/image.py` & `unstructured-0.6.8/unstructured/partition/image.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/partition/json.py` & `unstructured-0.6.8/unstructured/partition/json.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/partition/md.py` & `unstructured-0.6.8/unstructured/partition/md.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/partition/msg.py` & `unstructured-0.6.8/unstructured/partition/msg.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/partition/odt.py` & `unstructured-0.6.8/unstructured/partition/odt.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/partition/pdf.py` & `unstructured-0.6.8/unstructured/partition/pdf.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/partition/ppt.py` & `unstructured-0.6.8/unstructured/partition/ppt.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/partition/pptx.py` & `unstructured-0.6.8/unstructured/partition/pptx.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/partition/rtf.py` & `unstructured-0.6.8/unstructured/partition/rtf.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/partition/strategies.py` & `unstructured-0.6.8/unstructured/partition/strategies.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/partition/text.py` & `unstructured-0.6.8/unstructured/partition/text.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/partition/text_type.py` & `unstructured-0.6.8/unstructured/partition/text_type.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/partition/xlsx.py` & `unstructured-0.6.8/unstructured/partition/xlsx.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,17 +21,15 @@
     Parameters
     ----------
     filename
         A string defining the target filename path.
     file
         A file-like object using "rb" mode --> open(filename, "rb").
     metadata_filename
-        The filename to use for the metadata. Relevant because partition_doc converts the
-        document to .xlsx before partition. We want the original source filename in the
-        metadata.
+        The filename to use for the metadata.
     include_metadata
         Determines whether or not metadata is included in the output.
     """
     exactly_one(filename=filename, file=file)
 
     if filename:
         sheets = pd.read_excel(filename, sheet_name=None)
```

### Comparing `unstructured-0.6.7/unstructured/partition/xml.py` & `unstructured-0.6.8/unstructured/partition/xml.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/staging/argilla.py` & `unstructured-0.6.8/unstructured/staging/argilla.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/staging/base.py` & `unstructured-0.6.8/unstructured/staging/base.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/staging/baseplate.py` & `unstructured-0.6.8/unstructured/staging/baseplate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/staging/datasaur.py` & `unstructured-0.6.8/unstructured/staging/datasaur.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/staging/huggingface.py` & `unstructured-0.6.8/unstructured/staging/huggingface.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/staging/label_box.py` & `unstructured-0.6.8/unstructured/staging/label_box.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/staging/label_studio.py` & `unstructured-0.6.8/unstructured/staging/label_studio.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/staging/prodigy.py` & `unstructured-0.6.8/unstructured/staging/prodigy.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured/utils.py` & `unstructured-0.6.8/unstructured/utils.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.7/unstructured.egg-info/PKG-INFO` & `unstructured-0.6.8/unstructured.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured
-Version: 0.6.7
+Version: 0.6.8
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
@@ -188,15 +188,15 @@
         ## :clap: Quick Tour
         
         You can run this [Colab notebook](https://colab.research.google.com/drive/1U8VCjY2-x8c6y5TYMbSFtQGlQVFHCVIW) to run the examples below.
         
         The following examples show how to get started with the `unstructured` library.
         
         You can parse **TXT**, **HTML**, **XML**, **PDF**, **EML**, **MSG**, **RTF**, **EPUB**, **DOC**, **DOCX**,
-        **XLSX**, **ODT**, **PPT**, **PPTX**, **JPG**,
+        **XLSX**, **CSV**, **ODT**, **PPT**, **PPTX**, **JPG**,
         and **PNG** documents with one line of code!
         <br></br>
         See our [documentation page](https://unstructured-io.github.io/unstructured) for a full description
         of the features in the library.
         
         ### Document Parsing
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unstructured Version: 0.6.7 Summary: A library that
+Metadata-Version: 2.1 Name: unstructured Version: 0.6.8 Summary: A library that
 prepares raw documents for downstream ML tasks. Home-page: https://github.com/
 Unstructured-IO/unstructured Author: Unstructured Technologies Author-email:
 devops@unstructuredai.io License: Apache-2.0 Description:
 **** [https://raw.githubusercontent.com/Unstructured-IO/unstructured/main/img/
                           unstructured_logo.png] ****
  ![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/
    unstructured.svg) ![https://pypi.python.org/pypi/unstructured/](https://
@@ -112,16 +112,16 @@
 since the `pre-commit` package is installed as part of `make install` mentioned
 above. Finally, if you decided to use `pre-commit` you can also uninstall the
 hooks with `pre-commit uninstall`. ## :clap: Quick Tour You can run this [Colab
 notebook](https://colab.research.google.com/drive/1U8VCjY2-
 x8c6y5TYMbSFtQGlQVFHCVIW) to run the examples below. The following examples
 show how to get started with the `unstructured` library. You can parse **TXT**,
 **HTML**, **XML**, **PDF**, **EML**, **MSG**, **RTF**, **EPUB**, **DOC**,
-**DOCX**, **XLSX**, **ODT**, **PPT**, **PPTX**, **JPG**, and **PNG** documents
-with one line of code!
+**DOCX**, **XLSX**, **CSV**, **ODT**, **PPT**, **PPTX**, **JPG**, and **PNG**
+documents with one line of code!
 See our [documentation page](https://unstructured-io.github.io/unstructured)
 for a full description of the features in the library. ### Document Parsing The
 easiest way to parse a document in unstructured is to use the `partition`
 brick. If you use `partition` brick, `unstructured` will detect the file type
 and route it to the appropriate file-specific partitioning brick. If you are
 using the `partition` brick, you may need to install additional parameters via
 `pip install unstructured[local-inference]`. Ensure you first install
```

### Comparing `unstructured-0.6.7/unstructured.egg-info/SOURCES.txt` & `unstructured-0.6.8/unstructured.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -61,14 +61,15 @@
 unstructured/nlp/partition.py
 unstructured/nlp/patterns.py
 unstructured/nlp/tokenize.py
 unstructured/partition/__init__.py
 unstructured/partition/api.py
 unstructured/partition/auto.py
 unstructured/partition/common.py
+unstructured/partition/csv.py
 unstructured/partition/doc.py
 unstructured/partition/docx.py
 unstructured/partition/email.py
 unstructured/partition/epub.py
 unstructured/partition/html.py
 unstructured/partition/image.py
 unstructured/partition/json.py
```

