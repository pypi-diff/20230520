# Comparing `tmp/mlflow_aws_rds_iam-0.1.0.tar.gz` & `tmp/mlflow_aws_rds_iam-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlflow_aws_rds_iam-0.1.0.tar", max compression
+gzip compressed data, was "mlflow_aws_rds_iam-0.2.0.tar", max compression
```

## Comparing `mlflow_aws_rds_iam-0.1.0.tar` & `mlflow_aws_rds_iam-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1085 2023-05-16 13:54:43.184482 mlflow_aws_rds_iam-0.1.0/LICENSE.md
--rw-r--r--   0        0        0     1434 2023-05-16 13:54:43.184482 mlflow_aws_rds_iam-0.1.0/README.md
--rw-r--r--   0        0        0       76 2023-05-16 13:54:43.184482 mlflow_aws_rds_iam-0.1.0/mlflow_aws_rds_iam/__init__.py
--rw-r--r--   0        0        0   174184 2023-05-16 13:54:43.185482 mlflow_aws_rds_iam-0.1.0/mlflow_aws_rds_iam/certs/global-bundle.pem
--rw-r--r--   0        0        0      947 2023-05-16 13:54:43.186483 mlflow_aws_rds_iam-0.1.0/mlflow_aws_rds_iam/listeners.py
--rw-r--r--   0        0        0     2422 2023-05-16 13:54:43.186483 mlflow_aws_rds_iam-0.1.0/mlflow_aws_rds_iam/model_registry.py
--rw-r--r--   0        0        0      808 2023-05-16 13:54:43.186483 mlflow_aws_rds_iam-0.1.0/mlflow_aws_rds_iam/ssl.py
--rw-r--r--   0        0        0     2566 2023-05-16 13:54:43.186483 mlflow_aws_rds_iam-0.1.0/mlflow_aws_rds_iam/tracking.py
--rw-r--r--   0        0        0      537 2023-05-16 13:54:43.186483 mlflow_aws_rds_iam-0.1.0/mlflow_aws_rds_iam/utils.py
--rw-r--r--   0        0        0     1530 2023-05-16 13:54:43.187483 mlflow_aws_rds_iam-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2438 1970-01-01 00:00:00.000000 mlflow_aws_rds_iam-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-05-20 10:38:40.387615 mlflow_aws_rds_iam-0.2.0/LICENSE.md
+-rw-r--r--   0        0        0     1555 2023-05-20 10:38:40.387615 mlflow_aws_rds_iam-0.2.0/README.md
+-rw-r--r--   0        0        0      227 2023-05-20 10:38:40.387615 mlflow_aws_rds_iam-0.2.0/mlflow_aws_rds_iam/__init__.py
+-rw-r--r--   0        0        0   174184 2023-05-20 10:38:40.388615 mlflow_aws_rds_iam-0.2.0/mlflow_aws_rds_iam/certs/global-bundle.pem
+-rw-r--r--   0        0        0      947 2023-05-20 10:38:40.388615 mlflow_aws_rds_iam-0.2.0/mlflow_aws_rds_iam/listeners.py
+-rw-r--r--   0        0        0     2441 2023-05-20 10:38:40.388615 mlflow_aws_rds_iam-0.2.0/mlflow_aws_rds_iam/model_registry.py
+-rw-r--r--   0        0        0      808 2023-05-20 10:38:40.388615 mlflow_aws_rds_iam-0.2.0/mlflow_aws_rds_iam/ssl.py
+-rw-r--r--   0        0        0     2585 2023-05-20 10:38:40.388615 mlflow_aws_rds_iam-0.2.0/mlflow_aws_rds_iam/tracking.py
+-rw-r--r--   0        0        0      537 2023-05-20 10:38:40.388615 mlflow_aws_rds_iam-0.2.0/mlflow_aws_rds_iam/utils.py
+-rw-r--r--   0        0        0     1548 2023-05-20 10:38:40.389615 mlflow_aws_rds_iam-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2457 1970-01-01 00:00:00.000000 mlflow_aws_rds_iam-0.2.0/PKG-INFO
```

### Comparing `mlflow_aws_rds_iam-0.1.0/LICENSE.md` & `mlflow_aws_rds_iam-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mlflow_aws_rds_iam-0.1.0/README.md` & `mlflow_aws_rds_iam-0.2.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -37,14 +37,16 @@
 
 If a *password* is provided in the database URI, AWS IAM authentication will be skipped, *effectively disabling the plugins*.
 
 *Credentials* are required in order to use AWS IAM authentication. Refer to [Boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/credentials.html) for configuration instructions.
 
 *SSL connection to the database is enabled by default*, but can be disabled with the environment variable `MLFLOW_DISABLE_DB_SSL=true`.
 
+Debug log of the plugins and underlying libraries (boto3, urllib3) can be enabled with `MLFLOW_AWS_RDS_IAM_DEBUG=true`.
+
 
 License
 -------
 
 This project is licensed under the terms of the MIT license.
