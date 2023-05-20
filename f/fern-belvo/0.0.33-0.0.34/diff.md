# Comparing `tmp/fern_belvo-0.0.33.tar.gz` & `tmp/fern_belvo-0.0.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fern_belvo-0.0.33.tar", max compression
+gzip compressed data, was "fern_belvo-0.0.34.tar", max compression
```

## Comparing `fern_belvo-0.0.33.tar` & `fern_belvo-0.0.34.tar`

### file list

```diff
@@ -1,469 +1,469 @@
--rw-r--r--   0        0        0     2460 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/README.md
--rw-r--r--   0        0        0      371 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/pyproject.toml
--rw-r--r--   0        0        0    27716 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/__init__.py
--rw-r--r--   0        0        0    12781 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/client.py
--rw-r--r--   0        0        0      348 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/core/__init__.py
--rw-r--r--   0        0        0      426 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      247 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/environment.py
--rw-r--r--   0        0        0      594 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/errors/__init__.py
--rw-r--r--   0        0        0      346 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/errors/bad_request_error.py
--rw-r--r--   0        0        0      341 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/errors/forbidden_error.py
--rw-r--r--   0        0        0      323 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/errors/internal_server_error.py
--rw-r--r--   0        0        0      325 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/errors/not_found_error.py
--rw-r--r--   0        0        0      340 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/errors/precondition_error.py
--rw-r--r--   0        0        0      349 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/errors/request_timeout_error.py
--rw-r--r--   0        0        0      340 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/errors/unauthorized_error.py
--rw-r--r--   0        0        0        0 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/py.typed
--rw-r--r--   0        0        0     1252 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/resources/accounts/__init__.py
--rw-r--r--   0        0        0    24969 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/resources/accounts/client.py
--rw-r--r--   0        0        0       65 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/resources/balances/__init__.py
--rw-r--r--   0        0        0    23438 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/resources/balances/client.py
--rw-r--r--   0        0        0       65 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/resources/bank_accounts/__init__.py
--rw-r--r--   0        0        0    12881 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/resources/bank_accounts/client.py
--rw-r--r--   0        0        0       65 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/resources/categorization/__init__.py
--rw-r--r--   0        0        0     5136 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/resources/categorization/client.py
--rw-r--r--   0        0        0       65 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/resources/customers/__init__.py
--rw-r--r--   0        0        0    11285 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/resources/customers/client.py
--rw-r--r--   0        0        0       65 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/resources/employment_records/__init__.py
--rw-r--r--   0        0        0    14543 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/resources/employment_records/client.py
--rw-r--r--   0        0        0       65 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/resources/income_verification/__init__.py
--rw-r--r--   0        0        0     7011 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/resources/income_verification/client.py
--rw-r--r--   0        0        0       65 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/resources/incomes/__init__.py
--rw-r--r--   0        0        0    20690 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/resources/incomes/client.py
--rw-r--r--   0        0        0       65 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/resources/institutions/__init__.py
--rw-r--r--   0        0        0     8765 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/resources/institutions/client.py
--rw-r--r--   0        0        0       65 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/resources/investment_portfolios/__init__.py
--rw-r--r--   0        0        0    18632 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/resources/investment_portfolios/client.py
--rw-r--r--   0        0        0       65 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/resources/invoices/__init__.py
--rw-r--r--   0        0        0    24516 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/resources/invoices/client.py
--rw-r--r--   0        0        0       65 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/resources/links/__init__.py
--rw-r--r--   0        0        0    33898 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/resources/links/client.py
--rw-r--r--   0        0        0       65 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/resources/owners/__init__.py
--rw-r--r--   0        0        0    19773 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/resources/owners/client.py
--rw-r--r--   0        0        0       65 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/resources/payment_institutions/__init__.py
--rw-r--r--   0        0        0     7761 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/resources/payment_institutions/client.py
--rw-r--r--   0        0        0       65 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/resources/payment_intents/__init__.py
--rw-r--r--   0        0        0    16753 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/resources/payment_intents/client.py
--rw-r--r--   0        0        0       65 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/resources/payment_links/__init__.py
--rw-r--r--   0        0        0    12471 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/resources/payment_links/client.py
--rw-r--r--   0        0        0       65 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/resources/payment_transactions/__init__.py
--rw-r--r--   0        0        0    10337 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/resources/payment_transactions/client.py
--rw-r--r--   0        0        0       65 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/resources/payment_webhooks/__init__.py
--rw-r--r--   0        0        0    12737 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/resources/payment_webhooks/client.py
--rw-r--r--   0        0        0       65 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/resources/receivable_transactions/__init__.py
--rw-r--r--   0        0        0    17393 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/resources/receivable_transactions/client.py
--rw-r--r--   0        0        0       65 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/resources/recurring_expenses/__init__.py
--rw-r--r--   0        0        0    20402 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/resources/recurring_expenses/client.py
--rw-r--r--   0        0        0       65 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/resources/risk_insights/__init__.py
--rw-r--r--   0        0        0    18655 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/resources/risk_insights/client.py
--rw-r--r--   0        0        0       65 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/resources/secret_keys/__init__.py
--rw-r--r--   0        0        0     5974 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/resources/secret_keys/client.py
--rw-r--r--   0        0        0       65 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/resources/tax_compliance_status/__init__.py
--rw-r--r--   0        0        0    15905 2023-05-17 17:48:24.264602 fern_belvo-0.0.33/src/belvo/resources/tax_compliance_status/client.py
--rw-r--r--   0        0        0       65 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/resources/tax_declarations/__init__.py
--rw-r--r--   0        0        0    17236 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/resources/tax_declarations/client.py
--rw-r--r--   0        0        0       65 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/resources/tax_retentions/__init__.py
--rw-r--r--   0        0        0    15901 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/resources/tax_retentions/client.py
--rw-r--r--   0        0        0       65 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/resources/tax_returns/__init__.py
--rw-r--r--   0        0        0    16912 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/resources/tax_returns/client.py
--rw-r--r--   0        0        0       65 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/resources/tax_status/__init__.py
--rw-r--r--   0        0        0    15773 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/resources/tax_status/client.py
--rw-r--r--   0        0        0       65 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/resources/transactions/__init__.py
--rw-r--r--   0        0        0    34291 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/resources/transactions/client.py
--rw-r--r--   0        0        0    41108 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/__init__.py
--rw-r--r--   0        0        0     1908 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/access_to_resource_denied.py
--rw-r--r--   0        0        0     4506 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/account.py
--rw-r--r--   0        0        0     2443 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/accounts_balance.py
--rw-r--r--   0        0        0     2241 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/accounts_credit_data.py
--rw-r--r--   0        0        0     1594 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/accounts_funds_data.py
--rw-r--r--   0        0        0      958 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/accounts_funds_data_public_identifications.py
--rw-r--r--   0        0        0     4780 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/accounts_loan_data.py
--rw-r--r--   0        0        0      935 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/accounts_loan_data_fees.py
--rw-r--r--   0        0        0     1191 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/accounts_loan_data_interest_rate.py
--rw-r--r--   0        0        0     1674 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/accounts_paginated_response.py
--rw-r--r--   0        0        0     1349 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/accounts_receivables_data.py
--rw-r--r--   0        0        0     1588 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/annual_costs_and_deductions_statement_business.py
--rw-r--r--   0        0        0     1883 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/annual_income_statement_business.py
--rw-r--r--   0        0        0     1282 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/annual_income_statement_individual.py
--rw-r--r--   0        0        0     1514 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/annual_totals_individual.py
--rw-r--r--   0        0        0      992 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/asynchronous_accepted_202.py
--rw-r--r--   0        0        0     1014 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/bad_request_error_body_item.py
--rw-r--r--   0        0        0     1827 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/balance.py
--rw-r--r--   0        0        0     1671 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/balances_paginated_response.py
--rw-r--r--   0        0        0     2531 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/bank_account_business_pse.py
--rw-r--r--   0        0        0     1189 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/bank_account_details_ofpi.py
--rw-r--r--   0        0        0      930 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/bank_account_details_ofpi_pix.py
--rw-r--r--   0        0        0     1196 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/bank_account_details_open_finance.py
--rw-r--r--   0        0        0      937 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/bank_account_details_open_finance_pix.py
--rw-r--r--   0        0        0     1094 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/bank_account_holder_request_ofpi.py
--rw-r--r--   0        0        0      356 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/bank_account_holder_request_ofpi_information.py
--rw-r--r--   0        0        0      966 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/bank_account_information_content_pse.py
--rw-r--r--   0        0        0     1077 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/bank_account_information_pse.py
--rw-r--r--   0        0        0     1852 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/bank_account_ofpi_response.py
--rw-r--r--   0        0        0      309 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/bank_account_ofpi_response_details.py
--rw-r--r--   0        0        0     1801 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/bank_account_paginated_response.py
--rw-r--r--   0        0        0      311 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/bank_account_paginated_response_results_item.py
--rw-r--r--   0        0        0      176 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/bank_account_pse_response.py
--rw-r--r--   0        0        0     1439 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/beneficiary_bank_account_ofpi.py
--rw-r--r--   0        0        0      356 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/beneficiary_bank_account_ofpi_details.py
--rw-r--r--   0        0        0     1242 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/beneficiary_bank_account_pse.py
--rw-r--r--   0        0        0      945 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/categorization.py
--rw-r--r--   0        0        0     3020 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/categorization_body.py
--rw-r--r--   0        0        0     2488 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/categorization_body_request.py
--rw-r--r--   0        0        0     1052 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/categorization_merchant_data.py
--rw-r--r--   0        0        0     3723 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/charge.py
--rw-r--r--   0        0        0      342 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/charge_payment_method_details.py
--rw-r--r--   0        0        0      972 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/charge_payment_method_details_ofpi.py
--rw-r--r--   0        0        0     1135 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/charge_payment_method_details_ofpi_content.py
--rw-r--r--   0        0        0      959 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/charge_payment_method_details_pse.py
--rw-r--r--   0        0        0     1127 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/charge_payment_method_details_pse_content.py
--rw-r--r--   0        0        0      703 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/charge_status.py
--rw-r--r--   0        0        0     1304 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/create_bank_account_ofpi.py
--rw-r--r--   0        0        0      307 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/create_bank_account_ofpi_details.py
--rw-r--r--   0        0        0     1863 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/create_bank_account_pse.py
--rw-r--r--   0        0        0      284 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/create_bank_account_request.py
--rw-r--r--   0        0        0      297 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/create_bank_account_response.py
--rw-r--r--   0        0        0     1521 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/create_customer_ofpi.py
--rw-r--r--   0        0        0     1517 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/create_customer_pse.py
--rw-r--r--   0        0        0      261 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/create_customer_request.py
--rw-r--r--   0        0        0      224 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/create_customer_response.py
--rw-r--r--   0        0        0     2638 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/create_payment_intent_pse.py
--rw-r--r--   0        0        0      134 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/create_payment_intent_pse_amount.py
--rw-r--r--   0        0        0     2894 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/create_payment_link_ofpi.py
--rw-r--r--   0        0        0      135 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/create_payment_link_ofpi_amount.py
--rw-r--r--   0        0        0     2835 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/create_payment_link_pse.py
--rw-r--r--   0        0        0      132 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/create_payment_link_pse_amount.py
--rw-r--r--   0        0        0      284 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/create_paymentlink_request.py
--rw-r--r--   0        0        0      247 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/create_paymentlink_response.py
--rw-r--r--   0        0        0     1855 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/customer_ofpi.py
--rw-r--r--   0        0        0     1784 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/customer_paginated_response.py
--rw-r--r--   0        0        0      238 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/customer_paginated_response_results_item.py
--rw-r--r--   0        0        0     2229 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/customer_pse.py
--rw-r--r--   0        0        0      297 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/detail_bank_account_response.py
--rw-r--r--   0        0        0      253 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/detail_create_paymentlink_response.py
--rw-r--r--   0        0        0      224 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/detail_customer_response.py
--rw-r--r--   0        0        0      237 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/detail_invoice_response.py
--rw-r--r--   0        0        0      301 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/detail_tax_declaration_response.py
--rw-r--r--   0        0        0      450 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/detail_tax_return_response.py
--rw-r--r--   0        0        0      233 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/detail_tax_status_response.py
--rw-r--r--   0        0        0      972 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/display_confirmation_required_content_pse.py
--rw-r--r--   0        0        0     1301 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/display_confirmation_required_ofpi.py
--rw-r--r--   0        0        0     1001 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/display_credentials_required_content_pse.py
--rw-r--r--   0        0        0     1279 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/display_customer_bank_accounts_content_pse.py
--rw-r--r--   0        0        0      913 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/display_payment_failed.py
--rw-r--r--   0        0        0     1055 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/display_payment_method_information_content_ofpi.py
--rw-r--r--   0        0        0     1489 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/display_payment_method_information_content_pse.py
--rw-r--r--   0        0        0      917 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/display_payment_processing.py
--rw-r--r--   0        0        0      916 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/display_payment_succeeded.py
--rw-r--r--   0        0        0      861 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/display_token_required_content_pse.py
--rw-r--r--   0        0        0     1005 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/document_id_business.py
--rw-r--r--   0        0        0     1007 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/document_id_individual.py
--rw-r--r--   0        0        0     1277 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/document_information_business.py
--rw-r--r--   0        0        0     1275 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/document_information_individual.py
--rw-r--r--   0        0        0     2557 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/employment_record.py
--rw-r--r--   0        0        0     2769 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/employment_record_detail.py
--rw-r--r--   0        0        0     1086 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/employment_record_document_id.py
--rw-r--r--   0        0        0     1317 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/employment_record_employment_status_updates.py
--rw-r--r--   0        0        0     1584 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/employment_record_entitlement.py
--rw-r--r--   0        0        0     1034 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/employment_record_file.py
--rw-r--r--   0        0        0     1843 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/employment_record_personal_data.py
--rw-r--r--   0        0        0     1495 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/employment_record_social_security_summary.py
--rw-r--r--   0        0        0     1732 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/employment_records_paginated_response.py
--rw-r--r--   0        0        0      123 2023-05-17 17:48:24.268602 fern_belvo-0.0.33/src/belvo/types/enum_account_category.py
--rw-r--r--   0        0        0      630 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_bank_account_holder_type_ofpi.py
--rw-r--r--   0        0        0      506 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_bank_account_holder_type_pse.py
--rw-r--r--   0        0        0      850 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_bank_account_pix_account_type_ofpi.py
--rw-r--r--   0        0        0     1179 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_categorization_account_category.py
--rw-r--r--   0        0        0      668 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_categorization_account_holder_type.py
--rw-r--r--   0        0        0      141 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_categorization_transaction_category.py
--rw-r--r--   0        0        0      144 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_categorization_transaction_subcategory.py
--rw-r--r--   0        0        0      702 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_categorization_transaction_type.py
--rw-r--r--   0        0        0      592 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_customer_identifier_type_ofpi.py
--rw-r--r--   0        0        0     1031 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_customer_identifier_type_pse.py
--rw-r--r--   0        0        0      699 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_customer_type.py
--rw-r--r--   0        0        0      495 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_employment_record_document_type.py
--rw-r--r--   0        0        0      532 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_employment_record_status.py
--rw-r--r--   0        0        0     1719 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_employment_record_status_update_events.py
--rw-r--r--   0        0        0      911 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_income_minimum_confidence_level_request.py
--rw-r--r--   0        0        0      475 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_income_source_type.py
--rw-r--r--   0        0        0      824 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_income_stream_confidence.py
--rw-r--r--   0        0        0     1495 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_income_stream_frequency.py
--rw-r--r--   0        0        0     2123 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_income_stream_type.py
--rw-r--r--   0        0        0      758 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_income_verification_account_category.py
--rw-r--r--   0        0        0      484 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_income_verification_account_holder_type.py
--rw-r--r--   0        0        0      359 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_income_verification_type.py
--rw-r--r--   0        0        0      862 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_institution_integration_type.py
--rw-r--r--   0        0        0      630 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_institution_status.py
--rw-r--r--   0        0        0      805 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_institution_type.py
--rw-r--r--   0        0        0     1687 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_investment_portfolio_instrument_type.py
--rw-r--r--   0        0        0     1084 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_investment_portfolio_type.py
--rw-r--r--   0        0        0     2329 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_invoice_allowed_income_types_request.py
--rw-r--r--   0        0        0      470 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_invoice_dian_invoice_type.py
--rw-r--r--   0        0        0      132 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_invoice_dian_payment_method.py
--rw-r--r--   0        0        0      986 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_invoice_sat_invoice_type.py
--rw-r--r--   0        0        0      131 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_invoice_sat_payment_method.py
--rw-r--r--   0        0        0      119 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_invoice_type.py
--rw-r--r--   0        0        0      923 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_link_access_mode_request.py
--rw-r--r--   0        0        0      130 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_link_access_mode_response.py
--rw-r--r--   0        0        0      123 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_link_refresh_rate.py
--rw-r--r--   0        0        0     1144 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_link_status.py
--rw-r--r--   0        0        0      869 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_loan_data_fee_type.py
--rw-r--r--   0        0        0      513 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_loan_data_interest_rate_type.py
--rw-r--r--   0        0        0      636 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_payment_intent_holder_type_pse.py
--rw-r--r--   0        0        0     1196 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_payment_intent_status.py
--rw-r--r--   0        0        0      728 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_payment_link_allowed_payment_method.py
--rw-r--r--   0        0        0      711 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_payment_link_provider.py
--rw-r--r--   0        0        0      981 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_payment_links_status.py
--rw-r--r--   0        0        0      682 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_payment_transaction_type.py
--rw-r--r--   0        0        0      571 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_payments_country.py
--rw-r--r--   0        0        0      586 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_payments_currency.py
--rw-r--r--   0        0        0      416 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_receivable_transaction_fee_type.py
--rw-r--r--   0        0        0      930 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_receivable_transaction_status.py
--rw-r--r--   0        0        0      133 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_receivable_transaction_type.py
--rw-r--r--   0        0        0     2023 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_recurring_expense_category.py
--rw-r--r--   0        0        0      513 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_recurring_expense_frequency.py
--rw-r--r--   0        0        0      552 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_recurring_expense_payment_type.py
--rw-r--r--   0        0        0      760 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_tax_compliance_status_outcome.py
--rw-r--r--   0        0        0      526 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_tax_retention_payment_status.py
--rw-r--r--   0        0        0      544 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_tax_retention_receiver_nationality.py
--rw-r--r--   0        0        0      735 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_tax_retention_type.py
--rw-r--r--   0        0        0      129 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_transaction_bill_status.py
--rw-r--r--   0        0        0      127 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_transaction_category.py
--rw-r--r--   0        0        0      125 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_transaction_status.py
--rw-r--r--   0        0        0      130 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_transaction_subcategory.py
--rw-r--r--   0        0        0      123 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/enum_transaction_type.py
--rw-r--r--   0        0        0     2117 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/equity_statement_business.py
--rw-r--r--   0        0        0     1137 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/equity_statement_individual.py
--rw-r--r--   0        0        0     2410 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/eyod_income_verification_body_request.py
--rw-r--r--   0        0        0     1525 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/gross_income_individual.py
--rw-r--r--   0        0        0     1067 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/holder_bank_account_information_pse.py
--rw-r--r--   0        0        0     1089 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/holder_bank_account_pse.py
--rw-r--r--   0        0        0     1045 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/holder_business_pse.py
--rw-r--r--   0        0        0     1179 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/holder_business_response_pse.py
--rw-r--r--   0        0        0     1189 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/holder_information_business_ofpi.py
--rw-r--r--   0        0        0     1073 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/holder_information_business_ofpi_response.py
--rw-r--r--   0        0        0      935 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/holder_information_business_pse.py
--rw-r--r--   0        0        0      993 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/holder_information_business_pse_response.py
--rw-r--r--   0        0        0     1290 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/holder_information_individual_ofpi.py
--rw-r--r--   0        0        0     1174 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/holder_information_individual_ofpi_response.py
--rw-r--r--   0        0        0     1043 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/holder_response_ofpi.py
--rw-r--r--   0        0        0      402 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/holder_response_ofpi_information.py
--rw-r--r--   0        0        0     4077 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/income.py
--rw-r--r--   0        0        0     4769 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/income_streams_body.py
--rw-r--r--   0        0        0     1666 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/incomes_paginated_response.py
--rw-r--r--   0        0        0     3939 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/institution.py
--rw-r--r--   0        0        0     1205 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/institution_account.py
--rw-r--r--   0        0        0     1989 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/institution_down_error.py
--rw-r--r--   0        0        0     2062 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/institution_form_field.py
--rw-r--r--   0        0        0     1894 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/institution_inactive_error.py
--rw-r--r--   0        0        0     2011 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/institution_unavailable_error.py
--rw-r--r--   0        0        0      937 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/institutions_feature.py
--rw-r--r--   0        0        0     1937 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/institutions_form_field.py
--rw-r--r--   0        0        0     1513 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/institutions_form_field_values.py
--rw-r--r--   0        0        0     1691 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/institutions_paginated_response.py
--rw-r--r--   0        0        0     2002 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/invalid_access_mode.py
--rw-r--r--   0        0        0     1936 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/invalid_link_error.py
--rw-r--r--   0        0        0     1967 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/invalid_period_error.py
--rw-r--r--   0        0        0     2666 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/investments_portfolio.py
--rw-r--r--   0        0        0     4088 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/investments_portfolio_instrument.py
--rw-r--r--   0        0        0     1056 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/investments_portfolio_instrument_fees.py
--rw-r--r--   0        0        0     1465 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/investments_portfolio_instrument_interest_rate.py
--rw-r--r--   0        0        0     1008 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/investments_portfolio_instrument_public_id.py
--rw-r--r--   0        0        0      952 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/investments_portfolio_instrument_redemption_conditions.py
--rw-r--r--   0        0        0     1751 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/investments_portfolios_paginated_response.py
--rw-r--r--   0        0        0     2518 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/invoice_detail_dian.py
--rw-r--r--   0        0        0     1418 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/invoice_detail_retained_tax_sat.py
--rw-r--r--   0        0        0     3178 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/invoice_detail_sat.py
--rw-r--r--   0        0        0     7893 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/invoice_dian.py
--rw-r--r--   0        0        0     2326 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/invoice_sender_details_dian.py
--rw-r--r--   0        0        0     1066 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/invoice_warnings_dian.py
--rw-r--r--   0        0        0      925 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/invoice_warnings_sat.py
--rw-r--r--   0        0        0     9760 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/invoice_with_id_sat.py
--rw-r--r--   0        0        0     2919 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/invoices_payments_dian.py
--rw-r--r--   0        0        0     2063 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/invoices_payments_related_documents_dian.py
--rw-r--r--   0        0        0     2024 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/invoices_payments_related_documents_sat.py
--rw-r--r--   0        0        0     3037 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/invoices_payments_sat.py
--rw-r--r--   0        0        0     2066 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/invoices_payroll_dian.py
--rw-r--r--   0        0        0     1782 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/invoices_payroll_sat.py
--rw-r--r--   0        0        0     2343 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/invoices_receiver_details_dian.py
--rw-r--r--   0        0        0     1809 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/invoices_response_paginated_response.py
--rw-r--r--   0        0        0      260 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/invoices_response_paginated_response_results_item.py
--rw-r--r--   0        0        0     1249 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/last_error_invalid_credentials.py
--rw-r--r--   0        0        0     1227 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/last_error_invalid_token.py
--rw-r--r--   0        0        0     1257 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/last_error_login_error.py
--rw-r--r--   0        0        0     1243 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/last_error_payment_error.py
--rw-r--r--   0        0        0     1289 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/last_error_session_expired.py
--rw-r--r--   0        0        0     1261 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/last_error_two_factor.py
--rw-r--r--   0        0        0     2833 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/link.py
--rw-r--r--   0        0        0      554 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/list_payment_links_request_ordering.py
--rw-r--r--   0        0        0      521 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/list_payment_links_request_status.py
--rw-r--r--   0        0        0      356 2023-05-17 17:48:24.272602 fern_belvo-0.0.33/src/belvo/types/list_tax_declarations_response.py
--rw-r--r--   0        0        0      586 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/list_tax_returns_response.py
--rw-r--r--   0        0        0     2699 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/login_error.py
--rw-r--r--   0        0        0      913 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/needs_redirect_content.py
--rw-r--r--   0        0        0      923 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/needs_redirect_content_pse.py
--rw-r--r--   0        0        0     1588 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/net_income_individual.py
--rw-r--r--   0        0        0     1660 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/next_step_display_confirmation_required_ofpi.py
--rw-r--r--   0        0        0     2256 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/next_step_display_confirmation_required_ofpi_type.py
--rw-r--r--   0        0        0     1673 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/next_step_display_confirmation_required_pse.py
--rw-r--r--   0        0        0     2850 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/next_step_display_confirmation_required_pse_type.py
--rw-r--r--   0        0        0     1665 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/next_step_display_credentials_required_pse.py
--rw-r--r--   0        0        0     2840 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/next_step_display_credentials_required_pse_type.py
--rw-r--r--   0        0        0     1676 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/next_step_display_customer_bank_accounts_pse.py
--rw-r--r--   0        0        0     2850 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/next_step_display_customer_bank_accounts_pse_type.py
--rw-r--r--   0        0        0     1595 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/next_step_display_needs_redirect_pse.py
--rw-r--r--   0        0        0     2780 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/next_step_display_needs_redirect_pse_type.py
--rw-r--r--   0        0        0     1573 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/next_step_display_payment_failed.py
--rw-r--r--   0        0        0     2179 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/next_step_display_payment_failed_type.py
--rw-r--r--   0        0        0     1700 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/next_step_display_payment_method_information.py
--rw-r--r--   0        0        0     1874 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/next_step_display_payment_method_information_pse.py
--rw-r--r--   0        0        0     2890 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/next_step_display_payment_method_information_pse_type.py
--rw-r--r--   0        0        0     2256 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/next_step_display_payment_method_information_type.py
--rw-r--r--   0        0        0     1606 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/next_step_display_payment_processing.py
--rw-r--r--   0        0        0     2207 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/next_step_display_payment_processing_type.py
--rw-r--r--   0        0        0     1598 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/next_step_display_payment_succeeded.py
--rw-r--r--   0        0        0     2200 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/next_step_display_payment_succeeded_type.py
--rw-r--r--   0        0        0     2128 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/next_step_display_token_required_pse.py
--rw-r--r--   0        0        0     2780 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/next_step_display_token_required_pse_type.py
--rw-r--r--   0        0        0     1545 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/next_step_needs_redirect.py
--rw-r--r--   0        0        0     2130 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/next_step_needs_redirect_type.py
--rw-r--r--   0        0        0     1531 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/non_taxable_income_individual.py
--rw-r--r--   0        0        0     1703 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/not_found_error_body.py
--rw-r--r--   0        0        0     2545 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/owner.py
--rw-r--r--   0        0        0     1584 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/owner_document_id.py
--rw-r--r--   0        0        0     1661 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/owners_paginated_response.py
--rw-r--r--   0        0        0     1596 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/paginated_response_link.py
--rw-r--r--   0        0        0     1798 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/patch_body.py
--rw-r--r--   0        0        0     1479 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/patch_body_without_save_data.py
--rw-r--r--   0        0        0      241 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/patch_invoices_response_item.py
--rw-r--r--   0        0        0      876 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/patch_payment_intents_body_pse.py
--rw-r--r--   0        0        0     2677 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/patch_payment_method_details_pse.py
--rw-r--r--   0        0        0     2302 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/payment_institution.py
--rw-r--r--   0        0        0     4025 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/payment_intent_ofpi.py
--rw-r--r--   0        0        0      846 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/payment_intent_ofpi_next_step.py
--rw-r--r--   0        0        0      462 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/payment_intent_ofpi_payment_method_details.py
--rw-r--r--   0        0        0     1733 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/payment_intent_paginated_response.py
--rw-r--r--   0        0        0     1549 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/payment_intent_payment_method_details_body_business_ofpi.py
--rw-r--r--   0        0        0     1551 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/payment_intent_payment_method_details_body_individual_ofpi.py
--rw-r--r--   0        0        0     2222 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/payment_intent_payment_method_details_body_pse.py
--rw-r--r--   0        0        0     1013 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/payment_intent_payment_method_details_business_ofpi.py
--rw-r--r--   0        0        0     1030 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/payment_intent_payment_method_details_individual_ofpi.py
--rw-r--r--   0        0        0      983 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/payment_intent_payment_method_details_pse.py
--rw-r--r--   0        0        0     4050 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/payment_intent_pse.py
--rw-r--r--   0        0        0      656 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/payment_intent_pse_last_error.py
--rw-r--r--   0        0        0      933 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/payment_intent_pse_next_step.py
--rw-r--r--   0        0        0     1644 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/payment_intents_payment_method_details_body_pse.py
--rw-r--r--   0        0        0      995 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/payment_intents_payment_method_details_pse.py
--rw-r--r--   0        0        0     1499 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/payment_link_callback_urls.py
--rw-r--r--   0        0        0     1408 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/payment_link_callback_urls_response.py
--rw-r--r--   0        0        0     2547 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/payment_link_list_ofpi.py
--rw-r--r--   0        0        0     2546 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/payment_link_list_pse.py
--rw-r--r--   0        0        0     2331 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/payment_link_ofpi.py
--rw-r--r--   0        0        0     1801 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/payment_link_paginated_response.py
--rw-r--r--   0        0        0      287 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/payment_link_paginated_response_results_item.py
--rw-r--r--   0        0        0     2326 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/payment_link_pse.py
--rw-r--r--   0        0        0     1244 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/payment_links_payment_method_details_body_ofpi.py
--rw-r--r--   0        0        0     1646 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/payment_links_payment_method_details_body_pse.py
--rw-r--r--   0        0        0     1021 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/payment_method_details_ofpi.py
--rw-r--r--   0        0        0      980 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/payment_method_details_pse.py
--rw-r--r--   0        0        0     1530 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/payment_method_info_customer_bank_accounts_pse.py
--rw-r--r--   0        0        0     1256 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/payment_method_information_body_ofpi.py
--rw-r--r--   0        0        0     1390 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/payment_method_information_body_pse.py
--rw-r--r--   0        0        0     1013 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/payment_method_information_details_pse.py
--rw-r--r--   0        0        0      967 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/payment_method_information_ofpi.py
--rw-r--r--   0        0        0     1043 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/payment_method_information_pse.py
--rw-r--r--   0        0        0     2247 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/payment_transaction.py
--rw-r--r--   0        0        0      313 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/payment_transaction_payer.py
--rw-r--r--   0        0        0     1527 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/payment_webhook.py
--rw-r--r--   0        0        0     1742 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/payments_institutions_paginated_response.py
--rw-r--r--   0        0        0     1742 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/payments_transactions_paginated_response.py
--rw-r--r--   0        0        0     1471 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/payments_way.py
--rw-r--r--   0        0        0     1708 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/payments_webhooks_paginated_response.py
--rw-r--r--   0        0        0     1072 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/pension_income_statement_individual.py
--rw-r--r--   0        0        0      817 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/providers_pse.py
--rw-r--r--   0        0        0     2957 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/receivables_transaction.py
--rw-r--r--   0        0        0     1042 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/receivables_transaction_account.py
--rw-r--r--   0        0        0     1065 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/receivables_transaction_number_of_installments.py
--rw-r--r--   0        0        0     1750 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/receivables_transactions_paginated_response.py
--rw-r--r--   0        0        0     1026 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/recevables_transaction_fees.py
--rw-r--r--   0        0        0     1242 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/recurring_expense_source_transaction.py
--rw-r--r--   0        0        0     2895 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/recurring_expenses.py
--rw-r--r--   0        0        0     1735 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/recurring_expenses_paginated_response.py
--rw-r--r--   0        0        0     1120 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/reporting_id.py
--rw-r--r--   0        0        0     2051 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/request_timeout_error_body.py
--rw-r--r--   0        0        0     1454 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/retention_breakdown.py
--rw-r--r--   0        0        0      244 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/retrieve_invoices_response_item.py
--rw-r--r--   0        0        0      308 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/retrieve_tax_declarations_response_item.py
--rw-r--r--   0        0        0      307 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/retrieve_tax_returns_request_body.py
--rw-r--r--   0        0        0      457 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/retrieve_tax_returns_response_item.py
--rw-r--r--   0        0        0      235 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/retrieve_tax_status_response.py
--rw-r--r--   0        0        0     1980 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/risk_insights.py
--rw-r--r--   0        0        0     3951 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/risk_insights_balance_metrics.py
--rw-r--r--   0        0        0     3942 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/risk_insights_cashflow_metrics.py
--rw-r--r--   0        0        0     1093 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/risk_insights_credit_card_metrics.py
--rw-r--r--   0        0        0     1369 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/risk_insights_loans_metrics.py
--rw-r--r--   0        0        0     1711 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/risk_insights_paginated_response.py
--rw-r--r--   0        0        0     9169 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/risk_insights_transaction_metrics.py
--rw-r--r--   0        0        0     1176 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/secret_keys.py
--rw-r--r--   0        0        0     1694 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/secret_keys_paginated_response.py
--rw-r--r--   0        0        0     2013 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/session_expired_error.py
--rw-r--r--   0        0        0     1276 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/standard_request.py
--rw-r--r--   0        0        0     2491 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/tax_assessment_business.py
--rw-r--r--   0        0        0     2771 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/tax_assessment_individual.py
--rw-r--r--   0        0        0     1788 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/tax_compliance_status.py
--rw-r--r--   0        0        0     1748 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/tax_compliance_status_paginated_response.py
--rw-r--r--   0        0        0     2291 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/tax_declaration_business.py
--rw-r--r--   0        0        0     1755 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/tax_declaration_business_paginated.py
--rw-r--r--   0        0        0     2281 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/tax_declaration_individual.py
--rw-r--r--   0        0        0     1765 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/tax_declaration_individual_paginated.py
--rw-r--r--   0        0        0     1666 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/tax_payer_information_business.py
--rw-r--r--   0        0        0     1489 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/tax_payer_information_individual.py
--rw-r--r--   0        0        0     3880 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/tax_retentions.py
--rw-r--r--   0        0        0     1716 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/tax_retentions_paginated_response.py
--rw-r--r--   0        0        0     3482 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/tax_return_business.py
--rw-r--r--   0        0        0     2658 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/tax_return_business_monthly.py
--rw-r--r--   0        0        0     3051 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/tax_return_personal.py
--rw-r--r--   0        0        0     2248 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/tax_return_personal_monthly.py
--rw-r--r--   0        0        0     1768 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/tax_returns_business_monthly_paginated.py
--rw-r--r--   0        0        0     1731 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/tax_returns_business_paginated.py
--rw-r--r--   0        0        0     2175 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/tax_returns_monthly_request.py
--rw-r--r--   0        0        0     1768 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/tax_returns_personal_monthly_paginated.py
--rw-r--r--   0        0        0     1731 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/tax_returns_personal_paginated.py
--rw-r--r--   0        0        0     1967 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/tax_returns_yearly_request.py
--rw-r--r--   0        0        0     1089 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/tax_status_address_between_street_dian.py
--rw-r--r--   0        0        0     1029 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/tax_status_address_between_street_sat.py
--rw-r--r--   0        0        0     2076 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/tax_status_address_dian.py
--rw-r--r--   0        0        0     1919 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/tax_status_address_sat.py
--rw-r--r--   0        0        0     3269 2023-05-17 17:48:24.276602 fern_belvo-0.0.33/src/belvo/types/tax_status_dian.py
--rw-r--r--   0        0        0     1728 2023-05-17 17:48:24.280602 fern_belvo-0.0.33/src/belvo/types/tax_status_economic_activity_dian.py
--rw-r--r--   0        0        0     1328 2023-05-17 17:48:24.280602 fern_belvo-0.0.33/src/belvo/types/tax_status_economic_activity_sat.py
--rw-r--r--   0        0        0     1550 2023-05-17 17:48:24.280602 fern_belvo-0.0.33/src/belvo/types/tax_status_obligations_dian.py
--rw-r--r--   0        0        0     1357 2023-05-17 17:48:24.280602 fern_belvo-0.0.33/src/belvo/types/tax_status_obligations_sat.py
--rw-r--r--   0        0        0     1784 2023-05-17 17:48:24.280602 fern_belvo-0.0.33/src/belvo/types/tax_status_paginated_response.py
--rw-r--r--   0        0        0      247 2023-05-17 17:48:24.280602 fern_belvo-0.0.33/src/belvo/types/tax_status_paginated_response_results_item.py
--rw-r--r--   0        0        0     1179 2023-05-17 17:48:24.280602 fern_belvo-0.0.33/src/belvo/types/tax_status_regimens_dian.py
--rw-r--r--   0        0        0     1048 2023-05-17 17:48:24.280602 fern_belvo-0.0.33/src/belvo/types/tax_status_regimens_sat.py
--rw-r--r--   0        0        0     3194 2023-05-17 17:48:24.280602 fern_belvo-0.0.33/src/belvo/types/tax_status_sat.py
--rw-r--r--   0        0        0     2648 2023-05-17 17:48:24.280602 fern_belvo-0.0.33/src/belvo/types/tax_status_tax_payer_information_dian.py
--rw-r--r--   0        0        0     2672 2023-05-17 17:48:24.280602 fern_belvo-0.0.33/src/belvo/types/tax_status_tax_payer_information_sat.py
--rw-r--r--   0        0        0     2428 2023-05-17 17:48:24.280602 fern_belvo-0.0.33/src/belvo/types/token_required_response.py
--rw-r--r--   0        0        0     1605 2023-05-17 17:48:24.280602 fern_belvo-0.0.33/src/belvo/types/token_required_response_token_generation_data.py
--rw-r--r--   0        0        0     2133 2023-05-17 17:48:24.280602 fern_belvo-0.0.33/src/belvo/types/too_many_sessions_error.py
--rw-r--r--   0        0        0     3391 2023-05-17 17:48:24.280602 fern_belvo-0.0.33/src/belvo/types/transaction.py
--rw-r--r--   0        0        0     1052 2023-05-17 17:48:24.280602 fern_belvo-0.0.33/src/belvo/types/transaction_bank_account_body_pse.py
--rw-r--r--   0        0        0      138 2023-05-17 17:48:24.280602 fern_belvo-0.0.33/src/belvo/types/transaction_bank_account_ofpi.py
--rw-r--r--   0        0        0      325 2023-05-17 17:48:24.280602 fern_belvo-0.0.33/src/belvo/types/transaction_bank_account_pse.py
--rw-r--r--   0        0        0     1689 2023-05-17 17:48:24.280602 fern_belvo-0.0.33/src/belvo/types/transaction_credit_card_data.py
--rw-r--r--   0        0        0     1049 2023-05-17 17:48:24.280602 fern_belvo-0.0.33/src/belvo/types/transaction_merchant_data.py
--rw-r--r--   0        0        0     1691 2023-05-17 17:48:24.280602 fern_belvo-0.0.33/src/belvo/types/transactions_paginated_response.py
--rw-r--r--   0        0        0     2001 2023-05-17 17:48:24.280602 fern_belvo-0.0.33/src/belvo/types/transactions_request.py
--rw-r--r--   0        0        0     1945 2023-05-17 17:48:24.280602 fern_belvo-0.0.33/src/belvo/types/unauthorized_error_body.py
--rw-r--r--   0        0        0     2077 2023-05-17 17:48:24.280602 fern_belvo-0.0.33/src/belvo/types/unconfirmed_link_error.py
--rw-r--r--   0        0        0     2013 2023-05-17 17:48:24.280602 fern_belvo-0.0.33/src/belvo/types/unexpected_error.py
--rw-r--r--   0        0        0     2032 2023-05-17 17:48:24.280602 fern_belvo-0.0.33/src/belvo/types/unsupported_operation_error.py
--rw-r--r--   0        0        0     2657 2023-05-17 17:48:24.280602 fern_belvo-0.0.33/src/belvo/types/validation_error.py
--rw-r--r--   0        0        0     2968 1970-01-01 00:00:00.000000 fern_belvo-0.0.33/PKG-INFO
+-rw-r--r--   0        0        0     2460 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/README.md
+-rw-r--r--   0        0        0      371 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/pyproject.toml
+-rw-r--r--   0        0        0    27716 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/__init__.py
+-rw-r--r--   0        0        0    12781 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/client.py
+-rw-r--r--   0        0        0      348 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      247 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/environment.py
+-rw-r--r--   0        0        0      594 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/errors/__init__.py
+-rw-r--r--   0        0        0      346 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/errors/bad_request_error.py
+-rw-r--r--   0        0        0      341 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/errors/forbidden_error.py
+-rw-r--r--   0        0        0      323 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/errors/internal_server_error.py
+-rw-r--r--   0        0        0      325 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/errors/not_found_error.py
+-rw-r--r--   0        0        0      340 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/errors/precondition_error.py
+-rw-r--r--   0        0        0      349 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/errors/request_timeout_error.py
+-rw-r--r--   0        0        0      340 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/errors/unauthorized_error.py
+-rw-r--r--   0        0        0        0 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/py.typed
+-rw-r--r--   0        0        0     1252 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/resources/accounts/__init__.py
+-rw-r--r--   0        0        0    25173 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/resources/accounts/client.py
+-rw-r--r--   0        0        0       65 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/resources/balances/__init__.py
+-rw-r--r--   0        0        0    23438 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/resources/balances/client.py
+-rw-r--r--   0        0        0       65 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/resources/bank_accounts/__init__.py
+-rw-r--r--   0        0        0    12881 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/resources/bank_accounts/client.py
+-rw-r--r--   0        0        0       65 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/resources/categorization/__init__.py
+-rw-r--r--   0        0        0     5136 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/resources/categorization/client.py
+-rw-r--r--   0        0        0       65 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/resources/customers/__init__.py
+-rw-r--r--   0        0        0    11285 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/resources/customers/client.py
+-rw-r--r--   0        0        0       65 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/resources/employment_records/__init__.py
+-rw-r--r--   0        0        0    14543 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/resources/employment_records/client.py
+-rw-r--r--   0        0        0       65 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/resources/income_verification/__init__.py
+-rw-r--r--   0        0        0     7011 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/resources/income_verification/client.py
+-rw-r--r--   0        0        0       65 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/resources/incomes/__init__.py
+-rw-r--r--   0        0        0    20690 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/resources/incomes/client.py
+-rw-r--r--   0        0        0       65 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/resources/institutions/__init__.py
+-rw-r--r--   0        0        0     8765 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/resources/institutions/client.py
+-rw-r--r--   0        0        0       65 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/resources/investment_portfolios/__init__.py
+-rw-r--r--   0        0        0    18632 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/resources/investment_portfolios/client.py
+-rw-r--r--   0        0        0       65 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/resources/invoices/__init__.py
+-rw-r--r--   0        0        0    24548 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/resources/invoices/client.py
+-rw-r--r--   0        0        0       65 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/resources/links/__init__.py
+-rw-r--r--   0        0        0    33898 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/resources/links/client.py
+-rw-r--r--   0        0        0       65 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/resources/owners/__init__.py
+-rw-r--r--   0        0        0    19773 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/resources/owners/client.py
+-rw-r--r--   0        0        0       65 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/resources/payment_institutions/__init__.py
+-rw-r--r--   0        0        0     7761 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/resources/payment_institutions/client.py
+-rw-r--r--   0        0        0       65 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/resources/payment_intents/__init__.py
+-rw-r--r--   0        0        0    16753 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/resources/payment_intents/client.py
+-rw-r--r--   0        0        0       65 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/resources/payment_links/__init__.py
+-rw-r--r--   0        0        0    12471 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/resources/payment_links/client.py
+-rw-r--r--   0        0        0       65 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/resources/payment_transactions/__init__.py
+-rw-r--r--   0        0        0    10337 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/resources/payment_transactions/client.py
+-rw-r--r--   0        0        0       65 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/resources/payment_webhooks/__init__.py
+-rw-r--r--   0        0        0    12737 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/resources/payment_webhooks/client.py
+-rw-r--r--   0        0        0       65 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/resources/receivable_transactions/__init__.py
+-rw-r--r--   0        0        0    17393 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/resources/receivable_transactions/client.py
+-rw-r--r--   0        0        0       65 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/resources/recurring_expenses/__init__.py
+-rw-r--r--   0        0        0    20402 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/resources/recurring_expenses/client.py
+-rw-r--r--   0        0        0       65 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/resources/risk_insights/__init__.py
+-rw-r--r--   0        0        0    18655 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/resources/risk_insights/client.py
+-rw-r--r--   0        0        0       65 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/resources/secret_keys/__init__.py
+-rw-r--r--   0        0        0     5974 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/resources/secret_keys/client.py
+-rw-r--r--   0        0        0       65 2023-05-20 13:11:43.739068 fern_belvo-0.0.34/src/belvo/resources/tax_compliance_status/__init__.py
+-rw-r--r--   0        0        0    15905 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/resources/tax_compliance_status/client.py
+-rw-r--r--   0        0        0       65 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/resources/tax_declarations/__init__.py
+-rw-r--r--   0        0        0    17236 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/resources/tax_declarations/client.py
+-rw-r--r--   0        0        0       65 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/resources/tax_retentions/__init__.py
+-rw-r--r--   0        0        0    15901 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/resources/tax_retentions/client.py
+-rw-r--r--   0        0        0       65 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/resources/tax_returns/__init__.py
+-rw-r--r--   0        0        0    16912 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/resources/tax_returns/client.py
+-rw-r--r--   0        0        0       65 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/resources/tax_status/__init__.py
+-rw-r--r--   0        0        0    15773 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/resources/tax_status/client.py
+-rw-r--r--   0        0        0       65 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/resources/transactions/__init__.py
+-rw-r--r--   0        0        0    34291 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/resources/transactions/client.py
+-rw-r--r--   0        0        0    41108 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/__init__.py
+-rw-r--r--   0        0        0     1908 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/access_to_resource_denied.py
+-rw-r--r--   0        0        0     4758 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/account.py
+-rw-r--r--   0        0        0     2443 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/accounts_balance.py
+-rw-r--r--   0        0        0     2311 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/accounts_credit_data.py
+-rw-r--r--   0        0        0     1594 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/accounts_funds_data.py
+-rw-r--r--   0        0        0      958 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/accounts_funds_data_public_identifications.py
+-rw-r--r--   0        0        0     4865 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/accounts_loan_data.py
+-rw-r--r--   0        0        0      999 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/accounts_loan_data_fees.py
+-rw-r--r--   0        0        0     1208 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/accounts_loan_data_interest_rate.py
+-rw-r--r--   0        0        0     1705 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/accounts_paginated_response.py
+-rw-r--r--   0        0        0     1439 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/accounts_receivables_data.py
+-rw-r--r--   0        0        0     1588 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/annual_costs_and_deductions_statement_business.py
+-rw-r--r--   0        0        0     1883 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/annual_income_statement_business.py
+-rw-r--r--   0        0        0     1282 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/annual_income_statement_individual.py
+-rw-r--r--   0        0        0     1514 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/annual_totals_individual.py
+-rw-r--r--   0        0        0      992 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/asynchronous_accepted_202.py
+-rw-r--r--   0        0        0     1014 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/bad_request_error_body_item.py
+-rw-r--r--   0        0        0     1827 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/balance.py
+-rw-r--r--   0        0        0     1671 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/balances_paginated_response.py
+-rw-r--r--   0        0        0     2531 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/bank_account_business_pse.py
+-rw-r--r--   0        0        0     1189 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/bank_account_details_ofpi.py
+-rw-r--r--   0        0        0      930 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/bank_account_details_ofpi_pix.py
+-rw-r--r--   0        0        0     1196 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/bank_account_details_open_finance.py
+-rw-r--r--   0        0        0      937 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/bank_account_details_open_finance_pix.py
+-rw-r--r--   0        0        0     1094 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/bank_account_holder_request_ofpi.py
+-rw-r--r--   0        0        0      356 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/bank_account_holder_request_ofpi_information.py
+-rw-r--r--   0        0        0      966 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/bank_account_information_content_pse.py
+-rw-r--r--   0        0        0     1077 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/bank_account_information_pse.py
+-rw-r--r--   0        0        0     1852 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/bank_account_ofpi_response.py
+-rw-r--r--   0        0        0      309 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/bank_account_ofpi_response_details.py
+-rw-r--r--   0        0        0     1801 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/bank_account_paginated_response.py
+-rw-r--r--   0        0        0      311 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/bank_account_paginated_response_results_item.py
+-rw-r--r--   0        0        0      176 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/bank_account_pse_response.py
+-rw-r--r--   0        0        0     1439 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/beneficiary_bank_account_ofpi.py
+-rw-r--r--   0        0        0      356 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/beneficiary_bank_account_ofpi_details.py
+-rw-r--r--   0        0        0     1242 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/beneficiary_bank_account_pse.py
+-rw-r--r--   0        0        0      945 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/categorization.py
+-rw-r--r--   0        0        0     3054 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/categorization_body.py
+-rw-r--r--   0        0        0     2488 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/categorization_body_request.py
+-rw-r--r--   0        0        0     1141 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/categorization_merchant_data.py
+-rw-r--r--   0        0        0     3723 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/charge.py
+-rw-r--r--   0        0        0      342 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/charge_payment_method_details.py
+-rw-r--r--   0        0        0      972 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/charge_payment_method_details_ofpi.py
+-rw-r--r--   0        0        0     1135 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/charge_payment_method_details_ofpi_content.py
+-rw-r--r--   0        0        0      959 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/charge_payment_method_details_pse.py
+-rw-r--r--   0        0        0     1127 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/charge_payment_method_details_pse_content.py
+-rw-r--r--   0        0        0      703 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/charge_status.py
+-rw-r--r--   0        0        0     1304 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/create_bank_account_ofpi.py
+-rw-r--r--   0        0        0      307 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/create_bank_account_ofpi_details.py
+-rw-r--r--   0        0        0     1863 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/create_bank_account_pse.py
+-rw-r--r--   0        0        0      284 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/create_bank_account_request.py
+-rw-r--r--   0        0        0      297 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/create_bank_account_response.py
+-rw-r--r--   0        0        0     1521 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/create_customer_ofpi.py
+-rw-r--r--   0        0        0     1517 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/create_customer_pse.py
+-rw-r--r--   0        0        0      261 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/create_customer_request.py
+-rw-r--r--   0        0        0      224 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/create_customer_response.py
+-rw-r--r--   0        0        0     2638 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/create_payment_intent_pse.py
+-rw-r--r--   0        0        0      134 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/create_payment_intent_pse_amount.py
+-rw-r--r--   0        0        0     2894 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/create_payment_link_ofpi.py
+-rw-r--r--   0        0        0      135 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/create_payment_link_ofpi_amount.py
+-rw-r--r--   0        0        0     2835 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/create_payment_link_pse.py
+-rw-r--r--   0        0        0      132 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/create_payment_link_pse_amount.py
+-rw-r--r--   0        0        0      284 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/create_paymentlink_request.py
+-rw-r--r--   0        0        0      247 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/create_paymentlink_response.py
+-rw-r--r--   0        0        0     1855 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/customer_ofpi.py
+-rw-r--r--   0        0        0     1784 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/customer_paginated_response.py
+-rw-r--r--   0        0        0      238 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/customer_paginated_response_results_item.py
+-rw-r--r--   0        0        0     2229 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/customer_pse.py
+-rw-r--r--   0        0        0      297 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/detail_bank_account_response.py
+-rw-r--r--   0        0        0      253 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/detail_create_paymentlink_response.py
+-rw-r--r--   0        0        0      224 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/detail_customer_response.py
+-rw-r--r--   0        0        0      237 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/detail_invoice_response.py
+-rw-r--r--   0        0        0      301 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/detail_tax_declaration_response.py
+-rw-r--r--   0        0        0      450 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/detail_tax_return_response.py
+-rw-r--r--   0        0        0      233 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/detail_tax_status_response.py
+-rw-r--r--   0        0        0      972 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/display_confirmation_required_content_pse.py
+-rw-r--r--   0        0        0     1301 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/display_confirmation_required_ofpi.py
+-rw-r--r--   0        0        0     1001 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/display_credentials_required_content_pse.py
+-rw-r--r--   0        0        0     1279 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/display_customer_bank_accounts_content_pse.py
+-rw-r--r--   0        0        0      913 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/display_payment_failed.py
+-rw-r--r--   0        0        0     1055 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/display_payment_method_information_content_ofpi.py
+-rw-r--r--   0        0        0     1489 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/display_payment_method_information_content_pse.py
+-rw-r--r--   0        0        0      917 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/display_payment_processing.py
+-rw-r--r--   0        0        0      916 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/display_payment_succeeded.py
+-rw-r--r--   0        0        0      861 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/display_token_required_content_pse.py
+-rw-r--r--   0        0        0     1005 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/document_id_business.py
+-rw-r--r--   0        0        0     1007 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/document_id_individual.py
+-rw-r--r--   0        0        0     1277 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/document_information_business.py
+-rw-r--r--   0        0        0     1275 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/document_information_individual.py
+-rw-r--r--   0        0        0     2557 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/employment_record.py
+-rw-r--r--   0        0        0     2769 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/employment_record_detail.py
+-rw-r--r--   0        0        0     1086 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/employment_record_document_id.py
+-rw-r--r--   0        0        0     1317 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/employment_record_employment_status_updates.py
+-rw-r--r--   0        0        0     1584 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/employment_record_entitlement.py
+-rw-r--r--   0        0        0     1034 2023-05-20 13:11:43.743068 fern_belvo-0.0.34/src/belvo/types/employment_record_file.py
+-rw-r--r--   0        0        0     1843 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/employment_record_personal_data.py
+-rw-r--r--   0        0        0     1495 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/employment_record_social_security_summary.py
+-rw-r--r--   0        0        0     1732 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/employment_records_paginated_response.py
+-rw-r--r--   0        0        0       91 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_account_category.py
+-rw-r--r--   0        0        0      630 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_bank_account_holder_type_ofpi.py
+-rw-r--r--   0        0        0      506 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_bank_account_holder_type_pse.py
+-rw-r--r--   0        0        0      850 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_bank_account_pix_account_type_ofpi.py
+-rw-r--r--   0        0        0     1179 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_categorization_account_category.py
+-rw-r--r--   0        0        0      668 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_categorization_account_holder_type.py
+-rw-r--r--   0        0        0      109 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_categorization_transaction_category.py
+-rw-r--r--   0        0        0      112 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_categorization_transaction_subcategory.py
+-rw-r--r--   0        0        0      702 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_categorization_transaction_type.py
+-rw-r--r--   0        0        0      592 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_customer_identifier_type_ofpi.py
+-rw-r--r--   0        0        0     1031 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_customer_identifier_type_pse.py
+-rw-r--r--   0        0        0      699 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_customer_type.py
+-rw-r--r--   0        0        0      633 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_employment_record_document_type.py
+-rw-r--r--   0        0        0      634 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_employment_record_status.py
+-rw-r--r--   0        0        0     1719 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_employment_record_status_update_events.py
+-rw-r--r--   0        0        0      911 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_income_minimum_confidence_level_request.py
+-rw-r--r--   0        0        0      475 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_income_source_type.py
+-rw-r--r--   0        0        0      824 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_income_stream_confidence.py
+-rw-r--r--   0        0        0     1495 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_income_stream_frequency.py
+-rw-r--r--   0        0        0     2123 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_income_stream_type.py
+-rw-r--r--   0        0        0      758 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_income_verification_account_category.py
+-rw-r--r--   0        0        0      484 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_income_verification_account_holder_type.py
+-rw-r--r--   0        0        0      471 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_income_verification_type.py
+-rw-r--r--   0        0        0      862 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_institution_integration_type.py
+-rw-r--r--   0        0        0      630 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_institution_status.py
+-rw-r--r--   0        0        0      805 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_institution_type.py
+-rw-r--r--   0        0        0     1687 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_investment_portfolio_instrument_type.py
+-rw-r--r--   0        0        0     1084 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_investment_portfolio_type.py
+-rw-r--r--   0        0        0     2329 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_invoice_allowed_income_types_request.py
+-rw-r--r--   0        0        0      653 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_invoice_dian_invoice_type.py
+-rw-r--r--   0        0        0      100 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_invoice_dian_payment_method.py
+-rw-r--r--   0        0        0     1213 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_invoice_sat_invoice_type.py
+-rw-r--r--   0        0        0       99 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_invoice_sat_payment_method.py
+-rw-r--r--   0        0        0       87 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_invoice_type.py
+-rw-r--r--   0        0        0      923 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_link_access_mode_request.py
+-rw-r--r--   0        0        0       98 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_link_access_mode_response.py
+-rw-r--r--   0        0        0       91 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_link_refresh_rate.py
+-rw-r--r--   0        0        0     1144 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_link_status.py
+-rw-r--r--   0        0        0      869 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_loan_data_fee_type.py
+-rw-r--r--   0        0        0      662 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_loan_data_interest_rate_type.py
+-rw-r--r--   0        0        0      636 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_payment_intent_holder_type_pse.py
+-rw-r--r--   0        0        0     1196 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_payment_intent_status.py
+-rw-r--r--   0        0        0      728 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_payment_link_allowed_payment_method.py
+-rw-r--r--   0        0        0      711 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_payment_link_provider.py
+-rw-r--r--   0        0        0      981 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_payment_links_status.py
+-rw-r--r--   0        0        0      682 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_payment_transaction_type.py
+-rw-r--r--   0        0        0      571 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_payments_country.py
+-rw-r--r--   0        0        0      586 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_payments_currency.py
+-rw-r--r--   0        0        0      547 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_receivable_transaction_fee_type.py
+-rw-r--r--   0        0        0     1080 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_receivable_transaction_status.py
+-rw-r--r--   0        0        0      101 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_receivable_transaction_type.py
+-rw-r--r--   0        0        0     2023 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_recurring_expense_category.py
+-rw-r--r--   0        0        0      513 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_recurring_expense_frequency.py
+-rw-r--r--   0        0        0      685 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_recurring_expense_payment_type.py
+-rw-r--r--   0        0        0      944 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_tax_compliance_status_outcome.py
+-rw-r--r--   0        0        0      654 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_tax_retention_payment_status.py
+-rw-r--r--   0        0        0      782 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_tax_retention_receiver_nationality.py
+-rw-r--r--   0        0        0      735 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_tax_retention_type.py
+-rw-r--r--   0        0        0       97 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_transaction_bill_status.py
+-rw-r--r--   0        0        0       95 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_transaction_category.py
+-rw-r--r--   0        0        0       93 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_transaction_status.py
+-rw-r--r--   0        0        0       98 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_transaction_subcategory.py
+-rw-r--r--   0        0        0       91 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/enum_transaction_type.py
+-rw-r--r--   0        0        0     2117 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/equity_statement_business.py
+-rw-r--r--   0        0        0     1137 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/equity_statement_individual.py
+-rw-r--r--   0        0        0     2427 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/eyod_income_verification_body_request.py
+-rw-r--r--   0        0        0     1525 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/gross_income_individual.py
+-rw-r--r--   0        0        0     1067 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/holder_bank_account_information_pse.py
+-rw-r--r--   0        0        0     1089 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/holder_bank_account_pse.py
+-rw-r--r--   0        0        0     1045 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/holder_business_pse.py
+-rw-r--r--   0        0        0     1179 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/holder_business_response_pse.py
+-rw-r--r--   0        0        0     1189 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/holder_information_business_ofpi.py
+-rw-r--r--   0        0        0     1073 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/holder_information_business_ofpi_response.py
+-rw-r--r--   0        0        0      935 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/holder_information_business_pse.py
+-rw-r--r--   0        0        0      993 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/holder_information_business_pse_response.py
+-rw-r--r--   0        0        0     1290 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/holder_information_individual_ofpi.py
+-rw-r--r--   0        0        0     1174 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/holder_information_individual_ofpi_response.py
+-rw-r--r--   0        0        0     1043 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/holder_response_ofpi.py
+-rw-r--r--   0        0        0      402 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/holder_response_ofpi_information.py
+-rw-r--r--   0        0        0     4077 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/income.py
+-rw-r--r--   0        0        0     4769 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/income_streams_body.py
+-rw-r--r--   0        0        0     1666 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/incomes_paginated_response.py
+-rw-r--r--   0        0        0     3939 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/institution.py
+-rw-r--r--   0        0        0     1205 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/institution_account.py
+-rw-r--r--   0        0        0     1989 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/institution_down_error.py
+-rw-r--r--   0        0        0     2062 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/institution_form_field.py
+-rw-r--r--   0        0        0     1894 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/institution_inactive_error.py
+-rw-r--r--   0        0        0     2011 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/institution_unavailable_error.py
+-rw-r--r--   0        0        0      937 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/institutions_feature.py
+-rw-r--r--   0        0        0     1937 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/institutions_form_field.py
+-rw-r--r--   0        0        0     1513 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/institutions_form_field_values.py
+-rw-r--r--   0        0        0     1691 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/institutions_paginated_response.py
+-rw-r--r--   0        0        0     2002 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/invalid_access_mode.py
+-rw-r--r--   0        0        0     1936 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/invalid_link_error.py
+-rw-r--r--   0        0        0     1967 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/invalid_period_error.py
+-rw-r--r--   0        0        0     2683 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/investments_portfolio.py
+-rw-r--r--   0        0        0     4139 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/investments_portfolio_instrument.py
+-rw-r--r--   0        0        0     1056 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/investments_portfolio_instrument_fees.py
+-rw-r--r--   0        0        0     1465 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/investments_portfolio_instrument_interest_rate.py
+-rw-r--r--   0        0        0     1008 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/investments_portfolio_instrument_public_id.py
+-rw-r--r--   0        0        0      952 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/investments_portfolio_instrument_redemption_conditions.py
+-rw-r--r--   0        0        0     1751 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/investments_portfolios_paginated_response.py
+-rw-r--r--   0        0        0     2518 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/invoice_detail_dian.py
+-rw-r--r--   0        0        0     1418 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/invoice_detail_retained_tax_sat.py
+-rw-r--r--   0        0        0     3178 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/invoice_detail_sat.py
+-rw-r--r--   0        0        0     7944 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/invoice_dian.py
+-rw-r--r--   0        0        0     2377 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/invoice_sender_details_dian.py
+-rw-r--r--   0        0        0     1168 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/invoice_warnings_dian.py
+-rw-r--r--   0        0        0     1020 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/invoice_warnings_sat.py
+-rw-r--r--   0        0        0     9811 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/invoice_with_id_sat.py
+-rw-r--r--   0        0        0     2919 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/invoices_payments_dian.py
+-rw-r--r--   0        0        0     2063 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/invoices_payments_related_documents_dian.py
+-rw-r--r--   0        0        0     2024 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/invoices_payments_related_documents_sat.py
+-rw-r--r--   0        0        0     3037 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/invoices_payments_sat.py
+-rw-r--r--   0        0        0     2168 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/invoices_payroll_dian.py
+-rw-r--r--   0        0        0     1880 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/invoices_payroll_sat.py
+-rw-r--r--   0        0        0     2396 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/invoices_receiver_details_dian.py
+-rw-r--r--   0        0        0     1809 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/invoices_response_paginated_response.py
+-rw-r--r--   0        0        0      260 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/invoices_response_paginated_response_results_item.py
+-rw-r--r--   0        0        0     1249 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/last_error_invalid_credentials.py
+-rw-r--r--   0        0        0     1227 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/last_error_invalid_token.py
+-rw-r--r--   0        0        0     1257 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/last_error_login_error.py
+-rw-r--r--   0        0        0     1243 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/last_error_payment_error.py
+-rw-r--r--   0        0        0     1289 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/last_error_session_expired.py
+-rw-r--r--   0        0        0     1261 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/last_error_two_factor.py
+-rw-r--r--   0        0        0     2833 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/link.py
+-rw-r--r--   0        0        0      554 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/list_payment_links_request_ordering.py
+-rw-r--r--   0        0        0      521 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/list_payment_links_request_status.py
+-rw-r--r--   0        0        0      356 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/list_tax_declarations_response.py
+-rw-r--r--   0        0        0      586 2023-05-20 13:11:43.747068 fern_belvo-0.0.34/src/belvo/types/list_tax_returns_response.py
+-rw-r--r--   0        0        0     2699 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/login_error.py
+-rw-r--r--   0        0        0      913 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/needs_redirect_content.py
+-rw-r--r--   0        0        0      923 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/needs_redirect_content_pse.py
+-rw-r--r--   0        0        0     1588 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/net_income_individual.py
+-rw-r--r--   0        0        0     1660 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/next_step_display_confirmation_required_ofpi.py
+-rw-r--r--   0        0        0     2321 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/next_step_display_confirmation_required_ofpi_type.py
+-rw-r--r--   0        0        0     1673 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/next_step_display_confirmation_required_pse.py
+-rw-r--r--   0        0        0     2915 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/next_step_display_confirmation_required_pse_type.py
+-rw-r--r--   0        0        0     1665 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/next_step_display_credentials_required_pse.py
+-rw-r--r--   0        0        0     2905 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/next_step_display_credentials_required_pse_type.py
+-rw-r--r--   0        0        0     1676 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/next_step_display_customer_bank_accounts_pse.py
+-rw-r--r--   0        0        0     2915 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/next_step_display_customer_bank_accounts_pse_type.py
+-rw-r--r--   0        0        0     1595 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/next_step_display_needs_redirect_pse.py
+-rw-r--r--   0        0        0     2845 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/next_step_display_needs_redirect_pse_type.py
+-rw-r--r--   0        0        0     1573 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/next_step_display_payment_failed.py
+-rw-r--r--   0        0        0     2244 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/next_step_display_payment_failed_type.py
+-rw-r--r--   0        0        0     1700 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/next_step_display_payment_method_information.py
+-rw-r--r--   0        0        0     1874 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/next_step_display_payment_method_information_pse.py
+-rw-r--r--   0        0        0     2955 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/next_step_display_payment_method_information_pse_type.py
+-rw-r--r--   0        0        0     2321 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/next_step_display_payment_method_information_type.py
+-rw-r--r--   0        0        0     1606 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/next_step_display_payment_processing.py
+-rw-r--r--   0        0        0     2272 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/next_step_display_payment_processing_type.py
+-rw-r--r--   0        0        0     1598 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/next_step_display_payment_succeeded.py
+-rw-r--r--   0        0        0     2265 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/next_step_display_payment_succeeded_type.py
+-rw-r--r--   0        0        0     2128 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/next_step_display_token_required_pse.py
+-rw-r--r--   0        0        0     2845 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/next_step_display_token_required_pse_type.py
+-rw-r--r--   0        0        0     1545 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/next_step_needs_redirect.py
+-rw-r--r--   0        0        0     2195 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/next_step_needs_redirect_type.py
+-rw-r--r--   0        0        0     1531 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/non_taxable_income_individual.py
+-rw-r--r--   0        0        0     1703 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/not_found_error_body.py
+-rw-r--r--   0        0        0     2545 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/owner.py
+-rw-r--r--   0        0        0     1687 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/owner_document_id.py
+-rw-r--r--   0        0        0     1661 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/owners_paginated_response.py
+-rw-r--r--   0        0        0     1596 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/paginated_response_link.py
+-rw-r--r--   0        0        0     1798 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/patch_body.py
+-rw-r--r--   0        0        0     1479 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/patch_body_without_save_data.py
+-rw-r--r--   0        0        0      241 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/patch_invoices_response_item.py
+-rw-r--r--   0        0        0      876 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/patch_payment_intents_body_pse.py
+-rw-r--r--   0        0        0     2677 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/patch_payment_method_details_pse.py
+-rw-r--r--   0        0        0     2302 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/payment_institution.py
+-rw-r--r--   0        0        0     4025 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/payment_intent_ofpi.py
+-rw-r--r--   0        0        0      846 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/payment_intent_ofpi_next_step.py
+-rw-r--r--   0        0        0      462 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/payment_intent_ofpi_payment_method_details.py
+-rw-r--r--   0        0        0     1733 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/payment_intent_paginated_response.py
+-rw-r--r--   0        0        0     1549 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/payment_intent_payment_method_details_body_business_ofpi.py
+-rw-r--r--   0        0        0     1551 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/payment_intent_payment_method_details_body_individual_ofpi.py
+-rw-r--r--   0        0        0     2222 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/payment_intent_payment_method_details_body_pse.py
+-rw-r--r--   0        0        0     1013 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/payment_intent_payment_method_details_business_ofpi.py
+-rw-r--r--   0        0        0     1030 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/payment_intent_payment_method_details_individual_ofpi.py
+-rw-r--r--   0        0        0      983 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/payment_intent_payment_method_details_pse.py
+-rw-r--r--   0        0        0     4050 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/payment_intent_pse.py
+-rw-r--r--   0        0        0      656 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/payment_intent_pse_last_error.py
+-rw-r--r--   0        0        0      933 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/payment_intent_pse_next_step.py
+-rw-r--r--   0        0        0     1644 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/payment_intents_payment_method_details_body_pse.py
+-rw-r--r--   0        0        0      995 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/payment_intents_payment_method_details_pse.py
+-rw-r--r--   0        0        0     1499 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/payment_link_callback_urls.py
+-rw-r--r--   0        0        0     1408 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/payment_link_callback_urls_response.py
+-rw-r--r--   0        0        0     2547 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/payment_link_list_ofpi.py
+-rw-r--r--   0        0        0     2546 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/payment_link_list_pse.py
+-rw-r--r--   0        0        0     2331 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/payment_link_ofpi.py
+-rw-r--r--   0        0        0     1801 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/payment_link_paginated_response.py
+-rw-r--r--   0        0        0      287 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/payment_link_paginated_response_results_item.py
+-rw-r--r--   0        0        0     2326 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/payment_link_pse.py
+-rw-r--r--   0        0        0     1244 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/payment_links_payment_method_details_body_ofpi.py
+-rw-r--r--   0        0        0     1646 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/payment_links_payment_method_details_body_pse.py
+-rw-r--r--   0        0        0     1021 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/payment_method_details_ofpi.py
+-rw-r--r--   0        0        0      980 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/payment_method_details_pse.py
+-rw-r--r--   0        0        0     1530 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/payment_method_info_customer_bank_accounts_pse.py
+-rw-r--r--   0        0        0     1256 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/payment_method_information_body_ofpi.py
+-rw-r--r--   0        0        0     1390 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/payment_method_information_body_pse.py
+-rw-r--r--   0        0        0     1013 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/payment_method_information_details_pse.py
+-rw-r--r--   0        0        0      967 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/payment_method_information_ofpi.py
+-rw-r--r--   0        0        0     1043 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/payment_method_information_pse.py
+-rw-r--r--   0        0        0     2247 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/payment_transaction.py
+-rw-r--r--   0        0        0      313 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/payment_transaction_payer.py
+-rw-r--r--   0        0        0     1527 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/payment_webhook.py
+-rw-r--r--   0        0        0     1742 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/payments_institutions_paginated_response.py
+-rw-r--r--   0        0        0     1742 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/payments_transactions_paginated_response.py
+-rw-r--r--   0        0        0     1471 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/payments_way.py
+-rw-r--r--   0        0        0     1708 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/payments_webhooks_paginated_response.py
+-rw-r--r--   0        0        0     1072 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/pension_income_statement_individual.py
+-rw-r--r--   0        0        0      817 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/providers_pse.py
+-rw-r--r--   0        0        0     3008 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/receivables_transaction.py
+-rw-r--r--   0        0        0     1042 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/receivables_transaction_account.py
+-rw-r--r--   0        0        0     1167 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/receivables_transaction_number_of_installments.py
+-rw-r--r--   0        0        0     1750 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/receivables_transactions_paginated_response.py
+-rw-r--r--   0        0        0     1043 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/recevables_transaction_fees.py
+-rw-r--r--   0        0        0     1401 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/recurring_expense_source_transaction.py
+-rw-r--r--   0        0        0     2946 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/recurring_expenses.py
+-rw-r--r--   0        0        0     1735 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/recurring_expenses_paginated_response.py
+-rw-r--r--   0        0        0     1120 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/reporting_id.py
+-rw-r--r--   0        0        0     2051 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/request_timeout_error_body.py
+-rw-r--r--   0        0        0     1471 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/retention_breakdown.py
+-rw-r--r--   0        0        0      244 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/retrieve_invoices_response_item.py
+-rw-r--r--   0        0        0      308 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/retrieve_tax_declarations_response_item.py
+-rw-r--r--   0        0        0      307 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/retrieve_tax_returns_request_body.py
+-rw-r--r--   0        0        0      457 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/retrieve_tax_returns_response_item.py
+-rw-r--r--   0        0        0      235 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/retrieve_tax_status_response.py
+-rw-r--r--   0        0        0     2065 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/risk_insights.py
+-rw-r--r--   0        0        0     4064 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/risk_insights_balance_metrics.py
+-rw-r--r--   0        0        0     4199 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/risk_insights_cashflow_metrics.py
+-rw-r--r--   0        0        0     1186 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/risk_insights_credit_card_metrics.py
+-rw-r--r--   0        0        0     1455 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/risk_insights_loans_metrics.py
+-rw-r--r--   0        0        0     1711 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/risk_insights_paginated_response.py
+-rw-r--r--   0        0        0     9308 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/risk_insights_transaction_metrics.py
+-rw-r--r--   0        0        0     1176 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/secret_keys.py
+-rw-r--r--   0        0        0     1694 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/secret_keys_paginated_response.py
+-rw-r--r--   0        0        0     2013 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/session_expired_error.py
+-rw-r--r--   0        0        0     1276 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/standard_request.py
+-rw-r--r--   0        0        0     2491 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/tax_assessment_business.py
+-rw-r--r--   0        0        0     2771 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/tax_assessment_individual.py
+-rw-r--r--   0        0        0     1788 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/tax_compliance_status.py
+-rw-r--r--   0        0        0     1748 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/tax_compliance_status_paginated_response.py
+-rw-r--r--   0        0        0     2291 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/tax_declaration_business.py
+-rw-r--r--   0        0        0     1755 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/tax_declaration_business_paginated.py
+-rw-r--r--   0        0        0     2281 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/tax_declaration_individual.py
+-rw-r--r--   0        0        0     1765 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/tax_declaration_individual_paginated.py
+-rw-r--r--   0        0        0     1666 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/tax_payer_information_business.py
+-rw-r--r--   0        0        0     1489 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/tax_payer_information_individual.py
+-rw-r--r--   0        0        0     3897 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/tax_retentions.py
+-rw-r--r--   0        0        0     1716 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/tax_retentions_paginated_response.py
+-rw-r--r--   0        0        0     3482 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/tax_return_business.py
+-rw-r--r--   0        0        0     2658 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/tax_return_business_monthly.py
+-rw-r--r--   0        0        0     3051 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/tax_return_personal.py
+-rw-r--r--   0        0        0     2248 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/tax_return_personal_monthly.py
+-rw-r--r--   0        0        0     1768 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/tax_returns_business_monthly_paginated.py
+-rw-r--r--   0        0        0     1731 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/tax_returns_business_paginated.py
+-rw-r--r--   0        0        0     2175 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/tax_returns_monthly_request.py
+-rw-r--r--   0        0        0     1768 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/tax_returns_personal_monthly_paginated.py
+-rw-r--r--   0        0        0     1731 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/tax_returns_personal_paginated.py
+-rw-r--r--   0        0        0     1967 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/tax_returns_yearly_request.py
+-rw-r--r--   0        0        0     1089 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/tax_status_address_between_street_dian.py
+-rw-r--r--   0        0        0     1029 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/tax_status_address_between_street_sat.py
+-rw-r--r--   0        0        0     2130 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/tax_status_address_dian.py
+-rw-r--r--   0        0        0     1973 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/tax_status_address_sat.py
+-rw-r--r--   0        0        0     3303 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/tax_status_dian.py
+-rw-r--r--   0        0        0     1728 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/tax_status_economic_activity_dian.py
+-rw-r--r--   0        0        0     1328 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/tax_status_economic_activity_sat.py
+-rw-r--r--   0        0        0     1550 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/tax_status_obligations_dian.py
+-rw-r--r--   0        0        0     1357 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/tax_status_obligations_sat.py
+-rw-r--r--   0        0        0     1784 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/tax_status_paginated_response.py
+-rw-r--r--   0        0        0      247 2023-05-20 13:11:43.751068 fern_belvo-0.0.34/src/belvo/types/tax_status_paginated_response_results_item.py
+-rw-r--r--   0        0        0     1179 2023-05-20 13:11:43.755068 fern_belvo-0.0.34/src/belvo/types/tax_status_regimens_dian.py
+-rw-r--r--   0        0        0     1048 2023-05-20 13:11:43.755068 fern_belvo-0.0.34/src/belvo/types/tax_status_regimens_sat.py
+-rw-r--r--   0        0        0     3228 2023-05-20 13:11:43.755068 fern_belvo-0.0.34/src/belvo/types/tax_status_sat.py
+-rw-r--r--   0        0        0     2701 2023-05-20 13:11:43.755068 fern_belvo-0.0.34/src/belvo/types/tax_status_tax_payer_information_dian.py
+-rw-r--r--   0        0        0     2725 2023-05-20 13:11:43.755068 fern_belvo-0.0.34/src/belvo/types/tax_status_tax_payer_information_sat.py
+-rw-r--r--   0        0        0     2428 2023-05-20 13:11:43.755068 fern_belvo-0.0.34/src/belvo/types/token_required_response.py
+-rw-r--r--   0        0        0     1605 2023-05-20 13:11:43.755068 fern_belvo-0.0.34/src/belvo/types/token_required_response_token_generation_data.py
+-rw-r--r--   0        0        0     2133 2023-05-20 13:11:43.755068 fern_belvo-0.0.34/src/belvo/types/too_many_sessions_error.py
+-rw-r--r--   0        0        0     3476 2023-05-20 13:11:43.755068 fern_belvo-0.0.34/src/belvo/types/transaction.py
+-rw-r--r--   0        0        0     1052 2023-05-20 13:11:43.755068 fern_belvo-0.0.34/src/belvo/types/transaction_bank_account_body_pse.py
+-rw-r--r--   0        0        0      138 2023-05-20 13:11:43.755068 fern_belvo-0.0.34/src/belvo/types/transaction_bank_account_ofpi.py
+-rw-r--r--   0        0        0      325 2023-05-20 13:11:43.755068 fern_belvo-0.0.34/src/belvo/types/transaction_bank_account_pse.py
+-rw-r--r--   0        0        0     1784 2023-05-20 13:11:43.755068 fern_belvo-0.0.34/src/belvo/types/transaction_credit_card_data.py
+-rw-r--r--   0        0        0     1635 2023-05-20 13:11:43.755068 fern_belvo-0.0.34/src/belvo/types/transaction_merchant_data.py
+-rw-r--r--   0        0        0     1691 2023-05-20 13:11:43.755068 fern_belvo-0.0.34/src/belvo/types/transactions_paginated_response.py
+-rw-r--r--   0        0        0     2001 2023-05-20 13:11:43.755068 fern_belvo-0.0.34/src/belvo/types/transactions_request.py
+-rw-r--r--   0        0        0     1945 2023-05-20 13:11:43.755068 fern_belvo-0.0.34/src/belvo/types/unauthorized_error_body.py
+-rw-r--r--   0        0        0     2077 2023-05-20 13:11:43.755068 fern_belvo-0.0.34/src/belvo/types/unconfirmed_link_error.py
+-rw-r--r--   0        0        0     2013 2023-05-20 13:11:43.755068 fern_belvo-0.0.34/src/belvo/types/unexpected_error.py
+-rw-r--r--   0        0        0     2032 2023-05-20 13:11:43.755068 fern_belvo-0.0.34/src/belvo/types/unsupported_operation_error.py
+-rw-r--r--   0        0        0     2657 2023-05-20 13:11:43.755068 fern_belvo-0.0.34/src/belvo/types/validation_error.py
+-rw-r--r--   0        0        0     2968 1970-01-01 00:00:00.000000 fern_belvo-0.0.34/PKG-INFO
```

### Comparing `fern_belvo-0.0.33/README.md` & `fern_belvo-0.0.34/README.md`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/__init__.py` & `fern_belvo-0.0.34/src/belvo/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/client.py` & `fern_belvo-0.0.34/src/belvo/client.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/core/datetime_utils.py` & `fern_belvo-0.0.34/src/belvo/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/core/jsonable_encoder.py` & `fern_belvo-0.0.34/src/belvo/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/errors/__init__.py` & `fern_belvo-0.0.34/src/belvo/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/resources/__init__.py` & `fern_belvo-0.0.34/src/belvo/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/resources/accounts/client.py` & `fern_belvo-0.0.34/src/belvo/resources/accounts/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,27 +136,27 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def retrieve_accounts(
         self, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None, request: StandardRequest
-    ) -> typing.List[Account]:
+    ) -> typing.List[typing.Optional[Account]]:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/accounts"),
             params={"omit": omit, "fields": fields},
             json=jsonable_encoder(request),
             auth=(self._secret_id, self._secret_password)
             if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[Account], _response.json())  # type: ignore
+            return pydantic.parse_obj_as(typing.List[typing.Optional[Account]], _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
                 pydantic.parse_obj_as(typing.List[BadRequestErrorBodyItem], _response.json())  # type: ignore
             )
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
@@ -177,27 +177,27 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def patch_accounts(
         self, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None, request: PatchBody
-    ) -> typing.List[Account]:
+    ) -> typing.List[typing.Optional[Account]]:
         _response = httpx.request(
             "PATCH",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/accounts"),
             params={"omit": omit, "fields": fields},
             json=jsonable_encoder(request),
             auth=(self._secret_id, self._secret_password)
             if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[Account], _response.json())  # type: ignore
+            return pydantic.parse_obj_as(typing.List[typing.Optional[Account]], _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
                 pydantic.parse_obj_as(typing.List[BadRequestErrorBodyItem], _response.json())  # type: ignore
             )
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
@@ -218,26 +218,26 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def detail_account(
         self, id: str, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None
-    ) -> Account:
+    ) -> typing.Optional[Account]:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/accounts/{id}"),
             params={"omit": omit, "fields": fields},
             auth=(self._secret_id, self._secret_password)
             if self._secret_id is not None and self._secret_password is not None
             else None,
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(Account, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(typing.Optional[Account], _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
             )
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.List[NotFoundErrorBody], _response.json()))  # type: ignore
         try:
@@ -379,28 +379,28 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def retrieve_accounts(
         self, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None, request: StandardRequest
-    ) -> typing.List[Account]:
+    ) -> typing.List[typing.Optional[Account]]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "api/accounts"),
                 params={"omit": omit, "fields": fields},
                 json=jsonable_encoder(request),
                 auth=(self._secret_id, self._secret_password)
                 if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[Account], _response.json())  # type: ignore
+            return pydantic.parse_obj_as(typing.List[typing.Optional[Account]], _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
                 pydantic.parse_obj_as(typing.List[BadRequestErrorBodyItem], _response.json())  # type: ignore
             )
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
@@ -421,28 +421,28 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def patch_accounts(
         self, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None, request: PatchBody
-    ) -> typing.List[Account]:
+    ) -> typing.List[typing.Optional[Account]]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "PATCH",
                 urllib.parse.urljoin(f"{self._environment.value}/", "api/accounts"),
                 params={"omit": omit, "fields": fields},
                 json=jsonable_encoder(request),
                 auth=(self._secret_id, self._secret_password)
                 if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[Account], _response.json())  # type: ignore
+            return pydantic.parse_obj_as(typing.List[typing.Optional[Account]], _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(
                 pydantic.parse_obj_as(typing.List[BadRequestErrorBodyItem], _response.json())  # type: ignore
             )
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
@@ -463,27 +463,27 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def detail_account(
         self, id: str, *, omit: typing.Optional[str] = None, fields: typing.Optional[str] = None
-    ) -> Account:
+    ) -> typing.Optional[Account]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"api/accounts/{id}"),
                 params={"omit": omit, "fields": fields},
                 auth=(self._secret_id, self._secret_password)
                 if self._secret_id is not None and self._secret_password is not None
                 else None,
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(Account, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(typing.Optional[Account], _response.json())  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(
                 pydantic.parse_obj_as(typing.List[UnauthorizedErrorBody], _response.json())  # type: ignore
             )
         if _response.status_code == 404:
             raise NotFoundError(pydantic.parse_obj_as(typing.List[NotFoundErrorBody], _response.json()))  # type: ignore
         try:
```

