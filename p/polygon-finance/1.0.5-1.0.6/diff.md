# Comparing `tmp/polygon_finance-1.0.5.tar.gz` & `tmp/polygon_finance-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polygon_finance-1.0.5.tar", last modified: Sat May 20 03:50:17 2023, max compression
+gzip compressed data, was "polygon_finance-1.0.6.tar", last modified: Sat May 20 03:57:38 2023, max compression
```

## Comparing `polygon_finance-1.0.5.tar` & `polygon_finance-1.0.6.tar`

### file list

```diff
@@ -1,176 +1,176 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 03:50:17.089422 polygon_finance-1.0.5/
--rw-rw-rw-   0        0        0      241 2023-05-20 03:50:17.089422 polygon_finance-1.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-20 03:50:16.959333 polygon_finance-1.0.5/polygon_finance/
--rw-rw-rw-   0        0        0        0 2023-05-14 16:45:53.000000 polygon_finance-1.0.5/polygon_finance/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-20 03:50:16.975334 polygon_finance-1.0.5/polygon_finance/discord/
--rw-rw-rw-   0        0        0        0 2023-05-20 03:05:54.000000 polygon_finance-1.0.5/polygon_finance/discord/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-20 03:50:16.976333 polygon_finance-1.0.5/polygon_finance/discord/conditions/
--rw-rw-rw-   0        0        0        0 2023-05-20 03:05:57.000000 polygon_finance-1.0.5/polygon_finance/discord/conditions/__init__.py
--rw-rw-rw-   0        0        0        0 2023-05-20 01:47:54.000000 polygon_finance-1.0.5/polygon_finance/discord/conditions/conditions.py
-drwxrwxrwx   0        0        0        0 2023-05-20 03:50:16.981333 polygon_finance-1.0.5/polygon_finance/discord/discord_utils/
--rw-rw-rw-   0        0        0        2 2023-05-14 06:35:12.000000 polygon_finance-1.0.5/polygon_finance/discord/discord_utils/__init__.py
--rw-rw-rw-   0        0        0    45761 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/discord/discord_utils/discord_stock_market.py
--rw-rw-rw-   0        0        0      569 2023-05-20 01:55:03.000000 polygon_finance-1.0.5/polygon_finance/discord/discord_utils/emojis.py
-drwxrwxrwx   0        0        0        0 2023-05-20 03:50:16.984335 polygon_finance-1.0.5/polygon_finance/discord/discord_utils/hooks/
--rw-rw-rw-   0        0        0        2 2023-05-14 01:56:34.000000 polygon_finance-1.0.5/polygon_finance/discord/discord_utils/hooks/__init__.py
--rw-rw-rw-   0        0        0     1633 2023-05-15 20:55:38.000000 polygon_finance-1.0.5/polygon_finance/discord/discord_utils/hooks/channel_webhooks.py
--rw-rw-rw-   0        0        0     5556 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/discord/discord_utils/hooks/send_webhook.py
--rw-rw-rw-   0        0        0       53 2023-05-20 01:09:02.000000 polygon_finance-1.0.5/polygon_finance/discord/discord_utils/hooks/test_webhooks.py
--rw-rw-rw-   0        0        0     7298 2023-05-14 01:56:34.000000 polygon_finance-1.0.5/polygon_finance/discord/discord_utils/hooks/webhook_info.py
--rw-rw-rw-   0        0        0    39052 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/discord/discord_utils/live_discord.py
--rw-rw-rw-   0        0        0     3927 2023-05-14 01:56:34.000000 polygon_finance-1.0.5/polygon_finance/discord/discord_utils/menus.py
-drwxrwxrwx   0        0        0        0 2023-05-20 03:50:16.985333 polygon_finance-1.0.5/polygon_finance/discord/discord_utils/selectmenus/
--rw-rw-rw-   0        0        0        2 2023-05-14 01:56:34.000000 polygon_finance-1.0.5/polygon_finance/discord/discord_utils/selectmenus/__init__.py
--rw-rw-rw-   0        0        0    36758 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/discord/discord_utils/selectmenus/mainselect.py
-drwxrwxrwx   0        0        0        0 2023-05-20 03:50:16.987333 polygon_finance-1.0.5/polygon_finance/discord/discord_utils/views/
--rw-rw-rw-   0        0        0        2 2023-05-14 01:56:34.000000 polygon_finance-1.0.5/polygon_finance/discord/discord_utils/views/__init__.py
--rw-rw-rw-   0        0        0     1707 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/discord/discord_utils/views/mainview.py
--rw-rw-rw-   0        0        0     6516 2023-05-20 02:30:22.000000 polygon_finance-1.0.5/polygon_finance/discord/discord_utils/webhook_creation.py
-drwxrwxrwx   0        0        0        0 2023-05-20 03:50:16.989333 polygon_finance-1.0.5/polygon_finance/discord/embeddings/
--rw-rw-rw-   0        0        0        0 2023-05-20 03:06:01.000000 polygon_finance-1.0.5/polygon_finance/discord/embeddings/__init__.py
--rw-rw-rw-   0        0        0      934 2023-05-14 01:56:34.000000 polygon_finance-1.0.5/polygon_finance/discord/embeddings/embeddings.py
--rw-rw-rw-   0        0        0    10106 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/discord/embeddings/embeds.py
--rw-rw-rw-   0        0        0     2887 2023-05-20 03:06:46.000000 polygon_finance-1.0.5/polygon_finance/discord/webhook_creation.py
-drwxrwxrwx   0        0        0        0 2023-05-20 03:50:16.990333 polygon_finance-1.0.5/polygon_finance/discord_examples/
--rw-rw-rw-   0        0        0        0 2023-05-20 03:04:36.000000 polygon_finance-1.0.5/polygon_finance/discord_examples/__init__.py
--rw-rw-rw-   0        0        0     3113 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/discord_examples/indices_spx_rsi.py
-drwxrwxrwx   0        0        0        0 2023-05-20 03:50:17.006332 polygon_finance-1.0.5/polygon_finance/examples/
--rw-rw-rw-   0        0        0        0 2023-05-20 03:04:40.000000 polygon_finance-1.0.5/polygon_finance/examples/__init__.py
--rw-rw-rw-   0        0        0     6418 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/examples/all_attributes.py
--rw-rw-rw-   0        0        0      549 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/examples/bollinger_bands.py
--rw-rw-rw-   0        0        0      746 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/examples/create_option_symbol.py
--rw-rw-rw-   0        0        0     1732 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/examples/ema.py
--rw-rw-rw-   0        0        0      976 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/examples/fetch_entire_chain.py
-drwxrwxrwx   0        0        0        0 2023-05-20 03:50:17.032336 polygon_finance-1.0.5/polygon_finance/examples/functions/
--rw-rw-rw-   0        0        0        0 2023-05-20 03:04:44.000000 polygon_finance-1.0.5/polygon_finance/examples/functions/__init__.py
--rw-rw-rw-   0        0        0     6418 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/examples/functions/all_attributes.py
--rw-rw-rw-   0        0        0      549 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/examples/functions/bollinger_bands.py
--rw-rw-rw-   0        0        0      746 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/examples/functions/create_option_symbol.py
--rw-rw-rw-   0        0        0     1732 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/examples/functions/ema.py
--rw-rw-rw-   0        0        0      976 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/examples/functions/fetch_entire_chain.py
--rw-rw-rw-   0        0        0      687 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/examples/functions/find_gaps.py
--rw-rw-rw-   0        0        0      863 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/examples/functions/get_all_options_data.py
--rw-rw-rw-   0        0        0     2511 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/examples/functions/get_ema.py
--rw-rw-rw-   0        0        0      633 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/examples/functions/get_latest_crypto_data.py
--rw-rw-rw-   0        0        0      620 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/examples/functions/get_latest_forex_data.py
--rw-rw-rw-   0        0        0      476 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/examples/functions/get_latest_indices_data.py
--rw-rw-rw-   0        0        0     3291 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/examples/functions/get_macd.py
--rw-rw-rw-   0        0        0      617 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/examples/functions/get_pivot_points.py
--rw-rw-rw-   0        0        0     2161 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/examples/functions/get_rsi.py
--rw-rw-rw-   0        0        0     2285 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/examples/functions/get_sma.py
--rw-rw-rw-   0        0        0     1807 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/examples/functions/latest_news.py
--rw-rw-rw-   0        0        0     1695 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/examples/functions/option_quote.py
--rw-rw-rw-   0        0        0     2496 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/examples/functions/option_trades.py
--rw-rw-rw-   0        0        0     1471 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/examples/functions/plot_aggs.py
--rw-rw-rw-   0        0        0      848 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/examples/functions/plot_macd.py
--rw-rw-rw-   0        0        0     1870 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/examples/functions/plot_option_aggs.py
--rw-rw-rw-   0        0        0      517 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/examples/functions/rate_of_change.py
--rw-rw-rw-   0        0        0     5038 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/examples/functions/scanner_example.py
--rw-rw-rw-   0        0        0     2191 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/examples/functions/stock_aggregates.py
--rw-rw-rw-   0        0        0     5359 2023-05-14 01:56:34.000000 polygon_finance-1.0.5/polygon_finance/examples/functions/summarizer.py
--rw-rw-rw-   0        0        0     1237 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/examples/functions/support_resistance.py
--rw-rw-rw-   0        0        0      863 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/examples/get_all_options_data.py
--rw-rw-rw-   0        0        0      633 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/examples/get_latest_crypto_data.py
--rw-rw-rw-   0        0        0      620 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/examples/get_latest_forex_data.py
--rw-rw-rw-   0        0        0      476 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/examples/get_latest_indices_data.py
--rw-rw-rw-   0        0        0      681 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/examples/get_latest_ticker_data.py
--rw-rw-rw-   0        0        0      617 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/examples/get_pivot_points.py
--rw-rw-rw-   0        0        0     1863 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/examples/latest_news.py
--rw-rw-rw-   0        0        0     1695 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/examples/option_quote.py
--rw-rw-rw-   0        0        0     2496 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/examples/option_trades.py
--rw-rw-rw-   0        0        0     1471 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/examples/plot_aggs.py
--rw-rw-rw-   0        0        0      848 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/examples/plot_macd.py
--rw-rw-rw-   0        0        0     1870 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/examples/plot_option_aggs.py
--rw-rw-rw-   0        0        0      517 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/examples/rate_of_change.py
-drwxrwxrwx   0        0        0        0 2023-05-20 03:50:17.038337 polygon_finance-1.0.5/polygon_finance/examples/realtime_markets/
--rw-rw-rw-   0        0        0        0 2023-05-20 03:04:48.000000 polygon_finance-1.0.5/polygon_finance/examples/realtime_markets/__init__.py
--rw-rw-rw-   0        0        0     2586 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/examples/realtime_markets/crypto_market.py
--rw-rw-rw-   0        0        0      993 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/examples/realtime_markets/forex_market.py
--rw-rw-rw-   0        0        0      833 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/examples/realtime_markets/indices_market.py
--rw-rw-rw-   0        0        0     1037 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/examples/realtime_markets/options_market.py
--rw-rw-rw-   0        0        0     9392 2023-05-20 03:42:20.000000 polygon_finance-1.0.5/polygon_finance/examples/realtime_markets/stock_market.py
-drwxrwxrwx   0        0        0        0 2023-05-20 03:50:17.043337 polygon_finance-1.0.5/polygon_finance/examples/simulated_markets/
--rw-rw-rw-   0        0        0        0 2023-05-20 03:04:53.000000 polygon_finance-1.0.5/polygon_finance/examples/simulated_markets/__init__.py
--rw-rw-rw-   0        0        0      707 2023-05-15 07:34:31.000000 polygon_finance-1.0.5/polygon_finance/examples/simulated_markets/helpers.py
--rw-rw-rw-   0        0        0     5054 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/examples/simulated_markets/mock_discord.py
--rw-rw-rw-   0        0        0     2061 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/examples/simulated_markets/mock_market.py
--rw-rw-rw-   0        0        0     1891 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/examples/simulated_markets/mock_options_market.py
--rw-rw-rw-   0        0        0     2191 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/examples/stock_aggregates.py
--rw-rw-rw-   0        0        0     5359 2023-05-20 03:06:46.000000 polygon_finance-1.0.5/polygon_finance/examples/summarizer.py
--rw-rw-rw-   0        0        0     1237 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/examples/support_resistance.py
--rw-rw-rw-   0        0        0      681 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/get_latest_ticker_data.py
-drwxrwxrwx   0        0        0        0 2023-05-20 03:50:17.045337 polygon_finance-1.0.5/polygon_finance/models/
--rw-rw-rw-   0        0        0        2 2023-05-14 01:56:34.000000 polygon_finance-1.0.5/polygon_finance/models/__init__.py
--rw-rw-rw-   0        0        0      511 2023-05-14 01:56:34.000000 polygon_finance-1.0.5/polygon_finance/models/common.py
--rw-rw-rw-   0        0        0    13169 2023-05-20 01:07:08.000000 polygon_finance-1.0.5/polygon_finance/models/test_events.py
-drwxrwxrwx   0        0        0        0 2023-05-20 03:50:17.046337 polygon_finance-1.0.5/polygon_finance/read-me/
--rw-rw-rw-   0        0        0        8 2023-05-20 03:38:24.000000 polygon_finance-1.0.5/polygon_finance/read-me/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-20 03:50:17.046337 polygon_finance-1.0.5/polygon_finance/sdks/
--rw-rw-rw-   0        0        0        0 2023-05-20 03:46:41.000000 polygon_finance-1.0.5/polygon_finance/sdks/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-20 03:50:17.049422 polygon_finance-1.0.5/polygon_finance/sdks/discord_sdk/
--rw-rw-rw-   0        0        0        0 2023-05-20 03:48:57.000000 polygon_finance-1.0.5/polygon_finance/sdks/discord_sdk/__init__.py
--rw-rw-rw-   0        0        0       56 2023-05-18 01:25:22.000000 polygon_finance-1.0.5/polygon_finance/sdks/discord_sdk/channel_ids.py
--rw-rw-rw-   0        0        0     4625 2023-05-18 01:47:34.000000 polygon_finance-1.0.5/polygon_finance/sdks/discord_sdk/discord_sdk.py
--rw-rw-rw-   0        0        0     2206 2023-05-17 01:43:41.000000 polygon_finance-1.0.5/polygon_finance/sdks/discord_sdk/searching.py
-drwxrwxrwx   0        0        0        0 2023-05-20 03:50:17.051423 polygon_finance-1.0.5/polygon_finance/sdks/fudstop_sdk/
--rw-rw-rw-   0        0        0        0 2023-05-20 03:46:50.000000 polygon_finance-1.0.5/polygon_finance/sdks/fudstop_sdk/__init__.py
--rw-rw-rw-   0        0        0     2984 2023-05-14 20:38:44.000000 polygon_finance-1.0.5/polygon_finance/sdks/fudstop_sdk/fudstop_sdk.py
--rw-rw-rw-   0        0        0     1714 2023-05-14 01:56:34.000000 polygon_finance-1.0.5/polygon_finance/sdks/fudstop_sdk/gaps.py
--rw-rw-rw-   0        0        0      435 2023-05-14 01:56:34.000000 polygon_finance-1.0.5/polygon_finance/sdks/fudstop_sdk/option_vol_totals.py
-drwxrwxrwx   0        0        0        0 2023-05-20 03:50:17.068422 polygon_finance-1.0.5/polygon_finance/sdks/polygon_sdk/
--rw-rw-rw-   0        0        0        0 2023-05-20 03:48:48.000000 polygon_finance-1.0.5/polygon_finance/sdks/polygon_sdk/__init__.py
--rw-rw-rw-   0        0        0     1297 2023-05-14 01:56:34.000000 polygon_finance-1.0.5/polygon_finance/sdks/polygon_sdk/aggregates.py
--rw-rw-rw-   0        0        0    29904 2023-05-19 03:39:12.000000 polygon_finance-1.0.5/polygon_finance/sdks/polygon_sdk/async_options_sdk.py
--rw-rw-rw-   0        0        0    52505 2023-05-20 01:22:58.000000 polygon_finance-1.0.5/polygon_finance/sdks/polygon_sdk/async_polygon_sdk.py
--rw-rw-rw-   0        0        0      723 2023-05-14 01:56:34.000000 polygon_finance-1.0.5/polygon_finance/sdks/polygon_sdk/daily_open_close.py
--rw-rw-rw-   0        0        0    15262 2023-05-07 17:43:52.000000 polygon_finance-1.0.5/polygon_finance/sdks/polygon_sdk/financials.py
--rw-rw-rw-   0        0        0     6771 2023-05-14 23:53:31.000000 polygon_finance-1.0.5/polygon_finance/sdks/polygon_sdk/forex_crypto.py
--rw-rw-rw-   0        0        0     9148 2023-05-19 00:35:23.000000 polygon_finance-1.0.5/polygon_finance/sdks/polygon_sdk/get_all_options.py
--rw-rw-rw-   0        0        0     1154 2023-05-14 03:56:48.000000 polygon_finance-1.0.5/polygon_finance/sdks/polygon_sdk/indices_snapshot.py
--rw-rw-rw-   0        0        0      858 2023-05-14 01:56:34.000000 polygon_finance-1.0.5/polygon_finance/sdks/polygon_sdk/logo.py
--rw-rw-rw-   0        0        0    28260 2023-05-19 20:12:16.000000 polygon_finance-1.0.5/polygon_finance/sdks/polygon_sdk/mapping_dicts.py
--rw-rw-rw-   0        0        0      819 2023-05-14 01:56:34.000000 polygon_finance-1.0.5/polygon_finance/sdks/polygon_sdk/models.py
--rw-rw-rw-   0        0        0      836 2023-05-14 01:56:34.000000 polygon_finance-1.0.5/polygon_finance/sdks/polygon_sdk/news.py
--rw-rw-rw-   0        0        0      842 2023-05-14 01:56:34.000000 polygon_finance-1.0.5/polygon_finance/sdks/polygon_sdk/option_aggs.py
--rw-rw-rw-   0        0        0     1523 2023-05-15 20:01:03.000000 polygon_finance-1.0.5/polygon_finance/sdks/polygon_sdk/option_quote.py
--rw-rw-rw-   0        0        0     3144 2023-05-15 06:27:25.000000 polygon_finance-1.0.5/polygon_finance/sdks/polygon_sdk/option_snapshot.py
--rw-rw-rw-   0        0        0      891 2023-05-15 20:00:58.000000 polygon_finance-1.0.5/polygon_finance/sdks/polygon_sdk/option_trades.py
--rw-rw-rw-   0        0        0      556 2023-05-14 01:56:34.000000 polygon_finance-1.0.5/polygon_finance/sdks/polygon_sdk/pivot_points.py
--rw-rw-rw-   0        0        0      710 2023-05-14 01:56:34.000000 polygon_finance-1.0.5/polygon_finance/sdks/polygon_sdk/quote.py
--rw-rw-rw-   0        0        0     4347 2023-05-14 04:32:38.000000 polygon_finance-1.0.5/polygon_finance/sdks/polygon_sdk/snapshot.py
--rw-rw-rw-   0        0        0     1370 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/sdks/polygon_sdk/technical_conditions.py
--rw-rw-rw-   0        0        0     3437 2023-05-14 20:38:44.000000 polygon_finance-1.0.5/polygon_finance/sdks/polygon_sdk/tickernews.py
-drwxrwxrwx   0        0        0        0 2023-05-20 03:50:17.085421 polygon_finance-1.0.5/polygon_finance/sdks/webull_sdk/
--rw-rw-rw-   0        0        0        2 2023-05-14 01:56:34.000000 polygon_finance-1.0.5/polygon_finance/sdks/webull_sdk/__init__.py
--rw-rw-rw-   0        0        0      882 2023-05-14 01:56:34.000000 polygon_finance-1.0.5/polygon_finance/sdks/webull_sdk/calendar.py
--rw-rw-rw-   0        0        0     8295 2023-05-15 04:33:49.000000 polygon_finance-1.0.5/polygon_finance/sdks/webull_sdk/capitalflow.py
--rw-rw-rw-   0        0        0     1174 2023-05-14 01:56:34.000000 polygon_finance-1.0.5/polygon_finance/sdks/webull_sdk/cost_distribution.py
--rw-rw-rw-   0        0        0     2325 2023-05-14 01:56:34.000000 polygon_finance-1.0.5/polygon_finance/sdks/webull_sdk/derivative_query.py
--rw-rw-rw-   0        0        0     2426 2023-05-14 01:56:34.000000 polygon_finance-1.0.5/polygon_finance/sdks/webull_sdk/etf_finder.py
--rw-rw-rw-   0        0        0      500 2023-05-14 01:56:34.000000 polygon_finance-1.0.5/polygon_finance/sdks/webull_sdk/etf_holdings.py
--rw-rw-rw-   0        0        0     1025 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/sdks/webull_sdk/events.py
--rw-rw-rw-   0        0        0     7818 2023-05-14 01:56:34.000000 polygon_finance-1.0.5/polygon_finance/sdks/webull_sdk/financial_statement.py
--rw-rw-rw-   0        0        0     3871 2023-05-14 01:56:34.000000 polygon_finance-1.0.5/polygon_finance/sdks/webull_sdk/forecast.py
--rw-rw-rw-   0        0        0     1033 2023-05-14 01:56:34.000000 polygon_finance-1.0.5/polygon_finance/sdks/webull_sdk/institutional_holdings.py
--rw-rw-rw-   0        0        0     1156 2023-05-14 01:56:34.000000 polygon_finance-1.0.5/polygon_finance/sdks/webull_sdk/manage.py
--rw-rw-rw-   0        0        0      617 2023-05-14 01:56:34.000000 polygon_finance-1.0.5/polygon_finance/sdks/webull_sdk/news.py
--rw-rw-rw-   0        0        0      307 2023-05-14 01:56:34.000000 polygon_finance-1.0.5/polygon_finance/sdks/webull_sdk/shortinterest.py
--rw-rw-rw-   0        0        0     2768 2023-05-15 04:24:58.000000 polygon_finance-1.0.5/polygon_finance/sdks/webull_sdk/top_gainers.py
--rw-rw-rw-   0        0        0    16723 2023-05-14 01:56:34.000000 polygon_finance-1.0.5/polygon_finance/sdks/webull_sdk/top_options.py
--rw-rw-rw-   0        0        0     5556 2023-05-14 01:56:34.000000 polygon_finance-1.0.5/polygon_finance/sdks/webull_sdk/webull_data.py
--rw-rw-rw-   0        0        0    43244 2023-05-15 04:26:38.000000 polygon_finance-1.0.5/polygon_finance/sdks/webull_sdk/webull_sdk.py
--rw-rw-rw-   0        0        0     1113 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/start_here.py
-drwxrwxrwx   0        0        0        0 2023-05-20 03:50:17.085421 polygon_finance-1.0.5/polygon_finance/terminals/
--rw-rw-rw-   0        0        0        0 2023-05-14 16:41:17.000000 polygon_finance-1.0.5/polygon_finance/terminals/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-20 03:50:17.088422 polygon_finance-1.0.5/polygon_finance/terminals/crypto/
--rw-rw-rw-   0        0        0        0 2023-05-14 16:42:17.000000 polygon_finance-1.0.5/polygon_finance/terminals/crypto/__init__.py
--rw-rw-rw-   0        0        0     3637 2023-05-20 03:40:49.000000 polygon_finance-1.0.5/polygon_finance/terminals/crypto/crypto_terminal.py
--rw-rw-rw-   0        0        0     1731 2023-05-14 16:53:24.000000 polygon_finance-1.0.5/polygon_finance/terminals/crypto/menu.py
-drwxrwxrwx   0        0        0        0 2023-05-20 03:50:16.973333 polygon_finance-1.0.5/polygon_finance.egg-info/
--rw-rw-rw-   0        0        0      241 2023-05-20 03:50:16.000000 polygon_finance-1.0.5/polygon_finance.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7242 2023-05-20 03:50:16.000000 polygon_finance-1.0.5/polygon_finance.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 03:50:16.000000 polygon_finance-1.0.5/polygon_finance.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1253 2023-05-20 03:50:16.000000 polygon_finance-1.0.5/polygon_finance.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-20 03:50:16.000000 polygon_finance-1.0.5/polygon_finance.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-20 03:50:17.090423 polygon_finance-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     2577 2023-05-20 03:49:41.000000 polygon_finance-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:57:38.107189 polygon_finance-1.0.6/
+-rw-rw-rw-   0        0        0      241 2023-05-20 03:57:38.106189 polygon_finance-1.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-20 03:57:37.937626 polygon_finance-1.0.6/polygon_finance/
+-rw-rw-rw-   0        0        0        0 2023-05-14 16:45:53.000000 polygon_finance-1.0.6/polygon_finance/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:57:37.948628 polygon_finance-1.0.6/polygon_finance/discord/
+-rw-rw-rw-   0        0        0        0 2023-05-20 03:05:54.000000 polygon_finance-1.0.6/polygon_finance/discord/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:57:37.950629 polygon_finance-1.0.6/polygon_finance/discord/conditions/
+-rw-rw-rw-   0        0        0        0 2023-05-20 03:05:57.000000 polygon_finance-1.0.6/polygon_finance/discord/conditions/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-20 01:47:54.000000 polygon_finance-1.0.6/polygon_finance/discord/conditions/conditions.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:57:37.955628 polygon_finance-1.0.6/polygon_finance/discord/discord_utils/
+-rw-rw-rw-   0        0        0        2 2023-05-14 06:35:12.000000 polygon_finance-1.0.6/polygon_finance/discord/discord_utils/__init__.py
+-rw-rw-rw-   0        0        0    45781 2023-05-20 03:53:25.000000 polygon_finance-1.0.6/polygon_finance/discord/discord_utils/discord_stock_market.py
+-rw-rw-rw-   0        0        0      569 2023-05-20 01:55:03.000000 polygon_finance-1.0.6/polygon_finance/discord/discord_utils/emojis.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:57:37.959628 polygon_finance-1.0.6/polygon_finance/discord/discord_utils/hooks/
+-rw-rw-rw-   0        0        0        2 2023-05-14 01:56:34.000000 polygon_finance-1.0.6/polygon_finance/discord/discord_utils/hooks/__init__.py
+-rw-rw-rw-   0        0        0     1633 2023-05-15 20:55:38.000000 polygon_finance-1.0.6/polygon_finance/discord/discord_utils/hooks/channel_webhooks.py
+-rw-rw-rw-   0        0        0     5561 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/discord/discord_utils/hooks/send_webhook.py
+-rw-rw-rw-   0        0        0       53 2023-05-20 01:09:02.000000 polygon_finance-1.0.6/polygon_finance/discord/discord_utils/hooks/test_webhooks.py
+-rw-rw-rw-   0        0        0     7298 2023-05-14 01:56:34.000000 polygon_finance-1.0.6/polygon_finance/discord/discord_utils/hooks/webhook_info.py
+-rw-rw-rw-   0        0        0    39072 2023-05-20 03:53:34.000000 polygon_finance-1.0.6/polygon_finance/discord/discord_utils/live_discord.py
+-rw-rw-rw-   0        0        0     3927 2023-05-14 01:56:34.000000 polygon_finance-1.0.6/polygon_finance/discord/discord_utils/menus.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:57:37.968136 polygon_finance-1.0.6/polygon_finance/discord/discord_utils/selectmenus/
+-rw-rw-rw-   0        0        0        2 2023-05-14 01:56:34.000000 polygon_finance-1.0.6/polygon_finance/discord/discord_utils/selectmenus/__init__.py
+-rw-rw-rw-   0        0        0    36796 2023-05-20 03:54:12.000000 polygon_finance-1.0.6/polygon_finance/discord/discord_utils/selectmenus/mainselect.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:57:37.970137 polygon_finance-1.0.6/polygon_finance/discord/discord_utils/views/
+-rw-rw-rw-   0        0        0        2 2023-05-14 01:56:34.000000 polygon_finance-1.0.6/polygon_finance/discord/discord_utils/views/__init__.py
+-rw-rw-rw-   0        0        0     1712 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/discord/discord_utils/views/mainview.py
+-rw-rw-rw-   0        0        0     6516 2023-05-20 02:30:22.000000 polygon_finance-1.0.6/polygon_finance/discord/discord_utils/webhook_creation.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:57:37.973137 polygon_finance-1.0.6/polygon_finance/discord/embeddings/
+-rw-rw-rw-   0        0        0        0 2023-05-20 03:06:01.000000 polygon_finance-1.0.6/polygon_finance/discord/embeddings/__init__.py
+-rw-rw-rw-   0        0        0      934 2023-05-14 01:56:34.000000 polygon_finance-1.0.6/polygon_finance/discord/embeddings/embeddings.py
+-rw-rw-rw-   0        0        0    10121 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/discord/embeddings/embeds.py
+-rw-rw-rw-   0        0        0     2887 2023-05-20 03:06:46.000000 polygon_finance-1.0.6/polygon_finance/discord/webhook_creation.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:57:37.976137 polygon_finance-1.0.6/polygon_finance/discord_examples/
+-rw-rw-rw-   0        0        0        0 2023-05-20 03:04:36.000000 polygon_finance-1.0.6/polygon_finance/discord_examples/__init__.py
+-rw-rw-rw-   0        0        0     3102 2023-05-20 03:53:03.000000 polygon_finance-1.0.6/polygon_finance/discord_examples/indices_spx_rsi.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:57:38.006137 polygon_finance-1.0.6/polygon_finance/examples/
+-rw-rw-rw-   0        0        0        0 2023-05-20 03:04:40.000000 polygon_finance-1.0.6/polygon_finance/examples/__init__.py
+-rw-rw-rw-   0        0        0     6433 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/examples/all_attributes.py
+-rw-rw-rw-   0        0        0      554 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/examples/bollinger_bands.py
+-rw-rw-rw-   0        0        0      751 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/examples/create_option_symbol.py
+-rw-rw-rw-   0        0        0     1737 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/examples/ema.py
+-rw-rw-rw-   0        0        0      986 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/examples/fetch_entire_chain.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:57:38.033136 polygon_finance-1.0.6/polygon_finance/examples/functions/
+-rw-rw-rw-   0        0        0        0 2023-05-20 03:04:44.000000 polygon_finance-1.0.6/polygon_finance/examples/functions/__init__.py
+-rw-rw-rw-   0        0        0     6433 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/examples/functions/all_attributes.py
+-rw-rw-rw-   0        0        0      554 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/examples/functions/bollinger_bands.py
+-rw-rw-rw-   0        0        0      751 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/examples/functions/create_option_symbol.py
+-rw-rw-rw-   0        0        0     1737 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/examples/functions/ema.py
+-rw-rw-rw-   0        0        0      986 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/examples/functions/fetch_entire_chain.py
+-rw-rw-rw-   0        0        0      692 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/examples/functions/find_gaps.py
+-rw-rw-rw-   0        0        0      868 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/examples/functions/get_all_options_data.py
+-rw-rw-rw-   0        0        0     2521 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/examples/functions/get_ema.py
+-rw-rw-rw-   0        0        0      638 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/examples/functions/get_latest_crypto_data.py
+-rw-rw-rw-   0        0        0      625 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/examples/functions/get_latest_forex_data.py
+-rw-rw-rw-   0        0        0      481 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/examples/functions/get_latest_indices_data.py
+-rw-rw-rw-   0        0        0     3301 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/examples/functions/get_macd.py
+-rw-rw-rw-   0        0        0      622 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/examples/functions/get_pivot_points.py
+-rw-rw-rw-   0        0        0     2171 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/examples/functions/get_rsi.py
+-rw-rw-rw-   0        0        0     2295 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/examples/functions/get_sma.py
+-rw-rw-rw-   0        0        0     1812 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/examples/functions/latest_news.py
+-rw-rw-rw-   0        0        0     1700 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/examples/functions/option_quote.py
+-rw-rw-rw-   0        0        0     2506 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/examples/functions/option_trades.py
+-rw-rw-rw-   0        0        0     1476 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/examples/functions/plot_aggs.py
+-rw-rw-rw-   0        0        0      853 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/examples/functions/plot_macd.py
+-rw-rw-rw-   0        0        0     1875 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/examples/functions/plot_option_aggs.py
+-rw-rw-rw-   0        0        0      522 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/examples/functions/rate_of_change.py
+-rw-rw-rw-   0        0        0     5043 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/examples/functions/scanner_example.py
+-rw-rw-rw-   0        0        0     2196 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/examples/functions/stock_aggregates.py
+-rw-rw-rw-   0        0        0     5359 2023-05-14 01:56:34.000000 polygon_finance-1.0.6/polygon_finance/examples/functions/summarizer.py
+-rw-rw-rw-   0        0        0     1242 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/examples/functions/support_resistance.py
+-rw-rw-rw-   0        0        0      868 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/examples/get_all_options_data.py
+-rw-rw-rw-   0        0        0      638 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/examples/get_latest_crypto_data.py
+-rw-rw-rw-   0        0        0      625 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/examples/get_latest_forex_data.py
+-rw-rw-rw-   0        0        0      481 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/examples/get_latest_indices_data.py
+-rw-rw-rw-   0        0        0      686 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/examples/get_latest_ticker_data.py
+-rw-rw-rw-   0        0        0      622 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/examples/get_pivot_points.py
+-rw-rw-rw-   0        0        0     1868 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/examples/latest_news.py
+-rw-rw-rw-   0        0        0     1700 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/examples/option_quote.py
+-rw-rw-rw-   0        0        0     2506 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/examples/option_trades.py
+-rw-rw-rw-   0        0        0     1476 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/examples/plot_aggs.py
+-rw-rw-rw-   0        0        0      853 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/examples/plot_macd.py
+-rw-rw-rw-   0        0        0     1875 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/examples/plot_option_aggs.py
+-rw-rw-rw-   0        0        0      522 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/examples/rate_of_change.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:57:38.045136 polygon_finance-1.0.6/polygon_finance/examples/realtime_markets/
+-rw-rw-rw-   0        0        0        0 2023-05-20 03:04:48.000000 polygon_finance-1.0.6/polygon_finance/examples/realtime_markets/__init__.py
+-rw-rw-rw-   0        0        0     2591 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/examples/realtime_markets/crypto_market.py
+-rw-rw-rw-   0        0        0      998 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/examples/realtime_markets/forex_market.py
+-rw-rw-rw-   0        0        0      838 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/examples/realtime_markets/indices_market.py
+-rw-rw-rw-   0        0        0     1042 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/examples/realtime_markets/options_market.py
+-rw-rw-rw-   0        0        0     9402 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/examples/realtime_markets/stock_market.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:57:38.050143 polygon_finance-1.0.6/polygon_finance/examples/simulated_markets/
+-rw-rw-rw-   0        0        0        0 2023-05-20 03:04:53.000000 polygon_finance-1.0.6/polygon_finance/examples/simulated_markets/__init__.py
+-rw-rw-rw-   0        0        0      707 2023-05-15 07:34:31.000000 polygon_finance-1.0.6/polygon_finance/examples/simulated_markets/helpers.py
+-rw-rw-rw-   0        0        0     5064 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/examples/simulated_markets/mock_discord.py
+-rw-rw-rw-   0        0        0     2066 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/examples/simulated_markets/mock_market.py
+-rw-rw-rw-   0        0        0     1896 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/examples/simulated_markets/mock_options_market.py
+-rw-rw-rw-   0        0        0     2196 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/examples/stock_aggregates.py
+-rw-rw-rw-   0        0        0     5359 2023-05-20 03:06:46.000000 polygon_finance-1.0.6/polygon_finance/examples/summarizer.py
+-rw-rw-rw-   0        0        0     1242 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/examples/support_resistance.py
+-rw-rw-rw-   0        0        0      686 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/get_latest_ticker_data.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:57:38.052142 polygon_finance-1.0.6/polygon_finance/models/
+-rw-rw-rw-   0        0        0        2 2023-05-14 01:56:34.000000 polygon_finance-1.0.6/polygon_finance/models/__init__.py
+-rw-rw-rw-   0        0        0      511 2023-05-14 01:56:34.000000 polygon_finance-1.0.6/polygon_finance/models/common.py
+-rw-rw-rw-   0        0        0    13169 2023-05-20 01:07:08.000000 polygon_finance-1.0.6/polygon_finance/models/test_events.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:57:38.053142 polygon_finance-1.0.6/polygon_finance/read-me/
+-rw-rw-rw-   0        0        0        0 2023-05-20 03:53:10.000000 polygon_finance-1.0.6/polygon_finance/read-me/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:57:38.053142 polygon_finance-1.0.6/polygon_finance/sdks/
+-rw-rw-rw-   0        0        0        0 2023-05-20 03:46:41.000000 polygon_finance-1.0.6/polygon_finance/sdks/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:57:38.057141 polygon_finance-1.0.6/polygon_finance/sdks/discord_sdk/
+-rw-rw-rw-   0        0        0        0 2023-05-20 03:48:57.000000 polygon_finance-1.0.6/polygon_finance/sdks/discord_sdk/__init__.py
+-rw-rw-rw-   0        0        0       56 2023-05-18 01:25:22.000000 polygon_finance-1.0.6/polygon_finance/sdks/discord_sdk/channel_ids.py
+-rw-rw-rw-   0        0        0     4625 2023-05-18 01:47:34.000000 polygon_finance-1.0.6/polygon_finance/sdks/discord_sdk/discord_sdk.py
+-rw-rw-rw-   0        0        0     2206 2023-05-17 01:43:41.000000 polygon_finance-1.0.6/polygon_finance/sdks/discord_sdk/searching.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:57:38.060142 polygon_finance-1.0.6/polygon_finance/sdks/fudstop_sdk/
+-rw-rw-rw-   0        0        0        0 2023-05-20 03:46:50.000000 polygon_finance-1.0.6/polygon_finance/sdks/fudstop_sdk/__init__.py
+-rw-rw-rw-   0        0        0     2984 2023-05-14 20:38:44.000000 polygon_finance-1.0.6/polygon_finance/sdks/fudstop_sdk/fudstop_sdk.py
+-rw-rw-rw-   0        0        0     1714 2023-05-14 01:56:34.000000 polygon_finance-1.0.6/polygon_finance/sdks/fudstop_sdk/gaps.py
+-rw-rw-rw-   0        0        0      435 2023-05-14 01:56:34.000000 polygon_finance-1.0.6/polygon_finance/sdks/fudstop_sdk/option_vol_totals.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:57:38.084189 polygon_finance-1.0.6/polygon_finance/sdks/polygon_sdk/
+-rw-rw-rw-   0        0        0        0 2023-05-20 03:57:11.000000 polygon_finance-1.0.6/polygon_finance/sdks/polygon_sdk/__init__.py
+-rw-rw-rw-   0        0        0     1297 2023-05-14 01:56:34.000000 polygon_finance-1.0.6/polygon_finance/sdks/polygon_sdk/aggregates.py
+-rw-rw-rw-   0        0        0    29904 2023-05-19 03:39:12.000000 polygon_finance-1.0.6/polygon_finance/sdks/polygon_sdk/async_options_sdk.py
+-rw-rw-rw-   0        0        0    52505 2023-05-20 01:22:58.000000 polygon_finance-1.0.6/polygon_finance/sdks/polygon_sdk/async_polygon_sdk.py
+-rw-rw-rw-   0        0        0      723 2023-05-14 01:56:34.000000 polygon_finance-1.0.6/polygon_finance/sdks/polygon_sdk/daily_open_close.py
+-rw-rw-rw-   0        0        0    15262 2023-05-07 17:43:52.000000 polygon_finance-1.0.6/polygon_finance/sdks/polygon_sdk/financials.py
+-rw-rw-rw-   0        0        0     6771 2023-05-14 23:53:31.000000 polygon_finance-1.0.6/polygon_finance/sdks/polygon_sdk/forex_crypto.py
+-rw-rw-rw-   0        0        0     9148 2023-05-19 00:35:23.000000 polygon_finance-1.0.6/polygon_finance/sdks/polygon_sdk/get_all_options.py
+-rw-rw-rw-   0        0        0     1154 2023-05-14 03:56:48.000000 polygon_finance-1.0.6/polygon_finance/sdks/polygon_sdk/indices_snapshot.py
+-rw-rw-rw-   0        0        0      858 2023-05-14 01:56:34.000000 polygon_finance-1.0.6/polygon_finance/sdks/polygon_sdk/logo.py
+-rw-rw-rw-   0        0        0    28260 2023-05-19 20:12:16.000000 polygon_finance-1.0.6/polygon_finance/sdks/polygon_sdk/mapping_dicts.py
+-rw-rw-rw-   0        0        0      819 2023-05-14 01:56:34.000000 polygon_finance-1.0.6/polygon_finance/sdks/polygon_sdk/models.py
+-rw-rw-rw-   0        0        0      836 2023-05-14 01:56:34.000000 polygon_finance-1.0.6/polygon_finance/sdks/polygon_sdk/news.py
+-rw-rw-rw-   0        0        0      842 2023-05-14 01:56:34.000000 polygon_finance-1.0.6/polygon_finance/sdks/polygon_sdk/option_aggs.py
+-rw-rw-rw-   0        0        0     1523 2023-05-15 20:01:03.000000 polygon_finance-1.0.6/polygon_finance/sdks/polygon_sdk/option_quote.py
+-rw-rw-rw-   0        0        0     3144 2023-05-15 06:27:25.000000 polygon_finance-1.0.6/polygon_finance/sdks/polygon_sdk/option_snapshot.py
+-rw-rw-rw-   0        0        0      891 2023-05-15 20:00:58.000000 polygon_finance-1.0.6/polygon_finance/sdks/polygon_sdk/option_trades.py
+-rw-rw-rw-   0        0        0      556 2023-05-14 01:56:34.000000 polygon_finance-1.0.6/polygon_finance/sdks/polygon_sdk/pivot_points.py
+-rw-rw-rw-   0        0        0      710 2023-05-14 01:56:34.000000 polygon_finance-1.0.6/polygon_finance/sdks/polygon_sdk/quote.py
+-rw-rw-rw-   0        0        0     4347 2023-05-14 04:32:38.000000 polygon_finance-1.0.6/polygon_finance/sdks/polygon_sdk/snapshot.py
+-rw-rw-rw-   0        0        0     1375 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/sdks/polygon_sdk/technical_conditions.py
+-rw-rw-rw-   0        0        0     3437 2023-05-14 20:38:44.000000 polygon_finance-1.0.6/polygon_finance/sdks/polygon_sdk/tickernews.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:57:38.101190 polygon_finance-1.0.6/polygon_finance/sdks/webull_sdk/
+-rw-rw-rw-   0        0        0        2 2023-05-14 01:56:34.000000 polygon_finance-1.0.6/polygon_finance/sdks/webull_sdk/__init__.py
+-rw-rw-rw-   0        0        0      882 2023-05-14 01:56:34.000000 polygon_finance-1.0.6/polygon_finance/sdks/webull_sdk/calendar.py
+-rw-rw-rw-   0        0        0     8295 2023-05-15 04:33:49.000000 polygon_finance-1.0.6/polygon_finance/sdks/webull_sdk/capitalflow.py
+-rw-rw-rw-   0        0        0     1174 2023-05-14 01:56:34.000000 polygon_finance-1.0.6/polygon_finance/sdks/webull_sdk/cost_distribution.py
+-rw-rw-rw-   0        0        0     2325 2023-05-14 01:56:34.000000 polygon_finance-1.0.6/polygon_finance/sdks/webull_sdk/derivative_query.py
+-rw-rw-rw-   0        0        0     2426 2023-05-14 01:56:34.000000 polygon_finance-1.0.6/polygon_finance/sdks/webull_sdk/etf_finder.py
+-rw-rw-rw-   0        0        0      500 2023-05-14 01:56:34.000000 polygon_finance-1.0.6/polygon_finance/sdks/webull_sdk/etf_holdings.py
+-rw-rw-rw-   0        0        0     1025 2023-05-20 03:40:49.000000 polygon_finance-1.0.6/polygon_finance/sdks/webull_sdk/events.py
+-rw-rw-rw-   0        0        0     7818 2023-05-14 01:56:34.000000 polygon_finance-1.0.6/polygon_finance/sdks/webull_sdk/financial_statement.py
+-rw-rw-rw-   0        0        0     3871 2023-05-14 01:56:34.000000 polygon_finance-1.0.6/polygon_finance/sdks/webull_sdk/forecast.py
+-rw-rw-rw-   0        0        0     1033 2023-05-14 01:56:34.000000 polygon_finance-1.0.6/polygon_finance/sdks/webull_sdk/institutional_holdings.py
+-rw-rw-rw-   0        0        0     1156 2023-05-14 01:56:34.000000 polygon_finance-1.0.6/polygon_finance/sdks/webull_sdk/manage.py
+-rw-rw-rw-   0        0        0      617 2023-05-14 01:56:34.000000 polygon_finance-1.0.6/polygon_finance/sdks/webull_sdk/news.py
+-rw-rw-rw-   0        0        0      307 2023-05-14 01:56:34.000000 polygon_finance-1.0.6/polygon_finance/sdks/webull_sdk/shortinterest.py
+-rw-rw-rw-   0        0        0     2768 2023-05-15 04:24:58.000000 polygon_finance-1.0.6/polygon_finance/sdks/webull_sdk/top_gainers.py
+-rw-rw-rw-   0        0        0    16723 2023-05-14 01:56:34.000000 polygon_finance-1.0.6/polygon_finance/sdks/webull_sdk/top_options.py
+-rw-rw-rw-   0        0        0     5556 2023-05-14 01:56:34.000000 polygon_finance-1.0.6/polygon_finance/sdks/webull_sdk/webull_data.py
+-rw-rw-rw-   0        0        0    43244 2023-05-15 04:26:38.000000 polygon_finance-1.0.6/polygon_finance/sdks/webull_sdk/webull_sdk.py
+-rw-rw-rw-   0        0        0     1123 2023-05-20 03:53:51.000000 polygon_finance-1.0.6/polygon_finance/start_here.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:57:38.102189 polygon_finance-1.0.6/polygon_finance/terminals/
+-rw-rw-rw-   0        0        0        0 2023-05-14 16:41:17.000000 polygon_finance-1.0.6/polygon_finance/terminals/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:57:38.105190 polygon_finance-1.0.6/polygon_finance/terminals/crypto/
+-rw-rw-rw-   0        0        0        0 2023-05-14 16:42:17.000000 polygon_finance-1.0.6/polygon_finance/terminals/crypto/__init__.py
+-rw-rw-rw-   0        0        0     3642 2023-05-20 03:54:28.000000 polygon_finance-1.0.6/polygon_finance/terminals/crypto/crypto_terminal.py
+-rw-rw-rw-   0        0        0     1731 2023-05-14 16:53:24.000000 polygon_finance-1.0.6/polygon_finance/terminals/crypto/menu.py
+drwxrwxrwx   0        0        0        0 2023-05-20 03:57:37.946627 polygon_finance-1.0.6/polygon_finance.egg-info/
+-rw-rw-rw-   0        0        0      241 2023-05-20 03:57:37.000000 polygon_finance-1.0.6/polygon_finance.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7242 2023-05-20 03:57:37.000000 polygon_finance-1.0.6/polygon_finance.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 03:57:37.000000 polygon_finance-1.0.6/polygon_finance.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1253 2023-05-20 03:57:37.000000 polygon_finance-1.0.6/polygon_finance.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-20 03:57:37.000000 polygon_finance-1.0.6/polygon_finance.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-20 03:57:38.107189 polygon_finance-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     2577 2023-05-20 03:57:34.000000 polygon_finance-1.0.6/setup.py
```

### Comparing `polygon_finance-1.0.5/polygon_finance/discord/discord_utils/discord_stock_market.py` & `polygon_finance-1.0.6/polygon_finance/discord/discord_utils/discord_stock_market.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 from polygon.websocket import WebSocketMessage,EquityTrade, WebSocketClient, Market
 from asyncio import Queue
 import asyncio
 import numpy as np
 ##import SDKS, config files
 from cfg import YOUR_API_KEY, five_days_from_now_str, five_days_ago_str
 from discord_webhook import AsyncDiscordWebhook, DiscordEmbed
