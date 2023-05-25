# Comparing `tmp/pywfa-0.4.1.tar.gz` & `tmp/pywfa-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywfa-0.4.1.tar", last modified: Wed Mar  1 22:03:02 2023, max compression
+gzip compressed data, was "pywfa-0.4.2.tar", last modified: Wed May 24 10:17:00 2023, max compression
```

## Comparing `pywfa-0.4.1.tar` & `pywfa-0.4.2.tar`

### file list

```diff
@@ -1,183 +1,182 @@
-drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-03-01 22:03:02.853280 pywfa-0.4.1/
--rw-r--r--   0 kezcleal   (501) staff       (20)     1069 2022-03-13 11:23:19.000000 pywfa-0.4.1/LICENSE.md
--rw-r--r--   0 kezcleal   (501) staff       (20)       98 2022-07-15 09:07:29.000000 pywfa-0.4.1/MANIFEST.in
--rw-r--r--   0 kezcleal   (501) staff       (20)      274 2023-03-01 22:03:02.852971 pywfa-0.4.1/PKG-INFO
--rw-r--r--   0 kezcleal   (501) staff       (20)     6382 2023-01-05 12:17:08.000000 pywfa-0.4.1/README.rst
-drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-03-01 22:03:01.454517 pywfa-0.4.1/pywfa/
--rw-r--r--   0 kezcleal   (501) staff       (20)     6148 2022-07-15 09:12:49.000000 pywfa-0.4.1/pywfa/.DS_Store
-drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-03-01 22:03:01.127849 pywfa-0.4.1/pywfa/WFA2_lib/
-drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-03-01 22:03:01.462195 pywfa-0.4.1/pywfa/WFA2_lib/alignment/
--rw-rw-r--   0 kezcleal   (501) staff       (20)      850 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/alignment/Makefile
--rw-rw-r--   0 kezcleal   (501) staff       (20)     1483 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/alignment/affine2p_penalties.c
--rw-rw-r--   0 kezcleal   (501) staff       (20)     2317 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/alignment/affine2p_penalties.h
--rw-rw-r--   0 kezcleal   (501) staff       (20)     1482 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/alignment/affine_penalties.c
--rw-rw-r--   0 kezcleal   (501) staff       (20)     2043 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/alignment/affine_penalties.h
--rw-rw-r--   0 kezcleal   (501) staff       (20)    15257 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/alignment/cigar.c
--rw-rw-r--   0 kezcleal   (501) staff       (20)     3882 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/alignment/cigar.h
--rw-rw-r--   0 kezcleal   (501) staff       (20)     1767 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/alignment/linear_penalties.h
--rw-rw-r--   0 kezcleal   (501) staff       (20)     3714 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/alignment/score_matrix.c
--rw-rw-r--   0 kezcleal   (501) staff       (20)     2277 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/alignment/score_matrix.h
-drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-03-01 22:03:01.485018 pywfa-0.4.1/pywfa/WFA2_lib/build/
--rw-r--r--   0 kezcleal   (501) staff       (20)      680 2023-03-01 22:02:23.000000 pywfa-0.4.1/pywfa/WFA2_lib/build/affine2p_penalties.o
--rw-r--r--   0 kezcleal   (501) staff       (20)      680 2023-03-01 22:02:23.000000 pywfa-0.4.1/pywfa/WFA2_lib/build/affine_penalties.o
--rw-r--r--   0 kezcleal   (501) staff       (20)     7348 2023-03-01 22:02:28.000000 pywfa-0.4.1/pywfa/WFA2_lib/build/bitmap.o
--rw-r--r--   0 kezcleal   (501) staff       (20)    31884 2023-03-01 22:02:26.000000 pywfa-0.4.1/pywfa/WFA2_lib/build/cigar.o
--rw-r--r--   0 kezcleal   (501) staff       (20)     4344 2023-03-01 22:02:28.000000 pywfa-0.4.1/pywfa/WFA2_lib/build/commons.o
--rw-r--r--   0 kezcleal   (501) staff       (20)     2456 2023-03-01 22:02:28.000000 pywfa-0.4.1/pywfa/WFA2_lib/build/dna_text.o
--rw-r--r--   0 kezcleal   (501) staff       (20)    10732 2023-03-01 22:02:28.000000 pywfa-0.4.1/pywfa/WFA2_lib/build/heatmap.o
--rw-r--r--   0 kezcleal   (501) staff       (20)    35580 2023-03-01 22:02:26.000000 pywfa-0.4.1/pywfa/WFA2_lib/build/mm_allocator.o
--rw-r--r--   0 kezcleal   (501) staff       (20)    15460 2023-03-01 22:02:26.000000 pywfa-0.4.1/pywfa/WFA2_lib/build/mm_stack.o
--rw-r--r--   0 kezcleal   (501) staff       (20)    21188 2023-03-01 22:02:26.000000 pywfa-0.4.1/pywfa/WFA2_lib/build/profiler_counter.o
--rw-r--r--   0 kezcleal   (501) staff       (20)    20956 2023-03-01 22:02:28.000000 pywfa-0.4.1/pywfa/WFA2_lib/build/profiler_timer.o
--rw-r--r--   0 kezcleal   (501) staff       (20)    10220 2023-03-01 22:02:26.000000 pywfa-0.4.1/pywfa/WFA2_lib/build/score_matrix.o
--rw-r--r--   0 kezcleal   (501) staff       (20)     8124 2023-03-01 22:02:28.000000 pywfa-0.4.1/pywfa/WFA2_lib/build/sequence_buffer.o
--rw-r--r--   0 kezcleal   (501) staff       (20)    13868 2023-03-01 22:02:28.000000 pywfa-0.4.1/pywfa/WFA2_lib/build/string_padded.o
--rw-r--r--   0 kezcleal   (501) staff       (20)     8104 2023-03-01 22:02:29.000000 pywfa-0.4.1/pywfa/WFA2_lib/build/vector.o
--rw-r--r--   0 kezcleal   (501) staff       (20)     9204 2023-03-01 22:02:33.000000 pywfa-0.4.1/pywfa/WFA2_lib/build/wavefront.o
--rw-r--r--   0 kezcleal   (501) staff       (20)    34440 2023-03-01 22:02:29.000000 pywfa-0.4.1/pywfa/WFA2_lib/build/wavefront_align.o
--rw-r--r--   0 kezcleal   (501) staff       (20)    38040 2023-03-01 22:02:30.000000 pywfa-0.4.1/pywfa/WFA2_lib/build/wavefront_aligner.o
--rw-r--r--   0 kezcleal   (501) staff       (20)     6988 2023-03-01 22:02:30.000000 pywfa-0.4.1/pywfa/WFA2_lib/build/wavefront_attributes.o
--rw-r--r--   0 kezcleal   (501) staff       (20)    41816 2023-03-01 22:02:30.000000 pywfa-0.4.1/pywfa/WFA2_lib/build/wavefront_backtrace.o
--rw-r--r--   0 kezcleal   (501) staff       (20)    29876 2023-03-01 22:02:30.000000 pywfa-0.4.1/pywfa/WFA2_lib/build/wavefront_backtrace_buffer.o
--rw-r--r--   0 kezcleal   (501) staff       (20)    28184 2023-03-01 22:02:30.000000 pywfa-0.4.1/pywfa/WFA2_lib/build/wavefront_backtrace_offload.o
--rw-r--r--   0 kezcleal   (501) staff       (20)    41248 2023-03-01 22:02:30.000000 pywfa-0.4.1/pywfa/WFA2_lib/build/wavefront_bialign.o
--rw-r--r--   0 kezcleal   (501) staff       (20)    37060 2023-03-01 22:02:30.000000 pywfa-0.4.1/pywfa/WFA2_lib/build/wavefront_components.o
--rw-r--r--   0 kezcleal   (501) staff       (20)    39996 2023-03-01 22:02:32.000000 pywfa-0.4.1/pywfa/WFA2_lib/build/wavefront_compute.o
--rw-r--r--   0 kezcleal   (501) staff       (20)    26904 2023-03-01 22:02:31.000000 pywfa-0.4.1/pywfa/WFA2_lib/build/wavefront_compute_affine.o
--rw-r--r--   0 kezcleal   (501) staff       (20)    32276 2023-03-01 22:02:31.000000 pywfa-0.4.1/pywfa/WFA2_lib/build/wavefront_compute_affine2p.o
--rw-r--r--   0 kezcleal   (501) staff       (20)    42120 2023-03-01 22:02:31.000000 pywfa-0.4.1/pywfa/WFA2_lib/build/wavefront_compute_edit.o
--rw-r--r--   0 kezcleal   (501) staff       (20)    25536 2023-03-01 22:02:31.000000 pywfa-0.4.1/pywfa/WFA2_lib/build/wavefront_compute_linear.o
--rw-r--r--   0 kezcleal   (501) staff       (20)    23780 2023-03-01 22:02:32.000000 pywfa-0.4.1/pywfa/WFA2_lib/build/wavefront_debug.o
--rw-r--r--   0 kezcleal   (501) staff       (20)    34280 2023-03-01 22:02:32.000000 pywfa-0.4.1/pywfa/WFA2_lib/build/wavefront_display.o
--rw-r--r--   0 kezcleal   (501) staff       (20)    28068 2023-03-01 22:02:32.000000 pywfa-0.4.1/pywfa/WFA2_lib/build/wavefront_extend.o
--rw-r--r--   0 kezcleal   (501) staff       (20)    41060 2023-03-01 22:02:32.000000 pywfa-0.4.1/pywfa/WFA2_lib/build/wavefront_heuristic.o
--rw-r--r--   0 kezcleal   (501) staff       (20)    21688 2023-03-01 22:02:32.000000 pywfa-0.4.1/pywfa/WFA2_lib/build/wavefront_pcigar.o
--rw-r--r--   0 kezcleal   (501) staff       (20)     9172 2023-03-01 22:02:32.000000 pywfa-0.4.1/pywfa/WFA2_lib/build/wavefront_penalties.o
--rw-r--r--   0 kezcleal   (501) staff       (20)    27092 2023-03-01 22:02:33.000000 pywfa-0.4.1/pywfa/WFA2_lib/build/wavefront_plot.o
--rw-r--r--   0 kezcleal   (501) staff       (20)    17492 2023-03-01 22:02:33.000000 pywfa-0.4.1/pywfa/WFA2_lib/build/wavefront_slab.o
-drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-03-01 22:03:01.567729 pywfa-0.4.1/pywfa/WFA2_lib/examples/
--rw-rw-r--   0 kezcleal   (501) staff       (20)     1156 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/examples/Makefile
--rw-rw-r--   0 kezcleal   (501) staff       (20)      693 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/examples/README.md
--rw-rw-r--   0 kezcleal   (501) staff       (20)     2992 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/examples/wfa_adapt.c
--rw-rw-r--   0 kezcleal   (501) staff       (20)     2661 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/examples/wfa_basic.c
--rw-rw-r--   0 kezcleal   (501) staff       (20)     2143 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/examples/wfa_bindings.cpp
--rw-rw-r--   0 kezcleal   (501) staff       (20)     2521 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/examples/wfa_lambda.cpp
--rw-rw-r--   0 kezcleal   (501) staff       (20)     2533 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/examples/wfa_repeated.c
-drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-03-01 22:03:02.429340 pywfa-0.4.1/pywfa/WFA2_lib/img/
--rw-rw-r--   0 kezcleal   (501) staff       (20)   351138 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/img/heuristics.aband.10.10.png
--rw-rw-r--   0 kezcleal   (501) staff       (20)   395217 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/img/heuristics.aband.50.50.png
--rw-rw-r--   0 kezcleal   (501) staff       (20)   358048 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/img/heuristics.band.10.10.png
--rw-rw-r--   0 kezcleal   (501) staff       (20)   423890 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/img/heuristics.band.10.150.png
--rw-rw-r--   0 kezcleal   (501) staff       (20)   502376 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/img/heuristics.none.png
--rw-rw-r--   0 kezcleal   (501) staff       (20)   394728 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/img/heuristics.wfadap.10.50.1.png
--rw-rw-r--   0 kezcleal   (501) staff       (20)   502078 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/img/heuristics.wfadap.10.50.10.png
--rw-rw-r--   0 kezcleal   (501) staff       (20)   907275 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/img/wfa.vs.swg.png
-drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-03-01 22:03:02.578731 pywfa-0.4.1/pywfa/WFA2_lib/lib/
--rw-r--r--   0 kezcleal   (501) staff       (20)   844160 2023-03-01 22:02:37.000000 pywfa-0.4.1/pywfa/WFA2_lib/lib/libwfa.a
-drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-03-01 22:03:02.673368 pywfa-0.4.1/pywfa/WFA2_lib/scripts/
--rwxr-xr-x   0 kezcleal   (501) staff       (20)      390 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/scripts/fasta2seq.sh
--rwxr-xr-x   0 kezcleal   (501) staff       (20)      442 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/scripts/seq2fasta.sh
--rw-rw-r--   0 kezcleal   (501) staff       (20)    10228 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/scripts/wfa.alg.cmp.py
--rw-rw-r--   0 kezcleal   (501) staff       (20)      393 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/scripts/wfa.alg.cmp.score.sh
--rw-rw-r--   0 kezcleal   (501) staff       (20)     6423 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/scripts/wfa.alg.rescore.py
--rw-rw-r--   0 kezcleal   (501) staff       (20)     9646 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/scripts/wfa2png.py
-drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-03-01 22:03:02.677432 pywfa-0.4.1/pywfa/WFA2_lib/system/
--rw-rw-r--   0 kezcleal   (501) staff       (20)      838 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/system/Makefile
--rw-rw-r--   0 kezcleal   (501) staff       (20)    22734 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/system/mm_allocator.c
--rw-rw-r--   0 kezcleal   (501) staff       (20)     4837 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/system/mm_allocator.h
--rw-rw-r--   0 kezcleal   (501) staff       (20)     9143 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/system/mm_stack.c
--rw-rw-r--   0 kezcleal   (501) staff       (20)     3510 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/system/mm_stack.h
--rw-rw-r--   0 kezcleal   (501) staff       (20)    10898 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/system/profiler_counter.c
--rw-rw-r--   0 kezcleal   (501) staff       (20)     4634 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/system/profiler_counter.h
--rw-rw-r--   0 kezcleal   (501) staff       (20)     7247 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/system/profiler_timer.c
--rw-rw-r--   0 kezcleal   (501) staff       (20)     3937 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/system/profiler_timer.h
-drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-03-01 22:03:02.708641 pywfa-0.4.1/pywfa/WFA2_lib/tools/
--rw-r--r--   0 kezcleal   (501) staff       (20)     6148 2022-07-15 09:13:52.000000 pywfa-0.4.1/pywfa/WFA2_lib/tools/.DS_Store
--rw-rw-r--   0 kezcleal   (501) staff       (20)    12243 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/tools/README.md
-drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-03-01 22:03:02.733158 pywfa-0.4.1/pywfa/WFA2_lib/utils/
--rw-rw-r--   0 kezcleal   (501) staff       (20)      884 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/utils/Makefile
--rw-rw-r--   0 kezcleal   (501) staff       (20)     4480 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/utils/bitmap.c
--rw-rw-r--   0 kezcleal   (501) staff       (20)     3033 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/utils/bitmap.h
--rw-rw-r--   0 kezcleal   (501) staff       (20)     2386 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/utils/commons.c
--rw-rw-r--   0 kezcleal   (501) staff       (20)     8785 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/utils/commons.h
--rw-rw-r--   0 kezcleal   (501) staff       (20)     2043 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/utils/dna_text.c
--rw-rw-r--   0 kezcleal   (501) staff       (20)     2276 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/utils/dna_text.h
--rw-rw-r--   0 kezcleal   (501) staff       (20)     5201 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/utils/heatmap.c
--rw-rw-r--   0 kezcleal   (501) staff       (20)     2402 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/utils/heatmap.h
--rw-rw-r--   0 kezcleal   (501) staff       (20)     5325 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/utils/sequence_buffer.c
--rw-rw-r--   0 kezcleal   (501) staff       (20)     2506 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/utils/sequence_buffer.h
--rw-rw-r--   0 kezcleal   (501) staff       (20)     5499 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/utils/string_padded.c
--rw-rw-r--   0 kezcleal   (501) staff       (20)     2560 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/utils/string_padded.h
--rw-rw-r--   0 kezcleal   (501) staff       (20)     4305 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/utils/vector.c
--rw-rw-r--   0 kezcleal   (501) staff       (20)     5011 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/utils/vector.h
-drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-03-01 22:03:02.753491 pywfa-0.4.1/pywfa/WFA2_lib/wavefront/
--rw-rw-r--   0 kezcleal   (501) staff       (20)     1520 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/wavefront/Makefile
--rw-rw-r--   0 kezcleal   (501) staff       (20)     6046 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront.c
--rw-rw-r--   0 kezcleal   (501) staff       (20)     4814 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront.h
--rw-rw-r--   0 kezcleal   (501) staff       (20)    20093 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_align.c
--rw-rw-r--   0 kezcleal   (501) staff       (20)     2192 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_align.h
--rw-rw-r--   0 kezcleal   (501) staff       (20)    18740 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_aligner.c
--rw-rw-r--   0 kezcleal   (501) staff       (20)     8290 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_aligner.h
--rw-rw-r--   0 kezcleal   (501) staff       (20)     3584 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_attributes.c
--rw-rw-r--   0 kezcleal   (501) staff       (20)     6499 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_attributes.h
--rw-rw-r--   0 kezcleal   (501) staff       (20)    20606 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_backtrace.c
--rw-rw-r--   0 kezcleal   (501) staff       (20)     2334 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_backtrace.h
--rw-rw-r--   0 kezcleal   (501) staff       (20)    20399 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_backtrace_buffer.c
--rw-rw-r--   0 kezcleal   (501) staff       (20)     6138 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_backtrace_buffer.h
--rw-rw-r--   0 kezcleal   (501) staff       (20)    12970 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_backtrace_offload.c
--rw-rw-r--   0 kezcleal   (501) staff       (20)     2538 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_backtrace_offload.h
--rw-rw-r--   0 kezcleal   (501) staff       (20)    21142 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_bialign.c
--rw-rw-r--   0 kezcleal   (501) staff       (20)     2719 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_bialign.h
--rw-rw-r--   0 kezcleal   (501) staff       (20)    19200 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_components.c
--rw-rw-r--   0 kezcleal   (501) staff       (20)     4128 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_components.h
--rw-rw-r--   0 kezcleal   (501) staff       (20)    19880 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_compute.c
--rw-rw-r--   0 kezcleal   (501) staff       (20)     3164 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_compute.h
--rw-rw-r--   0 kezcleal   (501) staff       (20)    10059 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_compute_affine.c
--rw-rw-r--   0 kezcleal   (501) staff       (20)     2132 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_compute_affine.h
--rw-rw-r--   0 kezcleal   (501) staff       (20)    14496 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_compute_affine2p.c
--rw-rw-r--   0 kezcleal   (501) staff       (20)     1783 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_compute_affine2p.h
--rw-rw-r--   0 kezcleal   (501) staff       (20)    13902 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_compute_edit.c
--rw-rw-r--   0 kezcleal   (501) staff       (20)     1755 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_compute_edit.h
--rw-rw-r--   0 kezcleal   (501) staff       (20)     7207 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_compute_linear.c
--rw-rw-r--   0 kezcleal   (501) staff       (20)     1769 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_compute_linear.h
--rw-rw-r--   0 kezcleal   (501) staff       (20)     9318 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_debug.c
--rw-rw-r--   0 kezcleal   (501) staff       (20)     1765 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_debug.h
--rw-rw-r--   0 kezcleal   (501) staff       (20)    10578 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_display.c
--rw-rw-r--   0 kezcleal   (501) staff       (20)     1911 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_display.h
--rw-rw-r--   0 kezcleal   (501) staff       (20)    18252 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_extend.c
--rw-rw-r--   0 kezcleal   (501) staff       (20)     2029 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_extend.h
--rw-rw-r--   0 kezcleal   (501) staff       (20)    22178 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_heuristic.c
--rw-rw-r--   0 kezcleal   (501) staff       (20)     4380 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_heuristic.h
--rw-rw-r--   0 kezcleal   (501) staff       (20)     2312 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_offset.h
--rw-rw-r--   0 kezcleal   (501) staff       (20)     8949 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_pcigar.c
--rw-rw-r--   0 kezcleal   (501) staff       (20)     4335 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_pcigar.h
--rw-rw-r--   0 kezcleal   (501) staff       (20)     8443 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_penalties.c
--rw-rw-r--   0 kezcleal   (501) staff       (20)     4011 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_penalties.h
--rw-rw-r--   0 kezcleal   (501) staff       (20)     9696 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_plot.c
--rw-rw-r--   0 kezcleal   (501) staff       (20)     2765 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_plot.h
--rw-rw-r--   0 kezcleal   (501) staff       (20)    11285 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_slab.c
--rw-rw-r--   0 kezcleal   (501) staff       (20)     3361 2022-07-06 18:32:49.000000 pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_slab.h
--rw-r--r--   0 kezcleal   (501) staff       (20)   109797 2022-03-14 10:43:36.000000 pywfa-0.4.1/pywfa/WFA_wrap.c
--rw-r--r--   0 kezcleal   (501) staff       (20)    23033 2022-03-17 21:23:24.000000 pywfa-0.4.1/pywfa/WFA_wrap.pxd
--rw-r--r--   0 kezcleal   (501) staff       (20)      143 2022-03-17 16:10:01.000000 pywfa-0.4.1/pywfa/__init__.py
--rw-r--r--   0 kezcleal   (501) staff       (20)   657284 2023-01-05 12:18:00.000000 pywfa-0.4.1/pywfa/align.c
--rwxr-xr-x   0 kezcleal   (501) staff       (20)   596077 2023-03-01 22:02:47.000000 pywfa-0.4.1/pywfa/align.cpython-310-darwin.so
--rwxr-xr-x   0 kezcleal   (501) staff       (20)   340288 2023-03-01 22:02:47.000000 pywfa-0.4.1/pywfa/align.cpython-39-darwin.so
--rw-r--r--   0 kezcleal   (501) staff       (20)      369 2022-03-17 21:21:36.000000 pywfa-0.4.1/pywfa/align.pxd
--rw-r--r--   0 kezcleal   (501) staff       (20)    20736 2023-01-05 12:11:20.000000 pywfa-0.4.1/pywfa/align.pyx
-drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-03-01 22:03:02.834785 pywfa-0.4.1/pywfa/tests/
--rw-r--r--   0 kezcleal   (501) staff       (20)        0 2022-03-13 11:24:44.000000 pywfa-0.4.1/pywfa/tests/__init__.py
--rw-r--r--   0 kezcleal   (501) staff       (20)      727 2022-03-15 08:50:50.000000 pywfa-0.4.1/pywfa/tests/long.fa
--rw-r--r--   0 kezcleal   (501) staff       (20)     2214 2022-03-15 08:59:45.000000 pywfa-0.4.1/pywfa/tests/long.reference.fa
--rw-r--r--   0 kezcleal   (501) staff       (20)     1133 2022-03-16 11:51:32.000000 pywfa-0.4.1/pywfa/tests/short.fa
--rw-r--r--   0 kezcleal   (501) staff       (20)     4797 2022-03-16 11:50:49.000000 pywfa-0.4.1/pywfa/tests/short.reference.fa
--rw-r--r--   0 kezcleal   (501) staff       (20)     9054 2023-01-05 11:11:42.000000 pywfa-0.4.1/pywfa/tests/test.py
-drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-03-01 22:03:01.457381 pywfa-0.4.1/pywfa.egg-info/
--rw-r--r--   0 kezcleal   (501) staff       (20)      274 2023-03-01 22:03:00.000000 pywfa-0.4.1/pywfa.egg-info/PKG-INFO
--rw-r--r--   0 kezcleal   (501) staff       (20)     6301 2023-03-01 22:03:00.000000 pywfa-0.4.1/pywfa.egg-info/SOURCES.txt
--rw-r--r--   0 kezcleal   (501) staff       (20)        1 2023-03-01 22:03:00.000000 pywfa-0.4.1/pywfa.egg-info/dependency_links.txt
--rw-r--r--   0 kezcleal   (501) staff       (20)        1 2022-07-15 08:39:02.000000 pywfa-0.4.1/pywfa.egg-info/not-zip-safe
--rw-r--r--   0 kezcleal   (501) staff       (20)        7 2023-03-01 22:03:00.000000 pywfa-0.4.1/pywfa.egg-info/requires.txt
--rw-r--r--   0 kezcleal   (501) staff       (20)       33 2023-03-01 22:03:00.000000 pywfa-0.4.1/pywfa.egg-info/top_level.txt
--rw-r--r--   0 kezcleal   (501) staff       (20)       38 2023-03-01 22:03:02.853371 pywfa-0.4.1/setup.cfg
--rw-r--r--   0 kezcleal   (501) staff       (20)     4495 2023-03-01 21:59:07.000000 pywfa-0.4.1/setup.py
+drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-05-24 10:17:00.434820 pywfa-0.4.2/
+-rw-r--r--   0 kezcleal   (501) staff       (20)     1069 2023-05-24 10:14:49.000000 pywfa-0.4.2/LICENSE
+-rw-r--r--   0 kezcleal   (501) staff       (20)       98 2022-07-15 09:07:29.000000 pywfa-0.4.2/MANIFEST.in
+-rw-r--r--   0 kezcleal   (501) staff       (20)     6892 2023-05-24 10:17:00.434429 pywfa-0.4.2/PKG-INFO
+-rw-r--r--   0 kezcleal   (501) staff       (20)     6470 2023-05-24 10:14:49.000000 pywfa-0.4.2/README.rst
+-rw-r--r--   0 kezcleal   (501) staff       (20)     3775 2023-05-24 10:14:49.000000 pywfa-0.4.2/_custom_build.py
+-rw-r--r--   0 kezcleal   (501) staff       (20)      677 2023-05-24 10:14:49.000000 pywfa-0.4.2/pyproject.toml
+drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-05-24 10:16:58.467841 pywfa-0.4.2/pywfa/
+-rw-r--r--   0 kezcleal   (501) staff       (20)     6148 2022-07-15 09:12:49.000000 pywfa-0.4.2/pywfa/.DS_Store
+drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-05-24 10:16:58.307304 pywfa-0.4.2/pywfa/WFA2_lib/
+drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-05-24 10:16:58.482062 pywfa-0.4.2/pywfa/WFA2_lib/alignment/
+-rw-rw-r--   0 kezcleal   (501) staff       (20)      850 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/alignment/Makefile
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     1483 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/alignment/affine2p_penalties.c
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     2317 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/alignment/affine2p_penalties.h
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     1482 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/alignment/affine_penalties.c
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     2043 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/alignment/affine_penalties.h
+-rw-rw-r--   0 kezcleal   (501) staff       (20)    15257 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/alignment/cigar.c
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     3882 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/alignment/cigar.h
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     1767 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/alignment/linear_penalties.h
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     3714 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/alignment/score_matrix.c
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     2277 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/alignment/score_matrix.h
+drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-05-24 10:16:58.499714 pywfa-0.4.2/pywfa/WFA2_lib/build/
+-rw-r--r--   0 kezcleal   (501) staff       (20)      680 2023-05-24 10:16:50.000000 pywfa-0.4.2/pywfa/WFA2_lib/build/affine2p_penalties.o
+-rw-r--r--   0 kezcleal   (501) staff       (20)      680 2023-05-24 10:16:50.000000 pywfa-0.4.2/pywfa/WFA2_lib/build/affine_penalties.o
+-rw-r--r--   0 kezcleal   (501) staff       (20)     7348 2023-05-24 10:16:51.000000 pywfa-0.4.2/pywfa/WFA2_lib/build/bitmap.o
+-rw-r--r--   0 kezcleal   (501) staff       (20)    31884 2023-05-24 10:16:50.000000 pywfa-0.4.2/pywfa/WFA2_lib/build/cigar.o
+-rw-r--r--   0 kezcleal   (501) staff       (20)     4344 2023-05-24 10:16:52.000000 pywfa-0.4.2/pywfa/WFA2_lib/build/commons.o
+-rw-r--r--   0 kezcleal   (501) staff       (20)     2456 2023-05-24 10:16:52.000000 pywfa-0.4.2/pywfa/WFA2_lib/build/dna_text.o
+-rw-r--r--   0 kezcleal   (501) staff       (20)    10732 2023-05-24 10:16:52.000000 pywfa-0.4.2/pywfa/WFA2_lib/build/heatmap.o
+-rw-r--r--   0 kezcleal   (501) staff       (20)    35580 2023-05-24 10:16:51.000000 pywfa-0.4.2/pywfa/WFA2_lib/build/mm_allocator.o
+-rw-r--r--   0 kezcleal   (501) staff       (20)    15460 2023-05-24 10:16:51.000000 pywfa-0.4.2/pywfa/WFA2_lib/build/mm_stack.o
+-rw-r--r--   0 kezcleal   (501) staff       (20)    21188 2023-05-24 10:16:51.000000 pywfa-0.4.2/pywfa/WFA2_lib/build/profiler_counter.o
+-rw-r--r--   0 kezcleal   (501) staff       (20)    20956 2023-05-24 10:16:51.000000 pywfa-0.4.2/pywfa/WFA2_lib/build/profiler_timer.o
+-rw-r--r--   0 kezcleal   (501) staff       (20)    10220 2023-05-24 10:16:51.000000 pywfa-0.4.2/pywfa/WFA2_lib/build/score_matrix.o
+-rw-r--r--   0 kezcleal   (501) staff       (20)     8124 2023-05-24 10:16:52.000000 pywfa-0.4.2/pywfa/WFA2_lib/build/sequence_buffer.o
+-rw-r--r--   0 kezcleal   (501) staff       (20)    13868 2023-05-24 10:16:52.000000 pywfa-0.4.2/pywfa/WFA2_lib/build/string_padded.o
+-rw-r--r--   0 kezcleal   (501) staff       (20)     8104 2023-05-24 10:16:52.000000 pywfa-0.4.2/pywfa/WFA2_lib/build/vector.o
+-rw-r--r--   0 kezcleal   (501) staff       (20)     9204 2023-05-24 10:16:57.000000 pywfa-0.4.2/pywfa/WFA2_lib/build/wavefront.o
+-rw-r--r--   0 kezcleal   (501) staff       (20)    34440 2023-05-24 10:16:52.000000 pywfa-0.4.2/pywfa/WFA2_lib/build/wavefront_align.o
+-rw-r--r--   0 kezcleal   (501) staff       (20)    38040 2023-05-24 10:16:52.000000 pywfa-0.4.2/pywfa/WFA2_lib/build/wavefront_aligner.o
+-rw-r--r--   0 kezcleal   (501) staff       (20)     6988 2023-05-24 10:16:53.000000 pywfa-0.4.2/pywfa/WFA2_lib/build/wavefront_attributes.o
+-rw-r--r--   0 kezcleal   (501) staff       (20)    41816 2023-05-24 10:16:53.000000 pywfa-0.4.2/pywfa/WFA2_lib/build/wavefront_backtrace.o
+-rw-r--r--   0 kezcleal   (501) staff       (20)    29876 2023-05-24 10:16:53.000000 pywfa-0.4.2/pywfa/WFA2_lib/build/wavefront_backtrace_buffer.o
+-rw-r--r--   0 kezcleal   (501) staff       (20)    28184 2023-05-24 10:16:53.000000 pywfa-0.4.2/pywfa/WFA2_lib/build/wavefront_backtrace_offload.o
+-rw-r--r--   0 kezcleal   (501) staff       (20)    41248 2023-05-24 10:16:53.000000 pywfa-0.4.2/pywfa/WFA2_lib/build/wavefront_bialign.o
+-rw-r--r--   0 kezcleal   (501) staff       (20)    37060 2023-05-24 10:16:54.000000 pywfa-0.4.2/pywfa/WFA2_lib/build/wavefront_components.o
+-rw-r--r--   0 kezcleal   (501) staff       (20)    39996 2023-05-24 10:16:55.000000 pywfa-0.4.2/pywfa/WFA2_lib/build/wavefront_compute.o
+-rw-r--r--   0 kezcleal   (501) staff       (20)    26904 2023-05-24 10:16:55.000000 pywfa-0.4.2/pywfa/WFA2_lib/build/wavefront_compute_affine.o
+-rw-r--r--   0 kezcleal   (501) staff       (20)    32276 2023-05-24 10:16:55.000000 pywfa-0.4.2/pywfa/WFA2_lib/build/wavefront_compute_affine2p.o
+-rw-r--r--   0 kezcleal   (501) staff       (20)    42120 2023-05-24 10:16:55.000000 pywfa-0.4.2/pywfa/WFA2_lib/build/wavefront_compute_edit.o
+-rw-r--r--   0 kezcleal   (501) staff       (20)    25536 2023-05-24 10:16:55.000000 pywfa-0.4.2/pywfa/WFA2_lib/build/wavefront_compute_linear.o
+-rw-r--r--   0 kezcleal   (501) staff       (20)    23780 2023-05-24 10:16:56.000000 pywfa-0.4.2/pywfa/WFA2_lib/build/wavefront_debug.o
+-rw-r--r--   0 kezcleal   (501) staff       (20)    34280 2023-05-24 10:16:56.000000 pywfa-0.4.2/pywfa/WFA2_lib/build/wavefront_display.o
+-rw-r--r--   0 kezcleal   (501) staff       (20)    28068 2023-05-24 10:16:56.000000 pywfa-0.4.2/pywfa/WFA2_lib/build/wavefront_extend.o
+-rw-r--r--   0 kezcleal   (501) staff       (20)    41060 2023-05-24 10:16:56.000000 pywfa-0.4.2/pywfa/WFA2_lib/build/wavefront_heuristic.o
+-rw-r--r--   0 kezcleal   (501) staff       (20)    21688 2023-05-24 10:16:56.000000 pywfa-0.4.2/pywfa/WFA2_lib/build/wavefront_pcigar.o
+-rw-r--r--   0 kezcleal   (501) staff       (20)     9172 2023-05-24 10:16:57.000000 pywfa-0.4.2/pywfa/WFA2_lib/build/wavefront_penalties.o
+-rw-r--r--   0 kezcleal   (501) staff       (20)    27092 2023-05-24 10:16:57.000000 pywfa-0.4.2/pywfa/WFA2_lib/build/wavefront_plot.o
+-rw-r--r--   0 kezcleal   (501) staff       (20)    17492 2023-05-24 10:16:57.000000 pywfa-0.4.2/pywfa/WFA2_lib/build/wavefront_slab.o
+drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-05-24 10:16:58.581812 pywfa-0.4.2/pywfa/WFA2_lib/examples/
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     1156 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/examples/Makefile
+-rw-rw-r--   0 kezcleal   (501) staff       (20)      693 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/examples/README.md
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     2992 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/examples/wfa_adapt.c
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     2661 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/examples/wfa_basic.c
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     2143 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/examples/wfa_bindings.cpp
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     2521 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/examples/wfa_lambda.cpp
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     2533 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/examples/wfa_repeated.c
+drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-05-24 10:16:59.850767 pywfa-0.4.2/pywfa/WFA2_lib/img/
+-rw-rw-r--   0 kezcleal   (501) staff       (20)   351138 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/img/heuristics.aband.10.10.png
+-rw-rw-r--   0 kezcleal   (501) staff       (20)   395217 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/img/heuristics.aband.50.50.png
+-rw-rw-r--   0 kezcleal   (501) staff       (20)   358048 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/img/heuristics.band.10.10.png
+-rw-rw-r--   0 kezcleal   (501) staff       (20)   423890 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/img/heuristics.band.10.150.png
+-rw-rw-r--   0 kezcleal   (501) staff       (20)   502376 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/img/heuristics.none.png
+-rw-rw-r--   0 kezcleal   (501) staff       (20)   394728 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/img/heuristics.wfadap.10.50.1.png
+-rw-rw-r--   0 kezcleal   (501) staff       (20)   502078 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/img/heuristics.wfadap.10.50.10.png
+-rw-rw-r--   0 kezcleal   (501) staff       (20)   907275 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/img/wfa.vs.swg.png
+drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-05-24 10:17:00.060493 pywfa-0.4.2/pywfa/WFA2_lib/lib/
+-rw-r--r--   0 kezcleal   (501) staff       (20)   844160 2023-05-24 10:16:57.000000 pywfa-0.4.2/pywfa/WFA2_lib/lib/libwfa.a
+drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-05-24 10:17:00.112348 pywfa-0.4.2/pywfa/WFA2_lib/scripts/
+-rwxr-xr-x   0 kezcleal   (501) staff       (20)      390 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/scripts/fasta2seq.sh
+-rwxr-xr-x   0 kezcleal   (501) staff       (20)      442 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/scripts/seq2fasta.sh
+-rw-rw-r--   0 kezcleal   (501) staff       (20)    10228 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/scripts/wfa.alg.cmp.py
+-rw-rw-r--   0 kezcleal   (501) staff       (20)      393 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/scripts/wfa.alg.cmp.score.sh
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     6423 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/scripts/wfa.alg.rescore.py
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     9646 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/scripts/wfa2png.py
+drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-05-24 10:17:00.117120 pywfa-0.4.2/pywfa/WFA2_lib/system/
+-rw-rw-r--   0 kezcleal   (501) staff       (20)      838 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/system/Makefile
+-rw-rw-r--   0 kezcleal   (501) staff       (20)    22734 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/system/mm_allocator.c
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     4837 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/system/mm_allocator.h
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     9143 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/system/mm_stack.c
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     3510 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/system/mm_stack.h
+-rw-rw-r--   0 kezcleal   (501) staff       (20)    10898 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/system/profiler_counter.c
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     4634 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/system/profiler_counter.h
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     7247 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/system/profiler_timer.c
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     3937 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/system/profiler_timer.h
+drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-05-24 10:17:00.140074 pywfa-0.4.2/pywfa/WFA2_lib/tools/
+-rw-r--r--   0 kezcleal   (501) staff       (20)     6148 2022-07-15 09:13:52.000000 pywfa-0.4.2/pywfa/WFA2_lib/tools/.DS_Store
+-rw-rw-r--   0 kezcleal   (501) staff       (20)    12243 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/tools/README.md
+drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-05-24 10:17:00.165495 pywfa-0.4.2/pywfa/WFA2_lib/utils/
+-rw-rw-r--   0 kezcleal   (501) staff       (20)      884 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/utils/Makefile
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     4480 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/utils/bitmap.c
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     3033 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/utils/bitmap.h
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     2386 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/utils/commons.c
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     8785 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/utils/commons.h
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     2043 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/utils/dna_text.c
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     2276 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/utils/dna_text.h
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     5201 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/utils/heatmap.c
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     2402 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/utils/heatmap.h
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     5325 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/utils/sequence_buffer.c
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     2506 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/utils/sequence_buffer.h
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     5499 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/utils/string_padded.c
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     2560 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/utils/string_padded.h
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     4305 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/utils/vector.c
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     5011 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/utils/vector.h
+drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-05-24 10:17:00.184882 pywfa-0.4.2/pywfa/WFA2_lib/wavefront/
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     1520 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/wavefront/Makefile
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     6046 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront.c
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     4814 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront.h
+-rw-rw-r--   0 kezcleal   (501) staff       (20)    20093 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_align.c
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     2192 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_align.h
+-rw-rw-r--   0 kezcleal   (501) staff       (20)    18740 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_aligner.c
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     8290 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_aligner.h
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     3584 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_attributes.c
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     6499 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_attributes.h
+-rw-rw-r--   0 kezcleal   (501) staff       (20)    20606 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_backtrace.c
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     2334 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_backtrace.h
+-rw-rw-r--   0 kezcleal   (501) staff       (20)    20399 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_backtrace_buffer.c
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     6138 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_backtrace_buffer.h
+-rw-rw-r--   0 kezcleal   (501) staff       (20)    12970 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_backtrace_offload.c
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     2538 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_backtrace_offload.h
+-rw-rw-r--   0 kezcleal   (501) staff       (20)    21142 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_bialign.c
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     2719 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_bialign.h
+-rw-rw-r--   0 kezcleal   (501) staff       (20)    19200 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_components.c
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     4128 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_components.h
+-rw-rw-r--   0 kezcleal   (501) staff       (20)    19880 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_compute.c
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     3164 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_compute.h
+-rw-rw-r--   0 kezcleal   (501) staff       (20)    10059 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_compute_affine.c
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     2132 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_compute_affine.h
+-rw-rw-r--   0 kezcleal   (501) staff       (20)    14496 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_compute_affine2p.c
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     1783 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_compute_affine2p.h
+-rw-rw-r--   0 kezcleal   (501) staff       (20)    13902 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_compute_edit.c
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     1755 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_compute_edit.h
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     7207 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_compute_linear.c
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     1769 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_compute_linear.h
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     9318 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_debug.c
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     1765 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_debug.h
+-rw-rw-r--   0 kezcleal   (501) staff       (20)    10578 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_display.c
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     1911 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_display.h
+-rw-rw-r--   0 kezcleal   (501) staff       (20)    18252 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_extend.c
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     2029 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_extend.h
+-rw-rw-r--   0 kezcleal   (501) staff       (20)    22178 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_heuristic.c
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     4380 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_heuristic.h
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     2312 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_offset.h
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     8949 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_pcigar.c
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     4335 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_pcigar.h
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     8443 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_penalties.c
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     4011 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_penalties.h
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     9696 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_plot.c
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     2765 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_plot.h
+-rw-rw-r--   0 kezcleal   (501) staff       (20)    11285 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_slab.c
+-rw-rw-r--   0 kezcleal   (501) staff       (20)     3361 2022-07-06 18:32:49.000000 pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_slab.h
+-rw-r--r--   0 kezcleal   (501) staff       (20)   109797 2022-03-14 10:43:36.000000 pywfa-0.4.2/pywfa/WFA_wrap.c
+-rw-r--r--   0 kezcleal   (501) staff       (20)    23033 2022-03-17 21:23:24.000000 pywfa-0.4.2/pywfa/WFA_wrap.pxd
+-rw-r--r--   0 kezcleal   (501) staff       (20)      131 2023-05-24 10:14:49.000000 pywfa-0.4.2/pywfa/__init__.py
+-rw-r--r--   0 kezcleal   (501) staff       (20)   659018 2023-05-24 10:16:49.000000 pywfa-0.4.2/pywfa/align.c
+-rwxr-xr-x   0 kezcleal   (501) staff       (20)   596077 2023-05-24 10:16:58.000000 pywfa-0.4.2/pywfa/align.cpython-310-darwin.so
+-rwxr-xr-x   0 kezcleal   (501) staff       (20)   340288 2023-05-24 10:16:58.000000 pywfa-0.4.2/pywfa/align.cpython-39-darwin.so
+-rw-r--r--   0 kezcleal   (501) staff       (20)      369 2022-03-17 21:21:36.000000 pywfa-0.4.2/pywfa/align.pxd
+-rw-r--r--   0 kezcleal   (501) staff       (20)    20736 2023-01-05 12:11:20.000000 pywfa-0.4.2/pywfa/align.pyx
+drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-05-24 10:17:00.383207 pywfa-0.4.2/pywfa/tests/
+-rw-r--r--   0 kezcleal   (501) staff       (20)        0 2022-03-13 11:24:44.000000 pywfa-0.4.2/pywfa/tests/__init__.py
+-rw-r--r--   0 kezcleal   (501) staff       (20)      727 2022-03-15 08:50:50.000000 pywfa-0.4.2/pywfa/tests/long.fa
+-rw-r--r--   0 kezcleal   (501) staff       (20)     2214 2022-03-15 08:59:45.000000 pywfa-0.4.2/pywfa/tests/long.reference.fa
+-rw-r--r--   0 kezcleal   (501) staff       (20)     1133 2022-03-16 11:51:32.000000 pywfa-0.4.2/pywfa/tests/short.fa
+-rw-r--r--   0 kezcleal   (501) staff       (20)     4797 2022-03-16 11:50:49.000000 pywfa-0.4.2/pywfa/tests/short.reference.fa
+-rw-r--r--   0 kezcleal   (501) staff       (20)     9054 2023-01-05 11:11:42.000000 pywfa-0.4.2/pywfa/tests/test.py
+drwxr-xr-x   0 kezcleal   (501) staff       (20)        0 2023-05-24 10:16:58.477733 pywfa-0.4.2/pywfa.egg-info/
+-rw-r--r--   0 kezcleal   (501) staff       (20)     6892 2023-05-24 10:16:58.000000 pywfa-0.4.2/pywfa.egg-info/PKG-INFO
+-rw-r--r--   0 kezcleal   (501) staff       (20)     6265 2023-05-24 10:16:58.000000 pywfa-0.4.2/pywfa.egg-info/SOURCES.txt
+-rw-r--r--   0 kezcleal   (501) staff       (20)        1 2023-05-24 10:16:58.000000 pywfa-0.4.2/pywfa.egg-info/dependency_links.txt
+-rw-r--r--   0 kezcleal   (501) staff       (20)       20 2023-05-24 10:16:58.000000 pywfa-0.4.2/pywfa.egg-info/top_level.txt
+-rw-r--r--   0 kezcleal   (501) staff       (20)       38 2023-05-24 10:17:00.434908 pywfa-0.4.2/setup.cfg
```

### Comparing `pywfa-0.4.1/LICENSE.md` & `pywfa-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/README.rst` & `pywfa-0.4.2/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -8,28 +8,32 @@
 Installation
 ------------
 
 To download from pypi::
 
     pip install pywfa
 
