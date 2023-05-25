# Comparing `tmp/dwiqc-0.1.9-py2.py3-none-any.whl.zip` & `tmp/dwiqc-0.2.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,23 @@
-Zip file size: 21814 bytes, number of entries: 20
+Zip file size: 22467 bytes, number of entries: 21
 -rw-r--r--  2.0 unx      225 b- defN 23-May-19 16:11 dwiqc/__init__.py
--rw-r--r--  2.0 unx      247 b- defN 23-May-23 13:22 dwiqc/__version__.py
+-rw-r--r--  2.0 unx      247 b- defN 23-May-25 19:10 dwiqc/__version__.py
+-rw-r--r--  2.0 unx      283 b- defN 23-May-25 14:54 dwiqc/browser/__init__.py
 -rw-r--r--  2.0 unx       62 b- defN 23-May-19 16:11 dwiqc/cli/__init__.py
--rw-r--r--  2.0 unx     6651 b- defN 23-May-19 16:11 dwiqc/cli/get.py
--rw-r--r--  2.0 unx     5273 b- defN 23-May-19 16:11 dwiqc/cli/process.py
+-rw-r--r--  2.0 unx     6651 b- defN 23-May-25 14:45 dwiqc/cli/get.py
+-rw-r--r--  2.0 unx     5805 b- defN 23-May-25 14:56 dwiqc/cli/process.py
 -rw-r--r--  2.0 unx      160 b- defN 23-May-19 16:11 dwiqc/config/__init__.py
 -rw-r--r--  2.0 unx      274 b- defN 23-May-19 16:11 dwiqc/config/dwiqc.yaml
 -rw-r--r--  2.0 unx       98 b- defN 23-May-19 16:11 dwiqc/state/__init__.py
 -rw-r--r--  2.0 unx     1892 b- defN 23-May-19 16:11 dwiqc/tasks/__init__.py
--rw-r--r--  2.0 unx     8696 b- defN 23-May-23 13:17 dwiqc/tasks/prequal.py
+-rw-r--r--  2.0 unx     8664 b- defN 23-May-23 14:22 dwiqc/tasks/prequal.py
 -rw-r--r--  2.0 unx     4209 b- defN 23-May-22 17:12 dwiqc/tasks/prequal_EQ.py
 -rw-r--r--  2.0 unx     6193 b- defN 23-May-23 11:24 dwiqc/tasks/qsiprep.py
 -rw-r--r--  2.0 unx     3782 b- defN 23-May-19 16:11 dwiqc/tasks/qsiprep_EQ.py
--rw-r--r--  2.0 unx    13810 b- defN 23-May-23 12:53 dwiqc/xnat/__init__.py
--rwxr-xr-x  2.0 unx     3889 b- defN 23-May-23 13:23 dwiqc-0.1.9.data/scripts/dwiQC.py
--rw-r--r--  2.0 unx     1541 b- defN 23-May-23 13:23 dwiqc-0.1.9.dist-info/LICENSE
--rw-r--r--  2.0 unx      388 b- defN 23-May-23 13:23 dwiqc-0.1.9.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-May-23 13:23 dwiqc-0.1.9.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-May-23 13:23 dwiqc-0.1.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1559 b- defN 23-May-23 13:23 dwiqc-0.1.9.dist-info/RECORD
-20 files, 59065 bytes uncompressed, 19302 bytes compressed:  67.3%
+-rw-r--r--  2.0 unx    14029 b- defN 23-May-25 14:46 dwiqc/xnat/__init__.py
+-rwxr-xr-x  2.0 unx     3889 b- defN 23-May-25 19:12 dwiqc-0.2.0.data/scripts/dwiQC.py
+-rw-r--r--  2.0 unx     1541 b- defN 23-May-25 19:12 dwiqc-0.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      457 b- defN 23-May-25 19:12 dwiqc-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-May-25 19:12 dwiqc-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-May-25 19:12 dwiqc-0.2.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1640 b- defN 23-May-25 19:12 dwiqc-0.2.0.dist-info/RECORD
+21 files, 60217 bytes uncompressed, 19829 bytes compressed:  67.1%
```

## zipnote {}

```diff
@@ -1,13 +1,16 @@
 Filename: dwiqc/__init__.py
 Comment: 
 
 Filename: dwiqc/__version__.py
 Comment: 
 
