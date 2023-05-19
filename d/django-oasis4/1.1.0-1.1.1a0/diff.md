# Comparing `tmp/django-oasis4-1.1.0.tar.gz` & `tmp/django-oasis4-1.1.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-oasis4-1.1.0.tar", last modified: Sat Mar 18 14:58:10 2023, max compression
+gzip compressed data, was "django-oasis4-1.1.1a0.tar", last modified: Fri May 19 22:12:01 2023, max compression
```

## Comparing `django-oasis4-1.1.0.tar` & `django-oasis4-1.1.1a0.tar`

### file list

```diff
@@ -1,130 +1,144 @@
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-18 14:58:10.917141 django-oasis4-1.1.0/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    11375 2023-01-23 20:26:24.000000 django-oasis4-1.1.0/LICENSE
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      144 2023-03-02 20:32:01.000000 django-oasis4-1.1.0/MANIFEST.in
--rw-r--r--   0 macercha  (1000) macercha  (1000)    13078 2023-03-18 14:58:10.917141 django-oasis4-1.1.0/PKG-INFO
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      217 2023-02-13 15:48:51.000000 django-oasis4-1.1.0/README.md
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-18 14:58:10.889141 django-oasis4-1.1.0/django_oasis4.egg-info/
--rw-r--r--   0 macercha  (1000) macercha  (1000)    13078 2023-03-18 14:58:10.000000 django-oasis4-1.1.0/django_oasis4.egg-info/PKG-INFO
--rw-r--r--   0 macercha  (1000) macercha  (1000)     4030 2023-03-18 14:58:10.000000 django-oasis4-1.1.0/django_oasis4.egg-info/SOURCES.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)        1 2023-03-18 14:58:10.000000 django-oasis4-1.1.0/django_oasis4.egg-info/dependency_links.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)       78 2023-03-18 14:58:10.000000 django-oasis4-1.1.0/django_oasis4.egg-info/requires.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)        6 2023-03-18 14:58:10.000000 django-oasis4-1.1.0/django_oasis4.egg-info/top_level.txt
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-18 14:58:10.890141 django-oasis4-1.1.0/oasis/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2022-12-10 23:55:40.000000 django-oasis4-1.1.0/oasis/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1394 2023-03-03 21:24:43.000000 django-oasis4-1.1.0/oasis/apps.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-18 14:58:10.891141 django-oasis4-1.1.0/oasis/coffee_offers/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-22 14:19:30.000000 django-oasis4-1.1.0/oasis/coffee_offers/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      686 2023-03-06 19:37:38.000000 django-oasis4-1.1.0/oasis/coffee_offers/admin.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1253 2023-03-07 16:31:05.000000 django-oasis4-1.1.0/oasis/coffee_offers/admin_views.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-18 14:58:10.891141 django-oasis4-1.1.0/oasis/coffee_offers/api/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-02-23 15:03:46.000000 django-oasis4-1.1.0/oasis/coffee_offers/api/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-18 14:58:10.892141 django-oasis4-1.1.0/oasis/coffee_offers/api/serializers/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      683 2023-03-06 19:10:13.000000 django-oasis4-1.1.0/oasis/coffee_offers/api/serializers/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      772 2023-02-23 15:21:03.000000 django-oasis4-1.1.0/oasis/coffee_offers/api/serializers/coffee_ware_house.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1199 2023-03-06 20:11:27.000000 django-oasis4-1.1.0/oasis/coffee_offers/api/serializers/offer.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-18 14:58:10.892141 django-oasis4-1.1.0/oasis/coffee_offers/api/services/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      580 2023-03-01 20:03:07.000000 django-oasis4-1.1.0/oasis/coffee_offers/api/services/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    11193 2023-03-16 14:42:57.000000 django-oasis4-1.1.0/oasis/coffee_offers/api/services/coffee_offers.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     4101 2023-03-16 21:48:47.000000 django-oasis4-1.1.0/oasis/coffee_offers/apps.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-18 14:58:10.892141 django-oasis4-1.1.0/oasis/coffee_offers/lib/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-02-26 20:27:18.000000 django-oasis4-1.1.0/oasis/coffee_offers/lib/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-18 14:58:10.893141 django-oasis4-1.1.0/oasis/coffee_offers/lib/choices/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      656 2023-02-26 20:35:07.000000 django-oasis4-1.1.0/oasis/coffee_offers/lib/choices/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1137 2023-03-07 09:29:38.000000 django-oasis4-1.1.0/oasis/coffee_offers/lib/choices/coffee_offers_states.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      739 2023-02-26 20:34:29.000000 django-oasis4-1.1.0/oasis/coffee_offers/lib/choices/oasis_states.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-18 14:58:10.894141 django-oasis4-1.1.0/oasis/coffee_offers/lib/events/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      417 2023-03-16 21:48:47.000000 django-oasis4-1.1.0/oasis/coffee_offers/lib/events/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      939 2023-03-16 21:48:47.000000 django-oasis4-1.1.0/oasis/coffee_offers/lib/events/on_post_save_offer.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-18 14:58:10.895141 django-oasis4-1.1.0/oasis/coffee_offers/lib/utils/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      595 2023-03-06 21:38:01.000000 django-oasis4-1.1.0/oasis/coffee_offers/lib/utils/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     3414 2023-03-16 14:42:57.000000 django-oasis4-1.1.0/oasis/coffee_offers/lib/utils/offer_state_machine.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-18 14:58:10.895141 django-oasis4-1.1.0/oasis/coffee_offers/lib/validators/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      757 2023-02-26 21:14:28.000000 django-oasis4-1.1.0/oasis/coffee_offers/lib/validators/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1336 2023-02-26 21:13:57.000000 django-oasis4-1.1.0/oasis/coffee_offers/lib/validators/date_validators.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      823 2023-02-26 20:45:48.000000 django-oasis4-1.1.0/oasis/coffee_offers/lib/validators/oasis_statuses.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-18 14:58:10.884141 django-oasis4-1.1.0/oasis/coffee_offers/locale/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-18 14:58:10.884141 django-oasis4-1.1.0/oasis/coffee_offers/locale/es/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-18 14:58:10.896141 django-oasis4-1.1.0/oasis/coffee_offers/locale/es/LC_MESSAGES/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     4521 2023-03-16 14:42:57.000000 django-oasis4-1.1.0/oasis/coffee_offers/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     6279 2023-03-16 14:42:57.000000 django-oasis4-1.1.0/oasis/coffee_offers/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-18 14:58:10.896141 django-oasis4-1.1.0/oasis/coffee_offers/tasks/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      595 2023-03-06 23:14:13.000000 django-oasis4-1.1.0/oasis/coffee_offers/tasks/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1365 2023-03-16 14:42:57.000000 django-oasis4-1.1.0/oasis/coffee_offers/tasks/sync_coffe_offers.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-18 14:58:10.897141 django-oasis4-1.1.0/oasis/coffee_offers/templates/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1072 2023-03-08 13:40:32.000000 django-oasis4-1.1.0/oasis/coffee_offers/templates/change_status.html
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      803 2023-03-08 13:40:32.000000 django-oasis4-1.1.0/oasis/coffee_offers/templates/change_status.txt
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-18 14:58:10.897141 django-oasis4-1.1.0/oasis/coffee_offers/templates/coffee_offers/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      123 2023-03-07 09:07:24.000000 django-oasis4-1.1.0/oasis/coffee_offers/templates/coffee_offers/contract_template.html
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      123 2023-03-07 09:07:24.000000 django-oasis4-1.1.0/oasis/coffee_offers/templates/coffee_offers/promisory_note.html
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      123 2023-03-07 09:07:24.000000 django-oasis4-1.1.0/oasis/coffee_offers/templates/coffee_offers/terms_conditions.html
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1054 2023-03-02 20:24:29.000000 django-oasis4-1.1.0/oasis/coffee_offers/templates/save_offer.html
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      785 2023-03-02 20:03:04.000000 django-oasis4-1.1.0/oasis/coffee_offers/templates/save_offer.txt
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      981 2023-03-16 14:42:57.000000 django-oasis4-1.1.0/oasis/coffee_offers/urls.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-18 14:58:10.898141 django-oasis4-1.1.0/oasis/lib/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2022-11-16 14:55:35.000000 django-oasis4-1.1.0/oasis/lib/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-18 14:58:10.898141 django-oasis4-1.1.0/oasis/lib/choices/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      582 2023-01-17 21:45:20.000000 django-oasis4-1.1.0/oasis/lib/choices/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      783 2022-12-20 11:38:24.000000 django-oasis4-1.1.0/oasis/lib/choices/customer_type.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-18 14:58:10.906141 django-oasis4-1.1.0/oasis/lib/managers/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1525 2023-03-16 14:42:57.000000 django-oasis4-1.1.0/oasis/lib/managers/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      780 2023-02-23 14:39:16.000000 django-oasis4-1.1.0/oasis/lib/managers/local_coffee_ware_house.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      682 2023-01-28 14:38:17.000000 django-oasis4-1.1.0/oasis/lib/managers/local_company.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1355 2023-01-18 02:07:35.000000 django-oasis4-1.1.0/oasis/lib/managers/local_document_type.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1578 2023-03-08 14:17:45.000000 django-oasis4-1.1.0/oasis/lib/managers/local_offer.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1212 2022-12-14 20:34:45.000000 django-oasis4-1.1.0/oasis/lib/managers/local_product.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2159 2023-03-16 14:42:57.000000 django-oasis4-1.1.0/oasis/lib/managers/local_state_machine.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1201 2023-03-02 21:35:32.000000 django-oasis4-1.1.0/oasis/lib/managers/oasis_associate_balance.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2701 2023-03-01 16:42:42.000000 django-oasis4-1.1.0/oasis/lib/managers/oasis_client.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1050 2023-01-27 03:47:52.000000 django-oasis4-1.1.0/oasis/lib/managers/oasis_company.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1390 2023-02-07 10:48:09.000000 django-oasis4-1.1.0/oasis/lib/managers/oasis_cycle.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     4007 2023-01-24 23:42:01.000000 django-oasis4-1.1.0/oasis/lib/managers/oasis_discount.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1180 2023-01-24 23:42:01.000000 django-oasis4-1.1.0/oasis/lib/managers/oasis_geographic_location.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      799 2023-02-23 14:57:09.000000 django-oasis4-1.1.0/oasis/lib/managers/oasis_location.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     7130 2023-03-08 14:56:20.000000 django-oasis4-1.1.0/oasis/lib/managers/oasis_operation.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      939 2023-02-06 19:28:19.000000 django-oasis4-1.1.0/oasis/lib/managers/oasis_periods.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      906 2022-12-19 16:49:04.000000 django-oasis4-1.1.0/oasis/lib/managers/oasis_product.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      730 2023-01-25 00:42:41.000000 django-oasis4-1.1.0/oasis/lib/managers/oasis_type_client.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-18 14:58:10.907141 django-oasis4-1.1.0/oasis/lib/serializers/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      658 2023-02-07 09:06:27.000000 django-oasis4-1.1.0/oasis/lib/serializers/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      789 2023-02-07 09:25:36.000000 django-oasis4-1.1.0/oasis/lib/serializers/oasis_cycle.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      803 2022-12-14 20:01:00.000000 django-oasis4-1.1.0/oasis/lib/serializers/product.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-18 14:58:10.908141 django-oasis4-1.1.0/oasis/lib/utils/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      579 2023-03-03 19:38:17.000000 django-oasis4-1.1.0/oasis/lib/utils/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     3274 2023-03-08 14:31:18.000000 django-oasis4-1.1.0/oasis/lib/utils/oasis_actions.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-18 14:58:10.886141 django-oasis4-1.1.0/oasis/locale/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-18 14:58:10.886141 django-oasis4-1.1.0/oasis/locale/es/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-18 14:58:10.908141 django-oasis4-1.1.0/oasis/locale/es/LC_MESSAGES/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1744 2023-02-08 01:14:00.000000 django-oasis4-1.1.0/oasis/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2663 2023-02-08 01:13:42.000000 django-oasis4-1.1.0/oasis/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-18 14:58:10.914141 django-oasis4-1.1.0/oasis/migrations/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    29691 2022-12-13 18:21:01.000000 django-oasis4-1.1.0/oasis/migrations/0001_initial.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    31003 2023-01-17 22:22:35.000000 django-oasis4-1.1.0/oasis/migrations/0002_geographiclocation_typeclient_documenttype_client_and_more.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    17130 2023-01-26 02:36:44.000000 django-oasis4-1.1.0/oasis/migrations/0003_oasiscompany_company.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     5814 2023-01-27 03:47:55.000000 django-oasis4-1.1.0/oasis/migrations/0004_account_vaccountingbalanceclient.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      515 2023-02-02 01:56:29.000000 django-oasis4-1.1.0/oasis/migrations/0005_delete_vaccountingbalanceclient_and_more.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1582 2023-02-05 00:32:58.000000 django-oasis4-1.1.0/oasis/migrations/0006_periods.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      949 2023-02-07 02:05:07.000000 django-oasis4-1.1.0/oasis/migrations/0007_cycle.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     9373 2023-02-23 14:51:01.000000 django-oasis4-1.1.0/oasis/migrations/0008_location_coffeewarehouse_and_more.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     3584 2023-03-01 16:44:41.000000 django-oasis4-1.1.0/oasis/migrations/0009_associatebalance.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    47342 2023-03-03 23:16:58.000000 django-oasis4-1.1.0/oasis/migrations/0010_operation.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     3905 2023-03-04 03:34:51.000000 django-oasis4-1.1.0/oasis/migrations/0011_offer_statemachine_and_more.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      442 2023-03-04 03:50:49.000000 django-oasis4-1.1.0/oasis/migrations/0012_offer_price.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1782 2023-03-06 20:01:57.000000 django-oasis4-1.1.0/oasis/migrations/0013_statemachine_is_final_statemachine_is_initial_and_more.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      832 2023-03-07 08:33:48.000000 django-oasis4-1.1.0/oasis/migrations/0014_remove_statemachine_unq_coffeeoffer_statemachine_and_more.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      465 2023-03-07 08:43:20.000000 django-oasis4-1.1.0/oasis/migrations/0015_statemachine_update_oasis.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      624 2023-03-16 14:42:57.000000 django-oasis4-1.1.0/oasis/migrations/0016_statemachine_is_changed_statemachine_timeout.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      571 2023-03-16 14:42:57.000000 django-oasis4-1.1.0/oasis/migrations/0017_statemachine_state_at_timeout.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1553 2023-03-16 21:48:47.000000 django-oasis4-1.1.0/oasis/migrations/0018_offermov.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)        0 2022-12-10 21:43:40.000000 django-oasis4-1.1.0/oasis/migrations/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-18 14:58:10.915141 django-oasis4-1.1.0/oasis/models/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1604 2023-03-16 21:48:47.000000 django-oasis4-1.1.0/oasis/models/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     8516 2023-03-16 21:48:47.000000 django-oasis4-1.1.0/oasis/models/local_models.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)   117483 2023-03-04 02:04:38.000000 django-oasis4-1.1.0/oasis/models/oasis_models.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-03-18 14:58:10.917141 django-oasis4-1.1.0/oasis/tasks/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      812 2023-02-23 14:54:47.000000 django-oasis4-1.1.0/oasis/tasks/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1206 2023-02-23 14:46:31.000000 django-oasis4-1.1.0/oasis/tasks/sync_coffee_ware_house.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1474 2023-01-26 02:47:20.000000 django-oasis4-1.1.0/oasis/tasks/sync_company.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1018 2023-01-18 02:09:04.000000 django-oasis4-1.1.0/oasis/tasks/sync_document_types.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1856 2023-03-01 20:00:10.000000 django-oasis4-1.1.0/oasis/tasks/sync_products.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      858 2023-03-18 14:48:42.000000 django-oasis4-1.1.0/pyproject.toml
--rw-r--r--   0 macercha  (1000) macercha  (1000)       38 2023-03-18 14:58:10.917141 django-oasis4-1.1.0/setup.cfg
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-19 22:12:01.311973 django-oasis4-1.1.1a0/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    11375 2023-01-23 20:26:24.000000 django-oasis4-1.1.1a0/LICENSE
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      144 2023-03-02 20:32:01.000000 django-oasis4-1.1.1a0/MANIFEST.in
+-rw-r--r--   0 macercha  (1000) macercha  (1000)    13080 2023-05-19 22:12:01.311973 django-oasis4-1.1.1a0/PKG-INFO
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      217 2023-02-13 15:48:51.000000 django-oasis4-1.1.1a0/README.md
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-19 22:12:01.290974 django-oasis4-1.1.1a0/django_oasis4.egg-info/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)    13080 2023-05-19 22:12:01.000000 django-oasis4-1.1.1a0/django_oasis4.egg-info/PKG-INFO
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     4321 2023-05-19 22:12:01.000000 django-oasis4-1.1.1a0/django_oasis4.egg-info/SOURCES.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)        1 2023-05-19 22:12:01.000000 django-oasis4-1.1.1a0/django_oasis4.egg-info/dependency_links.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)       78 2023-05-19 22:12:01.000000 django-oasis4-1.1.1a0/django_oasis4.egg-info/requires.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)        6 2023-05-19 22:12:01.000000 django-oasis4-1.1.1a0/django_oasis4.egg-info/top_level.txt
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-19 22:12:01.290974 django-oasis4-1.1.1a0/oasis/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2022-12-10 23:55:40.000000 django-oasis4-1.1.1a0/oasis/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1394 2023-03-18 18:38:34.000000 django-oasis4-1.1.1a0/oasis/apps.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-19 22:12:01.291974 django-oasis4-1.1.1a0/oasis/coffee_offers/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-22 14:19:30.000000 django-oasis4-1.1.1a0/oasis/coffee_offers/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      686 2023-03-06 19:37:38.000000 django-oasis4-1.1.1a0/oasis/coffee_offers/admin.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1253 2023-03-07 16:31:05.000000 django-oasis4-1.1.1a0/oasis/coffee_offers/admin_views.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-19 22:12:01.291974 django-oasis4-1.1.1a0/oasis/coffee_offers/api/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-02-23 15:03:46.000000 django-oasis4-1.1.1a0/oasis/coffee_offers/api/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-19 22:12:01.292974 django-oasis4-1.1.1a0/oasis/coffee_offers/api/serializers/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      683 2023-03-06 19:10:13.000000 django-oasis4-1.1.1a0/oasis/coffee_offers/api/serializers/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      772 2023-02-23 15:21:03.000000 django-oasis4-1.1.1a0/oasis/coffee_offers/api/serializers/coffee_ware_house.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1199 2023-03-06 20:11:27.000000 django-oasis4-1.1.1a0/oasis/coffee_offers/api/serializers/offer.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-19 22:12:01.292974 django-oasis4-1.1.1a0/oasis/coffee_offers/api/services/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      580 2023-03-01 20:03:07.000000 django-oasis4-1.1.1a0/oasis/coffee_offers/api/services/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    11193 2023-04-03 19:11:07.000000 django-oasis4-1.1.1a0/oasis/coffee_offers/api/services/coffee_offers.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     4101 2023-03-16 21:48:47.000000 django-oasis4-1.1.1a0/oasis/coffee_offers/apps.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-19 22:12:01.293974 django-oasis4-1.1.1a0/oasis/coffee_offers/lib/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-02-26 20:27:18.000000 django-oasis4-1.1.1a0/oasis/coffee_offers/lib/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-19 22:12:01.293974 django-oasis4-1.1.1a0/oasis/coffee_offers/lib/choices/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      656 2023-02-26 20:35:07.000000 django-oasis4-1.1.1a0/oasis/coffee_offers/lib/choices/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1137 2023-03-07 09:29:38.000000 django-oasis4-1.1.1a0/oasis/coffee_offers/lib/choices/coffee_offers_states.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      739 2023-02-26 20:34:29.000000 django-oasis4-1.1.1a0/oasis/coffee_offers/lib/choices/oasis_states.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-19 22:12:01.294974 django-oasis4-1.1.1a0/oasis/coffee_offers/lib/events/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      417 2023-03-16 21:48:47.000000 django-oasis4-1.1.1a0/oasis/coffee_offers/lib/events/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      939 2023-03-16 21:48:47.000000 django-oasis4-1.1.1a0/oasis/coffee_offers/lib/events/on_post_save_offer.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-19 22:12:01.294974 django-oasis4-1.1.1a0/oasis/coffee_offers/lib/utils/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      595 2023-03-06 21:38:01.000000 django-oasis4-1.1.1a0/oasis/coffee_offers/lib/utils/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     3414 2023-03-16 14:42:57.000000 django-oasis4-1.1.1a0/oasis/coffee_offers/lib/utils/offer_state_machine.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-19 22:12:01.294974 django-oasis4-1.1.1a0/oasis/coffee_offers/lib/validators/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      757 2023-02-26 21:14:28.000000 django-oasis4-1.1.1a0/oasis/coffee_offers/lib/validators/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1336 2023-02-26 21:13:57.000000 django-oasis4-1.1.1a0/oasis/coffee_offers/lib/validators/date_validators.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      823 2023-02-26 20:45:48.000000 django-oasis4-1.1.1a0/oasis/coffee_offers/lib/validators/oasis_statuses.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-19 22:12:01.285974 django-oasis4-1.1.1a0/oasis/coffee_offers/locale/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-19 22:12:01.286974 django-oasis4-1.1.1a0/oasis/coffee_offers/locale/es/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-19 22:12:01.295974 django-oasis4-1.1.1a0/oasis/coffee_offers/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     4521 2023-03-16 14:42:57.000000 django-oasis4-1.1.1a0/oasis/coffee_offers/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     6279 2023-03-16 14:42:57.000000 django-oasis4-1.1.1a0/oasis/coffee_offers/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-19 22:12:01.295974 django-oasis4-1.1.1a0/oasis/coffee_offers/tasks/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      595 2023-03-06 23:14:13.000000 django-oasis4-1.1.1a0/oasis/coffee_offers/tasks/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1365 2023-03-16 14:42:57.000000 django-oasis4-1.1.1a0/oasis/coffee_offers/tasks/sync_coffe_offers.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-19 22:12:01.296974 django-oasis4-1.1.1a0/oasis/coffee_offers/templates/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1072 2023-03-08 13:40:32.000000 django-oasis4-1.1.1a0/oasis/coffee_offers/templates/change_status.html
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      803 2023-03-08 13:40:32.000000 django-oasis4-1.1.1a0/oasis/coffee_offers/templates/change_status.txt
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-19 22:12:01.296974 django-oasis4-1.1.1a0/oasis/coffee_offers/templates/coffee_offers/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      123 2023-03-07 09:07:24.000000 django-oasis4-1.1.1a0/oasis/coffee_offers/templates/coffee_offers/contract_template.html
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      123 2023-03-07 09:07:24.000000 django-oasis4-1.1.1a0/oasis/coffee_offers/templates/coffee_offers/promisory_note.html
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      123 2023-03-07 09:07:24.000000 django-oasis4-1.1.1a0/oasis/coffee_offers/templates/coffee_offers/terms_conditions.html
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1054 2023-03-02 20:24:29.000000 django-oasis4-1.1.1a0/oasis/coffee_offers/templates/save_offer.html
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      785 2023-03-02 20:03:04.000000 django-oasis4-1.1.1a0/oasis/coffee_offers/templates/save_offer.txt
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      981 2023-03-16 14:42:57.000000 django-oasis4-1.1.1a0/oasis/coffee_offers/urls.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-19 22:12:01.296974 django-oasis4-1.1.1a0/oasis/lib/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2022-11-16 14:55:35.000000 django-oasis4-1.1.1a0/oasis/lib/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-19 22:12:01.297974 django-oasis4-1.1.1a0/oasis/lib/choices/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      582 2023-01-17 21:45:20.000000 django-oasis4-1.1.1a0/oasis/lib/choices/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      783 2023-03-18 17:17:41.000000 django-oasis4-1.1.1a0/oasis/lib/choices/customer_type.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-19 22:12:01.300974 django-oasis4-1.1.1a0/oasis/lib/managers/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1525 2023-03-16 14:42:57.000000 django-oasis4-1.1.1a0/oasis/lib/managers/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      780 2023-02-23 14:39:16.000000 django-oasis4-1.1.1a0/oasis/lib/managers/local_coffee_ware_house.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      682 2023-01-28 14:38:17.000000 django-oasis4-1.1.1a0/oasis/lib/managers/local_company.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1355 2023-01-18 02:07:35.000000 django-oasis4-1.1.1a0/oasis/lib/managers/local_document_type.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1578 2023-03-08 14:17:45.000000 django-oasis4-1.1.1a0/oasis/lib/managers/local_offer.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1212 2022-12-14 20:34:45.000000 django-oasis4-1.1.1a0/oasis/lib/managers/local_product.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     2159 2023-03-16 14:42:57.000000 django-oasis4-1.1.1a0/oasis/lib/managers/local_state_machine.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1201 2023-03-02 21:35:32.000000 django-oasis4-1.1.1a0/oasis/lib/managers/oasis_associate_balance.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     2701 2023-03-01 16:42:42.000000 django-oasis4-1.1.1a0/oasis/lib/managers/oasis_client.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1050 2023-01-27 03:47:52.000000 django-oasis4-1.1.1a0/oasis/lib/managers/oasis_company.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1390 2023-02-07 10:48:09.000000 django-oasis4-1.1.1a0/oasis/lib/managers/oasis_cycle.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     4007 2023-01-24 23:42:01.000000 django-oasis4-1.1.1a0/oasis/lib/managers/oasis_discount.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1180 2023-01-24 23:42:01.000000 django-oasis4-1.1.1a0/oasis/lib/managers/oasis_geographic_location.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      799 2023-02-23 14:57:09.000000 django-oasis4-1.1.1a0/oasis/lib/managers/oasis_location.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     7130 2023-03-08 14:56:20.000000 django-oasis4-1.1.1a0/oasis/lib/managers/oasis_operation.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      939 2023-02-06 19:28:19.000000 django-oasis4-1.1.1a0/oasis/lib/managers/oasis_periods.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      906 2022-12-19 16:49:04.000000 django-oasis4-1.1.1a0/oasis/lib/managers/oasis_product.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      730 2023-01-25 00:42:41.000000 django-oasis4-1.1.1a0/oasis/lib/managers/oasis_type_client.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-19 22:12:01.301974 django-oasis4-1.1.1a0/oasis/lib/serializers/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      658 2023-02-07 09:06:27.000000 django-oasis4-1.1.1a0/oasis/lib/serializers/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      789 2023-02-07 09:25:36.000000 django-oasis4-1.1.1a0/oasis/lib/serializers/oasis_cycle.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      803 2022-12-14 20:01:00.000000 django-oasis4-1.1.1a0/oasis/lib/serializers/product.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-19 22:12:01.302974 django-oasis4-1.1.1a0/oasis/lib/utils/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      579 2023-03-03 19:38:17.000000 django-oasis4-1.1.1a0/oasis/lib/utils/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     3274 2023-04-03 19:11:07.000000 django-oasis4-1.1.1a0/oasis/lib/utils/oasis_actions.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-19 22:12:01.287974 django-oasis4-1.1.1a0/oasis/locale/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-19 22:12:01.287974 django-oasis4-1.1.1a0/oasis/locale/es/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-19 22:12:01.302974 django-oasis4-1.1.1a0/oasis/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1744 2023-02-08 01:14:00.000000 django-oasis4-1.1.1a0/oasis/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     2663 2023-02-08 01:13:42.000000 django-oasis4-1.1.1a0/oasis/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-19 22:12:01.306974 django-oasis4-1.1.1a0/oasis/migrations/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    29691 2022-12-13 18:21:01.000000 django-oasis4-1.1.1a0/oasis/migrations/0001_initial.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    31003 2023-01-17 22:22:35.000000 django-oasis4-1.1.1a0/oasis/migrations/0002_geographiclocation_typeclient_documenttype_client_and_more.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    17130 2023-01-26 02:36:44.000000 django-oasis4-1.1.1a0/oasis/migrations/0003_oasiscompany_company.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     5814 2023-01-27 03:47:55.000000 django-oasis4-1.1.1a0/oasis/migrations/0004_account_vaccountingbalanceclient.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      515 2023-02-02 01:56:29.000000 django-oasis4-1.1.1a0/oasis/migrations/0005_delete_vaccountingbalanceclient_and_more.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1582 2023-02-05 00:32:58.000000 django-oasis4-1.1.1a0/oasis/migrations/0006_periods.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      949 2023-02-07 02:05:07.000000 django-oasis4-1.1.1a0/oasis/migrations/0007_cycle.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     9373 2023-02-23 14:51:01.000000 django-oasis4-1.1.1a0/oasis/migrations/0008_location_coffeewarehouse_and_more.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     3584 2023-03-01 16:44:41.000000 django-oasis4-1.1.1a0/oasis/migrations/0009_associatebalance.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    47342 2023-03-03 23:16:58.000000 django-oasis4-1.1.1a0/oasis/migrations/0010_operation.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     3905 2023-03-04 03:34:51.000000 django-oasis4-1.1.1a0/oasis/migrations/0011_offer_statemachine_and_more.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      442 2023-03-04 03:50:49.000000 django-oasis4-1.1.1a0/oasis/migrations/0012_offer_price.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1782 2023-03-06 20:01:57.000000 django-oasis4-1.1.1a0/oasis/migrations/0013_statemachine_is_final_statemachine_is_initial_and_more.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      832 2023-03-07 08:33:48.000000 django-oasis4-1.1.1a0/oasis/migrations/0014_remove_statemachine_unq_coffeeoffer_statemachine_and_more.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      465 2023-03-07 08:43:20.000000 django-oasis4-1.1.1a0/oasis/migrations/0015_statemachine_update_oasis.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      624 2023-03-16 14:42:57.000000 django-oasis4-1.1.1a0/oasis/migrations/0016_statemachine_is_changed_statemachine_timeout.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      571 2023-03-16 14:42:57.000000 django-oasis4-1.1.1a0/oasis/migrations/0017_statemachine_state_at_timeout.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1553 2023-03-16 21:48:47.000000 django-oasis4-1.1.1a0/oasis/migrations/0018_offermov.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1009 2023-05-19 21:49:17.000000 django-oasis4-1.1.1a0/oasis/migrations/0019_stat.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)        0 2022-12-10 21:43:40.000000 django-oasis4-1.1.1a0/oasis/migrations/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-19 22:12:01.307973 django-oasis4-1.1.1a0/oasis/models/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1647 2023-05-19 21:49:17.000000 django-oasis4-1.1.1a0/oasis/models/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     9352 2023-05-19 21:49:17.000000 django-oasis4-1.1.1a0/oasis/models/local_models.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)   117483 2023-03-04 02:04:38.000000 django-oasis4-1.1.1a0/oasis/models/oasis_models.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-19 22:12:01.308974 django-oasis4-1.1.1a0/oasis/stats/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      293 2023-05-19 21:49:17.000000 django-oasis4-1.1.1a0/oasis/stats/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      419 2023-05-19 21:49:17.000000 django-oasis4-1.1.1a0/oasis/stats/admin.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-19 22:12:01.308974 django-oasis4-1.1.1a0/oasis/stats/api/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      293 2023-05-19 21:49:17.000000 django-oasis4-1.1.1a0/oasis/stats/api/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-19 22:12:01.309974 django-oasis4-1.1.1a0/oasis/stats/api/serializers/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      329 2023-05-19 21:49:17.000000 django-oasis4-1.1.1a0/oasis/stats/api/serializers/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-05-19 21:49:17.000000 django-oasis4-1.1.1a0/oasis/stats/api/serializers/stats.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-19 22:12:01.309974 django-oasis4-1.1.1a0/oasis/stats/api/services/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      327 2023-05-19 21:49:17.000000 django-oasis4-1.1.1a0/oasis/stats/api/services/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1947 2023-05-19 21:49:17.000000 django-oasis4-1.1.1a0/oasis/stats/api/services/stats.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      455 2023-05-19 21:49:17.000000 django-oasis4-1.1.1a0/oasis/stats/apps.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      518 2023-05-19 21:49:17.000000 django-oasis4-1.1.1a0/oasis/stats/urls.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-19 22:12:01.310974 django-oasis4-1.1.1a0/oasis/tasks/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      812 2023-02-23 14:54:47.000000 django-oasis4-1.1.1a0/oasis/tasks/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1206 2023-02-23 14:46:31.000000 django-oasis4-1.1.1a0/oasis/tasks/sync_coffee_ware_house.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1474 2023-01-26 02:47:20.000000 django-oasis4-1.1.1a0/oasis/tasks/sync_company.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1018 2023-01-18 02:09:04.000000 django-oasis4-1.1.1a0/oasis/tasks/sync_document_types.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1856 2023-03-01 20:00:10.000000 django-oasis4-1.1.1a0/oasis/tasks/sync_products.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      866 2023-05-19 22:03:09.000000 django-oasis4-1.1.1a0/pyproject.toml
+-rw-r--r--   0 macercha  (1000) macercha  (1000)       38 2023-05-19 22:12:01.311973 django-oasis4-1.1.1a0/setup.cfg
```

### Comparing `django-oasis4-1.1.0/LICENSE` & `django-oasis4-1.1.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/PKG-INFO` & `django-oasis4-1.1.1a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-oasis4
-Version: 1.1.0
+Version: 1.1.1a0
 Summary: OASIS4 Data Interfaces
 Author-email: Mario Cerón <mario.ceron@cqinversiones.co>
 License:                                     CQ INVERSIONES S.A.S.
                                       CONTRATO DE LICENCIA DE SOFTWARE
                                                     NO OEM
                                              (Version 2.0 - 2023)
