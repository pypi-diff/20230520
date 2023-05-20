# Comparing `tmp/cardlinky-1.6.1.tar.gz` & `tmp/cardlinky-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cardlinky-1.6.1.tar", max compression
+gzip compressed data, was "cardlinky-1.7.tar", max compression
```

## Comparing `cardlinky-1.6.1.tar` & `cardlinky-1.7.tar`

### file list

```diff
@@ -1,33 +1,30 @@
--rw-r--r--   0        0        0       35 2023-02-11 11:14:41.154873 cardlinky-1.6.1/cardlinky/__init__.py
--rw-r--r--   0        0        0    15436 2023-02-13 17:39:13.401125 cardlinky-1.6.1/cardlinky/cardlinky.py
--rw-r--r--   0        0        0      367 2023-02-11 18:55:50.554958 cardlinky-1.6.1/cardlinky/types/__init__.py
--rw-r--r--   0        0        0      492 2023-02-11 19:54:19.003399 cardlinky-1.6.1/cardlinky/types/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     5088 2023-02-11 19:54:19.099787 cardlinky-1.6.1/cardlinky/types/__pycache__/exceptions.cpython-38.pyc
--rw-r--r--   0        0        0        0 2023-02-06 14:24:03.122143 cardlinky-1.6.1/cardlinky/types/enums/__init__.py
--rw-r--r--   0        0        0      158 2023-02-11 19:54:19.006960 cardlinky-1.6.1/cardlinky/types/enums/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      431 2023-02-11 19:54:19.056544 cardlinky-1.6.1/cardlinky/types/enums/__pycache__/account_type.cpython-38.pyc
--rw-r--r--   0        0        0      700 2023-02-11 19:54:19.053986 cardlinky-1.6.1/cardlinky/types/enums/__pycache__/bill_type.cpython-38.pyc
--rw-r--r--   0        0        0      464 2023-02-11 19:54:19.050959 cardlinky-1.6.1/cardlinky/types/enums/__pycache__/currency.cpython-38.pyc
--rw-r--r--   0        0        0      650 2023-02-11 19:54:19.047982 cardlinky-1.6.1/cardlinky/types/enums/__pycache__/enum.cpython-38.pyc
--rw-r--r--   0        0        0      638 2023-02-11 19:54:19.009959 cardlinky-1.6.1/cardlinky/types/enums/__pycache__/status.cpython-38.pyc
--rw-r--r--   0        0        0      113 2023-02-11 19:45:43.025791 cardlinky-1.6.1/cardlinky/types/enums/account_type.py
--rw-r--r--   0        0        0      379 2023-02-13 17:37:54.678912 cardlinky-1.6.1/cardlinky/types/enums/bill_type.py
--rw-r--r--   0        0        0      138 2023-02-11 19:45:48.037121 cardlinky-1.6.1/cardlinky/types/enums/currency.py
--rw-r--r--   0        0        0      323 2023-02-13 17:50:08.408460 cardlinky-1.6.1/cardlinky/types/enums/enum.py
--rw-r--r--   0        0        0      336 2023-02-11 19:39:59.441413 cardlinky-1.6.1/cardlinky/types/enums/status.py
--rw-r--r--   0        0        0     3383 2023-02-11 18:54:41.059371 cardlinky-1.6.1/cardlinky/types/exceptions.py
--rw-r--r--   0        0        0        0 2023-02-06 14:36:33.956320 cardlinky-1.6.1/cardlinky/types/models/__init__.py
--rw-r--r--   0        0        0      159 2023-02-11 19:54:19.058708 cardlinky-1.6.1/cardlinky/types/models/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      783 2023-02-11 19:54:19.096790 cardlinky-1.6.1/cardlinky/types/models/__pycache__/balance.cpython-38.pyc
--rw-r--r--   0        0        0     3384 2023-02-11 19:54:19.062689 cardlinky-1.6.1/cardlinky/types/models/__pycache__/bill.cpython-38.pyc
--rw-r--r--   0        0        0     2314 2023-02-11 19:54:19.093170 cardlinky-1.6.1/cardlinky/types/models/__pycache__/payment.cpython-38.pyc
--rw-r--r--   0        0        0     1772 2023-02-11 19:54:19.090171 cardlinky-1.6.1/cardlinky/types/models/__pycache__/payout.cpython-38.pyc
--rw-r--r--   0        0        0      459 2023-02-11 18:55:29.826037 cardlinky-1.6.1/cardlinky/types/models/balance.py
--rw-r--r--   0        0        0     2785 2023-02-11 18:55:23.023896 cardlinky-1.6.1/cardlinky/types/models/bill.py
--rw-r--r--   0        0        0     2150 2023-02-14 12:48:48.774932 cardlinky-1.6.1/cardlinky/types/models/payment.py
--rw-r--r--   0        0        0     1351 2023-02-11 18:54:19.641530 cardlinky-1.6.1/cardlinky/types/models/payout.py
--rw-r--r--   0        0        0     1087 2023-02-11 14:00:50.493646 cardlinky-1.6.1/LICENSE
--rw-r--r--   0        0        0      560 2023-02-14 12:49:46.295779 cardlinky-1.6.1/pyproject.toml
--rw-r--r--   0        0        0     1691 2023-02-13 17:41:32.576211 cardlinky-1.6.1/README.md
--rw-r--r--   0        0        0     2421 1970-01-01 00:00:00.000000 cardlinky-1.6.1/setup.py
--rw-r--r--   0        0        0     2456 1970-01-01 00:00:00.000000 cardlinky-1.6.1/PKG-INFO
+-rw-r--r--   0        0        0       35 2023-05-20 19:31:20.496747 cardlinky-1.7/cardlinky/__init__.py
+-rw-r--r--   0        0        0    15104 2023-05-20 19:52:41.103901 cardlinky-1.7/cardlinky/cardlinky.py
+-rw-r--r--   0        0        0      367 2023-05-20 19:31:20.497750 cardlinky-1.7/cardlinky/types/__init__.py
+-rw-r--r--   0        0        0      580 2023-05-20 19:46:35.681938 cardlinky-1.7/cardlinky/types/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0        0 2023-05-20 19:31:20.497750 cardlinky-1.7/cardlinky/types/enums/__init__.py
+-rw-r--r--   0        0        0      168 2023-05-20 19:46:35.682940 cardlinky-1.7/cardlinky/types/enums/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      548 2023-05-20 19:46:35.688104 cardlinky-1.7/cardlinky/types/enums/__pycache__/account_type.cpython-311.pyc
+-rw-r--r--   0        0        0      858 2023-05-20 19:46:35.686973 cardlinky-1.7/cardlinky/types/enums/__pycache__/bill_type.cpython-311.pyc
+-rw-r--r--   0        0        0      613 2023-05-20 19:46:35.685675 cardlinky-1.7/cardlinky/types/enums/__pycache__/currency.cpython-311.pyc
+-rw-r--r--   0        0        0      980 2023-05-20 19:46:35.685675 cardlinky-1.7/cardlinky/types/enums/__pycache__/enum.cpython-311.pyc
+-rw-r--r--   0        0        0      883 2023-05-20 19:46:35.684229 cardlinky-1.7/cardlinky/types/enums/__pycache__/status.cpython-311.pyc
+-rw-r--r--   0        0        0      113 2023-05-20 19:31:20.497750 cardlinky-1.7/cardlinky/types/enums/account_type.py
+-rw-r--r--   0        0        0      379 2023-05-20 19:31:20.497750 cardlinky-1.7/cardlinky/types/enums/bill_type.py
+-rw-r--r--   0        0        0      138 2023-05-20 19:31:20.497750 cardlinky-1.7/cardlinky/types/enums/currency.py
+-rw-r--r--   0        0        0      323 2023-05-20 19:31:20.498823 cardlinky-1.7/cardlinky/types/enums/enum.py
+-rw-r--r--   0        0        0      336 2023-05-20 19:31:20.498823 cardlinky-1.7/cardlinky/types/enums/status.py
+-rw-r--r--   0        0        0        0 2023-05-20 19:31:20.498823 cardlinky-1.7/cardlinky/types/models/__init__.py
+-rw-r--r--   0        0        0      169 2023-05-20 19:46:35.689106 cardlinky-1.7/cardlinky/types/models/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      951 2023-05-20 19:46:35.743241 cardlinky-1.7/cardlinky/types/models/__pycache__/balance.cpython-311.pyc
+-rw-r--r--   0        0        0     4071 2023-05-20 19:46:35.690106 cardlinky-1.7/cardlinky/types/models/__pycache__/bill.cpython-311.pyc
+-rw-r--r--   0        0        0     3075 2023-05-20 19:46:35.740650 cardlinky-1.7/cardlinky/types/models/__pycache__/payment.cpython-311.pyc
+-rw-r--r--   0        0        0     2173 2023-05-20 19:46:35.738317 cardlinky-1.7/cardlinky/types/models/__pycache__/payout.cpython-311.pyc
+-rw-r--r--   0        0        0      455 2023-05-20 19:35:03.853462 cardlinky-1.7/cardlinky/types/models/balance.py
+-rw-r--r--   0        0        0     2778 2023-05-20 19:37:10.708942 cardlinky-1.7/cardlinky/types/models/bill.py
+-rw-r--r--   0        0        0     2145 2023-05-20 19:37:58.815912 cardlinky-1.7/cardlinky/types/models/payment.py
+-rw-r--r--   0        0        0     1346 2023-05-20 19:37:58.819285 cardlinky-1.7/cardlinky/types/models/payout.py
+-rw-r--r--   0        0        0     1087 2023-05-20 19:31:20.495744 cardlinky-1.7/LICENSE
+-rw-r--r--   0        0        0      601 2023-05-20 19:49:47.232495 cardlinky-1.7/pyproject.toml
+-rw-r--r--   0        0        0     1691 2023-05-20 19:31:20.495744 cardlinky-1.7/README.md
+-rw-r--r--   0        0        0     2495 1970-01-01 00:00:00.000000 cardlinky-1.7/PKG-INFO
```

### Comparing `cardlinky-1.6.1/cardlinky/cardlinky.py` & `cardlinky-1.7/cardlinky/cardlinky.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import datetime
 import requests
 from typing import Optional, MutableMapping, Mapping, Union, Any, List
 
