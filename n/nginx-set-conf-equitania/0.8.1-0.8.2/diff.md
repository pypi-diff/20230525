# Comparing `tmp/nginx-set-conf-equitania-0.8.1.tar.gz` & `tmp/nginx-set-conf-equitania-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nginx-set-conf-equitania-0.8.1.tar", last modified: Wed May 10 12:47:39 2023, max compression
+gzip compressed data, was "nginx-set-conf-equitania-0.8.2.tar", last modified: Thu May 25 10:00:06 2023, max compression
```

## Comparing `nginx-set-conf-equitania-0.8.1.tar` & `nginx-set-conf-equitania-0.8.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 picard     (501) staff       (20)        0 2023-05-10 12:47:39.837492 nginx-set-conf-equitania-0.8.1/
--rw-r--r--   0 picard     (501) staff       (20)    33892 2021-05-25 14:23:55.000000 nginx-set-conf-equitania-0.8.1/LICENSE.txt
--rw-r--r--   0 picard     (501) staff       (20)     3320 2023-05-10 12:47:39.837239 nginx-set-conf-equitania-0.8.1/PKG-INFO
--rw-r--r--   0 picard     (501) staff       (20)     2818 2023-01-21 08:58:48.000000 nginx-set-conf-equitania-0.8.1/README.md
-drwxr-xr-x   0 picard     (501) staff       (20)        0 2023-05-10 12:47:39.833801 nginx-set-conf-equitania-0.8.1/nginx_set_conf/
--rw-r--r--   0 picard     (501) staff       (20)       50 2021-05-27 17:15:29.000000 nginx-set-conf-equitania-0.8.1/nginx_set_conf/__init__.py
--rw-r--r--   0 picard     (501) staff       (20)    21510 2023-05-10 12:46:09.000000 nginx-set-conf-equitania-0.8.1/nginx_set_conf/config_templates.py
--rw-r--r--   0 picard     (501) staff       (20)     4006 2023-05-02 13:29:17.000000 nginx-set-conf-equitania-0.8.1/nginx_set_conf/nginx_set_conf.py
--rw-r--r--   0 picard     (501) staff       (20)     7078 2023-05-02 13:16:56.000000 nginx-set-conf-equitania-0.8.1/nginx_set_conf/utils.py
-drwxr-xr-x   0 picard     (501) staff       (20)        0 2023-05-10 12:47:39.836617 nginx-set-conf-equitania-0.8.1/nginx_set_conf_equitania.egg-info/
--rw-r--r--   0 picard     (501) staff       (20)     3320 2023-05-10 12:47:39.000000 nginx-set-conf-equitania-0.8.1/nginx_set_conf_equitania.egg-info/PKG-INFO
--rw-r--r--   0 picard     (501) staff       (20)      439 2023-05-10 12:47:39.000000 nginx-set-conf-equitania-0.8.1/nginx_set_conf_equitania.egg-info/SOURCES.txt
--rw-r--r--   0 picard     (501) staff       (20)        1 2023-05-10 12:47:39.000000 nginx-set-conf-equitania-0.8.1/nginx_set_conf_equitania.egg-info/dependency_links.txt
--rw-r--r--   0 picard     (501) staff       (20)       86 2023-05-10 12:47:39.000000 nginx-set-conf-equitania-0.8.1/nginx_set_conf_equitania.egg-info/entry_points.txt
--rw-r--r--   0 picard     (501) staff       (20)       27 2023-05-10 12:47:39.000000 nginx-set-conf-equitania-0.8.1/nginx_set_conf_equitania.egg-info/requires.txt
--rw-r--r--   0 picard     (501) staff       (20)       15 2023-05-10 12:47:39.000000 nginx-set-conf-equitania-0.8.1/nginx_set_conf_equitania.egg-info/top_level.txt
--rw-r--r--   0 picard     (501) staff       (20)       38 2023-05-10 12:47:39.837563 nginx-set-conf-equitania-0.8.1/setup.cfg
--rw-r--r--   0 picard     (501) staff       (20)      903 2023-05-10 12:46:45.000000 nginx-set-conf-equitania-0.8.1/setup.py
+drwxr-xr-x   0 picard     (501) staff       (20)        0 2023-05-25 10:00:06.865710 nginx-set-conf-equitania-0.8.2/
+-rw-r--r--   0 picard     (501) staff       (20)    33892 2021-05-25 14:23:55.000000 nginx-set-conf-equitania-0.8.2/LICENSE.txt
+-rw-r--r--   0 picard     (501) staff       (20)     3320 2023-05-25 10:00:06.865259 nginx-set-conf-equitania-0.8.2/PKG-INFO
+-rw-r--r--   0 picard     (501) staff       (20)     2818 2023-01-21 08:58:48.000000 nginx-set-conf-equitania-0.8.2/README.md
+drwxr-xr-x   0 picard     (501) staff       (20)        0 2023-05-25 10:00:06.859965 nginx-set-conf-equitania-0.8.2/nginx_set_conf/
+-rw-r--r--   0 picard     (501) staff       (20)       50 2021-05-27 17:15:29.000000 nginx-set-conf-equitania-0.8.2/nginx_set_conf/__init__.py
+-rw-r--r--   0 picard     (501) staff       (20)    21092 2023-05-25 09:54:50.000000 nginx-set-conf-equitania-0.8.2/nginx_set_conf/config_templates.py
+-rw-r--r--   0 picard     (501) staff       (20)     4006 2023-05-02 13:29:17.000000 nginx-set-conf-equitania-0.8.2/nginx_set_conf/nginx_set_conf.py
+-rw-r--r--   0 picard     (501) staff       (20)     7078 2023-05-02 13:16:56.000000 nginx-set-conf-equitania-0.8.2/nginx_set_conf/utils.py
+drwxr-xr-x   0 picard     (501) staff       (20)        0 2023-05-25 10:00:06.864196 nginx-set-conf-equitania-0.8.2/nginx_set_conf_equitania.egg-info/
+-rw-r--r--   0 picard     (501) staff       (20)     3320 2023-05-25 10:00:06.000000 nginx-set-conf-equitania-0.8.2/nginx_set_conf_equitania.egg-info/PKG-INFO
+-rw-r--r--   0 picard     (501) staff       (20)      439 2023-05-25 10:00:06.000000 nginx-set-conf-equitania-0.8.2/nginx_set_conf_equitania.egg-info/SOURCES.txt
+-rw-r--r--   0 picard     (501) staff       (20)        1 2023-05-25 10:00:06.000000 nginx-set-conf-equitania-0.8.2/nginx_set_conf_equitania.egg-info/dependency_links.txt
+-rw-r--r--   0 picard     (501) staff       (20)       86 2023-05-25 10:00:06.000000 nginx-set-conf-equitania-0.8.2/nginx_set_conf_equitania.egg-info/entry_points.txt
+-rw-r--r--   0 picard     (501) staff       (20)       27 2023-05-25 10:00:06.000000 nginx-set-conf-equitania-0.8.2/nginx_set_conf_equitania.egg-info/requires.txt
+-rw-r--r--   0 picard     (501) staff       (20)       15 2023-05-25 10:00:06.000000 nginx-set-conf-equitania-0.8.2/nginx_set_conf_equitania.egg-info/top_level.txt
+-rw-r--r--   0 picard     (501) staff       (20)       38 2023-05-25 10:00:06.865782 nginx-set-conf-equitania-0.8.2/setup.cfg
+-rw-r--r--   0 picard     (501) staff       (20)      903 2023-05-25 09:46:50.000000 nginx-set-conf-equitania-0.8.2/setup.py
```

### Comparing `nginx-set-conf-equitania-0.8.1/LICENSE.txt` & `nginx-set-conf-equitania-0.8.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nginx-set-conf-equitania-0.8.1/PKG-INFO` & `nginx-set-conf-equitania-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nginx-set-conf-equitania
-Version: 0.8.1
+Version: 0.8.2
 Summary: A package to create configurations for nginx with/without pagespeed for different web applications
 Author: Equitania Software GmbH
 Author-email: info@equitania.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `nginx-set-conf-equitania-0.8.1/README.md` & `nginx-set-conf-equitania-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `nginx-set-conf-equitania-0.8.1/nginx_set_conf/config_templates.py` & `nginx-set-conf-equitania-0.8.2/nginx_set_conf/config_templates.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 config_template_dict = {
 "ngx_code_server": """# Template for code-server configuration nginx incl. SSL/http2
-# Version 3.8 from 10.05.2023
+# Version 3.9 from 25.05.2023
 # upstream server.domain.de {
 #     server ip.ip.ip.ip weight=1 fail_timeout=0;
 # }
 
 server {
     listen server.domain.de:80;
     server_name server.domain.de;
@@ -59,21 +59,19 @@
     access_log off;
 
     location ~ ^/(.*)
     {
         # Connect to local port
         proxy_pass http://127.0.0.1:oldport;
     }
-    # Pagespeed
-    pagespeed off;
 }
 """,
 
 "ngx_fast_report": """# Template for FastReport configuration nginx incl. SSL/http2
-# Version 3.8 from 10.05.2023
+# Version 3.9 from 25.05.2023
 # upstream server.domain.de {
 #     server ip.ip.ip.ip weight=1 fail_timeout=0;
 # }
 
 server {
     listen server.domain.de:80;
     server_name server.domain.de;
@@ -128,21 +126,19 @@
     proxy_set_header X-Real-IP $remote_addr;
 
     # Proxy for docker
     location / {
         # Connect to local port
         proxy_pass http://127.0.0.1:oldport;
     }
-    # Pagespeed
-    pagespeed off;
 }
 """,
 
 "ngx_nextcloud": """# Template for NextCloud configuration nginx incl. SSL/http2
-# Version 3.8 from 10.05.2023
+# Version 3.9 from 25.05.2023
 # upstream server.domain.de {
 #     server ip.ip.ip.ip weight=1 fail_timeout=0;
 # }
 
 server {
     listen server.domain.de:80;
     server_name server.domain.de;
@@ -208,21 +204,19 @@
         #include /etc/nginx/proxy_params;
         proxy_set_header Host $http_host;
         proxy_set_header X-Real-IP $remote_addr;
         proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;
         proxy_set_header X-Forwarded-Proto $scheme;        # Connect to local port
         proxy_pass http://127.0.0.1:oldport;
     }
-    # Pagespeed
-    pagespeed off;
-}""",
-
+}
+""",
 
 "ngx_portainer": """# Template for Portainer configuration nginx incl. SSL/http2
