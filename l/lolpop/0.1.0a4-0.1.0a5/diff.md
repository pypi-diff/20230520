# Comparing `tmp/lolpop-0.1.0a4.tar.gz` & `tmp/lolpop-0.1.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lolpop-0.1.0a4.tar", max compression
+gzip compressed data, was "lolpop-0.1.0a5.tar", max compression
```

## Comparing `lolpop-0.1.0a4.tar` & `lolpop-0.1.0a5.tar`

### file list

```diff
@@ -1,157 +1,157 @@
--rw-r--r--   0        0        0    11357 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/LICENSE
--rw-r--r--   0        0        0      220 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/__init__.py
--rw-r--r--   0        0        0        0 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/cli/__init__.py
--rw-r--r--   0        0        0     2552 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/cli/cli.py
--rw-r--r--   0        0        0    12841 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/cli/create.py
--rw-r--r--   0        0        0     3464 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/cli/datagen.py
--rw-r--r--   0        0        0      432 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/cli/package.py
--rw-r--r--   0        0        0     1928 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/cli/run.py
--rw-r--r--   0        0        0     2037 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/cli/seed.py
--rw-r--r--   0        0        0      451 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/cli/test.py
--rw-r--r--   0        0        0     1311 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/__init__.py
--rw-r--r--   0        0        0     3652 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/base_component.py
--rw-r--r--   0        0        0        0 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_checker/__init__.py
--rw-r--r--   0        0        0      164 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_checker/base_data_checker.py
--rw-r--r--   0        0        0     2160 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_checker/deepchecks_data_checker.py
--rw-r--r--   0        0        0     1813 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_checker/evidentlyai_data_checker.py
--rw-r--r--   0        0        0        0 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_connector/__init__.py
--rw-r--r--   0        0        0      233 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_connector/base_data_connector.py
--rw-r--r--   0        0        0     6265 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_connector/bigquery_data_connector.py
--rw-r--r--   0        0        0     5431 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_connector/databricks_sql_data_connector.py
--rw-r--r--   0        0        0     4122 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_connector/duckdb_data_connector.py
--rw-r--r--   0        0        0     4275 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_connector/gcs_data_connector.py
--rw-r--r--   0        0        0     1299 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_connector/local_data_connector.py
--rw-r--r--   0        0        0     5453 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_connector/postgres_data_connector.py
--rw-r--r--   0        0        0      637 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_connector/redshift_data_connector.py
--rw-r--r--   0        0        0     3352 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_connector/s3_data_connector.py
--rw-r--r--   0        0        0     6484 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_connector/snowflake_data_connector.py
--rw-r--r--   0        0        0        0 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_profiler/__init__.py
--rw-r--r--   0        0        0      243 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_profiler/base_data_profiler.py
--rw-r--r--   0        0        0     1462 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_profiler/continual_data_profiler.py
--rw-r--r--   0        0        0     2314 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_profiler/evidentlyai_data_profiler.py
--rw-r--r--   0        0        0     2162 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_profiler/sweetviz_data_profiler.py
--rw-r--r--   0        0        0     1912 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_profiler/ydata_profiling_data_profiler.py
--rw-r--r--   0        0        0        0 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_splitter/__init__.py
--rw-r--r--   0        0        0      163 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_splitter/base_data_splitter.py
--rw-r--r--   0        0        0     8542 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_splitter/local_data_splitter.py
--rw-r--r--   0        0        0        0 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_synthesizer/__init__.py
--rw-r--r--   0        0        0      396 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_synthesizer/base_data_synthesizer.py
--rw-r--r--   0        0        0     5878 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_synthesizer/svd_data_synthesizer.py
--rw-r--r--   0        0        0        0 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_transformer/__init__.py
--rw-r--r--   0        0        0      301 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_transformer/base_data_transformer.py
--rw-r--r--   0        0        0      712 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_transformer/bigquery_data_transformer.py
--rw-r--r--   0        0        0      870 2023-05-17 13:45:13.744955 lolpop-0.1.0a4/lolpop/component/data_transformer/databricks_sql_data_transformer.py
--rw-r--r--   0        0        0     4525 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/data_transformer/dbt_data_transformer.py
--rw-r--r--   0        0        0      613 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/data_transformer/duckdb_data_transformer.py
--rw-r--r--   0        0        0     2086 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/data_transformer/local_data_transformer.py
--rw-r--r--   0        0        0      838 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/data_transformer/postrgres_data_transformer.py
--rw-r--r--   0        0        0      962 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/data_transformer/redshift_data_transformer.py
--rw-r--r--   0        0        0      855 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/data_transformer/snowflake_data_transformer.py
--rw-r--r--   0        0        0        0 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/genai_chatbot/__init__.py
--rw-r--r--   0        0        0      228 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/genai_chatbot/base_genai_chatbot.py
--rw-r--r--   0        0        0      940 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/genai_chatbot/openai_chatbot.py
--rw-r--r--   0        0        0        0 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/hyperparameter_tuner/__init__.py
--rw-r--r--   0        0        0     2346 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/hyperparameter_tuner/base_hyperparameter_tuner.py
--rw-r--r--   0        0        0     2755 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/hyperparameter_tuner/local_hyperparameter_tuner.py
--rw-r--r--   0        0        0     9180 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/hyperparameter_tuner/optuna_hyperparameter_tuner.py
--rw-r--r--   0        0        0        0 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/logger/__init__.py
--rw-r--r--   0        0        0      139 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/logger/base_logger.py
--rw-r--r--   0        0        0     1699 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/logger/file_logger.py
--rw-r--r--   0        0        0     2017 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/logger/stdout_logger.py
--rw-r--r--   0        0        0        0 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/metadata_tracker/__init__.py
--rw-r--r--   0        0        0     2073 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/metadata_tracker/base_metadata_tracker.py
--rw-r--r--   0        0        0    15598 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/metadata_tracker/continual_metadata_tracker.py
--rw-r--r--   0        0        0    12376 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/metadata_tracker/mlflow_metadata_tracker.py
--rw-r--r--   0        0        0        0 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/metrics_tracker/__init__.py
--rw-r--r--   0        0        0      229 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/metrics_tracker/base_metrics_tracker.py
--rw-r--r--   0        0        0     5843 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/metrics_tracker/continual_metrics_tracker.py
--rw-r--r--   0        0        0     4804 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/metrics_tracker/mlflow_metrics_tracker.py
--rw-r--r--   0        0        0        0 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/model_bias_checker/__init__.py
--rw-r--r--   0        0        0     3960 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/model_bias_checker/aifairness_model_bias_checker.py
--rw-r--r--   0        0        0      240 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/model_bias_checker/base_model_bias_checker.py
--rw-r--r--   0        0        0        0 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/model_checker/__init__.py
--rw-r--r--   0        0        0     5574 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/model_checker/base_model_checker.py
--rw-r--r--   0        0        0     2848 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/model_checker/deepchecks_model_checker.py
--rw-r--r--   0        0        0     3408 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/model_checker/evidentlyai_model_checker.py
--rw-r--r--   0        0        0        0 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/model_deployer/__init__.py
--rw-r--r--   0        0        0      371 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/model_deployer/base_model_deployer.py
--rw-r--r--   0        0        0      574 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/model_deployer/seldon_model_deployer.py
--rw-r--r--   0        0        0        0 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/model_explainer/__init__.py
--rw-r--r--   0        0        0     8917 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/model_explainer/alibi_model_explainer.py
--rw-r--r--   0        0        0      244 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/model_explainer/base_model_explainer.py
--rw-r--r--   0        0        0        0 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/model_repository/__init__.py
--rw-r--r--   0        0        0      309 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/model_repository/base_model_repository.py
--rw-r--r--   0        0        0     2993 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/model_repository/continual_model_repository.py
--rw-r--r--   0        0        0     4521 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/model_repository/mlflow_model_repository.py
--rw-r--r--   0        0        0        0 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/model_trainer/__init__.py
--rw-r--r--   0        0        0     7234 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/model_trainer/base_model_trainer.py
--rw-r--r--   0        0        0     2407 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/model_trainer/xgboost_model_trainer.py
--rw-r--r--   0        0        0        0 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/model_visualizer/__init__.py
--rw-r--r--   0        0        0      169 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/model_visualizer/base_model_visualizer.py
--rw-r--r--   0        0        0     3881 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/model_visualizer/yellowbrick_model_visualizer.py
--rw-r--r--   0        0        0        0 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/notifier/__init__.py
--rw-r--r--   0        0        0      156 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/notifier/base_notifier.py
--rw-r--r--   0        0        0     2904 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/notifier/gmail_notifier.py
--rw-r--r--   0        0        0      880 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/notifier/slack_notifier.py
--rw-r--r--   0        0        0     1272 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/notifier/smtp_notifier.py
--rw-r--r--   0        0        0      322 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/notifier/stdout_notifier.py
--rw-r--r--   0        0        0        0 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/resource_version_control/__init__.py
--rw-r--r--   0        0        0      376 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/resource_version_control/base_resource_version_control.py
--rw-r--r--   0        0        0     3221 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/resource_version_control/continual_version_control.py
--rw-r--r--   0        0        0     5828 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/component/resource_version_control/dvc_version_control.py
--rw-r--r--   0        0        0     2346 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/extension/__init__.py
--rw-r--r--   0        0        0     1299 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/pipeline/__init__.py
--rw-r--r--   0        0        0     4626 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/pipeline/base_pipeline.py
--rw-r--r--   0        0        0        0 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/pipeline/deploy/__init__.py
--rw-r--r--   0        0        0      454 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/pipeline/deploy/base_deploy.py
--rw-r--r--   0        0        0     3849 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/pipeline/deploy/metaflow_offline_deploy.py
--rw-r--r--   0        0        0     1660 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/pipeline/deploy/offline_deploy.py
--rw-r--r--   0        0        0       42 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/pipeline/predict/__init__.py
--rw-r--r--   0        0        0      227 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/pipeline/predict/base_predict.py
--rw-r--r--   0        0        0     7182 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/pipeline/predict/metaflow_offline_predict.py
--rw-r--r--   0        0        0     4068 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/pipeline/predict/offline_predict.py
--rw-r--r--   0        0        0        0 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/pipeline/process/__init__.py
--rw-r--r--   0        0        0      452 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/pipeline/process/base_process.py
--rw-r--r--   0        0        0     5459 2023-05-17 13:45:13.748955 lolpop-0.1.0a4/lolpop/pipeline/process/metaflow_offline_process.py
--rw-r--r--   0        0        0     3267 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/pipeline/process/offline_process.py
--rw-r--r--   0        0        0        0 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/pipeline/train/__init__.py
--rw-r--r--   0        0        0      645 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/pipeline/train/base_train.py
--rw-r--r--   0        0        0     7474 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/pipeline/train/metaflow_offline_train.py
--rw-r--r--   0        0        0     4495 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/pipeline/train/offline_train.py
--rw-r--r--   0        0        0        0 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/pipeline/wrapper/__init__.py
--rw-r--r--   0        0        0      275 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/pipeline/wrapper/base_wrapper.py
--rw-r--r--   0        0        0      789 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/pipeline/wrapper/metaflow_pipeline_wrapper.py
--rw-r--r--   0        0        0     1285 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/runner/__init__.py
--rw-r--r--   0        0        0     6578 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/runner/base_runner.py
--rw-r--r--   0        0        0        0 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/runner/classification_runner/__init__.py
--rw-r--r--   0        0        0     7686 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/runner/classification_runner/classification_runner.py
--rw-r--r--   0        0        0     6130 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/runner/classification_runner/metaflow_classification.py
--rw-r--r--   0        0        0      175 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/templates/component_template/cookiecutter.json
--rw-r--r--   0        0        0        0 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/templates/component_template/{{cookiecutter.component_type}}/__init__.py
--rw-r--r--   0        0        0      802 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/templates/component_template/{{cookiecutter.component_type}}/base_{{cookiecutter.component_type}}.py
--rw-r--r--   0        0        0     1122 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/templates/component_template/{{cookiecutter.component_type}}/{{cookiecutter.component_class}}.py
--rw-r--r--   0        0        0      167 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/templates/pipeline_template/cookiecutter.json
--rw-r--r--   0        0        0        0 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/templates/pipeline_template/{{cookiecutter.pipeline_type}}/__init__.py
--rw-r--r--   0        0        0      803 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/templates/pipeline_template/{{cookiecutter.pipeline_type}}/base_{{cookiecutter.pipeline_type}}.py
--rw-r--r--   0        0        0     1096 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/templates/pipeline_template/{{cookiecutter.pipeline_type}}/{{cookiecutter.pipeline_class}}.py
--rw-r--r--   0        0        0       66 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/templates/project_template/cookiecutter.json
--rw-r--r--   0        0        0        0 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/templates/project_template/{{cookiecutter.project_name}}/Makefile
--rw-r--r--   0        0        0       32 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/templates/project_template/{{cookiecutter.project_name}}/README.md
--rw-r--r--   0        0        0        0 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/templates/project_template/{{cookiecutter.project_name}}/dvc.yaml
--rw-r--r--   0        0        0        0 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/__init__.py
--rw-r--r--   0        0        0     1418 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/component/__init__.py
--rw-r--r--   0        0        0     1408 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/pipeline/__init__.py
--rw-r--r--   0        0        0     1363 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/runner/__init__.py
--rw-r--r--   0        0        0        0 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop_project.yaml
--rw-r--r--   0        0        0      310 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/templates/project_template/{{cookiecutter.project_name}}/pyproject.toml
--rw-r--r--   0        0        0      151 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/templates/runner_template/cookiecutter.json
--rw-r--r--   0        0        0        0 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/templates/runner_template/{{cookiecutter.runner_type}}/__init__.py
--rw-r--r--   0        0        0      795 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/templates/runner_template/{{cookiecutter.runner_type}}/base_{{cookiecutter.runner_type}}.py
--rw-r--r--   0        0        0     1054 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/templates/runner_template/{{cookiecutter.runner_type}}/{{cookiecutter.runner_class}}.py
--rw-r--r--   0        0        0        0 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/utils/__init__.py
--rw-r--r--   0        0        0    15386 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/utils/common_utils.py
--rw-r--r--   0        0        0     1566 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/utils/continual_utils.py
--rw-r--r--   0        0        0     2452 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/utils/metaflow_utils.py
--rw-r--r--   0        0        0     3298 2023-05-17 13:45:13.752955 lolpop-0.1.0a4/lolpop/utils/mlflow_utils.py
--rw-r--r--   0        0        0     2261 2023-05-17 13:45:38.588891 lolpop-0.1.0a4/pyproject.toml
--rw-r--r--   0        0        0     2695 1970-01-01 00:00:00.000000 lolpop-0.1.0a4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-20 04:33:11.842488 lolpop-0.1.0a5/LICENSE
+-rw-r--r--   0        0        0      220 2023-05-20 04:33:11.842488 lolpop-0.1.0a5/lolpop/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-20 04:33:11.842488 lolpop-0.1.0a5/lolpop/cli/__init__.py
+-rw-r--r--   0        0        0     2552 2023-05-20 04:33:11.842488 lolpop-0.1.0a5/lolpop/cli/cli.py
+-rw-r--r--   0        0        0    12841 2023-05-20 04:33:11.842488 lolpop-0.1.0a5/lolpop/cli/create.py
+-rw-r--r--   0        0        0     3464 2023-05-20 04:33:11.842488 lolpop-0.1.0a5/lolpop/cli/datagen.py
+-rw-r--r--   0        0        0      432 2023-05-20 04:33:11.842488 lolpop-0.1.0a5/lolpop/cli/package.py
+-rw-r--r--   0        0        0     1928 2023-05-20 04:33:11.842488 lolpop-0.1.0a5/lolpop/cli/run.py
+-rw-r--r--   0        0        0     2037 2023-05-20 04:33:11.842488 lolpop-0.1.0a5/lolpop/cli/seed.py
+-rw-r--r--   0        0        0      451 2023-05-20 04:33:11.842488 lolpop-0.1.0a5/lolpop/cli/test.py
+-rw-r--r--   0        0        0     1311 2023-05-20 04:33:11.842488 lolpop-0.1.0a5/lolpop/component/__init__.py
+-rw-r--r--   0        0        0     3744 2023-05-20 04:33:11.842488 lolpop-0.1.0a5/lolpop/component/base_component.py
+-rw-r--r--   0        0        0        0 2023-05-20 04:33:11.842488 lolpop-0.1.0a5/lolpop/component/data_checker/__init__.py
+-rw-r--r--   0        0        0      164 2023-05-20 04:33:11.842488 lolpop-0.1.0a5/lolpop/component/data_checker/base_data_checker.py
+-rw-r--r--   0        0        0     2160 2023-05-20 04:33:11.842488 lolpop-0.1.0a5/lolpop/component/data_checker/deepchecks_data_checker.py
+-rw-r--r--   0        0        0     1813 2023-05-20 04:33:11.842488 lolpop-0.1.0a5/lolpop/component/data_checker/evidentlyai_data_checker.py
+-rw-r--r--   0        0        0        0 2023-05-20 04:33:11.842488 lolpop-0.1.0a5/lolpop/component/data_connector/__init__.py
+-rw-r--r--   0        0        0      233 2023-05-20 04:33:11.842488 lolpop-0.1.0a5/lolpop/component/data_connector/base_data_connector.py
+-rw-r--r--   0        0        0     6265 2023-05-20 04:33:11.842488 lolpop-0.1.0a5/lolpop/component/data_connector/bigquery_data_connector.py
+-rw-r--r--   0        0        0     5431 2023-05-20 04:33:11.842488 lolpop-0.1.0a5/lolpop/component/data_connector/databricks_sql_data_connector.py
+-rw-r--r--   0        0        0     4122 2023-05-20 04:33:11.842488 lolpop-0.1.0a5/lolpop/component/data_connector/duckdb_data_connector.py
+-rw-r--r--   0        0        0     4275 2023-05-20 04:33:11.842488 lolpop-0.1.0a5/lolpop/component/data_connector/gcs_data_connector.py
+-rw-r--r--   0        0        0     1299 2023-05-20 04:33:11.842488 lolpop-0.1.0a5/lolpop/component/data_connector/local_data_connector.py
+-rw-r--r--   0        0        0     5453 2023-05-20 04:33:11.842488 lolpop-0.1.0a5/lolpop/component/data_connector/postgres_data_connector.py
+-rw-r--r--   0        0        0      637 2023-05-20 04:33:11.842488 lolpop-0.1.0a5/lolpop/component/data_connector/redshift_data_connector.py
+-rw-r--r--   0        0        0     3352 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/data_connector/s3_data_connector.py
+-rw-r--r--   0        0        0     6484 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/data_connector/snowflake_data_connector.py
+-rw-r--r--   0        0        0        0 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/data_profiler/__init__.py
+-rw-r--r--   0        0        0      243 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/data_profiler/base_data_profiler.py
+-rw-r--r--   0        0        0     1462 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/data_profiler/continual_data_profiler.py
+-rw-r--r--   0        0        0     2314 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/data_profiler/evidentlyai_data_profiler.py
+-rw-r--r--   0        0        0     2162 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/data_profiler/sweetviz_data_profiler.py
+-rw-r--r--   0        0        0     1912 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/data_profiler/ydata_profiling_data_profiler.py
+-rw-r--r--   0        0        0        0 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/data_splitter/__init__.py
+-rw-r--r--   0        0        0      163 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/data_splitter/base_data_splitter.py
+-rw-r--r--   0        0        0     8542 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/data_splitter/local_data_splitter.py
+-rw-r--r--   0        0        0        0 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/data_synthesizer/__init__.py
+-rw-r--r--   0        0        0      396 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/data_synthesizer/base_data_synthesizer.py
+-rw-r--r--   0        0        0     5878 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/data_synthesizer/svd_data_synthesizer.py
+-rw-r--r--   0        0        0        0 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/data_transformer/__init__.py
+-rw-r--r--   0        0        0      301 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/data_transformer/base_data_transformer.py
+-rw-r--r--   0        0        0      712 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/data_transformer/bigquery_data_transformer.py
+-rw-r--r--   0        0        0      870 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/data_transformer/databricks_sql_data_transformer.py
+-rw-r--r--   0        0        0     4525 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/data_transformer/dbt_data_transformer.py
+-rw-r--r--   0        0        0      613 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/data_transformer/duckdb_data_transformer.py
+-rw-r--r--   0        0        0     2472 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/data_transformer/local_data_transformer.py
+-rw-r--r--   0        0        0      838 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/data_transformer/postrgres_data_transformer.py
+-rw-r--r--   0        0        0      962 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/data_transformer/redshift_data_transformer.py
+-rw-r--r--   0        0        0      855 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/data_transformer/snowflake_data_transformer.py
+-rw-r--r--   0        0        0        0 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/genai_chatbot/__init__.py
+-rw-r--r--   0        0        0      228 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/genai_chatbot/base_genai_chatbot.py
+-rw-r--r--   0        0        0      940 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/genai_chatbot/openai_chatbot.py
+-rw-r--r--   0        0        0        0 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/hyperparameter_tuner/__init__.py
+-rw-r--r--   0        0        0     2346 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/hyperparameter_tuner/base_hyperparameter_tuner.py
+-rw-r--r--   0        0        0     2755 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/hyperparameter_tuner/local_hyperparameter_tuner.py
+-rw-r--r--   0        0        0     9180 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/hyperparameter_tuner/optuna_hyperparameter_tuner.py
+-rw-r--r--   0        0        0        0 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/logger/__init__.py
+-rw-r--r--   0        0        0      139 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/logger/base_logger.py
+-rw-r--r--   0        0        0     1699 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/logger/file_logger.py
+-rw-r--r--   0        0        0     2017 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/logger/stdout_logger.py
+-rw-r--r--   0        0        0        0 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/metadata_tracker/__init__.py
+-rw-r--r--   0        0        0     2073 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/metadata_tracker/base_metadata_tracker.py
+-rw-r--r--   0        0        0    15598 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/metadata_tracker/continual_metadata_tracker.py
+-rw-r--r--   0        0        0    12388 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/metadata_tracker/mlflow_metadata_tracker.py
+-rw-r--r--   0        0        0        0 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/metrics_tracker/__init__.py
+-rw-r--r--   0        0        0      460 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/metrics_tracker/base_metrics_tracker.py
+-rw-r--r--   0        0        0     5843 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/metrics_tracker/continual_metrics_tracker.py
+-rw-r--r--   0        0        0     4804 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/metrics_tracker/mlflow_metrics_tracker.py
+-rw-r--r--   0        0        0        0 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/model_bias_checker/__init__.py
+-rw-r--r--   0        0        0     3960 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/model_bias_checker/aifairness_model_bias_checker.py
+-rw-r--r--   0        0        0      240 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/model_bias_checker/base_model_bias_checker.py
+-rw-r--r--   0        0        0        0 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/model_checker/__init__.py
+-rw-r--r--   0        0        0     5574 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/model_checker/base_model_checker.py
+-rw-r--r--   0        0        0     2848 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/model_checker/deepchecks_model_checker.py
+-rw-r--r--   0        0        0     3408 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/model_checker/evidentlyai_model_checker.py
+-rw-r--r--   0        0        0        0 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/model_deployer/__init__.py
+-rw-r--r--   0        0        0      371 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/model_deployer/base_model_deployer.py
+-rw-r--r--   0        0        0      574 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/model_deployer/seldon_model_deployer.py
+-rw-r--r--   0        0        0        0 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/model_explainer/__init__.py
+-rw-r--r--   0        0        0     8917 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/model_explainer/alibi_model_explainer.py
+-rw-r--r--   0        0        0      244 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/model_explainer/base_model_explainer.py
+-rw-r--r--   0        0        0        0 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/model_repository/__init__.py
+-rw-r--r--   0        0        0      309 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/model_repository/base_model_repository.py
+-rw-r--r--   0        0        0     2993 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/model_repository/continual_model_repository.py
+-rw-r--r--   0        0        0     4521 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/model_repository/mlflow_model_repository.py
+-rw-r--r--   0        0        0        0 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/model_trainer/__init__.py
+-rw-r--r--   0        0        0     7260 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/model_trainer/base_model_trainer.py
+-rw-r--r--   0        0        0     2407 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/model_trainer/xgboost_model_trainer.py
+-rw-r--r--   0        0        0        0 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/model_visualizer/__init__.py
+-rw-r--r--   0        0        0      169 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/model_visualizer/base_model_visualizer.py
+-rw-r--r--   0        0        0     3881 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/model_visualizer/yellowbrick_model_visualizer.py
+-rw-r--r--   0        0        0        0 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/notifier/__init__.py
+-rw-r--r--   0        0        0      156 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/notifier/base_notifier.py
+-rw-r--r--   0        0        0     2904 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/notifier/gmail_notifier.py
+-rw-r--r--   0        0        0      880 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/notifier/slack_notifier.py
+-rw-r--r--   0        0        0     1272 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/notifier/smtp_notifier.py
+-rw-r--r--   0        0        0      322 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/notifier/stdout_notifier.py
+-rw-r--r--   0        0        0        0 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/resource_version_control/__init__.py
+-rw-r--r--   0        0        0      376 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/resource_version_control/base_resource_version_control.py
+-rw-r--r--   0        0        0     3221 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/resource_version_control/continual_version_control.py
+-rw-r--r--   0        0        0     5828 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/component/resource_version_control/dvc_version_control.py
+-rw-r--r--   0        0        0     2346 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/extension/__init__.py
+-rw-r--r--   0        0        0     1299 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/pipeline/__init__.py
+-rw-r--r--   0        0        0     4967 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/pipeline/base_pipeline.py
+-rw-r--r--   0        0        0        0 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/pipeline/deploy/__init__.py
+-rw-r--r--   0        0        0      454 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/pipeline/deploy/base_deploy.py
+-rw-r--r--   0        0        0     3849 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/pipeline/deploy/metaflow_offline_deploy.py
+-rw-r--r--   0        0        0     1660 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/pipeline/deploy/offline_deploy.py
+-rw-r--r--   0        0        0       42 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/pipeline/predict/__init__.py
+-rw-r--r--   0        0        0      227 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/pipeline/predict/base_predict.py
+-rw-r--r--   0        0        0     7182 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/pipeline/predict/metaflow_offline_predict.py
+-rw-r--r--   0        0        0     4137 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/pipeline/predict/offline_predict.py
+-rw-r--r--   0        0        0        0 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/pipeline/process/__init__.py
+-rw-r--r--   0        0        0      452 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/pipeline/process/base_process.py
+-rw-r--r--   0        0        0     5459 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/pipeline/process/metaflow_offline_process.py
+-rw-r--r--   0        0        0     3267 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/pipeline/process/offline_process.py
+-rw-r--r--   0        0        0        0 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/pipeline/train/__init__.py
+-rw-r--r--   0        0        0      645 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/pipeline/train/base_train.py
+-rw-r--r--   0        0        0     7474 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/pipeline/train/metaflow_offline_train.py
+-rw-r--r--   0        0        0     4499 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/pipeline/train/offline_train.py
+-rw-r--r--   0        0        0        0 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/pipeline/wrapper/__init__.py
+-rw-r--r--   0        0        0      275 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/pipeline/wrapper/base_wrapper.py
+-rw-r--r--   0        0        0      789 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/pipeline/wrapper/metaflow_pipeline_wrapper.py
+-rw-r--r--   0        0        0     1285 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/runner/__init__.py
+-rw-r--r--   0        0        0     7121 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/runner/base_runner.py
+-rw-r--r--   0        0        0        0 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/runner/classification_runner/__init__.py
+-rw-r--r--   0        0        0     7686 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/runner/classification_runner/classification_runner.py
+-rw-r--r--   0        0        0     6130 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/runner/classification_runner/metaflow_classification.py
+-rw-r--r--   0        0        0      175 2023-05-20 04:33:11.846488 lolpop-0.1.0a5/lolpop/templates/component_template/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-05-20 04:33:11.850488 lolpop-0.1.0a5/lolpop/templates/component_template/{{cookiecutter.component_type}}/__init__.py
+-rw-r--r--   0        0        0      802 2023-05-20 04:33:11.850488 lolpop-0.1.0a5/lolpop/templates/component_template/{{cookiecutter.component_type}}/base_{{cookiecutter.component_type}}.py
+-rw-r--r--   0        0        0     1122 2023-05-20 04:33:11.850488 lolpop-0.1.0a5/lolpop/templates/component_template/{{cookiecutter.component_type}}/{{cookiecutter.component_class}}.py
+-rw-r--r--   0        0        0      167 2023-05-20 04:33:11.850488 lolpop-0.1.0a5/lolpop/templates/pipeline_template/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-05-20 04:33:11.850488 lolpop-0.1.0a5/lolpop/templates/pipeline_template/{{cookiecutter.pipeline_type}}/__init__.py
+-rw-r--r--   0        0        0      803 2023-05-20 04:33:11.850488 lolpop-0.1.0a5/lolpop/templates/pipeline_template/{{cookiecutter.pipeline_type}}/base_{{cookiecutter.pipeline_type}}.py
+-rw-r--r--   0        0        0     1096 2023-05-20 04:33:11.850488 lolpop-0.1.0a5/lolpop/templates/pipeline_template/{{cookiecutter.pipeline_type}}/{{cookiecutter.pipeline_class}}.py
+-rw-r--r--   0        0        0       66 2023-05-20 04:33:11.850488 lolpop-0.1.0a5/lolpop/templates/project_template/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-05-20 04:33:11.850488 lolpop-0.1.0a5/lolpop/templates/project_template/{{cookiecutter.project_name}}/Makefile
+-rw-r--r--   0        0        0       32 2023-05-20 04:33:11.850488 lolpop-0.1.0a5/lolpop/templates/project_template/{{cookiecutter.project_name}}/README.md
+-rw-r--r--   0        0        0        0 2023-05-20 04:33:11.850488 lolpop-0.1.0a5/lolpop/templates/project_template/{{cookiecutter.project_name}}/dvc.yaml
+-rw-r--r--   0        0        0        0 2023-05-20 04:33:11.850488 lolpop-0.1.0a5/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/__init__.py
+-rw-r--r--   0        0        0     1418 2023-05-20 04:33:11.850488 lolpop-0.1.0a5/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/component/__init__.py
+-rw-r--r--   0        0        0     1408 2023-05-20 04:33:11.850488 lolpop-0.1.0a5/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/pipeline/__init__.py
+-rw-r--r--   0        0        0     1363 2023-05-20 04:33:11.850488 lolpop-0.1.0a5/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/runner/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-20 04:33:11.850488 lolpop-0.1.0a5/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop_project.yaml
+-rw-r--r--   0        0        0      310 2023-05-20 04:33:11.850488 lolpop-0.1.0a5/lolpop/templates/project_template/{{cookiecutter.project_name}}/pyproject.toml
+-rw-r--r--   0        0        0      151 2023-05-20 04:33:11.850488 lolpop-0.1.0a5/lolpop/templates/runner_template/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-05-20 04:33:11.850488 lolpop-0.1.0a5/lolpop/templates/runner_template/{{cookiecutter.runner_type}}/__init__.py
+-rw-r--r--   0        0        0      795 2023-05-20 04:33:11.850488 lolpop-0.1.0a5/lolpop/templates/runner_template/{{cookiecutter.runner_type}}/base_{{cookiecutter.runner_type}}.py
+-rw-r--r--   0        0        0     1054 2023-05-20 04:33:11.850488 lolpop-0.1.0a5/lolpop/templates/runner_template/{{cookiecutter.runner_type}}/{{cookiecutter.runner_class}}.py
+-rw-r--r--   0        0        0        0 2023-05-20 04:33:11.850488 lolpop-0.1.0a5/lolpop/utils/__init__.py
+-rw-r--r--   0        0        0    16250 2023-05-20 04:33:11.850488 lolpop-0.1.0a5/lolpop/utils/common_utils.py
+-rw-r--r--   0        0        0     1566 2023-05-20 04:33:11.850488 lolpop-0.1.0a5/lolpop/utils/continual_utils.py
+-rw-r--r--   0        0        0     2452 2023-05-20 04:33:11.850488 lolpop-0.1.0a5/lolpop/utils/metaflow_utils.py
+-rw-r--r--   0        0        0     3298 2023-05-20 04:33:11.850488 lolpop-0.1.0a5/lolpop/utils/mlflow_utils.py
+-rw-r--r--   0        0        0     2261 2023-05-20 04:33:29.454445 lolpop-0.1.0a5/pyproject.toml
+-rw-r--r--   0        0        0     2695 1970-01-01 00:00:00.000000 lolpop-0.1.0a5/PKG-INFO
```

### Comparing `lolpop-0.1.0a4/LICENSE` & `lolpop-0.1.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/cli/cli.py` & `lolpop-0.1.0a5/lolpop/cli/cli.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/cli/create.py` & `lolpop-0.1.0a5/lolpop/cli/create.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/cli/datagen.py` & `lolpop-0.1.0a5/lolpop/cli/datagen.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/cli/run.py` & `lolpop-0.1.0a5/lolpop/cli/run.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/cli/seed.py` & `lolpop-0.1.0a5/lolpop/cli/seed.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/component/__init__.py` & `lolpop-0.1.0a5/lolpop/component/__init__.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/component/base_component.py` & `lolpop-0.1.0a5/lolpop/component/base_component.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,16 @@
     __DEFAULT_CONF__ = {
         "config" : {}
     }
 
     suppress_logger = False
     suppress_notifier = False 
 
