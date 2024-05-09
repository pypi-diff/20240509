# Comparing `tmp/preliz-0.6.1.tar.gz` & `tmp/preliz-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "preliz-0.6.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "preliz-0.6.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `preliz-0.6.1.tar` & `preliz-0.6.2.tar`

### file list

```diff
@@ -1,102 +1,103 @@
--rw-r--r--   0        0        0     4324 2024-05-08 20:00:08.639523 preliz-0.6.1/README.md
--rw-r--r--   0        0        0      649 2024-05-08 20:00:08.695523 preliz-0.6.1/preliz/__init__.py
--rw-r--r--   0        0        0     2772 2024-05-08 20:00:08.695523 preliz-0.6.1/preliz/distributions/__init__.py
--rw-r--r--   0        0        0     6930 2024-05-08 20:00:08.695523 preliz-0.6.1/preliz/distributions/asymmetric_laplace.py
--rw-r--r--   0        0        0     4977 2024-05-08 20:00:08.695523 preliz-0.6.1/preliz/distributions/bernoulli.py
--rw-r--r--   0        0        0     7804 2024-05-08 20:00:08.695523 preliz-0.6.1/preliz/distributions/beta.py
--rw-r--r--   0        0        0     6721 2024-05-08 20:00:08.695523 preliz-0.6.1/preliz/distributions/betabinomial.py
--rw-r--r--   0        0        0     7169 2024-05-08 20:00:08.695523 preliz-0.6.1/preliz/distributions/betascaled.py
--rw-r--r--   0        0        0     5368 2024-05-08 20:00:08.695523 preliz-0.6.1/preliz/distributions/binomial.py
--rw-r--r--   0        0        0     4730 2024-05-08 20:00:08.695523 preliz-0.6.1/preliz/distributions/categorical.py
--rw-r--r--   0        0        0     4302 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/cauchy.py
--rw-r--r--   0        0        0     7488 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/censored.py
--rw-r--r--   0        0        0     4135 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/chi_squared.py
--rw-r--r--   0        0        0    21635 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/continuous_multivariate.py
--rw-r--r--   0        0        0     5071 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/discrete_uniform.py
--rw-r--r--   0        0        0     4942 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/discrete_weibull.py
--rw-r--r--   0        0        0    25870 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/distributions.py
--rw-r--r--   0        0        0     6516 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/distributions_multivariate.py
--rw-r--r--   0        0        0     5946 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/exgaussian.py
--rw-r--r--   0        0        0     4397 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/exponential.py
--rw-r--r--   0        0        0     5941 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/gamma.py
--rw-r--r--   0        0        0     3987 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/geometric.py
--rw-r--r--   0        0        0     4489 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/gumbel.py
--rw-r--r--   0        0        0     3991 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/halfcauchy.py
--rw-r--r--   0        0        0     4920 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/halfnormal.py
--rw-r--r--   0        0        0     8033 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/halfstudentt.py
--rw-r--r--   0        0        0     5386 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/hurdle.py
--rw-r--r--   0        0        0     6141 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/hypergeometric.py
--rw-r--r--   0        0        0     6527 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/inversegamma.py
--rw-r--r--   0        0        0     4899 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/kumaraswamy.py
--rw-r--r--   0        0        0     4061 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/laplace.py
--rw-r--r--   0        0        0     3938 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/logistic.py
--rw-r--r--   0        0        0     5742 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/logitnormal.py
--rw-r--r--   0        0        0     5093 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/lognormal.py
--rw-r--r--   0        0        0     4710 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/moyal.py
--rw-r--r--   0        0        0     6104 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/negativebinomial.py
--rw-r--r--   0        0        0     5017 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/normal.py
--rw-r--r--   0        0        0     5070 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/pareto.py
--rw-r--r--   0        0        0     4265 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/poisson.py
--rw-r--r--   0        0        0     5851 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/rice.py
--rw-r--r--   0        0        0     6212 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/skewnormal.py
--rw-r--r--   0        0        0     7610 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/studentt.py
--rw-r--r--   0        0        0     6875 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/triangular.py
--rw-r--r--   0        0        0     5680 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/truncated.py
--rw-r--r--   0        0        0    14719 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/truncatednormal.py
--rw-r--r--   0        0        0     4692 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/uniform.py
--rw-r--r--   0        0        0     4987 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/vonmises.py
--rw-r--r--   0        0        0     5712 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/wald.py
--rw-r--r--   0        0        0     5152 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/weibull.py
--rw-r--r--   0        0        0     5601 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/zi_binomial.py
--rw-r--r--   0        0        0     7262 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/zi_negativebinomial.py
--rw-r--r--   0        0        0     5707 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/distributions/zi_poisson.py
--rw-r--r--   0        0        0       64 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/internal/__init__.py
--rw-r--r--   0        0        0     4602 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/internal/distribution_helper.py
--rw-r--r--   0        0        0    13819 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/internal/optimization.py
--rw-r--r--   0        0        0     5596 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/internal/parser.py
--rw-r--r--   0        0        0    19087 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/internal/plot_helper.py
--rw-r--r--   0        0        0     9785 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/internal/plot_helper_multivariate.py
--rw-r--r--   0        0        0     2028 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/internal/predictive_helper.py
--rw-r--r--   0        0        0    12000 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/internal/special.py
--rw-r--r--   0        0        0     6565 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/ppls/pymc_io.py
--rw-r--r--   0        0        0      145 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/predictive/__init__.py
--rw-r--r--   0        0        0    14606 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/predictive/ppa.py
--rw-r--r--   0        0        0     2251 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/predictive/ppe.py
--rw-r--r--   0        0        0     2160 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/predictive/predictive_explorer.py
--rw-r--r--   0        0        0     1946 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/tests/check_inside_notebook.ipynb
--rw-r--r--   0        0        0     1787 2024-05-08 20:00:08.699523 preliz-0.6.1/preliz/tests/plot_interactive.ipynb
--rw-r--r--   0        0        0   477854 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/tests/ppa.ipynb
--rw-r--r--   0        0        0     2787 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/tests/predictive_explorer.ipynb
--rw-r--r--   0        0        0     1439 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/tests/quartile_int.ipynb
--rw-r--r--   0        0        0     1472 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/tests/roulette.ipynb
--rw-r--r--   0        0        0      661 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/tests/test_beta_mode.py
--rw-r--r--   0        0        0     1967 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/tests/test_censored.py
--rw-r--r--   0        0        0      757 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/tests/test_dirichlet_mode.py
--rw-r--r--   0        0        0     1144 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/tests/test_discrete_weibull.py
--rw-r--r--   0        0        0     7265 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/tests/test_distributions.py
--rw-r--r--   0        0        0      346 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/tests/test_distributions_helper.py
--rw-r--r--   0        0        0      626 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/tests/test_helper.py
--rw-r--r--   0        0        0     2292 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/tests/test_hurdle.py
--rw-r--r--   0        0        0      338 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/tests/test_internals.py
--rw-r--r--   0        0        0     6654 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/tests/test_maxent.py
--rw-r--r--   0        0        0     2919 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/tests/test_mle.py
--rw-r--r--   0        0        0      987 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/tests/test_optimization.py
--rw-r--r--   0        0        0     6153 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/tests/test_plots.py
--rw-r--r--   0        0        0       85 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/tests/test_ppa.py
--rw-r--r--   0        0        0      117 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/tests/test_predictive_explorer.py
--rw-r--r--   0        0        0     3475 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/tests/test_quartile.py
--rw-r--r--   0        0        0      103 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/tests/test_quartile_int.py
--rw-r--r--   0        0        0      910 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/tests/test_roulette.py
--rw-r--r--   0        0        0    11083 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/tests/test_scipy.py
--rw-r--r--   0        0        0     2287 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/tests/test_special.py
--rw-r--r--   0        0        0     2568 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/tests/test_truncated.py
--rw-r--r--   0        0        0      325 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/unidimensional/__init__.py
--rw-r--r--   0        0        0     2244 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/unidimensional/beta_mode.py
--rw-r--r--   0        0        0     2341 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/unidimensional/dirichlet_mode.py
--rw-r--r--   0        0        0     4125 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/unidimensional/maxent.py
--rw-r--r--   0        0        0     1654 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/unidimensional/mle.py
--rw-r--r--   0        0        0     3259 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/unidimensional/quartile.py
--rw-r--r--   0        0        0     6136 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/unidimensional/quartile_int.py
--rw-r--r--   0        0        0    12994 2024-05-08 20:00:08.703523 preliz-0.6.1/preliz/unidimensional/roulette.py
--rw-r--r--   0        0        0     1410 2024-05-08 20:00:08.703523 preliz-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     5568 1970-01-01 00:00:00.000000 preliz-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-09 16:13:24.830106 preliz-0.6.2/LICENSE
+-rw-r--r--   0        0        0     4324 2024-05-09 16:13:24.830106 preliz-0.6.2/README.md
+-rw-r--r--   0        0        0      649 2024-05-09 16:13:24.886105 preliz-0.6.2/preliz/__init__.py
+-rw-r--r--   0        0        0     2772 2024-05-09 16:13:24.886105 preliz-0.6.2/preliz/distributions/__init__.py
+-rw-r--r--   0        0        0     6930 2024-05-09 16:13:24.886105 preliz-0.6.2/preliz/distributions/asymmetric_laplace.py
+-rw-r--r--   0        0        0     4977 2024-05-09 16:13:24.886105 preliz-0.6.2/preliz/distributions/bernoulli.py
+-rw-r--r--   0        0        0     7804 2024-05-09 16:13:24.886105 preliz-0.6.2/preliz/distributions/beta.py
+-rw-r--r--   0        0        0     6721 2024-05-09 16:13:24.886105 preliz-0.6.2/preliz/distributions/betabinomial.py
+-rw-r--r--   0        0        0     7169 2024-05-09 16:13:24.886105 preliz-0.6.2/preliz/distributions/betascaled.py
+-rw-r--r--   0        0        0     5368 2024-05-09 16:13:24.886105 preliz-0.6.2/preliz/distributions/binomial.py
+-rw-r--r--   0        0        0     4730 2024-05-09 16:13:24.886105 preliz-0.6.2/preliz/distributions/categorical.py
+-rw-r--r--   0        0        0     4302 2024-05-09 16:13:24.886105 preliz-0.6.2/preliz/distributions/cauchy.py
+-rw-r--r--   0        0        0     7488 2024-05-09 16:13:24.886105 preliz-0.6.2/preliz/distributions/censored.py
+-rw-r--r--   0        0        0     4135 2024-05-09 16:13:24.886105 preliz-0.6.2/preliz/distributions/chi_squared.py
+-rw-r--r--   0        0        0    21635 2024-05-09 16:13:24.886105 preliz-0.6.2/preliz/distributions/continuous_multivariate.py
+-rw-r--r--   0        0        0     5071 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/discrete_uniform.py
+-rw-r--r--   0        0        0     4942 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/discrete_weibull.py
+-rw-r--r--   0        0        0    25870 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/distributions.py
+-rw-r--r--   0        0        0     6516 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/distributions_multivariate.py
+-rw-r--r--   0        0        0     5946 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/exgaussian.py
+-rw-r--r--   0        0        0     4397 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/exponential.py
+-rw-r--r--   0        0        0     5941 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/gamma.py
+-rw-r--r--   0        0        0     3987 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/geometric.py
+-rw-r--r--   0        0        0     4489 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/gumbel.py
+-rw-r--r--   0        0        0     3991 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/halfcauchy.py
+-rw-r--r--   0        0        0     4920 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/halfnormal.py
+-rw-r--r--   0        0        0     8033 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/halfstudentt.py
+-rw-r--r--   0        0        0     5386 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/hurdle.py
+-rw-r--r--   0        0        0     6141 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/hypergeometric.py
+-rw-r--r--   0        0        0     6527 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/inversegamma.py
+-rw-r--r--   0        0        0     4899 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/kumaraswamy.py
+-rw-r--r--   0        0        0     4061 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/laplace.py
+-rw-r--r--   0        0        0     3938 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/logistic.py
+-rw-r--r--   0        0        0     5742 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/logitnormal.py
+-rw-r--r--   0        0        0     5093 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/lognormal.py
+-rw-r--r--   0        0        0     4710 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/moyal.py
+-rw-r--r--   0        0        0     6104 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/negativebinomial.py
+-rw-r--r--   0        0        0     5017 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/normal.py
+-rw-r--r--   0        0        0     5070 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/pareto.py
+-rw-r--r--   0        0        0     4265 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/poisson.py
+-rw-r--r--   0        0        0     5851 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/rice.py
+-rw-r--r--   0        0        0     6212 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/skewnormal.py
+-rw-r--r--   0        0        0     7610 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/studentt.py
+-rw-r--r--   0        0        0     6875 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/triangular.py
+-rw-r--r--   0        0        0     5680 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/truncated.py
+-rw-r--r--   0        0        0    14719 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/truncatednormal.py
+-rw-r--r--   0        0        0     4692 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/uniform.py
+-rw-r--r--   0        0        0     4987 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/vonmises.py
+-rw-r--r--   0        0        0     5712 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/wald.py
+-rw-r--r--   0        0        0     5152 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/weibull.py
+-rw-r--r--   0        0        0     5601 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/zi_binomial.py
+-rw-r--r--   0        0        0     7262 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/zi_negativebinomial.py
+-rw-r--r--   0        0        0     5707 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/distributions/zi_poisson.py
+-rw-r--r--   0        0        0       64 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/internal/__init__.py
+-rw-r--r--   0        0        0     4602 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/internal/distribution_helper.py
+-rw-r--r--   0        0        0    13819 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/internal/optimization.py
+-rw-r--r--   0        0        0     5596 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/internal/parser.py
+-rw-r--r--   0        0        0    19087 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/internal/plot_helper.py
+-rw-r--r--   0        0        0     9785 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/internal/plot_helper_multivariate.py
+-rw-r--r--   0        0        0     2028 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/internal/predictive_helper.py
+-rw-r--r--   0        0        0    12000 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/internal/special.py
+-rw-r--r--   0        0        0     6565 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/ppls/pymc_io.py
+-rw-r--r--   0        0        0      145 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/predictive/__init__.py
+-rw-r--r--   0        0        0    14606 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/predictive/ppa.py
+-rw-r--r--   0        0        0     2251 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/predictive/ppe.py
+-rw-r--r--   0        0        0     2160 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/predictive/predictive_explorer.py
+-rw-r--r--   0        0        0     1946 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/tests/check_inside_notebook.ipynb
+-rw-r--r--   0        0        0     1787 2024-05-09 16:13:24.890106 preliz-0.6.2/preliz/tests/plot_interactive.ipynb
+-rw-r--r--   0        0        0   477854 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/tests/ppa.ipynb
+-rw-r--r--   0        0        0     2787 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/tests/predictive_explorer.ipynb
+-rw-r--r--   0        0        0     1439 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/tests/quartile_int.ipynb
+-rw-r--r--   0        0        0     1472 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/tests/roulette.ipynb
+-rw-r--r--   0        0        0      661 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/tests/test_beta_mode.py
+-rw-r--r--   0        0        0     1967 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/tests/test_censored.py
+-rw-r--r--   0        0        0      757 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/tests/test_dirichlet_mode.py
+-rw-r--r--   0        0        0     1144 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/tests/test_discrete_weibull.py
+-rw-r--r--   0        0        0     7265 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/tests/test_distributions.py
+-rw-r--r--   0        0        0      346 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/tests/test_distributions_helper.py
+-rw-r--r--   0        0        0      626 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/tests/test_helper.py
+-rw-r--r--   0        0        0     2292 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/tests/test_hurdle.py
+-rw-r--r--   0        0        0      338 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/tests/test_internals.py
+-rw-r--r--   0        0        0     6654 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/tests/test_maxent.py
+-rw-r--r--   0        0        0     2919 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/tests/test_mle.py
+-rw-r--r--   0        0        0      987 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/tests/test_optimization.py
+-rw-r--r--   0        0        0     6153 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/tests/test_plots.py
+-rw-r--r--   0        0        0       85 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/tests/test_ppa.py
+-rw-r--r--   0        0        0      117 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/tests/test_predictive_explorer.py
+-rw-r--r--   0        0        0     3475 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/tests/test_quartile.py
+-rw-r--r--   0        0        0      103 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/tests/test_quartile_int.py
+-rw-r--r--   0        0        0      910 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/tests/test_roulette.py
+-rw-r--r--   0        0        0    11083 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/tests/test_scipy.py
+-rw-r--r--   0        0        0     2287 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/tests/test_special.py
+-rw-r--r--   0        0        0     2568 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/tests/test_truncated.py
+-rw-r--r--   0        0        0      325 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/unidimensional/__init__.py
+-rw-r--r--   0        0        0     2244 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/unidimensional/beta_mode.py
+-rw-r--r--   0        0        0     2341 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/unidimensional/dirichlet_mode.py
+-rw-r--r--   0        0        0     4125 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/unidimensional/maxent.py
+-rw-r--r--   0        0        0     1654 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/unidimensional/mle.py
+-rw-r--r--   0        0        0     3259 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/unidimensional/quartile.py
+-rw-r--r--   0        0        0     6136 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/unidimensional/quartile_int.py
+-rw-r--r--   0        0        0    12994 2024-05-09 16:13:24.894106 preliz-0.6.2/preliz/unidimensional/roulette.py
+-rw-r--r--   0        0        0     1559 2024-05-09 16:13:24.894106 preliz-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     5705 1970-01-01 00:00:00.000000 preliz-0.6.2/PKG-INFO
```

