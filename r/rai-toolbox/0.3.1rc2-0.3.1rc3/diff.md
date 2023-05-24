# Comparing `tmp/rai_toolbox-0.3.1rc2.tar.gz` & `tmp/rai_toolbox-0.3.1rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rai_toolbox-0.3.1rc2.tar", last modified: Fri May 12 13:00:03 2023, max compression
+gzip compressed data, was "rai_toolbox-0.3.1rc3.tar", last modified: Wed May 24 23:36:24 2023, max compression
```

## Comparing `rai_toolbox-0.3.1rc2.tar` & `rai_toolbox-0.3.1rc3.tar`

### file list

```diff
@@ -1,228 +1,223 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.468278 rai_toolbox-0.3.1rc2/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.408277 rai_toolbox-0.3.1rc2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.412277 rai_toolbox-0.3.1rc2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/.github/workflows/nightly.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/.github/workflows/publish_docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/.github/workflows/publish_rai_experiments.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/.github/workflows/pypi_publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/.github/workflows/test_docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/.github/workflows/tox_run.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13258 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-05-12 13:00:03.468278 rai_toolbox-0.3.1rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/SPDX.spdx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.412277 rai_toolbox-0.3.1rc2/brand/
--rw-r--r--   0 runner    (1001) docker     (123)    39824 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/brand/logo_no_text.png
--rw-r--r--   0 runner    (1001) docker     (123)    11445 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/brand/logo_no_text_small.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.412277 rai_toolbox-0.3.1rc2/deps/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/deps/requirements-pyright.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.412277 rai_toolbox-0.3.1rc2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/conda_env.yml
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.416277 rai_toolbox-0.3.1rc2/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.416277 rai_toolbox-0.3.1rc2/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    13493 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/_static/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/_static/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/_static/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/api_reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.416277 rai_toolbox-0.3.1rc2/docs/source/explanation/
--rw-r--r--   0 runner    (1001) docker     (123)     9832 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/explanation/perturbations.rst
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/explanation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.428277 rai_toolbox-0.3.1rc2/docs/source/generated/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.augmentations.augmix.AugMix.rst
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.augmentations.augmix.Fork.rst
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.augmentations.augmix.augment_and_mix.rst
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.augmentations.fourier.FourierBasis.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.augmentations.fourier.create_heatmaps.rst
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.augmentations.fourier.generate_fourier_bases.rst
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.datasets.CIFAR100C.rst
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.datasets.CIFAR10C.rst
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.datasets.CIFAR10P1.rst
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.datasets.ImageNet.rst
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.datasets.ImageNetM10.rst
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.datasets.RestrictedImageNet.rst
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.evaluating.rst
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.freeze.rst
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.frozen.rst
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.losses.jensen_shannon_divergence.rst
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.mushin.BaseWorkflow.rst
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.mushin.HydraDDP.rst
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.mushin.MetricsCallback.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.mushin.MultiRunMetricsWorkflow.rst
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.mushin.RobustnessCurve.rst
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.negate.rst
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.optim.ChainedParamTransformingOptimizer.rst
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.optim.ClampedGradientOptimizer.rst
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.optim.ClampedParameterOptimizer.rst
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.optim.FrankWolfe.rst
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.optim.L1FrankWolfe.rst
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.optim.L1NormedGradientOptim.rst
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.optim.L1qFrankWolfe.rst
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.optim.L1qNormedGradientOptim.rst
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.optim.L2FrankWolfe.rst
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.optim.L2NormedGradientOptim.rst
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.optim.L2ProjectedOptim.rst
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.optim.LinfFrankWolfe.rst
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.optim.LinfProjectedOptim.rst
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.optim.ParamTransformingOptimizer.rst
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.optim.SignedGradientOptim.rst
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.optim.TopQGradientOptimizer.rst
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.perturbations.AdditivePerturbation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.perturbations.PerturbationModel.rst
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.perturbations.gradient_ascent.rst
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.perturbations.random_restart.rst
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.perturbations.uniform_like_l1_n_ball_.rst
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.perturbations.uniform_like_l2_n_ball_.rst
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.perturbations.uniform_like_linf_n_ball_.rst
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.to_batch.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.428277 rai_toolbox-0.3.1rc2/docs/source/how_to/
--rw-r--r--   0 runner    (1001) docker     (123)    10832 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/how_to/custom_optim.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/how_to/deterministic_workflow.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/how_to/hydraddp.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/how_to/univ_adv_pert.rst
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/how_tos.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/ref_augmentations.rst
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/ref_datasets.rst
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/ref_losses.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/ref_mushin.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/ref_optim.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/ref_perturbation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/ref_utils.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.432277 rai_toolbox-0.3.1rc2/docs/source/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)   253710 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/tutorials/Building-Workflows.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)  1202618 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/tutorials/CIFAR10-Adversarial-Perturbations.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   462921 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/tutorials/ImageNet-Concept-Probing.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/docs/source/tutorials.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.436277 rai_toolbox-0.3.1rc2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)  1196382 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/examples/CIFAR10-Adversarial-Perturbations.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)  2042525 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/examples/ImageNet-Concept-Probing.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   194591 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/examples/MNIST-Translation-Robustness.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.440277 rai_toolbox-0.3.1rc2/examples/fourier/
--rw-r--r--   0 runner    (1001) docker     (123)  1489515 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/examples/fourier/FourierBasisPerturbations.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/examples/fourier/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.440277 rai_toolbox-0.3.1rc2/experiments/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.444277 rai_toolbox-0.3.1rc2/experiments/adversarial_training/
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/adversarial_training/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    84317 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/adversarial_training/TestRobustness.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/adversarial_training/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/adversarial_training/solver.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/adversarial_training/test_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/adversarial_training/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.444277 rai_toolbox-0.3.1rc2/experiments/benchmarking/
--rw-r--r--   0 runner    (1001) docker     (123)    29132 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/benchmarking/benchmarks.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.448278 rai_toolbox-0.3.1rc2/experiments/madry/
--rw-r--r--   0 runner    (1001) docker     (123)   138231 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/madry/Experiments.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/madry/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   508348 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/madry/Visualizations.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4906 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/madry/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/madry/lightning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/madry/run.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/madry/test_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.404277 rai_toolbox-0.3.1rc2/experiments/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.448278 rai_toolbox-0.3.1rc2/experiments/src/rai_experiments/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/src/rai_experiments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.448278 rai_toolbox-0.3.1rc2/experiments/src/rai_experiments/models/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/src/rai_experiments/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/src/rai_experiments/models/_resnet_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/src/rai_experiments/models/pretrained.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/src/rai_experiments/models/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/src/rai_experiments/models/small_resnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.448278 rai_toolbox-0.3.1rc2/experiments/src/rai_experiments/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/src/rai_experiments/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33869 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/src/rai_experiments/utils/imagenet_labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/src/rai_experiments/utils/visualizations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.448278 rai_toolbox-0.3.1rc2/experiments/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/tests/test_rai_experiments.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.452278 rai_toolbox-0.3.1rc2/experiments/universal_perturbation/
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/universal_perturbation/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   248742 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/universal_perturbation/UniversalPerturbation.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/universal_perturbation/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/universal_perturbation/solver.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/universal_perturbation/test_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/universal_perturbation/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.456277 rai_toolbox-0.3.1rc2/experiments/xai/
--rw-r--r--   0 runner    (1001) docker     (123)   788118 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/xai/Example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/xai/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/xai/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/experiments/xai/test_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 13:00:03.468278 rai_toolbox-0.3.1rc2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.404277 rai_toolbox-0.3.1rc2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.456277 rai_toolbox-0.3.1rc2/src/rai_toolbox/
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/_typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.456277 rai_toolbox-0.3.1rc2/src/rai_toolbox/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     7659 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/_utils/itertools.py
--rw-r--r--   0 runner    (1001) docker     (123)     6746 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/_utils/stateful.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/_utils/tqdm.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-12 13:00:03.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.456277 rai_toolbox-0.3.1rc2/src/rai_toolbox/augmentations/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/augmentations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.456277 rai_toolbox-0.3.1rc2/src/rai_toolbox/augmentations/augmix/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/augmentations/augmix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/augmentations/augmix/_implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/augmentations/augmix/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.460278 rai_toolbox-0.3.1rc2/src/rai_toolbox/augmentations/fourier/
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/augmentations/fourier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/augmentations/fourier/_fourier_basis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/augmentations/fourier/_implementations.py
--rw-r--r--   0 runner    (1001) docker     (123)     9495 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/augmentations/fourier/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.460278 rai_toolbox-0.3.1rc2/src/rai_toolbox/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/datasets/_cifar10_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/datasets/_imagenet_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/datasets/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/datasets/cifar10_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11568 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/datasets/cifar_corruptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.460278 rai_toolbox-0.3.1rc2/src/rai_toolbox/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/losses/_jensen_shannon_divergence.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/losses/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.460278 rai_toolbox-0.3.1rc2/src/rai_toolbox/mushin/
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/mushin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/mushin/_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/mushin/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.464278 rai_toolbox-0.3.1rc2/src/rai_toolbox/mushin/lightning/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/mushin/lightning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/mushin/lightning/_pl_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/mushin/lightning/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    14095 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/mushin/lightning/launchers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.464278 rai_toolbox-0.3.1rc2/src/rai_toolbox/mushin/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/mushin/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/mushin/testing/lightning.py
--rw-r--r--   0 runner    (1001) docker     (123)    45121 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/mushin/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.464278 rai_toolbox-0.3.1rc2/src/rai_toolbox/optim/
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23073 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/optim/frank_wolfe.py
--rw-r--r--   0 runner    (1001) docker     (123)    26835 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/optim/lp_space.py
--rw-r--r--   0 runner    (1001) docker     (123)    13936 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/optim/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    32583 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/optim/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.468278 rai_toolbox-0.3.1rc2/src/rai_toolbox/perturbations/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/perturbations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9060 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/perturbations/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/perturbations/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    15842 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/perturbations/solvers.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 12:59:42.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:00:03.456277 rai_toolbox-0.3.1rc2/src/rai_toolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-05-12 13:00:03.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-05-12 13:00:03.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 13:00:03.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-12 13:00:03.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-12 13:00:03.000000 rai_toolbox-0.3.1rc2/src/rai_toolbox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:36:24.820600 rai_toolbox-0.3.1rc3/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:36:24.760594 rai_toolbox-0.3.1rc3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:36:24.764595 rai_toolbox-0.3.1rc3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/.github/workflows/nightly.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/.github/workflows/publish_docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/.github/workflows/publish_rai_experiments.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/.github/workflows/pypi_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/.github/workflows/test_docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/.github/workflows/tox_run.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13258 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-05-24 23:36:24.820600 rai_toolbox-0.3.1rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/SPDX.spdx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:36:24.764595 rai_toolbox-0.3.1rc3/brand/
+-rw-r--r--   0 runner    (1001) docker     (123)    39824 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/brand/logo_no_text.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11445 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/brand/logo_no_text_small.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:36:24.764595 rai_toolbox-0.3.1rc3/deps/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/deps/requirements-pyright.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:36:24.764595 rai_toolbox-0.3.1rc3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/conda_env.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:36:24.768595 rai_toolbox-0.3.1rc3/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:36:24.768595 rai_toolbox-0.3.1rc3/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    13493 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/_static/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/_static/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/_static/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/api_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:36:24.768595 rai_toolbox-0.3.1rc3/docs/source/explanation/
+-rw-r--r--   0 runner    (1001) docker     (123)     9832 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/explanation/perturbations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/explanation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:36:24.784597 rai_toolbox-0.3.1rc3/docs/source/generated/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/generated/rai_toolbox.augmentations.augmix.AugMix.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/generated/rai_toolbox.augmentations.augmix.Fork.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/generated/rai_toolbox.augmentations.augmix.augment_and_mix.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/generated/rai_toolbox.augmentations.fourier.FourierBasis.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/generated/rai_toolbox.augmentations.fourier.create_heatmaps.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/generated/rai_toolbox.augmentations.fourier.generate_fourier_bases.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/generated/rai_toolbox.datasets.CIFAR100C.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/generated/rai_toolbox.datasets.CIFAR10C.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/generated/rai_toolbox.datasets.CIFAR10P1.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/generated/rai_toolbox.datasets.ImageNet.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/generated/rai_toolbox.datasets.ImageNetM10.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/generated/rai_toolbox.datasets.RestrictedImageNet.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/generated/rai_toolbox.evaluating.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/generated/rai_toolbox.freeze.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/generated/rai_toolbox.frozen.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/generated/rai_toolbox.losses.jensen_shannon_divergence.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/generated/rai_toolbox.mushin.BaseWorkflow.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/generated/rai_toolbox.mushin.HydraDDP.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/generated/rai_toolbox.mushin.MetricsCallback.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/generated/rai_toolbox.mushin.MultiRunMetricsWorkflow.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/generated/rai_toolbox.mushin.RobustnessCurve.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/generated/rai_toolbox.negate.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/generated/rai_toolbox.optim.ChainedParamTransformingOptimizer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/generated/rai_toolbox.optim.ClampedGradientOptimizer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/generated/rai_toolbox.optim.ClampedParameterOptimizer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/generated/rai_toolbox.optim.FrankWolfe.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/generated/rai_toolbox.optim.L1FrankWolfe.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/generated/rai_toolbox.optim.L1NormedGradientOptim.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/generated/rai_toolbox.optim.L1qFrankWolfe.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/generated/rai_toolbox.optim.L1qNormedGradientOptim.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/generated/rai_toolbox.optim.L2FrankWolfe.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/generated/rai_toolbox.optim.L2NormedGradientOptim.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/generated/rai_toolbox.optim.L2ProjectedOptim.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/generated/rai_toolbox.optim.LinfFrankWolfe.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/generated/rai_toolbox.optim.LinfProjectedOptim.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/generated/rai_toolbox.optim.ParamTransformingOptimizer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/generated/rai_toolbox.optim.SignedGradientOptim.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/generated/rai_toolbox.optim.TopQGradientOptimizer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/generated/rai_toolbox.perturbations.AdditivePerturbation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/generated/rai_toolbox.perturbations.PerturbationModel.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/generated/rai_toolbox.perturbations.gradient_ascent.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/generated/rai_toolbox.perturbations.random_restart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/generated/rai_toolbox.perturbations.uniform_like_l1_n_ball_.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/generated/rai_toolbox.perturbations.uniform_like_l2_n_ball_.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/generated/rai_toolbox.perturbations.uniform_like_linf_n_ball_.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/generated/rai_toolbox.to_batch.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:36:24.784597 rai_toolbox-0.3.1rc3/docs/source/how_to/
+-rw-r--r--   0 runner    (1001) docker     (123)    10832 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/how_to/custom_optim.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/how_to/deterministic_workflow.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/how_to/hydraddp.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/how_to/univ_adv_pert.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/how_tos.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/ref_augmentations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/ref_datasets.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/ref_losses.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/ref_mushin.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/ref_optim.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/ref_perturbation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/ref_utils.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:36:24.788597 rai_toolbox-0.3.1rc3/docs/source/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)   253710 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/tutorials/Building-Workflows.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  1202618 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/tutorials/CIFAR10-Adversarial-Perturbations.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   462921 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/tutorials/ImageNet-Concept-Probing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/docs/source/tutorials.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:36:24.792597 rai_toolbox-0.3.1rc3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)  1196382 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/examples/CIFAR10-Adversarial-Perturbations.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  2042525 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/examples/ImageNet-Concept-Probing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   194591 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/examples/MNIST-Translation-Robustness.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:36:24.796598 rai_toolbox-0.3.1rc3/examples/fourier/
+-rw-r--r--   0 runner    (1001) docker     (123)  1489515 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/examples/fourier/FourierBasisPerturbations.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/examples/fourier/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:36:24.796598 rai_toolbox-0.3.1rc3/experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/experiments/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/experiments/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:36:24.800598 rai_toolbox-0.3.1rc3/experiments/adversarial_training/
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/experiments/adversarial_training/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    84317 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/experiments/adversarial_training/TestRobustness.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/experiments/adversarial_training/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/experiments/adversarial_training/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/experiments/adversarial_training/test_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/experiments/adversarial_training/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:36:24.800598 rai_toolbox-0.3.1rc3/experiments/benchmarking/
+-rw-r--r--   0 runner    (1001) docker     (123)    29132 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/experiments/benchmarking/benchmarks.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:36:24.800598 rai_toolbox-0.3.1rc3/experiments/madry/
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/experiments/madry/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11925 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/experiments/madry/madry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/experiments/madry/test_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/experiments/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/experiments/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:36:24.760594 rai_toolbox-0.3.1rc3/experiments/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:36:24.800598 rai_toolbox-0.3.1rc3/experiments/src/rai_experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/experiments/src/rai_experiments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:36:24.804599 rai_toolbox-0.3.1rc3/experiments/src/rai_experiments/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/experiments/src/rai_experiments/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/experiments/src/rai_experiments/models/_resnet_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/experiments/src/rai_experiments/models/pretrained.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/experiments/src/rai_experiments/models/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/experiments/src/rai_experiments/models/small_resnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:36:24.804599 rai_toolbox-0.3.1rc3/experiments/src/rai_experiments/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/experiments/src/rai_experiments/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33869 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/experiments/src/rai_experiments/utils/imagenet_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/experiments/src/rai_experiments/utils/visualizations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:36:24.804599 rai_toolbox-0.3.1rc3/experiments/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/experiments/tests/test_rai_experiments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:36:24.808599 rai_toolbox-0.3.1rc3/experiments/universal_perturbation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/experiments/universal_perturbation/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   248742 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/experiments/universal_perturbation/UniversalPerturbation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/experiments/universal_perturbation/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/experiments/universal_perturbation/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/experiments/universal_perturbation/test_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/experiments/universal_perturbation/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:36:24.812599 rai_toolbox-0.3.1rc3/experiments/xai/
+-rw-r--r--   0 runner    (1001) docker     (123)  1578920 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/experiments/xai/ConceptProbing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  1616920 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/experiments/xai/Perturbations.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/experiments/xai/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 23:36:24.820600 rai_toolbox-0.3.1rc3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:36:24.760594 rai_toolbox-0.3.1rc3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:36:24.812599 rai_toolbox-0.3.1rc3/src/rai_toolbox/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/src/rai_toolbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/src/rai_toolbox/_typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:36:24.816600 rai_toolbox-0.3.1rc3/src/rai_toolbox/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     7659 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/src/rai_toolbox/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/src/rai_toolbox/_utils/itertools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6746 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/src/rai_toolbox/_utils/stateful.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/src/rai_toolbox/_utils/tqdm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-24 23:36:24.000000 rai_toolbox-0.3.1rc3/src/rai_toolbox/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:36:24.816600 rai_toolbox-0.3.1rc3/src/rai_toolbox/augmentations/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/src/rai_toolbox/augmentations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:36:24.816600 rai_toolbox-0.3.1rc3/src/rai_toolbox/augmentations/augmix/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/src/rai_toolbox/augmentations/augmix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/src/rai_toolbox/augmentations/augmix/_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/src/rai_toolbox/augmentations/augmix/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:36:24.816600 rai_toolbox-0.3.1rc3/src/rai_toolbox/augmentations/fourier/
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/src/rai_toolbox/augmentations/fourier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/src/rai_toolbox/augmentations/fourier/_fourier_basis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/src/rai_toolbox/augmentations/fourier/_implementations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9495 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/src/rai_toolbox/augmentations/fourier/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:36:24.820600 rai_toolbox-0.3.1rc3/src/rai_toolbox/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/src/rai_toolbox/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/src/rai_toolbox/datasets/_cifar10_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/src/rai_toolbox/datasets/_imagenet_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/src/rai_toolbox/datasets/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/src/rai_toolbox/datasets/cifar10_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11568 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/src/rai_toolbox/datasets/cifar_corruptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:36:24.820600 rai_toolbox-0.3.1rc3/src/rai_toolbox/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/src/rai_toolbox/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/src/rai_toolbox/losses/_jensen_shannon_divergence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/src/rai_toolbox/losses/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:36:24.820600 rai_toolbox-0.3.1rc3/src/rai_toolbox/mushin/
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/src/rai_toolbox/mushin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/src/rai_toolbox/mushin/_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/src/rai_toolbox/mushin/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:36:24.820600 rai_toolbox-0.3.1rc3/src/rai_toolbox/mushin/lightning/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/src/rai_toolbox/mushin/lightning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/src/rai_toolbox/mushin/lightning/_pl_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/src/rai_toolbox/mushin/lightning/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14095 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/src/rai_toolbox/mushin/lightning/launchers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:36:24.820600 rai_toolbox-0.3.1rc3/src/rai_toolbox/mushin/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/src/rai_toolbox/mushin/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/src/rai_toolbox/mushin/testing/lightning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45121 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/src/rai_toolbox/mushin/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:36:24.820600 rai_toolbox-0.3.1rc3/src/rai_toolbox/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/src/rai_toolbox/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23073 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/src/rai_toolbox/optim/frank_wolfe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26835 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/src/rai_toolbox/optim/lp_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13936 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/src/rai_toolbox/optim/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32583 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/src/rai_toolbox/optim/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:36:24.820600 rai_toolbox-0.3.1rc3/src/rai_toolbox/perturbations/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/src/rai_toolbox/perturbations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9060 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/src/rai_toolbox/perturbations/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/src/rai_toolbox/perturbations/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15842 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/src/rai_toolbox/perturbations/solvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 23:36:10.000000 rai_toolbox-0.3.1rc3/src/rai_toolbox/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 23:36:24.812599 rai_toolbox-0.3.1rc3/src/rai_toolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-05-24 23:36:24.000000 rai_toolbox-0.3.1rc3/src/rai_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-05-24 23:36:24.000000 rai_toolbox-0.3.1rc3/src/rai_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 23:36:24.000000 rai_toolbox-0.3.1rc3/src/rai_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-24 23:36:24.000000 rai_toolbox-0.3.1rc3/src/rai_toolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-24 23:36:24.000000 rai_toolbox-0.3.1rc3/src/rai_toolbox.egg-info/top_level.txt
```

### Comparing `rai_toolbox-0.3.1rc2/.github/workflows/nightly.yml` & `rai_toolbox-0.3.1rc3/.github/workflows/nightly.yml`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/.github/workflows/publish_docs.yml` & `rai_toolbox-0.3.1rc3/.github/workflows/publish_docs.yml`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/.github/workflows/publish_rai_experiments.yml` & `rai_toolbox-0.3.1rc3/.github/workflows/publish_rai_experiments.yml`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/.github/workflows/pypi_publish.yml` & `rai_toolbox-0.3.1rc3/.github/workflows/pypi_publish.yml`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/.github/workflows/test_docs.yml` & `rai_toolbox-0.3.1rc3/.github/workflows/test_docs.yml`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/.github/workflows/tox_run.yml` & `rai_toolbox-0.3.1rc3/.github/workflows/tox_run.yml`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/.gitignore` & `rai_toolbox-0.3.1rc3/.gitignore`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+src/rai_toolbox/_version.py
+
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
 *.so
```

