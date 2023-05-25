# Comparing `tmp/cosmosis-2.4.1.tar.gz` & `tmp/cosmosis-2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cosmosis-2.4.1.tar", last modified: Mon Apr 24 13:28:36 2023, max compression
+gzip compressed data, was "cosmosis-2.5.tar", last modified: Thu May 25 15:56:25 2023, max compression
```

## Comparing `cosmosis-2.4.1.tar` & `cosmosis-2.5.tar`

### file list

```diff
@@ -1,280 +1,280 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.600744 cosmosis-2.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-24 13:28:34.000000 cosmosis-2.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-04-24 13:28:34.000000 cosmosis-2.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-24 13:28:36.600744 cosmosis-2.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-24 13:28:34.000000 cosmosis-2.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.580744 cosmosis-2.4.1/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      102 2023-04-24 13:28:34.000000 cosmosis-2.4.1/bin/cosmosis
--rwxr-xr-x   0 runner    (1001) docker     (123)      792 2023-04-24 13:28:34.000000 cosmosis-2.4.1/bin/cosmosis-configure
--rwxr-xr-x   0 runner    (1001) docker     (123)     1442 2023-04-24 13:28:34.000000 cosmosis-2.4.1/bin/cosmosis-extract
--rwxr-xr-x   0 runner    (1001) docker     (123)      102 2023-04-24 13:28:34.000000 cosmosis-2.4.1/bin/cosmosis-postprocess
--rwxr-xr-x   0 runner    (1001) docker     (123)     1527 2023-04-24 13:28:34.000000 cosmosis-2.4.1/bin/cosmosis-sample-fisher
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.580744 cosmosis-2.4.1/cosmosis/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.580744 cosmosis-2.4.1/cosmosis/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/config/compilers.mk
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/config/subdirs.mk
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/configure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.584744 cosmosis-2.4.1/cosmosis/datablock/
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51706 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/c_datablock.cc
--rw-r--r--   0 runner    (1001) docker     (123)    22811 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/c_datablock.h
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/clamp.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/cosmosis_constants.fh
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/cosmosis_constants.h
--rw-r--r--   0 runner    (1001) docker     (123)    34029 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/cosmosis_modules.F90
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.584744 cosmosis-2.4.1/cosmosis/datablock/cosmosis_py/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/cosmosis_py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52767 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/cosmosis_py/block.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/cosmosis_py/dbt_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/cosmosis_py/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/cosmosis_py/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/cosmosis_py/section_names.py
--rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/cosmosis_section_names.F90
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/cosmosis_types.F90
--rw-r--r--   0 runner    (1001) docker     (123)    28871 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/cosmosis_wrappers.F90
--rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/datablock.cc
--rw-r--r--   0 runner    (1001) docker     (123)    11258 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/datablock.hh
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/datablock_logging.cc
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/datablock_logging.h
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/datablock_status.h
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/datablock_types.h
--rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/entry.cc
--rw-r--r--   0 runner    (1001) docker     (123)    11879 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/entry.hh
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/exceptions.hh
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/generate_sections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/handler.c
--rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/ndarray.hh
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/section.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/section.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/section_names.h
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/datablock/section_names.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14009 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/gaussian_likelihood.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17782 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/names.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.584744 cosmosis-2.4.1/cosmosis/output/
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/output/cosmomc_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     6545 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/output/fits_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/output/in_memory_output.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/output/null_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     8092 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/output/output_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9534 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/output/text_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/output/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.584744 cosmosis-2.4.1/cosmosis/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/plotting/chain_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/plotting/grid_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/plotting/kde.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      404 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/plotting/plot_demo_3.py
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/plotting/plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/plotting/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6941 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/postprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.588744 cosmosis-2.4.1/cosmosis/postprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/postprocessing/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16163 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/postprocessing/cosmology_theory_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     9643 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/postprocessing/density.py
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/postprocessing/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/postprocessing/inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/postprocessing/latex.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/postprocessing/lazy_pylab.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/postprocessing/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    41832 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/postprocessing/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    10359 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/postprocessing/postprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/postprocessing/postprocess_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/postprocessing/reruns.py
--rw-r--r--   0 runner    (1001) docker     (123)    33731 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/postprocessing/statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/postprocessing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.588744 cosmosis-2.4.1/cosmosis/runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/runtime/analytics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/runtime/attribution.py
--rw-r--r--   0 runner    (1001) docker     (123)    17211 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/runtime/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/runtime/declare.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/runtime/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.588744 cosmosis-2.4.1/cosmosis/runtime/julia_modules/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/runtime/julia_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/runtime/julia_modules/julia.py
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/runtime/memmon.py
--rw-r--r--   0 runner    (1001) docker     (123)    17250 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/runtime/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/runtime/mpi_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    12277 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/runtime/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    56629 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/runtime/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    21210 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/runtime/prior.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/runtime/process_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/runtime/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.588744 cosmosis-2.4.1/cosmosis/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.588744 cosmosis-2.4.1/cosmosis/samplers/abc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/abc/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7126 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/abc/abc_sampler.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6698 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/abc/abc_sampler_mpi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.588744 cosmosis-2.4.1/cosmosis/samplers/apriori/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/apriori/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2262 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/apriori/apriori_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.588744 cosmosis-2.4.1/cosmosis/samplers/dynesty/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/dynesty/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3600 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/dynesty/dynesty_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.588744 cosmosis-2.4.1/cosmosis/samplers/emcee/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/emcee/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7265 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/emcee/emcee_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.588744 cosmosis-2.4.1/cosmosis/samplers/fisher/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/fisher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/fisher/fisher.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6726 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/fisher/fisher_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.592744 cosmosis-2.4.1/cosmosis/samplers/grid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/grid/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4715 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/grid/grid_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.592744 cosmosis-2.4.1/cosmosis/samplers/gridmax/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/gridmax/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4411 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/gridmax/gridmax_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/hints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.592744 cosmosis-2.4.1/cosmosis/samplers/importance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/importance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/importance/importance_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.592744 cosmosis-2.4.1/cosmosis/samplers/kombine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/kombine/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5406 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/kombine/kombine_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.592744 cosmosis-2.4.1/cosmosis/samplers/list/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/list/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4843 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/list/list_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.592744 cosmosis-2.4.1/cosmosis/samplers/maxlike/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/maxlike/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4790 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/maxlike/maxlike_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.592744 cosmosis-2.4.1/cosmosis/samplers/metropolis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/metropolis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10500 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/metropolis/metropolis.py
--rw-r--r--   0 runner    (1001) docker     (123)     9755 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/metropolis/metropolis_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.592744 cosmosis-2.4.1/cosmosis/samplers/metropolis/proposal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/metropolis/proposal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/metropolis/proposal/cobaya_proposal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/metropolis/proposal/standard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.592744 cosmosis-2.4.1/cosmosis/samplers/minuit/
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/minuit/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/minuit/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7592 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/minuit/minuit_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/minuit/minuit_wrapper.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.592744 cosmosis-2.4.1/cosmosis/samplers/multinest/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/multinest/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/multinest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/multinest/multinest_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.592744 cosmosis-2.4.1/cosmosis/samplers/multinest/multinest_src/
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/multinest/multinest_src/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/multinest/multinest_src/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    19512 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/multinest/multinest_src/README
--rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/multinest/multinest_src/cwrapper.f90
--rw-r--r--   0 runner    (1001) docker     (123)    42915 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/multinest/multinest_src/kmeans_clstr.f90
--rw-r--r--   0 runner    (1001) docker     (123)   106166 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/multinest/multinest_src/nested.f90
--rw-r--r--   0 runner    (1001) docker     (123)    22010 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/multinest/multinest_src/posterior.f90
--rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/multinest/multinest_src/priors.f90
--rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/multinest/multinest_src/utils.f90
--rw-r--r--   0 runner    (1001) docker     (123)    28039 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/multinest/multinest_src/utils1.f90
--rw-r--r--   0 runner    (1001) docker     (123)    86938 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/multinest/multinest_src/xmeans_clstr.f90
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.596744 cosmosis-2.4.1/cosmosis/samplers/nautilus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/nautilus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/nautilus/nautilus_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.596744 cosmosis-2.4.1/cosmosis/samplers/pmaxlike/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/pmaxlike/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4537 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/pmaxlike/pmaxlike_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.596744 cosmosis-2.4.1/cosmosis/samplers/pmc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/pmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/pmc/pmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/pmc/pmc_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.596744 cosmosis-2.4.1/cosmosis/samplers/poco/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/poco/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3675 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/poco/poco_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.596744 cosmosis-2.4.1/cosmosis/samplers/polychord/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/polychord/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/polychord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13001 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.596744 cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/README
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/abort.F90
--rw-r--r--   0 runner    (1001) docker     (123)    18110 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/array_utils.f90
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/c_interface.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/calculate.f90
--rw-r--r--   0 runner    (1001) docker     (123)     9725 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/chordal_sampling.f90
--rw-r--r--   0 runner    (1001) docker     (123)    10196 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/clustering.f90
--rw-r--r--   0 runner    (1001) docker     (123)    13421 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/feedback.f90
--rw-r--r--   0 runner    (1001) docker     (123)    26147 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/generate.F90
--rw-r--r--   0 runner    (1001) docker     (123)    19077 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/ini.f90
--rw-r--r--   0 runner    (1001) docker     (123)    20999 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/interfaces.F90
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/interfaces.h
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/interfaces.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    24257 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/mpi_utils.F90
--rw-r--r--   0 runner    (1001) docker     (123)    20674 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/nested_sampling.F90
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/params.f90
--rw-r--r--   0 runner    (1001) docker     (123)    19675 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/priors.f90
--rw-r--r--   0 runner    (1001) docker     (123)    18291 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/random_utils.F90
--rw-r--r--   0 runner    (1001) docker     (123)    44750 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/read_write.f90
--rw-r--r--   0 runner    (1001) docker     (123)    47427 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/run_time_info.f90
--rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/settings.f90
--rw-r--r--   0 runner    (1001) docker     (123)    29353 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/utils.F90
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.596744 cosmosis-2.4.1/cosmosis/samplers/pymc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/pymc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7345 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/pymc/pymc_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9337 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.596744 cosmosis-2.4.1/cosmosis/samplers/snake/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/snake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/snake/snake.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1974 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/snake/snake_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.600744 cosmosis-2.4.1/cosmosis/samplers/star/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/star/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4422 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/star/star_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.600744 cosmosis-2.4.1/cosmosis/samplers/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/test/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3221 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/test/test_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.600744 cosmosis-2.4.1/cosmosis/samplers/zeus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/zeus/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11516 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/samplers/zeus/zeus_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.600744 cosmosis-2.4.1/cosmosis/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.600744 cosmosis-2.4.1/cosmosis/test/libtest/
--rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/libtest/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/libtest/c_datablock_complex_array_test.c
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/libtest/c_datablock_double_array_test.c
--rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/libtest/c_datablock_int_array_test.c
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/libtest/c_datablock_multidim_complex_array_test.c
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/libtest/c_datablock_multidim_double_array_test.c
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/libtest/c_datablock_multidim_int_array_test.c
--rw-r--r--   0 runner    (1001) docker     (123)    11722 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/libtest/c_datablock_test.c
--rw-r--r--   0 runner    (1001) docker     (123)    11117 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/libtest/cosmosis_test.F90
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/libtest/cosmosis_tests.supp
--rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/libtest/datablock_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/libtest/entry_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/libtest/ndarray_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/libtest/section_test.cc
--rw-r--r--   0 runner    (1001) docker     (123)    28088 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/libtest/test_c_datablock_scalars.h
--rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/libtest/test_c_datablock_scalars.template
--rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/test_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/test_chaining.py
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/test_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/test_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/test_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/test_module2.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/test_module3.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/test_module4.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/test_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/test_polychord.py
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/test_samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/test_text_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-24 13:28:34.000000 cosmosis-2.4.1/cosmosis/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:28:36.580744 cosmosis-2.4.1/cosmosis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-24 13:28:36.000000 cosmosis-2.4.1/cosmosis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8924 2023-04-24 13:28:36.000000 cosmosis-2.4.1/cosmosis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 13:28:36.000000 cosmosis-2.4.1/cosmosis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-24 13:28:36.000000 cosmosis-2.4.1/cosmosis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-24 13:28:36.000000 cosmosis-2.4.1/cosmosis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-24 13:28:34.000000 cosmosis-2.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 13:28:36.600744 cosmosis-2.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-04-24 13:28:34.000000 cosmosis-2.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:25.721619 cosmosis-2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-25 15:56:23.000000 cosmosis-2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-05-25 15:56:23.000000 cosmosis-2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-25 15:56:25.721619 cosmosis-2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-25 15:56:23.000000 cosmosis-2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:25.681618 cosmosis-2.5/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      102 2023-05-25 15:56:23.000000 cosmosis-2.5/bin/cosmosis
+-rwxr-xr-x   0 runner    (1001) docker     (123)      792 2023-05-25 15:56:23.000000 cosmosis-2.5/bin/cosmosis-configure
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1442 2023-05-25 15:56:23.000000 cosmosis-2.5/bin/cosmosis-extract
+-rwxr-xr-x   0 runner    (1001) docker     (123)      102 2023-05-25 15:56:23.000000 cosmosis-2.5/bin/cosmosis-postprocess
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1527 2023-05-25 15:56:23.000000 cosmosis-2.5/bin/cosmosis-sample-fisher
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:25.681618 cosmosis-2.5/cosmosis/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:25.685618 cosmosis-2.5/cosmosis/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/config/compilers.mk
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/config/subdirs.mk
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:25.689618 cosmosis-2.5/cosmosis/datablock/
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/datablock/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/datablock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51706 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/datablock/c_datablock.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    22811 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/datablock/c_datablock.h
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/datablock/clamp.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/datablock/cosmosis_constants.fh
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/datablock/cosmosis_constants.h
+-rw-r--r--   0 runner    (1001) docker     (123)    34029 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/datablock/cosmosis_modules.F90
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:25.689618 cosmosis-2.5/cosmosis/datablock/cosmosis_py/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/datablock/cosmosis_py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52767 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/datablock/cosmosis_py/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/datablock/cosmosis_py/dbt_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/datablock/cosmosis_py/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/datablock/cosmosis_py/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/datablock/cosmosis_py/section_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/datablock/cosmosis_section_names.F90
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/datablock/cosmosis_types.F90
+-rw-r--r--   0 runner    (1001) docker     (123)    28871 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/datablock/cosmosis_wrappers.F90
+-rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/datablock/datablock.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    11258 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/datablock/datablock.hh
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/datablock/datablock_logging.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/datablock/datablock_logging.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/datablock/datablock_status.h
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/datablock/datablock_types.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/datablock/entry.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    11879 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/datablock/entry.hh
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/datablock/exceptions.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/datablock/generate_sections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/datablock/handler.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/datablock/ndarray.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/datablock/section.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/datablock/section.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/datablock/section_names.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/datablock/section_names.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14009 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/gaussian_likelihood.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17838 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/names.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:25.689618 cosmosis-2.5/cosmosis/output/
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/output/cosmomc_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6545 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/output/fits_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/output/in_memory_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/output/null_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8092 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/output/output_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9534 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/output/text_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/output/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:25.693618 cosmosis-2.5/cosmosis/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/plotting/chain_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/plotting/grid_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/plotting/kde.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      404 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/plotting/plot_demo_3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/plotting/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/plotting/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7217 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/postprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:25.693618 cosmosis-2.5/cosmosis/postprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/postprocessing/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16163 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/postprocessing/cosmology_theory_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9643 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/postprocessing/density.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/postprocessing/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/postprocessing/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/postprocessing/latex.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/postprocessing/lazy_pylab.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/postprocessing/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48757 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/postprocessing/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10076 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/postprocessing/postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/postprocessing/postprocess_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/postprocessing/reruns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33731 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/postprocessing/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/postprocessing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:25.697618 cosmosis-2.5/cosmosis/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/runtime/analytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/runtime/attribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17211 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/runtime/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/runtime/declare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/runtime/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:25.697618 cosmosis-2.5/cosmosis/runtime/julia_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/runtime/julia_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/runtime/julia_modules/julia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/runtime/memmon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17250 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/runtime/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/runtime/mpi_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12277 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/runtime/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56629 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/runtime/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21210 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/runtime/prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/runtime/process_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/runtime/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:25.697618 cosmosis-2.5/cosmosis/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:25.697618 cosmosis-2.5/cosmosis/samplers/abc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/abc/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7126 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/abc/abc_sampler.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6698 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/abc/abc_sampler_mpi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:25.697618 cosmosis-2.5/cosmosis/samplers/apriori/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/apriori/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2262 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/apriori/apriori_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:25.701618 cosmosis-2.5/cosmosis/samplers/dynesty/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/dynesty/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3600 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/dynesty/dynesty_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:25.701618 cosmosis-2.5/cosmosis/samplers/emcee/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/emcee/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7265 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/emcee/emcee_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:25.701618 cosmosis-2.5/cosmosis/samplers/fisher/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/fisher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/fisher/fisher.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6726 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/fisher/fisher_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:25.701618 cosmosis-2.5/cosmosis/samplers/grid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/grid/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4715 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/grid/grid_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:25.701618 cosmosis-2.5/cosmosis/samplers/gridmax/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/gridmax/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4411 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/gridmax/gridmax_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/hints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:25.701618 cosmosis-2.5/cosmosis/samplers/importance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/importance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/importance/importance_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:25.701618 cosmosis-2.5/cosmosis/samplers/kombine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/kombine/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5406 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/kombine/kombine_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:25.701618 cosmosis-2.5/cosmosis/samplers/list/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/list/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4843 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/list/list_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:25.701618 cosmosis-2.5/cosmosis/samplers/maxlike/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/maxlike/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4790 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/maxlike/maxlike_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:25.701618 cosmosis-2.5/cosmosis/samplers/metropolis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/metropolis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10500 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/metropolis/metropolis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9755 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/metropolis/metropolis_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:25.705618 cosmosis-2.5/cosmosis/samplers/metropolis/proposal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/metropolis/proposal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/metropolis/proposal/cobaya_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/metropolis/proposal/standard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:25.705618 cosmosis-2.5/cosmosis/samplers/minuit/
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/minuit/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/minuit/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7592 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/minuit/minuit_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/minuit/minuit_wrapper.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:25.705618 cosmosis-2.5/cosmosis/samplers/multinest/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/multinest/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/multinest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/multinest/multinest_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:25.705618 cosmosis-2.5/cosmosis/samplers/multinest/multinest_src/
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/multinest/multinest_src/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/multinest/multinest_src/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    19512 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/multinest/multinest_src/README
+-rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/multinest/multinest_src/cwrapper.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    42915 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/multinest/multinest_src/kmeans_clstr.f90
+-rw-r--r--   0 runner    (1001) docker     (123)   106166 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/multinest/multinest_src/nested.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    22010 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/multinest/multinest_src/posterior.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/multinest/multinest_src/priors.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/multinest/multinest_src/utils.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    28039 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/multinest/multinest_src/utils1.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    86938 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/multinest/multinest_src/xmeans_clstr.f90
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:25.709618 cosmosis-2.5/cosmosis/samplers/nautilus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/nautilus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/nautilus/nautilus_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:25.709618 cosmosis-2.5/cosmosis/samplers/pmaxlike/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/pmaxlike/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4537 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/pmaxlike/pmaxlike_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:25.709618 cosmosis-2.5/cosmosis/samplers/pmc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/pmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/pmc/pmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/pmc/pmc_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:25.709618 cosmosis-2.5/cosmosis/samplers/poco/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/poco/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3675 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/poco/poco_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:25.709618 cosmosis-2.5/cosmosis/samplers/polychord/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/polychord/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/polychord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13001 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/polychord/polychord_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:25.713619 cosmosis-2.5/cosmosis/samplers/polychord/polychord_src/
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/polychord/polychord_src/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/polychord/polychord_src/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/polychord/polychord_src/README
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/polychord/polychord_src/abort.F90
+-rw-r--r--   0 runner    (1001) docker     (123)    18110 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/polychord/polychord_src/array_utils.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/polychord/polychord_src/c_interface.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/polychord/polychord_src/calculate.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     9725 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/polychord/polychord_src/chordal_sampling.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    10196 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/polychord/polychord_src/clustering.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    13421 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/polychord/polychord_src/feedback.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    26147 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/polychord/polychord_src/generate.F90
+-rw-r--r--   0 runner    (1001) docker     (123)    19077 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/polychord/polychord_src/ini.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    20999 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/polychord/polychord_src/interfaces.F90
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/polychord/polychord_src/interfaces.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/polychord/polychord_src/interfaces.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    24257 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/polychord/polychord_src/mpi_utils.F90
+-rw-r--r--   0 runner    (1001) docker     (123)    20674 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/polychord/polychord_src/nested_sampling.F90
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/polychord/polychord_src/params.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    19675 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/polychord/polychord_src/priors.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    18291 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/polychord/polychord_src/random_utils.F90
+-rw-r--r--   0 runner    (1001) docker     (123)    44750 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/polychord/polychord_src/read_write.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    47427 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/polychord/polychord_src/run_time_info.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/polychord/polychord_src/settings.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    29353 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/polychord/polychord_src/utils.F90
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:25.713619 cosmosis-2.5/cosmosis/samplers/pymc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/pymc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7345 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/pymc/pymc_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9337 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:25.713619 cosmosis-2.5/cosmosis/samplers/snake/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/snake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/snake/snake.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1974 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/snake/snake_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:25.721619 cosmosis-2.5/cosmosis/samplers/star/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/star/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4422 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/star/star_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:25.721619 cosmosis-2.5/cosmosis/samplers/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/test/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3221 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/test/test_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:25.721619 cosmosis-2.5/cosmosis/samplers/zeus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/zeus/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11516 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/samplers/zeus/zeus_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:25.721619 cosmosis-2.5/cosmosis/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:25.721619 cosmosis-2.5/cosmosis/test/libtest/
+-rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/test/libtest/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/test/libtest/c_datablock_complex_array_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/test/libtest/c_datablock_double_array_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/test/libtest/c_datablock_int_array_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/test/libtest/c_datablock_multidim_complex_array_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/test/libtest/c_datablock_multidim_double_array_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/test/libtest/c_datablock_multidim_int_array_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11722 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/test/libtest/c_datablock_test.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11117 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/test/libtest/cosmosis_test.F90
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/test/libtest/cosmosis_tests.supp
+-rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/test/libtest/datablock_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/test/libtest/entry_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/test/libtest/ndarray_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/test/libtest/section_test.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    28088 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/test/libtest/test_c_datablock_scalars.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/test/libtest/test_c_datablock_scalars.template
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/test/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/test/test_chaining.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/test/test_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/test/test_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/test/test_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/test/test_module2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/test/test_module3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/test/test_module4.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/test/test_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/test/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/test/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/test/test_polychord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/test/test_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/test/test_text_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-25 15:56:23.000000 cosmosis-2.5/cosmosis/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:56:25.685618 cosmosis-2.5/cosmosis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-25 15:56:25.000000 cosmosis-2.5/cosmosis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8924 2023-05-25 15:56:25.000000 cosmosis-2.5/cosmosis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 15:56:25.000000 cosmosis-2.5/cosmosis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-25 15:56:25.000000 cosmosis-2.5/cosmosis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-25 15:56:25.000000 cosmosis-2.5/cosmosis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-25 15:56:23.000000 cosmosis-2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 15:56:25.721619 cosmosis-2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-05-25 15:56:23.000000 cosmosis-2.5/setup.py
```

### Comparing `cosmosis-2.4.1/LICENSE` & `cosmosis-2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/MANIFEST.in` & `cosmosis-2.5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/bin/cosmosis-configure` & `cosmosis-2.5/bin/cosmosis-configure`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/bin/cosmosis-extract` & `cosmosis-2.5/bin/cosmosis-extract`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/bin/cosmosis-sample-fisher` & `cosmosis-2.5/bin/cosmosis-sample-fisher`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/__init__.py` & `cosmosis-2.5/cosmosis/__init__.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/config/compilers.mk` & `cosmosis-2.5/cosmosis/config/compilers.mk`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/configure.py` & `cosmosis-2.5/cosmosis/configure.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/constants.py` & `cosmosis-2.5/cosmosis/constants.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/datablock/Makefile` & `cosmosis-2.5/cosmosis/datablock/Makefile`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/datablock/c_datablock.cc` & `cosmosis-2.5/cosmosis/datablock/c_datablock.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/datablock/c_datablock.h` & `cosmosis-2.5/cosmosis/datablock/c_datablock.h`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/datablock/clamp.hh` & `cosmosis-2.5/cosmosis/datablock/clamp.hh`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/datablock/cosmosis_constants.fh` & `cosmosis-2.5/cosmosis/datablock/cosmosis_constants.fh`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/datablock/cosmosis_constants.h` & `cosmosis-2.5/cosmosis/datablock/cosmosis_constants.h`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/datablock/cosmosis_modules.F90` & `cosmosis-2.5/cosmosis/datablock/cosmosis_modules.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/datablock/cosmosis_py/block.py` & `cosmosis-2.5/cosmosis/datablock/cosmosis_py/block.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/datablock/cosmosis_py/errors.py` & `cosmosis-2.5/cosmosis/datablock/cosmosis_py/errors.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/datablock/cosmosis_py/lib.py` & `cosmosis-2.5/cosmosis/datablock/cosmosis_py/lib.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/datablock/cosmosis_py/section_names.py` & `cosmosis-2.5/cosmosis/datablock/cosmosis_py/section_names.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/datablock/cosmosis_section_names.F90` & `cosmosis-2.5/cosmosis/datablock/cosmosis_section_names.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/datablock/cosmosis_wrappers.F90` & `cosmosis-2.5/cosmosis/datablock/cosmosis_wrappers.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/datablock/datablock.cc` & `cosmosis-2.5/cosmosis/datablock/datablock.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/datablock/datablock.hh` & `cosmosis-2.5/cosmosis/datablock/datablock.hh`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/datablock/datablock_logging.cc` & `cosmosis-2.5/cosmosis/datablock/datablock_logging.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/datablock/datablock_logging.h` & `cosmosis-2.5/cosmosis/datablock/datablock_logging.h`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/datablock/datablock_status.h` & `cosmosis-2.5/cosmosis/datablock/datablock_status.h`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/datablock/entry.cc` & `cosmosis-2.5/cosmosis/datablock/entry.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/datablock/entry.hh` & `cosmosis-2.5/cosmosis/datablock/entry.hh`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/datablock/generate_sections.py` & `cosmosis-2.5/cosmosis/datablock/generate_sections.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/datablock/handler.c` & `cosmosis-2.5/cosmosis/datablock/handler.c`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/datablock/ndarray.hh` & `cosmosis-2.5/cosmosis/datablock/ndarray.hh`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/datablock/section.cc` & `cosmosis-2.5/cosmosis/datablock/section.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/datablock/section.hh` & `cosmosis-2.5/cosmosis/datablock/section.hh`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/datablock/section_names.h` & `cosmosis-2.5/cosmosis/datablock/section_names.h`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/datablock/section_names.txt` & `cosmosis-2.5/cosmosis/datablock/section_names.txt`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/gaussian_likelihood.py` & `cosmosis-2.5/cosmosis/gaussian_likelihood.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/main.py` & `cosmosis-2.5/cosmosis/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,15 +158,15 @@
 
     if ("filename" in output_options):
         print("* Saving output -> {}".format(output_options['filename']))
 
     return output
 
 
