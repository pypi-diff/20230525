# Comparing `tmp/finsy-0.8.0.tar.gz` & `tmp/finsy-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finsy-0.8.0.tar", max compression
+gzip compressed data, was "finsy-0.9.0.tar", max compression
```

## Comparing `finsy-0.8.0.tar` & `finsy-0.9.0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
--rw-r--r--   0        0        0    11341 2022-11-01 03:46:15.721255 finsy-0.8.0/LICENSE.txt
--rw-r--r--   0        0        0     2829 2022-11-01 03:46:15.721255 finsy-0.8.0/README.md
--rw-r--r--   0        0        0     2198 2022-11-01 03:46:15.725255 finsy-0.8.0/finsy/__init__.py
--rw-r--r--   0        0        0     6993 2022-11-01 03:46:15.725255 finsy-0.8.0/finsy/controller.py
--rw-r--r--   0        0        0     3004 2022-11-01 03:46:15.725255 finsy-0.8.0/finsy/futures.py
--rw-r--r--   0        0        0    14619 2022-11-01 03:46:15.725255 finsy-0.8.0/finsy/gnmiclient.py
--rw-r--r--   0        0        0     8018 2022-11-01 03:46:15.725255 finsy-0.8.0/finsy/gnmipath.py
--rw-r--r--   0        0        0     4332 2022-11-01 03:46:15.725255 finsy-0.8.0/finsy/gnmistring.py
--rw-r--r--   0        0        0     4038 2022-11-01 03:46:15.725255 finsy-0.8.0/finsy/grpcutil.py
--rw-r--r--   0        0        0     2981 2022-11-01 03:46:15.725255 finsy-0.8.0/finsy/log.py
--rw-r--r--   0        0        0     8153 2022-11-01 03:46:15.725255 finsy-0.8.0/finsy/p4arbitrator.py
--rw-r--r--   0        0        0    12545 2022-11-01 03:46:15.725255 finsy-0.8.0/finsy/p4client.py
--rw-r--r--   0        0        0    47567 2022-11-01 03:46:15.725255 finsy-0.8.0/finsy/p4entity.py
--rw-r--r--   0        0        0    66527 2022-11-01 03:46:15.725255 finsy-0.8.0/finsy/p4schema.py
--rw-r--r--   0        0        0    16169 2022-11-01 03:46:15.725255 finsy-0.8.0/finsy/p4values.py
--rw-r--r--   0        0        0     7431 2022-11-01 03:46:15.725255 finsy-0.8.0/finsy/pbuf.py
--rw-r--r--   0        0        0     4181 2022-11-01 03:46:15.725255 finsy-0.8.0/finsy/ports.py
--rw-r--r--   0        0        0     2608 2022-11-01 03:46:15.725255 finsy-0.8.0/finsy/proto/__init__.py
--rw-r--r--   0        0        0        0 2022-11-01 03:46:15.725255 finsy-0.8.0/finsy/proto/gnmi1/__init__.py
--rw-r--r--   0        0        0    21350 2022-11-01 03:46:15.725255 finsy-0.8.0/finsy/proto/gnmi1/gnmi.proto
--rw-r--r--   0        0        0     3186 2022-11-01 03:46:15.725255 finsy-0.8.0/finsy/proto/gnmi1/gnmi_ext.proto
--rw-r--r--   0        0        0     2572 2022-11-01 03:46:15.725255 finsy-0.8.0/finsy/proto/gnmi1/gnmi_ext_pb2.py
--rw-r--r--   0        0        0     8305 2022-11-01 03:46:15.725255 finsy-0.8.0/finsy/proto/gnmi1/gnmi_ext_pb2.pyi
--rw-r--r--   0        0        0    11952 2022-11-01 03:46:15.725255 finsy-0.8.0/finsy/proto/gnmi1/gnmi_pb2.py
--rw-r--r--   0        0        0    47153 2022-11-01 03:46:15.725255 finsy-0.8.0/finsy/proto/gnmi1/gnmi_pb2.pyi
--rw-r--r--   0        0        0     8011 2022-11-01 03:46:15.725255 finsy-0.8.0/finsy/proto/gnmi1/gnmi_pb2_grpc.py
--rw-r--r--   0        0        0     4768 2022-11-01 03:46:15.725255 finsy-0.8.0/finsy/proto/gnmi1/gnmi_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2022-11-01 03:46:15.725255 finsy-0.8.0/finsy/proto/google/rpc/__init__.py
--rw-r--r--   0        0        0     7125 2022-11-01 03:46:15.725255 finsy-0.8.0/finsy/proto/google/rpc/code.proto
--rw-r--r--   0        0        0     1772 2022-11-01 03:46:15.725255 finsy-0.8.0/finsy/proto/google/rpc/code_pb2.py
--rw-r--r--   0        0        0    13544 2022-11-01 03:46:15.725255 finsy-0.8.0/finsy/proto/google/rpc/code_pb2.pyi
--rw-r--r--   0        0        0        0 2022-11-01 03:46:15.725255 finsy-0.8.0/finsy/proto/google/rpc/context/__init__.py
--rw-r--r--   0        0        0    12015 2022-11-01 03:46:15.725255 finsy-0.8.0/finsy/proto/google/rpc/context/attribute_context.proto
--rw-r--r--   0        0        0     5999 2022-11-01 03:46:15.725255 finsy-0.8.0/finsy/proto/google/rpc/context/attribute_context_pb2.py
--rw-r--r--   0        0        0    23920 2022-11-01 03:46:15.725255 finsy-0.8.0/finsy/proto/google/rpc/context/attribute_context_pb2.pyi
--rw-r--r--   0        0        0     9504 2022-11-01 03:46:15.725255 finsy-0.8.0/finsy/proto/google/rpc/error_details.proto
--rw-r--r--   0        0        0     4296 2022-11-01 03:46:15.725255 finsy-0.8.0/finsy/proto/google/rpc/error_details_pb2.py
--rw-r--r--   0        0        0    18622 2022-11-01 03:46:15.729255 finsy-0.8.0/finsy/proto/google/rpc/error_details_pb2.pyi
--rw-r--r--   0        0        0     1924 2022-11-01 03:46:15.729255 finsy-0.8.0/finsy/proto/google/rpc/status.proto
--rw-r--r--   0        0        0     1479 2022-11-01 03:46:15.729255 finsy-0.8.0/finsy/proto/google/rpc/status_pb2.py
--rw-r--r--   0        0        0     2726 2022-11-01 03:46:15.729255 finsy-0.8.0/finsy/proto/google/rpc/status_pb2.pyi
--rw-r--r--   0        0        0        0 2022-11-01 03:46:15.729255 finsy-0.8.0/finsy/proto/p4/__init__.py
--rw-r--r--   0        0        0        0 2022-11-01 03:46:15.729255 finsy-0.8.0/finsy/proto/p4/config/__init__.py
--rw-r--r--   0        0        0        0 2022-11-01 03:46:15.729255 finsy-0.8.0/finsy/proto/p4/config/v1/__init__.py
--rw-r--r--   0        0        0    13657 2022-11-01 03:46:15.729255 finsy-0.8.0/finsy/proto/p4/config/v1/p4info.proto
--rw-r--r--   0        0        0    12623 2022-11-01 03:46:15.729255 finsy-0.8.0/finsy/proto/p4/config/v1/p4info_pb2.py
--rw-r--r--   0        0        0    50784 2022-11-01 03:46:15.729255 finsy-0.8.0/finsy/proto/p4/config/v1/p4info_pb2.pyi
--rw-r--r--   0        0        0     9876 2022-11-01 03:46:15.729255 finsy-0.8.0/finsy/proto/p4/config/v1/p4types.proto
--rw-r--r--   0        0        0    13219 2022-11-01 03:46:15.729255 finsy-0.8.0/finsy/proto/p4/config/v1/p4types_pb2.py
--rw-r--r--   0        0        0    45500 2022-11-01 03:46:15.729255 finsy-0.8.0/finsy/proto/p4/config/v1/p4types_pb2.pyi
--rw-r--r--   0        0        0        0 2022-11-01 03:46:15.729255 finsy-0.8.0/finsy/proto/p4/v1/__init__.py
--rw-r--r--   0        0        0     2161 2022-11-01 03:46:15.729255 finsy-0.8.0/finsy/proto/p4/v1/p4data.proto
--rw-r--r--   0        0        0     2799 2022-11-01 03:46:15.729255 finsy-0.8.0/finsy/proto/p4/v1/p4data_pb2.py
--rw-r--r--   0        0        0     8495 2022-11-01 03:46:15.729255 finsy-0.8.0/finsy/proto/p4/v1/p4data_pb2.pyi
--rw-r--r--   0        0        0    30522 2022-11-01 03:46:15.729255 finsy-0.8.0/finsy/proto/p4/v1/p4runtime.proto
--rw-r--r--   0        0        0    22190 2022-11-01 03:46:15.729255 finsy-0.8.0/finsy/proto/p4/v1/p4runtime_pb2.py
--rw-r--r--   0        0        0    90205 2022-11-01 03:46:15.729255 finsy-0.8.0/finsy/proto/p4/v1/p4runtime_pb2.pyi
--rw-r--r--   0        0        0    11550 2022-11-01 03:46:15.729255 finsy-0.8.0/finsy/proto/p4/v1/p4runtime_pb2_grpc.py
--rw-r--r--   0        0        0     4506 2022-11-01 03:46:15.729255 finsy-0.8.0/finsy/proto/p4/v1/p4runtime_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2022-11-01 03:46:15.729255 finsy-0.8.0/finsy/proto/stratum1/__init__.py
--rw-r--r--   0        0        0     1451 2022-11-01 03:46:15.729255 finsy-0.8.0/finsy/proto/stratum1/p4_role_config.proto
--rw-r--r--   0        0        0     1533 2022-11-01 03:46:15.729255 finsy-0.8.0/finsy/proto/stratum1/p4_role_config_pb2.py
--rw-r--r--   0        0        0     3750 2022-11-01 03:46:15.729255 finsy-0.8.0/finsy/proto/stratum1/p4_role_config_pb2.pyi
--rw-r--r--   0        0        0    33738 2022-11-01 03:46:15.729255 finsy-0.8.0/finsy/switch.py
--rw-r--r--   0        0        0     9461 2022-11-01 03:46:15.729255 finsy-0.8.0/finsy/test/gnmi_server.py
--rw-r--r--   0        0        0     6068 2022-11-01 03:46:15.729255 finsy-0.8.0/finsy/test/p4runtime_server.py
--rw-r--r--   0        0        0     3129 2022-11-01 03:46:15.729255 finsy-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     3916 1970-01-01 00:00:00.000000 finsy-0.8.0/setup.py
--rw-r--r--   0        0        0     3846 1970-01-01 00:00:00.000000 finsy-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11341 2022-11-10 20:05:27.685813 finsy-0.9.0/LICENSE.txt
+-rw-r--r--   0        0        0     2982 2022-11-10 20:05:27.685813 finsy-0.9.0/README.md
+-rw-r--r--   0        0        0     2450 2022-11-10 20:05:27.689813 finsy-0.9.0/finsy/__init__.py
+-rw-r--r--   0        0        0     7016 2022-11-10 20:05:27.689813 finsy-0.9.0/finsy/controller.py
+-rw-r--r--   0        0        0     3004 2022-11-10 20:05:27.689813 finsy-0.9.0/finsy/futures.py
+-rw-r--r--   0        0        0    15364 2022-11-10 20:05:27.689813 finsy-0.9.0/finsy/gnmiclient.py
+-rw-r--r--   0        0        0     8058 2022-11-10 20:05:27.689813 finsy-0.9.0/finsy/gnmipath.py
+-rw-r--r--   0        0        0     4651 2022-11-10 20:05:27.689813 finsy-0.9.0/finsy/gnmistring.py
+-rw-r--r--   0        0        0     4038 2022-11-10 20:05:27.689813 finsy-0.9.0/finsy/grpcutil.py
+-rw-r--r--   0        0        0     3078 2022-11-10 20:05:27.689813 finsy-0.9.0/finsy/log.py
+-rw-r--r--   0        0        0     8195 2022-11-10 20:05:27.689813 finsy-0.9.0/finsy/p4arbitrator.py
+-rw-r--r--   0        0        0    12633 2022-11-10 20:05:27.689813 finsy-0.9.0/finsy/p4client.py
+-rw-r--r--   0        0        0    47567 2022-11-10 20:05:27.689813 finsy-0.9.0/finsy/p4entity.py
+-rw-r--r--   0        0        0    66593 2022-11-10 20:05:27.689813 finsy-0.9.0/finsy/p4schema.py
+-rw-r--r--   0        0        0    16169 2022-11-10 20:05:27.693813 finsy-0.9.0/finsy/p4values.py
+-rw-r--r--   0        0        0     7431 2022-11-10 20:05:27.693813 finsy-0.9.0/finsy/pbuf.py
+-rw-r--r--   0        0        0     4217 2022-11-10 20:05:27.693813 finsy-0.9.0/finsy/ports.py
+-rw-r--r--   0        0        0     2578 2022-11-10 20:05:27.693813 finsy-0.9.0/finsy/proto/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-10 20:05:27.693813 finsy-0.9.0/finsy/proto/gnmi1/__init__.py
+-rw-r--r--   0        0        0    21350 2022-11-10 20:05:27.693813 finsy-0.9.0/finsy/proto/gnmi1/gnmi.proto
+-rw-r--r--   0        0        0     3186 2022-11-10 20:05:27.693813 finsy-0.9.0/finsy/proto/gnmi1/gnmi_ext.proto
+-rw-r--r--   0        0        0     2572 2022-11-10 20:05:27.693813 finsy-0.9.0/finsy/proto/gnmi1/gnmi_ext_pb2.py
+-rw-r--r--   0        0        0     8305 2022-11-10 20:05:27.693813 finsy-0.9.0/finsy/proto/gnmi1/gnmi_ext_pb2.pyi
+-rw-r--r--   0        0        0    11952 2022-11-10 20:05:27.693813 finsy-0.9.0/finsy/proto/gnmi1/gnmi_pb2.py
+-rw-r--r--   0        0        0    47153 2022-11-10 20:05:27.693813 finsy-0.9.0/finsy/proto/gnmi1/gnmi_pb2.pyi
+-rw-r--r--   0        0        0     8011 2022-11-10 20:05:27.693813 finsy-0.9.0/finsy/proto/gnmi1/gnmi_pb2_grpc.py
+-rw-r--r--   0        0        0     4768 2022-11-10 20:05:27.693813 finsy-0.9.0/finsy/proto/gnmi1/gnmi_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2022-11-10 20:05:27.693813 finsy-0.9.0/finsy/proto/google/rpc/__init__.py
+-rw-r--r--   0        0        0     7125 2022-11-10 20:05:27.693813 finsy-0.9.0/finsy/proto/google/rpc/code.proto
+-rw-r--r--   0        0        0     1772 2022-11-10 20:05:27.693813 finsy-0.9.0/finsy/proto/google/rpc/code_pb2.py
+-rw-r--r--   0        0        0    13544 2022-11-10 20:05:27.693813 finsy-0.9.0/finsy/proto/google/rpc/code_pb2.pyi
+-rw-r--r--   0        0        0        0 2022-11-10 20:05:27.693813 finsy-0.9.0/finsy/proto/google/rpc/context/__init__.py
+-rw-r--r--   0        0        0    12015 2022-11-10 20:05:27.693813 finsy-0.9.0/finsy/proto/google/rpc/context/attribute_context.proto
+-rw-r--r--   0        0        0     5999 2022-11-10 20:05:27.693813 finsy-0.9.0/finsy/proto/google/rpc/context/attribute_context_pb2.py
+-rw-r--r--   0        0        0    23920 2022-11-10 20:05:27.693813 finsy-0.9.0/finsy/proto/google/rpc/context/attribute_context_pb2.pyi
+-rw-r--r--   0        0        0     9504 2022-11-10 20:05:27.693813 finsy-0.9.0/finsy/proto/google/rpc/error_details.proto
+-rw-r--r--   0        0        0     4296 2022-11-10 20:05:27.693813 finsy-0.9.0/finsy/proto/google/rpc/error_details_pb2.py
+-rw-r--r--   0        0        0    18622 2022-11-10 20:05:27.693813 finsy-0.9.0/finsy/proto/google/rpc/error_details_pb2.pyi
+-rw-r--r--   0        0        0     1924 2022-11-10 20:05:27.693813 finsy-0.9.0/finsy/proto/google/rpc/status.proto
+-rw-r--r--   0        0        0     1479 2022-11-10 20:05:27.693813 finsy-0.9.0/finsy/proto/google/rpc/status_pb2.py
+-rw-r--r--   0        0        0     2726 2022-11-10 20:05:27.693813 finsy-0.9.0/finsy/proto/google/rpc/status_pb2.pyi
+-rw-r--r--   0        0        0        0 2022-11-10 20:05:27.693813 finsy-0.9.0/finsy/proto/p4/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-10 20:05:27.693813 finsy-0.9.0/finsy/proto/p4/config/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-10 20:05:27.693813 finsy-0.9.0/finsy/proto/p4/config/v1/__init__.py
+-rw-r--r--   0        0        0    13657 2022-11-10 20:05:27.693813 finsy-0.9.0/finsy/proto/p4/config/v1/p4info.proto
+-rw-r--r--   0        0        0    12623 2022-11-10 20:05:27.693813 finsy-0.9.0/finsy/proto/p4/config/v1/p4info_pb2.py
+-rw-r--r--   0        0        0    50784 2022-11-10 20:05:27.693813 finsy-0.9.0/finsy/proto/p4/config/v1/p4info_pb2.pyi
+-rw-r--r--   0        0        0     9876 2022-11-10 20:05:27.693813 finsy-0.9.0/finsy/proto/p4/config/v1/p4types.proto
+-rw-r--r--   0        0        0    13219 2022-11-10 20:05:27.693813 finsy-0.9.0/finsy/proto/p4/config/v1/p4types_pb2.py
+-rw-r--r--   0        0        0    45500 2022-11-10 20:05:27.693813 finsy-0.9.0/finsy/proto/p4/config/v1/p4types_pb2.pyi
+-rw-r--r--   0        0        0        0 2022-11-10 20:05:27.693813 finsy-0.9.0/finsy/proto/p4/v1/__init__.py
+-rw-r--r--   0        0        0     2161 2022-11-10 20:05:27.693813 finsy-0.9.0/finsy/proto/p4/v1/p4data.proto
+-rw-r--r--   0        0        0     2799 2022-11-10 20:05:27.693813 finsy-0.9.0/finsy/proto/p4/v1/p4data_pb2.py
+-rw-r--r--   0        0        0     8495 2022-11-10 20:05:27.693813 finsy-0.9.0/finsy/proto/p4/v1/p4data_pb2.pyi
+-rw-r--r--   0        0        0    30522 2022-11-10 20:05:27.693813 finsy-0.9.0/finsy/proto/p4/v1/p4runtime.proto
+-rw-r--r--   0        0        0    22190 2022-11-10 20:05:27.693813 finsy-0.9.0/finsy/proto/p4/v1/p4runtime_pb2.py
+-rw-r--r--   0        0        0    90205 2022-11-10 20:05:27.693813 finsy-0.9.0/finsy/proto/p4/v1/p4runtime_pb2.pyi
+-rw-r--r--   0        0        0    11550 2022-11-10 20:05:27.693813 finsy-0.9.0/finsy/proto/p4/v1/p4runtime_pb2_grpc.py
+-rw-r--r--   0        0        0     4506 2022-11-10 20:05:27.693813 finsy-0.9.0/finsy/proto/p4/v1/p4runtime_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2022-11-10 20:05:27.693813 finsy-0.9.0/finsy/proto/stratum1/__init__.py
+-rw-r--r--   0        0        0     1451 2022-11-10 20:05:27.693813 finsy-0.9.0/finsy/proto/stratum1/p4_role_config.proto
+-rw-r--r--   0        0        0     1533 2022-11-10 20:05:27.693813 finsy-0.9.0/finsy/proto/stratum1/p4_role_config_pb2.py
+-rw-r--r--   0        0        0     3750 2022-11-10 20:05:27.693813 finsy-0.9.0/finsy/proto/stratum1/p4_role_config_pb2.pyi
+-rw-r--r--   0        0        0    33675 2022-11-10 20:05:27.697813 finsy-0.9.0/finsy/switch.py
+-rw-r--r--   0        0        0     9462 2022-11-10 20:05:27.697813 finsy-0.9.0/finsy/test/gnmi_server.py
+-rw-r--r--   0        0        0     6135 2022-11-10 20:05:27.697813 finsy-0.9.0/finsy/test/p4runtime_server.py
+-rw-r--r--   0        0        0     2893 2022-11-10 20:05:27.697813 finsy-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     4073 1970-01-01 00:00:00.000000 finsy-0.9.0/setup.py
+-rw-r--r--   0        0        0     3999 1970-01-01 00:00:00.000000 finsy-0.9.0/PKG-INFO
```

### Comparing `finsy-0.8.0/LICENSE.txt` & `finsy-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `finsy-0.8.0/README.md` & `finsy-0.9.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 # 🐟 Finsy P4Runtime Library
 
-[![pypi](https://img.shields.io/pypi/v/finsy)](https://pypi.org/project/finsy/) [![ci](https://github.com/byllyfish/finsy/actions/workflows/ci.yml/badge.svg)](https://github.com/byllyfish/finsy/actions/workflows/ci.yml) [![codecov](https://codecov.io/gh/byllyfish/finsy/branch/main/graph/badge.svg?token=8RPYWRXNGS)](https://codecov.io/gh/byllyfish/finsy)
+[![pypi](https://img.shields.io/pypi/v/finsy)](https://pypi.org/project/finsy/) [![ci](https://github.com/byllyfish/finsy/actions/workflows/ci.yml/badge.svg)](https://github.com/byllyfish/finsy/actions/workflows/ci.yml) [![codecov](https://codecov.io/gh/byllyfish/finsy/branch/main/graph/badge.svg?token=8RPYWRXNGS)](https://codecov.io/gh/byllyfish/finsy) [![docs](https://img.shields.io/badge/-docs-informational)](https://byllyfish.github.io/finsy/finsy.html)
 
 Finsy is a [P4Runtime](https://p4.org/p4-spec/p4runtime/main/P4Runtime-Spec.html) controller library written in Python using asyncio. Finsy includes support for [gNMI](https://github.com/openconfig/reference/blob/master/rpc/gnmi/gnmi-specification.md).
 
 ```python
 import asyncio
 import finsy as fy
 
 async def main():
     async with fy.Switch("sw1", "127.0.0.1:50001") as sw1:
         print(sw1.p4info)
 
 asyncio.run(main())
 ```
 
-## Multiple Switches
+## Requirements
+
+Finsy requires Python 3.10 or later.
+
+## P4Runtime Controller
 
 With Finsy, you can write a P4Runtime controller that manages multiple switches.
 
 Each switch is managed by an async `ready_handler` function. Your `ready_handler` function can read or 
 update various P4Runtime entities in the switch. It can also create tasks to listen for 
 packets or digests.
 
 When you write P4Runtime updates to the switch, you use a unary operator (+, -, \~) to specify the operation:
 INSERT (+), DELETE (-) or MODIFY (\~).
 
 ```python
