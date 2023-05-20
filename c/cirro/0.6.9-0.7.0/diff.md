# Comparing `tmp/cirro-0.6.9.tar.gz` & `tmp/cirro-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cirro-0.6.9.tar", max compression
+gzip compressed data, was "cirro-0.7.0.tar", max compression
```

## Comparing `cirro-0.6.9.tar` & `cirro-0.7.0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0     1086 2023-04-19 22:05:51.562855 cirro-0.6.9/LICENSE.txt
--rw-r--r--   0        0        0     4982 2023-04-19 22:05:51.562855 cirro-0.6.9/README.md
--rw-r--r--   0        0        0       65 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/__init__.py
--rw-r--r--   0        0        0       92 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/__init__.py
--rw-r--r--   0        0        0     1908 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/auth/__init__.py
--rw-r--r--   0        0        0      576 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/auth/base.py
--rw-r--r--   0        0        0     1653 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/auth/iam.py
--rw-r--r--   0        0        0     6650 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/auth/oauth_client.py
--rw-r--r--   0        0        0     1856 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/auth/username.py
--rw-r--r--   0        0        0      133 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/clients/__init__.py
--rw-r--r--   0        0        0     1460 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/clients/api.py
--rw-r--r--   0        0        0     1559 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/clients/portal.py
--rw-r--r--   0        0        0     4045 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/clients/s3.py
--rw-r--r--   0        0        0      199 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/clients/utils.py
--rw-r--r--   0        0        0     3304 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/config.py
--rw-r--r--   0        0        0        0 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/models/__init__.py
--rw-r--r--   0        0        0      101 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/models/api.py
--rw-r--r--   0        0        0      566 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/models/auth.py
--rw-r--r--   0        0        0     1706 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/models/dataset.py
--rw-r--r--   0        0        0      120 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/models/exceptions.py
--rw-r--r--   0        0        0     4250 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/models/file.py
--rw-r--r--   0        0        0     2659 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/models/form_specification.py
--rw-r--r--   0        0        0     3013 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/models/process.py
--rw-r--r--   0        0        0      539 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/models/project.py
--rw-r--r--   0        0        0     1425 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/models/reference.py
--rw-r--r--   0        0        0      430 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/models/s3_path.py
--rw-r--r--   0        0        0      268 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/models/status.py
--rw-r--r--   0        0        0      777 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/models/workflow_models.py
--rw-r--r--   0        0        0      382 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/services/__init__.py
--rw-r--r--   0        0        0     1045 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/services/base.py
--rw-r--r--   0        0        0      690 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/services/common.py
--rw-r--r--   0        0        0     6351 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/services/dataset.py
--rw-r--r--   0        0        0     4201 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/services/file.py
--rw-r--r--   0        0        0     6454 2023-04-19 22:05:51.562855 cirro-0.6.9/cirro/api/services/process.py
--rw-r--r--   0        0        0     2471 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/api/services/project.py
--rw-r--r--   0        0        0      244 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/cli/__init__.py
--rw-r--r--   0        0        0     2523 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/cli/cli.py
--rw-r--r--   0        0        0     6458 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/cli/controller.py
--rw-r--r--   0        0        0        0 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/cli/interactive/__init__.py
--rw-r--r--   0        0        0     1587 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/cli/interactive/auth_args.py
--rw-r--r--   0        0        0      583 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/cli/interactive/common_args.py
--rw-r--r--   0        0        0     4610 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/cli/interactive/download_args.py
--rw-r--r--   0        0        0      573 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/cli/interactive/list_dataset_args.py
--rw-r--r--   0        0        0     3507 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/cli/interactive/upload_args.py
--rw-r--r--   0        0        0     2250 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/cli/interactive/utils.py
--rw-r--r--   0        0        0    12069 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/cli/interactive/workflow_args.py
--rw-r--r--   0        0        0     9132 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/cli/interactive/workflow_form_args.py
--rw-r--r--   0        0        0      371 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/cli/models.py
--rw-r--r--   0        0        0     3685 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/file_utils.py
--rw-r--r--   0        0        0      257 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/helpers/__init__.py
--rw-r--r--   0        0        0     1708 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/helpers/constants.py
--rw-r--r--   0        0        0     5202 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/helpers/form.py
--rw-r--r--   0        0        0     5901 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/helpers/preprocess_dataset.py
--rw-r--r--   0        0        0     9137 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/helpers/workflow_config.py
--rw-r--r--   0        0        0       73 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/sdk/__init__.py
--rw-r--r--   0        0        0     2901 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/sdk/asset.py
--rw-r--r--   0        0        0     3713 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/sdk/dataset.py
--rw-r--r--   0        0        0      245 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/sdk/exceptions.py
--rw-r--r--   0        0        0     4317 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/sdk/file.py
--rw-r--r--   0        0        0     1670 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/sdk/helpers.py
--rw-r--r--   0        0        0     2779 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/sdk/portal.py
--rw-r--r--   0        0        0     1552 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/sdk/process.py
--rw-r--r--   0        0        0     6418 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/sdk/project.py
--rw-r--r--   0        0        0      861 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/sdk/reference.py
--rw-r--r--   0        0        0      964 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/sdk/reference_type.py
--rw-r--r--   0        0        0     1215 2023-04-19 22:05:51.566855 cirro-0.6.9/cirro/utils.py
--rw-r--r--   0        0        0      887 2023-04-19 22:05:51.566855 cirro-0.6.9/pyproject.toml
--rw-r--r--   0        0        0     6227 1970-01-01 00:00:00.000000 cirro-0.6.9/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-05-20 02:59:38.742799 cirro-0.7.0/LICENSE.txt
+-rw-r--r--   0        0        0     5024 2023-05-20 02:59:38.742799 cirro-0.7.0/README.md
+-rw-r--r--   0        0        0       65 2023-05-20 02:59:38.742799 cirro-0.7.0/cirro/__init__.py
+-rw-r--r--   0        0        0       92 2023-05-20 02:59:38.742799 cirro-0.7.0/cirro/api/__init__.py
+-rw-r--r--   0        0        0     1908 2023-05-20 02:59:38.742799 cirro-0.7.0/cirro/api/auth/__init__.py
+-rw-r--r--   0        0        0      576 2023-05-20 02:59:38.742799 cirro-0.7.0/cirro/api/auth/base.py
+-rw-r--r--   0        0        0     1653 2023-05-20 02:59:38.742799 cirro-0.7.0/cirro/api/auth/iam.py
+-rw-r--r--   0        0        0     6663 2023-05-20 02:59:38.742799 cirro-0.7.0/cirro/api/auth/oauth_client.py
+-rw-r--r--   0        0        0     1856 2023-05-20 02:59:38.742799 cirro-0.7.0/cirro/api/auth/username.py
+-rw-r--r--   0        0        0      133 2023-05-20 02:59:38.742799 cirro-0.7.0/cirro/api/clients/__init__.py
+-rw-r--r--   0        0        0     1460 2023-05-20 02:59:38.742799 cirro-0.7.0/cirro/api/clients/api.py
+-rw-r--r--   0        0        0     1559 2023-05-20 02:59:38.742799 cirro-0.7.0/cirro/api/clients/portal.py
+-rw-r--r--   0        0        0     4045 2023-05-20 02:59:38.742799 cirro-0.7.0/cirro/api/clients/s3.py
+-rw-r--r--   0        0        0      199 2023-05-20 02:59:38.742799 cirro-0.7.0/cirro/api/clients/utils.py
+-rw-r--r--   0        0        0     3544 2023-05-20 02:59:38.742799 cirro-0.7.0/cirro/api/config.py
+-rw-r--r--   0        0        0        0 2023-05-20 02:59:38.742799 cirro-0.7.0/cirro/api/models/__init__.py
+-rw-r--r--   0        0        0      101 2023-05-20 02:59:38.742799 cirro-0.7.0/cirro/api/models/api.py
+-rw-r--r--   0        0        0      566 2023-05-20 02:59:38.742799 cirro-0.7.0/cirro/api/models/auth.py
+-rw-r--r--   0        0        0     1763 2023-05-20 02:59:38.742799 cirro-0.7.0/cirro/api/models/dataset.py
+-rw-r--r--   0        0        0      120 2023-05-20 02:59:38.742799 cirro-0.7.0/cirro/api/models/exceptions.py
+-rw-r--r--   0        0        0     4250 2023-05-20 02:59:38.742799 cirro-0.7.0/cirro/api/models/file.py
+-rw-r--r--   0        0        0     2659 2023-05-20 02:59:38.742799 cirro-0.7.0/cirro/api/models/form_specification.py
+-rw-r--r--   0        0        0     3013 2023-05-20 02:59:38.742799 cirro-0.7.0/cirro/api/models/process.py
+-rw-r--r--   0        0        0      539 2023-05-20 02:59:38.742799 cirro-0.7.0/cirro/api/models/project.py
+-rw-r--r--   0        0        0     1425 2023-05-20 02:59:38.742799 cirro-0.7.0/cirro/api/models/reference.py
+-rw-r--r--   0        0        0      430 2023-05-20 02:59:38.742799 cirro-0.7.0/cirro/api/models/s3_path.py
+-rw-r--r--   0        0        0      268 2023-05-20 02:59:38.742799 cirro-0.7.0/cirro/api/models/status.py
+-rw-r--r--   0        0        0      777 2023-05-20 02:59:38.742799 cirro-0.7.0/cirro/api/models/workflow_models.py
+-rw-r--r--   0        0        0      382 2023-05-20 02:59:38.742799 cirro-0.7.0/cirro/api/services/__init__.py
+-rw-r--r--   0        0        0     1045 2023-05-20 02:59:38.742799 cirro-0.7.0/cirro/api/services/base.py
+-rw-r--r--   0        0        0      690 2023-05-20 02:59:38.742799 cirro-0.7.0/cirro/api/services/common.py
+-rw-r--r--   0        0        0     6405 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/api/services/dataset.py
+-rw-r--r--   0        0        0     4189 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/api/services/file.py
+-rw-r--r--   0        0        0     6454 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/api/services/process.py
+-rw-r--r--   0        0        0     2471 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/api/services/project.py
+-rw-r--r--   0        0        0      244 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/cli/__init__.py
+-rw-r--r--   0        0        0     2523 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/cli/cli.py
+-rw-r--r--   0        0        0     6754 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/cli/controller.py
+-rw-r--r--   0        0        0        0 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/cli/interactive/__init__.py
+-rw-r--r--   0        0        0      318 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/cli/interactive/auth_args.py
+-rw-r--r--   0        0        0      770 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/cli/interactive/common_args.py
+-rw-r--r--   0        0        0     4610 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/cli/interactive/download_args.py
+-rw-r--r--   0        0        0      573 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/cli/interactive/list_dataset_args.py
+-rw-r--r--   0        0        0     3507 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/cli/interactive/upload_args.py
+-rw-r--r--   0        0        0     2250 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/cli/interactive/utils.py
+-rw-r--r--   0        0        0    12069 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/cli/interactive/workflow_args.py
+-rw-r--r--   0        0        0     9132 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/cli/interactive/workflow_form_args.py
+-rw-r--r--   0        0        0      371 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/cli/models.py
+-rw-r--r--   0        0        0     3685 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/file_utils.py
+-rw-r--r--   0        0        0      257 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/helpers/__init__.py
+-rw-r--r--   0        0        0     1708 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/helpers/constants.py
+-rw-r--r--   0        0        0     5202 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/helpers/form.py
+-rw-r--r--   0        0        0     5901 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/helpers/preprocess_dataset.py
+-rw-r--r--   0        0        0     9137 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/helpers/workflow_config.py
+-rw-r--r--   0        0        0       73 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/sdk/__init__.py
+-rw-r--r--   0        0        0     2901 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/sdk/asset.py
+-rw-r--r--   0        0        0     3758 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/sdk/dataset.py
+-rw-r--r--   0        0        0      245 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/sdk/exceptions.py
+-rw-r--r--   0        0        0     4317 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/sdk/file.py
+-rw-r--r--   0        0        0     1670 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/sdk/helpers.py
+-rw-r--r--   0        0        0     2779 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/sdk/portal.py
+-rw-r--r--   0        0        0     1552 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/sdk/process.py
+-rw-r--r--   0        0        0     6418 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/sdk/project.py
+-rw-r--r--   0        0        0      861 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/sdk/reference.py
+-rw-r--r--   0        0        0      964 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/sdk/reference_type.py
+-rw-r--r--   0        0        0     1215 2023-05-20 02:59:38.746799 cirro-0.7.0/cirro/utils.py
+-rw-r--r--   0        0        0      887 2023-05-20 02:59:38.750799 cirro-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     6269 1970-01-01 00:00:00.000000 cirro-0.7.0/PKG-INFO
```

### Comparing `cirro-0.6.9/LICENSE.txt` & `cirro-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cirro-0.6.9/README.md` & `cirro-0.7.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -12,21 +12,19 @@
 
 `pip install cirro`
 
 or by cloning the repository and running:
 
 `python setup.py install`
 
