# Comparing `tmp/sslcompare-1.6.1-py3-none-any.whl.zip` & `tmp/sslcompare-1.7.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3112127 bytes, number of entries: 30
+Zip file size: 3112337 bytes, number of entries: 30
 -rw-r--r--  2.0 unx     5743 b- defN 80-Jan-01 00:00 sslcompare/anssi.yaml
--rwxr-xr-x  2.0 unx     3705 b- defN 80-Jan-01 00:00 sslcompare/sslcompare.py
+-rwxr-xr-x  2.0 unx     4366 b- defN 80-Jan-01 00:00 sslcompare/sslcompare.py
 -rw-r--r--  2.0 unx     4380 b- defN 80-Jan-01 00:00 sslcompare/testssl.sh/CREDITS.md
 -rw-r--r--  2.0 unx    18092 b- defN 80-Jan-01 00:00 sslcompare/testssl.sh/LICENSE
 -rw-r--r--  2.0 unx     6279 b- defN 80-Jan-01 00:00 sslcompare/testssl.sh/bin/OPENSSL-LICENSE.txt
 -rwxr-xr-x  2.0 unx  4009248 b- defN 80-Jan-01 00:00 sslcompare/testssl.sh/bin/openssl.Linux.x86_64
 -rw-r--r--  2.0 unx   262468 b- defN 80-Jan-01 00:00 sslcompare/testssl.sh/etc/Apple.pem
 -rw-r--r--  2.0 unx     1200 b- defN 80-Jan-01 00:00 sslcompare/testssl.sh/etc/DST Root CA X3.txt
 -rw-r--r--  2.0 unx   137523 b- defN 80-Jan-01 00:00 sslcompare/testssl.sh/etc/Java.pem
@@ -20,13 +20,13 @@
 -rw-r--r--  2.0 unx    72132 b- defN 80-Jan-01 00:00 sslcompare/testssl.sh/etc/client-simulation.wiresharked.txt
 -rw-r--r--  2.0 unx    52655 b- defN 80-Jan-01 00:00 sslcompare/testssl.sh/etc/common-primes.txt
 -rw-r--r--  2.0 unx     2085 b- defN 80-Jan-01 00:00 sslcompare/testssl.sh/etc/curves-mapping.txt
 -rw-r--r--  2.0 unx      688 b- defN 80-Jan-01 00:00 sslcompare/testssl.sh/etc/curves.txt
 -rw-r--r--  2.0 unx    10771 b- defN 80-Jan-01 00:00 sslcompare/testssl.sh/etc/openssl.cnf
 -rw-r--r--  2.0 unx    28780 b- defN 80-Jan-01 00:00 sslcompare/testssl.sh/etc/tls_data.txt
 -rwxr-xr-x  2.0 unx  1194674 b- defN 80-Jan-01 00:00 sslcompare/testssl.sh/testssl.sh
--rw-r--r--  2.0 unx    18093 b- defN 80-Jan-01 00:00 sslcompare-1.6.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      562 b- defN 80-Jan-01 00:00 sslcompare-1.6.1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 sslcompare-1.6.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       57 b- defN 80-Jan-01 00:00 sslcompare-1.6.1.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     2832 b- defN 16-Jan-01 00:00 sslcompare-1.6.1.dist-info/RECORD
-30 files, 7392029 bytes uncompressed, 3107513 bytes compressed:  58.0%
+-rw-r--r--  2.0 unx    18093 b- defN 80-Jan-01 00:00 sslcompare-1.7.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      562 b- defN 80-Jan-01 00:00 sslcompare-1.7.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 sslcompare-1.7.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       57 b- defN 80-Jan-01 00:00 sslcompare-1.7.0.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     2832 b- defN 16-Jan-01 00:00 sslcompare-1.7.0.dist-info/RECORD
+30 files, 7392690 bytes uncompressed, 3107723 bytes compressed:  58.0%
```

## zipnote {}

```diff
@@ -69,23 +69,23 @@
 
 Filename: sslcompare/testssl.sh/etc/tls_data.txt
 Comment: 
 
 Filename: sslcompare/testssl.sh/testssl.sh
 Comment: 
 