### Comparing `rai_toolbox-0.3.1rc2/CONTRIBUTING.md` & `rai_toolbox-0.3.1rc3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/LICENSE.txt` & `rai_toolbox-0.3.1rc3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/PKG-INFO` & `rai_toolbox-0.3.1rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rai_toolbox
-Version: 0.3.1rc2
+Version: 0.3.1rc3
 Summary: PyTorch-centric library for evaluating and enhancing the robustness of AI technologies
 Author: Olivia Brown, Michael Yee
 Author-email: Ryan Soklaski <rsoklaski@gmail.com>, Justin Goodwin <jgoodwin@ll.mit.edu>
 Maintainer-email: Ryan Soklaski <rsoklaski@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Massachusetts Institute of Technology
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rai_toolbox Version: 0.3.1rc2 Summary: PyTorch-
+Metadata-Version: 2.1 Name: rai_toolbox Version: 0.3.1rc3 Summary: PyTorch-
 centric library for evaluating and enhancing the robustness of AI technologies
 Author: Olivia Brown, Michael Yee Author-email: Ryan Soklaski
 gmail.com>, Justin Goodwin
 ll.mit.edu> Maintainer-email: Ryan Soklaski
 gmail.com> License: MIT License Copyright (c) 2023 Massachusetts Institute of
 Technology Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
