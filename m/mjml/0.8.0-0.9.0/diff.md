# Comparing `tmp/mjml-0.8.0.tar.gz` & `tmp/mjml-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mjml-0.8.0.tar", last modified: Thu Aug 25 19:08:39 2022, max compression
+gzip compressed data, was "mjml-0.9.0.tar", last modified: Thu May 25 19:41:33 2023, max compression
```

## Comparing `mjml-0.8.0.tar` & `mjml-0.9.0.tar`

### file list

```diff
@@ -1,115 +1,147 @@
-drwxr-xr-x   0 fschwarz  (1004) fschwarz  (1004)        0 2022-08-25 19:08:39.628643 mjml-0.8.0/
-drwxr-xr-x   0 fschwarz  (1004) fschwarz  (1004)        0 2022-08-25 19:08:39.618643 mjml-0.8.0/.github/
-drwxr-xr-x   0 fschwarz  (1004) fschwarz  (1004)        0 2022-08-25 19:08:39.619643 mjml-0.8.0/.github/workflows/
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)      655 2022-08-03 22:19:24.000000 mjml-0.8.0/.github/workflows/tests.yml
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     2228 2022-08-25 19:08:24.000000 mjml-0.8.0/CHANGELOG.md
--rw-rw-r--   0 fschwarz  (1004) fschwarz  (1004)     1128 2020-06-09 12:33:50.000000 mjml-0.8.0/LICENSE.txt
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)      122 2022-08-25 12:38:10.000000 mjml-0.8.0/MANIFEST.in
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     4834 2022-08-25 19:08:39.628643 mjml-0.8.0/PKG-INFO
--rw-rw-r--   0 fschwarz  (1004) fschwarz  (1004)     3729 2022-08-03 22:24:43.000000 mjml-0.8.0/README.md
--rw-rw-r--   0 fschwarz  (1004) fschwarz  (1004)        6 2022-08-25 19:06:51.000000 mjml-0.8.0/VERSION.txt
-drwxr-xr-x   0 fschwarz  (1004) fschwarz  (1004)        0 2022-08-25 19:08:39.619643 mjml-0.8.0/mjml/
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)       38 2020-06-09 13:05:12.000000 mjml-0.8.0/mjml/__init__.py
-drwxr-xr-x   0 fschwarz  (1004) fschwarz  (1004)        0 2022-08-25 19:08:39.620643 mjml-0.8.0/mjml/core/
--rw-rw-r--   0 fschwarz  (1004) fschwarz  (1004)       20 2020-06-11 12:30:44.000000 mjml-0.8.0/mjml/core/__init__.py
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     2633 2022-08-22 08:39:21.000000 mjml-0.8.0/mjml/core/api.py
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)      828 2021-01-20 20:36:30.000000 mjml-0.8.0/mjml/core/registry.py
-drwxr-xr-x   0 fschwarz  (1004) fschwarz  (1004)        0 2022-08-25 19:08:39.622643 mjml-0.8.0/mjml/elements/
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)      243 2021-01-20 20:36:30.000000 mjml-0.8.0/mjml/elements/__init__.py
--rw-rw-r--   0 fschwarz  (1004) fschwarz  (1004)     5375 2022-06-07 20:37:41.000000 mjml-0.8.0/mjml/elements/_base.py
-drwxr-xr-x   0 fschwarz  (1004) fschwarz  (1004)        0 2022-08-25 19:08:39.622643 mjml-0.8.0/mjml/elements/head/
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)      150 2021-01-20 20:36:30.000000 mjml-0.8.0/mjml/elements/head/__init__.py
--rw-rw-r--   0 fschwarz  (1004) fschwarz  (1004)      942 2021-03-31 09:08:18.000000 mjml-0.8.0/mjml/elements/head/_head_base.py
--rw-rw-r--   0 fschwarz  (1004) fschwarz  (1004)     1332 2020-08-18 10:46:39.000000 mjml-0.8.0/mjml/elements/head/mj_attributes.py
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)      382 2021-01-20 20:36:30.000000 mjml-0.8.0/mjml/elements/head/mj_font.py
--rw-rw-r--   0 fschwarz  (1004) fschwarz  (1004)      154 2020-06-11 12:30:44.000000 mjml-0.8.0/mjml/elements/head/mj_head.py
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)      199 2021-01-20 20:36:30.000000 mjml-0.8.0/mjml/elements/head/mj_preview.py
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)      397 2022-08-03 22:19:24.000000 mjml-0.8.0/mjml/elements/head/mj_style.py
--rw-rw-r--   0 fschwarz  (1004) fschwarz  (1004)      192 2020-06-11 12:30:44.000000 mjml-0.8.0/mjml/elements/head/mj_title.py
--rw-rw-r--   0 fschwarz  (1004) fschwarz  (1004)     1027 2021-03-31 09:08:18.000000 mjml-0.8.0/mjml/elements/mj_body.py
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     6924 2022-06-07 20:38:52.000000 mjml-0.8.0/mjml/elements/mj_button.py
--rw-rw-r--   0 fschwarz  (1004) fschwarz  (1004)     9435 2022-06-07 20:17:08.000000 mjml-0.8.0/mjml/elements/mj_column.py
--rw-rw-r--   0 fschwarz  (1004) fschwarz  (1004)     3052 2021-04-01 08:06:25.000000 mjml-0.8.0/mjml/elements/mj_divider.py
--rw-rw-r--   0 fschwarz  (1004) fschwarz  (1004)     6035 2020-08-19 12:35:03.000000 mjml-0.8.0/mjml/elements/mj_group.py
--rw-rw-r--   0 fschwarz  (1004) fschwarz  (1004)     6158 2021-04-05 19:58:29.000000 mjml-0.8.0/mjml/elements/mj_image.py
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)      164 2021-01-20 20:36:30.000000 mjml-0.8.0/mjml/elements/mj_raw.py
--rw-rw-r--   0 fschwarz  (1004) fschwarz  (1004)    14588 2022-03-24 13:50:45.000000 mjml-0.8.0/mjml/elements/mj_section.py
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     2813 2022-08-22 08:39:21.000000 mjml-0.8.0/mjml/elements/mj_table.py
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     2822 2022-08-22 08:39:36.000000 mjml-0.8.0/mjml/elements/mj_text.py
-drwxr-xr-x   0 fschwarz  (1004) fschwarz  (1004)        0 2022-08-25 19:08:39.623643 mjml-0.8.0/mjml/helpers/
--rw-rw-r--   0 fschwarz  (1004) fschwarz  (1004)      312 2021-03-03 17:22:31.000000 mjml-0.8.0/mjml/helpers/__init__.py
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)      834 2020-05-26 10:35:34.000000 mjml-0.8.0/mjml/helpers/conditional_tag.py
--rw-rw-r--   0 fschwarz  (1004) fschwarz  (1004)     1078 2021-03-31 09:08:18.000000 mjml-0.8.0/mjml/helpers/fonts.py
--rw-rw-r--   0 fschwarz  (1004) fschwarz  (1004)     1341 2021-03-04 08:13:25.000000 mjml-0.8.0/mjml/helpers/json_to_xml.py
--rw-rw-r--   0 fschwarz  (1004) fschwarz  (1004)      984 2021-04-01 08:06:25.000000 mjml-0.8.0/mjml/helpers/media_queries.py
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)      341 2021-01-25 21:13:23.000000 mjml-0.8.0/mjml/helpers/mergeOutlookConditionals.py
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)      272 2020-05-26 20:57:05.000000 mjml-0.8.0/mjml/helpers/preview.py
--rw-rw-r--   0 fschwarz  (1004) fschwarz  (1004)     1212 2022-03-18 13:53:18.000000 mjml-0.8.0/mjml/helpers/py_utils.py
--rw-rw-r--   0 fschwarz  (1004) fschwarz  (1004)     1156 2021-01-25 21:13:33.000000 mjml-0.8.0/mjml/helpers/shorthand_parser.py
--rw-rw-r--   0 fschwarz  (1004) fschwarz  (1004)     3936 2022-03-24 13:50:45.000000 mjml-0.8.0/mjml/helpers/skeleton.py
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)      263 2020-05-28 09:28:14.000000 mjml-0.8.0/mjml/helpers/suffixCssClasses.py
--rw-rw-r--   0 fschwarz  (1004) fschwarz  (1004)     1164 2021-01-25 21:13:40.000000 mjml-0.8.0/mjml/helpers/width_parser.py
-drwxr-xr-x   0 fschwarz  (1004) fschwarz  (1004)        0 2022-08-25 19:08:39.624643 mjml-0.8.0/mjml/lib/
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)       58 2020-05-26 14:24:50.000000 mjml-0.8.0/mjml/lib/__init__.py
--rw-rw-r--   0 fschwarz  (1004) fschwarz  (1004)      795 2020-05-22 10:23:08.000000 mjml-0.8.0/mjml/lib/attribute_dict.py
--rw-rw-r--   0 fschwarz  (1004) fschwarz  (1004)      933 2020-08-17 10:49:53.000000 mjml-0.8.0/mjml/lib/dict_merger.py
-drwxr-xr-x   0 fschwarz  (1004) fschwarz  (1004)        0 2022-08-25 19:08:39.624643 mjml-0.8.0/mjml/lib/tests/
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)        0 2020-05-26 10:22:39.000000 mjml-0.8.0/mjml/lib/tests/__init__.py
--rw-rw-r--   0 fschwarz  (1004) fschwarz  (1004)      758 2020-06-08 14:29:56.000000 mjml-0.8.0/mjml/lib/tests/dict_merger_test.py
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)    10207 2022-08-22 08:39:21.000000 mjml-0.8.0/mjml/mjml2html.py
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)      383 2021-09-17 21:08:18.000000 mjml-0.8.0/mjml/parser.py
-drwxr-xr-x   0 fschwarz  (1004) fschwarz  (1004)        0 2022-08-25 19:08:39.624643 mjml-0.8.0/mjml/scripts/
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)        0 2020-08-18 14:26:35.000000 mjml-0.8.0/mjml/scripts/__init__.py
--rw-rw-r--   0 fschwarz  (1004) fschwarz  (1004)      471 2020-08-19 08:16:31.000000 mjml-0.8.0/mjml/scripts/mjml-html-compare
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     1396 2021-03-23 16:17:05.000000 mjml-0.8.0/mjml/scripts/mjml.py
-drwxr-xr-x   0 fschwarz  (1004) fschwarz  (1004)        0 2022-08-25 19:08:39.620643 mjml-0.8.0/mjml.egg-info/
--rw-rw-r--   0 fschwarz  (1004) fschwarz  (1004)     4834 2022-08-25 19:08:39.000000 mjml-0.8.0/mjml.egg-info/PKG-INFO
--rw-rw-r--   0 fschwarz  (1004) fschwarz  (1004)     3184 2022-08-25 19:08:39.000000 mjml-0.8.0/mjml.egg-info/SOURCES.txt
--rw-rw-r--   0 fschwarz  (1004) fschwarz  (1004)        1 2022-08-25 19:08:39.000000 mjml-0.8.0/mjml.egg-info/dependency_links.txt
--rw-rw-r--   0 fschwarz  (1004) fschwarz  (1004)       49 2022-08-25 19:08:39.000000 mjml-0.8.0/mjml.egg-info/entry_points.txt
--rw-rw-r--   0 fschwarz  (1004) fschwarz  (1004)      126 2022-08-25 19:08:39.000000 mjml-0.8.0/mjml.egg-info/requires.txt
--rw-rw-r--   0 fschwarz  (1004) fschwarz  (1004)        5 2022-08-25 19:08:39.000000 mjml-0.8.0/mjml.egg-info/top_level.txt
--rw-rw-r--   0 fschwarz  (1004) fschwarz  (1004)        1 2020-08-20 14:41:40.000000 mjml-0.8.0/mjml.egg-info/zip-safe
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     1487 2022-08-25 19:08:39.628643 mjml-0.8.0/setup.cfg
--rw-rw-r--   0 fschwarz  (1004) fschwarz  (1004)       63 2020-10-29 10:48:03.000000 mjml-0.8.0/setup.py
-drwxr-xr-x   0 fschwarz  (1004) fschwarz  (1004)        0 2022-08-25 19:08:39.625643 mjml-0.8.0/tests/
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)      197 2021-01-13 15:45:19.000000 mjml-0.8.0/tests/border_parser_test.py
--rw-rw-r--   0 fschwarz  (1004) fschwarz  (1004)      872 2021-06-01 09:01:10.000000 mjml-0.8.0/tests/includes_with_umlauts_test.py
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     1562 2022-08-22 08:39:21.000000 mjml-0.8.0/tests/missing_functionality_test.py
--rw-rw-r--   0 fschwarz  (1004) fschwarz  (1004)     1166 2022-03-18 12:14:32.000000 mjml-0.8.0/tests/mj_button_mailto_link_test.py
--rw-rw-r--   0 fschwarz  (1004) fschwarz  (1004)      362 2020-08-18 10:46:42.000000 mjml-0.8.0/tests/mjml2html_test.py
-drwxr-xr-x   0 fschwarz  (1004) fschwarz  (1004)        0 2022-08-25 19:08:39.628643 mjml-0.8.0/tests/testdata/
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     4451 2022-08-25 19:05:45.000000 mjml-0.8.0/tests/testdata/button-expected.html
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     5074 2022-08-25 19:05:46.000000 mjml-0.8.0/tests/testdata/css-inlining-expected.html
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     5039 2022-08-25 19:05:46.000000 mjml-0.8.0/tests/testdata/hello-world-expected.html
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     3814 2022-08-25 19:05:47.000000 mjml-0.8.0/tests/testdata/html-entities-expected.html
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     3723 2022-08-25 19:05:46.000000 mjml-0.8.0/tests/testdata/html-without-closing-tag-expected.html
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     3723 2022-08-25 19:05:47.000000 mjml-0.8.0/tests/testdata/minimal-expected.html
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     3723 2022-08-25 19:05:45.000000 mjml-0.8.0/tests/testdata/missing-whitespace-before-tag-expected.html
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     3406 2022-08-25 19:05:45.000000 mjml-0.8.0/tests/testdata/mj-attributes-expected.html
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     3773 2022-08-25 19:05:46.000000 mjml-0.8.0/tests/testdata/mj-body-with-background-color-expected.html
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     4470 2022-08-25 19:05:46.000000 mjml-0.8.0/tests/testdata/mj-button-with-width-expected.html
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     4095 2022-08-25 19:05:46.000000 mjml-0.8.0/tests/testdata/mj-column-with-attributes-expected.html
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     3668 2022-08-25 19:05:46.000000 mjml-0.8.0/tests/testdata/mj-font-expected.html
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     3834 2022-08-25 19:05:45.000000 mjml-0.8.0/tests/testdata/mj-font-multiple-expected.html
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     3417 2022-08-25 19:05:46.000000 mjml-0.8.0/tests/testdata/mj-font-unused-expected.html
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     7417 2022-08-25 19:05:47.000000 mjml-0.8.0/tests/testdata/mj-group-expected.html
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     1497 2022-08-25 19:05:45.000000 mjml-0.8.0/tests/testdata/mj-head-with-comment-expected.html
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     4105 2022-08-25 19:05:46.000000 mjml-0.8.0/tests/testdata/mj-image-with-empty-alt-attribute-expected.html
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     4215 2022-08-25 19:05:45.000000 mjml-0.8.0/tests/testdata/mj-image-with-href-expected.html
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     6911 2022-08-25 19:05:46.000000 mjml-0.8.0/tests/testdata/mj-include-body-expected.html
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     3867 2022-08-25 19:05:46.000000 mjml-0.8.0/tests/testdata/mj-preview-expected.html
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     1512 2022-08-25 19:05:45.000000 mjml-0.8.0/tests/testdata/mj-raw-expected.html
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     3754 2022-08-25 19:05:45.000000 mjml-0.8.0/tests/testdata/mj-raw-head-expected.html
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     3559 2022-08-25 19:05:46.000000 mjml-0.8.0/tests/testdata/mj-raw-head-with-tags-expected.html
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     1568 2022-08-25 19:05:47.000000 mjml-0.8.0/tests/testdata/mj-raw-with-tags-expected.html
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     4437 2022-08-25 19:05:45.000000 mjml-0.8.0/tests/testdata/mj-section-with-background-url-expected.html
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     3813 2022-08-25 19:05:47.000000 mjml-0.8.0/tests/testdata/mj-section-with-mj-class-expected.html
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     3848 2022-08-25 19:05:47.000000 mjml-0.8.0/tests/testdata/mj-style-expected.html
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     4744 2022-08-25 19:05:45.000000 mjml-0.8.0/tests/testdata/mj-table-expected.html
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     3728 2022-08-25 19:05:45.000000 mjml-0.8.0/tests/testdata/mj-text-with-tail-text-expected.html
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     3729 2022-08-25 19:05:47.000000 mjml-0.8.0/tests/testdata/mj-title-expected.html
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     3547 2022-08-25 19:05:45.000000 mjml-0.8.0/tests/testdata/text_with_html-expected.html
--rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     4074 2022-08-22 09:04:27.000000 mjml-0.8.0/tests/upstream_alignment_test.py
-drwxr-xr-x   0 fschwarz  (1004) fschwarz  (1004)        0 2022-08-25 19:08:39.628643 mjml-0.8.0/tools/
--rwxr-xr-x   0 fschwarz  (1004) fschwarz  (1004)     2834 2022-08-25 12:35:48.000000 mjml-0.8.0/tools/update-expected-html.py
+drwxr-xr-x   0 fschwarz  (1004) fschwarz  (1004)        0 2023-05-25 19:41:33.933149 mjml-0.9.0/
+drwxr-xr-x   0 fschwarz  (1004) fschwarz  (1004)        0 2023-05-25 19:41:33.915149 mjml-0.9.0/.github/
+drwxr-xr-x   0 fschwarz  (1004) fschwarz  (1004)        0 2023-05-25 19:41:33.917149 mjml-0.9.0/.github/workflows/
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)      785 2023-05-24 19:42:32.000000 mjml-0.9.0/.github/workflows/tests.yml
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     2688 2023-05-25 19:39:59.000000 mjml-0.9.0/CHANGELOG.md
+-rw-rw-r--   0 fschwarz  (1004) fschwarz  (1004)     1128 2020-06-09 12:33:50.000000 mjml-0.9.0/LICENSE.txt
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)      121 2023-05-24 19:42:32.000000 mjml-0.9.0/MANIFEST.in
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     5180 2023-05-25 19:41:33.933149 mjml-0.9.0/PKG-INFO
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     4038 2023-05-25 19:38:12.000000 mjml-0.9.0/README.md
+-rw-rw-r--   0 fschwarz  (1004) fschwarz  (1004)        6 2023-05-25 19:39:22.000000 mjml-0.9.0/VERSION.txt
+drwxr-xr-x   0 fschwarz  (1004) fschwarz  (1004)        0 2023-05-25 19:41:33.918149 mjml-0.9.0/mjml/
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)       60 2023-05-24 19:42:32.000000 mjml-0.9.0/mjml/__init__.py
+drwxr-xr-x   0 fschwarz  (1004) fschwarz  (1004)        0 2023-05-25 19:41:33.919149 mjml-0.9.0/mjml/core/
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)       20 2023-02-18 20:41:15.000000 mjml-0.9.0/mjml/core/__init__.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     2740 2023-05-24 19:42:32.000000 mjml-0.9.0/mjml/core/api.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     1675 2023-05-25 19:13:21.000000 mjml-0.9.0/mjml/core/registry.py
+drwxr-xr-x   0 fschwarz  (1004) fschwarz  (1004)        0 2023-05-25 19:41:33.922150 mjml-0.9.0/mjml/elements/
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)      621 2023-05-25 19:13:21.000000 mjml-0.9.0/mjml/elements/__init__.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     5540 2023-05-25 19:13:21.000000 mjml-0.9.0/mjml/elements/_base.py
+drwxr-xr-x   0 fschwarz  (1004) fschwarz  (1004)        0 2023-05-25 19:41:33.923149 mjml-0.9.0/mjml/elements/head/
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)      213 2023-05-25 19:13:21.000000 mjml-0.9.0/mjml/elements/head/__init__.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)      941 2023-05-24 19:42:32.000000 mjml-0.9.0/mjml/elements/head/_head_base.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     1370 2023-05-24 19:42:32.000000 mjml-0.9.0/mjml/elements/head/mj_attributes.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)      360 2023-02-18 20:41:15.000000 mjml-0.9.0/mjml/elements/head/mj_breakpoint.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)      414 2023-02-18 20:41:15.000000 mjml-0.9.0/mjml/elements/head/mj_font.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)      185 2023-05-24 19:42:32.000000 mjml-0.9.0/mjml/elements/head/mj_head.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)      899 2023-05-25 19:13:21.000000 mjml-0.9.0/mjml/elements/head/mj_html_attributes.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)      233 2023-02-18 20:41:15.000000 mjml-0.9.0/mjml/elements/head/mj_preview.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)      429 2023-05-24 19:42:32.000000 mjml-0.9.0/mjml/elements/head/mj_style.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)      224 2023-05-24 19:42:32.000000 mjml-0.9.0/mjml/elements/head/mj_title.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     4995 2023-05-25 19:13:21.000000 mjml-0.9.0/mjml/elements/mj_accordion.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     3821 2023-05-25 19:13:21.000000 mjml-0.9.0/mjml/elements/mj_accordion_element.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     2797 2023-05-25 19:13:21.000000 mjml-0.9.0/mjml/elements/mj_accordion_text.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     4072 2023-05-25 19:13:21.000000 mjml-0.9.0/mjml/elements/mj_accordion_title.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     1058 2023-05-24 19:42:32.000000 mjml-0.9.0/mjml/elements/mj_body.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     6939 2023-05-24 19:42:32.000000 mjml-0.9.0/mjml/elements/mj_button.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)    12679 2023-05-25 19:13:21.000000 mjml-0.9.0/mjml/elements/mj_carousel.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     4937 2023-05-25 19:13:21.000000 mjml-0.9.0/mjml/elements/mj_carousel_image.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     9676 2023-05-24 19:42:32.000000 mjml-0.9.0/mjml/elements/mj_column.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     3107 2023-05-24 19:42:32.000000 mjml-0.9.0/mjml/elements/mj_divider.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     6175 2023-05-24 19:42:32.000000 mjml-0.9.0/mjml/elements/mj_group.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)    12572 2023-05-25 19:13:21.000000 mjml-0.9.0/mjml/elements/mj_hero.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     6190 2023-05-24 19:42:32.000000 mjml-0.9.0/mjml/elements/mj_image.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     6717 2023-05-24 19:42:32.000000 mjml-0.9.0/mjml/elements/mj_navbar.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     4079 2023-05-24 19:42:32.000000 mjml-0.9.0/mjml/elements/mj_navbar_link.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)      195 2023-02-18 20:41:15.000000 mjml-0.9.0/mjml/elements/mj_raw.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)    15358 2023-05-24 19:42:32.000000 mjml-0.9.0/mjml/elements/mj_section.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     5187 2023-05-25 19:13:21.000000 mjml-0.9.0/mjml/elements/mj_social.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     9958 2023-05-25 19:13:21.000000 mjml-0.9.0/mjml/elements/mj_social_element.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     1286 2023-02-18 20:41:15.000000 mjml-0.9.0/mjml/elements/mj_spacer.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     2845 2023-05-24 19:42:32.000000 mjml-0.9.0/mjml/elements/mj_table.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     2875 2023-05-24 19:42:32.000000 mjml-0.9.0/mjml/elements/mj_text.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     1102 2023-05-24 19:42:32.000000 mjml-0.9.0/mjml/elements/mj_wrapper.py
+drwxr-xr-x   0 fschwarz  (1004) fschwarz  (1004)        0 2023-05-25 19:41:33.925150 mjml-0.9.0/mjml/helpers/
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)      312 2023-02-18 20:41:15.000000 mjml-0.9.0/mjml/helpers/__init__.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)      833 2023-05-24 19:42:32.000000 mjml-0.9.0/mjml/helpers/conditional_tag.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     1077 2023-05-24 19:42:32.000000 mjml-0.9.0/mjml/helpers/fonts.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     1343 2023-05-25 19:15:03.000000 mjml-0.9.0/mjml/helpers/json_to_xml.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)      983 2023-05-24 19:42:32.000000 mjml-0.9.0/mjml/helpers/media_queries.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)      341 2023-05-24 19:42:32.000000 mjml-0.9.0/mjml/helpers/mergeOutlookConditionals.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)      293 2023-05-24 19:42:32.000000 mjml-0.9.0/mjml/helpers/preview.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     1211 2023-05-24 19:42:32.000000 mjml-0.9.0/mjml/helpers/py_utils.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     1155 2023-05-24 19:42:32.000000 mjml-0.9.0/mjml/helpers/shorthand_parser.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     3957 2023-05-24 19:42:32.000000 mjml-0.9.0/mjml/helpers/skeleton.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)      262 2023-05-24 19:42:32.000000 mjml-0.9.0/mjml/helpers/suffixCssClasses.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     1163 2023-05-24 19:42:32.000000 mjml-0.9.0/mjml/helpers/width_parser.py
+drwxr-xr-x   0 fschwarz  (1004) fschwarz  (1004)        0 2023-05-25 19:41:33.925150 mjml-0.9.0/mjml/lib/
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)       58 2023-02-18 20:41:15.000000 mjml-0.9.0/mjml/lib/__init__.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)      866 2023-05-24 19:42:32.000000 mjml-0.9.0/mjml/lib/attribute_dict.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)      932 2023-05-24 19:42:32.000000 mjml-0.9.0/mjml/lib/dict_merger.py
+drwxr-xr-x   0 fschwarz  (1004) fschwarz  (1004)        0 2023-05-25 19:41:33.925150 mjml-0.9.0/mjml/lib/tests/
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)        0 2023-02-18 20:41:15.000000 mjml-0.9.0/mjml/lib/tests/__init__.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)      758 2023-05-24 19:42:32.000000 mjml-0.9.0/mjml/lib/tests/dict_merger_test.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)    11239 2023-05-25 19:13:21.000000 mjml-0.9.0/mjml/mjml2html.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)      383 2023-02-21 08:27:37.000000 mjml-0.9.0/mjml/parser.py
+drwxr-xr-x   0 fschwarz  (1004) fschwarz  (1004)        0 2023-05-25 19:41:33.926149 mjml-0.9.0/mjml/scripts/
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)        0 2023-02-18 20:41:15.000000 mjml-0.9.0/mjml/scripts/__init__.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)      470 2023-05-24 19:42:32.000000 mjml-0.9.0/mjml/scripts/mjml-html-compare
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     1414 2023-05-24 19:42:32.000000 mjml-0.9.0/mjml/scripts/mjml.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)      614 2023-05-24 19:42:32.000000 mjml-0.9.0/mjml/testing_helpers.py
+drwxr-xr-x   0 fschwarz  (1004) fschwarz  (1004)        0 2023-05-25 19:41:33.918149 mjml-0.9.0/mjml.egg-info/
+-rw-rw-r--   0 fschwarz  (1004) fschwarz  (1004)     5180 2023-05-25 19:41:33.000000 mjml-0.9.0/mjml.egg-info/PKG-INFO
+-rw-rw-r--   0 fschwarz  (1004) fschwarz  (1004)     4319 2023-05-25 19:41:33.000000 mjml-0.9.0/mjml.egg-info/SOURCES.txt
+-rw-rw-r--   0 fschwarz  (1004) fschwarz  (1004)        1 2023-05-25 19:41:33.000000 mjml-0.9.0/mjml.egg-info/dependency_links.txt
+-rw-rw-r--   0 fschwarz  (1004) fschwarz  (1004)       48 2023-05-25 19:41:33.000000 mjml-0.9.0/mjml.egg-info/entry_points.txt
+-rw-rw-r--   0 fschwarz  (1004) fschwarz  (1004)      126 2023-05-25 19:41:33.000000 mjml-0.9.0/mjml.egg-info/requires.txt
+-rw-rw-r--   0 fschwarz  (1004) fschwarz  (1004)        5 2023-05-25 19:41:33.000000 mjml-0.9.0/mjml.egg-info/top_level.txt
+-rw-rw-r--   0 fschwarz  (1004) fschwarz  (1004)        1 2020-08-20 14:41:40.000000 mjml-0.9.0/mjml.egg-info/zip-safe
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)      873 2023-05-25 19:13:21.000000 mjml-0.9.0/pyproject.toml
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     1533 2023-05-25 19:41:33.933149 mjml-0.9.0/setup.cfg
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)       63 2023-05-24 19:42:32.000000 mjml-0.9.0/setup.py
+drwxr-xr-x   0 fschwarz  (1004) fschwarz  (1004)        0 2023-05-25 19:41:33.927149 mjml-0.9.0/tests/
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)        0 2023-02-18 20:41:15.000000 mjml-0.9.0/tests/__init__.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)      195 2023-05-24 19:42:32.000000 mjml-0.9.0/tests/border_parser_test.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     1252 2023-02-18 20:41:15.000000 mjml-0.9.0/tests/custom_components_test.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)      870 2023-05-24 19:42:32.000000 mjml-0.9.0/tests/includes_with_umlauts_test.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     1656 2023-05-24 19:42:32.000000 mjml-0.9.0/tests/missing_functionality_test.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     1164 2023-05-24 19:42:32.000000 mjml-0.9.0/tests/mj_button_mailto_link_test.py
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)      360 2023-05-24 19:42:32.000000 mjml-0.9.0/tests/mjml2html_test.py
+drwxr-xr-x   0 fschwarz  (1004) fschwarz  (1004)        0 2023-05-25 19:41:33.932150 mjml-0.9.0/tests/testdata/
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     4183 2023-02-18 20:19:21.000000 mjml-0.9.0/tests/testdata/_custom-expected.html
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     4448 2023-05-25 19:13:21.000000 mjml-0.9.0/tests/testdata/button-expected.html
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     5071 2023-05-25 19:13:21.000000 mjml-0.9.0/tests/testdata/css-inlining-expected.html
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     5036 2023-05-25 19:13:21.000000 mjml-0.9.0/tests/testdata/hello-world-expected.html
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     3811 2023-05-25 19:13:21.000000 mjml-0.9.0/tests/testdata/html-entities-expected.html
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     3720 2023-05-25 19:13:21.000000 mjml-0.9.0/tests/testdata/html-without-closing-tag-expected.html
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     3720 2023-05-25 19:13:21.000000 mjml-0.9.0/tests/testdata/minimal-expected.html
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     3720 2023-05-25 19:13:21.000000 mjml-0.9.0/tests/testdata/missing-whitespace-before-tag-expected.html
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)    11231 2023-05-25 19:13:21.000000 mjml-0.9.0/tests/testdata/mj-accordion-expected.html
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     3403 2023-05-25 19:13:21.000000 mjml-0.9.0/tests/testdata/mj-attributes-expected.html
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     3770 2023-05-25 19:13:21.000000 mjml-0.9.0/tests/testdata/mj-body-with-background-color-expected.html
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     3717 2023-05-25 19:13:21.000000 mjml-0.9.0/tests/testdata/mj-breakpoint-expected.html
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     4467 2023-05-25 19:13:21.000000 mjml-0.9.0/tests/testdata/mj-button-with-width-expected.html
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)    14764 2023-05-25 19:13:21.000000 mjml-0.9.0/tests/testdata/mj-carousel-expected.html
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     4092 2023-05-25 19:13:21.000000 mjml-0.9.0/tests/testdata/mj-column-with-attributes-expected.html
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     3665 2023-05-25 19:13:21.000000 mjml-0.9.0/tests/testdata/mj-font-expected.html
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     3831 2023-05-25 19:13:21.000000 mjml-0.9.0/tests/testdata/mj-font-multiple-expected.html
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     3414 2023-05-25 19:13:21.000000 mjml-0.9.0/tests/testdata/mj-font-unused-expected.html
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     7414 2023-05-25 19:13:21.000000 mjml-0.9.0/tests/testdata/mj-group-expected.html
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     1494 2023-05-25 19:13:21.000000 mjml-0.9.0/tests/testdata/mj-head-with-comment-expected.html
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     5410 2023-05-25 19:13:21.000000 mjml-0.9.0/tests/testdata/mj-hero-fixed-expected.html
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     5565 2023-05-25 19:13:21.000000 mjml-0.9.0/tests/testdata/mj-hero-fluid-expected.html
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     4145 2023-05-25 19:13:21.000000 mjml-0.9.0/tests/testdata/mj-html-attributes-expected.html
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     4102 2023-05-25 19:13:21.000000 mjml-0.9.0/tests/testdata/mj-image-with-empty-alt-attribute-expected.html
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     4212 2023-05-25 19:13:21.000000 mjml-0.9.0/tests/testdata/mj-image-with-href-expected.html
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     6908 2023-05-25 19:13:21.000000 mjml-0.9.0/tests/testdata/mj-include-body-expected.html
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     7555 2023-05-25 19:13:21.000000 mjml-0.9.0/tests/testdata/mj-navbar-expected.html
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     3862 2023-05-25 19:13:21.000000 mjml-0.9.0/tests/testdata/mj-preview-expected.html
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     1509 2023-05-25 19:13:21.000000 mjml-0.9.0/tests/testdata/mj-raw-expected.html
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     3751 2023-05-25 19:13:21.000000 mjml-0.9.0/tests/testdata/mj-raw-head-expected.html
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     3556 2023-05-25 19:13:21.000000 mjml-0.9.0/tests/testdata/mj-raw-head-with-tags-expected.html
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     1565 2023-05-25 19:13:21.000000 mjml-0.9.0/tests/testdata/mj-raw-with-tags-expected.html
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     4434 2023-05-25 19:13:21.000000 mjml-0.9.0/tests/testdata/mj-section-with-background-url-expected.html
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     3757 2023-05-24 19:42:32.000000 mjml-0.9.0/tests/testdata/mj-section-with-css-class-expected.html
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     7790 2023-05-24 19:42:32.000000 mjml-0.9.0/tests/testdata/mj-section-with-full-width-expected.html
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     3810 2023-05-25 19:13:21.000000 mjml-0.9.0/tests/testdata/mj-section-with-mj-class-expected.html
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     8977 2023-05-25 19:13:21.000000 mjml-0.9.0/tests/testdata/mj-social-expected.html
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     4278 2023-05-25 19:13:21.000000 mjml-0.9.0/tests/testdata/mj-spacer-expected.html
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     3845 2023-05-25 19:13:21.000000 mjml-0.9.0/tests/testdata/mj-style-expected.html
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     4741 2023-05-25 19:13:21.000000 mjml-0.9.0/tests/testdata/mj-table-expected.html
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     3725 2023-05-25 19:13:21.000000 mjml-0.9.0/tests/testdata/mj-text-with-tail-text-expected.html
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     3727 2023-05-25 19:13:21.000000 mjml-0.9.0/tests/testdata/mj-title-expected.html
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     7921 2023-05-25 19:13:21.000000 mjml-0.9.0/tests/testdata/mj-wrapper-expected.html
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     3544 2023-05-25 19:13:21.000000 mjml-0.9.0/tests/testdata/text_with_html-expected.html
+-rw-r--r--   0 fschwarz  (1004) fschwarz  (1004)     5818 2023-05-25 19:13:21.000000 mjml-0.9.0/tests/upstream_alignment_test.py
+drwxr-xr-x   0 fschwarz  (1004) fschwarz  (1004)        0 2023-05-25 19:41:33.932150 mjml-0.9.0/tools/
+-rwxr-xr-x   0 fschwarz  (1004) fschwarz  (1004)     2833 2023-05-24 19:42:32.000000 mjml-0.9.0/tools/update-expected-html.py
```

### Comparing `mjml-0.8.0/CHANGELOG.md` & `mjml-0.9.0/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,17 @@
 