-## Set Up
-Run a one-time configuration of your login credentials in the command line using:
+## Authentication
 
-`cirro-cli configure`
-
- This will ask you to select an authentication method. If you are a member of Fred Hutch or the University of Washington, select the default method which will give you a link to use to log through the browser. If you are not a member of those institutions, select the non-institutional authentication method and enter your Data Portal username and password into the command line when prompted.
+Upon first use, the Cirro client will ask if you would like to save your login information and give you a link to authenticate through the web browser.
 
+If you need to change your credentials after this point, and you've opted to save your login, please see the [clearing saved login](#clearing-saved-login) section.
 
 ## Command Line Usage
 
 #### Downloading a dataset:
 ```bash
 Usage: cirro-cli download [OPTIONS]
 
@@ -103,27 +101,32 @@
 |-----------------------------------------------------|---------------------|
 | [Downloading a dataset in R](samples/Using-R.ipynb) | Reading data with R |
 
 ## Advanced Usage
 
 ### Supported environment variables
 
-| Name        | Description                   | Default         |
-|-------------|-------------------------------|-----------------|
-| PW_HOME     | Local configuration directory | ~/.cirro        |
-| PW_BASE_URL | Base URL of the data portal   | data-portal.io  |
+| Name        | Description                   | Default   |
+|-------------|-------------------------------|-----------|
+| PW_HOME     | Local configuration directory | ~/.cirro  |
+| PW_BASE_URL | Base URL of the data portal   | cirro.bio |
 
 ### Configuration
 
 The `cirro-cli configure` command creates a file in `PW_HOME` called `config.ini`.
 
 You can set the `base_url` property in the config file rather than using the environment variable. 
 
 The `transfer_max_retries` configuration property specifies the maximum number of times to attempt uploading a file to Cirro in the event of a transfer failure. 
 When uploading files to Cirro, network issues or temporary outages can occasionally cause a transfer to fail.
 It will pause for an increasing amount of time for each retry attempt.
 
 ```ini
 [General]
