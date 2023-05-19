# Comparing `tmp/sphinxcontrib_confluencebuilder-2.1.0.tar.gz` & `tmp/sphinxcontrib_confluencebuilder-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxcontrib_confluencebuilder-2.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sphinxcontrib_confluencebuilder-2.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sphinxcontrib_confluencebuilder-2.1.0.tar` & `sphinxcontrib_confluencebuilder-2.1.1.tar`

### file list

```diff
@@ -1,146 +1,149 @@
--rw-r--r--   0        0        0     4076 2023-05-16 00:58:11.667937 sphinxcontrib_confluencebuilder-2.1.0/README.rst
--rw-r--r--   0        0        0     1774 2023-05-07 18:59:45.812201 sphinxcontrib_confluencebuilder-2.1.0/pyproject.toml
--rw-r--r--   0        0        0    18061 2023-05-16 01:13:54.764696 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/__init__.py
--rw-r--r--   0        0        0     3630 2023-04-07 19:29:44.220864 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/__main__.py
--rw-r--r--   0        0        0    14586 2023-04-15 14:46:27.000054 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/assets.py
--rw-r--r--   0        0        0    48600 2023-05-13 15:11:25.713682 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/builder.py
--rw-r--r--   0        0        0        0 2023-01-22 17:27:22.404126 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/cmd/__init__.py
--rw-r--r--   0        0        0     2442 2023-04-07 19:29:44.222817 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/cmd/build.py
--rw-r--r--   0        0        0    11521 2023-04-07 19:29:44.222817 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/cmd/report.py
--rw-r--r--   0        0        0     6780 2023-04-08 16:47:36.734308 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/cmd/wipe.py
--rw-r--r--   0        0        0     3476 2023-04-07 19:29:44.224766 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/compat.py
--rw-r--r--   0        0        0     2929 2023-04-08 16:47:36.735307 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/config/__init__.py
--rw-r--r--   0        0        0    28152 2023-04-17 01:06:14.719799 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/config/checks.py
--rw-r--r--   0        0        0     4150 2023-04-16 01:30:57.889226 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/config/defaults.py
--rw-r--r--   0        0        0     1431 2023-04-07 19:29:44.227698 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/config/env.py
--rw-r--r--   0        0        0     3529 2023-04-07 19:29:44.227698 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/config/manager.py
--rw-r--r--   0        0        0     3402 2023-04-08 16:47:36.736308 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/config/notifications.py
--rw-r--r--   0        0        0    17687 2023-04-07 19:29:44.229651 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/config/validation.py
--rw-r--r--   0        0        0    11596 2023-05-13 21:00:30.923234 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/directives.py
--rw-r--r--   0        0        0     9196 2023-04-07 19:29:44.230626 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/exceptions.py
--rw-r--r--   0        0        0     3057 2023-04-07 19:29:44.231602 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/intersphinx.py
--rw-r--r--   0        0        0      432 2023-04-07 19:29:44.231602 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/__init__.py
--rw-r--r--   0        0        0      590 2023-01-05 22:53:18.094822 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/ar/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1387 2023-05-16 00:43:39.061378 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/ar/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      533 2023-01-05 22:53:18.096782 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/bg/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1330 2023-05-16 00:43:39.062380 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/bg/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      458 2023-01-05 22:53:18.098731 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/bn/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1284 2023-05-16 00:43:39.063378 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/bn/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      500 2023-01-05 22:53:18.099707 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/ca/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1297 2023-05-16 00:43:39.064377 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/ca/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      526 2023-01-05 22:53:18.100682 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/cs/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1323 2023-05-16 00:43:39.064377 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/cs/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      579 2023-01-05 22:53:18.101658 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/cy/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1376 2023-05-16 00:43:39.065377 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/cy/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      499 2023-01-05 22:53:18.103611 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/da/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1296 2023-05-16 00:43:39.066377 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/da/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      503 2023-01-05 22:53:18.104592 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/de/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1300 2023-05-16 00:43:39.067377 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/de/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      518 2023-01-05 22:53:18.106543 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/el/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1315 2023-05-16 00:43:39.067377 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/el/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      460 2023-01-05 22:53:18.108080 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/eo/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1300 2023-05-16 00:43:39.068378 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/eo/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      458 2023-01-05 22:53:18.109032 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/es/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1287 2023-05-16 00:43:39.068378 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/es/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      505 2023-01-05 22:53:18.110006 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/et/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1302 2023-05-16 00:43:39.069379 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/et/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      500 2023-01-05 22:53:18.111962 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/eu/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1297 2023-05-16 00:43:39.069379 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/eu/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      505 2023-01-05 22:53:18.113918 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/fi/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1302 2023-05-16 00:43:39.070376 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/fi/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      503 2023-01-05 22:53:18.114891 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/fr/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1300 2023-05-16 00:43:39.071378 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/fr/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      507 2023-01-05 22:53:18.116843 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/he/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1333 2023-05-16 00:43:39.071378 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/he/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      535 2023-01-05 22:53:18.117819 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/hi/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1332 2023-05-16 00:43:39.072377 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/hi/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      573 2023-01-05 22:53:18.118796 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/hr/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1370 2023-05-16 00:43:39.072377 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/hr/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      510 2023-01-05 22:53:18.120751 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/hu/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1307 2023-05-16 00:43:39.073376 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/hu/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      497 2023-01-05 22:53:18.122701 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/id/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1294 2023-05-16 00:43:39.074377 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/id/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      458 2023-01-05 22:53:18.124656 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/it/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1284 2023-05-16 00:43:39.074377 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/it/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      499 2023-01-05 22:53:18.125629 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/ja/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1296 2023-05-16 00:43:39.075377 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/ja/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      492 2023-01-05 22:53:18.127584 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/ko/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1289 2023-05-16 00:43:39.075377 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/ko/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      609 2023-01-05 22:53:18.128562 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/lt/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1406 2023-05-16 00:43:39.076379 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/lt/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      535 2023-01-05 22:53:18.130512 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/lv/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1332 2023-05-16 00:43:39.077376 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/lv/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      535 2023-01-05 22:53:18.133442 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/mk/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1332 2023-05-16 00:43:39.080380 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/mk/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      509 2023-01-05 22:53:18.135398 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/nb/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1306 2023-05-16 00:43:39.081380 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/nb/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      551 2023-01-05 22:53:18.137353 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/ne/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1351 2023-05-16 00:43:39.082381 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/ne/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      498 2023-01-05 22:53:18.139304 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/nl/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1295 2023-05-16 00:43:39.083377 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/nl/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      648 2023-01-05 22:53:18.141258 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/pl/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1445 2023-05-16 00:43:39.084381 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/pl/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      513 2023-01-05 22:53:18.143207 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/pt_BR/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1313 2023-05-16 00:43:39.085380 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/pt_BR/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      546 2023-01-05 22:53:18.144187 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/ro/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1343 2023-05-16 00:43:39.085380 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/ro/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      623 2023-01-05 22:53:18.146138 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/ru/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1449 2023-05-16 00:43:39.086379 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/ru/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      458 2023-01-05 22:53:18.148092 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/si/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1287 2023-05-16 00:43:39.086379 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/si/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      527 2023-01-05 22:53:18.150044 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/sk/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1324 2023-05-16 00:43:39.087380 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/sk/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      512 2023-01-05 22:53:18.151996 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/sl/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1338 2023-05-16 00:43:39.088379 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/sl/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      821 2023-05-16 00:43:39.088379 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/sphinxcontrib.confluencebuilder.pot
--rw-r--r--   0        0        0      511 2023-01-05 22:53:18.153947 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/sq/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1308 2023-05-16 00:43:39.089376 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/sq/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      540 2023-01-05 22:53:18.155966 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/sr_CS/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1369 2023-05-16 00:43:39.089376 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/sr_CS/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      502 2023-01-05 22:53:18.158443 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/sv/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1302 2023-05-16 00:43:39.090376 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/sv/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      546 2023-01-05 22:53:18.160396 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/ta/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1343 2023-05-16 00:43:39.091378 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/ta/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      538 2023-01-05 22:53:18.162349 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/te/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1335 2023-05-16 00:43:39.091378 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/te/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      505 2023-01-05 22:53:18.164303 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/tr/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1302 2023-05-16 00:43:39.092379 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/tr/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      689 2023-01-05 22:53:18.165278 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/uk/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1486 2023-05-16 00:43:39.092379 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/uk/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      496 2023-01-05 22:53:18.167232 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/vi/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1293 2023-05-16 00:43:39.093380 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/vi/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      504 2023-01-05 22:48:19.243628 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/zh_TW/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1304 2023-05-16 00:43:53.313328 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/zh_TW/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0     4581 2023-04-07 19:29:44.232579 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/logger.py
--rw-r--r--   0        0        0     6304 2023-05-13 21:00:30.923234 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/nodes.py
--rw-r--r--   0        0        0    49499 2023-05-14 05:04:32.872359 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/publisher.py
--rw-r--r--   0        0        0      430 2023-04-07 19:29:44.234534 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/reportbuilder.py
--rw-r--r--   0        0        0    14702 2023-04-07 19:29:44.235511 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/rest.py
--rw-r--r--   0        0        0     7784 2023-05-13 21:00:30.924232 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/roles.py
--rw-r--r--   0        0        0    11845 2023-04-07 19:29:44.236486 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/singlebuilder.py
--rw-r--r--   0        0        0     9455 2023-04-07 19:29:44.237465 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/state.py
--rw-r--r--   0        0        0        0 2023-01-22 17:27:22.418126 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/std/__init__.py
--rw-r--r--   0        0        0    12663 2023-04-07 19:29:44.237465 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/std/confluence.py
--rw-r--r--   0        0        0      319 2023-04-07 19:29:44.238438 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/std/sphinx.py
--rw-r--r--   0        0        0     2038 2023-04-07 19:29:44.238438 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/storage/__init__.py
--rw-r--r--   0        0        0     4747 2023-04-07 19:29:44.239414 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/storage/index.py
--rw-r--r--   0        0        0     1189 2023-04-07 19:29:44.239414 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/storage/search.py
--rw-r--r--   0        0        0        0 2023-01-22 17:27:22.420125 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/storage/templates/__init__.py
--rw-r--r--   0        0        0     1801 2023-04-07 19:29:44.240391 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/storage/templates/domainindex.html
--rw-r--r--   0        0        0     1634 2023-04-07 19:29:44.241370 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/storage/templates/domainindex_v2.html
--rw-r--r--   0        0        0     2201 2023-04-07 19:29:44.241370 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/storage/templates/genindex.html
--rw-r--r--   0        0        0     2323 2023-04-07 19:29:44.242347 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/storage/templates/genindex_v2.html
--rw-r--r--   0        0        0      758 2023-04-07 19:29:44.242347 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/storage/templates/search.html
--rw-r--r--   0        0        0   136506 2023-05-14 03:33:11.714778 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/storage/translator.py
--rw-r--r--   0        0        0     7571 2023-04-08 04:21:05.378651 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/svg.py
--rw-r--r--   0        0        0    17887 2023-04-22 17:53:45.115343 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/translator.py
--rw-r--r--   0        0        0    12095 2023-04-07 19:29:44.246253 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/transmute/__init__.py
--rw-r--r--   0        0        0     1910 2023-04-07 19:29:44.246253 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/transmute/ext_jupyter_sphinx.py
--rw-r--r--   0        0        0     1743 2023-04-07 19:29:44.247227 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/transmute/ext_nbsphinx.py
--rw-r--r--   0        0        0     2534 2023-04-07 19:29:44.247227 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/transmute/ext_sphinx_diagrams.py
--rw-r--r--   0        0        0     1556 2023-04-07 19:29:44.248204 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/transmute/ext_sphinx_gallery.py
--rw-r--r--   0        0        0     4240 2023-04-07 19:29:44.249180 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/transmute/ext_sphinx_toolbox.py
--rw-r--r--   0        0        0     2520 2023-04-07 19:29:44.249180 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/transmute/ext_sphinxcontrib_mermaid.py
--rw-r--r--   0        0        0    11692 2023-05-14 03:23:15.068220 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/util.py
--rw-r--r--   0        0        0      659 2023-04-07 19:29:44.250159 sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/writer.py
--rw-r--r--   0        0        0     5424 1970-01-01 00:00:00.000000 sphinxcontrib_confluencebuilder-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1330 2023-05-16 01:08:09.090533 sphinxcontrib_confluencebuilder-2.1.1/AUTHORS
+-rw-r--r--   0        0        0     3159 2023-04-07 19:29:44.215004 sphinxcontrib_confluencebuilder-2.1.1/LICENSE
+-rw-r--r--   0        0        0      145 2023-01-02 01:52:19.799871 sphinxcontrib_confluencebuilder-2.1.1/MANIFEST.in
+-rw-r--r--   0        0        0     4076 2023-05-16 00:58:11.667937 sphinxcontrib_confluencebuilder-2.1.1/README.rst
+-rw-r--r--   0        0        0     1828 2023-05-19 23:40:55.298174 sphinxcontrib_confluencebuilder-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0    18061 2023-05-19 23:42:25.549873 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/__init__.py
+-rw-r--r--   0        0        0     3630 2023-04-07 19:29:44.220864 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/__main__.py
+-rw-r--r--   0        0        0    14586 2023-04-15 14:46:27.000054 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/assets.py
+-rw-r--r--   0        0        0    48600 2023-05-13 15:11:25.713682 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/builder.py
+-rw-r--r--   0        0        0        0 2023-01-22 17:27:22.404126 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/cmd/__init__.py
+-rw-r--r--   0        0        0     2442 2023-04-07 19:29:44.222817 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/cmd/build.py
+-rw-r--r--   0        0        0    11521 2023-04-07 19:29:44.222817 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/cmd/report.py
+-rw-r--r--   0        0        0     6780 2023-04-08 16:47:36.734308 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/cmd/wipe.py
+-rw-r--r--   0        0        0     3476 2023-04-07 19:29:44.224766 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/compat.py
+-rw-r--r--   0        0        0     2929 2023-04-08 16:47:36.735307 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/config/__init__.py
+-rw-r--r--   0        0        0    28152 2023-04-17 01:06:14.719799 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/config/checks.py
+-rw-r--r--   0        0        0     4150 2023-04-16 01:30:57.889226 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/config/defaults.py
+-rw-r--r--   0        0        0     1431 2023-04-07 19:29:44.227698 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/config/env.py
+-rw-r--r--   0        0        0     3529 2023-04-07 19:29:44.227698 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/config/manager.py
+-rw-r--r--   0        0        0     3402 2023-04-08 16:47:36.736308 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/config/notifications.py
+-rw-r--r--   0        0        0    17687 2023-04-07 19:29:44.229651 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/config/validation.py
+-rw-r--r--   0        0        0    11596 2023-05-13 21:00:30.923234 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/directives.py
+-rw-r--r--   0        0        0     9196 2023-04-07 19:29:44.230626 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/exceptions.py
+-rw-r--r--   0        0        0     3057 2023-04-07 19:29:44.231602 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/intersphinx.py
+-rw-r--r--   0        0        0      432 2023-04-07 19:29:44.231602 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/__init__.py
+-rw-r--r--   0        0        0      590 2023-01-05 22:53:18.094822 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/ar/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1387 2023-05-16 00:43:39.061378 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/ar/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      533 2023-01-05 22:53:18.096782 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/bg/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1330 2023-05-16 00:43:39.062380 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/bg/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      458 2023-01-05 22:53:18.098731 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/bn/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1284 2023-05-16 00:43:39.063378 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/bn/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      500 2023-01-05 22:53:18.099707 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/ca/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1297 2023-05-16 00:43:39.064377 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/ca/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      526 2023-01-05 22:53:18.100682 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/cs/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1323 2023-05-16 00:43:39.064377 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/cs/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      579 2023-01-05 22:53:18.101658 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/cy/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1376 2023-05-16 00:43:39.065377 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/cy/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      499 2023-01-05 22:53:18.103611 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/da/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1296 2023-05-16 00:43:39.066377 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/da/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      503 2023-01-05 22:53:18.104592 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/de/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1300 2023-05-16 00:43:39.067377 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/de/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      518 2023-01-05 22:53:18.106543 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/el/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1315 2023-05-16 00:43:39.067377 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/el/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      460 2023-01-05 22:53:18.108080 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/eo/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1300 2023-05-16 00:43:39.068378 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/eo/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      458 2023-01-05 22:53:18.109032 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/es/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1287 2023-05-16 00:43:39.068378 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/es/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      505 2023-01-05 22:53:18.110006 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/et/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1302 2023-05-16 00:43:39.069379 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/et/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      500 2023-01-05 22:53:18.111962 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/eu/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1297 2023-05-16 00:43:39.069379 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/eu/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      505 2023-01-05 22:53:18.113918 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/fi/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1302 2023-05-16 00:43:39.070376 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/fi/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      503 2023-01-05 22:53:18.114891 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/fr/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1300 2023-05-16 00:43:39.071378 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/fr/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      507 2023-01-05 22:53:18.116843 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/he/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1333 2023-05-16 00:43:39.071378 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/he/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      535 2023-01-05 22:53:18.117819 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/hi/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1332 2023-05-16 00:43:39.072377 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/hi/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      573 2023-01-05 22:53:18.118796 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/hr/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1370 2023-05-16 00:43:39.072377 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/hr/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      510 2023-01-05 22:53:18.120751 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/hu/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1307 2023-05-16 00:43:39.073376 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/hu/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      497 2023-01-05 22:53:18.122701 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/id/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1294 2023-05-16 00:43:39.074377 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/id/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      458 2023-01-05 22:53:18.124656 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/it/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1284 2023-05-16 00:43:39.074377 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/it/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      499 2023-01-05 22:53:18.125629 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/ja/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1296 2023-05-16 00:43:39.075377 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/ja/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      492 2023-01-05 22:53:18.127584 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/ko/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1289 2023-05-16 00:43:39.075377 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/ko/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      609 2023-01-05 22:53:18.128562 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/lt/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1406 2023-05-16 00:43:39.076379 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/lt/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      535 2023-01-05 22:53:18.130512 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/lv/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1332 2023-05-16 00:43:39.077376 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/lv/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      535 2023-01-05 22:53:18.133442 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/mk/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1332 2023-05-16 00:43:39.080380 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/mk/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      509 2023-01-05 22:53:18.135398 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/nb/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1306 2023-05-16 00:43:39.081380 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/nb/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      551 2023-01-05 22:53:18.137353 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/ne/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1351 2023-05-16 00:43:39.082381 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/ne/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      498 2023-01-05 22:53:18.139304 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/nl/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1295 2023-05-16 00:43:39.083377 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/nl/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      648 2023-01-05 22:53:18.141258 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/pl/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1445 2023-05-16 00:43:39.084381 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/pl/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      513 2023-01-05 22:53:18.143207 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/pt_BR/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1313 2023-05-16 00:43:39.085380 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/pt_BR/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      546 2023-01-05 22:53:18.144187 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/ro/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1343 2023-05-16 00:43:39.085380 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/ro/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      623 2023-01-05 22:53:18.146138 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/ru/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1449 2023-05-16 00:43:39.086379 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/ru/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      458 2023-01-05 22:53:18.148092 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/si/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1287 2023-05-16 00:43:39.086379 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/si/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      527 2023-01-05 22:53:18.150044 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/sk/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1324 2023-05-16 00:43:39.087380 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/sk/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      512 2023-01-05 22:53:18.151996 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/sl/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1338 2023-05-16 00:43:39.088379 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/sl/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      821 2023-05-16 00:43:39.088379 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/sphinxcontrib.confluencebuilder.pot
+-rw-r--r--   0        0        0      511 2023-01-05 22:53:18.153947 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/sq/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1308 2023-05-16 00:43:39.089376 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/sq/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      540 2023-01-05 22:53:18.155966 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/sr_CS/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1369 2023-05-16 00:43:39.089376 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/sr_CS/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      502 2023-01-05 22:53:18.158443 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/sv/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1302 2023-05-16 00:43:39.090376 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/sv/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      546 2023-01-05 22:53:18.160396 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/ta/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1343 2023-05-16 00:43:39.091378 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/ta/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      538 2023-01-05 22:53:18.162349 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/te/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1335 2023-05-16 00:43:39.091378 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/te/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      505 2023-01-05 22:53:18.164303 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/tr/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1302 2023-05-16 00:43:39.092379 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/tr/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      689 2023-01-05 22:53:18.165278 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/uk/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1486 2023-05-16 00:43:39.092379 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/uk/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      496 2023-01-05 22:53:18.167232 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/vi/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1293 2023-05-16 00:43:39.093380 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/vi/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      504 2023-01-05 22:48:19.243628 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/zh_TW/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1304 2023-05-16 00:43:53.313328 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/zh_TW/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0     4581 2023-04-07 19:29:44.232579 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/logger.py
+-rw-r--r--   0        0        0     6304 2023-05-13 21:00:30.923234 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/nodes.py
+-rw-r--r--   0        0        0    49499 2023-05-14 05:04:32.872359 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/publisher.py
+-rw-r--r--   0        0        0      430 2023-04-07 19:29:44.234534 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/reportbuilder.py
+-rw-r--r--   0        0        0    14702 2023-04-07 19:29:44.235511 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/rest.py
+-rw-r--r--   0        0        0     7784 2023-05-13 21:00:30.924232 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/roles.py
+-rw-r--r--   0        0        0    11845 2023-04-07 19:29:44.236486 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/singlebuilder.py
+-rw-r--r--   0        0        0     9455 2023-04-07 19:29:44.237465 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/state.py
+-rw-r--r--   0        0        0        0 2023-01-22 17:27:22.418126 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/std/__init__.py
+-rw-r--r--   0        0        0    12663 2023-04-07 19:29:44.237465 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/std/confluence.py
+-rw-r--r--   0        0        0      319 2023-04-07 19:29:44.238438 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/std/sphinx.py
+-rw-r--r--   0        0        0     2038 2023-04-07 19:29:44.238438 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/storage/__init__.py
+-rw-r--r--   0        0        0     4747 2023-04-07 19:29:44.239414 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/storage/index.py
+-rw-r--r--   0        0        0     1189 2023-04-07 19:29:44.239414 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/storage/search.py
+-rw-r--r--   0        0        0        0 2023-01-22 17:27:22.420125 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/storage/templates/__init__.py
+-rw-r--r--   0        0        0     1801 2023-04-07 19:29:44.240391 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/storage/templates/domainindex.html
+-rw-r--r--   0        0        0     1634 2023-04-07 19:29:44.241370 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/storage/templates/domainindex_v2.html
+-rw-r--r--   0        0        0     2201 2023-04-07 19:29:44.241370 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/storage/templates/genindex.html
+-rw-r--r--   0        0        0     2323 2023-04-07 19:29:44.242347 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/storage/templates/genindex_v2.html
+-rw-r--r--   0        0        0      758 2023-04-07 19:29:44.242347 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/storage/templates/search.html
+-rw-r--r--   0        0        0   136545 2023-05-19 23:40:45.834292 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/storage/translator.py
+-rw-r--r--   0        0        0     7571 2023-04-08 04:21:05.378651 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/svg.py
+-rw-r--r--   0        0        0    17887 2023-04-22 17:53:45.115343 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/translator.py
+-rw-r--r--   0        0        0    12095 2023-04-07 19:29:44.246253 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/transmute/__init__.py
+-rw-r--r--   0        0        0     1910 2023-04-07 19:29:44.246253 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/transmute/ext_jupyter_sphinx.py
+-rw-r--r--   0        0        0     1743 2023-04-07 19:29:44.247227 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/transmute/ext_nbsphinx.py
+-rw-r--r--   0        0        0     2534 2023-04-07 19:29:44.247227 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/transmute/ext_sphinx_diagrams.py
+-rw-r--r--   0        0        0     1556 2023-04-07 19:29:44.248204 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/transmute/ext_sphinx_gallery.py
+-rw-r--r--   0        0        0     4240 2023-04-07 19:29:44.249180 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/transmute/ext_sphinx_toolbox.py
+-rw-r--r--   0        0        0     2520 2023-04-07 19:29:44.249180 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/transmute/ext_sphinxcontrib_mermaid.py
+-rw-r--r--   0        0        0    11692 2023-05-14 03:23:15.068220 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/util.py
+-rw-r--r--   0        0        0      659 2023-04-07 19:29:44.250159 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/writer.py
+-rw-r--r--   0        0        0     5424 1970-01-01 00:00:00.000000 sphinxcontrib_confluencebuilder-2.1.1/PKG-INFO
```

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/README.rst` & `sphinxcontrib_confluencebuilder-2.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/pyproject.toml` & `sphinxcontrib_confluencebuilder-2.1.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,14 @@
     {name = 'Anthony Shaw', email = 'anthonyshaw@apache.org'},
 ]
 maintainers = [
     {name = 'James Knight', email = 'james.d.knight@live.com'},
 ]
 requires-python = '>=3.7'
 readme = 'README.rst'