-from polygon_finance.polygon_sdk.technical_conditions import check_macd_condition_bearish, check_macd_condition_bullish,check_rsi_condition_bearish,check_rsi_condition_bullish
+from polygon_finance.sdks.polygon_sdk.technical_conditions import check_macd_condition_bearish, check_macd_condition_bullish,check_rsi_condition_bearish,check_rsi_condition_bullish
 from cfg import today_str
-from polygon_finance.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
-from polygon_finance.webull_sdk.webull_sdk import AsyncWebullSDK, thresholds
-from polygon_finance.polygon_sdk.async_options_sdk import PolygonOptionsSDK
+from polygon_finance.sdks.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
+from polygon_finance.sdks.webull_sdk.webull_sdk import AsyncWebullSDK, thresholds
+from polygon_finance.sdks.polygon_sdk.async_options_sdk import PolygonOptionsSDK
 
 #different ticker-hooks to send ticker-specific messages to discord
 
 from hooks.webhook_info import (
     china_hooks,
     india_hooks,
     index_hooks,
```

### Comparing `polygon_finance-1.0.5/polygon_finance/discord/discord_utils/emojis.py` & `polygon_finance-1.0.6/polygon_finance/discord/discord_utils/emojis.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.5/polygon_finance/discord/discord_utils/hooks/channel_webhooks.py` & `polygon_finance-1.0.6/polygon_finance/discord/discord_utils/hooks/channel_webhooks.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.5/polygon_finance/discord/discord_utils/hooks/send_webhook.py` & `polygon_finance-1.0.6/polygon_finance/discord/discord_utils/hooks/send_webhook.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import aiohttp
 from discord_webhook import AsyncDiscordWebhook, DiscordEmbed
-from polygon_finance.polygon_sdk.helpers.helpers import human_readable
+from polygon_finance.sdks.polygon_sdk.helpers.helpers import human_readable
 
 async def send_webhook(webhook_url, logo, description,symb, price, ask, mid, bid, bid_size, ask_size, break_even, 
                        change_to_break_even, contract_type, day_change, day_change_percent, 
                        close, high, open, low, decoded_conditions, last_trade_exchange, 
                        last_sip_timestamp, last_trade_price, last_trade_size, previous_close, 
                        day_volume, day_vwap, delta, gamma, theta, vega, iv, expiration, strike, 
                        exercise_style, under_ticker, oi, er_date, avg_10d_vol, avg_3m_vol, fifty_high,
```

### Comparing `polygon_finance-1.0.5/polygon_finance/discord/discord_utils/hooks/webhook_info.py` & `polygon_finance-1.0.6/polygon_finance/discord/discord_utils/hooks/webhook_info.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.5/polygon_finance/discord/discord_utils/live_discord.py` & `polygon_finance-1.0.6/polygon_finance/discord/discord_utils/live_discord.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from polygon.websocket import WebSocketClient, WebSocketMessage, EquityAgg, Market, EquityTrade
 from asyncio import Queue, BoundedSemaphore
 import asyncio
 import numpy as np
-from polygon_finance.polygon_sdk.technical_conditions import check_macd_condition,check_rsi_condition
+from polygon_finance.sdks.polygon_sdk.technical_conditions import check_macd_condition,check_rsi_condition
 
 
 from discord_utils.hooks.webhook_info import china_hooks,india_hooks,index_hooks,meme_hooks,russia_hooks,ETF_BROAD_MARKET_HOOKS
 from discord_utils.hooks.channel_webhooks import sell,strongbuy,underperform,holdrating, oversold,overbought, overbought_1day,overbought_week,oversold_1day,oversold_week, eightypercent,tenorless,twentytoforty,fortytoeighty, onehundredplus
 from discord_utils.hooks.channel_webhooks import firesale,accumulate,neutzone, aboveavgvolume, belowavgvolume, fiftyhighh,fiftylowh, earningstoday, weekbanana,daybanana,hourbanana, lowfloat
 c = WebSocketClient(YOUR_API_KEY, subscriptions=["T.*"], market= Market.Stocks)
 
 from cfg import today_str, YOUR_API_KEY, five_days_from_now_str
 from discord_webhook import AsyncDiscordWebhook, DiscordEmbed
-from polygon_finance.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
-from polygon_finance.webull_sdk.webull_sdk import AsyncWebullSDK, thresholds
-from polygon_finance.polygon_sdk.async_options_sdk import PolygonOptionsSDK
+from polygon_finance.sdks.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
+from polygon_finance.sdks.webull_sdk.webull_sdk import AsyncWebullSDK, thresholds
+from polygon_finance.sdks.polygon_sdk.async_options_sdk import PolygonOptionsSDK
 polyoptions = PolygonOptionsSDK(YOUR_API_KEY)
 polygon = AsyncPolygonSDK(YOUR_API_KEY)
 webull = AsyncWebullSDK()
 import logging
 semaphore = BoundedSemaphore(10)
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
```

### Comparing `polygon_finance-1.0.5/polygon_finance/discord/discord_utils/menus.py` & `polygon_finance-1.0.6/polygon_finance/discord/discord_utils/menus.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.5/polygon_finance/discord/discord_utils/selectmenus/mainselect.py` & `polygon_finance-1.0.6/polygon_finance/discord/discord_utils/selectmenus/mainselect.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 import disnake
 import pandas as pd
-from polygon_finance.webull_sdk.forecast import ForecastEvaluator
+from polygon_finance.sdks.webull_sdk.forecast import ForecastEvaluator
 import openai
-from polygon_finance.polygon_sdk.get_all_options import fetch_all_option_contracts
+from polygon_finance.sdks.polygon_sdk.get_all_options import fetch_all_option_contracts
 from tabulate import tabulate
 from urllib.request import url2pathname
 from cfg import today_str, YOUR_OPENAI_KEY, YOUR_API_KEY
 from datetime import datetime
-from polygon_finance.webull_sdk.webull_sdk import thresholds
-from polygon_finance.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
-from polygon_finance.polygon_sdk.helpers.helpers import get_checkmark
+from polygon_finance.sdks.webull_sdk.webull_sdk import thresholds
+from polygon_finance.sdks.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
+from polygon_finance.helpers.helpers import get_checkmark
 from examples.summarizer import extract_pdf_text,extract_html_text,extract_html_text_from_file,extract_pdf_text_from_url,create_summary
 from bs4 import BeautifulSoup
 from discord_utils.menus import AlertMenus
 import pandas as pd
-from polygon_finance.polygon_sdk.async_options_sdk import PolygonOptionsSDK
+from polygon_finance.sdks.polygon_sdk.async_options_sdk import PolygonOptionsSDK
 import disnake
-from polygon_finance.webull_sdk.webull_sdk import AsyncWebullSDK
+from polygon_finance.sdks.webull_sdk.webull_sdk import AsyncWebullSDK
 webull = AsyncWebullSDK()
 import requests
 import disnake
 
 from ..menus import AlertMenus
 import requests
-from polygon_finance.webull_sdk.webull_sdk import AsyncWebullSDK
+from polygon_finance.sdks.webull_sdk.webull_sdk import AsyncWebullSDK
 from cfg import today_str
-from polygon_finance.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
+from polygon_finance.sdks.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
 from datetime import datetime
 import asyncio
 
 today = datetime.today()
 from cfg import YOUR_API_KEY
-from polygon_finance.fudstop_sdk.fudstop_sdk import fudstopSDK
+from polygon_finance.sdks.fudstop_sdk.fudstop_sdk import fudstopSDK
 fudstop = fudstopSDK()
 polygon = AsyncPolygonSDK(YOUR_API_KEY)
-from polygon_finance.polygon_sdk.async_options_sdk import PolygonOptionsSDK
+from polygon_finance.sdks.polygon_sdk.async_options_sdk import PolygonOptionsSDK
 polyoptions = PolygonOptionsSDK(YOUR_API_KEY)
 webull = AsyncWebullSDK()
 import disnake
 import asyncio
 from examples.summarizer import (
     extract_html_text,
     extract_html_text_from_file,
```

### Comparing `polygon_finance-1.0.5/polygon_finance/discord/discord_utils/views/mainview.py` & `polygon_finance-1.0.6/polygon_finance/discord/discord_utils/views/mainview.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import disnake
 from ..selectmenus.mainselect import FTDShortSelect
 import requests
-from polygon_finance.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
+from polygon_finance.sdks.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
 from typing import List
 from datetime import datetime
 import asyncio
 today = datetime.today()
 from cfg import YOUR_API_KEY
 polygon = AsyncPolygonSDK(YOUR_API_KEY)
```

### Comparing `polygon_finance-1.0.5/polygon_finance/discord/discord_utils/webhook_creation.py` & `polygon_finance-1.0.6/polygon_finance/discord/discord_utils/webhook_creation.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.5/polygon_finance/discord/embeddings/embeddings.py` & `polygon_finance-1.0.6/polygon_finance/discord/embeddings/embeddings.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.5/polygon_finance/discord/embeddings/embeds.py` & `polygon_finance-1.0.6/polygon_finance/discord/embeddings/embeds.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 
 
 sys.path.append(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
 
 
 from discord_utils import emojis
 from discord_webhook import AsyncDiscordWebhook, DiscordEmbed
-from polygon_finance.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
-from polygon_finance.polygon_sdk.async_options_sdk import PolygonOptionsSDK
+from polygon_finance.sdks.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
+from polygon_finance.sdks.polygon_sdk.async_options_sdk import PolygonOptionsSDK
 from polygon_finance.webull_sdk.webull_sdk import AsyncWebullSDK
-from polygon_finance.polygon_sdk.mapping_dicts import STOCK_EXCHANGES, stock_condition_dict
+from polygon_finance.sdks.polygon_sdk.mapping_dicts import STOCK_EXCHANGES, stock_condition_dict
 
 
 from cfg import YOUR_API_KEY
 
 webull = AsyncWebullSDK()
 class Data:
     def __init__(self, symbol=None):
```

### Comparing `polygon_finance-1.0.5/polygon_finance/discord/webhook_creation.py` & `polygon_finance-1.0.6/polygon_finance/discord/webhook_creation.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.5/polygon_finance/discord_examples/indices_spx_rsi.py` & `polygon_finance-1.0.6/polygon_finance/discord_examples/indices_spx_rsi.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from polygon.websocket import Market, WebSocketClient, WebSocketMessage
 import time
 from typing import List
 import asyncio
 from discord_webhook import AsyncDiscordWebhook, DiscordEmbed
 from cfg import YOUR_API_KEY, hex_colors
-from polygon_finance.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
+from sdks.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
 
 poly = AsyncPolygonSDK(YOUR_API_KEY)
 c = WebSocketClient(subscriptions=["V.I:SPX"], market=Market.Indices, api_key=YOUR_API_KEY) #connect to the crypto market and subscribe to trades and quotes
 
 
 async def handle_msg(msgs: List[WebSocketMessage]):
     for m in msgs:
```

### Comparing `polygon_finance-1.0.5/polygon_finance/examples/all_attributes.py` & `polygon_finance-1.0.6/polygon_finance/examples/all_attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 import os
 
 sys.path.append(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
 
 import asyncio
 
 
-from polygon_finance.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
-from polygon_finance.polygon_sdk.async_options_sdk import PolygonOptionsSDK
+from polygon_finance.sdks.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
+from polygon_finance.sdks.polygon_sdk.async_options_sdk import PolygonOptionsSDK
 from polygon_finance.webull_sdk.webull_sdk import AsyncWebullSDK
 from polygon_finance.fudstop_sdk.fudstop_sdk import fudstopSDK
-from polygon_finance.polygon_sdk.helpers.helpers import human_readable
+from polygon_finance.sdks.polygon_sdk.helpers.helpers import human_readable
 
 from cfg import YOUR_API_KEY, five_days_ago_str, today_str
 
 poly = AsyncPolygonSDK(YOUR_API_KEY)
 webull = AsyncWebullSDK()
 fudstop = fudstopSDK()
```

### Comparing `polygon_finance-1.0.5/polygon_finance/examples/bollinger_bands.py` & `polygon_finance-1.0.6/polygon_finance/examples/bollinger_bands.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 sys.path.append(os.path.dirname(os.path.dirname(os.path.dirname(os.path.abspath(__file__)))))
 
 
 import asyncio
 
-from polygon_finance.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
+from polygon_finance.sdks.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
 from cfg import YOUR_API_KEY, today_str
 
 poly = AsyncPolygonSDK(YOUR_API_KEY)
 ticker = "NVDA"
 
 async def main():
```

### Comparing `polygon_finance-1.0.5/polygon_finance/examples/create_option_symbol.py` & `polygon_finance-1.0.6/polygon_finance/examples/create_option_symbol.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 sys.path.append(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
 
 import asyncio
 
 from cfg import YOUR_API_KEY
 
-from polygon_finance.polygon_sdk.async_options_sdk import PolygonOptionsSDK
+from polygon_finance.sdks.polygon_sdk.async_options_sdk import PolygonOptionsSDK
 
 polyoptions = PolygonOptionsSDK(YOUR_API_KEY)
 
 
 underlying_symbol = "F"
 expiration_date = "2023-05-19"
 option_type = "C"
```

### Comparing `polygon_finance-1.0.5/polygon_finance/examples/ema.py` & `polygon_finance-1.0.6/polygon_finance/examples/ema.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 sys.path.append(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
 
 
 import asyncio
 
-from polygon_finance.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
+from polygon_finance.sdks.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
 from cfg import YOUR_API_KEY
 
 ticker = "BAC"
 polygonsdk = AsyncPolygonSDK(YOUR_API_KEY)
 
 
 async def exponential_moving_average(ticker):
```

### Comparing `polygon_finance-1.0.5/polygon_finance/examples/fetch_entire_chain.py` & `polygon_finance-1.0.6/polygon_finance/examples/fetch_entire_chain.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 sys.path.append(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
 
 import asyncio
 import pandas as pd
 
 from cfg import YOUR_API_KEY
 
-from polygon_finance.polygon_sdk.async_options_sdk import PolygonOptionsSDK
-from polygon_finance.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
+from polygon_finance.sdks.polygon_sdk.async_options_sdk import PolygonOptionsSDK
+from polygon_finance.sdks.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
 from polygon_finance.webull_sdk.webull_sdk import AsyncWebullSDK
 
 
 webull = AsyncWebullSDK()
 poly = AsyncPolygonSDK(YOUR_API_KEY)
 polyoptions = PolygonOptionsSDK(YOUR_API_KEY)
```

### Comparing `polygon_finance-1.0.5/polygon_finance/examples/functions/all_attributes.py` & `polygon_finance-1.0.6/polygon_finance/examples/functions/all_attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 import os
 
 sys.path.append(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
 
 import asyncio
 
 
-from polygon_finance.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
-from polygon_finance.polygon_sdk.async_options_sdk import PolygonOptionsSDK
+from polygon_finance.sdks.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
+from polygon_finance.sdks.polygon_sdk.async_options_sdk import PolygonOptionsSDK
 from polygon_finance.webull_sdk.webull_sdk import AsyncWebullSDK
 from polygon_finance.fudstop_sdk.fudstop_sdk import fudstopSDK
-from polygon_finance.polygon_sdk.helpers.helpers import human_readable
+from polygon_finance.sdks.polygon_sdk.helpers.helpers import human_readable
 
 from cfg import YOUR_API_KEY, five_days_ago_str, today_str
 
 poly = AsyncPolygonSDK(YOUR_API_KEY)
 webull = AsyncWebullSDK()
 fudstop = fudstopSDK()
```

### Comparing `polygon_finance-1.0.5/polygon_finance/examples/functions/bollinger_bands.py` & `polygon_finance-1.0.6/polygon_finance/examples/functions/bollinger_bands.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 sys.path.append(os.path.dirname(os.path.dirname(os.path.dirname(os.path.abspath(__file__)))))
 
 
 import asyncio
 
-from polygon_finance.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
+from polygon_finance.sdks.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
 from cfg import YOUR_API_KEY, today_str
 
 poly = AsyncPolygonSDK(YOUR_API_KEY)
 ticker = "NVDA"
 
 async def main():
```

### Comparing `polygon_finance-1.0.5/polygon_finance/examples/functions/create_option_symbol.py` & `polygon_finance-1.0.6/polygon_finance/examples/functions/create_option_symbol.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 sys.path.append(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
 
 import asyncio
 
 from cfg import YOUR_API_KEY
 
-from polygon_finance.polygon_sdk.async_options_sdk import PolygonOptionsSDK
+from polygon_finance.sdks.polygon_sdk.async_options_sdk import PolygonOptionsSDK
 
 polyoptions = PolygonOptionsSDK(YOUR_API_KEY)
 
 
 underlying_symbol = "F"
 expiration_date = "2023-05-19"
 option_type = "C"
```

### Comparing `polygon_finance-1.0.5/polygon_finance/examples/functions/ema.py` & `polygon_finance-1.0.6/polygon_finance/examples/functions/ema.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 sys.path.append(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
 
 
 import asyncio
 
-from polygon_finance.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
+from polygon_finance.sdks.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
 from cfg import YOUR_API_KEY
 
 ticker = "BAC"
 polygonsdk = AsyncPolygonSDK(YOUR_API_KEY)
 
 
 async def exponential_moving_average(ticker):
```

### Comparing `polygon_finance-1.0.5/polygon_finance/examples/functions/fetch_entire_chain.py` & `polygon_finance-1.0.6/polygon_finance/examples/functions/fetch_entire_chain.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 sys.path.append(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
 
 import asyncio
 import pandas as pd
 
 from cfg import YOUR_API_KEY
 
-from polygon_finance.polygon_sdk.async_options_sdk import PolygonOptionsSDK
-from polygon_finance.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
+from polygon_finance.sdks.polygon_sdk.async_options_sdk import PolygonOptionsSDK
+from polygon_finance.sdks.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
 from polygon_finance.webull_sdk.webull_sdk import AsyncWebullSDK
 
 
 webull = AsyncWebullSDK()
 poly = AsyncPolygonSDK(YOUR_API_KEY)
 polyoptions = PolygonOptionsSDK(YOUR_API_KEY)
```

### Comparing `polygon_finance-1.0.5/polygon_finance/examples/functions/find_gaps.py` & `polygon_finance-1.0.6/polygon_finance/examples/functions/find_gaps.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 import os
 
 sys.path.append(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
 
 
-from polygon_finance.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
+from polygon_finance.sdks.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
 import asyncio
 from cfg import YOUR_API_KEY
 
 sdk = AsyncPolygonSDK(YOUR_API_KEY)
 async def main():
 
     ticker="SPY"
```

### Comparing `polygon_finance-1.0.5/polygon_finance/examples/functions/get_all_options_data.py` & `polygon_finance-1.0.6/polygon_finance/examples/functions/get_all_options_data.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import sys
 import os
 
 sys.path.append(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
 
 import asyncio
-from polygon_finance.polygon_sdk.async_options_sdk import PolygonOptionsSDK
+from polygon_finance.sdks.polygon_sdk.async_options_sdk import PolygonOptionsSDK
 from cfg import YOUR_API_KEY
 polyoptions = PolygonOptionsSDK(YOUR_API_KEY)
 
 
 async def get_all_options_data():
 
     contracts  = await polyoptions.fetch_all_option_contracts(
```

### Comparing `polygon_finance-1.0.5/polygon_finance/examples/functions/get_ema.py` & `polygon_finance-1.0.6/polygon_finance/examples/functions/get_ema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 import os
 
 sys.path.append(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
 
-from polygon_finance.polygon_sdk.async_options_sdk import PolygonOptionsSDK
-from polygon_finance.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
+from polygon_finance.sdks.polygon_sdk.async_options_sdk import PolygonOptionsSDK
+from polygon_finance.sdks.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
 from cfg import YOUR_API_KEY
 
 import asyncio
 
 poly = AsyncPolygonSDK(YOUR_API_KEY)
 polyopt = PolygonOptionsSDK(YOUR_API_KEY)
```

### Comparing `polygon_finance-1.0.5/polygon_finance/examples/functions/get_latest_crypto_data.py` & `polygon_finance-1.0.6/polygon_finance/examples/functions/get_latest_crypto_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 import os
 
 sys.path.append(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
 
 import asyncio
 import pandas as pd
-from polygon_finance.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
+from polygon_finance.sdks.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
 from cfg import YOUR_API_KEY
 polygonsdk = AsyncPolygonSDK(YOUR_API_KEY)
 
 
 async def get_all_crypto_data():
 
     crypto_snapshots = await polygonsdk.get_all_crypto_snapshots()
```

### Comparing `polygon_finance-1.0.5/polygon_finance/examples/functions/get_latest_forex_data.py` & `polygon_finance-1.0.6/polygon_finance/examples/functions/get_latest_forex_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 import os
 
 sys.path.append(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
 
 import asyncio
 import pandas as pd
-from polygon_finance.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
+from polygon_finance.sdks.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
 from cfg import YOUR_API_KEY
 polygonsdk = AsyncPolygonSDK(YOUR_API_KEY)
 
 
 async def get_forex_data():
 
     forex_snapshots = await polygonsdk.get_all_forex_snapshots()
```

### Comparing `polygon_finance-1.0.5/polygon_finance/examples/functions/get_macd.py` & `polygon_finance-1.0.6/polygon_finance/examples/functions/get_macd.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 import os
 
 sys.path.append(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
 
-from polygon_finance.polygon_sdk.async_options_sdk import PolygonOptionsSDK
-from polygon_finance.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
+from polygon_finance.sdks.polygon_sdk.async_options_sdk import PolygonOptionsSDK
+from polygon_finance.sdks.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
 from cfg import YOUR_API_KEY
 
 import asyncio
 
 poly = AsyncPolygonSDK(YOUR_API_KEY)
 polyopt = PolygonOptionsSDK(YOUR_API_KEY)
```

### Comparing `polygon_finance-1.0.5/polygon_finance/examples/functions/get_pivot_points.py` & `polygon_finance-1.0.6/polygon_finance/examples/functions/get_pivot_points.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 sys.path.append(os.path.dirname(os.path.dirname(os.path.dirname(os.path.abspath(__file__)))))
 
 
 import asyncio 
 
-from polygon_finance.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
+from polygon_finance.sdks.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
 
 from cfg import YOUR_API_KEY
 
 poly = AsyncPolygonSDK(YOUR_API_KEY)
 async def pivot_point():
```

### Comparing `polygon_finance-1.0.5/polygon_finance/examples/functions/get_rsi.py` & `polygon_finance-1.0.6/polygon_finance/examples/functions/get_rsi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 import os
 
 sys.path.append(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
 
-from polygon_finance.polygon_sdk.async_options_sdk import PolygonOptionsSDK
-from polygon_finance.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
+from polygon_finance.sdks.polygon_sdk.async_options_sdk import PolygonOptionsSDK
+from polygon_finance.sdks.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
 from cfg import YOUR_API_KEY
 
 import asyncio
 
 poly = AsyncPolygonSDK(YOUR_API_KEY)
 polyopt = PolygonOptionsSDK(YOUR_API_KEY)
```

### Comparing `polygon_finance-1.0.5/polygon_finance/examples/functions/get_sma.py` & `polygon_finance-1.0.6/polygon_finance/examples/functions/get_sma.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 import os
 
 sys.path.append(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
 
-from polygon_finance.polygon_sdk.async_options_sdk import PolygonOptionsSDK
-from polygon_finance.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
+from polygon_finance.sdks.polygon_sdk.async_options_sdk import PolygonOptionsSDK
+from polygon_finance.sdks.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
 from cfg import YOUR_API_KEY
 
 import asyncio
 
 poly = AsyncPolygonSDK(YOUR_API_KEY)
 polyopt = PolygonOptionsSDK(YOUR_API_KEY)
```

### Comparing `polygon_finance-1.0.5/polygon_finance/examples/functions/latest_news.py` & `polygon_finance-1.0.6/polygon_finance/examples/functions/latest_news.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 import os
 
 sys.path.append(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
 
 import asyncio
 
-from polygon_finance.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
+from polygon_finance.sdks.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
 from cfg import YOUR_API_KEY
 
 polygonsdk = AsyncPolygonSDK(YOUR_API_KEY)
 ticker="AAPL"
 async def news(ticker):
     """
     Retrieve the latest news for a specific ticker and print the details.
```

### Comparing `polygon_finance-1.0.5/polygon_finance/examples/functions/option_quote.py` & `polygon_finance-1.0.6/polygon_finance/examples/functions/option_quote.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 sys.path.append(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
 
 import asyncio
 from datetime import datetime
 import pandas as pd
 
-from polygon_finance.polygon_sdk.async_options_sdk import PolygonOptionsSDK
+from polygon_finance.sdks.polygon_sdk.async_options_sdk import PolygonOptionsSDK
 from polygon_finance.helpers.helpers import get_date_string
 
 from cfg import YOUR_API_KEY
 
 now = datetime.now()
 sdk = PolygonOptionsSDK(YOUR_API_KEY)
```

### Comparing `polygon_finance-1.0.5/polygon_finance/examples/functions/option_trades.py` & `polygon_finance-1.0.6/polygon_finance/examples/functions/option_trades.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 sys.path.append(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
 
 import asyncio
 import pandas as pd
 
 from cfg import YOUR_API_KEY
-from polygon_finance.polygon_sdk.async_options_sdk import PolygonOptionsSDK
-from polygon_finance.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
+from polygon_finance.sdks.polygon_sdk.async_options_sdk import PolygonOptionsSDK
+from polygon_finance.sdks.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
 
 polyoptions = PolygonOptionsSDK(YOUR_API_KEY)
 poly = AsyncPolygonSDK(YOUR_API_KEY)
 
 async def get_trades():
     """
     Retrieve option trades for a specific option symbol and save them to a CSV file.
```

### Comparing `polygon_finance-1.0.5/polygon_finance/examples/functions/plot_aggs.py` & `polygon_finance-1.0.6/polygon_finance/examples/functions/plot_aggs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 PLOT CHARTS USING AGGREGATES DATA
 """
 import asyncio
 import pandas as pd
 import matplotlib.pyplot as plt
 import mplfinance as mpf
-from polygon_finance.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
+from polygon_finance.sdks.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
 from cfg import YOUR_API_KEY
 poly = AsyncPolygonSDK(YOUR_API_KEY)
 
 
 ticker="SPY"
 multiplier=1
 timespan="day"
```

### Comparing `polygon_finance-1.0.5/polygon_finance/examples/functions/plot_macd.py` & `polygon_finance-1.0.6/polygon_finance/examples/functions/plot_macd.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 PLOT CHARTS USING AGGREGATES DATA
 """
 import asyncio
 import pandas as pd
 import matplotlib.pyplot as plt
 import mplfinance as mpf
-from polygon_finance.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
+from polygon_finance.sdks.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
 from cfg import YOUR_API_KEY
 poly = AsyncPolygonSDK(YOUR_API_KEY)
 
 
 
 ticker="AMD"
 multiplier=1
```

### Comparing `polygon_finance-1.0.5/polygon_finance/examples/functions/plot_option_aggs.py` & `polygon_finance-1.0.6/polygon_finance/examples/functions/plot_option_aggs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 PLOT CHARTS USING AGGREGATES DATA
 """
 import asyncio
 import pandas as pd
 import matplotlib.pyplot as plt
 import mplfinance as mpf
-from polygon_finance.polygon_sdk.async_options_sdk import PolygonOptionsSDK
+from polygon_finance.sdks.polygon_sdk.async_options_sdk import PolygonOptionsSDK
 from cfg import YOUR_API_KEY
 poly = PolygonOptionsSDK(YOUR_API_KEY)
 
 
 underlying_symbol="SPY"
 expiration_date="2023-05-22"
 option_type="C"
```

### Comparing `polygon_finance-1.0.5/polygon_finance/examples/functions/rate_of_change.py` & `polygon_finance-1.0.6/polygon_finance/examples/functions/rate_of_change.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 sys.path.append(os.path.dirname(os.path.dirname(os.path.dirname(os.path.abspath(__file__)))))
 
 import asyncio
 import pandas as pd
 
-from polygon_finance.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
+from polygon_finance.sdks.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
 from cfg import YOUR_API_KEY, today_str
 
 poly = AsyncPolygonSDK(YOUR_API_KEY)
 ticker = "MSFT"
 
 async def main():
```

### Comparing `polygon_finance-1.0.5/polygon_finance/examples/functions/scanner_example.py` & `polygon_finance-1.0.6/polygon_finance/examples/functions/scanner_example.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from typing import List
 from asyncio import Queue
 import random
 import csv
 import asyncio
 import pandas as pd
 from polygon_finance.helpers.helpers import human_readable
-from polygon_finance.polygon_sdk.async_options_sdk import PolygonOptionsSDK
+from polygon_finance.sdks.polygon_sdk.async_options_sdk import PolygonOptionsSDK
 from polygon_finance.models.test_events import TestOptionsEvent, option_condition_dict, OPTIONS_EXCHANGES
 
 from polygon_finance.helpers.helpers import extract_underlying_symbol
 from polygon_finance.simulated_markets.helpers import write_to_csv
 from cfg import YOUR_API_KEY
 from cachetools import TTLCache
 sdk = PolygonOptionsSDK(YOUR_API_KEY)
```

### Comparing `polygon_finance-1.0.5/polygon_finance/examples/functions/stock_aggregates.py` & `polygon_finance-1.0.6/polygon_finance/examples/functions/stock_aggregates.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 sys.path.append(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
 
 import asyncio
 import pandas as pd
 
-from polygon_finance.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
+from polygon_finance.sdks.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
 from cfg import YOUR_API_KEY, five_days_ago_str, today_str
 
 polygonsdk = AsyncPolygonSDK(YOUR_API_KEY)
 ticker = "GME"
 
 async def stock_aggregates_example(ticker):
     """
```

### Comparing `polygon_finance-1.0.5/polygon_finance/examples/functions/summarizer.py` & `polygon_finance-1.0.6/polygon_finance/examples/functions/summarizer.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.5/polygon_finance/examples/functions/support_resistance.py` & `polygon_finance-1.0.6/polygon_finance/examples/functions/support_resistance.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 import os
 
 sys.path.append(os.path.dirname(os.path.dirname(os.path.dirname(os.path.abspath(__file__)))))
 
 
 import asyncio
-from polygon_finance.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
+from polygon_finance.sdks.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
 from cfg import YOUR_API_KEY, five_days_ago_str, today_str
 
 polygonsdk = AsyncPolygonSDK(YOUR_API_KEY)
 ticker = "GME"
 
 async def support_resistance_example(ticker):
     """
```

### Comparing `polygon_finance-1.0.5/polygon_finance/examples/get_all_options_data.py` & `polygon_finance-1.0.6/polygon_finance/examples/get_all_options_data.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import sys
 import os
 
 sys.path.append(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
 
 import asyncio
-from polygon_finance.polygon_sdk.async_options_sdk import PolygonOptionsSDK
+from polygon_finance.sdks.polygon_sdk.async_options_sdk import PolygonOptionsSDK
 from cfg import YOUR_API_KEY
 polyoptions = PolygonOptionsSDK(YOUR_API_KEY)
 
 
 async def get_all_options_data():
 
     contracts  = await polyoptions.fetch_all_option_contracts(
```

### Comparing `polygon_finance-1.0.5/polygon_finance/examples/get_latest_crypto_data.py` & `polygon_finance-1.0.6/polygon_finance/examples/get_latest_crypto_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 import os
 
 sys.path.append(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
 
 import asyncio
 import pandas as pd
-from polygon_finance.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
+from polygon_finance.sdks.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
 from cfg import YOUR_API_KEY
 polygonsdk = AsyncPolygonSDK(YOUR_API_KEY)
 
 
 async def get_all_crypto_data():
 
     crypto_snapshots = await polygonsdk.get_all_crypto_snapshots()
```

### Comparing `polygon_finance-1.0.5/polygon_finance/examples/get_latest_forex_data.py` & `polygon_finance-1.0.6/polygon_finance/examples/get_latest_forex_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 import os
 
 sys.path.append(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
 
 import asyncio
 import pandas as pd
-from polygon_finance.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
+from polygon_finance.sdks.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
 from cfg import YOUR_API_KEY
 polygonsdk = AsyncPolygonSDK(YOUR_API_KEY)
 
 
 async def get_forex_data():
 
     forex_snapshots = await polygonsdk.get_all_forex_snapshots()
```

### Comparing `polygon_finance-1.0.5/polygon_finance/examples/get_latest_ticker_data.py` & `polygon_finance-1.0.6/polygon_finance/examples/realtime_markets/indices_market.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 import sys
 import os
 
-sys.path.append(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
+sys.path.append(os.path.dirname(os.path.dirname(os.path.dirname(os.path.abspath(__file__)))))
 
+from polygon.websocket import WebSocketMessage, WebSocketClient, Market
+from polygon.websocket import WebSocketClient
+from polygon.websocket.models import WebSocketMessage
+from typing import List
 import asyncio
 
-import asyncio
-import csv
-from polygon_finance.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
 from cfg import YOUR_API_KEY
-import pandas as pd
-polygonsdk = AsyncPolygonSDK(YOUR_API_KEY)
+from polygon_finance.sdks.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
+
+poly = AsyncPolygonSDK(YOUR_API_KEY)
+c = WebSocketClient(subscriptions=["V.*"], market=Market.Indices, api_key=YOUR_API_KEY) #connect to the crypto market and subscribe to trades and quotes
+
+
+async def handle_msg(msgs: List[WebSocketMessage]):
+    for m in msgs:
+        print(m)
 
 
-filename="files/stocks/all_snapshots.csv"
 
-async def get_all_ticker_data():
-    """Gets all snapshots market-wide and saves
-    to CSV for further analysis / testing purposes."""
 
-    await polygonsdk.write_snapshots_to_csv()
+async def main():
+    await asyncio.gather(c.connect(handle_msg))
 
-    print(f"Data has been successfully saved to files/stocks/all_snapshots.csv.")
-asyncio.run(get_all_ticker_data())
 
+asyncio.run(main())
```

### Comparing `polygon_finance-1.0.5/polygon_finance/examples/get_pivot_points.py` & `polygon_finance-1.0.6/polygon_finance/examples/get_pivot_points.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 sys.path.append(os.path.dirname(os.path.dirname(os.path.dirname(os.path.abspath(__file__)))))
 
 
 import asyncio 
 
-from polygon_finance.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
+from polygon_finance.sdks.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
 
 from cfg import YOUR_API_KEY
 
 poly = AsyncPolygonSDK(YOUR_API_KEY)
 async def pivot_point():
```

### Comparing `polygon_finance-1.0.5/polygon_finance/examples/latest_news.py` & `polygon_finance-1.0.6/polygon_finance/examples/latest_news.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 import os
 
 sys.path.append(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
 
 import asyncio
 
-from polygon_finance.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
+from polygon_finance.sdks.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
 from cfg import YOUR_API_KEY
 
 polygonsdk = AsyncPolygonSDK(YOUR_API_KEY)
 ticker="AAPL"
 async def news(ticker):
     """
     Retrieve the latest news for a specific ticker and print the details.
```

### Comparing `polygon_finance-1.0.5/polygon_finance/examples/option_quote.py` & `polygon_finance-1.0.6/polygon_finance/examples/option_quote.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 sys.path.append(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
 
 import asyncio
 from datetime import datetime
 import pandas as pd
 
-from polygon_finance.polygon_sdk.async_options_sdk import PolygonOptionsSDK
+from polygon_finance.sdks.polygon_sdk.async_options_sdk import PolygonOptionsSDK
 from polygon_finance.helpers.helpers import get_date_string
 
 from cfg import YOUR_API_KEY
 
 now = datetime.now()
 sdk = PolygonOptionsSDK(YOUR_API_KEY)
```

### Comparing `polygon_finance-1.0.5/polygon_finance/examples/option_trades.py` & `polygon_finance-1.0.6/polygon_finance/examples/option_trades.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 sys.path.append(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
 
 import asyncio
 import pandas as pd
 
 from cfg import YOUR_API_KEY
-from polygon_finance.polygon_sdk.async_options_sdk import PolygonOptionsSDK
-from polygon_finance.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
+from polygon_finance.sdks.polygon_sdk.async_options_sdk import PolygonOptionsSDK
+from polygon_finance.sdks.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
 
 polyoptions = PolygonOptionsSDK(YOUR_API_KEY)
 poly = AsyncPolygonSDK(YOUR_API_KEY)
 
 async def get_trades():
     """
     Retrieve option trades for a specific option symbol and save them to a CSV file.
```

### Comparing `polygon_finance-1.0.5/polygon_finance/examples/plot_aggs.py` & `polygon_finance-1.0.6/polygon_finance/examples/plot_aggs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 PLOT CHARTS USING AGGREGATES DATA
 """
 import asyncio
 import pandas as pd
 import matplotlib.pyplot as plt
 import mplfinance as mpf
-from polygon_finance.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
+from polygon_finance.sdks.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
 from cfg import YOUR_API_KEY
 poly = AsyncPolygonSDK(YOUR_API_KEY)
 
 
 ticker="SPY"
 multiplier=1
 timespan="day"
```

### Comparing `polygon_finance-1.0.5/polygon_finance/examples/plot_macd.py` & `polygon_finance-1.0.6/polygon_finance/examples/plot_macd.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 PLOT CHARTS USING AGGREGATES DATA
 """
 import asyncio
 import pandas as pd
 import matplotlib.pyplot as plt
 import mplfinance as mpf
-from polygon_finance.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
+from polygon_finance.sdks.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
 from cfg import YOUR_API_KEY
 poly = AsyncPolygonSDK(YOUR_API_KEY)
 
 
 
 ticker="AMD"
 multiplier=1
```

### Comparing `polygon_finance-1.0.5/polygon_finance/examples/plot_option_aggs.py` & `polygon_finance-1.0.6/polygon_finance/examples/plot_option_aggs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 PLOT CHARTS USING AGGREGATES DATA
 """
 import asyncio
 import pandas as pd
 import matplotlib.pyplot as plt
 import mplfinance as mpf
-from polygon_finance.polygon_sdk.async_options_sdk import PolygonOptionsSDK
+from polygon_finance.sdks.polygon_sdk.async_options_sdk import PolygonOptionsSDK
 from cfg import YOUR_API_KEY
 poly = PolygonOptionsSDK(YOUR_API_KEY)
 
 
 underlying_symbol="SPY"
 expiration_date="2023-05-22"
 option_type="C"
```

### Comparing `polygon_finance-1.0.5/polygon_finance/examples/rate_of_change.py` & `polygon_finance-1.0.6/polygon_finance/examples/rate_of_change.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 sys.path.append(os.path.dirname(os.path.dirname(os.path.dirname(os.path.abspath(__file__)))))
 
 import asyncio
 import pandas as pd
 
-from polygon_finance.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
+from polygon_finance.sdks.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
 from cfg import YOUR_API_KEY, today_str
 
 poly = AsyncPolygonSDK(YOUR_API_KEY)
 ticker = "MSFT"
 
 async def main():
```

### Comparing `polygon_finance-1.0.5/polygon_finance/examples/realtime_markets/crypto_market.py` & `polygon_finance-1.0.6/polygon_finance/examples/realtime_markets/crypto_market.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 sys.path.append(os.path.dirname(os.path.dirname(os.path.dirname(os.path.abspath(__file__)))))
 
 
 import asyncio
 from typing import List
 from polygon.websocket import WebSocketClient, WebSocketMessage, CryptoQuote, CryptoTrade, Market
-from polygon_finance.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
+from polygon_finance.sdks.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
 from cachetools import TTLCache
 
 from cfg import YOUR_API_KEY
 poly = AsyncPolygonSDK(YOUR_API_KEY)
 c = WebSocketClient(subscriptions=["XT.*, XQ.*"], market=Market.Crypto, api_key=YOUR_API_KEY)  # connect to the crypto market and subscribe to trades and quotes
 
 # Cache to store recent RSI values for each symbol
```

### Comparing `polygon_finance-1.0.5/polygon_finance/examples/realtime_markets/forex_market.py` & `polygon_finance-1.0.6/polygon_finance/examples/realtime_markets/forex_market.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from polygon.websocket import WebSocketMessage, WebSocketClient, Market, ForexQuote, CurrencyAgg, CryptoTrade
 from polygon.websocket import WebSocketClient
 from polygon.websocket.models import WebSocketMessage
 from typing import List
 import asyncio
 
 from cfg import YOUR_API_KEY
-from polygon_finance.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
+from polygon_finance.sdks.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
 
 poly = AsyncPolygonSDK(YOUR_API_KEY)
 c = WebSocketClient(subscriptions=["CA.*,C.*"], market=Market.Forex, api_key=YOUR_API_KEY) #connect to the crypto market and subscribe to trades and quotes
 
 
 async def handle_msg(msgs: List[WebSocketMessage]):
     for m in msgs:
```

### Comparing `polygon_finance-1.0.5/polygon_finance/examples/realtime_markets/options_market.py` & `polygon_finance-1.0.6/polygon_finance/examples/realtime_markets/options_market.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from polygon.websocket import WebSocketMessage, WebSocketClient, Market, EquityAgg, EquityQuote, EquityTrade
 from polygon.websocket import WebSocketClient
 from polygon.websocket.models import WebSocketMessage
 from typing import List
 import asyncio
 
 from cfg import YOUR_API_KEY
-from polygon_finance.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
+from polygon_finance.sdks.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
 
 poly = AsyncPolygonSDK(YOUR_API_KEY)
 c = WebSocketClient(subscriptions=["T.*,A.*,Q.*"], market=Market.Options, api_key=YOUR_API_KEY) #connect to the options market trades, aggs, and quotes.
 
 
 async def handle_msg(msgs: List[WebSocketMessage]):
     for m in msgs:
```

### Comparing `polygon_finance-1.0.5/polygon_finance/examples/realtime_markets/stock_market.py` & `polygon_finance-1.0.6/polygon_finance/examples/realtime_markets/stock_market.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 from polygon.websocket import WebSocketMessage, WebSocketClient, Market, EquityAgg, EquityQuote, EquityTrade
 from polygon.websocket import WebSocketClient
 from typing import List
 import asyncio
 
 from cfg import YOUR_API_KEY
-from polygon_finance.polygon_sdk.mapping_dicts import stock_condition_dict, STOCK_EXCHANGES, TAPES, quote_conditions, indicators
-from polygon_finance.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
+from polygon_finance.sdks.polygon_sdk.mapping_dicts import stock_condition_dict, STOCK_EXCHANGES, TAPES, quote_conditions, indicators
+from polygon_finance.sdks.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
 
 from asyncio import Queue
 import csv
 
 from discord_webhook import AsyncDiscordWebhook, DiscordEmbed
 
 poly = AsyncPolygonSDK(YOUR_API_KEY) #create instance of polygon SDK
```

### Comparing `polygon_finance-1.0.5/polygon_finance/examples/simulated_markets/helpers.py` & `polygon_finance-1.0.6/polygon_finance/examples/simulated_markets/helpers.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.5/polygon_finance/examples/simulated_markets/mock_discord.py` & `polygon_finance-1.0.6/polygon_finance/examples/simulated_markets/mock_discord.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 
 from typing import List
 import random
 import asyncio
 from datetime import datetime
 from polygon_finance.models.test_events import TestStocksEvent, STOCK_EXCHANGES
 
-from polygon_finance.polygon_sdk.mapping_dicts import stock_condition_dict
+from polygon_finance.sdks.polygon_sdk.mapping_dicts import stock_condition_dict
 
 import pandas as pd
 
-from polygon_finance.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
+from polygon_finance.sdks.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
 
 from cfg import YOUR_API_KEY
 
 from asyncio import Queue
 from discord.embeddings.embeds import Data
 
 sdk = AsyncPolygonSDK(YOUR_API_KEY)
```

### Comparing `polygon_finance-1.0.5/polygon_finance/examples/simulated_markets/mock_market.py` & `polygon_finance-1.0.6/polygon_finance/examples/simulated_markets/mock_market.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,115 +15,116 @@
 000000e0: 6e5f 6669 6e61 6e63 652e 6d6f 6465 6c73  n_finance.models
 000000f0: 2e74 6573 745f 6576 656e 7473 2069 6d70  .test_events imp
 00000100: 6f72 7420 5465 7374 5374 6f63 6b73 4576  ort TestStocksEv
 00000110: 656e 742c 2045 5155 4954 595f 5452 4144  ent, EQUITY_TRAD
 00000120: 455f 434f 4e44 4954 494f 4e53 0d0a 696d  E_CONDITIONS..im
 00000130: 706f 7274 2070 616e 6461 7320 6173 2070  port pandas as p
 00000140: 640d 0a0d 0a66 726f 6d20 706f 6c79 676f  d....from polygo
-00000150: 6e5f 6669 6e61 6e63 652e 706f 6c79 676f  n_finance.polygo
-00000160: 6e5f 7364 6b2e 6173 796e 635f 706f 6c79  n_sdk.async_poly
-00000170: 676f 6e5f 7364 6b20 696d 706f 7274 2041  gon_sdk import A
-00000180: 7379 6e63 506f 6c79 676f 6e53 444b 0d0a  syncPolygonSDK..
-00000190: 0d0a 6672 6f6d 2063 6667 2069 6d70 6f72  ..from cfg impor
-000001a0: 7420 594f 5552 5f41 5049 5f4b 4559 0d0a  t YOUR_API_KEY..
-000001b0: 0d0a 6672 6f6d 2061 7379 6e63 696f 2069  ..from asyncio i
-000001c0: 6d70 6f72 7420 5175 6575 650d 0a0d 0a0d  mport Queue.....
-000001d0: 0a73 646b 203d 2041 7379 6e63 506f 6c79  .sdk = AsyncPoly
-000001e0: 676f 6e53 444b 2859 4f55 525f 4150 495f  gonSDK(YOUR_API_
-000001f0: 4b45 5929 0d0a 6466 203d 2070 642e 7265  KEY)..df = pd.re
-00000200: 6164 5f63 7376 2827 6669 6c65 732f 7374  ad_csv('files/st
-00000210: 6f63 6b73 2f61 6c6c 5f73 6e61 7073 686f  ocks/all_snapsho
-00000220: 7473 2e63 7376 2729 0d0a 0d0a 0d0a 0d0a  ts.csv')........
-00000230: 6173 796e 6320 6465 6620 636f 6e73 756d  async def consum
-00000240: 6528 7175 6575 653a 2051 7565 7565 293a  e(queue: Queue):
-00000250: 0d0a 2020 2020 7768 696c 6520 5472 7565  ..    while True
-00000260: 3a0d 0a20 2020 2020 2020 206d 203d 2061  :..        m = a
-00000270: 7761 6974 2071 7565 7565 2e67 6574 2829  wait queue.get()
-00000280: 0d0a 2020 2020 2020 2020 7072 696e 7428  ..        print(
-00000290: 6d29 0d0a 2020 2020 2020 2020 2320 6173  m)..        # as
-000002a0: 6b20 3d20 6d2e 6c61 7374 5f71 756f 7465  k = m.last_quote
-000002b0: 5f61 736b 5f70 7269 6365 0d0a 2020 2020  _ask_price..    
-000002c0: 2020 2020 2320 636c 6f73 6520 3d6d 2e63      # close =m.c
-000002d0: 6c6f 7365 0d0a 2020 2020 2020 2020 2320  lose..        # 
-000002e0: 6c6f 773d 6d2e 6c6f 770d 0a20 2020 2020  low=m.low..     
-000002f0: 2020 2023 206f 7065 6e20 3d20 6d2e 6f70     # open = m.op
-00000300: 656e 0d0a 2020 2020 2020 2020 2320 6869  en..        # hi
-00000310: 6768 203d 206d 2e68 6967 680d 0a20 2020  gh = m.high..   
-00000320: 2020 2020 2023 2076 6f6c 756d 6520 3d20       # volume = 
-00000330: 6d2e 766f 6c75 6d65 0d0a 2020 2020 2020  m.volume..      
-00000340: 2020 2320 7072 6576 5f76 6f6c 756d 6520    # prev_volume 
-00000350: 3d20 6d2e 7072 6576 5f76 6f6c 756d 650d  = m.prev_volume.
-00000360: 0a20 2020 2020 2020 2023 2070 7265 765f  .        # prev_
-00000370: 7677 6170 203d 206d 2e70 7265 765f 7677  vwap = m.prev_vw
-00000380: 6170 0d0a 2020 2020 2020 2020 2320 7677  ap..        # vw
-00000390: 6170 203d 206d 2e76 7761 700d 0a20 2020  ap = m.vwap..   
-000003a0: 2020 2020 2023 2062 6964 203d 206d 2e6c       # bid = m.l
-000003b0: 6173 745f 7175 6f74 655f 6269 645f 7072  ast_quote_bid_pr
-000003c0: 6963 650d 0a20 2020 2020 2020 2023 2063  ice..        # c
-000003d0: 6f6e 6469 7469 6f6e 7320 3d20 6d2e 6c61  onditions = m.la
-000003e0: 7374 5f74 7261 6465 5f63 6f6e 6469 7469  st_trade_conditi
-000003f0: 6f6e 730d 0a20 2020 2020 2020 2023 2070  ons..        # p
-00000400: 7269 6e74 286f 7065 6e2c 2068 6967 6829  rint(open, high)
-00000410: 0d0a 2020 2020 2020 2020 2320 5072 6f63  ..        # Proc
-00000420: 6573 7320 7468 6520 6576 656e 7420 6173  ess the event as
-00000430: 206e 6563 6573 7361 7279 0d0a 2020 2020   necessary..    
-00000440: 2020 2020 0d0a 2020 2020 2020 2020 0d0a      ..        ..
-00000450: 0d0a 6173 796e 6320 6465 6620 6861 6e64  ..async def hand
-00000460: 6c65 5f6d 7367 286d 7367 733a 204c 6973  le_msg(msgs: Lis
-00000470: 745b 5465 7374 5374 6f63 6b73 4576 656e  t[TestStocksEven
-00000480: 745d 2c20 7175 6575 653a 2051 7565 7565  t], queue: Queue
-00000490: 293a 0d0a 2020 2020 666f 7220 6d20 696e  ):..    for m in
-000004a0: 206d 7367 733a 0d0a 0d0a 2020 2020 2020   msgs:....      
-000004b0: 2020 0d0a 2020 2020 2020 2020 6177 6169    ..        awai
-000004c0: 7420 7175 6575 652e 7075 7428 6d29 0d0a  t queue.put(m)..
-000004d0: 0d0a 6173 796e 6320 6465 6620 7365 6e64  ..async def send
-000004e0: 5f6d 6573 7361 6765 7328 6861 6e64 6c65  _messages(handle
-000004f0: 722c 2071 7565 7565 293a 2020 2320 7061  r, queue):  # pa
-00000500: 7373 2071 7565 7565 2061 7320 616e 2061  ss queue as an a
-00000510: 7267 756d 656e 740d 0a20 2020 2077 6869  rgument..    whi
-00000520: 6c65 2054 7275 653a 0d0a 2020 2020 2020  le True:..      
-00000530: 2020 2320 5365 6c65 6374 2061 2072 616e    # Select a ran
-00000540: 646f 6d20 726f 7720 6672 6f6d 2074 6865  dom row from the
-00000550: 2044 6174 6146 7261 6d65 0d0a 2020 2020   DataFrame..    
-00000560: 2020 2020 696e 6465 7820 3d20 7261 6e64      index = rand
-00000570: 6f6d 2e72 616e 6469 6e74 2830 2c20 6c65  om.randint(0, le
-00000580: 6e28 6466 2920 2d20 3129 0d0a 2020 2020  n(df) - 1)..    
-00000590: 2020 2020 726f 7720 3d20 6466 2e69 6c6f      row = df.ilo
-000005a0: 635b 696e 6465 785d 0d0a 0d0a 2020 2020  c[index]....    
-000005b0: 2020 2020 2320 4372 6561 7465 2054 6573      # Create Tes
-000005c0: 7453 746f 636b 7345 7665 6e74 206f 626a  tStocksEvent obj
-000005d0: 6563 7420 6672 6f6d 2072 6f77 2064 6174  ect from row dat
-000005e0: 610d 0a20 2020 2020 2020 2065 7665 6e74  a..        event
-000005f0: 203d 2054 6573 7453 746f 636b 7345 7665   = TestStocksEve
-00000600: 6e74 2e66 726f 6d5f 726f 7728 726f 7729  nt.from_row(row)
-00000610: 0d0a 0d0a 2020 2020 2020 2020 2320 4361  ....        # Ca
-00000620: 6c6c 2074 6865 2068 616e 646c 6572 2077  ll the handler w
-00000630: 6974 6820 7468 6520 6d65 7373 6167 650d  ith the message.
-00000640: 0a20 2020 2020 2020 2061 7761 6974 2068  .        await h
-00000650: 616e 646c 6572 285b 6576 656e 745d 2c20  andler([event], 
-00000660: 7175 6575 6529 0d0a 2020 2020 2020 2020  queue)..        
-00000670: 6177 6169 7420 6173 796e 6369 6f2e 736c  await asyncio.sl
-00000680: 6565 7028 302e 3031 290d 0a0d 0a61 7379  eep(0.01)....asy
-00000690: 6e63 2064 6566 206d 6169 6e28 293a 0d0a  nc def main():..
-000006a0: 2020 2020 6461 7461 5f71 7565 7565 203d      data_queue =
-000006b0: 2051 7565 7565 2829 200d 0a0d 0a20 2020   Queue() ....   
-000006c0: 206e 756d 5f77 6f72 6b65 7273 203d 2031   num_workers = 1
-000006d0: 3520 2023 2061 646a 7573 7420 7468 6973  5  # adjust this
-000006e0: 2076 616c 7565 2062 6173 6564 206f 6e20   value based on 
-000006f0: 796f 7572 2072 6571 7569 7265 6d65 6e74  your requirement
-00000700: 730d 0a20 2020 2073 646b 5f74 6173 6b73  s..    sdk_tasks
-00000710: 203d 205b 0d0a 2020 2020 2020 2020 636f   = [..        co
-00000720: 6e73 756d 6528 6461 7461 5f71 7565 7565  nsume(data_queue
-00000730: 2920 666f 7220 5f20 696e 2072 616e 6765  ) for _ in range
-00000740: 286e 756d 5f77 6f72 6b65 7273 290d 0a20  (num_workers).. 
-00000750: 2020 205d 0d0a 0d0a 2020 2020 7364 6b5f     ]....    sdk_
-00000760: 7461 736b 732e 6170 7065 6e64 2861 7379  tasks.append(asy
-00000770: 6e63 696f 2e63 7265 6174 655f 7461 736b  ncio.create_task
-00000780: 2873 656e 645f 6d65 7373 6167 6573 2868  (send_messages(h
-00000790: 616e 646c 655f 6d73 672c 2064 6174 615f  andle_msg, data_
-000007a0: 7175 6575 6529 2929 0d0a 0d0a 2020 2020  queue)))....    
-000007b0: 6177 6169 7420 6173 796e 6369 6f2e 6761  await asyncio.ga
-000007c0: 7468 6572 282a 7364 6b5f 7461 736b 7329  ther(*sdk_tasks)
-000007d0: 2020 2320 696e 636c 7564 6520 636f 6e73    # include cons
-000007e0: 756d 655f 7461 736b 2069 6e20 6761 7468  ume_task in gath
-000007f0: 6572 2829 0d0a 0d0a 6173 796e 6369 6f2e  er()....asyncio.
-00000800: 7275 6e28 6d61 696e 2829 290d 0a         run(main())..
+00000150: 6e5f 6669 6e61 6e63 652e 7364 6b73 2e70  n_finance.sdks.p
+00000160: 6f6c 7967 6f6e 5f73 646b 2e61 7379 6e63  olygon_sdk.async
+00000170: 5f70 6f6c 7967 6f6e 5f73 646b 2069 6d70  _polygon_sdk imp
+00000180: 6f72 7420 4173 796e 6350 6f6c 7967 6f6e  ort AsyncPolygon
+00000190: 5344 4b0d 0a0d 0a66 726f 6d20 6366 6720  SDK....from cfg 
+000001a0: 696d 706f 7274 2059 4f55 525f 4150 495f  import YOUR_API_
+000001b0: 4b45 590d 0a0d 0a66 726f 6d20 6173 796e  KEY....from asyn
+000001c0: 6369 6f20 696d 706f 7274 2051 7565 7565  cio import Queue
+000001d0: 0d0a 0d0a 0d0a 7364 6b20 3d20 4173 796e  ......sdk = Asyn
+000001e0: 6350 6f6c 7967 6f6e 5344 4b28 594f 5552  cPolygonSDK(YOUR
+000001f0: 5f41 5049 5f4b 4559 290d 0a64 6620 3d20  _API_KEY)..df = 
+00000200: 7064 2e72 6561 645f 6373 7628 2766 696c  pd.read_csv('fil
+00000210: 6573 2f73 746f 636b 732f 616c 6c5f 736e  es/stocks/all_sn
+00000220: 6170 7368 6f74 732e 6373 7627 290d 0a0d  apshots.csv')...
+00000230: 0a0d 0a0d 0a61 7379 6e63 2064 6566 2063  .....async def c
+00000240: 6f6e 7375 6d65 2871 7565 7565 3a20 5175  onsume(queue: Qu
+00000250: 6575 6529 3a0d 0a20 2020 2077 6869 6c65  eue):..    while
+00000260: 2054 7275 653a 0d0a 2020 2020 2020 2020   True:..        
+00000270: 6d20 3d20 6177 6169 7420 7175 6575 652e  m = await queue.
+00000280: 6765 7428 290d 0a20 2020 2020 2020 2070  get()..        p
+00000290: 7269 6e74 286d 290d 0a20 2020 2020 2020  rint(m)..       
+000002a0: 2023 2061 736b 203d 206d 2e6c 6173 745f   # ask = m.last_
+000002b0: 7175 6f74 655f 6173 6b5f 7072 6963 650d  quote_ask_price.
+000002c0: 0a20 2020 2020 2020 2023 2063 6c6f 7365  .        # close
+000002d0: 203d 6d2e 636c 6f73 650d 0a20 2020 2020   =m.close..     
+000002e0: 2020 2023 206c 6f77 3d6d 2e6c 6f77 0d0a     # low=m.low..
+000002f0: 2020 2020 2020 2020 2320 6f70 656e 203d          # open =
+00000300: 206d 2e6f 7065 6e0d 0a20 2020 2020 2020   m.open..       
+00000310: 2023 2068 6967 6820 3d20 6d2e 6869 6768   # high = m.high
+00000320: 0d0a 2020 2020 2020 2020 2320 766f 6c75  ..        # volu
+00000330: 6d65 203d 206d 2e76 6f6c 756d 650d 0a20  me = m.volume.. 
+00000340: 2020 2020 2020 2023 2070 7265 765f 766f         # prev_vo
+00000350: 6c75 6d65 203d 206d 2e70 7265 765f 766f  lume = m.prev_vo
+00000360: 6c75 6d65 0d0a 2020 2020 2020 2020 2320  lume..        # 
+00000370: 7072 6576 5f76 7761 7020 3d20 6d2e 7072  prev_vwap = m.pr
+00000380: 6576 5f76 7761 700d 0a20 2020 2020 2020  ev_vwap..       
+00000390: 2023 2076 7761 7020 3d20 6d2e 7677 6170   # vwap = m.vwap
+000003a0: 0d0a 2020 2020 2020 2020 2320 6269 6420  ..        # bid 
+000003b0: 3d20 6d2e 6c61 7374 5f71 756f 7465 5f62  = m.last_quote_b
+000003c0: 6964 5f70 7269 6365 0d0a 2020 2020 2020  id_price..      
+000003d0: 2020 2320 636f 6e64 6974 696f 6e73 203d    # conditions =
+000003e0: 206d 2e6c 6173 745f 7472 6164 655f 636f   m.last_trade_co
+000003f0: 6e64 6974 696f 6e73 0d0a 2020 2020 2020  nditions..      
+00000400: 2020 2320 7072 696e 7428 6f70 656e 2c20    # print(open, 
+00000410: 6869 6768 290d 0a20 2020 2020 2020 2023  high)..        #
+00000420: 2050 726f 6365 7373 2074 6865 2065 7665   Process the eve
+00000430: 6e74 2061 7320 6e65 6365 7373 6172 790d  nt as necessary.
+00000440: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
+00000450: 2020 200d 0a0d 0a61 7379 6e63 2064 6566     ....async def
+00000460: 2068 616e 646c 655f 6d73 6728 6d73 6773   handle_msg(msgs
+00000470: 3a20 4c69 7374 5b54 6573 7453 746f 636b  : List[TestStock
+00000480: 7345 7665 6e74 5d2c 2071 7565 7565 3a20  sEvent], queue: 
+00000490: 5175 6575 6529 3a0d 0a20 2020 2066 6f72  Queue):..    for
+000004a0: 206d 2069 6e20 6d73 6773 3a0d 0a0d 0a20   m in msgs:.... 
+000004b0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+000004c0: 2061 7761 6974 2071 7565 7565 2e70 7574   await queue.put
+000004d0: 286d 290d 0a0d 0a61 7379 6e63 2064 6566  (m)....async def
+000004e0: 2073 656e 645f 6d65 7373 6167 6573 2868   send_messages(h
+000004f0: 616e 646c 6572 2c20 7175 6575 6529 3a20  andler, queue): 
+00000500: 2023 2070 6173 7320 7175 6575 6520 6173   # pass queue as
+00000510: 2061 6e20 6172 6775 6d65 6e74 0d0a 2020   an argument..  
+00000520: 2020 7768 696c 6520 5472 7565 3a0d 0a20    while True:.. 
+00000530: 2020 2020 2020 2023 2053 656c 6563 7420         # Select 
+00000540: 6120 7261 6e64 6f6d 2072 6f77 2066 726f  a random row fro
+00000550: 6d20 7468 6520 4461 7461 4672 616d 650d  m the DataFrame.
+00000560: 0a20 2020 2020 2020 2069 6e64 6578 203d  .        index =
+00000570: 2072 616e 646f 6d2e 7261 6e64 696e 7428   random.randint(
+00000580: 302c 206c 656e 2864 6629 202d 2031 290d  0, len(df) - 1).
+00000590: 0a20 2020 2020 2020 2072 6f77 203d 2064  .        row = d
+000005a0: 662e 696c 6f63 5b69 6e64 6578 5d0d 0a0d  f.iloc[index]...
+000005b0: 0a20 2020 2020 2020 2023 2043 7265 6174  .        # Creat
+000005c0: 6520 5465 7374 5374 6f63 6b73 4576 656e  e TestStocksEven
+000005d0: 7420 6f62 6a65 6374 2066 726f 6d20 726f  t object from ro
+000005e0: 7720 6461 7461 0d0a 2020 2020 2020 2020  w data..        
+000005f0: 6576 656e 7420 3d20 5465 7374 5374 6f63  event = TestStoc
+00000600: 6b73 4576 656e 742e 6672 6f6d 5f72 6f77  ksEvent.from_row
+00000610: 2872 6f77 290d 0a0d 0a20 2020 2020 2020  (row)....       
+00000620: 2023 2043 616c 6c20 7468 6520 6861 6e64   # Call the hand
+00000630: 6c65 7220 7769 7468 2074 6865 206d 6573  ler with the mes
+00000640: 7361 6765 0d0a 2020 2020 2020 2020 6177  sage..        aw
+00000650: 6169 7420 6861 6e64 6c65 7228 5b65 7665  ait handler([eve
+00000660: 6e74 5d2c 2071 7565 7565 290d 0a20 2020  nt], queue)..   
+00000670: 2020 2020 2061 7761 6974 2061 7379 6e63       await async
+00000680: 696f 2e73 6c65 6570 2830 2e30 3129 0d0a  io.sleep(0.01)..
+00000690: 0d0a 6173 796e 6320 6465 6620 6d61 696e  ..async def main
+000006a0: 2829 3a0d 0a20 2020 2064 6174 615f 7175  ():..    data_qu
+000006b0: 6575 6520 3d20 5175 6575 6528 2920 0d0a  eue = Queue() ..
+000006c0: 0d0a 2020 2020 6e75 6d5f 776f 726b 6572  ..    num_worker
+000006d0: 7320 3d20 3135 2020 2320 6164 6a75 7374  s = 15  # adjust
+000006e0: 2074 6869 7320 7661 6c75 6520 6261 7365   this value base
+000006f0: 6420 6f6e 2079 6f75 7220 7265 7175 6972  d on your requir
+00000700: 656d 656e 7473 0d0a 2020 2020 7364 6b5f  ements..    sdk_
+00000710: 7461 736b 7320 3d20 5b0d 0a20 2020 2020  tasks = [..     
+00000720: 2020 2063 6f6e 7375 6d65 2864 6174 615f     consume(data_
+00000730: 7175 6575 6529 2066 6f72 205f 2069 6e20  queue) for _ in 
+00000740: 7261 6e67 6528 6e75 6d5f 776f 726b 6572  range(num_worker
+00000750: 7329 0d0a 2020 2020 5d0d 0a0d 0a20 2020  s)..    ]....   
+00000760: 2073 646b 5f74 6173 6b73 2e61 7070 656e   sdk_tasks.appen
+00000770: 6428 6173 796e 6369 6f2e 6372 6561 7465  d(asyncio.create
+00000780: 5f74 6173 6b28 7365 6e64 5f6d 6573 7361  _task(send_messa
+00000790: 6765 7328 6861 6e64 6c65 5f6d 7367 2c20  ges(handle_msg, 
+000007a0: 6461 7461 5f71 7565 7565 2929 290d 0a0d  data_queue)))...
+000007b0: 0a20 2020 2061 7761 6974 2061 7379 6e63  .    await async
+000007c0: 696f 2e67 6174 6865 7228 2a73 646b 5f74  io.gather(*sdk_t
+000007d0: 6173 6b73 2920 2023 2069 6e63 6c75 6465  asks)  # include
+000007e0: 2063 6f6e 7375 6d65 5f74 6173 6b20 696e   consume_task in
+000007f0: 2067 6174 6865 7228 290d 0a0d 0a61 7379   gather()....asy
+00000800: 6e63 696f 2e72 756e 286d 6169 6e28 2929  ncio.run(main())
+00000810: 0d0a                                     ..
```

### Comparing `polygon_finance-1.0.5/polygon_finance/examples/simulated_markets/mock_options_market.py` & `polygon_finance-1.0.6/polygon_finance/examples/simulated_markets/mock_options_market.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from asyncio import Queue
 from datetime import datetime
 from dataclasses import asdict
 from polygon_finance.models.test_events import TestOptionsEvent, option_condition_dict, OPTIONS_EXCHANGES
 import pandas as pd
 
 
-from polygon_finance.polygon_sdk.async_options_sdk import PolygonOptionsSDK
+from polygon_finance.sdks.polygon_sdk.async_options_sdk import PolygonOptionsSDK
 from cfg import YOUR_API_KEY
 
 sdk= PolygonOptionsSDK(YOUR_API_KEY)
 
 
 
 df = pd.read_csv('files/options/all_options_data.csv')
```

### Comparing `polygon_finance-1.0.5/polygon_finance/examples/stock_aggregates.py` & `polygon_finance-1.0.6/polygon_finance/examples/stock_aggregates.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 sys.path.append(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
 
 import asyncio
 import pandas as pd
 
-from polygon_finance.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
+from polygon_finance.sdks.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
 from cfg import YOUR_API_KEY, five_days_ago_str, today_str
 
 polygonsdk = AsyncPolygonSDK(YOUR_API_KEY)
 ticker = "GME"
 
 async def stock_aggregates_example(ticker):
     """
```

### Comparing `polygon_finance-1.0.5/polygon_finance/examples/summarizer.py` & `polygon_finance-1.0.6/polygon_finance/examples/summarizer.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.5/polygon_finance/examples/support_resistance.py` & `polygon_finance-1.0.6/polygon_finance/examples/support_resistance.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 import os
 
 sys.path.append(os.path.dirname(os.path.dirname(os.path.dirname(os.path.abspath(__file__)))))
 
 
 import asyncio
-from polygon_finance.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
+from polygon_finance.sdks.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
 from cfg import YOUR_API_KEY, five_days_ago_str, today_str
 
 polygonsdk = AsyncPolygonSDK(YOUR_API_KEY)
 ticker = "GME"
 
 async def support_resistance_example(ticker):
     """
```

### Comparing `polygon_finance-1.0.5/polygon_finance/models/test_events.py` & `polygon_finance-1.0.6/polygon_finance/models/test_events.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.5/polygon_finance/sdks/discord_sdk/discord_sdk.py` & `polygon_finance-1.0.6/polygon_finance/sdks/discord_sdk/discord_sdk.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.5/polygon_finance/sdks/discord_sdk/searching.py` & `polygon_finance-1.0.6/polygon_finance/sdks/discord_sdk/searching.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.5/polygon_finance/sdks/fudstop_sdk/fudstop_sdk.py` & `polygon_finance-1.0.6/polygon_finance/sdks/fudstop_sdk/fudstop_sdk.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.5/polygon_finance/sdks/fudstop_sdk/gaps.py` & `polygon_finance-1.0.6/polygon_finance/sdks/fudstop_sdk/gaps.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.5/polygon_finance/sdks/polygon_sdk/aggregates.py` & `polygon_finance-1.0.6/polygon_finance/sdks/polygon_sdk/aggregates.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.5/polygon_finance/sdks/polygon_sdk/async_options_sdk.py` & `polygon_finance-1.0.6/polygon_finance/sdks/polygon_sdk/async_options_sdk.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.5/polygon_finance/sdks/polygon_sdk/async_polygon_sdk.py` & `polygon_finance-1.0.6/polygon_finance/sdks/polygon_sdk/async_polygon_sdk.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.5/polygon_finance/sdks/polygon_sdk/daily_open_close.py` & `polygon_finance-1.0.6/polygon_finance/sdks/polygon_sdk/daily_open_close.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.5/polygon_finance/sdks/polygon_sdk/financials.py` & `polygon_finance-1.0.6/polygon_finance/sdks/polygon_sdk/financials.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.5/polygon_finance/sdks/polygon_sdk/forex_crypto.py` & `polygon_finance-1.0.6/polygon_finance/sdks/polygon_sdk/forex_crypto.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.5/polygon_finance/sdks/polygon_sdk/get_all_options.py` & `polygon_finance-1.0.6/polygon_finance/sdks/polygon_sdk/get_all_options.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.5/polygon_finance/sdks/polygon_sdk/indices_snapshot.py` & `polygon_finance-1.0.6/polygon_finance/sdks/polygon_sdk/indices_snapshot.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.5/polygon_finance/sdks/polygon_sdk/logo.py` & `polygon_finance-1.0.6/polygon_finance/sdks/polygon_sdk/logo.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.5/polygon_finance/sdks/polygon_sdk/mapping_dicts.py` & `polygon_finance-1.0.6/polygon_finance/sdks/polygon_sdk/mapping_dicts.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.5/polygon_finance/sdks/polygon_sdk/models.py` & `polygon_finance-1.0.6/polygon_finance/sdks/polygon_sdk/models.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.5/polygon_finance/sdks/polygon_sdk/news.py` & `polygon_finance-1.0.6/polygon_finance/sdks/polygon_sdk/news.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.5/polygon_finance/sdks/polygon_sdk/option_aggs.py` & `polygon_finance-1.0.6/polygon_finance/sdks/polygon_sdk/option_aggs.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.5/polygon_finance/sdks/polygon_sdk/option_quote.py` & `polygon_finance-1.0.6/polygon_finance/sdks/polygon_sdk/option_quote.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.5/polygon_finance/sdks/polygon_sdk/option_snapshot.py` & `polygon_finance-1.0.6/polygon_finance/sdks/polygon_sdk/option_snapshot.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.5/polygon_finance/sdks/polygon_sdk/option_trades.py` & `polygon_finance-1.0.6/polygon_finance/sdks/polygon_sdk/option_trades.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.5/polygon_finance/sdks/polygon_sdk/pivot_points.py` & `polygon_finance-1.0.6/polygon_finance/sdks/polygon_sdk/pivot_points.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.5/polygon_finance/sdks/polygon_sdk/quote.py` & `polygon_finance-1.0.6/polygon_finance/sdks/polygon_sdk/quote.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.5/polygon_finance/sdks/polygon_sdk/snapshot.py` & `polygon_finance-1.0.6/polygon_finance/sdks/polygon_sdk/snapshot.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.5/polygon_finance/sdks/polygon_sdk/technical_conditions.py` & `polygon_finance-1.0.6/polygon_finance/sdks/polygon_sdk/technical_conditions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from polygon_finance.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
+from polygon_finance.sdks.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
 from cfg import YOUR_API_KEY
 polygon = AsyncPolygonSDK(YOUR_API_KEY)
 from asyncio import Semaphore
 
 sem = Semaphore()
```

### Comparing `polygon_finance-1.0.5/polygon_finance/sdks/polygon_sdk/tickernews.py` & `polygon_finance-1.0.6/polygon_finance/sdks/polygon_sdk/tickernews.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.5/polygon_finance/sdks/webull_sdk/calendar.py` & `polygon_finance-1.0.6/polygon_finance/sdks/webull_sdk/calendar.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.5/polygon_finance/sdks/webull_sdk/capitalflow.py` & `polygon_finance-1.0.6/polygon_finance/sdks/webull_sdk/capitalflow.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.5/polygon_finance/sdks/webull_sdk/cost_distribution.py` & `polygon_finance-1.0.6/polygon_finance/sdks/webull_sdk/cost_distribution.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.5/polygon_finance/sdks/webull_sdk/derivative_query.py` & `polygon_finance-1.0.6/polygon_finance/sdks/webull_sdk/derivative_query.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.5/polygon_finance/sdks/webull_sdk/etf_finder.py` & `polygon_finance-1.0.6/polygon_finance/sdks/webull_sdk/etf_finder.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.5/polygon_finance/sdks/webull_sdk/events.py` & `polygon_finance-1.0.6/polygon_finance/sdks/webull_sdk/events.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.5/polygon_finance/sdks/webull_sdk/financial_statement.py` & `polygon_finance-1.0.6/polygon_finance/sdks/webull_sdk/financial_statement.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.5/polygon_finance/sdks/webull_sdk/forecast.py` & `polygon_finance-1.0.6/polygon_finance/sdks/webull_sdk/forecast.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.5/polygon_finance/sdks/webull_sdk/institutional_holdings.py` & `polygon_finance-1.0.6/polygon_finance/sdks/webull_sdk/institutional_holdings.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.5/polygon_finance/sdks/webull_sdk/manage.py` & `polygon_finance-1.0.6/polygon_finance/sdks/webull_sdk/manage.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.5/polygon_finance/sdks/webull_sdk/news.py` & `polygon_finance-1.0.6/polygon_finance/sdks/webull_sdk/news.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.5/polygon_finance/sdks/webull_sdk/top_gainers.py` & `polygon_finance-1.0.6/polygon_finance/sdks/webull_sdk/top_gainers.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.5/polygon_finance/sdks/webull_sdk/top_options.py` & `polygon_finance-1.0.6/polygon_finance/sdks/webull_sdk/top_options.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.5/polygon_finance/sdks/webull_sdk/webull_data.py` & `polygon_finance-1.0.6/polygon_finance/sdks/webull_sdk/webull_data.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.5/polygon_finance/sdks/webull_sdk/webull_sdk.py` & `polygon_finance-1.0.6/polygon_finance/sdks/webull_sdk/webull_sdk.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.5/polygon_finance/start_here.py` & `polygon_finance-1.0.6/polygon_finance/start_here.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 """
 #from get_data.get_all_options_data import get_all_options_data
 #from get_data.get_latest_crypto_data import get_all_crypto_data
 #from get_data.get_latest_forex_data import get_forex_data
 #from get_data.get_latest_indices_data import get_all_indices_data
 from get_data.get_latest_ticker_data import get_all_ticker_data
 
-from polygon_finance.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
-from polygon_finance.polygon_sdk.async_options_sdk import PolygonOptionsSDK
+from polygon_finance.sdks.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
+from polygon_finance.sdks.polygon_sdk.async_options_sdk import PolygonOptionsSDK
 
 from cfg import YOUR_API_KEY, today_str
 
 poly = AsyncPolygonSDK(YOUR_API_KEY)
 polyoptions = PolygonOptionsSDK(YOUR_API_KEY)
```

### Comparing `polygon_finance-1.0.5/polygon_finance/terminals/crypto/crypto_terminal.py` & `polygon_finance-1.0.6/polygon_finance/terminals/crypto/crypto_terminal.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 sys.path.append(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
 
 from terminals.crypto.menu import menu
 import asyncio
 from typing import List
 from polygon.websocket import WebSocketClient, WebSocketMessage, CryptoQuote, CryptoTrade, Market
-from polygon_finance.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
+from polygon_finance.sdks.polygon_sdk.async_polygon_sdk import AsyncPolygonSDK
 from cachetools import TTLCache
 
 import threading
 import sqlite3
 from sqlite3 import Error
 
 from cfg import YOUR_API_KEY
```

### Comparing `polygon_finance-1.0.5/polygon_finance/terminals/crypto/menu.py` & `polygon_finance-1.0.6/polygon_finance/terminals/crypto/menu.py`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.5/polygon_finance.egg-info/SOURCES.txt` & `polygon_finance-1.0.6/polygon_finance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.5/polygon_finance.egg-info/requires.txt` & `polygon_finance-1.0.6/polygon_finance.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `polygon_finance-1.0.5/setup.py` & `polygon_finance-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='polygon_finance',
-    version='1.0.5',
+    version='1.0.6',
     description='The real-time market analysis library that utilizes the real-time rest apis and websockets from polygon.io',
     author='Charlies Vids',
     author_email='chuckdustin12@gmail.com',
     packages=find_packages(),
     install_requires=[
         'aiofiles==23.1.0',
         'aiohttp==3.8.4',
```

