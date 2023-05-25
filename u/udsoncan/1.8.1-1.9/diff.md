# Comparing `tmp/udsoncan-1.8.1.tar.gz` & `tmp/udsoncan-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/udsoncan-1.8.1.tar", last modified: Sat Oct 19 09:53:04 2019, max compression
+gzip compressed data, was "dist/udsoncan-1.9.tar", last modified: Sun Nov  3 23:20:31 2019, max compression
```

## Comparing `udsoncan-1.8.1.tar` & `udsoncan-1.9.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2019-10-19 09:53:04.000000 udsoncan-1.8.1/
--rw-rw-r--   0 py        (1000) py        (1000)     3078 2019-10-19 09:53:04.000000 udsoncan-1.8.1/PKG-INFO
--rwxrwxr-x   0 py        (1000) py        (1000)     1838 2019-04-28 01:47:47.000000 udsoncan-1.8.1/README.rst
--rwxr--r--   0 py        (1000) py        (1000)       80 2019-10-19 09:53:04.000000 udsoncan-1.8.1/setup.cfg
--rwxrwxr-x   0 py        (1000) py        (1000)     1290 2019-10-19 09:52:16.000000 udsoncan-1.8.1/setup.py
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2019-10-19 09:53:04.000000 udsoncan-1.8.1/test/
--rwxrwxr-x   0 py        (1000) py        (1000)     1069 2019-08-07 02:33:43.000000 udsoncan-1.8.1/test/ClientServerTest.py
--rwxrwxr-x   0 py        (1000) py        (1000)     2438 2019-08-07 02:33:43.000000 udsoncan-1.8.1/test/ThreadableTest.py
--rwxrwxr-x   0 py        (1000) py        (1000)      177 2019-08-07 02:33:42.000000 udsoncan-1.8.1/test/UdsTest.py
--rwxrwxr-x   0 py        (1000) py        (1000)      108 2019-08-07 02:22:24.000000 udsoncan-1.8.1/test/__init__.py
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2019-10-19 09:53:04.000000 udsoncan-1.8.1/test/client/
--rw-rw-rw-   0 py        (1000) py        (1000)        0 2017-10-20 01:00:44.000000 udsoncan-1.8.1/test/client/__init__.py
--rwxrwxr-x   0 py        (1000) py        (1000)     6588 2019-08-07 02:33:46.000000 udsoncan-1.8.1/test/client/test_access_timing_parameters.py
--rwxrwxr-x   0 py        (1000) py        (1000)     3900 2019-08-07 02:33:46.000000 udsoncan-1.8.1/test/client/test_clear_dtc.py
--rwxrwxr-x   0 py        (1000) py        (1000)     5727 2019-08-07 02:33:44.000000 udsoncan-1.8.1/test/client/test_client.py
--rwxrwxr-x   0 py        (1000) py        (1000)     8335 2019-08-07 02:33:46.000000 udsoncan-1.8.1/test/client/test_communication_control.py
--rwxrwxr-x   0 py        (1000) py        (1000)     5730 2019-08-07 02:33:44.000000 udsoncan-1.8.1/test/client/test_control_dtc_setting.py
--rwxrwxr-x   0 py        (1000) py        (1000)     4844 2019-08-07 02:33:44.000000 udsoncan-1.8.1/test/client/test_diagnostic_session_control.py
--rwxrwxr-x   0 py        (1000) py        (1000)     5280 2019-08-07 02:33:45.000000 udsoncan-1.8.1/test/client/test_ecu_reset.py
--rwxrwxr-x   0 py        (1000) py        (1000)    13759 2019-08-07 02:33:45.000000 udsoncan-1.8.1/test/client/test_io_control.py
--rwxrwxr-x   0 py        (1000) py        (1000)     7573 2019-08-07 02:33:44.000000 udsoncan-1.8.1/test/client/test_link_control.py
--rwxrwxr-x   0 py        (1000) py        (1000)     9506 2019-08-07 02:33:43.000000 udsoncan-1.8.1/test/client/test_read_data_by_identifier.py
--rwxrwxr-x   0 py        (1000) py        (1000)   125048 2019-08-07 02:33:46.000000 udsoncan-1.8.1/test/client/test_read_dtc_information.py
--rwxrwxr-x   0 py        (1000) py        (1000)     6487 2019-08-07 02:33:44.000000 udsoncan-1.8.1/test/client/test_read_memory_by_address.py
--rwxrwxr-x   0 py        (1000) py        (1000)     6588 2019-08-07 02:33:44.000000 udsoncan-1.8.1/test/client/test_request_download.py
--rwxrwxr-x   0 py        (1000) py        (1000)     4699 2019-08-07 02:33:44.000000 udsoncan-1.8.1/test/client/test_request_transfer_exit.py
--rwxrwxr-x   0 py        (1000) py        (1000)     6523 2019-08-07 02:33:45.000000 udsoncan-1.8.1/test/client/test_request_upload.py
--rwxrwxr-x   0 py        (1000) py        (1000)     8232 2019-08-07 02:33:44.000000 udsoncan-1.8.1/test/client/test_routine_control.py
--rwxrwxr-x   0 py        (1000) py        (1000)    11959 2019-08-07 02:33:43.000000 udsoncan-1.8.1/test/client/test_security_access.py
--rwxrwxr-x   0 py        (1000) py        (1000)     3623 2019-08-07 02:33:46.000000 udsoncan-1.8.1/test/client/test_tester_present.py
--rwxrwxr-x   0 py        (1000) py        (1000)     5931 2019-08-07 02:33:44.000000 udsoncan-1.8.1/test/client/test_transfer_data.py
--rwxrwxr-x   0 py        (1000) py        (1000)     7154 2019-08-07 02:58:33.000000 udsoncan-1.8.1/test/client/test_write_data_by_identifier.py
--rwxrwxr-x   0 py        (1000) py        (1000)     9914 2019-08-07 02:33:44.000000 udsoncan-1.8.1/test/client/test_write_memory_by_address.py
--rwxrwxr-x   0 py        (1000) py        (1000)     1694 2019-08-07 02:33:43.000000 udsoncan-1.8.1/test/stub.py
--rwxrwxr-x   0 py        (1000) py        (1000)     7308 2019-08-07 02:33:43.000000 udsoncan-1.8.1/test/test_connection.py
--rwxrwxr-x   0 py        (1000) py        (1000)      485 2019-08-07 02:33:43.000000 udsoncan-1.8.1/test/test_definitions.py
--rwxrwxr-x   0 py        (1000) py        (1000)    19767 2019-08-07 02:33:43.000000 udsoncan-1.8.1/test/test_helper_class.py
--rwxrwxr-x   0 py        (1000) py        (1000)     4057 2019-08-07 02:33:43.000000 udsoncan-1.8.1/test/test_request.py
--rwxrwxr-x   0 py        (1000) py        (1000)     4843 2019-08-07 02:33:43.000000 udsoncan-1.8.1/test/test_response.py
--rwxrwxr-x   0 py        (1000) py        (1000)     2233 2019-08-07 02:33:43.000000 udsoncan-1.8.1/test/test_stubbed_isotpsock.py
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2019-10-19 09:53:04.000000 udsoncan-1.8.1/udsoncan/
--rwxrwxr-x   0 py        (1000) py        (1000)     5688 2019-08-07 02:33:40.000000 udsoncan-1.8.1/udsoncan/Request.py
--rwxrwxr-x   0 py        (1000) py        (1000)    10619 2019-08-07 02:33:40.000000 udsoncan-1.8.1/udsoncan/Response.py
--rwxrwxr-x   0 py        (1000) py        (1000)    48909 2019-08-07 02:33:41.000000 udsoncan-1.8.1/udsoncan/__init__.py
--rwxrwxr-x   0 py        (1000) py        (1000)    80704 2019-10-19 09:51:15.000000 udsoncan-1.8.1/udsoncan/client.py
--rwxrwxr-x   0 py        (1000) py        (1000)      725 2019-08-07 02:33:40.000000 udsoncan-1.8.1/udsoncan/configs.py
--rwxrwxr-x   0 py        (1000) py        (1000)    16751 2019-08-07 02:33:41.000000 udsoncan-1.8.1/udsoncan/connections.py
--rwxr--r--   0 py        (1000) py        (1000)     1714 2019-08-07 02:16:22.000000 udsoncan-1.8.1/udsoncan/dummy_client.py
--rwxr--r--   0 py        (1000) py        (1000)     4110 2019-08-07 02:16:23.000000 udsoncan-1.8.1/udsoncan/dummy_server.py
--rwxrwxr-x   0 py        (1000) py        (1000)     3610 2019-08-07 02:33:40.000000 udsoncan-1.8.1/udsoncan/exceptions.py
--rwxr--r--   0 py        (1000) py        (1000)     1092 2019-03-01 02:49:44.000000 udsoncan-1.8.1/udsoncan/logging.conf
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2019-10-19 09:53:04.000000 udsoncan-1.8.1/udsoncan/services/
--rwxrwxr-x   0 py        (1000) py        (1000)     3709 2019-08-07 02:33:42.000000 udsoncan-1.8.1/udsoncan/services/AccessTimingParameter.py
--rwxrwxr-x   0 py        (1000) py        (1000)     1874 2019-08-07 02:33:41.000000 udsoncan-1.8.1/udsoncan/services/ClearDiagnosticInformation.py
--rwxrwxr-x   0 py        (1000) py        (1000)     3382 2019-08-07 02:33:42.000000 udsoncan-1.8.1/udsoncan/services/CommunicationControl.py
--rwxrwxr-x   0 py        (1000) py        (1000)     2823 2019-08-07 02:33:42.000000 udsoncan-1.8.1/udsoncan/services/ControlDTCSetting.py
--rwxrwxr-x   0 py        (1000) py        (1000)     2736 2019-08-07 02:33:41.000000 udsoncan-1.8.1/udsoncan/services/DiagnosticSessionControl.py
--rwxrwxr-x   0 py        (1000) py        (1000)     1046 2019-08-07 02:33:41.000000 udsoncan-1.8.1/udsoncan/services/DynamicallyDefineDataIdentifier.py
--rwxrwxr-x   0 py        (1000) py        (1000)     3108 2019-08-07 02:33:42.000000 udsoncan-1.8.1/udsoncan/services/ECUReset.py
--rwxrwxr-x   0 py        (1000) py        (1000)    10342 2019-08-07 02:33:42.000000 udsoncan-1.8.1/udsoncan/services/InputOutputControlByIdentifier.py
--rwxrwxr-x   0 py        (1000) py        (1000)     4259 2019-08-07 02:33:42.000000 udsoncan-1.8.1/udsoncan/services/LinkControl.py
--rwxrwxr-x   0 py        (1000) py        (1000)    32046 2019-08-07 02:33:42.000000 udsoncan-1.8.1/udsoncan/services/ReadDTCInformation.py
--rwxrwxr-x   0 py        (1000) py        (1000)     5712 2019-08-07 02:33:41.000000 udsoncan-1.8.1/udsoncan/services/ReadDataByIdentifier.py
--rwxrwxr-x   0 py        (1000) py        (1000)      948 2019-08-07 02:33:42.000000 udsoncan-1.8.1/udsoncan/services/ReadDataByPeriodicIdentifier.py
--rwxrwxr-x   0 py        (1000) py        (1000)     2517 2019-08-07 02:33:42.000000 udsoncan-1.8.1/udsoncan/services/ReadMemoryByAddress.py
--rwxrwxr-x   0 py        (1000) py        (1000)      946 2019-08-07 02:33:42.000000 udsoncan-1.8.1/udsoncan/services/ReadScalingDataByIdentifier.py
--rwxrwxr-x   0 py        (1000) py        (1000)     4087 2019-08-07 02:33:42.000000 udsoncan-1.8.1/udsoncan/services/RequestDownload.py
--rwxrwxr-x   0 py        (1000) py        (1000)     1837 2019-08-07 02:33:42.000000 udsoncan-1.8.1/udsoncan/services/RequestTransferExit.py
--rwxrwxr-x   0 py        (1000) py        (1000)     4040 2019-08-07 02:33:42.000000 udsoncan-1.8.1/udsoncan/services/RequestUpload.py
--rwxrwxr-x   0 py        (1000) py        (1000)      925 2019-08-07 02:33:42.000000 udsoncan-1.8.1/udsoncan/services/ResponseOnEvent.py
--rwxrwxr-x   0 py        (1000) py        (1000)     3767 2019-08-07 02:33:41.000000 udsoncan-1.8.1/udsoncan/services/RoutineControl.py
--rwxrwxr-x   0 py        (1000) py        (1000)     2391 2019-08-07 02:33:41.000000 udsoncan-1.8.1/udsoncan/services/SecuredDataTransmission.py
--rwxrwxr-x   0 py        (1000) py        (1000)     4382 2019-08-07 02:33:41.000000 udsoncan-1.8.1/udsoncan/services/SecurityAccess.py
--rwxrwxr-x   0 py        (1000) py        (1000)     1629 2019-08-07 02:33:41.000000 udsoncan-1.8.1/udsoncan/services/TesterPresent.py
--rwxrwxr-x   0 py        (1000) py        (1000)     3255 2019-08-07 02:33:41.000000 udsoncan-1.8.1/udsoncan/services/TransferData.py
--rwxrwxr-x   0 py        (1000) py        (1000)     3202 2019-08-07 03:09:51.000000 udsoncan-1.8.1/udsoncan/services/WriteDataByIdentifier.py
--rwxrwxr-x   0 py        (1000) py        (1000)     4318 2019-08-07 02:33:41.000000 udsoncan-1.8.1/udsoncan/services/WriteMemoryByAddress.py
--rwxrwxr-x   0 py        (1000) py        (1000)     9587 2019-08-07 02:33:42.000000 udsoncan-1.8.1/udsoncan/services/__init__.py
-drwxrwxr-x   0 py        (1000) py        (1000)        0 2019-10-19 09:53:04.000000 udsoncan-1.8.1/udsoncan.egg-info/
--rw-rw-r--   0 py        (1000) py        (1000)     3078 2019-10-19 09:53:04.000000 udsoncan-1.8.1/udsoncan.egg-info/PKG-INFO
--rw-rw-r--   0 py        (1000) py        (1000)     2500 2019-10-19 09:53:04.000000 udsoncan-1.8.1/udsoncan.egg-info/SOURCES.txt
--rw-rw-r--   0 py        (1000) py        (1000)        1 2019-10-19 09:53:04.000000 udsoncan-1.8.1/udsoncan.egg-info/dependency_links.txt
--rw-rw-r--   0 py        (1000) py        (1000)       14 2019-10-19 09:53:04.000000 udsoncan-1.8.1/udsoncan.egg-info/top_level.txt
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2019-11-03 23:20:31.000000 udsoncan-1.9/
+-rw-rw-r--   0 py        (1000) py        (1000)     3074 2019-11-03 23:20:31.000000 udsoncan-1.9/PKG-INFO
+-rwxrwxr-x   0 py        (1000) py        (1000)     1838 2019-04-28 01:47:47.000000 udsoncan-1.9/README.rst
+-rwxr--r--   0 py        (1000) py        (1000)       80 2019-11-03 23:20:31.000000 udsoncan-1.9/setup.cfg
+-rwxrwxr-x   0 py        (1000) py        (1000)     1286 2019-11-03 23:14:22.000000 udsoncan-1.9/setup.py
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2019-11-03 23:20:31.000000 udsoncan-1.9/test/
+-rwxrwxr-x   0 py        (1000) py        (1000)     1069 2019-08-07 02:33:43.000000 udsoncan-1.9/test/ClientServerTest.py
+-rwxrwxr-x   0 py        (1000) py        (1000)     2438 2019-08-07 02:33:43.000000 udsoncan-1.9/test/ThreadableTest.py
+-rwxrwxr-x   0 py        (1000) py        (1000)      177 2019-08-07 02:33:42.000000 udsoncan-1.9/test/UdsTest.py
+-rwxrwxr-x   0 py        (1000) py        (1000)      108 2019-08-07 02:22:24.000000 udsoncan-1.9/test/__init__.py
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2019-11-03 23:20:31.000000 udsoncan-1.9/test/client/
+-rw-rw-rw-   0 py        (1000) py        (1000)        0 2017-10-20 01:00:44.000000 udsoncan-1.9/test/client/__init__.py
+-rwxrwxr-x   0 py        (1000) py        (1000)     6588 2019-08-07 02:33:46.000000 udsoncan-1.9/test/client/test_access_timing_parameters.py
+-rwxrwxr-x   0 py        (1000) py        (1000)     3900 2019-08-07 02:33:46.000000 udsoncan-1.9/test/client/test_clear_dtc.py
+-rwxrwxr-x   0 py        (1000) py        (1000)     6834 2019-10-31 01:50:24.000000 udsoncan-1.9/test/client/test_client.py
+-rwxrwxr-x   0 py        (1000) py        (1000)     8335 2019-08-07 02:33:46.000000 udsoncan-1.9/test/client/test_communication_control.py
+-rwxrwxr-x   0 py        (1000) py        (1000)     5730 2019-08-07 02:33:44.000000 udsoncan-1.9/test/client/test_control_dtc_setting.py
+-rwxrwxr-x   0 py        (1000) py        (1000)     4844 2019-08-07 02:33:44.000000 udsoncan-1.9/test/client/test_diagnostic_session_control.py
+-rwxrwxr-x   0 py        (1000) py        (1000)     5280 2019-08-07 02:33:45.000000 udsoncan-1.9/test/client/test_ecu_reset.py
+-rwxrwxr-x   0 py        (1000) py        (1000)    13759 2019-08-07 02:33:45.000000 udsoncan-1.9/test/client/test_io_control.py
+-rwxrwxr-x   0 py        (1000) py        (1000)     7573 2019-08-07 02:33:44.000000 udsoncan-1.9/test/client/test_link_control.py
+-rwxrwxr-x   0 py        (1000) py        (1000)     9506 2019-08-07 02:33:43.000000 udsoncan-1.9/test/client/test_read_data_by_identifier.py
+-rwxrwxr-x   0 py        (1000) py        (1000)   125048 2019-08-07 02:33:46.000000 udsoncan-1.9/test/client/test_read_dtc_information.py
+-rwxrwxr-x   0 py        (1000) py        (1000)     6487 2019-08-07 02:33:44.000000 udsoncan-1.9/test/client/test_read_memory_by_address.py
+-rwxrwxr-x   0 py        (1000) py        (1000)     6588 2019-08-07 02:33:44.000000 udsoncan-1.9/test/client/test_request_download.py
+-rwxrwxr-x   0 py        (1000) py        (1000)     4699 2019-08-07 02:33:44.000000 udsoncan-1.9/test/client/test_request_transfer_exit.py
+-rwxrwxr-x   0 py        (1000) py        (1000)     6523 2019-08-07 02:33:45.000000 udsoncan-1.9/test/client/test_request_upload.py
+-rwxrwxr-x   0 py        (1000) py        (1000)     8232 2019-08-07 02:33:44.000000 udsoncan-1.9/test/client/test_routine_control.py
+-rwxrwxr-x   0 py        (1000) py        (1000)    11959 2019-08-07 02:33:43.000000 udsoncan-1.9/test/client/test_security_access.py
+-rwxrwxr-x   0 py        (1000) py        (1000)     3623 2019-08-07 02:33:46.000000 udsoncan-1.9/test/client/test_tester_present.py
+-rwxrwxr-x   0 py        (1000) py        (1000)     5931 2019-08-07 02:33:44.000000 udsoncan-1.9/test/client/test_transfer_data.py
+-rwxrwxr-x   0 py        (1000) py        (1000)     7154 2019-08-07 02:58:33.000000 udsoncan-1.9/test/client/test_write_data_by_identifier.py
+-rwxrwxr-x   0 py        (1000) py        (1000)     9914 2019-08-07 02:33:44.000000 udsoncan-1.9/test/client/test_write_memory_by_address.py
+-rwxrwxr-x   0 py        (1000) py        (1000)     1694 2019-08-07 02:33:43.000000 udsoncan-1.9/test/stub.py
+-rwxrwxr-x   0 py        (1000) py        (1000)     7308 2019-08-07 02:33:43.000000 udsoncan-1.9/test/test_connection.py
+-rwxrwxr-x   0 py        (1000) py        (1000)      485 2019-08-07 02:33:43.000000 udsoncan-1.9/test/test_definitions.py
+-rwxrwxr-x   0 py        (1000) py        (1000)    19767 2019-08-07 02:33:43.000000 udsoncan-1.9/test/test_helper_class.py
+-rwxrwxr-x   0 py        (1000) py        (1000)     4057 2019-08-07 02:33:43.000000 udsoncan-1.9/test/test_request.py
+-rwxrwxr-x   0 py        (1000) py        (1000)     4843 2019-08-07 02:33:43.000000 udsoncan-1.9/test/test_response.py
+-rwxrwxr-x   0 py        (1000) py        (1000)     2233 2019-08-07 02:33:43.000000 udsoncan-1.9/test/test_stubbed_isotpsock.py
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2019-11-03 23:20:31.000000 udsoncan-1.9/udsoncan/
+-rwxrwxr-x   0 py        (1000) py        (1000)     5688 2019-08-07 02:33:40.000000 udsoncan-1.9/udsoncan/Request.py
+-rwxrwxr-x   0 py        (1000) py        (1000)    10619 2019-08-07 02:33:40.000000 udsoncan-1.9/udsoncan/Response.py
+-rwxrwxr-x   0 py        (1000) py        (1000)    48909 2019-08-07 02:33:41.000000 udsoncan-1.9/udsoncan/__init__.py
+-rwxrwxr-x   0 py        (1000) py        (1000)    81519 2019-10-31 01:49:19.000000 udsoncan-1.9/udsoncan/client.py
+-rwxrwxr-x   0 py        (1000) py        (1000)      725 2019-08-07 02:33:40.000000 udsoncan-1.9/udsoncan/configs.py
+-rwxrwxr-x   0 py        (1000) py        (1000)    16751 2019-08-07 02:33:41.000000 udsoncan-1.9/udsoncan/connections.py
+-rwxr--r--   0 py        (1000) py        (1000)     1714 2019-08-07 02:16:22.000000 udsoncan-1.9/udsoncan/dummy_client.py
+-rwxr--r--   0 py        (1000) py        (1000)     4110 2019-08-07 02:16:23.000000 udsoncan-1.9/udsoncan/dummy_server.py
+-rwxrwxr-x   0 py        (1000) py        (1000)     3610 2019-08-07 02:33:40.000000 udsoncan-1.9/udsoncan/exceptions.py
+-rwxr--r--   0 py        (1000) py        (1000)     1092 2019-10-31 01:44:08.000000 udsoncan-1.9/udsoncan/logging.conf
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2019-11-03 23:20:31.000000 udsoncan-1.9/udsoncan/services/
+-rwxrwxr-x   0 py        (1000) py        (1000)     3709 2019-08-07 02:33:42.000000 udsoncan-1.9/udsoncan/services/AccessTimingParameter.py
+-rwxrwxr-x   0 py        (1000) py        (1000)     1874 2019-08-07 02:33:41.000000 udsoncan-1.9/udsoncan/services/ClearDiagnosticInformation.py
+-rwxrwxr-x   0 py        (1000) py        (1000)     3382 2019-08-07 02:33:42.000000 udsoncan-1.9/udsoncan/services/CommunicationControl.py
+-rwxrwxr-x   0 py        (1000) py        (1000)     2823 2019-08-07 02:33:42.000000 udsoncan-1.9/udsoncan/services/ControlDTCSetting.py
+-rwxrwxr-x   0 py        (1000) py        (1000)     2736 2019-08-07 02:33:41.000000 udsoncan-1.9/udsoncan/services/DiagnosticSessionControl.py
+-rwxrwxr-x   0 py        (1000) py        (1000)     1046 2019-08-07 02:33:41.000000 udsoncan-1.9/udsoncan/services/DynamicallyDefineDataIdentifier.py
+-rwxrwxr-x   0 py        (1000) py        (1000)     3108 2019-08-07 02:33:42.000000 udsoncan-1.9/udsoncan/services/ECUReset.py
+-rwxrwxr-x   0 py        (1000) py        (1000)    10342 2019-08-07 02:33:42.000000 udsoncan-1.9/udsoncan/services/InputOutputControlByIdentifier.py
+-rwxrwxr-x   0 py        (1000) py        (1000)     4259 2019-08-07 02:33:42.000000 udsoncan-1.9/udsoncan/services/LinkControl.py
+-rwxrwxr-x   0 py        (1000) py        (1000)    32046 2019-08-07 02:33:42.000000 udsoncan-1.9/udsoncan/services/ReadDTCInformation.py
+-rwxrwxr-x   0 py        (1000) py        (1000)     5712 2019-08-07 02:33:41.000000 udsoncan-1.9/udsoncan/services/ReadDataByIdentifier.py
+-rwxrwxr-x   0 py        (1000) py        (1000)      948 2019-08-07 02:33:42.000000 udsoncan-1.9/udsoncan/services/ReadDataByPeriodicIdentifier.py
+-rwxrwxr-x   0 py        (1000) py        (1000)     2517 2019-08-07 02:33:42.000000 udsoncan-1.9/udsoncan/services/ReadMemoryByAddress.py
+-rwxrwxr-x   0 py        (1000) py        (1000)      946 2019-08-07 02:33:42.000000 udsoncan-1.9/udsoncan/services/ReadScalingDataByIdentifier.py
+-rwxrwxr-x   0 py        (1000) py        (1000)     4087 2019-08-07 02:33:42.000000 udsoncan-1.9/udsoncan/services/RequestDownload.py
+-rwxrwxr-x   0 py        (1000) py        (1000)     1837 2019-08-07 02:33:42.000000 udsoncan-1.9/udsoncan/services/RequestTransferExit.py
+-rwxrwxr-x   0 py        (1000) py        (1000)     4040 2019-08-07 02:33:42.000000 udsoncan-1.9/udsoncan/services/RequestUpload.py
+-rwxrwxr-x   0 py        (1000) py        (1000)      925 2019-08-07 02:33:42.000000 udsoncan-1.9/udsoncan/services/ResponseOnEvent.py
+-rwxrwxr-x   0 py        (1000) py        (1000)     3767 2019-08-07 02:33:41.000000 udsoncan-1.9/udsoncan/services/RoutineControl.py
+-rwxrwxr-x   0 py        (1000) py        (1000)     2391 2019-08-07 02:33:41.000000 udsoncan-1.9/udsoncan/services/SecuredDataTransmission.py
+-rwxrwxr-x   0 py        (1000) py        (1000)     4382 2019-08-07 02:33:41.000000 udsoncan-1.9/udsoncan/services/SecurityAccess.py
+-rwxrwxr-x   0 py        (1000) py        (1000)     1629 2019-08-07 02:33:41.000000 udsoncan-1.9/udsoncan/services/TesterPresent.py
+-rwxrwxr-x   0 py        (1000) py        (1000)     3255 2019-08-07 02:33:41.000000 udsoncan-1.9/udsoncan/services/TransferData.py
+-rwxrwxr-x   0 py        (1000) py        (1000)     3202 2019-08-07 03:09:51.000000 udsoncan-1.9/udsoncan/services/WriteDataByIdentifier.py
+-rwxrwxr-x   0 py        (1000) py        (1000)     4318 2019-08-07 02:33:41.000000 udsoncan-1.9/udsoncan/services/WriteMemoryByAddress.py
+-rwxrwxr-x   0 py        (1000) py        (1000)     9587 2019-08-07 02:33:42.000000 udsoncan-1.9/udsoncan/services/__init__.py
+drwxrwxr-x   0 py        (1000) py        (1000)        0 2019-11-03 23:20:31.000000 udsoncan-1.9/udsoncan.egg-info/
+-rw-rw-r--   0 py        (1000) py        (1000)     3074 2019-11-03 23:20:31.000000 udsoncan-1.9/udsoncan.egg-info/PKG-INFO
+-rw-rw-r--   0 py        (1000) py        (1000)     2500 2019-11-03 23:20:31.000000 udsoncan-1.9/udsoncan.egg-info/SOURCES.txt
+-rw-rw-r--   0 py        (1000) py        (1000)        1 2019-11-03 23:20:31.000000 udsoncan-1.9/udsoncan.egg-info/dependency_links.txt
+-rw-rw-r--   0 py        (1000) py        (1000)       14 2019-11-03 23:20:31.000000 udsoncan-1.9/udsoncan.egg-info/top_level.txt
```

### Comparing `udsoncan-1.8.1/PKG-INFO` & `udsoncan-1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.2
 Name: udsoncan
