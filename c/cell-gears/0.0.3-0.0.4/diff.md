# Comparing `tmp/cell-gears-0.0.3.tar.gz` & `tmp/cell-gears-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cell-gears-0.0.3.tar", last modified: Sat Apr 15 23:25:39 2023, max compression
+gzip compressed data, was "cell-gears-0.0.4.tar", last modified: Sat May 20 04:16:54 2023, max compression
```

## Comparing `cell-gears-0.0.3.tar` & `cell-gears-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 yhr      (20138) users      (100)        0 2023-04-15 23:25:39.315057 cell-gears-0.0.3/
--rw-r--r--   0 yhr      (20138) users      (100)     1098 2023-04-15 23:05:14.000000 cell-gears-0.0.3/LICENSE
--rw-r--r--   0 yhr      (20138) users      (100)       69 2023-04-15 23:05:14.000000 cell-gears-0.0.3/MANIFEST.in
--rw-r--r--   0 yhr      (20138) users      (100)     3253 2023-04-15 23:25:39.322057 cell-gears-0.0.3/PKG-INFO
--rw-r--r--   0 yhr      (20138) users      (100)     3008 2023-04-15 23:05:14.000000 cell-gears-0.0.3/README.md
-drwxr-xr-x   0 yhr      (20138) users      (100)        0 2023-04-15 23:25:39.156064 cell-gears-0.0.3/cell_gears.egg-info/
--rw-r--r--   0 yhr      (20138) users      (100)     3253 2023-04-15 23:25:38.000000 cell-gears-0.0.3/cell_gears.egg-info/PKG-INFO
--rw-r--r--   0 yhr      (20138) users      (100)      404 2023-04-15 23:25:38.000000 cell-gears-0.0.3/cell_gears.egg-info/SOURCES.txt
--rw-r--r--   0 yhr      (20138) users      (100)        1 2023-04-15 23:25:38.000000 cell-gears-0.0.3/cell_gears.egg-info/dependency_links.txt
--rw-r--r--   0 yhr      (20138) users      (100)        1 2023-04-15 23:25:38.000000 cell-gears-0.0.3/cell_gears.egg-info/not-zip-safe
--rw-r--r--   0 yhr      (20138) users      (100)       58 2023-04-15 23:25:38.000000 cell-gears-0.0.3/cell_gears.egg-info/requires.txt
--rw-r--r--   0 yhr      (20138) users      (100)        6 2023-04-15 23:25:38.000000 cell-gears-0.0.3/cell_gears.egg-info/top_level.txt
-drwxr-xr-x   0 yhr      (20138) users      (100)        0 2023-04-15 23:25:39.292058 cell-gears-0.0.3/gears/
--rw-r--r--   0 yhr      (20138) users      (100)       55 2023-04-15 23:05:14.000000 cell-gears-0.0.3/gears/__init__.py
--rw-r--r--   0 yhr      (20138) users      (100)    18902 2023-04-15 23:05:14.000000 cell-gears-0.0.3/gears/data_utils.py
--rw-r--r--   0 yhr      (20138) users      (100)    22799 2023-04-15 23:05:14.000000 cell-gears-0.0.3/gears/gears.py
--rw-r--r--   0 yhr      (20138) users      (100)    39585 2023-04-15 23:05:14.000000 cell-gears-0.0.3/gears/inference.py
--rw-r--r--   0 yhr      (20138) users      (100)     9126 2023-04-15 23:05:14.000000 cell-gears-0.0.3/gears/model.py
--rw-r--r--   0 yhr      (20138) users      (100)    16994 2023-04-15 23:05:14.000000 cell-gears-0.0.3/gears/pertdata.py
--rw-r--r--   0 yhr      (20138) users      (100)    17572 2023-04-15 23:05:15.000000 cell-gears-0.0.3/gears/utils.py
--rw-r--r--   0 yhr      (20138) users      (100)      537 2023-04-15 23:24:35.000000 cell-gears-0.0.3/gears/version.py
--rw-r--r--   0 yhr      (20138) users      (100)       57 2023-04-15 23:05:15.000000 cell-gears-0.0.3/requirements.txt
--rw-r--r--   0 yhr      (20138) users      (100)       79 2023-04-15 23:25:39.331056 cell-gears-0.0.3/setup.cfg
--rw-r--r--   0 yhr      (20138) users      (100)     1149 2023-04-15 23:05:15.000000 cell-gears-0.0.3/setup.py
+drwxr-xr-x   0 yhr      (20138) users      (100)        0 2023-05-20 04:16:54.481434 cell-gears-0.0.4/
+-rw-r--r--   0 yhr      (20138) users      (100)     1098 2023-05-20 04:05:18.000000 cell-gears-0.0.4/LICENSE
+-rw-r--r--   0 yhr      (20138) users      (100)       69 2023-05-20 04:05:18.000000 cell-gears-0.0.4/MANIFEST.in
+-rw-r--r--   0 yhr      (20138) users      (100)     3255 2023-05-20 04:16:54.494434 cell-gears-0.0.4/PKG-INFO
+-rw-r--r--   0 yhr      (20138) users      (100)     3010 2023-05-20 04:05:18.000000 cell-gears-0.0.4/README.md
+drwxr-xr-x   0 yhr      (20138) users      (100)        0 2023-05-20 04:16:54.175448 cell-gears-0.0.4/cell_gears.egg-info/
+-rw-r--r--   0 yhr      (20138) users      (100)     3255 2023-05-20 04:16:53.000000 cell-gears-0.0.4/cell_gears.egg-info/PKG-INFO
+-rw-r--r--   0 yhr      (20138) users      (100)      404 2023-05-20 04:16:53.000000 cell-gears-0.0.4/cell_gears.egg-info/SOURCES.txt
+-rw-r--r--   0 yhr      (20138) users      (100)        1 2023-05-20 04:16:53.000000 cell-gears-0.0.4/cell_gears.egg-info/dependency_links.txt
+-rw-r--r--   0 yhr      (20138) users      (100)        1 2023-05-20 04:16:53.000000 cell-gears-0.0.4/cell_gears.egg-info/not-zip-safe
+-rw-r--r--   0 yhr      (20138) users      (100)       58 2023-05-20 04:16:53.000000 cell-gears-0.0.4/cell_gears.egg-info/requires.txt
+-rw-r--r--   0 yhr      (20138) users      (100)        6 2023-05-20 04:16:53.000000 cell-gears-0.0.4/cell_gears.egg-info/top_level.txt
+drwxr-xr-x   0 yhr      (20138) users      (100)        0 2023-05-20 04:16:54.440436 cell-gears-0.0.4/gears/
+-rw-r--r--   0 yhr      (20138) users      (100)       55 2023-05-20 04:05:18.000000 cell-gears-0.0.4/gears/__init__.py
+-rw-r--r--   0 yhr      (20138) users      (100)    18902 2023-05-20 04:05:18.000000 cell-gears-0.0.4/gears/data_utils.py
+-rw-r--r--   0 yhr      (20138) users      (100)    22807 2023-05-20 04:05:18.000000 cell-gears-0.0.4/gears/gears.py
+-rw-r--r--   0 yhr      (20138) users      (100)    39585 2023-05-20 04:05:18.000000 cell-gears-0.0.4/gears/inference.py
+-rw-r--r--   0 yhr      (20138) users      (100)     9126 2023-05-20 04:05:18.000000 cell-gears-0.0.4/gears/model.py
+-rw-r--r--   0 yhr      (20138) users      (100)    17993 2023-05-20 04:05:18.000000 cell-gears-0.0.4/gears/pertdata.py
+-rw-r--r--   0 yhr      (20138) users      (100)    17959 2023-05-20 04:05:18.000000 cell-gears-0.0.4/gears/utils.py
+-rw-r--r--   0 yhr      (20138) users      (100)      537 2023-05-20 04:16:28.000000 cell-gears-0.0.4/gears/version.py
+-rw-r--r--   0 yhr      (20138) users      (100)       57 2023-05-20 04:05:18.000000 cell-gears-0.0.4/requirements.txt
+-rw-r--r--   0 yhr      (20138) users      (100)       79 2023-05-20 04:16:54.517433 cell-gears-0.0.4/setup.cfg
+-rw-r--r--   0 yhr      (20138) users      (100)     1149 2023-05-20 04:05:18.000000 cell-gears-0.0.4/setup.py
```

### Comparing `cell-gears-0.0.3/LICENSE` & `cell-gears-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cell-gears-0.0.3/PKG-INFO` & `cell-gears-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cell-gears
-Version: 0.0.3
+Version: 0.0.4
 Summary: GEARS
 Home-page: https://github.com/snap-stanford/GEARS
 Author: Yusuf Roohani, Kexin Huang, Jure Leskovec
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -43,15 +43,15 @@
 
 # save/load model
 gears_model.save_model('gears')
 gears_model.load_pretrained('gears')
 
 # predict
 gears_model.predict([['CBL', 'CNN1'], ['FEV']])