-from cardlinky.types.exceptions import exceptions
 from cardlinky.types.models.balance import Balance
 from cardlinky.types.models.payout import Payout, PayoutStatus
 from cardlinky.types.models.payment import Payment, PaymentStatus
 from cardlinky.types.models.bill import Bill, BillCreate, BillStatus, BillToggleActivity
 from cardlinky.types.enums.status import Status
 from cardlinky.types.enums.currency import Currency
 from cardlinky.types.enums.bill_type import BillType
@@ -32,24 +31,17 @@
         }
 
     @staticmethod
     def __handle_error(json: Mapping[str, Any]) -> None:
         if not json["success"]:
             if "errors" in tuple(json.keys()):
                 error = tuple(json["errors"].values())[0][0]
-
-                if error in tuple(exceptions.keys()):
-                    raise exceptions[tuple(json["errors"].values())[0][0]]
-                raise ValueError(error)
             else:
                 error = json["message"]
-
-                if json["message"] in tuple(exceptions.keys()):
-                    raise exceptions[json["message"]]
-                raise ValueError(error)
+            raise requests.exceptions.HTTPError(error)
 
     def _get(self, path: str, json: MutableMapping[str, Any]) -> MutableMapping[str, Any]:
         response = requests.get(
             url=self._base_url + path,
             headers=self._headers,
             json=json,
         )
