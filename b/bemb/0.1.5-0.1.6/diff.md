# Comparing `tmp/bemb-0.1.5.tar.gz` & `tmp/bemb-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bemb-0.1.5.tar", last modified: Thu Sep 29 07:28:30 2022, max compression
+gzip compressed data, was "bemb-0.1.6.tar", last modified: Sat May 20 21:17:14 2023, max compression
```

## Comparing `bemb-0.1.5.tar` & `bemb-0.1.6.tar`

### file list

```diff
@@ -1,24 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 07:28:30.995228 bemb-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (121)     1117 2022-09-29 07:28:21.000000 bemb-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4221 2022-09-29 07:28:30.995228 bemb-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3790 2022-09-29 07:28:21.000000 bemb-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 07:28:30.995228 bemb-0.1.5/bemb/
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-09-29 07:28:21.000000 bemb-0.1.5/bemb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 07:28:30.995228 bemb-0.1.5/bemb/model/
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-09-29 07:28:21.000000 bemb-0.1.5/bemb/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    45328 2022-09-29 07:28:21.000000 bemb-0.1.5/bemb/model/_bemb_dev.py
--rw-r--r--   0 runner    (1001) docker     (121)    53950 2022-09-29 07:28:21.000000 bemb-0.1.5/bemb/model/_bemb_flex.py
--rw-r--r--   0 runner    (1001) docker     (121)    14578 2022-09-29 07:28:21.000000 bemb-0.1.5/bemb/model/bayesian_coefficient.py
--rw-r--r--   0 runner    (1001) docker     (121)     8042 2022-09-29 07:28:21.000000 bemb-0.1.5/bemb/model/bayesian_linear.py
--rw-r--r--   0 runner    (1001) docker     (121)    70581 2022-09-29 07:28:21.000000 bemb-0.1.5/bemb/model/bemb.py
--rw-r--r--   0 runner    (1001) docker     (121)     8004 2022-09-29 07:28:21.000000 bemb-0.1.5/bemb/model/bemb_flex_lightning.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 07:28:30.995228 bemb-0.1.5/bemb/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 07:28:21.000000 bemb-0.1.5/bemb/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2892 2022-09-29 07:28:21.000000 bemb-0.1.5/bemb/utils/run_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 07:28:30.995228 bemb-0.1.5/bemb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4221 2022-09-29 07:28:30.000000 bemb-0.1.5/bemb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      393 2022-09-29 07:28:30.000000 bemb-0.1.5/bemb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-29 07:28:30.000000 bemb-0.1.5/bemb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-09-29 07:28:30.000000 bemb-0.1.5/bemb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-29 07:28:30.995228 bemb-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      969 2022-09-29 07:28:21.000000 bemb-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 21:17:14.924973 bemb-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-05-20 21:17:04.000000 bemb-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-05-20 21:17:14.924973 bemb-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-05-20 21:17:04.000000 bemb-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 21:17:14.920973 bemb-0.1.6/bemb/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-20 21:17:04.000000 bemb-0.1.6/bemb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 21:17:14.920973 bemb-0.1.6/bemb/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-20 21:17:04.000000 bemb-0.1.6/bemb/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-20 21:17:04.000000 bemb-0.1.6/bemb/data/simulate_choice_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 21:17:14.924973 bemb-0.1.6/bemb/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-20 21:17:04.000000 bemb-0.1.6/bemb/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45328 2023-05-20 21:17:04.000000 bemb-0.1.6/bemb/model/_bemb_dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53950 2023-05-20 21:17:04.000000 bemb-0.1.6/bemb/model/_bemb_flex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14578 2023-05-20 21:17:04.000000 bemb-0.1.6/bemb/model/bayesian_coefficient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8042 2023-05-20 21:17:04.000000 bemb-0.1.6/bemb/model/bayesian_linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72322 2023-05-20 21:17:04.000000 bemb-0.1.6/bemb/model/bemb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8550 2023-05-20 21:17:04.000000 bemb-0.1.6/bemb/model/bemb_flex_lightning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 21:17:14.924973 bemb-0.1.6/bemb/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 21:17:04.000000 bemb-0.1.6/bemb/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-05-20 21:17:04.000000 bemb-0.1.6/bemb/utils/run_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-05-20 21:17:04.000000 bemb-0.1.6/bemb/utils/run_helper_lightning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 21:17:14.920973 bemb-0.1.6/bemb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-05-20 21:17:14.000000 bemb-0.1.6/bemb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-20 21:17:14.000000 bemb-0.1.6/bemb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 21:17:14.000000 bemb-0.1.6/bemb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-20 21:17:14.000000 bemb-0.1.6/bemb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 21:17:14.924973 bemb-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-20 21:17:04.000000 bemb-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 21:17:14.924973 bemb-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7091 2023-05-20 21:17:04.000000 bemb-0.1.6/tests/test_bemb_functionality.py
```

### Comparing `bemb-0.1.5/LICENSE` & `bemb-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bemb-0.1.5/PKG-INFO` & `bemb-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bemb
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Pytorch Backend Library for Choice Modelling with Bayesian Matrix Factorization
 Home-page: 
 Author: Tianyu Du
 Author-email: tianyudu@stanford.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bemb-0.1.5/README.md` & `bemb-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `bemb-0.1.5/bemb/model/_bemb_dev.py` & `bemb-0.1.6/bemb/model/_bemb_dev.py`

 * *Files identical despite different names*