### Comparing `fern_belvo-0.0.33/src/belvo/resources/balances/client.py` & `fern_belvo-0.0.34/src/belvo/resources/balances/client.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/resources/bank_accounts/client.py` & `fern_belvo-0.0.34/src/belvo/resources/bank_accounts/client.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/resources/categorization/client.py` & `fern_belvo-0.0.34/src/belvo/resources/categorization/client.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/resources/customers/client.py` & `fern_belvo-0.0.34/src/belvo/resources/customers/client.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/resources/employment_records/client.py` & `fern_belvo-0.0.34/src/belvo/resources/employment_records/client.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/resources/income_verification/client.py` & `fern_belvo-0.0.34/src/belvo/resources/income_verification/client.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/resources/incomes/client.py` & `fern_belvo-0.0.34/src/belvo/resources/incomes/client.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/resources/institutions/client.py` & `fern_belvo-0.0.34/src/belvo/resources/institutions/client.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/resources/investment_portfolios/client.py` & `fern_belvo-0.0.34/src/belvo/resources/investment_portfolios/client.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/resources/invoices/client.py` & `fern_belvo-0.0.34/src/belvo/resources/invoices/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,24 +133,21 @@
         self,
         *,
         omit: typing.Optional[str] = None,
         fields: typing.Optional[str] = None,
         link: str,
         date_from: str,
         date_to: str,