```

### Comparing `django-oasis4-1.1.0/django_oasis4.egg-info/PKG-INFO` & `django-oasis4-1.1.1a0/django_oasis4.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-oasis4
-Version: 1.1.0
+Version: 1.1.1a0
 Summary: OASIS4 Data Interfaces
 Author-email: Mario Cerón <mario.ceron@cqinversiones.co>
 License:                                     CQ INVERSIONES S.A.S.
                                       CONTRATO DE LICENCIA DE SOFTWARE
                                                     NO OEM
                                              (Version 2.0 - 2023)
```

### Comparing `django-oasis4-1.1.0/django_oasis4.egg-info/SOURCES.txt` & `django-oasis4-1.1.1a0/django_oasis4.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -84,16 +84,26 @@
 oasis/migrations/0012_offer_price.py
 oasis/migrations/0013_statemachine_is_final_statemachine_is_initial_and_more.py
 oasis/migrations/0014_remove_statemachine_unq_coffeeoffer_statemachine_and_more.py
 oasis/migrations/0015_statemachine_update_oasis.py
 oasis/migrations/0016_statemachine_is_changed_statemachine_timeout.py
 oasis/migrations/0017_statemachine_state_at_timeout.py
 oasis/migrations/0018_offermov.py
+oasis/migrations/0019_stat.py
 oasis/migrations/__init__.py
 oasis/models/__init__.py
 oasis/models/local_models.py
 oasis/models/oasis_models.py
