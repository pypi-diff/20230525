# Comparing `tmp/ar_ex_sys_worker-1.6.23-py3-none-any.whl.zip` & `tmp/ar_ex_sys_worker-1.6.24-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 16247 bytes, number of entries: 11
+Zip file size: 16237 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Feb-14 05:51 ar_external_sys_worker/__init__.py
 -rw-rw-rw-  2.0 fat    27525 b- defN 23-May-12 05:03 ar_external_sys_worker/main.py
--rw-rw-rw-  2.0 fat    19932 b- defN 23-May-15 07:51 ar_external_sys_worker/mixins.py
+-rw-rw-rw-  2.0 fat    19928 b- defN 23-May-25 14:07 ar_external_sys_worker/mixins.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Feb-14 05:52 ar_external_sys_worker/tests/__init__.py
 -rw-rw-rw-  2.0 fat    11225 b- defN 23-Apr-28 12:19 ar_external_sys_worker/tests/main_test.py
 -rw-rw-rw-  2.0 fat     1107 b- defN 23-Apr-25 11:47 ar_external_sys_worker/tests/mixins_test.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-May-15 07:52 ar_ex_sys_worker-1.6.23.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      344 b- defN 23-May-15 07:52 ar_ex_sys_worker-1.6.23.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-15 07:52 ar_ex_sys_worker-1.6.23.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       23 b- defN 23-May-15 07:52 ar_ex_sys_worker-1.6.23.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      994 b- defN 23-May-15 07:52 ar_ex_sys_worker-1.6.23.dist-info/RECORD
-11 files, 62333 bytes uncompressed, 14531 bytes compressed:  76.7%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-May-25 14:08 ar_ex_sys_worker-1.6.24.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      344 b- defN 23-May-25 14:08 ar_ex_sys_worker-1.6.24.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-25 14:08 ar_ex_sys_worker-1.6.24.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       23 b- defN 23-May-25 14:08 ar_ex_sys_worker-1.6.24.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      994 b- defN 23-May-25 14:08 ar_ex_sys_worker-1.6.24.dist-info/RECORD
+11 files, 62329 bytes uncompressed, 14521 bytes compressed:  76.7%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: ar_external_sys_worker/tests/main_test.py
 Comment: 
 
 Filename: ar_external_sys_worker/tests/mixins_test.py
 Comment: 
 
-Filename: ar_ex_sys_worker-1.6.23.dist-info/LICENSE
+Filename: ar_ex_sys_worker-1.6.24.dist-info/LICENSE
 Comment: 
 
-Filename: ar_ex_sys_worker-1.6.23.dist-info/METADATA
+Filename: ar_ex_sys_worker-1.6.24.dist-info/METADATA
 Comment: 
 
-Filename: ar_ex_sys_worker-1.6.23.dist-info/WHEEL
+Filename: ar_ex_sys_worker-1.6.24.dist-info/WHEEL
 Comment: 
 
-Filename: ar_ex_sys_worker-1.6.23.dist-info/top_level.txt
+Filename: ar_ex_sys_worker-1.6.24.dist-info/top_level.txt
 Comment: 
 
-Filename: ar_ex_sys_worker-1.6.23.dist-info/RECORD
+Filename: ar_ex_sys_worker-1.6.24.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ar_external_sys_worker/mixins.py

```diff
@@ -396,18 +396,18 @@
                   "oc.changing as changing_comm, oc.closing as closing_comm," \
                   "oc.single as single_comm, " \
                   "dro.owner as polygon_id, ai.number as rfid, rri.route_num," \
                   "rri.containers_plan, rri.containers_fact, ra.alerts," \
                   "pol_objects.name as pol_object," \
                   "aprm.number as act_number, acts_packages.name as package_name " \
                   "FROM records r " \
-                  "INNER JOIN clients carriers ON (r.carrier=carriers.id) " \
-                  "INNER JOIN clients ON (r.client_id=clients.id) " \
-                  "INNER JOIN trash_cats tc ON (r.trash_cat=tc.id) " \
-                  "INNER JOIN trash_types tt ON (r.trash_type=tt.id) " \
+                  "LEFT JOIN clients carriers ON (r.carrier=carriers.id) " \
+                  "LEFT JOIN clients ON (r.client_id=clients.id) " \
+                  "LEFT JOIN trash_cats tc ON (r.trash_cat=tc.id) " \
+                  "LEFT JOIN trash_types tt ON (r.trash_type=tt.id) " \
                   "LEFT JOIN operator_comments oc ON (r.id=oc.record_id) " \
                   "LEFT JOIN auto a ON (a.id=r.auto) " \
                   "LEFT JOIN clients_juridical_info carrier_cji ON (carrier_cji.client_id=carriers.id) " \
                   "LEFT JOIN clients_juridical_info client_cji ON (client_cji.client_id=clients.id) " \
                   "LEFT JOIN ex_sys_data_send_reports esdsr ON (esdsr.local_id = r.id)" \
                   "LEFT JOIN duo_records_owning dro on r.id = dro.record " \
                   "LEFT JOIN auto_idents ai ON ai.id=a.identifier " \
```

## Comparing `ar_ex_sys_worker-1.6.23.dist-info/LICENSE` & `ar_ex_sys_worker-1.6.24.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ar_ex_sys_worker-1.6.23.dist-info/RECORD` & `ar_ex_sys_worker-1.6.24.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ar_external_sys_worker/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ar_external_sys_worker/main.py,sha256=06JgXXUu4RQ69guazXnYhKIAJmHhm4Z1SXaqs1PAfbg,27525
-ar_external_sys_worker/mixins.py,sha256=yGwnnP7QI14J7JvnIdCI0j3STAvCZ_LbQe6oFmwMVq8,19932
+ar_external_sys_worker/mixins.py,sha256=UXagTBmWlwPwMVhgjZk8WKIShc__Lm9q4r7AsswA-uQ,19928
 ar_external_sys_worker/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ar_external_sys_worker/tests/main_test.py,sha256=eOqy3_5sPoq7knV5fjESJ6FVWEXehwSOLTd8qXckdXw,11225
 ar_external_sys_worker/tests/mixins_test.py,sha256=NTPOm74h7bL5ra_acU3AxLgDhn75waGOGKtbkkGSxoc,1107
-ar_ex_sys_worker-1.6.23.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
-ar_ex_sys_worker-1.6.23.dist-info/METADATA,sha256=iReyIuivyR5oMFJxkQjVPi_aCDGns-WFzk7hqIEkREA,344
-ar_ex_sys_worker-1.6.23.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-ar_ex_sys_worker-1.6.23.dist-info/top_level.txt,sha256=jmzKGE0ibiJisGg8N7tgxcU9IPcoJJoiT2hiJmRd_rA,23
-ar_ex_sys_worker-1.6.23.dist-info/RECORD,,
+ar_ex_sys_worker-1.6.24.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
+ar_ex_sys_worker-1.6.24.dist-info/METADATA,sha256=PWrcruNxZHmfsYYBjG2TEctqKdIQnx0NhTYC-TfLacs,344
+ar_ex_sys_worker-1.6.24.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+ar_ex_sys_worker-1.6.24.dist-info/top_level.txt,sha256=jmzKGE0ibiJisGg8N7tgxcU9IPcoJJoiT2hiJmRd_rA,23
+ar_ex_sys_worker-1.6.24.dist-info/RECORD,,
```

