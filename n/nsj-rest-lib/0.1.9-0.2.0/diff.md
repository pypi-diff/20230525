# Comparing `tmp/nsj_rest_lib-0.1.9.tar.gz` & `tmp/nsj_rest_lib-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsj_rest_lib-0.1.9.tar", last modified: Wed Feb 15 09:59:06 2023, max compression
+gzip compressed data, was "nsj_rest_lib-0.2.0.tar", last modified: Thu May 25 14:19:51 2023, max compression
```

## Comparing `nsj_rest_lib-0.1.9.tar` & `nsj_rest_lib-0.2.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-02-15 09:59:06.373179 nsj_rest_lib-0.1.9/
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      743 2023-02-15 09:59:06.373179 nsj_rest_lib-0.1.9/PKG-INFO
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      130 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.9/README.md
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      103 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.9/pyproject.toml
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      888 2023-02-15 09:59:06.381179 nsj_rest_lib-0.1.9/setup.cfg
-drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-02-15 09:59:06.197179 nsj_rest_lib-0.1.9/src/
-drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-02-15 09:59:06.229179 nsj_rest_lib-0.1.9/src/nsj_rest_lib/
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)        0 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/__init__.py
-drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-02-15 09:59:06.289179 nsj_rest_lib-0.1.9/src/nsj_rest_lib/controller/
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)        0 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/controller/__init__.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)       75 2023-02-01 14:48:00.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/controller/controller_util.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     3985 2023-02-01 14:48:00.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/controller/delete_route.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      944 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/controller/funtion_route_wrapper.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     4555 2023-02-01 14:48:00.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/controller/get_route.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     5359 2023-02-01 14:48:00.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/controller/list_route.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     4886 2023-02-01 14:48:00.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/controller/post_route.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     5199 2023-02-01 14:48:00.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/controller/put_route.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     4921 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/controller/route_base.py
-drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-02-15 09:59:06.301179 nsj_rest_lib-0.1.9/src/nsj_rest_lib/dao/
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)        0 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/dao/__init__.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)    17853 2023-02-01 14:48:00.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/dao/dao_base.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     1223 2023-02-01 14:48:00.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/db_pool_config.py
-drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-02-15 09:59:06.313179 nsj_rest_lib-0.1.9/src/nsj_rest_lib/decorator/
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)        0 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/decorator/__init__.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     3987 2023-02-01 14:54:52.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/decorator/dto.py
-drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-02-15 09:59:06.337179 nsj_rest_lib-0.1.9/src/nsj_rest_lib/descriptor/
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)        0 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/descriptor/__init__.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     8871 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/descriptor/dto_field.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     7563 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/descriptor/dto_field_validators.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     5408 2023-02-01 14:48:00.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/descriptor/dto_list_field.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      195 2023-02-01 14:48:00.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/descriptor/filter_operator.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     2295 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/doc_route_generator.py
-drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-02-15 09:59:06.349179 nsj_rest_lib-0.1.9/src/nsj_rest_lib/dto/
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)        0 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/dto/__init__.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     7218 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/dto/dto_base.py
-drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-02-15 09:59:06.357179 nsj_rest_lib-0.1.9/src/nsj_rest_lib/entity/
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)        0 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/entity/__init__.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      544 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/entity/entity_base.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      322 2023-02-01 14:48:00.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/entity/filter.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      483 2022-12-09 11:46:59.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/exception.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     2856 2023-02-01 14:48:00.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/healthcheck_config.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      825 2023-02-01 14:48:00.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/injector_factory_base.py
-drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-02-15 09:59:06.369179 nsj_rest_lib-0.1.9/src/nsj_rest_lib/service/
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)        0 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/service/__init__.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)    22894 2023-02-15 09:54:51.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/service/service_base.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      580 2023-02-01 14:48:00.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/settings.py
-drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-02-15 09:59:06.373179 nsj_rest_lib-0.1.9/src/nsj_rest_lib/validator/
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)        0 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/validator/__init__.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     4196 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/validator/cpf_cnpj.py
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      527 2022-10-27 12:09:42.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib/validator/validate_data.py
-drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-02-15 09:59:06.253179 nsj_rest_lib-0.1.9/src/nsj_rest_lib.egg-info/
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      743 2023-02-15 09:59:06.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib.egg-info/PKG-INFO
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     1609 2023-02-15 09:59:06.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)        1 2023-02-15 09:59:06.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      113 2023-02-15 09:59:06.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib.egg-info/requires.txt
--rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)       13 2023-02-15 09:59:06.000000 nsj_rest_lib-0.1.9/src/nsj_rest_lib.egg-info/top_level.txt
+drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-05-25 14:19:50.988175 nsj_rest_lib-0.2.0/
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      743 2023-05-25 14:19:50.992175 nsj_rest_lib-0.2.0/PKG-INFO
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      130 2022-10-27 12:09:42.000000 nsj_rest_lib-0.2.0/README.md
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      103 2022-10-27 12:09:42.000000 nsj_rest_lib-0.2.0/pyproject.toml
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      888 2023-05-25 14:19:50.992175 nsj_rest_lib-0.2.0/setup.cfg
+drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-05-25 14:19:50.852174 nsj_rest_lib-0.2.0/src/
+drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-05-25 14:19:50.888174 nsj_rest_lib-0.2.0/src/nsj_rest_lib/
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)        0 2022-10-27 12:09:42.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/__init__.py
+drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-05-25 14:19:50.940175 nsj_rest_lib-0.2.0/src/nsj_rest_lib/controller/
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)        0 2022-10-27 12:09:42.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/controller/__init__.py
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)       75 2023-02-01 14:48:00.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/controller/controller_util.py
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     3131 2023-05-25 14:14:05.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/controller/delete_route.py
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      944 2022-10-27 12:09:42.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/controller/funtion_route_wrapper.py
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     3700 2023-05-25 14:14:05.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/controller/get_route.py
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     4349 2023-05-25 14:14:05.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/controller/list_route.py
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     3742 2023-05-25 14:14:05.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/controller/post_route.py
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     4152 2023-05-25 14:14:05.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/controller/put_route.py
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     4664 2023-05-25 14:14:05.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/controller/route_base.py
+drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-05-25 14:19:50.944175 nsj_rest_lib-0.2.0/src/nsj_rest_lib/dao/
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)        0 2022-10-27 12:09:42.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/dao/__init__.py
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)    16639 2023-05-25 14:14:05.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/dao/dao_base.py
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     1223 2023-02-01 14:48:00.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/db_pool_config.py
+drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-05-25 14:19:50.944175 nsj_rest_lib-0.2.0/src/nsj_rest_lib/decorator/
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)        0 2022-10-27 12:09:42.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/decorator/__init__.py
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     3987 2023-02-01 14:54:52.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/decorator/dto.py
+drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-05-25 14:19:50.968175 nsj_rest_lib-0.2.0/src/nsj_rest_lib/descriptor/
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)        0 2022-10-27 12:09:42.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/descriptor/__init__.py
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     8870 2023-03-30 14:16:13.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/descriptor/dto_field.py
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     7563 2022-10-27 12:09:42.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/descriptor/dto_field_validators.py
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     5408 2023-02-01 14:48:00.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/descriptor/dto_list_field.py
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      195 2023-02-01 14:48:00.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/descriptor/filter_operator.py
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     2295 2022-10-27 12:09:42.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/doc_route_generator.py
+drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-05-25 14:19:50.968175 nsj_rest_lib-0.2.0/src/nsj_rest_lib/dto/
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)        0 2022-10-27 12:09:42.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/dto/__init__.py
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     7290 2023-04-17 15:08:09.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/dto/dto_base.py
+drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-05-25 14:19:50.976175 nsj_rest_lib-0.2.0/src/nsj_rest_lib/entity/
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)        0 2022-10-27 12:09:42.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/entity/__init__.py
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      772 2023-04-17 15:08:09.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/entity/entity_base.py
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      322 2023-02-01 14:48:00.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/entity/filter.py
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      483 2022-12-09 11:46:59.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/exception.py
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     2856 2023-02-01 14:48:00.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/healthcheck_config.py
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      825 2023-02-01 14:48:00.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/injector_factory_base.py
+drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-05-25 14:19:50.976175 nsj_rest_lib-0.2.0/src/nsj_rest_lib/service/
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)        0 2022-10-27 12:09:42.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/service/__init__.py
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)    23200 2023-05-25 14:14:05.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/service/service_base.py
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      582 2023-03-30 14:16:13.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/settings.py
+drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-05-25 14:19:50.988175 nsj_rest_lib-0.2.0/src/nsj_rest_lib/validator/
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)        0 2022-10-27 12:09:42.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/validator/__init__.py
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     4196 2022-10-27 12:09:42.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/validator/cpf_cnpj.py
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      527 2022-10-27 12:09:42.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib/validator/validate_data.py
+drwxrwxr-x   0 wallacepinho  (1000) wallacepinho  (1000)        0 2023-05-25 14:19:50.904174 nsj_rest_lib-0.2.0/src/nsj_rest_lib.egg-info/
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      743 2023-05-25 14:19:50.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)     1609 2023-05-25 14:19:50.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)        1 2023-05-25 14:19:50.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)      113 2023-05-25 14:19:50.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib.egg-info/requires.txt
+-rw-rw-r--   0 wallacepinho  (1000) wallacepinho  (1000)       13 2023-05-25 14:19:50.000000 nsj_rest_lib-0.2.0/src/nsj_rest_lib.egg-info/top_level.txt
```

### Comparing `nsj_rest_lib-0.1.9/PKG-INFO` & `nsj_rest_lib-0.2.0/src/nsj_rest_lib.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: nsj_rest_lib
-Version: 0.1.9
+Name: nsj-rest-lib
+Version: 0.2.0
 Summary: Biblioteca para construção de APIs Rest Python, de acordo com o guidelines interno, e com paradigma declarativo.
 Home-page: https://github.com/Nasajon/nsj_rest_lib
 Author: Nasajon Sistemas
 Author-email: contact.dev@nasajon.com.br
 Project-URL: Source, https://github.com/Nasajon/nsj_rest_lib
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `nsj_rest_lib-0.1.9/setup.cfg` & `nsj_rest_lib-0.2.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nsj_rest_lib
-version = 0.1.9
+version = 0.2.0
 author = Nasajon Sistemas
 author_email = contact.dev@nasajon.com.br
 description = Biblioteca para construção de APIs Rest Python, de acordo com o guidelines interno, e com paradigma declarativo.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Nasajon/nsj_rest_lib
 project_urls =
```

