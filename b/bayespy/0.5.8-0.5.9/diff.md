# Comparing `tmp/bayespy-0.5.8.tar.gz` & `tmp/bayespy-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bayespy-0.5.8.tar", last modified: Sat May 13 09:46:47 2017, max compression
+gzip compressed data, was "dist/bayespy-0.5.9.tar", last modified: Sat Sep  2 16:17:21 2017, max compression
```

## Comparing `bayespy-0.5.8.tar` & `bayespy-0.5.9.tar`

### file list

```diff
@@ -1,1909 +1,1909 @@
-drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-05-13 09:46:47.000000 bayespy-0.5.8/
--rw-------   0 jluttine  (1000) jluttine  (1000)     7148 2017-05-13 09:46:47.000000 bayespy-0.5.8/PKG-INFO
--rw-------   0 jluttine  (1000) jluttine  (1000)     4038 2017-01-22 15:43:29.000000 bayespy-0.5.8/setup.py
-drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-05-13 09:46:47.000000 bayespy-0.5.8/bayespy/
-drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-05-13 09:46:47.000000 bayespy-0.5.8/bayespy/tests/
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)     5085 2015-11-02 11:23:25.000000 bayespy-0.5.8/bayespy/tests/test_plot.py
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      393 2015-10-30 13:13:53.000000 bayespy-0.5.8/bayespy/tests/__init__.py
-drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-05-13 09:46:47.000000 bayespy-0.5.8/bayespy/tests/baseline_images/
-drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-05-13 09:46:47.000000 bayespy-0.5.8/bayespy/tests/baseline_images/test_plot/
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)    75254 2015-02-24 08:36:24.000000 bayespy-0.5.8/bayespy/tests/baseline_images/test_plot/contour.png
--rw-------   0 jluttine  (1000) jluttine  (1000)     8322 2016-05-04 12:21:07.000000 bayespy-0.5.8/bayespy/tests/baseline_images/test_plot/hinton_z.png
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)    37179 2015-03-12 13:07:15.000000 bayespy-0.5.8/bayespy/tests/baseline_images/test_plot/gaussian_mixture.png
--rw-------   0 jluttine  (1000) jluttine  (1000)     3769 2016-05-04 12:21:07.000000 bayespy-0.5.8/bayespy/tests/baseline_images/test_plot/hinton_r.png
--rw-------   0 jluttine  (1000) jluttine  (1000)     7439 2016-05-04 12:21:07.000000 bayespy-0.5.8/bayespy/tests/baseline_images/test_plot/hinton_p.png
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)    14971 2015-02-24 08:36:24.000000 bayespy-0.5.8/bayespy/tests/baseline_images/test_plot/pdf.png
-drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-05-13 09:46:47.000000 bayespy-0.5.8/bayespy/utils/
-drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-05-13 09:46:47.000000 bayespy-0.5.8/bayespy/utils/tests/
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)        0 2013-07-24 18:00:26.000000 bayespy-0.5.8/bayespy/utils/tests/__init__.py
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)    17119 2017-01-19 07:35:06.000000 bayespy-0.5.8/bayespy/utils/tests/test_misc.py
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)     6200 2015-11-02 11:23:25.000000 bayespy-0.5.8/bayespy/utils/tests/test_linalg.py
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)     9697 2015-11-02 11:23:25.000000 bayespy-0.5.8/bayespy/utils/tests/test_random.py
--rw-------   0 jluttine  (1000) jluttine  (1000)    11769 2016-05-04 12:21:07.000000 bayespy-0.5.8/bayespy/utils/random.py
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      339 2015-06-03 09:18:36.000000 bayespy-0.5.8/bayespy/utils/__init__.py
--rw-------   0 jluttine  (1000) jluttine  (1000)    17933 2017-01-22 15:43:29.000000 bayespy-0.5.8/bayespy/utils/linalg.py
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)     1566 2015-11-02 11:23:25.000000 bayespy-0.5.8/bayespy/utils/optimize.py
-drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-05-13 09:46:47.000000 bayespy-0.5.8/bayespy/utils/covfunc/
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)    11412 2015-06-03 09:18:36.000000 bayespy-0.5.8/bayespy/utils/covfunc/covariance.py
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)        0 2013-07-24 18:00:26.000000 bayespy-0.5.8/bayespy/utils/covfunc/__init__.py
--rw-------   0 jluttine  (1000) jluttine  (1000)    44791 2017-01-22 15:43:29.000000 bayespy-0.5.8/bayespy/utils/misc.py
--rw-------   0 jluttine  (1000) jluttine  (1000)     1997 2016-05-04 12:21:07.000000 bayespy-0.5.8/bayespy/testing.py
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)     1910 2015-11-02 11:23:25.000000 bayespy-0.5.8/bayespy/discrete_example.py
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      502 2016-08-17 16:45:23.000000 bayespy-0.5.8/bayespy/__init__.py
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      168 2016-08-17 16:45:23.000000 bayespy-0.5.8/bayespy/_meta.py
-drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-05-13 09:46:47.000000 bayespy-0.5.8/bayespy/nodes/
--rw-------   0 jluttine  (1000) jluttine  (1000)     1729 2016-05-04 12:21:07.000000 bayespy-0.5.8/bayespy/nodes/__init__.py
--rw-------   0 jluttine  (1000) jluttine  (1000)      502 2017-01-22 17:35:50.000000 bayespy-0.5.8/bayespy/nodes/gaussian.py
--rw-------   0 jluttine  (1000) jluttine  (1000)    36219 2016-05-04 12:21:07.000000 bayespy-0.5.8/bayespy/plot.py
--rw-------   0 jluttine  (1000) jluttine  (1000)      471 2017-05-13 09:46:47.000000 bayespy-0.5.8/bayespy/_version.py
-drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-05-13 09:46:47.000000 bayespy-0.5.8/bayespy/models/
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)       21 2016-02-11 08:24:32.000000 bayespy-0.5.8/bayespy/models/__init__.py
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     2891 2016-03-21 09:17:48.000000 bayespy-0.5.8/bayespy/models/pca.py
-drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-05-13 09:46:47.000000 bayespy-0.5.8/bayespy/demos/
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)     3429 2015-06-03 09:18:36.000000 bayespy-0.5.8/bayespy/demos/black_box.py
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)     3944 2015-06-09 10:31:05.000000 bayespy-0.5.8/bayespy/demos/pattern_search.py
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)    10707 2015-06-09 10:01:58.000000 bayespy-0.5.8/bayespy/demos/lssm_sd.py
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)     3332 2015-06-03 09:18:36.000000 bayespy-0.5.8/bayespy/demos/annealing.py
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      907 2015-06-03 09:18:36.000000 bayespy-0.5.8/bayespy/demos/categorical.py
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)        0 2015-06-03 09:18:36.000000 bayespy-0.5.8/bayespy/demos/__init__.py
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)    14726 2015-06-03 09:18:36.000000 bayespy-0.5.8/bayespy/demos/lssm_tvd.py
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)     4657 2015-06-03 09:18:36.000000 bayespy-0.5.8/bayespy/demos/pca.py
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)     4028 2015-06-03 09:18:36.000000 bayespy-0.5.8/bayespy/demos/saving.py
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)     4839 2015-06-03 09:18:36.000000 bayespy-0.5.8/bayespy/demos/hmm.py
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)     5013 2015-06-03 09:18:36.000000 bayespy-0.5.8/bayespy/demos/stochastic_inference.py
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      484 2015-07-31 11:15:05.000000 bayespy-0.5.8/bayespy/demos/gamma_shape.py
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)     3284 2015-06-09 09:48:54.000000 bayespy-0.5.8/bayespy/demos/collapsed_cg.py
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)    10690 2015-06-03 09:18:36.000000 bayespy-0.5.8/bayespy/demos/lssm.py
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)     7241 2015-06-15 21:10:51.000000 bayespy-0.5.8/bayespy/demos/lda.py
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)     3110 2015-06-03 09:18:36.000000 bayespy-0.5.8/bayespy/demos/mog.py
-drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-05-13 09:46:47.000000 bayespy-0.5.8/bayespy/inference/
-drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-05-13 09:46:47.000000 bayespy-0.5.8/bayespy/inference/vmp/
-drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-05-13 09:46:47.000000 bayespy-0.5.8/bayespy/inference/vmp/tests/
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)    42154 2015-11-02 11:23:25.000000 bayespy-0.5.8/bayespy/inference/vmp/tests/test_transformations.py
--rw-------   0 jluttine  (1000) jluttine  (1000)     3211 2016-05-04 12:21:07.000000 bayespy-0.5.8/bayespy/inference/vmp/tests/test_annealing.py
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)        0 2013-07-24 18:00:26.000000 bayespy-0.5.8/bayespy/inference/vmp/tests/__init__.py
--rw-------   0 jluttine  (1000) jluttine  (1000)    59456 2016-05-04 12:21:07.000000 bayespy-0.5.8/bayespy/inference/vmp/transformations.py
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)        0 2013-07-24 18:00:26.000000 bayespy-0.5.8/bayespy/inference/vmp/__init__.py
-drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-05-13 09:46:47.000000 bayespy-0.5.8/bayespy/inference/vmp/nodes/
-drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-05-13 09:46:47.000000 bayespy-0.5.8/bayespy/inference/vmp/nodes/tests/
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)     2500 2015-11-02 11:23:25.000000 bayespy-0.5.8/bayespy/inference/vmp/nodes/tests/test_poisson.py
--rw-------   0 jluttine  (1000) jluttine  (1000)    11503 2016-05-04 12:21:07.000000 bayespy-0.5.8/bayespy/inference/vmp/nodes/tests/test_deterministic.py
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)     3781 2015-11-02 11:23:25.000000 bayespy-0.5.8/bayespy/inference/vmp/nodes/tests/test_wishart.py
--rw-------   0 jluttine  (1000) jluttine  (1000)    12147 2017-01-22 15:43:29.000000 bayespy-0.5.8/bayespy/inference/vmp/nodes/tests/test_take.py
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)     3550 2015-11-02 11:23:25.000000 bayespy-0.5.8/bayespy/inference/vmp/nodes/tests/test_bernoulli.py
--rw-------   0 jluttine  (1000) jluttine  (1000)    34034 2016-05-04 12:21:07.000000 bayespy-0.5.8/bayespy/inference/vmp/nodes/tests/test_node.py
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)     2291 2015-11-02 11:23:25.000000 bayespy-0.5.8/bayespy/inference/vmp/nodes/tests/test_dirichlet.py
--rw-------   0 jluttine  (1000) jluttine  (1000)    10768 2016-05-04 12:21:07.000000 bayespy-0.5.8/bayespy/inference/vmp/nodes/tests/test_gate.py
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)     7353 2015-11-02 11:23:25.000000 bayespy-0.5.8/bayespy/inference/vmp/nodes/tests/test_categorical_markov_chain.py
--rw-------   0 jluttine  (1000) jluttine  (1000)    10082 2017-01-22 15:43:29.000000 bayespy-0.5.8/bayespy/inference/vmp/nodes/tests/test_concatenate.py
--rw-------   0 jluttine  (1000) jluttine  (1000)    12835 2017-01-22 15:43:29.000000 bayespy-0.5.8/bayespy/inference/vmp/nodes/tests/test_mixture.py
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)        0 2014-05-03 08:22:08.000000 bayespy-0.5.8/bayespy/inference/vmp/nodes/tests/__init__.py
--rw-------   0 jluttine  (1000) jluttine  (1000)    38334 2017-01-22 15:43:29.000000 bayespy-0.5.8/bayespy/inference/vmp/nodes/tests/test_gaussian_markov_chain.py
--rw-------   0 jluttine  (1000) jluttine  (1000)    50883 2017-01-22 15:43:29.000000 bayespy-0.5.8/bayespy/inference/vmp/nodes/tests/test_gaussian.py
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)     5069 2015-11-02 11:23:25.000000 bayespy-0.5.8/bayespy/inference/vmp/nodes/tests/test_binomial.py
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)     2667 2015-11-02 11:23:25.000000 bayespy-0.5.8/bayespy/inference/vmp/nodes/tests/test_beta.py
--rw-------   0 jluttine  (1000) jluttine  (1000)     7079 2016-05-04 12:21:07.000000 bayespy-0.5.8/bayespy/inference/vmp/nodes/tests/test_categorical.py
--rw-------   0 jluttine  (1000) jluttine  (1000)     5599 2016-05-04 12:21:07.000000 bayespy-0.5.8/bayespy/inference/vmp/nodes/tests/test_gamma.py
--rw-------   0 jluttine  (1000) jluttine  (1000)    31570 2016-05-04 12:21:07.000000 bayespy-0.5.8/bayespy/inference/vmp/nodes/tests/test_dot.py
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)     5319 2017-01-19 07:35:06.000000 bayespy-0.5.8/bayespy/inference/vmp/nodes/tests/test_multinomial.py
--rw-------   0 jluttine  (1000) jluttine  (1000)    13538 2016-05-04 12:21:07.000000 bayespy-0.5.8/bayespy/inference/vmp/nodes/categorical_markov_chain.py
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)    28645 2015-06-03 09:18:36.000000 bayespy-0.5.8/bayespy/inference/vmp/nodes/CovarianceFunctions.py
--rw-------   0 jluttine  (1000) jluttine  (1000)     5448 2016-11-04 16:38:16.000000 bayespy-0.5.8/bayespy/inference/vmp/nodes/newnode.py
--rw-------   0 jluttine  (1000) jluttine  (1000)     6069 2017-05-13 09:44:22.000000 bayespy-0.5.8/bayespy/inference/vmp/nodes/logistic.py
--rw-------   0 jluttine  (1000) jluttine  (1000)     3889 2017-01-22 15:43:29.000000 bayespy-0.5.8/bayespy/inference/vmp/nodes/concat_gaussian.py
--rw-------   0 jluttine  (1000) jluttine  (1000)    74001 2017-01-22 15:43:29.000000 bayespy-0.5.8/bayespy/inference/vmp/nodes/gaussian_markov_chain.py
--rw-------   0 jluttine  (1000) jluttine  (1000)     5230 2016-05-04 12:21:07.000000 bayespy-0.5.8/bayespy/inference/vmp/nodes/beta.py
--rw-------   0 jluttine  (1000) jluttine  (1000)     4418 2016-05-04 12:21:07.000000 bayespy-0.5.8/bayespy/inference/vmp/nodes/bernoulli.py
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)    23431 2015-06-03 09:18:36.000000 bayespy-0.5.8/bayespy/inference/vmp/nodes/gp.py
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)     8964 2017-01-19 07:35:06.000000 bayespy-0.5.8/bayespy/inference/vmp/nodes/multinomial.py
--rw-------   0 jluttine  (1000) jluttine  (1000)     2796 2017-01-22 15:43:29.000000 bayespy-0.5.8/bayespy/inference/vmp/nodes/constant.py
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)    25953 2015-06-03 09:18:36.000000 bayespy-0.5.8/bayespy/inference/vmp/nodes/GaussianProcesses.py
--rw-------   0 jluttine  (1000) jluttine  (1000)     3066 2016-05-04 12:21:07.000000 bayespy-0.5.8/bayespy/inference/vmp/nodes/logpdf.py
--rw-------   0 jluttine  (1000) jluttine  (1000)    21428 2017-01-22 15:43:29.000000 bayespy-0.5.8/bayespy/inference/vmp/nodes/dot.py
--rw-------   0 jluttine  (1000) jluttine  (1000)     5541 2016-05-04 12:21:07.000000 bayespy-0.5.8/bayespy/inference/vmp/nodes/categorical.py
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)    21001 2017-01-19 07:35:06.000000 bayespy-0.5.8/bayespy/inference/vmp/nodes/mixture.py
--rw-------   0 jluttine  (1000) jluttine  (1000)     1544 2017-01-22 15:43:29.000000 bayespy-0.5.8/bayespy/inference/vmp/nodes/__init__.py
--rw-------   0 jluttine  (1000) jluttine  (1000)    11968 2017-01-22 15:43:29.000000 bayespy-0.5.8/bayespy/inference/vmp/nodes/deterministic.py
--rw-------   0 jluttine  (1000) jluttine  (1000)     5228 2016-05-04 12:21:07.000000 bayespy-0.5.8/bayespy/inference/vmp/nodes/point_estimate.py
--rw-------   0 jluttine  (1000) jluttine  (1000)     9550 2017-01-22 15:43:29.000000 bayespy-0.5.8/bayespy/inference/vmp/nodes/wishart.py
--rw-------   0 jluttine  (1000) jluttine  (1000)    80752 2017-01-22 15:43:29.000000 bayespy-0.5.8/bayespy/inference/vmp/nodes/gaussian.py
--rw-------   0 jluttine  (1000) jluttine  (1000)     4426 2016-05-04 12:21:07.000000 bayespy-0.5.8/bayespy/inference/vmp/nodes/add.py
--rw-------   0 jluttine  (1000) jluttine  (1000)     5584 2016-05-04 12:21:07.000000 bayespy-0.5.8/bayespy/inference/vmp/nodes/ml.py
--rw-------   0 jluttine  (1000) jluttine  (1000)      543 2016-11-13 18:28:47.000000 bayespy-0.5.8/bayespy/inference/vmp/nodes/multinomial_probit.py
--rw-------   0 jluttine  (1000) jluttine  (1000)     6038 2016-05-04 12:21:07.000000 bayespy-0.5.8/bayespy/inference/vmp/nodes/binomial.py
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)    11102 2017-01-19 07:35:06.000000 bayespy-0.5.8/bayespy/inference/vmp/nodes/dirichlet.py
--rw-------   0 jluttine  (1000) jluttine  (1000)     5955 2016-05-04 12:21:07.000000 bayespy-0.5.8/bayespy/inference/vmp/nodes/concatenate.py
--rw-------   0 jluttine  (1000) jluttine  (1000)    10709 2017-01-22 15:43:29.000000 bayespy-0.5.8/bayespy/inference/vmp/nodes/gamma.py
--rw-------   0 jluttine  (1000) jluttine  (1000)    18343 2017-01-22 15:43:29.000000 bayespy-0.5.8/bayespy/inference/vmp/nodes/expfamily.py
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)     2137 2015-06-03 09:18:36.000000 bayespy-0.5.8/bayespy/inference/vmp/nodes/exponential.py
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)    11461 2017-01-19 07:35:06.000000 bayespy-0.5.8/bayespy/inference/vmp/nodes/stochastic.py
--rw-------   0 jluttine  (1000) jluttine  (1000)     4426 2017-01-22 15:43:29.000000 bayespy-0.5.8/bayespy/inference/vmp/nodes/take.py
--rw-------   0 jluttine  (1000) jluttine  (1000)     8011 2016-05-04 12:21:07.000000 bayespy-0.5.8/bayespy/inference/vmp/nodes/gate.py
--rw-------   0 jluttine  (1000) jluttine  (1000)    47354 2017-01-22 15:43:29.000000 bayespy-0.5.8/bayespy/inference/vmp/nodes/node.py
--rw-------   0 jluttine  (1000) jluttine  (1000)     1557 2016-05-04 12:21:07.000000 bayespy-0.5.8/bayespy/inference/vmp/nodes/converters.py
--rw-------   0 jluttine  (1000) jluttine  (1000)     3991 2017-05-13 09:44:22.000000 bayespy-0.5.8/bayespy/inference/vmp/nodes/poisson.py
--rw-------   0 jluttine  (1000) jluttine  (1000)    23939 2016-05-04 12:21:07.000000 bayespy-0.5.8/bayespy/inference/vmp/vmp.py
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      799 2015-06-03 09:18:36.000000 bayespy-0.5.8/bayespy/inference/__init__.py
--rw-------   0 jluttine  (1000) jluttine  (1000)      314 2016-08-17 10:33:49.000000 bayespy-0.5.8/MANIFEST.in
--rw-------   0 jluttine  (1000) jluttine  (1000)     6150 2017-01-22 15:43:29.000000 bayespy-0.5.8/INSTALL.rst
-drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-05-13 09:46:47.000000 bayespy-0.5.8/doc/
-drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-05-13 09:46:47.000000 bayespy-0.5.8/doc/source/
-drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-05-13 09:46:47.000000 bayespy-0.5.8/doc/source/dev_guide/
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      701 2015-06-03 09:18:36.000000 bayespy-0.5.8/doc/source/dev_guide/engine.rst
-drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-05-13 09:46:47.000000 bayespy-0.5.8/doc/source/dev_guide/vmp/
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     2465 2013-07-24 18:00:26.000000 bayespy-0.5.8/doc/source/dev_guide/vmp/vmp_gaussian.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1922 2013-07-24 18:00:26.000000 bayespy-0.5.8/doc/source/dev_guide/vmp/vmp_wishart.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)       62 2013-07-24 18:00:26.000000 bayespy-0.5.8/doc/source/dev_guide/vmp/vmp_normal.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)       38 2013-07-24 18:00:26.000000 bayespy-0.5.8/doc/source/dev_guide/vmp/vmp_gamma.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)       57 2013-07-24 18:00:26.000000 bayespy-0.5.8/doc/source/dev_guide/vmp/vmp_gaussian_gamma.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     3286 2013-07-24 18:00:26.000000 bayespy-0.5.8/doc/source/dev_guide/vmp/vmp_mixture.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)       52 2013-07-24 18:00:26.000000 bayespy-0.5.8/doc/source/dev_guide/vmp/vmp_normal_gamma.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)       61 2013-07-24 18:00:26.000000 bayespy-0.5.8/doc/source/dev_guide/vmp/vmp_gaussian_wishart.rst
--rw-------   0 jluttine  (1000) jluttine  (1000)    15553 2016-05-04 12:21:07.000000 bayespy-0.5.8/doc/source/dev_guide/writingnodes.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      459 2015-06-03 09:18:36.000000 bayespy-0.5.8/doc/source/dev_guide/dev_guide.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)    10777 2015-06-03 09:18:36.000000 bayespy-0.5.8/doc/source/dev_guide/vmp.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)     2337 2015-11-02 11:23:25.000000 bayespy-0.5.8/doc/source/dev_guide/workflow.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)     6201 2015-06-03 09:18:36.000000 bayespy-0.5.8/doc/source/dev_guide/advanced.rst
-drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-05-13 09:46:47.000000 bayespy-0.5.8/doc/source/dev_api/
--rw-------   0 jluttine  (1000) jluttine  (1000)     1015 2016-05-04 12:21:07.000000 bayespy-0.5.8/doc/source/dev_api/distributions.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      287 2015-06-03 09:18:36.000000 bayespy-0.5.8/doc/source/dev_api/utils.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      355 2015-06-03 09:18:36.000000 bayespy-0.5.8/doc/source/dev_api/dev_api.rst
-drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-05-13 09:46:47.000000 bayespy-0.5.8/doc/source/dev_api/generated/
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1096 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGammaISO.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      427 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.node.Moments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      485 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.poisson.PoissonMoments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1656 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      978 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianWishartDistribution.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      971 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.categorical.CategoricalDistribution.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      816 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.constant.Constant.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      544 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianWishartMoments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      525 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.multinomial.MultinomialMoments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      591 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISOMoments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1215 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDToGaussianWishart.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      917 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.binomial.BinomialDistribution.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      505 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.dirichlet.DirichletMoments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      527 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.binomial.BinomialMoments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      687 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.categorical_markov_chain.CategoricalMarkovChainMoments.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)     1045 2016-03-30 08:06:12.000000 bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGamma.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1121 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.GaussianMarkovChainDistribution.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      977 2016-03-30 08:06:12.000000 bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGamma.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      935 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.bernoulli.BernoulliDistribution.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1256 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.SwitchingGaussianMarkovChainDistribution.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      560 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.categorical.CategoricalMoments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      890 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.deterministic.Deterministic.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      673 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.node.Node.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1634 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/bayespy.utils.misc.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      971 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.multinomial.MultinomialDistribution.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      829 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gamma.GammaDistribution.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      664 2016-03-30 08:06:12.000000 bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaMoments.rst
-drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-05-13 09:46:47.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      270 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaToGaussianWishart.get_shape.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      291 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaARD.lower_bound_contribution.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      309 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDDistribution.compute_cgf_from_parents.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      252 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaARD.set_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      219 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gamma.GammaMoments.add_converter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      279 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDDistribution.compute_logpdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      264 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDToGaussianWishart.plot.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      246 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaMoments.from_values.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      131 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.is_callable.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      219 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.save.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      276 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaDistribution.plates_to_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      116 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.random.mask.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      303 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianWishartDistribution.compute_moments_and_cgf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      189 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.constant.Constant.plot.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      225 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.update.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      201 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.stochastic.Stochastic.save.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      276 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.dirichlet.DirichletMoments.compute_dims_from_values.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      264 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaToGaussianWishart.plates.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      231 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGamma.plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      243 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.bernoulli.BernoulliDistribution.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      255 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical.CategoricalDistribution.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      131 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.linalg.transpose.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      140 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.squeeze_to_dim.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      303 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical.CategoricalDistribution.compute_phi_from_parents.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      282 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianDistribution.compute_moments_and_cgf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      152 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.random.gaussian_entropy.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      231 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.deterministic.Deterministic.get_mask.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      300 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaDistribution.compute_cgf_from_parents.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      149 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.random.invwishart_rand.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      282 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.wishart.WishartDistribution.compute_weights_to_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      270 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDToGaussianWishart.delete.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      285 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDDistribution.plates_to_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      113 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.linalg.dot.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      312 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical_markov_chain.CategoricalMarkovChainMoments.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      300 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.bernoulli.BernoulliDistribution.compute_fixed_moments_and_f.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      255 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical.CategoricalMoments.get_converter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      201 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.stochastic.Stochastic.plot.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      122 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.get_diag.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      237 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.binomial.BinomialDistribution.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      285 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical.CategoricalDistribution.plates_from_parent.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      243 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGamma.set_plotter.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      255 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGamma.set_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      249 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.deterministic.Deterministic.add_plate_axis.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      165 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.node.Node.plot.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      237 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.binomial.BinomialMoments.add_converter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      128 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.linalg.tracedot.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      255 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.binomial.BinomialDistribution.compute_logpdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      237 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaISO.delete.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      288 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.bernoulli.BernoulliDistribution.compute_moments_and_cgf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      219 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.load.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      237 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianWishart.plates.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      303 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaMoments.get_instance_conversion_kwargs.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      291 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamilyDistribution.plates_to_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      336 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.SwitchingGaussianMarkovChainDistribution.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      285 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianDistribution.compute_cgf_from_parents.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      228 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianWishart.plot.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      177 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.node.Node.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      288 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.binomial.BinomialDistribution.compute_weights_to_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      231 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaISO.plot.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      201 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.stochastic.Stochastic.show.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      294 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.dirichlet.DirichletDistribution.compute_message_to_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      134 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.sum_to_shape.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      312 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamilyDistribution.compute_moments_and_cgf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      134 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.rts_smoother.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      246 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaARD.get_shape.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      222 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianMoments.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      312 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISODistribution.compute_weights_to_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      243 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.stochastic.Stochastic.plates_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      372 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical_markov_chain.CategoricalMarkovChainDistribution.compute_moments_and_cgf.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      249 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGamma.get_shape.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      207 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.beta.BetaDistribution.random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      161 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.random.gaussian_gamma_to_t.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      243 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaARD.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      116 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.linalg.chol.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      113 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.trues.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      140 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.random.wishart_rand.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      252 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaISO.move_plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      333 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.GaussianMarkovChainMoments.compute_fixed_moments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      270 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.stochastic.Distribution.compute_weights_to_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      267 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.bernoulli.BernoulliMoments.compute_fixed_moments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      315 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianWishartDistribution.compute_fixed_moments_and_f.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      240 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.has_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      125 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.m_digamma.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      312 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical.CategoricalDistribution.compute_fixed_moments_and_f.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      285 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaToGaussianWishart.add_plate_axis.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      240 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical.CategoricalMoments.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      231 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.constant.Constant.plates_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      216 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.stochastic.Stochastic.unobserve.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      237 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.beta.BetaDistribution.plates_to_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      237 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gamma.GammaDistribution.compute_logpdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      110 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.symm.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      243 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianWishart.get_shape.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      158 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.linalg.block_banded_solve.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      261 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaARD.add_plate_axis.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      128 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.put_simple.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      318 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISODistribution.compute_fixed_moments_and_f.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      357 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical_markov_chain.CategoricalMarkovChainDistribution.plates_from_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      255 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGammaISO.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      201 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.node.Moments.add_converter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      255 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.poisson.PoissonDistribution.plates_to_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      351 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical_markov_chain.CategoricalMarkovChainMoments.compute_fixed_moments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      149 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.broadcasted_shape.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      152 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.m_solve_triangular.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      149 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.is_scalar_integer.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      231 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaARD.plot.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      231 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.wishart.WishartMoments.add_converter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      122 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.identity.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      261 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.binomial.BinomialMoments.compute_fixed_moments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      146 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.add_leading_axes.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      243 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGamma.get_moments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      297 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISOToGaussianGammaARD.add_plate_axis.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      285 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGammaISO.plates_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      143 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.nested_iterator.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      243 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGamma.has_plotter.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      300 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaDistribution.compute_phi_from_parents.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      119 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.linalg.inner.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      122 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.add_axes.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      234 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.unobserve.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      288 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianWishart.lower_bound_contribution.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      240 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.deterministic.Deterministic.get_moments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      285 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISOMoments.compute_fixed_moments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      210 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.stochastic.Stochastic.plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      333 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.GaussianMarkovChainDistribution.compute_gradient.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      152 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.linalg.solve_triangular.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      273 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical.CategoricalDistribution.compute_logpdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      243 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gamma.GammaMoments.compute_fixed_moments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      249 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianWishart.set_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      219 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.show.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      240 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianWishart.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      228 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      279 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.poisson.PoissonDistribution.compute_cgf_from_parents.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      270 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.binomial.BinomialMoments.compute_dims_from_values.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      288 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.wishart.WishartDistribution.compute_fixed_moments_and_f.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      315 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamilyDistribution.compute_phi_from_parents.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      222 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.node.Node.broadcasting_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      255 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGammaISO.get_mask.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      267 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianDistribution.plates_from_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      276 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.wishart.WishartDistribution.compute_moments_and_cgf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      321 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical_markov_chain.CategoricalMarkovChainDistribution.random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      243 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.beta.BetaDistribution.plates_from_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      303 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGammaISO.lower_bound_contribution.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      276 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaToGaussianWishart.set_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      186 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.node.Node.set_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      285 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISODistribution.plates_to_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      167 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.broadcasting_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      107 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.put.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      294 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianARDDistribution.compute_cgf_from_parents.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      204 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.constant.Constant.get_shape.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      234 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianWishart.delete.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      252 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaARD.get_moments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      131 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.random.dirichlet.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      276 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGamma.plates_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      297 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianARDDistribution.compute_message_to_parent.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      240 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGamma.delete.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      279 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.multinomial.MultinomialDistribution.compute_gradient.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      270 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.initialize_from_value.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      303 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.multinomial.MultinomialDistribution.compute_phi_from_parents.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      249 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.get_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      255 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.multinomial.MultinomialMoments.add_converter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      285 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDToGaussianWishart.has_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      134 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.sum_multiply.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      270 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianMoments.compute_dims_from_values.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      261 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianMoments.compute_fixed_moments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      164 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.random.alpha_beta_recursion.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      204 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.constant.Constant.set_value.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      252 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGamma.add_plate_axis.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      252 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaARD.move_plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      309 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.GaussianMarkovChainMoments.get_converter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      285 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.multinomial.MultinomialDistribution.plates_from_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      303 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianARDDistribution.compute_fixed_moments_and_f.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      210 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.constant.Constant.has_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      375 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical_markov_chain.CategoricalMarkovChainDistribution.compute_phi_from_parents.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      264 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGammaISO.move_plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      210 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.constant.Constant.move_plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      395 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.CholeskyDense.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      255 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianDistribution.compute_logpdf.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      255 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGamma.move_plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      264 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gamma.GammaDistribution.compute_moments_and_cgf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      249 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.poisson.PoissonDistribution.compute_logpdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      219 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.constant.Constant.add_plate_axis.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      279 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.deterministic.Deterministic.lower_bound_contribution.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      125 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.isinteger.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      288 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.dirichlet.DirichletDistribution.compute_moments_and_cgf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      137 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.kalman_filter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      201 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.node.Moments.get_converter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      273 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.bernoulli.BernoulliDistribution.plates_from_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      222 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.stochastic.Stochastic.set_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      207 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.stochastic.Stochastic.random.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      261 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaToGaussianWishart.delete.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      285 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.initialize_from_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      276 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianWishartDistribution.compute_logpdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      249 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.multinomial.MultinomialDistribution.random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      119 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.linalg.m_dot.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      134 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.linalg.logdet_tri.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      128 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.atleast_nd.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      255 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.poisson.PoissonDistribution.compute_gradient.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      237 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianMoments.add_converter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      231 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.deterministic.Deterministic.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      327 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.GaussianMarkovChainDistribution.compute_logpdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      288 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISOToGaussianGammaARD.move_plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      279 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.wishart.WishartDistribution.compute_cgf_from_parents.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      360 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.SwitchingGaussianMarkovChainDistribution.compute_gradient.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      128 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.linalg.chol_inv.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      231 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.binomial.BinomialDistribution.random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      143 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.is_shape_subset.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      267 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.bernoulli.BernoulliDistribution.plates_to_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      282 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.binomial.BinomialDistribution.compute_moments_and_cgf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      210 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.constant.Constant.get_moments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      378 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.VaryingGaussianMarkovChainDistribution.compute_phi_from_parents.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      225 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.deterministic.Deterministic.delete.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      125 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.logsumexp.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      252 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaISO.has_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      285 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.binomial.BinomialDistribution.compute_cgf_from_parents.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      255 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDDistribution.random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      219 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.stochastic.Stochastic.lowerbound.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      315 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamilyDistribution.compute_cgf_from_parents.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      249 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGammaISO.delete.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      288 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianDistribution.compute_weights_to_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      264 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianARDDistribution.compute_logpdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      231 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.beta.BetaDistribution.compute_logpdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      354 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.VaryingGaussianMarkovChainDistribution.compute_gradient.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      143 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.make_equal_ndim.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      291 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaISO.lower_bound_contribution.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      312 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDDistribution.compute_message_to_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      240 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.move_plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      282 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISOToGaussianGammaARD.get_shape.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      240 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianARDDistribution.random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      288 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaISO.broadcasting_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      234 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.node.Moments.compute_dims_from_values.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      378 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.VaryingGaussianMarkovChainDistribution.compute_cgf_from_parents.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      270 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianARDDistribution.compute_gradient.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      294 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDMoments.compute_dims_from_values.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      177 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.node.Node.get_mask.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      255 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGamma.has_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      246 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.beta.BetaMoments.compute_dims_from_values.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      246 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGamma.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      237 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.beta.BetaDistribution.compute_gradient.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      378 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical_markov_chain.CategoricalMarkovChainDistribution.compute_message_to_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      294 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianARDDistribution.compute_phi_from_parents.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      210 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.constant.Constant.set_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      119 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.linalg.mvdot.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      387 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.SwitchingGaussianMarkovChainDistribution.compute_weights_to_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      333 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.GaussianMarkovChainDistribution.plates_to_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      137 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.linalg.chol_logdet.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      134 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.multidigamma.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      149 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.random.gaussian_logpdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      261 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.bernoulli.BernoulliDistribution.compute_logpdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      225 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.logpdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      321 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDToGaussianWishart.broadcasting_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      303 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.multinomial.MultinomialDistribution.compute_cgf_from_parents.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      243 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.get_gradient.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      140 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.dist_haversine.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      207 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.node.Node.plates_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      228 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.deterministic.Deterministic.plates.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      246 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaDistribution.random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      122 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.gradient.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      119 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.linalg.mmdot.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      270 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gamma.GammaDistribution.compute_message_to_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      282 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.wishart.WishartDistribution.compute_message_to_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      309 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISODistribution.compute_cgf_from_parents.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      237 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.lowerbound.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      231 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.get_mask.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      258 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianWishartMoments.get_converter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      243 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.stochastic.Distribution.plates_to_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      128 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.chol_solve.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      306 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISODistribution.compute_moments_and_cgf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      264 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGammaISO.set_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      318 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDDistribution.compute_fixed_moments_and_f.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      261 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamilyDistribution.random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      294 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDToGaussianWishart.add_plate_axis.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      285 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDToGaussianWishart.get_moments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      186 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.node.Node.move_plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      309 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.GaussianMarkovChainMoments.add_converter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      279 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISODistribution.compute_logpdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      261 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDDistribution.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      345 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical_markov_chain.CategoricalMarkovChainDistribution.compute_logpdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      143 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.gaussian_logpdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      116 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.random.orth.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      342 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.GaussianMarkovChainMoments.compute_dims_from_values.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      234 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGamma.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      231 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.stochastic.Stochastic.add_plate_axis.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      252 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gamma.GammaMoments.compute_dims_from_values.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      110 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.rmse.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.node.Node.get_shape.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      222 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.stochastic.Stochastic.has_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      143 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.repeat_to_shape.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      252 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaMoments.get_converter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      354 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.SwitchingGaussianMarkovChainDistribution.compute_logpdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      276 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.deterministic.Deterministic.broadcasting_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      261 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaISO.add_plate_axis.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      171 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.node.Node.delete.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      279 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISOToGaussianGammaARD.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      264 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGammaISO.has_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      152 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.optimize.check_gradient.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      264 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGamma.add_plate_axis.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      279 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.multinomial.MultinomialMoments.compute_fixed_moments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      279 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.poisson.PoissonDistribution.compute_phi_from_parents.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      240 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianWishart.get_mask.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      131 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.chol_logdet.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      288 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISOToGaussianGammaARD.has_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      228 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.observe.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      360 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.SwitchingGaussianMarkovChainDistribution.plates_to_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      249 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.add_plate_axis.rst
-drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-05-13 09:46:47.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertRaisesRegex.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      177 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertGreaterEqual.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertNotIsInstance.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      177 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertAlmostEquals.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      153 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.CholeskyDense.solve.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertRaises.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      162 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.CholeskyDense.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      171 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertWarnsRegex.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertEquals.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      165 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertNotRegex.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      153 2016-01-03 11:18:08.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.failUnless.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      165 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertAllClose.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:08.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.setUp.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      156 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertIsNot.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:08.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.failIfAlmostEqual.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.defaultTestResult.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      153 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertLess.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      156 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.CholeskyDense.logdet.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      177 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertRaisesRegexp.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      186 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertNotAlmostEquals.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      156 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.CholeskySparse.solve.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      171 2016-01-03 11:18:08.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.failUnlessRaises.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      156 2016-01-03 11:18:08.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.failIfEqual.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      171 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertIsInstance.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      156 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertEqual.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:08.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.id.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:08.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.fail.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      168 2016-01-03 11:18:08.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.failUnlessEqual.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:08.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.skipTest.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      165 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.CholeskySparse.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:08.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.tearDown.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      198 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.CholeskyDense.trace_solve_gradient.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      171 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertCountEqual.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      156 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertNotIn.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertRegexpMatches.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertIsNone.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      171 2016-01-03 11:18:08.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.shortDescription.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      162 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertMessage.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      183 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertMessageToChild.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertIn.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      171 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertTupleEqual.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      165 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertNotEqual.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.debug.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      183 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertMultiLineEqual.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:08.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.failIf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assert_.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      168 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertLessEqual.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.addTypeEqualityFunc.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      156 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertRegex.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      195 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertDictContainsSubset.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      162 2016-01-03 11:18:08.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.tearDownClass.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      171 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertArrayEqual.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      201 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.CholeskySparse.trace_solve_gradient.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      153 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertTrue.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      189 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertNotRegexpMatches.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      153 2016-01-03 11:18:08.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.doCleanups.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      183 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertNotAlmostEqual.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      132 2016-01-03 11:18:08.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.run.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      162 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertGreater.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      168 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertNotEquals.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      186 2016-01-03 11:18:08.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.failUnlessAlmostEqual.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      153 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.addCleanup.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      165 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.countTestCases.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertSequenceEqual.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      153 2016-01-03 11:18:08.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.setUpClass.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      168 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertListEqual.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      168 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertIsNotNone.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      156 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertFalse.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertIs.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      156 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertWarns.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      153 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertLogs.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      168 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertDictEqual.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:08.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.maxDiff.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:08.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.longMessage.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      165 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertSetEqual.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.CholeskySparse.logdet.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:08.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.subTest.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertAlmostEqual.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      273 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaISO.plates_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      354 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.VaryingGaussianMarkovChainDistribution.plates_to_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      285 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianWishart.broadcasting_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      237 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.binomial.BinomialMoments.get_converter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      291 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDDistribution.plates_from_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      354 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.GaussianMarkovChainDistribution.compute_moments_and_cgf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      261 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.binomial.BinomialDistribution.compute_gradient.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      267 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.dirichlet.DirichletDistribution.plates_to_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      288 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical.CategoricalMoments.compute_dims_from_values.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      276 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISOToGaussianGammaARD.plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      279 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.multinomial.MultinomialDistribution.plates_to_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      261 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.poisson.PoissonDistribution.plates_from_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      255 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.poisson.PoissonMoments.compute_fixed_moments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      128 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.is_numeric.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      285 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDToGaussianWishart.move_plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      252 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaISO.set_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      285 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDMoments.compute_fixed_moments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      122 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.cholesky.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      222 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.stochastic.Stochastic.move_plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      276 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.bernoulli.BernoulliMoments.compute_dims_from_values.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      255 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.wishart.WishartDistribution.plates_to_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      261 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.deterministic.Deterministic.plates_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      101 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.T.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      249 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.wishart.WishartDistribution.compute_logpdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      384 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.SwitchingGaussianMarkovChainDistribution.compute_phi_from_parents.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      149 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.add_trailing_axes.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      294 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.dirichlet.DirichletDistribution.compute_weights_to_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      201 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.stochastic.Stochastic.load.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      270 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.beta.BetaDistribution.compute_fixed_moments_and_f.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      318 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamilyDistribution.compute_weights_to_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      384 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.SwitchingGaussianMarkovChainDistribution.compute_cgf_from_parents.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      300 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.dirichlet.DirichletDistribution.compute_fixed_moments_and_f.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      330 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.VaryingGaussianMarkovChainDistribution.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      252 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianWishartDistribution.random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      393 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.SwitchingGaussianMarkovChainDistribution.compute_fixed_moments_and_f.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      222 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.stochastic.Stochastic.get_moments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      288 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianWishartDistribution.plates_from_parent.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      255 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGamma.get_moments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      137 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.write_to_hdf5.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      264 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.beta.BetaDistribution.compute_weights_to_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      219 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.deterministic.Deterministic.plot.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      264 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.beta.BetaDistribution.compute_message_to_parent.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      243 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGamma.move_plates.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      234 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGamma.plot.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      243 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.bernoulli.BernoulliMoments.get_converter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      306 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDToGaussianWishart.plates_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      279 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDToGaussianWishart.get_shape.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      213 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gamma.GammaDistribution.random.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      282 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGamma.lower_bound_contribution.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      252 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaDistribution.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      297 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianARDDistribution.compute_weights_to_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      240 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.get_moments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      164 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.sum_multiply_to_plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      261 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianDistribution.plates_to_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      134 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.optimize.minimize.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      288 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.multinomial.MultinomialMoments.compute_dims_from_values.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      258 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.beta.BetaDistribution.compute_moments_and_cgf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      282 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.poisson.PoissonDistribution.compute_weights_to_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      309 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISODistribution.compute_phi_from_parents.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      276 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gamma.GammaDistribution.compute_fixed_moments_and_f.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      264 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGammaISO.get_moments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      125 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.random.wishart.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      279 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.wishart.WishartDistribution.compute_phi_from_parents.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      303 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.GaussianMarkovChainDistribution.random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      273 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDToGaussianWishart.plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      282 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianWishartMoments.compute_fixed_moments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      264 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.wishart.WishartMoments.compute_dims_from_values.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      246 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.constant.Constant.broadcasting_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      276 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDToGaussianWishart.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      348 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.VaryingGaussianMarkovChainDistribution.compute_logpdf.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      282 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaDistribution.plates_from_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      285 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamilyDistribution.compute_logpdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      185 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.broadcasted_shape_from_arrays.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      327 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical_markov_chain.CategoricalMarkovChainDistribution.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      240 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.deterministic.Deterministic.move_plates.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      267 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaToGaussianWishart.get_mask.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      258 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianWishart.add_plate_axis.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      213 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.stochastic.Stochastic.get_mask.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      134 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.random.covariance.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      270 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaDistribution.compute_logpdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      309 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.GaussianMarkovChainDistribution.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      243 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.dirichlet.DirichletMoments.get_converter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      261 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISOMoments.add_converter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      119 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.linalg.outer.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      249 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.constant.Constant.lower_bound_contribution.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      216 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.stochastic.Stochastic.get_shape.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      149 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.remove_whitespace.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      282 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.poisson.PoissonDistribution.compute_message_to_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      152 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.composite_function.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      309 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianWishartDistribution.compute_message_to_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      306 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.multinomial.MultinomialDistribution.compute_message_to_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      113 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.random.svd.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      237 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaARD.delete.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      201 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.constant.Constant.__init__.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      297 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaToGaussianWishart.plates_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      309 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianWishartDistribution.compute_weights_to_parent.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      309 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaDistribution.compute_fixed_moments_and_f.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      246 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGamma.get_mask.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      149 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.make_equal_length.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      195 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.node.Node.add_plate_axis.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      116 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.invpsi.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      309 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISOToGaussianGammaARD.plates_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      288 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISOToGaussianGammaARD.get_moments.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      252 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaMoments.add_converter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      381 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.VaryingGaussianMarkovChainDistribution.compute_message_to_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      267 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gamma.GammaDistribution.compute_phi_from_parents.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      300 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical.CategoricalDistribution.compute_moments_and_cgf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      387 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.VaryingGaussianMarkovChainDistribution.compute_fixed_moments_and_f.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      134 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.linalg.logdet_cov.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      119 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.squeeze.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      273 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.initialize_from_random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      312 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.multinomial.MultinomialDistribution.compute_fixed_moments_and_f.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      240 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaARD.plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      240 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.deterministic.Deterministic.has_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      252 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaARD.has_plotter.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      303 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaDistribution.compute_message_to_parent.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      297 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaDistribution.compute_moments_and_cgf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      261 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDMoments.get_converter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      261 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.binomial.BinomialDistribution.plates_to_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      261 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDMoments.add_converter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      285 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDDistribution.compute_gradient.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      360 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.GaussianMarkovChainDistribution.compute_weights_to_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      255 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.multinomial.MultinomialDistribution.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      231 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.poisson.PoissonMoments.get_converter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      288 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISOToGaussianGammaARD.set_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      131 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.random.bernoulli.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      291 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianARDDistribution.compute_moments_and_cgf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      267 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.bernoulli.BernoulliDistribution.compute_gradient.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      170 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.random.logodds_to_probability.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      273 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGammaISO.add_plate_axis.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      318 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamilyDistribution.compute_message_to_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      267 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISOToGaussianGammaARD.plot.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      110 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.grid.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      122 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.tempfile.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      303 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical.CategoricalDistribution.compute_cgf_from_parents.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      134 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.zipper_merge.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      285 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISODistribution.compute_gradient.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      276 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaDistribution.compute_gradient.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      134 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.block_banded.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      378 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical_markov_chain.CategoricalMarkovChainDistribution.compute_weights_to_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      324 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamilyDistribution.compute_fixed_moments_and_f.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      216 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.pdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      213 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.stochastic.Distribution.random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      234 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.get_shape.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      255 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.wishart.WishartDistribution.compute_gradient.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      264 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGamma.plates_multiplier.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      237 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGamma.get_shape.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      249 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.stochastic.Distribution.plates_from_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      128 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.sum_to_dim.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      294 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianDistribution.compute_fixed_moments_and_f.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      143 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.array_to_scalar.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      240 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.deterministic.Deterministic.set_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      312 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDDistribution.compute_weights_to_parent.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      315 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaToGaussianWishart.lower_bound_contribution.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      122 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.moveaxis.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      125 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.is_string.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      237 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianMoments.get_converter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      384 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical_markov_chain.CategoricalMarkovChainDistribution.compute_fixed_moments_and_f.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      294 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.bernoulli.BernoulliDistribution.compute_message_to_parent.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      255 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaToGaussianWishart.plot.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      300 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGammaISO.broadcasting_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      270 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.stochastic.Distribution.compute_message_to_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      357 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.GaussianMarkovChainDistribution.compute_phi_from_parents.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      246 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaISO.get_shape.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      291 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.dirichlet.DirichletDistribution.compute_phi_from_parents.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      276 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaToGaussianWishart.has_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      113 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.m_dot.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      137 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.random.categorical.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      360 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.GaussianMarkovChainDistribution.compute_message_to_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      306 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDDistribution.compute_moments_and_cgf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      122 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.random.sphere.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      270 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianARDDistribution.plates_to_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      291 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.bernoulli.BernoulliDistribution.compute_phi_from_parents.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      213 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.beta.BetaMoments.get_converter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      222 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.binomial.BinomialMoments.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      273 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISOToGaussianGammaARD.delete.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      291 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISODistribution.plates_from_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      252 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGammaISO.plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      231 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.poisson.PoissonMoments.add_converter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      146 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.axes_to_collapse.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      222 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGamma.plot.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      276 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.poisson.PoissonDistribution.compute_moments_and_cgf.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      243 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGamma.plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      327 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISOToGaussianGammaARD.lower_bound_contribution.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      294 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISOMoments.compute_dims_from_values.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      240 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.set_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      134 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.linalg.chol_solve.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      249 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.set_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.node.Node.plates.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      276 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaToGaussianWishart.get_moments.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      276 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaMoments.compute_fixed_moments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      291 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.dirichlet.DirichletDistribution.compute_cgf_from_parents.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      122 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.invgamma.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      324 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDToGaussianWishart.lower_bound_contribution.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      213 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.beta.BetaMoments.add_converter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      255 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical.CategoricalMoments.add_converter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      255 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.multinomial.MultinomialMoments.get_converter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      119 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.ceildiv.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      210 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.stochastic.Stochastic.observe.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      258 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGammaISO.get_shape.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      273 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.multinomial.MultinomialDistribution.compute_logpdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      279 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical.CategoricalDistribution.compute_gradient.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      375 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.VaryingGaussianMarkovChainDistribution.compute_moments_and_cgf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      261 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.wishart.WishartDistribution.plates_from_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      279 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.lower_bound_contribution.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      186 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.node.Node.get_moments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      306 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical.CategoricalDistribution.compute_message_to_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      273 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.dirichlet.DirichletDistribution.plates_from_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      186 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.node.Node.has_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      267 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.dirichlet.DirichletMoments.compute_fixed_moments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      357 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.GaussianMarkovChainDistribution.compute_cgf_from_parents.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      225 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      309 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDDistribution.compute_phi_from_parents.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      285 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianDistribution.compute_phi_from_parents.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      243 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGammaISO.plot.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      279 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaMoments.get_instance_converter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      225 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.poisson.PoissonDistribution.random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      143 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.random.gamma_entropy.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      243 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaISO.get_mask.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      303 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaDistribution.compute_weights_to_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      294 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.binomial.BinomialDistribution.compute_fixed_moments_and_f.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      285 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.binomial.BinomialDistribution.compute_phi_from_parents.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      143 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.multiply_shapes.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      288 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaARD.broadcasting_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      207 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.stochastic.Stochastic.delete.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      360 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.VaryingGaussianMarkovChainDistribution.plates_from_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      306 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianWishartDistribution.compute_phi_from_parents.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      366 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.GaussianMarkovChainDistribution.compute_fixed_moments_and_f.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      261 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.beta.BetaDistribution.compute_phi_from_parents.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      312 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISODistribution.compute_message_to_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      137 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.linalg.logdet_chol.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      228 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.bernoulli.BernoulliMoments.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      249 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianWishart.move_plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      134 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.safe_indices.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      255 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.wishart.WishartMoments.compute_fixed_moments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      360 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical_markov_chain.CategoricalMarkovChainMoments.compute_dims_from_values.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      113 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.first.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      264 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.poisson.PoissonMoments.compute_dims_from_values.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      122 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.diagonal.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      387 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.SwitchingGaussianMarkovChainDistribution.compute_message_to_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      246 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISOMoments.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      282 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianWishartDistribution.compute_gradient.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      243 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gamma.GammaDistribution.plates_to_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      119 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.m_outer.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      131 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.logdet_chol.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      291 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGamma.broadcasting_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      270 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.initialize_from_prior.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      267 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gamma.GammaDistribution.compute_cgf_from_parents.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      231 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianDistribution.random.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      237 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaMoments.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      252 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaISO.get_moments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      201 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.constant.Constant.get_mask.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      291 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.bernoulli.BernoulliDistribution.compute_cgf_from_parents.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      249 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianWishart.get_moments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      279 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISOToGaussianGammaARD.get_mask.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      225 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.node.Moments.compute_fixed_moments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      222 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.dims.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      261 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.beta.BetaDistribution.compute_cgf_from_parents.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      261 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.dirichlet.DirichletDistribution.compute_logpdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      131 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.random.intervals.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      282 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianWishartDistribution.plates_to_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      243 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaARD.get_mask.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      225 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.delete.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      375 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical_markov_chain.CategoricalMarkovChainDistribution.compute_cgf_from_parents.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      237 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.bernoulli.BernoulliDistribution.random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      113 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.linalg.inv.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      285 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDToGaussianWishart.set_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      261 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianDistribution.compute_gradient.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      276 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.get_riemannian_gradient.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      116 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.unique.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      243 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.dirichlet.DirichletMoments.add_converter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      267 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.dirichlet.DirichletDistribution.compute_gradient.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      246 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianARDDistribution.__init__.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      228 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGamma.delete.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      327 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical_markov_chain.CategoricalMarkovChainMoments.add_converter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      131 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.sum_product.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      270 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gamma.GammaDistribution.compute_weights_to_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      267 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.binomial.BinomialDistribution.plates_from_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      402 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.CholeskySparse.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      246 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDMoments.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      306 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianWishartDistribution.compute_cgf_from_parents.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      330 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.SwitchingGaussianMarkovChainDistribution.random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      291 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamilyDistribution.compute_gradient.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      237 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.dirichlet.DirichletDistribution.random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      261 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISOMoments.get_converter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      258 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianWishartMoments.add_converter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      240 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaISO.plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      182 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.parse_command_line_arguments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      279 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical.CategoricalMoments.compute_fixed_moments.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      312 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaToGaussianWishart.broadcasting_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      270 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianWishart.plates_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      297 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamilyDistribution.plates_from_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      288 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianDistribution.compute_message_to_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      273 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaARD.plates_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      261 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.plates_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      276 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDToGaussianWishart.get_mask.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      137 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.random.correlation.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     2479 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.TestCase.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      231 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      255 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISODistribution.random.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      279 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGamma.broadcasting_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      243 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.bernoulli.BernoulliMoments.add_converter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      237 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.beta.BetaMoments.compute_fixed_moments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      288 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.binomial.BinomialDistribution.compute_message_to_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      213 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.stochastic.Stochastic.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      381 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.SwitchingGaussianMarkovChainDistribution.compute_moments_and_cgf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      110 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.chol.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      267 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaToGaussianWishart.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      351 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical_markov_chain.CategoricalMarkovChainDistribution.compute_gradient.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      306 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical.CategoricalDistribution.compute_weights_to_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      219 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.plot.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      351 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical_markov_chain.CategoricalMarkovChainDistribution.plates_to_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      122 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.chol_inv.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      339 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.GaussianMarkovChainDistribution.plates_from_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      140 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.random.gamma_logpdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      234 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.deterministic.Deterministic.get_shape.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      249 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianWishart.has_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      195 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.constant.Constant.delete.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      276 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianARDDistribution.plates_from_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      276 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.broadcasting_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      243 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaISO.__init__.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      276 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaToGaussianWishart.move_plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      258 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.stochastic.Stochastic.broadcasting_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      225 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.wishart.WishartDistribution.random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      243 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gamma.GammaDistribution.compute_gradient.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      324 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISOToGaussianGammaARD.broadcasting_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      324 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.VaryingGaussianMarkovChainDistribution.random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      110 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.mean.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      327 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical_markov_chain.CategoricalMarkovChainMoments.get_converter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      198 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.constant.Constant.plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      279 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical.CategoricalDistribution.plates_to_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      249 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical.CategoricalDistribution.random.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      294 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGamma.lower_bound_contribution.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      128 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.random.t_logpdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      288 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.poisson.PoissonDistribution.compute_fixed_moments_and_f.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      219 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gamma.GammaMoments.get_converter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      140 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.find_set_index.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      291 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianWishartMoments.compute_dims_from_values.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      110 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.diag.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      306 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.multinomial.MultinomialDistribution.compute_weights_to_parent.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      234 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGamma.get_mask.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      110 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.nans.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      207 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.stochastic.Stochastic.update.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      249 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gamma.GammaDistribution.plates_from_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      300 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.multinomial.MultinomialDistribution.compute_moments_and_cgf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      381 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.VaryingGaussianMarkovChainDistribution.compute_weights_to_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      366 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.SwitchingGaussianMarkovChainDistribution.plates_from_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      231 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.wishart.WishartMoments.get_converter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      294 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.bernoulli.BernoulliDistribution.compute_weights_to_parent.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      581 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/bayespy.utils.random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1009 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamilyDistribution.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      863 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.poisson.PoissonDistribution.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      538 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.bernoulli.BernoulliMoments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1037 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDDistribution.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)     1164 2016-03-30 08:06:12.000000 bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaToGaussianWishart.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1175 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.categorical_markov_chain.CategoricalMarkovChainDistribution.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      992 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISODistribution.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      992 2016-03-30 08:06:12.000000 bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaDistribution.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      863 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.wishart.WishartDistribution.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1028 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaARD.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      880 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianDistribution.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1028 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaISO.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1232 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISOToGaussianGammaARD.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      471 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/bayespy.utils.linalg.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1011 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianWishart.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      455 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.beta.BetaMoments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      962 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianARDDistribution.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      591 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDMoments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1226 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.VaryingGaussianMarkovChainDistribution.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      520 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.stochastic.Distribution.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      812 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.beta.BetaDistribution.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      611 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.GaussianMarkovChainMoments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      485 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.wishart.WishartMoments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      989 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.stochastic.Stochastic.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      527 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianMoments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      897 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.dirichlet.DirichletDistribution.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      465 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gamma.GammaMoments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      241 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/dev_api/generated/bayespy.utils.optimize.rst
--rw-------   0 jluttine  (1000) jluttine  (1000)      751 2016-05-04 12:21:07.000000 bayespy-0.5.8/doc/source/dev_api/nodes.rst
--rw-------   0 jluttine  (1000) jluttine  (1000)      713 2016-05-04 12:21:07.000000 bayespy-0.5.8/doc/source/dev_api/moments.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      219 2015-06-03 09:18:36.000000 bayespy-0.5.8/doc/source/references.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      449 2015-06-03 09:18:36.000000 bayespy-0.5.8/doc/source/index.rst
-drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-05-13 09:46:47.000000 bayespy-0.5.8/doc/source/_templates/
-drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-05-13 09:46:47.000000 bayespy-0.5.8/doc/source/_templates/autosummary/
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      581 2014-07-07 08:35:29.000000 bayespy-0.5.8/doc/source/_templates/autosummary/class.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      716 2014-07-07 08:35:29.000000 bayespy-0.5.8/doc/source/_templates/autosummary/module.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)       63 2014-07-07 08:35:29.000000 bayespy-0.5.8/doc/source/_templates/autosummary/short_module.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)    11016 2016-08-17 16:45:23.000000 bayespy-0.5.8/doc/source/conf.py
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      283 2015-06-03 09:18:36.000000 bayespy-0.5.8/doc/source/intro.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      526 2015-06-03 09:18:36.000000 bayespy-0.5.8/doc/source/nodes.rst
-drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-05-13 09:46:47.000000 bayespy-0.5.8/doc/source/user_api/
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      323 2015-06-03 09:18:36.000000 bayespy-0.5.8/doc/source/user_api/user_api.rst
-drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-05-13 09:46:47.000000 bayespy-0.5.8/doc/source/user_api/generated/
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)       55 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/bayespy.plot.rst
-drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-05-13 09:46:47.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      284 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.plot.ContourPlotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      344 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.plot.CategoricalMarkovChainPlotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1482 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.nodes.GaussianARD.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      877 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.inference.VB.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)       98 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.plot.hinton.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1116 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.nodes.Beta.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1313 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.nodes.Gaussian.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1407 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.nodes.Exponential.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1368 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.nodes.Categorical.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1949 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1296 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.nodes.Bernoulli.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      618 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.inference.vmp.transformations.RotateSwitchingMarkovChain.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)     1667 2016-03-30 08:06:12.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.nodes.GaussianGamma.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      101 2016-06-12 17:22:50.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.nodes.Choose.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     2023 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)       92 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.nodes.Dot.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1224 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.nodes.Poisson.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1224 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.nodes.Wishart.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      256 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.plot.Plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      600 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.inference.vmp.transformations.RotateVaryingMarkovChain.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      636 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.nodes.Add.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      510 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.inference.vmp.transformations.RotateMultiple.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1548 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.nodes.GaussianGammaARD.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      137 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.plot.gaussian_mixture_2d.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      403 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.inference.vmp.transformations.RotationOptimizer.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      721 2016-06-12 17:22:50.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.nodes.Function.rst
-drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-05-13 09:46:47.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      276 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateGaussianMarkovChain.get_bound_terms.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      165 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.broadcasting_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      153 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.set_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.add_plate_axis.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      177 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.initialize_from_random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      171 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.plates_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      165 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.get_riemannian_gradient.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      165 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gate.broadcasting_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      120 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.set_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.VB.set_callback.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      123 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.plot.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      162 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.initialize_from_prior.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      198 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.initialize_from_random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      177 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.initialize_from_random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      123 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.update.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.get_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      123 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.get_mask.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      117 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.observe.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.set_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.has_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      186 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.get_gradient.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      120 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.save.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.move_plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      183 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.set_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.VB.pattern_search.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      249 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateGaussianMarkovChain.rotate.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      168 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.get_shape.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.set_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      183 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.has_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      156 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.VB.compute_lowerbound.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      171 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.VB.plot_iteration_by_nodes.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.get_riemannian_gradient.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      231 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.broadcasting_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      162 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.initialize_from_value.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      192 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.get_mask.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      114 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      120 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Add.get_shape.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.delete.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      153 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.add_plate_axis.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      171 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.initialize_from_random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.get_riemannian_gradient.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      171 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.plates_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.pdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.rotate.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      114 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Add.plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.has_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      189 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.initialize_from_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.initialize_from_prior.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      114 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.update.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      225 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.initialize_from_value.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      210 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.set_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      207 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.initialize_from_random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.delete.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      195 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.get_moments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      207 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.initialize_from_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.move_plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      183 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.initialize_from_random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      117 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.delete.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      222 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateGaussian.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.get_mask.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      210 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.get_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.get_moments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.logpdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.show.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      147 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.update.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.get_riemannian_gradient.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      213 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateGaussian.setup.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      183 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.dims.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      252 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateVaryingMarkovChain.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      189 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.pdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gate.get_moments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      222 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateGaussianARD.nodes.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      213 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.lower_bound_contribution.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.add_plate_axis.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      201 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.get_moments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      114 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.pdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      117 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.pdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      114 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.dims.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      105 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.pdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      162 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.load.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      183 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.observe.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      153 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.observe.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.get_mask.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Add.get_moments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Add.set_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.broadcasting_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      219 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.initialize_from_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.set_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      117 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Add.get_mask.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.plates_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.set_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.lowerbound.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.set_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.unobserve.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.lowerbound.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 14:57:36.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Take.plates_multiplier.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      147 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.get_mask.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.load.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      156 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      114 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.pdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      168 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.lower_bound_contribution.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.get_riemannian_gradient.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      120 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.save.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.load.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.logpdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.add_plate_axis.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      117 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.pdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      234 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.initialize_from_random.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      147 2016-06-12 17:22:50.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.ConcatGaussian.plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      183 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.initialize_from_random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.initialize_from_value.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.logpdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      195 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.integrated_logpdf_from_parents.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      189 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.unobserve.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.get_shape.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.set_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      120 2016-01-03 14:57:36.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Take.get_mask.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      240 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.lower_bound_contribution.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      168 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.initialize_from_prior.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.get_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.update.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      213 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateGaussian.nodes.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      183 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.get_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.logpdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.set_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.initialize_from_value.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      177 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.dims.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.get_shape.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      123 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gate.get_shape.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.delete.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      123 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.plot.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.load.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.unobserve.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      183 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.lower_bound_contribution.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      156 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.get_moments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.set_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      165 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.get_gradient.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      132 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.dims.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.lowerbound.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.dims.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.get_gradient.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      153 2016-06-12 17:22:50.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.ConcatGaussian.get_shape.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.initialize_from_prior.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      165 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.move_plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.initialize_from_random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      132 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.set_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.lower_bound_contribution.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.has_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.lowerbound.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      108 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.save.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      120 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.dims.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      177 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.get_gradient.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      123 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.delete.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.move_plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.plot.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      171 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.set_parameters.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      141 2016-06-12 17:22:50.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Function.has_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      114 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.delete.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      156 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.set_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      171 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.plates_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.delete.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      153 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.plot.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      123 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.load.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      138 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.dims.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.get_shape.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      168 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.get_riemannian_gradient.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      186 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.get_gaussian_location.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gate.move_plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      189 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.lower_bound_contribution.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      168 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.broadcasting_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.broadcasting_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.has_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.get_gradient.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.observe.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      171 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.initialize_from_random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      195 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.unobserve.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.rotate.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.SumMultiply.move_plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      171 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.lower_bound_contribution.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.SumMultiply.get_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      177 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.lower_bound_contribution.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.get_moments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.add_plate_axis.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.initialize_from_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.get_riemannian_gradient.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      165 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Add.lower_bound_contribution.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      123 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.save.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.set_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.unobserve.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.random.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      198 2016-06-12 17:22:50.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.ConcatGaussian.lower_bound_contribution.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      198 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.broadcasting_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      171 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.pdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      156 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.unobserve.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      111 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.show.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.move_plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.__init__.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      150 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.get_shape.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.VB.use_logging.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.get_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      222 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateGaussianARD.setup.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      156 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.rotate_plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.initialize_from_prior.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      156 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.dims.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.get_mask.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      153 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.plotmatrix.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gate.has_plotter.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      132 2016-06-12 17:22:50.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Function.get_mask.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      189 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.lower_bound_contribution.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      186 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.get_riemannian_gradient.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.rotate.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      213 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateMultiple.nodes.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      165 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.initialize_from_random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      153 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.get_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      132 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.unobserve.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.pdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      183 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.initialize_from_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.observe.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      108 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gate.plot.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 14:57:36.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Take.add_plate_axis.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      243 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateMultiple.get_bound_terms.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      120 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.pdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      186 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.update.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      123 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.delete.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      144 2016-06-12 17:22:50.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.ConcatGaussian.delete.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      150 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.translate.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.get_gradient.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      234 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.lower_bound_contribution.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      117 2016-01-03 14:57:36.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Take.plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      195 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.initialize_from_prior.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.observe.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.plot.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      177 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.broadcasting_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      201 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.broadcasting_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.get_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.plot.Plotter.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      228 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.initialize_from_random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      108 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.pdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 14:57:36.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Take.has_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      132 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.get_mask.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      156 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.as_diagonal_wishart.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.set_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      168 2016-01-03 14:57:36.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Take.lower_bound_contribution.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      120 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      165 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.set_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.get_gradient.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      120 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.dims.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.dims.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      153 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      228 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.initialize_from_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      195 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.has_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.load.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      123 2016-01-03 14:57:36.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Take.get_shape.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.observe.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.initialize_from_value.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      189 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.SumMultiply.lower_bound_contribution.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      120 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.show.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      162 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.VB.ignore_bound_checks.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      225 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateGaussianARD.rotate.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.get_moments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      183 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.move_plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.pdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.initialize_from_value.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      201 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.has_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      216 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateGaussian.rotate.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      165 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.set_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      204 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.lower_bound_contribution.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      132 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.has_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      162 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.show.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.get_mask.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.get_shape.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      210 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.initialize_from_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      123 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.show.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      165 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.plates_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      171 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.plates_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      210 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.initialize_from_parameters.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      186 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.initialize_from_prior.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      231 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateGaussianARD.__init__.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      150 2016-06-12 17:22:50.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.ConcatGaussian.get_mask.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      273 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateVaryingMarkovChain.get_bound_terms.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      246 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateGaussianMarkovChain.setup.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      111 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.dims.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      204 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.add_plate_axis.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.has_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      189 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.get_marginal_logpdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      123 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.dims.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.VB.gradient_step.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      204 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.get_gradient.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      159 2016-06-12 17:22:50.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.ConcatGaussian.move_plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.get_gradient.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.initialize_from_value.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.set_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.unobserve.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.SumMultiply.has_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      162 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.rotate.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      123 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.get_shape.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      213 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateMultiple.setup.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      120 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gate.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.set_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      186 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      192 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.lowerbound.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.set_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      162 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.plotmatrix.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      204 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.plates_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      156 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.get_mask.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      204 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.initialize_from_prior.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      231 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotationOptimizer.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      168 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.initialize_from_value.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.get_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Add.add_plate_axis.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.rotate_matrix.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.broadcasting_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      162 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.move_plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.initialize_from_random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.get_shape.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      216 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.plates_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.get_gradient.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.plot.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.has_plotter.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      162 2016-06-12 17:22:50.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Function.plates_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.show.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      213 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateMultiple.bound.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      165 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.set_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      117 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.show.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.update.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      171 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      108 2016-01-03 14:57:36.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Take.plot.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.SumMultiply.add_plate_axis.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.set_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      225 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotationOptimizer.rotate.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.set_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.save.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.pdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      132 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.dims.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      111 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Add.delete.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      195 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.lower_bound_contribution.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.VB.optimize.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      117 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.load.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.move_plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      171 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.initialize_from_value.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.as_diagonal_wishart.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      120 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.plot.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      192 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.get_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.delete.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      249 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateSwitchingMarkovChain.setup.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.set_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      123 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.load.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      132 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.get_mask.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      123 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      195 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.initialize_from_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      201 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.lower_bound_contribution.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      186 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.initialize_from_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      117 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.show.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      171 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.initialize_from_prior.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.move_plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      153 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.get_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      165 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.get_moments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.add_plate_axis.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.SumMultiply.get_shape.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      177 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.unobserve.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      111 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.VB.dot.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      108 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.show.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      198 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.get_riemannian_gradient.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      183 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.set_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.VB.compute_lowerbound_terms.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      114 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gate.delete.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.get_moments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      198 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.lowerbound.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.dims.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      195 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.initialize_from_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.plates_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.has_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      204 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.get_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      204 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.initialize_from_value.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.save.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      138 2016-06-12 17:22:50.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.ConcatGaussian.plot.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      141 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.update.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      120 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.load.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      192 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.initialize_from_value.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.unobserve.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.get_mask.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.logpdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      171 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.initialize_from_value.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      180 2016-06-12 17:22:50.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Function.lower_bound_contribution.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      150 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.unobserve.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      132 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.dims.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      183 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.initialize_from_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      123 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.show.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.get_mask.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      108 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.plot.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      180 2016-06-12 17:22:50.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.ConcatGaussian.plates_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      132 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.set_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      186 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.SumMultiply.broadcasting_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      153 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.observe.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      168 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.logpdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.pdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      177 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.get_riemannian_gradient.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      252 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateSwitchingMarkovChain.rotate.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.VB.has_converged.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.VB.set_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.move_plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      246 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.initialize_from_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      168 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.initialize_from_prior.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      123 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.__init__.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      144 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.get_parameters.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      141 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      153 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.get_gradient.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.logpdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.delete.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      183 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.initialize_from_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      204 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.lower_bound_contribution.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      192 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      123 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.unobserve.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.save.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      171 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.initialize_from_prior.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      168 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.unobserve.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.dims.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.pdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      114 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.pdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.add_plate_axis.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      219 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.get_riemannian_gradient.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.lowerbound.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.add_plate_axis.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      189 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.observe.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.plot.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      162 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.plates_multiplier.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      195 2016-06-12 17:22:50.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.ConcatGaussian.broadcasting_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      162 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.lowerbound.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      186 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.plates_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.unobserve.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      180 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.get_marginal_logpdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      117 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.load.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      168 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.delete.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      117 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gate.plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      120 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.observe.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      159 2016-06-12 17:22:50.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.ConcatGaussian.get_moments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      117 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      222 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.lower_bound_contribution.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      117 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.logpdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.show.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      120 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.plot.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      141 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.rotate.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      153 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.get_gradient.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      129 2016-06-12 17:22:50.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Function.plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.get_mask.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      168 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.initialize_from_prior.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      192 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.broadcasting_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      117 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.load.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      177 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.pdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.show.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      183 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.initialize_from_random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      195 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.plates_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      243 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateVaryingMarkovChain.nodes.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      117 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.get_mask.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.load.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      237 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.get_riemannian_gradient.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      186 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.get_mask.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      120 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.VB.update.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      123 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.logpdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.initialize_from_prior.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.set_parameters.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      168 2016-06-12 17:22:50.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.ConcatGaussian.add_plate_axis.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.update.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      258 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateSwitchingMarkovChain.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      123 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.dims.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      114 2016-01-03 14:57:36.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Take.delete.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      201 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.set_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      153 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.set_parameters.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      144 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.observe.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.show.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      189 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.initialize_from_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.unobserve.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      162 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.save.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.lowerbound.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      165 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.get_mask.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      249 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateSwitchingMarkovChain.bound.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.get_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      132 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.get_gradient.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      162 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.plot.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      222 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateGaussianARD.bound.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      135 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.save.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.update.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      135 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.plot.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      153 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.delete.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      120 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.get_mask.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      222 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateMultiple.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      213 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.initialize_from_prior.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      213 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.get_gaussian_mean_and_variance.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.plot.ContourPlotter.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      117 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.plot.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      117 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.update.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      177 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.get_riemannian_gradient.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      132 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.observe.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.get_moments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.lowerbound.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.save.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      150 2016-06-12 17:22:50.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.ConcatGaussian.__init__.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      189 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.initialize_from_random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      192 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.plot.CategoricalMarkovChainPlotter.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      231 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.get_riemannian_gradient.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      279 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateSwitchingMarkovChain.get_bound_terms.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.get_moments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.delete.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      231 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.initialize_from_value.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.show.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      237 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.broadcasting_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      114 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.logpdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      111 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.plot.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.logpdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 14:57:36.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Take.set_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      177 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.get_shape.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      210 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.get_riemannian_gradient.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      168 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.initialize_from_value.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      168 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.get_gradient.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      153 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.add_plate_axis.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      135 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.show.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.delete.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      177 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.lower_bound_contribution.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      153 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.show.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.logpdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      132 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.get_shape.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.plot.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      195 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.initialize_from_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      132 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.dims.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.get_moments.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      135 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.load.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.pdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      114 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.VB.plot.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      201 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.get_riemannian_gradient.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      168 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gate.lower_bound_contribution.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      168 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.VB.get_iteration_by_nodes.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      120 2016-01-03 14:57:36.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Take.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      216 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateMultiple.rotate.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      183 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.plates_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.logpdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.save.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.SumMultiply.set_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.lowerbound.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.add_plate_axis.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.broadcasting_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      213 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.initialize_from_value.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      111 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.VB.add.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      192 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.initialize_from_prior.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      222 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.plates_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      204 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.set_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.get_shape.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.broadcasting_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.get_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.initialize_from_value.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.set_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.observe.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      153 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.get_gradient.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      132 2016-06-12 17:22:50.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Function.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      222 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.get_gaussian_mean_and_variance.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.set_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.get_shape.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      165 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.has_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      123 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.update.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.get_shape.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      123 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.logpdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.save.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      186 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.initialize_from_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.VB.set_annealing.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      246 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateVaryingMarkovChain.rotate.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      240 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.initialize_from_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      132 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.get_shape.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      132 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.get_moments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.get_shape.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.update.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      243 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateVaryingMarkovChain.setup.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      186 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.broadcasting_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.get_shape.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      192 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.get_riemannian_gradient.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      156 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.has_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.move_plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      132 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.move_plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      168 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      189 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.lower_bound_contribution.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      195 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.get_shape.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      186 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.broadcasting_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gate.plates_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      108 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.load.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      195 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.initialize_from_random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      162 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.has_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      195 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.move_plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.load.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      186 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.rotate.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.update.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      171 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.add_plate_axis.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      123 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.unobserve.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      186 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.plates_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.lowerbound.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      192 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.add_plate_axis.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      195 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.initialize_from_value.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      111 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.load.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      195 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.initialize_from_value.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      141 2016-06-12 17:22:50.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Function.get_moments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      162 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.plates_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      165 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.move_plates.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      126 2016-06-12 17:22:50.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Function.delete.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.add_plate_axis.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      132 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.plates_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      183 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.initialize_from_random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      117 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.save.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 14:57:36.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Take.get_moments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      183 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.get_moments.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      201 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.initialize_from_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.plot.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.lowerbound.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      165 2016-01-03 14:57:36.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Take.broadcasting_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.delete.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.VB.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.observe.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      177 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.lower_bound_contribution.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.lowerbound.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      120 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.pdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      183 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.add_plate_axis.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      210 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.broadcasting_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      246 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateGaussianMarkovChain.bound.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      132 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      153 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.get_gradient.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      177 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.plates_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.VB.set_autosave.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      123 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.update.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      243 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateGaussian.get_bound_terms.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      153 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.save.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      189 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.get_shape.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      159 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.get_gradient.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      171 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.observe.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.SumMultiply.get_mask.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      210 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.add_plate_axis.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.get_shape.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      171 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.get_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.SumMultiply.plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.save.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      219 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.broadcasting_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      120 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gate.get_mask.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.add_plate_axis.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.plot.FunctionPlotter.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.__init__.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      153 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.lowerbound.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      162 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.initialize_from_random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.plates_multiplier.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      177 2016-06-12 17:22:50.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Function.broadcasting_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.set_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.dims.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      192 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.set_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      186 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.lowerbound.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.has_plotter.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      186 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.initialize_from_value.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.initialize_from_value.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      141 2016-06-12 17:22:50.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Function.move_plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.VB.loglikelihood_lowerbound.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      111 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.save.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.add_plate_axis.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      195 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.initialize_from_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.load.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      171 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.initialize_from_random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.logpdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.set_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      186 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.logpdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      117 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.show.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.get_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.lower_bound_contribution.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.move_plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Add.plates_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      165 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.plates_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      123 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.logpdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.logpdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      177 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.broadcasting_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      162 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.lowerbound.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.delete.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      132 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.unobserve.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.logpdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      162 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.observe.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.get_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.initialize_from_prior.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.random.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      141 2016-06-12 17:22:50.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Function.set_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      153 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.get_mask.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.update.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.get_moments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      168 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.get_gradient.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      150 2016-06-12 17:22:50.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Function.add_plate_axis.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      225 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.initialize_from_prior.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      195 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.set_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      123 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.save.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.has_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gate.add_plate_axis.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      120 2016-06-12 17:22:50.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Function.plot.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.set_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      162 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.set_plotter.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      132 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.pdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      171 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.SumMultiply.plates_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      189 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.lower_bound_contribution.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.get_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.VB.get_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.has_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.get_gradient.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.observe.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.get_moments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.get_moments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      156 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.get_shape.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Add.move_plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.lowerbound.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.lowerbound.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.delete.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      114 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.VB.save.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      141 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.delete.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.__init__.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      135 2016-06-12 17:22:50.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Function.get_shape.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.initialize_from_prior.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.observe.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      165 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.get_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      252 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateGaussianARD.get_bound_terms.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.plot.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      198 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.get_gradient.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      156 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.get_mask.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.show.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      153 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.plates_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.observe.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      141 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.logpdf.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      165 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.add_plate_axis.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      159 2016-06-12 17:22:50.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.ConcatGaussian.set_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.plot.PDFPlotter.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.update.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      159 2016-06-12 17:22:50.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.ConcatGaussian.has_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.show.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      201 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.broadcasting_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      156 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.unobserve.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.get_moments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      153 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.load.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.update.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.get_mask.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      255 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateGaussianMarkovChain.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.logpdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.SumMultiply.plot.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      123 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.delete.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.save.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.unobserve.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.plot.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.delete.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      105 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Add.plot.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.show.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      186 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.broadcasting_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      183 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      117 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.plot.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      183 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.lower_bound_contribution.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      186 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.broadcasting_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.get_moments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.get_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.initialize_from_prior.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      222 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.initialize_from_mean_and_covariance.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      114 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.VB.load.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.load.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      186 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.get_riemannian_gradient.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.get_gradient.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      162 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.get_moments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.save.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.plot.HintonPlotter.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      243 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateVaryingMarkovChain.bound.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      165 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.has_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      165 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.get_moments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.move_plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.move_plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.update.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      171 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.lowerbound.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.set_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      117 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.save.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.get_moments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      117 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.save.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      168 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.initialize_from_value.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      132 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.observe.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      120 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.dims.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      231 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.initialize_from_prior.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      156 2016-03-30 08:06:13.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.move_plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      216 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.initialize_from_random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.has_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.SumMultiply.delete.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      165 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.VB.get_gradients.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      165 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.dims.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      186 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.delete.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      123 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.move_plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      177 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.initialize_from_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      249 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateSwitchingMarkovChain.nodes.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Add.has_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      201 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.get_riemannian_gradient.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      198 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.initialize_from_random.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      162 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Add.broadcasting_multiplier.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.has_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      120 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.show.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.update.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gate.set_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.add_plate_axis.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.update.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.unobserve.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.plot.GaussianTimeseriesPlotter.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.load.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      186 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.get_riemannian_gradient.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.add_plate_axis.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.plot.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      201 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.move_plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      186 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.get_riemannian_gradient.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      168 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.update.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      195 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.initialize_from_prior.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      153 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 14:57:36.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Take.move_plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      117 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.plot.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.pdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      132 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.get_mask.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.set_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      132 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.unobserve.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.SumMultiply.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.observe.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.move_plates.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      246 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateGaussianMarkovChain.nodes.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.get_parameters.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.lowerbound.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.has_plotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      117 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Add.__init__.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      120 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.load.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.SumMultiply.get_moments.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      132 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.get_shape.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      213 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateGaussian.bound.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      268 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.plot.PDFPlotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      510 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.inference.vmp.transformations.RotateGaussian.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)       92 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.plot.plot.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1296 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.nodes.Dirichlet.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      537 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.inference.vmp.transformations.RotateGaussianARD.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      288 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.plot.FunctionPlotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1185 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.nodes.Gamma.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1682 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.nodes.GaussianGammaISO.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      280 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.plot.HintonPlotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)       89 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.plot.pdf.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1764 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.nodes.CategoricalMarkovChain.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      328 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.plot.GaussianTimeseriesPlotter.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      806 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.nodes.SumMultiply.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      653 2016-01-03 14:57:36.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.nodes.Take.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      609 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.inference.vmp.transformations.RotateGaussianMarkovChain.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      823 2016-06-12 17:22:50.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.nodes.ConcatGaussian.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      101 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.plot.contour.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1512 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.nodes.GaussianWishart.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1690 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.nodes.GaussianMarkovChain.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1270 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.nodes.Mixture.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1368 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.nodes.Multinomial.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1260 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.nodes.Binomial.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      653 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.nodes.Gate.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)       58 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/bayespy.nodes.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)       70 2016-01-03 11:18:07.000000 bayespy-0.5.8/doc/source/user_api/generated/bayespy.inference.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      213 2015-06-03 09:18:36.000000 bayespy-0.5.8/doc/source/demos.rst
-drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-05-13 09:46:47.000000 bayespy-0.5.8/doc/source/examples/
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)     8023 2015-06-03 09:18:36.000000 bayespy-0.5.8/doc/source/examples/gmm.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)     3617 2015-06-03 09:18:36.000000 bayespy-0.5.8/doc/source/examples/additive_fhmm.rst
--rw-------   0 jluttine  (1000) jluttine  (1000)     6089 2016-08-17 10:33:18.000000 bayespy-0.5.8/doc/source/examples/pca.rst
--rw-------   0 jluttine  (1000) jluttine  (1000)      255 2016-05-04 12:21:07.000000 bayespy-0.5.8/doc/source/examples/examples.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)     8310 2015-06-03 09:18:36.000000 bayespy-0.5.8/doc/source/examples/bmm.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)     8558 2015-09-23 09:36:09.000000 bayespy-0.5.8/doc/source/examples/lda.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)       77 2015-08-17 06:34:53.000000 bayespy-0.5.8/doc/source/examples/my_test.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)    12291 2015-06-03 09:18:36.000000 bayespy-0.5.8/doc/source/examples/hmm.rst
--rw-------   0 jluttine  (1000) jluttine  (1000)    14132 2016-08-17 10:33:18.000000 bayespy-0.5.8/doc/source/examples/lssm.rst
-drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-05-13 09:46:47.000000 bayespy-0.5.8/doc/source/user_guide/
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      173 2015-06-03 09:18:36.000000 bayespy-0.5.8/doc/source/user_guide/install.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      279 2015-06-03 09:18:36.000000 bayespy-0.5.8/doc/source/user_guide/user_guide.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)    20918 2015-06-03 09:18:36.000000 bayespy-0.5.8/doc/source/user_guide/modelconstruct.rst
--rw-------   0 jluttine  (1000) jluttine  (1000)    14269 2016-08-17 10:33:18.000000 bayespy-0.5.8/doc/source/user_guide/inference.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)     5068 2015-06-03 09:18:36.000000 bayespy-0.5.8/doc/source/user_guide/quickstartbackup.rst
--rw-------   0 jluttine  (1000) jluttine  (1000)     5880 2016-05-04 12:21:07.000000 bayespy-0.5.8/doc/source/user_guide/quickstart.rst
--rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     3380 2014-06-12 13:50:13.000000 bayespy-0.5.8/doc/source/user_guide/quickstartbackup.py
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)    14493 2015-06-03 09:18:36.000000 bayespy-0.5.8/doc/source/user_guide/advanced.rst
--rw-------   0 jluttine  (1000) jluttine  (1000)    15602 2016-05-04 12:21:07.000000 bayespy-0.5.8/doc/source/user_guide/plot.rst
--rw-------   0 jluttine  (1000) jluttine  (1000)     7121 2016-05-04 12:21:07.000000 bayespy-0.5.8/doc/Makefile
--rw-------   0 jluttine  (1000) jluttine  (1000)    65747 2016-08-17 10:33:49.000000 bayespy-0.5.8/versioneer.py
--rw-------   0 jluttine  (1000) jluttine  (1000)     5205 2016-05-04 12:21:07.000000 bayespy-0.5.8/README.rst
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)     1090 2015-06-03 09:18:36.000000 bayespy-0.5.8/LICENSE
-drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-05-13 09:46:47.000000 bayespy-0.5.8/bayespy.egg-info/
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)       58 2017-05-13 09:46:46.000000 bayespy-0.5.8/bayespy.egg-info/entry_points.txt
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)        1 2017-05-13 09:46:46.000000 bayespy-0.5.8/bayespy.egg-info/dependency_links.txt
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)     7148 2017-05-13 09:46:46.000000 bayespy-0.5.8/bayespy.egg-info/PKG-INFO
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)        8 2017-05-13 09:46:46.000000 bayespy-0.5.8/bayespy.egg-info/top_level.txt
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)      186 2017-05-13 09:46:46.000000 bayespy-0.5.8/bayespy.egg-info/requires.txt
--rw-r--r--   0 jluttine  (1000) jluttine  (1000)   177993 2017-05-13 09:46:46.000000 bayespy-0.5.8/bayespy.egg-info/SOURCES.txt
--rw-------   0 jluttine  (1000) jluttine  (1000)      400 2017-05-13 09:46:47.000000 bayespy-0.5.8/setup.cfg
+drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-09-02 16:17:21.000000 bayespy-0.5.9/
+-rw-------   0 jluttine  (1000) jluttine  (1000)      314 2016-08-17 10:33:49.000000 bayespy-0.5.9/MANIFEST.in
+-rw-------   0 jluttine  (1000) jluttine  (1000)     7179 2017-09-02 16:17:21.000000 bayespy-0.5.9/PKG-INFO
+-rw-------   0 jluttine  (1000) jluttine  (1000)     6150 2017-01-22 15:43:29.000000 bayespy-0.5.9/INSTALL.rst
+drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-09-02 16:17:21.000000 bayespy-0.5.9/bayespy.egg-info/
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)        8 2017-09-02 16:17:20.000000 bayespy-0.5.9/bayespy.egg-info/top_level.txt
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      186 2017-09-02 16:17:20.000000 bayespy-0.5.9/bayespy.egg-info/requires.txt
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)     7179 2017-09-02 16:17:20.000000 bayespy-0.5.9/bayespy.egg-info/PKG-INFO
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)       58 2017-09-02 16:17:20.000000 bayespy-0.5.9/bayespy.egg-info/entry_points.txt
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)        1 2017-09-02 16:17:20.000000 bayespy-0.5.9/bayespy.egg-info/dependency_links.txt
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)   177993 2017-09-02 16:17:20.000000 bayespy-0.5.9/bayespy.egg-info/SOURCES.txt
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)     1090 2015-06-03 09:18:36.000000 bayespy-0.5.9/LICENSE
+-rw-------   0 jluttine  (1000) jluttine  (1000)     5220 2017-09-02 16:06:14.000000 bayespy-0.5.9/README.rst
+drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-09-02 16:17:21.000000 bayespy-0.5.9/bayespy/
+-rw-------   0 jluttine  (1000) jluttine  (1000)    37379 2017-09-02 16:06:14.000000 bayespy-0.5.9/bayespy/plot.py
+-rw-------   0 jluttine  (1000) jluttine  (1000)     1997 2016-05-04 12:21:07.000000 bayespy-0.5.9/bayespy/testing.py
+drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-09-02 16:17:21.000000 bayespy-0.5.9/bayespy/models/
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     2891 2016-03-21 09:17:48.000000 bayespy-0.5.9/bayespy/models/pca.py
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)       21 2016-02-11 08:24:32.000000 bayespy-0.5.9/bayespy/models/__init__.py
+drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-09-02 16:17:21.000000 bayespy-0.5.9/bayespy/utils/
+drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-09-02 16:17:21.000000 bayespy-0.5.9/bayespy/utils/covfunc/
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)        0 2013-07-24 18:00:26.000000 bayespy-0.5.9/bayespy/utils/covfunc/__init__.py
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)    11412 2015-06-03 09:18:36.000000 bayespy-0.5.9/bayespy/utils/covfunc/covariance.py
+drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-09-02 16:17:21.000000 bayespy-0.5.9/bayespy/utils/tests/
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)     6200 2015-11-02 11:23:25.000000 bayespy-0.5.9/bayespy/utils/tests/test_linalg.py
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)        0 2013-07-24 18:00:26.000000 bayespy-0.5.9/bayespy/utils/tests/__init__.py
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)    17119 2017-01-19 07:35:06.000000 bayespy-0.5.9/bayespy/utils/tests/test_misc.py
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)     9697 2015-11-02 11:23:25.000000 bayespy-0.5.9/bayespy/utils/tests/test_random.py
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      339 2015-06-03 09:18:36.000000 bayespy-0.5.9/bayespy/utils/__init__.py
+-rw-------   0 jluttine  (1000) jluttine  (1000)    17933 2017-01-22 15:43:29.000000 bayespy-0.5.9/bayespy/utils/linalg.py
+-rw-------   0 jluttine  (1000) jluttine  (1000)    44791 2017-01-22 15:43:29.000000 bayespy-0.5.9/bayespy/utils/misc.py
+-rw-------   0 jluttine  (1000) jluttine  (1000)    11769 2016-05-04 12:21:07.000000 bayespy-0.5.9/bayespy/utils/random.py
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)     1566 2015-11-02 11:23:25.000000 bayespy-0.5.9/bayespy/utils/optimize.py
+drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-09-02 16:17:21.000000 bayespy-0.5.9/bayespy/tests/
+drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-09-02 16:17:21.000000 bayespy-0.5.9/bayespy/tests/baseline_images/
+drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-09-02 16:17:21.000000 bayespy-0.5.9/bayespy/tests/baseline_images/test_plot/
+-rw-------   0 jluttine  (1000) jluttine  (1000)    56291 2017-09-02 16:06:14.000000 bayespy-0.5.9/bayespy/tests/baseline_images/test_plot/contour.png
+-rw-------   0 jluttine  (1000) jluttine  (1000)     8322 2016-05-04 12:21:07.000000 bayespy-0.5.9/bayespy/tests/baseline_images/test_plot/hinton_z.png
+-rw-------   0 jluttine  (1000) jluttine  (1000)     7439 2016-05-04 12:21:07.000000 bayespy-0.5.9/bayespy/tests/baseline_images/test_plot/hinton_p.png
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)    14971 2015-02-24 08:36:24.000000 bayespy-0.5.9/bayespy/tests/baseline_images/test_plot/pdf.png
+-rw-------   0 jluttine  (1000) jluttine  (1000)     3769 2016-05-04 12:21:07.000000 bayespy-0.5.9/bayespy/tests/baseline_images/test_plot/hinton_r.png
+-rw-------   0 jluttine  (1000) jluttine  (1000)    36488 2017-09-02 16:06:14.000000 bayespy-0.5.9/bayespy/tests/baseline_images/test_plot/gaussian_mixture.png
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      393 2015-10-30 13:13:53.000000 bayespy-0.5.9/bayespy/tests/__init__.py
+-rw-------   0 jluttine  (1000) jluttine  (1000)     5444 2017-09-02 16:06:14.000000 bayespy-0.5.9/bayespy/tests/test_plot.py
+drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-09-02 16:17:21.000000 bayespy-0.5.9/bayespy/nodes/
+-rw-------   0 jluttine  (1000) jluttine  (1000)     1729 2016-05-04 12:21:07.000000 bayespy-0.5.9/bayespy/nodes/__init__.py
+-rw-------   0 jluttine  (1000) jluttine  (1000)      502 2017-01-22 17:35:50.000000 bayespy-0.5.9/bayespy/nodes/gaussian.py
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      502 2016-08-17 16:45:23.000000 bayespy-0.5.9/bayespy/__init__.py
+drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-09-02 16:17:21.000000 bayespy-0.5.9/bayespy/demos/
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)     4839 2015-06-03 09:18:36.000000 bayespy-0.5.9/bayespy/demos/hmm.py
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      907 2015-06-03 09:18:36.000000 bayespy-0.5.9/bayespy/demos/categorical.py
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)     4657 2015-06-03 09:18:36.000000 bayespy-0.5.9/bayespy/demos/pca.py
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)    10690 2015-06-03 09:18:36.000000 bayespy-0.5.9/bayespy/demos/lssm.py
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)     5013 2015-06-03 09:18:36.000000 bayespy-0.5.9/bayespy/demos/stochastic_inference.py
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)    10707 2015-06-09 10:01:58.000000 bayespy-0.5.9/bayespy/demos/lssm_sd.py
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)     3332 2015-06-03 09:18:36.000000 bayespy-0.5.9/bayespy/demos/annealing.py
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)     7241 2015-06-15 21:10:51.000000 bayespy-0.5.9/bayespy/demos/lda.py
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)     4028 2015-06-03 09:18:36.000000 bayespy-0.5.9/bayespy/demos/saving.py
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)    14726 2015-06-03 09:18:36.000000 bayespy-0.5.9/bayespy/demos/lssm_tvd.py
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)        0 2015-06-03 09:18:36.000000 bayespy-0.5.9/bayespy/demos/__init__.py
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)     3944 2015-06-09 10:31:05.000000 bayespy-0.5.9/bayespy/demos/pattern_search.py
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)     3284 2015-06-09 09:48:54.000000 bayespy-0.5.9/bayespy/demos/collapsed_cg.py
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)     3429 2015-06-03 09:18:36.000000 bayespy-0.5.9/bayespy/demos/black_box.py
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      484 2015-07-31 11:15:05.000000 bayespy-0.5.9/bayespy/demos/gamma_shape.py
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)     3110 2015-06-03 09:18:36.000000 bayespy-0.5.9/bayespy/demos/mog.py
+-rw-------   0 jluttine  (1000) jluttine  (1000)      471 2017-09-02 16:17:21.000000 bayespy-0.5.9/bayespy/_version.py
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)     1910 2015-11-02 11:23:25.000000 bayespy-0.5.9/bayespy/discrete_example.py
+-rw-------   0 jluttine  (1000) jluttine  (1000)      168 2017-09-02 16:06:14.000000 bayespy-0.5.9/bayespy/_meta.py
+drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-09-02 16:17:21.000000 bayespy-0.5.9/bayespy/inference/
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      799 2015-06-03 09:18:36.000000 bayespy-0.5.9/bayespy/inference/__init__.py
+drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-09-02 16:17:21.000000 bayespy-0.5.9/bayespy/inference/vmp/
+-rw-------   0 jluttine  (1000) jluttine  (1000)    24028 2017-09-02 16:06:14.000000 bayespy-0.5.9/bayespy/inference/vmp/vmp.py
+drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-09-02 16:17:21.000000 bayespy-0.5.9/bayespy/inference/vmp/tests/
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)    42154 2015-11-02 11:23:25.000000 bayespy-0.5.9/bayespy/inference/vmp/tests/test_transformations.py
+-rw-------   0 jluttine  (1000) jluttine  (1000)     3211 2016-05-04 12:21:07.000000 bayespy-0.5.9/bayespy/inference/vmp/tests/test_annealing.py
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)        0 2013-07-24 18:00:26.000000 bayespy-0.5.9/bayespy/inference/vmp/tests/__init__.py
+drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-09-02 16:17:21.000000 bayespy-0.5.9/bayespy/inference/vmp/nodes/
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)    28645 2015-06-03 09:18:36.000000 bayespy-0.5.9/bayespy/inference/vmp/nodes/CovarianceFunctions.py
+-rw-------   0 jluttine  (1000) jluttine  (1000)     5541 2016-05-04 12:21:07.000000 bayespy-0.5.9/bayespy/inference/vmp/nodes/categorical.py
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)    23431 2015-06-03 09:18:36.000000 bayespy-0.5.9/bayespy/inference/vmp/nodes/gp.py
+-rw-------   0 jluttine  (1000) jluttine  (1000)    10709 2017-01-22 15:43:29.000000 bayespy-0.5.9/bayespy/inference/vmp/nodes/gamma.py
+-rw-------   0 jluttine  (1000) jluttine  (1000)    47354 2017-01-22 15:43:29.000000 bayespy-0.5.9/bayespy/inference/vmp/nodes/node.py
+-rw-------   0 jluttine  (1000) jluttine  (1000)     6038 2016-05-04 12:21:07.000000 bayespy-0.5.9/bayespy/inference/vmp/nodes/binomial.py
+-rw-------   0 jluttine  (1000) jluttine  (1000)     4426 2016-05-04 12:21:07.000000 bayespy-0.5.9/bayespy/inference/vmp/nodes/add.py
+-rw-------   0 jluttine  (1000) jluttine  (1000)     8011 2016-05-04 12:21:07.000000 bayespy-0.5.9/bayespy/inference/vmp/nodes/gate.py
+-rw-------   0 jluttine  (1000) jluttine  (1000)     9550 2017-01-22 15:43:29.000000 bayespy-0.5.9/bayespy/inference/vmp/nodes/wishart.py
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)    21001 2017-01-19 07:35:06.000000 bayespy-0.5.9/bayespy/inference/vmp/nodes/mixture.py
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)     8964 2017-01-19 07:35:06.000000 bayespy-0.5.9/bayespy/inference/vmp/nodes/multinomial.py
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)    11102 2017-01-19 07:35:06.000000 bayespy-0.5.9/bayespy/inference/vmp/nodes/dirichlet.py
+-rw-------   0 jluttine  (1000) jluttine  (1000)     5955 2016-05-04 12:21:07.000000 bayespy-0.5.9/bayespy/inference/vmp/nodes/concatenate.py
+-rw-------   0 jluttine  (1000) jluttine  (1000)      543 2016-11-13 18:28:47.000000 bayespy-0.5.9/bayespy/inference/vmp/nodes/multinomial_probit.py
+drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-09-02 16:17:21.000000 bayespy-0.5.9/bayespy/inference/vmp/nodes/tests/
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)     5319 2017-01-19 07:35:06.000000 bayespy-0.5.9/bayespy/inference/vmp/nodes/tests/test_multinomial.py
+-rw-------   0 jluttine  (1000) jluttine  (1000)    34034 2016-05-04 12:21:07.000000 bayespy-0.5.9/bayespy/inference/vmp/nodes/tests/test_node.py
+-rw-------   0 jluttine  (1000) jluttine  (1000)    12835 2017-01-22 15:43:29.000000 bayespy-0.5.9/bayespy/inference/vmp/nodes/tests/test_mixture.py
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)     2291 2015-11-02 11:23:25.000000 bayespy-0.5.9/bayespy/inference/vmp/nodes/tests/test_dirichlet.py
+-rw-------   0 jluttine  (1000) jluttine  (1000)     5599 2016-05-04 12:21:07.000000 bayespy-0.5.9/bayespy/inference/vmp/nodes/tests/test_gamma.py
+-rw-------   0 jluttine  (1000) jluttine  (1000)    31570 2016-05-04 12:21:07.000000 bayespy-0.5.9/bayespy/inference/vmp/nodes/tests/test_dot.py
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)     2667 2015-11-02 11:23:25.000000 bayespy-0.5.9/bayespy/inference/vmp/nodes/tests/test_beta.py
+-rw-------   0 jluttine  (1000) jluttine  (1000)     7079 2016-05-04 12:21:07.000000 bayespy-0.5.9/bayespy/inference/vmp/nodes/tests/test_categorical.py
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)     3781 2015-11-02 11:23:25.000000 bayespy-0.5.9/bayespy/inference/vmp/nodes/tests/test_wishart.py
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)     2500 2015-11-02 11:23:25.000000 bayespy-0.5.9/bayespy/inference/vmp/nodes/tests/test_poisson.py
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)        0 2014-05-03 08:22:08.000000 bayespy-0.5.9/bayespy/inference/vmp/nodes/tests/__init__.py
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)     5069 2015-11-02 11:23:25.000000 bayespy-0.5.9/bayespy/inference/vmp/nodes/tests/test_binomial.py
+-rw-------   0 jluttine  (1000) jluttine  (1000)    11503 2016-05-04 12:21:07.000000 bayespy-0.5.9/bayespy/inference/vmp/nodes/tests/test_deterministic.py
+-rw-------   0 jluttine  (1000) jluttine  (1000)    10082 2017-01-22 15:43:29.000000 bayespy-0.5.9/bayespy/inference/vmp/nodes/tests/test_concatenate.py
+-rw-------   0 jluttine  (1000) jluttine  (1000)    50883 2017-01-22 15:43:29.000000 bayespy-0.5.9/bayespy/inference/vmp/nodes/tests/test_gaussian.py
+-rw-------   0 jluttine  (1000) jluttine  (1000)    10768 2016-05-04 12:21:07.000000 bayespy-0.5.9/bayespy/inference/vmp/nodes/tests/test_gate.py
+-rw-------   0 jluttine  (1000) jluttine  (1000)    12147 2017-01-22 15:43:29.000000 bayespy-0.5.9/bayespy/inference/vmp/nodes/tests/test_take.py
+-rw-------   0 jluttine  (1000) jluttine  (1000)    38334 2017-01-22 15:43:29.000000 bayespy-0.5.9/bayespy/inference/vmp/nodes/tests/test_gaussian_markov_chain.py
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)     7353 2015-11-02 11:23:25.000000 bayespy-0.5.9/bayespy/inference/vmp/nodes/tests/test_categorical_markov_chain.py
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)     3550 2015-11-02 11:23:25.000000 bayespy-0.5.9/bayespy/inference/vmp/nodes/tests/test_bernoulli.py
+-rw-------   0 jluttine  (1000) jluttine  (1000)    13538 2016-05-04 12:21:07.000000 bayespy-0.5.9/bayespy/inference/vmp/nodes/categorical_markov_chain.py
+-rw-------   0 jluttine  (1000) jluttine  (1000)     2796 2017-01-22 15:43:29.000000 bayespy-0.5.9/bayespy/inference/vmp/nodes/constant.py
+-rw-------   0 jluttine  (1000) jluttine  (1000)     1544 2017-01-22 15:43:29.000000 bayespy-0.5.9/bayespy/inference/vmp/nodes/__init__.py
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)    25953 2015-06-03 09:18:36.000000 bayespy-0.5.9/bayespy/inference/vmp/nodes/GaussianProcesses.py
+-rw-------   0 jluttine  (1000) jluttine  (1000)    11968 2017-01-22 15:43:29.000000 bayespy-0.5.9/bayespy/inference/vmp/nodes/deterministic.py
+-rw-------   0 jluttine  (1000) jluttine  (1000)    21428 2017-01-22 15:43:29.000000 bayespy-0.5.9/bayespy/inference/vmp/nodes/dot.py
+-rw-------   0 jluttine  (1000) jluttine  (1000)     5228 2016-05-04 12:21:07.000000 bayespy-0.5.9/bayespy/inference/vmp/nodes/point_estimate.py
+-rw-------   0 jluttine  (1000) jluttine  (1000)     3991 2017-05-13 09:44:22.000000 bayespy-0.5.9/bayespy/inference/vmp/nodes/poisson.py
+-rw-------   0 jluttine  (1000) jluttine  (1000)     5448 2016-11-04 16:38:16.000000 bayespy-0.5.9/bayespy/inference/vmp/nodes/newnode.py
+-rw-------   0 jluttine  (1000) jluttine  (1000)    74001 2017-01-22 15:43:29.000000 bayespy-0.5.9/bayespy/inference/vmp/nodes/gaussian_markov_chain.py
+-rw-------   0 jluttine  (1000) jluttine  (1000)     4426 2017-01-22 15:43:29.000000 bayespy-0.5.9/bayespy/inference/vmp/nodes/take.py
+-rw-------   0 jluttine  (1000) jluttine  (1000)     3889 2017-01-22 15:43:29.000000 bayespy-0.5.9/bayespy/inference/vmp/nodes/concat_gaussian.py
+-rw-------   0 jluttine  (1000) jluttine  (1000)    18343 2017-01-22 15:43:29.000000 bayespy-0.5.9/bayespy/inference/vmp/nodes/expfamily.py
+-rw-------   0 jluttine  (1000) jluttine  (1000)     6069 2017-05-13 09:44:22.000000 bayespy-0.5.9/bayespy/inference/vmp/nodes/logistic.py
+-rw-------   0 jluttine  (1000) jluttine  (1000)     3066 2016-05-04 12:21:07.000000 bayespy-0.5.9/bayespy/inference/vmp/nodes/logpdf.py
+-rw-------   0 jluttine  (1000) jluttine  (1000)     5584 2016-05-04 12:21:07.000000 bayespy-0.5.9/bayespy/inference/vmp/nodes/ml.py
+-rw-------   0 jluttine  (1000) jluttine  (1000)     4418 2016-05-04 12:21:07.000000 bayespy-0.5.9/bayespy/inference/vmp/nodes/bernoulli.py
+-rw-------   0 jluttine  (1000) jluttine  (1000)     1557 2016-05-04 12:21:07.000000 bayespy-0.5.9/bayespy/inference/vmp/nodes/converters.py
+-rw-------   0 jluttine  (1000) jluttine  (1000)    80752 2017-01-22 15:43:29.000000 bayespy-0.5.9/bayespy/inference/vmp/nodes/gaussian.py
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)     2137 2015-06-03 09:18:36.000000 bayespy-0.5.9/bayespy/inference/vmp/nodes/exponential.py
+-rw-------   0 jluttine  (1000) jluttine  (1000)     5230 2016-05-04 12:21:07.000000 bayespy-0.5.9/bayespy/inference/vmp/nodes/beta.py
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)    11461 2017-01-19 07:35:06.000000 bayespy-0.5.9/bayespy/inference/vmp/nodes/stochastic.py
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)        0 2013-07-24 18:00:26.000000 bayespy-0.5.9/bayespy/inference/vmp/__init__.py
+-rw-------   0 jluttine  (1000) jluttine  (1000)    59456 2016-05-04 12:21:07.000000 bayespy-0.5.9/bayespy/inference/vmp/transformations.py
+-rw-------   0 jluttine  (1000) jluttine  (1000)    65747 2016-08-17 10:33:49.000000 bayespy-0.5.9/versioneer.py
+drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-09-02 16:17:21.000000 bayespy-0.5.9/doc/
+-rw-------   0 jluttine  (1000) jluttine  (1000)     7121 2016-05-04 12:21:07.000000 bayespy-0.5.9/doc/Makefile
+drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-09-02 16:17:21.000000 bayespy-0.5.9/doc/source/
+drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-09-02 16:17:21.000000 bayespy-0.5.9/doc/source/examples/
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)       77 2015-08-17 06:34:53.000000 bayespy-0.5.9/doc/source/examples/my_test.rst
+-rw-------   0 jluttine  (1000) jluttine  (1000)    14132 2016-08-17 10:33:18.000000 bayespy-0.5.9/doc/source/examples/lssm.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)     8310 2015-06-03 09:18:36.000000 bayespy-0.5.9/doc/source/examples/bmm.rst
+-rw-------   0 jluttine  (1000) jluttine  (1000)      255 2016-05-04 12:21:07.000000 bayespy-0.5.9/doc/source/examples/examples.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)     8558 2015-09-23 09:36:09.000000 bayespy-0.5.9/doc/source/examples/lda.rst
+-rw-------   0 jluttine  (1000) jluttine  (1000)     6089 2016-08-17 10:33:18.000000 bayespy-0.5.9/doc/source/examples/pca.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)     3617 2015-06-03 09:18:36.000000 bayespy-0.5.9/doc/source/examples/additive_fhmm.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)    12291 2015-06-03 09:18:36.000000 bayespy-0.5.9/doc/source/examples/hmm.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)     8023 2015-06-03 09:18:36.000000 bayespy-0.5.9/doc/source/examples/gmm.rst
+drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-09-02 16:17:21.000000 bayespy-0.5.9/doc/source/_templates/
+drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-09-02 16:17:21.000000 bayespy-0.5.9/doc/source/_templates/autosummary/
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      716 2014-07-07 08:35:29.000000 bayespy-0.5.9/doc/source/_templates/autosummary/module.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      581 2014-07-07 08:35:29.000000 bayespy-0.5.9/doc/source/_templates/autosummary/class.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)       63 2014-07-07 08:35:29.000000 bayespy-0.5.9/doc/source/_templates/autosummary/short_module.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      283 2015-06-03 09:18:36.000000 bayespy-0.5.9/doc/source/intro.rst
+drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-09-02 16:17:21.000000 bayespy-0.5.9/doc/source/dev_api/
+drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-09-02 16:17:21.000000 bayespy-0.5.9/doc/source/dev_api/generated/
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1634 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/bayespy.utils.misc.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      611 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.GaussianMarkovChainMoments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      241 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/bayespy.utils.optimize.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      812 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.beta.BetaDistribution.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      427 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.node.Moments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      505 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.dirichlet.DirichletMoments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1011 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianWishart.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      935 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.bernoulli.BernoulliDistribution.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1175 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.categorical_markov_chain.CategoricalMarkovChainDistribution.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      485 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.wishart.WishartMoments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      538 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.bernoulli.BernoulliMoments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      863 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.poisson.PoissonDistribution.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      485 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.poisson.PoissonMoments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      687 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.categorical_markov_chain.CategoricalMarkovChainMoments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1121 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.GaussianMarkovChainDistribution.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      890 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.deterministic.Deterministic.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      581 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/bayespy.utils.random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      591 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDMoments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1096 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGammaISO.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      525 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.multinomial.MultinomialMoments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      880 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianDistribution.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1028 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaARD.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1232 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISOToGaussianGammaARD.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      465 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gamma.GammaMoments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      527 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianMoments.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)     1045 2016-03-30 08:06:12.000000 bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGamma.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      971 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.multinomial.MultinomialDistribution.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      978 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianWishartDistribution.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      520 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.stochastic.Distribution.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      544 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianWishartMoments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      897 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.dirichlet.DirichletDistribution.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)     1164 2016-03-30 08:06:12.000000 bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaToGaussianWishart.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1028 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaISO.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1256 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.SwitchingGaussianMarkovChainDistribution.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      989 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.stochastic.Stochastic.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      455 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.beta.BetaMoments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      673 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.node.Node.rst
+drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-09-02 16:17:21.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      152 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.m_solve_triangular.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      279 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.wishart.WishartDistribution.compute_phi_from_parents.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      243 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaISO.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      252 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaARD.move_plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      267 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.bernoulli.BernoulliDistribution.plates_to_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      125 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.m_digamma.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      140 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.dist_haversine.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      146 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.axes_to_collapse.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      279 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.multinomial.MultinomialDistribution.plates_to_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      110 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.mean.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      249 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.set_parameters.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      300 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaDistribution.compute_phi_from_parents.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      285 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamilyDistribution.compute_logpdf.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      303 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaDistribution.compute_message_to_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      113 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.trues.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      201 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.node.Moments.add_converter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      225 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.logpdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      110 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.grid.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      375 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical_markov_chain.CategoricalMarkovChainDistribution.compute_cgf_from_parents.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      276 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaDistribution.compute_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      243 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gamma.GammaDistribution.compute_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      372 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical_markov_chain.CategoricalMarkovChainDistribution.compute_moments_and_cgf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      195 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.node.Node.add_plate_axis.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      327 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISOToGaussianGammaARD.lower_bound_contribution.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      210 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.constant.Constant.has_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      222 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.stochastic.Stochastic.has_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      128 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.atleast_nd.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      288 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.dirichlet.DirichletDistribution.compute_moments_and_cgf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      240 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.deterministic.Deterministic.has_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      285 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISOMoments.compute_fixed_moments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      303 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.multinomial.MultinomialDistribution.compute_phi_from_parents.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      249 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.get_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      270 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gamma.GammaDistribution.compute_message_to_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      261 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.binomial.BinomialDistribution.plates_to_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      330 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.VaryingGaussianMarkovChainDistribution.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      270 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.initialize_from_prior.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      216 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.stochastic.Stochastic.get_shape.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      240 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGamma.delete.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      279 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.poisson.PoissonDistribution.compute_cgf_from_parents.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      243 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.dirichlet.DirichletMoments.get_converter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      288 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaISO.broadcasting_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      279 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical.CategoricalMoments.compute_fixed_moments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      128 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.is_numeric.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      294 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.bernoulli.BernoulliDistribution.compute_message_to_parent.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      300 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaDistribution.compute_cgf_from_parents.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      288 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaARD.broadcasting_multiplier.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      237 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaMoments.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      255 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.multinomial.MultinomialMoments.get_converter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      294 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDMoments.compute_dims_from_values.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      273 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.initialize_from_random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      324 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISOToGaussianGammaARD.broadcasting_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      255 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical.CategoricalMoments.get_converter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      270 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.beta.BetaDistribution.compute_fixed_moments_and_f.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      348 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.VaryingGaussianMarkovChainDistribution.compute_logpdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      170 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.random.logodds_to_probability.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      237 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.beta.BetaDistribution.compute_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      312 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical_markov_chain.CategoricalMarkovChainMoments.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      279 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical.CategoricalDistribution.plates_to_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      306 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical.CategoricalDistribution.compute_weights_to_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      378 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical_markov_chain.CategoricalMarkovChainDistribution.compute_weights_to_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      384 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.SwitchingGaussianMarkovChainDistribution.compute_cgf_from_parents.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      264 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGammaISO.set_plotter.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      270 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaDistribution.compute_logpdf.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      255 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGamma.has_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      267 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISOToGaussianGammaARD.plot.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      131 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.linalg.transpose.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      303 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaMoments.get_instance_conversion_kwargs.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      255 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical.CategoricalMoments.add_converter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      276 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianARDDistribution.plates_from_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      246 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaISO.get_shape.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      303 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.multinomial.MultinomialDistribution.compute_cgf_from_parents.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      164 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.random.alpha_beta_recursion.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      246 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaARD.get_shape.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      282 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGamma.lower_bound_contribution.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      288 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.binomial.BinomialDistribution.compute_message_to_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      387 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.SwitchingGaussianMarkovChainDistribution.compute_message_to_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      219 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.constant.Constant.add_plate_axis.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      231 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.binomial.BinomialDistribution.random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      309 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.GaussianMarkovChainMoments.add_converter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      143 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.multiply_shapes.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      306 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.multinomial.MultinomialDistribution.compute_weights_to_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      149 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.broadcasted_shape.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      201 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.stochastic.Stochastic.save.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      243 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.beta.BetaDistribution.plates_from_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      351 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical_markov_chain.CategoricalMarkovChainMoments.compute_fixed_moments.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      231 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGamma.plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      134 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.linalg.logdet_cov.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      333 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.GaussianMarkovChainDistribution.plates_to_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      273 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaARD.plates_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      101 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.T.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      276 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDToGaussianWishart.get_mask.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      312 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISODistribution.compute_message_to_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      231 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.deterministic.Deterministic.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      125 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.random.wishart.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      261 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaARD.add_plate_axis.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      131 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.chol_logdet.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      131 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.random.dirichlet.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      125 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.is_string.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      237 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gamma.GammaDistribution.compute_logpdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      252 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianWishartDistribution.random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      360 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.SwitchingGaussianMarkovChainDistribution.compute_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      128 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.sum_to_dim.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      261 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianMoments.compute_fixed_moments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      321 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical_markov_chain.CategoricalMarkovChainDistribution.random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      282 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.wishart.WishartDistribution.compute_message_to_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      228 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.bernoulli.BernoulliMoments.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      252 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gamma.GammaMoments.compute_dims_from_values.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      279 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaMoments.get_instance_converter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      279 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.multinomial.MultinomialDistribution.compute_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      258 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.beta.BetaDistribution.compute_moments_and_cgf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      113 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.random.svd.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      261 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.dirichlet.DirichletDistribution.compute_logpdf.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      246 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGamma.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      276 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.get_riemannian_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      128 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.random.t_logpdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      384 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical_markov_chain.CategoricalMarkovChainDistribution.compute_fixed_moments_and_f.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      237 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaARD.delete.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      291 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianWishartMoments.compute_dims_from_values.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      276 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gamma.GammaDistribution.compute_fixed_moments_and_f.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      122 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.chol_inv.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      119 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.linalg.mvdot.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      134 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.block_banded.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      285 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianDistribution.compute_cgf_from_parents.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      213 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.stochastic.Distribution.random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      225 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.node.Moments.compute_fixed_moments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      255 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.wishart.WishartDistribution.compute_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      231 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaARD.plot.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      357 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical_markov_chain.CategoricalMarkovChainDistribution.plates_from_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      285 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDMoments.compute_fixed_moments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      231 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.poisson.PoissonMoments.get_converter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      294 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDToGaussianWishart.add_plate_axis.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      303 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaDistribution.compute_weights_to_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      282 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.poisson.PoissonDistribution.compute_weights_to_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      237 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.dirichlet.DirichletDistribution.random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      378 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.VaryingGaussianMarkovChainDistribution.compute_cgf_from_parents.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      107 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.put.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      309 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaDistribution.compute_fixed_moments_and_f.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      357 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.GaussianMarkovChainDistribution.compute_cgf_from_parents.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      122 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.add_axes.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      258 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianWishart.add_plate_axis.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      279 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.lower_bound_contribution.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      258 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianWishartMoments.get_converter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      276 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDToGaussianWishart.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      267 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.dirichlet.DirichletMoments.compute_fixed_moments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      330 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.SwitchingGaussianMarkovChainDistribution.random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      119 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.ceildiv.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      276 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.broadcasting_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      306 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDToGaussianWishart.plates_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      387 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.SwitchingGaussianMarkovChainDistribution.compute_weights_to_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      152 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.random.gaussian_entropy.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      243 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.bernoulli.BernoulliMoments.add_converter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      122 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.cholesky.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      267 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.bernoulli.BernoulliDistribution.compute_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      303 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical.CategoricalDistribution.compute_cgf_from_parents.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      261 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianDistribution.compute_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      213 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.stochastic.Stochastic.get_mask.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      264 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGamma.add_plate_axis.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      237 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.lowerbound.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      264 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.wishart.WishartMoments.compute_dims_from_values.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      152 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.optimize.check_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      327 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.GaussianMarkovChainDistribution.compute_logpdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      279 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical.CategoricalDistribution.compute_gradient.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      252 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaMoments.add_converter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      291 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamilyDistribution.plates_to_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      285 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDToGaussianWishart.get_moments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      134 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.sum_to_shape.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      270 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianARDDistribution.compute_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      273 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGammaISO.add_plate_axis.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      291 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaARD.lower_bound_contribution.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      327 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical_markov_chain.CategoricalMarkovChainMoments.get_converter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      375 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical_markov_chain.CategoricalMarkovChainDistribution.compute_phi_from_parents.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      309 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.GaussianMarkovChainMoments.get_converter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      240 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.deterministic.Deterministic.set_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      306 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical.CategoricalDistribution.compute_message_to_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      113 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.m_dot.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      285 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaToGaussianWishart.add_plate_axis.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      228 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGamma.delete.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      264 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGamma.plates_multiplier.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      267 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaToGaussianWishart.get_mask.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      131 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.random.bernoulli.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      122 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.diagonal.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      264 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.beta.BetaDistribution.compute_message_to_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      255 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianDistribution.compute_logpdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      240 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.deterministic.Deterministic.get_moments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      291 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.bernoulli.BernoulliDistribution.compute_phi_from_parents.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      249 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianWishart.set_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      243 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaARD.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      152 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.linalg.solve_triangular.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      219 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gamma.GammaMoments.get_converter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      261 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.binomial.BinomialMoments.compute_fixed_moments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      231 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianDistribution.random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      113 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.linalg.dot.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      119 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.squeeze.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      261 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.plates_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      279 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISODistribution.compute_logpdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      288 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianWishartDistribution.plates_from_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      288 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISOToGaussianGammaARD.set_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      240 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.set_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      351 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical_markov_chain.CategoricalMarkovChainDistribution.plates_to_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      270 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.stochastic.Distribution.compute_message_to_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      234 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianWishart.delete.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      387 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.VaryingGaussianMarkovChainDistribution.compute_fixed_moments_and_f.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      231 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.get_mask.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      128 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.linalg.tracedot.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      243 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGamma.plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      143 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.gaussian_logpdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      273 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISOToGaussianGammaARD.delete.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      149 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.random.gaussian_logpdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      312 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDDistribution.compute_message_to_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      210 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.constant.Constant.move_plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      210 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.stochastic.Stochastic.observe.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      273 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.multinomial.MultinomialDistribution.compute_logpdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      249 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.poisson.PoissonDistribution.compute_logpdf.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      315 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaToGaussianWishart.lower_bound_contribution.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      195 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.constant.Constant.delete.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      231 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.wishart.WishartMoments.add_converter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      228 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.observe.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      255 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGammaISO.get_mask.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      276 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaMoments.compute_fixed_moments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      282 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianWishartDistribution.plates_to_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      264 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianARDDistribution.compute_logpdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      312 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDDistribution.compute_weights_to_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      246 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianARDDistribution.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      261 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISOMoments.get_converter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      285 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.multinomial.MultinomialDistribution.plates_from_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      201 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.constant.Constant.get_mask.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      213 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gamma.GammaDistribution.random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      303 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.GaussianMarkovChainDistribution.random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      243 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.stochastic.Stochastic.plates_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      395 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.CholeskyDense.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      240 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianARDDistribution.random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      143 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.make_equal_ndim.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      237 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaISO.delete.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      393 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.SwitchingGaussianMarkovChainDistribution.compute_fixed_moments_and_f.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      279 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.deterministic.Deterministic.lower_bound_contribution.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      225 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      375 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.VaryingGaussianMarkovChainDistribution.compute_moments_and_cgf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      282 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.binomial.BinomialDistribution.compute_moments_and_cgf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      231 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.constant.Constant.plates_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      270 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianARDDistribution.plates_to_parent.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      276 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaToGaussianWishart.has_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      324 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDToGaussianWishart.lower_bound_contribution.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      255 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.multinomial.MultinomialMoments.add_converter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      261 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.wishart.WishartDistribution.plates_from_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      291 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaISO.lower_bound_contribution.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      285 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDToGaussianWishart.set_plotter.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      279 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGamma.broadcasting_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      333 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.GaussianMarkovChainDistribution.compute_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      354 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.SwitchingGaussianMarkovChainDistribution.compute_logpdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      198 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.constant.Constant.plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      351 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical_markov_chain.CategoricalMarkovChainDistribution.compute_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      324 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.VaryingGaussianMarkovChainDistribution.random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      294 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.binomial.BinomialDistribution.compute_fixed_moments_and_f.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      149 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.remove_whitespace.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      285 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianWishart.broadcasting_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      309 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDDistribution.compute_cgf_from_parents.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      282 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianWishartDistribution.compute_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      303 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical.CategoricalDistribution.compute_phi_from_parents.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      204 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.constant.Constant.set_value.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      143 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.is_shape_subset.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      300 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.dirichlet.DirichletDistribution.compute_fixed_moments_and_f.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      306 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianWishartDistribution.compute_cgf_from_parents.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      360 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.GaussianMarkovChainDistribution.compute_message_to_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      360 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.SwitchingGaussianMarkovChainDistribution.plates_to_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      306 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.multinomial.MultinomialDistribution.compute_message_to_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      207 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.stochastic.Stochastic.delete.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      378 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.VaryingGaussianMarkovChainDistribution.compute_phi_from_parents.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      252 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaISO.move_plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      237 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianMoments.add_converter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      285 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGammaISO.plates_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      291 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISODistribution.plates_from_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      249 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical.CategoricalDistribution.random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      182 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.parse_command_line_arguments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      318 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamilyDistribution.compute_weights_to_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      204 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.constant.Constant.get_shape.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      258 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.stochastic.Stochastic.broadcasting_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      234 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.node.Moments.compute_dims_from_values.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      288 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.multinomial.MultinomialMoments.compute_dims_from_values.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      285 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical.CategoricalDistribution.plates_from_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      285 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.initialize_from_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      315 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamilyDistribution.compute_phi_from_parents.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      149 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.add_trailing_axes.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      225 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.delete.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      381 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.VaryingGaussianMarkovChainDistribution.compute_weights_to_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      249 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.stochastic.Distribution.plates_from_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      240 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.get_moments.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      312 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaToGaussianWishart.broadcasting_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      167 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.broadcasting_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      276 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.wishart.WishartDistribution.compute_moments_and_cgf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      288 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.binomial.BinomialDistribution.compute_weights_to_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      345 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical_markov_chain.CategoricalMarkovChainDistribution.compute_logpdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      285 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.binomial.BinomialDistribution.compute_phi_from_parents.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      252 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaISO.set_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      164 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.sum_multiply_to_plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      219 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gamma.GammaMoments.add_converter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      222 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.stochastic.Stochastic.get_moments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      219 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.load.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      234 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.get_shape.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      186 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.node.Node.has_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      273 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical.CategoricalDistribution.compute_logpdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      261 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDDistribution.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      267 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gamma.GammaDistribution.compute_phi_from_parents.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      291 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.bernoulli.BernoulliDistribution.compute_cgf_from_parents.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      134 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.optimize.minimize.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      177 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.node.Node.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      237 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.bernoulli.BernoulliDistribution.random.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      276 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaToGaussianWishart.set_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      285 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDToGaussianWishart.move_plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      279 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISOToGaussianGammaARD.get_mask.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      276 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.bernoulli.BernoulliMoments.compute_dims_from_values.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      110 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.chol.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      264 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gamma.GammaDistribution.compute_moments_and_cgf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      270 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.stochastic.Distribution.compute_weights_to_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      309 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISOToGaussianGammaARD.plates_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      312 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamilyDistribution.compute_moments_and_cgf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      243 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gamma.GammaDistribution.plates_to_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      231 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      267 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianDistribution.plates_from_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      261 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.beta.BetaDistribution.compute_cgf_from_parents.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      309 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianWishartDistribution.compute_message_to_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      240 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaISO.plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      189 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.constant.Constant.plot.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      122 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.tempfile.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      285 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianDistribution.compute_phi_from_parents.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      207 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.node.Node.plates_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      137 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.write_to_hdf5.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      312 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISODistribution.compute_weights_to_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      318 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamilyDistribution.compute_message_to_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     2479 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.TestCase.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      122 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.moveaxis.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      279 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.poisson.PoissonDistribution.compute_phi_from_parents.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      240 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaARD.plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      210 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.constant.Constant.set_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      300 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical.CategoricalDistribution.compute_moments_and_cgf.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      234 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGamma.plot.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      222 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGamma.plot.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      243 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.dirichlet.DirichletMoments.add_converter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      113 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.linalg.inv.rst
+drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-09-02 16:17:21.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      177 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertGreaterEqual.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      156 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertEqual.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:08.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.fail.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      153 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertLogs.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      171 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertTupleEqual.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      162 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertGreater.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      171 2016-01-03 11:18:08.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.shortDescription.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:08.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.setUp.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      165 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertNotEqual.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      177 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertRaisesRegexp.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      171 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertArrayEqual.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      171 2016-01-03 11:18:08.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.failUnlessRaises.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      177 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertAlmostEquals.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      171 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertWarnsRegex.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      153 2016-01-03 11:18:08.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.setUpClass.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      165 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertSetEqual.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      195 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertDictContainsSubset.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      156 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertFalse.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      189 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertNotRegexpMatches.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:08.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.skipTest.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      183 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertMessageToChild.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertAlmostEqual.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      162 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.CholeskyDense.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      153 2016-01-03 11:18:08.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.doCleanups.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      168 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertLessEqual.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertIn.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      156 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertNotIn.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      156 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.CholeskySparse.solve.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assert_.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:08.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.subTest.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      156 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertWarns.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      165 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.CholeskySparse.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:08.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.longMessage.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      153 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.addCleanup.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.addTypeEqualityFunc.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      183 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertNotAlmostEqual.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      153 2016-01-03 11:18:08.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.failUnless.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      153 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertTrue.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.defaultTestResult.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:08.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.failIfAlmostEqual.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.debug.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      168 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertNotEquals.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertIsNone.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      162 2016-01-03 11:18:08.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.tearDownClass.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      153 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertLess.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:08.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.failIf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:08.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.id.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertIs.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      168 2016-01-03 11:18:08.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.failUnlessEqual.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      183 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertMultiLineEqual.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      168 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertListEqual.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      186 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertNotAlmostEquals.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertRegexpMatches.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      165 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.countTestCases.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      201 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.CholeskySparse.trace_solve_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      198 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.CholeskyDense.trace_solve_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      156 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertIsNot.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      168 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertIsNotNone.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertEquals.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      165 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertNotRegex.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      165 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertAllClose.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      156 2016-01-03 11:18:08.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.failIfEqual.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.CholeskySparse.logdet.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      168 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertDictEqual.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      162 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertMessage.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      171 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertCountEqual.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      171 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertIsInstance.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      156 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertRegex.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      186 2016-01-03 11:18:08.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.failUnlessAlmostEqual.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:08.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.maxDiff.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      132 2016-01-03 11:18:08.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.run.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertRaisesRegex.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertRaises.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      153 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.CholeskyDense.solve.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:08.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.tearDown.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      156 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.CholeskyDense.logdet.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertSequenceEqual.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/generated/bayespy.utils.misc.TestCase.assertNotIsInstance.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      366 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.GaussianMarkovChainDistribution.compute_fixed_moments_and_f.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      288 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.poisson.PoissonDistribution.compute_fixed_moments_and_f.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      237 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.beta.BetaMoments.compute_fixed_moments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      240 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical.CategoricalMoments.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      300 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGammaISO.broadcasting_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      276 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.dirichlet.DirichletMoments.compute_dims_from_values.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      246 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.beta.BetaMoments.compute_dims_from_values.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      201 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.stochastic.Stochastic.show.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      249 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.wishart.WishartDistribution.compute_logpdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      249 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.add_plate_axis.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      282 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaDistribution.plates_from_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      131 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.random.intervals.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      243 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGamma.move_plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.node.Node.plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      222 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianMoments.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      267 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.bernoulli.BernoulliMoments.compute_fixed_moments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      261 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISOMoments.add_converter.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      267 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaToGaussianWishart.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      261 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaISO.add_plate_axis.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      249 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.constant.Constant.lower_bound_contribution.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      122 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.identity.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      327 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical_markov_chain.CategoricalMarkovChainMoments.add_converter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      243 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gamma.GammaMoments.compute_fixed_moments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      276 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISOToGaussianGammaARD.plates.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      276 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaDistribution.plates_to_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      225 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.deterministic.Deterministic.delete.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      255 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDDistribution.random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      333 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.GaussianMarkovChainMoments.compute_fixed_moments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      306 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianWishartDistribution.compute_phi_from_parents.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      231 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaISO.plot.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      237 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianWishart.plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      366 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.SwitchingGaussianMarkovChainDistribution.plates_from_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      222 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.node.Node.broadcasting_multiplier.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      246 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGamma.get_mask.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      252 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGamma.add_plate_axis.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      303 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianWishartDistribution.compute_moments_and_cgf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      237 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.binomial.BinomialMoments.get_converter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      270 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianWishart.plates_multiplier.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      234 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGamma.get_mask.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      216 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.stochastic.Stochastic.unobserve.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      360 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical_markov_chain.CategoricalMarkovChainMoments.compute_dims_from_values.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      309 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISODistribution.compute_phi_from_parents.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      231 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.deterministic.Deterministic.get_mask.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      294 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.dirichlet.DirichletDistribution.compute_weights_to_parent.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      237 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGamma.get_shape.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      318 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDDistribution.compute_fixed_moments_and_f.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      315 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamilyDistribution.compute_cgf_from_parents.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      276 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.deterministic.Deterministic.broadcasting_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      216 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.pdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      279 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.wishart.WishartDistribution.compute_cgf_from_parents.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      219 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.deterministic.Deterministic.plot.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      315 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianWishartDistribution.compute_fixed_moments_and_f.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      273 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDToGaussianWishart.plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      125 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.isinteger.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      243 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaARD.get_mask.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      261 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaToGaussianWishart.delete.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      140 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.random.wishart_rand.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      324 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamilyDistribution.compute_fixed_moments_and_f.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      252 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaARD.has_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      270 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianMoments.compute_dims_from_values.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      294 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianARDDistribution.compute_cgf_from_parents.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      276 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.poisson.PoissonDistribution.compute_moments_and_cgf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      228 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianWishart.plot.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      128 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.chol_solve.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      258 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianWishartMoments.add_converter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      222 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.stochastic.Stochastic.move_plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      285 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISODistribution.compute_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      186 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.node.Node.set_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      140 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.find_set_index.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      113 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.first.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      255 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGammaISO.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      309 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianWishartDistribution.compute_weights_to_parent.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      255 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGamma.move_plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      225 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.wishart.WishartDistribution.random.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      264 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaToGaussianWishart.plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      279 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDDistribution.compute_logpdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      309 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDDistribution.compute_phi_from_parents.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      128 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.linalg.chol_inv.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      261 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.binomial.BinomialDistribution.compute_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      149 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.is_scalar_integer.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      282 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianWishartMoments.compute_fixed_moments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      240 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.has_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      381 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.VaryingGaussianMarkovChainDistribution.compute_message_to_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      294 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISOMoments.compute_dims_from_values.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      255 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.poisson.PoissonDistribution.compute_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      270 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDToGaussianWishart.delete.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      228 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      264 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGammaISO.get_moments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      237 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.binomial.BinomialMoments.add_converter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      207 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.stochastic.Stochastic.random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      116 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.random.mask.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      267 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gamma.GammaDistribution.compute_cgf_from_parents.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      402 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.CholeskySparse.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      237 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.beta.BetaDistribution.plates_to_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      297 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamilyDistribution.plates_from_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      339 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.GaussianMarkovChainDistribution.plates_from_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      318 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISODistribution.compute_fixed_moments_and_f.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      303 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianARDDistribution.compute_fixed_moments_and_f.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      137 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.kalman_filter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      252 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGammaISO.plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      137 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.linalg.logdet_chol.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      240 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.deterministic.Deterministic.move_plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      291 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.dirichlet.DirichletDistribution.compute_phi_from_parents.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      143 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.array_to_scalar.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      134 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.linalg.logdet_tri.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      255 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.wishart.WishartDistribution.plates_to_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      264 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGammaISO.has_plotter.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      255 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaToGaussianWishart.plot.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      288 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISOToGaussianGammaARD.move_plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      137 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.random.correlation.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      134 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.multidigamma.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      285 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDDistribution.compute_gradient.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      246 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaMoments.from_values.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      249 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianWishart.get_moments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      297 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianARDDistribution.compute_message_to_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      237 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianMoments.get_converter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      134 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.linalg.chol_solve.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      213 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.beta.BetaMoments.get_converter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      219 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.stochastic.Stochastic.lowerbound.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      255 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.poisson.PoissonMoments.compute_fixed_moments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      336 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.SwitchingGaussianMarkovChainDistribution.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      357 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.GaussianMarkovChainDistribution.compute_phi_from_parents.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      234 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.unobserve.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      288 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianWishart.lower_bound_contribution.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      149 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.make_equal_length.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      234 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.deterministic.Deterministic.get_shape.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      119 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.linalg.m_dot.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      243 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.bernoulli.BernoulliMoments.get_converter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      137 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.random.categorical.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      186 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.node.Node.move_plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      134 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.random.covariance.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      261 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.beta.BetaDistribution.compute_phi_from_parents.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      288 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianDistribution.compute_message_to_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.node.Node.get_shape.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      264 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGammaISO.move_plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      249 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.deterministic.Deterministic.add_plate_axis.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      255 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.wishart.WishartMoments.compute_fixed_moments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      186 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.node.Node.get_moments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      252 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaISO.get_moments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      261 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDMoments.add_converter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      270 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.binomial.BinomialMoments.compute_dims_from_values.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      297 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaDistribution.compute_moments_and_cgf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      252 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaARD.get_moments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      225 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.poisson.PoissonDistribution.random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      210 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.stochastic.Stochastic.plates.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      243 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGamma.get_moments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      122 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      297 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianARDDistribution.compute_weights_to_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      240 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianWishart.get_mask.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      294 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianDistribution.compute_fixed_moments_and_f.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      306 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDDistribution.compute_moments_and_cgf.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      252 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaMoments.get_converter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      270 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gamma.GammaDistribution.compute_weights_to_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      116 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.invpsi.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      246 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDMoments.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      249 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianWishart.has_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      219 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.plot.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      213 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.beta.BetaMoments.add_converter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      231 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.stochastic.Stochastic.add_plate_axis.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      134 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.safe_indices.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      291 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGamma.broadcasting_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      288 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianDistribution.compute_weights_to_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      321 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDToGaussianWishart.broadcasting_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      119 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.linalg.outer.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      294 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGamma.lower_bound_contribution.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      342 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.GaussianMarkovChainMoments.compute_dims_from_values.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      122 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.invgamma.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      285 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.binomial.BinomialDistribution.compute_cgf_from_parents.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      225 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.update.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      288 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical.CategoricalMoments.compute_dims_from_values.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      309 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISODistribution.compute_cgf_from_parents.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      243 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianWishart.get_shape.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      327 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical_markov_chain.CategoricalMarkovChainDistribution.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      267 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.dirichlet.DirichletDistribution.plates_to_parent.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      297 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaToGaussianWishart.plates_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      285 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDToGaussianWishart.has_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      360 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.GaussianMarkovChainDistribution.compute_weights_to_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      243 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGammaISO.plot.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      201 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.stochastic.Stochastic.load.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      122 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.get_diag.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      285 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDDistribution.plates_to_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      258 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGammaISO.get_shape.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      294 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.dirichlet.DirichletDistribution.compute_message_to_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      264 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDToGaussianWishart.plot.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      231 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.wishart.WishartMoments.get_converter.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      276 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGamma.plates_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      119 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.linalg.mmdot.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      143 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.repeat_to_shape.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      303 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGammaISO.lower_bound_contribution.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      125 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.logsumexp.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      291 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianARDDistribution.compute_moments_and_cgf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      279 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.multinomial.MultinomialMoments.compute_fixed_moments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      122 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.random.sphere.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      273 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaISO.plates_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      312 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.multinomial.MultinomialDistribution.compute_fixed_moments_and_f.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      261 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamilyDistribution.random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      131 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.sum_product.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      210 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.constant.Constant.get_moments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      354 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.GaussianMarkovChainDistribution.compute_moments_and_cgf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      131 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.is_callable.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      152 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.composite_function.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      276 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaToGaussianWishart.move_plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      222 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.stochastic.Stochastic.set_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      110 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.symm.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      261 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDMoments.get_converter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      222 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.dims.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      231 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.poisson.PoissonMoments.add_converter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      288 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.bernoulli.BernoulliDistribution.compute_moments_and_cgf.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      249 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGamma.get_shape.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      243 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.get_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      261 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianDistribution.plates_to_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      128 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.put_simple.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      255 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.binomial.BinomialDistribution.compute_logpdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      291 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDDistribution.plates_from_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      354 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.VaryingGaussianMarkovChainDistribution.plates_to_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      384 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.SwitchingGaussianMarkovChainDistribution.compute_phi_from_parents.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      119 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.m_outer.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      261 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.poisson.PoissonDistribution.plates_from_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      270 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.initialize_from_value.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      222 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.binomial.BinomialMoments.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      231 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.beta.BetaDistribution.compute_logpdf.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      255 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGamma.get_moments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      171 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.node.Node.delete.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      300 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.bernoulli.BernoulliDistribution.compute_fixed_moments_and_f.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      110 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.nans.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      381 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.SwitchingGaussianMarkovChainDistribution.compute_moments_and_cgf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      240 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianWishart.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      237 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.binomial.BinomialDistribution.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      309 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.GaussianMarkovChainDistribution.__init__.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      243 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGamma.has_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      134 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.zipper_merge.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      249 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGammaISO.delete.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      285 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISODistribution.plates_to_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      149 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.random.invwishart_rand.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      276 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianWishartDistribution.compute_logpdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      273 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.bernoulli.BernoulliDistribution.plates_from_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      143 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.random.gamma_entropy.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      165 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.node.Node.plot.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      249 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianWishart.move_plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      201 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.stochastic.Stochastic.plot.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      116 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.linalg.chol.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      116 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.random.orth.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      146 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.add_leading_axes.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      140 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.random.gamma_logpdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      255 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISODistribution.random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      116 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.unique.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      312 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical.CategoricalDistribution.compute_fixed_moments_and_f.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      261 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.deterministic.Deterministic.plates_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      255 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.poisson.PoissonDistribution.plates_to_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      282 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianDistribution.compute_moments_and_cgf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      249 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.multinomial.MultinomialDistribution.random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      282 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.poisson.PoissonDistribution.compute_message_to_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      291 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.dirichlet.DirichletDistribution.compute_cgf_from_parents.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      354 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.VaryingGaussianMarkovChainDistribution.compute_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      207 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.stochastic.Stochastic.update.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      246 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaDistribution.random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      288 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISOToGaussianGammaARD.has_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      243 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.bernoulli.BernoulliDistribution.__init__.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      276 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaToGaussianWishart.get_moments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      140 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.squeeze_to_dim.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      255 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.multinomial.MultinomialDistribution.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      279 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISOToGaussianGammaARD.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      207 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.beta.BetaDistribution.random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      297 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISOToGaussianGammaARD.add_plate_axis.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      300 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.multinomial.MultinomialDistribution.compute_moments_and_cgf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      294 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.bernoulli.BernoulliDistribution.compute_weights_to_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      110 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.diag.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      243 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.stochastic.Distribution.plates_to_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      243 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaISO.get_mask.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      267 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.dirichlet.DirichletDistribution.compute_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      249 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gamma.GammaDistribution.plates_from_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      110 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.rmse.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      201 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.node.Moments.get_converter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      228 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.deterministic.Deterministic.plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      134 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.sum_multiply.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      234 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGamma.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      185 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.broadcasted_shape_from_arrays.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      291 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamilyDistribution.compute_gradient.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      252 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaDistribution.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      246 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.constant.Constant.broadcasting_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      282 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISOToGaussianGammaARD.get_shape.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      243 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGamma.set_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      255 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical.CategoricalDistribution.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      134 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.rts_smoother.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      213 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.stochastic.Stochastic.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      161 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.random.gaussian_gamma_to_t.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      137 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.linalg.chol_logdet.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      270 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaToGaussianWishart.get_shape.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      261 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.bernoulli.BernoulliDistribution.compute_logpdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      219 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.save.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      279 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDToGaussianWishart.get_shape.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      201 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.constant.Constant.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      306 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISODistribution.compute_moments_and_cgf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      246 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISOMoments.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      294 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianARDDistribution.compute_phi_from_parents.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      255 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGamma.set_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      131 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.logdet_chol.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      264 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.beta.BetaDistribution.compute_weights_to_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      219 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.show.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      378 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.categorical_markov_chain.CategoricalMarkovChainDistribution.compute_message_to_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      119 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.linalg.inner.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      288 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.wishart.WishartDistribution.compute_fixed_moments_and_f.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      273 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.dirichlet.DirichletDistribution.plates_from_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      288 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISOToGaussianGammaARD.get_moments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      177 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.node.Node.get_mask.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      252 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaARD.set_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      158 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.linalg.block_banded_solve.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      264 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.poisson.PoissonMoments.compute_dims_from_values.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      282 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.wishart.WishartDistribution.compute_weights_to_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      240 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.move_plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      360 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.VaryingGaussianMarkovChainDistribution.plates_from_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      267 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.binomial.BinomialDistribution.plates_from_parent.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      143 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.nested_iterator.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      252 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaISO.has_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      471 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/bayespy.utils.linalg.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      527 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.binomial.BinomialMoments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      829 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gamma.GammaDistribution.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      992 2016-03-30 08:06:12.000000 bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaDistribution.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      560 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.categorical.CategoricalMoments.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      664 2016-03-30 08:06:12.000000 bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaMoments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1037 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDDistribution.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1656 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      992 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISODistribution.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      816 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.constant.Constant.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      971 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.categorical.CategoricalDistribution.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      591 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISOMoments.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      977 2016-03-30 08:06:12.000000 bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGamma.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1226 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.VaryingGaussianMarkovChainDistribution.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1215 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDToGaussianWishart.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      917 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.binomial.BinomialDistribution.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      962 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianARDDistribution.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      863 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.wishart.WishartDistribution.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1009 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamilyDistribution.rst
+-rw-------   0 jluttine  (1000) jluttine  (1000)     1015 2016-05-04 12:21:07.000000 bayespy-0.5.9/doc/source/dev_api/distributions.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      355 2015-06-03 09:18:36.000000 bayespy-0.5.9/doc/source/dev_api/dev_api.rst
+-rw-------   0 jluttine  (1000) jluttine  (1000)      713 2016-05-04 12:21:07.000000 bayespy-0.5.9/doc/source/dev_api/moments.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      287 2015-06-03 09:18:36.000000 bayespy-0.5.9/doc/source/dev_api/utils.rst
+-rw-------   0 jluttine  (1000) jluttine  (1000)      751 2016-05-04 12:21:07.000000 bayespy-0.5.9/doc/source/dev_api/nodes.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      219 2015-06-03 09:18:36.000000 bayespy-0.5.9/doc/source/references.rst
+drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-09-02 16:17:21.000000 bayespy-0.5.9/doc/source/user_guide/
+-rw-------   0 jluttine  (1000) jluttine  (1000)     5880 2016-05-04 12:21:07.000000 bayespy-0.5.9/doc/source/user_guide/quickstart.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      279 2015-06-03 09:18:36.000000 bayespy-0.5.9/doc/source/user_guide/user_guide.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)    14493 2015-06-03 09:18:36.000000 bayespy-0.5.9/doc/source/user_guide/advanced.rst
+-rw-------   0 jluttine  (1000) jluttine  (1000)    14269 2016-08-17 10:33:18.000000 bayespy-0.5.9/doc/source/user_guide/inference.rst
+-rw-------   0 jluttine  (1000) jluttine  (1000)    15602 2016-05-04 12:21:07.000000 bayespy-0.5.9/doc/source/user_guide/plot.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     3380 2014-06-12 13:50:13.000000 bayespy-0.5.9/doc/source/user_guide/quickstartbackup.py
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)    20918 2015-06-03 09:18:36.000000 bayespy-0.5.9/doc/source/user_guide/modelconstruct.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      173 2015-06-03 09:18:36.000000 bayespy-0.5.9/doc/source/user_guide/install.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)     5068 2015-06-03 09:18:36.000000 bayespy-0.5.9/doc/source/user_guide/quickstartbackup.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      449 2015-06-03 09:18:36.000000 bayespy-0.5.9/doc/source/index.rst
+-rw-------   0 jluttine  (1000) jluttine  (1000)    11116 2017-09-02 16:06:14.000000 bayespy-0.5.9/doc/source/conf.py
+drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-09-02 16:17:21.000000 bayespy-0.5.9/doc/source/dev_guide/
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)     6201 2015-06-03 09:18:36.000000 bayespy-0.5.9/doc/source/dev_guide/advanced.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      701 2015-06-03 09:18:36.000000 bayespy-0.5.9/doc/source/dev_guide/engine.rst
+-rw-------   0 jluttine  (1000) jluttine  (1000)    15553 2016-05-04 12:21:07.000000 bayespy-0.5.9/doc/source/dev_guide/writingnodes.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)    10777 2015-06-03 09:18:36.000000 bayespy-0.5.9/doc/source/dev_guide/vmp.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)     2337 2015-11-02 11:23:25.000000 bayespy-0.5.9/doc/source/dev_guide/workflow.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      459 2015-06-03 09:18:36.000000 bayespy-0.5.9/doc/source/dev_guide/dev_guide.rst
+drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-09-02 16:17:21.000000 bayespy-0.5.9/doc/source/dev_guide/vmp/
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     2465 2013-07-24 18:00:26.000000 bayespy-0.5.9/doc/source/dev_guide/vmp/vmp_gaussian.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)       61 2013-07-24 18:00:26.000000 bayespy-0.5.9/doc/source/dev_guide/vmp/vmp_gaussian_wishart.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     3286 2013-07-24 18:00:26.000000 bayespy-0.5.9/doc/source/dev_guide/vmp/vmp_mixture.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1922 2013-07-24 18:00:26.000000 bayespy-0.5.9/doc/source/dev_guide/vmp/vmp_wishart.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)       38 2013-07-24 18:00:26.000000 bayespy-0.5.9/doc/source/dev_guide/vmp/vmp_gamma.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)       57 2013-07-24 18:00:26.000000 bayespy-0.5.9/doc/source/dev_guide/vmp/vmp_gaussian_gamma.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)       52 2013-07-24 18:00:26.000000 bayespy-0.5.9/doc/source/dev_guide/vmp/vmp_normal_gamma.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)       62 2013-07-24 18:00:26.000000 bayespy-0.5.9/doc/source/dev_guide/vmp/vmp_normal.rst
+drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-09-02 16:17:21.000000 bayespy-0.5.9/doc/source/user_api/
+drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-09-02 16:17:21.000000 bayespy-0.5.9/doc/source/user_api/generated/
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)       55 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/bayespy.plot.rst
+drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-09-02 16:17:21.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      268 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.plot.PDFPlotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1368 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.nodes.Multinomial.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      823 2016-06-12 17:22:50.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.nodes.ConcatGaussian.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      510 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.inference.vmp.transformations.RotateGaussian.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      653 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.nodes.Gate.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)       92 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.nodes.Dot.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)       92 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.plot.plot.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      256 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.plot.Plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      510 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.inference.vmp.transformations.RotateMultiple.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      403 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.inference.vmp.transformations.RotationOptimizer.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1482 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.nodes.GaussianARD.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      609 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.inference.vmp.transformations.RotateGaussianMarkovChain.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1185 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.nodes.Gamma.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1407 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.nodes.Exponential.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1682 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.nodes.GaussianGammaISO.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1260 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.nodes.Binomial.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     2023 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1313 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.nodes.Gaussian.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      328 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.plot.GaussianTimeseriesPlotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      600 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.inference.vmp.transformations.RotateVaryingMarkovChain.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      137 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.plot.gaussian_mixture_2d.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      537 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.inference.vmp.transformations.RotateGaussianARD.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)       98 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.plot.hinton.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      721 2016-06-12 17:22:50.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.nodes.Function.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      618 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.inference.vmp.transformations.RotateSwitchingMarkovChain.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1224 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.nodes.Wishart.rst
+drwx------   0 jluttine  (1000) jluttine  (1000)        0 2017-09-02 16:17:21.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      201 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.initialize_from_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      168 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.get_riemannian_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      114 2016-01-03 14:57:36.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Take.delete.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      219 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.get_riemannian_gradient.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      141 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.logpdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      153 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.get_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      177 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.broadcasting_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      111 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.plot.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.dims.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      222 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateGaussian.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      117 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.load.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.get_mask.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      243 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateMultiple.get_bound_terms.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      141 2016-06-12 17:22:50.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Function.get_moments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.get_moments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.get_moments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gate.get_moments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      156 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.VB.compute_lowerbound.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      252 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateSwitchingMarkovChain.rotate.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      156 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.get_mask.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      168 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.initialize_from_prior.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.get_riemannian_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      195 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.integrated_logpdf_from_parents.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.initialize_from_prior.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.get_moments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.observe.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.delete.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      105 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.pdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Add.get_moments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      153 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.observe.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.VB.set_callback.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.SumMultiply.get_moments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      171 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.initialize_from_random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      195 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.initialize_from_value.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      243 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateVaryingMarkovChain.nodes.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      153 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.get_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.plot.FunctionPlotter.__init__.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      180 2016-06-12 17:22:50.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Function.lower_bound_contribution.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      153 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.set_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      210 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.set_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.logpdf.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      186 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.initialize_from_prior.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.observe.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      165 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.has_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      123 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.delete.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      201 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.broadcasting_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.get_mask.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.dims.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      201 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.get_riemannian_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      153 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.observe.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.set_parameters.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      165 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.add_plate_axis.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      183 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.get_moments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      210 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.initialize_from_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      186 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.delete.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      120 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.dims.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      186 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.get_riemannian_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      165 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.get_shape.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.load.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      120 2016-01-03 14:57:36.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Take.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.has_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      120 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.dims.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      132 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.get_shape.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.move_plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      123 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.dims.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      150 2016-06-12 17:22:50.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.ConcatGaussian.get_mask.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      132 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.observe.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      111 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Add.delete.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      183 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.lower_bound_contribution.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.get_moments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.move_plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      171 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.initialize_from_prior.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      192 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.get_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      219 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.initialize_from_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      189 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.lower_bound_contribution.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      171 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.VB.plot_iteration_by_nodes.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      225 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.initialize_from_prior.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.SumMultiply.get_shape.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gate.set_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      213 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateGaussian.nodes.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      162 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.show.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      165 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.plates_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      183 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.initialize_from_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      117 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.logpdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.initialize_from_prior.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      213 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.initialize_from_prior.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.set_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      165 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.plates_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      183 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.initialize_from_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      204 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.lower_bound_contribution.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.set_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.initialize_from_value.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      189 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.lower_bound_contribution.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      162 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.set_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.get_mask.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.get_mask.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.update.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      114 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.VB.load.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.lowerbound.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.load.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.set_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.get_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.set_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      123 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.save.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      117 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.save.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      222 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.get_gaussian_mean_and_variance.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.delete.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      114 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      183 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.plates_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.lowerbound.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      132 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.has_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.delete.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      216 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateGaussian.rotate.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.has_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.delete.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.broadcasting_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      192 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.get_mask.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      213 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateMultiple.nodes.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.initialize_from_random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.add_plate_axis.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      117 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.load.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      186 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      165 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.dims.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      132 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.get_shape.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.initialize_from_prior.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 14:57:36.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Take.add_plate_axis.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.plot.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      171 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.SumMultiply.plates_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.move_plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.add_plate_axis.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.get_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 14:57:36.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Take.move_plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      120 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.plot.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.initialize_from_prior.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.save.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      240 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.lower_bound_contribution.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.has_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      168 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gate.lower_bound_contribution.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      192 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.lowerbound.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      198 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.get_riemannian_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.get_shape.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.move_plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      123 2016-01-03 14:57:36.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Take.get_shape.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      186 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.initialize_from_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      111 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.dims.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      141 2016-06-12 17:22:50.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Function.move_plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.delete.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      240 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.initialize_from_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      186 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      120 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.observe.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.plot.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      117 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gate.plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      117 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.show.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gate.add_plate_axis.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      186 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.broadcasting_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      192 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.initialize_from_value.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      204 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.initialize_from_prior.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.set_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 14:57:36.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Take.has_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      171 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.get_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 14:57:36.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Take.set_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      231 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.initialize_from_prior.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.set_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.get_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      198 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.initialize_from_random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      171 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.initialize_from_prior.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      162 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.plot.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      132 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.get_shape.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.rotate.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.lowerbound.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      123 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.update.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.unobserve.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.plot.HintonPlotter.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      165 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Add.lower_bound_contribution.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      189 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.get_shape.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      186 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.get_gaussian_location.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.get_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.move_plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      195 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.has_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      111 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.show.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.lowerbound.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.get_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      177 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.get_shape.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      123 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.logpdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      258 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateSwitchingMarkovChain.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      198 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.get_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.lowerbound.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.add_plate_axis.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.save.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      108 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gate.plot.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      123 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      195 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.set_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.add_plate_axis.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      225 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateGaussianARD.rotate.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      222 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateGaussianARD.setup.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      135 2016-06-12 17:22:50.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Function.get_shape.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      153 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.plotmatrix.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.broadcasting_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.get_riemannian_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.logpdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      234 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.initialize_from_random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.save.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.add_plate_axis.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.add_plate_axis.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      156 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.get_moments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      243 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateVaryingMarkovChain.setup.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      120 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.save.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      153 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.add_plate_axis.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      156 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.move_plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      132 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.get_moments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      198 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.initialize_from_random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      186 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.get_mask.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      189 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.lowerbound.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      171 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.plates_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      192 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.set_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      153 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      168 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.initialize_from_value.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      117 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.plot.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      222 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateGaussianARD.bound.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Add.move_plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      213 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateGaussian.setup.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      123 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.save.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      207 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.initialize_from_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      195 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.get_shape.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      120 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.VB.update.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      195 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.initialize_from_value.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.get_riemannian_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.plot.Plotter.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      162 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.plates_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.set_parameters.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      141 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.random.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      177 2016-06-12 17:22:50.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Function.broadcasting_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      177 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.lower_bound_contribution.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      162 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.save.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      117 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.plates.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      150 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.translate.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      237 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.get_riemannian_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      162 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.observe.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      177 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.get_riemannian_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      192 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.initialize_from_prior.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      222 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.plates_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.logpdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.load.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      177 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.lower_bound_contribution.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      210 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.initialize_from_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.get_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.has_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.set_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      132 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.unobserve.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      159 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.get_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      201 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.get_moments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.get_moments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      114 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gate.delete.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      132 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.unobserve.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.show.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.logpdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      168 2016-01-03 14:57:36.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Take.lower_bound_contribution.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      156 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.has_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      168 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.initialize_from_prior.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      111 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.load.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.as_diagonal_wishart.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      216 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.initialize_from_random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.get_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      117 2016-01-03 14:57:36.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Take.plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      117 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.plot.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.get_shape.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.set_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      204 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.plates_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.lowerbound.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      132 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.dims.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.set_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.save.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      279 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateSwitchingMarkovChain.get_bound_terms.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.initialize_from_prior.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      153 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.lowerbound.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      141 2016-06-12 17:22:50.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Function.set_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      198 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.broadcasting_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      171 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.add_plate_axis.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      132 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.move_plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      189 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.SumMultiply.lower_bound_contribution.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      153 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.plates_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      117 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.load.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      159 2016-06-12 17:22:50.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.ConcatGaussian.set_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      114 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.logpdf.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      213 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.get_gaussian_mean_and_variance.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      120 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.dims.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      177 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.broadcasting_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 14:57:36.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Take.get_moments.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      147 2016-06-12 17:22:50.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.ConcatGaussian.plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      189 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.unobserve.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.get_moments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.update.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      117 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.show.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      168 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.initialize_from_prior.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.plot.GaussianTimeseriesPlotter.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.add_plate_axis.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      183 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.move_plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.set_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.unobserve.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.delete.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      246 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateGaussianMarkovChain.setup.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      117 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.unobserve.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.move_plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      153 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.get_moments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.logpdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.VB.loglikelihood_lowerbound.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.VB.gradient_step.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      183 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.set_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      177 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.lower_bound_contribution.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      171 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.lowerbound.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.has_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.set_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      120 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.pdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      231 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateGaussianARD.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.unobserve.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      120 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.pdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      222 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateMultiple.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      123 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.show.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      177 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.unobserve.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.add_plate_axis.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.delete.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      207 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.initialize_from_random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      162 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.get_moments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      117 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Add.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      114 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.pdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      111 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.save.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      120 2016-01-03 14:57:36.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Take.get_mask.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.update.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.initialize_from_prior.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      153 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.load.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.lowerbound.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.pdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      153 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.get_gradient.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      144 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      195 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.unobserve.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      123 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.update.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.unobserve.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      123 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.plot.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      249 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateSwitchingMarkovChain.bound.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      183 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.lower_bound_contribution.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.SumMultiply.plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.initialize_from_value.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.SumMultiply.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.load.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.dims.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      183 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.initialize_from_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      171 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.rotate.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      210 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.get_riemannian_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      204 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.lower_bound_contribution.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      120 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.load.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      186 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.get_riemannian_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.delete.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      165 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.set_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.move_plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.add_plate_axis.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      117 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Add.get_mask.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      123 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.plot.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      183 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.dims.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.VB.compute_lowerbound_terms.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      153 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.get_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.unobserve.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      117 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.delete.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.dims.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.get_shape.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      162 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.plates_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.lowerbound.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      204 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.add_plate_axis.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      162 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.initialize_from_random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      111 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.VB.dot.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      123 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.logpdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gate.move_plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      153 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.get_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      171 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.initialize_from_value.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.delete.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      186 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.rotate.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      123 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.delete.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.broadcasting_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      171 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.set_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      120 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      195 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.plates_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      189 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.lower_bound_contribution.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      153 2016-06-12 17:22:50.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.ConcatGaussian.get_shape.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      165 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.broadcasting_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      171 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.observe.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.VB.get_gradients.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.set_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      171 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.lower_bound_contribution.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      132 2016-06-12 17:22:50.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Function.__init__.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      141 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.delete.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      168 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.get_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.dims.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      189 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.observe.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      195 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.initialize_from_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      237 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.broadcasting_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.rotate.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      162 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.plotmatrix.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.SumMultiply.has_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      114 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Add.plates.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      159 2016-06-12 17:22:50.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.ConcatGaussian.move_plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      168 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.VB.get_iteration_by_nodes.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      135 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.plot.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      201 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.lower_bound_contribution.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.delete.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      132 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.dims.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      177 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.initialize_from_random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      171 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.plates_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.update.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      138 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.dims.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      123 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      171 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.plates_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      162 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.load.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      156 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.set_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      201 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.broadcasting_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      177 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.initialize_from_random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      117 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.show.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.VB.pattern_search.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.lowerbound.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      150 2016-06-12 17:22:50.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Function.add_plate_axis.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      177 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.get_riemannian_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.set_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.get_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      186 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.plates_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      210 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.get_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      123 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.logpdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.lowerbound.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      171 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.initialize_from_value.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      123 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.dims.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      165 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.get_moments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.__init__.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      192 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.broadcasting_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.has_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.show.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.unobserve.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      162 2016-06-12 17:22:50.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Function.plates_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      171 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.initialize_from_random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.plot.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      153 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.plot.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.get_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.plot.ContourPlotter.__init__.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      129 2016-06-12 17:22:50.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Function.plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      123 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.load.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      120 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.plot.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      165 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.set_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      177 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.dims.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.VB.has_converged.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.observe.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      147 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.load.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.has_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      171 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.pdf.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      165 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.get_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      168 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.get_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      162 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.initialize_from_random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      201 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.set_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.get_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      114 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.VB.save.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.SumMultiply.add_plate_axis.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      135 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.save.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.get_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      243 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateVaryingMarkovChain.bound.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      165 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.has_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      132 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      186 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.broadcasting_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.delete.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      135 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.load.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      162 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Add.broadcasting_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      117 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.pdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.logpdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.set_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      132 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.show.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      201 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.has_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.logpdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.load.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      231 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.get_riemannian_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      195 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.move_plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.get_shape.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.initialize_from_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      120 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.save.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      192 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.get_riemannian_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      276 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateGaussianMarkovChain.get_bound_terms.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      228 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.initialize_from_random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.update.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.update.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      120 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.show.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      114 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.pdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      195 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.initialize_from_random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.set_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      120 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.load.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      123 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.show.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      165 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.initialize_from_random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      231 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.broadcasting_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      117 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.save.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      153 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.add_plate_axis.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.pdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.show.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      132 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.unobserve.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      168 2016-06-12 17:22:50.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.ConcatGaussian.add_plate_axis.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      156 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      162 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.has_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.move_plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      108 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.load.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      162 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.initialize_from_value.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      195 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.initialize_from_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      246 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateGaussianMarkovChain.bound.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      162 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.VB.ignore_bound_checks.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      195 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.lower_bound_contribution.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.observe.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.logpdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      120 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      132 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.get_mask.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      201 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.move_plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      186 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.initialize_from_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.lowerbound.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.get_shape.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.pdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      156 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.unobserve.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      168 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.broadcasting_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      255 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateGaussianMarkovChain.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.logpdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      108 2016-01-03 14:57:36.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Take.plot.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      165 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.set_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.unobserve.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.initialize_from_value.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.get_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      132 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.plates.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      132 2016-06-12 17:22:50.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Function.get_mask.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.SumMultiply.delete.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      216 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.plates_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      153 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.get_mask.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.has_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.set_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.get_moments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.has_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      231 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.initialize_from_value.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.get_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.get_riemannian_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      165 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.move_plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      123 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gate.get_shape.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.SumMultiply.plot.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      159 2016-06-12 17:22:50.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.ConcatGaussian.get_moments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.lower_bound_contribution.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.VB.set_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.SumMultiply.get_mask.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Add.set_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.get_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      195 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.initialize_from_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      132 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.dims.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      150 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.unobserve.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.random.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      180 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.get_marginal_logpdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      249 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateGaussianMarkovChain.rotate.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      177 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.initialize_from_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.get_mask.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.add_plate_axis.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      210 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.add_plate_axis.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      204 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.set_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      183 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.has_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      189 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.initialize_from_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.get_mask.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      117 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.pdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.update.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.observe.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      123 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.unobserve.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.show.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.logpdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.save.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.plot.PDFPlotter.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.plot.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      117 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.observe.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.move_plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      183 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.initialize_from_random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      183 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.initialize_from_random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      228 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.initialize_from_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.set_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.initialize_from_value.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      153 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      183 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      162 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.lowerbound.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.VB.use_logging.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.set_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      186 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.broadcasting_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      132 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.get_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.plates_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      186 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.broadcasting_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      165 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.get_moments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.pdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      123 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.update.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.has_plotter.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      141 2016-06-12 17:22:50.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Function.has_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 14:57:36.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Take.plates_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.save.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      123 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.load.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      144 2016-06-12 17:22:50.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.ConcatGaussian.delete.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.get_mask.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      156 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.rotate_plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      156 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.dims.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.show.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.get_mask.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      120 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gate.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.broadcasting_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.get_moments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      165 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.get_riemannian_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.observe.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.show.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.has_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      225 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.initialize_from_value.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      162 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.lowerbound.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.initialize_from_value.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.pdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      132 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      105 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Add.plot.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.show.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.show.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gate.plates_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      153 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.show.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      114 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.delete.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      126 2016-06-12 17:22:50.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Function.delete.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      186 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.initialize_from_value.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      114 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.pdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      156 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      114 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.dims.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.set_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.rotate.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      132 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.dims.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.observe.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.pdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.get_gradient.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      180 2016-06-12 17:22:50.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.ConcatGaussian.plates_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Add.plates_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.pdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.VB.optimize.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      168 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.unobserve.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      195 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.initialize_from_prior.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.pdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      168 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.delete.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.lower_bound_contribution.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      216 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateMultiple.rotate.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.pdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.get_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      252 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateGaussianARD.get_bound_terms.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.get_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.set_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      153 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.save.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      252 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateVaryingMarkovChain.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.get_shape.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.move_plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      198 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.lowerbound.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      156 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.get_shape.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      186 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.SumMultiply.broadcasting_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.delete.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.SumMultiply.move_plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      186 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.get_riemannian_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      183 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.initialize_from_random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      117 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.plot.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      120 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.show.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      192 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.plot.CategoricalMarkovChainPlotter.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.logpdf.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      177 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.plates_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      213 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.lower_bound_contribution.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.unobserve.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.set_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      165 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gate.broadcasting_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.logpdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.get_shape.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.lowerbound.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      189 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.get_marginal_logpdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      108 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.pdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.save.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      162 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.initialize_from_prior.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.get_moments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      165 2016-01-03 14:57:36.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Take.broadcasting_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.get_riemannian_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.add_plate_axis.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      186 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.update.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      108 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.show.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.update.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.add_plate_axis.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      222 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateGaussianARD.nodes.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      123 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.get_mask.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.initialize_from_prior.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.lowerbound.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      165 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.get_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.plot.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      114 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.VB.plot.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.initialize_from_value.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      123 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      189 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.lower_bound_contribution.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.VB.set_autosave.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.plot.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      192 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      108 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.plot.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      213 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateMultiple.setup.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.update.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      144 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.observe.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      246 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateVaryingMarkovChain.rotate.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      219 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.broadcasting_multiplier.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      141 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.rotate.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      141 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.update.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      171 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.initialize_from_random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      213 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.initialize_from_value.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      150 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.get_shape.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      120 2016-06-12 17:22:50.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Function.plot.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      246 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.initialize_from_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      213 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateGaussian.bound.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.logpdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.set_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      192 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.add_plate_axis.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      231 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotationOptimizer.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      153 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.get_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.VB.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      201 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.get_riemannian_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      171 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.plates_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      225 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotationOptimizer.rotate.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      168 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.initialize_from_value.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      150 2016-06-12 17:22:50.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.ConcatGaussian.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.get_mask.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      168 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.get_shape.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      177 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.get_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      123 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.plot.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.set_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.initialize_from_value.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      210 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.broadcasting_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      183 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.initialize_from_random.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      147 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.get_mask.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.broadcasting_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.move_plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.get_mask.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      168 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.update.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      183 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.add_plate_axis.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      204 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.get_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      120 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.get_mask.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      135 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.show.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      204 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.initialize_from_value.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      108 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.save.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      168 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.logpdf.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      138 2016-06-12 17:22:50.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.ConcatGaussian.plot.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.unobserve.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.get_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      132 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.set_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      249 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateSwitchingMarkovChain.nodes.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.update.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.SumMultiply.set_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.get_moments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      120 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gate.get_mask.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.get_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      165 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.move_plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Add.has_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      177 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.pdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      114 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.update.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      246 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateGaussianMarkovChain.nodes.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.get_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      126 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.observe.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      195 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.get_moments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.load.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      186 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.plates_multiplier.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      195 2016-06-12 17:22:50.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.ConcatGaussian.broadcasting_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.get_moments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gate.has_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.move_plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.lowerbound.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.get_shape.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.has_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.get_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      186 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.logpdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      168 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.initialize_from_value.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.plot.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      186 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.get_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Poisson.set_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.save.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.load.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.plates_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      273 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateVaryingMarkovChain.get_bound_terms.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.unobserve.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      117 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.update.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.plates_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      195 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.initialize_from_prior.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      153 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Dirichlet.set_parameters.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      132 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.pdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      156 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gamma.as_diagonal_wishart.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      234 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.lower_bound_contribution.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      159 2016-06-12 17:22:50.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.ConcatGaussian.has_plotter.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      198 2016-06-12 17:22:50.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.ConcatGaussian.lower_bound_contribution.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      168 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      111 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.VB.add.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      204 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.get_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      186 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.get_riemannian_gradient.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      222 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.lower_bound_contribution.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      123 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.get_shape.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.has_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      123 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Wishart.delete.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      195 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.initialize_from_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.plot.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.observe.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      243 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateGaussian.get_bound_terms.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.VB.set_annealing.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      213 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateMultiple.bound.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      183 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.CategoricalMarkovChain.set_plotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      129 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.delete.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      249 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.vmp.transformations.RotateSwitchingMarkovChain.setup.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      189 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.initialize_from_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      156 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.get_mask.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.move_plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      117 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.save.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      189 2016-03-30 08:06:13.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGamma.initialize_from_random.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      132 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.get_mask.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      183 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.get_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      138 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.observe.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      180 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.update.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Exponential.get_shape.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      120 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Add.get_shape.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      132 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Bernoulli.observe.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaARD.save.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      162 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianWishart.move_plates.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.SumMultiply.get_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.inference.VB.get_parameters.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      159 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Mixture.plates_multiplier.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.update.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      147 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Gaussian.rotate_matrix.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Multinomial.get_moments.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      165 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianMarkovChain.get_mask.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      222 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianARD.initialize_from_mean_and_covariance.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      144 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.load.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      183 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.observe.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Add.add_plate_axis.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      174 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.add_plate_axis.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      135 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Binomial.get_shape.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      168 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Beta.lower_bound_contribution.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      141 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.Categorical.__init__.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      150 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/generated/bayespy.nodes.GaussianGammaISO.update.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1764 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.nodes.CategoricalMarkovChain.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      636 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.nodes.Add.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      284 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.plot.ContourPlotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      877 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.inference.VB.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1296 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.nodes.Bernoulli.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      101 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.plot.contour.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1270 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.nodes.Mixture.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      653 2016-01-03 14:57:36.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.nodes.Take.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1368 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.nodes.Categorical.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      280 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.plot.HintonPlotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1224 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.nodes.Poisson.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1512 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.nodes.GaussianWishart.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1296 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.nodes.Dirichlet.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1949 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)     1667 2016-03-30 08:06:12.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.nodes.GaussianGamma.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      344 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.plot.CategoricalMarkovChainPlotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      806 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.nodes.SumMultiply.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      101 2016-06-12 17:22:50.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.nodes.Choose.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1690 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.nodes.GaussianMarkovChain.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1548 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.nodes.GaussianGammaARD.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)     1116 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.nodes.Beta.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)      288 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.plot.FunctionPlotter.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)       89 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.plot.pdf.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)       58 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/bayespy.nodes.rst
+-rw-rw-r--   0 jluttine  (1000) jluttine  (1000)       70 2016-01-03 11:18:07.000000 bayespy-0.5.9/doc/source/user_api/generated/bayespy.inference.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      323 2015-06-03 09:18:36.000000 bayespy-0.5.9/doc/source/user_api/user_api.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      213 2015-06-03 09:18:36.000000 bayespy-0.5.9/doc/source/demos.rst
+-rw-r--r--   0 jluttine  (1000) jluttine  (1000)      526 2015-06-03 09:18:36.000000 bayespy-0.5.9/doc/source/nodes.rst
+-rw-------   0 jluttine  (1000) jluttine  (1000)      379 2017-09-02 16:17:21.000000 bayespy-0.5.9/setup.cfg
+-rw-------   0 jluttine  (1000) jluttine  (1000)     4038 2017-01-22 15:43:29.000000 bayespy-0.5.9/setup.py
```

### Comparing `bayespy-0.5.8/PKG-INFO` & `bayespy-0.5.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: bayespy
-Version: 0.5.8
+Version: 0.5.9
 Summary: Variational Bayesian inference tools for Python
 Home-page: http://bayespy.org
 Author: Jaakko Luttinen
 Author-email: jaakko.luttinen@iki.fi
 License: UNKNOWN
 Description: BayesPy - Bayesian Python
         =========================
