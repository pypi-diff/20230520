# Comparing `tmp/transaction-accounts-0.1.3.tar.gz` & `tmp/transaction-accounts-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transaction-accounts-0.1.3.tar", last modified: Mon May 15 04:09:37 2023, max compression
+gzip compressed data, was "transaction-accounts-0.2.0.tar", last modified: Sat May 20 14:32:40 2023, max compression
```

## Comparing `transaction-accounts-0.1.3.tar` & `transaction-accounts-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-05-15 04:09:37.012588 transaction-accounts-0.1.3/
--rw-r--r--   0 igormusic   (501) staff       (20)     1066 2023-04-22 05:45:17.000000 transaction-accounts-0.1.3/LICENSE.txt
--rw-r--r--   0 igormusic   (501) staff       (20)     7342 2023-05-15 04:09:37.012729 transaction-accounts-0.1.3/PKG-INFO
-drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-05-15 04:09:37.003661 transaction-accounts-0.1.3/accounts/
--rw-r--r--   0 igormusic   (501) staff       (20)        0 2023-04-22 04:58:04.000000 transaction-accounts-0.1.3/accounts/__init__.py
--rw-r--r--   0 igormusic   (501) staff       (20)    10292 2023-05-03 05:01:15.000000 transaction-accounts-0.1.3/accounts/metadata.py
--rw-r--r--   0 igormusic   (501) staff       (20)    21745 2023-05-15 04:05:33.000000 transaction-accounts-0.1.3/accounts/runtime.py
--rw-r--r--   0 igormusic   (501) staff       (20)      201 2023-04-24 01:19:31.000000 transaction-accounts-0.1.3/accounts/utility.py
--rw-r--r--   0 igormusic   (501) staff       (20)       79 2023-05-15 04:09:37.013797 transaction-accounts-0.1.3/setup.cfg
--rw-r--r--   0 igormusic   (501) staff       (20)     7631 2023-05-15 04:09:36.000000 transaction-accounts-0.1.3/setup.py
-drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-05-15 04:09:37.010083 transaction-accounts-0.1.3/tests/
--rw-r--r--   0 igormusic   (501) staff       (20)     2834 2023-04-27 01:51:20.000000 transaction-accounts-0.1.3/tests/test_calendar.py
--rw-r--r--   0 igormusic   (501) staff       (20)    18462 2023-05-03 03:32:40.000000 transaction-accounts-0.1.3/tests/test_config.py
--rw-r--r--   0 igormusic   (501) staff       (20)     1054 2023-05-01 04:20:09.000000 transaction-accounts-0.1.3/tests/test_configuration.py
--rw-r--r--   0 igormusic   (501) staff       (20)     4595 2023-05-15 03:57:18.000000 transaction-accounts-0.1.3/tests/test_loanGiven.py
--rw-r--r--   0 igormusic   (501) staff       (20)     2197 2023-04-24 02:01:02.000000 transaction-accounts-0.1.3/tests/test_rate_type.py
--rw-r--r--   0 igormusic   (501) staff       (20)     6171 2023-05-01 09:24:39.000000 transaction-accounts-0.1.3/tests/test_runtime.py
--rw-r--r--   0 igormusic   (501) staff       (20)     3942 2023-04-23 19:46:30.000000 transaction-accounts-0.1.3/tests/test_schedule.py
-drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-05-15 04:09:37.012290 transaction-accounts-0.1.3/transaction_accounts.egg-info/
--rw-r--r--   0 igormusic   (501) staff       (20)     7342 2023-05-15 04:09:36.000000 transaction-accounts-0.1.3/transaction_accounts.egg-info/PKG-INFO
--rw-r--r--   0 igormusic   (501) staff       (20)      496 2023-05-15 04:09:36.000000 transaction-accounts-0.1.3/transaction_accounts.egg-info/SOURCES.txt
--rw-r--r--   0 igormusic   (501) staff       (20)        1 2023-05-15 04:09:36.000000 transaction-accounts-0.1.3/transaction_accounts.egg-info/dependency_links.txt
--rw-r--r--   0 igormusic   (501) staff       (20)       31 2023-05-15 04:09:36.000000 transaction-accounts-0.1.3/transaction_accounts.egg-info/requires.txt
--rw-r--r--   0 igormusic   (501) staff       (20)        9 2023-05-15 04:09:36.000000 transaction-accounts-0.1.3/transaction_accounts.egg-info/top_level.txt
+drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-05-20 14:32:40.340746 transaction-accounts-0.2.0/
+-rw-r--r--   0 igormusic   (501) staff       (20)     1066 2023-04-22 05:45:17.000000 transaction-accounts-0.2.0/LICENSE.txt
+-rw-r--r--   0 igormusic   (501) staff       (20)     7342 2023-05-20 14:32:40.340894 transaction-accounts-0.2.0/PKG-INFO
+drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-05-20 14:32:40.331696 transaction-accounts-0.2.0/accounts/
+-rw-r--r--   0 igormusic   (501) staff       (20)        0 2023-04-22 04:58:04.000000 transaction-accounts-0.2.0/accounts/__init__.py
+-rw-r--r--   0 igormusic   (501) staff       (20)    10292 2023-05-03 05:01:15.000000 transaction-accounts-0.2.0/accounts/metadata.py
+-rw-r--r--   0 igormusic   (501) staff       (20)    21392 2023-05-20 14:27:48.000000 transaction-accounts-0.2.0/accounts/runtime.py
+-rw-r--r--   0 igormusic   (501) staff       (20)      201 2023-04-24 01:19:31.000000 transaction-accounts-0.2.0/accounts/utility.py
+-rw-r--r--   0 igormusic   (501) staff       (20)       79 2023-05-20 14:32:40.341443 transaction-accounts-0.2.0/setup.cfg
+-rw-r--r--   0 igormusic   (501) staff       (20)     7631 2023-05-20 14:32:39.000000 transaction-accounts-0.2.0/setup.py
+drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-05-20 14:32:40.337038 transaction-accounts-0.2.0/tests/
+-rw-r--r--   0 igormusic   (501) staff       (20)     2834 2023-04-27 01:51:20.000000 transaction-accounts-0.2.0/tests/test_calendar.py
+-rw-r--r--   0 igormusic   (501) staff       (20)    18462 2023-05-03 03:32:40.000000 transaction-accounts-0.2.0/tests/test_config.py
+-rw-r--r--   0 igormusic   (501) staff       (20)     1054 2023-05-01 04:20:09.000000 transaction-accounts-0.2.0/tests/test_configuration.py
+-rw-r--r--   0 igormusic   (501) staff       (20)     4673 2023-05-20 14:28:42.000000 transaction-accounts-0.2.0/tests/test_loanGiven.py
+-rw-r--r--   0 igormusic   (501) staff       (20)     2197 2023-04-24 02:01:02.000000 transaction-accounts-0.2.0/tests/test_rate_type.py
+-rw-r--r--   0 igormusic   (501) staff       (20)     6240 2023-05-20 14:31:40.000000 transaction-accounts-0.2.0/tests/test_runtime.py
+-rw-r--r--   0 igormusic   (501) staff       (20)     3942 2023-04-23 19:46:30.000000 transaction-accounts-0.2.0/tests/test_schedule.py
+drwxr-xr-x   0 igormusic   (501) staff       (20)        0 2023-05-20 14:32:40.340371 transaction-accounts-0.2.0/transaction_accounts.egg-info/
+-rw-r--r--   0 igormusic   (501) staff       (20)     7342 2023-05-20 14:32:40.000000 transaction-accounts-0.2.0/transaction_accounts.egg-info/PKG-INFO
+-rw-r--r--   0 igormusic   (501) staff       (20)      496 2023-05-20 14:32:40.000000 transaction-accounts-0.2.0/transaction_accounts.egg-info/SOURCES.txt
+-rw-r--r--   0 igormusic   (501) staff       (20)        1 2023-05-20 14:32:40.000000 transaction-accounts-0.2.0/transaction_accounts.egg-info/dependency_links.txt
+-rw-r--r--   0 igormusic   (501) staff       (20)       31 2023-05-20 14:32:40.000000 transaction-accounts-0.2.0/transaction_accounts.egg-info/requires.txt
+-rw-r--r--   0 igormusic   (501) staff       (20)        9 2023-05-20 14:32:40.000000 transaction-accounts-0.2.0/transaction_accounts.egg-info/top_level.txt
```

### Comparing `transaction-accounts-0.1.3/LICENSE.txt` & `transaction-accounts-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `transaction-accounts-0.1.3/PKG-INFO` & `transaction-accounts-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transaction-accounts
-Version: 0.1.3
+Version: 0.2.0
 Summary: Create configuration for transactional accounts and implement account runtime
 Home-page: https://github.com/igormusic/transaction-accounts
 Download-URL: https://github.com/igormusic/transaction-accounts/archive/refs/tags/0.0.6.tar.gz
 Author: Igor Music
 Author-email: igormusich@gmail.com
 License: MIT
 Keywords: TRANSACTION PROCESSING,LOANS,SAVINGS,ACCOUNTS,FINANCE,BANKING
```

