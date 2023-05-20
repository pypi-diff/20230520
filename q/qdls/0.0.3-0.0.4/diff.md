# Comparing `tmp/qdls-0.0.3.tar.gz` & `tmp/qdls-0.0.4.tar.gz`

## Comparing `qdls-0.0.3.tar` & `qdls-0.0.4.tar`

### file list

```diff
@@ -1,50 +1,52 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.0.3/src/__init__.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 qdls-0.0.3/src/qdls/__init__.py
--rw-r--r--   0        0        0    11695 2020-02-02 00:00:00.000000 qdls-0.0.3/src/qdls/data.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 qdls-0.0.3/src/qdls/loggers.py
--rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 qdls-0.0.3/src/qdls/losses.py
--rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 qdls-0.0.3/src/qdls/metrics.py
--rw-r--r--   0        0        0    12975 2020-02-02 00:00:00.000000 qdls-0.0.3/src/qdls/object.py
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 qdls-0.0.3/src/qdls/optim.py
--rw-r--r--   0        0        0    13209 2020-02-02 00:00:00.000000 qdls-0.0.3/src/qdls/pretrains.py
--rw-r--r--   0        0        0     4282 2020-02-02 00:00:00.000000 qdls-0.0.3/src/qdls/tensor_ops.py
--rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 qdls-0.0.3/src/qdls/test.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 qdls-0.0.3/src/qdls/train.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.0.3/src/qdls/draw/__init__.py
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 qdls-0.0.3/src/qdls/draw/experiment.py
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 qdls-0.0.3/src/qdls/draw/stats.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 qdls-0.0.3/src/qdls/gql/__init__.py
--rw-r--r--   0        0        0     6940 2020-02-02 00:00:00.000000 qdls-0.0.3/src/qdls/gql/process_utils.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 qdls-0.0.3/src/qdls/gql/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.0.3/src/qdls/gql/cypher/__init__.py
--rw-r--r--   0        0        0    61918 2020-02-02 00:00:00.000000 qdls-0.0.3/src/qdls/gql/cypher/grammar/Cypher.interp
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 qdls-0.0.3/src/qdls/gql/cypher/grammar/Cypher.tokens
--rw-r--r--   0        0        0    61096 2020-02-02 00:00:00.000000 qdls-0.0.3/src/qdls/gql/cypher/grammar/CypherLexer.interp
--rw-r--r--   0        0        0    72699 2020-02-02 00:00:00.000000 qdls-0.0.3/src/qdls/gql/cypher/grammar/CypherLexer.py
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 qdls-0.0.3/src/qdls/gql/cypher/grammar/CypherLexer.tokens
--rw-r--r--   0        0        0    33891 2020-02-02 00:00:00.000000 qdls-0.0.3/src/qdls/gql/cypher/grammar/CypherListener.py
--rw-r--r--   0        0        0   413383 2020-02-02 00:00:00.000000 qdls-0.0.3/src/qdls/gql/cypher/grammar/CypherParser.py
--rw-r--r--   0        0        0    19984 2020-02-02 00:00:00.000000 qdls-0.0.3/src/qdls/gql/cypher/grammar/CypherVisitor.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.0.3/src/qdls/gql/cypher/grammar/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.0.3/src/qdls/gql/cypher/utils/__init__.py
--rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 qdls-0.0.3/src/qdls/gql/cypher/utils/execute.py
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 qdls-0.0.3/src/qdls/gql/cypher/utils/parse.py
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 qdls-0.0.3/src/qdls/gql/cypher/utils/syntax.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.0.3/src/qdls/gql/sparql/__init__.py
--rw-r--r--   0        0        0    57079 2020-02-02 00:00:00.000000 qdls-0.0.3/src/qdls/gql/sparql/grammar/Sparql.interp
--rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 qdls-0.0.3/src/qdls/gql/sparql/grammar/Sparql.tokens
--rw-r--r--   0        0        0    52018 2020-02-02 00:00:00.000000 qdls-0.0.3/src/qdls/gql/sparql/grammar/SparqlLexer.interp
--rw-r--r--   0        0        0    62363 2020-02-02 00:00:00.000000 qdls-0.0.3/src/qdls/gql/sparql/grammar/SparqlLexer.py
--rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 qdls-0.0.3/src/qdls/gql/sparql/grammar/SparqlLexer.tokens
--rw-r--r--   0        0        0    44193 2020-02-02 00:00:00.000000 qdls-0.0.3/src/qdls/gql/sparql/grammar/SparqlListener.py
--rw-r--r--   0        0        0   497844 2020-02-02 00:00:00.000000 qdls-0.0.3/src/qdls/gql/sparql/grammar/SparqlParser.py
--rw-r--r--   0        0        0    26235 2020-02-02 00:00:00.000000 qdls-0.0.3/src/qdls/gql/sparql/grammar/SparqlVisitor.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.0.3/src/qdls/gql/sparql/grammar/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.0.3/src/qdls/gql/sparql/utils/__init__.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 qdls-0.0.3/src/qdls/gql/sparql/utils/parse.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.0.3/test/test_draw.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 qdls-0.0.3/.gitignore
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 qdls-0.0.3/LICENSE
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 qdls-0.0.3/README.md
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 qdls-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 qdls-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 qdls-0.0.4/build_upload.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.0.4/src/__init__.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 qdls-0.0.4/src/qdls/__init__.py
+-rw-r--r--   0        0        0    11695 2020-02-02 00:00:00.000000 qdls-0.0.4/src/qdls/data.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 qdls-0.0.4/src/qdls/loggers.py
+-rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 qdls-0.0.4/src/qdls/losses.py
+-rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 qdls-0.0.4/src/qdls/metrics.py
+-rw-r--r--   0        0        0    13203 2020-02-02 00:00:00.000000 qdls-0.0.4/src/qdls/object.py
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 qdls-0.0.4/src/qdls/optim.py
+-rw-r--r--   0        0        0    13611 2020-02-02 00:00:00.000000 qdls-0.0.4/src/qdls/pretrains.py
+-rw-r--r--   0        0        0     4282 2020-02-02 00:00:00.000000 qdls-0.0.4/src/qdls/tensor_ops.py
+-rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 qdls-0.0.4/src/qdls/test.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 qdls-0.0.4/src/qdls/train.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.0.4/src/qdls/draw/__init__.py
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 qdls-0.0.4/src/qdls/draw/experiment.py
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 qdls-0.0.4/src/qdls/draw/stats.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 qdls-0.0.4/src/qdls/gql/__init__.py
+-rw-r--r--   0        0        0     6940 2020-02-02 00:00:00.000000 qdls-0.0.4/src/qdls/gql/process_utils.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 qdls-0.0.4/src/qdls/gql/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.0.4/src/qdls/gql/cypher/__init__.py
+-rw-r--r--   0        0        0    61918 2020-02-02 00:00:00.000000 qdls-0.0.4/src/qdls/gql/cypher/grammar/Cypher.interp
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 qdls-0.0.4/src/qdls/gql/cypher/grammar/Cypher.tokens
+-rw-r--r--   0        0        0    61096 2020-02-02 00:00:00.000000 qdls-0.0.4/src/qdls/gql/cypher/grammar/CypherLexer.interp
+-rw-r--r--   0        0        0    72699 2020-02-02 00:00:00.000000 qdls-0.0.4/src/qdls/gql/cypher/grammar/CypherLexer.py
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 qdls-0.0.4/src/qdls/gql/cypher/grammar/CypherLexer.tokens
+-rw-r--r--   0        0        0    33891 2020-02-02 00:00:00.000000 qdls-0.0.4/src/qdls/gql/cypher/grammar/CypherListener.py
+-rw-r--r--   0        0        0   413383 2020-02-02 00:00:00.000000 qdls-0.0.4/src/qdls/gql/cypher/grammar/CypherParser.py
+-rw-r--r--   0        0        0    19984 2020-02-02 00:00:00.000000 qdls-0.0.4/src/qdls/gql/cypher/grammar/CypherVisitor.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.0.4/src/qdls/gql/cypher/grammar/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.0.4/src/qdls/gql/cypher/utils/__init__.py
+-rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 qdls-0.0.4/src/qdls/gql/cypher/utils/execute.py
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 qdls-0.0.4/src/qdls/gql/cypher/utils/parse.py
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 qdls-0.0.4/src/qdls/gql/cypher/utils/syntax.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.0.4/src/qdls/gql/sparql/__init__.py
+-rw-r--r--   0        0        0    57079 2020-02-02 00:00:00.000000 qdls-0.0.4/src/qdls/gql/sparql/grammar/Sparql.interp
+-rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 qdls-0.0.4/src/qdls/gql/sparql/grammar/Sparql.tokens
+-rw-r--r--   0        0        0    52018 2020-02-02 00:00:00.000000 qdls-0.0.4/src/qdls/gql/sparql/grammar/SparqlLexer.interp
+-rw-r--r--   0        0        0    62363 2020-02-02 00:00:00.000000 qdls-0.0.4/src/qdls/gql/sparql/grammar/SparqlLexer.py
+-rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 qdls-0.0.4/src/qdls/gql/sparql/grammar/SparqlLexer.tokens
+-rw-r--r--   0        0        0    44193 2020-02-02 00:00:00.000000 qdls-0.0.4/src/qdls/gql/sparql/grammar/SparqlListener.py
+-rw-r--r--   0        0        0   497844 2020-02-02 00:00:00.000000 qdls-0.0.4/src/qdls/gql/sparql/grammar/SparqlParser.py
+-rw-r--r--   0        0        0    26235 2020-02-02 00:00:00.000000 qdls-0.0.4/src/qdls/gql/sparql/grammar/SparqlVisitor.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.0.4/src/qdls/gql/sparql/grammar/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.0.4/src/qdls/gql/sparql/utils/__init__.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 qdls-0.0.4/src/qdls/gql/sparql/utils/parse.py
+-rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 qdls-0.0.4/src/qdls/gql/sparql/utils/syntax.py
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 qdls-0.0.4/test/test_draw.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 qdls-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 qdls-0.0.4/LICENSE
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 qdls-0.0.4/README.md
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 qdls-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 qdls-0.0.4/PKG-INFO
```