@@ -23,27 +23,27 @@
         Markov chain Monte Carlo (MCMC) and other methods. Contributions are
         welcome.
         
         
         Project information
         -------------------
         
-        Copyright (C) 2011-2016 Jaakko Luttinen and other contributors (see below)
+        Copyright (C) 2011-2017 Jaakko Luttinen and other contributors (see below)
         
         BayesPy including the documentation is licensed under the MIT License. See
         LICENSE file for a text of the license or visit
         http://opensource.org/licenses/MIT.
         
         .. |chat| image:: https://badges.gitter.im/Join%20Chat.svg
            :target: https://gitter.im/bayespy/bayespy?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge
         .. |release| image:: https://badge.fury.io/py/bayespy.svg
            :target: https://pypi.python.org/pypi/bayespy
         
         ============== =============================================
-        Latest release |release| 
+        Latest release |release|
         Documentation  http://bayespy.org
         Repository     https://github.com/bayespy/bayespy.git
         Bug reports    https://github.com/bayespy/bayespy/issues
         Author         Jaakko Luttinen jaakko.luttinen@iki.fi
         Chat           |chat|
         Mailing list   bayespy@googlegroups.com
         ============== =============================================
@@ -73,15 +73,15 @@
         
         ==================== =============== ============== =============
         Branch               Test status     Test coverage  Documentation
         ==================== =============== ============== =============
         **master (stable)**  |travismaster|  |covermaster|  |docsmaster|
         **develop (latest)** |travisdevelop| |coverdevelop| |docsdevelop|
         ==================== =============== ============== =============