+Filename: dwiqc/browser/__init__.py
+Comment: 
+
 Filename: dwiqc/cli/__init__.py
 Comment: 
 
 Filename: dwiqc/cli/get.py
 Comment: 
 
 Filename: dwiqc/cli/process.py
@@ -36,26 +39,26 @@
 
 Filename: dwiqc/tasks/qsiprep_EQ.py
 Comment: 
 
 Filename: dwiqc/xnat/__init__.py
 Comment: 
 
-Filename: dwiqc-0.1.9.data/scripts/dwiQC.py
+Filename: dwiqc-0.2.0.data/scripts/dwiQC.py
 Comment: 
 
-Filename: dwiqc-0.1.9.dist-info/LICENSE
+Filename: dwiqc-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: dwiqc-0.1.9.dist-info/METADATA
+Filename: dwiqc-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: dwiqc-0.1.9.dist-info/WHEEL
+Filename: dwiqc-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: dwiqc-0.1.9.dist-info/top_level.txt
+Filename: dwiqc-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: dwiqc-0.1.9.dist-info/RECORD
+Filename: dwiqc-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dwiqc/__version__.py

```diff
@@ -1,6 +1,6 @@
 __title__ = 'dwiqc'
 __description__ = 'Quality Assurance Pipeline for Diffusion MR Data'
 __url__ = 'https://github.com/harvard-nrg/dwiqc'
-__version__ = '0.1.9'
+__version__ = '0.2.0'
 __author__ = 'Neuroinformatics Research Group'
 __author_email__ = 'info@neuroinfo.org'
```

## dwiqc/cli/process.py

```diff
@@ -2,28 +2,34 @@
 import re
 import sys
 import json
 import yaml
 import yaxil
 import glob
 import math
+import anatqc
 import logging
 import tarfile
 import executors
 import tempfile
 import subprocess as sp
 import shutil
 from executors.models import Job, JobArray
 from bids import BIDSLayout
 from dwiqc.xnat import Report
 import dwiqc.tasks.prequal as prequal
 import dwiqc.tasks.qsiprep as qsiprep
 import dwiqc.tasks.prequal_EQ as prequal_EQ
 import dwiqc.tasks.qsiprep_EQ as qsiprep_EQ
-from dwiqc.state import State
+import dwiqc.broswer as browser
+sys.path.insert(0, os.path.join(os.environ['MODULESHOME'], "init"))
+from env_modules_python import module
+
+module('load', 'chromium.org/chromium/102.0.5005.115-ncf')
+
 
 logger = logging.getLogger(__name__)
 
 def do(args):
     if args.insecure:
         logger.warning('disabling ssl certificate verification')
         yaxil.CHECK_CERTIFICATE = False
@@ -74,20 +80,23 @@
         logger.info(json.dumps(prequal_task.command, indent=1))
         jarray.add(prequal_task.job)
 
     # qsiprep job
     qsiprep_outdir = None
     if 'qsiprep' in args.sub_tasks:
         qsiprep_outdir = os.path.join(args.bids_dir, 'derivatives', 'dwiqc-qsiprep', f'sub-{args.sub}', f'ses-{args.ses}', basename, 'qsiprep_output')
+        qsiprep_trick = tempfile.TemporaryDirectory(dir='/n/holyscratch01/LABS/nrg/Lab', suffix='.qsiprep')
+        os.makedirs(qsiprep_outdir, exist_ok=True)
+        os.symlink(qsiprep_outdir, f"{qsiprep_trick.name}/q")
         qsiprep_task = qsiprep.Task(
             sub=args.sub,
             ses=args.ses,
             run=args.run,
             bids=args.bids_dir,
-            outdir=qsiprep_outdir,
+            outdir=f"{qsiprep_trick.name}/q",
             tempdir=tempfile.gettempdir(),
             pipenv='/sw/apps/qsiprep'
         )
         os.environ['OPENBLAS_NUM_THREADS'] = '1'
         logger.info(json.dumps(qsiprep_task.command, indent=1))
         #check_for_output(args, qsiprep_outdir)
         jarray.add(qsiprep_task.job)
@@ -99,14 +108,15 @@
         logger.info('waiting for all jobs to finish')
         jarray.wait()
         numjobs = len(jarray.array)
         failed = len(jarray.failed)
         complete = len(jarray.complete)
         prequal_eddy(args, prequal_outdir)
         qsiprep_eddy(args, qsiprep_outdir)
+        browser.snapshot(f"{qsiprep_outdir}/qsiprep/sub-{args.sub}.html", f"{qsiprep_outdir}/qsiprep/qsiprep.pdf") 
         if failed:
             logger.info('%s/%s jobs failed', failed, numjobs)
             for pid,job in iter(jarray.failed.items()):
                 logger.error('%s exited with returncode %s', job.name, job.returncode)
                 with open(job.output, 'r') as fp:
                     logger.error('standard output\n%s', fp.read())
                 with open(job.error, 'r') as fp:
@@ -160,9 +170,9 @@
 
 
 
 #    # upload data to xnat over rest api
 #    if args.xnat_upload:
 #        logger.info('Uploading artifacts to XNAT')
 #        auth = yaxil.auth2(args.xnat_alias)
-#        yaxil.storerest(auth, args.artifacts_dir, 'dwiqc-resource')
+#        yaxil.storerest(auth, args.artifacts_dir, 'anatqc-resource')
```