### Comparing `bemb-0.1.5/bemb/model/_bemb_flex.py` & `bemb-0.1.6/bemb/model/_bemb_flex.py`

 * *Files identical despite different names*

### Comparing `bemb-0.1.5/bemb/model/bayesian_coefficient.py` & `bemb-0.1.6/bemb/model/bayesian_coefficient.py`

 * *Files identical despite different names*

### Comparing `bemb-0.1.5/bemb/model/bayesian_linear.py` & `bemb-0.1.6/bemb/model/bayesian_linear.py`

 * *Files identical despite different names*

### Comparing `bemb-0.1.5/bemb/model/bemb.py` & `bemb-0.1.6/bemb/model/bemb.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 Author: Tianyu Du
 Update: Apr. 28, 2022
 """
 import warnings
 from pprint import pprint
 import warnings
 from typing import Dict, List, Optional, Tuple, Union
+from pprint import pprint
+from typing import Dict, List, Optional, Union, Tuple
 
 import numpy as np
 import torch
 import torch.nn as nn
 from torch_choice.data import ChoiceDataset
 from torch_scatter import scatter_logsumexp, scatter_max
 from torch_scatter.composite import scatter_log_softmax
@@ -103,28 +105,28 @@
                  obs2prior_dict: Dict[str, bool],
                  coef_dim_dict: Dict[str, int],
                  num_items: int,
                  pred_item: bool,
                  num_classes: int = 2,
                  H_zero_mask_dict: Optional[Dict[str, torch.BoolTensor]] = None,
                  prior_mean: Union[float, Dict[str, float]] = 0.0,
-                 default_prior_mean: float = 0.0,
                  prior_variance: Union[float, Dict[str, float]] = 1.0,
                  num_users: Optional[int] = None,
                  num_sessions: Optional[int] = None,
                  trace_log_q: bool = False,
                  category_to_item: Dict[int, List[int]] = None,
                  # number of observables.
                  num_user_obs: Optional[int] = None,
                  num_item_obs: Optional[int] = None,
                  num_session_obs: Optional[int] = None,
                  num_price_obs: Optional[int] = None,
                  num_taste_obs: Optional[int] = None,
                  # additional modules.
-                 additional_modules: Optional[List[nn.Module]] = None
+                 additional_modules: Optional[List[nn.Module]] = None,
+                 deterministic_variational: bool = False,
                  ) -> None:
         """
         Args:
             utility_formula (str): a string representing the utility function U[user, item, session].
                 See documentation for more details in the documentation for the format of formula.
                 Examples:
                     lambda_item
@@ -159,43 +161,47 @@
                 Case 1: which item among all items user `user_index[i]` is going to purchase, the prediction label
                     is therefore `item_index[i]`. Equivalently, we can ask what's the likelihood for user `user_index[i]`
                     to purchase `item_index[i]`.
                 Case 2: what rating would user `user_index[i]` assign to item `item_index[i]`? In this case, the dataset
                     object needs to contain a separate label.
                     NOTE: for now, we only support binary labels.
 
-            default_prior_mean (float): the default prior mean for coefficients,
-            if it is not specified in the prior_mean; defaults to 0.0.
-
             prior_mean (Union[float, Dict[str, float]]): the mean of prior
                 distribution for coefficients. If a float is provided, all prior
                 mean will be diagonal matrix with the provided value.  If a
                 dictionary is provided, keys of prior_mean should be coefficient
                 names, and the mean of prior of coef_name would the provided
                 value Defaults to 0.0, which means all prior means are
                 initialized to 0.0
 
