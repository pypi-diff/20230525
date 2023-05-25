# Comparing `tmp/yunchi-1.0.6-cp38-cp38-win_amd64.whl.zip` & `tmp/yunchi-1.0.7-cp38-cp38-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 432181 bytes, number of entries: 18
+Zip file size: 450640 bytes, number of entries: 18
 -rw-rw-rw-  2.0 fat      188 b- defN 23-Apr-14 03:05 yunchi/__init__.py
 -rw-rw-rw-  2.0 fat      150 b- defN 23-Apr-14 03:00 yunchi/api.py
--rw-rw-rw-  2.0 fat   387584 b- defN 23-May-05 09:00 yunchi/data.cp38-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   431104 b- defN 23-May-25 05:26 yunchi/data.cp38-win_amd64.pyd
 -rw-rw-rw-  2.0 fat     9397 b- defN 23-Apr-27 03:17 yunchi/model.py
--rw-rw-rw-  2.0 fat   176640 b- defN 23-May-05 09:00 yunchi/quote.cp38-win_amd64.pyd
--rw-rw-rw-  2.0 fat   107520 b- defN 23-May-05 09:00 yunchi/strategy.cp38-win_amd64.pyd
--rw-rw-rw-  2.0 fat   267264 b- defN 23-May-05 09:00 yunchi/trade.cp38-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   176640 b- defN 23-May-25 05:19 yunchi/quote.cp38-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   107520 b- defN 23-May-25 05:20 yunchi/strategy.cp38-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   267776 b- defN 23-May-25 05:19 yunchi/trade.cp38-win_amd64.pyd
 -rw-rw-rw-  2.0 fat     9745 b- defN 23-Apr-06 07:48 yunchi/pb/Quotation.proto
 -rw-rw-rw-  2.0 fat   102268 b- defN 23-Mar-10 07:41 yunchi/pb/Quotation_pb2.py
 -rw-rw-rw-  2.0 fat      104 b- defN 23-Apr-14 01:57 yunchi/pb/__init__.py
 -rw-rw-rw-  2.0 fat   352070 b- defN 23-Apr-14 01:58 yunchi/pb/api_pb2.py
 -rw-rw-rw-  2.0 fat    35275 b- defN 23-Jan-10 06:21 yunchi/pb/dtp.api.proto
 -rw-rw-rw-  2.0 fat    10950 b- defN 23-Jan-10 06:21 yunchi/pb/dtp.type.proto
 -rw-rw-rw-  2.0 fat    49067 b- defN 23-Apr-14 01:57 yunchi/pb/type_pb2.py
--rw-rw-rw-  2.0 fat      466 b- defN 23-May-05 09:00 yunchi-1.0.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-May-05 09:00 yunchi-1.0.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-May-05 09:00 yunchi-1.0.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1435 b- defN 23-May-05 09:00 yunchi-1.0.6.dist-info/RECORD
-18 files, 1510230 bytes uncompressed, 429879 bytes compressed:  71.5%
+-rw-rw-rw-  2.0 fat      466 b- defN 23-May-25 05:26 yunchi-1.0.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-May-25 05:26 yunchi-1.0.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-May-25 05:26 yunchi-1.0.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1435 b- defN 23-May-25 05:26 yunchi-1.0.7.dist-info/RECORD
+18 files, 1554262 bytes uncompressed, 448338 bytes compressed:  71.2%
```

## zipnote {}

```diff
@@ -36,20 +36,20 @@
 
 Filename: yunchi/pb/dtp.type.proto
 Comment: 
 
 Filename: yunchi/pb/type_pb2.py
 Comment: 
 
-Filename: yunchi-1.0.6.dist-info/METADATA
+Filename: yunchi-1.0.7.dist-info/METADATA
 Comment: 
 