## dwiqc/tasks/prequal.py

```diff
@@ -1,10 +1,10 @@
 
 #### load necessary libraries
-
+import tempfile
 import subprocess
 import os
 import logging
 from bids import BIDSLayout
 import sys
 import json
 import dwiqc.tasks as tasks
@@ -258,20 +258,16 @@
 					json.dump(file_data, f, indent = 2)
 
 
 	# build the prequal sbatch command and create job
 
 	def build(self):
 		self.add_intended_for()
-		cwd = os.getcwd()
-		print(self._tempdir)
-		os.chdir(self._tempdir)
-		print(os.getcwd())
-		sys.exit()
-		os.chdir(cwd)
+		os.system('mkdir -p $TMPDIR')
+		self._tempdir = tempfile.gettempdir()
 		inputs_dir = f'{self._tempdir}/INPUTS/'
 		self.copy_inputs(inputs_dir)
 		self._command = [
 			'selfie',
 			'--lock',
 			'--output-file', self._prov,
 			'singularity',
```

## dwiqc/xnat/__init__.py

```diff
@@ -165,14 +165,18 @@
                 'source': os.path.join(self.dirs['prequal'], 'OUTPUTS', 'PDF', 'dtiQA.pdf'),
                 'dest': os.path.join('prequal_pdf', '{0}_prequal_qc.pdf'.format(aid))
             },
 
             # pull files from qsiprep output
 
             {
+                'source': os.path.join(self.dirs['qsiprep'], 'qsiprep_output', 'qsiprep',  'qsiprep.pdf'),
+                'dest': os.path.join('qsiprep-pdf', '{0}_qsiprep.pdf'.format(aid))
+            },
+            {
                 'source': os.path.join(self.dirs['qsiprep'], 'qsiprep_output', 'qsiprep',  self.sub + '.html'),
                 'dest': os.path.join('qsiprep-html', '{0}_qsiprep.html'.format(aid))
             },
             {
                 'source': os.path.join(self.dirs['qsiprep'], 'qsiprep_output', 'qsiprep',  self.sub, 'figures', self.sub + '_ses-' + self.ses + '_run-' + self.run + '_carpetplot.svg'),
                 'dest': os.path.join('carpet-plot', '{0}_carpetplot.svg'.format(aid))
             },
```

## Comparing `dwiqc-0.1.9.data/scripts/dwiQC.py` & `dwiqc-0.2.0.data/scripts/dwiQC.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import sys
 import dwiqc
 import dwiqc.cli as cli
 import logging
 import argparse as ap
 import dwiqc.config as config
 
+
 logger = logging.getLogger(__name__)
 
 
 
 
 def main():
     parser = ap.ArgumentParser()
@@ -96,10 +97,10 @@
     logging.basicConfig(
         level=level,
         format='%(asctime)s.%(msecs)03d %(levelname)s %(module)s - %(funcName)s: %(message)s',
         datefmt='%Y-%m-%d %H:%M:%S'
     )
 
 if __name__ == '__main__':
