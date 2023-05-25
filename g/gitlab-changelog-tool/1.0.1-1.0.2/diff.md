# Comparing `tmp/gitlab_changelog_tool-1.0.1-py3-none-any.whl.zip` & `tmp/gitlab_changelog_tool-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 7760 bytes, number of entries: 12
--rw-r--r--  2.0 unx       71 b- defN 23-May-22 12:10 gitlab_changelog_tool/__init__.py
--rw-r--r--  2.0 unx      140 b- defN 23-May-22 12:10 gitlab_changelog_tool/__main__.py
--rw-r--r--  2.0 unx     4574 b- defN 23-May-22 12:10 gitlab_changelog_tool/api.py
--rw-r--r--  2.0 unx     1989 b- defN 23-May-22 12:10 gitlab_changelog_tool/cli.py
--rw-r--r--  2.0 unx      614 b- defN 23-May-22 12:10 gitlab_changelog_tool/package.py
--rw-r--r--  2.0 unx      430 b- defN 23-May-22 12:10 gitlab_changelog_tool/templates/CHANGELOG.md
--rw-r--r--  2.0 unx     1502 b- defN 23-May-22 12:10 gitlab_changelog_tool-1.0.1.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     4623 b- defN 23-May-22 12:10 gitlab_changelog_tool-1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-22 12:10 gitlab_changelog_tool-1.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       77 b- defN 23-May-22 12:10 gitlab_changelog_tool-1.0.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       22 b- defN 23-May-22 12:10 gitlab_changelog_tool-1.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1103 b- defN 23-May-22 12:10 gitlab_changelog_tool-1.0.1.dist-info/RECORD
-12 files, 15237 bytes uncompressed, 5858 bytes compressed:  61.6%
+Zip file size: 7776 bytes, number of entries: 12
+-rw-r--r--  2.0 unx       71 b- defN 23-May-25 19:49 gitlab_changelog_tool/__init__.py
+-rw-r--r--  2.0 unx      140 b- defN 23-May-25 19:49 gitlab_changelog_tool/__main__.py
+-rw-r--r--  2.0 unx     4605 b- defN 23-May-25 19:49 gitlab_changelog_tool/api.py
+-rw-r--r--  2.0 unx     1989 b- defN 23-May-25 19:49 gitlab_changelog_tool/cli.py
+-rw-r--r--  2.0 unx      614 b- defN 23-May-25 19:49 gitlab_changelog_tool/package.py
+-rw-r--r--  2.0 unx      430 b- defN 23-May-25 19:49 gitlab_changelog_tool/templates/CHANGELOG.md
+-rw-r--r--  2.0 unx     1502 b- defN 23-May-25 19:49 gitlab_changelog_tool-1.0.2.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     4623 b- defN 23-May-25 19:49 gitlab_changelog_tool-1.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-25 19:49 gitlab_changelog_tool-1.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       77 b- defN 23-May-25 19:49 gitlab_changelog_tool-1.0.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       22 b- defN 23-May-25 19:49 gitlab_changelog_tool-1.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1103 b- defN 23-May-25 19:49 gitlab_changelog_tool-1.0.2.dist-info/RECORD
+12 files, 15268 bytes uncompressed, 5874 bytes compressed:  61.5%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: gitlab_changelog_tool/package.py
 Comment: 
 
 Filename: gitlab_changelog_tool/templates/CHANGELOG.md
 Comment: 
 
-Filename: gitlab_changelog_tool-1.0.1.dist-info/LICENSE.md
+Filename: gitlab_changelog_tool-1.0.2.dist-info/LICENSE.md
 Comment: 
 
-Filename: gitlab_changelog_tool-1.0.1.dist-info/METADATA
+Filename: gitlab_changelog_tool-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: gitlab_changelog_tool-1.0.1.dist-info/WHEEL
+Filename: gitlab_changelog_tool-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: gitlab_changelog_tool-1.0.1.dist-info/entry_points.txt
+Filename: gitlab_changelog_tool-1.0.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: gitlab_changelog_tool-1.0.1.dist-info/top_level.txt
+Filename: gitlab_changelog_tool-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: gitlab_changelog_tool-1.0.1.dist-info/RECORD
+Filename: gitlab_changelog_tool-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gitlab_changelog_tool/api.py

```diff
@@ -1,12 +1,12 @@
 '''
 Application implementation package.
 '''
 
-from datetime import datetime, timedelta
+from datetime import datetime, timedelta, timezone
 from operator import attrgetter
 from pathlib import Path
 from typing import Iterable, List
 
 import dateutil.parser
 import gitlab
 import semver
@@ -69,15 +69,15 @@
         current_tag_name = tag.name
         updated_after = (
             dateutil.parser.parse(
                 tag.commit['committed_date']) + timedelta(seconds=2)
         ).isoformat()
     except StopIteration:
         current_tag_name = 'v0.0.0'
-        updated_after = datetime(1970, 1, 1).isoformat()
+        updated_after = datetime(1970, 1, 1, tzinfo=timezone.utc).isoformat()
 
     if current_tag_name.startswith('v'):
         current_version = current_tag_name[1:]
     else:
         current_version = current_tag_name
 
     features = ensure_merge_request_format(
```

## gitlab_changelog_tool/package.py

```diff
@@ -2,15 +2,15 @@
 Package description information.
 '''
 
 #: Package display name.
 __title__ = 'GitLab Changelog Tool'
 
 #: Package version.
-__version__ = '1.0.1'
+__version__ = '1.0.2'
 
 #: Package description.
 __description__ = 'Automatically generate changelogs from merge requests on GitLab.'
 
 #: Package author name.
 __author__ = 'Danilo Peixoto Ferreira'
```

## Comparing `gitlab_changelog_tool-1.0.1.dist-info/LICENSE.md` & `gitlab_changelog_tool-1.0.2.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `gitlab_changelog_tool-1.0.1.dist-info/METADATA` & `gitlab_changelog_tool-1.0.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlab-changelog-tool
-Version: 1.0.1
+Version: 1.0.2
 Summary: Automatically generate changelogs from merge requests on GitLab.
 Home-page: https://github.com/danilopeixoto/gitlab-changelog-tool
 Download-URL: https://pypi.org/project/gitlab-changelog-tool
 Author: Danilo Peixoto Ferreira
 License: BSD-3-Clause
 Project-URL: Code, https://github.com/danilopeixoto/gitlab-changelog-tool
 Project-URL: Issue tracker, https://github.com/danilopeixoto/gitlab-changelog-tool/issues
```