-Version: 1.8.1
+Version: 1.9
 Summary: Implementation of the Unified Diagnostic Service (UDS) protocol (ISO-14229) used in the automotive industry.
 Home-page: https://github.com/pylessard/python-udsoncan
 Author: Pier-Yves Lessard
 Author-email: py.lessard@gmail.com
 License: MIT
-Download-URL: https://github.com/pylessard/python-udsoncan/archive/v1.8.1.tar.gz
+Download-URL: https://github.com/pylessard/python-udsoncan/archive/v1.9.tar.gz
 Description: python-udsoncan
         ###############
         
         This project is an implementation of the Unified Diagnostic Services (UDS) protocol defined by ISO-14229 written in Python 3. The code is published under MIT license on GitHub (pylessard/python-udsoncan).
         
         Documentation
         -------------
```

### Comparing `udsoncan-1.8.1/README.rst` & `udsoncan-1.9/README.rst`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/setup.py` & `udsoncan-1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 
 setup(
     name = 'udsoncan',
   packages = find_packages(exclude=['test']),
   package_data={
       '': ['*.conf'],
   },
-  version = '1.8.1',
+  version = '1.9',
   description = 'Implementation of the Unified Diagnostic Service (UDS) protocol (ISO-14229) used in the automotive industry.',
   long_description=long_description,
   author = 'Pier-Yves Lessard',
   author_email = 'py.lessard@gmail.com',
   license='MIT',
   url = 'https://github.com/pylessard/python-udsoncan',
-  download_url = 'https://github.com/pylessard/python-udsoncan/archive/v1.8.1.tar.gz',
+  download_url = 'https://github.com/pylessard/python-udsoncan/archive/v1.9.tar.gz',
   keywords = ['uds', '14229', 'iso-14229', 'diagnostic', 'automotive'], 
   python_requires='>=3.0',
   classifiers = [
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Development Status :: 4 - Beta",
         "Operating System :: POSIX :: Linux",
```

