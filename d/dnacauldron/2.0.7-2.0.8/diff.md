# Comparing `tmp/dnacauldron-2.0.7.tar.gz` & `tmp/dnacauldron-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dnacauldron-2.0.7.tar", last modified: Fri Jun 10 21:45:20 2022, max compression
+gzip compressed data, was "dnacauldron-2.0.8.tar", last modified: Thu May 25 21:39:39 2023, max compression
```

## Comparing `dnacauldron-2.0.7.tar` & `dnacauldron-2.0.8.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-06-10 21:45:20.384662 dnacauldron-2.0.7/
--rw-rw-r--   0 peter     (1000) peter     (1000)     1081 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/LICENCE.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)      142 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/MANIFEST.in
--rw-rw-r--   0 peter     (1000) peter     (1000)     1624 2022-06-10 21:45:20.384662 dnacauldron-2.0.7/PKG-INFO
--rw-rw-r--   0 peter     (1000) peter     (1000)     7465 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/README.rst
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-06-10 21:45:20.368662 dnacauldron-2.0.7/dnacauldron/
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-06-10 21:45:20.368662 dnacauldron-2.0.7/dnacauldron/Assembly/
--rw-rw-r--   0 peter     (1000) peter     (1000)     4949 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/Assembly/Assembly.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1063 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/Assembly/AssemblyFlaw.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-06-10 21:45:20.368662 dnacauldron-2.0.7/dnacauldron/Assembly/AssemblyReportWriter/
--rw-rw-r--   0 peter     (1000) peter     (1000)     1148 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/Assembly/AssemblyReportWriter/AssemblyPlotTranslator.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1843 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/Assembly/AssemblyReportWriter/AssemblyReportPlotsMixin.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     8123 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/Assembly/AssemblyReportWriter/AssemblyReportWriter.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      175 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/Assembly/AssemblyReportWriter/__init__.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2324 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/Assembly/AssemblyReportWriter/plot_cuts.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     4992 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/Assembly/AssemblySimulation.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      922 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/Assembly/__init__.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-06-10 21:45:20.368662 dnacauldron-2.0.7/dnacauldron/Assembly/builtin_assembly_classes/
--rw-rw-r--   0 peter     (1000) peter     (1000)     6080 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/Assembly/builtin_assembly_classes/BASICAssembly.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     6816 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/Assembly/builtin_assembly_classes/BioBrickStandardAssembly.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     7816 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/Assembly/builtin_assembly_classes/GibsonAssembly.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     8788 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/Assembly/builtin_assembly_classes/LigaseCyclingReactionAssembly.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3283 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/Assembly/builtin_assembly_classes/OligoPairAnnealing.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     8859 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/Assembly/builtin_assembly_classes/Type2sRestrictionAssembly.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      521 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/Assembly/builtin_assembly_classes/__init__.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-06-10 21:45:20.372662 dnacauldron-2.0.7/dnacauldron/AssemblyMix/
--rw-rw-r--   0 peter     (1000) peter     (1000)      984 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/AssemblyMix/AssemblyMix.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      254 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/AssemblyMix/AssemblyMixError.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2372 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/AssemblyMix/HomologousAssemblyMix.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     4859 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/AssemblyMix/LigaseCyclingReactionMix.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3768 2022-06-10 21:42:51.000000 dnacauldron-2.0.7/dnacauldron/AssemblyMix/RestrictionLigationMix.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-06-10 21:45:20.372662 dnacauldron-2.0.7/dnacauldron/AssemblyMix/StickyEndAssemblyMix/
--rw-rw-r--   0 peter     (1000) peter     (1000)     5787 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/AssemblyMix/StickyEndAssemblyMix/PlotsMixin.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3423 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/AssemblyMix/StickyEndAssemblyMix/SlotsMixin.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2348 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/AssemblyMix/StickyEndAssemblyMix/StickyEndAssemblyMix.py
--rw-rw-r--   0 peter     (1000) peter     (1000)       54 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/AssemblyMix/StickyEndAssemblyMix/__init__.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      509 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/AssemblyMix/__init__.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-06-10 21:45:20.372662 dnacauldron-2.0.7/dnacauldron/AssemblyMix/mixins/
--rw-rw-r--   0 peter     (1000) peter     (1000)     3607 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/AssemblyMix/mixins/ConnectorsMixin.py
--rw-rw-r--   0 peter     (1000) peter     (1000)    11176 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/AssemblyMix/mixins/ConstructsMixin.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1733 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/AssemblyMix/mixins/FragmentsMixin.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3938 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/AssemblyMix/mixins/GraphsMixin.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2150 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/AssemblyMix/mixins/PlotsMixin.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      204 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/AssemblyMix/mixins/__init__.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-06-10 21:45:20.372662 dnacauldron-2.0.7/dnacauldron/AssemblyPlan/
--rw-rw-r--   0 peter     (1000) peter     (1000)    10277 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/AssemblyPlan/AssemblyPlan.py
--rw-rw-r--   0 peter     (1000) peter     (1000)    12568 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/AssemblyPlan/AssemblyPlanSimulation.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      168 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/AssemblyPlan/__init__.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     4111 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/AssemblyPlan/plot_leveled_graph.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3236 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/Filter.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-06-10 21:45:20.372662 dnacauldron-2.0.7/dnacauldron/Fragment/
--rw-rw-r--   0 peter     (1000) peter     (1000)     2146 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/Fragment/Fragment.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     5698 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/Fragment/FragmentChain.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-06-10 21:45:20.372662 dnacauldron-2.0.7/dnacauldron/Fragment/HomologousFragment/
--rw-rw-r--   0 peter     (1000) peter     (1000)     6008 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/Fragment/HomologousFragment/HomologousFragment.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3418 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/Fragment/HomologousFragment/HomologyChecker.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      148 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/Fragment/HomologousFragment/__init__.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-06-10 21:45:20.376662 dnacauldron-2.0.7/dnacauldron/Fragment/StickyEndFragment/
--rw-rw-r--   0 peter     (1000) peter     (1000)     1669 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/Fragment/StickyEndFragment/StickyEnd.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     6665 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/Fragment/StickyEndFragment/StickyEndFragment.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     9453 2022-06-10 21:42:51.000000 dnacauldron-2.0.7/dnacauldron/Fragment/StickyEndFragment/StickyEndSeq.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      316 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/Fragment/StickyEndFragment/__init__.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      314 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/Fragment/__init__.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     7104 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/SequenceRepository.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1233 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/__init__.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-06-10 21:45:20.376662 dnacauldron-2.0.7/dnacauldron/biotools/
--rw-rw-r--   0 peter     (1000) peter     (1000)      342 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/biotools/__init__.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      921 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/biotools/autoselect_enzyme.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     4516 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/biotools/record_operations.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     8602 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/biotools/sequence_io.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-06-10 21:45:20.376662 dnacauldron-2.0.7/dnacauldron/report_assets/
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-06-10 21:45:20.376662 dnacauldron-2.0.7/dnacauldron/report_assets/imgs/
--rw-rw-r--   0 peter     (1000) peter     (1000)    19541 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/report_assets/imgs/logo.png
--rw-rw-r--   0 peter     (1000) peter     (1000)      303 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/report_assets/report_style.css
--rw-rw-r--   0 peter     (1000) peter     (1000)      973 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/report_assets/simulation_report.pug
--rw-rw-r--   0 peter     (1000) peter     (1000)     1989 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/reports.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      562 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/tools.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-06-10 21:45:20.380662 dnacauldron-2.0.7/dnacauldron/utils/
--rw-rw-r--   0 peter     (1000) peter     (1000)      512 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/utils/__init__.py
--rw-rw-r--   0 peter     (1000) peter     (1000)    11627 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/utils/insert_parts_on_backbones.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     4918 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/dnacauldron/utils/utils.py
--rw-rw-r--   0 peter     (1000) peter     (1000)       22 2022-06-10 21:45:00.000000 dnacauldron-2.0.7/dnacauldron/version.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-06-10 21:45:20.368662 dnacauldron-2.0.7/dnacauldron.egg-info/
--rw-rw-r--   0 peter     (1000) peter     (1000)     1624 2022-06-10 21:45:19.000000 dnacauldron-2.0.7/dnacauldron.egg-info/PKG-INFO
--rw-rw-r--   0 peter     (1000) peter     (1000)     3745 2022-06-10 21:45:20.000000 dnacauldron-2.0.7/dnacauldron.egg-info/SOURCES.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)        1 2022-06-10 21:45:19.000000 dnacauldron-2.0.7/dnacauldron.egg-info/dependency_links.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)      175 2022-06-10 21:45:20.000000 dnacauldron-2.0.7/dnacauldron.egg-info/requires.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)       12 2022-06-10 21:45:20.000000 dnacauldron-2.0.7/dnacauldron.egg-info/top_level.txt
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-06-10 21:45:20.364662 dnacauldron-2.0.7/examples/
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-06-10 21:45:20.380662 dnacauldron-2.0.7/examples/BASIC_assembly/
--rw-rw-r--   0 peter     (1000) peter     (1000)      330 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/examples/BASIC_assembly/BASIC_assembly.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-06-10 21:45:20.380662 dnacauldron-2.0.7/examples/autoselect_connectors/
--rw-rw-r--   0 peter     (1000) peter     (1000)      795 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/examples/autoselect_connectors/autoselect_connectors.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-06-10 21:45:20.380662 dnacauldron-2.0.7/examples/combinatorial_golden_gate/
--rw-rw-r--   0 peter     (1000) peter     (1000)      661 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/examples/combinatorial_golden_gate/combinatorial_golden_gate.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      640 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/examples/combinatorial_golden_gate/random_constructs_from_combinatorial_design.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-06-10 21:45:20.380662 dnacauldron-2.0.7/examples/gibson_assembly/
--rw-rw-r--   0 peter     (1000) peter     (1000)      634 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/examples/gibson_assembly/gibson_assembly.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-06-10 21:45:20.380662 dnacauldron-2.0.7/examples/hierarchical_biobrick/
--rw-rw-r--   0 peter     (1000) peter     (1000)      454 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/examples/hierarchical_biobrick/hierarchical_biobrick.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-06-10 21:45:20.380662 dnacauldron-2.0.7/examples/hierarchical_golden_gate/
--rw-rw-r--   0 peter     (1000) peter     (1000)      523 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/examples/hierarchical_golden_gate/hierarchical_golden_gate.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-06-10 21:45:20.380662 dnacauldron-2.0.7/examples/lcr_assembly/
--rw-rw-r--   0 peter     (1000) peter     (1000)      329 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/examples/lcr_assembly/README.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)      384 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/examples/lcr_assembly/example_with_assembly_plan.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-06-10 21:45:20.380662 dnacauldron-2.0.7/examples/multi_assemby_plan/
--rw-rw-r--   0 peter     (1000) peter     (1000)     1511 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/examples/multi_assemby_plan/multi_assembly.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     8512 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/ez_setup.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1275 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/pypi-readme.rst
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2022-06-10 21:45:20.384662 dnacauldron-2.0.7/scripts/
--rw-rw-r--   0 peter     (1000) peter     (1000)     2213 2021-11-25 11:15:52.000000 dnacauldron-2.0.7/scripts/dnacauldron
--rw-rw-r--   0 peter     (1000) peter     (1000)       38 2022-06-10 21:45:20.384662 dnacauldron-2.0.7/setup.cfg
--rw-rw-r--   0 peter     (1000) peter     (1000)     1056 2022-06-10 21:42:51.000000 dnacauldron-2.0.7/setup.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-05-25 21:39:39.698314 dnacauldron-2.0.8/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1081 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/LICENCE.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)      142 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/MANIFEST.in
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1624 2023-05-25 21:39:39.694314 dnacauldron-2.0.8/PKG-INFO
+-rw-rw-r--   0 peter     (1000) peter     (1000)     7501 2023-05-25 21:39:26.000000 dnacauldron-2.0.8/README.rst
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-05-25 21:39:39.686314 dnacauldron-2.0.8/dnacauldron/
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-05-25 21:39:39.690314 dnacauldron-2.0.8/dnacauldron/Assembly/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4949 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/Assembly/Assembly.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1063 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/Assembly/AssemblyFlaw.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-05-25 21:39:39.690314 dnacauldron-2.0.8/dnacauldron/Assembly/AssemblyReportWriter/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1148 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/Assembly/AssemblyReportWriter/AssemblyPlotTranslator.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1843 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/Assembly/AssemblyReportWriter/AssemblyReportPlotsMixin.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     8123 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/Assembly/AssemblyReportWriter/AssemblyReportWriter.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      175 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/Assembly/AssemblyReportWriter/__init__.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2324 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/Assembly/AssemblyReportWriter/plot_cuts.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4992 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/Assembly/AssemblySimulation.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      922 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/Assembly/__init__.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-05-25 21:39:39.690314 dnacauldron-2.0.8/dnacauldron/Assembly/builtin_assembly_classes/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6114 2023-05-25 21:39:26.000000 dnacauldron-2.0.8/dnacauldron/Assembly/builtin_assembly_classes/BASICAssembly.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6816 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/Assembly/builtin_assembly_classes/BioBrickStandardAssembly.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     7816 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/Assembly/builtin_assembly_classes/GibsonAssembly.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     8788 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/Assembly/builtin_assembly_classes/LigaseCyclingReactionAssembly.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3311 2023-05-25 21:39:26.000000 dnacauldron-2.0.8/dnacauldron/Assembly/builtin_assembly_classes/OligoPairAnnealing.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     8859 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/Assembly/builtin_assembly_classes/Type2sRestrictionAssembly.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      521 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/Assembly/builtin_assembly_classes/__init__.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-05-25 21:39:39.690314 dnacauldron-2.0.8/dnacauldron/AssemblyMix/
+-rw-rw-r--   0 peter     (1000) peter     (1000)      984 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/AssemblyMix/AssemblyMix.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      254 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/AssemblyMix/AssemblyMixError.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2372 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/AssemblyMix/HomologousAssemblyMix.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4859 2022-12-18 16:46:46.000000 dnacauldron-2.0.8/dnacauldron/AssemblyMix/LigaseCyclingReactionMix.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3768 2022-06-10 21:42:51.000000 dnacauldron-2.0.8/dnacauldron/AssemblyMix/RestrictionLigationMix.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-05-25 21:39:39.690314 dnacauldron-2.0.8/dnacauldron/AssemblyMix/StickyEndAssemblyMix/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     5787 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/AssemblyMix/StickyEndAssemblyMix/PlotsMixin.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3423 2022-12-18 16:46:46.000000 dnacauldron-2.0.8/dnacauldron/AssemblyMix/StickyEndAssemblyMix/SlotsMixin.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2348 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/AssemblyMix/StickyEndAssemblyMix/StickyEndAssemblyMix.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)       54 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/AssemblyMix/StickyEndAssemblyMix/__init__.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      509 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/AssemblyMix/__init__.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-05-25 21:39:39.690314 dnacauldron-2.0.8/dnacauldron/AssemblyMix/mixins/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3607 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/AssemblyMix/mixins/ConnectorsMixin.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)    11176 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/AssemblyMix/mixins/ConstructsMixin.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1733 2022-12-18 16:46:46.000000 dnacauldron-2.0.8/dnacauldron/AssemblyMix/mixins/FragmentsMixin.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3938 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/AssemblyMix/mixins/GraphsMixin.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2150 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/AssemblyMix/mixins/PlotsMixin.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      204 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/AssemblyMix/mixins/__init__.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-05-25 21:39:39.690314 dnacauldron-2.0.8/dnacauldron/AssemblyPlan/
+-rw-rw-r--   0 peter     (1000) peter     (1000)    10277 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/AssemblyPlan/AssemblyPlan.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)    12568 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/AssemblyPlan/AssemblyPlanSimulation.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      168 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/AssemblyPlan/__init__.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4111 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/AssemblyPlan/plot_leveled_graph.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3236 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/Filter.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-05-25 21:39:39.690314 dnacauldron-2.0.8/dnacauldron/Fragment/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2146 2022-12-18 17:38:32.000000 dnacauldron-2.0.8/dnacauldron/Fragment/Fragment.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     5698 2022-12-18 16:46:46.000000 dnacauldron-2.0.8/dnacauldron/Fragment/FragmentChain.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-05-25 21:39:39.694314 dnacauldron-2.0.8/dnacauldron/Fragment/HomologousFragment/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6008 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/Fragment/HomologousFragment/HomologousFragment.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3418 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/Fragment/HomologousFragment/HomologyChecker.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      148 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/Fragment/HomologousFragment/__init__.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-05-25 21:39:39.694314 dnacauldron-2.0.8/dnacauldron/Fragment/StickyEndFragment/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1676 2023-05-25 21:39:26.000000 dnacauldron-2.0.8/dnacauldron/Fragment/StickyEndFragment/StickyEnd.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6665 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/Fragment/StickyEndFragment/StickyEndFragment.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     9470 2023-05-25 21:39:26.000000 dnacauldron-2.0.8/dnacauldron/Fragment/StickyEndFragment/StickyEndSeq.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      316 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/Fragment/StickyEndFragment/__init__.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      314 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/Fragment/__init__.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     7104 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/SequenceRepository.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1233 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/__init__.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-05-25 21:39:39.694314 dnacauldron-2.0.8/dnacauldron/biotools/
+-rw-rw-r--   0 peter     (1000) peter     (1000)      342 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/biotools/__init__.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      921 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/biotools/autoselect_enzyme.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4516 2022-12-18 17:38:32.000000 dnacauldron-2.0.8/dnacauldron/biotools/record_operations.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     8602 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/biotools/sequence_io.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-05-25 21:39:39.694314 dnacauldron-2.0.8/dnacauldron/report_assets/
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-05-25 21:39:39.694314 dnacauldron-2.0.8/dnacauldron/report_assets/imgs/
+-rw-rw-r--   0 peter     (1000) peter     (1000)    19541 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/report_assets/imgs/logo.png
+-rw-rw-r--   0 peter     (1000) peter     (1000)      303 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/report_assets/report_style.css
+-rw-rw-r--   0 peter     (1000) peter     (1000)      973 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/report_assets/simulation_report.pug
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1989 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/reports.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      562 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/tools.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-05-25 21:39:39.694314 dnacauldron-2.0.8/dnacauldron/utils/
+-rw-rw-r--   0 peter     (1000) peter     (1000)      512 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/dnacauldron/utils/__init__.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)    11627 2022-12-18 16:46:46.000000 dnacauldron-2.0.8/dnacauldron/utils/insert_parts_on_backbones.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4918 2022-12-18 16:46:46.000000 dnacauldron-2.0.8/dnacauldron/utils/utils.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)       22 2023-05-25 21:39:26.000000 dnacauldron-2.0.8/dnacauldron/version.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-05-25 21:39:39.686314 dnacauldron-2.0.8/dnacauldron.egg-info/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1624 2023-05-25 21:39:39.000000 dnacauldron-2.0.8/dnacauldron.egg-info/PKG-INFO
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3745 2023-05-25 21:39:39.000000 dnacauldron-2.0.8/dnacauldron.egg-info/SOURCES.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)        1 2023-05-25 21:39:39.000000 dnacauldron-2.0.8/dnacauldron.egg-info/dependency_links.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)      175 2023-05-25 21:39:39.000000 dnacauldron-2.0.8/dnacauldron.egg-info/requires.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)       12 2023-05-25 21:39:39.000000 dnacauldron-2.0.8/dnacauldron.egg-info/top_level.txt
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-05-25 21:39:39.686314 dnacauldron-2.0.8/examples/
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-05-25 21:39:39.694314 dnacauldron-2.0.8/examples/BASIC_assembly/
+-rw-rw-r--   0 peter     (1000) peter     (1000)      330 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/examples/BASIC_assembly/BASIC_assembly.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-05-25 21:39:39.694314 dnacauldron-2.0.8/examples/autoselect_connectors/
+-rw-rw-r--   0 peter     (1000) peter     (1000)      795 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/examples/autoselect_connectors/autoselect_connectors.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-05-25 21:39:39.694314 dnacauldron-2.0.8/examples/combinatorial_golden_gate/
+-rw-rw-r--   0 peter     (1000) peter     (1000)      661 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/examples/combinatorial_golden_gate/combinatorial_golden_gate.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      640 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/examples/combinatorial_golden_gate/random_constructs_from_combinatorial_design.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-05-25 21:39:39.694314 dnacauldron-2.0.8/examples/gibson_assembly/
+-rw-rw-r--   0 peter     (1000) peter     (1000)      634 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/examples/gibson_assembly/gibson_assembly.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-05-25 21:39:39.694314 dnacauldron-2.0.8/examples/hierarchical_biobrick/
+-rw-rw-r--   0 peter     (1000) peter     (1000)      454 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/examples/hierarchical_biobrick/hierarchical_biobrick.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-05-25 21:39:39.694314 dnacauldron-2.0.8/examples/hierarchical_golden_gate/
+-rw-rw-r--   0 peter     (1000) peter     (1000)      523 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/examples/hierarchical_golden_gate/hierarchical_golden_gate.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-05-25 21:39:39.694314 dnacauldron-2.0.8/examples/lcr_assembly/
+-rw-rw-r--   0 peter     (1000) peter     (1000)      329 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/examples/lcr_assembly/README.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)      384 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/examples/lcr_assembly/example_with_assembly_plan.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-05-25 21:39:39.694314 dnacauldron-2.0.8/examples/multi_assemby_plan/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1511 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/examples/multi_assemby_plan/multi_assembly.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     8512 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/ez_setup.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1275 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/pypi-readme.rst
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-05-25 21:39:39.694314 dnacauldron-2.0.8/scripts/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2213 2021-11-25 11:15:52.000000 dnacauldron-2.0.8/scripts/dnacauldron
+-rw-rw-r--   0 peter     (1000) peter     (1000)       38 2023-05-25 21:39:39.698314 dnacauldron-2.0.8/setup.cfg
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1056 2022-06-10 21:42:51.000000 dnacauldron-2.0.8/setup.py
```

### Comparing `dnacauldron-2.0.7/LICENCE.txt` & `dnacauldron-2.0.8/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.7/PKG-INFO` & `dnacauldron-2.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnacauldron
-Version: 2.0.7
+Version: 2.0.8
 Summary: Cloning simulation for DNA assembly (Golden Gate, Gibson...)
 Home-page: https://github.com/Edinburgh-Genome-Foundry/DnaCauldron
 Author: Zulko
 License: MIT
 Keywords: DNA assembly cloning simulator synthetic biology
 Platform: UNKNOWN
 Provides-Extra: reports
