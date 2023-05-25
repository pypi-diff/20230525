# Comparing `tmp/neon_enclosure-1.4.3a1-py3-none-any.whl.zip` & `tmp/neon_enclosure-1.4.3a2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,15 @@
-Zip file size: 12221 bytes, number of entries: 12
--rw-r--r--  2.0 unx     1831 b- defN 23-May-17 21:19 neon_enclosure/__init__.py
--rw-r--r--  2.0 unx     2913 b- defN 23-May-17 21:19 neon_enclosure/__main__.py
--rw-r--r--  2.0 unx     3660 b- defN 23-May-17 21:19 neon_enclosure/service.py
--rw-r--r--  2.0 unx     1832 b- defN 23-May-17 21:19 neon_enclosure/admin/__init__.py
--rw-r--r--  2.0 unx     2863 b- defN 23-May-17 21:19 neon_enclosure/admin/__main__.py
--rw-r--r--  2.0 unx     2406 b- defN 23-May-17 21:19 neon_enclosure/admin/service.py
--rw-r--r--  2.0 unx     1634 b- defN 23-May-17 21:20 neon_enclosure-1.4.3a1.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     2702 b- defN 23-May-17 21:20 neon_enclosure-1.4.3a1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-17 21:20 neon_enclosure-1.4.3a1.dist-info/WHEEL
--rw-r--r--  2.0 unx       71 b- defN 23-May-17 21:20 neon_enclosure-1.4.3a1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       15 b- defN 23-May-17 21:20 neon_enclosure-1.4.3a1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1052 b- defN 23-May-17 21:20 neon_enclosure-1.4.3a1.dist-info/RECORD
-12 files, 21071 bytes uncompressed, 10431 bytes compressed:  50.5%
+Zip file size: 13817 bytes, number of entries: 13
+-rw-r--r--  2.0 unx     1831 b- defN 23-May-25 16:56 neon_enclosure/__init__.py
+-rw-r--r--  2.0 unx     2832 b- defN 23-May-25 16:56 neon_enclosure/__main__.py
+-rw-r--r--  2.0 unx     3152 b- defN 23-May-25 16:56 neon_enclosure/cli.py
+-rw-r--r--  2.0 unx     3660 b- defN 23-May-25 16:56 neon_enclosure/service.py
+-rw-r--r--  2.0 unx     1832 b- defN 23-May-25 16:56 neon_enclosure/admin/__init__.py
+-rw-r--r--  2.0 unx     2839 b- defN 23-May-25 16:56 neon_enclosure/admin/__main__.py
+-rw-r--r--  2.0 unx     2406 b- defN 23-May-25 16:56 neon_enclosure/admin/service.py
+-rw-r--r--  2.0 unx     1634 b- defN 23-May-25 16:56 neon_enclosure-1.4.3a2.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     2702 b- defN 23-May-25 16:56 neon_enclosure-1.4.3a2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-25 16:56 neon_enclosure-1.4.3a2.dist-info/WHEEL
+-rw-r--r--  2.0 unx      126 b- defN 23-May-25 16:56 neon_enclosure-1.4.3a2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       15 b- defN 23-May-25 16:56 neon_enclosure-1.4.3a2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1131 b- defN 23-May-25 16:56 neon_enclosure-1.4.3a2.dist-info/RECORD
+13 files, 24252 bytes uncompressed, 11909 bytes compressed:  50.9%
```

## zipnote {}

```diff
@@ -1,37 +1,40 @@
 Filename: neon_enclosure/__init__.py
 Comment: 
 
 Filename: neon_enclosure/__main__.py
 Comment: 
 
+Filename: neon_enclosure/cli.py
+Comment: 
+
 Filename: neon_enclosure/service.py
 Comment: 
 
 Filename: neon_enclosure/admin/__init__.py
 Comment: 
 
 Filename: neon_enclosure/admin/__main__.py
 Comment: 
 
 Filename: neon_enclosure/admin/service.py
 Comment: 
 
-Filename: neon_enclosure-1.4.3a1.dist-info/LICENSE.md
+Filename: neon_enclosure-1.4.3a2.dist-info/LICENSE.md
 Comment: 
 
-Filename: neon_enclosure-1.4.3a1.dist-info/METADATA
+Filename: neon_enclosure-1.4.3a2.dist-info/METADATA
 Comment: 
 
-Filename: neon_enclosure-1.4.3a1.dist-info/WHEEL
+Filename: neon_enclosure-1.4.3a2.dist-info/WHEEL
 Comment: 
 
-Filename: neon_enclosure-1.4.3a1.dist-info/entry_points.txt
+Filename: neon_enclosure-1.4.3a2.dist-info/entry_points.txt
 Comment: 
 
-Filename: neon_enclosure-1.4.3a1.dist-info/top_level.txt
+Filename: neon_enclosure-1.4.3a2.dist-info/top_level.txt
 Comment: 
 
-Filename: neon_enclosure-1.4.3a1.dist-info/RECORD
+Filename: neon_enclosure-1.4.3a2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## neon_enclosure/__main__.py