### Comparing `udsoncan-1.8.1/test/ClientServerTest.py` & `udsoncan-1.9/test/ClientServerTest.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/test/ThreadableTest.py` & `udsoncan-1.9/test/ThreadableTest.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/test/client/test_access_timing_parameters.py` & `udsoncan-1.9/test/client/test_access_timing_parameters.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/test/client/test_clear_dtc.py` & `udsoncan-1.9/test/client/test_clear_dtc.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/test/client/test_client.py` & `udsoncan-1.9/test/client/test_client.py`

 * *Files 17% similar despite different names*

```diff
@@ -103,7 +103,33 @@
         except TimeoutException as e:
             self.assertIsNotNone(self.udsclient.last_response, 'Client never received the PendingResponse message')
             self.completed = True
             diff = time.time() - t1
             self.assertGreater(diff, timeout, 'Timeout raised after %.3f seconds when it should be %.3f sec' % (diff, timeout))
             self.assertLess(diff, timeout+0.5, 'Timeout raised after %.3f seconds when it should be %.3f sec' % (diff, timeout))
 
+
+    def test_payload_override_literal(self):
+        request = self.conn.touserqueue.get(timeout=0.2)
+        self.assertEqual(request, b'\x12\x34\x56\x78')
+        self.conn.fromuserqueue.put(b"\x7E\x00")
+
+    def _test_payload_override_literal(self):
+        req = Request(service = services.TesterPresent, subfunction=0) 
+        with self.udsclient.payload_override(b'\x12\x34\x56\x78'):
+            response = self.udsclient.send_request(req)
+            self.assertEqual(response.original_payload, b'\x7E\x00')
+
+
+    def test_payload_override_func(self):
+        request = self.conn.touserqueue.get(timeout=0.2)
+        self.assertEqual(request, b'\x99\x88\x77\x66')
+        self.conn.fromuserqueue.put(b"\x7E\x00")
+
+    def _test_payload_override_func(self):
+        def func(payload):
+            return b'\x99\x88\x77\x66'
+
+        req = Request(service = services.TesterPresent, subfunction=0) 
+        with self.udsclient.payload_override(func):
+            response = self.udsclient.send_request(req)
+            self.assertEqual(response.original_payload, b'\x7E\x00')
```

