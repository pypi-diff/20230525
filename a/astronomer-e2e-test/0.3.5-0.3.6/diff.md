# Comparing `tmp/astronomer_e2e_test-0.3.5-py3-none-any.whl.zip` & `tmp/astronomer_e2e_test-0.3.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 24526 bytes, number of entries: 37
+Zip file size: 24523 bytes, number of entries: 37
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 astronomer_ci/__init__.py
--rw-r--r--  2.0 unx     1848 b- defN 80-Jan-01 00:00 astronomer_ci/cli.py
+-rw-r--r--  2.0 unx     1844 b- defN 80-Jan-01 00:00 astronomer_ci/cli.py
 -rwxr-xr-x  2.0 unx     5350 b- defN 80-Jan-01 00:00 astronomer_ci/dockerhub.py
 -rw-r--r--  2.0 unx      643 b- defN 80-Jan-01 00:00 astronomer_ci/exceptions.py
--rw-r--r--  2.0 unx     4695 b- defN 80-Jan-01 00:00 astronomer_ci/github.py
+-rw-r--r--  2.0 unx     4692 b- defN 80-Jan-01 00:00 astronomer_ci/github.py
 -rw-r--r--  2.0 unx       24 b- defN 80-Jan-01 00:00 astronomer_ci/test/functional/Dockerfile
 -rw-r--r--  2.0 unx     2128 b- defN 80-Jan-01 00:00 astronomer_ci/test/functional/test_get_next_version.py
 -rw-r--r--  2.0 unx     1281 b- defN 80-Jan-01 00:00 astronomer_ci/test/unit/test_github.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 astronomer_e2e_test/__init__.py
 -rwxr-xr-x  2.0 unx     4615 b- defN 80-Jan-01 00:00 astronomer_e2e_test/astronomer_e2e_test.py
 -rwxr-xr-x  2.0 unx     4793 b- defN 80-Jan-01 00:00 astronomer_e2e_test/graphql_requests.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 astronomer_platform/__init__.py
@@ -27,13 +27,13 @@
 -rw-r--r--  2.0 unx     1145 b- defN 80-Jan-01 00:00 astronomer_platform/features/environment.py
 -rw-r--r--  2.0 unx     1291 b- defN 80-Jan-01 00:00 astronomer_platform/features/steps/auth.py
 -rw-r--r--  2.0 unx     2297 b- defN 80-Jan-01 00:00 astronomer_platform/features/steps/deployments-api.py
 -rw-r--r--  2.0 unx      861 b- defN 80-Jan-01 00:00 astronomer_platform/features/steps/deployments-cli.py
 -rw-r--r--  2.0 unx     1526 b- defN 80-Jan-01 00:00 astronomer_platform/features/steps/workspaces-api.py
 -rw-r--r--  2.0 unx     1508 b- defN 80-Jan-01 00:00 astronomer_platform/features/steps/workspaces-cli.py
 -rw-r--r--  2.0 unx      933 b- defN 80-Jan-01 00:00 astronomer_platform/regressions/009_deployments_regression_001_api.feature
--rw-r--r--  2.0 unx     1067 b- defN 80-Jan-01 00:00 astronomer_e2e_test-0.3.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     2817 b- defN 80-Jan-01 00:00 astronomer_e2e_test-0.3.5.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 astronomer_e2e_test-0.3.5.dist-info/WHEEL
--rw-r--r--  2.0 unx      186 b- defN 80-Jan-01 00:00 astronomer_e2e_test-0.3.5.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     3567 b- defN 16-Jan-01 00:00 astronomer_e2e_test-0.3.5.dist-info/RECORD
-37 files, 57700 bytes uncompressed, 18616 bytes compressed:  67.7%
+-rw-r--r--  2.0 unx     1067 b- defN 80-Jan-01 00:00 astronomer_e2e_test-0.3.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2817 b- defN 80-Jan-01 00:00 astronomer_e2e_test-0.3.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 astronomer_e2e_test-0.3.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx      186 b- defN 80-Jan-01 00:00 astronomer_e2e_test-0.3.6.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     3567 b- defN 16-Jan-01 00:00 astronomer_e2e_test-0.3.6.dist-info/RECORD
+37 files, 57693 bytes uncompressed, 18613 bytes compressed:  67.7%
```

## zipnote {}

```diff
@@ -90,23 +90,23 @@
 
 Filename: astronomer_platform/features/steps/workspaces-cli.py
 Comment: 
 
 Filename: astronomer_platform/regressions/009_deployments_regression_001_api.feature
 Comment: 
 