-# Version 3.8 from 10.05.2023
+# Version 3.9 from 25.05.2023
 # upstream server.domain.de {
 #     server ip.ip.ip.ip weight=1 fail_timeout=0;
 # }
 
 server {
     listen server.domain.de:80;
     server_name server.domain.de;
@@ -265,20 +259,19 @@
         proxy_set_header Upgrade $http_upgrade;
         proxy_set_header Connection "upgrade";
         proxy_set_header Host $http_host;
         proxy_set_header X-Real-IP $remote_addr;
         proxy_set_header X-Real-PORT $remote_port;
         proxy_pass http://127.0.0.1:oldport;
     }
-    # Pagespeed
-    pagespeed off;
-}""",
+}
+""",
 
 "ngx_odoo_http": """# Template for Odoo configuration nginx
-# Version 3.8 from 10.05.2023
+# Version 3.9 from 25.05.2023
 # upstream server.domain.de {
 #     server ip.ip.ip.ip weight=1 fail_timeout=0;
 # }
 
 server {
     listen server.domain.de:80;
     server_name server.domain.de;
@@ -332,20 +325,19 @@
 
     location ~* /web/static/ {
         proxy_cache_valid 200 60m;
         proxy_buffering    on;
         expires 864000;
         proxy_pass http://127.0.0.1:oldport;
     }
-    # Pagespeed
-    pagespeed off;
-}""",
+}
+""",
 
 "ngx_odoo_ssl": """# Template for Odoo configuration nginx incl. SSL