```

### Comparing `cardlinky-1.6.1/cardlinky/types/models/bill.py` & `cardlinky-1.7/cardlinky/types/models/payment.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,92 +1,65 @@
 import datetime
-from dataclasses import dataclass
+from typing import Optional
+from pydantic import BaseModel
 
 from cardlinky.types.enums.status import Status
 from cardlinky.types.enums.currency import Currency
-from cardlinky.types.enums.bill_type import BillType
 
 
-@dataclass
-class Bill:
+class Payment(BaseModel):
     """
-    :param id: str - Unique bill id
-    :param status: enums.Status - Bill status
-    :param active: boll - Is bill active
-    :param amount: float - Bill amount
-    :param type: enums.BillType - Bill type. 'Normal' type accepts only one payment.
-        'Multi' type accepts unlimited number of payments.
+    :param id: str - Unique payment ID
+    :param bill_id: str - Unique bill ID
+    :param status: enums.Status - Status of payment
+    :param amount: float - Total payment amount
+    :param commission: float - Total payment commission
     :param currency_in: enums.Currency - Payment currency
+    :param account_amount: float - Total account amount
+    :param account_currency_code: enums.Currency - Account currency
+    :param from_card: str - Payer's card
     :param created_at: datetime.datetime - Creation date and time
+    :param error_code: Optional[int] - Error code
+    :param error_message: Optional[str] - Error message
     """
 
     id: str