### Comparing `preliz-0.6.1/README.md` & `preliz-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/__init__.py` & `preliz-0.6.2/preliz/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from .distributions import *
 from .predictive import *
 from .unidimensional import *
 
 
 __all__ = ["maxent", "mle", "ppa", "roulette", "quartile"]
 
-__version__ = "0.6.1"
+__version__ = "0.6.2"
 
 _log = logging.getLogger("preliz")
 
 if not logging.root.handlers:
     _log.setLevel(logging.INFO)
     if len(_log.handlers) == 0:
         handler = logging.StreamHandler()
```

### Comparing `preliz-0.6.1/preliz/distributions/__init__.py` & `preliz-0.6.2/preliz/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/distributions/asymmetric_laplace.py` & `preliz-0.6.2/preliz/distributions/asymmetric_laplace.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/distributions/bernoulli.py` & `preliz-0.6.2/preliz/distributions/bernoulli.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/distributions/beta.py` & `preliz-0.6.2/preliz/distributions/beta.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/distributions/betabinomial.py` & `preliz-0.6.2/preliz/distributions/betabinomial.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/distributions/betascaled.py` & `preliz-0.6.2/preliz/distributions/betascaled.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/distributions/binomial.py` & `preliz-0.6.2/preliz/distributions/binomial.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/distributions/categorical.py` & `preliz-0.6.2/preliz/distributions/categorical.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/distributions/cauchy.py` & `preliz-0.6.2/preliz/distributions/cauchy.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/distributions/censored.py` & `preliz-0.6.2/preliz/distributions/censored.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/distributions/chi_squared.py` & `preliz-0.6.2/preliz/distributions/chi_squared.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/distributions/continuous_multivariate.py` & `preliz-0.6.2/preliz/distributions/continuous_multivariate.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/distributions/discrete_uniform.py` & `preliz-0.6.2/preliz/distributions/discrete_uniform.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/distributions/discrete_weibull.py` & `preliz-0.6.2/preliz/distributions/discrete_weibull.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/distributions/distributions.py` & `preliz-0.6.2/preliz/distributions/distributions.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/distributions/distributions_multivariate.py` & `preliz-0.6.2/preliz/distributions/distributions_multivariate.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/distributions/exgaussian.py` & `preliz-0.6.2/preliz/distributions/exgaussian.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/distributions/exponential.py` & `preliz-0.6.2/preliz/distributions/exponential.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/distributions/gamma.py` & `preliz-0.6.2/preliz/distributions/gamma.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/distributions/geometric.py` & `preliz-0.6.2/preliz/distributions/geometric.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/distributions/gumbel.py` & `preliz-0.6.2/preliz/distributions/gumbel.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/distributions/halfcauchy.py` & `preliz-0.6.2/preliz/distributions/halfcauchy.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/distributions/halfnormal.py` & `preliz-0.6.2/preliz/distributions/halfnormal.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/distributions/halfstudentt.py` & `preliz-0.6.2/preliz/distributions/halfstudentt.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/distributions/hurdle.py` & `preliz-0.6.2/preliz/distributions/hurdle.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/distributions/hypergeometric.py` & `preliz-0.6.2/preliz/distributions/hypergeometric.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/distributions/inversegamma.py` & `preliz-0.6.2/preliz/distributions/inversegamma.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/distributions/kumaraswamy.py` & `preliz-0.6.2/preliz/distributions/kumaraswamy.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/distributions/laplace.py` & `preliz-0.6.2/preliz/distributions/laplace.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/distributions/logistic.py` & `preliz-0.6.2/preliz/distributions/logistic.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/distributions/logitnormal.py` & `preliz-0.6.2/preliz/distributions/logitnormal.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/distributions/lognormal.py` & `preliz-0.6.2/preliz/distributions/lognormal.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/distributions/moyal.py` & `preliz-0.6.2/preliz/distributions/moyal.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/distributions/negativebinomial.py` & `preliz-0.6.2/preliz/distributions/negativebinomial.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/distributions/normal.py` & `preliz-0.6.2/preliz/distributions/normal.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/distributions/pareto.py` & `preliz-0.6.2/preliz/distributions/pareto.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/distributions/poisson.py` & `preliz-0.6.2/preliz/distributions/poisson.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/distributions/rice.py` & `preliz-0.6.2/preliz/distributions/rice.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/distributions/skewnormal.py` & `preliz-0.6.2/preliz/distributions/skewnormal.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/distributions/studentt.py` & `preliz-0.6.2/preliz/distributions/studentt.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/distributions/triangular.py` & `preliz-0.6.2/preliz/distributions/triangular.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/distributions/truncated.py` & `preliz-0.6.2/preliz/distributions/truncated.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/distributions/truncatednormal.py` & `preliz-0.6.2/preliz/distributions/truncatednormal.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/distributions/uniform.py` & `preliz-0.6.2/preliz/distributions/uniform.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/distributions/vonmises.py` & `preliz-0.6.2/preliz/distributions/vonmises.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/distributions/wald.py` & `preliz-0.6.2/preliz/distributions/wald.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/distributions/weibull.py` & `preliz-0.6.2/preliz/distributions/weibull.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/distributions/zi_binomial.py` & `preliz-0.6.2/preliz/distributions/zi_binomial.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/distributions/zi_negativebinomial.py` & `preliz-0.6.2/preliz/distributions/zi_negativebinomial.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/distributions/zi_poisson.py` & `preliz-0.6.2/preliz/distributions/zi_poisson.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/internal/distribution_helper.py` & `preliz-0.6.2/preliz/internal/distribution_helper.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/internal/optimization.py` & `preliz-0.6.2/preliz/internal/optimization.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/internal/parser.py` & `preliz-0.6.2/preliz/internal/parser.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/internal/plot_helper.py` & `preliz-0.6.2/preliz/internal/plot_helper.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/internal/plot_helper_multivariate.py` & `preliz-0.6.2/preliz/internal/plot_helper_multivariate.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/internal/predictive_helper.py` & `preliz-0.6.2/preliz/internal/predictive_helper.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/internal/special.py` & `preliz-0.6.2/preliz/internal/special.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/ppls/pymc_io.py` & `preliz-0.6.2/preliz/ppls/pymc_io.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/predictive/ppa.py` & `preliz-0.6.2/preliz/predictive/ppa.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/predictive/ppe.py` & `preliz-0.6.2/preliz/predictive/ppe.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/predictive/predictive_explorer.py` & `preliz-0.6.2/preliz/predictive/predictive_explorer.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/tests/check_inside_notebook.ipynb` & `preliz-0.6.2/preliz/tests/check_inside_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/tests/plot_interactive.ipynb` & `preliz-0.6.2/preliz/tests/plot_interactive.ipynb`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/tests/ppa.ipynb` & `preliz-0.6.2/preliz/tests/ppa.ipynb`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/tests/predictive_explorer.ipynb` & `preliz-0.6.2/preliz/tests/predictive_explorer.ipynb`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/tests/quartile_int.ipynb` & `preliz-0.6.2/preliz/tests/quartile_int.ipynb`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/tests/roulette.ipynb` & `preliz-0.6.2/preliz/tests/roulette.ipynb`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/tests/test_beta_mode.py` & `preliz-0.6.2/preliz/tests/test_beta_mode.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/tests/test_censored.py` & `preliz-0.6.2/preliz/tests/test_censored.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/tests/test_dirichlet_mode.py` & `preliz-0.6.2/preliz/tests/test_dirichlet_mode.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/tests/test_discrete_weibull.py` & `preliz-0.6.2/preliz/tests/test_discrete_weibull.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/tests/test_distributions.py` & `preliz-0.6.2/preliz/tests/test_distributions.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/tests/test_helper.py` & `preliz-0.6.2/preliz/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/tests/test_hurdle.py` & `preliz-0.6.2/preliz/tests/test_hurdle.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/tests/test_maxent.py` & `preliz-0.6.2/preliz/tests/test_maxent.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/tests/test_mle.py` & `preliz-0.6.2/preliz/tests/test_mle.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/tests/test_optimization.py` & `preliz-0.6.2/preliz/tests/test_optimization.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/tests/test_plots.py` & `preliz-0.6.2/preliz/tests/test_plots.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/tests/test_quartile.py` & `preliz-0.6.2/preliz/tests/test_quartile.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/tests/test_roulette.py` & `preliz-0.6.2/preliz/tests/test_roulette.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/tests/test_scipy.py` & `preliz-0.6.2/preliz/tests/test_scipy.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/tests/test_special.py` & `preliz-0.6.2/preliz/tests/test_special.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/tests/test_truncated.py` & `preliz-0.6.2/preliz/tests/test_truncated.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/unidimensional/beta_mode.py` & `preliz-0.6.2/preliz/unidimensional/beta_mode.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/unidimensional/dirichlet_mode.py` & `preliz-0.6.2/preliz/unidimensional/dirichlet_mode.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/unidimensional/maxent.py` & `preliz-0.6.2/preliz/unidimensional/maxent.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/unidimensional/mle.py` & `preliz-0.6.2/preliz/unidimensional/mle.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/unidimensional/quartile.py` & `preliz-0.6.2/preliz/unidimensional/quartile.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/unidimensional/quartile_int.py` & `preliz-0.6.2/preliz/unidimensional/quartile_int.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/preliz/unidimensional/roulette.py` & `preliz-0.6.2/preliz/unidimensional/roulette.py`

 * *Files identical despite different names*