-gears_model.GI_predict([['CBL', 'CNN1'], ['FEV', 'AHR']])
+gears_model.GI_predict(['CBL', 'CNN1'], GI_genes_file=None)
 ```
 
 To use your own dataset, create a scanpy adata object with a `gene_name` column in `adata.var`, and two columns `condition`, `cell_type` in `adata.obs`. Then run:
 
 ```python
 pert_data.new_data_process(dataset_name = 'XXX', adata = adata)
 # to load the processed data
```

### Comparing `cell-gears-0.0.3/README.md` & `cell-gears-0.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 # save/load model
 gears_model.save_model('gears')
 gears_model.load_pretrained('gears')
 
 # predict
 gears_model.predict([['CBL', 'CNN1'], ['FEV']])
-gears_model.GI_predict([['CBL', 'CNN1'], ['FEV', 'AHR']])
+gears_model.GI_predict(['CBL', 'CNN1'], GI_genes_file=None)
 ```
 
 To use your own dataset, create a scanpy adata object with a `gene_name` column in `adata.var`, and two columns `condition`, `cell_type` in `adata.obs`. Then run:
 
 ```python
 pert_data.new_data_process(dataset_name = 'XXX', adata = adata)
 # to load the processed data
```

### Comparing `cell-gears-0.0.3/cell_gears.egg-info/PKG-INFO` & `cell-gears-0.0.4/cell_gears.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cell-gears
-Version: 0.0.3
+Version: 0.0.4
 Summary: GEARS
 Home-page: https://github.com/snap-stanford/GEARS
 Author: Yusuf Roohani, Kexin Huang, Jure Leskovec
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -43,15 +43,15 @@
 
 # save/load model
 gears_model.save_model('gears')
 gears_model.load_pretrained('gears')
 
 # predict
 gears_model.predict([['CBL', 'CNN1'], ['FEV']])