```diff
@@ -22,25 +22,23 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-from neon_utils.configuration_utils import init_config_dir
 from neon_utils.log_utils import init_log
 from neon_utils.process_utils import start_malloc, snapshot_malloc, print_malloc
 from ovos_utils.messagebus import get_mycroft_bus
 from ovos_utils.process_utils import reset_sigint_handler
 from ovos_utils.log import LOG
 from ovos_utils import wait_for_exit_signal
 
 
 def main(*args, **kwargs):
-    init_config_dir()
     init_log(log_name="enclosure")
     malloc_running = start_malloc(stack_depth=4)
     bus = get_mycroft_bus()
     kwargs["bus"] = bus
     from neon_utils.signal_utils import init_signal_bus, \
         init_signal_handlers
     init_signal_bus(bus)
```

## neon_enclosure/admin/__main__.py

```diff
@@ -31,15 +31,14 @@
 from ovos_utils.messagebus import get_mycroft_bus
 from ovos_utils.process_utils import reset_sigint_handler
 from ovos_utils import wait_for_exit_signal
 from ovos_utils.log import LOG
 
 
 def main(*args, **kwargs):
-    # init_config_dir()
     init_log(log_name="admin")
     malloc_running = start_malloc(stack_depth=4)
 
     bus = get_mycroft_bus()
     kwargs["bus"] = bus
     from neon_utils.signal_utils import init_signal_bus, \
         init_signal_handlers
```

## Comparing `neon_enclosure-1.4.3a1.dist-info/LICENSE.md` & `neon_enclosure-1.4.3a2.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `neon_enclosure-1.4.3a1.dist-info/METADATA` & `neon_enclosure-1.4.3a2.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-enclosure
-Version: 1.4.3a1
+Version: 1.4.3a2
 Summary: Neon Enclosure Module
 Home-page: https://github.com/NeonGeckoCom/neon-enclosure
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

## Comparing `neon_enclosure-1.4.3a1.dist-info/RECORD` & `neon_enclosure-1.4.3a2.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 neon_enclosure/__init__.py,sha256=UDwbScPcnqA05m_zQmXnY6YeoL5j6NS_TaLj0mQdU_8,1831
-neon_enclosure/__main__.py,sha256=D-bJQWvxmWuejEjtTQOLT1bObyyF87pmypGfGp7Y_H0,2913
+neon_enclosure/__main__.py,sha256=v0iXqgiP-OXIHMoReuZ3v_3cCm7SVKsvlEyobaldfv0,2832
+neon_enclosure/cli.py,sha256=hrt0DltcdUypm-g08OFDG8ojbMXSANkgRw1OAVk_10g,3152
 neon_enclosure/service.py,sha256=ntd4ky4nfdtDEkWEKn8wRJkrqQFX1_N9l0HDXQwDcfI,3660
 neon_enclosure/admin/__init__.py,sha256=FCW9FTGwZxZm9BbxptD2ri02MXw5mq0YtuIfJ0Rm0SA,1832
-neon_enclosure/admin/__main__.py,sha256=jCOB5uT0EOXNgrJxVNYSdPQ3IqGH-E0bMxF6Odcx5lA,2863
+neon_enclosure/admin/__main__.py,sha256=bMiOyKwsqEyqXlgOSiy64lT1pqCw7hq5pvrTUXGVZdE,2839
 neon_enclosure/admin/service.py,sha256=UrD0RLVFi-27A0wnFFfQjVlmo-GHWxEyma1Q0W8TLqE,2406
-neon_enclosure-1.4.3a1.dist-info/LICENSE.md,sha256=gxKa3HnxC7fSIlGFpLAiSAhQS22pIyVEyXmPQR2KlXM,1634
-neon_enclosure-1.4.3a1.dist-info/METADATA,sha256=zR0ip4Z9pF7HaGPDuKKhizPrElbozCf-0V-o0vUoLNI,2702
-neon_enclosure-1.4.3a1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-neon_enclosure-1.4.3a1.dist-info/entry_points.txt,sha256=B38ve9l9IDVVfjPQFWLh0CYSoOJ454sgGWq3dfu6EPU,71
-neon_enclosure-1.4.3a1.dist-info/top_level.txt,sha256=JyzbDWcL_LA7RBt9baW_93Ep9FDpe-ukXCsowuQm2Ug,15
-neon_enclosure-1.4.3a1.dist-info/RECORD,,
+neon_enclosure-1.4.3a2.dist-info/LICENSE.md,sha256=gxKa3HnxC7fSIlGFpLAiSAhQS22pIyVEyXmPQR2KlXM,1634
+neon_enclosure-1.4.3a2.dist-info/METADATA,sha256=exB9f5HzPBmZO-LAvwcEK82GvFOu7h0eYB2qPQViNQ0,2702
+neon_enclosure-1.4.3a2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+neon_enclosure-1.4.3a2.dist-info/entry_points.txt,sha256=xIujp8DylZvh005eOZ7canZhQr2JdIepZhoV2SXRnEI,126
+neon_enclosure-1.4.3a2.dist-info/top_level.txt,sha256=JyzbDWcL_LA7RBt9baW_93Ep9FDpe-ukXCsowuQm2Ug,15
+neon_enclosure-1.4.3a2.dist-info/RECORD,,
```