+oasis/stats/__init__.py
+oasis/stats/admin.py
+oasis/stats/apps.py
+oasis/stats/urls.py
+oasis/stats/api/__init__.py
+oasis/stats/api/serializers/__init__.py
+oasis/stats/api/serializers/stats.py
+oasis/stats/api/services/__init__.py
+oasis/stats/api/services/stats.py
 oasis/tasks/__init__.py
 oasis/tasks/sync_coffee_ware_house.py
 oasis/tasks/sync_company.py
 oasis/tasks/sync_document_types.py
 oasis/tasks/sync_products.py
```

### Comparing `django-oasis4-1.1.0/oasis/apps.py` & `django-oasis4-1.1.1a0/oasis/apps.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/coffee_offers/admin.py` & `django-oasis4-1.1.1a0/oasis/coffee_offers/admin.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/coffee_offers/admin_views.py` & `django-oasis4-1.1.1a0/oasis/coffee_offers/admin_views.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/coffee_offers/api/serializers/__init__.py` & `django-oasis4-1.1.1a0/oasis/coffee_offers/api/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/coffee_offers/api/serializers/coffee_ware_house.py` & `django-oasis4-1.1.1a0/oasis/coffee_offers/api/serializers/coffee_ware_house.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/coffee_offers/api/serializers/offer.py` & `django-oasis4-1.1.1a0/oasis/coffee_offers/api/serializers/offer.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/coffee_offers/api/services/__init__.py` & `django-oasis4-1.1.1a0/oasis/coffee_offers/api/services/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/coffee_offers/api/services/coffee_offers.py` & `django-oasis4-1.1.1a0/oasis/coffee_offers/api/services/coffee_offers.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/coffee_offers/apps.py` & `django-oasis4-1.1.1a0/oasis/coffee_offers/apps.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/coffee_offers/lib/choices/__init__.py` & `django-oasis4-1.1.1a0/oasis/coffee_offers/lib/choices/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/coffee_offers/lib/choices/coffee_offers_states.py` & `django-oasis4-1.1.1a0/oasis/coffee_offers/lib/choices/coffee_offers_states.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/coffee_offers/lib/choices/oasis_states.py` & `django-oasis4-1.1.1a0/oasis/coffee_offers/lib/choices/oasis_states.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/coffee_offers/lib/events/on_post_save_offer.py` & `django-oasis4-1.1.1a0/oasis/coffee_offers/lib/events/on_post_save_offer.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/coffee_offers/lib/utils/__init__.py` & `django-oasis4-1.1.1a0/oasis/coffee_offers/lib/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/coffee_offers/lib/utils/offer_state_machine.py` & `django-oasis4-1.1.1a0/oasis/coffee_offers/lib/utils/offer_state_machine.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/coffee_offers/lib/validators/__init__.py` & `django-oasis4-1.1.1a0/oasis/coffee_offers/lib/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/coffee_offers/lib/validators/date_validators.py` & `django-oasis4-1.1.1a0/oasis/coffee_offers/lib/validators/date_validators.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/coffee_offers/lib/validators/oasis_statuses.py` & `django-oasis4-1.1.1a0/oasis/coffee_offers/lib/validators/oasis_statuses.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/coffee_offers/locale/es/LC_MESSAGES/django.mo` & `django-oasis4-1.1.1a0/oasis/coffee_offers/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/coffee_offers/locale/es/LC_MESSAGES/django.po` & `django-oasis4-1.1.1a0/oasis/coffee_offers/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/coffee_offers/tasks/__init__.py` & `django-oasis4-1.1.1a0/oasis/coffee_offers/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/coffee_offers/tasks/sync_coffe_offers.py` & `django-oasis4-1.1.1a0/oasis/coffee_offers/tasks/sync_coffe_offers.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/coffee_offers/templates/change_status.html` & `django-oasis4-1.1.1a0/oasis/coffee_offers/templates/change_status.html`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/coffee_offers/templates/change_status.txt` & `django-oasis4-1.1.1a0/oasis/coffee_offers/templates/change_status.txt`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/coffee_offers/templates/save_offer.html` & `django-oasis4-1.1.1a0/oasis/coffee_offers/templates/save_offer.html`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/coffee_offers/templates/save_offer.txt` & `django-oasis4-1.1.1a0/oasis/coffee_offers/templates/save_offer.txt`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/coffee_offers/urls.py` & `django-oasis4-1.1.1a0/oasis/coffee_offers/urls.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/lib/choices/__init__.py` & `django-oasis4-1.1.1a0/oasis/lib/choices/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/lib/choices/customer_type.py` & `django-oasis4-1.1.1a0/oasis/lib/choices/customer_type.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/lib/managers/__init__.py` & `django-oasis4-1.1.1a0/oasis/lib/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/lib/managers/local_coffee_ware_house.py` & `django-oasis4-1.1.1a0/oasis/lib/managers/local_coffee_ware_house.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/lib/managers/local_company.py` & `django-oasis4-1.1.1a0/oasis/lib/managers/local_company.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/lib/managers/local_document_type.py` & `django-oasis4-1.1.1a0/oasis/lib/managers/local_document_type.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/lib/managers/local_offer.py` & `django-oasis4-1.1.1a0/oasis/lib/managers/local_offer.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/lib/managers/local_product.py` & `django-oasis4-1.1.1a0/oasis/lib/managers/local_product.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/lib/managers/local_state_machine.py` & `django-oasis4-1.1.1a0/oasis/lib/managers/local_state_machine.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/lib/managers/oasis_associate_balance.py` & `django-oasis4-1.1.1a0/oasis/lib/managers/oasis_associate_balance.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/lib/managers/oasis_client.py` & `django-oasis4-1.1.1a0/oasis/lib/managers/oasis_client.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/lib/managers/oasis_company.py` & `django-oasis4-1.1.1a0/oasis/lib/managers/oasis_company.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/lib/managers/oasis_cycle.py` & `django-oasis4-1.1.1a0/oasis/lib/managers/oasis_cycle.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/lib/managers/oasis_discount.py` & `django-oasis4-1.1.1a0/oasis/lib/managers/oasis_discount.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/lib/managers/oasis_geographic_location.py` & `django-oasis4-1.1.1a0/oasis/lib/managers/oasis_geographic_location.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/lib/managers/oasis_location.py` & `django-oasis4-1.1.1a0/oasis/lib/managers/oasis_location.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/lib/managers/oasis_operation.py` & `django-oasis4-1.1.1a0/oasis/lib/managers/oasis_operation.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/lib/managers/oasis_periods.py` & `django-oasis4-1.1.1a0/oasis/lib/managers/oasis_periods.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/lib/managers/oasis_product.py` & `django-oasis4-1.1.1a0/oasis/lib/managers/oasis_product.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/lib/managers/oasis_type_client.py` & `django-oasis4-1.1.1a0/oasis/lib/managers/oasis_type_client.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/lib/serializers/__init__.py` & `django-oasis4-1.1.1a0/oasis/lib/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/lib/serializers/oasis_cycle.py` & `django-oasis4-1.1.1a0/oasis/lib/serializers/oasis_cycle.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/lib/serializers/product.py` & `django-oasis4-1.1.1a0/oasis/lib/serializers/product.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/lib/utils/__init__.py` & `django-oasis4-1.1.1a0/oasis/lib/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/lib/utils/oasis_actions.py` & `django-oasis4-1.1.1a0/oasis/lib/utils/oasis_actions.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/locale/es/LC_MESSAGES/django.mo` & `django-oasis4-1.1.1a0/oasis/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/locale/es/LC_MESSAGES/django.po` & `django-oasis4-1.1.1a0/oasis/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/migrations/0001_initial.py` & `django-oasis4-1.1.1a0/oasis/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/migrations/0002_geographiclocation_typeclient_documenttype_client_and_more.py` & `django-oasis4-1.1.1a0/oasis/migrations/0002_geographiclocation_typeclient_documenttype_client_and_more.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/migrations/0003_oasiscompany_company.py` & `django-oasis4-1.1.1a0/oasis/migrations/0003_oasiscompany_company.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/migrations/0004_account_vaccountingbalanceclient.py` & `django-oasis4-1.1.1a0/oasis/migrations/0004_account_vaccountingbalanceclient.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/migrations/0005_delete_vaccountingbalanceclient_and_more.py` & `django-oasis4-1.1.1a0/oasis/migrations/0005_delete_vaccountingbalanceclient_and_more.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/migrations/0006_periods.py` & `django-oasis4-1.1.1a0/oasis/migrations/0006_periods.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/migrations/0007_cycle.py` & `django-oasis4-1.1.1a0/oasis/migrations/0007_cycle.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/migrations/0008_location_coffeewarehouse_and_more.py` & `django-oasis4-1.1.1a0/oasis/migrations/0008_location_coffeewarehouse_and_more.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/migrations/0009_associatebalance.py` & `django-oasis4-1.1.1a0/oasis/migrations/0009_associatebalance.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/migrations/0010_operation.py` & `django-oasis4-1.1.1a0/oasis/migrations/0010_operation.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/migrations/0011_offer_statemachine_and_more.py` & `django-oasis4-1.1.1a0/oasis/migrations/0011_offer_statemachine_and_more.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/migrations/0013_statemachine_is_final_statemachine_is_initial_and_more.py` & `django-oasis4-1.1.1a0/oasis/migrations/0013_statemachine_is_final_statemachine_is_initial_and_more.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/migrations/0014_remove_statemachine_unq_coffeeoffer_statemachine_and_more.py` & `django-oasis4-1.1.1a0/oasis/migrations/0014_remove_statemachine_unq_coffeeoffer_statemachine_and_more.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/migrations/0016_statemachine_is_changed_statemachine_timeout.py` & `django-oasis4-1.1.1a0/oasis/migrations/0016_statemachine_is_changed_statemachine_timeout.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/migrations/0017_statemachine_state_at_timeout.py` & `django-oasis4-1.1.1a0/oasis/migrations/0017_statemachine_state_at_timeout.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/migrations/0018_offermov.py` & `django-oasis4-1.1.1a0/oasis/migrations/0018_offermov.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/models/__init__.py` & `django-oasis4-1.1.1a0/oasis/models/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from .local_models import CoffeeWareHouse
 from .local_models import Company
 from .local_models import DocumentType
 from .local_models import Offer
 from .local_models import OfferMov
 from .local_models import Product
 from .local_models import StateMachine