-base_url = data-portal.io
+base_url = cirro.bio
 transfer_max_retries = 15
-```
+```
+
+### Clearing saved login
+
+You can clear your saved login information by removing the `~/.cirro/token.dat` file from your system or
+by running `cirro-cli configure` and selecting **No** when it asks if you'd like to save your login information.
```

### Comparing `cirro-0.6.9/cirro/api/auth/__init__.py` & `cirro-0.7.0/cirro/api/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.9/cirro/api/auth/base.py` & `cirro-0.7.0/cirro/api/auth/base.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.9/cirro/api/auth/iam.py` & `cirro-0.7.0/cirro/api/auth/iam.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.9/cirro/api/auth/oauth_client.py` & `cirro-0.7.0/cirro/api/auth/oauth_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         'device_code': flow['device_code'],
         'grant_type': 'urn:ietf:params:oauth:grant-type:device_code'
     }
 
     auth_status = 'authorization_pending'
     while auth_status == 'authorization_pending':
         time.sleep(flow['interval'])
-        if device_expiry < datetime.now():
+        if device_expiry < datetime.now().astimezone():
             raise RuntimeError('Authentication timed out')
 
         resp = requests.post(f'{auth_endpoint}/token', params=params)
         token_result: OAuthTokenResponse = resp.json()
         auth_status = token_result.get('message')
         logger.debug(auth_status)