+                If a dictionary prior_mean is supplied, for coefficient names not in the prior_mean.keys(), the
+                user can add a `prior_mean['default']` value to specify the mean for those coefficients.
+                If no `prior_mean['default']` is provided, the default prior mean will be 0.0 for those coefficients
+                not in the prior_mean.keys().
+
+                Defaults to 0.0.
+
             prior_variance (Union[float, Dict[str, float]], Dict[str, torch. Tensor]): the variance of prior distribution
                 for coefficients.
                 If a float is provided, all priors will be diagonal matrix with prior_variance along the diagonal.
                 If a float-valued dictionary is provided, keys of prior_variance should be coefficient names, and the
                 variance of prior of coef_name would be a diagonal matrix with prior_variance[coef_name] along the diagonal.
                 If a tensor-valued dictionary is provided, keys of prior_variance should be coefficient names, and the
                 values need to be tensor with shape (num_classes, coef_dim_dict[coef_name]). For example, for `beta_user` in
                 `U = beta_user * item_obs`, the prior_variance should be a tensor with shape (num_classes, dimension_of_item_obs).
                 In this case, every single entry in the coefficient has its own prior variance.
                 Following the `beta_user` example, for every `i` and `j`, `beta_user[i, j]` is a scalar with prior variance
                 `prior_variance['beta_user'][i, j]`. Moreover, `beta_user[i, j]`'s are independent for different `i, j`.
 
                 If a dictionary prior_variance is supplied, for coefficient names not in the prior_variance.keys(), the
-                can add a `prior_variance['default']` value to specify the variance for those coefficients.
+                user can add a `prior_variance['default']` value to specify the variance for those coefficients.
                 If no `prior_variance['default']` is provided, the default prior variance will be 1.0 for those coefficients
                 not in the prior_variance.keys().
 
-                Defaults to 1.0, which means all prior have identity matrix as the covariance matrix.
+                Defaults to 1.0, which means all priors have identity matrix as the covariance matrix.
 
             num_users (int, optional): number of users, required only if coefficient or observable
                 depending on user is in utility. Defaults to None.
             num_sessions (int, optional): number of sessions, required only if coefficient or
                 observable depending on session is in utility. Defaults to None.
 
             trace_log_q (bool, optional): whether to trace the derivative of variational likelihood logQ
@@ -208,39 +214,42 @@
                 Defaults to None.
 
             num_{user, item, session, price, taste}_obs (int, optional): number of observables of
                 each type of features, only required if observable enters prior.
                 NOTE: currently we only allow coefficient to depend on either user or item, thus only
                 user and item observables can enter the prior of coefficient. Hence session, price,
                 and taste observables are never required, we include it here for completeness.