### Comparing `udsoncan-1.8.1/test/client/test_communication_control.py` & `udsoncan-1.9/test/client/test_communication_control.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/test/client/test_control_dtc_setting.py` & `udsoncan-1.9/test/client/test_control_dtc_setting.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/test/client/test_diagnostic_session_control.py` & `udsoncan-1.9/test/client/test_diagnostic_session_control.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/test/client/test_ecu_reset.py` & `udsoncan-1.9/test/client/test_ecu_reset.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/test/client/test_io_control.py` & `udsoncan-1.9/test/client/test_io_control.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/test/client/test_link_control.py` & `udsoncan-1.9/test/client/test_link_control.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/test/client/test_read_data_by_identifier.py` & `udsoncan-1.9/test/client/test_read_data_by_identifier.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/test/client/test_read_dtc_information.py` & `udsoncan-1.9/test/client/test_read_dtc_information.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/test/client/test_read_memory_by_address.py` & `udsoncan-1.9/test/client/test_read_memory_by_address.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/test/client/test_request_download.py` & `udsoncan-1.9/test/client/test_request_download.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/test/client/test_request_transfer_exit.py` & `udsoncan-1.9/test/client/test_request_transfer_exit.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/test/client/test_request_upload.py` & `udsoncan-1.9/test/client/test_request_upload.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/test/client/test_routine_control.py` & `udsoncan-1.9/test/client/test_routine_control.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/test/client/test_security_access.py` & `udsoncan-1.9/test/client/test_security_access.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/test/client/test_tester_present.py` & `udsoncan-1.9/test/client/test_tester_present.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/test/client/test_transfer_data.py` & `udsoncan-1.9/test/client/test_transfer_data.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/test/client/test_write_data_by_identifier.py` & `udsoncan-1.9/test/client/test_write_data_by_identifier.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/test/client/test_write_memory_by_address.py` & `udsoncan-1.9/test/client/test_write_memory_by_address.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/test/stub.py` & `udsoncan-1.9/test/stub.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/test/test_connection.py` & `udsoncan-1.9/test/test_connection.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/test/test_helper_class.py` & `udsoncan-1.9/test/test_helper_class.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/test/test_request.py` & `udsoncan-1.9/test/test_request.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/test/test_response.py` & `udsoncan-1.9/test/test_response.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/test/test_stubbed_isotpsock.py` & `udsoncan-1.9/test/test_stubbed_isotpsock.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/udsoncan/Request.py` & `udsoncan-1.9/udsoncan/Request.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/udsoncan/Response.py` & `udsoncan-1.9/udsoncan/Response.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/udsoncan/__init__.py` & `udsoncan-1.9/udsoncan/__init__.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/udsoncan/client.py` & `udsoncan-1.9/udsoncan/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,22 +33,47 @@
         def __enter__(self):
             self.enabled = True
             return self
 
         def __exit__(self, type, value, traceback):
             self.enabled = False
 