-def run_cosmosis(args, pool=None, ini=None, pipeline=None, values=None):
+def run_cosmosis(args, pool=None, ini=None, pipeline=None, values=None, priors=None):
     no_subprocesses = os.environ.get("COSMOSIS_NO_SUBPROCESS", "") not in ["", "0"]
     # In case we need to hand-hold a naive demo-10 user.
 
     # Load configuration.
     is_root = (pool is None) or pool.is_master()
     if ini is None:
         ini = Inifile(args.inifile, override=args.params, print_include_messages=is_root)
@@ -196,22 +196,22 @@
         profile.enable()
 
     # Create pipeline.
     if pipeline is None:
         cleanup_pipeline = True
         pool_stdout = ini.getboolean(RUNTIME_INI_SECTION, "pool_stdout", fallback=False)
         if is_root or pool_stdout:
-            pipeline = LikelihoodPipeline(ini, override=args.variables, values=values, only=args.only)
+            pipeline = LikelihoodPipeline(ini, override=args.variables, values=values, only=args.only, priors=priors)
         else:
             # Suppress output on everything except the master process
             if pool_stdout:
-                pipeline = LikelihoodPipeline(ini, override=args.variables, only=args.only) 
+                pipeline = LikelihoodPipeline(ini, override=args.variables, only=args.only, priors=priors)
             else:
                 with stdout_redirected():
