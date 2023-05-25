# Comparing `tmp/edsnlp-0.7.4.tar.gz` & `tmp/edsnlp-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edsnlp-0.7.4.tar", last modified: Mon Dec 12 14:37:26 2022, max compression
+gzip compressed data, was "edsnlp-0.8.0.tar", last modified: Thu May 25 07:54:46 2023, max compression
```

## Comparing `edsnlp-0.7.4.tar` & `edsnlp-0.8.0.tar`

### file list

```diff
@@ -1,273 +1,485 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:26.834102 edsnlp-0.7.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2022-12-12 14:37:03.000000 edsnlp-0.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-12 14:37:03.000000 edsnlp-0.7.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3657 2022-12-12 14:37:26.834102 edsnlp-0.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2022-12-12 14:37:03.000000 edsnlp-0.7.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:26.806102 edsnlp-0.7.4/edsnlp/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/conjugator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:26.806102 edsnlp-0.7.4/edsnlp/connectors/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20367 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/connectors/brat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/connectors/labeltool.py
--rw-r--r--   0 runner    (1001) docker     (123)     8130 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/connectors/omop.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/language.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:26.806102 edsnlp-0.7.4/edsnlp/matchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/matchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1209539 2022-12-12 14:37:24.000000 edsnlp-0.7.4/edsnlp/matchers/phrase.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      431 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/matchers/phrase.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     6151 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/matchers/phrase.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    12958 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/matchers/regex.py
--rw-r--r--   0 runner    (1001) docker     (123)     9420 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/matchers/simstring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:26.806102 edsnlp-0.7.4/edsnlp/matchers/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/matchers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/matchers/utils/offset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/matchers/utils/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:26.810102 edsnlp-0.7.4/edsnlp/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9481 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/models/pytorch_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6370 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/models/stack_crf_ner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:26.810102 edsnlp-0.7.4/edsnlp/models/torch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/models/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14962 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/models/torch/crf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7734 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/patch_spacy_dot_components.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:26.810102 edsnlp-0.7.4/edsnlp/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:26.810102 edsnlp-0.7.4/edsnlp/pipelines/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:26.810102 edsnlp-0.7.4/edsnlp/pipelines/core/context/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/core/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/core/context/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/core/context/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:26.810102 edsnlp-0.7.4/edsnlp/pipelines/core/contextual_matcher/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/core/contextual_matcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13511 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/core/contextual_matcher/contextual_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/core/contextual_matcher/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/core/contextual_matcher/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:26.810102 edsnlp-0.7.4/edsnlp/pipelines/core/endlines/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/core/endlines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6155 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/core/endlines/endlines.py
--rw-r--r--   0 runner    (1001) docker     (123)    22602 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/core/endlines/endlinesmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/core/endlines/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/core/endlines/functional.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:26.810102 edsnlp-0.7.4/edsnlp/pipelines/core/matcher/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/core/matcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/core/matcher/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/core/matcher/matcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:26.810102 edsnlp-0.7.4/edsnlp/pipelines/core/normalizer/
--rw-r--r--   0 runner    (1001) docker     (123)      515 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/core/normalizer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:26.810102 edsnlp-0.7.4/edsnlp/pipelines/core/normalizer/accents/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/core/normalizer/accents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/core/normalizer/accents/accents.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/core/normalizer/accents/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/core/normalizer/accents/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/core/normalizer/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:26.810102 edsnlp-0.7.4/edsnlp/pipelines/core/normalizer/lowercase/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/core/normalizer/lowercase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/core/normalizer/lowercase/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/core/normalizer/normalizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:26.814102 edsnlp-0.7.4/edsnlp/pipelines/core/normalizer/pollution/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/core/normalizer/pollution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/core/normalizer/pollution/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/core/normalizer/pollution/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/core/normalizer/pollution/pollution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:26.814102 edsnlp-0.7.4/edsnlp/pipelines/core/normalizer/quotes/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/core/normalizer/quotes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/core/normalizer/quotes/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/core/normalizer/quotes/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/core/normalizer/quotes/quotes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:26.814102 edsnlp-0.7.4/edsnlp/pipelines/core/sentences/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/core/sentences/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/core/sentences/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)  1051913 2022-12-12 14:37:25.000000 edsnlp-0.7.4/edsnlp/pipelines/core/sentences/sentences.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      441 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/core/sentences/sentences.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/core/sentences/sentences.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/core/sentences/terms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:26.814102 edsnlp-0.7.4/edsnlp/pipelines/core/terminology/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/core/terminology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/core/terminology/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4742 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/core/terminology/terminology.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/factories.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:26.814102 edsnlp-0.7.4/edsnlp/pipelines/misc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/misc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:26.814102 edsnlp-0.7.4/edsnlp/pipelines/misc/consultation_dates/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/misc/consultation_dates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4931 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/misc/consultation_dates/consultation_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/misc/consultation_dates/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/misc/consultation_dates/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:26.814102 edsnlp-0.7.4/edsnlp/pipelines/misc/dates/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/misc/dates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8581 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/misc/dates/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/misc/dates/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     6524 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/misc/dates/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:26.814102 edsnlp-0.7.4/edsnlp/pipelines/misc/dates/patterns/
--rw-r--r--   0 runner    (1001) docker     (123)      233 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/misc/dates/patterns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/misc/dates/patterns/absolute.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:26.818102 edsnlp-0.7.4/edsnlp/pipelines/misc/dates/patterns/atomic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/misc/dates/patterns/atomic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/misc/dates/patterns/atomic/days.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/misc/dates/patterns/atomic/delimiters.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/misc/dates/patterns/atomic/directions.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/misc/dates/patterns/atomic/modes.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/misc/dates/patterns/atomic/months.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/misc/dates/patterns/atomic/numbers.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/misc/dates/patterns/atomic/time.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/misc/dates/patterns/atomic/units.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/misc/dates/patterns/atomic/years.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/misc/dates/patterns/current.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/misc/dates/patterns/duration.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/misc/dates/patterns/false_positive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/misc/dates/patterns/relative.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:26.818102 edsnlp-0.7.4/edsnlp/pipelines/misc/measurements/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/misc/measurements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/misc/measurements/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    23794 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/misc/measurements/measurements.py
--rw-r--r--   0 runner    (1001) docker     (123)    13442 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/misc/measurements/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:26.818102 edsnlp-0.7.4/edsnlp/pipelines/misc/reason/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/misc/reason/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/misc/reason/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/misc/reason/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     4361 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/misc/reason/reason.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:26.818102 edsnlp-0.7.4/edsnlp/pipelines/misc/sections/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/misc/sections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/misc/sections/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/misc/sections/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     4028 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/misc/sections/sections.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:26.818102 edsnlp-0.7.4/edsnlp/pipelines/ner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/ner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:26.818102 edsnlp-0.7.4/edsnlp/pipelines/ner/adicap/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/ner/adicap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3417 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/ner/adicap/adicap.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/ner/adicap/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/ner/adicap/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/ner/adicap/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:26.818102 edsnlp-0.7.4/edsnlp/pipelines/ner/cim10/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/ner/cim10/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/ner/cim10/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/ner/cim10/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:26.818102 edsnlp-0.7.4/edsnlp/pipelines/ner/covid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/ner/covid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/ner/covid/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/ner/covid/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:26.818102 edsnlp-0.7.4/edsnlp/pipelines/ner/drugs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/ner/drugs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/ner/drugs/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/ner/drugs/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:26.822102 edsnlp-0.7.4/edsnlp/pipelines/ner/scores/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/ner/scores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4857 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/ner/scores/base_score.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:26.822102 edsnlp-0.7.4/edsnlp/pipelines/ner/scores/charlson/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/ner/scores/charlson/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/ner/scores/charlson/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/ner/scores/charlson/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:26.822102 edsnlp-0.7.4/edsnlp/pipelines/ner/scores/elstonellis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/ner/scores/elstonellis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/ner/scores/elstonellis/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/ner/scores/elstonellis/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:26.822102 edsnlp-0.7.4/edsnlp/pipelines/ner/scores/emergency/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/ner/scores/emergency/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:26.822102 edsnlp-0.7.4/edsnlp/pipelines/ner/scores/emergency/ccmu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/ner/scores/emergency/ccmu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/ner/scores/emergency/ccmu/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/ner/scores/emergency/ccmu/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:26.822102 edsnlp-0.7.4/edsnlp/pipelines/ner/scores/emergency/gemsa/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/ner/scores/emergency/gemsa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/ner/scores/emergency/gemsa/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/ner/scores/emergency/gemsa/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:26.822102 edsnlp-0.7.4/edsnlp/pipelines/ner/scores/emergency/priority/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/ner/scores/emergency/priority/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/ner/scores/emergency/priority/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/ner/scores/emergency/priority/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/ner/scores/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:26.822102 edsnlp-0.7.4/edsnlp/pipelines/ner/scores/sofa/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/ner/scores/sofa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/ner/scores/sofa/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/ner/scores/sofa/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/ner/scores/sofa/sofa.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:26.822102 edsnlp-0.7.4/edsnlp/pipelines/ner/scores/tnm/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/ner/scores/tnm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/ner/scores/tnm/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/ner/scores/tnm/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/ner/scores/tnm/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/ner/scores/tnm/tnm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:26.826102 edsnlp-0.7.4/edsnlp/pipelines/ner/umls/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/ner/umls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/ner/umls/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4487 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/ner/umls/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:26.826102 edsnlp-0.7.4/edsnlp/pipelines/qualifiers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/qualifiers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/qualifiers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/qualifiers/factories.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:26.826102 edsnlp-0.7.4/edsnlp/pipelines/qualifiers/family/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/qualifiers/family/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/qualifiers/family/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5474 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/qualifiers/family/family.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/qualifiers/family/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:26.826102 edsnlp-0.7.4/edsnlp/pipelines/qualifiers/history/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/qualifiers/history/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/qualifiers/history/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    18178 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/qualifiers/history/history.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/qualifiers/history/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:26.826102 edsnlp-0.7.4/edsnlp/pipelines/qualifiers/hypothesis/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/qualifiers/hypothesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/qualifiers/hypothesis/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     7921 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/qualifiers/hypothesis/hypothesis.py
--rw-r--r--   0 runner    (1001) docker     (123)    13450 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/qualifiers/hypothesis/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:26.826102 edsnlp-0.7.4/edsnlp/pipelines/qualifiers/negation/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/qualifiers/negation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/qualifiers/negation/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     8884 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/qualifiers/negation/negation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/qualifiers/negation/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:26.826102 edsnlp-0.7.4/edsnlp/pipelines/qualifiers/reported_speech/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/qualifiers/reported_speech/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/qualifiers/reported_speech/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/qualifiers/reported_speech/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/qualifiers/reported_speech/reported_speech.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/terminations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:26.826102 edsnlp-0.7.4/edsnlp/pipelines/trainable/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/trainable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14332 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/pipelines/trainable/nested_ner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:26.830102 edsnlp-0.7.4/edsnlp/processing/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9653 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/processing/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/processing/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/processing/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6708 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/processing/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      257 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/processing/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/processing/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:26.830102 edsnlp-0.7.4/edsnlp/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    96806 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/resources/adicap.json.gz
--rw-r--r--   0 runner    (1001) docker     (123)   604577 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/resources/cim10.csv.gz
--rw-r--r--   0 runner    (1001) docker     (123)   136088 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/resources/drugs.json
--rw-r--r--   0 runner    (1001) docker     (123)   200566 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/resources/verbs.csv.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:26.834102 edsnlp-0.7.4/edsnlp/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4362 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/utils/blocs.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/utils/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/utils/examples.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/utils/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6193 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/utils/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/utils/inclusion.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/utils/lists.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/utils/merge_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/utils/regex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/utils/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    10766 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/utils/training.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:26.834102 edsnlp-0.7.4/edsnlp/viz/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/viz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5439 2022-12-12 14:37:03.000000 edsnlp-0.7.4/edsnlp/viz/quick_examples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 14:37:26.806102 edsnlp-0.7.4/edsnlp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3657 2022-12-12 14:37:26.000000 edsnlp-0.7.4/edsnlp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8770 2022-12-12 14:37:26.000000 edsnlp-0.7.4/edsnlp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-12 14:37:26.000000 edsnlp-0.7.4/edsnlp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2022-12-12 14:37:26.000000 edsnlp-0.7.4/edsnlp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2022-12-12 14:37:26.000000 edsnlp-0.7.4/edsnlp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2022-12-12 14:37:26.000000 edsnlp-0.7.4/edsnlp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2022-12-12 14:37:03.000000 edsnlp-0.7.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      220 2022-12-12 14:37:03.000000 edsnlp-0.7.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-12 14:37:26.834102 edsnlp-0.7.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2022-12-12 14:37:03.000000 edsnlp-0.7.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.399655 edsnlp-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-25 07:54:19.000000 edsnlp-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-05-25 07:54:46.399655 edsnlp-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-25 07:54:19.000000 edsnlp-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.315655 edsnlp-0.8.0/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)     9814 2023-05-25 07:54:19.000000 edsnlp-0.8.0/demo/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.283655 edsnlp-0.8.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.315655 edsnlp-0.8.0/docs/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-25 07:54:19.000000 edsnlp-0.8.0/docs/scripts/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.315655 edsnlp-0.8.0/edsnlp/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/conjugator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.319655 edsnlp-0.8.0/edsnlp/connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20290 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/connectors/brat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/connectors/labeltool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8130 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/connectors/omop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/language.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.319655 edsnlp-0.8.0/edsnlp/matchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/matchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1214559 2023-05-25 07:54:43.000000 edsnlp-0.8.0/edsnlp/matchers/phrase.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14621 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/matchers/regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/matchers/simstring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.323655 edsnlp-0.8.0/edsnlp/matchers/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/matchers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/matchers/utils/offset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/matchers/utils/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7734 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/patch_spacy_dot_components.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.323655 edsnlp-0.8.0/edsnlp/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.323655 edsnlp-0.8.0/edsnlp/pipelines/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.323655 edsnlp-0.8.0/edsnlp/pipelines/core/context/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/context/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/context/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.323655 edsnlp-0.8.0/edsnlp/pipelines/core/contextual_matcher/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/contextual_matcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15103 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/contextual_matcher/contextual_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/contextual_matcher/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/contextual_matcher/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.327655 edsnlp-0.8.0/edsnlp/pipelines/core/endlines/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/endlines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/endlines/endlines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22602 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/endlines/endlinesmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/endlines/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/endlines/functional.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.327655 edsnlp-0.8.0/edsnlp/pipelines/core/matcher/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/matcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/matcher/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/matcher/matcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.327655 edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.327655 edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/accents/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/accents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/accents/accents.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/accents/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/accents/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.331655 edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/lowercase/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/lowercase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/lowercase/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/normalizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.331655 edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/pollution/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/pollution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/pollution/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/pollution/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/pollution/pollution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.331655 edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/quotes/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/quotes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/quotes/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/quotes/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/quotes/quotes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.331655 edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/spaces/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/spaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/spaces/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/spaces/spaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.335655 edsnlp-0.8.0/edsnlp/pipelines/core/sentences/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/sentences/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/sentences/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1054497 2023-05-25 07:54:45.000000 edsnlp-0.8.0/edsnlp/pipelines/core/sentences/sentences.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/sentences/terms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.335655 edsnlp-0.8.0/edsnlp/pipelines/core/terminology/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/terminology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/terminology/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/core/terminology/terminology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/factories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.335655 edsnlp-0.8.0/edsnlp/pipelines/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.335655 edsnlp-0.8.0/edsnlp/pipelines/misc/consultation_dates/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/consultation_dates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/consultation_dates/consultation_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/consultation_dates/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/consultation_dates/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.335655 edsnlp-0.8.0/edsnlp/pipelines/misc/dates/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/dates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8282 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/dates/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/dates/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6524 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/dates/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.339655 edsnlp-0.8.0/edsnlp/pipelines/misc/dates/patterns/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/dates/patterns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/dates/patterns/absolute.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.339655 edsnlp-0.8.0/edsnlp/pipelines/misc/dates/patterns/atomic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/dates/patterns/atomic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/dates/patterns/atomic/days.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/dates/patterns/atomic/delimiters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/dates/patterns/atomic/directions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/dates/patterns/atomic/modes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/dates/patterns/atomic/months.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/dates/patterns/atomic/numbers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/dates/patterns/atomic/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/dates/patterns/atomic/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/dates/patterns/atomic/years.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/dates/patterns/current.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/dates/patterns/duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/dates/patterns/false_positive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/dates/patterns/relative.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.339655 edsnlp-0.8.0/edsnlp/pipelines/misc/measurements/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/measurements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/measurements/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33920 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/measurements/measurements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14168 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/measurements/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.339655 edsnlp-0.8.0/edsnlp/pipelines/misc/reason/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/reason/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/reason/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/reason/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/reason/reason.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.343655 edsnlp-0.8.0/edsnlp/pipelines/misc/sections/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/sections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/sections/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/sections/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/sections/sections.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.343655 edsnlp-0.8.0/edsnlp/pipelines/misc/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/tables/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/tables/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/misc/tables/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.343655 edsnlp-0.8.0/edsnlp/pipelines/ner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.343655 edsnlp-0.8.0/edsnlp/pipelines/ner/adicap/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/adicap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/adicap/adicap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/adicap/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/adicap/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/adicap/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.343655 edsnlp-0.8.0/edsnlp/pipelines/ner/behaviors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/behaviors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.343655 edsnlp-0.8.0/edsnlp/pipelines/ner/behaviors/alcohol/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/behaviors/alcohol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/behaviors/alcohol/alcohol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/behaviors/alcohol/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/behaviors/alcohol/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.343655 edsnlp-0.8.0/edsnlp/pipelines/ner/behaviors/tobacco/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/behaviors/tobacco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/behaviors/tobacco/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/behaviors/tobacco/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/behaviors/tobacco/tobacco.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.347655 edsnlp-0.8.0/edsnlp/pipelines/ner/cim10/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/cim10/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/cim10/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/cim10/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.347655 edsnlp-0.8.0/edsnlp/pipelines/ner/covid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/covid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/covid/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/covid/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.347655 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.347655 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/AIDS/
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/AIDS/AIDS.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/AIDS/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/AIDS/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/AIDS/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.347655 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/CKD/
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/CKD/CKD.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/CKD/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/CKD/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/CKD/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.347655 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/COPD/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/COPD/COPD.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/COPD/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/COPD/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/COPD/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.351655 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/cerebrovascular_accident/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/cerebrovascular_accident/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/cerebrovascular_accident/cerebrovascular_accident.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/cerebrovascular_accident/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/cerebrovascular_accident/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.351655 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/congestive_heart_failure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/congestive_heart_failure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/congestive_heart_failure/congestive_heart_failure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/congestive_heart_failure/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/congestive_heart_failure/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.351655 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/connective_tissue_disease/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/connective_tissue_disease/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/connective_tissue_disease/connective_tissue_disease.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/connective_tissue_disease/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/connective_tissue_disease/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.351655 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/dementia/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/dementia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/dementia/dementia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/dementia/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/dementia/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.351655 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/diabetes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/diabetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/diabetes/diabetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/diabetes/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/diabetes/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.351655 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/hemiplegia/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/hemiplegia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/hemiplegia/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/hemiplegia/hemiplegia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/hemiplegia/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.355655 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/leukemia/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/leukemia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/leukemia/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/leukemia/leukemia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/leukemia/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.355655 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/liver_disease/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/liver_disease/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/liver_disease/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/liver_disease/liver_disease.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/liver_disease/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.355655 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/lymphoma/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/lymphoma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/lymphoma/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/lymphoma/lymphoma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/lymphoma/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.355655 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/myocardial_infarction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/myocardial_infarction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/myocardial_infarction/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/myocardial_infarction/myocardial_infarction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/myocardial_infarction/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.355655 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/peptic_ulcer_disease/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/peptic_ulcer_disease/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/peptic_ulcer_disease/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/peptic_ulcer_disease/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/peptic_ulcer_disease/peptic_ulcer_disease.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.359655 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/peripheral_vascular_disease/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/peripheral_vascular_disease/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/peripheral_vascular_disease/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/peripheral_vascular_disease/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/peripheral_vascular_disease/peripheral_vascular_disease.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.359655 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/solid_tumor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/solid_tumor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/solid_tumor/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/solid_tumor/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/solid_tumor/solid_tumor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/disorders/terms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.359655 edsnlp-0.8.0/edsnlp/pipelines/ner/drugs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/drugs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/drugs/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/drugs/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.359655 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/base_score.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.359655 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/charlson/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/charlson/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/charlson/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/charlson/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.359655 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/elstonellis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/elstonellis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/elstonellis/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/elstonellis/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.359655 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/emergency/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/emergency/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.359655 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/emergency/ccmu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/emergency/ccmu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/emergency/ccmu/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/emergency/ccmu/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.363655 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/emergency/gemsa/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/emergency/gemsa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/emergency/gemsa/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/emergency/gemsa/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.363655 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/emergency/priority/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/emergency/priority/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/emergency/priority/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/emergency/priority/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.363655 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/sofa/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/sofa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/sofa/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/sofa/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/sofa/sofa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.363655 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/tnm/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/tnm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/tnm/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/tnm/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/tnm/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/scores/tnm/tnm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.363655 edsnlp-0.8.0/edsnlp/pipelines/ner/umls/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/umls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/umls/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/ner/umls/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.363655 edsnlp-0.8.0/edsnlp/pipelines/qualifiers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/qualifiers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/qualifiers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/qualifiers/factories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.367655 edsnlp-0.8.0/edsnlp/pipelines/qualifiers/family/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/qualifiers/family/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/qualifiers/family/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5524 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/qualifiers/family/family.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/qualifiers/family/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.367655 edsnlp-0.8.0/edsnlp/pipelines/qualifiers/history/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/qualifiers/history/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/qualifiers/history/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18237 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/qualifiers/history/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/qualifiers/history/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.367655 edsnlp-0.8.0/edsnlp/pipelines/qualifiers/hypothesis/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/qualifiers/hypothesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/qualifiers/hypothesis/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8001 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/qualifiers/hypothesis/hypothesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13450 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/qualifiers/hypothesis/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.367655 edsnlp-0.8.0/edsnlp/pipelines/qualifiers/negation/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/qualifiers/negation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/qualifiers/negation/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9129 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/qualifiers/negation/negation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/qualifiers/negation/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.367655 edsnlp-0.8.0/edsnlp/pipelines/qualifiers/reported_speech/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/qualifiers/reported_speech/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/qualifiers/reported_speech/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/qualifiers/reported_speech/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7668 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/qualifiers/reported_speech/reported_speech.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/terminations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.367655 edsnlp-0.8.0/edsnlp/pipelines/trainable/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/trainable/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.367655 edsnlp-0.8.0/edsnlp/pipelines/trainable/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/trainable/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14885 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/trainable/layers/crf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.371655 edsnlp-0.8.0/edsnlp/pipelines/trainable/nested_ner/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/trainable/nested_ner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/trainable/nested_ner/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12934 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/trainable/nested_ner/nested_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7042 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/trainable/nested_ner/stack_crf_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9682 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/trainable/pytorch_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.371655 edsnlp-0.8.0/edsnlp/pipelines/trainable/span_qualifier/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/trainable/span_qualifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/trainable/span_qualifier/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8149 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/trainable/span_qualifier/span_multi_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18193 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/trainable/span_qualifier/span_qualifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/pipelines/trainable/span_qualifier/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.371655 edsnlp-0.8.0/edsnlp/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9653 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/processing/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/processing/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/processing/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6708 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/processing/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/processing/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/processing/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.375655 edsnlp-0.8.0/edsnlp/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     7192 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/resources/AVC.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    95841 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/resources/adicap.json.gz
+-rw-r--r--   0 runner    (1001) docker     (123)   604577 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/resources/cim10.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (123)   136088 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/resources/drugs.json
+-rw-r--r--   0 runner    (1001) docker     (123)   200566 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/resources/verbs.csv.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.379655 edsnlp-0.8.0/edsnlp/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/utils/blocs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/utils/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/utils/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/utils/examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/utils/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8838 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/utils/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/utils/inclusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/utils/lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/utils/merge_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/utils/numbers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/utils/regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/utils/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/utils/span_getters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10810 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/utils/training.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.379655 edsnlp-0.8.0/edsnlp/viz/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/viz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-05-25 07:54:19.000000 edsnlp-0.8.0/edsnlp/viz/quick_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.315655 edsnlp-0.8.0/edsnlp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-05-25 07:54:46.000000 edsnlp-0.8.0/edsnlp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16631 2023-05-25 07:54:46.000000 edsnlp-0.8.0/edsnlp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 07:54:46.000000 edsnlp-0.8.0/edsnlp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-05-25 07:54:46.000000 edsnlp-0.8.0/edsnlp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-25 07:54:46.000000 edsnlp-0.8.0/edsnlp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-25 07:54:46.000000 edsnlp-0.8.0/edsnlp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.379655 edsnlp-0.8.0/notebooks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.379655 edsnlp-0.8.0/notebooks/connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-25 07:54:19.000000 edsnlp-0.8.0/notebooks/connectors/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-25 07:54:19.000000 edsnlp-0.8.0/notebooks/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.379655 edsnlp-0.8.0/notebooks/dates/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-25 07:54:19.000000 edsnlp-0.8.0/notebooks/dates/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.379655 edsnlp-0.8.0/notebooks/normalizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-25 07:54:19.000000 edsnlp-0.8.0/notebooks/normalizer/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.379655 edsnlp-0.8.0/notebooks/sections/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-25 07:54:19.000000 edsnlp-0.8.0/notebooks/sections/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.379655 edsnlp-0.8.0/notebooks/sentences/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-25 07:54:19.000000 edsnlp-0.8.0/notebooks/sentences/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.379655 edsnlp-0.8.0/notebooks/tokenizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-25 07:54:19.000000 edsnlp-0.8.0/notebooks/tokenizer/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.379655 edsnlp-0.8.0/notebooks/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-25 07:54:19.000000 edsnlp-0.8.0/notebooks/utilities/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8518 2023-05-25 07:54:19.000000 edsnlp-0.8.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.379655 edsnlp-0.8.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-25 07:54:19.000000 edsnlp-0.8.0/scripts/adicap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-25 07:54:19.000000 edsnlp-0.8.0/scripts/cim10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-25 07:54:19.000000 edsnlp-0.8.0/scripts/conjugate_verbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-25 07:54:19.000000 edsnlp-0.8.0/scripts/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-05-25 07:54:19.000000 edsnlp-0.8.0/scripts/serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 07:54:46.399655 edsnlp-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-25 07:54:19.000000 edsnlp-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.379655 edsnlp-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.383655 edsnlp-0.8.0/tests/connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/connectors/test_brat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/connectors/test_labeltool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/connectors/test_omop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.383655 edsnlp-0.8.0/tests/matchers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/matchers/test_phrase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/matchers/test_regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/matchers/test_simstring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.383655 edsnlp-0.8.0/tests/pipelines/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.383655 edsnlp-0.8.0/tests/pipelines/core/
+-rw-r--r--   0 runner    (1001) docker     (123)    12263 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/core/test_contextual_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/core/test_endlines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/core/test_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/core/test_normalisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/core/test_sentences.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/core/test_terminology.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.383655 edsnlp-0.8.0/tests/pipelines/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/misc/test_consultation_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10361 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/misc/test_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/misc/test_measurements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/misc/test_reason.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/misc/test_sections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/misc/test_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.387655 edsnlp-0.8.0/tests/pipelines/ner/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.391655 edsnlp-0.8.0/tests/pipelines/ner/disorders/
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/ner/disorders/AIDS.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/ner/disorders/CKD.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/ner/disorders/COPD.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/ner/disorders/alcohol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/ner/disorders/cerebrovascular_accident.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/ner/disorders/congestive_heart_failure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/ner/disorders/connective_tissue_disease.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/ner/disorders/dementia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/ner/disorders/diabetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/ner/disorders/hemiplegia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/ner/disorders/leukemia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/ner/disorders/liver_disease.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/ner/disorders/lymphoma.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/ner/disorders/myocardial_infarction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/ner/disorders/peptic_ulcer_disease.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/ner/disorders/peripheral_vascular_disease.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/ner/disorders/solid_tumor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/ner/disorders/test_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/ner/disorders/tobacco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/ner/test_adicap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/ner/test_adicap_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/ner/test_cim10.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/ner/test_covid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/ner/test_drugs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/ner/test_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/ner/test_tnm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/ner/test_umls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.391655 edsnlp-0.8.0/tests/pipelines/qualifiers/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/qualifiers/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/qualifiers/test_family.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/qualifiers/test_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/qualifiers/test_hypothesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/qualifiers/test_negation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/qualifiers/test_reported_speech.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/test_pipelines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.391655 edsnlp-0.8.0/tests/pipelines/trainable/
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/trainable/test_nested_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/pipelines/trainable/test_span_classifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.391655 edsnlp-0.8.0/tests/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/processing/test_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/test_conjugator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/test_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/test_language.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:54:46.391655 edsnlp-0.8.0/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/utils/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/utils/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-25 07:54:19.000000 edsnlp-0.8.0/tests/utils/test_quick_examples.py
```

### Comparing `edsnlp-0.7.4/LICENSE` & `edsnlp-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/PKG-INFO` & `edsnlp-0.8.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,9 @@
-Metadata-Version: 2.1
-Name: edsnlp
-Version: 0.7.4
-Summary: A set of spaCy components to extract information from clinical notes written in French.
-Home-page: https://github.com/aphp/edsnlp
-Author: Data Science - DSI APHP
-Author-email: basile.dura-ext@aphp.fr
-Project-URL: Documentation, https://aphp.github.io/edsnlp
-Project-URL: Demo, https://aphp.github.io/edsnlp/demo
-Project-URL: Bug Tracker, https://github.com/aphp/edsnlp/issues
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: demo
-Provides-Extra: distributed
-License-File: LICENSE
-
-![Tests](https://img.shields.io/github/workflow/status/aphp/edsnlp/Tests%20and%20Linting?label=tests&style=flat-square)
-[![Documentation](https://img.shields.io/github/workflow/status/aphp/edsnlp/Documentation?label=docs&style=flat-square)](https://aphp.github.io/edsnlp/latest/)
+![Tests](https://img.shields.io/github/actions/workflow/status/aphp/edsnlp/tests.yml?branch=master&label=tests&style=flat-square)
+[![Documentation](https://img.shields.io/github/actions/workflow/status/aphp/edsnlp/documentation.yml?branch=master&label=docs&style=flat-square)](https://aphp.github.io/edsnlp/latest/)
 [![PyPI](https://img.shields.io/pypi/v/edsnlp?color=blue&style=flat-square)](https://pypi.org/project/edsnlp/)
 [![Demo](https://img.shields.io/badge/demo%20%F0%9F%9A%80-streamit-grean?style=flat-square)](https://aphp.github.io/edsnlp/demo/)
 [![Codecov](https://img.shields.io/codecov/c/github/aphp/edsnlp?logo=codecov&style=flat-square)](https://codecov.io/gh/aphp/edsnlp)
 [![DOI](https://zenodo.org/badge/467585436.svg)](https://zenodo.org/badge/latestdoi/467585436)
 
 # EDS-NLP
 
@@ -38,15 +22,15 @@
 ```shell
 pip install edsnlp
 ```
 
 We recommend pinning the library version in your projects, or use a strict package manager like [Poetry](https://python-poetry.org/).
 
 ```shell
-pip install edsnlp==0.7.4
+pip install edsnlp==0.8.0
 ```
 
 ### A first pipeline
 
 Once you've installed the library, let's begin with a very simple example that extracts mentions of COVID19 in a text, and detects whether they are negated.
 
 ```python
@@ -99,8 +83,8 @@
   title  = {EDS-NLP: efficient information extraction from French clinical notes},
   url    = {http://aphp.github.io/edsnlp}
 }
 ```
 
 ## Acknowledgement
 
-We would like to thank [Assistance Publique – Hôpitaux de Paris](https://www.aphp.fr/) and [AP-HP Foundation](https://fondationrechercheaphp.fr/) for funding this project.
+We would like to thank [Assistance Publique – Hôpitaux de Paris](https://www.aphp.fr/), [AP-HP Foundation](https://fondationrechercheaphp.fr/) and [Inria](https://www.inria.fr) for funding this project.
```

### Comparing `edsnlp-0.7.4/edsnlp/conjugator.py` & `edsnlp-0.8.0/edsnlp/conjugator.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/connectors/brat.py` & `edsnlp-0.8.0/edsnlp/connectors/brat.py`

 * *Files 1% similar despite different names*

```diff
@@ -309,22 +309,17 @@
     def full_path(self, filename: str) -> str:
         return os.path.join(self.directory, filename)
 
     def load_brat(self) -> List[Dict]:
         """
         Transforms a BRAT folder to a list of spaCy documents.
 
-        Parameters
-        ----------
-        nlp:
-            A spaCy pipeline.
-
         Returns
         -------
-        docs:
+        List[Dict]
             List of spaCy documents, with annotations in the `ents` attribute.
         """
         filenames = [
             path.relative_to(self.directory) for path in self.directory.rglob("*.txt")
         ]
 
         assert len(filenames), f"BRAT directory {self.directory} is empty!"
```

### Comparing `edsnlp-0.7.4/edsnlp/connectors/labeltool.py` & `edsnlp-0.8.0/edsnlp/connectors/labeltool.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/connectors/omop.py` & `edsnlp-0.8.0/edsnlp/connectors/omop.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/language.py` & `edsnlp-0.8.0/edsnlp/language.py`

 * *Files 25% similar despite different names*

```diff
@@ -38,34 +38,50 @@
     """
 
     lang = "eds"
     Defaults = EDSDefaults
     default_config = Defaults
 
 
+TOKENIZER_EXCEPTIONS = [r"Dr\.", r"Pr\.", r"M\.", r"Mme\.", r"Mlle\.", r"(?i)(?:ep\.)"]
+
+
 class EDSTokenizer(DummyTokenizer):
     def __init__(self, vocab: Vocab) -> None:
         """
         Tokenizer class for French clinical documents.
         It better handles tokenization around:
         - numbers: "ACR5" -> ["ACR", "5"] instead of ["ACR5"]
         - newlines: "\n \n \n" -> ["\n", "\n", "\n"] instead of ["\n \n \n"]
         and should be around 5-6 times faster than its standard French counterpart.
-
         Parameters
         ----------
         vocab: Vocab
             The spacy vocabulary
         """
         self.vocab = vocab
         punct = "[:punct:]" + "\"'ˊ＂〃ײ᳓″״‶˶ʺ“”˝"
-        num_like = r"\d+(?:[.,]\d+)?"
-        default = rf"[^\d{punct}'\n[[:space:]]+(?:['ˊ](?=[[:alpha:]]|$))?"
+        num_like = r"\d+(?:[.,]\d(?![.,]?[0-9])|(?![.,]?[0-9]))?"
+        sep = rf"\d{punct}'\n[:space:]"
+        default = rf"[^{sep}]+(?:['ˊ](?=[[:alpha:]]|$))?"
+        exceptions = "|".join(TOKENIZER_EXCEPTIONS)
+        acronym = r"[A-Z][A-Z0-9]*[.](?=[A-Z0-9])"
         self.word_regex = regex.compile(
-            rf"({num_like}|[{punct}]|[\n\r\t]|[^\S\r\n\t]+|{default})([^\S\r\n\t])?"
+            rf"""(?x)
+        (
+            {exceptions}    # tokenizer exceptions like M., Dr., etc
+            |{acronym}      # acronyms
+            |{num_like}     # numbers
+            |[{punct}]      # punctuations
+            |[\n\r\t]       # new lines or tabs
+            |[^\S\r\n\t]+   # multi-spaces
+            |{default}      # anything else: most often alpha-numerical words
+        )                   # followed by
+        ([^\S\r\n\t])?      # an optional space
+        """
         )
 
     def __call__(self, text: str) -> Doc:
         """
         Tokenizes the text using the EDSTokenizer
 
         Parameters
```

### Comparing `edsnlp-0.7.4/edsnlp/matchers/phrase.cpp` & `edsnlp-0.8.0/edsnlp/matchers/phrase.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-/* Generated by Cython 0.29.32 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h",
+            "/tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h",
             "/usr/include/python3.10/Python.h"
         ],
         "extra_compile_args": [
             "-std=c++11"
         ],
         "include_dirs": [
-            "/tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/core/include",
+            "/tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/core/include",
             "/usr/include/python3.10"
         ],
         "language": "c++",
         "name": "edsnlp.matchers.phrase",
         "sources": [
             "edsnlp/matchers/phrase.pyx"
         ]
@@ -33,16 +33,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_32"
-#define CYTHON_HEX_VERSION 0x001D20F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -111,15 +111,15 @@
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -227,15 +227,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -266,15 +266,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -590,35 +590,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
   #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -1233,195 +1233,195 @@
 /* "typedefs.pxd":11
  * ctypedef uint64_t flags_t
  * ctypedef uint16_t len_t
  * ctypedef uint16_t tag_t             # <<<<<<<<<<<<<<
  */
 typedef uint16_t __pyx_t_5spacy_8typedefs_tag_t;
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":690
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":690
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":691
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":691
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":692
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":693
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":693
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":697
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":697
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":698
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":698
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":699
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":700
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":700
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":704
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":704
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":705
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":705
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":714
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":714
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":715
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":715
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":716
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":716
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":718
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":719
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":720
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":720
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":722
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":722
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":723
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":723
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":725
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":726
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":727
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -2286,42 +2286,42 @@
   std::vector<int>  first_head;
   std::vector<int>  first_tail;
   std::unordered_set<int>  *roots;
   std::unordered_map<__pyx_t_5spacy_8typedefs_hash_t,int>  *node_map;
   std::unordered_map<__pyx_t_5spacy_8typedefs_hash_t,int>  *edge_map;
 };
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":729
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":730
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":730
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":731
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":733
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":733
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2650,26 +2650,26 @@
   __pyx_t_5spacy_8typedefs_attr_t excluded_hash;
 };
 
 
 /* "edsnlp/matchers/phrase.pyx":73
  *             Span.set_extension("normalized_variant", getter=get_normalized_variant)
  * 
- *     def build_patterns(self, nlp: Language, terms: Patterns):             # <<<<<<<<<<<<<<
+ *     def build_patterns(self, nlp: Language, terms: Patterns, progress: bool = False):             # <<<<<<<<<<<<<<
  *         """
  *         Build patterns and adds them for matching.
  */
 struct __pyx_obj_6edsnlp_8matchers_6phrase___pyx_scope_struct__build_patterns {
   PyObject_HEAD
   PyObject *__pyx_8genexpr1__pyx_v_name;
   PyObject *__pyx_v_nlp;
 };
 
 
-/* "edsnlp/matchers/phrase.pyx":93
+/* "edsnlp/matchers/phrase.pyx":95
  *             for name, pipe in nlp.pipeline
  *             if any(
  *                 "token" in assign and not assign == "token.is_sent_start"             # <<<<<<<<<<<<<<
  *                 for assign in nlp.get_pipe_meta(name).assigns
  *             )
  */
 struct __pyx_obj_6edsnlp_8matchers_6phrase___pyx_scope_struct_1_genexpr {
@@ -3440,26 +3440,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -3816,20 +3816,28 @@
 #else
 #define __Pyx_PyObject_GenericGetAttr PyObject_GenericGetAttr
 #endif
 
 /* TypeImport.proto */
 #ifndef __PYX_HAVE_RT_ImportType_proto
 #define __PYX_HAVE_RT_ImportType_proto
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#endif
 enum __Pyx_ImportType_CheckSize {
    __Pyx_ImportType_CheckSize_Error = 0,
    __Pyx_ImportType_CheckSize_Warn = 1,
    __Pyx_ImportType_CheckSize_Ignore = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
 #endif
 
 /* GetVTable.proto */
 static void* __Pyx_GetVtable(PyObject *dict);
 
 /* SetVTable.proto */
 static int __Pyx_SetVtable(PyObject *dict, void *vtable);
@@ -4484,14 +4492,15 @@
 static const char __pyx_k_Language[] = "Language";
 static const char __pyx_k_Patterns[] = "Patterns";
 static const char __pyx_k_excluded[] = "excluded";
 static const char __pyx_k_getstate[] = "__getstate__";
 static const char __pyx_k_itemsize[] = "itemsize";
 static const char __pyx_k_patterns[] = "patterns";
 static const char __pyx_k_pipeline[] = "pipeline";
+static const char __pyx_k_progress[] = "progress";
 static const char __pyx_k_pyx_type[] = "__pyx_type";
 static const char __pyx_k_setstate[] = "__setstate__";
 static const char __pyx_k_validate[] = "validate";
 static const char __pyx_k_TypeError[] = "TypeError";
 static const char __pyx_k_enumerate[] = "enumerate";
 static const char __pyx_k_pyx_state[] = "__pyx_state";
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
@@ -4661,14 +4670,15 @@
 static PyObject *__pyx_kp_u_numpy_core_umath_failed_to_impor;
 static PyObject *__pyx_n_s_obj;
 static PyObject *__pyx_n_s_pack;
 static PyObject *__pyx_n_u_patterns;
 static PyObject *__pyx_n_s_pickle;
 static PyObject *__pyx_n_s_pipe;
 static PyObject *__pyx_n_s_pipeline;
+static PyObject *__pyx_n_s_progress;
 static PyObject *__pyx_n_s_pyx_PickleError;
 static PyObject *__pyx_n_s_pyx_checksum;
 static PyObject *__pyx_n_s_pyx_getbuffer;
 static PyObject *__pyx_n_s_pyx_result;
 static PyObject *__pyx_n_s_pyx_state;
 static PyObject *__pyx_n_s_pyx_type;
 static PyObject *__pyx_n_s_pyx_unpickle_Enum;
@@ -4718,15 +4728,15 @@
 static PyObject *__pyx_n_s_variant;
 static PyObject *__pyx_n_s_vocab;
 static PyObject *__pyx_n_s_whitespace;
 static PyObject *__pyx_pf_6edsnlp_8matchers_6phrase_get_normalized_variant(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_doclike); /* proto */
 static int __pyx_pf_6edsnlp_8matchers_6phrase_16EDSPhraseMatcher___init__(struct __pyx_obj_6edsnlp_8matchers_6phrase_EDSPhraseMatcher *__pyx_v_self, struct __pyx_obj_5spacy_5vocab_Vocab *__pyx_v_vocab, PyObject *__pyx_v_attr, PyObject *__pyx_v_ignore_excluded, PyObject *__pyx_v_ignore_space_tokens, PyObject *__pyx_v_validate); /* proto */
 static PyObject *__pyx_pf_6edsnlp_8matchers_6phrase_16EDSPhraseMatcher_2set_extensions(void); /* proto */
 static PyObject *__pyx_pf_6edsnlp_8matchers_6phrase_16EDSPhraseMatcher_14build_patterns_8genexpr1_genexpr(PyObject *__pyx_self); /* proto */
-static PyObject *__pyx_pf_6edsnlp_8matchers_6phrase_16EDSPhraseMatcher_4build_patterns(struct __pyx_obj_6edsnlp_8matchers_6phrase_EDSPhraseMatcher *__pyx_v_self, PyObject *__pyx_v_nlp, PyObject *__pyx_v_terms); /* proto */
+static PyObject *__pyx_pf_6edsnlp_8matchers_6phrase_16EDSPhraseMatcher_4build_patterns(struct __pyx_obj_6edsnlp_8matchers_6phrase_EDSPhraseMatcher *__pyx_v_self, PyObject *__pyx_v_nlp, PyObject *__pyx_v_terms, PyObject *__pyx_v_progress); /* proto */
 static PyObject *__pyx_pf_6edsnlp_8matchers_6phrase_16EDSPhraseMatcher_6__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_6edsnlp_8matchers_6phrase_EDSPhraseMatcher *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_6edsnlp_8matchers_6phrase_16EDSPhraseMatcher_8__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_6edsnlp_8matchers_6phrase_EDSPhraseMatcher *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array___cinit__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_shape, Py_ssize_t __pyx_v_itemsize, PyObject *__pyx_v_format, PyObject *__pyx_v_mode, int __pyx_v_allocate_buffer); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array_2__getbuffer__(struct __pyx_array_obj *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags); /* proto */
 static void __pyx_array___pyx_pf_15View_dot_MemoryView_5array_4__dealloc__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_15View_dot_MemoryView_5array_7memview___get__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static Py_ssize_t __pyx_array___pyx_pf_15View_dot_MemoryView_5array_6__len__(struct __pyx_array_obj *__pyx_v_self); /* proto */
@@ -5038,15 +5048,15 @@
  *     variant = variant.rstrip(" ")
  *     variant = re.sub(r"\s+", " ", variant)
  *     return variant             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  if (!(likely(PyUnicode_CheckExact(__pyx_v_variant))||((__pyx_v_variant) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_v_variant)->tp_name), 0))) __PYX_ERR(0, 23, __pyx_L1_error)
+  if (!(likely(PyUnicode_CheckExact(__pyx_v_variant))||((__pyx_v_variant) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_v_variant)->tp_name), 0))) __PYX_ERR(0, 23, __pyx_L1_error)
   __Pyx_INCREF(__pyx_v_variant);
   __pyx_r = ((PyObject*)__pyx_v_variant);
   goto __pyx_L0;
 
   /* "edsnlp/matchers/phrase.pyx":18
  * 
  * 
@@ -5497,15 +5507,15 @@
   if (__pyx_t_5) {
 
     /* "edsnlp/matchers/phrase.pyx":71
  *     def set_extensions():
  *         if not Span.has_extension("normalized_variant"):
  *             Span.set_extension("normalized_variant", getter=get_normalized_variant)             # <<<<<<<<<<<<<<
  * 
- *     def build_patterns(self, nlp: Language, terms: Patterns):
+ *     def build_patterns(self, nlp: Language, terms: Patterns, progress: bool = False):
  */
     __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_5spacy_6tokens_4span_Span), __pyx_n_s_set_extension); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 71, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 71, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_get_normalized_variant); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 71, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
@@ -5549,38 +5559,42 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "edsnlp/matchers/phrase.pyx":73
  *             Span.set_extension("normalized_variant", getter=get_normalized_variant)
  * 
- *     def build_patterns(self, nlp: Language, terms: Patterns):             # <<<<<<<<<<<<<<
+ *     def build_patterns(self, nlp: Language, terms: Patterns, progress: bool = False):             # <<<<<<<<<<<<<<
  *         """
  *         Build patterns and adds them for matching.
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_6edsnlp_8matchers_6phrase_16EDSPhraseMatcher_5build_patterns(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_6edsnlp_8matchers_6phrase_16EDSPhraseMatcher_4build_patterns[] = "\n        Build patterns and adds them for matching.\n        Helper function for pipelines using this matcher.\n\n        Parameters\n        ----------\n        nlp : Language\n            The instance of the spaCy language class.\n        terms : Patterns\n            Dictionary of label/terms, or label/dictionary of terms/attribute.\n        ";
+static char __pyx_doc_6edsnlp_8matchers_6phrase_16EDSPhraseMatcher_4build_patterns[] = "\n        Build patterns and adds them for matching.\n        Helper function for pipelines using this matcher.\n\n        Parameters\n        ----------\n        nlp : Language\n            The instance of the spaCy language class.\n        terms : Patterns\n            Dictionary of label/terms, or label/dictionary of terms/attribute.\n        progress: bool\n            Whether to track progress when preprocessing terms\n        ";
 static PyObject *__pyx_pw_6edsnlp_8matchers_6phrase_16EDSPhraseMatcher_5build_patterns(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_nlp = 0;
   PyObject *__pyx_v_terms = 0;
+  PyObject *__pyx_v_progress = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("build_patterns (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_nlp,&__pyx_n_s_terms,0};
-    PyObject* values[2] = {0,0};
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_nlp,&__pyx_n_s_terms,&__pyx_n_s_progress,0};
+    PyObject* values[3] = {0,0,0};
+    values[2] = ((PyObject *)Py_False);
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
+        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
@@ -5589,46 +5603,57 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_nlp)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_terms)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("build_patterns", 1, 2, 2, 1); __PYX_ERR(0, 73, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("build_patterns", 0, 2, 3, 1); __PYX_ERR(0, 73, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  2:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_progress);
+          if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
         if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "build_patterns") < 0)) __PYX_ERR(0, 73, __pyx_L3_error)
       }
-    } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
-      goto __pyx_L5_argtuple_error;
     } else {
-      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+      switch (PyTuple_GET_SIZE(__pyx_args)) {
+        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        CYTHON_FALLTHROUGH;
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        break;
+        default: goto __pyx_L5_argtuple_error;
+      }
     }
     __pyx_v_nlp = values[0];
     __pyx_v_terms = values[1];
+    __pyx_v_progress = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("build_patterns", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 73, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("build_patterns", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 73, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("edsnlp.matchers.phrase.EDSPhraseMatcher.build_patterns", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_6edsnlp_8matchers_6phrase_16EDSPhraseMatcher_4build_patterns(((struct __pyx_obj_6edsnlp_8matchers_6phrase_EDSPhraseMatcher *)__pyx_v_self), __pyx_v_nlp, __pyx_v_terms);
+  __pyx_r = __pyx_pf_6edsnlp_8matchers_6phrase_16EDSPhraseMatcher_4build_patterns(((struct __pyx_obj_6edsnlp_8matchers_6phrase_EDSPhraseMatcher *)__pyx_v_self), __pyx_v_nlp, __pyx_v_terms, __pyx_v_progress);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 static PyObject *__pyx_gb_6edsnlp_8matchers_6phrase_16EDSPhraseMatcher_14build_patterns_8genexpr1_2generator(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "edsnlp/matchers/phrase.pyx":93
+/* "edsnlp/matchers/phrase.pyx":95
  *             for name, pipe in nlp.pipeline
  *             if any(
  *                 "token" in assign and not assign == "token.is_sent_start"             # <<<<<<<<<<<<<<
  *                 for assign in nlp.get_pipe_meta(name).assigns
  *             )
  */
 
@@ -5640,23 +5665,23 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("genexpr", 0);
   __pyx_cur_scope = (struct __pyx_obj_6edsnlp_8matchers_6phrase___pyx_scope_struct_1_genexpr *)__pyx_tp_new_6edsnlp_8matchers_6phrase___pyx_scope_struct_1_genexpr(__pyx_ptype_6edsnlp_8matchers_6phrase___pyx_scope_struct_1_genexpr, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_6edsnlp_8matchers_6phrase___pyx_scope_struct_1_genexpr *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 93, __pyx_L1_error)
+    __PYX_ERR(0, 95, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_outer_scope = (struct __pyx_obj_6edsnlp_8matchers_6phrase___pyx_scope_struct__build_patterns *) __pyx_self;
   __Pyx_INCREF(((PyObject *)__pyx_cur_scope->__pyx_outer_scope));
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_outer_scope);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_6edsnlp_8matchers_6phrase_16EDSPhraseMatcher_14build_patterns_8genexpr1_2generator, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_build_patterns_locals_genexpr, __pyx_n_s_edsnlp_matchers_phrase); if (unlikely(!gen)) __PYX_ERR(0, 93, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_6edsnlp_8matchers_6phrase_16EDSPhraseMatcher_14build_patterns_8genexpr1_2generator, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_build_patterns_locals_genexpr, __pyx_n_s_edsnlp_matchers_phrase); if (unlikely(!gen)) __PYX_ERR(0, 95, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
@@ -5682,184 +5707,184 @@
   int __pyx_t_7;
   int __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("genexpr", 0);
-  __Pyx_TraceCall("genexpr", __pyx_f[0], 93, 0, __PYX_ERR(0, 93, __pyx_L1_error));
+  __Pyx_TraceCall("genexpr", __pyx_f[0], 95, 0, __PYX_ERR(0, 95, __pyx_L1_error));
   switch (__pyx_generator->resume_label) {
     case 0: goto __pyx_L3_first_run;
     default: /* CPython raises the right error here */
     __Pyx_TraceReturn(Py_None, 0);
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 93, __pyx_L1_error)
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 95, __pyx_L1_error)
 
-  /* "edsnlp/matchers/phrase.pyx":94
+  /* "edsnlp/matchers/phrase.pyx":96
  *             if any(
  *                 "token" in assign and not assign == "token.is_sent_start"
  *                 for assign in nlp.get_pipe_meta(name).assigns             # <<<<<<<<<<<<<<
  *             )
  *         ]
  */
-  if (unlikely(!__pyx_cur_scope->__pyx_outer_scope->__pyx_v_nlp)) { __Pyx_RaiseClosureNameError("nlp"); __PYX_ERR(0, 94, __pyx_L1_error) }
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_outer_scope->__pyx_v_nlp, __pyx_n_s_get_pipe_meta); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 94, __pyx_L1_error)
+  if (unlikely(!__pyx_cur_scope->__pyx_outer_scope->__pyx_v_nlp)) { __Pyx_RaiseClosureNameError("nlp"); __PYX_ERR(0, 96, __pyx_L1_error) }
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_outer_scope->__pyx_v_nlp, __pyx_n_s_get_pipe_meta); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 96, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (unlikely(!__pyx_cur_scope->__pyx_outer_scope->__pyx_8genexpr1__pyx_v_name)) { __Pyx_RaiseClosureNameError("name"); __PYX_ERR(0, 94, __pyx_L1_error) }
+  if (unlikely(!__pyx_cur_scope->__pyx_outer_scope->__pyx_8genexpr1__pyx_v_name)) { __Pyx_RaiseClosureNameError("name"); __PYX_ERR(0, 96, __pyx_L1_error) }
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_cur_scope->__pyx_outer_scope->__pyx_8genexpr1__pyx_v_name) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_cur_scope->__pyx_outer_scope->__pyx_8genexpr1__pyx_v_name);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 94, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 96, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_assigns); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_assigns); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 96, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (likely(PyList_CheckExact(__pyx_t_2)) || PyTuple_CheckExact(__pyx_t_2)) {
     __pyx_t_1 = __pyx_t_2; __Pyx_INCREF(__pyx_t_1); __pyx_t_4 = 0;
     __pyx_t_5 = NULL;
   } else {
-    __pyx_t_4 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 94, __pyx_L1_error)
+    __pyx_t_4 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 96, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_5 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 94, __pyx_L1_error)
+    __pyx_t_5 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 96, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   for (;;) {
     if (likely(!__pyx_t_5)) {
       if (likely(PyList_CheckExact(__pyx_t_1))) {
         if (__pyx_t_4 >= PyList_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_2 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 94, __pyx_L1_error)
+        __pyx_t_2 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 96, __pyx_L1_error)
         #else
-        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 94, __pyx_L1_error)
+        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 96, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         #endif
       } else {
         if (__pyx_t_4 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 94, __pyx_L1_error)
+        __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 96, __pyx_L1_error)
         #else
-        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 94, __pyx_L1_error)
+        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 96, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         #endif
       }
     } else {
       __pyx_t_2 = __pyx_t_5(__pyx_t_1);
       if (unlikely(!__pyx_t_2)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 94, __pyx_L1_error)
+          else __PYX_ERR(0, 96, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_2);
     }
     __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_assign);
     __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_assign, __pyx_t_2);
     __Pyx_GIVEREF(__pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "edsnlp/matchers/phrase.pyx":93
+    /* "edsnlp/matchers/phrase.pyx":95
  *             for name, pipe in nlp.pipeline
  *             if any(
  *                 "token" in assign and not assign == "token.is_sent_start"             # <<<<<<<<<<<<<<
  *                 for assign in nlp.get_pipe_meta(name).assigns
  *             )
  */
-    __pyx_t_7 = (__Pyx_PySequence_ContainsTF(__pyx_n_u_token, __pyx_cur_scope->__pyx_v_assign, Py_EQ)); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 93, __pyx_L1_error)
+    __pyx_t_7 = (__Pyx_PySequence_ContainsTF(__pyx_n_u_token, __pyx_cur_scope->__pyx_v_assign, Py_EQ)); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 95, __pyx_L1_error)
     __pyx_t_8 = (__pyx_t_7 != 0);
     if (__pyx_t_8) {
     } else {
       __pyx_t_6 = __pyx_t_8;
       goto __pyx_L7_bool_binop_done;
     }
-    __pyx_t_8 = (__Pyx_PyUnicode_Equals(__pyx_cur_scope->__pyx_v_assign, __pyx_kp_u_token_is_sent_start, Py_EQ)); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 93, __pyx_L1_error)
+    __pyx_t_8 = (__Pyx_PyUnicode_Equals(__pyx_cur_scope->__pyx_v_assign, __pyx_kp_u_token_is_sent_start, Py_EQ)); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 95, __pyx_L1_error)
     __pyx_t_7 = ((!__pyx_t_8) != 0);
     __pyx_t_6 = __pyx_t_7;
     __pyx_L7_bool_binop_done:;
     if (__pyx_t_6) {
 
-      /* "edsnlp/matchers/phrase.pyx":92
+      /* "edsnlp/matchers/phrase.pyx":94
  *             name
  *             for name, pipe in nlp.pipeline
  *             if any(             # <<<<<<<<<<<<<<
  *                 "token" in assign and not assign == "token.is_sent_start"
  *                 for assign in nlp.get_pipe_meta(name).assigns
  */
       __Pyx_XDECREF(__pyx_r);
 
-      /* "edsnlp/matchers/phrase.pyx":93
+      /* "edsnlp/matchers/phrase.pyx":95
  *             for name, pipe in nlp.pipeline
  *             if any(
  *                 "token" in assign and not assign == "token.is_sent_start"             # <<<<<<<<<<<<<<
  *                 for assign in nlp.get_pipe_meta(name).assigns
  *             )
  */
       __Pyx_INCREF(Py_True);
       __pyx_r = Py_True;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       goto __pyx_L0;
     }
 
-    /* "edsnlp/matchers/phrase.pyx":94
+    /* "edsnlp/matchers/phrase.pyx":96
  *             if any(
  *                 "token" in assign and not assign == "token.is_sent_start"
  *                 for assign in nlp.get_pipe_meta(name).assigns             # <<<<<<<<<<<<<<
  *             )
  *         ]
  */
   }
   /*else*/ {
 
-    /* "edsnlp/matchers/phrase.pyx":92
+    /* "edsnlp/matchers/phrase.pyx":94
  *             name
  *             for name, pipe in nlp.pipeline
  *             if any(             # <<<<<<<<<<<<<<
  *                 "token" in assign and not assign == "token.is_sent_start"
  *                 for assign in nlp.get_pipe_meta(name).assigns
  */
     __Pyx_XDECREF(__pyx_r);
 
-    /* "edsnlp/matchers/phrase.pyx":93
+    /* "edsnlp/matchers/phrase.pyx":95
  *             for name, pipe in nlp.pipeline
  *             if any(
  *                 "token" in assign and not assign == "token.is_sent_start"             # <<<<<<<<<<<<<<
  *                 for assign in nlp.get_pipe_meta(name).assigns
  *             )
  */
     __Pyx_INCREF(Py_False);
     __pyx_r = Py_False;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     goto __pyx_L0;
   }
 
-  /* "edsnlp/matchers/phrase.pyx":94
+  /* "edsnlp/matchers/phrase.pyx":96
  *             if any(
  *                 "token" in assign and not assign == "token.is_sent_start"
  *                 for assign in nlp.get_pipe_meta(name).assigns             # <<<<<<<<<<<<<<
  *             )
  *         ]
  */
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
 
-  /* "edsnlp/matchers/phrase.pyx":93
+  /* "edsnlp/matchers/phrase.pyx":95
  *             for name, pipe in nlp.pipeline
  *             if any(
  *                 "token" in assign and not assign == "token.is_sent_start"             # <<<<<<<<<<<<<<
  *                 for assign in nlp.get_pipe_meta(name).assigns
  *             )
  */
 
@@ -5881,20 +5906,20 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "edsnlp/matchers/phrase.pyx":73
  *             Span.set_extension("normalized_variant", getter=get_normalized_variant)
  * 
- *     def build_patterns(self, nlp: Language, terms: Patterns):             # <<<<<<<<<<<<<<
+ *     def build_patterns(self, nlp: Language, terms: Patterns, progress: bool = False):             # <<<<<<<<<<<<<<
  *         """
  *         Build patterns and adds them for matching.
  */
 
-static PyObject *__pyx_pf_6edsnlp_8matchers_6phrase_16EDSPhraseMatcher_4build_patterns(struct __pyx_obj_6edsnlp_8matchers_6phrase_EDSPhraseMatcher *__pyx_v_self, PyObject *__pyx_v_nlp, PyObject *__pyx_v_terms) {
+static PyObject *__pyx_pf_6edsnlp_8matchers_6phrase_16EDSPhraseMatcher_4build_patterns(struct __pyx_obj_6edsnlp_8matchers_6phrase_EDSPhraseMatcher *__pyx_v_self, PyObject *__pyx_v_nlp, PyObject *__pyx_v_terms, PyObject *__pyx_v_progress) {
   struct __pyx_obj_6edsnlp_8matchers_6phrase___pyx_scope_struct__build_patterns *__pyx_cur_scope;
   PyObject *__pyx_v_token_pipelines = NULL;
   PyObject *__pyx_v_key = NULL;
   PyObject *__pyx_v_expressions = NULL;
   PyObject *__pyx_v_attr = NULL;
   PyObject *__pyx_v_patterns = NULL;
   CYTHON_UNUSED PyObject *__pyx_8genexpr1__pyx_v_pipe = NULL;
@@ -5933,202 +5958,202 @@
   }
   __Pyx_TraceCall("build_patterns", __pyx_f[0], 73, 0, __PYX_ERR(0, 73, __pyx_L1_error));
   __pyx_cur_scope->__pyx_v_nlp = __pyx_v_nlp;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_nlp);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_nlp);
   __Pyx_INCREF(__pyx_v_terms);
 
-  /* "edsnlp/matchers/phrase.pyx":86
+  /* "edsnlp/matchers/phrase.pyx":88
  *         """
  * 
  *         if not terms:             # <<<<<<<<<<<<<<
  *             terms = dict()
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_terms); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_terms); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 88, __pyx_L1_error)
   __pyx_t_2 = ((!__pyx_t_1) != 0);
   if (__pyx_t_2) {
 
-    /* "edsnlp/matchers/phrase.pyx":87
+    /* "edsnlp/matchers/phrase.pyx":89
  * 
  *         if not terms:
  *             terms = dict()             # <<<<<<<<<<<<<<
  * 
  *         token_pipelines = [
  */
-    __pyx_t_3 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 87, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 89, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF_SET(__pyx_v_terms, __pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "edsnlp/matchers/phrase.pyx":86
+    /* "edsnlp/matchers/phrase.pyx":88
  *         """
  * 
  *         if not terms:             # <<<<<<<<<<<<<<
  *             terms = dict()
  * 
  */
   }
 
-  /* "edsnlp/matchers/phrase.pyx":89
+  /* "edsnlp/matchers/phrase.pyx":91
  *             terms = dict()
  * 
  *         token_pipelines = [             # <<<<<<<<<<<<<<
  *             name
  *             for name, pipe in nlp.pipeline
  */
   { /* enter inner scope */
-    __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 89, __pyx_L6_error)
+    __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 91, __pyx_L6_error)
     __Pyx_GOTREF(__pyx_t_3);
 
-    /* "edsnlp/matchers/phrase.pyx":91
+    /* "edsnlp/matchers/phrase.pyx":93
  *         token_pipelines = [
  *             name
  *             for name, pipe in nlp.pipeline             # <<<<<<<<<<<<<<
  *             if any(
  *                 "token" in assign and not assign == "token.is_sent_start"
  */
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_nlp, __pyx_n_s_pipeline); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 91, __pyx_L6_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_nlp, __pyx_n_s_pipeline); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 93, __pyx_L6_error)
     __Pyx_GOTREF(__pyx_t_4);
     if (likely(PyList_CheckExact(__pyx_t_4)) || PyTuple_CheckExact(__pyx_t_4)) {
       __pyx_t_5 = __pyx_t_4; __Pyx_INCREF(__pyx_t_5); __pyx_t_6 = 0;
       __pyx_t_7 = NULL;
     } else {
-      __pyx_t_6 = -1; __pyx_t_5 = PyObject_GetIter(__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 91, __pyx_L6_error)
+      __pyx_t_6 = -1; __pyx_t_5 = PyObject_GetIter(__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 93, __pyx_L6_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_7 = Py_TYPE(__pyx_t_5)->tp_iternext; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 91, __pyx_L6_error)
+      __pyx_t_7 = Py_TYPE(__pyx_t_5)->tp_iternext; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 93, __pyx_L6_error)
     }
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     for (;;) {
       if (likely(!__pyx_t_7)) {
         if (likely(PyList_CheckExact(__pyx_t_5))) {
           if (__pyx_t_6 >= PyList_GET_SIZE(__pyx_t_5)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_4 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_6); __Pyx_INCREF(__pyx_t_4); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 91, __pyx_L6_error)
+          __pyx_t_4 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_6); __Pyx_INCREF(__pyx_t_4); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 93, __pyx_L6_error)
           #else
-          __pyx_t_4 = PySequence_ITEM(__pyx_t_5, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 91, __pyx_L6_error)
+          __pyx_t_4 = PySequence_ITEM(__pyx_t_5, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 93, __pyx_L6_error)
           __Pyx_GOTREF(__pyx_t_4);
           #endif
         } else {
           if (__pyx_t_6 >= PyTuple_GET_SIZE(__pyx_t_5)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_5, __pyx_t_6); __Pyx_INCREF(__pyx_t_4); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 91, __pyx_L6_error)
+          __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_5, __pyx_t_6); __Pyx_INCREF(__pyx_t_4); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 93, __pyx_L6_error)
           #else
-          __pyx_t_4 = PySequence_ITEM(__pyx_t_5, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 91, __pyx_L6_error)
+          __pyx_t_4 = PySequence_ITEM(__pyx_t_5, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 93, __pyx_L6_error)
           __Pyx_GOTREF(__pyx_t_4);
           #endif
         }
       } else {
         __pyx_t_4 = __pyx_t_7(__pyx_t_5);
         if (unlikely(!__pyx_t_4)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 91, __pyx_L6_error)
+            else __PYX_ERR(0, 93, __pyx_L6_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_4);
       }
       if ((likely(PyTuple_CheckExact(__pyx_t_4))) || (PyList_CheckExact(__pyx_t_4))) {
         PyObject* sequence = __pyx_t_4;
         Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
         if (unlikely(size != 2)) {
           if (size > 2) __Pyx_RaiseTooManyValuesError(2);
           else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-          __PYX_ERR(0, 91, __pyx_L6_error)
+          __PYX_ERR(0, 93, __pyx_L6_error)
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
         if (likely(PyTuple_CheckExact(sequence))) {
           __pyx_t_8 = PyTuple_GET_ITEM(sequence, 0); 
           __pyx_t_9 = PyTuple_GET_ITEM(sequence, 1); 
         } else {
           __pyx_t_8 = PyList_GET_ITEM(sequence, 0); 
           __pyx_t_9 = PyList_GET_ITEM(sequence, 1); 
         }
         __Pyx_INCREF(__pyx_t_8);
         __Pyx_INCREF(__pyx_t_9);
         #else
-        __pyx_t_8 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 91, __pyx_L6_error)
+        __pyx_t_8 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 93, __pyx_L6_error)
         __Pyx_GOTREF(__pyx_t_8);
-        __pyx_t_9 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 91, __pyx_L6_error)
+        __pyx_t_9 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 93, __pyx_L6_error)
         __Pyx_GOTREF(__pyx_t_9);
         #endif
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       } else {
         Py_ssize_t index = -1;
-        __pyx_t_10 = PyObject_GetIter(__pyx_t_4); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 91, __pyx_L6_error)
+        __pyx_t_10 = PyObject_GetIter(__pyx_t_4); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 93, __pyx_L6_error)
         __Pyx_GOTREF(__pyx_t_10);
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
         __pyx_t_11 = Py_TYPE(__pyx_t_10)->tp_iternext;
         index = 0; __pyx_t_8 = __pyx_t_11(__pyx_t_10); if (unlikely(!__pyx_t_8)) goto __pyx_L9_unpacking_failed;
         __Pyx_GOTREF(__pyx_t_8);
         index = 1; __pyx_t_9 = __pyx_t_11(__pyx_t_10); if (unlikely(!__pyx_t_9)) goto __pyx_L9_unpacking_failed;
         __Pyx_GOTREF(__pyx_t_9);
-        if (__Pyx_IternextUnpackEndCheck(__pyx_t_11(__pyx_t_10), 2) < 0) __PYX_ERR(0, 91, __pyx_L6_error)
+        if (__Pyx_IternextUnpackEndCheck(__pyx_t_11(__pyx_t_10), 2) < 0) __PYX_ERR(0, 93, __pyx_L6_error)
         __pyx_t_11 = NULL;
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
         goto __pyx_L10_unpacking_done;
         __pyx_L9_unpacking_failed:;
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
         __pyx_t_11 = NULL;
         if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-        __PYX_ERR(0, 91, __pyx_L6_error)
+        __PYX_ERR(0, 93, __pyx_L6_error)
         __pyx_L10_unpacking_done:;
       }
       __Pyx_XGOTREF(__pyx_cur_scope->__pyx_8genexpr1__pyx_v_name);
       __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_8genexpr1__pyx_v_name, __pyx_t_8);
       __Pyx_GIVEREF(__pyx_t_8);
       __pyx_t_8 = 0;
       __Pyx_XDECREF_SET(__pyx_8genexpr1__pyx_v_pipe, __pyx_t_9);
       __pyx_t_9 = 0;
 
-      /* "edsnlp/matchers/phrase.pyx":93
+      /* "edsnlp/matchers/phrase.pyx":95
  *             for name, pipe in nlp.pipeline
  *             if any(
  *                 "token" in assign and not assign == "token.is_sent_start"             # <<<<<<<<<<<<<<
  *                 for assign in nlp.get_pipe_meta(name).assigns
  *             )
  */
-      __pyx_t_4 = __pyx_pf_6edsnlp_8matchers_6phrase_16EDSPhraseMatcher_14build_patterns_8genexpr1_genexpr(((PyObject*)__pyx_cur_scope)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 93, __pyx_L6_error)
+      __pyx_t_4 = __pyx_pf_6edsnlp_8matchers_6phrase_16EDSPhraseMatcher_14build_patterns_8genexpr1_genexpr(((PyObject*)__pyx_cur_scope)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 95, __pyx_L6_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_9 = __Pyx_Generator_Next(__pyx_t_4); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 93, __pyx_L6_error)
+      __pyx_t_9 = __Pyx_Generator_Next(__pyx_t_4); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 95, __pyx_L6_error)
       __Pyx_GOTREF(__pyx_t_9);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 93, __pyx_L6_error)
+      __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 95, __pyx_L6_error)
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-      /* "edsnlp/matchers/phrase.pyx":92
+      /* "edsnlp/matchers/phrase.pyx":94
  *             name
  *             for name, pipe in nlp.pipeline
  *             if any(             # <<<<<<<<<<<<<<
  *                 "token" in assign and not assign == "token.is_sent_start"
  *                 for assign in nlp.get_pipe_meta(name).assigns
  */
       if (__pyx_t_2) {
 
-        /* "edsnlp/matchers/phrase.pyx":90
+        /* "edsnlp/matchers/phrase.pyx":92
  * 
  *         token_pipelines = [
  *             name             # <<<<<<<<<<<<<<
  *             for name, pipe in nlp.pipeline
  *             if any(
  */
-        if (unlikely(__Pyx_ListComp_Append(__pyx_t_3, (PyObject*)__pyx_cur_scope->__pyx_8genexpr1__pyx_v_name))) __PYX_ERR(0, 89, __pyx_L6_error)
+        if (unlikely(__Pyx_ListComp_Append(__pyx_t_3, (PyObject*)__pyx_cur_scope->__pyx_8genexpr1__pyx_v_name))) __PYX_ERR(0, 91, __pyx_L6_error)
 
-        /* "edsnlp/matchers/phrase.pyx":92
+        /* "edsnlp/matchers/phrase.pyx":94
  *             name
  *             for name, pipe in nlp.pipeline
  *             if any(             # <<<<<<<<<<<<<<
  *                 "token" in assign and not assign == "token.is_sent_start"
  *                 for assign in nlp.get_pipe_meta(name).assigns
  */
       }
 
-      /* "edsnlp/matchers/phrase.pyx":91
+      /* "edsnlp/matchers/phrase.pyx":93
  *         token_pipelines = [
  *             name
  *             for name, pipe in nlp.pipeline             # <<<<<<<<<<<<<<
  *             if any(
  *                 "token" in assign and not assign == "token.is_sent_start"
  */
     }
@@ -6139,451 +6164,500 @@
     __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_pipe); __pyx_8genexpr1__pyx_v_pipe = 0;
     goto __pyx_L1_error;
     __pyx_L12_exit_scope:;
   } /* exit inner scope */
   __pyx_v_token_pipelines = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "edsnlp/matchers/phrase.pyx":97
+  /* "edsnlp/matchers/phrase.pyx":99
  *             )
  *         ]
  *         with nlp.select_pipes(enable=token_pipelines):             # <<<<<<<<<<<<<<
- *             for key, expressions in tqdm(
+ *             for key, expressions in (tqdm(
  *                 terms.items(),
  */
   /*with:*/ {
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_nlp, __pyx_n_s_select_pipes); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 97, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_nlp, __pyx_n_s_select_pipes); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 99, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 97, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 99, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_enable, __pyx_v_token_pipelines) < 0) __PYX_ERR(0, 97, __pyx_L1_error)
-    __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_empty_tuple, __pyx_t_5); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 97, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_enable, __pyx_v_token_pipelines) < 0) __PYX_ERR(0, 99, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_empty_tuple, __pyx_t_5); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 99, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_12 = __Pyx_PyObject_LookupSpecial(__pyx_t_9, __pyx_n_s_exit); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 97, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyObject_LookupSpecial(__pyx_t_9, __pyx_n_s_exit); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 99, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_12);
-    __pyx_t_3 = __Pyx_PyObject_LookupSpecial(__pyx_t_9, __pyx_n_s_enter); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 97, __pyx_L13_error)
+    __pyx_t_3 = __Pyx_PyObject_LookupSpecial(__pyx_t_9, __pyx_n_s_enter); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 99, __pyx_L13_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_5 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 97, __pyx_L13_error)
+    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 99, __pyx_L13_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     /*try:*/ {
       {
         __Pyx_PyThreadState_declare
         __Pyx_PyThreadState_assign
         __Pyx_ExceptionSave(&__pyx_t_13, &__pyx_t_14, &__pyx_t_15);
         __Pyx_XGOTREF(__pyx_t_13);
         __Pyx_XGOTREF(__pyx_t_14);
         __Pyx_XGOTREF(__pyx_t_15);
         /*try:*/ {
 
-          /* "edsnlp/matchers/phrase.pyx":98
+          /* "edsnlp/matchers/phrase.pyx":103
+ *                 terms.items(),
+ *                 desc="Adding terms into the pipeline"
+ *             ) if progress else terms.items()):             # <<<<<<<<<<<<<<
+ *                 if isinstance(expressions, dict):
+ *                     attr = expressions.get("attr")
+ */
+          __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_progress); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 103, __pyx_L17_error)
+          if (__pyx_t_2) {
+
+            /* "edsnlp/matchers/phrase.pyx":100
  *         ]
  *         with nlp.select_pipes(enable=token_pipelines):
- *             for key, expressions in tqdm(             # <<<<<<<<<<<<<<
+ *             for key, expressions in (tqdm(             # <<<<<<<<<<<<<<
  *                 terms.items(),
  *                 desc="Adding terms into the pipeline"
  */
-          __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_tqdm); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 98, __pyx_L17_error)
-          __Pyx_GOTREF(__pyx_t_9);
+            __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_tqdm); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 100, __pyx_L17_error)
+            __Pyx_GOTREF(__pyx_t_5);
 
-          /* "edsnlp/matchers/phrase.pyx":99
+            /* "edsnlp/matchers/phrase.pyx":101
  *         with nlp.select_pipes(enable=token_pipelines):
- *             for key, expressions in tqdm(
+ *             for key, expressions in (tqdm(
  *                 terms.items(),             # <<<<<<<<<<<<<<
  *                 desc="Adding terms into the pipeline"
- *             ):
+ *             ) if progress else terms.items()):
  */
-          __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_terms, __pyx_n_s_items); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 99, __pyx_L17_error)
-          __Pyx_GOTREF(__pyx_t_3);
-          __pyx_t_4 = NULL;
-          if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
-            __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
-            if (likely(__pyx_t_4)) {
-              PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-              __Pyx_INCREF(__pyx_t_4);
-              __Pyx_INCREF(function);
-              __Pyx_DECREF_SET(__pyx_t_3, function);
+            __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_terms, __pyx_n_s_items); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 101, __pyx_L17_error)
+            __Pyx_GOTREF(__pyx_t_4);
+            __pyx_t_8 = NULL;
+            if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
+              __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_4);
+              if (likely(__pyx_t_8)) {
+                PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+                __Pyx_INCREF(__pyx_t_8);
+                __Pyx_INCREF(function);
+                __Pyx_DECREF_SET(__pyx_t_4, function);
+              }
             }
-          }
-          __pyx_t_5 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
-          __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-          if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 99, __pyx_L17_error)
-          __Pyx_GOTREF(__pyx_t_5);
-          __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+            __pyx_t_3 = (__pyx_t_8) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_8) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
+            __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+            if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 101, __pyx_L17_error)
+            __Pyx_GOTREF(__pyx_t_3);
+            __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-          /* "edsnlp/matchers/phrase.pyx":98
+            /* "edsnlp/matchers/phrase.pyx":100
  *         ]
  *         with nlp.select_pipes(enable=token_pipelines):
- *             for key, expressions in tqdm(             # <<<<<<<<<<<<<<
+ *             for key, expressions in (tqdm(             # <<<<<<<<<<<<<<
  *                 terms.items(),
  *                 desc="Adding terms into the pipeline"
  */
-          __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 98, __pyx_L17_error)
-          __Pyx_GOTREF(__pyx_t_3);
-          __Pyx_GIVEREF(__pyx_t_5);
-          PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_5);
-          __pyx_t_5 = 0;
+            __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 100, __pyx_L17_error)
+            __Pyx_GOTREF(__pyx_t_4);
+            __Pyx_GIVEREF(__pyx_t_3);
+            PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_3);
+            __pyx_t_3 = 0;
 
-          /* "edsnlp/matchers/phrase.pyx":100
- *             for key, expressions in tqdm(
+            /* "edsnlp/matchers/phrase.pyx":102
+ *             for key, expressions in (tqdm(
  *                 terms.items(),
  *                 desc="Adding terms into the pipeline"             # <<<<<<<<<<<<<<
- *             ):
+ *             ) if progress else terms.items()):
  *                 if isinstance(expressions, dict):
  */
-          __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 100, __pyx_L17_error)
-          __Pyx_GOTREF(__pyx_t_5);
-          if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_desc, __pyx_kp_u_Adding_terms_into_the_pipeline) < 0) __PYX_ERR(0, 100, __pyx_L17_error)
+            __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 102, __pyx_L17_error)
+            __Pyx_GOTREF(__pyx_t_3);
+            if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_desc, __pyx_kp_u_Adding_terms_into_the_pipeline) < 0) __PYX_ERR(0, 102, __pyx_L17_error)
 
-          /* "edsnlp/matchers/phrase.pyx":98
+            /* "edsnlp/matchers/phrase.pyx":100
  *         ]
  *         with nlp.select_pipes(enable=token_pipelines):
- *             for key, expressions in tqdm(             # <<<<<<<<<<<<<<
+ *             for key, expressions in (tqdm(             # <<<<<<<<<<<<<<
  *                 terms.items(),
  *                 desc="Adding terms into the pipeline"
  */
-          __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_t_3, __pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 98, __pyx_L17_error)
-          __Pyx_GOTREF(__pyx_t_4);
-          __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-          __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-          __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-          if (likely(PyList_CheckExact(__pyx_t_4)) || PyTuple_CheckExact(__pyx_t_4)) {
-            __pyx_t_5 = __pyx_t_4; __Pyx_INCREF(__pyx_t_5); __pyx_t_6 = 0;
+            __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_4, __pyx_t_3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 100, __pyx_L17_error)
+            __Pyx_GOTREF(__pyx_t_8);
+            __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+            __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+            __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+            __pyx_t_9 = __pyx_t_8;
+            __pyx_t_8 = 0;
+          } else {
+
+            /* "edsnlp/matchers/phrase.pyx":103
+ *                 terms.items(),
+ *                 desc="Adding terms into the pipeline"
+ *             ) if progress else terms.items()):             # <<<<<<<<<<<<<<
+ *                 if isinstance(expressions, dict):
+ *                     attr = expressions.get("attr")
+ */
+            __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_terms, __pyx_n_s_items); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 103, __pyx_L17_error)
+            __Pyx_GOTREF(__pyx_t_3);
+            __pyx_t_4 = NULL;
+            if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
+              __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
+              if (likely(__pyx_t_4)) {
+                PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+                __Pyx_INCREF(__pyx_t_4);
+                __Pyx_INCREF(function);
+                __Pyx_DECREF_SET(__pyx_t_3, function);
+              }
+            }
+            __pyx_t_8 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
+            __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+            if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 103, __pyx_L17_error)
+            __Pyx_GOTREF(__pyx_t_8);
+            __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+            __pyx_t_9 = __pyx_t_8;
+            __pyx_t_8 = 0;
+          }
+
+          /* "edsnlp/matchers/phrase.pyx":100
+ *         ]
+ *         with nlp.select_pipes(enable=token_pipelines):
+ *             for key, expressions in (tqdm(             # <<<<<<<<<<<<<<
+ *                 terms.items(),
+ *                 desc="Adding terms into the pipeline"
+ */
+          if (likely(PyList_CheckExact(__pyx_t_9)) || PyTuple_CheckExact(__pyx_t_9)) {
+            __pyx_t_8 = __pyx_t_9; __Pyx_INCREF(__pyx_t_8); __pyx_t_6 = 0;
             __pyx_t_7 = NULL;
           } else {
-            __pyx_t_6 = -1; __pyx_t_5 = PyObject_GetIter(__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 98, __pyx_L17_error)
-            __Pyx_GOTREF(__pyx_t_5);
-            __pyx_t_7 = Py_TYPE(__pyx_t_5)->tp_iternext; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 98, __pyx_L17_error)
+            __pyx_t_6 = -1; __pyx_t_8 = PyObject_GetIter(__pyx_t_9); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 100, __pyx_L17_error)
+            __Pyx_GOTREF(__pyx_t_8);
+            __pyx_t_7 = Py_TYPE(__pyx_t_8)->tp_iternext; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 100, __pyx_L17_error)
           }
-          __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+          __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
           for (;;) {
             if (likely(!__pyx_t_7)) {
-              if (likely(PyList_CheckExact(__pyx_t_5))) {
-                if (__pyx_t_6 >= PyList_GET_SIZE(__pyx_t_5)) break;
+              if (likely(PyList_CheckExact(__pyx_t_8))) {
+                if (__pyx_t_6 >= PyList_GET_SIZE(__pyx_t_8)) break;
                 #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-                __pyx_t_4 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_6); __Pyx_INCREF(__pyx_t_4); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 98, __pyx_L17_error)
+                __pyx_t_9 = PyList_GET_ITEM(__pyx_t_8, __pyx_t_6); __Pyx_INCREF(__pyx_t_9); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 100, __pyx_L17_error)
                 #else
-                __pyx_t_4 = PySequence_ITEM(__pyx_t_5, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 98, __pyx_L17_error)
-                __Pyx_GOTREF(__pyx_t_4);
+                __pyx_t_9 = PySequence_ITEM(__pyx_t_8, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 100, __pyx_L17_error)
+                __Pyx_GOTREF(__pyx_t_9);
                 #endif
               } else {
-                if (__pyx_t_6 >= PyTuple_GET_SIZE(__pyx_t_5)) break;
+                if (__pyx_t_6 >= PyTuple_GET_SIZE(__pyx_t_8)) break;
                 #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-                __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_5, __pyx_t_6); __Pyx_INCREF(__pyx_t_4); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 98, __pyx_L17_error)
+                __pyx_t_9 = PyTuple_GET_ITEM(__pyx_t_8, __pyx_t_6); __Pyx_INCREF(__pyx_t_9); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 100, __pyx_L17_error)
                 #else
-                __pyx_t_4 = PySequence_ITEM(__pyx_t_5, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 98, __pyx_L17_error)
-                __Pyx_GOTREF(__pyx_t_4);
+                __pyx_t_9 = PySequence_ITEM(__pyx_t_8, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 100, __pyx_L17_error)
+                __Pyx_GOTREF(__pyx_t_9);
                 #endif
               }
             } else {
-              __pyx_t_4 = __pyx_t_7(__pyx_t_5);
-              if (unlikely(!__pyx_t_4)) {
+              __pyx_t_9 = __pyx_t_7(__pyx_t_8);
+              if (unlikely(!__pyx_t_9)) {
                 PyObject* exc_type = PyErr_Occurred();
                 if (exc_type) {
                   if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-                  else __PYX_ERR(0, 98, __pyx_L17_error)
+                  else __PYX_ERR(0, 100, __pyx_L17_error)
                 }
                 break;
               }
-              __Pyx_GOTREF(__pyx_t_4);
+              __Pyx_GOTREF(__pyx_t_9);
             }
-            if ((likely(PyTuple_CheckExact(__pyx_t_4))) || (PyList_CheckExact(__pyx_t_4))) {
-              PyObject* sequence = __pyx_t_4;
+            if ((likely(PyTuple_CheckExact(__pyx_t_9))) || (PyList_CheckExact(__pyx_t_9))) {
+              PyObject* sequence = __pyx_t_9;
               Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
               if (unlikely(size != 2)) {
                 if (size > 2) __Pyx_RaiseTooManyValuesError(2);
                 else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-                __PYX_ERR(0, 98, __pyx_L17_error)
+                __PYX_ERR(0, 100, __pyx_L17_error)
               }
               #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
               if (likely(PyTuple_CheckExact(sequence))) {
                 __pyx_t_3 = PyTuple_GET_ITEM(sequence, 0); 
-                __pyx_t_9 = PyTuple_GET_ITEM(sequence, 1); 
+                __pyx_t_4 = PyTuple_GET_ITEM(sequence, 1); 
               } else {
                 __pyx_t_3 = PyList_GET_ITEM(sequence, 0); 
-                __pyx_t_9 = PyList_GET_ITEM(sequence, 1); 
+                __pyx_t_4 = PyList_GET_ITEM(sequence, 1); 
               }
               __Pyx_INCREF(__pyx_t_3);
-              __Pyx_INCREF(__pyx_t_9);
+              __Pyx_INCREF(__pyx_t_4);
               #else
-              __pyx_t_3 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 98, __pyx_L17_error)
+              __pyx_t_3 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 100, __pyx_L17_error)
               __Pyx_GOTREF(__pyx_t_3);
-              __pyx_t_9 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 98, __pyx_L17_error)
-              __Pyx_GOTREF(__pyx_t_9);
+              __pyx_t_4 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 100, __pyx_L17_error)
+              __Pyx_GOTREF(__pyx_t_4);
               #endif
-              __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+              __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
             } else {
               Py_ssize_t index = -1;
-              __pyx_t_8 = PyObject_GetIter(__pyx_t_4); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 98, __pyx_L17_error)
-              __Pyx_GOTREF(__pyx_t_8);
-              __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-              __pyx_t_11 = Py_TYPE(__pyx_t_8)->tp_iternext;
-              index = 0; __pyx_t_3 = __pyx_t_11(__pyx_t_8); if (unlikely(!__pyx_t_3)) goto __pyx_L25_unpacking_failed;
+              __pyx_t_5 = PyObject_GetIter(__pyx_t_9); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 100, __pyx_L17_error)
+              __Pyx_GOTREF(__pyx_t_5);
+              __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+              __pyx_t_11 = Py_TYPE(__pyx_t_5)->tp_iternext;
+              index = 0; __pyx_t_3 = __pyx_t_11(__pyx_t_5); if (unlikely(!__pyx_t_3)) goto __pyx_L25_unpacking_failed;
               __Pyx_GOTREF(__pyx_t_3);
-              index = 1; __pyx_t_9 = __pyx_t_11(__pyx_t_8); if (unlikely(!__pyx_t_9)) goto __pyx_L25_unpacking_failed;
-              __Pyx_GOTREF(__pyx_t_9);
-              if (__Pyx_IternextUnpackEndCheck(__pyx_t_11(__pyx_t_8), 2) < 0) __PYX_ERR(0, 98, __pyx_L17_error)
+              index = 1; __pyx_t_4 = __pyx_t_11(__pyx_t_5); if (unlikely(!__pyx_t_4)) goto __pyx_L25_unpacking_failed;
+              __Pyx_GOTREF(__pyx_t_4);
+              if (__Pyx_IternextUnpackEndCheck(__pyx_t_11(__pyx_t_5), 2) < 0) __PYX_ERR(0, 100, __pyx_L17_error)
               __pyx_t_11 = NULL;
-              __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+              __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
               goto __pyx_L26_unpacking_done;
               __pyx_L25_unpacking_failed:;
-              __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+              __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
               __pyx_t_11 = NULL;
               if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-              __PYX_ERR(0, 98, __pyx_L17_error)
+              __PYX_ERR(0, 100, __pyx_L17_error)
               __pyx_L26_unpacking_done:;
             }
             __Pyx_XDECREF_SET(__pyx_v_key, __pyx_t_3);
             __pyx_t_3 = 0;
-            __Pyx_XDECREF_SET(__pyx_v_expressions, __pyx_t_9);
-            __pyx_t_9 = 0;
+            __Pyx_XDECREF_SET(__pyx_v_expressions, __pyx_t_4);
+            __pyx_t_4 = 0;
 
-            /* "edsnlp/matchers/phrase.pyx":102
+            /* "edsnlp/matchers/phrase.pyx":104
  *                 desc="Adding terms into the pipeline"
- *             ):
+ *             ) if progress else terms.items()):
  *                 if isinstance(expressions, dict):             # <<<<<<<<<<<<<<
  *                     attr = expressions.get("attr")
  *                     expressions = expressions.get("patterns")
  */
             __pyx_t_2 = PyDict_Check(__pyx_v_expressions); 
             __pyx_t_1 = (__pyx_t_2 != 0);
             if (__pyx_t_1) {
 
-              /* "edsnlp/matchers/phrase.pyx":103
- *             ):
+              /* "edsnlp/matchers/phrase.pyx":105
+ *             ) if progress else terms.items()):
  *                 if isinstance(expressions, dict):
  *                     attr = expressions.get("attr")             # <<<<<<<<<<<<<<
  *                     expressions = expressions.get("patterns")
  *                 else:
  */
-              __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_expressions, __pyx_n_s_get); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 103, __pyx_L17_error)
-              __Pyx_GOTREF(__pyx_t_9);
+              __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_expressions, __pyx_n_s_get); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 105, __pyx_L17_error)
+              __Pyx_GOTREF(__pyx_t_4);
               __pyx_t_3 = NULL;
-              if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_9))) {
-                __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_9);
+              if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
+                __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
                 if (likely(__pyx_t_3)) {
-                  PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
+                  PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
                   __Pyx_INCREF(__pyx_t_3);
                   __Pyx_INCREF(function);
-                  __Pyx_DECREF_SET(__pyx_t_9, function);
+                  __Pyx_DECREF_SET(__pyx_t_4, function);
                 }
               }
-              __pyx_t_4 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_9, __pyx_t_3, __pyx_n_u_attr) : __Pyx_PyObject_CallOneArg(__pyx_t_9, __pyx_n_u_attr);
+              __pyx_t_9 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_3, __pyx_n_u_attr) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_n_u_attr);
               __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-              if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 103, __pyx_L17_error)
-              __Pyx_GOTREF(__pyx_t_4);
-              __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-              __Pyx_XDECREF_SET(__pyx_v_attr, __pyx_t_4);
-              __pyx_t_4 = 0;
+              if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 105, __pyx_L17_error)
+              __Pyx_GOTREF(__pyx_t_9);
+              __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+              __Pyx_XDECREF_SET(__pyx_v_attr, __pyx_t_9);
+              __pyx_t_9 = 0;
 
-              /* "edsnlp/matchers/phrase.pyx":104
+              /* "edsnlp/matchers/phrase.pyx":106
  *                 if isinstance(expressions, dict):
  *                     attr = expressions.get("attr")
  *                     expressions = expressions.get("patterns")             # <<<<<<<<<<<<<<
  *                 else:
  *                     attr = None
  */
-              __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_expressions, __pyx_n_s_get); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 104, __pyx_L17_error)
-              __Pyx_GOTREF(__pyx_t_9);
+              __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_expressions, __pyx_n_s_get); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 106, __pyx_L17_error)
+              __Pyx_GOTREF(__pyx_t_4);
               __pyx_t_3 = NULL;
-              if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_9))) {
-                __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_9);
+              if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
+                __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
                 if (likely(__pyx_t_3)) {
-                  PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
+                  PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
                   __Pyx_INCREF(__pyx_t_3);
                   __Pyx_INCREF(function);
-                  __Pyx_DECREF_SET(__pyx_t_9, function);
+                  __Pyx_DECREF_SET(__pyx_t_4, function);
                 }
               }
-              __pyx_t_4 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_9, __pyx_t_3, __pyx_n_u_patterns) : __Pyx_PyObject_CallOneArg(__pyx_t_9, __pyx_n_u_patterns);
+              __pyx_t_9 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_3, __pyx_n_u_patterns) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_n_u_patterns);
               __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-              if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 104, __pyx_L17_error)
-              __Pyx_GOTREF(__pyx_t_4);
-              __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-              __Pyx_DECREF_SET(__pyx_v_expressions, __pyx_t_4);
-              __pyx_t_4 = 0;
+              if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 106, __pyx_L17_error)
+              __Pyx_GOTREF(__pyx_t_9);
+              __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+              __Pyx_DECREF_SET(__pyx_v_expressions, __pyx_t_9);
+              __pyx_t_9 = 0;
 
-              /* "edsnlp/matchers/phrase.pyx":102
+              /* "edsnlp/matchers/phrase.pyx":104
  *                 desc="Adding terms into the pipeline"
- *             ):
+ *             ) if progress else terms.items()):
  *                 if isinstance(expressions, dict):             # <<<<<<<<<<<<<<
  *                     attr = expressions.get("attr")
  *                     expressions = expressions.get("patterns")
  */
               goto __pyx_L27;
             }
 
-            /* "edsnlp/matchers/phrase.pyx":106
+            /* "edsnlp/matchers/phrase.pyx":108
  *                     expressions = expressions.get("patterns")
  *                 else:
  *                     attr = None             # <<<<<<<<<<<<<<
  *                 if isinstance(expressions, str):
  *                     expressions = [expressions]
  */
             /*else*/ {
               __Pyx_INCREF(Py_None);
               __Pyx_XDECREF_SET(__pyx_v_attr, Py_None);
             }
             __pyx_L27:;
 
-            /* "edsnlp/matchers/phrase.pyx":107
+            /* "edsnlp/matchers/phrase.pyx":109
  *                 else:
  *                     attr = None
  *                 if isinstance(expressions, str):             # <<<<<<<<<<<<<<
  *                     expressions = [expressions]
  *                 patterns = list(nlp.pipe(expressions))
  */
             __pyx_t_1 = PyUnicode_Check(__pyx_v_expressions); 
             __pyx_t_2 = (__pyx_t_1 != 0);
             if (__pyx_t_2) {
 
-              /* "edsnlp/matchers/phrase.pyx":108
+              /* "edsnlp/matchers/phrase.pyx":110
  *                     attr = None
  *                 if isinstance(expressions, str):
  *                     expressions = [expressions]             # <<<<<<<<<<<<<<
  *                 patterns = list(nlp.pipe(expressions))
  *                 self.add(key, patterns, attr)
  */
-              __pyx_t_4 = PyList_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 108, __pyx_L17_error)
-              __Pyx_GOTREF(__pyx_t_4);
+              __pyx_t_9 = PyList_New(1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 110, __pyx_L17_error)
+              __Pyx_GOTREF(__pyx_t_9);
               __Pyx_INCREF(__pyx_v_expressions);
               __Pyx_GIVEREF(__pyx_v_expressions);
-              PyList_SET_ITEM(__pyx_t_4, 0, __pyx_v_expressions);
-              __Pyx_DECREF_SET(__pyx_v_expressions, __pyx_t_4);
-              __pyx_t_4 = 0;
+              PyList_SET_ITEM(__pyx_t_9, 0, __pyx_v_expressions);
+              __Pyx_DECREF_SET(__pyx_v_expressions, __pyx_t_9);
+              __pyx_t_9 = 0;
 
-              /* "edsnlp/matchers/phrase.pyx":107
+              /* "edsnlp/matchers/phrase.pyx":109
  *                 else:
  *                     attr = None
  *                 if isinstance(expressions, str):             # <<<<<<<<<<<<<<
  *                     expressions = [expressions]
  *                 patterns = list(nlp.pipe(expressions))
  */
             }
 
-            /* "edsnlp/matchers/phrase.pyx":109
+            /* "edsnlp/matchers/phrase.pyx":111
  *                 if isinstance(expressions, str):
  *                     expressions = [expressions]
  *                 patterns = list(nlp.pipe(expressions))             # <<<<<<<<<<<<<<
  *                 self.add(key, patterns, attr)
  * 
  */
-            __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_nlp, __pyx_n_s_pipe); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 109, __pyx_L17_error)
-            __Pyx_GOTREF(__pyx_t_9);
+            __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_nlp, __pyx_n_s_pipe); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 111, __pyx_L17_error)
+            __Pyx_GOTREF(__pyx_t_4);
             __pyx_t_3 = NULL;
-            if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_9))) {
-              __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_9);
+            if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
+              __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
               if (likely(__pyx_t_3)) {
-                PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
+                PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
                 __Pyx_INCREF(__pyx_t_3);
                 __Pyx_INCREF(function);
-                __Pyx_DECREF_SET(__pyx_t_9, function);
+                __Pyx_DECREF_SET(__pyx_t_4, function);
               }
             }
-            __pyx_t_4 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_9, __pyx_t_3, __pyx_v_expressions) : __Pyx_PyObject_CallOneArg(__pyx_t_9, __pyx_v_expressions);
+            __pyx_t_9 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_3, __pyx_v_expressions) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_expressions);
             __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-            if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 109, __pyx_L17_error)
-            __Pyx_GOTREF(__pyx_t_4);
-            __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-            __pyx_t_9 = PySequence_List(__pyx_t_4); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 109, __pyx_L17_error)
+            if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 111, __pyx_L17_error)
             __Pyx_GOTREF(__pyx_t_9);
             __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-            __Pyx_XDECREF_SET(__pyx_v_patterns, ((PyObject*)__pyx_t_9));
-            __pyx_t_9 = 0;
+            __pyx_t_4 = PySequence_List(__pyx_t_9); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 111, __pyx_L17_error)
+            __Pyx_GOTREF(__pyx_t_4);
+            __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+            __Pyx_XDECREF_SET(__pyx_v_patterns, ((PyObject*)__pyx_t_4));
+            __pyx_t_4 = 0;
 
-            /* "edsnlp/matchers/phrase.pyx":110
+            /* "edsnlp/matchers/phrase.pyx":112
  *                     expressions = [expressions]
  *                 patterns = list(nlp.pipe(expressions))
  *                 self.add(key, patterns, attr)             # <<<<<<<<<<<<<<
  * 
  *     cdef void find_matches(self, Doc doc, int start_idx, int end_idx, vector[SpanC] *matches) nogil:
  */
-            __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_add); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 110, __pyx_L17_error)
-            __Pyx_GOTREF(__pyx_t_4);
+            __pyx_t_9 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_add); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 112, __pyx_L17_error)
+            __Pyx_GOTREF(__pyx_t_9);
             __pyx_t_3 = NULL;
             __pyx_t_16 = 0;
-            if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
-              __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
+            if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_9))) {
+              __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_9);
               if (likely(__pyx_t_3)) {
-                PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+                PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
                 __Pyx_INCREF(__pyx_t_3);
                 __Pyx_INCREF(function);
-                __Pyx_DECREF_SET(__pyx_t_4, function);
+                __Pyx_DECREF_SET(__pyx_t_9, function);
                 __pyx_t_16 = 1;
               }
             }
             #if CYTHON_FAST_PYCALL
-            if (PyFunction_Check(__pyx_t_4)) {
+            if (PyFunction_Check(__pyx_t_9)) {
               PyObject *__pyx_temp[4] = {__pyx_t_3, __pyx_v_key, __pyx_v_patterns, __pyx_v_attr};
-              __pyx_t_9 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_16, 3+__pyx_t_16); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 110, __pyx_L17_error)
+              __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_9, __pyx_temp+1-__pyx_t_16, 3+__pyx_t_16); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 112, __pyx_L17_error)
               __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-              __Pyx_GOTREF(__pyx_t_9);
+              __Pyx_GOTREF(__pyx_t_4);
             } else
             #endif
             #if CYTHON_FAST_PYCCALL
-            if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
+            if (__Pyx_PyFastCFunction_Check(__pyx_t_9)) {
               PyObject *__pyx_temp[4] = {__pyx_t_3, __pyx_v_key, __pyx_v_patterns, __pyx_v_attr};
-              __pyx_t_9 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_16, 3+__pyx_t_16); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 110, __pyx_L17_error)
+              __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_9, __pyx_temp+1-__pyx_t_16, 3+__pyx_t_16); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 112, __pyx_L17_error)
               __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-              __Pyx_GOTREF(__pyx_t_9);
+              __Pyx_GOTREF(__pyx_t_4);
             } else
             #endif
             {
-              __pyx_t_8 = PyTuple_New(3+__pyx_t_16); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 110, __pyx_L17_error)
-              __Pyx_GOTREF(__pyx_t_8);
+              __pyx_t_5 = PyTuple_New(3+__pyx_t_16); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 112, __pyx_L17_error)
+              __Pyx_GOTREF(__pyx_t_5);
               if (__pyx_t_3) {
-                __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_3); __pyx_t_3 = NULL;
+                __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_3); __pyx_t_3 = NULL;
               }
               __Pyx_INCREF(__pyx_v_key);
               __Pyx_GIVEREF(__pyx_v_key);
-              PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_16, __pyx_v_key);
+              PyTuple_SET_ITEM(__pyx_t_5, 0+__pyx_t_16, __pyx_v_key);
               __Pyx_INCREF(__pyx_v_patterns);
               __Pyx_GIVEREF(__pyx_v_patterns);
-              PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_16, __pyx_v_patterns);
+              PyTuple_SET_ITEM(__pyx_t_5, 1+__pyx_t_16, __pyx_v_patterns);
               __Pyx_INCREF(__pyx_v_attr);
               __Pyx_GIVEREF(__pyx_v_attr);
-              PyTuple_SET_ITEM(__pyx_t_8, 2+__pyx_t_16, __pyx_v_attr);
-              __pyx_t_9 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_8, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 110, __pyx_L17_error)
-              __Pyx_GOTREF(__pyx_t_9);
-              __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+              PyTuple_SET_ITEM(__pyx_t_5, 2+__pyx_t_16, __pyx_v_attr);
+              __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_t_5, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 112, __pyx_L17_error)
+              __Pyx_GOTREF(__pyx_t_4);
+              __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
             }
-            __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
             __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+            __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-            /* "edsnlp/matchers/phrase.pyx":98
+            /* "edsnlp/matchers/phrase.pyx":100
  *         ]
  *         with nlp.select_pipes(enable=token_pipelines):
- *             for key, expressions in tqdm(             # <<<<<<<<<<<<<<
+ *             for key, expressions in (tqdm(             # <<<<<<<<<<<<<<
  *                 terms.items(),
  *                 desc="Adding terms into the pipeline"
  */
           }
-          __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+          __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-          /* "edsnlp/matchers/phrase.pyx":97
+          /* "edsnlp/matchers/phrase.pyx":99
  *             )
  *         ]
  *         with nlp.select_pipes(enable=token_pipelines):             # <<<<<<<<<<<<<<
- *             for key, expressions in tqdm(
+ *             for key, expressions in (tqdm(
  *                 terms.items(),
  */
         }
         __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
         __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
         __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
         goto __pyx_L22_try_end;
@@ -6592,40 +6666,40 @@
         __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
         __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
         __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
         __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
         /*except:*/ {
           __Pyx_AddTraceback("edsnlp.matchers.phrase.EDSPhraseMatcher.build_patterns", __pyx_clineno, __pyx_lineno, __pyx_filename);
-          if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_9, &__pyx_t_4) < 0) __PYX_ERR(0, 97, __pyx_L19_except_error)
-          __Pyx_GOTREF(__pyx_t_5);
-          __Pyx_GOTREF(__pyx_t_9);
-          __Pyx_GOTREF(__pyx_t_4);
-          __pyx_t_8 = PyTuple_Pack(3, __pyx_t_5, __pyx_t_9, __pyx_t_4); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 97, __pyx_L19_except_error)
+          if (__Pyx_GetException(&__pyx_t_8, &__pyx_t_4, &__pyx_t_9) < 0) __PYX_ERR(0, 99, __pyx_L19_except_error)
           __Pyx_GOTREF(__pyx_t_8);
-          __pyx_t_17 = __Pyx_PyObject_Call(__pyx_t_12, __pyx_t_8, NULL);
+          __Pyx_GOTREF(__pyx_t_4);
+          __Pyx_GOTREF(__pyx_t_9);
+          __pyx_t_5 = PyTuple_Pack(3, __pyx_t_8, __pyx_t_4, __pyx_t_9); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 99, __pyx_L19_except_error)
+          __Pyx_GOTREF(__pyx_t_5);
+          __pyx_t_17 = __Pyx_PyObject_Call(__pyx_t_12, __pyx_t_5, NULL);
           __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-          __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-          if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 97, __pyx_L19_except_error)
+          __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+          if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 99, __pyx_L19_except_error)
           __Pyx_GOTREF(__pyx_t_17);
           __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_17);
           __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
-          if (__pyx_t_2 < 0) __PYX_ERR(0, 97, __pyx_L19_except_error)
+          if (__pyx_t_2 < 0) __PYX_ERR(0, 99, __pyx_L19_except_error)
           __pyx_t_1 = ((!(__pyx_t_2 != 0)) != 0);
           if (__pyx_t_1) {
-            __Pyx_GIVEREF(__pyx_t_5);
-            __Pyx_GIVEREF(__pyx_t_9);
-            __Pyx_XGIVEREF(__pyx_t_4);
-            __Pyx_ErrRestoreWithState(__pyx_t_5, __pyx_t_9, __pyx_t_4);
-            __pyx_t_5 = 0; __pyx_t_9 = 0; __pyx_t_4 = 0; 
-            __PYX_ERR(0, 97, __pyx_L19_except_error)
+            __Pyx_GIVEREF(__pyx_t_8);
+            __Pyx_GIVEREF(__pyx_t_4);
+            __Pyx_XGIVEREF(__pyx_t_9);
+            __Pyx_ErrRestoreWithState(__pyx_t_8, __pyx_t_4, __pyx_t_9);
+            __pyx_t_8 = 0; __pyx_t_4 = 0; __pyx_t_9 = 0; 
+            __PYX_ERR(0, 99, __pyx_L19_except_error)
           }
-          __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-          __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
+          __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+          __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
           goto __pyx_L18_exception_handled;
         }
         __pyx_L19_except_error:;
         __Pyx_XGIVEREF(__pyx_t_13);
         __Pyx_XGIVEREF(__pyx_t_14);
         __Pyx_XGIVEREF(__pyx_t_15);
         __Pyx_ExceptionReset(__pyx_t_13, __pyx_t_14, __pyx_t_15);
@@ -6639,15 +6713,15 @@
       }
     }
     /*finally:*/ {
       /*normal exit:*/{
         if (__pyx_t_12) {
           __pyx_t_15 = __Pyx_PyObject_Call(__pyx_t_12, __pyx_tuple__7, NULL);
           __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-          if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 97, __pyx_L1_error)
+          if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 99, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_15);
           __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
         }
         goto __pyx_L16;
       }
       __pyx_L16:;
     }
@@ -6657,15 +6731,15 @@
     goto __pyx_L1_error;
     __pyx_L32:;
   }
 
   /* "edsnlp/matchers/phrase.pyx":73
  *             Span.set_extension("normalized_variant", getter=get_normalized_variant)
  * 
- *     def build_patterns(self, nlp: Language, terms: Patterns):             # <<<<<<<<<<<<<<
+ *     def build_patterns(self, nlp: Language, terms: Patterns, progress: bool = False):             # <<<<<<<<<<<<<<
  *         """
  *         Build patterns and adds them for matching.
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
@@ -6690,15 +6764,15 @@
   __Pyx_DECREF(((PyObject *)__pyx_cur_scope));
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "edsnlp/matchers/phrase.pyx":112
+/* "edsnlp/matchers/phrase.pyx":114
  *                 self.add(key, patterns, attr)
  * 
  *     cdef void find_matches(self, Doc doc, int start_idx, int end_idx, vector[SpanC] *matches) nogil:             # <<<<<<<<<<<<<<
  *         cdef:
  *             MapStruct * current_node = self.c_map
  */
 
@@ -6714,504 +6788,480 @@
   void *__pyx_v_result;
   __pyx_t_5spacy_8typedefs_attr_t __pyx_v_token;
   __pyx_t_5spacy_8typedefs_attr_t __pyx_v_inner_token;
   __Pyx_TraceDeclarations
   struct __pyx_t_7preshed_4maps_MapStruct *__pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
+  int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_TraceCall("find_matches", __pyx_f[0], 112, 1, __PYX_ERR(0, 112, __pyx_L1_error));
+  __Pyx_TraceCall("find_matches", __pyx_f[0], 114, 1, __PYX_ERR(0, 114, __pyx_L1_error));
 
-  /* "edsnlp/matchers/phrase.pyx":114
+  /* "edsnlp/matchers/phrase.pyx":116
  *     cdef void find_matches(self, Doc doc, int start_idx, int end_idx, vector[SpanC] *matches) nogil:
  *         cdef:
  *             MapStruct * current_node = self.c_map             # <<<<<<<<<<<<<<
  *             int start = 0
  *             int idx = start_idx
  */
   __pyx_t_1 = __pyx_v_self->__pyx_base.c_map;
   __pyx_v_current_node = __pyx_t_1;
 
-  /* "edsnlp/matchers/phrase.pyx":115
+  /* "edsnlp/matchers/phrase.pyx":117
  *         cdef:
  *             MapStruct * current_node = self.c_map
  *             int start = 0             # <<<<<<<<<<<<<<
  *             int idx = start_idx
  *             int idy = start_idx
  */
   __pyx_v_start = 0;
 
-  /* "edsnlp/matchers/phrase.pyx":116
+  /* "edsnlp/matchers/phrase.pyx":118
  *             MapStruct * current_node = self.c_map
  *             int start = 0
  *             int idx = start_idx             # <<<<<<<<<<<<<<
  *             int idy = start_idx
  *             key_t key
  */
   __pyx_v_idx = __pyx_v_start_idx;
 
-  /* "edsnlp/matchers/phrase.pyx":117
+  /* "edsnlp/matchers/phrase.pyx":119
  *             int start = 0
  *             int idx = start_idx
  *             int idy = start_idx             # <<<<<<<<<<<<<<
  *             key_t key
  *             void * value
  */
   __pyx_v_idy = __pyx_v_start_idx;
 
-  /* "edsnlp/matchers/phrase.pyx":120
+  /* "edsnlp/matchers/phrase.pyx":122
  *             key_t key
  *             void * value
  *             int i = 0             # <<<<<<<<<<<<<<
  *             SpanC ms
  *             void * result
  */
   __pyx_v_i = 0;
 
-  /* "edsnlp/matchers/phrase.pyx":123
+  /* "edsnlp/matchers/phrase.pyx":125
  *             SpanC ms
  *             void * result
  *         while idx < end_idx:             # <<<<<<<<<<<<<<
- *             start = idx
- *             token = Token.get_struct_attr(&doc.c[idx], self.attr)
+ *             while (
+ *                 (0 < self.space_hash == doc.c[idx].tag)
  */
   while (1) {
     __pyx_t_2 = ((__pyx_v_idx < __pyx_v_end_idx) != 0);
     if (!__pyx_t_2) break;
 
-    /* "edsnlp/matchers/phrase.pyx":124
+    /* "edsnlp/matchers/phrase.pyx":126
  *             void * result
  *         while idx < end_idx:
- *             start = idx             # <<<<<<<<<<<<<<
- *             token = Token.get_struct_attr(&doc.c[idx], self.attr)
- *             # look for sequences from this position
+ *             while (             # <<<<<<<<<<<<<<
+ *                 (0 < self.space_hash == doc.c[idx].tag)
+ *                 or (0 < self.excluded_hash == doc.c[idx].tag)
  */
-    __pyx_v_start = __pyx_v_idx;
+    while (1) {
 
-    /* "edsnlp/matchers/phrase.pyx":125
+      /* "edsnlp/matchers/phrase.pyx":127
  *         while idx < end_idx:
- *             start = idx
- *             token = Token.get_struct_attr(&doc.c[idx], self.attr)             # <<<<<<<<<<<<<<
- *             # look for sequences from this position
- *             if 0 < self.space_hash == doc.c[idx].tag:
+ *             while (
+ *                 (0 < self.space_hash == doc.c[idx].tag)             # <<<<<<<<<<<<<<
+ *                 or (0 < self.excluded_hash == doc.c[idx].tag)
+ *             ):
  */
-    __pyx_v_token = __pyx_f_5spacy_6tokens_5token_5Token_get_struct_attr((&(__pyx_v_doc->c[__pyx_v_idx])), __pyx_v_self->__pyx_base.attr);
+      __pyx_t_3 = (0 < __pyx_v_self->space_hash);
+      if (__pyx_t_3) {
+        __pyx_t_3 = (__pyx_v_self->space_hash == (__pyx_v_doc->c[__pyx_v_idx]).tag);
+      }
+      __pyx_t_4 = (__pyx_t_3 != 0);
+      if (!__pyx_t_4) {
+      } else {
+        __pyx_t_2 = __pyx_t_4;
+        goto __pyx_L7_bool_binop_done;
+      }
 
-    /* "edsnlp/matchers/phrase.pyx":127
- *             token = Token.get_struct_attr(&doc.c[idx], self.attr)
- *             # look for sequences from this position
- *             if 0 < self.space_hash == doc.c[idx].tag:             # <<<<<<<<<<<<<<
+      /* "edsnlp/matchers/phrase.pyx":128
+ *             while (
+ *                 (0 < self.space_hash == doc.c[idx].tag)
+ *                 or (0 < self.excluded_hash == doc.c[idx].tag)             # <<<<<<<<<<<<<<
+ *             ):
  *                 idx += 1
- *                 continue
  */
-    __pyx_t_2 = (0 < __pyx_v_self->space_hash);
-    if (__pyx_t_2) {
-      __pyx_t_2 = (__pyx_v_self->space_hash == (__pyx_v_doc->c[__pyx_v_idx]).tag);
-    }
-    __pyx_t_3 = (__pyx_t_2 != 0);
-    if (__pyx_t_3) {
+      __pyx_t_4 = (0 < __pyx_v_self->excluded_hash);
+      if (__pyx_t_4) {
+        __pyx_t_4 = (__pyx_v_self->excluded_hash == (__pyx_v_doc->c[__pyx_v_idx]).tag);
+      }
+      __pyx_t_3 = (__pyx_t_4 != 0);
+      __pyx_t_2 = __pyx_t_3;
+      __pyx_L7_bool_binop_done:;
+      if (!__pyx_t_2) break;
 
-      /* "edsnlp/matchers/phrase.pyx":128
- *             # look for sequences from this position
- *             if 0 < self.space_hash == doc.c[idx].tag:
+      /* "edsnlp/matchers/phrase.pyx":130
+ *                 or (0 < self.excluded_hash == doc.c[idx].tag)
+ *             ):
  *                 idx += 1             # <<<<<<<<<<<<<<
- *                 continue
- *             if 0 < self.excluded_hash == doc.c[idx].tag:
+ *                 if idx >= end_idx:
+ *                     return
  */
       __pyx_v_idx = (__pyx_v_idx + 1);
 
-      /* "edsnlp/matchers/phrase.pyx":129
- *             if 0 < self.space_hash == doc.c[idx].tag:
- *                 idx += 1
- *                 continue             # <<<<<<<<<<<<<<
- *             if 0 < self.excluded_hash == doc.c[idx].tag:
+      /* "edsnlp/matchers/phrase.pyx":131
+ *             ):
  *                 idx += 1
+ *                 if idx >= end_idx:             # <<<<<<<<<<<<<<
+ *                     return
+ *             start = idx
  */
-      goto __pyx_L3_continue;
+      __pyx_t_2 = ((__pyx_v_idx >= __pyx_v_end_idx) != 0);
+      if (__pyx_t_2) {
 
-      /* "edsnlp/matchers/phrase.pyx":127
- *             token = Token.get_struct_attr(&doc.c[idx], self.attr)
- *             # look for sequences from this position
- *             if 0 < self.space_hash == doc.c[idx].tag:             # <<<<<<<<<<<<<<
+        /* "edsnlp/matchers/phrase.pyx":132
  *                 idx += 1
- *                 continue
+ *                 if idx >= end_idx:
+ *                     return             # <<<<<<<<<<<<<<
+ *             start = idx
+ *             # look for sequences from this position
  */
-    }
+        goto __pyx_L0;
 
-    /* "edsnlp/matchers/phrase.pyx":130
- *                 idx += 1
- *                 continue
- *             if 0 < self.excluded_hash == doc.c[idx].tag:             # <<<<<<<<<<<<<<
+        /* "edsnlp/matchers/phrase.pyx":131
+ *             ):
  *                 idx += 1
- *                 continue
+ *                 if idx >= end_idx:             # <<<<<<<<<<<<<<
+ *                     return
+ *             start = idx
  */
-    __pyx_t_3 = (0 < __pyx_v_self->excluded_hash);
-    if (__pyx_t_3) {
-      __pyx_t_3 = (__pyx_v_self->excluded_hash == (__pyx_v_doc->c[__pyx_v_idx]).tag);
+      }
     }
-    __pyx_t_2 = (__pyx_t_3 != 0);
-    if (__pyx_t_2) {
 
-      /* "edsnlp/matchers/phrase.pyx":131
- *                 continue
- *             if 0 < self.excluded_hash == doc.c[idx].tag:
- *                 idx += 1             # <<<<<<<<<<<<<<
- *                 continue
- *             result = map_get(current_node, token)
+    /* "edsnlp/matchers/phrase.pyx":133
+ *                 if idx >= end_idx:
+ *                     return
+ *             start = idx             # <<<<<<<<<<<<<<
+ *             # look for sequences from this position
+ *             token = Token.get_struct_attr(&doc.c[idx], self.attr)
  */
-      __pyx_v_idx = (__pyx_v_idx + 1);
+    __pyx_v_start = __pyx_v_idx;
 
-      /* "edsnlp/matchers/phrase.pyx":132
- *             if 0 < self.excluded_hash == doc.c[idx].tag:
- *                 idx += 1
- *                 continue             # <<<<<<<<<<<<<<
+    /* "edsnlp/matchers/phrase.pyx":135
+ *             start = idx
+ *             # look for sequences from this position
+ *             token = Token.get_struct_attr(&doc.c[idx], self.attr)             # <<<<<<<<<<<<<<
  *             result = map_get(current_node, token)
  *             if result:
  */
-      goto __pyx_L3_continue;
-
-      /* "edsnlp/matchers/phrase.pyx":130
- *                 idx += 1
- *                 continue
- *             if 0 < self.excluded_hash == doc.c[idx].tag:             # <<<<<<<<<<<<<<
- *                 idx += 1
- *                 continue
- */
-    }
+    __pyx_v_token = __pyx_f_5spacy_6tokens_5token_5Token_get_struct_attr((&(__pyx_v_doc->c[__pyx_v_idx])), __pyx_v_self->__pyx_base.attr);
 
-    /* "edsnlp/matchers/phrase.pyx":133
- *                 idx += 1
- *                 continue
+    /* "edsnlp/matchers/phrase.pyx":136
+ *             # look for sequences from this position
+ *             token = Token.get_struct_attr(&doc.c[idx], self.attr)
  *             result = map_get(current_node, token)             # <<<<<<<<<<<<<<
  *             if result:
  *                 current_node = <MapStruct *> result
  */
     __pyx_v_result = __pyx_f_7preshed_4maps_map_get(__pyx_v_current_node, __pyx_v_token);
 
-    /* "edsnlp/matchers/phrase.pyx":134
- *                 continue
+    /* "edsnlp/matchers/phrase.pyx":137
+ *             token = Token.get_struct_attr(&doc.c[idx], self.attr)
  *             result = map_get(current_node, token)
  *             if result:             # <<<<<<<<<<<<<<
  *                 current_node = <MapStruct *> result
  *                 idy = idx + 1
  */
     __pyx_t_2 = (__pyx_v_result != 0);
     if (__pyx_t_2) {
 
-      /* "edsnlp/matchers/phrase.pyx":135
+      /* "edsnlp/matchers/phrase.pyx":138
  *             result = map_get(current_node, token)
  *             if result:
  *                 current_node = <MapStruct *> result             # <<<<<<<<<<<<<<
  *                 idy = idx + 1
  *                 while idy < end_idx:
  */
       __pyx_v_current_node = ((struct __pyx_t_7preshed_4maps_MapStruct *)__pyx_v_result);
 
-      /* "edsnlp/matchers/phrase.pyx":136
+      /* "edsnlp/matchers/phrase.pyx":139
  *             if result:
  *                 current_node = <MapStruct *> result
  *                 idy = idx + 1             # <<<<<<<<<<<<<<
  *                 while idy < end_idx:
- *                     if 0 < self.space_hash == doc.c[idy].tag:
+ *                     result = map_get(current_node, self._terminal_hash)
  */
       __pyx_v_idy = (__pyx_v_idx + 1);
 
-      /* "edsnlp/matchers/phrase.pyx":137
+      /* "edsnlp/matchers/phrase.pyx":140
  *                 current_node = <MapStruct *> result
  *                 idy = idx + 1
  *                 while idy < end_idx:             # <<<<<<<<<<<<<<
- *                     if 0 < self.space_hash == doc.c[idy].tag:
- *                         idy += 1
+ *                     result = map_get(current_node, self._terminal_hash)
+ *                     if result:
  */
       while (1) {
         __pyx_t_2 = ((__pyx_v_idy < __pyx_v_end_idx) != 0);
         if (!__pyx_t_2) break;
 
-        /* "edsnlp/matchers/phrase.pyx":138
- *                 idy = idx + 1
- *                 while idy < end_idx:
- *                     if 0 < self.space_hash == doc.c[idy].tag:             # <<<<<<<<<<<<<<
- *                         idy += 1
- *                         continue
- */
-        __pyx_t_2 = (0 < __pyx_v_self->space_hash);
-        if (__pyx_t_2) {
-          __pyx_t_2 = (__pyx_v_self->space_hash == (__pyx_v_doc->c[__pyx_v_idy]).tag);
-        }
-        __pyx_t_3 = (__pyx_t_2 != 0);
-        if (__pyx_t_3) {
-
-          /* "edsnlp/matchers/phrase.pyx":139
- *                 while idy < end_idx:
- *                     if 0 < self.space_hash == doc.c[idy].tag:
- *                         idy += 1             # <<<<<<<<<<<<<<
- *                         continue
- *                     if 0 < self.excluded_hash == doc.c[idy].tag:
- */
-          __pyx_v_idy = (__pyx_v_idy + 1);
-
-          /* "edsnlp/matchers/phrase.pyx":140
- *                     if 0 < self.space_hash == doc.c[idy].tag:
- *                         idy += 1
- *                         continue             # <<<<<<<<<<<<<<
- *                     if 0 < self.excluded_hash == doc.c[idy].tag:
- *                         idy += 1
- */
-          goto __pyx_L8_continue;
-
-          /* "edsnlp/matchers/phrase.pyx":138
+        /* "edsnlp/matchers/phrase.pyx":141
  *                 idy = idx + 1
  *                 while idy < end_idx:
- *                     if 0 < self.space_hash == doc.c[idy].tag:             # <<<<<<<<<<<<<<
- *                         idy += 1
- *                         continue
- */
-        }
-
-        /* "edsnlp/matchers/phrase.pyx":141
- *                         idy += 1
- *                         continue
- *                     if 0 < self.excluded_hash == doc.c[idy].tag:             # <<<<<<<<<<<<<<
- *                         idy += 1
- *                         continue
- */
-        __pyx_t_3 = (0 < __pyx_v_self->excluded_hash);
-        if (__pyx_t_3) {
-          __pyx_t_3 = (__pyx_v_self->excluded_hash == (__pyx_v_doc->c[__pyx_v_idy]).tag);
-        }
-        __pyx_t_2 = (__pyx_t_3 != 0);
-        if (__pyx_t_2) {
-
-          /* "edsnlp/matchers/phrase.pyx":142
- *                         continue
- *                     if 0 < self.excluded_hash == doc.c[idy].tag:
- *                         idy += 1             # <<<<<<<<<<<<<<
- *                         continue
- *                     result = map_get(current_node, self._terminal_hash)
- */
-          __pyx_v_idy = (__pyx_v_idy + 1);
-
-          /* "edsnlp/matchers/phrase.pyx":143
- *                     if 0 < self.excluded_hash == doc.c[idy].tag:
- *                         idy += 1
- *                         continue             # <<<<<<<<<<<<<<
- *                     result = map_get(current_node, self._terminal_hash)
- *                     if result:
- */
-          goto __pyx_L8_continue;
-
-          /* "edsnlp/matchers/phrase.pyx":141
- *                         idy += 1
- *                         continue
- *                     if 0 < self.excluded_hash == doc.c[idy].tag:             # <<<<<<<<<<<<<<
- *                         idy += 1
- *                         continue
- */
-        }
-
-        /* "edsnlp/matchers/phrase.pyx":144
- *                         idy += 1
- *                         continue
  *                     result = map_get(current_node, self._terminal_hash)             # <<<<<<<<<<<<<<
  *                     if result:
  *                         i = 0
  */
         __pyx_v_result = __pyx_f_7preshed_4maps_map_get(__pyx_v_current_node, __pyx_v_self->__pyx_base._terminal_hash);
 
-        /* "edsnlp/matchers/phrase.pyx":145
- *                         continue
+        /* "edsnlp/matchers/phrase.pyx":142
+ *                 while idy < end_idx:
  *                     result = map_get(current_node, self._terminal_hash)
  *                     if result:             # <<<<<<<<<<<<<<
  *                         i = 0
  *                         while map_iter(<MapStruct *> result, &i, &key, &value):
  */
         __pyx_t_2 = (__pyx_v_result != 0);
         if (__pyx_t_2) {
 
-          /* "edsnlp/matchers/phrase.pyx":146
+          /* "edsnlp/matchers/phrase.pyx":143
  *                     result = map_get(current_node, self._terminal_hash)
  *                     if result:
  *                         i = 0             # <<<<<<<<<<<<<<
  *                         while map_iter(<MapStruct *> result, &i, &key, &value):
  *                             ms = make_spanstruct(key, start, idy)
  */
           __pyx_v_i = 0;
 
-          /* "edsnlp/matchers/phrase.pyx":147
+          /* "edsnlp/matchers/phrase.pyx":144
  *                     if result:
  *                         i = 0
  *                         while map_iter(<MapStruct *> result, &i, &key, &value):             # <<<<<<<<<<<<<<
  *                             ms = make_spanstruct(key, start, idy)
  *                             matches.push_back(ms)
  */
           while (1) {
             __pyx_t_2 = (__pyx_f_7preshed_4maps_map_iter(((struct __pyx_t_7preshed_4maps_MapStruct *)__pyx_v_result), (&__pyx_v_i), (&__pyx_v_key), (&__pyx_v_value)) != 0);
             if (!__pyx_t_2) break;
 
-            /* "edsnlp/matchers/phrase.pyx":148
+            /* "edsnlp/matchers/phrase.pyx":145
  *                         i = 0
  *                         while map_iter(<MapStruct *> result, &i, &key, &value):
  *                             ms = make_spanstruct(key, start, idy)             # <<<<<<<<<<<<<<
  *                             matches.push_back(ms)
- *                     inner_token = Token.get_struct_attr(&doc.c[idy], self.attr)
+ * 
  */
             __pyx_v_ms = __pyx_f_6edsnlp_8matchers_6phrase_make_spanstruct(__pyx_v_key, __pyx_v_start, __pyx_v_idy);
 
-            /* "edsnlp/matchers/phrase.pyx":149
+            /* "edsnlp/matchers/phrase.pyx":146
  *                         while map_iter(<MapStruct *> result, &i, &key, &value):
  *                             ms = make_spanstruct(key, start, idy)
  *                             matches.push_back(ms)             # <<<<<<<<<<<<<<
- *                     inner_token = Token.get_struct_attr(&doc.c[idy], self.attr)
- *                     result = map_get(current_node, inner_token)
+ * 
+ *                     while idy < end_idx and (
  */
             try {
               __pyx_v_matches->push_back(__pyx_v_ms);
             } catch(...) {
               #ifdef WITH_THREAD
               PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
               #endif
               __Pyx_CppExn2PyErr();
               #ifdef WITH_THREAD
               __Pyx_PyGILState_Release(__pyx_gilstate_save);
               #endif
-              __PYX_ERR(0, 149, __pyx_L1_error)
+              __PYX_ERR(0, 146, __pyx_L1_error)
             }
           }
 
-          /* "edsnlp/matchers/phrase.pyx":145
- *                         continue
+          /* "edsnlp/matchers/phrase.pyx":142
+ *                 while idy < end_idx:
  *                     result = map_get(current_node, self._terminal_hash)
  *                     if result:             # <<<<<<<<<<<<<<
  *                         i = 0
  *                         while map_iter(<MapStruct *> result, &i, &key, &value):
  */
         }
 
-        /* "edsnlp/matchers/phrase.pyx":150
- *                             ms = make_spanstruct(key, start, idy)
+        /* "edsnlp/matchers/phrase.pyx":148
  *                             matches.push_back(ms)
+ * 
+ *                     while idy < end_idx and (             # <<<<<<<<<<<<<<
+ *                         (0 < self.space_hash == doc.c[idy].tag)
+ *                         or (0 < self.excluded_hash == doc.c[idy].tag)
+ */
+        while (1) {
+          __pyx_t_3 = ((__pyx_v_idy < __pyx_v_end_idx) != 0);
+          if (__pyx_t_3) {
+          } else {
+            __pyx_t_2 = __pyx_t_3;
+            goto __pyx_L18_bool_binop_done;
+          }
+
+          /* "edsnlp/matchers/phrase.pyx":149
+ * 
+ *                     while idy < end_idx and (
+ *                         (0 < self.space_hash == doc.c[idy].tag)             # <<<<<<<<<<<<<<
+ *                         or (0 < self.excluded_hash == doc.c[idy].tag)
+ *                     ):
+ */
+          __pyx_t_3 = (0 < __pyx_v_self->space_hash);
+          if (__pyx_t_3) {
+            __pyx_t_3 = (__pyx_v_self->space_hash == (__pyx_v_doc->c[__pyx_v_idy]).tag);
+          }
+          __pyx_t_4 = (__pyx_t_3 != 0);
+          if (!__pyx_t_4) {
+          } else {
+            __pyx_t_2 = __pyx_t_4;
+            goto __pyx_L18_bool_binop_done;
+          }
+
+          /* "edsnlp/matchers/phrase.pyx":150
+ *                     while idy < end_idx and (
+ *                         (0 < self.space_hash == doc.c[idy].tag)
+ *                         or (0 < self.excluded_hash == doc.c[idy].tag)             # <<<<<<<<<<<<<<
+ *                     ):
+ *                         idy += 1
+ */
+          __pyx_t_4 = (0 < __pyx_v_self->excluded_hash);
+          if (__pyx_t_4) {
+            __pyx_t_4 = (__pyx_v_self->excluded_hash == (__pyx_v_doc->c[__pyx_v_idy]).tag);
+          }
+          __pyx_t_3 = (__pyx_t_4 != 0);
+          __pyx_t_2 = __pyx_t_3;
+          __pyx_L18_bool_binop_done:;
+          if (!__pyx_t_2) break;
+
+          /* "edsnlp/matchers/phrase.pyx":152
+ *                         or (0 < self.excluded_hash == doc.c[idy].tag)
+ *                     ):
+ *                         idy += 1             # <<<<<<<<<<<<<<
+ *                     inner_token = Token.get_struct_attr(&doc.c[idy], self.attr)
+ *                     result = map_get(current_node, inner_token)
+ */
+          __pyx_v_idy = (__pyx_v_idy + 1);
+        }
+
+        /* "edsnlp/matchers/phrase.pyx":153
+ *                     ):
+ *                         idy += 1
  *                     inner_token = Token.get_struct_attr(&doc.c[idy], self.attr)             # <<<<<<<<<<<<<<
  *                     result = map_get(current_node, inner_token)
  *                     if result:
  */
         __pyx_v_inner_token = __pyx_f_5spacy_6tokens_5token_5Token_get_struct_attr((&(__pyx_v_doc->c[__pyx_v_idy])), __pyx_v_self->__pyx_base.attr);
 
-        /* "edsnlp/matchers/phrase.pyx":151
- *                             matches.push_back(ms)
+        /* "edsnlp/matchers/phrase.pyx":154
+ *                         idy += 1
  *                     inner_token = Token.get_struct_attr(&doc.c[idy], self.attr)
  *                     result = map_get(current_node, inner_token)             # <<<<<<<<<<<<<<
  *                     if result:
  *                         current_node = <MapStruct *> result
  */
         __pyx_v_result = __pyx_f_7preshed_4maps_map_get(__pyx_v_current_node, __pyx_v_inner_token);
 
-        /* "edsnlp/matchers/phrase.pyx":152
+        /* "edsnlp/matchers/phrase.pyx":155
  *                     inner_token = Token.get_struct_attr(&doc.c[idy], self.attr)
  *                     result = map_get(current_node, inner_token)
  *                     if result:             # <<<<<<<<<<<<<<
  *                         current_node = <MapStruct *> result
  *                         idy += 1
  */
         __pyx_t_2 = (__pyx_v_result != 0);
         if (__pyx_t_2) {
 
-          /* "edsnlp/matchers/phrase.pyx":153
+          /* "edsnlp/matchers/phrase.pyx":156
  *                     result = map_get(current_node, inner_token)
  *                     if result:
  *                         current_node = <MapStruct *> result             # <<<<<<<<<<<<<<
  *                         idy += 1
  *                     else:
  */
           __pyx_v_current_node = ((struct __pyx_t_7preshed_4maps_MapStruct *)__pyx_v_result);
 
-          /* "edsnlp/matchers/phrase.pyx":154
+          /* "edsnlp/matchers/phrase.pyx":157
  *                     if result:
  *                         current_node = <MapStruct *> result
  *                         idy += 1             # <<<<<<<<<<<<<<
  *                     else:
  *                         break
  */
           __pyx_v_idy = (__pyx_v_idy + 1);
 
-          /* "edsnlp/matchers/phrase.pyx":152
+          /* "edsnlp/matchers/phrase.pyx":155
  *                     inner_token = Token.get_struct_attr(&doc.c[idy], self.attr)
  *                     result = map_get(current_node, inner_token)
  *                     if result:             # <<<<<<<<<<<<<<
  *                         current_node = <MapStruct *> result
  *                         idy += 1
  */
-          goto __pyx_L15;
+          goto __pyx_L21;
         }
 
-        /* "edsnlp/matchers/phrase.pyx":156
+        /* "edsnlp/matchers/phrase.pyx":159
  *                         idy += 1
  *                     else:
  *                         break             # <<<<<<<<<<<<<<
  *                 else:
  *                     # end of doc reached
  */
         /*else*/ {
-          goto __pyx_L9_break;
+          goto __pyx_L12_break;
         }
-        __pyx_L15:;
-        __pyx_L8_continue:;
+        __pyx_L21:;
       }
 
-      /* "edsnlp/matchers/phrase.pyx":159
+      /* "edsnlp/matchers/phrase.pyx":162
  *                 else:
  *                     # end of doc reached
  *                     result = map_get(current_node, self._terminal_hash)             # <<<<<<<<<<<<<<
  *                     if result:
  *                         i = 0
  */
       /*else*/ {
         __pyx_v_result = __pyx_f_7preshed_4maps_map_get(__pyx_v_current_node, __pyx_v_self->__pyx_base._terminal_hash);
 
-        /* "edsnlp/matchers/phrase.pyx":160
+        /* "edsnlp/matchers/phrase.pyx":163
  *                     # end of doc reached
  *                     result = map_get(current_node, self._terminal_hash)
  *                     if result:             # <<<<<<<<<<<<<<
  *                         i = 0
  *                         while map_iter(<MapStruct *> result, &i, &key, &value):
  */
         __pyx_t_2 = (__pyx_v_result != 0);
         if (__pyx_t_2) {
 
-          /* "edsnlp/matchers/phrase.pyx":161
+          /* "edsnlp/matchers/phrase.pyx":164
  *                     result = map_get(current_node, self._terminal_hash)
  *                     if result:
  *                         i = 0             # <<<<<<<<<<<<<<
  *                         while map_iter(<MapStruct *> result, &i, &key, &value):
  *                             ms = make_spanstruct(key, start, idy)
  */
           __pyx_v_i = 0;
 
-          /* "edsnlp/matchers/phrase.pyx":162
+          /* "edsnlp/matchers/phrase.pyx":165
  *                     if result:
  *                         i = 0
  *                         while map_iter(<MapStruct *> result, &i, &key, &value):             # <<<<<<<<<<<<<<
  *                             ms = make_spanstruct(key, start, idy)
  *                             matches.push_back(ms)
  */
           while (1) {
             __pyx_t_2 = (__pyx_f_7preshed_4maps_map_iter(((struct __pyx_t_7preshed_4maps_MapStruct *)__pyx_v_result), (&__pyx_v_i), (&__pyx_v_key), (&__pyx_v_value)) != 0);
             if (!__pyx_t_2) break;
 
-            /* "edsnlp/matchers/phrase.pyx":163
+            /* "edsnlp/matchers/phrase.pyx":166
  *                         i = 0
  *                         while map_iter(<MapStruct *> result, &i, &key, &value):
  *                             ms = make_spanstruct(key, start, idy)             # <<<<<<<<<<<<<<
  *                             matches.push_back(ms)
  *             current_node = self.c_map
  */
             __pyx_v_ms = __pyx_f_6edsnlp_8matchers_6phrase_make_spanstruct(__pyx_v_key, __pyx_v_start, __pyx_v_idy);
 
-            /* "edsnlp/matchers/phrase.pyx":164
+            /* "edsnlp/matchers/phrase.pyx":167
  *                         while map_iter(<MapStruct *> result, &i, &key, &value):
  *                             ms = make_spanstruct(key, start, idy)
  *                             matches.push_back(ms)             # <<<<<<<<<<<<<<
  *             current_node = self.c_map
  *             idx += 1
  */
             try {
@@ -7220,60 +7270,59 @@
               #ifdef WITH_THREAD
               PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
               #endif
               __Pyx_CppExn2PyErr();
               #ifdef WITH_THREAD
               __Pyx_PyGILState_Release(__pyx_gilstate_save);
               #endif
-              __PYX_ERR(0, 164, __pyx_L1_error)
+              __PYX_ERR(0, 167, __pyx_L1_error)
             }
           }
 
-          /* "edsnlp/matchers/phrase.pyx":160
+          /* "edsnlp/matchers/phrase.pyx":163
  *                     # end of doc reached
  *                     result = map_get(current_node, self._terminal_hash)
  *                     if result:             # <<<<<<<<<<<<<<
  *                         i = 0
  *                         while map_iter(<MapStruct *> result, &i, &key, &value):
  */
         }
       }
-      __pyx_L9_break:;
+      __pyx_L12_break:;
 
-      /* "edsnlp/matchers/phrase.pyx":134
- *                 continue
+      /* "edsnlp/matchers/phrase.pyx":137
+ *             token = Token.get_struct_attr(&doc.c[idx], self.attr)
  *             result = map_get(current_node, token)
  *             if result:             # <<<<<<<<<<<<<<
  *                 current_node = <MapStruct *> result
  *                 idy = idx + 1
  */
     }
 
-    /* "edsnlp/matchers/phrase.pyx":165
+    /* "edsnlp/matchers/phrase.pyx":168
  *                             ms = make_spanstruct(key, start, idy)
  *                             matches.push_back(ms)
  *             current_node = self.c_map             # <<<<<<<<<<<<<<
  *             idx += 1
  * 
  */
     __pyx_t_1 = __pyx_v_self->__pyx_base.c_map;
     __pyx_v_current_node = __pyx_t_1;
 
-    /* "edsnlp/matchers/phrase.pyx":166
+    /* "edsnlp/matchers/phrase.pyx":169
  *                             matches.push_back(ms)
  *             current_node = self.c_map
  *             idx += 1             # <<<<<<<<<<<<<<
  * 
  * cdef SpanC make_spanstruct(attr_t label, int start, int end) nogil:
  */
     __pyx_v_idx = (__pyx_v_idx + 1);
-    __pyx_L3_continue:;
   }
 
-  /* "edsnlp/matchers/phrase.pyx":112
+  /* "edsnlp/matchers/phrase.pyx":114
  *                 self.add(key, patterns, attr)
  * 
  *     cdef void find_matches(self, Doc doc, int start_idx, int end_idx, vector[SpanC] *matches) nogil:             # <<<<<<<<<<<<<<
  *         cdef:
  *             MapStruct * current_node = self.c_map
  */
 
@@ -7400,66 +7449,66 @@
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "edsnlp/matchers/phrase.pyx":168
+/* "edsnlp/matchers/phrase.pyx":171
  *             idx += 1
  * 
  * cdef SpanC make_spanstruct(attr_t label, int start, int end) nogil:             # <<<<<<<<<<<<<<
  *     cdef SpanC spanc
  *     spanc.label = label
  */
 
 static struct __pyx_t_5spacy_7structs_SpanC __pyx_f_6edsnlp_8matchers_6phrase_make_spanstruct(__pyx_t_5spacy_8typedefs_attr_t __pyx_v_label, int __pyx_v_start, int __pyx_v_end) {
   struct __pyx_t_5spacy_7structs_SpanC __pyx_v_spanc;
   struct __pyx_t_5spacy_7structs_SpanC __pyx_r;
   __Pyx_TraceDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_TraceCall("make_spanstruct", __pyx_f[0], 168, 1, __PYX_ERR(0, 168, __pyx_L1_error));
+  __Pyx_TraceCall("make_spanstruct", __pyx_f[0], 171, 1, __PYX_ERR(0, 171, __pyx_L1_error));
 
-  /* "edsnlp/matchers/phrase.pyx":170
+  /* "edsnlp/matchers/phrase.pyx":173
  * cdef SpanC make_spanstruct(attr_t label, int start, int end) nogil:
  *     cdef SpanC spanc
  *     spanc.label = label             # <<<<<<<<<<<<<<
  *     spanc.start = start
  *     spanc.end = end
  */
   __pyx_v_spanc.label = __pyx_v_label;
 
-  /* "edsnlp/matchers/phrase.pyx":171
+  /* "edsnlp/matchers/phrase.pyx":174
  *     cdef SpanC spanc
  *     spanc.label = label
  *     spanc.start = start             # <<<<<<<<<<<<<<
  *     spanc.end = end
  *     return spanc
  */
   __pyx_v_spanc.start = __pyx_v_start;
 
-  /* "edsnlp/matchers/phrase.pyx":172
+  /* "edsnlp/matchers/phrase.pyx":175
  *     spanc.label = label
  *     spanc.start = start
  *     spanc.end = end             # <<<<<<<<<<<<<<
  *     return spanc
  */
   __pyx_v_spanc.end = __pyx_v_end;
 
-  /* "edsnlp/matchers/phrase.pyx":173
+  /* "edsnlp/matchers/phrase.pyx":176
  *     spanc.start = start
  *     spanc.end = end
  *     return spanc             # <<<<<<<<<<<<<<
  */
   __pyx_r = __pyx_v_spanc;
   goto __pyx_L0;
 
-  /* "edsnlp/matchers/phrase.pyx":168
+  /* "edsnlp/matchers/phrase.pyx":171
  *             idx += 1
  * 
  * cdef SpanC make_spanstruct(attr_t label, int start, int end) nogil:             # <<<<<<<<<<<<<<
  *     cdef SpanC spanc
  *     spanc.label = label
  */
 
@@ -7468,15 +7517,15 @@
   __Pyx_WriteUnraisable("edsnlp.matchers.phrase.make_spanstruct", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 1);
   __Pyx_pretend_to_initialize(&__pyx_r);
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":735
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -7487,29 +7536,29 @@
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
   __Pyx_TraceCall("PyArray_MultiIterNew1", __pyx_f[2], 735, 0, __PYX_ERR(2, 735, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":736
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":736
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 736, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -7521,15 +7570,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":738
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -7540,29 +7589,29 @@
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
   __Pyx_TraceCall("PyArray_MultiIterNew2", __pyx_f[2], 738, 0, __PYX_ERR(2, 738, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":739
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":739
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 739, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -7574,15 +7623,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":741
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -7593,29 +7642,29 @@
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
   __Pyx_TraceCall("PyArray_MultiIterNew3", __pyx_f[2], 741, 0, __PYX_ERR(2, 741, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":742
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":742
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 742, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -7627,15 +7676,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":744
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -7646,29 +7695,29 @@
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
   __Pyx_TraceCall("PyArray_MultiIterNew4", __pyx_f[2], 744, 0, __PYX_ERR(2, 744, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":745
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":745
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 745, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -7680,15 +7729,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":747
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -7699,29 +7748,29 @@
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
   __Pyx_TraceCall("PyArray_MultiIterNew5", __pyx_f[2], 747, 0, __PYX_ERR(2, 747, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":748
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":748
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 748, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -7733,15 +7782,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":750
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
@@ -7752,60 +7801,60 @@
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
   __Pyx_TraceCall("PyDataType_SHAPE", __pyx_f[2], 750, 0, __PYX_ERR(2, 750, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":751
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":752
+    /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":752
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":754
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":754
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
@@ -7816,15 +7865,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":929
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -7833,33 +7882,33 @@
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
   __Pyx_TraceCall("set_array_base", __pyx_f[2], 929, 0, __PYX_ERR(2, 929, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":930
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":931
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":931
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -7868,15 +7917,15 @@
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":933
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
@@ -7888,66 +7937,66 @@
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_array_base", 0);
   __Pyx_TraceCall("get_array_base", __pyx_f[2], 933, 0, __PYX_ERR(2, 933, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":934
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":935
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":936
+    /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":936
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":937
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":937
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
@@ -7958,15 +8007,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_TraceReturn(__pyx_r, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":941
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -7984,15 +8033,15 @@
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
   __Pyx_TraceCall("import_array", __pyx_f[2], 941, 0, __PYX_ERR(2, 941, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":942
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -8000,53 +8049,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":943
+      /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":943
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 943, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":944
+    /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 944, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":945
+      /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 945, __pyx_L5_except_error)
@@ -8054,30 +8103,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 945, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":942
+    /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -8093,15 +8142,15 @@
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":947
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -8119,15 +8168,15 @@
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
   __Pyx_TraceCall("import_umath", __pyx_f[2], 947, 0, __PYX_ERR(2, 947, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":948
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -8135,53 +8184,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":949
+      /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":949
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 949, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":950
+    /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 950, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":951
+      /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 951, __pyx_L5_except_error)
@@ -8189,30 +8238,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 951, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":948
+    /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -8228,15 +8277,15 @@
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":953
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -8254,15 +8303,15 @@
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
   __Pyx_TraceCall("import_ufunc", __pyx_f[2], 953, 0, __PYX_ERR(2, 953, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":954
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -8270,53 +8319,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":955
+      /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":955
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 955, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":956
+    /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":956
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 956, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":957
+      /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":957
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 957, __pyx_L5_except_error)
@@ -8324,30 +8373,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 957, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":954
+    /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -8363,15 +8412,15 @@
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":967
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":967
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
@@ -8381,25 +8430,25 @@
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
   __Pyx_TraceCall("is_timedelta64_object", __pyx_f[2], 967, 0, __PYX_ERR(2, 967, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":979
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":979
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":967
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":967
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
@@ -8409,15 +8458,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":982
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":982
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
@@ -8427,25 +8476,25 @@
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
   __Pyx_TraceCall("is_datetime64_object", __pyx_f[2], 982, 0, __PYX_ERR(2, 982, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":994
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":994
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":982
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":982
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
@@ -8455,15 +8504,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 0);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":997
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":997
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
@@ -8471,25 +8520,25 @@
   npy_datetime __pyx_r;
   __Pyx_TraceDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_TraceCall("get_datetime64_value", __pyx_f[2], 997, 1, __PYX_ERR(2, 997, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":1004
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":1004
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":997
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":997
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
@@ -8498,15 +8547,15 @@
   __Pyx_WriteUnraisable("numpy.get_datetime64_value", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 1);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":1007
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":1007
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
@@ -8514,25 +8563,25 @@
   npy_timedelta __pyx_r;
   __Pyx_TraceDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_TraceCall("get_timedelta64_value", __pyx_f[2], 1007, 1, __PYX_ERR(2, 1007, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":1011
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":1011
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":1007
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":1007
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
@@ -8541,15 +8590,15 @@
   __Pyx_WriteUnraisable("numpy.get_timedelta64_value", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 1);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_TraceReturn(Py_None, 1);
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":1014
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":1014
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -8557,23 +8606,23 @@
   NPY_DATETIMEUNIT __pyx_r;
   __Pyx_TraceDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_TraceCall("get_datetime64_unit", __pyx_f[2], 1014, 1, __PYX_ERR(2, 1014, __pyx_L1_error));
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":1018
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":1018
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":1014
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":1014
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -10928,15 +10977,15 @@
   /* "View.MemoryView":141
  *         if not isinstance(format, bytes):
  *             format = format.encode('ASCII')
  *         self._format = format  # keep a reference to the byte string             # <<<<<<<<<<<<<<
  *         self.format = self._format
  * 
  */
-  if (!(likely(PyBytes_CheckExact(__pyx_v_format))||((__pyx_v_format) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_v_format)->tp_name), 0))) __PYX_ERR(1, 141, __pyx_L1_error)
+  if (!(likely(PyBytes_CheckExact(__pyx_v_format))||((__pyx_v_format) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_v_format)->tp_name), 0))) __PYX_ERR(1, 141, __pyx_L1_error)
   __pyx_t_3 = __pyx_v_format;
   __Pyx_INCREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_3);
   __Pyx_GOTREF(__pyx_v_self->_format);
   __Pyx_DECREF(__pyx_v_self->_format);
   __pyx_v_self->_format = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
@@ -12978,15 +13027,15 @@
   __Pyx_TraceCall("__setstate_cython__", __pyx_f[1], 16, 0, __PYX_ERR(1, 16, __pyx_L1_error));
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle_Enum, (type(self), 0xb068931, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_Enum__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
-  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
+  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
   __pyx_t_1 = __pyx_unpickle_Enum__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_Enum, (type(self), 0xb068931, state)
@@ -15330,15 +15379,15 @@
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_6, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 512, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(1, 512, __pyx_L1_error)
+    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(1, 512, __pyx_L1_error)
     __pyx_v_bytesvalue = ((PyObject*)__pyx_t_4);
     __pyx_t_4 = 0;
 
     /* "View.MemoryView":511
  *         cdef Py_ssize_t i
  * 
  *         if isinstance(value, tuple):             # <<<<<<<<<<<<<<
@@ -15403,15 +15452,15 @@
       PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_v_value);
       __pyx_t_1 = 0;
       __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_8, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 514, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     }
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(1, 514, __pyx_L1_error)
+    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(1, 514, __pyx_L1_error)
     __pyx_v_bytesvalue = ((PyObject*)__pyx_t_4);
     __pyx_t_4 = 0;
   }
   __pyx_L3:;
 
   /* "View.MemoryView":516
  *             bytesvalue = struct.pack(self.view.format, value)
@@ -23883,15 +23932,15 @@
     /* "(tree fragment)":9
  *     __pyx_result = Enum.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_Enum__set_state(<Enum> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_Enum__set_state(Enum __pyx_result, tuple __pyx_state):
  */
-    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
+    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
     __pyx_t_4 = __pyx_unpickle_Enum__set_state(((struct __pyx_MemviewEnum_obj *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))" % __pyx_checksum)
  *     __pyx_result = Enum.__new__(__pyx_type)
@@ -25296,14 +25345,15 @@
   {&__pyx_kp_u_numpy_core_umath_failed_to_impor, __pyx_k_numpy_core_umath_failed_to_impor, sizeof(__pyx_k_numpy_core_umath_failed_to_impor), 0, 1, 0, 0},
   {&__pyx_n_s_obj, __pyx_k_obj, sizeof(__pyx_k_obj), 0, 0, 1, 1},
   {&__pyx_n_s_pack, __pyx_k_pack, sizeof(__pyx_k_pack), 0, 0, 1, 1},
   {&__pyx_n_u_patterns, __pyx_k_patterns, sizeof(__pyx_k_patterns), 0, 1, 0, 1},
   {&__pyx_n_s_pickle, __pyx_k_pickle, sizeof(__pyx_k_pickle), 0, 0, 1, 1},
   {&__pyx_n_s_pipe, __pyx_k_pipe, sizeof(__pyx_k_pipe), 0, 0, 1, 1},
   {&__pyx_n_s_pipeline, __pyx_k_pipeline, sizeof(__pyx_k_pipeline), 0, 0, 1, 1},
+  {&__pyx_n_s_progress, __pyx_k_progress, sizeof(__pyx_k_progress), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_PickleError, __pyx_k_pyx_PickleError, sizeof(__pyx_k_pyx_PickleError), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_checksum, __pyx_k_pyx_checksum, sizeof(__pyx_k_pyx_checksum), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_getbuffer, __pyx_k_pyx_getbuffer, sizeof(__pyx_k_pyx_getbuffer), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_result, __pyx_k_pyx_result, sizeof(__pyx_k_pyx_result), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_state, __pyx_k_pyx_state, sizeof(__pyx_k_pyx_state), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_type, __pyx_k_pyx_type, sizeof(__pyx_k_pyx_type), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_unpickle_Enum, __pyx_k_pyx_unpickle_Enum, sizeof(__pyx_k_pyx_unpickle_Enum), 0, 0, 1, 1},
@@ -25377,28 +25427,28 @@
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
   /* "edsnlp/matchers/phrase.pyx":71
  *     def set_extensions():
  *         if not Span.has_extension("normalized_variant"):
  *             Span.set_extension("normalized_variant", getter=get_normalized_variant)             # <<<<<<<<<<<<<<
  * 
- *     def build_patterns(self, nlp: Language, terms: Patterns):
+ *     def build_patterns(self, nlp: Language, terms: Patterns, progress: bool = False):
  */
   __pyx_tuple__6 = PyTuple_Pack(1, __pyx_n_u_normalized_variant); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 71, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
 
-  /* "edsnlp/matchers/phrase.pyx":97
+  /* "edsnlp/matchers/phrase.pyx":99
  *             )
  *         ]
  *         with nlp.select_pipes(enable=token_pipelines):             # <<<<<<<<<<<<<<
- *             for key, expressions in tqdm(
+ *             for key, expressions in (tqdm(
  *                 terms.items(),
  */
-  __pyx_tuple__7 = PyTuple_Pack(3, Py_None, Py_None, Py_None); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 97, __pyx_L1_error)
+  __pyx_tuple__7 = PyTuple_Pack(3, Py_None, Py_None, Py_None); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 99, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("self.c_map cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
@@ -25413,26 +25463,26 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("self.c_map cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_s_self_c_map_cannot_be_converted_t); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":945
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 945, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":951
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(2, 951, __pyx_L1_error)
@@ -25724,15 +25774,15 @@
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
   __pyx_umethod_PyUnicode_Type_rstrip.type = (PyObject*)&PyUnicode_Type;
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_112105877 = PyInt_FromLong(112105877L); if (unlikely(!__pyx_int_112105877)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_136983863 = PyInt_FromLong(136983863L); if (unlikely(!__pyx_int_136983863)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_184977713 = PyInt_FromLong(184977713L); if (unlikely(!__pyx_int_184977713)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_neg_1 = PyInt_FromLong(-1); if (unlikely(!__pyx_int_neg_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
@@ -25783,15 +25833,16 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
   __pyx_t_1 = PyImport_ImportModule("spacy.matcher.phrasematcher"); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5spacy_7matcher_13phrasematcher_PhraseMatcher = __Pyx_ImportType(__pyx_t_1, "spacy.matcher.phrasematcher", "PhraseMatcher", sizeof(struct __pyx_obj_5spacy_7matcher_13phrasematcher_PhraseMatcher), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5spacy_7matcher_13phrasematcher_PhraseMatcher = __Pyx_ImportType(__pyx_t_1, "spacy.matcher.phrasematcher", "PhraseMatcher", sizeof(struct __pyx_obj_5spacy_7matcher_13phrasematcher_PhraseMatcher), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_5spacy_7matcher_13phrasematcher_PhraseMatcher),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5spacy_7matcher_13phrasematcher_PhraseMatcher) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_vtabptr_5spacy_7matcher_13phrasematcher_PhraseMatcher = (struct __pyx_vtabstruct_5spacy_7matcher_13phrasematcher_PhraseMatcher*)__Pyx_GetVtable(__pyx_ptype_5spacy_7matcher_13phrasematcher_PhraseMatcher->tp_dict); if (unlikely(!__pyx_vtabptr_5spacy_7matcher_13phrasematcher_PhraseMatcher)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_vtabptr_6edsnlp_8matchers_6phrase_EDSPhraseMatcher = &__pyx_vtable_6edsnlp_8matchers_6phrase_EDSPhraseMatcher;
   __pyx_vtable_6edsnlp_8matchers_6phrase_EDSPhraseMatcher.__pyx_base = *__pyx_vtabptr_5spacy_7matcher_13phrasematcher_PhraseMatcher;
   __pyx_vtable_6edsnlp_8matchers_6phrase_EDSPhraseMatcher.__pyx_base.find_matches = (void (*)(struct __pyx_obj_5spacy_7matcher_13phrasematcher_PhraseMatcher *, struct __pyx_obj_5spacy_6tokens_3doc_Doc *, int, int, std::vector<struct __pyx_t_5spacy_7structs_SpanC>  *))__pyx_f_6edsnlp_8matchers_6phrase_16EDSPhraseMatcher_find_matches;
   __pyx_type_6edsnlp_8matchers_6phrase_EDSPhraseMatcher.tp_base = __pyx_ptype_5spacy_7matcher_13phrasematcher_PhraseMatcher;
   if (PyType_Ready(&__pyx_type_6edsnlp_8matchers_6phrase_EDSPhraseMatcher) < 0) __PYX_ERR(0, 26, __pyx_L1_error)
@@ -25819,15 +25870,15 @@
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_6edsnlp_8matchers_6phrase___pyx_scope_struct__build_patterns.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6edsnlp_8matchers_6phrase___pyx_scope_struct__build_patterns.tp_dictoffset && __pyx_type_6edsnlp_8matchers_6phrase___pyx_scope_struct__build_patterns.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_6edsnlp_8matchers_6phrase___pyx_scope_struct__build_patterns.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_6edsnlp_8matchers_6phrase___pyx_scope_struct__build_patterns = &__pyx_type_6edsnlp_8matchers_6phrase___pyx_scope_struct__build_patterns;
-  if (PyType_Ready(&__pyx_type_6edsnlp_8matchers_6phrase___pyx_scope_struct_1_genexpr) < 0) __PYX_ERR(0, 93, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_6edsnlp_8matchers_6phrase___pyx_scope_struct_1_genexpr) < 0) __PYX_ERR(0, 95, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_6edsnlp_8matchers_6phrase___pyx_scope_struct_1_genexpr.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6edsnlp_8matchers_6phrase___pyx_scope_struct_1_genexpr.tp_dictoffset && __pyx_type_6edsnlp_8matchers_6phrase___pyx_scope_struct_1_genexpr.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_6edsnlp_8matchers_6phrase___pyx_scope_struct_1_genexpr.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_6edsnlp_8matchers_6phrase___pyx_scope_struct_1_genexpr = &__pyx_type_6edsnlp_8matchers_6phrase___pyx_scope_struct_1_genexpr;
@@ -25897,118 +25948,146 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule("cymem.cymem"); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5cymem_5cymem_PyMalloc = __Pyx_ImportType(__pyx_t_1, "cymem.cymem", "PyMalloc", sizeof(struct __pyx_obj_5cymem_5cymem_PyMalloc), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5cymem_5cymem_PyMalloc = __Pyx_ImportType(__pyx_t_1, "cymem.cymem", "PyMalloc", sizeof(struct __pyx_obj_5cymem_5cymem_PyMalloc), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_5cymem_5cymem_PyMalloc),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5cymem_5cymem_PyMalloc) __PYX_ERR(6, 4, __pyx_L1_error)
   __pyx_vtabptr_5cymem_5cymem_PyMalloc = (struct __pyx_vtabstruct_5cymem_5cymem_PyMalloc*)__Pyx_GetVtable(__pyx_ptype_5cymem_5cymem_PyMalloc->tp_dict); if (unlikely(!__pyx_vtabptr_5cymem_5cymem_PyMalloc)) __PYX_ERR(6, 4, __pyx_L1_error)
-  __pyx_ptype_5cymem_5cymem_PyFree = __Pyx_ImportType(__pyx_t_1, "cymem.cymem", "PyFree", sizeof(struct __pyx_obj_5cymem_5cymem_PyFree), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5cymem_5cymem_PyFree = __Pyx_ImportType(__pyx_t_1, "cymem.cymem", "PyFree", sizeof(struct __pyx_obj_5cymem_5cymem_PyFree), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_5cymem_5cymem_PyFree),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5cymem_5cymem_PyFree) __PYX_ERR(6, 10, __pyx_L1_error)
   __pyx_vtabptr_5cymem_5cymem_PyFree = (struct __pyx_vtabstruct_5cymem_5cymem_PyFree*)__Pyx_GetVtable(__pyx_ptype_5cymem_5cymem_PyFree->tp_dict); if (unlikely(!__pyx_vtabptr_5cymem_5cymem_PyFree)) __PYX_ERR(6, 10, __pyx_L1_error)
-  __pyx_ptype_5cymem_5cymem_Pool = __Pyx_ImportType(__pyx_t_1, "cymem.cymem", "Pool", sizeof(struct __pyx_obj_5cymem_5cymem_Pool), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5cymem_5cymem_Pool = __Pyx_ImportType(__pyx_t_1, "cymem.cymem", "Pool", sizeof(struct __pyx_obj_5cymem_5cymem_Pool), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_5cymem_5cymem_Pool),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5cymem_5cymem_Pool) __PYX_ERR(6, 16, __pyx_L1_error)
   __pyx_vtabptr_5cymem_5cymem_Pool = (struct __pyx_vtabstruct_5cymem_5cymem_Pool*)__Pyx_GetVtable(__pyx_ptype_5cymem_5cymem_Pool->tp_dict); if (unlikely(!__pyx_vtabptr_5cymem_5cymem_Pool)) __PYX_ERR(6, 16, __pyx_L1_error)
-  __pyx_ptype_5cymem_5cymem_Address = __Pyx_ImportType(__pyx_t_1, "cymem.cymem", "Address", sizeof(struct __pyx_obj_5cymem_5cymem_Address), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5cymem_5cymem_Address = __Pyx_ImportType(__pyx_t_1, "cymem.cymem", "Address", sizeof(struct __pyx_obj_5cymem_5cymem_Address), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_5cymem_5cymem_Address),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5cymem_5cymem_Address) __PYX_ERR(6, 28, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("preshed.maps"); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 45, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7preshed_4maps_PreshMap = __Pyx_ImportType(__pyx_t_1, "preshed.maps", "PreshMap", sizeof(struct __pyx_obj_7preshed_4maps_PreshMap), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_7preshed_4maps_PreshMap = __Pyx_ImportType(__pyx_t_1, "preshed.maps", "PreshMap", sizeof(struct __pyx_obj_7preshed_4maps_PreshMap), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_7preshed_4maps_PreshMap),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7preshed_4maps_PreshMap) __PYX_ERR(7, 45, __pyx_L1_error)
   __pyx_vtabptr_7preshed_4maps_PreshMap = (struct __pyx_vtabstruct_7preshed_4maps_PreshMap*)__Pyx_GetVtable(__pyx_ptype_7preshed_4maps_PreshMap->tp_dict); if (unlikely(!__pyx_vtabptr_7preshed_4maps_PreshMap)) __PYX_ERR(7, 45, __pyx_L1_error)
-  __pyx_ptype_7preshed_4maps_PreshMapArray = __Pyx_ImportType(__pyx_t_1, "preshed.maps", "PreshMapArray", sizeof(struct __pyx_obj_7preshed_4maps_PreshMapArray), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_7preshed_4maps_PreshMapArray = __Pyx_ImportType(__pyx_t_1, "preshed.maps", "PreshMapArray", sizeof(struct __pyx_obj_7preshed_4maps_PreshMapArray), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_7preshed_4maps_PreshMapArray),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7preshed_4maps_PreshMapArray) __PYX_ERR(7, 53, __pyx_L1_error)
   __pyx_vtabptr_7preshed_4maps_PreshMapArray = (struct __pyx_vtabstruct_7preshed_4maps_PreshMapArray*)__Pyx_GetVtable(__pyx_ptype_7preshed_4maps_PreshMapArray->tp_dict); if (unlikely(!__pyx_vtabptr_7preshed_4maps_PreshMapArray)) __PYX_ERR(7, 53, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(8, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(8, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 200, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT(PyArray_Descr),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 200, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 223, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayMultiIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 227, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 239, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 771, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 773, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 775, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 777, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 779, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 781, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 783, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 785, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 787, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 789, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT(PyUFuncObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 827, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("spacy.strings"); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 22, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5spacy_7strings_StringStore = __Pyx_ImportType(__pyx_t_1, "spacy.strings", "StringStore", sizeof(struct __pyx_obj_5spacy_7strings_StringStore), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5spacy_7strings_StringStore = __Pyx_ImportType(__pyx_t_1, "spacy.strings", "StringStore", sizeof(struct __pyx_obj_5spacy_7strings_StringStore), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_5spacy_7strings_StringStore),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5spacy_7strings_StringStore) __PYX_ERR(9, 22, __pyx_L1_error)
   __pyx_vtabptr_5spacy_7strings_StringStore = (struct __pyx_vtabstruct_5spacy_7strings_StringStore*)__Pyx_GetVtable(__pyx_ptype_5spacy_7strings_StringStore->tp_dict); if (unlikely(!__pyx_vtabptr_5spacy_7strings_StringStore)) __PYX_ERR(9, 22, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("spacy.morphology"); if (unlikely(!__pyx_t_1)) __PYX_ERR(10, 11, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5spacy_10morphology_Morphology = __Pyx_ImportType(__pyx_t_1, "spacy.morphology", "Morphology", sizeof(struct __pyx_obj_5spacy_10morphology_Morphology), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5spacy_10morphology_Morphology = __Pyx_ImportType(__pyx_t_1, "spacy.morphology", "Morphology", sizeof(struct __pyx_obj_5spacy_10morphology_Morphology), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_5spacy_10morphology_Morphology),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5spacy_10morphology_Morphology) __PYX_ERR(10, 11, __pyx_L1_error)
   __pyx_vtabptr_5spacy_10morphology_Morphology = (struct __pyx_vtabstruct_5spacy_10morphology_Morphology*)__Pyx_GetVtable(__pyx_ptype_5spacy_10morphology_Morphology->tp_dict); if (unlikely(!__pyx_vtabptr_5spacy_10morphology_Morphology)) __PYX_ERR(10, 11, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("spacy.vocab"); if (unlikely(!__pyx_t_1)) __PYX_ERR(11, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5spacy_5vocab_Vocab = __Pyx_ImportType(__pyx_t_1, "spacy.vocab", "Vocab", sizeof(struct __pyx_obj_5spacy_5vocab_Vocab), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5spacy_5vocab_Vocab = __Pyx_ImportType(__pyx_t_1, "spacy.vocab", "Vocab", sizeof(struct __pyx_obj_5spacy_5vocab_Vocab), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_5spacy_5vocab_Vocab),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5spacy_5vocab_Vocab) __PYX_ERR(11, 26, __pyx_L1_error)
   __pyx_vtabptr_5spacy_5vocab_Vocab = (struct __pyx_vtabstruct_5spacy_5vocab_Vocab*)__Pyx_GetVtable(__pyx_ptype_5spacy_5vocab_Vocab->tp_dict); if (unlikely(!__pyx_vtabptr_5spacy_5vocab_Vocab)) __PYX_ERR(11, 26, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("spacy.tokens.doc"); if (unlikely(!__pyx_t_1)) __PYX_ERR(12, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5spacy_6tokens_3doc_Doc = __Pyx_ImportType(__pyx_t_1, "spacy.tokens.doc", "Doc", sizeof(struct __pyx_obj_5spacy_6tokens_3doc_Doc), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5spacy_6tokens_3doc_Doc = __Pyx_ImportType(__pyx_t_1, "spacy.tokens.doc", "Doc", sizeof(struct __pyx_obj_5spacy_6tokens_3doc_Doc), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_5spacy_6tokens_3doc_Doc),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5spacy_6tokens_3doc_Doc) __PYX_ERR(12, 37, __pyx_L1_error)
   __pyx_vtabptr_5spacy_6tokens_3doc_Doc = (struct __pyx_vtabstruct_5spacy_6tokens_3doc_Doc*)__Pyx_GetVtable(__pyx_ptype_5spacy_6tokens_3doc_Doc->tp_dict); if (unlikely(!__pyx_vtabptr_5spacy_6tokens_3doc_Doc)) __PYX_ERR(12, 37, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("spacy.tokens.span"); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5spacy_6tokens_4span_Span = __Pyx_ImportType(__pyx_t_1, "spacy.tokens.span", "Span", sizeof(struct __pyx_obj_5spacy_6tokens_4span_Span), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5spacy_6tokens_4span_Span = __Pyx_ImportType(__pyx_t_1, "spacy.tokens.span", "Span", sizeof(struct __pyx_obj_5spacy_6tokens_4span_Span), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_5spacy_6tokens_4span_Span),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5spacy_6tokens_4span_Span) __PYX_ERR(3, 8, __pyx_L1_error)
   __pyx_vtabptr_5spacy_6tokens_4span_Span = (struct __pyx_vtabstruct_5spacy_6tokens_4span_Span*)__Pyx_GetVtable(__pyx_ptype_5spacy_6tokens_4span_Span->tp_dict); if (unlikely(!__pyx_vtabptr_5spacy_6tokens_4span_Span)) __PYX_ERR(3, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("spacy.lexeme"); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5spacy_6lexeme_Lexeme = __Pyx_ImportType(__pyx_t_1, "spacy.lexeme", "Lexeme", sizeof(struct __pyx_obj_5spacy_6lexeme_Lexeme), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5spacy_6lexeme_Lexeme = __Pyx_ImportType(__pyx_t_1, "spacy.lexeme", "Lexeme", sizeof(struct __pyx_obj_5spacy_6lexeme_Lexeme), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_5spacy_6lexeme_Lexeme),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5spacy_6lexeme_Lexeme) __PYX_ERR(4, 15, __pyx_L1_error)
   __pyx_vtabptr_5spacy_6lexeme_Lexeme = (struct __pyx_vtabstruct_5spacy_6lexeme_Lexeme*)__Pyx_GetVtable(__pyx_ptype_5spacy_6lexeme_Lexeme->tp_dict); if (unlikely(!__pyx_vtabptr_5spacy_6lexeme_Lexeme)) __PYX_ERR(4, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("spacy.tokens.token"); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 14, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5spacy_6tokens_5token_Token = __Pyx_ImportType(__pyx_t_1, "spacy.tokens.token", "Token", sizeof(struct __pyx_obj_5spacy_6tokens_5token_Token), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5spacy_6tokens_5token_Token = __Pyx_ImportType(__pyx_t_1, "spacy.tokens.token", "Token", sizeof(struct __pyx_obj_5spacy_6tokens_5token_Token), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_5spacy_6tokens_5token_Token),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5spacy_6tokens_5token_Token) __PYX_ERR(5, 14, __pyx_L1_error)
   __pyx_vtabptr_5spacy_6tokens_5token_Token = (struct __pyx_vtabstruct_5spacy_6tokens_5token_Token*)__Pyx_GetVtable(__pyx_ptype_5spacy_6tokens_5token_Token->tp_dict); if (unlikely(!__pyx_vtabptr_5spacy_6tokens_5token_Token)) __PYX_ERR(5, 14, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
@@ -26238,15 +26317,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_edsnlp__matchers__phrase) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name_2, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -26785,19 +26864,19 @@
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_CallUnboundCMethod1(__Pyx_CachedCFunction* cfunc, PyObject* self, PyObject* arg) {
     if (likely(cfunc->func)) {
         int flag = cfunc->flag;
         if (flag == METH_O) {
             return (*(cfunc->func))(self, arg);
         } else if (PY_VERSION_HEX >= 0x030600B1 && flag == METH_FASTCALL) {
-            if (PY_VERSION_HEX >= 0x030700A0) {
+            #if PY_VERSION_HEX >= 0x030700A0
                 return (*(__Pyx_PyCFunctionFast)(void*)(PyCFunction)cfunc->func)(self, &arg, 1);
-            } else {
+            #else
                 return (*(__Pyx_PyCFunctionFastWithKeywords)(void*)(PyCFunction)cfunc->func)(self, &arg, 1, NULL);
-            }
+            #endif
         } else if (PY_VERSION_HEX >= 0x030700A0 && flag == (METH_FASTCALL | METH_KEYWORDS)) {
             return (*(__Pyx_PyCFunctionFastWithKeywords)(void*)(PyCFunction)cfunc->func)(self, &arg, 1, NULL);
         }
     }
     return __Pyx__CallUnboundCMethod1(cfunc, self, arg);
 }
 #endif
@@ -27285,15 +27364,15 @@
 #endif
     return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
 }
 
 /* ObjectGetItem */
 #if CYTHON_USE_TYPE_SLOTS
 static PyObject *__Pyx_PyObject_GetIndex(PyObject *obj, PyObject* index) {
-    PyObject *runerr;
+    PyObject *runerr = NULL;
     Py_ssize_t key_value;
     PySequenceMethods *m = Py_TYPE(obj)->tp_as_sequence;
     if (unlikely(!(m && m->sq_item))) {
         PyErr_Format(PyExc_TypeError, "'%.200s' object is not subscriptable", Py_TYPE(obj)->tp_name);
         return NULL;
     }
     key_value = __Pyx_PyIndex_AsSsize_t(index);
@@ -27339,15 +27418,15 @@
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
 #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(func)) {
         return __Pyx_PyFunction_FastCall(func, NULL, 0);
     }
 #endif
-#ifdef __Pyx_CyFunction_USED
+#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
     if (likely(PyCFunction_Check(func) || __Pyx_CyFunction_Check(func)))
 #else
     if (likely(PyCFunction_Check(func)))
 #endif
     {
         if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
             return __Pyx_PyObject_CallMethO(func, NULL);
@@ -27670,18 +27749,16 @@
 
 /* UnpackItemEndCheck */
 static int __Pyx_IternextUnpackEndCheck(PyObject *retval, Py_ssize_t expected) {
     if (unlikely(retval)) {
         Py_DECREF(retval);
         __Pyx_RaiseTooManyValuesError(expected);
         return -1;
-    } else {
-        return __Pyx_IterFinish();
     }
-    return 0;
+    return __Pyx_IterFinish();
 }
 
 /* GetTopmostException */
 #if CYTHON_USE_EXC_INFO_STACK
 static _PyErr_StackItem *
 __Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
 {
@@ -27817,17 +27894,15 @@
     PyObject *old_exc, *old_val, *old_tb;
     PyObject *ctx;
     __Pyx_PyThreadState_declare
 #ifdef WITH_THREAD
     PyGILState_STATE state;
     if (nogil)
         state = PyGILState_Ensure();
-#ifdef _MSC_VER
-    else state = (PyGILState_STATE)-1;
-#endif
+    else state = (PyGILState_STATE)0;
 #endif
     __Pyx_PyThreadState_assign
     __Pyx_ErrFetch(&old_exc, &old_val, &old_tb);
     if (full_traceback) {
         Py_XINCREF(old_exc);
         Py_XINCREF(old_val);
         Py_XINCREF(old_tb);
@@ -27985,28 +28060,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -28576,44 +28651,62 @@
 }
 #endif
 
 /* TypeImport */
 #ifndef __PYX_HAVE_RT_ImportType
 #define __PYX_HAVE_RT_ImportType
 static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
     if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
@@ -28819,15 +28912,15 @@
         result = __Pyx_GetGlobalNameAfterAttributeLookup(name);
     }
     return result;
 }
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
@@ -29197,15 +29290,15 @@
                         z = __Pyx_c_prod_float(a, a);
                         return __Pyx_c_prod_float(z, z);
                 }
             }
             if (a.imag == 0) {
                 if (a.real == 0) {
                     return a;
-                } else if (b.imag == 0) {
+                } else if ((b.imag == 0) && (a.real >= 0)) {
                     z.real = powf(a.real, b.real);
                     z.imag = 0;
                     return z;
                 } else if (a.real > 0) {
                     r = a.real;
                     theta = 0;
                 } else {
@@ -29351,15 +29444,15 @@
                         z = __Pyx_c_prod_double(a, a);
                         return __Pyx_c_prod_double(z, z);
                 }
             }
             if (a.imag == 0) {
                 if (a.real == 0) {
                     return a;
-                } else if (b.imag == 0) {
+                } else if ((b.imag == 0) && (a.real >= 0)) {
                     z.real = pow(a.real, b.real);
                     z.imag = 0;
                     return z;
                 } else if (a.real > 0) {
                     r = a.real;
                     theta = 0;
                 } else {
```

### Comparing `edsnlp-0.7.4/edsnlp/matchers/regex.py` & `edsnlp-0.8.0/edsnlp/matchers/regex.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+import re
 from bisect import bisect_left
 from functools import lru_cache
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from loguru import logger
 from spacy.tokens import Doc, Span, Token
 
-from edsnlp.utils.regex import compile_regex, re
+from edsnlp.utils.regex import compile_regex
 
 from .utils import Patterns, alignment, get_text, offset
 
 
 @lru_cache(32)
 def get_first_included(doclike: Union[Doc, Span]) -> Token:
     for token in doclike:
@@ -76,14 +77,15 @@
     doclike: Union[Doc, Span],
     start_char: int,
     end_char: int,
     key: str,
     attr: str,
     alignment_mode: str,
     ignore_excluded: bool,
+    ignore_space_tokens: bool,
 ) -> Span:
     """
     spaCy only allows strict alignment mode for char_span on Spans.
     This method circumvents this.
     Parameters
     ----------
     doclike : Union[Doc, Span]
@@ -94,39 +96,43 @@
         Character index of the end, within the Doc-like object.
     key : str
         The key used to match.
     alignment_mode : str
         The alignment mode.
     ignore_excluded : bool
         Whether to skip excluded tokens.
+    ignore_space_tokens : bool
+        Whether to skip space tokens.
+
     Returns
     -------
     span:
         A span matched on the Doc-like object.
     """
 
     doc = doclike if isinstance(doclike, Doc) else doclike.doc
 
     # Handle the simple case immediately
-    if attr in {"TEXT", "LOWER"} and not ignore_excluded:
+    if attr in {"TEXT", "LOWER"} and not ignore_excluded and not ignore_space_tokens:
         off = doclike[0].idx
         return doc.char_span(
             start_char + off,
             end_char + off,
             label=key,
             alignment_mode=alignment_mode,
         )
 
     # If doclike is a Span, we need to get the clean
     # index of the first included token
-    if ignore_excluded:
+    if ignore_excluded or ignore_space_tokens:
         original, clean = alignment(
             doc=doc,
             attr=attr,
             ignore_excluded=ignore_excluded,
+            ignore_space_tokens=ignore_space_tokens,
         )
 
         first_included = get_first_included(doclike)
         i = bisect_left(original, first_included.idx)
         first = clean[i]
 
     else:
@@ -135,25 +141,27 @@
     start_char = (
         first
         + start_char
         + offset(
             doc,
             attr=attr,
             ignore_excluded=ignore_excluded,
+            ignore_space_tokens=ignore_space_tokens,
             index=first + start_char,
         )
     )
 
     end_char = (
         first
         + end_char
         + offset(
             doc,
             attr=attr,
             ignore_excluded=ignore_excluded,
+            ignore_space_tokens=ignore_space_tokens,
             index=first + end_char,
         )
     )
 
     span = doc.char_span(
         start_char,
         end_char,
@@ -181,37 +189,44 @@
         Default attribute to match on, by default "TEXT".
         Can be overiden in the `add` method.
     flags : Union[re.RegexFlag, int]
         Additional flags provided to the `re` module.
         Can be overiden in the `add` method.
     ignore_excluded : bool
         Whether to skip exclusions
+    ignore_space_tokens: bool
+        Whether to skip space tokens during matching.
+
+        You won't be able to match on newlines if this is enabled and
+        the "spaces"/"newline" option of `eds.normalizer` is enabled (by default).
     span_from_group : bool
         If set to `False`, will create spans basede on the regex's full match.
         If set to `True`, will use the first matching capturing group as a span
         (and fall back to using the full match if no capturing group is matching)
     """
 
     def __init__(
         self,
         alignment_mode: str = "expand",
         attr: str = "TEXT",
         ignore_excluded: bool = False,
+        ignore_space_tokens: bool = False,
         flags: Union[re.RegexFlag, int] = 0,  # No additional flags
         span_from_group: bool = False,
     ):
         self.alignment_mode = alignment_mode
         self.regex = []
 
         self.default_attr = attr
 
         self.flags = flags
         self.span_from_group = span_from_group
 
         self.ignore_excluded = ignore_excluded
+        self.ignore_space_tokens = ignore_space_tokens
 
         self.set_extensions()
 
     @classmethod
     def set_extensions(cls):
         if not Span.has_extension("normalized_variant"):
             Span.set_extension("normalized_variant", getter=get_normalized_variant)
@@ -253,50 +268,69 @@
 
     def add(
         self,
         key: str,
         patterns: List[str],
         attr: Optional[str] = None,
         ignore_excluded: Optional[bool] = None,
+        ignore_space_tokens: Optional[bool] = None,
         alignment_mode: Optional[str] = None,
         flags: Optional[re.RegexFlag] = None,
     ):
         """
         Add a pattern to the registry.
 
         Parameters
         ----------
         key : str
             Key of the new/updated pattern.
         patterns : List[str]
             List of patterns to add.
-        attr : str, optional
+        attr : Optional[str]
             Attribute to use for matching.
-            By default uses the `default_attr` attribute
-        ignore_excluded : bool, optional
+            By default, uses the `default_attr` attribute
+        ignore_excluded : Optional[bool]
             Whether to skip excluded tokens during matching.
-        alignment_mode : str, optional
+        ignore_space_tokens: Optional[bool]
+            Whether to skip space tokens during matching.
+
+            You won't be able to match on newlines if this is enabled and
+            the "spaces"/"newline" option of `eds.normalizer` is enabled (by default).
+
+        alignment_mode : Optional[str]
             Overwrite alignment mode.
         """
 
         if attr is None:
             attr = self.default_attr
 
         if ignore_excluded is None:
             ignore_excluded = self.ignore_excluded
 
+        if ignore_space_tokens is None:
+            ignore_space_tokens = self.ignore_space_tokens
+
         if alignment_mode is None:
             alignment_mode = self.alignment_mode
 
         if flags is None:
             flags = self.flags
 
         patterns = [compile_regex(pattern, flags) for pattern in patterns]
 
-        self.regex.append((key, patterns, attr, ignore_excluded, alignment_mode))
+        self.regex.append(
+            (
+                key,
+                patterns,
+                attr,
+                ignore_excluded,
+                ignore_space_tokens,
+                alignment_mode,
+            )
+        )
 
     def remove(
         self,
         key: str,
     ):
         """
         Remove a pattern for the registry.
@@ -308,15 +342,15 @@
 
         Raises
         ------
         ValueError
             If the key is not present in the registered patterns.
         """
         n = len(self.regex)
-        self.regex = [(k, p, a, i, am) for k, p, a, i, am in self.regex if k != key]
+        self.regex = [pat for pat in self.regex if pat[0] != key]
         if len(self.regex) == n:
             raise ValueError(f"`{key}` is not referenced in the matcher")
 
     def __len__(self):
         return len(set([regex[0] for regex in self.regex]))
 
     def match(
@@ -333,16 +367,23 @@
 
         Yields
         -------
         span:
             A match.
         """
 
-        for key, patterns, attr, ignore_excluded, alignment_mode in self.regex:
-            text = get_text(doclike, attr, ignore_excluded)
+        for (
+            key,
+            patterns,
+            attr,
+            ignore_excluded,
+            ignore_space_tokens,
+            alignment_mode,
+        ) in self.regex:
+            text = get_text(doclike, attr, ignore_excluded, ignore_space_tokens)
 
             for pattern in patterns:
                 for match in pattern.finditer(text):
                     logger.trace(f"Matched a regex from {key}: {repr(match.group())}")
 
                     start_char, end_char = span_from_match(
                         match=match,
@@ -353,14 +394,15 @@
                         doclike=doclike,
                         start_char=start_char,
                         end_char=end_char,
                         key=key,
                         attr=attr,
                         alignment_mode=alignment_mode,
                         ignore_excluded=ignore_excluded,
+                        ignore_space_tokens=ignore_space_tokens,
                     )
 
                     if span is None:
                         continue
 
                     yield span, match
 
@@ -378,16 +420,23 @@
 
         Yields
         -------
         span:
             A match.
         """
 
-        for key, patterns, attr, ignore_excluded, alignment_mode in self.regex:
-            text = get_text(doclike, attr, ignore_excluded)
+        for (
+            key,
+            patterns,
+            attr,
+            ignore_excluded,
+            ignore_space_tokens,
+            alignment_mode,
+        ) in self.regex:
+            text = get_text(doclike, attr, ignore_excluded, ignore_space_tokens)
 
             for pattern in patterns:
                 for match in pattern.finditer(text):
                     logger.trace(f"Matched a regex from {key}: {repr(match.group())}")
 
                     start_char, end_char = span_from_match(
                         match=match,
@@ -398,26 +447,28 @@
                         doclike=doclike,
                         start_char=start_char,
                         end_char=end_char,
                         key=key,
                         attr=attr,
                         alignment_mode=alignment_mode,
                         ignore_excluded=ignore_excluded,
+                        ignore_space_tokens=ignore_space_tokens,
                     )
                     group_spans = {}
                     for group_key, group_string in match.groupdict().items():
                         if group_string:
                             group_spans[group_key] = create_span(
                                 doclike=doclike,
                                 start_char=match.start(group_key),
                                 end_char=match.end(group_key),
                                 key=group_key,
                                 attr=attr,
                                 alignment_mode=alignment_mode,
                                 ignore_excluded=ignore_excluded,
+                                ignore_space_tokens=ignore_space_tokens,
                             )
 
                     yield span, group_spans
 
     def __call__(
         self,
         doclike: Union[Doc, Span],
```

### Comparing `edsnlp-0.7.4/edsnlp/matchers/simstring.py` & `edsnlp-0.8.0/edsnlp/matchers/simstring.py`

 * *Files 9% similar despite different names*

```diff
@@ -53,14 +53,15 @@
         self,
         vocab: Vocab,
         path: Optional[Union[Path, str]] = None,
         measure: SimilarityMeasure = SimilarityMeasure.dice,
         threshold: float = 0.75,
         windows: int = 5,
         ignore_excluded: bool = False,
+        ignore_space_tokens: bool = False,
         attr: str = "NORM",
     ):
         """
         PhraseMatcher that allows to skip excluded tokens.
         Heavily inspired by https://github.com/Georgetown-IR-Lab/QuickUMLS
 
         Parameters
@@ -72,15 +73,17 @@
         measure: SimilarityMeasure
             Name of the similarity measure.
             One of [jaccard, dice, overlap, cosine]
         windows: int
             Maximum number of words in a candidate span
         threshold: float
             Minimum similarity value to match a concept's synonym
-        ignore_excluded : bool, optional
+        ignore_excluded : Optional[bool]
+            Whether to exclude tokens that have an EXCLUDED tag, by default False
+        ignore_space_tokens : Optional[bool]
             Whether to exclude tokens that have a "SPACE" tag, by default False
         attr : str
             Default attribute to match on, by default "TEXT".
             Can be overridden in the `add` method.
             To match on a custom attribute, prepend the attribute name with `_`.
         """
 
@@ -92,33 +95,38 @@
         )
 
         self.vocab = vocab
         self.windows = windows
         self.measure = measure
         self.threshold = threshold
         self.ignore_excluded = ignore_excluded
+        self.ignore_space_tokens = ignore_space_tokens
         self.attr = attr
 
         if path is None:
             path = tempfile.mkdtemp()
         self.path = Path(path)
 
         self.ss_reader = None
         self.syn2cuis = None
 
-    def build_patterns(self, nlp: Language, terms: Dict[str, Iterable[str]]):
+    def build_patterns(
+        self, nlp: Language, terms: Dict[str, Iterable[str]], progress: bool = False
+    ):
         """
         Build patterns and adds them for matching.
 
         Parameters
         ----------
         nlp : Language
             The instance of the spaCy language class.
         terms : Patterns
             Dictionary of label/terms, or label/dictionary of terms/attribute.
+        progress: bool
+            Whether to track progress when preprocessing terms
         """
 
         self.ss_reader = None
         self.syn2cuis = None
 
         syn2cuis = defaultdict(lambda: [])
         token_pipelines = [
@@ -127,18 +135,21 @@
             if any(
                 "token" in assign and not assign == "token.is_sent_start"
                 for assign in nlp.get_pipe_meta(name).assigns
             )
         ]
         with nlp.select_pipes(enable=token_pipelines):
             with SimstringWriter(self.path) as ss_db:
-                for cui, synset in tqdm(terms.items()):
+                for cui, synset in tqdm(terms.items()) if progress else terms.items():
                     for term in nlp.pipe(synset):
                         norm_text = get_text(
-                            term, self.attr, ignore_excluded=self.ignore_excluded
+                            term,
+                            self.attr,
+                            ignore_excluded=self.ignore_excluded,
+                            ignore_space_tokens=self.ignore_space_tokens,
                         )
                         term = "##" + norm_text + "##"
                         ss_db.insert(term)
                         syn2cuis[term].append(cui)
         syn2cuis = {term: tuple(sorted(set(cuis))) for term, cuis in syn2cuis.items()}
         with open(self.path / "cui-db.pkl", "wb") as f:
             pickle.dump(syn2cuis, f)
@@ -170,20 +181,20 @@
                 doclike=sent,
                 attr=self.attr,
                 ignore_excluded=self.ignore_excluded,
             )
             sent_start = getattr(sent, "start", 0)
             for size in range(1, self.windows):
                 for i in range(0, len(offsets) - size):
-                    begin_char, _, begin_i = offsets[i]
-                    _, end_char, end_i = offsets[i + size]
+                    begin_char, _, begin_i, _ = offsets[i]
+                    _, end_char, _, end_i = offsets[i + size]
                     span_text = "##" + text[begin_char:end_char] + "##"
                     matches = self.ss_reader.retrieve(span_text)
                     for res in matches:
-                        sim = similarity(span_text, res, measure=self.measure)
+                        sim = _similarity(span_text, res, measure=self.measure)
                         for cui in self.syn2cuis[res]:
                             ents.append(
                                 (cui, begin_i + sent_start, end_i + sent_start, sim)
                             )
 
         sorted_spans = sorted(ents, key=simstring_sort_key, reverse=True)
         results = []
@@ -201,15 +212,15 @@
                 for span_data in results
             ]
             return spans
         else:
             return [(self.vocab.strings[span[0]], span[1], span[2]) for span in results]
 
 
-def similarity(x: str, y: str, measure: SimilarityMeasure = SimilarityMeasure.dice):
+def _similarity(x: str, y: str, measure: SimilarityMeasure = SimilarityMeasure.dice):
 
     x_ngrams = {x[i : i + 3] for i in range(0, len(x) - 3)}
     y_ngrams = {y[i : i + 3] for i in range(0, len(y) - 3)}
 
     if measure == SimilarityMeasure.jaccard:
         return len(x_ngrams & y_ngrams) / (len(x_ngrams | y_ngrams))
 
@@ -218,45 +229,47 @@
 
     if measure == SimilarityMeasure.cosine:
         return len(x_ngrams & y_ngrams) / sqrt(len(x_ngrams) * len(y_ngrams))
 
     if measure == SimilarityMeasure.overlap:
         return len(x_ngrams & y_ngrams)
 
-    raise ValueError("Cannot compute similarity {}".format(repr(measure)))
-
 
 def simstring_sort_key(span_data: Tuple[str, int, int, float]):
     return span_data[3], span_data[2] - span_data[1], -span_data[1]
 
 
 @lru_cache(maxsize=128)
 def get_text_and_offsets(
     doclike: Union[Span, Doc],
     attr: str = "TEXT",
     ignore_excluded: bool = True,
+    ignore_space_tokens: bool = True,
 ) -> Tuple[str, List[Tuple[int, int, int]]]:
     """
     Align different representations of a `Doc` or `Span` object.
 
     Parameters
     ----------
     doclike : Doc
         spaCy `Doc` or `Span` object
     attr : str, optional
         Attribute to use, by default `"TEXT"`
-    ignore_excluded : bool, optional
+    ignore_excluded : bool
         Whether to remove excluded tokens, by default True
+    ignore_space_tokens : bool
+        Whether to remove space tokens, by default False
+
 
     Returns
     -------
-    Tuple[str, List[Tuple[int, int, int]]]
+    Tuple[str, List[Tuple[int, int, int, int]]]
         The new clean text and offset tuples for each word giving the begin char indice
         of the word in the new text, the end char indice of its preceding word and the
-        indice of the word in the original document
+        begin / end indices of the word in the original document
     """
     attr = attr.upper()
     attr = ATTRIBUTES.get(attr, attr)
 
     custom = attr.startswith("_")
 
     if custom:
@@ -265,31 +278,35 @@
     offsets = []
 
     cursor = 0
 
     text = []
 
     last = cursor
+    last_i = 0
     for i, token in enumerate(doclike):
 
-        if not ignore_excluded or not token._.excluded:
+        if (not ignore_excluded or token.tag_ != "EXCLUDED") and (
+            not ignore_space_tokens or token.tag_ != "SPACE"
+        ):
             if custom:
                 token_text = getattr(token._, attr)
             else:
                 token_text = getattr(token, attr)
 
             # We add the cursor
             end = cursor + len(token_text)
-            offsets.append((cursor, last, i))
+            offsets.append((cursor, last, i, last_i + 1))
 
             cursor = end
             last = end
+            last_i = i
 
             text.append(token_text)
 
             if token.whitespace_:
                 cursor += 1
                 text.append(" ")
 
-    offsets.append((cursor, last, len(doclike)))
+    offsets.append((cursor, last, len(doclike), last_i + 1))
 
     return "".join(text), offsets
```

### Comparing `edsnlp-0.7.4/edsnlp/matchers/utils/offset.py` & `edsnlp-0.8.0/edsnlp/matchers/utils/offset.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,26 +16,29 @@
 
 
 @lru_cache(maxsize=32)
 def alignment(
     doc: Doc,
     attr: str = "TEXT",
     ignore_excluded: bool = True,
+    ignore_space_tokens: bool = True,
 ) -> Tuple[List[int], List[int]]:
     """
     Align different representations of a `Doc` or `Span` object.
 
     Parameters
     ----------
     doc : Doc
         spaCy `Doc` or `Span` object
     attr : str, optional
         Attribute to use, by default `"TEXT"`
     ignore_excluded : bool, optional
         Whether to remove excluded tokens, by default True
+    ignore_space_tokens : bool, optional
+        Whether to remove space tokens, by default True
 
     Returns
     -------
     Tuple[List[int], List[int]]
         An alignment tuple: original and clean lists.
     """
     assert isinstance(doc, Doc)
@@ -54,15 +57,17 @@
     original = []
     clean = []
 
     cursor = 0
 
     for token in doc:
 
-        if not ignore_excluded or token.tag_ != "EXCLUDED":
+        if (not ignore_excluded or token.tag_ != "EXCLUDED") and (
+            not ignore_space_tokens or not token.tag_ == "SPACE"
+        ):
 
             # The token is not excluded, we add its extremities to the list
             original.append(token.idx)
 
             # We add the cursor
             clean.append(cursor)
             cursor += length(token)
@@ -73,14 +78,15 @@
     return original, clean
 
 
 def offset(
     doc: Doc,
     attr: str,
     ignore_excluded: bool,
+    ignore_space_tokens: bool,
     index: int,
 ) -> int:
     """
     Compute offset between the original text and a given representation
     (defined by the couple `attr`, `ignore_excluded`).
 
     The alignment itself is computed with
@@ -90,28 +96,31 @@
     ----------
     doc : Doc
         The spaCy `Doc` object
     attr : str
         The attribute used by the [`RegexMatcher`][edsnlp.matchers.regex.RegexMatcher]
         (eg `NORM`)
     ignore_excluded : bool
-        Whether the RegexMatcher ignores excluded tokens.
+        Whether to ignore excluded tokens.
+    ignore_space_tokens : bool
+        Whether to ignore spaces tokens.
     index : int
         The index in the pre-processed text.
 
     Returns
     -------
     int
         The offset. To get the character index in the original document,
         just do: `#!python original = index + offset(doc, attr, ignore_excluded, index)`
     """
     original, clean = alignment(
         doc=doc,
         attr=attr,
         ignore_excluded=ignore_excluded,
+        ignore_space_tokens=ignore_space_tokens,
     )
 
     # We use bisect to efficiently find the correct rightmost-lower index
     i = bisect_left(clean, index)
     i = min(i, len(original) - 1)
 
     return original[i] - clean[i]
```

### Comparing `edsnlp-0.7.4/edsnlp/matchers/utils/text.py` & `edsnlp-0.8.0/edsnlp/matchers/utils/text.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,44 +7,50 @@
 
 
 @lru_cache(32)
 def get_text(
     doclike: Union[Doc, Span],
     attr: str,
     ignore_excluded: bool,
+    ignore_space_tokens: bool = False,
 ) -> str:
     """
     Get text using a custom attribute, possibly ignoring excluded tokens.
 
     Parameters
     ----------
     doclike : Union[Doc, Span]
         Doc or Span to get text from.
     attr : str
         Attribute to use.
     ignore_excluded : bool
         Whether to skip excluded tokens, by default False
+    ignore_space_tokens : bool
+        Whether to skip space tokens, by default False
 
     Returns
     -------
     str
         Extracted text.
     """
 
     attr = attr.upper()
 
-    if not ignore_excluded:
+    if not ignore_excluded and not ignore_space_tokens:
         if attr == "TEXT":
             return doclike.text
         elif attr == "LOWER":
             return doclike.text.lower()
         else:
             tokens = doclike
     else:
-        tokens = [t for t in doclike if t.tag_ != "EXCLUDED"]
+        if not ignore_space_tokens:
+            tokens = [t for t in doclike if t.tag_ != "EXCLUDED"]
+        else:
+            tokens = [t for t in doclike if t.tag_ not in ("EXCLUDED", "SPACE")]
 
     if not tokens:
         return ""
 
     attr = ATTRIBUTES.get(attr, attr)
 
     if attr.startswith("_"):
```

### Comparing `edsnlp-0.7.4/edsnlp/models/pytorch_wrapper.py` & `edsnlp-0.8.0/edsnlp/pipelines/trainable/pytorch_wrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import typing
-from typing import Any, Callable, Iterable, List, Optional, OrderedDict, Tuple
+from typing import Any, Callable, Iterable, List, Optional, OrderedDict, Sequence, Tuple
 
 import torch
 from spacy.tokens import Doc
 from thinc.model import Model
 from thinc.shims import PyTorchShim
 from thinc.types import ArgsKwargs, Floats1d, Floats2d, Ints2d
 from thinc.util import (
@@ -23,15 +23,15 @@
         self,
         input_size: Optional[int] = None,
         n_labels: Optional[int] = None,
     ):
         """
         Pytorch wrapping module for Spacy.
         Models that expect to be wrapped with
-        [wrap_pytorch_model][edsnlp.models.pytorch_wrapper.wrap_pytorch_model]
+        [wrap_pytorch_model][edsnlp.pipelines.trainable.pytorch_wrapper.wrap_pytorch_model]
         should inherit from this module.
 
         Parameters
         ----------
         input_size: int
             Size of the input embeddings
         n_labels: int
@@ -58,15 +58,15 @@
         Parameters
         ----------
         state_dict: OrderedDict[str, torch.Tensor]
         strict: bool
         """
         self.cfg = state_dict.pop("cfg")
         self.initialize()
-        super().load_state_dict(state_dict, strict)
+        super().load_state_dict(state_dict, False)
 
     def state_dict(self, destination=None, prefix="", keep_vars=False):
         """
         Loads the model inplace from a dumped `state_dict` object
 
         Parameters
         ----------
@@ -241,15 +241,15 @@
     X: List[Doc]
         list of documents on which we apply the encoder layer
     Y: Ints2d
         Unused gold spans
 
     Returns
     -------
-
+    Model
     """
     encoder = model.get_ref("encoder")
     if X is not None:
         encoder.initialize(X)
 
     pt_model = model.attrs["pt_model"]
     pt_model.cfg["input_size"] = encoder.get_dim("nO")
@@ -292,14 +292,15 @@
 ]:
     ...
 
 
 def wrap_pytorch_model(
     encoder: Model[List[Doc], List[Floats2d]],
     pt_model: PytorchWrapperModule,
+    attrs: Sequence[str] = ("set_n_labels",),
 ) -> Model[
     Tuple[Iterable[Doc], Optional[PredT], Optional[bool]],
     Tuple[Floats1d, PredT],
 ]:
     """
     Chain and wraps a spaCy/Thinc encoder model (like a tok2vec) and a pytorch model.
     The loss should be computed directly in the Pytorch module and Categorical
@@ -307,28 +308,30 @@
 
     Parameters
     ----------
     encoder: Model[List[Doc], List[Floats2d]]
         The Thinc document token embedding layer
     pt_model: PytorchWrapperModule
         The Pytorch model
+    attrs: Sequence[str]
+        The attributes of the Pytorch model that should be copied to the Thinc model
 
     Returns
     -------
         Tuple[Iterable[Doc], Optional[PredT], Optional[bool]],
         # inputs (docs, gold, *rest, is_predict)
         Tuple[Floats1d, PredT],
         # outputs (loss, *additional_outputs)
     """
     return Model(
         "pytorch",
         pytorch_forward,
         attrs={
-            "set_n_labels": pt_model.set_n_labels,
             "pt_model": pt_model,
+            **{attr: getattr(pt_model, attr) for attr in attrs},
         },
         layers=[encoder],
         shims=[PyTorchShim(pt_model)],
         refs={"encoder": encoder},
         dims={"nI": None, "nO": None},
         init=instance_init,
     )
```

### Comparing `edsnlp-0.7.4/edsnlp/models/stack_crf_ner.py` & `edsnlp-0.8.0/edsnlp/pipelines/trainable/nested_ner/stack_crf_ner.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,19 @@
 import torch
 from loguru import logger
 from spacy import registry
 from spacy.tokens import Doc
 from thinc.model import Model
 from thinc.types import Floats1d, Floats2d, Ints2d
 
-from edsnlp.models.pytorch_wrapper import PytorchWrapperModule, wrap_pytorch_model
-from edsnlp.models.torch.crf import IMPOSSIBLE, MultiLabelBIOULDecoder
+from edsnlp.pipelines.trainable.layers.crf import IMPOSSIBLE, MultiLabelBIOULDecoder
+from edsnlp.pipelines.trainable.pytorch_wrapper import (
+    PytorchWrapperModule,
+    wrap_pytorch_model,
+)
 
 
 class CRFMode(str, Enum):
     independent = "independent"
     joint = "joint"
     marginal = "marginal"
 
@@ -172,19 +175,37 @@
         return loss
 
 
 @registry.layers("eds.stack_crf_ner_model.v1")
 def create_model(
     tok2vec: Model[List[Doc], List[Floats2d]],
     mode: CRFMode,
-    n_labels: int = None,
+    n_labels: Optional[int] = None,
 ) -> Model[
     Tuple[Iterable[Doc], Optional[Ints2d], Optional[bool]],
     Tuple[Floats1d, Ints2d],
 ]:
+    """
+    Parameters
+    ----------
+    tok2vec: Model[List[Doc], List[Floats2d]]
+        The tok2vec embedding model used to generate the word embeddings
+    mode: CRFMode
+        How the CRF loss is computed
+
+        - `joint`: Loss accounts for CRF transitions
+        - `independent`: Loss does not account for CRF transitions (softmax loss)
+        - `marginal`: Tag scores are smoothly updated with CRF transitions, and softmax loss is applied
+    n_labels: Optional[int]
+        Number of labels. This will be automatically set later during initialization
+
+    Returns
+    -------
+    Model
+    """  # noqa: E501
     return wrap_pytorch_model(  # noqa
         encoder=tok2vec,
         pt_model=StackedCRFNERModule(
             input_size=None,  # will be set later during initialization
             n_labels=n_labels,  # will likely be set later during initialization
             mode=mode,
         ),
```

### Comparing `edsnlp-0.7.4/edsnlp/models/torch/crf.py` & `edsnlp-0.8.0/edsnlp/pipelines/trainable/layers/crf.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         forbidden_transitions: torch.BoolTensor
             Shape: n_tags * n_tags
             Impossible transitions (1 means impossible) from position n to position n+1
         start_forbidden_transitions: Optional[torch.BoolTensor]
             Shape: n_tags
             Impossible transitions at the start of a sequence
         end_forbidden_transitions Optional[torch.BoolTensor]
-            Shape: n_tags
+            Shape is (n_tags,)
             Impossible transitions at the end of a sequence
         learnable_transitions: bool
             Should we learn transition scores to complete the
             constraints ?
         with_start_end_transitions:
             Should we apply start-end transitions.
             If learnable_transitions is True, learn start/end transition scores
@@ -406,16 +406,14 @@
         """
         Convert a sequence of multiple label BIOUL tags to a sequence of spans
 
         Parameters
         ----------
         tags: torch.LongTensor
             Shape: n_samples * n_labels * n_tokens
-        mask: torch.BoolTensor
-            Shape: n_samples * n_labels * n_tokens
 
         Returns
         -------
         torch.LongTensor
             Shape: n_spans *  4
             (doc_idx, label_idx, begin, end)
         """
```

### Comparing `edsnlp-0.7.4/edsnlp/patch_spacy_dot_components.py` & `edsnlp-0.8.0/edsnlp/patch_spacy_dot_components.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/core/context/context.py` & `edsnlp-0.8.0/edsnlp/pipelines/core/context/context.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/core/contextual_matcher/contextual_matcher.py` & `edsnlp-0.8.0/edsnlp/pipelines/core/contextual_matcher/contextual_matcher.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,23 +16,23 @@
 from edsnlp.utils.lists import flatten
 
 from . import models
 
 
 @lru_cache(64)
 def get_window(
-    doclike: Union[Doc, Span],
-    window: Tuple[int, int],
+    doclike: Union[Doc, Span], window: Tuple[int, int], limit_to_sentence: bool
 ):
+    start_limit = doclike.sent.start if limit_to_sentence else 0
+    end_limit = doclike.sent.end if limit_to_sentence else len(doclike.doc)
 
-    return doclike.doc[
-        max(doclike.start + window[0], doclike.sent.start) : min(
-            doclike.end + window[1], doclike.sent.end
-        )
-    ]
+    start = max(doclike.start + window[0], start_limit)
+    end = min(doclike.end + window[1], end_limit)
+
+    return doclike.doc[start:end]
 
 
 class ContextualMatcher(BaseComponent):
     """
     Allows additional matching in the surrounding context of the main match group,
     for qualification/filtering.
 
@@ -40,57 +40,71 @@
     ----------
     nlp : Language
         spaCy `Language` object.
     name : str
         The name of the pipe
     patterns: Union[Dict[str, Any], List[Dict[str, Any]]]
         The configuration dictionary
+    assign_as_span : bool
+        Whether to store eventual extractions defined via the `assign` key as Spans
+        or as string
     attr : str
         Attribute to match on, eg `TEXT`, `NORM`, etc.
     ignore_excluded : bool
         Whether to skip excluded tokens during matching.
+    ignore_space_tokens: bool
+        Whether to skip space tokens during matching.
     alignment_mode : str
         Overwrite alignment mode.
+    regex_flags : Union[re.RegexFlag, int]
+        RegExp flags to use when matching, filtering and assigning (See
+        [here](https://docs.python.org/3/library/re.html#flags))
+    include_assigned : bool
+        Whether to include (eventual) assign matches to the final entity
     """
 
     def __init__(
         self,
         nlp: Language,
         name: str,
         patterns: Union[Dict[str, Any], List[Dict[str, Any]]],
-        assign_as_span: bool,
-        alignment_mode: str,
-        attr: str,
-        regex_flags: Union[re.RegexFlag, int],
-        ignore_excluded: bool,
-        include_assigned: bool,
+        assign_as_span: bool = False,
+        alignment_mode: str = "expand",
+        attr: str = "NORM",
+        regex_flags: Union[re.RegexFlag, int] = 0,
+        ignore_excluded: bool = False,
+        ignore_space_tokens: bool = False,
+        include_assigned: bool = False,
     ):
         self.name = name
         self.nlp = nlp
         self.attr = attr
         self.assign_as_span = assign_as_span
         self.ignore_excluded = ignore_excluded
+        self.ignore_space_tokens = ignore_space_tokens
         self.alignment_mode = alignment_mode
         self.regex_flags = regex_flags
         self.include_assigned = include_assigned
 
         # Configuration parsing
         patterns = models.FullConfig.parse_obj(patterns).__root__
         self.patterns = {pattern.source: pattern for pattern in patterns}
 
         # Matchers for the anchors
         self.phrase_matcher = EDSPhraseMatcher(
             self.nlp.vocab,
             attr=attr,
             ignore_excluded=ignore_excluded,
+            ignore_space_tokens=ignore_space_tokens,
         )
         self.regex_matcher = RegexMatcher(
             attr=attr,
             flags=regex_flags,
             ignore_excluded=ignore_excluded,
+            ignore_space_tokens=ignore_space_tokens,
             alignment_mode=alignment_mode,
         )
 
         self.phrase_matcher.build_patterns(
             nlp=nlp,
             terms={
                 source: {
@@ -119,56 +133,59 @@
         self.reduce_mode = {}
 
         # Will contain the name of the assign matcher from which
         # entity will be replaced (for each source)
         self.replace_key = {}
 
         for source, p in self.patterns.items():
-
             p = p.dict()
 
             for exclude in p["exclude"]:
-
                 exclude_matcher = RegexMatcher(
-                    attr=p["regex_attr"] or self.attr,
-                    flags=p["regex_flags"] or self.regex_flags,
+                    attr=exclude["regex_attr"] or p["regex_attr"] or self.attr,
+                    flags=exclude["regex_flags"]
+                    or p["regex_flags"]
+                    or self.regex_flags,
                     ignore_excluded=ignore_excluded,
+                    ignore_space_tokens=ignore_space_tokens,
                     alignment_mode="expand",
                 )
 
                 exclude_matcher.build_patterns(regex={"exclude": exclude["regex"]})
 
                 self.exclude_matchers[source].append(
                     dict(
                         matcher=exclude_matcher,
                         window=exclude["window"],
+                        limit_to_sentence=exclude["limit_to_sentence"],
                     )
                 )
 
             replace_key = None
 
             for assign in p["assign"]:
-
                 assign_matcher = RegexMatcher(
-                    attr=p["regex_attr"] or self.attr,
-                    flags=p["regex_flags"] or self.regex_flags,
+                    attr=assign["regex_attr"] or p["regex_attr"] or self.attr,
+                    flags=assign["regex_flags"] or p["regex_flags"] or self.regex_flags,
                     ignore_excluded=ignore_excluded,
+                    ignore_space_tokens=ignore_space_tokens,
                     alignment_mode=alignment_mode,
                     span_from_group=True,
                 )
 
                 assign_matcher.build_patterns(
                     regex={assign["name"]: assign["regex"]},
                 )
 
                 self.assign_matchers[source].append(
                     dict(
                         name=assign["name"],
                         matcher=assign_matcher,
                         window=assign["window"],
+                        limit_to_sentence=assign["limit_to_sentence"],
                         replace_entity=assign["replace_entity"],
                         reduce_mode=assign["reduce_mode"],
                     )
                 )
 
                 if assign["replace_entity"]:
                     # We know that there is only one assign name
@@ -205,19 +222,20 @@
         -------
         Optional[Span]
             None if the span was filtered, the span else
         """
         source = span.label_
         to_keep = True
         for matcher in self.exclude_matchers[source]:
-
             window = matcher["window"]
+            limit_to_sentence = matcher["limit_to_sentence"]
             snippet = get_window(
                 doclike=span,
                 window=window,
+                limit_to_sentence=limit_to_sentence,
             )
 
             if (
                 next(
                     matcher["matcher"](snippet, as_spans=True),
                     None,
                 )
@@ -254,22 +272,23 @@
             return
 
         source = span.label_
         assigned_dict = models.AssignDict(reduce_mode=self.reduce_mode[source])
         replace_key = None
 
         for matcher in self.assign_matchers[source]:
-
             attr = self.patterns[source].regex_attr or matcher["matcher"].default_attr
             window = matcher["window"]
+            limit_to_sentence = matcher["limit_to_sentence"]
             replace_entity = matcher["replace_entity"]  # Boolean
 
             snippet = get_window(
                 doclike=span,
                 window=window,
+                limit_to_sentence=limit_to_sentence,
             )
 
             # Getting the matches
             assigned_list = list(matcher["matcher"].match(snippet))
 
             assigned_list = [
                 (span, span)
@@ -278,16 +297,17 @@
                     span,
                     create_span(
                         doclike=snippet,
                         start_char=match.start(0),
                         end_char=match.end(0),
                         key=matcher["matcher"].regex[0][0],
                         attr=matcher["matcher"].regex[0][2],
-                        alignment_mode=matcher["matcher"].regex[0][4],
+                        alignment_mode=matcher["matcher"].regex[0][5],
                         ignore_excluded=matcher["matcher"].regex[0][3],
+                        ignore_space_tokens=matcher["matcher"].regex[0][4],
                     ),
                 )
                 for (span, match) in assigned_list
             ]
 
             # assigned_list now contains tuples with
             # - the first element being the span extracted from the group
@@ -350,20 +370,18 @@
 
             for replaced in kept_ents:
                 # Propagating attributes from the anchor
                 replaced._.source = source
                 replaced.label_ = self.name
 
         else:
-
             # Entity expansion
             expandables = flatten([a["span"] for a in assigned_dict.values()])
 
             if self.include_assigned and expandables:
-
                 span = Span(
                     span.doc,
                     min(expandables + [span], key=attrgetter("start")).start,
                     max(expandables + [span], key=attrgetter("end")).end,
                     span.label_,
                 )
```

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/core/contextual_matcher/models.py` & `edsnlp-0.8.0/edsnlp/pipelines/core/contextual_matcher/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import re
 from typing import List, Optional, Tuple, Union
 
+import regex
 from pydantic import BaseModel, Extra, validator
 
 from edsnlp.matchers.utils import ListOrStr
 
 Flags = Union[re.RegexFlag, int]
 Window = Union[
     Tuple[int, int],
@@ -85,15 +86,17 @@
             "keep_last": keep_last,
         }
 
 
 class SingleExcludeModel(BaseModel):
     regex: ListOrStr = []
     window: Window
+    limit_to_sentence: Optional[bool] = True
     regex_flags: Optional[Flags] = None
+    regex_attr: Optional[str] = None
 
     @validator("regex")
     def exclude_regex_validation(cls, v):
         if type(v) == str:
             v = [v]
         return v
 
@@ -114,21 +117,25 @@
         return v
 
 
 class SingleAssignModel(BaseModel):
     name: str
     regex: str
     window: Window
+    limit_to_sentence: Optional[bool] = True
     regex_flags: Optional[Flags] = None
+    regex_attr: Optional[str] = None
     replace_entity: bool = False
     reduce_mode: Optional[str] = None
 
     @validator("regex")
     def check_single_regex_group(cls, pat):
-        compiled_pat = re.compile(pat)
+        compiled_pat = regex.compile(
+            pat
+        )  # Using regex to allow multiple fgroups with same name
         n_groups = compiled_pat.groups
         assert n_groups == 1, (
             "The pattern {pat} should have only one capturing group, not {n_groups}"
         ).format(
             pat=pat,
             n_groups=n_groups,
         )
```

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/core/endlines/endlines.py` & `edsnlp-0.8.0/edsnlp/pipelines/core/endlines/endlines.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,14 +45,15 @@
             nlp,
             terms=None,
             attr="TEXT",
             regex=dict(
                 new_line=r"\n+",
             ),
             ignore_excluded=False,
+            ignore_space_tokens=False,
             **kwargs,
         )
 
         self._read_model(end_lines_model)
 
     def _read_model(self, end_lines_model: Optional[Union[str, EndLinesModel]]):
         """
```

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/core/endlines/endlinesmodel.py` & `edsnlp-0.8.0/edsnlp/pipelines/core/endlines/endlinesmodel.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/core/endlines/functional.py` & `edsnlp-0.8.0/edsnlp/pipelines/core/endlines/functional.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/core/matcher/factory.py` & `edsnlp-0.8.0/edsnlp/pipelines/ner/cim10/factory.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,53 +1,67 @@
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Dict, Union
 
 from spacy.language import Language
 
-from edsnlp.pipelines.core.matcher import GenericMatcher
-from edsnlp.pipelines.core.matcher.matcher import GenericTermMatcher
-from edsnlp.utils.deprecation import deprecated_factory
+from edsnlp.pipelines.core.terminology import TerminologyMatcher, TerminologyTermMatcher
+
+from . import patterns
 
 DEFAULT_CONFIG = dict(
-    terms=None,
-    regex=None,
-    attr="TEXT",
+    attr="NORM",
     ignore_excluded=False,
-    term_matcher=GenericTermMatcher.exact,
+    ignore_space_tokens=False,
+    term_matcher=TerminologyTermMatcher.exact,
     term_matcher_config={},
 )
 
 
-@deprecated_factory(
-    "matcher",
-    "eds.matcher",
-    default_config=DEFAULT_CONFIG,
-    assigns=["doc.ents", "doc.spans"],
-)
 @Language.factory(
-    "eds.matcher", default_config=DEFAULT_CONFIG, assigns=["doc.ents", "doc.spans"]
+    "eds.cim10", default_config=DEFAULT_CONFIG, assigns=["doc.ents", "doc.spans"]
 )
 def create_component(
     nlp: Language,
-    name: str,
-    terms: Optional[Dict[str, Union[str, List[str]]]],
-    attr: Union[str, Dict[str, str]],
-    regex: Optional[Dict[str, Union[str, List[str]]]],
-    ignore_excluded: bool,
-    term_matcher: GenericTermMatcher,
-    term_matcher_config: Dict[str, Any],
+    name: str = "eds.cim10",
+    attr: Union[str, Dict[str, str]] = "NORM",
+    ignore_excluded: bool = False,
+    ignore_space_tokens: bool = False,
+    term_matcher: TerminologyTermMatcher = TerminologyTermMatcher.exact,
+    term_matcher_config: Dict[str, Any] = {},
 ):
-    assert not (terms is None and regex is None)
-
-    if terms is None:
-        terms = dict()
-    if regex is None:
-        regex = dict()
+    """
+    Create a factory that returns new a component to recognize and normalize CIM10 codes
+    and concepts in documents.
+
+    Parameters
+    ----------
+    nlp: Language
+        spaCy `Language` object.
+    name: str
+        The name of the pipe
+    attr: Union[str, Dict[str, str]]
+        Attribute to match on, eg `TEXT`, `NORM`, etc.
+    ignore_excluded: bool
+        Whether to skip excluded tokens during matching.
+    ignore_space_tokens: bool
+        Whether to skip space tokens during matching.
+    term_matcher: TerminologyTermMatcher
+        The term matcher to use, either `TerminologyTermMatcher.exact` or
+        `TerminologyTermMatcher.simstring`
+    term_matcher_config: Dict[str, Any]
+        The configuration for the term matcher
+
+    Returns
+    -------
+    TerminologyMatcher
+    """
 
-    return GenericMatcher(
+    return TerminologyMatcher(
         nlp,
-        terms=terms,
+        label="cim10",
+        regex=None,
+        terms=patterns.get_patterns(),
         attr=attr,
-        regex=regex,
         ignore_excluded=ignore_excluded,
+        ignore_space_tokens=ignore_space_tokens,
         term_matcher=term_matcher,
         term_matcher_config=term_matcher_config,
     )
```

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/core/matcher/matcher.py` & `edsnlp-0.8.0/edsnlp/pipelines/core/matcher/matcher.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,59 +31,68 @@
         A dictionary of regular expressions.
     attr : str
         The default attribute to use for matching.
         Can be overridden using the `terms` and `regex` configurations.
     ignore_excluded : bool
         Whether to skip excluded tokens (requires an upstream
         pipeline to mark excluded tokens).
+    ignore_space_tokens: bool
+        Whether to skip space tokens during matching.
+
+        You won't be able to match on newlines if this is enabled and
+        the "spaces"/"newline" option of `eds.normalizer` is enabled (by default).
     term_matcher: GenericTermMatcher
         The matcher to use for matching phrases ?
         One of (exact, simstring)
     term_matcher_config: Dict[str,Any]
         Parameters of the matcher class
     """
 
     def __init__(
         self,
         nlp: Language,
         terms: Optional[Patterns],
         regex: Optional[Patterns],
         attr: str,
         ignore_excluded: bool,
+        ignore_space_tokens: bool = False,
         term_matcher: GenericTermMatcher = GenericTermMatcher.exact,
         term_matcher_config: Dict[str, Any] = None,
     ):
 
         self.nlp = nlp
 
         self.attr = attr
 
         if term_matcher == GenericTermMatcher.exact:
             self.phrase_matcher = EDSPhraseMatcher(
                 self.nlp.vocab,
                 attr=attr,
                 ignore_excluded=ignore_excluded,
+                ignore_space_tokens=ignore_space_tokens,
                 **(term_matcher_config or {}),
             )
         elif term_matcher == GenericTermMatcher.simstring:
             self.phrase_matcher = SimstringMatcher(
                 self.nlp.vocab,
                 attr=attr,
                 ignore_excluded=ignore_excluded,
+                ignore_space_tokens=ignore_space_tokens,
                 **(term_matcher_config or {}),
             )
         else:
             raise ValueError(
                 f"Algorithm {repr(term_matcher)} does not belong to"
                 f" known matcher [exact, simstring]."
             )
 
         self.regex_matcher = RegexMatcher(
             attr=attr,
             ignore_excluded=ignore_excluded,
+            ignore_space_tokens=ignore_space_tokens,
         )
 
         self.phrase_matcher.build_patterns(nlp=nlp, terms=terms)
         self.regex_matcher.build_patterns(regex=regex)
 
         self.set_extensions()
```

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/core/normalizer/__init__.py` & `edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/__init__.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/core/normalizer/accents/accents.py` & `edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/accents/accents.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/core/normalizer/accents/factory.py` & `edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/accents/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/core/normalizer/lowercase/factory.py` & `edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/lowercase/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/core/normalizer/normalizer.py` & `edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/normalizer.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,48 +2,54 @@
 
 from spacy.tokens import Doc
 
 from .accents import Accents
 from .lowercase import remove_lowercase
 from .pollution import Pollution
 from .quotes import Quotes
+from .spaces import Spaces
 
 
 class Normalizer(object):
     """
     Normalisation pipeline. Modifies the `NORM` attribute,
-    acting on four dimensions :
+    acting on five dimensions :
 
     - `lowercase`: using the default `NORM`
     - `accents`: deterministic and fixed-length normalisation of accents.
     - `quotes`: deterministic and fixed-length normalisation of quotation marks.
-    - `pollution`: removal of pollutions.
+    - `spaces`: "removal" of spaces tokens (via the tag_ attribute).
+    - `pollution`: "removal" of pollutions (via the tag_ attribute).
 
     Parameters
     ----------
     lowercase : bool
         Whether to remove case.
     accents : Optional[Accents]
         Optional `Accents` object.
     quotes : Optional[Quotes]
         Optional `Quotes` object.
+    spaces : Optional[Spaces]
+        Optional `Spaces` object.
     pollution : Optional[Pollution]
         Optional `Pollution` object.
     """
 
     def __init__(
         self,
         lowercase: bool,
         accents: Optional[Accents],
         quotes: Optional[Quotes],
+        spaces: Optional[Spaces],
         pollution: Optional[Pollution],
     ):
         self.lowercase = lowercase
         self.accents = accents
         self.quotes = quotes
+        self.spaces = spaces
         self.pollution = pollution
 
     def __call__(self, doc: Doc) -> Doc:
         """
         Apply the normalisation pipeline, one component at a time.
 
         Parameters
@@ -58,11 +64,12 @@
         """
         if not self.lowercase:
             remove_lowercase(doc)
         if self.accents is not None:
             self.accents(doc)
         if self.quotes is not None:
             self.quotes(doc)
+        if self.spaces is not None:
+            self.spaces(doc)
         if self.pollution is not None:
             self.pollution(doc)
-
         return doc
```

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/core/normalizer/pollution/factory.py` & `edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/pollution/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/core/normalizer/pollution/patterns.py` & `edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/pollution/patterns.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,41 @@
 # noinspection SpellCheckingInspection
-information = (
-    r"(?s)(=====+\s*)?(L\s*e\s*s\sdonnées\s*administratives,\s*sociales\s*|"
-    r"I?nfo\s*rmation\s*aux?\s*patients?|"
-    r"L[’']AP-HP\s*collecte\s*vos\s*données\s*administratives|"
-    r"L[’']Assistance\s*Publique\s*-\s*Hôpitaux\s*de\s*Paris\s*"
-    r"\(?AP-HP\)?\s*a\s*créé\s*une\s*base\s*de\s*données)"
-    r".{,2000}https?:\/\/recherche\.aphp\.fr\/eds\/droit-opposition[\s\.]*"
-)
-
+information = [
+    (
+        r"(?s)(=====+\s*)?(L\s*e\s*s\sdonnées\s*administratives,\s*sociales\s*|"
+        r"I?nfo\s*rmation\s*aux?\s*patients?|"
+        r"L[’']AP-HP\s*collecte\s*vos\s*données\s*administratives|"
+        r"L[’']Assistance\s*Publique\s*-\s*Hôpitaux\s*de\s*Paris\s*"
+        r"\(?AP-HP\)?\s*a\s*créé\s*une\s*base\s*de\s*données)"
+        r".{,2000}https?:\/\/recherche\.aphp\.fr\/eds\/droit-opposition[\s\.]*"
+    ),
+    (
+        r"(?si)l’arrêt\s*du\s*tabac\s*permet\s*de\s*diminuer\s*le\s*risque\s*"
+        r"de\s*maladie\s*cardiovasculaire."
+    ),
+]
 # Example : NBNbWbWbNbWbNBNbNbWbWbNBNbWbNbNbWbNBNbW...
 bars = r"(?i)([nbw]|_|-|=){5,}"
 
 # Biology tables: Prone to false positive with disease names
 biology = r"(\b.*[|¦].*\n)+"
 
 # Leftside note with doctor names
 doctors = r"(?mi)(^((dr)|(pr))(\.|\s|of).*)+"
 
 # Mails or websites
-web = r"(www\.\S*)|(\S*@\S*)"
+web = [
+    r"(www\.\S*)",
+    r"(\S*@\S*)",
+    r"\S*\.(?:fr|com|net|org)",
+]
 
 # Subsection with ICD-10 Codes
-coding = r".*?[a-zA-Z]\d{2,4}.*?(\n|[a-zA-Z]\d{2,4})"
+coding = r".*? \(\d+\) [a-zA-Z]\d{2,4}.*?(\n|[a-zA-Z]\d{2,4})"
+
 
 # New page
 date = r"\b\d\d/\d\d/\d\d\d\d\b"
 ipp = r"80\d{8}"
 page = r"((^\d\/\d\s?)|(^\d\d?\/\d\d\?))"
 footer = rf"(?i)({page}.*\n?pat.*(ipp)?.*\n?(courrier valid.*)?)"
 footer += rf"|(.*{date}.*{ipp}.*)|(imprim.\sle\s{date}.*\d/\d.*\n?pat.*{date})"
```

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/core/normalizer/pollution/pollution.py` & `edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/pollution/pollution.py`

 * *Files 11% similar despite different names*

```diff
@@ -43,15 +43,16 @@
 
         if pollution is None:
             pollution = {k: True for k in patterns.pollution.keys()}
         self.pollution = dict()
 
         for k, v in pollution.items():
             if v is True:
-                self.pollution[k] = [patterns.pollution[k]]
+                pattern = patterns.pollution[k]
+                self.pollution[k] = pattern if isinstance(pattern, list) else [pattern]
             elif isinstance(v, str):
                 self.pollution[k] = [v]
             elif isinstance(v, list):
                 self.pollution[k] = v
 
         self.regex_matcher = RegexMatcher(flags=re.MULTILINE)
         self.build_patterns()
```

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/core/normalizer/quotes/factory.py` & `edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/quotes/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/core/normalizer/quotes/patterns.py` & `edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/quotes/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/core/normalizer/quotes/quotes.py` & `edsnlp-0.8.0/edsnlp/pipelines/core/normalizer/quotes/quotes.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/core/sentences/factory.py` & `edsnlp-0.8.0/edsnlp/pipelines/core/sentences/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/core/sentences/sentences.cpp` & `edsnlp-0.8.0/edsnlp/pipelines/core/sentences/sentences.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-/* Generated by Cython 0.29.32 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h",
+            "/tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h",
             "/usr/include/python3.10/Python.h"
         ],
         "extra_compile_args": [
             "-std=c++11"
         ],
         "include_dirs": [
-            "/tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/core/include",
+            "/tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/core/include",
             "/usr/include/python3.10"
         ],
         "language": "c++",
         "name": "edsnlp.pipelines.core.sentences.sentences",
         "sources": [
             "edsnlp/pipelines/core/sentences/sentences.pyx"
         ]
@@ -33,16 +33,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_32"
-#define CYTHON_HEX_VERSION 0x001D20F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -111,15 +111,15 @@
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -227,15 +227,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -266,15 +266,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -590,35 +590,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
   #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -1163,195 +1163,195 @@
   Py_ssize_t shape[8];
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":690
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":690
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":691
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":691
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":692
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":693
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":693
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":697
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":697
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":698
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":698
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":699
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":700
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":700
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":704
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":704
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":705
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":705
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":714
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":714
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":715
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":715
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":716
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":716
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":718
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":719
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":720
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":720
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":722
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":722
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":723
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":723
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":725
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":726
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":727
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1479,42 +1479,42 @@
  * ctypedef void* (*malloc_t)(size_t n)
  * ctypedef void (*free_t)(void *p)             # <<<<<<<<<<<<<<
  * 
  * cdef class PyMalloc:
  */
 typedef void (*__pyx_t_5cymem_5cymem_free_t)(void *);
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":729
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":730
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":730
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":731
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":733
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":733
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -3053,26 +3053,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -3421,20 +3421,28 @@
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
 #ifndef __PYX_HAVE_RT_ImportType_proto
 #define __PYX_HAVE_RT_ImportType_proto
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#endif
 enum __Pyx_ImportType_CheckSize {
    __Pyx_ImportType_CheckSize_Error = 0,
    __Pyx_ImportType_CheckSize_Warn = 1,
    __Pyx_ImportType_CheckSize_Ignore = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
 #endif
 
 /* GetVTable.proto */
 static void* __Pyx_GetVtable(PyObject *dict);
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
@@ -5404,15 +5412,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle_SentenceSegmenter, (type(self), 0x80392e3, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_SentenceSegmenter__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
-  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
+  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
   __pyx_t_1 = __pyx_f_6edsnlp_9pipelines_4core_9sentences_9sentences___pyx_unpickle_SentenceSegmenter__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_SentenceSegmenter, (type(self), 0x80392e3, state)
@@ -5650,15 +5658,15 @@
     /* "(tree fragment)":9
  *     __pyx_result = SentenceSegmenter.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_SentenceSegmenter__set_state(<SentenceSegmenter> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_SentenceSegmenter__set_state(SentenceSegmenter __pyx_result, tuple __pyx_state):
  */
-    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
+    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
     __pyx_t_4 = __pyx_f_6edsnlp_9pipelines_4core_9sentences_9sentences___pyx_unpickle_SentenceSegmenter__set_state(((struct __pyx_obj_6edsnlp_9pipelines_4core_9sentences_9sentences_SentenceSegmenter *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x80392e3, 0x56d5ac8, 0x70dfbb1) = (capitalized_shapes_hash, endline_hash, excluded_hash, ignore_excluded, newline_hash, punct_chars_hash))" % __pyx_checksum)
  *     __pyx_result = SentenceSegmenter.__new__(__pyx_type)
@@ -5876,15 +5884,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":735
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -5893,29 +5901,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":736
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":736
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 736, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -5926,15 +5934,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":738
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -5943,29 +5951,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":739
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":739
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 739, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -5976,15 +5984,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":741
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -5993,29 +6001,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":742
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":742
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 742, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -6026,15 +6034,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":744
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -6043,29 +6051,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":745
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":745
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 745, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -6076,15 +6084,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":747
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -6093,29 +6101,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":748
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":748
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 748, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -6126,212 +6134,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":750
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":751
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":752
+    /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":752
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":754
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":754
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":929
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":930
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":931
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":931
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":933
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":934
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":935
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":936
+    /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":936
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":937
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":937
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":941
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -6347,15 +6355,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":942
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -6363,53 +6371,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":943
+      /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":943
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 943, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":944
+    /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 944, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":945
+      /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 945, __pyx_L5_except_error)
@@ -6417,30 +6425,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 945, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":942
+    /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -6455,15 +6463,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":947
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6479,15 +6487,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":948
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -6495,53 +6503,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":949
+      /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":949
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 949, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":950
+    /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 950, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":951
+      /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 951, __pyx_L5_except_error)
@@ -6549,30 +6557,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 951, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":948
+    /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6587,15 +6595,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":953
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6611,15 +6619,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":954
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -6627,53 +6635,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":955
+      /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":955
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 955, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":956
+    /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":956
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 956, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":957
+      /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":957
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 957, __pyx_L5_except_error)
@@ -6681,30 +6689,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 957, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":954
+    /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6719,176 +6727,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":967
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":967
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":979
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":979
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":967
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":967
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":982
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":982
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":994
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":994
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":982
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":982
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":997
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":997
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":1004
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":1004
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":997
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":997
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":1007
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":1007
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":1011
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":1011
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":1007
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":1007
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":1014
+/* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":1014
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":1018
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":1018
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":1014
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":1014
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -9262,15 +9270,15 @@
   /* "View.MemoryView":141
  *         if not isinstance(format, bytes):
  *             format = format.encode('ASCII')
  *         self._format = format  # keep a reference to the byte string             # <<<<<<<<<<<<<<
  *         self.format = self._format
  * 
  */
-  if (!(likely(PyBytes_CheckExact(__pyx_v_format))||((__pyx_v_format) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_v_format)->tp_name), 0))) __PYX_ERR(1, 141, __pyx_L1_error)
+  if (!(likely(PyBytes_CheckExact(__pyx_v_format))||((__pyx_v_format) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_v_format)->tp_name), 0))) __PYX_ERR(1, 141, __pyx_L1_error)
   __pyx_t_3 = __pyx_v_format;
   __Pyx_INCREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_3);
   __Pyx_GOTREF(__pyx_v_self->_format);
   __Pyx_DECREF(__pyx_v_self->_format);
   __pyx_v_self->_format = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
@@ -11240,15 +11248,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle_Enum, (type(self), 0xb068931, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_Enum__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
-  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
+  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
   __pyx_t_1 = __pyx_unpickle_Enum__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_Enum, (type(self), 0xb068931, state)
@@ -13543,15 +13551,15 @@
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_6, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 512, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(1, 512, __pyx_L1_error)
+    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(1, 512, __pyx_L1_error)
     __pyx_v_bytesvalue = ((PyObject*)__pyx_t_4);
     __pyx_t_4 = 0;
 
     /* "View.MemoryView":511
  *         cdef Py_ssize_t i
  * 
  *         if isinstance(value, tuple):             # <<<<<<<<<<<<<<
@@ -13616,15 +13624,15 @@
       PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_v_value);
       __pyx_t_1 = 0;
       __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_8, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 514, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     }
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(1, 514, __pyx_L1_error)
+    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(1, 514, __pyx_L1_error)
     __pyx_v_bytesvalue = ((PyObject*)__pyx_t_4);
     __pyx_t_4 = 0;
   }
   __pyx_L3:;
 
   /* "View.MemoryView":516
  *             bytesvalue = struct.pack(self.view.format, value)
@@ -21819,15 +21827,15 @@
     /* "(tree fragment)":9
  *     __pyx_result = Enum.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_Enum__set_state(<Enum> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_Enum__set_state(Enum __pyx_result, tuple __pyx_state):
  */
-    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
+    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
     __pyx_t_4 = __pyx_unpickle_Enum__set_state(((struct __pyx_MemviewEnum_obj *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))" % __pyx_checksum)
  *     __pyx_result = Enum.__new__(__pyx_type)
@@ -23051,26 +23059,26 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x80392e3, 0x56d5ac8, 0x70dfbb1) = (capitalized_shapes_hash, endline_hash, excluded_hash, ignore_excluded, newline_hash, punct_chars_hash))" % __pyx_checksum)
  */
   __pyx_tuple__4 = PyTuple_Pack(3, __pyx_int_134451939, __pyx_int_91052744, __pyx_int_118356913); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":945
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(2, 945, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
 
-  /* "../../../../../tmp/build-env-e_0tlxsv/lib/python3.10/site-packages/numpy/__init__.pxd":951
+  /* "../../../../../tmp/build-env-05nh97he/lib/python3.10/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(2, 951, __pyx_L1_error)
@@ -23350,15 +23358,15 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_91052744 = PyInt_FromLong(91052744L); if (unlikely(!__pyx_int_91052744)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_112105877 = PyInt_FromLong(112105877L); if (unlikely(!__pyx_int_112105877)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_118356913 = PyInt_FromLong(118356913L); if (unlikely(!__pyx_int_118356913)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_134451939 = PyInt_FromLong(134451939L); if (unlikely(!__pyx_int_134451939)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_136983863 = PyInt_FromLong(136983863L); if (unlikely(!__pyx_int_136983863)) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -23490,112 +23498,139 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule("cymem.cymem"); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5cymem_5cymem_PyMalloc = __Pyx_ImportType(__pyx_t_1, "cymem.cymem", "PyMalloc", sizeof(struct __pyx_obj_5cymem_5cymem_PyMalloc), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5cymem_5cymem_PyMalloc = __Pyx_ImportType(__pyx_t_1, "cymem.cymem", "PyMalloc", sizeof(struct __pyx_obj_5cymem_5cymem_PyMalloc), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_5cymem_5cymem_PyMalloc),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5cymem_5cymem_PyMalloc) __PYX_ERR(5, 4, __pyx_L1_error)
   __pyx_vtabptr_5cymem_5cymem_PyMalloc = (struct __pyx_vtabstruct_5cymem_5cymem_PyMalloc*)__Pyx_GetVtable(__pyx_ptype_5cymem_5cymem_PyMalloc->tp_dict); if (unlikely(!__pyx_vtabptr_5cymem_5cymem_PyMalloc)) __PYX_ERR(5, 4, __pyx_L1_error)
-  __pyx_ptype_5cymem_5cymem_PyFree = __Pyx_ImportType(__pyx_t_1, "cymem.cymem", "PyFree", sizeof(struct __pyx_obj_5cymem_5cymem_PyFree), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5cymem_5cymem_PyFree = __Pyx_ImportType(__pyx_t_1, "cymem.cymem", "PyFree", sizeof(struct __pyx_obj_5cymem_5cymem_PyFree), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_5cymem_5cymem_PyFree),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5cymem_5cymem_PyFree) __PYX_ERR(5, 10, __pyx_L1_error)
   __pyx_vtabptr_5cymem_5cymem_PyFree = (struct __pyx_vtabstruct_5cymem_5cymem_PyFree*)__Pyx_GetVtable(__pyx_ptype_5cymem_5cymem_PyFree->tp_dict); if (unlikely(!__pyx_vtabptr_5cymem_5cymem_PyFree)) __PYX_ERR(5, 10, __pyx_L1_error)
-  __pyx_ptype_5cymem_5cymem_Pool = __Pyx_ImportType(__pyx_t_1, "cymem.cymem", "Pool", sizeof(struct __pyx_obj_5cymem_5cymem_Pool), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5cymem_5cymem_Pool = __Pyx_ImportType(__pyx_t_1, "cymem.cymem", "Pool", sizeof(struct __pyx_obj_5cymem_5cymem_Pool), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_5cymem_5cymem_Pool),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5cymem_5cymem_Pool) __PYX_ERR(5, 16, __pyx_L1_error)
   __pyx_vtabptr_5cymem_5cymem_Pool = (struct __pyx_vtabstruct_5cymem_5cymem_Pool*)__Pyx_GetVtable(__pyx_ptype_5cymem_5cymem_Pool->tp_dict); if (unlikely(!__pyx_vtabptr_5cymem_5cymem_Pool)) __PYX_ERR(5, 16, __pyx_L1_error)
-  __pyx_ptype_5cymem_5cymem_Address = __Pyx_ImportType(__pyx_t_1, "cymem.cymem", "Address", sizeof(struct __pyx_obj_5cymem_5cymem_Address), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5cymem_5cymem_Address = __Pyx_ImportType(__pyx_t_1, "cymem.cymem", "Address", sizeof(struct __pyx_obj_5cymem_5cymem_Address), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_5cymem_5cymem_Address),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5cymem_5cymem_Address) __PYX_ERR(5, 28, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(6, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 200, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT(PyArray_Descr),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 200, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 223, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayMultiIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 227, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 239, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 771, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 773, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 775, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 777, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 779, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 781, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 783, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 785, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 787, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 789, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT(PyUFuncObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 827, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("preshed.maps"); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 45, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7preshed_4maps_PreshMap = __Pyx_ImportType(__pyx_t_1, "preshed.maps", "PreshMap", sizeof(struct __pyx_obj_7preshed_4maps_PreshMap), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_7preshed_4maps_PreshMap = __Pyx_ImportType(__pyx_t_1, "preshed.maps", "PreshMap", sizeof(struct __pyx_obj_7preshed_4maps_PreshMap), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_7preshed_4maps_PreshMap),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7preshed_4maps_PreshMap) __PYX_ERR(7, 45, __pyx_L1_error)
   __pyx_vtabptr_7preshed_4maps_PreshMap = (struct __pyx_vtabstruct_7preshed_4maps_PreshMap*)__Pyx_GetVtable(__pyx_ptype_7preshed_4maps_PreshMap->tp_dict); if (unlikely(!__pyx_vtabptr_7preshed_4maps_PreshMap)) __PYX_ERR(7, 45, __pyx_L1_error)
-  __pyx_ptype_7preshed_4maps_PreshMapArray = __Pyx_ImportType(__pyx_t_1, "preshed.maps", "PreshMapArray", sizeof(struct __pyx_obj_7preshed_4maps_PreshMapArray), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_7preshed_4maps_PreshMapArray = __Pyx_ImportType(__pyx_t_1, "preshed.maps", "PreshMapArray", sizeof(struct __pyx_obj_7preshed_4maps_PreshMapArray), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_7preshed_4maps_PreshMapArray),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7preshed_4maps_PreshMapArray) __PYX_ERR(7, 53, __pyx_L1_error)
   __pyx_vtabptr_7preshed_4maps_PreshMapArray = (struct __pyx_vtabstruct_7preshed_4maps_PreshMapArray*)__Pyx_GetVtable(__pyx_ptype_7preshed_4maps_PreshMapArray->tp_dict); if (unlikely(!__pyx_vtabptr_7preshed_4maps_PreshMapArray)) __PYX_ERR(7, 53, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("spacy.strings"); if (unlikely(!__pyx_t_1)) __PYX_ERR(8, 22, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5spacy_7strings_StringStore = __Pyx_ImportType(__pyx_t_1, "spacy.strings", "StringStore", sizeof(struct __pyx_obj_5spacy_7strings_StringStore), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5spacy_7strings_StringStore = __Pyx_ImportType(__pyx_t_1, "spacy.strings", "StringStore", sizeof(struct __pyx_obj_5spacy_7strings_StringStore), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_5spacy_7strings_StringStore),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5spacy_7strings_StringStore) __PYX_ERR(8, 22, __pyx_L1_error)
   __pyx_vtabptr_5spacy_7strings_StringStore = (struct __pyx_vtabstruct_5spacy_7strings_StringStore*)__Pyx_GetVtable(__pyx_ptype_5spacy_7strings_StringStore->tp_dict); if (unlikely(!__pyx_vtabptr_5spacy_7strings_StringStore)) __PYX_ERR(8, 22, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("spacy.morphology"); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 11, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5spacy_10morphology_Morphology = __Pyx_ImportType(__pyx_t_1, "spacy.morphology", "Morphology", sizeof(struct __pyx_obj_5spacy_10morphology_Morphology), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5spacy_10morphology_Morphology = __Pyx_ImportType(__pyx_t_1, "spacy.morphology", "Morphology", sizeof(struct __pyx_obj_5spacy_10morphology_Morphology), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_5spacy_10morphology_Morphology),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5spacy_10morphology_Morphology) __PYX_ERR(9, 11, __pyx_L1_error)
   __pyx_vtabptr_5spacy_10morphology_Morphology = (struct __pyx_vtabstruct_5spacy_10morphology_Morphology*)__Pyx_GetVtable(__pyx_ptype_5spacy_10morphology_Morphology->tp_dict); if (unlikely(!__pyx_vtabptr_5spacy_10morphology_Morphology)) __PYX_ERR(9, 11, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("spacy.vocab"); if (unlikely(!__pyx_t_1)) __PYX_ERR(10, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5spacy_5vocab_Vocab = __Pyx_ImportType(__pyx_t_1, "spacy.vocab", "Vocab", sizeof(struct __pyx_obj_5spacy_5vocab_Vocab), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5spacy_5vocab_Vocab = __Pyx_ImportType(__pyx_t_1, "spacy.vocab", "Vocab", sizeof(struct __pyx_obj_5spacy_5vocab_Vocab), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_5spacy_5vocab_Vocab),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5spacy_5vocab_Vocab) __PYX_ERR(10, 26, __pyx_L1_error)
   __pyx_vtabptr_5spacy_5vocab_Vocab = (struct __pyx_vtabstruct_5spacy_5vocab_Vocab*)__Pyx_GetVtable(__pyx_ptype_5spacy_5vocab_Vocab->tp_dict); if (unlikely(!__pyx_vtabptr_5spacy_5vocab_Vocab)) __PYX_ERR(10, 26, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("spacy.tokens.doc"); if (unlikely(!__pyx_t_1)) __PYX_ERR(11, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5spacy_6tokens_3doc_Doc = __Pyx_ImportType(__pyx_t_1, "spacy.tokens.doc", "Doc", sizeof(struct __pyx_obj_5spacy_6tokens_3doc_Doc), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5spacy_6tokens_3doc_Doc = __Pyx_ImportType(__pyx_t_1, "spacy.tokens.doc", "Doc", sizeof(struct __pyx_obj_5spacy_6tokens_3doc_Doc), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_5spacy_6tokens_3doc_Doc),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5spacy_6tokens_3doc_Doc) __PYX_ERR(11, 37, __pyx_L1_error)
   __pyx_vtabptr_5spacy_6tokens_3doc_Doc = (struct __pyx_vtabstruct_5spacy_6tokens_3doc_Doc*)__Pyx_GetVtable(__pyx_ptype_5spacy_6tokens_3doc_Doc->tp_dict); if (unlikely(!__pyx_vtabptr_5spacy_6tokens_3doc_Doc)) __PYX_ERR(11, 37, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("spacy.lexeme"); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5spacy_6lexeme_Lexeme = __Pyx_ImportType(__pyx_t_1, "spacy.lexeme", "Lexeme", sizeof(struct __pyx_obj_5spacy_6lexeme_Lexeme), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5spacy_6lexeme_Lexeme = __Pyx_ImportType(__pyx_t_1, "spacy.lexeme", "Lexeme", sizeof(struct __pyx_obj_5spacy_6lexeme_Lexeme), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_5spacy_6lexeme_Lexeme),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5spacy_6lexeme_Lexeme) __PYX_ERR(3, 15, __pyx_L1_error)
   __pyx_vtabptr_5spacy_6lexeme_Lexeme = (struct __pyx_vtabstruct_5spacy_6lexeme_Lexeme*)__Pyx_GetVtable(__pyx_ptype_5spacy_6lexeme_Lexeme->tp_dict); if (unlikely(!__pyx_vtabptr_5spacy_6lexeme_Lexeme)) __PYX_ERR(3, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("spacy.tokens.token"); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 14, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5spacy_6tokens_5token_Token = __Pyx_ImportType(__pyx_t_1, "spacy.tokens.token", "Token", sizeof(struct __pyx_obj_5spacy_6tokens_5token_Token), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5spacy_6tokens_5token_Token = __Pyx_ImportType(__pyx_t_1, "spacy.tokens.token", "Token", sizeof(struct __pyx_obj_5spacy_6tokens_5token_Token), __PYX_GET_STRUCT_ALIGNMENT(struct __pyx_obj_5spacy_6tokens_5token_Token),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5spacy_6tokens_5token_Token) __PYX_ERR(4, 14, __pyx_L1_error)
   __pyx_vtabptr_5spacy_6tokens_5token_Token = (struct __pyx_vtabstruct_5spacy_6tokens_5token_Token*)__Pyx_GetVtable(__pyx_ptype_5spacy_6tokens_5token_Token->tp_dict); if (unlikely(!__pyx_vtabptr_5spacy_6tokens_5token_Token)) __PYX_ERR(4, 14, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
@@ -23816,15 +23851,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_edsnlp__pipelines__core__sentences__sentences) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name_2, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -24462,15 +24497,15 @@
 #endif
     return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
 }
 
 /* ObjectGetItem */
 #if CYTHON_USE_TYPE_SLOTS
 static PyObject *__Pyx_PyObject_GetIndex(PyObject *obj, PyObject* index) {
-    PyObject *runerr;
+    PyObject *runerr = NULL;
     Py_ssize_t key_value;
     PySequenceMethods *m = Py_TYPE(obj)->tp_as_sequence;
     if (unlikely(!(m && m->sq_item))) {
         PyErr_Format(PyExc_TypeError, "'%.200s' object is not subscriptable", Py_TYPE(obj)->tp_name);
         return NULL;
     }
     key_value = __Pyx_PyIndex_AsSsize_t(index);
@@ -25032,28 +25067,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -25893,44 +25928,62 @@
     return ret;
 }
 
 /* TypeImport */
 #ifndef __PYX_HAVE_RT_ImportType
 #define __PYX_HAVE_RT_ImportType
 static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
     if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
@@ -25972,15 +26025,15 @@
 bad:
     Py_XDECREF(ob);
     return NULL;
 }
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
@@ -26350,15 +26403,15 @@
                         z = __Pyx_c_prod_float(a, a);
                         return __Pyx_c_prod_float(z, z);
                 }
             }
             if (a.imag == 0) {
                 if (a.real == 0) {
                     return a;
-                } else if (b.imag == 0) {
+                } else if ((b.imag == 0) && (a.real >= 0)) {
                     z.real = powf(a.real, b.real);
                     z.imag = 0;
                     return z;
                 } else if (a.real > 0) {
                     r = a.real;
                     theta = 0;
                 } else {
@@ -26504,15 +26557,15 @@
                         z = __Pyx_c_prod_double(a, a);
                         return __Pyx_c_prod_double(z, z);
                 }
             }
             if (a.imag == 0) {
                 if (a.real == 0) {
                     return a;
-                } else if (b.imag == 0) {
+                } else if ((b.imag == 0) && (a.real >= 0)) {
                     z.real = pow(a.real, b.real);
                     z.imag = 0;
                     return z;
                 } else if (a.real > 0) {
                     r = a.real;
                     theta = 0;
                 } else {
```

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/core/sentences/terms.py` & `edsnlp-0.8.0/edsnlp/pipelines/core/sentences/terms.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/core/terminology/terminology.py` & `edsnlp-0.8.0/edsnlp/pipelines/core/terminology/terminology.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,14 +38,16 @@
         A dictionary of regular expressions.
     attr : str
         The default attribute to use for matching.
         Can be overridden using the `terms` and `regex` configurations.
     ignore_excluded : bool
         Whether to skip excluded tokens (requires an upstream
         pipeline to mark excluded tokens).
+    ignore_space_tokens: bool
+        Whether to skip space tokens during matching.
     term_matcher: TerminologyTermMatcher
         The matcher to use for matching phrases ?
         One of (exact, simstring)
     term_matcher_config: Dict[str,Any]
         Parameters of the matcher class
     """
 
@@ -53,14 +55,15 @@
         self,
         nlp: Language,
         label: str,
         terms: Optional[Patterns],
         regex: Optional[Patterns],
         attr: str,
         ignore_excluded: bool,
+        ignore_space_tokens: bool = False,
         term_matcher: TerminologyTermMatcher = TerminologyTermMatcher.exact,
         term_matcher_config=None,
     ):
 
         self.nlp = nlp
 
         self.label = label
@@ -68,35 +71,38 @@
         self.attr = attr
 
         if term_matcher == TerminologyTermMatcher.exact:
             self.phrase_matcher = EDSPhraseMatcher(
                 self.nlp.vocab,
                 attr=attr,
                 ignore_excluded=ignore_excluded,
+                ignore_space_tokens=ignore_space_tokens,
                 **(term_matcher_config or {}),
             )
         elif term_matcher == TerminologyTermMatcher.simstring:
             self.phrase_matcher = SimstringMatcher(
                 vocab=self.nlp.vocab,
                 attr=attr,
                 ignore_excluded=ignore_excluded,
+                ignore_space_tokens=ignore_space_tokens,
                 **(term_matcher_config or {}),
             )
         else:
             raise ValueError(
                 f"Algorithm {repr(term_matcher)} does not belong to"
                 f" known matchers [exact, simstring]."
             )
 
         self.regex_matcher = RegexMatcher(
             attr=attr,
             ignore_excluded=ignore_excluded,
+            ignore_space_tokens=ignore_space_tokens,
         )
 
-        self.phrase_matcher.build_patterns(nlp=nlp, terms=terms)
+        self.phrase_matcher.build_patterns(nlp=nlp, terms=terms, progress=True)
         self.regex_matcher.build_patterns(regex=regex)
 
         self.set_extensions()
 
     def set_extensions(self) -> None:
         super().set_extensions()
         if not Span.has_extension(self.label):
```

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/factories.py` & `edsnlp-0.8.0/edsnlp/pipelines/factories.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,25 +11,57 @@
 from .core.sentences.factory import create_component as sentences
 from .core.terminology.factory import create_component as terminology
 from .misc.consultation_dates.factory import create_component as consultation_dates
 from .misc.dates.factory import create_component as dates
 from .misc.measurements.factory import create_component as measurements
 from .misc.reason.factory import create_component as reason
 from .misc.sections.factory import create_component as sections
+from .misc.tables.factory import create_component as tables
 from .ner.adicap.factory import create_component as adicap
+from .ner.behaviors.alcohol.factory import create_component as alcohol
+from .ner.behaviors.tobacco.factory import create_component as tobacco
 from .ner.cim10.factory import create_component as cim10
 from .ner.covid.factory import create_component as covid
+from .ner.disorders.AIDS.factory import create_component as AIDS
+from .ner.disorders.cerebrovascular_accident.factory import (
+    create_component as cerebrovascular_accident,
+)
+from .ner.disorders.CKD.factory import create_component as CKD
+from .ner.disorders.congestive_heart_failure.factory import (
+    create_component as congestive_heart_failure,
+)
+from .ner.disorders.connective_tissue_disease.factory import (
+    create_component as connective_tissue_disease,
+)
+from .ner.disorders.COPD.factory import create_component as COPD
+from .ner.disorders.dementia.factory import create_component as dementia
+from .ner.disorders.diabetes.factory import create_component as diabetes
+from .ner.disorders.hemiplegia.factory import create_component as hemiplegia
+from .ner.disorders.leukemia.factory import create_component as leukemia
+from .ner.disorders.liver_disease.factory import create_component as liver_disease
+from .ner.disorders.lymphoma.factory import create_component as lymphoma
+from .ner.disorders.myocardial_infarction.factory import (
+    create_component as myocardial_infarction,
+)
+from .ner.disorders.peptic_ulcer_disease.factory import (
+    create_component as peptic_ulcer_disease,
+)
+from .ner.disorders.peripheral_vascular_disease.factory import (
+    create_component as peripheral_vascular_disease,
+)
+from .ner.disorders.solid_tumor.factory import create_component as solid_tumor
 from .ner.drugs.factory import create_component as drugs
 from .ner.scores.charlson.factory import create_component as charlson
 from .ner.scores.emergency.ccmu.factory import create_component as ccmu
 from .ner.scores.emergency.gemsa.factory import create_component as gemsa
 from .ner.scores.emergency.priority.factory import create_component as priority
 from .ner.scores.factory import create_component as score
 from .ner.scores.sofa.factory import create_component as sofa
 from .ner.scores.tnm.factory import create_component as tnm
 from .ner.umls.factory import create_component as umls
 from .qualifiers.family.factory import create_component as family
 from .qualifiers.history.factory import create_component as history
 from .qualifiers.hypothesis.factory import create_component as hypothesis
 from .qualifiers.negation.factory import create_component as negation
 from .qualifiers.reported_speech.factory import create_component as rspeech
-from .trainable.nested_ner import create_component as nested_ner
+from .trainable.nested_ner.factory import create_component as nested_ner
+from .trainable.span_qualifier.factory import create_component as span_qualifier
```

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/misc/consultation_dates/consultation_dates.py` & `edsnlp-0.8.0/edsnlp/pipelines/misc/consultation_dates/consultation_dates.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/misc/consultation_dates/factory.py` & `edsnlp-0.8.0/edsnlp/pipelines/misc/consultation_dates/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/misc/consultation_dates/patterns.py` & `edsnlp-0.8.0/edsnlp/pipelines/misc/consultation_dates/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/misc/dates/dates.py` & `edsnlp-0.8.0/edsnlp/pipelines/misc/dates/dates.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """`eds.dates` pipeline."""
 
 from itertools import chain
-from typing import Dict, List, Optional, Tuple, Union
+from typing import Dict, Iterable, List, Optional, Tuple, Union
 
 from loguru import logger
 from spacy.language import Language
 from spacy.tokens import Doc, Span
 
 from edsnlp.matchers.regex import RegexMatcher
 from edsnlp.pipelines.base import BaseComponent
@@ -36,15 +36,15 @@
         List of regular expressions for relative dates
         (eg `hier`, `la semaine prochaine`).
     duration : Union[List[str], str]
         List of regular expressions for durations
         (eg `pendant trois mois`).
     false_positive : Union[List[str], str]
         List of regular expressions for false positive (eg phone numbers, etc).
-    on_ents_only : Union[bool, str, List[str]]
+    on_ents_only : Union[bool, str, Iterable[str]]
         Wether to look on dates in the whole document or in specific sentences:
 
         - If `True`: Only look in the sentences of each entity in doc.ents
         - If False: Look in the whole document
         - If given a string `key` or list of string: Only look in the sentences of
           each entity in `#!python doc.spans[key]`
     detect_periods : bool
@@ -59,15 +59,15 @@
     def __init__(
         self,
         nlp: Language,
         absolute: Optional[List[str]],
         relative: Optional[List[str]],
         duration: Optional[List[str]],
         false_positive: Optional[List[str]],
-        on_ents_only: Union[bool, List[str]],
+        on_ents_only: Union[bool, str, Iterable[str]],
         detect_periods: bool,
         detect_time: bool,
         as_ents: bool,
         attr: str,
     ):
 
         self.nlp = nlp
@@ -137,26 +137,16 @@
         Returns
         -------
         dates:
             list of date spans
         """
 
         if self.on_ents_only:
-
-            if type(self.on_ents_only) == bool:
-                ents = doc.ents
-            else:
-                if type(self.on_ents_only) == str:
-                    self.on_ents_only = [self.on_ents_only]
-                ents = []
-                for key in self.on_ents_only:
-                    ents.extend(list(doc.spans[key]))
-
             dates = []
-            for sent in set([ent.sent for ent in ents]):
+            for sent in set([ent.sent for ent in self.get_spans(doc)]):
                 dates = chain(
                     dates,
                     self.regex_matcher(
                         sent,
                         as_spans=True,
                         return_groupdict=True,
                     ),
```

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/misc/dates/factory.py` & `edsnlp-0.8.0/edsnlp/pipelines/misc/dates/factory.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Optional, Union
+from typing import List, Optional, Set, Union
 
 from spacy.language import Language
 
 from edsnlp.utils.deprecation import deprecated_factory
 
 from . import Dates
 
@@ -26,15 +26,15 @@
 def create_component(
     nlp: Language,
     name: str,
     absolute: Optional[List[str]],
     relative: Optional[List[str]],
     duration: Optional[List[str]],
     false_positive: Optional[List[str]],
-    on_ents_only: Union[bool, List[str]],
+    on_ents_only: Union[bool, str, List[str], Set[str]],
     detect_periods: bool,
     detect_time: bool,
     as_ents: bool,
     attr: str,
 ):
     return Dates(
         nlp,
```

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/misc/dates/models.py` & `edsnlp-0.8.0/edsnlp/pipelines/misc/dates/models.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/misc/dates/patterns/absolute.py` & `edsnlp-0.8.0/edsnlp/pipelines/misc/dates/patterns/absolute.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/misc/dates/patterns/atomic/days.py` & `edsnlp-0.8.0/edsnlp/pipelines/misc/dates/patterns/atomic/days.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/misc/dates/patterns/atomic/delimiters.py` & `edsnlp-0.8.0/edsnlp/pipelines/misc/dates/patterns/atomic/delimiters.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/misc/dates/patterns/atomic/directions.py` & `edsnlp-0.8.0/edsnlp/pipelines/misc/dates/patterns/atomic/directions.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/misc/dates/patterns/atomic/months.py` & `edsnlp-0.8.0/edsnlp/pipelines/misc/dates/patterns/atomic/months.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/misc/dates/patterns/atomic/numbers.py` & `edsnlp-0.8.0/edsnlp/pipelines/misc/dates/patterns/atomic/numbers.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/misc/dates/patterns/atomic/time.py` & `edsnlp-0.8.0/edsnlp/pipelines/misc/dates/patterns/atomic/time.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/misc/dates/patterns/relative.py` & `edsnlp-0.8.0/edsnlp/pipelines/misc/dates/patterns/relative.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/misc/measurements/factory.py` & `edsnlp-0.8.0/edsnlp/pipelines/misc/measurements/factory.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,62 @@
-from typing import Dict, List, Optional, Union
+from typing import Dict, List, Optional, Tuple, Union
 
 from spacy.language import Language
 
 import edsnlp.pipelines.misc.measurements.patterns as patterns
 from edsnlp.pipelines.misc.measurements.measurements import (
     MeasureConfig,
     MeasurementsMatcher,
+    MergeStrategy,
     UnitConfig,
 )
 from edsnlp.utils.deprecation import deprecated_factory
 
 DEFAULT_CONFIG = dict(
     attr="NORM",
+    measurements=None,
     ignore_excluded=True,
     units_config=patterns.units_config,
     number_terms=patterns.number_terms,
     unit_divisors=patterns.unit_divisors,
-    measurements=None,
     stopwords=patterns.stopwords,
+    compose_units=True,
+    extract_ranges=False,
+    range_patterns=patterns.range_patterns,
+    as_ents=False,
+    merge_mode=MergeStrategy.union,
 )
 
 
 @Language.factory("eds.measurements", default_config=DEFAULT_CONFIG)
 @deprecated_factory("eds.measures", "eds.measurements", default_config=DEFAULT_CONFIG)
 def create_component(
     nlp: Language,
     name: str,
     measurements: Optional[Union[Dict[str, MeasureConfig], List[str]]],
     units_config: Dict[str, UnitConfig],
     number_terms: Dict[str, List[str]],
     stopwords: List[str],
     unit_divisors: List[str],
     ignore_excluded: bool,
+    compose_units: bool,
     attr: str,
+    extract_ranges: bool,
+    range_patterns: List[Tuple[Optional[str], Optional[str]]],
+    as_ents: bool,
+    merge_mode: MergeStrategy,
 ):
     return MeasurementsMatcher(
         nlp,
+        measurements=measurements,
         units_config=units_config,
         number_terms=number_terms,
-        unit_divisors=unit_divisors,
-        measurements=measurements,
         stopwords=stopwords,
-        attr=attr,
+        unit_divisors=unit_divisors,
         ignore_excluded=ignore_excluded,
+        compose_units=compose_units,
+        attr=attr,
+        extract_ranges=extract_ranges,
+        range_patterns=range_patterns,
+        as_ents=as_ents,
+        merge_mode=merge_mode,
     )
```

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/misc/measurements/measurements.py` & `edsnlp-0.8.0/edsnlp/pipelines/misc/measurements/measurements.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,43 +1,61 @@
 import abc
 import re
 import unicodedata
 from collections import defaultdict
+from enum import Enum
 from functools import lru_cache
 from itertools import repeat
 from typing import Any, Dict, Iterable, List, Optional, Set, Tuple, Union
 
 import regex
 import spacy
 from spacy.tokens import Doc, Span
-from typing_extensions import TypedDict
+from typing_extensions import NotRequired, TypedDict
 
 from edsnlp.matchers.phrase import EDSPhraseMatcher
 from edsnlp.matchers.regex import RegexMatcher
-from edsnlp.pipelines.misc.measurements.patterns import common_measurements
-from edsnlp.utils.filter import filter_spans
+from edsnlp.matchers.utils import get_text
+from edsnlp.pipelines.misc.measurements import patterns
+from edsnlp.utils.collections import dedup
+from edsnlp.utils.filter import align_spans, filter_spans, get_span_group
 
 __all__ = ["MeasurementsMatcher"]
 
 
 AFTER_SNIPPET_LIMIT = 6
 BEFORE_SNIPPET_LIMIT = 10
 
 
+class MergeStrategy(str, Enum):
+    """
+    The strategy to use when merging measurements.
+    """
+
+    # Align the new measurement to existing spans
+    align = "align"
+
+    # Only extract measurements if they fall within an existing span
+    intersect = "intersect"
+
+    # Extract measurements regardless of whether they fall within an existing span
+    union = "union"
+
+
 class UnitConfig(TypedDict):
     dim: str
     degree: int
     scale: float
     terms: List[str]
     followed_by: Optional[str] = None
 
 
 class UnitlessRange(TypedDict):
-    min: int
-    max: int
+    min: NotRequired[int]
+    max: NotRequired[int]
     unit: str
 
 
 class UnitlessPatternConfig(TypedDict):
     terms: List[str]
     ranges: List[UnitlessRange]
 
@@ -46,40 +64,51 @@
     terms: List[str]
     ranges: List[UnitlessRange]
     name: str
 
 
 class MeasureConfig(TypedDict):
     unit: str
-    unitless_patterns: List[UnitlessPatternConfig]
+    unitless_patterns: NotRequired[List[UnitlessPatternConfig]]
+    name: NotRequired[str]
 
 
 class Measurement(abc.ABC):
     @abc.abstractmethod
+    def __len__(self) -> Iterable["SimpleMeasurement"]:
+        """
+        Number of items in the measure (only one for SimpleMeasurement)
+
+        Returns
+        -------
+        Iterable["SimpleMeasurement"]
+        """
+
+    @abc.abstractmethod
     def __iter__(self) -> Iterable["SimpleMeasurement"]:
         """
         Iter over items of the measure (only one for SimpleMeasurement)
 
         Returns
         -------
-        iterable : Iterable["SimpleMeasurement"]
+        Iterable["SimpleMeasurement"]
         """
 
     @abc.abstractmethod
     def __getitem__(self, item) -> "SimpleMeasurement":
         """
         Access items of the measure (only one for SimpleMeasurement)
 
         Parameters
         ----------
         item : int
 
         Returns
         -------
-        measure : SimpleMeasurement
+        SimpleMeasurement
         """
 
 
 class UnitRegistry:
     def __init__(self, config: Dict[str, UnitConfig]):
         self.config = {unicodedata.normalize("NFKC", k): v for k, v in config.items()}
         for unit, unit_config in list(self.config.items()):
@@ -88,20 +117,25 @@
                     "dim": unit_config["dim"],
                     "degree": -unit_config["degree"],
                     "scale": 1 / unit_config["scale"],
                 }
 
     @lru_cache(maxsize=-1)
     def parse_unit(self, unit: str) -> Tuple[str, float]:
-        degrees = defaultdict(lambda: 0)
+        degrees = defaultdict(lambda: [])
         scale = 1
         for part in regex.split("(?<!per)_", unit):
             unit_config = self.config[unicodedata.normalize("NFKC", part)]
-            degrees[unit_config["dim"]] += unit_config["degree"]
+            degrees[unit_config["dim"]].append(unit_config["degree"])
             scale *= unit_config["scale"]
+        degrees = {
+            k: sum(v) if len(set(v)) > 1 else v[0]
+            for k, v in degrees.items()
+            if sum(v) != 0
+        }
         return str(dict(sorted(degrees.items()))), scale
 
 
 class SimpleMeasurement(Measurement):
     def __init__(self, value, unit, registry):
         """
         The SimpleMeasurement class contains the value and unit
@@ -123,14 +157,17 @@
     def __getitem__(self, item: int):
         assert isinstance(item, int)
         return [self][item]
 
     def __str__(self):
         return f"{self.value} {self.unit}"
 
+    def __len__(self):
+        return 1
+
     def __repr__(self):
         return f"Measurement({self.value}, {repr(self.unit)})"
 
     def __eq__(self, other: Any):
         if isinstance(other, SimpleMeasurement):
             return self.convert_to(other.unit) == other.value
         return False
@@ -138,51 +175,129 @@
     def __add__(self, other: "SimpleMeasurement"):
         if other.unit == self.unit:
             return self.__class__(self.value + other.value, self.unit, self.registry)
         return self.__class__(
             self.value + other.convert_to(self.unit), self.unit, self.registry
         )
 
-    def __lt__(self, other: "SimpleMeasurement"):
-        return self.convert_to(other.unit) < other.value
+    def __lt__(self, other: Union["SimpleMeasurement", "RangeMeasurement"]):
+        return self.convert_to(other.unit) < min((part.value for part in other))
 
-    def __le__(self, other: "SimpleMeasurement"):
-        return self.convert_to(other.unit) <= other.value
+    def __le__(self, other: Union["SimpleMeasurement", "RangeMeasurement"]):
+        return self.convert_to(other.unit) <= min((part.value for part in other))
 
     def convert_to(self, other_unit):
         self_degrees, self_scale = self.registry.parse_unit(self.unit)
         other_degrees, other_scale = self.registry.parse_unit(other_unit)
 
         if self_degrees != other_degrees:
             raise AttributeError(
                 f"Units {self.unit} and {other_unit} are not homogenous"
             )
-        new_value = self.value * self_scale / other_scale
-        return new_value
+        ratio = self_scale / other_scale
+        if ratio != 1:
+            return self.value * ratio
+        return self.value
 
     def __getattr__(self, other_unit):
         return self.convert_to(other_unit)
 
     @classmethod
     def verify(cls, ent):
         return True
 
 
+class RangeMeasurement(Measurement):
+    def __init__(self, from_value, to_value, unit, registry):
+        super().__init__()
+        self.value = (from_value, to_value)
+        self.unit = unit
+        self.registry = registry
+
+    @classmethod
+    def from_measurements(cls, a, b):
+        a_value = a.value
+        b_value = b.convert_to(a.unit)
+        return RangeMeasurement(a_value, b_value, a.unit, a.registry)
+
+    def convert_to(self, other_unit):
+        self_degrees, self_scale = self.registry.parse_unit(self.unit)
+        other_degrees, other_scale = self.registry.parse_unit(other_unit)
+
+        if self_degrees != other_degrees:
+            raise AttributeError(
+                f"Units {self.unit} and {other_unit} are not homogenous"
+            )
+        ratio = self_scale / other_scale
+        if ratio == 1:
+            return self.value
+        from_value = self.value[0] * ratio
+        to_value = self.value[1] * ratio
+        return (from_value, to_value)
+
+    def __iter__(self):
+        yield self[0]
+        yield self[1]
+
+    def __len__(self):
+        return 2
+
+    def __lt__(self, other: Union[SimpleMeasurement, "RangeMeasurement"]):
+        return max(self.convert_to(other.unit)) < min((part.value for part in other))
+
+    def __le__(self, other: Union[SimpleMeasurement, "RangeMeasurement"]):
+        return max(self.convert_to(other.unit)) <= max((part.value for part in other))
+
+    def __getattr__(self, other_unit):
+        return self.convert_to(other_unit)
+
+    def __eq__(self, other: Any):
+        if isinstance(other, RangeMeasurement):
+            return self.convert_to(other.unit) == other.value
+        return False
+
+    def __str__(self):
+        return f"{self.value[0]}-{self.value[1]} {self.unit}"
+
+    def __repr__(self):
+        return f"RangeMeasurement({self.value}, {repr(self.unit)})"
+
+    def __getitem__(self, item: int):
+        assert isinstance(item, int)
+        return SimpleMeasurement(self.value[item], self.unit, self.registry)
+
+    @classmethod
+    def verify(cls, ent):
+        return True
+
+
 class MeasurementsMatcher:
     def __init__(
         self,
         nlp: spacy.Language,
-        measurements: Union[List[str], Tuple[str], Dict[str, MeasureConfig]],
-        units_config: Dict[str, UnitConfig],
-        number_terms: Dict[str, List[str]],
-        stopwords: List[str] = ("par", "sur", "de", "a", ":"),
-        unit_divisors: List[str] = ("par", "/"),
+        measurements: Optional[
+            Union[
+                List[Union[str, MeasureConfig]],
+                Dict[str, MeasureConfig],
+            ]
+        ] = None,
+        units_config: Dict[str, UnitConfig] = patterns.units_config,
+        number_terms: Dict[str, List[str]] = patterns.number_terms,
+        stopwords: List[str] = patterns.stopwords,
+        unit_divisors: List[str] = patterns.unit_divisors,
         name: str = "measurements",
         ignore_excluded: bool = True,
+        compose_units: bool = True,
         attr: str = "NORM",
+        extract_ranges: bool = False,
+        range_patterns: List[
+            Tuple[Optional[str], Optional[str]]
+        ] = patterns.range_patterns,  # noqa: E501
+        as_ents: bool = False,
+        merge_mode: MergeStrategy = MergeStrategy.union,
     ):
         """
         Matcher component to extract measurements.
         A measurements is most often composed of a number and a unit like
         > 1,26 cm
         The unit can also be positioned in place of the decimal dot/comma
         > 1 cm 26
@@ -194,15 +309,15 @@
         The recognized measurements are stored in the "measurements" SpanGroup.
         Each span has a `Measurement` object stored in the "value" extension attribute.
 
         Parameters
         ----------
         nlp : Language
             The SpaCy object.
-        measurements : Dict[str, MeasureConfig]
+        measurements : Optional[Union[List[Union[str, MeasureConfig]],Dict[str, MeasureConfig]]]
             A mapping from measure names to MeasureConfig
             Each measure's configuration has the following shape:
             {
                 "unit": str, # the unit of the measure (like "kg"),
                 "unitless_patterns": { # optional patterns to handle unitless cases
                     "terms": List[str], # list of preceding terms used to trigger the
                     measure
@@ -225,38 +340,69 @@
             and a number
         unit_divisors: List[str]
             A list of terms used to divide two units (like: m / s)
         attr : str
             Whether to match on the text ('TEXT') or on the normalized text ('NORM')
         ignore_excluded : bool
             Whether to exclude pollution patterns when matching in the text
-        """
+        compose_units: bool
+            Whether to compose units (like "m/s" or "m.s-1")
+        extract_ranges: bool
+            Whether to extract ranges (like "entre 1 et 2 cm")
+        range_patterns: List[Tuple[str, str]]
+            A list of "{FROM} xx {TO} yy" patterns to match range measurements
+        """  # noqa E501
 
         if measurements is None:
-            measurements = common_measurements
+            measurements = [
+                {**m, "name": k} for k, m in patterns.common_measurements.items()
+            ]
         elif isinstance(measurements, (list, tuple)):
-            measurements = {m: common_measurements[m] for m in measurements}
+            measurements = [
+                m
+                if isinstance(m, dict)
+                else {**patterns.common_measurements[m], "name": m}
+                for m in measurements
+            ]
+        elif isinstance(measurements, dict):
+            measurements = [{"name": k, **m} for k, m in measurements.items()]
 
         self.nlp = nlp
         self.name = name
         self.unit_registry = UnitRegistry(units_config)
-        self.regex_matcher = RegexMatcher(attr=attr, ignore_excluded=True)
-        self.term_matcher = EDSPhraseMatcher(nlp.vocab, attr=attr, ignore_excluded=True)
+        self.regex_matcher = RegexMatcher(
+            attr=attr,
+            ignore_excluded=True,
+        )
+        self.term_matcher = EDSPhraseMatcher(
+            nlp.vocab,
+            attr=attr,
+            ignore_excluded=ignore_excluded,
+            ignore_space_tokens=True,
+        )
         self.unitless_patterns: Dict[str, UnitlessPatternConfigWithName] = {}
         self.unit_part_label_hashes: Set[int] = set()
         self.unitless_label_hashes: Set[int] = set()
         self.unit_followers: Dict[str, str] = {}
         self.measure_names: Dict[str, str] = {}
+        self.as_ents = as_ents
+        self.compose_units = compose_units
+        self.extract_ranges = extract_ranges
+        self.range_patterns = range_patterns
+        self.merge_mode = merge_mode
 
         # NUMBER PATTERNS
+        one_plus = "[1-9][0-9]*"
         self.regex_matcher.add(
             "number",
             [
-                r"(?<![a-z-])\d+([ ]\d{3})*[ ]+(?:[,.][ ]+\d+)?",
-                r"(?<![a-z-])\d+([ ]\d{3})*(?:[,.]\d+)?",
+                rf"(?<![0-9][.,]?){one_plus}([ ]\d{{3}})*[ ]+(?:[,.][ ]+\d+)?",
+                rf"(?<![0-9][.,]?){one_plus}([ ]\d{{3}})*(?:[,.]\d+)?",
+                rf"(?<![0-9][.,]?){one_plus}([ ]/[ ]|/){one_plus}",
+                r"(?<![0-9][.,]?)00?",
             ],
         )
         self.number_label_hashes = {nlp.vocab.strings["number"]}
         for number, terms in number_terms.items():
             self.term_matcher.build_patterns(nlp, {number: terms})
             self.number_label_hashes.add(nlp.vocab.strings[number])
 
@@ -269,19 +415,21 @@
 
         self.unit_part_label_hashes.add(nlp.vocab.strings["per"])
         self.term_matcher.build_patterns(
             nlp,
             {
                 "per": unit_divisors,
                 "stopword": stopwords,
+                "unitless_stopword": [":"],
             },
         )
 
         # MEASURES
-        for name, measure_config in measurements.items():
+        for measure_config in measurements:
+            name = measure_config["name"]
             unit = measure_config["unit"]
             self.measure_names[self.unit_registry.parse_unit(unit)[0]] = name
             if "unitless_patterns" in measure_config:
                 for pattern in measure_config["unitless_patterns"]:
                     pattern_name = f"unitless_{len(self.unitless_patterns)}"
                     self.term_matcher.build_patterns(
                         nlp,
@@ -323,29 +471,38 @@
         last = None
         units = []
         current = []
         unit_label_hashes = set()
         for unit_part in filter_spans(term_matches):
             if unit_part.label not in self.unit_part_label_hashes:
                 continue
-            if last is not None and unit_part.start != last.end and len(current):
+            if last is not None and (
+                (
+                    unit_part.doc[last.end : unit_part.start].text.strip() != ""
+                    and len(current)
+                )
+                or (
+                    not self.compose_units
+                    and len(current)
+                    and current[-1].label_ != "per"
+                )
+            ):
                 doc = current[0].doc
                 # Last non "per" match: we don't want our units to be like `g_per`
                 end = next(
                     (i for i, e in list(enumerate(current))[::-1] if e.label_ != "per"),
                     None,
                 )
                 if end is not None:
                     unit = "_".join(part.label_ for part in current[: end + 1])
                     units.append(Span(doc, current[0].start, current[end].end, unit))
                     unit_label_hashes.add(units[-1].label)
                 current = []
                 last = None
-            if len(current) > 0 or unit_part.label_ != "per":
-                current.append(unit_part)
+            current.append(unit_part)
             last = unit_part
 
         end = next(
             (i for i, e in list(enumerate(current))[::-1] if e.label_ != "per"), None
         )
         if end is not None:
             doc = current[0].doc
@@ -354,51 +511,53 @@
             unit_label_hashes.add(units[-1].label)
 
         return units
 
     @classmethod
     def make_pseudo_sentence(
         cls,
-        doc: Doc,
+        doclike: Union[Doc, Span],
         matches: List[Tuple[Span, bool]],
         pseudo_mapping: Dict[int, str],
     ) -> Tuple[str, List[int]]:
         """
         Creates a pseudo sentence (one letter per entity)
         to extract higher order patterns
         Ex: the sentence
         "Il font {1}{,} {2} {et} {3} {cm} de long{.}" is transformed into "wn,n,nuw."
 
         Parameters
         ----------
-        doc: Doc
+        doclike: Union[Doc, Span]
+            The document or span to transform
         matches: List[(Span, bool)]
             List of tuple of span and whether the span represents a sentence end
         pseudo_mapping: Dict[int, str]
             A mapping from label to char in the pseudo sentence
 
         Returns
         -------
         (str, List[int])
             - the pseudo sentence
             - a list of offsets to convert match indices into pseudo sent char indices
         """
         pseudo = []
-        last = 0
+        snippet = doclike if isinstance(doclike, Span) else doclike[:]
+        last = snippet.start
         offsets = []
         for ent, is_sent_split in matches:
-            if ent.start != last:
+            if (
+                ent.start != last
+                and not doclike.doc[last : ent.start].text.strip() == ""
+            ):
                 pseudo.append("w")
             offsets.append(len(pseudo))
-            if is_sent_split:
-                pseudo.append(".")
-            else:
-                pseudo.append(pseudo_mapping.get(ent.label, "w"))
+            pseudo.append(pseudo_mapping.get(ent.label, "." if is_sent_split else "w"))
             last = ent.end
-        if len(doc) != last:
+        if snippet.end != last and doclike.doc[last : snippet.end].text.strip() == "":
             pseudo.append("w")
         pseudo = "".join(pseudo)
 
         return pseudo, offsets
 
     def get_matches(self, doc):
         """
@@ -431,53 +590,54 @@
             for term in term_matches
             if term.label not in self.unit_part_label_hashes
         ]
 
         # Filter out measurement-related spans that overlap already matched
         # entities (in doc.ents or doc.spans["dates"])
         # Note: we also include sentence ends tokens as 1-token spans in those matches
+        # Prevent from matching over ents that are not measurement related
+        ents = (e for e in doc.ents if e.label_ not in self.measure_names.values())
         spans__keep__is_sent_end = filter_spans(
             [
                 # Tuples (span, keep = is measurement related, is sentence end)
-                *zip(doc.spans.get("dates", ()), repeat(False), repeat(False)),
+                *zip(get_span_group(doc, "dates"), repeat(False), repeat(False)),
                 *zip(regex_matches, repeat(True), repeat(False)),
                 *zip(non_unit_terms, repeat(True), repeat(False)),
                 *zip(units, repeat(True), repeat(False)),
-                *zip(doc.ents, repeat(False), repeat(False)),
+                *zip(ents, repeat(False), repeat(False)),
                 *zip(sent_ends, repeat(True), repeat(True)),
-            ],
-            # filter entities to keep only the ...
-            sort_key=measurements_match_tuples_sort_key,
+            ]
         )
 
         # Remove non-measurement related spans (keep = False) and sort the matches
         matches_and_is_sentence_end: List[(Span, bool)] = sorted(
             [
                 (span, is_sent_end)
                 for span, keep, is_sent_end in spans__keep__is_sent_end
                 # and remove entities that are not relevant to this pipeline
                 if keep
             ]
         )
 
         return matches_and_is_sentence_end, unit_label_hashes
 
-    def extract_measurements(self, doc: Doc):
+    def extract_measurements(self, doclike: Doc):
         """
         Extracts measure entities from the document
 
         Parameters
         ----------
-        doc: Doc
+        doclike: Doc
 
         Returns
         -------
         List[Span]
         """
-        matches, unit_label_hashes = self.get_matches(doc)
+        doc = doclike.doc if isinstance(doclike, Span) else doclike
+        matches, unit_label_hashes = self.get_matches(doclike)
 
         # Make match slice function to query them
         def get_matches_after(i):
             anchor = matches[i][0]
             for j, (ent, is_sent_end) in enumerate(matches[i + 1 :]):
                 if not is_sent_end and ent.start > anchor.end + AFTER_SNIPPET_LIMIT:
                     return
@@ -490,41 +650,47 @@
                     return
                 yield i - j, ent
 
         # Make a pseudo sentence to query higher order patterns in the main loop
         # `offsets` is a mapping from matches indices (ie match n°i) to
         # char indices in the pseudo sentence
         pseudo, offsets = self.make_pseudo_sentence(
-            doc,
+            doclike,
             matches,
             {
                 self.nlp.vocab.strings["stopword"]: ",",
+                self.nlp.vocab.strings["unitless_stopword"]: ":",
                 self.nlp.vocab.strings["number"]: "n",
                 **{name: "u" for name in unit_label_hashes},
                 **{name: "n" for name in self.number_label_hashes},
             },
         )
 
         measurements = []
         matched_unit_indices = set()
+        matched_number_indices = set()
 
         # Iterate through the number matches
         for number_idx, (number, is_sent_split) in enumerate(matches):
             if not is_sent_split and number.label not in self.number_label_hashes:
                 continue
 
             # Detect the measure value
             try:
                 if number.label_ == "number":
-                    value = float(
-                        number.text.replace(" ", "").replace(",", ".").replace(" ", "")
+                    number_text = (
+                        number.text.replace(" ", "")
+                        .replace(",", ".")
+                        .replace(" ", "")
+                        .lstrip("0")
                     )
+                    value = eval(number_text or "0")
                 else:
-                    value = float(number.label_)
-            except ValueError:
+                    value = eval(number.label_)
+            except (ValueError, SyntaxError):
                 continue
 
             unit_idx = unit_text = unit_norm = None
 
             # Find the closest unit after the number
             try:
                 unit_idx, unit_text = next(
@@ -562,15 +728,15 @@
                     (unitless_idx, unitless_text) = next(
                         (j, e)
                         for j, e in get_matches_before(number_idx)
                         if e.label in self.unitless_label_hashes
                     )
                     unit_norm = None
                     if re.fullmatch(
-                        r"[,n]*",
+                        r"[,:n]*",
                         pseudo[offsets[unitless_idx] + 1 : offsets[number_idx]],
                     ):
                         unitless_pattern = self.unitless_patterns[unitless_text.label_]
                         unit_norm = next(
                             scope["unit"]
                             for scope in unitless_pattern["ranges"]
                             if ("min" not in scope or value >= scope["min"])
@@ -580,18 +746,28 @@
                     pass
 
             # Otherwise, skip this number
             if not unit_norm:
                 continue
 
             # Compute the final entity
-            if unit_text and unit_text.end == number.start:
-                ent = doc[unit_text.start : number.end]
-            elif unit_text and unit_text.start == number.end:
+            # TODO: handle this part better without .text.strip(), with cases for
+            #  stopwords, etc
+            if (
+                unit_text
+                and number.start <= unit_text.end
+                and doc[number.end : unit_text.start].text.strip() == ""
+            ):
                 ent = doc[number.start : unit_text.end]
+            elif (
+                unit_text
+                and unit_text.start <= number.end
+                and doc[unit_text.end : number.start].text.strip() == ""
+            ):
+                ent = doc[unit_text.start : number.end]
             else:
                 ent = number
 
             # Compute the dimensionality of the parsed unit
             try:
                 dims = self.unit_registry.parse_unit(unit_norm)[0]
             except KeyError:
@@ -605,16 +781,28 @@
             ent._.value = SimpleMeasurement(value, unit_norm, self.unit_registry)
             ent.label_ = self.measure_names[dims]
 
             measurements.append(ent)
 
             if unit_idx is not None:
                 matched_unit_indices.add(unit_idx)
+            if number_idx is not None:
+                matched_number_indices.add(number_idx)
 
-        return measurements
+        unmatched = []
+        for idx, (match, _) in enumerate(matches):
+            if (
+                match.label in unit_label_hashes
+                and idx not in matched_unit_indices
+                or match.label in self.number_label_hashes
+                and idx not in matched_number_indices
+            ):
+                unmatched.append(match)
+
+        return measurements, unmatched
 
     @classmethod
     def merge_adjacent_measurements(cls, measurements: List[Span]) -> List[Span]:
         """
         Aggregates extracted measurements together when they are adjacent to handle
         cases like
         - 1 meter 50 cm
@@ -641,40 +829,140 @@
                 except (AttributeError, TypeError):
                     merged.append(ent)
             else:
                 merged.append(ent)
 
         return merged
 
+    def merge_measurements_in_ranges(self, measurements: List[Span]) -> List[Span]:
+        """
+        Aggregates extracted measurements together when they are adjacent to handle
+        cases like
+        - 1 meter 50 cm
+        - 30° 4' 54"
+
+        Parameters
+        ----------
+        measurements: List[Span]
+
+        Returns
+        -------
+        List[Span]
+        """
+        if not self.extract_ranges or not self.range_patterns:
+            return measurements
+
+        merged = measurements[:1]
+        for ent in measurements[1:]:
+            last = merged[-1]
+
+            from_text = last.doc[last.start - 1].norm_ if last.start > 0 else None
+            to_text = get_text(last.doc[last.end : ent.start], "NORM", True)
+            matching_patterns = [
+                (a, b)
+                for a, b in self.range_patterns
+                if b == to_text and (a is None or a == from_text)
+            ]
+            if len(matching_patterns):
+                try:
+                    new_value = RangeMeasurement.from_measurements(
+                        last._.value, ent._.value
+                    )
+                    merged[-1] = last = last.doc[
+                        last.start
+                        if matching_patterns[0][0] is None
+                        else last.start - 1 : ent.end
+                    ]
+                    last.label_ = ent.label_
+                    last._.value = new_value
+                except (AttributeError, TypeError):
+                    merged.append(ent)
+            else:
+                merged.append(ent)
+
+        return merged
+
+    def merge_with_existing(
+        self,
+        extracted: List[Span],
+        existing: List[Span],
+    ) -> List[Span]:
+        """
+        Merges the extracted measurements with the existing measurements in the
+        document.
+
+        Parameters
+        ----------
+        extracted: List[Span]
+            The extracted measurements
+        existing: List[Span]
+            The existing measurements in the document
+
+        Returns
+        -------
+        List[Span]
+        """
+        if self.merge_mode == "align":
+            spans_measurements = align_spans(extracted, existing, sort_by_overlap=True)
+
+            extracted = []
+            for span, span_measurements in zip(existing, spans_measurements):
+                if len(span_measurements):
+                    span._.value = span_measurements[0]._.value
+                    extracted.append(span)
+
+        elif self.merge_mode == "intersect":
+            spans_measurements = align_spans(extracted, existing)
+            extracted = []
+            for span, span_measurements in zip(existing, spans_measurements):
+                extracted.extend(span_measurements)
+            extracted = list(dict.fromkeys(extracted))
+
+        else:
+            extracted = [*extracted, *existing]
+
+        return extracted
+
     def __call__(self, doc):
         """
         Adds measurements to document's "measurements" SpanGroup.
 
         Parameters
         ----------
         doc:
             spaCy Doc object
 
         Returns
         -------
         doc:
             spaCy Doc object, annotated for extracted measurements.
         """
-        measurements = self.extract_measurements(doc)
+        ent_labels = set(self.measure_names.values())
+        existing = [
+            ent
+            for ent in (*doc.ents, *doc.spans.get(self.name, ()))
+            if ent.label_ in ent_labels
+        ]
+        other_ents = [ent for ent in doc.ents if ent.label_ not in ent_labels]
+        snippets = (
+            dict.fromkeys(ent.sent for ent in existing)
+            if self.merge_mode in ("intersect", "align")
+            else [doc]
+        )
+        measurements = [m for s in snippets for m in self.extract_measurements(s)[0]]
         measurements = self.merge_adjacent_measurements(measurements)
+        measurements = self.merge_measurements_in_ranges(measurements)
+        measurements = self.merge_with_existing(measurements, existing)
+
+        if self.as_ents:
+            doc.ents = filter_spans((*other_ents, *measurements))
 
-        doc.spans["measurements"] = measurements
+        doc.spans[self.name] = dedup(
+            (*measurements, *doc.spans.get(self.name, ())),
+            key=lambda x: (x.start, x.end, x.label_),
+        )
 
         # for backward compatibility
-        doc.spans["measures"] = doc.spans["measurements"]
+        if self.name == "measurements":
+            doc.spans["measures"] = doc.spans["measurements"]
 
         return doc
-
-
-def measurements_match_tuples_sort_key(
-    span__keep__is_sent_end: Tuple[Span, bool, bool]
-) -> Tuple[int, int, bool]:
-    span, _, is_sent_end = span__keep__is_sent_end
-
-    length = span.end - span.start
-
-    return length, span.end, not is_sent_end
```

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/misc/measurements/patterns.py` & `edsnlp-0.8.0/edsnlp/pipelines/misc/measurements/patterns.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,15 @@
 number_terms = {
+    "0.125": ["⅛"],
+    "0.16666666": ["⅙"],
+    "0.2": ["⅕"],
+    "0.25": ["¼"],
+    "0.3333333": ["⅓"],
+    "0.5": ["½"],
+    "2.5": ["21/2"],
     "1": ["un", "une"],
     "2": ["deux"],
     "3": ["trois"],
     "4": ["quatre"],
     "5": ["cinq"],
     "6": ["six"],
     "7": ["sept"],
@@ -72,14 +79,27 @@
         "dim": "length",
         "degree": 1,
         "scale": 1e2,
         "terms": ["metre", "metres", "m"],
         "followed_by": "cm",
     },
     # Weights
+    "µg": {
+        "dim": "mass",
+        "degree": 1,
+        "scale": 1e-1,
+        "terms": [
+            "microgramme",
+            "microgrammes",
+            "micro-gramme",
+            "microgrammes",
+            "µg",
+        ],
+        "followed_by": None,
+    },
     "mg": {
         "dim": "mass",
         "degree": 1,
         "scale": 1e0,
         "terms": [
             "milligramme",
             "miligramme",
@@ -133,42 +153,42 @@
         "terms": ["mn", "min", "minute", "minutes"],
         "followed_by": "second",
     },
     "hour": {
         "dim": "time",
         "degree": 1,
         "scale": 3600,
-        "terms": ["heure", "h"],
+        "terms": ["heure", "heures", "h"],
         "followed_by": "minute",
     },
     "day": {
         "dim": "time",
         "degree": 1,
-        "scale": 3600 * 1,
+        "scale": 3600 * 24,
         "terms": ["jour", "jours", "j"],
         "followed_by": None,
     },
     "month": {
         "dim": "time",
         "degree": 1,
-        "scale": 3600 * 30.4167,
+        "scale": 3600 * 24 * 30.4167,
         "terms": ["mois"],
         "followed_by": None,
     },
     "week": {
         "dim": "time",
         "degree": 1,
-        "scale": 3600 * 7,
-        "terms": ["semaine", "semaines"],
+        "scale": 3600 * 24 * 7,
+        "terms": ["semaine", "semaines", "sem"],
         "followed_by": None,
     },
     "year": {
         "dim": "time",
         "degree": 1,
-        "scale": 3600 * 365.25,
+        "scale": 3600 * 24 * 365.25,
         "terms": ["an", "année", "ans", "années"],
         "followed_by": None,
     },
     # Angle
     "arc-second": {
         "dim": "time",
         "degree": 1,
@@ -234,15 +254,15 @@
         "terms": ["cac", "c.a.c", "cuillere à café", "cuillères à café"],
         "followed_by": None,
     },
     "goutte": {
         "dim": "length",
         "degree": 3,
         "scale": 5e-5,
-        "terms": ["gt", "goutte"],
+        "terms": ["gt", "goutte", "gouttes"],
         "followed_by": None,
     },
     "mm3": {
         "dim": "length",
         "degree": 3,
         "scale": 1e-3,
         "terms": ["mm3", "mm³"],
@@ -570,8 +590,20 @@
         ],
     },
     "eds.volume": {"unit": "m3", "unitless_patterns": []},
 }
 
 unit_divisors = ["/", "par"]
 
-stopwords = ["par", "sur", "de", "a", ":", ",", "et"]
+stopwords = ["par", "sur", "de", "a", ",", "et"]
+
+# Should we only make accented patterns and expect the user to use
+# `eds.normalizer` component first ?
+range_patterns = [
+    ("De", "à"),
+    ("De", "a"),
+    ("de", "à"),
+    ("de", "a"),
+    ("Entre", "et"),
+    ("entre", "et"),
+    (None, "à"),
+]
```

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/misc/reason/factory.py` & `edsnlp-0.8.0/edsnlp/pipelines/misc/reason/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/misc/reason/patterns.py` & `edsnlp-0.8.0/edsnlp/pipelines/misc/reason/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/misc/reason/reason.py` & `edsnlp-0.8.0/edsnlp/pipelines/misc/reason/reason.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/misc/sections/factory.py` & `edsnlp-0.8.0/edsnlp/pipelines/misc/sections/factory.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/misc/sections/patterns.py` & `edsnlp-0.8.0/edsnlp/pipelines/misc/sections/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/misc/sections/sections.py` & `edsnlp-0.8.0/edsnlp/pipelines/misc/sections/sections.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/ner/adicap/adicap.py` & `edsnlp-0.8.0/edsnlp/pipelines/ner/adicap/adicap.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """`eds.adicap` pipeline"""
-
+import re
 
 from spacy.tokens import Doc, Span
 
 from edsnlp.pipelines.core.contextual_matcher import ContextualMatcher
 from edsnlp.utils.filter import filter_spans
 from edsnlp.utils.resources import get_adicap_dict
 
@@ -57,14 +57,15 @@
         super().set_extensions()
         if not Span.has_extension("adicap"):
             Span.set_extension("adicap", default=None)
         if not Span.has_extension("value"):
             Span.set_extension("value", default=None)
 
     def decode(self, code):
+        code = re.sub("[^A-Za-z0-9 ]+", "", code)
         exploded = list(code)
         adicap = AdicapCode(
             code=code,
             sampling_mode=self.decode_dict["D1"]["codes"].get(exploded[0]),
             technic=self.decode_dict["D2"]["codes"].get(exploded[1]),
             organ=self.decode_dict["D3"]["codes"].get("".join(exploded[2:4])),
         )
```

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/ner/cim10/patterns.py` & `edsnlp-0.8.0/edsnlp/pipelines/ner/cim10/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/ner/scores/base_score.py` & `edsnlp-0.8.0/edsnlp/pipelines/ner/scores/base_score.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,59 +6,64 @@
 from spacy.tokens import Doc, Span
 
 from edsnlp.pipelines.core.contextual_matcher import ContextualMatcher
 from edsnlp.utils.filter import filter_spans
 
 
 class Score(ContextualMatcher):
-    """
-    Matcher component to extract a numeric score
-
-    Parameters
-    ----------
-    nlp : Language
-        The spaCy object.
-    score_name : str
-        The name of the extracted score
-    regex : List[str]
-        A list of regexes to identify the score
-    attr : str
-        Wether to match on the text ('TEXT') or on the normalized text ('NORM')
-    value_extract : str
-        Regex with capturing group to get the score value
-    score_normalization : Callable[[Union[str,None]], Any]
-        Function that takes the "raw" value extracted from the `value_extract` regex,
-        and should return
-        - None if no score could be extracted
-        - The desired score value else
-    window : int
-        Number of token to include after the score's mention to find the
-        score's value
-    """
+    """Matcher component to extract a numeric score"""
 
     def __init__(
         self,
         nlp: Language,
         score_name: str,
         regex: List[str],
         attr: str,
         value_extract: Union[str, Dict[str, str], List[Dict[str, str]]],
         score_normalization: Union[str, Callable[[Union[str, None]], Any]],
         window: int,
         ignore_excluded: bool,
+        ignore_space_tokens: bool,
         flags: Union[re.RegexFlag, int],
     ):
+        """
+        Parameters
+        ----------
+        nlp : Language
+            The spaCy object.
+        score_name : str
+            The name of the extracted score
+        regex : List[str]
+            A list of regexes to identify the score
+        attr : str
+            Whether to match on the text ('TEXT') or on the normalized text ('NORM')
+        value_extract : str
+            Regex with capturing group to get the score value
+        score_normalization : Callable[[Union[str,None]], Any]
+            Function that takes the "raw" value extracted from the `value_extract`
+            regex and should return:
+
+            - None if no score could be extracted
+            - The desired score value else
+        window : int
+            Number of token to include after the score's mention to find the
+            score's value
+        ignore_excluded : bool
+            Whether to ignore excluded spans when matching
+        ignore_space_tokens : bool
+            Whether to ignore space tokens when matching
+        flags : Union[re.RegexFlag, int]
+            Regex flags to use when matching
+        """
         if isinstance(value_extract, str):
-            value_extract = [
-                dict(
-                    name="value",
-                    regex=value_extract,
-                    window=window,
-                )
-            ]
+            value_extract = dict(
+                name="value",
+                regex=value_extract,
+                window=window,
+            )
 
         if isinstance(value_extract, dict):
             value_extract = [value_extract]
 
         value_exists = False
         for i, extract in enumerate(value_extract):
             extract["window"] = extract.get("window", window)
@@ -79,14 +84,15 @@
         super().__init__(
             nlp=nlp,
             name=score_name,
             patterns=patterns,
             assign_as_span=False,
             alignment_mode="expand",
             ignore_excluded=ignore_excluded,
+            ignore_space_tokens=ignore_space_tokens,
             attr=attr,
             regex_flags=flags,
             include_assigned=False,
         )
 
         self.score_name = score_name
```

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/ner/scores/charlson/factory.py` & `edsnlp-0.8.0/edsnlp/pipelines/ner/scores/charlson/factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 DEFAULT_CONFIG = dict(
     regex=patterns.regex,
     value_extract=patterns.value_extract,
     score_normalization=patterns.score_normalization_str,
     attr="NORM",
     window=7,
     ignore_excluded=False,
+    ignore_space_tokens=False,
     flags=0,
 )
 
 
 @deprecated_factory(
     "charlson",
     "eds.charlson",
@@ -34,20 +35,22 @@
     name: str,
     regex: List[str],
     value_extract: str,
     score_normalization: Union[str, Callable[[Union[str, None]], Any]],
     attr: str,
     window: int,
     ignore_excluded: bool,
+    ignore_space_tokens: bool,
     flags: Union[re.RegexFlag, int],
 ):
     return Score(
         nlp,
         score_name=name,
         regex=regex,
         value_extract=value_extract,
         score_normalization=score_normalization,
         attr=attr,
         window=window,
         ignore_excluded=ignore_excluded,
+        ignore_space_tokens=ignore_space_tokens,
         flags=flags,
     )
```

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/ner/scores/charlson/patterns.py` & `edsnlp-0.8.0/edsnlp/pipelines/ner/scores/charlson/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/ner/scores/elstonellis/factory.py` & `edsnlp-0.8.0/edsnlp/pipelines/ner/scores/elstonellis/factory.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,38 +9,73 @@
 DEFAULT_CONFIG = dict(
     regex=patterns.regex,
     value_extract=patterns.value_extract,
     score_normalization=patterns.score_normalization_str,
     attr="TEXT",
     window=20,
     ignore_excluded=False,
+    ignore_space_tokens=False,
     flags=0,
 )
 
 
 @Language.factory(
     "eds.elston-ellis",
     default_config=DEFAULT_CONFIG,
     assigns=["doc.ents", "doc.spans"],
 )
 def create_component(
     nlp: Language,
     name: str,
-    regex: List[str],
-    value_extract: str,
-    score_normalization: Union[str, Callable[[Union[str, None]], Any]],
-    attr: str,
-    window: int,
-    ignore_excluded: bool,
-    flags: Union[re.RegexFlag, int],
+    regex: List[str] = patterns.regex,
+    value_extract: str = patterns.value_extract,
+    score_normalization: Union[
+        str, Callable[[Union[str, None]], Any]
+    ] = patterns.score_normalization_str,
+    attr: str = "TEXT",
+    window: int = 20,
+    ignore_excluded: bool = False,
+    ignore_space_tokens: bool = False,
+    flags: Union[re.RegexFlag, int] = 0,
 ):
+    """
+    Matcher for the Elston-Ellis score.
+
+    Parameters
+    ----------
+    nlp: Language
+        The spaCy Language object
+    name: str
+        The name of the component
+    regex: List[str]
+        The regex patterns to match
+    value_extract: str
+        The regex pattern to extract the value from the matched text
+    score_normalization: Union[str, Callable[[Union[str, None]], Any]]
+        The normalization function to apply to the extracted value
+    attr: str
+        The token attribute to match on (e.g. "TEXT" or "NORM")
+    window: int
+        The window size to search for the regex pattern
+    ignore_excluded: bool
+        Whether to ignore excluded tokens
+    ignore_space_tokens: bool
+        Whether to ignore space tokens
+    flags: Union[re.RegexFlag, int]
+        The regex flags to use
+
+    Returns
+    -------
+    Score
+    """
     return Score(
         nlp,
         score_name=name,
         regex=regex,
         value_extract=value_extract,
         score_normalization=score_normalization,
         attr=attr,
         window=window,
         ignore_excluded=ignore_excluded,
+        ignore_space_tokens=ignore_space_tokens,
         flags=flags,
     )
```

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/ner/scores/elstonellis/patterns.py` & `edsnlp-0.8.0/edsnlp/pipelines/ner/scores/elstonellis/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/ner/scores/emergency/ccmu/factory.py` & `edsnlp-0.8.0/edsnlp/pipelines/ner/scores/emergency/priority/factory.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,53 +1,87 @@
 import re
 from typing import Any, Callable, List, Union
 
 from spacy.language import Language
 
 from edsnlp.pipelines.ner.scores import Score
-from edsnlp.pipelines.ner.scores.emergency.ccmu import patterns
+from edsnlp.pipelines.ner.scores.emergency.priority import patterns
 from edsnlp.utils.deprecation import deprecated_factory
 
 DEFAULT_CONFIG = dict(
     regex=patterns.regex,
     value_extract=patterns.value_extract,
     score_normalization=patterns.score_normalization_str,
     attr="NORM",
-    window=20,
+    window=7,
     ignore_excluded=False,
     flags=0,
 )
 
 
 @deprecated_factory(
-    "emergency.ccmu",
-    "eds.emergency.ccmu",
+    "emergency.priority",
+    "eds.emergency.priority",
     default_config=DEFAULT_CONFIG,
     assigns=["doc.ents", "doc.spans"],
 )
 @Language.factory(
-    "eds.emergency.ccmu",
+    "eds.emergency.priority",
     default_config=DEFAULT_CONFIG,
     assigns=["doc.ents", "doc.spans"],
 )
 def create_component(
     nlp: Language,
-    name: str,
-    regex: List[str],
-    value_extract: str,
-    score_normalization: Union[str, Callable[[Union[str, None]], Any]],
-    attr: str,
-    window: int,
-    ignore_excluded: bool,
-    flags: Union[re.RegexFlag, int],
+    name: str = "emergency.priority",
+    regex: List[str] = patterns.regex,
+    value_extract: str = patterns.value_extract,
+    score_normalization: Union[
+        str, Callable[[Union[str, None]], Any]
+    ] = patterns.score_normalization_str,
+    attr: str = "NORM",
+    window: int = 7,
+    ignore_excluded: bool = False,
+    ignore_space_tokens: bool = False,
+    flags: Union[re.RegexFlag, int] = 0,
 ):
+    """
+    Matcher for the Emergency Priority score.
+
+    Parameters
+    ----------
+    nlp: Language
+        The spaCy Language object
+    name: str
+        The name of the component
+    regex: List[str]
+        The regex patterns to match
+    value_extract: str
+        The regex pattern to extract the value from the matched text
+    score_normalization: Union[str, Callable[[Union[str, None]], Any]]
+        The normalization function to apply to the extracted value
+    attr: str
+        The token attribute to match on (e.g. "TEXT" or "NORM")
+    window: int
+        The window size to search for the regex pattern
+    ignore_excluded: bool
+        Whether to ignore excluded tokens
+    ignore_space_tokens: bool
+        Whether to ignore space tokens
+    flags: Union[re.RegexFlag, int]
+        The regex flags to use
+
+    Returns
+    -------
+    Score
+    """
     return Score(
         nlp,
         score_name=name,
         regex=regex,
         value_extract=value_extract,
         score_normalization=score_normalization,
         attr=attr,
         window=window,
         ignore_excluded=ignore_excluded,
+        ignore_space_tokens=ignore_space_tokens,
         flags=flags,
     )
```

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/ner/scores/emergency/ccmu/patterns.py` & `edsnlp-0.8.0/edsnlp/pipelines/ner/scores/emergency/ccmu/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/ner/scores/emergency/gemsa/factory.py` & `edsnlp-0.8.0/edsnlp/pipelines/ner/scores/emergency/ccmu/factory.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,53 +1,87 @@
 import re
 from typing import Any, Callable, List, Union
 
 from spacy.language import Language
 
 from edsnlp.pipelines.ner.scores import Score
-from edsnlp.pipelines.ner.scores.emergency.gemsa import patterns
+from edsnlp.pipelines.ner.scores.emergency.ccmu import patterns
 from edsnlp.utils.deprecation import deprecated_factory
 
 DEFAULT_CONFIG = dict(
     regex=patterns.regex,
     value_extract=patterns.value_extract,
     score_normalization=patterns.score_normalization_str,
     attr="NORM",
     window=20,
     ignore_excluded=False,
     flags=0,
 )
 
 
 @deprecated_factory(
-    "emergency.gemsa",
-    "eds.emergency.gemsa",
+    "emergency.ccmu",
+    "eds.emergency.ccmu",
     default_config=DEFAULT_CONFIG,
     assigns=["doc.ents", "doc.spans"],
 )
 @Language.factory(
-    "eds.emergency.gemsa",
+    "eds.emergency.ccmu",
     default_config=DEFAULT_CONFIG,
     assigns=["doc.ents", "doc.spans"],
 )
 def create_component(
     nlp: Language,
-    name: str,
-    regex: List[str],
-    value_extract: str,
-    score_normalization: Union[str, Callable[[Union[str, None]], Any]],
-    attr: str,
-    window: int,
-    ignore_excluded: bool,
-    flags: Union[re.RegexFlag, int],
+    name: str = "eds.emergency.ccmu",
+    regex: List[str] = patterns.regex,
+    value_extract: str = patterns.value_extract,
+    score_normalization: Union[
+        str, Callable[[Union[str, None]], Any]
+    ] = patterns.score_normalization_str,
+    attr: str = "NORM",
+    window: int = 20,
+    ignore_excluded: bool = False,
+    ignore_space_tokens: bool = False,
+    flags: Union[re.RegexFlag, int] = 0,
 ):
+    """
+    Matcher for the Emergency CCMU score.
+
+    Parameters
+    ----------
+    nlp: Language
+        The spaCy Language object
+    name: str
+        The name of the component
+    regex: List[str]
+        The regex patterns to match
+    value_extract: str
+        The regex pattern to extract the value from the matched text
+    score_normalization: Union[str, Callable[[Union[str, None]], Any]]
+        The normalization function to apply to the extracted value
+    attr: str
+        The token attribute to match on (e.g. "TEXT" or "NORM")
+    window: int
+        The window size to search for the regex pattern
+    ignore_excluded: bool
+        Whether to ignore excluded tokens
+    ignore_space_tokens: bool
+        Whether to ignore space tokens
+    flags: Union[re.RegexFlag, int]
+        The regex flags to use
+
+    Returns
+    -------
+    Score
+    """
     return Score(
         nlp,
         score_name=name,
         regex=regex,
         value_extract=value_extract,
         score_normalization=score_normalization,
         attr=attr,
         window=window,
         ignore_excluded=ignore_excluded,
+        ignore_space_tokens=ignore_space_tokens,
         flags=flags,
     )
```

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/ner/scores/emergency/gemsa/patterns.py` & `edsnlp-0.8.0/edsnlp/pipelines/ner/scores/emergency/gemsa/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/ner/scores/emergency/priority/patterns.py` & `edsnlp-0.8.0/edsnlp/pipelines/ner/scores/emergency/priority/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/ner/scores/factory.py` & `edsnlp-0.8.0/edsnlp/pipelines/misc/tables/factory.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,50 +1,32 @@
-import re
-from typing import Any, Callable, List, Union
+from typing import Dict, List, Optional, Union
 
 from spacy.language import Language
 
-from edsnlp.pipelines.ner.scores import Score
+from edsnlp.pipelines.misc.tables import TablesMatcher
 from edsnlp.utils.deprecation import deprecated_factory
 
 DEFAULT_CONFIG = dict(
-    attr="NORM",
-    window=7,
-    ignore_excluded=False,
-    flags=0,
+    tables_pattern=None,
+    sep_pattern=None,
+    attr="TEXT",
+    ignore_excluded=True,
 )
 
 
-@deprecated_factory(
-    "score",
-    "eds.score",
-    default_config=DEFAULT_CONFIG,
-    assigns=["doc.ents", "doc.spans"],
-)
-@Language.factory(
-    "eds.score",
-    default_config=DEFAULT_CONFIG,
-    assigns=["doc.ents", "doc.spans"],
-)
+@deprecated_factory("tables", "eds.tables", default_config=DEFAULT_CONFIG)
+@Language.factory("eds.tables", default_config=DEFAULT_CONFIG)
 def create_component(
     nlp: Language,
     name: str,
-    score_name: str,
-    regex: List[str],
-    value_extract: str,
-    score_normalization: Union[str, Callable[[Union[str, None]], Any]],
+    tables_pattern: Optional[Dict[str, Union[List[str], str]]],
+    sep_pattern: Optional[str],
     attr: str,
-    window: int,
-    flags: Union[re.RegexFlag, int],
     ignore_excluded: bool,
 ):
-    return Score(
+    return TablesMatcher(
         nlp,
-        score_name=score_name,
-        regex=regex,
-        value_extract=value_extract,
-        score_normalization=score_normalization,
+        tables_pattern=tables_pattern,
+        sep_pattern=sep_pattern,
         attr=attr,
-        flags=flags,
-        window=window,
         ignore_excluded=ignore_excluded,
     )
```

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/ner/scores/sofa/factory.py` & `edsnlp-0.8.0/edsnlp/pipelines/ner/covid/factory.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,52 +1,56 @@
-import re
-from typing import Any, Callable, Dict, List, Union
+from typing import Dict, Union
 
 from spacy.language import Language
 
-from edsnlp.pipelines.ner.scores.sofa import Sofa, patterns
-from edsnlp.utils.deprecation import deprecated_factory
+from edsnlp.pipelines.core.matcher import GenericMatcher
+
+from . import patterns
 
 DEFAULT_CONFIG = dict(
-    regex=patterns.regex,
-    value_extract=patterns.value_extract,
-    score_normalization=patterns.score_normalization_str,
-    attr="NORM",
-    window=10,
+    attr="LOWER",
     ignore_excluded=False,
-    flags=0,
+    ignore_space_tokens=False,
 )
 
 
-@deprecated_factory(
-    "SOFA",
-    "eds.SOFA",
-    default_config=DEFAULT_CONFIG,
-    assigns=["doc.ents", "doc.spans"],
-)
 @Language.factory(
-    "eds.SOFA",
+    "eds.covid",
     default_config=DEFAULT_CONFIG,
     assigns=["doc.ents", "doc.spans"],
 )
 def create_component(
     nlp: Language,
-    name: str,
-    regex: List[str],
-    value_extract: List[Dict[str, str]],
-    score_normalization: Union[str, Callable[[Union[str, None]], Any]],
-    attr: str,
-    window: int,
-    ignore_excluded: bool,
-    flags: Union[re.RegexFlag, int],
+    name: str = "eds.covid",
+    attr: Union[str, Dict[str, str]] = "LOWER",
+    ignore_excluded: bool = False,
+    ignore_space_tokens: bool = False,
 ):
-    return Sofa(
+    """
+    Create a factory that returns new GenericMatcher with patterns for covid
+
+    Parameters
+    ----------
+    nlp: Language
+        spaCy `Language` object.
+    name: str
+        The name of the pipe
+    attr: Union[str, Dict[str, str]]
+        Attribute to match on, eg `TEXT`, `NORM`, etc.
+    ignore_excluded: bool
+        Whether to skip excluded tokens during matching.
+    ignore_space_tokens: bool
+        Whether to skip space tokens during matching.
+
+    Returns
+    -------
+    GenericMatcher
+    """
+
+    return GenericMatcher(
         nlp,
-        score_name=name,
-        regex=regex,
-        value_extract=value_extract,
-        score_normalization=score_normalization,
+        terms=None,
+        regex=dict(covid=patterns.pattern),
         attr=attr,
-        window=window,
         ignore_excluded=ignore_excluded,
-        flags=flags,
+        ignore_space_tokens=ignore_space_tokens,
     )
```

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/ner/scores/sofa/patterns.py` & `edsnlp-0.8.0/edsnlp/pipelines/ner/scores/sofa/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/ner/scores/sofa/sofa.py` & `edsnlp-0.8.0/edsnlp/pipelines/ner/scores/sofa/sofa.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,58 +11,61 @@
     """
     Matcher component to extract the SOFA score
 
     Parameters
     ----------
     nlp : Language
         The spaCy object.
-    score_name : str
-        The name of the extracted score
     regex : List[str]
         A list of regexes to identify the SOFA score
     attr : str
-        Wether to match on the text ('TEXT') or on the normalized text ('CUSTOM_NORM')
-    method_regex : str
-        Regex with capturing group to get the score extraction method
-        (e.g. "à l'admission", "à 24H", "Maximum")
-    value_regex : str
+        Whether to match on the text ('TEXT') or on the normalized text ('CUSTOM_NORM')
+    value_extract : Dict[str, str]
         Regex to extract the score value
     score_normalization : Callable[[Union[str,None]], Any]
         Function that takes the "raw" value extracted from the `value_extract` regex,
         and should return
         - None if no score could be extracted
         - The desired score value else
     window : int
         Number of token to include after the score's mention to find the
         score's value
+    ignore_excluded : bool
+        Whether to ignore excluded spans
+    ignore_space_tokens : bool
+        Whether to ignore space tokens
+    flags : Union[re.RegexFlag, int]
+        Flags to pass to the regex
     """
 
     def __init__(
         self,
         nlp: Language,
         score_name: str,
         regex: List[str],
         attr: str,
         value_extract: List[Dict[str, str]],
         score_normalization: Union[str, Callable[[Union[str, None]], Any]],
         window: int,
         flags: Union[re.RegexFlag, int],
         ignore_excluded: bool,
+        ignore_space_tokens: bool,
     ):
 
         super().__init__(
             nlp,
             score_name=score_name,
             regex=regex,
             value_extract=value_extract,
             score_normalization=score_normalization,
             attr=attr,
             window=window,
             flags=flags,
             ignore_excluded=ignore_excluded,
+            ignore_space_tokens=ignore_space_tokens,
         )
 
         self.set_extensions()
 
     @classmethod
     def set_extensions(cls) -> None:
         super(Sofa, Sofa).set_extensions()
```

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/ner/scores/tnm/models.py` & `edsnlp-0.8.0/edsnlp/pipelines/ner/scores/tnm/models.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/ner/scores/tnm/patterns.py` & `edsnlp-0.8.0/edsnlp/pipelines/ner/scores/tnm/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/ner/scores/tnm/tnm.py` & `edsnlp-0.8.0/edsnlp/pipelines/ner/scores/tnm/tnm.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/ner/umls/patterns.py` & `edsnlp-0.8.0/edsnlp/pipelines/ner/umls/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/qualifiers/base.py` & `edsnlp-0.8.0/edsnlp/pipelines/qualifiers/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from itertools import chain
-from typing import Dict, List, Optional
+from typing import Dict, List, Optional, Set, Union
 
 from loguru import logger
 from spacy.language import Language
 from spacy.tokens import Doc, Span
 
 from edsnlp.matchers.phrase import EDSPhraseMatcher
 from edsnlp.pipelines.base import BaseComponent
@@ -41,46 +41,59 @@
     ----------
     nlp : Language
         spaCy nlp pipeline to use for matching.
     attr : str
         spaCy's attribute to use:
         a string with the value "TEXT" or "NORM", or a dict with the key 'term_attr'
         we can also add a key for each regex.
-    on_ents_only : bool
+    on_ents_only : Union[bool, str, List[str], Set[str]]
         Whether to look for matches around detected entities only.
         Useful for faster inference in downstream tasks.
+
+        - If True, will look in all ents located in `doc.ents` only
+        - If an iterable of string is passed, will additionally look in `doc.spans[key]`
+        for each key in the iterable
     explain : bool
         Whether to keep track of cues for each entity.
     **terms : Dict[str, Optional[List[str]]]
         Terms to look for.
     """
 
     defaults = dict()
 
     def __init__(
         self,
         nlp: Language,
         attr: str,
-        on_ents_only: bool,
+        on_ents_only: Union[bool, str, List[str], Set[str]],
         explain: bool,
         **terms: Dict[str, Optional[List[str]]],
     ):
 
         if attr.upper() == "NORM":
             check_normalizer(nlp)
 
         self.phrase_matcher = EDSPhraseMatcher(vocab=nlp.vocab, attr=attr)
         self.phrase_matcher.build_patterns(nlp=nlp, terms=terms)
 
         self.on_ents_only = on_ents_only
+
+        assert isinstance(on_ents_only, (list, str, set, bool)), (
+            "The `on_ents_only` argument should be a "
+            "string, a bool, a list or a set of string"
+        )
+
+        if isinstance(on_ents_only, list):
+            on_ents_only = set(on_ents_only)
+        elif isinstance(on_ents_only, str):
+            on_ents_only = set([on_ents_only])
+        self.on_ents_only = on_ents_only
         self.explain = explain
 
-    def get_defaults(
-        self, **kwargs: Dict[str, Optional[List[str]]]
-    ) -> Dict[str, List[str]]:
+    def get_defaults(self, **kwargs: Optional[List[str]]) -> Dict[str, List[str]]:
         """
         Merge terms with their defaults. Null keys are replaced with defaults.
 
         Returns
         -------
         Dict[str, List[str]]
             Merged dictionary
@@ -98,29 +111,30 @@
         """
         Extract matches.
 
         Parameters
         ----------
         doc : Doc
             spaCy `Doc` object.
-
         Returns
         -------
         List[Span]
             List of detected spans
         """
+
         if self.on_ents_only:
+            sents = set([ent.sent for ent in self.get_spans(doc)])
 
-            sents = set([ent.sent for ent in doc.ents])
             match_iterator = map(
                 lambda sent: self.phrase_matcher(sent, as_spans=True), sents
             )
 
             matches = chain.from_iterable(match_iterator)
 
         else:
+
             matches = self.phrase_matcher(doc, as_spans=True)
 
         return list(matches)
 
     def __call__(self, doc: Doc) -> Doc:
         return self.process(doc)
```

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/qualifiers/family/factory.py` & `edsnlp-0.8.0/edsnlp/pipelines/qualifiers/family/factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Optional
+from typing import List, Optional, Set, Union
 
 from spacy.language import Language
 
 from edsnlp.pipelines.qualifiers.family import FamilyContext
 from edsnlp.utils.deprecation import deprecated_factory
 
 DEFAULT_CONFIG = dict(
@@ -29,15 +29,15 @@
 def create_component(
     nlp: Language,
     name: str,
     family: Optional[List[str]],
     termination: Optional[List[str]],
     attr: str,
     explain: bool,
-    on_ents_only: bool,
+    on_ents_only: Union[bool, str, List[str], Set[str]],
     use_sections: bool,
 ):
     return FamilyContext(
         nlp,
         family=family,
         termination=termination,
         attr=attr,
```

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/qualifiers/family/family.py` & `edsnlp-0.8.0/edsnlp/pipelines/qualifiers/family/family.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Optional
+from typing import List, Optional, Set, Union
 
 from loguru import logger
 from spacy.language import Language
 from spacy.tokens import Doc, Span, Token
 
 from edsnlp.pipelines.qualifiers.base import Qualifier
 from edsnlp.pipelines.terminations import termination
@@ -12,33 +12,32 @@
 from .patterns import family
 
 
 class FamilyContext(Qualifier):
     """
     Implements a family context detection algorithm.
 
-    The components looks for terms indicating family references in the text.
+    The component looks for terms indicating family references in the text.
 
     Parameters
     ----------
     nlp : Language
         spaCy nlp pipeline to use for matching.
     family : Optional[List[str]]
         List of terms indicating family reference.
-    terminations : Optional[List[str]]
-        List of termination terms, to separate syntagmas.
     attr : str
         spaCy's attribute to use:
         a string with the value "TEXT" or "NORM", or a dict with the key 'term_attr'
         we can also add a key for each regex.
-    on_ents_only : bool
+    on_ents_only : Union[bool, str, List[str], Set[str]]
         Whether to look for matches around detected entities only.
         Useful for faster inference in downstream tasks.
-    regex : Optional[Dict[str, Union[List[str], str]]]
-        A dictionnary of regex patterns.
+        - If True, will look in all ents located in `doc.ents` only
+        - If an iterable of string is passed, will additionally look in `doc.spans[key]`
+        for each key in the iterable
     explain : bool
         Whether to keep track of cues for each entity.
     use_sections : bool, by default `False`
         Whether to use annotated sections (namely `antécédents familiaux`).
     """
 
     defaults = dict(
@@ -50,15 +49,15 @@
         self,
         nlp: Language,
         attr: str,
         family: Optional[List[str]],
         termination: Optional[List[str]],
         use_sections: bool,
         explain: bool,
-        on_ents_only: bool,
+        on_ents_only: Union[bool, str, List[str], Set[str]],
     ):
 
         terms = self.get_defaults(
             family=family,
             termination=termination,
         )
 
@@ -124,15 +123,15 @@
 
         terminations = get_spans(matches, "termination")
         boundaries = self._boundaries(doc, terminations)
 
         # Removes duplicate matches and pseudo-expressions in one statement
         matches = filter_spans(matches, label_to_remove="pseudo")
 
-        entities = list(doc.ents) + list(doc.spans.get("discarded", []))
+        entities = list(self.get_spans(doc))
         ents = None
 
         sections = []
 
         if self.sections:
             sections = [
                 Span(doc, section.start, section.end, label="FAMILY")
```

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/qualifiers/family/patterns.py` & `edsnlp-0.8.0/edsnlp/pipelines/qualifiers/family/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/qualifiers/history/factory.py` & `edsnlp-0.8.0/edsnlp/pipelines/qualifiers/history/factory.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Optional
+from typing import List, Optional, Set, Union
 
 from spacy.language import Language
 
 from edsnlp.pipelines.qualifiers.history import History, patterns
 from edsnlp.pipelines.terminations import termination
 from edsnlp.utils.deprecation import deprecated_factory
 
@@ -51,15 +51,15 @@
     use_sections: bool,
     use_dates: bool,
     history_limit: int,
     exclude_birthdate: bool,
     closest_dates_only: bool,
     attr: str,
     explain: bool,
-    on_ents_only: bool,
+    on_ents_only: Union[bool, str, List[str], Set[str]],
 ):
     return History(
         nlp,
         attr=attr,
         history=history,
         termination=termination,
         use_sections=use_sections,
```

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/qualifiers/history/history.py` & `edsnlp-0.8.0/edsnlp/pipelines/qualifiers/history/history.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import timedelta
-from typing import List, Optional
+from typing import List, Optional, Set, Union
 
 import pendulum
 from loguru import logger
 from spacy.language import Language
 from spacy.tokens import Doc, Span, Token
 
 from edsnlp.pipelines.qualifiers.base import Qualifier
@@ -13,26 +13,24 @@
 from edsnlp.utils.inclusion import check_inclusion, check_sent_inclusion
 
 from .patterns import history, sections_history
 
 
 class History(Qualifier):
     """
-    Implements an history detection algorithm.
+    Implements a history detection algorithm.
 
-    The components looks for terms indicating history in the text.
+    The component looks for terms indicating history in the text.
 
     Parameters
     ----------
     nlp : Language
         spaCy nlp pipeline to use for matching.
     history : Optional[List[str]]
         List of terms indicating medical history reference.
-    termination : Optional[List[str]]
-        List of syntagme termination terms.
     use_sections : bool
         Whether to use section pipeline to detect medical history section.
     use_dates : bool
         Whether to use dates pipeline to detect if the event occurs
          a long time before the document date.
     history_limit : int
         The number of days after which the event is considered as history.
@@ -40,19 +38,20 @@
         Whether to exclude the birth date from history dates.
     closest_dates_only : bool
         Whether to include the closest dates only.
     attr : str
         spaCy's attribute to use:
         a string with the value "TEXT" or "NORM", or a dict with the key 'term_attr'
         we can also add a key for each regex.
-    on_ents_only : bool
+    on_ents_only : Union[bool, str, List[str], Set[str]]
         Whether to look for matches around detected entities only.
         Useful for faster inference in downstream tasks.
-    regex : Optional[Dict[str, Union[List[str], str]]]
-        A dictionary of regex patterns.
+        - If True, will look in all ents located in `doc.ents` only
+        - If an iterable of string is passed, will additionally look in `doc.spans[key]`
+        for each key in the iterable
     explain : bool
         Whether to keep track of cues for each entity.
     """
 
     defaults = dict(
         history=history,
         termination=termination,
@@ -66,15 +65,15 @@
         termination: Optional[List[str]],
         use_sections: bool,
         use_dates: bool,
         history_limit: int,
         closest_dates_only: bool,
         exclude_birthdate: bool,
         explain: bool,
-        on_ents_only: bool,
+        on_ents_only: Union[bool, str, List[str], Set[str]],
     ):
 
         terms = self.get_defaults(
             history=history,
             termination=termination,
         )
 
@@ -257,15 +256,15 @@
 
         terminations = get_spans(matches, "termination")
         boundaries = self._boundaries(doc, terminations)
 
         # Removes duplicate matches and pseudo-expressions in one statement
         matches = filter_spans(matches, label_to_remove="pseudo")
 
-        entities = list(doc.ents) + list(doc.spans.get("discarded", []))
+        entities = self.get_spans(doc)
         ents = None
         sub_sections = None
         sub_recent_dates = None
         sub_history_dates = None
 
         sections = []
         if self.sections:
```

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/qualifiers/hypothesis/factory.py` & `edsnlp-0.8.0/edsnlp/pipelines/qualifiers/hypothesis/factory.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Optional
+from typing import List, Optional, Set, Union
 
 from spacy.language import Language
 
 from edsnlp.pipelines.qualifiers.hypothesis import Hypothesis
 from edsnlp.utils.deprecation import deprecated_factory
 
 DEFAULT_CONFIG = dict(
@@ -36,15 +36,15 @@
     attr: str,
     pseudo: Optional[List[str]],
     preceding: Optional[List[str]],
     following: Optional[List[str]],
     termination: Optional[List[str]],
     verbs_eds: Optional[List[str]],
     verbs_hyp: Optional[List[str]],
-    on_ents_only: bool,
+    on_ents_only: Union[bool, str, List[str], Set[str]],
     within_ents: bool,
     explain: bool,
 ):
     return Hypothesis(
         nlp=nlp,
         attr=attr,
         pseudo=pseudo,
```

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/qualifiers/hypothesis/hypothesis.py` & `edsnlp-0.8.0/edsnlp/pipelines/qualifiers/hypothesis/hypothesis.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Optional
+from typing import List, Optional, Set, Union
 
 from spacy.language import Language
 from spacy.tokens import Doc, Span, Token
 
 from edsnlp.pipelines.qualifiers.base import Qualifier
 from edsnlp.pipelines.terminations import termination
 from edsnlp.utils.filter import consume_spans, filter_spans, get_spans
@@ -14,50 +14,50 @@
 
 class Hypothesis(Qualifier):
     """
     Hypothesis detection with spaCy.
 
     The component looks for five kinds of expressions in the text :
 
-    - preceding hypothesis, ie cues that precede a hypothetic expression
-    - following hypothesis, ie cues that follow a hypothetic expression
+    - preceding hypothesis, ie cues that precede a hypothetical expression
+    - following hypothesis, ie cues that follow a hypothetical expression
     - pseudo hypothesis : contain a hypothesis cue, but are not hypothesis
       (eg "pas de doute"/"no doubt")
-    - hypothetic verbs : verbs indicating hypothesis (eg "douter")
+    - hypothetical verbs : verbs indicating hypothesis (eg "douter")
     - classic verbs conjugated to the conditional, thus indicating hypothesis
 
     Parameters
     ----------
     nlp : Language
         spaCy nlp pipeline to use for matching.
     pseudo : Optional[List[str]]
         List of pseudo hypothesis cues.
     preceding : Optional[List[str]]
         List of preceding hypothesis cues
     following : Optional[List[str]]
         List of following hypothesis cues.
     verbs_hyp : Optional[List[str]]
-        List of hypothetic verbs.
+        List of hypothetical verbs.
     verbs_eds : Optional[List[str]]
         List of mainstream verbs.
-    filter_matches : bool
-        Whether to filter out overlapping matches.
     attr : str
         spaCy's attribute to use:
         a string with the value "TEXT" or "NORM", or a dict with the key 'term_attr'
         we can also add a key for each regex.
-    on_ents_only : bool
+    on_ents_only : Union[bool, str, List[str], Set[str]]
         Whether to look for matches around detected entities only.
         Useful for faster inference in downstream tasks.
+
+        - If True, will look in all ents located in `doc.ents` only
+        - If an iterable of string is passed, will additionally look in `doc.spans[key]`
+        for each key in the iterable
     within_ents : bool
         Whether to consider cues within entities.
     explain : bool
         Whether to keep track of cues for each entity.
-    regex : Optional[Dict[str, Union[List[str], str]]]
-        A dictionnary of regex patterns.
     """
 
     defaults = dict(
         following=following,
         preceding=preceding,
         pseudo=pseudo,
         termination=termination,
@@ -71,15 +71,15 @@
         attr: str,
         pseudo: Optional[List[str]],
         preceding: Optional[List[str]],
         following: Optional[List[str]],
         termination: Optional[List[str]],
         verbs_eds: Optional[List[str]],
         verbs_hyp: Optional[List[str]],
-        on_ents_only: bool,
+        on_ents_only: Union[bool, str, List[str], Set[str]],
         within_ents: bool,
         explain: bool,
     ):
 
         terms = self.get_defaults(
             pseudo=pseudo,
             preceding=preceding,
@@ -182,15 +182,15 @@
 
         terminations = get_spans(matches, "termination")
         boundaries = self._boundaries(doc, terminations)
 
         # Removes duplicate matches and pseudo-expressions in one statement
         matches = filter_spans(matches, label_to_remove="pseudo")
 
-        entities = list(doc.ents) + list(doc.spans.get("discarded", []))
+        entities = list(self.get_spans(doc))
         ents = None
 
         for start, end in boundaries:
 
             ents, entities = consume_spans(
                 entities,
                 filter=lambda s: check_inclusion(s, start, end),
```

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/qualifiers/hypothesis/patterns.py` & `edsnlp-0.8.0/edsnlp/pipelines/qualifiers/hypothesis/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/qualifiers/negation/factory.py` & `edsnlp-0.8.0/edsnlp/pipelines/qualifiers/negation/factory.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Optional
+from typing import List, Optional, Set, Union
 
 from spacy.language import Language
 
 from edsnlp.pipelines.qualifiers.negation import Negation
 from edsnlp.utils.deprecation import deprecated_factory
 
 DEFAULT_CONFIG = dict(
@@ -34,15 +34,15 @@
     name: str,
     attr: str,
     pseudo: Optional[List[str]],
     preceding: Optional[List[str]],
     following: Optional[List[str]],
     termination: Optional[List[str]],
     verbs: Optional[List[str]],
-    on_ents_only: bool,
+    on_ents_only: Union[bool, str, List[str], Set[str]],
     within_ents: bool,
     explain: bool,
 ):
 
     return Negation(
         nlp=nlp,
         attr=attr,
```

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/qualifiers/negation/negation.py` & `edsnlp-0.8.0/edsnlp/pipelines/qualifiers/negation/negation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Optional
+from typing import List, Optional, Set, Union
 
 from spacy.language import Language
 from spacy.tokens import Doc, Span, Token
 
 from edsnlp.pipelines.qualifiers.base import Qualifier
 from edsnlp.pipelines.terminations import termination
 from edsnlp.utils.deprecation import deprecated_getter_factory
@@ -43,17 +43,21 @@
         List of preceding negation terms
     following : Optional[List[str]]
         List of following negation terms.
     termination : Optional[List[str]]
         List of termination terms.
     verbs : Optional[List[str]]
         List of negation verbs.
-    on_ents_only : bool
+    on_ents_only : Union[bool, str, List[str], Set[str]]
         Whether to look for matches around detected entities only.
         Useful for faster inference in downstream tasks.
+
+        - If True, will look in all ents located in `doc.ents` only
+        - If an iterable of string is passed, will additionally look in `doc.spans[key]`
+        for each key in the iterable
     within_ents : bool
         Whether to consider cues within entities.
     explain : bool
         Whether to keep track of cues for each entity.
     """
 
     defaults = dict(
@@ -69,15 +73,15 @@
         nlp: Language,
         attr: str,
         pseudo: Optional[List[str]],
         preceding: Optional[List[str]],
         following: Optional[List[str]],
         termination: Optional[List[str]],
         verbs: Optional[List[str]],
-        on_ents_only: bool,
+        on_ents_only: Union[bool, str, List[str], Set[str]],
         within_ents: bool,
         explain: bool,
     ):
 
         terms = self.get_defaults(
             pseudo=pseudo,
             preceding=preceding,
@@ -227,20 +231,20 @@
         """
 
         matches = self.get_matches(doc)
 
         terminations = get_spans(matches, "termination")
         boundaries = self._boundaries(doc, terminations)
 
-        entities = list(doc.ents) + list(doc.spans.get("discarded", []))
-        ents = None
-
         # Removes duplicate matches and pseudo-expressions in one statement
         matches = filter_spans(matches, label_to_remove="pseudo")
 
+        entities = list(self.get_spans(doc))
+        ents = None
+
         for start, end in boundaries:
 
             ents, entities = consume_spans(
                 entities,
                 filter=lambda s: check_inclusion(s, start, end),
                 second_chance=ents,
             )
```

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/qualifiers/negation/patterns.py` & `edsnlp-0.8.0/edsnlp/pipelines/qualifiers/negation/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/qualifiers/reported_speech/factory.py` & `edsnlp-0.8.0/edsnlp/pipelines/qualifiers/reported_speech/factory.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Optional
+from typing import List, Optional, Set, Union
 
 from spacy.language import Language
 
 from edsnlp.pipelines.qualifiers.reported_speech import ReportedSpeech
 from edsnlp.utils.deprecation import deprecated_factory
 
 DEFAULT_CONFIG = dict(
@@ -40,15 +40,15 @@
     name: str,
     attr: str,
     pseudo: Optional[List[str]],
     preceding: Optional[List[str]],
     following: Optional[List[str]],
     quotation: Optional[List[str]],
     verbs: Optional[List[str]],
-    on_ents_only: bool,
+    on_ents_only: Union[bool, str, List[str], Set[str]],
     within_ents: bool,
     explain: bool,
 ):
     return ReportedSpeech(
         nlp=nlp,
         attr=attr,
         pseudo=pseudo,
```

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/qualifiers/reported_speech/patterns.py` & `edsnlp-0.8.0/edsnlp/pipelines/qualifiers/reported_speech/patterns.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/qualifiers/reported_speech/reported_speech.py` & `edsnlp-0.8.0/edsnlp/pipelines/qualifiers/reported_speech/reported_speech.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Optional
+from typing import List, Optional, Set, Union
 
 from spacy.language import Language
 from spacy.tokens import Doc, Span, Token
 
 from edsnlp.matchers.regex import RegexMatcher
 from edsnlp.pipelines.qualifiers.base import Qualifier
 from edsnlp.utils.filter import consume_spans, filter_spans, get_spans
@@ -27,24 +27,26 @@
         String gathering all quotation cues.
     verbs : List[str]
         List of reported speech verbs.
     following : List[str]
         List of terms following a reported speech.
     preceding : List[str]
         List of terms preceding a reported speech.
-    filter_matches : bool
-        Whether to filter out overlapping matches.
     attr : str
         spaCy's attribute to use:
         a string with the value "TEXT" or "NORM",
         or a dict with the key 'term_attr'
         we can also add a key for each regex.
-    on_ents_only : bool
+    on_ents_only : Union[bool, str, List[str], Set[str]]
         Whether to look for matches around detected entities only.
         Useful for faster inference in downstream tasks.
+
+        - If True, will look in all ents located in `doc.ents` only
+        - If an iterable of string is passed, will additionally look in `doc.spans[key]`
+        for each key in the iterable
     within_ents : bool
         Whether to consider cues within entities.
     explain : bool
         Whether to keep track of cues for each entity.
     """
 
     defaults = dict(
@@ -59,15 +61,15 @@
         nlp: Language,
         attr: str,
         pseudo: Optional[List[str]],
         preceding: Optional[List[str]],
         following: Optional[List[str]],
         quotation: Optional[List[str]],
         verbs: Optional[List[str]],
-        on_ents_only: bool,
+        on_ents_only: Union[bool, str, List[str], Set[str]],
         within_ents: bool,
         explain: bool,
     ):
 
         terms = self.get_defaults(
             pseudo=pseudo,
             preceding=preceding,
@@ -166,15 +168,15 @@
         """
 
         matches = self.get_matches(doc)
         matches += list(self.regex_matcher(doc, as_spans=True))
 
         boundaries = self._boundaries(doc)
 
-        entities = list(doc.ents) + list(doc.spans.get("discarded", []))
+        entities = self.get_spans(doc)
         ents = None
 
         # Removes duplicate matches and pseudo-expressions in one statement
         matches = filter_spans(matches, label_to_remove="pseudo")
 
         for start, end in boundaries:
```

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/terminations.py` & `edsnlp-0.8.0/edsnlp/pipelines/terminations.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/pipelines/trainable/nested_ner.py` & `edsnlp-0.8.0/edsnlp/pipelines/trainable/nested_ner/nested_ner.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,87 +6,27 @@
 from spacy import Language
 from spacy.pipeline import TrainablePipe
 from spacy.tokens import Doc, Span
 from spacy.training import Example
 from spacy.vocab import Vocab
 from thinc.api import Model, Optimizer
 from thinc.backends import NumpyOps
-from thinc.config import Config
 from thinc.model import set_dropout_rate
 from thinc.types import Ints2d
 from wasabi import Printer
 
 from edsnlp.utils.filter import filter_spans
 
 msg = Printer()
 
-
 NUM_INITIALIZATION_EXAMPLES = 1000
 
-
-nested_ner_default_config = """
-[model]
-    @architectures = "eds.stack_crf_ner_model.v1"
-    mode = "joint"
-
-    [model.tok2vec]
-        @architectures = "spacy.Tok2Vec.v1"
-
-    [model.tok2vec.embed]
-        @architectures = "spacy.MultiHashEmbed.v1"
-        width = 96
-        rows = [5000, 2000, 1000, 1000]
-        attrs = ["ORTH", "PREFIX", "SUFFIX", "SHAPE"]
-        include_static_vectors = false
-
-    [model.tok2vec.encode]
-        @architectures = "spacy.MaxoutWindowEncoder.v1"
-        width = ${model.tok2vec.embed.width}
-        window_size = 1
-        maxout_pieces = 3
-        depth = 4
-
-[scorer]
-    @scorers = "eds.nested_ner_scorer.v1"
-"""
-
-NESTED_NER_DEFAULTS = Config().from_str(nested_ner_default_config)
 np_ops = NumpyOps()
 
 
-@Language.factory(
-    "nested_ner",
-    default_config=NESTED_NER_DEFAULTS,
-    requires=["doc.ents", "doc.spans"],
-    assigns=["doc.ents", "doc.spans"],
-    default_score_weights={
-        "ents_f": 1.0,
-        "ents_p": 0.0,
-        "ents_r": 0.0,
-    },
-)
-def create_component(
-    nlp: Language,
-    name: str,
-    model: Model,
-    ent_labels=None,
-    spans_labels=None,
-    scorer=None,
-):
-    """Construct a TrainableQualifier component."""
-    return TrainableNer(
-        vocab=nlp.vocab,
-        model=model,
-        name=name,
-        ent_labels=ent_labels,
-        spans_labels=spans_labels,
-        scorer=scorer,
-    )
-
-
 def nested_ner_scorer(examples: Iterable[Example], **cfg):
     """
     Scores the extracted entities that may be overlapping or nested
     by looking in `doc.ents`, and `doc.spans`.
 
     Parameters
     ----------
```

### Comparing `edsnlp-0.7.4/edsnlp/processing/distributed.py` & `edsnlp-0.8.0/edsnlp/processing/distributed.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/processing/helpers.py` & `edsnlp-0.8.0/edsnlp/processing/helpers.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/processing/parallel.py` & `edsnlp-0.8.0/edsnlp/processing/parallel.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/processing/simple.py` & `edsnlp-0.8.0/edsnlp/processing/simple.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/processing/wrapper.py` & `edsnlp-0.8.0/edsnlp/processing/wrapper.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/resources/cim10.csv.gz` & `edsnlp-0.8.0/edsnlp/resources/cim10.csv.gz`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/resources/drugs.json` & `edsnlp-0.8.0/edsnlp/resources/drugs.json`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/resources/verbs.csv.gz` & `edsnlp-0.8.0/edsnlp/resources/verbs.csv.gz`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/utils/blocs.py` & `edsnlp-0.8.0/edsnlp/utils/blocs.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/utils/colors.py` & `edsnlp-0.8.0/edsnlp/utils/colors.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/utils/deprecation.py` & `edsnlp-0.8.0/edsnlp/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/utils/examples.py` & `edsnlp-0.8.0/edsnlp/utils/examples.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/utils/filter.py` & `edsnlp-0.8.0/edsnlp/utils/filter.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from typing import Any, Callable, Iterable, List, Optional, Tuple, Union
+from typing import Any, Callable, Iterable, List, Optional, Sequence, Tuple, Union
 
 from spacy.tokens import Span
+from spacy.tokens.doc import Doc
 
 
 def default_sort_key(span: Span) -> Tuple[int, int]:
     """
     Returns the sort key for filtering spans.
 
     Parameters
@@ -202,7 +203,104 @@
     List[Span]
         Filtered spans.
     """
     if isinstance(label, int):
         return [span for span in spans if span.label == label]
     else:
         return [span for span in spans if span.label_ == label]
+
+
+def span_f1(a: Span, b: Span) -> float:
+    """
+    Computes the F1 overlap between two spans.
+
+    Parameters
+    ----------
+    a: Span
+        First span
+    b: Span
+        Second span
+
+    Returns
+    -------
+    float
+        F1 overlap
+    """
+    start_a, end_a = a.start, a.end
+    start_b, end_b = b.start, b.end
+    overlap = max(0, min(end_a, end_b) - max(start_a, start_b))
+    return 2 * overlap / (end_a - start_a + end_b - start_b)
+
+
+def align_spans(
+    source: Sequence[Span],
+    target: Sequence[Span],
+    sort_by_overlap: bool = False,
+) -> List[List[Span]]:
+    """
+    Aligns two lists of spans, by matching source spans that overlap target spans.
+    This function is optimized to avoid quadratic complexity.
+
+    Parameters
+    ----------
+    source : List[Span]
+        List of spans to align.
+    target : List[Span]
+        List of spans to align.
+    sort_by_overlap : bool
+        Whether to sort the aligned spans by maximum dice/f1 overlap
+        with the target span.
+
+    Returns
+    -------
+    List[List[Span]]
+        Subset of `source` spans for each target span
+    """
+    source = sorted(source, key=lambda x: (x.start, x.end))
+    target = sorted(target, key=lambda x: (x.start, x.end))
+
+    aligned = [set() for _ in target]
+    source_idx = 0
+    for target_idx in range(len(target)):
+        while source[source_idx].end <= target[target_idx].start:
+            source_idx += 1
+        i = source_idx
+        while i < len(source) and source[i].start <= target[target_idx].end:
+            aligned[target_idx].add(source[i])
+            i += 1
+
+    aligned = [list(span_set) for span_set in aligned]
+
+    # Sort the aligned spans by maximum dice/f1 overlap with the target span
+    if sort_by_overlap:
+        aligned = [
+            sorted(span_set, key=lambda x: span_f1(x, y), reverse=True)
+            for span_set, y in zip(aligned, target)
+        ]
+
+    return aligned
+
+
+def get_span_group(doclike: Union[Doc, Span], group: str) -> List[Span]:
+    """
+    Get the spans of a span group that are contained inside a doclike object.
+
+    Parameters
+    ----------
+    doclike : Union[Doc, Span]
+        Doclike object to act as a mask.
+    group : str
+        Group name from which to get the spans.
+
+    Returns
+    -------
+    List[Span]
+        List of spans.
+    """
+    if isinstance(doclike, Doc):
+        return [span for span in doclike.spans.get(group, ())]
+    else:
+        return [
+            span
+            for span in doclike.doc.spans.get(group, ())
+            if span.start >= doclike.start and span.end <= doclike.end
+        ]
```

### Comparing `edsnlp-0.7.4/edsnlp/utils/inclusion.py` & `edsnlp-0.8.0/edsnlp/utils/inclusion.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/utils/merge_configs.py` & `edsnlp-0.8.0/edsnlp/utils/merge_configs.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/utils/regex.py` & `edsnlp-0.8.0/edsnlp/utils/regex.py`

 * *Files identical despite different names*

### Comparing `edsnlp-0.7.4/edsnlp/utils/resources.py` & `edsnlp-0.8.0/edsnlp/utils/resources.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,7 +51,19 @@
     Dict
     """
 
     with gzip.open(BASE_DIR / "resources" / "adicap.json.gz", "r") as fin:
         decode_dict = json.loads(fin.read().decode("utf-8"))
 
     return decode_dict
+
+
+@lru_cache()
+def get_AVC_care_site(prefix: bool = True):
+    df = pd.read_csv(BASE_DIR / "resources" / "AVC.csv.gz")
+
+    col = (
+        df.care_site_name.str.split(" ").str[:2].str.join(" ")
+        if prefix
+        else df.care_site_name
+    )
+    return set(col.to_list())
```

### Comparing `edsnlp-0.7.4/edsnlp/utils/training.py` & `edsnlp-0.8.0/edsnlp/utils/training.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,16 +187,16 @@
         raise Exception()
 
     if data_format != "spacy" or isinstance(dev_data, (float, int)):
         tmp_path = Path(tempfile.mkdtemp())
         train_path = tmp_path / "train.spacy"
         dev_path = tmp_path / "dev.spacy"
 
-        DocBin(docs=train_docs).to_disk(train_path)
-        DocBin(docs=dev_docs).to_disk(dev_path)
+        DocBin(docs=train_docs, store_user_data=True).to_disk(train_path)
+        DocBin(docs=dev_docs, store_user_data=True).to_disk(dev_path)
     else:
         train_path = train_data
         dev_path = dev_data
 
     return Config().from_str(
         f"""
         [corpora]
```

### Comparing `edsnlp-0.7.4/edsnlp/viz/quick_examples.py` & `edsnlp-0.8.0/edsnlp/viz/quick_examples.py`

 * *Files identical despite different names*