-async def ready_handler(sw: fy.Switch):
+async def ready_handler(sw):
     await sw.delete_all()
     await sw.write(
         [
             # Insert multicast group with ports 1, 2, 3 and CONTROLLER.
             +fy.P4MulticastGroupEntry(1, replicas=[1, 2, 3, 255]),
             # Modify default table entry to flood all unmatched packets.
             ~fy.P4TableEntry(
```

### Comparing `finsy-0.8.0/finsy/__init__.py` & `finsy-0.9.0/finsy/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,25 +10,27 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.8.0"
+__version__ = "0.9.0"
 
 import sys
 
 if sys.version_info < (3, 10):  # pragma: no cover
     raise RuntimeError("Requires Python 3.10+.")
 
 from .controller import Controller, current_controller
-from .gnmiclient import gNMIClient, gNMISubscription, gNMIUpdate
-from .gnmipath import gNMIPath
+from .gnmiclient import GNMIClient, GNMISubscription, GNMIUpdate
+from .gnmipath import GNMIPath
+from .grpcutil import GRPCStatusCode
 from .log import LoggerAdapter
+from .p4client import P4Client, P4ClientError, P4Error
 from .p4entity import (
     P4ActionProfileGroup,
     P4ActionProfileMember,
     P4CloneSessionEntry,
     P4CounterData,
     P4CounterEntry,
     P4DigestEntry,
@@ -43,30 +45,34 @@
     P4PacketOut,
     P4RegisterEntry,
     P4TableAction,
     P4TableEntry,
     P4TableMatch,
 )
 from .p4schema import P4ConfigAction, P4CounterUnit, P4Schema
+from .ports import SwitchPort, SwitchPortList
 from .switch import Switch, SwitchEvent, SwitchOptions
 
 __all__ = [
     "current_controller",
     "Controller",
     "LoggerAdapter",
     "P4ActionProfileGroup",
     "P4ActionProfileMember",
+    "P4Client",
+    "P4ClientError",
     "P4CloneSessionEntry",
     "P4CounterData",
     "P4CounterEntry",
     "P4CounterUnit",
     "P4DigestEntry",
     "P4DigestList",
     "P4DigestListAck",
     "P4DirectCounterEntry",
+    "P4Error",
     "P4IndirectAction",
     "P4MeterConfig",
     "P4MeterCounterData",
     "P4MulticastGroupEntry",
     "P4PacketIn",
     "P4PacketOut",
     "P4RegisterEntry",
@@ -74,12 +80,15 @@
     "P4TableEntry",
     "P4TableMatch",
     "P4ConfigAction",
     "P4Schema",
     "Switch",
     "SwitchEvent",
     "SwitchOptions",
-    "gNMIClient",
-    "gNMIPath",
-    "gNMISubscription",
-    "gNMIUpdate",
+    "SwitchPort",
+    "SwitchPortList",
+    "GNMIClient",
+    "GNMIPath",
+    "GNMISubscription",
+    "GNMIUpdate",
+    "GRPCStatusCode",
 ]
```

### Comparing `finsy-0.8.0/finsy/controller.py` & `finsy-0.9.0/finsy/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     _switches: dict[str, Switch]
     _removed: set[Switch]
     _task_count: CountdownFuture
 
     control_task: asyncio.Task[Any] | None = None
     "Keep track of controller's main task."
 
-    def __init__(self, switches: Iterable[Switch], *, name="controller"):
+    def __init__(self, switches: Iterable[Switch], *, name: str = "controller"):
         self._name = name
         self._switches = {}
         self._removed = set()
         self._task_count = CountdownFuture()
 
         for switch in switches:
             if switch.name in self._switches:
@@ -157,15 +157,15 @@
             raise ValueError(f"Switch named {name!r} not found")
 
         del self._switches[name]
 
         if self.running:
             self._stop_switch(switch)
             self._removed.add(switch)
-            switch.ee.once(SwitchEvent.CONTROLLER_LEAVE, self._removed.discard)
+            switch.ee.once(SwitchEvent.CONTROLLER_LEAVE, self._removed.discard)  # type: ignore
 
     def _start_switch(self, switch: Switch):
         "Start the switch's control task."
         LOGGER.debug("Controller._start_switch: %r", switch)
         assert switch.control_task is None
 
         switch.ee.emit(SwitchEvent.CONTROLLER_ENTER, switch)
```

### Comparing `finsy-0.8.0/finsy/futures.py` & `finsy-0.9.0/finsy/futures.py`

 * *Files identical despite different names*

### Comparing `finsy-0.8.0/finsy/gnmiclient.py` & `finsy-0.9.0/finsy/gnmiclient.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"Implements the gNMIClient class."
+"Implements the GNMIClient class."
 
 # Copyright (c) 2022 Bill Fisher
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -19,57 +19,53 @@
 import asyncio
 from dataclasses import dataclass
 from typing import Any, AsyncIterator, Iterator, Sequence, TypeAlias
 
 import grpc  # pyright: ignore[reportMissingTypeStubs]
 
 from finsy import pbuf
-from finsy.gnmipath import gNMIPath
+from finsy.gnmipath import GNMIPath
 from finsy.grpcutil import GRPC_EOF, GRPCStatusCode, grpc_channel
 from finsy.log import LOGGER
 from finsy.proto import gnmi, gnmi_grpc
 
 
-class gNMIClientError(Exception):
+class GNMIClientError(Exception):
     "Represents a `grpc.RpcError`."
 
     _code: GRPCStatusCode
     _message: str
 
     def __init__(self, error: grpc.RpcError):
         super().__init__()
         assert isinstance(error, grpc.aio.AioRpcError)
 
         self._code = GRPCStatusCode.from_status_code(error.code())
         self._message = error.details() or ""
 
-        LOGGER.debug("gNMI failed: %s", self)
+        LOGGER.debug("GNMI failed: %s", self)
 
     @property
     def code(self):
         return self._code
 
     @property
     def message(self):
         return self._message
 
-    @property
-    def is_unimplemented(self):
-        return self.code == GRPCStatusCode.UNIMPLEMENTED
-
     def __str__(self) -> str:
-        return f"gNMIClientError(code={self.code!r}, message={self.message!r})"
+        return f"GNMIClientError(code={self.code!r}, message={self.message!r})"
 
 
 @dataclass
-class gNMIUpdate:
-    "Represents a gNMI update returned from gNMIClient."
+class GNMIUpdate:
+    "Represents a gNMI update returned from GNMIClient."
 
     timestamp: int
-    path: gNMIPath
+    path: GNMIPath
     typed_value: gnmi.TypedValue | None
 
     @property
     def value(self) -> Any:
         "Return the value as a Python value."
         if self.typed_value is None:
             return None
@@ -79,50 +75,82 @@
             raise ValueError("typed_value is not set")
         return getattr(self.typed_value, attr)
 
     def __repr__(self):
         "Override repr to strip newline from end of `TypedValue`."
 
         value = repr(self.typed_value).rstrip()
-        return f"gNMIUpdate(timestamp={self.timestamp!r}, path={self.path!r}, typed_value=`{value}`)"
+        return f"GNMIUpdate(timestamp={self.timestamp!r}, path={self.path!r}, typed_value=`{value}`)"
+
+
+GNMISetValueType = bool | int | float | str | bytes | gnmi.TypedValue
+
+
+def gnmi_update(
+    path: GNMIPath,
+    value: GNMISetValueType,
+) -> gnmi.Update:
+    "Construct a `gnmi.Update` message from path and value."
+
+    match value:
+        case gnmi.TypedValue():
+            val = value
+        case bool():
+            val = gnmi.TypedValue(bool_val=value)
+        case int():
+            # Use uint_val if value is non-negative?
+            if value >= 0:
+                val = gnmi.TypedValue(uint_val=value)
+            else:
+                val = gnmi.TypedValue(int_val=value)
+        case float():
+            val = gnmi.TypedValue(double_val=value)
+        case str():
+            val = gnmi.TypedValue(string_val=value)
+        case bytes():
+            val = gnmi.TypedValue(bytes_val=value)
+        case _:
+            raise TypeError(f"unexpected type: {type(value).__name__}")
+
+    return gnmi.Update(path=path.path, val=val)
 
 
-class gNMIClient:
+class GNMIClient:
     """Async GNMI client.
 
     This client implements `get`, `set`, `subscribe` and `capabilities`.
 
     The API depends on the protobuf definition of `gnmi.TypedValue`.
 
     Get usage:
     ```
-    client = gNMIClient('127.0.0.1:9339')
+    client = GNMIClient('127.0.0.1:9339')
     await client.open()
 
-    path = gNMIPath("interfaces/interface")
+    path = GNMIPath("interfaces/interface")
     async for update in client.get(path):
         print(update)
     ```
 
     Subscribe usage:
     ```
-    path = gNMIPath("interfaces/interface[name=eth1]/state/oper-status")
+    path = GNMIPath("interfaces/interface[name=eth1]/state/oper-status")
     sub = client.subscribe()
     sub.on_change(path)
 
     async for initial_state in sub.synchronize():
         print(initial_state)
 
     async for update in sub.updates():
         print(update)
     ```
 
     Set usage:
     ```
-    enabled = gNMIPath("interfaces/interface[name=eth1]/config/enabled")
+    enabled = GNMIPath("interfaces/interface[name=eth1]/config/enabled")
 
     await client.set(update={
         enabled: gnmi.TypedValue(boolValue=True),
     })
     ```
     """
 
@@ -153,50 +181,50 @@
         channel: grpc.aio.Channel | None = None,
     ) -> None:
         """Open the client channel.
 
         Note: This method is `async` for forward-compatible reasons.
         """
         if self._channel is not None:
-            raise RuntimeError("gNMIClient: client is already open")
+            raise RuntimeError("GNMIClient: client is already open")
 
         assert self._stub is None
 
         if channel is not None:
             self._channel = channel
             self._channel_reused = True
         else:
             self._channel = grpc_channel(
                 self._address,
                 credentials=self._credentials,
-                client_type="gNMIClient",
+                client_type="GNMIClient",
             )
 
         self._stub = gnmi_grpc.gNMIStub(self._channel)  # type: ignore
 
     async def close(self) -> None:
         "Close the client channel."
         if self._channel is not None:
             if not self._channel_reused:
-                LOGGER.debug("gNMIClient: close channel %r", self._address)
+                LOGGER.debug("GNMIClient: close channel %r", self._address)
                 await self._channel.close()
 
             self._channel = None
             self._stub = None
             self._channel_reused = False
 
     async def get(
         self,
-        *path: gNMIPath,
-        prefix: gNMIPath | None = None,
+        *path: GNMIPath,
+        prefix: GNMIPath | None = None,
         config: bool = False,
-    ) -> Sequence[gNMIUpdate]:
+    ) -> Sequence[GNMIUpdate]:
         "Retrieve value(s) using a GetRequest."
         if self._stub is None:
-            raise RuntimeError("gNMIClient: client is not open")
+            raise RuntimeError("GNMIClient: client is not open")
 
         request = gnmi.GetRequest(
             path=(i.path for i in path),
             encoding=gnmi.Encoding.PROTO,
         )
 
         if prefix is not None:
@@ -205,30 +233,30 @@
         if config:
             request.type = gnmi.GetRequest.CONFIG
 
         self._log_msg(request)
         try:
             reply: gnmi.GetResponse = await self._stub.Get(request)
         except grpc.RpcError as ex:
-            raise gNMIClientError(ex) from None
+            raise GNMIClientError(ex) from None
 
         self._log_msg(reply)
 
-        result: list[gNMIUpdate] = []
+        result: list[GNMIUpdate] = []
         for notification in reply.notification:
             for update in _read_updates(notification):
                 result.append(update)
 
         return result
 
     def subscribe(
         self,
         *,
-        prefix: gNMIPath | None = None,
-    ) -> "gNMISubscription":
+        prefix: GNMIPath | None = None,
+    ) -> "GNMISubscription":
         """Subscribe to gNMI change notifications.
 
         Usage:
         ```
         sub = client.subscribe()
         sub.on_change(path1, ...)
         sub.sample(path3, path4, sample_interval=1000000000)
@@ -249,61 +277,56 @@
             # do something with info
         ```
 
         The subscription object is not re-entrant, but a fully consumed
         subscription may be reused.
         """
         if self._stub is None:
-            raise RuntimeError("gNMIClient: client is not open")
+            raise RuntimeError("GNMIClient: client is not open")
 
-        return gNMISubscription(self, prefix)
+        return GNMISubscription(self, prefix)
 
     async def capabilities(self) -> gnmi.CapabilityResponse:
         "Issue a CapabilitiesRequest."
         if self._stub is None:
-            raise RuntimeError("gNMIClient: client is not open")
+            raise RuntimeError("GNMIClient: client is not open")
 
         request = gnmi.CapabilityRequest()
 
         self._log_msg(request)
         try:
             reply: gnmi.CapabilityResponse = await self._stub.Capabilities(request)
         except grpc.RpcError as ex:
-            raise gNMIClientError(ex) from None
+            raise GNMIClientError(ex) from None
 
         self._log_msg(reply)
         return reply
 
     async def set(
         self,
         *,
-        update: dict[gNMIPath, gnmi.TypedValue] | None = None,
-        replace: dict[gNMIPath, gnmi.TypedValue] | None = None,
-        delete: Sequence[gNMIPath] | None = None,
-        prefix: gNMIPath | None = None,
+        update: Sequence[tuple[GNMIPath, GNMISetValueType]] | None = None,
+        replace: Sequence[tuple[GNMIPath, GNMISetValueType]] | None = None,
+        delete: Sequence[GNMIPath] | None = None,
+        prefix: GNMIPath | None = None,
     ) -> int:
         """Set value(s) using SetRequest.
 
         Returns the timestamp from the successful `SetResponse`.
         """
         if self._stub is None:
-            raise RuntimeError("gNMIClient: client is not open")
+            raise RuntimeError("GNMIClient: client is not open")
 
         if update is not None:
-            updates = [
-                gnmi.Update(path=path.path, val=value) for path, value in update.items()
-            ]
+            updates = [gnmi_update(path, value) for path, value in update]
         else:
             updates = None
 
         if replace is not None:
-            replaces = [
-                gnmi.Update(path=path.path, val=value)
-                for path, value in replace.items()
-            ]
+            replaces = [gnmi_update(path, value) for path, value in replace]
         else:
             replaces = None
 
         if delete is not None:
             deletes = [path.path for path in delete]
         else:
             deletes = None
@@ -317,15 +340,15 @@
         if prefix is not None:
             request.prefix.CopyFrom(prefix.path)
 
         self._log_msg(request)
         try:
             reply: gnmi.SetResponse = await self._stub.Set(request)
         except grpc.RpcError as ex:
-            raise gNMIClientError(ex) from None
+            raise GNMIClientError(ex) from None
 
         self._log_msg(reply)
 
         # According to the comments in the current protobuf, I expect all error
         # results to be raised as an exception. The only useful value in a
         # successful response is the timestamp.
 
@@ -344,49 +367,49 @@
 
 
 _StreamTypeAlias: TypeAlias = grpc.aio.StreamStreamCall[
     gnmi.SubscribeRequest, gnmi.SubscribeResponse
 ]
 
 
-class gNMISubscription:
+class GNMISubscription:
     """Represents a gNMI subscription stream."""
 
-    _client: gNMIClient
+    _client: GNMIClient
     _stream: _StreamTypeAlias | None
 
-    def __init__(self, client: gNMIClient, prefix: gNMIPath | None = None):
+    def __init__(self, client: GNMIClient, prefix: GNMIPath | None = None):
         self._client = client
         self._stream = None
         self._sublist = gnmi.SubscriptionList(
             mode=gnmi.SubscriptionList.Mode.STREAM,
         )
         if prefix is not None:
             self._sublist.prefix.CopyFrom(prefix.path)
 
-    def once(self, *paths: gNMIPath):
+    def once(self, *paths: GNMIPath):
         self._sublist.mode = gnmi.SubscriptionList.Mode.ONCE
 
         for path in paths:
             sub = gnmi.Subscription(path=path.path)
             self._sublist.subscription.append(sub)
 