-                    pipeline = LikelihoodPipeline(ini, override=args.variables, only=args.only) 
+                    pipeline = LikelihoodPipeline(ini, override=args.variables, only=args.only, priors=priors)
 
         if pipeline.do_fast_slow:
             pipeline.setup_fast_subspaces()
     else:
         # We should not cleanup a pipeline which we didn't make
         cleanup_pipeline = False
```

### Comparing `cosmosis-2.4.1/cosmosis/output/__init__.py` & `cosmosis-2.5/cosmosis/output/__init__.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/output/cosmomc_output.py` & `cosmosis-2.5/cosmosis/output/cosmomc_output.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/output/fits_output.py` & `cosmosis-2.5/cosmosis/output/fits_output.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/output/in_memory_output.py` & `cosmosis-2.5/cosmosis/output/in_memory_output.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/output/null_output.py` & `cosmosis-2.5/cosmosis/output/null_output.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/output/output_base.py` & `cosmosis-2.5/cosmosis/output/output_base.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/output/text_output.py` & `cosmosis-2.5/cosmosis/output/text_output.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/output/utils.py` & `cosmosis-2.5/cosmosis/output/utils.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/plotting/chain_plots.py` & `cosmosis-2.5/cosmosis/plotting/chain_plots.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/plotting/grid_plots.py` & `cosmosis-2.5/cosmosis/plotting/grid_plots.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/plotting/kde.py` & `cosmosis-2.5/cosmosis/plotting/kde.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/plotting/plotter.py` & `cosmosis-2.5/cosmosis/plotting/plotter.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/postprocess.py` & `cosmosis-2.5/cosmosis/postprocess.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,20 +31,23 @@
 
 plots=parser.add_argument_group(title="Plotting", description="Plotting options")
 plots.add_argument("--legend", help="Add a legend to the plot with the specified titles, separated by | (the pipe symbol)")
 plots.add_argument("--legend-loc", default='best', help="The location of the legend: best, UR, UL, LL, LR, R, CL, CR, LC, UC, C (use quotes for the ones with two words.)")
 plots.add_argument("--swap", action='store_true', help="Swap the ordering of the parameters in (x,y)")
 plots.add_argument("--only", type=str, dest='prefix_only', help="Only make 2D plots where both parameter names start with this")
 plots.add_argument("--either", type=str, dest='prefix_either', help="Only make 2D plots where one of the parameter names starts with this.")
+parser.add_argument("--exclude", nargs="+", dest='prefix_exclude', help='Specify one or more prefixes to exclude matching parameters from 2D plots')
+
 plots.add_argument("--no-plots", action='store_true', help="Do not make any default plots")
 plots.add_argument("--no-2d", action='store_true', help="Do not make any 2D plots")
 plots.add_argument("--no-alpha", dest='alpha', action='store_false', help="No alpha effect - shaded contours will not be visible through other ones")
 plots.add_argument("-f", "--file-type", default="png", help="Filename suffix for plots")
 plots.add_argument("--no-smooth", dest='smooth', default=True, action='store_false', help="Do not smooth grid plot joint constraints")
-plots.add_argument("--fix-edges", dest='fix_edges', default=False, action='store_true', help="Use an alternative KDE to fix 1D plot boundaries")
+plots.add_argument("--fix-edges", dest='fix_edges', default=True, action='store_true', help="Use an alternative KDE to fix 1D plot boundaries")
+plots.add_argument("--no-fix-edges", dest='fix_edges', default=False, action='store_false', help="Switch off the edge fixing")
 plots.add_argument("--n-kde", default=100, type=int, help="Number of KDE smoothing points per dimension to use for MCMC 2D curves. Reduce to speed up, but can make plots look worse.")
 plots.add_argument("--factor-kde", default=2.0, type=float, help="Smoothing factor for MCMC plots.  More makes plots look better but can smooth out too much.")
 plots.add_argument("--no-fill", dest='fill', default=True, action='store_false', help="Do not fill in 2D constraint plots with color")
 plots.add_argument("--extra", dest='extra', default="", help="Load extra post-processing steps from this file.")
 plots.add_argument("--tweaks", dest='tweaks', default="", help="Load plot tweaks from this file.")
 plots.add_argument("--no-image", dest='image', default=True, action='store_false', help="Do not plot the image in  2D grids; just show the contours")
 plots.add_argument("--run-max-post", default="", help="Run the test sampler on maximum-posterior sample and save to the named directory.")