+    class PayloadOverrider:
+        def __init__(self):
+            self.modifier = None
+            self.enabled = False
+
+        def __enter__(self):
+            self.enabled = True
+            return self
+
+        def __exit__(self, type, value, traceback):
+            self.modifier = None
+            self.enabled = False
+
+        def __call__(self, modifier):
+            self.modifier = modifier
+            return self
+
+        def get_overrided_payload(self, original_payload):
+            if callable(self.modifier):
+                return self.modifier(original_payload)
+            else:
+                return self.modifier
+
+
     def __init__(self, conn, config=default_client_config, request_timeout=None):
         self.conn = conn
         self.config = dict(config) # Makes a copy of given configuration
 
         #For backward compatibility
         if request_timeout is not None:
             self.config['request_timeout'] = request_timeout
         self.suppress_positive_response = Client.SuppressPositiveResponse()
+        self.payload_override = Client.PayloadOverrider()
         self.last_response = None
 
         self.refresh_config()
 
     def __enter__(self):
         self.open()
         return self
@@ -1431,14 +1456,17 @@
         override_suppress_positive_response = False
         if self.suppress_positive_response.enabled == True and request.service.use_subfunction():
             payload = request.get_payload(suppress_positive_response=True)
             override_suppress_positive_response = True
         else:
             payload = request.get_payload()
 