### Comparing `transaction-accounts-0.1.3/accounts/metadata.py` & `transaction-accounts-0.2.0/accounts/metadata.py`

 * *Files identical despite different names*

### Comparing `transaction-accounts-0.1.3/accounts/runtime.py` & `transaction-accounts-0.2.0/accounts/runtime.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     frequency: ScheduleFrequency
     interval: int = 0,
     adjustment: BusinessDayAdjustment = BusinessDayAdjustment.NO_ADJUSTMENT
     end_date: Optional[date]
     number_of_repeats: int = 0
     include_dates: list[date] = []
     exclude_dates: list[date] = []
-    cached_dates: dict[date, date] = Field(default_factory=dict,  exclude=True)
+    cached_dates: dict[date, date] = Field(default_factory=dict, exclude=True)
 
     class Config:
         # exclude the "cached_dates" field from JSON serialization
         exclude = {"cached_dates"}
 
     def __is_simple_daily_schedule(self):
         return (self.frequency == ScheduleFrequency.DAILY and
@@ -317,39 +317,29 @@
                 value_date=value_date,
                 transaction_type=transaction_type,
                 amount=new_amount - original_amount,
                 original=original_transactions,
                 new=new_transactions)
 
 
-class TransactionTrace:
+class TransactionTrace(BaseModel):
     transaction: Transaction
     positions: Dict[str, Decimal]
 
