# Comparing `tmp/pagure-messages-0.0.6.tar.gz` & `tmp/pagure-messages-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pagure-messages-0.0.6.tar", last modified: Tue Feb  2 14:52:51 2021, max compression
+gzip compressed data, was "pagure-messages-1.0.0.tar", last modified: Thu May 25 09:17:59 2023, max compression
```

## Comparing `pagure-messages-0.0.6.tar` & `pagure-messages-1.0.0.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 pierrey   (1000) pierrey   (1000)        0 2021-02-02 14:52:51.450344 pagure-messages-0.0.6/
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)    18092 2020-10-13 13:54:45.000000 pagure-messages-0.0.6/LICENSE
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)       24 2020-10-13 13:54:45.000000 pagure-messages-0.0.6/MANIFEST.in
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)     1001 2021-02-02 14:52:51.450344 pagure-messages-0.0.6/PKG-INFO
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)      202 2020-10-13 13:54:45.000000 pagure-messages-0.0.6/README.md
-drwxr-xr-x   0 pierrey   (1000) pierrey   (1000)        0 2021-02-02 14:52:51.442345 pagure-messages-0.0.6/pagure_messages/
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)     2551 2020-10-27 15:21:38.000000 pagure-messages-0.0.6/pagure_messages/__init__.py
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)    11681 2021-02-02 14:52:19.000000 pagure-messages-0.0.6/pagure_messages/base.py
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)     9426 2021-01-08 14:43:02.000000 pagure-messages-0.0.6/pagure_messages/git_schema.py
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)    15705 2021-01-08 14:43:02.000000 pagure-messages-0.0.6/pagure_messages/issue_schema.py
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)     6413 2021-01-08 14:43:02.000000 pagure-messages-0.0.6/pagure_messages/misc_schema.py
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)    16909 2021-01-08 14:43:02.000000 pagure-messages-0.0.6/pagure_messages/project_schema.py
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)    21713 2021-01-08 14:43:02.000000 pagure-messages-0.0.6/pagure_messages/pull_requests_schema.py
-drwxr-xr-x   0 pierrey   (1000) pierrey   (1000)        0 2021-02-02 14:52:51.450344 pagure-messages-0.0.6/pagure_messages/tests/
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)        0 2020-10-13 13:54:45.000000 pagure-messages-0.0.6/pagure_messages/tests/__init__.py
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)     2485 2021-01-08 14:43:02.000000 pagure-messages-0.0.6/pagure_messages/tests/test_commit_flag_added.py
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)     2496 2021-01-08 14:43:02.000000 pagure-messages-0.0.6/pagure_messages/tests/test_commit_flag_updated.py
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)     1467 2020-10-21 08:53:59.000000 pagure-messages-0.0.6/pagure_messages/tests/test_common.py
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)     4110 2021-01-08 14:43:02.000000 pagure-messages-0.0.6/pagure_messages/tests/test_git_branch_creation.py
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)     3372 2021-01-08 14:43:02.000000 pagure-messages-0.0.6/pagure_messages/tests/test_git_branch_deletion.py
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)     4716 2020-10-21 09:31:46.000000 pagure-messages-0.0.6/pagure_messages/tests/test_git_receive.py
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)     3337 2021-01-08 14:43:02.000000 pagure-messages-0.0.6/pagure_messages/tests/test_git_tag_creation.py
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)     3321 2021-01-08 14:43:02.000000 pagure-messages-0.0.6/pagure_messages/tests/test_git_tag_deletion.py
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)     2393 2021-01-08 14:43:02.000000 pagure-messages-0.0.6/pagure_messages/tests/test_group_edit.py
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)     2682 2021-01-08 14:43:02.000000 pagure-messages-0.0.6/pagure_messages/tests/test_issue_assigned_added.py
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)     2380 2021-01-08 14:43:02.000000 pagure-messages-0.0.6/pagure_messages/tests/test_issue_assigned_reset.py
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)     2391 2021-01-08 14:43:02.000000 pagure-messages-0.0.6/pagure_messages/tests/test_issue_comment_added.py
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)     2550 2021-01-08 14:43:02.000000 pagure-messages-0.0.6/pagure_messages/tests/test_issue_dependency_added.py
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)     2608 2021-01-08 14:43:02.000000 pagure-messages-0.0.6/pagure_messages/tests/test_issue_dependency_removed.py
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)     2401 2021-01-08 14:43:02.000000 pagure-messages-0.0.6/pagure_messages/tests/test_issue_drop.py
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)     2496 2021-01-08 14:43:02.000000 pagure-messages-0.0.6/pagure_messages/tests/test_issue_edit.py
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)     2347 2021-01-08 14:43:02.000000 pagure-messages-0.0.6/pagure_messages/tests/test_issue_new.py
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)     2486 2021-01-08 14:43:02.000000 pagure-messages-0.0.6/pagure_messages/tests/test_issue_tag_added.py
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)     2538 2021-01-08 14:43:02.000000 pagure-messages-0.0.6/pagure_messages/tests/test_issue_tag_removed.py
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)     1460 2020-10-20 13:29:18.000000 pagure-messages-0.0.6/pagure_messages/tests/test_object_from_topic.py
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)     2178 2020-10-21 08:52:47.000000 pagure-messages-0.0.6/pagure_messages/tests/test_project_deleted.py
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)     2405 2021-01-08 14:43:02.000000 pagure-messages-0.0.6/pagure_messages/tests/test_project_edit.py
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)     2192 2021-01-08 14:43:02.000000 pagure-messages-0.0.6/pagure_messages/tests/test_project_forked.py
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)     2543 2021-01-08 14:43:02.000000 pagure-messages-0.0.6/pagure_messages/tests/test_project_group_access_updated.py
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)     2484 2021-01-08 14:43:02.000000 pagure-messages-0.0.6/pagure_messages/tests/test_project_group_added.py
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)     2501 2021-01-08 14:43:02.000000 pagure-messages-0.0.6/pagure_messages/tests/test_project_group_removed.py
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)     2195 2021-01-08 14:43:02.000000 pagure-messages-0.0.6/pagure_messages/tests/test_project_new.py
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)     2360 2021-01-08 14:43:02.000000 pagure-messages-0.0.6/pagure_messages/tests/test_project_tag_edited.py
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)     2369 2021-01-08 14:43:02.000000 pagure-messages-0.0.6/pagure_messages/tests/test_project_tag_removed.py
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)     2500 2021-01-08 14:43:02.000000 pagure-messages-0.0.6/pagure_messages/tests/test_project_user_access_updated.py
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)     2318 2021-01-08 14:43:02.000000 pagure-messages-0.0.6/pagure_messages/tests/test_project_user_added.py
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)     2371 2021-01-08 14:43:02.000000 pagure-messages-0.0.6/pagure_messages/tests/test_project_user_removed.py
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)     2578 2021-01-08 14:43:02.000000 pagure-messages-0.0.6/pagure_messages/tests/test_pull_request_assigned_added.py
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)     2429 2021-01-08 14:43:02.000000 pagure-messages-0.0.6/pagure_messages/tests/test_pull_request_assigned_reset.py
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)     3172 2021-01-08 14:43:02.000000 pagure-messages-0.0.6/pagure_messages/tests/test_pull_request_closed.py
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)     2336 2021-01-08 14:43:02.000000 pagure-messages-0.0.6/pagure_messages/tests/test_pull_request_comment_added.py
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)     2346 2021-01-08 14:43:02.000000 pagure-messages-0.0.6/pagure_messages/tests/test_pull_request_comment_edited.py
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)     2412 2021-01-08 14:43:02.000000 pagure-messages-0.0.6/pagure_messages/tests/test_pull_request_flag_added.py
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)     2427 2021-01-08 14:43:02.000000 pagure-messages-0.0.6/pagure_messages/tests/test_pull_request_flag_updated.py
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)     2494 2021-01-08 14:43:02.000000 pagure-messages-0.0.6/pagure_messages/tests/test_pull_request_initial_comment_edited.py
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)     2306 2021-01-08 14:43:02.000000 pagure-messages-0.0.6/pagure_messages/tests/test_pull_request_new.py
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)     2260 2021-01-08 14:43:02.000000 pagure-messages-0.0.6/pagure_messages/tests/test_pull_request_rebased.py
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)     2269 2021-01-08 14:43:02.000000 pagure-messages-0.0.6/pagure_messages/tests/test_pull_request_reopened.py
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)     2531 2021-01-08 14:43:02.000000 pagure-messages-0.0.6/pagure_messages/tests/test_pull_request_tag_added.py
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)     2564 2021-01-08 14:43:02.000000 pagure-messages-0.0.6/pagure_messages/tests/test_pull_request_tag_removed.py
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)     2260 2021-01-08 14:43:02.000000 pagure-messages-0.0.6/pagure_messages/tests/test_pull_request_updated.py
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)     1929 2020-10-21 08:57:41.000000 pagure-messages-0.0.6/pagure_messages/tests/test_test_notification.py
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)    19998 2021-01-08 14:43:02.000000 pagure-messages-0.0.6/pagure_messages/tests/utils.py
-drwxr-xr-x   0 pierrey   (1000) pierrey   (1000)        0 2021-02-02 14:52:51.443344 pagure-messages-0.0.6/pagure_messages.egg-info/
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)     1001 2021-02-02 14:52:51.000000 pagure-messages-0.0.6/pagure_messages.egg-info/PKG-INFO
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)     2958 2021-02-02 14:52:51.000000 pagure-messages-0.0.6/pagure_messages.egg-info/SOURCES.txt
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)        1 2021-02-02 14:52:51.000000 pagure-messages-0.0.6/pagure_messages.egg-info/dependency_links.txt
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)     3667 2021-02-02 14:52:51.000000 pagure-messages-0.0.6/pagure_messages.egg-info/entry_points.txt
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)        1 2020-10-13 13:57:09.000000 pagure-messages-0.0.6/pagure_messages.egg-info/not-zip-safe
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)       17 2021-02-02 14:52:51.000000 pagure-messages-0.0.6/pagure_messages.egg-info/requires.txt
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)       16 2021-02-02 14:52:51.000000 pagure-messages-0.0.6/pagure_messages.egg-info/top_level.txt
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)     4965 2021-02-02 14:52:51.451344 pagure-messages-0.0.6/setup.cfg
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)       61 2020-11-03 13:06:34.000000 pagure-messages-0.0.6/setup.py
--rw-r--r--   0 pierrey   (1000) pierrey   (1000)      564 2020-10-29 11:44:02.000000 pagure-messages-0.0.6/tox.ini
+drwxr-xr-x   0 abompard  (1000) abompard  (1000)        0 2023-05-25 09:17:59.574225 pagure-messages-1.0.0/
+-rw-r--r--   0 abompard  (1000) abompard  (1000)    18092 2023-05-15 10:07:56.000000 pagure-messages-1.0.0/LICENSE
+-rw-r--r--   0 abompard  (1000) abompard  (1000)       24 2023-05-15 10:07:56.000000 pagure-messages-1.0.0/MANIFEST.in
+-rw-r--r--   0 abompard  (1000) abompard  (1000)      970 2023-05-25 09:17:59.574225 pagure-messages-1.0.0/PKG-INFO
+-rw-r--r--   0 abompard  (1000) abompard  (1000)      202 2023-05-15 10:07:56.000000 pagure-messages-1.0.0/README.md
+drwxr-xr-x   0 abompard  (1000) abompard  (1000)        0 2023-05-25 09:17:59.569225 pagure-messages-1.0.0/pagure_messages/
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2549 2023-05-24 11:23:39.000000 pagure-messages-1.0.0/pagure_messages/__init__.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)    11945 2023-05-24 11:50:07.000000 pagure-messages-1.0.0/pagure_messages/base.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     9683 2023-05-24 11:50:07.000000 pagure-messages-1.0.0/pagure_messages/git_schema.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)    16131 2023-05-24 11:50:07.000000 pagure-messages-1.0.0/pagure_messages/issue_schema.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     6481 2023-05-24 11:50:07.000000 pagure-messages-1.0.0/pagure_messages/misc_schema.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)    17528 2023-05-24 11:50:07.000000 pagure-messages-1.0.0/pagure_messages/project_schema.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)    22019 2023-05-24 11:50:07.000000 pagure-messages-1.0.0/pagure_messages/pull_requests_schema.py
+drwxr-xr-x   0 abompard  (1000) abompard  (1000)        0 2023-05-25 09:17:59.574225 pagure-messages-1.0.0/pagure_messages/tests/
+-rw-r--r--   0 abompard  (1000) abompard  (1000)        0 2023-05-15 10:07:56.000000 pagure-messages-1.0.0/pagure_messages/tests/__init__.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2485 2023-05-24 11:43:37.000000 pagure-messages-1.0.0/pagure_messages/tests/test_commit_flag_added.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2496 2023-05-24 11:43:45.000000 pagure-messages-1.0.0/pagure_messages/tests/test_commit_flag_updated.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     1743 2023-05-24 11:50:07.000000 pagure-messages-1.0.0/pagure_messages/tests/test_common.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     4132 2023-05-24 11:44:01.000000 pagure-messages-1.0.0/pagure_messages/tests/test_git_branch_creation.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     3383 2023-05-24 11:44:08.000000 pagure-messages-1.0.0/pagure_messages/tests/test_git_branch_deletion.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     6039 2023-05-24 11:44:14.000000 pagure-messages-1.0.0/pagure_messages/tests/test_git_receive.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     3356 2023-05-24 11:44:19.000000 pagure-messages-1.0.0/pagure_messages/tests/test_git_tag_creation.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     3356 2023-05-24 11:44:24.000000 pagure-messages-1.0.0/pagure_messages/tests/test_git_tag_deletion.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2393 2023-05-24 11:44:28.000000 pagure-messages-1.0.0/pagure_messages/tests/test_group_edit.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2682 2023-05-24 11:44:36.000000 pagure-messages-1.0.0/pagure_messages/tests/test_issue_assigned_added.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2380 2023-05-24 11:44:41.000000 pagure-messages-1.0.0/pagure_messages/tests/test_issue_assigned_reset.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2391 2023-05-24 11:44:45.000000 pagure-messages-1.0.0/pagure_messages/tests/test_issue_comment_added.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2550 2023-05-24 11:44:49.000000 pagure-messages-1.0.0/pagure_messages/tests/test_issue_dependency_added.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2608 2023-05-24 11:44:54.000000 pagure-messages-1.0.0/pagure_messages/tests/test_issue_dependency_removed.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2401 2023-05-24 11:45:00.000000 pagure-messages-1.0.0/pagure_messages/tests/test_issue_drop.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2496 2023-05-24 11:45:04.000000 pagure-messages-1.0.0/pagure_messages/tests/test_issue_edit.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2347 2023-05-24 11:45:09.000000 pagure-messages-1.0.0/pagure_messages/tests/test_issue_new.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2486 2023-05-24 11:45:15.000000 pagure-messages-1.0.0/pagure_messages/tests/test_issue_tag_added.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2538 2023-05-24 11:45:20.000000 pagure-messages-1.0.0/pagure_messages/tests/test_issue_tag_removed.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     1559 2023-05-24 11:23:39.000000 pagure-messages-1.0.0/pagure_messages/tests/test_object_from_topic.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2219 2023-05-24 11:45:31.000000 pagure-messages-1.0.0/pagure_messages/tests/test_project_deleted.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2405 2023-05-24 11:45:37.000000 pagure-messages-1.0.0/pagure_messages/tests/test_project_edit.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2192 2023-05-24 11:45:43.000000 pagure-messages-1.0.0/pagure_messages/tests/test_project_forked.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2543 2023-05-24 11:45:48.000000 pagure-messages-1.0.0/pagure_messages/tests/test_project_group_access_updated.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2484 2023-05-24 11:45:53.000000 pagure-messages-1.0.0/pagure_messages/tests/test_project_group_added.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2501 2023-05-24 11:45:58.000000 pagure-messages-1.0.0/pagure_messages/tests/test_project_group_removed.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2195 2023-05-24 11:46:04.000000 pagure-messages-1.0.0/pagure_messages/tests/test_project_new.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2360 2023-05-24 11:46:08.000000 pagure-messages-1.0.0/pagure_messages/tests/test_project_tag_edited.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2369 2023-05-24 11:46:12.000000 pagure-messages-1.0.0/pagure_messages/tests/test_project_tag_removed.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2500 2023-05-24 11:46:16.000000 pagure-messages-1.0.0/pagure_messages/tests/test_project_user_access_updated.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2318 2023-05-24 11:46:22.000000 pagure-messages-1.0.0/pagure_messages/tests/test_project_user_added.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2371 2023-05-24 11:46:29.000000 pagure-messages-1.0.0/pagure_messages/tests/test_project_user_removed.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2578 2023-05-24 11:46:34.000000 pagure-messages-1.0.0/pagure_messages/tests/test_pull_request_assigned_added.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2429 2023-05-24 11:46:38.000000 pagure-messages-1.0.0/pagure_messages/tests/test_pull_request_assigned_reset.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     3172 2023-05-24 11:46:43.000000 pagure-messages-1.0.0/pagure_messages/tests/test_pull_request_closed.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2336 2023-05-24 11:46:49.000000 pagure-messages-1.0.0/pagure_messages/tests/test_pull_request_comment_added.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2346 2023-05-24 11:46:53.000000 pagure-messages-1.0.0/pagure_messages/tests/test_pull_request_comment_edited.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2412 2023-05-24 11:46:58.000000 pagure-messages-1.0.0/pagure_messages/tests/test_pull_request_flag_added.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2427 2023-05-24 11:47:02.000000 pagure-messages-1.0.0/pagure_messages/tests/test_pull_request_flag_updated.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2494 2023-05-24 11:47:06.000000 pagure-messages-1.0.0/pagure_messages/tests/test_pull_request_initial_comment_edited.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2306 2023-05-24 11:47:10.000000 pagure-messages-1.0.0/pagure_messages/tests/test_pull_request_new.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2260 2023-05-24 11:47:17.000000 pagure-messages-1.0.0/pagure_messages/tests/test_pull_request_rebased.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2269 2023-05-24 11:47:22.000000 pagure-messages-1.0.0/pagure_messages/tests/test_pull_request_reopened.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2531 2023-05-24 11:47:26.000000 pagure-messages-1.0.0/pagure_messages/tests/test_pull_request_tag_added.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2564 2023-05-24 11:47:29.000000 pagure-messages-1.0.0/pagure_messages/tests/test_pull_request_tag_removed.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2260 2023-05-24 11:47:33.000000 pagure-messages-1.0.0/pagure_messages/tests/test_pull_request_updated.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     1929 2023-05-15 10:07:56.000000 pagure-messages-1.0.0/pagure_messages/tests/test_test_notification.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)    19998 2023-05-15 10:25:11.000000 pagure-messages-1.0.0/pagure_messages/tests/utils.py
+drwxr-xr-x   0 abompard  (1000) abompard  (1000)        0 2023-05-25 09:17:59.570225 pagure-messages-1.0.0/pagure_messages.egg-info/
+-rw-r--r--   0 abompard  (1000) abompard  (1000)      970 2023-05-25 09:17:59.000000 pagure-messages-1.0.0/pagure_messages.egg-info/PKG-INFO
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     2958 2023-05-25 09:17:59.000000 pagure-messages-1.0.0/pagure_messages.egg-info/SOURCES.txt
+-rw-r--r--   0 abompard  (1000) abompard  (1000)        1 2023-05-25 09:17:59.000000 pagure-messages-1.0.0/pagure_messages.egg-info/dependency_links.txt
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     3666 2023-05-25 09:17:59.000000 pagure-messages-1.0.0/pagure_messages.egg-info/entry_points.txt
+-rw-r--r--   0 abompard  (1000) abompard  (1000)        1 2023-05-25 09:17:59.000000 pagure-messages-1.0.0/pagure_messages.egg-info/not-zip-safe
+-rw-r--r--   0 abompard  (1000) abompard  (1000)       17 2023-05-25 09:17:59.000000 pagure-messages-1.0.0/pagure_messages.egg-info/requires.txt
+-rw-r--r--   0 abompard  (1000) abompard  (1000)       16 2023-05-25 09:17:59.000000 pagure-messages-1.0.0/pagure_messages.egg-info/top_level.txt
+-rw-r--r--   0 abompard  (1000) abompard  (1000)     4965 2023-05-25 09:17:59.574225 pagure-messages-1.0.0/setup.cfg
+-rw-r--r--   0 abompard  (1000) abompard  (1000)       61 2023-05-15 10:07:56.000000 pagure-messages-1.0.0/setup.py
+-rw-r--r--   0 abompard  (1000) abompard  (1000)      564 2023-05-15 10:07:56.000000 pagure-messages-1.0.0/tox.ini
```

### Comparing `pagure-messages-0.0.6/LICENSE` & `pagure-messages-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pagure-messages-0.0.6/PKG-INFO` & `pagure-messages-1.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: pagure-messages
-Version: 0.0.6
+Version: 1.0.0
 Summary: A schema package for messages sent by pagure
 Home-page: https://pagure.io/pagure
 Maintainer: Fedora Infrastructure Team
 Maintainer-email: infrastructure@lists.fedoraproject.org
 License: GPLv2+