-# Version 3.8 from 10.05.2023
+# Version 3.9 from 25.05.2023
 # upstream server.domain.de {
 #     server ip.ip.ip.ip weight=1 fail_timeout=0;
 # }
 
 server {
     listen server.domain.de:80;
     server_name server.domain.de;
@@ -418,19 +410,15 @@
 
     location ~* /web/static/ {
         proxy_cache_valid 200 60m;
         proxy_buffering    on;
         expires 864000;
         proxy_pass http://127.0.0.1:oldport;
     }
-    #include "pagespeed_main.conf";
-    # Pagespeed
-    pagespeed off;
 }
-
 """,
 
 "ngx_odoo_ssl_pagespeed": """# Template for Odoo configuration nginx incl. SSL/http2 and Google PageSpeed
 # source: https://github.com/apache/incubator-pagespeed-ngx/blob/master/scripts/build_ngx_pagespeed.sh
 # Version 3.8 from 10.05.2023
 # upstream server.domain.de {
 #     server ip.ip.ip.ip weight=1 fail_timeout=0;
@@ -517,15 +505,15 @@
 
     include "pagespeed_main.conf";
     # Pagespeed
     pagespeed on;
 }""",
 
 "ngx_pgadmin": """# Template for pgAdmin configuration nginx incl. SSL/http2