-Filename: yunchi-1.0.6.dist-info/WHEEL
+Filename: yunchi-1.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: yunchi-1.0.6.dist-info/top_level.txt
+Filename: yunchi-1.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: yunchi-1.0.6.dist-info/RECORD
+Filename: yunchi-1.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `yunchi-1.0.6.dist-info/RECORD` & `yunchi-1.0.7.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 yunchi/__init__.py,sha256=WQkjHPmt3UIX0zmS-kHM88Ce3Fm_42hpsvXreNBCdlY,188
 yunchi/api.py,sha256=E4wCo1vQJ6isvmmmi7UL007j97aKD8wi934US_JhxhQ,150
-yunchi/data.cp38-win_amd64.pyd,sha256=c83d3n7wQWx_njcLVktklxSeQpO5OJodWHr7YJe7Gug,387584
+yunchi/data.cp38-win_amd64.pyd,sha256=X1HFJlburmDlyhpkTG6l-_aHpBi5J8elxROfOJ70zS4,431104
 yunchi/model.py,sha256=7YF5APh_t9xYf_xg4J89AzColhUgIBJhGGOICGoJunc,9397
-yunchi/quote.cp38-win_amd64.pyd,sha256=lrz0uaozgfaVZILf32s6MOzyLPqm-Z_6VfjRsPU5--Q,176640
-yunchi/strategy.cp38-win_amd64.pyd,sha256=4_0cNOFx1vBQNu4mefCnu1obTuCepWDEjmpXYOiVIf4,107520
-yunchi/trade.cp38-win_amd64.pyd,sha256=CXzactOl7U-y8Z_LOCHu6C9azDWCwwggFyE6YJ9kFZE,267264
+yunchi/quote.cp38-win_amd64.pyd,sha256=fjyEV0DiGv6Cgz9SpOe4iFkgjozWJiiKtRd5OL_InaU,176640
+yunchi/strategy.cp38-win_amd64.pyd,sha256=QwM2R8nkCjmy7jVvHuCdCOpi_jRb0KkLXG3_nyHcl9U,107520
+yunchi/trade.cp38-win_amd64.pyd,sha256=kIOyDkGG0UKmiUrCUkyhYle3046T7p3nnLi2sqHmol0,267776
 yunchi/pb/Quotation.proto,sha256=KC6dzPpDNlzmo9_K2W6mdyh-4rRLunVPY4SpA4uKylo,9745
 yunchi/pb/Quotation_pb2.py,sha256=y9r4cYXLmwIHHkx_9tEJp0g6r-OSioz_aKrs89TRQgI,102268
 yunchi/pb/__init__.py,sha256=N26GSqDd_YKeXVuG9Um4bJCFoMCof_Dd3iq0-ehlQyY,104
 yunchi/pb/api_pb2.py,sha256=O7ilgzdadtZk9fAuUeNznxdfp5faBWYrTeqZfIKvMZg,352070
 yunchi/pb/dtp.api.proto,sha256=FAemqV_DYHlleYoGhXLK0sR9mJjkhTs-raueiJT2L7k,35275
 yunchi/pb/dtp.type.proto,sha256=2gZjLhOKCfpgXMO-dNF_Ya6hsNEwiAt3SBNeGuqc91U,10950
 yunchi/pb/type_pb2.py,sha256=KROjyokWYQxkA0VzaWBiPSFYeK4WxfZ17tQlxQyqu7w,49067
-yunchi-1.0.6.dist-info/METADATA,sha256=hxueHQz8ahHwvN48NmyhPJQu8JRCRrQPlOX8LHYmrqg,466
-yunchi-1.0.6.dist-info/WHEEL,sha256=b_PH-i_F2xFYDXcROE5vpDbWUcY020I0eLFvEIYA9Pc,100
-yunchi-1.0.6.dist-info/top_level.txt,sha256=z4mMQZtRXbemouOLS2_nNueye-Jq_5L2J_YfHRJJ8aQ,7
-yunchi-1.0.6.dist-info/RECORD,,
+yunchi-1.0.7.dist-info/METADATA,sha256=Ix88J-JXGN2c3USwVzoFAjX6w_W22rGe9arLBgyhoNM,466
+yunchi-1.0.7.dist-info/WHEEL,sha256=b_PH-i_F2xFYDXcROE5vpDbWUcY020I0eLFvEIYA9Pc,100
+yunchi-1.0.7.dist-info/top_level.txt,sha256=z4mMQZtRXbemouOLS2_nNueye-Jq_5L2J_YfHRJJ8aQ,7
+yunchi-1.0.7.dist-info/RECORD,,
```