-    def __init__(self, transaction: Transaction, positions: Dict[str, Decimal]):
-        self.transaction = transaction
-        self.positions = positions
-
     def __str__(self):
         return f" {self.transaction.value_date} {self.transaction.transaction_type} {self.transaction.amount} {self.positions}"
 
 
-class AccountValuation:
+class AccountValuation(BaseModel):
     account: Account
     account_type: AccountType
     action_date: date
-    trace: bool
+    trace: bool = False
     trace_list: List[TransactionTrace] = []
 
-    def __init__(self, account: Account, account_type: AccountType, action_date: date, trace: bool = False):
-        self.account = account
-        self.account_type = account_type
-        self.action_date = action_date
-        self.trace = trace
-
     def init_account(self):
         # reset all positions to zero
         for position in self.account.positions.values():
             position.amount = Decimal(0)
 
         self.account.transactions = []
 
@@ -423,15 +413,15 @@
         transaction = Transaction(action_date=self.action_date, value_date=value_date,
                                   transaction_type=transaction_type.name,
                                   amount=amount, system_generated=system_generated)
 
         positions = self.account.add_transaction(transaction, transaction_type)
 
         if self.trace:
-            self.trace_list.append(TransactionTrace(transaction, positions))
+            self.trace_list.append(TransactionTrace(transaction=transaction, positions=positions))
 
         triggered_transaction = self.account_type.get_trigger_transaction(transaction_type.name)
 
         if triggered_transaction:
             trigger_amount = self.account.evaluate(triggered_transaction.amount_expression,
                                                    {"transaction": transaction,
                                                     "accountType": self.account_type,
```

### Comparing `transaction-accounts-0.1.3/setup.py` & `transaction-accounts-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='transaction-accounts',
-    version='0.1.3',
+    version='0.2.0',
     description='Create configuration for transactional accounts and implement account runtime',
     long_description='''
 Transaction Accounts
 ====================
 
 This library provides basic functionality for working with transaction accounts.
```

### Comparing `transaction-accounts-0.1.3/tests/test_calendar.py` & `transaction-accounts-0.2.0/tests/test_calendar.py`

 * *Files identical despite different names*

### Comparing `transaction-accounts-0.1.3/tests/test_config.py` & `transaction-accounts-0.2.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `transaction-accounts-0.1.3/tests/test_configuration.py` & `transaction-accounts-0.2.0/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `transaction-accounts-0.1.3/tests/test_loanGiven.py` & `transaction-accounts-0.2.0/tests/test_loanGiven.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,26 +105,26 @@
         self.assertRaises(ValueError, create_without_mandatory_properties)
 
     def test_forecast(self):
         account_type = create_loan_given_account()
 
         account, end_date = create_loan_account(account_type, date(2013, 3, 8))
 
-        valuation = AccountValuation(account, account_type, end_date, True)
+        valuation = AccountValuation(account=account, account_type=account_type, action_date=end_date, trace=True)
 
         valuation.forecast(end_date + relativedelta(days=1), [])
 
         self.assertEqual(5, len(account.positions.keys()))
         self.assertAlmostEqual(Decimal(1333778.93), account.positions["principal"].amount, places=2)
         self.assertAlmostEqual(Decimal(709778.93), account.positions["interest_capitalized"].amount, places=2)
         self.assertAlmostEqual(Decimal(0.005), account.positions["accrued"].amount, places=2)
 
     def test_installments(self):
         account_type = create_loan_given_account()
 
         account, end_date = create_loan_account(account_type, date(2013, 3, 8))
 
-        valuation = AccountValuation(account, account_type, end_date, False)
+        valuation = AccountValuation(account=account, account_type=account_type, action_date=end_date, trace=False)
 
         payment = valuation.solve_instalment()
 
         self.assertAlmostEqual(Decimal(2964.37), Decimal(payment), places=2)
```

### Comparing `transaction-accounts-0.1.3/tests/test_rate_type.py` & `transaction-accounts-0.2.0/tests/test_rate_type.py`

 * *Files identical despite different names*

### Comparing `transaction-accounts-0.1.3/tests/test_runtime.py` & `transaction-accounts-0.2.0/tests/test_runtime.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
                      withholding_tax: Decimal) -> Account:
     start_date = date(2019, 1, 1)
     account = Account(start_date=start_date, account_type_name=account_type.name,
                       account_type=account_type,
                       properties={"monthlyFee": PropertyValue(value={start_date: monthly_fee}),
                                   "withholdingTax": PropertyValue(value={start_date: withholding_tax})})
 
-    valuation = AccountValuation(account, account_type, date(2020, 1, 1))
+    valuation = AccountValuation(account= account, account_type= account_type, action_date= date(2020, 1, 1))
     deposit_transaction_type = account_type.get_transaction_type("deposit")
     external_transactions = group_by_date([
         ExternalTransaction(transaction_type_name=deposit_transaction_type.name,
                             amount=deposit, value_date=date(2019, 1, 1))])
 
     valuation.forecast(date(2020, 1, 1), external_transactions)
     return account
@@ -28,15 +28,15 @@
     start_date = date(2019, 1, 1)
     account = Account(start_date=start_date, account_type_name=account_type.name,
                       account_type=account_type,
                       properties={"monthlyFee": PropertyValue(value={start_date: monthly_fee}),
                                   "withholdingTax": PropertyValue(value={start_date: withholding_tax1,
                                                                          tax_change_date: withholding_tax2})})
 
-    valuation = AccountValuation(account, account_type, date(2020, 1, 1))
+    valuation = AccountValuation(account=account, account_type=account_type, action_date=date(2020, 1, 1))
     deposit_transaction_type = account_type.get_transaction_type("deposit")
     external_transactions = group_by_date([
         ExternalTransaction(transaction_type_name=deposit_transaction_type.name,
                             amount=deposit, value_date=date(2019, 1, 1))])
 
     valuation.forecast(date(2020, 1, 1), external_transactions)
     return account
```

### Comparing `transaction-accounts-0.1.3/tests/test_schedule.py` & `transaction-accounts-0.2.0/tests/test_schedule.py`

 * *Files identical despite different names*

### Comparing `transaction-accounts-0.1.3/transaction_accounts.egg-info/PKG-INFO` & `transaction-accounts-0.2.0/transaction_accounts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transaction-accounts
-Version: 0.1.3
+Version: 0.2.0
 Summary: Create configuration for transactional accounts and implement account runtime
 Home-page: https://github.com/igormusic/transaction-accounts
 Download-URL: https://github.com/igormusic/transaction-accounts/archive/refs/tags/0.0.6.tar.gz
 Author: Igor Music
 Author-email: igormusich@gmail.com
 License: MIT
 Keywords: TRANSACTION PROCESSING,LOANS,SAVINGS,ACCOUNTS,FINANCE,BANKING
```