-    def on_change(self, *paths: gNMIPath):
+    def on_change(self, *paths: GNMIPath):
         assert self._sublist.mode == gnmi.SubscriptionList.Mode.STREAM
 
         for path in paths:
             sub = gnmi.Subscription(
                 path=path.path,
                 mode=gnmi.SubscriptionMode.ON_CHANGE,
             )
             self._sublist.subscription.append(sub)
 
     def sample(
         self,
-        *paths: gNMIPath,
+        *paths: GNMIPath,
         sample_interval: int,
         suppress_redundant: bool = False,
         heartbeat_interval: int = 0,
     ):
         assert self._sublist.mode == gnmi.SubscriptionList.Mode.STREAM
 
         for path in paths:
@@ -395,33 +418,33 @@
                 mode=gnmi.SubscriptionMode.SAMPLE,
                 sample_interval=sample_interval,
                 suppress_redundant=suppress_redundant,
                 heartbeat_interval=heartbeat_interval,
             )
             self._sublist.subscription.append(sub)
 
-    async def synchronize(self) -> AsyncIterator[gNMIUpdate]:
+    async def synchronize(self) -> AsyncIterator[GNMIUpdate]:
         if self._stream is None:
             await self._subscribe()
 
         try:
             async for result in self._read(True):
                 yield result
         except grpc.RpcError as ex:
-            raise gNMIClientError(ex) from None
+            raise GNMIClientError(ex) from None
 
-    async def updates(self) -> AsyncIterator[gNMIUpdate]:
+    async def updates(self) -> AsyncIterator[GNMIUpdate]:
         if self._stream is None:
             await self._subscribe()
 
         try:
             async for result in self._read(False):
                 yield result
         except grpc.RpcError as ex:
-            raise gNMIClientError(ex) from None
+            raise GNMIClientError(ex) from None
 
     def cancel(self):
         if self._stream is not None:
             self._stream.cancel()
             self._stream = None
 
     async def _subscribe(self):
@@ -432,17 +455,17 @@
         self._stream = s
         request = gnmi.SubscribeRequest(subscribe=self._sublist)
 
         self._client._log_msg(request)
         try:
             await self._stream.write(request)
         except grpc.RpcError as ex:
-            raise gNMIClientError(ex) from None
+            raise GNMIClientError(ex) from None
 
-    async def _read(self, stop_at_sync: bool) -> AsyncIterator[gNMIUpdate]:
+    async def _read(self, stop_at_sync: bool) -> AsyncIterator[GNMIUpdate]:
         assert self._stream is not None
 
         while True:
             msg = await self._stream.read()
             if msg == GRPC_EOF:
                 LOGGER.warning("gNMI _read: unexpected EOF")
                 return
@@ -468,23 +491,23 @@
                     LOGGER.warning("gNMI _read: unexpected oneof: %s", other)
 
     def _is_once(self) -> bool:
         "Return true if the subscription is in ONCE mode."
         return self._sublist.mode == gnmi.SubscriptionList.Mode.ONCE
 
 
-def _read_updates(notification: gnmi.Notification) -> Iterator[gNMIUpdate]:
+def _read_updates(notification: gnmi.Notification) -> Iterator[GNMIUpdate]:
     "Generator to retrieve all updates from a notification."
 
     for update in notification.update:
-        yield gNMIUpdate(
+        yield GNMIUpdate(
             timestamp=notification.timestamp,
-            path=gNMIPath(update.path),
+            path=GNMIPath(update.path),
             typed_value=update.val,
         )
 
     for delete in notification.delete:
-        yield gNMIUpdate(
+        yield GNMIUpdate(
             timestamp=notification.timestamp,
-            path=gNMIPath(delete),
+            path=GNMIPath(delete),
             typed_value=None,
         )
```

### Comparing `finsy-0.8.0/finsy/gnmipath.py` & `finsy-0.9.0/finsy/gnmipath.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"Implements the gNMIPath class."
+"Implements the GNMIPath class."
 
 # Copyright (c) 2022 Bill Fisher
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -19,36 +19,36 @@
 
 from typing_extensions import Self
 
 from finsy import gnmistring
 from finsy.proto import gnmi
 
 
-class gNMIPath:
+class GNMIPath:
     """Concrete class for working with `gnmi.Path` objects.
 
-    A `gNMIPath` should be treated as an immutable object. You can access
+    A `GNMIPath` should be treated as an immutable object. You can access
     the wrapped `gnmi.Path` protobuf class using the `.path` property.
-    `gNMIPath` objects are hashable, but you must be careful that you do not
+    `GNMIPath` objects are hashable, but you must be careful that you do not
     mutate them via the underlying `gnmi.Path`.
 
-    You can construct a gNMIPath from a string:
+    You can construct a GNMIPath from a string:
     ```
-    path = gNMIPath("interfaces/interface[name=eth1]/state")
+    path = GNMIPath("interfaces/interface[name=eth1]/state")
     ```
 
-    You can construct a gNMIPath object from a `gnmi.Path` directly.
+    You can construct a GNMIPath object from a `gnmi.Path` directly.
     ```
-    path = gNMIPath(update.path)
+    path = GNMIPath(update.path)
     ```
 
     You can create paths by using an existing path as a template, without
     modifying the original path. Use the `set` method:
     ```
-    operStatus = gNMIPath("interfaces/interface/state/oper-status")
+    operStatus = GNMIPath("interfaces/interface/state/oper-status")
     path = operStatus.set("interface", name="eth1")
     ```
 
     Use [] to access the name/key of path elements:
     ```
     path[1] == "interface"
     path["interface", "name"] == "eth1"
@@ -62,15 +62,15 @@
     def __init__(
         self,
         path: gnmi.Path | str = "",
         *,
         origin: str = "",
         target: str = "",
     ):
-        "Construct a `gNMIPath` from a string or `gnmi.Path`."
+        "Construct a `GNMIPath` from a string or `gnmi.Path`."
         if isinstance(path, str):
             path = gnmistring.parse(path)
 
         if origin:
             path.origin = origin
 
         if target:
@@ -95,15 +95,15 @@
 
     @property
     def target(self) -> str:
         "Return the path's target."
         return self.path.target
 
     def set(self, __elem: str | int | None = None, **kwds: Any) -> Self:
-        "Construct a new gNMIPath with keys set for the given elem."
+        "Construct a new GNMIPath with keys set for the given elem."
         if __elem is None:
             return self._rekey(kwds)
 
         if isinstance(__elem, str):
             elem = _find_index(__elem, self.path)
         else:
             elem = __elem
@@ -114,23 +114,23 @@
         keys.update({key: str(val) for key, val in kwds.items()})
         return result
 
     def copy(self) -> Self:
         "Return a copy of the path."
         new_path = gnmi.Path()
         new_path.CopyFrom(self.path)
-        return gNMIPath(new_path)
+        return GNMIPath(new_path)
 
     @overload
     def __getitem__(self, key: int | str | tuple[int | str, str]) -> str:
-        ...
+        ...  # pragma: no cover
 
     @overload
     def __getitem__(self, key: slice) -> Self:
-        ...
+        ...  # pragma: no cover
 
     def __getitem__(
         self,
         key: int | str | tuple[int | str, str] | slice,
     ) -> str | Self:
         "Return the specified element or key value."
         match key:
@@ -154,15 +154,15 @@
             case slice() as s:
                 return self._slice(s.start, s.stop, s.step)
             case other:
                 raise TypeError(f"invalid key type: {other!r}")
 
     def __eq__(self, rhs: Self) -> bool:
         "Return True if path's are equal."
-        if not isinstance(rhs, gNMIPath):
+        if not isinstance(rhs, GNMIPath):
             return False
         return self.path == rhs.path  # pyright: ignore[reportUnknownVariableType]
 
     def __hash__(self) -> int:
         "Return hash of path."
         return hash(tuple(_to_tuple(elem) for elem in self.path.elem))
 
@@ -173,42 +173,42 @@
                 return True
         return False
 
     def __repr__(self) -> str:
         "Return string representation of path."
         path = gnmistring.to_str(self.path)
         if self.target or self.origin:
-            return f"gNMIPath({path!r}, origin={self.origin!r}, target={self.target!r})"
-        return f"gNMIPath({path!r})"
+            return f"GNMIPath({path!r}, origin={self.origin!r}, target={self.target!r})"
+        return f"GNMIPath({path!r})"
 
     def __str__(self) -> str:
         "Return path as string."
         return gnmistring.to_str(self.path)
 
     def __len__(self) -> int:
         "Return the length of the path."
         return len(self.path.elem)
 
     def __truediv__(self, rhs: Self | str) -> Self:
         "Append values to end of path."
-        if not isinstance(rhs, gNMIPath):
-            rhs = gNMIPath(rhs)
+        if not isinstance(rhs, GNMIPath):
+            rhs = GNMIPath(rhs)
 
         result = gnmi.Path(elem=itertools.chain(self.path.elem, rhs.path.elem))
-        return gNMIPath(result)
+        return GNMIPath(result)
 
     def __rtruediv__(self, lhs: str) -> Self:
         "Prepend values to the beginning of the path."
-        path = gNMIPath(lhs)
+        path = GNMIPath(lhs)
 
         result = gnmi.Path(elem=itertools.chain(path.path.elem, self.path.elem))
-        return gNMIPath(result)
+        return GNMIPath(result)
 
     def _slice(self, start: int | None, stop: int | None, step: int | None) -> Self:
-        "Return specified slice of gNMIPath."
+        "Return specified slice of GNMIPath."
 
         if start is None:
             start = 0
 
         if stop is None:
             stop = len(self)
         elif stop < 0:
@@ -218,15 +218,15 @@
             step = 1
 
         path = gnmi.Path()
         for i in range(start, stop, step):
             elem = self.path.elem[i]
             path.elem.append(gnmi.PathElem(name=elem.name, key=elem.key))
 
-        return gNMIPath(path)
+        return GNMIPath(path)
 
     def _rekey(self, keys: dict[str, Any]) -> Self:
         """Construct a new path with specified keys replaced."""
         if not keys:
             raise ValueError("empty keys")
 
         result = self.copy()
```

### Comparing `finsy-0.8.0/finsy/gnmistring.py` & `finsy-0.9.0/finsy/gnmistring.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,17 +10,22 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+# pyright/strict and parsy don't mix well.
+#   pyright: reportUnknownMemberType=false, reportUnknownArgumentType=false
+#   pyright: reportUnknownParameterType=false, reportUnknownVariableType=false
+#   pyright: reportFunctionMemberAccess=false, reportUnknownLambdaType=false
+
 import re
 
-import parsy as pa
+import parsy as pa  # pyright: ignore[reportMissingTypeStubs]
 
 from finsy.proto import gnmi
 
 #################################
 # Parser Combinator Definitions #
 #################################
 
@@ -84,15 +89,15 @@
 # Example:
 #
 # ```
 # path = gnmistring.parse("interfaces/interface[name=eth1]/state")
 # ```
 #
 # This module does NOT allow the `origin` or `target` prefix properties to be
-# specified in the string. Set these in `gNMIPath`.
+# specified in the string. Set these in `GNMIPath`.
 #
 # FIXME: This module does not support Unicode surrogate pairs.
 #
 # Reference:
 # https://github.com/openconfig/reference/blob/master/rpc/gnmi/gnmi-path-strings.md
```

### Comparing `finsy-0.8.0/finsy/grpcutil.py` & `finsy-0.9.0/finsy/grpcutil.py`

 * *Files identical despite different names*

### Comparing `finsy-0.8.0/finsy/log.py` & `finsy-0.9.0/finsy/log.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         return False
     return value.strip().lower() not in {"0", "false"}
 
 
 FINSY_DEBUG = get_setting("FINSY_DEBUG")
 
 
-if TYPE_CHECKING:
+if TYPE_CHECKING:  # pragma: no cover
     _BaseLoggerAdapter: TypeAlias = logging.LoggerAdapter[logging.Logger]
 else:
     # logging.LoggerAdapter will be generic at runtime in Python 3.11.
     _BaseLoggerAdapter: TypeAlias = logging.LoggerAdapter
 
 
 def _get_current_task_name(shorten: bool = False) -> str:
@@ -86,9 +86,10 @@
             task_name = _get_current_task_name(True)
             self.logger.info(f"[{task_name}] {msg}", *args, **kwargs)
 
 
 LOGGER = LoggerAdapter(logging.getLogger(__package__))
 MSG_LOG = LoggerAdapter(logging.getLogger(f"{__package__}.msg"))
 
-if FINSY_DEBUG:
+if FINSY_DEBUG:  # pragma: no cover
+    # If FINSY_DEBUG is true, log all protobuf messages.
     MSG_LOG.setLevel(logging.DEBUG)
```

### Comparing `finsy-0.8.0/finsy/p4arbitrator.py` & `finsy-0.9.0/finsy/p4arbitrator.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,21 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+# pyright: reportPrivateUsage=false
+
 import finsy.switch as _sw  # break circular import
 from finsy import pbuf
 from finsy.grpcutil import GRPCStatusCode
 from finsy.log import LOGGER
-from finsy.p4client import P4ClientError, P4Status
+from finsy.p4client import P4ClientError, P4RpcStatus
 from finsy.proto import U128, p4r
 
 _NOT_ASSIGNED = -1
 
 
 class Arbitrator:
     """Manages state used for client/role arbitration.
@@ -61,34 +63,34 @@
 
         if conflict:
             # Current election_id conflicts with another connection, so start
             # the bidding at one less.
             self.election_id -= 1
 
         response = await self._arbitration_request(switch)
-        status = P4Status.from_status(response.status)
+        status = P4RpcStatus.from_status(response.status)
         primary_id = U128.decode(response.election_id)
 
         while status.code == GRPCStatusCode.NOT_FOUND:
             self.election_id = primary_id
 
             response = await self._arbitration_request(switch)
-            status = P4Status.from_status(response.status)
+            status = P4RpcStatus.from_status(response.status)
             primary_id = U128.decode(response.election_id)
 
         assert status.code in (GRPCStatusCode.OK, GRPCStatusCode.ALREADY_EXISTS)
 
         self.primary_id = primary_id
         self.is_primary = status.code == GRPCStatusCode.OK
         self._check_invariant()
 
     async def update(self, switch: "_sw.Switch", msg: p4r.MasterArbitrationUpdate):
         "Called with subsequent arbitration update responses."
 
-        status_code = P4Status.from_status(msg.status).code
+        status_code = P4RpcStatus.from_status(msg.status).code
         new_primary_id = U128.decode(msg.election_id)
 
         if new_primary_id >= self.primary_id:
             self.primary_id = new_primary_id
         else:
             # TECHDEBT: simple_switch_grpc sends a status code of OK and a
             # decreased election_id when it wants the next backup client to
@@ -185,15 +187,15 @@
         assert switch._p4client is not None
 
         try:
             # TODO: Maybe put a timeout on this receive?
             response = await switch._p4client.receive()
 
         except P4ClientError as ex:
-            if ex.status.is_election_id_used:
+            if ex.is_election_id_used:
                 return None
             raise
 
         if response.WhichOneof("update") != "arbitration":
             raise ValueError(f"Unexpected response: {response!r}")
 
         # TODO: Match arbitration response to request we sent?
```

### Comparing `finsy-0.8.0/finsy/p4client.py` & `finsy-0.9.0/finsy/p4client.py`

 * *Files 15% similar despite different names*

```diff
@@ -44,185 +44,179 @@
 _NO_PIPELINE_CONFIG = re.compile(
     r"no .*\bforwarding pipeline config",
     re.IGNORECASE,
 )
 
 
 @dataclass
-class P4SubError:
+class P4Error:
+    "P4Runtime Error message used to report a single P4-entity error."
+
     canonical_code: GRPCStatusCode
     message: str
     space: str
     code: int
     subvalue: pbuf.PBMessage | None = None
 
 
 @dataclass
-class P4Status:
+class P4RpcStatus:
     "Implements rpc.status."
 
     code: GRPCStatusCode
     message: str
-    details: dict[int, P4SubError]
-
-    @property
-    def is_not_found_only(self) -> bool:
-        """Return True if the only sub-errors are NOT_FOUND."""
-        if self.code != GRPCStatusCode.UNKNOWN:
-            return False
-
-        for err in self.details.values():
-            if err.canonical_code != GRPCStatusCode.NOT_FOUND:
-                return False
-        return True
-
-    @property
-    def is_election_id_used(self) -> bool:
-        """Return true if error is that election ID is in use."""
-        return (
-            self.code == GRPCStatusCode.INVALID_ARGUMENT
-            and _ELECTION_ID_EXISTS.search(self.message) is not None
-        )
-
-    @property
-    def is_no_pipeline_configured(self) -> bool:
-        "Return true if error is that no pipeline config is set."
-        return (
-            self.code == GRPCStatusCode.FAILED_PRECONDITION
-            and _NO_PIPELINE_CONFIG.search(self.message) is not None
-        )
+    details: dict[int, P4Error]
 
     @staticmethod
-    def from_rpc_error(error: grpc.RpcError) -> "P4Status":
+    def from_rpc_error(error: grpc.RpcError) -> "P4RpcStatus":
         "Construct status from RpcError."
         assert isinstance(error, grpc.aio.AioRpcError)
 
         for key, value in error.trailing_metadata():
             if key == "grpc-status-details-bin":
                 assert isinstance(value, bytes)
-                return P4Status.from_bytes(value)
+                return P4RpcStatus.from_bytes(value)
 
-        return P4Status(
+        return P4RpcStatus(
             GRPCStatusCode.from_status_code(error.code()),
             error.details() or "",
             {},
         )
 
     @staticmethod
-    def from_bytes(data: bytes) -> "P4Status":
+    def from_bytes(data: bytes) -> "P4RpcStatus":
         "Construct status from protobuf bytes."
         status = rpc_status.Status()
         status.ParseFromString(data)
-        return P4Status.from_status(status)
+        return P4RpcStatus.from_status(status)
 
     @staticmethod
-    def from_status(status: rpc_status.Status) -> "P4Status":
+    def from_status(status: rpc_status.Status) -> "P4RpcStatus":
         "Construct status from RPC status."
-        return P4Status(
+        return P4RpcStatus(
             GRPCStatusCode(status.code),
             status.message,
-            P4Status._parse_error(status.details),
+            P4RpcStatus._parse_error(status.details),
         )
 
     @staticmethod
-    def _parse_error(details: Sequence[pbuf.PBAny]) -> dict[int, P4SubError]:
-        result: dict[int, P4SubError] = {}
+    def _parse_error(details: Sequence[pbuf.PBAny]) -> dict[int, P4Error]:
+        result: dict[int, P4Error] = {}
 
         for i in range(len(details)):
             err = pbuf.from_any(details[i], p4r.Error)
             if err.canonical_code != rpc_code.OK:
-                result[i] = P4SubError(
+                result[i] = P4Error(
                     GRPCStatusCode(err.canonical_code),
                     err.message,
                     err.space,
                     err.code,
                 )
         return result
 
 
 class P4ClientError(Exception):
-    "Wrap grpc.RpcError."
+    "Wrap `grpc.RpcError`."
 
     _operation: str
-    _status: P4Status
+    _status: P4RpcStatus
     _outer_code: GRPCStatusCode
     _outer_message: str
 
     def __init__(
         self,
         error: grpc.RpcError,
         operation: str,
         *,
         msg: pbuf.PBMessage | None = None,
     ):
         super().__init__()
         assert isinstance(error, grpc.aio.AioRpcError)
 
         self._operation = operation
-        self._status = P4Status.from_rpc_error(error)
+        self._status = P4RpcStatus.from_rpc_error(error)
         self._outer_code = GRPCStatusCode.from_status_code(error.code())
         self._outer_message = error.details() or ""
 
         if msg is not None and self.details:
             self._attach_details(msg)
 
         LOGGER.debug("%s failed: %s", operation, self)
 
     @property
-    def operation(self) -> str:
-        return self._operation
-
-    @property
-    def status(self) -> P4Status:
-        return self._status
-
-    @property
     def code(self) -> GRPCStatusCode:
+        "GRPC status code."
         return self._status.code
 
     @property
     def message(self) -> str:
+        "GRPC status message."
         return self._status.message
 
     @property
-    def details(self) -> dict[int, P4SubError]:
+    def details(self) -> dict[int, P4Error]:
+        "Optional details about P4Runtime Write updates that failed."
         return self._status.details
 
     @property
-    def is_unimplemented(self) -> bool:
-        return self.code == GRPCStatusCode.UNIMPLEMENTED
+    def is_not_found_only(self) -> bool:
+        """Return True if the only sub-errors are NOT_FOUND."""
+        if self.code != GRPCStatusCode.UNKNOWN:
+            return False
+
+        for err in self.details.values():
+            if err.canonical_code != GRPCStatusCode.NOT_FOUND:
+                return False
+        return True
+
+    @property
+    def is_election_id_used(self) -> bool:
+        """Return true if error is that election ID is in use."""
+        return (
+            self.code == GRPCStatusCode.INVALID_ARGUMENT
+            and _ELECTION_ID_EXISTS.search(self.message) is not None
+        )
+
+    @property
+    def is_pipeline_missing(self) -> bool:
+        "Return true if error is that no pipeline config is set."
+        return (
+            self.code == GRPCStatusCode.FAILED_PRECONDITION
+            and _NO_PIPELINE_CONFIG.search(self.message) is not None
+        )
 
     def _attach_details(self, msg: pbuf.PBMessage):
         "Attach the subvalue(s) from the message that caused the error."
         if isinstance(msg, p4r.WriteRequest):
             for key, value in self.details.items():
                 value.subvalue = msg.updates[key]
 
     def __str__(self) -> str:
+        "Return string representation of P4ClientError object."
         if self.details:
 
-            def _indent(value: P4SubError):
+            def _indent(value: P4Error):
                 s = repr(value).replace("\n}\n)", "\n})")  # tidy multiline repr
                 return s.replace("\n", "\n" + " " * 6)
 
             items = [""] + [
                 f"  [details.{key}] {_indent(val)}" for key, val in self.details.items()
             ]
             details = "\n".join(items)
         else:
             details = ""
 
         if self.code == self._outer_code and self.message == self._outer_message:
             return (
-                f"operation={self.operation} code={self.code!r} "
+                f"operation={self._operation} code={self.code!r} "
                 f"message={self.message!r} {details}"
             )
         return (
             f"code={self.code!r} message={self.message!r} "
-            f"details={self.details!r} operation={self.operation} "
+            f"details={self.details!r} operation={self._operation} "
             f"_outer_message={self._outer_message!r} _outer_code={self._outer_code!r}"
         )
 
 
 _P4StreamTypeAlias: TypeAlias = grpc.aio.StreamStreamCall[
     p4r.StreamMessageRequest, p4r.StreamMessageResponse
 ]
@@ -340,31 +334,31 @@
             raise P4ClientError(ex, "receive") from None
 
         self._log_msg(msg)
         return msg
 
     @overload
     async def request(self, msg: p4r.WriteRequest) -> p4r.WriteResponse:
-        ...
+        ...  # pragma: no cover
 
     @overload
     async def request(
         self, msg: p4r.GetForwardingPipelineConfigRequest
     ) -> p4r.GetForwardingPipelineConfigResponse:
-        ...
+        ...  # pragma: no cover
 
     @overload
     async def request(
         self, msg: p4r.SetForwardingPipelineConfigRequest
     ) -> p4r.SetForwardingPipelineConfigResponse:
-        ...
+        ...  # pragma: no cover
 
     @overload
     async def request(self, msg: p4r.CapabilitiesRequest) -> p4r.CapabilitiesResponse:
-        ...
+        ...  # pragma: no cover
 
     async def request(self, msg: pbuf.PBMessage) -> pbuf.PBMessage:
         "Send a unary-unary P4Runtime request and wait for the response."
 
         if self._complete_request:
             self._complete_request(msg)
```

### Comparing `finsy-0.8.0/finsy/p4entity.py` & `finsy-0.9.0/finsy/p4entity.py`

 * *Files identical despite different names*

### Comparing `finsy-0.8.0/finsy/p4schema.py` & `finsy-0.9.0/finsy/p4schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -940,15 +940,15 @@
         return P4ActionScope(self.pbuf.scope)
 
 
 class P4ActionProfile(_P4TopLevel[p4i.ActionProfile]):
     "Represents ActionProfile in schema."
 
     _actions: P4EntityMap[P4Action]
-    _table_names: list[str]
+    _table_names: list[str] = []
 
     def __init__(self, pbuf: p4i.ActionProfile):
         super().__init__(pbuf)
         self._actions = P4EntityMap("action")
 
     def _finish_init(self, defs: _P4Defs):
         # Copy actions from first table.  FIXME: Is `actions` used anywhere?
@@ -1195,15 +1195,15 @@
     def decode(self, data: p4r.PacketMetadata):
         return p4values.decode_exact(data.value, self.bitwidth)
 
 
 class P4DirectCounter(_P4TopLevel[p4i.DirectCounter]):
     "Represents DirectCounter in schema."
 
-    _direct_table_name: str
+    _direct_table_name: str = ""
 
     def _finish_init(self, defs: _P4Defs):
         direct_table = defs.tables[self.direct_table_id]
         assert direct_table.direct_counter == self
         self._direct_table_name = direct_table.name
 
     @property
@@ -1804,15 +1804,15 @@
     def size(self) -> int:
         return self.pbuf.size
 
 
 class P4Digest(_P4TopLevel[p4i.Digest]):
     "Represents Digest in schema."
 
-    _type_spec: _P4Type
+    _type_spec: _P4Type  # pyright: ignore[reportUninitializedInstanceVariable]
 
     def _finish_init(self, defs: _P4Defs):
         self._type_spec = _parse_type_spec(self.pbuf.type_spec, defs.type_info)
 
     @property
     def type_spec(self) -> _P4Type:
         return self._type_spec
```

### Comparing `finsy-0.8.0/finsy/p4values.py` & `finsy-0.9.0/finsy/p4values.py`

 * *Files identical despite different names*

### Comparing `finsy-0.8.0/finsy/pbuf.py` & `finsy-0.9.0/finsy/pbuf.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 import grpc  # pyright: ignore [reportMissingTypeStubs]
 from google.protobuf import json_format, text_format
 from google.protobuf.any_pb2 import Any as _Any  # pylint: disable=E0611
 from google.protobuf.message import Message as _Message
 
 import finsy as _fy
-from finsy.gnmiclient import gNMIPath
+from finsy.gnmiclient import GNMIPath
 from finsy.log import MSG_LOG
 from finsy.proto import gnmi, p4r
 
 PBAny = _Any
 PBMessage = _Message
 
 _MT = TypeVar("_MT", bound=PBMessage)
@@ -105,20 +105,20 @@
         if msg.HasField("cookie"):
             cookie = f"0x{msg.cookie.cookie:x}"
         else:
             cookie = "<unset>"
         return f"📦p4cookie={cookie}"
 
     if isinstance(msg, gnmi.Path):
-        return f"📂{gNMIPath(msg)}"
+        return f"📂{GNMIPath(msg)}"
 
     if isinstance(msg, gnmi.Update):
         value = repr(msg.val).strip()
         dups = "" if not msg.duplicates else f" ({msg.duplicates} dups)"
-        return f"📂{gNMIPath(msg.path)} = {value}{dups}"
+        return f"📂{GNMIPath(msg.path)} = {value}{dups}"
 
     if isinstance(msg, (p4r.PacketIn, p4r.PacketOut)):
         metadata = " ".join(
             f"meta[{md.metadata_id}]={md.value.hex()}" for md in msg.metadata
         )
         return f"📬{msg.payload.hex()} {metadata}"
 
@@ -145,16 +145,16 @@
 
     Format:
         <state><mesg-type> (<size> bytes): <msg-contents>
 
     <state> is empty if the client state is READY. Otherwise, it's the
     channel connectivity state.
     """
-    if not MSG_LOG.isEnabledFor(level):
-        return  # pragma: no cover
+    if not MSG_LOG.isEnabledFor(level):  # pragma: no cover
+        return
 
     # Include the channel's state if it's not READY.
     assert channel is not None
     state = channel.get_state()
     state_name = ""
     if state != grpc.ChannelConnectivity.READY:
         state_name = f"{state.name} "  # trailing space necessary
```

### Comparing `finsy-0.8.0/finsy/ports.py` & `finsy-0.9.0/finsy/ports.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import enum
 from dataclasses import dataclass
 
 import finsy.switch as _sw  # circular import
-from finsy.gnmiclient import gNMIClient, gNMIPath, gNMISubscription, gNMIUpdate
+from finsy.gnmiclient import GNMIClient, GNMIPath, GNMISubscription, GNMIUpdate
 from finsy.log import LOGGER
 
 # FIXME: Use GNMI id or ifIndex?
-_ifIndex = gNMIPath("interfaces/interface[name=*]/state/ifindex")
-_ifOperStatus = gNMIPath("interfaces/interface[name=*]/state/oper-status")
+_ifIndex = GNMIPath("interfaces/interface[name=*]/state/ifindex")
+_ifOperStatus = GNMIPath("interfaces/interface[name=*]/state/oper-status")
 
 
 class OperStatus(enum.Enum):
     "gNMI values for ifOperStatus"
 
     DORMANT = "DORMANT"
     LOWER_LAYER_DOWN = "LOWER_LAYER_DOWN"
@@ -35,47 +35,47 @@
     TESTING = "TESTING"
     UP = "UP"
     DOWN = "DOWN"
     NOT_PRESENT = "NOT_PRESENT"
 
 
 @dataclass
-class Port:
+class SwitchPort:
     "Represents a switch port."
 
     id: int
     name: str
     oper_status: OperStatus = OperStatus.UNKNOWN
 
     @property
     def up(self) -> bool:
         "Return true if port is basically up."
         return self.oper_status == OperStatus.UP
 
 
-class PortList:
+class SwitchPortList:
     "Represents a list of switch ports."
 
-    _ports: dict[str, Port]
-    _subscription: gNMISubscription | None = None
+    _ports: dict[str, SwitchPort]
+    _subscription: GNMISubscription | None = None
 
     def __init__(self):
         self._ports = {}
 
     def __getitem__(self, key: str):
         "Retrieve interface by ID."
         return self._ports[key]
 
     def __len__(self):
         return len(self._ports)
 
     def __iter__(self):
         return iter(self._ports.values())
 
-    async def subscribe(self, client: gNMIClient):
+    async def subscribe(self, client: GNMIClient):
         assert self._subscription is None
 
         self._ports = await self._get_ports(client)
         self._subscription = await self._get_subscription(client)
 
     async def update(self, switch: "_sw.Switch | None" = None):
         assert self._subscription is not None
@@ -85,42 +85,42 @@
 
     def close(self):
         if self._subscription is not None:
             self._subscription.cancel()
             self._subscription = None
             self._ports = {}
 
-    async def _get_ports(self, client: gNMIClient) -> dict[str, Port]:
+    async def _get_ports(self, client: GNMIClient) -> dict[str, SwitchPort]:
         "Retrieve ID and name of each port."
-        ports: dict[str, Port] = {}
+        ports: dict[str, SwitchPort] = {}
 
         result = await client.get(_ifIndex)
         for update in result:
             path = update.path
             assert path.last == _ifIndex.last
 
-            port = Port(update.value, path["name"])
+            port = SwitchPort(update.value, path["name"])
             ports[port.name] = port
 
         return ports
 
-    async def _get_subscription(self, client: gNMIClient):
+    async def _get_subscription(self, client: GNMIClient):
         sub = client.subscribe()
 
         # Subscribe to change notifications.
         for port in self._ports.values():
             sub.on_change(_ifOperStatus.set(name=port.name))
 
         # Synchronize initial settings for ports.
         async for update in sub.synchronize():
             self._update(update, None)
 
         return sub
 
-    def _update(self, update: gNMIUpdate, switch: "_sw.Switch | None"):
+    def _update(self, update: GNMIUpdate, switch: "_sw.Switch | None"):
         path = update.path
         name = path["name"]
 
         match path.last:
             case _ifOperStatus.last:
                 status = OperStatus(update.value)
                 self._update_port(name, status, switch)
```

### Comparing `finsy-0.8.0/finsy/proto/__init__.py` & `finsy-0.9.0/finsy/proto/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,16 +40,16 @@
 import sys
 
 # Generated protobuf files reference their dependencies using absolute imports.
 # To work around this, modify the import path to substitute our embedded
 # modules for global "p4" and "google.rpc" modules. After we've imported the
 # protobuf modules, we switch `sys.path` back.
 
-if "p4.v1.p4runtime_pb2" in sys.modules:
-    raise RuntimeError("p4runtime_pb2 already imported?")  # pragma: no cover
+if "p4.v1.p4runtime_pb2" in sys.modules:  # pragma: no cover
+    raise RuntimeError("p4runtime_pb2 already imported?")
 
 sys.path.insert(0, os.path.dirname(__file__))
 
 from gnmi1 import gnmi_ext_pb2 as gnmi_ext
 from gnmi1 import gnmi_pb2 as gnmi
 from gnmi1 import gnmi_pb2_grpc as gnmi_grpc
 from google.rpc import code_pb2 as rpc_code
@@ -67,15 +67,15 @@
 class U128:
     "Utility class for p4r.Uint128."
 
     @staticmethod
     def encode(value: int) -> p4r.Uint128:
         "Create a Uint128 object from an integer."
 
-        if not isinstance(value, int) or value < 0:
+        if value < 0:
             raise ValueError(f"invalid argument: {value!r}")
         return p4r.Uint128(high=value >> 64, low=value & 0xFFFFFFFFFFFFFFFF)
 
     @staticmethod
     def decode(value: p4r.Uint128) -> int:
         "Convert a Uint128 object to an integer."
```

### Comparing `finsy-0.8.0/finsy/proto/gnmi1/gnmi.proto` & `finsy-0.9.0/finsy/proto/gnmi1/gnmi.proto`

 * *Files identical despite different names*

### Comparing `finsy-0.8.0/finsy/proto/gnmi1/gnmi_ext.proto` & `finsy-0.9.0/finsy/proto/gnmi1/gnmi_ext.proto`

 * *Files identical despite different names*

### Comparing `finsy-0.8.0/finsy/proto/gnmi1/gnmi_ext_pb2.py` & `finsy-0.9.0/finsy/proto/gnmi1/gnmi_ext_pb2.py`

 * *Files identical despite different names*

### Comparing `finsy-0.8.0/finsy/proto/gnmi1/gnmi_ext_pb2.pyi` & `finsy-0.9.0/finsy/proto/gnmi1/gnmi_ext_pb2.pyi`

 * *Files identical despite different names*

### Comparing `finsy-0.8.0/finsy/proto/gnmi1/gnmi_pb2.py` & `finsy-0.9.0/finsy/proto/gnmi1/gnmi_pb2.py`

 * *Files identical despite different names*

### Comparing `finsy-0.8.0/finsy/proto/gnmi1/gnmi_pb2.pyi` & `finsy-0.9.0/finsy/proto/gnmi1/gnmi_pb2.pyi`

 * *Files identical despite different names*

### Comparing `finsy-0.8.0/finsy/proto/gnmi1/gnmi_pb2_grpc.py` & `finsy-0.9.0/finsy/proto/gnmi1/gnmi_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finsy-0.8.0/finsy/proto/gnmi1/gnmi_pb2_grpc.pyi` & `finsy-0.9.0/finsy/proto/gnmi1/gnmi_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `finsy-0.8.0/finsy/proto/google/rpc/code.proto` & `finsy-0.9.0/finsy/proto/google/rpc/code.proto`

 * *Files identical despite different names*

### Comparing `finsy-0.8.0/finsy/proto/google/rpc/code_pb2.py` & `finsy-0.9.0/finsy/proto/google/rpc/code_pb2.py`

 * *Files identical despite different names*

### Comparing `finsy-0.8.0/finsy/proto/google/rpc/code_pb2.pyi` & `finsy-0.9.0/finsy/proto/google/rpc/code_pb2.pyi`

 * *Files identical despite different names*

### Comparing `finsy-0.8.0/finsy/proto/google/rpc/context/attribute_context.proto` & `finsy-0.9.0/finsy/proto/google/rpc/context/attribute_context.proto`

 * *Files identical despite different names*

### Comparing `finsy-0.8.0/finsy/proto/google/rpc/context/attribute_context_pb2.py` & `finsy-0.9.0/finsy/proto/google/rpc/context/attribute_context_pb2.py`

 * *Files identical despite different names*

### Comparing `finsy-0.8.0/finsy/proto/google/rpc/context/attribute_context_pb2.pyi` & `finsy-0.9.0/finsy/proto/google/rpc/context/attribute_context_pb2.pyi`

 * *Files identical despite different names*

### Comparing `finsy-0.8.0/finsy/proto/google/rpc/error_details.proto` & `finsy-0.9.0/finsy/proto/google/rpc/error_details.proto`

 * *Files identical despite different names*

### Comparing `finsy-0.8.0/finsy/proto/google/rpc/error_details_pb2.py` & `finsy-0.9.0/finsy/proto/google/rpc/error_details_pb2.py`

 * *Files identical despite different names*

### Comparing `finsy-0.8.0/finsy/proto/google/rpc/error_details_pb2.pyi` & `finsy-0.9.0/finsy/proto/google/rpc/error_details_pb2.pyi`

 * *Files identical despite different names*

### Comparing `finsy-0.8.0/finsy/proto/google/rpc/status.proto` & `finsy-0.9.0/finsy/proto/google/rpc/status.proto`

 * *Files identical despite different names*

### Comparing `finsy-0.8.0/finsy/proto/google/rpc/status_pb2.py` & `finsy-0.9.0/finsy/proto/google/rpc/status_pb2.py`

 * *Files identical despite different names*

### Comparing `finsy-0.8.0/finsy/proto/google/rpc/status_pb2.pyi` & `finsy-0.9.0/finsy/proto/google/rpc/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `finsy-0.8.0/finsy/proto/p4/config/v1/p4info.proto` & `finsy-0.9.0/finsy/proto/p4/config/v1/p4info.proto`

 * *Files identical despite different names*

### Comparing `finsy-0.8.0/finsy/proto/p4/config/v1/p4info_pb2.py` & `finsy-0.9.0/finsy/proto/p4/config/v1/p4info_pb2.py`

 * *Files identical despite different names*

### Comparing `finsy-0.8.0/finsy/proto/p4/config/v1/p4info_pb2.pyi` & `finsy-0.9.0/finsy/proto/p4/config/v1/p4info_pb2.pyi`

 * *Files identical despite different names*

### Comparing `finsy-0.8.0/finsy/proto/p4/config/v1/p4types.proto` & `finsy-0.9.0/finsy/proto/p4/config/v1/p4types.proto`

 * *Files identical despite different names*

### Comparing `finsy-0.8.0/finsy/proto/p4/config/v1/p4types_pb2.py` & `finsy-0.9.0/finsy/proto/p4/config/v1/p4types_pb2.py`

 * *Files identical despite different names*

### Comparing `finsy-0.8.0/finsy/proto/p4/config/v1/p4types_pb2.pyi` & `finsy-0.9.0/finsy/proto/p4/config/v1/p4types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `finsy-0.8.0/finsy/proto/p4/v1/p4data.proto` & `finsy-0.9.0/finsy/proto/p4/v1/p4data.proto`

 * *Files identical despite different names*

### Comparing `finsy-0.8.0/finsy/proto/p4/v1/p4data_pb2.py` & `finsy-0.9.0/finsy/proto/p4/v1/p4data_pb2.py`

 * *Files identical despite different names*

### Comparing `finsy-0.8.0/finsy/proto/p4/v1/p4data_pb2.pyi` & `finsy-0.9.0/finsy/proto/p4/v1/p4data_pb2.pyi`

 * *Files identical despite different names*

### Comparing `finsy-0.8.0/finsy/proto/p4/v1/p4runtime.proto` & `finsy-0.9.0/finsy/proto/p4/v1/p4runtime.proto`

 * *Files identical despite different names*

### Comparing `finsy-0.8.0/finsy/proto/p4/v1/p4runtime_pb2.py` & `finsy-0.9.0/finsy/proto/p4/v1/p4runtime_pb2.py`

 * *Files identical despite different names*

### Comparing `finsy-0.8.0/finsy/proto/p4/v1/p4runtime_pb2.pyi` & `finsy-0.9.0/finsy/proto/p4/v1/p4runtime_pb2.pyi`

 * *Files identical despite different names*

### Comparing `finsy-0.8.0/finsy/proto/p4/v1/p4runtime_pb2_grpc.py` & `finsy-0.9.0/finsy/proto/p4/v1/p4runtime_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finsy-0.8.0/finsy/proto/p4/v1/p4runtime_pb2_grpc.pyi` & `finsy-0.9.0/finsy/proto/p4/v1/p4runtime_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `finsy-0.8.0/finsy/proto/stratum1/p4_role_config.proto` & `finsy-0.9.0/finsy/proto/stratum1/p4_role_config.proto`

 * *Files identical despite different names*

### Comparing `finsy-0.8.0/finsy/proto/stratum1/p4_role_config_pb2.py` & `finsy-0.9.0/finsy/proto/stratum1/p4_role_config_pb2.py`

 * *Files identical despite different names*

### Comparing `finsy-0.8.0/finsy/proto/stratum1/p4_role_config_pb2.pyi` & `finsy-0.9.0/finsy/proto/stratum1/p4_role_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `finsy-0.8.0/finsy/switch.py` & `finsy-0.9.0/finsy/switch.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,21 +36,21 @@
 
 import grpc  # pyright: ignore[reportMissingTypeStubs]
 import pyee
 from typing_extensions import Self
 
 from finsy import p4entity, pbuf
 from finsy.futures import CountdownFuture
-from finsy.gnmiclient import gNMIClient, gNMIClientError
+from finsy.gnmiclient import GNMIClient, GNMIClientError
 from finsy.grpcutil import GRPCStatusCode
 from finsy.log import LOGGER
 from finsy.p4arbitrator import Arbitrator
 from finsy.p4client import P4Client, P4ClientError
 from finsy.p4schema import P4ConfigAction, P4ConfigResponseType, P4Schema
-from finsy.ports import PortList
+from finsy.ports import SwitchPortList
 from finsy.proto import p4r
 
 # Maximum size of queues used for PacketIn, DigestList, etc.
 
 _DEFAULT_QUEUE_SIZE = 50
 
 # If switch fails to run for longer than _FAIL_MIN_TIME_SECS, wait
@@ -143,16 +143,16 @@
     _options: SwitchOptions
     _p4client: P4Client | None
     _p4schema: P4Schema
     _tasks: "SwitchTasks | None"
     _queues: dict[str, asyncio.Queue[Any]]
     _packet_queues: list[tuple[Callable[[bytes], bool], asyncio.Queue[Any]]]
     _arbitrator: "Arbitrator"
-    _gnmi_client: gNMIClient | None
-    _ports: PortList
+    _gnmi_client: GNMIClient | None
+    _ports: SwitchPortList
     _is_channel_up: bool = False
     _api_version: ApiVersion = ApiVersion(1, 0, 0, "")
 
     control_task: asyncio.Task[Any] | None = None
     "Used by Controller to track switch's main task."
 
     ee: "SwitchEmitter"
@@ -178,15 +178,15 @@
         self._tasks = None
         self._queues = {}
         self._packet_queues = []
         self._arbitrator = Arbitrator(
             options.initial_election_id, options.role_name, options.role_config
         )
         self._gnmi_client = None
-        self._ports = PortList()
+        self._ports = SwitchPortList()
         self.ee = SwitchEmitter(self)
 
     @property
     def name(self) -> str:
         "Name of the switch."
         return self._name
 
@@ -244,20 +244,20 @@
 
     @property
     def p4info(self) -> P4Schema:
         "Switch's P4 schema."
         return self._p4schema
 
     @property
-    def gnmi_client(self) -> gNMIClient | None:
+    def gnmi_client(self) -> GNMIClient | None:
         "Switch's gNMI client."
         return self._gnmi_client
 
     @property
-    def ports(self) -> PortList:
+    def ports(self) -> SwitchPortList:
         "Switch's list of interfaces."
         return self._ports
 
     @property
     def api_version(self) -> ApiVersion:
         "P4Runtime protocol version."
         return self._api_version
@@ -399,15 +399,15 @@
 
         client = self._p4client
 
         while True:
             try:
                 msg = await client.receive()
             except P4ClientError as ex:
-                if not ex.status.is_election_id_used:
+                if not ex.is_election_id_used:
                     raise
                 # Handle "election ID in use" error.
                 await self._arbitrator.handshake(self, conflict=True)
             else:
                 await self._handle_stream_message(msg)
 
     async def _handle_stream_message(self, msg: p4r.StreamMessageResponse):
@@ -482,40 +482,45 @@
         self._switch_stop()
 
     def _switch_start(self):
         "Called when switch starts its run() cycle."
         assert not self._is_channel_up
 
         LOGGER.info(
-            "Switch start (name=%r, address=%r, device_id=%r, initial_election_id=%r)",
+            "Switch start (name=%r, address=%r, device_id=%r, role_name=%r, initial_election_id=%r)",
             self.name,
-            self._address,
+            self.address,
             self.device_id,
+            self.role_name,
             self.options.initial_election_id,
         )
         self.ee.emit(SwitchEvent.SWITCH_START)
 
     def _switch_stop(self):
         "Called when switch stops its run() cycle."
         assert not self._is_channel_up
 
-        LOGGER.info("Switch stop (name=%r)", self.name)
+        LOGGER.info(
+            "Switch stop (name=%r, address=%r, device_id=%r, role_name=%r)",
+            self.name,
+            self.address,
+            self.device_id,
+            self.role_name,
+        )
         self.ee.emit(SwitchEvent.SWITCH_STOP)
 
     def _channel_up(self):
         "Called when P4Runtime channel is UP."
         assert not self._is_channel_up
 
         ports = " ".join(f"({port.id}){port.name}" for port in self.ports)
         LOGGER.info(
-            "Channel up (is_primary=%r, role_name=%r, election_id=%r, primary_id=%r, p4r=%s): %s",
+            "Channel up (is_primary=%r, role_name=%r, p4r=%s): %s",
             self.is_primary,
             self.role_name,
-            self.election_id,
-            self.primary_id,
             self.api_version,
             ports,
         )
         self._is_channel_up = True
         self.create_task(self._ready())
 
         self.ee.emit(SwitchEvent.CHANNEL_UP, self)
@@ -535,36 +540,32 @@
         self.ee.emit(SwitchEvent.CHANNEL_DOWN, self)
 
     def _become_primary(self):
         "Called when a P4Runtime backup channel becomes the primary."
         assert self._tasks is not None
 
         LOGGER.info(
-            "Become primary (is_primary=%r, role_name=%r, election_id=%r, primary_id=%r)",
+            "Become primary (is_primary=%r, role_name=%r)",
             self.is_primary,
             self.role_name,
-            self.election_id,
-            self.primary_id,
         )
 
         self._tasks.cancel_primary()
         self.create_task(self._ready())
 
         self.ee.emit(SwitchEvent.BECOME_PRIMARY, self)
 
     def _become_backup(self):
         "Called when a P4Runtime primary channel becomes a backup."
         assert self._tasks is not None
 
         LOGGER.info(
-            "Become backup (is_primary=%r, role_name=%r, election_id=%r, primary_id=%r)",
+            "Become backup (is_primary=%r, role_name=%r)",
             self.is_primary,
             self.role_name,
-            self.election_id,
-            self.primary_id,
         )
 
         self._tasks.cancel_primary()
         self.create_task(self._ready())
 
         self.ee.emit(SwitchEvent.BECOME_BACKUP, self)
 
@@ -630,15 +631,15 @@
                     # If we don't have P4Info yet, set it.
                     self.p4info.set_p4info(p4info)
                 elif not self.p4info.has_p4info(p4info):
                     # If P4Info is not identical, log a warning message.
                     LOGGER.warning("Retrieved P4Info is different than expected!")
 
         except P4ClientError as ex:
-            if not ex.status.is_no_pipeline_configured:
+            if not ex.is_pipeline_missing:
                 raise
 
         if not has_pipeline and self.p4info.exists:
             LOGGER.warning("Forwarding pipeline is not configured")
 
     async def _set_pipeline(self):
         "Set up the pipeline."
@@ -646,15 +647,15 @@
         cookie = -1
         try:
             reply = await self._get_pipeline_config_request()
             if reply.config.HasField("cookie"):
                 cookie = reply.config.cookie.cookie
 
         except P4ClientError as ex:
-            if not ex.status.is_no_pipeline_configured:
+            if not ex.is_pipeline_missing:
                 raise
 
         if cookie != self.p4info.p4cookie:
             LOGGER.debug(
                 "cookie %#x does not match expected %#x", cookie, self.p4info.p4cookie
             )
             await self._set_pipeline_config_request(
@@ -880,52 +881,52 @@
             await self._p4client.request(
                 p4r.WriteRequest(
                     device_id=self.device_id,
                     updates=updates,
                 )
             )
         except P4ClientError as ex:
-            if strict or not ex.status.is_not_found_only:
+            if strict or not ex.is_not_found_only:
                 if warn_only:
                     LOGGER.warning(
                         "WriteRequest with `warn_only=True` failed",
                         exc_info=True,
                     )
                 else:
                     raise
 
-            assert (not strict and ex.status.is_not_found_only) or warn_only
+            assert (not strict and ex.is_not_found_only) or warn_only
 
     async def _fetch_capabilities(self):
         "Check the P4Runtime protocol version supported by the other end."
         assert self._p4client is not None
 
         try:
             reply = await self._p4client.request(p4r.CapabilitiesRequest())
             self._api_version = ApiVersion.parse(reply.p4runtime_api_version)
 
         except P4ClientError as ex:
-            if not ex.is_unimplemented:
+            if ex.code != GRPCStatusCode.UNIMPLEMENTED:
                 raise
             LOGGER.warning("CapabilitiesRequest is not implemented")
 
     async def _start_gnmi(self):
         "Start the associated gNMI client."
         assert self._gnmi_client is None
         assert self._p4client is not None
 
-        self._gnmi_client = gNMIClient(self._address, self._options.channel_credentials)
+        self._gnmi_client = GNMIClient(self._address, self._options.channel_credentials)
         await self._gnmi_client.open(channel=self._p4client.channel)
 
         try:
             await self._ports.subscribe(self._gnmi_client)
             self.create_task(self._ports.update(), background=True, name="_ports")
 
-        except gNMIClientError as ex:
-            if not ex.is_unimplemented:
+        except GNMIClientError as ex:
+            if ex.code != GRPCStatusCode.UNIMPLEMENTED:
                 raise
             LOGGER.warning("gNMI is not implemented")
             await self._gnmi_client.close()
             self._gnmi_client = None
 
     async def _stop_gnmi(self):
         "Stop the associated gNMI client."
```

### Comparing `finsy-0.8.0/finsy/test/gnmi_server.py` & `finsy-0.9.0/finsy/test/gnmi_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,19 +15,20 @@
 # limitations under the License.
 
 import asyncio
 import contextlib
 from typing import AsyncIterator
 
 import grpc
+
 from finsy import pbuf
 from finsy.proto import gnmi, gnmi_grpc
 
 
-class gNMIServer(gnmi_grpc.gNMIServicer):
+class GNMIServer(gnmi_grpc.gNMIServicer):
     "Test gNMI server."
 
     _listen_addr: str
     _server: grpc.aio.Server | None
 
     def __init__(self, listen_addr: str):
         "Initialize gNMI server."
```

### Comparing `finsy-0.8.0/finsy/test/p4runtime_server.py` & `finsy-0.9.0/finsy/test/p4runtime_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import argparse
 import asyncio
 import contextlib
 import logging
 from typing import AsyncIterator
 
 import grpc
+
 from finsy.futures import wait_for_cancel
 from finsy.log import LOGGER
 from finsy.proto import p4r, p4r_grpc
 
 
 class _TaskSet(set[asyncio.Task]):
     "Keep fire-and-forget Tasks alive while task is running."
@@ -56,15 +57,17 @@
             await self._server.stop(0)
             self._server = None
 
     def _create_server(self) -> grpc.aio.Server:
         "Create AIO server."
 
         server = grpc.aio.server()
-        p4r_grpc.add_P4RuntimeServicer_to_server(self, server)
+        p4r_grpc.add_P4RuntimeServicer_to_server(
+            self, server  # pyright: ignore[reportGeneralTypeIssues]
+        )
         server.add_insecure_port(self._listen_addr)
         return server
 
     async def StreamChannel(
         self,
         _request_iter,
         context: grpc.aio.ServicerContext,
```

### Comparing `finsy-0.8.0/pyproject.toml` & `finsy-0.9.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "finsy"
-version = "0.8.0"
+version = "0.9.0"
 description = "P4Runtime Client Library"
 license = "Apache-2.0"
 authors = ["Bill Fisher <william.w.fisher@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/byllyfish/finsy"
 classifiers = [
   "Development Status :: 3 - Alpha", 
@@ -54,36 +54,27 @@
   "finsy/proto/**/*_pb2_grpc.py", 
   "finsy/proto/**/*_pb2_grpc.pyi", 
   "examples/ngsdn/demonet/topo-v6.py",
   "examples/tests/*.py"
 ]
 strict = [
   "examples/**/*.py", 
-  "finsy/p4values.py", 
-  "finsy/pbuf.py", 
-  "finsy/util.py", 
-  "finsy/log.py", 
-  "finsy/grpcutil.py", 
-  "finsy/p4entity.py", 
-  "finsy/p4schema.py", 
-  "finsy/p4client.py", 
-  "finsy/gnmipath.py", 
-  "finsy/gnmiclient.py", 
-  "finsy/ports.py", 
-  "finsy/switch.py", 
+  "finsy/*.py",
   "tests/test_p4data.py",
   "tests/test_p4entity.py",
-  "tests/test_p4values.py"
+  "tests/test_p4values.py",
+  "tests/test_controller.py",
+  "tests/test_switch.py"
 ]
 useLibraryCodeForTypes = true
 
 # Enable additional warnings for things not enabled by `strict`.
-# reportUninitializedInstanceVariable = "warning"
+reportUninitializedInstanceVariable = "warning"
 reportCallInDefaultInitializer = "warning"
-reportUnnecessaryTypeIgnoreComment = "warning"
+# reportUnnecessaryTypeIgnoreComment = "warning"
 
 [tool.black]
 target-version = ['py310']
 required-version = "22.10.0"
 extend-exclude = "_pb2(_grpc)?\\.pyi?$"
 
 [tool.coverage.run]
@@ -92,15 +83,14 @@
 
 [tool.pylint.main]
 ignore-patterns = [".*_pb2\\.py", ".*_pb2_grpc\\.py"]
 ignore-paths = ["finsy/proto"]
 
 [tool.pylint.basic]
 good-names = ["i", "j", "k", "ex", "Run", "_", "m", "s", "ee", "up", "id", "vt"]
-good-names-rgxs = ["gNMI[A-Za-z]*"]
 
 [tool.pylint.design]
 max-attributes = 15
 max-public-methods = 25
 
 [tool.pylint.format]
 max-module-lines = 2000
```

### Comparing `finsy-0.8.0/setup.py` & `finsy-0.9.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,17 +23,17 @@
  'parsy>=2.0.0,<3.0.0',
  'protobuf>=4.21.5,<5.0.0',
  'pyee>=9.0.4,<10.0.0',
  'pylev>=1.4.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'finsy',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'P4Runtime Client Library',
-    'long_description': '# 🐟 Finsy P4Runtime Library\n\n[![pypi](https://img.shields.io/pypi/v/finsy)](https://pypi.org/project/finsy/) [![ci](https://github.com/byllyfish/finsy/actions/workflows/ci.yml/badge.svg)](https://github.com/byllyfish/finsy/actions/workflows/ci.yml) [![codecov](https://codecov.io/gh/byllyfish/finsy/branch/main/graph/badge.svg?token=8RPYWRXNGS)](https://codecov.io/gh/byllyfish/finsy)\n\nFinsy is a [P4Runtime](https://p4.org/p4-spec/p4runtime/main/P4Runtime-Spec.html) controller library written in Python using asyncio. Finsy includes support for [gNMI](https://github.com/openconfig/reference/blob/master/rpc/gnmi/gnmi-specification.md).\n\n```python\nimport asyncio\nimport finsy as fy\n\nasync def main():\n    async with fy.Switch("sw1", "127.0.0.1:50001") as sw1:\n        print(sw1.p4info)\n\nasyncio.run(main())\n```\n\n## Multiple Switches\n\nWith Finsy, you can write a P4Runtime controller that manages multiple switches.\n\nEach switch is managed by an async `ready_handler` function. Your `ready_handler` function can read or \nupdate various P4Runtime entities in the switch. It can also create tasks to listen for \npackets or digests.\n\nWhen you write P4Runtime updates to the switch, you use a unary operator (+, -, \\~) to specify the operation:\nINSERT (+), DELETE (-) or MODIFY (\\~).\n\n```python\nasync def ready_handler(sw: fy.Switch):\n    await sw.delete_all()\n    await sw.write(\n        [\n            # Insert multicast group with ports 1, 2, 3 and CONTROLLER.\n            +fy.P4MulticastGroupEntry(1, replicas=[1, 2, 3, 255]),\n            # Modify default table entry to flood all unmatched packets.\n            ~fy.P4TableEntry(\n                "ipv4",\n                action=fy.P4TableAction("flood"),\n                is_default_action=True,\n            ),\n        ]\n    )\n\n    async for packet in sw.read_packets():\n        print(f"{sw.name}: {packet}")\n```\n\nUse the `SwitchOptions` class to specify each switch\'s settings, including the p4info/p4blob and \n`ready_handler`. Use the `Controller` class to drive multiple switch connections. Each switch will call back\ninto your `ready_handler` function after the P4Runtime connection is established.\n\n```python\nfrom pathlib import Path\n\noptions = fy.SwitchOptions(\n    p4info=Path("hello.p4info.txt"),\n    p4blob=Path("hello.json"),\n    ready_handler=ready_handler,\n)\n\ncontroller = fy.Controller([\n    fy.Switch("sw1", "127.0.0.1:50001", options),\n    fy.Switch("sw2", "127.0.0.1:50002", options),\n    fy.Switch("sw3", "127.0.0.1:50003", options),\n])\n\nasyncio.run(controller.run())\n```\n\nIf the switch disconnects or its role changes to backup, the task running your `ready_handler` \n(and any tasks it spawned) will be cancelled and the `ready_handler` will begin again.\n\nFor more examples, see the [examples](https://github.com/byllyfish/finsy/tree/main/examples) directory.\n',
+    'long_description': '# 🐟 Finsy P4Runtime Library\n\n[![pypi](https://img.shields.io/pypi/v/finsy)](https://pypi.org/project/finsy/) [![ci](https://github.com/byllyfish/finsy/actions/workflows/ci.yml/badge.svg)](https://github.com/byllyfish/finsy/actions/workflows/ci.yml) [![codecov](https://codecov.io/gh/byllyfish/finsy/branch/main/graph/badge.svg?token=8RPYWRXNGS)](https://codecov.io/gh/byllyfish/finsy) [![docs](https://img.shields.io/badge/-docs-informational)](https://byllyfish.github.io/finsy/finsy.html)\n\nFinsy is a [P4Runtime](https://p4.org/p4-spec/p4runtime/main/P4Runtime-Spec.html) controller library written in Python using asyncio. Finsy includes support for [gNMI](https://github.com/openconfig/reference/blob/master/rpc/gnmi/gnmi-specification.md).\n\n```python\nimport asyncio\nimport finsy as fy\n\nasync def main():\n    async with fy.Switch("sw1", "127.0.0.1:50001") as sw1:\n        print(sw1.p4info)\n\nasyncio.run(main())\n```\n\n## Requirements\n\nFinsy requires Python 3.10 or later.\n\n## P4Runtime Controller\n\nWith Finsy, you can write a P4Runtime controller that manages multiple switches.\n\nEach switch is managed by an async `ready_handler` function. Your `ready_handler` function can read or \nupdate various P4Runtime entities in the switch. It can also create tasks to listen for \npackets or digests.\n\nWhen you write P4Runtime updates to the switch, you use a unary operator (+, -, \\~) to specify the operation:\nINSERT (+), DELETE (-) or MODIFY (\\~).\n\n```python\nasync def ready_handler(sw):\n    await sw.delete_all()\n    await sw.write(\n        [\n            # Insert multicast group with ports 1, 2, 3 and CONTROLLER.\n            +fy.P4MulticastGroupEntry(1, replicas=[1, 2, 3, 255]),\n            # Modify default table entry to flood all unmatched packets.\n            ~fy.P4TableEntry(\n                "ipv4",\n                action=fy.P4TableAction("flood"),\n                is_default_action=True,\n            ),\n        ]\n    )\n\n    async for packet in sw.read_packets():\n        print(f"{sw.name}: {packet}")\n```\n\nUse the `SwitchOptions` class to specify each switch\'s settings, including the p4info/p4blob and \n`ready_handler`. Use the `Controller` class to drive multiple switch connections. Each switch will call back\ninto your `ready_handler` function after the P4Runtime connection is established.\n\n```python\nfrom pathlib import Path\n\noptions = fy.SwitchOptions(\n    p4info=Path("hello.p4info.txt"),\n    p4blob=Path("hello.json"),\n    ready_handler=ready_handler,\n)\n\ncontroller = fy.Controller([\n    fy.Switch("sw1", "127.0.0.1:50001", options),\n    fy.Switch("sw2", "127.0.0.1:50002", options),\n    fy.Switch("sw3", "127.0.0.1:50003", options),\n])\n\nasyncio.run(controller.run())\n```\n\nIf the switch disconnects or its role changes to backup, the task running your `ready_handler` \n(and any tasks it spawned) will be cancelled and the `ready_handler` will begin again.\n\nFor more examples, see the [examples](https://github.com/byllyfish/finsy/tree/main/examples) directory.\n',
     'author': 'Bill Fisher',
     'author_email': 'william.w.fisher@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/byllyfish/finsy',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `finsy-0.8.0/PKG-INFO` & `finsy-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finsy
-Version: 0.8.0
+Version: 0.9.0
 Summary: P4Runtime Client Library
 Home-page: https://github.com/byllyfish/finsy
 License: Apache-2.0
 Author: Bill Fisher
 Author-email: william.w.fisher@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -22,42 +22,46 @@
 Requires-Dist: pylev (>=1.4.0,<2.0.0)
 Project-URL: Issue Tracker, https://github.com/byllyfish/finsy/issues
 Project-URL: Release Notes, https://github.com/byllyfish/finsy/blob/main/CHANGELOG.md
 Description-Content-Type: text/markdown
 
 # 🐟 Finsy P4Runtime Library
 
-[![pypi](https://img.shields.io/pypi/v/finsy)](https://pypi.org/project/finsy/) [![ci](https://github.com/byllyfish/finsy/actions/workflows/ci.yml/badge.svg)](https://github.com/byllyfish/finsy/actions/workflows/ci.yml) [![codecov](https://codecov.io/gh/byllyfish/finsy/branch/main/graph/badge.svg?token=8RPYWRXNGS)](https://codecov.io/gh/byllyfish/finsy)
+[![pypi](https://img.shields.io/pypi/v/finsy)](https://pypi.org/project/finsy/) [![ci](https://github.com/byllyfish/finsy/actions/workflows/ci.yml/badge.svg)](https://github.com/byllyfish/finsy/actions/workflows/ci.yml) [![codecov](https://codecov.io/gh/byllyfish/finsy/branch/main/graph/badge.svg?token=8RPYWRXNGS)](https://codecov.io/gh/byllyfish/finsy) [![docs](https://img.shields.io/badge/-docs-informational)](https://byllyfish.github.io/finsy/finsy.html)
 
 Finsy is a [P4Runtime](https://p4.org/p4-spec/p4runtime/main/P4Runtime-Spec.html) controller library written in Python using asyncio. Finsy includes support for [gNMI](https://github.com/openconfig/reference/blob/master/rpc/gnmi/gnmi-specification.md).
 
 ```python
 import asyncio
 import finsy as fy
 
 async def main():
     async with fy.Switch("sw1", "127.0.0.1:50001") as sw1:
         print(sw1.p4info)
 
 asyncio.run(main())
 ```
 
-## Multiple Switches
+## Requirements
+
+Finsy requires Python 3.10 or later.
+
+## P4Runtime Controller
 
 With Finsy, you can write a P4Runtime controller that manages multiple switches.
 
 Each switch is managed by an async `ready_handler` function. Your `ready_handler` function can read or 
 update various P4Runtime entities in the switch. It can also create tasks to listen for 
 packets or digests.
 
 When you write P4Runtime updates to the switch, you use a unary operator (+, -, \~) to specify the operation:
 INSERT (+), DELETE (-) or MODIFY (\~).
 
 ```python
-async def ready_handler(sw: fy.Switch):
+async def ready_handler(sw):
     await sw.delete_all()
     await sw.write(
         [
             # Insert multicast group with ports 1, 2, 3 and CONTROLLER.
             +fy.P4MulticastGroupEntry(1, replicas=[1, 2, 3, 255]),
             # Modify default table entry to flood all unmatched packets.
             ~fy.P4TableEntry(
```

