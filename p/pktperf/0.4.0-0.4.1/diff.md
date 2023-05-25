# Comparing `tmp/pktperf-0.4.0.tar.gz` & `tmp/pktperf-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pktperf-0.4.0.tar", last modified: Fri Feb 17 04:20:15 2023, max compression
+gzip compressed data, was "pktperf-0.4.1.tar", last modified: Thu May 25 12:11:55 2023, max compression
```

## Comparing `pktperf-0.4.0.tar` & `pktperf-0.4.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 04:20:15.381338 pktperf-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-02-17 04:20:01.000000 pktperf-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-02-17 04:20:15.381338 pktperf-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-02-17 04:20:01.000000 pktperf-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 04:20:15.381338 pktperf-0.4.0/pktperf/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-02-17 04:20:01.000000 pktperf-0.4.0/pktperf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17067 2023-02-17 04:20:01.000000 pktperf-0.4.0/pktperf/pktgen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-02-17 04:20:01.000000 pktperf-0.4.0/pktperf/pktperf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-02-17 04:20:01.000000 pktperf-0.4.0/pktperf/pktsar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 04:20:15.381338 pktperf-0.4.0/pktperf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-02-17 04:20:15.000000 pktperf-0.4.0/pktperf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-02-17 04:20:15.000000 pktperf-0.4.0/pktperf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 04:20:15.000000 pktperf-0.4.0/pktperf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-17 04:20:15.000000 pktperf-0.4.0/pktperf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-17 04:20:15.000000 pktperf-0.4.0/pktperf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-02-17 04:20:01.000000 pktperf-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-17 04:20:15.381338 pktperf-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-02-17 04:20:01.000000 pktperf-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:11:55.198103 pktperf-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-05-25 12:11:36.000000 pktperf-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-05-25 12:11:55.198103 pktperf-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-05-25 12:11:36.000000 pktperf-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:11:55.198103 pktperf-0.4.1/pktperf/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-25 12:11:36.000000 pktperf-0.4.1/pktperf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17534 2023-05-25 12:11:36.000000 pktperf-0.4.1/pktperf/pktgen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-05-25 12:11:36.000000 pktperf-0.4.1/pktperf/pktperf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-25 12:11:36.000000 pktperf-0.4.1/pktperf/pktsar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 12:11:55.198103 pktperf-0.4.1/pktperf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-05-25 12:11:55.000000 pktperf-0.4.1/pktperf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-25 12:11:55.000000 pktperf-0.4.1/pktperf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 12:11:55.000000 pktperf-0.4.1/pktperf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-25 12:11:55.000000 pktperf-0.4.1/pktperf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-25 12:11:55.000000 pktperf-0.4.1/pktperf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-25 12:11:36.000000 pktperf-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 12:11:55.198103 pktperf-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-25 12:11:36.000000 pktperf-0.4.1/setup.py
```

### Comparing `pktperf-0.4.0/LICENSE` & `pktperf-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pktperf-0.4.0/PKG-INFO` & `pktperf-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pktperf
-Version: 0.4.0
+Version: 0.4.1
 Summary: pktgen python scripts
 Author: junka
 Author-email: wan.junjie@fixmail.com
 Project-URL: Bug Tracker, https://github.com/junka/pktperf/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.5
```

### Comparing `pktperf-0.4.0/README.md` & `pktperf-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pktperf-0.4.0/pktperf/pktgen.py` & `pktperf-0.4.1/pktperf/pktgen.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# -*- coding: UTF-8 -*-
 """
 classes provide functions for pktgen operation
 """
 import sys
 import re
 import os
 import ipaddress
@@ -43,15 +44,15 @@
             threads: number of threads to start
             first_thread: index of first thread to start
             clone: number of skb clones sent before alloc new skb
             num: number of packets to send per thread, 0 means indefinitely
             burst: hw level bursting of skbs
             verbose: verbose
             debug: debug