-Filename: astronomer_e2e_test-0.3.5.dist-info/LICENSE
+Filename: astronomer_e2e_test-0.3.6.dist-info/LICENSE
 Comment: 
 
-Filename: astronomer_e2e_test-0.3.5.dist-info/METADATA
+Filename: astronomer_e2e_test-0.3.6.dist-info/METADATA
 Comment: 
 
-Filename: astronomer_e2e_test-0.3.5.dist-info/WHEEL
+Filename: astronomer_e2e_test-0.3.6.dist-info/WHEEL
 Comment: 
 
-Filename: astronomer_e2e_test-0.3.5.dist-info/entry_points.txt
+Filename: astronomer_e2e_test-0.3.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: astronomer_e2e_test-0.3.5.dist-info/RECORD
+Filename: astronomer_e2e_test-0.3.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## astronomer_ci/cli.py

```diff
@@ -56,20 +56,20 @@
 )
 @click.option(
     "--github-organization",
     required=True,
     help='The name of the GitHub organization (e.g. "astronomer")',
 )
 @click.option(
-    "--committish",
+    "--commitish",
     required=True,
-    help='The small Git commit hash ("committish") you want for the release',
+    help='The small Git commit hash ("commitish") you want for the release',
 )
-def publish_github_release(version, github_repository, github_organization, committish):
-    publish_release(version, github_repository, github_organization, committish)
+def publish_github_release(version, github_repository, github_organization, commitish):
+    publish_release(version, github_repository, github_organization, commitish)
 
 
 # leave this here for backwards compatibility
 def astronomer_next_version():
     get_next_version()
```

## astronomer_ci/github.py

```diff
@@ -76,15 +76,15 @@
                 + str(invalid_config)
             ) from invalid_config
 
         yield tag
 
 
 def publish_release(
-    version, repo, org, committish, pre_release=False, github_client=None
+    version, repo, org, commitish, pre_release=False, github_client=None
 ):
     """Safely deploy a release to Github"""
     # If 'version' is None, then check in the current directory for
     # Chart.yaml
     if not version:
         if not os.path.isfile("Chart.yaml"):
             raise InvalidConfiguration(
@@ -118,10 +118,10 @@
     logging.debug(f"Publishing release {version}...")
     _ = repo.create_git_release(
         version,
         version,
         release_notes,
         draft=False,
         prerelease=pre_release,
-        target_committish=committish,
+        target_commitish=commitish,
     )
     logging.info(f"Published release {version}")
```

## Comparing `astronomer_e2e_test-0.3.5.dist-info/LICENSE` & `astronomer_e2e_test-0.3.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `astronomer_e2e_test-0.3.5.dist-info/METADATA` & `astronomer_e2e_test-0.3.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astronomer-e2e-test
-Version: 0.3.5
+Version: 0.3.6
 Summary: Astronomer scripts for internal use
 License: MIT
 Author: Steven Miller
 Author-email: sjmiller609@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
```

## Comparing `astronomer_e2e_test-0.3.5.dist-info/RECORD` & `astronomer_e2e_test-0.3.6.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 astronomer_ci/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-astronomer_ci/cli.py,sha256=L453HaKBNnGO9GrZUUWG6QfNmw_1N4E-p_IYBjKE3t4,1848
+astronomer_ci/cli.py,sha256=RdI62bveukCWIoXNRV1HPRvHSayD19ft9dxRctIFznM,1844
 astronomer_ci/dockerhub.py,sha256=Y8TgTYAUxLylPdRSO-znShJ4tuKVxttQFSP4t_j8VUo,5350
 astronomer_ci/exceptions.py,sha256=ZYJzoWya4My5l3SjRe_HLCtBC_L8_VOhdvkaZcleoGA,643
