# Comparing `tmp/asociita-0.1.4.2.tar.gz` & `tmp/asociita-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asociita-0.1.4.2.tar", max compression
+gzip compressed data, was "asociita-0.1.5.tar", max compression
```

## Comparing `asociita-0.1.4.2.tar` & `asociita-0.1.5.tar`

### file list

```diff
@@ -1,26 +1,28 @@
--rw-r--r--   0        0        0        0 2023-04-07 16:31:28.755226 asociita-0.1.4.2/asociita/__init__.py
--rw-r--r--   0        0        0     4768 2023-04-27 12:57:58.598318 asociita-0.1.4.2/asociita/components/evaluator/evaluation_manager.py
--rw-r--r--   0        0        0    13585 2023-05-04 12:29:03.864051 asociita-0.1.4.2/asociita/components/evaluator/mr_evaluator.py
--rw-r--r--   0        0        0    10175 2023-05-03 13:58:58.211507 asociita-0.1.4.2/asociita/components/evaluator/or_evaluator.py
--rw-r--r--   0        0        0     4497 2023-04-17 14:01:29.838168 asociita-0.1.4.2/asociita/components/nodes/federated_node.py
--rw-r--r--   0        0        0     9733 2023-05-17 14:47:51.693120 asociita-0.1.4.2/asociita/components/orchestrator/evaluator_orchestrator.py
--rw-r--r--   0        0        0     6711 2023-05-09 09:31:15.259259 asociita-0.1.4.2/asociita/components/orchestrator/fedopt_orchestrator.py
--rw-r--r--   0        0        0    11325 2023-05-17 10:21:06.930212 asociita-0.1.4.2/asociita/components/orchestrator/generic_orchestrator.py
--rw-r--r--   0        0        0     1685 2023-05-17 14:12:22.175320 asociita-0.1.4.2/asociita/datasets/fetch_data.py
--rw-r--r--   0        0        0     7959 2023-05-17 13:06:20.822173 asociita-0.1.4.2/asociita/datasets/load_mnist.py
--rw-r--r--   0        0        0     4661 2023-05-12 12:28:36.608168 asociita-0.1.4.2/asociita/datasets/shard_transformation.py
--rw-r--r--   0        0        0    15252 2023-05-17 14:24:21.228395 asociita-0.1.4.2/asociita/models/pytorch/federated_model.py
--rw-r--r--   0        0        0      966 2023-05-12 12:18:20.228520 asociita-0.1.4.2/asociita/models/pytorch/mnist.py
--rw-r--r--   0        0        0     6068 2023-04-26 13:48:40.502010 asociita-0.1.4.2/asociita/utils/computations.py
--rw-r--r--   0        0        0      633 2023-05-12 12:12:31.672198 asociita-0.1.4.2/asociita/utils/custom_transformations.py
--rw-r--r--   0        0        0     4756 2023-05-17 12:51:14.070551 asociita-0.1.4.2/asociita/utils/handlers.py
--rw-r--r--   0        0        0      484 2023-05-16 12:10:20.265814 asociita-0.1.4.2/asociita/utils/helpers.py
--rw-r--r--   0        0        0     1843 2023-04-14 15:47:01.523825 asociita-0.1.4.2/asociita/utils/loggers.py
--rw-r--r--   0        0        0     3776 2023-04-24 11:46:41.291752 asociita-0.1.4.2/asociita/utils/optimizers.py
--rw-r--r--   0        0        0     4176 2023-04-19 13:27:23.001147 asociita-0.1.4.2/asociita/utils/orchestrations.py
--rw-r--r--   0        0        0     1059 2023-05-03 14:04:40.497199 asociita-0.1.4.2/asociita/utils/showcase.py
--rw-r--r--   0        0        0     1084 2023-04-07 16:30:34.501923 asociita-0.1.4.2/LICENSE
--rw-r--r--   0        0        0      671 2023-05-17 15:04:07.576690 asociita-0.1.4.2/pyproject.toml
--rw-r--r--   0        0        0     2862 2023-04-18 20:10:20.511705 asociita-0.1.4.2/README.md
--rw-r--r--   0        0        0     3941 1970-01-01 00:00:00.000000 asociita-0.1.4.2/setup.py
--rw-r--r--   0        0        0     3713 1970-01-01 00:00:00.000000 asociita-0.1.4.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-07 16:31:28.755226 asociita-0.1.5/asociita/__init__.py
+-rw-r--r--   0        0        0     3959 2023-05-20 16:17:12.712011 asociita-0.1.5/asociita/components/archiver/archive_manager.py
+-rw-r--r--   0        0        0     4768 2023-05-18 12:35:56.518494 asociita-0.1.5/asociita/components/evaluator/evaluation_manager.py
+-rw-r--r--   0        0        0    13585 2023-05-04 12:29:03.864051 asociita-0.1.5/asociita/components/evaluator/mr_evaluator.py
+-rw-r--r--   0        0        0    10175 2023-05-03 13:58:58.211507 asociita-0.1.5/asociita/components/evaluator/or_evaluator.py
+-rw-r--r--   0        0        0     4497 2023-04-17 14:01:29.838168 asociita-0.1.5/asociita/components/nodes/federated_node.py
+-rw-r--r--   0        0        0     7400 2023-05-20 16:22:57.462290 asociita-0.1.5/asociita/components/orchestrator/evaluator_orchestrator.py
+-rw-r--r--   0        0        0     6202 2023-05-20 16:45:47.898655 asociita-0.1.5/asociita/components/orchestrator/fedopt_orchestrator.py
+-rw-r--r--   0        0        0    10709 2023-05-20 16:39:01.642026 asociita-0.1.5/asociita/components/orchestrator/generic_orchestrator.py
+-rw-r--r--   0        0        0     1682 2023-05-19 17:32:35.712307 asociita-0.1.5/asociita/datasets/fetch_data.py
+-rw-r--r--   0        0        0     7959 2023-05-17 13:06:20.822173 asociita-0.1.5/asociita/datasets/load_mnist.py
+-rw-r--r--   0        0        0     4661 2023-05-12 12:28:36.608168 asociita-0.1.5/asociita/datasets/shard_transformation.py
+-rw-r--r--   0        0        0      329 2023-05-19 09:42:13.494113 asociita-0.1.5/asociita/exceptions/settingexception.py
+-rw-r--r--   0        0        0    15252 2023-05-19 10:09:48.869064 asociita-0.1.5/asociita/models/pytorch/federated_model.py
+-rw-r--r--   0        0        0      966 2023-05-12 12:18:20.228520 asociita-0.1.5/asociita/models/pytorch/mnist.py
+-rw-r--r--   0        0        0     6068 2023-04-26 13:48:40.502010 asociita-0.1.5/asociita/utils/computations.py
+-rw-r--r--   0        0        0      633 2023-05-12 12:12:31.672198 asociita-0.1.5/asociita/utils/custom_transformations.py
+-rw-r--r--   0        0        0     4756 2023-05-17 12:51:14.070551 asociita-0.1.5/asociita/utils/handlers.py
+-rw-r--r--   0        0        0      484 2023-05-16 12:10:20.265814 asociita-0.1.5/asociita/utils/helpers.py
+-rw-r--r--   0        0        0     1843 2023-04-14 15:47:01.523825 asociita-0.1.5/asociita/utils/loggers.py
+-rw-r--r--   0        0        0     3776 2023-04-24 11:46:41.291752 asociita-0.1.5/asociita/utils/optimizers.py
+-rw-r--r--   0        0        0     4176 2023-04-19 13:27:23.001147 asociita-0.1.5/asociita/utils/orchestrations.py
+-rw-r--r--   0        0        0     1059 2023-05-03 14:04:40.497199 asociita-0.1.5/asociita/utils/showcase.py
+-rw-r--r--   0        0        0     1084 2023-04-07 16:30:34.501923 asociita-0.1.5/LICENSE
+-rw-r--r--   0        0        0      669 2023-05-20 17:42:48.598223 asociita-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2862 2023-04-18 20:10:20.511705 asociita-0.1.5/README.md
+-rw-r--r--   0        0        0     3996 1970-01-01 00:00:00.000000 asociita-0.1.5/setup.py
+-rw-r--r--   0        0        0     3711 1970-01-01 00:00:00.000000 asociita-0.1.5/PKG-INFO
```

### Comparing `asociita-0.1.4.2/asociita/components/evaluator/evaluation_manager.py` & `asociita-0.1.5/asociita/components/evaluator/evaluation_manager.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.4.2/asociita/components/evaluator/mr_evaluator.py` & `asociita-0.1.5/asociita/components/evaluator/mr_evaluator.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.4.2/asociita/components/evaluator/or_evaluator.py` & `asociita-0.1.5/asociita/components/evaluator/or_evaluator.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.4.2/asociita/components/nodes/federated_node.py` & `asociita-0.1.5/asociita/components/nodes/federated_node.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.4.2/asociita/components/orchestrator/evaluator_orchestrator.py` & `asociita-0.1.5/asociita/components/orchestrator/evaluator_orchestrator.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from asociita.utils.orchestrations import create_nodes, sample_nodes, train_nodes
 from asociita.utils.computations import Aggregators
 from asociita.utils.handlers import Handler
 from asociita.utils.loggers import Loggers
 from asociita.utils.orchestrations import create_nodes, sample_nodes, train_nodes
 from asociita.utils.optimizers import Optimizers
 from asociita.components.evaluator.evaluation_manager import Evaluation_Manager