```

### Comparing `cosmosis-2.4.1/cosmosis/postprocessing/__init__.py` & `cosmosis-2.5/cosmosis/postprocessing/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,29 +18,33 @@
     FisherProcessor,
     StarProcessor,
 )
 from .plots import (
     GridPlots1D,
     GridPlots2D,
     SnakePlots2D,
-    MetropolisHastingsPlots1D,
-    MetropolisHastingsPlots2D,
+    MetropolisHastingsPlots,
     TestPlots,
-    WeightedPlots1D,
-    WeightedPlots2D,
-    MultinestPlots1D,
-    MultinestPlots2D,
-    PolychordPlots1D,
-    PolychordPlots2D,
-    WeightedMetropolisPlots1D,
-    WeightedMetropolisPlots2D,
-    TrianglePlot,
+    WeightedPlots,
+    MultinestPlots,
+    PolychordPlots,
+    WeightedMetropolisPlots,
     MCMCColorScatterPlot,
     WeightedMCMCColorScatterPlot,
     MultinestColorScatterPlot,
     PolychordColorScatterPlot,
     CovarianceMatrixGaussians,
     CovarianceMatrixEllipse,
     StarPlots,
     Tweaks,
+    # These are deprecated:
+    MetropolisHastingsPlots1D,
+    WeightedMetropolisPlots1D,
+    MultinestPlots1D,
+    PolychordPlots1D,
+    MetropolisHastingsPlots2D,
+    WeightedMetropolisPlots2D,
+    MultinestPlots2D,
+    PolychordPlots2D,
+
 )
 from .reruns import BestFitRerunner, ini_from_header