+    bill_id: str
     status: Status
-    active: bool
     amount: float
-    type: BillType
+    commission: float
     currency_in: Currency
+    account_amount: float
+    account_currency_code: Currency
+    from_card: str
     created_at: datetime.datetime
+    error_code: Optional[int] = None
+    error_message: Optional[str] = None
 
 
-@dataclass
-class BillCreate:
+class PaymentStatus(BaseModel):
     """
-    :param success: bool - Payment status
-    :param link_url: str - Link to the page with QR-code. Example: https://cardlink.link/link/5QWlqB2kKJ
-    :param link_page_url: str - Link to the payment page. Example: https://cardlink.link/transfer/5QWlqB2kKJ
+    :param id: str - Unique payment ID
     :param bill_id: str - Unique bill ID
-    """
-
-    success: bool
-    link_url: str
-    link_page_url: str
-    bill_id: str
-
-
-@dataclass
-class BillStatus:
-    """
-    :param id: str - Unique bill id
-    :param status: enums.Status - Bill status
-    :param active: boll - Is bill active
+    :param status: enums.Status - Status of payment
     :param amount: float - Bill amount
-    :param type: enums.BillType - Bill type. 'Normal' type accepts only one payment.
-        'Multi' type accepts unlimited number of payments
+    :param commission: float - Commission amount
     :param currency_in: enums.Currency - Payment currency
+    :param account_amount: float - Total account amount
+    :param account_currency_code: enums.Currency - Account currency
+    :param from_card: str - Payer's card number
     :param created_at: datetime.datetime - Creation date and time
     :param created_at: datetime.datetime - Creation date and time
     :param success: bool - Payment status
     """
 
     id: str
+    bill_id: str
     status: Status
-    active: bool
     amount: float
-    type: BillType
+    commission: float
     currency_in: Currency
+    account_amount: float
+    account_currency_code: Currency
+    from_card: str
     created_at: datetime.datetime
     success: bool
-
-
-@dataclass
-class BillToggleActivity:
-    """
-    :param id: str - Unique bill id
-    :param active: bool - Bill activity flag
-    :param status: enums.Status - Bill status
-    :param amount: float - Bill amount
-    :param type: enums.BillType - Type of bill. NORMAL is for onetime payments and
-        MULTI is for infinity number of payments
-    :param created_at: datetime.datetime - Bill creation date and time
-    :param currency_in: enums.Currency - Currency
-    :param success: bool - This flag indicates status of request
-    """
-
-    id: str
-    active: bool
-    status: Status
-    amount: float
-    type: BillType
-    created_at: datetime.datetime
-    currency_in: Currency
-    success: bool
```

### Comparing `cardlinky-1.6.1/cardlinky/types/models/payout.py` & `cardlinky-1.7/cardlinky/types/models/payout.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import datetime
-from dataclasses import dataclass
+from pydantic import BaseModel
 
 from cardlinky.types.enums.status import Status
 from cardlinky.types.enums.currency import Currency
 
 