-license = {text = 'BSD-2-Clause'}
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Environment :: Console',
     'Environment :: Web Environment',
     'Framework :: Sphinx',
     'Framework :: Sphinx :: Extension',
     'Intended Audience :: Developers',
@@ -51,7 +50,14 @@
 Source = 'https://github.com/sphinx-contrib/confluencebuilder'
 
 [project.scripts]
 sphinx-build-confluence = 'sphinxcontrib.confluencebuilder.__main__:main'
 
 [tool.flit.module]
 name = 'sphinxcontrib.confluencebuilder'
+
+[tool.flit.sdist]
+include = [
+    'AUTHORS',
+    'LICENSE',
+    'MANIFEST.in',
+]
```

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/__init__.py` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 # load imgmath extension if available to handle math configuration options
 try:
     from sphinx.ext import imgmath
 except ImportError:
     imgmath = None
 
-__version__ = '2.1.0'
+__version__ = '2.1.1'
 
 
 def setup(app):
     ConfluenceLogger.initialize()
     cm = app.config_manager_ = ConfigManager(app)
 
     app.require_sphinx('1.8')
```

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/__main__.py` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/__main__.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/assets.py` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/assets.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/builder.py` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/builder.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/cmd/build.py` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/cmd/build.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/cmd/report.py` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/cmd/report.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/cmd/wipe.py` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/cmd/wipe.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/compat.py` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/compat.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/config/__init__.py` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/config/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/config/checks.py` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/config/checks.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/config/defaults.py` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/config/defaults.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/config/env.py` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/config/env.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/config/manager.py` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/config/manager.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/config/notifications.py` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/config/notifications.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/config/validation.py` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/config/validation.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/directives.py` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/directives.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/exceptions.py` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/exceptions.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/intersphinx.py` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/intersphinx.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/ar/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/ar/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/ar/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/ar/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/bg/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/bg/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/bg/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/bg/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/bn/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/bn/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/ca/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/ca/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/cs/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/cs/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/cs/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/cs/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/cy/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/cy/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/cy/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/cy/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/da/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/da/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/de/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/de/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/el/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/el/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/el/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/el/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/eo/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/eo/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/es/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/es/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/et/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/et/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/eu/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/eu/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/fi/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/fi/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/fr/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/fr/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/he/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/he/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/hi/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/hi/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/hi/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/hi/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/hr/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/hr/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/hr/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/hr/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/hu/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/hu/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/id/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/id/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/it/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/it/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/ja/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/ja/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/ko/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/ko/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/lt/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/lt/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/lt/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/lt/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/lv/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/lv/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/lv/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/lv/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/mk/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/mk/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/mk/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/mk/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/nb/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/nb/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/ne/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/ne/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/ne/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/ne/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/nl/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/nl/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/pl/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/pl/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/pl/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/pl/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/pt_BR/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/pt_BR/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/pt_BR/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/pt_BR/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/ro/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/ro/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/ro/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/ro/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/ru/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/ru/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/ru/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/ru/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/si/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/si/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/sk/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/sk/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/sk/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/sk/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/sl/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/sl/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/sl/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/sl/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/sphinxcontrib.confluencebuilder.pot` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/sphinxcontrib.confluencebuilder.pot`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/sq/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/sq/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/sr_CS/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/sr_CS/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/sr_CS/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/sr_CS/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/sv/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/sv/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/ta/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/ta/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/ta/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/ta/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/te/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/te/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/te/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/te/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/tr/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/tr/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/uk/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/uk/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/uk/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/uk/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/vi/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/vi/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/locale/zh_TW/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/zh_TW/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/logger.py` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/logger.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/nodes.py` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/nodes.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/publisher.py` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/publisher.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/rest.py` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/rest.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/roles.py` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/roles.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/singlebuilder.py` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/singlebuilder.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/state.py` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/state.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/std/confluence.py` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/std/confluence.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/storage/__init__.py` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/storage/index.py` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/storage/index.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/storage/search.py` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/storage/search.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/storage/templates/domainindex.html` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/storage/templates/domainindex.html`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/storage/templates/domainindex_v2.html` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/storage/templates/domainindex_v2.html`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/storage/templates/genindex.html` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/storage/templates/genindex.html`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/storage/templates/genindex_v2.html` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/storage/templates/genindex_v2.html`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/storage/templates/search.html` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/storage/templates/search.html`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/storage/translator.py` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/storage/translator.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,14 +57,15 @@
         self._figure_context = []
         self._indent_level = 0
         self._list_context = ['']
         self._manpage_url = getattr(config, 'manpages_url', None)
         self._needs_navnode_spacing = False
         self._reference_context = []
         self._thead_context = []
