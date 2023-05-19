# Comparing `tmp/ds4finance-0.1.15.tar.gz` & `tmp/ds4finance-0.1.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ds4finance-0.1.15.tar", last modified: Mon May  8 14:17:32 2023, max compression
+gzip compressed data, was "ds4finance-0.1.17.tar", last modified: Fri May 19 22:40:09 2023, max compression
```

## Comparing `ds4finance-0.1.15.tar` & `ds4finance-0.1.17.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 14:17:32.784198 ds4finance-0.1.15/
--rw-rw-rw-   0        0        0     2627 2023-05-08 14:17:32.783197 ds4finance-0.1.15/PKG-INFO
--rw-rw-rw-   0        0        0     1243 2023-04-20 20:51:26.000000 ds4finance-0.1.15/README.md
-drwxrwxrwx   0        0        0        0 2023-05-08 14:17:32.767194 ds4finance-0.1.15/ds4finance/
--rw-rw-rw-   0        0        0     1021 2023-05-08 14:17:00.000000 ds4finance-0.1.15/ds4finance/__init__.py
--rw-rw-rw-   0        0        0    31358 2023-05-08 14:07:04.000000 ds4finance-0.1.15/ds4finance/functions.py
-drwxrwxrwx   0        0        0        0 2023-05-08 14:17:32.781197 ds4finance-0.1.15/ds4finance.egg-info/
--rw-rw-rw-   0        0        0     2627 2023-05-08 14:17:32.000000 ds4finance-0.1.15/ds4finance.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2023-05-08 14:17:32.000000 ds4finance-0.1.15/ds4finance.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 14:17:32.000000 ds4finance-0.1.15/ds4finance.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-08 14:17:32.000000 ds4finance-0.1.15/ds4finance.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-08 14:17:32.000000 ds4finance-0.1.15/ds4finance.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-08 14:17:32.784198 ds4finance-0.1.15/setup.cfg
--rw-rw-rw-   0        0        0     1174 2023-05-08 14:17:29.000000 ds4finance-0.1.15/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 22:40:09.798157 ds4finance-0.1.17/
+-rw-rw-rw-   0        0        0     1088 2023-04-20 20:49:15.000000 ds4finance-0.1.17/LICENSE.txt
+-rw-rw-rw-   0        0        0     2215 2023-05-19 22:40:09.798157 ds4finance-0.1.17/PKG-INFO
+-rw-rw-rw-   0        0        0     1243 2023-04-20 20:51:26.000000 ds4finance-0.1.17/README.md
+drwxrwxrwx   0        0        0        0 2023-05-19 22:40:09.721819 ds4finance-0.1.17/ds4finance/
+-rw-rw-rw-   0        0        0     1077 2023-05-19 22:35:03.000000 ds4finance-0.1.17/ds4finance/__init__.py
+-rw-rw-rw-   0        0        0    34627 2023-05-19 22:34:40.000000 ds4finance-0.1.17/ds4finance/functions.py
+drwxrwxrwx   0        0        0        0 2023-05-19 22:40:09.795500 ds4finance-0.1.17/ds4finance.egg-info/
+-rw-rw-rw-   0        0        0     2215 2023-05-19 22:40:09.000000 ds4finance-0.1.17/ds4finance.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2023-05-19 22:40:09.000000 ds4finance-0.1.17/ds4finance.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 22:40:09.000000 ds4finance-0.1.17/ds4finance.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-19 22:40:09.000000 ds4finance-0.1.17/ds4finance.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-19 22:40:09.000000 ds4finance-0.1.17/ds4finance.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-19 22:40:09.798157 ds4finance-0.1.17/setup.cfg
+-rw-rw-rw-   0        0        0     1175 2023-05-19 22:36:25.000000 ds4finance-0.1.17/setup.py
```

### Comparing `ds4finance-0.1.15/PKG-INFO` & `ds4finance-0.1.17/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,75 +1,75 @@
 Metadata-Version: 2.1
 Name: ds4finance