```

### Comparing `cosmosis-2.4.1/cosmosis/postprocessing/cosmology_theory_plots.py` & `cosmosis-2.5/cosmosis/postprocessing/cosmology_theory_plots.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/postprocessing/density.py` & `cosmosis-2.5/cosmosis/postprocessing/density.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/postprocessing/elements.py` & `cosmosis-2.5/cosmosis/postprocessing/elements.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/postprocessing/inputs.py` & `cosmosis-2.5/cosmosis/postprocessing/inputs.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/postprocessing/latex.ini` & `cosmosis-2.5/cosmosis/postprocessing/latex.ini`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/postprocessing/lazy_pylab.py` & `cosmosis-2.5/cosmosis/postprocessing/lazy_pylab.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/postprocessing/outputs.py` & `cosmosis-2.5/cosmosis/postprocessing/outputs.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/postprocessing/plots.py` & `cosmosis-2.5/cosmosis/postprocessing/plots.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 from . import cosmology_theory_plots
 import configparser
 import numpy as np
 import scipy.optimize
 from . import lazy_pylab as pylab
 import itertools
 import os
-import sys
-import collections
+import warnings
+
 
 default_latex_file = os.path.join(os.path.split(__file__)[0], "latex.ini")
 legend_locations = {
 "BEST": 0,
 "UR": 1,
 "UL": 2,
 "LL": 3,
@@ -39,14 +39,15 @@
         latex_file = self.options.get("more_latex") 
         self._latex = {}
         self.plot_set = self.source.index
         if self.source.cosmosis_standard_output and not self.no_latex:
             self.load_latex(latex_file)
         self.quiet =  False
         self.truth = None
+        self.cache = {}
         truth = self.options.get("truth")
         if truth:
             self.truth = {str(p): p.start for p in Parameter.load_parameters(truth)}
 
     def finalize(self):
         super(Plots, self).finalize()
         legend = self.options.get("legend", "")
@@ -169,28 +170,32 @@
         return col, light_col
 
 
     def parameter_pairs(self):
         swap=self.options.get("swap")
         prefix_only = self.options.get("prefix_only")
         prefix_either = self.options.get("prefix_either")
+        prefix_exclude = self.options.get("prefix_exclude")
         #only overrides either
 
         for name1 in self.source.colnames[:]:
             for name2 in self.source.colnames[:]:
                 if name1<=name2: continue
                 if prefix_only and not (
                     name1.startswith(prefix_only)
                 and name2.startswith(prefix_only)
                     ): continue
                 elif prefix_either and not (
                     name1.startswith(prefix_either)
                 or name2.startswith(prefix_either)
                     ): continue
-
+                if prefix_exclude and any([name1.startswith(p) for p in prefix_exclude]):
+                    continue
+                if prefix_exclude and any([name2.startswith(p) for p in prefix_exclude]):
+                    continue
                 if name1.lower() in self.excluded_columns: continue
                 if name2.lower() in self.excluded_columns: continue
                 if swap:
                     yield name2,name1
                 else:
                     yield name1, name2
 
@@ -343,16 +348,16 @@
         cols1 = self.source.get_col(name1)
         cols2 = self.source.get_col(name2)
         try: like = self.source.get_col("post")
         except: like = self.source.get_col("like")
         vals1 = np.unique(cols1)
         vals2 = np.unique(cols2)
 
-        n1 = self.nsample_dimension
-        n2 = self.nsample_dimension
+        n1 = int(self.nsample_dimension)
+        n2 = n1
 
         like = like - like.max()
 
         #Marginalize over all the other parameters by summing
         #them up
         like_sum = np.zeros((n1,n2))
         for k,(v1, v2) in enumerate(itertools.product(vals1, vals2)):
@@ -459,15 +464,15 @@
         like -= like.max()
         like = np.exp(like).reshape((n1,n2)).T
         extent=(left1, right1, left2, right2)
 
         return extent, like
 
 
-class MetropolisHastingsPlots(Plots, MCMCPostProcessorElement):
+class MetropolisHastingsPlotsBase(Plots, MCMCPostProcessorElement):
     excluded_columns = ["like","post", "prior"]
 
 def get_param_limits(source, name):
     values = source.extract_ini("VALUES")
     priors = source.extract_ini("PRIORS")
     params = Parameter.load_parameters(values, [priors])
     i = params.index(name)
@@ -491,30 +496,36 @@
         near_boundary = True
     else:
         xmin = x.min()
 
     return xmin, xmax, near_boundary
 
 
+def next_entry(l, m):
+    return m[(l.index(m) + 1)%len(m)]
+
+
+class MetropolisHastingsPlots(MetropolisHastingsPlotsBase):
+    def run(self):
+        return self.run_1d() + self.run_2d()
 
-class MetropolisHastingsPlots1D(MetropolisHastingsPlots):
     def keywords_1d(self):
         return {}
 
-    def smooth_likelihood(self, x, name):
+    def smooth_likelihood_1d(self, x, name):
         #Interpolate using KDE
         if self.options.get("fix_edges"):
-            return self.smooth_likelihood_with_boundaries(x, name)
+            return self.smooth_likelihood_with_boundaries_1d(x, name)
         n = self.options.get("n_kde", 100)
         factor = self.options.get("factor_kde", 2.0)
         kde = KDE(x, factor=factor)
         x_axis, like = kde.grid_evaluate(n, (x.min(), x.max()) )
         return x_axis, like
 
-    def smooth_likelihood_with_boundaries(self, x, name):
+    def smooth_likelihood_with_boundaries_1d(self, x, name):
         # find the limits on this parameter
         factor = self.options.get("factor_kde", 2.0)
         xmin, xmax, fix = select_limits(x, self.source, name)
         xout, like = smooth_density_estimate_1d(x, xmin, xmax,
                             smoothing=factor, fix_boundary=fix)
         cut = (xout >= x.min()) & (xout <= x.max())
         return xout[cut], like[cut]
@@ -526,43 +537,39 @@
             print(" - 1D plot ", name)
         if figure is None:
             figure, filename = self.figure(name)
         else:
             filename = None
         if x.max()-x.min()==0: return
 
-        x_axis, like = self.smooth_likelihood(x, name)
+        x_axis, like = self.smooth_likelihood_1d(x, name)
         like/=like.max()
+        self.cache[name] = x_axis, like
 
         #Choose colors
         color = self.line_color()
 
         #Make the plot
         pylab.figure(figure.number)
         keywords = self.keywords_1d()
         pylab.plot(x_axis, like, '-', color=color, lw=2, label=self.source.label,  **keywords)
         pylab.xlabel(self.latex(name, dollar=True))
         if not hasattr(figure, 'cosmosis_done_truth'):
             self.plot_truth_1d(name)
             figure.cosmosis_done_truth = True
         return filename
 
-    def run(self):
+    def run_1d(self):
         filenames = []
         for name in self.source.colnames:
             if name.lower() in self.excluded_columns: continue
             filename = self.make_1d_plot(name)
             if filename: filenames.append(filename)
         return filenames
 
-def next_entry(l, m):
-    return m[(l.index(m) + 1)%len(m)]
-
-class MetropolisHastingsPlots2D(MetropolisHastingsPlots):
-
     def keywords_2d(self):
         return {}
 
     def _find_contours(self, like, x, y, x_axis, y_axis, contour1, contour2):
         N = len(x)
         hx = 0.5 * (x_axis[1] - x_axis[0])
         hy = 0.5 * (y_axis[1] - y_axis[0])
@@ -577,40 +584,153 @@
             return count.sum() - target
         target1 = N*(1-contour1)
         target2 = N*(1-contour2)
         level1 = scipy.optimize.bisect(objective, like.min(), like.max(), args=(target1,))
         level2 = scipy.optimize.bisect(objective, like.min(), like.max(), args=(target2,))
         return level1, level2, like.sum()
 
-    def smooth_likelihood(self, x, y, xname, yname):
+    def smooth_likelihood_2d(self, x, y, xname, yname):
         if self.options.get("fix_edges"):
-            return self.smooth_likelihood_with_boundaries(x, y, xname, yname)
+            return self.smooth_likelihood_with_boundaries_2d(x, y, xname, yname)
 
         n = self.options.get("n_kde", 100)
         factor = self.options.get("factor_kde", 2.0)
         kde = KDE([x,y], factor=factor)
         x_range = (x.min(), x.max())
         y_range = (y.min(), y.max())
         (x_axis, y_axis), like = kde.grid_evaluate(n, [x_range, y_range])
         return x_axis, y_axis, like
 
-    def smooth_likelihood_with_boundaries(self, x, y, xname, yname):
+    def smooth_likelihood_with_boundaries_2d(self, x, y, xname, yname):
         factor = self.options.get("factor_kde", 2.0)
         xmin, xmax, fix_x = select_limits(x, self.source, xname)
         ymin, ymax, fix_y = select_limits(y, self.source, yname)
         xout, yout, like = smooth_density_estimate_2d(x, y, xmin, xmax, ymin, ymax,
                             smoothing=factor, fix_boundary=fix_x or fix_y)
         xcut = np.where((xout >= x.min()) & (xout <= x.max()))[0]
         ycut = np.where((yout >= y.min()) & (yout <= y.max()))[0]
         xcut0 = xcut.min()
         xcut1 = xcut.max() + 1
         ycut0 = ycut.min()
         ycut1 = ycut.max() + 1
         return xout[xcut0:xcut1], yout[ycut0:ycut1], like[xcut0:xcut1, ycut0:ycut1]
 
+    def make_corner_plot(self, figure=None):
+        from matplotlib.ticker import AutoMinorLocator, AutoLocator, ScalarFormatter
+        from matplotlib.axis import Ticker
+
+        pairs = list(self.parameter_pairs())
+
+        # parameters, in the order we will use
+        params = list(dict.fromkeys([p[0] for p in pairs]))
+        nparam = len(params)
+        fig, filename = self.figure("corner")
+
+        # enlarge for this extra big figure
+        size = min(4 * nparam, 24)
+        fig.set_size_inches(size, size)
+
+        axes = fig.subplots(nparam, nparam, squeeze=False)
+        for i in range(nparam):
+            for j in range(nparam):
+                ax = axes[i, j]
+
+                # Switch on minor ticks and have them point inwards like sensible people
+                ax.tick_params(direction='in', which='both', bottom=True, left=True)
+                ax.tick_params(which='minor', length=5, bottom=True, left=True)
+                ax.minorticks_on()
+
+                # Remove upper right above diagonal
+                if j > i:
+                    fig.delaxes(ax)
+                    continue
+
+                p1 = params[j]
+                p2 = params[i]
+                if i == j:
+                    # Left column only has a y-label, and others also have no y tick labels
+                    # and only the bottom row as an x-label, and others have no x ticks.
+                    # Top left is labelled "Posterior"
+                    # Only the bottom row has
+                    if i == 0:
+                        ax.set_ylabel("Posterior")
+                    else:
+                        ax.yaxis.set_ticklabels([])
+                    if j == nparam - 1:
+                        ax.set_xlabel(self.latex(p2))
+                    else:
+                        ax.xaxis.set_ticklabels([])
+
+                    if nparam > 10:
+                        ax.xaxis.set_ticklabels([])
+
+                    # Use the same 1D information as in the 1D plots
+                    x, like = self.cache[p1]
+
+                    # Plot and set the limits explicitly.
+                    # Trying to use the sharex / sharey feature here is painful
+                    # because we want to remove the diagonal, and that seems to make
+                    # the tick stuff really fiddly.
+                    ax.plot(x, like / like.max(), color=self.line_color())
+                    ax.set_xlim(x.min(), x.max())
+                    ax.set_ylim(0, 1.1)
+
+                    # ax.tick_params(axis='both', which='minor', bottom=True, left=True)
+
+                else:
+                    # We might have done the swap thing, in which case
+                    # check both directions.
+                    # If the user has done some funny things with the --only or --either
+                    # parameters then things might get funny here, so allow missing panels.
+                    try:
+                        x, y, like, levels = self.cache[p1, p2]
+                    except KeyError:
+                        # we have to switch the parameter ordering in this case,
+                        # and flip the contours
+                        try:
+                            x, y, like, levels = self.cache[p2, p1]
+                            x, y = y, x
+                            like = like.T
+                        except KeyError:
+                            continue
+                    color = self.line_color()
+
+                    # This is the same contour code as in the main 2D plot code
+                    ax.contour(x, y, like, levels=levels[:2], colors=color)
+
+                    # As with the 1D plots on the diagonal we have to remove
+                    # the labelling from most of the panels.
+                    if i == nparam - 1:
+                        ax.set_xlabel(self.latex(p1))
+                    else:
+                        ax.xaxis.set_ticklabels([])
+                    if j == 0:
+                        ax.set_ylabel(self.latex(p2))
+                    else:
+                        ax.yaxis.set_ticklabels([])
+
+                    if nparam > 10:
+                        ax.xaxis.set_ticklabels([])
+
+                    # Explicitly set the ranges so that they are the
+                    # same for all the panels. To ensure that axes are identical to
+                    # the 1D version we set them to the same range as that.
+
+                    x1, _ = self.cache[p1]
+                    y1, _ = self.cache[p2]
+
+                    ax.set_xlim(x1.min(), x1.max())
+                    ax.set_ylim(y1.min(), y1.max())
+
+        fig.tight_layout()
+        fig.subplots_adjust(hspace=0.04, wspace=0.08)
+        return filename
+
+
+
     def make_2d_plot(self, name1, name2, figure=None):
         #Get the data
         x = self.reduced_col(name1)
         y = self.reduced_col(name2)
 
 
         if x.max()-x.min()==0 or y.max()-y.min()==0:
@@ -618,15 +738,15 @@
 
         if not self.quiet:
             print("  (making %s vs %s)" % (name1, name2))
 
 
         #Interpolate using KDE
         try:
-            x_axis, y_axis, like = self.smooth_likelihood(x, y, name1, name2)
+            x_axis, y_axis, like = self.smooth_likelihood_2d(x, y, name1, name2)
         except np.linalg.LinAlgError:
             print("  -- these two parameters have singular covariance - probably a linear relation")
             print("Not making a 2D plot of them")
             return []
 
         if figure is None:
             figure, filename = self.figure("2D", name1, name2)
@@ -645,14 +765,16 @@
         #Make the plot
         pylab.figure(figure.number)
         keywords = self.keywords_2d()
         fill = self.options.get("fill", True)
         imshow = self.options.get("imshow", False)
         plot_points = self.options.get("plot_points", False)
 
+        self.cache[name1, name2] = (x_axis, y_axis, like.T, levels)
+
         if imshow:
             pylab.imshow(like.T, extent=(x_axis[0], x_axis[-1], y_axis[0], y_axis[-1]), aspect='auto', origin='lower')
             pylab.colorbar()
         elif fill:
             dark,light = self.shade_colors()
             pylab.contourf(x_axis, y_axis, like.T, [level2,level0], colors=[light], alpha=0.25)
             pylab.contourf(x_axis, y_axis, like.T, [level1,level0], colors=[dark], alpha=0.25)
@@ -673,15 +795,15 @@
         if not hasattr(figure, 'cosmosis_done_truth'):
             self.plot_truth_2d(name1, name2)
             figure.cosmosis_done_truth = True
         
         return filename        
 
 
-    def run(self):
+    def run_2d(self):
         if self.options.get("no_2d", False):
             print("Not making any 2D plots because you said --no-2d")
             return []
         filenames = []
         print("(Making 2D plots using KDE; this takes a while but is really cool)")
         for name1,name2 in self.parameter_pairs():
                 try:
@@ -691,14 +813,15 @@
                 except: #any other error we just continue
                     import traceback
                     print("Failed to make plot of {} vs {}.  Here is the error context:".format(name1,name2))
                     filename=None
                     print(traceback.format_exc())
                 if filename:
                     filenames.append(filename)
+        filenames.append(self.make_corner_plot())
         return filenames
 
 
 class TestPlots(Plots):
     def run(self):
         dirname = self.source.sampler_option("save_dir")
         output_dir = self.options.get("outdir", "png")
@@ -728,75 +851,58 @@
                     #Then we got as far as making the figure before
                     #failing.  so remove it
                     pylab.close()
                 print(err)
         return filenames
 
 
-class WeightedPlots1D(object):
-    def smooth_likelihood(self, x, name):
+class WeightedPlots(object):
+    excluded_columns = ["like","old_like","post", "weight", "log_weight", "old_log_weight", "old_weight", "old_post", "prior"]
+
+    def smooth_likelihood_1d(self, x, name):
         #Interpolate using KDE
         n = self.options.get("n_kde", 100)
         weights = self.weight_col()
         #speed things up by removing zero-weighted samples
         if self.options.get("fix_edges"):
-            return self.smooth_likelihood_with_boundaries(x, name, weights)
+            return self.smooth_likelihood_with_boundaries_1d(x, name, weights)
 
         x_range = get_plot_range(x, weights)
 
         factor = self.options.get("factor_kde", 2.0)
         kde = KDE(x, factor=factor, weights=weights)
         x_axis, like = kde.grid_evaluate(n, x_range )
         return x_axis, like
 
-    def smooth_likelihood_with_boundaries(self, x, name, weights):
+    def smooth_likelihood_with_boundaries_1d(self, x, name, weights):
         # find the limits on this parameter
         factor = self.options.get("factor_kde", 2.0)
         xmin, xmax, fix = select_limits(x, self.source, name)
         xout, like = smooth_density_estimate_1d(x, xmin, xmax, weights=weights,
                             smoothing=factor, fix_boundary=fix)
         xmin0, xmax0 = get_plot_range(x, weights)
         cut = (xout >= xmin0) & (xout <= xmax0)
         return xout[cut], like[cut]
 
-
-class MultinestPlots1D(WeightedPlots1D, MultinestPostProcessorElement, MetropolisHastingsPlots1D):
-    excluded_columns = ["like","old_like","post", "weight", "log_weight", "old_log_weight", "old_weight", "old_post", "prior"]
-
-class PolychordPlots1D(MultinestPlots1D):
-    pass
-
-
-class WeightedMetropolisPlots1D(WeightedPlots1D, WeightedMCMCPostProcessorElement, MetropolisHastingsPlots1D):
-    excluded_columns = ["like","old_like","post", "weight", "log_weight", "old_log_weight", "old_weight", "old_post", "prior"]
-
-def get_plot_range(x, weights):
-    dx = std_weight(x, weights)*4
-    mu_x = mean_weight(x, weights)
-    return (max(x.min(), mu_x-dx), min(x.max(), mu_x+dx))
-
-
-class WeightedPlots2D(object):
-    excluded_columns = ["like","old_like","post", "weight", "log_weight", "old_log_weight", "old_weight", "old_post", "prior"]
-    def smooth_likelihood(self, x, y, xname, yname):
+    def smooth_likelihood_2d(self, x, y, xname, yname):
         weights = self.weight_col()
 
         if self.options.get("fix_edges"):
-            return self.smooth_likelihood_with_boundaries(x, y, weights, xname, yname)
+            return self.smooth_likelihood_with_boundaries_2d(x, y, weights, xname, yname)
 
         n = self.options.get("n_kde", 100)
         fill = self.options.get("fill", True)
         factor = self.options.get("factor_kde", 2.0)
         kde = KDE([x,y], factor=factor, weights=weights)
         x_range = get_plot_range(x, weights)
         y_range = get_plot_range(y, weights)
         (x_axis, y_axis), like = kde.grid_evaluate(n, [x_range, y_range])
         return x_axis, y_axis, like
 
-    def smooth_likelihood_with_boundaries(self, x, y, weights, xname, yname):
+    def smooth_likelihood_with_boundaries_2d(self, x, y, weights, xname, yname):
         factor = self.options.get("factor_kde", 2.0)
         xmin, xmax, fix_x = select_limits(x, self.source, xname)
         ymin, ymax, fix_y = select_limits(y, self.source, yname)
         xout, yout, like = smooth_density_estimate_2d(x, y, xmin, xmax, ymin, ymax, weights=weights,
                             smoothing=factor, fix_boundary=fix_x or fix_y)
         xmin0, xmax0 = get_plot_range(x, weights)
         ymin0, ymax0 = get_plot_range(y, weights)
@@ -826,14 +932,33 @@
         target1 = histogram.sum()*(1-contour1)
         target2 = histogram.sum()*(1-contour2)
 
         level1 = scipy.optimize.bisect(objective, like.min(), like.max(), args=(target1,))
         level2 = scipy.optimize.bisect(objective, like.min(), like.max(), args=(target2,))
         return level1, level2, like.sum()
 
+
+class MultinestPlots(WeightedPlots, MultinestPostProcessorElement, MetropolisHastingsPlots):
+    excluded_columns = ["like","old_like","post", "weight", "log_weight", "old_log_weight", "old_weight", "old_post", "prior"]
+
+class PolychordPlots(MultinestPlots):
+    pass
+
+def get_plot_range(x, weights):
+    dx = std_weight(x, weights)*4
+    mu_x = mean_weight(x, weights)
+    return (max(x.min(), mu_x-dx), min(x.max(), mu_x+dx))
+
+
+class WeightedMetropolisPlots(WeightedPlots, WeightedMCMCPostProcessorElement, MetropolisHastingsPlots):
+    excluded_columns = ["like","old_like","post", "weight", "log_weight", "old_log_weight", "old_weight", "old_post", "prior"]
+
+
+
+
 class TracePlots(Plots, MCMCPostProcessorElement):
     excluded_columns = []
     def run(self):
         return [self.plot_1d(name) for name in self.source.colnames if not name in self.excluded_columns]
 
     def plot_truth_1d(self, name):
         val = self.get_truth_value(name)
@@ -852,41 +977,14 @@
         pylab.ylabel(self.latex(name))
         if not hasattr(fig, 'cosmosis_done_truth'):
             self.plot_truth_1d(name)
             fig.cosmosis_done_truth = True
         return filename
 
 
-class WeightedMetropolisPlots2D(WeightedPlots2D, WeightedMCMCPostProcessorElement, MetropolisHastingsPlots2D):
-    excluded_columns = ["like","old_like","post", "weight", "log_weight", "old_log_weight", "old_weight", "old_post", "prior"]
-    pass
-
-class MultinestPlots2D(WeightedPlots2D, MultinestPostProcessorElement, MetropolisHastingsPlots2D):
-    excluded_columns = ["like","old_like","post", "weight", "log_weight", "old_log_weight", "old_weight", "old_post", "prior"]
-    pass
-
-class PolychordPlots2D(MultinestPlots2D):
-    pass
-
-class TrianglePlot(MetropolisHastingsPlots):
-    def run(self):
-        try:
-            import triangle
-        except ImportError:
-            print("Triangle library not available - no corner plot for you")
-            print("Maybe try pip install triangle")
-            return []
-        names = [name for name in self.source.colnames if not name in self.excluded_columns]
-        labels = [self.latex(name) for name in names]
-        chains = np.transpose([self.reduced_col(name) for name in names])
-        filename = self.filename("triangle")
-        figure = triangle.corner(chains, labels=labels, plot_datapoints=False)
-        self.set_output("triangle", PostprocessPlot("triangle",filename,figure))
-
-        return [filename]
 
 class ColorScatterPlotBase(Plots):
     scatter_filename='scatter'
     x_column = None
     y_column = None
     color_column = None
 
@@ -1089,15 +1187,17 @@
         pylab.gca().add_patch(ellip)
         return ellip
 
 class StarPlots(Plots):
     excluded_columns=["post","like", "prior"]
 
     def star_plot(self, i, name, log):
-        n = self.source.metadata[0]['nsample_dimension']
+        n = int(self.source.metadata[0]['nsample_dimension'])
+        shp = self.source.get_col(name).shape
+
         x = self.source.get_col(name)[i*n:(i+1)*n]
         y = self.source.get_col("post")[i*n:(i+1)*n]
         if log:
             figure,filename = self.figure(name+"_log")
         else:
             figure,filename = self.figure(name)
             y = np.exp(y-y.max())
@@ -1110,22 +1210,24 @@
             pylab.ylabel("Posterior")
         return filename
 
     def run(self):
         filenames = []
 
         i=0
-        for name in self.source.colnames:
-            if name.lower() in self.excluded_columns: continue
+        # We can only make plots of varied parameters in the star sampler,
+        # doing derived parameters doesn't really make sense
+        nv = self.source.metadata[0]['n_varied']
+        for i in range(nv):
+            name = self.source.colnames[i]
             # Do both log and non-log variants
             filename = self.star_plot(i,name, True)
             filenames.append(filename)
             filename = self.star_plot(i,name, False)
             filenames.append(filename)
-            i+=1
         return filenames
 
 
 
 
 class Tweaks(Loadable):
     filename="default_nonexistent_filename_ignore"
@@ -1152,7 +1254,69 @@
     if len(hex_color) != 7:
         raise Exception("Passed %s into color_variant(), needs to be in #87c95f format." % hex_color)
     rgb_hex = [hex_color[x:x+2] for x in [1, 3, 5]]
     new_rgb_int = [int(hex_value, 16) + brightness_offset for hex_value in rgb_hex]
     new_rgb_int = [min([255, max([0, i])]) for i in new_rgb_int] # make sure new values are between 0 and 255
     # hex() produces "0x88", we want just "88"
     return "#" + "".join([hex(i)[2:] for i in new_rgb_int])
+
+
+
+# For backwards-compatibility with any poor souls using these, we provide replacements for the old
+# separate 1D and 2D classes, which were unified to make it easier to do a corner plot.
+class WeightedMetropolisPlots1D(WeightedMetropolisPlots):
+    def run(self):
+        warnings.warn('WeightedMetropolisPlots1D and the other 1D and 2D plotters are deprecated', DeprecationWarning, stacklevel=2)
+        return self.run_1d()
+    def smooth_likelihood(self, x, name):
+        return self.smooth_likelihood_1d(x, name)
+
+class MetropolisHastingsPlots1D(MetropolisHastingsPlots):
+    def run(self):
+        warnings.warn('MetropolisPlots1D and the other 1D and 2D plotters are deprecated', DeprecationWarning, stacklevel=2)
+        return self.run_1d()
+    def smooth_likelihood(self, x, name):
+        return self.smooth_likelihood_1d(x, name)
+
+class PolychordPlots1D(PolychordPlots):
+    def run(self):
+        warnings.warn('PolychordPlots1D and the other 1D and 2D plotters are deprecated', DeprecationWarning, stacklevel=2)
+        return self.run_1d()
+    def smooth_likelihood(self, x, name):
+        return self.smooth_likelihood_1d(x, name)
+
+class MultinestPlots1D(MultinestPlots):
+    def run(self):
+        warnings.warn('MetropolisHastingsPlots1D and the other 1D and 2D plotters are deprecated', DeprecationWarning, stacklevel=2)
+        return self.run_1d()
+    def smooth_likelihood(self, x, name):
+        return self.smooth_likelihood_2d(x, name)
+
+# 2D versions of the above
+
+class MetropolisHastingsPlots2D(MetropolisHastingsPlots):
+    def run(self):
+        warnings.warn('MetropolisHastingsPlots2D and the other 1D and 2D plotters are deprecated', DeprecationWarning, stacklevel=2)
+        return self.run_2d()
+    def smooth_likelihood(self, x, y, xname, yname):
+        return self.smooth_likelihood_2d(x, y, xname, yname)
+
+class WeightedMetropolisPlots2D(WeightedMetropolisPlots):
+    def run(self):
+        warnings.warn('WeightedMetropolisPlots2D and the other 1D and 2D plotters are deprecated', DeprecationWarning, stacklevel=2)
+        return self.run_2d()
+    def smooth_likelihood(self, x, y, xname, yname):
+        return self.smooth_likelihood_2d(x, y, xname, yname)
+
+class MultinestPlots2D(MultinestPlots):
+    def run(self):
+        warnings.warn('MultinestPlots2D and the other 1D and 2D plotters are deprecated', DeprecationWarning, stacklevel=2)
+        return self.run_2d()
+    def smooth_likelihood(self, x, y, xname, yname):
+        return self.smooth_likelihood_2d(x, y, xname, yname)
+
+class PolychordPlots2D(PolychordPlots):
+    def run(self):
+        warnings.warn('Polychord2D and the other 1D and 2D plotters are deprecated', DeprecationWarning, stacklevel=2)
+        return self.run_2d()
+    def smooth_likelihood(self, x, y, xname, yname):
+        return self.smooth_likelihood_2d(x, y, xname, yname)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cosmosis-2.4.1/cosmosis/postprocessing/postprocess.py` & `cosmosis-2.5/cosmosis/postprocessing/postprocess.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,16 +57,15 @@
 			P.multiplicative_blind_column(c,f)
 
 
 
 
 class MetropolisHastingsProcessor(PostProcessor):
 	elements=[
-		plots.MetropolisHastingsPlots1D,
-		plots.MetropolisHastingsPlots2D,
+		plots.MetropolisHastingsPlots,
 		plots.TracePlots,
 		statistics.MetropolisHastingsStatistics,
 		statistics.MetropolisHastingsCovariance,
 		statistics.Citations,
 	]
 	def reduced_col(self, name, stacked=True):
 		cols = self.get_col(name, stacked=False)
@@ -140,29 +139,27 @@
 class PymcProcessor(MetropolisHastingsProcessor):
 	sampler="pymc"
 	pass
 
 class MetropolisProcessor(MetropolisHastingsProcessor):
 	sampler="metropolis"
 	elements=[
-		plots.MetropolisHastingsPlots1D,
-		plots.MetropolisHastingsPlots2D,
+		plots.MetropolisHastingsPlots,
 		statistics.MetropolisHastingsStatistics,
 		statistics.MetropolisHastingsCovariance,
 		statistics.DunkleyTest,
 		statistics.GelmanRubinStatistic,
 		statistics.Citations,
 		]
 
 
 class WeightedMetropolisProcessor(MetropolisHastingsProcessor):
 	sampler="weighted_metropolis"
 	elements=[
-		plots.WeightedMetropolisPlots1D,
-		plots.WeightedMetropolisPlots2D,
+		plots.WeightedMetropolisPlots,
 		plots.TracePlots,
 		statistics.WeightedMetropolisStatistics,
 		statistics.WeightedMetropolisHastingsCovariance,
 		#statistics.DunkleyTest,
 		statistics.Citations,		
 		]
 
@@ -205,16 +202,15 @@
 		u = np.random.uniform(size=w.size)
 		return u<w
 
 
 class ImportanceProcessor(WeightedMetropolisProcessor):
 	sampler="importance"
 	elements=[
-		plots.WeightedMetropolisPlots1D,
-		plots.WeightedMetropolisPlots2D,
+		plots.WeightedMetropolisPlots,
 		statistics.WeightedMetropolisStatistics,
 		# statistics.DunkleyTest,
 		statistics.Citations,		
 		]
 
 class GridProcessor(PostProcessor):
 	elements=[
@@ -239,16 +235,15 @@
 			for key,val in ini.items("test"):
 				self.sampler_options[key]=str(val)
 
 
 
 class MultinestProcessor(WeightedMetropolisProcessor):
 	elements = [
-		plots.MultinestPlots1D, 
-		plots.MultinestPlots2D,
+		plots.MultinestPlots,
 		plots.TracePlots,
 		statistics.MultinestStatistics,
 		statistics.MultinestCovariance,
 		statistics.Citations,
 		]
 	sampler="multinest"
 	def reduced_col(self, name, stacked=True):
@@ -280,27 +275,25 @@
 		w = self.weight_col()
 		w = w / w.max()
 		u = np.random.uniform(size=w.size)
 		return u<w
 
 class PolyChordProcessor(MultinestProcessor):
     elements = [
-            plots.PolychordPlots1D, 
-            plots.PolychordPlots2D,
+            plots.PolychordPlots,
             plots.TracePlots,
             statistics.PolychordStatistics,
             statistics.PolychordCovariance,
             statistics.Citations,
             ]
     sampler="polychord"
 
 class DynestyProcessor(MultinestProcessor):
 	elements = [
-			plots.PolychordPlots1D, 
-			plots.PolychordPlots2D,
+			plots.PolychordPlots,
 			plots.TracePlots,
 			statistics.PolychordStatistics,
 			statistics.PolychordCovariance,
 			statistics.Citations,
 			]
 	sampler="dynesty"
 
@@ -319,16 +312,15 @@
 class NautilusProcess(DynestyProcessor):
 	sampler = "nautilus"
 
 
 class PMCPostProcessor(WeightedMetropolisProcessor):
 	sampler="pmc"
 	elements = [
-		plots.WeightedMetropolisPlots1D,
-		plots.WeightedMetropolisPlots2D,
+		plots.WeightedMetropolisPlots,
 		statistics.WeightedMetropolisStatistics,
 		#statistics.WeightedMetropolisHastingsCovariance,
 		#statistics.DunkleyTest,
 		statistics.Citations,		
 	]
 	def reduced_col(self, name, stacked=True):
 		#we only use the last n samples from a multinest output
```