### Comparing `nsj_rest_lib-0.1.9/src/nsj_rest_lib/controller/delete_route.py` & `nsj_rest_lib-0.2.0/src/nsj_rest_lib/controller/get_route.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,85 +9,81 @@
 from nsj_rest_lib.injector_factory_base import NsjInjectorFactoryBase
 
 from nsj_gcf_utils.json_util import json_dumps
 from nsj_gcf_utils.pagination_util import PaginationException
 from nsj_gcf_utils.rest_error_util import format_json_error
 
 
-class DeleteRoute(RouteBase):
+class GetRoute(RouteBase):
     def __init__(
         self,
         url: str,
         http_method: str,
         dto_class: DTOBase,
         entity_class: EntityBase,
         injector_factory: NsjInjectorFactoryBase = NsjInjectorFactoryBase,
         service_name: str = None,
         handle_exception: Callable = None,
-        require_tenant: bool = True,
-        require_grupo_emprearial: bool = True
     ):
         super().__init__(
             url=url,
             http_method=http_method,
             dto_class=dto_class,
             entity_class=entity_class,
             dto_response_class=None,
             injector_factory=injector_factory,
             service_name=service_name,
-            handle_exception=handle_exception,
-            require_tenant=require_tenant,
-            require_grupo_emprearial=require_grupo_emprearial,
+            handle_exception=handle_exception
         )
 
     def handle_request(self, id):
         """
-        Tratando requisições HTTP Delete para excluir uma instância de uma entidade.
+        Tratando requisições HTTP Get para recuperar uma instância de uma entidade.
         """
 
         with self._injector_factory() as factory:
             try:
                 # Recuperando os parâmetros básicos
                 args = request.args
 
