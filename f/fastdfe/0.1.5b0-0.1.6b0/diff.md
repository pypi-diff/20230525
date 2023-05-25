# Comparing `tmp/fastdfe-0.1.5b0.tar.gz` & `tmp/fastdfe-0.1.6b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastdfe-0.1.5b0.tar", max compression
+gzip compressed data, was "fastdfe-0.1.6b0.tar", max compression
```

## Comparing `fastdfe-0.1.5b0.tar` & `fastdfe-0.1.6b0.tar`

### file list

```diff
@@ -1,19 +1,22 @@
--rw-r--r--   0        0        0      795 2023-05-11 10:05:21.534399 fastdfe-0.1.5b0/README.md
--rw-r--r--   0        0        0     2570 2023-05-11 10:05:21.702400 fastdfe-0.1.5b0/fastdfe/__init__.py
--rw-r--r--   0        0        0    20068 2023-05-11 10:05:21.706400 fastdfe-0.1.5b0/fastdfe/abstract_inference.py
--rw-r--r--   0        0        0    45394 2023-05-11 10:05:21.706400 fastdfe-0.1.5b0/fastdfe/base_inference.py
--rw-r--r--   0        0        0     4869 2023-05-11 10:05:21.706400 fastdfe-0.1.5b0/fastdfe/bootstrap.py
--rw-r--r--   0        0        0    10146 2023-05-11 10:05:21.706400 fastdfe-0.1.5b0/fastdfe/config.py
--rw-r--r--   0        0        0    15067 2023-05-11 10:05:21.706400 fastdfe-0.1.5b0/fastdfe/discretization.py
--rw-r--r--   0        0        0    41939 2023-05-11 10:05:21.706400 fastdfe-0.1.5b0/fastdfe/joint_inference.py
--rw-r--r--   0        0        0     3902 2023-05-11 10:05:21.706400 fastdfe-0.1.5b0/fastdfe/json_handlers.py
--rw-r--r--   0        0        0     1541 2023-05-11 10:05:21.706400 fastdfe-0.1.5b0/fastdfe/mle.py
--rw-r--r--   0        0        0    36389 2023-05-11 10:05:21.706400 fastdfe-0.1.5b0/fastdfe/optimization.py
--rw-r--r--   0        0        0    21093 2023-05-11 10:05:21.706400 fastdfe-0.1.5b0/fastdfe/parametrization.py
--rw-r--r--   0        0        0    19733 2023-05-11 10:05:21.706400 fastdfe-0.1.5b0/fastdfe/parser.py
--rw-r--r--   0        0        0    12485 2023-05-11 10:05:21.706400 fastdfe-0.1.5b0/fastdfe/polydfe.py
--rw-r--r--   0        0        0     5254 2023-05-11 10:05:21.706400 fastdfe-0.1.5b0/fastdfe/polydfe_utils.py
--rw-r--r--   0        0        0    17957 2023-05-11 10:05:21.706400 fastdfe-0.1.5b0/fastdfe/spectrum.py
--rw-r--r--   0        0        0    28157 2023-05-11 10:05:21.706400 fastdfe-0.1.5b0/fastdfe/visualization.py
--rw-r--r--   0        0        0      642 2023-05-11 10:05:21.706400 fastdfe-0.1.5b0/pyproject.toml
--rw-r--r--   0        0        0     1820 1970-01-01 00:00:00.000000 fastdfe-0.1.5b0/PKG-INFO
+-rw-r--r--   0        0        0      881 2023-05-25 06:14:31.511946 fastdfe-0.1.6b0/README.md
+-rw-r--r--   0        0        0     4933 2023-05-25 06:14:31.675947 fastdfe-0.1.6b0/fastdfe/__init__.py
+-rw-r--r--   0        0        0    20069 2023-05-25 06:14:31.675947 fastdfe-0.1.6b0/fastdfe/abstract_inference.py
+-rw-r--r--   0        0        0    31181 2023-05-25 06:14:31.675947 fastdfe-0.1.6b0/fastdfe/annotation.py
+-rw-r--r--   0        0        0    48780 2023-05-25 06:14:31.679947 fastdfe-0.1.6b0/fastdfe/base_inference.py
+-rw-r--r--   0        0        0     4869 2023-05-25 06:14:31.679947 fastdfe-0.1.6b0/fastdfe/bootstrap.py
+-rw-r--r--   0        0        0    10468 2023-05-25 06:14:31.679947 fastdfe-0.1.6b0/fastdfe/config.py
+-rw-r--r--   0        0        0    15069 2023-05-25 06:14:31.679947 fastdfe-0.1.6b0/fastdfe/discretization.py
+-rw-r--r--   0        0        0     9215 2023-05-25 06:14:31.679947 fastdfe-0.1.6b0/fastdfe/filtration.py
+-rw-r--r--   0        0        0    44110 2023-05-25 06:14:31.679947 fastdfe-0.1.6b0/fastdfe/joint_inference.py
+-rw-r--r--   0        0        0     3902 2023-05-25 06:14:31.679947 fastdfe-0.1.6b0/fastdfe/json_handlers.py
+-rw-r--r--   0        0        0     2484 2023-05-25 06:14:31.679947 fastdfe-0.1.6b0/fastdfe/mle.py
+-rw-r--r--   0        0        0    37834 2023-05-25 06:14:31.679947 fastdfe-0.1.6b0/fastdfe/optimization.py
+-rw-r--r--   0        0        0    21679 2023-05-25 06:14:31.679947 fastdfe-0.1.6b0/fastdfe/parametrization.py
+-rw-r--r--   0        0        0    27820 2023-05-25 06:14:31.679947 fastdfe-0.1.6b0/fastdfe/parser.py
+-rw-r--r--   0        0        0    12485 2023-05-25 06:14:31.679947 fastdfe-0.1.6b0/fastdfe/polydfe.py
+-rw-r--r--   0        0        0     5254 2023-05-25 06:14:31.679947 fastdfe-0.1.6b0/fastdfe/polydfe_utils.py
+-rw-r--r--   0        0        0    22109 2023-05-25 06:14:31.679947 fastdfe-0.1.6b0/fastdfe/spectrum.py
+-rw-r--r--   0        0        0     8492 2023-05-25 06:14:31.679947 fastdfe-0.1.6b0/fastdfe/vcf.py
+-rw-r--r--   0        0        0    28670 2023-05-25 06:14:31.679947 fastdfe-0.1.6b0/fastdfe/visualization.py
+-rw-r--r--   0        0        0     1084 2023-05-25 06:14:31.679947 fastdfe-0.1.6b0/pyproject.toml
+-rw-r--r--   0        0        0     2027 1970-01-01 00:00:00.000000 fastdfe-0.1.6b0/PKG-INFO
```

### Comparing `fastdfe-0.1.5b0/README.md` & `fastdfe-0.1.6b0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,8 @@
-[![fastDFE](https://github.com/Sendrowski/fastDFE/actions/workflows/python-app.yml/badge.svg?branch=master)](https://github.com/Sendrowski/fastDFE/actions/workflows/python-app.yml)
+[![tests](https://github.com/Sendrowski/fastDFE/actions/workflows/run-tests.yml/badge.svg?branch=master)](https://github.com/Sendrowski/fastDFE/actions/workflows/run-tests.yml)
 [![codecov](https://codecov.io/gh/Sendrowski/fastDFE/branch/master/graph/badge.svg?token=0LUE8SZYBJ)](https://codecov.io/gh/Sendrowski/fastDFE)
 [![Documentation Status](https://readthedocs.org/projects/fastdfe/badge/?version=latest)](https://fastdfe.readthedocs.io/en/latest/?badge=latest)
+[![PyPI version](https://badge.fury.io/py/fastdfe.svg)](https://badge.fury.io/py/fastdfe)
 
 fastDFE is a new package designed for inferring the distribution of fitness effects (DFE) from site-frequency spectra (SFS). As it is currently in its beta phase, we are continuously working to improve and refine its features.
 
 Please see the [documentation](https://fastdfe.readthedocs.io/en/latest/) for all the details.
```

### Comparing `fastdfe-0.1.5b0/fastdfe/abstract_inference.py` & `fastdfe-0.1.6b0/fastdfe/abstract_inference.py`

 * *Files 0% similar despite different names*

```diff
@@ -397,15 +397,15 @@
 
         :param model: DFE parametrization
         :param params: Parameters of the model
         :param intervals: Array of interval boundaries yielding ``intervals.shape[0] - 1`` bins.
         :return: Discretized DFE
         """
         # discrete DFE
-        y = from_string(model).discretize(params, intervals)
+        y = from_string(model)._discretize(params, intervals)
 
         # return normalized histogram
         return y / y.sum()
 
 
 class AbstractInference(ABC):
     """
```

### Comparing `fastdfe-0.1.5b0/fastdfe/base_inference.py` & `fastdfe-0.1.6b0/fastdfe/base_inference.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,16 +40,41 @@
 
 
 class BaseInference(AbstractInference):
     """
     Base inference class for inferring the SFS given one neutral and one selected SFS.
     Note that BaseInference is by default seeded.
 
-    .. warning::
-        TODO add confidence intervals for inferred SFS.
+    Basic usage:
+
+    ::
+
+        from fastdfe import Spectrum, BaseInference
+
+        sfs_neut = Spectrum([177130, 997, 441, 228, 156, 117, 114, 83, 105, 109, 652])
+        sfs_sel = Spectrum([797939, 1329, 499, 265, 162, 104, 117, 90, 94, 119, 794])
+
+        # create inference object
+        inf = BaseInference(
+            sfs_neut=sfs_neut,
+            sfs_sel=sfs_sel,
+            n_runs=10,
+            n_bootstraps=100,
+            do_bootstrap=True
+        )
+
+        # run inference
+        inf.run()
+
+        # plot discretized DFE
+        inf.plot_discretized()
+
+        # plot SFS comparison
+        inf.plot_sfs_comparison()
+
     """
 
     #: Default parameters not connected to the DFE parametrization
     default_x0 = dict(
         eps=0.0
     )
 
@@ -61,16 +86,16 @@
     #: Scales for the parameters not connected to the DFE parametrization
     default_scales = dict(
         eps='lin'
     )
 
     #: Default options for the MLE
     default_opts_mle = dict(
-        # ftol=1e-20,
-        # gtol=1e-20
+        # ftol=1e-10,
+        # gtol=1e-10
     )
 
     def __init__(
             self,
             sfs_neut: Spectra | Spectrum,
             sfs_sel: Spectra | Spectrum,
             intervals_del: (float, float, int) = (-1.0e+8, -1.0e-5, 1000),
@@ -85,45 +110,54 @@
             loss_type: Literal['likelihood', 'L2'] = 'likelihood',
             opts_mle: dict = {},
             n_runs: int = 10,
             fixed_params: Dict[str, Dict[str, float]] = {},
             do_bootstrap: bool = False,
             n_bootstraps: int = 100,
             parallelize: bool = True,
+            folded: bool = None,
             discretization: Discretization = None,
             optimization: Optimization = None,
             locked: bool = False,
             **kwargs
     ):
         """
         Create BaseInference instance.
 
         :param sfs_neut: The neutral SFS. Note that we require monomorphic counts to be specified in order to infer
-            the mutation rate.
+            the mutation rate. If a ``Spectra`` object with more than one SFS is provided, the ``all`` attribute will be
+            used.
         :param sfs_sel: The selected SFS. Note that we require monomorphic counts to be specified in order to infer
-            the mutation rate.
+            the mutation rate. If a ``Spectra`` object with more than one SFS is provided, the ``all`` attribute will be
+            used.
         :param intervals_del: ``(start, stop, n_interval)`` for deleterious population-scaled
             selection coefficients. The intervals will be log10-spaced.
+        :param integration_mode: Integration mode for the DFE, ``quad`` not recommended
+        :param linearized: Whether to use the linearized DFE, ``False`` not recommended
         :param intervals_ben: Same as for intervals_del but for beneficial selection coefficients.
         :param model: Instance of DFEParametrization which parametrized the DFE
         :param seed: Seed for the random number generator.
-        :param x0: Dictionary of initial values in the form {'all': {param: value}}
-        :param bounds: Bounds for the optimization in the form {param: (lower, upper)}
-        :param scales: Scales for the optimization in the form {param: scale}
+        :param x0: Dictionary of initial values in the form ``{'all': {param: value}}``
+        :param bounds: Bounds for the optimization in the form ``{param: (lower, upper)}``
+        :param scales: Scales for the optimization in the form ``{param: scale}`
         :param loss_type: Type of loss function to use for optimization.
         :param opts_mle: Options for the optimization.
-        :param n_runs: Number of optimization runs. The first run will use the initial values if provided.
-        :param fixed_params: Fixed parameters for the optimization.
+        :param n_runs: Number of independent optimization runs out of which the best one is chosen. The first run
+            will use the initial values if specified. Consider increasing this number if the optimization does not
+            produce good results.
+        :param fixed_params: Parameters held fixed when optimization, i.e., ``{'all': {param: value}}``
         :param do_bootstrap: Whether to do bootstrapping.
         :param n_bootstraps: Number of bootstraps.
         :param parallelize: Whether to parallelize the bootstrapping.
+        :param folded: Whether the SFS are folded. If not specified, the SFS will be folded if both of the given
+            SFS appear to be folded.
         :param discretization: Discretization instance. Mainly intended for internal use.
         :param optimization: Optimization instance. Mainly intended for internal use.
         :param locked: Whether to lock the instance.
-        :param kwargs: Additional arguments.
+        :param kwargs: Additional keyword arguments which are ignored.
         """
         super().__init__()
 
         # assign neutral SFS
         if isinstance(sfs_neut, Spectra):
             #: Neutral SFS
             self.sfs_neut: Spectrum = sfs_neut.all
@@ -140,20 +174,26 @@
             self.sfs_sel: Spectrum = sfs_sel
 
         # check that we have monomorphic counts
         if self.sfs_neut.to_list()[0] == 0 or self.sfs_sel.to_list()[0] == 0:
             raise ValueError('Some of the provided SFS have zero ancestral monomorphic counts. '
                              'Note that we require monomorphic counts in order to infer the mutation rate.')
 
-        #: Sample size
-        self.n: int = sfs_neut.n
-
         #: The DFE parametrization
         self.model: Parametrization = parametrization.from_string(model)
 
+        if folded is None:
+            #: Whether the SFS are folded
+            self.folded: bool = self.sfs_sel.is_folded() and self.sfs_neut.is_folded()
+        else:
+            self.folded = folded
+
+        #: Sample size
+        self.n: int = sfs_neut.n
+
         if discretization is None:
             # create discretization instance
             #: Discretization instance
             self.discretization: Discretization = Discretization(
                 n=self.n,
                 intervals_del=intervals_del,
                 intervals_ben=intervals_ben,
@@ -164,14 +204,18 @@
         else:
             # otherwise assign instance
             self.discretization: Discretization = discretization
 
         #: Estimate of theta from neutral SFS
         self.theta: float = self.sfs_neut.theta
 
+        # raise warning if theta is unusually large
+        if self.theta > 0.05 or self.sfs_sel.theta > 0.05:
+            logger.warning("Mutation rate is unusually highly. This is a reminder to provide monomorphic counts.")
+
         #: MLE estimates of the initial optimization
         self.params_mle: Optional[Dict[str, float]] = None
 
         #: Modelled MLE SFS
         self.sfs_mle: Optional[Spectrum] = None
 
         #: Likelihood of the MLE, this value may be updated after bootstrapping
@@ -224,20 +268,33 @@
                 fixed_params=fixed_params,
                 seed=seed
             )
         else:
             # otherwise assign instance
             self.optimization: Optimization = optimization
 
+        # warn if folded is true, and we estimate the full DFE
+        if self.folded:
+            fixed_dele = set(self.model.submodels['dele'].keys()) if 'dele' in self.model.submodels else set()
+            fixed = set(self.fixed_params['all'].keys()) if 'all' in self.fixed_params else set()
+
+            if not fixed_dele.issubset(fixed):
+                logger.warning("You are estimating the full DFE, but the SFS are folded. "
+                               "This is not recommend as the folded SFS contains little information "
+                               "on beneficial mutations.")
+
         #: Initial values
         self.x0 = dict(all=self.model.x0 | self.default_x0 | (x0['all'] if 'all' in x0 else {}))
 
         #: Bootstrapped MLE parameter estimates
         self.bootstraps: Optional[pd.DataFrame] = None
 
+        #: Bootstrap optimization results
+        self.bootstrap_results: Optional[List[OptimizeResult]] = None
+
         #: L2 norm of fit minus observed SFS
         self.L2_residual: Optional[float] = None
 
         #: Random number generator seed
         self.seed: int | None = seed
 
         #: Random generator instance
@@ -372,15 +429,15 @@
         # assign likelihoods
         self.likelihoods = self.optimization.likelihoods
 
         # unpack shared parameters
         params_mle = unpack_shared(params_mle)
 
         # normalize parameters
-        params_mle['all'] = self.model.normalize(params_mle['all'])
+        params_mle['all'] = self.model._normalize(params_mle['all'])
 
         # assign optimization result and MLE parameters
         self.assign_result(result, params_mle['all'])
 
         # report on optimization result
         self.report_result(result, params_mle)
 
@@ -458,31 +515,35 @@
         """
         # report on optimization result
         if result.success:
             logger.info(f"Successfully finished optimization after {result.nit} iterations "
                         f"and {result.nfev} function evaluations, obtaining a log-likelihood "
                         f"of -{result.fun}.")
         else:
-            logger.warning("Numerical optimization did not terminate normally "
-                           f"so result might be compromised. Number of iterations: {result.nit}."
-                           "Please check the result property for more information.")
+            logger.warning("Numerical optimization did not terminate normally, so "
+                           "the result might be compromised. Consider adjusting "
+                           "the optimization parameters (increasing `gtol` or `n_runs`) "
+                           "or decrease the number of optimized parameters.")
 
         logger.info(f"Inferred parameters: {flatten_dict(params)}.")
 
-    def update_properties(self, **kwargs):
+    def update_properties(self, **kwargs) -> Self:
         """
         Update the properties of this class with the given dictionary
         given that its entries are not None.
 
         :param kwargs: Dictionary of properties to update.
+        :return: Self.
         """
         for key, value in kwargs.items():
             if value is not None:
                 setattr(self, key, value)
 
+        return self
+
     def bootstrap(
             self, n_samples: int = None,
             parallelize: bool = None,
             update_likelihood: bool = True
     ) -> pd.DataFrame:
         """
         Perform the parametric bootstrap.
@@ -532,19 +593,24 @@
         # number of successful runs
         n_success = np.sum([res.success for res in result[:, 0]])
 
         # issue warning if some runs did not finish successfully
         if n_success < self.n_bootstraps:
             logger.warning(f"{self.n_bootstraps - n_success} out of {self.n_bootstraps} bootstrap samples "
                            "did not terminate normally during numerical optimization. "
-                           "The confidence intervals might thus be unreliable.")
+                           "The confidence intervals might thus be unreliable. Consider adjusting "
+                           "the optimization parameters (increasing `gtol` or `n_runs`) "
+                           "or decrease the number of optimized parameters.")
 
-        # dataframe of MLE estimates
+            # dataframe of MLE estimates
         self.bootstraps = pd.DataFrame([r['all'] for r in result[:, 1]])
 
+        # assign bootstrap results
+        self.bootstrap_results = list(result[:, 0])
+
         # add estimates for alpha to the bootstraps
         self.add_alpha_to_bootstraps()
 
         # add execution time
         self.execution_time += time.time() - start_time
 
         # assign average likelihood of successful runs
@@ -611,15 +677,15 @@
             ))
         )
 
         # unpack shared parameters
         params_mle = unpack_shared(params_mle)
 
         # normalize MLE estimates
-        params_mle['all'] = self.model.normalize(params_mle['all'])
+        params_mle['all'] = self.model._normalize(params_mle['all'])
 
         return result, params_mle
 
     def get_scales_linear(self) -> Dict[str, Literal['lin']]:
         """
         Get linear scales for all parameters. We do this for the bootstraps as x0 should be close to MLE.
 
@@ -659,37 +725,44 @@
 
         # multiply by mutational target size
         counts_modelled *= sfs_sel.n_sites
 
         # add contribution of demography and polarization error
         counts_modelled = self.add_demography(sfs_neut, counts_modelled, eps=params['eps'])
 
-        return counts_modelled, sfs_sel.polymorphic
+        # fold if necessary
+        if self.folded:
+            counts_sel = sfs_sel.fold().polymorphic
+            counts_modelled = Spectrum.from_polymorphic(counts_modelled).fold().polymorphic
+        else:
+            counts_sel = sfs_sel.polymorphic
+
+        return counts_modelled, counts_sel
 
     @staticmethod
     def adjust_polarization(counts: np.ndarray, eps: float) -> np.ndarray:
         """
         Adjust the polarization of the given SFS where
-        eps is the rate of wrong ancestral misidentification.
+        eps is the rate of ancestral misidentification.
 
         :param counts: Polymorphic SFS counts to adjust.
-        :param eps: Rate of wrong ancestral misidentification.
+        :param eps: Rate of ancestral misidentification.
         :return: Adjusted SFS counts.
         """
         return (1 - eps) * counts + eps * counts[::-1]
 
     def add_demography(self, sfs_neut: Spectrum, counts_sel: np.ndarray, eps: float) -> np.ndarray:
         """
         Add the effect of demography to counts_sel by considering
         how counts_neut is perturbed relative to the standard coalescent.
         The polarization error is also included here.
 
         :param sfs_neut: Observed spectrum of neutral sites.
         :param counts_sel: Modelled counts of selected sites.
-        :param eps: Rate of wrong ancestral misidentification.
+        :param eps: Rate of ancestral misidentification.
         :return: Adjusted counts of selected sites.
         """
         # normalized counts of the standard coalescent
         counts_kingman = standard_kingman(self.n).polymorphic * sfs_neut.theta * sfs_neut.n_sites
 
         # apply polarization error to neutral and selected counts
         counts_neut_adjusted = self.adjust_polarization(sfs_neut.polymorphic, eps)
@@ -774,15 +847,15 @@
         :param file: File to save plot to.
         :param show: Whether to show plot.
         :param title: Plot title.
         :param ax: Axes object to plot on.
         :return: Axes object
         """
         # evaluate at fixed parameters
-        sizes = self.model.discretize(self.params_mle, self.discretization.bins)
+        sizes = self.model._discretize(self.params_mle, self.discretization.bins)
 
         return Visualization.plot_buckets_sizes(
             n_intervals=self.discretization.n_intervals,
             bins=self.discretization.bins,
             sizes=sizes,
             title=title,
             file=file,
@@ -884,14 +957,16 @@
             ax=ax
         )
 
     @run_if_required_wrapper
     def plot_all(self, show: bool = True):
         """
         Plot everything.
+
+        :param show: Whether to show plot.
         """
         self.plot_inferred_parameters(show=show)
         self.plot_discretized(show=show)
         self.plot_sfs_comparison(show=show)
         self.plot_continuous(show=show)
         self.plot_interval_density(show=show)
         self.plot_likelihoods(show=show)
@@ -1057,15 +1132,15 @@
             # disable bootstraps
             inference.do_bootstrap = do_bootstrap
 
             # dict of params to be fixed
             params = dict(all=submodels_dfe[p[0]] | submodels_outer[p[1]])
 
             # assign fixed parameters
-            inference.set_fixed_params(params)
+            inference._set_fixed_params(params)
 
             # inform about fixed parameters
             logger.info(f'Holding parameters fixed to {params}.')
 
             # run inference
             inference.run()
 
@@ -1144,14 +1219,19 @@
             file=file,
             show=show,
             cmap=cmap,
             title=title,
             ax=ax
         )
 
+    @functools.wraps(AbstractInference.plot_discretized)
+    @run_if_required_wrapper
+    def plot_discretized(self, *args, **kwargs):
+        return super().plot_discretized(*args, **kwargs)
+
     def get_alpha(self, params: dict = None) -> float:
         """
         Get alpha, the proportion of beneficial non-synonymous substitutions.
 
         :param params: Parameters to use for calculation.
         """
         if params is None:
@@ -1270,15 +1350,15 @@
         """
         Parameter names.
 
         :return: List of parameter names.
         """
         return self.model.param_names + ['eps']
 
-    def set_fixed_params(self, params: Dict[str, Dict[str, float]]):
+    def _set_fixed_params(self, params: Dict[str, Dict[str, float]]):
         """
         Set fixed parameters.
 
         :param params: Fixed parameters.
         """
         self.fixed_params = expand_fixed(params, ['all'])
```

### Comparing `fastdfe-0.1.5b0/fastdfe/bootstrap.py` & `fastdfe-0.1.6b0/fastdfe/bootstrap.py`

 * *Files identical despite different names*

### Comparing `fastdfe-0.1.5b0/fastdfe/config.py` & `fastdfe-0.1.6b0/fastdfe/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 from .spectrum import Spectra, parse_polydfe_sfs_config
 
 logger = logging.getLogger('fastdfe')
 
 
 class Config:
     """
-    Configuration class to be used for :class:``~fastdfe.base_inference.BaseInference`` and
-    :class:``fastdfe.joint_inference.JointInference``.
+    Configuration class to be used for :class:`~fastdfe.base_inference.BaseInference` and
+    :class:`fastdfe.joint_inference.JointInference`.
     """
 
     def __init__(
             self,
             polydfe_spectra_config: str = None,
             polydfe_init_file: str = None,
             polydfe_init_file_id: int = 1,
@@ -48,45 +48,48 @@
             opts_mle: dict = {},
             n_runs: int = 10,
             fixed_params: Dict[str, Dict[str, float]] = {},
             shared_params: List[SharedParams] = [],
             covariates: List[Covariate] = [],
             do_bootstrap: bool = False,
             n_bootstraps: int = 100,
-            parallelize: bool = True
+            parallelize: bool = True,
+            **kwargs
     ):
         """
         Create config object.
 
         :param polydfe_spectra_config: Path to polyDFE SFS config file.
         :param polydfe_init_file: Path to polyDFE init file.
         :param polydfe_init_file_id: ID of polyDFE init file.
         :param sfs_neut: Neutral SFS. Note that we require monomorphic counts to be specified in order to infer
             the mutation rate.
         :param sfs_sel: Selected SFS. Note that we require monomorphic counts to be specified in order to infer
             the mutation rate.
         :param intervals_del: Integration intervals for deleterious mutations in log space.
         :param intervals_ben: Integration intervals for beneficial mutations in log space.
-        :param integration_mode: Integration mode.
-        :param linearized: Whether to use the linearized version of the DFE.
+        :param integration_mode: Integration mode, ``quad`` not recommended
+        :param linearized: Whether to use the linearized version of the DFE, ``False`` not recommended.
         :param model: Parametrization of the DFE.
         :param seed: Seed for the random number generator.
         :param x0: Dictionary of initial values in the form ``{type: {param: value}}``
         :param bounds: Bounds for the optimization in the form {param: (lower, upper)}
         :param scales: Scales for the optimization in the form {param: scale}
         :param loss_type: Loss function to use.
         :param opts_mle: Options for the optimization.
-        :param n_runs: Number of optimization runs. Number of optimization runs.
-            The first run will use the initial values if provided.
+        :param n_runs: Number of independent optimization runs out of which the best one is chosen. The first run
+            will use the initial values if specified. Consider increasing this number if the optimization does not
+            produce good results.
         :param fixed_params: Fixed parameters for the optimization.
         :param shared_params: Shared parameters for the optimization.
         :param covariates: Covariates for the optimization.
         :param do_bootstrap: Whether to do bootstrapping automatically.
         :param n_bootstraps: Number of bootstraps.
         :param parallelize: Whether to parallelize the optimization.
+        :param kwargs: Additional keyword arguments which are ignored.
         """
 
         # save options
         self.data = dict(
             model=model,
             intervals_del=intervals_del,
             intervals_ben=intervals_ben,
@@ -113,22 +116,25 @@
         if polydfe_spectra_config is not None:
             self.parse_polydfe_sfs_config(polydfe_spectra_config)
 
         # parse init file if specified
         if polydfe_init_file is not None:
             self.parse_polydfe_init_file(polydfe_init_file, polydfe_init_file_id)
 
-    def update(self, **kwargs):
+    def update(self, **kwargs) -> 'Config':
         """
         Update config with given data.
 
         :param kwargs: Data to update.
+        :return: Updated config.
         """
         self.data |= kwargs
 
+        return self
+
     def parse_polydfe_init_file(self, file: str, id: int = 1, type='all'):
         """
         Parse polyDFE init file.
         This will define the initial parameters and
         which ones will be held fixed during the optimization.
 
         :param type: Type of parameters to parse for.
```

### Comparing `fastdfe-0.1.5b0/fastdfe/discretization.py` & `fastdfe-0.1.6b0/fastdfe/discretization.py`

 * *Files 0% similar despite different names*

```diff
@@ -401,15 +401,15 @@
         :param params: Parameters of the DFE
         :param model: DFE parametrization
         :return: SFS
         """
         if self.linearized:
 
             # get discretized DFE
-            dfe = model.discretize(params, self.bins) / self.interval_sizes
+            dfe = model._discretize(params, self.bins) / self.interval_sizes
 
             # get SFS from DFE using linearization
             # the interval sizes are already included here
             counts_modelled = self.dfe_to_sfs @ dfe
         else:
             dfe_pdf = model.get_pdf(**params)
 
@@ -437,15 +437,15 @@
         """
         Get alpha, the proportion of beneficial non-synonymous substitutions.
 
         :param model: DFE parametrization
         :param params: Parameters of the DFE
         :return: Estimated for alpha
         """
-        y = model.discretize(params, self.bins) * H_fixed_regularized(self.s)
+        y = model._discretize(params, self.bins) * H_fixed_regularized(self.s)
 
         return np.sum(y[self.s > 0]) / np.sum(y)
 
     def get_interval_density(
             self,
             inter: list | np.ndarray = np.array([-np.inf, -100, -10, -1, 0, 1, np.inf])
     ) -> np.ndarray:
```

### Comparing `fastdfe-0.1.5b0/fastdfe/joint_inference.py` & `fastdfe-0.1.6b0/fastdfe/joint_inference.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,44 @@
 # get logger
 logger = logging.getLogger('fastdfe')
 
 
 class JointInference(BaseInference):
     """
     Enabling the sharing of parameters among several Inference objects.
+
+    Basic usage:
+
+    ::
+
+        from fastdfe import JointInference, Spectra, SharedParams
+
+        # neutral SFS for two types
+        sfs_neut = Spectra(dict(
+            pendula=[177130, 997, 441, 228, 156, 117, 114, 83, 105, 109, 652],
+            pubescens=[172528, 3612, 1359, 790, 584, 427, 325, 234, 166, 76, 31]
+        ))
+
+        # selected SFS for two types
+        sfs_sel = Spectra(dict(
+            pendula=[797939, 1329, 499, 265, 162, 104, 117, 90, 94, 119, 794],
+            pubescens=[791106, 5326, 1741, 1005, 756, 546, 416, 294, 177, 104, 41]
+        ))
+
+        # create inference object
+        inf = JointInference(
+            sfs_neut=sfs_neut,
+            sfs_sel=sfs_sel,
+            fixed_params=dict(eps=0), # fix eps to 0
+            do_bootstrap=True
+        )
+
+        # run inference
+        inf.run()
+
     """
 
     def __init__(
             self,
             sfs_neut: Spectra,
             sfs_sel: Spectra,
             include_divergence: bool = None,
@@ -57,50 +87,63 @@
             n_runs: int = 10,
             fixed_params: Dict[str, Dict[str, float]] = {},
             shared_params: List[SharedParams] = [],
             covariates: List[Covariate] = [],
             do_bootstrap: bool = False,
             n_bootstraps: int = 100,
             parallelize: bool = True,
+            folded: bool = None,
+            **kwargs
     ):
         """
         Create instance.
 
         :param sfs_neut: Neutral SFS. Note that we require monomorphic counts to be specified in order to infer
             the mutation rate.
         :param sfs_sel: Selected SFS. Note that we require monomorphic counts to be specified in order to infer
             the mutation rate.
         :param include_divergence: Whether to include divergence in the likelihood
         :param intervals_del: ``(start, stop, n_interval)`` for deleterious population-scaled
             selection coefficients. The intervals will be log10-spaced.
         :param intervals_ben: Same as intervals_del but for beneficial selection coefficients
-        :param integration_mode: Integration mode
-        :param linearized: Whether to use the linearized model
+        :param integration_mode: Integration mode, ``quad`` not recommmended
+        :param linearized: Whether to use the linearized model, ``False`` not recommended
         :param model: DFE parametrization
         :param seed: Random seed
         :param x0: Dictionary of initial values in the form ``{type: {param: value}}``
         :param bounds: Bounds for the optimization in the form {param: (lower, upper)}
         :param scales: Scales for the optimization in the form {param: scale}
         :param loss_type: Loss type
         :param opts_mle: Options for the optimization
-        :param n_runs: Number of independent optimization runs
-        :param fixed_params: dictionary of fixed parameters in the form ``{type: {param: value}}``
+        :param n_runs: Number of independent optimization runs out of which the best one is chosen. The first run
+            will use the initial values if specified. Consider increasing this number if the optimization does not
+            produce good results.
+        :param fixed_params: Dictionary of fixed parameters in the form ``{type: {param: value}}``
         :param shared_params: List of shared parameters
         :param do_bootstrap: Whether to perform bootstrapping
         :param n_bootstraps: Number of bootstraps
         :param parallelize: Whether to parallelize the optimization
-        """
+        :param folded: Whether the SFS are folded. If not specified, the SFS will be folded if all of the given
+            SFS appear to be folded.
+        :param kwargs: Additional keyword arguments which are ignored.
+        """
+        if sfs_neut.has_dots() or sfs_sel.has_dots():
+            raise ValueError('Type names cannot contain dots are not allowed as they are used internally.'
+                             'You can use the `replace_dots` method to replace dots with another character.')
+
         # check whether types are equal
         if set(sfs_neut.types) != set(sfs_sel.types):
-            raise Exception('The neutral and selected spectra must have exactly the same types.')
+            raise ValueError('The neutral and selected spectra must have exactly the same types.')
 
         #: SFS types
         self.types: List[str] = sfs_neut.types
 
         # initialize parent
+        # the `self.folded` property will generalize nicely as we
+        # evaluate ``sfs_sel.all.is_folded and sfs_neut.all.is_folded``
         BaseInference.__init__(**locals())
 
         #: original MLE parameters before adding covariates and unpacked shared
         self.params_mle_raw: Optional[Dict[str, Dict[str, float]]] = None
 
         #: Shared parameters with expanded 'all' type
         self.shared_params = expand_shared(shared_params, self.types, self.optimization.param_names)
@@ -162,14 +205,15 @@
                 scales=scales,
                 loss_type=loss_type,
                 opts_mle=opts_mle,
                 fixed_params=dict(all=fixed_collapsed['all']) if 'all' in fixed_collapsed else {},
                 do_bootstrap=do_bootstrap,
                 n_bootstraps=n_bootstraps,
                 parallelize=parallelize,
+                folded=self.folded,
                 n_runs=n_runs)
         )
 
         # check that the fixed parameters are valid
         self.check_fixed_params_exist()
 
         # check if the fixed parameters are compatible with the shared parameters
@@ -215,14 +259,15 @@
                 scales=scales,
                 loss_type=loss_type,
                 opts_mle=opts_mle,
                 fixed_params=dict(all=self.fixed_params[t]) if t in self.fixed_params else {},
                 do_bootstrap=do_bootstrap,
                 n_bootstraps=n_bootstraps,
                 parallelize=parallelize,
+                folded=self.folded,
                 n_runs=n_runs
             )
 
         #: Joint inference object indexed by type
         self.joint_inferences: Dict[str, BaseInference] = {}
 
         # only add if more than one type and at least one shared parameter is given
@@ -241,14 +286,15 @@
                     scales=scales,
                     loss_type=loss_type,
                     opts_mle=opts_mle,
                     fixed_params=dict(all=self.fixed_params[t]) if t in self.fixed_params else {},
                     do_bootstrap=do_bootstrap,
                     n_bootstraps=n_bootstraps,
                     parallelize=parallelize,
+                    folded=self.folded,
                     n_runs=n_runs,
                     locked=True
                 )
 
     def check_shared_params(self):
         """
         Check if the shared parameters were specified correctly.
@@ -444,15 +490,15 @@
         self.params_mle_raw = copy.deepcopy(params_mle)
 
         # unpack shared parameters
         params_mle = unpack_shared(params_mle)
 
         # normalize parameters for each type
         for t in self.types:
-            params_mle[t] = self.model.normalize(params_mle[t])
+            params_mle[t] = self.model._normalize(params_mle[t])
 
         # report on optimization result
         self.report_result(self.result, params_mle)
 
         # assign optimization result and MLE parameters for each type
         for t, inf in self.joint_inferences.items():
             params_mle[t] = correct_values(
@@ -667,19 +713,24 @@
         # number of successful runs
         n_success = np.sum([res.success for res in result[:, 0]])
 
         # issue warning if some runs did not finish successfully
         if n_success < self.n_bootstraps:
             logger.warning(f"{self.n_bootstraps - n_success} out of {self.n_bootstraps} bootstrap samples "
                            "did not terminate normally during numerical optimization. "
-                           "The confidence intervals might thus be unreliable.")
+                           "The confidence intervals might thus be unreliable. Consider adjusting "
+                           "the optimization parameters (increasing `gtol` or `n_runs`) "
+                           "or decrease the number of optimized parameters.")
 
         # dataframe of MLE estimates in flattened format
         self.bootstraps = pd.DataFrame([flatten_dict(r) for r in result[:, 1]])
 
+        # assign bootstrap results
+        self.bootstrap_results = list(result[:, 0])
+
         # assign bootstrap parameters to joint inferences
         for t, inf in self.joint_inferences.items():
             inf.bootstraps = self.bootstraps.filter(regex=f'{t}.*').rename(columns=lambda x: x.split('.')[-1])
 
             # add estimates for alpha to the bootstraps
             inf.add_alpha_to_bootstraps()
 
@@ -724,15 +775,15 @@
         )
 
         # unpack shared parameters
         params_mle = unpack_shared(params_mle)
 
         for t in self.types:
             # normalize parameters for each type
-            params_mle[t] = self.model.normalize(params_mle[t])
+            params_mle[t] = self.model._normalize(params_mle[t])
 
             # add covariates for each type
             params_mle[t] = correct_values(
                 params=self.add_covariates(params_mle[t], t),
                 bounds=self.bounds,
                 scales=self.scales
             )
@@ -1074,30 +1125,30 @@
         The is no single alpha for the joint inference. Please refer
         to the ``self.joint_inferences[t].alpha``.
 
         :return: None
         """
         return None
 
-    def set_fixed_params(self, params: Dict[str, Dict[str, float]]):
+    def _set_fixed_params(self, params: Dict[str, Dict[str, float]]):
         """
         Set fixed parameters.
 
         :param params: Fixed parameters
         """
         # set for 'all' type
-        self.marginal_inferences['all'].set_fixed_params(params)
+        self.marginal_inferences['all']._set_fixed_params(params)
 
         # expand types
         self.fixed_params = expand_fixed(params, self.types)
 
         # propagate to inference objects
         for t in self.types:
-            self.marginal_inferences[t].set_fixed_params(dict(all=self.fixed_params[t]))
-            self.joint_inferences[t].set_fixed_params(dict(all=self.fixed_params[t]))
+            self.marginal_inferences[t]._set_fixed_params(dict(all=self.fixed_params[t]))
+            self.joint_inferences[t]._set_fixed_params(dict(all=self.fixed_params[t]))
 
         # propagate to optimization
         self.optimization.set_fixed_params(self.fixed_params)
 
         # check if the fixed parameters are compatible with the shared parameters
         self.check_no_shared_params_fixed()
```

### Comparing `fastdfe-0.1.5b0/fastdfe/json_handlers.py` & `fastdfe-0.1.6b0/fastdfe/json_handlers.py`

 * *Files identical despite different names*

### Comparing `fastdfe-0.1.5b0/fastdfe/optimization.py` & `fastdfe-0.1.6b0/fastdfe/optimization.py`

 * *Files 2% similar despite different names*

```diff
@@ -630,14 +630,44 @@
 
 
 @dataclass
 class SharedParams:
     """
     Class specifying the sharing of params among types.
     'all' means all available types or params.
+
+    Basic usage:
+
+    ::
+
+        from fastdfe import JointInference, Spectra, SharedParams
+
+        # neutral SFS for two types
+        sfs_neut = Spectra(dict(
+            pendula=[177130, 997, 441, 228, 156, 117, 114, 83, 105, 109, 652],
+            pubescens=[172528, 3612, 1359, 790, 584, 427, 325, 234, 166, 76, 31]
+        ))
+
+        # selected SFS for two types
+        sfs_sel = Spectra(dict(
+            pendula=[797939, 1329, 499, 265, 162, 104, 117, 90, 94, 119, 794],
+            pubescens=[791106, 5326, 1741, 1005, 756, 546, 416, 294, 177, 104, 41]
+        ))
+
+        # create inference object
+        inf = JointInference(
+            sfs_neut=sfs_neut,
+            sfs_sel=sfs_sel,
+            shared_params=[SharedParams(types=["pendula", "pubescens"], params=["eps", "S_d"])],
+            do_bootstrap=True
+        )
+
+        # run inference
+        inf.run()
+
     """
     #: The params to share
     params: List[str] | Literal['all']
 
     #: The types to share
     types: List[str] | Literal['all']
 
@@ -733,78 +763,95 @@
         :param bounds: Dictionary of bounds
         :param opts_mle: Dictionary of options for the optimizer
         :param loss_type: Type of loss function to use
         :param fixed_params: Dictionary of fixed parameters
         :param scales: Dictionary of scales
         :param param_names: List of parameter names
         """
+        #: Parameter bounds
         self.bounds = bounds
+
+        #: Parameter scales to use
         self.scales = scales
 
+        #: additional options for the optimizer
         self.opts_mle = opts_mle
+
+        #: Type of loss function to use
         self.loss_type = loss_type
 
+        #: Fixed parameters
         self.fixed_params = flatten_dict(fixed_params)
 
         # check if fixed parameters are within the specified bounds
         if correct_values(self.fixed_params, self.bounds, warn=False, scales=scales) != self.fixed_params:
             raise ValueError('Fixed parameters are outside the specified bounds. '
                              f'Fixed params: {self.fixed_params}, bounds: {self.bounds}.')
 
+        #: Parameter names
         self.param_names = param_names
+
+        #: Whether to parallelize the optimization
         self.parallelize = parallelize
 
-        # the initial values
+        #: Initial values
         self.x0: Optional[dict] = None
 
-        # the number of runs
+        #: Number of runs
         self.n_runs: Optional[int] = None
 
-        # store the likelihoods for each run
+        #: Likelihoods for each run
         self.likelihoods: Optional[np.ndarray] = None
 
-        # get a random generator instance
+        #: Random generator instance
         self.rng = np.random.default_rng(seed=seed)
 
     def run(
             self,
             get_counts: Dict[str, Callable],
             x0: Dict[str, Dict[str, float]] = {},
             scales: Dict[str, Literal['lin', 'log', 'symlog']] = {},
             bounds: Dict[str, Tuple[float, float]] = {},
             n_runs: int = 1,
             debug_iterations: bool = True,
             print_info: bool = True,
+            opts_mle: dict = None,
             pbar: bool = None
     ) -> (OptimizeResult, dict):
         """
         Perform the optimization procedure.
 
         :param scales: Scales of the parameters
         :param bounds: Bounds of the parameters
-        :param pbar: Whether to show a progress bar
-        :param print_info: Whether to inform the user about the bounds
-        :param n_runs: Number of optimization runs. Number of optimization runs. The first run will use the
-            initial values if provided.
+        :param n_runs: Number of independent optimization runs out of which the best one is chosen. The first run
+            will use the initial values if specified. Consider increasing this number if the optimization does not
+            produce good results.
         :param x0: Dictionary of initial values in the form ``{type: {param: value}}``
         :param get_counts: Dictionary of functions to evaluate counts for each type
         :param debug_iterations: Whether to print debug messages for each iteration
+        :param opts_mle: Dictionary of options for the optimizer
+        :param print_info: Whether to print information about the bounds
+        :param pbar: Whether to show a progress bar
         :return: The optimization result and the likelihoods
         """
         # number of optimization runs
         self.n_runs = n_runs
 
         # store the scales of the parameters
         if scales:
             self.scales = scales
 
         # store the bounds of the parameters
         if bounds:
             self.bounds = bounds
 
+        # store the options for the optimizer
+        if opts_mle:
+            self.opts_mle = opts_mle
+
         # filter out unneeded values
         # this also holds the fixed parameters
         self.x0 = filter_dict(x0, self.param_names)
 
         # flatten initial values
         flattened = flatten_dict(self.x0)
```

### Comparing `fastdfe-0.1.5b0/fastdfe/parametrization.py` & `fastdfe-0.1.6b0/fastdfe/parametrization.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 import logging
 from abc import abstractmethod
 from functools import wraps
 from typing import Callable, List, Union
 
 import numpy as np
+from matplotlib import pyplot as plt
 from scipy.stats import gamma, expon
 
 # get logger
 logger = logging.getLogger('fastdfe')
 
 
 def from_string(model: Union['Parametrization', str]) -> 'Parametrization':
@@ -24,15 +25,18 @@
 
     :param model: Class name string or parametrization object
     :return: Parametrization object
     """
     if isinstance(model, Parametrization):
         return model
 
-    return globals()[model]()
+    if isinstance(model, str):
+        return globals()[model]()
+
+    raise ValueError(f'Unknown parametrization: {model}')
 
 
 def to_string(model: Union['Parametrization', str]) -> str:
     """
     Return class name string from Parametrization.
 
     :param model: Class name string or Parametrization object
@@ -54,28 +58,31 @@
     #: Default initial parameters
     x0 = {}
 
     #: Default parameter bounds
     bounds = {}
 
     #: The kind of submodels supported by holding some parameters fixed
-    submodels = {}
+    submodels = dict(
+        full=dict(),
+        dele=dict()
+    )
 
     #: Scales over which to optimize the parameters, either 'log' or 'lin'
     scales = {}
 
     def __init__(self):
         """
         Initialize parametrization.
         """
         #: argument names
         self.param_names: List = list(self.x0.keys())
 
     @staticmethod
-    def accepts_scalars(func: Callable) -> Callable[[np.ndarray | float], np.ndarray | float]:
+    def _accepts_scalars(func: Callable) -> Callable[[np.ndarray | float], np.ndarray | float]:
         """
         Make func accept scalar values.
 
         :return: Function that accepts scalars
         """
 
         @wraps(func)
@@ -109,15 +116,15 @@
         """
         Get probability distribution function of DFE.
 
         :return: Function that accepts an array of selection coefficients and returns their cumulative probability
         """
         pass
 
-    def discretize(self, params, bins: np.ndarray) -> np.ndarray:
+    def _discretize(self, params, bins: np.ndarray) -> np.ndarray:
         """
         Discretize by using the CDF.
 
         :param params: Parameters of the parametrization
         :param bins: Bins to use for discretization
         :return: Histogram
         """
@@ -130,27 +137,27 @@
                            f'Used parameters: {params}.')
 
         # compute histogram
         hist = x[1:] - x[:-1]
 
         return hist
 
-    def normalize(self, params: dict) -> dict:
+    def _normalize(self, params: dict) -> dict:
         """
         Normalize parameters.
 
         :param params: Parameters of the parametrization
         :return: Normalized parameters
         """
         # do nothing by default
         return params
 
 
 class GammaExpParametrization(Parametrization):
-    """
+    r"""
     Parametrization for mixture of a gamma and exponential distribution. This corresponds to
     model C in polyDFE.
 
     We have the following probability density function:
 
     .. math::
         \phi(S; S_d, b, p_b, S_b) = (1 - p_b) f_\Gamma(-S; S_d, b) \cdot \mathbf{1}_{\{S < 0\}} +
@@ -212,15 +219,15 @@
         :param S_d: Mean selection coefficient for deleterious mutations
         :param b: Shape parameter for gamma distribution
         :param p_b: Probability of a beneficial mutation
         :param S_b: Mean selection coefficient for beneficial mutations
         :return: Function that accepts an array of selection coefficients and returns their probability density
         """
 
-        @Parametrization.accepts_scalars
+        @Parametrization._accepts_scalars
         def pdf(S: np.ndarray) -> np.ndarray:
             """
             The PDF.
 
             :param S: Selection coefficients
             :return: Probability density
             """
@@ -255,15 +262,15 @@
         :param S_d: Mean selection coefficient for deleterious mutations
         :param b: Shape parameter for gamma distribution
         :param p_b: Probability of a beneficial mutation
         :param S_b: Mean selection coefficient for beneficial mutations
         :return: Function that accepts an array of selection coefficients and returns their cumulative probability
         """
 
-        @Parametrization.accepts_scalars
+        @Parametrization._accepts_scalars
         def cdf(S: np.ndarray) -> np.ndarray:
             """
             The CDF.
 
             :param S: Selection coefficients
             :return: Cumulative probability
             """
@@ -284,15 +291,15 @@
 
             return x
 
         return cdf
 
 
 class DisplacedGammaParametrization(Parametrization):
-    """
+    r"""
     Parametrization for a reflected displaced gamma distribution.
 
     We have the following probability density function:
 
     .. math::
         \phi(S; \hat{S}, b, S_{max}) = f_\Gamma(S_{max} - S; S_{max} - \hat{S}, b) \cdot \mathbf{1}_{\{S \leq S_{max}\}}
 
@@ -302,15 +309,15 @@
     * :math:`b` is the shape of the gamma distribution
     * :math:`S_{max}` is the maximum value that :math:`S` can take
     * :math:`f_\Gamma(x; m, b)` is the density of the gamma distribution with mean :math:`m` and shape :math:`b`
     * :math:`\mathbf{1}_{\{A\}}` denotes the indicator function, which is 1 if :math:`A` is true, and 0 otherwise.
 
     This parametrization uses a single gamma distribution for both positive and negative selection coefficients.
     This is a less flexible parametrization, which may produce results similar to the other models while requiring
-    fewer parameters.
+    fewer parameters. It also does not allow for a purely deleterious sub-parametrization.
 
     """
 
     #: Default initial parameters
     x0 = dict(
         S_mean=-100,
         b=1,
@@ -327,23 +334,29 @@
     #: Scales over which to optimize the parameters
     scales = dict(
         S_mean='log',
         b='lin',
         S_max='log'
     )
 
+    #: The kind of submodels supported by holding some parameters fixed
+    submodels = dict(
+        full=dict(),
+        dele=dict()
+    )
+
     @staticmethod
     def get_pdf(S_mean: float, b: float, S_max: float, **kwargs) -> Callable[[np.ndarray], np.ndarray]:
         """
         Get PDF.
 
         :return: Function that accepts an array of selection coefficients and returns their probability density
         """
 
-        @Parametrization.accepts_scalars
+        @Parametrization._accepts_scalars
         def pdf(S: np.ndarray) -> np.ndarray:
             """
             The PDF.
 
             :param S: Selection coefficients
             :return: Probability density
             """
@@ -361,15 +374,15 @@
     def get_cdf(S_mean: float, b: float, S_max: float, **kwargs) -> Callable[[np.ndarray], np.ndarray]:
         """
         Get CDF.
 
         :return: Function that accepts an array of selection coefficients and returns their cumulative probability
         """
 
-        @Parametrization.accepts_scalars
+        @Parametrization._accepts_scalars
         def cdf(S: np.ndarray) -> np.ndarray:
             """
             The CDF.
 
             :param S: Selection coefficients
             :return: Cumulative probability
             """
@@ -384,15 +397,15 @@
 
             return x
 
         return cdf
 
 
 class GammaDiscreteParametrization(Parametrization):
-    """
+    r"""
     Parametrization for a mixture of a gamma and discrete distribution. This corresponds to polyDFE's model B.
 
     We have the following probability density function:
 
     .. math::
         \phi(S; S_d, b, p_b, S_b) = (1 - p_b) f_{\Gamma}(S; S_d, b) \cdot \mathbf{1}_{\{S < 0\}} +
         p_b \cdot S_b \cdot \mathbf{1}_{\{0 \leq S \leq 1 / S_b\}}
@@ -429,27 +442,36 @@
     scales = dict(
         S_d='log',
         b='log',
         p_b='lin',
         S_b='log'
     )
 
+    #: The kind of submodels supported by holding some parameters fixed
+    submodels = dict(
+        full=dict(),
+        dele=dict(
+            p_b=0,
+            S_b=1
+        )
+    )
+
     @staticmethod
     def get_pdf(S_d: float, b: float, p_b: float, S_b: float, **kwargs) -> Callable[[np.ndarray], np.ndarray]:
         """
         Get PDF.
 
         :param S_d: Mean of the DFE for S >= 0
         :param b: Shape of the gamma distribution
         :param p_b: Probability that S > 0
         :param S_b: Shared selection coefficient of all positively selected mutations up to S_b
         :return: Function that accepts an array of selection coefficients and returns their probability density
         """
 
-        @Parametrization.accepts_scalars
+        @Parametrization._accepts_scalars
         def pdf(S: np.ndarray) -> np.ndarray:
             """
             The PDF.
             
             :param S: Selection coefficients
             :return: Probability density
             """
@@ -475,15 +497,15 @@
         :param S_d: Mean of the DFE for S >= 0
         :param b: Shape of the gamma distribution
         :param p_b: Probability that S > 0
         :param S_b: Shared selection coefficient of all positively selected mutations up to S_b
         :return: Function that accepts an array of selection coefficients and returns their cumulative probability
         """
 
-        @Parametrization.accepts_scalars
+        @Parametrization._accepts_scalars
         def cdf(S: np.ndarray) -> np.ndarray:
             """
             The CDF.
 
             :param S: Selection coefficients
             :return: Cumulative probability
             """
@@ -500,15 +522,15 @@
 
             return x
 
         return cdf
 
 
 class DiscreteParametrization(Parametrization):
-    """
+    r"""
     Parametrization for a discrete distribution. This corresponds to polyDFE's model D.
     By default we use 6 bins, but this can be changed by passing a different array to the constructor.
     The resulting parameter names are :math:`S_1, S_2, \dots, S_k`, where :math:`k` is the number of bins.
 
     That is, the probability density function is given by:
 
     :math:`\phi(S; S_1, S_2, \dots, S_k) = \sum_{i=1}^{k} S_i/c_i \cdot \mathbf{1}_{\{S \in B_i\}}`
@@ -529,48 +551,48 @@
         """
         Constructor.
 
         :param intervals: The intervals of the discrete distribution.
         """
         super().__init__()
 
-        #: intervals
+        #: Intervals
         self.intervals = np.concatenate(([-np.inf], intervals, [np.inf]))
 
-        #: compute the interval sizes
+        #: Interval sizes
         self.interval_sizes = self.intervals[1:] - self.intervals[:-1]
 
-        #: number of intervals
+        #: Number of intervals
         self.k = self.intervals.shape[0] - 1
 
-        #: all parameter names
+        #: All parameter names
         self.params = np.array([f"S{i}" for i in range(self.k)])
 
-        #: parameter names without bounds
+        #: Parameter names without bounds
         self.param_names = self.params[1:-1].tolist()
 
-        #: fixed parameters
+        #: Fixed parameters
         self.fixed_params = {self.params[0]: 0, self.params[-1]: 0}
 
-        #: default initial parameters
+        #: Default initial parameters
         self.x0 = dict((p, 1 / self.k) for p in self.param_names)
 
-        #: default parameter bounds
+        #: Default parameter bounds
         self.bounds = dict((p, (0, 1)) for p in self.param_names)
 
-        #: scales
+        #: Scales
         self.scales = dict((p, 'lin') for p in self.param_names)
 
-        #: submodels
+        #: Submodels
         self.submodels = dict(
             full=dict(),
             dele=dict((p, 0) for p in self.params[1:-1][self.intervals[1:-2] < 0])
         )
 
-    def normalize(self, params: dict) -> dict:
+    def _normalize(self, params: dict) -> dict:
         """
         Add params for boundaries and normalize so that
         the parameters sum up to 1.
 
         :param params: Parameter values
         :return: Dict of normalized values plus remaining parameters
         """
@@ -588,17 +610,17 @@
         Get PDF.
 
         :param kwargs: Parameter values S1, S2, ..., Sk
         :return: Function that computes the PDF for given S values
         """
 
         # normalize and add boundary parameters
-        values = self.normalize(kwargs) | self.fixed_params
+        values = self._normalize(kwargs) | self.fixed_params
 
-        @Parametrization.accepts_scalars
+        @Parametrization._accepts_scalars
         def pdf(S: np.ndarray) -> np.ndarray:
             """
             The PDF.
 
             :param S: Selection coefficients
             :return: Probability density
             """
@@ -617,24 +639,24 @@
         Get CDF.
 
         :param kwargs: Parameter values S1, S2, ..., Sk
         :return: Function that computes the CDF for given S values
         """
 
         # normalize and add boundary parameters
-        values = self.normalize(kwargs) | self.fixed_params
+        values = self._normalize(kwargs) | self.fixed_params
 
         # convert to numpy arrays
         intervals = np.array(self.intervals)
         interval_sizes = np.array(self.interval_sizes)
 
         # convert to ordered array values
         vals = np.array([values[self.params[i]] for i in range(self.k)])
 
-        @Parametrization.accepts_scalars
+        @Parametrization._accepts_scalars
         def cdf(S: np.ndarray) -> np.ndarray:
             """
             The CDF.
 
             :param S: Selection coefficients
             :return: Cumulative probability
             """
```

### Comparing `fastdfe-0.1.5b0/fastdfe/parser.py` & `fastdfe-0.1.6b0/fastdfe/parser.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,35 +2,51 @@
 Parser module.
 """
 
 __author__ = "Janek Sendrowski"
 __contact__ = "sendrowski.janek@gmail.com"
 __date__ = "2023-03-26"
 
-import gzip
 import itertools
 import logging
 from abc import ABC, abstractmethod
-from typing import List, Callable, Literal, Optional, TextIO, Iterable
+from functools import cached_property
+from typing import List, Callable, Literal, Optional, Iterable, Dict
 
 import numpy as np
-from cyvcf2 import VCF, Variant
-from numpy.random import Generator
+from cyvcf2 import Variant, VCF
 from pyfaidx import Fasta
-from tqdm import tqdm
 
+from .annotation import Annotation, Annotator
+from .filtration import Filtration, PolyAllelicFiltration
 from .spectrum import Spectra
+from .vcf import VCFHandler
 
 #: Logger
 logger = logging.getLogger('fastdfe')
 
 #: The DNA bases
 bases = ["A", "C", "G", "T"]
 
 
+def count_no_type(func: Callable) -> Callable:
+    """
+    Decorator that increases ``self.n_no_type`` by 1 if the decorated function raises a ``NoTypeException``.
+    """
+
+    def wrapper(self, variant):
+        try:
+            return func(self, variant)
+        except NoTypeException as e:
+            self.n_no_type += 1
+            raise e
+
+    return wrapper
+
+
 class NoTypeException(BaseException):
     """
     Exception thrown when no type can be determined.
     """
     pass
 
 
@@ -39,24 +55,36 @@
     Abstract class for Stratifying the SFS by determining
     a site's type based on its properties.
     """
 
     #: Parser instance
     parser: Optional['Parser'] = None
 
-    def provide_context(self, parser: 'Parser'):
+    #: The number of sites that didn't have a type.
+    n_no_type: int = 0
+
+    def _setup(self, parser: 'Parser'):
         """
         Provide the stratification with some context by specifying the parser.
-        This should be done before called ``get_type``.
+        This should be done before calling :meth:`get_type`.
 
         :param parser: The parser
         """
         self.parser = parser
 
-    def get_ancestral(self, variant: Variant) -> str:
+    def _teardown(self):
+        """
+        Perform any necessary post-processing. This method is called after the actual stratification.
+        """
+        n_total = self.parser.n_sites - self.parser.n_skipped + self.n_no_type
+        n_valid = n_total - self.n_no_type
+
+        logger.info(f":{type(self).__name__} Number of sites with valid type: {n_valid} / {n_total}")
+
+    def _get_ancestral(self, variant: Variant) -> str:
         """
         Determine the ancestral allele.
 
         :param variant: The vcf site
         :return: Ancestral allele
         :raises ValueError: If the ancestral allele could not be determined
         """
@@ -68,15 +96,15 @@
             if aa in bases:
                 return aa
 
             # if we don't skip non-polarized sites, we raise an error
             if self.parser.ignore_not_polarized:
                 raise ValueError("No valid AA tag found.")
 
-        # if we don't skip non-polarized sites, or if the site is not a SNP
+        # if we don't skip non-polarized sites, or if the site is not an SNP
         # we return the reference allele
         return variant.REF
 
     @abstractmethod
     def get_type(self, variant: Variant) -> Optional[str]:
         """
         Get type of given Variant. Only the types
@@ -102,44 +130,59 @@
     """
     Stratify the SFS by the base context of the mutation. The number of flanking bases
     can be configured. Note that we attempt to take the ancestral allele as the
     middle base. If ``ignore_not_polarized`` is set to ``True``, we skip sites
     that are not polarized, otherwise we use the reference allele as the middle base.
     """
 
-    def __init__(self, fasta_file: str, n_flanking: int = 1):
+    def __init__(self, fasta_file: str, n_flanking: int = 1, aliases: Dict[str, List[str]] = {}):
         """
         Create instance. Note that we require a fasta file to be specified
         for base context to be able to be inferred
 
-        :param fasta_file: The fasta file path
+        :param fasta_file: The fasta file path, possibly gzipped or a URL
         :param n_flanking: The number of flanking bases
+        :param aliases: Dictionary of aliases for the contigs in the VCF file, e.g. ``{'chr1': ['1']}``.
+            This is used to match the contig names in the VCF file with the contig names in the FASTA file and GFF file.
         """
-        self.fasta_file = fasta_file
-        self.n_flanking = n_flanking
+        #: The fasta file
+        self.fasta_file: str = fasta_file
 
-        # load reference genome
-        self.reference = Fasta(self.fasta_file)
+        #: The number of flanking bases
+        self.n_flanking: int = n_flanking
 
+        #: Aliases for the contigs in the VCF file
+        self.aliases: Dict[str, List[str]] = aliases
+
+    @cached_property
+    def _ref(self) -> Fasta:
+        """
+        Get the reference reader.
+
+        :return: The reference reader.
+        """
+        return VCFHandler.load_fasta(self.fasta_file)
+
+    @count_no_type
     def get_type(self, variant: Variant) -> str:
         """
         Get the base context for a given mutation
 
         :param variant: The vcf site
         :return: Base context of the mutation
         """
         pos = variant.POS - 1
 
         try:
-            ref = self.get_ancestral(variant)
+            ref = self._get_ancestral(variant)
         except ValueError:
             raise NoTypeException("Invalid ancestral allele: Ancestral allele must be a valid base.")
 
         # retrieve the sequence of the chromosome from the reference genome
-        sequence = self.reference[variant.CHROM][:].seq
+        sequence = VCFHandler.get_contig(self._ref, VCFHandler.get_aliases(variant.CHROM, self.aliases))
 
         if pos < 0 or pos >= len(sequence):
             raise NoTypeException("Invalid position: Position must be within the bounds of the sequence.")
 
         upstream_start = max(0, pos - self.n_flanking)
         upstream_bases = sequence[upstream_start:pos]
 
@@ -164,39 +207,44 @@
     used for the monomorphic counts, and once to determine the base transitions.
     Note that we assume sites here to be at most bi-allelic.
     """
 
     #: Base-transition probabilities
     probabilities = dict()
 
-    def provide_context(self, parser: 'Parser'):
+    def _setup(self, parser: 'Parser'):
         """
         Determine base transition probabilities for polymorphic sites.
         We do this to calibrate the number of monomorphic sites.
 
         :param parser: The parser
         """
         self.parser = parser
 
         logger.info(f'Determining base transition probabilities.')
 
         # initialize counts
         counts = {base_transition: 0 for base_transition in self.get_types()}
 
-        # count base transitions
-        for i, variant in enumerate(parser.get_sites()):
-            if variant.is_snp:
-                try:
-                    counts[self.get_type(variant)] += 1
-                except NoTypeException:
-                    pass
+        with parser.get_pbar() as pbar:
+
+            # count base transitions
+            for i, variant in enumerate(VCF(parser.vcf)):
+                if variant.is_snp:
+                    try:
+                        counts[self.get_type(variant)] += 1
+                    except NoTypeException:
+                        pass
+
+                pbar.update()
 
         # normalize counts to probabilities
         self.probabilities = {k: v / sum(counts.values()) for k, v in counts.items()}
 
+    @count_no_type
     def get_type(self, variant: Variant) -> str:
         """
         Get the base transition for the given variant.
 
         :param variant: The vcf site
         :return: Base transition
         :raises NoTypeException: if not type could be determined
@@ -239,25 +287,29 @@
 
 
 class AncestralBaseStratification(Stratification):
     """
     Stratify the SFS by the base context of the mutation: the reference base.
     If ``ignore_not_polarized`` is set to ``True``, we skip sites
     that are not polarized, otherwise we use the reference allele as ancestral base.
+    By default, we use the ``AA`` tag to determine the ancestral allele.
+
+    Any subclass of :class:`~fastdfe.parser.AncestralAnnotation` can be used to annotate the ancestral allele.
     """
 
+    @count_no_type
     def get_type(self, variant: Variant) -> str:
         """
         Get the type which is the reference allele.
 
         :param variant: The vcf site
         :return: reference allele
         """
         try:
-            return self.get_ancestral(variant)
+            return self._get_ancestral(variant)
         except ValueError:
             raise NoTypeException("Invalid ancestral allele: Ancestral allele must be a valid base.")
 
     def get_types(self) -> List[str]:
         """
         The possible base types.
 
@@ -276,15 +328,15 @@
 
     #: Transition-transversion probabilities
     probabilities = dict(
         transition=0.5,
         transversion=0.5
     )
 
-    def provide_context(self, parser: 'Parser'):
+    def _setup(self, parser: 'Parser'):
         """
         Determine transition-transversion probabilities for polymorphic sites.
         We do this to calibrate the number of monomorphic sites.
 
         :param parser: The parser
         """
         self.parser = parser
@@ -293,22 +345,27 @@
 
         # initialize counts
         counts = dict(
             transition=0,
             transversion=0
         )
 
-        # count transitions and transversions
-        for i, variant in enumerate(parser.get_sites()):
-            if variant.is_snp:
-                counts[self.get_type(variant)] += 1
+        with parser.get_pbar() as pbar:
+
+            # count transitions and transversions
+            for i, variant in enumerate(VCF(parser.vcf)):
+                if variant.is_snp:
+                    counts[self.get_type(variant)] += 1
+
+                pbar.update()
 
         # normalize counts to probabilities
         self.probabilities = {k: v / sum(counts.values()) for k, v in counts.items()}
 
+    @count_no_type
     def get_type(self, variant: Variant) -> str:
         """
         Get the mutation type (transition or transversion) for a given mutation.
 
         :param variant: The vcf site
         :return: Mutation type
         """
@@ -328,47 +385,54 @@
         :return: List of mutation types
         """
         return ["transition", "transversion"]
 
 
 class DegeneracyStratification(Stratification):
     """
-    Stratify SFS by degeneracy, i.e. whether a site is 4-fold degenerate (neutral) or 0-fold degenerate (selected).
+    Stratify SFS by degeneracy. We only consider sides which 4-fold degenerate (neutral) or
+    0-fold degenerate (selected) which facilitates counting.
+
+    :class:`~fastdfe.annotation.DegeneracyAnnotation` can be used to annotate the degeneracy of a site.
     """
 
-    def __init__(self, custom_callback: Callable[[Variant], str] = None):
+    def __init__(
+            self,
+            custom_callback: Callable[[Variant], str] = None,
+    ):
         """
         Initialize the stratification.
 
         :param custom_callback: Custom callback to determine the type of mutation
         """
         #: Custom callback to determine the degeneracy of mutation
-        self.get_degeneracy = custom_callback if custom_callback is not None else self.get_degeneracy_default
+        self.get_degeneracy = custom_callback if custom_callback is not None else self._get_degeneracy_default
 
     @staticmethod
-    def get_degeneracy_default(variant: Variant) -> Optional[Literal['neutral', 'selected']]:
+    def _get_degeneracy_default(variant: Variant) -> Optional[Literal['neutral', 'selected']]:
         """
         Get degeneracy based on 'Degeneracy' tag.
 
         :param variant: The vcf site
         :return: Type of the mutation
         """
         degeneracy = variant.INFO.get('Degeneracy')
 
         if degeneracy is None:
-            raise NoTypeException("Degeneracy tag not found.")
+            raise NoTypeException("No degeneracy tag found.")
         else:
             if degeneracy == 4:
                 return 'neutral'
 
             if degeneracy == 0:
                 return 'selected'
 
-            raise NoTypeException(f"Degeneracy tag has invalid value: {degeneracy}")
+            raise NoTypeException(f"Degeneracy tag has invalid value: '{degeneracy}' at {variant.CHROM}:{variant.POS}")
 
+    @count_no_type
     def get_type(self, variant: Variant) -> Literal['neutral', 'selected']:
         """
         Get the degeneracy.
 
         :param variant: The vcf site
         :return: Type of the mutation
         :raises NoTypeException: If the mutation is not synonymous or non-synonymous
@@ -380,237 +444,396 @@
         Get all possible degeneracy type (``neutral`` and ``selected``).
 
         :return: List of contexts
         """
         return ['neutral', 'selected']
 
 
-class Parser:
+class SynonymyStratification(Stratification):
+    """
+    Stratify SFS by synonymy (neutral or selected). Note that we extrapolate the number of monomorphic sites
+    for each type from the relative number of types for polymorphic sites.
+
+    :class:`~fastdfe.annotation.SynonymyAnnotation` can be used to annotate the synonymy of a site.
+    """
+
+    def get_types(self) -> List[str]:
+        """
+        Get all possible synonymy types (``neutral`` and ``selected``).
+
+        :return: List of contexts
+        """
+        return ['neutral', 'selected']
+
+    @count_no_type
+    def get_type(self, variant: Variant) -> Literal['neutral', 'selected']:
+        """
+        Get the synonymy using the custom synonymy annotation.
+
+        :param variant: The vcf site
+        :return: Type of the mutation, either ``neutral`` or ``selected``
+        """
+        synonymy = variant.INFO.get('Synonymy')
+
+        if synonymy is None:
+            raise NoTypeException("No synonymy tag found.")
+        else:
+            if synonymy == 1:
+                return 'neutral'
+
+            if synonymy == 0:
+                return 'selected'
+
+            raise NoTypeException(f"Synonymy tag has invalid value: '{synonymy}' at {variant.CHROM}:{variant.POS}")
+
+
+class VEPStratification(SynonymyStratification):
+    """
+    Stratify SFS by synonymy (neutral or selected) based on annotation provided by VEP.
+    """
+
+    def get_types(self) -> List[str]:
+        """
+        Get all possible synonymy types (``neutral`` and ``selected``).
+
+        :return: List of contexts
+        """
+        return ['neutral', 'selected']
+
+    @count_no_type
+    def get_type(self, variant: Variant) -> Literal['neutral', 'selected']:
+        """
+        Get the synonymy of a site.
+
+        :param variant: The vcf site
+        :return: Type of the mutation, either ``neutral`` or ``selected``
+        """
+        synonymy = variant.INFO.get('CSQ')
+
+        if 'synonymous_variant' in synonymy:
+            return 'neutral'
+
+        if 'missense_variant' in synonymy:
+            return 'selected'
+
+        raise NoTypeException(f"Synonymy tag has invalid value: '{synonymy}' at {variant.CHROM}:{variant.POS}")
+
+
+class SnpEffStratification(SynonymyStratification):
+    """
+    Stratify SFS by synonymy (neutral or selected) based on annotation provided by SnpEff.
+    """
+
+    def get_types(self) -> List[str]:
+        """
+        Get all possible synonymy types (``neutral`` and ``selected``).
+
+        :return: List of contexts
+        """
+        return ['neutral', 'selected']
+
+    @count_no_type
+    def get_type(self, variant: Variant) -> Literal['neutral', 'selected']:
+        """
+        Get the synonymy of a site.
+
+        :param variant: The vcf site
+        :return: Type of the mutation, either ``neutral`` or ``selected``
+        """
+        synonymy = variant.INFO.get('CSQ')
+
+        if 'synonymous_variant' in synonymy:
+            return 'neutral'
+
+        if 'missense_variant' in synonymy:
+            return 'selected'
+
+        raise NoTypeException(f"Synonymy tag has invalid value: '{synonymy}' at {variant.CHROM}:{variant.POS}")
+
+
+class Parser(VCFHandler):
     """
     Parse site-frequency spectra from VCF files.
 
     By default, the parser looks at the ``AA`` tag in the VCF file's info field to retrieve
     the correct polarization. Sites for which this tag is not well-defined are by default
     included. Note that non-polarized frequency spectra provide little information on the
     distribution of beneficial mutations.
 
+    We can also annotate the SFS with additional information, such as the degeneracy of the
+    sites and their ancestral alleles. This is done by providing a list of annotations to
+    the parser. The annotations are applied in the order they are provided.
+
+    The parser also allows to filter sites based on their annotations. This is done by
+    providing a list of filtrations to the parser. By default, we filter out poly-allelic
+    sites which is highly recommended as some stratifications assume sites to be at most bi-allelic.
+
     :warning: Not tested for polyploids.
     """
 
     def __init__(
             self,
             vcf: str | Iterable[Variant],
             n: int,
             info_ancestral: str = 'AA',
             ignore_not_polarized: bool = False,
             stratifications: List[Stratification] = [
                 DegeneracyStratification()
             ],
+            annotations: List[Annotation] = [],
+            filtrations: List[Filtration] = [PolyAllelicFiltration()],
             max_sites: int = np.inf,
+            n_target_sites: int = None,
             seed: int | None = 0
     ):
         """
         Initialize the parser.
 
-        :param vcf: The path to the VCF file or an iterable of variants
+        :param vcf: The path to the VCF file or an iterable of variants, can be gzipped, urls are also supported
         :param n: The number of individuals in the sample. We down-sample to this number by drawing without replacement.
             Sites with fewer than ``n`` individuals are skipped.
         :param info_ancestral: The tag in the INFO field that contains the ancestral allele
         :param ignore_not_polarized: Whether to ignore sites that are not polarized, i.e., without a valid info tag
             providing the ancestral allele
         :param stratifications: List of stratifications to use
+        :param annotations: List of annotations to use
+        :param filtrations: List of filtrations to use.
         :param max_sites: Maximum number of sites to parse
+        :param n_target_sites: The number of mutational target sites.
+            Allows to adjust the number of monomorphic site count. Ideally, we obtain the SFS by
+            parsing VCF files that contain both mono- and polymorphic sites. This is because for DFE inference, we
+            require the number of monomorphic sites to calibrate the mutation rate. However, often, only polymorphic
+            sites are available. In this case, we can use ``n_target_sites`` to extrapolate the number of monomorphic
+            sites by looking at the relative number of polymorphic sites for each type. Note that the total number of
+            mono- and polymorphic sites should be specified here. This often corresponds to the number of sites in
+            coding regions over the sequence considered.
         :param seed: Seed for the random number generator
         """
+        super().__init__(
+            vcf=vcf,
+            max_sites=max_sites,
+            seed=seed,
+            info_ancestral=info_ancestral
+        )
 
         #: The number of individuals in the sample
         self.n = n
 
-        #: The path to the VCF file or an iterable of variants
-        self.vcf = vcf
-
-        #: The tag in the INFO field that contains the ancestral allele
-        self.info_ancestral: str = info_ancestral
+        #: The number of mutational target sites
+        self.n_target_sites: int | None = n_target_sites
 
         #: Whether to ignore sites that are not polarized, i.e., without a valid info tag providing the ancestral allele
         self.ignore_not_polarized: bool = ignore_not_polarized
 
         #: List of stratifications to use
         self.stratifications: List[Stratification] = stratifications
 
-        #: Maximum number of sites to parse
-        self.max_sites: int = max_sites
+        #: List of annotations to use
+        self.annotations: List[Annotation] = annotations
 
-        #: Seed for the random number generator
-        self.seed: Optional[int] = seed
+        #: List of filtrations to use
+        self.filtrations: List[Filtration] = filtrations
 
-        #: Random generator instance
-        self.rng = np.random.default_rng(seed=seed)
+        #: The number of sites that were skipped for various reasons
+        self.n_skipped: int = 0
 
-        #: Number of sites to be parsed
-        self.n_sites: Optional[int] = None
+        #: Dictionary of SFS indexed by type
+        self.sfs: Dict[str, np.ndarray] = {}
 
-        #: The number of sites that were skipped when parsing
-        self.n_skipped: int = 0
+        #: The VCF reader
+        self.reader: Optional[VCF] = None
 
-    @staticmethod
-    def open_file(file: str) -> TextIO:
+    def _create_sfs_dictionary(self):
         """
-        Open a file, either gzipped or not.
+        Create an SFS dictionary initialized with all possible base contexts.
 
-        :param file: File to open
-        :return: stream
+        :return: SFS dictionary
         """
-        if file.endswith('.gz'):
-            return gzip.open(file, "rt")
+        types = [s.get_types() for s in self.stratifications]
+        # define the DNA bases
+        contexts = ['.'.join(t) for t in itertools.product(*types)]
+
+        # create dict
+        sfs = {}
+        for context in contexts:
+            sfs[context] = np.zeros(self.n + 1)
 
-        return open(file, 'r')
+        self.sfs = sfs
 
-    def count_lines_vcf(self) -> int:
+    def _parse_site(self, variant: Variant):
         """
-        Count the number of sites in the VCF.
+        Parse a single site.
 
-        :return: Number of sites
+        :param variant: The variant
         """
-        from . import disable_pbar
 
-        logger.info('Counting number of sites.')
+        # number of samples
+        n_samples = variant.ploidy * variant.num_called
 
-        # if we don't have a file path, we can just count the number of variants
-        if not isinstance(self.vcf, str):
-            return len(list(self.vcf))
+        # skip if not enough samples
+        if n_samples < self.n:
+            logger.debug(f'Skipping site due to too few samples at {variant.CHROM}:{variant.POS}.')
+            self.n_skipped += 1
+            return
 
-        i = 0
-        with self.open_file(self.vcf) as f:
+        # determine reference allele count
+        # this doesn't work for polyploids
+        n_ref = variant.ploidy * variant.num_hom_ref + variant.num_het
 
-            with tqdm(disable=disable_pbar) as pbar:
-                for line in f:
-                    if not line.startswith('#'):
-                        i += 1
-                        pbar.update()
+        # swap reference and alternative allele if the AA info field
+        # is defined and indicates so
+        aa = variant.INFO.get(self.info_ancestral)
 
-                    # stop counting if max_sites was reached
-                    if i >= self.max_sites:
-                        break
+        if aa not in bases:
 
-        return i
+            # log a warning
+            logger.debug(f'No valid ancestral allele defined at {variant.CHROM}:{variant.POS}.')
 
-    def create_sfs_dictionary(self) -> dict:
+            if self.ignore_not_polarized:
+                self.n_skipped += 1
+                return
+        else:
+            # adjust orientation if the ancestral allele is not the reference
+            if aa != variant.REF:
+
+                # change alternative allele if defined
+                if len(variant.ALT) != 0:
+                    # we only consider the first alternative allele
+                    variant.ALT[0] = variant.REF
+
+                # change reference allele
+                variant.REF = aa
+
+                # change reference count
+                n_ref = n_samples - n_ref
+
+        # determine down-projected allele count
+        k = self.rng.hypergeometric(ngood=n_samples - n_ref, nbad=n_ref, nsample=self.n)
+
+        # try to obtain type
+        try:
+            t = '.'.join([s.get_type(variant) for s in self.stratifications])
+
+            # add count by 1 if context is defined
+            if t in self.sfs:
+                self.sfs[t][k] += 1
+
+        except NoTypeException as e:
+            self.n_skipped += 1
+            logger.debug(e)
+
+    def _handle_site(self, variant: Variant):
         """
-        Create an SFS dictionary initialized with all possible base contexts.
+        Handle a single site.
 
-        :return: SFS dictionary
+        :param variant: The variant
         """
-        types = [s.get_types() for s in self.stratifications]
-        # define the DNA bases
-        contexts = ['.'.join(t) for t in itertools.product(*types)]
+        # filter the variant
+        for filtration in self.filtrations:
+            if not filtration.filter_site(variant):
+                self.n_skipped += 1
+                return
 
-        # create dict
-        sfs = {}
-        for context in contexts:
-            sfs[context] = np.zeros(self.n + 1)
+        # apply annotations
+        for annotation in self.annotations:
+            annotation.annotate_site(variant)
 
-        return sfs
+        # parse site
+        self._parse_site(variant)
 
-    def get_sites(self) -> Iterable[Variant]:
+    def _teardown(self):
         """
-        Return an iterable object over the VCF file's sites.
-
-        :return: iterable
+        Teardown the parser.
         """
-        from . import disable_pbar
+        for f in self.filtrations:
+            f._teardown()
 
-        vcf = self.vcf
+        for s in self.stratifications:
+            s._teardown()
 
-        if isinstance(vcf, str):
-            vcf = VCF(vcf)
+        for a in self.annotations:
+            a._teardown()
 
-        return tqdm(vcf, total=self.n_sites, disable=disable_pbar)
+    def _infer_monomorphic_counts(self):
+        """
+        Infer the number of monomorphic sites from the number of polymorphic sites.
+        """
+        # total number of polymorphic sites across all types
+        n_polymorphic = np.sum([np.sum(c[1:-1]) for c in self.sfs.values()])
+
+        for t, counts in self.sfs.items():
+            self.sfs[t][0] = np.sum(counts[1:-1]) / n_polymorphic * (self.n_target_sites - n_polymorphic)
+            self.sfs[t][-1] = 0
 
     def parse(self) -> Spectra:
         """
         Parse the VCF file.
 
         :return: The spectra for the different stratifications
         """
-        sfs = self.create_sfs_dictionary()
+        self._create_sfs_dictionary()
 
         # create a string representation of the stratifications
-        representation = '.'.join(['[' + ','.join(s.get_types()) + ']' for s in self.stratifications])
+        representation = '.'.join(['[' + ', '.join(s.get_types()) + ']' for s in self.stratifications])
 
         # log the stratifications
         logger.info(f'Using stratification: {representation}.')
 
         # count the number of sites
-        self.n_sites = self.count_lines_vcf()
+        self.n_sites = self.count_sites()
 
         # make parser available to stratifications
         for s in self.stratifications:
-            s.provide_context(self)
-
-        # reset the number of skipped sites
-        self.n_skipped = 0
+            s._setup(self)
 
-        logger.info(f'Starting to parse.')
-
-        for i, variant in enumerate(self.get_sites()):
-
-            # stop if max_sites was reached
-            if i >= self.max_sites:
-                break
-
-            # number of samples
-            n_samples = variant.ploidy * variant.num_called
-
-            # skip if not enough samples
-            if n_samples < self.n:
-                logger.debug(f'Skipping site due to too few samples {str(variant).strip()}.')
-                self.n_skipped += 1
-                continue
+        # touch all filtrations
+        for f in self.filtrations:
+            f._setup()
+
+        # instantiate annotator to provide context to annotations
+        ann = Annotator(
+            vcf=self.vcf,
+            max_sites=self.max_sites,
+            seed=self.seed,
+            info_ancestral=self.info_ancestral,
+            annotations=[],
+            output=''
+        )
 
-            # determine reference allele count
-            # this doesn't work for polyploids
-            n_ref = variant.ploidy * variant.num_hom_ref + variant.num_het
+        # create reader
+        reader = VCF(self.download_if_url(self.vcf))
 
-            # swap reference and alternative allele if the AA info field
-            # is defined and indicates so
-            aa = variant.INFO.get(self.info_ancestral)
+        # provide annotator to annotations and add info fields
+        for annotation in self.annotations:
+            annotation._setup(ann)
+            annotation._add_info(reader)
 
-            if aa not in bases:
+        logger.info(f'Starting to parse.')
 
-                # log a warning
-                logger.debug(f'No valid ancestral allele defined for {str(variant).strip()}.')
+        # create progress bar
+        with self.get_pbar() as pbar:
 
-                if self.ignore_not_polarized:
-                    self.n_skipped += 1
-                    continue
-            else:
-                # adjust orientation if the ancestral allele is not the reference
-                if aa != variant.REF:
+            for i, variant in enumerate(reader):
 
-                    # change alternative allele if defined
-                    if len(variant.ALT) != 0:
-                        # we only consider the first alternative allele
-                        variant.ALT[0] = variant.REF
+                # handle site
+                self._handle_site(variant)
 
-                    # change reference allele
-                    variant.REF = aa
+                pbar.update()
 
-                    # change reference count
-                    n_ref = n_samples - n_ref
+                # explicitly stopping after ``n``sites fixes a bug with cyvcf2:
+                # 'error parsing variant with `htslib::bcf_read` error-code: 0 and ret: -2'
+                if i + 1 == self.n_sites or i + 1 == self.max_sites:
+                    break
 
-            # determine down-projected allele count
-            k = self.rng.hypergeometric(ngood=n_samples - n_ref, nbad=n_ref, nsample=self.n)
+        # tear down all objects
+        self._teardown()
 
-            # try to obtain type
-            try:
-                t = '.'.join([s.get_type(variant) for s in self.stratifications])
+        # close reader
+        reader.close()
 
-                # add count by 1 if context is defined
-                if t in sfs:
-                    sfs[t][k] += 1
+        # correct monomorphic counts if number of target sites is defined
+        if self.n_target_sites is not None:
+            self._infer_monomorphic_counts()
 
-            except NoTypeException as e:
-                self.n_skipped += 1
-                logger.debug(str(e) + ' ' + str(variant).strip())
+        logger.info(f'Parsed {self.n_sites - self.n_skipped} out of {self.n_sites} sites in total.')
 
-        return Spectra(sfs)
+        return Spectra(self.sfs)
```

### Comparing `fastdfe-0.1.5b0/fastdfe/polydfe.py` & `fastdfe-0.1.6b0/fastdfe/polydfe.py`

 * *Files identical despite different names*

### Comparing `fastdfe-0.1.5b0/fastdfe/polydfe_utils.py` & `fastdfe-0.1.6b0/fastdfe/polydfe_utils.py`

 * *Files identical despite different names*

### Comparing `fastdfe-0.1.5b0/fastdfe/spectrum.py` & `fastdfe-0.1.6b0/fastdfe/spectrum.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 
 def standard_kingman(n: int) -> 'Spectrum':
     """
     Get standard Kingman SFS.
 
     :param n: Standard Kingman SFS
+    :return: Spectrum
     """
     return Spectrum(pad(1 / np.arange(1, n)))
 
 
 def pad(counts: list | np.ndarray) -> np.ndarray:
     """
     Pad array with monomorphic counts.
@@ -50,56 +51,70 @@
         """
         self.data = np.array(data, dtype=float)
 
     @property
     def n(self) -> int:
         """
         The sample size.
+
+        :return: Sample size
         """
         return self.data.shape[0] - 1
 
     @property
     def n_sites(self) -> float:
         """
         The total number of sites.
+
+        :return: Total number of sites
         """
         return sum(self.data)
 
     @property
     def n_div(self) -> float:
         """
         Number of divergence counts.
+
+        :return: Number of divergence counts
         """
         return self.data[-1]
 
     @property
     def has_div(self) -> bool:
         """
         Whether n_div was specified.
+
+        :return: Whether n_div was specified
         """
         return self.n_div != 0
 
     @property
     def n_monomorphic(self) -> float:
         """
         Number of monomorphic sites.
+
+        :return: Number of monomorphic sites
         """
         return self.data[0] + self.data[-1]
 
     @property
     def polymorphic(self) -> np.ndarray:
         """
         Get the polymorphic counts.
+
+        :return: Polymorphic counts
         """
         return self.data[1:-1]
 
     @property
     def n_polymorphic(self) -> np.ndarray:
         """
         Get the polymorphic counts.
+
+        :return: Polymorphic counts
         """
         return np.sum(self.polymorphic)
 
     def to_list(self) -> list:
         """
         Convert to list.
 
@@ -120,27 +135,63 @@
         """
         Calculate site-wise theta using Watterson's estimator.
 
         :return: Site-wise theta
         """
         return self.n_polymorphic / np.sum(1 / np.arange(1, self.n)) / self.n_sites
 
+    def fold(self) -> 'Spectrum':
+        """
+        Fold the site-frequency spectrum.
+
+        :return: Folded spectrum
+        """
+        mid = (self.n + 1) // 2
+        data = self.data.copy()
+
+        data[:mid] += data[-mid:][::-1]
+        data[-mid:] = 0
+
+        return Spectrum(data)
+
+    def is_folded(self) -> bool:
+        """
+        Check if the site-frequency spectrum is folded.
+
+        :return: True if folded, False otherwise
+        """
+        mid = (self.n + 1) // 2
+
+        return np.all(self.data[-mid:] == 0)
+
+    def copy(self) -> 'Spectrum':
+        """
+        Copy the spectrum.
+
+        :return: Copy of the spectrum
+        """
+        return Spectrum(self.data.copy())
+
     @staticmethod
     def from_polymorphic(data: list | np.ndarray) -> 'Spectrum':
         """
         Create Spectrum from polymorphic counts only.
 
         :param data: Polymorphic counts
+        :return: Spectrum
         """
         return Spectrum([0] + list(data) + [0])
 
     @staticmethod
     def from_list(data: list | np.ndarray) -> 'Spectrum':
         """
         Create Spectrum from list.
+
+        :param data: SFS counts
+        :return: Spectrum
         """
         return Spectrum(data)
 
     @staticmethod
     def from_polydfe(
             polymorphic: list | np.ndarray,
             n_sites: float,
@@ -150,53 +201,58 @@
         Create Spectra from polyDFE specification which treats the number
         of mutational target sites and the divergence counts separately.
         Note that the monomorphic counts are included here, although ignored.
 
         :param polymorphic: Polymorphic counts
         :param n_sites: Total number of sites
         :param n_div: Number of divergence counts
+        :return: Spectrum
         """
         # determine number of monomorphic ancestral counts
         n_monomorphic = n_sites - np.sum(list(polymorphic) + [n_div])
 
         data = [n_monomorphic] + list(polymorphic) + [n_div]
 
         return Spectrum.from_list(data)
 
     def __mul__(self, other) -> 'Spectrum':
         """
         Multiply spectrum.
 
         :param other: Scalar
+        :return: Spectrum
         """
         return Spectrum.from_list(self.data * other)
 
     __rmul__ = __mul__
 
     def __add__(self, other) -> 'Spectrum':
         """
         Add spectrum.
 
         :param other: Spectrum
+        :return: Spectrum
         """
         return Spectrum.from_list(self.data * other)
 
     def __floordiv__(self, other) -> 'Spectrum':
         """
         Divide spectrum.
 
         :param other: Scalar
+        :return: Spectrum
         """
         return Spectrum.from_list(self.data // other)
 
     def __truediv__(self, other) -> 'Spectrum':
         """
         Add spectrum.
 
         :param other: Scalar
+        :return: Spectrum
         """
         return Spectrum.from_list(self.data / other)
 
     def plot(
             self,
             show: bool = True,
             file: str = None,
@@ -250,170 +306,212 @@
         """
         self.data = pd.DataFrame(data)
 
     @property
     def n(self) -> int:
         """
         The sample size.
+
+        :return: Sample size
         """
         return self.data.shape[0] - 1
 
     @property
     def k(self) -> int:
         """
         The number of types.
+
+        :return: Number of types
         """
         return self.data.shape[1]
 
     @property
     def n_monomorphic(self) -> float:
         """
         The number of monomorphic sites.
+
+        :return: Number of monomorphic sites
         """
         return self.data[0] + self.data[-1]
 
     @property
     def polymorphic(self) -> np.ndarray:
         """
         The polymorphic counts.
+
+        :return: Polymorphic counts
         """
         return self.data[1:-1]
 
     @property
     def n_polymorphic(self) -> np.ndarray:
         """
         The total number of polymorphic counts.
+
+        :return: Total number of polymorphic counts for each type
         """
         return np.sum(self.polymorphic)
 
     @staticmethod
     def from_list(data: list | np.ndarray, types: List) -> 'Spectra':
         """
         Create from array of spectra.
         Note that data.ndim needs to be 2.
+
+        :param data: Array of spectra
+        :param types: Types
+        :return: Spectra
         """
         return Spectra(dict((t, d) for t, d in zip(types, data)))
 
     @property
     def types(self) -> List[str]:
         """
         The types.
+
+        :return: Types
         """
         return self.data.columns.to_list()
 
     @property
     def n_sites(self) -> pd.Series:
         """
         The number of mutational target sites which is the sum of all SFS entries.
+
+        :return: Number of mutational target sites for each type
         """
         return self.data.sum()
 
     @property
     def n_div(self) -> pd.Series:
         """
         The number of divergence counts.
+
+        :return: Number of divergence counts for each type
         """
         return self.data.iloc[-1]
 
     @property
     def has_div(self) -> pd.Series:
         """
         Whether n_div was specified.
+
+        :return: Whether n_div was specified for each type
         """
         return self.n_div != 0
 
     def normalize(self) -> 'Spectra':
         """
         Normalize spectra by sum of all entries.
+
+        :return: Normalized spectra
         """
         return self / self.data.sum()
 
     def to_file(self, file: str):
         """
         Save object to file.
 
         :param file: File name
         """
         self.data.to_csv(file, index=False)
 
     def to_spectra(self) -> Dict[str, Spectrum]:
         """
         Convert to dictionary of spectrum objects.
+
+        :return: Dictionary of spectrum objects
         """
         return dict((t, self[t]) for t in self.types)
 
     def to_dataframe(self) -> pd.DataFrame:
         """
         Get representation as dataframe.
+
+        :return: Dataframe
         """
         return self.data
 
     def to_numpy(self) -> np.ndarray:
         """
         Convert to numpy array.
+
+        :return: Numpy array
         """
         return self.data.to_numpy().T
 
     def to_list(self) -> list:
         """
         Convert to nested list.
+
+        :return: Nested list
         """
         return list(list(d) for d in self.to_numpy())
 
     def to_dict(self) -> dict:
         """
         Convert to dictionary.
+
+        :return: Dictionary of lists
         """
         # return dictionary of lists
         return dict((k, list(v.values())) for k, v in self.data.to_dict().items())
 
     def __mul__(self, other) -> 'Spectra':
         """
         Multiply Spectra.
 
         :param other: Scalar
+        :return: Spectra
         """
         return Spectra.from_dataframe(self.data * other)
 
     __rmul__ = __mul__
 
     def __floordiv__(self, other) -> 'Spectra':
         """
         Divide Spectra.
 
         :param other: Scalar
+        :return: Spectra
         """
         return Spectra.from_dataframe(self.data // other)
 
     def __truediv__(self, other) -> 'Spectra':
         """
         Divide Spectra.
 
         :param other: Scalar
+        :return: Spectra
         """
         return Spectra.from_dataframe(self.data / other)
 
     def __len__(self) -> int:
         """
         Get number of spectra.
+
+        :return: Number of spectra
         """
         return self.k
 
     def __add__(self, other: 'Spectra') -> 'Spectra':
         """
         Merge types of two spectra objects by adding up their counts entry-wise.
+
+        :param other: Spectra object
+        :return: Spectra object
         """
         return Spectra.from_dataframe(self.data.add(other.data, fill_value=0))
 
     def __getitem__(self, keys) -> Union['Spectrum', 'Spectra']:
         """
         Get item.
 
         :param keys: string or list of strings
-        :return: Key or list of keys
+        :return: Spectrum or Spectra
         """
         # whether the input in an array
         is_array = isinstance(keys, (np.ndarray, list, tuple))
 
         # use regex to select columns
         subset = self.data.filter(regex=('|'.join(keys) if is_array else keys))
 
@@ -433,115 +531,158 @@
         :param s: Spectrum
         """
         self.data[key] = s.to_list()
 
     def __iter__(self):
         """
         Get iterator.
+
+        :return: Iterator
         """
         self.data.__iter__()
 
     def copy(self) -> 'Spectra':
         """
         Copy object.
+
+        :return: Copy of object
         """
         return Spectra.from_dataframe(self.data.copy())
 
     def to_multi_index(self) -> 'Spectra':
         """
         Convert to Spectra object with multi-indexed columns.
+
+        :return: Spectra object with multi-indexed columns
         """
         other = self.copy()
         columns = [tuple(col.split('.')) for col in other.data.columns]
         other.data.columns = pd.MultiIndex.from_tuples(columns)
 
         return other
 
     def to_single_index(self) -> 'Spectra':
         """
         Convert to Spectra object with single-indexed columns (using dot notation).
+
+        :return: Spectra object with single-indexed columns
         """
         other = self.copy()
 
         if other.data.columns.nlevels > 1:
             columns = other.data.columns.map('.'.join)
             other.data.columns = columns
 
         return other
 
     def get_empty(self) -> 'Spectra':
         """
         Get a Spectra object with zero counts but having the same shape and types as self.
+
+        :return: Spectra object with zero counts
         """
         return Spectra.from_dataframe(pd.DataFrame(0, index=self.data.index, columns=self.data.columns))
 
     def merge_groups(self, level: List[int] | int = 0) -> 'Spectra':
         """
         Group over given levels and sum up spectra so the spectra
         are summed over the levels that were not specified.
+
+        :param level: Level(s) to group over
+        :return: Spectra object with merged groups
         """
         return Spectra.from_dataframe(self.to_multi_index().data.groupby(axis=1, level=level).sum()).to_single_index()
 
+    def has_dots(self) -> bool:
+        """
+        Check whether column names contain dots.
+
+        :return: True if column names contain dots, False otherwise
+        """
+        return any('.' in col for col in self.data.columns)
+
+    def replace_dots(self, replacement: str = '_') -> 'Spectra':
+        """
+        Replace dots in column names with a given string.
+
+        :param replacement: Replacement string
+        :return: Spectra object with replaced dots
+        """
+        other = self.copy()
+        other.data.columns = other.data.columns.str.replace('.', replacement)
+
+        return other
+
     @property
     def all(self) -> 'Spectrum':
         """
         The 'all' type equals the sum of all spectra.
+
+        :return: Spectrum object
         """
         return Spectrum.from_list(self.data.sum(axis=1).to_list())
 
     def combine(self, s: 'Spectra') -> 'Spectra':
         """
         Merge types of two Spectra objects.
 
         :param s: Other Spectra object
+        :return: Merged Spectra object
         """
         return Spectra(self.to_dict() | s.to_dict())
 
     @staticmethod
     def from_dict(data: dict) -> 'Spectra':
         """
         Load from dictionary.
 
         :param data: Dictionary of lists indexed by types
+        :return: Spectra object
         """
         lists = [list(v.values() if isinstance(v, dict) else v) for v in data.values()]
 
         return Spectra.from_list(lists, types=list(data.keys()))
 
     @staticmethod
     def from_dataframe(data: pd.DataFrame) -> 'Spectra':
         """
         Load Spectra object from dataframe.
 
         :param data: Dataframe
+        :return: Spectra object
         """
         return Spectra.from_dict(data.to_dict())
 
     @staticmethod
     def from_file(file: str) -> 'Spectra':
         """
         Save object to file.
 
         :param file: File name
+        :return: Spectra object
         """
         return Spectra.from_dataframe(pd.read_csv(file))
 
     @staticmethod
     def from_spectra(spectra: Dict[str, Spectrum]) -> 'Spectra':
         """
         Create from dict of spectrum objects indexed by types.
+
+        :param spectra: Dictionary of spectrum objects indexed by types
+        :return: Spectra object
         """
         return Spectra.from_list([sfs.to_list() for sfs in spectra.values()], types=list(spectra.keys()))
 
     @staticmethod
     def from_spectrum(sfs: Spectrum) -> 'Spectra':
         """
         Create from single spectrum object. The type of the spectrum is set to 'all'.
 
         :param sfs: Spectrum
+        :return: Spectra object
         """
         return Spectra.from_spectra(dict(all=sfs))
 
     def plot(
             self,
             show: bool = True,
             file: str = None,
@@ -574,56 +715,84 @@
             show_monomorphic=show_monomorphic,
             ax=ax
         )
 
     def remove_empty(self) -> 'Spectra':
         """
         Remove types whose spectra have no counts.
+
+        :return: Spectra with non-empty types
         """
         return Spectra.from_dataframe(self.data.loc[:, self.data.any()])
 
     def remove_zero_entries(self) -> 'Spectra':
         """
         Remove types whose spectra have some zero entries.
         Note that we ignore zero counts in the last entry i.e. fixed derived alleles.
+
+        :return: Spectra with non-zero entries
         """
         return Spectra.from_dataframe(self.data.loc[:, self.data[:-1].all()])
 
     def rename(self, names: List[str]) -> 'Spectra':
         """
         Rename types.
 
-        :return: New names
+        :param names: New names
+        :return: Spectra with renamed types
         """
         other = self.copy()
         other.data.columns = names
 
         return other
 
     def prefix(self, prefix: str) -> 'Spectra':
         """
         Prefix types, i.e. 'type' -> 'prefix.type' for all types.
 
-        :return: Prefix
+        :param prefix: Prefix
+        :return: Spectra with prefixed types
         """
         return self.rename([prefix + '.' + col for col in self.types])
 
     def print(self):
         """
         Print spectra.
         """
         print(self.data.T)
 
+    def fold(self):
+        """
+        Fold spectra.
+
+        :return: Folded spectra
+        """
+        spectra = self.to_spectra()
+
+        for t, s in spectra.items():
+            spectra[t] = s.fold()
+
+        return Spectra.from_spectra(spectra)
+
+    def is_folded(self) -> Dict[str, bool]:
+        """
+        Check whether spectra are folded.
+
+        :return: Dictionary of types and whether they are folded
+        """
+        return {t: s.is_folded() for t, s in self.to_spectra().items()}
+
 
 def parse_polydfe_sfs_config(file: str) -> Spectra:
     """
     Parse frequency spectra and mutational target site from
     polyDFE configuration file.
 
-    :return: File name
+    :param file: File name
+    :return: Spectra object
     """
     df = pd.read_csv(file, header=None, comment='#')
 
     # parse number of spectra and sample size
     n_neut, n_sel, n = np.array(df.iloc[0][0].split()).astype(int)
 
     # issue notice about number of spectra and sample size
@@ -638,15 +807,16 @@
 
     def to_spectrum(data: np.array) -> Spectrum:
         """
         Parse spectrum and number of mutational target sites.
         We ignore the number of mutational target sites for divergence counts
         but include the divergence counts for completeness of the SFS.
 
-        :return: Data
+        :param data: Spectrum data
+        :return: Spectrum object
         """
         # iterate over spectra and merge them as we do not
         # support variable mutation rates
         data_merged = data.sum(axis=0)
 
         # polymorphic counts
         polymorphic = list(data_merged[:n - 1])
```

### Comparing `fastdfe-0.1.5b0/fastdfe/visualization.py` & `fastdfe-0.1.6b0/fastdfe/visualization.py`

 * *Files 2% similar despite different names*

```diff
@@ -559,14 +559,17 @@
                     ax=axes[i],
                     n_ticks=15 // min(2, n_cols),
                     log_scale=log_scale,
                     show_monomorphic=show_monomorphic,
                     show=False
                 )
 
+                # set title
+                axes[i].set_title(labels[i] if len(labels) <= i else '')
+
             # make empty plots invisible
             [ax.set_visible(False) for ax in axes[n_plots:]]
 
             # show and save plot
             Visualization.show_and_save(file, show)
 
             return plt.gca()
@@ -656,16 +659,16 @@
         return c[0] * amount, c[1] * amount, c[2] * amount, c[3]
 
     @staticmethod
     @clear_show_save
     def plot_pdf(
             model: Parametrization,
             params: dict,
-            s: np.array,
             ax: plt.Axes,
+            s: np.array = np.linspace(-100, 100, 1000),
             file: str = None,
             show: bool = True
     ) -> plt.Axes:
         """
         Plot PDF of given parametrization.
 
         :param model: DFE parametrization
@@ -687,16 +690,16 @@
         return ax
 
     @staticmethod
     @clear_show_save
     def plot_cdf(
             model: Parametrization,
             params: dict,
-            s: np.array,
             ax: plt.Axes,
+            s: np.array = np.linspace(-100, 100, 1000),
             file: str = None,
             show: bool = True
     ) -> plt.Axes:
         """
         Plot CDF of given parametrization.
 
         :param model: DFE parametrization
@@ -799,49 +802,61 @@
             P: np.ndarray,
             labels_x: list,
             labels_y: list,
             ax: plt.Axes,
             file: str = None,
             show: bool = True,
             cmap: str = None,
-            title: str = None
+            title: str = None,
+            vmin: float = 1e-10,
+            vmax: float = 1,
+
     ) -> plt.Axes:
         """
         Plot p-values of nested likelihoods.
 
         :param P: Matrix of p-values
         :param labels_x: Labels for x-axis
         :param labels_y: Labels for y-axis
         :param file: File to save plot to
         :param show: Whether to show plot
         :param cmap: Colormap to use
         :param title: Title of plot
         :param ax: Axes to plot on
+        :param vmin: Minimum value for colorbar
+        :param vmax: Maximum value for colorbar
         :return: Axes
         """
 
         def format_number(x: float | int | None) -> float | int | str:
             """
             Format number to be displayed.
+
+            :param x: Number to format
+            :return: Formatted number
             """
             if x == 0 or x is None:
                 return 0
 
             if x < 0.0001:
                 return "{:.1e}".format(x)
 
             return np.round(x, 4)
 
         # determine values to display
-        annot = np.vectorize(lambda x: str(format_number(x)))(P)
-        annot[np.equal(P, None)] = '-'
+        annotation = np.vectorize(lambda x: str(format_number(x)))(P)
+        annotation[np.equal(P, None)] = '-'
 
         # change to 1 to get a nicer color
         P[np.equal(P, None)] = 1
 
+        # keep within color bar bounds
+        P[P < vmin] = vmin
+        P[P > vmax] = vmax
+
         # make the cbar have the same height as the heatmap
         cbar_ax = make_axes_locatable(ax).new_horizontal(size="4%", pad=0.15)
         plt.gcf().add_axes(cbar_ax)
 
         # default color map
         if cmap is None:
             cmap = colors.LinearSegmentedColormap.from_list('_', plt.get_cmap('inferno')(np.linspace(0.3, 1, 100)))
@@ -849,18 +864,18 @@
         # plot heatmap
         sns.heatmap(
             P.astype(float),
             ax=ax,
             cbar_ax=cbar_ax,
             cmap=cmap,
             norm=LogNorm(
-                vmin=1e-10,
-                vmax=1
+                vmin=vmin,
+                vmax=vmax
             ),
-            annot=annot,
+            annot=annotation,
             fmt="",
             square=True,
             linewidths=0.5,
             linecolor='#cccccc',
             cbar_kws=dict(
                 label='p-value'
             )
```

### Comparing `fastdfe-0.1.5b0/PKG-INFO` & `fastdfe-0.1.6b0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 Metadata-Version: 2.1
 Name: fastdfe
-Version: 0.1.5b0
+Version: 0.1.6b0
 Summary: Fast, flexible, and hierarchical inference of the distribution of fitness effects
 License: MIT
 Author: Sendrowski
 Author-email: sendrowski.janek@gmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: biopython (>=1.80,<1.82)
 Requires-Dist: cyvcf2 (>=0.30.9,<0.31.0)
 Requires-Dist: jsonpickle (>=3.0.0,<4.0.0)
 Requires-Dist: matplotlib (>=3.7.0,<4.0.0)
 Requires-Dist: mpmath (>=1.3.0,<2.0.0)
 Requires-Dist: multiprocess (>=0.70.12,<0.71.0)
 Requires-Dist: numpy (>=1.24.0,<2.0.0)
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
 Requires-Dist: pyfaidx (>=0.7.1,<0.8.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
-Requires-Dist: scipy (>=1.9.3,<2.0.0)
+Requires-Dist: requests (>=2.28)
+Requires-Dist: requests-cache (>=1.0.0,<2.0.0)
+Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: seaborn (>=0.12.0,<0.13.0)
 Requires-Dist: tqdm (>=4.60.0,<5.0.0)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
 Description-Content-Type: text/markdown
 
-[![fastDFE](https://github.com/Sendrowski/fastDFE/actions/workflows/python-app.yml/badge.svg?branch=master)](https://github.com/Sendrowski/fastDFE/actions/workflows/python-app.yml)
+[![tests](https://github.com/Sendrowski/fastDFE/actions/workflows/run-tests.yml/badge.svg?branch=master)](https://github.com/Sendrowski/fastDFE/actions/workflows/run-tests.yml)
 [![codecov](https://codecov.io/gh/Sendrowski/fastDFE/branch/master/graph/badge.svg?token=0LUE8SZYBJ)](https://codecov.io/gh/Sendrowski/fastDFE)
 [![Documentation Status](https://readthedocs.org/projects/fastdfe/badge/?version=latest)](https://fastdfe.readthedocs.io/en/latest/?badge=latest)
+[![PyPI version](https://badge.fury.io/py/fastdfe.svg)](https://badge.fury.io/py/fastdfe)
 
 fastDFE is a new package designed for inferring the distribution of fitness effects (DFE) from site-frequency spectra (SFS). As it is currently in its beta phase, we are continuously working to improve and refine its features.
 
 Please see the [documentation](https://fastdfe.readthedocs.io/en/latest/) for all the details.
```