-@dataclass
-class Payout:
+class Payout(BaseModel):
     """
     :param id: str - Unique ID of payout
     :param status: enums.Status - Payout status
     :param amount: float - Payout amount
     :param commission: float - Fees
     :param account_identifier: str - Account to which money will be sent
     :param currency: enums.Currency - Currency
@@ -22,16 +21,15 @@
     amount: float
     commission: float
     account_identifier: str
     currency: Currency
     created_at: datetime.datetime
 
 
-@dataclass
-class PayoutStatus:
+class PayoutStatus(BaseModel):
     """
     :param id: str - Unique ID of payout
     :param status: enums.Status - Payout status
     :param amount: float - Payout amount
     :param commission: float - Fees
     :param account_identifier: str - Account to which money will be sent
     :param currency: enums.Currency - Currency
```

### Comparing `cardlinky-1.6.1/LICENSE` & `cardlinky-1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cardlinky-1.6.1/README.md` & `cardlinky-1.7/README.md`

 * *Files identical despite different names*

### Comparing `cardlinky-1.6.1/PKG-INFO` & `cardlinky-1.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: cardlinky
-Version: 1.6.1
+Version: 1.7
 Summary: Wrapper for the Cardlink API in Python
 Home-page: https://github.com/LuK050/cardlinky
 License: MIT
 Keywords: cardlink,api
 Author: LuK050
 Author-email: volychevk@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pydantic (>=4.5.0,<5.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Project-URL: Documentation, https://cardlink.link/reference/api
 Project-URL: Repository, https://github.com/LuK050/cardlinky
 Description-Content-Type: text/markdown
 
 # cardlinky
 <a href="https://pypi.org/project/cardlinky/"><img src="https://img.shields.io/pypi/v/cardlinky?style=flat-square"></a> <a href="https://pypi.org/project/cardlinky/"><img src="https://img.shields.io/pypi/dm/cardlinky?color=blue&style=flat-square"></a> <img src="https://img.shields.io/pypi/pyversions/cardlinky?style=flat-square">
```

#### html2text {}

```diff
@@ -1,20 +1,21 @@
-Metadata-Version: 2.1 Name: cardlinky Version: 1.6.1 Summary: Wrapper for the
+Metadata-Version: 2.1 Name: cardlinky Version: 1.7 Summary: Wrapper for the
 Cardlink API in Python Home-page: https://github.com/LuK050/cardlinky License:
 MIT Keywords: cardlink,api Author: LuK050 Author-email: volychevk@gmail.com
 Requires-Python: >=3.7,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: requests (>=2.28.2,<3.0.0) Project-URL: Documentation, https://
-cardlink.link/reference/api Project-URL: Repository, https://github.com/LuK050/
-cardlinky Description-Content-Type: text/markdown # cardlinky [https://
-img.shields.io/pypi/v/cardlinky?style=flat-square] [https://img.shields.io/
-pypi/dm/cardlinky?color=blue&style=flat-square] [https://img.shields.io/pypi/
+Requires-Dist: pydantic (>=4.5.0,<5.0.0) Requires-Dist: requests
+(>=2.28.2,<3.0.0) Project-URL: Documentation, https://cardlink.link/reference/
+api Project-URL: Repository, https://github.com/LuK050/cardlinky Description-
+Content-Type: text/markdown # cardlinky [https://img.shields.io/pypi/v/
+cardlinky?style=flat-square] [https://img.shields.io/pypi/dm/
+cardlinky?color=blue&style=flat-square] [https://img.shields.io/pypi/
 pyversions/cardlinky?style=flat-square] [ð Official documentation](https://
 cardlink.link/reference/api) ## Usage Firstly, you need to create an account
 and Ð° shop in https://cardlink.link/. After confirmation, you will be able to
 get a token and a shop ID to work with the API. ### Creating a bill and getting
 a payment link: ```py from cardlinky import Cardlinky def print_bill_url(token:
 str, shop_id: str, amount: float) -> None: # Creating an instance of the class
 cardlinky = Cardlinky(token) # Create a bill and save it bill =
```