-                # Tratando do tenant e do grupo_empresarial
-                # TODO Refatorar para exibir os dois erros ao mesmo tempo
-                tenant = args.get('tenant')
-                grupo_empresarial = args.get('grupo_empresarial')
-
-                if self._require_tenant:
-                    if tenant is None:
-                        raise MissingParameterException('tenant')
-
-                    if not ('tenant' in self._dto_class.fields_map):
-                        raise DTOConfigException(
-                            f"Missing 'tenant' field declaration on DTOClass: {self._dto_class}")
-
-                if self._require_grupo_emprearial:
-                    if grupo_empresarial is None:
-                        raise MissingParameterException('grupo_empresarial')
-
-                    if not ('grupo_empresarial' in self._dto_class.fields_map):
-                        raise DTOConfigException(
-                            f"Missing 'grupo_empresarial' field declaration on DTOClass: {self._dto_class}")
+                # Tratando dos fields
+                fields = args.get('fields')
+                fields = self._parse_fields(fields)
+
+                partition_fields = {}
+                # Tratando campos de particionamento
+                for field in self._dto_class.partition_fields:
+                    value = args.get(field)
+                    if value is None:
+                        raise MissingParameterException(field)
+                    
+                    partition_fields[field] = value
 
                 # Construindo os objetos
                 service = self._get_service(factory)
 
                 # Chamando o service (método get)
                 # TODO Rever parametro order_fields abaixo
-                service.delete(id, grupo_empresarial, tenant)
+                data = service.get(id, partition_fields, fields)
+
+                # Convertendo para o formato de dicionário (permitindo omitir campos do DTO)
+                dict_data = data.convert_to_dict(fields)
 
                 # Retornando a resposta da requuisição
-                return ('', 204, {**DEFAULT_RESP_HEADERS})
+                return (json_dumps(dict_data), 200, {**DEFAULT_RESP_HEADERS})
             except MissingParameterException as e:
                 if self._handle_exception is not None:
                     return self._handle_exception(e)
                 else:
                     return (format_json_error(e), 400, {**DEFAULT_RESP_HEADERS})
+            except PaginationException as e:
+                if self._handle_exception is not None:
+                    return self._handle_exception(e)
+                else:
+                    return (format_json_error(e), 400, {**DEFAULT_RESP_HEADERS})
             except NotFoundException as e:
                 if self._handle_exception is not None:
                     return self._handle_exception(e)
                 else:
                     return (format_json_error(e), 404, {**DEFAULT_RESP_HEADERS})
             except Exception as e:
                 if self._handle_exception is not None:
```

### Comparing `nsj_rest_lib-0.1.9/src/nsj_rest_lib/controller/funtion_route_wrapper.py` & `nsj_rest_lib-0.2.0/src/nsj_rest_lib/controller/funtion_route_wrapper.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.1.9/src/nsj_rest_lib/controller/get_route.py` & `nsj_rest_lib-0.2.0/src/nsj_rest_lib/controller/list_route.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,108 +1,109 @@
 from flask import request
 from typing import Callable
 
 from nsj_rest_lib.controller.controller_util import DEFAULT_RESP_HEADERS
 from nsj_rest_lib.controller.route_base import RouteBase
 from nsj_rest_lib.dto.dto_base import DTOBase
 from nsj_rest_lib.entity.entity_base import EntityBase
-from nsj_rest_lib.exception import DTOConfigException, MissingParameterException, NotFoundException
+from nsj_rest_lib.exception import DTOConfigException, MissingParameterException
 from nsj_rest_lib.injector_factory_base import NsjInjectorFactoryBase
+from nsj_rest_lib.settings import DEFAULT_PAGE_SIZE
 
 from nsj_gcf_utils.json_util import json_dumps
-from nsj_gcf_utils.pagination_util import PaginationException
+from nsj_gcf_utils.pagination_util import page_body, PaginationException
 from nsj_gcf_utils.rest_error_util import format_json_error
 
 
