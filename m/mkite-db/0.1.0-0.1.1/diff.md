# Comparing `tmp/mkite_db-0.1.0.tar.gz` & `tmp/mkite_db-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkite_db-0.1.0.tar", last modified: Fri Apr 28 17:13:49 2023, max compression
+gzip compressed data, was "mkite_db-0.1.1.tar", last modified: Thu May 25 14:36:59 2023, max compression
```

## Comparing `mkite_db-0.1.0.tar` & `mkite_db-0.1.1.tar`

### file list

```diff
@@ -1,159 +1,159 @@
-drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-04-28 17:13:49.447149 mkite_db-0.1.0/
--rw-r--r--   0 schwalbekoda1 (61642)    61642     1374 2023-04-28 04:43:28.000000 mkite_db-0.1.0/.gitignore
--rw-r--r--   0 schwalbekoda1 (61642)    61642     3266 2023-04-28 04:43:28.000000 mkite_db-0.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 schwalbekoda1 (61642)    61642    12276 2023-04-28 04:43:28.000000 mkite_db-0.1.0/LICENSE
--rw-r--r--   0 schwalbekoda1 (61642)    61642     1167 2023-04-28 04:43:28.000000 mkite_db-0.1.0/NOTICE
--rw-r--r--   0 schwalbekoda1 (61642)    61642     3172 2023-04-28 17:13:49.446964 mkite_db-0.1.0/PKG-INFO
--rw-r--r--   0 schwalbekoda1 (61642)    61642     2834 2023-04-28 17:12:53.000000 mkite_db-0.1.0/README.md
-drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-04-28 17:13:49.421964 mkite_db-0.1.0/docs/
-drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-04-28 17:13:49.426713 mkite_db-0.1.0/docs/_static/
--rwx------   0 schwalbekoda1 (61642)    61642     3039 2023-04-28 04:43:28.000000 mkite_db-0.1.0/docs/_static/mkite-logo.svg
--rw-r--r--   0 schwalbekoda1 (61642)    61642    42781 2023-04-28 04:43:28.000000 mkite_db-0.1.0/docs/_static/mkite.png
-drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-04-28 17:13:49.426902 mkite_db-0.1.0/mkite_db/
-drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-04-28 17:13:49.428520 mkite_db-0.1.0/mkite_db/cfg/
--rw-r--r--   0 schwalbekoda1 (61642)    61642        0 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/cfg/__init__.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642      397 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/cfg/asgi.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642     3021 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/cfg/settings.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642      741 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/cfg/urls.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642      397 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/cfg/wsgi.py
-drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-04-28 17:13:49.428676 mkite_db-0.1.0/mkite_db/cli/
--rw-r--r--   0 schwalbekoda1 (61642)    61642      430 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/cli/run_manage.py
-drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-04-28 17:13:49.429482 mkite_db-0.1.0/mkite_db/dbimport/
--rw-r--r--   0 schwalbekoda1 (61642)    61642      184 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/dbimport/__init__.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642     1663 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/dbimport/ase.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642     2492 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/dbimport/base.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642     1617 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/dbimport/molfile.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642     2872 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/dbimport/mp.py
-drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-04-28 17:13:49.430144 mkite_db-0.1.0/mkite_db/dbimport/tests/
--rw-r--r--   0 schwalbekoda1 (61642)    61642        0 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/dbimport/tests/__init__.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642     2149 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/dbimport/tests/test_ase.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642     1578 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/dbimport/tests/test_molfile.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642     3458 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/dbimport/tests/test_mp.py
--rwxr-xr-x   0 schwalbekoda1 (61642)    61642      783 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/manage.py
-drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-04-28 17:13:49.431419 mkite_db-0.1.0/mkite_db/orm/
--rw-r--r--   0 schwalbekoda1 (61642)    61642       14 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/orm/.gitignore
--rw-r--r--   0 schwalbekoda1 (61642)    61642        0 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/orm/__init__.py
-drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-04-28 17:13:49.432143 mkite_db-0.1.0/mkite_db/orm/base/
--rw-r--r--   0 schwalbekoda1 (61642)    61642        0 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/orm/base/__init__.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642      150 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/orm/base/apps.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642     5444 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/orm/base/models.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642      958 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/orm/base/serializers.py
-drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-04-28 17:13:49.432713 mkite_db-0.1.0/mkite_db/orm/base/tests/
--rw-r--r--   0 schwalbekoda1 (61642)    61642        0 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/orm/base/tests/__init__.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642      672 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/orm/base/tests/test_models.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642     3073 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/orm/base/tests/test_serializers.py
-drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-04-28 17:13:49.433457 mkite_db-0.1.0/mkite_db/orm/calcs/
--rw-r--r--   0 schwalbekoda1 (61642)    61642        0 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/orm/calcs/__init__.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642      152 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/orm/calcs/apps.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642      348 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/orm/calcs/models.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642      656 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/orm/calcs/serializers.py
-drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-04-28 17:13:49.433818 mkite_db-0.1.0/mkite_db/orm/calcs/tests/
--rw-r--r--   0 schwalbekoda1 (61642)    61642        0 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/orm/calcs/tests/__init__.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642     2812 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/orm/calcs/tests/test_serializers.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642     2792 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/orm/deserializers.py
-drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-04-28 17:13:49.434860 mkite_db-0.1.0/mkite_db/orm/jobs/
--rw-r--r--   0 schwalbekoda1 (61642)    61642        0 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/orm/jobs/__init__.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642      150 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/orm/jobs/apps.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642      447 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/orm/jobs/deleter.py
-drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-04-28 17:13:49.423418 mkite_db-0.1.0/mkite_db/orm/jobs/management/
-drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-04-28 17:13:49.435565 mkite_db-0.1.0/mkite_db/orm/jobs/management/commands/
--rw-r--r--   0 schwalbekoda1 (61642)    61642        0 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/orm/jobs/management/commands/__init__.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642     1672 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/orm/jobs/management/commands/create_experiment.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642     1309 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/orm/jobs/management/commands/create_project.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642     2216 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/orm/jobs/management/commands/scanrecipes.py
-drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-04-28 17:13:49.435897 mkite_db-0.1.0/mkite_db/orm/jobs/management/commands/tests/
--rw-r--r--   0 schwalbekoda1 (61642)    61642        0 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/orm/jobs/management/commands/tests/__init__.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642      501 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/orm/jobs/management/commands/tests/test_scanrecipes.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642     5297 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/orm/jobs/models.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642     3493 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/orm/jobs/serializers.py
-drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-04-28 17:13:49.436784 mkite_db-0.1.0/mkite_db/orm/jobs/tests/
--rw-r--r--   0 schwalbekoda1 (61642)    61642        0 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/orm/jobs/tests/__init__.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642     1703 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/orm/jobs/tests/test_deleter.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642     4539 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/orm/jobs/tests/test_models.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642     8712 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/orm/jobs/tests/test_serializers.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642      371 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/orm/models.py
-drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-04-28 17:13:49.437629 mkite_db-0.1.0/mkite_db/orm/mols/
--rw-r--r--   0 schwalbekoda1 (61642)    61642        0 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/orm/mols/__init__.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642      150 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/orm/mols/apps.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642     1956 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/orm/mols/models.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642     1369 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/orm/mols/serializers.py
-drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-04-28 17:13:49.438095 mkite_db-0.1.0/mkite_db/orm/mols/tests/
--rw-r--r--   0 schwalbekoda1 (61642)    61642        0 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/orm/mols/tests/__init__.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642     3231 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/orm/mols/tests/test_models.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642     2860 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/orm/mols/tests/test_serializers.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642       86 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/orm/repr.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642     5039 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/orm/serializers.py
-drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-04-28 17:13:49.438749 mkite_db-0.1.0/mkite_db/orm/structs/
--rw-r--r--   0 schwalbekoda1 (61642)    61642        0 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/orm/structs/__init__.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642      156 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/orm/structs/apps.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642     7873 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/orm/structs/models.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642     1244 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/orm/structs/serializers.py
-drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-04-28 17:13:49.439247 mkite_db-0.1.0/mkite_db/orm/structs/tests/
--rw-r--r--   0 schwalbekoda1 (61642)    61642        0 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/orm/structs/tests/__init__.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642     1499 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/orm/structs/tests/test_models.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642     2110 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/orm/structs/tests/test_serializers.py
-drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-04-28 17:13:49.439810 mkite_db-0.1.0/mkite_db/orm/tests/
--rw-r--r--   0 schwalbekoda1 (61642)    61642        0 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/orm/tests/__init__.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642     1051 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/orm/tests/test_deserializers.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642      423 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/orm/tests/test_repr.py
-drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-04-28 17:13:49.439974 mkite_db-0.1.0/mkite_db/tests/
--rw-r--r--   0 schwalbekoda1 (61642)    61642        0 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/tests/__init__.py
-drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-04-28 17:13:49.440396 mkite_db-0.1.0/mkite_db/tests/files/
--rw-r--r--   0 schwalbekoda1 (61642)    61642        0 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/tests/files/__init__.py
-drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-04-28 17:13:49.441516 mkite_db-0.1.0/mkite_db/tests/files/dbimport/
--rw-r--r--   0 schwalbekoda1 (61642)    61642        0 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/tests/files/dbimport/__init__.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642     1378 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/tests/files/dbimport/caffeine.xyz
--rw-r--r--   0 schwalbekoda1 (61642)    61642       94 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/tests/files/dbimport/molfile.yaml
--rw-r--r--   0 schwalbekoda1 (61642)    61642     4170 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/tests/files/dbimport/mp.json
--rw-r--r--   0 schwalbekoda1 (61642)    61642      232 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/tests/files/dbimport/mp_query.json
--rw-r--r--   0 schwalbekoda1 (61642)    61642     5854 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/tests/files/dbimport/silicon.cif
--rw-r--r--   0 schwalbekoda1 (61642)    61642       55 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/tests/files/engine.yaml
-drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-04-28 17:13:49.441914 mkite_db-0.1.0/mkite_db/tests/files/workflow/
--rw-r--r--   0 schwalbekoda1 (61642)    61642        0 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/tests/files/workflow/__init__.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642      695 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/tests/files/workflow/create_rules.yaml
--rw-r--r--   0 schwalbekoda1 (61642)    61642     2322 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/tests/files/workflow/jobresults.json
-drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-04-28 17:13:49.442421 mkite_db-0.1.0/mkite_db/workflow/
--rw-r--r--   0 schwalbekoda1 (61642)    61642        0 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/workflow/__init__.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642      154 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/workflow/apps.py
-drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-04-28 17:13:49.443143 mkite_db-0.1.0/mkite_db/workflow/create/
--rw-r--r--   0 schwalbekoda1 (61642)    61642      202 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/workflow/create/__init__.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642     3894 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/workflow/create/base.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642     1515 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/workflow/create/simple.py
-drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-04-28 17:13:49.443579 mkite_db-0.1.0/mkite_db/workflow/create/tests/
--rw-r--r--   0 schwalbekoda1 (61642)    61642        0 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/workflow/create/tests/__init__.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642     3158 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/workflow/create/tests/test_simple.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642     4557 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/workflow/create/tests/test_tuple.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642     2573 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/workflow/create/tuple.py
-drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-04-28 17:13:49.443791 mkite_db-0.1.0/mkite_db/workflow/management/
--rw-r--r--   0 schwalbekoda1 (61642)    61642        0 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/workflow/management/__init__.py
-drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-04-28 17:13:49.445123 mkite_db-0.1.0/mkite_db/workflow/management/commands/
--rw-r--r--   0 schwalbekoda1 (61642)    61642        0 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/workflow/management/commands/__init__.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642     3267 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/workflow/management/commands/create_from_file.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642     4369 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/workflow/management/commands/create_simple.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642     5048 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/workflow/management/commands/dbimport.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642     3938 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/workflow/management/commands/parse.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642     2922 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/workflow/management/commands/parse_file.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642     4689 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/workflow/management/commands/submit.py
-drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-04-28 17:13:49.446382 mkite_db-0.1.0/mkite_db/workflow/management/commands/tests/
--rw-r--r--   0 schwalbekoda1 (61642)    61642        0 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/workflow/management/commands/tests/__init__.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642     1137 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/workflow/management/commands/tests/test_create_from_file.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642     2202 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/workflow/management/commands/tests/test_create_simple.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642     3632 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/workflow/management/commands/tests/test_dbimport.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642     2310 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/workflow/management/commands/tests/test_parse.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642     2415 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/workflow/management/commands/tests/test_parse_file.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642     3397 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/workflow/management/commands/tests/test_submit.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642     3002 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/workflow/parse.py
-drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-04-28 17:13:49.446708 mkite_db-0.1.0/mkite_db/workflow/tests/
--rw-r--r--   0 schwalbekoda1 (61642)    61642        0 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/workflow/tests/__init__.py
--rw-r--r--   0 schwalbekoda1 (61642)    61642     2076 2023-04-28 04:43:28.000000 mkite_db-0.1.0/mkite_db/workflow/tests/test_parse.py
-drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-04-28 17:13:49.427802 mkite_db-0.1.0/mkite_db.egg-info/
--rw-r--r--   0 schwalbekoda1 (61642)    61642     3172 2023-04-28 17:13:49.000000 mkite_db-0.1.0/mkite_db.egg-info/PKG-INFO
--rw-r--r--   0 schwalbekoda1 (61642)    61642     4354 2023-04-28 17:13:49.000000 mkite_db-0.1.0/mkite_db.egg-info/SOURCES.txt
--rw-r--r--   0 schwalbekoda1 (61642)    61642        1 2023-04-28 17:13:49.000000 mkite_db-0.1.0/mkite_db.egg-info/dependency_links.txt
--rw-r--r--   0 schwalbekoda1 (61642)    61642       53 2023-04-28 17:13:49.000000 mkite_db-0.1.0/mkite_db.egg-info/entry_points.txt
--rw-r--r--   0 schwalbekoda1 (61642)    61642      228 2023-04-28 17:13:49.000000 mkite_db-0.1.0/mkite_db.egg-info/requires.txt
--rw-r--r--   0 schwalbekoda1 (61642)    61642        9 2023-04-28 17:13:49.000000 mkite_db-0.1.0/mkite_db.egg-info/top_level.txt
--rw-r--r--   0 schwalbekoda1 (61642)    61642      880 2023-04-28 17:12:35.000000 mkite_db-0.1.0/pyproject.toml
--rw-r--r--   0 schwalbekoda1 (61642)    61642      253 2023-04-28 17:03:10.000000 mkite_db-0.1.0/requirements.txt
--rw-r--r--   0 schwalbekoda1 (61642)    61642       38 2023-04-28 17:13:49.447197 mkite_db-0.1.0/setup.cfg
--rw-r--r--   0 schwalbekoda1 (61642)    61642       38 2023-04-28 05:37:26.000000 mkite_db-0.1.0/setup.py
+drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-05-25 14:36:59.444629 mkite_db-0.1.1/
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     1374 2023-04-28 04:43:28.000000 mkite_db-0.1.1/.gitignore
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     3266 2023-04-28 04:43:28.000000 mkite_db-0.1.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 schwalbekoda1 (61642)    61642    12276 2023-04-28 04:43:28.000000 mkite_db-0.1.1/LICENSE
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     1167 2023-04-28 04:43:28.000000 mkite_db-0.1.1/NOTICE
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     3172 2023-05-25 14:36:59.444372 mkite_db-0.1.1/PKG-INFO
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     2834 2023-04-28 17:12:53.000000 mkite_db-0.1.1/README.md
+drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-05-25 14:36:59.416522 mkite_db-0.1.1/docs/
+drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-05-25 14:36:59.422157 mkite_db-0.1.1/docs/_static/
+-rwx------   0 schwalbekoda1 (61642)    61642     3039 2023-04-28 04:43:28.000000 mkite_db-0.1.1/docs/_static/mkite-logo.svg
+-rw-r--r--   0 schwalbekoda1 (61642)    61642    42781 2023-04-28 04:43:28.000000 mkite_db-0.1.1/docs/_static/mkite.png
+drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-05-25 14:36:59.422415 mkite_db-0.1.1/mkite_db/
+drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-05-25 14:36:59.424602 mkite_db-0.1.1/mkite_db/cfg/
+-rw-r--r--   0 schwalbekoda1 (61642)    61642        0 2023-04-28 04:43:28.000000 mkite_db-0.1.1/mkite_db/cfg/__init__.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642      397 2023-04-28 04:43:28.000000 mkite_db-0.1.1/mkite_db/cfg/asgi.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     3039 2023-05-25 14:34:35.000000 mkite_db-0.1.1/mkite_db/cfg/settings.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642      741 2023-04-28 04:43:28.000000 mkite_db-0.1.1/mkite_db/cfg/urls.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642      397 2023-04-28 04:43:28.000000 mkite_db-0.1.1/mkite_db/cfg/wsgi.py
+drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-05-25 14:36:59.424783 mkite_db-0.1.1/mkite_db/cli/
+-rw-r--r--   0 schwalbekoda1 (61642)    61642      430 2023-04-28 04:43:28.000000 mkite_db-0.1.1/mkite_db/cli/run_manage.py
+drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-05-25 14:36:59.425950 mkite_db-0.1.1/mkite_db/dbimport/
+-rw-r--r--   0 schwalbekoda1 (61642)    61642      184 2023-04-28 04:43:28.000000 mkite_db-0.1.1/mkite_db/dbimport/__init__.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     1661 2023-05-25 14:34:35.000000 mkite_db-0.1.1/mkite_db/dbimport/ase.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     2492 2023-04-28 04:43:28.000000 mkite_db-0.1.1/mkite_db/dbimport/base.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     1620 2023-05-25 14:30:31.000000 mkite_db-0.1.1/mkite_db/dbimport/molfile.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     2872 2023-04-28 04:43:28.000000 mkite_db-0.1.1/mkite_db/dbimport/mp.py
+drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-05-25 14:36:59.426854 mkite_db-0.1.1/mkite_db/dbimport/tests/
+-rw-r--r--   0 schwalbekoda1 (61642)    61642        0 2023-04-28 04:43:28.000000 mkite_db-0.1.1/mkite_db/dbimport/tests/__init__.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     2158 2023-05-25 14:30:31.000000 mkite_db-0.1.1/mkite_db/dbimport/tests/test_ase.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     1584 2023-05-25 14:30:31.000000 mkite_db-0.1.1/mkite_db/dbimport/tests/test_molfile.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     3465 2023-05-25 14:34:35.000000 mkite_db-0.1.1/mkite_db/dbimport/tests/test_mp.py
+-rwxr-xr-x   0 schwalbekoda1 (61642)    61642      783 2023-04-28 04:43:28.000000 mkite_db-0.1.1/mkite_db/manage.py
+drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-05-25 14:36:59.428038 mkite_db-0.1.1/mkite_db/orm/
+-rw-r--r--   0 schwalbekoda1 (61642)    61642       14 2023-04-28 04:43:28.000000 mkite_db-0.1.1/mkite_db/orm/.gitignore
+-rw-r--r--   0 schwalbekoda1 (61642)    61642        0 2023-04-28 04:43:28.000000 mkite_db-0.1.1/mkite_db/orm/__init__.py
+drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-05-25 14:36:59.429224 mkite_db-0.1.1/mkite_db/orm/base/
+-rw-r--r--   0 schwalbekoda1 (61642)    61642        0 2023-04-28 04:43:28.000000 mkite_db-0.1.1/mkite_db/orm/base/__init__.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642      153 2023-05-25 14:30:31.000000 mkite_db-0.1.1/mkite_db/orm/base/apps.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     5444 2023-04-28 04:43:28.000000 mkite_db-0.1.1/mkite_db/orm/base/models.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642      964 2023-05-25 14:30:31.000000 mkite_db-0.1.1/mkite_db/orm/base/serializers.py
+drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-05-25 14:36:59.429750 mkite_db-0.1.1/mkite_db/orm/base/tests/
+-rw-r--r--   0 schwalbekoda1 (61642)    61642        0 2023-04-28 04:43:28.000000 mkite_db-0.1.1/mkite_db/orm/base/tests/__init__.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642      675 2023-05-25 14:30:31.000000 mkite_db-0.1.1/mkite_db/orm/base/tests/test_models.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     3100 2023-05-25 14:30:31.000000 mkite_db-0.1.1/mkite_db/orm/base/tests/test_serializers.py
+drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-05-25 14:36:59.430488 mkite_db-0.1.1/mkite_db/orm/calcs/
+-rw-r--r--   0 schwalbekoda1 (61642)    61642        0 2023-04-28 04:43:28.000000 mkite_db-0.1.1/mkite_db/orm/calcs/__init__.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642      155 2023-05-25 14:30:31.000000 mkite_db-0.1.1/mkite_db/orm/calcs/apps.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642      351 2023-05-25 14:30:31.000000 mkite_db-0.1.1/mkite_db/orm/calcs/models.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642      659 2023-05-25 14:30:31.000000 mkite_db-0.1.1/mkite_db/orm/calcs/serializers.py
+drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-05-25 14:36:59.430837 mkite_db-0.1.1/mkite_db/orm/calcs/tests/
+-rw-r--r--   0 schwalbekoda1 (61642)    61642        0 2023-04-28 04:43:28.000000 mkite_db-0.1.1/mkite_db/orm/calcs/tests/__init__.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     2842 2023-05-25 14:30:31.000000 mkite_db-0.1.1/mkite_db/orm/calcs/tests/test_serializers.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     2807 2023-05-25 14:30:31.000000 mkite_db-0.1.1/mkite_db/orm/deserializers.py
+drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-05-25 14:36:59.431906 mkite_db-0.1.1/mkite_db/orm/jobs/
+-rw-r--r--   0 schwalbekoda1 (61642)    61642        0 2023-04-28 04:43:28.000000 mkite_db-0.1.1/mkite_db/orm/jobs/__init__.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642      153 2023-05-25 14:30:31.000000 mkite_db-0.1.1/mkite_db/orm/jobs/apps.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642      447 2023-04-28 04:43:28.000000 mkite_db-0.1.1/mkite_db/orm/jobs/deleter.py
+drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-05-25 14:36:59.418070 mkite_db-0.1.1/mkite_db/orm/jobs/management/
+drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-05-25 14:36:59.432676 mkite_db-0.1.1/mkite_db/orm/jobs/management/commands/
+-rw-r--r--   0 schwalbekoda1 (61642)    61642        0 2023-04-28 04:43:28.000000 mkite_db-0.1.1/mkite_db/orm/jobs/management/commands/__init__.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     1675 2023-05-25 14:30:31.000000 mkite_db-0.1.1/mkite_db/orm/jobs/management/commands/create_experiment.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     1312 2023-05-25 14:30:31.000000 mkite_db-0.1.1/mkite_db/orm/jobs/management/commands/create_project.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     2225 2023-05-25 14:30:31.000000 mkite_db-0.1.1/mkite_db/orm/jobs/management/commands/scanrecipes.py
+drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-05-25 14:36:59.432993 mkite_db-0.1.1/mkite_db/orm/jobs/management/commands/tests/
+-rw-r--r--   0 schwalbekoda1 (61642)    61642        0 2023-04-28 04:43:28.000000 mkite_db-0.1.1/mkite_db/orm/jobs/management/commands/tests/__init__.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642      504 2023-05-25 14:30:31.000000 mkite_db-0.1.1/mkite_db/orm/jobs/management/commands/tests/test_scanrecipes.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     5303 2023-05-25 14:30:31.000000 mkite_db-0.1.1/mkite_db/orm/jobs/models.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     3496 2023-05-25 14:30:31.000000 mkite_db-0.1.1/mkite_db/orm/jobs/serializers.py
+drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-05-25 14:36:59.433757 mkite_db-0.1.1/mkite_db/orm/jobs/tests/
+-rw-r--r--   0 schwalbekoda1 (61642)    61642        0 2023-04-28 04:43:28.000000 mkite_db-0.1.1/mkite_db/orm/jobs/tests/__init__.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     1709 2023-05-25 14:30:31.000000 mkite_db-0.1.1/mkite_db/orm/jobs/tests/test_deleter.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     4542 2023-05-25 14:30:31.000000 mkite_db-0.1.1/mkite_db/orm/jobs/tests/test_models.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     8718 2023-05-25 14:30:31.000000 mkite_db-0.1.1/mkite_db/orm/jobs/tests/test_serializers.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642      371 2023-04-28 04:43:28.000000 mkite_db-0.1.1/mkite_db/orm/models.py
+drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-05-25 14:36:59.434468 mkite_db-0.1.1/mkite_db/orm/mols/
+-rw-r--r--   0 schwalbekoda1 (61642)    61642        0 2023-04-28 04:43:28.000000 mkite_db-0.1.1/mkite_db/orm/mols/__init__.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642      153 2023-05-25 14:30:31.000000 mkite_db-0.1.1/mkite_db/orm/mols/apps.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     1962 2023-05-25 14:30:31.000000 mkite_db-0.1.1/mkite_db/orm/mols/models.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     1378 2023-05-25 14:30:31.000000 mkite_db-0.1.1/mkite_db/orm/mols/serializers.py
+drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-05-25 14:36:59.434973 mkite_db-0.1.1/mkite_db/orm/mols/tests/
+-rw-r--r--   0 schwalbekoda1 (61642)    61642        0 2023-04-28 04:43:28.000000 mkite_db-0.1.1/mkite_db/orm/mols/tests/__init__.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     3243 2023-05-25 14:30:31.000000 mkite_db-0.1.1/mkite_db/orm/mols/tests/test_models.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     2872 2023-05-25 14:30:31.000000 mkite_db-0.1.1/mkite_db/orm/mols/tests/test_serializers.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642       86 2023-04-28 04:43:28.000000 mkite_db-0.1.1/mkite_db/orm/repr.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     5042 2023-05-25 14:30:31.000000 mkite_db-0.1.1/mkite_db/orm/serializers.py
+drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-05-25 14:36:59.435592 mkite_db-0.1.1/mkite_db/orm/structs/
+-rw-r--r--   0 schwalbekoda1 (61642)    61642        0 2023-04-28 04:43:28.000000 mkite_db-0.1.1/mkite_db/orm/structs/__init__.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642      159 2023-05-25 14:30:31.000000 mkite_db-0.1.1/mkite_db/orm/structs/apps.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     7879 2023-05-25 14:30:31.000000 mkite_db-0.1.1/mkite_db/orm/structs/models.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     1253 2023-05-25 14:30:31.000000 mkite_db-0.1.1/mkite_db/orm/structs/serializers.py
+drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-05-25 14:36:59.436040 mkite_db-0.1.1/mkite_db/orm/structs/tests/
+-rw-r--r--   0 schwalbekoda1 (61642)    61642        0 2023-04-28 04:43:28.000000 mkite_db-0.1.1/mkite_db/orm/structs/tests/__init__.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     1508 2023-05-25 14:30:31.000000 mkite_db-0.1.1/mkite_db/orm/structs/tests/test_models.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     2119 2023-05-25 14:30:31.000000 mkite_db-0.1.1/mkite_db/orm/structs/tests/test_serializers.py
+drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-05-25 14:36:59.436536 mkite_db-0.1.1/mkite_db/orm/tests/
+-rw-r--r--   0 schwalbekoda1 (61642)    61642        0 2023-04-28 04:43:28.000000 mkite_db-0.1.1/mkite_db/orm/tests/__init__.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     1060 2023-05-25 14:30:31.000000 mkite_db-0.1.1/mkite_db/orm/tests/test_deserializers.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642      426 2023-05-25 14:30:31.000000 mkite_db-0.1.1/mkite_db/orm/tests/test_repr.py
+drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-05-25 14:36:59.436736 mkite_db-0.1.1/mkite_db/tests/
+-rw-r--r--   0 schwalbekoda1 (61642)    61642        0 2023-04-28 04:43:28.000000 mkite_db-0.1.1/mkite_db/tests/__init__.py
+drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-05-25 14:36:59.437016 mkite_db-0.1.1/mkite_db/tests/files/
+-rw-r--r--   0 schwalbekoda1 (61642)    61642        0 2023-04-28 04:43:28.000000 mkite_db-0.1.1/mkite_db/tests/files/__init__.py
+drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-05-25 14:36:59.438135 mkite_db-0.1.1/mkite_db/tests/files/dbimport/
+-rw-r--r--   0 schwalbekoda1 (61642)    61642        0 2023-04-28 04:43:28.000000 mkite_db-0.1.1/mkite_db/tests/files/dbimport/__init__.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     1378 2023-04-28 04:43:28.000000 mkite_db-0.1.1/mkite_db/tests/files/dbimport/caffeine.xyz
+-rw-r--r--   0 schwalbekoda1 (61642)    61642       94 2023-04-28 04:43:28.000000 mkite_db-0.1.1/mkite_db/tests/files/dbimport/molfile.yaml
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     4170 2023-04-28 04:43:28.000000 mkite_db-0.1.1/mkite_db/tests/files/dbimport/mp.json
+-rw-r--r--   0 schwalbekoda1 (61642)    61642      232 2023-04-28 04:43:28.000000 mkite_db-0.1.1/mkite_db/tests/files/dbimport/mp_query.json
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     5854 2023-04-28 04:43:28.000000 mkite_db-0.1.1/mkite_db/tests/files/dbimport/silicon.cif
+-rw-r--r--   0 schwalbekoda1 (61642)    61642       55 2023-04-28 04:43:28.000000 mkite_db-0.1.1/mkite_db/tests/files/engine.yaml
+drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-05-25 14:36:59.438620 mkite_db-0.1.1/mkite_db/tests/files/workflow/
+-rw-r--r--   0 schwalbekoda1 (61642)    61642        0 2023-04-28 04:43:28.000000 mkite_db-0.1.1/mkite_db/tests/files/workflow/__init__.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642      695 2023-04-28 04:43:28.000000 mkite_db-0.1.1/mkite_db/tests/files/workflow/create_rules.yaml
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     2328 2023-05-25 14:30:31.000000 mkite_db-0.1.1/mkite_db/tests/files/workflow/jobresults.json
+drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-05-25 14:36:59.439105 mkite_db-0.1.1/mkite_db/workflow/
+-rw-r--r--   0 schwalbekoda1 (61642)    61642        0 2023-04-28 04:43:28.000000 mkite_db-0.1.1/mkite_db/workflow/__init__.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642      157 2023-05-25 14:30:31.000000 mkite_db-0.1.1/mkite_db/workflow/apps.py
+drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-05-25 14:36:59.440001 mkite_db-0.1.1/mkite_db/workflow/create/
+-rw-r--r--   0 schwalbekoda1 (61642)    61642      202 2023-04-28 04:43:28.000000 mkite_db-0.1.1/mkite_db/workflow/create/__init__.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     3900 2023-05-25 14:30:31.000000 mkite_db-0.1.1/mkite_db/workflow/create/base.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     1521 2023-05-25 14:30:31.000000 mkite_db-0.1.1/mkite_db/workflow/create/simple.py
+drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-05-25 14:36:59.440523 mkite_db-0.1.1/mkite_db/workflow/create/tests/
+-rw-r--r--   0 schwalbekoda1 (61642)    61642        0 2023-04-28 04:43:28.000000 mkite_db-0.1.1/mkite_db/workflow/create/tests/__init__.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     3173 2023-05-25 14:30:31.000000 mkite_db-0.1.1/mkite_db/workflow/create/tests/test_simple.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     4572 2023-05-25 14:30:31.000000 mkite_db-0.1.1/mkite_db/workflow/create/tests/test_tuple.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     2579 2023-05-25 14:30:31.000000 mkite_db-0.1.1/mkite_db/workflow/create/tuple.py
+drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-05-25 14:36:59.440703 mkite_db-0.1.1/mkite_db/workflow/management/
+-rw-r--r--   0 schwalbekoda1 (61642)    61642        0 2023-04-28 04:43:28.000000 mkite_db-0.1.1/mkite_db/workflow/management/__init__.py
+drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-05-25 14:36:59.442006 mkite_db-0.1.1/mkite_db/workflow/management/commands/
+-rw-r--r--   0 schwalbekoda1 (61642)    61642        0 2023-04-28 04:43:28.000000 mkite_db-0.1.1/mkite_db/workflow/management/commands/__init__.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     3270 2023-05-25 14:30:31.000000 mkite_db-0.1.1/mkite_db/workflow/management/commands/create_from_file.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     4372 2023-05-25 14:30:31.000000 mkite_db-0.1.1/mkite_db/workflow/management/commands/create_simple.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     5057 2023-05-25 14:34:05.000000 mkite_db-0.1.1/mkite_db/workflow/management/commands/dbimport.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     3930 2023-05-25 14:34:35.000000 mkite_db-0.1.1/mkite_db/workflow/management/commands/parse.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     2928 2023-05-25 14:30:31.000000 mkite_db-0.1.1/mkite_db/workflow/management/commands/parse_file.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     4692 2023-05-25 14:30:31.000000 mkite_db-0.1.1/mkite_db/workflow/management/commands/submit.py
+drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-05-25 14:36:59.443207 mkite_db-0.1.1/mkite_db/workflow/management/commands/tests/
+-rw-r--r--   0 schwalbekoda1 (61642)    61642        0 2023-04-28 04:43:28.000000 mkite_db-0.1.1/mkite_db/workflow/management/commands/tests/__init__.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     1146 2023-05-25 14:30:31.000000 mkite_db-0.1.1/mkite_db/workflow/management/commands/tests/test_create_from_file.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     2208 2023-05-25 14:30:31.000000 mkite_db-0.1.1/mkite_db/workflow/management/commands/tests/test_create_simple.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     3650 2023-05-25 14:30:31.000000 mkite_db-0.1.1/mkite_db/workflow/management/commands/tests/test_dbimport.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     2322 2023-05-25 14:30:31.000000 mkite_db-0.1.1/mkite_db/workflow/management/commands/tests/test_parse.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     2427 2023-05-25 14:30:31.000000 mkite_db-0.1.1/mkite_db/workflow/management/commands/tests/test_parse_file.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     3406 2023-05-25 14:30:31.000000 mkite_db-0.1.1/mkite_db/workflow/management/commands/tests/test_submit.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     3008 2023-05-25 14:30:31.000000 mkite_db-0.1.1/mkite_db/workflow/parse.py
+drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-05-25 14:36:59.443520 mkite_db-0.1.1/mkite_db/workflow/tests/
+-rw-r--r--   0 schwalbekoda1 (61642)    61642        0 2023-04-28 04:43:28.000000 mkite_db-0.1.1/mkite_db/workflow/tests/__init__.py
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     2091 2023-05-25 14:30:31.000000 mkite_db-0.1.1/mkite_db/workflow/tests/test_parse.py
+drwxr-xr-x   0 schwalbekoda1 (61642)    61642        0 2023-05-25 14:36:59.423522 mkite_db-0.1.1/mkite_db.egg-info/
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     3172 2023-05-25 14:36:59.000000 mkite_db-0.1.1/mkite_db.egg-info/PKG-INFO
+-rw-r--r--   0 schwalbekoda1 (61642)    61642     4354 2023-05-25 14:36:59.000000 mkite_db-0.1.1/mkite_db.egg-info/SOURCES.txt
+-rw-r--r--   0 schwalbekoda1 (61642)    61642        1 2023-05-25 14:36:59.000000 mkite_db-0.1.1/mkite_db.egg-info/dependency_links.txt
+-rw-r--r--   0 schwalbekoda1 (61642)    61642       56 2023-05-25 14:36:59.000000 mkite_db-0.1.1/mkite_db.egg-info/entry_points.txt
+-rw-r--r--   0 schwalbekoda1 (61642)    61642      228 2023-05-25 14:36:59.000000 mkite_db-0.1.1/mkite_db.egg-info/requires.txt
+-rw-r--r--   0 schwalbekoda1 (61642)    61642        9 2023-05-25 14:36:59.000000 mkite_db-0.1.1/mkite_db.egg-info/top_level.txt
+-rw-r--r--   0 schwalbekoda1 (61642)    61642      883 2023-05-25 14:36:24.000000 mkite_db-0.1.1/pyproject.toml
+-rw-r--r--   0 schwalbekoda1 (61642)    61642      253 2023-04-28 17:03:10.000000 mkite_db-0.1.1/requirements.txt
+-rw-r--r--   0 schwalbekoda1 (61642)    61642       38 2023-05-25 14:36:59.444686 mkite_db-0.1.1/setup.cfg
+-rw-r--r--   0 schwalbekoda1 (61642)    61642       38 2023-04-28 05:37:26.000000 mkite_db-0.1.1/setup.py
```

### Comparing `mkite_db-0.1.0/.gitignore` & `mkite_db-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `mkite_db-0.1.0/CODE_OF_CONDUCT.md` & `mkite_db-0.1.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `mkite_db-0.1.0/LICENSE` & `mkite_db-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mkite_db-0.1.0/NOTICE` & `mkite_db-0.1.1/NOTICE`

 * *Files identical despite different names*

### Comparing `mkite_db-0.1.0/PKG-INFO` & `mkite_db-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkite_db
-Version: 0.1.0
+Version: 0.1.1
 Summary: mkite: distributed computing platform for high-throughput materials simulations
 Author-email: Daniel Schwalbe-Koda <dskoda@llnl.gov>
 Keywords: workflow,materials-science
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
```

### Comparing `mkite_db-0.1.0/README.md` & `mkite_db-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `mkite_db-0.1.0/docs/_static/mkite-logo.svg` & `mkite_db-0.1.1/docs/_static/mkite-logo.svg`

 * *Files identical despite different names*