### Comparing `preliz-0.6.1/pyproject.toml` & `preliz-0.6.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 [build-system]
 requires = ["flit_core >=3.4,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "preliz"
 readme = "README.md"
+requires-python = ">=3.10"
+license = {file = "LICENSE"}
 authors = [
     {name = "ArviZ team", email = "arviz.devs@gmail.com"}
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Science/Research",
     "Intended Audience :: Education",
@@ -32,14 +34,16 @@
 
 [tool.flit.module]
 name = "preliz"
 
 [project.urls]
 source = "https://github.com/arviz-devs/preliz"
 tracker = "https://github.com/arviz-devs/preliz/issues"
+documentation = "https://preliz.readthedocs.io"
+funding = "https://opencollective.com/arviz"
 
 [project.optional-dependencies]
 full = [
   "nbclient<0.6,>=0.2",
   "ipywidgets",
   "ipympl",
 ]
```

### Comparing `preliz-0.6.1/PKG-INFO` & `preliz-0.6.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: preliz
-Version: 0.6.1
+Version: 0.6.2
 Summary: The place for all your prior elicitation needs.
 Author-email: ArviZ team <arviz.devs@gmail.com>
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -20,14 +21,16 @@
 Requires-Dist: numpy>=1.22
 Requires-Dist: scipy>=1.9.1, <1.13
 Requires-Dist: nbclient<0.6,>=0.2 ; extra == "full"
 Requires-Dist: ipywidgets ; extra == "full"
 Requires-Dist: ipympl ; extra == "full"
 Requires-Dist: jupyterlab ; extra == "lab"
 Requires-Dist: notebook ; extra == "notebook"
+Project-URL: documentation, https://preliz.readthedocs.io
+Project-URL: funding, https://opencollective.com/arviz
 Project-URL: source, https://github.com/arviz-devs/preliz
 Project-URL: tracker, https://github.com/arviz-devs/preliz/issues
 Provides-Extra: full
 Provides-Extra: lab
 Provides-Extra: notebook
 
 <img src="https://raw.githubusercontent.com/arviz-devs/preliz/main/docs/logos/PreliZ.png#gh-light-mode-only" width=200></img>
```