-        type: EnumInvoiceType,
+        type: typing.Optional[EnumInvoiceType] = OMIT,
         attach_xml: typing.Optional[bool] = OMIT,
         save_data: typing.Optional[bool] = OMIT,
     ) -> typing.List[RetrieveInvoicesResponseItem]:
-        _request: typing.Dict[str, typing.Any] = {
-            "link": link,
-            "date_from": date_from,
-            "date_to": date_to,
-            "type": type,
-        }
+        _request: typing.Dict[str, typing.Any] = {"link": link, "date_from": date_from, "date_to": date_to}
+        if type is not OMIT:
+            _request["type"] = type
         if attach_xml is not OMIT:
             _request["attach_xml"] = attach_xml
         if save_data is not OMIT:
             _request["save_data"] = save_data
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/invoices"),
@@ -377,24 +374,21 @@
         self,
         *,
         omit: typing.Optional[str] = None,
         fields: typing.Optional[str] = None,
         link: str,
         date_from: str,
         date_to: str,
-        type: EnumInvoiceType,
+        type: typing.Optional[EnumInvoiceType] = OMIT,
         attach_xml: typing.Optional[bool] = OMIT,
         save_data: typing.Optional[bool] = OMIT,
     ) -> typing.List[RetrieveInvoicesResponseItem]:
-        _request: typing.Dict[str, typing.Any] = {
-            "link": link,
-            "date_from": date_from,
-            "date_to": date_to,
-            "type": type,
-        }
+        _request: typing.Dict[str, typing.Any] = {"link": link, "date_from": date_from, "date_to": date_to}
+        if type is not OMIT:
+            _request["type"] = type
         if attach_xml is not OMIT:
             _request["attach_xml"] = attach_xml
         if save_data is not OMIT:
             _request["save_data"] = save_data
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
```

### Comparing `fern_belvo-0.0.33/src/belvo/resources/links/client.py` & `fern_belvo-0.0.34/src/belvo/resources/links/client.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/resources/owners/client.py` & `fern_belvo-0.0.34/src/belvo/resources/owners/client.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/resources/payment_institutions/client.py` & `fern_belvo-0.0.34/src/belvo/resources/payment_institutions/client.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/resources/payment_intents/client.py` & `fern_belvo-0.0.34/src/belvo/resources/payment_intents/client.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/resources/payment_links/client.py` & `fern_belvo-0.0.34/src/belvo/resources/payment_links/client.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/resources/payment_transactions/client.py` & `fern_belvo-0.0.34/src/belvo/resources/payment_transactions/client.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/resources/payment_webhooks/client.py` & `fern_belvo-0.0.34/src/belvo/resources/payment_webhooks/client.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/resources/receivable_transactions/client.py` & `fern_belvo-0.0.34/src/belvo/resources/receivable_transactions/client.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/resources/recurring_expenses/client.py` & `fern_belvo-0.0.34/src/belvo/resources/recurring_expenses/client.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/resources/risk_insights/client.py` & `fern_belvo-0.0.34/src/belvo/resources/risk_insights/client.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/resources/secret_keys/client.py` & `fern_belvo-0.0.34/src/belvo/resources/secret_keys/client.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/resources/tax_compliance_status/client.py` & `fern_belvo-0.0.34/src/belvo/resources/tax_compliance_status/client.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/resources/tax_declarations/client.py` & `fern_belvo-0.0.34/src/belvo/resources/tax_declarations/client.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/resources/tax_retentions/client.py` & `fern_belvo-0.0.34/src/belvo/resources/tax_retentions/client.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/resources/tax_returns/client.py` & `fern_belvo-0.0.34/src/belvo/resources/tax_returns/client.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/resources/tax_status/client.py` & `fern_belvo-0.0.34/src/belvo/resources/tax_status/client.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/resources/transactions/client.py` & `fern_belvo-0.0.34/src/belvo/resources/transactions/client.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/__init__.py` & `fern_belvo-0.0.34/src/belvo/types/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/access_to_resource_denied.py` & `fern_belvo-0.0.34/src/belvo/types/access_to_resource_denied.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/account.py` & `fern_belvo-0.0.34/src/belvo/types/account.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,24 +12,30 @@
 from .accounts_loan_data import AccountsLoanData
 from .accounts_receivables_data import AccountsReceivablesData
 from .enum_account_category import EnumAccountCategory
 from .institution_account import InstitutionAccount
 
 
 class Account(pydantic.BaseModel):
+    """
+    Details regarding the account.
+
+    **Note**: For our recurring expenses resource, this account relates to the account that was analyzed to generate the recurring expenses report.
+    """
+
     id: typing.Optional[str] = pydantic.Field(
         description=("The unique identifier created by Belvo used to reference the current account.\n")
     )
     link: typing.Optional[str] = pydantic.Field(description=("The `link.id` the account belongs to.\n"))
     institution: typing.Optional[InstitutionAccount]
     collected_at: str = pydantic.Field(description=("The ISO-8601 timestamp when the data point was collected.\n"))
     created_at: typing.Optional[str] = pydantic.Field(
         description=("The ISO-8601 timestamp of when the data point was last updated in Belvo's database.\n")
     )
-    category: EnumAccountCategory
+    category: typing.Optional[EnumAccountCategory]
     balance_type: typing.Optional[str] = pydantic.Field(
         description=(
             "Indicates whether this account is either an `ASSET` or a `LIABILITY`. You can consider the balance of an `ASSET` as being positive, while the balance of a `LIABILITY` as negative.\n"
         )
     )
     type: typing.Optional[str] = pydantic.Field(description=("The account type, as designated by the institution.\n"))
     name: typing.Optional[str] = pydantic.Field(description=("The account name, as given by the institution.\n"))
@@ -63,16 +69,16 @@
         )
     )
     last_accessed_at: typing.Optional[str] = pydantic.Field(
         description=(
             "The ISO-8601 timestamp of Belvo's most recent successful access to the institution for the given link.\n"
         )
     )