+from asociita.components.archiver.archive_manager import Archive_Manager
 # ADDITIONAL IMPORTS
 import datasets, copy
 from multiprocessing import Pool, Manager
 
 
 orchestrator_logger = Loggers.orchestrator_logger()
 
@@ -55,24 +56,27 @@
         # 1. SETTINGS -> CHANGE IF NEEDED
         # GENERAL SETTINGS
         iterations = self.settings['iterations'] # Number of iterations of the Fed training, int.
         nodes_number = self.settings['number_of_nodes'] # Number of nodes prepared for sampling, int.
         local_warm_start = self.settings["local_warm_start"] # Local warm start for pre-trained models - not implemented yet.
         nodes = self.settings["nodes"] # List of nodes, list[int]
         sample_size = self.settings["sample_size"] # Size of the sample, int.
-        save_path = self.settings["save_path"] # Save_path of all the relevant sim. details, str or path-like.
         # OPTIMIZER SETTINGS
         optimizer_settings = self.settings["optimizer"] # Dict containing instructions for the optimizer, dict.
         optimizer_name = optimizer_settings["name"] # Name of the optimizer, e.g. FedAdagard, dict.
         
 
         # 2. SET-UP PHASE -> CHANGE IF NEEDED
         # SETTING-UP EVALUATION MANAGER
         evaluation_maanger = Evaluation_Manager(settings=self.settings,
                                                 model=self.central_model)