### Comparing `mkite_db-0.1.0/docs/_static/mkite.png` & `mkite_db-0.1.1/docs/_static/mkite.png`

 * *Files identical despite different names*

### Comparing `mkite_db-0.1.0/mkite_db/cfg/settings.py` & `mkite_db-0.1.1/mkite_db/cfg/settings.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,49 +8,47 @@
         f"{MKITE_ENV_KEY} is not defined in the environment. \
         Without this variable, it is unclear what database \
         or settings to use. Please create a .env file and \
         point the {MKITE_ENV_KEY} file to it."
     )
 MKITE_ENV = os.environ[MKITE_ENV_KEY]
 if not os.path.exists(MKITE_ENV):
-    raise FileNotFoundError(
-        f"Could not find environment file {MKITE_ENV}."
-    )
+    raise FileNotFoundError(f"Could not find environment file {MKITE_ENV}.")
 
 # Reads the access to the database via environmental variables
 env = environ.Env(DEBUG=(bool, False))
 env.read_env(MKITE_ENV)
 
 BASE_DIR = Path(__file__).resolve().parent.parent
 DEBUG = env("DEBUG")
 SECRET_KEY = env("SECRET_KEY")
 ALLOWED_HOSTS = env.list("DJANGO_ALLOWED_HOSTS", default=["*"])
 
 # Sets up the database connection