+0.9.0 (2023-05-25)
+------------------
+
+- add mjml-accordion, mjml-accordion-element, mjml-accordion-text, mjml-accordion-title, mjml-carousel, mjml-head-breakpoint, mjml-hero, mjml-navbar, mjml-navbar-link, mjml-social, mjml-spacer, and mjml-wrapper components (Casey Holzer)
+- add support for custom components (Casey Holzer)
+- add support for full-width attribute to mj-section (Casey Holzer)
+- renamed project to "mjml-python", dropping the "-stub" suffix
+
+
 0.8.0 (2022-08-25)
 ------------------
 
 - parse MJML using BeautifulSoup4 which fixes several issues with HTML inside
   `mj-text` (e.g. HTML entities, missing white space) (Casey Holzer)
 - prevent exception when trying to set padding for `<mj-column>` (reported by Peter Coles)
 - fix setting `width` attribute for `mj-button` (spotted by Michael Romanenko)
@@ -72,8 +81,7 @@
 - mjml: always return "binary" data (UTF-8) to avoid encoding problems in Windows
 
 
 0.5.1 (2021-08-20)
 ------------------
 
 - mjml script: use setuptools-based wrapper so Windows users can run it more easily
-
```

### Comparing `mjml-0.8.0/LICENSE.txt` & `mjml-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mjml-0.8.0/PKG-INFO` & `mjml-0.9.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,70 +1,88 @@
 Metadata-Version: 2.1
 Name: mjml
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python implementation for MJML - a framework that makes responsive-email easy
-Home-page: https://github.com/FelixSchwarz/mjml-stub
+Home-page: https://github.com/FelixSchwarz/mjml-python
 Author: Felix Schwarz
 Author-email: felix.schwarz@oss.schwarz.eu
 License: MIT