```

### Comparing `cirro-0.6.9/cirro/api/auth/username.py` & `cirro-0.7.0/cirro/api/auth/username.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.9/cirro/api/clients/api.py` & `cirro-0.7.0/cirro/api/clients/api.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.9/cirro/api/clients/portal.py` & `cirro-0.7.0/cirro/api/clients/portal.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.9/cirro/api/clients/s3.py` & `cirro-0.7.0/cirro/api/clients/s3.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.9/cirro/api/config.py` & `cirro-0.7.0/cirro/api/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import requests
 from requests import HTTPError
 
 
 class Constants:
     home = os.environ.get('PW_HOME', '~/.cirro')
     config_path = Path(home, 'config.ini').expanduser()
-    default_base_url = "data-portal.io"
+    default_base_url = 'cirro.bio'
     default_max_retries = 10
 
 
 class UserConfig(NamedTuple):
     auth_method: str
     auth_method_config: Dict  # This needs to match the init params of the auth method
     base_url: Optional[str]
@@ -27,14 +27,15 @@
     ini_config['General'] = {
         'auth_method': user_config.auth_method,
         'base_url': Constants.default_base_url,
         'transfer_max_retries': Constants.default_max_retries
     }
     if original_user_config:
         ini_config['General']['base_url'] = original_user_config.base_url
