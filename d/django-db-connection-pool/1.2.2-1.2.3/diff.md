# Comparing `tmp/django-db-connection-pool-1.2.2.tar.gz` & `tmp/django-db-connection-pool-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\django-db-connection-pool-1.2.2.tar", last modified: Wed Nov  2 02:05:57 2022, max compression
+gzip compressed data, was "django-db-connection-pool-1.2.3.tar", last modified: Thu May 25 08:06:07 2023, max compression
```

## Comparing `django-db-connection-pool-1.2.2.tar` & `django-db-connection-pool-1.2.3.tar`

### file list

```diff
@@ -1,48 +1,68 @@
-drwxrwxrwx   0        0        0        0 2022-11-02 02:05:57.000000 django-db-connection-pool-1.2.2/
-drwxrwxrwx   0        0        0        0 2022-11-02 02:05:57.000000 django-db-connection-pool-1.2.2/django_db_connection_pool.egg-info/
--rw-rw-rw-   0        0        0        1 2022-11-02 02:05:57.000000 django-db-connection-pool-1.2.2/django_db_connection_pool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     5781 2022-11-02 02:05:57.000000 django-db-connection-pool-1.2.2/django_db_connection_pool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2022-11-02 02:05:57.000000 django-db-connection-pool-1.2.2/django_db_connection_pool.egg-info/requires.txt
--rw-rw-rw-   0        0        0     1243 2022-11-02 02:05:57.000000 django-db-connection-pool-1.2.2/django_db_connection_pool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       16 2022-11-02 02:05:57.000000 django-db-connection-pool-1.2.2/django_db_connection_pool.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-11-02 02:05:57.000000 django-db-connection-pool-1.2.2/dj_db_conn_pool/
-drwxrwxrwx   0        0        0        0 2022-11-02 02:05:57.000000 django-db-connection-pool-1.2.2/dj_db_conn_pool/backends/
-drwxrwxrwx   0        0        0        0 2022-11-02 02:05:57.000000 django-db-connection-pool-1.2.2/dj_db_conn_pool/backends/jdbc/
-drwxrwxrwx   0        0        0        0 2022-11-02 02:05:57.000000 django-db-connection-pool-1.2.2/dj_db_conn_pool/backends/jdbc/oceanbase/
--rw-rw-rw-   0        0        0     1632 2022-11-02 02:04:52.000000 django-db-connection-pool-1.2.2/dj_db_conn_pool/backends/jdbc/oceanbase/base.py
--rw-rw-rw-   0        0        0        0 2022-03-28 02:57:23.000000 django-db-connection-pool-1.2.2/dj_db_conn_pool/backends/jdbc/oceanbase/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-02 02:05:57.000000 django-db-connection-pool-1.2.2/dj_db_conn_pool/backends/jdbc/oracle/
--rw-rw-rw-   0        0        0     1224 2022-07-01 02:17:41.000000 django-db-connection-pool-1.2.2/dj_db_conn_pool/backends/jdbc/oracle/base.py
--rw-rw-rw-   0        0        0        0 2021-08-20 08:50:55.000000 django-db-connection-pool-1.2.2/dj_db_conn_pool/backends/jdbc/oracle/__init__.py
--rw-rw-rw-   0        0        0     1163 2022-07-01 03:47:20.000000 django-db-connection-pool-1.2.2/dj_db_conn_pool/backends/jdbc/utils.py
--rw-rw-rw-   0        0        0     1962 2022-07-01 03:02:44.000000 django-db-connection-pool-1.2.2/dj_db_conn_pool/backends/jdbc/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-02 02:05:57.000000 django-db-connection-pool-1.2.2/dj_db_conn_pool/backends/mysql/
--rw-rw-rw-   0        0        0      501 2022-07-01 02:46:15.000000 django-db-connection-pool-1.2.2/dj_db_conn_pool/backends/mysql/base.py
--rw-rw-rw-   0        0        0        0 2021-08-20 08:50:55.000000 django-db-connection-pool-1.2.2/dj_db_conn_pool/backends/mysql/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-02 02:05:57.000000 django-db-connection-pool-1.2.2/dj_db_conn_pool/backends/oracle/
--rw-rw-rw-   0        0        0      325 2022-07-01 02:54:21.000000 django-db-connection-pool-1.2.2/dj_db_conn_pool/backends/oracle/base.py
--rw-rw-rw-   0        0        0        0 2021-08-20 08:50:55.000000 django-db-connection-pool-1.2.2/dj_db_conn_pool/backends/oracle/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-02 02:05:57.000000 django-db-connection-pool-1.2.2/dj_db_conn_pool/backends/postgresql/
--rw-rw-rw-   0        0        0      230 2022-07-01 08:01:28.000000 django-db-connection-pool-1.2.2/dj_db_conn_pool/backends/postgresql/base.py
-drwxrwxrwx   0        0        0        0 2022-11-02 02:05:57.000000 django-db-connection-pool-1.2.2/dj_db_conn_pool/backends/postgresql/django_tenants/
--rw-rw-rw-   0        0        0      312 2022-07-01 08:05:12.000000 django-db-connection-pool-1.2.2/dj_db_conn_pool/backends/postgresql/django_tenants/base.py
--rw-rw-rw-   0        0        0        0 2021-08-20 08:50:55.000000 django-db-connection-pool-1.2.2/dj_db_conn_pool/backends/postgresql/django_tenants/__init__.py
--rw-rw-rw-   0        0        0      294 2022-07-01 08:01:28.000000 django-db-connection-pool-1.2.2/dj_db_conn_pool/backends/postgresql/mixins.py
--rw-rw-rw-   0        0        0        0 2021-08-20 08:50:55.000000 django-db-connection-pool-1.2.2/dj_db_conn_pool/backends/postgresql/__init__.py
--rw-rw-rw-   0        0        0        0 2021-08-20 08:50:55.000000 django-db-connection-pool-1.2.2/dj_db_conn_pool/backends/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-02 02:05:57.000000 django-db-connection-pool-1.2.2/dj_db_conn_pool/compat/
--rw-rw-rw-   0        0        0      703 2022-05-26 01:09:52.000000 django-db-connection-pool-1.2.2/dj_db_conn_pool/compat/jdbc.py
--rw-rw-rw-   0        0        0      302 2022-01-12 07:58:01.000000 django-db-connection-pool-1.2.2/dj_db_conn_pool/compat/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-02 02:05:57.000000 django-db-connection-pool-1.2.2/dj_db_conn_pool/core/
--rw-rw-rw-   0        0        0       70 2021-08-20 08:50:55.000000 django-db-connection-pool-1.2.2/dj_db_conn_pool/core/exceptions.py
--rw-rw-rw-   0        0        0     4691 2022-10-10 01:27:03.000000 django-db-connection-pool-1.2.2/dj_db_conn_pool/core/mixins.py
--rw-rw-rw-   0        0        0      988 2022-05-26 01:02:07.000000 django-db-connection-pool-1.2.2/dj_db_conn_pool/core/__init__.py
--rw-rw-rw-   0        0        0      391 2022-11-02 02:01:02.000000 django-db-connection-pool-1.2.2/dj_db_conn_pool/__init__.py
--rw-rw-rw-   0        0        0     1067 2021-08-20 08:50:55.000000 django-db-connection-pool-1.2.2/LICENSE
--rw-rw-rw-   0        0        0       80 2021-08-20 08:50:55.000000 django-db-connection-pool-1.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0     5781 2022-11-02 02:05:57.000000 django-db-connection-pool-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     4618 2022-03-29 02:30:42.000000 django-db-connection-pool-1.2.2/README.md
--rw-rw-rw-   0        0        0     7109 2022-09-29 08:00:35.000000 django-db-connection-pool-1.2.2/README_cn.md
--rw-rw-rw-   0        0        0       97 2021-11-23 03:19:46.000000 django-db-connection-pool-1.2.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2022-11-02 02:05:57.000000 django-db-connection-pool-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0     2093 2022-07-01 02:23:22.000000 django-db-connection-pool-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 08:06:07.156866 django-db-connection-pool-1.2.3/
+-rw-rw-rw-   0        0        0     1067 2021-08-20 08:50:55.000000 django-db-connection-pool-1.2.3/LICENSE
+-rw-rw-rw-   0        0        0       80 2021-08-20 08:50:55.000000 django-db-connection-pool-1.2.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     6082 2023-05-25 08:06:07.156866 django-db-connection-pool-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4913 2023-04-20 13:56:04.000000 django-db-connection-pool-1.2.3/README.md
+-rw-rw-rw-   0        0        0     6665 2023-04-20 13:56:04.000000 django-db-connection-pool-1.2.3/README_cn.md
+drwxrwxrwx   0        0        0        0 2023-05-25 08:06:07.131354 django-db-connection-pool-1.2.3/dj_db_conn_pool/
+-rw-rw-rw-   0        0        0      391 2023-04-21 08:48:04.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 08:06:07.132354 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/
+-rw-rw-rw-   0        0        0        0 2021-08-20 08:50:55.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 08:06:07.132354 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/jdbc/
+-rw-rw-rw-   0        0        0     2096 2023-04-21 06:54:28.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/jdbc/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 08:06:07.133354 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/jdbc/oceanbase/
+-rw-rw-rw-   0        0        0        0 2022-03-28 02:57:23.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/jdbc/oceanbase/__init__.py
+-rw-rw-rw-   0        0        0      281 2022-11-10 08:02:57.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/jdbc/oceanbase/mixins.py
+drwxrwxrwx   0        0        0        0 2023-05-25 08:06:07.135353 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/jdbc/oceanbase/mysql/
+-rw-rw-rw-   0        0        0        0 2022-11-10 07:45:39.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/jdbc/oceanbase/mysql/__init__.py
+-rw-rw-rw-   0        0        0      574 2023-04-20 13:56:04.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/jdbc/oceanbase/mysql/base.py
+drwxrwxrwx   0        0        0        0 2023-05-25 08:06:07.135353 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/jdbc/oceanbase/oracle/
+-rw-rw-rw-   0        0        0        0 2022-11-10 07:45:39.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/jdbc/oceanbase/oracle/__init__.py
+-rw-rw-rw-   0        0        0      703 2023-04-20 13:56:04.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/jdbc/oceanbase/oracle/base.py
+drwxrwxrwx   0        0        0        0 2023-05-25 08:06:07.136858 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/jdbc/oracle/
+-rw-rw-rw-   0        0        0        0 2021-08-20 08:50:55.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/jdbc/oracle/__init__.py
+-rw-rw-rw-   0        0        0     1133 2023-04-21 07:24:27.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/jdbc/oracle/base.py
+drwxrwxrwx   0        0        0        0 2023-05-25 08:06:07.137864 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/mysql/
+-rw-rw-rw-   0        0        0        0 2021-08-20 08:50:55.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/mysql/__init__.py
+-rw-rw-rw-   0        0        0      516 2023-04-21 02:41:00.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/mysql/base.py
+drwxrwxrwx   0        0        0        0 2023-05-25 08:06:07.138864 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/odbc/
+-rw-rw-rw-   0        0        0        0 2022-11-10 07:54:21.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/odbc/__init__.py
+-rw-rw-rw-   0        0        0      682 2023-04-21 02:00:57.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/odbc/mixins.py
+drwxrwxrwx   0        0        0        0 2023-05-25 08:06:07.139866 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/odbc/oceanbase/
+-rw-rw-rw-   0        0        0        1 2022-11-10 07:54:21.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/odbc/oceanbase/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 08:06:07.140864 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/odbc/oceanbase/oracle/
+-rw-rw-rw-   0        0        0        0 2022-11-10 07:54:21.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/odbc/oceanbase/oracle/__init__.py
+-rw-rw-rw-   0        0        0      365 2023-04-21 02:42:53.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/odbc/oceanbase/oracle/base.py
+drwxrwxrwx   0        0        0        0 2023-05-25 08:06:07.141864 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/oracle/
+-rw-rw-rw-   0        0        0        0 2021-08-20 08:50:55.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/oracle/__init__.py
+-rw-rw-rw-   0        0        0      488 2023-04-21 06:08:53.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/oracle/base.py
+drwxrwxrwx   0        0        0        0 2023-05-25 08:06:07.143864 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/postgis/
+-rw-rw-rw-   0        0        0        0 2023-03-31 04:15:33.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/postgis/__init__.py
+-rw-rw-rw-   0        0        0      342 2023-04-21 02:41:09.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/postgis/base.py
+drwxrwxrwx   0        0        0        0 2023-05-25 08:06:07.144866 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/postgresql/
+-rw-rw-rw-   0        0        0        0 2021-08-20 08:50:55.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/postgresql/__init__.py
+-rw-rw-rw-   0        0        0      446 2023-05-25 07:53:09.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/postgresql/base.py
+drwxrwxrwx   0        0        0        0 2023-05-25 08:06:07.146864 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/postgresql/django_tenants/
+-rw-rw-rw-   0        0        0        0 2021-08-20 08:50:55.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/postgresql/django_tenants/__init__.py
+-rw-rw-rw-   0        0        0      312 2022-07-01 08:05:12.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/postgresql/django_tenants/base.py
+-rw-rw-rw-   0        0        0      302 2023-04-21 02:41:12.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/postgresql/mixins.py
+drwxrwxrwx   0        0        0        0 2023-05-25 08:06:07.147864 django-db-connection-pool-1.2.3/dj_db_conn_pool/compat/
+-rw-rw-rw-   0        0        0      302 2022-01-12 07:58:01.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/compat/__init__.py
+-rw-rw-rw-   0        0        0      947 2023-04-21 06:02:01.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/compat/jdbc.py
+drwxrwxrwx   0        0        0        0 2023-05-25 08:06:07.149871 django-db-connection-pool-1.2.3/dj_db_conn_pool/core/
+-rw-rw-rw-   0        0        0     1070 2023-04-06 08:30:16.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/core/__init__.py
+-rw-rw-rw-   0        0        0       70 2021-08-20 08:50:55.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/core/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-25 08:06:07.151867 django-db-connection-pool-1.2.3/dj_db_conn_pool/core/mixins/
+-rw-rw-rw-   0        0        0       77 2023-04-06 03:18:16.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/core/mixins/__init__.py
+-rw-rw-rw-   0        0        0     5385 2023-04-21 07:25:01.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/core/mixins/core.py
+-rw-rw-rw-   0        0        0      385 2023-04-06 07:58:20.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/core/mixins/creation.py
+-rw-rw-rw-   0        0        0     1293 2023-04-21 08:02:44.000000 django-db-connection-pool-1.2.3/dj_db_conn_pool/core/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-25 08:06:07.155867 django-db-connection-pool-1.2.3/django_db_connection_pool.egg-info/
+-rw-rw-rw-   0        0        0     6082 2023-05-25 08:06:07.000000 django-db-connection-pool-1.2.3/django_db_connection_pool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1881 2023-05-25 08:06:07.000000 django-db-connection-pool-1.2.3/django_db_connection_pool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 08:06:07.000000 django-db-connection-pool-1.2.3/django_db_connection_pool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      275 2023-05-25 08:06:07.000000 django-db-connection-pool-1.2.3/django_db_connection_pool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-25 08:06:07.000000 django-db-connection-pool-1.2.3/django_db_connection_pool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      125 2023-04-20 13:56:04.000000 django-db-connection-pool-1.2.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-25 08:06:07.157864 django-db-connection-pool-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     2255 2023-04-21 06:08:53.000000 django-db-connection-pool-1.2.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-db-connection-pool-1.2.2/django_db_connection_pool.egg-info/PKG-INFO` & `django-db-connection-pool-1.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: django-db-connection-pool
-Version: 1.2.2
+Version: 1.2.3
 Summary: Persistent database connection backends for Django
 Home-page: https://github.com/altairbow/django-db-connection-pool
