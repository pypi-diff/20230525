# Comparing `tmp/netbox-validity-1.2.0.tar.gz` & `tmp/netbox-validity-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-validity-1.2.0.tar", last modified: Tue May 16 00:03:00 2023, max compression
+gzip compressed data, was "netbox-validity-1.2.1.tar", last modified: Thu May 25 19:54:24 2023, max compression
```

## Comparing `netbox-validity-1.2.0.tar` & `netbox-validity-1.2.1.tar`

### file list

```diff
@@ -1,136 +1,139 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:03:00.109245 netbox-validity-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-05-16 00:03:00.109245 netbox-validity-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:03:00.097245 netbox-validity-1.2.0/netbox_validity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-05-16 00:03:00.000000 netbox-validity-1.2.0/netbox_validity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-05-16 00:03:00.000000 netbox-validity-1.2.0/netbox_validity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 00:03:00.000000 netbox-validity-1.2.0/netbox_validity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-16 00:03:00.000000 netbox-validity-1.2.0/netbox_validity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-16 00:03:00.000000 netbox-validity-1.2.0/netbox_validity.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:03:00.097245 netbox-validity-1.2.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 00:03:00.113245 netbox-validity-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:03:00.101245 netbox-validity-1.2.0/validity/
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:03:00.101245 netbox-validity-1.2.0/validity/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/api/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9744 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/choices.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:03:00.101245 netbox-validity-1.2.0/validity/config_compliance/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:03:00.101245 netbox-validity-1.2.0/validity/config_compliance/device_config/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/config_compliance/device_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/config_compliance/device_config/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/config_compliance/device_config/routeros.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/config_compliance/device_config/ttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/config_compliance/device_config/yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/config_compliance/dynamic_pairs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:03:00.101245 netbox-validity-1.2.0/validity/config_compliance/eval/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/config_compliance/eval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/config_compliance/eval/default_nameset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/config_compliance/eval/eval.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/config_compliance/eval/eval_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/config_compliance/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/filtersets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:03:00.101245 netbox-validity-1.2.0/validity/forms/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/forms/filterset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/forms/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/forms/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/graphql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:03:00.101245 netbox-validity-1.2.0/validity/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:03:00.101245 netbox-validity-1.2.0/validity/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/management/commands/linkscripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/managers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:03:00.101245 netbox-validity-1.2.0/validity/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    12486 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/migrations/0002_custom_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/migrations/0003_complianceselector_dp_tag_prefix.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:03:00.105245 netbox-validity-1.2.0/validity/models/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/models/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/models/nameset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/models/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/models/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/models/selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/models/serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/models/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/models/test_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/navigation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:03:00.105245 netbox-validity-1.2.0/validity/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/scripts/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/scripts/run_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:03:00.097245 netbox-validity-1.2.0/validity/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:03:00.105245 netbox-validity-1.2.0/validity/templates/validity/
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/templates/validity/compliance_results.html
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/templates/validity/compliancereport.html
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/templates/validity/complianceselector.html
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/templates/validity/compliancetest.html
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/templates/validity/compliancetestresult.html
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/templates/validity/configserializer.html
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/templates/validity/device_config.html
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/templates/validity/gitrepo.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:03:00.105245 netbox-validity-1.2.0/validity/templates/validity/inc/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/templates/validity/inc/git_link.html
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/templates/validity/inc/path_with_link.html
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/templates/validity/inc/report_stats_row.html
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/templates/validity/inc/search_form.html
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/templates/validity/nameset.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:03:00.105245 netbox-validity-1.2.0/validity/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/templatetags/validity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:03:00.109245 netbox-validity-1.2.0/validity/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/tests/test_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:03:00.109245 netbox-validity-1.2.0/validity/tests/test_config_compliance/
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/tests/test_config_compliance/test_device_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/tests/test_config_compliance/test_dynamic_pairs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/tests/test_config_compliance/test_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/tests/test_graphql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:03:00.109245 netbox-validity-1.2.0/validity/tests/test_models/
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/tests/test_models/test_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/tests/test_models/test_git_link.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/tests/test_models/test_git_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/tests/test_models/test_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/tests/test_models/test_vdevice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:03:00.109245 netbox-validity-1.2.0/validity/tests/test_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/tests/test_scripts/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/tests/test_scripts/test_run_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:03:00.109245 netbox-validity-1.2.0/validity/tests/test_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/tests/test_utils/test_git.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/tests/test_utils/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:03:00.109245 netbox-validity-1.2.0/validity/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/utils/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/utils/password.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 00:03:00.109245 netbox-validity-1.2.0/validity/views/
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/views/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/views/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/views/git_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/views/nameset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/views/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/views/selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/views/serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/views/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-16 00:02:46.000000 netbox-validity-1.2.0/validity/views/test_result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:24.473896 netbox-validity-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-05-25 19:54:24.473896 netbox-validity-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:24.453896 netbox-validity-1.2.1/netbox_validity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-05-25 19:54:24.000000 netbox-validity-1.2.1/netbox_validity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-05-25 19:54:24.000000 netbox-validity-1.2.1/netbox_validity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 19:54:24.000000 netbox-validity-1.2.1/netbox_validity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-25 19:54:24.000000 netbox-validity-1.2.1/netbox_validity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-25 19:54:24.000000 netbox-validity-1.2.1/netbox_validity.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:24.453896 netbox-validity-1.2.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 19:54:24.473896 netbox-validity-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:24.457896 netbox-validity-1.2.1/validity/
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:24.457896 netbox-validity-1.2.1/validity/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/api/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9744 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/choices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:24.457896 netbox-validity-1.2.1/validity/config_compliance/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:24.457896 netbox-validity-1.2.1/validity/config_compliance/device_config/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/config_compliance/device_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/config_compliance/device_config/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/config_compliance/device_config/routeros.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/config_compliance/device_config/ttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/config_compliance/device_config/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/config_compliance/dynamic_pairs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:24.461896 netbox-validity-1.2.1/validity/config_compliance/eval/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/config_compliance/eval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/config_compliance/eval/default_nameset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/config_compliance/eval/eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/config_compliance/eval/eval_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/config_compliance/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/filtersets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:24.461896 netbox-validity-1.2.1/validity/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/forms/filterset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/forms/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/forms/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/graphql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:24.461896 netbox-validity-1.2.1/validity/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:24.461896 netbox-validity-1.2.1/validity/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/management/commands/linkscripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/managers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:24.461896 netbox-validity-1.2.1/validity/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    12486 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/migrations/0002_custom_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/migrations/0003_complianceselector_dp_tag_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/migrations/0004_netbox35_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:24.465896 netbox-validity-1.2.1/validity/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/models/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/models/nameset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/models/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/models/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/models/selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/models/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/models/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/models/test_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/navigation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:24.465896 netbox-validity-1.2.1/validity/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/scripts/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/scripts/run_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/scripts/validity_git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/scripts/validity_run_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:24.449896 netbox-validity-1.2.1/validity/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:24.465896 netbox-validity-1.2.1/validity/templates/validity/
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/templates/validity/compliance_results.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/templates/validity/compliancereport.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/templates/validity/complianceselector.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/templates/validity/compliancetest.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/templates/validity/compliancetestresult.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/templates/validity/configserializer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/templates/validity/device_config.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/templates/validity/gitrepo.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:24.465896 netbox-validity-1.2.1/validity/templates/validity/inc/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/templates/validity/inc/git_link.html
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/templates/validity/inc/path_with_link.html
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/templates/validity/inc/report_stats_row.html
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/templates/validity/inc/search_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/templates/validity/nameset.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:24.469896 netbox-validity-1.2.1/validity/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/templatetags/validity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:24.469896 netbox-validity-1.2.1/validity/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/tests/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:24.469896 netbox-validity-1.2.1/validity/tests/test_config_compliance/
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/tests/test_config_compliance/test_device_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/tests/test_config_compliance/test_dynamic_pairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/tests/test_config_compliance/test_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/tests/test_graphql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:24.469896 netbox-validity-1.2.1/validity/tests/test_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/tests/test_models/test_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/tests/test_models/test_git_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/tests/test_models/test_git_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/tests/test_models/test_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/tests/test_models/test_vdevice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:24.473896 netbox-validity-1.2.1/validity/tests/test_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/tests/test_scripts/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6804 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/tests/test_scripts/test_run_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:24.473896 netbox-validity-1.2.1/validity/tests/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/tests/test_utils/test_git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/tests/test_utils/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:24.473896 netbox-validity-1.2.1/validity/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/utils/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/utils/password.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:54:24.473896 netbox-validity-1.2.1/validity/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/views/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/views/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/views/git_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/views/nameset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/views/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/views/selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/views/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/views/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-25 19:54:07.000000 netbox-validity-1.2.1/validity/views/test_result.py
```

### Comparing `netbox-validity-1.2.0/LICENSE` & `netbox-validity-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/PKG-INFO` & `netbox-validity-1.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6e65 7462  : 2.1.Name: netb
 00000020: 6f78 2d76 616c 6964 6974 790a 5665 7273  ox-validity.Vers
-00000030: 696f 6e3a 2031 2e32 2e30 0a53 756d 6d61  ion: 1.2.0.Summa
+00000030: 696f 6e3a 2031 2e32 2e31 0a53 756d 6d61  ion: 1.2.1.Summa
 00000040: 7279 3a20 4e65 7442 6f78 2070 6c75 6769  ry: NetBox plugi
 00000050: 6e20 666f 7220 7665 6e64 6f72 2d61 676e  n for vendor-agn
 00000060: 6f73 7469 6320 636f 6e66 6967 7572 6174  ostic configurat
 00000070: 696f 6e20 636f 6d70 6c69 616e 6365 0a41  ion compliance.A
 00000080: 7574 686f 722d 656d 6169 6c3a 2041 6e74  uthor-email: Ant
 00000090: 6f6e 204d 6961 736e 696b 6f76 203c 616e  on Miasnikov <an
 000000a0: 746f 6e32 3030 386d 4067 6d61 696c 2e63  ton2008m@gmail.c
@@ -137,269 +137,304 @@
 00000880: 6e3a 203e 3d33 2e31 300a 4465 7363 7269  n: >=3.10.Descri
 00000890: 7074 696f 6e2d 436f 6e74 656e 742d 5479  ption-Content-Ty
 000008a0: 7065 3a20 7465 7874 2f6d 6172 6b64 6f77  pe: text/markdow
 000008b0: 6e0a 5072 6f76 6964 6573 2d45 7874 7261  n.Provides-Extra
 000008c0: 3a20 6465 760a 5072 6f76 6964 6573 2d45  : dev.Provides-E
 000008d0: 7874 7261 3a20 646f 6373 0a4c 6963 656e  xtra: docs.Licen
 000008e0: 7365 2d46 696c 653a 204c 4943 454e 5345  se-File: LICENSE