-DATABASES = {'default': env.db()}
+DATABASES = {"default": env.db()}
 
 # Application definition
 DJANGO_APPS = [
     "django.contrib.admin",
     "django.contrib.auth",
     "django.contrib.contenttypes",
     "django.contrib.sessions",
     "django.contrib.messages",
     "django.contrib.staticfiles",
 ]
 
 THIRD_PARTY_APPS = ["django_extensions", "rest_framework", "taggit"]
 
 LOCAL_APPS = [
-    "mkite.orm.base",
-    "mkite.orm.jobs",
-    "mkite.orm.calcs",
-    "mkite.orm.mols",
-    "mkite.orm.structs",
-    "mkite.workflow",
+    "mkite_db.orm.base",
+    "mkite_db.orm.jobs",
+    "mkite_db.orm.calcs",
+    "mkite_db.orm.mols",
+    "mkite_db.orm.structs",
+    "mkite_db.workflow",
 ]
 
 INSTALLED_APPS = DJANGO_APPS + THIRD_PARTY_APPS + LOCAL_APPS
 
 MIDDLEWARE = [
     "django.middleware.security.SecurityMiddleware",
     "django.contrib.sessions.middleware.SessionMiddleware",
@@ -80,15 +78,17 @@
 ]
 
 WSGI_APPLICATION = "cfg.wsgi.application"
 
 
 # Password validation
 AUTH_PASSWORD_VALIDATORS = [
-    {"NAME": "django.contrib.auth.password_validation.UserAttributeSimilarityValidator"},
+    {
+        "NAME": "django.contrib.auth.password_validation.UserAttributeSimilarityValidator"
+    },
     {"NAME": "django.contrib.auth.password_validation.MinimumLengthValidator"},
     {"NAME": "django.contrib.auth.password_validation.CommonPasswordValidator"},
     {"NAME": "django.contrib.auth.password_validation.NumericPasswordValidator"},
 ]
 
 
 # Internationalization