-Description: # pagure messages
-        
-        A schema package for [pagure](https://pagure.io/pagure).
-        
-        See the [detailed documentation](https://fedora-messaging.readthedocs.io/en/latest/messages.html) on packaging your schemas.
-        
 Keywords: fedora
 Platform: Fedora
 Platform: GNU/Linux
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+License-File: LICENSE
+
+# pagure messages
+
+A schema package for [pagure](https://pagure.io/pagure).
+
+See the [detailed documentation](https://fedora-messaging.readthedocs.io/en/latest/messages.html) on packaging your schemas.
```

### Comparing `pagure-messages-0.0.6/pagure_messages/__init__.py` & `pagure-messages-1.0.0/pagure_messages/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 def get_message_object_from_topic(topic):
     """Returns the Message class corresponding to the topic."""
 
     output = None
 
     for entry_point in pkg_resources.iter_entry_points("fedora.messages"):
         cls = entry_point.load()
-        if cls().topic == topic:
+        if cls.topic == topic:
             output = cls
             break
 
     if output is None:
         output = message.Message
 
     return output
```

### Comparing `pagure-messages-0.0.6/pagure_messages/base.py` & `pagure-messages-1.0.0/pagure_messages/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
+import warnings
 
 from fedora_messaging import message
 from fedora_messaging.schema_utils import user_avatar_url
 
 
 SCHEMA_URL = "http://fedoraproject.org/message-schema/"
 
@@ -410,24 +411,33 @@
         base_url = self.__link__
         if ".stg." in self.topic:  # pragma: no cover
             base_url = self.__stg_link__
         return base_url
 
     @property
     def app_name(self):
-        return "pagure"
+        return "Pagure"
 
     @property
     def app_icon(self):
         return "https://apps.fedoraproject.org/img/icons/pagure.png"
 
     @property
     def agent(self):
+        warnings.warn(
+            "agent property is deprecated, please use agent_name instead",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        return self.agent_name
+
+    @property
+    def agent_name(self):
         return self.body.get("agent")
 
     @property
     def agent_avatar(self):
-        return user_avatar_url(self.agent)
+        return user_avatar_url(self.agent_name)
 
     @property
     def usernames(self):
-        return [self.agent]
+        return [self.agent_name]
```

### Comparing `pagure-messages-0.0.6/pagure_messages/git_schema.py` & `pagure-messages-1.0.0/pagure_messages/git_schema.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,42 @@
 # You should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 
 from .base import GIT_RECEIVE_USER, PROJECT, PagureMessage, SCHEMA_URL
 
 
-class GitBranchCreationV1(PagureMessage):
+class GitMessage(PagureMessage):
+    """
+    Used when git events generate Fedora messages.
+    """
+
+    def _name_if_namespace(self, namespace):
+        if self.body["repo"]["namespace"] == namespace:
+            return [self.body["repo"]["name"]]
+        return []
+
+    @property
+    def packages(self):
+        return self._name_if_namespace("rpms")
+
+    @property
+    def containers(self):
+        return self._name_if_namespace("containers")
+
+    @property
+    def modules(self):
+        return self._name_if_namespace("modules")
+
+    @property
+    def flatpaks(self):
+        return self._name_if_namespace("flatpaks")
+
+
+class GitBranchCreationV1(GitMessage):
     """
     A sub-class of a Fedora message that defines a message schema for messages
     published by pagure when a new thing is created.
     """
 
     topic = "pagure.git.branch.creation"
 
@@ -38,42 +65,41 @@
             "authors": {"type": "array", "items": GIT_RECEIVE_USER},
         },
         "required": ["agent", "repo", "branch", "rev", "authors"],
     }
 
     def __str__(self):
         """Return a complete human-readable representation of the message."""
-        return "Git branch: {branch} created\nBy: {agent}".format(
+        return "Git branch: {branch} created\nBy: {agent_name}".format(
             branch=self.body["branch"],
-            agent=self.body["agent"],
+            agent_name=self.agent_name,
         )
 
     @property
     def summary(self):
         """Return a summary of the message."""
-        return "{agent} created the branch {branch} on {name}".format(
-            agent=self.body["agent"],
+        return "{agent_name} created the branch {branch} on {name}".format(
+            agent_name=self.agent_name,
             name=self.body["repo"]["fullname"],
             branch=self.body["branch"],
         )
 
     @property
     def url(self):
-        base_url = self.get_base_url()
-        fullname = self.body["repo"]["url_path"]
+        base_url = self.body["repo"]["full_url"]
 
         item = self.body["branch"]
         if "refs/heads/" in item:
             item = item.replace("refs/heads/", "")
 
-        tmpl = "{base_url}/{fullname}/tree/{item}"
-        return tmpl.format(base_url=base_url, fullname=fullname, item=item)
+        tmpl = "{base_url}/tree/{item}"
+        return tmpl.format(base_url=base_url, item=item)
 
 
-class GitBranchDeletionV1(PagureMessage):
+class GitBranchDeletionV1(GitMessage):
     """
     A sub-class of a Fedora message that defines a message schema for messages
     published by pagure when a new thing is created.
     """
 
     topic = "pagure.git.branch.deletion"
 
@@ -90,38 +116,34 @@
             "authors": {"type": "array", "items": GIT_RECEIVE_USER},
         },
         "required": ["agent", "repo", "branch", "rev", "authors"],
     }
 
     def __str__(self):
         """Return a complete human-readable representation of the message."""
-        return "Git branch: {branch} deleted\nBy: {agent}".format(
+        return "Git branch: {branch} deleted\nBy: {agent_name}".format(
             branch=self.body["branch"],
-            agent=self.body["agent"],
+            agent_name=self.agent_name,
         )
 
     @property
     def summary(self):
         """Return a summary of the message."""
-        return "{agent} deleted the branch {branch} on {name}".format(
-            agent=self.body["agent"],
+        return "{agent_name} deleted the branch {branch} on {name}".format(
+            agent_name=self.agent_name,
             name=self.body["repo"]["fullname"],
             branch=self.body["branch"],
         )
 
     @property
     def url(self):
-        base_url = self.get_base_url()
-        fullname = self.body["repo"]["url_path"]
-
-        tmpl = "{base_url}/{fullname}"
-        return tmpl.format(base_url=base_url, fullname=fullname)
+        return self.body["repo"]["full_url"]
 
 
-class GitReceiveV1(PagureMessage):
+class GitReceiveV1(GitMessage):
     """
     A sub-class of a Fedora message that defines a message schema for messages
     published by pagure when a new thing is created.
     """
 
     topic = "pagure.git.receive"
 
@@ -152,43 +174,42 @@
             "start_commit",
             "end_commit",
         ],
     }
 
     def __str__(self):
         """Return a complete human-readable representation of the message."""
-        return "New commit: {count} commits\nBy: {agent}".format(
+        return "New commit: {count} commits\nBy: {agent_name}".format(
             count=self.body["total_commits"],
-            agent=self.body["agent"],
+            agent_name=self.agent_name,
         )
 
     @property
     def summary(self):
         """Return a summary of the message."""
-        return "{agent} pushed {count} commits on {fullname} (branch: {branch})".format(
-            agent=self.body["agent"],
+        return "{agent_name} pushed {count} commits on {fullname} (branch: {branch})".format(
+            agent_name=self.agent_name,
             fullname=self.body["repo"]["fullname"],
             count=self.body["total_commits"],
             branch=self.body["branch"],
         )
 
     @property
     def url(self):
-        base_url = self.get_base_url()
-        fullname = self.body["repo"]["url_path"]
+        base_url = self.body["repo"]["full_url"]
 
         item = self.body["branch"]
         if "refs/heads/" in item:
             item = item.replace("refs/heads/", "")
 
-        tmpl = "{base_url}/{fullname}/tree/{item}"
-        return tmpl.format(base_url=base_url, fullname=fullname, item=item)
+        tmpl = "{base_url}/tree/{item}"
+        return tmpl.format(base_url=base_url, item=item)
 
 
-class GitTagCreationV1(PagureMessage):
+class GitTagCreationV1(GitMessage):
     """
     A sub-class of a Fedora message that defines a message schema for messages
     published by pagure when a new thing is created.
     """
 
     topic = "pagure.git.tag.creation"
 
@@ -205,40 +226,39 @@
             "authors": {"type": "array", "items": GIT_RECEIVE_USER},
         },
         "required": ["agent", "repo", "tag", "rev", "authors"],
     }
 
     def __str__(self):
         """Return a complete human-readable representation of the message."""
-        return "Git tag: {tag} created\nBy: {agent}".format(
+        return "Git tag: {tag} created\nBy: {agent_name}".format(
             tag=self.body["tag"],
-            agent=self.body["agent"],
+            agent_name=self.agent_name,
         )
 
     @property
     def summary(self):
         """Return a summary of the message."""
-        return "{agent} tagged the commit {rev} on {name} as {tag}".format(
-            agent=self.body["agent"],
+        return "{agent_name} tagged the commit {rev} on {name} as {tag}".format(
+            agent_name=self.agent_name,
             name=self.body["repo"]["fullname"],
             tag=self.body["tag"],
             rev=self.body["rev"],
         )
 
     @property
     def url(self):
-        base_url = self.get_base_url()
-        fullname = self.body["repo"]["url_path"]
+        base_url = self.body["repo"]["full_url"]
         tag = self.body["tag"]
 
-        tmpl = "{base_url}/{fullname}/commits/{tag}"
-        return tmpl.format(base_url=base_url, fullname=fullname, tag=tag)
+        tmpl = "{base_url}/commits/{tag}"
+        return tmpl.format(base_url=base_url, tag=tag)
 
 
-class GitTagDeletionV1(PagureMessage):
+class GitTagDeletionV1(GitMessage):
     """
     A sub-class of a Fedora message that defines a message schema for messages
     published by pagure when a new thing is created.
     """
 
     topic = "pagure.git.tag.deletion"
 
@@ -255,29 +275,27 @@
             "authors": {"type": "array", "items": GIT_RECEIVE_USER},
         },
         "required": ["agent", "repo", "tag", "rev", "authors"],
     }
 
     def __str__(self):
         """Return a complete human-readable representation of the message."""
-        return "Git tag: {tag} deleted\nBy: {agent}".format(
+        return "Git tag: {tag} deleted\nBy: {agent_name}".format(
             tag=self.body["tag"],
-            agent=self.body["agent"],
+            agent_name=self.agent_name,
         )
 
     @property
     def summary(self):
         """Return a summary of the message."""
-        return "{agent} deleted the tag {tag} of commit {rev} on {name}".format(
-            agent=self.body["agent"],
+        return "{agent_name} deleted the tag {tag} of commit {rev} on {name}".format(
+            agent_name=self.agent_name,
             name=self.body["repo"]["fullname"],
             tag=self.body["tag"],
             rev=self.body["rev"],
         )
 
     @property
     def url(self):
-        base_url = self.get_base_url()
-        fullname = self.body["repo"]["url_path"]
-
-        tmpl = "{base_url}/{fullname}/releases"
-        return tmpl.format(base_url=base_url, fullname=fullname)
+        base_url = self.body["repo"]["full_url"]
+        tmpl = "{base_url}/releases"
+        return tmpl.format(base_url=base_url)
```

### Comparing `pagure-messages-0.0.6/pagure_messages/issue_schema.py` & `pagure-messages-1.0.0/pagure_messages/issue_schema.py`

 * *Files 14% similar despite different names*

```diff
@@ -36,26 +36,26 @@
             "issue": ISSUE,
         },
         "required": ["agent", "project", "issue"],
     }
 
     def __str__(self):
         """Return a complete human-readable representation of the message."""
-        return "Issue: {fullname}#{id} assigned to {assignee}\nBy: {agent}".format(
+        return "Issue: {fullname}#{id} assigned to {assignee}\nBy: {agent_name}".format(
             fullname=self.body["project"]["fullname"],
             id=self.body["issue"]["id"],
-            agent=self.body["agent"],
+            agent_name=self.agent_name,
             assignee=self.body["issue"]["assignee"]["name"],
         )
 
     @property
     def summary(self):
         """Return a summary of the message."""
-        return "{agent} assigned issue {name}#{id} to {assignee}".format(
-            agent=self.body["agent"],
+        return "{agent_name} assigned issue {name}#{id} to {assignee}".format(
+            agent_name=self.agent_name,
             name=self.body["project"]["fullname"],
             id=self.body["issue"]["id"],
             assignee=self.body["issue"]["assignee"]["name"],
         )
 
     @property
     def url(self):
@@ -81,25 +81,25 @@
             "issue": ISSUE,
         },
         "required": ["agent", "project", "issue"],
     }
 
     def __str__(self):
         """Return a complete human-readable representation of the message."""
-        return "Issue un-assigned: {fullname}#{id}\nBy: {agent}".format(
+        return "Issue un-assigned: {fullname}#{id}\nBy: {agent_name}".format(
             fullname=self.body["project"]["fullname"],
             id=self.body["issue"]["id"],
-            agent=self.body["agent"],
+            agent_name=self.agent_name,
         )
 
     @property
     def summary(self):
         """Return a summary of the message."""
-        return "{agent} reset the assignee on issue {name}#{id}".format(
-            agent=self.body["agent"],
+        return "{agent_name} reset the assignee on issue {name}#{id}".format(
+            agent_name=self.agent_name,
             name=self.body["project"]["fullname"],
             id=self.body["issue"]["id"],
         )
 
     @property
     def url(self):
         return self.body["issue"]["full_url"]
@@ -124,25 +124,25 @@
             "issue": ISSUE,
         },
         "required": ["agent", "project"],
     }
 
     def __str__(self):
         """Return a complete human-readable representation of the message."""
-        return "Issue: {fullname}#{id} has a new comment\nBy: {agent}".format(
+        return "Issue: {fullname}#{id} has a new comment\nBy: {agent_name}".format(
             fullname=self.body["project"]["fullname"],
             id=self.body["issue"]["id"],
-            agent=self.body["agent"],
+            agent_name=self.agent_name,
         )
 
     @property
     def summary(self):
         """Return a summary of the message."""
-        return "{agent} commented on the issue {name}#{id}".format(
-            agent=self.body["agent"],
+        return "{agent_name} commented on the issue {name}#{id}".format(
+            agent_name=self.agent_name,
             name=self.body["project"]["fullname"],
             id=self.body["issue"]["id"],
         )
 
     @property
     def url(self):
         issue_url = self.body["issue"]["full_url"]
@@ -173,26 +173,28 @@
             "added_dependency": {"type": "number"},
         },
         "required": ["agent", "project", "added_dependency"],
     }
 
     def __str__(self):
         """Return a complete human-readable representation of the message."""
-        return "Issue: {fullname}#{id} depends on #{depissueid}\nBy: {agent}".format(
-            fullname=self.body["project"]["fullname"],
-            id=self.body["issue"]["id"],
-            agent=self.body["agent"],
-            depissueid=self.body["added_dependency"],
+        return (
+            "Issue: {fullname}#{id} depends on #{depissueid}\nBy: {agent_name}".format(
+                fullname=self.body["project"]["fullname"],
+                id=self.body["issue"]["id"],
+                agent_name=self.agent_name,
+                depissueid=self.body["added_dependency"],
+            )
         )
 
     @property
     def summary(self):
         """Return a summary of the message."""
-        return "{agent} set the issue {name}#{id} as depending on #{depissueid}".format(
-            agent=self.body["agent"],
+        return "{agent_name} set the issue {name}#{id} as depending on #{depissueid}".format(
+            agent_name=self.agent_name,
             name=self.body["project"]["fullname"],
             id=self.body["issue"]["id"],
             depissueid=self.body["added_dependency"],
         )
 
     @property
     def url(self):
@@ -219,29 +221,39 @@
             "removed_dependency": {"type": "array", "items": {"type": "number"}},
         },
         "required": ["agent", "project", "removed_dependency"],
     }
 
     def __str__(self):
         """Return a complete human-readable representation of the message."""
-        return "Issue: {fullname}#{id} no longer depending on #{depissueid}\nBy: {agent}".format(
-            fullname=self.body["project"]["fullname"],
-            id=self.body["issue"]["id"],
-            agent=self.body["agent"],
-            depissueid=", #".join([str(i) for i in self.body["removed_dependency"]]),
+        return (
+            "Issue: {fullname}#{id} no longer depending"
+            " on #{depissueid}\nBy: {agent_name}".format(
+                fullname=self.body["project"]["fullname"],
+                id=self.body["issue"]["id"],
+                agent_name=self.agent_name,
+                depissueid=", #".join(
+                    [str(i) for i in self.body["removed_dependency"]]
+                ),
+            )
         )
 
     @property
     def summary(self):
         """Return a summary of the message."""
-        return "{agent} removed the dependency on #{depissueid} on the issue {name}#{id}".format(
-            agent=self.body["agent"],
-            name=self.body["project"]["fullname"],
-            id=self.body["issue"]["id"],
-            depissueid=", #".join([str(i) for i in self.body["removed_dependency"]]),
+        return (
+            "{agent_name} removed the dependency"
+            " on #{depissueid} on the issue {name}#{id}".format(
+                agent_name=self.agent_name,
+                name=self.body["project"]["fullname"],
+                id=self.body["issue"]["id"],
+                depissueid=", #".join(
+                    [str(i) for i in self.body["removed_dependency"]]
+                ),
+            )
         )
 
     @property
     def url(self):
         return self.body["issue"]["full_url"]
 
 
@@ -264,25 +276,25 @@
             "issue": ISSUE,
         },
         "required": ["agent", "project", "issue"],
     }
 
     def __str__(self):
         """Return a complete human-readable representation of the message."""
-        return "Issue deleted: {fullname}#{id}\nBy: {agent}".format(
+        return "Issue deleted: {fullname}#{id}\nBy: {agent_name}".format(
             fullname=self.body["project"]["fullname"],
             id=self.body["issue"]["id"],
-            agent=self.body["agent"],
+            agent_name=self.agent_name,
         )
 
     @property
     def summary(self):
         """Return a summary of the message."""
-        return "{agent} deleted issue {name}#{id}: {title}".format(
-            agent=self.body["agent"],
+        return "{agent_name} deleted issue {name}#{id}: {title}".format(
+            agent_name=self.agent_name,
             name=self.body["project"]["fullname"],
             id=self.body["issue"]["id"],
             title=self.body["issue"]["title"],
         )
 
     @property
     def url(self):
@@ -311,29 +323,31 @@
             "fields": {"type": "array", "items": {"type": ["string", "null"]}},
         },
         "required": ["agent", "project", "issue", "fields"],
     }
 
     def __str__(self):
         """Return a complete human-readable representation of the message."""
-        return "Edited Issue: {fullname}#{id}\nBy: {agent}".format(
+        return "Edited Issue: {fullname}#{id}\nBy: {agent_name}".format(
             fullname=self.body["project"]["fullname"],
             id=self.body["issue"]["id"],
-            agent=self.body["agent"],
+            agent_name=self.agent_name,
         )
 
     @property
     def summary(self):
         """Return a summary of the message."""
-        return "{agent} edited fields {fields} of issue {name}#{id}: {title}".format(
-            agent=self.body["agent"],
-            name=self.body["project"]["fullname"],
-            id=self.body["issue"]["id"],
-            title=self.body["issue"]["title"],
-            fields=", ".join(self.body["fields"]),
+        return (
+            "{agent_name} edited fields {fields} of issue {name}#{id}: {title}".format(
+                agent_name=self.agent_name,
+                name=self.body["project"]["fullname"],
+                id=self.body["issue"]["id"],
+                title=self.body["issue"]["title"],
+                fields=", ".join(self.body["fields"]),
+            )
         )
 
     @property
     def url(self):
         return self.body["issue"]["full_url"]
 
 
@@ -356,25 +370,25 @@
             "issue": ISSUE,
         },
         "required": ["agent", "project", "issue"],
     }
 
     def __str__(self):
         """Return a complete human-readable representation of the message."""
-        return "New Issue: {fullname}#{id}\nBy: {agent}".format(
+        return "New Issue: {fullname}#{id}\nBy: {agent_name}".format(
             fullname=self.body["project"]["fullname"],
             id=self.body["issue"]["id"],
-            agent=self.body["agent"],
+            agent_name=self.agent_name,
         )
 
     @property
     def summary(self):
         """Return a summary of the message."""
-        return "{agent} created issue {name}#{id}: {title}".format(
-            agent=self.body["agent"],
+        return "{agent_name} created issue {name}#{id}: {title}".format(
+            agent_name=self.agent_name,
             name=self.body["project"]["fullname"],
             id=self.body["issue"]["id"],
             title=self.body["issue"]["title"],
         )
 
     @property
     def url(self):
@@ -401,26 +415,26 @@
             "tags": {"type": "array", "items": {"type": "string"}},
         },
         "required": ["agent", "project"],
     }
 
     def __str__(self):
         """Return a complete human-readable representation of the message."""
-        return "Issue: {fullname}#{id} tagged with {tags}\nBy: {agent}".format(
+        return "Issue: {fullname}#{id} tagged with {tags}\nBy: {agent_name}".format(
             fullname=self.body["project"]["fullname"],
             id=self.body["issue"]["id"],
-            agent=self.body["agent"],
+            agent_name=self.agent_name,
             tags=", ".join(self.body["tags"]),
         )
 
     @property
     def summary(self):
         """Return a summary of the message."""
-        return "{agent} tagged the issue {name}#{id} with: {tags}".format(
-            agent=self.body["agent"],
+        return "{agent_name} tagged the issue {name}#{id} with: {tags}".format(
+            agent_name=self.agent_name,
             name=self.body["project"]["fullname"],
             id=self.body["issue"]["id"],
             tags=", ".join(self.body["tags"]),
         )
 
     @property
     def url(self):
@@ -447,26 +461,26 @@
             "tags": {"type": "array", "items": {"type": "string"}},
         },
         "required": ["agent", "project"],
     }
 
     def __str__(self):
         """Return a complete human-readable representation of the message."""
-        return "Issue: {fullname}#{id} un-tagged with {tags}\nBy: {agent}".format(
+        return "Issue: {fullname}#{id} un-tagged with {tags}\nBy: {agent_name}".format(
             fullname=self.body["project"]["fullname"],
             id=self.body["issue"]["id"],
-            agent=self.body["agent"],
+            agent_name=self.agent_name,
             tags=", ".join(self.body["tags"]),
         )
 
     @property
     def summary(self):
         """Return a summary of the message."""
-        return "{agent} removed tags {tags} from issue {name}#{id}".format(
-            agent=self.body["agent"],
+        return "{agent_name} removed tags {tags} from issue {name}#{id}".format(
+            agent_name=self.agent_name,
             name=self.body["project"]["fullname"],
             id=self.body["issue"]["id"],
             tags=", ".join(self.body["tags"]),
         )
 
     @property
     def url(self):
```

### Comparing `pagure-messages-0.0.6/pagure_messages/misc_schema.py` & `pagure-messages-1.0.0/pagure_messages/misc_schema.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,16 +36,16 @@
             "flag": COMMIT_FLAG,
         },
         "required": ["agent", "repo", "flag"],
     }
 
     def __str__(self):
         """Return a complete human-readable representation of the message."""
-        return "New commit flag: {username} {status}\nBy: {agent}".format(
-            agent=self.body["agent"],
+        return "New commit flag: {username} {status}\nBy: {agent_name}".format(
+            agent_name=self.agent_name,
             username=self.body["flag"]["username"],
             status=self.body["flag"]["status"],
         )
 
     @property
     def summary(self):
         """Return a summary of the message."""
@@ -88,16 +88,16 @@
             "flag": COMMIT_FLAG,
         },
         "required": ["agent", "repo", "flag"],
     }
 
     def __str__(self):
         """Return a complete human-readable representation of the message."""
-        return "New commit flag: {username} {status}\nBy: {agent}".format(
-            agent=self.body["agent"],
+        return "New commit flag: {username} {status}\nBy: {agent_name}".format(
+            agent_name=self.agent_name,
             username=self.body["flag"]["username"],
             status=self.body["flag"]["status"],
         )
 
     @property
     def summary(self):
         """Return a summary of the message."""
@@ -140,26 +140,28 @@
             "fields": {"type": "array", "items": {"type": "string"}},
         },
         "required": ["agent", "group", "fields"],
     }
 
     def __str__(self):
         """Return a complete human-readable representation of the message."""
-        return "Group edit: {group_name}\nBy: {agent}".format(
-            agent=self.body["agent"],
+        return "Group edit: {group_name}\nBy: {agent_name}".format(
+            agent_name=self.agent_name,
             group_name=self.body["group"]["name"],
         )
 
     @property
     def summary(self):
         """Return a summary of the message."""
-        return "{agent} edited the fields {fields} of the group {group_name}".format(
-            agent=self.body["agent"],
-            group_name=self.body["group"]["name"],
-            fields=", ".join(self.body["fields"]),
+        return (
+            "{agent_name} edited the fields {fields} of the group {group_name}".format(
+                agent_name=self.agent_name,
+                group_name=self.body["group"]["name"],
+                fields=", ".join(self.body["fields"]),
+            )
         )
 
     @property
     def url(self):
         return self.body["group"]["full_url"]
```

### Comparing `pagure-messages-0.0.6/pagure_messages/project_schema.py` & `pagure-messages-1.0.0/pagure_messages/project_schema.py`

 * *Files 18% similar despite different names*

```diff
@@ -26,30 +26,33 @@
     topic = "pagure.project.new"
 
     body_schema = {
         "id": SCHEMA_URL + topic,
         "$schema": "http://json-schema.org/draft-04/schema#",
         "description": "Schema for messages sent when a new project is created",
         "type": "object",
-        "properties": {"agent": {"type": "string"}, "project": PROJECT},
+        "properties": {
+            "agent": {"type": "string"},
+            "project": PROJECT,
+        },
         "required": ["agent", "project"],
     }
 
     def __str__(self):
         """Return a complete human-readable representation of the message."""
-        return "New Project: {fullname}\nBy: {agent}".format(
+        return "New Project: {fullname}\nBy: {agent_name}".format(
             fullname=self.body["project"]["fullname"],
-            agent=self.body["agent"],
+            agent_name=self.agent_name,
         )
 
     @property
     def summary(self):
         """Return a summary of the message."""
-        return '{agent} created project "{name}"'.format(
-            agent=self.body["agent"],
+        return '{agent_name} created project "{name}"'.format(
+            agent_name=self.agent_name,
             name=self.body["project"]["fullname"],
         )
 
     @property
     def url(self):
         return self.body["project"]["full_url"]
 
@@ -73,24 +76,24 @@
             "fields": {"type": "array", "items": {"type": ["string", "null"]}},
         },
         "required": ["agent", "project", "fields"],
     }
 
     def __str__(self):
         """Return a complete human-readable representation of the message."""
-        return "Project Edited: {fullname}\nBy: {agent}".format(
+        return "Project Edited: {fullname}\nBy: {agent_name}".format(
             fullname=self.body["project"]["fullname"],
-            agent=self.body["agent"],
+            agent_name=self.agent_name,
         )
 
     @property
     def summary(self):
         """Return a summary of the message."""
-        return '{agent} edited the fields {fields} of project "{name}"'.format(
-            agent=self.body["agent"],
+        return '{agent_name} edited the fields {fields} of project "{name}"'.format(
+            agent_name=self.agent_name,
             fields=", ".join(self.body["fields"]),
             name=self.body["project"]["fullname"],
         )
 
     @property
     def url(self):
         return self.body["project"]["full_url"]
@@ -105,30 +108,33 @@
     topic = "pagure.project.forked"
 
     body_schema = {
         "id": SCHEMA_URL + topic,
         "$schema": "http://json-schema.org/draft-04/schema#",
         "description": "Schema for messages sent when a new project is created",
         "type": "object",
-        "properties": {"agent": {"type": "string"}, "project": PROJECT},
+        "properties": {
+            "agent": {"type": "string"},
+            "project": PROJECT,
+        },
         "required": ["agent", "project"],
     }
 
     def __str__(self):
         """Return a complete human-readable representation of the message."""
-        return "Project: {fullname}\nForked by: {agent}".format(
+        return "Project: {fullname}\nForked by: {agent_name}".format(
             fullname=self.body["project"]["parent"]["fullname"],
-            agent=self.body["agent"],
+            agent_name=self.agent_name,
         )
 
     @property
     def summary(self):
         """Return a summary of the message."""
-        return '{agent} forked project "{parent}" to {name}'.format(
-            agent=self.body["agent"],
+        return '{agent_name} forked project "{parent}" to {name}'.format(
+            agent_name=self.agent_name,
             parent=self.body["project"]["parent"]["fullname"],
             name=self.body["project"]["fullname"],
         )
 
     @property
     def url(self):
         return self.body["project"]["full_url"]
@@ -143,36 +149,39 @@
     topic = "pagure.project.deleted"
 
     body_schema = {
         "id": SCHEMA_URL + topic,
         "$schema": "http://json-schema.org/draft-04/schema#",
         "description": "Schema for messages sent when a new project is created",
         "type": "object",
-        "properties": {"agent": {"type": "string"}, "project": PROJECT},
+        "properties": {
+            "agent": {"type": "string"},
+            "project": PROJECT,
+        },
         "required": ["agent", "project"],
     }
 
     def __str__(self):
         """Return a complete human-readable representation of the message."""
-        return "Project: {fullname}\nDeleted by: {agent}".format(
+        return "Project: {fullname}\nDeleted by: {agent_name}".format(
             fullname=self.body["project"]["fullname"],
-            agent=self.body["agent"],
+            agent_name=self.agent_name,
         )
 
     @property
     def summary(self):
         """Return a summary of the message."""
-        return '{agent} deleted project "{name}"'.format(
-            agent=self.body["agent"],
+        return '{agent_name} deleted project "{name}"'.format(
+            agent_name=self.agent_name,
             name=self.body["project"]["fullname"],
         )
 
     @property
     def url(self):
-        return self.get_base_url()
+        return self.body["project"]["full_url"]
 
 
 class ProjectGroupAddedV1(PagureMessage):
     """
     A sub-class of a Fedora message that defines a message schema for messages
     published by pagure when a new thing is created.
     """
@@ -180,34 +189,39 @@
     topic = "pagure.project.group.added"
 
     body_schema = {
         "id": SCHEMA_URL + topic,
         "$schema": "http://json-schema.org/draft-04/schema#",
         "description": "Schema for messages sent when a new project is created",
         "type": "object",
-        "properties": {"agent": {"type": "string"}, "project": PROJECT},
+        "properties": {
+            "agent": {"type": "string"},
+            "project": PROJECT,
+        },
         "required": ["agent", "project"],
     }
 
     def __str__(self):
         """Return a complete human-readable representation of the message."""
-        return "Group: {group} added to {fullname} as {access}\nBy: {agent}".format(
-            fullname=self.body["project"]["fullname"],
-            group=self.body["new_group"],
-            access=self.body["access"],
-            agent=self.body["agent"],
+        return (
+            "Group: {group} added to {fullname} as {access}\nBy: {agent_name}".format(
+                fullname=self.body["project"]["fullname"],
+                group=self.body["new_group"],
+                access=self.body["access"],
+                agent_name=self.agent_name,
+            )
         )
 
     @property
     def summary(self):
         """Return a summary of the message."""
         return (
-            '{agent} added the group {group} to the project "{name}" at '
+            '{agent_name} added the group {group} to the project "{name}" at '
             "the {access} level".format(
-                agent=self.body["agent"],
+                agent_name=self.agent_name,
                 group=self.body["new_group"],
                 access=self.body["access"],
                 name=self.body["project"]["fullname"],
             )
         )
 
     @property
@@ -234,28 +248,30 @@
             "removed_groups": {"type": "array", "items": {"type": "string"}},
         },
         "required": ["agent", "project"],
     }
 
     def __str__(self):
         """Return a complete human-readable representation of the message."""
-        return "Group: {group} removed from {fullname}({access})\nBy: {agent}".format(
-            fullname=self.body["project"]["fullname"],
-            group=self.body["new_group"],
-            access=self.body["access"],
-            agent=self.body["agent"],
+        return (
+            "Group: {group} removed from {fullname}({access})\nBy: {agent_name}".format(
+                fullname=self.body["project"]["fullname"],
+                group=self.body["new_group"],
+                access=self.body["access"],
+                agent_name=self.agent_name,
+            )
         )
 
     @property
     def summary(self):
         """Return a summary of the message."""
         return (
-            "{agent} removed the group {group} (with {access} level)  from the "
+            "{agent_name} removed the group {group} (with {access} level)  from the "
             'project "{name}"'.format(
-                agent=self.body["agent"],
+                agent_name=self.agent_name,
                 group=self.body["new_group"],
                 access=self.body["access"],
                 name=self.body["project"]["fullname"],
             )
         )
 
     @property
@@ -272,34 +288,37 @@
     topic = "pagure.project.group.access.updated"
 
     body_schema = {
         "id": SCHEMA_URL + topic,
         "$schema": "http://json-schema.org/draft-04/schema#",
         "description": "Schema for messages sent when a new project is created",
         "type": "object",
-        "properties": {"agent": {"type": "string"}, "project": PROJECT},
+        "properties": {
+            "agent": {"type": "string"},
+            "project": PROJECT,
+        },
         "required": ["agent", "project"],
     }
 
     def __str__(self):
         """Return a complete human-readable representation of the message."""
-        return "Group: {group} access updated to {access} on {fullname}\nBy: {agent}".format(
+        return "Group: {group} access updated to {access} on {fullname}\nBy: {agent_name}".format(
             fullname=self.body["project"]["fullname"],
             group=self.body["new_group"],
             access=self.body["new_access"],
-            agent=self.body["agent"],
+            agent_name=self.agent_name,
         )
 
     @property
     def summary(self):
         """Return a summary of the message."""
         return (
-            "{agent} updated the access of group {group} to {access} on "
+            "{agent_name} updated the access of group {group} to {access} on "
             'the project "{name}"'.format(
-                agent=self.body["agent"],
+                agent_name=self.agent_name,
                 group=self.body["new_group"],
                 access=self.body["new_access"],
                 name=self.body["project"]["fullname"],
             )
         )
 
     @property
@@ -316,31 +335,34 @@
     topic = "pagure.project.tag.edited"
 
     body_schema = {
         "id": SCHEMA_URL + topic,
         "$schema": "http://json-schema.org/draft-04/schema#",
         "description": "Schema for messages sent when a new project is created",
         "type": "object",
-        "properties": {"agent": {"type": "string"}, "project": PROJECT},
+        "properties": {
+            "agent": {"type": "string"},
+            "project": PROJECT,
+        },
         "required": ["agent", "project"],
     }
 
     def __str__(self):
         """Return a complete human-readable representation of the message."""
-        return "Tag: {tag_name} edited on {fullname}\nBy: {agent}".format(
+        return "Tag: {tag_name} edited on {fullname}\nBy: {agent_name}".format(
             fullname=self.body["project"]["fullname"],
             tag_name=self.body["new_tag"],
-            agent=self.body["agent"],
+            agent_name=self.agent_name,
         )
 
     @property
     def summary(self):
         """Return a summary of the message."""
-        return '{agent} edited the tag {tag_name} on the project "{name}"'.format(
-            agent=self.body["agent"],
+        return '{agent_name} edited the tag {tag_name} on the project "{name}"'.format(
+            agent_name=self.agent_name,
             tag_name=self.body["new_tag"],
             name=self.body["project"]["fullname"],
         )
 
     @property
     def url(self):
         return self.body["project"]["full_url"]
@@ -355,31 +377,34 @@
     topic = "pagure.project.tag.removed"
 
     body_schema = {
         "id": SCHEMA_URL + topic,
         "$schema": "http://json-schema.org/draft-04/schema#",
         "description": "Schema for messages sent when a new project is created",
         "type": "object",
-        "properties": {"agent": {"type": "string"}, "project": PROJECT},
+        "properties": {
+            "agent": {"type": "string"},
+            "project": PROJECT,
+        },
         "required": ["agent", "project"],
     }
 
     def __str__(self):
         """Return a complete human-readable representation of the message."""
-        return "Tag(s): {tags} removed from {fullname}\nBy: {agent}".format(
+        return "Tag(s): {tags} removed from {fullname}\nBy: {agent_name}".format(
             fullname=self.body["project"]["fullname"],
             tags=", ".join(self.body["tags"]),
-            agent=self.body["agent"],
+            agent_name=self.agent_name,
         )
 
     @property
     def summary(self):
         """Return a summary of the message."""
-        return '{agent} removed the tag(s) {tags} of project "{name}"'.format(
-            agent=self.body["agent"],
+        return '{agent_name} removed the tag(s) {tags} of project "{name}"'.format(
+            agent_name=self.agent_name,
             tags=", ".join(self.body["tags"]),
             name=self.body["project"]["fullname"],
         )
 
     @property
     def url(self):
         return self.body["project"]["full_url"]
@@ -394,34 +419,37 @@
     topic = "pagure.project.user.access.updated"
 
     body_schema = {
         "id": SCHEMA_URL + topic,
         "$schema": "http://json-schema.org/draft-04/schema#",
         "description": "Schema for messages sent when a new project is created",
         "type": "object",
-        "properties": {"agent": {"type": "string"}, "project": PROJECT},
+        "properties": {
+            "agent": {"type": "string"},
+            "project": PROJECT,
+        },
         "required": ["agent", "project"],
     }
 
     def __str__(self):
         """Return a complete human-readable representation of the message."""
-        return "User: {user} access edited to {new_access} on {fullname}\nBy: {agent}".format(
+        return "User: {user} access edited to {new_access} on {fullname}\nBy: {agent_name}".format(
             fullname=self.body["project"]["fullname"],
             user=self.body["new_user"],
             new_access=self.body["new_access"],
-            agent=self.body["agent"],
+            agent_name=self.agent_name,
         )
 
     @property
     def summary(self):
         """Return a summary of the message."""
         return (
-            "{agent} updated the access of {user} to {new_access} on the "
+            "{agent_name} updated the access of {user} to {new_access} on the "
             'project "{name}"'.format(
-                agent=self.body["agent"],
+                agent_name=self.agent_name,
                 user=self.body["new_user"],
                 new_access=self.body["new_access"],
                 name=self.body["project"]["fullname"],
             )
         )
 
     @property
@@ -438,31 +466,34 @@
     topic = "pagure.project.user.added"
 
     body_schema = {
         "id": SCHEMA_URL + topic,
         "$schema": "http://json-schema.org/draft-04/schema#",
         "description": "Schema for messages sent when a new project is created",
         "type": "object",
-        "properties": {"agent": {"type": "string"}, "project": PROJECT},
+        "properties": {
+            "agent": {"type": "string"},
+            "project": PROJECT,
+        },
         "required": ["agent", "project"],
     }
 
     def __str__(self):
         """Return a complete human-readable representation of the message."""
-        return "User: {user} added to {fullname}\nBy: {agent}".format(
+        return "User: {user} added to {fullname}\nBy: {agent_name}".format(
             fullname=self.body["project"]["fullname"],
             user=self.body["new_user"],
-            agent=self.body["agent"],
+            agent_name=self.agent_name,
         )
 
     @property
     def summary(self):
         """Return a summary of the message."""
-        return '{agent} added the {user} to the project "{name}"'.format(
-            agent=self.body["agent"],
+        return '{agent_name} added the {user} to the project "{name}"'.format(
+            agent_name=self.agent_name,
             user=self.body["new_user"],
             name=self.body["project"]["fullname"],
         )
 
     @property
     def url(self):
         return self.body["project"]["full_url"]
@@ -477,31 +508,34 @@
     topic = "pagure.project.user.removed"
 
     body_schema = {
         "id": SCHEMA_URL + topic,
         "$schema": "http://json-schema.org/draft-04/schema#",
         "description": "Schema for messages sent when a new project is created",
         "type": "object",
-        "properties": {"agent": {"type": "string"}, "project": PROJECT},
+        "properties": {
+            "agent": {"type": "string"},
+            "project": PROJECT,
+        },
         "required": ["agent", "project"],
     }
 
     def __str__(self):
         """Return a complete human-readable representation of the message."""
-        return "User: {user} removed from {fullname}\nBy: {agent}".format(
+        return "User: {user} removed from {fullname}\nBy: {agent_name}".format(
             fullname=self.body["project"]["fullname"],
             user=self.body["removed_user"],
-            agent=self.body["agent"],
+            agent_name=self.agent_name,
         )
 
     @property
     def summary(self):
         """Return a summary of the message."""
-        return '{agent} removed the {user} from the project "{name}"'.format(
-            agent=self.body["agent"],
+        return '{agent_name} removed the {user} from the project "{name}"'.format(
+            agent_name=self.agent_name,
             user=self.body["removed_user"],
             name=self.body["project"]["fullname"],
         )
 
     @property
     def url(self):
         return self.body["project"]["full_url"]
```

### Comparing `pagure-messages-0.0.6/pagure_messages/pull_requests_schema.py` & `pagure-messages-1.0.0/pagure_messages/pull_requests_schema.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,27 +36,27 @@
             "project": PROJECT,
         },
         "required": ["agent", "pullrequest", "project"],
     }
 
     def __str__(self):
         """Return a complete human-readable representation of the message."""
-        return "Pull-request {name}#{id} was assigned\nBy: {agent}".format(
-            agent=self.body["agent"],
+        return "Pull-request {name}#{id} was assigned\nBy: {agent_name}".format(
+            agent_name=self.agent_name,
             name=self.body["pullrequest"]["project"]["fullname"],
             id=self.body["pullrequest"]["id"],
         )
 
     @property
     def summary(self):
         """Return a summary of the message."""
         return "{username} assigned the pull-request {name}#{id} to {assignee}".format(
             name=self.body["pullrequest"]["project"]["fullname"],
             id=self.body["pullrequest"]["id"],
-            username=self.body["agent"],
+            username=self.agent_name,
             assignee=self.body["pullrequest"]["assignee"]["name"],
         )
 
     @property
     def url(self):
         return self.body["pullrequest"]["full_url"]
 
@@ -80,27 +80,27 @@
             "project": PROJECT,
         },
         "required": ["agent", "pullrequest", "project"],
     }
 
     def __str__(self):
         """Return a complete human-readable representation of the message."""
-        return "Pull-request {name}#{id} was un-assigned\nBy: {agent}".format(
-            agent=self.body["agent"],
+        return "Pull-request {name}#{id} was un-assigned\nBy: {agent_name}".format(
+            agent_name=self.agent_name,
             name=self.body["pullrequest"]["project"]["fullname"],
             id=self.body["pullrequest"]["id"],
         )
 
     @property
     def summary(self):
         """Return a summary of the message."""
         return "{username} reset the assignee of the pull-request {name}#{id}".format(
             name=self.body["pullrequest"]["project"]["fullname"],
             id=self.body["pullrequest"]["id"],
-            username=self.body["agent"],
+            username=self.agent_name,
         )
 
     @property
     def url(self):
         return self.body["pullrequest"]["full_url"]
 
 
@@ -123,26 +123,28 @@
             "merged": {"type": "boolean"},
         },
         "required": ["agent", "pullrequest", "merged"],
     }
 
     def __str__(self):
         """Return a complete human-readable representation of the message."""
-        return "Pull-Request: {fullname}#{id} has been {action}\nBy: {agent}".format(
-            fullname=self.body["pullrequest"]["project"]["fullname"],
-            id=self.body["pullrequest"]["id"],
-            agent=self.body["agent"],
-            action="merged" if self.body["merged"] else "closed without merging",
+        return (
+            "Pull-Request: {fullname}#{id} has been {action}\nBy: {agent_name}".format(
+                fullname=self.body["pullrequest"]["project"]["fullname"],
+                id=self.body["pullrequest"]["id"],
+                agent_name=self.agent_name,
+                action="merged" if self.body["merged"] else "closed without merging",
+            )
         )
 
     @property
     def summary(self):
         """Return a summary of the message."""
-        return "{agent} {action} the pull-request {name}#{id}".format(
-            agent=self.body["agent"],
+        return "{agent_name} {action} the pull-request {name}#{id}".format(
+            agent_name=self.agent_name,
             name=self.body["pullrequest"]["project"]["fullname"],
             id=self.body["pullrequest"]["id"],
             action="merged" if self.body["merged"] else "closed without merging",
         )
 
     @property
     def url(self):
@@ -167,25 +169,27 @@
             "pullrequest": PULL_REQUEST,
         },
         "required": ["agent", "pullrequest"],
     }
 
     def __str__(self):
         """Return a complete human-readable representation of the message."""
-        return "Pull-Request: {fullname}#{id} has a new comment\nBy: {agent}".format(
-            fullname=self.body["pullrequest"]["project"]["fullname"],
-            id=self.body["pullrequest"]["id"],
-            agent=self.body["agent"],
+        return (
+            "Pull-Request: {fullname}#{id} has a new comment\nBy: {agent_name}".format(
+                fullname=self.body["pullrequest"]["project"]["fullname"],
+                id=self.body["pullrequest"]["id"],
+                agent_name=self.agent_name,
+            )
         )
 
     @property
     def summary(self):
         """Return a summary of the message."""
-        return "{agent} commented on the pull-request {name}#{id}".format(
-            agent=self.body["agent"],
+        return "{agent_name} commented on the pull-request {name}#{id}".format(
+            agent_name=self.agent_name,
             name=self.body["pullrequest"]["project"]["fullname"],
             id=self.body["pullrequest"]["id"],
         )
 
     @property
     def url(self):
         full_url = self.body["pullrequest"]["full_url"]
@@ -214,25 +218,27 @@
             "pullrequest": PULL_REQUEST,
         },
         "required": ["agent", "pullrequest"],
     }
 
     def __str__(self):
         """Return a complete human-readable representation of the message."""
-        return "Edited comment on Pull-Request: {fullname}#{id}\nBy: {agent}".format(
-            fullname=self.body["pullrequest"]["project"]["fullname"],
-            id=self.body["pullrequest"]["id"],
-            agent=self.body["agent"],
+        return (
+            "Edited comment on Pull-Request: {fullname}#{id}\nBy: {agent_name}".format(
+                fullname=self.body["pullrequest"]["project"]["fullname"],
+                id=self.body["pullrequest"]["id"],
+                agent_name=self.agent_name,
+            )
         )
 
     @property
     def summary(self):
         """Return a summary of the message."""
-        return "{agent} edited comment on the pull-request {name}#{id}".format(
-            agent=self.body["agent"],
+        return "{agent_name} edited comment on the pull-request {name}#{id}".format(
+            agent_name=self.agent_name,
             name=self.body["pullrequest"]["project"]["fullname"],
             id=self.body["pullrequest"]["id"],
         )
 
     @property
     def url(self):
         full_url = self.body["pullrequest"]["full_url"]
@@ -262,16 +268,16 @@
             "flag": COMMIT_FLAG,
         },
         "required": ["agent", "pullrequest", "flag"],
     }
 
     def __str__(self):
         """Return a complete human-readable representation of the message."""
-        return "New pull-request flag: {username} {status}\nBy: {agent}".format(
-            agent=self.body["agent"],
+        return "New pull-request flag: {username} {status}\nBy: {agent_name}".format(
+            agent_name=self.agent_name,
             username=self.body["flag"]["username"],
             status=self.body["flag"]["status"],
         )
 
     @property
     def summary(self):
         """Return a summary of the message."""
@@ -306,18 +312,20 @@
             "flag": COMMIT_FLAG,
         },
         "required": ["agent", "pullrequest", "flag"],
     }
 
     def __str__(self):
         """Return a complete human-readable representation of the message."""
-        return "Pull-request flag updated: {username} {status}\nBy: {agent}".format(
-            agent=self.body["agent"],
-            username=self.body["flag"]["username"],
-            status=self.body["flag"]["status"],
+        return (
+            "Pull-request flag updated: {username} {status}\nBy: {agent_name}".format(
+                agent_name=self.agent_name,
+                username=self.body["flag"]["username"],
+                status=self.body["flag"]["status"],
+            )
         )
 
     @property
     def summary(self):
         """Return a summary of the message."""
         return "{username} updated flag on pull-request {name}#{id} to {status}".format(
             name=self.body["pullrequest"]["project"]["fullname"],
@@ -350,27 +358,29 @@
             "pullrequest": PULL_REQUEST,
         },
         "required": ["agent", "pullrequest", "project"],
     }
 
     def __str__(self):
         """Return a complete human-readable representation of the message."""
-        return "Description of pull-request {name}#{id} edited\nBy: {agent}".format(
-            agent=self.body["agent"],
-            name=self.body["pullrequest"]["project"]["fullname"],
-            id=self.body["pullrequest"]["id"],
+        return (
+            "Description of pull-request {name}#{id} edited\nBy: {agent_name}".format(
+                agent_name=self.agent_name,
+                name=self.body["pullrequest"]["project"]["fullname"],
+                id=self.body["pullrequest"]["id"],
+            )
         )
 
     @property
     def summary(self):
         """Return a summary of the message."""
         return "{username} has edited the description of the pull-request {name}#{id}".format(
             name=self.body["pullrequest"]["project"]["fullname"],
             id=self.body["pullrequest"]["id"],
-            username=self.body["agent"],
+            username=self.agent_name,
         )
 
     @property
     def url(self):
         return self.body["pullrequest"]["full_url"]
 
 
@@ -392,25 +402,25 @@
             "pullrequest": PULL_REQUEST,
         },
         "required": ["agent", "pullrequest"],
     }
 
     def __str__(self):
         """Return a complete human-readable representation of the message."""
-        return "New Pull-Request: {fullname}#{id}\nBy: {agent}".format(
+        return "New Pull-Request: {fullname}#{id}\nBy: {agent_name}".format(
             fullname=self.body["pullrequest"]["project"]["fullname"],
             id=self.body["pullrequest"]["id"],
-            agent=self.body["agent"],
+            agent_name=self.agent_name,
         )
 
     @property
     def summary(self):
         """Return a summary of the message."""
-        return "{agent} opened a pull-request {fullname}#{id}: {title}".format(
-            agent=self.body["agent"],
+        return "{agent_name} opened a pull-request {fullname}#{id}: {title}".format(
+            agent_name=self.agent_name,
             fullname=self.body["pullrequest"]["project"]["fullname"],
             id=self.body["pullrequest"]["id"],
             title=self.body["pullrequest"]["title"],
         )
 
     @property
     def url(self):
@@ -435,27 +445,27 @@
             "pullrequest": PULL_REQUEST,
         },
         "required": ["agent", "pullrequest"],
     }
 
     def __str__(self):
         """Return a complete human-readable representation of the message."""
-        return "Pull-request {name}#{id} was rebased\nBy: {agent}".format(
-            agent=self.body["agent"],
+        return "Pull-request {name}#{id} was rebased\nBy: {agent_name}".format(
+            agent_name=self.agent_name,
             name=self.body["pullrequest"]["project"]["fullname"],
             id=self.body["pullrequest"]["id"],
         )
 
     @property
     def summary(self):
         """Return a summary of the message."""
         return "{username} rebased the pull-request {name}#{id}".format(
             name=self.body["pullrequest"]["project"]["fullname"],
             id=self.body["pullrequest"]["id"],
-            username=self.body["agent"],
+            username=self.agent_name,
         )
 
     @property
     def url(self):
         return self.body["pullrequest"]["full_url"]
 
 
@@ -477,27 +487,27 @@
             "pullrequest": PULL_REQUEST,
         },
         "required": ["agent", "pullrequest"],
     }
 
     def __str__(self):
         """Return a complete human-readable representation of the message."""
-        return "Pull-request {name}#{id} was re-opened\nBy: {agent}".format(
-            agent=self.body["agent"],
+        return "Pull-request {name}#{id} was re-opened\nBy: {agent_name}".format(
+            agent_name=self.agent_name,
             name=self.body["pullrequest"]["project"]["fullname"],
             id=self.body["pullrequest"]["id"],
         )
 
     @property
     def summary(self):
         """Return a summary of the message."""
         return "{username} re-opened the pull-request {name}#{id}".format(
             name=self.body["pullrequest"]["project"]["fullname"],
             id=self.body["pullrequest"]["id"],
-            username=self.body["agent"],
+            username=self.agent_name,
         )
 
     @property
     def url(self):
         return self.body["pullrequest"]["full_url"]
 
 
@@ -521,27 +531,27 @@
             "tags": {"type": "array", "items": {"type": "string"}},
         },
         "required": ["agent", "pullrequest", "project", "tags"],
     }
 
     def __str__(self):
         """Return a complete human-readable representation of the message."""
-        return "Pull-request {name}#{id} was tagged\nBy: {agent}".format(
-            agent=self.body["agent"],
+        return "Pull-request {name}#{id} was tagged\nBy: {agent_name}".format(
+            agent_name=self.agent_name,
             name=self.body["pullrequest"]["project"]["fullname"],
             id=self.body["pullrequest"]["id"],
         )
 
     @property
     def summary(self):
         """Return a summary of the message."""
         return "{username} tagged the pull-request {name}#{id} with {tags}".format(
             name=self.body["pullrequest"]["project"]["fullname"],
             id=self.body["pullrequest"]["id"],
-            username=self.body["agent"],
+            username=self.agent_name,
             tags=", ".join(self.body["tags"]),
         )
 
     @property
     def url(self):
         return self.body["pullrequest"]["full_url"]
 
@@ -566,27 +576,27 @@
             "tags": {"type": "array", "items": {"type": "string"}},
         },
         "required": ["agent", "pullrequest", "project", "tags"],
     }
 
     def __str__(self):
         """Return a complete human-readable representation of the message."""
-        return "Pull-request {name}#{id} was un-tagged\nBy: {agent}".format(
-            agent=self.body["agent"],
+        return "Pull-request {name}#{id} was un-tagged\nBy: {agent_name}".format(
+            agent_name=self.agent_name,
             name=self.body["pullrequest"]["project"]["fullname"],
             id=self.body["pullrequest"]["id"],
         )
 
     @property
     def summary(self):
         """Return a summary of the message."""
         return "{username} un-tagged the pull-request {name}#{id} with: {tags}".format(
             name=self.body["pullrequest"]["project"]["fullname"],
             id=self.body["pullrequest"]["id"],
-            username=self.body["agent"],
+            username=self.agent_name,
             tags=", ".join(self.body["tags"]),
         )
 
     @property
     def url(self):
         return self.body["pullrequest"]["full_url"]
 
@@ -609,25 +619,25 @@
             "pullrequest": PULL_REQUEST,
         },
         "required": ["agent", "pullrequest"],
     }
 
     def __str__(self):
         """Return a complete human-readable representation of the message."""
-        return "Pull-request {name}#{id} was updated\nBy: {agent}".format(
-            agent=self.body["agent"],
+        return "Pull-request {name}#{id} was updated\nBy: {agent_name}".format(
+            agent_name=self.agent_name,
             name=self.body["pullrequest"]["project"]["fullname"],
             id=self.body["pullrequest"]["id"],
         )
 
     @property
     def summary(self):
         """Return a summary of the message."""
         return "{username} updated the pull-request {name}#{id}".format(
             name=self.body["pullrequest"]["project"]["fullname"],
             id=self.body["pullrequest"]["id"],
-            username=self.body["agent"],
+            username=self.agent_name,
         )
 
     @property
     def url(self):
         return self.body["pullrequest"]["full_url"]
```

### Comparing `pagure-messages-0.0.6/pagure_messages/tests/test_commit_flag_added.py` & `pagure-messages-1.0.0/pagure_messages/tests/test_commit_flag_added.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-0.0.6/pagure_messages/tests/test_commit_flag_updated.py` & `pagure-messages-1.0.0/pagure_messages/tests/test_commit_flag_updated.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-0.0.6/pagure_messages/tests/test_common.py` & `pagure-messages-1.0.0/pagure_messages/tests/test_common.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,29 +11,37 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 
 """Unit tests for common properties of the message schemas."""
+import pytest
 
 from .utils import PROJECT
 from ..project_schema import ProjectNewV1
 
 
 def test_properties():
     """Assert some properties are correct."""
     body = {
         "agent": "dummy-user",
         "project": PROJECT,
     }
     message = ProjectNewV1(body=body)
 
-    assert message.app_name == "pagure"
+    assert message.app_name == "Pagure"
     assert message.app_icon == "https://apps.fedoraproject.org/img/icons/pagure.png"
-    assert message.agent == "dummy-user"
+    assert message.agent_name == "dummy-user"
     assert message.agent_avatar == (
         "https://seccdn.libravatar.org/avatar/"
         "18e8268125372e35f95ef082fd124e9274d46916efe2277417fa5fecfee31af1"
         "?s=64&d=retro"
     )
     assert message.usernames == ["dummy-user"]
+    with pytest.warns(DeprecationWarning) as w:
+        assert message.agent == "dummy-user"
+        assert len(w) == 1
+        assert (
+            w[0].message.args[0]
+            == "agent property is deprecated, please use agent_name instead"
+        )
```

### Comparing `pagure-messages-0.0.6/pagure_messages/tests/test_git_branch_creation.py` & `pagure-messages-1.0.0/pagure_messages/tests/test_git_branch_creation.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
                 "email": None,
             }
         ],
     }
     message = GitBranchCreationV1(body=body)
     message.validate()
     assert (
-        message.url == "https://pagure.io/fedora-infra/fedocal-messages/"
+        message.url == "http://localhost.localdomain/fedora-infra/fedocal-messages/"
         "tree/feature/awesome"
     )
 
 
 def test_minimal_short_branch():
     """
     Assert the message schema validates a message with the required fields.
@@ -67,15 +67,15 @@
                 "email": None,
             }
         ],
     }
     message = GitBranchCreationV1(body=body)
     message.validate()
     assert (
-        message.url == "https://pagure.io/fedora-infra/fedocal-messages/"
+        message.url == "http://localhost.localdomain/fedora-infra/fedocal-messages/"
         "tree/feature/awesome"
     )
 
 
 def test_missing_fields():
     """Assert an exception is actually raised on validation failure."""
     minimal_message = {
```

### Comparing `pagure-messages-0.0.6/pagure_messages/tests/test_git_branch_deletion.py` & `pagure-messages-1.0.0/pagure_messages/tests/test_git_branch_deletion.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
                 "name": "dummy-user",
                 "email": None,
             }
         ],
     }
     message = GitBranchDeletionV1(body=body)
     message.validate()
-    assert message.url == "https://pagure.io/fedora-infra/fedocal-messages"
+    assert message.url == "http://localhost.localdomain/fedora-infra/fedocal-messages"
 
 
 def test_missing_fields():
     """Assert an exception is actually raised on validation failure."""
     minimal_message = {
         "repo": PROJECT,
         "branch": "feature/awesome",
```

### Comparing `pagure-messages-0.0.6/pagure_messages/tests/test_git_receive.py` & `pagure-messages-1.0.0/pagure_messages/tests/test_git_receive.py`

 * *Files 13% similar despite different names*

```diff
@@ -44,15 +44,22 @@
         ],
         "total_commits": 42,
         "start_commit": "hash_commit_start",
         "end_commit": "hash_commit_stop",
     }
     message = GitReceiveV1(body=body)
     message.validate()
-    assert message.url == "https://pagure.io/fedora-infra/fedocal-messages/tree/develop"
+    assert (
+        message.url
+        == "http://localhost.localdomain/fedora-infra/fedocal-messages/tree/develop"
+    )
+    assert message.packages == []
+    assert message.containers == []
+    assert message.modules == []
+    assert message.flatpaks == []
 
 
 def test_minimal_short_branch():
     """
     Assert the message schema validates a message with the required fields.
     """
     body = {
@@ -71,15 +78,18 @@
         ],
         "total_commits": 42,
         "start_commit": "hash_commit_start",
         "end_commit": "hash_commit_stop",
     }
     message = GitReceiveV1(body=body)
     message.validate()
-    assert message.url == "https://pagure.io/fedora-infra/fedocal-messages/tree/develop"
+    assert (
+        message.url
+        == "http://localhost.localdomain/fedora-infra/fedocal-messages/tree/develop"
+    )
 
 
 def test_missing_fields():
     """Assert an exception is actually raised on validation failure."""
     minimal_message = {
         "forced": False,
         "repo": PROJECT,
@@ -151,7 +161,46 @@
     expected_summary = (
         "dummy-user pushed 42 commits on "
         "fedora-infra/fedocal-messages (branch: develop)"
     )
     message = GitReceiveV1(body=body)
     message.validate()
     assert expected_summary == message.summary
+
+
+@pytest.mark.parametrize(
+    "namespace,msg_attr",
+    [
+        ("rpms", "packages"),
+        ("containers", "containers"),
+        ("modules", "modules"),
+        ("flatpaks", "flatpaks"),
+    ],
+)
+def test_artifacts(namespace, msg_attr):
+    """
+    Assert the message has the correct artifacts set
+    """
+    body = {
+        "agent": "dummy-user",
+        "forced": False,
+        "repo": PROJECT.copy(),
+        "old_commit": "hash_commit_old",
+        "branch": "refs/heads/develop",
+        "authors": [
+            {
+                "fullname": "dummy-user",
+                "url_path": "user/dummy-user",
+                "name": "dummy-user",
+                "email": None,
+            }
+        ],
+        "total_commits": 42,
+        "start_commit": "hash_commit_start",
+        "end_commit": "hash_commit_stop",
+    }
+    body["repo"]["namespace"] = namespace
+    message = GitReceiveV1(body=body)
+
+    for test_attr in ("packages", "containers", "modules", "flatpaks"):
+        expected = ["fedocal-messages"] if msg_attr == test_attr else []
+        assert getattr(message, test_attr) == expected
```

### Comparing `pagure-messages-0.0.6/pagure_messages/tests/test_git_tag_creation.py` & `pagure-messages-1.0.0/pagure_messages/tests/test_git_tag_deletion.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 """Unit tests for the message schema."""
 
 from jsonschema import ValidationError
 
 import pytest
 
 from .utils import PROJECT
-from ..git_schema import GitTagCreationV1
+from ..git_schema import GitTagDeletionV1
 
 
 def test_minimal():
     """
     Assert the message schema validates a message with the required fields.
     """
     body = {
@@ -38,18 +38,19 @@
                 "fullname": "dummy-user",
                 "url_path": "user/dummy-user",
                 "name": "dummy-user",
                 "email": None,
             }
         ],
     }
-    message = GitTagCreationV1(body=body)
+    message = GitTagDeletionV1(body=body)
     message.validate()
     assert (
-        message.url == "https://pagure.io/fedora-infra/fedocal-messages/commits/0.0.1"
+        message.url
+        == "http://localhost.localdomain/fedora-infra/fedocal-messages/releases"
     )
 
 
 def test_missing_fields():
     """Assert an exception is actually raised on validation failure."""
     minimal_message = {
         "repo": PROJECT,
@@ -60,15 +61,15 @@
                 "fullname": "dummy-user",
                 "url_path": "user/dummy-user",
                 "name": "dummy-user",
                 "email": None,
             }
         ],
     }
-    message = GitTagCreationV1(body=minimal_message)
+    message = GitTagDeletionV1(body=minimal_message)
     with pytest.raises(ValidationError):
         message.validate()
 
 
 def test_str():
     """Assert __str__ produces a human-readable message."""
     body = {
@@ -81,16 +82,16 @@
                 "fullname": "dummy-user",
                 "url_path": "user/dummy-user",
                 "name": "dummy-user",
                 "email": None,
             }
         ],
     }
-    expected_str = "Git tag: 0.0.1 created\nBy: dummy-user"
-    message = GitTagCreationV1(body=body)
+    expected_str = "Git tag: 0.0.1 deleted\nBy: dummy-user"
+    message = GitTagDeletionV1(body=body)
     message.validate()
     assert expected_str == str(message)
 
 
 def test_summary():
     """Assert the summary is correct."""
     body = {
@@ -104,13 +105,13 @@
                 "url_path": "user/dummy-user",
                 "name": "dummy-user",
                 "email": None,
             }
         ],
     }
     expected_summary = (
-        "dummy-user tagged the commit hash_commit on "
-        "fedora-infra/fedocal-messages as 0.0.1"
+        "dummy-user deleted the tag 0.0.1 of commit hash_commit on "
+        "fedora-infra/fedocal-messages"
     )
-    message = GitTagCreationV1(body=body)
+    message = GitTagDeletionV1(body=body)
     message.validate()
     assert expected_summary == message.summary
```

### Comparing `pagure-messages-0.0.6/pagure_messages/tests/test_git_tag_deletion.py` & `pagure-messages-1.0.0/pagure_messages/tests/test_project_user_access_updated.py`

 * *Files 19% similar despite different names*

```diff
@@ -17,98 +17,65 @@
 """Unit tests for the message schema."""
 
 from jsonschema import ValidationError
 
 import pytest
 
 from .utils import PROJECT
-from ..git_schema import GitTagDeletionV1
+from ..project_schema import ProjectUserAccessUpdatedV1
 
 
 def test_minimal():
     """
     Assert the message schema validates a message with the required fields.
     """
     body = {
         "agent": "dummy-user",
-        "repo": PROJECT,
-        "tag": "0.0.1",
-        "rev": "hash_commit",
-        "authors": [
-            {
-                "fullname": "dummy-user",
-                "url_path": "user/dummy-user",
-                "name": "dummy-user",
-                "email": None,
-            }
-        ],
+        "project": PROJECT,
     }
-    message = GitTagDeletionV1(body=body)
+    message = ProjectUserAccessUpdatedV1(body=body)
     message.validate()
-    assert message.url == "https://pagure.io/fedora-infra/fedocal-messages/releases"
+    assert message.url == "http://localhost.localdomain/fedora-infra/fedocal-messages"
 
 
 def test_missing_fields():
     """Assert an exception is actually raised on validation failure."""
     minimal_message = {
-        "repo": PROJECT,
-        "tag": "0.0.1",
-        "rev": "hash_commit",
-        "authors": [
-            {
-                "fullname": "dummy-user",
-                "url_path": "user/dummy-user",
-                "name": "dummy-user",
-                "email": None,
-            }
-        ],
+        "project": PROJECT,
     }
-    message = GitTagDeletionV1(body=minimal_message)
+    message = ProjectUserAccessUpdatedV1(body=minimal_message)
     with pytest.raises(ValidationError):
         message.validate()
 
 
 def test_str():
     """Assert __str__ produces a human-readable message."""
     body = {
         "agent": "dummy-user",
-        "repo": PROJECT,
-        "tag": "0.0.1",
-        "rev": "hash_commit",
-        "authors": [
-            {
-                "fullname": "dummy-user",
-                "url_path": "user/dummy-user",
-                "name": "dummy-user",
-                "email": None,
-            }
-        ],
+        "project": PROJECT,
+        "new_user": "newu",
+        "new_access": "commit",
     }
-    expected_str = "Git tag: 0.0.1 deleted\nBy: dummy-user"
-    message = GitTagDeletionV1(body=body)
+    expected_str = (
+        "User: newu access edited to commit on "
+        "fedora-infra/fedocal-messages\nBy: dummy-user"
+    )
+    message = ProjectUserAccessUpdatedV1(body=body)
     message.validate()
     assert expected_str == str(message)
 
 
 def test_summary():
     """Assert the summary is correct."""
     body = {
         "agent": "dummy-user",
-        "repo": PROJECT,
-        "tag": "0.0.1",
-        "rev": "hash_commit",
-        "authors": [
-            {
-                "fullname": "dummy-user",
-                "url_path": "user/dummy-user",
-                "name": "dummy-user",
-                "email": None,
-            }
-        ],
+        "project": PROJECT,
+        "new_user": "newu",
+        "new_access": "commit",
     }
     expected_summary = (
-        "dummy-user deleted the tag 0.0.1 of commit hash_commit on "
-        "fedora-infra/fedocal-messages"
+        "dummy-user updated the access of newu to commit on "
+        'the project "fedora-infra/fedocal-messages"'
     )
-    message = GitTagDeletionV1(body=body)
+    message = ProjectUserAccessUpdatedV1(body=body)
     message.validate()
     assert expected_summary == message.summary
```

### Comparing `pagure-messages-0.0.6/pagure_messages/tests/test_group_edit.py` & `pagure-messages-1.0.0/pagure_messages/tests/test_group_edit.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-0.0.6/pagure_messages/tests/test_issue_assigned_added.py` & `pagure-messages-1.0.0/pagure_messages/tests/test_issue_assigned_added.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-0.0.6/pagure_messages/tests/test_issue_assigned_reset.py` & `pagure-messages-1.0.0/pagure_messages/tests/test_issue_assigned_reset.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-0.0.6/pagure_messages/tests/test_issue_comment_added.py` & `pagure-messages-1.0.0/pagure_messages/tests/test_issue_comment_added.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-0.0.6/pagure_messages/tests/test_issue_dependency_added.py` & `pagure-messages-1.0.0/pagure_messages/tests/test_issue_dependency_added.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-0.0.6/pagure_messages/tests/test_issue_dependency_removed.py` & `pagure-messages-1.0.0/pagure_messages/tests/test_issue_dependency_removed.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-0.0.6/pagure_messages/tests/test_issue_drop.py` & `pagure-messages-1.0.0/pagure_messages/tests/test_issue_drop.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-0.0.6/pagure_messages/tests/test_issue_edit.py` & `pagure-messages-1.0.0/pagure_messages/tests/test_issue_edit.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-0.0.6/pagure_messages/tests/test_issue_new.py` & `pagure-messages-1.0.0/pagure_messages/tests/test_issue_new.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-0.0.6/pagure_messages/tests/test_issue_tag_added.py` & `pagure-messages-1.0.0/pagure_messages/tests/test_issue_tag_added.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-0.0.6/pagure_messages/tests/test_issue_tag_removed.py` & `pagure-messages-1.0.0/pagure_messages/tests/test_issue_tag_removed.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-0.0.6/pagure_messages/tests/test_object_from_topic.py` & `pagure-messages-1.0.0/pagure_messages/tests/test_object_from_topic.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,28 +12,31 @@
 #
 # You should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 
 """Unit tests for common properties of the message schemas."""
 
+from .utils import PROJECT
 from .. import get_message_object_from_topic
 
 
 def test_object_type():
     """Assert some properties are correct."""
     cls = get_message_object_from_topic("pagure.git.receive")
-    assert str(type(cls())) == "<class 'pagure_messages.git_schema.GitReceiveV1'>"
+    msg = cls(body={"repo": PROJECT})
+    assert str(type(msg)) == "<class 'pagure_messages.git_schema.GitReceiveV1'>"
 
 
 def test_topic():
     """Assert some properties are correct."""
     cls = get_message_object_from_topic("pagure.git.receive")
+    msg = cls(body={"repo": PROJECT})
 
-    assert cls().topic == "pagure.git.receive"
+    assert msg.topic == "pagure.git.receive"
 
 
 def test_invalidtopic():
     """Assert some properties are correct."""
     cls = get_message_object_from_topic("fedocal.invalid.topic")
 
     assert str(type(cls())) == "<class 'fedora_messaging.message.Message'>"
```

### Comparing `pagure-messages-0.0.6/pagure_messages/tests/test_project_deleted.py` & `pagure-messages-1.0.0/pagure_messages/tests/test_project_deleted.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     """
     body = {
         "agent": "dummy-user",
         "project": PROJECT,
     }
     message = ProjectDeletedV1(body=body)
     message.validate()
-    assert message.url == "https://pagure.io"
+    assert message.url == "http://localhost.localdomain/fedora-infra/fedocal-messages"
 
 
 def test_missing_fields():
     """Assert an exception is actually raised on validation failure."""
     minimal_message = {
         "project": PROJECT,
     }
```

### Comparing `pagure-messages-0.0.6/pagure_messages/tests/test_project_edit.py` & `pagure-messages-1.0.0/pagure_messages/tests/test_project_edit.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-0.0.6/pagure_messages/tests/test_project_forked.py` & `pagure-messages-1.0.0/pagure_messages/tests/test_project_forked.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-0.0.6/pagure_messages/tests/test_project_group_access_updated.py` & `pagure-messages-1.0.0/pagure_messages/tests/test_project_group_access_updated.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-0.0.6/pagure_messages/tests/test_project_group_added.py` & `pagure-messages-1.0.0/pagure_messages/tests/test_project_group_added.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-0.0.6/pagure_messages/tests/test_project_group_removed.py` & `pagure-messages-1.0.0/pagure_messages/tests/test_project_group_removed.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-0.0.6/pagure_messages/tests/test_project_new.py` & `pagure-messages-1.0.0/pagure_messages/tests/test_project_new.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-0.0.6/pagure_messages/tests/test_project_tag_edited.py` & `pagure-messages-1.0.0/pagure_messages/tests/test_project_tag_edited.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-0.0.6/pagure_messages/tests/test_project_tag_removed.py` & `pagure-messages-1.0.0/pagure_messages/tests/test_project_tag_removed.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-0.0.6/pagure_messages/tests/test_project_user_access_updated.py` & `pagure-messages-1.0.0/pagure_messages/tests/test_project_user_added.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,65 +17,59 @@
 """Unit tests for the message schema."""
 
 from jsonschema import ValidationError
 
 import pytest
 
 from .utils import PROJECT
-from ..project_schema import ProjectUserAccessUpdatedV1
+from ..project_schema import ProjectUserAddedV1
 
 
 def test_minimal():
     """
     Assert the message schema validates a message with the required fields.
     """
     body = {
         "agent": "dummy-user",
         "project": PROJECT,
     }
-    message = ProjectUserAccessUpdatedV1(body=body)
+    message = ProjectUserAddedV1(body=body)
     message.validate()
     assert message.url == "http://localhost.localdomain/fedora-infra/fedocal-messages"
 
 
 def test_missing_fields():
     """Assert an exception is actually raised on validation failure."""
     minimal_message = {
         "project": PROJECT,
     }
-    message = ProjectUserAccessUpdatedV1(body=minimal_message)
+    message = ProjectUserAddedV1(body=minimal_message)
     with pytest.raises(ValidationError):
         message.validate()
 
 
 def test_str():
     """Assert __str__ produces a human-readable message."""
     body = {
         "agent": "dummy-user",
         "project": PROJECT,
         "new_user": "newu",
-        "new_access": "commit",
     }
-    expected_str = (
-        "User: newu access edited to commit on "
-        "fedora-infra/fedocal-messages\nBy: dummy-user"
-    )
-    message = ProjectUserAccessUpdatedV1(body=body)
+    expected_str = "User: newu added to fedora-infra/fedocal-messages\nBy: dummy-user"
+    message = ProjectUserAddedV1(body=body)
     message.validate()
     assert expected_str == str(message)
 
 
 def test_summary():
     """Assert the summary is correct."""
     body = {
         "agent": "dummy-user",
         "project": PROJECT,
         "new_user": "newu",
-        "new_access": "commit",
     }
     expected_summary = (
-        "dummy-user updated the access of newu to commit on "
-        'the project "fedora-infra/fedocal-messages"'
+        'dummy-user added the newu to the project "fedora-infra/fedocal-messages"'
     )
-    message = ProjectUserAccessUpdatedV1(body=body)
+    message = ProjectUserAddedV1(body=body)
     message.validate()
     assert expected_summary == message.summary
```

### Comparing `pagure-messages-0.0.6/pagure_messages/tests/test_project_user_added.py` & `pagure-messages-1.0.0/pagure_messages/tests/test_project_user_removed.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,59 +17,62 @@
 """Unit tests for the message schema."""
 
 from jsonschema import ValidationError
 
 import pytest
 
 from .utils import PROJECT
-from ..project_schema import ProjectUserAddedV1
+from ..project_schema import ProjectUserRemovedV1
 
 
 def test_minimal():
     """
     Assert the message schema validates a message with the required fields.
     """
     body = {
         "agent": "dummy-user",
         "project": PROJECT,
     }
-    message = ProjectUserAddedV1(body=body)
+    message = ProjectUserRemovedV1(body=body)
     message.validate()
     assert message.url == "http://localhost.localdomain/fedora-infra/fedocal-messages"
 
 
 def test_missing_fields():
     """Assert an exception is actually raised on validation failure."""
     minimal_message = {
         "project": PROJECT,
     }
-    message = ProjectUserAddedV1(body=minimal_message)
+    message = ProjectUserRemovedV1(body=minimal_message)
     with pytest.raises(ValidationError):
         message.validate()
 
 
 def test_str():
     """Assert __str__ produces a human-readable message."""
     body = {
         "agent": "dummy-user",
         "project": PROJECT,
-        "new_user": "newu",
+        "removed_user": "newu",
     }
-    expected_str = "User: newu added to fedora-infra/fedocal-messages\nBy: dummy-user"
-    message = ProjectUserAddedV1(body=body)
+    expected_str = (
+        "User: newu removed from fedora-infra/fedocal-messages\nBy: dummy-user"
+    )
+    message = ProjectUserRemovedV1(body=body)
     message.validate()
     assert expected_str == str(message)
 
 
 def test_summary():
     """Assert the summary is correct."""
     body = {
         "agent": "dummy-user",
         "project": PROJECT,
-        "new_user": "newu",
+        "removed_user": "newu",
     }
     expected_summary = (
-        'dummy-user added the newu to the project "fedora-infra/fedocal-messages"'
+        "dummy-user removed the newu from the project "
+        '"fedora-infra/fedocal-messages"'
     )
-    message = ProjectUserAddedV1(body=body)
+    message = ProjectUserRemovedV1(body=body)
     message.validate()
     assert expected_summary == message.summary
```

### Comparing `pagure-messages-0.0.6/pagure_messages/tests/test_project_user_removed.py` & `pagure-messages-1.0.0/pagure_messages/tests/test_git_tag_creation.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,62 +17,101 @@
 """Unit tests for the message schema."""
 
 from jsonschema import ValidationError
 
 import pytest
 
 from .utils import PROJECT
-from ..project_schema import ProjectUserRemovedV1
+from ..git_schema import GitTagCreationV1
 
 
 def test_minimal():
     """
     Assert the message schema validates a message with the required fields.
     """
     body = {
         "agent": "dummy-user",
-        "project": PROJECT,
+        "repo": PROJECT,
+        "tag": "0.0.1",
+        "rev": "hash_commit",
+        "authors": [
+            {
+                "fullname": "dummy-user",
+                "url_path": "user/dummy-user",
+                "name": "dummy-user",
+                "email": None,
+            }
+        ],
     }
-    message = ProjectUserRemovedV1(body=body)
+    message = GitTagCreationV1(body=body)
     message.validate()
-    assert message.url == "http://localhost.localdomain/fedora-infra/fedocal-messages"
+    assert (
+        message.url
+        == "http://localhost.localdomain/fedora-infra/fedocal-messages/commits/0.0.1"
+    )
 
 
 def test_missing_fields():
     """Assert an exception is actually raised on validation failure."""
     minimal_message = {
-        "project": PROJECT,
+        "repo": PROJECT,
+        "tag": "0.0.1",
+        "rev": "hash_commit",
+        "authors": [
+            {
+                "fullname": "dummy-user",
+                "url_path": "user/dummy-user",
+                "name": "dummy-user",
+                "email": None,
+            }
+        ],
     }
-    message = ProjectUserRemovedV1(body=minimal_message)
+    message = GitTagCreationV1(body=minimal_message)
     with pytest.raises(ValidationError):
         message.validate()
 
 
 def test_str():
     """Assert __str__ produces a human-readable message."""
     body = {
         "agent": "dummy-user",
-        "project": PROJECT,
-        "removed_user": "newu",
+        "repo": PROJECT,
+        "tag": "0.0.1",
+        "rev": "hash_commit",
+        "authors": [
+            {
+                "fullname": "dummy-user",
+                "url_path": "user/dummy-user",
+                "name": "dummy-user",
+                "email": None,
+            }
+        ],
     }
-    expected_str = (
-        "User: newu removed from fedora-infra/fedocal-messages\nBy: dummy-user"
-    )
-    message = ProjectUserRemovedV1(body=body)
+    expected_str = "Git tag: 0.0.1 created\nBy: dummy-user"
+    message = GitTagCreationV1(body=body)
     message.validate()
     assert expected_str == str(message)
 
 
 def test_summary():
     """Assert the summary is correct."""
     body = {
         "agent": "dummy-user",
-        "project": PROJECT,
-        "removed_user": "newu",
+        "repo": PROJECT,
+        "tag": "0.0.1",
+        "rev": "hash_commit",
+        "authors": [
+            {
+                "fullname": "dummy-user",
+                "url_path": "user/dummy-user",
+                "name": "dummy-user",
+                "email": None,
+            }
+        ],
     }
     expected_summary = (
-        "dummy-user removed the newu from the project "
-        '"fedora-infra/fedocal-messages"'
+        "dummy-user tagged the commit hash_commit on "
+        "fedora-infra/fedocal-messages as 0.0.1"
     )
-    message = ProjectUserRemovedV1(body=body)
+    message = GitTagCreationV1(body=body)
     message.validate()
     assert expected_summary == message.summary
```

### Comparing `pagure-messages-0.0.6/pagure_messages/tests/test_pull_request_assigned_added.py` & `pagure-messages-1.0.0/pagure_messages/tests/test_pull_request_assigned_added.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-0.0.6/pagure_messages/tests/test_pull_request_assigned_reset.py` & `pagure-messages-1.0.0/pagure_messages/tests/test_pull_request_assigned_reset.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-0.0.6/pagure_messages/tests/test_pull_request_closed.py` & `pagure-messages-1.0.0/pagure_messages/tests/test_pull_request_closed.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-0.0.6/pagure_messages/tests/test_pull_request_comment_added.py` & `pagure-messages-1.0.0/pagure_messages/tests/test_pull_request_comment_added.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-0.0.6/pagure_messages/tests/test_pull_request_comment_edited.py` & `pagure-messages-1.0.0/pagure_messages/tests/test_pull_request_comment_edited.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-0.0.6/pagure_messages/tests/test_pull_request_flag_added.py` & `pagure-messages-1.0.0/pagure_messages/tests/test_pull_request_flag_added.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-0.0.6/pagure_messages/tests/test_pull_request_flag_updated.py` & `pagure-messages-1.0.0/pagure_messages/tests/test_pull_request_flag_updated.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-0.0.6/pagure_messages/tests/test_pull_request_initial_comment_edited.py` & `pagure-messages-1.0.0/pagure_messages/tests/test_pull_request_initial_comment_edited.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-0.0.6/pagure_messages/tests/test_pull_request_new.py` & `pagure-messages-1.0.0/pagure_messages/tests/test_pull_request_new.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-0.0.6/pagure_messages/tests/test_pull_request_rebased.py` & `pagure-messages-1.0.0/pagure_messages/tests/test_pull_request_rebased.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-0.0.6/pagure_messages/tests/test_pull_request_reopened.py` & `pagure-messages-1.0.0/pagure_messages/tests/test_pull_request_reopened.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-0.0.6/pagure_messages/tests/test_pull_request_tag_added.py` & `pagure-messages-1.0.0/pagure_messages/tests/test_pull_request_tag_added.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-0.0.6/pagure_messages/tests/test_pull_request_tag_removed.py` & `pagure-messages-1.0.0/pagure_messages/tests/test_pull_request_tag_removed.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-0.0.6/pagure_messages/tests/test_pull_request_updated.py` & `pagure-messages-1.0.0/pagure_messages/tests/test_pull_request_updated.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-0.0.6/pagure_messages/tests/test_test_notification.py` & `pagure-messages-1.0.0/pagure_messages/tests/test_test_notification.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-0.0.6/pagure_messages/tests/utils.py` & `pagure-messages-1.0.0/pagure_messages/tests/utils.py`

 * *Files identical despite different names*

### Comparing `pagure-messages-0.0.6/pagure_messages.egg-info/PKG-INFO` & `pagure-messages-1.0.0/pagure_messages.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: pagure-messages
-Version: 0.0.6
+Version: 1.0.0
 Summary: A schema package for messages sent by pagure
 Home-page: https://pagure.io/pagure
 Maintainer: Fedora Infrastructure Team
 Maintainer-email: infrastructure@lists.fedoraproject.org
 License: GPLv2+
-Description: # pagure messages
-        
-        A schema package for [pagure](https://pagure.io/pagure).
-        
-        See the [detailed documentation](https://fedora-messaging.readthedocs.io/en/latest/messages.html) on packaging your schemas.
-        
 Keywords: fedora
 Platform: Fedora
 Platform: GNU/Linux
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+License-File: LICENSE
+
+# pagure messages
+
+A schema package for [pagure](https://pagure.io/pagure).
+
+See the [detailed documentation](https://fedora-messaging.readthedocs.io/en/latest/messages.html) on packaging your schemas.
```

### Comparing `pagure-messages-0.0.6/pagure_messages.egg-info/SOURCES.txt` & `pagure-messages-1.0.0/pagure_messages.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pagure-messages-0.0.6/pagure_messages.egg-info/entry_points.txt` & `pagure-messages-1.0.0/pagure_messages.egg-info/entry_points.txt`

 * *Files 0% similar despite different names*

```diff
@@ -40,8 +40,7 @@
 pagure.pull-request.initial_comment.edited = pagure_messages.pull_requests_schema:PullRequestInitialCommentEditedV1
 pagure.pull-request.new = pagure_messages.pull_requests_schema:PullRequestNewV1
 pagure.pull-request.rebased = pagure_messages.pull_requests_schema:PullRequestRebasedV1
 pagure.pull-request.reopened = pagure_messages.pull_requests_schema:PullRequestReopenedV1
 pagure.pull-request.tag.added = pagure_messages.pull_requests_schema:PullRequestTagAddedV1
 pagure.pull-request.tag.removed = pagure_messages.pull_requests_schema:PullRequestTagRemovedV1
 pagure.pull-request.updated = pagure_messages.pull_requests_schema:PullRequestUpdatedV1
-
```

### Comparing `pagure-messages-0.0.6/setup.cfg` & `pagure-messages-1.0.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pagure-messages
-version = 0.0.6
+version = 1.0.0
 description = A schema package for messages sent by pagure
 long_description = file: README.md
 url = https://pagure.io/pagure
 maintainer = Fedora Infrastructure Team
 maintainer_email = infrastructure@lists.fedoraproject.org
 keywords = fedora
 platforms = Fedora, GNU/Linux
```

### Comparing `pagure-messages-0.0.6/tox.ini` & `pagure-messages-1.0.0/tox.ini`

 * *Files identical despite different names*