+from .local_models import Stat
 from .oasis_models import Account
 from .oasis_models import AssociateBalance
 from .oasis_models import Classification
 from .oasis_models import Client
 from .oasis_models import Cycle
 from .oasis_models import Discount
 from .oasis_models import GeographicLocation
@@ -47,10 +48,11 @@
     "OasisCompany",
     "OasisProduct",
     "Offer",
     "OfferMov",
     "Operation",
     "Periods",
     "StateMachine",
-    "TypeClient"
+    "TypeClient",
+    "Stat"
 ]
```

### Comparing `django-oasis4-1.1.0/oasis/models/local_models.py` & `django-oasis4-1.1.1a0/oasis/models/local_models.py`

 * *Files 3% similar despite different names*

```diff
@@ -151,17 +151,36 @@
         return self.status in [CoffeeOffersStates.NEW, CoffeeOffersStates.SIGNED, CoffeeOffersStates.PARTIAL]
 
     class Meta:
         constraints = [
             models.UniqueConstraint(fields=("contract",), name="UNQ_Offer_Contract")
         ]
 
+
 class OfferMov(models.DatedModel):
-    offer = models.ForeignKey(Offer, on_delete=models.PROTECT, related_name="offer_movements", related_query_name="offer")
+    offer = models.ForeignKey(Offer, on_delete=models.PROTECT, related_name="offer_movements",
+                              related_query_name="offer")
     status = models.IntegerField(choices=CoffeeOffersStates.choices, null=False, blank=False)
     delivery_date = models.DateField(blank=True, null=True)
     price = models.DecimalField(max_digits=7, decimal_places=2, blank=True, null=True)
     kg_offered = models.DecimalField(max_digits=9, decimal_places=2, blank=True, null=True)
     kg_received = models.DecimalField(max_digits=9, decimal_places=2, blank=True, null=True)
     created = models.BooleanField(default=False, blank=False, null=False)
 
 