### Comparing `cosmosis-2.4.1/cosmosis/postprocessing/postprocess_base.py` & `cosmosis-2.5/cosmosis/postprocessing/postprocess_base.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/postprocessing/reruns.py` & `cosmosis-2.5/cosmosis/postprocessing/reruns.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/postprocessing/statistics.py` & `cosmosis-2.5/cosmosis/postprocessing/statistics.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/postprocessing/utils.py` & `cosmosis-2.5/cosmosis/postprocessing/utils.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/runtime/analytics.py` & `cosmosis-2.5/cosmosis/runtime/analytics.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/runtime/attribution.py` & `cosmosis-2.5/cosmosis/runtime/attribution.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/runtime/config.py` & `cosmosis-2.5/cosmosis/runtime/config.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/runtime/declare.py` & `cosmosis-2.5/cosmosis/runtime/declare.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/runtime/julia_modules/julia.py` & `cosmosis-2.5/cosmosis/runtime/julia_modules/julia.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/runtime/memmon.py` & `cosmosis-2.5/cosmosis/runtime/memmon.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/runtime/module.py` & `cosmosis-2.5/cosmosis/runtime/module.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/runtime/mpi_pool.py` & `cosmosis-2.5/cosmosis/runtime/mpi_pool.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/runtime/parameter.py` & `cosmosis-2.5/cosmosis/runtime/parameter.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/runtime/pipeline.py` & `cosmosis-2.5/cosmosis/runtime/pipeline.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/runtime/prior.py` & `cosmosis-2.5/cosmosis/runtime/prior.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/runtime/process_pool.py` & `cosmosis-2.5/cosmosis/runtime/process_pool.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/__init__.py` & `cosmosis-2.5/cosmosis/samplers/__init__.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/abc/abc_sampler.py` & `cosmosis-2.5/cosmosis/samplers/abc/abc_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/abc/abc_sampler_mpi.py` & `cosmosis-2.5/cosmosis/samplers/abc/abc_sampler_mpi.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/apriori/apriori_sampler.py` & `cosmosis-2.5/cosmosis/samplers/apriori/apriori_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/dynesty/dynesty_sampler.py` & `cosmosis-2.5/cosmosis/samplers/dynesty/dynesty_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/emcee/emcee_sampler.py` & `cosmosis-2.5/cosmosis/samplers/emcee/emcee_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/fisher/fisher.py` & `cosmosis-2.5/cosmosis/samplers/fisher/fisher.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/fisher/fisher_sampler.py` & `cosmosis-2.5/cosmosis/samplers/fisher/fisher_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/grid/grid_sampler.py` & `cosmosis-2.5/cosmosis/samplers/grid/grid_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/gridmax/gridmax_sampler.py` & `cosmosis-2.5/cosmosis/samplers/gridmax/gridmax_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/hints.py` & `cosmosis-2.5/cosmosis/samplers/hints.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/importance/importance_sampler.py` & `cosmosis-2.5/cosmosis/samplers/importance/importance_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/kombine/kombine_sampler.py` & `cosmosis-2.5/cosmosis/samplers/kombine/kombine_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/list/list_sampler.py` & `cosmosis-2.5/cosmosis/samplers/list/list_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/maxlike/maxlike_sampler.py` & `cosmosis-2.5/cosmosis/samplers/maxlike/maxlike_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/metropolis/metropolis.py` & `cosmosis-2.5/cosmosis/samplers/metropolis/metropolis.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/metropolis/metropolis_sampler.py` & `cosmosis-2.5/cosmosis/samplers/metropolis/metropolis_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/metropolis/proposal/cobaya_proposal.py` & `cosmosis-2.5/cosmosis/samplers/metropolis/proposal/cobaya_proposal.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/metropolis/proposal/standard.py` & `cosmosis-2.5/cosmosis/samplers/metropolis/proposal/standard.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/minuit/Makefile` & `cosmosis-2.5/cosmosis/samplers/minuit/Makefile`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/minuit/minuit_sampler.py` & `cosmosis-2.5/cosmosis/samplers/minuit/minuit_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/minuit/minuit_wrapper.cpp` & `cosmosis-2.5/cosmosis/samplers/minuit/minuit_wrapper.cpp`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/multinest/multinest_sampler.py` & `cosmosis-2.5/cosmosis/samplers/multinest/multinest_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/multinest/multinest_src/LICENCE` & `cosmosis-2.5/cosmosis/samplers/multinest/multinest_src/LICENCE`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/multinest/multinest_src/Makefile` & `cosmosis-2.5/cosmosis/samplers/multinest/multinest_src/Makefile`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/multinest/multinest_src/README` & `cosmosis-2.5/cosmosis/samplers/multinest/multinest_src/README`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/multinest/multinest_src/cwrapper.f90` & `cosmosis-2.5/cosmosis/samplers/multinest/multinest_src/cwrapper.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/multinest/multinest_src/kmeans_clstr.f90` & `cosmosis-2.5/cosmosis/samplers/multinest/multinest_src/kmeans_clstr.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/multinest/multinest_src/nested.f90` & `cosmosis-2.5/cosmosis/samplers/multinest/multinest_src/nested.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/multinest/multinest_src/posterior.f90` & `cosmosis-2.5/cosmosis/samplers/multinest/multinest_src/posterior.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/multinest/multinest_src/priors.f90` & `cosmosis-2.5/cosmosis/samplers/multinest/multinest_src/priors.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/multinest/multinest_src/utils.f90` & `cosmosis-2.5/cosmosis/samplers/multinest/multinest_src/utils.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/multinest/multinest_src/utils1.f90` & `cosmosis-2.5/cosmosis/samplers/multinest/multinest_src/utils1.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/multinest/multinest_src/xmeans_clstr.f90` & `cosmosis-2.5/cosmosis/samplers/multinest/multinest_src/xmeans_clstr.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/nautilus/nautilus_sampler.py` & `cosmosis-2.5/cosmosis/samplers/nautilus/nautilus_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/pmaxlike/pmaxlike_sampler.py` & `cosmosis-2.5/cosmosis/samplers/pmaxlike/pmaxlike_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/pmc/pmc.py` & `cosmosis-2.5/cosmosis/samplers/pmc/pmc.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/pmc/pmc_sampler.py` & `cosmosis-2.5/cosmosis/samplers/pmc/pmc_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/poco/poco_sampler.py` & `cosmosis-2.5/cosmosis/samplers/poco/poco_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_sampler.py` & `cosmosis-2.5/cosmosis/samplers/polychord/polychord_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/LICENCE` & `cosmosis-2.5/cosmosis/samplers/polychord/polychord_src/LICENCE`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/Makefile` & `cosmosis-2.5/cosmosis/samplers/polychord/polychord_src/Makefile`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/README` & `cosmosis-2.5/cosmosis/samplers/polychord/polychord_src/README`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/abort.F90` & `cosmosis-2.5/cosmosis/samplers/polychord/polychord_src/abort.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/array_utils.f90` & `cosmosis-2.5/cosmosis/samplers/polychord/polychord_src/array_utils.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/c_interface.cpp` & `cosmosis-2.5/cosmosis/samplers/polychord/polychord_src/c_interface.cpp`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/calculate.f90` & `cosmosis-2.5/cosmosis/samplers/polychord/polychord_src/calculate.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/chordal_sampling.f90` & `cosmosis-2.5/cosmosis/samplers/polychord/polychord_src/chordal_sampling.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/clustering.f90` & `cosmosis-2.5/cosmosis/samplers/polychord/polychord_src/clustering.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/feedback.f90` & `cosmosis-2.5/cosmosis/samplers/polychord/polychord_src/feedback.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/generate.F90` & `cosmosis-2.5/cosmosis/samplers/polychord/polychord_src/generate.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/ini.f90` & `cosmosis-2.5/cosmosis/samplers/polychord/polychord_src/ini.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/interfaces.F90` & `cosmosis-2.5/cosmosis/samplers/polychord/polychord_src/interfaces.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/interfaces.h` & `cosmosis-2.5/cosmosis/samplers/polychord/polychord_src/interfaces.h`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/interfaces.hpp` & `cosmosis-2.5/cosmosis/samplers/polychord/polychord_src/interfaces.hpp`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/mpi_utils.F90` & `cosmosis-2.5/cosmosis/samplers/polychord/polychord_src/mpi_utils.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/nested_sampling.F90` & `cosmosis-2.5/cosmosis/samplers/polychord/polychord_src/nested_sampling.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/params.f90` & `cosmosis-2.5/cosmosis/samplers/polychord/polychord_src/params.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/priors.f90` & `cosmosis-2.5/cosmosis/samplers/polychord/polychord_src/priors.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/random_utils.F90` & `cosmosis-2.5/cosmosis/samplers/polychord/polychord_src/random_utils.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/read_write.f90` & `cosmosis-2.5/cosmosis/samplers/polychord/polychord_src/read_write.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/run_time_info.f90` & `cosmosis-2.5/cosmosis/samplers/polychord/polychord_src/run_time_info.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/settings.f90` & `cosmosis-2.5/cosmosis/samplers/polychord/polychord_src/settings.f90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/polychord/polychord_src/utils.F90` & `cosmosis-2.5/cosmosis/samplers/polychord/polychord_src/utils.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/pymc/pymc_sampler.py` & `cosmosis-2.5/cosmosis/samplers/pymc/pymc_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/sampler.py` & `cosmosis-2.5/cosmosis/samplers/sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/snake/snake.py` & `cosmosis-2.5/cosmosis/samplers/snake/snake.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/snake/snake_sampler.py` & `cosmosis-2.5/cosmosis/samplers/snake/snake_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/star/star_sampler.py` & `cosmosis-2.5/cosmosis/samplers/star/star_sampler.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     understands_fast_subspaces = True
 
     def config(self):
         global star_sampler
         star_sampler = self
 
         self.converged = False