```

### Comparing `dnacauldron-2.0.7/README.rst` & `dnacauldron-2.0.8/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 .. raw:: html
 
     <p align="center">
     <img alt="DNA Cauldron Logo" title="DNA Cauldron Logo" src="https://raw.githubusercontent.com/Edinburgh-Genome-Foundry/DnaCauldron/master/docs/_static/images/title.png" width="500">
     <br /><br />
     </p>
 
-.. image:: https://app.travis-ci.com/Edinburgh-Genome-Foundry/DnaCauldron.svg?branch=master
-    :target: https://app.travis-ci.com/Edinburgh-Genome-Foundry/DnaCauldron
-    :alt: Travis CI build status
+.. image:: https://github.com/Edinburgh-Genome-Foundry/DnaCauldron/actions/workflows/build.yml/badge.svg
+    :target: https://github.com/Edinburgh-Genome-Foundry/DnaCauldron/actions/workflows/build.yml
+    :alt: GitHub CI build status
 
 .. image:: https://coveralls.io/repos/github/Edinburgh-Genome-Foundry/DnaCauldron/badge.svg?branch=master
-  :target: https://coveralls.io/github/Edinburgh-Genome-Foundry/DnaCauldron?branch=master
+    :target: https://coveralls.io/github/Edinburgh-Genome-Foundry/DnaCauldron?branch=master
 
 
 DNA Cauldron
 ============
 
 DNA Cauldron (full documentation `here <https://edinburgh-genome-foundry.github.io/DnaCauldron/>`_)
 is a generic cloning simulation framework to predict