+class Stat(models.Model):
+    """
+    Model class to represent stats entity of the app Stats
+    """
+    name = models.CharField(null=False, blank=False, max_length=120, verbose_name=_("Stat name"))
+    query_text = models.TextField(null=False, blank=False, verbose_name=_("Query Text"),
+                                  help_text=_("Text used to execute the query"))
+    is_staff = models.BooleanField(default=True, null=False, blank=False, verbose_name=_("Is staff"),
+                                   help_text=_("It is required to be staff to see the stat"))
+    enabled = models.BooleanField(default=True, null=False, blank=False, verbose_name=_("Enabled"))
+
+    def __str__(self):
+        return self.name
+
+    class Meta:
+        verbose_name = _("Stat")
+        verbose_name_plural = _("Stats")
```

### Comparing `django-oasis4-1.1.0/oasis/models/oasis_models.py` & `django-oasis4-1.1.1a0/oasis/models/oasis_models.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/tasks/__init__.py` & `django-oasis4-1.1.1a0/oasis/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/tasks/sync_coffee_ware_house.py` & `django-oasis4-1.1.1a0/oasis/tasks/sync_coffee_ware_house.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/tasks/sync_company.py` & `django-oasis4-1.1.1a0/oasis/tasks/sync_company.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/tasks/sync_document_types.py` & `django-oasis4-1.1.1a0/oasis/tasks/sync_document_types.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/oasis/tasks/sync_products.py` & `django-oasis4-1.1.1a0/oasis/tasks/sync_products.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.0/pyproject.toml` & `django-oasis4-1.1.1a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel",
 ]
 build-backend="setuptools.build_meta"
 
 [project]
 name = "django-oasis4"
-version = "1.1.0"
+version = "1.1.1-alpha.0"
 authors = [
     {name="Mario Cerón", email="mario.ceron@cqinversiones.co"}
 ]
 description = "OASIS4 Data Interfaces"
 readme = "README.md"
 license = {file="LICENSE"}
 requires-python = ">=3.9"
```