+        if self.payload_override.enabled:
+            payload = self.payload_override.get_overrided_payload(payload)
+
         if self.suppress_positive_response.enabled and not request.service.use_subfunction():
             self.logger.warning('SuppressPositiveResponse cannot be used for service %s. Ignoring' % (request.service.get_name()))
 
         self.conn.send(payload)
 
         if request.suppress_positive_response  or override_suppress_positive_response:
             return
```

### Comparing `udsoncan-1.8.1/udsoncan/configs.py` & `udsoncan-1.9/udsoncan/configs.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/udsoncan/connections.py` & `udsoncan-1.9/udsoncan/connections.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/udsoncan/dummy_client.py` & `udsoncan-1.9/udsoncan/dummy_client.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/udsoncan/dummy_server.py` & `udsoncan-1.9/udsoncan/dummy_server.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/udsoncan/exceptions.py` & `udsoncan-1.9/udsoncan/exceptions.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/udsoncan/logging.conf` & `udsoncan-1.9/udsoncan/logging.conf`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/udsoncan/services/AccessTimingParameter.py` & `udsoncan-1.9/udsoncan/services/AccessTimingParameter.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/udsoncan/services/ClearDiagnosticInformation.py` & `udsoncan-1.9/udsoncan/services/ClearDiagnosticInformation.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/udsoncan/services/CommunicationControl.py` & `udsoncan-1.9/udsoncan/services/CommunicationControl.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/udsoncan/services/ControlDTCSetting.py` & `udsoncan-1.9/udsoncan/services/ControlDTCSetting.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/udsoncan/services/DiagnosticSessionControl.py` & `udsoncan-1.9/udsoncan/services/DiagnosticSessionControl.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/udsoncan/services/DynamicallyDefineDataIdentifier.py` & `udsoncan-1.9/udsoncan/services/DynamicallyDefineDataIdentifier.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/udsoncan/services/ECUReset.py` & `udsoncan-1.9/udsoncan/services/ECUReset.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/udsoncan/services/InputOutputControlByIdentifier.py` & `udsoncan-1.9/udsoncan/services/InputOutputControlByIdentifier.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/udsoncan/services/LinkControl.py` & `udsoncan-1.9/udsoncan/services/LinkControl.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/udsoncan/services/ReadDTCInformation.py` & `udsoncan-1.9/udsoncan/services/ReadDTCInformation.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/udsoncan/services/ReadDataByIdentifier.py` & `udsoncan-1.9/udsoncan/services/ReadDataByIdentifier.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/udsoncan/services/ReadDataByPeriodicIdentifier.py` & `udsoncan-1.9/udsoncan/services/ReadDataByPeriodicIdentifier.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/udsoncan/services/ReadMemoryByAddress.py` & `udsoncan-1.9/udsoncan/services/ReadMemoryByAddress.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/udsoncan/services/ReadScalingDataByIdentifier.py` & `udsoncan-1.9/udsoncan/services/ReadScalingDataByIdentifier.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/udsoncan/services/RequestDownload.py` & `udsoncan-1.9/udsoncan/services/RequestDownload.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/udsoncan/services/RequestTransferExit.py` & `udsoncan-1.9/udsoncan/services/RequestTransferExit.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/udsoncan/services/RequestUpload.py` & `udsoncan-1.9/udsoncan/services/RequestUpload.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/udsoncan/services/ResponseOnEvent.py` & `udsoncan-1.9/udsoncan/services/ResponseOnEvent.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/udsoncan/services/RoutineControl.py` & `udsoncan-1.9/udsoncan/services/RoutineControl.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/udsoncan/services/SecuredDataTransmission.py` & `udsoncan-1.9/udsoncan/services/SecuredDataTransmission.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/udsoncan/services/SecurityAccess.py` & `udsoncan-1.9/udsoncan/services/SecurityAccess.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/udsoncan/services/TesterPresent.py` & `udsoncan-1.9/udsoncan/services/TesterPresent.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/udsoncan/services/TransferData.py` & `udsoncan-1.9/udsoncan/services/TransferData.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/udsoncan/services/WriteDataByIdentifier.py` & `udsoncan-1.9/udsoncan/services/WriteDataByIdentifier.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/udsoncan/services/WriteMemoryByAddress.py` & `udsoncan-1.9/udsoncan/services/WriteMemoryByAddress.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/udsoncan/services/__init__.py` & `udsoncan-1.9/udsoncan/services/__init__.py`

 * *Files identical despite different names*

### Comparing `udsoncan-1.8.1/udsoncan.egg-info/PKG-INFO` & `udsoncan-1.9/udsoncan.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.2
 Name: udsoncan
-Version: 1.8.1
+Version: 1.9
 Summary: Implementation of the Unified Diagnostic Service (UDS) protocol (ISO-14229) used in the automotive industry.
 Home-page: https://github.com/pylessard/python-udsoncan
 Author: Pier-Yves Lessard
 Author-email: py.lessard@gmail.com
 License: MIT
-Download-URL: https://github.com/pylessard/python-udsoncan/archive/v1.8.1.tar.gz
+Download-URL: https://github.com/pylessard/python-udsoncan/archive/v1.9.tar.gz
 Description: python-udsoncan
         ###############
         
         This project is an implementation of the Unified Diagnostic Services (UDS) protocol defined by ISO-14229 written in Python 3. The code is published under MIT license on GitHub (pylessard/python-udsoncan).
         
         Documentation
         -------------
```

### Comparing `udsoncan-1.8.1/udsoncan.egg-info/SOURCES.txt` & `udsoncan-1.9/udsoncan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