```

### Comparing `dnacauldron-2.0.7/dnacauldron/Assembly/Assembly.py` & `dnacauldron-2.0.8/dnacauldron/Assembly/Assembly.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.7/dnacauldron/Assembly/AssemblyFlaw.py` & `dnacauldron-2.0.8/dnacauldron/Assembly/AssemblyFlaw.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.7/dnacauldron/Assembly/AssemblyReportWriter/AssemblyPlotTranslator.py` & `dnacauldron-2.0.8/dnacauldron/Assembly/AssemblyReportWriter/AssemblyPlotTranslator.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.7/dnacauldron/Assembly/AssemblyReportWriter/AssemblyReportPlotsMixin.py` & `dnacauldron-2.0.8/dnacauldron/Assembly/AssemblyReportWriter/AssemblyReportPlotsMixin.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.7/dnacauldron/Assembly/AssemblyReportWriter/AssemblyReportWriter.py` & `dnacauldron-2.0.8/dnacauldron/Assembly/AssemblyReportWriter/AssemblyReportWriter.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.7/dnacauldron/Assembly/AssemblyReportWriter/plot_cuts.py` & `dnacauldron-2.0.8/dnacauldron/Assembly/AssemblyReportWriter/plot_cuts.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.7/dnacauldron/Assembly/AssemblySimulation.py` & `dnacauldron-2.0.8/dnacauldron/Assembly/AssemblySimulation.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.7/dnacauldron/Assembly/__init__.py` & `dnacauldron-2.0.8/dnacauldron/Assembly/__init__.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.7/dnacauldron/Assembly/builtin_assembly_classes/BASICAssembly.py` & `dnacauldron-2.0.8/dnacauldron/Assembly/builtin_assembly_classes/BASICAssembly.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
       connector autocompletion.
 
     dependencies
       (do not use). Metadata indicating which assemblies depend on this
       assembly, or are depended on by it.
 
     """
-    def simulate_adapters_assembly(self, records):
+    def simulate_adapters_assembly(self, records, sequence_repository):
         original_part = records[1]
         mix = RestrictionLigationMix(
             records,
             enzymes=["BsaI"],
             name="%s_adapters_ligation" % original_part.id,
         )
         adapter_fragments = []
@@ -65,16 +65,17 @@
             right_end = str(fragment.seq.right_end)
             if max(len(left_end), len(right_end)) > 4:
                 adapter_fragments.append(fragment_index)
         if len(adapter_fragments) != 4:  # Two "ends" and their complements
             error = AssemblyFlaw(
                 message="Two many fragments have a long overhang",
                 data={"parts": [r.id for r in records]},
+                assembly=self
             )
-            return AssemblySimulation(errors=[error], mixes=(mix,))
+            return mix, error
         graph = mix.connections_graph
         constructs = []
         for start, end in itertools.product(adapter_fragments, repeat=2):
             if end == start:
                 continue
             if nx.has_path(graph, start, end):
                 path = nx.shortest_path(graph, start, end)
@@ -114,15 +115,15 @@
 
         # ANNEAL PARTS AND ADAPTERS SEPARATELY
 
         adapted_part_records = []
         errors, warnings = [], []
         part_triplets = [parts[i : i + 3] for i in range(0, L, 3)]
         for triplet in part_triplets:
-            simulation = self.simulate_adapters_assembly(triplet)
+            simulation = self.simulate_adapters_assembly(triplet, sequence_repository)
             if isinstance(simulation, StickyEndFragment):
                 adapted_part_records.append(simulation)
             else:
                 mix, error = simulation
                 return AssemblySimulation(
                     assembly=self,
                     sequence_repository=sequence_repository,
```

### Comparing `dnacauldron-2.0.7/dnacauldron/Assembly/builtin_assembly_classes/BioBrickStandardAssembly.py` & `dnacauldron-2.0.8/dnacauldron/Assembly/builtin_assembly_classes/BioBrickStandardAssembly.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.7/dnacauldron/Assembly/builtin_assembly_classes/GibsonAssembly.py` & `dnacauldron-2.0.8/dnacauldron/Assembly/builtin_assembly_classes/GibsonAssembly.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.7/dnacauldron/Assembly/builtin_assembly_classes/LigaseCyclingReactionAssembly.py` & `dnacauldron-2.0.8/dnacauldron/Assembly/builtin_assembly_classes/LigaseCyclingReactionAssembly.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.7/dnacauldron/Assembly/builtin_assembly_classes/OligoPairAnnealing.py` & `dnacauldron-2.0.8/dnacauldron/Assembly/builtin_assembly_classes/OligoPairAnnealing.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,23 +8,26 @@
     StickyEndSeq,
     StickyEndFragment,
 )
 
 
 class OligoPairAnnealing(Assembly):
     """Represent and simulate oligo pair annealing