```

### Comparing `rai_toolbox-0.3.1rc2/README.md` & `rai_toolbox-0.3.1rc3/README.md`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/brand/logo_no_text.png` & `rai_toolbox-0.3.1rc3/brand/logo_no_text.png`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/brand/logo_no_text_small.png` & `rai_toolbox-0.3.1rc3/brand/logo_no_text_small.png`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/docs/Makefile` & `rai_toolbox-0.3.1rc3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/docs/README.md` & `rai_toolbox-0.3.1rc3/docs/README.md`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/docs/make.bat` & `rai_toolbox-0.3.1rc3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/docs/source/_static/apple-touch-icon.png` & `rai_toolbox-0.3.1rc3/docs/source/_static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/docs/source/_static/favicon-16x16.png` & `rai_toolbox-0.3.1rc3/docs/source/_static/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/docs/source/_static/favicon-32x32.png` & `rai_toolbox-0.3.1rc3/docs/source/_static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/docs/source/api_reference.rst` & `rai_toolbox-0.3.1rc3/docs/source/api_reference.rst`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/docs/source/changes.rst` & `rai_toolbox-0.3.1rc3/docs/source/changes.rst`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/docs/source/conf.py` & `rai_toolbox-0.3.1rc3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/docs/source/explanation/perturbations.rst` & `rai_toolbox-0.3.1rc3/docs/source/explanation/perturbations.rst`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.mushin.BaseWorkflow.rst` & `rai_toolbox-0.3.1rc3/docs/source/generated/rai_toolbox.mushin.BaseWorkflow.rst`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.mushin.MultiRunMetricsWorkflow.rst` & `rai_toolbox-0.3.1rc3/docs/source/generated/rai_toolbox.mushin.MultiRunMetricsWorkflow.rst`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.mushin.RobustnessCurve.rst` & `rai_toolbox-0.3.1rc3/docs/source/generated/rai_toolbox.mushin.RobustnessCurve.rst`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/docs/source/generated/rai_toolbox.optim.ParamTransformingOptimizer.rst` & `rai_toolbox-0.3.1rc3/docs/source/generated/rai_toolbox.optim.ParamTransformingOptimizer.rst`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/docs/source/how_to/custom_optim.rst` & `rai_toolbox-0.3.1rc3/docs/source/how_to/custom_optim.rst`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/docs/source/how_to/deterministic_workflow.rst` & `rai_toolbox-0.3.1rc3/docs/source/how_to/deterministic_workflow.rst`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/docs/source/how_to/hydraddp.rst` & `rai_toolbox-0.3.1rc3/docs/source/how_to/hydraddp.rst`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/docs/source/how_to/univ_adv_pert.rst` & `rai_toolbox-0.3.1rc3/docs/source/how_to/univ_adv_pert.rst`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/docs/source/index.rst` & `rai_toolbox-0.3.1rc3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/docs/source/ref_augmentations.rst` & `rai_toolbox-0.3.1rc3/docs/source/ref_augmentations.rst`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/docs/source/ref_datasets.rst` & `rai_toolbox-0.3.1rc3/docs/source/ref_datasets.rst`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/docs/source/ref_mushin.rst` & `rai_toolbox-0.3.1rc3/docs/source/ref_mushin.rst`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/docs/source/ref_optim.rst` & `rai_toolbox-0.3.1rc3/docs/source/ref_optim.rst`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/docs/source/ref_perturbation.rst` & `rai_toolbox-0.3.1rc3/docs/source/ref_perturbation.rst`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/docs/source/tutorials/Building-Workflows.ipynb` & `rai_toolbox-0.3.1rc3/docs/source/tutorials/Building-Workflows.ipynb`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/docs/source/tutorials/CIFAR10-Adversarial-Perturbations.ipynb` & `rai_toolbox-0.3.1rc3/docs/source/tutorials/CIFAR10-Adversarial-Perturbations.ipynb`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/docs/source/tutorials/ImageNet-Concept-Probing.ipynb` & `rai_toolbox-0.3.1rc3/docs/source/tutorials/ImageNet-Concept-Probing.ipynb`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/docs/source/tutorials.rst` & `rai_toolbox-0.3.1rc3/docs/source/tutorials.rst`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/examples/CIFAR10-Adversarial-Perturbations.ipynb` & `rai_toolbox-0.3.1rc3/examples/CIFAR10-Adversarial-Perturbations.ipynb`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/examples/ImageNet-Concept-Probing.ipynb` & `rai_toolbox-0.3.1rc3/examples/ImageNet-Concept-Probing.ipynb`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/examples/MNIST-Translation-Robustness.ipynb` & `rai_toolbox-0.3.1rc3/examples/MNIST-Translation-Robustness.ipynb`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/examples/fourier/FourierBasisPerturbations.ipynb` & `rai_toolbox-0.3.1rc3/examples/fourier/FourierBasisPerturbations.ipynb`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/examples/fourier/utils.py` & `rai_toolbox-0.3.1rc3/examples/fourier/utils.py`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/experiments/LICENSE.txt` & `rai_toolbox-0.3.1rc3/experiments/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/experiments/README.md` & `rai_toolbox-0.3.1rc3/experiments/README.md`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/experiments/adversarial_training/README.md` & `rai_toolbox-0.3.1rc3/experiments/adversarial_training/README.md`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/experiments/adversarial_training/TestRobustness.ipynb` & `rai_toolbox-0.3.1rc3/experiments/adversarial_training/TestRobustness.ipynb`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/experiments/adversarial_training/configs.py` & `rai_toolbox-0.3.1rc3/experiments/adversarial_training/configs.py`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/experiments/adversarial_training/solver.py` & `rai_toolbox-0.3.1rc3/experiments/adversarial_training/solver.py`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/experiments/adversarial_training/test_experiment.py` & `rai_toolbox-0.3.1rc3/experiments/adversarial_training/test_experiment.py`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/experiments/adversarial_training/train.py` & `rai_toolbox-0.3.1rc3/experiments/adversarial_training/train.py`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/experiments/benchmarking/benchmarks.ipynb` & `rai_toolbox-0.3.1rc3/experiments/benchmarking/benchmarks.ipynb`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/experiments/madry/README.md` & `rai_toolbox-0.3.1rc3/experiments/madry/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -7,100 +7,73 @@
   - `mitll_cifar_l2_1_0`: A simplified data structure of the pre-trained model available via the [README](https://github.com/MadryLab/robustness/blob/master/README.rst). This is a ResNet-50 model trained with Projected Gradient Descent (PGD) using the $\ell_2$-norm with $\epsilon=1.0$
   - `mitll_restricted_imagenet_l2_3_0`: TA simplified data structure of the pre-trained model available via the [README](https://github.com/MadryLab/robust_representations/blob/master/README.md).  This is a ResNet-50 model trained with PGD using the $\ell_2$-norm with $\epsilon=3.0$.
 
 
 # Prerequisites
   - hydra-zen
   - torchvision
-  - PyTorch Lightning
   - torchmetrics
 
 ## Exeperiments
 
 
 ### CIFAR10
+
 Reproduce last column of "CIFAR10 L2-robust accuracy" table from https://github.com/MadryLab/robustness by executing PGD with multiple $\epsilon$ values and the robustly trained ResNet-50 model.  These results are for 20-step PGD with step size of `2.5 * ε-test / num_steps`.
 
-```
-PYTHONPATH=$PWD:$PYTHONPATH python run.py ckpt=mitll_cifar_l2_1_0.pt steps=20 epsilon=[0,0.25,0.5,1.0,2.0]
-```
+Experiment Configurations:
+    - standard: standard training (full dataset)
+    - robust: adversarial training (full dataset)
+    - standard_fast: standard training with only 100 examples
+    - robust_fast: adversarial training with only 100 examples
 
-or in an interactive python environment such as a notebook:
+1. CPU (single process)
 
-```python
-import os
+```bash
+$ python madry.py +experiment=standard_fast
+standard [0.9570, 0.1063, 0.0216, 0., 0.]
 
-import configs
-import hydra
-import pytorch_lightning as pl
-from rai_toolbox.mushin.workflows import RobustnessCurve
-
-# Need add current working directory to the python path
-os.environ["PYTHONPATH"] = f"{os.getcwd()}:{os.getenv('PYTHONPATH')}"
-
-# Implement the evaluation task for RobustnessCurv
-class MadryLabRobustness(RobustnessCurve):
-    @staticmethod
-    def task(
-        seed: int, trainer: pl.Trainer, module: pl.LightningModule
-    ) -> dict:
-        pl.seed_everything(seed)
-        trainer.test(module)
-        assert Path("test_metrics.pt").exists()
-        return tr.load("test_metrics.pt")
-
-robustness_job = MadryLabRobustness(configs.Config)
-robustness_job.run(
-    epsilon=[0, 0.25, 0.5, 1.0, 2.0],
-    ckpt="mitll_cifar_l2_1_0.pt"
-)
-robustness_job.plot("Test/Accuracy")
+$ python madry.py +experiment=robust_fast
+robust [0.8251, 0.7855, 0.6789, 0.4522, 0.1719]
 ```
 