+
+            deterministic_variational (bool, optional): if True, the variational posterior is equivalent to frequentist MLE estimates of parameters.
+                Note that this is equivalent to having a point mass with zero variance for the variational posterior.
+                Defaults to False.
         """
         super(BEMBFlex, self).__init__()
         self.utility_formula = utility_formula
         self.obs2prior_dict = obs2prior_dict
         self.coef_dim_dict = coef_dim_dict
         if H_zero_mask_dict is not None:
             self.H_zero_mask_dict = H_zero_mask_dict
         else:
             self.H_zero_mask_dict = dict()
         self.prior_variance = prior_variance
-        self.default_prior_mean = default_prior_mean
         self.prior_mean = prior_mean
-
         self.pred_item = pred_item
         if not self.pred_item:
             assert isinstance(num_classes, int) and num_classes > 0, \
                 f"With pred_item being False, the num_classes should be a positive integer, received {num_classes} instead."
             self.num_classes = num_classes
             if self.num_classes != 2:
                 raise NotImplementedError('Multi-class classification is not supported yet.')
             # we don't set the num_classes attribute when pred_item == False to avoid calling it accidentally.
 
         self.num_items = num_items
         self.num_users = num_users
         self.num_sessions = num_sessions
+        self.deterministic_variational = deterministic_variational
 
         self.trace_log_q = trace_log_q
         self.category_to_item = category_to_item
 
         # ==============================================================================================================
         # Category ID to Item ID mapping.
         # Category ID to Category Size mapping.
@@ -309,23 +318,32 @@
             'category' : self.num_categories,
         }
 
         coef_dict = dict()
         for additive_term in self.formula:
             for coef_name in additive_term['coefficient']:
                 variation = coef_name.split('_')[-1]
+                if isinstance(self.prior_mean, dict):
+                    # the user didn't specify prior mean for this coefficient.
+                    if coef_name not in self.prior_mean.keys():
+                        # the user may specify 'default' prior variance through the prior_variance dictionary.
+                        if 'default' in self.prior_mean.keys():
+                            self.prior_mean[coef_name] = self.prior_mean['default']
+                        else:
+                            warnings.warn(f"You provided a dictionary of prior mean, but coefficient {coef_name} is not a key in it. Supply a value for 'default' in the prior_mean dictionary to use that as default value (e.g., prior_mean['default'] = 0.1); now using mean=0.0 since this is not supplied.")
+                            self.prior_mean[coef_name] = 0.0
+
                 mean = self.prior_mean[coef_name] if isinstance(
-                    self.prior_mean, dict) else self.default_prior_mean
+                    self.prior_mean, dict) else self.prior_mean
 
                 if isinstance(self.prior_variance, dict):
                     # the user didn't specify prior variance for this coefficient.
                     if coef_name not in self.prior_variance.keys():
                         # the user may specify 'default' prior variance through the prior_variance dictionary.
                         if 'default' in self.prior_variance.keys():
-                            warnings.warn(f"You provided a dictionary of prior variance, but coefficient {coef_name} is not a key in it. We found a key 'default' in the dictionary, so we use the value of 'default' as the prior variance for coefficient {coef_name}.")
                             self.prior_variance[coef_name] = self.prior_variance['default']
                         else:
                             warnings.warn(f"You provided a dictionary of prior variance, but coefficient {coef_name} is not a key in it. Supply a value for 'default' in the prior_variance dictionary to use that as default value (e.g., prior_variance['default'] = 0.3); now using variance=1.0 since this is not supplied.")
                             self.prior_variance[coef_name] = 1.0
 
                 s2 = self.prior_variance[coef_name] if isinstance(
                     self.prior_variance, dict) else self.prior_variance
@@ -549,32 +567,29 @@
         # ==============================================================================================================
         assert return_type in [
             'log_prob', 'utility'], "return_type must be either 'log_prob' or 'utility'."
         assert return_scope in [
             'item_index', 'all_items'], "return_scope must be either 'item_index' or 'all_items'."
         assert deterministic in [True, False]
         if (not deterministic) and (sample_dict is None):
-            assert num_seeds >= 1, "A positive interger `num_seeds` is required if `deterministic` is False and no `sample_dict` is provided."
+            assert num_seeds >= 1, "A positive integer `num_seeds` is required if `deterministic` is False and no `sample_dict` is provided."
 
         # when pred_item is true, the model is predicting which item is bought (specified by item_index).
         if self.pred_item:
             batch.label = batch.item_index
 
         # ==============================================================================================================
         # get sample_dict ready.
         # ==============================================================================================================
         if deterministic:
             num_seeds = 1
             # Use the means of variational distributions as the sole deterministic MC sample.
             # NOTE: here we don't need to sample the obs2prior weight H since we only compute the log-likelihood.
             # TODO: is this correct?
-            sample_dict = dict()
-            for coef_name, coef in self.coef_dict.items():
-                sample_dict[coef_name] = coef.variational_distribution.mean.unsqueeze(
-                    dim=0)  # (1, num_*, dim)
+            sample_dict = self.sample_coefficient_dictionary(num_seeds, deterministic=True)
         else:
             if sample_dict is None:
                 # sample stochastic parameters.
                 sample_dict = self.sample_coefficient_dictionary(num_seeds)
             else:
                 # use the provided sample_dict.
                 num_seeds = list(sample_dict.values())[0].shape[0]
@@ -615,37 +630,43 @@
     def device(self) -> torch.device:
         for coef in self.coef_dict.values():
             return coef.device
 
     # ==================================================================================================================
     # helper functions.
     # ==================================================================================================================
-    def sample_coefficient_dictionary(self, num_seeds: int) -> Dict[str, torch.Tensor]:
+    def sample_coefficient_dictionary(self, num_seeds: int, deterministic: bool = False) -> Dict[str, torch.Tensor]:
         """A helper function to sample parameters from coefficients.
 
         Args:
             num_seeds (int): number of random samples.