-000008f0: 0a0a 2320 5661 6c69 6469 7479 3a20 7665  ..# Validity: ve
-00000900: 6e64 6f72 2d61 676e 6f73 7469 6320 636f  ndor-agnostic co
-00000910: 6e66 6967 7572 6174 696f 6e20 636f 6d70  nfiguration comp
-00000920: 6c69 616e 6365 0a0a 215b 4349 5d28 6874  liance..![CI](ht
-00000930: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000940: 2f61 6d79 6173 6e69 6b6f 762f 7661 6c69  /amyasnikov/vali
-00000950: 6469 7479 2f61 6374 696f 6e73 2f77 6f72  dity/actions/wor
-00000960: 6b66 6c6f 7773 2f63 692e 796d 6c2f 6261  kflows/ci.yml/ba
-00000970: 6467 652e 7376 6729 0a21 5b43 6f76 6572  dge.svg).![Cover
-00000980: 6167 655d 2868 7474 7073 3a2f 2f69 6d67  age](https://img
-00000990: 2e73 6869 656c 6473 2e69 6f2f 656e 6470  .shields.io/endp
-000009a0: 6f69 6e74 3f75 726c 3d68 7474 7073 3a2f  oint?url=https:/
-000009b0: 2f67 6973 742e 6769 7468 7562 7573 6572  /gist.githubuser
-000009c0: 636f 6e74 656e 742e 636f 6d2f 616d 7961  content.com/amya
-000009d0: 736e 696b 6f76 2f39 6535 3138 6165 3862  snikov/9e518ae8b
-000009e0: 6162 6431 3862 3765 6464 3865 6535 6161  abd18b7edd8ee5aa
-000009f0: 6435 3831 3436 622f 7261 772f 636f 762e  d58146b/raw/cov.
-00000a00: 6a73 6f6e 290a 215b 5079 7468 6f6e 2076  json).![Python v
-00000a10: 6572 7369 6f6e 5d28 6874 7470 733a 2f2f  ersion](https://
-00000a20: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
-00000a30: 6164 6765 2f50 7974 686f 6e2d 332e 3130  adge/Python-3.10
-00000a40: 2b2d 626c 7565 2e73 7667 290a 215b 4e65  +-blue.svg).![Ne
-00000a50: 7442 6f78 2076 6572 7369 6f6e 5d28 6874  tBox version](ht
-00000a60: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-00000a70: 732e 696f 2f62 6164 6765 2f4e 6574 426f  s.io/badge/NetBo
-00000a80: 782d 332e 347c 332e 352d 626c 7565 2e73  x-3.4|3.5-blue.s
-00000a90: 7667 290a 0a3c 212d 2d6d 6b64 6f63 732d  vg)..<!--mkdocs-
-00000aa0: 7374 6172 742d 2d3e 0a23 2320 5768 6174  start-->.## What
-00000ab0: 3f0a 5661 6c69 6469 7479 2069 7320 7468  ?.Validity is th
-00000ac0: 6520 5b4e 6574 426f 785d 2868 7474 7073  e [NetBox](https
-00000ad0: 3a2f 2f6e 6574 626f 782e 6465 7629 2070  ://netbox.dev) p
-00000ae0: 6c75 6769 6e20 746f 2064 6561 6c20 7769  lugin to deal wi
-00000af0: 7468 2063 6f6e 6669 6775 7261 7469 6f6e  th configuration
-00000b00: 2063 6f6d 706c 6961 6e63 652e 2059 6f75   compliance. You
-00000b10: 2064 6566 696e 6520 636f 6d70 6c69 616e   define complian
-00000b20: 6365 2074 6573 7473 2061 6e64 2056 616c  ce tests and Val
-00000b30: 6964 6974 7920 6368 6563 6b73 206e 6574  idity checks net
-00000b40: 776f 726b 2064 6576 6963 6520 636f 6e66  work device conf
-00000b50: 6967 7572 6174 696f 6e20 6669 6c65 7320  iguration files 
-00000b60: 6167 6169 6e73 7420 7468 6573 6520 7465  against these te
-00000b70: 7374 732e 2041 7320 6120 7265 7375 6c74  sts. As a result
-00000b80: 2079 6f75 2063 616e 2066 696e 6420 6f75   you can find ou
-00000b90: 7420 7768 6963 6820 6465 7669 6365 7320  t which devices 
-00000ba0: 6172 6520 7072 6f76 6973 696f 6e65 6420  are provisioned 
-00000bb0: 7072 6f70 6572 6c79 2028 6163 636f 7264  properly (accord
-00000bc0: 696e 6720 746f 2074 6865 2074 6573 7473  ing to the tests
-00000bd0: 2079 6f75 2068 6176 6520 7772 6974 7465   you have writte
-00000be0: 6e29 2061 6e64 2077 6869 6368 2061 7265  n) and which are
-00000bf0: 206e 6f74 2e0a 0a54 6f20 7573 6520 7661   not...To use va
-00000c00: 6c69 6469 7479 2079 6f75 206e 6565 643a  lidity you need:
-00000c10: 0a0a 312e 2053 746f 7265 2063 6f6e 6669  ..1. Store confi
-00000c20: 6775 7261 7469 6f6e 2066 696c 6573 206f  guration files o
-00000c30: 6620 796f 7572 2064 6576 6963 6573 2069  f your devices i
-00000c40: 6e20 6120 4769 7420 7265 706f 7369 746f  n a Git reposito
-00000c50: 7279 2e20 5661 6c69 6469 7479 2064 6f65  ry. Validity doe
-00000c60: 7320 6e6f 7420 636f 6c6c 6563 7420 7468  s not collect th
-00000c70: 6520 636f 6e66 6967 7320 6672 6f6d 2079  e configs from y
-00000c80: 6f75 7220 6e65 7477 6f72 6b2c 2079 6f75  our network, you
-00000c90: 2068 6176 6520 746f 2064 6f20 6974 2062   have to do it b
-00000ca0: 7920 7468 6972 642d 7061 7274 7920 746f  y third-party to
-00000cb0: 6f6c 2028 652e 672e 205b 6f78 6964 697a  ol (e.g. [oxidiz
-00000cc0: 6564 5d28 6874 7470 733a 2f2f 6769 7468  ed](https://gith
-00000cd0: 7562 2e63 6f6d 2f79 7474 692f 6f78 6964  ub.com/ytti/oxid
-00000ce0: 697a 6564 2929 2e0a 0a32 2e20 4465 6669  ized))...2. Defi
-00000cf0: 6e65 205b 5454 5020 5465 6d70 6c61 7465  ne [TTP Template
-00000d00: 5d28 6874 7470 733a 2f2f 7474 702e 7265  ](https://ttp.re
-00000d10: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
-00000d20: 6c61 7465 7374 2f29 2074 6f20 7472 616e  latest/) to tran
-00000d30: 736c 6174 6520 7468 6520 636f 6e66 6967  slate the config
-00000d40: 2066 726f 6d20 7665 6e64 6f72 2073 7065   from vendor spe
-00000d50: 6369 6669 6320 666f 726d 6174 2069 6e74  cific format int
-00000d60: 6f20 4a53 4f4e 2e0a 0a33 2e20 5772 6974  o JSON...3. Writ
-00000d70: 6520 636f 6d70 6c69 616e 6365 2074 6573  e compliance tes
-00000d80: 7420 6173 2061 2070 7974 686f 6e20 6578  t as a python ex
-00000d90: 7072 6573 7369 6f6e 2c20 652e 672e 3c62  pression, e.g.<b
-00000da0: 722f 3e0a 6064 6576 6963 652e 636f 6e66  r/>.`device.conf
-00000db0: 6967 5b22 6e74 702d 7365 7276 6572 7322  ig["ntp-servers"
-00000dc0: 5d20 3d3d 205b 2231 2e32 2e33 2e34 222c  ] == ["1.2.3.4",
-00000dd0: 2022 352e 362e 372e 3822 5d60 0a0a 342e   "5.6.7.8"]`..4.
-00000de0: 2041 7070 6c79 2063 7265 6174 6564 2074   Apply created t
-00000df0: 6573 7420 746f 2073 7065 6369 6669 6320  est to specific 
-00000e00: 6465 7669 6365 7320 616e 6420 6765 7420  devices and get 
-00000e10: 7468 6520 7265 7375 6c74 7320 7065 7220  the results per 
-00000e20: 6465 7669 6365 2028 7061 7373 6564 206f  device (passed o
-00000e30: 7220 6661 696c 6564 292e 0a0a 0a23 2320  r failed)....## 
-00000e40: 5768 793f 0a43 6f6e 6669 6775 7261 7469  Why?.Configurati
-00000e50: 6f6e 2063 6f6d 706c 6961 6e63 6520 6973  on compliance is
-00000e60: 206f 6e65 206f 6620 7468 6520 7665 7279   one of the very
-00000e70: 2063 6f6d 6d6f 6e20 7072 6f62 6c65 6d73   common problems
-00000e80: 2074 6861 7420 6172 6973 6573 2069 6e20   that arises in 
-00000e90: 6576 6572 7920 636f 6d70 616e 7920 7769  every company wi
-00000ea0: 7468 2074 6865 2067 726f 7774 6820 6f66  th the growth of
-00000eb0: 2074 6865 6972 206e 6574 776f 726b 2e20   their network. 
-00000ec0: 5573 7561 6c6c 7920 636f 6d70 616e 6965  Usually companie
-00000ed0: 7320 736f 6c76 6520 7468 6973 2070 726f  s solve this pro
-00000ee0: 626c 656d 2077 6974 6820 736f 6d65 206b  blem with some k
-00000ef0: 696e 6420 6f66 2073 6372 6970 7473 2074  ind of scripts t
-00000f00: 6861 7420 646f 2061 6c6c 2074 6865 2074  hat do all the t
-00000f10: 6869 6e67 7320 6174 2074 6865 2073 616d  hings at the sam
-00000f20: 6520 7469 6d65 3a20 7468 6579 2070 6172  e time: they par
-00000f30: 7365 2063 6f6e 6669 6773 2c20 6170 706c  se configs, appl
-00000f40: 7920 736f 6d65 2063 6f6d 706c 6961 6e63  y some complianc
-00000f50: 6520 6c6f 6769 6320 616e 6420 7075 7368  e logic and push
-00000f60: 2074 6865 2072 6573 756c 7473 2069 6e74   the results int
-00000f70: 6f20 736f 6d65 2044 4220 6f72 2074 6869  o some DB or thi
-00000f80: 7264 2d70 6172 7479 204f 5353 2073 7973  rd-party OSS sys
-00000f90: 7465 6d2e 2055 7375 616c 6c79 2061 6674  tem. Usually aft
-00000fa0: 6572 2074 6865 2061 6464 6974 696f 6e20  er the addition 
-00000fb0: 6f66 2073 6576 6572 616c 2076 656e 646f  of several vendo
-00000fc0: 7273 2028 6f72 2065 7665 6e20 7365 7665  rs (or even seve
-00000fd0: 7261 6c20 736f 6674 7761 7265 2072 6576  ral software rev
-00000fe0: 6973 696f 6e73 206f 6620 6f6e 6520 6d6f  isions of one mo
-00000ff0: 6465 6c29 2074 6865 7365 2073 6372 6970  del) these scrip
-00001000: 7473 2062 6563 6f6d 6520 756e 7265 6164  ts become unread
-00001010: 6162 6c65 2061 6e64 2061 6c6d 6f73 7420  able and almost 
-00001020: 6e6f 206f 6e65 2063 616e 2064 6566 696e  no one can defin
-00001030: 6974 656c 7920 7361 7920 7768 6963 6820  itely say which 
-00001040: 7275 6c65 7320 7468 6520 7363 7269 7074  rules the script
-00001050: 2063 6865 636b 7320 666f 722e 0a0a 5661   checks for...Va
-00001060: 6c69 6469 7479 2063 6f6d 706c 6574 656c  lidity completel
-00001070: 7920 7365 7061 7261 7465 7320 636f 6d70  y separates comp
-00001080: 6c69 616e 6365 2074 6573 7420 636f 6465  liance test code
-00001090: 2066 726f 6d20 616c 6c20 6f74 6865 7220   from all other 
-000010a0: 7468 696e 6773 206c 696b 6520 636f 6e66  things like conf
-000010b0: 6967 2073 6572 6961 6c69 7a61 7469 6f6e  ig serialization
-000010c0: 2e20 5468 6973 206f 6e65 2065 6e63 6f75  . This one encou
-000010d0: 7261 6765 7320 796f 7520 746f 2077 7269  rages you to wri
-000010e0: 7465 2073 686f 7274 2c20 636c 6561 6e20  te short, clean 
-000010f0: 616e 6420 756e 6465 7273 7461 6e64 6162  and understandab
-00001100: 6c65 2063 6f6d 706c 6961 6e63 6520 7465  le compliance te
-00001110: 7374 7320 746f 6765 7468 6572 2077 6974  sts together wit
-00001120: 6820 7468 6520 6d61 6e64 6174 6f72 7920  h the mandatory 
-00001130: 6465 7363 7269 7074 696f 6e2e 0a0a 0a23  description....#
-00001140: 2320 4b65 7920 6665 6174 7572 6573 0a2a  # Key features.*
-00001150: 2054 7275 6c79 2076 656e 646f 722d 6167   Truly vendor-ag
-00001160: 6e6f 7374 6963 2e20 596f 7520 6361 6e20  nostic. You can 
-00001170: 6561 7369 6c79 2069 6e74 6567 7261 7465  easily integrate
-00001180: 2061 6e79 2076 656e 646f 7220 636f 6e66   any vendor conf
-00001190: 6967 2066 6f72 6d61 7420 7573 696e 6720  ig format using 
-000011a0: 5b54 5450 5d28 6874 7470 733a 2f2f 6769  [TTP](https://gi
-000011b0: 7468 7562 2e63 6f6d 2f64 6d75 6c79 616c  thub.com/dmulyal
-000011c0: 696e 2f74 7470 290a 2a20 5772 6974 696e  in/ttp).* Writin
-000011d0: 6720 636f 6d70 6c69 616e 6365 2074 6573  g compliance tes
-000011e0: 7473 2075 7369 6e67 2050 7974 686f 6e20  ts using Python 
-000011f0: 6578 7072 6573 7369 6f6e 7320 616e 6420  expressions and 
-00001200: 5b4a 515d 2868 7474 7073 3a2f 2f73 7465  [JQ](https://ste
-00001210: 646f 6c61 6e2e 6769 7468 7562 2e69 6f2f  dolan.github.io/
-00001220: 6a71 2f6d 616e 7561 6c2f 290a 2a20 466c  jq/manual/).* Fl
-00001230: 6578 6962 6c65 2073 656c 6563 746f 7220  exible selector 
-00001240: 7379 7374 656d 2074 6f20 6170 706c 7920  system to apply 
-00001250: 7468 6520 7465 7374 7320 6f6e 6c79 2074  the tests only t
-00001260: 6f20 6120 7370 6563 6966 6963 2073 7562  o a specific sub
-00001270: 7365 7420 6f66 2064 6576 6963 6573 0a2a  set of devices.*
-00001280: 2043 6f6e 6365 7074 206f 6620 2a2a 6479   Concept of **dy
-00001290: 6e61 6d69 6320 7061 6972 732a 2a2e 2057  namic pairs**. W
-000012a0: 6974 6820 6479 6e61 6d69 6320 7061 6972  ith dynamic pair
-000012b0: 2079 6f75 2063 616e 2063 6f6d 7061 7265   you can compare
-000012c0: 2032 2064 6966 6665 7265 6e74 2064 6576   2 different dev
-000012d0: 6963 6573 2062 6574 7765 656e 2065 6163  ices between eac
-000012e0: 6820 6f74 6865 7220 2865 2e67 2e20 636f  h other (e.g. co
-000012f0: 6d70 6172 6520 7468 6520 636f 6e66 6967  mpare the config
-00001300: 7572 6174 696f 6e20 6f66 2032 204d 432d  uration of 2 MC-
-00001310: 4c41 4720 6d65 6d62 6572 7329 2e0a 2a20  LAG members)..* 
-00001320: 2a2a 5465 7374 2072 6573 756c 7420 6578  **Test result ex
-00001330: 706c 616e 6174 696f 6e2a 2a2e 2057 6865  planation**. Whe
-00001340: 6e20 736f 6d65 2074 6573 7420 6661 696c  n some test fail
-00001350: 732c 2079 6f75 2063 616e 2067 6574 2074  s, you can get t
-00001360: 6865 202a 2a65 7870 6c61 6e61 7469 6f6e  he **explanation
-00001370: 2a2a 206f 6620 7468 6520 6361 6c63 756c  ** of the calcul
-00001380: 6174 696f 6e20 7072 6f63 6573 7320 7374  ation process st
-00001390: 6570 2062 7920 7374 6570 2e20 4974 2068  ep by step. It h
-000013a0: 656c 7073 2074 6f20 6964 656e 7469 6679  elps to identify
-000013b0: 2074 6865 2063 6175 7365 206f 6620 7468   the cause of th
-000013c0: 6520 6661 696c 7572 652e 0a2a 202a 2a4f  e failure..* **O
-000013d0: 524d 2061 6363 6573 732a 2a20 696e 7369  RM access** insi
-000013e0: 6465 2074 6865 2074 6573 742e 2059 6f75  de the test. You
-000013f0: 2068 6176 6520 6675 6c6c 2061 6363 6573   have full acces
-00001400: 7320 746f 2074 6865 202a 2a64 6576 6963  s to the **devic
-00001410: 652a 2a20 7072 6f70 6572 7469 6573 2e20  e** properties. 
-00001420: 466f 7220 696e 7374 616e 6365 2c20 796f  For instance, yo
-00001430: 7520 6d61 7920 6c65 7665 7261 6765 205b  u may leverage [
-00001440: 436f 6e66 6967 7572 6174 696f 6e20 436f  Configuration Co
-00001450: 6e74 6578 7473 5d28 6874 7470 733a 2f2f  ntexts](https://
-00001460: 646f 6373 2e6e 6574 626f 782e 6465 762f  docs.netbox.dev/
-00001470: 656e 2f73 7461 626c 652f 6665 6174 7572  en/stable/featur
-00001480: 6573 2f63 6f6e 7465 7874 2d64 6174 612f  es/context-data/
-00001490: 2920 4e65 7442 6f78 2066 6561 7475 7265  ) NetBox feature
-000014a0: 2074 6f20 7374 6f72 6520 796f 7572 2064   to store your d
-000014b0: 6573 6972 6564 2063 6f6e 6669 6775 7261  esired configura
-000014c0: 7469 6f6e 2061 6e64 2063 6f6d 7061 7265  tion and compare
-000014d0: 2069 7420 7769 7468 2074 6865 2063 6f6e   it with the con
-000014e0: 6669 6720 636f 6c6c 6563 7465 6420 6672  fig collected fr
-000014f0: 6f6d 2074 6865 2064 6576 6963 652e 0a2a  om the device..*
-00001500: 202a 2a52 6570 6f72 7473 2061 6e64 2077   **Reports and w
-00001510: 6562 686f 6f6b 732a 2a2e 2041 6674 6572  ebhooks**. After
-00001520: 2065 7865 6375 7469 6f6e 206f 6620 736f   execution of so
-00001530: 6d65 2062 756e 6368 206f 6620 7465 7374  me bunch of test
-00001540: 7320 796f 7520 6361 6e20 6765 7420 7468  s you can get th
-00001550: 6520 7265 706f 7274 2077 6974 6820 7061  e report with pa
-00001560: 7373 6564 2f66 6169 6c65 6420 7374 6174  ssed/failed stat
-00001570: 6973 7469 6373 2067 726f 7570 6564 2062  istics grouped b
-00001580: 7920 736f 6d65 204c 6f63 6174 696f 6e2f  y some Location/
-00001590: 5369 7465 2f4d 616e 7566 6163 7475 7265  Site/Manufacture
-000015a0: 722f 6574 632e 204d 6f72 656f 7665 722c  r/etc. Moreover,
-000015b0: 2079 6f75 2063 616e 2070 726f 7669 7369   you can provisi
-000015c0: 6f6e 2074 6865 2077 6562 686f 6f6b 2074  on the webhook t
-000015d0: 6f20 6e6f 7469 6679 2061 6e20 6578 7465  o notify an exte
-000015e0: 726e 616c 2073 7973 7465 6d20 7768 656e  rnal system when
-000015f0: 2063 6f6d 706c 6961 6e63 6520 7265 706f   compliance repo
-00001600: 7274 2069 7320 6765 6e65 7261 7465 642e  rt is generated.
-00001610: 0a2a 202a 2a54 6573 7420 6578 7465 6e73  .* **Test extens
-00001620: 6962 696c 6974 792a 2a2e 2059 6f75 2063  ibility**. You c
-00001630: 616e 2064 6566 696e 6520 796f 7572 206f  an define your o
-00001640: 776e 2070 7974 686f 6e20 6675 6e63 7469  wn python functi
-00001650: 6f6e 7320 6f72 2063 6c61 7373 6573 2074  ons or classes t
-00001660: 6f20 7265 7573 6520 7468 6520 636f 6465  o reuse the code
-00001670: 2062 6574 7765 656e 206d 756c 7469 706c   between multipl
-00001680: 6520 636f 6d70 6c69 616e 6365 2074 6573  e compliance tes
-00001690: 7473 2e0a 2a20 506f 7373 6962 696c 6974  ts..* Possibilit
-000016a0: 7920 746f 2073 746f 7265 2061 6c6c 2068  y to store all h
-000016b0: 6561 7679 2074 6578 742d 6261 7365 6420  eavy text-based 
-000016c0: 656e 7469 7469 6573 2028 6c69 6b65 2063  entities (like c
-000016d0: 6f6d 706c 6961 6e63 6520 7465 7374 7320  ompliance tests 
-000016e0: 6f72 2054 5450 2054 656d 706c 6174 6573  or TTP Templates
-000016f0: 2920 696e 2061 202a 2a47 6974 2072 6570  ) in a **Git rep
-00001700: 6f73 6974 6f72 792a 2a0a 3c21 2d2d 6d6b  ository**.<!--mk
-00001710: 646f 6373 2d65 6e64 2d2d 3e0a 0a23 2320  docs-end-->..## 
-00001720: 446f 6375 6d65 6e74 6174 696f 6e0a 5265  Documentation.Re
-00001730: 6164 2074 6865 2066 756c 6c20 646f 6375  ad the full docu
-00001740: 6d65 6e74 6174 696f 6e20 6f6e 205b 7661  mentation on [va
-00001750: 6c69 6469 7479 2e72 6561 6474 6865 646f  lidity.readthedo
-00001760: 6373 2e69 6f5d 2868 7474 7073 3a2f 2f76  cs.io](https://v
-00001770: 616c 6964 6974 792e 7265 6164 7468 6564  alidity.readthed
-00001780: 6f63 732e 696f 290a 0a0a 2323 2051 7569  ocs.io)...## Qui
-00001790: 636b 2053 7461 7274 0a0a 5468 6520 7368  ck Start..The sh
-000017a0: 6f72 7420 7669 6465 6f20 6162 6f75 7420  ort video about 
-000017b0: 6669 7273 7420 7374 6570 7320 7769 7468  first steps with
-000017c0: 2056 616c 6964 6974 793a 0a0a 5b21 5b57   Validity:..[![W
-000017d0: 6174 6368 2074 6865 2076 6964 656f 5d28  atch the video](
-000017e0: 6874 7470 733a 2f2f 696d 672e 796f 7574  https://img.yout
-000017f0: 7562 652e 636f 6d2f 7669 2f48 7332 4955  ube.com/vi/Hs2IU
-00001800: 4536 724b 4334 2f30 2e6a 7067 295d 2868  E6rKC4/0.jpg)](h
-00001810: 7474 7073 3a2f 2f79 6f75 7475 2e62 652f  ttps://youtu.be/
-00001820: 4873 3249 5545 3672 4b43 3429 0a0a 2323  Hs2IUE6rKC4)..##
-00001830: 2043 6f6e 7472 6962 7574 696e 670a 0a46   Contributing..F
-00001840: 6565 6c20 6672 6565 2074 6f20 6173 6b20  eel free to ask 
-00001850: 6120 5b51 7565 7374 696f 6e5d 2868 7474  a [Question](htt
-00001860: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00001870: 616d 7961 736e 696b 6f76 2f76 616c 6964  amyasnikov/valid
-00001880: 6974 792f 6469 7363 7573 7369 6f6e 7329  ity/discussions)
-00001890: 2c20 7265 706f 7274 2061 6e20 5b49 7373  , report an [Iss
-000018a0: 7565 5d28 6874 7470 733a 2f2f 6769 7468  ue](https://gith
-000018b0: 7562 2e63 6f6d 2f61 6d79 6173 6e69 6b6f  ub.com/amyasniko
-000018c0: 762f 7661 6c69 6469 7479 2f69 7373 7565  v/validity/issue
-000018d0: 7329 206f 7220 6576 656e 206d 616b 6520  s) or even make 
-000018e0: 6120 5b50 525d 2843 4f4e 5452 4942 5554  a [PR](CONTRIBUT
-000018f0: 494e 472e 6d64 292e 2052 6561 6420 6d6f  ING.md). Read mo
-00001900: 7265 2061 626f 7574 2063 6f6e 7472 6962  re about contrib
-00001910: 7574 696f 6e20 696e 2074 6865 205b 434f  ution in the [CO
-00001920: 4e54 5249 4255 5449 4e47 5d28 434f 4e54  NTRIBUTING](CONT
-00001930: 5249 4255 5449 4e47 2e6d 6429 2067 7569  RIBUTING.md) gui
-00001940: 6465 2e0a                                de..
+000008f0: 0a0a 3c64 6976 2061 6c69 676e 3d22 6365  ..<div align="ce
+00000900: 6e74 6572 223e 0a20 2020 203c 6120 6872  nter">.    <a hr
+00000910: 6566 3d22 6874 7470 733a 2f2f 7661 6c69  ef="https://vali
+00000920: 6469 7479 2e72 6561 6474 6865 646f 6373  dity.readthedocs
+00000930: 2e69 6f22 3e3c 696d 6720 7372 633d 2268  .io"><img src="h
+00000940: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
+00000950: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
+00000960: 2f61 6d79 6173 6e69 6b6f 762f 7661 6c69  /amyasnikov/vali
+00000970: 6469 7479 2f6d 6173 7465 722f 646f 6373  dity/master/docs
+00000980: 2f76 616c 6964 6974 795f 6c6f 676f 2e70  /validity_logo.p
+00000990: 6e67 2220 616c 743d 2243 6c69 636b 2074  ng" alt="Click t
+000009a0: 6f20 7669 6577 2056 616c 6964 6974 7920  o view Validity 
+000009b0: 646f 6373 222f 3e3c 2f61 3e0a 2020 2020  docs"/></a>.    
+000009c0: 3c68 313e 5661 6c69 6469 7479 3a20 7665  <h1>Validity: ve
+000009d0: 6e64 6f72 2d61 676e 6f73 7469 6320 636f  ndor-agnostic co
+000009e0: 6e66 6967 7572 6174 696f 6e20 636f 6d70  nfiguration comp
+000009f0: 6c69 616e 6365 3c2f 6831 3e0a 2020 2020  liance</h1>.    
+00000a00: 3c70 3e0a 2020 2020 2020 2020 3c69 6d67  <p>.        <img
+00000a10: 2073 7263 3d22 6874 7470 733a 2f2f 6769   src="https://gi
+00000a20: 7468 7562 2e63 6f6d 2f61 6d79 6173 6e69  thub.com/amyasni
+00000a30: 6b6f 762f 7661 6c69 6469 7479 2f61 6374  kov/validity/act
+00000a40: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f63  ions/workflows/c
+00000a50: 692e 796d 6c2f 6261 6467 652e 7376 6722  i.yml/badge.svg"
+00000a60: 2061 6c74 3d22 4349 223e 0a20 2020 2020   alt="CI">.     
+00000a70: 2020 203c 696d 6720 7372 633d 2268 7474     <img src="htt
+00000a80: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00000a90: 2e69 6f2f 656e 6470 6f69 6e74 3f75 726c  .io/endpoint?url
+00000aa0: 3d68 7474 7073 3a2f 2f67 6973 742e 6769  =https://gist.gi
+00000ab0: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
+00000ac0: 636f 6d2f 616d 7961 736e 696b 6f76 2f39  com/amyasnikov/9
+00000ad0: 6535 3138 6165 3862 6162 6431 3862 3765  e518ae8babd18b7e
+00000ae0: 6464 3865 6535 6161 6435 3831 3436 622f  dd8ee5aad58146b/
+00000af0: 7261 772f 636f 762e 6a73 6f6e 2220 616c  raw/cov.json" al
+00000b00: 743d 2243 6f76 6572 6167 6522 3e0a 2020  t="Coverage">.  
+00000b10: 2020 2020 2020 3c69 6d67 2073 7263 3d22        <img src="
+00000b20: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000b30: 6c64 732e 696f 2f62 6164 6765 2f50 7974  lds.io/badge/Pyt
+00000b40: 686f 6e2d 332e 3130 2b2d 626c 7565 2e73  hon-3.10+-blue.s
+00000b50: 7667 2220 616c 743d 2250 7974 686f 6e20  vg" alt="Python 
+00000b60: 7665 7273 696f 6e22 3e0a 2020 2020 2020  version">.      
+00000b70: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
+00000b80: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000b90: 696f 2f62 6164 6765 2f4e 6574 426f 782d  io/badge/NetBox-
+00000ba0: 332e 347c 332e 352d 626c 7565 2e73 7667  3.4|3.5-blue.svg
+00000bb0: 2220 616c 743d 224e 6574 426f 7820 7665  " alt="NetBox ve
+00000bc0: 7273 696f 6e22 3e0a 2020 2020 3c2f 703e  rsion">.    </p>
+00000bd0: 0a3c 2f64 6976 3e0a 0a3c 212d 2d6d 6b64  .</div>..<!--mkd
+00000be0: 6f63 732d 7374 6172 742d 2d3e 0a23 2320  ocs-start-->.## 
+00000bf0: 5768 6174 3f0a 5661 6c69 6469 7479 2069  What?.Validity i
+00000c00: 7320 7468 6520 5b4e 6574 426f 785d 2868  s the [NetBox](h
+00000c10: 7474 7073 3a2f 2f6e 6574 626f 782e 6465  ttps://netbox.de
+00000c20: 7629 2070 6c75 6769 6e20 746f 2077 7269  v) plugin to wri
+00000c30: 7465 2022 6175 746f 2074 6573 7473 2220  te "auto tests" 
+00000c40: 666f 7220 636f 6e66 6967 7572 6174 696f  for configuratio
+00000c50: 6e2e 2059 6f75 2064 6566 696e 6520 636f  n. You define co
+00000c60: 6d70 6c69 616e 6365 2074 6573 7473 2061  mpliance tests a
+00000c70: 6e64 2056 616c 6964 6974 7920 6368 6563  nd Validity chec
+00000c80: 6b73 206e 6574 776f 726b 2064 6576 6963  ks network devic
+00000c90: 6520 636f 6e66 6967 7572 6174 696f 6e20  e configuration 
+00000ca0: 6669 6c65 7320 6167 6169 6e73 7420 7468  files against th
+00000cb0: 6573 6520 7465 7374 732e 2041 7320 6120  ese tests. As a 
+00000cc0: 7265 7375 6c74 2079 6f75 2063 616e 2066  result you can f
+00000cd0: 696e 6420 6f75 7420 7768 6963 6820 6465  ind out which de
+00000ce0: 7669 6365 7320 6172 6520 7072 6f76 6973  vices are provis
+00000cf0: 696f 6e65 6420 7072 6f70 6572 6c79 2028  ioned properly (
+00000d00: 6163 636f 7264 696e 6720 746f 2074 6865  according to the
+00000d10: 2074 6573 7473 2079 6f75 2068 6176 6520   tests you have 
+00000d20: 7772 6974 7465 6e29 2061 6e64 2077 6869  written) and whi
+00000d30: 6368 2061 7265 206e 6f74 2e0a 0a54 6f20  ch are not...To 
+00000d40: 7573 6520 7661 6c69 6469 7479 2079 6f75  use validity you
+00000d50: 206e 6565 643a 0a0a 312e 2053 746f 7265   need:..1. Store
+00000d60: 2063 6f6e 6669 6775 7261 7469 6f6e 2066   configuration f
+00000d70: 696c 6573 206f 6620 796f 7572 2064 6576  iles of your dev
+00000d80: 6963 6573 2069 6e20 6120 4769 7420 7265  ices in a Git re
+00000d90: 706f 7369 746f 7279 2e20 5661 6c69 6469  pository. Validi
+00000da0: 7479 2064 6f65 7320 6e6f 7420 636f 6c6c  ty does not coll
+00000db0: 6563 7420 7468 6520 636f 6e66 6967 7320  ect the configs 
+00000dc0: 6672 6f6d 2079 6f75 7220 6e65 7477 6f72  from your networ
+00000dd0: 6b2c 2079 6f75 2068 6176 6520 746f 2064  k, you have to d
+00000de0: 6f20 6974 2062 7920 7468 6972 642d 7061  o it by third-pa
+00000df0: 7274 7920 746f 6f6c 2028 652e 672e 205b  rty tool (e.g. [
+00000e00: 6f78 6964 697a 6564 5d28 6874 7470 733a  oxidized](https:
+00000e10: 2f2f 6769 7468 7562 2e63 6f6d 2f79 7474  //github.com/ytt
+00000e20: 692f 6f78 6964 697a 6564 2929 2e0a 0a32  i/oxidized))...2
+00000e30: 2e20 4465 6669 6e65 205b 5454 5020 5465  . Define [TTP Te
+00000e40: 6d70 6c61 7465 5d28 6874 7470 733a 2f2f  mplate](https://
+00000e50: 7474 702e 7265 6164 7468 6564 6f63 732e  ttp.readthedocs.
+00000e60: 696f 2f65 6e2f 6c61 7465 7374 2f29 2074  io/en/latest/) t
+00000e70: 6f20 7472 616e 736c 6174 6520 7468 6520  o translate the 
+00000e80: 636f 6e66 6967 2066 726f 6d20 7665 6e64  config from vend
+00000e90: 6f72 2073 7065 6369 6669 6320 666f 726d  or specific form
+00000ea0: 6174 2069 6e74 6f20 4a53 4f4e 2e0a 0a33  at into JSON...3
+00000eb0: 2e20 5772 6974 6520 636f 6d70 6c69 616e  . Write complian
+00000ec0: 6365 2074 6573 7420 6173 2061 2070 7974  ce test as a pyt
+00000ed0: 686f 6e20 6578 7072 6573 7369 6f6e 2c20  hon expression, 
+00000ee0: 652e 672e 3c62 722f 3e0a 6064 6576 6963  e.g.<br/>.`devic
+00000ef0: 652e 636f 6e66 6967 5b22 6e74 702d 7365  e.config["ntp-se
+00000f00: 7276 6572 7322 5d20 3d3d 205b 2231 2e32  rvers"] == ["1.2
+00000f10: 2e33 2e34 222c 2022 352e 362e 372e 3822  .3.4", "5.6.7.8"
+00000f20: 5d60 0a0a 342e 2041 7070 6c79 2063 7265  ]`..4. Apply cre
+00000f30: 6174 6564 2074 6573 7420 746f 2073 7065  ated test to spe
+00000f40: 6369 6669 6320 6465 7669 6365 7320 616e  cific devices an
+00000f50: 6420 6765 7420 7468 6520 7265 7375 6c74  d get the result
+00000f60: 7320 7065 7220 6465 7669 6365 2028 7061  s per device (pa
+00000f70: 7373 6564 206f 7220 6661 696c 6564 292e  ssed or failed).
+00000f80: 0a0a 0a23 2320 5768 793f 0a43 6f6e 6669  ...## Why?.Confi
+00000f90: 6775 7261 7469 6f6e 2063 6f6d 706c 6961  guration complia
+00000fa0: 6e63 6520 6973 206f 6e65 206f 6620 7468  nce is one of th
+00000fb0: 6520 7665 7279 2063 6f6d 6d6f 6e20 7072  e very common pr
+00000fc0: 6f62 6c65 6d73 2074 6861 7420 6172 6973  oblems that aris
+00000fd0: 6573 2069 6e20 6576 6572 7920 636f 6d70  es in every comp
+00000fe0: 616e 7920 7769 7468 2074 6865 2067 726f  any with the gro
+00000ff0: 7774 6820 6f66 2074 6865 6972 206e 6574  wth of their net
+00001000: 776f 726b 2e20 5573 7561 6c6c 7920 636f  work. Usually co
+00001010: 6d70 616e 6965 7320 736f 6c76 6520 7468  mpanies solve th
+00001020: 6973 2070 726f 626c 656d 2077 6974 6820  is problem with 
+00001030: 736f 6d65 206b 696e 6420 6f66 2073 6372  some kind of scr
+00001040: 6970 7473 2074 6861 7420 646f 2061 6c6c  ipts that do all
+00001050: 2074 6865 2074 6869 6e67 7320 6174 2074   the things at t
+00001060: 6865 2073 616d 6520 7469 6d65 3a20 7468  he same time: th
+00001070: 6579 2070 6172 7365 2063 6f6e 6669 6773  ey parse configs
+00001080: 2c20 6170 706c 7920 736f 6d65 2063 6f6d  , apply some com
+00001090: 706c 6961 6e63 6520 6c6f 6769 6320 616e  pliance logic an
+000010a0: 6420 7075 7368 2074 6865 2072 6573 756c  d push the resul
+000010b0: 7473 2069 6e74 6f20 736f 6d65 2044 4220  ts into some DB 
+000010c0: 6f72 2074 6869 7264 2d70 6172 7479 204f  or third-party O
+000010d0: 5353 2073 7973 7465 6d2e 2055 7375 616c  SS system. Usual
+000010e0: 6c79 2061 6674 6572 2074 6865 2061 6464  ly after the add
+000010f0: 6974 696f 6e20 6f66 2073 6576 6572 616c  ition of several
+00001100: 2076 656e 646f 7273 2028 6f72 2065 7665   vendors (or eve
+00001110: 6e20 7365 7665 7261 6c20 736f 6674 7761  n several softwa
+00001120: 7265 2072 6576 6973 696f 6e73 206f 6620  re revisions of 
+00001130: 6f6e 6520 6d6f 6465 6c29 2074 6865 7365  one model) these
+00001140: 2073 6372 6970 7473 2062 6563 6f6d 6520   scripts become 
+00001150: 756e 7265 6164 6162 6c65 2061 6e64 2061  unreadable and a
+00001160: 6c6d 6f73 7420 6e6f 206f 6e65 2063 616e  lmost no one can
+00001170: 2064 6566 696e 6974 656c 7920 7361 7920   definitely say 
+00001180: 7768 6963 6820 7275 6c65 7320 7468 6520  which rules the 
+00001190: 7363 7269 7074 2063 6865 636b 7320 666f  script checks fo
+000011a0: 722e 0a0a 5661 6c69 6469 7479 2063 6f6d  r...Validity com
+000011b0: 706c 6574 656c 7920 7365 7061 7261 7465  pletely separate
+000011c0: 7320 636f 6d70 6c69 616e 6365 2074 6573  s compliance tes
+000011d0: 7420 636f 6465 2066 726f 6d20 616c 6c20  t code from all 
+000011e0: 6f74 6865 7220 7468 696e 6773 206c 696b  other things lik
+000011f0: 6520 636f 6e66 6967 2073 6572 6961 6c69  e config seriali
+00001200: 7a61 7469 6f6e 2e20 5468 6973 206f 6e65  zation. This one
+00001210: 2065 6e63 6f75 7261 6765 7320 796f 7520   encourages you 
+00001220: 746f 2077 7269 7465 2073 686f 7274 2c20  to write short, 
+00001230: 636c 6561 6e20 616e 6420 756e 6465 7273  clean and unders
+00001240: 7461 6e64 6162 6c65 2063 6f6d 706c 6961  tandable complia
+00001250: 6e63 6520 7465 7374 7320 746f 6765 7468  nce tests togeth
+00001260: 6572 2077 6974 6820 7468 6520 6d61 6e64  er with the mand
+00001270: 6174 6f72 7920 6465 7363 7269 7074 696f  atory descriptio
+00001280: 6e2e 0a0a 0a23 2320 4b65 7920 4665 6174  n....## Key Feat
+00001290: 7572 6573 0a2a 2054 7275 6c79 2076 656e  ures.* Truly ven
+000012a0: 646f 722d 6167 6e6f 7374 6963 2e20 596f  dor-agnostic. Yo
+000012b0: 7520 6361 6e20 6561 7369 6c79 2069 6e74  u can easily int
+000012c0: 6567 7261 7465 2061 6e79 2076 656e 646f  egrate any vendo
+000012d0: 7220 636f 6e66 6967 2066 6f72 6d61 7420  r config format 
+000012e0: 7573 696e 6720 5b54 5450 5d28 6874 7470  using [TTP](http
+000012f0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f64  s://github.com/d
+00001300: 6d75 6c79 616c 696e 2f74 7470 290a 2a20  mulyalin/ttp).* 
+00001310: 5772 6974 696e 6720 636f 6d70 6c69 616e  Writing complian
+00001320: 6365 2074 6573 7473 2075 7369 6e67 2050  ce tests using P
+00001330: 7974 686f 6e20 6578 7072 6573 7369 6f6e  ython expression
+00001340: 7320 616e 6420 5b4a 515d 2868 7474 7073  s and [JQ](https
+00001350: 3a2f 2f73 7465 646f 6c61 6e2e 6769 7468  ://stedolan.gith
+00001360: 7562 2e69 6f2f 6a71 2f6d 616e 7561 6c2f  ub.io/jq/manual/
+00001370: 290a 2a20 466c 6578 6962 6c65 2073 656c  ).* Flexible sel
+00001380: 6563 746f 7220 7379 7374 656d 2074 6f20  ector system to 
+00001390: 6170 706c 7920 7468 6520 7465 7374 7320  apply the tests 
+000013a0: 6f6e 6c79 2074 6f20 6120 7370 6563 6966  only to a specif
+000013b0: 6963 2073 7562 7365 7420 6f66 2064 6576  ic subset of dev
+000013c0: 6963 6573 0a2a 2043 6f6e 6365 7074 206f  ices.* Concept o
+000013d0: 6620 2a2a 6479 6e61 6d69 6320 7061 6972  f **dynamic pair
+000013e0: 732a 2a2e 2057 6974 6820 6479 6e61 6d69  s**. With dynami
+000013f0: 6320 7061 6972 2079 6f75 2063 616e 2063  c pair you can c
+00001400: 6f6d 7061 7265 2032 2064 6966 6665 7265  ompare 2 differe
+00001410: 6e74 2064 6576 6963 6573 2062 6574 7765  nt devices betwe
+00001420: 656e 2065 6163 6820 6f74 6865 7220 2865  en each other (e
+00001430: 2e67 2e20 636f 6d70 6172 6520 7468 6520  .g. compare the 
+00001440: 636f 6e66 6967 7572 6174 696f 6e20 6f66  configuration of
+00001450: 2032 204d 432d 4c41 4720 6d65 6d62 6572   2 MC-LAG member
+00001460: 7329 2e0a 2a20 2a2a 5465 7374 2072 6573  s)..* **Test res
+00001470: 756c 7420 6578 706c 616e 6174 696f 6e2a  ult explanation*
+00001480: 2a2e 2057 6865 6e20 736f 6d65 2074 6573  *. When some tes
+00001490: 7420 6661 696c 732c 2079 6f75 2063 616e  t fails, you can
+000014a0: 2067 6574 2074 6865 202a 2a65 7870 6c61   get the **expla
+000014b0: 6e61 7469 6f6e 2a2a 206f 6620 7468 6520  nation** of the 
+000014c0: 6361 6c63 756c 6174 696f 6e20 7072 6f63  calculation proc
+000014d0: 6573 7320 7374 6570 2062 7920 7374 6570  ess step by step
+000014e0: 2e20 4974 2068 656c 7073 2074 6f20 6964  . It helps to id
+000014f0: 656e 7469 6679 2074 6865 2063 6175 7365  entify the cause
+00001500: 206f 6620 7468 6520 6661 696c 7572 652e   of the failure.
+00001510: 0a2a 202a 2a4f 524d 2061 6363 6573 732a  .* **ORM access*
+00001520: 2a20 696e 7369 6465 2074 6865 2074 6573  * inside the tes
+00001530: 742e 2059 6f75 2068 6176 6520 6675 6c6c  t. You have full
+00001540: 2061 6363 6573 7320 746f 2074 6865 202a   access to the *
+00001550: 2a64 6576 6963 652a 2a20 7072 6f70 6572  *device** proper
+00001560: 7469 6573 2e20 466f 7220 696e 7374 616e  ties. For instan
+00001570: 6365 2c20 796f 7520 6d61 7920 6c65 7665  ce, you may leve
+00001580: 7261 6765 205b 436f 6e66 6967 7572 6174  rage [Configurat
+00001590: 696f 6e20 436f 6e74 6578 7473 5d28 6874  ion Contexts](ht
+000015a0: 7470 733a 2f2f 646f 6373 2e6e 6574 626f  tps://docs.netbo
+000015b0: 782e 6465 762f 656e 2f73 7461 626c 652f  x.dev/en/stable/
+000015c0: 6665 6174 7572 6573 2f63 6f6e 7465 7874  features/context
+000015d0: 2d64 6174 612f 2920 4e65 7442 6f78 2066  -data/) NetBox f
+000015e0: 6561 7475 7265 2074 6f20 7374 6f72 6520  eature to store 
+000015f0: 796f 7572 2064 6573 6972 6564 2063 6f6e  your desired con
+00001600: 6669 6775 7261 7469 6f6e 2061 6e64 2063  figuration and c
+00001610: 6f6d 7061 7265 2069 7420 7769 7468 2074  ompare it with t
+00001620: 6865 2063 6f6e 6669 6720 636f 6c6c 6563  he config collec
+00001630: 7465 6420 6672 6f6d 2074 6865 2064 6576  ted from the dev
+00001640: 6963 652e 0a2a 202a 2a52 6570 6f72 7473  ice..* **Reports
+00001650: 2061 6e64 2077 6562 686f 6f6b 732a 2a2e   and webhooks**.
+00001660: 2041 6674 6572 2065 7865 6375 7469 6f6e   After execution
+00001670: 206f 6620 736f 6d65 2062 756e 6368 206f   of some bunch o
+00001680: 6620 7465 7374 7320 796f 7520 6361 6e20  f tests you can 
+00001690: 6765 7420 7468 6520 7265 706f 7274 2077  get the report w
+000016a0: 6974 6820 7061 7373 6564 2f66 6169 6c65  ith passed/faile
+000016b0: 6420 7374 6174 6973 7469 6373 2067 726f  d statistics gro
+000016c0: 7570 6564 2062 7920 736f 6d65 204c 6f63  uped by some Loc
+000016d0: 6174 696f 6e2f 5369 7465 2f4d 616e 7566  ation/Site/Manuf
+000016e0: 6163 7475 7265 722f 6574 632e 204d 6f72  acturer/etc. Mor
+000016f0: 656f 7665 722c 2079 6f75 2063 616e 2070  eover, you can p
+00001700: 726f 7669 7369 6f6e 2074 6865 2077 6562  rovision the web
+00001710: 686f 6f6b 2074 6f20 6e6f 7469 6679 2061  hook to notify a
+00001720: 6e20 6578 7465 726e 616c 2073 7973 7465  n external syste
+00001730: 6d20 7768 656e 2063 6f6d 706c 6961 6e63  m when complianc
+00001740: 6520 7265 706f 7274 2069 7320 6765 6e65  e report is gene
+00001750: 7261 7465 642e 0a2a 202a 2a54 6573 7420  rated..* **Test 
+00001760: 6578 7465 6e73 6962 696c 6974 792a 2a2e  extensibility**.
+00001770: 2059 6f75 2063 616e 2064 6566 696e 6520   You can define 
+00001780: 796f 7572 206f 776e 2070 7974 686f 6e20  your own python 
+00001790: 6675 6e63 7469 6f6e 7320 6f72 2063 6c61  functions or cla
+000017a0: 7373 6573 2074 6f20 7265 7573 6520 7468  sses to reuse th
+000017b0: 6520 636f 6465 2062 6574 7765 656e 206d  e code between m
+000017c0: 756c 7469 706c 6520 636f 6d70 6c69 616e  ultiple complian
+000017d0: 6365 2074 6573 7473 2e0a 2a20 506f 7373  ce tests..* Poss
+000017e0: 6962 696c 6974 7920 746f 2073 746f 7265  ibility to store
+000017f0: 2061 6c6c 2068 6561 7679 2074 6578 742d   all heavy text-
+00001800: 6261 7365 6420 656e 7469 7469 6573 2028  based entities (
+00001810: 6c69 6b65 2063 6f6d 706c 6961 6e63 6520  like compliance 
+00001820: 7465 7374 7320 6f72 2054 5450 2054 656d  tests or TTP Tem
+00001830: 706c 6174 6573 2920 696e 2061 202a 2a47  plates) in a **G
+00001840: 6974 2072 6570 6f73 6974 6f72 792a 2a0a  it repository**.
+00001850: 0a23 2320 446f 776e 6c6f 6164 2061 6e64  .## Download and
+00001860: 2049 6e73 7461 6c6c 0a0a 596f 7520 6361   Install..You ca
+00001870: 6e20 646f 776e 6c6f 6164 2056 616c 6964  n download Valid
+00001880: 6974 7920 7669 6120 2a2a 7069 702a 2a0a  ity via **pip**.
+00001890: 6060 600a 7069 7020 696e 7374 616c 6c20  ```.pip install 
+000018a0: 6e65 7462 6f78 2d76 616c 6964 6974 790a  netbox-validity.
+000018b0: 6060 600a 4166 7465 7220 7468 6174 2066  ```.After that f
+000018c0: 6f6c 6c6f 7720 7468 6520 5b69 6e73 7461  ollow the [insta
+000018d0: 6c6c 6174 696f 6e20 6775 6964 655d 2868  llation guide](h
+000018e0: 7474 7073 3a2f 2f76 616c 6964 6974 792e  ttps://validity.
+000018f0: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
+00001900: 6e2f 6c61 7465 7374 2f69 6e73 7461 6c6c  n/latest/install
+00001910: 6174 696f 6e2f 2920 746f 2063 6f72 7265  ation/) to corre
+00001920: 6374 6c79 2061 6464 2056 616c 6964 6974  ctly add Validit
+00001930: 7920 746f 2079 6f75 7220 4e65 7442 6f78  y to your NetBox
+00001940: 2e0a 3c21 2d2d 6d6b 646f 6373 2d65 6e64  ..<!--mkdocs-end
+00001950: 2d2d 3e0a 0a23 2320 446f 6375 6d65 6e74  -->..## Document
+00001960: 6174 696f 6e0a 5265 6164 2074 6865 2066  ation.Read the f
+00001970: 756c 6c20 646f 6375 6d65 6e74 6174 696f  ull documentatio
+00001980: 6e20 6f6e 205b 7661 6c69 6469 7479 2e72  n on [validity.r
+00001990: 6561 6474 6865 646f 6373 2e69 6f5d 2868  eadthedocs.io](h
+000019a0: 7474 7073 3a2f 2f76 616c 6964 6974 792e  ttps://validity.
+000019b0: 7265 6164 7468 6564 6f63 732e 696f 290a  readthedocs.io).
+000019c0: 0a0a 2323 2051 7569 636b 2053 7461 7274  ..## Quick Start
+000019d0: 0a0a 5468 6520 7368 6f72 7420 7669 6465  ..The short vide
+000019e0: 6f20 6162 6f75 7420 6669 7273 7420 7374  o about first st
+000019f0: 6570 7320 7769 7468 2056 616c 6964 6974  eps with Validit
+00001a00: 793a 0a0a 5b21 5b57 6174 6368 2074 6865  y:..[![Watch the
+00001a10: 2076 6964 656f 5d28 6874 7470 733a 2f2f   video](https://
+00001a20: 696d 672e 796f 7574 7562 652e 636f 6d2f  img.youtube.com/
+00001a30: 7669 2f48 7332 4955 4536 724b 4334 2f30  vi/Hs2IUE6rKC4/0
+00001a40: 2e6a 7067 295d 2868 7474 7073 3a2f 2f79  .jpg)](https://y
+00001a50: 6f75 7475 2e62 652f 4873 3249 5545 3672  outu.be/Hs2IUE6r
+00001a60: 4b43 3429 0a0a 2323 2043 6f6e 7472 6962  KC4)..## Contrib
+00001a70: 7574 696e 670a 0a46 6565 6c20 6672 6565  uting..Feel free
+00001a80: 2074 6f20 6173 6b20 6120 5b51 7565 7374   to ask a [Quest
+00001a90: 696f 6e5d 2868 7474 7073 3a2f 2f67 6974  ion](https://git
+00001aa0: 6875 622e 636f 6d2f 616d 7961 736e 696b  hub.com/amyasnik
+00001ab0: 6f76 2f76 616c 6964 6974 792f 6469 7363  ov/validity/disc
+00001ac0: 7573 7369 6f6e 7329 2c20 7265 706f 7274  ussions), report
+00001ad0: 2061 6e20 5b49 7373 7565 5d28 6874 7470   an [Issue](http
+00001ae0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f61  s://github.com/a
+00001af0: 6d79 6173 6e69 6b6f 762f 7661 6c69 6469  myasnikov/validi
+00001b00: 7479 2f69 7373 7565 7329 206f 7220 6576  ty/issues) or ev
+00001b10: 656e 206d 616b 6520 6120 5b50 525d 2843  en make a [PR](C
+00001b20: 4f4e 5452 4942 5554 494e 472e 6d64 292e  ONTRIBUTING.md).
+00001b30: 2052 6561 6420 6d6f 7265 2061 626f 7574   Read more about
+00001b40: 2063 6f6e 7472 6962 7574 696f 6e20 696e   contribution in
+00001b50: 2074 6865 205b 434f 4e54 5249 4255 5449   the [CONTRIBUTI
+00001b60: 4e47 5d28 434f 4e54 5249 4255 5449 4e47  NG](CONTRIBUTING
+00001b70: 2e6d 6429 2067 7569 6465 2e0a            .md) guide..
```

### Comparing `netbox-validity-1.2.0/README.md` & `netbox-validity-1.2.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,262 +1,297 @@
-00000000: 2320 5661 6c69 6469 7479 3a20 7665 6e64  # Validity: vend
-00000010: 6f72 2d61 676e 6f73 7469 6320 636f 6e66  or-agnostic conf
-00000020: 6967 7572 6174 696f 6e20 636f 6d70 6c69  iguration compli
-00000030: 616e 6365 0a0a 215b 4349 5d28 6874 7470  ance..![CI](http
-00000040: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f61  s://github.com/a
-00000050: 6d79 6173 6e69 6b6f 762f 7661 6c69 6469  myasnikov/validi
-00000060: 7479 2f61 6374 696f 6e73 2f77 6f72 6b66  ty/actions/workf
-00000070: 6c6f 7773 2f63 692e 796d 6c2f 6261 6467  lows/ci.yml/badg
-00000080: 652e 7376 6729 0a21 5b43 6f76 6572 6167  e.svg).![Coverag
-00000090: 655d 2868 7474 7073 3a2f 2f69 6d67 2e73  e](https://img.s
-000000a0: 6869 656c 6473 2e69 6f2f 656e 6470 6f69  hields.io/endpoi
-000000b0: 6e74 3f75 726c 3d68 7474 7073 3a2f 2f67  nt?url=https://g
-000000c0: 6973 742e 6769 7468 7562 7573 6572 636f  ist.githubuserco
-000000d0: 6e74 656e 742e 636f 6d2f 616d 7961 736e  ntent.com/amyasn
-000000e0: 696b 6f76 2f39 6535 3138 6165 3862 6162  ikov/9e518ae8bab
-000000f0: 6431 3862 3765 6464 3865 6535 6161 6435  d18b7edd8ee5aad5
-00000100: 3831 3436 622f 7261 772f 636f 762e 6a73  8146b/raw/cov.js
-00000110: 6f6e 290a 215b 5079 7468 6f6e 2076 6572  on).![Python ver
-00000120: 7369 6f6e 5d28 6874 7470 733a 2f2f 696d  sion](https://im
-00000130: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
-00000140: 6765 2f50 7974 686f 6e2d 332e 3130 2b2d  ge/Python-3.10+-
-00000150: 626c 7565 2e73 7667 290a 215b 4e65 7442  blue.svg).![NetB
-00000160: 6f78 2076 6572 7369 6f6e 5d28 6874 7470  ox version](http
-00000170: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00000180: 696f 2f62 6164 6765 2f4e 6574 426f 782d  io/badge/NetBox-
-00000190: 332e 347c 332e 352d 626c 7565 2e73 7667  3.4|3.5-blue.svg
-000001a0: 290a 0a3c 212d 2d6d 6b64 6f63 732d 7374  )..<!--mkdocs-st
-000001b0: 6172 742d 2d3e 0a23 2320 5768 6174 3f0a  art-->.## What?.
-000001c0: 5661 6c69 6469 7479 2069 7320 7468 6520  Validity is the 
-000001d0: 5b4e 6574 426f 785d 2868 7474 7073 3a2f  [NetBox](https:/
-000001e0: 2f6e 6574 626f 782e 6465 7629 2070 6c75  /netbox.dev) plu
-000001f0: 6769 6e20 746f 2064 6561 6c20 7769 7468  gin to deal with
-00000200: 2063 6f6e 6669 6775 7261 7469 6f6e 2063   configuration c
-00000210: 6f6d 706c 6961 6e63 652e 2059 6f75 2064  ompliance. You d
-00000220: 6566 696e 6520 636f 6d70 6c69 616e 6365  efine compliance
-00000230: 2074 6573 7473 2061 6e64 2056 616c 6964   tests and Valid
-00000240: 6974 7920 6368 6563 6b73 206e 6574 776f  ity checks netwo
-00000250: 726b 2064 6576 6963 6520 636f 6e66 6967  rk device config
-00000260: 7572 6174 696f 6e20 6669 6c65 7320 6167  uration files ag
-00000270: 6169 6e73 7420 7468 6573 6520 7465 7374  ainst these test
-00000280: 732e 2041 7320 6120 7265 7375 6c74 2079  s. As a result y
-00000290: 6f75 2063 616e 2066 696e 6420 6f75 7420  ou can find out 
-000002a0: 7768 6963 6820 6465 7669 6365 7320 6172  which devices ar
-000002b0: 6520 7072 6f76 6973 696f 6e65 6420 7072  e provisioned pr
-000002c0: 6f70 6572 6c79 2028 6163 636f 7264 696e  operly (accordin
-000002d0: 6720 746f 2074 6865 2074 6573 7473 2079  g to the tests y
-000002e0: 6f75 2068 6176 6520 7772 6974 7465 6e29  ou have written)
-000002f0: 2061 6e64 2077 6869 6368 2061 7265 206e   and which are n
-00000300: 6f74 2e0a 0a54 6f20 7573 6520 7661 6c69  ot...To use vali
-00000310: 6469 7479 2079 6f75 206e 6565 643a 0a0a  dity you need:..
-00000320: 312e 2053 746f 7265 2063 6f6e 6669 6775  1. Store configu
-00000330: 7261 7469 6f6e 2066 696c 6573 206f 6620  ration files of 
-00000340: 796f 7572 2064 6576 6963 6573 2069 6e20  your devices in 
-00000350: 6120 4769 7420 7265 706f 7369 746f 7279  a Git repository
-00000360: 2e20 5661 6c69 6469 7479 2064 6f65 7320  . Validity does 
-00000370: 6e6f 7420 636f 6c6c 6563 7420 7468 6520  not collect the 
-00000380: 636f 6e66 6967 7320 6672 6f6d 2079 6f75  configs from you
-00000390: 7220 6e65 7477 6f72 6b2c 2079 6f75 2068  r network, you h
-000003a0: 6176 6520 746f 2064 6f20 6974 2062 7920  ave to do it by 
-000003b0: 7468 6972 642d 7061 7274 7920 746f 6f6c  third-party tool
-000003c0: 2028 652e 672e 205b 6f78 6964 697a 6564   (e.g. [oxidized
-000003d0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-000003e0: 2e63 6f6d 2f79 7474 692f 6f78 6964 697a  .com/ytti/oxidiz
-000003f0: 6564 2929 2e0a 0a32 2e20 4465 6669 6e65  ed))...2. Define
-00000400: 205b 5454 5020 5465 6d70 6c61 7465 5d28   [TTP Template](
-00000410: 6874 7470 733a 2f2f 7474 702e 7265 6164  https://ttp.read
-00000420: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
-00000430: 7465 7374 2f29 2074 6f20 7472 616e 736c  test/) to transl
-00000440: 6174 6520 7468 6520 636f 6e66 6967 2066  ate the config f
-00000450: 726f 6d20 7665 6e64 6f72 2073 7065 6369  rom vendor speci
-00000460: 6669 6320 666f 726d 6174 2069 6e74 6f20  fic format into 
-00000470: 4a53 4f4e 2e0a 0a33 2e20 5772 6974 6520  JSON...3. Write 
-00000480: 636f 6d70 6c69 616e 6365 2074 6573 7420  compliance test 
-00000490: 6173 2061 2070 7974 686f 6e20 6578 7072  as a python expr
-000004a0: 6573 7369 6f6e 2c20 652e 672e 3c62 722f  ession, e.g.<br/
-000004b0: 3e0a 6064 6576 6963 652e 636f 6e66 6967  >.`device.config
-000004c0: 5b22 6e74 702d 7365 7276 6572 7322 5d20  ["ntp-servers"] 
-000004d0: 3d3d 205b 2231 2e32 2e33 2e34 222c 2022  == ["1.2.3.4", "
-000004e0: 352e 362e 372e 3822 5d60 0a0a 342e 2041  5.6.7.8"]`..4. A
-000004f0: 7070 6c79 2063 7265 6174 6564 2074 6573  pply created tes
-00000500: 7420 746f 2073 7065 6369 6669 6320 6465  t to specific de
-00000510: 7669 6365 7320 616e 6420 6765 7420 7468  vices and get th
-00000520: 6520 7265 7375 6c74 7320 7065 7220 6465  e results per de
-00000530: 7669 6365 2028 7061 7373 6564 206f 7220  vice (passed or 
-00000540: 6661 696c 6564 292e 0a0a 0a23 2320 5768  failed)....## Wh
-00000550: 793f 0a43 6f6e 6669 6775 7261 7469 6f6e  y?.Configuration
-00000560: 2063 6f6d 706c 6961 6e63 6520 6973 206f   compliance is o
-00000570: 6e65 206f 6620 7468 6520 7665 7279 2063  ne of the very c
-00000580: 6f6d 6d6f 6e20 7072 6f62 6c65 6d73 2074  ommon problems t
-00000590: 6861 7420 6172 6973 6573 2069 6e20 6576  hat arises in ev
-000005a0: 6572 7920 636f 6d70 616e 7920 7769 7468  ery company with
-000005b0: 2074 6865 2067 726f 7774 6820 6f66 2074   the growth of t
-000005c0: 6865 6972 206e 6574 776f 726b 2e20 5573  heir network. Us
-000005d0: 7561 6c6c 7920 636f 6d70 616e 6965 7320  ually companies 
-000005e0: 736f 6c76 6520 7468 6973 2070 726f 626c  solve this probl
-000005f0: 656d 2077 6974 6820 736f 6d65 206b 696e  em with some kin
-00000600: 6420 6f66 2073 6372 6970 7473 2074 6861  d of scripts tha
-00000610: 7420 646f 2061 6c6c 2074 6865 2074 6869  t do all the thi
-00000620: 6e67 7320 6174 2074 6865 2073 616d 6520  ngs at the same 
-00000630: 7469 6d65 3a20 7468 6579 2070 6172 7365  time: they parse
-00000640: 2063 6f6e 6669 6773 2c20 6170 706c 7920   configs, apply 
-00000650: 736f 6d65 2063 6f6d 706c 6961 6e63 6520  some compliance 
-00000660: 6c6f 6769 6320 616e 6420 7075 7368 2074  logic and push t
-00000670: 6865 2072 6573 756c 7473 2069 6e74 6f20  he results into 
-00000680: 736f 6d65 2044 4220 6f72 2074 6869 7264  some DB or third
-00000690: 2d70 6172 7479 204f 5353 2073 7973 7465  -party OSS syste
-000006a0: 6d2e 2055 7375 616c 6c79 2061 6674 6572  m. Usually after
-000006b0: 2074 6865 2061 6464 6974 696f 6e20 6f66   the addition of
-000006c0: 2073 6576 6572 616c 2076 656e 646f 7273   several vendors
-000006d0: 2028 6f72 2065 7665 6e20 7365 7665 7261   (or even severa
-000006e0: 6c20 736f 6674 7761 7265 2072 6576 6973  l software revis
-000006f0: 696f 6e73 206f 6620 6f6e 6520 6d6f 6465  ions of one mode
-00000700: 6c29 2074 6865 7365 2073 6372 6970 7473  l) these scripts
-00000710: 2062 6563 6f6d 6520 756e 7265 6164 6162   become unreadab
-00000720: 6c65 2061 6e64 2061 6c6d 6f73 7420 6e6f  le and almost no
-00000730: 206f 6e65 2063 616e 2064 6566 696e 6974   one can definit
-00000740: 656c 7920 7361 7920 7768 6963 6820 7275  ely say which ru
-00000750: 6c65 7320 7468 6520 7363 7269 7074 2063  les the script c
-00000760: 6865 636b 7320 666f 722e 0a0a 5661 6c69  hecks for...Vali
-00000770: 6469 7479 2063 6f6d 706c 6574 656c 7920  dity completely 
-00000780: 7365 7061 7261 7465 7320 636f 6d70 6c69  separates compli
-00000790: 616e 6365 2074 6573 7420 636f 6465 2066  ance test code f
-000007a0: 726f 6d20 616c 6c20 6f74 6865 7220 7468  rom all other th
-000007b0: 696e 6773 206c 696b 6520 636f 6e66 6967  ings like config
-000007c0: 2073 6572 6961 6c69 7a61 7469 6f6e 2e20   serialization. 
-000007d0: 5468 6973 206f 6e65 2065 6e63 6f75 7261  This one encoura
-000007e0: 6765 7320 796f 7520 746f 2077 7269 7465  ges you to write
-000007f0: 2073 686f 7274 2c20 636c 6561 6e20 616e   short, clean an
-00000800: 6420 756e 6465 7273 7461 6e64 6162 6c65  d understandable
-00000810: 2063 6f6d 706c 6961 6e63 6520 7465 7374   compliance test
-00000820: 7320 746f 6765 7468 6572 2077 6974 6820  s together with 
-00000830: 7468 6520 6d61 6e64 6174 6f72 7920 6465  the mandatory de
-00000840: 7363 7269 7074 696f 6e2e 0a0a 0a23 2320  scription....## 
-00000850: 4b65 7920 6665 6174 7572 6573 0a2a 2054  Key features.* T
-00000860: 7275 6c79 2076 656e 646f 722d 6167 6e6f  ruly vendor-agno
-00000870: 7374 6963 2e20 596f 7520 6361 6e20 6561  stic. You can ea
-00000880: 7369 6c79 2069 6e74 6567 7261 7465 2061  sily integrate a
-00000890: 6e79 2076 656e 646f 7220 636f 6e66 6967  ny vendor config
-000008a0: 2066 6f72 6d61 7420 7573 696e 6720 5b54   format using [T
-000008b0: 5450 5d28 6874 7470 733a 2f2f 6769 7468  TP](https://gith
-000008c0: 7562 2e63 6f6d 2f64 6d75 6c79 616c 696e  ub.com/dmulyalin
-000008d0: 2f74 7470 290a 2a20 5772 6974 696e 6720  /ttp).* Writing 
-000008e0: 636f 6d70 6c69 616e 6365 2074 6573 7473  compliance tests
-000008f0: 2075 7369 6e67 2050 7974 686f 6e20 6578   using Python ex
-00000900: 7072 6573 7369 6f6e 7320 616e 6420 5b4a  pressions and [J
-00000910: 515d 2868 7474 7073 3a2f 2f73 7465 646f  Q](https://stedo
-00000920: 6c61 6e2e 6769 7468 7562 2e69 6f2f 6a71  lan.github.io/jq
-00000930: 2f6d 616e 7561 6c2f 290a 2a20 466c 6578  /manual/).* Flex
-00000940: 6962 6c65 2073 656c 6563 746f 7220 7379  ible selector sy
-00000950: 7374 656d 2074 6f20 6170 706c 7920 7468  stem to apply th
-00000960: 6520 7465 7374 7320 6f6e 6c79 2074 6f20  e tests only to 
-00000970: 6120 7370 6563 6966 6963 2073 7562 7365  a specific subse
-00000980: 7420 6f66 2064 6576 6963 6573 0a2a 2043  t of devices.* C
-00000990: 6f6e 6365 7074 206f 6620 2a2a 6479 6e61  oncept of **dyna
-000009a0: 6d69 6320 7061 6972 732a 2a2e 2057 6974  mic pairs**. Wit
-000009b0: 6820 6479 6e61 6d69 6320 7061 6972 2079  h dynamic pair y
-000009c0: 6f75 2063 616e 2063 6f6d 7061 7265 2032  ou can compare 2
-000009d0: 2064 6966 6665 7265 6e74 2064 6576 6963   different devic
-000009e0: 6573 2062 6574 7765 656e 2065 6163 6820  es between each 
-000009f0: 6f74 6865 7220 2865 2e67 2e20 636f 6d70  other (e.g. comp
-00000a00: 6172 6520 7468 6520 636f 6e66 6967 7572  are the configur
-00000a10: 6174 696f 6e20 6f66 2032 204d 432d 4c41  ation of 2 MC-LA
-00000a20: 4720 6d65 6d62 6572 7329 2e0a 2a20 2a2a  G members)..* **
-00000a30: 5465 7374 2072 6573 756c 7420 6578 706c  Test result expl
-00000a40: 616e 6174 696f 6e2a 2a2e 2057 6865 6e20  anation**. When 
-00000a50: 736f 6d65 2074 6573 7420 6661 696c 732c  some test fails,
-00000a60: 2079 6f75 2063 616e 2067 6574 2074 6865   you can get the
-00000a70: 202a 2a65 7870 6c61 6e61 7469 6f6e 2a2a   **explanation**
-00000a80: 206f 6620 7468 6520 6361 6c63 756c 6174   of the calculat
-00000a90: 696f 6e20 7072 6f63 6573 7320 7374 6570  ion process step
-00000aa0: 2062 7920 7374 6570 2e20 4974 2068 656c   by step. It hel
-00000ab0: 7073 2074 6f20 6964 656e 7469 6679 2074  ps to identify t
-00000ac0: 6865 2063 6175 7365 206f 6620 7468 6520  he cause of the 
-00000ad0: 6661 696c 7572 652e 0a2a 202a 2a4f 524d  failure..* **ORM
-00000ae0: 2061 6363 6573 732a 2a20 696e 7369 6465   access** inside
-00000af0: 2074 6865 2074 6573 742e 2059 6f75 2068   the test. You h
-00000b00: 6176 6520 6675 6c6c 2061 6363 6573 7320  ave full access 
-00000b10: 746f 2074 6865 202a 2a64 6576 6963 652a  to the **device*
-00000b20: 2a20 7072 6f70 6572 7469 6573 2e20 466f  * properties. Fo
-00000b30: 7220 696e 7374 616e 6365 2c20 796f 7520  r instance, you 
-00000b40: 6d61 7920 6c65 7665 7261 6765 205b 436f  may leverage [Co
-00000b50: 6e66 6967 7572 6174 696f 6e20 436f 6e74  nfiguration Cont
-00000b60: 6578 7473 5d28 6874 7470 733a 2f2f 646f  exts](https://do
-00000b70: 6373 2e6e 6574 626f 782e 6465 762f 656e  cs.netbox.dev/en
-00000b80: 2f73 7461 626c 652f 6665 6174 7572 6573  /stable/features
-00000b90: 2f63 6f6e 7465 7874 2d64 6174 612f 2920  /context-data/) 
-00000ba0: 4e65 7442 6f78 2066 6561 7475 7265 2074  NetBox feature t
-00000bb0: 6f20 7374 6f72 6520 796f 7572 2064 6573  o store your des
-00000bc0: 6972 6564 2063 6f6e 6669 6775 7261 7469  ired configurati
-00000bd0: 6f6e 2061 6e64 2063 6f6d 7061 7265 2069  on and compare i
-00000be0: 7420 7769 7468 2074 6865 2063 6f6e 6669  t with the confi
-00000bf0: 6720 636f 6c6c 6563 7465 6420 6672 6f6d  g collected from
-00000c00: 2074 6865 2064 6576 6963 652e 0a2a 202a   the device..* *
-00000c10: 2a52 6570 6f72 7473 2061 6e64 2077 6562  *Reports and web
-00000c20: 686f 6f6b 732a 2a2e 2041 6674 6572 2065  hooks**. After e
-00000c30: 7865 6375 7469 6f6e 206f 6620 736f 6d65  xecution of some
-00000c40: 2062 756e 6368 206f 6620 7465 7374 7320   bunch of tests 
-00000c50: 796f 7520 6361 6e20 6765 7420 7468 6520  you can get the 
-00000c60: 7265 706f 7274 2077 6974 6820 7061 7373  report with pass
-00000c70: 6564 2f66 6169 6c65 6420 7374 6174 6973  ed/failed statis
-00000c80: 7469 6373 2067 726f 7570 6564 2062 7920  tics grouped by 
-00000c90: 736f 6d65 204c 6f63 6174 696f 6e2f 5369  some Location/Si
-00000ca0: 7465 2f4d 616e 7566 6163 7475 7265 722f  te/Manufacturer/
-00000cb0: 6574 632e 204d 6f72 656f 7665 722c 2079  etc. Moreover, y
-00000cc0: 6f75 2063 616e 2070 726f 7669 7369 6f6e  ou can provision
-00000cd0: 2074 6865 2077 6562 686f 6f6b 2074 6f20   the webhook to 
-00000ce0: 6e6f 7469 6679 2061 6e20 6578 7465 726e  notify an extern
-00000cf0: 616c 2073 7973 7465 6d20 7768 656e 2063  al system when c
-00000d00: 6f6d 706c 6961 6e63 6520 7265 706f 7274  ompliance report
-00000d10: 2069 7320 6765 6e65 7261 7465 642e 0a2a   is generated..*
-00000d20: 202a 2a54 6573 7420 6578 7465 6e73 6962   **Test extensib
-00000d30: 696c 6974 792a 2a2e 2059 6f75 2063 616e  ility**. You can
-00000d40: 2064 6566 696e 6520 796f 7572 206f 776e   define your own
-00000d50: 2070 7974 686f 6e20 6675 6e63 7469 6f6e   python function
-00000d60: 7320 6f72 2063 6c61 7373 6573 2074 6f20  s or classes to 
-00000d70: 7265 7573 6520 7468 6520 636f 6465 2062  reuse the code b
-00000d80: 6574 7765 656e 206d 756c 7469 706c 6520  etween multiple 
-00000d90: 636f 6d70 6c69 616e 6365 2074 6573 7473  compliance tests
-00000da0: 2e0a 2a20 506f 7373 6962 696c 6974 7920  ..* Possibility 
-00000db0: 746f 2073 746f 7265 2061 6c6c 2068 6561  to store all hea
-00000dc0: 7679 2074 6578 742d 6261 7365 6420 656e  vy text-based en
-00000dd0: 7469 7469 6573 2028 6c69 6b65 2063 6f6d  tities (like com
-00000de0: 706c 6961 6e63 6520 7465 7374 7320 6f72  pliance tests or
-00000df0: 2054 5450 2054 656d 706c 6174 6573 2920   TTP Templates) 
-00000e00: 696e 2061 202a 2a47 6974 2072 6570 6f73  in a **Git repos
-00000e10: 6974 6f72 792a 2a0a 3c21 2d2d 6d6b 646f  itory**.<!--mkdo
-00000e20: 6373 2d65 6e64 2d2d 3e0a 0a23 2320 446f  cs-end-->..## Do
-00000e30: 6375 6d65 6e74 6174 696f 6e0a 5265 6164  cumentation.Read
-00000e40: 2074 6865 2066 756c 6c20 646f 6375 6d65   the full docume
-00000e50: 6e74 6174 696f 6e20 6f6e 205b 7661 6c69  ntation on [vali
-00000e60: 6469 7479 2e72 6561 6474 6865 646f 6373  dity.readthedocs
-00000e70: 2e69 6f5d 2868 7474 7073 3a2f 2f76 616c  .io](https://val
-00000e80: 6964 6974 792e 7265 6164 7468 6564 6f63  idity.readthedoc
-00000e90: 732e 696f 290a 0a0a 2323 2051 7569 636b  s.io)...## Quick
-00000ea0: 2053 7461 7274 0a0a 5468 6520 7368 6f72   Start..The shor
-00000eb0: 7420 7669 6465 6f20 6162 6f75 7420 6669  t video about fi
-00000ec0: 7273 7420 7374 6570 7320 7769 7468 2056  rst steps with V
-00000ed0: 616c 6964 6974 793a 0a0a 5b21 5b57 6174  alidity:..[![Wat
-00000ee0: 6368 2074 6865 2076 6964 656f 5d28 6874  ch the video](ht
-00000ef0: 7470 733a 2f2f 696d 672e 796f 7574 7562  tps://img.youtub
-00000f00: 652e 636f 6d2f 7669 2f48 7332 4955 4536  e.com/vi/Hs2IUE6
-00000f10: 724b 4334 2f30 2e6a 7067 295d 2868 7474  rKC4/0.jpg)](htt
-00000f20: 7073 3a2f 2f79 6f75 7475 2e62 652f 4873  ps://youtu.be/Hs
-00000f30: 3249 5545 3672 4b43 3429 0a0a 2323 2043  2IUE6rKC4)..## C
-00000f40: 6f6e 7472 6962 7574 696e 670a 0a46 6565  ontributing..Fee
-00000f50: 6c20 6672 6565 2074 6f20 6173 6b20 6120  l free to ask a 
-00000f60: 5b51 7565 7374 696f 6e5d 2868 7474 7073  [Question](https
-00000f70: 3a2f 2f67 6974 6875 622e 636f 6d2f 616d  ://github.com/am
-00000f80: 7961 736e 696b 6f76 2f76 616c 6964 6974  yasnikov/validit
-00000f90: 792f 6469 7363 7573 7369 6f6e 7329 2c20  y/discussions), 
-00000fa0: 7265 706f 7274 2061 6e20 5b49 7373 7565  report an [Issue
-00000fb0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00000fc0: 2e63 6f6d 2f61 6d79 6173 6e69 6b6f 762f  .com/amyasnikov/
-00000fd0: 7661 6c69 6469 7479 2f69 7373 7565 7329  validity/issues)
-00000fe0: 206f 7220 6576 656e 206d 616b 6520 6120   or even make a 
-00000ff0: 5b50 525d 2843 4f4e 5452 4942 5554 494e  [PR](CONTRIBUTIN
-00001000: 472e 6d64 292e 2052 6561 6420 6d6f 7265  G.md). Read more
-00001010: 2061 626f 7574 2063 6f6e 7472 6962 7574   about contribut
-00001020: 696f 6e20 696e 2074 6865 205b 434f 4e54  ion in the [CONT
-00001030: 5249 4255 5449 4e47 5d28 434f 4e54 5249  RIBUTING](CONTRI
-00001040: 4255 5449 4e47 2e6d 6429 2067 7569 6465  BUTING.md) guide
-00001050: 2e0a                                     ..
+00000000: 3c64 6976 2061 6c69 676e 3d22 6365 6e74  <div align="cent
+00000010: 6572 223e 0a20 2020 203c 6120 6872 6566  er">.    <a href
+00000020: 3d22 6874 7470 733a 2f2f 7661 6c69 6469  ="https://validi
+00000030: 7479 2e72 6561 6474 6865 646f 6373 2e69  ty.readthedocs.i
+00000040: 6f22 3e3c 696d 6720 7372 633d 2268 7474  o"><img src="htt
+00000050: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
+00000060: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f61  sercontent.com/a
+00000070: 6d79 6173 6e69 6b6f 762f 7661 6c69 6469  myasnikov/validi
+00000080: 7479 2f6d 6173 7465 722f 646f 6373 2f76  ty/master/docs/v
+00000090: 616c 6964 6974 795f 6c6f 676f 2e70 6e67  alidity_logo.png
+000000a0: 2220 616c 743d 2243 6c69 636b 2074 6f20  " alt="Click to 
+000000b0: 7669 6577 2056 616c 6964 6974 7920 646f  view Validity do
+000000c0: 6373 222f 3e3c 2f61 3e0a 2020 2020 3c68  cs"/></a>.    <h
+000000d0: 313e 5661 6c69 6469 7479 3a20 7665 6e64  1>Validity: vend
+000000e0: 6f72 2d61 676e 6f73 7469 6320 636f 6e66  or-agnostic conf
+000000f0: 6967 7572 6174 696f 6e20 636f 6d70 6c69  iguration compli
+00000100: 616e 6365 3c2f 6831 3e0a 2020 2020 3c70  ance</h1>.    <p
+00000110: 3e0a 2020 2020 2020 2020 3c69 6d67 2073  >.        <img s
+00000120: 7263 3d22 6874 7470 733a 2f2f 6769 7468  rc="https://gith
+00000130: 7562 2e63 6f6d 2f61 6d79 6173 6e69 6b6f  ub.com/amyasniko
+00000140: 762f 7661 6c69 6469 7479 2f61 6374 696f  v/validity/actio
+00000150: 6e73 2f77 6f72 6b66 6c6f 7773 2f63 692e  ns/workflows/ci.
+00000160: 796d 6c2f 6261 6467 652e 7376 6722 2061  yml/badge.svg" a
+00000170: 6c74 3d22 4349 223e 0a20 2020 2020 2020  lt="CI">.       
+00000180: 203c 696d 6720 7372 633d 2268 7474 7073   <img src="https
+00000190: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+000001a0: 6f2f 656e 6470 6f69 6e74 3f75 726c 3d68  o/endpoint?url=h
+000001b0: 7474 7073 3a2f 2f67 6973 742e 6769 7468  ttps://gist.gith
+000001c0: 7562 7573 6572 636f 6e74 656e 742e 636f  ubusercontent.co
+000001d0: 6d2f 616d 7961 736e 696b 6f76 2f39 6535  m/amyasnikov/9e5
+000001e0: 3138 6165 3862 6162 6431 3862 3765 6464  18ae8babd18b7edd
+000001f0: 3865 6535 6161 6435 3831 3436 622f 7261  8ee5aad58146b/ra
+00000200: 772f 636f 762e 6a73 6f6e 2220 616c 743d  w/cov.json" alt=
+00000210: 2243 6f76 6572 6167 6522 3e0a 2020 2020  "Coverage">.    
+00000220: 2020 2020 3c69 6d67 2073 7263 3d22 6874      <img src="ht
+00000230: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000240: 732e 696f 2f62 6164 6765 2f50 7974 686f  s.io/badge/Pytho
+00000250: 6e2d 332e 3130 2b2d 626c 7565 2e73 7667  n-3.10+-blue.svg
+00000260: 2220 616c 743d 2250 7974 686f 6e20 7665  " alt="Python ve
+00000270: 7273 696f 6e22 3e0a 2020 2020 2020 2020  rsion">.        
+00000280: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00000290: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+000002a0: 2f62 6164 6765 2f4e 6574 426f 782d 332e  /badge/NetBox-3.
+000002b0: 347c 332e 352d 626c 7565 2e73 7667 2220  4|3.5-blue.svg" 
+000002c0: 616c 743d 224e 6574 426f 7820 7665 7273  alt="NetBox vers
+000002d0: 696f 6e22 3e0a 2020 2020 3c2f 703e 0a3c  ion">.    </p>.<
+000002e0: 2f64 6976 3e0a 0a3c 212d 2d6d 6b64 6f63  /div>..<!--mkdoc
+000002f0: 732d 7374 6172 742d 2d3e 0a23 2320 5768  s-start-->.## Wh
+00000300: 6174 3f0a 5661 6c69 6469 7479 2069 7320  at?.Validity is 
+00000310: 7468 6520 5b4e 6574 426f 785d 2868 7474  the [NetBox](htt
+00000320: 7073 3a2f 2f6e 6574 626f 782e 6465 7629  ps://netbox.dev)
+00000330: 2070 6c75 6769 6e20 746f 2077 7269 7465   plugin to write
+00000340: 2022 6175 746f 2074 6573 7473 2220 666f   "auto tests" fo
+00000350: 7220 636f 6e66 6967 7572 6174 696f 6e2e  r configuration.
+00000360: 2059 6f75 2064 6566 696e 6520 636f 6d70   You define comp
+00000370: 6c69 616e 6365 2074 6573 7473 2061 6e64  liance tests and
+00000380: 2056 616c 6964 6974 7920 6368 6563 6b73   Validity checks
+00000390: 206e 6574 776f 726b 2064 6576 6963 6520   network device 
+000003a0: 636f 6e66 6967 7572 6174 696f 6e20 6669  configuration fi
+000003b0: 6c65 7320 6167 6169 6e73 7420 7468 6573  les against thes
+000003c0: 6520 7465 7374 732e 2041 7320 6120 7265  e tests. As a re
+000003d0: 7375 6c74 2079 6f75 2063 616e 2066 696e  sult you can fin
+000003e0: 6420 6f75 7420 7768 6963 6820 6465 7669  d out which devi
+000003f0: 6365 7320 6172 6520 7072 6f76 6973 696f  ces are provisio
+00000400: 6e65 6420 7072 6f70 6572 6c79 2028 6163  ned properly (ac
+00000410: 636f 7264 696e 6720 746f 2074 6865 2074  cording to the t
+00000420: 6573 7473 2079 6f75 2068 6176 6520 7772  ests you have wr
+00000430: 6974 7465 6e29 2061 6e64 2077 6869 6368  itten) and which
+00000440: 2061 7265 206e 6f74 2e0a 0a54 6f20 7573   are not...To us
+00000450: 6520 7661 6c69 6469 7479 2079 6f75 206e  e validity you n
+00000460: 6565 643a 0a0a 312e 2053 746f 7265 2063  eed:..1. Store c
+00000470: 6f6e 6669 6775 7261 7469 6f6e 2066 696c  onfiguration fil
+00000480: 6573 206f 6620 796f 7572 2064 6576 6963  es of your devic
+00000490: 6573 2069 6e20 6120 4769 7420 7265 706f  es in a Git repo
+000004a0: 7369 746f 7279 2e20 5661 6c69 6469 7479  sitory. Validity
+000004b0: 2064 6f65 7320 6e6f 7420 636f 6c6c 6563   does not collec
+000004c0: 7420 7468 6520 636f 6e66 6967 7320 6672  t the configs fr
+000004d0: 6f6d 2079 6f75 7220 6e65 7477 6f72 6b2c  om your network,
+000004e0: 2079 6f75 2068 6176 6520 746f 2064 6f20   you have to do 
+000004f0: 6974 2062 7920 7468 6972 642d 7061 7274  it by third-part
+00000500: 7920 746f 6f6c 2028 652e 672e 205b 6f78  y tool (e.g. [ox
+00000510: 6964 697a 6564 5d28 6874 7470 733a 2f2f  idized](https://
+00000520: 6769 7468 7562 2e63 6f6d 2f79 7474 692f  github.com/ytti/
+00000530: 6f78 6964 697a 6564 2929 2e0a 0a32 2e20  oxidized))...2. 
+00000540: 4465 6669 6e65 205b 5454 5020 5465 6d70  Define [TTP Temp
+00000550: 6c61 7465 5d28 6874 7470 733a 2f2f 7474  late](https://tt
+00000560: 702e 7265 6164 7468 6564 6f63 732e 696f  p.readthedocs.io
+00000570: 2f65 6e2f 6c61 7465 7374 2f29 2074 6f20  /en/latest/) to 
+00000580: 7472 616e 736c 6174 6520 7468 6520 636f  translate the co
+00000590: 6e66 6967 2066 726f 6d20 7665 6e64 6f72  nfig from vendor
+000005a0: 2073 7065 6369 6669 6320 666f 726d 6174   specific format
+000005b0: 2069 6e74 6f20 4a53 4f4e 2e0a 0a33 2e20   into JSON...3. 
+000005c0: 5772 6974 6520 636f 6d70 6c69 616e 6365  Write compliance
+000005d0: 2074 6573 7420 6173 2061 2070 7974 686f   test as a pytho
+000005e0: 6e20 6578 7072 6573 7369 6f6e 2c20 652e  n expression, e.
+000005f0: 672e 3c62 722f 3e0a 6064 6576 6963 652e  g.<br/>.`device.
+00000600: 636f 6e66 6967 5b22 6e74 702d 7365 7276  config["ntp-serv
+00000610: 6572 7322 5d20 3d3d 205b 2231 2e32 2e33  ers"] == ["1.2.3
+00000620: 2e34 222c 2022 352e 362e 372e 3822 5d60  .4", "5.6.7.8"]`
+00000630: 0a0a 342e 2041 7070 6c79 2063 7265 6174  ..4. Apply creat
+00000640: 6564 2074 6573 7420 746f 2073 7065 6369  ed test to speci
+00000650: 6669 6320 6465 7669 6365 7320 616e 6420  fic devices and 
+00000660: 6765 7420 7468 6520 7265 7375 6c74 7320  get the results 
+00000670: 7065 7220 6465 7669 6365 2028 7061 7373  per device (pass
+00000680: 6564 206f 7220 6661 696c 6564 292e 0a0a  ed or failed)...
+00000690: 0a23 2320 5768 793f 0a43 6f6e 6669 6775  .## Why?.Configu
+000006a0: 7261 7469 6f6e 2063 6f6d 706c 6961 6e63  ration complianc
+000006b0: 6520 6973 206f 6e65 206f 6620 7468 6520  e is one of the 
+000006c0: 7665 7279 2063 6f6d 6d6f 6e20 7072 6f62  very common prob
+000006d0: 6c65 6d73 2074 6861 7420 6172 6973 6573  lems that arises
+000006e0: 2069 6e20 6576 6572 7920 636f 6d70 616e   in every compan
+000006f0: 7920 7769 7468 2074 6865 2067 726f 7774  y with the growt
+00000700: 6820 6f66 2074 6865 6972 206e 6574 776f  h of their netwo
+00000710: 726b 2e20 5573 7561 6c6c 7920 636f 6d70  rk. Usually comp
+00000720: 616e 6965 7320 736f 6c76 6520 7468 6973  anies solve this
+00000730: 2070 726f 626c 656d 2077 6974 6820 736f   problem with so
+00000740: 6d65 206b 696e 6420 6f66 2073 6372 6970  me kind of scrip
+00000750: 7473 2074 6861 7420 646f 2061 6c6c 2074  ts that do all t
+00000760: 6865 2074 6869 6e67 7320 6174 2074 6865  he things at the
+00000770: 2073 616d 6520 7469 6d65 3a20 7468 6579   same time: they
+00000780: 2070 6172 7365 2063 6f6e 6669 6773 2c20   parse configs, 
+00000790: 6170 706c 7920 736f 6d65 2063 6f6d 706c  apply some compl
+000007a0: 6961 6e63 6520 6c6f 6769 6320 616e 6420  iance logic and 
+000007b0: 7075 7368 2074 6865 2072 6573 756c 7473  push the results
+000007c0: 2069 6e74 6f20 736f 6d65 2044 4220 6f72   into some DB or
+000007d0: 2074 6869 7264 2d70 6172 7479 204f 5353   third-party OSS
+000007e0: 2073 7973 7465 6d2e 2055 7375 616c 6c79   system. Usually
+000007f0: 2061 6674 6572 2074 6865 2061 6464 6974   after the addit
+00000800: 696f 6e20 6f66 2073 6576 6572 616c 2076  ion of several v
+00000810: 656e 646f 7273 2028 6f72 2065 7665 6e20  endors (or even 
+00000820: 7365 7665 7261 6c20 736f 6674 7761 7265  several software
+00000830: 2072 6576 6973 696f 6e73 206f 6620 6f6e   revisions of on
+00000840: 6520 6d6f 6465 6c29 2074 6865 7365 2073  e model) these s
+00000850: 6372 6970 7473 2062 6563 6f6d 6520 756e  cripts become un
+00000860: 7265 6164 6162 6c65 2061 6e64 2061 6c6d  readable and alm
+00000870: 6f73 7420 6e6f 206f 6e65 2063 616e 2064  ost no one can d
+00000880: 6566 696e 6974 656c 7920 7361 7920 7768  efinitely say wh
+00000890: 6963 6820 7275 6c65 7320 7468 6520 7363  ich rules the sc
+000008a0: 7269 7074 2063 6865 636b 7320 666f 722e  ript checks for.
+000008b0: 0a0a 5661 6c69 6469 7479 2063 6f6d 706c  ..Validity compl
+000008c0: 6574 656c 7920 7365 7061 7261 7465 7320  etely separates 
+000008d0: 636f 6d70 6c69 616e 6365 2074 6573 7420  compliance test 
+000008e0: 636f 6465 2066 726f 6d20 616c 6c20 6f74  code from all ot
+000008f0: 6865 7220 7468 696e 6773 206c 696b 6520  her things like 
+00000900: 636f 6e66 6967 2073 6572 6961 6c69 7a61  config serializa
+00000910: 7469 6f6e 2e20 5468 6973 206f 6e65 2065  tion. This one e
+00000920: 6e63 6f75 7261 6765 7320 796f 7520 746f  ncourages you to
+00000930: 2077 7269 7465 2073 686f 7274 2c20 636c   write short, cl
+00000940: 6561 6e20 616e 6420 756e 6465 7273 7461  ean and understa
+00000950: 6e64 6162 6c65 2063 6f6d 706c 6961 6e63  ndable complianc
+00000960: 6520 7465 7374 7320 746f 6765 7468 6572  e tests together
+00000970: 2077 6974 6820 7468 6520 6d61 6e64 6174   with the mandat
+00000980: 6f72 7920 6465 7363 7269 7074 696f 6e2e  ory description.
+00000990: 0a0a 0a23 2320 4b65 7920 4665 6174 7572  ...## Key Featur
+000009a0: 6573 0a2a 2054 7275 6c79 2076 656e 646f  es.* Truly vendo
+000009b0: 722d 6167 6e6f 7374 6963 2e20 596f 7520  r-agnostic. You 
+000009c0: 6361 6e20 6561 7369 6c79 2069 6e74 6567  can easily integ
+000009d0: 7261 7465 2061 6e79 2076 656e 646f 7220  rate any vendor 
+000009e0: 636f 6e66 6967 2066 6f72 6d61 7420 7573  config format us
+000009f0: 696e 6720 5b54 5450 5d28 6874 7470 733a  ing [TTP](https:
+00000a00: 2f2f 6769 7468 7562 2e63 6f6d 2f64 6d75  //github.com/dmu
+00000a10: 6c79 616c 696e 2f74 7470 290a 2a20 5772  lyalin/ttp).* Wr
+00000a20: 6974 696e 6720 636f 6d70 6c69 616e 6365  iting compliance
+00000a30: 2074 6573 7473 2075 7369 6e67 2050 7974   tests using Pyt
+00000a40: 686f 6e20 6578 7072 6573 7369 6f6e 7320  hon expressions 
+00000a50: 616e 6420 5b4a 515d 2868 7474 7073 3a2f  and [JQ](https:/
+00000a60: 2f73 7465 646f 6c61 6e2e 6769 7468 7562  /stedolan.github
+00000a70: 2e69 6f2f 6a71 2f6d 616e 7561 6c2f 290a  .io/jq/manual/).
+00000a80: 2a20 466c 6578 6962 6c65 2073 656c 6563  * Flexible selec
+00000a90: 746f 7220 7379 7374 656d 2074 6f20 6170  tor system to ap
+00000aa0: 706c 7920 7468 6520 7465 7374 7320 6f6e  ply the tests on
+00000ab0: 6c79 2074 6f20 6120 7370 6563 6966 6963  ly to a specific
+00000ac0: 2073 7562 7365 7420 6f66 2064 6576 6963   subset of devic
+00000ad0: 6573 0a2a 2043 6f6e 6365 7074 206f 6620  es.* Concept of 
+00000ae0: 2a2a 6479 6e61 6d69 6320 7061 6972 732a  **dynamic pairs*
+00000af0: 2a2e 2057 6974 6820 6479 6e61 6d69 6320  *. With dynamic 
+00000b00: 7061 6972 2079 6f75 2063 616e 2063 6f6d  pair you can com
+00000b10: 7061 7265 2032 2064 6966 6665 7265 6e74  pare 2 different
+00000b20: 2064 6576 6963 6573 2062 6574 7765 656e   devices between
+00000b30: 2065 6163 6820 6f74 6865 7220 2865 2e67   each other (e.g
+00000b40: 2e20 636f 6d70 6172 6520 7468 6520 636f  . compare the co
+00000b50: 6e66 6967 7572 6174 696f 6e20 6f66 2032  nfiguration of 2
+00000b60: 204d 432d 4c41 4720 6d65 6d62 6572 7329   MC-LAG members)
+00000b70: 2e0a 2a20 2a2a 5465 7374 2072 6573 756c  ..* **Test resul
+00000b80: 7420 6578 706c 616e 6174 696f 6e2a 2a2e  t explanation**.
+00000b90: 2057 6865 6e20 736f 6d65 2074 6573 7420   When some test 
+00000ba0: 6661 696c 732c 2079 6f75 2063 616e 2067  fails, you can g
+00000bb0: 6574 2074 6865 202a 2a65 7870 6c61 6e61  et the **explana
+00000bc0: 7469 6f6e 2a2a 206f 6620 7468 6520 6361  tion** of the ca
+00000bd0: 6c63 756c 6174 696f 6e20 7072 6f63 6573  lculation proces
+00000be0: 7320 7374 6570 2062 7920 7374 6570 2e20  s step by step. 
+00000bf0: 4974 2068 656c 7073 2074 6f20 6964 656e  It helps to iden
+00000c00: 7469 6679 2074 6865 2063 6175 7365 206f  tify the cause o
+00000c10: 6620 7468 6520 6661 696c 7572 652e 0a2a  f the failure..*
+00000c20: 202a 2a4f 524d 2061 6363 6573 732a 2a20   **ORM access** 
+00000c30: 696e 7369 6465 2074 6865 2074 6573 742e  inside the test.
+00000c40: 2059 6f75 2068 6176 6520 6675 6c6c 2061   You have full a
+00000c50: 6363 6573 7320 746f 2074 6865 202a 2a64  ccess to the **d
+00000c60: 6576 6963 652a 2a20 7072 6f70 6572 7469  evice** properti
+00000c70: 6573 2e20 466f 7220 696e 7374 616e 6365  es. For instance
+00000c80: 2c20 796f 7520 6d61 7920 6c65 7665 7261  , you may levera
+00000c90: 6765 205b 436f 6e66 6967 7572 6174 696f  ge [Configuratio
+00000ca0: 6e20 436f 6e74 6578 7473 5d28 6874 7470  n Contexts](http
+00000cb0: 733a 2f2f 646f 6373 2e6e 6574 626f 782e  s://docs.netbox.
+00000cc0: 6465 762f 656e 2f73 7461 626c 652f 6665  dev/en/stable/fe
+00000cd0: 6174 7572 6573 2f63 6f6e 7465 7874 2d64  atures/context-d
+00000ce0: 6174 612f 2920 4e65 7442 6f78 2066 6561  ata/) NetBox fea
+00000cf0: 7475 7265 2074 6f20 7374 6f72 6520 796f  ture to store yo
+00000d00: 7572 2064 6573 6972 6564 2063 6f6e 6669  ur desired confi
+00000d10: 6775 7261 7469 6f6e 2061 6e64 2063 6f6d  guration and com
+00000d20: 7061 7265 2069 7420 7769 7468 2074 6865  pare it with the
+00000d30: 2063 6f6e 6669 6720 636f 6c6c 6563 7465   config collecte
+00000d40: 6420 6672 6f6d 2074 6865 2064 6576 6963  d from the devic
+00000d50: 652e 0a2a 202a 2a52 6570 6f72 7473 2061  e..* **Reports a
+00000d60: 6e64 2077 6562 686f 6f6b 732a 2a2e 2041  nd webhooks**. A
+00000d70: 6674 6572 2065 7865 6375 7469 6f6e 206f  fter execution o
+00000d80: 6620 736f 6d65 2062 756e 6368 206f 6620  f some bunch of 
+00000d90: 7465 7374 7320 796f 7520 6361 6e20 6765  tests you can ge
+00000da0: 7420 7468 6520 7265 706f 7274 2077 6974  t the report wit
+00000db0: 6820 7061 7373 6564 2f66 6169 6c65 6420  h passed/failed 
+00000dc0: 7374 6174 6973 7469 6373 2067 726f 7570  statistics group
+00000dd0: 6564 2062 7920 736f 6d65 204c 6f63 6174  ed by some Locat
+00000de0: 696f 6e2f 5369 7465 2f4d 616e 7566 6163  ion/Site/Manufac
+00000df0: 7475 7265 722f 6574 632e 204d 6f72 656f  turer/etc. Moreo
+00000e00: 7665 722c 2079 6f75 2063 616e 2070 726f  ver, you can pro
+00000e10: 7669 7369 6f6e 2074 6865 2077 6562 686f  vision the webho
+00000e20: 6f6b 2074 6f20 6e6f 7469 6679 2061 6e20  ok to notify an 
+00000e30: 6578 7465 726e 616c 2073 7973 7465 6d20  external system 
+00000e40: 7768 656e 2063 6f6d 706c 6961 6e63 6520  when compliance 
+00000e50: 7265 706f 7274 2069 7320 6765 6e65 7261  report is genera
+00000e60: 7465 642e 0a2a 202a 2a54 6573 7420 6578  ted..* **Test ex
+00000e70: 7465 6e73 6962 696c 6974 792a 2a2e 2059  tensibility**. Y
+00000e80: 6f75 2063 616e 2064 6566 696e 6520 796f  ou can define yo
+00000e90: 7572 206f 776e 2070 7974 686f 6e20 6675  ur own python fu
+00000ea0: 6e63 7469 6f6e 7320 6f72 2063 6c61 7373  nctions or class
+00000eb0: 6573 2074 6f20 7265 7573 6520 7468 6520  es to reuse the 
+00000ec0: 636f 6465 2062 6574 7765 656e 206d 756c  code between mul
+00000ed0: 7469 706c 6520 636f 6d70 6c69 616e 6365  tiple compliance
+00000ee0: 2074 6573 7473 2e0a 2a20 506f 7373 6962   tests..* Possib
+00000ef0: 696c 6974 7920 746f 2073 746f 7265 2061  ility to store a
+00000f00: 6c6c 2068 6561 7679 2074 6578 742d 6261  ll heavy text-ba
+00000f10: 7365 6420 656e 7469 7469 6573 2028 6c69  sed entities (li
+00000f20: 6b65 2063 6f6d 706c 6961 6e63 6520 7465  ke compliance te
+00000f30: 7374 7320 6f72 2054 5450 2054 656d 706c  sts or TTP Templ
+00000f40: 6174 6573 2920 696e 2061 202a 2a47 6974  ates) in a **Git
+00000f50: 2072 6570 6f73 6974 6f72 792a 2a0a 0a23   repository**..#
+00000f60: 2320 446f 776e 6c6f 6164 2061 6e64 2049  # Download and I
+00000f70: 6e73 7461 6c6c 0a0a 596f 7520 6361 6e20  nstall..You can 
+00000f80: 646f 776e 6c6f 6164 2056 616c 6964 6974  download Validit
+00000f90: 7920 7669 6120 2a2a 7069 702a 2a0a 6060  y via **pip**.``
+00000fa0: 600a 7069 7020 696e 7374 616c 6c20 6e65  `.pip install ne
+00000fb0: 7462 6f78 2d76 616c 6964 6974 790a 6060  tbox-validity.``
+00000fc0: 600a 4166 7465 7220 7468 6174 2066 6f6c  `.After that fol
+00000fd0: 6c6f 7720 7468 6520 5b69 6e73 7461 6c6c  low the [install
+00000fe0: 6174 696f 6e20 6775 6964 655d 2868 7474  ation guide](htt
+00000ff0: 7073 3a2f 2f76 616c 6964 6974 792e 7265  ps://validity.re
+00001000: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
+00001010: 6c61 7465 7374 2f69 6e73 7461 6c6c 6174  latest/installat
+00001020: 696f 6e2f 2920 746f 2063 6f72 7265 6374  ion/) to correct
+00001030: 6c79 2061 6464 2056 616c 6964 6974 7920  ly add Validity 
+00001040: 746f 2079 6f75 7220 4e65 7442 6f78 2e0a  to your NetBox..
+00001050: 3c21 2d2d 6d6b 646f 6373 2d65 6e64 2d2d  <!--mkdocs-end--
+00001060: 3e0a 0a23 2320 446f 6375 6d65 6e74 6174  >..## Documentat
+00001070: 696f 6e0a 5265 6164 2074 6865 2066 756c  ion.Read the ful
+00001080: 6c20 646f 6375 6d65 6e74 6174 696f 6e20  l documentation 
+00001090: 6f6e 205b 7661 6c69 6469 7479 2e72 6561  on [validity.rea
+000010a0: 6474 6865 646f 6373 2e69 6f5d 2868 7474  dthedocs.io](htt
+000010b0: 7073 3a2f 2f76 616c 6964 6974 792e 7265  ps://validity.re
+000010c0: 6164 7468 6564 6f63 732e 696f 290a 0a0a  adthedocs.io)...
+000010d0: 2323 2051 7569 636b 2053 7461 7274 0a0a  ## Quick Start..
+000010e0: 5468 6520 7368 6f72 7420 7669 6465 6f20  The short video 
+000010f0: 6162 6f75 7420 6669 7273 7420 7374 6570  about first step
+00001100: 7320 7769 7468 2056 616c 6964 6974 793a  s with Validity:
+00001110: 0a0a 5b21 5b57 6174 6368 2074 6865 2076  ..[![Watch the v
+00001120: 6964 656f 5d28 6874 7470 733a 2f2f 696d  ideo](https://im
+00001130: 672e 796f 7574 7562 652e 636f 6d2f 7669  g.youtube.com/vi
+00001140: 2f48 7332 4955 4536 724b 4334 2f30 2e6a  /Hs2IUE6rKC4/0.j
+00001150: 7067 295d 2868 7474 7073 3a2f 2f79 6f75  pg)](https://you
+00001160: 7475 2e62 652f 4873 3249 5545 3672 4b43  tu.be/Hs2IUE6rKC
+00001170: 3429 0a0a 2323 2043 6f6e 7472 6962 7574  4)..## Contribut
+00001180: 696e 670a 0a46 6565 6c20 6672 6565 2074  ing..Feel free t
+00001190: 6f20 6173 6b20 6120 5b51 7565 7374 696f  o ask a [Questio
+000011a0: 6e5d 2868 7474 7073 3a2f 2f67 6974 6875  n](https://githu
+000011b0: 622e 636f 6d2f 616d 7961 736e 696b 6f76  b.com/amyasnikov
+000011c0: 2f76 616c 6964 6974 792f 6469 7363 7573  /validity/discus
+000011d0: 7369 6f6e 7329 2c20 7265 706f 7274 2061  sions), report a
+000011e0: 6e20 5b49 7373 7565 5d28 6874 7470 733a  n [Issue](https:
+000011f0: 2f2f 6769 7468 7562 2e63 6f6d 2f61 6d79  //github.com/amy
+00001200: 6173 6e69 6b6f 762f 7661 6c69 6469 7479  asnikov/validity
+00001210: 2f69 7373 7565 7329 206f 7220 6576 656e  /issues) or even
+00001220: 206d 616b 6520 6120 5b50 525d 2843 4f4e   make a [PR](CON
+00001230: 5452 4942 5554 494e 472e 6d64 292e 2052  TRIBUTING.md). R
+00001240: 6561 6420 6d6f 7265 2061 626f 7574 2063  ead more about c
+00001250: 6f6e 7472 6962 7574 696f 6e20 696e 2074  ontribution in t
+00001260: 6865 205b 434f 4e54 5249 4255 5449 4e47  he [CONTRIBUTING
+00001270: 5d28 434f 4e54 5249 4255 5449 4e47 2e6d  ](CONTRIBUTING.m
+00001280: 6429 2067 7569 6465 2e0a                 d) guide..
```

### Comparing `netbox-validity-1.2.0/netbox_validity.egg-info/PKG-INFO` & `netbox-validity-1.2.1/netbox_validity.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6e65 7462  : 2.1.Name: netb
 00000020: 6f78 2d76 616c 6964 6974 790a 5665 7273  ox-validity.Vers
-00000030: 696f 6e3a 2031 2e32 2e30 0a53 756d 6d61  ion: 1.2.0.Summa
+00000030: 696f 6e3a 2031 2e32 2e31 0a53 756d 6d61  ion: 1.2.1.Summa
 00000040: 7279 3a20 4e65 7442 6f78 2070 6c75 6769  ry: NetBox plugi
 00000050: 6e20 666f 7220 7665 6e64 6f72 2d61 676e  n for vendor-agn
 00000060: 6f73 7469 6320 636f 6e66 6967 7572 6174  ostic configurat
 00000070: 696f 6e20 636f 6d70 6c69 616e 6365 0a41  ion compliance.A
 00000080: 7574 686f 722d 656d 6169 6c3a 2041 6e74  uthor-email: Ant
 00000090: 6f6e 204d 6961 736e 696b 6f76 203c 616e  on Miasnikov <an
 000000a0: 746f 6e32 3030 386d 4067 6d61 696c 2e63  ton2008m@gmail.c
@@ -137,269 +137,304 @@
 00000880: 6e3a 203e 3d33 2e31 300a 4465 7363 7269  n: >=3.10.Descri
 00000890: 7074 696f 6e2d 436f 6e74 656e 742d 5479  ption-Content-Ty
 000008a0: 7065 3a20 7465 7874 2f6d 6172 6b64 6f77  pe: text/markdow
 000008b0: 6e0a 5072 6f76 6964 6573 2d45 7874 7261  n.Provides-Extra
 000008c0: 3a20 6465 760a 5072 6f76 6964 6573 2d45  : dev.Provides-E
 000008d0: 7874 7261 3a20 646f 6373 0a4c 6963 656e  xtra: docs.Licen
 000008e0: 7365 2d46 696c 653a 204c 4943 454e 5345  se-File: LICENSE
-000008f0: 0a0a 2320 5661 6c69 6469 7479 3a20 7665  ..# Validity: ve
-00000900: 6e64 6f72 2d61 676e 6f73 7469 6320 636f  ndor-agnostic co
-00000910: 6e66 6967 7572 6174 696f 6e20 636f 6d70  nfiguration comp
-00000920: 6c69 616e 6365 0a0a 215b 4349 5d28 6874  liance..![CI](ht
-00000930: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000940: 2f61 6d79 6173 6e69 6b6f 762f 7661 6c69  /amyasnikov/vali
-00000950: 6469 7479 2f61 6374 696f 6e73 2f77 6f72  dity/actions/wor
-00000960: 6b66 6c6f 7773 2f63 692e 796d 6c2f 6261  kflows/ci.yml/ba
-00000970: 6467 652e 7376 6729 0a21 5b43 6f76 6572  dge.svg).![Cover
-00000980: 6167 655d 2868 7474 7073 3a2f 2f69 6d67  age](https://img
-00000990: 2e73 6869 656c 6473 2e69 6f2f 656e 6470  .shields.io/endp
-000009a0: 6f69 6e74 3f75 726c 3d68 7474 7073 3a2f  oint?url=https:/
-000009b0: 2f67 6973 742e 6769 7468 7562 7573 6572  /gist.githubuser
-000009c0: 636f 6e74 656e 742e 636f 6d2f 616d 7961  content.com/amya
-000009d0: 736e 696b 6f76 2f39 6535 3138 6165 3862  snikov/9e518ae8b
-000009e0: 6162 6431 3862 3765 6464 3865 6535 6161  abd18b7edd8ee5aa
-000009f0: 6435 3831 3436 622f 7261 772f 636f 762e  d58146b/raw/cov.
-00000a00: 6a73 6f6e 290a 215b 5079 7468 6f6e 2076  json).![Python v
-00000a10: 6572 7369 6f6e 5d28 6874 7470 733a 2f2f  ersion](https://
-00000a20: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
-00000a30: 6164 6765 2f50 7974 686f 6e2d 332e 3130  adge/Python-3.10
-00000a40: 2b2d 626c 7565 2e73 7667 290a 215b 4e65  +-blue.svg).![Ne
-00000a50: 7442 6f78 2076 6572 7369 6f6e 5d28 6874  tBox version](ht
-00000a60: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-00000a70: 732e 696f 2f62 6164 6765 2f4e 6574 426f  s.io/badge/NetBo
-00000a80: 782d 332e 347c 332e 352d 626c 7565 2e73  x-3.4|3.5-blue.s
-00000a90: 7667 290a 0a3c 212d 2d6d 6b64 6f63 732d  vg)..<!--mkdocs-
-00000aa0: 7374 6172 742d 2d3e 0a23 2320 5768 6174  start-->.## What
-00000ab0: 3f0a 5661 6c69 6469 7479 2069 7320 7468  ?.Validity is th
-00000ac0: 6520 5b4e 6574 426f 785d 2868 7474 7073  e [NetBox](https
-00000ad0: 3a2f 2f6e 6574 626f 782e 6465 7629 2070  ://netbox.dev) p
-00000ae0: 6c75 6769 6e20 746f 2064 6561 6c20 7769  lugin to deal wi
-00000af0: 7468 2063 6f6e 6669 6775 7261 7469 6f6e  th configuration
-00000b00: 2063 6f6d 706c 6961 6e63 652e 2059 6f75   compliance. You
-00000b10: 2064 6566 696e 6520 636f 6d70 6c69 616e   define complian
-00000b20: 6365 2074 6573 7473 2061 6e64 2056 616c  ce tests and Val
-00000b30: 6964 6974 7920 6368 6563 6b73 206e 6574  idity checks net
-00000b40: 776f 726b 2064 6576 6963 6520 636f 6e66  work device conf
-00000b50: 6967 7572 6174 696f 6e20 6669 6c65 7320  iguration files 
-00000b60: 6167 6169 6e73 7420 7468 6573 6520 7465  against these te
-00000b70: 7374 732e 2041 7320 6120 7265 7375 6c74  sts. As a result
-00000b80: 2079 6f75 2063 616e 2066 696e 6420 6f75   you can find ou
-00000b90: 7420 7768 6963 6820 6465 7669 6365 7320  t which devices 
-00000ba0: 6172 6520 7072 6f76 6973 696f 6e65 6420  are provisioned 
-00000bb0: 7072 6f70 6572 6c79 2028 6163 636f 7264  properly (accord
-00000bc0: 696e 6720 746f 2074 6865 2074 6573 7473  ing to the tests
-00000bd0: 2079 6f75 2068 6176 6520 7772 6974 7465   you have writte
-00000be0: 6e29 2061 6e64 2077 6869 6368 2061 7265  n) and which are
-00000bf0: 206e 6f74 2e0a 0a54 6f20 7573 6520 7661   not...To use va
-00000c00: 6c69 6469 7479 2079 6f75 206e 6565 643a  lidity you need:
-00000c10: 0a0a 312e 2053 746f 7265 2063 6f6e 6669  ..1. Store confi
-00000c20: 6775 7261 7469 6f6e 2066 696c 6573 206f  guration files o
-00000c30: 6620 796f 7572 2064 6576 6963 6573 2069  f your devices i
-00000c40: 6e20 6120 4769 7420 7265 706f 7369 746f  n a Git reposito
-00000c50: 7279 2e20 5661 6c69 6469 7479 2064 6f65  ry. Validity doe
-00000c60: 7320 6e6f 7420 636f 6c6c 6563 7420 7468  s not collect th
-00000c70: 6520 636f 6e66 6967 7320 6672 6f6d 2079  e configs from y
-00000c80: 6f75 7220 6e65 7477 6f72 6b2c 2079 6f75  our network, you
-00000c90: 2068 6176 6520 746f 2064 6f20 6974 2062   have to do it b
-00000ca0: 7920 7468 6972 642d 7061 7274 7920 746f  y third-party to
-00000cb0: 6f6c 2028 652e 672e 205b 6f78 6964 697a  ol (e.g. [oxidiz
-00000cc0: 6564 5d28 6874 7470 733a 2f2f 6769 7468  ed](https://gith
-00000cd0: 7562 2e63 6f6d 2f79 7474 692f 6f78 6964  ub.com/ytti/oxid
-00000ce0: 697a 6564 2929 2e0a 0a32 2e20 4465 6669  ized))...2. Defi
-00000cf0: 6e65 205b 5454 5020 5465 6d70 6c61 7465  ne [TTP Template
-00000d00: 5d28 6874 7470 733a 2f2f 7474 702e 7265  ](https://ttp.re
-00000d10: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
-00000d20: 6c61 7465 7374 2f29 2074 6f20 7472 616e  latest/) to tran
-00000d30: 736c 6174 6520 7468 6520 636f 6e66 6967  slate the config
-00000d40: 2066 726f 6d20 7665 6e64 6f72 2073 7065   from vendor spe
-00000d50: 6369 6669 6320 666f 726d 6174 2069 6e74  cific format int
-00000d60: 6f20 4a53 4f4e 2e0a 0a33 2e20 5772 6974  o JSON...3. Writ
-00000d70: 6520 636f 6d70 6c69 616e 6365 2074 6573  e compliance tes
-00000d80: 7420 6173 2061 2070 7974 686f 6e20 6578  t as a python ex
-00000d90: 7072 6573 7369 6f6e 2c20 652e 672e 3c62  pression, e.g.<b
-00000da0: 722f 3e0a 6064 6576 6963 652e 636f 6e66  r/>.`device.conf
-00000db0: 6967 5b22 6e74 702d 7365 7276 6572 7322  ig["ntp-servers"
-00000dc0: 5d20 3d3d 205b 2231 2e32 2e33 2e34 222c  ] == ["1.2.3.4",
-00000dd0: 2022 352e 362e 372e 3822 5d60 0a0a 342e   "5.6.7.8"]`..4.
-00000de0: 2041 7070 6c79 2063 7265 6174 6564 2074   Apply created t
-00000df0: 6573 7420 746f 2073 7065 6369 6669 6320  est to specific 
-00000e00: 6465 7669 6365 7320 616e 6420 6765 7420  devices and get 
-00000e10: 7468 6520 7265 7375 6c74 7320 7065 7220  the results per 
-00000e20: 6465 7669 6365 2028 7061 7373 6564 206f  device (passed o
-00000e30: 7220 6661 696c 6564 292e 0a0a 0a23 2320  r failed)....## 
-00000e40: 5768 793f 0a43 6f6e 6669 6775 7261 7469  Why?.Configurati
-00000e50: 6f6e 2063 6f6d 706c 6961 6e63 6520 6973  on compliance is
-00000e60: 206f 6e65 206f 6620 7468 6520 7665 7279   one of the very
-00000e70: 2063 6f6d 6d6f 6e20 7072 6f62 6c65 6d73   common problems
-00000e80: 2074 6861 7420 6172 6973 6573 2069 6e20   that arises in 
-00000e90: 6576 6572 7920 636f 6d70 616e 7920 7769  every company wi
-00000ea0: 7468 2074 6865 2067 726f 7774 6820 6f66  th the growth of
-00000eb0: 2074 6865 6972 206e 6574 776f 726b 2e20   their network. 
-00000ec0: 5573 7561 6c6c 7920 636f 6d70 616e 6965  Usually companie
-00000ed0: 7320 736f 6c76 6520 7468 6973 2070 726f  s solve this pro
-00000ee0: 626c 656d 2077 6974 6820 736f 6d65 206b  blem with some k
-00000ef0: 696e 6420 6f66 2073 6372 6970 7473 2074  ind of scripts t
-00000f00: 6861 7420 646f 2061 6c6c 2074 6865 2074  hat do all the t
-00000f10: 6869 6e67 7320 6174 2074 6865 2073 616d  hings at the sam
-00000f20: 6520 7469 6d65 3a20 7468 6579 2070 6172  e time: they par
-00000f30: 7365 2063 6f6e 6669 6773 2c20 6170 706c  se configs, appl
-00000f40: 7920 736f 6d65 2063 6f6d 706c 6961 6e63  y some complianc
-00000f50: 6520 6c6f 6769 6320 616e 6420 7075 7368  e logic and push
-00000f60: 2074 6865 2072 6573 756c 7473 2069 6e74   the results int
-00000f70: 6f20 736f 6d65 2044 4220 6f72 2074 6869  o some DB or thi
-00000f80: 7264 2d70 6172 7479 204f 5353 2073 7973  rd-party OSS sys
-00000f90: 7465 6d2e 2055 7375 616c 6c79 2061 6674  tem. Usually aft
-00000fa0: 6572 2074 6865 2061 6464 6974 696f 6e20  er the addition 
-00000fb0: 6f66 2073 6576 6572 616c 2076 656e 646f  of several vendo
-00000fc0: 7273 2028 6f72 2065 7665 6e20 7365 7665  rs (or even seve
-00000fd0: 7261 6c20 736f 6674 7761 7265 2072 6576  ral software rev
-00000fe0: 6973 696f 6e73 206f 6620 6f6e 6520 6d6f  isions of one mo
-00000ff0: 6465 6c29 2074 6865 7365 2073 6372 6970  del) these scrip
-00001000: 7473 2062 6563 6f6d 6520 756e 7265 6164  ts become unread
-00001010: 6162 6c65 2061 6e64 2061 6c6d 6f73 7420  able and almost 
-00001020: 6e6f 206f 6e65 2063 616e 2064 6566 696e  no one can defin
-00001030: 6974 656c 7920 7361 7920 7768 6963 6820  itely say which 
-00001040: 7275 6c65 7320 7468 6520 7363 7269 7074  rules the script
-00001050: 2063 6865 636b 7320 666f 722e 0a0a 5661   checks for...Va
-00001060: 6c69 6469 7479 2063 6f6d 706c 6574 656c  lidity completel
-00001070: 7920 7365 7061 7261 7465 7320 636f 6d70  y separates comp
-00001080: 6c69 616e 6365 2074 6573 7420 636f 6465  liance test code
-00001090: 2066 726f 6d20 616c 6c20 6f74 6865 7220   from all other 
-000010a0: 7468 696e 6773 206c 696b 6520 636f 6e66  things like conf
-000010b0: 6967 2073 6572 6961 6c69 7a61 7469 6f6e  ig serialization
-000010c0: 2e20 5468 6973 206f 6e65 2065 6e63 6f75  . This one encou
-000010d0: 7261 6765 7320 796f 7520 746f 2077 7269  rages you to wri
-000010e0: 7465 2073 686f 7274 2c20 636c 6561 6e20  te short, clean 
-000010f0: 616e 6420 756e 6465 7273 7461 6e64 6162  and understandab
-00001100: 6c65 2063 6f6d 706c 6961 6e63 6520 7465  le compliance te
-00001110: 7374 7320 746f 6765 7468 6572 2077 6974  sts together wit
-00001120: 6820 7468 6520 6d61 6e64 6174 6f72 7920  h the mandatory 
-00001130: 6465 7363 7269 7074 696f 6e2e 0a0a 0a23  description....#
-00001140: 2320 4b65 7920 6665 6174 7572 6573 0a2a  # Key features.*
-00001150: 2054 7275 6c79 2076 656e 646f 722d 6167   Truly vendor-ag
-00001160: 6e6f 7374 6963 2e20 596f 7520 6361 6e20  nostic. You can 
-00001170: 6561 7369 6c79 2069 6e74 6567 7261 7465  easily integrate
-00001180: 2061 6e79 2076 656e 646f 7220 636f 6e66   any vendor conf
-00001190: 6967 2066 6f72 6d61 7420 7573 696e 6720  ig format using 
-000011a0: 5b54 5450 5d28 6874 7470 733a 2f2f 6769  [TTP](https://gi
-000011b0: 7468 7562 2e63 6f6d 2f64 6d75 6c79 616c  thub.com/dmulyal
-000011c0: 696e 2f74 7470 290a 2a20 5772 6974 696e  in/ttp).* Writin
-000011d0: 6720 636f 6d70 6c69 616e 6365 2074 6573  g compliance tes
-000011e0: 7473 2075 7369 6e67 2050 7974 686f 6e20  ts using Python 
-000011f0: 6578 7072 6573 7369 6f6e 7320 616e 6420  expressions and 
-00001200: 5b4a 515d 2868 7474 7073 3a2f 2f73 7465  [JQ](https://ste
-00001210: 646f 6c61 6e2e 6769 7468 7562 2e69 6f2f  dolan.github.io/
-00001220: 6a71 2f6d 616e 7561 6c2f 290a 2a20 466c  jq/manual/).* Fl
-00001230: 6578 6962 6c65 2073 656c 6563 746f 7220  exible selector 
-00001240: 7379 7374 656d 2074 6f20 6170 706c 7920  system to apply 
-00001250: 7468 6520 7465 7374 7320 6f6e 6c79 2074  the tests only t
-00001260: 6f20 6120 7370 6563 6966 6963 2073 7562  o a specific sub
-00001270: 7365 7420 6f66 2064 6576 6963 6573 0a2a  set of devices.*
-00001280: 2043 6f6e 6365 7074 206f 6620 2a2a 6479   Concept of **dy
-00001290: 6e61 6d69 6320 7061 6972 732a 2a2e 2057  namic pairs**. W
-000012a0: 6974 6820 6479 6e61 6d69 6320 7061 6972  ith dynamic pair
-000012b0: 2079 6f75 2063 616e 2063 6f6d 7061 7265   you can compare
-000012c0: 2032 2064 6966 6665 7265 6e74 2064 6576   2 different dev
-000012d0: 6963 6573 2062 6574 7765 656e 2065 6163  ices between eac
-000012e0: 6820 6f74 6865 7220 2865 2e67 2e20 636f  h other (e.g. co
-000012f0: 6d70 6172 6520 7468 6520 636f 6e66 6967  mpare the config
-00001300: 7572 6174 696f 6e20 6f66 2032 204d 432d  uration of 2 MC-
-00001310: 4c41 4720 6d65 6d62 6572 7329 2e0a 2a20  LAG members)..* 
-00001320: 2a2a 5465 7374 2072 6573 756c 7420 6578  **Test result ex
-00001330: 706c 616e 6174 696f 6e2a 2a2e 2057 6865  planation**. Whe
-00001340: 6e20 736f 6d65 2074 6573 7420 6661 696c  n some test fail
-00001350: 732c 2079 6f75 2063 616e 2067 6574 2074  s, you can get t
-00001360: 6865 202a 2a65 7870 6c61 6e61 7469 6f6e  he **explanation
-00001370: 2a2a 206f 6620 7468 6520 6361 6c63 756c  ** of the calcul
-00001380: 6174 696f 6e20 7072 6f63 6573 7320 7374  ation process st
-00001390: 6570 2062 7920 7374 6570 2e20 4974 2068  ep by step. It h
-000013a0: 656c 7073 2074 6f20 6964 656e 7469 6679  elps to identify
-000013b0: 2074 6865 2063 6175 7365 206f 6620 7468   the cause of th
-000013c0: 6520 6661 696c 7572 652e 0a2a 202a 2a4f  e failure..* **O
-000013d0: 524d 2061 6363 6573 732a 2a20 696e 7369  RM access** insi
-000013e0: 6465 2074 6865 2074 6573 742e 2059 6f75  de the test. You
-000013f0: 2068 6176 6520 6675 6c6c 2061 6363 6573   have full acces
-00001400: 7320 746f 2074 6865 202a 2a64 6576 6963  s to the **devic
-00001410: 652a 2a20 7072 6f70 6572 7469 6573 2e20  e** properties. 
-00001420: 466f 7220 696e 7374 616e 6365 2c20 796f  For instance, yo
-00001430: 7520 6d61 7920 6c65 7665 7261 6765 205b  u may leverage [
-00001440: 436f 6e66 6967 7572 6174 696f 6e20 436f  Configuration Co
-00001450: 6e74 6578 7473 5d28 6874 7470 733a 2f2f  ntexts](https://
-00001460: 646f 6373 2e6e 6574 626f 782e 6465 762f  docs.netbox.dev/
-00001470: 656e 2f73 7461 626c 652f 6665 6174 7572  en/stable/featur
-00001480: 6573 2f63 6f6e 7465 7874 2d64 6174 612f  es/context-data/
-00001490: 2920 4e65 7442 6f78 2066 6561 7475 7265  ) NetBox feature
-000014a0: 2074 6f20 7374 6f72 6520 796f 7572 2064   to store your d
-000014b0: 6573 6972 6564 2063 6f6e 6669 6775 7261  esired configura
-000014c0: 7469 6f6e 2061 6e64 2063 6f6d 7061 7265  tion and compare
-000014d0: 2069 7420 7769 7468 2074 6865 2063 6f6e   it with the con
-000014e0: 6669 6720 636f 6c6c 6563 7465 6420 6672  fig collected fr
-000014f0: 6f6d 2074 6865 2064 6576 6963 652e 0a2a  om the device..*
-00001500: 202a 2a52 6570 6f72 7473 2061 6e64 2077   **Reports and w
-00001510: 6562 686f 6f6b 732a 2a2e 2041 6674 6572  ebhooks**. After
-00001520: 2065 7865 6375 7469 6f6e 206f 6620 736f   execution of so
-00001530: 6d65 2062 756e 6368 206f 6620 7465 7374  me bunch of test
-00001540: 7320 796f 7520 6361 6e20 6765 7420 7468  s you can get th
-00001550: 6520 7265 706f 7274 2077 6974 6820 7061  e report with pa
-00001560: 7373 6564 2f66 6169 6c65 6420 7374 6174  ssed/failed stat
-00001570: 6973 7469 6373 2067 726f 7570 6564 2062  istics grouped b
-00001580: 7920 736f 6d65 204c 6f63 6174 696f 6e2f  y some Location/
-00001590: 5369 7465 2f4d 616e 7566 6163 7475 7265  Site/Manufacture
-000015a0: 722f 6574 632e 204d 6f72 656f 7665 722c  r/etc. Moreover,
-000015b0: 2079 6f75 2063 616e 2070 726f 7669 7369   you can provisi
-000015c0: 6f6e 2074 6865 2077 6562 686f 6f6b 2074  on the webhook t
-000015d0: 6f20 6e6f 7469 6679 2061 6e20 6578 7465  o notify an exte
-000015e0: 726e 616c 2073 7973 7465 6d20 7768 656e  rnal system when
-000015f0: 2063 6f6d 706c 6961 6e63 6520 7265 706f   compliance repo
-00001600: 7274 2069 7320 6765 6e65 7261 7465 642e  rt is generated.
-00001610: 0a2a 202a 2a54 6573 7420 6578 7465 6e73  .* **Test extens
-00001620: 6962 696c 6974 792a 2a2e 2059 6f75 2063  ibility**. You c
-00001630: 616e 2064 6566 696e 6520 796f 7572 206f  an define your o
-00001640: 776e 2070 7974 686f 6e20 6675 6e63 7469  wn python functi
-00001650: 6f6e 7320 6f72 2063 6c61 7373 6573 2074  ons or classes t
-00001660: 6f20 7265 7573 6520 7468 6520 636f 6465  o reuse the code
-00001670: 2062 6574 7765 656e 206d 756c 7469 706c   between multipl
-00001680: 6520 636f 6d70 6c69 616e 6365 2074 6573  e compliance tes
-00001690: 7473 2e0a 2a20 506f 7373 6962 696c 6974  ts..* Possibilit
-000016a0: 7920 746f 2073 746f 7265 2061 6c6c 2068  y to store all h
-000016b0: 6561 7679 2074 6578 742d 6261 7365 6420  eavy text-based 
-000016c0: 656e 7469 7469 6573 2028 6c69 6b65 2063  entities (like c
-000016d0: 6f6d 706c 6961 6e63 6520 7465 7374 7320  ompliance tests 
-000016e0: 6f72 2054 5450 2054 656d 706c 6174 6573  or TTP Templates
-000016f0: 2920 696e 2061 202a 2a47 6974 2072 6570  ) in a **Git rep
-00001700: 6f73 6974 6f72 792a 2a0a 3c21 2d2d 6d6b  ository**.<!--mk
-00001710: 646f 6373 2d65 6e64 2d2d 3e0a 0a23 2320  docs-end-->..## 
-00001720: 446f 6375 6d65 6e74 6174 696f 6e0a 5265  Documentation.Re
-00001730: 6164 2074 6865 2066 756c 6c20 646f 6375  ad the full docu
-00001740: 6d65 6e74 6174 696f 6e20 6f6e 205b 7661  mentation on [va
-00001750: 6c69 6469 7479 2e72 6561 6474 6865 646f  lidity.readthedo
-00001760: 6373 2e69 6f5d 2868 7474 7073 3a2f 2f76  cs.io](https://v
-00001770: 616c 6964 6974 792e 7265 6164 7468 6564  alidity.readthed
-00001780: 6f63 732e 696f 290a 0a0a 2323 2051 7569  ocs.io)...## Qui
-00001790: 636b 2053 7461 7274 0a0a 5468 6520 7368  ck Start..The sh
-000017a0: 6f72 7420 7669 6465 6f20 6162 6f75 7420  ort video about 
-000017b0: 6669 7273 7420 7374 6570 7320 7769 7468  first steps with
-000017c0: 2056 616c 6964 6974 793a 0a0a 5b21 5b57   Validity:..[![W
-000017d0: 6174 6368 2074 6865 2076 6964 656f 5d28  atch the video](
-000017e0: 6874 7470 733a 2f2f 696d 672e 796f 7574  https://img.yout
-000017f0: 7562 652e 636f 6d2f 7669 2f48 7332 4955  ube.com/vi/Hs2IU
-00001800: 4536 724b 4334 2f30 2e6a 7067 295d 2868  E6rKC4/0.jpg)](h
-00001810: 7474 7073 3a2f 2f79 6f75 7475 2e62 652f  ttps://youtu.be/
-00001820: 4873 3249 5545 3672 4b43 3429 0a0a 2323  Hs2IUE6rKC4)..##
-00001830: 2043 6f6e 7472 6962 7574 696e 670a 0a46   Contributing..F
-00001840: 6565 6c20 6672 6565 2074 6f20 6173 6b20  eel free to ask 
-00001850: 6120 5b51 7565 7374 696f 6e5d 2868 7474  a [Question](htt
-00001860: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00001870: 616d 7961 736e 696b 6f76 2f76 616c 6964  amyasnikov/valid
-00001880: 6974 792f 6469 7363 7573 7369 6f6e 7329  ity/discussions)
-00001890: 2c20 7265 706f 7274 2061 6e20 5b49 7373  , report an [Iss
-000018a0: 7565 5d28 6874 7470 733a 2f2f 6769 7468  ue](https://gith
-000018b0: 7562 2e63 6f6d 2f61 6d79 6173 6e69 6b6f  ub.com/amyasniko
-000018c0: 762f 7661 6c69 6469 7479 2f69 7373 7565  v/validity/issue
-000018d0: 7329 206f 7220 6576 656e 206d 616b 6520  s) or even make 
-000018e0: 6120 5b50 525d 2843 4f4e 5452 4942 5554  a [PR](CONTRIBUT
-000018f0: 494e 472e 6d64 292e 2052 6561 6420 6d6f  ING.md). Read mo
-00001900: 7265 2061 626f 7574 2063 6f6e 7472 6962  re about contrib
-00001910: 7574 696f 6e20 696e 2074 6865 205b 434f  ution in the [CO
-00001920: 4e54 5249 4255 5449 4e47 5d28 434f 4e54  NTRIBUTING](CONT
-00001930: 5249 4255 5449 4e47 2e6d 6429 2067 7569  RIBUTING.md) gui
-00001940: 6465 2e0a                                de..
+000008f0: 0a0a 3c64 6976 2061 6c69 676e 3d22 6365  ..<div align="ce
+00000900: 6e74 6572 223e 0a20 2020 203c 6120 6872  nter">.    <a hr
+00000910: 6566 3d22 6874 7470 733a 2f2f 7661 6c69  ef="https://vali
+00000920: 6469 7479 2e72 6561 6474 6865 646f 6373  dity.readthedocs
+00000930: 2e69 6f22 3e3c 696d 6720 7372 633d 2268  .io"><img src="h
+00000940: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
+00000950: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
+00000960: 2f61 6d79 6173 6e69 6b6f 762f 7661 6c69  /amyasnikov/vali
+00000970: 6469 7479 2f6d 6173 7465 722f 646f 6373  dity/master/docs
+00000980: 2f76 616c 6964 6974 795f 6c6f 676f 2e70  /validity_logo.p
+00000990: 6e67 2220 616c 743d 2243 6c69 636b 2074  ng" alt="Click t
+000009a0: 6f20 7669 6577 2056 616c 6964 6974 7920  o view Validity 
+000009b0: 646f 6373 222f 3e3c 2f61 3e0a 2020 2020  docs"/></a>.    
+000009c0: 3c68 313e 5661 6c69 6469 7479 3a20 7665  <h1>Validity: ve
+000009d0: 6e64 6f72 2d61 676e 6f73 7469 6320 636f  ndor-agnostic co
+000009e0: 6e66 6967 7572 6174 696f 6e20 636f 6d70  nfiguration comp
+000009f0: 6c69 616e 6365 3c2f 6831 3e0a 2020 2020  liance</h1>.    
+00000a00: 3c70 3e0a 2020 2020 2020 2020 3c69 6d67  <p>.        <img
+00000a10: 2073 7263 3d22 6874 7470 733a 2f2f 6769   src="https://gi
+00000a20: 7468 7562 2e63 6f6d 2f61 6d79 6173 6e69  thub.com/amyasni
+00000a30: 6b6f 762f 7661 6c69 6469 7479 2f61 6374  kov/validity/act
+00000a40: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f63  ions/workflows/c
+00000a50: 692e 796d 6c2f 6261 6467 652e 7376 6722  i.yml/badge.svg"
+00000a60: 2061 6c74 3d22 4349 223e 0a20 2020 2020   alt="CI">.     
+00000a70: 2020 203c 696d 6720 7372 633d 2268 7474     <img src="htt
+00000a80: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00000a90: 2e69 6f2f 656e 6470 6f69 6e74 3f75 726c  .io/endpoint?url
+00000aa0: 3d68 7474 7073 3a2f 2f67 6973 742e 6769  =https://gist.gi
+00000ab0: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
+00000ac0: 636f 6d2f 616d 7961 736e 696b 6f76 2f39  com/amyasnikov/9
+00000ad0: 6535 3138 6165 3862 6162 6431 3862 3765  e518ae8babd18b7e
+00000ae0: 6464 3865 6535 6161 6435 3831 3436 622f  dd8ee5aad58146b/
+00000af0: 7261 772f 636f 762e 6a73 6f6e 2220 616c  raw/cov.json" al
+00000b00: 743d 2243 6f76 6572 6167 6522 3e0a 2020  t="Coverage">.  
+00000b10: 2020 2020 2020 3c69 6d67 2073 7263 3d22        <img src="
+00000b20: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000b30: 6c64 732e 696f 2f62 6164 6765 2f50 7974  lds.io/badge/Pyt
+00000b40: 686f 6e2d 332e 3130 2b2d 626c 7565 2e73  hon-3.10+-blue.s
+00000b50: 7667 2220 616c 743d 2250 7974 686f 6e20  vg" alt="Python 
+00000b60: 7665 7273 696f 6e22 3e0a 2020 2020 2020  version">.      
+00000b70: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
+00000b80: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000b90: 696f 2f62 6164 6765 2f4e 6574 426f 782d  io/badge/NetBox-
+00000ba0: 332e 347c 332e 352d 626c 7565 2e73 7667  3.4|3.5-blue.svg
+00000bb0: 2220 616c 743d 224e 6574 426f 7820 7665  " alt="NetBox ve
+00000bc0: 7273 696f 6e22 3e0a 2020 2020 3c2f 703e  rsion">.    </p>
+00000bd0: 0a3c 2f64 6976 3e0a 0a3c 212d 2d6d 6b64  .</div>..<!--mkd
+00000be0: 6f63 732d 7374 6172 742d 2d3e 0a23 2320  ocs-start-->.## 
+00000bf0: 5768 6174 3f0a 5661 6c69 6469 7479 2069  What?.Validity i
+00000c00: 7320 7468 6520 5b4e 6574 426f 785d 2868  s the [NetBox](h
+00000c10: 7474 7073 3a2f 2f6e 6574 626f 782e 6465  ttps://netbox.de
+00000c20: 7629 2070 6c75 6769 6e20 746f 2077 7269  v) plugin to wri
+00000c30: 7465 2022 6175 746f 2074 6573 7473 2220  te "auto tests" 
+00000c40: 666f 7220 636f 6e66 6967 7572 6174 696f  for configuratio
+00000c50: 6e2e 2059 6f75 2064 6566 696e 6520 636f  n. You define co
+00000c60: 6d70 6c69 616e 6365 2074 6573 7473 2061  mpliance tests a
+00000c70: 6e64 2056 616c 6964 6974 7920 6368 6563  nd Validity chec
+00000c80: 6b73 206e 6574 776f 726b 2064 6576 6963  ks network devic
+00000c90: 6520 636f 6e66 6967 7572 6174 696f 6e20  e configuration 
+00000ca0: 6669 6c65 7320 6167 6169 6e73 7420 7468  files against th
+00000cb0: 6573 6520 7465 7374 732e 2041 7320 6120  ese tests. As a 
+00000cc0: 7265 7375 6c74 2079 6f75 2063 616e 2066  result you can f
+00000cd0: 696e 6420 6f75 7420 7768 6963 6820 6465  ind out which de
+00000ce0: 7669 6365 7320 6172 6520 7072 6f76 6973  vices are provis
+00000cf0: 696f 6e65 6420 7072 6f70 6572 6c79 2028  ioned properly (
+00000d00: 6163 636f 7264 696e 6720 746f 2074 6865  according to the
+00000d10: 2074 6573 7473 2079 6f75 2068 6176 6520   tests you have 
+00000d20: 7772 6974 7465 6e29 2061 6e64 2077 6869  written) and whi
+00000d30: 6368 2061 7265 206e 6f74 2e0a 0a54 6f20  ch are not...To 
+00000d40: 7573 6520 7661 6c69 6469 7479 2079 6f75  use validity you
+00000d50: 206e 6565 643a 0a0a 312e 2053 746f 7265   need:..1. Store
+00000d60: 2063 6f6e 6669 6775 7261 7469 6f6e 2066   configuration f
+00000d70: 696c 6573 206f 6620 796f 7572 2064 6576  iles of your dev
+00000d80: 6963 6573 2069 6e20 6120 4769 7420 7265  ices in a Git re
+00000d90: 706f 7369 746f 7279 2e20 5661 6c69 6469  pository. Validi
+00000da0: 7479 2064 6f65 7320 6e6f 7420 636f 6c6c  ty does not coll
+00000db0: 6563 7420 7468 6520 636f 6e66 6967 7320  ect the configs 
+00000dc0: 6672 6f6d 2079 6f75 7220 6e65 7477 6f72  from your networ
+00000dd0: 6b2c 2079 6f75 2068 6176 6520 746f 2064  k, you have to d
+00000de0: 6f20 6974 2062 7920 7468 6972 642d 7061  o it by third-pa
+00000df0: 7274 7920 746f 6f6c 2028 652e 672e 205b  rty tool (e.g. [
+00000e00: 6f78 6964 697a 6564 5d28 6874 7470 733a  oxidized](https:
+00000e10: 2f2f 6769 7468 7562 2e63 6f6d 2f79 7474  //github.com/ytt
+00000e20: 692f 6f78 6964 697a 6564 2929 2e0a 0a32  i/oxidized))...2
+00000e30: 2e20 4465 6669 6e65 205b 5454 5020 5465  . Define [TTP Te
+00000e40: 6d70 6c61 7465 5d28 6874 7470 733a 2f2f  mplate](https://
+00000e50: 7474 702e 7265 6164 7468 6564 6f63 732e  ttp.readthedocs.
+00000e60: 696f 2f65 6e2f 6c61 7465 7374 2f29 2074  io/en/latest/) t
+00000e70: 6f20 7472 616e 736c 6174 6520 7468 6520  o translate the 
+00000e80: 636f 6e66 6967 2066 726f 6d20 7665 6e64  config from vend
+00000e90: 6f72 2073 7065 6369 6669 6320 666f 726d  or specific form
+00000ea0: 6174 2069 6e74 6f20 4a53 4f4e 2e0a 0a33  at into JSON...3
+00000eb0: 2e20 5772 6974 6520 636f 6d70 6c69 616e  . Write complian
+00000ec0: 6365 2074 6573 7420 6173 2061 2070 7974  ce test as a pyt
+00000ed0: 686f 6e20 6578 7072 6573 7369 6f6e 2c20  hon expression, 
+00000ee0: 652e 672e 3c62 722f 3e0a 6064 6576 6963  e.g.<br/>.`devic
+00000ef0: 652e 636f 6e66 6967 5b22 6e74 702d 7365  e.config["ntp-se
+00000f00: 7276 6572 7322 5d20 3d3d 205b 2231 2e32  rvers"] == ["1.2
+00000f10: 2e33 2e34 222c 2022 352e 362e 372e 3822  .3.4", "5.6.7.8"
+00000f20: 5d60 0a0a 342e 2041 7070 6c79 2063 7265  ]`..4. Apply cre
+00000f30: 6174 6564 2074 6573 7420 746f 2073 7065  ated test to spe
+00000f40: 6369 6669 6320 6465 7669 6365 7320 616e  cific devices an
+00000f50: 6420 6765 7420 7468 6520 7265 7375 6c74  d get the result
+00000f60: 7320 7065 7220 6465 7669 6365 2028 7061  s per device (pa
+00000f70: 7373 6564 206f 7220 6661 696c 6564 292e  ssed or failed).
+00000f80: 0a0a 0a23 2320 5768 793f 0a43 6f6e 6669  ...## Why?.Confi
+00000f90: 6775 7261 7469 6f6e 2063 6f6d 706c 6961  guration complia
+00000fa0: 6e63 6520 6973 206f 6e65 206f 6620 7468  nce is one of th
+00000fb0: 6520 7665 7279 2063 6f6d 6d6f 6e20 7072  e very common pr
+00000fc0: 6f62 6c65 6d73 2074 6861 7420 6172 6973  oblems that aris
+00000fd0: 6573 2069 6e20 6576 6572 7920 636f 6d70  es in every comp
+00000fe0: 616e 7920 7769 7468 2074 6865 2067 726f  any with the gro
+00000ff0: 7774 6820 6f66 2074 6865 6972 206e 6574  wth of their net
+00001000: 776f 726b 2e20 5573 7561 6c6c 7920 636f  work. Usually co
+00001010: 6d70 616e 6965 7320 736f 6c76 6520 7468  mpanies solve th
+00001020: 6973 2070 726f 626c 656d 2077 6974 6820  is problem with 
+00001030: 736f 6d65 206b 696e 6420 6f66 2073 6372  some kind of scr
+00001040: 6970 7473 2074 6861 7420 646f 2061 6c6c  ipts that do all
+00001050: 2074 6865 2074 6869 6e67 7320 6174 2074   the things at t
+00001060: 6865 2073 616d 6520 7469 6d65 3a20 7468  he same time: th
+00001070: 6579 2070 6172 7365 2063 6f6e 6669 6773  ey parse configs
+00001080: 2c20 6170 706c 7920 736f 6d65 2063 6f6d  , apply some com
+00001090: 706c 6961 6e63 6520 6c6f 6769 6320 616e  pliance logic an
+000010a0: 6420 7075 7368 2074 6865 2072 6573 756c  d push the resul
+000010b0: 7473 2069 6e74 6f20 736f 6d65 2044 4220  ts into some DB 
+000010c0: 6f72 2074 6869 7264 2d70 6172 7479 204f  or third-party O
+000010d0: 5353 2073 7973 7465 6d2e 2055 7375 616c  SS system. Usual
+000010e0: 6c79 2061 6674 6572 2074 6865 2061 6464  ly after the add
+000010f0: 6974 696f 6e20 6f66 2073 6576 6572 616c  ition of several
+00001100: 2076 656e 646f 7273 2028 6f72 2065 7665   vendors (or eve
+00001110: 6e20 7365 7665 7261 6c20 736f 6674 7761  n several softwa
+00001120: 7265 2072 6576 6973 696f 6e73 206f 6620  re revisions of 
+00001130: 6f6e 6520 6d6f 6465 6c29 2074 6865 7365  one model) these
+00001140: 2073 6372 6970 7473 2062 6563 6f6d 6520   scripts become 
+00001150: 756e 7265 6164 6162 6c65 2061 6e64 2061  unreadable and a
+00001160: 6c6d 6f73 7420 6e6f 206f 6e65 2063 616e  lmost no one can
+00001170: 2064 6566 696e 6974 656c 7920 7361 7920   definitely say 
+00001180: 7768 6963 6820 7275 6c65 7320 7468 6520  which rules the 
+00001190: 7363 7269 7074 2063 6865 636b 7320 666f  script checks fo
+000011a0: 722e 0a0a 5661 6c69 6469 7479 2063 6f6d  r...Validity com
+000011b0: 706c 6574 656c 7920 7365 7061 7261 7465  pletely separate
+000011c0: 7320 636f 6d70 6c69 616e 6365 2074 6573  s compliance tes
+000011d0: 7420 636f 6465 2066 726f 6d20 616c 6c20  t code from all 
+000011e0: 6f74 6865 7220 7468 696e 6773 206c 696b  other things lik
+000011f0: 6520 636f 6e66 6967 2073 6572 6961 6c69  e config seriali
+00001200: 7a61 7469 6f6e 2e20 5468 6973 206f 6e65  zation. This one
+00001210: 2065 6e63 6f75 7261 6765 7320 796f 7520   encourages you 
+00001220: 746f 2077 7269 7465 2073 686f 7274 2c20  to write short, 
+00001230: 636c 6561 6e20 616e 6420 756e 6465 7273  clean and unders
+00001240: 7461 6e64 6162 6c65 2063 6f6d 706c 6961  tandable complia
+00001250: 6e63 6520 7465 7374 7320 746f 6765 7468  nce tests togeth
+00001260: 6572 2077 6974 6820 7468 6520 6d61 6e64  er with the mand
+00001270: 6174 6f72 7920 6465 7363 7269 7074 696f  atory descriptio
+00001280: 6e2e 0a0a 0a23 2320 4b65 7920 4665 6174  n....## Key Feat
+00001290: 7572 6573 0a2a 2054 7275 6c79 2076 656e  ures.* Truly ven
+000012a0: 646f 722d 6167 6e6f 7374 6963 2e20 596f  dor-agnostic. Yo
+000012b0: 7520 6361 6e20 6561 7369 6c79 2069 6e74  u can easily int
+000012c0: 6567 7261 7465 2061 6e79 2076 656e 646f  egrate any vendo
+000012d0: 7220 636f 6e66 6967 2066 6f72 6d61 7420  r config format 
+000012e0: 7573 696e 6720 5b54 5450 5d28 6874 7470  using [TTP](http
+000012f0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f64  s://github.com/d
+00001300: 6d75 6c79 616c 696e 2f74 7470 290a 2a20  mulyalin/ttp).* 
+00001310: 5772 6974 696e 6720 636f 6d70 6c69 616e  Writing complian
+00001320: 6365 2074 6573 7473 2075 7369 6e67 2050  ce tests using P
+00001330: 7974 686f 6e20 6578 7072 6573 7369 6f6e  ython expression
+00001340: 7320 616e 6420 5b4a 515d 2868 7474 7073  s and [JQ](https
+00001350: 3a2f 2f73 7465 646f 6c61 6e2e 6769 7468  ://stedolan.gith
+00001360: 7562 2e69 6f2f 6a71 2f6d 616e 7561 6c2f  ub.io/jq/manual/
+00001370: 290a 2a20 466c 6578 6962 6c65 2073 656c  ).* Flexible sel
+00001380: 6563 746f 7220 7379 7374 656d 2074 6f20  ector system to 
+00001390: 6170 706c 7920 7468 6520 7465 7374 7320  apply the tests 
+000013a0: 6f6e 6c79 2074 6f20 6120 7370 6563 6966  only to a specif
+000013b0: 6963 2073 7562 7365 7420 6f66 2064 6576  ic subset of dev
+000013c0: 6963 6573 0a2a 2043 6f6e 6365 7074 206f  ices.* Concept o
+000013d0: 6620 2a2a 6479 6e61 6d69 6320 7061 6972  f **dynamic pair
+000013e0: 732a 2a2e 2057 6974 6820 6479 6e61 6d69  s**. With dynami
+000013f0: 6320 7061 6972 2079 6f75 2063 616e 2063  c pair you can c
+00001400: 6f6d 7061 7265 2032 2064 6966 6665 7265  ompare 2 differe
+00001410: 6e74 2064 6576 6963 6573 2062 6574 7765  nt devices betwe
+00001420: 656e 2065 6163 6820 6f74 6865 7220 2865  en each other (e
+00001430: 2e67 2e20 636f 6d70 6172 6520 7468 6520  .g. compare the 
+00001440: 636f 6e66 6967 7572 6174 696f 6e20 6f66  configuration of
+00001450: 2032 204d 432d 4c41 4720 6d65 6d62 6572   2 MC-LAG member
+00001460: 7329 2e0a 2a20 2a2a 5465 7374 2072 6573  s)..* **Test res
+00001470: 756c 7420 6578 706c 616e 6174 696f 6e2a  ult explanation*
+00001480: 2a2e 2057 6865 6e20 736f 6d65 2074 6573  *. When some tes
+00001490: 7420 6661 696c 732c 2079 6f75 2063 616e  t fails, you can
+000014a0: 2067 6574 2074 6865 202a 2a65 7870 6c61   get the **expla
+000014b0: 6e61 7469 6f6e 2a2a 206f 6620 7468 6520  nation** of the 
+000014c0: 6361 6c63 756c 6174 696f 6e20 7072 6f63  calculation proc
+000014d0: 6573 7320 7374 6570 2062 7920 7374 6570  ess step by step
+000014e0: 2e20 4974 2068 656c 7073 2074 6f20 6964  . It helps to id
+000014f0: 656e 7469 6679 2074 6865 2063 6175 7365  entify the cause
+00001500: 206f 6620 7468 6520 6661 696c 7572 652e   of the failure.
+00001510: 0a2a 202a 2a4f 524d 2061 6363 6573 732a  .* **ORM access*
+00001520: 2a20 696e 7369 6465 2074 6865 2074 6573  * inside the tes
+00001530: 742e 2059 6f75 2068 6176 6520 6675 6c6c  t. You have full
+00001540: 2061 6363 6573 7320 746f 2074 6865 202a   access to the *
+00001550: 2a64 6576 6963 652a 2a20 7072 6f70 6572  *device** proper
+00001560: 7469 6573 2e20 466f 7220 696e 7374 616e  ties. For instan
+00001570: 6365 2c20 796f 7520 6d61 7920 6c65 7665  ce, you may leve
+00001580: 7261 6765 205b 436f 6e66 6967 7572 6174  rage [Configurat
+00001590: 696f 6e20 436f 6e74 6578 7473 5d28 6874  ion Contexts](ht
+000015a0: 7470 733a 2f2f 646f 6373 2e6e 6574 626f  tps://docs.netbo
+000015b0: 782e 6465 762f 656e 2f73 7461 626c 652f  x.dev/en/stable/
+000015c0: 6665 6174 7572 6573 2f63 6f6e 7465 7874  features/context
+000015d0: 2d64 6174 612f 2920 4e65 7442 6f78 2066  -data/) NetBox f
+000015e0: 6561 7475 7265 2074 6f20 7374 6f72 6520  eature to store 
+000015f0: 796f 7572 2064 6573 6972 6564 2063 6f6e  your desired con
+00001600: 6669 6775 7261 7469 6f6e 2061 6e64 2063  figuration and c
+00001610: 6f6d 7061 7265 2069 7420 7769 7468 2074  ompare it with t
+00001620: 6865 2063 6f6e 6669 6720 636f 6c6c 6563  he config collec
+00001630: 7465 6420 6672 6f6d 2074 6865 2064 6576  ted from the dev
+00001640: 6963 652e 0a2a 202a 2a52 6570 6f72 7473  ice..* **Reports
+00001650: 2061 6e64 2077 6562 686f 6f6b 732a 2a2e   and webhooks**.
+00001660: 2041 6674 6572 2065 7865 6375 7469 6f6e   After execution
+00001670: 206f 6620 736f 6d65 2062 756e 6368 206f   of some bunch o
+00001680: 6620 7465 7374 7320 796f 7520 6361 6e20  f tests you can 
+00001690: 6765 7420 7468 6520 7265 706f 7274 2077  get the report w
+000016a0: 6974 6820 7061 7373 6564 2f66 6169 6c65  ith passed/faile
+000016b0: 6420 7374 6174 6973 7469 6373 2067 726f  d statistics gro
+000016c0: 7570 6564 2062 7920 736f 6d65 204c 6f63  uped by some Loc
+000016d0: 6174 696f 6e2f 5369 7465 2f4d 616e 7566  ation/Site/Manuf
+000016e0: 6163 7475 7265 722f 6574 632e 204d 6f72  acturer/etc. Mor
+000016f0: 656f 7665 722c 2079 6f75 2063 616e 2070  eover, you can p
+00001700: 726f 7669 7369 6f6e 2074 6865 2077 6562  rovision the web
+00001710: 686f 6f6b 2074 6f20 6e6f 7469 6679 2061  hook to notify a
+00001720: 6e20 6578 7465 726e 616c 2073 7973 7465  n external syste
+00001730: 6d20 7768 656e 2063 6f6d 706c 6961 6e63  m when complianc
+00001740: 6520 7265 706f 7274 2069 7320 6765 6e65  e report is gene
+00001750: 7261 7465 642e 0a2a 202a 2a54 6573 7420  rated..* **Test 
+00001760: 6578 7465 6e73 6962 696c 6974 792a 2a2e  extensibility**.
+00001770: 2059 6f75 2063 616e 2064 6566 696e 6520   You can define 
+00001780: 796f 7572 206f 776e 2070 7974 686f 6e20  your own python 
+00001790: 6675 6e63 7469 6f6e 7320 6f72 2063 6c61  functions or cla
+000017a0: 7373 6573 2074 6f20 7265 7573 6520 7468  sses to reuse th
+000017b0: 6520 636f 6465 2062 6574 7765 656e 206d  e code between m
+000017c0: 756c 7469 706c 6520 636f 6d70 6c69 616e  ultiple complian
+000017d0: 6365 2074 6573 7473 2e0a 2a20 506f 7373  ce tests..* Poss
+000017e0: 6962 696c 6974 7920 746f 2073 746f 7265  ibility to store
+000017f0: 2061 6c6c 2068 6561 7679 2074 6578 742d   all heavy text-
+00001800: 6261 7365 6420 656e 7469 7469 6573 2028  based entities (
+00001810: 6c69 6b65 2063 6f6d 706c 6961 6e63 6520  like compliance 
+00001820: 7465 7374 7320 6f72 2054 5450 2054 656d  tests or TTP Tem
+00001830: 706c 6174 6573 2920 696e 2061 202a 2a47  plates) in a **G
+00001840: 6974 2072 6570 6f73 6974 6f72 792a 2a0a  it repository**.
+00001850: 0a23 2320 446f 776e 6c6f 6164 2061 6e64  .## Download and
+00001860: 2049 6e73 7461 6c6c 0a0a 596f 7520 6361   Install..You ca
+00001870: 6e20 646f 776e 6c6f 6164 2056 616c 6964  n download Valid
+00001880: 6974 7920 7669 6120 2a2a 7069 702a 2a0a  ity via **pip**.
+00001890: 6060 600a 7069 7020 696e 7374 616c 6c20  ```.pip install 
+000018a0: 6e65 7462 6f78 2d76 616c 6964 6974 790a  netbox-validity.
+000018b0: 6060 600a 4166 7465 7220 7468 6174 2066  ```.After that f
+000018c0: 6f6c 6c6f 7720 7468 6520 5b69 6e73 7461  ollow the [insta
+000018d0: 6c6c 6174 696f 6e20 6775 6964 655d 2868  llation guide](h
+000018e0: 7474 7073 3a2f 2f76 616c 6964 6974 792e  ttps://validity.
+000018f0: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
+00001900: 6e2f 6c61 7465 7374 2f69 6e73 7461 6c6c  n/latest/install
+00001910: 6174 696f 6e2f 2920 746f 2063 6f72 7265  ation/) to corre
+00001920: 6374 6c79 2061 6464 2056 616c 6964 6974  ctly add Validit
+00001930: 7920 746f 2079 6f75 7220 4e65 7442 6f78  y to your NetBox
+00001940: 2e0a 3c21 2d2d 6d6b 646f 6373 2d65 6e64  ..<!--mkdocs-end
+00001950: 2d2d 3e0a 0a23 2320 446f 6375 6d65 6e74  -->..## Document
+00001960: 6174 696f 6e0a 5265 6164 2074 6865 2066  ation.Read the f
+00001970: 756c 6c20 646f 6375 6d65 6e74 6174 696f  ull documentatio
+00001980: 6e20 6f6e 205b 7661 6c69 6469 7479 2e72  n on [validity.r
+00001990: 6561 6474 6865 646f 6373 2e69 6f5d 2868  eadthedocs.io](h
+000019a0: 7474 7073 3a2f 2f76 616c 6964 6974 792e  ttps://validity.
+000019b0: 7265 6164 7468 6564 6f63 732e 696f 290a  readthedocs.io).
+000019c0: 0a0a 2323 2051 7569 636b 2053 7461 7274  ..## Quick Start
+000019d0: 0a0a 5468 6520 7368 6f72 7420 7669 6465  ..The short vide
+000019e0: 6f20 6162 6f75 7420 6669 7273 7420 7374  o about first st
+000019f0: 6570 7320 7769 7468 2056 616c 6964 6974  eps with Validit
+00001a00: 793a 0a0a 5b21 5b57 6174 6368 2074 6865  y:..[![Watch the
+00001a10: 2076 6964 656f 5d28 6874 7470 733a 2f2f   video](https://
+00001a20: 696d 672e 796f 7574 7562 652e 636f 6d2f  img.youtube.com/
+00001a30: 7669 2f48 7332 4955 4536 724b 4334 2f30  vi/Hs2IUE6rKC4/0
+00001a40: 2e6a 7067 295d 2868 7474 7073 3a2f 2f79  .jpg)](https://y
+00001a50: 6f75 7475 2e62 652f 4873 3249 5545 3672  outu.be/Hs2IUE6r
+00001a60: 4b43 3429 0a0a 2323 2043 6f6e 7472 6962  KC4)..## Contrib
+00001a70: 7574 696e 670a 0a46 6565 6c20 6672 6565  uting..Feel free
+00001a80: 2074 6f20 6173 6b20 6120 5b51 7565 7374   to ask a [Quest
+00001a90: 696f 6e5d 2868 7474 7073 3a2f 2f67 6974  ion](https://git
+00001aa0: 6875 622e 636f 6d2f 616d 7961 736e 696b  hub.com/amyasnik
+00001ab0: 6f76 2f76 616c 6964 6974 792f 6469 7363  ov/validity/disc
+00001ac0: 7573 7369 6f6e 7329 2c20 7265 706f 7274  ussions), report
+00001ad0: 2061 6e20 5b49 7373 7565 5d28 6874 7470   an [Issue](http
+00001ae0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f61  s://github.com/a
+00001af0: 6d79 6173 6e69 6b6f 762f 7661 6c69 6469  myasnikov/validi
+00001b00: 7479 2f69 7373 7565 7329 206f 7220 6576  ty/issues) or ev
+00001b10: 656e 206d 616b 6520 6120 5b50 525d 2843  en make a [PR](C
+00001b20: 4f4e 5452 4942 5554 494e 472e 6d64 292e  ONTRIBUTING.md).
+00001b30: 2052 6561 6420 6d6f 7265 2061 626f 7574   Read more about
+00001b40: 2063 6f6e 7472 6962 7574 696f 6e20 696e   contribution in
+00001b50: 2074 6865 205b 434f 4e54 5249 4255 5449   the [CONTRIBUTI
+00001b60: 4e47 5d28 434f 4e54 5249 4255 5449 4e47  NG](CONTRIBUTING
+00001b70: 2e6d 6429 2067 7569 6465 2e0a            .md) guide..
```

### Comparing `netbox-validity-1.2.0/netbox_validity.egg-info/SOURCES.txt` & `netbox-validity-1.2.1/netbox_validity.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -41,28 +41,31 @@
 validity/forms/helpers.py
 validity/management/__init__.py
 validity/management/commands/__init__.py
 validity/management/commands/linkscripts.py
 validity/migrations/0001_initial.py
 validity/migrations/0002_custom_fields.py
 validity/migrations/0003_complianceselector_dp_tag_prefix.py
+validity/migrations/0004_netbox35_scripts.py
 validity/migrations/__init__.py
 validity/models/__init__.py
 validity/models/base.py
 validity/models/device.py
 validity/models/nameset.py
 validity/models/repo.py
 validity/models/report.py
 validity/models/selector.py
 validity/models/serializer.py
 validity/models/test.py
 validity/models/test_result.py
 validity/scripts/__init__.py
 validity/scripts/git.py
 validity/scripts/run_tests.py
+validity/scripts/validity_git.py
+validity/scripts/validity_run_tests.py
 validity/templates/validity/compliance_results.html
 validity/templates/validity/compliancereport.html
 validity/templates/validity/complianceselector.html
 validity/templates/validity/compliancetest.html
 validity/templates/validity/compliancetestresult.html
 validity/templates/validity/configserializer.html
 validity/templates/validity/device_config.html
```

### Comparing `netbox-validity-1.2.0/pyproject.toml` & `netbox-validity-1.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "netbox-validity"
-version = "1.2.0"
+version = "1.2.1"
 description = "NetBox plugin for vendor-agnostic configuration compliance"
 authors = [
     {name = "Anton Miasnikov", email = "anton2008m@gmail.com"},
 ]
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `netbox-validity-1.2.0/validity/__init__.py` & `netbox-validity-1.2.1/validity/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 import logging
 import os
 from pathlib import Path
 
 from django.conf import settings as django_settings
 from extras.plugins import PluginConfig
+from netbox.settings import VERSION
 from pydantic import BaseModel, DirectoryPath, Field
 
+from validity.utils.misc import NetboxVersion
+
 
 logger = logging.getLogger(__name__)
 
 
 class NetBoxValidityConfig(PluginConfig):
     name = "validity"
     verbose_name = "Validity: Configuration Compliance"
     description = "Vendor-agnostic framework to build your own configuration compliance rule set"
     author = "Anton Miasnikov"
     author_email = "anton2008m@gmail.com"
-    version = "1.2.0"
+    version = "1.2.1"
     base_url = "validity"
     django_apps = ["bootstrap5"]
     min_version = "3.4.0"
 
+    # custom field
+    netbox_version = NetboxVersion(VERSION)
+
     def ready(self):
         try:
             os.makedirs(settings.git_folder, exist_ok=True)
         except OSError as e:
             if not settings.git_folder.is_dir():
                 logger.error("Cannot create git_folder (%s), %s: %s", settings.git_folder, type(e).__name__, e)
         return super().ready()
```

### Comparing `netbox-validity-1.2.0/validity/api/helpers.py` & `netbox-validity-1.2.1/validity/api/helpers.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/api/serializers.py` & `netbox-validity-1.2.1/validity/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/api/urls.py` & `netbox-validity-1.2.1/validity/api/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/api/views.py` & `netbox-validity-1.2.1/validity/api/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from http import HTTPStatus
 
 from netbox.api.viewsets import NetBoxModelViewSet
-from netbox.settings import VERSION
 from rest_framework.exceptions import NotFound
 from rest_framework.response import Response
 from rest_framework.views import APIView
 
-from validity import filtersets, models
+from validity import config, filtersets, models
 from validity.config_compliance.device_config import DeviceConfig
 from ..config_compliance.exceptions import DeviceConfigError
 from . import serializers
 
 
-if VERSION.split(".") < ["3", "5"]:
+if config.netbox_version < "3.5.0":
     from drf_yasg.utils import swagger_auto_schema as extend_schema
 else:
     from drf_spectacular.utils import extend_schema
 
 
 class ReadOnlyNetboxViewSet(NetBoxModelViewSet):
     http_method_names = ["get", "head", "options", "trace"]
```

### Comparing `netbox-validity-1.2.0/validity/choices.py` & `netbox-validity-1.2.1/validity/choices.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/config_compliance/device_config/base.py` & `netbox-validity-1.2.1/validity/config_compliance/device_config/base.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/config_compliance/device_config/routeros.py` & `netbox-validity-1.2.1/validity/config_compliance/device_config/routeros.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/config_compliance/device_config/ttp.py` & `netbox-validity-1.2.1/validity/config_compliance/device_config/ttp.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/config_compliance/device_config/yaml.py` & `netbox-validity-1.2.1/validity/config_compliance/device_config/yaml.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/config_compliance/dynamic_pairs.py` & `netbox-validity-1.2.1/validity/config_compliance/dynamic_pairs.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/config_compliance/eval/default_nameset.py` & `netbox-validity-1.2.1/validity/config_compliance/eval/default_nameset.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/config_compliance/eval/eval.py` & `netbox-validity-1.2.1/validity/config_compliance/eval/eval.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/config_compliance/eval/eval_defaults.py` & `netbox-validity-1.2.1/validity/config_compliance/eval/eval_defaults.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/filtersets.py` & `netbox-validity-1.2.1/validity/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/forms/filterset.py` & `netbox-validity-1.2.1/validity/forms/filterset.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/forms/general.py` & `netbox-validity-1.2.1/validity/forms/general.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/forms/helpers.py` & `netbox-validity-1.2.1/validity/forms/helpers.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/graphql.py` & `netbox-validity-1.2.1/validity/graphql.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/management/commands/linkscripts.py` & `netbox-validity-1.2.1/validity/management/commands/linkscripts.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 class Command(BaseCommand):
     help = "Makes symlinks inside $SCRIPTS_ROOT dir for Validity scripts"
 
     plugin_scripts_dir = "scripts"
     script_prefix = "validity_"
 
     def handle(self, *args, **options):
+        if (ver := validity.config.netbox_version) >= 3.5:
+            self.stdout.write(f"You do not need this command for NetBox {ver}, ignoring")
+            return
         validity_scripts = Path(validity.__file__).parent.absolute() / self.plugin_scripts_dir
         self.symlink_scripts(Path(validity_scripts), Path(settings.SCRIPTS_ROOT))
 
     def symlink_scripts(self, src_dir: Path, dst_dir: Path) -> None:
         symlinks_created = 0
         for script_file in Path(src_dir).iterdir():
             if not script_file.is_file() or not script_file.name.endswith(".py") or script_file.name == "__init__.py":
```

### Comparing `netbox-validity-1.2.0/validity/managers.py` & `netbox-validity-1.2.1/validity/managers.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/migrations/0001_initial.py` & `netbox-validity-1.2.1/validity/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/migrations/0002_custom_fields.py` & `netbox-validity-1.2.1/validity/migrations/0002_custom_fields.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/models/base.py` & `netbox-validity-1.2.1/validity/models/base.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/models/device.py` & `netbox-validity-1.2.1/validity/models/device.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/models/nameset.py` & `netbox-validity-1.2.1/validity/models/nameset.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/models/repo.py` & `netbox-validity-1.2.1/validity/models/repo.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/models/selector.py` & `netbox-validity-1.2.1/validity/models/selector.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/models/serializer.py` & `netbox-validity-1.2.1/validity/models/serializer.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/models/test.py` & `netbox-validity-1.2.1/validity/models/test.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/models/test_result.py` & `netbox-validity-1.2.1/validity/models/test_result.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/navigation.py` & `netbox-validity-1.2.1/validity/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/scripts/git.py` & `netbox-validity-1.2.1/validity/scripts/git.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/scripts/run_tests.py` & `netbox-validity-1.2.1/validity/scripts/run_tests.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/search.py` & `netbox-validity-1.2.1/validity/search.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/tables.py` & `netbox-validity-1.2.1/validity/tables.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/templates/validity/compliance_results.html` & `netbox-validity-1.2.1/validity/templates/validity/compliance_results.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/templates/validity/compliancereport.html` & `netbox-validity-1.2.1/validity/templates/validity/compliancereport.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/templates/validity/complianceselector.html` & `netbox-validity-1.2.1/validity/templates/validity/complianceselector.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/templates/validity/compliancetest.html` & `netbox-validity-1.2.1/validity/templates/validity/compliancetest.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/templates/validity/compliancetestresult.html` & `netbox-validity-1.2.1/validity/templates/validity/compliancetestresult.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/templates/validity/configserializer.html` & `netbox-validity-1.2.1/validity/templates/validity/configserializer.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/templates/validity/device_config.html` & `netbox-validity-1.2.1/validity/templates/validity/device_config.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/templates/validity/gitrepo.html` & `netbox-validity-1.2.1/validity/templates/validity/gitrepo.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/templates/validity/nameset.html` & `netbox-validity-1.2.1/validity/templates/validity/nameset.html`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/templatetags/validity.py` & `netbox-validity-1.2.1/validity/templatetags/validity.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/tests/base.py` & `netbox-validity-1.2.1/validity/tests/base.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/tests/conftest.py` & `netbox-validity-1.2.1/validity/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/tests/factories.py` & `netbox-validity-1.2.1/validity/tests/factories.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/tests/test_api.py` & `netbox-validity-1.2.1/validity/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/tests/test_config_compliance/test_device_config.py` & `netbox-validity-1.2.1/validity/tests/test_config_compliance/test_device_config.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/tests/test_config_compliance/test_dynamic_pairs.py` & `netbox-validity-1.2.1/validity/tests/test_config_compliance/test_dynamic_pairs.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/tests/test_config_compliance/test_eval.py` & `netbox-validity-1.2.1/validity/tests/test_config_compliance/test_eval.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/tests/test_graphql.py` & `netbox-validity-1.2.1/validity/tests/test_graphql.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/tests/test_models/test_clean.py` & `netbox-validity-1.2.1/validity/tests/test_models/test_clean.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/tests/test_models/test_git_link.py` & `netbox-validity-1.2.1/validity/tests/test_models/test_git_link.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/tests/test_models/test_git_repo.py` & `netbox-validity-1.2.1/validity/tests/test_models/test_git_repo.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/tests/test_models/test_selector.py` & `netbox-validity-1.2.1/validity/tests/test_models/test_selector.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/tests/test_models/test_vdevice.py` & `netbox-validity-1.2.1/validity/tests/test_models/test_vdevice.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/tests/test_scripts/test_run_tests.py` & `netbox-validity-1.2.1/validity/tests/test_scripts/test_run_tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import pytest
 from factories import CompTestDBFactory, DeviceFactory, NameSetDBFactory, ReportFactory, SelectorFactory
 from simpleeval import InvalidExpression
 
 from validity.config_compliance.exceptions import EvalError
 from validity.models import ComplianceReport, ComplianceTestResult, VDevice
-from validity.scripts import run_tests
-from validity.scripts.run_tests import RunTestsScript
+from validity.scripts import validity_run_tests
+from validity.scripts.validity_run_tests import RunTestsScript
 from validity.utils.misc import null_request
 
 
 NS_1 = """
 __all__ = ["func1", "var", "func2"]
 
 def func1(var): pass
@@ -80,15 +80,15 @@
 
 
 def test_run_test(monkeypatch):
     script = RunTestsScript()
     nm_functions = Mock()
     evaluator_cls = Mock(return_value=Mock(explanation=[("var1", "val1")]))
     monkeypatch.setattr(script, "nameset_functions", nm_functions)
-    monkeypatch.setattr(run_tests, "ExplanationalEval", evaluator_cls)
+    monkeypatch.setattr(validity_run_tests, "ExplanationalEval", evaluator_cls)
     device = Mock()
     test = Mock()
     passed, explanation = script.run_test(device, test)
     assert passed  # bool(Mock()) is True
     assert explanation
     nm_functions.assert_called_once_with(test.namesets.all())
     evaluator_cls.assert_called_once_with(
@@ -104,15 +104,15 @@
         Mock(return_value=(False, [("1", "2"), ("3", "4")])),
         Mock(side_effect=InvalidExpression()),
         Mock(side_effect=EvalError(InvalidExpression())),
     ],
 )
 def test_run_tests_for_device(mock_script_logging, run_test_mock, monkeypatch):
     result_cls = namedtuple("MockResult", "passed explanation device test report dynamic_pair")
-    monkeypatch.setattr(run_tests, "ComplianceTestResult", result_cls)
+    monkeypatch.setattr(validity_run_tests, "ComplianceTestResult", result_cls)
     script = RunTestsScript()
     script._sleep_between_tests = 0
     monkeypatch.setattr(script, "run_test", run_test_mock)
     tests = ["test1", "test2", "test3"]
     device = Mock()
     report = Mock()
     results = list(script.run_tests_for_device(tests, device, report))
@@ -148,24 +148,24 @@
     script.run_tests_for_device.assert_any_call(selector.tests.all(), devices[0], report)
     script.run_tests_for_device.assert_any_call(selector.tests.all(), devices[1], report)
 
 
 @pytest.mark.django_db
 def test_webhook_without_ctx_is_not_fired(monkeypatch):
     enq_obj = Mock()
-    monkeypatch.setattr(run_tests, "enqueue_object", enq_obj)
+    monkeypatch.setattr(validity_run_tests, "enqueue_object", enq_obj)
     with null_request():
         ComplianceReport.objects.create()
     enq_obj.assert_not_called()
 
 
 @pytest.mark.django_db
 def test_fire_report_webhook(monkeypatch):
     enq_obj = Mock()
-    monkeypatch.setattr(run_tests, "enqueue_object", enq_obj)
+    monkeypatch.setattr(validity_run_tests, "enqueue_object", enq_obj)
     script = RunTestsScript()
     script.request = Mock(id=uuid4(), user=Mock(username="admin"))
     report = ReportFactory()
     script.fire_report_webhook(report.pk)
     enq_obj.assert_called_once()
```

### Comparing `netbox-validity-1.2.0/validity/tests/test_utils/test_git.py` & `netbox-validity-1.2.1/validity/tests/test_utils/test_git.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/tests/test_views.py` & `netbox-validity-1.2.1/validity/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/urls.py` & `netbox-validity-1.2.1/validity/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/utils/git.py` & `netbox-validity-1.2.1/validity/utils/git.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/utils/password.py` & `netbox-validity-1.2.1/validity/utils/password.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/views/__init__.py` & `netbox-validity-1.2.1/validity/views/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/views/base.py` & `netbox-validity-1.2.1/validity/views/base.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/views/device.py` & `netbox-validity-1.2.1/validity/views/device.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/views/git_repo.py` & `netbox-validity-1.2.1/validity/views/git_repo.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/views/nameset.py` & `netbox-validity-1.2.1/validity/views/nameset.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/views/report.py` & `netbox-validity-1.2.1/validity/views/report.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/views/selector.py` & `netbox-validity-1.2.1/validity/views/selector.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/views/serializer.py` & `netbox-validity-1.2.1/validity/views/serializer.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/views/test.py` & `netbox-validity-1.2.1/validity/views/test.py`

 * *Files identical despite different names*

### Comparing `netbox-validity-1.2.0/validity/views/test_result.py` & `netbox-validity-1.2.1/validity/views/test_result.py`

 * *Files identical despite different names*

