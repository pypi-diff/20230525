# Comparing `tmp/sequana_laa-0.8.0.tar.gz` & `tmp/sequana_laa-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sequana_laa-0.8.0.tar", last modified: Fri Jan 14 12:50:11 2022, max compression
+gzip compressed data, was "dist/sequana_laa-0.9.0.tar", last modified: Tue Aug 30 19:32:36 2022, max compression
```

## Comparing `sequana_laa-0.8.0.tar` & `sequana_laa-0.9.0.tar`

### file list

```diff
@@ -1,32 +1,24 @@
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2022-01-14 12:50:11.000000 sequana_laa-0.8.0/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       66 2022-01-14 09:49:19.000000 sequana_laa-0.8.0/.coveragerc
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2022-01-14 12:50:11.000000 sequana_laa-0.8.0/.github/
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2022-01-14 12:50:11.000000 sequana_laa-0.8.0/.github/workflows/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1198 2022-01-14 12:28:47.000000 sequana_laa-0.8.0/.github/workflows/main.yml
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1036 2022-01-14 12:18:27.000000 sequana_laa-0.8.0/.github/workflows/pypi.yml
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1172 2022-01-14 09:49:19.000000 sequana_laa-0.8.0/.gitignore
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1530 2022-01-14 09:49:19.000000 sequana_laa-0.8.0/LICENSE
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      182 2022-01-14 12:20:49.000000 sequana_laa-0.8.0/MANIFEST.in
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4322 2022-01-14 12:50:11.000000 sequana_laa-0.8.0/PKG-INFO
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3044 2022-01-14 12:49:53.000000 sequana_laa-0.8.0/README.rst
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       76 2022-01-14 12:27:20.000000 sequana_laa-0.8.0/conda.yml
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       41 2022-01-14 09:49:19.000000 sequana_laa-0.8.0/requirements.txt
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2022-01-14 12:50:11.000000 sequana_laa-0.8.0/sequana_laa.egg-info/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4322 2022-01-14 12:50:11.000000 sequana_laa-0.8.0/sequana_laa.egg-info/PKG-INFO
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      632 2022-01-14 12:50:11.000000 sequana_laa-0.8.0/sequana_laa.egg-info/SOURCES.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        1 2022-01-14 12:50:11.000000 sequana_laa-0.8.0/sequana_laa.egg-info/dependency_links.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       65 2022-01-14 12:50:11.000000 sequana_laa-0.8.0/sequana_laa.egg-info/entry_points.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        1 2022-01-14 10:06:35.000000 sequana_laa-0.8.0/sequana_laa.egg-info/not-zip-safe
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       41 2022-01-14 12:50:11.000000 sequana_laa-0.8.0/sequana_laa.egg-info/requires.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       18 2022-01-14 12:50:11.000000 sequana_laa-0.8.0/sequana_laa.egg-info/top_level.txt
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2022-01-14 12:50:11.000000 sequana_laa-0.8.0/sequana_pipelines/
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2022-01-14 12:50:11.000000 sequana_laa-0.8.0/sequana_pipelines/laa/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      121 2022-01-14 09:49:19.000000 sequana_laa-0.8.0/sequana_pipelines/laa/__init__.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1752 2022-01-14 12:15:44.000000 sequana_laa-0.8.0/sequana_pipelines/laa/config.yaml
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    95984 2022-01-14 11:03:19.000000 sequana_laa-0.8.0/sequana_pipelines/laa/dag.png
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    36652 2022-01-14 12:15:47.000000 sequana_laa-0.8.0/sequana_pipelines/laa/laa.rules
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3260 2022-01-14 10:14:12.000000 sequana_laa-0.8.0/sequana_pipelines/laa/main.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       66 2022-01-14 12:27:01.000000 sequana_laa-0.8.0/sequana_pipelines/laa/requirements.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      280 2022-01-14 09:49:19.000000 sequana_laa-0.8.0/sequana_pipelines/laa/schema.yaml
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      249 2022-01-14 12:50:11.000000 sequana_laa-0.8.0/setup.cfg
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3373 2022-01-14 12:22:06.000000 sequana_laa-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 19:32:36.000000 sequana_laa-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)      149 2022-08-30 19:32:33.000000 sequana_laa-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     5136 2022-08-30 19:32:36.000000 sequana_laa-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3069 2022-08-30 19:32:33.000000 sequana_laa-0.9.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       41 2022-08-30 19:32:33.000000 sequana_laa-0.9.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 19:32:36.000000 sequana_laa-0.9.0/sequana_laa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5136 2022-08-30 19:32:36.000000 sequana_laa-0.9.0/sequana_laa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      537 2022-08-30 19:32:36.000000 sequana_laa-0.9.0/sequana_laa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-30 19:32:36.000000 sequana_laa-0.9.0/sequana_laa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2022-08-30 19:32:36.000000 sequana_laa-0.9.0/sequana_laa.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-30 19:32:36.000000 sequana_laa-0.9.0/sequana_laa.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       41 2022-08-30 19:32:36.000000 sequana_laa-0.9.0/sequana_laa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-08-30 19:32:36.000000 sequana_laa-0.9.0/sequana_laa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 19:32:36.000000 sequana_laa-0.9.0/sequana_pipelines/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 19:32:36.000000 sequana_laa-0.9.0/sequana_pipelines/laa/
+-rw-r--r--   0 runner    (1001) docker     (121)      121 2022-08-30 19:32:33.000000 sequana_laa-0.9.0/sequana_pipelines/laa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1752 2022-08-30 19:32:33.000000 sequana_laa-0.9.0/sequana_pipelines/laa/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    95984 2022-08-30 19:32:33.000000 sequana_laa-0.9.0/sequana_pipelines/laa/dag.png
+-rw-r--r--   0 runner    (1001) docker     (121)    35082 2022-08-30 19:32:33.000000 sequana_laa-0.9.0/sequana_pipelines/laa/laa.rules
+-rw-r--r--   0 runner    (1001) docker     (121)     3344 2022-08-30 19:32:33.000000 sequana_laa-0.9.0/sequana_pipelines/laa/main.py
+-rw-r--r--   0 runner    (1001) docker     (121)       66 2022-08-30 19:32:33.000000 sequana_laa-0.9.0/sequana_pipelines/laa/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2299 2022-08-30 19:32:33.000000 sequana_laa-0.9.0/sequana_pipelines/laa/schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      249 2022-08-30 19:32:36.000000 sequana_laa-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     3325 2022-08-30 19:32:33.000000 sequana_laa-0.9.0/setup.py
```

### Comparing `sequana_laa-0.8.0/PKG-INFO` & `sequana_laa-0.9.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,134 +1,132 @@
 Metadata-Version: 2.1
 Name: sequana_laa
