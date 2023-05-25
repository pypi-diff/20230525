# Comparing `tmp/sleuren-1.0.6.tar.gz` & `tmp/sleuren-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sleuren-1.0.6.tar", last modified: Mon May  1 12:40:30 2023, max compression
+gzip compressed data, was "sleuren-1.0.7.tar", last modified: Thu May 25 11:08:21 2023, max compression
```

## Comparing `sleuren-1.0.6.tar` & `sleuren-1.0.7.tar`

### file list

```diff
@@ -1,71 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:40:30.560358 sleuren-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-01 12:40:17.000000 sleuren-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-05-01 12:40:30.556358 sleuren-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-05-01 12:40:17.000000 sleuren-1.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 12:40:30.560358 sleuren-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-01 12:40:17.000000 sleuren-1.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:40:30.540357 sleuren-1.0.6/sleuren/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 12:40:17.000000 sleuren-1.0.6/sleuren/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:40:30.556358 sleuren-1.0.6/sleuren/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 12:40:17.000000 sleuren-1.0.6/sleuren/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-01 12:40:17.000000 sleuren-1.0.6/sleuren/plugins/apt-updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-01 12:40:17.000000 sleuren-1.0.6/sleuren/plugins/asterisk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-01 12:40:17.000000 sleuren-1.0.6/sleuren/plugins/bitninja.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-01 12:40:17.000000 sleuren-1.0.6/sleuren/plugins/cloudlinux-dbgov.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-01 12:40:17.000000 sleuren-1.0.6/sleuren/plugins/cloudlinux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-01 12:40:17.000000 sleuren-1.0.6/sleuren/plugins/cpanel.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2020 2023-05-01 12:40:17.000000 sleuren-1.0.6/sleuren/plugins/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-01 12:40:17.000000 sleuren-1.0.6/sleuren/plugins/cpu_freq.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-01 12:40:17.000000 sleuren-1.0.6/sleuren/plugins/dirsize.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-01 12:40:17.000000 sleuren-1.0.6/sleuren/plugins/diskinodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-01 12:40:17.000000 sleuren-1.0.6/sleuren/plugins/diskstatus-nvme.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-01 12:40:17.000000 sleuren-1.0.6/sleuren/plugins/diskstatus.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4138 2023-05-01 12:40:17.000000 sleuren-1.0.6/sleuren/plugins/diskusage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-05-01 12:40:17.000000 sleuren-1.0.6/sleuren/plugins/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-05-01 12:40:17.000000 sleuren-1.0.6/sleuren/plugins/elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-01 12:40:17.000000 sleuren-1.0.6/sleuren/plugins/exim.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-01 12:40:17.000000 sleuren-1.0.6/sleuren/plugins/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-05-01 12:40:17.000000 sleuren-1.0.6/sleuren/plugins/haproxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-05-01 12:40:17.000000 sleuren-1.0.6/sleuren/plugins/httpd.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5227 2023-05-01 12:40:17.000000 sleuren-1.0.6/sleuren/plugins/iostat.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-01 12:40:17.000000 sleuren-1.0.6/sleuren/plugins/janus.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-01 12:40:17.000000 sleuren-1.0.6/sleuren/plugins/kamailio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-01 12:40:17.000000 sleuren-1.0.6/sleuren/plugins/litespeed.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      332 2023-05-01 12:40:17.000000 sleuren-1.0.6/sleuren/plugins/loadavg.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-01 12:40:17.000000 sleuren-1.0.6/sleuren/plugins/loggedin.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-01 12:40:17.000000 sleuren-1.0.6/sleuren/plugins/mailq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-01 12:40:17.000000 sleuren-1.0.6/sleuren/plugins/mdstat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-05-01 12:40:17.000000 sleuren-1.0.6/sleuren/plugins/megacli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-05-01 12:40:17.000000 sleuren-1.0.6/sleuren/plugins/memcached.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      919 2023-05-01 12:40:17.000000 sleuren-1.0.6/sleuren/plugins/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-05-01 12:40:17.000000 sleuren-1.0.6/sleuren/plugins/minecraft.py
--rw-r--r--   0 runner    (1001) docker     (123)     5766 2023-05-01 12:40:17.000000 sleuren-1.0.6/sleuren/plugins/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-05-01 12:40:17.000000 sleuren-1.0.6/sleuren/plugins/mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-01 12:40:17.000000 sleuren-1.0.6/sleuren/plugins/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-05-01 12:40:17.000000 sleuren-1.0.6/sleuren/plugins/nginx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-01 12:40:17.000000 sleuren-1.0.6/sleuren/plugins/openvpn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-05-01 12:40:17.000000 sleuren-1.0.6/sleuren/plugins/phpfpm.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2673 2023-05-01 12:40:17.000000 sleuren-1.0.6/sleuren/plugins/ping.py
--rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-05-01 12:40:17.000000 sleuren-1.0.6/sleuren/plugins/plesk-cgroups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-01 12:40:17.000000 sleuren-1.0.6/sleuren/plugins/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-05-01 12:40:17.000000 sleuren-1.0.6/sleuren/plugins/powerdns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-01 12:40:17.000000 sleuren-1.0.6/sleuren/plugins/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-05-01 12:40:17.000000 sleuren-1.0.6/sleuren/plugins/rabbitmq.py
--rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-05-01 12:40:17.000000 sleuren-1.0.6/sleuren/plugins/redis_stat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      244 2023-05-01 12:40:17.000000 sleuren-1.0.6/sleuren/plugins/sleeper.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      364 2023-05-01 12:40:17.000000 sleuren-1.0.6/sleuren/plugins/swap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-05-01 12:40:17.000000 sleuren-1.0.6/sleuren/plugins/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-01 12:40:17.000000 sleuren-1.0.6/sleuren/plugins/temp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-05-01 12:40:17.000000 sleuren-1.0.6/sleuren/plugins/unbound.py
--rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-05-01 12:40:17.000000 sleuren-1.0.6/sleuren/plugins/vms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-01 12:40:17.000000 sleuren-1.0.6/sleuren/plugins/wp-toolkit.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-01 12:40:17.000000 sleuren-1.0.6/sleuren/plugins/yum-updates.py
--rw-r--r--   0 runner    (1001) docker     (123)    24473 2023-05-01 12:40:17.000000 sleuren-1.0.6/sleuren/sleuren.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 12:40:30.540357 sleuren-1.0.6/sleuren.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-05-01 12:40:30.000000 sleuren-1.0.6/sleuren.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-01 12:40:30.000000 sleuren-1.0.6/sleuren.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 12:40:30.000000 sleuren-1.0.6/sleuren.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-01 12:40:30.000000 sleuren-1.0.6/sleuren.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-01 12:40:30.000000 sleuren-1.0.6/sleuren.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-01 12:40:30.000000 sleuren-1.0.6/sleuren.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-01 12:40:17.000000 sleuren-1.0.6/sleuren.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:08:21.023585 sleuren-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-25 11:08:11.000000 sleuren-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-05-25 11:08:21.023585 sleuren-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-05-25 11:08:11.000000 sleuren-1.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 11:08:21.023585 sleuren-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-25 11:08:11.000000 sleuren-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:08:21.011585 sleuren-1.0.7/sleuren/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:08:21.023585 sleuren-1.0.7/sleuren/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren/plugins/apt-updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren/plugins/asterisk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren/plugins/bitninja.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren/plugins/cloudlinux-dbgov.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren/plugins/cloudlinux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren/plugins/cpanel.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2020 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren/plugins/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren/plugins/cpu_freq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren/plugins/dirsize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren/plugins/diskinodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren/plugins/diskstatus-nvme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren/plugins/diskstatus.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4138 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren/plugins/diskusage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren/plugins/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren/plugins/dovecot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren/plugins/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren/plugins/exim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren/plugins/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren/plugins/haproxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren/plugins/httpd.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5227 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren/plugins/iostat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren/plugins/janus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren/plugins/kamailio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren/plugins/litespeed.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      332 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren/plugins/loadavg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren/plugins/loggedin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren/plugins/mailq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren/plugins/mdstat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren/plugins/megacli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren/plugins/memcached.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      919 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren/plugins/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren/plugins/minecraft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5766 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren/plugins/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren/plugins/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren/plugins/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren/plugins/nginx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren/plugins/openvpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren/plugins/phpfpm.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2948 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren/plugins/ping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren/plugins/plesk-cgroups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren/plugins/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren/plugins/postfix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren/plugins/powerdns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren/plugins/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren/plugins/proftpd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren/plugins/rabbitmq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren/plugins/redis_stat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      244 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren/plugins/sleeper.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      364 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren/plugins/swap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren/plugins/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren/plugins/temp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren/plugins/unbound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren/plugins/vms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren/plugins/wp-toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren/plugins/yum-updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24473 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren/sleuren.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:08:21.015585 sleuren-1.0.7/sleuren.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-05-25 11:08:20.000000 sleuren-1.0.7/sleuren.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-05-25 11:08:21.000000 sleuren-1.0.7/sleuren.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 11:08:20.000000 sleuren-1.0.7/sleuren.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-25 11:08:20.000000 sleuren-1.0.7/sleuren.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-25 11:08:20.000000 sleuren-1.0.7/sleuren.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-25 11:08:20.000000 sleuren-1.0.7/sleuren.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-25 11:08:11.000000 sleuren-1.0.7/sleuren.ini
```

### Comparing `sleuren-1.0.6/LICENSE` & `sleuren-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.6/PKG-INFO` & `sleuren-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleuren
-Version: 1.0.6
+Version: 1.0.7
 Summary: Server monitoring agent
 Home-page: https://github.com/sleuren/agent
 Author: sleuren
 Author-email: hello@sleuren.com
 Maintainer: sleuren
 Maintainer-email: hello@sleuren.com
 License: MIT
