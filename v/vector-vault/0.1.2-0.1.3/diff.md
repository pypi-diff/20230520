# Comparing `tmp/vector_vault-0.1.2.tar.gz` & `tmp/vector_vault-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-0.1.2.tar", last modified: Sat May 20 07:46:20 2023, max compression
+gzip compressed data, was "vector_vault-0.1.3.tar", last modified: Sat May 20 07:47:54 2023, max compression
```

## Comparing `vector_vault-0.1.2.tar` & `vector_vault-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-20 07:46:20.222961 vector_vault-0.1.2/
--rw-r--r--   0 johnrood   (501) staff       (20)      688 2023-05-20 04:34:30.000000 vector_vault-0.1.2/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)     9741 2023-05-20 07:46:20.222801 vector_vault-0.1.2/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)     8976 2023-05-20 07:46:11.000000 vector_vault-0.1.2/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-05-20 07:46:20.223003 vector_vault-0.1.2/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1082 2023-05-20 07:46:16.000000 vector_vault-0.1.2/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-20 07:46:20.221769 vector_vault-0.1.2/vector_vault/
--rw-r--r--   0 johnrood   (501) staff       (20)      675 2023-05-20 04:33:21.000000 vector_vault-0.1.2/vector_vault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3660 2023-05-20 06:06:36.000000 vector_vault-0.1.2/vector_vault/closedai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3331 2023-05-20 04:21:10.000000 vector_vault-0.1.2/vector_vault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1855 2023-05-20 04:21:04.000000 vector_vault-0.1.2/vector_vault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-0.1.2/vector_vault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)    18515 2023-05-20 06:46:35.000000 vector_vault-0.1.2/vector_vault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-0.1.2/vector_vault/wrap.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-20 07:46:20.222615 vector_vault-0.1.2/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)     9741 2023-05-20 07:46:20.000000 vector_vault-0.1.2/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      374 2023-05-20 07:46:20.000000 vector_vault-0.1.2/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-05-20 07:46:20.000000 vector_vault-0.1.2/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       53 2023-05-20 07:46:20.000000 vector_vault-0.1.2/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       13 2023-05-20 07:46:20.000000 vector_vault-0.1.2/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-20 07:47:54.261907 vector_vault-0.1.3/
+-rw-r--r--   0 johnrood   (501) staff       (20)      688 2023-05-20 04:34:30.000000 vector_vault-0.1.3/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)     9738 2023-05-20 07:47:54.261711 vector_vault-0.1.3/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)     8973 2023-05-20 07:47:26.000000 vector_vault-0.1.3/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-05-20 07:47:54.261950 vector_vault-0.1.3/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1082 2023-05-20 07:47:49.000000 vector_vault-0.1.3/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-20 07:47:54.260516 vector_vault-0.1.3/vector_vault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      675 2023-05-20 04:33:21.000000 vector_vault-0.1.3/vector_vault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3660 2023-05-20 06:06:36.000000 vector_vault-0.1.3/vector_vault/closedai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3331 2023-05-20 04:21:10.000000 vector_vault-0.1.3/vector_vault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1855 2023-05-20 04:21:04.000000 vector_vault-0.1.3/vector_vault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-0.1.3/vector_vault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    18515 2023-05-20 06:46:35.000000 vector_vault-0.1.3/vector_vault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-0.1.3/vector_vault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-20 07:47:54.261505 vector_vault-0.1.3/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)     9738 2023-05-20 07:47:54.000000 vector_vault-0.1.3/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      374 2023-05-20 07:47:54.000000 vector_vault-0.1.3/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-05-20 07:47:54.000000 vector_vault-0.1.3/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       53 2023-05-20 07:47:54.000000 vector_vault-0.1.3/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       13 2023-05-20 07:47:54.000000 vector_vault-0.1.3/vector_vault.egg-info/top_level.txt
```

### Comparing `vector_vault-0.1.2/LICENSE` & `vector_vault-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-0.1.2/PKG-INFO` & `vector_vault-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 0.1.2
+Version: 0.1.3
 Summary: Vector Vault: Simplified vector database management and secure cloud storage for data science and machine learning workflows.
 Home-page: http://github.com/John-Rood/vector_vault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -13,19 +13,19 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-Vector Vault is designed to simplify the process of working with vector databases. It allows users to manage vector databases efficiently, integrated and accessed seamlessly from the cloud. It's scalable, suitable for both small and large scale databases, and designed with a user-friendly interface. Furthermore, it simplifies complex workflows, ensures secure and isolated data handling, and enables users to create and interact vector databases - aka "vaults" - simply and easily.