-Filename: sslcompare-1.6.1.dist-info/LICENSE
+Filename: sslcompare-1.7.0.dist-info/LICENSE
 Comment: 
 
-Filename: sslcompare-1.6.1.dist-info/METADATA
+Filename: sslcompare-1.7.0.dist-info/METADATA
 Comment: 
 
-Filename: sslcompare-1.6.1.dist-info/WHEEL
+Filename: sslcompare-1.7.0.dist-info/WHEEL
 Comment: 
 
-Filename: sslcompare-1.6.1.dist-info/entry_points.txt
+Filename: sslcompare-1.7.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: sslcompare-1.6.1.dist-info/RECORD
+Filename: sslcompare-1.7.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sslcompare/sslcompare.py

```diff
@@ -38,37 +38,52 @@
     """
     strip_ansi = partial(re.compile(r"\x1b\[\d*m").sub, "")
 
     with open(baseline) as baseline_path:
         baseline_suites = yaml.safe_load(baseline_path)
 
     click.secho(
-        "This is testssl.sh's raw output, mainly for debugging purposes. Do not screenshot this !",
+        f'running "testssl.sh -E -U {url}", and showing the full output:',
         fg="black",
         bg="white",
         bold=True,
     )
-
     output = []
     with resources.path("sslcompare", "testssl.sh") as testssl_path:
         with subprocess.Popen(
             shlex.split(f"{testssl_path / 'testssl.sh'} -E -U {url}"),
             # bufsize=1,
             # universal_newlines=True,
             stdout=subprocess.PIPE,
             stderr=subprocess.STDOUT,
         ) as testssl:
+            # The following is to ensure that testssl's output is immediately shown
+            # to the user, even if no newline is present.
+            # For instance, a case was encountered where testssl would ask the user
+            # something like "type 'yes' to continue".
+            # Because the output was line-buffered, sslcompare would hang
+            # and the user would not see anything.
+            # The following code should fix that
             for chunk in iter(partial(testssl.stdout.read, 1), b""):
-                sys.stdout.buffer.write(chunk)
+                if hasattr(sys.stdout, "buffer"):
+                    sys.stdout.buffer.write(chunk)
+                    sys.stdout.flush()
+                else:
+                    sys.stdout.write(chunk.decode())
                 output.append(chunk)
 
     current_protocol = None
     interesting_lines = False
 
-    click.secho("Here is the screenshotable output:", fg="black", bg="white", bold=True)
+    click.secho(
+        "Here is the summarized output with ANSSI's recommandations:",
+        fg="black",
+        bg="white",
+        bold=True,
+    )
     for line in b"".join(output).decode().split("\n"):
         if "Start" in line:
             click.echo(line)
 
         elif "Done" in line:
             click.echo(line)
             break
```

## Comparing `sslcompare-1.6.1.dist-info/LICENSE` & `sslcompare-1.7.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sslcompare-1.6.1.dist-info/METADATA` & `sslcompare-1.7.0.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sslcompare
-Version: 1.6.1
+Version: 1.7.0
 Summary: Compares a server's cipher suites with a provided baseline
 License: GPLv2
 Author: Arthur Le Corguille
 Requires-Python: >=3.8.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