```

### Comparing `sleuren-1.0.6/README.md` & `sleuren-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.6/setup.py` & `sleuren-1.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     install_requires = ['psutil==5.6.7', 'netifaces', 'configparser==3.5.0', 'future']
 else:
     install_requires = ['psutil', 'netifaces', 'configparser', 'future']
 
 
 setuptools.setup(
     name='sleuren',
-    version='1.0.6',
+    version='1.0.7',
     description='Server monitoring agent',
     long_description_content_type='text/markdown',
     long_description=readme,
     url='https://github.com/sleuren/agent',
     author='sleuren',
     author_email='hello@sleuren.com',
     maintainer='sleuren',
```

### Comparing `sleuren-1.0.6/sleuren/plugins/apt-updates.py` & `sleuren-1.0.7/sleuren/plugins/apt-updates.py`

 * *Files 19% similar despite different names*

```diff
@@ -19,11 +19,19 @@
         [apt-updates]
         enabled = yes
         interval = 3600
         '''
         data = {}
         data['security'] = int(os.popen('sudo -n apt-get upgrade -s | grep Inst | grep security | wc -l').read())
         data['other'] = int(os.popen('sudo -n apt-get upgrade -s | grep Inst | grep -v security | wc -l').read())
+        try:
+            checkreboot = config.get('apt-updates', 'checkreboot')
+            if os.path.exists('/var/run/reboot-required') and checkreboot == "true":
+                data['Reboot Required'] = 'Yes'
+            elif checkreboot == "true":
+                data['Reboot Required'] = 'No'
+        except Exception:
+            pass
         return data
 
 if __name__ == '__main__':
     Plugin().execute()
```

### Comparing `sleuren-1.0.6/sleuren/plugins/asterisk.py` & `sleuren-1.0.7/sleuren/plugins/asterisk.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.6/sleuren/plugins/bitninja.py` & `sleuren-1.0.7/sleuren/plugins/bitninja.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.6/sleuren/plugins/cloudlinux-dbgov.py` & `sleuren-1.0.7/sleuren/plugins/cloudlinux-dbgov.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.6/sleuren/plugins/cloudlinux.py` & `sleuren-1.0.7/sleuren/plugins/cloudlinux.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.6/sleuren/plugins/cpanel.py` & `sleuren-1.0.7/sleuren/plugins/cpanel.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.6/sleuren/plugins/cpu.py` & `sleuren-1.0.7/sleuren/plugins/cpu.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.6/sleuren/plugins/cpu_freq.py` & `sleuren-1.0.7/sleuren/plugins/cpu_freq.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.6/sleuren/plugins/dirsize.py` & `sleuren-1.0.7/sleuren/plugins/dirsize.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.6/sleuren/plugins/diskinodes.py` & `sleuren-1.0.7/sleuren/plugins/diskinodes.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.6/sleuren/plugins/diskstatus-nvme.py` & `sleuren-1.0.7/sleuren/plugins/diskstatus-nvme.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.6/sleuren/plugins/diskstatus.py` & `sleuren-1.0.7/sleuren/plugins/diskstatus.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.6/sleuren/plugins/diskusage.py` & `sleuren-1.0.7/sleuren/plugins/diskusage.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.6/sleuren/plugins/docker.py` & `sleuren-1.0.7/sleuren/plugins/docker.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.6/sleuren/plugins/elasticsearch.py` & `sleuren-1.0.7/sleuren/plugins/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.6/sleuren/plugins/gpu.py` & `sleuren-1.0.7/sleuren/plugins/gpu.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.6/sleuren/plugins/haproxy.py` & `sleuren-1.0.7/sleuren/plugins/haproxy.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,20 @@
             next_cache = dict()
             try:
                 username = config.get('haproxy', 'username')
                 password = config.get('haproxy', 'password')
                 user_pass = (username, password)
             except:
                 user_pass = False
-            request = requests.get(config.get('haproxy', 'status_page_url'), auth=user_pass)
+            status_page_url = config.get('haproxy', 'status_page_url')
+            if not ";csv" in status_page_url:
+                status_page_url = status_page_url + ";csv"
+
+            request = requests.get(status_page_url, auth=user_pass)
+
             next_cache['ts'] = time.time()
             prev_cache = self.get_agent_cache()  # Get absolute values from previous check
             if request.status_code is 200:
                 response = request.text.split("\n")
             else:
                 return "Could not load haproxy status page: {}".format(request.text)
```

### Comparing `sleuren-1.0.6/sleuren/plugins/httpd.py` & `sleuren-1.0.7/sleuren/plugins/httpd.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.6/sleuren/plugins/iostat.py` & `sleuren-1.0.7/sleuren/plugins/iostat.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.6/sleuren/plugins/janus.py` & `sleuren-1.0.7/sleuren/plugins/janus.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.6/sleuren/plugins/kamailio.py` & `sleuren-1.0.7/sleuren/plugins/kamailio.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.6/sleuren/plugins/litespeed.py` & `sleuren-1.0.7/sleuren/plugins/litespeed.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.6/sleuren/plugins/mailq.py` & `sleuren-1.0.7/sleuren/plugins/mailq.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.6/sleuren/plugins/mdstat.py` & `sleuren-1.0.7/sleuren/plugins/mdstat.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.6/sleuren/plugins/megacli.py` & `sleuren-1.0.7/sleuren/plugins/megacli.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.6/sleuren/plugins/memcached.py` & `sleuren-1.0.7/sleuren/plugins/memcached.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.6/sleuren/plugins/memory.py` & `sleuren-1.0.7/sleuren/plugins/memory.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.6/sleuren/plugins/minecraft.py` & `sleuren-1.0.7/sleuren/plugins/minecraft.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.6/sleuren/plugins/mongodb.py` & `sleuren-1.0.7/sleuren/plugins/mongodb.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.6/sleuren/plugins/mysql.py` & `sleuren-1.0.7/sleuren/plugins/mysql.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.6/sleuren/plugins/network.py` & `sleuren-1.0.7/sleuren/plugins/network.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.6/sleuren/plugins/nginx.py` & `sleuren-1.0.7/sleuren/plugins/nginx.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.6/sleuren/plugins/openvpn.py` & `sleuren-1.0.7/sleuren/plugins/openvpn.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.6/sleuren/plugins/phpfpm.py` & `sleuren-1.0.7/sleuren/plugins/phpfpm.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.6/sleuren/plugins/ping.py` & `sleuren-1.0.7/sleuren/plugins/ping.py`

 * *Files 18% similar despite different names*

```diff
@@ -55,27 +55,34 @@
         matched = _get_match_groups(response, matcher)
         if matched is False:
             response = -1
         else:
             minping, avgping, maxping, jitter = matched
             response = avgping
     elif sys.platform == "win32":
+        #response = 0
         response = -1
         try:
             ping = Popen(["ping", "-n", "1 ", hostname], stdout=PIPE, stderr=PIPE)
             out, error = ping.communicate()
             if out:
                 try:
                     response = int(re.findall(r"Average = (\d+)", out)[0])
                 except Exception:
                     pass
             else:
                 response = -1
         except CalledProcessError:
             pass
+        if response == -1:
+            try:
+                rxresponse = re.findall(br" + .+ = [0-9]{1,9}ms, .+ = [0-9]{1,9}ms, .+ = (\d+){1,9}ms", out)
+                response = rxresponse[0].decode()
+            except Exception:
+                pass
     else:
         response = -1
     return {'avgping': response, 'host': hostname}
 
 
 class Plugin(plugins.BasePlugin):
     __name__ = 'ping'
@@ -86,8 +93,8 @@
         data['ping'] = []
         for host in my_hosts:
             data['ping'].append(collect_ping(host))
         return data['ping']
 
 
 if __name__ == '__main__':
-    Plugin().execute()
+    Plugin().execute()
```

### Comparing `sleuren-1.0.6/sleuren/plugins/plesk-cgroups.py` & `sleuren-1.0.7/sleuren/plugins/plesk-cgroups.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.6/sleuren/plugins/plugins.py` & `sleuren-1.0.7/sleuren/plugins/plugins.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.6/sleuren/plugins/powerdns.py` & `sleuren-1.0.7/sleuren/plugins/powerdns.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.6/sleuren/plugins/process.py` & `sleuren-1.0.7/sleuren/plugins/process.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.6/sleuren/plugins/rabbitmq.py` & `sleuren-1.0.7/sleuren/plugins/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.6/sleuren/plugins/redis_stat.py` & `sleuren-1.0.7/sleuren/plugins/redis_stat.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.6/sleuren/plugins/system.py` & `sleuren-1.0.7/sleuren/plugins/system.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.6/sleuren/plugins/temp.py` & `sleuren-1.0.7/sleuren/plugins/temp.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.6/sleuren/plugins/unbound.py` & `sleuren-1.0.7/sleuren/plugins/unbound.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.6/sleuren/plugins/vms.py` & `sleuren-1.0.7/sleuren/plugins/vms.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.6/sleuren/plugins/wp-toolkit.py` & `sleuren-1.0.7/sleuren/plugins/wp-toolkit.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.6/sleuren/plugins/yum-updates.py` & `sleuren-1.0.7/sleuren/plugins/yum-updates.py`

 * *Files identical despite different names*

### Comparing `sleuren-1.0.6/sleuren/sleuren.py` & `sleuren-1.0.7/sleuren/sleuren.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     from urllib.request import urlopen, Request
     from urllib.error import HTTPError
 except ImportError:
     from urlparse import urlparse
     from urllib import urlencode
     from urllib2 import urlopen, Request, HTTPError
 
-__version__ = '1.0.6'
+__version__ = '1.0.7'
 __FILEABSDIRNAME__ = os.path.dirname(os.path.abspath(__file__))
 
 ini_files = (
     os.path.join('/etc', 'sleuren.ini'),
     os.path.join('/etc', 'sleuren-token.ini'),
     os.path.join(os.path.dirname(__FILEABSDIRNAME__), 'sleuren.ini'),
     os.path.join(os.path.dirname(__FILEABSDIRNAME__), 'sleuren-token.ini'),
```

### Comparing `sleuren-1.0.6/sleuren.egg-info/PKG-INFO` & `sleuren-1.0.7/sleuren.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleuren
-Version: 1.0.6
+Version: 1.0.7
 Summary: Server monitoring agent
 Home-page: https://github.com/sleuren/agent
 Author: sleuren
 Author-email: hello@sleuren.com
 Maintainer: sleuren
 Maintainer-email: hello@sleuren.com
 License: MIT
```

### Comparing `sleuren-1.0.6/sleuren.egg-info/SOURCES.txt` & `sleuren-1.0.7/sleuren.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 sleuren/plugins/cpu_freq.py
 sleuren/plugins/dirsize.py
 sleuren/plugins/diskinodes.py
 sleuren/plugins/diskstatus-nvme.py
 sleuren/plugins/diskstatus.py
 sleuren/plugins/diskusage.py
 sleuren/plugins/docker.py
+sleuren/plugins/dovecot.py
 sleuren/plugins/elasticsearch.py
 sleuren/plugins/exim.py
 sleuren/plugins/gpu.py
 sleuren/plugins/haproxy.py
 sleuren/plugins/httpd.py
 sleuren/plugins/iostat.py
 sleuren/plugins/janus.py
@@ -47,16 +48,18 @@
 sleuren/plugins/network.py
 sleuren/plugins/nginx.py
 sleuren/plugins/openvpn.py
 sleuren/plugins/phpfpm.py
 sleuren/plugins/ping.py
 sleuren/plugins/plesk-cgroups.py
 sleuren/plugins/plugins.py
+sleuren/plugins/postfix.py
 sleuren/plugins/powerdns.py
 sleuren/plugins/process.py
+sleuren/plugins/proftpd.py
 sleuren/plugins/rabbitmq.py
 sleuren/plugins/redis_stat.py
 sleuren/plugins/sleeper.py
 sleuren/plugins/swap.py
 sleuren/plugins/system.py
 sleuren/plugins/temp.py
 sleuren/plugins/unbound.py
```