+From conda::
+
+    conda install -c bioconda pywfa
+
 Build from source::
 
     git clone https://github.com/kcleal/pywfa
     cd pywfa
     pip install .
 
 Overview
 --------
 
 Alignment of pattern and text strings can be performed by accessing WFA2-lib functions directly:
 
 .. code-block:: python
 
-    from pywfa.align import WavefrontAligner
+    from pywfa import WavefrontAligner
 
     pattern = "TCTTTACTCGCGCGTTGGAGAAATACAATAGT"
     text =    "TCTATACTGCGCGTTTGGAGAAATAAAATAGT"
     a = WavefrontAligner(pattern)
     score = a.wavefront_align(text)
     assert a.status == 0  # alignment was successful
     assert a.cigarstring == "3M1X4M1D7M1I9M1X6M"
@@ -84,15 +88,16 @@
 For convenience, a results object can be obtained by calling the `WavefrontAligner` with a pattern and text:
 
 .. code-block:: python
 
     pattern = "TCTTTACTCGCGCGTTGGAGAAATACAATAGT"
     text =    "TCTATACTGCGCGTTTGGAGAAATAAAATAGT"
     a = WavefrontAligner(pattern)
-    a(text)
+    result = a(text)  # alignment result
+    result.__dict__
     >>> {'pattern_length': 32, 'text_length': 32, 'pattern_start': 0, 'pattern_end': 32, 'text_start': 0, 'text_end': 32, 'cigartuples': [(0, 3), (8, 1), (0, 4), (2, 1), (0, 7), (1, 1), (0, 9), (8, 1), (0, 6)], 'score': -24, 'pattern': 'TCTTTACTCGCGCGTTGGAGAAATACAATAGT', 'text': 'TCTATACTGCGCGTTTGGAGAAATAAAATAGT', 'status': 0}
 
     # Alignment can also be called with a pattern like this:
     a(text, pattern)
 
     # obtain a string in the same format as cigar_print_pretty
     a.pretty