-Version: 0.1.15
+Version: 0.1.17
 Summary: A collection of data science tools for finance
 Home-page: https://github.com/LuisSousaSilva/ds4finance
 Author: Luis Silva
 Author-email: luis_paulo_silva@hotmail.com
 License: MIT
-Description: # ds4finance
-        
-        A collection of data science tools for finance.
-        
-        ## Installation
-        
-        Install the package from PyPI using pip:
-        
-        ```python
-        pip install ds4finance
-        ```
-        
-        ## Usage 
-        
-        To use the package, import it using the alias dsf:
-        
-        import ds4finance as dsf
-        
-        ### Example: Computing Standard Deviation
-        
-        ```python
-        import pandas as pd
-        import ds4finance as dsf
-        
-        # Load or create a DataFrame containing financial data
-        data = pd.read_csv("your_data.csv")
-        
-        # Compute the annualized standard deviation for the data
-        std_dev = dsf.compute_std_dev(data)
-        ```
-        
-        ## License
-        
-        This project is licensed under the MIT License. See the [LICENSE.txt](LICENSE.txt) file for more information.
-        
-        ## Contributing
-        
-        We welcome contributions to the project. If you'd like to contribute, please follow these steps:
-        
-        1. Fork the repository.
-        2. Create a new branch for your feature or bugfix.
-        3. Make your changes, and ensure that the code follows PEP 8 guidelines.
-        4. Submit a pull request to the main repository.
-        
-        ## Support
-        
-        If you encounter any issues or have questions, please [open an issue](https://github.com/LuisSousaSilva/ds4finance/issues) on the GitHub repository.
-        
-        ## Authors
-        
-        - Luis Silva - luis_paulo_silva@hotmail.com
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# ds4finance
+
+A collection of data science tools for finance.
+
+## Installation
+
+Install the package from PyPI using pip:
+
+```python
+pip install ds4finance
+```
+
+## Usage 
+
+To use the package, import it using the alias dsf:
+
+import ds4finance as dsf
+
+### Example: Computing Standard Deviation
+
+```python
+import pandas as pd
+import ds4finance as dsf
+
+# Load or create a DataFrame containing financial data
+data = pd.read_csv("your_data.csv")
+
+# Compute the annualized standard deviation for the data
+std_dev = dsf.compute_std_dev(data)
+```
+
+## License
+
+This project is licensed under the MIT License. See the [LICENSE.txt](LICENSE.txt) file for more information.
+
+## Contributing
+
+We welcome contributions to the project. If you'd like to contribute, please follow these steps:
+
+1. Fork the repository.
+2. Create a new branch for your feature or bugfix.
+3. Make your changes, and ensure that the code follows PEP 8 guidelines.
+4. Submit a pull request to the main repository.
+
+## Support
+
+If you encounter any issues or have questions, please [open an issue](https://github.com/LuisSousaSilva/ds4finance/issues) on the GitHub repository.
+
+## Authors
+
+- Luis Silva - luis_paulo_silva@hotmail.com
```

### Comparing `ds4finance-0.1.15/README.md` & `ds4finance-0.1.17/README.md`

 * *Files identical despite different names*

### Comparing `ds4finance-0.1.15/ds4finance/__init__.py` & `ds4finance-0.1.17/ds4finance/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,8 +11,9 @@
 from .functions import compute_drawdowns_i  # noqa: F401
 from .functions import compute_drawdowns_periods  # noqa: F401
 from .functions import compute_max_drawdown_in_period  # noqa: F401
 from .functions import compute_drawdowns_min  # noqa: F401
 from .functions import compute_drawdowns_table  # noqa: F401
 from .functions import merge_time_series  # noqa: F401
 from .functions import ichart  # noqa: F401
-from .functions import compute_time_series  # noqa: F401
+from .functions import compute_time_series  # noqa: F401
+from .functions import compute_portfolio  # noqa: F401
```

### Comparing `ds4finance-0.1.15/ds4finance/functions.py` & `ds4finance-0.1.17/ds4finance/functions.py`

 * *Files 10% similar despite different names*

```diff
@@ -897,8 +897,112 @@
         A pandas DataFrame containing the growth time series for each column in the input DataFrame.
     """
     # Validate input
     if not isinstance(dataframe, pd.DataFrame):
         raise TypeError("Input 'dataframe' must be a pandas DataFrame.")
 
     # Calculate growth time series
-    return (np.exp(np.log1p(dataframe).cumsum())) * start_value
+    return (np.exp(np.log1p(dataframe).cumsum())) * start_value
+
+def compute_portfolio(quotes, weights):
+    
+    Nomes=quotes.columns
+    
+    # Anos do Portfolio
+    Years = quotes.index.year.unique()
+
+    # Dicionário com Dataframes anuais das cotações dos quotes
+    Years_dict = {}
+    k = 0
+
+    for Year in Years:
+        # Dynamically create key
+        key = Year
+        # Calculate value
+        value = quotes.loc[str(Year)]
+        # Insert in dictionary
+        Years_dict[key] = value
+        # Counter
+        k += 1
+
+    # Dicionário com Dataframes anuais das cotações dos quotes
+    Quotes_dict = {}
+    Portfolio_dict = {}
+
+    k = 0    
+    
+    for Year in Years:
+        
+        n = 0
+        
+        #Setting Portfolio to be a Global Variable
+        global Portfolio
+        
+        # Dynamically create key
+        key = Year
+
+        # Calculate value
+        if (Year-1) in Years:
+            value = Years_dict[Year].append(Years_dict[Year-1].iloc[[-1]]).sort_index()
+        else:
+            value = Years_dict[Year].append(Years_dict[Year].iloc[[-1]]).sort_index()
+
+        # Set beginning value to 100
+        value = (value / value.iloc[0]) * 100
+        # 
+        for column in value.columns:
+            value[column] = value[column] * weights[n]
+            n +=1
+        
+        # Get Returns
+        Returns = value.pct_change()
+        # Calculating Portfolio Value
+        value['Portfolio'] = value.sum(axis=1)
+
+        # Creating Weights_EOP empty DataFrame
+        Weights_EOP = pd.DataFrame()
+        # Calculating End Of Period weights
+        for Name in Nomes:
+            Weights_EOP[Name] = value[Name] / value['Portfolio']
+        # Calculating Beginning Of Period weights
+        Weights_BOP = Weights_EOP.shift(periods=1)
+
+        # Calculatins Portfolio Value
+        Portfolio = pd.DataFrame(Weights_BOP.multiply(Returns).sum(axis=1))
+        Portfolio.columns=['Simple']
+        # Transformar os simple returns em log returns 
+        Portfolio['Log'] = np.log(Portfolio['Simple'] + 1)
+        # Cumsum() dos log returns para obter o preço do Portfolio 
+        Portfolio['Price'] = 100*np.exp(np.nan_to_num(Portfolio['Log'].cumsum()))
+        Portfolio['Price'] = Portfolio['Price']   
+
+        # Insert in dictionaries
+        Quotes_dict[key] = value
+        Portfolio_dict[key] = Portfolio
+        # Counter
+        k += 1
+
+    # Making an empty Dataframe for Portfolio data
+    Portfolio = pd.DataFrame()
+
+    for Year in Years:
+        Portfolio = pd.concat([Portfolio, Portfolio_dict[Year]['Log']])
+
+    # Delete repeated index values in Portfolio    
+    Portfolio.drop_duplicates(keep='last')
+
+    # Naming the column of log returns 'Log'
+    Portfolio.columns= ['Log']
+
+    # Cumsum() dos log returns para obter o preço do Portfolio 
+    Portfolio['Price'] = 100*np.exp(np.nan_to_num(Portfolio['Log'].cumsum()))
+        
+    # Round Portfolio to 2 decimals and eliminate returns
+    Portfolio = pd.DataFrame(round(Portfolio['Price'], 2))
+
+    # Naming the column of Portfolio as 'Portfolio'
+    Portfolio.columns= ['Portfolio']
+
+    # Delete repeated days
+    Portfolio = Portfolio.loc[~Portfolio.index.duplicated(keep='first')]
+
+    return Portfolio
```

### Comparing `ds4finance-0.1.15/ds4finance.egg-info/PKG-INFO` & `ds4finance-0.1.17/ds4finance.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,75 +1,75 @@
 Metadata-Version: 2.1
 Name: ds4finance
-Version: 0.1.15
+Version: 0.1.17
 Summary: A collection of data science tools for finance
 Home-page: https://github.com/LuisSousaSilva/ds4finance
 Author: Luis Silva
 Author-email: luis_paulo_silva@hotmail.com
 License: MIT
-Description: # ds4finance
-        
-        A collection of data science tools for finance.
-        
-        ## Installation
-        
-        Install the package from PyPI using pip:
-        
-        ```python
-        pip install ds4finance
-        ```
-        
-        ## Usage 
-        
-        To use the package, import it using the alias dsf:
-        
-        import ds4finance as dsf
-        
-        ### Example: Computing Standard Deviation
-        
-        ```python
-        import pandas as pd
-        import ds4finance as dsf
-        
-        # Load or create a DataFrame containing financial data
-        data = pd.read_csv("your_data.csv")
-        
-        # Compute the annualized standard deviation for the data
-        std_dev = dsf.compute_std_dev(data)
-        ```
-        
-        ## License
-        
-        This project is licensed under the MIT License. See the [LICENSE.txt](LICENSE.txt) file for more information.
-        
-        ## Contributing
-        
-        We welcome contributions to the project. If you'd like to contribute, please follow these steps:
-        
-        1. Fork the repository.
-        2. Create a new branch for your feature or bugfix.
-        3. Make your changes, and ensure that the code follows PEP 8 guidelines.
-        4. Submit a pull request to the main repository.
-        
-        ## Support
-        
-        If you encounter any issues or have questions, please [open an issue](https://github.com/LuisSousaSilva/ds4finance/issues) on the GitHub repository.
-        
-        ## Authors
-        
-        - Luis Silva - luis_paulo_silva@hotmail.com
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# ds4finance
+
+A collection of data science tools for finance.
+
+## Installation
+
+Install the package from PyPI using pip:
+
+```python
+pip install ds4finance
+```
+
+## Usage 
+
+To use the package, import it using the alias dsf:
+
+import ds4finance as dsf
+
+### Example: Computing Standard Deviation
+
+```python
+import pandas as pd
+import ds4finance as dsf
+
+# Load or create a DataFrame containing financial data
+data = pd.read_csv("your_data.csv")
+
+# Compute the annualized standard deviation for the data
+std_dev = dsf.compute_std_dev(data)
+```
+
+## License
+
+This project is licensed under the MIT License. See the [LICENSE.txt](LICENSE.txt) file for more information.
+
+## Contributing
+
+We welcome contributions to the project. If you'd like to contribute, please follow these steps:
+
+1. Fork the repository.
+2. Create a new branch for your feature or bugfix.
+3. Make your changes, and ensure that the code follows PEP 8 guidelines.
+4. Submit a pull request to the main repository.
+
+## Support
+
+If you encounter any issues or have questions, please [open an issue](https://github.com/LuisSousaSilva/ds4finance/issues) on the GitHub repository.
+
+## Authors
+
+- Luis Silva - luis_paulo_silva@hotmail.com
```

### Comparing `ds4finance-0.1.15/setup.py` & `ds4finance-0.1.17/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 
 setup(
     name="ds4finance",
-    version="0.1.15",
+    version="0.1.17",
     description="A collection of data science tools for finance",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     author="Luis Silva",
     author_email="luis_paulo_silva@hotmail.com",
     url="https://github.com/LuisSousaSilva/ds4finance",
     packages=find_packages(),
     install_requires=["numpy", "pandas"],
     license="MIT",
     classifiers=[
-        "Development Status :: 1 - Planning",
+        "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Financial and Insurance Industry",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
```