-#### Results
-
-|Test-eps | Expected | rai_toolbox    |
-|---------|----------|----------------|
-| 0.0     | 82       | 82             |
-| 0.25    | 76       | 76             |
-| 0.5     | 69       | 69             |
-| 1.0     | 53       | 53             |
-| 2.0     | 15       | 19             |
-
-Small difference for $\epsilon=2.0$.
-
-#### Training a Standard and Robust Model
+2. Torch Distributed (2 GPU)
 
-To train a standard CIFAR-10 model:
+```bash
+$ torchrun --nproc_per_node=2 madry.py +experiment=standard_fast
+standard [0.9570, 0.0895, 0.0091, 0., 0.]
 
+$ torchrun --nproc_per_node=2 madry.py +experiment=standard_fast
+robust [0.8251, 0.7855, 0.6726, 0.4431, 0.1719]
 ```
-python run.py mushin/dataset=cifar10 mushin/model=cifar10_resnet50 +mushin/optim=cifar ~mushin/perturbation
-```
-
-To train a robust CIFAR-10 model:
-
-```
-python run.py mushin/dataset=cifar10 mushin/model=cifar10_resnet50 +mushin/optim=cifar mushin.perturbation.epsilon=1.0 mushin.perturbation.steps=7
-```
-
 
-### Restricted ImageNet
+3. Multiple Experiments (2 GPU)
 
-Reproduce test results shown in Appendix A.4 from https://arxiv.org/abs/1906.00945 by executing PGD with multiple $\epsilon$ values and the robustly trained ResNet-50 model. These results are for 20-step PGD with step size of `2.5 * ε-test / num_steps`.
+```bash
+$ torchrun --nproc_per_node=2 madry.py +experiment=robust,standard --multirun
+[2023-05-24 16:27:48,649][HYDRA] Launching 2 jobs locally
+[2023-05-24 16:27:48,649][HYDRA]        #0 : +experiment=robust
+robust [0.8158999681472778, 0.7568999528884888, 0.6894999742507935, 0.5347999334335327, 0.19189998507499695]
 