+VectorVault is designed to simplify the process of working with vector databases. It allows users to manage vector databases efficiently, integrated and accessed seamlessly from the cloud. It's scalable, suitable for both small and large scale databases, and designed with a user-friendly interface. Furthermore, it simplifies complex workflows, ensures secure and isolated data handling, and enables users to create and interact vector databases - aka "vaults" - simply and easily.
 
-Vector Vault was built with the goal of making complex work flows, that utilize vector databases for informed generative ai, simple and easy. By combining similarity vector search with generative ai chat, new possibilities for conversation and communication emerge. Product information can be added to a vault, and then when customers ask a product question, the right information can be instantly retreived and seamlessly used in conversation by chatgpt for an accurate response. This allows for informed conversation and the possibilites range from ai automated customer support, to new ways to get news and entertainment, to ai code reviews that reference documentation, and much more.
+VectorVault was built with the goal of making complex work flows, that utilize vector databases for informed generative ai, simple and easy. By combining similarity vector search with generative ai chat, new possibilities for conversation and communication emerge. Product information can be added to a vault, and then when customers ask a product question, the right information can be instantly retreived and seamlessly used in conversation by chatgpt for an accurate response. This allows for informed conversation and the possibilites range from ai automated customer support, to new ways to get news and entertainment, to ai code reviews that reference documentation, and much more.
 