-# Version 3.8 from 10.05.2023
+# Version 3.9 from 25.05.2023
 # upstream server.domain.de {
 #     server ip.ip.ip.ip weight=1 fail_timeout=0;
 # }
 
 server {
     listen server.domain.de:80;
     server_name server.domain.de;
@@ -572,21 +560,19 @@
         # Connect to local port
         proxy_set_header Host $host;
         proxy_set_header X-Real-IP $remote_addr;
         proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;
         proxy_set_header X-Forwarded-Proto https;
         proxy_pass http://127.0.0.1:oldport;
     }
-    # Pagespeed
-    pagespeed off;
 }
 """,
 
 "ngx_pwa": """# Template for Progressive Web App .NET Core configuration nginx incl. SSL/http2
-# Version 3.8 from 10.05.2023
+# Version 3.9 from 25.05.2023
 # upstream server.domain.de {
 #     server ip.ip.ip.ip weight=1 fail_timeout=0;
 # }
 
 server {
     listen server.domain.de:80;
     server_name server.domain.de;
@@ -637,33 +623,31 @@
     proxy_set_header X-Real-IP $remote_addr;
 
     # Proxy for docker
     location / {
         # Connect to local port
         proxy_pass http://127.0.0.1:oldport;
     }
-    # Pagespeed
-    pagespeed off;
-}""",
+}
+""",
 
 "ngx_redirect": """# Template for Redirect Domain configuration nginx
-# Version 3.6 from 10.05.2023
+# Version 3.7 from 25.05.2023
 upstream server.domain.de {
     server ip.ip.ip.ip weight=1 fail_timeout=0;
 }
 
 server {
     listen server.domain.de:80;
     server_name server.domain.de;
     rewrite ^/.*$ http://target.domain.de$request_uri? permanent;
     access_log /var/log/nginx/target.domain.de-access.log;
     error_log /var/log/nginx/target.domain.de-error.log;
-    # Pagespeed
-    pagespeed off;
-}""",
+}
+""",
 
 "ngx_redirect_ssl": """# Template for Redirect domain configuration nginx ssl/http2
 # Version 3.8 from 10.05.2023
 # upstream server.domain.de {
 #     server ip.ip.ip.ip weight=1 fail_timeout=0;
 # }
 
@@ -698,18 +682,16 @@
     ssl_protocols        TLSv1.3 TLSv1.2;
     ssl_prefer_server_ciphers on;
     ssl_ciphers         HIGH:!aNULL:!MD5;
 
     # limit ciphers
     ssl_session_cache    shared:SSL:1m;
     ssl_session_timeout  5m;
-    #include "pagespeed_main.conf";
-    # Pagespeed
-    pagespeed off;
-}"""
+}
+"""
 }
 
 
 def get_config_template(config_template_name):
     if config_template_name in config_template_dict:
         return config_template_dict[config_template_name]
     else:
```

### Comparing `nginx-set-conf-equitania-0.8.1/nginx_set_conf/nginx_set_conf.py` & `nginx-set-conf-equitania-0.8.2/nginx_set_conf/nginx_set_conf.py`

 * *Files identical despite different names*

### Comparing `nginx-set-conf-equitania-0.8.1/nginx_set_conf/utils.py` & `nginx-set-conf-equitania-0.8.2/nginx_set_conf/utils.py`

 * *Files identical despite different names*

### Comparing `nginx-set-conf-equitania-0.8.1/nginx_set_conf_equitania.egg-info/PKG-INFO` & `nginx-set-conf-equitania-0.8.2/nginx_set_conf_equitania.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nginx-set-conf-equitania
-Version: 0.8.1
+Version: 0.8.2
 Summary: A package to create configurations for nginx with/without pagespeed for different web applications
 Author: Equitania Software GmbH
 Author-email: info@equitania.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `nginx-set-conf-equitania-0.8.1/setup.py` & `nginx-set-conf-equitania-0.8.2/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nginx-set-conf-equitania",
-    version="0.8.1",
+    version="0.8.2",
     author="Equitania Software GmbH",
     author_email="info@equitania.de",
     description="A package to create configurations for nginx with/without pagespeed for different web applications",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=['nginx_set_conf'],
     classifiers=[
```