## Comparing `sslcompare-1.6.1.dist-info/RECORD` & `sslcompare-1.7.0.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 sslcompare/anssi.yaml,sha256=KKgftCem90blkyiruITpNcZS1wldxQHafY2yYTyaDm4,5743
-sslcompare/sslcompare.py,sha256=KjdYnhe0D43UKeb9zAXSFQU3XHhuSAsbFSyOYC3E1b8,3705
+sslcompare/sslcompare.py,sha256=TN4rJyobXXyr8Ja4MQONA6EoIYB6srsE2whK8xE2S64,4366
 sslcompare/testssl.sh/CREDITS.md,sha256=7sHh3dfMqrF_YCxcgkFXyIyUUXNfifii3mo9y66x9Rc,4380
 sslcompare/testssl.sh/LICENSE,sha256=gXf5dRMhNSbfLPYYTY_5hsZ1r7UU1OaKQEAQUhuIBkM,18092
 sslcompare/testssl.sh/bin/OPENSSL-LICENSE.txt,sha256=JX_htUL4RlV9D8k49CBtbJpjNOK1cfoCDlH5Y3dTcSA,6279
 sslcompare/testssl.sh/bin/openssl.Linux.x86_64,sha256=-mlTiOxFVb8F7iSZOJnVebvgkj5wMwRvI0kS0hS0QUM,4009248
 sslcompare/testssl.sh/etc/Apple.pem,sha256=IKm7Bw6KjzMCDVs0H_fGSwJEn1sP-j3h65QHaG6V_xs,262468
 sslcompare/testssl.sh/etc/DST Root CA X3.txt,sha256=E5peSk4PpQU3jHLF9wCTTOgzP05rG1CIhsSw6xT0vpk,1200
 sslcompare/testssl.sh/etc/Java.pem,sha256=ur4Hmu4MKKqiERtHY1LNhpy52rGVPrL3WIPGCRRjV_I,137523
@@ -19,12 +19,12 @@
 sslcompare/testssl.sh/etc/client-simulation.wiresharked.txt,sha256=9Wpe0AgaLoCRZTJW6fJiZR8Y5qk4klX_NnHVwpHoFC4,72132
 sslcompare/testssl.sh/etc/common-primes.txt,sha256=uEY-4GrxHDk0z9tnZqZGuY2wF3nukxYTF-6YQXBm8wU,52655
 sslcompare/testssl.sh/etc/curves-mapping.txt,sha256=spcpLI_s6MbVnrib6inW_nCkJZ38Si8Y_2LV8DmdZsI,2085
 sslcompare/testssl.sh/etc/curves.txt,sha256=QRm3onnWi5g5dHmxV1F5INvaLyy_W4V2IgghAHE0n8Y,688
 sslcompare/testssl.sh/etc/openssl.cnf,sha256=H4d7agZbfwFH49D8tckzg8s_EIK7W_tJNPSTheiYvCw,10771
 sslcompare/testssl.sh/etc/tls_data.txt,sha256=9FbHc796s8O9t6Lgzbohqi4RVJkKmDhEsLW-gRIBN2w,28780
 sslcompare/testssl.sh/testssl.sh,sha256=h9yYcVDHTWa2V6ndbgcFkiMvcqYV4Vdw_kzb7SLTGXM,1194674
-sslcompare-1.6.1.dist-info/LICENSE,sha256=ZA2Q9u5AEkH_YoNNDRsz-DBJ6ZuL_foE7RsKFjXd4-c,18093
-sslcompare-1.6.1.dist-info/METADATA,sha256=NNCxSY1szdtMw0SHJdUqRAMJH9YOBwNaizD6ubxRjDw,562
-sslcompare-1.6.1.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-sslcompare-1.6.1.dist-info/entry_points.txt,sha256=5mlmXkHhO-VpoC2TXItTiJe_7QZpXSL6ouL5v70JK4k,57
-sslcompare-1.6.1.dist-info/RECORD,,
+sslcompare-1.7.0.dist-info/LICENSE,sha256=ZA2Q9u5AEkH_YoNNDRsz-DBJ6ZuL_foE7RsKFjXd4-c,18093
+sslcompare-1.7.0.dist-info/METADATA,sha256=NNn_iG07ni8t8Mzq-xw-928AJot7GcyfavhpfAeDDrM,562
+sslcompare-1.7.0.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+sslcompare-1.7.0.dist-info/entry_points.txt,sha256=5mlmXkHhO-VpoC2TXItTiJe_7QZpXSL6ouL5v70JK4k,57
+sslcompare-1.7.0.dist-info/RECORD,,
```