-class GetRoute(RouteBase):
+class ListRoute(RouteBase):
     def __init__(
         self,
         url: str,
         http_method: str,
         dto_class: DTOBase,
         entity_class: EntityBase,
         injector_factory: NsjInjectorFactoryBase = NsjInjectorFactoryBase,
         service_name: str = None,
         handle_exception: Callable = None,
-        require_tenant: bool = True,
-        require_grupo_emprearial: bool = True
     ):
         super().__init__(
             url=url,
             http_method=http_method,
             dto_class=dto_class,
             entity_class=entity_class,
             dto_response_class=None,
             injector_factory=injector_factory,
             service_name=service_name,
             handle_exception=handle_exception,
-            require_tenant=require_tenant,
-            require_grupo_emprearial=require_grupo_emprearial,
         )
 
-    def handle_request(self, id):
+    def handle_request(self):
         """
-        Tratando requisições HTTP Get para recuperar uma instância de uma entidade.
+        Tratando requisições HTTP Get (para listar entidades, e não para recuperar pelo ID).
         """
 
         with self._injector_factory() as factory:
             try:
                 # Recuperando os parâmetros básicos
+                base_url = request.base_url
                 args = request.args
+                limit = int(args.get('limit', DEFAULT_PAGE_SIZE))
+                current_after = args.get('after') or args.get('offset')
 
                 # Tratando dos fields
                 fields = args.get('fields')
                 fields = self._parse_fields(fields)
 
-                # Tratando do tenant e do grupo_empresarial
-                # TODO Refatorar para exibir os dois erros ao mesmo tempo
-                tenant = args.get('tenant')
-                grupo_empresarial = args.get('grupo_empresarial')
-
-                if self._require_tenant:
-                    if tenant is None:
-                        raise MissingParameterException('tenant')
-
-                    if not ('tenant' in self._dto_class.fields_map):
-                        raise DTOConfigException(
-                            f"Missing 'tenant' field declaration on DTOClass: {self._dto_class}")
-
-                if self._require_grupo_emprearial:
-                    if grupo_empresarial is None:
-                        raise MissingParameterException('grupo_empresarial')
-
-                    if not ('grupo_empresarial' in self._dto_class.fields_map):
-                        raise DTOConfigException(
-                            f"Missing 'grupo_empresarial' field declaration on DTOClass: {self._dto_class}")
+                # Tratando dos filters
+                filters = {}
+                for arg in args:
+                    if arg in ['limit', 'after', 'offset', 'fields', 'tenant', 'grupo_empresarial']:
+                        continue
+
+                    filters[arg] = args.get(arg)
+
+                # Tratando campos de particionamento
+                for field in self._dto_class.partition_fields:
+                    value = args.get(field)
+                    if value is None:
+                        raise MissingParameterException(field)
+                    
+                    filters[field] = value
 
                 # Construindo os objetos
                 service = self._get_service(factory)
 
-                # Chamando o service (método get)
+                # Chamando o service (método list)
                 # TODO Rever parametro order_fields abaixo
-                data = service.get(id, grupo_empresarial, tenant, fields)
+                data = service.list(current_after, limit,
+                                    fields, None, filters)
 
                 # Convertendo para o formato de dicionário (permitindo omitir campos do DTO)
-                dict_data = data.convert_to_dict(fields)
+                dict_data = [dto.convert_to_dict(fields) for dto in data]
+
+                # Construindo o corpo da página
+                page = page_body(
+                    base_url=base_url,
+                    limit=limit,
+                    current_after=current_after,
+                    current_before=None,
+                    result=dict_data,
+                    id_field='id'  # TODO Rever esse parâmetro
+                )
 
                 # Retornando a resposta da requuisição
-                return (json_dumps(dict_data), 200, {**DEFAULT_RESP_HEADERS})
+                return (json_dumps(page), 200, {**DEFAULT_RESP_HEADERS})
             except MissingParameterException as e:
                 if self._handle_exception is not None:
                     return self._handle_exception(e)
                 else:
                     return (format_json_error(e), 400, {**DEFAULT_RESP_HEADERS})
             except PaginationException as e:
                 if self._handle_exception is not None:
                     return self._handle_exception(e)
                 else:
                     return (format_json_error(e), 400, {**DEFAULT_RESP_HEADERS})
-            except NotFoundException as e:
-                if self._handle_exception is not None:
-                    return self._handle_exception(e)
-                else:
-                    return (format_json_error(e), 404, {**DEFAULT_RESP_HEADERS})
             except Exception as e:
                 if self._handle_exception is not None:
                     return self._handle_exception(e)
                 else:
                     return (format_json_error(f'Erro desconhecido: {e}'), 500, {**DEFAULT_RESP_HEADERS})
```

### Comparing `nsj_rest_lib-0.1.9/src/nsj_rest_lib/controller/post_route.py` & `nsj_rest_lib-0.2.0/src/nsj_rest_lib/controller/post_route.py`

 * *Files 19% similar despite different names*

```diff
@@ -19,61 +19,37 @@
         http_method: str,
         dto_class: DTOBase,
         entity_class: EntityBase,
         dto_response_class: DTOBase = None,
         injector_factory: NsjInjectorFactoryBase = NsjInjectorFactoryBase,
         service_name: str = None,
         handle_exception: Callable = None,