+        ini_config['General']['transfer_max_retries'] = str(original_user_config.transfer_max_retries)
 
     ini_config[user_config.auth_method] = user_config.auth_method_config
     Constants.config_path.parent.mkdir(exist_ok=True)
     with Constants.config_path.open('w') as configfile:
         ini_config.write(configfile)
 
 
@@ -68,14 +69,16 @@
 class AppConfig:
     def __init__(self, base_url: str = None):
         self.user_config = load_user_config()
         self.base_url = (base_url or
                          os.environ.get('PW_BASE_URL') or
                          (self.user_config.base_url if self.user_config else None) or
                          Constants.default_base_url)
+        self.transfer_max_retries = self.user_config.transfer_max_retries\
+            if self.user_config else Constants.default_max_retries
         self._init_config()
 
     def _init_config(self):
         self.rest_endpoint = f'https://api.{self.base_url}'
         self.auth_endpoint = f'https://api.{self.base_url}/auth'
 
         try:
```

### Comparing `cirro-0.6.9/cirro/api/models/auth.py` & `cirro-0.7.0/cirro/api/models/auth.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.9/cirro/api/models/dataset.py` & `cirro-0.7.0/cirro/api/models/dataset.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     process_id: str
     project_id: str
     status: Status
     source_dataset_ids: List[str]
     info: Dict[str, Any]
     params: Dict[str, Any]
     created_at: datetime
+    created_by: str
 
     @classmethod
     def from_record(cls, record):
         if record is None:
             raise DataPortalModelException("Cannot construct Dataset from null object.")
         return cls(
             record.get('id'),
@@ -53,13 +54,14 @@
             record.get('desc'),
             record.get('process'),
             record.get('project'),
             Status[record.get('status')],
             record.get('sourceDatasets'),
             safe_load_json(record.get('infoJson')),
             safe_load_json(record.get('paramJson')),
-            parse_json_date(record.get('createdAt'))
+            parse_json_date(record.get('createdAt')),
+            record.get('createdBy')
         )
 
     @property
     def relative_url(self):
         return f'projects/{self.project_id}/dataset/{self.id}'
```

### Comparing `cirro-0.6.9/cirro/api/models/file.py` & `cirro-0.7.0/cirro/api/models/file.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.9/cirro/api/models/form_specification.py` & `cirro-0.7.0/cirro/api/models/form_specification.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.9/cirro/api/models/process.py` & `cirro-0.7.0/cirro/api/models/process.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.9/cirro/api/models/project.py` & `cirro-0.7.0/cirro/api/models/project.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.9/cirro/api/models/reference.py` & `cirro-0.7.0/cirro/api/models/reference.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.9/cirro/api/models/workflow_models.py` & `cirro-0.7.0/cirro/api/models/workflow_models.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.9/cirro/api/services/base.py` & `cirro-0.7.0/cirro/api/services/base.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.9/cirro/api/services/common.py` & `cirro-0.7.0/cirro/api/services/common.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.9/cirro/api/services/dataset.py` & `cirro-0.7.0/cirro/api/services/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
                 status
                 name
                 desc
                 sourceDatasets
                 infoJson
                 paramJson
                 process