-Version: 0.8.0
+Version: 0.9.0
 Summary: Long read amplicon analysis
 Home-page: https://github.com/sequana/
 Author: thomas cokelaer
 Author-email: thomas.cokelaer@pasteur.fr
 Maintainer: thomas cokelaer
 Maintainer-email: thomas.cokelaer@pasteur.fr
 License: new BSD
+Description: 
+        .. image:: https://badge.fury.io/py/sequana-laa.svg
+             :target: https://pypi.python.org/pypi/sequana_laa
+        
+        .. image:: http://joss.theoj.org/papers/10.21105/joss.00352/status.svg
+            :target: http://joss.theoj.org/papers/10.21105/joss.00352
+            :alt: JOSS (journal of open source software) DOI
+        
+        .. image:: https://github.com/sequana/laa/actions/workflows/main.yml/badge.svg
+           :target: https://github.com/sequana/laa/actions/workflows/main.yml)
+        
+        
+        
+        This is is the **laa** pipeline from the `Sequana <https://sequana.readthedocs.org>`_ project
+        
+        :Overview: Perform amplicon analysis on Pacbio data sets including variant and phylogeny
+        :Input: A set of CCS files from pacbio in FastQ formats
+        :Output: variant calling, phylogney, consensus genomes, etc
+        :Status: production but may change
+        :Citation: Cokelaer et al, (2017), ‘Sequana’: a Set of Snakemake NGS pipelines, Journal of Open Source Software, 2(16), 352, JOSS DOI doi:10.21105/joss.00352
+        
+        This pipeline was used in :
+        
+        - L'Honneur et al (polyomavirus, 2022) https://pubmed.ncbi.nlm.nih.gov/34979561/ 
+        - Kali et al (rabies,2021), https://pubmed.ncbi.nlm.nih.gov/33444703/
+        - Claireaux et al. (gene involved in HIV, 2022) accepted, not yet on pubmed
+        
+        Installation
+        ~~~~~~~~~~~~
+        
+        You must install Sequana first::
+        
+            pip install sequana
+        
+        Then, just install this package::
+        
+            pip install sequana_laa
+        
+        
+        Usage
+        ~~~~~
+        
+        ::
+        
+            sequana_laa --help
+            sequana_laa --input-directory DATAPATH 
+        
+        This creates a directory with the pipeline and configuration file. You will then need 
+        to execute the pipeline::
+        
+            cd laa
+            sh laa.sh  # for a local run
+        
+        This launch a snakemake pipeline. If you are familiar with snakemake, you can 
+        retrieve the pipeline itself and its configuration files and then execute the pipeline yourself with specific parameters::
+        
+            snakemake -s laa.rules -c config.yaml --cores 4 --stats stats.txt --wrapper-prefix git+file:///home/cokelaer/Work/github/forked/sequana-wrappers
+        
+        Or use `sequanix <https://sequana.readthedocs.io/en/main/sequanix.html>`_ interface.
+        
+        Requirements
+        ~~~~~~~~~~~~
+        
+        This pipelines requires the following executable(s):
+        
+        - vt
+        - freebayes
+        - igvtools
+        - sequana
+        - snpeff (optional)
+        - samtools
+        - bamtools
+        - minimap2
+        
+        .. image:: https://raw.githubusercontent.com/sequana/laa/main/sequana_pipelines/laa/dag.png
+        
+        
+        Details
+        ~~~~~~~~~
+        
+        This pipeline runs amplicon analysis on long reads data from pacbio sequencers. 
+        
+        
+        Rules and configuration details
+        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        
+        Here is the `latest documented configuration file <https://raw.githubusercontent.com/sequana/laa/main/sequana_pipelines/laa/config.yaml>`_
+        to be used with the pipeline. Each rule used in the pipeline may have a section in the configuration file. 
+        
+        Changelog
+        ~~~~~~~~~
+        
+        ========= ====================================================================
+        Version   Description
+        ========= ====================================================================
+        0.9.0     add singularity containers
+        0.8.0     **First release.**
+        ========= ====================================================================
+        
+        
+        
 Keywords: Snakemake, Sequana, Amplicon, Variant calling, phylogeny
 Platform: Linux
 Platform: Unix
 Platform: MacOsX
 Platform: Windows
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Description-Content-Type: text/x-rst
-License-File: LICENSE
-
-
-.. image:: https://badge.fury.io/py/sequana-laa.svg
-     :target: https://pypi.python.org/pypi/sequana_laa
-
-.. image:: http://joss.theoj.org/papers/10.21105/joss.00352/status.svg
-    :target: http://joss.theoj.org/papers/10.21105/joss.00352
-    :alt: JOSS (journal of open source software) DOI
-
-.. image:: https://github.com/sequana/laa/actions/workflows/main.yml/badge.svg
-   :target: https://github.com/sequana/laa/actions/workflows/main.yml)
-
-
-
-This is is the **laa** pipeline from the `Sequana <https://sequana.readthedocs.org>`_ project
-
-:Overview: Perform amplicon analysis on Pacbio data sets including variant and phylogeny
-:Input: A set of CCS files from pacbio in FastQ formats
-:Output: variant calling, phylogney, consensus genomes, etc
-:Status: production but may change
-:Citation: Cokelaer et al, (2017), ‘Sequana’: a Set of Snakemake NGS pipelines, Journal of Open Source Software, 2(16), 352, JOSS DOI doi:10.21105/joss.00352
-
-This pipeline was used in :
-
-- L'Honneur et al (polyomavirus, 2022) https://pubmed.ncbi.nlm.nih.gov/34979561/ 
-- Kali et al (rabies,2021), https://pubmed.ncbi.nlm.nih.gov/33444703/
-- Claireaux et al. (gene involved in HIV, 2022) accepted, not yet on pubmed
-
-Installation
-~~~~~~~~~~~~
-
-You must install Sequana first::
-
-    pip install sequana
-
-Then, just install this package::
-
-    pip install sequana_laa
-
-
-Usage
-~~~~~
-
-::
-
-    sequana_laa --help
-    sequana_laa --input-directory DATAPATH 
-
-This creates a directory with the pipeline and configuration file. You will then need 
-to execute the pipeline::
-
-    cd laa
-    sh laa.sh  # for a local run
-
-This launch a snakemake pipeline. If you are familiar with snakemake, you can 
-retrieve the pipeline itself and its configuration files and then execute the pipeline yourself with specific parameters::
-
-    snakemake -s laa.rules -c config.yaml --cores 4 --stats stats.txt --wrapper-prefix git+file:///home/cokelaer/Work/github/forked/sequana-wrappers
-
-Or use `sequanix <https://sequana.readthedocs.io/en/master/sequanix.html>`_ interface.
-
-Requirements
-~~~~~~~~~~~~
-
-This pipelines requires the following executable(s):
-
-- vt
-- freebayes
-- igvtools
-- sequana
-- snpeff (optional)
-- samtools
-- bamtools
-- minimap2
-
-.. image:: https://raw.githubusercontent.com/sequana/laa/main/sequana_pipelines/laa/dag.png
-
-
-Details
-~~~~~~~~~
-
-This pipeline runs amplicon analysis on long reads data from pacbio sequencers. 
-
-
-Rules and configuration details
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-Here is the `latest documented configuration file <https://raw.githubusercontent.com/sequana/sequana_laa/master/sequana_pipelines/laa/config.yaml>`_
-to be used with the pipeline. Each rule used in the pipeline may have a section in the configuration file. 
-
-Changelog
-~~~~~~~~~
-
-========= ====================================================================
-Version   Description
-========= ====================================================================
-0.8.0     **First release.**
-========= ====================================================================
-
-
-
-
```

### Comparing `sequana_laa-0.8.0/README.rst` & `sequana_laa-0.9.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     sh laa.sh  # for a local run
 
 This launch a snakemake pipeline. If you are familiar with snakemake, you can 
 retrieve the pipeline itself and its configuration files and then execute the pipeline yourself with specific parameters::
 
     snakemake -s laa.rules -c config.yaml --cores 4 --stats stats.txt --wrapper-prefix git+file:///home/cokelaer/Work/github/forked/sequana-wrappers
 