-        require_tenant: bool = True,
-        require_grupo_emprearial: bool = True
     ):
         super().__init__(
             url=url,
             http_method=http_method,
             dto_class=dto_class,
             entity_class=entity_class,
             dto_response_class=dto_response_class,
             injector_factory=injector_factory,
             service_name=service_name,
             handle_exception=handle_exception,
-            require_tenant=require_tenant,
-            require_grupo_emprearial=require_grupo_emprearial,
         )
 
     def handle_request(self):
         """
         Tratando requisições HTTP Post para inserir uma instância de uma entidade.
         """
 
         with self._injector_factory() as factory:
             try:
                 # Recuperando os dados do corpo da rquisição
                 data = request.get_data(as_text=True)
                 data = json_loads(data)
 
-                # Tratando do tenant e do grupo_empresarial
-                tenant = data.get('tenant')
-                grupo_empresarial = data.get('grupo_empresarial')
-
-                if self._require_tenant:
-                    if tenant is None:
-                        raise MissingParameterException('tenant')
-
-                    if not ('tenant' in self._dto_class.fields_map):
-                        raise DTOConfigException(
-                            f"Missing 'tenant' field declaration on DTOClass: {self._dto_class}")
-
-                if self._require_grupo_emprearial:
-                    if grupo_empresarial is None:
-                        raise MissingParameterException('grupo_empresarial')
-
-                    if not ('grupo_empresarial' in self._dto_class.fields_map):
-                        raise DTOConfigException(
-                            f"Missing 'grupo_empresarial' field declaration on DTOClass: {self._dto_class}")
-
                 # Convertendo os dados para o DTO
                 data = self._dto_class(**data)
 
                 # Construindo os objetos
                 service = self._get_service(factory)
 
                 # Chamando o service (método insert)
```

### Comparing `nsj_rest_lib-0.1.9/src/nsj_rest_lib/controller/route_base.py` & `nsj_rest_lib-0.2.0/src/nsj_rest_lib/controller/route_base.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,44 +18,38 @@
 
     _injector_factory: NsjInjectorFactoryBase
     _service_name: str
     _handle_exception: Callable
     _dto_class: DTOBase
     _entity_class: EntityBase
     _dto_response_class: DTOBase
-    _require_tenant: bool
-    _require_grupo_emprearial: bool
 
     def __init__(
         self,
         url: str,
         http_method: str,
         dto_class: DTOBase,
         entity_class: EntityBase,
         dto_response_class: DTOBase = None,
         injector_factory: NsjInjectorFactoryBase = NsjInjectorFactoryBase,
         service_name: str = None,
         handle_exception: Callable = None,
-        require_tenant: bool = True,
-        require_grupo_emprearial: bool = True
     ):
         super().__init__()
 
         self.url = url
         self.http_method = http_method
         self.__class__.registered_routes.append(self)
 
         self._injector_factory = injector_factory
         self._service_name = service_name
         self._handle_exception = handle_exception
         self._dto_class = dto_class
         self._entity_class = entity_class
         self._dto_response_class = dto_response_class
-        self._require_tenant = require_tenant
-        self._require_grupo_emprearial = require_grupo_emprearial
 
     def __call__(self, func):
         self.function_wrapper = FunctionRouteWrapper(self, func)
         return self.function_wrapper
 
     def _get_service(self, factory: NsjInjectorFactoryBase) -> ServiceBase:
         """
```

### Comparing `nsj_rest_lib-0.1.9/src/nsj_rest_lib/dao/dao_base.py` & `nsj_rest_lib-0.2.0/src/nsj_rest_lib/dao/dao_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         # Building SQL fields
         if fields is None:
             fields = [f"t0.{k}" for k in entity.__dict__ if not callable(
                 getattr(entity, k, None)) and not k.startswith('_')]
 
         return ', '.join(fields)
 
-    def get(self, id: uuid.UUID, fields: List[str] = None, grupo_empresarial=None, tenant=None) -> EntityBase:
+    def get(self, id: uuid.UUID, fields: List[str] = None, partition_fields=None) -> EntityBase:
         """
         Returns an entity instance by its ID.
         """
 
         # Creating a entity instance
         entity = self._entity_class()
 
@@ -83,31 +83,26 @@
         select
             {self._sql_fields(fields)}
         from
             {entity.get_table_name()} as t0
         where
             t0.{entity.get_pk_column_name()} = :id
         """
+        values = {"id": id}
 
-        # TODO Refatorar para suportar outros nomes para as colunas grupo_empresarial e tenant
-        if grupo_empresarial is not None:
-            sql += "\n"
-            sql += "    and t0.grupo_empresarial = :grupo_empresarial"
-
-        if tenant is not None:
-            sql += "\n"
-            sql += "    and t0.tenant = :tenant"
-
+        if partition_fields is not None:
+            for field in partition_fields:
+                sql += f" \n and t0.{field} = :{field}"
+                values[field] = partition_fields[field]
+                
         # Running query
         resp = self._db.execute_query_to_model(
             sql,
             self._entity_class,
-            id=id,
-            grupo_empresarial=grupo_empresarial,
-            tenant=tenant
+            **values
         )
 
         # Checking if ID was found
         if len(resp) <= 0:
             raise NotFoundException(
                 f'{self._entity_class.__name__} com id {id} não encontrado.')
 