-    
+
+    This class is used for BASIC assembly simulation.
+
+
     Parameters
     ----------
-    
+
     parts
       A list of parts names corresponding to records in a repository.
       The parts should be exactly two, corresponding oligo sequences in
       direct sense (5'3').
-    
+
     homology_checker
       An HomologyChecker instance defining which oligo homology sizes and
       melting temperatures are valid. WARNING: DEPRECATED. Open an issue if
       you need this feature.
 
     name
       Name of the assembly as it will appear in reports.
@@ -71,33 +74,32 @@
             result = StickyEndFragment(seq)
             result.id = result.original_part = self.name
             p1_copy = deepcopy(p1)
             p2_copy = deepcopy(p2)
             p1_copy.is_reversed = False
             p2_copy.is_reversed = True
             result.fragments = [p1_copy, p2_copy]
-            result.annotations['topology'] = 'linear'
+            result.annotations["topology"] = "linear"
             return result
 
         products = []
         p1_fwd = str(p1.seq)
         p2_fwd = str(p2.seq)
         p2_rv = str(p2.seq.reverse_complement())
         p1_rv = str(p1.seq.reverse_complement())
-        
-        
+
         if p2_rv in p1_fwd:
             products.append(internal_annealing(p1_fwd, p2_rv))
         if p1_rv in p2_fwd:
             products.append(internal_annealing(p2_fwd, p1_rv))
 
         errors = []
         if len(products) == 0:
             msg = "No homology found between oligos %s and %s" % (p1.id, p2.id)
             errors.append(AssemblyFlaw(message=msg, assembly=self))
 
         return AssemblySimulation(
             assembly=self,
             sequence_repository=sequence_repository,
             construct_records=products,
-            errors=errors
+            errors=errors,
         )