### Comparing `qdls-0.0.3/src/qdls/data.py` & `qdls-0.0.4/src/qdls/data.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.3/src/qdls/loggers.py` & `qdls-0.0.4/src/qdls/loggers.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.3/src/qdls/losses.py` & `qdls-0.0.4/src/qdls/losses.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.3/src/qdls/metrics.py` & `qdls-0.0.4/src/qdls/metrics.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.3/src/qdls/object.py` & `qdls-0.0.4/src/qdls/object.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import sys
 import json
 import yaml
 import argparse
 from  argparse import Namespace
+import omegaconf
 from omegaconf import OmegaConf as oc
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 import pytorch_lightning as pl
 import multiprocessing
@@ -293,15 +294,20 @@
     """ 两边是==，输入字符串居中，两边各有5个空格，输出字体颜色为黄色 """
     print(Fore.YELLOW,"="*25 + string.center(len(string)+10,) + "="*25)
     print(Style.RESET_ALL)
 
 def print_config(config):
     """ 打印字典，config等， 字体颜色为绿色 """
     print("="*80)
-    print(Fore.GREEN, config)
+    if type(config) is omegaconf.dictconfig.DictConfig:
+        config_dict = oc.to_object(config)
+    else:
+        config_dict = namespace2dict(config)
+    s = json.dumps(config_dict, ensure_ascii=False, indent=2)
+    print(Fore.GREEN, s)
     print(Style.RESET_ALL)
     print("="*80)
 
 def resume_config(config, path):
     """ 
     pytorch lightning save_hyperparameters() 保存的yaml文件 在预测的时候需要更新
     从原先保存的yaml恢复，重写新的 mode max_epochs, data and preds
```

### Comparing `qdls-0.0.3/src/qdls/optim.py` & `qdls-0.0.4/src/qdls/optim.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.3/src/qdls/tensor_ops.py` & `qdls-0.0.4/src/qdls/tensor_ops.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.3/src/qdls/test.py` & `qdls-0.0.4/src/qdls/test.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.3/src/qdls/draw/experiment.py` & `qdls-0.0.4/src/qdls/draw/experiment.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.3/src/qdls/draw/stats.py` & `qdls-0.0.4/src/qdls/draw/stats.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.3/src/qdls/gql/process_utils.py` & `qdls-0.0.4/src/qdls/gql/process_utils.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.3/src/qdls/gql/utils.py` & `qdls-0.0.4/src/qdls/gql/utils.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.3/src/qdls/gql/cypher/grammar/Cypher.interp` & `qdls-0.0.4/src/qdls/gql/cypher/grammar/Cypher.interp`

 * *Files identical despite different names*

### Comparing `qdls-0.0.3/src/qdls/gql/cypher/grammar/Cypher.tokens` & `qdls-0.0.4/src/qdls/gql/cypher/grammar/Cypher.tokens`

 * *Files identical despite different names*

### Comparing `qdls-0.0.3/src/qdls/gql/cypher/grammar/CypherLexer.interp` & `qdls-0.0.4/src/qdls/gql/cypher/grammar/CypherLexer.interp`

 * *Files identical despite different names*

### Comparing `qdls-0.0.3/src/qdls/gql/cypher/grammar/CypherLexer.py` & `qdls-0.0.4/src/qdls/gql/cypher/grammar/CypherLexer.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.3/src/qdls/gql/cypher/grammar/CypherLexer.tokens` & `qdls-0.0.4/src/qdls/gql/cypher/grammar/CypherLexer.tokens`

 * *Files identical despite different names*

### Comparing `qdls-0.0.3/src/qdls/gql/cypher/grammar/CypherListener.py` & `qdls-0.0.4/src/qdls/gql/cypher/grammar/CypherListener.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.3/src/qdls/gql/cypher/grammar/CypherParser.py` & `qdls-0.0.4/src/qdls/gql/cypher/grammar/CypherParser.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.3/src/qdls/gql/cypher/grammar/CypherVisitor.py` & `qdls-0.0.4/src/qdls/gql/cypher/grammar/CypherVisitor.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.3/src/qdls/gql/cypher/utils/execute.py` & `qdls-0.0.4/src/qdls/gql/cypher/utils/execute.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.3/src/qdls/gql/cypher/utils/parse.py` & `qdls-0.0.4/src/qdls/gql/cypher/utils/parse.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.3/src/qdls/gql/cypher/utils/syntax.py` & `qdls-0.0.4/src/qdls/gql/cypher/utils/syntax.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.3/src/qdls/gql/sparql/grammar/Sparql.interp` & `qdls-0.0.4/src/qdls/gql/sparql/grammar/Sparql.interp`

 * *Files identical despite different names*

### Comparing `qdls-0.0.3/src/qdls/gql/sparql/grammar/Sparql.tokens` & `qdls-0.0.4/src/qdls/gql/sparql/grammar/Sparql.tokens`

 * *Files identical despite different names*

### Comparing `qdls-0.0.3/src/qdls/gql/sparql/grammar/SparqlLexer.interp` & `qdls-0.0.4/src/qdls/gql/sparql/grammar/SparqlLexer.interp`

 * *Files identical despite different names*

### Comparing `qdls-0.0.3/src/qdls/gql/sparql/grammar/SparqlLexer.py` & `qdls-0.0.4/src/qdls/gql/sparql/grammar/SparqlLexer.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.3/src/qdls/gql/sparql/grammar/SparqlLexer.tokens` & `qdls-0.0.4/src/qdls/gql/sparql/grammar/SparqlLexer.tokens`

 * *Files identical despite different names*

### Comparing `qdls-0.0.3/src/qdls/gql/sparql/grammar/SparqlListener.py` & `qdls-0.0.4/src/qdls/gql/sparql/grammar/SparqlListener.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.3/src/qdls/gql/sparql/grammar/SparqlParser.py` & `qdls-0.0.4/src/qdls/gql/sparql/grammar/SparqlParser.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.3/src/qdls/gql/sparql/grammar/SparqlVisitor.py` & `qdls-0.0.4/src/qdls/gql/sparql/grammar/SparqlVisitor.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.3/src/qdls/gql/sparql/utils/parse.py` & `qdls-0.0.4/src/qdls/gql/sparql/utils/parse.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.3/.gitignore` & `qdls-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `qdls-0.0.3/LICENSE` & `qdls-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qdls-0.0.3/pyproject.toml` & `qdls-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "qdls"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Qing25", email="aqsz2526@outlook.com" },
 ]
 description = "Q-Deep Learning Snippets, my working code snippets"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `qdls-0.0.3/PKG-INFO` & `qdls-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qdls
-Version: 0.0.3
+Version: 0.0.4
 Summary: Q-Deep Learning Snippets, my working code snippets
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Qing25 <aqsz2526@outlook.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