@@ -364,18 +359,18 @@
         """
         Retorna lista com os campos para update, no padrão "field = :field"
         """
 
         # Building SQL fields
         if ignore_nones:
             fields = [f"{k} = :{k}" for k in entity.__dict__ if not callable(
-                getattr(entity, k, None)) and not k.startswith('_') and getattr(entity, k) is not None]
+                getattr(entity, k, None)) and not k.startswith('_') and getattr(entity, k) is not None and k not in entity.get_const_fields()]
         else:
             fields = [f"{k} = :{k}" for k in entity.__dict__ if not callable(
-                getattr(entity, k, None)) and not k.startswith('_')]
+                getattr(entity, k, None)) and not k.startswith('_') and k not in entity.get_const_fields()]
 
         return ', '.join(fields)
 
     def update(
         self,
         entity: EntityBase,
         filters: Dict[str, List[Filter]],
@@ -436,15 +431,15 @@
         rowcount, returning = self._db.execute(
             sql,
             **kwargs
         )
 
         if rowcount <= 0:
             raise NotFoundException(
-                f'{self._entity_class.__name__} com id {values_map[pk_field]} não encontrado.')
+                f'{self._entity_class.__name__} com id {values_map[self._entity_class().get_pk_field()]} não encontrado.')
 
         # Complementando o objeto com os dados de retorno
         if returning_fields is not None and USE_SQL_RETURNING_CLAUSE:
             for field in returning_fields:
                 setattr(entity, field, returning[0][field])
 
         return entity
@@ -517,48 +512,7 @@
             **filter_values_map
         )
 
         # Verificando se houve alguma deleção
         if rowcount <= 0:
             raise NotFoundException(
                 f'{self._entity_class.__name__} não encontrado. Filtros: {filters}')
-
-    def delete(self, id: uuid.UUID, grupo_empresarial=None, tenant=None):
-        """
-        Returns an entity instance by its ID.
-        """
-
-        # Creating a entity instance
-        entity = self._entity_class()
-
-        # Building query
-        sql = f"""
-        delete
-        from
-            {entity.get_table_name()} as t0
-        where
-            t0.{entity.get_pk_column_name()} = :id
-        """
-
-        # TODO Refatorar para suportar outros nomes para as colunas grupo_empresarial e tenant
-        if grupo_empresarial is not None:
-            sql += "\n"
-            sql += "    and t0.grupo_empresarial = :grupo_empresarial"
-
-        if tenant is not None:
-            sql += "\n"
-            sql += "    and t0.tenant = :tenant"
-
-        # Running query
-        resp = self._db.execute(
-            sql,
-            id=id,
-            grupo_empresarial=grupo_empresarial,
-            tenant=tenant
-        )
-
-        # Checking if ID was found
-        if len(resp) <= 0:
-            raise NotFoundException(
-                f'{self._entity_class.__name__} com id {id} não encontrado.')
-
-        return resp[0]
```

### Comparing `nsj_rest_lib-0.1.9/src/nsj_rest_lib/db_pool_config.py` & `nsj_rest_lib-0.2.0/src/nsj_rest_lib/db_pool_config.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.1.9/src/nsj_rest_lib/decorator/dto.py` & `nsj_rest_lib-0.2.0/src/nsj_rest_lib/decorator/dto.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.1.9/src/nsj_rest_lib/descriptor/dto_field.py` & `nsj_rest_lib-0.2.0/src/nsj_rest_lib/descriptor/dto_field.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,15 +176,15 @@
                 value = self.expected_type(value)
             except ValueError as e:
                 raise ValueError(
                     f"{self.storage_name} não é um {self.expected_type.__name__} válido. Valor recebido: {value}.")
         elif self.expected_type is bool and isinstance(value, int):
             # Booleanos
             # Converting int to bool (0 is False, otherwise is True)
-            value = (value == 0)
+            value = bool(value)
         elif self.expected_type is datetime.datetime and isinstance(value, datetime.date):
             # Datetime
             # Assumindo hora 0, minuto 0 e segundo 0 (quanto é recebida uma data para campo data + hora)
             value = datetime.datetime(
                 value.year, value.month, value.day, 0, 0, 0)
         elif self.expected_type is datetime.date and isinstance(value, datetime.datetime):
             # Date
```

### Comparing `nsj_rest_lib-0.1.9/src/nsj_rest_lib/descriptor/dto_field_validators.py` & `nsj_rest_lib-0.2.0/src/nsj_rest_lib/descriptor/dto_field_validators.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.1.9/src/nsj_rest_lib/descriptor/dto_list_field.py` & `nsj_rest_lib-0.2.0/src/nsj_rest_lib/descriptor/dto_list_field.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.1.9/src/nsj_rest_lib/doc_route_generator.py` & `nsj_rest_lib-0.2.0/src/nsj_rest_lib/doc_route_generator.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.1.9/src/nsj_rest_lib/dto/dto_base.py` & `nsj_rest_lib-0.2.0/src/nsj_rest_lib/dto/dto_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import abc
 import copy
 # import uuid
 
-from typing import Any, Dict, List, Set
+from typing import Any, Dict, List, Set, Union
 
 from nsj_rest_lib.entity.entity_base import EMPTY, EntityBase
 from nsj_rest_lib.descriptor.dto_field import DTOField, DTOFieldFilter
 
 
 class DTOBase(abc.ABC):
     resume_fields: Set[str] = set()
@@ -14,20 +14,20 @@
     fields_map: Dict[str, DTOField] = {}
     list_fields_map: dict = {}
     field_filters_map: Dict[str, DTOFieldFilter]
     # TODO Refatorar para suportar PK composto
     pk_field: str
     fixed_filters: Dict[str, Any]
 
-    def __init__(self, entity: EntityBase = None, **kwargs) -> None:
+    def __init__(self, entity: Union[EntityBase, dict] = None, **kwargs) -> None:
         super().__init__()
 
         # Transformando a entity em dict (se houver uma entity)
         if entity is not None:
-            kwargs = copy.deepcopy(entity.__dict__)
+            kwargs =  copy.deepcopy(entity) if type(entity) is dict else copy.deepcopy(entity.__dict__)
 
         # Setando os campos registrados como fields simples
         for field in self.__class__.fields_map:
             # Recuperando a configuração do campo
             dto_field = self.__class__.fields_map[field]
 
             # Tratando do valor default
```

### Comparing `nsj_rest_lib-0.1.9/src/nsj_rest_lib/healthcheck_config.py` & `nsj_rest_lib-0.2.0/src/nsj_rest_lib/healthcheck_config.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.1.9/src/nsj_rest_lib/injector_factory_base.py` & `nsj_rest_lib-0.2.0/src/nsj_rest_lib/injector_factory_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.1.9/src/nsj_rest_lib/service/service_base.py` & `nsj_rest_lib-0.2.0/src/nsj_rest_lib/service/service_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,26 +36,25 @@
         self._dto_post_response_class = dto_post_response_class
         self._created_by_property = 'criado_por'
         self._updated_by_property = 'atualizado_por'
 
     def get(
         self,
         id: str,
-        grupo_empresarial: str,
-        tenant: str,
+        partition_fields: Dict[str, Any],
         fields: Dict[str, List[str]]
     ) -> DTOBase:
         # Resolving fields
         fields = self._resolving_fields(fields)
 
         # Handling the fields to retrieve
         entity_fields = self._convert_to_entity_fields(fields['root'])
 
         # Recuperando a entity
-        entity = self._dao.get(id, entity_fields, grupo_empresarial, tenant)
+        entity = self._dao.get(id, entity_fields, partition_fields)
 
         # Convertendo para DTO
         dto = self._dto_class(entity)
 
         # Tratando das propriedades de lista
         if len(self._dto_class.list_fields_map) > 0:
             self._retrieve_related_lists([dto], fields)
@@ -243,14 +242,20 @@
                 # Making filter to relation
                 filters = {
                     # TODO Adicionar os campos de particionamento de dados
                     list_field.related_entity_field: getattr(
                         dto, self._dto_class.pk_field)
                 }
 
+                # Tratando campos de particionamento
+                for field in self._dto_class.partition_fields:
+                    if field in list_field.dto_type.partition_fields:
+                        filters[field] = getattr(
+                            dto, field)
+
                 # Resolvendo os fields da entidade aninhada
                 fields_to_list = copy.deepcopy(fields)
                 if master_dto_attr in fields:
                     fields_to_list['root'] = fields[master_dto_attr]
                     del fields_to_list[master_dto_attr]
                 else:
                     fields_to_list['root'] = set()
@@ -350,15 +355,15 @@
                         value = getattr(entity, self._updated_by_property)
                         if value is None or value == '':
                             raise ValueError(
                                 f"É necessário preencher o campo '{self._updated_by_property}'")
 
             # Invocando o DAO
             if insert:
-                if self.entity_exists(entity):
+                if self.entity_exists(entity, aditional_filters):
                     raise ConflictException(
                         f"Já existe um registro no banco com o identificador '{getattr(entity, entity_pk_field)}'")
                 entity = self._dao.insert(entity)
             else:
                 # Montando os filtros
                 id_condiction = Filter(
                     FilterOperator.EQUALS,
@@ -459,14 +464,22 @@
                     pk_value
                 )
 
                 relation_filter = {
                     list_field.related_entity_field: [relation_condiction]
                 }
 
+                # Tratando campos de particionamento
+                for field in self._dto_class.partition_fields:
+                    if field in list_field.dto_type.partition_fields:
+                        relation_filter[field] = [Filter(
+                            FilterOperator.EQUALS,
+                            getattr(dto, field)
+                        )]
+
                 # Recuperando do BD
                 old_detail_ids = detail_dao.list_ids(relation_filter)
             
             # Lista de DTOs detalhes a criar ou atualizar
             detail_upsert_list = []
 
             # Salvando cada DTO detalhe
@@ -501,15 +514,15 @@
                 })
 
             # Verificando se sobraram relacionamentos anteriores para remover
             if not partial_update and old_detail_ids is not None and len(old_detail_ids) > 0:
 
                 for old_id in old_detail_ids:
                     # Apagando cada relacionamento removido
-                    detail_service.delete(old_id, **aditional_filters)
+                    detail_service.delete(old_id, aditional_filters)
             
             # Salvando cada DTO detalhe
             for item in detail_upsert_list:
                 response_detail_dto = detail_service._save(
                     item["is_detail_insert"], item["detail_dto"], False, partial_update, relation_field_map, item["detail_pk"])
 
                 # Guardando o DTO na lista de retorno
@@ -518,99 +531,82 @@
             # Setting dto property
             if response_dto is not None and master_dto_field in response_dto.list_fields_map and list_field.dto_post_response_type is not None:
                 setattr(response_dto, master_dto_field, response_list)
 
     def delete(
         self,
         id: Any,
-        aditional_filters: Dict[str, Any] = None
+        additional_filters: Dict[str, Any] = None
     ) -> DTOBase:
+        self._delete(id,manage_transaction=True,additional_filters=additional_filters)
+        
 