```

### Comparing `dnacauldron-2.0.7/dnacauldron/Assembly/builtin_assembly_classes/Type2sRestrictionAssembly.py` & `dnacauldron-2.0.8/dnacauldron/Assembly/builtin_assembly_classes/Type2sRestrictionAssembly.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.7/dnacauldron/Assembly/builtin_assembly_classes/__init__.py` & `dnacauldron-2.0.8/dnacauldron/Assembly/builtin_assembly_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.7/dnacauldron/AssemblyMix/AssemblyMix.py` & `dnacauldron-2.0.8/dnacauldron/AssemblyMix/AssemblyMix.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.7/dnacauldron/AssemblyMix/HomologousAssemblyMix.py` & `dnacauldron-2.0.8/dnacauldron/AssemblyMix/HomologousAssemblyMix.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.7/dnacauldron/AssemblyMix/LigaseCyclingReactionMix.py` & `dnacauldron-2.0.8/dnacauldron/AssemblyMix/LigaseCyclingReactionMix.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.7/dnacauldron/AssemblyMix/RestrictionLigationMix.py` & `dnacauldron-2.0.8/dnacauldron/AssemblyMix/RestrictionLigationMix.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.7/dnacauldron/AssemblyMix/StickyEndAssemblyMix/PlotsMixin.py` & `dnacauldron-2.0.8/dnacauldron/AssemblyMix/StickyEndAssemblyMix/PlotsMixin.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.7/dnacauldron/AssemblyMix/StickyEndAssemblyMix/SlotsMixin.py` & `dnacauldron-2.0.8/dnacauldron/AssemblyMix/StickyEndAssemblyMix/SlotsMixin.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.7/dnacauldron/AssemblyMix/StickyEndAssemblyMix/StickyEndAssemblyMix.py` & `dnacauldron-2.0.8/dnacauldron/AssemblyMix/StickyEndAssemblyMix/StickyEndAssemblyMix.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.7/dnacauldron/AssemblyMix/mixins/ConnectorsMixin.py` & `dnacauldron-2.0.8/dnacauldron/AssemblyMix/mixins/ConnectorsMixin.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.7/dnacauldron/AssemblyMix/mixins/ConstructsMixin.py` & `dnacauldron-2.0.8/dnacauldron/AssemblyMix/mixins/ConstructsMixin.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.7/dnacauldron/AssemblyMix/mixins/FragmentsMixin.py` & `dnacauldron-2.0.8/dnacauldron/AssemblyMix/mixins/FragmentsMixin.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.7/dnacauldron/AssemblyMix/mixins/GraphsMixin.py` & `dnacauldron-2.0.8/dnacauldron/AssemblyMix/mixins/GraphsMixin.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.7/dnacauldron/AssemblyMix/mixins/PlotsMixin.py` & `dnacauldron-2.0.8/dnacauldron/AssemblyMix/mixins/PlotsMixin.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.7/dnacauldron/AssemblyPlan/AssemblyPlan.py` & `dnacauldron-2.0.8/dnacauldron/AssemblyPlan/AssemblyPlan.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.7/dnacauldron/AssemblyPlan/AssemblyPlanSimulation.py` & `dnacauldron-2.0.8/dnacauldron/AssemblyPlan/AssemblyPlanSimulation.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.7/dnacauldron/AssemblyPlan/plot_leveled_graph.py` & `dnacauldron-2.0.8/dnacauldron/AssemblyPlan/plot_leveled_graph.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.7/dnacauldron/Filter.py` & `dnacauldron-2.0.8/dnacauldron/Filter.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.7/dnacauldron/Fragment/Fragment.py` & `dnacauldron-2.0.8/dnacauldron/Fragment/Fragment.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.7/dnacauldron/Fragment/FragmentChain.py` & `dnacauldron-2.0.8/dnacauldron/Fragment/FragmentChain.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.7/dnacauldron/Fragment/HomologousFragment/HomologousFragment.py` & `dnacauldron-2.0.8/dnacauldron/Fragment/HomologousFragment/HomologousFragment.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.7/dnacauldron/Fragment/HomologousFragment/HomologyChecker.py` & `dnacauldron-2.0.8/dnacauldron/Fragment/HomologousFragment/HomologyChecker.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.7/dnacauldron/Fragment/StickyEndFragment/StickyEnd.py` & `dnacauldron-2.0.8/dnacauldron/Fragment/StickyEndFragment/StickyEnd.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,28 +25,28 @@
     strand
       The strand (+1 or -1) on which the protusion is.
 
     **k
       Optional keyword arguments for the sequence, such as ``alphabet`` etc.
     """
 
-    def __init__(self, data, strand, **k):
+    def __init__(self, data, strand=None, **k):
         Seq.__init__(self, str(data).upper(), **k)
         self.strand = strand
 
     def reverse_complement(self):
 
         if has_dna_alphabet:  # Biopython <1.78
             return StickyEnd(
                 str(Seq.reverse_complement(self)),
                 strand=-self.strand,
                 alphabet=self.alphabet,
             )
         else:
-            return StickyEnd(str(Seq.reverse_complement(self)), strand=-self.strand,)
+            return StickyEnd(str(Seq(self).reverse_complement()), strand=-self.strand,)
 
     def __repr__(self):
         return "%s(%s)" % (Seq.__str__(self), {1: "+", -1: "-"}[self.strand])
 
     def will_clip_directly_with(self, other):
         return (
             (other is not None)
```

### Comparing `dnacauldron-2.0.7/dnacauldron/Fragment/StickyEndFragment/StickyEndFragment.py` & `dnacauldron-2.0.8/dnacauldron/Fragment/StickyEndFragment/StickyEndFragment.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.7/dnacauldron/Fragment/StickyEndFragment/StickyEndSeq.py` & `dnacauldron-2.0.8/dnacauldron/Fragment/StickyEndFragment/StickyEndSeq.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     """
 
     def __init__(self, data, left_end=None, right_end=None, **k):
         Seq.__init__(self, str(data), **k)
         self.left_end = left_end
         self.right_end = right_end
 