+[2023-05-24 16:28:00,911][HYDRA]        #1 : +experiment=standard
+standard [0.950700044631958, 0.09849999845027924, 0.002500000176951289, 0.0, 0.0]
 ```
-python run.py data_path=$HOME/.torch/data/imagenet/normal/val ckpt=mitll_restricted_imagenet_l2_3_0.pt mushin/dataset=restricted_imagenet mushin/model=resnet50 mushin.perturbation.steps=20 mushin.perturbation.epsilon=3 
-```
-
 #### Results
 
+Here are the results from the Madry Lab's Robustness Toolbox and the results from this experiment.
+
 |Test-eps | Expected | rai_toolbox    |
 |---------|----------|----------------|
-| 3.0     | 82       | 82             |
+| 0.0     | 82       | 82             |
+| 0.25    | 76       | 76             |
+| 0.5     | 69       | 69             |
+| 1.0     | 53       | 53             |
+| 2.0     | 15       | 19             |
 
+Small difference for $\epsilon=2.0$.
 
 
 ## 📄 Citations
 
 ```
 @misc{robustness,
    title={Robustness (Python Library)},
```

### Comparing `rai_toolbox-0.3.1rc2/experiments/madry/configs.py` & `rai_toolbox-0.3.1rc3/experiments/universal_perturbation/configs.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,199 +1,182 @@
 # Copyright 2023, MASSACHUSETTS INSTITUTE OF TECHNOLOGY
 # Subject to FAR 52.227-11 – Patent Rights – Ownership by the Contractor (May 2014).
 # SPDX-License-Identifier: MIT
 
-from pathlib import Path
-
 import pytorch_lightning as pl
-import torch
 from hydra.core.config_store import ConfigStore
-from hydra_zen import MISSING, make_config, make_custom_builds_fn
-from lightning import EvaluateModule
+from hydra_zen import MISSING, builds, make_config, make_custom_builds_fn
+from pytorch_lightning.callbacks import ModelCheckpoint
+from solver import UniversalPerturbationSolver
 from torch import nn