+                createdBy
                 createdAt
                 updatedAt
               }
               nextToken
             }
           }
         '''
@@ -75,14 +76,15 @@
                   name
                   desc
                   sourceDatasets
                   paramJson
                   infoJson
                   process
                   project
+                  createdBy
                   createdAt
                   updatedAt
                 }
               }
               '''
 
         item = self._api_client.query(query, variables={'id': _id})['getDataset']
```

### Comparing `cirro-0.6.9/cirro/api/services/file.py` & `cirro-0.7.0/cirro/api/services/file.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         :param access_context: File access context, use class methods to generate
         :param directory: base path to upload from
         :param files: relative path of files to upload
         :return:
         """
         s3_client = S3Client(partial(self.get_access_credentials, access_context), self._configuration.region)
         upload_directory(directory, files, s3_client, access_context.bucket, access_context.path_prefix,
-                         max_retries=self._configuration.user_config.transfer_max_retries)
+                         max_retries=self._configuration.transfer_max_retries)
 
     def download_files(self, access_context: FileAccessContext, directory: str, files: List[str]):
         """
         Download a list of files to the specified directory
         :param access_context: File access context, use class methods to generate
         :param directory: download location
         :param files: relative path of files to download
```

### Comparing `cirro-0.6.9/cirro/api/services/process.py` & `cirro-0.7.0/cirro/api/services/process.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.9/cirro/api/services/project.py` & `cirro-0.7.0/cirro/api/services/project.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.9/cirro/cli/cli.py` & `cirro-0.7.0/cirro/cli/cli.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.9/cirro/cli/controller.py` & `cirro-0.7.0/cirro/cli/controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from cirro.api.clients.portal import DataPortalClient
-from cirro.api.config import UserConfig, save_user_config
+from cirro.api.config import UserConfig, save_user_config, load_user_config
 from cirro.api.models.dataset import CreateIngestDatasetInput
 from cirro.api.models.process import Executor
 from cirro.cli.interactive.auth_args import gather_auth_config
 from cirro.cli.interactive.download_args import gather_download_arguments, ask_dataset_files
 from cirro.cli.interactive.download_args import gather_download_arguments_dataset
 from cirro.cli.interactive.list_dataset_args import gather_list_arguments
 from cirro.cli.interactive.upload_args import gather_upload_arguments
@@ -15,16 +15,15 @@
 from cirro.cli.models import ListArguments, UploadArguments, DownloadArguments
 from cirro.file_utils import get_files_in_directory
 from cirro.helpers import WorkflowConfigBuilder
 
 
 def run_list_datasets(input_params: ListArguments, interactive=False):
     """List the datasets available in a particular project."""
-
-    # Instantiate the Cirro Data Portal client
+    _check_configure()
     cirro = DataPortalClient()
 
     # If the user provided the --interactive flag
     if interactive:
 
         # Get the list of projects available to the user
         projects = cirro.project.list()
@@ -43,14 +42,15 @@
     print("\n\n".join([f'Name: {dataset.name}\n'
                        f'Desc: {dataset.description}\n'
                        f'GUID: ({dataset.id})'
                        for dataset in sorted_datasets]))
 
 
 def run_ingest(input_params: UploadArguments, interactive=False):
+    _check_configure()
     cirro = DataPortalClient()
     projects = cirro.project.list()
     processes = cirro.process.list(process_type=Executor.INGEST)
 
     if len(projects) == 0:
         print("No projects available")
         return
@@ -79,14 +79,15 @@
     cirro.dataset.upload_files(dataset_id=create_resp['datasetId'],
                                project_id=create_request.project_id,
                                directory=directory,
                                files=files)
 
 
 def run_download(input_params: DownloadArguments, interactive=False):
+    _check_configure()
     cirro = DataPortalClient()
 
     projects = cirro.project.list()
 
     if len(projects) == 0:
         print("No projects available")
         return