+        archive_manager = Archive_Manager(archive_manager = self.settings['archiver'],
+                                          logger = orchestrator_logger)
+        self.metrics_save_path = self.settings['metrics_save_path']
+
         # CREATING FEDERATED NODES
         nodes_green = create_nodes(nodes, self.node_settings)
         # CREATING LOCAL MODELS (that will be loaded onto nodes)
         model_list = self.model_initialization(nodes_number=nodes_number,
                                                model=self.central_net)
         # INITIALIZING ALL THE NODES
         nodes_green = self.nodes_initialization(nodes_list=nodes_green,
@@ -106,65 +110,26 @@
                     grad_avg = Aggregators.compute_average(gradients) # AGGREGATING FUNCTION -> CHANGE IF NEEDED
                     updated_weights = Optim.fed_optimize(optimizer=optimizer_name,
                                                          settings=optimizer_settings,
                                                          weights=self.central_model.get_weights(),
                                                          delta=grad_avg)
                     # TRACKING GRADIENTS FOR EVALUATION
                     evaluation_maanger.track_gradients(gradients=gradients) # TRACKING FUNCTION -> CHANGE IF NEEDED
-
+                    ### WEIGHTS UPDATE
                     # Updating the nodes
                     for node in nodes_green:
                         node.model.update_weights(updated_weights)
                     # Upadting the orchestrator
-                    self.central_model.update_weights(updated_weights)
-
-                    # SAVING TRAINING METRICS <- ONLY IF ENABLED IN SETTINGS
-                    if self.settings['training_evaluation'] == 'log_and_save':
-                        Handler.save_model_metrics(iteration=iteration,
-                            model = self.central_model,
-                            logger = orchestrator_logger,
-                            saving_path = save_path,
-                            log_to_screen = True,
-                            file_name=self.training_metrics_filename) # PRESERVING METRICS FUNCTION -> CHANGE IF NEEDED
-                    elif self.settings['training_evaluation'] == 'log':
-                        Handler.log_model_metrics(iteration=iteration,
-                                                logger = orchestrator_logger,
-                                                model = self.central_model)
-                    else:
-                        orchestrator_logger.warning("No training metrics being preserved. To enable metric preservation add 'log_and_save' or 'log' to settings.")
-                    
-
-                    # SAVING NODES METRICS <- ONLY IF ENABLED IN SETTINGS
-                    if self.settings['nodes_evaluation'] == 'log_and_save':
-                        for node in nodes_green:
-                            Handler.save_model_metrics(iteration=iteration,
-                                model = node.model,
-                                logger = orchestrator_logger,
-                                saving_path = save_path,
-                                log_to_screen = True,
-                                file_name=self.nodes_metrics_filename) # PRESERVING METRICS FUNCTION -> CHANGE IF NEEDED
-                    elif self.settings['nodes_evaluation'] == 'log':
-                        for nodes in nodes_green:
-                            Handler.log_model_metrics(iteration=iteration,
-                                                    logger = orchestrator_logger,
-                                                    model = node.model)
-                    else:
-                        orchestrator_logger.warning("No nodes metrics being preserved. To enable metric preservation add 'log_and_save' or 'log' to settings.")
-
-                    if self.settings['model_preservation'] == 'full':
-                        # Saving general model
-                        self.central_model.store_model_on_disk(iteration = iteration,
-                                                               path = self.settings['central_model_preservation_path'])
-                        for node in nodes_green:
-                            node.model.store_model_on_disk(iteration=iteration,
-                                                           path=self.settings['local_model_preservation_path'])
-                    
+                    self.central_model.update_weights(updated_weights)                 
+                    archive_manager.archive_training_results(iteration = iteration,
+                                                             central_model=self.central_model,
+                                                             nodes=nodes_green)
         # 4. FINALIZING PHASE
         # EVALUATING THE RESULTS
         evaluation_results, mapped_results = evaluation_maanger.calculate_results()
         
         # FINAL MESSAGES
         print(evaluation_results)
         print(mapped_results)
-        evaluation_maanger.save_results(path = save_path,
+        evaluation_maanger.save_results(path = self.metrics_save_path,
                                         mapped_results=mapped_results)
         orchestrator_logger.critical("Training complete")
```

### Comparing `asociita-0.1.4.2/asociita/components/orchestrator/fedopt_orchestrator.py` & `asociita-0.1.5/asociita/components/orchestrator/fedopt_orchestrator.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from asociita.components.nodes.federated_node import FederatedNode
 from asociita.models.pytorch.federated_model import FederatedModel
 from asociita.utils.computations import Aggregators
 from asociita.utils.handlers import Handler
 from asociita.utils.loggers import Loggers
 from asociita.utils.orchestrations import prepare_nodes, create_nodes, check_health, sample_nodes, train_nodes
 from asociita.utils.optimizers import Optimizers
+from asociita.components.archiver.archive_manager import Archive_Manager
 from multiprocessing import Pool, Manager
 from torch import nn
 
 orchestrator_logger = Loggers.orchestrator_logger()
 
 
 class Fedopt_Orchestrator(Orchestrator):
@@ -52,15 +53,16 @@
         # SETTINGS -> CHANGE IF NEEDED
         # GENERAL SETTINGS
         iterations = self.settings['iterations']
         nodes_number = self.settings['number_of_nodes']
         local_warm_start = self.settings["local_warm_start"]
         nodes = self.settings["nodes"]
         sample_size = self.settings["sample_size"]
-        save_path = self.settings["save_path"]
+        archive_manager = Archive_Manager(archive_manager = self.settings['archiver'],
+                                          logger = orchestrator_logger)
 
         # OPTIMIZER SETTINGS
         optimizer_settings = self.settings["optimizer"]
         optimizer_name = optimizer_settings["name"]
         
         # CREATING FEDERATED NODES
         nodes_green = create_nodes(nodes, self.node_settings) # Exterior method / function, can override in childr.
@@ -107,24 +109,12 @@
                                                          delta=grad_avg)
                     # Updating the nodes
                     for node in nodes_green:
                         node.model.update_weights(updated_weights)
                     # Upadting the orchestrator
                     self.central_model.update_weights(updated_weights)
 
-                    # SAVING METRICS <- ONLY IF ENABLED IN SETTINGS
-                    Handler.save_model_metrics(iteration=iteration,
-                        model = self.central_model,
-                        logger = orchestrator_logger,
-                        saving_path= save_path,
-                        log_to_screen=True,
-                        file_name=self.metrics_filename) # PRESERVING METRICS FUNCTION -> CHANGE IF NEEDED
-                    
-                    # LOGGING METRICS <- ONLY IF ENABLED IN SETTINGS
-                    # Logging the metrics of sample or all nodes
-                    if self.settings['evaluation'] == "full":
-                        for node in nodes_green:
-                            Handler.log_model_metrics(iteration=iteration,
-                                model = node.model,
-                                logger = orchestrator_logger) # LOGGING METRICS FUNCTION -> CHANGE IF NEEDED
+                    archive_manager.archive_training_results(iteration = iteration,
+                                                             central_model=self.central_model,
+                                                             nodes=nodes_green)
         
         orchestrator_logger.critical("Training complete")
```

### Comparing `asociita-0.1.4.2/asociita/components/orchestrator/generic_orchestrator.py` & `asociita-0.1.5/asociita/components/orchestrator/generic_orchestrator.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Any, Union
 from asociita.components.nodes.federated_node import FederatedNode
 from asociita.models.pytorch.federated_model import FederatedModel
 from asociita.utils.computations import Aggregators
 from asociita.utils.handlers import Handler
 from asociita.utils.loggers import Loggers
 from asociita.utils.orchestrations import prepare_nodes, create_nodes, check_health, sample_nodes, train_nodes
+from asociita.components.archiver.archive_manager import Archive_Manager
 from multiprocessing import Pool, Manager
 from torch import nn
 
 
 orchestrator_logger = Loggers.orchestrator_logger()
 
 class Orchestrator():
@@ -162,16 +163,16 @@
         
         # SETTINGS -> CHANGE IF NEEDED
         iterations = self.settings['iterations']
         nodes_number = self.settings['number_of_nodes']
         local_warm_start = self.settings["local_warm_start"]
         nodes = self.settings["nodes"]
         sample_size = self.settings["sample_size"]
-        save_path = self.settings["save_path"]
-        
+        archive_manager = Archive_Manager(archive_manager = self.settings['archiver'],
+                                          logger = orchestrator_logger)
 
         # CREATING FEDERATED NODES
         nodes_green = create_nodes(nodes, self.node_settings) # Exterior method / function, can override in childr.
 
 
         # CREATING LOCAL MODELS (that will be loaded onto nodes)
         model_list = self.model_initialization(nodes_number=nodes_number,
@@ -204,26 +205,13 @@
                     avg = Aggregators.compute_average(weights) # AGGREGATING FUNCTION -> CHANGE IF NEEDED
                     # Updating the nodes
                     for node in nodes_green:
                         node.model.update_weights(avg)
                     # Upadting the orchestrator
                     self.central_model.update_weights(avg)
 
-                    # SAVING METRICS <- ONLY IF ENABLED IN SETTINGS
-                    if self.settings['save_metrics'] == True:
-                        Handler.save_model_metrics(iteration=iteration,
-                            model = self.central_model,
-                            logger = orchestrator_logger,
-                            saving_path= save_path,
-                            log_to_screen=True,
-                            file_name = self.metrics_filename) # PRESERVING METRICS FUNCTION -> CHANGE IF NEEDED
-                    
-                    # LOGGING METRICS <- ONLY IF ENABLED IN SETTINGS
-                    # Logging the metrics of sample or all nodes
-                    if self.settings['evaluation'] == "full":
-                        for node in nodes_green:
-                            Handler.log_model_metrics(iteration=iteration,
-                                model = node.model,
-                                logger = orchestrator_logger) # LOGGING METRICS FUNCTION -> CHANGE IF NEEDED
-        
+                    archive_manager.archive_training_results(iteration = iteration,
+                                                             central_model=self.central_model,
+                                                             nodes=nodes_green)
+
         orchestrator_logger.critical("Training complete")
```

### Comparing `asociita-0.1.4.2/asociita/datasets/fetch_data.py` & `asociita-0.1.5/asociita/datasets/fetch_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,15 @@
                                        list[list[list[datasets.arrow_dataset.Dataset]]]]"""
     
     dataset_name = settings['dataset_name']
     if dataset_name == 'mnist':
         loaded_dataset = load_mnist(settings=settings)
         if settings['save_dataset'] == True:
             dataset_name = f"MNIST_{settings['shards']}_dataset"
-            path = os.path.join(settings['dataset_path'], dataset_name)
+            path = os.path.join(settings['save_path'], dataset_name)
             with open(path, 'wb') as file:
                 pickle.dump(loaded_dataset, file)
             return loaded_dataset
         else:
             return loaded_dataset
     else:
         logging.warning("Wrong name of the dataset. Please provide a valid name.")
```

### Comparing `asociita-0.1.4.2/asociita/datasets/load_mnist.py` & `asociita-0.1.5/asociita/datasets/load_mnist.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.4.2/asociita/datasets/shard_transformation.py` & `asociita-0.1.5/asociita/datasets/shard_transformation.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.4.2/asociita/models/pytorch/federated_model.py` & `asociita-0.1.5/asociita/models/pytorch/federated_model.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.4.2/asociita/models/pytorch/mnist.py` & `asociita-0.1.5/asociita/models/pytorch/mnist.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.4.2/asociita/utils/computations.py` & `asociita-0.1.5/asociita/utils/computations.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.4.2/asociita/utils/custom_transformations.py` & `asociita-0.1.5/asociita/utils/custom_transformations.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.4.2/asociita/utils/handlers.py` & `asociita-0.1.5/asociita/utils/handlers.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.4.2/asociita/utils/loggers.py` & `asociita-0.1.5/asociita/utils/loggers.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.4.2/asociita/utils/optimizers.py` & `asociita-0.1.5/asociita/utils/optimizers.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.4.2/asociita/utils/orchestrations.py` & `asociita-0.1.5/asociita/utils/orchestrations.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.4.2/asociita/utils/showcase.py` & `asociita-0.1.5/asociita/utils/showcase.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.4.2/LICENSE` & `asociita-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `asociita-0.1.4.2/pyproject.toml` & `asociita-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asociita"
-version = "0.1.4.2"
+version = "0.1.5"
 description = "An intuitive and modular simulator for assessing the marginal value of a client's contribution in a decentralized setting."
 authors = ["Maciej Zuziak <maciejkrzysztof.zuziak@isti.cnr.it>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Scolpe/Asociita"
 repository = "https://github.com/Scolpe/Asociita"
```

### Comparing `asociita-0.1.4.2/README.md` & `asociita-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `asociita-0.1.4.2/setup.py` & `asociita-0.1.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['asociita',
+ 'asociita.components.archiver',
  'asociita.components.evaluator',
  'asociita.components.nodes',
  'asociita.components.orchestrator',
  'asociita.datasets',
+ 'asociita.exceptions',
  'asociita.models.pytorch',
  'asociita.utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
@@ -19,15 +21,15 @@
  'numpy>=1.24.1,<2.0.0',
  'scikit-learn>=1.2.0,<2.0.0',
  'torch>=1.13.1,<2.0.0',
  'torchvision>=0.14.1,<0.15.0']
 
 setup_kwargs = {
     'name': 'asociita',
-    'version': '0.1.4.2',
+    'version': '0.1.5',
     'description': "An intuitive and modular simulator for assessing the marginal value of a client's contribution in a decentralized setting.",
     'long_description': '### Setting Configuration\n\nIn order to run the simulation, the `Orchestrator` instance must receive a `settings` object that contains all the necessary parameters. It is possible to store those parameters in a `JSON` format and load them as the Python dictionary by using `asociita.utils.helper.load_from_json` function. Below is an exemplary settings object embedded as a `json` file. All the elements are necessary unless stated otherwise.\n\n```\n{\n    "orchestrator":{\n        "iterations": int,\n        "number_of_nodes": int,\n        "local_warm_start": bool,\n        "sample_size": int,\n        "evaluation": "none" | "full"\n        "save_metrics": bool,\n\t"save_models": bool,\n\t"save_path": str\n\t"nodes": [0,\n\t1,\n\t2]\n    },\n    "nodes":{\n    "local_epochs": int,\n    "model_settings": {\n        "optimizer": "RMS",\n        "batch_size": int,\n        "learning_rate": float}\n        }\n}\n```\n\nThe `settings` contains two dictionaries: `orchestrator` and `nodes`.\n\n`orchestrator` contains all the settings necessary details of the training:\n\n* `iterations` is the number of rounds to be performed. Example: `iterations:12`\n* `number_of_nodes` is the number of nodes that will be included in the training. Example: `number_of_nodes: 10`\n* `local_warm_start` allows to distribute various pre-trained weights to different local clients. Not implemeneted yet. Example: `local_warm_start: false`.\n* `sample_size` is the size of the sample that will be taken each round. Example: `sample_size : 4.`\n* `evaluation` allows to control the evaluation procedure across the clients.  Currently, only `none` or `full` are supported. Setting the evaluation to full will perform a full evaluation of every client included in the training. Example: `evaluation: full`\n* `save_metrics` allows to control whether the metrics should be saved in a csv file. Example: `save_metrics: true.`\n* `save_models` allows to control whether the models should be saved. Not implemeneted yet. Example: `save_metrics: false`.\n* `save_path` is the system path that will be used when saving the model. It is possible to define a saving_path in a method call.\n* `nodes` is the list containing the ids of all the nodes participating in the training. Length of `nodes` must be equal `number_of_nodes`.\n\n`nodes` contains all the necessary configuration for nodes.\n\n* `"local_epochs":` the number of local epochs to be performed on the local nodes.\n* `"model_settings"` is a dictionary containing all the parameters for training the model.\n  * `optimizer` is an optimizer that will be used during the training. Example: `optimizer: "RMS"`\n  * `batch_size` is the batch size that will be used during the training. Example: `batch_size: 32`\n  * `learning_rate` is the learning rate that will be used during the training. Example: `learning_rate: 0.001`\n',
     'author': 'Maciej Zuziak',
     'author_email': 'maciejkrzysztof.zuziak@isti.cnr.it',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Scolpe/Asociita',
```

### Comparing `asociita-0.1.4.2/PKG-INFO` & `asociita-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asociita
-Version: 0.1.4.2
+Version: 0.1.5
 Summary: An intuitive and modular simulator for assessing the marginal value of a client's contribution in a decentralized setting.
 Home-page: https://github.com/Scolpe/Asociita
 License: MIT
 Author: Maciej Zuziak
 Author-email: maciejkrzysztof.zuziak@isti.cnr.it
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