-astronomer_ci/github.py,sha256=kCm2p4srWaQkgaR-bPuyxOMZJKjP5Ixtv2TxrV3aCIU,4695
+astronomer_ci/github.py,sha256=Jq0HpVMa7X8cK0LcxksmM8V_a-Ye_3oWsKcR_j7QRw8,4692
 astronomer_ci/test/functional/Dockerfile,sha256=HV7f8mAvnd3Ln3r1IBWiWiWpUtpcKLOVX66li8gFm3o,24
 astronomer_ci/test/functional/test_get_next_version.py,sha256=x4mYmWDDY9XyoO6ouYZPmG5uoVSBtqmJOZQb1HNkLEg,2128
 astronomer_ci/test/unit/test_github.py,sha256=V3pNngsY4d8HkK6Oe8HGjONRSb9-OrT45AO7fXmNCCI,1281
 astronomer_e2e_test/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 astronomer_e2e_test/astronomer_e2e_test.py,sha256=Q-LssJg8Dcv5nY8mGgUNn-YWK9FWzS_OoXfgzrO1E6o,4615
 astronomer_e2e_test/graphql_requests.py,sha256=zT6KvF-ncniehvlK02kqiJnEqd_Pp_0kOfCcQhoKTH0,4793
 astronomer_platform/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -26,12 +26,12 @@
 astronomer_platform/features/environment.py,sha256=PE7oKBWlM0aZufPgmqsNZ7ISrmG4mVX7eiXD3g1djIc,1145
 astronomer_platform/features/steps/auth.py,sha256=Fni1lCsn1AYq33JDaQsRk95oi9p79WcFil012SOgvNo,1291
 astronomer_platform/features/steps/deployments-api.py,sha256=3-2VtI2-JrT8INU0tjR5_XbaLZe0ng85YpGknCgFtjs,2297
 astronomer_platform/features/steps/deployments-cli.py,sha256=I_yoa5zCAK-4MwvxRMoyRdOUVv5H_cPymrnGPLRzoyw,861
 astronomer_platform/features/steps/workspaces-api.py,sha256=ij1Uv9jK2BwucjiCXjz7FlBWpvpbhMzMnW6R1ujfVIU,1526
 astronomer_platform/features/steps/workspaces-cli.py,sha256=3_qfRd5Qq6WtmoHZKCaWV2nOz3aTVsYgdEq7AsHau3E,1508
 astronomer_platform/regressions/009_deployments_regression_001_api.feature,sha256=kzk23aCdLXf8MlhQLoToWQQzdD7HUj-p7z6-8c5SZLw,933
-astronomer_e2e_test-0.3.5.dist-info/LICENSE,sha256=Gej_qxfs522UPm5wwKagrIvW8LvM7vq6B4QahF6hKa4,1067
-astronomer_e2e_test-0.3.5.dist-info/METADATA,sha256=-LWUpYf3aiGg8YN9-f9tGBV2t6fJ5IQG9VMkHqJcMvU,2817
-astronomer_e2e_test-0.3.5.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-astronomer_e2e_test-0.3.5.dist-info/entry_points.txt,sha256=a1nUV5UZtDlfl-6Z4a6xLfo-q0BFSKhGtLDfwgH3Mao,186
-astronomer_e2e_test-0.3.5.dist-info/RECORD,,
+astronomer_e2e_test-0.3.6.dist-info/LICENSE,sha256=Gej_qxfs522UPm5wwKagrIvW8LvM7vq6B4QahF6hKa4,1067
+astronomer_e2e_test-0.3.6.dist-info/METADATA,sha256=hthO99tfxQkgZOPKfNLdeJpUyPj9QwUvR-L45qrCLXg,2817
+astronomer_e2e_test-0.3.6.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+astronomer_e2e_test-0.3.6.dist-info/entry_points.txt,sha256=a1nUV5UZtDlfl-6Z4a6xLfo-q0BFSKhGtLDfwgH3Mao,186
+astronomer_e2e_test-0.3.6.dist-info/RECORD,,
```