-Project-URL: Code, https://github.com/FelixSchwarz/mjml-stub
-Project-URL: Issue tracker, https://github.com/FelixSchwarz/mjml-stub/issues
-Platform: UNKNOWN
+Project-URL: Code, https://github.com/FelixSchwarz/mjml-python
+Project-URL: Issue tracker, https://github.com/FelixSchwarz/mjml-python/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Communications :: Email
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 Provides-Extra: css_inlining
 License-File: LICENSE.txt
 
-mjml-stub
-=============
+# mjml-python
 
 This is an unofficial Python port of [mjml v4](https://github.com/mjmlio/mjml). It is implemented in pure Python and does not require JavaScript/NodeJS. mjml is a markup language created by [Mailjet](https://www.mailjet.com/) and designed to reduce the pain of coding a responsive email.
 
-    pip install mjml
+### Installation
 
+```sh
+pip install mjml
+```
+
+### Usage
+
+```py
+from mjml import mjml_to_html
+with open('foo.mjml', 'rb') as mjml_fp:
+    result = mjml_to_html(mjml_fp)
+assert not result.errors
+html: str = result.html
+```
+
+Alternatively you can run the code from the CLI:
+
+```sh
+$ mjml foo.mjml
+```
+
+
+## Limitations
 
-WARNING: stub implementation only!
-------------------------------------
 This library only implements a subset of the original MJML project. It lacks several features found in the JavaScript mjml implementation (e.g. minification, beautification and validation). Also the code likely contains many additional bugs.
 
 The upside is that there are lot of possibilities for you to make a real difference when you improve the code :-)
 
 