-    credit_data: AccountsCreditData
-    loan_data: AccountsLoanData
+    credit_data: typing.Optional[AccountsCreditData]
+    loan_data: typing.Optional[AccountsLoanData]
     funds_data: typing.Optional[typing.List[AccountsFundsData]] = pydantic.Field(
         description=("One or more funds that contribute to the the pension account.\n")
     )
     receivables_data: typing.Optional[AccountsReceivablesData]
     bank_product_id: typing.Optional[str] = pydantic.Field(
         description=(
             "*This field has been deprecated.*\n" "\n" "*The institution's product ID for the account type.*\n"
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/accounts_balance.py` & `fern_belvo-0.0.34/src/belvo/types/accounts_balance.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/accounts_credit_data.py` & `fern_belvo-0.0.34/src/belvo/types/accounts_credit_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
 class AccountsCreditData(pydantic.BaseModel):
+    """
+    The credit options associated with this account.
+    """
+
     credit_limit: typing.Optional[float] = pydantic.Field(
         description=("The maximum amount of credit the owner can receive.\n")
     )
     collected_at: typing.Optional[str] = pydantic.Field(
         description=("The ISO-8601 timestamp when the data point was collected.\n")
     )
     cutting_date: typing.Optional[str] = pydantic.Field(description=("The closing date of the credit period.\n"))
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/accounts_funds_data.py` & `fern_belvo-0.0.34/src/belvo/types/accounts_funds_data.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/accounts_funds_data_public_identifications.py` & `fern_belvo-0.0.34/src/belvo/types/accounts_funds_data_public_identifications.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/accounts_loan_data.py` & `fern_belvo-0.0.34/src/belvo/types/accounts_loan_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 
 from ..core.datetime_utils import serialize_datetime
 from .accounts_loan_data_fees import AccountsLoanDataFees
 from .accounts_loan_data_interest_rate import AccountsLoanDataInterestRate
 
 
 class AccountsLoanData(pydantic.BaseModel):
+    """
+    The loan options associated with this account.
+    """
+
     collected_at: str = pydantic.Field(description=("The ISO-8601 timestamp when the data point was collected.\n"))
     contract_amount: typing.Optional[float] = pydantic.Field(
         description=(
             "The initial total loan amount, calculated by the institution, when the contract was signed. This amount includes the principal + interest + taxes + fees.\n"
         )
     )
     principal: typing.Optional[float] = pydantic.Field(
@@ -36,15 +40,15 @@
     )
     monthly_payment: typing.Optional[float] = pydantic.Field(
         description=("The recurrent monthly payment, if applicable.\n")
     )
     interest_rates: typing.Optional[typing.List[AccountsLoanDataInterestRate]] = pydantic.Field(
         description=("Breakdown of the interest applied to the loan.\n")
     )
-    fees: typing.Optional[typing.List[AccountsLoanDataFees]] = pydantic.Field(
+    fees: typing.Optional[typing.List[typing.Optional[AccountsLoanDataFees]]] = pydantic.Field(
         description=("Breakdown of the fees applied to the loan.\n")
     )
     number_of_installments_total: typing.Optional[int] = pydantic.Field(
         description=("The total number of installments required to pay the loan.\n")
     )
     number_of_installments_outstanding: typing.Optional[int] = pydantic.Field(
         description=("The number of installments left to pay.\n")
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/accounts_loan_data_fees.py` & `fern_belvo-0.0.34/src/belvo/types/accounts_loan_data_fees.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 from .enum_loan_data_fee_type import EnumLoanDataFeeType
 
 
 class AccountsLoanDataFees(pydantic.BaseModel):
+    """
+    Breakdown of the fees applied to the loan.
+    """
+
     type: EnumLoanDataFeeType
     value: float = pydantic.Field(description=("The total value of the fee. Same currency of the Loan.\n"))
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/accounts_loan_data_interest_rate.py` & `fern_belvo-0.0.34/src/belvo/types/accounts_loan_data_interest_rate.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     """
     Breakdown of the interest applied to the loan.
     """
 
     name: typing.Optional[str] = pydantic.Field(
         description=("The name of the type of interest rate applied to the loan.\n")
     )
-    type: EnumLoanDataInterestRateType
+    type: typing.Optional[EnumLoanDataInterestRateType]
     value: typing.Optional[float] = pydantic.Field(description=("The interest rate (in percent or currency value).\n"))
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/accounts_paginated_response.py` & `fern_belvo-0.0.34/src/belvo/types/owners_paginated_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .account import Account
+from .owner import Owner
 
 
-class AccountsPaginatedResponse(pydantic.BaseModel):
+class OwnersPaginatedResponse(pydantic.BaseModel):
     count: typing.Optional[int] = pydantic.Field(description=("The total number of results in your Belvo account.\n"))
     next: typing.Optional[str] = pydantic.Field(
         description=(
             "The URL to next page of results. Each page consists of up to 100 items. If there are not enough results for an additional page, the value is `null`.\n"
             "\n"
             "In our documentation example, we use `{endpoint}` as a placeholder value. In production, this value will be replaced by the actual endpoint you are currently using (for example, `accounts` or `owners`).\n"
         )
     )
     previous: typing.Optional[str] = pydantic.Field(
         description=("The URL to the previous page of results. If there is no previous page, the value is `null`.\n")
     )
-    results: typing.Optional[typing.List[Account]] = pydantic.Field(description=("An array of Account objects.\n"))
+    results: typing.Optional[typing.List[Owner]] = pydantic.Field(description=("Array of owner objects.\n"))
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/accounts_receivables_data.py` & `fern_belvo-0.0.34/src/belvo/types/invoice_detail_retained_tax_sat.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,25 +4,26 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class AccountsReceivablesData(pydantic.BaseModel):
-    current: typing.Optional[float] = pydantic.Field(
-        description=("The total sum of all receivables (`available` + `anticipated`)\n")
+class InvoiceDetailRetainedTaxSat(pydantic.BaseModel):
+    collected_at: typing.Optional[str] = pydantic.Field(
+        description=("The ISO-8601 timestamp when the data point was collected.\n")
     )
-    available: typing.Optional[float] = pydantic.Field(
-        description=("The amount that the owner of the account will receive according to an established date.\n")
+    tax_type: typing.Optional[str] = pydantic.Field(
+        description=("**Note**: This field is not applicable for SAT Mexico and will return `null`.\n")
     )
-    anticipated: typing.Optional[float] = pydantic.Field(
-        description=("The amount that the owner of the account received earlier than contracted.\n")
+    tax: typing.Optional[str] = pydantic.Field(
+        description=("The type of retained tax (for example, ISR, IVA or IEPS).\n")
     )
-    collected_at: str = pydantic.Field(description=("The ISO-8601 timestamp when the data point was collected.\n"))
+    tax_percentage: typing.Optional[float] = pydantic.Field(description=("The percentage of tax retained.\n"))
+    retained_tax_amount: typing.Optional[float] = pydantic.Field(description=("The amount of retained tax.\n"))
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/annual_costs_and_deductions_statement_business.py` & `fern_belvo-0.0.34/src/belvo/types/annual_costs_and_deductions_statement_business.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/annual_income_statement_business.py` & `fern_belvo-0.0.34/src/belvo/types/annual_income_statement_business.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/annual_income_statement_individual.py` & `fern_belvo-0.0.34/src/belvo/types/annual_income_statement_individual.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/annual_totals_individual.py` & `fern_belvo-0.0.34/src/belvo/types/annual_totals_individual.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/asynchronous_accepted_202.py` & `fern_belvo-0.0.34/src/belvo/types/asynchronous_accepted_202.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/bad_request_error_body_item.py` & `fern_belvo-0.0.34/src/belvo/types/bad_request_error_body_item.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/balance.py` & `fern_belvo-0.0.34/src/belvo/types/balance.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/balances_paginated_response.py` & `fern_belvo-0.0.34/src/belvo/types/balances_paginated_response.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/bank_account_business_pse.py` & `fern_belvo-0.0.34/src/belvo/types/bank_account_business_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/bank_account_details_ofpi.py` & `fern_belvo-0.0.34/src/belvo/types/bank_account_details_ofpi.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/bank_account_details_ofpi_pix.py` & `fern_belvo-0.0.34/src/belvo/types/bank_account_details_ofpi_pix.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/bank_account_details_open_finance.py` & `fern_belvo-0.0.34/src/belvo/types/bank_account_details_open_finance.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/bank_account_details_open_finance_pix.py` & `fern_belvo-0.0.34/src/belvo/types/bank_account_details_open_finance_pix.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/bank_account_holder_request_ofpi.py` & `fern_belvo-0.0.34/src/belvo/types/bank_account_holder_request_ofpi.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/bank_account_information_content_pse.py` & `fern_belvo-0.0.34/src/belvo/types/bank_account_information_content_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/bank_account_information_pse.py` & `fern_belvo-0.0.34/src/belvo/types/bank_account_information_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/bank_account_ofpi_response.py` & `fern_belvo-0.0.34/src/belvo/types/bank_account_ofpi_response.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/bank_account_paginated_response.py` & `fern_belvo-0.0.34/src/belvo/types/bank_account_paginated_response.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/beneficiary_bank_account_ofpi.py` & `fern_belvo-0.0.34/src/belvo/types/beneficiary_bank_account_ofpi.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/beneficiary_bank_account_pse.py` & `fern_belvo-0.0.34/src/belvo/types/beneficiary_bank_account_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/categorization.py` & `fern_belvo-0.0.34/src/belvo/types/categorization.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/categorization_body.py` & `fern_belvo-0.0.34/src/belvo/types/categorization_body.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,17 +42,17 @@
         )
     )
     mcc: typing.Optional[int] = pydantic.Field(
         description=(
             "The four-digit ISO 18245 Merchant Category Code (MCC). We only return this value when `account_type` = `CREDIT_CARD`.\n"
         )
     )
-    category: EnumCategorizationTransactionCategory
+    category: typing.Optional[EnumCategorizationTransactionCategory]
     subcategory: typing.Optional[EnumCategorizationTransactionSubcategory]
-    merchant: CategorizationMerchantData
+    merchant: typing.Optional[CategorizationMerchantData]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/categorization_body_request.py` & `fern_belvo-0.0.34/src/belvo/types/categorization_body_request.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/categorization_merchant_data.py` & `fern_belvo-0.0.34/src/belvo/types/categorization_merchant_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
 class CategorizationMerchantData(pydantic.BaseModel):
+    """
+    Additional data regarding the merchant involved in the transaction.
+    """
+
     logo: typing.Optional[str] = pydantic.Field(description=("The URL to the merchant's logo.\n"))
     website: typing.Optional[str] = pydantic.Field(description=("The URL to the merchant's website.\n"))
     merchant_name: typing.Optional[str] = pydantic.Field(description=("The name of the merchant.\n"))
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/charge.py` & `fern_belvo-0.0.34/src/belvo/types/charge.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/charge_payment_method_details_ofpi.py` & `fern_belvo-0.0.34/src/belvo/types/charge_payment_method_details_ofpi.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/charge_payment_method_details_ofpi_content.py` & `fern_belvo-0.0.34/src/belvo/types/charge_payment_method_details_ofpi_content.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/charge_payment_method_details_pse.py` & `fern_belvo-0.0.34/src/belvo/types/charge_payment_method_details_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/charge_payment_method_details_pse_content.py` & `fern_belvo-0.0.34/src/belvo/types/charge_payment_method_details_pse_content.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/charge_status.py` & `fern_belvo-0.0.34/src/belvo/types/charge_status.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/create_bank_account_ofpi.py` & `fern_belvo-0.0.34/src/belvo/types/create_bank_account_ofpi.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/create_bank_account_pse.py` & `fern_belvo-0.0.34/src/belvo/types/create_bank_account_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/create_customer_ofpi.py` & `fern_belvo-0.0.34/src/belvo/types/create_customer_ofpi.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/create_customer_pse.py` & `fern_belvo-0.0.34/src/belvo/types/create_customer_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/create_payment_intent_pse.py` & `fern_belvo-0.0.34/src/belvo/types/create_payment_intent_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/create_payment_link_ofpi.py` & `fern_belvo-0.0.34/src/belvo/types/create_payment_link_ofpi.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/create_payment_link_pse.py` & `fern_belvo-0.0.34/src/belvo/types/create_payment_link_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/customer_ofpi.py` & `fern_belvo-0.0.34/src/belvo/types/customer_ofpi.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/customer_paginated_response.py` & `fern_belvo-0.0.34/src/belvo/types/customer_paginated_response.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/customer_pse.py` & `fern_belvo-0.0.34/src/belvo/types/customer_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/display_confirmation_required_content_pse.py` & `fern_belvo-0.0.34/src/belvo/types/display_confirmation_required_content_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/display_confirmation_required_ofpi.py` & `fern_belvo-0.0.34/src/belvo/types/display_confirmation_required_ofpi.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/display_credentials_required_content_pse.py` & `fern_belvo-0.0.34/src/belvo/types/display_credentials_required_content_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/display_customer_bank_accounts_content_pse.py` & `fern_belvo-0.0.34/src/belvo/types/display_customer_bank_accounts_content_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/display_payment_failed.py` & `fern_belvo-0.0.34/src/belvo/types/display_payment_failed.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/display_payment_method_information_content_ofpi.py` & `fern_belvo-0.0.34/src/belvo/types/display_payment_method_information_content_ofpi.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/display_payment_method_information_content_pse.py` & `fern_belvo-0.0.34/src/belvo/types/display_payment_method_information_content_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/display_payment_processing.py` & `fern_belvo-0.0.34/src/belvo/types/display_payment_processing.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/display_payment_succeeded.py` & `fern_belvo-0.0.34/src/belvo/types/display_payment_succeeded.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/display_token_required_content_pse.py` & `fern_belvo-0.0.34/src/belvo/types/display_token_required_content_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/document_id_business.py` & `fern_belvo-0.0.34/src/belvo/types/document_id_business.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/document_id_individual.py` & `fern_belvo-0.0.34/src/belvo/types/document_id_individual.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/document_information_business.py` & `fern_belvo-0.0.34/src/belvo/types/document_information_business.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/document_information_individual.py` & `fern_belvo-0.0.34/src/belvo/types/document_information_individual.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/employment_record.py` & `fern_belvo-0.0.34/src/belvo/types/employment_record.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/employment_record_detail.py` & `fern_belvo-0.0.34/src/belvo/types/employment_record_detail.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/employment_record_document_id.py` & `fern_belvo-0.0.34/src/belvo/types/employment_record_document_id.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/employment_record_employment_status_updates.py` & `fern_belvo-0.0.34/src/belvo/types/employment_record_employment_status_updates.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/employment_record_entitlement.py` & `fern_belvo-0.0.34/src/belvo/types/employment_record_entitlement.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/employment_record_file.py` & `fern_belvo-0.0.34/src/belvo/types/employment_record_file.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/employment_record_personal_data.py` & `fern_belvo-0.0.34/src/belvo/types/employment_record_personal_data.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/employment_record_social_security_summary.py` & `fern_belvo-0.0.34/src/belvo/types/employment_record_social_security_summary.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/employment_records_paginated_response.py` & `fern_belvo-0.0.34/src/belvo/types/employment_records_paginated_response.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/enum_bank_account_holder_type_ofpi.py` & `fern_belvo-0.0.34/src/belvo/types/enum_bank_account_holder_type_ofpi.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/enum_bank_account_pix_account_type_ofpi.py` & `fern_belvo-0.0.34/src/belvo/types/enum_bank_account_pix_account_type_ofpi.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/enum_categorization_account_category.py` & `fern_belvo-0.0.34/src/belvo/types/enum_categorization_account_category.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/enum_categorization_account_holder_type.py` & `fern_belvo-0.0.34/src/belvo/types/enum_categorization_account_holder_type.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/enum_categorization_transaction_type.py` & `fern_belvo-0.0.34/src/belvo/types/enum_categorization_transaction_type.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/enum_customer_identifier_type_ofpi.py` & `fern_belvo-0.0.34/src/belvo/types/enum_customer_identifier_type_ofpi.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/enum_customer_identifier_type_pse.py` & `fern_belvo-0.0.34/src/belvo/types/enum_customer_identifier_type_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/enum_customer_type.py` & `fern_belvo-0.0.34/src/belvo/types/enum_customer_type.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/enum_employment_record_status.py` & `fern_belvo-0.0.34/src/belvo/types/enum_employment_record_status.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 import enum
 import typing
 
 T_Result = typing.TypeVar("T_Result")
 
 
 class EnumEmploymentRecordStatus(str, enum.Enum):
+    """
+    Indicates whether or not the individual is currently `EMPLOYED` or `UNEMPLOYED`.
+    """
+
     EMPLOYED = "EMPLOYED"
     UNEMPLOYED = "UNEMPLOYED"
 
     def visit(self, employed: typing.Callable[[], T_Result], unemployed: typing.Callable[[], T_Result]) -> T_Result:
         if self is EnumEmploymentRecordStatus.EMPLOYED:
             return employed()
         if self is EnumEmploymentRecordStatus.UNEMPLOYED:
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/enum_employment_record_status_update_events.py` & `fern_belvo-0.0.34/src/belvo/types/enum_employment_record_status_update_events.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/enum_income_minimum_confidence_level_request.py` & `fern_belvo-0.0.34/src/belvo/types/enum_income_minimum_confidence_level_request.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/enum_income_stream_confidence.py` & `fern_belvo-0.0.34/src/belvo/types/enum_income_stream_confidence.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/enum_income_stream_frequency.py` & `fern_belvo-0.0.34/src/belvo/types/enum_income_stream_frequency.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/enum_income_stream_type.py` & `fern_belvo-0.0.34/src/belvo/types/enum_income_stream_type.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/enum_income_verification_account_category.py` & `fern_belvo-0.0.34/src/belvo/types/enum_income_verification_account_category.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/enum_institution_integration_type.py` & `fern_belvo-0.0.34/src/belvo/types/enum_institution_integration_type.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/enum_institution_status.py` & `fern_belvo-0.0.34/src/belvo/types/enum_institution_status.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/enum_institution_type.py` & `fern_belvo-0.0.34/src/belvo/types/enum_institution_type.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/enum_investment_portfolio_instrument_type.py` & `fern_belvo-0.0.34/src/belvo/types/enum_investment_portfolio_instrument_type.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/enum_investment_portfolio_type.py` & `fern_belvo-0.0.34/src/belvo/types/enum_investment_portfolio_type.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/enum_invoice_allowed_income_types_request.py` & `fern_belvo-0.0.34/src/belvo/types/enum_invoice_allowed_income_types_request.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/enum_link_access_mode_request.py` & `fern_belvo-0.0.34/src/belvo/types/enum_link_access_mode_request.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/enum_link_status.py` & `fern_belvo-0.0.34/src/belvo/types/enum_link_status.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/enum_loan_data_fee_type.py` & `fern_belvo-0.0.34/src/belvo/types/enum_loan_data_fee_type.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/enum_payment_intent_holder_type_pse.py` & `fern_belvo-0.0.34/src/belvo/types/enum_payment_intent_holder_type_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/enum_payment_intent_status.py` & `fern_belvo-0.0.34/src/belvo/types/enum_payment_intent_status.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/enum_payment_link_allowed_payment_method.py` & `fern_belvo-0.0.34/src/belvo/types/enum_payment_link_allowed_payment_method.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/enum_payment_link_provider.py` & `fern_belvo-0.0.34/src/belvo/types/enum_payment_link_provider.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/enum_payment_links_status.py` & `fern_belvo-0.0.34/src/belvo/types/enum_payment_links_status.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/enum_payment_transaction_type.py` & `fern_belvo-0.0.34/src/belvo/types/enum_payment_transaction_type.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/enum_payments_country.py` & `fern_belvo-0.0.34/src/belvo/types/enum_payments_country.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/enum_payments_currency.py` & `fern_belvo-0.0.34/src/belvo/types/enum_payments_currency.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/enum_receivable_transaction_status.py` & `fern_belvo-0.0.34/src/belvo/types/enum_recurring_expense_payment_type.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,28 +2,23 @@
 
 import enum
 import typing
 
 T_Result = typing.TypeVar("T_Result")
 
 
-class EnumReceivableTransactionStatus(str, enum.Enum):
-    APPROVED = "APPROVED"
-    CANCELLED = "CANCELLED"
-    REVERTED = "REVERTED"
-    UNCATEGORIZED = "UNCATEGORIZED"
-
-    def visit(
-        self,
-        approved: typing.Callable[[], T_Result],
-        cancelled: typing.Callable[[], T_Result],
-        reverted: typing.Callable[[], T_Result],
-        uncategorized: typing.Callable[[], T_Result],
-    ) -> T_Result:
-        if self is EnumReceivableTransactionStatus.APPROVED:
-            return approved()
-        if self is EnumReceivableTransactionStatus.CANCELLED:
-            return cancelled()
-        if self is EnumReceivableTransactionStatus.REVERTED:
-            return reverted()
-        if self is EnumReceivableTransactionStatus.UNCATEGORIZED:
-            return uncategorized()
+class EnumRecurringExpensePaymentType(str, enum.Enum):
+    """
+    The type of recurring expense. We return one of the following values:
+
+      - `SUBSCRIPTION`
+      - `REGULAR`
+    """
+
+    SUBSCRIPTION = "SUBSCRIPTION"
+    REGULAR = "REGULAR"
+
+    def visit(self, subscription: typing.Callable[[], T_Result], regular: typing.Callable[[], T_Result]) -> T_Result:
+        if self is EnumRecurringExpensePaymentType.SUBSCRIPTION:
+            return subscription()
+        if self is EnumRecurringExpensePaymentType.REGULAR:
+            return regular()
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/enum_recurring_expense_category.py` & `fern_belvo-0.0.34/src/belvo/types/enum_recurring_expense_category.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/enum_recurring_expense_frequency.py` & `fern_belvo-0.0.34/src/belvo/types/enum_recurring_expense_frequency.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/enum_recurring_expense_payment_type.py` & `fern_belvo-0.0.34/src/belvo/types/enum_employment_record_document_type.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,16 +2,23 @@
 
 import enum
 import typing
 
 T_Result = typing.TypeVar("T_Result")
 
 
-class EnumRecurringExpensePaymentType(str, enum.Enum):
-    SUBSCRIPTION = "SUBSCRIPTION"
-    REGULAR = "REGULAR"
-
-    def visit(self, subscription: typing.Callable[[], T_Result], regular: typing.Callable[[], T_Result]) -> T_Result:
-        if self is EnumRecurringExpensePaymentType.SUBSCRIPTION:
-            return subscription()
-        if self is EnumRecurringExpensePaymentType.REGULAR:
-            return regular()
+class EnumEmploymentRecordDocumentType(str, enum.Enum):
+    """
+    The type of document related to the individual. We return one of the following values:
+
+      - `NSS`
+      - `CURP`
+    """
+
+    NSS = "NSS"
+    CURP = "CURP"
+
+    def visit(self, nss: typing.Callable[[], T_Result], curp: typing.Callable[[], T_Result]) -> T_Result:
+        if self is EnumEmploymentRecordDocumentType.NSS:
+            return nss()
+        if self is EnumEmploymentRecordDocumentType.CURP:
+            return curp()
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/enum_tax_retention_receiver_nationality.py` & `fern_belvo-0.0.34/src/belvo/types/enum_tax_retention_type.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,16 +2,23 @@
 
 import enum
 import typing
 
 T_Result = typing.TypeVar("T_Result")
 
 
-class EnumTaxRetentionReceiverNationality(str, enum.Enum):
-    NATIONAL = "NATIONAL"
-    FOREIGN = "FOREIGN"
-
-    def visit(self, national: typing.Callable[[], T_Result], foreign: typing.Callable[[], T_Result]) -> T_Result:
-        if self is EnumTaxRetentionReceiverNationality.NATIONAL:
-            return national()
-        if self is EnumTaxRetentionReceiverNationality.FOREIGN:
-            return foreign()
+class EnumTaxRetentionType(str, enum.Enum):
+    """
+    The type of tax retention in relation to the invoice (from the perspective of the Link owner).
+
+    - `OUTFLOW` relates to a tax retention for a sent invoice.
+    - `INFLOW` related to a tax retention for a received invoice.
+    """
+
+    OUTFLOW = "OUTFLOW"
+    INFLOW = "INFLOW"
+
+    def visit(self, outflow: typing.Callable[[], T_Result], inflow: typing.Callable[[], T_Result]) -> T_Result:
+        if self is EnumTaxRetentionType.OUTFLOW:
+            return outflow()
+        if self is EnumTaxRetentionType.INFLOW:
+            return inflow()
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/equity_statement_business.py` & `fern_belvo-0.0.34/src/belvo/types/equity_statement_business.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/equity_statement_individual.py` & `fern_belvo-0.0.34/src/belvo/types/equity_statement_individual.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/eyod_income_verification_body_request.py` & `fern_belvo-0.0.34/src/belvo/types/eyod_income_verification_body_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     account_holder_id: str = pydantic.Field(description=("Your unique ID for the account holder, in UUID format.\n"))
     account_id: str = pydantic.Field(description=("Your unique ID for the account where the transaction occurred.\n"))
     account_category: EnumIncomeVerificationAccountCategory
     value_date: str = pydantic.Field(
         description=("The date when the income transaction occurred, in `YYYY-MM-DD` format.\n")
     )
     description: str = pydantic.Field(description=("The description of the income.\n"))
-    type: EnumIncomeVerificationType
+    type: typing.Optional[EnumIncomeVerificationType]
     amount: float = pydantic.Field(description=("The income amount.\n"))
     currency: str = pydantic.Field(
         description=(
             "The three-letter currency code of the income. For example:\n"
             "\n"
             "  • 🇧🇷 BRL (Brazilian Real)\n"
             "  • 🇨🇴 COP (Colombian Peso)\n"
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/gross_income_individual.py` & `fern_belvo-0.0.34/src/belvo/types/gross_income_individual.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/holder_bank_account_information_pse.py` & `fern_belvo-0.0.34/src/belvo/types/holder_bank_account_information_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/holder_bank_account_pse.py` & `fern_belvo-0.0.34/src/belvo/types/holder_bank_account_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/holder_business_pse.py` & `fern_belvo-0.0.34/src/belvo/types/holder_business_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/holder_business_response_pse.py` & `fern_belvo-0.0.34/src/belvo/types/holder_business_response_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/holder_information_business_ofpi.py` & `fern_belvo-0.0.34/src/belvo/types/holder_information_business_ofpi.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/holder_information_business_ofpi_response.py` & `fern_belvo-0.0.34/src/belvo/types/holder_information_business_ofpi_response.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/holder_information_business_pse.py` & `fern_belvo-0.0.34/src/belvo/types/holder_information_business_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/holder_information_business_pse_response.py` & `fern_belvo-0.0.34/src/belvo/types/holder_information_business_pse_response.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/holder_information_individual_ofpi.py` & `fern_belvo-0.0.34/src/belvo/types/holder_information_individual_ofpi.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/holder_information_individual_ofpi_response.py` & `fern_belvo-0.0.34/src/belvo/types/holder_information_individual_ofpi_response.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/holder_response_ofpi.py` & `fern_belvo-0.0.34/src/belvo/types/holder_response_ofpi.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/income.py` & `fern_belvo-0.0.34/src/belvo/types/income.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/income_streams_body.py` & `fern_belvo-0.0.34/src/belvo/types/income_streams_body.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/incomes_paginated_response.py` & `fern_belvo-0.0.34/src/belvo/types/incomes_paginated_response.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/institution.py` & `fern_belvo-0.0.34/src/belvo/types/institution.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/institution_account.py` & `fern_belvo-0.0.34/src/belvo/types/institution_account.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/institution_down_error.py` & `fern_belvo-0.0.34/src/belvo/types/institution_down_error.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/institution_form_field.py` & `fern_belvo-0.0.34/src/belvo/types/institution_form_field.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/institution_inactive_error.py` & `fern_belvo-0.0.34/src/belvo/types/institution_inactive_error.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/institution_unavailable_error.py` & `fern_belvo-0.0.34/src/belvo/types/institution_unavailable_error.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/institutions_feature.py` & `fern_belvo-0.0.34/src/belvo/types/institutions_feature.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/institutions_form_field.py` & `fern_belvo-0.0.34/src/belvo/types/institutions_form_field.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/institutions_form_field_values.py` & `fern_belvo-0.0.34/src/belvo/types/institutions_form_field_values.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/institutions_paginated_response.py` & `fern_belvo-0.0.34/src/belvo/types/institutions_paginated_response.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/invalid_access_mode.py` & `fern_belvo-0.0.34/src/belvo/types/invalid_access_mode.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/invalid_link_error.py` & `fern_belvo-0.0.34/src/belvo/types/invalid_link_error.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/invalid_period_error.py` & `fern_belvo-0.0.34/src/belvo/types/invalid_period_error.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/investments_portfolio.py` & `fern_belvo-0.0.34/src/belvo/types/investments_portfolio.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
             "- 🇨🇴 COP (Colombian Peso)\n"
             "- 🇲🇽 MXN (Mexican Peso)\n"
             "\n"
             "\n"
             "Please note that other currencies other than in the list above may be returned.\n"
         )
     )
-    instruments: typing.Optional[typing.List[InvestmentsPortfolioInstrument]] = pydantic.Field(
+    instruments: typing.Optional[typing.List[typing.Optional[InvestmentsPortfolioInstrument]]] = pydantic.Field(
         description=("An array of instruments that fall into the investment portfolio.\n")
     )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/investments_portfolio_instrument.py` & `fern_belvo-0.0.34/src/belvo/types/investments_portfolio_instrument.py`

 * *Files 10% similar despite different names*

```diff
@@ -50,28 +50,28 @@
         description=("The average price of each share acquired in the instrument.\n")
     )
     profit: typing.Optional[float] = pydantic.Field(description=("The current profit earned in the instrument.\n"))
     open_date: typing.Optional[str] = pydantic.Field(
         description=("The start date of the instrument. Only applicable for instruments of type `bond` or `savings`.\n")
     )
     redemption_conditions: typing.Optional[
-        typing.List[InvestmentsPortfolioInstrumentRedemptionConditions]
+        typing.List[typing.Optional[InvestmentsPortfolioInstrumentRedemptionConditions]]
     ] = pydantic.Field(
         description=(
             "An array of conditions that apply to the instrument in order to retrieve the final value.\n"
             "\n"
             "For example, the due date, the liquidity date, the previdencia type, and so on.\n"
         )
     )
-    fees: typing.Optional[typing.List[InvestmentsPortfolioInstrumentFees]] = pydantic.Field(
+    fees: typing.Optional[typing.List[typing.Optional[InvestmentsPortfolioInstrumentFees]]] = pydantic.Field(
         description=("An array of fees that apply to the instrument.\n")
     )
-    interest_rates: typing.Optional[typing.List[InvestmentsPortfolioInstrumentInterestRate]] = pydantic.Field(
-        description=("An array of interest rates that apply to the instrument.\n")
-    )
+    interest_rates: typing.Optional[
+        typing.List[typing.Optional[InvestmentsPortfolioInstrumentInterestRate]]
+    ] = pydantic.Field(description=("An array of interest rates that apply to the instrument.\n"))
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/investments_portfolio_instrument_fees.py` & `fern_belvo-0.0.34/src/belvo/types/investments_portfolio_instrument_fees.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/investments_portfolio_instrument_interest_rate.py` & `fern_belvo-0.0.34/src/belvo/types/investments_portfolio_instrument_interest_rate.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/investments_portfolio_instrument_public_id.py` & `fern_belvo-0.0.34/src/belvo/types/investments_portfolio_instrument_public_id.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/investments_portfolio_instrument_redemption_conditions.py` & `fern_belvo-0.0.34/src/belvo/types/investments_portfolio_instrument_redemption_conditions.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/investments_portfolios_paginated_response.py` & `fern_belvo-0.0.34/src/belvo/types/investments_portfolios_paginated_response.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/invoice_detail_dian.py` & `fern_belvo-0.0.34/src/belvo/types/invoice_detail_dian.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/invoice_detail_retained_tax_sat.py` & `fern_belvo-0.0.34/src/belvo/types/payment_webhook.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,26 +4,28 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class InvoiceDetailRetainedTaxSat(pydantic.BaseModel):
-    collected_at: typing.Optional[str] = pydantic.Field(
-        description=("The ISO-8601 timestamp when the data point was collected.\n")
+class PaymentWebhook(pydantic.BaseModel):
+    id: str = pydantic.Field(description=("Belvo's unique ID for the webhook.\n"))
+    name: typing.Any
+    url: str = pydantic.Field(description=("The URL where webhook events should be sent to.\n"))
+    auth_header: typing.Optional[str] = pydantic.Field(
+        description=("The authentication header for the request. **Must** be set to `Authorization`.\n")
     )
-    tax_type: typing.Optional[str] = pydantic.Field(
-        description=("**Note**: This field is not applicable for SAT Mexico and will return `null`.\n")
+    auth_token: typing.Optional[str] = pydantic.Field(
+        description=("The authentication token you need to send webhook events. This value is obfuscated.\n")
     )
-    tax: typing.Optional[str] = pydantic.Field(
-        description=("The type of retained tax (for example, ISR, IVA or IEPS).\n")
+    created_at: str = pydantic.Field(
+        description=("The ISO-8601 timestamp of when the webhook was created in our database.\n")
     )
-    tax_percentage: typing.Optional[float] = pydantic.Field(description=("The percentage of tax retained.\n"))
-    retained_tax_amount: typing.Optional[float] = pydantic.Field(description=("The amount of retained tax.\n"))
+    created_by: str = pydantic.Field(description=("Belvo's unique ID of the user that created the webhook.\n"))
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/invoice_detail_sat.py` & `fern_belvo-0.0.34/src/belvo/types/invoice_detail_sat.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/invoice_dian.py` & `fern_belvo-0.0.34/src/belvo/types/invoice_dian.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,16 +42,16 @@
     expiration_date: typing.Optional[str] = pydantic.Field(
         description=(
             "Indicates when the invoice is set to expire.\n"
             "\n"
             "For example: If the invoice is paid in installments, this field indicates the date when the installment is to be paid.\n"
         )
     )
-    invoice_type: EnumInvoiceDianInvoiceType
-    type: EnumInvoiceType
+    invoice_type: typing.Optional[EnumInvoiceDianInvoiceType]
+    type: typing.Optional[EnumInvoiceType]
     sender_id: typing.Optional[str] = pydantic.Field(description=("The fiscal ID of the invoice sender.\n"))
     sender_name: typing.Optional[str] = pydantic.Field(description=("The name of the invoice sender.\n"))
     sender_details: typing.Optional[InvoiceSenderDetailsDian]
     sender_tax_fraud_status: typing.Optional[str] = pydantic.Field(
         description=(
             "Indicates whether or not the sender is on a tax fraud list for having submitted incorrect data, having outstanding payments, or having conducted business that is in violation of the fiscal institution's regulations.\n"
             "**Note**: This field is not applicable for DIAN Colombia and will return `null`.\n"
@@ -125,15 +125,15 @@
     )
     total_amount: typing.Optional[float] = pydantic.Field(
         description=("The total amount of the invoice (`subtotal_amount` + `tax_amount` - `discount_amount`)\n")
     )
     payments: typing.List[InvoicesPaymentsDian] = pydantic.Field(
         description=("**Note**: This field is not applicable for DIAN Colombia and will return `null`.\n")
     )
-    payroll: InvoicesPayrollDian
+    payroll: typing.Optional[InvoicesPayrollDian]
     folio: typing.Optional[str] = pydantic.Field(
         description=("**Note**: This field is not applicable for DIAN Colombia and will return `null`.\n")
     )
     xml: typing.Optional[str] = pydantic.Field(
         description=("**Note**: This field is not applicable for DIAN Colombia and will return `null`.\n")
     )
     warnings: typing.Optional[InvoiceWarningsDian]
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/invoice_sender_details_dian.py` & `fern_belvo-0.0.34/src/belvo/types/invoice_sender_details_dian.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
 class InvoiceSenderDetailsDian(pydantic.BaseModel):
+    """
+    Details regarding the sender.
+    """
+
     collected_at: typing.Optional[str] = pydantic.Field(
         description=("The ISO-8601 timestamp when the data point was collected.\n")
     )
     tax_payer_type: typing.Optional[str] = pydantic.Field(
         description=(
             "Indicates if the sender is a business or an individual. Can be either:\n"
             "\n"
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/invoice_warnings_dian.py` & `fern_belvo-0.0.34/src/belvo/types/invoice_warnings_dian.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
 class InvoiceWarningsDian(pydantic.BaseModel):
+    """
+    **Note**: This field is not applicable for DIAN Colombia and will return `null`.
+    """
+
     code: typing.Optional[str] = pydantic.Field(
         description=("**Note**: This field is not applicable for DIAN Colombia and will return `null`.\n")
     )
     message: typing.Optional[str] = pydantic.Field(
         description=("**Note**: This field is not applicable for DIAN Colombia and will return `null`.\n")
     )
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/invoice_warnings_sat.py` & `fern_belvo-0.0.34/src/belvo/types/transaction_bank_account_body_pse.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,17 +4,22 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class InvoiceWarningsSat(pydantic.BaseModel):
-    code: typing.Optional[str] = pydantic.Field(description=("The warning code.\n"))
-    message: typing.Optional[str] = pydantic.Field(description=("The description of the warning.\n"))
+class TransactionBankAccountBodyPse(pydantic.BaseModel):
+    """
+    Information about the payer's bank account. Belvo returns the bank account ID when the account is already saved in the Belvo database.
+    """
+
+    bank_account: typing.Optional[str] = pydantic.Field(
+        description=("Belvo's unique identifier for the payer’s bank account.\n")
+    )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/invoice_with_id_sat.py` & `fern_belvo-0.0.34/src/belvo/types/invoice_with_id_sat.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,16 +29,16 @@
     invoice_identification: typing.Optional[str] = pydantic.Field(
         description=("The fiscal institution's unique ID for the invoice.\n")
     )
     invoice_date: typing.Optional[str] = pydantic.Field(description=("The date of the invoice.\n"))
     status: typing.Optional[str] = pydantic.Field(
         description=("The status of the invoice. Can be either *Vigente* (valid) or *Cancelado* (cancelled).\n")
     )
-    invoice_type: EnumInvoiceSatInvoiceType
-    type: EnumInvoiceType
+    invoice_type: typing.Optional[EnumInvoiceSatInvoiceType]
+    type: typing.Optional[EnumInvoiceType]
     sender_id: typing.Optional[str] = pydantic.Field(description=("The fiscal ID of the invoice sender\n"))
     sender_name: typing.Optional[str] = pydantic.Field(description=("The name of the invoice sender.\n"))
     sender_tax_fraud_status: typing.Optional[str] = pydantic.Field(
         description=(
             "Indicates whether or not the sender is on SAT's tax fraud list for having submitted incorrect data, having outstanding payments, or having conducted business that is in violation of the fiscal institution's regulations.<br><br>\n"
             "SAT updates the tax fraud list every three months. <br><br>\n"
             "For more information regarding the reason's a taxpayer can be put on the tax fraud list, please see [Article 69](http://omawww.sat.gob.mx/cifras_sat/Paginas/datos/vinculo.html?page=ListCompleta69.html) and [Article 69-B](http://omawww.sat.gob.mx/cifras_sat/Paginas/datos/vinculo.html?page=ListCompleta69B.html) of Mexico's Código Fiscal de la Federación. <br><br>\n"
@@ -121,15 +121,15 @@
     )
     total_amount: typing.Optional[float] = pydantic.Field(
         description=("The total amount of the invoice (`subtotal_amount` + `tax_amount` - `discount_amount`)\n")
     )
     payments: typing.List[InvoicesPaymentsSat] = pydantic.Field(
         description=("A list detailing all the invoice payments.\n")
     )
-    payroll: InvoicesPayrollSat
+    payroll: typing.Optional[InvoicesPayrollSat]
     folio: typing.Optional[str] = pydantic.Field(
         description=("The internal control number that the taxpayer assigns to the invoice.\n")
     )
     xml: typing.Optional[str] = pydantic.Field(description=("XML of the invoice document.\n"))
     warnings: typing.Optional[InvoiceWarningsSat]
     sender_blacklist_status: typing.Optional[str] = pydantic.Field(
         description=("This field has been deprecated. Please use `sender_tax_fraud_status` instead.\n")
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/invoices_payments_dian.py` & `fern_belvo-0.0.34/src/belvo/types/invoices_payments_dian.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/invoices_payments_related_documents_dian.py` & `fern_belvo-0.0.34/src/belvo/types/invoices_payments_related_documents_dian.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/invoices_payments_related_documents_sat.py` & `fern_belvo-0.0.34/src/belvo/types/invoices_payments_related_documents_sat.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/invoices_payments_sat.py` & `fern_belvo-0.0.34/src/belvo/types/invoices_payments_sat.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/invoices_payroll_dian.py` & `fern_belvo-0.0.34/src/belvo/types/invoices_payroll_dian.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
 class InvoicesPayrollDian(pydantic.BaseModel):
+    """
+    **Note**: This field is not applicable for DIAN Colombia and will return `null`.
+    """
+
     days: typing.Optional[int] = pydantic.Field(
         description=("**Note**: This field is not applicable for DIAN Colombia and will return `null`.\n")
     )
     type: typing.Optional[str] = pydantic.Field(
         description=("**Note**: This field is not applicable for DIAN Colombia and will return `null`.\n")
     )
     amount: typing.Optional[float] = pydantic.Field(
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/invoices_payroll_sat.py` & `fern_belvo-0.0.34/src/belvo/types/invoices_payroll_sat.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
 class InvoicesPayrollSat(pydantic.BaseModel):
+    """
+    Details regarding the payroll payment. Only applicable for payroll invoices.
+    """
+
     days: typing.Optional[int] = pydantic.Field(description=("The number of days covered by the payment.\n"))
     type: typing.Optional[str] = pydantic.Field(
         description=(
             "The payroll type, as defined by the legal entity of the country.\n"
             "\n"
             "- 🇲🇽 Mexico [SAT catalog reference article](https://developers.belvo.com/docs/sat-catalogs#payroll-type)\n"
         )
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/invoices_receiver_details_dian.py` & `fern_belvo-0.0.34/src/belvo/types/invoices_receiver_details_dian.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
 class InvoicesReceiverDetailsDian(pydantic.BaseModel):
+    """
+    Details regarding the receiver.
+    """
+
     collected_at: typing.Optional[str] = pydantic.Field(
         description=("The ISO-8601 timestamp when the data point was collected.\n")
     )
     tax_payer_type: typing.Optional[str] = pydantic.Field(
         description=(
             "Indicates if the receiver is a business or an individual. Can be either:\n"
             "\n"
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/invoices_response_paginated_response.py` & `fern_belvo-0.0.34/src/belvo/types/invoices_response_paginated_response.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/last_error_invalid_credentials.py` & `fern_belvo-0.0.34/src/belvo/types/last_error_invalid_credentials.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/last_error_invalid_token.py` & `fern_belvo-0.0.34/src/belvo/types/last_error_invalid_token.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/last_error_login_error.py` & `fern_belvo-0.0.34/src/belvo/types/last_error_login_error.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/last_error_payment_error.py` & `fern_belvo-0.0.34/src/belvo/types/last_error_payment_error.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/last_error_session_expired.py` & `fern_belvo-0.0.34/src/belvo/types/last_error_session_expired.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/last_error_two_factor.py` & `fern_belvo-0.0.34/src/belvo/types/last_error_two_factor.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/link.py` & `fern_belvo-0.0.34/src/belvo/types/link.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/list_payment_links_request_ordering.py` & `fern_belvo-0.0.34/src/belvo/types/list_payment_links_request_ordering.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/list_payment_links_request_status.py` & `fern_belvo-0.0.34/src/belvo/types/list_payment_links_request_status.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/list_tax_returns_response.py` & `fern_belvo-0.0.34/src/belvo/types/list_tax_returns_response.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/login_error.py` & `fern_belvo-0.0.34/src/belvo/types/login_error.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/needs_redirect_content.py` & `fern_belvo-0.0.34/src/belvo/types/needs_redirect_content.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/needs_redirect_content_pse.py` & `fern_belvo-0.0.34/src/belvo/types/needs_redirect_content_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/net_income_individual.py` & `fern_belvo-0.0.34/src/belvo/types/net_income_individual.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/next_step_display_confirmation_required_ofpi.py` & `fern_belvo-0.0.34/src/belvo/types/next_step_display_confirmation_required_ofpi.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/next_step_display_confirmation_required_ofpi_type.py` & `fern_belvo-0.0.34/src/belvo/types/next_step_display_confirmation_required_ofpi_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 import enum
 import typing
 
 T_Result = typing.TypeVar("T_Result")
 
 
 class NextStepDisplayConfirmationRequiredOfpiType(str, enum.Enum):
+    """
+    The type of `next_step` you need to follow.
+    """
+
     OPEN_FINANCE_DISPLAY_PAYMENT_METHOD_INFORMATION = "open_finance_display_payment_method_information"
     OPEN_FINANCE_DISPLAY_CONFIRMATION_REQUIRED = "open_finance_display_confirmation_required"
     OPEN_FINANCE_DISPLAY_NEEDS_REDIRECT = "open_finance_display_needs_redirect"
     OPEN_FINANCE_DISPLAY_PAYMENT_PROCESSING = "open_finance_display_payment_processing"
     OPEN_FINANCE_DISPLAY_PAYMENT_SUCCEEDED = "open_finance_display_payment_succeeded"
     OPEN_FINANCE_DISPLAY_PAYMENT_FAILED = "open_finance_display_payment_failed"
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/next_step_display_confirmation_required_pse.py` & `fern_belvo-0.0.34/src/belvo/types/next_step_display_confirmation_required_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/next_step_display_confirmation_required_pse_type.py` & `fern_belvo-0.0.34/src/belvo/types/next_step_display_confirmation_required_pse_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 import enum
 import typing
 
 T_Result = typing.TypeVar("T_Result")
 
 
 class NextStepDisplayConfirmationRequiredPseType(str, enum.Enum):
+    """
+    The type of `next_step` you need to follow.
+    """
+
     PSE_DISPLAY_PAYMENT_METHOD_INFORMATION = "pse_display_payment_method_information"
     PSE_DISPLAY_CREDENTIALS_REQUIRED = "pse_display_credentials_required"
     PSE_DISPLAY_NEEDS_REDIRECT = "pse_display_needs_redirect"
     PSE_DISPLAY_TOKEN_REQUIRED = "pse_display_token_required"
     PSE_DISPLAY_CUSTOMER_BANK_ACCOUNTS = "pse_display_customer_bank_accounts"
     PSE_DISPLAY_CONFIRMATION_REQUIRED = "pse_display_confirmation_required"
     PSE_DISPLAY_PAYMENT_PROCESSING = "pse_display_payment_processing"
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/next_step_display_credentials_required_pse.py` & `fern_belvo-0.0.34/src/belvo/types/next_step_display_credentials_required_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/next_step_display_credentials_required_pse_type.py` & `fern_belvo-0.0.34/src/belvo/types/next_step_display_credentials_required_pse_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 import enum
 import typing
 
 T_Result = typing.TypeVar("T_Result")
 
 
 class NextStepDisplayCredentialsRequiredPseType(str, enum.Enum):
+    """
+    The type of `next_step` you need to follow.
+    """
+
     PSE_DISPLAY_PAYMENT_METHOD_INFORMATION = "pse_display_payment_method_information"
     PSE_DISPLAY_CREDENTIALS_REQUIRED = "pse_display_credentials_required"
     PSE_DISPLAY_NEEDS_REDIRECT = "pse_display_needs_redirect"
     PSE_DISPLAY_TOKEN_REQUIRED = "pse_display_token_required"
     PSE_DISPLAY_CUSTOMER_BANK_ACCOUNTS = "pse_display_customer_bank_accounts"
     PSE_DISPLAY_CONFIRMATION_REQUIRED = "pse_display_confirmation_required"
     PSE_DISPLAY_PAYMENT_PROCESSING = "pse_display_payment_processing"
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/next_step_display_customer_bank_accounts_pse.py` & `fern_belvo-0.0.34/src/belvo/types/next_step_display_customer_bank_accounts_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/next_step_display_customer_bank_accounts_pse_type.py` & `fern_belvo-0.0.34/src/belvo/types/next_step_display_customer_bank_accounts_pse_type.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 import enum
 import typing
 
 T_Result = typing.TypeVar("T_Result")
 
 
 class NextStepDisplayCustomerBankAccountsPseType(str, enum.Enum):
+    """
+    The type of `next_step` you need to follow.
+    """
+
     PSE_DISPLAY_PAYMENT_METHOD_INFORMATION = "pse_display_payment_method_information"
     PSE_DISPLAY_CREDENTIALS_REQUIRED = "pse_display_credentials_required"
     PSE_DISPLAY_NEEDS_REDIRECT = "pse_display_needs_redirect"
     PSE_DISPLAY_TOKEN_REQUIRED = "pse_display_token_required"
     PSE_DISPLAY_CUSTOMER_BANK_ACCOUNTS = "pse_display_customer_bank_accounts"
     PSE_DISPLAY_CONFIRMATION_REQUIRED = "pse_display_confirmation_required"
     PSE_DISPLAY_PAYMENT_PROCESSING = "pse_display_payment_processing"
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/next_step_display_needs_redirect_pse.py` & `fern_belvo-0.0.34/src/belvo/types/next_step_display_needs_redirect_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/next_step_display_needs_redirect_pse_type.py` & `fern_belvo-0.0.34/src/belvo/types/next_step_display_needs_redirect_pse_type.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 import enum
 import typing
 
 T_Result = typing.TypeVar("T_Result")
 
 
 class NextStepDisplayNeedsRedirectPseType(str, enum.Enum):
+    """
+    The type of `next_step` you need to follow.
+    """
+
     PSE_DISPLAY_PAYMENT_METHOD_INFORMATION = "pse_display_payment_method_information"
     PSE_DISPLAY_CREDENTIALS_REQUIRED = "pse_display_credentials_required"
     PSE_DISPLAY_NEEDS_REDIRECT = "pse_display_needs_redirect"
     PSE_DISPLAY_TOKEN_REQUIRED = "pse_display_token_required"
     PSE_DISPLAY_CUSTOMER_BANK_ACCOUNTS = "pse_display_customer_bank_accounts"
     PSE_DISPLAY_CONFIRMATION_REQUIRED = "pse_display_confirmation_required"
     PSE_DISPLAY_PAYMENT_PROCESSING = "pse_display_payment_processing"
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/next_step_display_payment_failed.py` & `fern_belvo-0.0.34/src/belvo/types/next_step_display_payment_failed.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/next_step_display_payment_failed_type.py` & `fern_belvo-0.0.34/src/belvo/types/next_step_needs_redirect_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,19 @@
 
 import enum
 import typing
 
 T_Result = typing.TypeVar("T_Result")
 
 
-class NextStepDisplayPaymentFailedType(str, enum.Enum):
+class NextStepNeedsRedirectType(str, enum.Enum):
+    """
+    The type of `next_step` you need to follow.
+    """
+
     OPEN_FINANCE_DISPLAY_PAYMENT_METHOD_INFORMATION = "open_finance_display_payment_method_information"
     OPEN_FINANCE_DISPLAY_CONFIRMATION_REQUIRED = "open_finance_display_confirmation_required"
     OPEN_FINANCE_DISPLAY_NEEDS_REDIRECT = "open_finance_display_needs_redirect"
     OPEN_FINANCE_DISPLAY_PAYMENT_PROCESSING = "open_finance_display_payment_processing"
     OPEN_FINANCE_DISPLAY_PAYMENT_SUCCEEDED = "open_finance_display_payment_succeeded"
     OPEN_FINANCE_DISPLAY_PAYMENT_FAILED = "open_finance_display_payment_failed"
 
@@ -19,19 +23,19 @@
         open_finance_display_payment_method_information: typing.Callable[[], T_Result],
         open_finance_display_confirmation_required: typing.Callable[[], T_Result],
         open_finance_display_needs_redirect: typing.Callable[[], T_Result],
         open_finance_display_payment_processing: typing.Callable[[], T_Result],
         open_finance_display_payment_succeeded: typing.Callable[[], T_Result],
         open_finance_display_payment_failed: typing.Callable[[], T_Result],
     ) -> T_Result:
-        if self is NextStepDisplayPaymentFailedType.OPEN_FINANCE_DISPLAY_PAYMENT_METHOD_INFORMATION:
+        if self is NextStepNeedsRedirectType.OPEN_FINANCE_DISPLAY_PAYMENT_METHOD_INFORMATION:
             return open_finance_display_payment_method_information()
-        if self is NextStepDisplayPaymentFailedType.OPEN_FINANCE_DISPLAY_CONFIRMATION_REQUIRED:
+        if self is NextStepNeedsRedirectType.OPEN_FINANCE_DISPLAY_CONFIRMATION_REQUIRED:
             return open_finance_display_confirmation_required()
-        if self is NextStepDisplayPaymentFailedType.OPEN_FINANCE_DISPLAY_NEEDS_REDIRECT:
+        if self is NextStepNeedsRedirectType.OPEN_FINANCE_DISPLAY_NEEDS_REDIRECT:
             return open_finance_display_needs_redirect()
-        if self is NextStepDisplayPaymentFailedType.OPEN_FINANCE_DISPLAY_PAYMENT_PROCESSING:
+        if self is NextStepNeedsRedirectType.OPEN_FINANCE_DISPLAY_PAYMENT_PROCESSING:
             return open_finance_display_payment_processing()
-        if self is NextStepDisplayPaymentFailedType.OPEN_FINANCE_DISPLAY_PAYMENT_SUCCEEDED:
+        if self is NextStepNeedsRedirectType.OPEN_FINANCE_DISPLAY_PAYMENT_SUCCEEDED:
             return open_finance_display_payment_succeeded()
-        if self is NextStepDisplayPaymentFailedType.OPEN_FINANCE_DISPLAY_PAYMENT_FAILED:
+        if self is NextStepNeedsRedirectType.OPEN_FINANCE_DISPLAY_PAYMENT_FAILED:
             return open_finance_display_payment_failed()
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/next_step_display_payment_method_information.py` & `fern_belvo-0.0.34/src/belvo/types/next_step_display_payment_method_information.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/next_step_display_payment_method_information_pse.py` & `fern_belvo-0.0.34/src/belvo/types/next_step_display_payment_method_information_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/next_step_display_payment_method_information_pse_type.py` & `fern_belvo-0.0.34/src/belvo/types/next_step_display_payment_method_information_pse_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 import enum
 import typing
 
 T_Result = typing.TypeVar("T_Result")
 
 
 class NextStepDisplayPaymentMethodInformationPseType(str, enum.Enum):
+    """
+    The type of `next_step` you need to follow.
+    """
+
     PSE_DISPLAY_PAYMENT_METHOD_INFORMATION = "pse_display_payment_method_information"
     PSE_DISPLAY_CREDENTIALS_REQUIRED = "pse_display_credentials_required"
     PSE_DISPLAY_NEEDS_REDIRECT = "pse_display_needs_redirect"
     PSE_DISPLAY_TOKEN_REQUIRED = "pse_display_token_required"
     PSE_DISPLAY_CUSTOMER_BANK_ACCOUNTS = "pse_display_customer_bank_accounts"
     PSE_DISPLAY_CONFIRMATION_REQUIRED = "pse_display_confirmation_required"
     PSE_DISPLAY_PAYMENT_PROCESSING = "pse_display_payment_processing"
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/next_step_display_payment_method_information_type.py` & `fern_belvo-0.0.34/src/belvo/types/next_step_display_payment_method_information_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 import enum
 import typing
 
 T_Result = typing.TypeVar("T_Result")
 
 
 class NextStepDisplayPaymentMethodInformationType(str, enum.Enum):
+    """
+    The type of `next_step` you need to follow.
+    """
+
     OPEN_FINANCE_DISPLAY_PAYMENT_METHOD_INFORMATION = "open_finance_display_payment_method_information"
     OPEN_FINANCE_DISPLAY_CONFIRMATION_REQUIRED = "open_finance_display_confirmation_required"
     OPEN_FINANCE_DISPLAY_NEEDS_REDIRECT = "open_finance_display_needs_redirect"
     OPEN_FINANCE_DISPLAY_PAYMENT_PROCESSING = "open_finance_display_payment_processing"
     OPEN_FINANCE_DISPLAY_PAYMENT_SUCCEEDED = "open_finance_display_payment_succeeded"
     OPEN_FINANCE_DISPLAY_PAYMENT_FAILED = "open_finance_display_payment_failed"
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/next_step_display_payment_processing.py` & `fern_belvo-0.0.34/src/belvo/types/next_step_display_payment_processing.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/next_step_display_payment_processing_type.py` & `fern_belvo-0.0.34/src/belvo/types/next_step_display_payment_processing_type.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 import enum
 import typing
 
 T_Result = typing.TypeVar("T_Result")
 
 
 class NextStepDisplayPaymentProcessingType(str, enum.Enum):
+    """
+    The type of `next_step` you need to follow.
+    """
+
     OPEN_FINANCE_DISPLAY_PAYMENT_METHOD_INFORMATION = "open_finance_display_payment_method_information"
     OPEN_FINANCE_DISPLAY_CONFIRMATION_REQUIRED = "open_finance_display_confirmation_required"
     OPEN_FINANCE_DISPLAY_NEEDS_REDIRECT = "open_finance_display_needs_redirect"
     OPEN_FINANCE_DISPLAY_PAYMENT_PROCESSING = "open_finance_display_payment_processing"
     OPEN_FINANCE_DISPLAY_PAYMENT_SUCCEEDED = "open_finance_display_payment_succeeded"
     OPEN_FINANCE_DISPLAY_PAYMENT_FAILED = "open_finance_display_payment_failed"
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/next_step_display_payment_succeeded.py` & `fern_belvo-0.0.34/src/belvo/types/next_step_display_payment_succeeded.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/next_step_display_payment_succeeded_type.py` & `fern_belvo-0.0.34/src/belvo/types/next_step_display_payment_succeeded_type.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 import enum
 import typing
 
 T_Result = typing.TypeVar("T_Result")
 
 
 class NextStepDisplayPaymentSucceededType(str, enum.Enum):
+    """
+    The type of `next_step` you need to follow.
+    """
+
     OPEN_FINANCE_DISPLAY_PAYMENT_METHOD_INFORMATION = "open_finance_display_payment_method_information"
     OPEN_FINANCE_DISPLAY_CONFIRMATION_REQUIRED = "open_finance_display_confirmation_required"
     OPEN_FINANCE_DISPLAY_NEEDS_REDIRECT = "open_finance_display_needs_redirect"
     OPEN_FINANCE_DISPLAY_PAYMENT_PROCESSING = "open_finance_display_payment_processing"
     OPEN_FINANCE_DISPLAY_PAYMENT_SUCCEEDED = "open_finance_display_payment_succeeded"
     OPEN_FINANCE_DISPLAY_PAYMENT_FAILED = "open_finance_display_payment_failed"
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/next_step_display_token_required_pse.py` & `fern_belvo-0.0.34/src/belvo/types/next_step_display_token_required_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/next_step_display_token_required_pse_type.py` & `fern_belvo-0.0.34/src/belvo/types/next_step_display_token_required_pse_type.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 import enum
 import typing
 
 T_Result = typing.TypeVar("T_Result")
 
 
 class NextStepDisplayTokenRequiredPseType(str, enum.Enum):
+    """
+    The type of `next_step` you need to follow.
+    """
+
     PSE_DISPLAY_PAYMENT_METHOD_INFORMATION = "pse_display_payment_method_information"
     PSE_DISPLAY_CREDENTIALS_REQUIRED = "pse_display_credentials_required"
     PSE_DISPLAY_NEEDS_REDIRECT = "pse_display_needs_redirect"
     PSE_DISPLAY_TOKEN_REQUIRED = "pse_display_token_required"
     PSE_DISPLAY_CUSTOMER_BANK_ACCOUNTS = "pse_display_customer_bank_accounts"
     PSE_DISPLAY_CONFIRMATION_REQUIRED = "pse_display_confirmation_required"
     PSE_DISPLAY_PAYMENT_PROCESSING = "pse_display_payment_processing"
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/next_step_needs_redirect.py` & `fern_belvo-0.0.34/src/belvo/types/next_step_needs_redirect.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/next_step_needs_redirect_type.py` & `fern_belvo-0.0.34/src/belvo/types/next_step_display_payment_failed_type.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,15 +2,19 @@
 
 import enum
 import typing
 
 T_Result = typing.TypeVar("T_Result")
 
 
-class NextStepNeedsRedirectType(str, enum.Enum):
+class NextStepDisplayPaymentFailedType(str, enum.Enum):
+    """
+    The type of `next_step` you need to follow.
+    """
+
     OPEN_FINANCE_DISPLAY_PAYMENT_METHOD_INFORMATION = "open_finance_display_payment_method_information"
     OPEN_FINANCE_DISPLAY_CONFIRMATION_REQUIRED = "open_finance_display_confirmation_required"
     OPEN_FINANCE_DISPLAY_NEEDS_REDIRECT = "open_finance_display_needs_redirect"
     OPEN_FINANCE_DISPLAY_PAYMENT_PROCESSING = "open_finance_display_payment_processing"
     OPEN_FINANCE_DISPLAY_PAYMENT_SUCCEEDED = "open_finance_display_payment_succeeded"
     OPEN_FINANCE_DISPLAY_PAYMENT_FAILED = "open_finance_display_payment_failed"
 
@@ -19,19 +23,19 @@
         open_finance_display_payment_method_information: typing.Callable[[], T_Result],
         open_finance_display_confirmation_required: typing.Callable[[], T_Result],
         open_finance_display_needs_redirect: typing.Callable[[], T_Result],
         open_finance_display_payment_processing: typing.Callable[[], T_Result],
         open_finance_display_payment_succeeded: typing.Callable[[], T_Result],
         open_finance_display_payment_failed: typing.Callable[[], T_Result],
     ) -> T_Result:
-        if self is NextStepNeedsRedirectType.OPEN_FINANCE_DISPLAY_PAYMENT_METHOD_INFORMATION:
+        if self is NextStepDisplayPaymentFailedType.OPEN_FINANCE_DISPLAY_PAYMENT_METHOD_INFORMATION:
             return open_finance_display_payment_method_information()
-        if self is NextStepNeedsRedirectType.OPEN_FINANCE_DISPLAY_CONFIRMATION_REQUIRED:
+        if self is NextStepDisplayPaymentFailedType.OPEN_FINANCE_DISPLAY_CONFIRMATION_REQUIRED:
             return open_finance_display_confirmation_required()
-        if self is NextStepNeedsRedirectType.OPEN_FINANCE_DISPLAY_NEEDS_REDIRECT:
+        if self is NextStepDisplayPaymentFailedType.OPEN_FINANCE_DISPLAY_NEEDS_REDIRECT:
             return open_finance_display_needs_redirect()
-        if self is NextStepNeedsRedirectType.OPEN_FINANCE_DISPLAY_PAYMENT_PROCESSING:
+        if self is NextStepDisplayPaymentFailedType.OPEN_FINANCE_DISPLAY_PAYMENT_PROCESSING:
             return open_finance_display_payment_processing()
-        if self is NextStepNeedsRedirectType.OPEN_FINANCE_DISPLAY_PAYMENT_SUCCEEDED:
+        if self is NextStepDisplayPaymentFailedType.OPEN_FINANCE_DISPLAY_PAYMENT_SUCCEEDED:
             return open_finance_display_payment_succeeded()
-        if self is NextStepNeedsRedirectType.OPEN_FINANCE_DISPLAY_PAYMENT_FAILED:
+        if self is NextStepDisplayPaymentFailedType.OPEN_FINANCE_DISPLAY_PAYMENT_FAILED:
             return open_finance_display_payment_failed()
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/non_taxable_income_individual.py` & `fern_belvo-0.0.34/src/belvo/types/non_taxable_income_individual.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/not_found_error_body.py` & `fern_belvo-0.0.34/src/belvo/types/not_found_error_body.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/owner.py` & `fern_belvo-0.0.34/src/belvo/types/owner.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/owner_document_id.py` & `fern_belvo-0.0.34/src/belvo/types/owner_document_id.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
 class OwnerDocumentId(pydantic.BaseModel):
+    """
+    Information regarding the identification document the owner provided to the bank.
+    """
+
     document_type: typing.Optional[str] = pydantic.Field(
         description=(
             "The type of document the owner provided to the institution to open the account. Common document types are:\n"
             "\n"
             "🇧🇷 Brazil\n"
             "- `CPF` (*Cadastro de Pessoas Físicas*)\n"
             "- `CNPJ`(*Cadastro Nacional de Pessoas Jurídicas*)\n"
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/owners_paginated_response.py` & `fern_belvo-0.0.34/src/belvo/types/tax_retentions_paginated_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,30 +2,32 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .owner import Owner
+from .tax_retentions import TaxRetentions
 
 
-class OwnersPaginatedResponse(pydantic.BaseModel):
+class TaxRetentionsPaginatedResponse(pydantic.BaseModel):
     count: typing.Optional[int] = pydantic.Field(description=("The total number of results in your Belvo account.\n"))
     next: typing.Optional[str] = pydantic.Field(
         description=(
             "The URL to next page of results. Each page consists of up to 100 items. If there are not enough results for an additional page, the value is `null`.\n"
             "\n"
             "In our documentation example, we use `{endpoint}` as a placeholder value. In production, this value will be replaced by the actual endpoint you are currently using (for example, `accounts` or `owners`).\n"
         )
     )
     previous: typing.Optional[str] = pydantic.Field(
         description=("The URL to the previous page of results. If there is no previous page, the value is `null`.\n")
     )
-    results: typing.Optional[typing.List[Owner]] = pydantic.Field(description=("Array of owner objects.\n"))
+    results: typing.Optional[typing.List[TaxRetentions]] = pydantic.Field(
+        description=("Array of tax retentions objects.\n")
+    )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/paginated_response_link.py` & `fern_belvo-0.0.34/src/belvo/types/paginated_response_link.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/patch_body.py` & `fern_belvo-0.0.34/src/belvo/types/patch_body.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/patch_body_without_save_data.py` & `fern_belvo-0.0.34/src/belvo/types/patch_body_without_save_data.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/patch_payment_intents_body_pse.py` & `fern_belvo-0.0.34/src/belvo/types/patch_payment_intents_body_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/patch_payment_method_details_pse.py` & `fern_belvo-0.0.34/src/belvo/types/patch_payment_method_details_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/payment_institution.py` & `fern_belvo-0.0.34/src/belvo/types/payment_institution.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/payment_intent_ofpi.py` & `fern_belvo-0.0.34/src/belvo/types/payment_intent_ofpi.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/payment_intent_ofpi_next_step.py` & `fern_belvo-0.0.34/src/belvo/types/payment_intent_ofpi_next_step.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/payment_intent_paginated_response.py` & `fern_belvo-0.0.34/src/belvo/types/payment_intent_paginated_response.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/payment_intent_payment_method_details_body_business_ofpi.py` & `fern_belvo-0.0.34/src/belvo/types/payment_intent_payment_method_details_body_business_ofpi.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/payment_intent_payment_method_details_body_individual_ofpi.py` & `fern_belvo-0.0.34/src/belvo/types/payment_intent_payment_method_details_body_individual_ofpi.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/payment_intent_payment_method_details_body_pse.py` & `fern_belvo-0.0.34/src/belvo/types/payment_intent_payment_method_details_body_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/payment_intent_payment_method_details_business_ofpi.py` & `fern_belvo-0.0.34/src/belvo/types/payment_intent_payment_method_details_business_ofpi.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/payment_intent_payment_method_details_individual_ofpi.py` & `fern_belvo-0.0.34/src/belvo/types/payment_intent_payment_method_details_individual_ofpi.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/payment_intent_payment_method_details_pse.py` & `fern_belvo-0.0.34/src/belvo/types/payment_intent_payment_method_details_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/payment_intent_pse.py` & `fern_belvo-0.0.34/src/belvo/types/payment_intent_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/payment_intent_pse_last_error.py` & `fern_belvo-0.0.34/src/belvo/types/payment_intent_pse_last_error.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/payment_intent_pse_next_step.py` & `fern_belvo-0.0.34/src/belvo/types/payment_intent_pse_next_step.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/payment_intents_payment_method_details_body_pse.py` & `fern_belvo-0.0.34/src/belvo/types/payment_intents_payment_method_details_body_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/payment_intents_payment_method_details_pse.py` & `fern_belvo-0.0.34/src/belvo/types/payment_intents_payment_method_details_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/payment_link_callback_urls.py` & `fern_belvo-0.0.34/src/belvo/types/payment_link_callback_urls.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/payment_link_callback_urls_response.py` & `fern_belvo-0.0.34/src/belvo/types/payment_link_callback_urls_response.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/payment_link_list_ofpi.py` & `fern_belvo-0.0.34/src/belvo/types/payment_link_list_ofpi.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/payment_link_list_pse.py` & `fern_belvo-0.0.34/src/belvo/types/payment_link_list_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/payment_link_ofpi.py` & `fern_belvo-0.0.34/src/belvo/types/payment_link_ofpi.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/payment_link_paginated_response.py` & `fern_belvo-0.0.34/src/belvo/types/payment_link_paginated_response.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/payment_link_pse.py` & `fern_belvo-0.0.34/src/belvo/types/payment_link_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/payment_links_payment_method_details_body_ofpi.py` & `fern_belvo-0.0.34/src/belvo/types/payment_links_payment_method_details_body_ofpi.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/payment_links_payment_method_details_body_pse.py` & `fern_belvo-0.0.34/src/belvo/types/payment_links_payment_method_details_body_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/payment_method_details_ofpi.py` & `fern_belvo-0.0.34/src/belvo/types/payment_method_details_ofpi.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/payment_method_details_pse.py` & `fern_belvo-0.0.34/src/belvo/types/payment_method_details_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/payment_method_info_customer_bank_accounts_pse.py` & `fern_belvo-0.0.34/src/belvo/types/payment_method_info_customer_bank_accounts_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/payment_method_information_body_ofpi.py` & `fern_belvo-0.0.34/src/belvo/types/payment_method_information_body_ofpi.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/payment_method_information_body_pse.py` & `fern_belvo-0.0.34/src/belvo/types/payment_method_information_body_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/payment_method_information_details_pse.py` & `fern_belvo-0.0.34/src/belvo/types/payment_method_information_details_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/payment_method_information_ofpi.py` & `fern_belvo-0.0.34/src/belvo/types/payment_method_information_ofpi.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/payment_method_information_pse.py` & `fern_belvo-0.0.34/src/belvo/types/payment_method_information_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/payment_transaction.py` & `fern_belvo-0.0.34/src/belvo/types/payment_transaction.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/payment_webhook.py` & `fern_belvo-0.0.34/src/belvo/types/tax_payer_information_business.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,30 +2,33 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
+from .document_id_business import DocumentIdBusiness
+from .reporting_id import ReportingId
 
 
-class PaymentWebhook(pydantic.BaseModel):
-    id: str = pydantic.Field(description=("Belvo's unique ID for the webhook.\n"))
-    name: typing.Any
-    url: str = pydantic.Field(description=("The URL where webhook events should be sent to.\n"))
-    auth_header: typing.Optional[str] = pydantic.Field(
-        description=("The authentication header for the request. **Must** be set to `Authorization`.\n")
+class TaxPayerInformationBusiness(pydantic.BaseModel):
+    """
+    Object containing information about the tax payer.
+    """
+
+    first_last_name: typing.Optional[str] = pydantic.Field(description=("The tax payer's first last name.\n"))
+    second_last_name: typing.Optional[str] = pydantic.Field(description=("The tax payer's second last name.\n"))
+    first_name: typing.Optional[str] = pydantic.Field(description=("The tax payer's first name.\n"))
+    other_names: typing.Optional[str] = pydantic.Field(description=("Additional names of the tax payer.\n"))
+    company_name: str = pydantic.Field(description=("The name of the company, as registered at the institution.\n"))
+    main_economic_activity: str = pydantic.Field(
+        description=("The main economic activity the tax payer is involved in.\n")
     )
-    auth_token: typing.Optional[str] = pydantic.Field(
-        description=("The authentication token you need to send webhook events. This value is obfuscated.\n")
-    )
-    created_at: str = pydantic.Field(
-        description=("The ISO-8601 timestamp of when the webhook was created in our database.\n")
-    )
-    created_by: str = pydantic.Field(description=("Belvo's unique ID of the user that created the webhook.\n"))
+    document_id: DocumentIdBusiness
+    reporting_id: ReportingId
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/payments_institutions_paginated_response.py` & `fern_belvo-0.0.34/src/belvo/types/payments_institutions_paginated_response.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/payments_transactions_paginated_response.py` & `fern_belvo-0.0.34/src/belvo/types/payments_transactions_paginated_response.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/payments_way.py` & `fern_belvo-0.0.34/src/belvo/types/payments_way.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/payments_webhooks_paginated_response.py` & `fern_belvo-0.0.34/src/belvo/types/payments_webhooks_paginated_response.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/pension_income_statement_individual.py` & `fern_belvo-0.0.34/src/belvo/types/pension_income_statement_individual.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/providers_pse.py` & `fern_belvo-0.0.34/src/belvo/types/providers_pse.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/receivables_transaction.py` & `fern_belvo-0.0.34/src/belvo/types/receivables_transaction.py`

 * *Files 17% similar despite different names*

```diff
@@ -38,20 +38,20 @@
             "- 🇧🇷 BRL (Brazilian Real)\n"
             "- 🇨🇴 COP (Colombian Peso)\n"
             "- 🇲🇽 MXN (Mexican Peso)\n"
             "\n"
             " Please note that currencies other than those listed above may be returned.\n"
         )
     )
-    type: EnumReceivableTransactionType
+    type: typing.Optional[EnumReceivableTransactionType]
     gross_amount: typing.Optional[float] = pydantic.Field(description=("The total gross amount of the transaction.\n"))
     net_amount: typing.Optional[float] = pydantic.Field(description=("The net amount of the transaction.\n"))
     fees: typing.List[RecevablesTransactionFees]
-    status: EnumReceivableTransactionStatus
-    number_of_installments: ReceivablesTransactionNumberOfInstallments
+    status: typing.Optional[EnumReceivableTransactionStatus]
+    number_of_installments: typing.Optional[ReceivablesTransactionNumberOfInstallments]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/receivables_transaction_account.py` & `fern_belvo-0.0.34/src/belvo/types/receivables_transaction_account.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/receivables_transaction_number_of_installments.py` & `fern_belvo-0.0.34/src/belvo/types/receivables_transaction_number_of_installments.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
 class ReceivablesTransactionNumberOfInstallments(pydantic.BaseModel):
+    """
+    Details regarding the number of installments for the transaction, if applicable.
+    """
+
     paid: typing.Optional[int] = pydantic.Field(
         description=("The number of payments already made to pay the cost of the transaction.\n")
     )
     total: typing.Optional[int] = pydantic.Field(
         description=("The number of payments required to pay the cost of the transaction.\n")
     )
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/receivables_transactions_paginated_response.py` & `fern_belvo-0.0.34/src/belvo/types/receivables_transactions_paginated_response.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/recevables_transaction_fees.py` & `fern_belvo-0.0.34/src/belvo/types/recevables_transaction_fees.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 class RecevablesTransactionFees(pydantic.BaseModel):
     """
     Details regarding the fees applied to the transaction.
     """
 
-    type: EnumReceivableTransactionFeeType
+    type: typing.Optional[EnumReceivableTransactionFeeType]
     value: float = pydantic.Field(description=("The value of `fees.type`.\n"))
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/recurring_expense_source_transaction.py` & `fern_belvo-0.0.34/src/belvo/types/recurring_expense_source_transaction.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
 class RecurringExpenseSourceTransaction(pydantic.BaseModel):
+    """
+    An array of minified transaction objects used to evaluate the recurring expense. If no transactions were found, we return an empty array.
+    """
+
     amount: float = pydantic.Field(description=("The transaction amount.\n"))
     description: typing.Optional[str] = pydantic.Field(
         description=(
             "The description of the transaction provided by the institution. Usually, this is the text that the end user would see in the bank statement. The description can be an empty string.\n"
         )
     )
     value_date: str = pydantic.Field(description=("The date when the transaction occurred, in `YYYY-MM-DD` format.\n"))
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/recurring_expenses.py` & `fern_belvo-0.0.34/src/belvo/types/recurring_expenses.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,23 +20,23 @@
 
     ℹ️ If no recurring expense insights are found, we return an empty array.
     """
 
     id: typing.Optional[str] = pydantic.Field(
         description=("Belvo's unique identifier used to reference the current recurring expense.\n")
     )
-    account: Account
+    account: typing.Optional[Account]
     name: typing.Optional[str] = pydantic.Field(
         description=(
             "The name for the recurring expense.\n"
             "\n"
             'ℹ️ **Note**: This information is taken from the description section of a transaction and then normalized to provide you with an easy-to-read name. As such, sometimes the name will reflect the merchant the payment is made to (for example, Netflix.com), while for other recurring expenses, this could be something like "Monthly payment to John".\n'
         )
     )
-    transactions: typing.List[RecurringExpenseSourceTransaction] = pydantic.Field(
+    transactions: typing.List[typing.Optional[RecurringExpenseSourceTransaction]] = pydantic.Field(
         description=(
             "An array of minified transaction objects used to evaluate the recurring expense. If no transactions were found, we return an empty array.\n"
         )
     )
     frequency: EnumRecurringExpenseFrequency
     average_transaction_amount: float = pydantic.Field(
         description=("The average transaction amount of the recurring expense.\n")
@@ -48,15 +48,15 @@
         description=(
             "Number of days since the last recurring expense occurred.\n"
             "\n"
             "Based on the frequency, you can infer how many days until the next charge will occur.\n"
         )
     )
     category: EnumRecurringExpenseCategory
-    payment_type: EnumRecurringExpensePaymentType
+    payment_type: typing.Optional[EnumRecurringExpensePaymentType]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/recurring_expenses_paginated_response.py` & `fern_belvo-0.0.34/src/belvo/types/recurring_expenses_paginated_response.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/reporting_id.py` & `fern_belvo-0.0.34/src/belvo/types/reporting_id.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/request_timeout_error_body.py` & `fern_belvo-0.0.34/src/belvo/types/request_timeout_error_body.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/retention_breakdown.py` & `fern_belvo-0.0.34/src/belvo/types/retention_breakdown.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     )
     tax_type: typing.Optional[str] = pydantic.Field(
         description=(
             "Optional attribute to indicate the type of tax withheld for the period or year according to the [SAT catalog](https://developers.belvo.com/docs/sat-catalogs#retention-code).\n"
         )
     )
     retained_amount: typing.Optional[float] = pydantic.Field(description=("The amount retained.\n"))
-    payment_status: EnumTaxRetentionPaymentStatus
+    payment_status: typing.Optional[EnumTaxRetentionPaymentStatus]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/risk_insights.py` & `fern_belvo-0.0.34/src/belvo/types/risk_insights.py`

 * *Files 17% similar despite different names*

```diff
@@ -20,19 +20,19 @@
         description=(
             "An array of Belvo-generated account numbers (UUIDs) that were used during the risk insights analysis. If no accounts were found, we return an empty array.\n"
         )
     )
     created_at: str = pydantic.Field(
         description=("The ISO-8601 timestamp of when the data point was last updated in Belvo's database.\n")
     )
-    transactions_metrics: RiskInsightsTransactionMetrics
-    balances_metrics: RiskInsightsBalanceMetrics
-    cashflow_metrics: RiskInsightsCashflowMetrics
-    credit_cards_metrics: RiskInsightsCreditCardMetrics
-    loans_metrics: RiskInsightsLoansMetrics
+    transactions_metrics: typing.Optional[RiskInsightsTransactionMetrics]
+    balances_metrics: typing.Optional[RiskInsightsBalanceMetrics]
+    cashflow_metrics: typing.Optional[RiskInsightsCashflowMetrics]
+    credit_cards_metrics: typing.Optional[RiskInsightsCreditCardMetrics]
+    loans_metrics: typing.Optional[RiskInsightsLoansMetrics]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/risk_insights_balance_metrics.py` & `fern_belvo-0.0.34/src/belvo/types/risk_insights_balance_metrics.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
 class RiskInsightsBalanceMetrics(pydantic.BaseModel):
+    """
+    Balance metrics calculated based on the user's balances from checking and savings accounts.
+    """
+
     min_balance_1_w: typing.Optional[float] = pydantic.Field(
         alias="min_balance_1w", description=("The minimum balance in the period (one week).\n")
     )
     min_balance_1_m: typing.Optional[float] = pydantic.Field(
         alias="min_balance_1m", description=("The minimum balance in the period (one month).\n")
     )
     min_balance_3_m: typing.Optional[float] = pydantic.Field(
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/risk_insights_cashflow_metrics.py` & `fern_belvo-0.0.34/src/belvo/types/risk_insights_cashflow_metrics.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,20 @@
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
 class RiskInsightsCashflowMetrics(pydantic.BaseModel):
+    """
+    Aggregated metrics calculated based on the user's transactions from checking, savings, credit, and loan accounts.
+
+    However, internal transfers (transfers between accounts belonging to the same link) are not used in the calculation.
+    """
+
     sum_positive_1_w: typing.Optional[float] = pydantic.Field(
         alias="sum_positive_1w",
         description=(
             "Sum total of all transactions leading to a positive cashflow in the last week (counted from the time of the request).\n"
         ),
     )
     sum_positive_1_m: typing.Optional[float] = pydantic.Field(
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/risk_insights_credit_card_metrics.py` & `fern_belvo-0.0.34/src/belvo/types/risk_insights_credit_card_metrics.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
 class RiskInsightsCreditCardMetrics(pydantic.BaseModel):
+    """
+    Aggregated metrics calculated based on the link's credit card accounts.
+    """
+
     num_accounts: int = pydantic.Field(description=("Number of credit cards accounts associated to the link.\n"))
     sum_credit_limit: typing.Optional[float] = pydantic.Field(description=("Sum total of all credit cards' limits.\n"))
     sum_credit_used: typing.Optional[float] = pydantic.Field(description=("Sum total of all credit used.\n"))
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/risk_insights_loans_metrics.py` & `fern_belvo-0.0.34/src/belvo/types/risk_insights_loans_metrics.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
 class RiskInsightsLoansMetrics(pydantic.BaseModel):
+    """
+    Aggregated metrics calculated based on the user's loan accounts.
+    """
+
     num_accounts: int = pydantic.Field(description=("Number of loan accounts associated with the link.\n"))
     sum_loans_principal: typing.Optional[float] = pydantic.Field(
         description=("Sum total of the principal for all of the link's loan accounts.\n")
     )
     sum_loans_outstanding_principal: typing.Optional[float] = pydantic.Field(
         description=("Sum total of the outstanding principal for all the link's loan accounts.\n")
     )
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/risk_insights_paginated_response.py` & `fern_belvo-0.0.34/src/belvo/types/risk_insights_paginated_response.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/risk_insights_transaction_metrics.py` & `fern_belvo-0.0.34/src/belvo/types/risk_insights_transaction_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
 class RiskInsightsTransactionMetrics(pydantic.BaseModel):
+    """
+    Aggregated metrics calculated band on the user's transactions from checking, savings, credit card, and loan accounts.
+    """
+
     num_transactions_1_w: int = pydantic.Field(
         alias="num_transactions_1w",
         description=(
             "The total number of transactions analyzed to determine the risk insights for the last week (incoming and outgoing).\n"
         ),
     )
     num_transactions_1_m: int = pydantic.Field(
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/secret_keys.py` & `fern_belvo-0.0.34/src/belvo/types/secret_keys.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/secret_keys_paginated_response.py` & `fern_belvo-0.0.34/src/belvo/types/secret_keys_paginated_response.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/session_expired_error.py` & `fern_belvo-0.0.34/src/belvo/types/session_expired_error.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/standard_request.py` & `fern_belvo-0.0.34/src/belvo/types/standard_request.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/tax_assessment_business.py` & `fern_belvo-0.0.34/src/belvo/types/tax_assessment_business.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/tax_assessment_individual.py` & `fern_belvo-0.0.34/src/belvo/types/tax_assessment_individual.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/tax_compliance_status.py` & `fern_belvo-0.0.34/src/belvo/types/tax_compliance_status.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/tax_compliance_status_paginated_response.py` & `fern_belvo-0.0.34/src/belvo/types/tax_compliance_status_paginated_response.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/tax_declaration_business.py` & `fern_belvo-0.0.34/src/belvo/types/tax_declaration_business.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/tax_declaration_business_paginated.py` & `fern_belvo-0.0.34/src/belvo/types/tax_declaration_business_paginated.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/tax_declaration_individual.py` & `fern_belvo-0.0.34/src/belvo/types/tax_declaration_individual.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/tax_declaration_individual_paginated.py` & `fern_belvo-0.0.34/src/belvo/types/tax_declaration_individual_paginated.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/tax_payer_information_business.py` & `fern_belvo-0.0.34/src/belvo/types/tax_status_address_dian.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,33 +2,38 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .document_id_business import DocumentIdBusiness
-from .reporting_id import ReportingId
+from .tax_status_address_between_street_dian import TaxStatusAddressBetweenStreetDian
 
 
-class TaxPayerInformationBusiness(pydantic.BaseModel):
+class TaxStatusAddressDian(pydantic.BaseModel):
     """
-    Object containing information about the tax payer.
+    The tax payer's address details.
     """
 
-    first_last_name: typing.Optional[str] = pydantic.Field(description=("The tax payer's first last name.\n"))
-    second_last_name: typing.Optional[str] = pydantic.Field(description=("The tax payer's second last name.\n"))
-    first_name: typing.Optional[str] = pydantic.Field(description=("The tax payer's first name.\n"))
-    other_names: typing.Optional[str] = pydantic.Field(description=("Additional names of the tax payer.\n"))
-    company_name: str = pydantic.Field(description=("The name of the company, as registered at the institution.\n"))
-    main_economic_activity: str = pydantic.Field(
-        description=("The main economic activity the tax payer is involved in.\n")
+    postal_code: typing.Optional[str] = pydantic.Field(description=("The postcode of the address.\n"))
+    street_type: typing.Optional[str] = pydantic.Field(description=("The `street` type.\n"))
+    street: typing.Optional[str] = pydantic.Field(description=("The tax payers street.\n"))
+    exterior_number: typing.Optional[str] = pydantic.Field(description=("The street number.\n"))
+    interior_number: typing.Optional[str] = pydantic.Field(description=("Additional address information.\n"))
+    suburb: typing.Optional[str] = pydantic.Field(
+        description=("**Note**: This field is not applicable for DIAN Colombia and will return `null`.\n")
+    )
+    locality: typing.Optional[str] = pydantic.Field(
+        description=("**Note**: This field is not applicable for DIAN Colombia and will return `null`.\n")
+    )
+    municipality: typing.Optional[str] = pydantic.Field(description=("The municipality of the address.\n"))
+    state: typing.Optional[str] = pydantic.Field(description=("The state that the address is in.\n"))
+    between_street: typing.Optional[typing.List[TaxStatusAddressBetweenStreetDian]] = pydantic.Field(
+        description=("**Note**: This field is not applicable for DIAN Colombia and will return `null`.\n")
     )
-    document_id: DocumentIdBusiness
-    reporting_id: ReportingId
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/tax_payer_information_individual.py` & `fern_belvo-0.0.34/src/belvo/types/tax_payer_information_individual.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/tax_retentions.py` & `fern_belvo-0.0.34/src/belvo/types/tax_retentions.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         description=("The ISO-8601 timestamp of when the tax retention was certified.\n")
     )
     cancelled_at: typing.Optional[str] = pydantic.Field(
         description=("The ISO-8601 timestamp of when the tax retention was canceled (if applicable).\n")
     )
     sender_id: typing.Optional[str] = pydantic.Field(description=("The fiscal ID of the invoice sender.\n"))
     sender_name: typing.Optional[str] = pydantic.Field(description=("The name of the invoice sender.\n"))
-    receiver_nationality: EnumTaxRetentionReceiverNationality
+    receiver_nationality: typing.Optional[EnumTaxRetentionReceiverNationality]
     receiver_id: typing.Optional[str] = pydantic.Field(description=("The fiscal ID of the invoice receiver.\n"))
     receiver_name: typing.Optional[str] = pydantic.Field(description=("The name of the invoice receiver.\n"))
     total_invoice_amount: typing.Optional[float] = pydantic.Field(
         description=("The total amount of the invoice that the tax retention relates to.\n")
     )
     total_exempt_amount: typing.Optional[float] = pydantic.Field(
         description=("Total amount that is exempt from taxation.\n")
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/tax_retentions_paginated_response.py` & `fern_belvo-0.0.34/src/belvo/types/tax_returns_personal_monthly_paginated.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,31 +2,31 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .tax_retentions import TaxRetentions
+from .tax_return_personal_monthly import TaxReturnPersonalMonthly
 
 
-class TaxRetentionsPaginatedResponse(pydantic.BaseModel):
+class TaxReturnsPersonalMonthlyPaginated(pydantic.BaseModel):
     count: typing.Optional[int] = pydantic.Field(description=("The total number of results in your Belvo account.\n"))
     next: typing.Optional[str] = pydantic.Field(
         description=(
             "The URL to next page of results. Each page consists of up to 100 items. If there are not enough results for an additional page, the value is `null`.\n"
             "\n"
             "In our documentation example, we use `{endpoint}` as a placeholder value. In production, this value will be replaced by the actual endpoint you are currently using (for example, `accounts` or `owners`).\n"
         )
     )
     previous: typing.Optional[str] = pydantic.Field(
         description=("The URL to the previous page of results. If there is no previous page, the value is `null`.\n")
     )
-    results: typing.Optional[typing.List[TaxRetentions]] = pydantic.Field(
-        description=("Array of tax retentions objects.\n")
+    results: typing.Optional[typing.List[TaxReturnPersonalMonthly]] = pydantic.Field(
+        description=("Array of Monthly Personal Tax Return objects.\n")
     )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/tax_return_business.py` & `fern_belvo-0.0.34/src/belvo/types/tax_return_business.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/tax_return_business_monthly.py` & `fern_belvo-0.0.34/src/belvo/types/tax_return_business_monthly.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/tax_return_personal.py` & `fern_belvo-0.0.34/src/belvo/types/tax_return_personal.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/tax_return_personal_monthly.py` & `fern_belvo-0.0.34/src/belvo/types/tax_return_personal_monthly.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/tax_returns_business_monthly_paginated.py` & `fern_belvo-0.0.34/src/belvo/types/tax_returns_business_monthly_paginated.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/tax_returns_business_paginated.py` & `fern_belvo-0.0.34/src/belvo/types/tax_returns_business_paginated.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/tax_returns_monthly_request.py` & `fern_belvo-0.0.34/src/belvo/types/tax_returns_monthly_request.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/tax_returns_personal_monthly_paginated.py` & `fern_belvo-0.0.34/src/belvo/types/tax_status_paginated_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,31 +2,31 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .tax_return_personal_monthly import TaxReturnPersonalMonthly
+from .tax_status_paginated_response_results_item import TaxStatusPaginatedResponseResultsItem
 
 
-class TaxReturnsPersonalMonthlyPaginated(pydantic.BaseModel):
+class TaxStatusPaginatedResponse(pydantic.BaseModel):
     count: typing.Optional[int] = pydantic.Field(description=("The total number of results in your Belvo account.\n"))
     next: typing.Optional[str] = pydantic.Field(
         description=(
             "The URL to next page of results. Each page consists of up to 100 items. If there are not enough results for an additional page, the value is `null`.\n"
             "\n"
             "In our documentation example, we use `{endpoint}` as a placeholder value. In production, this value will be replaced by the actual endpoint you are currently using (for example, `accounts` or `owners`).\n"
         )
     )
     previous: typing.Optional[str] = pydantic.Field(
         description=("The URL to the previous page of results. If there is no previous page, the value is `null`.\n")
     )
-    results: typing.Optional[typing.List[TaxReturnPersonalMonthly]] = pydantic.Field(
-        description=("Array of Monthly Personal Tax Return objects.\n")
+    results: typing.Optional[typing.List[TaxStatusPaginatedResponseResultsItem]] = pydantic.Field(
+        description=("Array of tax status objects.\n")
     )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/tax_returns_personal_paginated.py` & `fern_belvo-0.0.34/src/belvo/types/tax_returns_personal_paginated.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/tax_returns_yearly_request.py` & `fern_belvo-0.0.34/src/belvo/types/tax_returns_yearly_request.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/tax_status_address_between_street_dian.py` & `fern_belvo-0.0.34/src/belvo/types/tax_status_address_between_street_dian.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/tax_status_address_between_street_sat.py` & `fern_belvo-0.0.34/src/belvo/types/tax_status_address_between_street_sat.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/tax_status_address_dian.py` & `fern_belvo-0.0.34/src/belvo/types/tax_status_tax_payer_information_dian.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,34 +2,52 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .tax_status_address_between_street_dian import TaxStatusAddressBetweenStreetDian
 
 
-class TaxStatusAddressDian(pydantic.BaseModel):
-    postal_code: typing.Optional[str] = pydantic.Field(description=("The postcode of the address.\n"))
-    street_type: typing.Optional[str] = pydantic.Field(description=("The `street` type.\n"))
-    street: typing.Optional[str] = pydantic.Field(description=("The tax payers street.\n"))
-    exterior_number: typing.Optional[str] = pydantic.Field(description=("The street number.\n"))
-    interior_number: typing.Optional[str] = pydantic.Field(description=("Additional address information.\n"))
-    suburb: typing.Optional[str] = pydantic.Field(
+class TaxStatusTaxPayerInformationDian(pydantic.BaseModel):
+    """
+    Details regarding the taxpayer.
+    """
+
+    rfc: typing.Optional[str] = pydantic.Field(description=("The tax payers's identification number (NIT).\n"))
+    curp: typing.Optional[str] = pydantic.Field(
+        description=("**Note**: This field is not applicable for DIAN Colombia and will return `null`.\n")
+    )
+    name: typing.Optional[str] = pydantic.Field(description=("The tax payers's first name.\n"))
+    first_last_name: typing.Optional[str] = pydantic.Field(description=("The tax payers's first last name.\n"))
+    second_last_name: typing.Optional[str] = pydantic.Field(description=("The tax payers's second last name.\n"))
+    start_operations_date: typing.Optional[str] = pydantic.Field(
         description=("**Note**: This field is not applicable for DIAN Colombia and will return `null`.\n")
     )
-    locality: typing.Optional[str] = pydantic.Field(
+    status_padron: typing.Optional[str] = pydantic.Field(
         description=("**Note**: This field is not applicable for DIAN Colombia and will return `null`.\n")
     )
-    municipality: typing.Optional[str] = pydantic.Field(description=("The municipality of the address.\n"))
-    state: typing.Optional[str] = pydantic.Field(description=("The state that the address is in.\n"))
-    between_street: typing.Optional[typing.List[TaxStatusAddressBetweenStreetDian]] = pydantic.Field(
+    last_status_change_date: typing.Optional[str] = pydantic.Field(
         description=("**Note**: This field is not applicable for DIAN Colombia and will return `null`.\n")
     )
+    commercial_name: typing.Optional[str] = pydantic.Field(
+        description=(
+            "The name of the business designated for consumers and the general public.\n"
+            "\n"
+            "**Note**: Only applicable for businesses.\n"
+        )
+    )
+    social_name: typing.Optional[str] = pydantic.Field(
+        description=(
+            "The unique and exclusive name within the national territory that companies receive for legal or administrative purposes.\n"
+            "**Note**: Only applicable for businesses.\n"
+        )
+    )
+    email: typing.Optional[str] = pydantic.Field(description=("Contact email address for the tax payer.\n"))
+    phone: typing.Optional[str] = pydantic.Field(description=("Contact phone number for the tax payer.\n"))
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/tax_status_address_sat.py` & `fern_belvo-0.0.34/src/belvo/types/tax_status_address_sat.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 from .tax_status_address_between_street_sat import TaxStatusAddressBetweenStreetSat
 
 
 class TaxStatusAddressSat(pydantic.BaseModel):
+    """
+    The tax payer's address details.
+    """
+
     postal_code: typing.Optional[str] = pydantic.Field(description=("The postcode of the address.\n"))
     street_type: typing.Optional[str] = pydantic.Field(description=("The `street` type.\n"))
     street: typing.Optional[str] = pydantic.Field(description=("The tax payers street.\n"))
     exterior_number: typing.Optional[str] = pydantic.Field(description=("The street number.\n"))
     interior_number: typing.Optional[str] = pydantic.Field(description=("Additional address information.\n"))
     suburb: typing.Optional[str] = pydantic.Field(description=("The suburb of the tax payer.\n"))
     locality: typing.Optional[str] = pydantic.Field(description=("The locality of the address.\n"))
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/tax_status_dian.py` & `fern_belvo-0.0.34/src/belvo/types/tax_status_dian.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,16 +31,16 @@
         description=(
             "The name of the business.\n" "\n" "Note: For individuals in Colombia, this field will return `null`.\n"
         )
     )
     id_cif: typing.Optional[str] = pydantic.Field(
         description=("The taxpayer's *Cédula de ciudadanía* (CC) ID. Only applicable for individuals.\n")
     )
-    tax_payer_information: TaxStatusTaxPayerInformationDian
-    address: TaxStatusAddressDian
+    tax_payer_information: typing.Optional[TaxStatusTaxPayerInformationDian]
+    address: typing.Optional[TaxStatusAddressDian]
     economic_activity: typing.Optional[typing.List[TaxStatusEconomicActivityDian]] = pydantic.Field(
         description=("A list of economic activity objects.\n")
     )
     regimes: typing.Optional[typing.List[TaxStatusRegimensDian]] = pydantic.Field(
         description=("A list of regimen objects.\n")
     )
     obligations: typing.Optional[typing.List[TaxStatusObligationsDian]] = pydantic.Field(
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/tax_status_economic_activity_dian.py` & `fern_belvo-0.0.34/src/belvo/types/tax_status_economic_activity_dian.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/tax_status_economic_activity_sat.py` & `fern_belvo-0.0.34/src/belvo/types/tax_status_economic_activity_sat.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/tax_status_obligations_dian.py` & `fern_belvo-0.0.34/src/belvo/types/tax_status_obligations_dian.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/tax_status_obligations_sat.py` & `fern_belvo-0.0.34/src/belvo/types/tax_status_obligations_sat.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/tax_status_paginated_response.py` & `fern_belvo-0.0.34/src/belvo/types/transactions_paginated_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,32 +2,30 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .tax_status_paginated_response_results_item import TaxStatusPaginatedResponseResultsItem
+from .transaction import Transaction
 
 
-class TaxStatusPaginatedResponse(pydantic.BaseModel):
+class TransactionsPaginatedResponse(pydantic.BaseModel):
     count: typing.Optional[int] = pydantic.Field(description=("The total number of results in your Belvo account.\n"))
     next: typing.Optional[str] = pydantic.Field(
         description=(
             "The URL to next page of results. Each page consists of up to 100 items. If there are not enough results for an additional page, the value is `null`.\n"
             "\n"
             "In our documentation example, we use `{endpoint}` as a placeholder value. In production, this value will be replaced by the actual endpoint you are currently using (for example, `accounts` or `owners`).\n"
         )
     )
     previous: typing.Optional[str] = pydantic.Field(
         description=("The URL to the previous page of results. If there is no previous page, the value is `null`.\n")
     )
-    results: typing.Optional[typing.List[TaxStatusPaginatedResponseResultsItem]] = pydantic.Field(
-        description=("Array of tax status objects.\n")
-    )
+    results: typing.Optional[typing.List[Transaction]] = pydantic.Field(description=("Array of transaction objects.\n"))
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/tax_status_regimens_dian.py` & `fern_belvo-0.0.34/src/belvo/types/tax_status_regimens_dian.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/tax_status_regimens_sat.py` & `fern_belvo-0.0.34/src/belvo/types/tax_status_regimens_sat.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/tax_status_sat.py` & `fern_belvo-0.0.34/src/belvo/types/tax_status_sat.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,16 @@
     place_and_date_of_issuance: typing.Optional[str] = pydantic.Field(
         description=("The place and date of that the tax status was issued.\n")
     )
     official_name: typing.Optional[str] = pydantic.Field(description=("The name of the person or business.\n"))
     id_cif: typing.Optional[str] = pydantic.Field(
         description=("The taxpayer's *Cédula de Identificación Fiscal* (CIF) ID.\n")
     )
-    tax_payer_information: TaxStatusTaxPayerInformationSat
-    address: TaxStatusAddressSat
+    tax_payer_information: typing.Optional[TaxStatusTaxPayerInformationSat]
+    address: typing.Optional[TaxStatusAddressSat]
     economic_activity: typing.Optional[typing.List[TaxStatusEconomicActivitySat]] = pydantic.Field(
         description=("A list of economic activity objects.\n")
     )
     regimes: typing.Optional[typing.List[TaxStatusRegimensSat]] = pydantic.Field(
         description=("A list of regimen objects.\n")
     )
     obligations: typing.Optional[typing.List[TaxStatusObligationsSat]] = pydantic.Field(
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/tax_status_tax_payer_information_dian.py` & `fern_belvo-0.0.34/src/belvo/types/tax_status_tax_payer_information_sat.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,30 +4,38 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class TaxStatusTaxPayerInformationDian(pydantic.BaseModel):
-    rfc: typing.Optional[str] = pydantic.Field(description=("The tax payers's identification number (NIT).\n"))
+class TaxStatusTaxPayerInformationSat(pydantic.BaseModel):
+    """
+    Details regarding the taxpayer.
+    """
+
+    rfc: typing.Optional[str] = pydantic.Field(
+        description=("The tax payers's identification number (For Mexico, this is the RFC).\n")
+    )
     curp: typing.Optional[str] = pydantic.Field(
-        description=("**Note**: This field is not applicable for DIAN Colombia and will return `null`.\n")
+        description=("The tax payers's *Clave Única de Registro de Población* (CURP) number.\n")
     )
     name: typing.Optional[str] = pydantic.Field(description=("The tax payers's first name.\n"))
     first_last_name: typing.Optional[str] = pydantic.Field(description=("The tax payers's first last name.\n"))
     second_last_name: typing.Optional[str] = pydantic.Field(description=("The tax payers's second last name.\n"))
     start_operations_date: typing.Optional[str] = pydantic.Field(
-        description=("**Note**: This field is not applicable for DIAN Colombia and will return `null`.\n")
+        description=("Date when the tax payer commenced taxable commercial activities.\n")
     )
     status_padron: typing.Optional[str] = pydantic.Field(
-        description=("**Note**: This field is not applicable for DIAN Colombia and will return `null`.\n")
+        description=(
+            "Status of the taxpayer in the Federal Register of Taxpayers (RFC). Can be `ACTIVO` or `INACTIVO`.\n"
+        )
     )
     last_status_change_date: typing.Optional[str] = pydantic.Field(
-        description=("**Note**: This field is not applicable for DIAN Colombia and will return `null`.\n")
+        description=("Date when `status_padron` was most recently updated.\n")
     )
     commercial_name: typing.Optional[str] = pydantic.Field(
         description=(
             "The name of the business designated for consumers and the general public.\n"
             "\n"
             "**Note**: Only applicable for businesses.\n"
         )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/token_required_response.py` & `fern_belvo-0.0.34/src/belvo/types/token_required_response.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/token_required_response_token_generation_data.py` & `fern_belvo-0.0.34/src/belvo/types/token_required_response_token_generation_data.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/too_many_sessions_error.py` & `fern_belvo-0.0.34/src/belvo/types/too_many_sessions_error.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/transaction.py` & `fern_belvo-0.0.34/src/belvo/types/transaction.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 
 class Transaction(pydantic.BaseModel):
     id: typing.Optional[str] = pydantic.Field(description=("Belvo's unique ID for the transaction.\n"))
     internal_identification: typing.Optional[str] = pydantic.Field(
         description=("The institution's internal identification for the transaction.\n")
     )
-    account: Account
+    account: typing.Optional[Account]
     collected_at: typing.Optional[str] = pydantic.Field(
         description=("The ISO-8601 timestamp when the data point was collected.\n")
     )
     created_at: typing.Optional[str] = pydantic.Field(
         description=("The ISO-8601 timestamp of when the data point was last updated in Belvo's database.\n")
     )
     value_date: typing.Optional[str] = pydantic.Field(
@@ -45,22 +45,22 @@
         description=(
             "The description of transaction provided by the institution. Usually this is the text that the end user sees in the online platform.\n"
         )
     )
     observations: typing.Optional[str] = pydantic.Field(
         description=("Additional observations provided by the institution on the transaction.\n")
     )
-    merchant: TransactionMerchantData
-    category: EnumTransactionCategory
+    merchant: typing.Optional[TransactionMerchantData]
+    category: typing.Optional[EnumTransactionCategory]
     subcategory: typing.Optional[EnumTransactionSubcategory]
     reference: typing.Optional[str] = pydantic.Field(
         description=("The reference number of the transaction, provided by the bank.\n")
     )
-    type: EnumTransactionType
-    status: EnumTransactionStatus
+    type: typing.Optional[EnumTransactionType]
+    status: typing.Optional[EnumTransactionStatus]
     credit_card_data: typing.Optional[TransactionCreditCardData]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/transaction_bank_account_body_pse.py` & `fern_belvo-0.0.34/src/belvo/types/invoice_warnings_sat.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,22 +4,21 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class TransactionBankAccountBodyPse(pydantic.BaseModel):
+class InvoiceWarningsSat(pydantic.BaseModel):
     """
-    Information about the payer's bank account. Belvo returns the bank account ID when the account is already saved in the Belvo database.
+    Object containing information about any warnings related to this invoice.
     """
 
-    bank_account: typing.Optional[str] = pydantic.Field(
-        description=("Belvo's unique identifier for the payer’s bank account.\n")
-    )
+    code: typing.Optional[str] = pydantic.Field(description=("The warning code.\n"))
+    message: typing.Optional[str] = pydantic.Field(description=("The description of the warning.\n"))
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/transaction_credit_card_data.py` & `fern_belvo-0.0.34/src/belvo/types/transaction_credit_card_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 from .enum_transaction_bill_status import EnumTransactionBillStatus
 
 
 class TransactionCreditCardData(pydantic.BaseModel):
+    """
+    Additional data provided by the institution for credit card transactions.
+    """
+
     collected_at: typing.Optional[str] = pydantic.Field(
         description=("The ISO-8601 timestamp when the data point was collected.\n")
     )
     bill_name: typing.Optional[str] = pydantic.Field(
         description=(
             "The title of the monthly credit card bill the transaction belongs to. The format of the returned value is institution specific, however, some common examples are:\n"
             "\n"
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/transaction_merchant_data.py` & `fern_belvo-0.0.34/src/belvo/types/accounts_receivables_data.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,18 +4,29 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class TransactionMerchantData(pydantic.BaseModel):
-    logo: typing.Optional[str] = pydantic.Field(description=("The URL to the merchant's logo.\n"))
-    website: typing.Optional[str] = pydantic.Field(description=("The URL to the merchant's website.\n"))
-    merchant_name: typing.Optional[str] = pydantic.Field(description=("The name of the merchant.\n"))
+class AccountsReceivablesData(pydantic.BaseModel):
+    """
+    Additional details regarding the receivables account, if applicable.
+    """
+
+    current: typing.Optional[float] = pydantic.Field(
+        description=("The total sum of all receivables (`available` + `anticipated`)\n")
+    )
+    available: typing.Optional[float] = pydantic.Field(
+        description=("The amount that the owner of the account will receive according to an established date.\n")
+    )
+    anticipated: typing.Optional[float] = pydantic.Field(
+        description=("The amount that the owner of the account received earlier than contracted.\n")
+    )
+    collected_at: str = pydantic.Field(description=("The ISO-8601 timestamp when the data point was collected.\n"))
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/transactions_paginated_response.py` & `fern_belvo-0.0.34/src/belvo/types/accounts_paginated_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,30 +2,32 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .transaction import Transaction
+from .account import Account
 
 
-class TransactionsPaginatedResponse(pydantic.BaseModel):
+class AccountsPaginatedResponse(pydantic.BaseModel):
     count: typing.Optional[int] = pydantic.Field(description=("The total number of results in your Belvo account.\n"))
     next: typing.Optional[str] = pydantic.Field(
         description=(
             "The URL to next page of results. Each page consists of up to 100 items. If there are not enough results for an additional page, the value is `null`.\n"
             "\n"
             "In our documentation example, we use `{endpoint}` as a placeholder value. In production, this value will be replaced by the actual endpoint you are currently using (for example, `accounts` or `owners`).\n"
         )
     )
     previous: typing.Optional[str] = pydantic.Field(
         description=("The URL to the previous page of results. If there is no previous page, the value is `null`.\n")
     )
-    results: typing.Optional[typing.List[Transaction]] = pydantic.Field(description=("Array of transaction objects.\n"))
+    results: typing.Optional[typing.List[typing.Optional[Account]]] = pydantic.Field(
+        description=("An array of Account objects.\n")
+    )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_belvo-0.0.33/src/belvo/types/transactions_request.py` & `fern_belvo-0.0.34/src/belvo/types/transactions_request.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/unauthorized_error_body.py` & `fern_belvo-0.0.34/src/belvo/types/unauthorized_error_body.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/unconfirmed_link_error.py` & `fern_belvo-0.0.34/src/belvo/types/unconfirmed_link_error.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/unexpected_error.py` & `fern_belvo-0.0.34/src/belvo/types/unexpected_error.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/unsupported_operation_error.py` & `fern_belvo-0.0.34/src/belvo/types/unsupported_operation_error.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/src/belvo/types/validation_error.py` & `fern_belvo-0.0.34/src/belvo/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `fern_belvo-0.0.33/PKG-INFO` & `fern_belvo-0.0.34/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fern-belvo
-Version: 0.0.33
+Version: 0.0.34
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