+Download-URL: https://pypi.python.org/pypi/django-db-connection-pool/
 Author: Altair Bow
 Author-email: altair.bow@foxmail.com
 License: MIT
-Download-URL: https://pypi.python.org/pypi/django-db-connection-pool/
-Keywords: django,db,database,persistent,connection,pool
-Platform: UNKNOWN
+Keywords: django,db,database,persistent,connection,pool,pooling
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 Provides-Extra: all
+Provides-Extra: jdbc
 Provides-Extra: mysql
+Provides-Extra: odbc
 Provides-Extra: oracle
 Provides-Extra: postgresql
-Provides-Extra: jdbc
 License-File: LICENSE
 
 # django-db-connection-pool
 
 *:star: Leave a star if django-db-connection-pool is helpful to you, or you like it, Thank you:smile:*
 
 MySQL & Oracle & PostgreSQL & JDBC (Oracle, OceanBase) connection pool backends of Django, 
@@ -134,34 +134,33 @@
 Or, you can use dj_db_conn_pool.setup to change default arguments(for each pool's creation), before using database pool:
 
 ```python
 import dj_db_conn_pool
 dj_db_conn_pool.setup(pool_size=100, max_overflow=50)
 ```
 
+#### multiprocessing environment
+In a multiprocessing environment, such as uWSGI, each process will have its own `dj_db_conn_pool.core:pool_container` object,
+It means that each process has an independent connection pool, for example: 
+The `POOL_OPTIONS` configuration of database `db1` is`{ 'POOL_SIZE': 10, 'MAX_OVERFLOW': 20 }`,
+If uWSGI starts 8 worker processes, then the total connection pool size of `db1`  is `8 * 10`,
+The maximum number of connections will not exceed `8 * 10 + 8 * 20`
+
+
 ## JDBC (experimental, NOT PRODUCTION READY)
-Thanks to [JPype](https://github.com/jpype-project/jpype) [JayDeBeApi](https://github.com/baztian/jaydebeapi/) ,
+Thanks to [JPype](https://github.com/jpype-project/jpype),
 django-db-connection-pool can connect to database in jdbc way
 
 ### Usage
 #### Set Java runtime environment
 ```bash
 export JAVA_HOME=$PATH_TO_JRE;
 export CLASSPATH=$PATH_RO_JDBC_DRIVER_JAR
 ```
 
-#### Start JVM
-Start JVM before initialization of Django
-
-```python
-import jpype
-jvm_path = jpype.getDefaultJVMPath()
-jpype.startJVM(jvm_path)
-```
-
 #### Update settings.DATABASES
 ##### Oracle
 
 change `django.db.backends.oracle` to `dj_db_conn_pool.backends.jdbc.oracle`:
 ```python
 DATABASES = {
     'default': {
@@ -175,9 +174,7 @@
 ```python
 DATABASES = {
     'default': {
         'ENGINE': 'dj_db_conn_pool.backends.jdbc.oceanbase'
     }
 }
 ```
-
-
```

### Comparing `django-db-connection-pool-1.2.2/django_db_connection_pool.egg-info/SOURCES.txt` & `django-db-connection-pool-1.2.3/django_db_connection_pool.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -3,31 +3,44 @@
 README.md
 README_cn.md
 requirements.txt
 setup.py
 dj_db_conn_pool/__init__.py
 dj_db_conn_pool/backends/__init__.py
 dj_db_conn_pool/backends/jdbc/__init__.py
-dj_db_conn_pool/backends/jdbc/utils.py
 dj_db_conn_pool/backends/jdbc/oceanbase/__init__.py
-dj_db_conn_pool/backends/jdbc/oceanbase/base.py
+dj_db_conn_pool/backends/jdbc/oceanbase/mixins.py
+dj_db_conn_pool/backends/jdbc/oceanbase/mysql/__init__.py
+dj_db_conn_pool/backends/jdbc/oceanbase/mysql/base.py
+dj_db_conn_pool/backends/jdbc/oceanbase/oracle/__init__.py
+dj_db_conn_pool/backends/jdbc/oceanbase/oracle/base.py
 dj_db_conn_pool/backends/jdbc/oracle/__init__.py
 dj_db_conn_pool/backends/jdbc/oracle/base.py
 dj_db_conn_pool/backends/mysql/__init__.py
 dj_db_conn_pool/backends/mysql/base.py
+dj_db_conn_pool/backends/odbc/__init__.py
+dj_db_conn_pool/backends/odbc/mixins.py
+dj_db_conn_pool/backends/odbc/oceanbase/__init__.py
+dj_db_conn_pool/backends/odbc/oceanbase/oracle/__init__.py
+dj_db_conn_pool/backends/odbc/oceanbase/oracle/base.py
 dj_db_conn_pool/backends/oracle/__init__.py
 dj_db_conn_pool/backends/oracle/base.py
+dj_db_conn_pool/backends/postgis/__init__.py
+dj_db_conn_pool/backends/postgis/base.py
 dj_db_conn_pool/backends/postgresql/__init__.py
 dj_db_conn_pool/backends/postgresql/base.py
 dj_db_conn_pool/backends/postgresql/mixins.py
 dj_db_conn_pool/backends/postgresql/django_tenants/__init__.py
 dj_db_conn_pool/backends/postgresql/django_tenants/base.py
 dj_db_conn_pool/compat/__init__.py
 dj_db_conn_pool/compat/jdbc.py
 dj_db_conn_pool/core/__init__.py
 dj_db_conn_pool/core/exceptions.py
-dj_db_conn_pool/core/mixins.py
+dj_db_conn_pool/core/utils.py
+dj_db_conn_pool/core/mixins/__init__.py
+dj_db_conn_pool/core/mixins/core.py
+dj_db_conn_pool/core/mixins/creation.py
 django_db_connection_pool.egg-info/PKG-INFO
 django_db_connection_pool.egg-info/SOURCES.txt
 django_db_connection_pool.egg-info/dependency_links.txt
 django_db_connection_pool.egg-info/requires.txt
 django_db_connection_pool.egg-info/top_level.txt
```

### Comparing `django-db-connection-pool-1.2.2/dj_db_conn_pool/backends/jdbc/oracle/base.py` & `django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/jdbc/oracle/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # -*- coding: utf-8 -*-
 
 import getpass
 import socket
 from multiprocessing import current_process
-import jpype
-import jaydebeapi
+import jpype.dbapi2
 from django.db.backends.oracle import base
 from sqlalchemy.dialects.oracle.base import OracleDialect
 from dj_db_conn_pool.backends.jdbc import JDBCDatabaseWrapperMixin
 
 
 import logging
 logger = logging.getLogger(__name__)
@@ -22,22 +21,19 @@
 
 
 class DatabaseWrapper(JDBCDatabaseWrapperMixin, base.DatabaseWrapper):
     class SQLAlchemyDialect(OracleDialect):
         def do_ping(self, dbapi_connection):
             try:
                 return super(OracleDialect, self).do_ping(dbapi_connection)
-            except (jaydebeapi.DatabaseError, jpype.JException):
+            except jpype.dbapi2.DatabaseError:
                 return False
 
     jdbc_driver = 'oracle.jdbc.OracleDriver'
 
-    @property
-    def jdbc_url(self):
-        return 'jdbc:oracle:thin:@//{NAME}'.format(**self.settings_dict)
+    jdbc_url_prefix = 'jdbc:oracle:thin:@'
 
-    @property
-    def jdbc_options(self):
+    def get_connection_params(self):
         return {
             **oracle_session_info,
-            **super(DatabaseWrapper, self).jdbc_options
+            **super(DatabaseWrapper, self).get_connection_params()
         }
```

### Comparing `django-db-connection-pool-1.2.2/dj_db_conn_pool/backends/jdbc/utils.py` & `django-db-connection-pool-1.2.3/dj_db_conn_pool/core/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,46 @@
+import logging
 import sqlparams
 
-import logging
 logger = logging.getLogger(__name__)
 
-sql_params_converter = sqlparams.SQLParams('named', 'qmark')
-
 
 class CursorWrapper:
-    def __init__(self, cursor):
+    def __init__(self, cursor, style, sql_converter):
         self._cursor = cursor
 
-        self.statement = None
+        self._sql_params_converter = sqlparams.SQLParams('named', style, True, True)
+
+        self._sql_converter = sql_converter
+
+        self._statement = None
 
     def execute(self, query, parameters=None):
-        """
-        :param self: django's cursor
-        :param query: SQL
-        :param parameters: SQL parameters
-        :return:
-        """
         if isinstance(parameters, dict):
-            # convert sql and parameters
-            _query, _parameters = sql_params_converter.format(query, parameters)
+            _query, _parameters = self._sql_params_converter.format(query, parameters)
+        else:
+            _query, _parameters = self._sql_converter(query), parameters
 
+        if query != _query:
             logger.debug(
                 'SQL (%s), parameters(%s) has been converted to SQL(%s), parameters(%s)',
-                query, parameters, _query, _parameters)
-
-            query, parameters = (_query, _parameters)
-        else:
-            # change paramstyle 'format' to 'qmark'
-            query = query.replace('%s', '?')
-
-        # record last query
-        self.statement = query
+                query, parameters, _query, _parameters
+            )
 
-        # call jaydebeapi
-        self._cursor.cursor.execute(query, parameters)
+        query, parameters = _query, _parameters
 
-    def __getattr__(self, item):
-        return getattr(self._cursor, item)
+        try:
+            cursor = self._cursor.cursor
+        except AttributeError:
+            cursor = self._cursor
+
+        self._statement = query
+
+        return cursor.execute(query, parameters or [])
+
+    def __getattr__(self, attr):
+        try:
+            return getattr(self._cursor, attr)
+        except AttributeError:
+            if attr == 'statement':
+                return self._statement
+            raise
```

### Comparing `django-db-connection-pool-1.2.2/dj_db_conn_pool/backends/jdbc/__init__.py` & `django-db-connection-pool-1.2.3/dj_db_conn_pool/backends/jdbc/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,64 +1,69 @@
 # -*- coding: utf-8 -*-
 
-import jaydebeapi
-from dj_db_conn_pool.core.mixins import PooledDatabaseWrapperMixin
-from dj_db_conn_pool.backends.jdbc.utils import CursorWrapper
+import threading
+import jpype
+import jpype.dbapi2
+from dj_db_conn_pool.core.mixins import PersistentDatabaseWrapperMixin
 
 import logging
 logger = logging.getLogger(__name__)
 
+jdbc_type_converters = {}
 
-class JDBCDatabaseWrapperMixin(PooledDatabaseWrapperMixin):
-    def _set_dbapi_autocommit(self, autocommit):
-        self.connection.connection.jconn.setAutoCommit(autocommit)
+lock_check_jvm_status = threading.Lock()
+
+
+class JDBCDatabaseWrapperMixin(PersistentDatabaseWrapperMixin):
+    _sql_param_style = 'qmark'
+
+    _sql_converter = staticmethod(lambda sql: sql.replace('%s', '?'))
 
     @property
     def jdbc_driver(self):
         raise NotImplementedError()
 
     @property
-    def jdbc_url(self):
+    def jdbc_url_prefix(self):
         raise NotImplementedError()
 
     @property
-    def jdbc_options(self):
-        return self.settings_dict.get('JDBC_OPTIONS', {})
+    def jdbc_url(self):
+        return '{prefix}//{HOST}:{PORT}/{NAME}'.format(
+            prefix=self.jdbc_url_prefix,
+            **self.settings_dict
+        )
+
+    def get_connection_params(self):
+        return self.settings_dict.get('OPTIONS', {})
 
     def _get_new_connection(self, conn_params):
-        conn = jaydebeapi.connect(
-            self.jdbc_driver,
+        with lock_check_jvm_status:
+            if not jpype.isJVMStarted():
+                jpype.startJVM(ignoreUnrecognized=True)
+
+        conn = jpype.dbapi2.connect(
             self.jdbc_url,
-            {
-                'user': self.settings_dict['USER'],
-                'password': self.settings_dict['PASSWORD'],
-                **self.jdbc_options
-            }
+            driver=self.jdbc_driver,
+            driver_args=dict(
+                user=self.settings_dict['USER'],
+                password=self.settings_dict['PASSWORD'],
+                **conn_params
+            ),
+            converters=jdbc_type_converters,
         )
 
         return conn
 
-    def create_cursor(self, name=None):
-        """
-        create a cursor
-        do some tricks here
-        :param name:
-        :return:
-        """
-        # get cursor from django
-        cursor = super().create_cursor(name)
-
-        return CursorWrapper(cursor)
-
     def _close(self):
-        if self.connection is not None and self.connection.connection.jconn.getAutoCommit():
+        if self.connection is not None and self.connection.driver_connection.autocommit:
             # if jdbc connection's autoCommit is on
-            # jaydebeapi will throw an exception after rollback called
+            # jpype will throw NotSupportedError after rollback called
             # we make a little dynamic patch here, make sure
             # SQLAlchemy will not do rollback before recycling connection
             self.connection._pool._reset_on_return = None
 
             logger.debug(
                 "autoCommit of current JDBC connection to %s %s is on, won't do rollback before returning",
-                self.alias, self.connection.connection)
+                self.alias, self.connection.driver_connection)
 
         return super(JDBCDatabaseWrapperMixin, self)._close()
```

### Comparing `django-db-connection-pool-1.2.2/dj_db_conn_pool/core/mixins.py` & `django-db-connection-pool-1.2.3/dj_db_conn_pool/core/mixins/core.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,64 @@
 # -*- coding: utf-8 -*-
 
 from sqlalchemy import pool
 from dj_db_conn_pool.compat import gettext_lazy as _
 from dj_db_conn_pool.core import pool_container
+from dj_db_conn_pool.core.utils import CursorWrapper
+from dj_db_conn_pool.core.mixins.creation import DatabaseCreationMixin
 
 
 import logging
 logger = logging.getLogger(__name__)
 
 
-class PooledDatabaseWrapperMixin(object):
+class PersistentDatabaseWrapperMixin(object):
+    def __init__(self, *args, **kwargs):
+        # override creation_class
+        self.creation_class = type('', (DatabaseCreationMixin, self.creation_class), {})
+
+        super(PersistentDatabaseWrapperMixin, self).__init__(*args, **kwargs)
+
     def __str__(self):
         try:
-            conn = repr(self.connection.connection)
+            conn = repr(self.connection.driver_connection)
         except AttributeError:
             conn = '<Not connected>'
 
         return f'{self.vendor} connection to {self.alias}: {conn}'
 
     __repr__ = __str__
 
     def _set_dbapi_autocommit(self, autocommit):
-        self.connection.connection.autocommit = autocommit
+        self.connection.driver_connection.autocommit = autocommit
 
     def _set_autocommit(self, autocommit):
         with self.wrap_database_errors:
             try:
                 self._set_dbapi_autocommit(autocommit)
             except (Exception, ) as exc:
                 logger.exception('unable to set autocommit mode of %s(%s) to %s, caused by: %s',
                                  self.vendor, self.alias, autocommit, exc)
                 raise exc from None
 
     def _get_dialect(self):
         return self.SQLAlchemyDialect(dbapi=self.Database)
 
+    _sql_param_style = 'format'
+
+    _sql_converter = staticmethod(lambda sql: sql)
+
+    def create_cursor(self, name=None):
+        # get cursor from django
+        cursor = super().create_cursor(name)
+
+        return CursorWrapper(cursor, self._sql_param_style, self._sql_converter)
+
     def _get_new_connection(self, conn_params):
-        return super(PooledDatabaseWrapperMixin, self).get_new_connection(conn_params)
+        return super(PersistentDatabaseWrapperMixin, self).get_new_connection(conn_params)
 
     def get_new_connection(self, conn_params):
         """
         override django.db.backends.<database>.base.DatabaseWrapper.get_new_connection to
         change the default behavior of getting new connection to database, we maintain
         pool_container who contains the connection pool of each database here
         when django call this method to get new connection, we check whether there exists
@@ -97,17 +115,17 @@
         # get self.alias's pool from pool_container
         db_pool = pool_container.get(self.alias)
         # get one connection from the pool
         conn = db_pool.connect()
 
         logger.debug(
             _("got %s's connection %s from its pool"),
-            self.alias, conn.connection)
+            self.alias, conn.driver_connection)
 
         return conn
 
     def close(self, *args, **kwargs):
         logger.debug(
             _("release %s's connection %s to its pool"),
-            self.alias, getattr(self.connection, 'connection', None))
+            self.alias, getattr(self.connection, 'driver_connection', None))
 
-        return super(PooledDatabaseWrapperMixin, self).close(*args, **kwargs)
+        return super(PersistentDatabaseWrapperMixin, self).close(*args, **kwargs)
```

### Comparing `django-db-connection-pool-1.2.2/dj_db_conn_pool/core/__init__.py` & `django-db-connection-pool-1.2.3/dj_db_conn_pool/core/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,42 @@
-# -*- coding: utf-8 -*-
-
-import threading
-from dj_db_conn_pool.compat import gettext_lazy as _
-from dj_db_conn_pool.core.exceptions import PoolDoesNotExist
-
-
-class PoolContainer(dict):
-    # acquire this lock before modify pool_container
-    lock = threading.Lock()
-
-    # the default parameters of pool
-    pool_default_params = {
-        'pre_ping': True,
-        'echo': False,
-        'timeout': 30,
-        'recycle': 60 * 15,
-        'pool_size': 10,
-        'max_overflow': 10,
-    }
-
-    def has(self, pool_name):
-        return pool_name in self
-
-    def put(self, pool_name, pool):
-        self[pool_name] = pool
-
-    def get(self, pool_name):
-        try:
-            return self[pool_name]
-        except KeyError:
-            raise PoolDoesNotExist(_('No such pool: {pool_name}').format(pool_name=pool_name))
-
-
-# the pool's container, for maintaining the pools
-# every process has it's own pool container
-pool_container = PoolContainer()
+# -*- coding: utf-8 -*-
+
+import threading
+from dj_db_conn_pool.compat import gettext_lazy as _
+from dj_db_conn_pool.core.exceptions import PoolDoesNotExist
+
+
+class PoolContainer(dict):
+    # acquire this lock before modify pool_container
+    lock = threading.Lock()
+
+    # the default parameters of pool
+    pool_default_params = {
+        'pre_ping': True,
+        'echo': False,
+        'timeout': 30,
+        'recycle': 60 * 15,
+        'pool_size': 10,
+        'max_overflow': 10,
+    }
+
+    def has(self, pool_name):
+        return pool_name in self
+
+    def put(self, pool_name, pool):
+        self[pool_name] = pool
+
+    def get(self, pool_name):
+        try:
+            return self[pool_name]
+        except KeyError:
+            raise PoolDoesNotExist(_('No such pool: {pool_name}').format(pool_name=pool_name))
+
+    def dispose(self):
+        # dispose all pools
+        for name, pool in self.items():
+            pool.dispose()
+
+
+# the pool's container, for maintaining the pools
+# every process has it's own pool container
+pool_container = PoolContainer()
```

### Comparing `django-db-connection-pool-1.2.2/LICENSE` & `django-db-connection-pool-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-db-connection-pool-1.2.2/PKG-INFO` & `django-db-connection-pool-1.2.3/django_db_connection_pool.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: django-db-connection-pool
-Version: 1.2.2
+Version: 1.2.3
 Summary: Persistent database connection backends for Django
 Home-page: https://github.com/altairbow/django-db-connection-pool
+Download-URL: https://pypi.python.org/pypi/django-db-connection-pool/
 Author: Altair Bow
 Author-email: altair.bow@foxmail.com
 License: MIT
-Download-URL: https://pypi.python.org/pypi/django-db-connection-pool/
-Keywords: django,db,database,persistent,connection,pool
-Platform: UNKNOWN
+Keywords: django,db,database,persistent,connection,pool,pooling
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 Provides-Extra: all
+Provides-Extra: jdbc
 Provides-Extra: mysql
+Provides-Extra: odbc
 Provides-Extra: oracle
 Provides-Extra: postgresql
-Provides-Extra: jdbc
 License-File: LICENSE
 
 # django-db-connection-pool
 
 *:star: Leave a star if django-db-connection-pool is helpful to you, or you like it, Thank you:smile:*
 
 MySQL & Oracle & PostgreSQL & JDBC (Oracle, OceanBase) connection pool backends of Django, 
@@ -134,34 +134,33 @@
 Or, you can use dj_db_conn_pool.setup to change default arguments(for each pool's creation), before using database pool:
 
 ```python
 import dj_db_conn_pool
 dj_db_conn_pool.setup(pool_size=100, max_overflow=50)
 ```
 
+#### multiprocessing environment
+In a multiprocessing environment, such as uWSGI, each process will have its own `dj_db_conn_pool.core:pool_container` object,
+It means that each process has an independent connection pool, for example: 
+The `POOL_OPTIONS` configuration of database `db1` is`{ 'POOL_SIZE': 10, 'MAX_OVERFLOW': 20 }`,
+If uWSGI starts 8 worker processes, then the total connection pool size of `db1`  is `8 * 10`,
+The maximum number of connections will not exceed `8 * 10 + 8 * 20`
+
+
 ## JDBC (experimental, NOT PRODUCTION READY)
-Thanks to [JPype](https://github.com/jpype-project/jpype) [JayDeBeApi](https://github.com/baztian/jaydebeapi/) ,
+Thanks to [JPype](https://github.com/jpype-project/jpype),
 django-db-connection-pool can connect to database in jdbc way
 
 ### Usage
 #### Set Java runtime environment
 ```bash
 export JAVA_HOME=$PATH_TO_JRE;
 export CLASSPATH=$PATH_RO_JDBC_DRIVER_JAR
 ```
 
-#### Start JVM
-Start JVM before initialization of Django
-
-```python
-import jpype
-jvm_path = jpype.getDefaultJVMPath()
-jpype.startJVM(jvm_path)
-```
-
 #### Update settings.DATABASES
 ##### Oracle
 
 change `django.db.backends.oracle` to `dj_db_conn_pool.backends.jdbc.oracle`:
 ```python
 DATABASES = {
     'default': {
@@ -175,9 +174,7 @@
 ```python
 DATABASES = {
     'default': {
         'ENGINE': 'dj_db_conn_pool.backends.jdbc.oceanbase'
     }
 }
 ```
-
-
```

### Comparing `django-db-connection-pool-1.2.2/README.md` & `django-db-connection-pool-1.2.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -107,34 +107,33 @@
 Or, you can use dj_db_conn_pool.setup to change default arguments(for each pool's creation), before using database pool:
 
 ```python
 import dj_db_conn_pool
 dj_db_conn_pool.setup(pool_size=100, max_overflow=50)
 ```
 
+#### multiprocessing environment
+In a multiprocessing environment, such as uWSGI, each process will have its own `dj_db_conn_pool.core:pool_container` object,
+It means that each process has an independent connection pool, for example: 
+The `POOL_OPTIONS` configuration of database `db1` is`{ 'POOL_SIZE': 10, 'MAX_OVERFLOW': 20 }`,
+If uWSGI starts 8 worker processes, then the total connection pool size of `db1`  is `8 * 10`,
+The maximum number of connections will not exceed `8 * 10 + 8 * 20`
+
+
 ## JDBC (experimental, NOT PRODUCTION READY)
-Thanks to [JPype](https://github.com/jpype-project/jpype) [JayDeBeApi](https://github.com/baztian/jaydebeapi/) ,
+Thanks to [JPype](https://github.com/jpype-project/jpype),
 django-db-connection-pool can connect to database in jdbc way
 
 ### Usage
 #### Set Java runtime environment
 ```bash
 export JAVA_HOME=$PATH_TO_JRE;
 export CLASSPATH=$PATH_RO_JDBC_DRIVER_JAR
 ```
 
-#### Start JVM
-Start JVM before initialization of Django
-
-```python
-import jpype
-jvm_path = jpype.getDefaultJVMPath()
-jpype.startJVM(jvm_path)
-```
-
 #### Update settings.DATABASES
 ##### Oracle
 
 change `django.db.backends.oracle` to `dj_db_conn_pool.backends.jdbc.oracle`:
 ```python
 DATABASES = {
     'default': {
```

### Comparing `django-db-connection-pool-1.2.2/README_cn.md` & `django-db-connection-pool-1.2.3/README_cn.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,207 +1,198 @@
-# django-db-connection-pool
-
-*:star: 如果这个库能对你有所帮助，不妨点个star，谢谢:smile:*
-
-驱动 Django 访问 MySQL、Oracle、PostgreSQL、JDBC (Oracle, OceanBase) 连接池的轮子, 
-基于 [SQLAlchemy](https://github.com/sqlalchemy/sqlalchemy) 队列池。
-在多进程、多线程 django 项目中，运行良好。
-
-* [English version](README.md)
-
-## 快速开始
-### 安装
-+ 使用 `pip` 安装所有所支持的数据库组件:
-```bash
-$ pip install django-db-connection-pool[all]
-```
-+ 或者是选择性安装数据库组件:
-```bash
-$ pip install django-db-connection-pool[mysql,oracle,postgresql,jdbc]
-```
-+ 或只选择部分组件，比如 Oracle
-```bash
-$ pip install django-db-connection-pool[oracle]
-```
-
-### 更新 settings.DATABASES 配置
-
-#### MySQL  
-将 ENGINE `django.db.backends.mysql` 更改为 `dj_db_conn_pool.backends.mysql`:
-```python
-DATABASES = {
-    'default': {
-        'ENGINE': 'dj_db_conn_pool.backends.mysql',
-        "NAME": "db1",
-        "USER": "user",
-        "PASSWORD": "password",
-        "HOST": "127.0.0.1",
-        "PORT": "3306",
-        "POOL_OPTIONS": {
-          "POOL_SIZE": 10,
-          "MAX_OVERFLOW": 10
-        }
-    }
-}
-```
-
-#### Oracle
-将 ENGINE `django.db.backends.oracle` 更改为 `dj_db_conn_pool.backends.oracle`:
-```python
-DATABASES = {
-    'default': {
-        'ENGINE': 'dj_db_conn_pool.backends.oracle',
-        "NAME": "db1",
-        "USER": "user",
-        "PASSWORD": "password",
-        "HOST": "127.0.0.1",
-        "PORT": "1521",
-        "POOL_OPTIONS": {
-          "POOL_SIZE": 10,
-          "MAX_OVERFLOW": 10
-        }
-    }
-}
-```
-
-#### PostgreSQL  
-将 ENGINE `django.db.backends.postgresql` 更改为 `dj_db_conn_pool.backends.postgresql`:
-```python
-DATABASES = {
-    'default': {
-        'ENGINE': 'dj_db_conn_pool.backends.postgresql',
-        "NAME": "db1",
-        "USER": "user",
-        "PASSWORD": "password",
-        "HOST": "127.0.0.1",
-        "PORT": "5432",
-        "POOL_OPTIONS": {
-          "POOL_SIZE": 10,
-          "MAX_OVERFLOW": 10
-        }
-    }
-}
-```
-
-#### 连接池配置（可选）
-目前连接池限制用户传入的连接池配置为：POOL_SIZE（连接池容量）、MAX_OVERFLOW（连接池容量向上浮动最大值）
-这两个参数包含在 `POOL_OPTIONS` 内，例如下面的配置，default 的连接池常规容量为10个连接，最大浮动10个，
-即为：在 default 连接池创建后，随着程序对连接池的请求，连接池内连接将逐步增加到10个，如果在连接池内连接
-全部用光后，程序又请求了第11个连接，此时的连接池容量将短暂超过 POOL_SIZE，但最大不超过 POOL_SIZE + MAX_OVERFLOW，
-如果程序请求 default 数据库的连接数量超过 POOL_SIZE + MAX_OVERFLOW，那么连接池将一直等待直到程序释放连接，
-请注意线程池对数据库连接池的使用，如果线程池大于连接池，且线程无主动释放连接的动作，可能会造成其他线程一直阻塞。
-
-```python
-DATABASES = {
-    'default': {
-        'POOL_OPTIONS' : {
-            'POOL_SIZE': 10,
-            'MAX_OVERFLOW': 10,
-            'RECYCLE': 24 * 60 * 60,
-            'PRE_PING': True,
-            'ECHO': False,
-            'TIMEOUT': 30,
-        }
-     }
- }
-```
-
-附这些参数的解释：(摘录于 SQLAlchemy 的文档):
-
-* **pool_size**: The size of the pool to be maintained,
-          defaults to 5. This is the largest number of connections that
-          will be kept persistently in the pool. Note that the pool
-          begins with no connections; once this number of connections
-          is requested, that number of connections will remain.
-          `pool_size` can be set to 0 to indicate no size limit; to
-          disable pooling, use a :class:`~sqlalchemy.pool.NullPool`
-          instead.
-
-* **max_overflow**: The maximum overflow size of the
-          pool. When the number of checked-out connections reaches the
-          size set in pool_size, additional connections will be
-          returned up to this limit. When those additional connections
-          are returned to the pool, they are disconnected and
-          discarded. It follows then that the total number of
-          simultaneous connections the pool will allow is pool_size +
-          `max_overflow`, and the total number of "sleeping"
-          connections the pool will allow is pool_size. `max_overflow`
-          can be set to -1 to indicate no overflow limit; no limit
-          will be placed on the total number of concurrent
-          connections. Defaults to 10.
-
-* **recycle**: If set to a value other than -1, number of seconds 
-          between connection recycling, which means upon checkout, 
-          if this timeout is surpassed the connection will be closed 
-          and replaced with a newly opened connection. 
-          Defaults to -1.       
-
-或者调用 `dj_db_conn_pool.setup` 覆盖默认参数
-
-```python
-import dj_db_conn_pool
-dj_db_conn_pool.setup(pool_size=10, max_overflow=20)
-```
-
-#### 多进程环境
-在多进程环境内，每个进程都会拥有一个`dj_db_conn_pool.core:pool_container`对象， 意味着每个进程都拥有一个独立的连接池，举例说明：  
-数据库`db1`的`POOL_OPTIONS`的配置是
-`{ 'POOL_SIZE': 10, 'MAX_OVERFLOW': 20 }`，项目启动了8个进程，则该项目的`db1`连接池总大小是`8 * 10`，最大连接数是`8 * 10 + 8 * 20`
-
-## JDBC（仍在完善中，不建议用于生产）
-基于 [JPype](https://github.com/jpype-project/jpype) [JayDeBeApi](https://github.com/baztian/jaydebeapi/) ，django-db-connection-pool 现在可以通过 jdbc 连接到数据库并保持连接
-
-### 使用方法
-#### 设置环境变量
-```bash
-export JAVA_HOME=$PATH_TO_JRE;
-export CLASSPATH=$PATH_RO_JDBC_DRIVER_JAR
-```
-
-#### 启动 JVM
-在引用 `dj_db_conn_pool.backends.jdbc.xxx` 前，调用 jpype 启动 JVM
-
-```python
-import jpype
-jvm_path = jpype.getDefaultJVMPath()
-jpype.startJVM(jvm_path)
-```
-
-#### 更新 settings.DATABASES 配置
-##### Oracle
-
-将 ENGINE `django.db.backends.oracle` 更改为 `dj_db_conn_pool.backends.jdbc.oracle`:
-```python
-DATABASES = {
-    'default': {
-        'ENGINE': 'dj_db_conn_pool.backends.jdbc.oracle',
-        "NAME": "db1",
-        "USER": "user",
-        "PASSWORD": "password",
-        "HOST": "127.0.0.1",
-        "PORT": "1521",
-        "POOL_OPTIONS": {
-          "POOL_SIZE": 10,
-          "MAX_OVERFLOW": 10
-        }
-    }
-}
-```
-
-##### OceanBase
-使用 `dj_db_conn_pool.backends.jdbc.oceanbase` 作为 Django 数据库后端:
-```python
-DATABASES = {
-    'default': {
-        'ENGINE': 'dj_db_conn_pool.backends.jdbc.oceanbase',
-        "NAME": "db1",
-        "USER": "user",
-        "PASSWORD": "password",
-        "HOST": "127.0.0.1",
-        "PORT": "2881",
-        "POOL_OPTIONS": {
-          "POOL_SIZE": 10,
-          "MAX_OVERFLOW": 10
-        }
-    }
-}
-```
+# django-db-connection-pool
+
+*:star: 如果这个库能对你有所帮助，不妨点个star，谢谢:smile:*
+
+驱动 Django 访问 MySQL、Oracle、PostgreSQL、JDBC (Oracle, OceanBase) 连接池的轮子, 
+基于 [SQLAlchemy](https://github.com/sqlalchemy/sqlalchemy) 队列池。
+在多进程、多线程 django 项目中，运行良好。
+
+* [English version](README.md)
+
+## 快速开始
+### 安装
++ 使用 `pip` 安装所有所支持的数据库组件:
+```bash
+$ pip install django-db-connection-pool[all]
+```
++ 或者是选择性安装数据库组件:
+```bash
+$ pip install django-db-connection-pool[mysql,oracle,postgresql,jdbc]
+```
++ 或只选择部分组件，比如 Oracle
+```bash
+$ pip install django-db-connection-pool[oracle]
+```
+
+### 更新 settings.DATABASES 配置
+
+#### MySQL  
+将 ENGINE `django.db.backends.mysql` 更改为 `dj_db_conn_pool.backends.mysql`:
+```python
+DATABASES = {
+    'default': {
+        'ENGINE': 'dj_db_conn_pool.backends.mysql',
+        "NAME": "db1",
+        "USER": "user",
+        "PASSWORD": "password",
+        "HOST": "127.0.0.1",
+        "PORT": "3306",
+        "POOL_OPTIONS": {
+          "POOL_SIZE": 10,
+          "MAX_OVERFLOW": 10
+        }
+    }
+}
+```
+
+#### Oracle
+将 ENGINE `django.db.backends.oracle` 更改为 `dj_db_conn_pool.backends.oracle`:
+```python
+DATABASES = {
+    'default': {
+        'ENGINE': 'dj_db_conn_pool.backends.oracle',
+        "NAME": "db1",
+        "USER": "user",
+        "PASSWORD": "password",
+        "HOST": "127.0.0.1",
+        "PORT": "1521",
+        "POOL_OPTIONS": {
+          "POOL_SIZE": 10,
+          "MAX_OVERFLOW": 10
+        }
+    }
+}
+```
+
+#### PostgreSQL  
+将 ENGINE `django.db.backends.postgresql` 更改为 `dj_db_conn_pool.backends.postgresql`:
+```python
+DATABASES = {
+    'default': {
+        'ENGINE': 'dj_db_conn_pool.backends.postgresql',
+        "NAME": "db1",
+        "USER": "user",
+        "PASSWORD": "password",
+        "HOST": "127.0.0.1",
+        "PORT": "5432",
+        "POOL_OPTIONS": {
+          "POOL_SIZE": 10,
+          "MAX_OVERFLOW": 10
+        }
+    }
+}
+```
+
+#### 连接池配置（可选）
+目前连接池限制用户传入的连接池配置为：POOL_SIZE（连接池容量）、MAX_OVERFLOW（连接池容量向上浮动最大值）
+这两个参数包含在 `POOL_OPTIONS` 内，例如下面的配置，default 的连接池常规容量为10个连接，最大浮动10个，
+即为：在 default 连接池创建后，随着程序对连接池的请求，连接池内连接将逐步增加到10个，如果在连接池内连接
+全部用光后，程序又请求了第11个连接，此时的连接池容量将短暂超过 POOL_SIZE，但最大不超过 POOL_SIZE + MAX_OVERFLOW，
+如果程序请求 default 数据库的连接数量超过 POOL_SIZE + MAX_OVERFLOW，那么连接池将一直等待直到程序释放连接，
+请注意线程池对数据库连接池的使用，如果线程池大于连接池，且线程无主动释放连接的动作，可能会造成其他线程一直阻塞。
+
+```python
+DATABASES = {
+    'default': {
+        'POOL_OPTIONS' : {
+            'POOL_SIZE': 10,
+            'MAX_OVERFLOW': 10,
+            'RECYCLE': 24 * 60 * 60,
+            'PRE_PING': True,
+            'ECHO': False,
+            'TIMEOUT': 30,
+        }
+     }
+ }
+```
+
+附这些参数的解释：(摘录于 SQLAlchemy 的文档):
+
+* **pool_size**: The size of the pool to be maintained,
+          defaults to 5. This is the largest number of connections that
+          will be kept persistently in the pool. Note that the pool
+          begins with no connections; once this number of connections
+          is requested, that number of connections will remain.
+          `pool_size` can be set to 0 to indicate no size limit; to
+          disable pooling, use a :class:`~sqlalchemy.pool.NullPool`
+          instead.
+
+* **max_overflow**: The maximum overflow size of the
+          pool. When the number of checked-out connections reaches the
+          size set in pool_size, additional connections will be
+          returned up to this limit. When those additional connections
+          are returned to the pool, they are disconnected and
+          discarded. It follows then that the total number of
+          simultaneous connections the pool will allow is pool_size +
+          `max_overflow`, and the total number of "sleeping"
+          connections the pool will allow is pool_size. `max_overflow`
+          can be set to -1 to indicate no overflow limit; no limit
+          will be placed on the total number of concurrent
+          connections. Defaults to 10.
+
+* **recycle**: If set to a value other than -1, number of seconds 
+          between connection recycling, which means upon checkout, 
+          if this timeout is surpassed the connection will be closed 
+          and replaced with a newly opened connection. 
+          Defaults to -1.       
+
+或者调用 `dj_db_conn_pool.setup` 覆盖默认参数
+
+```python
+import dj_db_conn_pool
+dj_db_conn_pool.setup(pool_size=10, max_overflow=20)
+```
+
+#### 多进程环境
+在多进程环境内，每个进程都会拥有一个`dj_db_conn_pool.core:pool_container`对象， 意味着每个进程都拥有一个独立的连接池，举例说明：  
+数据库`db1`的`POOL_OPTIONS`的配置是
+`{ 'POOL_SIZE': 10, 'MAX_OVERFLOW': 20 }`，项目启动了8个进程，则该项目的`db1`连接池总大小是`8 * 10`，最大连接数是`8 * 10 + 8 * 20`
+
+## JDBC（仍在完善中，不建议用于生产）
+基于 [JPype](https://github.com/jpype-project/jpype)，django-db-connection-pool 现在可以通过 jdbc 连接到数据库并保持连接
+
+### 使用方法
+#### 设置环境变量
+```bash
+export JAVA_HOME=$PATH_TO_JRE;
+export CLASSPATH=$PATH_RO_JDBC_DRIVER_JAR
+```
+
+#### 更新 settings.DATABASES 配置
+##### Oracle
+
+将 ENGINE `django.db.backends.oracle` 更改为 `dj_db_conn_pool.backends.jdbc.oracle`:
+```python
+DATABASES = {
+    'default': {
+        'ENGINE': 'dj_db_conn_pool.backends.jdbc.oracle',
+        "NAME": "db1",
+        "USER": "user",
+        "PASSWORD": "password",
+        "HOST": "127.0.0.1",
+        "PORT": "1521",
+        "POOL_OPTIONS": {
+          "POOL_SIZE": 10,
+          "MAX_OVERFLOW": 10
+        }
+    }
+}
+```
+
+##### OceanBase
+使用 `dj_db_conn_pool.backends.jdbc.oceanbase` 作为 Django 数据库后端:
+```python
+DATABASES = {
+    'default': {
+        'ENGINE': 'dj_db_conn_pool.backends.jdbc.oceanbase',
+        "NAME": "db1",
+        "USER": "user",
+        "PASSWORD": "password",
+        "HOST": "127.0.0.1",
+        "PORT": "2881",
+        "POOL_OPTIONS": {
+          "POOL_SIZE": 10,
+          "MAX_OVERFLOW": 10
+        }
+    }
+}
+```
```

### Comparing `django-db-connection-pool-1.2.2/setup.py` & `django-db-connection-pool-1.2.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# encoding: utf-8
+
 import codecs
 import shutil
 import setuptools
 
 from dj_db_conn_pool import (
     __version__,
     __author__,
@@ -30,36 +32,42 @@
         author=__author__,
         author_email=__author_email__,
         url='https://github.com/altairbow/django-db-connection-pool',
         download_url='https://pypi.python.org/pypi/django-db-connection-pool/',
         packages=setuptools.find_packages(),
         include_package_data=True,
         install_requires=[
-            'Django',
+            'Django>=2.0',
             'SQLAlchemy>=1.4.24',
+            'sqlparams>=4.0.0',
         ],
         extras_require={
             'all': [
-                'PyMySQL>=0.9.3', 'cx-Oracle>=6.4.1', 'psycopg2>=2.8.6',
-                'JayDeBeApi>=1.2.3', 'sqlparams>=3.0.0'
+                'JPype1>=1.3.0',
+                'sqlparams>=3.0.0',
+                'PyMySQL>=0.9.3',
+                'pyodbc>=4.0.34',
+                'cx-Oracle>=6.4.1',
+                'psycopg2>=2.8.6',
             ],
+            'jdbc': ['JPype1>=1.3.0'],
             'mysql': ['PyMySQL>=0.9.3'],
+            'odbc': ['pyodbc>=4.0.34'],
             'oracle': ['cx-Oracle>=6.4.1'],
             'postgresql': ['psycopg2>=2.8.6'],
-            'jdbc': ['JayDeBeApi>=1.2.3', 'sqlparams>=3.0.0'],
         },
         classifiers=[
             'Development Status :: 5 - Production/Stable',
             'Environment :: Web Environment',
             'Framework :: Django',
             'Intended Audience :: Developers',
             'License :: OSI Approved :: MIT License',
             'Operating System :: OS Independent',
             'Programming Language :: Python :: 3',
             'Topic :: Software Development :: Libraries :: Python Modules',
         ],
-        keywords=['django', 'db', 'database', 'persistent', 'connection', 'pool'],
+        keywords=['django', 'db', 'database', 'persistent', 'connection', 'pool', 'pooling'],
     )
 
 
 if __name__ == '__main__':
     setup()
```