-Goals / Motivation
-------------------------------------
+## Goals / Motivation
+
 This library should track the [JS version of mjml](https://github.com/mjmlio/mjml) so ideally you should get the same HTML. However even under the best circumstances this library will always lag a bit behind as each change must be translated to Python manually (a mostly mechanical process).
 
 While I like the idea behind mjml and all the knowledge about the quirks to get acceptable HTML rendering by various email clients we did not want to deploy a Node.js-based stack on our production servers. We did not feel comfortable auditing all 220 JS packages which are installed by `npm install mjml` (and re-doing this whenever new versions are available). Also due to data-privacy concerns we were unable to use any third-party products (i.e. MJML's API offering).
 
 After a short [spike](https://en.wikipedia.org/wiki/Spike_(software_development)) to check the viability of a Python implementation I went ahead and wrote enough code to ensure some existing messages could be converted to mjml. Currently the library is deployed in some light production scenarios.
 
-Another benefit of using Python is that we can integrate that in our web apps more closely. As the startup overhead of CPython is much lower than Node.js we can also generate a few mails via CLI applications without massive performance problems. CPython uses ~70ms to translate a trivial mjml template to HTML while Node.JS needs ~650ms.
+Another benefit of using Python is that we can integrate that in our web apps more closely. As the startup overhead of CPython is much lower than Node.js we can also generate a few mails via CLI applications without massive performance problems. CPython uses \~70ms to translate a trivial mjml template to HTML while Node.JS needs \~650ms.
+
 
 
+## Documentation
 
-Documentation
-------------------------------------
 The idea is to implement the mjml XML dialect exactly like the JS implementation so eventually you should be able to use the [official docs](https://mjml.io/documentation/) and other online resources found on [mjml.io](https://mjml.io/). However we are nowhere near that right now! The current code can render the "Hello World" example as well as images, tables and groups but many components remain to be reimplemented. I'd love to see your pull requests to improve the current state though.
 
 
-Alternatives / Additional Resources
-------------------------------------
+
+## Alternatives / Additional Resources
 
 - **django-mjml**: If deploying NodeJS is not an issue and you are using Django you could use the well established [django-mjml](https://github.com/liminspace/django-mjml) library. That library integrates the mjml JavaScript implementation with Django templates so you can access all mjml features.
 - **MJML.NET**: This is an unofficial port of mjml to C# ([github repo](https://github.com/LiamRiddell/MJML.NET/)) which supports more components than this Python implementation.
+- **mrml**: rust implementation of mjml ([github repo](https://github.com/jdrouet/mrml))
 - [email-bugs](https://github.com/hteumeuleu/email-bugs) is a github project which contains a lot of knowledge about rendering quirks in various email clients.
 - [htmlemailcheck](https://www.htmlemailcheck.com/knowledge-base/) is a commercial offering to help you checking email rendering in various environments. I don't have any experience with their services but they provide a free knowledgebase.
-
-
-
+- [#emailgeeks](https://email.geeks.chat) - Slack community for email marketers, designers, and developers
```

### Comparing `mjml-0.8.0/README.md` & `mjml-0.9.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,60 @@
-mjml-stub
-=============
+# mjml-python
 
 This is an unofficial Python port of [mjml v4](https://github.com/mjmlio/mjml). It is implemented in pure Python and does not require JavaScript/NodeJS. mjml is a markup language created by [Mailjet](https://www.mailjet.com/) and designed to reduce the pain of coding a responsive email.
 
-    pip install mjml
+### Installation
 
+```sh
+pip install mjml
+```
+
+### Usage
+
+```py
+from mjml import mjml_to_html
+with open('foo.mjml', 'rb') as mjml_fp:
+    result = mjml_to_html(mjml_fp)
+assert not result.errors
+html: str = result.html
+```
+
+Alternatively you can run the code from the CLI:
+
+```sh
+$ mjml foo.mjml
+```
+
+
+## Limitations
 
-WARNING: stub implementation only!
-------------------------------------
 This library only implements a subset of the original MJML project. It lacks several features found in the JavaScript mjml implementation (e.g. minification, beautification and validation). Also the code likely contains many additional bugs.
 
 The upside is that there are lot of possibilities for you to make a real difference when you improve the code :-)
 
 
-Goals / Motivation
-------------------------------------
+## Goals / Motivation
+
 This library should track the [JS version of mjml](https://github.com/mjmlio/mjml) so ideally you should get the same HTML. However even under the best circumstances this library will always lag a bit behind as each change must be translated to Python manually (a mostly mechanical process).
 
 While I like the idea behind mjml and all the knowledge about the quirks to get acceptable HTML rendering by various email clients we did not want to deploy a Node.js-based stack on our production servers. We did not feel comfortable auditing all 220 JS packages which are installed by `npm install mjml` (and re-doing this whenever new versions are available). Also due to data-privacy concerns we were unable to use any third-party products (i.e. MJML's API offering).
 
 After a short [spike](https://en.wikipedia.org/wiki/Spike_(software_development)) to check the viability of a Python implementation I went ahead and wrote enough code to ensure some existing messages could be converted to mjml. Currently the library is deployed in some light production scenarios.
 
-Another benefit of using Python is that we can integrate that in our web apps more closely. As the startup overhead of CPython is much lower than Node.js we can also generate a few mails via CLI applications without massive performance problems. CPython uses ~70ms to translate a trivial mjml template to HTML while Node.JS needs ~650ms.
+Another benefit of using Python is that we can integrate that in our web apps more closely. As the startup overhead of CPython is much lower than Node.js we can also generate a few mails via CLI applications without massive performance problems. CPython uses \~70ms to translate a trivial mjml template to HTML while Node.JS needs \~650ms.
+
 
 
+## Documentation
 
-Documentation
-------------------------------------
 The idea is to implement the mjml XML dialect exactly like the JS implementation so eventually you should be able to use the [official docs](https://mjml.io/documentation/) and other online resources found on [mjml.io](https://mjml.io/). However we are nowhere near that right now! The current code can render the "Hello World" example as well as images, tables and groups but many components remain to be reimplemented. I'd love to see your pull requests to improve the current state though.
 
 
-Alternatives / Additional Resources
-------------------------------------
+
+## Alternatives / Additional Resources
 
 - **django-mjml**: If deploying NodeJS is not an issue and you are using Django you could use the well established [django-mjml](https://github.com/liminspace/django-mjml) library. That library integrates the mjml JavaScript implementation with Django templates so you can access all mjml features.
 - **MJML.NET**: This is an unofficial port of mjml to C# ([github repo](https://github.com/LiamRiddell/MJML.NET/)) which supports more components than this Python implementation.
+- **mrml**: rust implementation of mjml ([github repo](https://github.com/jdrouet/mrml))
 - [email-bugs](https://github.com/hteumeuleu/email-bugs) is a github project which contains a lot of knowledge about rendering quirks in various email clients.
 - [htmlemailcheck](https://www.htmlemailcheck.com/knowledge-base/) is a commercial offering to help you checking email rendering in various environments. I don't have any experience with their services but they provide a free knowledgebase.
-
+- [#emailgeeks](https://email.geeks.chat) - Slack community for email marketers, designers, and developers
```

### Comparing `mjml-0.8.0/mjml/core/api.py` & `mjml-0.9.0/mjml/core/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 
-from ..lib import merge_dicts, AttrDict
-
-from .registry import _components
+from ..lib import AttrDict, merge_dicts
+from .registry import components
 
 
 __all__ = ['initComponent', 'Component']
 
 def initComponent(name, **initialDatas):
     if name is None:
         return None
-    components = _components()
     component_cls = components[name]
     if not component_cls:
         return None
 
     component = component_cls(**initialDatas)
     if getattr(component, 'headStyle', None):
         component.context['addHeadStyle'](name, component.headStyle)
@@ -21,15 +19,16 @@
         component.context['addComponentHeadSyle'](component.componentHeadStyle)
     return component
 
 
 
 class Component:
     # LATER: not sure upstream also passes tagName, makes code easier for us
-    def __init__(self, *, attributes=None, children=(), content='', context=None, props=None, globalAttributes=None, headStyle=None, tagName=None):
+    def __init__(self, *, attributes=None, children=(), content='', context=None,
+                 props=None, globalAttributes=None, headStyle=None, tagName=None):
         self.children = list(children)
         self.content = content
         self.context = context
         self.tagName = tagName
 
         self.props = AttrDict(merge_dicts(props, {'children': children, 'content': content}))
 
@@ -73,16 +72,17 @@
             return ''
         return self.content.strip()
 
     def getChildContext(self):
         return self.context
 
     # js: getAttribute(name)
-    def get_attr(self, name):
-        if (name not in self.allowed_attrs()) and (name not in self.default_attrs()):
+    def get_attr(self, name, *, missing_ok=False):
+        is_allowed_attr = name in self.allowed_attrs()
+        is_default_attr = name in self.default_attrs()
+        if not missing_ok and (not is_allowed_attr) and (not is_default_attr):
             raise AssertionError(f'{self.__class__.__name__} has no declared attr {name}')
         return self.attrs.get(name)
     getAttribute = get_attr
 
     def render(self):
         return ''
-
```

### Comparing `mjml-0.8.0/mjml/elements/_base.py` & `mjml-0.9.0/mjml/elements/_base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 
-from ..lib import merge_dicts, AttrDict
-from ..core import initComponent, Component
-from ..core.registry import _components
+from ..core import Component, initComponent
+from ..core.registry import components
 from ..helpers import *
+from ..lib import AttrDict, merge_dicts
 
 
 __all__ = [
     'BodyComponent',
 ]
 
 class BodyComponent(Component):
@@ -31,15 +31,16 @@
         borderDirection = direction and self.getAttribute(f'border-{direction}')
         border = self.getAttribute('border')
         return borderParser(borderDirection or border or '0')
 
     def getBoxWidths(self):
         containerWidth = self.context['containerWidth']
         parsedWidth = strip_unit(containerWidth)
-        paddings = self.getShorthandAttrValue('padding', 'right') + self.getShorthandAttrValue('padding', 'left')
+        get_padding = lambda d: self.getShorthandAttrValue('padding', d)
+        paddings = get_padding('right') + get_padding('left')
         borders = self.getShorthandBorderValue('right') + self.getShorthandBorderValue('left')
 
         return AttrDict({
             'totalWidth': parsedWidth,
             'borders'   : borders,
             'paddings'  : paddings,
             'box'       : parsedWidth - paddings - borders,
@@ -47,16 +48,16 @@
 
     # js: htmlAttributes(attributes)
     def html_attrs(self, **attrs):
         def _to_str(kv):
             key, value = kv
             if key == 'style':
                 value = self.styles(value)
-            elif key == 'class_':
-                key = 'class'
+            elif key in ['class_', 'for_']:
+                key = key[:-1]
                 if not value:
                     return None
             if value is None:
                 return None
             return f'{key}="{value}"'
         serialized_attrs = map(_to_str, attrs.items())
         return ' '.join(filter(None, serialized_attrs))
@@ -66,15 +67,18 @@
         return {}
 
     # js: styles(styles)
     def styles(self, key=None):
         _styles = None
         if key and isinstance(key, str):
             _styles_dict = self.get_styles()
-            _styles = _styles_dict.get(key)
+            keys = key.split('.')
+            _styles = _styles_dict.get(keys[0])
+            if len(keys) > 1:
+                _styles = _styles.get(keys[1])
             if _styles and not isinstance(_styles, dict):
                 raise ValueError(f'key={key}')
         elif key:
             # predefined dict
             _styles = key
         if not _styles:
             _styles = {}
@@ -82,15 +86,16 @@
         def serializer(kv):
             k, v = kv
             return f'{k}:{v}' if is_not_empty(v) else None
         style_attr_strs = filter(None, map(serializer, _styles.items()))
         style_str = ';'.join(style_attr_strs)
         return style_str
 
-    def renderChildren(self, childrens=None, props=None, renderer=None, attributes=None, rawXML=False):
+    def renderChildren(self, childrens=None, props=None, renderer=None,
+                       attributes=None, rawXML=False):
         if not props:
             props = {}
         if not renderer:
             renderer = lambda component: component.render()
         if not attributes:
             attributes = {}
         childrens = childrens or self.props.children
@@ -107,15 +112,15 @@
         #
         # upstream:
         # const rawComponents = filter(components, c => c.isRawElement())
         # const nonRawSiblings = childrens.filter(
         #  child => !find(rawComponents, c => c.getTagName() === child.tagName),
         #).length
         raw_tag_names = set()
-        for tag_name, component in _components().items():
+        for tag_name, component in components.items():
             if component.isRawElement():
                 raw_tag_names.add(tag_name)
         is_raw_element = lambda c: (c['tagName'] in raw_tag_names)
 
         _nonRawSiblings = []
         for child in childrens:
             if (child is None) or is_raw_element(child):
@@ -147,8 +152,7 @@
                 name = children['tagName'],
                 **initialDatas,
             )
             if component:
                 output += renderer(component)
             index += 1
         return output
-
```

### Comparing `mjml-0.8.0/mjml/elements/head/_head_base.py` & `mjml-0.9.0/mjml/elements/head/_head_base.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-from mjml.core import initComponent, Component
+from mjml.core import Component, initComponent
 
 
 __all__ = ['HeadComponent']
 
 class HeadComponent(Component):
     def handlerChildren(self):
         def handle_children(children):
@@ -23,8 +23,7 @@
                 component.handler()
             if hasattr(component, 'render'):
                 return component.render()
             return None
 
         childrens = self.props.children
         return tuple(map(handle_children, childrens))
-
```

### Comparing `mjml-0.8.0/mjml/elements/head/mj_attributes.py` & `mjml-0.9.0/mjml/elements/head/mj_attributes.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 
-from ._head_base import HeadComponent
 from mjml.helpers import omit
 
+from ._head_base import HeadComponent
+
 
 __all__ = ['MjAttributes']
 
 class MjAttributes(HeadComponent):
+    component_name = 'mj-attributes'
+
     def handler(self):
         add = self.context['add']
         _children = self.props.children
 
         for child in _children:
             tagName = child['tagName']
             attributes = child['attributes']
@@ -33,8 +36,7 @@
                 #    return {'tagName': attributes, **acc}
                 #add('classesDefault', attr_name, reduce(children, reducer, {}))
             else:
                 if not attributes:
                     # TODO: not present upstream
                     continue
                 add('defaultAttributes', tagName, attributes)
-
```

### Comparing `mjml-0.8.0/mjml/elements/mj_body.py` & `mjml-0.9.0/mjml/elements/mj_body.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 
-from ._base import BodyComponent
 from ..lib import merge_dicts
+from ._base import BodyComponent
 
 
 __all__ = ['MjBody']
 
 class MjBody(BodyComponent):
+    component_name = 'mj-body'
+
     @classmethod
     def allowed_attrs(cls):
         return {
             'background-color': '',
             'css-class'       : None,
         }
 
@@ -35,8 +37,7 @@
     def render(self):
         setBackgroundColor = self.context['setBackgroundColor']
         setBackgroundColor(self.get_attr('background-color'))
 
         html_attrs = self.html_attrs(class_=self.get_attr('css-class'), style='div')
         children_str = self.renderChildren()
         return f'<div {html_attrs}>{children_str}</div>'
-
```

### Comparing `mjml-0.8.0/mjml/elements/mj_button.py` & `mjml-0.9.0/mjml/elements/mj_button.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 
-from ._base import BodyComponent
 from ..helpers import widthParser
+from ._base import BodyComponent
 
 
 __all__ = ['MjButton']
 
 class MjButton(BodyComponent):
+    component_name = 'mj-button'
+
     @classmethod
     def allowed_attrs(cls):
         return {
             'align'            : 'enum(left,center,right)',
             'background-color' : 'color',
             'border-bottom'    : 'string',
             'border-left'      : 'string',
@@ -115,18 +117,18 @@
             return None
 
         parsedWidth, unit = widthParser(width)
         # impossible to handle percents because it depends on padding and text width
         if unit != 'px':
             return None
 
-        _box_widths = self.getBoxWidths()
-        borders = _box_widths.borders
-        _inner_padding = lambda d: self.getShorthandAttrValue('inner-padding', d, attr_with_direction=False)
+        def _inner_padding(d):
+            return self.getShorthandAttrValue('inner-padding', d, attr_with_direction=False)
         innerPaddings = _inner_padding('left') + _inner_padding('right')
+        borders = self.getBoxWidths().borders
         width_int = parsedWidth - innerPaddings - borders
         return f'{width_int}px'
 
     def render(self):
         href_str = self.getAttribute('href')
         is_anchor = bool(href_str)
         target = self.getAttribute('target') if is_anchor else None
```

### Comparing `mjml-0.8.0/mjml/elements/mj_column.py` & `mjml-0.9.0/mjml/elements/mj_column.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 
-from ._base import BodyComponent
 from ..helpers import parse_float, parse_int, strip_unit, widthParser
 from ..lib import merge_dicts
+from ._base import BodyComponent
 
 
 __all__ = ['MjColumn']
 
 class MjColumn(BodyComponent):
+    component_name = 'mj-column'
+
     @classmethod
     def allowed_attrs(cls):
         return {
             'background-color': 'color',
             'border'          : 'string',
             'border-bottom'   : 'string',
             'border-left'     : 'string',
@@ -173,15 +175,21 @@
         else:
             width = parsedWidth - allPaddings
             containerWidth = f'{width}px'
         return merge_dicts(self.context, {'containerWidth': containerWidth})
 
 
     def hasGutter(self):
-        padding_attrs = ('padding', 'padding-bottom', 'padding-left', 'padding-right', 'padding-top')
+        padding_attrs = (
+            'padding',
+            'padding-bottom',
+            'padding-left',
+            'padding-right',
+            'padding-top'
+        )
         attr_values = map(lambda n: self.get_attr(n), padding_attrs)
         return any(filter(lambda v: bool(v), attr_values))
 
     def renderGutter(self):
         table_attrs = self.html_attrs(**{
             'border': '0',
             'cellpadding': '0',
@@ -201,30 +209,31 @@
 
     def renderColumn(self):
         children = self.props['children']
         def render_child(component):
             if component.isRawElement():
                 return component.render()
             td_attrs = component.html_attrs(
-                align = component.getAttribute('align'),
+                align = component.getAttribute('align', missing_ok=True),
                 # vertical-align
-                class_ = component.getAttribute('css-class'),
+                class_ = component.getAttribute('css-class', missing_ok=True),
                 style = {
                     'background': component.getAttribute(
-                      'container-background-color',
+                        'container-background-color',
+                        missing_ok=True
                     ),
                     'font-size': '0px',
                     'padding': component.getAttribute('padding'),
                     'padding-top': component.getAttribute('padding-top'),
                     'padding-right': component.getAttribute('padding-right'),
                     'padding-bottom': component.getAttribute('padding-bottom'),
                     'padding-left': component.getAttribute('padding-left'),
                     'word-break': 'break-word',
                   },
-                **{'vertical-align': component.getAttribute('vertical-align')}
+                **{'vertical-align': component.getAttribute('vertical-align', missing_ok=True)}
             )
             return f'''<tr>
               <td {td_attrs}>
                 {component.render()}
               </td>
             </tr>'''
 
@@ -233,10 +242,11 @@
             cellpadding='0',
             cellspacing='0',
             role='presentation',
             style='table',
             width='100%',
         )
         return f'''<table {table_attrs}>
-            {self.renderChildren(children, renderer=render_child)}
+            <tbody>
+                {self.renderChildren(children, renderer=render_child)}
+            </tbody>
         </table>'''
-
```

### Comparing `mjml-0.8.0/mjml/elements/mj_divider.py` & `mjml-0.9.0/mjml/elements/mj_divider.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 
-from ._base import BodyComponent
 from ..helpers import parse_int, widthParser
 from ..lib import merge_dicts
+from ._base import BodyComponent
 
 
 __all__ = ['MjDivider']
 
 class MjDivider(BodyComponent):
+    component_name = 'mj-divider'
+
     @classmethod
     def allowed_attrs(cls):
         return {
             'border-color'    : 'color',
             'border-style'    : 'string',
             'border-width'    : 'unit(px)',
             'container-background-color': 'color',
@@ -51,15 +53,16 @@
             'p': p,
             'outlook': merge_dicts(p, {'width': self.getOutlookWidth()}),
         }
 
     def getOutlookWidth(self):
         this = self
         containerWidth = this.context['containerWidth']
-        paddingSize = this.getShorthandAttrValue('padding', 'left') + this.getShorthandAttrValue('padding', 'right')
+        get_padding = lambda d: self.getShorthandAttrValue('padding', d)
+        paddingSize = get_padding('right') + get_padding('left')
         width = this.getAttribute('width')
         parsedWidth, unit = widthParser(width)
 
         if unit == '%':
             px = (parse_int(containerWidth) * parse_int(parsedWidth)) / 100 - paddingSize
             return f'{px}px'
         elif unit == 'px':
@@ -89,8 +92,7 @@
             <![endif]-->'''
 
     def render(self):
         return f'''
             <p {self.html_attrs(style='p')} > </p>
             {self.renderAfter()}
         '''
-
```

### Comparing `mjml-0.8.0/mjml/elements/mj_group.py` & `mjml-0.9.0/mjml/elements/mj_group.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 
-from ._base import BodyComponent
 from ..helpers import strip_unit, widthParser
 from ..lib import merge_dicts
+from ._base import BodyComponent
 
 
 __all__ = ['MjGroup']
 
 class MjGroup(BodyComponent):
+    component_name = 'mj-group'
+
     @classmethod
     def default_attrs(cls):
         return {
             'background-color' : '',
             'direction'        : 'ltr',
             'vertical-align'   : '',
             'width'            : '',
@@ -41,27 +43,32 @@
             }
         }
 
     def getChildContext(self):
         parentWidth = float(strip_unit(self.context['containerWidth']))
         nonRawSiblings = self.props['nonRawSiblings']
         children = self.props['children']
-        paddingSize = self.getShorthandAttrValue('padding', 'left') + self.getShorthandAttrValue('padding', 'right')
+        get_padding = lambda d: self.getShorthandAttrValue('padding', d)
+        paddingSize = get_padding('right') + get_padding('left')
 
         containerWidth = self.getAttribute('width') or f'{(parentWidth / nonRawSiblings)}px'
         parsedWidth, unit = widthParser(containerWidth, parseFloatToInt=False)
 
         width_px = None
         if unit == '%':
             width_px = (parentWidth * parsedWidth) / 100 - paddingSize
         else:
             width_px = parsedWidth - paddingSize
         containerWidth = f'{width_px}px'
 
-        return merge_dicts(self.context, {'containerWidth': containerWidth, 'nonRawSiblings': len(children)})
+        extra_ctx = {
+            'containerWidth': containerWidth,
+            'nonRawSiblings': len(children),
+        }
+        return merge_dicts(self.context, extra_ctx)
 
     def getParsedWidth(self, toString=False):
         nonRawSiblings = self.props['nonRawSiblings']
         width = self.getAttribute('width') or f'{100 / nonRawSiblings}%'
         width_unit = widthParser(width, parseFloatToInt=False)
         if toString:
             return str(width_unit)
@@ -156,9 +163,8 @@
               <tr>
             <![endif]-->
             {self.renderChildren(children, attributes={'mobileWidth': 'mobileWidth'}, renderer=child_renderer)}
             <!--[if mso | IE]>
               </tr>
               </table>
             <![endif]-->
-        </div>'''
-
+        </div>''' # noqa: line-too-long
```

### Comparing `mjml-0.8.0/mjml/elements/mj_image.py` & `mjml-0.9.0/mjml/elements/mj_image.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 
 import math
 
-from ._base import BodyComponent
 from ..helpers import parse_int, strip_unit, widthParser
+from ._base import BodyComponent
 
 
 __all__ = ['MjImage']
 
 class MjImage(BodyComponent):
+    component_name = 'mj-image'
+
     @classmethod
     def allowed_attrs(cls):
         return {
             'alt'             : 'string',
             'href'            : 'string',
             'name'            : 'string',
             'src'             : 'string',
@@ -166,8 +168,7 @@
               <tr>
                 <td {td_attrs} >
                   {this.renderImage()}
                 </td>
               </tr>
             </tbody>
           </table>'''
-
```

### Comparing `mjml-0.8.0/mjml/elements/mj_section.py` & `mjml-0.9.0/mjml/elements/mj_section.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 
+import re
 from collections import namedtuple
 from decimal import Decimal
-import re
 
-from ._base import BodyComponent
 from ..helpers import parse_percentage, strip_unit, suffixCssClasses
-from ..lib import merge_dicts, AttrDict
+from ..lib import AttrDict, merge_dicts
+from ._base import BodyComponent
 
 
 __all__ = ['MjSection']
 
 Position = namedtuple('Position', ('x', 'y'))
 
 
 class MjSection(BodyComponent):
+    component_name = 'mj-section'
+
     @classmethod
     def allowed_attrs(cls):
         return {
             'background-color' : 'color',
             'background-url'   : 'string',
             'background-repeat': 'enum(repeat,no-repeat)',
             'background-size'  : 'string',
@@ -141,15 +143,41 @@
 
     def render(self):
         if self.isFullWidth():
             return self.renderFullWidth()
         return self.renderSimple()
 
     def renderFullWidth(self):
-        raise NotImplementedError()
+        content = f'{self.renderBefore()}{self.renderSection()}{self.renderAfter()}'
+
+        if self.hasBackground():
+            content = self.renderWithBackground(content)
+
+        return f'''
+            <table
+                {self.html_attrs(
+                    align='center',
+                    class_=self.getAttribute('css-class'),
+                    background=self.getAttribute('background-url'),
+                    border='0',
+                    cellpadding='0',
+                    cellspacing='0',
+                    role='presentation',
+                    style='tableFullwidth',
+                )}
+            >
+                <tbody>
+                    <tr>
+                        <td>
+                            {content}
+                        </td>
+                    </tr>
+                </tbody>
+            </table>
+        '''
 
     def renderSimple(self):
         section = self.renderSection()
         if self.hasBackground():
             section = self.renderWithBackground(section)
 
         return ''.join([
@@ -193,19 +221,19 @@
 
     def isFullWidth(self):
         return self.get_attr('full-width') == 'full-width'
 
     def renderSection(self):
         hasBackground = self.hasBackground()
 
-        wrapper_class = self.get_attr('css-class') if self.isFullWidth() else None
+        wrapper_class = None if self.isFullWidth() else self.get_attr('css-class')
         wrapper_attr_str = self.html_attrs(class_=wrapper_class, style='div')
 
         bg_div_start = f'<div {self.html_attrs(style="innerDiv")}>' if hasBackground else ''
-        bg_div_end = f'</div>' if hasBackground else ''
+        bg_div_end = '</div>' if hasBackground else ''
 
         table_attrs = self.html_attrs(
             align='center',
             background=None if self.isFullWidth() else self.get_attr('background-url'),
             border='0',
             cellpadding='0',
             cellspacing='0',
@@ -240,27 +268,24 @@
     def renderWrappedChildren(self):
         children = self.props['children']
 
         def render_child(component):
             if component.isRawElement():
                 return component.render()
             td_ie_attrs = component.html_attrs(
-                # TODO: no component has an "align" attr, also never used?
-                #align=component.get_attr('align'),
+                align=component.get_attr('align', missing_ok=True),
                 class_=suffixCssClasses(
                       component.get_attr('css-class'),
                       'outlook',
                     ),
                 style='tdOutlook',
             )
             return f'''
               <!--[if mso | IE]>
-                <td
-                  {td_ie_attrs}
-                >
+                <td {td_ie_attrs}>
               <![endif]-->
                 {component.render()}
               <!--[if mso | IE]>
                 </td>
               <![endif]-->
             '''
 
@@ -404,8 +429,7 @@
 
 def is_percentage(value):
     match = re.search(r'^\d+(\.\d+)?%$', value)
     return (match is not None)
 
 def makeBackgroundString(parts):
     return ' '.join(filter(None, parts))
-
```

### Comparing `mjml-0.8.0/mjml/elements/mj_table.py` & `mjml-0.9.0/mjml/elements/mj_table.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 
-from ._base import BodyComponent
 from ..helpers import widthParser
+from ._base import BodyComponent
 
 
 __all__ = ['MjTable']
 
 class MjTable(BodyComponent):
+    component_name = 'mj-table'
+
     @classmethod
     def allowed_attrs(cls):
         return {
             'align'            : 'enum(left,right,center)',
             'border'           : 'string',
             'cellpadding'      : 'integer',
             'cellspacing'      : 'integer',
@@ -74,8 +76,7 @@
             cellpadding = self.get_attr('cellpadding'),
             cellspacing = self.get_attr('cellspacing'),
         )
         content_html = self.getContent()
         return f'''<table {table_attrs}>
             {content_html}
         </table>'''
-
```

### Comparing `mjml-0.8.0/mjml/elements/mj_text.py` & `mjml-0.9.0/mjml/elements/mj_text.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 
 from ._base import BodyComponent
 
 
 __all__ = ['MjText']
 
 class MjText(BodyComponent):
+    component_name = 'mj-text'
+
     @classmethod
     def allowed_attrs(cls):
         return {
             'align'            : 'enum(left,right,center,justify)',
             'background-color' : 'color',
             'color'            : 'color',
             'container-background-color': 'color',
@@ -61,15 +63,14 @@
     def render(self):
         height = self.getAttribute('height')
         if not height:
             return self._render_content()
 
         start_conditional = f'''
             <table role="presentation" border="0" cellpadding="0" cellspacing="0"><tr><td height="{height}" style="vertical-align:top;height:{height};">
-        '''
+        ''' # noqa: line-too-long
         end_conditional = '</td></tr></table>'
         return f'''{start_conditional}{self._render_content()}{end_conditional}'''
 
     def _render_content(self):
         content_html = self.getContent()
         return '<div ' + self.html_attrs(style='text') + '>' + content_html + '</div>'
-
```

### Comparing `mjml-0.8.0/mjml/helpers/conditional_tag.py` & `mjml-0.9.0/mjml/helpers/conditional_tag.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,8 +23,7 @@
 
 def msoConditionalTag(content, negation=False):
     if negation:
         start, end = startMsoNegationConditionalTag, endNegationConditionalTag
     else:
         start, end = startConditionalTag, endConditionalTag
     return start + content + end
-
```

### Comparing `mjml-0.8.0/mjml/helpers/fonts.py` & `mjml-0.9.0/mjml/helpers/fonts.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,8 +26,7 @@
       <!--[if !mso]><!-->
         {link_tags_str}
         <style type="text/css">
           {import_lines_str}
         </style>
       <!--<![endif]-->\n
     '''
-
```

### Comparing `mjml-0.8.0/mjml/helpers/json_to_xml.py` & `mjml-0.9.0/mjml/helpers/json_to_xml.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     elif 'children' in root:
         child_indent = f'{indent}  '
         children = []
         for child in root.get('children', []):
             # {"passport": "hidden"} is a special attribute only present in
             # JSON MJML. The attribute is set by Passport (Mailjet's template
             # editor) to hide specific elements.
-            # https://github.com/FelixSchwarz/mjml-stub/commit/e1c006e213f26fb6dd9cf406b6e7b849350f6bc7#r47810966
+            # https://github.com/FelixSchwarz/mjml-python/commit/e1c006e213f26fb6dd9cf406b6e7b849350f6bc7#r47810966
             if child.get('attributes', {}).get('passport', {}).get('hidden'):
                 continue
             child_xml = json_to_xml(child, indent=child_indent)
             children.append(child_xml)
         content = '\n'.join(children)
     else:
         content = ''
```

### Comparing `mjml-0.8.0/mjml/helpers/media_queries.py` & `mjml-0.9.0/mjml/helpers/media_queries.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,8 +27,7 @@
           {media_queries_str}
       }}
     </style>
     <style media="screen and (min-width:{breakpoint})">
         {thunderbird_media_queries_str}
     </style>
     '''
-
```

### Comparing `mjml-0.8.0/mjml/helpers/py_utils.py` & `mjml-0.9.0/mjml/helpers/py_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
-from decimal import Decimal
 import re
+from decimal import Decimal
 
 
 __all__ = [
     'is_nil',
     'is_empty',
     'is_not_empty',
     'is_not_nil',
@@ -53,8 +53,7 @@
         return True
     elif hasattr(v, 'strip'):
         return not bool(v.strip())
     return not bool(v)
 
 def is_not_empty(v):
     return not is_empty(v)
-
```

### Comparing `mjml-0.8.0/mjml/helpers/shorthand_parser.py` & `mjml-0.9.0/mjml/helpers/shorthand_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,8 +39,7 @@
     # Upstream does not have to deal with this case as "parseInt(undefined, 10)"
     # does not trigger an exception in JavaScript but just returns NaN.
     # The JS function returns 0 in these cases due to "NaN || 0".
     if match is None:
         return 0
     border_value = match.group(1)
     return parse_int(border_value)
-
```

### Comparing `mjml-0.8.0/mjml/helpers/skeleton.py` & `mjml-0.9.0/mjml/helpers/skeleton.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,11 +103,10 @@
         {{ extra_style }}
         {{ headRaw_str }}
       </head>
       <body style="word-spacing:normal;{{ backgroundColor }}">
         {{ preview_str }}
         {{ content }}
       </body>
-    </html>'''
+    </html>''' # noqa: line-too-long
 
 skeleton_tmpl_str = textwrap.dedent(skeleton_tmpl_str_raw)
-
```

### Comparing `mjml-0.8.0/mjml/helpers/width_parser.py` & `mjml-0.9.0/mjml/helpers/width_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
-from collections import namedtuple
 import re
+from collections import namedtuple
 
 from .py_utils import strip_unit
 
 
 __all__ = ['widthParser']
 
 _WidthUnit = namedtuple('_WidthUnit', ('width', 'unit'))
@@ -39,8 +39,7 @@
     # type sytem). parseFloat() might return a number without fractional but
     # python does.
     width_int = int(width)
     if parsed_width == width_int:
         parsed_width = width_int
 
     return WidthUnit(width=parsed_width, unit=widthUnit)
-
```

### Comparing `mjml-0.8.0/mjml/lib/attribute_dict.py` & `mjml-0.9.0/mjml/lib/attribute_dict.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: UTF-8 -*-
 
 # License: Public Domain
 # Authors: Felix Schwarz <felix.schwarz@oss.schwarz.eu>
-# 
+#
 # Version 1.2
 #
 # 1.2 (2018-02-16)
 #   - split tests into separate file
 #   - add ".copy()" method
 #
 # 1.1 (08.09.2015)
@@ -20,14 +20,16 @@
 
 class AttrDict(dict):
     def copy(self):
         return AttrDict(self)
 
     def __getattr__(self, name):
         if name not in self:
-            raise AttributeError("'%s' object has no attribute '%s'" % (self.__class__.__name__, name))
+            class_name = self.__class__.__name__
+            raise AttributeError("'%s' object has no attribute '%s'" % (class_name, name))
         return self[name]
 
     def __setattr__(self, name, value):
         if name not in self:
-            raise AttributeError("'%s' object has no attribute '%s'" % (self.__class__.__name__, name))
+            class_name = self.__class__.__name__
+            raise AttributeError("'%s' object has no attribute '%s'" % (class_name, name))
         self[name] = value
```

### Comparing `mjml-0.8.0/mjml/lib/dict_merger.py` & `mjml-0.9.0/mjml/lib/dict_merger.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,8 +19,7 @@
                 src_item_is_dict = isinstance(current_src.get(key), dict)
                 dst_item_is_dict = isinstance(current_dst.get(key), dict)
                 if src_item_is_dict and dst_item_is_dict:
                     stack.append((current_src[key], current_dst[key]))
                 else:
                     current_dst[key] = current_src[key]
     return result
-
```

### Comparing `mjml-0.8.0/mjml/lib/tests/dict_merger_test.py` & `mjml-0.9.0/mjml/lib/tests/dict_merger_test.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # Copyright 2015 Felix Schwarz
 # The source code in this file is licensed under the MIT license.
 
 from pythonic_testcase import *
 
 from ..dict_merger import merge_dicts
 
+
 class DictMergerTest(PythonicTestCase):
     def test_returns_single_dict_unmodified(self):
         assert_equals({}, merge_dicts({}))
         assert_equals({'bar': 42}, merge_dicts({'bar': 42}))
 
     def test_can_merge_two_dicts_without_modifying_inputs(self):
         a = {'a': 1}
@@ -17,8 +18,7 @@
         assert_equals({'a': 1, 'b': 2}, merge_dicts(a, b))
 
     def test_can_merge_three_dicts_without_modifying_inputs(self):
         a = {'a': 1}
         b = {'b': 2}
         c = {'c': 3}
         assert_equals({'a': 1, 'b': 2, 'c': 3}, merge_dicts(a, b, c))
-
```

### Comparing `mjml-0.8.0/mjml/mjml2html.py` & `mjml-0.9.0/mjml/mjml2html.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,31 @@
-
 from io import BytesIO, StringIO
 from pathlib import Path, PurePath
+from typing import List, Optional
 
 from bs4 import BeautifulSoup
 
 from .core import initComponent
-from .helpers import mergeOutlookConditionnals, json_to_xml, omit, skeleton_str as default_skeleton
-from .lib import merge_dicts, AttrDict
+from .core.registry import register_components, register_core_components
+from .helpers import json_to_xml, mergeOutlookConditionnals, omit, skeleton_str as default_skeleton
+from .lib import AttrDict, merge_dicts
 
 
 def ignore_empty(values):
     result = []
     for value in values:
         if value:
             result.append(value)
     return tuple(result)
 
 
-def mjml_to_html(xml_fp_or_json, skeleton=None, template_dir=None):
+def mjml_to_html(xml_fp_or_json, skeleton=None, template_dir=None,
+                 custom_components: Optional[List]=None):
+    register_core_components()
+
     if isinstance(xml_fp_or_json, dict):
         xml_fp = StringIO(json_to_xml(xml_fp_or_json))
     elif isinstance(xml_fp_or_json, str):
         xml_fp = StringIO(xml_fp_or_json)
     else:
         xml_fp = xml_fp_or_json
 
@@ -32,14 +36,17 @@
     mjml_root = mjml_doc.mjml
 
     skeleton_path = skeleton
     if skeleton_path:
         raise NotImplementedError('not yet implemented')
     skeleton = default_skeleton
 
+    if custom_components:
+        register_components(custom_components)
+
     fonts = {
       'Open Sans': 'https://fonts.googleapis.com/css?family=Open+Sans:300,400,500,700',
       'Droid Sans': 'https://fonts.googleapis.com/css?family=Droid+Sans:300,400,500,700',
       'Lato': 'https://fonts.googleapis.com/css?family=Lato:300,400,500,700',
       'Roboto': 'https://fonts.googleapis.com/css?family=Roboto:300,400,500,700',
       'Ubuntu': 'https://fonts.googleapis.com/css?family=Ubuntu:300,400,500,700',
     }
@@ -47,26 +54,29 @@
 
     globalDatas = AttrDict({
         'backgroundColor'    : None,
         'breakpoint'         : '480px',
         'classes'            : {},
         'classesDefault'     : {},
         'defaultAttributes'  : {},
+        'htmlAttributes'     : {},
         'fonts'              : fonts,
         'inlineStyle'        : [],
         'headStyle'          : {},
         'componentsHeadStyle': [],
         'headRaw'            : [],
         'mediaQueries'       : {},
         'preview'            : '',
         'style'              : [],
         'title'              : '',
     })
 
-    validationLevel = 'skip'
+    # "validationLevel" is not used but available upstream - makes it easier to
+    # match the line of code with the upstream sources.
+    validationLevel = 'skip' # noqa: F841
     errors = []
     # LATER: optional validation
 
     mjBody = mjml_root('mj-body')[0]
     mjHead = mjml_root('mj-head')
     if mjHead:
         assert len(mjHead) == 1
@@ -124,15 +134,17 @@
                 globalDatas.defaultAttributes.get(tagName, {}),
                 attributesClasses,
                 defaultAttributesForClasses,
                 _attrs_omit,
             )
 
             if tagName == 'mj-include':
-                mj_include_subtree = handle_include(attributes['path'], parse_mjml=parse, template_dir=template_dir)
+                mj_include_subtree = handle_include(attributes['path'],
+                                                    parse_mjml=parse,
+                                                    template_dir=template_dir)
                 return mj_include_subtree
             result = {
                 'tagName': tagName,
                 'content': content,
                 'attributes': _returned_attributes,
                 'globalAttributes': globalDatas.defaultAttributes.get('mj-all', {}).copy(),
                 'children': [], # will be set afterwards
@@ -148,15 +160,16 @@
         return parse(mjml_element, template_dir=template_dir)
 
     def addHeadStyle(identifier, headStyle):
         globalDatas.headStyle[identifier] = headStyle
 
     def addMediaQuery(className, parsedWidth, unit):
         width_str = f'{parsedWidth}{unit}'
-        globalDatas.mediaQueries[className] = f'{{ width:{width_str} !important; max-width: {width_str}; }}'
+        width_css = f'{{ width:{width_str} !important; max-width: {width_str}; }}'
+        globalDatas.mediaQueries[className] = width_css
 
     def addComponentHeadSyle(headStyle):
         globalDatas.componentsHeadStyle.append(headStyle)
 
     def setBackgroundColor(color):
         globalDatas.backgroundColor = color
 
@@ -167,15 +180,15 @@
         setBackgroundColor = setBackgroundColor,
         backgroundColor = lambda node, context: processing(node, context, applyAttributes),
     )
 
     def _head_data_add(attr, *params):
         if attr not in globalDatas:
             param_str = ''.join(params) if isinstance(params, list) else params
-            exc_msg = f'A mj-head element add an unknown head attribute : {attr} with params {param_str}'
+            exc_msg = f'A mj-head element add an unknown head attribute: {attr} with params {param_str}' # noqa: E501
             raise ValueError(exc_msg)
 
         current_attr_value = globalDatas[attr]
         if isinstance(current_attr_value, (list, tuple)):
             current_attr_value.extend(params)
         elif len(params) == 1:
             assert len(params) == 1
@@ -188,30 +201,40 @@
 
     headHelpers = AttrDict(
         add = _head_data_add,
     )
     globalDatas.headRaw = processing(mjHead, headHelpers)
     content = processing(mjBody, bodyHelpers, applyAttributes)
 
+    if globalDatas.htmlAttributes:
+        contentSoup = BeautifulSoup(content, 'html.parser')
+        for selector, data in globalDatas.htmlAttributes.items():
+            for attrName, value in data.items():
+                for element in contentSoup.select(selector):
+                    element[attrName] = value or ''
+
+        content = contentSoup.decode_contents()
+
     content = skeleton(
         content=content,
         # upstream just passes this extra key to skeleton() as JavaScript
         # won't complain about additional parameters.
-        **omit(globalDatas, ('classesDefault',)),
+        **omit(globalDatas, ('classesDefault', 'htmlAttributes')),
     )
     # LATER: upstream has also beautify
     # LATER: upstream has also minify
 
     if len(globalDatas.inlineStyle) > 0:
         try:
             import css_inline
         except ImportError:
-            raise ImportError('CSS inlining is an optional feature. Run `pip install -e ".[css_inlining]"` to install the required dependencies.')
+            raise ImportError('CSS inlining is an optional feature. Run `pip install -e ".[css_inlining]"` to install the required dependencies.') # noqa: E501
 
-        inliner = css_inline.CSSInliner(inline_style_tags=False, extra_css=''.join(globalDatas.inlineStyle))
+        extra_css = ''.join(globalDatas.inlineStyle)
+        inliner = css_inline.CSSInliner(inline_style_tags=False, extra_css=extra_css)
         content = inliner.inline(content)
 
     content = mergeOutlookConditionnals(content)
 
     return AttrDict({
         'html': content,
         'errors': errors,
```

### Comparing `mjml-0.8.0/mjml.egg-info/PKG-INFO` & `mjml-0.9.0/mjml.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,70 +1,88 @@
 Metadata-Version: 2.1
 Name: mjml
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python implementation for MJML - a framework that makes responsive-email easy
-Home-page: https://github.com/FelixSchwarz/mjml-stub
+Home-page: https://github.com/FelixSchwarz/mjml-python
 Author: Felix Schwarz
 Author-email: felix.schwarz@oss.schwarz.eu
 License: MIT
-Project-URL: Code, https://github.com/FelixSchwarz/mjml-stub
-Project-URL: Issue tracker, https://github.com/FelixSchwarz/mjml-stub/issues
-Platform: UNKNOWN
+Project-URL: Code, https://github.com/FelixSchwarz/mjml-python
+Project-URL: Issue tracker, https://github.com/FelixSchwarz/mjml-python/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Communications :: Email
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 Provides-Extra: css_inlining
 License-File: LICENSE.txt
 
-mjml-stub
-=============
+# mjml-python
 
 This is an unofficial Python port of [mjml v4](https://github.com/mjmlio/mjml). It is implemented in pure Python and does not require JavaScript/NodeJS. mjml is a markup language created by [Mailjet](https://www.mailjet.com/) and designed to reduce the pain of coding a responsive email.
 
-    pip install mjml
+### Installation
 
+```sh
+pip install mjml
+```
+
+### Usage
+
+```py
+from mjml import mjml_to_html
+with open('foo.mjml', 'rb') as mjml_fp:
+    result = mjml_to_html(mjml_fp)
+assert not result.errors
+html: str = result.html
+```
+
+Alternatively you can run the code from the CLI:
+
+```sh
+$ mjml foo.mjml
+```
+
+
+## Limitations
 
-WARNING: stub implementation only!
-------------------------------------
 This library only implements a subset of the original MJML project. It lacks several features found in the JavaScript mjml implementation (e.g. minification, beautification and validation). Also the code likely contains many additional bugs.
 
 The upside is that there are lot of possibilities for you to make a real difference when you improve the code :-)
 
 
-Goals / Motivation
-------------------------------------
+## Goals / Motivation
+
 This library should track the [JS version of mjml](https://github.com/mjmlio/mjml) so ideally you should get the same HTML. However even under the best circumstances this library will always lag a bit behind as each change must be translated to Python manually (a mostly mechanical process).
 
 While I like the idea behind mjml and all the knowledge about the quirks to get acceptable HTML rendering by various email clients we did not want to deploy a Node.js-based stack on our production servers. We did not feel comfortable auditing all 220 JS packages which are installed by `npm install mjml` (and re-doing this whenever new versions are available). Also due to data-privacy concerns we were unable to use any third-party products (i.e. MJML's API offering).
 
 After a short [spike](https://en.wikipedia.org/wiki/Spike_(software_development)) to check the viability of a Python implementation I went ahead and wrote enough code to ensure some existing messages could be converted to mjml. Currently the library is deployed in some light production scenarios.
 
-Another benefit of using Python is that we can integrate that in our web apps more closely. As the startup overhead of CPython is much lower than Node.js we can also generate a few mails via CLI applications without massive performance problems. CPython uses ~70ms to translate a trivial mjml template to HTML while Node.JS needs ~650ms.
+Another benefit of using Python is that we can integrate that in our web apps more closely. As the startup overhead of CPython is much lower than Node.js we can also generate a few mails via CLI applications without massive performance problems. CPython uses \~70ms to translate a trivial mjml template to HTML while Node.JS needs \~650ms.
+
 
 
+## Documentation
 
-Documentation
-------------------------------------
 The idea is to implement the mjml XML dialect exactly like the JS implementation so eventually you should be able to use the [official docs](https://mjml.io/documentation/) and other online resources found on [mjml.io](https://mjml.io/). However we are nowhere near that right now! The current code can render the "Hello World" example as well as images, tables and groups but many components remain to be reimplemented. I'd love to see your pull requests to improve the current state though.
 
 
-Alternatives / Additional Resources
-------------------------------------
+
+## Alternatives / Additional Resources
 
 - **django-mjml**: If deploying NodeJS is not an issue and you are using Django you could use the well established [django-mjml](https://github.com/liminspace/django-mjml) library. That library integrates the mjml JavaScript implementation with Django templates so you can access all mjml features.
 - **MJML.NET**: This is an unofficial port of mjml to C# ([github repo](https://github.com/LiamRiddell/MJML.NET/)) which supports more components than this Python implementation.
+- **mrml**: rust implementation of mjml ([github repo](https://github.com/jdrouet/mrml))
 - [email-bugs](https://github.com/hteumeuleu/email-bugs) is a github project which contains a lot of knowledge about rendering quirks in various email clients.
 - [htmlemailcheck](https://www.htmlemailcheck.com/knowledge-base/) is a commercial offering to help you checking email rendering in various environments. I don't have any experience with their services but they provide a free knowledgebase.
-
-
-
+- [#emailgeeks](https://email.geeks.chat) - Slack community for email marketers, designers, and developers
```

### Comparing `mjml-0.8.0/mjml.egg-info/SOURCES.txt` & `mjml-0.9.0/mjml.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,62 @@
 CHANGELOG.md
 LICENSE.txt
 MANIFEST.in
 README.md
 VERSION.txt
+pyproject.toml
 setup.cfg
 setup.py
 .github/workflows/tests.yml
 mjml/__init__.py
 mjml/mjml2html.py
 mjml/parser.py
+mjml/testing_helpers.py
 mjml.egg-info/PKG-INFO
 mjml.egg-info/SOURCES.txt
 mjml.egg-info/dependency_links.txt
 mjml.egg-info/entry_points.txt
 mjml.egg-info/requires.txt
 mjml.egg-info/top_level.txt
 mjml.egg-info/zip-safe
 mjml/core/__init__.py
 mjml/core/api.py
 mjml/core/registry.py
 mjml/elements/__init__.py
 mjml/elements/_base.py
+mjml/elements/mj_accordion.py
+mjml/elements/mj_accordion_element.py
+mjml/elements/mj_accordion_text.py
+mjml/elements/mj_accordion_title.py
 mjml/elements/mj_body.py
 mjml/elements/mj_button.py
+mjml/elements/mj_carousel.py
+mjml/elements/mj_carousel_image.py
 mjml/elements/mj_column.py
 mjml/elements/mj_divider.py
 mjml/elements/mj_group.py
+mjml/elements/mj_hero.py
 mjml/elements/mj_image.py
+mjml/elements/mj_navbar.py
+mjml/elements/mj_navbar_link.py
 mjml/elements/mj_raw.py
 mjml/elements/mj_section.py
+mjml/elements/mj_social.py
+mjml/elements/mj_social_element.py
+mjml/elements/mj_spacer.py
 mjml/elements/mj_table.py
 mjml/elements/mj_text.py
+mjml/elements/mj_wrapper.py
 mjml/elements/head/__init__.py
 mjml/elements/head/_head_base.py
 mjml/elements/head/mj_attributes.py
+mjml/elements/head/mj_breakpoint.py
 mjml/elements/head/mj_font.py
 mjml/elements/head/mj_head.py
+mjml/elements/head/mj_html_attributes.py
 mjml/elements/head/mj_preview.py
 mjml/elements/head/mj_style.py
 mjml/elements/head/mj_title.py
 mjml/helpers/__init__.py
 mjml/helpers/conditional_tag.py
 mjml/helpers/fonts.py
 mjml/helpers/json_to_xml.py
@@ -55,45 +72,60 @@
 mjml/lib/attribute_dict.py
 mjml/lib/dict_merger.py
 mjml/lib/tests/__init__.py
 mjml/lib/tests/dict_merger_test.py
 mjml/scripts/__init__.py
 mjml/scripts/mjml-html-compare
 mjml/scripts/mjml.py
+tests/__init__.py
 tests/border_parser_test.py
+tests/custom_components_test.py
 tests/includes_with_umlauts_test.py
 tests/missing_functionality_test.py
 tests/mj_button_mailto_link_test.py
 tests/mjml2html_test.py
 tests/upstream_alignment_test.py
+tests/testdata/_custom-expected.html
 tests/testdata/button-expected.html
 tests/testdata/css-inlining-expected.html
 tests/testdata/hello-world-expected.html
 tests/testdata/html-entities-expected.html
 tests/testdata/html-without-closing-tag-expected.html
 tests/testdata/minimal-expected.html
 tests/testdata/missing-whitespace-before-tag-expected.html
+tests/testdata/mj-accordion-expected.html
 tests/testdata/mj-attributes-expected.html
 tests/testdata/mj-body-with-background-color-expected.html
+tests/testdata/mj-breakpoint-expected.html
 tests/testdata/mj-button-with-width-expected.html
+tests/testdata/mj-carousel-expected.html
 tests/testdata/mj-column-with-attributes-expected.html
 tests/testdata/mj-font-expected.html
 tests/testdata/mj-font-multiple-expected.html
 tests/testdata/mj-font-unused-expected.html
 tests/testdata/mj-group-expected.html
 tests/testdata/mj-head-with-comment-expected.html
+tests/testdata/mj-hero-fixed-expected.html
+tests/testdata/mj-hero-fluid-expected.html
+tests/testdata/mj-html-attributes-expected.html
 tests/testdata/mj-image-with-empty-alt-attribute-expected.html
 tests/testdata/mj-image-with-href-expected.html
 tests/testdata/mj-include-body-expected.html
+tests/testdata/mj-navbar-expected.html
 tests/testdata/mj-preview-expected.html
 tests/testdata/mj-raw-expected.html
 tests/testdata/mj-raw-head-expected.html
 tests/testdata/mj-raw-head-with-tags-expected.html
 tests/testdata/mj-raw-with-tags-expected.html
 tests/testdata/mj-section-with-background-url-expected.html
+tests/testdata/mj-section-with-css-class-expected.html
+tests/testdata/mj-section-with-full-width-expected.html
 tests/testdata/mj-section-with-mj-class-expected.html
+tests/testdata/mj-social-expected.html
+tests/testdata/mj-spacer-expected.html
 tests/testdata/mj-style-expected.html
 tests/testdata/mj-table-expected.html
 tests/testdata/mj-text-with-tail-text-expected.html
 tests/testdata/mj-title-expected.html
+tests/testdata/mj-wrapper-expected.html
 tests/testdata/text_with_html-expected.html
 tools/update-expected-html.py
```

### Comparing `mjml-0.8.0/setup.cfg` & `mjml-0.9.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -2,32 +2,33 @@
 name = mjml
 version = file: VERSION.txt
 description = Python implementation for MJML - a framework that makes responsive-email easy
 long_description = file:README.md
 long_description_content_type = text/markdown
 author = Felix Schwarz
 author_email = felix.schwarz@oss.schwarz.eu
-url = https://github.com/FelixSchwarz/mjml-stub
+url = https://github.com/FelixSchwarz/mjml-python
 license = MIT
 license_file = LICENSE.txt
 classifiers = 
 	Development Status :: 3 - Alpha
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Communications :: Email
 	Topic :: Text Processing :: Markup :: HTML
 project_urls = 
-	Code = https://github.com/FelixSchwarz/mjml-stub
-	Issue tracker = https://github.com/FelixSchwarz/mjml-stub/issues
+	Code = https://github.com/FelixSchwarz/mjml-python
+	Issue tracker = https://github.com/FelixSchwarz/mjml-python/issues
 
 [options]
 python_requires = >= 3.6
 packages = find:
 zip_safe = true
 include_package_data = true
 install_requires =
```

### Comparing `mjml-0.8.0/tests/includes_with_umlauts_test.py` & `mjml-0.9.0/tests/includes_with_umlauts_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from unittest import TestCase
 
 from schwarz.fakefs_helpers import FakeFS
 
 from mjml import mjml_to_html
 
 
-
 class IncludesWithUmlautsTest(TestCase):
     def test_can_properly_handle_include_umlauts(self):
         fs = FakeFS.set_up(test=self)
         included_mjml = (
             '<mj-section>'
             '  <mj-column>'
             '    <mj-text>äöüß</mj-text>'
@@ -28,8 +27,7 @@
         )
         fs.create_file('footer.mjml', contents=included_mjml.encode('utf8'))
 
         result = mjml_to_html(StringIO(mjml))
         html = result.html
 
         assert ('äöüß' in html)
-
```

### Comparing `mjml-0.8.0/tests/missing_functionality_test.py` & `mjml-0.9.0/tests/missing_functionality_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 from pathlib import Path
-from unittest import expectedFailure, TestCase
+from unittest import TestCase, expectedFailure
 
-from ddt import ddt as DataDrivenTestCase, data as ddt_data
+from ddt import data as ddt_data, ddt as DataDrivenTestCase
 from htmlcompare import assert_same_html
 
 from mjml import mjml_to_html
 
 
 TESTDATA_DIR = Path(__file__).parent / 'missing_functionality'
 
@@ -40,9 +40,11 @@
 def _patch_nose1_result(test):
     # nose's TextTestResult does not support "expected failures" but I still
     # like that test runner. Just treat an expected failure like a skipped test.
     result = test._outcome.result
     if not hasattr(result, 'addExpectedFailure'):
         result.addExpectedFailure = result.addSkip
     if not hasattr(result, 'addUnexpectedSuccess'):
-        result.addUnexpectedSuccess = lambda test: result.addFailure(test, (AssertionError, AssertionError('unexpected success'), None))
-
+        def _addUnexpectedSuccess(test):
+            error = (AssertionError, AssertionError('unexpected success'), None)
+            return result.addFailure(test, error)
+        result.addUnexpectedSuccess = _addUnexpectedSuccess
```

### Comparing `mjml-0.8.0/tests/mj_button_mailto_link_test.py` & `mjml-0.9.0/tests/mj_button_mailto_link_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 
-from io import StringIO
 import re
+from io import StringIO
 from unittest import TestCase
 
 import lxml.html
 
 from mjml import mjml_to_html
 
 
-
 class MjButtonMailtoLinkTest(TestCase):
     def test_no_target_for_mailto_links(self):
         mjml = (
             '<mjml>'
             '  <mj-body>'
             '    <mj-button href="mailto:foo@site.example">Click me</mj-button>'
             '  </mj-body>'
@@ -30,8 +29,7 @@
         target = a_el.attrib.get('target')
         # Thunderbird opens a blank page instead of the new message window if
         # the <a> contains 'target="_blank"'.
         #   https://bugzilla.mozilla.org/show_bug.cgi?id=1677248
         #   https://bugzilla.mozilla.org/show_bug.cgi?id=1589968
         #   https://bugzilla.mozilla.org/show_bug.cgi?id=421310
         assert not target, f'target="{target}"'
-
```

### Comparing `mjml-0.8.0/tests/testdata/button-expected.html` & `mjml-0.9.0/tests/testdata/button-expected.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 <!doctype html>
 <html xmlns="http://www.w3.org/1999/xhtml" xmlns:v="urn:schemas-microsoft-com:vml" xmlns:o="urn:schemas-microsoft-com:office:office">
 
 <head>
-  <title>
-  </title>
+  <title></title>
   <!--[if !mso]><!-->
   <meta http-equiv="X-UA-Compatible" content="IE=edge">
   <!--<![endif]-->
   <meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
   <meta name="viewport" content="width=device-width, initial-scale=1">
   <style type="text/css">
     #outlook a {
```

### Comparing `mjml-0.8.0/tests/testdata/css-inlining-expected.html` & `mjml-0.9.0/tests/testdata/css-inlining-expected.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 <!doctype html>
 <html xmlns="http://www.w3.org/1999/xhtml" xmlns:v="urn:schemas-microsoft-com:vml" xmlns:o="urn:schemas-microsoft-com:office:office">
 
 <head>
-  <title>
-  </title>
+  <title></title>
   <!--[if !mso]><!-->
   <meta http-equiv="X-UA-Compatible" content="IE=edge">
   <!--<![endif]-->
   <meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
   <meta name="viewport" content="width=device-width, initial-scale=1">
   <style type="text/css">
     #outlook a {
```

### Comparing `mjml-0.8.0/tests/testdata/hello-world-expected.html` & `mjml-0.9.0/tests/testdata/hello-world-expected.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 <!doctype html>
 <html xmlns="http://www.w3.org/1999/xhtml" xmlns:v="urn:schemas-microsoft-com:vml" xmlns:o="urn:schemas-microsoft-com:office:office">
 
 <head>
-  <title>
-  </title>
+  <title></title>
   <!--[if !mso]><!-->
   <meta http-equiv="X-UA-Compatible" content="IE=edge">
   <!--<![endif]-->
   <meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
   <meta name="viewport" content="width=device-width, initial-scale=1">
   <style type="text/css">
     #outlook a {
```

### Comparing `mjml-0.8.0/tests/testdata/html-entities-expected.html` & `mjml-0.9.0/tests/testdata/html-entities-expected.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 <!doctype html>
 <html xmlns="http://www.w3.org/1999/xhtml" xmlns:v="urn:schemas-microsoft-com:vml" xmlns:o="urn:schemas-microsoft-com:office:office">
 
 <head>
-  <title>
-  </title>
+  <title></title>
   <!--[if !mso]><!-->
   <meta http-equiv="X-UA-Compatible" content="IE=edge">
   <!--<![endif]-->
   <meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
   <meta name="viewport" content="width=device-width, initial-scale=1">
   <style type="text/css">
     #outlook a {
```

### Comparing `mjml-0.8.0/tests/testdata/html-without-closing-tag-expected.html` & `mjml-0.9.0/tests/testdata/html-without-closing-tag-expected.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 <!doctype html>
 <html xmlns="http://www.w3.org/1999/xhtml" xmlns:v="urn:schemas-microsoft-com:vml" xmlns:o="urn:schemas-microsoft-com:office:office">
 
 <head>
-  <title>
-  </title>
+  <title></title>
   <!--[if !mso]><!-->
   <meta http-equiv="X-UA-Compatible" content="IE=edge">
   <!--<![endif]-->
   <meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
   <meta name="viewport" content="width=device-width, initial-scale=1">
   <style type="text/css">
     #outlook a {
```

### Comparing `mjml-0.8.0/tests/testdata/minimal-expected.html` & `mjml-0.9.0/tests/testdata/minimal-expected.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 <!doctype html>
 <html xmlns="http://www.w3.org/1999/xhtml" xmlns:v="urn:schemas-microsoft-com:vml" xmlns:o="urn:schemas-microsoft-com:office:office">
 
 <head>
-  <title>
-  </title>
+  <title></title>
   <!--[if !mso]><!-->
   <meta http-equiv="X-UA-Compatible" content="IE=edge">
   <!--<![endif]-->
   <meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
   <meta name="viewport" content="width=device-width, initial-scale=1">
   <style type="text/css">
     #outlook a {
```

### Comparing `mjml-0.8.0/tests/testdata/missing-whitespace-before-tag-expected.html` & `mjml-0.9.0/tests/testdata/missing-whitespace-before-tag-expected.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 <!doctype html>
 <html xmlns="http://www.w3.org/1999/xhtml" xmlns:v="urn:schemas-microsoft-com:vml" xmlns:o="urn:schemas-microsoft-com:office:office">
 
 <head>
-  <title>
-  </title>
+  <title></title>
   <!--[if !mso]><!-->
   <meta http-equiv="X-UA-Compatible" content="IE=edge">
   <!--<![endif]-->
   <meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
   <meta name="viewport" content="width=device-width, initial-scale=1">
   <style type="text/css">
     #outlook a {
```

### Comparing `mjml-0.8.0/tests/testdata/mj-attributes-expected.html` & `mjml-0.9.0/tests/testdata/mj-attributes-expected.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 <!doctype html>
 <html xmlns="http://www.w3.org/1999/xhtml" xmlns:v="urn:schemas-microsoft-com:vml" xmlns:o="urn:schemas-microsoft-com:office:office">
 
 <head>
-  <title>
-  </title>
+  <title></title>
   <!--[if !mso]><!-->
   <meta http-equiv="X-UA-Compatible" content="IE=edge">
   <!--<![endif]-->
   <meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
   <meta name="viewport" content="width=device-width, initial-scale=1">
   <style type="text/css">
     #outlook a {
```

### Comparing `mjml-0.8.0/tests/testdata/mj-body-with-background-color-expected.html` & `mjml-0.9.0/tests/testdata/mj-body-with-background-color-expected.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 <!doctype html>
 <html xmlns="http://www.w3.org/1999/xhtml" xmlns:v="urn:schemas-microsoft-com:vml" xmlns:o="urn:schemas-microsoft-com:office:office">
 
 <head>
-  <title>
-  </title>
+  <title></title>
   <!--[if !mso]><!-->
   <meta http-equiv="X-UA-Compatible" content="IE=edge">
   <!--<![endif]-->
   <meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
   <meta name="viewport" content="width=device-width, initial-scale=1">
   <style type="text/css">
     #outlook a {
```

### Comparing `mjml-0.8.0/tests/testdata/mj-button-with-width-expected.html` & `mjml-0.9.0/tests/testdata/mj-button-with-width-expected.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 <!doctype html>
 <html xmlns="http://www.w3.org/1999/xhtml" xmlns:v="urn:schemas-microsoft-com:vml" xmlns:o="urn:schemas-microsoft-com:office:office">
 
 <head>
-  <title>
-  </title>
+  <title></title>
   <!--[if !mso]><!-->
   <meta http-equiv="X-UA-Compatible" content="IE=edge">
   <!--<![endif]-->
   <meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
   <meta name="viewport" content="width=device-width, initial-scale=1">
   <style type="text/css">
     #outlook a {
```

### Comparing `mjml-0.8.0/tests/testdata/mj-column-with-attributes-expected.html` & `mjml-0.9.0/tests/testdata/mj-column-with-attributes-expected.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 <!doctype html>
 <html xmlns="http://www.w3.org/1999/xhtml" xmlns:v="urn:schemas-microsoft-com:vml" xmlns:o="urn:schemas-microsoft-com:office:office">
 
 <head>
-  <title>
-  </title>
+  <title></title>
   <!--[if !mso]><!-->
   <meta http-equiv="X-UA-Compatible" content="IE=edge">
   <!--<![endif]-->
   <meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
   <meta name="viewport" content="width=device-width, initial-scale=1">
   <style type="text/css">
     #outlook a {
```

### Comparing `mjml-0.8.0/tests/testdata/mj-font-expected.html` & `mjml-0.9.0/tests/testdata/mj-font-expected.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 <!doctype html>
 <html xmlns="http://www.w3.org/1999/xhtml" xmlns:v="urn:schemas-microsoft-com:vml" xmlns:o="urn:schemas-microsoft-com:office:office">
 
 <head>
-  <title>
-  </title>
+  <title></title>
   <!--[if !mso]><!-->
   <meta http-equiv="X-UA-Compatible" content="IE=edge">
   <!--<![endif]-->
   <meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
   <meta name="viewport" content="width=device-width, initial-scale=1">
   <style type="text/css">
     #outlook a {
```

### Comparing `mjml-0.8.0/tests/testdata/mj-font-multiple-expected.html` & `mjml-0.9.0/tests/testdata/mj-font-multiple-expected.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 <!doctype html>
 <html xmlns="http://www.w3.org/1999/xhtml" xmlns:v="urn:schemas-microsoft-com:vml" xmlns:o="urn:schemas-microsoft-com:office:office">
 
 <head>
-  <title>
-  </title>
+  <title></title>
   <!--[if !mso]><!-->
   <meta http-equiv="X-UA-Compatible" content="IE=edge">
   <!--<![endif]-->
   <meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
   <meta name="viewport" content="width=device-width, initial-scale=1">
   <style type="text/css">
     #outlook a {
```

### Comparing `mjml-0.8.0/tests/testdata/mj-font-unused-expected.html` & `mjml-0.9.0/tests/testdata/mj-font-unused-expected.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 <!doctype html>
 <html xmlns="http://www.w3.org/1999/xhtml" xmlns:v="urn:schemas-microsoft-com:vml" xmlns:o="urn:schemas-microsoft-com:office:office">
 
 <head>
-  <title>
-  </title>
+  <title></title>
   <!--[if !mso]><!-->
   <meta http-equiv="X-UA-Compatible" content="IE=edge">
   <!--<![endif]-->
   <meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
   <meta name="viewport" content="width=device-width, initial-scale=1">
   <style type="text/css">
     #outlook a {
```

### Comparing `mjml-0.8.0/tests/testdata/mj-group-expected.html` & `mjml-0.9.0/tests/testdata/mj-group-expected.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 <!doctype html>
 <html xmlns="http://www.w3.org/1999/xhtml" xmlns:v="urn:schemas-microsoft-com:vml" xmlns:o="urn:schemas-microsoft-com:office:office">
 
 <head>
-  <title>
-  </title>
+  <title></title>
   <!--[if !mso]><!-->
   <meta http-equiv="X-UA-Compatible" content="IE=edge">
   <!--<![endif]-->
   <meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
   <meta name="viewport" content="width=device-width, initial-scale=1">
   <style type="text/css">
     #outlook a {
```

### Comparing `mjml-0.8.0/tests/testdata/mj-head-with-comment-expected.html` & `mjml-0.9.0/tests/testdata/mj-head-with-comment-expected.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 <!doctype html>
 <html xmlns="http://www.w3.org/1999/xhtml" xmlns:v="urn:schemas-microsoft-com:vml" xmlns:o="urn:schemas-microsoft-com:office:office">
 
 <head>
-  <title>
-  </title>
+  <title></title>
   <!--[if !mso]><!-->
   <meta http-equiv="X-UA-Compatible" content="IE=edge">
   <!--<![endif]-->
   <meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
   <meta name="viewport" content="width=device-width, initial-scale=1">
   <style type="text/css">
     #outlook a {
```

### Comparing `mjml-0.8.0/tests/testdata/mj-image-with-empty-alt-attribute-expected.html` & `mjml-0.9.0/tests/testdata/mj-image-with-empty-alt-attribute-expected.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 <!doctype html>
 <html xmlns="http://www.w3.org/1999/xhtml" xmlns:v="urn:schemas-microsoft-com:vml" xmlns:o="urn:schemas-microsoft-com:office:office">
 
 <head>
-  <title>
-  </title>
+  <title></title>
   <!--[if !mso]><!-->
   <meta http-equiv="X-UA-Compatible" content="IE=edge">
   <!--<![endif]-->
   <meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
   <meta name="viewport" content="width=device-width, initial-scale=1">
   <style type="text/css">
     #outlook a {
```

### Comparing `mjml-0.8.0/tests/testdata/mj-image-with-href-expected.html` & `mjml-0.9.0/tests/testdata/mj-image-with-href-expected.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 <!doctype html>
 <html xmlns="http://www.w3.org/1999/xhtml" xmlns:v="urn:schemas-microsoft-com:vml" xmlns:o="urn:schemas-microsoft-com:office:office">
 
 <head>
-  <title>
-  </title>
+  <title></title>
   <!--[if !mso]><!-->
   <meta http-equiv="X-UA-Compatible" content="IE=edge">
   <!--<![endif]-->
   <meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
   <meta name="viewport" content="width=device-width, initial-scale=1">
   <style type="text/css">
     #outlook a {
```

### Comparing `mjml-0.8.0/tests/testdata/mj-include-body-expected.html` & `mjml-0.9.0/tests/testdata/mj-include-body-expected.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 <!doctype html>
 <html xmlns="http://www.w3.org/1999/xhtml" xmlns:v="urn:schemas-microsoft-com:vml" xmlns:o="urn:schemas-microsoft-com:office:office">
 
 <head>
-  <title>
-  </title>
+  <title></title>
   <!--[if !mso]><!-->
   <meta http-equiv="X-UA-Compatible" content="IE=edge">
   <!--<![endif]-->
   <meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
   <meta name="viewport" content="width=device-width, initial-scale=1">
   <style type="text/css">
     #outlook a {
```

### Comparing `mjml-0.8.0/tests/testdata/mj-preview-expected.html` & `mjml-0.9.0/tests/testdata/mj-preview-expected.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 <!doctype html>
 <html xmlns="http://www.w3.org/1999/xhtml" xmlns:v="urn:schemas-microsoft-com:vml" xmlns:o="urn:schemas-microsoft-com:office:office">
 
 <head>
-  <title>
-  </title>
+  <title></title>
   <!--[if !mso]><!-->
   <meta http-equiv="X-UA-Compatible" content="IE=edge">
   <!--<![endif]-->
   <meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
   <meta name="viewport" content="width=device-width, initial-scale=1">
   <style type="text/css">
     #outlook a {
@@ -84,15 +83,15 @@
   <style type="text/css">
   </style>
   <style type="text/css">
   </style>
 </head>
 
 <body style="word-spacing:normal;">
-  <div style="display:none;font-size:1px;color:#ffffff;line-height:1px;max-height:0px;max-width:0px;opacity:0;overflow:hidden;"> Hello MJML </div>
+  <div style="display:none;font-size:1px;color:#ffffff;line-height:1px;max-height:0px;max-width:0px;opacity:0;overflow:hidden;">Hello MJML</div>
   <div style="">
     <!--[if mso | IE]><table align="center" border="0" cellpadding="0" cellspacing="0" class="" role="presentation" style="width:600px;" width="600" ><tr><td style="line-height:0px;font-size:0px;mso-line-height-rule:exactly;"><![endif]-->
     <div style="margin:0px auto;max-width:600px;">
       <table align="center" border="0" cellpadding="0" cellspacing="0" role="presentation" style="width:100%;">
         <tbody>
           <tr>
             <td style="direction:ltr;font-size:0px;padding:20px 0;text-align:center;">
```

### Comparing `mjml-0.8.0/tests/testdata/mj-raw-expected.html` & `mjml-0.9.0/tests/testdata/mj-raw-expected.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 <!doctype html>
 <html xmlns="http://www.w3.org/1999/xhtml" xmlns:v="urn:schemas-microsoft-com:vml" xmlns:o="urn:schemas-microsoft-com:office:office">
 
 <head>
-  <title>
-  </title>
+  <title></title>
   <!--[if !mso]><!-->
   <meta http-equiv="X-UA-Compatible" content="IE=edge">
   <!--<![endif]-->
   <meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
   <meta name="viewport" content="width=device-width, initial-scale=1">
   <style type="text/css">
     #outlook a {
```

### Comparing `mjml-0.8.0/tests/testdata/mj-raw-head-expected.html` & `mjml-0.9.0/tests/testdata/mj-breakpoint-expected.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 <!doctype html>
 <html xmlns="http://www.w3.org/1999/xhtml" xmlns:v="urn:schemas-microsoft-com:vml" xmlns:o="urn:schemas-microsoft-com:office:office">
 
 <head>
-  <title>
-  </title>
+  <title></title>
   <!--[if !mso]><!-->
   <meta http-equiv="X-UA-Compatible" content="IE=edge">
   <!--<![endif]-->
   <meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
   <meta name="viewport" content="width=device-width, initial-scale=1">
   <style type="text/css">
     #outlook a {
@@ -62,34 +61,33 @@
   <link href="https://fonts.googleapis.com/css?family=Ubuntu:300,400,500,700" rel="stylesheet" type="text/css">
   <style type="text/css">
     @import url(https://fonts.googleapis.com/css?family=Ubuntu:300,400,500,700);
 
   </style>
   <!--<![endif]-->
   <style type="text/css">
-    @media only screen and (min-width:480px) {
+    @media only screen and (min-width:100px) {
       .mj-column-per-100 {
         width: 100% !important;
         max-width: 100%;
       }
     }
 
   </style>
-  <style media="screen and (min-width:480px)">
+  <style media="screen and (min-width:100px)">
     .moz-text-html .mj-column-per-100 {
       width: 100% !important;
       max-width: 100%;
     }
 
   </style>
   <style type="text/css">
   </style>
   <style type="text/css">
   </style>
-  <!-- Your content goes here -->
 </head>
 
 <body style="word-spacing:normal;">
   <div style="">
     <!--[if mso | IE]><table align="center" border="0" cellpadding="0" cellspacing="0" class="" role="presentation" style="width:600px;" width="600" ><tr><td style="line-height:0px;font-size:0px;mso-line-height-rule:exactly;"><![endif]-->
     <div style="margin:0px auto;max-width:600px;">
       <table align="center" border="0" cellpadding="0" cellspacing="0" role="presentation" style="width:100%;">
```

#### html2text {}

```diff
@@ -1,7 +1,6 @@
 
 
 
 
 
-
                                  Hello World!
```

### Comparing `mjml-0.8.0/tests/testdata/mj-raw-head-with-tags-expected.html` & `mjml-0.9.0/tests/testdata/mj-raw-head-with-tags-expected.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 <!doctype html>
 <html xmlns="http://www.w3.org/1999/xhtml" xmlns:v="urn:schemas-microsoft-com:vml" xmlns:o="urn:schemas-microsoft-com:office:office">
 
 <head>
-  <title>
-  </title>
+  <title></title>
   <!--[if !mso]><!-->
   <meta http-equiv="X-UA-Compatible" content="IE=edge">
   <!--<![endif]-->
   <meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
   <meta name="viewport" content="width=device-width, initial-scale=1">
   <style type="text/css">
     #outlook a {
```

### Comparing `mjml-0.8.0/tests/testdata/mj-raw-with-tags-expected.html` & `mjml-0.9.0/tests/testdata/mj-raw-with-tags-expected.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 <!doctype html>
 <html xmlns="http://www.w3.org/1999/xhtml" xmlns:v="urn:schemas-microsoft-com:vml" xmlns:o="urn:schemas-microsoft-com:office:office">
 
 <head>
-  <title>
-  </title>
+  <title></title>
   <!--[if !mso]><!-->
   <meta http-equiv="X-UA-Compatible" content="IE=edge">
   <!--<![endif]-->
   <meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
   <meta name="viewport" content="width=device-width, initial-scale=1">
   <style type="text/css">
     #outlook a {
```

### Comparing `mjml-0.8.0/tests/testdata/mj-section-with-background-url-expected.html` & `mjml-0.9.0/tests/testdata/mj-section-with-background-url-expected.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 <!doctype html>
 <html xmlns="http://www.w3.org/1999/xhtml" xmlns:v="urn:schemas-microsoft-com:vml" xmlns:o="urn:schemas-microsoft-com:office:office">
 
 <head>
-  <title>
-  </title>
+  <title></title>
   <!--[if !mso]><!-->
   <meta http-equiv="X-UA-Compatible" content="IE=edge">
   <!--<![endif]-->
   <meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
   <meta name="viewport" content="width=device-width, initial-scale=1">
   <style type="text/css">
     #outlook a {
```

### Comparing `mjml-0.8.0/tests/testdata/mj-section-with-mj-class-expected.html` & `mjml-0.9.0/tests/testdata/mj-section-with-mj-class-expected.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 <!doctype html>
 <html xmlns="http://www.w3.org/1999/xhtml" xmlns:v="urn:schemas-microsoft-com:vml" xmlns:o="urn:schemas-microsoft-com:office:office">
 
 <head>
-  <title>
-  </title>
+  <title></title>
   <!--[if !mso]><!-->
   <meta http-equiv="X-UA-Compatible" content="IE=edge">
   <!--<![endif]-->
   <meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
   <meta name="viewport" content="width=device-width, initial-scale=1">
   <style type="text/css">
     #outlook a {
```

### Comparing `mjml-0.8.0/tests/testdata/mj-style-expected.html` & `mjml-0.9.0/tests/testdata/mj-style-expected.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 <!doctype html>
 <html xmlns="http://www.w3.org/1999/xhtml" xmlns:v="urn:schemas-microsoft-com:vml" xmlns:o="urn:schemas-microsoft-com:office:office">
 
 <head>
-  <title>
-  </title>
+  <title></title>
   <!--[if !mso]><!-->
   <meta http-equiv="X-UA-Compatible" content="IE=edge">
   <!--<![endif]-->
   <meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
   <meta name="viewport" content="width=device-width, initial-scale=1">
   <style type="text/css">
     #outlook a {
```

### Comparing `mjml-0.8.0/tests/testdata/mj-table-expected.html` & `mjml-0.9.0/tests/testdata/mj-table-expected.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 <!doctype html>
 <html xmlns="http://www.w3.org/1999/xhtml" xmlns:v="urn:schemas-microsoft-com:vml" xmlns:o="urn:schemas-microsoft-com:office:office">
 
 <head>
-  <title>
-  </title>
+  <title></title>
   <!--[if !mso]><!-->
   <meta http-equiv="X-UA-Compatible" content="IE=edge">
   <!--<![endif]-->
   <meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
   <meta name="viewport" content="width=device-width, initial-scale=1">
   <style type="text/css">
     #outlook a {
```

### Comparing `mjml-0.8.0/tests/testdata/mj-text-with-tail-text-expected.html` & `mjml-0.9.0/tests/testdata/mj-text-with-tail-text-expected.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 <!doctype html>
 <html xmlns="http://www.w3.org/1999/xhtml" xmlns:v="urn:schemas-microsoft-com:vml" xmlns:o="urn:schemas-microsoft-com:office:office">
 
 <head>
-  <title>
-  </title>
+  <title></title>
   <!--[if !mso]><!-->
   <meta http-equiv="X-UA-Compatible" content="IE=edge">
   <!--<![endif]-->
   <meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
   <meta name="viewport" content="width=device-width, initial-scale=1">
   <style type="text/css">
     #outlook a {
```

### Comparing `mjml-0.8.0/tests/testdata/mj-title-expected.html` & `mjml-0.9.0/tests/testdata/mj-title-expected.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 <!doctype html>
 <html xmlns="http://www.w3.org/1999/xhtml" xmlns:v="urn:schemas-microsoft-com:vml" xmlns:o="urn:schemas-microsoft-com:office:office">
 
 <head>
-  <title> Hello MJML </title>
+  <title>Hello MJML</title>
   <!--[if !mso]><!-->
   <meta http-equiv="X-UA-Compatible" content="IE=edge">
   <!--<![endif]-->
   <meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
   <meta name="viewport" content="width=device-width, initial-scale=1">
   <style type="text/css">
     #outlook a {
```

### Comparing `mjml-0.8.0/tests/testdata/text_with_html-expected.html` & `mjml-0.9.0/tests/testdata/text_with_html-expected.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 <!doctype html>
 <html xmlns="http://www.w3.org/1999/xhtml" xmlns:v="urn:schemas-microsoft-com:vml" xmlns:o="urn:schemas-microsoft-com:office:office">
 
 <head>
-  <title>
-  </title>
+  <title></title>
   <!--[if !mso]><!-->
   <meta http-equiv="X-UA-Compatible" content="IE=edge">
   <!--<![endif]-->
   <meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
   <meta name="viewport" content="width=device-width, initial-scale=1">
   <style type="text/css">
     #outlook a {
```

### Comparing `mjml-0.8.0/tests/upstream_alignment_test.py` & `mjml-0.9.0/tests/upstream_alignment_test.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,55 +1,61 @@
 
-from contextlib import contextmanager
 from json import load as json_load
-from pathlib import Path
 from unittest import SkipTest, TestCase
 
 from bs4 import BeautifulSoup
-from ddt import ddt as DataDrivenTestCase, data as ddt_data
+from ddt import data as ddt_data, ddt as DataDrivenTestCase
 from htmlcompare import assert_same_html
 
 from mjml import mjml_to_html
+from mjml.testing_helpers import get_mjml_fp, load_expected_html
 
 
-
-TESTDATA_DIR = Path(__file__).parent / 'testdata'
-
 @DataDrivenTestCase
 class UpstreamAlignmentTest(TestCase):
     @ddt_data(
         'minimal',
         'hello-world',
         'html-entities',
         'html-without-closing-tag',
         'button',
         'text_with_html',
         'mj-body-with-background-color',
+        'mj-breakpoint',
         'mj-title',
         'mj-style',
+        'mj-accordion',
         'mj-attributes',
+        'mj-html-attributes',
         'mj-column-with-attributes',
         'mj-group',
+        'mj-hero-fixed',
+        'mj-hero-fluid',
         'mj-button-with-width',
         'mj-text-with-tail-text',
         'mj-table',
         'mj-head-with-comment',
         'mj-image-with-empty-alt-attribute',
         'mj-image-with-href',
+        'mj-section-with-full-width',
+        'mj-section-with-css-class',
         'mj-section-with-mj-class',
         'mj-section-with-background-url',
         'mj-font',
         'mj-font-multiple',
         'mj-font-unused',
         'mj-include-body',
         'mj-preview',
         'mj-raw',
         'mj-raw-with-tags',
         'mj-raw-head',
         'mj-raw-head-with-tags',
+        'mj-social',
+        'mj-spacer',
+        'mj-wrapper',
     )
     def test_ensure_same_html(self, test_id):
         expected_html = load_expected_html(test_id)
         with get_mjml_fp(test_id) as mjml_fp:
             result = mjml_to_html(mjml_fp)
 
         assert not result.errors
@@ -75,51 +81,74 @@
 
         assert not result.errors
         actual_html = result.html
         assert_same_html(expected_html, actual_html, verbose=True)
 
     def test_can_use_css_inlining(self):
         try:
-            import css_inline
+            import css_inline  # noqa: unused-import
         except ImportError:
             raise SkipTest('"css_inline" not installed')
         test_id = 'css-inlining'
         expected_html = load_expected_html(test_id)
         with get_mjml_fp(test_id) as mjml_fp:
             mjml_str = mjml_fp.read().decode('utf8')
             result = mjml_to_html(mjml_str)
 
         assert not result.errors
         assert_same_html(expected_html, result.html, verbose=True)
 
+    # The dynamically generated menu key prevents us from just using
+    # test_ensure_same_html to test mj-navbar
+    def test_mj_navbar(self):
+        test_id = 'mj-navbar'
+        expected_html = load_expected_html(test_id)
+        with get_mjml_fp(test_id) as mjml_fp:
+            result = mjml_to_html(mjml_fp)
+
+        assert not result.errors
+        expected_soup = BeautifulSoup(expected_html, 'html.parser')
+        actual_soup = BeautifulSoup(result.html, 'html.parser')
+
+        # This key is randomly generated, so we need to manually replace it.
+        menuKey = actual_soup.find(attrs={'class': 'mj-menu-checkbox'})['id']
+        expected_soup.find(attrs={'class': 'mj-menu-checkbox'})['id'] = menuKey
+        expected_soup.find(attrs={'class': 'mj-menu-label'})['for'] = menuKey
+
+        assert_same_html(str(expected_soup), str(actual_soup), verbose=True)
+
+    # The dynamically generated carousel ID prevents us from just using
+    # test_ensure_same_html to test mj-carousel
+    def test_mj_carousel(self):
+        test_id = 'mj-carousel'
+        expected_html = load_expected_html(test_id)
+        with get_mjml_fp(test_id) as mjml_fp:
+            result = mjml_to_html(mjml_fp)
+
+        assert not result.errors
+        expected_soup = BeautifulSoup(expected_html, 'html.parser')
+        actual_soup = BeautifulSoup(result.html, 'html.parser')
+
+        # This ID is randomly generated, so we need to manually replace it.
+        def _replace_random_radio_class(soup):
+            _mj_cr_str = 'mj-carousel-radio'
+            return soup.find(attrs={'class': _mj_cr_str})['name'].replace(f'{_mj_cr_str}-', '')
+        expected_carousel_id = _replace_random_radio_class(expected_soup)
+        actual_carousel_id = _replace_random_radio_class(actual_soup)
+        actual_html = str(actual_soup).replace(actual_carousel_id, expected_carousel_id)
+        assert_same_html(str(expected_soup), actual_html, verbose=True)
+
     # htmlcompare is currently unable to detect these kind of
     # whitespace differences.
     def test_keep_whitespace_before_tag(self):
         test_id = 'missing-whitespace-before-tag'
         expected_html = load_expected_html(test_id)
         with get_mjml_fp(test_id) as mjml_fp:
             result = mjml_to_html(mjml_fp)
 
         assert not result.errors
         expected_text = BeautifulSoup(expected_html, 'html.parser').body.get_text().strip()
         body_actual = BeautifulSoup(result.html, 'html.parser').body
         actual_text = body_actual.get_text().strip()
         assert (expected_text == actual_text)
-        actual_html = (body_actual.select('table > tr > td > div')[0]).renderContents()
+        actual_html = (body_actual.select('.mj-column-per-100 div')[0]).renderContents()
         assert (b'foo <b>bar</b>.' == actual_html)
-
-
-
-def load_expected_html(test_id):
-    html_filename = f'{test_id}-expected.html'
-    with (TESTDATA_DIR / html_filename).open('rb') as html_fp:
-        expected_html = html_fp.read()
-    return expected_html
-
-@contextmanager
-def get_mjml_fp(test_id, json=False):
-    mjml_filename = f'{test_id}.mjml'
-    if json:
-        mjml_filename += '.json'
-    with (TESTDATA_DIR / mjml_filename).open('rb') as mjml_fp:
-        yield mjml_fp
-
```

### Comparing `mjml-0.8.0/tools/update-expected-html.py` & `mjml-0.9.0/tools/update-expected-html.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 options:
   -h, --help        show this help message and exit
   --single-process  run HTML generation in a single process (slower but easier
                     to debug)
 """
 
 import argparse
-from collections import namedtuple
-from multiprocessing import Pool
 import os
-from pathlib import Path
 import subprocess
 import sys
+from collections import namedtuple
+from multiprocessing import Pool
+from pathlib import Path
 
 
 Job = namedtuple('Job', ('mjml_path', 'expected_path', 'mjml_bin'))
 
 def job_for_file(mjml_path, mjml_js):
     expected_path = mjml_path.parent / (mjml_path.stem + '-expected.html')
     return Job(
@@ -89,8 +89,7 @@
             _update_expected_html(job)
     else:
         with Pool() as p:
             p.map(_update_expected_html, jobs)
 
 if __name__ == '__main__':
     main()
-
```