+from torch.nn import functional as F
 from torch.optim import SGD
-from torchvision import datasets, models, transforms
+from torch.utils.data.dataloader import DataLoader
+from torchvision import datasets, transforms
 
 from rai_experiments.models.small_resnet import resnet50 as cifar_resnet50
-from rai_toolbox import datasets as rai_datasets
+from rai_toolbox import negate
 from rai_toolbox.mushin import load_from_checkpoint
 from rai_toolbox.mushin.lightning import HydraDDP, MetricsCallback
-from rai_toolbox.optim import L2ProjectedOptim
-from rai_toolbox.perturbations import AdditivePerturbation, gradient_ascent
-from rai_toolbox.perturbations.init import uniform_like_l2_n_ball_
-
-###############
-# Custom Builds
-###############
-builds = make_custom_builds_fn()
+from rai_toolbox.optim import L1qFrankWolfe, L2ProjectedOptim
+from rai_toolbox.perturbations import AdditivePerturbation
+from rai_toolbox.perturbations.init import (
+    uniform_like_l1_n_ball_,
+    uniform_like_l2_n_ball_,
+)
+
+cs = ConfigStore.instance()
 pbuilds = make_custom_builds_fn(zen_partial=True)
 
 #########
 # Dataset
 #########
 CIFAR10Normalizer = builds(
     transforms.Normalize,
     mean=[0.4914, 0.4822, 0.4465],
     std=[0.2023, 0.1994, 0.2010],
 )
 
+CIFAR10Transforms = builds(
+    transforms.Compose,
+    [builds(transforms.RandomCrop, size=32, padding=4), builds(transforms.ToTensor)],
+)
+
 CIFAR10 = builds(
     datasets.CIFAR10,
-    root="${data_path}",
-    train=False,
+    root="${oc.env:HOME}/.torch/data",
+    train=True,
     download=True,
-    transform=builds(transforms.ToTensor),
-)
-
-ImageNetNormalizer = builds(
-    transforms.Normalize,
-    mean=[0.485, 0.456, 0.406],
-    std=[0.229, 0.224, 0.225],
+    transform=CIFAR10Transforms,
 )
 