-gears_model.GI_predict([['CBL', 'CNN1'], ['FEV', 'AHR']])
+gears_model.GI_predict(['CBL', 'CNN1'], GI_genes_file=None)
 ```
 
 To use your own dataset, create a scanpy adata object with a `gene_name` column in `adata.var`, and two columns `condition`, `cell_type` in `adata.obs`. Then run:
 
 ```python
 pert_data.new_data_process(dataset_name = 'XXX', adata = adata)
 # to load the processed data
```

### Comparing `cell-gears-0.0.3/gears/data_utils.py` & `cell-gears-0.0.4/gears/data_utils.py`

 * *Files identical despite different names*

### Comparing `cell-gears-0.0.3/gears/gears.py` & `cell-gears-0.0.4/gears/gears.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         self.set2conditions = pert_data.set2conditions
         self.subgroup = pert_data.subgroup
         self.gi_predict = gi_predict
         self.gene_list = pert_data.gene_names.values.tolist()
         self.pert_list = pert_data.pert_names.tolist()
         self.num_genes = len(self.gene_list)
         self.num_perts = len(self.pert_list)
-        self.default_GO_graph = pert_data.default_GO_graph
+        self.default_pert_graph = pert_data.default_pert_graph
         self.saved_pred = {}
         self.saved_logvar_sum = {}
         
         self.ctrl_expression = torch.tensor(
             np.mean(self.adata.X[self.adata.obs.condition == 'ctrl'],
                     axis=0)).reshape(-1, ).to(self.device)
         pert_full_id2pert = dict(self.adata.obs[['condition_name', 'condition']].values)
@@ -161,15 +161,15 @@
                                                k=num_similar_genes_go_graph,
                                                pert_list=self.pert_list,
                                                data_path=self.data_path,
                                                data_name=self.dataset_name,
                                                split=self.split, seed=self.seed,
                                                train_gene_set_size=self.train_gene_set_size,
                                                set2conditions=self.set2conditions,
-                                               default_GO_graph=self.default_GO_graph)
+                                               default_pert_graph=self.default_pert_graph)
 
             sim_network = GeneSimNetwork(edge_list, self.pert_list, node_map = self.node_map_pert)
             self.config['G_go'] = sim_network.edge_index
             self.config['G_go_weight'] = sim_network.edge_weight
             
         self.model = GEARS_Model(self.config).to(self.device)
         self.best_model = deepcopy(self.model)