@@ -110,15 +111,15 @@
                                  dataset_id=dataset_params['dataset'],
                                  download_location=input_params['data_directory'],
                                  files=files_to_download)
 
 
 def run_configure_workflow():
     """Configure a workflow to be run in the Data Portal as a process."""
-
+    _check_configure()
     cirro = DataPortalClient()
     process_options = cirro.process.list(process_type=Executor.NEXTFLOW)
     resources_folder, repo_prefix = get_output_resources_path()
 
     workflow = WorkflowConfigBuilder(repo_prefix)
 
     # Process record
@@ -167,8 +168,19 @@
     workflow.save_local(resources_folder)
 
 
 def run_configure():
     auth_method, auth_method_config = gather_auth_config()
     save_user_config(UserConfig(auth_method=auth_method,
                                 auth_method_config=auth_method_config,
-                                base_url=None))
+                                base_url=None,
+                                transfer_max_retries=None))
+
+
+def _check_configure():
+    """
+    Prompts the user to do initial configuration if needed
+    """
+    if load_user_config() is not None:
+        return
+
+    run_configure()
```

### Comparing `cirro-0.6.9/cirro/cli/interactive/common_args.py` & `cirro-0.7.0/cirro/cli/interactive/common_args.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 from typing import List
 
 from cirro.api.models.project import Project
-from cirro.cli.interactive.utils import prompt_wrapper
+from cirro.cli.interactive.utils import ask
 
 
 def ask_project(projects: List[Project], input_value: str) -> str:
-    project_names = [project.name for project in projects]
-    project_prompt = {
-        'type': 'list',
-        'name': 'project',
-        'message': 'What project is this dataset associated with?',
-        'choices': project_names,
-        'default': input_value if input_value in project_names else None
-    }
-    answers = prompt_wrapper(project_prompt)
-    return answers['project']
+    project_names = sorted([project.name for project in projects])
+    if len(project_names) <= 10:
+        return ask(
+            'select',
+            'What project is this dataset associated with?',
+            choices=project_names,
+            default=input_value if input_value in project_names else None
+        )
+    else:
+        return ask(
+            'autocomplete',
+            'What project is this dataset associated with? (use TAB to display options)',
+            choices=project_names,
+            default=input_value if input_value in project_names else ''
+        )
```

### Comparing `cirro-0.6.9/cirro/cli/interactive/download_args.py` & `cirro-0.7.0/cirro/cli/interactive/download_args.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.9/cirro/cli/interactive/list_dataset_args.py` & `cirro-0.7.0/cirro/cli/interactive/list_dataset_args.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.9/cirro/cli/interactive/upload_args.py` & `cirro-0.7.0/cirro/cli/interactive/upload_args.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.9/cirro/cli/interactive/utils.py` & `cirro-0.7.0/cirro/cli/interactive/utils.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.9/cirro/cli/interactive/workflow_args.py` & `cirro-0.7.0/cirro/cli/interactive/workflow_args.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.9/cirro/cli/interactive/workflow_form_args.py` & `cirro-0.7.0/cirro/cli/interactive/workflow_form_args.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.9/cirro/file_utils.py` & `cirro-0.7.0/cirro/file_utils.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.9/cirro/helpers/constants.py` & `cirro-0.7.0/cirro/helpers/constants.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.9/cirro/helpers/form.py` & `cirro-0.7.0/cirro/helpers/form.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.9/cirro/helpers/preprocess_dataset.py` & `cirro-0.7.0/cirro/helpers/preprocess_dataset.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.9/cirro/helpers/workflow_config.py` & `cirro-0.7.0/cirro/helpers/workflow_config.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.9/cirro/sdk/asset.py` & `cirro-0.7.0/cirro/sdk/asset.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.9/cirro/sdk/dataset.py` & `cirro-0.7.0/cirro/sdk/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
         self.process_id = dataset.process_id
         self.project_id = dataset.project_id
         self.status = dataset.status
         self.source_dataset_ids = dataset.source_dataset_ids
         self.info = dataset.info
         self.params = dataset.params
         self.created_at = dataset.created_at
+        self.created_by = dataset.created_by
         self._client = client
 
     def __str__(self):
         return '\n'.join([
             f"{i.title()}: {self.__getattribute__(i)}"
             for i in ['name', 'id', 'description', 'status']
         ])