-    def reverse_complement(self):
+    def reverse_complement(self, inplace=False):
         """The reverse is a StickyEndSeq with reversed ends
 
         left-right versions are interchanged and reverse complemented.
         """
 
         if has_dna_alphabet:  # Biopython <1.78
             sticky_end_seq = StickyEndSeq(
@@ -39,15 +39,15 @@
                 right_end=None
                 if self.left_end is None
                 else self.left_end.reverse_complement(),
                 alphabet=self.alphabet,
             )
         else:
             sticky_end_seq = StickyEndSeq(
-                str(Seq.reverse_complement(self)),
+                str(Seq(self).reverse_complement()),
                 left_end=None
                 if self.right_end is None
                 else self.right_end.reverse_complement(),
                 right_end=None
                 if self.left_end is None
                 else self.left_end.reverse_complement(),
             )
```

### Comparing `dnacauldron-2.0.7/dnacauldron/SequenceRepository.py` & `dnacauldron-2.0.8/dnacauldron/SequenceRepository.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.7/dnacauldron/__init__.py` & `dnacauldron-2.0.8/dnacauldron/__init__.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.7/dnacauldron/biotools/autoselect_enzyme.py` & `dnacauldron-2.0.8/dnacauldron/biotools/autoselect_enzyme.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.7/dnacauldron/biotools/record_operations.py` & `dnacauldron-2.0.8/dnacauldron/biotools/record_operations.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.7/dnacauldron/biotools/sequence_io.py` & `dnacauldron-2.0.8/dnacauldron/biotools/sequence_io.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.7/dnacauldron/report_assets/imgs/logo.png` & `dnacauldron-2.0.8/dnacauldron/report_assets/imgs/logo.png`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.7/dnacauldron/report_assets/simulation_report.pug` & `dnacauldron-2.0.8/dnacauldron/report_assets/simulation_report.pug`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.7/dnacauldron/reports.py` & `dnacauldron-2.0.8/dnacauldron/reports.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.7/dnacauldron/tools.py` & `dnacauldron-2.0.8/dnacauldron/tools.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.7/dnacauldron/utils/__init__.py` & `dnacauldron-2.0.8/dnacauldron/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.7/dnacauldron/utils/insert_parts_on_backbones.py` & `dnacauldron-2.0.8/dnacauldron/utils/insert_parts_on_backbones.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.7/dnacauldron/utils/utils.py` & `dnacauldron-2.0.8/dnacauldron/utils/utils.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.7/dnacauldron.egg-info/PKG-INFO` & `dnacauldron-2.0.8/dnacauldron.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnacauldron
-Version: 2.0.7
+Version: 2.0.8
 Summary: Cloning simulation for DNA assembly (Golden Gate, Gibson...)
 Home-page: https://github.com/Edinburgh-Genome-Foundry/DnaCauldron
 Author: Zulko
 License: MIT
 Keywords: DNA assembly cloning simulator synthetic biology
 Platform: UNKNOWN
 Provides-Extra: reports