@@ -213,15 +213,15 @@
         ## if uncertainty mode is on, also return uncertainty score.
         
         self.ctrl_adata = self.adata[self.adata.obs['condition'] == 'ctrl']
         for pert in pert_list:
             for i in pert:
                 if i not in self.pert_list:
                     raise ValueError(i+ " is not in the perturbation graph. "
-                                        "Please select from GEARS.gene_list!")
+                                        "Please select from GEARS.pert_list!")
         
         if self.config['uncertainty']:
             results_logvar = {}
             
         self.best_model = self.best_model.to(self.device)
         self.best_model.eval()
         results_pred = {}
```

### Comparing `cell-gears-0.0.3/gears/inference.py` & `cell-gears-0.0.4/gears/inference.py`

 * *Files identical despite different names*

### Comparing `cell-gears-0.0.3/gears/model.py` & `cell-gears-0.0.4/gears/model.py`

 * *Files identical despite different names*

### Comparing `cell-gears-0.0.3/gears/pertdata.py` & `cell-gears-0.0.4/gears/pertdata.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,23 +10,27 @@
 import pandas as pd
 
 import warnings
 warnings.filterwarnings("ignore")
 sc.settings.verbosity = 0
 
 from .data_utils import get_DE_genes, get_dropout_non_zero_genes, DataSplitter
-from .utils import print_sys, zip_data_download_wrapper, dataverse_download, filter_pert_in_go
+from .utils import print_sys, zip_data_download_wrapper, dataverse_download,\
+                  filter_pert_in_go, get_genes_from_perts
 
 class PertData:
     
-    def __init__(self, data_path, gene_set_path = None):
+    def __init__(self, data_path, 
+                 gene_set_path=None, 
+                 default_pert_graph=True):
         
         # Dataset/Dataloader attributes
         self.data_path = data_path
-        self.default_GO_graph = True
+        self.default_pert_graph = default_pert_graph
+        self.gene_set_path = gene_set_path
         self.dataset_name = None
         self.dataset_path = None
         self.adata = None
         self.dataset_processed = None
         self.ctrl_adata = None
         self.gene_names = []
         self.node_map = {}
@@ -39,35 +43,56 @@
 
         if not os.path.exists(self.data_path):
             os.mkdir(self.data_path)
         server_path = 'https://dataverse.harvard.edu/api/access/datafile/6153417'
         dataverse_download(server_path,
                            os.path.join(self.data_path, 'gene2go_all.pkl'))
         with open(os.path.join(self.data_path, 'gene2go_all.pkl'), 'rb') as f:
-            gene2go = pickle.load(f)
-        
-        if gene_set_path is not None:
-            # If gene set specified for GO graph, use that
-            gene_set_path = gene_set_path
-            self.default_GO_graph = False
+            self.gene2go = pickle.load(f)
+    
+    def set_pert_genes(self):
+        """
+        Set the list of genes that can be perturbed and are to be included in 
+        perturbation graph
+        """
+        
+        if self.gene_set_path is not None:
+            # If gene set specified for perturbation graph, use that
+            path_ = self.gene_set_path
+            self.default_pert_graph = False
+            with open(path_, 'rb') as f:
+                essential_genes = pickle.load(f)
+            
+        elif self.default_pert_graph is False:
+            # Use a smaller perturbation graph 
+            all_pert_genes = get_genes_from_perts(self.adata.obs['condition'])
+            essential_genes = list(self.adata.var['gene_name'].values)
+            essential_genes += all_pert_genes
+            
         else:
-            # Otherwise, use a large set of genes to create GO
+            # Otherwise, use a large set of genes to create perturbation graph
             server_path = 'https://dataverse.harvard.edu/api/access/datafile/6934320'