-Or use `sequanix <https://sequana.readthedocs.io/en/master/sequanix.html>`_ interface.
+Or use `sequanix <https://sequana.readthedocs.io/en/main/sequanix.html>`_ interface.
 
 Requirements
 ~~~~~~~~~~~~
 
 This pipelines requires the following executable(s):
 
 - vt
@@ -80,20 +80,21 @@
 
 This pipeline runs amplicon analysis on long reads data from pacbio sequencers. 
 
 
 Rules and configuration details
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-Here is the `latest documented configuration file <https://raw.githubusercontent.com/sequana/sequana_laa/master/sequana_pipelines/laa/config.yaml>`_
+Here is the `latest documented configuration file <https://raw.githubusercontent.com/sequana/laa/main/sequana_pipelines/laa/config.yaml>`_
 to be used with the pipeline. Each rule used in the pipeline may have a section in the configuration file. 
 
 Changelog
 ~~~~~~~~~
 
 ========= ====================================================================
 Version   Description
 ========= ====================================================================
+0.9.0     add singularity containers
 0.8.0     **First release.**
 ========= ====================================================================
```

### Comparing `sequana_laa-0.8.0/sequana_laa.egg-info/PKG-INFO` & `sequana_laa-0.9.0/sequana_laa.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,134 +1,132 @@
 Metadata-Version: 2.1
 Name: sequana-laa
-Version: 0.8.0
+Version: 0.9.0
 Summary: Long read amplicon analysis
 Home-page: https://github.com/sequana/
 Author: thomas cokelaer
 Author-email: thomas.cokelaer@pasteur.fr
 Maintainer: thomas cokelaer
 Maintainer-email: thomas.cokelaer@pasteur.fr
 License: new BSD