```

### Comparing `cirro-0.6.9/cirro/sdk/file.py` & `cirro-0.7.0/cirro/sdk/file.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.9/cirro/sdk/helpers.py` & `cirro-0.7.0/cirro/sdk/helpers.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.9/cirro/sdk/portal.py` & `cirro-0.7.0/cirro/sdk/portal.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.9/cirro/sdk/process.py` & `cirro-0.7.0/cirro/sdk/process.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.9/cirro/sdk/project.py` & `cirro-0.7.0/cirro/sdk/project.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.9/cirro/sdk/reference.py` & `cirro-0.7.0/cirro/sdk/reference.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.9/cirro/sdk/reference_type.py` & `cirro-0.7.0/cirro/sdk/reference_type.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.9/cirro/utils.py` & `cirro-0.7.0/cirro/utils.py`

 * *Files identical despite different names*

### Comparing `cirro-0.6.9/pyproject.toml` & `cirro-0.7.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cirro"
-version = "0.6.9"
+version = "0.7.0"
 description = "CLI tool and SDK for interacting with the Cirro platform"
 authors = ["Fred Hutch <cirro@fredhutch.org>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/FredHutch/Cirro-client"
 packages = [{include = "cirro"}]
```

### Comparing `cirro-0.6.9/PKG-INFO` & `cirro-0.7.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cirro
-Version: 0.6.9
+Version: 0.7.0
 Summary: CLI tool and SDK for interacting with the Cirro platform
 Home-page: https://github.com/FredHutch/Cirro-client
 License: MIT
 Author: Fred Hutch
 Author-email: cirro@fredhutch.org
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -44,21 +44,19 @@
 
 `pip install cirro`
 
 or by cloning the repository and running:
 
 `python setup.py install`
 
-## Set Up
-Run a one-time configuration of your login credentials in the command line using:
+## Authentication
 
-`cirro-cli configure`
-
- This will ask you to select an authentication method. If you are a member of Fred Hutch or the University of Washington, select the default method which will give you a link to use to log through the browser. If you are not a member of those institutions, select the non-institutional authentication method and enter your Data Portal username and password into the command line when prompted.
+Upon first use, the Cirro client will ask if you would like to save your login information and give you a link to authenticate through the web browser.
 
+If you need to change your credentials after this point, and you've opted to save your login, please see the [clearing saved login](#clearing-saved-login) section.
 
 ## Command Line Usage
 
 #### Downloading a dataset:
 ```bash
 Usage: cirro-cli download [OPTIONS]
 
@@ -135,27 +133,33 @@
 |-----------------------------------------------------|---------------------|
 | [Downloading a dataset in R](samples/Using-R.ipynb) | Reading data with R |
 
 ## Advanced Usage
 
 ### Supported environment variables
 
-| Name        | Description                   | Default         |
-|-------------|-------------------------------|-----------------|
-| PW_HOME     | Local configuration directory | ~/.cirro        |
-| PW_BASE_URL | Base URL of the data portal   | data-portal.io  |
+| Name        | Description                   | Default   |
+|-------------|-------------------------------|-----------|
+| PW_HOME     | Local configuration directory | ~/.cirro  |
+| PW_BASE_URL | Base URL of the data portal   | cirro.bio |
 
 ### Configuration
 
 The `cirro-cli configure` command creates a file in `PW_HOME` called `config.ini`.
 
 You can set the `base_url` property in the config file rather than using the environment variable. 
 
 The `transfer_max_retries` configuration property specifies the maximum number of times to attempt uploading a file to Cirro in the event of a transfer failure. 
 When uploading files to Cirro, network issues or temporary outages can occasionally cause a transfer to fail.
 It will pause for an increasing amount of time for each retry attempt.
 
 ```ini
 [General]
-base_url = data-portal.io
+base_url = cirro.bio
 transfer_max_retries = 15
 ```
+
+### Clearing saved login
+
+You can clear your saved login information by removing the `~/.cirro/token.dat` file from your system or
+by running `cirro-cli configure` and selecting **No** when it asks if you'd like to save your login information.
+
```