@@ -106,15 +111,15 @@
 Configure
 ---------
 To configure the `WaveFrontAligner`, options can be provided during initialization:
 
 
 .. code-block:: python
 
-    from pywfa.align import WavefrontAligner
+    from pywfa import WavefrontAligner
 
     a = WavefrontAligner(scope="score",
                          distance="affine2p",
                          span="end-to-end",
                          heuristic="adaptive")
 
 Supported distance metrics are "affine" (default) and "affine2p". Scope can be "full" (default)
```

### Comparing `pywfa-0.4.1/pywfa/.DS_Store` & `pywfa-0.4.2/pywfa/.DS_Store`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/alignment/Makefile` & `pywfa-0.4.2/pywfa/WFA2_lib/alignment/Makefile`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/alignment/affine2p_penalties.c` & `pywfa-0.4.2/pywfa/WFA2_lib/alignment/affine2p_penalties.c`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/alignment/affine2p_penalties.h` & `pywfa-0.4.2/pywfa/WFA2_lib/alignment/affine2p_penalties.h`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/alignment/affine_penalties.c` & `pywfa-0.4.2/pywfa/WFA2_lib/alignment/affine_penalties.c`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/alignment/affine_penalties.h` & `pywfa-0.4.2/pywfa/WFA2_lib/alignment/affine_penalties.h`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/alignment/cigar.c` & `pywfa-0.4.2/pywfa/WFA2_lib/alignment/cigar.c`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/alignment/cigar.h` & `pywfa-0.4.2/pywfa/WFA2_lib/alignment/cigar.h`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/alignment/linear_penalties.h` & `pywfa-0.4.2/pywfa/WFA2_lib/alignment/linear_penalties.h`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/alignment/score_matrix.c` & `pywfa-0.4.2/pywfa/WFA2_lib/alignment/score_matrix.c`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/alignment/score_matrix.h` & `pywfa-0.4.2/pywfa/WFA2_lib/alignment/score_matrix.h`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/build/affine2p_penalties.o` & `pywfa-0.4.2/pywfa/WFA2_lib/build/affine2p_penalties.o`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/build/affine_penalties.o` & `pywfa-0.4.2/pywfa/WFA2_lib/build/affine_penalties.o`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/build/bitmap.o` & `pywfa-0.4.2/pywfa/WFA2_lib/build/bitmap.o`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/build/cigar.o` & `pywfa-0.4.2/pywfa/WFA2_lib/build/cigar.o`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/build/commons.o` & `pywfa-0.4.2/pywfa/WFA2_lib/build/commons.o`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/build/dna_text.o` & `pywfa-0.4.2/pywfa/WFA2_lib/build/dna_text.o`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/build/heatmap.o` & `pywfa-0.4.2/pywfa/WFA2_lib/build/heatmap.o`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/build/mm_allocator.o` & `pywfa-0.4.2/pywfa/WFA2_lib/build/mm_allocator.o`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/build/mm_stack.o` & `pywfa-0.4.2/pywfa/WFA2_lib/build/mm_stack.o`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/build/profiler_counter.o` & `pywfa-0.4.2/pywfa/WFA2_lib/build/profiler_counter.o`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/build/profiler_timer.o` & `pywfa-0.4.2/pywfa/WFA2_lib/build/profiler_timer.o`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/build/score_matrix.o` & `pywfa-0.4.2/pywfa/WFA2_lib/build/score_matrix.o`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/build/sequence_buffer.o` & `pywfa-0.4.2/pywfa/WFA2_lib/build/sequence_buffer.o`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/build/string_padded.o` & `pywfa-0.4.2/pywfa/WFA2_lib/build/string_padded.o`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/build/vector.o` & `pywfa-0.4.2/pywfa/WFA2_lib/build/vector.o`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/build/wavefront.o` & `pywfa-0.4.2/pywfa/WFA2_lib/build/wavefront.o`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/build/wavefront_align.o` & `pywfa-0.4.2/pywfa/WFA2_lib/build/wavefront_align.o`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/build/wavefront_aligner.o` & `pywfa-0.4.2/pywfa/WFA2_lib/build/wavefront_aligner.o`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/build/wavefront_attributes.o` & `pywfa-0.4.2/pywfa/WFA2_lib/build/wavefront_attributes.o`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/build/wavefront_backtrace.o` & `pywfa-0.4.2/pywfa/WFA2_lib/build/wavefront_backtrace.o`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/build/wavefront_backtrace_buffer.o` & `pywfa-0.4.2/pywfa/WFA2_lib/build/wavefront_backtrace_buffer.o`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/build/wavefront_backtrace_offload.o` & `pywfa-0.4.2/pywfa/WFA2_lib/build/wavefront_backtrace_offload.o`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/build/wavefront_bialign.o` & `pywfa-0.4.2/pywfa/WFA2_lib/build/wavefront_bialign.o`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/build/wavefront_components.o` & `pywfa-0.4.2/pywfa/WFA2_lib/build/wavefront_components.o`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/build/wavefront_compute.o` & `pywfa-0.4.2/pywfa/WFA2_lib/build/wavefront_compute.o`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/build/wavefront_compute_affine.o` & `pywfa-0.4.2/pywfa/WFA2_lib/build/wavefront_compute_affine.o`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/build/wavefront_compute_affine2p.o` & `pywfa-0.4.2/pywfa/WFA2_lib/build/wavefront_compute_affine2p.o`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/build/wavefront_compute_edit.o` & `pywfa-0.4.2/pywfa/WFA2_lib/build/wavefront_compute_edit.o`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/build/wavefront_compute_linear.o` & `pywfa-0.4.2/pywfa/WFA2_lib/build/wavefront_compute_linear.o`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/build/wavefront_debug.o` & `pywfa-0.4.2/pywfa/WFA2_lib/build/wavefront_debug.o`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/build/wavefront_display.o` & `pywfa-0.4.2/pywfa/WFA2_lib/build/wavefront_display.o`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/build/wavefront_extend.o` & `pywfa-0.4.2/pywfa/WFA2_lib/build/wavefront_extend.o`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/build/wavefront_heuristic.o` & `pywfa-0.4.2/pywfa/WFA2_lib/build/wavefront_heuristic.o`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/build/wavefront_pcigar.o` & `pywfa-0.4.2/pywfa/WFA2_lib/build/wavefront_pcigar.o`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/build/wavefront_penalties.o` & `pywfa-0.4.2/pywfa/WFA2_lib/build/wavefront_penalties.o`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/build/wavefront_plot.o` & `pywfa-0.4.2/pywfa/WFA2_lib/build/wavefront_plot.o`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/build/wavefront_slab.o` & `pywfa-0.4.2/pywfa/WFA2_lib/build/wavefront_slab.o`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/examples/Makefile` & `pywfa-0.4.2/pywfa/WFA2_lib/examples/Makefile`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/examples/README.md` & `pywfa-0.4.2/pywfa/WFA2_lib/examples/README.md`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/examples/wfa_adapt.c` & `pywfa-0.4.2/pywfa/WFA2_lib/examples/wfa_adapt.c`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/examples/wfa_basic.c` & `pywfa-0.4.2/pywfa/WFA2_lib/examples/wfa_basic.c`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/examples/wfa_bindings.cpp` & `pywfa-0.4.2/pywfa/WFA2_lib/examples/wfa_bindings.cpp`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/examples/wfa_lambda.cpp` & `pywfa-0.4.2/pywfa/WFA2_lib/examples/wfa_lambda.cpp`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/examples/wfa_repeated.c` & `pywfa-0.4.2/pywfa/WFA2_lib/examples/wfa_repeated.c`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/img/heuristics.aband.10.10.png` & `pywfa-0.4.2/pywfa/WFA2_lib/img/heuristics.aband.10.10.png`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/img/heuristics.aband.50.50.png` & `pywfa-0.4.2/pywfa/WFA2_lib/img/heuristics.aband.50.50.png`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/img/heuristics.band.10.10.png` & `pywfa-0.4.2/pywfa/WFA2_lib/img/heuristics.band.10.10.png`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/img/heuristics.band.10.150.png` & `pywfa-0.4.2/pywfa/WFA2_lib/img/heuristics.band.10.150.png`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/img/heuristics.none.png` & `pywfa-0.4.2/pywfa/WFA2_lib/img/heuristics.none.png`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/img/heuristics.wfadap.10.50.1.png` & `pywfa-0.4.2/pywfa/WFA2_lib/img/heuristics.wfadap.10.50.1.png`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/img/heuristics.wfadap.10.50.10.png` & `pywfa-0.4.2/pywfa/WFA2_lib/img/heuristics.wfadap.10.50.10.png`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/img/wfa.vs.swg.png` & `pywfa-0.4.2/pywfa/WFA2_lib/img/wfa.vs.swg.png`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/lib/libwfa.a` & `pywfa-0.4.2/pywfa/WFA2_lib/lib/libwfa.a`

 * *Files 0% similar despite different names*

#### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0      501       20    12880 2023-03-01 22:02:42.000000 __.SYMDEF SORTED
--rw-r--r--   0      501       20      680 2023-03-01 22:02:23.000000 affine2p_penalties.o
--rw-r--r--   0      501       20      680 2023-03-01 22:02:23.000000 affine_penalties.o
--rw-r--r--   0      501       20     7352 2023-03-01 22:02:28.000000 bitmap.o
--rw-r--r--   0      501       20    31888 2023-03-01 22:02:26.000000 cigar.o
--rw-r--r--   0      501       20     4344 2023-03-01 22:02:28.000000 commons.o
--rw-r--r--   0      501       20     2456 2023-03-01 22:02:28.000000 dna_text.o
--rw-r--r--   0      501       20    10736 2023-03-01 22:02:28.000000 heatmap.o
--rw-r--r--   0      501       20    35584 2023-03-01 22:02:26.000000 mm_allocator.o
--rw-r--r--   0      501       20    15464 2023-03-01 22:02:26.000000 mm_stack.o
--rw-r--r--   0      501       20    21192 2023-03-01 22:02:26.000000 profiler_counter.o
--rw-r--r--   0      501       20    20960 2023-03-01 22:02:28.000000 profiler_timer.o
--rw-r--r--   0      501       20    10224 2023-03-01 22:02:26.000000 score_matrix.o
--rw-r--r--   0      501       20     8128 2023-03-01 22:02:28.000000 sequence_buffer.o
--rw-r--r--   0      501       20    13872 2023-03-01 22:02:28.000000 string_padded.o
--rw-r--r--   0      501       20     8104 2023-03-01 22:02:29.000000 vector.o
--rw-r--r--   0      501       20     9208 2023-03-01 22:02:33.000000 wavefront.o
--rw-r--r--   0      501       20    34440 2023-03-01 22:02:29.000000 wavefront_align.o
--rw-r--r--   0      501       20    38040 2023-03-01 22:02:30.000000 wavefront_aligner.o
--rw-r--r--   0      501       20     6992 2023-03-01 22:02:30.000000 wavefront_attributes.o
--rw-r--r--   0      501       20    41816 2023-03-01 22:02:30.000000 wavefront_backtrace.o
--rw-r--r--   0      501       20    29880 2023-03-01 22:02:30.000000 wavefront_backtrace_buffer.o
--rw-r--r--   0      501       20    28184 2023-03-01 22:02:30.000000 wavefront_backtrace_offload.o
--rw-r--r--   0      501       20    41248 2023-03-01 22:02:30.000000 wavefront_bialign.o
--rw-r--r--   0      501       20    37064 2023-03-01 22:02:30.000000 wavefront_components.o
--rw-r--r--   0      501       20    40000 2023-03-01 22:02:32.000000 wavefront_compute.o
--rw-r--r--   0      501       20    26904 2023-03-01 22:02:31.000000 wavefront_compute_affine.o
--rw-r--r--   0      501       20    32280 2023-03-01 22:02:31.000000 wavefront_compute_affine2p.o
--rw-r--r--   0      501       20    42120 2023-03-01 22:02:31.000000 wavefront_compute_edit.o
--rw-r--r--   0      501       20    25536 2023-03-01 22:02:31.000000 wavefront_compute_linear.o
--rw-r--r--   0      501       20    23784 2023-03-01 22:02:32.000000 wavefront_debug.o
--rw-r--r--   0      501       20    34280 2023-03-01 22:02:32.000000 wavefront_display.o
--rw-r--r--   0      501       20    28072 2023-03-01 22:02:32.000000 wavefront_extend.o
--rw-r--r--   0      501       20    41064 2023-03-01 22:02:32.000000 wavefront_heuristic.o
--rw-r--r--   0      501       20    21688 2023-03-01 22:02:32.000000 wavefront_pcigar.o
--rw-r--r--   0      501       20     9176 2023-03-01 22:02:32.000000 wavefront_penalties.o
--rw-r--r--   0      501       20    27096 2023-03-01 22:02:33.000000 wavefront_plot.o
--rw-r--r--   0      501       20    17496 2023-03-01 22:02:33.000000 wavefront_slab.o
+-rw-r--r--   0      501       20    12880 2023-05-24 10:17:02.000000 __.SYMDEF SORTED
+-rw-r--r--   0      501       20      680 2023-05-24 10:16:50.000000 affine2p_penalties.o
+-rw-r--r--   0      501       20      680 2023-05-24 10:16:50.000000 affine_penalties.o
+-rw-r--r--   0      501       20     7352 2023-05-24 10:16:51.000000 bitmap.o
+-rw-r--r--   0      501       20    31888 2023-05-24 10:16:50.000000 cigar.o
+-rw-r--r--   0      501       20     4344 2023-05-24 10:16:52.000000 commons.o
+-rw-r--r--   0      501       20     2456 2023-05-24 10:16:52.000000 dna_text.o
+-rw-r--r--   0      501       20    10736 2023-05-24 10:16:52.000000 heatmap.o
+-rw-r--r--   0      501       20    35584 2023-05-24 10:16:51.000000 mm_allocator.o
+-rw-r--r--   0      501       20    15464 2023-05-24 10:16:51.000000 mm_stack.o
+-rw-r--r--   0      501       20    21192 2023-05-24 10:16:51.000000 profiler_counter.o
+-rw-r--r--   0      501       20    20960 2023-05-24 10:16:51.000000 profiler_timer.o
+-rw-r--r--   0      501       20    10224 2023-05-24 10:16:51.000000 score_matrix.o
+-rw-r--r--   0      501       20     8128 2023-05-24 10:16:52.000000 sequence_buffer.o
+-rw-r--r--   0      501       20    13872 2023-05-24 10:16:52.000000 string_padded.o
+-rw-r--r--   0      501       20     8104 2023-05-24 10:16:52.000000 vector.o
+-rw-r--r--   0      501       20     9208 2023-05-24 10:16:57.000000 wavefront.o
+-rw-r--r--   0      501       20    34440 2023-05-24 10:16:52.000000 wavefront_align.o
+-rw-r--r--   0      501       20    38040 2023-05-24 10:16:52.000000 wavefront_aligner.o
+-rw-r--r--   0      501       20     6992 2023-05-24 10:16:53.000000 wavefront_attributes.o
+-rw-r--r--   0      501       20    41816 2023-05-24 10:16:53.000000 wavefront_backtrace.o
+-rw-r--r--   0      501       20    29880 2023-05-24 10:16:53.000000 wavefront_backtrace_buffer.o
+-rw-r--r--   0      501       20    28184 2023-05-24 10:16:53.000000 wavefront_backtrace_offload.o
+-rw-r--r--   0      501       20    41248 2023-05-24 10:16:53.000000 wavefront_bialign.o
+-rw-r--r--   0      501       20    37064 2023-05-24 10:16:54.000000 wavefront_components.o
+-rw-r--r--   0      501       20    40000 2023-05-24 10:16:55.000000 wavefront_compute.o
+-rw-r--r--   0      501       20    26904 2023-05-24 10:16:55.000000 wavefront_compute_affine.o
+-rw-r--r--   0      501       20    32280 2023-05-24 10:16:55.000000 wavefront_compute_affine2p.o
+-rw-r--r--   0      501       20    42120 2023-05-24 10:16:55.000000 wavefront_compute_edit.o
+-rw-r--r--   0      501       20    25536 2023-05-24 10:16:55.000000 wavefront_compute_linear.o
+-rw-r--r--   0      501       20    23784 2023-05-24 10:16:56.000000 wavefront_debug.o
+-rw-r--r--   0      501       20    34280 2023-05-24 10:16:56.000000 wavefront_display.o
+-rw-r--r--   0      501       20    28072 2023-05-24 10:16:56.000000 wavefront_extend.o
+-rw-r--r--   0      501       20    41064 2023-05-24 10:16:56.000000 wavefront_heuristic.o
+-rw-r--r--   0      501       20    21688 2023-05-24 10:16:56.000000 wavefront_pcigar.o
+-rw-r--r--   0      501       20     9176 2023-05-24 10:16:57.000000 wavefront_penalties.o
+-rw-r--r--   0      501       20    27096 2023-05-24 10:16:57.000000 wavefront_plot.o
+-rw-r--r--   0      501       20    17496 2023-05-24 10:16:57.000000 wavefront_slab.o
```

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/scripts/wfa.alg.cmp.py` & `pywfa-0.4.2/pywfa/WFA2_lib/scripts/wfa.alg.cmp.py`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/scripts/wfa.alg.rescore.py` & `pywfa-0.4.2/pywfa/WFA2_lib/scripts/wfa.alg.rescore.py`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/scripts/wfa2png.py` & `pywfa-0.4.2/pywfa/WFA2_lib/scripts/wfa2png.py`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/system/Makefile` & `pywfa-0.4.2/pywfa/WFA2_lib/system/Makefile`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/system/mm_allocator.c` & `pywfa-0.4.2/pywfa/WFA2_lib/system/mm_allocator.c`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/system/mm_allocator.h` & `pywfa-0.4.2/pywfa/WFA2_lib/system/mm_allocator.h`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/system/mm_stack.c` & `pywfa-0.4.2/pywfa/WFA2_lib/system/mm_stack.c`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/system/mm_stack.h` & `pywfa-0.4.2/pywfa/WFA2_lib/system/mm_stack.h`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/system/profiler_counter.c` & `pywfa-0.4.2/pywfa/WFA2_lib/system/profiler_counter.c`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/system/profiler_counter.h` & `pywfa-0.4.2/pywfa/WFA2_lib/system/profiler_counter.h`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/system/profiler_timer.c` & `pywfa-0.4.2/pywfa/WFA2_lib/system/profiler_timer.c`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/system/profiler_timer.h` & `pywfa-0.4.2/pywfa/WFA2_lib/system/profiler_timer.h`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/tools/.DS_Store` & `pywfa-0.4.2/pywfa/WFA2_lib/tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/tools/README.md` & `pywfa-0.4.2/pywfa/WFA2_lib/tools/README.md`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/utils/Makefile` & `pywfa-0.4.2/pywfa/WFA2_lib/utils/Makefile`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/utils/bitmap.c` & `pywfa-0.4.2/pywfa/WFA2_lib/utils/bitmap.c`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/utils/bitmap.h` & `pywfa-0.4.2/pywfa/WFA2_lib/utils/bitmap.h`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/utils/commons.c` & `pywfa-0.4.2/pywfa/WFA2_lib/utils/commons.c`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/utils/commons.h` & `pywfa-0.4.2/pywfa/WFA2_lib/utils/commons.h`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/utils/dna_text.c` & `pywfa-0.4.2/pywfa/WFA2_lib/utils/dna_text.c`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/utils/dna_text.h` & `pywfa-0.4.2/pywfa/WFA2_lib/utils/dna_text.h`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/utils/heatmap.c` & `pywfa-0.4.2/pywfa/WFA2_lib/utils/heatmap.c`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/utils/heatmap.h` & `pywfa-0.4.2/pywfa/WFA2_lib/utils/heatmap.h`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/utils/sequence_buffer.c` & `pywfa-0.4.2/pywfa/WFA2_lib/utils/sequence_buffer.c`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/utils/sequence_buffer.h` & `pywfa-0.4.2/pywfa/WFA2_lib/utils/sequence_buffer.h`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/utils/string_padded.c` & `pywfa-0.4.2/pywfa/WFA2_lib/utils/string_padded.c`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/utils/string_padded.h` & `pywfa-0.4.2/pywfa/WFA2_lib/utils/string_padded.h`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/utils/vector.c` & `pywfa-0.4.2/pywfa/WFA2_lib/utils/vector.c`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/utils/vector.h` & `pywfa-0.4.2/pywfa/WFA2_lib/utils/vector.h`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/wavefront/Makefile` & `pywfa-0.4.2/pywfa/WFA2_lib/wavefront/Makefile`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront.c` & `pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront.c`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront.h` & `pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront.h`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_align.c` & `pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_align.c`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_align.h` & `pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_align.h`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_aligner.c` & `pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_aligner.c`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_aligner.h` & `pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_aligner.h`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_attributes.c` & `pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_attributes.c`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_attributes.h` & `pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_attributes.h`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_backtrace.c` & `pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_backtrace.c`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_backtrace.h` & `pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_backtrace.h`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_backtrace_buffer.c` & `pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_backtrace_buffer.c`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_backtrace_buffer.h` & `pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_backtrace_buffer.h`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_backtrace_offload.c` & `pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_backtrace_offload.c`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_backtrace_offload.h` & `pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_backtrace_offload.h`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_bialign.c` & `pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_bialign.c`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_bialign.h` & `pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_bialign.h`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_components.c` & `pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_components.c`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_components.h` & `pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_components.h`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_compute.c` & `pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_compute.c`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_compute.h` & `pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_compute.h`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_compute_affine.c` & `pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_compute_affine.c`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_compute_affine.h` & `pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_compute_affine.h`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_compute_affine2p.c` & `pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_compute_affine2p.c`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_compute_affine2p.h` & `pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_compute_affine2p.h`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_compute_edit.c` & `pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_compute_edit.c`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_compute_edit.h` & `pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_compute_edit.h`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_compute_linear.c` & `pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_compute_linear.c`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_compute_linear.h` & `pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_compute_linear.h`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_debug.c` & `pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_debug.c`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_debug.h` & `pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_debug.h`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_display.c` & `pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_display.c`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_display.h` & `pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_display.h`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_extend.c` & `pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_extend.c`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_extend.h` & `pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_extend.h`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_heuristic.c` & `pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_heuristic.c`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_heuristic.h` & `pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_heuristic.h`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_offset.h` & `pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_offset.h`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_pcigar.c` & `pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_pcigar.c`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_pcigar.h` & `pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_pcigar.h`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_penalties.c` & `pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_penalties.c`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_penalties.h` & `pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_penalties.h`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_plot.c` & `pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_plot.c`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_plot.h` & `pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_plot.h`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_slab.c` & `pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_slab.c`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA2_lib/wavefront/wavefront_slab.h` & `pywfa-0.4.2/pywfa/WFA2_lib/wavefront/wavefront_slab.h`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA_wrap.c` & `pywfa-0.4.2/pywfa/WFA_wrap.c`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/WFA_wrap.pxd` & `pywfa-0.4.2/pywfa/WFA_wrap.pxd`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/align.c` & `pywfa-0.4.2/pywfa/align.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.30 */
+/* Generated by Cython 0.29.34 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "extra_compile_args": [
             "-Wno-unused-function",
@@ -46,16 +46,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_30"
-#define CYTHON_HEX_VERSION 0x001D1EF0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -86,14 +86,15 @@
 #ifndef Py_HUGE_VAL
   #define Py_HUGE_VAL HUGE_VAL
 #endif
 #ifdef PYPY_VERSION
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
   #define CYTHON_USE_TYPE_SLOTS 0
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #if PY_VERSION_HEX < 0x03050000
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
@@ -123,20 +124,21 @@
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #undef CYTHON_USE_ASYNC_SLOTS
   #define CYTHON_USE_ASYNC_SLOTS 0
@@ -169,18 +171,64 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+#elif defined(PY_NOGIL)
+  #define CYTHON_COMPILING_IN_PYPY 0
+  #define CYTHON_COMPILING_IN_PYSTON 0
+  #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 1
+  #ifndef CYTHON_USE_TYPE_SLOTS
+    #define CYTHON_USE_TYPE_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYTYPE_LOOKUP
+  #define CYTHON_USE_PYTYPE_LOOKUP 0
+  #ifndef CYTHON_USE_ASYNC_SLOTS
+    #define CYTHON_USE_ASYNC_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYLIST_INTERNALS
+  #define CYTHON_USE_PYLIST_INTERNALS 0
+  #ifndef CYTHON_USE_UNICODE_INTERNALS
+    #define CYTHON_USE_UNICODE_INTERNALS 1
+  #endif
+  #undef CYTHON_USE_UNICODE_WRITER
+  #define CYTHON_USE_UNICODE_WRITER 0
+  #undef CYTHON_USE_PYLONG_INTERNALS
+  #define CYTHON_USE_PYLONG_INTERNALS 0
+  #ifndef CYTHON_AVOID_BORROWED_REFS
+    #define CYTHON_AVOID_BORROWED_REFS 0
+  #endif
+  #ifndef CYTHON_ASSUME_SAFE_MACROS
+    #define CYTHON_ASSUME_SAFE_MACROS 1
+  #endif
+  #ifndef CYTHON_UNPACK_METHODS
+    #define CYTHON_UNPACK_METHODS 1
+  #endif
+  #undef CYTHON_FAST_THREAD_STATE
+  #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_PYCALL
+  #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
+  #ifndef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE 1
+  #endif
+  #undef CYTHON_USE_DICT_VERSIONS
+  #define CYTHON_USE_DICT_VERSIONS 0
+  #undef CYTHON_USE_EXC_INFO_STACK
+  #define CYTHON_USE_EXC_INFO_STACK 0
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYTYPE_LOOKUP
     #define CYTHON_USE_PYTYPE_LOOKUP 0
   #elif !defined(CYTHON_USE_PYTYPE_LOOKUP)
@@ -192,15 +240,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -231,15 +279,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -541,35 +589,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
   #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -1358,26 +1406,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -6774,15 +6822,15 @@
     /* "pywfa/align.pyx":334
  *         self.text_len = 0
  *         if pattern:
  *             self._pattern = pattern             # <<<<<<<<<<<<<<
  * 
  *         # could get a malloc version working
  */
-    if (!(likely(PyUnicode_CheckExact(__pyx_v_pattern))||((__pyx_v_pattern) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_v_pattern)->tp_name), 0))) __PYX_ERR(0, 334, __pyx_L1_error)
+    if (!(likely(PyUnicode_CheckExact(__pyx_v_pattern))||((__pyx_v_pattern) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_v_pattern)->tp_name), 0))) __PYX_ERR(0, 334, __pyx_L1_error)
     __pyx_t_2 = __pyx_v_pattern;
     __Pyx_INCREF(__pyx_t_2);
     __Pyx_GIVEREF(__pyx_t_2);
     __Pyx_GOTREF(__pyx_v_self->_pattern);
     __Pyx_DECREF(__pyx_v_self->_pattern);
     __pyx_v_self->_pattern = ((PyObject*)__pyx_t_2);
     __pyx_t_2 = 0;
@@ -7514,26 +7562,26 @@
       }
     }
     __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_n_u_ascii) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_n_u_ascii);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 410, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (!(likely(PyBytes_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_3)->tp_name), 0))) __PYX_ERR(0, 410, __pyx_L1_error)
+    if (!(likely(PyBytes_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_3)->tp_name), 0))) __PYX_ERR(0, 410, __pyx_L1_error)
     __pyx_v_p = ((PyObject*)__pyx_t_3);
     __pyx_t_3 = 0;
 
     /* "pywfa/align.pyx":411
  *         if pattern is not None:
  *             p = pattern.encode('ascii')
  *             self._pattern = pattern             # <<<<<<<<<<<<<<
  *         else:
  *             p = self._pattern.encode('ascii')
  */
-    if (!(likely(PyUnicode_CheckExact(__pyx_v_pattern))||((__pyx_v_pattern) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_v_pattern)->tp_name), 0))) __PYX_ERR(0, 411, __pyx_L1_error)
+    if (!(likely(PyUnicode_CheckExact(__pyx_v_pattern))||((__pyx_v_pattern) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_v_pattern)->tp_name), 0))) __PYX_ERR(0, 411, __pyx_L1_error)
     __pyx_t_3 = __pyx_v_pattern;
     __Pyx_INCREF(__pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_3);
     __Pyx_GOTREF(__pyx_v_self->_pattern);
     __Pyx_DECREF(__pyx_v_self->_pattern);
     __pyx_v_self->_pattern = ((PyObject*)__pyx_t_3);
     __pyx_t_3 = 0;
@@ -7587,26 +7635,26 @@
     }
   }
   __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_n_u_ascii) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_n_u_ascii);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 414, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (!(likely(PyBytes_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_3)->tp_name), 0))) __PYX_ERR(0, 414, __pyx_L1_error)
+  if (!(likely(PyBytes_CheckExact(__pyx_t_3))||((__pyx_t_3) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_3)->tp_name), 0))) __PYX_ERR(0, 414, __pyx_L1_error)
   __pyx_v_t = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
 
   /* "pywfa/align.pyx":415
  *             p = self._pattern.encode('ascii')
  *         cdef bytes t = text.encode('ascii')
  *         self._text = text             # <<<<<<<<<<<<<<
  *         self.text_len = len(t)
  *         self.pattern_len = len(p)
  */
-  if (!(likely(PyUnicode_CheckExact(__pyx_v_text))||((__pyx_v_text) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_v_text)->tp_name), 0))) __PYX_ERR(0, 415, __pyx_L1_error)
+  if (!(likely(PyUnicode_CheckExact(__pyx_v_text))||((__pyx_v_text) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_v_text)->tp_name), 0))) __PYX_ERR(0, 415, __pyx_L1_error)
   __pyx_t_3 = __pyx_v_text;
   __Pyx_INCREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_3);
   __Pyx_GOTREF(__pyx_v_self->_text);
   __Pyx_DECREF(__pyx_v_self->_text);
   __pyx_v_self->_text = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
@@ -7852,15 +7900,15 @@
       }
     }
     __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_kp_u_UTF_8) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_kp_u_UTF_8);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 428, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (!(likely(PyBytes_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 428, __pyx_L1_error)
+    if (!(likely(PyBytes_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 428, __pyx_L1_error)
     __pyx_v_fname_bytes = ((PyObject*)__pyx_t_1);
     __pyx_t_1 = 0;
 
     /* "pywfa/align.pyx":429
  *         if file_name:
  *             fname_bytes = file_name.encode("UTF-8")
  *             fname = fname_bytes             # <<<<<<<<<<<<<<
@@ -11412,15 +11460,15 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_2 = PyInt_FromLong(2); if (unlikely(!__pyx_int_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_4 = PyInt_FromLong(4); if (unlikely(!__pyx_int_4)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_5 = PyInt_FromLong(5); if (unlikely(!__pyx_int_5)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_7 = PyInt_FromLong(7); if (unlikely(!__pyx_int_7)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_8 = PyInt_FromLong(8); if (unlikely(!__pyx_int_8)) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -11687,15 +11735,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_pywfa__align) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -12383,15 +12431,15 @@
 #endif
     return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
 }
 
 /* ObjectGetItem */
 #if CYTHON_USE_TYPE_SLOTS
 static PyObject *__Pyx_PyObject_GetIndex(PyObject *obj, PyObject* index) {
-    PyObject *runerr;
+    PyObject *runerr = NULL;
     Py_ssize_t key_value;
     PySequenceMethods *m = Py_TYPE(obj)->tp_as_sequence;
     if (unlikely(!(m && m->sq_item))) {
         PyErr_Format(PyExc_TypeError, "'%.200s' object is not subscriptable", Py_TYPE(obj)->tp_name);
         return NULL;
     }
     key_value = __Pyx_PyIndex_AsSsize_t(index);
@@ -12911,18 +12959,16 @@
 
 /* UnpackItemEndCheck */
 static int __Pyx_IternextUnpackEndCheck(PyObject *retval, Py_ssize_t expected) {
     if (unlikely(retval)) {
         Py_DECREF(retval);
         __Pyx_RaiseTooManyValuesError(expected);
         return -1;
-    } else {
-        return __Pyx_IterFinish();
     }
-    return 0;
+    return __Pyx_IterFinish();
 }
 
 /* PyIntCompare */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_EqObjC(PyObject *op1, PyObject *op2, CYTHON_UNUSED long intval, CYTHON_UNUSED long inplace) {
     if (op1 == op2) {
         Py_RETURN_TRUE;
     }
@@ -13145,28 +13191,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -13392,15 +13438,15 @@
         uval = NULL;
         if (uoffset > 0) {
             prepend_sign = !!prepend_sign;
             if (uoffset > prepend_sign) {
                 padding = PyUnicode_FromOrdinal(padding_char);
                 if (likely(padding) && uoffset > prepend_sign + 1) {
                     PyObject *tmp;
-                    PyObject *repeat = PyInt_FromSize_t(uoffset - prepend_sign);
+                    PyObject *repeat = PyInt_FromSsize_t(uoffset - prepend_sign);
                     if (unlikely(!repeat)) goto done_or_error;
                     tmp = PyNumber_Multiply(padding, repeat);
                     Py_DECREF(repeat);
                     Py_DECREF(padding);
                     padding = tmp;
                 }
                 if (unlikely(!padding)) goto done_or_error;
@@ -14526,17 +14572,22 @@
         argc = PyTuple_GET_SIZE(args);
         new_args = PyTuple_GetSlice(args, 1, argc);
         if (unlikely(!new_args))
             return NULL;
         self = PyTuple_GetItem(args, 0);
         if (unlikely(!self)) {
             Py_DECREF(new_args);
+#if PY_MAJOR_VERSION > 2
             PyErr_Format(PyExc_TypeError,
                          "unbound method %.200S() needs an argument",
                          cyfunc->func_qualname);
+#else
+            PyErr_SetString(PyExc_TypeError,
+                            "unbound method needs an argument");
+#endif
             return NULL;
         }
         result = __Pyx_CyFunction_CallMethod(func, self, new_args, kw);
         Py_DECREF(new_args);
     } else {
         result = __Pyx_CyFunction_Call(func, args, kw);
     }
@@ -14761,15 +14812,15 @@
     }
     Py_XDECREF(owned_metaclass);
     return result;
 }
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
```