+Description: 
+        .. image:: https://badge.fury.io/py/sequana-laa.svg
+             :target: https://pypi.python.org/pypi/sequana_laa
+        
+        .. image:: http://joss.theoj.org/papers/10.21105/joss.00352/status.svg
+            :target: http://joss.theoj.org/papers/10.21105/joss.00352
+            :alt: JOSS (journal of open source software) DOI
+        
+        .. image:: https://github.com/sequana/laa/actions/workflows/main.yml/badge.svg
+           :target: https://github.com/sequana/laa/actions/workflows/main.yml)
+        
+        
+        
+        This is is the **laa** pipeline from the `Sequana <https://sequana.readthedocs.org>`_ project
+        
+        :Overview: Perform amplicon analysis on Pacbio data sets including variant and phylogeny
+        :Input: A set of CCS files from pacbio in FastQ formats
+        :Output: variant calling, phylogney, consensus genomes, etc
+        :Status: production but may change
+        :Citation: Cokelaer et al, (2017), ‘Sequana’: a Set of Snakemake NGS pipelines, Journal of Open Source Software, 2(16), 352, JOSS DOI doi:10.21105/joss.00352
+        
+        This pipeline was used in :
+        
+        - L'Honneur et al (polyomavirus, 2022) https://pubmed.ncbi.nlm.nih.gov/34979561/ 
+        - Kali et al (rabies,2021), https://pubmed.ncbi.nlm.nih.gov/33444703/
+        - Claireaux et al. (gene involved in HIV, 2022) accepted, not yet on pubmed
+        
+        Installation
+        ~~~~~~~~~~~~
+        
+        You must install Sequana first::
+        
+            pip install sequana
+        
+        Then, just install this package::
+        
+            pip install sequana_laa
+        
+        
+        Usage
+        ~~~~~
+        
+        ::
+        
+            sequana_laa --help
+            sequana_laa --input-directory DATAPATH 
+        
+        This creates a directory with the pipeline and configuration file. You will then need 
+        to execute the pipeline::
+        
+            cd laa
+            sh laa.sh  # for a local run
+        
+        This launch a snakemake pipeline. If you are familiar with snakemake, you can 
+        retrieve the pipeline itself and its configuration files and then execute the pipeline yourself with specific parameters::
+        
+            snakemake -s laa.rules -c config.yaml --cores 4 --stats stats.txt --wrapper-prefix git+file:///home/cokelaer/Work/github/forked/sequana-wrappers
+        
+        Or use `sequanix <https://sequana.readthedocs.io/en/main/sequanix.html>`_ interface.
+        
+        Requirements
+        ~~~~~~~~~~~~
+        
+        This pipelines requires the following executable(s):
+        
+        - vt
+        - freebayes
+        - igvtools
+        - sequana
+        - snpeff (optional)
+        - samtools
+        - bamtools
+        - minimap2
+        
+        .. image:: https://raw.githubusercontent.com/sequana/laa/main/sequana_pipelines/laa/dag.png
+        
+        
+        Details
+        ~~~~~~~~~
+        
+        This pipeline runs amplicon analysis on long reads data from pacbio sequencers. 
+        
+        
+        Rules and configuration details
+        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        
+        Here is the `latest documented configuration file <https://raw.githubusercontent.com/sequana/laa/main/sequana_pipelines/laa/config.yaml>`_
+        to be used with the pipeline. Each rule used in the pipeline may have a section in the configuration file. 
+        
+        Changelog
+        ~~~~~~~~~
+        
+        ========= ====================================================================
+        Version   Description
+        ========= ====================================================================
+        0.9.0     add singularity containers
+        0.8.0     **First release.**
+        ========= ====================================================================
+        
+        
+        
 Keywords: Snakemake, Sequana, Amplicon, Variant calling, phylogeny
 Platform: Linux
 Platform: Unix
 Platform: MacOsX
 Platform: Windows
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Description-Content-Type: text/x-rst
-License-File: LICENSE
-
-
-.. image:: https://badge.fury.io/py/sequana-laa.svg
-     :target: https://pypi.python.org/pypi/sequana_laa
-
-.. image:: http://joss.theoj.org/papers/10.21105/joss.00352/status.svg
-    :target: http://joss.theoj.org/papers/10.21105/joss.00352
-    :alt: JOSS (journal of open source software) DOI
-
-.. image:: https://github.com/sequana/laa/actions/workflows/main.yml/badge.svg
-   :target: https://github.com/sequana/laa/actions/workflows/main.yml)
-
-
-
-This is is the **laa** pipeline from the `Sequana <https://sequana.readthedocs.org>`_ project
-
-:Overview: Perform amplicon analysis on Pacbio data sets including variant and phylogeny
-:Input: A set of CCS files from pacbio in FastQ formats
-:Output: variant calling, phylogney, consensus genomes, etc
-:Status: production but may change
-:Citation: Cokelaer et al, (2017), ‘Sequana’: a Set of Snakemake NGS pipelines, Journal of Open Source Software, 2(16), 352, JOSS DOI doi:10.21105/joss.00352
-
-This pipeline was used in :
-
-- L'Honneur et al (polyomavirus, 2022) https://pubmed.ncbi.nlm.nih.gov/34979561/ 
-- Kali et al (rabies,2021), https://pubmed.ncbi.nlm.nih.gov/33444703/
-- Claireaux et al. (gene involved in HIV, 2022) accepted, not yet on pubmed
-
-Installation
-~~~~~~~~~~~~
-
-You must install Sequana first::
-
-    pip install sequana
-
-Then, just install this package::
-
-    pip install sequana_laa
-
-
-Usage
-~~~~~
-
-::
-
-    sequana_laa --help
-    sequana_laa --input-directory DATAPATH 
-
-This creates a directory with the pipeline and configuration file. You will then need 
-to execute the pipeline::
-
-    cd laa
-    sh laa.sh  # for a local run
-
-This launch a snakemake pipeline. If you are familiar with snakemake, you can 
-retrieve the pipeline itself and its configuration files and then execute the pipeline yourself with specific parameters::
-
-    snakemake -s laa.rules -c config.yaml --cores 4 --stats stats.txt --wrapper-prefix git+file:///home/cokelaer/Work/github/forked/sequana-wrappers
-
-Or use `sequanix <https://sequana.readthedocs.io/en/master/sequanix.html>`_ interface.
-
-Requirements
-~~~~~~~~~~~~
-
-This pipelines requires the following executable(s):
-
-- vt
-- freebayes
-- igvtools
-- sequana
-- snpeff (optional)
-- samtools
-- bamtools
-- minimap2
-
-.. image:: https://raw.githubusercontent.com/sequana/laa/main/sequana_pipelines/laa/dag.png
-
-
-Details
-~~~~~~~~~
-
-This pipeline runs amplicon analysis on long reads data from pacbio sequencers. 
-
-
-Rules and configuration details
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-Here is the `latest documented configuration file <https://raw.githubusercontent.com/sequana/sequana_laa/master/sequana_pipelines/laa/config.yaml>`_
-to be used with the pipeline. Each rule used in the pipeline may have a section in the configuration file. 
-
-Changelog
-~~~~~~~~~
-
-========= ====================================================================
-Version   Description
-========= ====================================================================
-0.8.0     **First release.**
-========= ====================================================================
-
-
-
-
```

### Comparing `sequana_laa-0.8.0/sequana_laa.egg-info/SOURCES.txt` & `sequana_laa-0.9.0/sequana_laa.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,12 @@
-.coveragerc
-.gitignore
-LICENSE
 MANIFEST.in
 README.rst
-conda.yml
 requirements.txt
 setup.cfg
 setup.py
-.github/workflows/main.yml
-.github/workflows/pypi.yml
 sequana_laa.egg-info/PKG-INFO
 sequana_laa.egg-info/SOURCES.txt
 sequana_laa.egg-info/dependency_links.txt
 sequana_laa.egg-info/entry_points.txt
 sequana_laa.egg-info/not-zip-safe
 sequana_laa.egg-info/requires.txt
 sequana_laa.egg-info/top_level.txt
```

### Comparing `sequana_laa-0.8.0/sequana_pipelines/laa/config.yaml` & `sequana_laa-0.9.0/sequana_pipelines/laa/config.yaml`

 * *Files identical despite different names*

### Comparing `sequana_laa-0.8.0/sequana_pipelines/laa/dag.png` & `sequana_laa-0.9.0/sequana_pipelines/laa/dag.png`

 * *Files identical despite different names*

### Comparing `sequana_laa-0.8.0/sequana_pipelines/laa/laa.rules` & `sequana_laa-0.9.0/sequana_pipelines/laa/laa.rules`

 * *Files 4% similar despite different names*

```diff
@@ -24,35 +24,20 @@
 # ========================================================= The main config file
 #
 configfile: "config.yaml"
 
 
 # ================================================== The sequana pipeline manager
 #
-manager = sm.PipelineManagerGeneric("laa", config)
-manager.setup(globals(), mode="warning")
-config = manager.config
-
-#__snakefile__ = os.path.abspath(__snakefile__) + ".rules"
-
-
-# TEST to performed
-# set snpeff on True/False
-# set kraken on True/False   OK
-# set do_vcf_filter on/off
-
-
-
-
-M = sm.PipelineManagerGeneric("laa", config)
+manager = sm.PipelineManager("laa", config)
 
 # set reference alias
-reference = config["reference_file"]
+reference = manager.config["reference_file"]
 
-if len(M.ff) == 0:
+if len(manager.ff) == 0:
     logger.error("No files found.")
     sys.exit(0)
 
 # CHECK the input type
 #assert config['input']['data_type_choice'] in ['lima.ccs.fastq', 'lima.ccs.bam', 'subreads.bam']
 
 
@@ -64,77 +49,47 @@
 do_snpeff = config['snpeff']['do']
 do_kraken = config['kraken']['do']
 do_freebayes = config["freebayes"]["do"]
 do_split_multiallelic = config["freebayes"]["split_multiallelic"]
 do_freebayes_vcf_filter =  config["freebayes_vcf_filter"]["do"]
 
 