-        # Convertendo os filtros para os filtros de entidade
-        entity_filters = {}
-        if aditional_filters is not None:
-            entity_filters = self._create_entity_filters(aditional_filters)
-
-        # Adicionando o ID nos filtros
-        id_condiction = Filter(
-            FilterOperator.EQUALS,
-            id
-        )
-
-        pk_field = self._entity_class().get_pk_field()
-        entity_filters[pk_field] = [id_condiction]
-
-        # Chamando o DAO para a exclusão
-        self._dao.delete(entity_filters)
-
-    def entity_exists(self, entity: EntityBase):
+    def entity_exists(self, entity: EntityBase, partition_fields: Dict[str, Any]):
         # Getting values
         entity_pk_field = entity.get_pk_field()
         entity_pk_value = getattr(entity, entity_pk_field)
-        grupo_empresarial = getattr(entity, 'grupo_empresarial', None)
-        tenant = getattr(entity, 'tenant', None)
+        
 
         if entity_pk_value is None:
             return False
 
         # Searching entity in DB
         try:
             self._dao.get(entity_pk_value, [entity.get_pk_column_name(
-            )], grupo_empresarial=grupo_empresarial, tenant=tenant)
+            )], partition_fields)
         except NotFoundException as e:
             return False
 
         return True
 
-    def delete(
-        self,
-        id: str,
-        grupo_empresarial: str,
-        tenant: str
-    ) -> DTOBase:
-
-        self._delete(
-            id,
-            grupo_empresarial,
-            tenant,
-            manage_transaction=True
-        )
-
     def _delete(
         self,
         id: str,
-        grupo_empresarial: str,
-        tenant: str,
-        manage_transaction: bool
+        manage_transaction: bool,
+        additional_filters: Dict[str, Any] = None
     ) -> DTOBase:
 
         try:
             if manage_transaction:
                 self._dao.begin()
 
+            # Convertendo os filtros para os filtros de entidade
+            entity_filters = {}
+            if additional_filters is not None:
+                entity_filters = self._create_entity_filters(additional_filters)
+
+            # Adicionando o ID nos filtros
+            id_condiction = Filter(
+                FilterOperator.EQUALS,
+                id
+            )
+
+            pk_field = self._entity_class().get_pk_field()
+            entity_filters[pk_field] = [id_condiction]
+
+            
             # Tratando das propriedades de lista
             if len(self._dto_class.list_fields_map) > 0:
-                self._delete_related_lists(id, grupo_empresarial, tenant)
+                self._delete_related_lists(id, additional_filters)
 
             # Excluindo a entity principal
-            self._dao.delete(id, grupo_empresarial, tenant)
+            self._dao.delete(entity_filters)
 
         except:
             if manage_transaction:
                 self._dao.rollback()
             raise
         finally:
             if manage_transaction:
                 self._dao.commit()
 
     def _delete_related_lists(
         self,
         id,
-        grupo_empresarial: str,
-        tenant: str
+        additional_filters: Dict[str, Any] = None
     ):
 
         # Handling each related list
         for _, list_field in self._dto_class.list_fields_map.items():
 
             # Getting service instance
             # TODO Refatorar para suportar services customizados
@@ -645,9 +641,8 @@
                         f"PK field not found in DTO: {self._dto_class}")
 
                 # Recuperando o ID da entidade detalhe
                 related_id = getattr(
                     related_dto, list_field.dto_type.pk_field)
 
                 # Chamando a exclusão recursivamente
-                service._delete(related_id, grupo_empresarial,
-                                tenant, manage_transaction=False)
+                service._delete(related_id, manage_transaction=False, additional_filters=additional_filters)
```

### Comparing `nsj_rest_lib-0.1.9/src/nsj_rest_lib/settings.py` & `nsj_rest_lib-0.2.0/src/nsj_rest_lib/settings.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 
 # Lendo variáveis de ambiente
 DEFAULT_PAGE_SIZE = int(os.getenv('DEFAULT_PAGE_SIZE', 20))
 USE_SQL_RETURNING_CLAUSE = (
-    os.getenv('USE_SQL_RETURNING_CLAUSE', 'true').lower == 'true')
+    os.getenv('USE_SQL_RETURNING_CLAUSE', 'true').lower() == 'true')
 
 DATABASE_HOST = os.getenv('DATABASE_HOST', '')
 DATABASE_PASS = os.getenv('DATABASE_PASS', '')
 DATABASE_PORT = os.getenv('DATABASE_PORT', '')
 DATABASE_NAME = os.getenv('DATABASE_NAME', '')
 DATABASE_USER = os.getenv('DATABASE_USER', '')
 DATABASE_DRIVER = os.getenv('DATABASE_DRIVER', 'POSTGRES')
```

### Comparing `nsj_rest_lib-0.1.9/src/nsj_rest_lib/validator/cpf_cnpj.py` & `nsj_rest_lib-0.2.0/src/nsj_rest_lib/validator/cpf_cnpj.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.1.9/src/nsj_rest_lib/validator/validate_data.py` & `nsj_rest_lib-0.2.0/src/nsj_rest_lib/validator/validate_data.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-0.1.9/src/nsj_rest_lib.egg-info/PKG-INFO` & `nsj_rest_lib-0.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: nsj-rest-lib
-Version: 0.1.9
+Name: nsj_rest_lib
+Version: 0.2.0
 Summary: Biblioteca para construção de APIs Rest Python, de acordo com o guidelines interno, e com paradigma declarativo.
 Home-page: https://github.com/Nasajon/nsj_rest_lib
 Author: Nasajon Sistemas
 Author-email: contact.dev@nasajon.com.br
 Project-URL: Source, https://github.com/Nasajon/nsj_rest_lib
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `nsj_rest_lib-0.1.9/src/nsj_rest_lib.egg-info/SOURCES.txt` & `nsj_rest_lib-0.2.0/src/nsj_rest_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