-            ip6: send IPv6 packets
+            ipv6: send IPv6 packets
             flows: limit number of flows
             flow_len: packets number a flow will send
             tx_delay: tx delay value in ns
             append: script will not reset generator state, append its config
             queue: queue mapping with irq affinity
         """
         if self.os_check() is False:
@@ -64,49 +65,51 @@
         is_exists = os.path.exists(mod)
         if is_exists is False:
             print("No pktgen module\nPlease do \'modprobe pktgen\'")
             sys.exit(0)
         self.pgdev = args.interface
         self.pkt_size = int(args.size)
         self.dst_mac = args.mac
-        self.__init_ip_dst(args.ip6, args.dest)
+        self.__init_ip_dst(args.ipv6, args.dest)
         self.__init_port_range(args.portrange)
         self.frags = None
         self.csum = args.txcsum
         self.debug = args.debug
         self.verbose = args.verbose
         self.append = args.append
         if args.clone is not None:
             self.clone = int(args.clone)
         self.num = int(args.num)
         if args.burst is not None:
             self.burst = int(args.burst)
         if args.threads is not None:
             self.threads = int(args.threads)
         self.stats = []
-        if args.first_thread is not None:
-            self.first_thread = int(args.first_thread)
+        if args.firstthread is not None:
+            self.first_thread = int(args.firstthread)
         if args.delay is not None:
             self.tx_delay = int(args.delay)
         if args.flows is not None:
             self.flows = int(args.flows)
         if args.flowpkt is not None:
             self.flow_len = int(args.flowpkt)
-        self.__init_irq(args.queue_map)
+        self.__init_irq(args.queuemap)
         if args.tos is not None:
             self.tos = int(args.tos)
         self.bps_rate = args.bps
         self.pps_rate = args.pps
         if args.frags is not None:
             self.frags = int(args.frags)
+        self.vlan = args.vlan
+        self.svlan = args.svlan
 
-    def __init_ip_dst(self, is_ipv6, dest):
+    def __init_ip_dst(self, is_ipv6, dest_ip):
         """ Init pktgen module ip dst """
         self.ipv6 = is_ipv6
-        if dest is None:
+        if dest_ip is None:
             if self.ipv6 is True:
                 dest_ip = "FD00::1"
             else:
                 dest_ip = "198.18.0.42"
         net = None
         try:
             net = ipaddress.ip_network(dest_ip, strict=False)
@@ -206,14 +209,21 @@
         """config tos """
         if self.tos is not None and self.tos != 0:
             if self.ipv6 is True:
                 self.pg_set(dev, "traffic_class %x" % self.tos)
             else:
                 self.pg_set(dev, "tos %s" % self.tos)
 
+    def __config_vlan(self, dev) -> None:
+        """config vlan related parameter """
+        if self.vlan is not None and 0 <= int(self.vlan) < 4096:
+            self.pg_set(dev, "vlan_id %d" % int(self.vlan))
+        if self.svlan is not None and 0 <= int(self.svlan) < 4096:
+            self.pg_set(dev, "svlan_id %d" % int(self.svlan))
+
     def __config_udp_portrange(self, dev) -> None:
         """config udp port range """
         if self.dst_port_max is not None:
             # Single destination port or random port range
             self.pg_set(dev, "flag UDPDST_RND")
             self.pg_set(dev, "udp_dst_min %d" % (self.dst_port_min))
             self.pg_set(dev, "udp_dst_max %d" % (self.dst_port_max))
@@ -247,15 +257,15 @@
             # Add remove all other devices and add_device $dev to thread
             if self.append is False:
                 self.pg_thread(i, "rem_device_all")
             self.pg_thread(i, "add_device %s" % dev)
 
             # select queue and bind the queue and $dev in 1:1 relationship
             if self.queue is True:
-                qid = (i - self.first_thread)
+                qid = i - self.first_thread
                 if self.debug is True:
                     print("queue number is %d" % (qid))
                 self.pg_set(dev, "queue_map_min %d" % qid)
                 self.pg_set(dev, "queue_map_max %d" % qid)
 
             # Notice config queue to map to cpu (mirrors smp_processor_id())
             # It is beneficial to map IRQ /proc/irq/*/smp_affinity 1:1 to CPU
@@ -280,14 +290,15 @@
                 self.pg_set(dev, "dst_min6 %s" % (self.dst_ip_min))
                 self.pg_set(dev, "dst_max6 %s" % (self.dst_ip_max))
             else:
                 self.pg_set(dev, "dst_min %s" % (self.dst_ip_min))
                 self.pg_set(dev, "dst_max %s" % (self.dst_ip_max))
 
             self.__config_udp_portrange(dev)
+            self.__config_vlan(dev)
 
             # hw burst
             if self.burst is not None and self.burst > 0:
                 self.pg_set(dev, "burst %d" % self.burst)
 
             # rate limit
             if self.bps_rate is not None:
```

### Comparing `pktperf-0.4.0/pktperf/pktsar.py` & `pktperf-0.4.1/pktperf/pktsar.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,35 @@
+# -*- coding: UTF-8 -*-
 """
 classes provide for stats update
 """
 from __future__ import division
 
 
 class PktSar:
     """pkt sar stats class
 
     calculate the pps and bps from the text
     """
+
     def __init__(self, start_time: int, pkt_size: int) -> None:
         """ init sar stats """
         self.start = start_time
         self._pkts = 0
         self._pkt_size = pkt_size
         self._bytes = 0
         self.last_update = start_time
         self.pps = 0.0
         self.bps = 0.0
 
     def update(self, pkts_so_far, timestamp):
         """ update stats """
         diff_pkts = pkts_so_far - self._pkts
         self._pkts = pkts_so_far
-        diff_time = ((timestamp - self.last_update)/1000000)
+        diff_time = (timestamp - self.last_update) / 1000000
         if diff_time != 0:
             self.last_update = timestamp
             if timestamp == self.start:
                 self.pps = 0.0
                 self.bps = 0.0
             else:
                 self.pps = diff_pkts / diff_time
```

### Comparing `pktperf-0.4.0/pktperf.egg-info/PKG-INFO` & `pktperf-0.4.1/pktperf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pktperf
-Version: 0.4.0
+Version: 0.4.1
 Summary: pktgen python scripts
 Author: junka
 Author-email: wan.junjie@fixmail.com
 Project-URL: Bug Tracker, https://github.com/junka/pktperf/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.5
```

### Comparing `pktperf-0.4.0/setup.py` & `pktperf-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pktperf',
-    version="0.4.0",
+    version="0.4.1",
     description="pktgen python scripts",
     author="junka",
     author_email="wan.junjie@fixmail.com",
     packages=["pktperf"],
     package_dir={'pktperf': 'pktperf/'},
     entry_points={'console_scripts': [
         'pktperf=pktperf.pktperf:main',
```