```

### Comparing `dnacauldron-2.0.7/dnacauldron.egg-info/SOURCES.txt` & `dnacauldron-2.0.8/dnacauldron.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.7/examples/autoselect_connectors/autoselect_connectors.py` & `dnacauldron-2.0.8/examples/autoselect_connectors/autoselect_connectors.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.7/examples/combinatorial_golden_gate/combinatorial_golden_gate.py` & `dnacauldron-2.0.8/examples/combinatorial_golden_gate/combinatorial_golden_gate.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.7/examples/combinatorial_golden_gate/random_constructs_from_combinatorial_design.py` & `dnacauldron-2.0.8/examples/combinatorial_golden_gate/random_constructs_from_combinatorial_design.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.7/examples/gibson_assembly/gibson_assembly.py` & `dnacauldron-2.0.8/examples/gibson_assembly/gibson_assembly.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.7/examples/hierarchical_golden_gate/hierarchical_golden_gate.py` & `dnacauldron-2.0.8/examples/hierarchical_golden_gate/hierarchical_golden_gate.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.7/examples/multi_assemby_plan/multi_assembly.py` & `dnacauldron-2.0.8/examples/multi_assemby_plan/multi_assembly.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.7/ez_setup.py` & `dnacauldron-2.0.8/ez_setup.py`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.7/pypi-readme.rst` & `dnacauldron-2.0.8/pypi-readme.rst`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.7/scripts/dnacauldron` & `dnacauldron-2.0.8/scripts/dnacauldron`

 * *Files identical despite different names*

### Comparing `dnacauldron-2.0.7/setup.py` & `dnacauldron-2.0.8/setup.py`

 * *Files identical despite different names*