-    main()
+   main()
```

## Comparing `dwiqc-0.1.9.dist-info/LICENSE` & `dwiqc-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dwiqc-0.1.9.dist-info/RECORD` & `dwiqc-0.2.0.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 dwiqc/__init__.py,sha256=MZJhUZKhHHoZ2w_GeoFCITk1m_0ASdRw_ZaeDixFEPU,225
-dwiqc/__version__.py,sha256=s0Ubik8_58WTORo_NGEJ5QXWgfZgTdyq_fUnySJkR2U,247
+dwiqc/__version__.py,sha256=1KRq0DVFDxk2iSmDfpBZnQA7Rttv4X1YZA8dflf7aSc,247
+dwiqc/browser/__init__.py,sha256=MlUOz0v7bA_dtQyXX27WF0dzyGGo4xkEEt2PT2B0_aQ,283
 dwiqc/cli/__init__.py,sha256=zGIm7lrjh3wA191D-VjQBZNjSlspFUx148VwDNQGaTk,62
 dwiqc/cli/get.py,sha256=6ixaBdwEgY_GXh8L-_3QDY4MEsNqSJgXle_mxW99mlk,6651
-dwiqc/cli/process.py,sha256=X4eUXf-jRuOR_3cVQ0FfcDXmNPVQzILH35uGAtz9upE,5273
+dwiqc/cli/process.py,sha256=bRZ4tOIyJM3xLB1XVN5035YdkQRma_1NcZ4nDIxzZMs,5805
 dwiqc/config/__init__.py,sha256=k_w5JzoJN_7R7eI_sIJxHA4FQQHs0_KGf-6jsbG4Xs8,160
 dwiqc/config/dwiqc.yaml,sha256=x8gKMFZyChdzvNX3GthRe0eWvyKDDL5itXo0kLWVfd0,274
 dwiqc/state/__init__.py,sha256=NaRifw26bI3F1J9BqeLa-KLSzEPq2m_UNhMbXdmPdh4,98
 dwiqc/tasks/__init__.py,sha256=LnlN7iYjpqiBic2ihFrM-_h7m8FD_N7Beh7UIwKyGZ8,1892
-dwiqc/tasks/prequal.py,sha256=vbjvACbD4kNSQScpYC_cYf20SyUVhve-hqo6Y_bazo4,8696
+dwiqc/tasks/prequal.py,sha256=GagoXzYhHaWV2uEfcadsc-85ij71hxP3YnZDANMO2UY,8664
 dwiqc/tasks/prequal_EQ.py,sha256=PWmlo8u_D5qM1lyXdmT7iq865JL6xoPM0JHGEwzRnes,4209
 dwiqc/tasks/qsiprep.py,sha256=2HAmLSSXyKRUuYmok9EEmoPaSo8_7LoCAU-JGfudeiY,6193
 dwiqc/tasks/qsiprep_EQ.py,sha256=JWildptHsuyJVj7ZYMFlWWYvsAIszJpWk1a0m05JM-Q,3782
-dwiqc/xnat/__init__.py,sha256=8jjaZO_5JlUhiSHNsmDr59HsfOS-uZAunSQuLPUXb1g,13810
-dwiqc-0.1.9.data/scripts/dwiQC.py,sha256=OkI1WZqnUIqS4DWSt-pSm01taEv3m_aNmqSJUM50N_U,3889
-dwiqc-0.1.9.dist-info/LICENSE,sha256=ReOF9BmlQdkCj4b2gQYogJrk_QkbUAuz8W1ZVqI0pcs,1541
-dwiqc-0.1.9.dist-info/METADATA,sha256=xaGdhumZ8S4f0eMWQZ50M-BaaZxBXhDplwqpUHubiPs,388
-dwiqc-0.1.9.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-dwiqc-0.1.9.dist-info/top_level.txt,sha256=omH7pmKt7fzFyiNkTPDLX4yyBccoge5Saqc9rgyu0Wk,6
-dwiqc-0.1.9.dist-info/RECORD,,
+dwiqc/xnat/__init__.py,sha256=oPnIkNNM5Tw7Q677VioA8sSU2_Qa6FH-ckjxTQakFdc,14029
+dwiqc-0.2.0.data/scripts/dwiQC.py,sha256=D6ZRhtwJAl0gYODeWhrT4fl7tZtnul0iXrMRyrHxIfE,3889
+dwiqc-0.2.0.dist-info/LICENSE,sha256=ReOF9BmlQdkCj4b2gQYogJrk_QkbUAuz8W1ZVqI0pcs,1541
+dwiqc-0.2.0.dist-info/METADATA,sha256=W_VJDbRBkOIr85VtRTzuPZEyyX7Gz41enYGWuZn4bW8,457
+dwiqc-0.2.0.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
+dwiqc-0.2.0.dist-info/top_level.txt,sha256=omH7pmKt7fzFyiNkTPDLX4yyBccoge5Saqc9rgyu0Wk,6
+dwiqc-0.2.0.dist-info/RECORD,,
```