```

### Comparing `mkite_db-0.1.0/mkite_db/cfg/urls.py` & `mkite_db-0.1.1/mkite_db/cfg/urls.py`

 * *Files identical despite different names*

### Comparing `mkite_db-0.1.0/mkite_db/dbimport/ase.py` & `mkite_db-0.1.1/mkite_db/dbimport/ase.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,41 +9,41 @@
 
 
 class AseFileImporter(DbImporter):
     RECIPE_DICT = {
         "name": "dbimport.AseFileImporter",
         "method": "EXT",
     }
-    PACKAGE_DICT = {"name": "mkite.dbimport"}
+    PACKAGE_DICT = {"name": "mkite_db.dbimport"}
 
     def query(self, filename: os.PathLike, **kwargs):
         """Opens the file provided and returns its contents.
         For now, does not perform any filtering."""
         raw_data = self.read(filename)
 
         return raw_data
 
     def read(self, filename: os.PathLike):
         """Reads whatever ASE can read"""
         return ase_read(filename, index=":")
 
     def convert(self, parsed: List[dict]) -> List[NodeResults]:
         """Converts the files into Infos, which is then converted into a
-        Node. 
+        Node.
         """
         return [self.convert_item(atoms) for atoms in parsed]
 
     def convert_item(self, atoms: Atoms) -> NodeResults:
         if atoms.pbc.any():
             info = self.get_crystal_info(atoms)
         else:
             info = self.get_conformer_info(atoms)
 
         return NodeResults(chemnode=info.as_dict())
-    
+
     def get_crystal_info(self, atoms: Atoms) -> CrystalInfo:
         return CrystalInfo.from_ase(atoms)
 
     def get_conformer_info(self, atoms: Atoms) -> ConformerInfo:
         if "smiles" in atoms.info:
             mol = MoleculeInfo.from_smiles(atoms.info["smiles"])
         else:
```

### Comparing `mkite_db-0.1.0/mkite_db/dbimport/base.py` & `mkite_db-0.1.1/mkite_db/dbimport/base.py`

 * *Files identical despite different names*

### Comparing `mkite_db-0.1.0/mkite_db/dbimport/molfile.py` & `mkite_db-0.1.1/mkite_db/dbimport/molfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 class MolFileImporter(DbImporter):
     RECIPE_DICT = {
         "name": "dbimport.MolFileImporter",
         "method": "EXT",
     }
-    PACKAGE_DICT = {"name": "mkite.dbimport"}
+    PACKAGE_DICT = {"name": "mkite_db.dbimport"}
 
     def query(self, **kwargs):
         """Opens the file provided and returns its contents.
         For now, does not perform any filtering."""
 
         if "filename" in kwargs:
             return self.read(kwargs["filename"])
```

### Comparing `mkite_db-0.1.0/mkite_db/dbimport/mp.py` & `mkite_db-0.1.1/mkite_db/dbimport/mp.py`

 * *Files identical despite different names*

### Comparing `mkite_db-0.1.0/mkite_db/dbimport/tests/test_ase.py` & `mkite_db-0.1.1/mkite_db/dbimport/tests/test_ase.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import unittest as ut
 from pkg_resources import resource_filename
 
 from ase import Atoms
 from ase.io import read
 from mkite_core.models import CrystalInfo, ConformerInfo, NodeResults