-    def __init__(self, conf={}, pipeline_conf={}, runner_conf={}, parent_process=None, problem_type = None, components = {}, *args, **kwargs):
+    def __init__(self, conf={}, pipeline_conf={}, runner_conf={}, parent_process=None, problem_type = None, 
+                 components = {}, skip_config_validation=False, *args, **kwargs):
         #set basic properties, like name and configs
         self.name = type(self).__name__
         config = utils.get_conf(conf)
         self.pipeline_conf = pipeline_conf
         self.runner_conf = runner_conf
         self.parent_process = parent_process
         self.problem_type = problem_type
@@ -32,15 +33,16 @@
         OmegaConf.update(valid_conf, "config",
                          utils.copy_config_into(valid_conf.get("config", {}),
                                                 utils.copy_config_into(pipeline_conf, runner_conf)
                                                 )
                         )
 
         #Now we validate config to make sure the component has everything it needs
-        self._validate_conf(valid_conf, components)
+        if not skip_config_validation: 
+            self._validate_conf(valid_conf, components)
         self.config = omega_conf.get("config", {})
 
         #if the config looks good, then we can set all our components 
         for component in components.keys(): 
             setattr(self, component, components.get(component))
         
     def _update_components(self, components = {}, *args, **kwargs):
```

### Comparing `lolpop-0.1.0a4/lolpop/component/data_checker/deepchecks_data_checker.py` & `lolpop-0.1.0a5/lolpop/component/data_checker/deepchecks_data_checker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/component/data_checker/evidentlyai_data_checker.py` & `lolpop-0.1.0a5/lolpop/component/data_checker/evidentlyai_data_checker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/component/data_connector/bigquery_data_connector.py` & `lolpop-0.1.0a5/lolpop/component/data_connector/bigquery_data_connector.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/component/data_connector/databricks_sql_data_connector.py` & `lolpop-0.1.0a5/lolpop/component/data_connector/databricks_sql_data_connector.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/component/data_connector/duckdb_data_connector.py` & `lolpop-0.1.0a5/lolpop/component/data_connector/duckdb_data_connector.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/component/data_connector/gcs_data_connector.py` & `lolpop-0.1.0a5/lolpop/component/data_connector/gcs_data_connector.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/component/data_connector/local_data_connector.py` & `lolpop-0.1.0a5/lolpop/component/data_connector/local_data_connector.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/component/data_connector/postgres_data_connector.py` & `lolpop-0.1.0a5/lolpop/component/data_connector/postgres_data_connector.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/component/data_connector/redshift_data_connector.py` & `lolpop-0.1.0a5/lolpop/component/data_connector/redshift_data_connector.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/component/data_connector/s3_data_connector.py` & `lolpop-0.1.0a5/lolpop/component/data_connector/s3_data_connector.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/component/data_connector/snowflake_data_connector.py` & `lolpop-0.1.0a5/lolpop/component/data_connector/snowflake_data_connector.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/component/data_profiler/continual_data_profiler.py` & `lolpop-0.1.0a5/lolpop/component/data_profiler/continual_data_profiler.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/component/data_profiler/evidentlyai_data_profiler.py` & `lolpop-0.1.0a5/lolpop/component/data_profiler/evidentlyai_data_profiler.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/component/data_profiler/sweetviz_data_profiler.py` & `lolpop-0.1.0a5/lolpop/component/data_profiler/sweetviz_data_profiler.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/component/data_profiler/ydata_profiling_data_profiler.py` & `lolpop-0.1.0a5/lolpop/component/data_profiler/ydata_profiling_data_profiler.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/component/data_splitter/local_data_splitter.py` & `lolpop-0.1.0a5/lolpop/component/data_splitter/local_data_splitter.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/component/data_synthesizer/svd_data_synthesizer.py` & `lolpop-0.1.0a5/lolpop/component/data_synthesizer/svd_data_synthesizer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/component/data_transformer/bigquery_data_transformer.py` & `lolpop-0.1.0a5/lolpop/component/data_transformer/bigquery_data_transformer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/component/data_transformer/databricks_sql_data_transformer.py` & `lolpop-0.1.0a5/lolpop/component/data_transformer/databricks_sql_data_transformer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/component/data_transformer/dbt_data_transformer.py` & `lolpop-0.1.0a5/lolpop/component/data_transformer/dbt_data_transformer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/component/data_transformer/duckdb_data_transformer.py` & `lolpop-0.1.0a5/lolpop/component/data_transformer/duckdb_data_transformer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/component/data_transformer/local_data_transformer.py` & `lolpop-0.1.0a5/lolpop/component/data_transformer/local_data_transformer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from lolpop.component.data_transformer.base_data_transformer import BaseDataTransformer
 from lolpop.component.data_connector.local_data_connector import LocalDataConnector
 from lolpop.utils import common_utils as utils
 
 from pathlib import Path 