-TestTransformImageNet = builds(
-    transforms.Compose,
-    [
-        builds(transforms.Resize, 256),
-        builds(transforms.CenterCrop, 224),
-        builds(transforms.ToTensor),
-    ],
-)
-
-RestrictedImageNet = builds(
-    rai_datasets.RestrictedImageNet,
-    root="${data_path}",
-    transform=TestTransformImageNet,
+TestCIFAR10 = builds(
+    datasets.CIFAR10,
+    root="${oc.env:HOME}/.torch/data",
+    train=False,
+    download=True,
+    transform=builds(transforms.ToTensor),
 )
 
 
 #######
 # Model
 #######
 LoadFromCheckpoint = builds(
     load_from_checkpoint,
     model=MISSING,
-    ckpt="${ckpt}",
+    ckpt=None,
     weights_key="state_dict",
     populate_full_signature=True,
 )
 
-CIFARResNet50 = builds(
-    load_from_checkpoint,
-    model=builds(cifar_resnet50),
-    builds_bases=(LoadFromCheckpoint,),
-)
-
-CIFARModel = builds(nn.Sequential, CIFAR10Normalizer, CIFARResNet50)
-
-RestictedImageNetResNet50 = builds(
-    load_from_checkpoint,
-    model=builds(models.resnet50, num_classes=9),
-    builds_bases=(LoadFromCheckpoint,),
+CIFARResNet50 = LoadFromCheckpoint(model=builds(cifar_resnet50), ckpt="${...ckpt}")
+CIFARModel = builds(
+    nn.Sequential,
+    CIFAR10Normalizer,
+    CIFARResNet50,
+    zen_meta=dict(ckpt="${oc.env:HOME}/.torch/models/${ckpt}.pt"),
 )
 
-RestictedImageNetModel = builds(
-    nn.Sequential, ImageNetNormalizer, RestictedImageNetResNet50
-)
-
-
-#####
-# PGD
-#####
-def get_stepsize(factor, steps, epsilon):
-    return factor * epsilon / steps
-
+###########
+# Optimizer
+###########
 
 L2PGOpt = pbuilds(
     L2ProjectedOptim,
     InnerOpt=SGD,
-    lr=builds(get_stepsize, factor=2.5, steps="${steps}", epsilon="${epsilon}"),
+    lr="${lr}",
     epsilon="${epsilon}",
+    param_ndim=None,  # ensure projection doesn't broadcast
 )
 
-PGDModel = pbuilds(
-    AdditivePerturbation, init_fn=pbuilds(uniform_like_l2_n_ball_, epsilon="${epsilon}")
+L1qFWOpt = pbuilds(
+    L1qFrankWolfe,
+    q=0.975,
+    lr=1.0,
+    epsilon="${epsilon}",
+    param_ndim=None,  # ensure grad transformation doesn't broadcast
 )
 
-L2PGD = pbuilds(
-    gradient_ascent,
-    # Type of Perturbation
-    perturbation_model=PGDModel,
-    # Optimizer (e.g., L2 PGD)
-    optimizer=L2PGOpt,
-    # solver parameters
-    steps="${steps}",
-    use_best=True,
-    targeted=False,
-    criterion=builds(torch.nn.CrossEntropyLoss, reduction="none"),
-)
 
+L2Init = pbuilds(uniform_like_l2_n_ball_)
+L1Init = pbuilds(uniform_like_l1_n_ball_)
+Perturbation = builds(AdditivePerturbation, data_or_shape=(3, 32, 32), init_fn=None)
+
+########
+# Solver
+########
+Criterion = builds(negate, F.cross_entropy)
+
+Solver = builds(
+    UniversalPerturbationSolver,
+    dataset="${dataset}",
+    val_dataset="${val_dataset}",
+    model="${model}",
+    optim=MISSING,
+    criterion=Criterion,
+    perturbation=Perturbation,
+)
 
-############
-# PL Trainer
-############
 Trainer = builds(
     pl.Trainer,
-    max_epochs=1,
-    num_nodes=1,
-    accelerator="gpu",
     devices="${gpus}",
+    max_epochs="${max_epochs}",
+    accelerator="gpu",
     strategy=builds(HydraDDP),
-    callbacks=[builds(MetricsCallback)],
+    callbacks=[
+        builds(MetricsCallback),
+        builds(
+            ModelCheckpoint,
+            monitor="Train/Loss",
+            save_last=True,
+            save_top_k=1,
+            filename="epoch_{epoch}",
+            auto_insert_metric_name=False,
+        ),
+    ],
     populate_full_signature=True,
 )
 
-Evaluator = builds(
-    EvaluateModule,
-    dataset="${dataset}",
-    model="${model}",
-    perturbation="${perturbation}",
-    criterion=builds(nn.CrossEntropyLoss),
-    batch_size="${batch_size}",
-    num_workers="${num_workers}",
-    hydra_convert="all",
-)
-
-
-######################################
-# Experiment Configs and Task Function
-# - Replaces config.yaml
-######################################
-NUM_GPUS = torch.cuda.device_count() if torch.cuda.is_available() else 0
-
+#########
+# Configs
+#########
 DatasetCfg = make_config(
-    data_path=str(Path.home() / ".torch" / "data"),
-    batch_size=256,
+    batch_size=128,
     num_workers=8,
-    dataset=MISSING,
-)
-
-ModelCfg = make_config(
-    ckpt=None,
-    model=MISSING,
-)
-
-PerturbationCfg = make_config(steps=7, perturbation=MISSING)
-TrainerCfg = make_config(gpus=NUM_GPUS, trainer=Trainer, module=Evaluator)
-
+    dataset=builds(
+        DataLoader,
+        CIFAR10,
+        batch_size="${batch_size}",
+        num_workers="${num_workers}",
+        shuffle=True,
+        pin_memory=True,
+    ),
+    val_dataset=builds(
+        DataLoader,
+        TestCIFAR10,
+        batch_size="${batch_size}",
+        num_workers="${num_workers}",
+        pin_memory=True,
+    ),
+)
+
+ModelCfg = make_config(ckpt="mitll_cifar_l2_1_0", model=CIFARModel)
+SolverCfg = make_config(lr=0.1, epsilon=0.0, init_fn=None, module=Solver)
+TrainerCfg = make_config(max_epochs=40, devices=2, trainer=Trainer)
 Config = make_config(
     defaults=[
         "_self_",
-        {"perturbation": "l2pgd"},
-        {"dataset": "cifar10"},
-        {"model": "cifar10_resnet50"},
+        {"module/optim": "l2pgd"},
+        {"module/perturbation/init_fn": "${module/optim}"},
     ],
-    seed=12219,
-    epsilon=0.0,
-    bases=(DatasetCfg, ModelCfg, PerturbationCfg, TrainerCfg),
+    random_seed=1223,
+    bases=(DatasetCfg, ModelCfg, SolverCfg, TrainerCfg),
 )
 
-
-###################
-# Swappable Configs
-###################
-cs = ConfigStore.instance()
-cs.store(group="dataset", name="cifar10", node=CIFAR10)
-cs.store(group="dataset", name="restricted_imagenet", node=RestrictedImageNet)
-cs.store(group="model", name="cifar10_resnet50", node=CIFARModel)
-cs.store(group="model", name="resnet50", node=RestictedImageNetModel)
-cs.store(group="perturbation", name="l2pgd", node=L2PGD)
+##########################
+# Swappable Configurations
+##########################
+cs.store(name="l2pg", group="module/optim", node=L2PGOpt)
+cs.store(name="l1qfw", group="module/optim", node=L1qFWOpt)
+cs.store(name="l2pg", group="module/perturbation/init_fn", node=L2Init)
+cs.store(name="l1qfw", group="module/perturbation/init_fn", node=L1Init)
```

### Comparing `rai_toolbox-0.3.1rc2/experiments/setup.cfg` & `rai_toolbox-0.3.1rc3/experiments/setup.cfg`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/experiments/src/rai_experiments/models/_resnet_blocks.py` & `rai_toolbox-0.3.1rc3/experiments/src/rai_experiments/models/_resnet_blocks.py`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/experiments/src/rai_experiments/models/pretrained.py` & `rai_toolbox-0.3.1rc3/experiments/src/rai_experiments/models/pretrained.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     .. [1] https://github.com/MadryLab/robustness
     .. [2] https://github.com/MadryLab/robust_representations
     """
 
     return _pre_trained_manager.fetch(model_name, progressbar=(tqdm is not None))
 
 
-def load_model(model_name: _MODEL_NAMES):
+def load_model(model_name: _MODEL_NAMES, **model_kwargs):
     r"""
     Loads pre-trained model weights. This function takes care of downloading and caching
     weights.
 
     All model weights were provided by Madry Lab [1]_. We converted these weights to a
     format that does not require extraneous dependencies, such as `dill`, to load.
 
@@ -136,14 +136,14 @@
         )
     else:
         raise ValueError(
             f"Unknown model name: {model_name}\nAvailable models: {', '.join(_pre_trained_manager.registry_files + ['imagenet_nat.pt'])}"
         )
 
     base_model = load_from_checkpoint(
-        model=model(),
+        model=model(**model_kwargs),
         ckpt=get_path_to_checkpoint(model_name),
         weights_key="state_dict" if model_name != "imagenet_nat.pt" else "model",
     )
 
     model = torch.nn.Sequential(norm, base_model)
     return model
```

### Comparing `rai_toolbox-0.3.1rc2/experiments/src/rai_experiments/models/resnet.py` & `rai_toolbox-0.3.1rc3/experiments/src/rai_experiments/models/resnet.py`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/experiments/src/rai_experiments/models/small_resnet.py` & `rai_toolbox-0.3.1rc3/experiments/src/rai_experiments/models/small_resnet.py`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/experiments/src/rai_experiments/utils/imagenet_labels.py` & `rai_toolbox-0.3.1rc3/experiments/src/rai_experiments/utils/imagenet_labels.py`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/experiments/src/rai_experiments/utils/visualizations.py` & `rai_toolbox-0.3.1rc3/experiments/src/rai_experiments/utils/visualizations.py`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/experiments/tests/test_rai_experiments.py` & `rai_toolbox-0.3.1rc3/experiments/tests/test_rai_experiments.py`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/experiments/universal_perturbation/README.md` & `rai_toolbox-0.3.1rc3/experiments/universal_perturbation/README.md`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/experiments/universal_perturbation/UniversalPerturbation.ipynb` & `rai_toolbox-0.3.1rc3/experiments/universal_perturbation/UniversalPerturbation.ipynb`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/experiments/universal_perturbation/solver.py` & `rai_toolbox-0.3.1rc3/experiments/universal_perturbation/solver.py`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/experiments/universal_perturbation/test_experiment.py` & `rai_toolbox-0.3.1rc3/experiments/universal_perturbation/test_experiment.py`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/experiments/universal_perturbation/train.py` & `rai_toolbox-0.3.1rc3/experiments/universal_perturbation/train.py`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/experiments/xai/README.md` & `rai_toolbox-0.3.1rc3/experiments/xai/README.md`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/pyproject.toml` & `rai_toolbox-0.3.1rc3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -230,9 +230,8 @@
 deps = 
        experiments/
 commands = 
    pytest experiments/tests
    pytest experiments/adversarial_training/test_experiment.py
    pytest experiments/madry/test_experiment.py
    pytest experiments/universal_perturbation/test_experiment.py
-   pytest experiments/xai/test_experiment.py
 """
```

### Comparing `rai_toolbox-0.3.1rc2/src/rai_toolbox/__init__.py` & `rai_toolbox-0.3.1rc3/src/rai_toolbox/__init__.py`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/src/rai_toolbox/_typing.py` & `rai_toolbox-0.3.1rc3/src/rai_toolbox/_typing.py`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/src/rai_toolbox/_utils/__init__.py` & `rai_toolbox-0.3.1rc3/src/rai_toolbox/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/src/rai_toolbox/_utils/itertools.py` & `rai_toolbox-0.3.1rc3/src/rai_toolbox/_utils/itertools.py`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/src/rai_toolbox/_utils/stateful.py` & `rai_toolbox-0.3.1rc3/src/rai_toolbox/_utils/stateful.py`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/src/rai_toolbox/_utils/tqdm.py` & `rai_toolbox-0.3.1rc3/src/rai_toolbox/_utils/tqdm.py`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/src/rai_toolbox/augmentations/augmix/_implementation.py` & `rai_toolbox-0.3.1rc3/src/rai_toolbox/augmentations/augmix/_implementation.py`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/src/rai_toolbox/augmentations/augmix/transforms.py` & `rai_toolbox-0.3.1rc3/src/rai_toolbox/augmentations/augmix/transforms.py`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/src/rai_toolbox/augmentations/fourier/_fourier_basis.py` & `rai_toolbox-0.3.1rc3/src/rai_toolbox/augmentations/fourier/_fourier_basis.py`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/src/rai_toolbox/augmentations/fourier/_implementations.py` & `rai_toolbox-0.3.1rc3/src/rai_toolbox/augmentations/fourier/_implementations.py`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/src/rai_toolbox/augmentations/fourier/transforms.py` & `rai_toolbox-0.3.1rc3/src/rai_toolbox/augmentations/fourier/transforms.py`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/src/rai_toolbox/datasets/_cifar10_base.py` & `rai_toolbox-0.3.1rc3/src/rai_toolbox/datasets/_cifar10_base.py`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/src/rai_toolbox/datasets/_imagenet_base.py` & `rai_toolbox-0.3.1rc3/src/rai_toolbox/datasets/_imagenet_base.py`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/src/rai_toolbox/datasets/_utils.py` & `rai_toolbox-0.3.1rc3/src/rai_toolbox/datasets/_utils.py`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/src/rai_toolbox/datasets/cifar10_extensions.py` & `rai_toolbox-0.3.1rc3/src/rai_toolbox/datasets/cifar10_extensions.py`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/src/rai_toolbox/datasets/cifar_corruptions.py` & `rai_toolbox-0.3.1rc3/src/rai_toolbox/datasets/cifar_corruptions.py`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/src/rai_toolbox/losses/_jensen_shannon_divergence.py` & `rai_toolbox-0.3.1rc3/src/rai_toolbox/losses/_jensen_shannon_divergence.py`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/src/rai_toolbox/losses/_utils.py` & `rai_toolbox-0.3.1rc3/src/rai_toolbox/losses/_utils.py`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/src/rai_toolbox/mushin/__init__.py` & `rai_toolbox-0.3.1rc3/src/rai_toolbox/mushin/__init__.py`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/src/rai_toolbox/mushin/_compatibility.py` & `rai_toolbox-0.3.1rc3/src/rai_toolbox/mushin/_compatibility.py`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/src/rai_toolbox/mushin/_utils.py` & `rai_toolbox-0.3.1rc3/src/rai_toolbox/mushin/_utils.py`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/src/rai_toolbox/mushin/lightning/_pl_main.py` & `rai_toolbox-0.3.1rc3/src/rai_toolbox/mushin/lightning/_pl_main.py`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/src/rai_toolbox/mushin/lightning/callbacks.py` & `rai_toolbox-0.3.1rc3/src/rai_toolbox/mushin/lightning/callbacks.py`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/src/rai_toolbox/mushin/lightning/launchers.py` & `rai_toolbox-0.3.1rc3/src/rai_toolbox/mushin/lightning/launchers.py`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/src/rai_toolbox/mushin/testing/lightning.py` & `rai_toolbox-0.3.1rc3/src/rai_toolbox/mushin/testing/lightning.py`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/src/rai_toolbox/mushin/workflows.py` & `rai_toolbox-0.3.1rc3/src/rai_toolbox/mushin/workflows.py`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/src/rai_toolbox/optim/__init__.py` & `rai_toolbox-0.3.1rc3/src/rai_toolbox/optim/__init__.py`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/src/rai_toolbox/optim/frank_wolfe.py` & `rai_toolbox-0.3.1rc3/src/rai_toolbox/optim/frank_wolfe.py`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/src/rai_toolbox/optim/lp_space.py` & `rai_toolbox-0.3.1rc3/src/rai_toolbox/optim/lp_space.py`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/src/rai_toolbox/optim/misc.py` & `rai_toolbox-0.3.1rc3/src/rai_toolbox/optim/misc.py`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/src/rai_toolbox/optim/optimizer.py` & `rai_toolbox-0.3.1rc3/src/rai_toolbox/optim/optimizer.py`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/src/rai_toolbox/perturbations/__init__.py` & `rai_toolbox-0.3.1rc3/src/rai_toolbox/perturbations/__init__.py`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/src/rai_toolbox/perturbations/init.py` & `rai_toolbox-0.3.1rc3/src/rai_toolbox/perturbations/init.py`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/src/rai_toolbox/perturbations/models.py` & `rai_toolbox-0.3.1rc3/src/rai_toolbox/perturbations/models.py`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/src/rai_toolbox/perturbations/solvers.py` & `rai_toolbox-0.3.1rc3/src/rai_toolbox/perturbations/solvers.py`

 * *Files identical despite different names*

### Comparing `rai_toolbox-0.3.1rc2/src/rai_toolbox.egg-info/PKG-INFO` & `rai_toolbox-0.3.1rc3/src/rai_toolbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rai-toolbox
-Version: 0.3.1rc2
+Version: 0.3.1rc3
 Summary: PyTorch-centric library for evaluating and enhancing the robustness of AI technologies
 Author: Olivia Brown, Michael Yee
 Author-email: Ryan Soklaski <rsoklaski@gmail.com>, Justin Goodwin <jgoodwin@ll.mit.edu>
 Maintainer-email: Ryan Soklaski <rsoklaski@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Massachusetts Institute of Technology
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rai-toolbox Version: 0.3.1rc2 Summary: PyTorch-
+Metadata-Version: 2.1 Name: rai-toolbox Version: 0.3.1rc3 Summary: PyTorch-
 centric library for evaluating and enhancing the robustness of AI technologies
 Author: Olivia Brown, Michael Yee Author-email: Ryan Soklaski
 gmail.com>, Justin Goodwin
 ll.mit.edu> Maintainer-email: Ryan Soklaski
 gmail.com> License: MIT License Copyright (c) 2023 Massachusetts Institute of
 Technology Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
```

### Comparing `rai_toolbox-0.3.1rc2/src/rai_toolbox.egg-info/SOURCES.txt` & `rai_toolbox-0.3.1rc3/src/rai_toolbox.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -105,20 +105,16 @@
 experiments/adversarial_training/README.md
 experiments/adversarial_training/TestRobustness.ipynb
 experiments/adversarial_training/configs.py
 experiments/adversarial_training/solver.py
 experiments/adversarial_training/test_experiment.py
 experiments/adversarial_training/train.py
 experiments/benchmarking/benchmarks.ipynb
-experiments/madry/Experiments.ipynb
 experiments/madry/README.md
-experiments/madry/Visualizations.ipynb
-experiments/madry/configs.py
-experiments/madry/lightning.py
-experiments/madry/run.py
+experiments/madry/madry.py
 experiments/madry/test_experiment.py
 experiments/src/rai_experiments/__init__.py
 experiments/src/rai_experiments/models/__init__.py
 experiments/src/rai_experiments/models/_resnet_blocks.py
 experiments/src/rai_experiments/models/pretrained.py
 experiments/src/rai_experiments/models/resnet.py
 experiments/src/rai_experiments/models/small_resnet.py
@@ -128,18 +124,17 @@
 experiments/tests/test_rai_experiments.py
 experiments/universal_perturbation/README.md
 experiments/universal_perturbation/UniversalPerturbation.ipynb
 experiments/universal_perturbation/configs.py
 experiments/universal_perturbation/solver.py
 experiments/universal_perturbation/test_experiment.py
 experiments/universal_perturbation/train.py
-experiments/xai/Example.ipynb
+experiments/xai/ConceptProbing.ipynb
+experiments/xai/Perturbations.ipynb
 experiments/xai/README.md
-experiments/xai/configs.py
-experiments/xai/test_experiment.py
 src/rai_toolbox/__init__.py
 src/rai_toolbox/_typing.py
 src/rai_toolbox/_version.py
 src/rai_toolbox/py.typed
 src/rai_toolbox.egg-info/PKG-INFO
 src/rai_toolbox.egg-info/SOURCES.txt
 src/rai_toolbox.egg-info/dependency_links.txt
```