-from mkite.dbimport.ase import AseFileImporter
+from mkite_db.dbimport.ase import AseFileImporter
 
 
-CIF_FILE = resource_filename("mkite.tests.files.dbimport", "silicon.cif")
-XYZ_FILE = resource_filename("mkite.tests.files.dbimport", "caffeine.xyz")
+CIF_FILE = resource_filename("mkite_db.tests.files.dbimport", "silicon.cif")
+XYZ_FILE = resource_filename("mkite_db.tests.files.dbimport", "caffeine.xyz")
 
 
 class TestAseFileImporter(ut.TestCase):
     def setUp(self):
         self.dbimp = AseFileImporter(
             project="test_prj",
             experiment="test_exp",
```

### Comparing `mkite_db-0.1.0/mkite_db/dbimport/tests/test_molfile.py` & `mkite_db-0.1.1/mkite_db/dbimport/tests/test_molfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import os
 import unittest as ut
 from mkite_core.external import load_config
 from unittest.mock import MagicMock
 from pkg_resources import resource_filename
 
 from mkite_core.models import MoleculeInfo, NodeResults, JobResults
-from mkite.dbimport.molfile import MolFileImporter
+from mkite_db.dbimport.molfile import MolFileImporter
 
 
-MOLFILE = resource_filename("mkite.tests.files.dbimport", "molfile.yaml")
+MOLFILE = resource_filename("mkite_db.tests.files.dbimport", "molfile.yaml")
 
 
 class TestMolFileImporter(ut.TestCase):
     def setUp(self):
         self.dbimp = MolFileImporter(
             project="test_prj",
             experiment="test_exp",
```

### Comparing `mkite_db-0.1.0/mkite_db/dbimport/tests/test_mp.py` & `mkite_db-0.1.1/mkite_db/dbimport/tests/test_mp.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 import unittest as ut
 from unittest.mock import MagicMock
 from monty.serialization import loadfn
 from pkg_resources import resource_filename
 
 from pymatgen.core import Structure
 from mkite_core.models import CrystalInfo, EnergyForcesInfo, NodeResults, JobResults
-from mkite.dbimport.mp import MPImporter, MP_KEY
+from mkite_db.dbimport.mp import MPImporter, MP_KEY
 
 
-RESPONSE_PATH = resource_filename("mkite.tests.files.dbimport", "mp.json")
+RESPONSE_PATH = resource_filename("mkite_db.tests.files.dbimport", "mp.json")
 
 
 class MockDoc(dict):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.__dict__ = self
 
@@ -104,15 +104,15 @@
         self.assertEqual(job, expected)
 
     def test_import_data(self):
         results = self.dbimp.import_data(
             project="test_prj",
             experiment="test_exp",
             isroot=True,
-            **self.get_query_args()
+            **self.get_query_args(),
         )
         self.assertIsInstance(results, JobResults)
 
     @ut.skip
     @ut.skipIf(MP_KEY not in os.environ, "MP_KEY not in environment")
     def test_connection(self):
         raise NotImplementedError("Test TO-DO")
```

### Comparing `mkite_db-0.1.0/mkite_db/manage.py` & `mkite_db-0.1.1/mkite_db/manage.py`

 * *Files identical despite different names*

### Comparing `mkite_db-0.1.0/mkite_db/orm/base/models.py` & `mkite_db-0.1.1/mkite_db/orm/base/models.py`

 * *Files identical despite different names*

### Comparing `mkite_db-0.1.0/mkite_db/orm/base/serializers.py` & `mkite_db-0.1.1/mkite_db/orm/base/serializers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from rest_framework import serializers
 
-from mkite.orm.serializers import BaseSerializer
-from mkite.orm.jobs.serializers import JobSerializer
+from mkite_db.orm.serializers import BaseSerializer
+from mkite_db.orm.jobs.serializers import JobSerializer
 from .models import Formula, ChemNode, CalcNode
 
 
 class FormulaSerializer(BaseSerializer):
     class Meta:
         model = Formula
         fields = "__all__"
```

### Comparing `mkite_db-0.1.0/mkite_db/orm/base/tests/test_models.py` & `mkite_db-0.1.1/mkite_db/orm/base/tests/test_models.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from model_bakery import baker
 from datetime import timedelta
 from django.test import TestCase
-from mkite.orm.base.models import (
+from mkite_db.orm.base.models import (
     ChemNode,
     CalcNode,
     Formula,
     Elements,
 )
```

### Comparing `mkite_db-0.1.0/mkite_db/orm/base/tests/test_serializers.py` & `mkite_db-0.1.1/mkite_db/orm/base/tests/test_serializers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from model_bakery import baker
 from django.test import TestCase
 
-from mkite.orm.base.models import Formula, ChemNode, CalcNode
-from mkite.orm.jobs.models import Job
-from mkite.orm.jobs.serializers import JobSerializer
-from mkite.orm.base.serializers import (
+from mkite_db.orm.base.models import Formula, ChemNode, CalcNode
+from mkite_db.orm.jobs.models import Job
+from mkite_db.orm.jobs.serializers import JobSerializer
+from mkite_db.orm.base.serializers import (
     FormulaSerializer,
     ChemNodeSerializer,
     CalcNodeSerializer,
 )
 
 
 class TestFormulaSerializer(TestCase):
@@ -22,15 +22,15 @@
     def test_serialize(self):
         f = baker.make(Formula, **self.dict)
         serial = FormulaSerializer(f)
         data = serial.data
 
         self.assertTrue("id" in data)
         expected = {
-            "@module": "mkite.orm.base.models",
+            "@module": "mkite_db.orm.base.models",
             "@class": "Formula",
             "name": "H20 C8 N1 +1",
             "charge": 1,
         }
         for k, v in expected.items():
             self.assertEqual(data[k], v)
 
@@ -45,44 +45,44 @@
         self.assertEqual(new.charge, self.dict["charge"])
 
 
 class TestChemSerializer(TestCase):
     def test_deserialize(self):
         job = baker.make(Job)
         data = {
-            "@module": "mkite.orm.base.models",
+            "@module": "mkite_db.orm.base.models",
             "@class": "ChemNode",
             "parentjob": {"id": job.id},
         }
         serial = ChemNodeSerializer(data=data)
         self.assertTrue(serial.is_valid())
 
         new = serial.save()
         self.assertEqual(new.parentjob, job)
 
     def test_serialize(self):
         node = baker.make(ChemNode)
         jobdata = JobSerializer(node.parentjob).data
         expected = {
-            "@module": "mkite.orm.base.models",
+            "@module": "mkite_db.orm.base.models",
             "@class": "ChemNode",
             "parentjob": jobdata,
             "id": node.id,
             "uuid": str(node.uuid),
         }
         serial = ChemNodeSerializer(node)
 
         self.assertEqual(serial.data, expected)
 
 
 class TestCalcSerializer(TestCase):
     def test_deserialize(self):
         chem = baker.make(ChemNode)
         data = {
-            "@module": "mkite.orm.base.models",
+            "@module": "mkite_db.orm.base.models",
             "@class": "CalcNode",
             "parentjob": {"id": chem.parentjob.id},
             "chemnode": {"id": chem.id},
         }
         serial = CalcNodeSerializer(data=data)
         self.assertTrue(serial.is_valid())
 
@@ -91,15 +91,15 @@
         self.assertEqual(new.parentjob, chem.parentjob)
 
     def test_serialize(self):
         node = baker.make(CalcNode)
         jobdata = JobSerializer(node.parentjob).data
         chemdata = ChemNodeSerializer(node.chemnode).data
         expected = {
-            "@module": "mkite.orm.base.models",
+            "@module": "mkite_db.orm.base.models",
             "@class": "CalcNode",
             "parentjob": jobdata,
             "chemnode": chemdata,
             "id": node.id,
             "uuid": str(node.uuid),
         }
         serial = CalcNodeSerializer(node)
```

### Comparing `mkite_db-0.1.0/mkite_db/orm/calcs/serializers.py` & `mkite_db-0.1.1/mkite_db/orm/calcs/serializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from django.db import transaction
 from rest_framework import serializers
 
-from mkite.orm.base.serializers import CalcNodeSerializer
+from mkite_db.orm.base.serializers import CalcNodeSerializer
 
 from .models import EnergyForces, Feature
 
 
 class EnergyForcesSerializer(CalcNodeSerializer):
     class Meta:
         model = EnergyForces
```

### Comparing `mkite_db-0.1.0/mkite_db/orm/calcs/tests/test_serializers.py` & `mkite_db-0.1.1/mkite_db/orm/calcs/tests/test_serializers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 import unittest as ut
 from model_bakery import baker
 from django.test import TestCase
 
-from mkite.orm.base.models import ChemNode
-from mkite.orm.base.serializers import ChemNodeSerializer
-from mkite.orm.jobs.models import Job
-from mkite.orm.jobs.serializers import JobSerializer
-from mkite.orm.calcs.models import Feature, EnergyForces
-from mkite.orm.calcs.serializers import EnergyForcesSerializer, FeatureSerializer
+from mkite_db.orm.base.models import ChemNode
+from mkite_db.orm.base.serializers import ChemNodeSerializer
+from mkite_db.orm.jobs.models import Job
+from mkite_db.orm.jobs.serializers import JobSerializer
+from mkite_db.orm.calcs.models import Feature, EnergyForces
+from mkite_db.orm.calcs.serializers import EnergyForcesSerializer, FeatureSerializer
 
 
 class TestFeatureSerializer(TestCase):
     @property
     def dict(self):
         return {"value": [1.0, 1.0, 0.0]}
 
     def test_serialize(self):
         f = baker.make(Feature, **self.dict)
         serial = FeatureSerializer(f)
         data = serial.data
 
         expected = {
-            "@module": "mkite.orm.calcs.models",
+            "@module": "mkite_db.orm.calcs.models",
             "@class": "Feature",
             **self.dict,
         }
         for k, v in expected.items():
             self.assertEqual(data[k], v)
 
         expected_keys = ["parentjob", "chemnode"]
         for key in expected_keys:
             self.assertTrue(key in data)
 
     def test_deserialize(self):
         chemnode = baker.make(ChemNode)
         data = {
-            "@module": "mkite.orm.calcs.models",
+            "@module": "mkite_db.orm.calcs.models",
             "@class": "Feature",
             "parentjob": {"id": chemnode.parentjob.id},
             "chemnode": {"id": chemnode.id},
             **self.dict,
         }
         serial = FeatureSerializer(data=data)
 
@@ -50,15 +50,15 @@
         self.assertEqual(new.value, self.dict["value"])
 
 
 class TestEnergyForcesSerializer(TestCase):
     def test_deserialize(self):
         chem = baker.make(ChemNode)
         data = {
-            "@module": "mkite.orm.calcs.models",
+            "@module": "mkite_db.orm.calcs.models",
             "@class": "EnergyForces",
             "parentjob": {"id": chem.parentjob.id},
             "chemnode": {"id": chem.id},
             "energy": -1,
             "forces": [[0, 0, 0]],
         }
         serial = EnergyForcesSerializer(data=data)
@@ -77,13 +77,13 @@
         expected = {
             "id": node.id,
             "uuid": str(node.uuid),
             "parentjob": jobdata,
             "chemnode": chemdata,
             "energy": node.energy,
             "forces": node.forces,
-            "@module": "mkite.orm.calcs.models",
+            "@module": "mkite_db.orm.calcs.models",
             "@class": "EnergyForces",
         }
         serial = EnergyForcesSerializer(node)
 
         self.assertEqual(serial.data, expected)
```

### Comparing `mkite_db-0.1.0/mkite_db/orm/deserializers.py` & `mkite_db-0.1.1/mkite_db/orm/deserializers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from mkite.orm.base.serializers import (
+from mkite_db.orm.base.serializers import (
     FormulaSerializer,
     ChemNodeSerializer,
     CalcNodeSerializer,
 )
-from mkite.orm.calcs.serializers import (
+from mkite_db.orm.calcs.serializers import (
     EnergyForcesSerializer,
     FeatureSerializer,
 )
-from mkite.orm.structs.serializers import CrystalSerializer
-from mkite.orm.mols.serializers import (
+from mkite_db.orm.structs.serializers import CrystalSerializer
+from mkite_db.orm.mols.serializers import (
     MoleculeSerializer,
     ConformerSerializer,
 )
-from mkite.orm.jobs.serializers import (
+from mkite_db.orm.jobs.serializers import (
     ProjectSerializer,
     ExperimentSerializer,
     JobPackageSerializer,
     JobRecipeSerializer,
     RunStatsSerializer,
     JobSerializer,
 )
```

### Comparing `mkite_db-0.1.0/mkite_db/orm/jobs/management/commands/create_experiment.py` & `mkite_db-0.1.1/mkite_db/orm/jobs/management/commands/create_experiment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from django.core.management.base import BaseCommand, CommandError
 
-from mkite.orm.jobs.models import Project, Experiment
+from mkite_db.orm.jobs.models import Project, Experiment
 
 
 class Command(BaseCommand):
     help = "Adds a new experiment to the database"
 
     def log(self, style, msg):
         style_fn = getattr(self.style, style.upper())
```

### Comparing `mkite_db-0.1.0/mkite_db/orm/jobs/management/commands/create_project.py` & `mkite_db-0.1.1/mkite_db/orm/jobs/management/commands/create_project.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from django.core.management.base import BaseCommand
 
-from mkite.orm.jobs.models import Project
+from mkite_db.orm.jobs.models import Project
 
 
 class Command(BaseCommand):
     help = "Adds a new project to the database"
 
     def log(self, style, msg):
         style_fn = getattr(self.style, style.upper())
```

### Comparing `mkite_db-0.1.0/mkite_db/orm/jobs/management/commands/scanrecipes.py` & `mkite_db-0.1.1/mkite_db/orm/jobs/management/commands/scanrecipes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from importlib import metadata
 from django.core.management.base import BaseCommand, CommandError
 
 from mkite_core.plugins import get_recipes
-from mkite.orm.jobs.models import JobRecipe
-from mkite.orm.jobs.serializers import JobRecipeSerializer
+from mkite_db.orm.jobs.models import JobRecipe
+from mkite_db.orm.jobs.serializers import JobRecipeSerializer
 
 
 class Command(BaseCommand):
     help = "Creates jobs according to the given input/output recipes"
 
     def log(self, style, msg):
         style_fn = getattr(self.style, style.upper())
@@ -18,15 +18,15 @@
             "--dry_run",
             action="store_true",
             help="If set, does not store objects into the database",
         )
         return argparser
 
     def handle(self, *args, dry_run=False, **kwargs):
-        self.log("notice", f"Scanning entry point mkite.recipes...")
+        self.log("notice", f"Scanning entry point mkite_db.recipes...")
         recipes = get_recipes()
 
         new_recipes = []
         for name, entry in recipes.items():
             new = self.add_entry_point(name, entry, dry_run=dry_run)
             if new is not None:
                 new_recipes.append(new)
```

### Comparing `mkite_db-0.1.0/mkite_db/orm/jobs/models.py` & `mkite_db-0.1.1/mkite_db/orm/jobs/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from datetime import timedelta
 from django.db import models
 from django.core.serializers.json import DjangoJSONEncoder
 
-from mkite.orm.repr import _named_repr
-from mkite.orm.base.models import DbEntry
+from mkite_db.orm.repr import _named_repr
+from mkite_db.orm.base.models import DbEntry
 from taggit.managers import TaggableManager
 
 
 class Project(DbEntry):
     name = models.CharField(max_length=32, unique=True)
     description = models.CharField(max_length=256, null=True)
```

### Comparing `mkite_db-0.1.0/mkite_db/orm/jobs/serializers.py` & `mkite_db-0.1.1/mkite_db/orm/jobs/serializers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from datetime import timedelta
 from rest_framework import serializers
 
 from taggit.serializers import TagListSerializerField, TaggitSerializer
-from mkite.orm.serializers import BaseSerializer
+from mkite_db.orm.serializers import BaseSerializer
 
 from .models import Project, Experiment, Job, JobRecipe, JobPackage, RunStats
 
 
 class ProjectSerializer(BaseSerializer):
     description = serializers.CharField(required=False)
```

### Comparing `mkite_db-0.1.0/mkite_db/orm/jobs/tests/test_deleter.py` & `mkite_db-0.1.1/mkite_db/orm/jobs/tests/test_deleter.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import unittest as ut
 from django.test import TestCase
 from model_bakery import baker
 
-from mkite.orm.models import Crystal, Job, RunStats
-from mkite.orm.jobs.deleter import delete_tree
+from mkite_db.orm.models import Crystal, Job, RunStats
+from mkite_db.orm.jobs.deleter import delete_tree
 
 
 class TestDeleter(TestCase):
     def setUp(self):
         """Creates a tree of jobs"""
         self.node1 = baker.make(Crystal)
         self.node2 = baker.make(Crystal)
```

### Comparing `mkite_db-0.1.0/mkite_db/orm/jobs/tests/test_models.py` & `mkite_db-0.1.1/mkite_db/orm/jobs/tests/test_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from datetime import timedelta
 from django.test import TestCase
-from mkite.orm.jobs.models import (
+from mkite_db.orm.jobs.models import (
     Project,
     Experiment,
     JobStatus,
     Job,
     JobRecipe,
     JobPackage,
     RunStats,
```

### Comparing `mkite_db-0.1.0/mkite_db/orm/jobs/tests/test_serializers.py` & `mkite_db-0.1.1/mkite_db/orm/jobs/tests/test_serializers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import unittest as ut
 from datetime import timedelta
 from model_bakery import baker
 from django.test import TestCase
 from rest_framework import serializers
 from collections.abc import Mapping
 
-from mkite.orm.jobs.models import (
+from mkite_db.orm.jobs.models import (
     Project,
     Experiment,
     JobPackage,
     JobRecipe,
     RunStats,
     Job,
     JobStatus,
 )
-from mkite.orm.jobs.serializers import (
+from mkite_db.orm.jobs.serializers import (
     ProjectSerializer,
     ExperimentSerializer,
     JobPackageSerializer,
     JobRecipeSerializer,
     RunStatsSerializer,
     JobSerializer,
 )
```

### Comparing `mkite_db-0.1.0/mkite_db/orm/mols/models.py` & `mkite_db-0.1.1/mkite_db/orm/mols/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from django.db import models
 from django.contrib.postgres.fields import ArrayField
 
 from taggit.managers import TaggableManager
-from mkite.orm.repr import _named_repr
-from mkite.orm.base.models import DbEntry, ChemNode, Elements, Formula
+from mkite_db.orm.repr import _named_repr
+from mkite_db.orm.base.models import DbEntry, ChemNode, Elements, Formula
 
 
 class Molecule(ChemNode):
     """Class to hold the information of molecular graphs"""
 
     formula = models.ForeignKey(
         Formula,
```

### Comparing `mkite_db-0.1.0/mkite_db/orm/mols/serializers.py` & `mkite_db-0.1.1/mkite_db/orm/mols/serializers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from django.db import transaction
 from rest_framework import serializers
 
 from taggit.serializers import TagListSerializerField, TaggitSerializer
-from mkite.orm.serializers import BaseSerializer
-from mkite.orm.base.models import Formula
-from mkite.orm.base.serializers import FormulaSerializer, ChemNodeSerializer
+from mkite_db.orm.serializers import BaseSerializer
+from mkite_db.orm.base.models import Formula
+from mkite_db.orm.base.serializers import FormulaSerializer, ChemNodeSerializer
 
 from .models import Molecule, Conformer
 
 
 class MoleculeSerializer(TaggitSerializer, ChemNodeSerializer):
     formula = FormulaSerializer(nested_field=True, required=False)
     tags = TagListSerializerField(required=False)
```

### Comparing `mkite_db-0.1.0/mkite_db/orm/mols/tests/test_models.py` & `mkite_db-0.1.1/mkite_db/orm/mols/tests/test_models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from model_bakery import baker
 from django.test import TestCase
 
-from mkite.orm.base.models import Formula
-from mkite.orm.jobs.models import Job
-from mkite.orm.mols.models import Molecule, Conformer
+from mkite_db.orm.base.models import Formula
+from mkite_db.orm.jobs.models import Job
+from mkite_db.orm.mols.models import Molecule, Conformer
 
 
 class MolCreator:
     def create_formula(self):
         formula, _ = Formula.objects.get_or_create(name="C9 H8 O4 +0", charge=0)
         return formula
 
@@ -75,15 +75,15 @@
         self.assertEqual(formula.name, "C9 H8 O4 +0")
 
     def test_molecule_dict(self):
         mol = self.creator.create_molecule()
         data = mol.as_dict()
 
         expected = {
-            "@module": "mkite.orm.mols.models",
+            "@module": "mkite_db.orm.mols.models",
             "@class": "Molecule",
             "id": mol.id,
             "uuid": str(mol.uuid),
             "ctime": mol.ctime,
             "mtime": mol.mtime,
             "parentjob": mol.parentjob.id,
             "chemnode_ptr": mol.chemnode_ptr.id,
```

### Comparing `mkite_db-0.1.0/mkite_db/orm/mols/tests/test_serializers.py` & `mkite_db-0.1.1/mkite_db/orm/mols/tests/test_serializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 from model_bakery import baker
 from django.test import TestCase
 from pkg_resources import resource_filename
 
-from mkite.orm.base.models import Formula
-from mkite.orm.jobs.models import Job
-from mkite.orm.mols.models import Molecule, Conformer
-from mkite.orm.mols.serializers import (
+from mkite_db.orm.base.models import Formula
+from mkite_db.orm.jobs.models import Job
+from mkite_db.orm.mols.models import Molecule, Conformer
+from mkite_db.orm.mols.serializers import (
     MoleculeSerializer,
     ConformerSerializer,
 )
 
 from .test_models import MolCreator
```

### Comparing `mkite_db-0.1.0/mkite_db/orm/serializers.py` & `mkite_db-0.1.1/mkite_db/orm/serializers.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
         self.nested_field = nested_field
         if nested_field:
             self._setup_serializer_as_field()
 
     def _setup_serializer_as_field(self):
         """Useful to bypass validation when nested serializers are used
-        in mkite. Ensures then that the rest of the validation is
+        in mkite_db. Ensures then that the rest of the validation is
         performed by the user at the creation/update stage.
         """
         for field_name, field in self.fields.items():
             field.required = False
             field.read_only = False
             if field_name in self.id_fields:
                 field.validators = []
```

### Comparing `mkite_db-0.1.0/mkite_db/orm/structs/models.py` & `mkite_db-0.1.1/mkite_db/orm/structs/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from django.db import models
 from django.contrib.postgres.fields import ArrayField
 from django.utils.translation import gettext_lazy as lazy
 
 from taggit.managers import TaggableManager
-from mkite.orm.repr import _named_repr
-from mkite.orm.base.models import DbEntry, ChemNode, Elements, Formula
+from mkite_db.orm.repr import _named_repr
+from mkite_db.orm.base.models import DbEntry, ChemNode, Elements, Formula
 
 
 class SpaceGroups(models.IntegerChoices):
     S1 = 1, lazy("P1")
     S2 = 2, lazy("P-1")
     S3 = 3, lazy("P2")
     S4 = 4, lazy("P21")
```

### Comparing `mkite_db-0.1.0/mkite_db/orm/structs/serializers.py` & `mkite_db-0.1.1/mkite_db/orm/structs/serializers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from django.db import transaction
 from rest_framework import serializers
 
 from taggit.serializers import TagListSerializerField, TaggitSerializer
-from mkite.orm.serializers import BaseSerializer
-from mkite.orm.base.models import Formula
-from mkite.orm.base.serializers import FormulaSerializer, ChemNodeSerializer
+from mkite_db.orm.serializers import BaseSerializer
+from mkite_db.orm.base.models import Formula
+from mkite_db.orm.base.serializers import FormulaSerializer, ChemNodeSerializer
 from mkite_core.models import FormulaInfo, CrystalInfo, SpaceGroupInfo
 
 from .models import Crystal, SpaceGroups
 
 
 class CrystalSerializer(TaggitSerializer, ChemNodeSerializer):
     spacegroup = serializers.ChoiceField(SpaceGroups.choices, required=False)
```

### Comparing `mkite_db-0.1.0/mkite_db/orm/structs/tests/test_models.py` & `mkite_db-0.1.1/mkite_db/orm/structs/tests/test_models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from model_bakery import baker
 from django.test import TestCase
 
-from mkite.orm.base.models import Formula
-from mkite.orm.jobs.models import Job
-from mkite.orm.structs.models import Crystal, SpaceGroups
+from mkite_db.orm.base.models import Formula
+from mkite_db.orm.jobs.models import Job
+from mkite_db.orm.structs.models import Crystal, SpaceGroups
 from mkite_core.models import CrystalInfo
 
 
 class CrystalCreator:
     def create_formula(self):
         formula, _ = Formula.objects.get_or_create(
             name="Si2 +0",
```

### Comparing `mkite_db-0.1.0/mkite_db/orm/structs/tests/test_serializers.py` & `mkite_db-0.1.1/mkite_db/orm/structs/tests/test_serializers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from model_bakery import baker
 from django.test import TestCase
 
-from mkite.orm.base.models import Formula
-from mkite.orm.jobs.models import Job
-from mkite.orm.structs.serializers import CrystalSerializer
+from mkite_db.orm.base.models import Formula
+from mkite_db.orm.jobs.models import Job
+from mkite_db.orm.structs.serializers import CrystalSerializer
 
 from .test_models import CrystalCreator
 
 
 class TestCrystalSerializer(TestCase):
     def setUp(self):
         self.creator = CrystalCreator()
```

### Comparing `mkite_db-0.1.0/mkite_db/orm/tests/test_deserializers.py` & `mkite_db-0.1.1/mkite_db/orm/tests/test_deserializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 from django.test import TestCase
 from pkg_resources import resource_filename
 
-from mkite.orm.deserializers import get_serializer
-from mkite.orm.mols.models import Molecule
-from mkite.orm.structs.models import Crystal
+from mkite_db.orm.deserializers import get_serializer
+from mkite_db.orm.mols.models import Molecule
+from mkite_db.orm.structs.models import Crystal
 
 
 MOL_JSON = resource_filename("mkite_core.tests.files.models", "molecule.json")
 CRYSTAL_JSON = resource_filename("mkite_core.tests.files.models", "crystal.json")
 
 
 def load_json(filename):
```

### Comparing `mkite_db-0.1.0/mkite_db/tests/files/dbimport/caffeine.xyz` & `mkite_db-0.1.1/mkite_db/tests/files/dbimport/caffeine.xyz`

 * *Files identical despite different names*

### Comparing `mkite_db-0.1.0/mkite_db/tests/files/dbimport/mp.json` & `mkite_db-0.1.1/mkite_db/tests/files/dbimport/mp.json`

 * *Files identical despite different names*

### Comparing `mkite_db-0.1.0/mkite_db/tests/files/dbimport/silicon.cif` & `mkite_db-0.1.1/mkite_db/tests/files/dbimport/silicon.cif`

 * *Files identical despite different names*

### Comparing `mkite_db-0.1.0/mkite_db/tests/files/workflow/create_rules.yaml` & `mkite_db-0.1.1/mkite_db/tests/files/workflow/create_rules.yaml`

 * *Files identical despite different names*

### Comparing `mkite_db-0.1.0/mkite_db/tests/files/workflow/jobresults.json` & `mkite_db-0.1.1/mkite_db/tests/files/workflow/jobresults.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9913194444444443%*

 * *Differences: {"'nodes'": "{0: {'chemnode': {'@module': 'mkite_db.orm.structs.models'}, 'calcnodes': {0: "*

 * *            "{'@module': 'mkite_db.orm.calcs.models'}}}}"}*

```diff
@@ -23,15 +23,15 @@
         "status": "D"
     },
     "nodes": [
         {
             "calcnodes": [
                 {
                     "@class": "EnergyForces",
-                    "@module": "mkite.orm.calcs.models",
+                    "@module": "mkite_db.orm.calcs.models",
                     "energy": -10.84136528,
                     "forces": [
                         [
                             0,
                             0,
                             0
                         ],
@@ -41,15 +41,15 @@
                             0
                         ]
                     ]
                 }
             ],
             "chemnode": {
                 "@class": "Crystal",
-                "@module": "mkite.orm.structs.models",
+                "@module": "mkite_db.orm.structs.models",
                 "attributes": {},
                 "coords": [
                     [
                         0,
                         0,
                         0
                     ],
```

### Comparing `mkite_db-0.1.0/mkite_db/workflow/create/base.py` & `mkite_db-0.1.1/mkite_db/workflow/create/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List, Dict, Union, Iterable, Tuple
 from abc import ABC, abstractmethod
 from pydantic import BaseModel, Field
 
-from mkite.orm.base.models import ChemNode
-from mkite.orm.jobs.models import Job, JobRecipe, Experiment
+from mkite_db.orm.base.models import ChemNode
+from mkite_db.orm.jobs.models import Job, JobRecipe, Experiment
 
 
 class JobCreationError(Exception):
     pass
 
 
 class InputQuery(BaseModel):
```

### Comparing `mkite_db-0.1.0/mkite_db/workflow/create/simple.py` & `mkite_db-0.1.1/mkite_db/workflow/create/simple.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import List, Tuple
 
 from django.db.models import QuerySet
-from mkite.orm.base.models import ChemNode
-from mkite.orm.jobs.models import Job
+from mkite_db.orm.base.models import ChemNode
+from mkite_db.orm.jobs.models import Job
 
 from .base import BaseJobCreator, JobCreationError
 
 
 class SimpleJobCreator(BaseJobCreator):
     def get_inputs(self) -> "QuerySet[ChemNode]":
         if len(self.inputs) != 1:
```

### Comparing `mkite_db-0.1.0/mkite_db/workflow/create/tests/test_simple.py` & `mkite_db-0.1.1/mkite_db/workflow/create/tests/test_simple.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import os
 import shutil
 import unittest as ut
 from model_bakery import baker
 from unittest.mock import patch
 from django.test import TestCase
 
-from mkite.orm.base.models import ChemNode
-from mkite.orm.structs.models import Crystal
-from mkite.orm.jobs.models import Job, JobStatus, JobRecipe, Experiment
+from mkite_db.orm.base.models import ChemNode
+from mkite_db.orm.structs.models import Crystal
+from mkite_db.orm.jobs.models import Job, JobStatus, JobRecipe, Experiment
 
-from mkite.workflow.create import InputQuery
-from mkite.workflow.create.simple import SimpleJobCreator
+from mkite_db.workflow.create import InputQuery
+from mkite_db.workflow.create.simple import SimpleJobCreator
 
 
 class TestJobCreator(TestCase):
     @classmethod
     def setUpClass(cls):
         super(TestJobCreator, cls).setUpClass()
         cls.inp_recipe = baker.make(JobRecipe)
```

### Comparing `mkite_db-0.1.0/mkite_db/workflow/create/tests/test_tuple.py` & `mkite_db-0.1.1/mkite_db/workflow/create/tests/test_tuple.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import unittest as ut
 from model_bakery import baker
 from unittest.mock import patch
 from django.test import TestCase
 
-from mkite.orm.base.models import ChemNode
-from mkite.orm.structs.models import Crystal
-from mkite.orm.jobs.models import Job, JobStatus, JobRecipe, Experiment
+from mkite_db.orm.base.models import ChemNode
+from mkite_db.orm.structs.models import Crystal
+from mkite_db.orm.jobs.models import Job, JobStatus, JobRecipe, Experiment
 
-from mkite.workflow.create import InputQuery
-from mkite.workflow.create.tuple import TupleJobCreator
+from mkite_db.workflow.create import InputQuery
+from mkite_db.workflow.create.tuple import TupleJobCreator
 
 
 class TestJobCreator(TestCase):
     @classmethod
     def setUpClass(cls):
         super(TestJobCreator, cls).setUpClass()
         cls.recipe_1 = baker.make(JobRecipe)
```

### Comparing `mkite_db-0.1.0/mkite_db/workflow/create/tuple.py` & `mkite_db-0.1.1/mkite_db/workflow/create/tuple.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import itertools
 from typing import List, Dict, Tuple
 
 from django.db.models import QuerySet
-from mkite.orm.base.models import ChemNode
-from mkite.orm.jobs.models import Job
+from mkite_db.orm.base.models import ChemNode
+from mkite_db.orm.jobs.models import Job
 
 from .base import BaseJobCreator, JobCreationError
 
 
 class TupleJobCreator(BaseJobCreator):
     def get_inputs(self) -> "List[QuerySet[ChemNode]]":
         inp_qs = self.get_input_queries()
```

### Comparing `mkite_db-0.1.0/mkite_db/workflow/management/commands/create_from_file.py` & `mkite_db-0.1.1/mkite_db/workflow/management/commands/create_from_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from typing import List
 from mkite_core.external import load_config
 from django.core.management.base import BaseCommand, CommandError
 
-from mkite.workflow.create import InputQuery, JOB_CREATORS
+from mkite_db.workflow.create import InputQuery, JOB_CREATORS
 
 
 class Command(BaseCommand):
     help = "Creates jobs according to the given input/output recipes"
 
     def log(self, style, msg):
         style_fn = getattr(self.style, style.upper())
```

### Comparing `mkite_db-0.1.0/mkite_db/workflow/management/commands/create_simple.py` & `mkite_db-0.1.1/mkite_db/workflow/management/commands/create_simple.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 from typing import List
 from django.db import transaction
 from django.core.management.base import BaseCommand, CommandError
 
-from mkite.workflow.create import InputQuery, SimpleJobCreator
+from mkite_db.workflow.create import InputQuery, SimpleJobCreator
 
 
 class Command(BaseCommand):
     help = "Creates jobs according to the given input/output recipes"
 
     def log(self, style, msg):
         style_fn = getattr(self.style, style.upper())
```

### Comparing `mkite_db-0.1.0/mkite_db/workflow/management/commands/dbimport.py` & `mkite_db-0.1.1/mkite_db/workflow/management/commands/dbimport.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import os
 import json
 from typing import List
 from mkite_core.external import load_config
 from django.core.management.base import BaseCommand, CommandError
 
-from mkite import dbimport as dbimp
 from mkite_core.models import JobResults
-from mkite.workflow.parse import JobParser
+from mkite_db import dbimport as dbimp
+from mkite_db.workflow.parse import JobParser
 
-from mkite.orm.jobs.models import Job
+from mkite_db.orm.jobs.models import Job
 
 
 DB_IMPORTERS = {cls.__name__: cls for cls in dbimp.DbImporter.__subclasses__()}
 
 
 class Command(BaseCommand):
     help = "Parses another database into the mkite database"
```

### Comparing `mkite_db-0.1.0/mkite_db/workflow/management/commands/parse.py` & `mkite_db-0.1.1/mkite_db/workflow/management/commands/parse.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 from typing import Iterable
 from django.core.management.base import BaseCommand, CommandError
 
 from mkite_core.models import JobResults
-from mkite.workflow.parse import JobParser
+from mkite_db.workflow.parse import JobParser
 from mkite_engines import Status, EngineRoles, instantiate_from_path
 
-from mkite.orm.jobs.models import Job
+from mkite_db.orm.jobs.models import Job
 
 
 class Command(BaseCommand):
     help = "Parses the job results from a folder into the database"
 
     def log(self, style, msg):
         style_fn = getattr(self.style, style.upper())
@@ -27,17 +27,15 @@
             "--num_parse",
             type=int,
             default=1000,
             help="maximum number of jobs to parse at once",
         )
         return argparser
 
-    def handle(
-        self, engine_config, *args, num_parse=1000, **kwargs
-    ):
+    def handle(self, engine_config, *args, num_parse=1000, **kwargs):
         self.engine = self.get_engine(engine_config)
         self.log("notice", f"Parsing from engine: {engine_config}")
         self.parse_all(num_parse)
 
     def get_engine(self, engine_config):
         engine = instantiate_from_path(engine_config, role=EngineRoles.consumer)
         engine.add_queue(Status.PARSING)
```

### Comparing `mkite_db-0.1.0/mkite_db/workflow/management/commands/parse_file.py` & `mkite_db-0.1.1/mkite_db/workflow/management/commands/parse_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 from typing import Iterable
 from django.core.management.base import BaseCommand, CommandError
 
 from mkite_core.models import JobResults
-from mkite.workflow.parse import JobParser
+from mkite_db.workflow.parse import JobParser
 from mkite_engines import Status, EngineRoles, instantiate_from_path
 
-from mkite.orm.jobs.models import Job
+from mkite_db.orm.jobs.models import Job
 
 
 class Command(BaseCommand):
     help = "Parses the job results from a folder into the database"
 
     def log(self, style, msg):
         style_fn = getattr(self.style, style.upper())
```

### Comparing `mkite_db-0.1.0/mkite_db/workflow/management/commands/submit.py` & `mkite_db-0.1.1/mkite_db/workflow/management/commands/submit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from django.db import models
 from django.core.exceptions import ObjectDoesNotExist
 from django.core.management.base import BaseCommand, CommandError
 
 from mkite_engines import Status, EngineRoles, instantiate_from_path
-from mkite.orm.jobs.models import Job, JobStatus, JobRecipe, Experiment, Project
+from mkite_db.orm.jobs.models import Job, JobStatus, JobRecipe, Experiment, Project
 
 
 class Command(BaseCommand):
     help = "Submits jobs using a given engine"
 
     def log(self, style, msg):
         style_fn = getattr(self.style, style.upper())
```

### Comparing `mkite_db-0.1.0/mkite_db/workflow/management/commands/tests/test_create_from_file.py` & `mkite_db-0.1.1/mkite_db/workflow/management/commands/tests/test_create_from_file.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 import unittest as ut
 from io import StringIO
 from model_bakery import baker
 from pkg_resources import resource_filename
 from django.test import TestCase
 from django.core.management import call_command
 
-from mkite.orm.structs.models import Crystal
-from mkite.orm.jobs.models import Job, JobStatus, JobRecipe, Experiment
+from mkite_db.orm.structs.models import Crystal
+from mkite_db.orm.jobs.models import Job, JobStatus, JobRecipe, Experiment
 
 
-RULES_FILE = resource_filename("mkite.tests.files.workflow", "create_rules.yaml")
+RULES_FILE = resource_filename("mkite_db.tests.files.workflow", "create_rules.yaml")
 
 
 class TestCommand(TestCase):
     @classmethod
     def setUpClass(cls):
         super(TestCommand, cls).setUpClass()
```

### Comparing `mkite_db-0.1.0/mkite_db/workflow/management/commands/tests/test_create_simple.py` & `mkite_db-0.1.1/mkite_db/workflow/management/commands/tests/test_create_simple.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 import unittest as ut
 from io import StringIO
 from model_bakery import baker
 from django.test import TestCase
 from django.core.management import call_command
 
-from mkite.orm.structs.models import Crystal
-from mkite.orm.jobs.models import Job, JobStatus, JobRecipe, Experiment
+from mkite_db.orm.structs.models import Crystal
+from mkite_db.orm.jobs.models import Job, JobStatus, JobRecipe, Experiment
 
 
 class TestCommand(TestCase):
     @classmethod
     def setUpClass(cls):
         super(TestCommand, cls).setUpClass()
         cls.inp_recipe = baker.make(JobRecipe)
```

### Comparing `mkite_db-0.1.0/mkite_db/workflow/management/commands/tests/test_dbimport.py` & `mkite_db-0.1.1/mkite_db/workflow/management/commands/tests/test_dbimport.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 from io import StringIO
 from model_bakery import baker
 from django.test import TestCase, SimpleTestCase
 from django.core.management import call_command
 
 from pkg_resources import resource_filename
 
-from mkite.orm.jobs.models import Job, Experiment, Project
+from mkite_db.orm.jobs.models import Job, Experiment, Project
 from mkite_core.models import JobResults
 from mkite_core.tests.tempdirs import run_in_tempdir
-from mkite.workflow.management.commands.dbimport import Command, DB_IMPORTERS
+from mkite_db.workflow.management.commands.dbimport import Command, DB_IMPORTERS
 
-from mkite.dbimport.tests.test_mp import MockMPImporter
+from mkite_db.dbimport.tests.test_mp import MockMPImporter
 
 
-JOB_RESULTS_FILE = resource_filename("mkite.tests.files.workflow", "jobresults.json")
-MP_QUERY_FILE = resource_filename("mkite.tests.files.dbimport", "mp_query.json")
+JOB_RESULTS_FILE = resource_filename("mkite_db.tests.files.workflow", "jobresults.json")
+MP_QUERY_FILE = resource_filename("mkite_db.tests.files.dbimport", "mp_query.json")
 
 MOCK_DB_IMPORTERS = {
     "MockMPImporter": MockMPImporter,
 }
 
 
 class QueryMixin:
@@ -112,15 +112,15 @@
 
         self.assertTrue(out is not None)
         self.assertIsInstance(out.job, Job)
         self.assertTrue(hasattr(out.job, "id"))
 
     @ut.skipIf("MP_API_KEY" not in os.environ, "MP_API_KEY is not in environment")
     @patch.dict(
-        "mkite.workflow.management.commands.dbimport.DB_IMPORTERS", MOCK_DB_IMPORTERS
+        "mkite_db.workflow.management.commands.dbimport.DB_IMPORTERS", MOCK_DB_IMPORTERS
     )
     def test_call(self):
         self.call_command(
             "MockMPImporter",
             "--project",
             "test_dbimport",
             "--experiment",
```

### Comparing `mkite_db-0.1.0/mkite_db/workflow/management/commands/tests/test_parse.py` & `mkite_db-0.1.1/mkite_db/workflow/management/commands/tests/test_parse.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import os
 import shutil
 from io import StringIO
 from django.test import TestCase
 from django.core.management import call_command
 from pkg_resources import resource_filename
 
-from mkite.orm.jobs.models import Job
+from mkite_db.orm.jobs.models import Job
 from mkite_core.models import JobResults
 from mkite_core.external import load_config
 from mkite_core.tests.tempdirs import run_in_tempdir
 from mkite_engines import Status
-from mkite.workflow.management.commands.parse import Command
+from mkite_db.workflow.management.commands.parse import Command
 
 
-ENGINE = resource_filename("mkite.tests.files", "engine.yaml")
+ENGINE = resource_filename("mkite_db.tests.files", "engine.yaml")
 ENGINE_CFG = load_config(ENGINE)
-JOB_RESULTS_FILE = resource_filename("mkite.tests.files.workflow", "jobresults.json")
+JOB_RESULTS_FILE = resource_filename("mkite_db.tests.files.workflow", "jobresults.json")
 
 
 def _prepare_folder():
     path = os.path.join(ENGINE_CFG["root_path"], Status.PARSING.value)
     os.mkdir(path)
     shutil.copy(JOB_RESULTS_FILE, path)
     return path
```

### Comparing `mkite_db-0.1.0/mkite_db/workflow/management/commands/tests/test_parse_file.py` & `mkite_db-0.1.1/mkite_db/workflow/management/commands/tests/test_parse_file.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import os
 import shutil
 from io import StringIO
 from django.test import TestCase
 from django.core.management import call_command
 from pkg_resources import resource_filename
 
-from mkite.orm.jobs.models import Job
+from mkite_db.orm.jobs.models import Job
 from mkite_core.models import JobResults
 from mkite_core.external import load_config
 from mkite_core.tests.tempdirs import run_in_tempdir
 from mkite_engines import Status
-from mkite.workflow.management.commands.parse import Command
+from mkite_db.workflow.management.commands.parse import Command
 
 
-ENGINE = resource_filename("mkite.tests.files", "engine.yaml")
+ENGINE = resource_filename("mkite_db.tests.files", "engine.yaml")
 ENGINE_CFG = load_config(ENGINE)
-JOB_RESULTS_FILE = resource_filename("mkite.tests.files.workflow", "jobresults.json")
+JOB_RESULTS_FILE = resource_filename("mkite_db.tests.files.workflow", "jobresults.json")
 
 
 def _prepare_folder():
     path = os.path.join(ENGINE_CFG["root_path"], Status.PARSING.value)
     os.mkdir(path)
     shutil.copy(JOB_RESULTS_FILE, path)
     return path
```

### Comparing `mkite_db-0.1.0/mkite_db/workflow/management/commands/tests/test_submit.py` & `mkite_db-0.1.1/mkite_db/workflow/management/commands/tests/test_submit.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 from io import StringIO
 from model_bakery import baker
 from django.test import TestCase
 from django.db import models
 from django.core.management import call_command
 from pkg_resources import resource_filename
 
-from mkite.orm.jobs.models import Job, JobStatus, JobRecipe, Experiment, Project
+from mkite_db.orm.jobs.models import Job, JobStatus, JobRecipe, Experiment, Project
 from mkite_core.tests.tempdirs import run_in_tempdir
-from mkite.workflow.management.commands.submit import Command, CommandError
+from mkite_db.workflow.management.commands.submit import Command, CommandError
 
 from mkite_core.tests.tempdirs import run_in_tempdir
 from mkite_engines import LocalProducer
 
 
-ENGINE = resource_filename("mkite.tests.files", "engine.yaml")
+ENGINE = resource_filename("mkite_db.tests.files", "engine.yaml")
 
 
 class TestCommand(TestCase):
     def setUp(self):
         self.cmd = Command(stdout=StringIO(), stderr=StringIO())
         self.cmd.recipe = "test_recipe"
         self.cmd.project = "test_project"
```

### Comparing `mkite_db-0.1.0/mkite_db/workflow/parse.py` & `mkite_db-0.1.1/mkite_db/workflow/parse.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Union
 from collections import namedtuple
 from django.db import transaction
 
 from mkite_core.models import JobResults
-from mkite.orm.deserializers import get_serializer, DeserializeError
-from mkite.orm.jobs.serializers import JobSerializer, RunStatsSerializer
+from mkite_db.orm.deserializers import get_serializer, DeserializeError
+from mkite_db.orm.jobs.serializers import JobSerializer, RunStatsSerializer
 
 
 ParserOutput = namedtuple("ParserOutput", "job runstats nodes")
 NodesOutput = namedtuple("NodesOutput", "chemnode calcnodes")
 
 
 class JobParser:
```

### Comparing `mkite_db-0.1.0/mkite_db/workflow/tests/test_parse.py` & `mkite_db-0.1.1/mkite_db/workflow/tests/test_parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import unittest as ut
 from model_bakery import baker
 from django.test import TestCase
 from pkg_resources import resource_filename
 
 from collections import namedtuple
 from mkite_core.models import JobResults
-from mkite.orm.jobs.models import Job, JobStatus, RunStats
-from mkite.orm.structs.models import Crystal
-from mkite.orm.calcs.models import EnergyForces
+from mkite_db.orm.jobs.models import Job, JobStatus, RunStats
+from mkite_db.orm.structs.models import Crystal
+from mkite_db.orm.calcs.models import EnergyForces
 
-from mkite.workflow.parse import JobParser
+from mkite_db.workflow.parse import JobParser
 
 
-RESULTS_FILE = resource_filename("mkite.tests.files.workflow", "jobresults.json")
+RESULTS_FILE = resource_filename("mkite_db.tests.files.workflow", "jobresults.json")
 
 
 class TestParser(TestCase):
     def setUp(self):
         self.results = JobResults.from_json(RESULTS_FILE)
         self.parser = JobParser(self.results)
```

### Comparing `mkite_db-0.1.0/mkite_db.egg-info/PKG-INFO` & `mkite_db-0.1.1/mkite_db.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkite-db
-Version: 0.1.0
+Version: 0.1.1
 Summary: mkite: distributed computing platform for high-throughput materials simulations
 Author-email: Daniel Schwalbe-Koda <dskoda@llnl.gov>
 Keywords: workflow,materials-science
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
```

### Comparing `mkite_db-0.1.0/mkite_db.egg-info/SOURCES.txt` & `mkite_db-0.1.1/mkite_db.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkite_db-0.1.0/pyproject.toml` & `mkite_db-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mkite_db"
-version = "0.1.0"
+version = "0.1.1"
 description = "mkite: distributed computing platform for high-throughput materials simulations"
 authors = [{name = "Daniel Schwalbe-Koda", email = "dskoda@llnl.gov"}]
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["workflow", "materials-science"]
 dependencies = [
     "Django >= 4.2",
@@ -27,11 +27,11 @@
     "pymatgen",
     "mp_api",
     "mkite_core",
     "mkite_engines",
 ]
 
 [project.scripts]
-kitedb = "mkite.cli.run_manage:main"
+kitedb = "mkite_db.cli.run_manage:main"
 
 [tool.setuptools]
 packages = ["mkite_db"]
```