+            deterministic (bool, optional): whether to use the mean of variational distributions as the sole sample.
 
         Returns:
             Dict[str, torch.Tensor]: a dictionary maps coefficient names to tensor of sampled coefficient parameters,
                 where the first dimension of the sampled tensor has size `num_seeds`.
                 Each sample tensor has shape (num_seeds, num_classes, dim).
         """
         sample_dict = dict()
         for coef_name, coef in self.coef_dict.items():
-            s = coef.rsample(num_seeds)
-            if coef.obs2prior:
-                # sample both obs2prior weight and realization of variable.
-                assert isinstance(s, tuple) and len(s) == 2
-                sample_dict[coef_name] = s[0]
-                sample_dict[coef_name + '.H'] = s[1]
+            if deterministic:
+                sample_dict[coef_name] = coef.variational_distribution.mean.unsqueeze(dim=0)  # (1, num_*, dim)
+                if coef.obs2prior:
+                    sample_dict[coef_name + '.H'] = coef.prior_H.variational_distribution.mean.unsqueeze(dim=0)  # (1, num_*, dim)
             else:
-                # only sample the realization of variable.
-                assert torch.is_tensor(s)
-                sample_dict[coef_name] = s
+                s = coef.rsample(num_seeds)
+                if coef.obs2prior:
+                    # sample both obs2prior weight and realization of variable.
+                    assert isinstance(s, tuple) and len(s) == 2
+                    sample_dict[coef_name] = s[0]
+                    sample_dict[coef_name + '.H'] = s[1]
+                else:
+                    # only sample the realization of variable.
+                    assert torch.is_tensor(s)
+                    sample_dict[coef_name] = s
         return sample_dict
 
     @torch.no_grad()
     def get_within_category_accuracy(self, log_p_all_items: torch.Tensor, label: torch.LongTensor) -> Dict[str, float]:
         """A helper function for computing prediction accuracy (i.e., all non-differential metrics)
         within category.
         In particular, this method calculates the accuracy, precision, recall and F1 score.
@@ -1280,29 +1301,29 @@
             raise NotImplementedError()
             # with shape (num_seeds,)
             total += module.log_variational().sum()
 
         return total
 
     def elbo(self, batch: ChoiceDataset, num_seeds: int = 1) -> torch.Tensor:
-        """A combined method to computes the current ELBO given a batch, this method is used for training the model.
+        """A combined method to compute the current ELBO given a batch, this method is used for training the model.
 
         Args:
             batch (ChoiceDataset): a ChoiceDataset containing necessary information.
             num_seeds (int, optional): the number of Monte Carlo samples from variational distributions
                 to evaluate the expectation in ELBO.
                 Defaults to 1.
 
         Returns:
             torch.Tensor: a scalar tensor of the ELBO estimated from num_seeds Monte Carlo samples.
         """
         # ==============================================================================================================
         # 1. sample latent variables from their variational distributions.
         # ==============================================================================================================
-        sample_dict = self.sample_coefficient_dictionary(num_seeds)
+        sample_dict = self.sample_coefficient_dictionary(num_seeds, self.deterministic_variational)
 
         # ==============================================================================================================
         # 2. compute log p(latent) prior.
         # (num_seeds,) --mean--> scalar.
         elbo = self.log_prior(batch, sample_dict).mean(dim=0)
         # ==============================================================================================================
 
@@ -1313,15 +1334,15 @@
         # ==============================================================================================================
         if self.pred_item:
             # the prediction target is item_index.
             elbo += self.forward(batch,
                                  return_type='log_prob',
                                  return_scope='item_index',
                                  deterministic=False,
-                                 sample_dict=sample_dict).sum(dim=1).mean(dim=0)  # (num_seeds, len(batch)) --> scalar.
+                                 sample_dict=sample_dict).sum(dim=1).mean(dim=0)
         else:
             # the prediction target is binary.
             # TODO: update the prediction function.
             utility = self.forward(batch,
                                    return_type='utility',
                                    return_scope='item_index',
                                    deterministic=False,
@@ -1337,10 +1358,11 @@
                        y_stacked).sum(dim=1).mean(dim=0)
             elbo += ll
 
         # ==============================================================================================================
         # 4. optionally add log likelihood under variational distributions q(latent).
         # ==============================================================================================================
         if self.trace_log_q:
+            assert not self.deterministic_variational, "deterministic_variational is not compatible with trace_log_q."
             elbo -= self.log_variational(sample_dict).mean(dim=0)
 
         return elbo
```

### Comparing `bemb-0.1.5/bemb/model/bemb_flex_lightning.py` & `bemb-0.1.6/bemb/model/bemb_flex_lightning.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,51 +12,65 @@
 import pytorch_lightning as pl
 import torch
 from sklearn import metrics
 from torch_choice.data import ChoiceDataset
 from torch_choice.data.utils import create_data_loader
 
 from bemb.model import BEMBFlex
+import numpy as np
+import torch
+import pytorch_lightning as pl
+from bemb.model import BEMBFlex
+from sklearn import metrics
 
 
 class LitBEMBFlex(pl.LightningModule):
 
-    def __init__(self, learning_rate: float = 0.3, num_seeds: int = 1, **kwargs):
+    def __init__(self,
+                 learning_rate: float = 0.3,
+                 num_seeds: int = 1,
+                 model_optimizer: str = "Adam",
+                 **kwargs):
         """The initialization method of the wrapper model.
 
         Args:
             learning_rate (float, optional): the learning rate of optimization. Defaults to 0.3.
             num_seeds (int, optional): number of random seeds for the Monte Carlo estimation in the variational inference.
                 Defaults to 1.