+        self._v2_header_added = False
         self.colspecs = []
         self._tocdepth = self.state.toctree_depth(self.docname)
 
     def encode(self, text):
         text = encode_storage_format(text)
         return ConfluenceBaseTranslator.encode(self, text)
```

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/svg.py` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/svg.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/translator.py` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/translator.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/transmute/__init__.py` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/transmute/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/transmute/ext_jupyter_sphinx.py` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/transmute/ext_jupyter_sphinx.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/transmute/ext_nbsphinx.py` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/transmute/ext_nbsphinx.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/transmute/ext_sphinx_diagrams.py` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/transmute/ext_sphinx_diagrams.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/transmute/ext_sphinx_gallery.py` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/transmute/ext_sphinx_gallery.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/transmute/ext_sphinx_toolbox.py` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/transmute/ext_sphinx_toolbox.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/transmute/ext_sphinxcontrib_mermaid.py` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/transmute/ext_sphinxcontrib_mermaid.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/util.py` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/util.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/sphinxcontrib/confluencebuilder/writer.py` & `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/writer.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.0/PKG-INFO` & `sphinxcontrib_confluencebuilder-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinxcontrib-confluencebuilder
-Version: 2.1.0
+Version: 2.1.1
 Summary: Sphinx extension to build Atlassian Confluence Storage Markup
 Author-email: Anthony Shaw <anthonyshaw@apache.org>
 Maintainer-email: James Knight <james.d.knight@live.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