-            gene_set_path = os.path.join(self.data_path,
+            path_ = os.path.join(self.data_path,
                                      'essential_all_data_pert_genes.pkl')
-            dataverse_download(server_path, gene_set_path)
-        with open(gene_set_path, 'rb') as f:
-            essential_genes = pickle.load(f)
+            dataverse_download(server_path, path_)
+            with open(path_, 'rb') as f:
+                essential_genes = pickle.load(f)
     
-        gene2go = {i: gene2go[i] for i in essential_genes if i in gene2go}
+        gene2go = {i: self.gene2go[i] for i in essential_genes if i in self.gene2go}
 
         self.pert_names = np.unique(list(gene2go.keys()))
         self.node_map_pert = {x: it for it, x in enumerate(self.pert_names)}
             
     def load(self, data_name = None, data_path = None):
+        """
+        Load existing dataloader
+        Use data_name for loading 'norman', 'adamson', 'dixit' datasets
+        For other datasets use data_path
+        """
+        
         if data_name in ['norman', 'adamson', 'dixit']:
             ## load from harvard dataverse
             if data_name == 'norman':
                 url = 'https://dataverse.harvard.edu/api/access/datafile/6154020'
             elif data_name == 'adamson':
                 url = 'https://dataverse.harvard.edu/api/access/datafile/6154417'
             elif data_name == 'dixit':
@@ -84,14 +109,15 @@
             self.adata = sc.read_h5ad(adata_path)
             self.dataset_name = data_path.split('/')[-1]
             self.dataset_path = data_path
         else:
             raise ValueError("data attribute is either Norman/Adamson/Dixit "
                              "or a path to an h5ad file")
         
+        self.set_pert_genes()
         print_sys('These perturbations are not in the GO graph and their '
                   'perturbation can thus not be predicted')
         not_in_go_pert = np.array(self.adata.obs[
                                   self.adata.obs.condition.apply(
                                   lambda x:not filter_pert_in_go(x,
                                         self.pert_names))].condition.unique())
         print_sys(not_in_go_pert)
@@ -138,14 +164,15 @@
             os.mkdir(save_data_folder)
         self.dataset_path = save_data_folder
         self.adata = get_DE_genes(adata, skip_calc_de)
         if not skip_calc_de:
             self.adata = get_dropout_non_zero_genes(self.adata)
         self.adata.write_h5ad(os.path.join(save_data_folder, 'perturb_processed.h5ad'))
         
+        self.set_pert_genes()
         self.ctrl_adata = self.adata[self.adata.obs['condition'] == 'ctrl']
         self.gene_names = self.adata.var.gene_name
         pyg_path = os.path.join(save_data_folder, 'data_pyg')
         if not os.path.exists(pyg_path):
             os.mkdir(pyg_path)
         dataset_fname = os.path.join(pyg_path, 'cell_graphs.pkl')
         print_sys("Creating pyg object for each cell in the data...")
```

### Comparing `cell-gears-0.0.3/gears/utils.py` & `cell-gears-0.0.4/gears/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -216,23 +216,23 @@
         print('Saving edge_list to file')
         df_edge_list.to_csv(fname, index=False)
 
     return df_edge_list
 
 def get_similarity_network(network_type, adata, threshold, k,
                            data_path, data_name, split, seed, train_gene_set_size,
-                           set2conditions, default_GO_graph=True, pert_list=None):
+                           set2conditions, default_pert_graph=True, pert_list=None):
     
     if network_type == 'co-express':
         df_out = get_coexpression_network_from_train(adata, threshold, k,
                                                      data_path, data_name, split,
                                                      seed, train_gene_set_size,
                                                      set2conditions)
     elif network_type == 'go':
-        if default_GO_graph:
+        if default_pert_graph:
             server_path = 'https://dataverse.harvard.edu/api/access/datafile/6934319'
             tar_data_download_wrapper(server_path, 
                                      os.path.join(data_path, 'go_essential_all'),
                                      data_path)
             df_jaccard = pd.read_csv(os.path.join(data_path, 
                                      'go_essential_all/go_essential_all.csv'))
 
@@ -437,7 +437,19 @@
     
     return GI_genes_idx
 
 def get_mean_control(adata):
     cols = adata.var.gene_name.values.astype('str')
     mean_ctrl_exp = adata[adata.obs['condition'] == 'ctrl'].to_df().mean()
     return mean_ctrl_exp
+
+def get_genes_from_perts(perts):
+    """
+    Returns list of genes involved in a given perturbation list
+    """
+
+    if type(perts) is str:
+        perts = [perts]
+    gene_list = [p.split('+') for p in np.unique(perts)]
+    gene_list = [item for sublist in gene_list for item in sublist]
+    gene_list = [g for g in gene_list if g != 'ctrl']
+    return list(np.unique(gene_list))
```

### Comparing `cell-gears-0.0.3/gears/version.py` & `cell-gears-0.0.4/gears/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,8 +15,8 @@
 # X.YbN # Beta release
 # X.YrcN # Release Candidate
 # X.Y # Final release
 #
 # Dev branch marker is: 'X.Y.dev' or 'X.Y.devN' where N is an integer.
 # 'X.Y.dev0' is the canonical version of 'X.Y.dev'
 #
-__version__ = '0.0.3'  # pragma: no cover
+__version__ = '0.0.4'  # pragma: no cover
```

### Comparing `cell-gears-0.0.3/setup.py` & `cell-gears-0.0.4/setup.py`

 * *Files identical despite different names*