+            model_optimizer (str, optional): the optimizer used for training the model. Defaults to "Adam".
             **kwargs: all keyword arguments used for constructing the wrapped BEMB model.
         """
         # use kwargs to pass parameter to BEMB Torch.
         super().__init__()
         self.model = BEMBFlex(**kwargs)
-        self.num_needs = num_seeds
+        self.num_seeds = num_seeds
         self.learning_rate = learning_rate
+        self.optimizer_class_string = model_optimizer
 
     def __str__(self) -> str:
-        return str(self.model)
+        return str(self.model) + '\nOptimizer: ' + str(self.optimizer_class_string) + ', Learning rate: ' + str(self.learning_rate)
+
+    def __repr__(self) -> str:
+        return str(self)
 
     def forward(self, *args, **kwargs):
-        """Calls the forward method of the wrapped BEMB model, please refer to the documentaton of the BEMB class
+        """Calls the forward method of the wrapped BEMB model, please refer to the documentation of the BEMB class
             for detailed definitions of the arguments.
 
         Args:
             args (_type_): arguments passed to the forward method of the wrapped BEMB model.
             kwargs (_type_): keyword arguments passed to the forward method of the wrapped BEMB model.
 
         Returns:
             _type_: returns whatever the wrapped BEMB model returns.
         """
         return self.model(*args, **kwargs)
 
     def training_step(self, batch, batch_idx):
-        elbo = self.model.elbo(batch, num_seeds=self.num_needs)
+        elbo = self.model.elbo(batch, num_seeds=self.num_seeds)
         self.log('train_elbo', elbo)
         loss = - elbo
         return loss
 
     def _get_performance_dict(self, batch):
         if self.model.pred_item:
             log_p = self.model(batch, return_type='log_prob',
@@ -110,16 +124,15 @@
 
         # pred = self.model(batch)
         # performance = self.model.get_within_category_accuracy(pred, batch.label)
         for key, val in self._get_performance_dict(batch).items():
             self.log('test_' + key, val, prog_bar=True, batch_size=len(batch))
 
     def configure_optimizers(self):
-        optimizer = torch.optim.Adam(self.parameters(), lr=self.learning_rate)
-        return optimizer
+        return getattr(torch.optim, self.optimizer_class_string)(self.parameters(), lr=self.learning_rate)
 
     def fit_model(self, dataset_list: List[ChoiceDataset], batch_size: int=-1, num_epochs: int=10, num_workers: int=8, **kwargs) -> "LitBEMBFlex":
         """A standard pipeline of model training and evaluation.
 
         Args:
             dataset_list (List[ChoiceDataset]): train_dataset, validation_test, and test_dataset in a list of length 3.
             batch_size (int, optional): batch_size for training and evaluation. Defaults to -1, which indicates full-batch training.
```

### Comparing `bemb-0.1.5/bemb/utils/run_helper.py` & `bemb-0.1.6/bemb/utils/run_helper.py`

 * *Files identical despite different names*

### Comparing `bemb-0.1.5/bemb.egg-info/PKG-INFO` & `bemb-0.1.6/bemb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bemb
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Pytorch Backend Library for Choice Modelling with Bayesian Matrix Factorization
 Home-page: 
 Author: Tianyu Du
 Author-email: tianyudu@stanford.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bemb-0.1.5/setup.py` & `bemb-0.1.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="bemb",
-    version="0.1.5",
+    version="0.1.6",
     description="A Pytorch Backend Library for Choice Modelling with Bayesian Matrix Factorization",
     long_description=README,
     long_description_content_type="text/markdown",
     url="",
     author="Tianyu Du",
     author_email="tianyudu@stanford.edu",
     license="MIT",
```