-         
+        
         
         Similar projects
         ----------------
         
         `VIBES <http://vibes.sourceforge.net/>`_
         (http://vibes.sourceforge.net/) allows variational inference to be
         performed automatically on a Bayesian network.  It is implemented in
@@ -131,14 +131,16 @@
         
         * Hannu Hartikainen
         
         * Deebul Nair
         
         * Christopher Cramer
         
+        * Till Hoffmann
+        
         Each file or the git log can be used for more detailed information.
         
 Keywords: variational Bayes,probabilistic programming,Bayesian networks,graphical models,variational message passing
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
```

### Comparing `bayespy-0.5.8/setup.py` & `bayespy-0.5.9/setup.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/tests/test_plot.py` & `bayespy-0.5.9/bayespy/tests/test_plot.py`

 * *Files 7% similar despite different names*

```diff
@@ -165,7 +165,17 @@
     Q = VB(Y, B, tau)
     Q.update(repeat=1000)
     xh = np.linspace(-5, 15, 100)
     Xh = np.vstack([xh, np.ones(len(xh))]).T
     Fh = SumMultiply('i,i', B, Xh)
 
     return locals()
+
+
+def test_ellipse_from_cov():
+    xy = np.random.normal(0, 1, 2)
+    cov = [[1, 0.5], [0.5, 1]]
+    ellipse = bpplt.ellipse_from_cov(xy, cov)
+    assert ellipse.angle == 135
+    np.testing.assert_allclose(ellipse.height, 2.4494897427831779)
+    np.testing.assert_allclose(ellipse.width, 1.4142135623730951)
+    np.testing.assert_allclose(xy, ellipse.center)
```

### Comparing `bayespy-0.5.8/bayespy/tests/baseline_images/test_plot/hinton_z.png` & `bayespy-0.5.9/bayespy/tests/baseline_images/test_plot/hinton_z.png`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/tests/baseline_images/test_plot/hinton_r.png` & `bayespy-0.5.9/bayespy/tests/baseline_images/test_plot/hinton_r.png`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/tests/baseline_images/test_plot/hinton_p.png` & `bayespy-0.5.9/bayespy/tests/baseline_images/test_plot/hinton_p.png`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/tests/baseline_images/test_plot/pdf.png` & `bayespy-0.5.9/bayespy/tests/baseline_images/test_plot/pdf.png`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/utils/tests/test_misc.py` & `bayespy-0.5.9/bayespy/utils/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/utils/tests/test_linalg.py` & `bayespy-0.5.9/bayespy/utils/tests/test_linalg.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/utils/tests/test_random.py` & `bayespy-0.5.9/bayespy/utils/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/utils/random.py` & `bayespy-0.5.9/bayespy/utils/random.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/utils/linalg.py` & `bayespy-0.5.9/bayespy/utils/linalg.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/utils/optimize.py` & `bayespy-0.5.9/bayespy/utils/optimize.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/utils/covfunc/covariance.py` & `bayespy-0.5.9/bayespy/utils/covfunc/covariance.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/utils/misc.py` & `bayespy-0.5.9/bayespy/utils/misc.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/testing.py` & `bayespy-0.5.9/bayespy/testing.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/discrete_example.py` & `bayespy-0.5.9/bayespy/discrete_example.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/nodes/__init__.py` & `bayespy-0.5.9/bayespy/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/plot.py` & `bayespy-0.5.9/bayespy/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,16 @@
    :toctree: generated/
 
    pdf
    contour
    plot
    hinton
    gaussian_mixture_2d
+   ellipse_from_cov
+   ellipse_from_precision
 
 Plotters
 ========
 
 .. autosummary::
    :toctree: generated/
 
@@ -54,14 +56,15 @@
 import numpy as np
 import scipy.sparse as sp
 import scipy
 from scipy import special
 import matplotlib.pyplot as plt
 from matplotlib import animation
 from matplotlib import colors
+from matplotlib import patches
 #from matplotlib.pyplot import *
 
 from bayespy.inference.vmp.nodes.categorical import CategoricalMoments
 from bayespy.inference.vmp.nodes.gaussian import (GaussianMoments,
                                                   GaussianWishartMoments)
 from bayespy.inference.vmp.nodes.beta import BetaMoments
 from bayespy.inference.vmp.nodes.beta import DirichletMoments
@@ -199,15 +202,15 @@
             name = Z.name
         except AttributeError:
             pass
 
     if name:
         axes.set_title(r'$q(%s)$' % (name))
         axes.set_xlabel(r'$%s$' % (name))
-        
+
     return retval
 
 
 def contour(Z, x, y, n=None, axes=None, fig=None, **kwargs):
     """
     Plot 2-D probability density function of a 2-D variable.
 
@@ -244,21 +247,21 @@
     Y = np.reshape(XY[:,1], shape)
     P = np.reshape(p, shape)
     if n is not None:
         levels = np.linspace(0, np.amax(P), num=n+2)[1:-1]
         return axes.contour(X, Y, P, levels, **kwargs)
     else:
         return axes.contour(X, Y, P, **kwargs)
-        
+
 
 
 def plot_gaussian_mc(X, scale=2, **kwargs):
     """
     Plot Gaussian Markov chain as a 1-D function
-    
+
     Parameters
     ----------
     X : node
         Node with Gaussian Markov chain moments.
     """
     timeseries_gaussian(X, axis=-2, scale=scale, **kwargs)
 
@@ -272,29 +275,29 @@
     z = u_X[0]
     return _timeseries_mean_and_error(z, None, axis=axis, **kwargs)
 
 
 def plot_gaussian(X, axis=-1, scale=2, **kwargs):
     """
     Plot Gaussian node as a 1-D function
-    
+
     Parameters
     ----------
     X : node
         Node with Gaussian moments.
     axis : int
         The index of the time axis.
     """
     X = X._ensure_moments(X, GaussianMoments, ndim=0)
     u_X = X.get_moments()
     x = u_X[0]
     xx = misc.get_diag(u_X[1], ndim=len(X.dims[0]))
     std = scale * np.sqrt(xx - x**2)
     #std = scale * np.sqrt(np.einsum('...ii->...i', xx) - x**2)
-    
+
     return _timeseries_mean_and_error(x, std, axis=axis, **kwargs)
 
 
 def plot(Y, axis=-1, scale=2, center=False, **kwargs):
     """
     Plot a variable or an array as 1-D function with errorbars
     """
@@ -317,19 +320,19 @@
         except GaussianMoments.NoConverterError:
             pass
         else:
             return plot_gaussian(Y, axis=axis, scale=scale, center=center, **kwargs)
 
     (mu, var) = Y.get_mean_and_variance()
     std = np.sqrt(var)
-    
-    return _timeseries_mean_and_error(mu, std, 
+
+    return _timeseries_mean_and_error(mu, std,
                                       axis=axis,
                                       scale=scale,
-                                      center=center, 
+                                      center=center,
                                       **kwargs)
 
 
 # Some backward compatibility
 def timeseries_gaussian_mc(*args, center=True, **kwargs):
     return plot_gaussian_mc(*args, center=center, **kwargs)
 def timeseries_gaussian(*args, center=True, **kwargs):
@@ -352,15 +355,15 @@
     # Get and remove the length of the time axis
     T = shape.pop(axis)
 
     # Move time axis to first
     y = np.rollaxis(y, axis)
     if std is not None:
         std = np.rollaxis(std, axis)
-    
+
     y = np.reshape(y, (T, -1))
     if std is not None:
         std = np.reshape(std, (T, -1))
 
     # Remove 1s
     shape = [s for s in shape if s > 1]
 
@@ -424,15 +427,15 @@
     xcorners = np.array([x - hs, x + hs, x + hs, x - hs])
     ycorners = np.array([y - hs, y - hs, y + hs, y + hs])
     axes.fill(xcorners, ycorners, colour, edgecolor=colour)
 
 def _rectangle(axes, x, y, width, height, **kwargs):
     _x = x - width/2
     _y = y - height/2
-    rectangle = plt.Rectangle((_x, _y), 
+    rectangle = plt.Rectangle((_x, _y),
                               width,
                               height,
                               **kwargs)
     axes.add_patch(rectangle)
     return
 
 
@@ -447,26 +450,26 @@
 
     alpha : Dirichlet-like node (optional)
        Probabilities for the clusters
 
     scale : float (optional)
        Scale for the covariance ellipses (by default, 2)
     """
-        
+
     if axes is None:
         axes = plt.gca()
 
     mu_Lambda = X._ensure_moments(X.parents[1], GaussianWishartMoments)
 
     (mu, _, Lambda, _) = mu_Lambda.get_moments()
     mu = np.linalg.solve(Lambda, mu)
 
     if len(mu_Lambda.plates) != 1:
         raise NotImplementedError("Not yet implemented for more plates")
-    
+
     K = mu_Lambda.plates[0]
 
     width = np.zeros(K)
     height = np.zeros(K)
     angle = np.zeros(K)
 
     for k in range(K):
@@ -507,21 +510,21 @@
     # If observed, plot the data too
     if np.any(X.observed):
         mask = np.array(X.observed) * np.ones(X.plates, dtype=np.bool)
         y = X.u[0][mask]
         plt.plot(y[:,0], y[:,1], 'r.')
 
     return
-    
-    
+
+
 def _hinton(W, error=None, vmax=None, square=False, axes=None):
     """
-    Draws a Hinton diagram for visualizing a weight matrix. 
+    Draws a Hinton diagram for visualizing a weight matrix.
 
-    Temporarily disables matplotlib interactive mode if it is on, 
+    Temporarily disables matplotlib interactive mode if it is on,
     otherwise this takes forever.
 
     Originally copied from
     http://wiki.scipy.org/Cookbook/Matplotlib/HintonDiagrams
     """
 
     if axes is None:
@@ -562,46 +565,46 @@
                     print(e, _w, vmax)
                     raise Exception("BUG? Negative error")
                 if _w + e > vmax:
                     print(e, _w, vmax)
                     raise Exception("BUG? Value+error greater than max")
                 _rectangle(axes,
                            _x,
-                           _y, 
+                           _y,
                            min(1, np.sqrt((_w+e)/vmax)),
                            min(1, np.sqrt((_w+e)/vmax)),
                            edgecolor=_c,
                            fill=False)
             _blob(axes, _x, _y, min(1, _w/vmax), _c)
-                
+
 
 def matrix(A, axes=None):
 
     if axes is None:
         axes = plt.gca()
 
     A = np.atleast_2d(A)
     vmax = np.max(np.abs(A))
-    return  axes.imshow(A, 
-                        interpolation='nearest', 
+    return  axes.imshow(A,
+                        interpolation='nearest',
                         cmap='RdBu_r',
                         vmin=-vmax,
                         vmax=vmax)
 
 def new_matrix(A, vmax=None):
     A = np.atleast_2d(A)
     if vmax is None:
         vmax = np.max(np.abs(A))
 
     (M, N) = np.shape(A)
 
     for i in range(M):
         for j in range(N):
             pass
-    
+
 def gaussian_hinton(X, rows=None, cols=None, scale=1, fig=None):
     """
     Plot the Hinton diagram of a Gaussian node
     """
 
     if fig is None:
         fig = plt.gcf()
@@ -668,15 +671,15 @@
 
     # Put the row and column axes to the end
     axes = [i for i in range(size) if i not in (rows, cols)] + [rows, cols]
     x = np.transpose(x, axes=axes)
     std = np.transpose(std, axes=axes)
 
     vmax = np.max(np.abs(x) + scale*std)
-    
+
     if scale == 0:
         _subplots(_hinton, (x, 2), fig=fig, kwargs=dict(vmax=vmax))
     else:
         def plotfunc(z, e, **kwargs):
             return _hinton(z, error=e, **kwargs)
 
         _subplots(plotfunc, (x, 2), (scale*std, 2), fig=fig, kwargs=dict(vmax=vmax))
@@ -812,15 +815,15 @@
     p = np.exp(P._message_to_child()[0][...,0])
 
     # Explicit broadcasting
     p = p * np.ones(P.plates)
 
     # Plot Hinton diagram
     return _hinton(p, vmax=1.0, square=square)
-    
+
 
 def dirichlet_hinton(P, square=True):
     """
     Plot a beta distributed random variable as a Hinton diagram
     """
 
     # Make sure that the node is beta
@@ -831,15 +834,15 @@
 
     # Explicit broadcasting
     p = p * np.ones(P.plates+(1,))
 
     # Plot Hinton diagram
     return _hinton(p, vmax=1.0, square=square)
 
-    
+
 def bernoulli_hinton(Z, square=True):
     """
     Plot a Bernoulli distributed random variable as a Hinton diagram
     """
 
     # Make sure that the node is Bernoulli
     Z = Z._ensure_moments(Z, BernoulliMoments)
@@ -848,15 +851,15 @@
     z = Z._message_to_child()[0]
 
     # Explicit broadcasting
     z = z * np.ones(Z.plates)
 
     # Plot Hinton diagram
     return _hinton(z, vmax=1.0, square=square)
-    
+
 
 def categorical_hinton(Z, square=True):
     """
     Plot a Bernoulli distributed random variable as a Hinton diagram
     """
 
     # Make sure that the node is Bernoulli
@@ -866,15 +869,15 @@
     z = Z._message_to_child()[0]
 
     # Explicit broadcasting
     z = z * np.ones(Z.plates+(1,))
 
     # Plot Hinton diagram
     return _hinton(np.squeeze(z), vmax=1.0, square=square)
-    
+
 
 def hinton(X, **kwargs):
     r"""
     Plot the Hinton diagram of a node
 
     The keyword arguments depend on the node type.  For some node types, the
     diagram also shows uncertainty with non-filled rectangles.  Currently,
@@ -928,24 +931,24 @@
             X = X._ensure_moments(X, CategoricalMoments, categories=None)
         except Moments.NoConverterError:
             pass
         else:
             return categorical_hinton(X, **kwargs)
 
     return _hinton_figure(X, **kwargs)
-    
+
 
 class Plotter():
     r"""
     Wrapper for plotting functions and base class for node plotters
 
     The purpose of this class is to collect all the parameters needed by a
     plotting function and provide a callable interface which needs only the node
     as the input.
-    
+
     Plotter instances are callable objects that plot a given node using a
     specified plotting function.
 
     Parameters
     ----------
 
     plotter : function
@@ -960,44 +963,44 @@
 
         Additional keyword arguments supported by the plotting function
 
     Examples
     --------
 
     First, create a gamma variable:
-    
+
     >>> import numpy as np
     >>> from bayespy.nodes import Gamma
     >>> x = Gamma(4, 5)
 
     The probability density function can be plotted as:
 
     >>> import bayespy.plot as bpplt
     >>> bpplt.pdf(x, np.linspace(0.1, 10, num=100))         # doctest: +ELLIPSIS
     [<matplotlib.lines.Line2D object at 0x...>]
 
     However, this can be problematic when one needs to provide a
     plotting function for the inference engine as the inference engine
     gives only the node as input.  Thus, we need to create a simple
     plotter wrapper:
-    
+
     >>> p = bpplt.Plotter(bpplt.pdf, np.linspace(0.1, 10, num=100))
 
     Now, this callable object ``p`` needs only the node as the input:
 
     >>> p(x)                                                # doctest: +ELLIPSIS
     [<matplotlib.lines.Line2D object at 0x...>]
 
     Thus, it can be given to the inference engine to use as a plotting function:
 
     >>> x = Gamma(4, 5, plotter=p)
     >>> x.plot()                                            # doctest: +ELLIPSIS
     [<matplotlib.lines.Line2D object at 0x...>]
     """
-    
+
 
     def __init__(self, plotter, *args, **kwargs):
         self._args = args
         self._kwargs = kwargs
         self._plotter = plotter
 
 
@@ -1012,15 +1015,15 @@
 
             The plotted node
         """
         kwargs_all = self._kwargs.copy()
         kwargs_all.update(kwargs)
         return self._plotter(X, *self._args, fig=fig, **kwargs_all)
 
-        
+
 class PDFPlotter(Plotter):
     r"""
     Plotter of probability density function of a scalar node
 
     Parameters
     ----------
 
@@ -1139,15 +1142,15 @@
         return (x, s)
 
     anim = animation.FuncAnimation(fig, animate,
                                    frames=np.shape(A)[0],
                                    interval=1000/fps,
                                    blit=False,
                                    repeat=False)
-        
+
     return anim
 
 
 def save_animation(anim, filename, fps=25, bitrate=5000, fig=None):
 
     # A bug in numpy/matplotlib causes this not to work in python3.3:
     # https://github.com/matplotlib/matplotlib/issues/1891
@@ -1157,15 +1160,15 @@
     # anim.save(filename, fps=fps)
 
     if fig is None:
         fig = plt.gcf()
 
     writer = animation.FFMpegFileWriter(fps=fps, bitrate=bitrate)
     writer.setup(fig, filename, 100)
-    anim.save(filename, 
+    anim.save(filename,
               fps=fps,
               writer=writer,
               bitrate=bitrate)
     return
 
 
 def binary_matrix(A, axes=None):
@@ -1205,16 +1208,16 @@
     # Log-determinant of Sigma:
     # Shape(ldet)  = (K,)
     ldet = linalg.chol_logdet(U)
 
     # Compute log pdf for each cluster:
     # Shape(lpdf)  = (N, K)
     lpdf = misc.gaussian_logpdf(z, 0, 0, ldet, D)
-    
-    
+
+
 
 def matrixplot(A, colorbar=False, axes=None):
     if axes is None:
         axes = plt.gca()
 
     if sp.issparse(A):
         A = A.toarray()
@@ -1222,26 +1225,26 @@
     if colorbar:
         plt.colorbar(ax=axes)
 
 
 def contourplot(x1, x2, y, colorbar=False, filled=True, axes=None):
     """ Plots 2D contour plot. x1 and x2 are 1D vectors, y contains
     the function values. y.size must be x1.size*x2.size. """
-    
+
     if axes is None:
         axes = plt.gca()
 
     y = np.reshape(y, (len(x2),len(x1)))
     if filled:
         axes.contourf(x1, x2, y)
     else:
         axes.contour(x1, x2, y)
     if colorbar:
         plt.colorbar(ax=axes)
-        
+
 
 def errorplot(y=None, error=None, x=None, lower=None, upper=None,
               color=(0,0,0,1), fillcolor=None, axes=None, **kwargs):
 
     if axes is None:
         axes = plt.gca()
 
@@ -1284,15 +1287,15 @@
     Creates a matrix of marginal plots.
 
     On diagonal, are marginal plots of each variable. Off-diagonal plot (i,j)
     shows the joint marginal density of x_i and x_j.
     """
     return X.plotmatrix()
 
-    
+
 def _pdf_t(mu, s2, nu, axes=None, scale=4, color='k'):
     """
     """
     if axes is None:
         axes = plt.gca()
 
     s = np.sqrt(s2)
@@ -1331,15 +1334,15 @@
     """
     if axes is None:
         axes = plt.gca()
 
     if np.shape(mu) != (2,) or np.shape(Cov) != (2,2) or np.shape(nu) != ():
         print(np.shape(mu), np.shape(Cov), np.shape(nu))
         raise ValueError("Only 2-d t-distribution allowed")
-    
+
     if transpose:
         mu = mu[[1,0]]
         Cov = Cov[np.ix_([1,0],[1,0])]
 
     s = np.sqrt(np.diag(Cov))
     x0 = np.linspace(mu[0]-scale*s[0], mu[0]+scale*s[0], num=100)
     x1 = np.linspace(mu[1]-scale*s[1], mu[1]+scale*s[1], num=100)
@@ -1358,7 +1361,54 @@
     return axes.contour(X0, X1, P, colors=colors)
 
 
 def _contour_gaussian_gamma(mu, s2, a, b, axes=None, transpose=False):
     """
     """
     pass
+
+
+def ellipse_from_cov(xy, cov, scale=2, **kwargs):
+    """
+    Create an ellipse from a covariance matrix.
+
+    Parameters
+    ----------
+    xy : np.ndarray
+        position of the ellipse
+    cov : np.ndarray
+        covariance matrix
+    scale : float
+        scale of the ellipse (default is three standard deviations)
+    kwargs : dict
+        keyword arguments passed on to `matplotlib.patches.Ellipse`
+
+    Returns
+    -------
+    ellipse : matplotlib.patches.Ellipse
+    """
+    evals, evecs = np.linalg.eigh(cov)
+    angle = np.arctan2(*evecs[::-1, 0])
+    width, height = scale * np.sqrt(evals)
+    return patches.Ellipse(xy, width, height, np.rad2deg(angle), **kwargs)
+
+
+def ellipse_from_precision(xy, precision, scale=2, **kwargs):
+    """
+    Create an ellipse from a covariance matrix.
+
+    Parameters
+    ----------
+    xy : np.ndarray
+        position of the ellipse
+    cov : np.ndarray
+        covariance matrix
+    scale : float
+        scale of the ellipse (default is three standard deviations)
+    kwargs : dict
+        keyword arguments passed on to `matplotlib.patches.Ellipse`
+
+    Returns
+    -------
+    ellipse : matplotlib.patches.Ellipse
+    """
+    return ellipse_from_cov(xy, np.linalg.inv(precision), scale, **kwargs)
```

### Comparing `bayespy-0.5.8/bayespy/models/pca.py` & `bayespy-0.5.9/bayespy/models/pca.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/demos/black_box.py` & `bayespy-0.5.9/bayespy/demos/black_box.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/demos/pattern_search.py` & `bayespy-0.5.9/bayespy/demos/pattern_search.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/demos/lssm_sd.py` & `bayespy-0.5.9/bayespy/demos/lssm_sd.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/demos/annealing.py` & `bayespy-0.5.9/bayespy/demos/annealing.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/demos/categorical.py` & `bayespy-0.5.9/bayespy/demos/categorical.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/demos/lssm_tvd.py` & `bayespy-0.5.9/bayespy/demos/lssm_tvd.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/demos/pca.py` & `bayespy-0.5.9/bayespy/demos/pca.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/demos/saving.py` & `bayespy-0.5.9/bayespy/demos/saving.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/demos/hmm.py` & `bayespy-0.5.9/bayespy/demos/hmm.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/demos/stochastic_inference.py` & `bayespy-0.5.9/bayespy/demos/stochastic_inference.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/demos/collapsed_cg.py` & `bayespy-0.5.9/bayespy/demos/collapsed_cg.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/demos/lssm.py` & `bayespy-0.5.9/bayespy/demos/lssm.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/demos/lda.py` & `bayespy-0.5.9/bayespy/demos/lda.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/demos/mog.py` & `bayespy-0.5.9/bayespy/demos/mog.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/tests/test_transformations.py` & `bayespy-0.5.9/bayespy/inference/vmp/tests/test_transformations.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/tests/test_annealing.py` & `bayespy-0.5.9/bayespy/inference/vmp/tests/test_annealing.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/transformations.py` & `bayespy-0.5.9/bayespy/inference/vmp/transformations.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/nodes/tests/test_poisson.py` & `bayespy-0.5.9/bayespy/inference/vmp/nodes/tests/test_poisson.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/nodes/tests/test_deterministic.py` & `bayespy-0.5.9/bayespy/inference/vmp/nodes/tests/test_deterministic.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/nodes/tests/test_wishart.py` & `bayespy-0.5.9/bayespy/inference/vmp/nodes/tests/test_wishart.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/nodes/tests/test_take.py` & `bayespy-0.5.9/bayespy/inference/vmp/nodes/tests/test_take.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/nodes/tests/test_bernoulli.py` & `bayespy-0.5.9/bayespy/inference/vmp/nodes/tests/test_bernoulli.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/nodes/tests/test_node.py` & `bayespy-0.5.9/bayespy/inference/vmp/nodes/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/nodes/tests/test_dirichlet.py` & `bayespy-0.5.9/bayespy/inference/vmp/nodes/tests/test_dirichlet.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/nodes/tests/test_gate.py` & `bayespy-0.5.9/bayespy/inference/vmp/nodes/tests/test_gate.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/nodes/tests/test_categorical_markov_chain.py` & `bayespy-0.5.9/bayespy/inference/vmp/nodes/tests/test_categorical_markov_chain.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/nodes/tests/test_concatenate.py` & `bayespy-0.5.9/bayespy/inference/vmp/nodes/tests/test_concatenate.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/nodes/tests/test_mixture.py` & `bayespy-0.5.9/bayespy/inference/vmp/nodes/tests/test_mixture.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/nodes/tests/test_gaussian_markov_chain.py` & `bayespy-0.5.9/bayespy/inference/vmp/nodes/tests/test_gaussian_markov_chain.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/nodes/tests/test_gaussian.py` & `bayespy-0.5.9/bayespy/inference/vmp/nodes/tests/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/nodes/tests/test_binomial.py` & `bayespy-0.5.9/bayespy/inference/vmp/nodes/tests/test_binomial.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/nodes/tests/test_beta.py` & `bayespy-0.5.9/bayespy/inference/vmp/nodes/tests/test_beta.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/nodes/tests/test_categorical.py` & `bayespy-0.5.9/bayespy/inference/vmp/nodes/tests/test_categorical.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/nodes/tests/test_gamma.py` & `bayespy-0.5.9/bayespy/inference/vmp/nodes/tests/test_gamma.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/nodes/tests/test_dot.py` & `bayespy-0.5.9/bayespy/inference/vmp/nodes/tests/test_dot.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/nodes/tests/test_multinomial.py` & `bayespy-0.5.9/bayespy/inference/vmp/nodes/tests/test_multinomial.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/nodes/categorical_markov_chain.py` & `bayespy-0.5.9/bayespy/inference/vmp/nodes/categorical_markov_chain.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/nodes/CovarianceFunctions.py` & `bayespy-0.5.9/bayespy/inference/vmp/nodes/CovarianceFunctions.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/nodes/newnode.py` & `bayespy-0.5.9/bayespy/inference/vmp/nodes/newnode.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/nodes/logistic.py` & `bayespy-0.5.9/bayespy/inference/vmp/nodes/logistic.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/nodes/concat_gaussian.py` & `bayespy-0.5.9/bayespy/inference/vmp/nodes/concat_gaussian.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/nodes/gaussian_markov_chain.py` & `bayespy-0.5.9/bayespy/inference/vmp/nodes/gaussian_markov_chain.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/nodes/beta.py` & `bayespy-0.5.9/bayespy/inference/vmp/nodes/beta.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/nodes/bernoulli.py` & `bayespy-0.5.9/bayespy/inference/vmp/nodes/bernoulli.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/nodes/gp.py` & `bayespy-0.5.9/bayespy/inference/vmp/nodes/gp.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/nodes/multinomial.py` & `bayespy-0.5.9/bayespy/inference/vmp/nodes/multinomial.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/nodes/constant.py` & `bayespy-0.5.9/bayespy/inference/vmp/nodes/constant.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/nodes/GaussianProcesses.py` & `bayespy-0.5.9/bayespy/inference/vmp/nodes/GaussianProcesses.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/nodes/logpdf.py` & `bayespy-0.5.9/bayespy/inference/vmp/nodes/logpdf.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/nodes/dot.py` & `bayespy-0.5.9/bayespy/inference/vmp/nodes/dot.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/nodes/categorical.py` & `bayespy-0.5.9/bayespy/inference/vmp/nodes/categorical.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/nodes/mixture.py` & `bayespy-0.5.9/bayespy/inference/vmp/nodes/mixture.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/nodes/__init__.py` & `bayespy-0.5.9/bayespy/inference/vmp/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/nodes/deterministic.py` & `bayespy-0.5.9/bayespy/inference/vmp/nodes/deterministic.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/nodes/point_estimate.py` & `bayespy-0.5.9/bayespy/inference/vmp/nodes/point_estimate.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/nodes/wishart.py` & `bayespy-0.5.9/bayespy/inference/vmp/nodes/wishart.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/nodes/gaussian.py` & `bayespy-0.5.9/bayespy/inference/vmp/nodes/gaussian.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/nodes/add.py` & `bayespy-0.5.9/bayespy/inference/vmp/nodes/add.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/nodes/ml.py` & `bayespy-0.5.9/bayespy/inference/vmp/nodes/ml.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/nodes/multinomial_probit.py` & `bayespy-0.5.9/bayespy/inference/vmp/nodes/multinomial_probit.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/nodes/binomial.py` & `bayespy-0.5.9/bayespy/inference/vmp/nodes/binomial.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/nodes/dirichlet.py` & `bayespy-0.5.9/bayespy/inference/vmp/nodes/dirichlet.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/nodes/concatenate.py` & `bayespy-0.5.9/bayespy/inference/vmp/nodes/concatenate.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/nodes/gamma.py` & `bayespy-0.5.9/bayespy/inference/vmp/nodes/gamma.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/nodes/expfamily.py` & `bayespy-0.5.9/bayespy/inference/vmp/nodes/expfamily.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/nodes/exponential.py` & `bayespy-0.5.9/bayespy/inference/vmp/nodes/exponential.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/nodes/stochastic.py` & `bayespy-0.5.9/bayespy/inference/vmp/nodes/stochastic.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/nodes/take.py` & `bayespy-0.5.9/bayespy/inference/vmp/nodes/take.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/nodes/gate.py` & `bayespy-0.5.9/bayespy/inference/vmp/nodes/gate.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/nodes/node.py` & `bayespy-0.5.9/bayespy/inference/vmp/nodes/node.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/nodes/converters.py` & `bayespy-0.5.9/bayespy/inference/vmp/nodes/converters.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/nodes/poisson.py` & `bayespy-0.5.9/bayespy/inference/vmp/nodes/poisson.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy/inference/vmp/vmp.py` & `bayespy-0.5.9/bayespy/inference/vmp/vmp.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,18 +23,18 @@
     r"""
     Variational Bayesian (VB) inference engine
 
     Parameters
     ----------
 
     nodes : nodes
-    
+
         Nodes that form the model. Must include all at least all stochastic
         nodes of the model.
-        
+
     tol : double, optional
 
         Convergence criterion.  Tolerance for the relative change in the VB
         lower bound.
 
     autosave_filename : string, optional
 
@@ -47,16 +47,16 @@
     callback : callable, optional
 
         Function which is called after each update iteration step
 
     """
 
     def __init__(self,
-                 *nodes, 
-                 tol=1e-5, 
+                 *nodes,
+                 tol=1e-5,
                  autosave_filename=None,
                  autosave_iterations=0,
                  use_logging=False,
                  user_data=None,
                  callback=None):
 
         self.user_data = user_data
@@ -67,28 +67,28 @@
 
         if use_logging:
             logger = logging.getLogger(__name__)
             self.print = logger.info
         else:
             # By default, don't use logging, just print stuff
             self.print = print
-            
+
         # Remove duplicate nodes
         self.model = misc.unique(nodes)
 
         self.ignore_bound_checks = False
 
         self._figures = {}
-        
+
         self.iter = 0
         self.annealing_changed = False
         self.converged = False
         self.L = np.array(())
         self.cputime = np.array(())
-        self.l = dict(zip(self.model, 
+        self.l = dict(zip(self.model,
                           len(self.model)*[np.array([])]))
         self.autosave_iterations = autosave_iterations
         self.autosave_nodes = None
         if not autosave_filename:
             date = datetime.datetime.today().strftime('%Y%m%d%H%M%S')
             prefix = 'vb_autosave_%s_' % date
             tmpfile = tempfile.NamedTemporaryFile(prefix=prefix,
@@ -126,15 +126,15 @@
         if iterations is not None:
             self.autosave_iterations = iterations
 
 
     def set_callback(self, callback):
         self.callback = callback
 
-    def update(self, *nodes, repeat=1, plot=False, tol=None, verbose=True):
+    def update(self, *nodes, repeat=1, plot=False, tol=None, verbose=True, tqdm=None):
 
         # TODO/FIXME:
         #
         # If no nodes are given and thus everything is updated, the update order
         # should be from down to bottom. Or something similar..
 
         # By default, update all nodes
@@ -152,27 +152,34 @@
         if (not self.ignore_bound_checks
             and all(~np.any(n.observed) for n in self.model)):
 
             raise Exception("At least one node in the model must be observed.")
 
         converged = False
 
-        for i in range(repeat):
+        if tqdm is not None:
+            tqdm = tqdm(total=repeat)
+        i = 0
+        while repeat is None or i < repeat:
 
             t = time.clock()
 
             # Update nodes
             for node in nodes:
                 X = self[node]
                 if hasattr(X, 'update') and callable(X.update):
                     X.update()
                 if X in plot_nodes:
                     self.plot(X)
 
             cputime = time.clock() - t
+            i += 1
+            if tqdm is not None:
+                tqdm.update()
+
             if self._end_iteration_step(None, cputime, tol=tol, verbose=verbose):
                 return
 
 
     def has_converged(self, tol=None):
         return self.converged
 
@@ -192,27 +199,27 @@
 
     def loglikelihood_lowerbound(self):
         L = 0
         for node in self.model:
             lp = node.lower_bound_contribution()
             L += lp
             self.l[node][self.iter] = lp
-            
+
         return L
 
     def plot_iteration_by_nodes(self, axes=None, diff=False):
         """
         Plot the cost function per node during the iteration.
 
         Handy tool for debugging.
         """
 
         if axes is None:
             axes = plt.gca()
-        
+
         D = len(self.l)
         N = self.iter + 1
         if diff:
             L = np.empty((N-1,D))
             x = np.arange(N-1) + 2
         else:
             L = np.empty((N,D))
@@ -239,21 +246,21 @@
         if len(nodes) == 0:
             nodes = self.model
         else:
             nodes = [self[node] for node in nodes if node is not None]
 
         if self.iter == 0:
             # Check HDF5 version.
-            if h5py.version.hdf5_version_tuple < (1,8,7): 
+            if h5py.version.hdf5_version_tuple < (1,8,7):
                 warnings.warn("WARNING! Your HDF5 version is %s. HDF5 versions "
                               "<1.8.7 are not able to save empty arrays, thus "
                               "you may experience problems if you for instance "
                               "try to save before running any iteration steps."
                               % str(h5py.version.hdf5_version_tuple))
-            
+
 
         # By default, use the same file as for auto-saving
         if not filename:
             if self.autosave_filename:
                 filename = self.autosave_filename
             else:
                 raise Exception("Filename must be given.")
@@ -272,15 +279,15 @@
                     node._save(nodegroup.create_group(node.name))
             # Write iteration statistics
             misc.write_to_hdf5(h5f, self.L, 'L')
             misc.write_to_hdf5(h5f, self.cputime, 'cputime')
             misc.write_to_hdf5(h5f, self.iter, 'iter')
             misc.write_to_hdf5(h5f, self.converged, 'converged')
             if self.callback_output is not None:
-                misc.write_to_hdf5(h5f, 
+                misc.write_to_hdf5(h5f,
                                    self.callback_output,
                                    'callback_output')
             boundgroup = h5f.create_group('boundterms')
             for node in nodes:
                 misc.write_to_hdf5(boundgroup, self.l[node], node.name)
             # Write user data
             if self.user_data is not None:
@@ -310,15 +317,15 @@
 
         # By default, use the same file as for auto-saving
         if not filename:
             if self.autosave_filename:
                 filename = self.autosave_filename
             else:
                 raise Exception("Filename must be given.")
-            
+
         # Open HDF5 file
         h5f = h5py.File(filename, 'r')
 
         try:
             # Get nodes to load
             if len(nodes) == 0:
                 nodes = self.model
@@ -350,22 +357,22 @@
                     self.callback_output = h5f['callback_output'][...]
                 except KeyError:
                     pass
 
         finally:
             # Close file
             h5f.close()
-        
+
     def __getitem__(self, name):
         if name in self.model:
             return name
         else:
             # Dictionary for mapping node names to nodes
             dictionary = {node.name: node for node in self.model}
-            return dictionary[name]        
+            return dictionary[name]
 
     def plot(self, *nodes, **kwargs):
         """
         Plot the distribution of the given nodes (or all nodes)
         """
 
         if len(nodes) == 0:
@@ -742,15 +749,15 @@
             if (L1 - L0) / div < tol:
             #if (L1 - L0) / div < tol or L1 - L0 <= 0:
                 if verbose:
                     self.print("Converged at iteration %d." % (self.iter+1))
                 self.converged = True
 
         # Auto-save, if requested
-        if (self.autosave_iterations > 0 
+        if (self.autosave_iterations > 0
             and np.mod(self.iter+1, self.autosave_iterations) == 0):
 
             if self.autosave_nodes is not None:
                 self.save(*self.autosave_nodes, filename=self.autosave_filename)
             else:
                 self.save(filename=self.autosave_filename)
             if verbose:
```

### Comparing `bayespy-0.5.8/bayespy/inference/__init__.py` & `bayespy-0.5.9/bayespy/inference/__init__.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/INSTALL.rst` & `bayespy-0.5.9/INSTALL.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_guide/engine.rst` & `bayespy-0.5.9/doc/source/dev_guide/engine.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_guide/vmp/vmp_gaussian.rst` & `bayespy-0.5.9/doc/source/dev_guide/vmp/vmp_gaussian.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_guide/vmp/vmp_wishart.rst` & `bayespy-0.5.9/doc/source/dev_guide/vmp/vmp_wishart.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_guide/vmp/vmp_mixture.rst` & `bayespy-0.5.9/doc/source/dev_guide/vmp/vmp_mixture.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_guide/writingnodes.rst` & `bayespy-0.5.9/doc/source/dev_guide/writingnodes.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_guide/vmp.rst` & `bayespy-0.5.9/doc/source/dev_guide/vmp.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_guide/workflow.rst` & `bayespy-0.5.9/doc/source/dev_guide/workflow.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_guide/advanced.rst` & `bayespy-0.5.9/doc/source/dev_guide/advanced.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_api/distributions.rst` & `bayespy-0.5.9/doc/source/dev_api/distributions.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGammaISO.rst` & `bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGammaISO.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.rst` & `bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamily.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianWishartDistribution.rst` & `bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianWishartDistribution.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.categorical.CategoricalDistribution.rst` & `bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.categorical.CategoricalDistribution.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.constant.Constant.rst` & `bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.constant.Constant.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianWishartMoments.rst` & `bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianWishartMoments.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.multinomial.MultinomialMoments.rst` & `bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.multinomial.MultinomialMoments.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISOMoments.rst` & `bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISOMoments.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDToGaussianWishart.rst` & `bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDToGaussianWishart.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.binomial.BinomialDistribution.rst` & `bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.binomial.BinomialDistribution.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.binomial.BinomialMoments.rst` & `bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.binomial.BinomialMoments.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.categorical_markov_chain.CategoricalMarkovChainMoments.rst` & `bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.categorical_markov_chain.CategoricalMarkovChainMoments.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGamma.rst` & `bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianToGaussianGamma.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.GaussianMarkovChainDistribution.rst` & `bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.GaussianMarkovChainDistribution.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGamma.rst` & `bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGamma.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.bernoulli.BernoulliDistribution.rst` & `bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.bernoulli.BernoulliDistribution.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.SwitchingGaussianMarkovChainDistribution.rst` & `bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.SwitchingGaussianMarkovChainDistribution.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.categorical.CategoricalMoments.rst` & `bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.categorical.CategoricalMoments.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.deterministic.Deterministic.rst` & `bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.deterministic.Deterministic.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.node.Node.rst` & `bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.node.Node.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_api/generated/bayespy.utils.misc.rst` & `bayespy-0.5.9/doc/source/dev_api/generated/bayespy.utils.misc.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.multinomial.MultinomialDistribution.rst` & `bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.multinomial.MultinomialDistribution.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gamma.GammaDistribution.rst` & `bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gamma.GammaDistribution.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaMoments.rst` & `bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaMoments.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_api/generated/generated/bayespy.utils.misc.TestCase.rst` & `bayespy-0.5.9/doc/source/dev_api/generated/generated/bayespy.utils.misc.TestCase.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_api/generated/bayespy.utils.random.rst` & `bayespy-0.5.9/doc/source/dev_api/generated/bayespy.utils.random.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamilyDistribution.rst` & `bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.expfamily.ExponentialFamilyDistribution.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.poisson.PoissonDistribution.rst` & `bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.poisson.PoissonDistribution.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.bernoulli.BernoulliMoments.rst` & `bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.bernoulli.BernoulliMoments.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDDistribution.rst` & `bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDDistribution.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaToGaussianWishart.rst` & `bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaToGaussianWishart.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.categorical_markov_chain.CategoricalMarkovChainDistribution.rst` & `bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.categorical_markov_chain.CategoricalMarkovChainDistribution.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISODistribution.rst` & `bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISODistribution.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaDistribution.rst` & `bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaDistribution.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.wishart.WishartDistribution.rst` & `bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.wishart.WishartDistribution.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaARD.rst` & `bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaARD.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianDistribution.rst` & `bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianDistribution.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaISO.rst` & `bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianGammaISO.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISOToGaussianGammaARD.rst` & `bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaISOToGaussianGammaARD.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianWishart.rst` & `bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.WrapToGaussianWishart.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianARDDistribution.rst` & `bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianARDDistribution.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDMoments.rst` & `bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianGammaARDMoments.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.VaryingGaussianMarkovChainDistribution.rst` & `bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.VaryingGaussianMarkovChainDistribution.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.stochastic.Distribution.rst` & `bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.stochastic.Distribution.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.beta.BetaDistribution.rst` & `bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.beta.BetaDistribution.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.GaussianMarkovChainMoments.rst` & `bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian_markov_chain.GaussianMarkovChainMoments.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.stochastic.Stochastic.rst` & `bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.stochastic.Stochastic.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianMoments.rst` & `bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.gaussian.GaussianMoments.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.dirichlet.DirichletDistribution.rst` & `bayespy-0.5.9/doc/source/dev_api/generated/bayespy.inference.vmp.nodes.dirichlet.DirichletDistribution.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_api/nodes.rst` & `bayespy-0.5.9/doc/source/dev_api/nodes.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/dev_api/moments.rst` & `bayespy-0.5.9/doc/source/dev_api/moments.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/_templates/autosummary/class.rst` & `bayespy-0.5.9/doc/source/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/_templates/autosummary/module.rst` & `bayespy-0.5.9/doc/source/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/conf.py` & `bayespy-0.5.9/doc/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -356,7 +356,10 @@
 
 # The depth of the table of contents in toc.ncx.
 #epub_tocdepth = 3
 
 # Allow duplicate toc entries.
 #epub_tocdup = True
 
+# Read the docs fails to import _tkinter so use Agg backend
+import matplotlib
+matplotlib.use('agg')
```

### Comparing `bayespy-0.5.8/doc/source/nodes.rst` & `bayespy-0.5.9/doc/source/nodes.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.nodes.GaussianARD.rst` & `bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.nodes.GaussianARD.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.inference.VB.rst` & `bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.inference.VB.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.nodes.Beta.rst` & `bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.nodes.Beta.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.nodes.Gaussian.rst` & `bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.nodes.Gaussian.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.nodes.Exponential.rst` & `bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.nodes.Exponential.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.nodes.Categorical.rst` & `bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.nodes.Categorical.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.rst` & `bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.nodes.VaryingGaussianMarkovChain.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.nodes.Bernoulli.rst` & `bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.nodes.Bernoulli.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.inference.vmp.transformations.RotateSwitchingMarkovChain.rst` & `bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.inference.vmp.transformations.RotateSwitchingMarkovChain.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.nodes.GaussianGamma.rst` & `bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.nodes.GaussianGamma.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.rst` & `bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.nodes.SwitchingGaussianMarkovChain.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.nodes.Poisson.rst` & `bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.nodes.Poisson.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.nodes.Wishart.rst` & `bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.nodes.Wishart.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.inference.vmp.transformations.RotateVaryingMarkovChain.rst` & `bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.inference.vmp.transformations.RotateVaryingMarkovChain.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.nodes.Add.rst` & `bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.nodes.Add.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.nodes.GaussianGammaARD.rst` & `bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.nodes.GaussianGammaARD.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.nodes.Function.rst` & `bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.nodes.Function.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.nodes.Dirichlet.rst` & `bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.nodes.Dirichlet.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.inference.vmp.transformations.RotateGaussianARD.rst` & `bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.inference.vmp.transformations.RotateGaussianARD.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.nodes.Gamma.rst` & `bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.nodes.Gamma.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.nodes.GaussianGammaISO.rst` & `bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.nodes.GaussianGammaISO.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.nodes.CategoricalMarkovChain.rst` & `bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.nodes.CategoricalMarkovChain.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.nodes.SumMultiply.rst` & `bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.nodes.SumMultiply.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.nodes.Take.rst` & `bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.nodes.Take.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.inference.vmp.transformations.RotateGaussianMarkovChain.rst` & `bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.inference.vmp.transformations.RotateGaussianMarkovChain.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.nodes.ConcatGaussian.rst` & `bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.nodes.ConcatGaussian.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.nodes.GaussianWishart.rst` & `bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.nodes.GaussianWishart.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.nodes.GaussianMarkovChain.rst` & `bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.nodes.GaussianMarkovChain.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.nodes.Mixture.rst` & `bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.nodes.Mixture.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.nodes.Multinomial.rst` & `bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.nodes.Multinomial.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.nodes.Binomial.rst` & `bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.nodes.Binomial.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/user_api/generated/generated/bayespy.nodes.Gate.rst` & `bayespy-0.5.9/doc/source/user_api/generated/generated/bayespy.nodes.Gate.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/examples/gmm.rst` & `bayespy-0.5.9/doc/source/examples/gmm.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/examples/additive_fhmm.rst` & `bayespy-0.5.9/doc/source/examples/additive_fhmm.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/examples/pca.rst` & `bayespy-0.5.9/doc/source/examples/pca.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/examples/bmm.rst` & `bayespy-0.5.9/doc/source/examples/bmm.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/examples/lda.rst` & `bayespy-0.5.9/doc/source/examples/lda.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/examples/hmm.rst` & `bayespy-0.5.9/doc/source/examples/hmm.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/examples/lssm.rst` & `bayespy-0.5.9/doc/source/examples/lssm.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/user_guide/modelconstruct.rst` & `bayespy-0.5.9/doc/source/user_guide/modelconstruct.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/user_guide/inference.rst` & `bayespy-0.5.9/doc/source/user_guide/inference.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/user_guide/quickstartbackup.rst` & `bayespy-0.5.9/doc/source/user_guide/quickstartbackup.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/user_guide/quickstart.rst` & `bayespy-0.5.9/doc/source/user_guide/quickstart.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/user_guide/quickstartbackup.py` & `bayespy-0.5.9/doc/source/user_guide/quickstartbackup.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/user_guide/advanced.rst` & `bayespy-0.5.9/doc/source/user_guide/advanced.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/source/user_guide/plot.rst` & `bayespy-0.5.9/doc/source/user_guide/plot.rst`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/doc/Makefile` & `bayespy-0.5.9/doc/Makefile`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/versioneer.py` & `bayespy-0.5.9/versioneer.py`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/README.rst` & `bayespy-0.5.9/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -15,27 +15,27 @@
 Markov chain Monte Carlo (MCMC) and other methods. Contributions are
 welcome.
 
 
 Project information
 -------------------
 
-Copyright (C) 2011-2016 Jaakko Luttinen and other contributors (see below)
+Copyright (C) 2011-2017 Jaakko Luttinen and other contributors (see below)
 
 BayesPy including the documentation is licensed under the MIT License. See
 LICENSE file for a text of the license or visit
 http://opensource.org/licenses/MIT.
 
 .. |chat| image:: https://badges.gitter.im/Join%20Chat.svg
    :target: https://gitter.im/bayespy/bayespy?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge
 .. |release| image:: https://badge.fury.io/py/bayespy.svg
    :target: https://pypi.python.org/pypi/bayespy
 
 ============== =============================================
-Latest release |release| 
+Latest release |release|
 Documentation  http://bayespy.org
 Repository     https://github.com/bayespy/bayespy.git
 Bug reports    https://github.com/bayespy/bayespy/issues
 Author         Jaakko Luttinen jaakko.luttinen@iki.fi
 Chat           |chat|
 Mailing list   bayespy@googlegroups.com
 ============== =============================================
@@ -65,15 +65,15 @@
 
 ==================== =============== ============== =============
 Branch               Test status     Test coverage  Documentation
 ==================== =============== ============== =============
 **master (stable)**  |travismaster|  |covermaster|  |docsmaster|
 **develop (latest)** |travisdevelop| |coverdevelop| |docsdevelop|
 ==================== =============== ============== =============
- 
+
 
 Similar projects
 ----------------
 
 `VIBES <http://vibes.sourceforge.net/>`_
 (http://vibes.sourceforge.net/) allows variational inference to be
 performed automatically on a Bayesian network.  It is implemented in
@@ -123,8 +123,10 @@
 
 * Hannu Hartikainen
 
 * Deebul Nair
 
 * Christopher Cramer
 
+* Till Hoffmann
+
 Each file or the git log can be used for more detailed information.
```

### Comparing `bayespy-0.5.8/LICENSE` & `bayespy-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bayespy-0.5.8/bayespy.egg-info/PKG-INFO` & `bayespy-0.5.9/bayespy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: bayespy
-Version: 0.5.8
+Version: 0.5.9
 Summary: Variational Bayesian inference tools for Python
 Home-page: http://bayespy.org
 Author: Jaakko Luttinen
 Author-email: jaakko.luttinen@iki.fi
 License: UNKNOWN
 Description: BayesPy - Bayesian Python
         =========================
@@ -23,27 +23,27 @@
         Markov chain Monte Carlo (MCMC) and other methods. Contributions are
         welcome.
         
         
         Project information
         -------------------
         
-        Copyright (C) 2011-2016 Jaakko Luttinen and other contributors (see below)
+        Copyright (C) 2011-2017 Jaakko Luttinen and other contributors (see below)
         
         BayesPy including the documentation is licensed under the MIT License. See
         LICENSE file for a text of the license or visit
         http://opensource.org/licenses/MIT.
         
         .. |chat| image:: https://badges.gitter.im/Join%20Chat.svg
            :target: https://gitter.im/bayespy/bayespy?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge
         .. |release| image:: https://badge.fury.io/py/bayespy.svg
            :target: https://pypi.python.org/pypi/bayespy
         
         ============== =============================================
-        Latest release |release| 
+        Latest release |release|
         Documentation  http://bayespy.org
         Repository     https://github.com/bayespy/bayespy.git
         Bug reports    https://github.com/bayespy/bayespy/issues
         Author         Jaakko Luttinen jaakko.luttinen@iki.fi
         Chat           |chat|
         Mailing list   bayespy@googlegroups.com
         ============== =============================================
@@ -73,15 +73,15 @@
         
         ==================== =============== ============== =============
         Branch               Test status     Test coverage  Documentation
         ==================== =============== ============== =============
         **master (stable)**  |travismaster|  |covermaster|  |docsmaster|
         **develop (latest)** |travisdevelop| |coverdevelop| |docsdevelop|
         ==================== =============== ============== =============
-         
+        
         
         Similar projects
         ----------------
         
         `VIBES <http://vibes.sourceforge.net/>`_
         (http://vibes.sourceforge.net/) allows variational inference to be
         performed automatically on a Bayesian network.  It is implemented in
@@ -131,14 +131,16 @@
         
         * Hannu Hartikainen
         
         * Deebul Nair
         
         * Christopher Cramer
         
+        * Till Hoffmann
+        
         Each file or the git log can be used for more detailed information.
         
 Keywords: variational Bayes,probabilistic programming,Bayesian networks,graphical models,variational message passing
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
```

### Comparing `bayespy-0.5.8/bayespy.egg-info/SOURCES.txt` & `bayespy-0.5.9/bayespy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