```

### Comparing `mlflow_aws_rds_iam-0.1.0/mlflow_aws_rds_iam/certs/global-bundle.pem` & `mlflow_aws_rds_iam-0.2.0/mlflow_aws_rds_iam/certs/global-bundle.pem`

 * *Files identical despite different names*

### Comparing `mlflow_aws_rds_iam-0.1.0/mlflow_aws_rds_iam/listeners.py` & `mlflow_aws_rds_iam-0.2.0/mlflow_aws_rds_iam/listeners.py`

 * *Files identical despite different names*

### Comparing `mlflow_aws_rds_iam-0.1.0/mlflow_aws_rds_iam/model_registry.py` & `mlflow_aws_rds_iam-0.2.0/mlflow_aws_rds_iam/model_registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from .ssl import IS_SSL_DISABLED_ENV_VAR, set_ssl_params
 from .utils import DatabaseType, get_db_default_port, get_db_type
 
 logger = logging.getLogger(__name__)
 
 
 class RDSIAMStore(SqlAlchemyStore):  # type: ignore[misc]
+    engine = None
+
     def __init__(self, store_uri: str):
         logger.debug("Using MLflow RDS IAM auth model registry store plugin.")
 
         db_uri = make_url(store_uri)
 
         if not get_db_type(db_uri) in DatabaseType:
             raise ValueError(
```

### Comparing `mlflow_aws_rds_iam-0.1.0/mlflow_aws_rds_iam/ssl.py` & `mlflow_aws_rds_iam-0.2.0/mlflow_aws_rds_iam/ssl.py`

 * *Files identical despite different names*

### Comparing `mlflow_aws_rds_iam-0.1.0/mlflow_aws_rds_iam/tracking.py` & `mlflow_aws_rds_iam-0.2.0/mlflow_aws_rds_iam/tracking.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from .ssl import IS_SSL_DISABLED_ENV_VAR, set_ssl_params
 from .utils import DatabaseType, get_db_default_port, get_db_type
 
 logger = logging.getLogger(__name__)
 
 
 class RDSIAMStore(SqlAlchemyStore):  # type: ignore[misc]
+    engine = None
+
     def __init__(self, store_uri: str, artifact_uri: str):
         logger.debug("Using MLflow RDS IAM auth tracking store plugin.")
 
         db_uri = make_url(store_uri)
 
         if not get_db_type(db_uri) in DatabaseType:
             raise ValueError(
```

### Comparing `mlflow_aws_rds_iam-0.1.0/mlflow_aws_rds_iam/utils.py` & `mlflow_aws_rds_iam-0.2.0/mlflow_aws_rds_iam/utils.py`

 * *Files identical despite different names*

### Comparing `mlflow_aws_rds_iam-0.1.0/pyproject.toml` & `mlflow_aws_rds_iam-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mlflow-aws-rds-iam"
-version = "0.1.0"
+version = "0.2.0"
 description = "MLflow plugins adding AWS RDS IAM auth for tracking and model registry stores"
 authors = ["Loris Zinsou <lzinsou@protonmail.com>"]
 readme = "README.md"
 keywords = ["mlflow", "plugin", "mlops", "aws", "rds", "iam", "postgresql", "mysql"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: Plugins",
@@ -36,14 +36,15 @@
 pytest = "^7.3.1"
 
 [tool.isort]
 profile = "black"
 
 [tool.mypy]
 strict = true
+exclude = "tests"
 
 [[tool.mypy.overrides]]
 module = "mlflow.store.model_registry.sqlalchemy_store"
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
 module = "mlflow.store.tracking.sqlalchemy_store"
```

### Comparing `mlflow_aws_rds_iam-0.1.0/PKG-INFO` & `mlflow_aws_rds_iam-0.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: mlflow-aws-rds-iam
-Version: 0.1.0
+Version: 0.2.0
 Summary: MLflow plugins adding AWS RDS IAM auth for tracking and model registry stores
 Home-page: https://gitlab.com/lzinsou/mlflow-aws-rds-iam
 Keywords: mlflow,plugin,mlops,aws,rds,iam,postgresql,mysql
 Author: Loris Zinsou
 Author-email: lzinsou@protonmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Plugins
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: StrEnum (>=0.4) ; python_version < "3.11"
 Requires-Dist: boto3 (>=1.26.134,<2)
 Requires-Dist: boto3-stubs[rds] (>=1.26.134,<2)
 Requires-Dist: mlflow (>=2,<3)
 Requires-Dist: sqlalchemy (>=2,<3)
 Project-URL: Repository, https://gitlab.com/lzinsou/mlflow-aws-rds-iam
 Description-Content-Type: text/markdown
@@ -61,14 +59,16 @@
 
 If a *password* is provided in the database URI, AWS IAM authentication will be skipped, *effectively disabling the plugins*.
 
 *Credentials* are required in order to use AWS IAM authentication. Refer to [Boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/credentials.html) for configuration instructions.
 
 *SSL connection to the database is enabled by default*, but can be disabled with the environment variable `MLFLOW_DISABLE_DB_SSL=true`.
 
+Debug log of the plugins and underlying libraries (boto3, urllib3) can be enabled with `MLFLOW_AWS_RDS_IAM_DEBUG=true`.
+
 
 License
 -------
 
 This project is licensed under the terms of the MIT license.
```