-Vector Vault uses a proprietary Inception Architecture, allowing you to create any number of vaults, and vaults within a vaults. Each vault is it's own database, and automatically integrates data storage in the cloud. You will need a Vector Vault account in order to get your user id and api key for cloud access. If you don't already have one, you can sign up free at [VectorVault.io](https://vectorvault.io)
+VectorVault uses a proprietary Inception Architecture, allowing you to create any number of vaults, and vaults within a vaults. Each vault is it's own database, and automatically integrates data storage in the cloud. You will need a Vector Vault account in order to get your user id and api key for cloud access. If you don't already have one, you can sign up free at [VectorVault.io](https://vectorvault.io)
 
 This python library allows you to interact with Vector Vault using its Python-based API. It includes operations such as creating a vault, deleting the vault, adding data to the vault, getting vector embeddings for the data, saving data to the vault, interacting with OpenAI's ChatGPT model to get responses, and managing conversation history for more contextualized responses.
 
 
 # Interact with your Vault:
 
 `add` : Add item to the Vault, with automatic text splitting and processing for long texts. Main way to add to vault
```

### Comparing `vector_vault-0.1.2/README.md` & `vector_vault-0.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-Vector Vault is designed to simplify the process of working with vector databases. It allows users to manage vector databases efficiently, integrated and accessed seamlessly from the cloud. It's scalable, suitable for both small and large scale databases, and designed with a user-friendly interface. Furthermore, it simplifies complex workflows, ensures secure and isolated data handling, and enables users to create and interact vector databases - aka "vaults" - simply and easily.
+VectorVault is designed to simplify the process of working with vector databases. It allows users to manage vector databases efficiently, integrated and accessed seamlessly from the cloud. It's scalable, suitable for both small and large scale databases, and designed with a user-friendly interface. Furthermore, it simplifies complex workflows, ensures secure and isolated data handling, and enables users to create and interact vector databases - aka "vaults" - simply and easily.
 
-Vector Vault was built with the goal of making complex work flows, that utilize vector databases for informed generative ai, simple and easy. By combining similarity vector search with generative ai chat, new possibilities for conversation and communication emerge. Product information can be added to a vault, and then when customers ask a product question, the right information can be instantly retreived and seamlessly used in conversation by chatgpt for an accurate response. This allows for informed conversation and the possibilites range from ai automated customer support, to new ways to get news and entertainment, to ai code reviews that reference documentation, and much more.
+VectorVault was built with the goal of making complex work flows, that utilize vector databases for informed generative ai, simple and easy. By combining similarity vector search with generative ai chat, new possibilities for conversation and communication emerge. Product information can be added to a vault, and then when customers ask a product question, the right information can be instantly retreived and seamlessly used in conversation by chatgpt for an accurate response. This allows for informed conversation and the possibilites range from ai automated customer support, to new ways to get news and entertainment, to ai code reviews that reference documentation, and much more.
 
-Vector Vault uses a proprietary Inception Architecture, allowing you to create any number of vaults, and vaults within a vaults. Each vault is it's own database, and automatically integrates data storage in the cloud. You will need a Vector Vault account in order to get your user id and api key for cloud access. If you don't already have one, you can sign up free at [VectorVault.io](https://vectorvault.io)
+VectorVault uses a proprietary Inception Architecture, allowing you to create any number of vaults, and vaults within a vaults. Each vault is it's own database, and automatically integrates data storage in the cloud. You will need a Vector Vault account in order to get your user id and api key for cloud access. If you don't already have one, you can sign up free at [VectorVault.io](https://vectorvault.io)
 
 This python library allows you to interact with Vector Vault using its Python-based API. It includes operations such as creating a vault, deleting the vault, adding data to the vault, getting vector embeddings for the data, saving data to the vault, interacting with OpenAI's ChatGPT model to get responses, and managing conversation history for more contextualized responses.
 
 
 # Interact with your Vault:
 
 `add` : Add item to the Vault, with automatic text splitting and processing for long texts. Main way to add to vault
```

### Comparing `vector_vault-0.1.2/setup.py` & `vector_vault-0.1.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="0.1.2",
+    version="0.1.3",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="Vector Vault: Simplified vector database management and secure cloud storage for data science and machine learning workflows.",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="http://github.com/John-Rood/vector_vault",
```

### Comparing `vector_vault-0.1.2/vector_vault/__init__.py` & `vector_vault-0.1.3/vector_vault/__init__.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.1.2/vector_vault/closedai.py` & `vector_vault-0.1.3/vector_vault/closedai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.1.2/vector_vault/cloudmanager.py` & `vector_vault-0.1.3/vector_vault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.1.2/vector_vault/creds.py` & `vector_vault-0.1.3/vector_vault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.1.2/vector_vault/download.py` & `vector_vault-0.1.3/vector_vault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.1.2/vector_vault/vault.py` & `vector_vault-0.1.3/vector_vault/vault.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.1.2/vector_vault/wrap.py` & `vector_vault-0.1.3/vector_vault/wrap.py`

 * *Files identical despite different names*

### Comparing `vector_vault-0.1.2/vector_vault.egg-info/PKG-INFO` & `vector_vault-0.1.3/vector_vault.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 0.1.2
+Version: 0.1.3
 Summary: Vector Vault: Simplified vector database management and secure cloud storage for data science and machine learning workflows.
 Home-page: http://github.com/John-Rood/vector_vault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -13,19 +13,19 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-Vector Vault is designed to simplify the process of working with vector databases. It allows users to manage vector databases efficiently, integrated and accessed seamlessly from the cloud. It's scalable, suitable for both small and large scale databases, and designed with a user-friendly interface. Furthermore, it simplifies complex workflows, ensures secure and isolated data handling, and enables users to create and interact vector databases - aka "vaults" - simply and easily.
+VectorVault is designed to simplify the process of working with vector databases. It allows users to manage vector databases efficiently, integrated and accessed seamlessly from the cloud. It's scalable, suitable for both small and large scale databases, and designed with a user-friendly interface. Furthermore, it simplifies complex workflows, ensures secure and isolated data handling, and enables users to create and interact vector databases - aka "vaults" - simply and easily.
 
-Vector Vault was built with the goal of making complex work flows, that utilize vector databases for informed generative ai, simple and easy. By combining similarity vector search with generative ai chat, new possibilities for conversation and communication emerge. Product information can be added to a vault, and then when customers ask a product question, the right information can be instantly retreived and seamlessly used in conversation by chatgpt for an accurate response. This allows for informed conversation and the possibilites range from ai automated customer support, to new ways to get news and entertainment, to ai code reviews that reference documentation, and much more.
+VectorVault was built with the goal of making complex work flows, that utilize vector databases for informed generative ai, simple and easy. By combining similarity vector search with generative ai chat, new possibilities for conversation and communication emerge. Product information can be added to a vault, and then when customers ask a product question, the right information can be instantly retreived and seamlessly used in conversation by chatgpt for an accurate response. This allows for informed conversation and the possibilites range from ai automated customer support, to new ways to get news and entertainment, to ai code reviews that reference documentation, and much more.
 
-Vector Vault uses a proprietary Inception Architecture, allowing you to create any number of vaults, and vaults within a vaults. Each vault is it's own database, and automatically integrates data storage in the cloud. You will need a Vector Vault account in order to get your user id and api key for cloud access. If you don't already have one, you can sign up free at [VectorVault.io](https://vectorvault.io)
+VectorVault uses a proprietary Inception Architecture, allowing you to create any number of vaults, and vaults within a vaults. Each vault is it's own database, and automatically integrates data storage in the cloud. You will need a Vector Vault account in order to get your user id and api key for cloud access. If you don't already have one, you can sign up free at [VectorVault.io](https://vectorvault.io)
 
 This python library allows you to interact with Vector Vault using its Python-based API. It includes operations such as creating a vault, deleting the vault, adding data to the vault, getting vector embeddings for the data, saving data to the vault, interacting with OpenAI's ChatGPT model to get responses, and managing conversation history for more contextualized responses.
 
 
 # Interact with your Vault:
 
 `add` : Add item to the Vault, with automatic text splitting and processing for long texts. Main way to add to vault
```