-
-
-"""
-smrtlink_file = config['input']['smrtlink_report_file']
-if smrtlink_file:
-    if os.path.exists(smrtlink_file) is False:
-        raise IOError("File {} does not exist".format(smrtlink_file))
-    do_smrtlink_report = True
-else:
-    do_smrtlink_report = False
-"""
-
-
-
 # identify the pattern
 
 data_type = config['data_type_choice']
 
-ccs2fastq = False
 
-if data_type == "lima.ccs.fastq":
-    for filename in M.ff.all_extensions:
-        if "--" not in filename:
-            raise ValueError("input file format must be lima_output.lbcXX--lbcXX.ccs.fastq")
-        sample = filename.split("--")[0]
-        if sample.startswith("lbc") is False:
-            raise ValueError("input file format must be lima_output.lbcXX--lbcXX.ccs.fastq")
-    samples = [sample.split('--')[0][3:] for sample in M.ff.all_extensions]
-elif data_type == "lima.ccs.bam":
-    for filename in M.ff.all_extensions:
-        if "--" not in filename:
-            raise ValueError("input file format must be lima_output.lbcXX--lbcXX.ccs.bam")
-        sample = filename.split("--")[0]
-        if sample.startswith("lbc") is False:
-            raise ValueError("input file format must be lima_output.lbcXX--lbcXX.ccs.bam")
-    samples = [sample.split('--')[0][3:] for sample in M.ff.all_extensions]
+if data_type.endswith(".fastq") or data_type.endswith(".fastq.gz"):
+    ccs2fastq = False
+elif data_type.endswith(".bam"):
     ccs2fastq = True
-elif data_type == "lima.subreads.bam":
-    raise NotImplementedError
 else:
     raise ValueError("Input file type must be one of lima.ccs.fastq, lima.ccs.bam, subreads.bam")
 
-M.samples = {tag:fl for tag, fl in zip(samples, M.ff.realpaths)}
+#manager.samples = {tag:fl for tag, fl in zip(samples, manager.ff.realpaths)}
 
 
 expected_output = [
-    expand("{sample}/images/coverage.png", sample=samples),
+    expand("{sample}/images/coverage.png", sample=manager.samples),
     "images/plot_ccs_histo.png",
     ".sequana/rulegraph.svg",
     "multiqc_report.html",
-    expand("{sample}/remapping/mapping.sorted.bam",sample=samples),
+    expand("{sample}/remapping/mapping.sorted.bam",sample=manager.samples),
     "outputs/mapping_consensus/mapping.sorted.bam",
     "outputs/raxml/RAxML_bipartitions.T3333",
     ]
 
 if do_freebayes_vcf_filter:
     expected_output.append(
-        expand("{sample}/report_variant/variant_calling.html", sample=samples)
+        expand("{sample}/report_variant/variant_calling.html", sample=manager.samples)
     )
 
-
-__phylogeny__output = "outputs/dendogram.png"
-expected_output.append(__phylogeny__output)
+if config['itol']['do']:
+    __phylogeny__output = "outputs/dendogram.png"
+    expected_output.append(__phylogeny__output)
 
 
 # Do kraken analysis ?
 if do_kraken:
    expected_output.append("images/proportion_kraken.png")
 
 
@@ -154,20 +109,17 @@
 
 
 # MUST BE ONE OF THE FIRST RULE ?
 rule pipeline:
     input:  expected_output
 
 
-# Add Conda
-__conda__output = "inputs/requirements.txt"
-include: sm.modules['conda']   # Create requirements.txt(dependencies)
 
 
-__rawdata__input = M.getrawdata()
+__rawdata__input = manager.getrawdata()
 
 
 laa = False
 if laa is True:
     # Looks like the input is not a CCS file but a raw bam files after lima
     # 6 mins on BC25 of project 812 so we use protected
     rule laa:
@@ -266,59 +218,76 @@
         sorted_bam = "{sample}/mapping/mapping.sorted.bam",
         bam = temp("{sample}/mapping/mapping.bam"),
         sam = temp("{sample}/mapping/mapping.sam"),
     params:
         reference = reference
     log:
         "{sample}/mapping/mapping.log"
-    threads: 4
+    threads: 
+        4
+    container:
+        "https://zenodo.org/record/7031863/files/sequana_tools_0.14.2.img"
     shell:
         """
-    minimap2 -x map-pb {input.reference} {input.fastq} -t {threads} -a 1> {output.sam} 2>{log}
-    bioconvert sam2bam {output.sam} {output.bam} --force
-    bamtools sort -in {output.bam} -out {output.sorted_bam}
+        minimap2 -x map-pb {input.reference} {input.fastq} -t {threads} -a 1> {output.sam} 2>{log}
+        samtools view -bh {output.sam} > {output.bam} 
+        bamtools sort -in {output.bam} -out {output.sorted_bam}
         """
 
 
 rule samtools_stats:
     input: "{sample}/mapping/mapping.sorted.bam"
     output: "{sample}/mapping/samtools_{sample}.txt"
+    container:
+        "https://zenodo.org/record/7031863/files/sequana_tools_0.14.2.img"
     shell:
         "samtools stats -in {input} > {output}"
 
 
 rule bamtools_stats:
     input: "{sample}/mapping/mapping.sorted.bam"
     output: "{sample}/mapping/sequana_bamtools_stats_{sample}.txt"
+    container:
+        "https://zenodo.org/record/7031863/files/sequana_tools_0.14.2.img"
     shell:
         "bamtools stats -in {input} > {output}"
 
 
 rule mapping_index:
         input: "{sample}/mapping/mapping.sorted.bam"
         output: "{sample}/mapping/mapping.sorted.bam.bai"
-        threads: 1
-        shell: "bamtools index -in {input}"
+        threads: 
+            1
+        container:
+            "https://zenodo.org/record/7031863/files/sequana_tools_0.14.2.img"
+        shell: 
+            "bamtools index -in {input}"
 
 
 if do_freebayes:
     __freebayes__input = "{sample}/mapping/mapping.sorted.bam"
     __freebayes__reference = reference
     __freebayes__output = "{sample}/freebayes/variants.raw.vcf"
     __freebayes__log = "{sample}/freebayes/freebayes.log"
     include: sm.modules["freebayes"]
 
 if do_split_multiallelic:
 
     __split_multiallelic__output = "{sample}/freebayes/variants.raw.split.vcf" 
     rule split_multiallelic:
-        input: __freebayes__output
-        output: "{sample}/freebayes/variants.raw.split.vcf"
+        input: 
+            __freebayes__output
+        output: 
+            "{sample}/freebayes/variants.raw.split.vcf"
+        container:
+            "https://zenodo.org/record/7031863/files/sequana_tools_0.14.2.img"
         shell:
-            """bcftools norm -m -both {input} | vt decompose_blocksub - > {output}"""
+            """
+            bcftools norm -m -both {input} | vt decompose_blocksub - > {output}
+            """
     __freebayes__output = __split_multiallelic__output
 
 
 
 if do_freebayes and do_snpeff:
     __snpeff__input = __freebayes__output
     __snpeff__output = "{sample}/snpeff/variants.ann.vcf"
@@ -348,107 +317,82 @@
     # samtools mpileup -R -B -f ../../reference/CCR5_whole_locus.fasta
     # mapping.sorted.bam > out
     #
     input: "{sample}/mapping/mapping.sorted.bam.bai"
     output: "{sample}/igvtools/bases.txt"
     params:
         reference = reference
-    log: "{sample}/igvtools/coverage.log"
+    log: 
+        "{sample}/igvtools/coverage.log"
+    #container:
+    #    "https://zenodo.org/record/7031863/files/sequana_tools_0.14.2.img"
     run:
         input = input[0].replace(".bai", "")
         cmd = "igvtools count {input} stdout {params.reference} -w 1 --bases 1> {output} 2>{log}"
         shell(cmd)
 
 
 rule igv_count:
-    input: "{sample}/mapping/mapping.sorted.bam.bai"
-    output: "{sample}/igvtools/coverage.txt"
+    input: 
+        "{sample}/mapping/mapping.sorted.bam.bai"
+    output: 
+        "{sample}/igvtools/coverage.txt"
     params:
         reference = reference
-    log: "{sample}/igvtools/coverage.log"
+    log: 
+        "{sample}/igvtools/coverage.log"
+    #container:
+    #    "https://zenodo.org/record/7022635/files/igvtools_2.12.0.img"
     run:
         input = input[0].replace(".bai", "")
         cmd = "igvtools count {input} stdout {params.reference} -w 1 > {output} 2>{log}"
         shell(cmd)
 
 
 rule coverage:
-    input: "{sample}/igvtools/coverage.txt"
-    output: "{sample}/images/coverage.png"
+    input:
+        "{sample}/igvtools/coverage.txt"
+    output:
+        "{sample}/images/coverage.png"
     run:
         from pylab import savefig, ylim, xlabel
         import pandas as pd
-        df  = pd.read_csv(input[0], skiprows=2, sep="\t", index_col=0, header=None)
+        try:df  = pd.read_csv(input[0], skiprows=2, sep="\t",  header=None)
+        except:df  = pd.read_csv(input[0], skiprows=4, sep="\t", header=None)
         df.plot(legend=False)
         ylim([0, max(ylim())])
         xlabel("position", fontsize=16)
         savefig(output[0], dpi=150)
 
-"""  DOES NOT WORK when using snakemake in the rulegraph/ directory
-# TODO merge with sequana/rulegraph
-__rulegraph__input = __snakefile__
-__rulegraph__output="rulegraph/rulegraph.svg"
-__rulegraph__mapper = {
-    "kraken": "../kraken/kraken.html",
-}
-include: sm.modules['rulegraph']
-#expected_output.extend([__rulegraph__output])
-"""
-
 
 
 rule rulegraph:
     input: str(manager.snakefile)
     output:
         svg = ".sequana/rulegraph.svg"
     params:
         mapper = {"multiqc": "../multiqc/multiqc_report.html"},
         configname = "config.yaml"
     wrapper:
         "main/wrappers/rulegraph"
 
 
-__rulegraph__output=".sequanah/rulegraph.svg"
-"""rule rulegraph:
-    input: __snakefile__.replace("rulegraph/", "")
-    output:
-        svg = __rulegraph__output,
-        dot = temp("rg.dot"),
-        dot2 = temp("rg.ann.dot"),
-    run:
-        import os
-        cwd = os.getcwd()
-        from sequana import SequanaConfig, DOTParser
-        from subprocess import Popen
-
-        cmd = "snakemake -s {} --rulegraph --nolock ".format(input[0])
-        # There is an error message caught by the PIPE
-        with open("rg.dot", "w") as fl:
-            p = Popen(cmd.split(), stdout=fl, stderr=subprocess.PIPE)
-            p.wait()
-        d = DOTParser(cwd + os.sep + output.dot)
-        d.add_urls(mapper={
-            #"sequana_kraken": "kraken.html",
-            #"create_proportion_plot_kraken": "images/proportion_kraken.png",
-            #"plot_ccs_histo": "images/plot_ccs_histo.png"
-        })
-        shell("dot -Tsvg {} -o {}".format(output.dot2, output.svg))
-"""
 
 if do_snpeff:
     __multiqc__input = (
-        expand("{sample}/snpeff/{sample}.snpeff.csv", sample=samples),
-        expand("{sample}/mapping/samtools_{sample}.txt", sample=samples),
-        expand("{sample}/mapping/sequana_bamtools_stats_{sample}.txt", sample=samples),
-        expand("{sample}/sequana_laa_{sample}.json", sample=samples))
+        expand("{sample}/snpeff/{sample}.snpeff.csv", sample=manager.samples),
+        expand("{sample}/mapping/samtools_{sample}.txt", sample=manager.samples),
+        expand("{sample}/mapping/sequana_bamtools_stats_{sample}.txt", sample=manager.samples),
+        expand("{sample}/sequana_laa_{sample}.json", sample=manager.samples))
 else:
     __multiqc__input = (
-        expand("{sample}/mapping/samtools_{sample}.txt", sample=samples),
-        expand("{sample}/mapping/sequana_bamtools_stats_{sample}.txt", sample=samples),
-        expand("{sample}/sequana_laa_{sample}.json", sample=samples))
+        expand("{sample}/mapping/samtools_{sample}.txt", sample=manager.samples),
+        expand("{sample}/mapping/sequana_bamtools_stats_{sample}.txt", sample=manager.samples),
+        expand("{sample}/sequana_laa_{sample}.json", sample=manager.samples))
+
 
 from sequana import sequana_data
 rule multiqc:
     input:
         __multiqc__input
     output: "multiqc_report.html"
     params:
@@ -562,15 +506,18 @@
 
     """
     input:
         reference= reference,
         fasta="outputs/allfasta.fa"
     output:
         aln="outputs/mafft/mafft.aln.fa"
-    threads: 2
+    threads: 
+        2
+    container:
+        "https://zenodo.org/record/7031863/files/sequana_tools_0.14.2.img"
     shell:
         """
         mafft --thread {threads} --retree 1 --maxiterate 0 --add {input.fasta} \
         --keeplength {input.reference} > {output.aln}
         """
 
 
@@ -596,28 +543,25 @@
         aln = "outputs/mafft/mafft.aln.fa"
     output:
         tree = "outputs/raxml/RAxML_bestTree.T1111",
         log = "outputs/raxml/raxml_parcimony.log",
     threads: 4
     params:
         N=config['raxml_mltree']['N'],
-        options=config['raxml_mltree']['options']
-    run:
+        options=config['raxml_mltree']['options'],
+        wkdir=os.path.abspath("outputs/raxml")
+    container:
+        "https://zenodo.org/record/7031863/files/sequana_tools_0.14.2.img"
+    shell:
+        """
         # First, let us get a best likelihood tree from 20 ML trees