-        self.nsample = self.read_ini("nsample_dimension", int, 1)
+        self.nsample = self.read_ini("nsample_dimension", int, 3)
         self.save_name = self.read_ini("save", str, "")
         self.nstep = self.read_ini("nstep", int, -1)
         self.allow_large = self.read_ini("allow_large", bool, False)
         self.sample_points = None
         self.ndone = 0
 
     def setup_sampling(self):
```

### Comparing `cosmosis-2.4.1/cosmosis/samplers/test/test_sampler.py` & `cosmosis-2.5/cosmosis/samplers/test/test_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/samplers/zeus/zeus_sampler.py` & `cosmosis-2.5/cosmosis/samplers/zeus/zeus_sampler.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/test/libtest/Makefile` & `cosmosis-2.5/cosmosis/test/libtest/Makefile`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/test/libtest/c_datablock_complex_array_test.c` & `cosmosis-2.5/cosmosis/test/libtest/c_datablock_complex_array_test.c`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/test/libtest/c_datablock_double_array_test.c` & `cosmosis-2.5/cosmosis/test/libtest/c_datablock_double_array_test.c`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/test/libtest/c_datablock_int_array_test.c` & `cosmosis-2.5/cosmosis/test/libtest/c_datablock_int_array_test.c`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/test/libtest/c_datablock_multidim_complex_array_test.c` & `cosmosis-2.5/cosmosis/test/libtest/c_datablock_multidim_complex_array_test.c`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/test/libtest/c_datablock_multidim_double_array_test.c` & `cosmosis-2.5/cosmosis/test/libtest/c_datablock_multidim_double_array_test.c`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/test/libtest/c_datablock_multidim_int_array_test.c` & `cosmosis-2.5/cosmosis/test/libtest/c_datablock_multidim_int_array_test.c`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/test/libtest/c_datablock_test.c` & `cosmosis-2.5/cosmosis/test/libtest/c_datablock_test.c`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/test/libtest/cosmosis_test.F90` & `cosmosis-2.5/cosmosis/test/libtest/cosmosis_test.F90`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/test/libtest/datablock_test.cc` & `cosmosis-2.5/cosmosis/test/libtest/datablock_test.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/test/libtest/entry_test.cc` & `cosmosis-2.5/cosmosis/test/libtest/entry_test.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/test/libtest/ndarray_test.cc` & `cosmosis-2.5/cosmosis/test/libtest/ndarray_test.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/test/libtest/section_test.cc` & `cosmosis-2.5/cosmosis/test/libtest/section_test.cc`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/test/libtest/test_c_datablock_scalars.h` & `cosmosis-2.5/cosmosis/test/libtest/test_c_datablock_scalars.h`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/test/libtest/test_c_datablock_scalars.template` & `cosmosis-2.5/cosmosis/test/libtest/test_c_datablock_scalars.template`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/test/test_block.py` & `cosmosis-2.5/cosmosis/test/test_block.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/test/test_chaining.py` & `cosmosis-2.5/cosmosis/test/test_chaining.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/test/test_gaussian.py` & `cosmosis-2.5/cosmosis/test/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/test/test_lib.py` & `cosmosis-2.5/cosmosis/test/test_lib.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/test/test_module2.py` & `cosmosis-2.5/cosmosis/test/test_module2.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/test/test_modules.py` & `cosmosis-2.5/cosmosis/test/test_modules.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/test/test_parameters.py` & `cosmosis-2.5/cosmosis/test/test_parameters.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/test/test_pipeline.py` & `cosmosis-2.5/cosmosis/test/test_pipeline.py`

 * *Files 9% similar despite different names*

```diff
@@ -202,12 +202,52 @@
         # shopuld work this time
         try:
             os.environ["COSMOSIS_NO_SUBPROCESS"] = "1"
             status = run_cosmosis(args, ini=ini)
         finally:
             del os.environ["COSMOSIS_NO_SUBPROCESS"]
 