+from omegaconf import dictconfig
 
 
 @utils.decorate_all_methods([utils.error_handler, utils.log_execution()])
 class LocalDataTransformer(BaseDataTransformer):
 
     #use load_config to allow setting "DBT_TARGET", "DBT_PROFILE", "DBT_PROJECT_DIR", "DBT_PROFILES_DIR",  via env variables
     __REQUIRED_CONF__ = {
@@ -41,13 +42,18 @@
 
         Args:
             input_data (String): Names of file to load and pass to transformer file.
 
         Returns:
             pd.DataFrame: the transformed data
         """
-        data = self.data_connector.get_data(input_data)
+        if isinstance(input_data,dict) or isinstance(input_data, dictconfig.DictConfig): 
+            data = {k: self.data_connector.get_data(v) for k,v in input_data.items()}
+        elif isinstance(input_data,str): 
+            data = self.data_connector.get_data(input_data)
+        else: 
+            raise Exception("input_data not a valid type. Expecting dict or str. Found: %s" %str(type(input_data)))
         kwargs = self._get_config("transformer_kwargs",{})
 
         data_out = self._transform(data, **kwargs)
 
         return data_out
```

### Comparing `lolpop-0.1.0a4/lolpop/component/data_transformer/postrgres_data_transformer.py` & `lolpop-0.1.0a5/lolpop/component/data_transformer/postrgres_data_transformer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/component/data_transformer/redshift_data_transformer.py` & `lolpop-0.1.0a5/lolpop/component/data_transformer/redshift_data_transformer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/component/data_transformer/snowflake_data_transformer.py` & `lolpop-0.1.0a5/lolpop/component/data_transformer/snowflake_data_transformer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/component/genai_chatbot/openai_chatbot.py` & `lolpop-0.1.0a5/lolpop/component/genai_chatbot/openai_chatbot.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/component/hyperparameter_tuner/base_hyperparameter_tuner.py` & `lolpop-0.1.0a5/lolpop/component/hyperparameter_tuner/base_hyperparameter_tuner.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/component/hyperparameter_tuner/local_hyperparameter_tuner.py` & `lolpop-0.1.0a5/lolpop/component/hyperparameter_tuner/local_hyperparameter_tuner.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/component/hyperparameter_tuner/optuna_hyperparameter_tuner.py` & `lolpop-0.1.0a5/lolpop/component/hyperparameter_tuner/optuna_hyperparameter_tuner.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/component/logger/file_logger.py` & `lolpop-0.1.0a5/lolpop/component/logger/file_logger.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/component/logger/stdout_logger.py` & `lolpop-0.1.0a5/lolpop/component/logger/stdout_logger.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/component/metadata_tracker/base_metadata_tracker.py` & `lolpop-0.1.0a5/lolpop/component/metadata_tracker/base_metadata_tracker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/component/metadata_tracker/continual_metadata_tracker.py` & `lolpop-0.1.0a5/lolpop/component/metadata_tracker/continual_metadata_tracker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/component/metadata_tracker/mlflow_metadata_tracker.py` & `lolpop-0.1.0a5/lolpop/component/metadata_tracker/mlflow_metadata_tracker.py`

 * *Files 0% similar despite different names*

```diff
@@ -198,15 +198,15 @@
             _, model_id = id.split(".")
             return model_id 
         else: #there's no real heirarchy other than this in the mlflow implementation
             return None 
         
     def register_vc_resource(self, resource, vc_info, key=None, additional_metadata={}, *args, **kwargs):
         #check if a git commit is present. if so then we know we did an external save
-        if "hexsha" in vc_info.keys():
+        if vc_info and "hexsha" in vc_info.keys():
             uri = vc_info.get("uri")
             hexsha = vc_info.get("hexsha")
 
             id = self.get_resource_id(resource)
             if "." not in id: #don't log experiment existance
                 self.log_tag(resource, "exists", "True")
             hexsha_key="hexsha"
```

### Comparing `lolpop-0.1.0a4/lolpop/component/metrics_tracker/continual_metrics_tracker.py` & `lolpop-0.1.0a5/lolpop/component/metrics_tracker/continual_metrics_tracker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/component/metrics_tracker/mlflow_metrics_tracker.py` & `lolpop-0.1.0a5/lolpop/component/metrics_tracker/mlflow_metrics_tracker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/component/model_bias_checker/aifairness_model_bias_checker.py` & `lolpop-0.1.0a5/lolpop/component/model_bias_checker/aifairness_model_bias_checker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/component/model_checker/base_model_checker.py` & `lolpop-0.1.0a5/lolpop/component/model_checker/base_model_checker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/component/model_checker/deepchecks_model_checker.py` & `lolpop-0.1.0a5/lolpop/component/model_checker/deepchecks_model_checker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/component/model_checker/evidentlyai_model_checker.py` & `lolpop-0.1.0a5/lolpop/component/model_checker/evidentlyai_model_checker.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/component/model_deployer/seldon_model_deployer.py` & `lolpop-0.1.0a5/lolpop/component/model_deployer/seldon_model_deployer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/component/model_explainer/alibi_model_explainer.py` & `lolpop-0.1.0a5/lolpop/component/model_explainer/alibi_model_explainer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/component/model_repository/continual_model_repository.py` & `lolpop-0.1.0a5/lolpop/component/model_repository/continual_model_repository.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/component/model_repository/mlflow_model_repository.py` & `lolpop-0.1.0a5/lolpop/component/model_repository/mlflow_model_repository.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/component/model_trainer/base_model_trainer.py` & `lolpop-0.1.0a5/lolpop/component/model_trainer/base_model_trainer.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,16 @@
     model = None 
     mlflow_module = "you_need_to_implement_this_for_mlflow_use"
     
     #predictions = {}
     def __init__(self, params=None, *args, **kwargs): 
         #set normal config
         super().__init__(params=params, *args, **kwargs)
+        if not params: #if params aren't passed in, try to retrieve from config
+            params = self._get_config("training_params", {})
         self.params = params
 
     def fit(self, data, *args, **kwargs): 
         pass 
 
     def predict(self, data, *args, **kwargs): 
         pass
@@ -95,15 +97,15 @@
                 if valid_exists:
                     metrics_out["valid"][metric] = sk_metrics.recall_score(data["y_valid"], predictions["valid"], average = average)
                 if test_exists:
                     metrics_out["test"][metric] = sk_metrics.recall_score(data["y_test"], predictions["test"], average = average)
 
         return metrics_out
 
-    def build_model(self, data, model_version, algo, params): 
+    def build_model(self, data, model_version, *args, **kwargs): 
         #fit model
         model_obj = self.fit(data)
 
         #create experiment and save model 
         experiment = self.metadata_tracker.create_resource(id=None, type="experiment", parent=model_version)
         self.save(experiment)
 
@@ -133,16 +135,15 @@
         df_y = pd.concat([data["y_train"], data["y_valid"]])
         if has_test: 
             df_X = pd.concat([df_X, data["X_test"]])
             df_y = pd.concat([df_y, data["y_test"]])
         train_data = {"X_train" : df_X, "y_train": df_y}
 
         #get params, class from winning experiment 
-        winning_experiment = self.metadata_tracker.get_winning_experiment(model_version)
-        params = self.metadata_tracker.get_metadata(winning_experiment, "training_params")
-        model_trainer = self.metadata_tracker.get_metadata(winning_experiment, "model_trainer")
+        #winning_experiment = self.metadata_tracker.get_winning_experiment(model_version)
+        #params = self.metadata_tracker.get_metadata(winning_experiment, "training_params")
+        #model_trainer = self.metadata_tracker.get_metadata(winning_experiment, "model_trainer")
         
         #rebuild model on all data 
-        #we need to use the single model entry point for this, as this doesn't log the rigth info
-        model, exp = self.build_model(train_data, model_version, model_trainer, params)                        
+        model, exp = self.build_model(train_data, model_version)                        
         
         return model, exp
```

### Comparing `lolpop-0.1.0a4/lolpop/component/model_trainer/xgboost_model_trainer.py` & `lolpop-0.1.0a5/lolpop/component/model_trainer/xgboost_model_trainer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/component/model_visualizer/yellowbrick_model_visualizer.py` & `lolpop-0.1.0a5/lolpop/component/model_visualizer/yellowbrick_model_visualizer.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/component/notifier/gmail_notifier.py` & `lolpop-0.1.0a5/lolpop/component/notifier/gmail_notifier.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/component/notifier/slack_notifier.py` & `lolpop-0.1.0a5/lolpop/component/notifier/slack_notifier.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/component/notifier/smtp_notifier.py` & `lolpop-0.1.0a5/lolpop/component/notifier/smtp_notifier.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/component/resource_version_control/continual_version_control.py` & `lolpop-0.1.0a5/lolpop/component/resource_version_control/continual_version_control.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/component/resource_version_control/dvc_version_control.py` & `lolpop-0.1.0a5/lolpop/component/resource_version_control/dvc_version_control.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/extension/__init__.py` & `lolpop-0.1.0a5/lolpop/extension/__init__.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/pipeline/__init__.py` & `lolpop-0.1.0a5/lolpop/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/pipeline/base_pipeline.py` & `lolpop-0.1.0a5/lolpop/pipeline/base_pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,17 @@
     __DEFAULT_CONF__ = {
         "config" : {}
     }
 
     suppress_logger = False
     suppress_notifier = False
 
-    def __init__(self, conf={}, runner_conf={}, parent_process="runner", problem_type=None, pipeline_type="base_pipeline", components={}, plugin_mods=[], plugin_paths=[], *args, **kwargs):
+    def __init__(self, conf={}, runner_conf={}, parent_process="runner", problem_type=None, 
+                 pipeline_type="base_pipeline", components={}, plugin_mods=[], plugin_paths=[], 
+                 skip_config_validation=False, *args, **kwargs):
         #set basic properties like configs
         self.name = type(self).__name__
         conf = utils.get_conf(conf)
         self.parent_process = parent_process
         self.pipeline_type = pipeline_type
         self.runner_conf = runner_conf
         self.problem_type = problem_type
@@ -27,15 +29,16 @@
         conf = utils.resolve_conf_variables(conf)
         #merge into default conf
         omega_conf = utils.copy_config_into(OmegaConf.create(conf), self.__DEFAULT_CONF__)
         #merge pipeline conf into runner conf
         valid_conf = omega_conf.copy()
         OmegaConf.update(valid_conf, "config", utils.copy_config_into(valid_conf.get("config", {}), runner_conf))
         #validate configuration
-        self._validate_conf(valid_conf, components)
+        if not skip_config_validation:
+            self._validate_conf(valid_conf, components)
         self.config = omega_conf.get("config", {})
 
         #set up reference to each component that is passed in from runner. 
         for component in components.keys(): 
             setattr(self, component, components.get(component))
 
         pipeline_conf = self.config
@@ -52,27 +55,30 @@
         self.plugin_mods = plugin_mods
 
         #now handle all components explicitly set for pipeline
         #note: this will override any component name inherited from the runner, which is what we want
         pipeline_components = {}
         if "components" in conf.keys(): 
             for component in conf.components.keys(): 
-                obj = utils.register_component_class(self, conf, component, pipeline_conf = pipeline_conf, runner_conf = runner_conf, parent_process=self.name, problem_type = self.problem_type, dependent_components=components, plugin_mods=plugin_mods)
+                obj = utils.register_component_class(self, conf, component, pipeline_conf = pipeline_conf, 
+                                                     runner_conf = runner_conf, parent_process=self.name, 
+                                                     problem_type = self.problem_type, dependent_components=components, 
+                                                     plugin_mods=plugin_mods, skip_config_validation=skip_config_validation)
                 if obj is not None: 
                     self.log("Loaded class %s into component %s" %(type(getattr(self, component)).__name__, component))
                     pipeline_components[component] = obj
                 else: 
                     self.log("Unable to load class for component %s" %
                              component)
 
         #now update all pipeline scope components to know about the other pipeline components
         for obj in pipeline_components.values(): 
             obj._update_components(components = pipeline_components)
 
-    def _validate_conf(self, conf, components):
+    def _validate_conf(self, conf, components, skip_validation=False):
         missing, total_missing = utils.validate_conf(conf, self.__REQUIRED_CONF__, components)
         if total_missing > 0: 
             #check to see if missing components are provided by runner via kwargs
             if len(missing.get("components")) > 0: 
                 for component in missing.get("components"): 
                     if components.get(component, None) is not None: 
                         total_missing = total_missing - 1
```

### Comparing `lolpop-0.1.0a4/lolpop/pipeline/deploy/metaflow_offline_deploy.py` & `lolpop-0.1.0a5/lolpop/pipeline/deploy/metaflow_offline_deploy.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/pipeline/deploy/offline_deploy.py` & `lolpop-0.1.0a5/lolpop/pipeline/deploy/offline_deploy.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/pipeline/predict/metaflow_offline_predict.py` & `lolpop-0.1.0a5/lolpop/pipeline/predict/metaflow_offline_predict.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/pipeline/predict/offline_predict.py` & `lolpop-0.1.0a5/lolpop/pipeline/predict/offline_predict.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,16 @@
 
         #make predictions
         data["predictions"] = model._predict_df(df)
         if self.problem_type == "classification": 
             data["predictions_proba"] = model._predict_proba_df(df, to_list=True)
 
         #get explanations
-        data["explanations"] = self.model_explainer.get_explanations(df, model, model_version, "predictions", to_list=True)
+        if not self._get_config("skip_prediction_explanations"):
+            data["explanations"] = self.model_explainer.get_explanations(df, model, model_version, "predictions", to_list=True)
 
         #log predictions
         self.metrics_tracker.log_prediction_metrics(prediction_job, data["predictions"])
 
         return data, prediction_job
 
     def track_predictions(self, prediction_job, data):
```

### Comparing `lolpop-0.1.0a4/lolpop/pipeline/process/metaflow_offline_process.py` & `lolpop-0.1.0a5/lolpop/pipeline/process/metaflow_offline_process.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/pipeline/process/offline_process.py` & `lolpop-0.1.0a5/lolpop/pipeline/process/offline_process.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/pipeline/train/base_train.py` & `lolpop-0.1.0a5/lolpop/pipeline/train/base_train.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/pipeline/train/metaflow_offline_train.py` & `lolpop-0.1.0a5/lolpop/pipeline/train/metaflow_offline_train.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/pipeline/train/offline_train.py` & `lolpop-0.1.0a5/lolpop/pipeline/train/offline_train.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         model_version = self.metadata_tracker.create_resource(id, type="model_version")
     
         #if we are using hyperparameter tuner, use that, otherwise just use the model trainer provided
         if hasattr(self, "hyperparameter_tuner"): 
             model = self.hyperparameter_tuner.run_experiment(data, model_version)
         else: 
             #TODO: this needs a better entry point. build_model doesn't actually log stuff
-            model = self.model_trainer.build_model(data, model_version)
+            model, _  = self.model_trainer.build_model(data, model_version)
 
         return model, model_version
 
     def check_model(self, data_dict, model, model_version, **kwargs):
         #run model checks
         model_report, file_path, checks_status = self.model_checker.check_model(data_dict, model)
```

### Comparing `lolpop-0.1.0a4/lolpop/pipeline/wrapper/metaflow_pipeline_wrapper.py` & `lolpop-0.1.0a5/lolpop/pipeline/wrapper/metaflow_pipeline_wrapper.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/runner/__init__.py` & `lolpop-0.1.0a5/lolpop/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/runner/base_runner.py` & `lolpop-0.1.0a5/lolpop/runner/base_runner.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,20 +13,23 @@
     __DEFAULT_CONF__ = {
         "config" : {}
     }
 
     suppress_logger = False 
     suppress_notifier = False
 
-    def __init__(self, conf={}, problem_type = "unspecified_problem_type", plugin_paths=[]):
+    def __init__(self, conf={}, problem_type = "unspecified_problem_type", plugin_paths=[], 
+                 skip_config_validation=False, *args, **kwargs):
         #handle configuration 
         self.name = type(self).__name__
         conf = utils.get_conf(conf)
+        conf = utils.resolve_conf_variables(conf)
         conf = utils.copy_config_into(conf, self.__DEFAULT_CONF__) 
-        conf = self._validate_conf(conf)
+        if not skip_config_validation:
+            conf = self._validate_conf(conf)
         self.config = conf.get("config", {})
         self.problem_type = conf.get("problem_type", problem_type)
 
         #handle plugins
         if len(plugin_paths) == 0: 
             plugin_paths=conf.get("plugin_paths",[])
         file_path = None
@@ -50,59 +53,63 @@
         # so that they are globally acessible, whereas a component defined at the pipeline level are only accessible
         # in that pipeline and components defined at that pipeline. 
         # componenets in the right scope should know about each other but pipelines act independently (for now, at least)
 
         #set up logger first because we want to pass that to all children
         #we set this up separately from the other components in case you want access to the logger in the 
         #__init__ function
-        logger_obj = utils.register_component_class(self, conf, "logger", default_class_name="StdOutLogger", runner_conf = self.config, plugin_mods=plugin_mods)
+        logger_obj = utils.register_component_class(self, conf, "logger", default_class_name="StdOutLogger", 
+                                                    runner_conf = self.config, plugin_mods=plugin_mods, 
+                                                    skip_config_validation=skip_config_validation)
         if logger_obj is not None: 
             runner_components = {"logger" : logger_obj}
             self.log("Loaded class %s into component %s" %(type(self.logger).__name__, "logger"))
         else: 
             raise Exception("Unable to find logger class.", level="ERROR")
 
         #we also want to special handle the metadata tracker, so we'll set that up first as well and pass 
         #it to all children so they have access in __init__. 
         #it's unclear why you might not want to use a metadata tracker, 
         #but we sould consider this use case in the future 
         meta_obj = utils.register_component_class(self, conf, "metadata_tracker", runner_conf=self.config, parent_process=self.name,
-                                                  problem_type=self.problem_type, dependent_components=runner_components, plugin_mods=plugin_mods)
+                                                  problem_type=self.problem_type, dependent_components=runner_components, 
+                                                  plugin_mods=plugin_mods, skip_config_validation=skip_config_validation)
         if meta_obj is not None:
             runner_components["metadata_tracker"] = meta_obj
             self.log("Loaded class %s into component %s" %(type(self.metadata_tracker).__name__, "metadata_tracker"))
         else: 
             #for local dev you may turn off metadata_tracker, so let's not strictly enforce that it exists for now
-            raise Exception("Unable to load metadata_tracker component.")
+            self.log("Unable to load metadata_tracker component.")
 
         #build all other components
         for component in conf.components.keys(): 
             #ignore logger and metadata_tracker since we have already set those up
             if component != "logger" and component !="metadata_tracker": 
                 obj = utils.register_component_class(self, conf, component, runner_conf=self.config, parent_process=self.name,
-                                                     problem_type=self.problem_type, dependent_components=runner_components, plugin_mods=plugin_mods)
+                                                     problem_type=self.problem_type, dependent_components=runner_components, 
+                                                     plugin_mods=plugin_mods, skip_config_validation=skip_config_validation)
                 if obj is not None: 
                     self.log("Loaded class %s into component %s" %(type(getattr(self, component)).__name__, component))
                     runner_components[component] = obj
                 else: 
                     raise Exception("Unable to load class for component %s" %component)
 
         #now that all component classes are built, we want to update all components so that they know about each other. 
         # there is probably a more elegant way to do this
         for obj in runner_components.values(): 
             obj._update_components(components = runner_components)
 
         #build all pipelines 
         for pipeline in conf.pipelines.keys(): 
             utils.register_pipeline_class(self, conf, pipeline, runner_conf=self.config, parent_process=self.name,
-                                          problem_type=self.problem_type, dependent_components=runner_components, plugin_mods=plugin_mods)
+                                          problem_type=self.problem_type, dependent_components=runner_components, 
+                                          plugin_mods=plugin_mods, skip_config_validation=skip_config_validation)
             self.log("Loaded class %s into pipeline %s" %(type(getattr(self, pipeline)).__name__, pipeline))
 
     def _validate_conf(self, conf):
-        conf = utils.resolve_conf_variables(conf)
         missing, total_missing = utils.validate_conf(conf, self.__REQUIRED_CONF__, conf.get("components"))
         if total_missing>0: 
             #logger is not necessarily set up yet
             #self.logger.log("Missing the following from runner configuration: %s" %missing)
             raise Exception("Missing the following from runner configuration: %s" %missing) 
         return conf
```

### Comparing `lolpop-0.1.0a4/lolpop/runner/classification_runner/classification_runner.py` & `lolpop-0.1.0a5/lolpop/runner/classification_runner/classification_runner.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/runner/classification_runner/metaflow_classification.py` & `lolpop-0.1.0a5/lolpop/runner/classification_runner/metaflow_classification.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/templates/component_template/{{cookiecutter.component_type}}/base_{{cookiecutter.component_type}}.py` & `lolpop-0.1.0a5/lolpop/templates/component_template/{{cookiecutter.component_type}}/base_{{cookiecutter.component_type}}.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/templates/component_template/{{cookiecutter.component_type}}/{{cookiecutter.component_class}}.py` & `lolpop-0.1.0a5/lolpop/templates/component_template/{{cookiecutter.component_type}}/{{cookiecutter.component_class}}.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/templates/pipeline_template/{{cookiecutter.pipeline_type}}/base_{{cookiecutter.pipeline_type}}.py` & `lolpop-0.1.0a5/lolpop/templates/pipeline_template/{{cookiecutter.pipeline_type}}/base_{{cookiecutter.pipeline_type}}.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/templates/pipeline_template/{{cookiecutter.pipeline_type}}/{{cookiecutter.pipeline_class}}.py` & `lolpop-0.1.0a5/lolpop/templates/pipeline_template/{{cookiecutter.pipeline_type}}/{{cookiecutter.pipeline_class}}.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/component/__init__.py` & `lolpop-0.1.0a5/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/component/__init__.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/pipeline/__init__.py` & `lolpop-0.1.0a5/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/runner/__init__.py` & `lolpop-0.1.0a5/lolpop/templates/project_template/{{cookiecutter.project_name}}/lolpop/extension/{{cookiecutter.project_name}}/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/templates/runner_template/{{cookiecutter.runner_type}}/base_{{cookiecutter.runner_type}}.py` & `lolpop-0.1.0a5/lolpop/templates/runner_template/{{cookiecutter.runner_type}}/base_{{cookiecutter.runner_type}}.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/templates/runner_template/{{cookiecutter.runner_type}}/{{cookiecutter.runner_class}}.py` & `lolpop-0.1.0a5/lolpop/templates/runner_template/{{cookiecutter.runner_type}}/{{cookiecutter.runner_class}}.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/utils/common_utils.py` & `lolpop-0.1.0a5/lolpop/utils/common_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -100,53 +100,67 @@
     spec = import_util.spec_from_file_location(file_path.stem, file_path)
     mod = import_util.module_from_spec(spec)
     sys.modules[spec.name]=mod #need to do this to properly register module
     spec.loader.exec_module(mod)
     return mod 
 
 #register component class as an attribute of the provided object
-def register_component_class(self_obj, conf, component_type, default_class_name=None, pipeline_conf = {}, runner_conf = {}, parent_process = "runner", problem_type = None, dependent_components = {}, plugin_mods=[]): 
+def register_component_class(self_obj, conf, component_type, default_class_name=None, 
+                             pipeline_conf = {}, runner_conf = {}, parent_process = "runner", 
+                             problem_type = None, dependent_components = {}, plugin_mods=[], *args, **kwargs): 
     obj = None
     component_class_name = conf.components.get(component_type, default_class_name)
     if component_class_name is not None:
-        obj = None
         try: 
             cl = load_class(component_class_name) 
         except: 
-            self_obj.log(
-            	"Unable to find class %s in built-in components. Searching plugins modules in %s..." %(component_class_name, str(plugin_mods)))
-            cl = load_class_from_plugin(component_class_name, plugin_mods)
-            if cl is not None: 
-                self_obj.log("Found class %s in plugins!" % component_class_name)
-            else: 
-                self_obj.log("Unable to find class %s in plugins!" %component_class_name)
+            try: 
+                self_obj.log("Unable to find component in build-in components. Searching extensions...")
+                cl = load_class(component_class_name, class_type="extension")
+                self_obj.log("Found class %s in extensions!" %component_class_name)
+            except: 
+                self_obj.log(
+                    "Unable to find class %s in extensions. Searching plugins modules in %s..." %(component_class_name, str(plugin_mods)))
+                cl = load_class_from_plugin(component_class_name, plugin_mods)
+                if cl is not None: 
+                    self_obj.log("Found class %s in plugins!" % component_class_name)
+                else: 
+                    self_obj.log("Unable to find class %s in plugins!" %component_class_name)
         if cl is not None: 
             obj = cl(conf=conf.get(component_type, {}), pipeline_conf=pipeline_conf, runner_conf=runner_conf,
-                     parent_process=parent_process, problem_type=problem_type, components=dependent_components)
+                     parent_process=parent_process, problem_type=problem_type, components=dependent_components, *args, **kwargs)
             setattr(self_obj, component_type, obj)
     return obj 
 
 #registers pipeline as an attribute of the provided object
-def register_pipeline_class(self_obj, conf, pipeline_type, default_class_name=None, runner_conf = {}, parent_process = "runner", problem_type = None, dependent_components = {}, plugin_mods=[]): 
+def register_pipeline_class(self_obj, conf, pipeline_type, default_class_name=None, runner_conf = {}, 
+                            parent_process = "runner", problem_type = None, dependent_components = {}, 
+                            plugin_mods=[], *args, **kwargs): 
     obj = None 
     pipeline_class_name = conf.pipelines.get(pipeline_type, default_class_name)
     if pipeline_class_name is not None: 
         try: 
             cl = load_class(pipeline_class_name, class_type="pipeline")
         except: 
-            self_obj.log(
-            	"Unable to find pipeline %s in built-in pipelines. Searching plugins..." % pipeline_class_name)
-            cl = load_class_from_plugin(
-            	pipeline_class_name, plugin_mods, class_type="pipeline")
-            self_obj.log(
-            	"Found class %s in plugins!" % pipeline_class_name)
-        obj = None
+            try: 
+                self_obj.log(
+                    "Unable to find component in build-in components. Searching extensions...")
+                cl = load_class(pipeline_class_name, class_type="extension")
+                self_obj.log("Found class %s in extensions!" %
+                             pipeline_class_name)
+            except: 
+                self_obj.log(
+                    "Unable to find pipeline %s in built-in pipelines. Searching plugins..." % pipeline_class_name)
+                cl = load_class_from_plugin(
+                    pipeline_class_name, plugin_mods, class_type="pipeline")
+                self_obj.log(
+                    "Found class %s in plugins!" % pipeline_class_name)
         if cl is not None: 
             obj = cl(conf=conf.get(pipeline_type, {}), runner_conf=runner_conf, parent_process=parent_process,
-                     problem_type=problem_type, components=dependent_components, plugin_mods=plugin_mods)
+                     problem_type=problem_type, components=dependent_components, plugin_mods=plugin_mods, *args, **kwargs)
             setattr(self_obj, pipeline_type, obj)
     return obj
 
 def lower_conf(conf): 
     return {k.lower():v for k,v in conf.items()}
     
 #Need to revisit. Seems like this is not actually merging on update, it's reassigning.
```

### Comparing `lolpop-0.1.0a4/lolpop/utils/continual_utils.py` & `lolpop-0.1.0a5/lolpop/utils/continual_utils.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/utils/metaflow_utils.py` & `lolpop-0.1.0a5/lolpop/utils/metaflow_utils.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/lolpop/utils/mlflow_utils.py` & `lolpop-0.1.0a5/lolpop/utils/mlflow_utils.py`

 * *Files identical despite different names*

### Comparing `lolpop-0.1.0a4/pyproject.toml` & `lolpop-0.1.0a5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lolpop"
-version = "v0.1.0-alpha.4"
+version = "v0.1.0-alpha.5"
 description = "A software engineering framework for machine learning workflows"
 authors = ["jordanvolz <jordan.volz@gmail.com>"]
 repository = "https://github.com/jordanvolz/lolpop"
 #hompage = 
 #documentation = 
 keywords = ["machine learning", "data science", "mlops"]
 license = "Apache-2.0"
```

### Comparing `lolpop-0.1.0a4/PKG-INFO` & `lolpop-0.1.0a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lolpop
-Version: 0.1.0a4
+Version: 0.1.0a5
 Summary: A software engineering framework for machine learning workflows
 Home-page: https://github.com/jordanvolz/lolpop
 License: Apache-2.0
 Keywords: machine learning,data science,mlops
 Author: jordanvolz
 Author-email: jordan.volz@gmail.com
 Requires-Python: >=3.9,<3.11
```