### Comparing `pywfa-0.4.1/pywfa/align.cpython-310-darwin.so` & `pywfa-0.4.2/pywfa/align.cpython-310-darwin.so`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/align.cpython-39-darwin.so` & `pywfa-0.4.2/pywfa/align.cpython-39-darwin.so`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/align.pyx` & `pywfa-0.4.2/pywfa/align.pyx`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/tests/long.fa` & `pywfa-0.4.2/pywfa/tests/long.fa`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/tests/long.reference.fa` & `pywfa-0.4.2/pywfa/tests/long.reference.fa`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/tests/short.fa` & `pywfa-0.4.2/pywfa/tests/short.fa`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/tests/short.reference.fa` & `pywfa-0.4.2/pywfa/tests/short.reference.fa`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa/tests/test.py` & `pywfa-0.4.2/pywfa/tests/test.py`

 * *Files identical despite different names*

### Comparing `pywfa-0.4.1/pywfa.egg-info/SOURCES.txt` & `pywfa-0.4.2/pywfa.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-LICENSE.md
+LICENSE
 MANIFEST.in
 README.rst
-setup.py
+_custom_build.py
+pyproject.toml
 pywfa/.DS_Store
 pywfa/WFA_wrap.c
 pywfa/WFA_wrap.pxd
 pywfa/__init__.py
 pywfa/align.c
 pywfa/align.cpython-310-darwin.so
 pywfa/align.cpython-39-darwin.so
 pywfa/align.pxd
 pywfa/align.pyx
 pywfa.egg-info/PKG-INFO
 pywfa.egg-info/SOURCES.txt
 pywfa.egg-info/dependency_links.txt
-pywfa.egg-info/not-zip-safe
-pywfa.egg-info/requires.txt
 pywfa.egg-info/top_level.txt
 pywfa/WFA2_lib/alignment/Makefile
 pywfa/WFA2_lib/alignment/affine2p_penalties.c
 pywfa/WFA2_lib/alignment/affine2p_penalties.h
 pywfa/WFA2_lib/alignment/affine_penalties.c
 pywfa/WFA2_lib/alignment/affine_penalties.h
 pywfa/WFA2_lib/alignment/cigar.c
```