-        shell("mkdir -p outputs/raxml")
-        shell("rm -f outputs/raxml/*T1111*")
-
-        cmd = "raxmlHPC-PTHREADS -m GTRGAMMA -s {}".format(input.aln)
-        cmd += " -p 12345 "
-        cmd += " -T {} ".format(threads)
-        cmd += " -w {}".format(os.path.abspath("outputs/raxml"))
-        cmd += " -N {}".format(params.N)
-        cmd += " -n T1111 1>{}".format(output.log)
-
-        shell(cmd)
+        mkdir -p outputs/raxml && \
+        rm -f outputs/raxml/*T1111* &&\
+        raxmlHPC-PTHREADS -m GTRGAMMA -s {input.aln}  -p 12345  -T {threads} -w {params.wkdir} -N {params.N} -n T1111 1>{output.log}
+        """
 
 
 rule raxml_bootstrap:
     """
     If we want to do bootstrapinp, we need to use the -b option (seed)::
 
         raxmlHPC -m GTRGAMMA -p 12345 -b 12345 -N 100 -s aln.fa -n T2
@@ -676,47 +620,47 @@
         cmd += " -w {}".format(os.path.abspath("outputs/raxml"))
         cmd += " -t {}".format(input.best)
         cmd += " -z {}".format(input.boot)
         cmd += " -n T3333 "  # 1>{} ".format(output.log)
 
         shell(cmd)
 
+if config['itol']['do']:
+    rule itol:
+        """
+            https://github.com/albertyw/itolapi
 
-rule itol:
-    """
-        https://github.com/albertyw/itolapi
+        """
+        input:
+            best="outputs/raxml/RAxML_bestTree.T1111",
+            boot="outputs/raxml/RAxML_bootstrap.T2222"
+        output:
+            png="outputs/dendogram.png",
+            svg="outputs/dendogram.svg",
+            pdf="outputs/dendogram.pdf"
+        run:
+            shell("mkdir -p outputs/itol")
+            shell("cp {} {}".format(input.best, "outputs/itol/tree_of_life.tree.txt"))
 
-    """
-    input:
-        best="outputs/raxml/RAxML_bestTree.T1111",
-        boot="outputs/raxml/RAxML_bootstrap.T2222"
-    output:
-        png="outputs/dendogram.png",
-        svg="outputs/dendogram.svg",
-        pdf="outputs/dendogram.pdf"
-    run:
-        shell("mkdir -p outputs/itol")
-        shell("cp {} {}".format(input.best, "outputs/itol/tree_of_life.tree.txt"))
+            from sequana import ITOL
 
-        from sequana import ITOL
-        
-        itol = ITOL("outputs/itol/tree_of_life.tree.txt")
-        itol.params['treeName'] = "amplicon"
-        itol.upload()
-
-        itol.params['display_mode'] = 2
-        itol.params['ignore_branch_length'] = 1
-        itol.params['line_width'] = 5
-        itol.params['bootstrap_display'] = 1
-        itol.params['bootstrap_type'] = 4
-        itol.params['bootstrap_label_size'] = 32
-
-        itol.export(output.png)
-        itol.export(output.svg)
-        itol.export(output.pdf)
+            itol = ITOL("outputs/itol/tree_of_life.tree.txt")
+            itol.params['treeName'] = "amplicon"
+            itol.upload()
+
+            itol.params['display_mode'] = 2
+            itol.params['ignore_branch_length'] = 1
+            itol.params['line_width'] = 5
+            itol.params['bootstrap_display'] = 1
+            itol.params['bootstrap_type'] = 4
+            itol.params['bootstrap_label_size'] = 32
+
+            itol.export(output.png)
+            itol.export(output.svg)
+            itol.export(output.pdf)
 
 
 rule mapping_consensus:
     input: 
         reference=reference,
         consensus="outputs/allfasta.fa"
     output:
@@ -755,22 +699,22 @@
         bioconvert sam2bam {output.sam} {output.bam} --force
         bamtools sort -in {output.bam} -out {output.sorted_bam}
         bamtools index -in {output.sorted_bam}
         """
 
 
 rule build_fasta:
-    input: expand("{sample}/consensus/consensus.fa", sample=sorted(samples))
+    input: expand("{sample}/consensus/consensus.fa", sample=sorted(manager.samples))
     output: "outputs/allfasta.fa"
     shell: "cat {input} > {output}"
 
 
 if do_kraken:
     rule sequana_kraken:
-        #input: lambda wildcards: M.samples[wildcards.sample]
+        #input: lambda wildcards: manager.samples[wildcards.sample]
         input: __sequana_kraken__input
         output:
             html="{sample}/taxonomy/summary.html",
             csv= "{sample}/taxonomy/kraken/kraken.csv"
         threads: 4
         run:
             #print(input)
@@ -782,15 +726,15 @@
             for this in config['kraken']['databases']:
                 assert os.path.exists(this), "databases {} does not exits".format(this)
                 cmd += " {} ".format(this)
             shell(cmd)
 
 
 rule plot_ccs_histo:
-    input: M.ff.realpaths
+    input: manager.ff.realpaths
     output: "images/plot_ccs_histo.png"
     run:
         from sequana import FastQ
         data = [len(FastQ(filename)) for filename in input]
         from pylab import plot, hist, savefig, xlabel
         hist(data, bins=10, lw=1, edgecolor="k")
         xlabel("Number of reads (in CCS bam file) per bar code", fontsize=16)
@@ -834,36 +778,36 @@
 
             pylab.clf()
             bc.plot_subreads_histogram()
             savefile("barcoding_subreads_histogram.png")
 
 
 if do_snpeff:
-    localrules: conda, copy_genbank, copy_reference, itol
+    localrules: copy_genbank, copy_reference, itol
 else:
-    localrules: conda, copy_reference, itol
+    localrules: copy_reference, itol
 
 
 onsuccess:
 
-    shell("rm -f igv.log")
     from sequana.modules_report.summary import SummaryModule
     from sequana.modules_report.kraken import KrakenModule
 
+    manager.teardown(extra_files_to_remove=['igv.log'])
 
     intro = """
       <h2>Amplicon Analysis Summary.</h2> <br>
       <br><b>Number of samples:</b> {} </br>
       <b> MultiQC report: </b> <a href="multiqc_report.html">multiqc report.</a> This multiqc report contains comparative analysis for the different analysis performed by the pipeline including the snpeff, raw reads information (e.g. number of CCS reads in each barcode), taxonomic analysis, variant calling (using freebayes) and some mapping statistics. 
 
 Here below you can find all individual links to HTML reports for each sample for snpeff, kraken and freebayes analysis.
 
 
 
- <h2>Directory Tree (for one sample, here named 25)</h2><p>
+ <h2>Directory Tree </h2><p>
 
   Each barcode (sample) is analysed and the corresponding results are stored in a 
   tree structure similar to this one (summary):
 
  <a href=".">.</a><br>
  ├── <a href="./25/">25</a><br>
  │   ├── <a href="./25/consensus/">consensus</a><br>
@@ -971,61 +915,64 @@
         """
 
     if do_kraken:
         intro += """<h2>Kraken analysis</h2>
       <p>Proportion of reads in virus, bacteria, human and unclassified categories:</p>
       <img src="images/proportion_kraken.png"></img><br>
         """
-        for sample in sorted(samples):
+        for sample in sorted(manager.samples):
             intro += """<a href="{}/taxonomy/summary.html">{}/kraken</a><br>""".format(sample, sample)
 
 
     if do_snpeff:
         intro += """<div><h2>SNP annotations</h2><p>Here below are links to
 SNPEff reports and variant calling reports. For a snpeff summary, please see
 this <a href="multiqc_report.html">multiqc report.</a></p>
         """
-        for sample in sorted(samples):
+        for sample in sorted(manager.samples):
             intro += """<a href="{}/snpeff/snpeff.html">{}/snpeff.html</a><br>""".format(sample, sample)
         intro += "</div>"
 
     else:
         intro +="""<p>No SNPEFF report available (was not required). Please see variant reports instead</p></div>"""
 
     intro += "<div><h2>Variant reports</h2>"
-    for sample in sorted(samples):
+    for sample in sorted(manager.samples):
         intro += """<a href="{}/report_variant/variant_calling.html">{}/variant report</a><br>""".format(sample, sample)
 
-    intro += "<div><h2>Phylogeny</h2><img src={}></img></div>".format(__phylogeny__output)
+    try:intro += "<div><h2>Phylogeny</h2><img src={}></img></div>".format(__phylogeny__output)
+    except NameError:pass
 
 
-    intro = intro.format(len(M.ff))
+    intro = intro.format(len(manager.ff))
 
-    data = {"inputs":None, "outputs":None, "html":None, "snakefile": __snakefile__,
-          "config": "config.yaml", "stats": "stats.txt", "rulegraph": __rulegraph__output,
+    data = {"inputs":None, "outputs":None, "html":None, "snakefile": "laa.rules",
+          "config": "config.yaml", "stats": "stats.txt", "rulegraph": ".sequana/rulegraph.svg",
           "requirements": "inputs/requirements.txt"}
 
     s = SummaryModule(data, intro=intro)
 
     if do_kraken:
         from sequana.utils import config as conf
-        for sample in sorted(samples):
+        for sample in sorted(manager.samples):
             sample_summary = {}
 
             conf.summary_sections = []
             conf.output_dir = "{}".format(sample)
 
             k = KrakenModule( sample + "/taxonomy/kraken")
             sample_summary['kraken_json'] = json.loads(k._get_stats().to_json())
             conf.summary_sections.append({
                 "name": "Kraken ",
                 "anchor'": "kraken",
                 "content": k._get_summary_section()
             })
 
 
-    from sequana.snaketools import Makefile, OnSuccess
-    sm.OnSuccess()
+    shell("chmod -R g+w .")
+    shell("rm -rf rulegraph")
 
 onerror:
-    print("An error occurred. See messages above.")
+    from sequana_pipetools.errors import PipeError
+    p = PipeError("laa")
+    p.status()
```

### Comparing `sequana_laa-0.8.0/sequana_pipelines/laa/main.py` & `sequana_laa-0.9.0/sequana_pipelines/laa/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         so.add_options(self)
 
         so = GeneralOptions()
         so.add_options(self)
 
         pipeline_group = self.add_argument_group("pipeline")
 
-        pipeline_group.add_argument("--TODO", dest="TODO", default=4, type=int)
+        pipeline_group.add_argument("--reference-file", dest="reference", required=True, type=str)
 
     def parse_args(self, *args):
         args_list = list(*args)
         if "--from-project" in args_list:
             if len(args_list) > 2:
                 msg = (
                     "WARNING [sequana]: With --from-project option, "
@@ -93,14 +93,16 @@
         # fill the config file with input parameters
         cfg = manager.config.config
         # EXAMPLE TOREPLACE WITH YOUR NEEDS
         cfg.input_directory = os.path.abspath(options.input_directory)
         cfg.input_pattern = options.input_pattern
         manager.exists(cfg.input_directory)
 
+        cfg.reference_file = os.path.abspath(options.reference)
+
     # finalise the command and save it; copy the snakemake. update the config
     # file and save it.
     manager.teardown()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `sequana_laa-0.8.0/setup.py` & `sequana_laa-0.9.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-# -*- coding: utf-8 -*-
-# License: 3-clause BSD
 from setuptools import setup, find_namespace_packages
 from setuptools.command.develop import develop
 from setuptools.command.install import install
 import subprocess
 
 
 # handle sequana git link
 with open("requirements.txt") as fh:
     requirements = [req.rstrip() if not req.startswith("git+") else req.rstrip().split("egg=")[-1] for req in fh]
 
 
 _MAJOR               = 0
-_MINOR               = 8
+_MINOR               = 9
 _MICRO               = 0
 version = f"{_MAJOR}.{_MINOR}.{_MICRO}"
 release = f"{_MAJOR}.{_MINOR}"
 
 
 metainfo = {
     'authors': {"main": ("thomas cokelaer", "thomas.cokelaer@pasteur.fr")},
@@ -31,17 +29,17 @@
           #'Development Status :: 5 - Production/Stable',
           'Intended Audience :: Education',
           'Intended Audience :: End Users/Desktop',
           'Intended Audience :: Developers',
           'Intended Audience :: Science/Research',
           'License :: OSI Approved :: BSD License',
           'Operating System :: OS Independent',
-          'Programming Language :: Python :: 3.6',
           'Programming Language :: Python :: 3.7',
           'Programming Language :: Python :: 3.8',
+          'Programming Language :: Python :: 3.9',
           'Topic :: Software Development :: Libraries :: Python Modules',
           'Topic :: Scientific/Engineering :: Bio-Informatics',
           'Topic :: Scientific/Engineering :: Information Analysis',
           'Topic :: Scientific/Engineering :: Mathematics',
           'Topic :: Scientific/Engineering :: Physics']
     }
```

