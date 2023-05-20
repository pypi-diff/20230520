# Comparing `tmp/polygon_finance-1.0.0.tar.gz` & `tmp/polygon_finance-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polygon_finance-1.0.0.tar", last modified: Sat May 20 02:56:54 2023, max compression
+gzip compressed data, was "polygon_finance-1.0.1.tar", last modified: Sat May 20 03:17:59 2023, max compression
```

## Comparing `polygon_finance-1.0.0.tar` & `polygon_finance-1.0.1.tar`

### file list

```diff
@@ -1,41 +1,137 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 02:56:54.043591 polygon_finance-1.0.0/
--rw-rw-rw-   0        0        0      241 2023-05-20 02:56:54.042592 polygon_finance-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-20 02:56:54.024592 polygon_finance-1.0.0/polygon_finance.egg-info/
--rw-rw-rw-   0        0        0      241 2023-05-20 02:56:53.000000 polygon_finance-1.0.0/polygon_finance.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      987 2023-05-20 02:56:53.000000 polygon_finance-1.0.0/polygon_finance.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 02:56:53.000000 polygon_finance-1.0.0/polygon_finance.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1253 2023-05-20 02:56:53.000000 polygon_finance-1.0.0/polygon_finance.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-20 02:56:53.000000 polygon_finance-1.0.0/polygon_finance.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-20 02:56:54.026593 polygon_finance-1.0.0/sdks/
--rw-rw-rw-   0        0        0        0 2023-05-14 16:45:53.000000 polygon_finance-1.0.0/sdks/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-20 02:56:54.027592 polygon_finance-1.0.0/sdks/models/
--rw-rw-rw-   0        0        0        2 2023-05-14 01:56:34.000000 polygon_finance-1.0.0/sdks/models/__init__.py
--rw-rw-rw-   0        0        0      511 2023-05-14 01:56:34.000000 polygon_finance-1.0.0/sdks/models/common.py
--rw-rw-rw-   0        0        0    13169 2023-05-20 01:07:08.000000 polygon_finance-1.0.0/sdks/models/test_events.py
-drwxrwxrwx   0        0        0        0 2023-05-20 02:56:54.028590 polygon_finance-1.0.0/sdks/terminals/
--rw-rw-rw-   0        0        0        0 2023-05-14 16:41:17.000000 polygon_finance-1.0.0/sdks/terminals/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-20 02:56:54.029590 polygon_finance-1.0.0/sdks/terminals/crypto/
--rw-rw-rw-   0        0        0        0 2023-05-14 16:42:17.000000 polygon_finance-1.0.0/sdks/terminals/crypto/__init__.py
--rw-rw-rw-   0        0        0     3626 2023-05-14 20:38:44.000000 polygon_finance-1.0.0/sdks/terminals/crypto/crypto_terminal.py
--rw-rw-rw-   0        0        0     1731 2023-05-14 16:53:24.000000 polygon_finance-1.0.0/sdks/terminals/crypto/menu.py
-drwxrwxrwx   0        0        0        0 2023-05-20 02:56:54.042592 polygon_finance-1.0.0/sdks/webull_sdk/
--rw-rw-rw-   0        0        0        2 2023-05-14 01:56:34.000000 polygon_finance-1.0.0/sdks/webull_sdk/__init__.py
--rw-rw-rw-   0        0        0      882 2023-05-14 01:56:34.000000 polygon_finance-1.0.0/sdks/webull_sdk/calendar.py
--rw-rw-rw-   0        0        0     8295 2023-05-15 04:33:49.000000 polygon_finance-1.0.0/sdks/webull_sdk/capitalflow.py
--rw-rw-rw-   0        0        0     1174 2023-05-14 01:56:34.000000 polygon_finance-1.0.0/sdks/webull_sdk/cost_distribution.py
--rw-rw-rw-   0        0        0     2325 2023-05-14 01:56:34.000000 polygon_finance-1.0.0/sdks/webull_sdk/derivative_query.py
--rw-rw-rw-   0        0        0     2426 2023-05-14 01:56:34.000000 polygon_finance-1.0.0/sdks/webull_sdk/etf_finder.py
--rw-rw-rw-   0        0        0      500 2023-05-14 01:56:34.000000 polygon_finance-1.0.0/sdks/webull_sdk/etf_holdings.py
--rw-rw-rw-   0        0        0     1014 2023-05-17 22:12:48.000000 polygon_finance-1.0.0/sdks/webull_sdk/events.py
--rw-rw-rw-   0        0        0     7818 2023-05-14 01:56:34.000000 polygon_finance-1.0.0/sdks/webull_sdk/financial_statement.py
--rw-rw-rw-   0        0        0     3871 2023-05-14 01:56:34.000000 polygon_finance-1.0.0/sdks/webull_sdk/forecast.py
--rw-rw-rw-   0        0        0     1033 2023-05-14 01:56:34.000000 polygon_finance-1.0.0/sdks/webull_sdk/institutional_holdings.py
--rw-rw-rw-   0        0        0     1156 2023-05-14 01:56:34.000000 polygon_finance-1.0.0/sdks/webull_sdk/manage.py
--rw-rw-rw-   0        0        0      617 2023-05-14 01:56:34.000000 polygon_finance-1.0.0/sdks/webull_sdk/news.py
--rw-rw-rw-   0        0        0      307 2023-05-14 01:56:34.000000 polygon_finance-1.0.0/sdks/webull_sdk/shortinterest.py
--rw-rw-rw-   0        0        0     2768 2023-05-15 04:24:58.000000 polygon_finance-1.0.0/sdks/webull_sdk/top_gainers.py
--rw-rw-rw-   0        0        0    16723 2023-05-14 01:56:34.000000 polygon_finance-1.0.0/sdks/webull_sdk/top_options.py
--rw-rw-rw-   0        0        0     5556 2023-05-14 01:56:34.000000 polygon_finance-1.0.0/sdks/webull_sdk/webull_data.py
--rw-rw-rw-   0        0        0    43244 2023-05-15 04:26:38.000000 polygon_finance-1.0.0/sdks/webull_sdk/webull_sdk.py
--rw-rw-rw-   0        0        0       42 2023-05-20 02:56:54.043591 polygon_finance-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     2577 2023-05-20 02:56:15.000000 polygon_finance-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:17:59.675260 polygon_finance-1.0.1/
+-rw-rw-rw-   0        0        0      241 2023-05-20 03:17:59.674260 polygon_finance-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-20 03:17:59.594316 polygon_finance-1.0.1/discord/
+-rw-rw-rw-   0        0        0        0 2023-05-20 03:05:54.000000 polygon_finance-1.0.1/discord/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:17:59.595602 polygon_finance-1.0.1/discord/conditions/
+-rw-rw-rw-   0        0        0        0 2023-05-20 03:05:57.000000 polygon_finance-1.0.1/discord/conditions/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-20 01:47:54.000000 polygon_finance-1.0.1/discord/conditions/conditions.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:17:59.599605 polygon_finance-1.0.1/discord/discord_utils/
+-rw-rw-rw-   0        0        0        2 2023-05-14 06:35:12.000000 polygon_finance-1.0.1/discord/discord_utils/__init__.py
+-rw-rw-rw-   0        0        0    45717 2023-05-17 23:45:59.000000 polygon_finance-1.0.1/discord/discord_utils/discord_stock_market.py
+-rw-rw-rw-   0        0        0      569 2023-05-20 01:55:03.000000 polygon_finance-1.0.1/discord/discord_utils/emojis.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:17:59.603605 polygon_finance-1.0.1/discord/discord_utils/hooks/
+-rw-rw-rw-   0        0        0        2 2023-05-14 01:56:34.000000 polygon_finance-1.0.1/discord/discord_utils/hooks/__init__.py
+-rw-rw-rw-   0        0        0     1633 2023-05-15 20:55:38.000000 polygon_finance-1.0.1/discord/discord_utils/hooks/channel_webhooks.py
+-rw-rw-rw-   0        0        0     5545 2023-05-14 05:22:53.000000 polygon_finance-1.0.1/discord/discord_utils/hooks/send_webhook.py
+-rw-rw-rw-   0        0        0       53 2023-05-20 01:09:02.000000 polygon_finance-1.0.1/discord/discord_utils/hooks/test_webhooks.py
+-rw-rw-rw-   0        0        0     7298 2023-05-14 01:56:34.000000 polygon_finance-1.0.1/discord/discord_utils/hooks/webhook_info.py
+-rw-rw-rw-   0        0        0    39008 2023-05-15 21:37:55.000000 polygon_finance-1.0.1/discord/discord_utils/live_discord.py
+-rw-rw-rw-   0        0        0     3927 2023-05-14 01:56:34.000000 polygon_finance-1.0.1/discord/discord_utils/menus.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:17:59.604604 polygon_finance-1.0.1/discord/discord_utils/selectmenus/
+-rw-rw-rw-   0        0        0        2 2023-05-14 01:56:34.000000 polygon_finance-1.0.1/discord/discord_utils/selectmenus/__init__.py
+-rw-rw-rw-   0        0        0    36637 2023-05-19 03:39:31.000000 polygon_finance-1.0.1/discord/discord_utils/selectmenus/mainselect.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:17:59.605604 polygon_finance-1.0.1/discord/discord_utils/views/
+-rw-rw-rw-   0        0        0        2 2023-05-14 01:56:34.000000 polygon_finance-1.0.1/discord/discord_utils/views/__init__.py
+-rw-rw-rw-   0        0        0     1696 2023-05-14 20:38:44.000000 polygon_finance-1.0.1/discord/discord_utils/views/mainview.py
+-rw-rw-rw-   0        0        0     6516 2023-05-20 02:30:22.000000 polygon_finance-1.0.1/discord/discord_utils/webhook_creation.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:17:59.607603 polygon_finance-1.0.1/discord/embeddings/
+-rw-rw-rw-   0        0        0        0 2023-05-20 03:06:01.000000 polygon_finance-1.0.1/discord/embeddings/__init__.py
+-rw-rw-rw-   0        0        0      934 2023-05-14 01:56:34.000000 polygon_finance-1.0.1/discord/embeddings/embeddings.py
+-rw-rw-rw-   0        0        0    10062 2023-05-20 01:50:41.000000 polygon_finance-1.0.1/discord/embeddings/embeds.py
+-rw-rw-rw-   0        0        0     2887 2023-05-20 03:06:46.000000 polygon_finance-1.0.1/discord/webhook_creation.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:17:59.608604 polygon_finance-1.0.1/discord_examples/
+-rw-rw-rw-   0        0        0        0 2023-05-20 03:04:36.000000 polygon_finance-1.0.1/discord_examples/__init__.py
+-rw-rw-rw-   0        0        0     3102 2023-05-19 16:28:52.000000 polygon_finance-1.0.1/discord_examples/indices_spx_rsi.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:17:59.622603 polygon_finance-1.0.1/examples/
+-rw-rw-rw-   0        0        0        0 2023-05-20 03:04:40.000000 polygon_finance-1.0.1/examples/__init__.py
+-rw-rw-rw-   0        0        0     6363 2023-05-20 03:06:46.000000 polygon_finance-1.0.1/examples/all_attributes.py
+-rw-rw-rw-   0        0        0      538 2023-05-20 03:06:46.000000 polygon_finance-1.0.1/examples/bollinger_bands.py
+-rw-rw-rw-   0        0        0      735 2023-05-20 03:06:46.000000 polygon_finance-1.0.1/examples/create_option_symbol.py
+-rw-rw-rw-   0        0        0     1721 2023-05-20 03:06:46.000000 polygon_finance-1.0.1/examples/ema.py
+-rw-rw-rw-   0        0        0      943 2023-05-20 03:06:46.000000 polygon_finance-1.0.1/examples/fetch_entire_chain.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:17:59.639602 polygon_finance-1.0.1/examples/functions/
+-rw-rw-rw-   0        0        0        0 2023-05-20 03:04:44.000000 polygon_finance-1.0.1/examples/functions/__init__.py
+-rw-rw-rw-   0        0        0     6363 2023-05-14 20:38:44.000000 polygon_finance-1.0.1/examples/functions/all_attributes.py
+-rw-rw-rw-   0        0        0      538 2023-05-17 16:27:39.000000 polygon_finance-1.0.1/examples/functions/bollinger_bands.py
+-rw-rw-rw-   0        0        0      735 2023-05-15 06:22:03.000000 polygon_finance-1.0.1/examples/functions/create_option_symbol.py
+-rw-rw-rw-   0        0        0     1721 2023-05-15 03:20:42.000000 polygon_finance-1.0.1/examples/functions/ema.py
+-rw-rw-rw-   0        0        0      943 2023-05-15 02:59:26.000000 polygon_finance-1.0.1/examples/functions/fetch_entire_chain.py
+-rw-rw-rw-   0        0        0      676 2023-05-16 19:15:37.000000 polygon_finance-1.0.1/examples/functions/find_gaps.py
+-rw-rw-rw-   0        0        0      852 2023-05-19 02:37:46.000000 polygon_finance-1.0.1/examples/functions/get_all_options_data.py
+-rw-rw-rw-   0        0        0     2489 2023-05-15 21:45:33.000000 polygon_finance-1.0.1/examples/functions/get_ema.py
+-rw-rw-rw-   0        0        0      622 2023-05-14 23:53:48.000000 polygon_finance-1.0.1/examples/functions/get_latest_crypto_data.py
+-rw-rw-rw-   0        0        0      609 2023-05-14 23:52:25.000000 polygon_finance-1.0.1/examples/functions/get_latest_forex_data.py
+-rw-rw-rw-   0        0        0      465 2023-05-14 20:38:44.000000 polygon_finance-1.0.1/examples/functions/get_latest_indices_data.py
+-rw-rw-rw-   0        0        0     3269 2023-05-15 21:39:17.000000 polygon_finance-1.0.1/examples/functions/get_macd.py
+-rw-rw-rw-   0        0        0      606 2023-05-16 23:07:21.000000 polygon_finance-1.0.1/examples/functions/get_pivot_points.py
+-rw-rw-rw-   0        0        0     2139 2023-05-15 21:40:13.000000 polygon_finance-1.0.1/examples/functions/get_rsi.py
+-rw-rw-rw-   0        0        0     2263 2023-05-19 03:35:23.000000 polygon_finance-1.0.1/examples/functions/get_sma.py
+-rw-rw-rw-   0        0        0     1796 2023-05-15 03:01:37.000000 polygon_finance-1.0.1/examples/functions/latest_news.py
+-rw-rw-rw-   0        0        0     1673 2023-05-15 06:36:53.000000 polygon_finance-1.0.1/examples/functions/option_quote.py
+-rw-rw-rw-   0        0        0     2474 2023-05-15 03:00:50.000000 polygon_finance-1.0.1/examples/functions/option_trades.py
+-rw-rw-rw-   0        0        0     1460 2023-05-19 03:26:46.000000 polygon_finance-1.0.1/examples/functions/plot_aggs.py
+-rw-rw-rw-   0        0        0      837 2023-05-19 03:03:57.000000 polygon_finance-1.0.1/examples/functions/plot_macd.py
+-rw-rw-rw-   0        0        0     1859 2023-05-19 02:59:03.000000 polygon_finance-1.0.1/examples/functions/plot_option_aggs.py
+-rw-rw-rw-   0        0        0      506 2023-05-18 01:15:04.000000 polygon_finance-1.0.1/examples/functions/rate_of_change.py
+-rw-rw-rw-   0        0        0     4983 2023-05-16 19:07:24.000000 polygon_finance-1.0.1/examples/functions/scanner_example.py
+-rw-rw-rw-   0        0        0     2180 2023-05-15 03:17:55.000000 polygon_finance-1.0.1/examples/functions/stock_aggregates.py
+-rw-rw-rw-   0        0        0     5359 2023-05-14 01:56:34.000000 polygon_finance-1.0.1/examples/functions/summarizer.py
+-rw-rw-rw-   0        0        0     1226 2023-05-16 18:14:43.000000 polygon_finance-1.0.1/examples/functions/support_resistance.py
+-rw-rw-rw-   0        0        0      852 2023-05-20 03:06:46.000000 polygon_finance-1.0.1/examples/get_all_options_data.py
+-rw-rw-rw-   0        0        0      622 2023-05-20 03:06:46.000000 polygon_finance-1.0.1/examples/get_latest_crypto_data.py
+-rw-rw-rw-   0        0        0      609 2023-05-20 03:06:46.000000 polygon_finance-1.0.1/examples/get_latest_forex_data.py
+-rw-rw-rw-   0        0        0      465 2023-05-20 03:06:46.000000 polygon_finance-1.0.1/examples/get_latest_indices_data.py
+-rw-rw-rw-   0        0        0      670 2023-05-20 03:06:46.000000 polygon_finance-1.0.1/examples/get_latest_ticker_data.py
+-rw-rw-rw-   0        0        0      606 2023-05-20 03:06:46.000000 polygon_finance-1.0.1/examples/get_pivot_points.py
+-rw-rw-rw-   0        0        0     1852 2023-05-20 03:06:46.000000 polygon_finance-1.0.1/examples/latest_news.py
+-rw-rw-rw-   0        0        0     1673 2023-05-20 03:06:46.000000 polygon_finance-1.0.1/examples/option_quote.py
+-rw-rw-rw-   0        0        0     2474 2023-05-20 03:06:46.000000 polygon_finance-1.0.1/examples/option_trades.py
+-rw-rw-rw-   0        0        0     1460 2023-05-20 03:06:46.000000 polygon_finance-1.0.1/examples/plot_aggs.py
+-rw-rw-rw-   0        0        0      837 2023-05-20 03:06:46.000000 polygon_finance-1.0.1/examples/plot_macd.py
+-rw-rw-rw-   0        0        0     1859 2023-05-20 03:06:46.000000 polygon_finance-1.0.1/examples/plot_option_aggs.py
+-rw-rw-rw-   0        0        0      506 2023-05-20 03:06:46.000000 polygon_finance-1.0.1/examples/rate_of_change.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:17:59.643602 polygon_finance-1.0.1/examples/realtime_markets/
+-rw-rw-rw-   0        0        0        0 2023-05-20 03:04:48.000000 polygon_finance-1.0.1/examples/realtime_markets/__init__.py
+-rw-rw-rw-   0        0        0     2575 2023-05-19 18:23:30.000000 polygon_finance-1.0.1/examples/realtime_markets/crypto_market.py
+-rw-rw-rw-   0        0        0      982 2023-05-19 18:24:05.000000 polygon_finance-1.0.1/examples/realtime_markets/forex_market.py
+-rw-rw-rw-   0        0        0      822 2023-05-19 18:24:31.000000 polygon_finance-1.0.1/examples/realtime_markets/indices_market.py
+-rw-rw-rw-   0        0        0     1026 2023-05-14 20:38:44.000000 polygon_finance-1.0.1/examples/realtime_markets/options_market.py
+-rw-rw-rw-   0        0        0     9370 2023-05-19 23:52:09.000000 polygon_finance-1.0.1/examples/realtime_markets/stock_market.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:17:59.646604 polygon_finance-1.0.1/examples/simulated_markets/
+-rw-rw-rw-   0        0        0        0 2023-05-20 03:04:53.000000 polygon_finance-1.0.1/examples/simulated_markets/__init__.py
+-rw-rw-rw-   0        0        0      707 2023-05-15 07:34:31.000000 polygon_finance-1.0.1/examples/simulated_markets/helpers.py
+-rw-rw-rw-   0        0        0     5021 2023-05-20 01:49:17.000000 polygon_finance-1.0.1/examples/simulated_markets/mock_discord.py
+-rw-rw-rw-   0        0        0     2039 2023-05-19 23:31:26.000000 polygon_finance-1.0.1/examples/simulated_markets/mock_market.py
+-rw-rw-rw-   0        0        0     1869 2023-05-20 03:11:50.000000 polygon_finance-1.0.1/examples/simulated_markets/mock_options_market.py
+-rw-rw-rw-   0        0        0     2180 2023-05-20 03:06:46.000000 polygon_finance-1.0.1/examples/stock_aggregates.py
+-rw-rw-rw-   0        0        0     5359 2023-05-20 03:06:46.000000 polygon_finance-1.0.1/examples/summarizer.py
+-rw-rw-rw-   0        0        0     1226 2023-05-20 03:06:46.000000 polygon_finance-1.0.1/examples/support_resistance.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:17:59.653606 polygon_finance-1.0.1/polygon_finance.egg-info/
+-rw-rw-rw-   0        0        0      241 2023-05-20 03:17:59.000000 polygon_finance-1.0.1/polygon_finance.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3938 2023-05-20 03:17:59.000000 polygon_finance-1.0.1/polygon_finance.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 03:17:59.000000 polygon_finance-1.0.1/polygon_finance.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1253 2023-05-20 03:17:59.000000 polygon_finance-1.0.1/polygon_finance.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       39 2023-05-20 03:17:59.000000 polygon_finance-1.0.1/polygon_finance.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-20 03:17:59.654605 polygon_finance-1.0.1/sdks/
+-rw-rw-rw-   0        0        0        0 2023-05-14 16:45:53.000000 polygon_finance-1.0.1/sdks/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:17:59.657605 polygon_finance-1.0.1/sdks/models/
+-rw-rw-rw-   0        0        0        2 2023-05-14 01:56:34.000000 polygon_finance-1.0.1/sdks/models/__init__.py
+-rw-rw-rw-   0        0        0      511 2023-05-14 01:56:34.000000 polygon_finance-1.0.1/sdks/models/common.py
+-rw-rw-rw-   0        0        0    13169 2023-05-20 01:07:08.000000 polygon_finance-1.0.1/sdks/models/test_events.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:17:59.658607 polygon_finance-1.0.1/sdks/terminals/
+-rw-rw-rw-   0        0        0        0 2023-05-14 16:41:17.000000 polygon_finance-1.0.1/sdks/terminals/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:17:59.660606 polygon_finance-1.0.1/sdks/terminals/crypto/
+-rw-rw-rw-   0        0        0        0 2023-05-14 16:42:17.000000 polygon_finance-1.0.1/sdks/terminals/crypto/__init__.py
+-rw-rw-rw-   0        0        0     3626 2023-05-14 20:38:44.000000 polygon_finance-1.0.1/sdks/terminals/crypto/crypto_terminal.py
+-rw-rw-rw-   0        0        0     1731 2023-05-14 16:53:24.000000 polygon_finance-1.0.1/sdks/terminals/crypto/menu.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:17:59.673261 polygon_finance-1.0.1/sdks/webull_sdk/
+-rw-rw-rw-   0        0        0        2 2023-05-14 01:56:34.000000 polygon_finance-1.0.1/sdks/webull_sdk/__init__.py
+-rw-rw-rw-   0        0        0      882 2023-05-14 01:56:34.000000 polygon_finance-1.0.1/sdks/webull_sdk/calendar.py
+-rw-rw-rw-   0        0        0     8295 2023-05-15 04:33:49.000000 polygon_finance-1.0.1/sdks/webull_sdk/capitalflow.py
+-rw-rw-rw-   0        0        0     1174 2023-05-14 01:56:34.000000 polygon_finance-1.0.1/sdks/webull_sdk/cost_distribution.py
+-rw-rw-rw-   0        0        0     2325 2023-05-14 01:56:34.000000 polygon_finance-1.0.1/sdks/webull_sdk/derivative_query.py
+-rw-rw-rw-   0        0        0     2426 2023-05-14 01:56:34.000000 polygon_finance-1.0.1/sdks/webull_sdk/etf_finder.py
+-rw-rw-rw-   0        0        0      500 2023-05-14 01:56:34.000000 polygon_finance-1.0.1/sdks/webull_sdk/etf_holdings.py
+-rw-rw-rw-   0        0        0     1014 2023-05-17 22:12:48.000000 polygon_finance-1.0.1/sdks/webull_sdk/events.py
+-rw-rw-rw-   0        0        0     7818 2023-05-14 01:56:34.000000 polygon_finance-1.0.1/sdks/webull_sdk/financial_statement.py
+-rw-rw-rw-   0        0        0     3871 2023-05-14 01:56:34.000000 polygon_finance-1.0.1/sdks/webull_sdk/forecast.py
+-rw-rw-rw-   0        0        0     1033 2023-05-14 01:56:34.000000 polygon_finance-1.0.1/sdks/webull_sdk/institutional_holdings.py
+-rw-rw-rw-   0        0        0     1156 2023-05-14 01:56:34.000000 polygon_finance-1.0.1/sdks/webull_sdk/manage.py
+-rw-rw-rw-   0        0        0      617 2023-05-14 01:56:34.000000 polygon_finance-1.0.1/sdks/webull_sdk/news.py
+-rw-rw-rw-   0        0        0      307 2023-05-14 01:56:34.000000 polygon_finance-1.0.1/sdks/webull_sdk/shortinterest.py
+-rw-rw-rw-   0        0        0     2768 2023-05-15 04:24:58.000000 polygon_finance-1.0.1/sdks/webull_sdk/top_gainers.py
+-rw-rw-rw-   0        0        0    16723 2023-05-14 01:56:34.000000 polygon_finance-1.0.1/sdks/webull_sdk/top_options.py
+-rw-rw-rw-   0        0        0     5556 2023-05-14 01:56:34.000000 polygon_finance-1.0.1/sdks/webull_sdk/webull_data.py
+-rw-rw-rw-   0        0        0    43244 2023-05-15 04:26:38.000000 polygon_finance-1.0.1/sdks/webull_sdk/webull_sdk.py
+-rw-rw-rw-   0        0        0       42 2023-05-20 03:17:59.675260 polygon_finance-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     2577 2023-05-20 03:17:35.000000 polygon_finance-1.0.1/setup.py
```

### Comparing `polygon_finance-1.0.0/polygon_finance.egg-info/requires.txt` & `polygon_finance-1.0.1/polygon_finance.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.0/sdks/models/test_events.py` & `polygon_finance-1.0.1/sdks/models/test_events.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.0/sdks/terminals/crypto/crypto_terminal.py` & `polygon_finance-1.0.1/sdks/terminals/crypto/crypto_terminal.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.0/sdks/terminals/crypto/menu.py` & `polygon_finance-1.0.1/sdks/terminals/crypto/menu.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.0/sdks/webull_sdk/calendar.py` & `polygon_finance-1.0.1/sdks/webull_sdk/calendar.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.0/sdks/webull_sdk/capitalflow.py` & `polygon_finance-1.0.1/sdks/webull_sdk/capitalflow.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.0/sdks/webull_sdk/cost_distribution.py` & `polygon_finance-1.0.1/sdks/webull_sdk/cost_distribution.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.0/sdks/webull_sdk/derivative_query.py` & `polygon_finance-1.0.1/sdks/webull_sdk/derivative_query.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.0/sdks/webull_sdk/etf_finder.py` & `polygon_finance-1.0.1/sdks/webull_sdk/etf_finder.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.0/sdks/webull_sdk/events.py` & `polygon_finance-1.0.1/sdks/webull_sdk/events.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.0/sdks/webull_sdk/financial_statement.py` & `polygon_finance-1.0.1/sdks/webull_sdk/financial_statement.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.0/sdks/webull_sdk/forecast.py` & `polygon_finance-1.0.1/sdks/webull_sdk/forecast.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.0/sdks/webull_sdk/institutional_holdings.py` & `polygon_finance-1.0.1/sdks/webull_sdk/institutional_holdings.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.0/sdks/webull_sdk/manage.py` & `polygon_finance-1.0.1/sdks/webull_sdk/manage.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.0/sdks/webull_sdk/news.py` & `polygon_finance-1.0.1/sdks/webull_sdk/news.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.0/sdks/webull_sdk/top_gainers.py` & `polygon_finance-1.0.1/sdks/webull_sdk/top_gainers.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.0/sdks/webull_sdk/top_options.py` & `polygon_finance-1.0.1/sdks/webull_sdk/top_options.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.0/sdks/webull_sdk/webull_data.py` & `polygon_finance-1.0.1/sdks/webull_sdk/webull_data.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.0/sdks/webull_sdk/webull_sdk.py` & `polygon_finance-1.0.1/sdks/webull_sdk/webull_sdk.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.0/setup.py` & `polygon_finance-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='polygon_finance',
-    version='1.0.0',
+    version='1.0.1',
     description='The real-time market analysis library that utilizes the real-time rest apis and websockets from polygon.io',
     author='Charlies Vids',
     author_email='chuckdustin12@gmail.com',
     packages=find_packages(),
     install_requires=[
         'aiofiles==23.1.0',
         'aiohttp==3.8.4',
```

