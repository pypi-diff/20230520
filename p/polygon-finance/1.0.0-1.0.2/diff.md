# Comparing `tmp/polygon_finance-1.0.0.tar.gz` & `tmp/polygon_finance-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polygon_finance-1.0.0.tar", last modified: Sat May 20 02:56:54 2023, max compression
+gzip compressed data, was "polygon_finance-1.0.2.tar", last modified: Sat May 20 03:43:33 2023, max compression
```

## Comparing `polygon_finance-1.0.0.tar` & `polygon_finance-1.0.2.tar`

### file list

```diff
@@ -1,41 +1,120 @@
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
+drwxrwxrwx   0        0        0        0 2023-05-20 03:43:33.694891 polygon_finance-1.0.2/
+-rw-rw-rw-   0        0        0      241 2023-05-20 03:43:33.694891 polygon_finance-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-20 03:43:33.615287 polygon_finance-1.0.2/polygon_finance/
+-rw-rw-rw-   0        0        0        0 2023-05-14 16:45:53.000000 polygon_finance-1.0.2/polygon_finance/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:43:33.625286 polygon_finance-1.0.2/polygon_finance/discord/
+-rw-rw-rw-   0        0        0        0 2023-05-20 03:05:54.000000 polygon_finance-1.0.2/polygon_finance/discord/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:43:33.626286 polygon_finance-1.0.2/polygon_finance/discord/conditions/
+-rw-rw-rw-   0        0        0        0 2023-05-20 03:05:57.000000 polygon_finance-1.0.2/polygon_finance/discord/conditions/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-20 01:47:54.000000 polygon_finance-1.0.2/polygon_finance/discord/conditions/conditions.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:43:33.629286 polygon_finance-1.0.2/polygon_finance/discord/discord_utils/
+-rw-rw-rw-   0        0        0        2 2023-05-14 06:35:12.000000 polygon_finance-1.0.2/polygon_finance/discord/discord_utils/__init__.py
+-rw-rw-rw-   0        0        0    45761 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/discord/discord_utils/discord_stock_market.py
+-rw-rw-rw-   0        0        0      569 2023-05-20 01:55:03.000000 polygon_finance-1.0.2/polygon_finance/discord/discord_utils/emojis.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:43:33.633287 polygon_finance-1.0.2/polygon_finance/discord/discord_utils/hooks/
+-rw-rw-rw-   0        0        0        2 2023-05-14 01:56:34.000000 polygon_finance-1.0.2/polygon_finance/discord/discord_utils/hooks/__init__.py
+-rw-rw-rw-   0        0        0     1633 2023-05-15 20:55:38.000000 polygon_finance-1.0.2/polygon_finance/discord/discord_utils/hooks/channel_webhooks.py
+-rw-rw-rw-   0        0        0     5556 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/discord/discord_utils/hooks/send_webhook.py
+-rw-rw-rw-   0        0        0       53 2023-05-20 01:09:02.000000 polygon_finance-1.0.2/polygon_finance/discord/discord_utils/hooks/test_webhooks.py
+-rw-rw-rw-   0        0        0     7298 2023-05-14 01:56:34.000000 polygon_finance-1.0.2/polygon_finance/discord/discord_utils/hooks/webhook_info.py
+-rw-rw-rw-   0        0        0    39052 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/discord/discord_utils/live_discord.py
+-rw-rw-rw-   0        0        0     3927 2023-05-14 01:56:34.000000 polygon_finance-1.0.2/polygon_finance/discord/discord_utils/menus.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:43:33.634287 polygon_finance-1.0.2/polygon_finance/discord/discord_utils/selectmenus/
+-rw-rw-rw-   0        0        0        2 2023-05-14 01:56:34.000000 polygon_finance-1.0.2/polygon_finance/discord/discord_utils/selectmenus/__init__.py
+-rw-rw-rw-   0        0        0    36758 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/discord/discord_utils/selectmenus/mainselect.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:43:33.636369 polygon_finance-1.0.2/polygon_finance/discord/discord_utils/views/
+-rw-rw-rw-   0        0        0        2 2023-05-14 01:56:34.000000 polygon_finance-1.0.2/polygon_finance/discord/discord_utils/views/__init__.py
+-rw-rw-rw-   0        0        0     1707 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/discord/discord_utils/views/mainview.py
+-rw-rw-rw-   0        0        0     6516 2023-05-20 02:30:22.000000 polygon_finance-1.0.2/polygon_finance/discord/discord_utils/webhook_creation.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:43:33.639371 polygon_finance-1.0.2/polygon_finance/discord/embeddings/
+-rw-rw-rw-   0        0        0        0 2023-05-20 03:06:01.000000 polygon_finance-1.0.2/polygon_finance/discord/embeddings/__init__.py
+-rw-rw-rw-   0        0        0      934 2023-05-14 01:56:34.000000 polygon_finance-1.0.2/polygon_finance/discord/embeddings/embeddings.py
+-rw-rw-rw-   0        0        0    10106 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/discord/embeddings/embeds.py
+-rw-rw-rw-   0        0        0     2887 2023-05-20 03:06:46.000000 polygon_finance-1.0.2/polygon_finance/discord/webhook_creation.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:43:33.641371 polygon_finance-1.0.2/polygon_finance/discord_examples/
+-rw-rw-rw-   0        0        0        0 2023-05-20 03:04:36.000000 polygon_finance-1.0.2/polygon_finance/discord_examples/__init__.py
+-rw-rw-rw-   0        0        0     3113 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/discord_examples/indices_spx_rsi.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:43:33.657375 polygon_finance-1.0.2/polygon_finance/examples/
+-rw-rw-rw-   0        0        0        0 2023-05-20 03:04:40.000000 polygon_finance-1.0.2/polygon_finance/examples/__init__.py
+-rw-rw-rw-   0        0        0     6418 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/examples/all_attributes.py
+-rw-rw-rw-   0        0        0      549 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/examples/bollinger_bands.py
+-rw-rw-rw-   0        0        0      746 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/examples/create_option_symbol.py
+-rw-rw-rw-   0        0        0     1732 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/examples/ema.py
+-rw-rw-rw-   0        0        0      976 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/examples/fetch_entire_chain.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:43:33.680890 polygon_finance-1.0.2/polygon_finance/examples/functions/
+-rw-rw-rw-   0        0        0        0 2023-05-20 03:04:44.000000 polygon_finance-1.0.2/polygon_finance/examples/functions/__init__.py
+-rw-rw-rw-   0        0        0     6418 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/examples/functions/all_attributes.py
+-rw-rw-rw-   0        0        0      549 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/examples/functions/bollinger_bands.py
+-rw-rw-rw-   0        0        0      746 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/examples/functions/create_option_symbol.py
+-rw-rw-rw-   0        0        0     1732 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/examples/functions/ema.py
+-rw-rw-rw-   0        0        0      976 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/examples/functions/fetch_entire_chain.py
+-rw-rw-rw-   0        0        0      687 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/examples/functions/find_gaps.py
+-rw-rw-rw-   0        0        0      863 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/examples/functions/get_all_options_data.py
+-rw-rw-rw-   0        0        0     2511 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/examples/functions/get_ema.py
+-rw-rw-rw-   0        0        0      633 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/examples/functions/get_latest_crypto_data.py
+-rw-rw-rw-   0        0        0      620 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/examples/functions/get_latest_forex_data.py
+-rw-rw-rw-   0        0        0      476 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/examples/functions/get_latest_indices_data.py
+-rw-rw-rw-   0        0        0     3291 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/examples/functions/get_macd.py
+-rw-rw-rw-   0        0        0      617 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/examples/functions/get_pivot_points.py
+-rw-rw-rw-   0        0        0     2161 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/examples/functions/get_rsi.py
+-rw-rw-rw-   0        0        0     2285 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/examples/functions/get_sma.py
+-rw-rw-rw-   0        0        0     1807 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/examples/functions/latest_news.py
+-rw-rw-rw-   0        0        0     1695 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/examples/functions/option_quote.py
+-rw-rw-rw-   0        0        0     2496 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/examples/functions/option_trades.py
+-rw-rw-rw-   0        0        0     1471 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/examples/functions/plot_aggs.py
+-rw-rw-rw-   0        0        0      848 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/examples/functions/plot_macd.py
+-rw-rw-rw-   0        0        0     1870 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/examples/functions/plot_option_aggs.py
+-rw-rw-rw-   0        0        0      517 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/examples/functions/rate_of_change.py
+-rw-rw-rw-   0        0        0     5038 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/examples/functions/scanner_example.py
+-rw-rw-rw-   0        0        0     2191 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/examples/functions/stock_aggregates.py
+-rw-rw-rw-   0        0        0     5359 2023-05-14 01:56:34.000000 polygon_finance-1.0.2/polygon_finance/examples/functions/summarizer.py
+-rw-rw-rw-   0        0        0     1237 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/examples/functions/support_resistance.py
+-rw-rw-rw-   0        0        0      863 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/examples/get_all_options_data.py
+-rw-rw-rw-   0        0        0      633 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/examples/get_latest_crypto_data.py
+-rw-rw-rw-   0        0        0      620 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/examples/get_latest_forex_data.py
+-rw-rw-rw-   0        0        0      476 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/examples/get_latest_indices_data.py
+-rw-rw-rw-   0        0        0      681 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/examples/get_latest_ticker_data.py
+-rw-rw-rw-   0        0        0      617 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/examples/get_pivot_points.py
+-rw-rw-rw-   0        0        0     1863 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/examples/latest_news.py
+-rw-rw-rw-   0        0        0     1695 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/examples/option_quote.py
+-rw-rw-rw-   0        0        0     2496 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/examples/option_trades.py
+-rw-rw-rw-   0        0        0     1471 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/examples/plot_aggs.py
+-rw-rw-rw-   0        0        0      848 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/examples/plot_macd.py
+-rw-rw-rw-   0        0        0     1870 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/examples/plot_option_aggs.py
+-rw-rw-rw-   0        0        0      517 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/examples/rate_of_change.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:43:33.686892 polygon_finance-1.0.2/polygon_finance/examples/realtime_markets/
+-rw-rw-rw-   0        0        0        0 2023-05-20 03:04:48.000000 polygon_finance-1.0.2/polygon_finance/examples/realtime_markets/__init__.py
+-rw-rw-rw-   0        0        0     2586 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/examples/realtime_markets/crypto_market.py
+-rw-rw-rw-   0        0        0      993 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/examples/realtime_markets/forex_market.py
+-rw-rw-rw-   0        0        0      833 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/examples/realtime_markets/indices_market.py
+-rw-rw-rw-   0        0        0     1037 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/examples/realtime_markets/options_market.py
+-rw-rw-rw-   0        0        0     9392 2023-05-20 03:42:20.000000 polygon_finance-1.0.2/polygon_finance/examples/realtime_markets/stock_market.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:43:33.689892 polygon_finance-1.0.2/polygon_finance/examples/simulated_markets/
+-rw-rw-rw-   0        0        0        0 2023-05-20 03:04:53.000000 polygon_finance-1.0.2/polygon_finance/examples/simulated_markets/__init__.py
+-rw-rw-rw-   0        0        0      707 2023-05-15 07:34:31.000000 polygon_finance-1.0.2/polygon_finance/examples/simulated_markets/helpers.py
+-rw-rw-rw-   0        0        0     5054 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/examples/simulated_markets/mock_discord.py
+-rw-rw-rw-   0        0        0     2061 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/examples/simulated_markets/mock_market.py
+-rw-rw-rw-   0        0        0     1891 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/examples/simulated_markets/mock_options_market.py
+-rw-rw-rw-   0        0        0     2191 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/examples/stock_aggregates.py
+-rw-rw-rw-   0        0        0     5359 2023-05-20 03:06:46.000000 polygon_finance-1.0.2/polygon_finance/examples/summarizer.py
+-rw-rw-rw-   0        0        0     1237 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/examples/support_resistance.py
+-rw-rw-rw-   0        0        0      681 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/get_latest_ticker_data.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:43:33.691892 polygon_finance-1.0.2/polygon_finance/models/
+-rw-rw-rw-   0        0        0        2 2023-05-14 01:56:34.000000 polygon_finance-1.0.2/polygon_finance/models/__init__.py
+-rw-rw-rw-   0        0        0      511 2023-05-14 01:56:34.000000 polygon_finance-1.0.2/polygon_finance/models/common.py
+-rw-rw-rw-   0        0        0    13169 2023-05-20 01:07:08.000000 polygon_finance-1.0.2/polygon_finance/models/test_events.py
+-rw-rw-rw-   0        0        0     1113 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/start_here.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:43:33.691892 polygon_finance-1.0.2/polygon_finance/terminals/
+-rw-rw-rw-   0        0        0        0 2023-05-14 16:41:17.000000 polygon_finance-1.0.2/polygon_finance/terminals/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:43:33.693891 polygon_finance-1.0.2/polygon_finance/terminals/crypto/
+-rw-rw-rw-   0        0        0        0 2023-05-14 16:42:17.000000 polygon_finance-1.0.2/polygon_finance/terminals/crypto/__init__.py
+-rw-rw-rw-   0        0        0     3637 2023-05-20 03:40:49.000000 polygon_finance-1.0.2/polygon_finance/terminals/crypto/crypto_terminal.py
+-rw-rw-rw-   0        0        0     1731 2023-05-14 16:53:24.000000 polygon_finance-1.0.2/polygon_finance/terminals/crypto/menu.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:43:33.623289 polygon_finance-1.0.2/polygon_finance.egg-info/
+-rw-rw-rw-   0        0        0      241 2023-05-20 03:43:33.000000 polygon_finance-1.0.2/polygon_finance.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4879 2023-05-20 03:43:33.000000 polygon_finance-1.0.2/polygon_finance.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 03:43:33.000000 polygon_finance-1.0.2/polygon_finance.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1253 2023-05-20 03:43:33.000000 polygon_finance-1.0.2/polygon_finance.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-20 03:43:33.000000 polygon_finance-1.0.2/polygon_finance.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-20 03:43:33.694891 polygon_finance-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     2577 2023-05-20 03:43:08.000000 polygon_finance-1.0.2/setup.py
```

### Comparing `polygon_finance-1.0.0/polygon_finance.egg-info/requires.txt` & `polygon_finance-1.0.2/polygon_finance.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.0/sdks/models/test_events.py` & `polygon_finance-1.0.2/polygon_finance/models/test_events.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.0/sdks/terminals/crypto/crypto_terminal.py` & `polygon_finance-1.0.2/polygon_finance/terminals/crypto/crypto_terminal.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 sys.path.append(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
 
 from terminals.crypto.menu import menu
 import asyncio
 from typing import List
 from polygon.websocket import WebSocketClient, WebSocketMessage, CryptoQuote, CryptoTrade, Market
-from sdks.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
+from polygon_finance.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
 from cachetools import TTLCache
 
 import threading
 import sqlite3
 from sqlite3 import Error
 
 from cfg import YOUR_API_KEY
```

### Comparing `polygon_finance-1.0.0/sdks/terminals/crypto/menu.py` & `polygon_finance-1.0.2/polygon_finance/terminals/crypto/menu.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.0/setup.py` & `polygon_finance-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='polygon_finance',
-    version='1.0.0',
+    version='1.0.2',
     description='The real-time market analysis library that utilizes the real-time rest apis and websockets from polygon.io',
     author='Charlies Vids',
     author_email='chuckdustin12@gmail.com',
     packages=find_packages(),
     install_requires=[
         'aiofiles==23.1.0',
         'aiohttp==3.8.4',
```