+def test_prior_override():
+    with tempfile.TemporaryDirectory() as dirname:
+        values_file = f"{dirname}/values.ini"
+        output_file = f"{dirname}/output.txt"
+        with open(values_file, "w") as values:
+            values.write(
+                "[parameters]\n"
+                "p1=-3.0  0.0  3.0\n"
+                "p2=-3.0  0.0  3.0\n")
+
+        params = {
+            ('runtime', 'root'): os.path.split(os.path.abspath(__file__))[0],
+            ('runtime', 'sampler'):  "apriori",
+            ('apriori', 'nsample'):  "1000",
+            ("pipeline", "debug"): "F",
+            ("pipeline", "quiet"): "F",
+            ("pipeline", "modules"): "test1",
+            ("pipeline", "values"): values_file,
+            ("test1", "file"): "test_module.py",
+            ("output", "filename"): output_file,
+        }
+
+        args = parser.parse_args(["not_a_real_file"])
+        ini = Inifile(None, override=params)
+
+        priors_vals = {
+            ('parameters', 'p1'): 'uniform -1.0    1.0'
+        }
+
+        priors = Inifile(None, override=priors_vals)
+
+        status = run_cosmosis(args, ini=ini, priors=priors)
+        chain = np.loadtxt(output_file).T
+        p1 = chain[0]
+        p2 = chain[1]
+        print(p1.min(), p1.max())
+        assert p1.max() < 1.0
+        assert p1.min() > -1.0
+
+
 
 
 
 if __name__ == '__main__':
     test_script_skip()
```

### Comparing `cosmosis-2.4.1/cosmosis/test/test_polychord.py` & `cosmosis-2.5/cosmosis/test/test_polychord.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/test/test_samplers.py` & `cosmosis-2.5/cosmosis/test/test_samplers.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import os
 import sys
 import pytest
 import numpy as np
 
 minuit_compiled = os.path.exists(cosmosis.samplers.minuit.minuit_sampler.libname)
 
-def run(name, check_prior, check_extra=True, can_postprocess=True, do_truth=False, no_extra=False, **options):
+def run(name, check_prior, check_extra=True, can_postprocess=True, do_truth=False, no_extra=False, pp_extra=True, pp_2d=True, **options):
 
     sampler_class = Sampler.registry[name]
 
     values = tempfile.NamedTemporaryFile('w')
     values.write(
         "[parameters]\n"
         "p1=-3.0  0.0  3.0\n"
@@ -68,15 +68,30 @@
 
     if can_postprocess:
         pp_class = postprocessor_for_sampler(name)
         print(pp_class)
         with tempfile.TemporaryDirectory() as dirname:
             truth_file = values.name if do_truth else None
             pp = pp_class(output, "Chain", 0, outdir=dirname, prefix=name, truth=truth_file)
-            pp.run()
+            pp_files = pp.run()
+            pp.finalize()
+            for p in pp_files:
+                print(p)
+            postprocess_files = ['parameters--p1', 'parameters--p2']
+            if pp_2d:
+                postprocess_files.append('2D_parameters--p2_parameters--p1')
+            if check_extra and pp_extra and not no_extra:
+                postprocess_files.append('parameters--p3')
+                if pp_2d:
+                    postprocess_files += ['2D_parameters--p3_parameters--p2', '2D_parameters--p3_parameters--p1']
+            for p in postprocess_files:
+                filename = f"{dirname}{os.path.sep}{name}_{p}.png"
+                print("WANT ", filename)
+                assert filename in pp_files
+                assert os.path.exists(filename)
 
 
     return output
 
 
 def test_apriori():
     run('apriori', True, can_postprocess=False, nsample=100)
@@ -91,15 +106,15 @@
 def test_truth():
     run('emcee', True, walkers=8, samples=100, do_truth=True)
 
 def test_fisher():
     run('fisher', False, check_extra=False)
 
 def test_grid():
-    run('grid', True, nsample_dimension=10)
+    run('grid', True, pp_extra=False, nsample_dimension=10)
 
 def test_gridmax():
     run('gridmax', True, can_postprocess=False, max_iterations=1000)
 
 # def test_kombine():
 #     run('kombine')
 
@@ -135,25 +150,24 @@
     run('zeus', True, maxiter=50_000, walkers=10, samples=100, nsteps=50)
 
 def test_polychord():
     with tempfile.TemporaryDirectory() as base_dir:
         run('polychord', True, live_points=20, feedback=0, base_dir=base_dir, polychord_outfile_root='pc')
 
 def test_snake():
-        run('snake', True)
+        run('snake', True, pp_extra=False)
 
 def test_nautilus():
     run('nautilus', True)
-    run('nautilus', True, no_extra=True)
-    run('nautilus', True, no_extra=True, n_live=500, enlarge_per_dim=1.05,
+    run('nautilus', True, n_live=500, enlarge_per_dim=1.05,
         split_threshold=95., n_networks=3, n_batch=50, verbose=True, f_live=0.02, n_shell=100)
 
 
 def test_star():
-        run('star', False)
+        run('star', False, pp_extra=False, pp_2d=False)
 
 def test_test():
     run('test', False, can_postprocess=False)
 
 @pytest.mark.skipif(sys.version_info < (3,7), reason="pocomc requires python3.6+")
 def test_poco():
     try:
```

### Comparing `cosmosis-2.4.1/cosmosis/test/test_text_output.py` & `cosmosis-2.5/cosmosis/test/test_text_output.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/test/test_utils.py` & `cosmosis-2.5/cosmosis/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis/utils.py` & `cosmosis-2.5/cosmosis/utils.py`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/cosmosis.egg-info/SOURCES.txt` & `cosmosis-2.5/cosmosis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cosmosis-2.4.1/setup.py` & `cosmosis-2.5/setup.py`

 * *Files identical despite different names*

