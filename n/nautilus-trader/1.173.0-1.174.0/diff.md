# Comparing `tmp/nautilus_trader-1.173.0.tar.gz` & `tmp/nautilus_trader-1.174.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nautilus_trader-1.173.0.tar", max compression
+gzip compressed data, was "nautilus_trader-1.174.0.tar", max compression
```

## Comparing `nautilus_trader-1.173.0.tar` & `nautilus_trader-1.174.0.tar`

### file list

```diff
@@ -1,703 +1,711 @@
--rw-r--r--   0        0        0     7652 2023-05-05 11:18:34.833063 nautilus_trader-1.173.0/LICENSE
--rw-r--r--   0        0        0    23501 2023-05-05 11:18:34.833063 nautilus_trader-1.173.0/README.md
--rw-r--r--   0        0        0    12351 2023-05-05 11:18:34.833063 nautilus_trader-1.173.0/build.py
--rw-r--r--   0        0        0      663 2023-05-05 11:18:34.849063 nautilus_trader-1.173.0/nautilus_core/.cargo/config.toml
--rw-r--r--   0        0        0       65 2023-05-05 11:18:34.849063 nautilus_trader-1.173.0/nautilus_core/.clippy.toml
--rw-r--r--   0        0        0       37 2023-05-05 11:18:34.849063 nautilus_trader-1.173.0/nautilus_core/.rustfmt.toml
--rw-r--r--   0        0        0    81280 2023-05-05 11:18:34.849063 nautilus_trader-1.173.0/nautilus_core/Cargo.lock
--rw-r--r--   0        0        0     1631 2023-05-05 11:18:34.849063 nautilus_trader-1.173.0/nautilus_core/Cargo.toml
--rw-r--r--   0        0        0     7652 2023-05-05 11:18:34.849063 nautilus_trader-1.173.0/nautilus_core/LICENSE
--rw-r--r--   0        0        0     1248 2023-05-05 11:18:34.849063 nautilus_trader-1.173.0/nautilus_core/README.md
--rw-r--r--   0        0        0      702 2023-05-05 11:18:34.849063 nautilus_trader-1.173.0/nautilus_core/backtest/Cargo.toml
--rw-r--r--   0        0        0     1889 2023-05-05 11:18:34.849063 nautilus_trader-1.173.0/nautilus_core/backtest/build.rs
--rw-r--r--   0        0        0      484 2023-05-05 11:18:34.849063 nautilus_trader-1.173.0/nautilus_core/backtest/cbindgen.toml
--rw-r--r--   0        0        0      788 2023-05-05 11:18:34.849063 nautilus_trader-1.173.0/nautilus_core/backtest/cbindgen_cython.toml
--rw-r--r--   0        0        0     5787 2023-05-05 11:18:34.849063 nautilus_trader-1.173.0/nautilus_core/backtest/src/engine.rs
--rw-r--r--   0        0        0      900 2023-05-05 11:18:34.849063 nautilus_trader-1.173.0/nautilus_core/backtest/src/lib.rs
--rw-r--r--   0        0        0      715 2023-05-05 11:18:34.849063 nautilus_trader-1.173.0/nautilus_core/common/Cargo.toml
--rw-r--r--   0        0        0     2555 2023-05-05 11:18:34.849063 nautilus_trader-1.173.0/nautilus_core/common/build.rs
--rw-r--r--   0        0        0      531 2023-05-05 11:18:34.849063 nautilus_trader-1.173.0/nautilus_core/common/cbindgen.toml
--rw-r--r--   0        0        0      724 2023-05-05 11:18:34.849063 nautilus_trader-1.173.0/nautilus_core/common/cbindgen_cython.toml
--rw-r--r--   0        0        0    25300 2023-05-05 11:18:34.849063 nautilus_trader-1.173.0/nautilus_core/common/src/clock.rs
--rw-r--r--   0        0        0     6296 2023-05-05 11:18:34.849063 nautilus_trader-1.173.0/nautilus_core/common/src/enums.rs
--rw-r--r--   0        0        0      979 2023-05-05 11:18:34.853062 nautilus_trader-1.173.0/nautilus_core/common/src/lib.rs
--rw-r--r--   0        0        0    25116 2023-05-05 11:18:34.853062 nautilus_trader-1.173.0/nautilus_core/common/src/logging.rs
--rw-r--r--   0        0        0     7311 2023-05-05 11:18:34.853062 nautilus_trader-1.173.0/nautilus_core/common/src/msgbus.rs
--rw-r--r--   0        0        0     1299 2023-05-05 11:18:34.853062 nautilus_trader-1.173.0/nautilus_core/common/src/testing.rs
--rw-r--r--   0        0        0     8979 2023-05-05 11:18:34.853062 nautilus_trader-1.173.0/nautilus_core/common/src/timer.rs
--rw-r--r--   0        0        0     3091 2023-05-05 11:18:34.853062 nautilus_trader-1.173.0/nautilus_core/common/tests/test_clock.rs
--rw-r--r--   0        0        0      616 2023-05-05 11:18:34.853062 nautilus_trader-1.173.0/nautilus_core/core/Cargo.toml
--rw-r--r--   0        0        0     1234 2023-05-05 11:18:34.853062 nautilus_trader-1.173.0/nautilus_core/core/benches/criterion_time_benchmark.rs
--rw-r--r--   0        0        0     2551 2023-05-05 11:18:34.853062 nautilus_trader-1.173.0/nautilus_core/core/build.rs
--rw-r--r--   0        0        0      681 2023-05-05 11:18:34.853062 nautilus_trader-1.173.0/nautilus_core/core/cbindgen.toml
--rw-r--r--   0        0        0      791 2023-05-05 11:18:34.853062 nautilus_trader-1.173.0/nautilus_core/core/cbindgen_cython.toml
--rw-r--r--   0        0        0     7634 2023-05-05 11:18:34.853062 nautilus_trader-1.173.0/nautilus_core/core/src/correctness.rs
--rw-r--r--   0        0        0     5262 2023-05-05 11:18:34.853062 nautilus_trader-1.173.0/nautilus_core/core/src/cvec.rs
--rw-r--r--   0        0        0     5256 2023-05-05 11:18:34.853062 nautilus_trader-1.173.0/nautilus_core/core/src/datetime.rs
--rw-r--r--   0        0        0      998 2023-05-05 11:18:34.853062 nautilus_trader-1.173.0/nautilus_core/core/src/lib.rs
--rw-r--r--   0        0        0     4973 2023-05-05 11:18:34.853062 nautilus_trader-1.173.0/nautilus_core/core/src/parsing.rs
--rw-r--r--   0        0        0     5119 2023-05-05 11:18:34.853062 nautilus_trader-1.173.0/nautilus_core/core/src/string.rs
--rw-r--r--   0        0        0     5105 2023-05-05 11:18:34.853062 nautilus_trader-1.173.0/nautilus_core/core/src/time.rs
--rw-r--r--   0        0        0     7352 2023-05-05 11:18:34.853062 nautilus_trader-1.173.0/nautilus_core/core/src/uuid.rs
--rw-r--r--   0        0        0      497 2023-05-05 11:18:34.853062 nautilus_trader-1.173.0/nautilus_core/indicators/Cargo.toml
--rw-r--r--   0        0        0     4125 2023-05-05 11:18:34.853062 nautilus_trader-1.173.0/nautilus_core/indicators/src/ema.rs
--rw-r--r--   0        0        0     1289 2023-05-05 11:18:34.853062 nautilus_trader-1.173.0/nautilus_core/indicators/src/lib.rs
--rw-r--r--   0        0        0      791 2023-05-05 11:18:34.853062 nautilus_trader-1.173.0/nautilus_core/model/Cargo.toml
--rw-r--r--   0        0        0      399 2023-05-05 11:18:34.853062 nautilus_trader-1.173.0/nautilus_core/model/benches/criterion_fixed_precision_benchmark.rs
--rw-r--r--   0        0        0      223 2023-05-05 11:18:34.853062 nautilus_trader-1.173.0/nautilus_core/model/benches/iai_fixed_precision_benchmark.rs
--rw-r--r--   0        0        0     2553 2023-05-05 11:18:34.853062 nautilus_trader-1.173.0/nautilus_core/model/build.rs
--rw-r--r--   0        0        0     1084 2023-05-05 11:18:34.853062 nautilus_trader-1.173.0/nautilus_core/model/cbindgen.toml
--rw-r--r--   0        0        0     1237 2023-05-05 11:18:34.853062 nautilus_trader-1.173.0/nautilus_core/model/cbindgen_cython.toml
--rw-r--r--   0        0        0    21348 2023-05-05 11:18:34.853062 nautilus_trader-1.173.0/nautilus_core/model/src/currencies.rs
--rw-r--r--   0        0        0    14247 2023-05-05 11:18:34.853062 nautilus_trader-1.173.0/nautilus_core/model/src/data/bar.rs
--rw-r--r--   0        0        0      911 2023-05-05 11:18:34.853062 nautilus_trader-1.173.0/nautilus_core/model/src/data/mod.rs
--rw-r--r--   0        0        0     9638 2023-05-05 11:18:34.853062 nautilus_trader-1.173.0/nautilus_core/model/src/data/tick.rs
--rw-r--r--   0        0        0    21928 2023-05-05 11:18:34.853062 nautilus_trader-1.173.0/nautilus_core/model/src/enums.rs
--rw-r--r--   0        0        0      917 2023-05-05 11:18:34.853062 nautilus_trader-1.173.0/nautilus_core/model/src/events/mod.rs
--rw-r--r--   0        0        0    10609 2023-05-05 11:18:34.853062 nautilus_trader-1.173.0/nautilus_core/model/src/events/order.rs
--rw-r--r--   0        0        0     3681 2023-05-05 11:18:34.853062 nautilus_trader-1.173.0/nautilus_core/model/src/events/position.rs
--rw-r--r--   0        0        0     7344 2023-05-05 11:18:34.853062 nautilus_trader-1.173.0/nautilus_core/model/src/identifiers/account_id.rs
--rw-r--r--   0        0        0     4806 2023-05-05 11:18:34.853062 nautilus_trader-1.173.0/nautilus_core/model/src/identifiers/client_id.rs
--rw-r--r--   0        0        0     4034 2023-05-05 11:18:34.853062 nautilus_trader-1.173.0/nautilus_core/model/src/identifiers/client_order_id.rs
--rw-r--r--   0        0        0     3839 2023-05-05 11:18:34.853062 nautilus_trader-1.173.0/nautilus_core/model/src/identifiers/component_id.rs
--rw-r--r--   0        0        0     3981 2023-05-05 11:18:34.853062 nautilus_trader-1.173.0/nautilus_core/model/src/identifiers/exec_algorithm_id.rs
--rw-r--r--   0        0        0     4602 2023-05-05 11:18:34.853062 nautilus_trader-1.173.0/nautilus_core/model/src/identifiers/instrument_id.rs
--rw-r--r--   0        0        0     1177 2023-05-05 11:18:34.853062 nautilus_trader-1.173.0/nautilus_core/model/src/identifiers/mod.rs
--rw-r--r--   0        0        0     3813 2023-05-05 11:18:34.853062 nautilus_trader-1.173.0/nautilus_core/model/src/identifiers/order_list_id.rs
--rw-r--r--   0        0        0     3804 2023-05-05 11:18:34.853062 nautilus_trader-1.173.0/nautilus_core/model/src/identifiers/position_id.rs
--rw-r--r--   0        0        0     3553 2023-05-05 11:18:34.853062 nautilus_trader-1.173.0/nautilus_core/model/src/identifiers/strategy_id.rs
--rw-r--r--   0        0        0     3642 2023-05-05 11:18:34.853062 nautilus_trader-1.173.0/nautilus_core/model/src/identifiers/symbol.rs
--rw-r--r--   0        0        0     3725 2023-05-05 11:18:34.853062 nautilus_trader-1.173.0/nautilus_core/model/src/identifiers/trade_id.rs
--rw-r--r--   0        0        0     3495 2023-05-05 11:18:34.853062 nautilus_trader-1.173.0/nautilus_core/model/src/identifiers/trader_id.rs
--rw-r--r--   0        0        0     3602 2023-05-05 11:18:34.853062 nautilus_trader-1.173.0/nautilus_core/model/src/identifiers/venue.rs
--rw-r--r--   0        0        0     3994 2023-05-05 11:18:34.853062 nautilus_trader-1.173.0/nautilus_core/model/src/identifiers/venue_order_id.rs
--rw-r--r--   0        0        0     1831 2023-05-05 11:18:34.853062 nautilus_trader-1.173.0/nautilus_core/model/src/instruments/mod.rs
--rw-r--r--   0        0        0     1357 2023-05-05 11:18:34.853062 nautilus_trader-1.173.0/nautilus_core/model/src/lib.rs
--rw-r--r--   0        0        0     3064 2023-05-05 11:18:34.853062 nautilus_trader-1.173.0/nautilus_core/model/src/orderbook/book.rs
--rw-r--r--   0        0        0    12946 2023-05-05 11:18:34.853062 nautilus_trader-1.173.0/nautilus_core/model/src/orderbook/ladder.rs
--rw-r--r--   0        0        0     7607 2023-05-05 11:18:34.853062 nautilus_trader-1.173.0/nautilus_core/model/src/orderbook/level.rs
--rw-r--r--   0        0        0      944 2023-05-05 11:18:34.853062 nautilus_trader-1.173.0/nautilus_core/model/src/orderbook/mod.rs
--rw-r--r--   0        0        0     2646 2023-05-05 11:18:34.853062 nautilus_trader-1.173.0/nautilus_core/model/src/orderbook/order.rs
--rw-r--r--   0        0        0     4703 2023-05-05 11:18:34.857063 nautilus_trader-1.173.0/nautilus_core/model/src/orders/limit.rs
--rw-r--r--   0        0        0    33212 2023-05-05 11:18:34.857063 nautilus_trader-1.173.0/nautilus_core/model/src/orders/mod.rs
--rw-r--r--   0        0        0     7517 2023-05-05 11:18:34.857063 nautilus_trader-1.173.0/nautilus_core/model/src/position.rs
--rw-r--r--   0        0        0     1341 2023-05-05 11:18:34.857063 nautilus_trader-1.173.0/nautilus_core/model/src/types/balance.rs
--rw-r--r--   0        0        0     5223 2023-05-05 11:18:34.857063 nautilus_trader-1.173.0/nautilus_core/model/src/types/currency.rs
--rw-r--r--   0        0        0     5917 2023-05-05 11:18:34.857063 nautilus_trader-1.173.0/nautilus_core/model/src/types/fixed.rs
--rw-r--r--   0        0        0      982 2023-05-05 11:18:34.857063 nautilus_trader-1.173.0/nautilus_core/model/src/types/mod.rs
--rw-r--r--   0        0        0     7403 2023-05-05 11:18:34.857063 nautilus_trader-1.173.0/nautilus_core/model/src/types/money.rs
--rw-r--r--   0        0        0     9986 2023-05-05 11:18:34.857063 nautilus_trader-1.173.0/nautilus_core/model/src/types/price.rs
--rw-r--r--   0        0        0    10136 2023-05-05 11:18:34.857063 nautilus_trader-1.173.0/nautilus_core/model/src/types/quantity.rs
--rw-r--r--   0        0        0      500 2023-05-05 11:18:34.857063 nautilus_trader-1.173.0/nautilus_core/network/Cargo.toml
--rw-r--r--   0        0        0      883 2023-05-05 11:18:34.857063 nautilus_trader-1.173.0/nautilus_core/network/src/lib.rs
--rw-r--r--   0        0        0      947 2023-05-05 11:18:34.857063 nautilus_trader-1.173.0/nautilus_core/persistence/Cargo.toml
--rw-r--r--   0        0        0     5948 2023-05-05 11:18:34.857063 nautilus_trader-1.173.0/nautilus_core/persistence/src/kmerge_batch.rs
--rw-r--r--   0        0        0     1279 2023-05-05 11:18:34.857063 nautilus_trader-1.173.0/nautilus_core/persistence/src/lib.rs
--rw-r--r--   0        0        0      916 2023-05-05 11:18:34.857063 nautilus_trader-1.173.0/nautilus_core/persistence/src/parquet/implementations/mod.rs
--rw-r--r--   0        0        0     4006 2023-05-05 11:18:34.857063 nautilus_trader-1.173.0/nautilus_core/persistence/src/parquet/implementations/quote_tick.rs
--rw-r--r--   0        0        0     4266 2023-05-05 11:18:34.857063 nautilus_trader-1.173.0/nautilus_core/persistence/src/parquet/implementations/trade_tick.rs
--rw-r--r--   0        0        0     1564 2023-05-05 11:18:34.857063 nautilus_trader-1.173.0/nautilus_core/persistence/src/parquet/mod.rs
--rw-r--r--   0        0        0     9820 2023-05-05 11:18:34.857063 nautilus_trader-1.173.0/nautilus_core/persistence/src/session.rs
--rw-r--r--   0        0        0     3626 2023-05-05 11:18:34.857063 nautilus_trader-1.173.0/nautilus_core/persistence/tests/test_catalog.rs
--rw-r--r--   0        0        0     2886 2023-05-05 11:18:34.857063 nautilus_trader-1.173.0/nautilus_core/persistence/tests/test_persistence_module.py
--rw-r--r--   0        0        0     2179 2023-05-05 11:18:34.857063 nautilus_trader-1.173.0/nautilus_core/persistence/tests/test_util.rs
--rw-r--r--   0        0        0      604 2023-05-05 11:18:34.857063 nautilus_trader-1.173.0/nautilus_core/pyo3/Cargo.toml
--rw-r--r--   0        0        0     1909 2023-05-05 11:18:34.857063 nautilus_trader-1.173.0/nautilus_core/pyo3/src/lib.rs
--rw-r--r--   0        0        0       50 2023-05-05 11:18:34.857063 nautilus_trader-1.173.0/nautilus_core/rust-toolchain.toml
--rw-r--r--   0        0        0      869 2023-05-05 11:18:34.857063 nautilus_trader-1.173.0/nautilus_trader/__init__.pxd
--rw-r--r--   0        0        0     1268 2023-05-05 11:18:34.857063 nautilus_trader-1.173.0/nautilus_trader/__init__.py
--rw-r--r--   0        0        0      869 2023-05-05 11:18:34.857063 nautilus_trader-1.173.0/nautilus_trader/accounting/__init__.pxd
--rw-r--r--   0        0        0     1414 2023-05-05 11:18:34.857063 nautilus_trader-1.173.0/nautilus_trader/accounting/__init__.py
--rw-r--r--   0        0        0      869 2023-05-05 11:18:34.857063 nautilus_trader-1.173.0/nautilus_trader/accounting/accounts/__init__.pxd
--rw-r--r--   0        0        0      869 2023-05-05 11:18:34.857063 nautilus_trader-1.173.0/nautilus_trader/accounting/accounts/__init__.py
--rw-r--r--   0        0        0     3970 2023-05-05 11:18:34.857063 nautilus_trader-1.173.0/nautilus_trader/accounting/accounts/base.pxd
--rw-r--r--   0        0        0    14302 2023-05-05 11:18:34.857063 nautilus_trader-1.173.0/nautilus_trader/accounting/accounts/base.pyx
--rw-r--r--   0        0        0     1442 2023-05-05 11:18:34.857063 nautilus_trader-1.173.0/nautilus_trader/accounting/accounts/betting.pxd
--rw-r--r--   0        0        0     2758 2023-05-05 11:18:34.857063 nautilus_trader-1.173.0/nautilus_trader/accounting/accounts/betting.pyx
--rw-r--r--   0        0        0     1881 2023-05-05 11:18:34.857063 nautilus_trader-1.173.0/nautilus_trader/accounting/accounts/cash.pxd
--rw-r--r--   0        0        0    11304 2023-05-05 11:18:34.857063 nautilus_trader-1.173.0/nautilus_trader/accounting/accounts/cash.pyx
--rw-r--r--   0        0        0     3168 2023-05-05 11:18:34.857063 nautilus_trader-1.173.0/nautilus_trader/accounting/accounts/margin.pxd
--rw-r--r--   0        0        0    20380 2023-05-05 11:18:34.857063 nautilus_trader-1.173.0/nautilus_trader/accounting/accounts/margin.pyx
--rw-r--r--   0        0        0     1488 2023-05-05 11:18:34.857063 nautilus_trader-1.173.0/nautilus_trader/accounting/calculators.pxd
--rw-r--r--   0        0        0    10743 2023-05-05 11:18:34.857063 nautilus_trader-1.173.0/nautilus_trader/accounting/calculators.pyx
--rw-r--r--   0        0        0     1203 2023-05-05 11:18:34.857063 nautilus_trader-1.173.0/nautilus_trader/accounting/error.py
--rw-r--r--   0        0        0     1089 2023-05-05 11:18:34.857063 nautilus_trader-1.173.0/nautilus_trader/accounting/factory.pxd
--rw-r--r--   0        0        0     4063 2023-05-05 11:18:34.857063 nautilus_trader-1.173.0/nautilus_trader/accounting/factory.pyx
--rw-r--r--   0        0        0     2659 2023-05-05 11:18:34.857063 nautilus_trader-1.173.0/nautilus_trader/accounting/manager.pxd
--rw-r--r--   0        0        0    22651 2023-05-05 11:18:34.857063 nautilus_trader-1.173.0/nautilus_trader/accounting/manager.pyx
--rw-r--r--   0        0        0     1153 2023-05-05 11:18:34.857063 nautilus_trader-1.173.0/nautilus_trader/adapters/__init__.py
--rw-r--r--   0        0        0      869 2023-05-05 11:18:34.857063 nautilus_trader-1.173.0/nautilus_trader/adapters/_template/__init__.py
--rw-r--r--   0        0        0     1013 2023-05-05 11:18:34.857063 nautilus_trader-1.173.0/nautilus_trader/adapters/_template/core.py
--rw-r--r--   0        0        0    13300 2023-05-05 11:18:34.857063 nautilus_trader-1.173.0/nautilus_trader/adapters/_template/data.py
--rw-r--r--   0        0        0     6617 2023-05-05 11:18:34.857063 nautilus_trader-1.173.0/nautilus_trader/adapters/_template/execution.py
--rw-r--r--   0        0        0     2461 2023-05-05 11:18:34.857063 nautilus_trader-1.173.0/nautilus_trader/adapters/_template/providers.py
--rw-r--r--   0        0        0      946 2023-05-05 11:18:34.857063 nautilus_trader-1.173.0/nautilus_trader/adapters/betfair/__init__.py
--rw-r--r--   0        0        0      869 2023-05-05 11:18:34.857063 nautilus_trader-1.173.0/nautilus_trader/adapters/betfair/client/__init__.py
--rw-r--r--   0        0        0    11420 2023-05-05 11:18:34.861063 nautilus_trader-1.173.0/nautilus_trader/adapters/betfair/client/core.py
--rw-r--r--   0        0        0     2278 2023-05-05 11:18:34.861063 nautilus_trader-1.173.0/nautilus_trader/adapters/betfair/client/enums.py
--rw-r--r--   0        0        0     3494 2023-05-05 11:18:34.861063 nautilus_trader-1.173.0/nautilus_trader/adapters/betfair/client/exceptions.py
--rw-r--r--   0        0        0     2395 2023-05-05 11:18:34.861063 nautilus_trader-1.173.0/nautilus_trader/adapters/betfair/client/spec.py
--rw-r--r--   0        0        0     2725 2023-05-05 11:18:34.861063 nautilus_trader-1.173.0/nautilus_trader/adapters/betfair/client/util.py
--rw-r--r--   0        0        0     2856 2023-05-05 11:18:34.861063 nautilus_trader-1.173.0/nautilus_trader/adapters/betfair/common.py
--rw-r--r--   0        0        0     2342 2023-05-05 11:18:34.861063 nautilus_trader-1.173.0/nautilus_trader/adapters/betfair/config.py
--rw-r--r--   0        0        0     2056 2023-05-05 11:18:34.861063 nautilus_trader-1.173.0/nautilus_trader/adapters/betfair/constants.py
--rw-r--r--   0        0        0    12952 2023-05-05 11:18:34.861063 nautilus_trader-1.173.0/nautilus_trader/adapters/betfair/data.py
--rw-r--r--   0        0        0     8038 2023-05-05 11:18:34.861063 nautilus_trader-1.173.0/nautilus_trader/adapters/betfair/data_types.py
--rw-r--r--   0        0        0    41744 2023-05-05 11:18:34.861063 nautilus_trader-1.173.0/nautilus_trader/adapters/betfair/execution.py
--rw-r--r--   0        0        0     8697 2023-05-05 11:18:34.861063 nautilus_trader-1.173.0/nautilus_trader/adapters/betfair/factories.py
--rw-r--r--   0        0        0     2919 2023-05-05 11:18:34.861063 nautilus_trader-1.173.0/nautilus_trader/adapters/betfair/historic.py
--rw-r--r--   0        0        0     1271 2023-05-05 11:18:34.861063 nautilus_trader-1.173.0/nautilus_trader/adapters/betfair/orderbook.pxd
--rw-r--r--   0        0        0     2017 2023-05-05 11:18:34.861063 nautilus_trader-1.173.0/nautilus_trader/adapters/betfair/orderbook.pyx
--rw-r--r--   0        0        0      869 2023-05-05 11:18:34.861063 nautilus_trader-1.173.0/nautilus_trader/adapters/betfair/parsing/__init__.py
--rw-r--r--   0        0        0     2560 2023-05-05 11:18:34.861063 nautilus_trader-1.173.0/nautilus_trader/adapters/betfair/parsing/common.py
--rw-r--r--   0        0        0     2151 2023-05-05 11:18:34.861063 nautilus_trader-1.173.0/nautilus_trader/adapters/betfair/parsing/core.py
--rw-r--r--   0        0        0    12500 2023-05-05 11:18:34.861063 nautilus_trader-1.173.0/nautilus_trader/adapters/betfair/parsing/requests.py
--rw-r--r--   0        0        0    24915 2023-05-05 11:18:34.861063 nautilus_trader-1.173.0/nautilus_trader/adapters/betfair/parsing/streaming.py
--rw-r--r--   0        0        0    13208 2023-05-05 11:18:34.861063 nautilus_trader-1.173.0/nautilus_trader/adapters/betfair/providers.py
--rw-r--r--   0        0        0     7303 2023-05-05 11:18:34.861063 nautilus_trader-1.173.0/nautilus_trader/adapters/betfair/sockets.py
--rw-r--r--   0        0        0      939 2023-05-05 11:18:34.861063 nautilus_trader-1.173.0/nautilus_trader/adapters/binance/__init__.py
--rw-r--r--   0        0        0      869 2023-05-05 11:18:34.861063 nautilus_trader-1.173.0/nautilus_trader/adapters/binance/common/__init__.py
--rw-r--r--   0        0        0      957 2023-05-05 11:18:34.861063 nautilus_trader-1.173.0/nautilus_trader/adapters/binance/common/constants.py
--rw-r--r--   0        0        0    27000 2023-05-05 11:18:34.861063 nautilus_trader-1.173.0/nautilus_trader/adapters/binance/common/data.py
--rw-r--r--   0        0        0    11975 2023-05-05 11:18:34.861063 nautilus_trader-1.173.0/nautilus_trader/adapters/binance/common/enums.py
--rw-r--r--   0        0        0    35646 2023-05-05 11:18:34.861063 nautilus_trader-1.173.0/nautilus_trader/adapters/binance/common/execution.py
--rw-r--r--   0        0        0      869 2023-05-05 11:18:34.861063 nautilus_trader-1.173.0/nautilus_trader/adapters/binance/common/schemas/__init__.py
--rw-r--r--   0        0        0    10209 2023-05-05 11:18:34.861063 nautilus_trader-1.173.0/nautilus_trader/adapters/binance/common/schemas/account.py
--rw-r--r--   0        0        0    21419 2023-05-05 11:18:34.861063 nautilus_trader-1.173.0/nautilus_trader/adapters/binance/common/schemas/market.py
--rw-r--r--   0        0        0     2434 2023-05-05 11:18:34.861063 nautilus_trader-1.173.0/nautilus_trader/adapters/binance/common/schemas/symbol.py
--rw-r--r--   0        0        0     1199 2023-05-05 11:18:34.861063 nautilus_trader-1.173.0/nautilus_trader/adapters/binance/common/schemas/user.py
--rw-r--r--   0        0        0    14983 2023-05-05 11:18:34.861063 nautilus_trader-1.173.0/nautilus_trader/adapters/binance/common/types.py
--rw-r--r--   0        0        0     4013 2023-05-05 11:18:34.861063 nautilus_trader-1.173.0/nautilus_trader/adapters/binance/config.py
--rw-r--r--   0        0        0    17031 2023-05-05 11:18:34.861063 nautilus_trader-1.173.0/nautilus_trader/adapters/binance/factories.py
--rw-r--r--   0        0        0      869 2023-05-05 11:18:34.865063 nautilus_trader-1.173.0/nautilus_trader/adapters/binance/futures/__init__.py
--rw-r--r--   0        0        0     8658 2023-05-05 11:18:34.865063 nautilus_trader-1.173.0/nautilus_trader/adapters/binance/futures/data.py
--rw-r--r--   0        0        0     6746 2023-05-05 11:18:34.865063 nautilus_trader-1.173.0/nautilus_trader/adapters/binance/futures/enums.py
--rw-r--r--   0        0        0    12288 2023-05-05 11:18:34.865063 nautilus_trader-1.173.0/nautilus_trader/adapters/binance/futures/execution.py
--rw-r--r--   0        0        0      869 2023-05-05 11:18:34.865063 nautilus_trader-1.173.0/nautilus_trader/adapters/binance/futures/http/__init__.py
--rw-r--r--   0        0        0    13354 2023-05-05 11:18:34.865063 nautilus_trader-1.173.0/nautilus_trader/adapters/binance/futures/http/account.py
--rw-r--r--   0        0        0     3646 2023-05-05 11:18:34.865063 nautilus_trader-1.173.0/nautilus_trader/adapters/binance/futures/http/market.py
--rw-r--r--   0        0        0     1972 2023-05-05 11:18:34.865063 nautilus_trader-1.173.0/nautilus_trader/adapters/binance/futures/http/user.py
--rw-r--r--   0        0        0     4884 2023-05-05 11:18:34.865063 nautilus_trader-1.173.0/nautilus_trader/adapters/binance/futures/http/wallet.py
--rw-r--r--   0        0        0    16566 2023-05-05 11:18:34.865063 nautilus_trader-1.173.0/nautilus_trader/adapters/binance/futures/providers.py
--rw-r--r--   0        0        0      869 2023-05-05 11:18:34.865063 nautilus_trader-1.173.0/nautilus_trader/adapters/binance/futures/schemas/__init__.py
--rw-r--r--   0        0        0     6885 2023-05-05 11:18:34.865063 nautilus_trader-1.173.0/nautilus_trader/adapters/binance/futures/schemas/account.py
--rw-r--r--   0        0        0     7594 2023-05-05 11:18:34.865063 nautilus_trader-1.173.0/nautilus_trader/adapters/binance/futures/schemas/market.py
--rw-r--r--   0        0        0    13834 2023-05-05 11:18:34.865063 nautilus_trader-1.173.0/nautilus_trader/adapters/binance/futures/schemas/user.py
--rw-r--r--   0        0        0     1271 2023-05-05 11:18:34.865063 nautilus_trader-1.173.0/nautilus_trader/adapters/binance/futures/schemas/wallet.py
--rw-r--r--   0        0        0     4630 2023-05-05 11:18:34.865063 nautilus_trader-1.173.0/nautilus_trader/adapters/binance/futures/types.py
--rw-r--r--   0        0        0      869 2023-05-05 11:18:34.865063 nautilus_trader-1.173.0/nautilus_trader/adapters/binance/http/__init__.py
--rw-r--r--   0        0        0    24541 2023-05-05 11:18:34.865063 nautilus_trader-1.173.0/nautilus_trader/adapters/binance/http/account.py
--rw-r--r--   0        0        0     6559 2023-05-05 11:18:34.865063 nautilus_trader-1.173.0/nautilus_trader/adapters/binance/http/client.py
--rw-r--r--   0        0        0     3226 2023-05-05 11:18:34.865063 nautilus_trader-1.173.0/nautilus_trader/adapters/binance/http/endpoint.py
--rw-r--r--   0        0        0     1524 2023-05-05 11:18:34.865063 nautilus_trader-1.173.0/nautilus_trader/adapters/binance/http/error.py
--rw-r--r--   0        0        0    31644 2023-05-05 11:18:34.865063 nautilus_trader-1.173.0/nautilus_trader/adapters/binance/http/market.py
--rw-r--r--   0        0        0     7786 2023-05-05 11:18:34.865063 nautilus_trader-1.173.0/nautilus_trader/adapters/binance/http/user.py
--rw-r--r--   0        0        0      869 2023-05-05 11:18:34.865063 nautilus_trader-1.173.0/nautilus_trader/adapters/binance/spot/__init__.py
--rw-r--r--   0        0        0     5728 2023-05-05 11:18:34.865063 nautilus_trader-1.173.0/nautilus_trader/adapters/binance/spot/data.py
--rw-r--r--   0        0        0     4799 2023-05-05 11:18:34.865063 nautilus_trader-1.173.0/nautilus_trader/adapters/binance/spot/enums.py
--rw-r--r--   0        0        0     9851 2023-05-05 11:18:34.865063 nautilus_trader-1.173.0/nautilus_trader/adapters/binance/spot/execution.py
--rw-r--r--   0        0        0      869 2023-05-05 11:18:34.865063 nautilus_trader-1.173.0/nautilus_trader/adapters/binance/spot/http/__init__.py
--rw-r--r--   0        0        0    26424 2023-05-05 11:18:34.865063 nautilus_trader-1.173.0/nautilus_trader/adapters/binance/spot/http/account.py
--rw-r--r--   0        0        0     6709 2023-05-05 11:18:34.865063 nautilus_trader-1.173.0/nautilus_trader/adapters/binance/spot/http/market.py
--rw-r--r--   0        0        0     1981 2023-05-05 11:18:34.865063 nautilus_trader-1.173.0/nautilus_trader/adapters/binance/spot/http/user.py
--rw-r--r--   0        0        0     4669 2023-05-05 11:18:34.865063 nautilus_trader-1.173.0/nautilus_trader/adapters/binance/spot/http/wallet.py
--rw-r--r--   0        0        0    13617 2023-05-05 11:18:34.865063 nautilus_trader-1.173.0/nautilus_trader/adapters/binance/spot/providers.py
--rw-r--r--   0        0        0      869 2023-05-05 11:18:34.865063 nautilus_trader-1.173.0/nautilus_trader/adapters/binance/spot/schemas/__init__.py
--rw-r--r--   0        0        0     3299 2023-05-05 11:18:34.865063 nautilus_trader-1.173.0/nautilus_trader/adapters/binance/spot/schemas/account.py
--rw-r--r--   0        0        0     6282 2023-05-05 11:18:34.865063 nautilus_trader-1.173.0/nautilus_trader/adapters/binance/spot/schemas/market.py
--rw-r--r--   0        0        0    11677 2023-05-05 11:18:34.865063 nautilus_trader-1.173.0/nautilus_trader/adapters/binance/spot/schemas/user.py
--rw-r--r--   0        0        0     1252 2023-05-05 11:18:34.865063 nautilus_trader-1.173.0/nautilus_trader/adapters/binance/spot/schemas/wallet.py
--rw-r--r--   0        0        0      869 2023-05-05 11:18:34.865063 nautilus_trader-1.173.0/nautilus_trader/adapters/binance/websocket/__init__.py
--rw-r--r--   0        0        0     7724 2023-05-05 11:18:34.865063 nautilus_trader-1.173.0/nautilus_trader/adapters/binance/websocket/client.py
--rw-r--r--   0        0        0      869 2023-05-05 11:18:34.865063 nautilus_trader-1.173.0/nautilus_trader/adapters/deribit/__init__.py
--rw-r--r--   0        0        0      869 2023-05-05 11:18:34.865063 nautilus_trader-1.173.0/nautilus_trader/adapters/deribit/http/__init__.py
--rw-r--r--   0        0        0     5601 2023-05-05 11:18:34.865063 nautilus_trader-1.173.0/nautilus_trader/adapters/deribit/http/client.py
--rw-r--r--   0        0        0     1554 2023-05-05 11:18:34.865063 nautilus_trader-1.173.0/nautilus_trader/adapters/deribit/http/error.py
--rw-r--r--   0        0        0      931 2023-05-05 11:18:34.865063 nautilus_trader-1.173.0/nautilus_trader/adapters/interactive_brokers/__init__.py
--rw-r--r--   0        0        0     1299 2023-05-05 11:18:34.869063 nautilus_trader-1.173.0/nautilus_trader/adapters/interactive_brokers/common.py
--rw-r--r--   0        0        0     4009 2023-05-05 11:18:34.869063 nautilus_trader-1.173.0/nautilus_trader/adapters/interactive_brokers/config.py
--rw-r--r--   0        0        0    21236 2023-05-05 11:18:34.869063 nautilus_trader-1.173.0/nautilus_trader/adapters/interactive_brokers/data.py
--rw-r--r--   0        0        0    16814 2023-05-05 11:18:34.869063 nautilus_trader-1.173.0/nautilus_trader/adapters/interactive_brokers/execution.py
--rw-r--r--   0        0        0     9892 2023-05-05 11:18:34.869063 nautilus_trader-1.173.0/nautilus_trader/adapters/interactive_brokers/factories.py
--rw-r--r--   0        0        0     6761 2023-05-05 11:18:34.869063 nautilus_trader-1.173.0/nautilus_trader/adapters/interactive_brokers/gateway.py
--rw-r--r--   0        0        0    14016 2023-05-05 11:18:34.869063 nautilus_trader-1.173.0/nautilus_trader/adapters/interactive_brokers/historic.py
--rw-r--r--   0        0        0      869 2023-05-05 11:18:34.869063 nautilus_trader-1.173.0/nautilus_trader/adapters/interactive_brokers/parsing/__init__.py
--rw-r--r--   0        0        0     3915 2023-05-05 11:18:34.869063 nautilus_trader-1.173.0/nautilus_trader/adapters/interactive_brokers/parsing/data.py
--rw-r--r--   0        0        0     4911 2023-05-05 11:18:34.869063 nautilus_trader-1.173.0/nautilus_trader/adapters/interactive_brokers/parsing/execution.py
--rw-r--r--   0        0        0     8268 2023-05-05 11:18:34.869063 nautilus_trader-1.173.0/nautilus_trader/adapters/interactive_brokers/parsing/instruments.py
--rw-r--r--   0        0        0     9224 2023-05-05 11:18:34.869063 nautilus_trader-1.173.0/nautilus_trader/adapters/interactive_brokers/providers.py
--rw-r--r--   0        0        0     4670 2023-05-05 11:18:34.869063 nautilus_trader-1.173.0/nautilus_trader/adapters/interactive_brokers/web.py
--rw-r--r--   0        0        0      869 2023-05-05 11:18:34.869063 nautilus_trader-1.173.0/nautilus_trader/adapters/sandbox/__init__.py
--rw-r--r--   0        0        0     1393 2023-05-05 11:18:34.869063 nautilus_trader-1.173.0/nautilus_trader/adapters/sandbox/config.py
--rw-r--r--   0        0        0     7657 2023-05-05 11:18:34.869063 nautilus_trader-1.173.0/nautilus_trader/adapters/sandbox/execution.py
--rw-r--r--   0        0        0     2693 2023-05-05 11:18:34.869063 nautilus_trader-1.173.0/nautilus_trader/adapters/sandbox/factory.py
--rw-r--r--   0        0        0      979 2023-05-05 11:18:34.869063 nautilus_trader-1.173.0/nautilus_trader/analysis/__init__.py
--rw-r--r--   0        0        0    15217 2023-05-05 11:18:34.869063 nautilus_trader-1.173.0/nautilus_trader/analysis/analyzer.py
--rw-r--r--   0        0        0     4714 2023-05-05 11:18:34.869063 nautilus_trader-1.173.0/nautilus_trader/analysis/reporter.py
--rw-r--r--   0        0        0     3968 2023-05-05 11:18:34.869063 nautilus_trader-1.173.0/nautilus_trader/analysis/statistic.py
--rw-r--r--   0        0        0     2255 2023-05-05 11:18:34.869063 nautilus_trader-1.173.0/nautilus_trader/analysis/statistics/__init__.py
--rw-r--r--   0        0        0     2016 2023-05-05 11:18:34.869063 nautilus_trader-1.173.0/nautilus_trader/analysis/statistics/expectancy.py
--rw-r--r--   0        0        0     1717 2023-05-05 11:18:34.869063 nautilus_trader-1.173.0/nautilus_trader/analysis/statistics/long_ratio.py
--rw-r--r--   0        0        0     1481 2023-05-05 11:18:34.869063 nautilus_trader-1.173.0/nautilus_trader/analysis/statistics/loser_avg.py
--rw-r--r--   0        0        0     1527 2023-05-05 11:18:34.869063 nautilus_trader-1.173.0/nautilus_trader/analysis/statistics/loser_max.py
--rw-r--r--   0        0        0     1525 2023-05-05 11:18:34.869063 nautilus_trader-1.173.0/nautilus_trader/analysis/statistics/loser_min.py
--rw-r--r--   0        0        0     1576 2023-05-05 11:18:34.869063 nautilus_trader-1.173.0/nautilus_trader/analysis/statistics/profit_factor.py
--rw-r--r--   0        0        0     1412 2023-05-05 11:18:34.869063 nautilus_trader-1.173.0/nautilus_trader/analysis/statistics/returns_avg.py
--rw-r--r--   0        0        0     1427 2023-05-05 11:18:34.869063 nautilus_trader-1.173.0/nautilus_trader/analysis/statistics/returns_avg_loss.py
--rw-r--r--   0        0        0     1426 2023-05-05 11:18:34.869063 nautilus_trader-1.173.0/nautilus_trader/analysis/statistics/returns_avg_win.py
--rw-r--r--   0        0        0     1728 2023-05-05 11:18:34.869063 nautilus_trader-1.173.0/nautilus_trader/analysis/statistics/returns_volatility.py
--rw-r--r--   0        0        0     1336 2023-05-05 11:18:34.869063 nautilus_trader-1.173.0/nautilus_trader/analysis/statistics/risk_return_ratio.py
--rw-r--r--   0        0        0     1788 2023-05-05 11:18:34.869063 nautilus_trader-1.173.0/nautilus_trader/analysis/statistics/sharpe_ratio.py
--rw-r--r--   0        0        0     1895 2023-05-05 11:18:34.869063 nautilus_trader-1.173.0/nautilus_trader/analysis/statistics/sortino_ratio.py
--rw-r--r--   0        0        0     1511 2023-05-05 11:18:34.869063 nautilus_trader-1.173.0/nautilus_trader/analysis/statistics/win_rate.py
--rw-r--r--   0        0        0     1502 2023-05-05 11:18:34.869063 nautilus_trader-1.173.0/nautilus_trader/analysis/statistics/winner_avg.py
--rw-r--r--   0        0        0     1360 2023-05-05 11:18:34.869063 nautilus_trader-1.173.0/nautilus_trader/analysis/statistics/winner_max.py
--rw-r--r--   0        0        0     1507 2023-05-05 11:18:34.869063 nautilus_trader-1.173.0/nautilus_trader/analysis/statistics/winner_min.py
--rw-r--r--   0        0        0      869 2023-05-05 11:18:34.869063 nautilus_trader-1.173.0/nautilus_trader/backtest/__init__.pxd
--rw-r--r--   0        0        0      945 2023-05-05 11:18:34.869063 nautilus_trader-1.173.0/nautilus_trader/backtest/__init__.py
--rw-r--r--   0        0        0     1710 2023-05-05 11:18:34.869063 nautilus_trader-1.173.0/nautilus_trader/backtest/__main__.py
--rw-r--r--   0        0        0     3879 2023-05-05 11:18:34.869063 nautilus_trader-1.173.0/nautilus_trader/backtest/auction.py
--rw-r--r--   0        0        0     1100 2023-05-05 11:18:34.869063 nautilus_trader-1.173.0/nautilus_trader/backtest/data_client.pxd
--rw-r--r--   0        0        0    12847 2023-05-05 11:18:34.869063 nautilus_trader-1.173.0/nautilus_trader/backtest/data_client.pyx
--rw-r--r--   0        0        0     2164 2023-05-05 11:18:34.873063 nautilus_trader-1.173.0/nautilus_trader/backtest/engine.pxd
--rw-r--r--   0        0        0    45526 2023-05-05 11:18:34.873063 nautilus_trader-1.173.0/nautilus_trader/backtest/engine.pyx
--rw-r--r--   0        0        0     6868 2023-05-05 11:18:34.873063 nautilus_trader-1.173.0/nautilus_trader/backtest/exchange.pxd
--rw-r--r--   0        0        0    28443 2023-05-05 11:18:34.873063 nautilus_trader-1.173.0/nautilus_trader/backtest/exchange.pyx
--rw-r--r--   0        0        0     1084 2023-05-05 11:18:34.873063 nautilus_trader-1.173.0/nautilus_trader/backtest/execution_client.pxd
--rw-r--r--   0        0        0     5182 2023-05-05 11:18:34.873063 nautilus_trader-1.173.0/nautilus_trader/backtest/execution_client.pyx
--rw-r--r--   0        0        0    11232 2023-05-05 11:18:34.873063 nautilus_trader-1.173.0/nautilus_trader/backtest/matching_engine.pxd
--rw-r--r--   0        0        0    85576 2023-05-05 11:18:34.873063 nautilus_trader-1.173.0/nautilus_trader/backtest/matching_engine.pyx
--rw-r--r--   0        0        0     2075 2023-05-05 11:18:34.873063 nautilus_trader-1.173.0/nautilus_trader/backtest/models.pxd
--rw-r--r--   0        0        0     5344 2023-05-05 11:18:34.873063 nautilus_trader-1.173.0/nautilus_trader/backtest/models.pyx
--rw-r--r--   0        0        0     1814 2023-05-05 11:18:34.873063 nautilus_trader-1.173.0/nautilus_trader/backtest/modules.pxd
--rw-r--r--   0        0        0     8294 2023-05-05 11:18:34.873063 nautilus_trader-1.173.0/nautilus_trader/backtest/modules.pyx
--rw-r--r--   0        0        0    11469 2023-05-05 11:18:34.873063 nautilus_trader-1.173.0/nautilus_trader/backtest/node.py
--rw-r--r--   0        0        0     3110 2023-05-05 11:18:34.873063 nautilus_trader-1.173.0/nautilus_trader/backtest/results.py
--rw-r--r--   0        0        0      869 2023-05-05 11:18:34.873063 nautilus_trader-1.173.0/nautilus_trader/cache/__init__.pxd
--rw-r--r--   0        0        0     1052 2023-05-05 11:18:34.873063 nautilus_trader-1.173.0/nautilus_trader/cache/__init__.py
--rw-r--r--   0        0        0     9896 2023-05-05 11:18:34.873063 nautilus_trader-1.173.0/nautilus_trader/cache/base.pxd
--rw-r--r--   0        0        0    23040 2023-05-05 11:18:34.873063 nautilus_trader-1.173.0/nautilus_trader/cache/base.pyx
--rw-r--r--   0        0        0     7346 2023-05-05 11:18:34.873063 nautilus_trader-1.173.0/nautilus_trader/cache/cache.pxd
--rw-r--r--   0        0        0   122388 2023-05-05 11:18:34.873063 nautilus_trader-1.173.0/nautilus_trader/cache/cache.pyx
--rw-r--r--   0        0        0     3663 2023-05-05 11:18:34.873063 nautilus_trader-1.173.0/nautilus_trader/cache/database.pxd
--rw-r--r--   0        0        0     9114 2023-05-05 11:18:34.873063 nautilus_trader-1.173.0/nautilus_trader/cache/database.pyx
--rw-r--r--   0        0        0      869 2023-05-05 11:18:34.873063 nautilus_trader-1.173.0/nautilus_trader/common/__init__.pxd
--rw-r--r--   0        0        0     1571 2023-05-05 11:18:34.873063 nautilus_trader-1.173.0/nautilus_trader/common/__init__.py
--rw-r--r--   0        0        0    10002 2023-05-05 11:18:34.873063 nautilus_trader-1.173.0/nautilus_trader/common/actor.pxd
--rw-r--r--   0        0        0    74030 2023-05-05 11:18:34.873063 nautilus_trader-1.173.0/nautilus_trader/common/actor.pyx
--rw-r--r--   0        0        0     3547 2023-05-05 11:18:34.873063 nautilus_trader-1.173.0/nautilus_trader/common/clock.pxd
--rw-r--r--   0        0        0    27216 2023-05-05 11:18:34.873063 nautilus_trader-1.173.0/nautilus_trader/common/clock.pyx
--rw-r--r--   0        0        0     2916 2023-05-05 11:18:34.873063 nautilus_trader-1.173.0/nautilus_trader/common/component.pxd
--rw-r--r--   0        0        0    19989 2023-05-05 11:18:34.873063 nautilus_trader-1.173.0/nautilus_trader/common/component.pyx
--rw-r--r--   0        0        0     1836 2023-05-05 11:18:34.873063 nautilus_trader-1.173.0/nautilus_trader/common/enums.pyx
--rw-r--r--   0        0        0     1518 2023-05-05 11:18:34.873063 nautilus_trader-1.173.0/nautilus_trader/common/enums_c.pxd
--rw-r--r--   0        0        0     2638 2023-05-05 11:18:34.873063 nautilus_trader-1.173.0/nautilus_trader/common/enums_c.pyx
--rw-r--r--   0        0        0     8599 2023-05-05 11:18:34.873063 nautilus_trader-1.173.0/nautilus_trader/common/factories.pxd
--rw-r--r--   0        0        0    51638 2023-05-05 11:18:34.877063 nautilus_trader-1.173.0/nautilus_trader/common/factories.pyx
--rw-r--r--   0        0        0     1320 2023-05-05 11:18:34.877063 nautilus_trader-1.173.0/nautilus_trader/common/functions.py
--rw-r--r--   0        0        0     2139 2023-05-05 11:18:34.877063 nautilus_trader-1.173.0/nautilus_trader/common/generators.pxd
--rw-r--r--   0        0        0     7837 2023-05-05 11:18:34.877063 nautilus_trader-1.173.0/nautilus_trader/common/generators.pyx
--rw-r--r--   0        0        0     2460 2023-05-05 11:18:34.877063 nautilus_trader-1.173.0/nautilus_trader/common/logging.pxd
--rw-r--r--   0        0        0    18699 2023-05-05 11:18:34.877063 nautilus_trader-1.173.0/nautilus_trader/common/logging.pyx
--rw-r--r--   0        0        0     2421 2023-05-05 11:18:34.877063 nautilus_trader-1.173.0/nautilus_trader/common/messages.pxd
--rw-r--r--   0        0        0    10632 2023-05-05 11:18:34.877063 nautilus_trader-1.173.0/nautilus_trader/common/messages.pyx
--rw-r--r--   0        0        0    10746 2023-05-05 11:18:34.877063 nautilus_trader-1.173.0/nautilus_trader/common/providers.py
--rw-r--r--   0        0        0     1566 2023-05-05 11:18:34.877063 nautilus_trader-1.173.0/nautilus_trader/common/queue.pxd
--rw-r--r--   0        0        0     5704 2023-05-05 11:18:34.877063 nautilus_trader-1.173.0/nautilus_trader/common/queue.pyx
--rw-r--r--   0        0        0     2440 2023-05-05 11:18:34.877063 nautilus_trader-1.173.0/nautilus_trader/common/throttler.pxd
--rw-r--r--   0        0        0     7418 2023-05-05 11:18:34.877063 nautilus_trader-1.173.0/nautilus_trader/common/throttler.pyx
--rw-r--r--   0        0        0     2482 2023-05-05 11:18:34.877063 nautilus_trader-1.173.0/nautilus_trader/common/timer.pxd
--rw-r--r--   0        0        0    11992 2023-05-05 11:18:34.877063 nautilus_trader-1.173.0/nautilus_trader/common/timer.pyx
--rw-r--r--   0        0        0     3793 2023-05-05 11:18:34.877063 nautilus_trader-1.173.0/nautilus_trader/config/__init__.py
--rw-r--r--   0        0        0     9927 2023-05-05 11:18:34.877063 nautilus_trader-1.173.0/nautilus_trader/config/backtest.py
--rw-r--r--   0        0        0    19928 2023-05-05 11:18:34.877063 nautilus_trader-1.173.0/nautilus_trader/config/common.py
--rw-r--r--   0        0        0     1015 2023-05-05 11:18:34.877063 nautilus_trader-1.173.0/nautilus_trader/config/error.py
--rw-r--r--   0        0        0     7535 2023-05-05 11:18:34.877063 nautilus_trader-1.173.0/nautilus_trader/config/live.py
--rw-r--r--   0        0        0     1264 2023-05-05 11:18:34.877063 nautilus_trader-1.173.0/nautilus_trader/config/validation.py
--rw-r--r--   0        0        0      869 2023-05-05 11:18:34.877063 nautilus_trader-1.173.0/nautilus_trader/core/__init__.pxd
--rw-r--r--   0        0        0     1339 2023-05-05 11:18:34.877063 nautilus_trader-1.173.0/nautilus_trader/core/__init__.py
--rw-r--r--   0        0        0     1230 2023-05-05 11:18:34.877063 nautilus_trader-1.173.0/nautilus_trader/core/asynchronous.py
--rw-r--r--   0        0        0     3628 2023-05-05 11:18:34.877063 nautilus_trader-1.173.0/nautilus_trader/core/correctness.pxd
--rw-r--r--   0        0        0    37204 2023-05-05 11:18:34.877063 nautilus_trader-1.173.0/nautilus_trader/core/correctness.pyx
--rw-r--r--   0        0        0     1191 2023-05-05 11:18:34.877063 nautilus_trader-1.173.0/nautilus_trader/core/data.pxd
--rw-r--r--   0        0        0     2665 2023-05-05 11:18:34.877063 nautilus_trader-1.173.0/nautilus_trader/core/data.pyx
--rw-r--r--   0        0        0     1680 2023-05-05 11:18:34.877063 nautilus_trader-1.173.0/nautilus_trader/core/datetime.pxd
--rw-r--r--   0        0        0     9470 2023-05-05 11:18:34.877063 nautilus_trader-1.173.0/nautilus_trader/core/datetime.pyx
--rw-r--r--   0        0        0     1230 2023-05-05 11:18:34.877063 nautilus_trader-1.173.0/nautilus_trader/core/fsm.pxd
--rw-r--r--   0        0        0     4364 2023-05-05 11:18:34.877063 nautilus_trader-1.173.0/nautilus_trader/core/fsm.pyx
--rw-r--r--   0        0        0      906 2023-05-05 11:18:34.877063 nautilus_trader-1.173.0/nautilus_trader/core/includes/backtest.h
--rw-r--r--   0        0        0     7882 2023-05-05 11:18:34.877063 nautilus_trader-1.173.0/nautilus_trader/core/includes/common.h
--rw-r--r--   0        0        0     2997 2023-05-05 11:18:34.877063 nautilus_trader-1.173.0/nautilus_trader/core/includes/core.h
--rw-r--r--   0        0        0    29675 2023-05-05 11:18:34.877063 nautilus_trader-1.173.0/nautilus_trader/core/includes/model.h
--rw-r--r--   0        0        0     2369 2023-05-05 11:18:34.877063 nautilus_trader-1.173.0/nautilus_trader/core/inspect.py
--rw-r--r--   0        0        0     2471 2023-05-05 11:18:34.877063 nautilus_trader-1.173.0/nautilus_trader/core/message.pxd
--rw-r--r--   0        0        0     6720 2023-05-05 11:18:34.877063 nautilus_trader-1.173.0/nautilus_trader/core/message.pyx
--rw-r--r--   0        0        0      869 2023-05-05 11:18:34.877063 nautilus_trader-1.173.0/nautilus_trader/core/rust/__init__.pxd
--rw-r--r--   0        0        0     1033 2023-05-05 11:18:34.877063 nautilus_trader-1.173.0/nautilus_trader/core/rust/backtest.pxd
--rw-r--r--   0        0        0     7915 2023-05-05 11:26:01.320665 nautilus_trader-1.173.0/nautilus_trader/core/rust/common.pxd
--rw-r--r--   0        0        0     1222 2023-05-05 11:18:34.877063 nautilus_trader-1.173.0/nautilus_trader/core/rust/common.pyx
--rw-r--r--   0        0        0     2942 2023-05-05 11:25:33.980445 nautilus_trader-1.173.0/nautilus_trader/core/rust/core.pxd
--rw-r--r--   0        0        0    28213 2023-05-05 11:25:41.536506 nautilus_trader-1.173.0/nautilus_trader/core/rust/model.pxd
--rw-r--r--   0        0        0     2689 2023-05-05 11:18:34.881063 nautilus_trader-1.173.0/nautilus_trader/core/rust/model.pyx
--rw-r--r--   0        0        0     1359 2023-05-05 11:18:34.881063 nautilus_trader-1.173.0/nautilus_trader/core/stats.pxd
--rw-r--r--   0        0        0     5710 2023-05-05 11:18:34.881063 nautilus_trader-1.173.0/nautilus_trader/core/stats.pyx
--rw-r--r--   0        0        0     3197 2023-05-05 11:18:34.881063 nautilus_trader-1.173.0/nautilus_trader/core/string.pxd
--rw-r--r--   0        0        0     1049 2023-05-05 11:18:34.881063 nautilus_trader-1.173.0/nautilus_trader/core/uuid.pxd
--rw-r--r--   0        0        0     3157 2023-05-05 11:18:34.881063 nautilus_trader-1.173.0/nautilus_trader/core/uuid.pyx
--rw-r--r--   0        0        0      869 2023-05-05 11:18:34.881063 nautilus_trader-1.173.0/nautilus_trader/data/__init__.pxd
--rw-r--r--   0        0        0     1360 2023-05-05 11:18:34.881063 nautilus_trader-1.173.0/nautilus_trader/data/__init__.py
--rw-r--r--   0        0        0     4156 2023-05-05 11:18:34.881063 nautilus_trader-1.173.0/nautilus_trader/data/aggregation.pxd
--rw-r--r--   0        0        0    24142 2023-05-05 11:18:34.881063 nautilus_trader-1.173.0/nautilus_trader/data/aggregation.pyx
--rw-r--r--   0        0        0     8386 2023-05-05 11:18:34.881063 nautilus_trader-1.173.0/nautilus_trader/data/client.pxd
--rw-r--r--   0        0        0    41143 2023-05-05 11:18:34.881063 nautilus_trader-1.173.0/nautilus_trader/data/client.pyx
--rw-r--r--   0        0        0     8913 2023-05-05 11:18:34.881063 nautilus_trader-1.173.0/nautilus_trader/data/engine.pxd
--rw-r--r--   0        0        0    56101 2023-05-05 11:18:34.881063 nautilus_trader-1.173.0/nautilus_trader/data/engine.pyx
--rw-r--r--   0        0        0     2396 2023-05-05 11:18:34.881063 nautilus_trader-1.173.0/nautilus_trader/data/messages.pxd
--rw-r--r--   0        0        0     8389 2023-05-05 11:18:34.881063 nautilus_trader-1.173.0/nautilus_trader/data/messages.pyx
--rw-r--r--   0        0        0      869 2023-05-05 11:18:34.881063 nautilus_trader-1.173.0/nautilus_trader/examples/__init__.py
--rw-r--r--   0        0        0      869 2023-05-05 11:18:34.881063 nautilus_trader-1.173.0/nautilus_trader/examples/algorithms/__init__.py
--rw-r--r--   0        0        0     4133 2023-05-05 11:18:34.881063 nautilus_trader-1.173.0/nautilus_trader/examples/algorithms/blank.py
--rw-r--r--   0        0        0    11512 2023-05-05 11:18:34.881063 nautilus_trader-1.173.0/nautilus_trader/examples/algorithms/twap.py
--rw-r--r--   0        0        0      869 2023-05-05 11:18:34.881063 nautilus_trader-1.173.0/nautilus_trader/examples/strategies/__init__.pxd
--rw-r--r--   0        0        0      869 2023-05-05 11:18:34.881063 nautilus_trader-1.173.0/nautilus_trader/examples/strategies/__init__.py
--rw-r--r--   0        0        0     5659 2023-05-05 11:18:34.881063 nautilus_trader-1.173.0/nautilus_trader/examples/strategies/blank.py
--rw-r--r--   0        0        0    12218 2023-05-05 11:18:34.881063 nautilus_trader-1.173.0/nautilus_trader/examples/strategies/ema_cross.py
--rw-r--r--   0        0        0    12075 2023-05-05 11:18:34.881063 nautilus_trader-1.173.0/nautilus_trader/examples/strategies/ema_cross_bracket.py
--rw-r--r--   0        0        0    15002 2023-05-05 11:18:34.881063 nautilus_trader-1.173.0/nautilus_trader/examples/strategies/ema_cross_bracket_algo.py
--rw-r--r--   0        0        0    10735 2023-05-05 11:18:34.881063 nautilus_trader-1.173.0/nautilus_trader/examples/strategies/ema_cross_cython.pyx
--rw-r--r--   0        0        0    16151 2023-05-05 11:18:34.881063 nautilus_trader-1.173.0/nautilus_trader/examples/strategies/ema_cross_stop_entry.py
--rw-r--r--   0        0        0    14566 2023-05-05 11:18:34.881063 nautilus_trader-1.173.0/nautilus_trader/examples/strategies/ema_cross_trailing_stop.py
--rw-r--r--   0        0        0    12855 2023-05-05 11:18:34.881063 nautilus_trader-1.173.0/nautilus_trader/examples/strategies/ema_cross_twap.py
--rw-r--r--   0        0        0     5315 2023-05-05 11:18:34.881063 nautilus_trader-1.173.0/nautilus_trader/examples/strategies/market_maker.py
--rw-r--r--   0        0        0     8049 2023-05-05 11:18:34.881063 nautilus_trader-1.173.0/nautilus_trader/examples/strategies/orderbook_imbalance.py
--rw-r--r--   0        0        0     2730 2023-05-05 11:18:34.881063 nautilus_trader-1.173.0/nautilus_trader/examples/strategies/signal_strategy.py
--rw-r--r--   0        0        0     4653 2023-05-05 11:18:34.881063 nautilus_trader-1.173.0/nautilus_trader/examples/strategies/subscribe.py
--rw-r--r--   0        0        0    13478 2023-05-05 11:18:34.881063 nautilus_trader-1.173.0/nautilus_trader/examples/strategies/volatility_market_maker.py
--rw-r--r--   0        0        0      869 2023-05-05 11:18:34.881063 nautilus_trader-1.173.0/nautilus_trader/execution/__init__.pxd
--rw-r--r--   0        0        0     1353 2023-05-05 11:18:34.881063 nautilus_trader-1.173.0/nautilus_trader/execution/__init__.py
--rw-r--r--   0        0        0     5954 2023-05-05 11:18:34.881063 nautilus_trader-1.173.0/nautilus_trader/execution/algorithm.pxd
--rw-r--r--   0        0        0    38095 2023-05-05 11:18:34.881063 nautilus_trader-1.173.0/nautilus_trader/execution/algorithm.pyx
--rw-r--r--   0        0        0     7458 2023-05-05 11:18:34.881063 nautilus_trader-1.173.0/nautilus_trader/execution/client.pxd
--rw-r--r--   0        0        0    28604 2023-05-05 11:18:34.881063 nautilus_trader-1.173.0/nautilus_trader/execution/client.pyx
--rw-r--r--   0        0        0     4418 2023-05-05 11:18:34.881063 nautilus_trader-1.173.0/nautilus_trader/execution/emulator.pxd
--rw-r--r--   0        0        0    38511 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/execution/emulator.pyx
--rw-r--r--   0        0        0     6030 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/execution/engine.pxd
--rw-r--r--   0        0        0    33464 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/execution/engine.pyx
--rw-r--r--   0        0        0     3485 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/execution/matching_core.pxd
--rw-r--r--   0        0        0    14476 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/execution/matching_core.pyx
--rw-r--r--   0        0        0     5380 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/execution/messages.pxd
--rw-r--r--   0        0        0    30396 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/execution/messages.pyx
--rw-r--r--   0        0        0     8370 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/execution/reports.pxd
--rw-r--r--   0        0        0    22070 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/execution/reports.pyx
--rw-r--r--   0        0        0     1785 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/execution/trailing.pxd
--rw-r--r--   0        0        0    16636 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/execution/trailing.pyx
--rw-r--r--   0        0        0      869 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/indicators/__init__.pxd
--rw-r--r--   0        0        0     1188 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/indicators/__init__.py
--rw-r--r--   0        0        0     1722 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/indicators/amat.pxd
--rw-r--r--   0        0        0     4836 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/indicators/amat.pyx
--rw-r--r--   0        0        0     1482 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/indicators/aroon.pxd
--rw-r--r--   0        0        0     3474 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/indicators/aroon.pyx
--rw-r--r--   0        0        0     1474 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/indicators/atr.pxd
--rw-r--r--   0        0        0     4324 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/indicators/atr.pyx
--rw-r--r--   0        0        0      869 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/indicators/average/__init__.pxd
--rw-r--r--   0        0        0      869 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/indicators/average/__init__.py
--rw-r--r--   0        0        0     1770 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/indicators/average/ama.pxd
--rw-r--r--   0        0        0     5197 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/indicators/average/ama.pyx
--rw-r--r--   0        0        0     1063 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/indicators/average/dema.pxd
--rw-r--r--   0        0        0     3852 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/indicators/average/dema.pyx
--rw-r--r--   0        0        0     1096 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/indicators/average/ema.pxd
--rw-r--r--   0        0        0     3466 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/indicators/average/ema.pyx
--rw-r--r--   0        0        0     1247 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/indicators/average/hma.pxd
--rw-r--r--   0        0        0     4335 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/indicators/average/hma.pyx
--rw-r--r--   0        0        0     3114 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/indicators/average/ma_factory.pyx
--rw-r--r--   0        0        0     1566 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/indicators/average/moving_average.pxd
--rw-r--r--   0        0        0     2945 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/indicators/average/moving_average.pyx
--rw-r--r--   0        0        0     1080 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/indicators/average/rma.pxd
--rw-r--r--   0        0        0     3478 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/indicators/average/rma.pyx
--rw-r--r--   0        0        0     1020 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/indicators/average/sma.pxd
--rw-r--r--   0        0        0     3542 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/indicators/average/sma.pyx
--rw-r--r--   0        0        0     1283 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/indicators/average/vidya.pxd
--rw-r--r--   0        0        0     4604 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/indicators/average/vidya.pyx
--rw-r--r--   0        0        0     1174 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/indicators/average/wma.pxd
--rw-r--r--   0        0        0     4712 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/indicators/average/wma.pyx
--rw-r--r--   0        0        0      869 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/indicators/base/__init__.pxd
--rw-r--r--   0        0        0      869 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/indicators/base/__init__.py
--rw-r--r--   0        0        0     1715 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/indicators/base/indicator.pxd
--rw-r--r--   0        0        0     2981 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/indicators/base/indicator.pyx
--rw-r--r--   0        0        0     1315 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/indicators/bias.pxd
--rw-r--r--   0        0        0     2872 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/indicators/bias.pyx
--rw-r--r--   0        0        0     1579 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/indicators/bollinger_bands.pxd
--rw-r--r--   0        0        0     5221 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/indicators/bollinger_bands.pyx
--rw-r--r--   0        0        0     1639 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/indicators/cci.pxd
--rw-r--r--   0        0        0     4060 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/indicators/cci.pyx
--rw-r--r--   0        0        0     1375 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/indicators/cmo.pxd
--rw-r--r--   0        0        0     3664 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/indicators/cmo.pyx
--rw-r--r--   0        0        0     1662 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/indicators/dm.pxd
--rw-r--r--   0        0        0     3736 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/indicators/dm.pyx
--rw-r--r--   0        0        0     1490 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/indicators/donchian_channel.pxd
--rw-r--r--   0        0        0     4376 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/indicators/donchian_channel.pyx
--rw-r--r--   0        0        0     1231 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/indicators/efficiency_ratio.pxd
--rw-r--r--   0        0        0     3123 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/indicators/efficiency_ratio.pyx
--rw-r--r--   0        0        0     3172 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/indicators/fuzzy_candlesticks.pxd
--rw-r--r--   0        0        0    12544 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/indicators/fuzzy_candlesticks.pyx
--rw-r--r--   0        0        0     1347 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/indicators/fuzzy_enum.pyx
--rw-r--r--   0        0        0      869 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/indicators/fuzzy_enums/__init__.pxd
--rw-r--r--   0        0        0      869 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/indicators/fuzzy_enums/__init__.py
--rw-r--r--   0        0        0      976 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/indicators/fuzzy_enums/candle_body.pxd
--rw-r--r--   0        0        0      980 2023-05-05 11:18:34.885063 nautilus_trader-1.173.0/nautilus_trader/indicators/fuzzy_enums/candle_body.pyx
--rw-r--r--   0        0        0      947 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/indicators/fuzzy_enums/candle_direction.pxd
--rw-r--r--   0        0        0      987 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/indicators/fuzzy_enums/candle_direction.pyx
--rw-r--r--   0        0        0     1020 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/indicators/fuzzy_enums/candle_size.pxd
--rw-r--r--   0        0        0      972 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/indicators/fuzzy_enums/candle_size.pyx
--rw-r--r--   0        0        0      972 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/indicators/fuzzy_enums/candle_wick.pxd
--rw-r--r--   0        0        0      980 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/indicators/fuzzy_enums/candle_wick.pyx
--rw-r--r--   0        0        0     1809 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/indicators/keltner_channel.pxd
--rw-r--r--   0        0        0     4675 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/indicators/keltner_channel.pyx
--rw-r--r--   0        0        0     1395 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/indicators/keltner_position.pxd
--rw-r--r--   0        0        0     4284 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/indicators/keltner_position.pyx
--rw-r--r--   0        0        0     1713 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/indicators/kvo.pxd
--rw-r--r--   0        0        0     4731 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/indicators/kvo.pyx
--rw-r--r--   0        0        0     1636 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/indicators/linear_regression.pxd
--rw-r--r--   0        0        0     3843 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/indicators/linear_regression.pyx
--rw-r--r--   0        0        0     1662 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/indicators/macd.pxd
--rw-r--r--   0        0        0     4821 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/indicators/macd.pyx
--rw-r--r--   0        0        0     1232 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/indicators/obv.pxd
--rw-r--r--   0        0        0     2962 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/indicators/obv.pyx
--rw-r--r--   0        0        0     1514 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/indicators/pressure.pxd
--rw-r--r--   0        0        0     4387 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/indicators/pressure.pyx
--rw-r--r--   0        0        0     1476 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/indicators/psl.pxd
--rw-r--r--   0        0        0     3315 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/indicators/psl.pyx
--rw-r--r--   0        0        0     1227 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/indicators/roc.pxd
--rw-r--r--   0        0        0     2730 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/indicators/roc.pyx
--rw-r--r--   0        0        0     1393 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/indicators/rsi.pxd
--rw-r--r--   0        0        0     3771 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/indicators/rsi.pyx
--rw-r--r--   0        0        0     1767 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/indicators/rvi.pxd
--rw-r--r--   0        0        0     4543 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/indicators/rvi.pyx
--rw-r--r--   0        0        0     1444 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/indicators/spread_analyzer.pxd
--rw-r--r--   0        0        0     3384 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/indicators/spread_analyzer.pyx
--rw-r--r--   0        0        0     1485 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/indicators/stochastics.pxd
--rw-r--r--   0        0        0     3888 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/indicators/stochastics.pyx
--rw-r--r--   0        0        0     2275 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/indicators/swings.pxd
--rw-r--r--   0        0        0     4682 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/indicators/swings.pyx
--rw-r--r--   0        0        0     1458 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/indicators/vhf.pxd
--rw-r--r--   0        0        0     3517 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/indicators/vhf.pyx
--rw-r--r--   0        0        0     1485 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/indicators/volatility_ratio.pxd
--rw-r--r--   0        0        0     4486 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/indicators/volatility_ratio.pyx
--rw-r--r--   0        0        0     1270 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/indicators/vwap.pxd
--rw-r--r--   0        0        0     2942 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/indicators/vwap.pyx
--rw-r--r--   0        0        0      869 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/infrastructure/__init__.pxd
--rw-r--r--   0        0        0     1047 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/infrastructure/__init__.py
--rw-r--r--   0        0        0     1362 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/infrastructure/cache.pxd
--rw-r--r--   0        0        0    30746 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/infrastructure/cache.pyx
--rw-r--r--   0        0        0     1155 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/live/__init__.py
--rw-r--r--   0        0        0     1849 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/live/__main__.py
--rw-r--r--   0        0        0    30864 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/live/data_client.py
--rw-r--r--   0        0        0    15072 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/live/data_engine.py
--rw-r--r--   0        0        0    16690 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/live/execution_client.py
--rw-r--r--   0        0        0    37135 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/live/execution_engine.py
--rw-r--r--   0        0        0     3535 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/live/factories.py
--rw-r--r--   0        0        0    20231 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/live/node.py
--rw-r--r--   0        0        0     8452 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/live/node_builder.py
--rw-r--r--   0        0        0     9203 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/live/risk_engine.py
--rw-r--r--   0        0        0     5560 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/model/__init__.pxd
--rw-r--r--   0        0        0     1141 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/model/__init__.py
--rw-r--r--   0        0        0      894 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/model/currencies.pxd
--rw-r--r--   0        0        0     9220 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/model/currencies.pyx
--rw-r--r--   0        0        0     1308 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/model/currency.pxd
--rw-r--r--   0        0        0     8403 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/model/currency.pyx
--rw-r--r--   0        0        0      869 2023-05-05 11:18:34.889063 nautilus_trader-1.173.0/nautilus_trader/model/data/__init__.pxd
--rw-r--r--   0        0        0      950 2023-05-05 11:18:34.893063 nautilus_trader-1.173.0/nautilus_trader/model/data/__init__.py
--rw-r--r--   0        0        0     2541 2023-05-05 11:18:34.893063 nautilus_trader-1.173.0/nautilus_trader/model/data/bar.pxd
--rw-r--r--   0        0        0    26622 2023-05-05 11:18:34.893063 nautilus_trader-1.173.0/nautilus_trader/model/data/bar.pyx
--rw-r--r--   0        0        0     1178 2023-05-05 11:18:34.893063 nautilus_trader-1.173.0/nautilus_trader/model/data/bar_aggregation.pxd
--rw-r--r--   0        0        0      958 2023-05-05 11:18:34.893063 nautilus_trader-1.173.0/nautilus_trader/model/data/bar_aggregation.pyx
--rw-r--r--   0        0        0     1467 2023-05-05 11:18:34.893063 nautilus_trader-1.173.0/nautilus_trader/model/data/base.pxd
--rw-r--r--   0        0        0     3443 2023-05-05 11:18:34.893063 nautilus_trader-1.173.0/nautilus_trader/model/data/base.pyx
--rw-r--r--   0        0        0     1373 2023-05-05 11:18:34.893063 nautilus_trader-1.173.0/nautilus_trader/model/data/bet.pxd
--rw-r--r--   0        0        0     4166 2023-05-05 11:18:34.893063 nautilus_trader-1.173.0/nautilus_trader/model/data/bet.pyx
--rw-r--r--   0        0        0     3259 2023-05-05 11:18:34.893063 nautilus_trader-1.173.0/nautilus_trader/model/data/tick.pxd
--rw-r--r--   0        0        0    24747 2023-05-05 11:18:34.893063 nautilus_trader-1.173.0/nautilus_trader/model/data/tick.pyx
--rw-r--r--   0        0        0     1225 2023-05-05 11:18:34.893063 nautilus_trader-1.173.0/nautilus_trader/model/data/ticker.pxd
--rw-r--r--   0        0        0     3293 2023-05-05 11:18:34.893063 nautilus_trader-1.173.0/nautilus_trader/model/data/ticker.pyx
--rw-r--r--   0        0        0     2492 2023-05-05 11:18:34.893063 nautilus_trader-1.173.0/nautilus_trader/model/data/venue.pxd
--rw-r--r--   0        0        0    10197 2023-05-05 11:18:34.893063 nautilus_trader-1.173.0/nautilus_trader/model/data/venue.pyx
--rw-r--r--   0        0        0     7484 2023-05-05 11:18:34.893063 nautilus_trader-1.173.0/nautilus_trader/model/enums.pyx
--rw-r--r--   0        0        0     4918 2023-05-05 11:18:34.893063 nautilus_trader-1.173.0/nautilus_trader/model/enums_c.pxd
--rw-r--r--   0        0        0    11387 2023-05-05 11:18:34.893063 nautilus_trader-1.173.0/nautilus_trader/model/enums_c.pyx
--rw-r--r--   0        0        0      869 2023-05-05 11:18:34.893063 nautilus_trader-1.173.0/nautilus_trader/model/events/__init__.pxd
--rw-r--r--   0        0        0      951 2023-05-05 11:18:34.893063 nautilus_trader-1.173.0/nautilus_trader/model/events/__init__.py
--rw-r--r--   0        0        0     2058 2023-05-05 11:18:34.893063 nautilus_trader-1.173.0/nautilus_trader/model/events/account.pxd
--rw-r--r--   0        0        0     5965 2023-05-05 11:18:34.893063 nautilus_trader-1.173.0/nautilus_trader/model/events/account.pyx
--rw-r--r--   0        0        0     9076 2023-05-05 11:18:34.893063 nautilus_trader-1.173.0/nautilus_trader/model/events/order.pxd
--rw-r--r--   0        0        0    85735 2023-05-05 11:18:34.893063 nautilus_trader-1.173.0/nautilus_trader/model/events/order.pyx
--rw-r--r--   0        0        0     5544 2023-05-05 11:18:34.893063 nautilus_trader-1.173.0/nautilus_trader/model/events/position.pxd
--rw-r--r--   0        0        0    34546 2023-05-05 11:18:34.893063 nautilus_trader-1.173.0/nautilus_trader/model/events/position.pyx
--rw-r--r--   0        0        0     2983 2023-05-05 11:18:34.893063 nautilus_trader-1.173.0/nautilus_trader/model/identifiers.pxd
--rw-r--r--   0        0        0    22672 2023-05-05 11:18:34.893063 nautilus_trader-1.173.0/nautilus_trader/model/identifiers.pyx
--rw-r--r--   0        0        0        0 2023-05-05 11:18:34.893063 nautilus_trader-1.173.0/nautilus_trader/model/instruments/__init__.pxd
--rw-r--r--   0        0        0     1752 2023-05-05 11:18:34.893063 nautilus_trader-1.173.0/nautilus_trader/model/instruments/__init__.py
--rw-r--r--   0        0        0     4880 2023-05-05 11:18:34.893063 nautilus_trader-1.173.0/nautilus_trader/model/instruments/base.pxd
--rw-r--r--   0        0        0    19261 2023-05-05 11:18:34.893063 nautilus_trader-1.173.0/nautilus_trader/model/instruments/base.pyx
--rw-r--r--   0        0        0     1745 2023-05-05 11:18:34.893063 nautilus_trader-1.173.0/nautilus_trader/model/instruments/betting.pxd
--rw-r--r--   0        0        0     7712 2023-05-05 11:18:34.893063 nautilus_trader-1.173.0/nautilus_trader/model/instruments/betting.pyx
--rw-r--r--   0        0        0     1521 2023-05-05 11:18:34.893063 nautilus_trader-1.173.0/nautilus_trader/model/instruments/crypto_future.pxd
--rw-r--r--   0        0        0    11042 2023-05-05 11:18:34.893063 nautilus_trader-1.173.0/nautilus_trader/model/instruments/crypto_future.pyx
--rw-r--r--   0        0        0     1491 2023-05-05 11:18:34.893063 nautilus_trader-1.173.0/nautilus_trader/model/instruments/crypto_perpetual.pxd
--rw-r--r--   0        0        0    11211 2023-05-05 11:18:34.893063 nautilus_trader-1.173.0/nautilus_trader/model/instruments/crypto_perpetual.pyx
--rw-r--r--   0        0        0     1265 2023-05-05 11:18:34.893063 nautilus_trader-1.173.0/nautilus_trader/model/instruments/currency_pair.pxd
--rw-r--r--   0        0        0    11354 2023-05-05 11:18:34.893063 nautilus_trader-1.173.0/nautilus_trader/model/instruments/currency_pair.pyx
--rw-r--r--   0        0        0     1108 2023-05-05 11:18:34.893063 nautilus_trader-1.173.0/nautilus_trader/model/instruments/equity.pxd
--rw-r--r--   0        0        0     7319 2023-05-05 11:18:34.893063 nautilus_trader-1.173.0/nautilus_trader/model/instruments/equity.pyx
--rw-r--r--   0        0        0     1344 2023-05-05 11:18:34.893063 nautilus_trader-1.173.0/nautilus_trader/model/instruments/futures_contract.pxd
--rw-r--r--   0        0        0     6806 2023-05-05 11:18:34.893063 nautilus_trader-1.173.0/nautilus_trader/model/instruments/futures_contract.pyx
--rw-r--r--   0        0        0     1386 2023-05-05 11:18:34.893063 nautilus_trader-1.173.0/nautilus_trader/model/instruments/options_contract.pxd
--rw-r--r--   0        0        0     7459 2023-05-05 11:18:34.893063 nautilus_trader-1.173.0/nautilus_trader/model/instruments/options_contract.pyx
--rw-r--r--   0        0        0     5280 2023-05-05 11:18:34.893063 nautilus_trader-1.173.0/nautilus_trader/model/objects.pxd
--rw-r--r--   0        0        0    40812 2023-05-05 11:18:34.893063 nautilus_trader-1.173.0/nautilus_trader/model/objects.pyx
--rw-r--r--   0        0        0      869 2023-05-05 11:18:34.897063 nautilus_trader-1.173.0/nautilus_trader/model/orderbook/__init__.pxd
--rw-r--r--   0        0        0     1625 2023-05-05 11:18:34.897063 nautilus_trader-1.173.0/nautilus_trader/model/orderbook/__init__.py
--rw-r--r--   0        0        0     5097 2023-05-05 11:18:34.897063 nautilus_trader-1.173.0/nautilus_trader/model/orderbook/book.pxd
--rw-r--r--   0        0        0    31125 2023-05-05 11:18:34.897063 nautilus_trader-1.173.0/nautilus_trader/model/orderbook/book.pyx
--rw-r--r--   0        0        0     3405 2023-05-05 11:18:34.897063 nautilus_trader-1.173.0/nautilus_trader/model/orderbook/data.pxd
--rw-r--r--   0        0        0    17415 2023-05-05 11:18:34.897063 nautilus_trader-1.173.0/nautilus_trader/model/orderbook/data.pyx
--rw-r--r--   0        0        0     1015 2023-05-05 11:18:34.897063 nautilus_trader-1.173.0/nautilus_trader/model/orderbook/error.py
--rw-r--r--   0        0        0     2757 2023-05-05 11:18:34.897063 nautilus_trader-1.173.0/nautilus_trader/model/orderbook/ladder.pxd
--rw-r--r--   0        0        0     8373 2023-05-05 11:18:34.897063 nautilus_trader-1.173.0/nautilus_trader/model/orderbook/ladder.pyx
--rw-r--r--   0        0        0     1362 2023-05-05 11:18:34.897063 nautilus_trader-1.173.0/nautilus_trader/model/orderbook/level.pxd
--rw-r--r--   0        0        0     4102 2023-05-05 11:18:34.897063 nautilus_trader-1.173.0/nautilus_trader/model/orderbook/level.pyx
--rw-r--r--   0        0        0     1336 2023-05-05 11:18:34.897063 nautilus_trader-1.173.0/nautilus_trader/model/orderbook/simulated.pxd
--rw-r--r--   0        0        0     6250 2023-05-05 11:18:34.897063 nautilus_trader-1.173.0/nautilus_trader/model/orderbook/simulated.pyx
--rw-r--r--   0        0        0      869 2023-05-05 11:18:34.897063 nautilus_trader-1.173.0/nautilus_trader/model/orders/__init__.pxd
--rw-r--r--   0        0        0     2093 2023-05-05 11:18:34.897063 nautilus_trader-1.173.0/nautilus_trader/model/orders/__init__.py
--rw-r--r--   0        0        0     8827 2023-05-05 11:18:34.897063 nautilus_trader-1.173.0/nautilus_trader/model/orders/base.pxd
--rw-r--r--   0        0        0    33961 2023-05-05 11:18:34.897063 nautilus_trader-1.173.0/nautilus_trader/model/orders/base.pyx
--rw-r--r--   0        0        0     1690 2023-05-05 11:18:34.897063 nautilus_trader-1.173.0/nautilus_trader/model/orders/limit.pxd
--rw-r--r--   0        0        0    16792 2023-05-05 11:18:34.897063 nautilus_trader-1.173.0/nautilus_trader/model/orders/limit.pyx
--rw-r--r--   0        0        0     2171 2023-05-05 11:18:34.897063 nautilus_trader-1.173.0/nautilus_trader/model/orders/limit_if_touched.pxd
--rw-r--r--   0        0        0    16477 2023-05-05 11:18:34.897063 nautilus_trader-1.173.0/nautilus_trader/model/orders/limit_if_touched.pyx
--rw-r--r--   0        0        0     1849 2023-05-05 11:18:34.897063 nautilus_trader-1.173.0/nautilus_trader/model/orders/list.pxd
--rw-r--r--   0        0        0     2367 2023-05-05 11:18:34.897063 nautilus_trader-1.173.0/nautilus_trader/model/orders/list.pyx
--rw-r--r--   0        0        0     1206 2023-05-05 11:18:34.897063 nautilus_trader-1.173.0/nautilus_trader/model/orders/market.pxd
--rw-r--r--   0        0        0    12902 2023-05-05 11:18:34.897063 nautilus_trader-1.173.0/nautilus_trader/model/orders/market.pyx
--rw-r--r--   0        0        0     1608 2023-05-05 11:18:34.897063 nautilus_trader-1.173.0/nautilus_trader/model/orders/market_if_touched.pxd
--rw-r--r--   0        0        0    14755 2023-05-05 11:18:34.897063 nautilus_trader-1.173.0/nautilus_trader/model/orders/market_if_touched.pyx
--rw-r--r--   0        0        0     1644 2023-05-05 11:18:34.897063 nautilus_trader-1.173.0/nautilus_trader/model/orders/market_to_limit.pxd
--rw-r--r--   0        0        0    13592 2023-05-05 11:18:34.897063 nautilus_trader-1.173.0/nautilus_trader/model/orders/market_to_limit.pyx
--rw-r--r--   0        0        0     2161 2023-05-05 11:18:34.897063 nautilus_trader-1.173.0/nautilus_trader/model/orders/stop_limit.pxd
--rw-r--r--   0        0        0    16617 2023-05-05 11:18:34.897063 nautilus_trader-1.173.0/nautilus_trader/model/orders/stop_limit.pyx
--rw-r--r--   0        0        0     1598 2023-05-05 11:18:34.897063 nautilus_trader-1.173.0/nautilus_trader/model/orders/stop_market.pxd
--rw-r--r--   0        0        0    15030 2023-05-05 11:18:34.897063 nautilus_trader-1.173.0/nautilus_trader/model/orders/stop_market.pyx
--rw-r--r--   0        0        0     2641 2023-05-05 11:18:34.897063 nautilus_trader-1.173.0/nautilus_trader/model/orders/trailing_stop_limit.pxd
--rw-r--r--   0        0        0    18630 2023-05-05 11:18:34.897063 nautilus_trader-1.173.0/nautilus_trader/model/orders/trailing_stop_limit.pyx
--rw-r--r--   0        0        0     1947 2023-05-05 11:18:34.897063 nautilus_trader-1.173.0/nautilus_trader/model/orders/trailing_stop_market.pxd
--rw-r--r--   0        0        0    16279 2023-05-05 11:18:34.897063 nautilus_trader-1.173.0/nautilus_trader/model/orders/trailing_stop_market.pyx
--rw-r--r--   0        0        0     1141 2023-05-05 11:18:34.897063 nautilus_trader-1.173.0/nautilus_trader/model/orders/unpacker.pxd
--rw-r--r--   0        0        0     3906 2023-05-05 11:18:34.897063 nautilus_trader-1.173.0/nautilus_trader/model/orders/unpacker.pyx
--rw-r--r--   0        0        0     6860 2023-05-05 11:18:34.897063 nautilus_trader-1.173.0/nautilus_trader/model/position.pxd
--rw-r--r--   0        0        0    23025 2023-05-05 11:18:34.897063 nautilus_trader-1.173.0/nautilus_trader/model/position.pyx
--rw-r--r--   0        0        0      869 2023-05-05 11:18:34.897063 nautilus_trader-1.173.0/nautilus_trader/model/tick_scheme/__init__.pxd
--rw-r--r--   0        0        0     1335 2023-05-05 11:18:34.897063 nautilus_trader-1.173.0/nautilus_trader/model/tick_scheme/__init__.py
--rw-r--r--   0        0        0     1581 2023-05-05 11:18:34.897063 nautilus_trader-1.173.0/nautilus_trader/model/tick_scheme/base.pxd
--rw-r--r--   0        0        0     3709 2023-05-05 11:18:34.897063 nautilus_trader-1.173.0/nautilus_trader/model/tick_scheme/base.pyx
--rw-r--r--   0        0        0     1142 2023-05-05 11:18:34.901063 nautilus_trader-1.173.0/nautilus_trader/model/tick_scheme/implementations/__init__.py
--rw-r--r--   0        0        0     1371 2023-05-05 11:18:34.901063 nautilus_trader-1.173.0/nautilus_trader/model/tick_scheme/implementations/fixed.pxd
--rw-r--r--   0        0        0     4052 2023-05-05 11:18:34.901063 nautilus_trader-1.173.0/nautilus_trader/model/tick_scheme/implementations/fixed.pyx
--rw-r--r--   0        0        0     1359 2023-05-05 11:18:34.901063 nautilus_trader-1.173.0/nautilus_trader/model/tick_scheme/implementations/tiered.pxd
--rw-r--r--   0        0        0     5632 2023-05-05 11:18:34.901063 nautilus_trader-1.173.0/nautilus_trader/model/tick_scheme/implementations/tiered.pyx
--rw-r--r--   0        0        0      869 2023-05-05 11:18:34.901063 nautilus_trader-1.173.0/nautilus_trader/msgbus/__init__.pxd
--rw-r--r--   0        0        0      994 2023-05-05 11:18:34.901063 nautilus_trader-1.173.0/nautilus_trader/msgbus/__init__.py
--rw-r--r--   0        0        0     2718 2023-05-05 11:18:34.901063 nautilus_trader-1.173.0/nautilus_trader/msgbus/bus.pxd
--rw-r--r--   0        0        0    16946 2023-05-05 11:18:34.901063 nautilus_trader-1.173.0/nautilus_trader/msgbus/bus.pyx
--rw-r--r--   0        0        0     1181 2023-05-05 11:18:34.901063 nautilus_trader-1.173.0/nautilus_trader/msgbus/subscription.pxd
--rw-r--r--   0        0        0     3066 2023-05-05 11:18:34.901063 nautilus_trader-1.173.0/nautilus_trader/msgbus/subscription.pyx
--rw-r--r--   0        0        0      869 2023-05-05 11:18:34.901063 nautilus_trader-1.173.0/nautilus_trader/network/__init__.pxd
--rw-r--r--   0        0        0     1125 2023-05-05 11:18:34.901063 nautilus_trader-1.173.0/nautilus_trader/network/__init__.py
--rw-r--r--   0        0        0     1020 2023-05-05 11:18:34.901063 nautilus_trader-1.173.0/nautilus_trader/network/error.py
--rw-r--r--   0        0        0     1520 2023-05-05 11:18:34.901063 nautilus_trader-1.173.0/nautilus_trader/network/http.pxd
--rw-r--r--   0        0        0     9912 2023-05-05 11:18:34.901063 nautilus_trader-1.173.0/nautilus_trader/network/http.pyx
--rw-r--r--   0        0        0     1868 2023-05-05 11:18:34.901063 nautilus_trader-1.173.0/nautilus_trader/network/socket.pxd
--rw-r--r--   0        0        0     6595 2023-05-05 11:18:34.901063 nautilus_trader-1.173.0/nautilus_trader/network/socket.pyx
--rw-r--r--   0        0        0     1832 2023-05-05 11:18:34.901063 nautilus_trader-1.173.0/nautilus_trader/network/websocket.pxd
--rw-r--r--   0        0        0    10808 2023-05-05 11:18:34.901063 nautilus_trader-1.173.0/nautilus_trader/network/websocket.pyx
--rw-r--r--   0        0        0      980 2023-05-05 11:18:34.901063 nautilus_trader-1.173.0/nautilus_trader/persistence/__init__.py
--rw-r--r--   0        0        0     1079 2023-05-05 11:18:34.901063 nautilus_trader-1.173.0/nautilus_trader/persistence/catalog/__init__.py
--rw-r--r--   0        0        0     6142 2023-05-05 11:18:34.901063 nautilus_trader-1.173.0/nautilus_trader/persistence/catalog/base.py
--rw-r--r--   0        0        0    18532 2023-05-05 11:18:34.901063 nautilus_trader-1.173.0/nautilus_trader/persistence/catalog/parquet.py
--rw-r--r--   0        0        0      869 2023-05-05 11:18:34.901063 nautilus_trader-1.173.0/nautilus_trader/persistence/external/__init__.py
--rw-r--r--   0        0        0    14925 2023-05-05 11:18:34.901063 nautilus_trader-1.173.0/nautilus_trader/persistence/external/core.py
--rw-r--r--   0        0        0     1555 2023-05-05 11:18:34.901063 nautilus_trader-1.173.0/nautilus_trader/persistence/external/metadata.py
--rw-r--r--   0        0        0    13281 2023-05-05 11:18:34.901063 nautilus_trader-1.173.0/nautilus_trader/persistence/external/readers.py
--rw-r--r--   0        0        0     3157 2023-05-05 11:18:34.901063 nautilus_trader-1.173.0/nautilus_trader/persistence/external/util.py
--rw-r--r--   0        0        0     2152 2023-05-05 11:18:34.901063 nautilus_trader-1.173.0/nautilus_trader/persistence/funcs.py
--rw-r--r--   0        0        0     5328 2023-05-05 11:18:34.901063 nautilus_trader-1.173.0/nautilus_trader/persistence/loaders.py
--rw-r--r--   0        0        0     1539 2023-05-05 11:18:34.901063 nautilus_trader-1.173.0/nautilus_trader/persistence/migrate.py
--rw-r--r--   0        0        0        0 2023-05-05 11:18:34.901063 nautilus_trader-1.173.0/nautilus_trader/persistence/streaming/__init__.py
--rw-r--r--   0        0        0     5330 2023-05-05 11:18:34.901063 nautilus_trader-1.173.0/nautilus_trader/persistence/streaming/batching.py
--rw-r--r--   0        0        0     8183 2023-05-05 11:18:34.901063 nautilus_trader-1.173.0/nautilus_trader/persistence/streaming/engine.py
--rw-r--r--   0        0        0     7610 2023-05-05 11:18:34.901063 nautilus_trader-1.173.0/nautilus_trader/persistence/streaming/writer.py
--rw-r--r--   0        0        0     2564 2023-05-05 11:18:34.901063 nautilus_trader-1.173.0/nautilus_trader/persistence/wranglers.pxd
--rw-r--r--   0        0        0    17864 2023-05-05 11:18:34.901063 nautilus_trader-1.173.0/nautilus_trader/persistence/wranglers.pyx
--rw-r--r--   0        0        0      869 2023-05-05 11:18:34.901063 nautilus_trader-1.173.0/nautilus_trader/portfolio/__init__.pxd
--rw-r--r--   0        0        0      948 2023-05-05 11:18:34.901063 nautilus_trader-1.173.0/nautilus_trader/portfolio/__init__.py
--rw-r--r--   0        0        0     2132 2023-05-05 11:18:34.901063 nautilus_trader-1.173.0/nautilus_trader/portfolio/base.pxd
--rw-r--r--   0        0        0     4033 2023-05-05 11:18:34.901063 nautilus_trader-1.173.0/nautilus_trader/portfolio/base.pyx
--rw-r--r--   0        0        0     3015 2023-05-05 11:18:34.901063 nautilus_trader-1.173.0/nautilus_trader/portfolio/portfolio.pxd
--rw-r--r--   0        0        0    37488 2023-05-05 11:18:34.901063 nautilus_trader-1.173.0/nautilus_trader/portfolio/portfolio.pyx
--rw-r--r--   0        0        0      869 2023-05-05 11:18:34.901063 nautilus_trader-1.173.0/nautilus_trader/risk/__init__.pxd
--rw-r--r--   0        0        0     1084 2023-05-05 11:18:34.901063 nautilus_trader-1.173.0/nautilus_trader/risk/__init__.py
--rw-r--r--   0        0        0     5613 2023-05-05 11:18:34.901063 nautilus_trader-1.173.0/nautilus_trader/risk/engine.pxd
--rw-r--r--   0        0        0    36965 2023-05-05 11:18:34.905063 nautilus_trader-1.173.0/nautilus_trader/risk/engine.pyx
--rw-r--r--   0        0        0     1747 2023-05-05 11:18:34.905063 nautilus_trader-1.173.0/nautilus_trader/risk/sizing.pxd
--rw-r--r--   0        0        0     7081 2023-05-05 11:18:34.905063 nautilus_trader-1.173.0/nautilus_trader/risk/sizing.pyx
--rw-r--r--   0        0        0      869 2023-05-05 11:18:34.905063 nautilus_trader-1.173.0/nautilus_trader/serialization/__init__.pxd
--rw-r--r--   0        0        0     1106 2023-05-05 11:18:34.905063 nautilus_trader-1.173.0/nautilus_trader/serialization/__init__.py
--rw-r--r--   0        0        0      869 2023-05-05 11:18:34.905063 nautilus_trader-1.173.0/nautilus_trader/serialization/arrow/__init__.pxd
--rw-r--r--   0        0        0      948 2023-05-05 11:18:34.905063 nautilus_trader-1.173.0/nautilus_trader/serialization/arrow/__init__.py
--rw-r--r--   0        0        0     1408 2023-05-05 11:18:34.905063 nautilus_trader-1.173.0/nautilus_trader/serialization/arrow/implementations/__init__.py
--rw-r--r--   0        0        0     4206 2023-05-05 11:18:34.905063 nautilus_trader-1.173.0/nautilus_trader/serialization/arrow/implementations/account_state.py
--rw-r--r--   0        0        0     1373 2023-05-05 11:18:34.905063 nautilus_trader-1.173.0/nautilus_trader/serialization/arrow/implementations/bar.py
--rw-r--r--   0        0        0     1095 2023-05-05 11:18:34.905063 nautilus_trader-1.173.0/nautilus_trader/serialization/arrow/implementations/instruments.py
--rw-r--r--   0        0        0     5482 2023-05-05 11:18:34.905063 nautilus_trader-1.173.0/nautilus_trader/serialization/arrow/implementations/order_book.py
--rw-r--r--   0        0        0     2961 2023-05-05 11:18:34.905063 nautilus_trader-1.173.0/nautilus_trader/serialization/arrow/implementations/order_events.py
--rw-r--r--   0        0        0     2873 2023-05-05 11:18:34.905063 nautilus_trader-1.173.0/nautilus_trader/serialization/arrow/implementations/position_events.py
--rw-r--r--   0        0        0    29125 2023-05-05 11:18:34.905063 nautilus_trader-1.173.0/nautilus_trader/serialization/arrow/schema.py
--rw-r--r--   0        0        0      910 2023-05-05 11:18:34.905063 nautilus_trader-1.173.0/nautilus_trader/serialization/arrow/serializer.pxd
--rw-r--r--   0        0        0     6290 2023-05-05 11:18:34.905063 nautilus_trader-1.173.0/nautilus_trader/serialization/arrow/serializer.pyx
--rw-r--r--   0        0        0     4625 2023-05-05 11:18:34.905063 nautilus_trader-1.173.0/nautilus_trader/serialization/arrow/util.py
--rw-r--r--   0        0        0     1053 2023-05-05 11:18:34.905063 nautilus_trader-1.173.0/nautilus_trader/serialization/base.pxd
--rw-r--r--   0        0        0    10114 2023-05-05 11:18:34.905063 nautilus_trader-1.173.0/nautilus_trader/serialization/base.pyx
--rw-r--r--   0        0        0      869 2023-05-05 11:18:34.905063 nautilus_trader-1.173.0/nautilus_trader/serialization/msgpack/__init__.pxd
--rw-r--r--   0        0        0      869 2023-05-05 11:18:34.905063 nautilus_trader-1.173.0/nautilus_trader/serialization/msgpack/__init__.py
--rw-r--r--   0        0        0     1097 2023-05-05 11:18:34.905063 nautilus_trader-1.173.0/nautilus_trader/serialization/msgpack/serializer.pxd
--rw-r--r--   0        0        0     3649 2023-05-05 11:18:34.905063 nautilus_trader-1.173.0/nautilus_trader/serialization/msgpack/serializer.pyx
--rw-r--r--   0        0        0      869 2023-05-05 11:18:34.905063 nautilus_trader-1.173.0/nautilus_trader/system/__init__.py
--rw-r--r--   0        0        0    23211 2023-05-05 11:18:34.905063 nautilus_trader-1.173.0/nautilus_trader/system/kernel.py
--rw-r--r--   0        0        0     1035 2023-05-05 11:18:34.905063 nautilus_trader-1.173.0/nautilus_trader/test_kit/__init__.py
--rw-r--r--   0        0        0      869 2023-05-05 11:18:34.905063 nautilus_trader-1.173.0/nautilus_trader/test_kit/mocks/__init__.py
--rw-r--r--   0        0        0     6160 2023-05-05 11:18:34.905063 nautilus_trader-1.173.0/nautilus_trader/test_kit/mocks/actors.py
--rw-r--r--   0        0        0     5825 2023-05-05 11:18:34.905063 nautilus_trader-1.173.0/nautilus_trader/test_kit/mocks/cache_database.py
--rw-r--r--   0        0        0     4006 2023-05-05 11:18:34.905063 nautilus_trader-1.173.0/nautilus_trader/test_kit/mocks/data.py
--rw-r--r--   0        0        0     3077 2023-05-05 11:18:34.905063 nautilus_trader-1.173.0/nautilus_trader/test_kit/mocks/engines.py
--rw-r--r--   0        0        0    12905 2023-05-05 11:18:34.905063 nautilus_trader-1.173.0/nautilus_trader/test_kit/mocks/exec_clients.py
--rw-r--r--   0        0        0     6073 2023-05-05 11:18:34.905063 nautilus_trader-1.173.0/nautilus_trader/test_kit/mocks/strategies.py
--rw-r--r--   0        0        0     3079 2023-05-05 11:18:34.905063 nautilus_trader-1.173.0/nautilus_trader/test_kit/performance.py
--rw-r--r--   0        0        0    20761 2023-05-05 11:18:34.905063 nautilus_trader-1.173.0/nautilus_trader/test_kit/providers.py
--rw-r--r--   0        0        0     1276 2023-05-05 11:18:34.905063 nautilus_trader-1.173.0/nautilus_trader/test_kit/stubs/__init__.py
--rw-r--r--   0        0        0     4385 2023-05-05 11:18:34.905063 nautilus_trader-1.173.0/nautilus_trader/test_kit/stubs/commands.py
--rw-r--r--   0        0        0     6613 2023-05-05 11:18:34.905063 nautilus_trader-1.173.0/nautilus_trader/test_kit/stubs/component.py
--rw-r--r--   0        0        0     6247 2023-05-05 11:18:34.905063 nautilus_trader-1.173.0/nautilus_trader/test_kit/stubs/config.py
--rw-r--r--   0        0        0    18081 2023-05-05 11:18:34.905063 nautilus_trader-1.173.0/nautilus_trader/test_kit/stubs/data.py
--rw-r--r--   0        0        0    13185 2023-05-05 11:18:34.905063 nautilus_trader-1.173.0/nautilus_trader/test_kit/stubs/events.py
--rw-r--r--   0        0        0     6612 2023-05-05 11:18:34.905063 nautilus_trader-1.173.0/nautilus_trader/test_kit/stubs/execution.py
--rw-r--r--   0        0        0     3425 2023-05-05 11:18:34.905063 nautilus_trader-1.173.0/nautilus_trader/test_kit/stubs/identifiers.py
--rw-r--r--   0        0        0     2970 2023-05-05 11:18:34.905063 nautilus_trader-1.173.0/nautilus_trader/test_kit/stubs/persistence.py
--rw-r--r--   0        0        0      869 2023-05-05 11:18:34.905063 nautilus_trader-1.173.0/nautilus_trader/trading/__init__.pxd
--rw-r--r--   0        0        0     1145 2023-05-05 11:18:34.905063 nautilus_trader-1.173.0/nautilus_trader/trading/__init__.py
--rw-r--r--   0        0        0     2103 2023-05-05 11:18:34.905063 nautilus_trader-1.173.0/nautilus_trader/trading/filters.pxd
--rw-r--r--   0        0        0    16813 2023-05-05 11:18:34.905063 nautilus_trader-1.173.0/nautilus_trader/trading/filters.pyx
--rw-r--r--   0        0        0     6676 2023-05-05 11:18:34.905063 nautilus_trader-1.173.0/nautilus_trader/trading/strategy.pxd
--rw-r--r--   0        0        0    53498 2023-05-05 11:18:34.905063 nautilus_trader-1.173.0/nautilus_trader/trading/strategy.pyx
--rw-r--r--   0        0        0     3055 2023-05-05 11:18:34.905063 nautilus_trader-1.173.0/nautilus_trader/trading/trader.pxd
--rw-r--r--   0        0        0    20063 2023-05-05 11:18:34.905063 nautilus_trader-1.173.0/nautilus_trader/trading/trader.pyx
--rw-r--r--   0        0        0     7372 2023-05-05 11:18:34.909063 nautilus_trader-1.173.0/pyproject.toml
--rw-r--r--   0        0        0    25945 1970-01-01 00:00:00.000000 nautilus_trader-1.173.0/PKG-INFO
+-rw-r--r--   0        0        0     7652 2023-05-20 00:56:32.860015 nautilus_trader-1.174.0/LICENSE
+-rw-r--r--   0        0        0    23501 2023-05-20 00:56:32.860015 nautilus_trader-1.174.0/README.md
+-rw-r--r--   0        0        0    12291 2023-05-20 00:56:32.860015 nautilus_trader-1.174.0/build.py
+-rw-r--r--   0        0        0      663 2023-05-20 00:56:32.872015 nautilus_trader-1.174.0/nautilus_core/.cargo/config.toml
+-rw-r--r--   0        0        0       65 2023-05-20 00:56:32.872015 nautilus_trader-1.174.0/nautilus_core/.clippy.toml
+-rw-r--r--   0        0        0       37 2023-05-20 00:56:32.872015 nautilus_trader-1.174.0/nautilus_core/.rustfmt.toml
+-rw-r--r--   0        0        0    84260 2023-05-20 00:56:32.872015 nautilus_trader-1.174.0/nautilus_core/Cargo.lock
+-rw-r--r--   0        0        0     1612 2023-05-20 00:56:32.872015 nautilus_trader-1.174.0/nautilus_core/Cargo.toml
+-rw-r--r--   0        0        0     7652 2023-05-20 00:56:32.872015 nautilus_trader-1.174.0/nautilus_core/LICENSE
+-rw-r--r--   0        0        0     1248 2023-05-20 00:56:32.872015 nautilus_trader-1.174.0/nautilus_core/README.md
+-rw-r--r--   0        0        0      702 2023-05-20 00:56:32.872015 nautilus_trader-1.174.0/nautilus_core/backtest/Cargo.toml
+-rw-r--r--   0        0        0     1889 2023-05-20 00:56:32.872015 nautilus_trader-1.174.0/nautilus_core/backtest/build.rs
+-rw-r--r--   0        0        0      484 2023-05-20 00:56:32.872015 nautilus_trader-1.174.0/nautilus_core/backtest/cbindgen.toml
+-rw-r--r--   0        0        0      810 2023-05-20 00:56:32.872015 nautilus_trader-1.174.0/nautilus_core/backtest/cbindgen_cython.toml
+-rw-r--r--   0        0        0     5773 2023-05-20 00:56:32.872015 nautilus_trader-1.174.0/nautilus_core/backtest/src/engine.rs
+-rw-r--r--   0        0        0      900 2023-05-20 00:56:32.872015 nautilus_trader-1.174.0/nautilus_core/backtest/src/lib.rs
+-rw-r--r--   0        0        0      715 2023-05-20 00:56:32.872015 nautilus_trader-1.174.0/nautilus_core/common/Cargo.toml
+-rw-r--r--   0        0        0     2542 2023-05-20 00:56:32.872015 nautilus_trader-1.174.0/nautilus_core/common/build.rs
+-rw-r--r--   0        0        0      531 2023-05-20 00:56:32.872015 nautilus_trader-1.174.0/nautilus_core/common/cbindgen.toml
+-rw-r--r--   0        0        0      724 2023-05-20 00:56:32.872015 nautilus_trader-1.174.0/nautilus_core/common/cbindgen_cython.toml
+-rw-r--r--   0        0        0    25390 2023-05-20 00:56:32.872015 nautilus_trader-1.174.0/nautilus_core/common/src/clock.rs
+-rw-r--r--   0        0        0     6296 2023-05-20 00:56:32.872015 nautilus_trader-1.174.0/nautilus_core/common/src/enums.rs
+-rw-r--r--   0        0        0      979 2023-05-20 00:56:32.872015 nautilus_trader-1.174.0/nautilus_core/common/src/lib.rs
+-rw-r--r--   0        0        0    25121 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/common/src/logging.rs
+-rw-r--r--   0        0        0     7311 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/common/src/msgbus.rs
+-rw-r--r--   0        0        0     1299 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/common/src/testing.rs
+-rw-r--r--   0        0        0     8996 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/common/src/timer.rs
+-rw-r--r--   0        0        0     3091 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/common/tests/test_clock.rs
+-rw-r--r--   0        0        0      616 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/core/Cargo.toml
+-rw-r--r--   0        0        0     1234 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/core/benches/criterion_time_benchmark.rs
+-rw-r--r--   0        0        0     2538 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/core/build.rs
+-rw-r--r--   0        0        0      681 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/core/cbindgen.toml
+-rw-r--r--   0        0        0      791 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/core/cbindgen_cython.toml
+-rw-r--r--   0        0        0     7634 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/core/src/correctness.rs
+-rw-r--r--   0        0        0     5544 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/core/src/cvec.rs
+-rw-r--r--   0        0        0     5256 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/core/src/datetime.rs
+-rw-r--r--   0        0        0      998 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/core/src/lib.rs
+-rw-r--r--   0        0        0     4973 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/core/src/parsing.rs
+-rw-r--r--   0        0        0     5119 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/core/src/string.rs
+-rw-r--r--   0        0        0     5105 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/core/src/time.rs
+-rw-r--r--   0        0        0     7354 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/core/src/uuid.rs
+-rw-r--r--   0        0        0      497 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/indicators/Cargo.toml
+-rw-r--r--   0        0        0     4123 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/indicators/src/ema.rs
+-rw-r--r--   0        0        0     1289 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/indicators/src/lib.rs
+-rw-r--r--   0        0        0      765 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/model/Cargo.toml
+-rw-r--r--   0        0        0      399 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/model/benches/criterion_fixed_precision_benchmark.rs
+-rw-r--r--   0        0        0      225 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/model/benches/iai_fixed_precision_benchmark.rs
+-rw-r--r--   0        0        0     2540 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/model/build.rs
+-rw-r--r--   0        0        0     1084 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/model/cbindgen.toml
+-rw-r--r--   0        0        0     1304 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/model/cbindgen_cython.toml
+-rw-r--r--   0        0        0    21360 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/model/src/currencies.rs
+-rw-r--r--   0        0        0    19066 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/model/src/data/bar.rs
+-rw-r--r--   0        0        0    12419 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/model/src/data/book.rs
+-rw-r--r--   0        0        0     2119 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/model/src/data/mod.rs
+-rw-r--r--   0        0        0     9260 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/model/src/data/tick.rs
+-rw-r--r--   0        0        0    22849 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/model/src/enums.rs
+-rw-r--r--   0        0        0      917 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/model/src/events/mod.rs
+-rw-r--r--   0        0        0    10645 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/model/src/events/order.rs
+-rw-r--r--   0        0        0     3681 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/model/src/events/position.rs
+-rw-r--r--   0        0        0     7336 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/model/src/identifiers/account_id.rs
+-rw-r--r--   0        0        0     4804 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/model/src/identifiers/client_id.rs
+-rw-r--r--   0        0        0     4027 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/model/src/identifiers/client_order_id.rs
+-rw-r--r--   0        0        0     3834 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/model/src/identifiers/component_id.rs
+-rw-r--r--   0        0        0     3972 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/model/src/identifiers/exec_algorithm_id.rs
+-rw-r--r--   0        0        0     6257 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/model/src/identifiers/instrument_id.rs
+-rw-r--r--   0        0        0     1177 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/model/src/identifiers/mod.rs
+-rw-r--r--   0        0        0     3808 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/model/src/identifiers/order_list_id.rs
+-rw-r--r--   0        0        0     3800 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/model/src/identifiers/position_id.rs
+-rw-r--r--   0        0        0     3549 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/model/src/identifiers/strategy_id.rs
+-rw-r--r--   0        0        0     3642 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/model/src/identifiers/symbol.rs
+-rw-r--r--   0        0        0     3726 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/model/src/identifiers/trade_id.rs
+-rw-r--r--   0        0        0     3493 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/model/src/identifiers/trader_id.rs
+-rw-r--r--   0        0        0     3603 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/model/src/identifiers/venue.rs
+-rw-r--r--   0        0        0     3980 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/model/src/identifiers/venue_order_id.rs
+-rw-r--r--   0        0        0     1831 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/model/src/instruments/mod.rs
+-rw-r--r--   0        0        0     1357 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/model/src/lib.rs
+-rw-r--r--   0        0        0     3480 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/model/src/orderbook/book.rs
+-rw-r--r--   0        0        0    12899 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/model/src/orderbook/ladder.rs
+-rw-r--r--   0        0        0     7569 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/model/src/orderbook/level.rs
+-rw-r--r--   0        0        0      929 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/model/src/orderbook/mod.rs
+-rw-r--r--   0        0        0     4637 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/model/src/orders/limit.rs
+-rw-r--r--   0        0        0    27273 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/model/src/orders/mod.rs
+-rw-r--r--   0        0        0     7685 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/model/src/position.rs
+-rw-r--r--   0        0        0     1358 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/model/src/types/balance.rs
+-rw-r--r--   0        0        0     5219 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/model/src/types/currency.rs
+-rw-r--r--   0        0        0     6164 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/model/src/types/fixed.rs
+-rw-r--r--   0        0        0      982 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/model/src/types/mod.rs
+-rw-r--r--   0        0        0     7444 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/model/src/types/money.rs
+-rw-r--r--   0        0        0    10073 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/model/src/types/price.rs
+-rw-r--r--   0        0        0    10189 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/model/src/types/quantity.rs
+-rw-r--r--   0        0        0      624 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/network/Cargo.toml
+-rw-r--r--   0        0        0     1539 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/network/benches/bench_client.rs
+-rw-r--r--   0        0        0    14287 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/network/src/lib.rs
+-rw-r--r--   0        0        0      509 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/network/tests/test_http.py
+-rw-r--r--   0        0        0     1052 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/persistence/Cargo.toml
+-rw-r--r--   0        0        0     3291 2023-05-20 00:56:32.876015 nautilus_trader-1.174.0/nautilus_core/persistence/benches/persistence_benchmark.rs
+-rw-r--r--   0        0        0     6101 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_core/persistence/src/kmerge_batch.rs
+-rw-r--r--   0        0        0     1285 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_core/persistence/src/lib.rs
+-rw-r--r--   0        0        0     6931 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_core/persistence/src/parquet/implementations/bar.rs
+-rw-r--r--   0        0        0     8338 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_core/persistence/src/parquet/implementations/book_delta.rs
+-rw-r--r--   0        0        0     6895 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_core/persistence/src/parquet/implementations/book_snapshot.rs
+-rw-r--r--   0        0        0      950 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_core/persistence/src/parquet/implementations/mod.rs
+-rw-r--r--   0        0        0     6601 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_core/persistence/src/parquet/implementations/quote.rs
+-rw-r--r--   0        0        0     6988 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_core/persistence/src/parquet/implementations/trade.rs
+-rw-r--r--   0        0        0     1680 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_core/persistence/src/parquet/mod.rs
+-rw-r--r--   0        0        0    11980 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_core/persistence/src/session.rs
+-rw-r--r--   0        0        0     3549 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_core/persistence/tests/test_catalog.rs
+-rw-r--r--   0        0        0     2906 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_core/persistence/tests/test_persistence_module.py
+-rw-r--r--   0        0        0     2179 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_core/persistence/tests/test_util.rs
+-rw-r--r--   0        0        0      647 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_core/pyo3/Cargo.toml
+-rw-r--r--   0        0        0     2275 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_core/pyo3/src/lib.rs
+-rw-r--r--   0        0        0       50 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_core/rust-toolchain.toml
+-rw-r--r--   0        0        0      869 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_trader/__init__.pxd
+-rw-r--r--   0        0        0     1268 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_trader/__init__.py
+-rw-r--r--   0        0        0      869 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_trader/accounting/__init__.pxd
+-rw-r--r--   0        0        0     1414 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_trader/accounting/__init__.py
+-rw-r--r--   0        0        0      869 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_trader/accounting/accounts/__init__.pxd
+-rw-r--r--   0        0        0      869 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_trader/accounting/accounts/__init__.py
+-rw-r--r--   0        0        0     3970 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_trader/accounting/accounts/base.pxd
+-rw-r--r--   0        0        0    14287 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_trader/accounting/accounts/base.pyx
+-rw-r--r--   0        0        0     1442 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_trader/accounting/accounts/betting.pxd
+-rw-r--r--   0        0        0     2758 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_trader/accounting/accounts/betting.pyx
+-rw-r--r--   0        0        0     1881 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_trader/accounting/accounts/cash.pxd
+-rw-r--r--   0        0        0    11292 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_trader/accounting/accounts/cash.pyx
+-rw-r--r--   0        0        0     3168 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_trader/accounting/accounts/margin.pxd
+-rw-r--r--   0        0        0    20650 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_trader/accounting/accounts/margin.pyx
+-rw-r--r--   0        0        0     1488 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_trader/accounting/calculators.pxd
+-rw-r--r--   0        0        0    10743 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_trader/accounting/calculators.pyx
+-rw-r--r--   0        0        0     2111 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_trader/accounting/error.py
+-rw-r--r--   0        0        0     1089 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_trader/accounting/factory.pxd
+-rw-r--r--   0        0        0     4063 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_trader/accounting/factory.pyx
+-rw-r--r--   0        0        0     2659 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_trader/accounting/manager.pxd
+-rw-r--r--   0        0        0    22701 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_trader/accounting/manager.pyx
+-rw-r--r--   0        0        0     1153 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_trader/adapters/__init__.py
+-rw-r--r--   0        0        0      869 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_trader/adapters/_template/__init__.py
+-rw-r--r--   0        0        0     1013 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_trader/adapters/_template/core.py
+-rw-r--r--   0        0        0    13300 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_trader/adapters/_template/data.py
+-rw-r--r--   0        0        0     6617 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_trader/adapters/_template/execution.py
+-rw-r--r--   0        0        0     2461 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_trader/adapters/_template/providers.py
+-rw-r--r--   0        0        0      946 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_trader/adapters/betfair/__init__.py
+-rw-r--r--   0        0        0      869 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_trader/adapters/betfair/client/__init__.py
+-rw-r--r--   0        0        0    11390 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_trader/adapters/betfair/client/core.py
+-rw-r--r--   0        0        0     2278 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_trader/adapters/betfair/client/enums.py
+-rw-r--r--   0        0        0     3484 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_trader/adapters/betfair/client/exceptions.py
+-rw-r--r--   0        0        0     2395 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_trader/adapters/betfair/client/spec.py
+-rw-r--r--   0        0        0     2725 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_trader/adapters/betfair/client/util.py
+-rw-r--r--   0        0        0     2856 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_trader/adapters/betfair/common.py
+-rw-r--r--   0        0        0     2342 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_trader/adapters/betfair/config.py
+-rw-r--r--   0        0        0     2056 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_trader/adapters/betfair/constants.py
+-rw-r--r--   0        0        0    12896 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_trader/adapters/betfair/data.py
+-rw-r--r--   0        0        0     7912 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_trader/adapters/betfair/data_types.py
+-rw-r--r--   0        0        0    41691 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_trader/adapters/betfair/execution.py
+-rw-r--r--   0        0        0     8697 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_trader/adapters/betfair/factories.py
+-rw-r--r--   0        0        0     2919 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_trader/adapters/betfair/historic.py
+-rw-r--r--   0        0        0     1271 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_trader/adapters/betfair/orderbook.pxd
+-rw-r--r--   0        0        0     2017 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_trader/adapters/betfair/orderbook.pyx
+-rw-r--r--   0        0        0      869 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_trader/adapters/betfair/parsing/__init__.py
+-rw-r--r--   0        0        0     2557 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_trader/adapters/betfair/parsing/common.py
+-rw-r--r--   0        0        0     2151 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_trader/adapters/betfair/parsing/core.py
+-rw-r--r--   0        0        0    12500 2023-05-20 00:56:32.880015 nautilus_trader-1.174.0/nautilus_trader/adapters/betfair/parsing/requests.py
+-rw-r--r--   0        0        0    24123 2023-05-20 00:56:32.884015 nautilus_trader-1.174.0/nautilus_trader/adapters/betfair/parsing/streaming.py
+-rw-r--r--   0        0        0    13206 2023-05-20 00:56:32.884015 nautilus_trader-1.174.0/nautilus_trader/adapters/betfair/providers.py
+-rw-r--r--   0        0        0     7303 2023-05-20 00:56:32.884015 nautilus_trader-1.174.0/nautilus_trader/adapters/betfair/sockets.py
+-rw-r--r--   0        0        0      939 2023-05-20 00:56:32.884015 nautilus_trader-1.174.0/nautilus_trader/adapters/binance/__init__.py
+-rw-r--r--   0        0        0      869 2023-05-20 00:56:32.884015 nautilus_trader-1.174.0/nautilus_trader/adapters/binance/common/__init__.py
+-rw-r--r--   0        0        0      957 2023-05-20 00:56:32.884015 nautilus_trader-1.174.0/nautilus_trader/adapters/binance/common/constants.py
+-rw-r--r--   0        0        0    27093 2023-05-20 00:56:32.884015 nautilus_trader-1.174.0/nautilus_trader/adapters/binance/common/data.py
+-rw-r--r--   0        0        0    11975 2023-05-20 00:56:32.884015 nautilus_trader-1.174.0/nautilus_trader/adapters/binance/common/enums.py
+-rw-r--r--   0        0        0    35889 2023-05-20 00:56:32.884015 nautilus_trader-1.174.0/nautilus_trader/adapters/binance/common/execution.py
+-rw-r--r--   0        0        0      869 2023-05-20 00:56:32.884015 nautilus_trader-1.174.0/nautilus_trader/adapters/binance/common/schemas/__init__.py
+-rw-r--r--   0        0        0    10209 2023-05-20 00:56:32.884015 nautilus_trader-1.174.0/nautilus_trader/adapters/binance/common/schemas/account.py
+-rw-r--r--   0        0        0    21194 2023-05-20 00:56:32.884015 nautilus_trader-1.174.0/nautilus_trader/adapters/binance/common/schemas/market.py
+-rw-r--r--   0        0        0     2434 2023-05-20 00:56:32.884015 nautilus_trader-1.174.0/nautilus_trader/adapters/binance/common/schemas/symbol.py
+-rw-r--r--   0        0        0     1199 2023-05-20 00:56:32.884015 nautilus_trader-1.174.0/nautilus_trader/adapters/binance/common/schemas/user.py
+-rw-r--r--   0        0        0    14983 2023-05-20 00:56:32.884015 nautilus_trader-1.174.0/nautilus_trader/adapters/binance/common/types.py
+-rw-r--r--   0        0        0     4013 2023-05-20 00:56:32.884015 nautilus_trader-1.174.0/nautilus_trader/adapters/binance/config.py
+-rw-r--r--   0        0        0    17023 2023-05-20 00:56:32.884015 nautilus_trader-1.174.0/nautilus_trader/adapters/binance/factories.py
+-rw-r--r--   0        0        0      869 2023-05-20 00:56:32.884015 nautilus_trader-1.174.0/nautilus_trader/adapters/binance/futures/__init__.py
+-rw-r--r--   0        0        0     8782 2023-05-20 00:56:32.884015 nautilus_trader-1.174.0/nautilus_trader/adapters/binance/futures/data.py
+-rw-r--r--   0        0        0     6746 2023-05-20 00:56:32.884015 nautilus_trader-1.174.0/nautilus_trader/adapters/binance/futures/enums.py
+-rw-r--r--   0        0        0    12284 2023-05-20 00:56:32.884015 nautilus_trader-1.174.0/nautilus_trader/adapters/binance/futures/execution.py
+-rw-r--r--   0        0        0      869 2023-05-20 00:56:32.884015 nautilus_trader-1.174.0/nautilus_trader/adapters/binance/futures/http/__init__.py
+-rw-r--r--   0        0        0    13354 2023-05-20 00:56:32.884015 nautilus_trader-1.174.0/nautilus_trader/adapters/binance/futures/http/account.py
+-rw-r--r--   0        0        0     3646 2023-05-20 00:56:32.884015 nautilus_trader-1.174.0/nautilus_trader/adapters/binance/futures/http/market.py
+-rw-r--r--   0        0        0     1964 2023-05-20 00:56:32.884015 nautilus_trader-1.174.0/nautilus_trader/adapters/binance/futures/http/user.py
+-rw-r--r--   0        0        0     4884 2023-05-20 00:56:32.884015 nautilus_trader-1.174.0/nautilus_trader/adapters/binance/futures/http/wallet.py
+-rw-r--r--   0        0        0    16539 2023-05-20 00:56:32.884015 nautilus_trader-1.174.0/nautilus_trader/adapters/binance/futures/providers.py
+-rw-r--r--   0        0        0      869 2023-05-20 00:56:32.884015 nautilus_trader-1.174.0/nautilus_trader/adapters/binance/futures/schemas/__init__.py
+-rw-r--r--   0        0        0     6885 2023-05-20 00:56:32.884015 nautilus_trader-1.174.0/nautilus_trader/adapters/binance/futures/schemas/account.py
+-rw-r--r--   0        0        0     7594 2023-05-20 00:56:32.884015 nautilus_trader-1.174.0/nautilus_trader/adapters/binance/futures/schemas/market.py
+-rw-r--r--   0        0        0    13834 2023-05-20 00:56:32.884015 nautilus_trader-1.174.0/nautilus_trader/adapters/binance/futures/schemas/user.py
+-rw-r--r--   0        0        0     1271 2023-05-20 00:56:32.884015 nautilus_trader-1.174.0/nautilus_trader/adapters/binance/futures/schemas/wallet.py
+-rw-r--r--   0        0        0     4630 2023-05-20 00:56:32.884015 nautilus_trader-1.174.0/nautilus_trader/adapters/binance/futures/types.py
+-rw-r--r--   0        0        0      869 2023-05-20 00:56:32.884015 nautilus_trader-1.174.0/nautilus_trader/adapters/binance/http/__init__.py
+-rw-r--r--   0        0        0    24541 2023-05-20 00:56:32.884015 nautilus_trader-1.174.0/nautilus_trader/adapters/binance/http/account.py
+-rw-r--r--   0        0        0     6438 2023-05-20 00:56:32.884015 nautilus_trader-1.174.0/nautilus_trader/adapters/binance/http/client.py
+-rw-r--r--   0        0        0     3226 2023-05-20 00:56:32.884015 nautilus_trader-1.174.0/nautilus_trader/adapters/binance/http/endpoint.py
+-rw-r--r--   0        0        0     1558 2023-05-20 00:56:32.884015 nautilus_trader-1.174.0/nautilus_trader/adapters/binance/http/error.py
+-rw-r--r--   0        0        0    31639 2023-05-20 00:56:32.884015 nautilus_trader-1.174.0/nautilus_trader/adapters/binance/http/market.py
+-rw-r--r--   0        0        0     7778 2023-05-20 00:56:32.884015 nautilus_trader-1.174.0/nautilus_trader/adapters/binance/http/user.py
+-rw-r--r--   0        0        0      869 2023-05-20 00:56:32.884015 nautilus_trader-1.174.0/nautilus_trader/adapters/binance/spot/__init__.py
+-rw-r--r--   0        0        0     5852 2023-05-20 00:56:32.884015 nautilus_trader-1.174.0/nautilus_trader/adapters/binance/spot/data.py
+-rw-r--r--   0        0        0     4799 2023-05-20 00:56:32.884015 nautilus_trader-1.174.0/nautilus_trader/adapters/binance/spot/enums.py
+-rw-r--r--   0        0        0     9847 2023-05-20 00:56:32.884015 nautilus_trader-1.174.0/nautilus_trader/adapters/binance/spot/execution.py
+-rw-r--r--   0        0        0      869 2023-05-20 00:56:32.884015 nautilus_trader-1.174.0/nautilus_trader/adapters/binance/spot/http/__init__.py
+-rw-r--r--   0        0        0    26424 2023-05-20 00:56:32.884015 nautilus_trader-1.174.0/nautilus_trader/adapters/binance/spot/http/account.py
+-rw-r--r--   0        0        0     6709 2023-05-20 00:56:32.884015 nautilus_trader-1.174.0/nautilus_trader/adapters/binance/spot/http/market.py
+-rw-r--r--   0        0        0     1973 2023-05-20 00:56:32.884015 nautilus_trader-1.174.0/nautilus_trader/adapters/binance/spot/http/user.py
+-rw-r--r--   0        0        0     4669 2023-05-20 00:56:32.884015 nautilus_trader-1.174.0/nautilus_trader/adapters/binance/spot/http/wallet.py
+-rw-r--r--   0        0        0    13617 2023-05-20 00:56:32.884015 nautilus_trader-1.174.0/nautilus_trader/adapters/binance/spot/providers.py
+-rw-r--r--   0        0        0      869 2023-05-20 00:56:32.884015 nautilus_trader-1.174.0/nautilus_trader/adapters/binance/spot/schemas/__init__.py
+-rw-r--r--   0        0        0     3299 2023-05-20 00:56:32.884015 nautilus_trader-1.174.0/nautilus_trader/adapters/binance/spot/schemas/account.py
+-rw-r--r--   0        0        0     6189 2023-05-20 00:56:32.884015 nautilus_trader-1.174.0/nautilus_trader/adapters/binance/spot/schemas/market.py
+-rw-r--r--   0        0        0    11677 2023-05-20 00:56:32.884015 nautilus_trader-1.174.0/nautilus_trader/adapters/binance/spot/schemas/user.py
+-rw-r--r--   0        0        0     1252 2023-05-20 00:56:32.884015 nautilus_trader-1.174.0/nautilus_trader/adapters/binance/spot/schemas/wallet.py
+-rw-r--r--   0        0        0      869 2023-05-20 00:56:32.884015 nautilus_trader-1.174.0/nautilus_trader/adapters/binance/websocket/__init__.py
+-rw-r--r--   0        0        0     7670 2023-05-20 00:56:32.884015 nautilus_trader-1.174.0/nautilus_trader/adapters/binance/websocket/client.py
+-rw-r--r--   0        0        0      869 2023-05-20 00:56:32.884015 nautilus_trader-1.174.0/nautilus_trader/adapters/deribit/__init__.py
+-rw-r--r--   0        0        0      869 2023-05-20 00:56:32.888015 nautilus_trader-1.174.0/nautilus_trader/adapters/deribit/http/__init__.py
+-rw-r--r--   0        0        0     5601 2023-05-20 00:56:32.888015 nautilus_trader-1.174.0/nautilus_trader/adapters/deribit/http/client.py
+-rw-r--r--   0        0        0     1554 2023-05-20 00:56:32.888015 nautilus_trader-1.174.0/nautilus_trader/adapters/deribit/http/error.py
+-rw-r--r--   0        0        0      931 2023-05-20 00:56:32.888015 nautilus_trader-1.174.0/nautilus_trader/adapters/interactive_brokers/__init__.py
+-rw-r--r--   0        0        0     1299 2023-05-20 00:56:32.888015 nautilus_trader-1.174.0/nautilus_trader/adapters/interactive_brokers/common.py
+-rw-r--r--   0        0        0     4009 2023-05-20 00:56:32.888015 nautilus_trader-1.174.0/nautilus_trader/adapters/interactive_brokers/config.py
+-rw-r--r--   0        0        0    21104 2023-05-20 00:56:32.888015 nautilus_trader-1.174.0/nautilus_trader/adapters/interactive_brokers/data.py
+-rw-r--r--   0        0        0    16801 2023-05-20 00:56:32.888015 nautilus_trader-1.174.0/nautilus_trader/adapters/interactive_brokers/execution.py
+-rw-r--r--   0        0        0     9905 2023-05-20 00:56:32.888015 nautilus_trader-1.174.0/nautilus_trader/adapters/interactive_brokers/factories.py
+-rw-r--r--   0        0        0     6745 2023-05-20 00:56:32.888015 nautilus_trader-1.174.0/nautilus_trader/adapters/interactive_brokers/gateway.py
+-rw-r--r--   0        0        0    14016 2023-05-20 00:56:32.888015 nautilus_trader-1.174.0/nautilus_trader/adapters/interactive_brokers/historic.py
+-rw-r--r--   0        0        0      869 2023-05-20 00:56:32.888015 nautilus_trader-1.174.0/nautilus_trader/adapters/interactive_brokers/parsing/__init__.py
+-rw-r--r--   0        0        0     3911 2023-05-20 00:56:32.888015 nautilus_trader-1.174.0/nautilus_trader/adapters/interactive_brokers/parsing/data.py
+-rw-r--r--   0        0        0     4905 2023-05-20 00:56:32.888015 nautilus_trader-1.174.0/nautilus_trader/adapters/interactive_brokers/parsing/execution.py
+-rw-r--r--   0        0        0     8268 2023-05-20 00:56:32.888015 nautilus_trader-1.174.0/nautilus_trader/adapters/interactive_brokers/parsing/instruments.py
+-rw-r--r--   0        0        0     9210 2023-05-20 00:56:32.888015 nautilus_trader-1.174.0/nautilus_trader/adapters/interactive_brokers/providers.py
+-rw-r--r--   0        0        0     4646 2023-05-20 00:56:32.888015 nautilus_trader-1.174.0/nautilus_trader/adapters/interactive_brokers/web.py
+-rw-r--r--   0        0        0      869 2023-05-20 00:56:32.888015 nautilus_trader-1.174.0/nautilus_trader/adapters/sandbox/__init__.py
+-rw-r--r--   0        0        0     1393 2023-05-20 00:56:32.888015 nautilus_trader-1.174.0/nautilus_trader/adapters/sandbox/config.py
+-rw-r--r--   0        0        0     7814 2023-05-20 00:56:32.888015 nautilus_trader-1.174.0/nautilus_trader/adapters/sandbox/execution.py
+-rw-r--r--   0        0        0     2693 2023-05-20 00:56:32.888015 nautilus_trader-1.174.0/nautilus_trader/adapters/sandbox/factory.py
+-rw-r--r--   0        0        0      979 2023-05-20 00:56:32.888015 nautilus_trader-1.174.0/nautilus_trader/analysis/__init__.py
+-rw-r--r--   0        0        0    15157 2023-05-20 00:56:32.888015 nautilus_trader-1.174.0/nautilus_trader/analysis/analyzer.py
+-rw-r--r--   0        0        0     4714 2023-05-20 00:56:32.888015 nautilus_trader-1.174.0/nautilus_trader/analysis/reporter.py
+-rw-r--r--   0        0        0     3968 2023-05-20 00:56:32.888015 nautilus_trader-1.174.0/nautilus_trader/analysis/statistic.py
+-rw-r--r--   0        0        0     2255 2023-05-20 00:56:32.888015 nautilus_trader-1.174.0/nautilus_trader/analysis/statistics/__init__.py
+-rw-r--r--   0        0        0     2016 2023-05-20 00:56:32.888015 nautilus_trader-1.174.0/nautilus_trader/analysis/statistics/expectancy.py
+-rw-r--r--   0        0        0     1717 2023-05-20 00:56:32.888015 nautilus_trader-1.174.0/nautilus_trader/analysis/statistics/long_ratio.py
+-rw-r--r--   0        0        0     1481 2023-05-20 00:56:32.888015 nautilus_trader-1.174.0/nautilus_trader/analysis/statistics/loser_avg.py
+-rw-r--r--   0        0        0     1527 2023-05-20 00:56:32.888015 nautilus_trader-1.174.0/nautilus_trader/analysis/statistics/loser_max.py
+-rw-r--r--   0        0        0     1525 2023-05-20 00:56:32.888015 nautilus_trader-1.174.0/nautilus_trader/analysis/statistics/loser_min.py
+-rw-r--r--   0        0        0     1576 2023-05-20 00:56:32.888015 nautilus_trader-1.174.0/nautilus_trader/analysis/statistics/profit_factor.py
+-rw-r--r--   0        0        0     1412 2023-05-20 00:56:32.888015 nautilus_trader-1.174.0/nautilus_trader/analysis/statistics/returns_avg.py
+-rw-r--r--   0        0        0     1427 2023-05-20 00:56:32.888015 nautilus_trader-1.174.0/nautilus_trader/analysis/statistics/returns_avg_loss.py
+-rw-r--r--   0        0        0     1426 2023-05-20 00:56:32.888015 nautilus_trader-1.174.0/nautilus_trader/analysis/statistics/returns_avg_win.py
+-rw-r--r--   0        0        0     1728 2023-05-20 00:56:32.888015 nautilus_trader-1.174.0/nautilus_trader/analysis/statistics/returns_volatility.py
+-rw-r--r--   0        0        0     1336 2023-05-20 00:56:32.888015 nautilus_trader-1.174.0/nautilus_trader/analysis/statistics/risk_return_ratio.py
+-rw-r--r--   0        0        0     1788 2023-05-20 00:56:32.888015 nautilus_trader-1.174.0/nautilus_trader/analysis/statistics/sharpe_ratio.py
+-rw-r--r--   0        0        0     1895 2023-05-20 00:56:32.888015 nautilus_trader-1.174.0/nautilus_trader/analysis/statistics/sortino_ratio.py
+-rw-r--r--   0        0        0     1511 2023-05-20 00:56:32.888015 nautilus_trader-1.174.0/nautilus_trader/analysis/statistics/win_rate.py
+-rw-r--r--   0        0        0     1502 2023-05-20 00:56:32.888015 nautilus_trader-1.174.0/nautilus_trader/analysis/statistics/winner_avg.py
+-rw-r--r--   0        0        0     1360 2023-05-20 00:56:32.888015 nautilus_trader-1.174.0/nautilus_trader/analysis/statistics/winner_max.py
+-rw-r--r--   0        0        0     1507 2023-05-20 00:56:32.888015 nautilus_trader-1.174.0/nautilus_trader/analysis/statistics/winner_min.py
+-rw-r--r--   0        0        0      869 2023-05-20 00:56:32.888015 nautilus_trader-1.174.0/nautilus_trader/backtest/__init__.pxd
+-rw-r--r--   0        0        0      945 2023-05-20 00:56:32.888015 nautilus_trader-1.174.0/nautilus_trader/backtest/__init__.py
+-rw-r--r--   0        0        0     1710 2023-05-20 00:56:32.888015 nautilus_trader-1.174.0/nautilus_trader/backtest/__main__.py
+-rw-r--r--   0        0        0     3874 2023-05-20 00:56:32.888015 nautilus_trader-1.174.0/nautilus_trader/backtest/auction.py
+-rw-r--r--   0        0        0     1100 2023-05-20 00:56:32.888015 nautilus_trader-1.174.0/nautilus_trader/backtest/data_client.pxd
+-rw-r--r--   0        0        0    12847 2023-05-20 00:56:32.888015 nautilus_trader-1.174.0/nautilus_trader/backtest/data_client.pyx
+-rw-r--r--   0        0        0     2164 2023-05-20 00:56:32.888015 nautilus_trader-1.174.0/nautilus_trader/backtest/engine.pxd
+-rw-r--r--   0        0        0    46027 2023-05-20 00:56:32.888015 nautilus_trader-1.174.0/nautilus_trader/backtest/engine.pyx
+-rw-r--r--   0        0        0     6839 2023-05-20 00:56:32.888015 nautilus_trader-1.174.0/nautilus_trader/backtest/exchange.pxd
+-rw-r--r--   0        0        0    28471 2023-05-20 00:56:32.888015 nautilus_trader-1.174.0/nautilus_trader/backtest/exchange.pyx
+-rw-r--r--   0        0        0     1084 2023-05-20 00:56:32.888015 nautilus_trader-1.174.0/nautilus_trader/backtest/execution_client.pxd
+-rw-r--r--   0        0        0     5182 2023-05-20 00:56:32.888015 nautilus_trader-1.174.0/nautilus_trader/backtest/execution_client.pyx
+-rw-r--r--   0        0        0    11198 2023-05-20 00:56:32.888015 nautilus_trader-1.174.0/nautilus_trader/backtest/matching_engine.pxd
+-rw-r--r--   0        0        0    85772 2023-05-20 00:56:32.888015 nautilus_trader-1.174.0/nautilus_trader/backtest/matching_engine.pyx
+-rw-r--r--   0        0        0     2075 2023-05-20 00:56:32.888015 nautilus_trader-1.174.0/nautilus_trader/backtest/models.pxd
+-rw-r--r--   0        0        0     5344 2023-05-20 00:56:32.892015 nautilus_trader-1.174.0/nautilus_trader/backtest/models.pyx
+-rw-r--r--   0        0        0     1814 2023-05-20 00:56:32.892015 nautilus_trader-1.174.0/nautilus_trader/backtest/modules.pxd
+-rw-r--r--   0        0        0     8294 2023-05-20 00:56:32.892015 nautilus_trader-1.174.0/nautilus_trader/backtest/modules.pyx
+-rw-r--r--   0        0        0    11400 2023-05-20 00:56:32.892015 nautilus_trader-1.174.0/nautilus_trader/backtest/node.py
+-rw-r--r--   0        0        0     3110 2023-05-20 00:56:32.892015 nautilus_trader-1.174.0/nautilus_trader/backtest/results.py
+-rw-r--r--   0        0        0      869 2023-05-20 00:56:32.892015 nautilus_trader-1.174.0/nautilus_trader/cache/__init__.pxd
+-rw-r--r--   0        0        0     1052 2023-05-20 00:56:32.892015 nautilus_trader-1.174.0/nautilus_trader/cache/__init__.py
+-rw-r--r--   0        0        0     9896 2023-05-20 00:56:32.892015 nautilus_trader-1.174.0/nautilus_trader/cache/base.pxd
+-rw-r--r--   0        0        0    23040 2023-05-20 00:56:32.892015 nautilus_trader-1.174.0/nautilus_trader/cache/base.pyx
+-rw-r--r--   0        0        0     7346 2023-05-20 00:56:32.892015 nautilus_trader-1.174.0/nautilus_trader/cache/cache.pxd
+-rw-r--r--   0        0        0   122388 2023-05-20 00:56:32.892015 nautilus_trader-1.174.0/nautilus_trader/cache/cache.pyx
+-rw-r--r--   0        0        0     3663 2023-05-20 00:56:32.892015 nautilus_trader-1.174.0/nautilus_trader/cache/database.pxd
+-rw-r--r--   0        0        0     9114 2023-05-20 00:56:32.892015 nautilus_trader-1.174.0/nautilus_trader/cache/database.pyx
+-rw-r--r--   0        0        0      869 2023-05-20 00:56:32.892015 nautilus_trader-1.174.0/nautilus_trader/common/__init__.pxd
+-rw-r--r--   0        0        0     1571 2023-05-20 00:56:32.892015 nautilus_trader-1.174.0/nautilus_trader/common/__init__.py
+-rw-r--r--   0        0        0     9919 2023-05-20 00:56:32.892015 nautilus_trader-1.174.0/nautilus_trader/common/actor.pxd
+-rw-r--r--   0        0        0    73833 2023-05-20 00:56:32.892015 nautilus_trader-1.174.0/nautilus_trader/common/actor.pyx
+-rw-r--r--   0        0        0     3551 2023-05-20 00:56:32.892015 nautilus_trader-1.174.0/nautilus_trader/common/clock.pxd
+-rw-r--r--   0        0        0    27216 2023-05-20 00:56:32.892015 nautilus_trader-1.174.0/nautilus_trader/common/clock.pyx
+-rw-r--r--   0        0        0     2916 2023-05-20 00:56:32.892015 nautilus_trader-1.174.0/nautilus_trader/common/component.pxd
+-rw-r--r--   0        0        0    19989 2023-05-20 00:56:32.892015 nautilus_trader-1.174.0/nautilus_trader/common/component.pyx
+-rw-r--r--   0        0        0     1836 2023-05-20 00:56:32.892015 nautilus_trader-1.174.0/nautilus_trader/common/enums.pyx
+-rw-r--r--   0        0        0     1518 2023-05-20 00:56:32.892015 nautilus_trader-1.174.0/nautilus_trader/common/enums_c.pxd
+-rw-r--r--   0        0        0     2638 2023-05-20 00:56:32.892015 nautilus_trader-1.174.0/nautilus_trader/common/enums_c.pyx
+-rw-r--r--   0        0        0     8599 2023-05-20 00:56:32.892015 nautilus_trader-1.174.0/nautilus_trader/common/factories.pxd
+-rw-r--r--   0        0        0    51638 2023-05-20 00:56:32.892015 nautilus_trader-1.174.0/nautilus_trader/common/factories.pyx
+-rw-r--r--   0        0        0     1320 2023-05-20 00:56:32.892015 nautilus_trader-1.174.0/nautilus_trader/common/functions.py
+-rw-r--r--   0        0        0     2139 2023-05-20 00:56:32.892015 nautilus_trader-1.174.0/nautilus_trader/common/generators.pxd
+-rw-r--r--   0        0        0     7837 2023-05-20 00:56:32.892015 nautilus_trader-1.174.0/nautilus_trader/common/generators.pyx
+-rw-r--r--   0        0        0     2460 2023-05-20 00:56:32.892015 nautilus_trader-1.174.0/nautilus_trader/common/logging.pxd
+-rw-r--r--   0        0        0    18699 2023-05-20 00:56:32.892015 nautilus_trader-1.174.0/nautilus_trader/common/logging.pyx
+-rw-r--r--   0        0        0     2421 2023-05-20 00:56:32.892015 nautilus_trader-1.174.0/nautilus_trader/common/messages.pxd
+-rw-r--r--   0        0        0    10632 2023-05-20 00:56:32.892015 nautilus_trader-1.174.0/nautilus_trader/common/messages.pyx
+-rw-r--r--   0        0        0    10746 2023-05-20 00:56:32.892015 nautilus_trader-1.174.0/nautilus_trader/common/providers.py
+-rw-r--r--   0        0        0     1566 2023-05-20 00:56:32.892015 nautilus_trader-1.174.0/nautilus_trader/common/queue.pxd
+-rw-r--r--   0        0        0     5704 2023-05-20 00:56:32.892015 nautilus_trader-1.174.0/nautilus_trader/common/queue.pyx
+-rw-r--r--   0        0        0     2440 2023-05-20 00:56:32.892015 nautilus_trader-1.174.0/nautilus_trader/common/throttler.pxd
+-rw-r--r--   0        0        0     7418 2023-05-20 00:56:32.892015 nautilus_trader-1.174.0/nautilus_trader/common/throttler.pyx
+-rw-r--r--   0        0        0     2482 2023-05-20 00:56:32.892015 nautilus_trader-1.174.0/nautilus_trader/common/timer.pxd
+-rw-r--r--   0        0        0    11992 2023-05-20 00:56:32.892015 nautilus_trader-1.174.0/nautilus_trader/common/timer.pyx
+-rw-r--r--   0        0        0     3793 2023-05-20 00:56:32.892015 nautilus_trader-1.174.0/nautilus_trader/config/__init__.py
+-rw-r--r--   0        0        0     9917 2023-05-20 00:56:32.892015 nautilus_trader-1.174.0/nautilus_trader/config/backtest.py
+-rw-r--r--   0        0        0    19918 2023-05-20 00:56:32.892015 nautilus_trader-1.174.0/nautilus_trader/config/common.py
+-rw-r--r--   0        0        0     1015 2023-05-20 00:56:32.892015 nautilus_trader-1.174.0/nautilus_trader/config/error.py
+-rw-r--r--   0        0        0     7535 2023-05-20 00:56:32.892015 nautilus_trader-1.174.0/nautilus_trader/config/live.py
+-rw-r--r--   0        0        0     1264 2023-05-20 00:56:32.892015 nautilus_trader-1.174.0/nautilus_trader/config/validation.py
+-rw-r--r--   0        0        0      869 2023-05-20 00:56:32.892015 nautilus_trader-1.174.0/nautilus_trader/core/__init__.pxd
+-rw-r--r--   0        0        0     1339 2023-05-20 00:56:32.892015 nautilus_trader-1.174.0/nautilus_trader/core/__init__.py
+-rw-r--r--   0        0        0     1230 2023-05-20 00:56:32.892015 nautilus_trader-1.174.0/nautilus_trader/core/asynchronous.py
+-rw-r--r--   0        0        0     3628 2023-05-20 00:56:32.892015 nautilus_trader-1.174.0/nautilus_trader/core/correctness.pxd
+-rw-r--r--   0        0        0    37204 2023-05-20 00:56:32.892015 nautilus_trader-1.174.0/nautilus_trader/core/correctness.pyx
+-rw-r--r--   0        0        0     1191 2023-05-20 00:56:32.896015 nautilus_trader-1.174.0/nautilus_trader/core/data.pxd
+-rw-r--r--   0        0        0     2665 2023-05-20 00:56:32.896015 nautilus_trader-1.174.0/nautilus_trader/core/data.pyx
+-rw-r--r--   0        0        0     1680 2023-05-20 00:56:32.896015 nautilus_trader-1.174.0/nautilus_trader/core/datetime.pxd
+-rw-r--r--   0        0        0     9470 2023-05-20 00:56:32.896015 nautilus_trader-1.174.0/nautilus_trader/core/datetime.pyx
+-rw-r--r--   0        0        0     1230 2023-05-20 00:56:32.896015 nautilus_trader-1.174.0/nautilus_trader/core/fsm.pxd
+-rw-r--r--   0        0        0     4364 2023-05-20 00:56:32.896015 nautilus_trader-1.174.0/nautilus_trader/core/fsm.pyx
+-rw-r--r--   0        0        0      907 2023-05-20 00:56:32.896015 nautilus_trader-1.174.0/nautilus_trader/core/includes/backtest.h
+-rw-r--r--   0        0        0     7908 2023-05-20 00:56:32.896015 nautilus_trader-1.174.0/nautilus_trader/core/includes/common.h
+-rw-r--r--   0        0        0     2997 2023-05-20 00:56:32.896015 nautilus_trader-1.174.0/nautilus_trader/core/includes/core.h
+-rw-r--r--   0        0        0    32646 2023-05-20 00:56:32.896015 nautilus_trader-1.174.0/nautilus_trader/core/includes/model.h
+-rw-r--r--   0        0        0     2325 2023-05-20 00:56:32.896015 nautilus_trader-1.174.0/nautilus_trader/core/inspect.py
+-rw-r--r--   0        0        0     2471 2023-05-20 00:56:32.896015 nautilus_trader-1.174.0/nautilus_trader/core/message.pxd
+-rw-r--r--   0        0        0     6720 2023-05-20 00:56:32.896015 nautilus_trader-1.174.0/nautilus_trader/core/message.pyx
+-rw-r--r--   0        0        0      869 2023-05-20 00:56:32.896015 nautilus_trader-1.174.0/nautilus_trader/core/rust/__init__.pxd
+-rw-r--r--   0        0        0     1050 2023-05-20 00:56:32.896015 nautilus_trader-1.174.0/nautilus_trader/core/rust/backtest.pxd
+-rw-r--r--   0        0        0     7939 2023-05-20 01:01:55.873037 nautilus_trader-1.174.0/nautilus_trader/core/rust/common.pxd
+-rw-r--r--   0        0        0     1222 2023-05-20 00:56:32.896015 nautilus_trader-1.174.0/nautilus_trader/core/rust/common.pyx
+-rw-r--r--   0        0        0     2942 2023-05-20 01:01:32.217266 nautilus_trader-1.174.0/nautilus_trader/core/rust/core.pxd
+-rw-r--r--   0        0        0    31055 2023-05-20 01:01:40.041191 nautilus_trader-1.174.0/nautilus_trader/core/rust/model.pxd
+-rw-r--r--   0        0        0     2689 2023-05-20 00:56:32.896015 nautilus_trader-1.174.0/nautilus_trader/core/rust/model.pyx
+-rw-r--r--   0        0        0     1359 2023-05-20 00:56:32.896015 nautilus_trader-1.174.0/nautilus_trader/core/stats.pxd
+-rw-r--r--   0        0        0     5710 2023-05-20 00:56:32.896015 nautilus_trader-1.174.0/nautilus_trader/core/stats.pyx
+-rw-r--r--   0        0        0     3197 2023-05-20 00:56:32.896015 nautilus_trader-1.174.0/nautilus_trader/core/string.pxd
+-rw-r--r--   0        0        0     1049 2023-05-20 00:56:32.896015 nautilus_trader-1.174.0/nautilus_trader/core/uuid.pxd
+-rw-r--r--   0        0        0     3157 2023-05-20 00:56:32.896015 nautilus_trader-1.174.0/nautilus_trader/core/uuid.pyx
+-rw-r--r--   0        0        0      869 2023-05-20 00:56:32.896015 nautilus_trader-1.174.0/nautilus_trader/data/__init__.pxd
+-rw-r--r--   0        0        0     1360 2023-05-20 00:56:32.896015 nautilus_trader-1.174.0/nautilus_trader/data/__init__.py
+-rw-r--r--   0        0        0     4156 2023-05-20 00:56:32.896015 nautilus_trader-1.174.0/nautilus_trader/data/aggregation.pxd
+-rw-r--r--   0        0        0    24142 2023-05-20 00:56:32.896015 nautilus_trader-1.174.0/nautilus_trader/data/aggregation.pyx
+-rw-r--r--   0        0        0     8386 2023-05-20 00:56:32.896015 nautilus_trader-1.174.0/nautilus_trader/data/client.pxd
+-rw-r--r--   0        0        0    41143 2023-05-20 00:56:32.896015 nautilus_trader-1.174.0/nautilus_trader/data/client.pyx
+-rw-r--r--   0        0        0     9022 2023-05-20 00:56:32.896015 nautilus_trader-1.174.0/nautilus_trader/data/engine.pxd
+-rw-r--r--   0        0        0    55431 2023-05-20 00:56:32.896015 nautilus_trader-1.174.0/nautilus_trader/data/engine.pyx
+-rw-r--r--   0        0        0     2396 2023-05-20 00:56:32.896015 nautilus_trader-1.174.0/nautilus_trader/data/messages.pxd
+-rw-r--r--   0        0        0     8389 2023-05-20 00:56:32.896015 nautilus_trader-1.174.0/nautilus_trader/data/messages.pyx
+-rw-r--r--   0        0        0      869 2023-05-20 00:56:32.896015 nautilus_trader-1.174.0/nautilus_trader/examples/__init__.py
+-rw-r--r--   0        0        0      869 2023-05-20 00:56:32.896015 nautilus_trader-1.174.0/nautilus_trader/examples/algorithms/__init__.py
+-rw-r--r--   0        0        0     4133 2023-05-20 00:56:32.896015 nautilus_trader-1.174.0/nautilus_trader/examples/algorithms/blank.py
+-rw-r--r--   0        0        0    11508 2023-05-20 00:56:32.896015 nautilus_trader-1.174.0/nautilus_trader/examples/algorithms/twap.py
+-rw-r--r--   0        0        0      869 2023-05-20 00:56:32.896015 nautilus_trader-1.174.0/nautilus_trader/examples/strategies/__init__.pxd
+-rw-r--r--   0        0        0      869 2023-05-20 00:56:32.896015 nautilus_trader-1.174.0/nautilus_trader/examples/strategies/__init__.py
+-rw-r--r--   0        0        0     5581 2023-05-20 00:56:32.896015 nautilus_trader-1.174.0/nautilus_trader/examples/strategies/blank.py
+-rw-r--r--   0        0        0    12340 2023-05-20 00:56:32.896015 nautilus_trader-1.174.0/nautilus_trader/examples/strategies/ema_cross.py
+-rw-r--r--   0        0        0    12010 2023-05-20 00:56:32.896015 nautilus_trader-1.174.0/nautilus_trader/examples/strategies/ema_cross_bracket.py
+-rw-r--r--   0        0        0    14927 2023-05-20 00:56:32.896015 nautilus_trader-1.174.0/nautilus_trader/examples/strategies/ema_cross_bracket_algo.py
+-rw-r--r--   0        0        0    10735 2023-05-20 00:56:32.896015 nautilus_trader-1.174.0/nautilus_trader/examples/strategies/ema_cross_cython.pyx
+-rw-r--r--   0        0        0    16017 2023-05-20 00:56:32.896015 nautilus_trader-1.174.0/nautilus_trader/examples/strategies/ema_cross_stop_entry.py
+-rw-r--r--   0        0        0    14424 2023-05-20 00:56:32.896015 nautilus_trader-1.174.0/nautilus_trader/examples/strategies/ema_cross_trailing_stop.py
+-rw-r--r--   0        0        0    12963 2023-05-20 00:56:32.896015 nautilus_trader-1.174.0/nautilus_trader/examples/strategies/ema_cross_twap.py
+-rw-r--r--   0        0        0     5512 2023-05-20 00:56:32.896015 nautilus_trader-1.174.0/nautilus_trader/examples/strategies/market_maker.py
+-rw-r--r--   0        0        0     8241 2023-05-20 00:56:32.896015 nautilus_trader-1.174.0/nautilus_trader/examples/strategies/orderbook_imbalance.py
+-rw-r--r--   0        0        0     2730 2023-05-20 00:56:32.896015 nautilus_trader-1.174.0/nautilus_trader/examples/strategies/signal_strategy.py
+-rw-r--r--   0        0        0     4629 2023-05-20 00:56:32.896015 nautilus_trader-1.174.0/nautilus_trader/examples/strategies/subscribe.py
+-rw-r--r--   0        0        0    13464 2023-05-20 00:56:32.896015 nautilus_trader-1.174.0/nautilus_trader/examples/strategies/volatility_market_maker.py
+-rw-r--r--   0        0        0      869 2023-05-20 00:56:32.896015 nautilus_trader-1.174.0/nautilus_trader/execution/__init__.pxd
+-rw-r--r--   0        0        0     1353 2023-05-20 00:56:32.896015 nautilus_trader-1.174.0/nautilus_trader/execution/__init__.py
+-rw-r--r--   0        0        0     5954 2023-05-20 00:56:32.896015 nautilus_trader-1.174.0/nautilus_trader/execution/algorithm.pxd
+-rw-r--r--   0        0        0    38095 2023-05-20 00:56:32.896015 nautilus_trader-1.174.0/nautilus_trader/execution/algorithm.pyx
+-rw-r--r--   0        0        0     7458 2023-05-20 00:56:32.896015 nautilus_trader-1.174.0/nautilus_trader/execution/client.pxd
+-rw-r--r--   0        0        0    28604 2023-05-20 00:56:32.896015 nautilus_trader-1.174.0/nautilus_trader/execution/client.pyx
+-rw-r--r--   0        0        0     4418 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/execution/emulator.pxd
+-rw-r--r--   0        0        0    39253 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/execution/emulator.pyx
+-rw-r--r--   0        0        0     6030 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/execution/engine.pxd
+-rw-r--r--   0        0        0    33464 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/execution/engine.pyx
+-rw-r--r--   0        0        0     3485 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/execution/matching_core.pxd
+-rw-r--r--   0        0        0    14476 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/execution/matching_core.pyx
+-rw-r--r--   0        0        0     5380 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/execution/messages.pxd
+-rw-r--r--   0        0        0    30396 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/execution/messages.pyx
+-rw-r--r--   0        0        0     8370 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/execution/reports.pxd
+-rw-r--r--   0        0        0    22070 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/execution/reports.pyx
+-rw-r--r--   0        0        0     1785 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/execution/trailing.pxd
+-rw-r--r--   0        0        0    16636 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/execution/trailing.pyx
+-rw-r--r--   0        0        0      869 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/__init__.pxd
+-rw-r--r--   0        0        0     1188 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/__init__.py
+-rw-r--r--   0        0        0     1722 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/amat.pxd
+-rw-r--r--   0        0        0     4836 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/amat.pyx
+-rw-r--r--   0        0        0     1482 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/aroon.pxd
+-rw-r--r--   0        0        0     3474 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/aroon.pyx
+-rw-r--r--   0        0        0     1474 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/atr.pxd
+-rw-r--r--   0        0        0     4324 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/atr.pyx
+-rw-r--r--   0        0        0      869 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/average/__init__.pxd
+-rw-r--r--   0        0        0      869 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/average/__init__.py
+-rw-r--r--   0        0        0     1770 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/average/ama.pxd
+-rw-r--r--   0        0        0     5197 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/average/ama.pyx
+-rw-r--r--   0        0        0     1063 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/average/dema.pxd
+-rw-r--r--   0        0        0     3852 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/average/dema.pyx
+-rw-r--r--   0        0        0     1096 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/average/ema.pxd
+-rw-r--r--   0        0        0     3466 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/average/ema.pyx
+-rw-r--r--   0        0        0     1247 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/average/hma.pxd
+-rw-r--r--   0        0        0     4335 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/average/hma.pyx
+-rw-r--r--   0        0        0     3114 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/average/ma_factory.pyx
+-rw-r--r--   0        0        0     1566 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/average/moving_average.pxd
+-rw-r--r--   0        0        0     2945 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/average/moving_average.pyx
+-rw-r--r--   0        0        0     1080 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/average/rma.pxd
+-rw-r--r--   0        0        0     3478 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/average/rma.pyx
+-rw-r--r--   0        0        0     1020 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/average/sma.pxd
+-rw-r--r--   0        0        0     3542 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/average/sma.pyx
+-rw-r--r--   0        0        0     1283 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/average/vidya.pxd
+-rw-r--r--   0        0        0     4604 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/average/vidya.pyx
+-rw-r--r--   0        0        0     1174 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/average/wma.pxd
+-rw-r--r--   0        0        0     4712 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/average/wma.pyx
+-rw-r--r--   0        0        0      869 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/base/__init__.pxd
+-rw-r--r--   0        0        0      869 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/base/__init__.py
+-rw-r--r--   0        0        0     1715 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/base/indicator.pxd
+-rw-r--r--   0        0        0     2981 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/base/indicator.pyx
+-rw-r--r--   0        0        0     1315 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/bias.pxd
+-rw-r--r--   0        0        0     2872 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/bias.pyx
+-rw-r--r--   0        0        0     1579 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/bollinger_bands.pxd
+-rw-r--r--   0        0        0     5221 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/bollinger_bands.pyx
+-rw-r--r--   0        0        0     1639 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/cci.pxd
+-rw-r--r--   0        0        0     4060 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/cci.pyx
+-rw-r--r--   0        0        0     1375 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/cmo.pxd
+-rw-r--r--   0        0        0     3664 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/cmo.pyx
+-rw-r--r--   0        0        0     1662 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/dm.pxd
+-rw-r--r--   0        0        0     3736 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/dm.pyx
+-rw-r--r--   0        0        0     1490 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/donchian_channel.pxd
+-rw-r--r--   0        0        0     4376 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/donchian_channel.pyx
+-rw-r--r--   0        0        0     1231 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/efficiency_ratio.pxd
+-rw-r--r--   0        0        0     3123 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/efficiency_ratio.pyx
+-rw-r--r--   0        0        0     3172 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/fuzzy_candlesticks.pxd
+-rw-r--r--   0        0        0    12544 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/fuzzy_candlesticks.pyx
+-rw-r--r--   0        0        0     1347 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/fuzzy_enum.pyx
+-rw-r--r--   0        0        0      869 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/fuzzy_enums/__init__.pxd
+-rw-r--r--   0        0        0      869 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/fuzzy_enums/__init__.py
+-rw-r--r--   0        0        0      976 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/fuzzy_enums/candle_body.pxd
+-rw-r--r--   0        0        0      980 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/fuzzy_enums/candle_body.pyx
+-rw-r--r--   0        0        0      947 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/fuzzy_enums/candle_direction.pxd
+-rw-r--r--   0        0        0      987 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/fuzzy_enums/candle_direction.pyx
+-rw-r--r--   0        0        0     1020 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/fuzzy_enums/candle_size.pxd
+-rw-r--r--   0        0        0      972 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/fuzzy_enums/candle_size.pyx
+-rw-r--r--   0        0        0      972 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/fuzzy_enums/candle_wick.pxd
+-rw-r--r--   0        0        0      980 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/fuzzy_enums/candle_wick.pyx
+-rw-r--r--   0        0        0     1809 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/keltner_channel.pxd
+-rw-r--r--   0        0        0     4675 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/keltner_channel.pyx
+-rw-r--r--   0        0        0     1395 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/keltner_position.pxd
+-rw-r--r--   0        0        0     4284 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/keltner_position.pyx
+-rw-r--r--   0        0        0     1713 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/kvo.pxd
+-rw-r--r--   0        0        0     4731 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/kvo.pyx
+-rw-r--r--   0        0        0     1636 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/linear_regression.pxd
+-rw-r--r--   0        0        0     3843 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/linear_regression.pyx
+-rw-r--r--   0        0        0     1662 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/macd.pxd
+-rw-r--r--   0        0        0     4821 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/macd.pyx
+-rw-r--r--   0        0        0     1232 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/obv.pxd
+-rw-r--r--   0        0        0     2962 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/obv.pyx
+-rw-r--r--   0        0        0     1514 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/pressure.pxd
+-rw-r--r--   0        0        0     4387 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/pressure.pyx
+-rw-r--r--   0        0        0     1476 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/psl.pxd
+-rw-r--r--   0        0        0     3315 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/psl.pyx
+-rw-r--r--   0        0        0     1227 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/roc.pxd
+-rw-r--r--   0        0        0     2730 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/roc.pyx
+-rw-r--r--   0        0        0     1393 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/rsi.pxd
+-rw-r--r--   0        0        0     3771 2023-05-20 00:56:32.900015 nautilus_trader-1.174.0/nautilus_trader/indicators/rsi.pyx
+-rw-r--r--   0        0        0     1767 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/indicators/rvi.pxd
+-rw-r--r--   0        0        0     4543 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/indicators/rvi.pyx
+-rw-r--r--   0        0        0     1444 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/indicators/spread_analyzer.pxd
+-rw-r--r--   0        0        0     3384 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/indicators/spread_analyzer.pyx
+-rw-r--r--   0        0        0     1485 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/indicators/stochastics.pxd
+-rw-r--r--   0        0        0     3888 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/indicators/stochastics.pyx
+-rw-r--r--   0        0        0     2275 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/indicators/swings.pxd
+-rw-r--r--   0        0        0     4682 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/indicators/swings.pyx
+-rw-r--r--   0        0        0     1458 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/indicators/vhf.pxd
+-rw-r--r--   0        0        0     3517 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/indicators/vhf.pyx
+-rw-r--r--   0        0        0     1485 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/indicators/volatility_ratio.pxd
+-rw-r--r--   0        0        0     4486 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/indicators/volatility_ratio.pyx
+-rw-r--r--   0        0        0     1270 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/indicators/vwap.pxd
+-rw-r--r--   0        0        0     2942 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/indicators/vwap.pyx
+-rw-r--r--   0        0        0      869 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/infrastructure/__init__.pxd
+-rw-r--r--   0        0        0     1047 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/infrastructure/__init__.py
+-rw-r--r--   0        0        0     1362 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/infrastructure/cache.pxd
+-rw-r--r--   0        0        0    30746 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/infrastructure/cache.pyx
+-rw-r--r--   0        0        0     1155 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/live/__init__.py
+-rw-r--r--   0        0        0     1849 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/live/__main__.py
+-rw-r--r--   0        0        0    30848 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/live/data_client.py
+-rw-r--r--   0        0        0    15072 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/live/data_engine.py
+-rw-r--r--   0        0        0    16682 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/live/execution_client.py
+-rw-r--r--   0        0        0    37117 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/live/execution_engine.py
+-rw-r--r--   0        0        0     3535 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/live/factories.py
+-rw-r--r--   0        0        0    20190 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/live/node.py
+-rw-r--r--   0        0        0     8452 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/live/node_builder.py
+-rw-r--r--   0        0        0     9203 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/live/risk_engine.py
+-rw-r--r--   0        0        0     5560 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/model/__init__.pxd
+-rw-r--r--   0        0        0     1141 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/model/__init__.py
+-rw-r--r--   0        0        0      894 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/model/currencies.pxd
+-rw-r--r--   0        0        0     9220 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/model/currencies.pyx
+-rw-r--r--   0        0        0     1308 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/model/currency.pxd
+-rw-r--r--   0        0        0     8403 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/model/currency.pyx
+-rw-r--r--   0        0        0      869 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/model/data/__init__.pxd
+-rw-r--r--   0        0        0      950 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/model/data/__init__.py
+-rw-r--r--   0        0        0     2541 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/model/data/bar.pxd
+-rw-r--r--   0        0        0    26622 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/model/data/bar.pyx
+-rw-r--r--   0        0        0     1178 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/model/data/bar_aggregation.pxd
+-rw-r--r--   0        0        0      958 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/model/data/bar_aggregation.pyx
+-rw-r--r--   0        0        0     1467 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/model/data/base.pxd
+-rw-r--r--   0        0        0     3443 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/model/data/base.pyx
+-rw-r--r--   0        0        0     1373 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/model/data/bet.pxd
+-rw-r--r--   0        0        0     4166 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/model/data/bet.pyx
+-rw-r--r--   0        0        0     3757 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/model/data/book.pxd
+-rw-r--r--   0        0        0    14710 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/model/data/book.pyx
+-rw-r--r--   0        0        0     3259 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/model/data/tick.pxd
+-rw-r--r--   0        0        0    24747 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/model/data/tick.pyx
+-rw-r--r--   0        0        0     1225 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/model/data/ticker.pxd
+-rw-r--r--   0        0        0     3293 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/model/data/ticker.pyx
+-rw-r--r--   0        0        0     2492 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/model/data/venue.pxd
+-rw-r--r--   0        0        0    10197 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/model/data/venue.pyx
+-rw-r--r--   0        0        0     7484 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/model/enums.pyx
+-rw-r--r--   0        0        0     4918 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/model/enums_c.pxd
+-rw-r--r--   0        0        0    11387 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/model/enums_c.pyx
+-rw-r--r--   0        0        0      869 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/model/events/__init__.pxd
+-rw-r--r--   0        0        0      951 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/model/events/__init__.py
+-rw-r--r--   0        0        0     2058 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/model/events/account.pxd
+-rw-r--r--   0        0        0     5965 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/model/events/account.pyx
+-rw-r--r--   0        0        0     9076 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/model/events/order.pxd
+-rw-r--r--   0        0        0    85735 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/model/events/order.pyx
+-rw-r--r--   0        0        0     5544 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/model/events/position.pxd
+-rw-r--r--   0        0        0    34546 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/model/events/position.pyx
+-rw-r--r--   0        0        0     2983 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/model/identifiers.pxd
+-rw-r--r--   0        0        0    22672 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/model/identifiers.pyx
+-rw-r--r--   0        0        0        0 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/model/instruments/__init__.pxd
+-rw-r--r--   0        0        0     1752 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/model/instruments/__init__.py
+-rw-r--r--   0        0        0     4880 2023-05-20 00:56:32.904015 nautilus_trader-1.174.0/nautilus_trader/model/instruments/base.pxd
+-rw-r--r--   0        0        0    19261 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/instruments/base.pyx
+-rw-r--r--   0        0        0     1745 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/instruments/betting.pxd
+-rw-r--r--   0        0        0     7712 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/instruments/betting.pyx
+-rw-r--r--   0        0        0     1521 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/instruments/crypto_future.pxd
+-rw-r--r--   0        0        0    11042 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/instruments/crypto_future.pyx
+-rw-r--r--   0        0        0     1491 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/instruments/crypto_perpetual.pxd
+-rw-r--r--   0        0        0    11211 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/instruments/crypto_perpetual.pyx
+-rw-r--r--   0        0        0     1265 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/instruments/currency_pair.pxd
+-rw-r--r--   0        0        0    11354 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/instruments/currency_pair.pyx
+-rw-r--r--   0        0        0     1108 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/instruments/equity.pxd
+-rw-r--r--   0        0        0     7319 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/instruments/equity.pyx
+-rw-r--r--   0        0        0     1344 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/instruments/futures_contract.pxd
+-rw-r--r--   0        0        0     6806 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/instruments/futures_contract.pyx
+-rw-r--r--   0        0        0     1386 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/instruments/options_contract.pxd
+-rw-r--r--   0        0        0     7459 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/instruments/options_contract.pyx
+-rw-r--r--   0        0        0     5280 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/objects.pxd
+-rw-r--r--   0        0        0    40812 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/objects.pyx
+-rw-r--r--   0        0        0      869 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/orderbook/__init__.pxd
+-rw-r--r--   0        0        0     1597 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/orderbook/__init__.py
+-rw-r--r--   0        0        0     5048 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/orderbook/book.pxd
+-rw-r--r--   0        0        0    30652 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/orderbook/book.pyx
+-rw-r--r--   0        0        0     1005 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/orderbook/error.py
+-rw-r--r--   0        0        0     2752 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/orderbook/ladder.pxd
+-rw-r--r--   0        0        0     8368 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/orderbook/ladder.pyx
+-rw-r--r--   0        0        0     1357 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/orderbook/level.pxd
+-rw-r--r--   0        0        0     4097 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/orderbook/level.pyx
+-rw-r--r--   0        0        0     1336 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/orderbook/simulated.pxd
+-rw-r--r--   0        0        0     6245 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/orderbook/simulated.pyx
+-rw-r--r--   0        0        0      869 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/orders/__init__.pxd
+-rw-r--r--   0        0        0     2093 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/orders/__init__.py
+-rw-r--r--   0        0        0     8827 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/orders/base.pxd
+-rw-r--r--   0        0        0    33961 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/orders/base.pyx
+-rw-r--r--   0        0        0     1705 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/orders/limit.pxd
+-rw-r--r--   0        0        0    17316 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/orders/limit.pyx
+-rw-r--r--   0        0        0     2171 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/orders/limit_if_touched.pxd
+-rw-r--r--   0        0        0    16477 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/orders/limit_if_touched.pyx
+-rw-r--r--   0        0        0     1849 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/orders/list.pxd
+-rw-r--r--   0        0        0     2367 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/orders/list.pyx
+-rw-r--r--   0        0        0     1206 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/orders/market.pxd
+-rw-r--r--   0        0        0    12902 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/orders/market.pyx
+-rw-r--r--   0        0        0     1608 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/orders/market_if_touched.pxd
+-rw-r--r--   0        0        0    14755 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/orders/market_if_touched.pyx
+-rw-r--r--   0        0        0     1644 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/orders/market_to_limit.pxd
+-rw-r--r--   0        0        0    13592 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/orders/market_to_limit.pyx
+-rw-r--r--   0        0        0     2161 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/orders/stop_limit.pxd
+-rw-r--r--   0        0        0    16617 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/orders/stop_limit.pyx
+-rw-r--r--   0        0        0     1598 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/orders/stop_market.pxd
+-rw-r--r--   0        0        0    15030 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/orders/stop_market.pyx
+-rw-r--r--   0        0        0     2641 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/orders/trailing_stop_limit.pxd
+-rw-r--r--   0        0        0    18630 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/orders/trailing_stop_limit.pyx
+-rw-r--r--   0        0        0     1947 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/orders/trailing_stop_market.pxd
+-rw-r--r--   0        0        0    16279 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/orders/trailing_stop_market.pyx
+-rw-r--r--   0        0        0     1141 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/orders/unpacker.pxd
+-rw-r--r--   0        0        0     3906 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/orders/unpacker.pyx
+-rw-r--r--   0        0        0     6860 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/position.pxd
+-rw-r--r--   0        0        0    23025 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/position.pyx
+-rw-r--r--   0        0        0      869 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/tick_scheme/__init__.pxd
+-rw-r--r--   0        0        0     1311 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/tick_scheme/__init__.py
+-rw-r--r--   0        0        0     1581 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/tick_scheme/base.pxd
+-rw-r--r--   0        0        0     3709 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/tick_scheme/base.pyx
+-rw-r--r--   0        0        0     1147 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/tick_scheme/implementations/__init__.py
+-rw-r--r--   0        0        0     1371 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/tick_scheme/implementations/fixed.pxd
+-rw-r--r--   0        0        0     4052 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/tick_scheme/implementations/fixed.pyx
+-rw-r--r--   0        0        0     1359 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/tick_scheme/implementations/tiered.pxd
+-rw-r--r--   0        0        0     5632 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/model/tick_scheme/implementations/tiered.pyx
+-rw-r--r--   0        0        0      869 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/msgbus/__init__.pxd
+-rw-r--r--   0        0        0      994 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/msgbus/__init__.py
+-rw-r--r--   0        0        0     2718 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/msgbus/bus.pxd
+-rw-r--r--   0        0        0    16946 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/msgbus/bus.pyx
+-rw-r--r--   0        0        0     1181 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/msgbus/subscription.pxd
+-rw-r--r--   0        0        0     3066 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/msgbus/subscription.pyx
+-rw-r--r--   0        0        0      869 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/network/__init__.pxd
+-rw-r--r--   0        0        0     1125 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/network/__init__.py
+-rw-r--r--   0        0        0     1020 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/network/error.py
+-rw-r--r--   0        0        0     1520 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/network/http.pxd
+-rw-r--r--   0        0        0     9912 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/network/http.pyx
+-rw-r--r--   0        0        0     1868 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/network/socket.pxd
+-rw-r--r--   0        0        0     6595 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/network/socket.pyx
+-rw-r--r--   0        0        0     1832 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/network/websocket.pxd
+-rw-r--r--   0        0        0    10808 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/network/websocket.pyx
+-rw-r--r--   0        0        0      972 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/persistence/__init__.py
+-rw-r--r--   0        0        0     1079 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/persistence/catalog/__init__.py
+-rw-r--r--   0        0        0     6131 2023-05-20 00:56:32.908015 nautilus_trader-1.174.0/nautilus_trader/persistence/catalog/base.py
+-rw-r--r--   0        0        0    18579 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/persistence/catalog/parquet.py
+-rw-r--r--   0        0        0      869 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/persistence/external/__init__.py
+-rw-r--r--   0        0        0    14916 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/persistence/external/core.py
+-rw-r--r--   0        0        0     1555 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/persistence/external/metadata.py
+-rw-r--r--   0        0        0    13281 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/persistence/external/readers.py
+-rw-r--r--   0        0        0     3157 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/persistence/external/util.py
+-rw-r--r--   0        0        0     2152 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/persistence/funcs.py
+-rw-r--r--   0        0        0     5280 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/persistence/loaders.py
+-rw-r--r--   0        0        0     1530 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/persistence/migrate.py
+-rw-r--r--   0        0        0      869 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/persistence/streaming/__init__.py
+-rw-r--r--   0        0        0     5330 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/persistence/streaming/batching.py
+-rw-r--r--   0        0        0     8232 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/persistence/streaming/engine.py
+-rw-r--r--   0        0        0     7476 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/persistence/streaming/writer.py
+-rw-r--r--   0        0        0     2564 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/persistence/wranglers.pxd
+-rw-r--r--   0        0        0    17866 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/persistence/wranglers.pyx
+-rw-r--r--   0        0        0      869 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/portfolio/__init__.pxd
+-rw-r--r--   0        0        0      948 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/portfolio/__init__.py
+-rw-r--r--   0        0        0     2132 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/portfolio/base.pxd
+-rw-r--r--   0        0        0     4033 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/portfolio/base.pyx
+-rw-r--r--   0        0        0     3015 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/portfolio/portfolio.pxd
+-rw-r--r--   0        0        0    37488 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/portfolio/portfolio.pyx
+-rw-r--r--   0        0        0      869 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/risk/__init__.pxd
+-rw-r--r--   0        0        0     1084 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/risk/__init__.py
+-rw-r--r--   0        0        0     5613 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/risk/engine.pxd
+-rw-r--r--   0        0        0    36965 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/risk/engine.pyx
+-rw-r--r--   0        0        0     1747 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/risk/sizing.pxd
+-rw-r--r--   0        0        0     7081 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/risk/sizing.pyx
+-rw-r--r--   0        0        0      869 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/serialization/__init__.pxd
+-rw-r--r--   0        0        0     1106 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/serialization/__init__.py
+-rw-r--r--   0        0        0      869 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/serialization/arrow/__init__.pxd
+-rw-r--r--   0        0        0      948 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/serialization/arrow/__init__.py
+-rw-r--r--   0        0        0     1408 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/serialization/arrow/implementations/__init__.py
+-rw-r--r--   0        0        0     4222 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/serialization/arrow/implementations/account_state.py
+-rw-r--r--   0        0        0     1373 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/serialization/arrow/implementations/bar.py
+-rw-r--r--   0        0        0     1090 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/serialization/arrow/implementations/instruments.py
+-rw-r--r--   0        0        0     5194 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/serialization/arrow/implementations/order_book.py
+-rw-r--r--   0        0        0     2947 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/serialization/arrow/implementations/order_events.py
+-rw-r--r--   0        0        0     5420 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/serialization/arrow/implementations/orderbook_v2.py
+-rw-r--r--   0        0        0     2873 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/serialization/arrow/implementations/position_events.py
+-rw-r--r--   0        0        0    29149 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/serialization/arrow/schema.py
+-rw-r--r--   0        0        0     3023 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/serialization/arrow/schema_v2.py
+-rw-r--r--   0        0        0      910 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/serialization/arrow/serializer.pxd
+-rw-r--r--   0        0        0     6290 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/serialization/arrow/serializer.pyx
+-rw-r--r--   0        0        0     4625 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/serialization/arrow/util.py
+-rw-r--r--   0        0        0     1053 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/serialization/base.pxd
+-rw-r--r--   0        0        0    10114 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/serialization/base.pyx
+-rw-r--r--   0        0        0      869 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/serialization/msgpack/__init__.pxd
+-rw-r--r--   0        0        0      869 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/serialization/msgpack/__init__.py
+-rw-r--r--   0        0        0     1097 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/serialization/msgpack/serializer.pxd
+-rw-r--r--   0        0        0     3649 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/serialization/msgpack/serializer.pyx
+-rw-r--r--   0        0        0      869 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/system/__init__.py
+-rw-r--r--   0        0        0    23192 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/system/kernel.py
+-rw-r--r--   0        0        0     1035 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/test_kit/__init__.py
+-rw-r--r--   0        0        0      869 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/test_kit/mocks/__init__.py
+-rw-r--r--   0        0        0     6160 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/test_kit/mocks/actors.py
+-rw-r--r--   0        0        0     5825 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/test_kit/mocks/cache_database.py
+-rw-r--r--   0        0        0     3967 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/test_kit/mocks/data.py
+-rw-r--r--   0        0        0     3077 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/test_kit/mocks/engines.py
+-rw-r--r--   0        0        0    12905 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/test_kit/mocks/exec_clients.py
+-rw-r--r--   0        0        0     6073 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/test_kit/mocks/strategies.py
+-rw-r--r--   0        0        0     3076 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/test_kit/performance.py
+-rw-r--r--   0        0        0    20761 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/test_kit/providers.py
+-rw-r--r--   0        0        0     1276 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/test_kit/stubs/__init__.py
+-rw-r--r--   0        0        0     4385 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/test_kit/stubs/commands.py
+-rw-r--r--   0        0        0     6613 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/test_kit/stubs/component.py
+-rw-r--r--   0        0        0     6251 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/test_kit/stubs/config.py
+-rw-r--r--   0        0        0    17802 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/test_kit/stubs/data.py
+-rw-r--r--   0        0        0    13185 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/test_kit/stubs/events.py
+-rw-r--r--   0        0        0     6704 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/test_kit/stubs/execution.py
+-rw-r--r--   0        0        0     3425 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/test_kit/stubs/identifiers.py
+-rw-r--r--   0        0        0     2970 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/test_kit/stubs/persistence.py
+-rw-r--r--   0        0        0      869 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/trading/__init__.pxd
+-rw-r--r--   0        0        0     1145 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/trading/__init__.py
+-rw-r--r--   0        0        0     2103 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/trading/filters.pxd
+-rw-r--r--   0        0        0    16813 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/trading/filters.pyx
+-rw-r--r--   0        0        0     6774 2023-05-20 00:56:32.912015 nautilus_trader-1.174.0/nautilus_trader/trading/strategy.pxd
+-rw-r--r--   0        0        0    53611 2023-05-20 00:56:32.916015 nautilus_trader-1.174.0/nautilus_trader/trading/strategy.pyx
+-rw-r--r--   0        0        0     3055 2023-05-20 00:56:32.916015 nautilus_trader-1.174.0/nautilus_trader/trading/trader.pxd
+-rw-r--r--   0        0        0    20063 2023-05-20 00:56:32.916015 nautilus_trader-1.174.0/nautilus_trader/trading/trader.pyx
+-rw-r--r--   0        0        0     7477 2023-05-20 00:56:32.916015 nautilus_trader-1.174.0/pyproject.toml
+-rw-r--r--   0        0        0    25793 1970-01-01 00:00:00.000000 nautilus_trader-1.174.0/PKG-INFO
```

### Comparing `nautilus_trader-1.173.0/LICENSE` & `nautilus_trader-1.174.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/README.md` & `nautilus_trader-1.174.0/README.md`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/build.py` & `nautilus_trader-1.174.0/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,19 +22,19 @@
 # The build mode (affects cargo)
 BUILD_MODE = os.getenv("BUILD_MODE", "release")
 # If PROFILE_MODE mode is enabled, include traces necessary for coverage and profiling
 PROFILE_MODE = bool(os.getenv("PROFILE_MODE", ""))
 # If ANNOTATION mode is enabled, generate an annotated HTML version of the input source files
 ANNOTATION_MODE = bool(os.getenv("ANNOTATION_MODE", ""))
 # If PARALLEL build is enabled, uses all CPUs for compile stage of build
-PARALLEL_BUILD = True if os.getenv("PARALLEL_BUILD", "true") == "true" else False
+PARALLEL_BUILD = os.getenv("PARALLEL_BUILD", "true") == "true"
 # If COPY_TO_SOURCE is enabled, copy built *.so files back into the source tree
-COPY_TO_SOURCE = True if os.getenv("COPY_TO_SOURCE", "true") == "true" else False
+COPY_TO_SOURCE = os.getenv("COPY_TO_SOURCE", "true") == "true"
 # If PyO3 only then don't build C extensions to reduce compilation time
-PYO3_ONLY = False if os.getenv("PYO3_ONLY", "") == "" else True
+PYO3_ONLY = os.getenv("PYO3_ONLY", "") != ""
 
 if PROFILE_MODE:
     # For subsequent debugging, the C source needs to be in the same tree as
     # the Cython code (not in a separate build directory).
     BUILD_DIR = None
 elif ANNOTATION_MODE:
     BUILD_DIR = "build/annotated"
@@ -185,25 +185,25 @@
 def _build_distribution(extensions: list[Extension]) -> Distribution:
     nthreads = os.cpu_count() or 1
     if platform.system() == "Windows":
         nthreads = min(nthreads, 60)
     print(f"nthreads={nthreads}")
 
     distribution = Distribution(
-        dict(
-            name="nautilus_trader",
-            ext_modules=cythonize(
+        {
+            "name": "nautilus_trader",
+            "ext_modules": cythonize(
                 module_list=extensions,
                 compiler_directives=CYTHON_COMPILER_DIRECTIVES,
                 nthreads=nthreads,
                 build_dir=BUILD_DIR,
                 gdb_debug=PROFILE_MODE,
             ),
-            zip_safe=False,
-        ),
+            "zip_safe": False,
+        },
     )
     return distribution
 
 
 def _copy_build_dir_to_project(cmd: build_ext) -> None:
     # Copy built extensions back to the project tree
     for output in cmd.get_outputs():
@@ -276,15 +276,15 @@
             if platform.system() == "Linux":
                 strip_cmd = f"strip --strip-unneeded {so}"
             elif platform.system() == "Darwin":
                 strip_cmd = f"strip -x {so}"
             else:
                 raise RuntimeError(f"Cannot strip symbols for platform {platform.system()}")
             subprocess.run(
-                strip_cmd,  # noqa
+                strip_cmd,
                 check=True,
                 shell=True,  # noqa
                 capture_output=True,
             )
     except subprocess.CalledProcessError as e:
         raise RuntimeError(f"Error when stripping symbols.\n{e.stderr.decode()}") from e
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/.cargo/config.toml` & `nautilus_trader-1.174.0/nautilus_core/.cargo/config.toml`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_core/Cargo.lock` & `nautilus_trader-1.174.0/nautilus_core/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -75,17 +75,17 @@
 name = "arrayvec"
 version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8da52d66c7071e2e3fa2a1e5c6d088fec47b593032b254f5e980de8ea54454d6"
 
 [[package]]
 name = "arrow"
-version = "37.0.0"
+version = "38.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1aea9fcb25bbb70f7f922f95b99ca29c1013dab47f6df61a6f24861842dd7f2e"
+checksum = "c107a57b5913d852da9d5a40e280e4695f2258b5b87733c13b770c63a7117287"
 dependencies = [
  "ahash 0.8.3",
  "arrow-arith",
  "arrow-array",
  "arrow-buffer",
  "arrow-cast",
  "arrow-csv",
@@ -97,76 +97,76 @@
  "arrow-schema",
  "arrow-select",
  "arrow-string",
 ]
 
 [[package]]
 name = "arrow-arith"
-version = "37.0.0"
+version = "38.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8d967b42f7b12c91fd78acd396b20c2973b184c8866846674abbb00c963e93ab"
+checksum = "ace6aa3d5617c5d03041a05e01c6819428a8ddf49dd0b055df9b40fef9d96094"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "chrono",
  "half 2.2.1",
  "num",
 ]
 
 [[package]]
 name = "arrow-array"
-version = "37.0.0"
+version = "38.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3190f208ee7aa0f3596fa0098d42911dec5e123ca88c002a08b24877ad14c71e"
+checksum = "104a04520692cc674e6afd7682f213ca41f9b13ff1873f63a5a2857a590b87b3"
 dependencies = [
  "ahash 0.8.3",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "chrono",
  "chrono-tz",
  "half 2.2.1",
  "hashbrown 0.13.2",
  "num",
 ]
 
 [[package]]
 name = "arrow-buffer"
-version = "37.0.0"
+version = "38.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5d33c733c5b6c44a0fc526f29c09546e04eb56772a7a21e48e602f368be381f6"
+checksum = "72c875bcb9530ec403998fb0b2dc6d180a7c64563ca4bc22b90eafb84b113143"
 dependencies = [
  "half 2.2.1",
  "num",
 ]
 
 [[package]]
 name = "arrow-cast"
-version = "37.0.0"
+version = "38.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "abd349520b6a1ed4924ae2afc9d23330a3044319e4ec3d5b124c09e4d440ae87"
+checksum = "d6d6e18281636c8fc0b93be59834da6bf9a72bb70fd0c98ddfdaf124da466c28"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "arrow-select",
  "chrono",
  "comfy-table",
  "lexical-core",
  "num",
 ]
 
 [[package]]
 name = "arrow-csv"
-version = "37.0.0"
+version = "38.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c80af3c3e290a2a7e1cc518f1471dff331878cb4af9a5b088bf030b89debf649"
+checksum = "3197dab0963a236ff8e7c82e2272535745955ac1321eb740c29f2f88b353f54e"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-cast",
  "arrow-data",
  "arrow-schema",
  "chrono",
@@ -175,43 +175,43 @@
  "lazy_static",
  "lexical-core",
  "regex",
 ]
 
 [[package]]
 name = "arrow-data"
-version = "37.0.0"
+version = "38.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1c8361947aaa96d331da9df3f7a08bdd8ab805a449994c97f5c4d24c4b7e2cf"
+checksum = "eb68113d6ecdbe8bba48b2c4042c151bf9e1c61244e45072a50250a6fc59bafe"
 dependencies = [
  "arrow-buffer",
  "arrow-schema",
  "half 2.2.1",
  "num",
 ]
 
 [[package]]
 name = "arrow-ipc"
-version = "37.0.0"
+version = "38.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a46ee000b9fbd1e8db6e8b26acb8c760838512b39d8c9f9d73892cb55351d50"
+checksum = "eab4bbf2dd3078facb5ce0a9641316a64f42bfd8cf357e6775c8a5e6708e3a8d"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-cast",
  "arrow-data",
  "arrow-schema",
  "flatbuffers",
 ]
 
 [[package]]
 name = "arrow-json"
-version = "37.0.0"
+version = "38.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4bf2366607be867ced681ad7f272371a5cf1fc2941328eef7b4fee14565166fb"
+checksum = "48c5b650d23746a494665d914a7fa3d21d939153cff9d53bdebe39bffa88f263"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-cast",
  "arrow-data",
  "arrow-schema",
  "chrono",
@@ -221,66 +221,66 @@
  "num",
  "serde",
  "serde_json",
 ]
 
 [[package]]
 name = "arrow-ord"
-version = "37.0.0"
+version = "38.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "304069901c867200e21ec868ae7521165875470ef2f1f6d58f979a443d63997e"
+checksum = "68c6fce28e5011e30acc7466b5efcb8ed0197c396240bd2b10e167f275a3c208"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "arrow-select",
  "half 2.2.1",
  "num",
 ]
 
 [[package]]
 name = "arrow-row"
-version = "37.0.0"
+version = "38.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0d57fe8ceef3392fdd493269d8a2d589de17bafce151aacbffbddac7a57f441a"
+checksum = "f20a421f19799d8b93eb8edde5217e910fa1e2d6ceb3c529f000e57b6db144c0"
 dependencies = [
  "ahash 0.8.3",
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "half 2.2.1",
  "hashbrown 0.13.2",
 ]
 
 [[package]]
 name = "arrow-schema"
-version = "37.0.0"
+version = "38.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a16b88a93ac8350f0200b1cd336a1f887315925b8dd7aa145a37b8bdbd8497a4"
+checksum = "bc85923d8d6662cc66ac6602c7d1876872e671002d60993dfdf492a6badeae92"
 
 [[package]]
 name = "arrow-select"
-version = "37.0.0"
+version = "38.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "98e8a4d6ca37d5212439b24caad4d80743fcbb706706200dd174bb98e68fe9d8"
+checksum = "f6ab6613ce65b61d85a3410241744e84e48fbab0fe06e1251b4429d21b3470fd"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "num",
 ]
 
 [[package]]
 name = "arrow-string"
-version = "37.0.0"
+version = "38.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cbb594efa397eb6a546f42b1f8df3d242ea84dbfda5232e06035dc2b2e2c8459"
+checksum = "f3008641239e884aefba66d8b8532da6af40d14296349fcc85935de4ba67b89e"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "arrow-select",
  "regex",
@@ -309,15 +309,15 @@
 name = "async-trait"
 version = "0.1.68"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b9ccdd8f2a161be9bd5c023df56f1b2a0bd1d83872ae53b71a84a12c9bf6e842"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.16",
 ]
 
 [[package]]
 name = "atty"
 version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d9b39be18770d11421cdb1b9947a45dd3f37e93092cbf377614828a319d5fee8"
@@ -351,14 +351,26 @@
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
+name = "bitvec"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1bc2832c24239b0141d5674bb9174f9d68a8b5b3f2753311927c172ca46f7e9c"
+dependencies = [
+ "funty",
+ "radium",
+ "tap",
+ "wyz",
+]
+
+[[package]]
 name = "borsh"
 version = "0.10.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4114279215a005bc675e386011e594e1d9b800918cea18fcadadcce864a2046b"
 dependencies = [
  "borsh-derive",
  "hashbrown 0.13.2",
@@ -418,34 +430,34 @@
 dependencies = [
  "alloc-no-stdlib",
  "alloc-stdlib",
 ]
 
 [[package]]
 name = "bumpalo"
-version = "3.12.1"
+version = "3.12.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9b1ce199063694f33ffb7dd4e0ee620741495c32833cde5aa08f02a0bf96f0c8"
+checksum = "3c6ed94e98ecff0c12dd1b04c15ec0d7d9458ca8fe806cea6f12954efe74c63b"
 
 [[package]]
 name = "bytecheck"
-version = "0.6.10"
+version = "0.6.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "13fe11640a23eb24562225322cd3e452b93a3d4091d62fab69c70542fcd17d1f"
+checksum = "8b6372023ac861f6e6dc89c8344a8f398fb42aaba2b5dbc649ca0c0e9dbcb627"
 dependencies = [
  "bytecheck_derive",
  "ptr_meta",
  "simdutf8",
 ]
 
 [[package]]
 name = "bytecheck_derive"
-version = "0.6.10"
+version = "0.6.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e31225543cb46f81a7e224762764f4a6a0f097b1db0b175f69e8065efaa42de5"
+checksum = "a7ec4c6f261935ad534c0c22dbef2201b45918860eb1c574b972bd213a76af61"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
@@ -556,34 +568,34 @@
  "parse-zoneinfo",
  "phf",
  "phf_codegen",
 ]
 
 [[package]]
 name = "ciborium"
-version = "0.2.0"
+version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b0c137568cc60b904a7724001b35ce2630fd00d5d84805fbb608ab89509d788f"
+checksum = "effd91f6c78e5a4ace8a5d3c0b6bfaec9e2baaef55f3efc00e45fb2e477ee926"
 dependencies = [
  "ciborium-io",
  "ciborium-ll",
  "serde",
 ]
 
 [[package]]
 name = "ciborium-io"
-version = "0.2.0"
+version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "346de753af073cc87b52b2083a506b38ac176a44cfb05497b622e27be899b369"
+checksum = "cdf919175532b369853f5d5e20b26b43112613fd6fe7aee757e35f7a44642656"
 
 [[package]]
 name = "ciborium-ll"
-version = "0.2.0"
+version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "213030a2b5a4e0c0892b6652260cf6ccac84827b83a85a534e178e3906c4cf1b"
+checksum = "defaa24ecc093c77630e6c15e17c51f5e187bf35ee514f4e2d67baaa96dae22b"
 dependencies = [
  "ciborium-io",
  "half 1.8.2",
 ]
 
 [[package]]
 name = "clap"
@@ -606,24 +618,14 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2850f2f5a82cbf437dd5af4d49848fbdfc27c157c3d010345776f952765261c5"
 dependencies = [
  "os_str_bytes",
 ]
 
 [[package]]
-name = "codespan-reporting"
-version = "0.11.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3538270d33cc669650c4b093848450d380def10c331d38c768e34cac80576e6e"
-dependencies = [
- "termcolor",
- "unicode-width",
-]
-
-[[package]]
 name = "comfy-table"
 version = "6.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6e7b787b0dc42e8111badfdbe4c3059158ccb2db8780352fa1b01e8ccf45cc4d"
 dependencies = [
  "strum",
  "strum_macros",
@@ -655,14 +657,24 @@
  "getrandom",
  "once_cell",
  "proc-macro-hack",
  "tiny-keccak",
 ]
 
 [[package]]
+name = "core-foundation"
+version = "0.9.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "194a7a9e6de53fa55116934067c844d9d749312f75c6f6d0980e8c252f8c2146"
+dependencies = [
+ "core-foundation-sys",
+ "libc",
+]
+
+[[package]]
 name = "core-foundation-sys"
 version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
 
 [[package]]
 name = "crc32fast"
@@ -776,58 +788,14 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b2466559f260f48ad25fe6317b3c8dac77b5bdb5763ac7d9d6103530663bc90"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
-name = "cxx"
-version = "1.0.94"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f61f1b6389c3fe1c316bf8a4dccc90a38208354b330925bce1f74a6c4756eb93"
-dependencies = [
- "cc",
- "cxxbridge-flags",
- "cxxbridge-macro",
- "link-cplusplus",
-]
-
-[[package]]
-name = "cxx-build"
-version = "1.0.94"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "12cee708e8962df2aeb38f594aae5d827c022b6460ac71a7a3e2c3c2aae5a07b"
-dependencies = [
- "cc",
- "codespan-reporting",
- "once_cell",
- "proc-macro2",
- "quote",
- "scratch",
- "syn 2.0.15",
-]
-
-[[package]]
-name = "cxxbridge-flags"
-version = "1.0.94"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7944172ae7e4068c533afbb984114a56c46e9ccddda550499caa222902c7f7bb"
-
-[[package]]
-name = "cxxbridge-macro"
-version = "1.0.94"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2345488264226bf682893e25de0769f3360aac9957980ec49361b083ddaa5bc5"
-dependencies = [
- "proc-macro2",
- "quote",
- "syn 2.0.15",
-]
-
-[[package]]
 name = "darling"
 version = "0.14.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7b750cb3417fd1b327431a470f388520309479ab0bf5e323505daf0290cd3850"
 dependencies = [
  "darling_core",
  "darling_macro",
@@ -869,17 +837,17 @@
  "lock_api",
  "once_cell",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "datafusion"
-version = "23.0.0"
+version = "24.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a8a7d4b334f4512ff2fdbce87f511f570ae895af1ac7c729e77c12583253b22a"
+checksum = "0404a559d5a6d8320369bb0a290b43bbc4f8622d0ef6f04bd095ace9a663f439"
 dependencies = [
  "ahash 0.8.3",
  "arrow",
  "arrow-array",
  "arrow-schema",
  "async-compression",
  "async-trait",
@@ -919,32 +887,32 @@
  "uuid",
  "xz2",
  "zstd 0.12.3+zstd.1.5.2",
 ]
 
 [[package]]
 name = "datafusion-common"
-version = "23.0.0"
+version = "24.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "80abfcb1dbc6390f952f21de9069e6177ad6318fcae5fbceabb50666d96533dd"
+checksum = "4653b79a55161852973760db69ea6dcd05c9966a1b588fd83028f625536a1d7f"
 dependencies = [
  "arrow",
  "arrow-array",
  "chrono",
  "num_cpus",
  "object_store",
  "parquet",
  "sqlparser",
 ]
 
 [[package]]
 name = "datafusion-execution"
-version = "23.0.0"
+version = "24.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "df2524f1b4b58319895b112809d2a59e54fa662d0e46330a455f22882c2cb7b9"
+checksum = "53481c334b73c6759697919d1d05690392381145fa1890849a65b5a71a24a1ec"
 dependencies = [
  "dashmap",
  "datafusion-common",
  "datafusion-expr",
  "hashbrown 0.13.2",
  "log",
  "object_store",
@@ -952,47 +920,47 @@
  "rand",
  "tempfile",
  "url",
 ]
 
 [[package]]
 name = "datafusion-expr"
-version = "23.0.0"
+version = "24.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "af8040b7a75b04685f4db0a1b11ffa93cd163c1bc13751df3f5cf76baabaf5a1"
+checksum = "a8ecd7c6605d0b4269346d03289e2ced1715a303e75e6d313dba0bafb1f823f2"
 dependencies = [
  "ahash 0.8.3",
  "arrow",
  "datafusion-common",
  "sqlparser",
 ]
 
 [[package]]
 name = "datafusion-optimizer"
-version = "23.0.0"
+version = "24.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "74ceae25accc0f640a4238283f55f3a9fd181d55398703a4330fb2c46261e6a2"
+checksum = "70a7c04e94cb4aa9c323993856e18b91f690dda0358a34ab07a3fe0f14bc6600"
 dependencies = [
  "arrow",
  "async-trait",
  "chrono",
  "datafusion-common",
  "datafusion-expr",
  "datafusion-physical-expr",
  "hashbrown 0.13.2",
  "itertools",
  "log",
- "regex-syntax 0.6.29",
+ "regex-syntax 0.7.1",
 ]
 
 [[package]]
 name = "datafusion-physical-expr"
-version = "23.0.0"
+version = "24.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "df4cf228b312f2758cb78e93fe3d2dc602345028efdf7cfa5b338cb370d0a347"
+checksum = "9e34eb8668fee1443965fff41ba73b2956d50a07ed8dd929cfa2e839ab91da5a"
 dependencies = [
  "ahash 0.8.3",
  "arrow",
  "arrow-array",
  "arrow-buffer",
  "arrow-schema",
  "chrono",
@@ -1011,29 +979,29 @@
  "regex",
  "unicode-segmentation",
  "uuid",
 ]
 
 [[package]]
 name = "datafusion-row"
-version = "23.0.0"
+version = "24.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b52b486fb3d81bb132e400304be01af5aba0ad6737e3518045bb98944991fe32"
+checksum = "efa800ae88dfd62ea6c58c24a1154d92937c755672f522b84e8ea6539fad369b"
 dependencies = [
  "arrow",
  "datafusion-common",
  "paste",
  "rand",
 ]
 
 [[package]]
 name = "datafusion-sql"
-version = "23.0.0"
+version = "24.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "773e985c182e41cfd68f7a7b483ab6bfb68beaac241c348cd4b1bf9f9d61b762"
+checksum = "556642ef90073e39af721362353ccce4e1f418da7a8e31c23510ed9de6eb71f2"
 dependencies = [
  "arrow",
  "arrow-schema",
  "datafusion-common",
  "datafusion-expr",
  "log",
  "sqlparser",
@@ -1141,23 +1109,44 @@
 [[package]]
 name = "fnv"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
 
 [[package]]
+name = "foreign-types"
+version = "0.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f6f339eb8adc052cd2ca78910fda869aefa38d22d5cb648e6485e4d3fc06f3b1"
+dependencies = [
+ "foreign-types-shared",
+]
+
+[[package]]
+name = "foreign-types-shared"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "00b0228411908ca8685dba7fc2cdd70ec9990a6e753e89b6ac91a84c40fbaf4b"
+
+[[package]]
 name = "form_urlencoded"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a9c384f161156f5260c24a097c56119f9be8c798586aecc13afbcbe7b7e26bf8"
 dependencies = [
  "percent-encoding",
 ]
 
 [[package]]
+name = "funty"
+version = "2.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e6d5a32815ae3f33302d95fdcb2ce17862f8c65363dcfd29360480ba1001fc9c"
+
+[[package]]
 name = "futures"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "23342abe12aba583913b2e62f22225ff9c950774065e4bfb61a19cd9770fec40"
 dependencies = [
  "futures-channel",
  "futures-core",
@@ -1205,15 +1194,15 @@
 name = "futures-macro"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "89ca545a94061b6365f2c7355b4b32bd20df3ff95f02da9329b34ccc3bd6ee72"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.16",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f43be4fe21a13b9781a69afa4985b0f6ee0e1afab2c6f454a8cf30e2b2237b6e"
@@ -1375,21 +1364,35 @@
  "futures-util",
  "http",
  "http-body",
  "httparse",
  "httpdate",
  "itoa",
  "pin-project-lite",
+ "socket2",
  "tokio",
  "tower-service",
  "tracing",
  "want",
 ]
 
 [[package]]
+name = "hyper-tls"
+version = "0.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d6183ddfa99b85da61a140bea0efc93fdf56ceaa041b37d553518030827f9905"
+dependencies = [
+ "bytes",
+ "hyper",
+ "native-tls",
+ "tokio",
+ "tokio-native-tls",
+]
+
+[[package]]
 name = "iai"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "71a816c97c42258aa5834d07590b718b4c9a598944cd39a52dc25b351185d678"
 
 [[package]]
 name = "iana-time-zone"
@@ -1403,20 +1406,19 @@
  "js-sys",
  "wasm-bindgen",
  "windows",
 ]
 
 [[package]]
 name = "iana-time-zone-haiku"
-version = "0.1.1"
+version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0703ae284fc167426161c2e3f1da3ea71d94b21bedbcc9494e92b28e334e3dca"
+checksum = "f31827a206f56af32e590ba56d5d2d085f558508192593743f16b2306495269f"
 dependencies = [
- "cxx",
- "cxx-build",
+ "cc",
 ]
 
 [[package]]
 name = "ident_case"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b9e0384b61958566e926dc50660321d12159025e767c18e043daf26b70104c39"
@@ -1495,17 +1497,17 @@
 checksum = "936cfd212a0155903bcbc060e316fb6cc7cbf2e1907329391ebadc1fe0ce77c2"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "js-sys"
-version = "0.3.61"
+version = "0.3.63"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "445dde2150c55e483f3d8416706b97ec8e8237c307e5b7b4b8dd15e6af2a0730"
+checksum = "2f37a4a5928311ac501dee68b3c7613a1037d0edb30c8e5427bd832d55d1b790"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "lazy_static"
 version = "1.4.0"
@@ -1574,32 +1576,23 @@
 dependencies = [
  "lexical-util",
  "static_assertions",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.142"
+version = "0.2.144"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6a987beff54b60ffa6d51982e1aa1146bc42f19bd26be28b0586f252fccf5317"
+checksum = "2b00cc1c228a6782d0f076e7b232802e0c5689d41bb5df366f2a6b6621cfdfe1"
 
 [[package]]
 name = "libm"
-version = "0.2.6"
+version = "0.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "348108ab3fba42ec82ff6e9564fc4ca0247bdccdc68dd8af9764bbc79c3c8ffb"
-
-[[package]]
-name = "link-cplusplus"
-version = "1.0.8"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ecd207c9c713c34f95a097a5b029ac2ce6010530c7b49d7fea24d977dede04f5"
-dependencies = [
- "cc",
-]
+checksum = "f7012b1bbb0719e1097c47611d3898568c546d597c2e74d66f6087edd5233ff4"
 
 [[package]]
 name = "linux-raw-sys"
 version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ece97ea872ece730aed82664c424eb4c8291e1ff2480247ccf7409044bc6479f"
 
@@ -1686,115 +1679,136 @@
  "libc",
  "log",
  "wasi 0.11.0+wasi-snapshot-preview1",
  "windows-sys 0.45.0",
 ]
 
 [[package]]
+name = "native-tls"
+version = "0.2.11"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "07226173c32f2926027b63cce4bcd8076c3552846cbe7925f3aaffeac0a3b92e"
+dependencies = [
+ "lazy_static",
+ "libc",
+ "log",
+ "openssl",
+ "openssl-probe",
+ "openssl-sys",
+ "schannel",
+ "security-framework",
+ "security-framework-sys",
+ "tempfile",
+]
+
+[[package]]
 name = "nautilus_backtest"
-version = "0.4.0"
+version = "0.5.0"
 dependencies = [
  "cbindgen",
  "nautilus_common",
  "nautilus_core",
  "nautilus_model",
  "pyo3",
  "tempfile",
 ]
 
 [[package]]
 name = "nautilus_common"
-version = "0.4.0"
+version = "0.5.0"
 dependencies = [
  "cbindgen",
  "chrono",
  "nautilus_core",
  "nautilus_model",
  "pyo3",
  "serde",
  "serde_json",
  "strum",
  "tempfile",
 ]
 
 [[package]]
 name = "nautilus_core"
-version = "0.4.0"
+version = "0.5.0"
 dependencies = [
  "cbindgen",
  "chrono",
  "criterion",
  "iai",
  "pyo3",
  "rstest",
  "serde_json",
  "uuid",
 ]
 
 [[package]]
 name = "nautilus_indicators"
-version = "0.4.0"
+version = "0.5.0"
 dependencies = [
  "nautilus_core",
  "nautilus_model",
  "pyo3",
 ]
 
 [[package]]
 name = "nautilus_model"
-version = "0.4.0"
+version = "0.5.0"
 dependencies = [
  "cbindgen",
  "criterion",
  "derive_builder",
  "iai",
  "lazy_static",
  "nautilus_core",
  "pyo3",
  "rstest",
- "rust-fsm",
  "rust_decimal",
  "strum",
  "thiserror",
 ]
 
 [[package]]
 name = "nautilus_network"
-version = "0.4.0"
+version = "0.5.0"
 dependencies = [
  "hyper",
+ "hyper-tls",
  "nautilus_core",
  "pyo3",
  "pyo3-asyncio",
+ "serde_json",
  "tokio",
 ]
 
 [[package]]
 name = "nautilus_persistence"
-version = "0.4.0"
+version = "0.5.0"
 dependencies = [
  "binary-heap-plus",
  "compare",
+ "criterion",
  "datafusion",
  "futures",
  "nautilus_core",
  "nautilus_model",
  "pin-project-lite",
  "pyo3",
  "pyo3-asyncio",
  "rand",
  "tokio",
 ]
 
 [[package]]
 name = "nautilus_pyo3"
-version = "0.4.0"
+version = "0.5.0"
 dependencies = [
  "nautilus_indicators",
  "nautilus_model",
+ "nautilus_network",
  "nautilus_persistence",
  "pyo3",
 ]
 
 [[package]]
 name = "num"
 version = "0.4.0"
@@ -1911,14 +1925,58 @@
 [[package]]
 name = "oorandom"
 version = "11.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ab1bc2a289d34bd04a330323ac98a1b4bc82c9d9fcb1e66b63caa84da26b575"
 
 [[package]]
+name = "openssl"
+version = "0.10.52"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "01b8574602df80f7b85fdfc5392fa884a4e3b3f4f35402c070ab34c3d3f78d56"
+dependencies = [
+ "bitflags",
+ "cfg-if",
+ "foreign-types",
+ "libc",
+ "once_cell",
+ "openssl-macros",
+ "openssl-sys",
+]
+
+[[package]]
+name = "openssl-macros"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a948666b637a0f465e8564c73e89d4dde00d72d4d473cc972f390fc3dcee7d9c"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.16",
+]
+
+[[package]]
+name = "openssl-probe"
+version = "0.1.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ff011a302c396a5197692431fc1948019154afc178baf7d8e37367442a4601cf"
+
+[[package]]
+name = "openssl-sys"
+version = "0.9.87"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8e17f59264b2809d77ae94f0e1ebabc434773f370d6ca667bd223ea10e06cc7e"
+dependencies = [
+ "cc",
+ "libc",
+ "pkg-config",
+ "vcpkg",
+]
+
+[[package]]
 name = "ordered-float"
 version = "2.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7940cf2ca942593318d07fcf2596cdca60a85c9e7fab408a5e21a4f9dcd40d87"
 dependencies = [
  "num-traits",
 ]
@@ -1950,17 +2008,17 @@
  "redox_syscall 0.2.16",
  "smallvec",
  "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "parquet"
-version = "37.0.0"
+version = "38.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b5022d98333271f4ca3e87bab760498e61726bf5a6ca919123c80517e20ded29"
+checksum = "4cbd51311f8d9ff3d2697b1522b18a588782e097d313a1a278b0faf2ccf2d3f6"
 dependencies = [
  "ahash 0.8.3",
  "arrow-array",
  "arrow-buffer",
  "arrow-cast",
  "arrow-data",
  "arrow-ipc",
@@ -1972,14 +2030,15 @@
  "chrono",
  "flate2",
  "futures",
  "hashbrown 0.13.2",
  "lz4",
  "num",
  "num-bigint",
+ "object_store",
  "paste",
  "seq-macro",
  "snap",
  "thrift",
  "tokio",
  "twox-hash",
  "zstd 0.12.3+zstd.1.5.2",
@@ -2119,17 +2178,17 @@
 name = "proc-macro-hack"
 version = "0.5.20+deprecated"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc375e1527247fe1a97d8b7156678dfe7c1af2fc075c9a4db3690ecd2a148068"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.56"
+version = "1.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
+checksum = "fa1fb82fc0c281dd9671101b66b771ebbe1eaf967b96ac8740dcba4b70005ca8"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "ptr_meta"
 version = "0.1.4"
@@ -2233,22 +2292,28 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.26"
+version = "1.0.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4424af4bf778aae2051a77b60283332f386554255d722233d09fbfc7e30da2fc"
+checksum = "8f4f29d145265ec1c483c7c654450edde0bfe043d3938d6972630663356d9500"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
+name = "radium"
+version = "0.7.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "dc33ff2d4973d518d823d61aa239014831e521c75da58e3df4840d3f47749d09"
+
+[[package]]
 name = "rand"
 version = "0.8.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "34af8d1a0e25924bc5b7c43c079c942339d8f0a8b57c39049bef581b46327404"
 dependencies = [
  "libc",
  "rand_chacha",
@@ -2344,31 +2409,34 @@
 checksum = "581008d2099240d37fb08d77ad713bcaec2c4d89d50b5b21a8bb1996bbab68ab"
 dependencies = [
  "bytecheck",
 ]
 
 [[package]]
 name = "rkyv"
-version = "0.7.41"
+version = "0.7.42"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "21499ed91807f07ae081880aabb2ccc0235e9d88011867d984525e9a4c3cfa3e"
+checksum = "0200c8230b013893c0b2d6213d6ec64ed2b9be2e0e016682b7224ff82cff5c58"
 dependencies = [
+ "bitvec",
  "bytecheck",
  "hashbrown 0.12.3",
  "ptr_meta",
  "rend",
  "rkyv_derive",
  "seahash",
+ "tinyvec",
+ "uuid",
 ]
 
 [[package]]
 name = "rkyv_derive"
-version = "0.7.41"
+version = "0.7.42"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ac1c672430eb41556291981f45ca900a0239ad007242d1cb4b4167af842db666"
+checksum = "b2e06b915b5c230a17d7a736d1e2e63ee753c256a8614ef3f5147b13a4f5541d"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
@@ -2394,33 +2462,14 @@
  "quote",
  "rustc_version",
  "syn 1.0.109",
  "unicode-ident",
 ]
 
 [[package]]
-name = "rust-fsm"
-version = "0.6.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "021d7de715253e45ad24a2fbb0725a0f7f271fd8d3163b130bd65ce2816a860d"
-dependencies = [
- "rust-fsm-dsl",
-]
-
-[[package]]
-name = "rust-fsm-dsl"
-version = "0.6.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a66b1273014079e4cf2b04aad1f3a2849e26e9a106f0411be2b1c15c23a791a"
-dependencies = [
- "quote",
- "syn 1.0.109",
-]
-
-[[package]]
 name = "rust_decimal"
 version = "1.29.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "26bd36b60561ee1fb5ec2817f198b6fd09fa571c897a5e86d1487cfc2b096dfc"
 dependencies = [
  "arrayvec",
  "borsh",
@@ -2475,61 +2524,87 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "93fc1dc3aaa9bfed95e02e6eadabb4baf7e3078b0bd1b4d7b6b0b68378900502"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
-name = "scopeguard"
-version = "1.1.0"
+name = "schannel"
+version = "0.1.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
+checksum = "713cfb06c7059f3588fb8044c0fad1d09e3c01d225e25b9220dbfdcf16dbb1b3"
+dependencies = [
+ "windows-sys 0.42.0",
+]
 
 [[package]]
-name = "scratch"
-version = "1.0.5"
+name = "scopeguard"
+version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1792db035ce95be60c3f8853017b3999209281c24e2ba5bc8e59bf97a0c590c1"
+checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "seahash"
 version = "4.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1c107b6f4780854c8b126e228ea8869f4d7b71260f962fefb57b996b8959ba6b"
 
 [[package]]
+name = "security-framework"
+version = "2.9.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1fc758eb7bffce5b308734e9b0c1468893cae9ff70ebf13e7090be8dcbcc83a8"
+dependencies = [
+ "bitflags",
+ "core-foundation",
+ "core-foundation-sys",
+ "libc",
+ "security-framework-sys",
+]
+
+[[package]]
+name = "security-framework-sys"
+version = "2.9.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f51d0c0d83bec45f16480d0ce0058397a69e48fcdc52d1dc8855fb68acbd31a7"
+dependencies = [
+ "core-foundation-sys",
+ "libc",
+]
+
+[[package]]
 name = "semver"
 version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bebd363326d05ec3e2f532ab7660680f3b02130d780c299bca73469d521bc0ed"
 
 [[package]]
 name = "seq-macro"
 version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e6b44e8fc93a14e66336d230954dda83d18b4605ccace8fe09bc7514a71ad0bc"
 
 [[package]]
 name = "serde"
-version = "1.0.162"
+version = "1.0.163"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "71b2f6e1ab5c2b98c05f0f35b236b22e8df7ead6ffbf51d7808da7f8817e7ab6"
+checksum = "2113ab51b87a539ae008b5c6c02dc020ffa39afd2d83cffcb3f4eb2722cebec2"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.162"
+version = "1.0.163"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a2a0814352fd64b58489904a44ea8d90cb1a91dcb6b4f5ebabc32c8318e93cb6"
+checksum = "8c805777e3930c8883389c602315a24224bcc738b63905ef87cd1420353ea93e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.16",
 ]
 
 [[package]]
 name = "serde_json"
 version = "1.0.96"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
@@ -2677,24 +2752,30 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.15"
+version = "2.0.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a34fcf3e8b60f57e6a14301a2e916d323af98b0ea63c599441eec8558660c822"
+checksum = "a6f671d4b5ffdb8eadec19c0ae67fe2639df8684bd7bc4b83d986b8db549cf01"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
+name = "tap"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "55937e1799185b12863d447f42597ed69d9928686b8d88a1df17376a097d8369"
+
+[[package]]
 name = "target-lexicon"
 version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
 name = "tempfile"
@@ -2737,15 +2818,15 @@
 name = "thiserror-impl"
 version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.16",
 ]
 
 [[package]]
 name = "thrift"
 version = "0.17.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7e54bc85fc7faa8bc175c4bab5b92ba8d9a3ce893d0e9f42cc455c8ab16a9e09"
@@ -2798,17 +2879,17 @@
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "tokio"
-version = "1.28.0"
+version = "1.28.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c3c786bf8134e5a3a166db9b29ab8f48134739014a3eca7bc6bfa95d673b136f"
+checksum = "0aa32867d44e6f2ce3385e89dceb990188b8bb0fb25b0cf576647a6f98ac5105"
 dependencies = [
  "autocfg",
  "bytes",
  "libc",
  "mio",
  "num_cpus",
  "parking_lot",
@@ -2823,15 +2904,25 @@
 name = "tokio-macros"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "630bdcf245f78637c13ec01ffae6187cca34625e8c63150d424b59e55af2675e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.16",
+]
+
+[[package]]
+name = "tokio-native-tls"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bbae76ab933c85776efabc971569dd6119c580d8f5d448769dec1764bf796ef2"
+dependencies = [
+ "native-tls",
+ "tokio",
 ]
 
 [[package]]
 name = "tokio-stream"
 version = "0.1.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "397c988d37662c7dda6d2208364a706264bf3d6138b11d436cbac0ad38832842"
@@ -2885,22 +2976,22 @@
 name = "tracing-attributes"
 version = "0.1.24"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0f57e3ca2a01450b1a921183a9c9cbfda207fd822cef4ccb00a65402cbba7a74"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.16",
 ]
 
 [[package]]
 name = "tracing-core"
-version = "0.1.30"
+version = "0.1.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "24eb03ba0eab1fd845050058ce5e616558e8f8d8fca633e6b163fe25c797213a"
+checksum = "0955b8137a1df6f1a2e9a37d8a6656291ff0297c1a97c24e0d8425fe2312f79a"
 dependencies = [
  "once_cell",
 ]
 
 [[package]]
 name = "try-lock"
 version = "0.2.4"
@@ -2965,22 +3056,28 @@
  "form_urlencoded",
  "idna",
  "percent-encoding",
 ]
 
 [[package]]
 name = "uuid"
-version = "1.3.2"
+version = "1.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4dad5567ad0cf5b760e5665964bec1b47dfd077ba8a2544b513f3556d3d239a2"
+checksum = "345444e32442451b267fc254ae85a209c64be56d2890e601a0c37ff0c3c5ecd2"
 dependencies = [
  "getrandom",
 ]
 
 [[package]]
+name = "vcpkg"
+version = "0.2.15"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "accd4ea62f7bb7a82fe23066fb0957d48ef677f6eeb8215f372f52e48bb32426"
+
+[[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
 name = "walkdir"
@@ -3012,71 +3109,71 @@
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.84"
+version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "31f8dcbc21f30d9b8f2ea926ecb58f6b91192c17e9d33594b3df58b2007ca53b"
+checksum = "5bba0e8cb82ba49ff4e229459ff22a191bbe9a1cb3a341610c9c33efc27ddf73"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.84"
+version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "95ce90fd5bcc06af55a641a86428ee4229e44e07033963a2290a8e241607ccb9"
+checksum = "19b04bc93f9d6bdee709f6bd2118f57dd6679cf1176a1af464fca3ab0d66d8fb"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.16",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.84"
+version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c21f77c0bedc37fd5dc21f897894a5ca01e7bb159884559461862ae90c0b4c5"
+checksum = "14d6b024f1a526bb0234f52840389927257beb670610081360e5a03c5df9c258"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.84"
+version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2aff81306fcac3c7515ad4e177f521b5c9a15f2b08f4e32d823066102f35a5f6"
+checksum = "e128beba882dd1eb6200e1dc92ae6c5dbaa4311aa7bb211ca035779e5efc39f8"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.16",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.84"
+version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0046fef7e28c3804e5e38bfa31ea2a0f73905319b677e57ebe37e49358989b5d"
+checksum = "ed9d5b4305409d1fc9482fee2d7f9bcbf24b3972bf59817ef757e23982242a93"
 
 [[package]]
 name = "web-sys"
-version = "0.3.61"
+version = "0.3.63"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e33b99f4b23ba3eec1a53ac264e35a755f00e966e0065077d6027c0f575b0b97"
+checksum = "3bdd9ef4e984da1187bf8110c5cf5b845fbc87a23602cdf912386a76fcd3a7c2"
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "winapi"
@@ -3116,14 +3213,29 @@
 checksum = "e686886bc078bc1b0b600cac0147aadb815089b6e4da64016cbd754b6342700f"
 dependencies = [
  "windows-targets 0.48.0",
 ]
 
 [[package]]
 name = "windows-sys"
+version = "0.42.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5a3e1820f08b8513f676f7ab6c1f99ff312fb97b553d30ff4dd86f9f15728aa7"
+dependencies = [
+ "windows_aarch64_gnullvm 0.42.2",
+ "windows_aarch64_msvc 0.42.2",
+ "windows_i686_gnu 0.42.2",
+ "windows_i686_msvc 0.42.2",
+ "windows_x86_64_gnu 0.42.2",
+ "windows_x86_64_gnullvm 0.42.2",
+ "windows_x86_64_msvc 0.42.2",
+]
+
+[[package]]
+name = "windows-sys"
 version = "0.45.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
 dependencies = [
  "windows-targets 0.42.2",
 ]
 
@@ -3247,14 +3359,23 @@
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
 
 [[package]]
+name = "wyz"
+version = "0.5.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "05f360fc0b24296329c78fda852a1e9ae82de9cf7b27dae4b7f62f118f77b9ed"
+dependencies = [
+ "tap",
+]
+
+[[package]]
 name = "xz2"
 version = "0.1.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "388c44dc09d76f1536602ead6d325eb532f5c122f17782bd57fb47baeeb767e2"
 dependencies = [
  "lzma-sys",
 ]
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/Cargo.toml` & `nautilus_trader-1.174.0/nautilus_core/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,35 +8,34 @@
     "network",
     "persistence",
     "pyo3"
 ]
 
 [workspace.package]
 rust-version = "1.69.0"
-version = "0.4.0"
+version = "0.5.0"
 edition = "2021"
 authors = ["Nautech Systems <info@nautechsystems.io>"]
 description = "A high-performance algorithmic trading platform and event-driven backtester"
 documentation = "https://docs.nautilustrader.io"
 
 [workspace.dependencies]
 chrono = "0.4.24"
 pyo3 = "0.18.3"
 pyo3-asyncio = { version = "0.18.0", features = [ "tokio-runtime", "tokio", "attributes" ] }
 pyo3-macros = "0.18.3"
 rand = "0.8.5"
 rust_decimal = "1.29.1"
 rust_decimal_macros = "1.29.1"
-rust-fsm = "0.6.1"
 serde = { version = "1.0", features = ["derive"] }
 serde_json = "1.0"
 strum = { version = "0.24.1", features = ["derive"] }
 thiserror = "1.0.40"
-tokio = { version = "1.28.0", features = ["full"] }
-uuid = { version = "1.3.2", features = ["v4"] }
+tokio = { version = "1.28.1", features = ["full"] }
+uuid = { version = "1.3.3", features = ["v4"] }
 
 # dev-dependencies
 criterion = "0.4.0"
 iai = "0.1"
 rstest = "0.17.0"
 tempfile = "3.5.0"
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/LICENSE` & `nautilus_trader-1.174.0/nautilus_core/LICENSE`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_core/README.md` & `nautilus_trader-1.174.0/nautilus_core/README.md`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_core/backtest/Cargo.toml` & `nautilus_trader-1.174.0/nautilus_core/backtest/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_core/backtest/build.rs` & `nautilus_trader-1.174.0/nautilus_core/backtest/build.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_core/backtest/cbindgen_cython.toml` & `nautilus_trader-1.174.0/nautilus_core/backtest/cbindgen_cython.toml`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 ]
 
 "cpython.object" = [
     "PyObject",
 ]
 
 "nautilus_trader.core.rust.common" = [
-    "TestClockAPI",
+    "TestClock_API",
+    "LiveClock_API",
 ]
 
 "nautilus_trader.core.rust.core" = [
     "CVec",
     "UUID4_t",
 ]
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/backtest/src/engine.rs` & `nautilus_trader-1.174.0/nautilus_core/backtest/src/engine.rs`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
 use std::ops::{Deref, DerefMut};
 
-use nautilus_common::clock::{TestClock, TestClockAPI};
+use nautilus_common::clock::{TestClock, TestClock_API};
 use nautilus_common::timer::TimeEventHandler;
 use nautilus_core::cvec::CVec;
 use nautilus_core::time::UnixNanos;
 
 /// Provides a means of accumulating and draining time event handlers.
 pub struct TimeEventAccumulator {
     event_handlers: Vec<TimeEventHandler>,
@@ -49,15 +49,15 @@
             .sort_unstable_by_key(|v| v.event.ts_event);
         self.event_handlers.drain(..).collect()
     }
 }
 
 impl Default for TimeEventAccumulator {
     fn default() -> Self {
-        TimeEventAccumulator::new()
+        Self::new()
     }
 }
 
 ////////////////////////////////////////////////////////////////////////////////
 // C API
 ////////////////////////////////////////////////////////////////////////////////
 
@@ -87,15 +87,15 @@
 pub extern "C" fn time_event_accumulator_drop(accumulator: TimeEventAccumulatorAPI) {
     drop(accumulator); // Memory freed here
 }
 
 #[no_mangle]
 pub extern "C" fn time_event_accumulator_advance_clock(
     accumulator: &mut TimeEventAccumulatorAPI,
-    clock: &mut TestClockAPI,
+    clock: &mut TestClock_API,
     to_time_ns: UnixNanos,
     set_time: u8,
 ) {
     accumulator.advance_clock(clock, to_time_ns, set_time != 0);
 }
 
 #[no_mangle]
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/backtest/src/lib.rs` & `nautilus_trader-1.174.0/nautilus_core/backtest/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_core/common/Cargo.toml` & `nautilus_trader-1.174.0/nautilus_core/common/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_core/common/build.rs` & `nautilus_trader-1.174.0/nautilus_core/common/build.rs`

 * *Files 2% similar despite different names*

```diff
@@ -50,11 +50,10 @@
     drop(src); // Close the file early
 
     // Run the replace operation in memory
     let new_data = data.replace("cdef enum", "cpdef enum");
 
     // Recreate the file and dump the processed contents to it
     let mut dst = File::create(cython_path).expect("`File::create` failed");
-    let _ = dst
-        .write(new_data.as_bytes())
+    dst.write_all(new_data.as_bytes())
         .expect("I/O error on `dist.write`");
 }
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/common/cbindgen.toml` & `nautilus_trader-1.174.0/nautilus_core/common/cbindgen.toml`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_core/common/cbindgen_cython.toml` & `nautilus_trader-1.174.0/nautilus_core/common/cbindgen_cython.toml`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_core/common/src/clock.rs` & `nautilus_trader-1.174.0/nautilus_core/common/src/clock.rs`

 * *Files 2% similar despite different names*

```diff
@@ -464,105 +464,105 @@
         self.timers = HashMap::new();
     }
 }
 
 ////////////////////////////////////////////////////////////////////////////////
 // C API - TestClock
 ////////////////////////////////////////////////////////////////////////////////
-
+#[allow(non_camel_case_types)]
 #[repr(C)]
-pub struct TestClockAPI(Box<TestClock>);
+pub struct TestClock_API(Box<TestClock>);
 
-impl Deref for TestClockAPI {
+impl Deref for TestClock_API {
     type Target = TestClock;
 
     fn deref(&self) -> &Self::Target {
         &self.0
     }
 }
 
-impl DerefMut for TestClockAPI {
+impl DerefMut for TestClock_API {
     fn deref_mut(&mut self) -> &mut Self::Target {
         &mut self.0
     }
 }
 
 #[no_mangle]
-pub extern "C" fn test_clock_new() -> TestClockAPI {
-    TestClockAPI(Box::new(TestClock::new()))
+pub extern "C" fn test_clock_new() -> TestClock_API {
+    TestClock_API(Box::new(TestClock::new()))
 }
 
 #[no_mangle]
-pub extern "C" fn test_clock_drop(clock: TestClockAPI) {
+pub extern "C" fn test_clock_drop(clock: TestClock_API) {
     drop(clock); // Memory freed here
 }
 
 /// # Safety
 /// - Assumes `callback_ptr` is a valid PyCallable pointer.
 #[no_mangle]
 pub unsafe extern "C" fn test_clock_register_default_handler(
-    clock: &mut TestClockAPI,
+    clock: &mut TestClock_API,
     callback_ptr: *mut ffi::PyObject,
 ) {
     assert!(!callback_ptr.is_null());
     assert!(ffi::Py_None() != callback_ptr);
 
     let callback_py = Python::with_gil(|py| PyObject::from_borrowed_ptr(py, callback_ptr));
     clock.register_default_handler_py(callback_py);
 }
 
 #[no_mangle]
-pub extern "C" fn test_clock_set_time(clock: &mut TestClockAPI, to_time_ns: u64) {
+pub extern "C" fn test_clock_set_time(clock: &mut TestClock_API, to_time_ns: u64) {
     clock.set_time(to_time_ns);
 }
 
 #[no_mangle]
-pub extern "C" fn test_clock_timestamp(clock: &mut TestClockAPI) -> f64 {
+pub extern "C" fn test_clock_timestamp(clock: &mut TestClock_API) -> f64 {
     clock.timestamp()
 }
 
 #[no_mangle]
-pub extern "C" fn test_clock_timestamp_ms(clock: &mut TestClockAPI) -> u64 {
+pub extern "C" fn test_clock_timestamp_ms(clock: &mut TestClock_API) -> u64 {
     clock.timestamp_ms()
 }
 
 #[no_mangle]
-pub extern "C" fn test_clock_timestamp_us(clock: &mut TestClockAPI) -> u64 {
+pub extern "C" fn test_clock_timestamp_us(clock: &mut TestClock_API) -> u64 {
     clock.timestamp_us()
 }
 
 #[no_mangle]
-pub extern "C" fn test_clock_timestamp_ns(clock: &mut TestClockAPI) -> u64 {
+pub extern "C" fn test_clock_timestamp_ns(clock: &mut TestClock_API) -> u64 {
     clock.timestamp_ns()
 }
 
 #[no_mangle]
-pub extern "C" fn test_clock_timer_names(clock: &TestClockAPI) -> *mut ffi::PyObject {
+pub extern "C" fn test_clock_timer_names(clock: &TestClock_API) -> *mut ffi::PyObject {
     Python::with_gil(|py| -> Py<PyList> {
         let names: Vec<Py<PyString>> = clock
             .timers
             .keys()
             .map(|k| PyString::new(py, k).into())
             .collect();
         PyList::new(py, names).into()
     })
     .as_ptr()
 }
 
 #[no_mangle]
-pub extern "C" fn test_clock_timer_count(clock: &mut TestClockAPI) -> usize {
+pub extern "C" fn test_clock_timer_count(clock: &mut TestClock_API) -> usize {
     clock.timer_count()
 }
 
 /// # Safety
 /// - Assumes `name_ptr` is a valid C string pointer.
 /// - Assumes `callback_ptr` is a valid PyCallable pointer.
 #[no_mangle]
 pub unsafe extern "C" fn test_clock_set_time_alert_ns(
-    clock: &mut TestClockAPI,
+    clock: &mut TestClock_API,
     name_ptr: *const c_char,
     alert_time_ns: UnixNanos,
     callback_ptr: *mut ffi::PyObject,
 ) {
     assert!(!callback_ptr.is_null());
 
     let name = cstr_to_string(name_ptr);
@@ -574,15 +574,15 @@
 }
 
 /// # Safety
 /// - Assumes `name_ptr` is a valid C string pointer.
 /// - Assumes `callback_ptr` is a valid PyCallable pointer.
 #[no_mangle]
 pub unsafe extern "C" fn test_clock_set_timer_ns(
-    clock: &mut TestClockAPI,
+    clock: &mut TestClock_API,
     name_ptr: *const c_char,
     interval_ns: u64,
     start_time_ns: UnixNanos,
     stop_time_ns: UnixNanos,
     callback_ptr: *mut ffi::PyObject,
 ) {
     assert!(!callback_ptr.is_null());
@@ -599,15 +599,15 @@
     clock.set_timer_ns_py(name, interval_ns, start_time_ns, stop_time_ns, callback_py);
 }
 
 /// # Safety
 /// - Assumes `set_time` is a correct `uint8_t` of either 0 or 1.
 #[no_mangle]
 pub unsafe extern "C" fn test_clock_advance_time(
-    clock: &mut TestClockAPI,
+    clock: &mut TestClock_API,
     to_time_ns: u64,
     set_time: u8,
 ) -> CVec {
     let events: Vec<TimeEvent> = clock.advance_time(to_time_ns, set_time != 0);
     clock.match_handlers_py(events).into()
 }
 
@@ -622,85 +622,85 @@
     drop(data); // Memory freed here
 }
 
 /// # Safety
 /// - Assumes `name_ptr` is a valid C string pointer.
 #[no_mangle]
 pub unsafe extern "C" fn test_clock_next_time_ns(
-    clock: &mut TestClockAPI,
+    clock: &mut TestClock_API,
     name_ptr: *const c_char,
 ) -> UnixNanos {
     let name = cstr_to_string(name_ptr);
     clock.next_time_ns(&name)
 }
 
 /// # Safety
 /// - Assumes `name_ptr` is a valid C string pointer.
 #[no_mangle]
 pub unsafe extern "C" fn test_clock_cancel_timer(
-    clock: &mut TestClockAPI,
+    clock: &mut TestClock_API,
     name_ptr: *const c_char,
 ) {
     let name = cstr_to_string(name_ptr);
     clock.cancel_timer(&name);
 }
 
 #[no_mangle]
-pub extern "C" fn test_clock_cancel_timers(clock: &mut TestClockAPI) {
+pub extern "C" fn test_clock_cancel_timers(clock: &mut TestClock_API) {
     clock.cancel_timers();
 }
 
 ////////////////////////////////////////////////////////////////////////////////
 // C API - LiveClock
 ////////////////////////////////////////////////////////////////////////////////
-
+#[allow(non_camel_case_types)]
 #[repr(C)]
-pub struct LiveClockAPI(Box<LiveClock>);
+pub struct LiveClock_API(Box<LiveClock>);
 
-impl Deref for LiveClockAPI {
+impl Deref for LiveClock_API {
     type Target = LiveClock;
 
     fn deref(&self) -> &Self::Target {
         &self.0
     }
 }
 
-impl DerefMut for LiveClockAPI {
+impl DerefMut for LiveClock_API {
     fn deref_mut(&mut self) -> &mut Self::Target {
         &mut self.0
     }
 }
 
 #[no_mangle]
-pub extern "C" fn live_clock_new() -> LiveClockAPI {
-    LiveClockAPI(Box::new(LiveClock::new()))
+pub extern "C" fn live_clock_new() -> LiveClock_API {
+    LiveClock_API(Box::new(LiveClock::new()))
 }
 
 #[no_mangle]
-pub extern "C" fn live_clock_drop(clock: LiveClockAPI) {
+pub extern "C" fn live_clock_drop(clock: LiveClock_API) {
     drop(clock); // Memory freed here
 }
 
 #[no_mangle]
-pub extern "C" fn live_clock_timestamp(clock: &mut LiveClockAPI) -> f64 {
+pub extern "C" fn live_clock_timestamp(clock: &mut LiveClock_API) -> f64 {
     clock.timestamp()
 }
 
 #[no_mangle]
-pub extern "C" fn live_clock_timestamp_ms(clock: &mut LiveClockAPI) -> u64 {
+pub extern "C" fn live_clock_timestamp_ms(clock: &mut LiveClock_API) -> u64 {
     clock.timestamp_ms()
 }
 
 #[no_mangle]
-pub extern "C" fn live_clock_timestamp_us(clock: &mut LiveClockAPI) -> u64 {
+pub extern "C" fn live_clock_timestamp_us(clock: &mut LiveClock_API) -> u64 {
     clock.timestamp_us()
 }
 
 #[no_mangle]
-pub extern "C" fn live_clock_timestamp_ns(clock: &mut LiveClockAPI) -> u64 {
+pub extern "C" fn live_clock_timestamp_ns(clock: &mut LiveClock_API) -> u64 {
     clock.timestamp_ns()
 }
 
 ////////////////////////////////////////////////////////////////////////////////
 // Tests
 ////////////////////////////////////////////////////////////////////////////////
 #[cfg(test)]
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/common/src/enums.rs` & `nautilus_trader-1.174.0/nautilus_core/common/src/enums.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_core/common/src/lib.rs` & `nautilus_trader-1.174.0/nautilus_core/common/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_core/common/src/logging.rs` & `nautilus_trader-1.174.0/nautilus_core/common/src/logging.rs`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     #[serde(skip_serializing)]
     color: LogColor,
     component: String,
     msg: String,
 }
 
 impl fmt::Display for LogMessage {
-    fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
+    fn fmt(&self, f: &mut fmt::Formatter<'_>) -> std::fmt::Result {
         write!(
             f,
             "{} [{}] {}: {}",
             self.timestamp_ns, self.level, self.component, self.msg
         )
     }
 }
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/common/src/msgbus.rs` & `nautilus_trader-1.174.0/nautilus_core/common/src/msgbus.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_core/common/src/testing.rs` & `nautilus_trader-1.174.0/nautilus_core/common/src/testing.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_core/common/src/timer.rs` & `nautilus_trader-1.174.0/nautilus_core/common/src/timer.rs`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
 use std::cmp::Ordering;
 use std::ffi::c_char;
-use std::fmt;
+use std::fmt::{Display, Formatter};
 use std::rc::Rc;
 
 use nautilus_core::correctness;
 use nautilus_core::string::{cstr_to_string, string_to_cstr};
 use nautilus_core::time::{TimedeltaNanos, UnixNanos};
 use nautilus_core::uuid::UUID4;
 use pyo3::ffi;
@@ -49,16 +49,16 @@
             event_id,
             ts_event,
             ts_init,
         }
     }
 }
 
-impl fmt::Display for TimeEvent {
-    fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
+impl Display for TimeEvent {
+    fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         write!(
             f,
             "TimeEvent(name={}, event_id={}, ts_event={}, ts_init={})",
             self.name, self.event_id, self.ts_event, self.ts_init
         )
     }
 }
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/common/tests/test_clock.rs` & `nautilus_trader-1.174.0/nautilus_core/common/tests/test_clock.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_core/core/Cargo.toml` & `nautilus_trader-1.174.0/nautilus_core/core/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_core/core/benches/criterion_time_benchmark.rs` & `nautilus_trader-1.174.0/nautilus_core/core/benches/criterion_time_benchmark.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_core/core/build.rs` & `nautilus_trader-1.174.0/nautilus_core/core/build.rs`

 * *Files 2% similar despite different names*

```diff
@@ -50,11 +50,10 @@
     drop(src); // Close the file early
 
     // Run the replace operation in memory
     let new_data = data.replace("cdef enum", "cpdef enum");
 
     // Recreate the file and dump the processed contents to it
     let mut dst = File::create(cython_path).expect("`File::create` failed");
-    let _ = dst
-        .write(new_data.as_bytes())
+    dst.write_all(new_data.as_bytes())
         .expect("I/O error on `dist.write`");
 }
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/core/cbindgen.toml` & `nautilus_trader-1.174.0/nautilus_core/core/cbindgen.toml`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_core/core/cbindgen_cython.toml` & `nautilus_trader-1.174.0/nautilus_core/core/cbindgen_cython.toml`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_core/core/src/correctness.rs` & `nautilus_trader-1.174.0/nautilus_core/core/src/correctness.rs`

 * *Files 0% similar despite different names*

```diff
@@ -9,29 +9,29 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
-const FAILED: &str = "condition check failed:";
+const FAILED: &str = "Condition check failed:";
 
 /// Check string `s` is valid.
 ///
 /// # Panics
 /// - If `s` is empty.
 /// - If `s` is all whitespace.
 /// - If `s` contains a Non-ASCII character.
 pub fn valid_string(s: &str, desc: &str) {
     if s.is_empty() {
         panic!("{FAILED} invalid string for {desc}, was empty");
     } else if s.as_bytes().iter().all(u8::is_ascii_whitespace) {
         panic!("{FAILED} invalid string for {desc}, was all whitespace");
     } else if !s.is_ascii() {
-        panic!("{FAILED} invalid string for {desc} contained a Non-ASCII char, was '{s}'");
+        panic!("{FAILED} invalid string for {desc} contained a non-ASCII char, was '{s}'");
     }
 }
 
 /// Check string `s` contains pattern `pat`.
 ///
 /// # Panics
 /// - If `s` does not contain `pat`.
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/core/src/cvec.rs` & `nautilus_trader-1.174.0/nautilus_core/core/src/cvec.rs`

 * *Files 12% similar despite different names*

```diff
@@ -9,23 +9,27 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
-use std::{ffi::c_void, ptr::null};
+use std::{
+    ffi::c_void,
+    fmt::{Display, Formatter},
+    ptr::null,
+};
 
 /// `CVec` is a C compatible struct that stores an opaque pointer to a block of
 /// memory, it's length and the capacity of the vector it was allocated from.
 ///
 /// NOTE: Changing the values here may lead to undefined behaviour when the
 /// memory is dropped.
 #[repr(C)]
-#[derive(Clone, Copy)]
+#[derive(Clone, Copy, Debug)]
 pub struct CVec {
     /// Opaque pointer to block of memory storing elements to access the
     /// elements cast it to the underlying type.
     pub ptr: *mut c_void,
     /// The number of elements in the block.
     pub len: usize,
     /// The capacity of vector from which it was allocated.
@@ -66,14 +70,24 @@
                 len,
                 cap,
             }
         }
     }
 }
 
+impl Display for CVec {
+    fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
+        write!(
+            f,
+            "CVec {{ ptr: {:?}, len: {}, cap: {} }}",
+            self.ptr, self.len, self.cap,
+        )
+    }
+}
+
 ////////////////////////////////////////////////////////////////////////////////
 // C API
 ////////////////////////////////////////////////////////////////////////////////
 #[no_mangle]
 pub extern "C" fn cvec_drop(cvec: CVec) {
     let CVec { ptr, len, cap } = cvec;
     let data: Vec<u8> = unsafe { Vec::from_raw_parts(ptr.cast::<u8>(), len, cap) };
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/core/src/datetime.rs` & `nautilus_trader-1.174.0/nautilus_core/core/src/datetime.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_core/core/src/lib.rs` & `nautilus_trader-1.174.0/nautilus_core/core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_core/core/src/parsing.rs` & `nautilus_trader-1.174.0/nautilus_core/core/src/parsing.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_core/core/src/string.rs` & `nautilus_trader-1.174.0/nautilus_core/core/src/string.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_core/core/src/time.rs` & `nautilus_trader-1.174.0/nautilus_core/core/src/time.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_core/core/src/uuid.rs` & `nautilus_trader-1.174.0/nautilus_core/core/src/uuid.rs`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
 use std::collections::hash_map::DefaultHasher;
 use std::ffi::{c_char, CStr};
-use std::fmt::{Debug, Display, Formatter, Result};
+use std::fmt::{Debug, Display, Formatter};
 use std::hash::{Hash, Hasher};
 use std::rc::Rc;
 
 use uuid::Uuid;
 
 use crate::string::string_to_cstr;
 
@@ -53,15 +53,15 @@
 impl Default for UUID4 {
     fn default() -> Self {
         Self::new()
     }
 }
 
 impl Display for UUID4 {
-    fn fmt(&self, f: &mut Formatter<'_>) -> Result {
+    fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         write!(f, "{}", self.value)
     }
 }
 
 ////////////////////////////////////////////////////////////////////////////////
 // C API
 ////////////////////////////////////////////////////////////////////////////////
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/indicators/src/ema.rs` & `nautilus_trader-1.174.0/nautilus_core/indicators/src/ema.rs`

 * *Files 2% similar despite different names*

```diff
@@ -36,16 +36,17 @@
     _has_inputs: bool,
     _is_initialized: bool,
 }
 
 #[pymethods]
 impl ExponentialMovingAverage {
     #[new]
+    #[must_use]
     pub fn new(period: usize, price_type: Option<PriceType>) -> Self {
-        ExponentialMovingAverage {
+        Self {
             period,
             price_type: price_type.unwrap_or(PriceType::Last),
             alpha: 2.0 / (period as f64 + 1.0),
             value: 0.0,
             count: 0,
             _has_inputs: false,
             _is_initialized: false,
@@ -54,15 +55,15 @@
 
     pub fn update_raw(&mut self, value: f64) {
         if !self._has_inputs {
             self._has_inputs = true;
             self.value = value;
         }
 
-        self.value = self.alpha * value + ((1.0 - self.alpha) * self.value);
+        self.value = self.alpha.mul_add(value, (1.0 - self.alpha) * self.value);
         self.count += 1;
 
         // Initialization logic
         if !self._is_initialized && self.count >= self.period {
             self._is_initialized = true;
         }
     }
@@ -103,15 +104,15 @@
 #[cfg(test)]
 mod tests {
     use super::*;
 
     #[test]
     fn test_ema_initialized() {
         let ema = ExponentialMovingAverage::new(20, Some(PriceType::Mid));
-        let display_str = format!("{:?}", ema);
+        let display_str = format!("{ema:?}");
         assert_eq!(display_str, "ExponentialMovingAverage { period: 20, price_type: Mid, alpha: 0.09523809523809523, value: 0.0, count: 0, _has_inputs: false, _is_initialized: false }");
     }
 
     #[test]
     fn test_ema_update_raw() {
         let mut ema = ExponentialMovingAverage::new(3, Some(PriceType::Mid));
         ema.update_raw(1.0);
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/indicators/src/lib.rs` & `nautilus_trader-1.174.0/nautilus_core/indicators/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_core/model/Cargo.toml` & `nautilus_trader-1.174.0/nautilus_core/model/Cargo.toml`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 name = "nautilus_model"
 crate-type = ["rlib", "staticlib"]
 
 [dependencies]
 nautilus_core = { path = "../core" }
 pyo3.workspace = true
 rust_decimal.workspace = true
-rust-fsm.workspace = true
 strum.workspace = true
 thiserror.workspace = true
 derive_builder = "0.12.0"
 lazy_static = "1.4.0"
 
 [features]
 extension-module = [
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/model/build.rs` & `nautilus_trader-1.174.0/nautilus_core/model/build.rs`

 * *Files 3% similar despite different names*

```diff
@@ -50,11 +50,10 @@
     drop(src); // Close the file early
 
     // Run the replace operation in memory
     let new_data = data.replace("cdef enum", "cpdef enum");
 
     // Recreate the file and dump the processed contents to it
     let mut dst = File::create(cython_path).expect("`File::create` failed");
-    let _ = dst
-        .write(new_data.as_bytes())
+    dst.write_all(new_data.as_bytes())
         .expect("I/O error on `dist.write`");
 }
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/model/cbindgen.toml` & `nautilus_trader-1.174.0/nautilus_core/model/cbindgen.toml`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_core/model/cbindgen_cython.toml` & `nautilus_trader-1.174.0/nautilus_core/model/cbindgen_cython.toml`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,19 @@
 "libc.stdint" = [
     "uint8_t",
     "uint16_t",
     "uint64_t",
     "int64_t",
 ]
 
+"nautilus_trader.core.rust.core" = [
+    "CVec",
+    "UUID4_t",
+]
+
 [enum]
 rename_variants = "ScreamingSnakeCase"
 
 [export]
 exclude = [
     "BarAggregation",
 ]
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/model/src/currencies.rs` & `nautilus_trader-1.174.0/nautilus_core/model/src/currencies.rs`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 // Defines currency definition constants
 
 use std::{collections::HashMap, sync::Arc};
 
 use crate::{enums::CurrencyType, types::currency::Currency};
 
+#[must_use]
 pub fn currency_map() -> HashMap<String, Currency> {
     [
         // Fiat currencies
         (String::from("AUD"), AUD.clone()),
         (String::from("BRL"), BRL.clone()),
         (String::from("CAD"), CAD.clone()),
         (String::from("CHF"), CHF.clone()),
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/model/src/data/bar.rs` & `nautilus_trader-1.174.0/nautilus_core/model/src/data/bar.rs`

 * *Files 21% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
 use std::cmp::Ordering;
 use std::collections::hash_map::DefaultHasher;
 use std::ffi::c_char;
-use std::fmt::{Debug, Display, Formatter, Result};
+use std::fmt::{Debug, Display, Formatter};
 use std::hash::{Hash, Hasher};
+use std::str::FromStr;
 
 use nautilus_core::string::string_to_cstr;
 use nautilus_core::time::UnixNanos;
+use thiserror::Error;
 
 use crate::enums::{AggregationSource, BarAggregation, PriceType};
 use crate::identifiers::instrument_id::InstrumentId;
 use crate::types::price::Price;
 use crate::types::quantity::Quantity;
 
 #[repr(C)]
@@ -32,15 +34,15 @@
 pub struct BarSpecification {
     pub step: u64,
     pub aggregation: BarAggregation,
     pub price_type: PriceType,
 }
 
 impl Display for BarSpecification {
-    fn fmt(&self, f: &mut Formatter<'_>) -> Result {
+    fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         write!(f, "{}-{}-{}", self.step, self.aggregation, self.price_type)
     }
 }
 
 impl PartialOrd for BarSpecification {
     fn partial_cmp(&self, other: &Self) -> Option<Ordering> {
         self.to_string().partial_cmp(&other.to_string())
@@ -121,14 +123,80 @@
 #[derive(Clone, Debug)]
 pub struct BarType {
     pub instrument_id: InstrumentId,
     pub spec: BarSpecification,
     pub aggregation_source: AggregationSource,
 }
 
+#[derive(Debug, Error)]
+#[error("Error parsing `BarType` from '{input}', invalid token: '{token}' at position {position}")]
+pub struct BarTypeParseError {
+    input: String,
+    token: String,
+    position: usize,
+}
+
+impl FromStr for BarType {
+    type Err = BarTypeParseError;
+
+    fn from_str(s: &str) -> Result<Self, Self::Err> {
+        // TODO: Requires handling some trait related thing
+        #[allow(clippy::needless_collect)]
+        let pieces: Vec<&str> = s.rsplitn(5, '-').collect();
+        let rev_pieces: Vec<&str> = pieces.into_iter().rev().collect();
+        if rev_pieces.len() != 5 {
+            return Err(BarTypeParseError {
+                input: s.to_string(),
+                token: "".to_string(),
+                position: 0,
+            });
+        }
+
+        let instrument_id =
+            InstrumentId::from_str(rev_pieces[0]).map_err(|_| BarTypeParseError {
+                input: s.to_string(),
+                token: rev_pieces[0].to_string(),
+                position: 0,
+            })?;
+
+        let step = rev_pieces[1].parse().map_err(|_| BarTypeParseError {
+            input: s.to_string(),
+            token: rev_pieces[1].to_string(),
+            position: 1,
+        })?;
+        let aggregation =
+            BarAggregation::from_str(rev_pieces[2]).map_err(|_| BarTypeParseError {
+                input: s.to_string(),
+                token: rev_pieces[2].to_string(),
+                position: 2,
+            })?;
+        let price_type = PriceType::from_str(rev_pieces[3]).map_err(|_| BarTypeParseError {
+            input: s.to_string(),
+            token: rev_pieces[3].to_string(),
+            position: 3,
+        })?;
+        let aggregation_source =
+            AggregationSource::from_str(rev_pieces[4]).map_err(|_| BarTypeParseError {
+                input: s.to_string(),
+                token: rev_pieces[4].to_string(),
+                position: 4,
+            })?;
+
+        Ok(BarType {
+            instrument_id,
+            spec: BarSpecification {
+                step,
+                aggregation,
+                price_type,
+            },
+            aggregation_source,
+        })
+    }
+}
+
 impl PartialEq for BarType {
     fn eq(&self, other: &Self) -> bool {
         self.instrument_id == other.instrument_id
             && self.spec == other.spec
             && self.aggregation_source == other.aggregation_source
     }
 }
@@ -159,15 +227,15 @@
 
     fn ge(&self, other: &Self) -> bool {
         self.to_string().ge(&other.to_string())
     }
 }
 
 impl Display for BarType {
-    fn fmt(&self, f: &mut Formatter<'_>) -> Result {
+    fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         write!(
             f,
             "{}-{}-{}",
             self.instrument_id, self.spec, self.aggregation_source
         )
     }
 }
@@ -175,15 +243,15 @@
 #[no_mangle]
 pub extern "C" fn bar_type_new(
     instrument_id: InstrumentId,
     spec: BarSpecification,
     aggregation_source: u8,
 ) -> BarType {
     let aggregation_source = AggregationSource::from_repr(aggregation_source as usize)
-        .expect("error converting enum from integer");
+        .expect("Error converting enum from integer");
     BarType {
         instrument_id,
         spec,
         aggregation_source,
     }
 }
 
@@ -245,15 +313,15 @@
     pub close: Price,
     pub volume: Quantity,
     pub ts_event: UnixNanos,
     pub ts_init: UnixNanos,
 }
 
 impl Display for Bar {
-    fn fmt(&self, f: &mut Formatter<'_>) -> Result {
+    fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         write!(
             f,
             "{},{},{},{},{},{},{}",
             self.bar_type, self.open, self.high, self.low, self.close, self.volume, self.ts_event
         )
     }
 }
@@ -401,14 +469,98 @@
             price_type: PriceType::Bid,
         };
         assert_eq!(bar_spec.to_string(), "1-MINUTE-BID");
         assert_eq!(format!("{bar_spec}"), "1-MINUTE-BID");
     }
 
     #[test]
+    fn test_bar_type_parse_valid() {
+        let input = "BTCUSDT-PERP.BINANCE-1-MINUTE-LAST-EXTERNAL";
+        let bar_type = BarType::from_str(input).unwrap();
+
+        assert_eq!(
+            bar_type.instrument_id,
+            InstrumentId::from_str("BTCUSDT-PERP.BINANCE").unwrap()
+        );
+        assert_eq!(
+            bar_type.spec,
+            BarSpecification {
+                step: 1,
+                aggregation: BarAggregation::Minute,
+                price_type: PriceType::Last,
+            }
+        );
+        assert_eq!(bar_type.aggregation_source, AggregationSource::External);
+    }
+
+    #[test]
+    fn test_bar_type_parse_invalid_token_pos_0() {
+        let input = "BTCUSDT-PERP-1-MINUTE-LAST-INTERNAL";
+        let result = BarType::from_str(input);
+
+        assert_eq!(
+            result.unwrap_err().to_string(),
+            format!("Error parsing `BarType` from '{input}', invalid token: 'BTCUSDT-PERP' at position 0")
+        );
+    }
+
+    #[test]
+    fn test_bar_type_parse_invalid_token_pos_1() {
+        let input = "BTCUSDT-PERP.BINANCE-INVALID-MINUTE-LAST-INTERNAL";
+        let result = BarType::from_str(input);
+
+        assert_eq!(
+            result.unwrap_err().to_string(),
+            format!(
+                "Error parsing `BarType` from '{input}', invalid token: 'INVALID' at position 1"
+            )
+        );
+    }
+
+    #[test]
+    fn test_bar_type_parse_invalid_token_pos_2() {
+        let input = "BTCUSDT-PERP.BINANCE-1-INVALID-LAST-INTERNAL";
+        let result = BarType::from_str(input);
+
+        assert_eq!(
+            result.unwrap_err().to_string(),
+            format!(
+                "Error parsing `BarType` from '{input}', invalid token: 'INVALID' at position 2"
+            )
+        );
+    }
+
+    #[test]
+    fn test_bar_type_parse_invalid_token_pos_3() {
+        let input = "BTCUSDT-PERP.BINANCE-1-MINUTE-INVALID-INTERNAL";
+        let result = BarType::from_str(input);
+
+        assert_eq!(
+            result.unwrap_err().to_string(),
+            format!(
+                "Error parsing `BarType` from '{input}', invalid token: 'INVALID' at position 3"
+            )
+        );
+    }
+
+    #[test]
+    fn test_bar_type_parse_invalid_token_pos_4() {
+        let input = "BTCUSDT-PERP.BINANCE-1-MINUTE-BID-INVALID";
+        let result = BarType::from_str(input);
+
+        assert!(result.is_err());
+        assert_eq!(
+            result.unwrap_err().to_string(),
+            format!(
+                "Error parsing `BarType` from '{input}', invalid token: 'INVALID' at position 4"
+            )
+        );
+    }
+
+    #[test]
     fn test_bar_type_equality() {
         let instrument_id1 = InstrumentId {
             symbol: Symbol::new("AUD/USD"),
             venue: Venue::new("SIM"),
         };
         let instrument_id2 = InstrumentId {
             symbol: Symbol::new("GBP/USD"),
@@ -472,14 +624,15 @@
         };
 
         assert!(bar_type1 <= bar_type2);
         assert!(bar_type1 < bar_type3);
         assert!(bar_type3 > bar_type1);
         assert!(bar_type3 >= bar_type1);
     }
+
     #[test]
     fn test_bar_equality() {
         let instrument_id = InstrumentId {
             symbol: Symbol::new("AUDUSD"),
             venue: Venue::new("SIM"),
         };
         let bar_spec = BarSpecification {
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/model/src/data/mod.rs` & `nautilus_trader-1.174.0/nautilus_trader/__init__.pxd`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,14 @@
-// -------------------------------------------------------------------------------------------------
-//  Copyright (C) 2015-2023 Nautech Systems Pty Ltd. All rights reserved.
-//  https://nautechsystems.io
-//
-//  Licensed under the GNU Lesser General Public License Version 3.0 (the "License");
-//  You may not use this file except in compliance with the License.
-//  You may obtain a copy of the License at https://www.gnu.org/licenses/lgpl-3.0.en.html
-//
-//  Unless required by applicable law or agreed to in writing, software
-//  distributed under the License is distributed on an "AS IS" BASIS,
-//  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-//  See the License for the specific language governing permissions and
-//  limitations under the License.
-// -------------------------------------------------------------------------------------------------
-
-pub mod bar;
-pub mod tick;
+# -------------------------------------------------------------------------------------------------
+#  Copyright (C) 2015-2023 Nautech Systems Pty Ltd. All rights reserved.
+#  https://nautechsystems.io
+#
+#  Licensed under the GNU Lesser General Public License Version 3.0 (the "License");
+#  You may not use this file except in compliance with the License.
+#  You may obtain a copy of the License at https://www.gnu.org/licenses/lgpl-3.0.en.html
+#
+#  Unless required by applicable law or agreed to in writing, software
+#  distributed under the License is distributed on an "AS IS" BASIS,
+#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#  See the License for the specific language governing permissions and
+#  limitations under the License.
+# -------------------------------------------------------------------------------------------------
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/model/src/data/tick.rs` & `nautilus_trader-1.174.0/nautilus_core/model/src/data/tick.rs`

 * *Files 4% similar despite different names*

```diff
@@ -11,27 +11,29 @@
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
 use std::cmp;
 use std::ffi::c_char;
-use std::fmt::{Display, Formatter, Result};
+use std::fmt::{Display, Formatter};
 
 use nautilus_core::correctness;
 use nautilus_core::string::string_to_cstr;
 use nautilus_core::time::UnixNanos;
 
 use crate::enums::{AggressorSide, PriceType};
 use crate::identifiers::instrument_id::InstrumentId;
 use crate::identifiers::trade_id::TradeId;
 use crate::types::fixed::FIXED_PRECISION;
 use crate::types::price::Price;
 use crate::types::quantity::Quantity;
 
+use super::Data;
+
 /// Represents a single quote tick in a financial market.
 #[repr(C)]
 #[derive(Clone, Debug, PartialEq, Eq, Hash)]
 pub struct QuoteTick {
     pub instrument_id: InstrumentId,
     pub bid: Price,
     pub ask: Price,
@@ -60,40 +62,41 @@
         );
         correctness::u8_equal(
             bid_size.precision,
             ask_size.precision,
             "bid_size.precision",
             "ask_size.precision",
         );
-        QuoteTick {
+        Self {
             instrument_id,
             bid,
             ask,
             bid_size,
             ask_size,
             ts_event,
             ts_init,
         }
     }
 
+    #[must_use]
     pub fn extract_price(&self, price_type: PriceType) -> Price {
         match price_type {
             PriceType::Bid => self.bid.clone(),
             PriceType::Ask => self.ask.clone(),
             PriceType::Mid => Price::from_raw(
                 (self.bid.raw + self.ask.raw) / 2,
                 cmp::min(self.bid.precision + 1, FIXED_PRECISION),
             ),
             _ => panic!("Cannot extract with price type {price_type}"),
         }
     }
 }
 
 impl Display for QuoteTick {
-    fn fmt(&self, f: &mut Formatter<'_>) -> Result {
+    fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         write!(
             f,
             "{},{},{},{},{},{}",
             self.instrument_id, self.bid, self.ask, self.bid_size, self.ask_size, self.ts_event,
         )
     }
 }
@@ -118,69 +121,41 @@
         price: Price,
         size: Quantity,
         aggressor_side: AggressorSide,
         trade_id: TradeId,
         ts_event: UnixNanos,
         ts_init: UnixNanos,
     ) -> Self {
-        TradeTick {
+        Self {
             instrument_id,
             price,
             size,
             aggressor_side,
             trade_id,
             ts_event,
             ts_init,
         }
     }
 }
 
 impl Display for TradeTick {
-    fn fmt(&self, f: &mut Formatter<'_>) -> Result {
+    fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         write!(
             f,
             "{},{},{},{},{},{}",
             self.instrument_id,
             self.price,
             self.size,
             self.aggressor_side,
             self.trade_id,
             self.ts_event,
         )
     }
 }
 
-#[repr(C)]
-#[derive(Debug, Clone)]
-pub enum Data {
-    Trade(TradeTick),
-    Quote(QuoteTick),
-}
-
-impl Data {
-    pub fn get_ts_init(&self) -> UnixNanos {
-        match self {
-            Data::Trade(t) => t.ts_init,
-            Data::Quote(q) => q.ts_init,
-        }
-    }
-}
-
-impl From<QuoteTick> for Data {
-    fn from(value: QuoteTick) -> Self {
-        Self::Quote(value)
-    }
-}
-
-impl From<TradeTick> for Data {
-    fn from(value: TradeTick) -> Self {
-        Self::Trade(value)
-    }
-}
-
 ////////////////////////////////////////////////////////////////////////////////
 // C API
 ////////////////////////////////////////////////////////////////////////////////
 #[no_mangle]
 pub extern "C" fn quote_tick_drop(tick: QuoteTick) {
     drop(tick); // Memory freed here
 }
@@ -292,27 +267,29 @@
 }
 
 ////////////////////////////////////////////////////////////////////////////////
 // Tests
 ////////////////////////////////////////////////////////////////////////////////
 #[cfg(test)]
 mod tests {
+    use std::str::FromStr;
+
     use rstest::rstest;
 
     use crate::data::tick::{QuoteTick, TradeTick};
     use crate::enums::{AggressorSide, PriceType};
     use crate::identifiers::instrument_id::InstrumentId;
     use crate::identifiers::trade_id::TradeId;
     use crate::types::price::Price;
     use crate::types::quantity::Quantity;
 
     #[test]
     fn test_quote_tick_to_string() {
         let tick = QuoteTick {
-            instrument_id: InstrumentId::from("ETHUSDT-PERP.BINANCE"),
+            instrument_id: InstrumentId::from_str("ETHUSDT-PERP.BINANCE").unwrap(),
             bid: Price::new(10000.0, 4),
             ask: Price::new(10001.0, 4),
             bid_size: Quantity::new(1.0, 8),
             ask_size: Quantity::new(1.0, 8),
             ts_event: 0,
             ts_init: 0,
         };
@@ -321,21 +298,21 @@
             "ETHUSDT-PERP.BINANCE,10000.0000,10001.0000,1.00000000,1.00000000,0"
         );
     }
 
     #[rstest(
         input,
         expected,
-        case(PriceType::Bid, 10000000000000),
-        case(PriceType::Ask, 10001000000000),
-        case(PriceType::Mid, 10000500000000)
+        case(PriceType::Bid, 10_000_000_000_000),
+        case(PriceType::Ask, 10_001_000_000_000),
+        case(PriceType::Mid, 10_000_500_000_000)
     )]
     fn test_quote_tick_extract_price(input: PriceType, expected: i64) {
         let tick = QuoteTick {
-            instrument_id: InstrumentId::from("ETHUSDT-PERP.BINANCE"),
+            instrument_id: InstrumentId::from_str("ETHUSDT-PERP.BINANCE").unwrap(),
             bid: Price::new(10000.0, 4),
             ask: Price::new(10001.0, 4),
             bid_size: Quantity::new(1.0, 8),
             ask_size: Quantity::new(1.0, 8),
             ts_event: 0,
             ts_init: 0,
         };
@@ -343,15 +320,15 @@
         let result = tick.extract_price(input).raw;
         assert_eq!(result, expected);
     }
 
     #[test]
     fn test_trade_tick_to_string() {
         let tick = TradeTick {
-            instrument_id: InstrumentId::from("ETHUSDT-PERP.BINANCE"),
+            instrument_id: InstrumentId::from_str("ETHUSDT-PERP.BINANCE").unwrap(),
             price: Price::new(10000.0, 4),
             size: Quantity::new(1.0, 8),
             aggressor_side: AggressorSide::Buyer,
             trade_id: TradeId::new("123456789"),
             ts_event: 0,
             ts_init: 0,
         };
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/model/src/enums.rs` & `nautilus_trader-1.174.0/nautilus_core/model/src/enums.rs`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,20 @@
 use std::fmt::Debug;
 use std::str::FromStr;
 
 use nautilus_core::string::{cstr_to_string, string_to_cstr};
 use pyo3::prelude::*;
 use strum::{Display, EnumString, FromRepr};
 
+pub trait FromU8 {
+    fn from_u8(value: u8) -> Option<Self>
+    where
+        Self: Sized;
+}
+
 #[pyclass]
 #[repr(C)]
 #[derive(Copy, Clone, Debug, Hash, PartialEq, Eq, FromRepr, EnumString, Display)]
 #[strum(ascii_case_insensitive)]
 #[strum(serialize_all = "SCREAMING_SNAKE_CASE")]
 pub enum AccountType {
     Cash = 1,
@@ -118,14 +124,26 @@
 pub enum BookAction {
     Add = 1,
     Update = 2,
     Delete = 3,
     Clear = 4,
 }
 
+impl FromU8 for BookAction {
+    fn from_u8(value: u8) -> Option<Self> {
+        match value {
+            1 => Some(BookAction::Add),
+            2 => Some(BookAction::Update),
+            3 => Some(BookAction::Delete),
+            4 => Some(BookAction::Clear),
+            _ => None,
+        }
+    }
+}
+
 #[pyclass]
 #[repr(C)]
 #[derive(Copy, Clone, Debug, Hash, PartialEq, Eq, FromRepr, EnumString, Display)]
 #[strum(ascii_case_insensitive)]
 #[strum(serialize_all = "SCREAMING_SNAKE_CASE")]
 #[allow(non_camel_case_types)]
 pub enum BookType {
@@ -133,14 +151,25 @@
     L1_TBBO = 1,
     /// Market by price.
     L2_MBP = 2,
     /// Market by order.
     L3_MBO = 3,
 }
 
+impl FromU8 for BookType {
+    fn from_u8(value: u8) -> Option<Self> {
+        match value {
+            1 => Some(BookType::L1_TBBO),
+            2 => Some(BookType::L2_MBP),
+            3 => Some(BookType::L3_MBO),
+            _ => None,
+        }
+    }
+}
+
 #[pyclass]
 #[repr(C)]
 #[derive(Copy, Clone, Debug, Hash, PartialEq, Eq, FromRepr, EnumString, Display)]
 #[strum(ascii_case_insensitive)]
 #[strum(serialize_all = "SCREAMING_SNAKE_CASE")]
 pub enum ContingencyType {
     NoContingency = 0, // Will be replaced by `Option`
@@ -233,14 +262,25 @@
 #[allow(clippy::enum_variant_names)]
 pub enum OrderSide {
     NoOrderSide = 0, // Will be replaced by `Option`
     Buy = 1,
     Sell = 2,
 }
 
+impl FromU8 for OrderSide {
+    fn from_u8(value: u8) -> Option<Self> {
+        match value {
+            0 => Some(OrderSide::NoOrderSide),
+            1 => Some(OrderSide::Buy),
+            2 => Some(OrderSide::Sell),
+            _ => None,
+        }
+    }
+}
+
 #[pyclass]
 #[repr(C)]
 #[derive(Copy, Clone, Debug, Hash, PartialEq, Eq, FromRepr, EnumString, Display)]
 #[strum(ascii_case_insensitive)]
 #[strum(serialize_all = "SCREAMING_SNAKE_CASE")]
 pub enum OrderStatus {
     Initialized = 1,
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/model/src/events/mod.rs` & `nautilus_trader-1.174.0/nautilus_core/model/src/events/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_core/model/src/events/order.rs` & `nautilus_trader-1.174.0/nautilus_core/model/src/events/order.rs`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
 use std::ops::Deref;
 use std::rc::Rc;
+use std::str::FromStr;
 
 use derive_builder::{self, Builder};
 use nautilus_core::time::UnixNanos;
 use nautilus_core::uuid::UUID4;
 
 use crate::enums::{
     ContingencyType, LiquiditySide, OrderSide, OrderType, TimeInForce, TriggerType,
@@ -67,15 +68,15 @@
 }
 
 impl Default for OrderIdentifiers {
     fn default() -> Self {
         Self {
             trader_id: TraderId::new("TRADER-001"),
             strategy_id: StrategyId::new("S-001"),
-            instrument_id: InstrumentId::from("AUD/USD.SIM"),
+            instrument_id: InstrumentId::from_str("AUD/USD.SIM").unwrap(),
             client_order_id: ClientOrderId::new("O-123456789"),
         }
     }
 }
 
 #[repr(C)]
 #[derive(Clone, Hash, PartialEq, Eq, Debug, Builder)]
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/model/src/events/position.rs` & `nautilus_trader-1.174.0/nautilus_core/model/src/events/position.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_core/model/src/identifiers/account_id.rs` & `nautilus_trader-1.174.0/nautilus_core/model/src/identifiers/account_id.rs`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
 use std::collections::hash_map::DefaultHasher;
 use std::ffi::{c_char, CStr};
-use std::fmt::{Debug, Display, Formatter, Result};
+use std::fmt::{Debug, Display, Formatter};
 use std::hash::{Hash, Hasher};
 use std::rc::Rc;
 
 use nautilus_core::correctness;
 use nautilus_core::string::string_to_cstr;
 
 #[repr(C)]
@@ -27,34 +27,34 @@
 #[allow(clippy::box_collection)] // C ABI compatibility
 #[allow(clippy::redundant_allocation)] // C ABI compatibility
 pub struct AccountId {
     pub value: Box<Rc<String>>,
 }
 
 impl Display for AccountId {
-    fn fmt(&self, f: &mut Formatter<'_>) -> Result {
+    fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         write!(f, "{}", self.value)
     }
 }
 
 impl AccountId {
     #[must_use]
     pub fn new(s: &str) -> Self {
         correctness::valid_string(s, "`AccountId` value");
         correctness::string_contains(s, "-", "`TraderId` value");
 
-        AccountId {
+        Self {
             value: Box::new(Rc::new(s.to_string())),
         }
     }
 }
 
 impl Default for AccountId {
     fn default() -> Self {
-        AccountId {
+        Self {
             value: Box::new(Rc::new(String::from("SIM-001"))),
         }
     }
 }
 
 ////////////////////////////////////////////////////////////////////////////////
 // C API
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/model/src/identifiers/client_id.rs` & `nautilus_trader-1.174.0/nautilus_core/model/src/identifiers/client_id.rs`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
 use std::collections::hash_map::DefaultHasher;
 use std::ffi::{c_char, CStr};
-use std::fmt::{Debug, Display, Formatter, Result};
+use std::fmt::{Debug, Display, Formatter};
 use std::hash::{Hash, Hasher};
 use std::rc::Rc;
 
 use nautilus_core::correctness;
 use nautilus_core::string::string_to_cstr;
 
 #[repr(C)]
@@ -27,25 +27,25 @@
 #[allow(clippy::box_collection)] // C ABI compatibility
 #[allow(clippy::redundant_allocation)] // C ABI compatibility
 pub struct ClientId {
     pub value: Box<Rc<String>>,
 }
 
 impl Display for ClientId {
-    fn fmt(&self, f: &mut Formatter<'_>) -> Result {
+    fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         write!(f, "{}", self.value)
     }
 }
 
 impl ClientId {
     #[must_use]
     pub fn new(s: &str) -> Self {
         correctness::valid_string(s, "`ClientId` value");
 
-        ClientId {
+        Self {
             value: Box::new(Rc::new(s.to_string())),
         }
     }
 }
 
 ////////////////////////////////////////////////////////////////////////////////
 // C API
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/model/src/identifiers/client_order_id.rs` & `nautilus_trader-1.174.0/nautilus_core/model/src/identifiers/client_order_id.rs`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
 use std::collections::hash_map::DefaultHasher;
 use std::ffi::{c_char, CStr};
-use std::fmt::{Debug, Display, Formatter, Result};
+use std::fmt::{Debug, Display, Formatter};
 use std::hash::{Hash, Hasher};
 use std::rc::Rc;
 
 use nautilus_core::correctness;
 use nautilus_core::string::string_to_cstr;
 
 #[repr(C)]
@@ -27,25 +27,25 @@
 #[allow(clippy::box_collection)] // C ABI compatibility
 #[allow(clippy::redundant_allocation)] // C ABI compatibility
 pub struct ClientOrderId {
     pub value: Box<Rc<String>>,
 }
 
 impl Display for ClientOrderId {
-    fn fmt(&self, f: &mut Formatter<'_>) -> Result {
+    fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         write!(f, "{}", self.value)
     }
 }
 
 impl ClientOrderId {
     #[must_use]
     pub fn new(s: &str) -> Self {
         correctness::valid_string(s, "`ClientOrderId` value");
 
-        ClientOrderId {
+        Self {
             value: Box::new(Rc::new(s.to_string())),
         }
     }
 }
 
 ////////////////////////////////////////////////////////////////////////////////
 // C API
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/model/src/identifiers/component_id.rs` & `nautilus_trader-1.174.0/nautilus_core/model/src/identifiers/component_id.rs`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
 use std::collections::hash_map::DefaultHasher;
 use std::ffi::{c_char, CStr};
-use std::fmt::{Debug, Display, Formatter, Result};
+use std::fmt::{Debug, Display, Formatter};
 use std::hash::{Hash, Hasher};
 use std::rc::Rc;
 
 use nautilus_core::correctness;
 use nautilus_core::string::string_to_cstr;
 
 #[repr(C)]
@@ -27,25 +27,25 @@
 #[allow(clippy::box_collection)] // C ABI compatibility
 #[allow(clippy::redundant_allocation)] // C ABI compatibility
 pub struct ComponentId {
     pub value: Box<Rc<String>>,
 }
 
 impl Display for ComponentId {
-    fn fmt(&self, f: &mut Formatter<'_>) -> Result {
+    fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         write!(f, "{}", self.value)
     }
 }
 
 impl ComponentId {
     #[must_use]
     pub fn new(s: &str) -> Self {
         correctness::valid_string(s, "`ComponentId` value");
 
-        ComponentId {
+        Self {
             value: Box::new(Rc::new(s.to_string())),
         }
     }
 }
 
 ////////////////////////////////////////////////////////////////////////////////
 // C API
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/model/src/identifiers/exec_algorithm_id.rs` & `nautilus_trader-1.174.0/nautilus_core/model/src/identifiers/exec_algorithm_id.rs`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
 use std::collections::hash_map::DefaultHasher;
 use std::ffi::{c_char, CStr};
-use std::fmt::{Debug, Display, Formatter, Result};
+use std::fmt::{Debug, Display, Formatter};
 use std::hash::{Hash, Hasher};
 use std::rc::Rc;
 
 use nautilus_core::correctness;
 use nautilus_core::string::string_to_cstr;
 
 #[repr(C)]
@@ -27,25 +27,25 @@
 #[allow(clippy::box_collection)] // C ABI compatibility
 #[allow(clippy::redundant_allocation)] // C ABI compatibility
 pub struct ExecAlgorithmId {
     pub value: Box<Rc<String>>,
 }
 
 impl Display for ExecAlgorithmId {
-    fn fmt(&self, f: &mut Formatter<'_>) -> Result {
+    fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         write!(f, "{}", self.value)
     }
 }
 
 impl ExecAlgorithmId {
     #[must_use]
     pub fn new(s: &str) -> Self {
         correctness::valid_string(s, "`ExecAlgorithmId` value");
 
-        ExecAlgorithmId {
+        Self {
             value: Box::new(Rc::new(s.to_string())),
         }
     }
 }
 
 ////////////////////////////////////////////////////////////////////////////////
 // C API
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/model/src/identifiers/instrument_id.rs` & `nautilus_trader-1.174.0/nautilus_core/model/src/identifiers/instrument_id.rs`

 * *Files 21% similar despite different names*

```diff
@@ -11,50 +11,64 @@
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
 use std::collections::hash_map::DefaultHasher;
 use std::ffi::c_char;
-use std::fmt::{Debug, Display, Formatter, Result};
+use std::fmt::{Debug, Display, Formatter};
 use std::hash::{Hash, Hasher};
+use std::str::FromStr;
 
 use nautilus_core::string::{cstr_to_string, string_to_cstr};
+use thiserror::Error;
 
 use crate::identifiers::symbol::Symbol;
 use crate::identifiers::venue::Venue;
 
 #[repr(C)]
 #[derive(Clone, Hash, PartialEq, Eq, Debug)]
 #[allow(clippy::box_collection)] // C ABI compatibility
 pub struct InstrumentId {
     pub symbol: Symbol,
     pub venue: Venue,
 }
 
-impl From<&str> for InstrumentId {
-    fn from(s: &str) -> Self {
-        let pieces = s.rsplit_once('.').expect("rsplit_once failed");
-        InstrumentId {
-            symbol: Symbol::new(pieces.0),
-            venue: Venue::new(pieces.1),
+#[derive(Debug, Error)]
+#[error("Error parsing `InstrumentId` from '{input}'")]
+pub struct InstrumentIdParseError {
+    input: String,
+}
+
+impl FromStr for InstrumentId {
+    type Err = InstrumentIdParseError;
+
+    fn from_str(s: &str) -> Result<Self, Self::Err> {
+        match s.rsplit_once('.') {
+            Some((symbol_part, venue_part)) => Ok(Self {
+                symbol: Symbol::new(symbol_part),
+                venue: Venue::new(venue_part),
+            }),
+            None => Err(InstrumentIdParseError {
+                input: s.to_string(),
+            }),
         }
     }
 }
 
 impl Display for InstrumentId {
-    fn fmt(&self, f: &mut Formatter<'_>) -> Result {
+    fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         write!(f, "{}.{}", self.symbol, self.venue)
     }
 }
 
 impl InstrumentId {
     #[must_use]
     pub fn new(symbol: Symbol, venue: Venue) -> Self {
-        InstrumentId { symbol, venue }
+        Self { symbol, venue }
     }
 }
 
 ////////////////////////////////////////////////////////////////////////////////
 // C API
 ////////////////////////////////////////////////////////////////////////////////
 #[no_mangle]
@@ -66,15 +80,15 @@
 
 /// Returns a Nautilus identifier from a C string pointer.
 ///
 /// # Safety
 /// - Assumes `ptr` is a valid C string pointer.
 #[no_mangle]
 pub unsafe extern "C" fn instrument_id_new_from_cstr(ptr: *const c_char) -> InstrumentId {
-    InstrumentId::from(cstr_to_string(ptr).as_str())
+    InstrumentId::from_str(cstr_to_string(ptr).as_str()).unwrap()
 }
 
 #[no_mangle]
 pub extern "C" fn instrument_id_clone(instrument_id: &InstrumentId) -> InstrumentId {
     instrument_id.clone()
 }
 
@@ -103,43 +117,79 @@
 }
 
 ////////////////////////////////////////////////////////////////////////////////
 // Tests
 ////////////////////////////////////////////////////////////////////////////////
 #[cfg(test)]
 mod tests {
-    use std::ffi::CStr;
+    use std::{ffi::CStr, str::FromStr};
 
     use super::InstrumentId;
-    use crate::identifiers::instrument_id::{instrument_id_drop, instrument_id_to_cstr};
+    use crate::identifiers::instrument_id::{
+        instrument_id_drop, instrument_id_to_cstr, InstrumentIdParseError,
+    };
+
+    #[test]
+    fn test_instrument_id_parse_success() {
+        let instrument_id = InstrumentId::from_str("ETH/USDT.BINANCE").unwrap();
+        assert_eq!(instrument_id.symbol.to_string(), "ETH/USDT");
+        assert_eq!(instrument_id.venue.to_string(), "BINANCE");
+    }
+
+    #[test]
+    fn test_instrument_id_parse_failure_no_dot() {
+        let result = InstrumentId::from_str("ETHUSDT-BINANCE");
+        assert!(result.is_err());
+
+        let error = result.unwrap_err();
+        assert!(matches!(error, InstrumentIdParseError { .. }));
+        assert_eq!(
+            error.to_string(),
+            "Error parsing `InstrumentId` from 'ETHUSDT-BINANCE'"
+        );
+    }
+
+    #[ignore] // Cannot implement yet due Betfair instrument IDs
+    #[test]
+    fn test_instrument_id_parse_failure_multiple_dots() {
+        let result = InstrumentId::from_str("ETH.USDT.BINANCE");
+        assert!(result.is_err());
+
+        let error = result.unwrap_err();
+        assert!(matches!(error, InstrumentIdParseError { .. }));
+        assert_eq!(
+            error.to_string(),
+            "Error parsing `InstrumentId` from 'ETH.USDT.BINANCE'"
+        );
+    }
 
     #[test]
     fn test_equality() {
-        let id1 = InstrumentId::from("ETH/USDT.BINANCE");
-        let id2 = InstrumentId::from("XBT/USD.BITMEX");
+        let id1 = InstrumentId::from_str("ETH/USDT.BINANCE").unwrap();
+        let id2 = InstrumentId::from_str("XBT/USD.BITMEX").unwrap();
         assert_eq!(id1, id1);
         assert_ne!(id1, id2);
     }
 
     #[test]
     fn test_string_reprs() {
-        let id = InstrumentId::from("ETH/USDT.BINANCE");
+        let id = InstrumentId::from_str("ETH/USDT.BINANCE").unwrap();
         assert_eq!(id.to_string(), "ETH/USDT.BINANCE");
         assert_eq!(format!("{id}"), "ETH/USDT.BINANCE");
     }
 
     #[test]
     fn test_to_cstr() {
         unsafe {
-            let id = InstrumentId::from("ETH/USDT.BINANCE");
+            let id = InstrumentId::from_str("ETH/USDT.BINANCE").unwrap();
             let result = instrument_id_to_cstr(&id);
             assert_eq!(CStr::from_ptr(result).to_str().unwrap(), "ETH/USDT.BINANCE");
         }
     }
 
     #[test]
     fn test_instrument_id_drop() {
-        let id = InstrumentId::from("ETH/USDT.BINANCE");
+        let id = InstrumentId::from_str("ETH/USDT.BINANCE").unwrap();
 
         instrument_id_drop(id); // No panic
     }
 }
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/model/src/identifiers/mod.rs` & `nautilus_trader-1.174.0/nautilus_core/model/src/identifiers/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_core/model/src/identifiers/order_list_id.rs` & `nautilus_trader-1.174.0/nautilus_core/model/src/identifiers/order_list_id.rs`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
 use std::collections::hash_map::DefaultHasher;
 use std::ffi::{c_char, CStr};
-use std::fmt::{Debug, Display, Formatter, Result};
+use std::fmt::{Debug, Display, Formatter};
 use std::hash::{Hash, Hasher};
 use std::rc::Rc;
 
 use nautilus_core::correctness;
 use nautilus_core::string::string_to_cstr;
 
 #[repr(C)]
@@ -27,25 +27,25 @@
 #[allow(clippy::box_collection)] // C ABI compatibility
 #[allow(clippy::redundant_allocation)] // C ABI compatibility
 pub struct OrderListId {
     pub value: Box<Rc<String>>,
 }
 
 impl Display for OrderListId {
-    fn fmt(&self, f: &mut Formatter<'_>) -> Result {
+    fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         write!(f, "{}", self.value)
     }
 }
 
 impl OrderListId {
     #[must_use]
     pub fn new(s: &str) -> Self {
         correctness::valid_string(s, "`OrderListId` value");
 
-        OrderListId {
+        Self {
             value: Box::new(Rc::new(s.to_string())),
         }
     }
 }
 
 ////////////////////////////////////////////////////////////////////////////////
 // C API
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/model/src/identifiers/position_id.rs` & `nautilus_trader-1.174.0/nautilus_core/model/src/identifiers/position_id.rs`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
 use std::collections::hash_map::DefaultHasher;
 use std::ffi::{c_char, CStr};
-use std::fmt::{Debug, Display, Formatter, Result};
+use std::fmt::{Debug, Display, Formatter};
 use std::hash::{Hash, Hasher};
 use std::rc::Rc;
 
 use nautilus_core::correctness;
 use nautilus_core::string::string_to_cstr;
 
 #[repr(C)]
@@ -27,25 +27,25 @@
 #[allow(clippy::box_collection)] // C ABI compatibility
 #[allow(clippy::redundant_allocation)] // C ABI compatibility
 pub struct PositionId {
     pub value: Box<Rc<String>>,
 }
 
 impl Display for PositionId {
-    fn fmt(&self, f: &mut Formatter<'_>) -> Result {
+    fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         write!(f, "{}", self.value)
     }
 }
 
 impl PositionId {
     #[must_use]
     pub fn new(s: &str) -> Self {
         correctness::valid_string(s, "`PositionId` value");
 
-        PositionId {
+        Self {
             value: Box::new(Rc::new(s.to_string())),
         }
     }
 }
 
 ////////////////////////////////////////////////////////////////////////////////
 // C API
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/model/src/identifiers/strategy_id.rs` & `nautilus_trader-1.174.0/nautilus_core/model/src/identifiers/strategy_id.rs`

 * *Files 3% similar despite different names*

```diff
@@ -10,43 +10,43 @@
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
 use std::ffi::{c_char, CStr};
-use std::fmt::{Debug, Display, Formatter, Result};
+use std::fmt::{Debug, Display, Formatter};
 use std::rc::Rc;
 
 use nautilus_core::correctness;
 use nautilus_core::string::string_to_cstr;
 
 #[repr(C)]
 #[derive(Clone, Hash, PartialEq, Eq, Debug)]
 #[allow(clippy::box_collection)] // C ABI compatibility
 #[allow(clippy::redundant_allocation)] // C ABI compatibility
 pub struct StrategyId {
     pub value: Box<Rc<String>>,
 }
 
 impl Display for StrategyId {
-    fn fmt(&self, f: &mut Formatter<'_>) -> Result {
+    fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         write!(f, "{}", self.value)
     }
 }
 
 impl StrategyId {
     #[must_use]
     pub fn new(s: &str) -> Self {
         correctness::valid_string(s, "`StrategyId` value");
         if s != "EXTERNAL" {
             correctness::string_contains(s, "-", "`StrategyId` value");
         }
 
-        StrategyId {
+        Self {
             value: Box::new(Rc::new(s.to_string())),
         }
     }
 }
 
 ////////////////////////////////////////////////////////////////////////////////
 // C API
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/model/src/identifiers/symbol.rs` & `nautilus_trader-1.174.0/nautilus_core/model/src/identifiers/symbol.rs`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
 use std::collections::hash_map::DefaultHasher;
 use std::ffi::{c_char, CStr};
-use std::fmt::{Debug, Display, Formatter, Result};
+use std::fmt::{Debug, Display, Formatter};
 use std::hash::{Hash, Hasher};
 use std::rc::Rc;
 
 use nautilus_core::correctness;
 use nautilus_core::string::string_to_cstr;
 
 #[repr(C)]
@@ -27,25 +27,25 @@
 #[allow(clippy::box_collection)] // C ABI compatibility
 #[allow(clippy::redundant_allocation)] // C ABI compatibility
 pub struct Symbol {
     pub value: Box<Rc<String>>,
 }
 
 impl Display for Symbol {
-    fn fmt(&self, f: &mut Formatter<'_>) -> Result {
+    fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         write!(f, "{}", self.value)
     }
 }
 
 impl Symbol {
     #[must_use]
     pub fn new(s: &str) -> Self {
         correctness::valid_string(s, "`Symbol` value");
 
-        Symbol {
+        Self {
             value: Box::new(Rc::new(s.to_string())),
         }
     }
 }
 
 ////////////////////////////////////////////////////////////////////////////////
 // C API
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/model/src/identifiers/trade_id.rs` & `nautilus_trader-1.174.0/nautilus_core/model/src/identifiers/trade_id.rs`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
 use std::collections::hash_map::DefaultHasher;
 use std::ffi::{c_char, CStr};
-use std::fmt::{Debug, Display, Formatter, Result};
+use std::fmt::{Debug, Display, Formatter};
 use std::hash::{Hash, Hasher};
 use std::rc::Rc;
 
 use nautilus_core::correctness;
 use nautilus_core::string::string_to_cstr;
 
 #[repr(C)]
@@ -27,25 +27,25 @@
 #[allow(clippy::box_collection)] // C ABI compatibility
 #[allow(clippy::redundant_allocation)] // C ABI compatibility
 pub struct TradeId {
     pub value: Box<Rc<String>>,
 }
 
 impl Display for TradeId {
-    fn fmt(&self, f: &mut Formatter<'_>) -> Result {
+    fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         write!(f, "{}", self.value)
     }
 }
 
 impl TradeId {
     #[must_use]
     pub fn new(s: &str) -> Self {
         correctness::valid_string(s, "`TradeId` value");
 
-        TradeId {
+        Self {
             value: Box::new(Rc::new(s.to_string())),
         }
     }
 }
 
 ////////////////////////////////////////////////////////////////////////////////
 // C API
@@ -66,15 +66,15 @@
 
 /// Frees the memory for the given `trade_id` by dropping.
 #[no_mangle]
 pub extern "C" fn trade_id_drop(trade_id: TradeId) {
     drop(trade_id); // Memory freed here
 }
 
-/// Returns [TradeId] as a C string pointer.
+/// Returns [`TradeId`] as a C string pointer.
 #[no_mangle]
 pub extern "C" fn trade_id_to_cstr(trade_id: &TradeId) -> *const c_char {
     string_to_cstr(&trade_id.value)
 }
 
 #[no_mangle]
 pub extern "C" fn trade_id_eq(lhs: &TradeId, rhs: &TradeId) -> u8 {
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/model/src/identifiers/trader_id.rs` & `nautilus_trader-1.174.0/nautilus_core/model/src/identifiers/trader_id.rs`

 * *Files 2% similar despite different names*

```diff
@@ -10,41 +10,41 @@
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
 use std::ffi::{c_char, CStr};
-use std::fmt::{Debug, Display, Formatter, Result};
+use std::fmt::{Debug, Display, Formatter};
 use std::rc::Rc;
 
 use nautilus_core::correctness;
 use nautilus_core::string::string_to_cstr;
 
 #[repr(C)]
 #[derive(Clone, Hash, PartialEq, Eq, Debug)]
 #[allow(clippy::box_collection)] // C ABI compatibility
 #[allow(clippy::redundant_allocation)] // C ABI compatibility
 pub struct TraderId {
     pub value: Box<Rc<String>>,
 }
 
 impl Display for TraderId {
-    fn fmt(&self, f: &mut Formatter<'_>) -> Result {
+    fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         write!(f, "{}", self.value)
     }
 }
 
 impl TraderId {
     #[must_use]
     pub fn new(s: &str) -> Self {
         correctness::valid_string(s, "`TraderId` value");
         correctness::string_contains(s, "-", "`TraderId` value");
 
-        TraderId {
+        Self {
             value: Box::new(Rc::new(s.to_string())),
         }
     }
 }
 
 ////////////////////////////////////////////////////////////////////////////////
 // C API
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/model/src/identifiers/venue.rs` & `nautilus_trader-1.174.0/nautilus_core/model/src/identifiers/venue.rs`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
 use std::collections::hash_map::DefaultHasher;
 use std::ffi::{c_char, CStr};
-use std::fmt::{Debug, Display, Formatter, Result};
+use std::fmt::{Debug, Display, Formatter};
 use std::hash::{Hash, Hasher};
 use std::rc::Rc;
 
 use nautilus_core::correctness;
 use nautilus_core::string::string_to_cstr;
 
 #[repr(C)]
@@ -27,25 +27,25 @@
 #[allow(clippy::box_collection)] // C ABI compatibility
 #[allow(clippy::redundant_allocation)] // C ABI compatibility
 pub struct Venue {
     pub value: Box<Rc<String>>,
 }
 
 impl Display for Venue {
-    fn fmt(&self, f: &mut Formatter<'_>) -> Result {
+    fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         write!(f, "{}", self.value)
     }
 }
 
 impl Venue {
     #[must_use]
     pub fn new(s: &str) -> Self {
         correctness::valid_string(s, "`Venue` value");
 
-        Venue {
+        Self {
             value: Box::new(Rc::new(s.to_string())),
         }
     }
 }
 
 ////////////////////////////////////////////////////////////////////////////////
 // C API
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/model/src/identifiers/venue_order_id.rs` & `nautilus_trader-1.174.0/nautilus_core/model/src/identifiers/venue_order_id.rs`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
 use std::collections::hash_map::DefaultHasher;
 use std::ffi::{c_char, CStr};
-use std::fmt::{Debug, Display, Formatter, Result};
+use std::fmt::{Debug, Display, Formatter};
 use std::hash::{Hash, Hasher};
 use std::rc::Rc;
 
 use nautilus_core::correctness;
 use nautilus_core::string::string_to_cstr;
 
 #[repr(C)]
@@ -27,33 +27,33 @@
 #[allow(clippy::box_collection)] // C ABI compatibility
 #[allow(clippy::redundant_allocation)] // C ABI compatibility
 pub struct VenueOrderId {
     pub value: Box<Rc<String>>,
 }
 
 impl Display for VenueOrderId {
-    fn fmt(&self, f: &mut Formatter<'_>) -> Result {
+    fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         write!(f, "{}", self.value)
     }
 }
 
 impl VenueOrderId {
     #[must_use]
     pub fn new(s: &str) -> Self {
         correctness::valid_string(s, "`VenueOrderId` value");
 
-        VenueOrderId {
+        Self {
             value: Box::new(Rc::new(s.to_string())),
         }
     }
 }
 
 impl Default for VenueOrderId {
     fn default() -> Self {
-        VenueOrderId {
+        Self {
             value: Box::new(Rc::new(String::from("001"))),
         }
     }
 }
 
 ////////////////////////////////////////////////////////////////////////////////
 // C API
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/model/src/instruments/mod.rs` & `nautilus_trader-1.174.0/nautilus_core/model/src/instruments/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_core/model/src/lib.rs` & `nautilus_trader-1.174.0/nautilus_core/model/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_core/model/src/orderbook/book.rs` & `nautilus_trader-1.174.0/nautilus_core/model/src/orderbook/book.rs`

 * *Files 22% similar despite different names*

```diff
@@ -9,33 +9,34 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
+use std::ops::{Deref, DerefMut};
+
+use crate::data::book::BookOrder;
 use crate::enums::{BookType, OrderSide};
 use crate::identifiers::instrument_id::InstrumentId;
 use crate::orderbook::ladder::Ladder;
-use crate::orderbook::order::BookOrder;
 
-#[repr(C)]
 pub struct OrderBook {
     bids: Ladder,
     asks: Ladder,
     pub instrument_id: InstrumentId,
     pub book_level: BookType,
     pub last_side: OrderSide,
     pub ts_last: u64,
 }
 
 impl OrderBook {
     #[must_use]
     pub fn new(instrument_id: InstrumentId, book_level: BookType) -> Self {
-        OrderBook {
+        Self {
             bids: Ladder::new(OrderSide::Buy),
             asks: Ladder::new(OrderSide::Sell),
             instrument_id,
             book_level,
             last_side: OrderSide::Buy,
             ts_last: 0,
         }
@@ -43,43 +44,64 @@
 
     pub fn add(&mut self, order: BookOrder, ts_event: u64) {
         self.last_side = order.side;
         self.ts_last = ts_event;
         match order.side {
             OrderSide::Buy => self.bids.add(order),
             OrderSide::Sell => self.asks.add(order),
-            _ => panic!("`OrderSide` was None"),
+            _ => panic!("Invalid `OrderSide` {}", order.side),
         }
     }
 
     pub fn update(&mut self, order: BookOrder, ts_event: u64) {
         self.last_side = order.side;
         self.ts_last = ts_event;
         if order.size.raw == 0 {
             self.delete(order, ts_event);
         } else {
             match order.side {
                 OrderSide::Buy => self.bids.update(order),
                 OrderSide::Sell => self.asks.update(order),
-                _ => panic!("`OrderSide` was None"),
+                _ => panic!("Invalid `OrderSide` {}", order.side),
             }
         }
     }
 
     pub fn delete(&mut self, order: BookOrder, ts_event: u64) {
         self.last_side = order.side;
         self.ts_last = ts_event;
         match order.side {
             OrderSide::Buy => self.bids.delete(order),
             OrderSide::Sell => self.asks.delete(order),
-            _ => panic!("`OrderSide` was None"),
+            _ => panic!("Invalid `OrderSide` {}", order.side),
         }
     }
 }
 
 ////////////////////////////////////////////////////////////////////////////////
 // C API
 ////////////////////////////////////////////////////////////////////////////////
+#[allow(non_camel_case_types)]
+#[repr(C)]
+pub struct OrderBook_API(Box<OrderBook>);
+
+impl Deref for OrderBook_API {
+    type Target = OrderBook;
+
+    fn deref(&self) -> &Self::Target {
+        &self.0
+    }
+}
+
+impl DerefMut for OrderBook_API {
+    fn deref_mut(&mut self) -> &mut Self::Target {
+        &mut self.0
+    }
+}
+
 #[no_mangle]
-pub extern "C" fn order_book_new(instrument_id: InstrumentId, book_level: BookType) -> OrderBook {
-    OrderBook::new(instrument_id, book_level)
+pub extern "C" fn order_book_new(
+    instrument_id: InstrumentId,
+    book_type: BookType,
+) -> OrderBook_API {
+    OrderBook_API(Box::new(OrderBook::new(instrument_id, book_type)))
 }
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/model/src/orderbook/ladder.rs` & `nautilus_trader-1.174.0/nautilus_core/model/src/orderbook/ladder.rs`

 * *Files 2% similar despite different names*

```diff
@@ -12,39 +12,38 @@
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
 use std::cmp::Ordering;
 use std::collections::{BTreeMap, HashMap};
 
+use crate::data::book::BookOrder;
 use crate::enums::OrderSide;
 use crate::orderbook::level::Level;
-use crate::orderbook::order::BookOrder;
 use crate::types::price::Price;
 
-#[repr(C)]
 #[derive(Clone, Debug, Eq)]
 pub struct BookPrice {
     pub value: Price,
     pub side: OrderSide,
 }
 
 impl BookPrice {
     #[must_use]
     pub fn new(value: Price, side: OrderSide) -> Self {
-        BookPrice { value, side }
+        Self { value, side }
     }
 }
 
 impl PartialOrd for BookPrice {
     fn partial_cmp(&self, other: &Self) -> Option<Ordering> {
         match self.side {
             OrderSide::Buy => Some(other.value.cmp(&self.value)),
             OrderSide::Sell => Some(self.value.cmp(&other.value)),
-            _ => panic!("`OrderSide` was None"),
+            _ => panic!("Invalid `OrderSide` {}", self.side),
         }
     }
 }
 
 impl PartialEq for BookPrice {
     fn eq(&self, other: &Self) -> bool {
         self.value == other.value
@@ -52,41 +51,41 @@
 }
 
 impl Ord for BookPrice {
     fn cmp(&self, other: &Self) -> Ordering {
         match self.side {
             OrderSide::Buy => other.value.cmp(&self.value),
             OrderSide::Sell => self.value.cmp(&other.value),
-            _ => panic!("`OrderSide` was None"),
+            _ => panic!("Invalid `OrderSide` {}", self.side),
         }
     }
 }
 
-#[repr(C)]
-#[allow(clippy::box_collection)] // C ABI compatibility
 pub struct Ladder {
     pub side: OrderSide,
-    pub levels: Box<BTreeMap<BookPrice, Level>>,
-    pub cache: Box<HashMap<u64, BookPrice>>,
+    pub levels: BTreeMap<BookPrice, Level>,
+    pub cache: HashMap<u64, BookPrice>,
 }
 
 impl Ladder {
     #[must_use]
     pub fn new(side: OrderSide) -> Self {
-        Ladder {
+        Self {
             side,
-            levels: Box::<BTreeMap<BookPrice, Level>>::default(),
-            cache: Box::<HashMap<u64, BookPrice>>::default(),
+            levels: BTreeMap::new(),
+            cache: HashMap::new(),
         }
     }
 
+    #[must_use]
     pub fn len(&self) -> usize {
         self.levels.len()
     }
 
+    #[must_use]
     pub fn is_empty(&self) -> bool {
         self.levels.len() == 0
     }
 
     pub fn add_bulk(&mut self, orders: Vec<BookOrder>) {
         for order in orders {
             self.add(order)
@@ -137,38 +136,41 @@
                 if level.is_empty() {
                     self.levels.remove(&price);
                 }
             }
         }
     }
 
+    #[must_use]
     pub fn volumes(&self) -> f64 {
-        return self.levels.iter().map(|(_, l)| l.volume()).sum();
+        return self.levels.values().map(|l| l.volume()).sum();
     }
 
+    #[must_use]
     pub fn exposures(&self) -> f64 {
-        return self.levels.iter().map(|(_, l)| l.exposure()).sum();
+        return self.levels.values().map(|l| l.exposure()).sum();
     }
 
+    #[must_use]
     pub fn top(&self) -> Option<&Level> {
         match self.levels.iter().next() {
             None => Option::None,
             Some((_, l)) => Option::Some(l),
         }
     }
 }
 
 ////////////////////////////////////////////////////////////////////////////////
 // Tests
 ////////////////////////////////////////////////////////////////////////////////
 #[cfg(test)]
 mod tests {
+    use crate::data::book::BookOrder;
     use crate::enums::OrderSide;
     use crate::orderbook::ladder::{BookPrice, Ladder};
-    use crate::orderbook::order::BookOrder;
     use crate::types::price::Price;
     use crate::types::quantity::Quantity;
 
     #[test]
     fn test_book_price_bid_sorting() {
         let mut bid_prices = vec![
             BookPrice::new(Price::new(2.0, 0), OrderSide::Buy),
@@ -193,249 +195,249 @@
         assert_eq!(ask_prices[0].value.as_f64(), 1.0);
     }
 
     #[test]
     fn test_ladder_add_single_order() {
         let mut ladder = Ladder::new(OrderSide::Buy);
         let order = BookOrder::new(
+            OrderSide::Buy,
             Price::new(10.00, 2),
             Quantity::new(20.0, 0),
-            OrderSide::Buy,
             0,
         );
 
         ladder.add(order);
         assert_eq!(ladder.len(), 1);
         assert_eq!(ladder.volumes(), 20.0);
         assert_eq!(ladder.exposures(), 200.0);
         assert_eq!(ladder.top().unwrap().price.value.as_f64(), 10.0)
     }
 
     #[test]
     fn test_ladder_add_multiple_buy_orders() {
         let mut ladder = Ladder::new(OrderSide::Buy);
         let order1 = BookOrder::new(
+            OrderSide::Buy,
             Price::new(10.00, 2),
             Quantity::new(20.0, 0),
-            OrderSide::Buy,
             0,
         );
         let order2 = BookOrder::new(
+            OrderSide::Buy,
             Price::new(9.00, 2),
             Quantity::new(30.0, 0),
-            OrderSide::Buy,
             0,
         );
         let order3 = BookOrder::new(
+            OrderSide::Buy,
             Price::new(9.00, 2),
             Quantity::new(50.0, 0),
-            OrderSide::Buy,
             0,
         );
         let order4 = BookOrder::new(
+            OrderSide::Buy,
             Price::new(8.00, 2),
             Quantity::new(200.0, 0),
-            OrderSide::Buy,
             0,
         );
 
         ladder.add_bulk(vec![order1, order2, order3, order4]);
         assert_eq!(ladder.len(), 3);
         assert_eq!(ladder.volumes(), 300.0);
         assert_eq!(ladder.exposures(), 2520.0);
         assert_eq!(ladder.top().unwrap().price.value.as_f64(), 10.0)
     }
 
     #[test]
     fn test_ladder_add_multiple_sell_orders() {
         let mut ladder = Ladder::new(OrderSide::Sell);
         let order1 = BookOrder::new(
+            OrderSide::Sell,
             Price::new(11.00, 2),
             Quantity::new(20.0, 0),
-            OrderSide::Sell,
             0,
         );
         let order2 = BookOrder::new(
+            OrderSide::Sell,
             Price::new(12.00, 2),
             Quantity::new(30.0, 0),
-            OrderSide::Sell,
             0,
         );
         let order3 = BookOrder::new(
+            OrderSide::Sell,
             Price::new(12.00, 2),
             Quantity::new(50.0, 0),
-            OrderSide::Sell,
             0,
         );
         let order4 = BookOrder::new(
+            OrderSide::Sell,
             Price::new(13.00, 2),
             Quantity::new(200.0, 0),
-            OrderSide::Sell,
             0,
         );
 
         ladder.add_bulk(vec![order1, order2, order3, order4]);
         assert_eq!(ladder.len(), 3);
         assert_eq!(ladder.volumes(), 300.0);
         assert_eq!(ladder.exposures(), 3780.0);
         assert_eq!(ladder.top().unwrap().price.value.as_f64(), 11.0)
     }
 
     #[test]
     fn test_ladder_update_buy_order_price() {
         let mut ladder = Ladder::new(OrderSide::Buy);
         let order = BookOrder::new(
+            OrderSide::Buy,
             Price::new(11.00, 2),
             Quantity::new(20.0, 0),
-            OrderSide::Buy,
             1,
         );
 
         ladder.add(order);
 
         let order = BookOrder::new(
+            OrderSide::Buy,
             Price::new(11.10, 2),
             Quantity::new(20.0, 0),
-            OrderSide::Buy,
             1,
         );
 
         ladder.update(order);
         assert_eq!(ladder.len(), 1);
         assert_eq!(ladder.volumes(), 20.0);
-        assert_eq!(ladder.exposures(), 222.00000000000003);
+        assert_eq!(ladder.exposures(), 222.000_000_000_000_03);
         assert_eq!(
             ladder.top().unwrap().price.value.as_f64(),
-            11.100000000000001
+            11.100_000_000_000_001
         )
     }
 
     #[test]
     fn test_ladder_update_sell_order_price() {
         let mut ladder = Ladder::new(OrderSide::Sell);
         let order = BookOrder::new(
+            OrderSide::Sell,
             Price::new(11.00, 2),
             Quantity::new(20.0, 0),
-            OrderSide::Sell,
             1,
         );
 
         ladder.add(order);
 
         let order = BookOrder::new(
+            OrderSide::Sell,
             Price::new(11.10, 2),
             Quantity::new(20.0, 0),
-            OrderSide::Sell,
             1,
         );
 
         ladder.update(order);
         assert_eq!(ladder.len(), 1);
         assert_eq!(ladder.volumes(), 20.0);
-        assert_eq!(ladder.exposures(), 222.00000000000003);
+        assert_eq!(ladder.exposures(), 222.000_000_000_000_03);
         assert_eq!(
             ladder.top().unwrap().price.value.as_f64(),
-            11.100000000000001
+            11.100_000_000_000_001
         )
     }
 
     #[test]
     fn test_ladder_update_buy_order_size() {
         let mut ladder = Ladder::new(OrderSide::Buy);
         let order = BookOrder::new(
+            OrderSide::Buy,
             Price::new(11.00, 2),
             Quantity::new(20.0, 0),
-            OrderSide::Buy,
             1,
         );
 
         ladder.add(order);
 
         let order = BookOrder::new(
+            OrderSide::Buy,
             Price::new(11.00, 2),
             Quantity::new(10.0, 0),
-            OrderSide::Buy,
             1,
         );
 
         ladder.update(order);
         assert_eq!(ladder.len(), 1);
         assert_eq!(ladder.volumes(), 10.0);
         assert_eq!(ladder.exposures(), 110.0);
         assert_eq!(ladder.top().unwrap().price.value.as_f64(), 11.0)
     }
 
     #[test]
     fn test_ladder_update_sell_order_size() {
         let mut ladder = Ladder::new(OrderSide::Sell);
         let order = BookOrder::new(
+            OrderSide::Sell,
             Price::new(11.00, 2),
             Quantity::new(20.0, 0),
-            OrderSide::Sell,
             1,
         );
 
         ladder.add(order);
 
         let order = BookOrder::new(
+            OrderSide::Sell,
             Price::new(11.00, 2),
             Quantity::new(10.0, 0),
-            OrderSide::Sell,
             1,
         );
 
         ladder.update(order);
         assert_eq!(ladder.len(), 1);
         assert_eq!(ladder.volumes(), 10.0);
         assert_eq!(ladder.exposures(), 110.0);
         assert_eq!(ladder.top().unwrap().price.value.as_f64(), 11.0)
     }
 
     #[test]
     fn test_ladder_delete_buy_order() {
         let mut ladder = Ladder::new(OrderSide::Buy);
         let order = BookOrder::new(
+            OrderSide::Buy,
             Price::new(11.00, 2),
             Quantity::new(20.0, 0),
-            OrderSide::Buy,
             1,
         );
 
         ladder.add(order);
 
         let order = BookOrder::new(
+            OrderSide::Buy,
             Price::new(11.00, 2),
             Quantity::new(10.0, 0),
-            OrderSide::Buy,
             1,
         );
 
         ladder.delete(order);
         assert_eq!(ladder.len(), 0);
         assert_eq!(ladder.volumes(), 0.0);
         assert_eq!(ladder.exposures(), 0.0);
         assert_eq!(ladder.top(), None)
     }
 
     #[test]
     fn test_ladder_delete_sell_order() {
         let mut ladder = Ladder::new(OrderSide::Sell);
         let order = BookOrder::new(
+            OrderSide::Sell,
             Price::new(10.00, 2),
             Quantity::new(10.0, 0),
-            OrderSide::Sell,
             1,
         );
 
         ladder.add(order);
 
         let order = BookOrder::new(
+            OrderSide::Sell,
             Price::new(10.00, 2),
             Quantity::new(10.0, 0),
-            OrderSide::Sell,
             1,
         );
 
         ladder.delete(order);
         assert_eq!(ladder.len(), 0);
         assert_eq!(ladder.volumes(), 0.0);
         assert_eq!(ladder.exposures(), 0.0);
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/model/src/orderbook/level.rs` & `nautilus_trader-1.174.0/nautilus_core/model/src/orderbook/level.rs`

 * *Files 6% similar despite different names*

```diff
@@ -10,48 +10,49 @@
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
 use std::cmp::Ordering;
-use std::fmt::{Debug, Display, Formatter, Result};
+use std::fmt::{Debug, Display, Formatter};
 
+use crate::data::book::BookOrder;
 use crate::orderbook::ladder::BookPrice;
-use crate::orderbook::order::BookOrder;
 
-#[repr(C)]
-#[allow(clippy::box_collection)] // C ABI compatibility
 pub struct Level {
     pub price: BookPrice,
-    pub orders: Box<Vec<BookOrder>>,
+    pub orders: Vec<BookOrder>,
 }
 
 impl Level {
     #[must_use]
     pub fn new(price: BookPrice) -> Self {
-        Level {
+        Self {
             price,
-            orders: Box::<Vec<BookOrder>>::default(),
+            orders: Vec::new(),
         }
     }
 
+    #[must_use]
     pub fn from_order(order: BookOrder) -> Self {
-        let mut level = Level {
+        let mut level = Self {
             price: order.to_book_price(),
-            orders: Box::<Vec<BookOrder>>::default(),
+            orders: Vec::new(),
         };
         level.add(order);
         level
     }
 
+    #[must_use]
     pub fn len(&self) -> usize {
         self.orders.len()
     }
 
+    #[must_use]
     pub fn is_empty(&self) -> bool {
         self.orders.len() == 0
     }
 
     pub fn add_bulk(&mut self, orders: Vec<BookOrder>) {
         for order in orders {
             self.add(order)
@@ -84,22 +85,24 @@
             .orders
             .iter()
             .position(|o| o.order_id == order.order_id)
             .expect("Cannot delete order: order not found");
         self.orders.remove(index);
     }
 
+    #[must_use]
     pub fn volume(&self) -> f64 {
         let mut sum: f64 = 0.0;
         for o in self.orders.iter() {
             sum += o.size.as_f64()
         }
         sum
     }
 
+    #[must_use]
     pub fn exposure(&self) -> f64 {
         let mut sum: f64 = 0.0;
         for o in self.orders.iter() {
             sum += o.price.as_f64() * o.size.as_f64()
         }
         sum
     }
@@ -138,34 +141,34 @@
 impl Ord for Level {
     fn cmp(&self, other: &Self) -> Ordering {
         self.price.cmp(&other.price)
     }
 }
 
 impl Debug for Level {
-    fn fmt(&self, f: &mut Formatter<'_>) -> Result {
+    fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         write!(f, "Level(price={})", self.price.value)
     }
 }
 
 impl Display for Level {
-    fn fmt(&self, f: &mut Formatter<'_>) -> Result {
+    fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         write!(f, "Level(price={})", self.price.value)
     }
 }
 
 ////////////////////////////////////////////////////////////////////////////////
 // Tests
 ////////////////////////////////////////////////////////////////////////////////
 #[cfg(test)]
 mod tests {
+    use crate::data::book::BookOrder;
     use crate::enums::OrderSide;
     use crate::orderbook::ladder::BookPrice;
     use crate::orderbook::level::Level;
-    use crate::orderbook::order::BookOrder;
     use crate::types::price::Price;
     use crate::types::quantity::Quantity;
 
     #[test]
     fn test_level_comparisons_bid_side() {
         let level0 = Level::new(BookPrice::new(Price::new(1.00, 2), OrderSide::Buy));
         let level1 = Level::new(BookPrice::new(Price::new(1.01, 2), OrderSide::Buy));
@@ -181,85 +184,85 @@
         assert!(level0 < level1);
     }
 
     #[test]
     fn test_level_add_one_order() {
         let mut level = Level::new(BookPrice::new(Price::new(1.00, 2), OrderSide::Buy));
         let order = BookOrder::new(
+            OrderSide::Buy,
             Price::new(1.00, 2),
             Quantity::new(10.0, 0),
-            OrderSide::Buy,
             0,
         );
 
         level.add(order);
         assert!(!level.is_empty());
         assert_eq!(level.len(), 1);
         assert_eq!(level.volume(), 10.0);
     }
 
     #[test]
     fn test_level_add_multiple_orders() {
         let mut level = Level::new(BookPrice::new(Price::new(2.00, 2), OrderSide::Buy));
         let order1 = BookOrder::new(
+            OrderSide::Buy,
             Price::new(2.00, 2),
             Quantity::new(10.0, 0),
-            OrderSide::Buy,
             0,
         );
         let order2 = BookOrder::new(
+            OrderSide::Buy,
             Price::new(2.00, 2),
             Quantity::new(20.0, 0),
-            OrderSide::Buy,
             1,
         );
 
         level.add(order1);
         level.add(order2);
         assert_eq!(level.len(), 2);
         assert_eq!(level.volume(), 30.0);
         assert_eq!(level.exposure(), 60.0);
     }
 
     #[test]
     fn test_level_update_order() {
         let mut level = Level::new(BookPrice::new(Price::new(1.00, 2), OrderSide::Buy));
         let order1 = BookOrder::new(
+            OrderSide::Buy,
             Price::new(1.00, 2),
             Quantity::new(10.0, 0),
-            OrderSide::Buy,
             0,
         );
         let order2 = BookOrder::new(
+            OrderSide::Buy,
             Price::new(1.00, 2),
             Quantity::new(20.0, 0),
-            OrderSide::Buy,
             0,
         );
 
         level.add(order1);
         level.update(order2);
         assert_eq!(level.len(), 1);
         assert_eq!(level.volume(), 20.0);
         assert_eq!(level.exposure(), 20.0);
     }
 
     #[test]
     fn test_level_update_order_with_zero_size_deletes() {
         let mut level = Level::new(BookPrice::new(Price::new(1.00, 2), OrderSide::Buy));
         let order1 = BookOrder::new(
+            OrderSide::Buy,
             Price::new(1.00, 2),
             Quantity::new(10.0, 0),
-            OrderSide::Buy,
             0,
         );
         let order2 = BookOrder::new(
+            OrderSide::Buy,
             Price::new(1.00, 2),
             Quantity::new(0.0, 0),
-            OrderSide::Buy,
             0,
         );
 
         level.add(order1);
         level.update(order2);
         assert_eq!(level.len(), 0);
         assert_eq!(level.volume(), 0.0);
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/model/src/orderbook/mod.rs` & `nautilus_trader-1.174.0/nautilus_core/persistence/src/parquet/implementations/mod.rs`

 * *Files 10% similar despite different names*

```diff
@@ -9,11 +9,12 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
-pub mod book;
-pub mod ladder;
-pub mod level;
-pub mod order;
+mod bar;
+mod book_delta;
+mod book_snapshot;
+mod quote;
+mod trade;
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/model/src/orders/limit.rs` & `nautilus_trader-1.174.0/nautilus_core/model/src/orders/limit.rs`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
 use std::rc::Rc;
 
 use nautilus_core::{time::UnixNanos, uuid::UUID4};
-use rust_fsm::StateMachine;
 
 use crate::{
     enums::{ContingencyType, OrderSide, OrderStatus, OrderType, TimeInForce, TriggerType},
     events::order::OrderIdentifiers,
     identifiers::{
         client_order_id::ClientOrderId, instrument_id::InstrumentId, order_list_id::OrderListId,
         strategy_id::StrategyId, trader_id::TraderId,
@@ -88,15 +87,14 @@
             instrument_id,
             client_order_id,
         };
         Self {
             events: Vec::new(),
             venue_order_ids: Vec::new(),
             trade_ids: Vec::new(),
-            fsm: StateMachine::new(),
             previous_status: None,
             triggered_price: None,
             status: OrderStatus::Initialized,
             ids: Rc::new(metadata),
             venue_order_id: None,
             position_id: None,
             account_id: None,
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/model/src/orders/mod.rs` & `nautilus_trader-1.174.0/nautilus_core/model/src/orders/mod.rs`

 * *Files 22% similar despite different names*

```diff
@@ -11,19 +11,20 @@
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
 #![allow(dead_code)]
 
+pub mod limit;
+
 use std::rc::Rc;
 
 use nautilus_core::time::UnixNanos;
 use nautilus_core::uuid::UUID4;
-use rust_fsm::*;
 use thiserror::Error;
 
 use crate::enums::{
     ContingencyType, LiquiditySide, OrderSide, OrderStatus, OrderType, PositionSide, TimeInForce,
     TriggerType,
 };
 use crate::events::order::{
@@ -37,161 +38,89 @@
 use crate::identifiers::position_id::PositionId;
 use crate::identifiers::trade_id::TradeId;
 use crate::identifiers::venue_order_id::VenueOrderId;
 use crate::types::fixed::fixed_i64_to_f64;
 use crate::types::price::Price;
 use crate::types::quantity::Quantity;
 
-pub mod limit;
-
 #[derive(Error, Debug)]
 pub enum OrderError {
     #[error("Invalid state transition")]
     InvalidStateTransition,
     #[error("Unrecognized event")]
     UnrecognizedEvent,
 }
 
-impl From<TransitionImpossibleError> for OrderError {
-    fn from(_: TransitionImpossibleError) -> Self {
-        OrderError::InvalidStateTransition
-    }
-}
-
-#[derive(Debug)]
-struct OrderFsm;
-
-impl StateMachineImpl for OrderFsm {
-    type Input = OrderEvent;
-    type State = OrderStatus;
-    type Output = OrderStatus;
-    const INITIAL_STATE: Self::State = OrderStatus::Initialized;
-
+impl OrderStatus {
     #[rustfmt::skip]
-    fn transition(state: &Self::State, input: &Self::Input) -> Option<Self::State> {
-        match (state, input) {
-            (OrderStatus::Initialized, OrderEvent::OrderDenied(_)) => Some(OrderStatus::Denied),
-            (OrderStatus::Initialized, OrderEvent::OrderSubmitted(_)) => Some(OrderStatus::Submitted),
-            (OrderStatus::Initialized, OrderEvent::OrderRejected(_)) => Some(OrderStatus::Rejected),  // Covers external orders
-            (OrderStatus::Initialized, OrderEvent::OrderAccepted(_)) => Some(OrderStatus::Accepted),  // Covers external orders
-            (OrderStatus::Initialized, OrderEvent::OrderCanceled(_)) => Some(OrderStatus::Canceled),  // Covers emulated and external orders
-            (OrderStatus::Initialized, OrderEvent::OrderExpired(_)) => Some(OrderStatus::Expired),  // Covers emulated and external orders
-            (OrderStatus::Initialized, OrderEvent::OrderTriggered(_)) => Some(OrderStatus::Triggered), // Covers emulated and external orders
-            (OrderStatus::Submitted, OrderEvent::OrderPendingUpdate(_)) => Some(OrderStatus::PendingUpdate),
-            (OrderStatus::Submitted, OrderEvent::OrderPendingCancel(_)) => Some(OrderStatus::PendingCancel),
-            (OrderStatus::Submitted, OrderEvent::OrderRejected(_)) => Some(OrderStatus::Rejected),
-            (OrderStatus::Submitted, OrderEvent::OrderCanceled(_)) => Some(OrderStatus::Canceled),  // Covers FOK and IOC cases
-            (OrderStatus::Submitted, OrderEvent::OrderAccepted(_)) => Some(OrderStatus::Accepted),
-            (OrderStatus::Submitted, OrderEvent::OrderTriggered(_)) => Some(OrderStatus::Triggered),  // Covers emulated StopLimit order
-            (OrderStatus::Submitted, OrderEvent::OrderPartiallyFilled(_)) => Some(OrderStatus::PartiallyFilled),
-            (OrderStatus::Submitted, OrderEvent::OrderFilled(_)) => Some(OrderStatus::Filled),
-            (OrderStatus::Accepted, OrderEvent::OrderRejected(_)) => Some(OrderStatus::Rejected),  // Covers StopLimit order
-            (OrderStatus::Accepted, OrderEvent::OrderPendingUpdate(_)) => Some(OrderStatus::PendingUpdate),
-            (OrderStatus::Accepted, OrderEvent::OrderPendingCancel(_)) => Some(OrderStatus::PendingCancel),
-            (OrderStatus::Accepted, OrderEvent::OrderCanceled(_)) => Some(OrderStatus::Canceled),
-            (OrderStatus::Accepted, OrderEvent::OrderTriggered(_)) => Some(OrderStatus::Triggered),
-            (OrderStatus::Accepted, OrderEvent::OrderExpired(_)) => Some(OrderStatus::Expired),
-            (OrderStatus::Accepted, OrderEvent::OrderPartiallyFilled(_)) => Some(OrderStatus::PartiallyFilled),
-            (OrderStatus::Accepted, OrderEvent::OrderFilled(_)) => Some(OrderStatus::Filled),
-            (OrderStatus::Canceled, OrderEvent::OrderPartiallyFilled(_)) => Some(OrderStatus::PartiallyFilled),  // Real world possibility
-            (OrderStatus::Canceled, OrderEvent::OrderFilled(_)) => Some(OrderStatus::Filled),  // Real world possibility
-            (OrderStatus::PendingUpdate, OrderEvent::OrderAccepted(_)) => Some(OrderStatus::Accepted),
-            (OrderStatus::PendingUpdate, OrderEvent::OrderCanceled(_)) => Some(OrderStatus::Canceled),
-            (OrderStatus::PendingUpdate, OrderEvent::OrderExpired(_)) => Some(OrderStatus::Expired),
-            (OrderStatus::PendingUpdate, OrderEvent::OrderTriggered(_)) => Some(OrderStatus::Triggered),
-            (OrderStatus::PendingUpdate, OrderEvent::OrderPendingUpdate(_)) => Some(OrderStatus::PendingUpdate),  // Allow multiple requests
-            (OrderStatus::PendingUpdate, OrderEvent::OrderPendingCancel(_)) => Some(OrderStatus::PendingCancel),
-            (OrderStatus::PendingUpdate, OrderEvent::OrderPartiallyFilled(_)) => Some(OrderStatus::PartiallyFilled),
-            (OrderStatus::PendingUpdate, OrderEvent::OrderFilled(_)) => Some(OrderStatus::Filled),
-            (OrderStatus::PendingCancel, OrderEvent::OrderPendingCancel(_)) => Some(OrderStatus::PendingCancel),  // Allow multiple requests
-            (OrderStatus::PendingCancel, OrderEvent::OrderCanceled(_)) => Some(OrderStatus::Canceled),
-            (OrderStatus::PendingCancel, OrderEvent::OrderAccepted(_)) => Some(OrderStatus::Accepted),  // Allow failed cancel requests
-            (OrderStatus::PendingCancel, OrderEvent::OrderPartiallyFilled(_)) => Some(OrderStatus::PartiallyFilled),
-            (OrderStatus::PendingCancel, OrderEvent::OrderFilled(_)) => Some(OrderStatus::Filled),
-            (OrderStatus::Triggered, OrderEvent::OrderRejected(_)) => Some(OrderStatus::Rejected),
-            (OrderStatus::Triggered, OrderEvent::OrderPendingUpdate(_)) => Some(OrderStatus::PendingUpdate),
-            (OrderStatus::Triggered, OrderEvent::OrderPendingCancel(_)) => Some(OrderStatus::PendingCancel),
-            (OrderStatus::Triggered, OrderEvent::OrderCanceled(_)) => Some(OrderStatus::Canceled),
-            (OrderStatus::Triggered, OrderEvent::OrderExpired(_)) => Some(OrderStatus::Expired),
-            (OrderStatus::Triggered, OrderEvent::OrderPartiallyFilled(_)) => Some(OrderStatus::PartiallyFilled),
-            (OrderStatus::Triggered, OrderEvent::OrderFilled(_)) => Some(OrderStatus::Filled),
-            (OrderStatus::PartiallyFilled, OrderEvent::OrderPendingUpdate(_)) => Some(OrderStatus::PendingUpdate),
-            (OrderStatus::PartiallyFilled, OrderEvent::OrderPendingCancel(_)) => Some(OrderStatus::PendingCancel),
-            (OrderStatus::PartiallyFilled, OrderEvent::OrderCanceled(_)) => Some(OrderStatus::Canceled),
-            (OrderStatus::PartiallyFilled, OrderEvent::OrderExpired(_)) => Some(OrderStatus::Expired),
-            (OrderStatus::PartiallyFilled, OrderEvent::OrderPartiallyFilled(_)) => Some(OrderStatus::PartiallyFilled),
-            (OrderStatus::PartiallyFilled, OrderEvent::OrderFilled(_)) => Some(OrderStatus::Filled),
-            _ => None,
-        }
-    }
-
-    #[rustfmt::skip]
-    fn output(state: &Self::State, input: &Self::Input) -> Option<Self::Output> {
-        match (state, input) {
-            (OrderStatus::Initialized, OrderEvent::OrderDenied(_)) => Some(OrderStatus::Denied),
-            (OrderStatus::Initialized, OrderEvent::OrderSubmitted(_)) => Some(OrderStatus::Submitted),
-            (OrderStatus::Initialized, OrderEvent::OrderRejected(_)) => Some(OrderStatus::Rejected),
-            (OrderStatus::Initialized, OrderEvent::OrderAccepted(_)) => Some(OrderStatus::Accepted),
-            (OrderStatus::Initialized, OrderEvent::OrderCanceled(_)) => Some(OrderStatus::Canceled),
-            (OrderStatus::Initialized, OrderEvent::OrderExpired(_)) => Some(OrderStatus::Expired),
-            (OrderStatus::Initialized, OrderEvent::OrderTriggered(_)) => Some(OrderStatus::Triggered),
-            (OrderStatus::Submitted, OrderEvent::OrderPendingUpdate(_)) => Some(OrderStatus::PendingUpdate),
-            (OrderStatus::Submitted, OrderEvent::OrderPendingCancel(_)) => Some(OrderStatus::PendingCancel),
-            (OrderStatus::Submitted, OrderEvent::OrderRejected(_)) => Some(OrderStatus::Rejected),
-            (OrderStatus::Submitted, OrderEvent::OrderCanceled(_)) => Some(OrderStatus::Canceled),
-            (OrderStatus::Submitted, OrderEvent::OrderAccepted(_)) => Some(OrderStatus::Accepted),
-            (OrderStatus::Submitted, OrderEvent::OrderTriggered(_)) => Some(OrderStatus::Triggered),
-            (OrderStatus::Submitted, OrderEvent::OrderPartiallyFilled(_)) => Some(OrderStatus::PartiallyFilled),
-            (OrderStatus::Submitted, OrderEvent::OrderFilled(_)) => Some(OrderStatus::Filled),
-            (OrderStatus::Accepted, OrderEvent::OrderRejected(_)) => Some(OrderStatus::Rejected),
-            (OrderStatus::Accepted, OrderEvent::OrderPendingUpdate(_)) => Some(OrderStatus::PendingUpdate),
-            (OrderStatus::Accepted, OrderEvent::OrderPendingCancel(_)) => Some(OrderStatus::PendingCancel),
-            (OrderStatus::Accepted, OrderEvent::OrderCanceled(_)) => Some(OrderStatus::Canceled),
-            (OrderStatus::Accepted, OrderEvent::OrderTriggered(_)) => Some(OrderStatus::Triggered),
-            (OrderStatus::Accepted, OrderEvent::OrderExpired(_)) => Some(OrderStatus::Expired),
-            (OrderStatus::Accepted, OrderEvent::OrderPartiallyFilled(_)) => Some(OrderStatus::PartiallyFilled),
-            (OrderStatus::Accepted, OrderEvent::OrderFilled(_)) => Some(OrderStatus::Filled),
-            (OrderStatus::Canceled, OrderEvent::OrderPartiallyFilled(_)) => Some(OrderStatus::PartiallyFilled),
-            (OrderStatus::Canceled, OrderEvent::OrderFilled(_)) => Some(OrderStatus::Filled),
-            (OrderStatus::PendingUpdate, OrderEvent::OrderAccepted(_)) => Some(OrderStatus::Accepted),
-            (OrderStatus::PendingUpdate, OrderEvent::OrderCanceled(_)) => Some(OrderStatus::Canceled),
-            (OrderStatus::PendingUpdate, OrderEvent::OrderExpired(_)) => Some(OrderStatus::Expired),
-            (OrderStatus::PendingUpdate, OrderEvent::OrderTriggered(_)) => Some(OrderStatus::Triggered),
-            (OrderStatus::PendingUpdate, OrderEvent::OrderPendingUpdate(_)) => Some(OrderStatus::PendingUpdate),
-            (OrderStatus::PendingUpdate, OrderEvent::OrderPendingCancel(_)) => Some(OrderStatus::PendingCancel),
-            (OrderStatus::PendingUpdate, OrderEvent::OrderPartiallyFilled(_)) => Some(OrderStatus::PartiallyFilled),
-            (OrderStatus::PendingUpdate, OrderEvent::OrderFilled(_)) => Some(OrderStatus::Filled),
-            (OrderStatus::PendingCancel, OrderEvent::OrderPendingCancel(_)) => Some(OrderStatus::PendingCancel),
-            (OrderStatus::PendingCancel, OrderEvent::OrderCanceled(_)) => Some(OrderStatus::Canceled),
-            (OrderStatus::PendingCancel, OrderEvent::OrderAccepted(_)) => Some(OrderStatus::Accepted),
-            (OrderStatus::PendingCancel, OrderEvent::OrderPartiallyFilled(_)) => Some(OrderStatus::PartiallyFilled),
-            (OrderStatus::PendingCancel, OrderEvent::OrderFilled(_)) => Some(OrderStatus::Filled),
-            (OrderStatus::Triggered, OrderEvent::OrderRejected(_)) => Some(OrderStatus::Rejected),
-            (OrderStatus::Triggered, OrderEvent::OrderPendingUpdate(_)) => Some(OrderStatus::PendingUpdate),
-            (OrderStatus::Triggered, OrderEvent::OrderPendingCancel(_)) => Some(OrderStatus::PendingCancel),
-            (OrderStatus::Triggered, OrderEvent::OrderCanceled(_)) => Some(OrderStatus::Canceled),
-            (OrderStatus::Triggered, OrderEvent::OrderExpired(_)) => Some(OrderStatus::Expired),
-            (OrderStatus::Triggered, OrderEvent::OrderPartiallyFilled(_)) => Some(OrderStatus::PartiallyFilled),
-            (OrderStatus::Triggered, OrderEvent::OrderFilled(_)) => Some(OrderStatus::Filled),
-            (OrderStatus::PartiallyFilled, OrderEvent::OrderPendingUpdate(_)) => Some(OrderStatus::PendingUpdate),
-            (OrderStatus::PartiallyFilled, OrderEvent::OrderPendingCancel(_)) => Some(OrderStatus::PendingCancel),
-            (OrderStatus::PartiallyFilled, OrderEvent::OrderCanceled(_)) => Some(OrderStatus::Canceled),
-            (OrderStatus::PartiallyFilled, OrderEvent::OrderExpired(_)) => Some(OrderStatus::Expired),
-            (OrderStatus::PartiallyFilled, OrderEvent::OrderPartiallyFilled(_)) => Some(OrderStatus::PartiallyFilled),
-            (OrderStatus::PartiallyFilled, OrderEvent::OrderFilled(_)) => Some(OrderStatus::Filled),
-            _ => None,
-        }
+    pub fn transition(&mut self, event: &OrderEvent) -> Result<OrderStatus, OrderError> {
+        let new_state = match (self, event) {
+            (OrderStatus::Initialized, OrderEvent::OrderDenied(_)) => OrderStatus::Denied,
+            (OrderStatus::Initialized, OrderEvent::OrderSubmitted(_)) => OrderStatus::Submitted,
+            (OrderStatus::Initialized, OrderEvent::OrderRejected(_)) => OrderStatus::Rejected,  // Covers external orders
+            (OrderStatus::Initialized, OrderEvent::OrderAccepted(_)) => OrderStatus::Accepted,  // Covers external orders
+            (OrderStatus::Initialized, OrderEvent::OrderCanceled(_)) => OrderStatus::Canceled,  // Covers emulated and external orders
+            (OrderStatus::Initialized, OrderEvent::OrderExpired(_)) => OrderStatus::Expired,  // Covers emulated and external orders
+            (OrderStatus::Initialized, OrderEvent::OrderTriggered(_)) => OrderStatus::Triggered, // Covers emulated and external orders
+            (OrderStatus::Submitted, OrderEvent::OrderPendingUpdate(_)) => OrderStatus::PendingUpdate,
+            (OrderStatus::Submitted, OrderEvent::OrderPendingCancel(_)) => OrderStatus::PendingCancel,
+            (OrderStatus::Submitted, OrderEvent::OrderRejected(_)) => OrderStatus::Rejected,
+            (OrderStatus::Submitted, OrderEvent::OrderCanceled(_)) => OrderStatus::Canceled,  // Covers FOK and IOC cases
+            (OrderStatus::Submitted, OrderEvent::OrderAccepted(_)) => OrderStatus::Accepted,
+            (OrderStatus::Submitted, OrderEvent::OrderTriggered(_)) => OrderStatus::Triggered,  // Covers emulated StopLimit order
+            (OrderStatus::Submitted, OrderEvent::OrderPartiallyFilled(_)) => OrderStatus::PartiallyFilled,
+            (OrderStatus::Submitted, OrderEvent::OrderFilled(_)) => OrderStatus::Filled,
+            (OrderStatus::Accepted, OrderEvent::OrderRejected(_)) => OrderStatus::Rejected,  // Covers StopLimit order
+            (OrderStatus::Accepted, OrderEvent::OrderPendingUpdate(_)) => OrderStatus::PendingUpdate,
+            (OrderStatus::Accepted, OrderEvent::OrderPendingCancel(_)) => OrderStatus::PendingCancel,
+            (OrderStatus::Accepted, OrderEvent::OrderCanceled(_)) => OrderStatus::Canceled,
+            (OrderStatus::Accepted, OrderEvent::OrderTriggered(_)) => OrderStatus::Triggered,
+            (OrderStatus::Accepted, OrderEvent::OrderExpired(_)) => OrderStatus::Expired,
+            (OrderStatus::Accepted, OrderEvent::OrderPartiallyFilled(_)) => OrderStatus::PartiallyFilled,
+            (OrderStatus::Accepted, OrderEvent::OrderFilled(_)) => OrderStatus::Filled,
+            (OrderStatus::Canceled, OrderEvent::OrderPartiallyFilled(_)) => OrderStatus::PartiallyFilled,  // Real world possibility
+            (OrderStatus::Canceled, OrderEvent::OrderFilled(_)) => OrderStatus::Filled,  // Real world possibility
+            (OrderStatus::PendingUpdate, OrderEvent::OrderRejected(_)) => OrderStatus::Rejected,
+            (OrderStatus::PendingUpdate, OrderEvent::OrderAccepted(_)) => OrderStatus::Accepted,
+            (OrderStatus::PendingUpdate, OrderEvent::OrderCanceled(_)) => OrderStatus::Canceled,
+            (OrderStatus::PendingUpdate, OrderEvent::OrderExpired(_)) => OrderStatus::Expired,
+            (OrderStatus::PendingUpdate, OrderEvent::OrderTriggered(_)) => OrderStatus::Triggered,
+            (OrderStatus::PendingUpdate, OrderEvent::OrderPendingUpdate(_)) => OrderStatus::PendingUpdate,  // Allow multiple requests
+            (OrderStatus::PendingUpdate, OrderEvent::OrderPendingCancel(_)) => OrderStatus::PendingCancel,
+            (OrderStatus::PendingUpdate, OrderEvent::OrderPartiallyFilled(_)) => OrderStatus::PartiallyFilled,
+            (OrderStatus::PendingUpdate, OrderEvent::OrderFilled(_)) => OrderStatus::Filled,
+            (OrderStatus::PendingCancel, OrderEvent::OrderRejected(_)) => OrderStatus::Rejected,
+            (OrderStatus::PendingCancel, OrderEvent::OrderPendingCancel(_)) => OrderStatus::PendingCancel,  // Allow multiple requests
+            (OrderStatus::PendingCancel, OrderEvent::OrderCanceled(_)) => OrderStatus::Canceled,
+            (OrderStatus::PendingCancel, OrderEvent::OrderAccepted(_)) => OrderStatus::Accepted,  // Allow failed cancel requests
+            (OrderStatus::PendingCancel, OrderEvent::OrderPartiallyFilled(_)) => OrderStatus::PartiallyFilled,
+            (OrderStatus::PendingCancel, OrderEvent::OrderFilled(_)) => OrderStatus::Filled,
+            (OrderStatus::Triggered, OrderEvent::OrderRejected(_)) => OrderStatus::Rejected,
+            (OrderStatus::Triggered, OrderEvent::OrderPendingUpdate(_)) => OrderStatus::PendingUpdate,
+            (OrderStatus::Triggered, OrderEvent::OrderPendingCancel(_)) => OrderStatus::PendingCancel,
+            (OrderStatus::Triggered, OrderEvent::OrderCanceled(_)) => OrderStatus::Canceled,
+            (OrderStatus::Triggered, OrderEvent::OrderExpired(_)) => OrderStatus::Expired,
+            (OrderStatus::Triggered, OrderEvent::OrderPartiallyFilled(_)) => OrderStatus::PartiallyFilled,
+            (OrderStatus::Triggered, OrderEvent::OrderFilled(_)) => OrderStatus::Filled,
+            (OrderStatus::PartiallyFilled, OrderEvent::OrderPendingUpdate(_)) => OrderStatus::PendingUpdate,
+            (OrderStatus::PartiallyFilled, OrderEvent::OrderPendingCancel(_)) => OrderStatus::PendingCancel,
+            (OrderStatus::PartiallyFilled, OrderEvent::OrderCanceled(_)) => OrderStatus::Canceled,
+            (OrderStatus::PartiallyFilled, OrderEvent::OrderExpired(_)) => OrderStatus::Expired,
+            (OrderStatus::PartiallyFilled, OrderEvent::OrderPartiallyFilled(_)) => OrderStatus::PartiallyFilled,
+            (OrderStatus::PartiallyFilled, OrderEvent::OrderFilled(_)) => OrderStatus::Filled,
+            _ => return Err(OrderError::InvalidStateTransition),
+        };
+        Ok(new_state)
     }
 }
 
 struct Order {
     events: Vec<OrderEvent>,
     venue_order_ids: Vec<VenueOrderId>, // TODO(cs): Should be `Vec<&VenueOrderId>` or similar
     trade_ids: Vec<TradeId>,            // TODO(cs): Should be `Vec<&TradeId>` or similar
-    fsm: StateMachine<OrderFsm>,
     previous_status: Option<OrderStatus>,
     triggered_price: Option<Price>,
     pub status: OrderStatus,
     pub ids: Rc<OrderIdentifiers>,
     pub venue_order_id: Option<VenueOrderId>,
     pub position_id: Option<PositionId>,
     pub account_id: Option<AccountId>,
@@ -238,15 +167,14 @@
 
 impl From<OrderInitialized> for Order {
     fn from(value: OrderInitialized) -> Self {
         Self {
             events: Vec::new(),
             venue_order_ids: Vec::new(),
             trade_ids: Vec::new(),
-            fsm: StateMachine::new(),
             previous_status: None,
             triggered_price: None,
             status: OrderStatus::Initialized,
             ids: value.ids,
             venue_order_id: None,
             position_id: None,
             account_id: None,
@@ -436,23 +364,17 @@
             (OrderSide::Sell, PositionSide::Short) => false,
             (OrderSide::Sell, PositionSide::Long) => self.leaves_qty <= position_qty,
             _ => true,
         }
     }
 
     pub fn apply(&mut self, event: OrderEvent) -> Result<(), OrderError> {
-        let status = self
-            .fsm
-            .consume(&event)?
-            .map(|status| {
-                self.previous_status.replace(self.status);
-                status
-            })
-            .ok_or(OrderError::InvalidStateTransition)?;
-        self.status = status;
+        let new_status = self.status.transition(&event)?;
+        self.previous_status = Some(self.status);
+        self.status = new_status;
 
         match &event {
             OrderEvent::OrderDenied(event) => self.denied(event),
             OrderEvent::OrderSubmitted(event) => self.submitted(event),
             OrderEvent::OrderRejected(event) => self.rejected(event),
             OrderEvent::OrderAccepted(event) => self.accepted(event),
             OrderEvent::OrderPendingUpdate(event) => self.pending_update(event),
@@ -560,44 +482,49 @@
         if self.avg_px.is_none() {
             self.avg_px = Some(last_px.as_f64());
         }
 
         let filled_qty = self.filled_qty.as_f64();
         let total_qty = filled_qty + last_qty.as_f64();
 
-        let avg_px = ((self.avg_px.unwrap() * filled_qty) + (last_px.as_f64() * last_qty.as_f64()))
+        let avg_px = self
+            .avg_px
+            .unwrap()
+            .mul_add(filled_qty, last_px.as_f64() * last_qty.as_f64())
             / total_qty;
         self.avg_px = Some(avg_px);
     }
 
     fn set_slippage(&mut self) {
         self.slippage = self.avg_px.and_then(|avg_px| {
             self.price
                 .as_ref()
                 .map(|price| fixed_i64_to_f64(price.raw))
-                .map(|price| match self.side {
+                .and_then(|price| match self.side {
                     OrderSide::Buy if avg_px > price => Some(avg_px - price),
                     OrderSide::Sell if avg_px < price => Some(price - avg_px),
                     _ => None,
                 })
-                .unwrap_or(None)
         })
     }
 }
 
 ////////////////////////////////////////////////////////////////////////////////
 // Tests
 ////////////////////////////////////////////////////////////////////////////////
 #[cfg(test)]
 mod tests {
-    use rstest::*;
+    use rstest::rstest;
 
     use super::*;
-    use crate::enums::*;
-    use crate::events::order::*;
+    use crate::enums::{OrderSide, OrderStatus, PositionSide};
+    use crate::events::order::{
+        OrderAcceptedBuilder, OrderDeniedBuilder, OrderEvent, OrderInitializedBuilder,
+        OrderSubmittedBuilder,
+    };
 
     #[test]
     fn test_order_initialized() {
         let order: Order = OrderInitializedBuilder::default().build().unwrap().into();
 
         assert_eq!(order.status, OrderStatus::Initialized);
         assert_eq!(order.last_event(), None);
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/model/src/position.rs` & `nautilus_trader-1.174.0/nautilus_core/model/src/position.rs`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
 impl Position {
     pub fn new(instrument: &Instrument, fill: &OrderFilled) -> Self {
         assert_eq!(instrument.id, fill.instrument_id);
         assert!(fill.position_id.is_some());
         assert!(fill.order_side != OrderSide::NoOrderSide);
 
-        Position {
+        Self {
             events: Vec::<OrderFilled>::new(),
             client_order_ids: Vec::<ClientOrderId>::new(),
             venue_order_ids: Vec::<VenueOrderId>::new(),
             trade_ids: Vec::<TradeId>::new(),
             buy_qty: Quantity::new(0.0, instrument.size_precision),
             sell_qty: Quantity::new(0.0, instrument.size_precision),
             commissions: HashMap::<Currency, Money>::new(),
@@ -192,7 +192,11 @@
 impl PartialEq<Self> for Position {
     fn eq(&self, other: &Self) -> bool {
         self.id == other.id
     }
 }
 
 impl Eq for Position {}
+
+////////////////////////////////////////////////////////////////////////////////
+// Tests
+////////////////////////////////////////////////////////////////////////////////
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/model/src/types/balance.rs` & `nautilus_trader-1.174.0/nautilus_core/model/src/types/balance.rs`

 * *Files 10% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
-use std::fmt;
+use std::fmt::{Display, Formatter};
 
 use crate::types::currency::Currency;
 use crate::types::money::Money;
 
 pub struct AccountBalance {
     pub currency: Currency,
     pub total: Money,
     pub locked: Money,
     pub free: Money,
 }
 
-impl fmt::Display for AccountBalance {
-    fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
+impl Display for AccountBalance {
+    fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         write!(
             f,
             "{} {} {} {}",
             self.currency.code, self.total, self.locked, self.free,
         )
     }
 }
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/model/src/types/currency.rs` & `nautilus_trader-1.174.0/nautilus_core/model/src/types/currency.rs`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         name: &str,
         currency_type: CurrencyType,
     ) -> Self {
         correctness::valid_string(code, "`Currency` code");
         correctness::valid_string(name, "`Currency` name");
         correctness::u8_in_range_inclusive(precision, 0, 9, "`Currency` precision");
 
-        Currency {
+        Self {
             code: Box::new(Arc::new(code.to_string())),
             precision,
             iso4217,
             name: Box::new(Arc::new(name.to_string())),
             currency_type,
         }
     }
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/model/src/types/fixed.rs` & `nautilus_trader-1.174.0/nautilus_core/model/src/types/fixed.rs`

 * *Files 26% similar despite different names*

```diff
@@ -10,147 +10,151 @@
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
 pub const FIXED_PRECISION: u8 = 9;
-pub const FIXED_SCALAR: f64 = 1000000000.0; // 10.0**FIXED_PRECISION
+pub const FIXED_SCALAR: f64 = 1_000_000_000.0; // 10.0**FIXED_PRECISION
 
+#[must_use]
 pub fn f64_to_fixed_i64(value: f64, precision: u8) -> i64 {
     assert!(precision <= FIXED_PRECISION, "precision exceeded maximum 9");
-    let pow1 = 10_i64.pow(precision as u32);
-    let pow2 = 10_i64.pow((FIXED_PRECISION - precision) as u32);
+    let pow1 = 10_i64.pow(u32::from(precision));
+    let pow2 = 10_i64.pow(u32::from(FIXED_PRECISION - precision));
     let rounded = (value * pow1 as f64).round() as i64;
     rounded * pow2
 }
 
+#[must_use]
 pub fn f64_to_fixed_u64(value: f64, precision: u8) -> u64 {
     assert!(precision <= FIXED_PRECISION, "precision exceeded maximum 9");
-    let pow1 = 10_u64.pow(precision as u32);
-    let pow2 = 10_u64.pow((FIXED_PRECISION - precision) as u32);
+    let pow1 = 10_u64.pow(u32::from(precision));
+    let pow2 = 10_u64.pow(u32::from(FIXED_PRECISION - precision));
     let rounded = (value * pow1 as f64).round() as u64;
     rounded * pow2
 }
 
+#[must_use]
 pub fn fixed_i64_to_f64(value: i64) -> f64 {
-    (value as f64) * 0.000000001
+    (value as f64) * 0.000_000_001
 }
 
+#[must_use]
 pub fn fixed_u64_to_f64(value: u64) -> f64 {
-    (value as f64) * 0.000000001
+    (value as f64) * 0.000_000_001
 }
 
 ////////////////////////////////////////////////////////////////////////////////
 // Tests
 ////////////////////////////////////////////////////////////////////////////////
 #[cfg(test)]
 mod tests {
-    use rstest::*;
+    use rstest::rstest;
 
     use super::*;
 
     #[rstest(precision, value,
         case(0, 0.0),
         case(1, 1.0),
         case(1, 1.1),
-        case(9, 0.000000001),
+        case(9, 0.000_000_001),
         case(0, -0.0),
         case(1, -1.0),
         case(1, -1.1),
-        case(9, -0.000000001),
+        case(9, -0.000_000_001),
     )]
     fn test_f64_to_fixed_i64_to_fixed(precision: u8, value: f64) {
         let fixed = f64_to_fixed_i64(value, precision);
         let result = fixed_i64_to_f64(fixed);
         assert_eq!(result, value);
     }
 
     #[rstest(
         precision,
         value,
         case(0, 0.0),
         case(1, 1.0),
         case(1, 1.1),
-        case(9, 0.000000001)
+        case(9, 0.000_000_001)
     )]
     fn test_f64_to_fixed_u64_to_fixed(precision: u8, value: f64) {
         let fixed = f64_to_fixed_u64(value, precision);
         let result = fixed_u64_to_f64(fixed);
         assert_eq!(result, value);
     }
 
     #[rstest(
         precision,
         value,
         expected,
-        case(0, 123456.0, 123456000000000),
-        case(0, 123456.7, 123457000000000),
-        case(0, 123456.4, 123456000000000),
-        case(1, 123456.0, 123456000000000),
-        case(1, 123456.7, 123456700000000),
-        case(1, 123456.4, 123456400000000),
-        case(2, 123456.0, 123456000000000),
-        case(2, 123456.7, 123456700000000),
-        case(2, 123456.4, 123456400000000)
+        case(0, 123_456.0, 123_456_000_000_000),
+        case(0, 123_456.7, 123_457_000_000_000),
+        case(0, 123_456.4, 123_456_000_000_000),
+        case(1, 123_456.0, 123_456_000_000_000),
+        case(1, 123_456.7, 123_456_700_000_000),
+        case(1, 123_456.4, 123_456_400_000_000),
+        case(2, 123_456.0, 123_456_000_000_000),
+        case(2, 123_456.7, 123_456_700_000_000),
+        case(2, 123_456.4, 123_456_400_000_000)
     )]
     fn test_f64_to_fixed_i64_with_precision(precision: u8, value: f64, expected: i64) {
         assert_eq!(f64_to_fixed_i64(value, precision), expected);
     }
 
     #[rstest(precision, value, expected,
-        case(0, 5.5, 6000000000),
-        case(1, 5.55, 5600000000),
-        case(2, 5.555, 5560000000),
-        case(3, 5.5555, 5556000000),
-        case(4, 5.55555, 5555600000),
-        case(5, 5.555555, 5555560000),
-        case(6, 5.5555555, 5555556000),
-        case(7, 5.55555555, 5555555600),
-        case(8, 5.555555555, 5555555560),
-        case(9, 5.5555555555, 5555555556),
-        case(0, -5.5, -6000000000),
-        case(1, -5.55, -5600000000),
-        case(2, -5.555, -5560000000),
-        case(3, -5.5555, -5556000000),
-        case(4, -5.55555, -5555600000),
-        case(5, -5.555555, -5555560000),
-        case(6, -5.5555555, -5555556000),
-        case(7, -5.55555555, -5555555600),
-        case(8, -5.555555555, -5555555560),
-        case(9, -5.5555555555, -5555555556),
+        case(0, 5.5, 6_000_000_000),
+        case(1, 5.55, 5_600_000_000),
+        case(2, 5.555, 5_560_000_000),
+        case(3, 5.5555, 5_556_000_000),
+        case(4, 5.55555, 5_555_600_000),
+        case(5, 5.555_555, 5_555_560_000),
+        case(6, 5.555_555_5, 5_555_556_000),
+        case(7, 5.555_555_55, 5_555_555_600),
+        case(8, 5.555_555_555, 5_555_555_560),
+        case(9, 5.555_555_555_5, 5_555_555_556),
+        case(0, -5.5, -6_000_000_000),
+        case(1, -5.55, -5_600_000_000),
+        case(2, -5.555, -5_560_000_000),
+        case(3, -5.5555, -5_556_000_000),
+        case(4, -5.55555, -5_555_600_000),
+        case(5, -5.555_555, -5_555_560_000),
+        case(6, -5.555_555_5, -5_555_556_000),
+        case(7, -5.555_555_55, -5_555_555_600),
+        case(8, -5.555_555_555, -5_555_555_560),
+        case(9, -5.555_555_555_5, -5_555_555_556),
     )]
     fn test_f64_to_fixed_i64(precision: u8, value: f64, expected: i64) {
         assert_eq!(f64_to_fixed_i64(value, precision), expected);
     }
 
     #[rstest(
         precision,
         value,
         expected,
-        case(0, 5.5, 6000000000),
-        case(1, 5.55, 5600000000),
-        case(2, 5.555, 5560000000),
-        case(3, 5.5555, 5556000000),
-        case(4, 5.55555, 5555600000),
-        case(5, 5.555555, 5555560000),
-        case(6, 5.5555555, 5555556000),
-        case(7, 5.55555555, 5555555600),
-        case(8, 5.555555555, 5555555560),
-        case(9, 5.5555555555, 5555555556)
+        case(0, 5.5, 6_000_000_000),
+        case(1, 5.55, 5_600_000_000),
+        case(2, 5.555, 5_560_000_000),
+        case(3, 5.5555, 5_556_000_000),
+        case(4, 5.55555, 5_555_600_000),
+        case(5, 5.555_555, 5_555_560_000),
+        case(6, 5.555_555_5, 5_555_556_000),
+        case(7, 5.555_555_55, 5_555_555_600),
+        case(8, 5.555_555_555, 5_555_555_560),
+        case(9, 5.555_555_555_5, 5_555_555_556)
     )]
     fn test_f64_to_fixed_u64(precision: u8, value: f64, expected: u64) {
         assert_eq!(f64_to_fixed_u64(value, precision), expected);
     }
 
     #[rstest]
     fn test_fixed_i64_to_f64(
         #[values(1, -1, 2, -2, 10, -10, 100, -100, 1_000, -1_000)] value: i64,
     ) {
-        assert_eq!(fixed_i64_to_f64(value), value as f64 * 0.000000001);
+        assert_eq!(fixed_i64_to_f64(value), value as f64 * 0.000_000_001);
     }
 
     #[rstest]
     fn test_fixed_u64_to_f64(
         #[values(
             0,
             1,
@@ -171,10 +175,10 @@
             10_000_000_000_000,
             100_000_000_000_000,
             1_000_000_000_000_000
         )]
         value: u64,
     ) {
         let result = fixed_u64_to_f64(value);
-        assert_eq!(result, (value as f64) * 0.000000001);
+        assert_eq!(result, (value as f64) * 0.000_000_001);
     }
 }
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/model/src/types/mod.rs` & `nautilus_trader-1.174.0/nautilus_core/model/src/types/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_core/model/src/types/money.rs` & `nautilus_trader-1.174.0/nautilus_core/model/src/types/money.rs`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
 use std::cmp::Ordering;
-use std::fmt::{Display, Formatter, Result};
+use std::fmt::{Display, Formatter};
 use std::hash::{Hash, Hasher};
 use std::ops::{Add, AddAssign, Mul, MulAssign, Neg, Sub, SubAssign};
 
 use nautilus_core::correctness;
 
 use crate::types::currency::Currency;
 use crate::types::fixed::{f64_to_fixed_i64, fixed_i64_to_f64};
@@ -34,27 +34,30 @@
 }
 
 impl Money {
     #[must_use]
     pub fn new(amount: f64, currency: Currency) -> Self {
         correctness::f64_in_range_inclusive(amount, MONEY_MIN, MONEY_MAX, "`Money` amount");
 
-        Money {
+        Self {
             raw: f64_to_fixed_i64(amount, currency.precision),
             currency,
         }
     }
 
-    pub fn from_raw(raw: i64, currency: Currency) -> Money {
+    #[must_use]
+    pub fn from_raw(raw: i64, currency: Currency) -> Self {
         Self { raw, currency }
     }
 
+    #[must_use]
     pub fn is_zero(&self) -> bool {
         self.raw == 0
     }
+    #[must_use]
     pub fn as_f64(&self) -> f64 {
         fixed_i64_to_f64(self.raw)
     }
 }
 
 impl Hash for Money {
     fn hash<H: Hasher>(&self, state: &mut H) {
@@ -101,48 +104,48 @@
         self.raw.cmp(&other.raw)
     }
 }
 
 impl Neg for Money {
     type Output = Self;
     fn neg(self) -> Self::Output {
-        Money {
+        Self {
             raw: -self.raw,
             currency: self.currency,
         }
     }
 }
 
 impl Add for Money {
     type Output = Self;
-    fn add(self, rhs: Money) -> Self::Output {
+    fn add(self, rhs: Self) -> Self::Output {
         assert_eq!(self.currency, rhs.currency);
-        Money {
+        Self {
             raw: self.raw + rhs.raw,
             currency: self.currency,
         }
     }
 }
 
 impl Sub for Money {
     type Output = Self;
-    fn sub(self, rhs: Money) -> Self::Output {
+    fn sub(self, rhs: Self) -> Self::Output {
         assert_eq!(self.currency, rhs.currency);
-        Money {
+        Self {
             raw: self.raw - rhs.raw,
             currency: self.currency,
         }
     }
 }
 
 impl Mul for Money {
     type Output = Self;
-    fn mul(self, rhs: Money) -> Self {
+    fn mul(self, rhs: Self) -> Self {
         assert_eq!(self.currency, rhs.currency);
-        Money {
+        Self {
             raw: self.raw * rhs.raw,
             currency: self.currency,
         }
     }
 }
 
 impl AddAssign for Money {
@@ -183,15 +186,15 @@
     type Output = f64;
     fn mul(self, rhs: f64) -> Self::Output {
         self.as_f64() * rhs
     }
 }
 
 impl Display for Money {
-    fn fmt(&self, f: &mut Formatter<'_>) -> Result {
+    fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         write!(
             f,
             "{:.*} {}",
             self.currency.precision as usize,
             self.as_f64(),
             self.currency.code
         )
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/model/src/types/price.rs` & `nautilus_trader-1.174.0/nautilus_core/model/src/types/price.rs`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
 use std::cmp::Ordering;
-use std::fmt::{Debug, Display, Formatter, Result};
+use std::fmt::{Debug, Display, Formatter};
 use std::hash::{Hash, Hasher};
 use std::ops::{Add, AddAssign, Deref, Mul, MulAssign, Neg, Sub, SubAssign};
 
 use nautilus_core::correctness;
 use nautilus_core::parsing::precision_from_str;
 
 use crate::types::fixed::{f64_to_fixed_i64, fixed_i64_to_f64};
@@ -36,52 +36,55 @@
 }
 
 impl Price {
     #[must_use]
     pub fn new(value: f64, precision: u8) -> Self {
         correctness::f64_in_range_inclusive(value, PRICE_MIN, PRICE_MAX, "`Price` value");
 
-        Price {
+        Self {
             raw: f64_to_fixed_i64(value, precision),
             precision,
         }
     }
 
+    #[must_use]
     pub fn from_raw(raw: i64, precision: u8) -> Self {
-        Price { raw, precision }
+        Self { raw, precision }
     }
 
+    #[must_use]
     pub fn is_zero(&self) -> bool {
         self.raw == 0
     }
 
+    #[must_use]
     pub fn as_f64(&self) -> f64 {
         fixed_i64_to_f64(self.raw)
     }
 }
 
 impl From<&str> for Price {
     fn from(input: &str) -> Self {
         let float_from_input = input.parse::<f64>();
         let float_res = match float_from_input {
             Ok(number) => number,
             Err(err) => panic!("Cannot parse `input` string '{input}' as f64, {err}"),
         };
-        Price::new(float_res, precision_from_str(input))
+        Self::new(float_res, precision_from_str(input))
     }
 }
 
 impl From<Price> for f64 {
-    fn from(value: Price) -> f64 {
+    fn from(value: Price) -> Self {
         value.as_f64()
     }
 }
 
 impl From<&Price> for f64 {
-    fn from(value: &Price) -> f64 {
+    fn from(value: &Price) -> Self {
         value.as_f64()
     }
 }
 
 impl Hash for Price {
     fn hash<H: Hasher>(&self, state: &mut H) {
         self.raw.hash(state)
@@ -129,45 +132,45 @@
         &self.raw
     }
 }
 
 impl Neg for Price {
     type Output = Self;
     fn neg(self) -> Self::Output {
-        Price {
+        Self {
             raw: -self.raw,
             precision: self.precision,
         }
     }
 }
 
 impl Add for Price {
     type Output = Self;
-    fn add(self, rhs: Price) -> Self::Output {
-        Price {
+    fn add(self, rhs: Self) -> Self::Output {
+        Self {
             raw: self.raw + rhs.raw,
             precision: self.precision,
         }
     }
 }
 
 impl Sub for Price {
     type Output = Self;
-    fn sub(self, rhs: Price) -> Self::Output {
-        Price {
+    fn sub(self, rhs: Self) -> Self::Output {
+        Self {
             raw: self.raw - rhs.raw,
             precision: self.precision,
         }
     }
 }
 
 impl Mul for Price {
     type Output = Self;
-    fn mul(self, rhs: Price) -> Self {
-        Price {
+    fn mul(self, rhs: Self) -> Self {
+        Self {
             raw: (self.raw * rhs.raw) / (FIXED_SCALAR as i64),
             precision: self.precision,
         }
     }
 }
 
 impl AddAssign for Price {
@@ -206,21 +209,21 @@
     type Output = f64;
     fn mul(self, rhs: f64) -> Self::Output {
         self.as_f64() * rhs
     }
 }
 
 impl Debug for Price {
-    fn fmt(&self, f: &mut Formatter<'_>) -> Result {
+    fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         write!(f, "{:.*}", self.precision as usize, self.as_f64())
     }
 }
 
 impl Display for Price {
-    fn fmt(&self, f: &mut Formatter<'_>) -> Result {
+    fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         write!(f, "{:.*}", self.precision as usize, self.as_f64())
     }
 }
 
 ////////////////////////////////////////////////////////////////////////////////
 // C API
 ////////////////////////////////////////////////////////////////////////////////
@@ -256,23 +259,23 @@
 mod tests {
     use super::Price;
 
     #[test]
     fn test_price_new() {
         let price = Price::new(0.00812, 8);
         assert_eq!(price, price);
-        assert_eq!(price.raw, 8120000);
+        assert_eq!(price.raw, 8_120_000);
         assert_eq!(price.precision, 8);
         assert_eq!(price.as_f64(), 0.00812);
         assert_eq!(price.to_string(), "0.00812000");
     }
 
     #[test]
     fn test_price_minimum() {
-        let price = Price::new(0.000000001, 9);
+        let price = Price::new(0.000_000_001, 9);
         assert_eq!(price.raw, 1);
         assert_eq!(price.to_string(), "0.000000001");
     }
 
     #[test]
     fn test_price_is_zero() {
         let price = Price::new(0.0, 8);
@@ -283,23 +286,23 @@
         assert_eq!(price.to_string(), "0.00000000");
         assert!(price.is_zero());
     }
 
     #[test]
     fn test_price_precision() {
         let price = Price::new(1.001, 2);
-        assert_eq!(price.raw, 1000000000);
+        assert_eq!(price.raw, 1_000_000_000);
         assert_eq!(price.to_string(), "1.00");
     }
 
     #[test]
     fn test_price_new_from_str() {
         let price = Price::from("0.00812000");
         assert_eq!(price, price);
-        assert_eq!(price.raw, 8120000);
+        assert_eq!(price.raw, 8_120_000);
         assert_eq!(price.precision, 8);
         assert_eq!(price.as_f64(), 0.00812);
         assert_eq!(price.to_string(), "0.00812000");
     }
 
     #[test]
     fn test_price_equality() {
@@ -317,53 +320,53 @@
     }
 
     #[test]
     fn test_add() {
         let price1 = Price::new(1.000, 3);
         let price2 = Price::new(1.011, 3);
         let price3 = price1 + price2;
-        assert_eq!(price3.raw, 2011000000)
+        assert_eq!(price3.raw, 2_011_000_000)
     }
 
     #[test]
     fn test_sub() {
         let price1 = Price::new(1.011, 3);
         let price2 = Price::new(1.000, 3);
         let price3 = price1 - price2;
-        assert_eq!(price3.raw, 11000000);
+        assert_eq!(price3.raw, 11_000_000);
     }
 
     #[test]
     fn test_add_assign() {
         let mut price = Price::new(1.000, 3);
         price += Price::new(1.011, 3);
-        assert_eq!(price.raw, 2011000000)
+        assert_eq!(price.raw, 2_011_000_000)
     }
 
     #[test]
     fn test_sub_assign() {
         let mut price = Price::new(1.000, 3);
         price -= Price::new(0.011, 3);
-        assert_eq!(price.raw, 989000000)
+        assert_eq!(price.raw, 989_000_000)
     }
 
     #[test]
     fn test_mul() {
         let price1 = Price::new(1.000, 3);
         let price2 = Price::new(1.011, 3);
         let price3 = price1 * price2;
-        assert_eq!(price3.raw, 1011000000);
+        assert_eq!(price3.raw, 1_011_000_000);
     }
 
     #[test]
     fn test_mul_assign() {
         let mut price1 = Price::new(1.000, 3);
         let price2 = Price::new(1.011, 3);
         price1 *= price2;
-        assert_eq!(price1.raw, 1011000000000000000);
+        assert_eq!(price1.raw, 1_011_000_000_000_000_000);
     }
 
     #[test]
     fn test_price_display_works() {
         use std::fmt::Write as FmtWrite;
         let input_string = "44.12";
         let price = Price::from(input_string);
@@ -372,13 +375,13 @@
         assert_eq!(res, input_string);
     }
 
     #[test]
     fn test_price_display() {
         let input_string = "44.123456";
         let price = Price::from(input_string);
-        assert_eq!(price.raw, 44123456000);
+        assert_eq!(price.raw, 44_123_456_000);
         assert_eq!(price.precision, 6);
-        assert_eq!(price.as_f64(), 44.123456000000004);
+        assert_eq!(price.as_f64(), 44.123_456_000_000_004);
         assert_eq!(price.to_string(), "44.123456");
     }
 }
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/model/src/types/quantity.rs` & `nautilus_trader-1.174.0/nautilus_core/model/src/types/quantity.rs`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
 use std::cmp::Ordering;
-use std::fmt::{Debug, Display, Formatter, Result};
+use std::fmt::{Debug, Display, Formatter};
 use std::hash::{Hash, Hasher};
 use std::ops::{Add, AddAssign, Deref, Mul, MulAssign, Sub, SubAssign};
 
 use nautilus_core::correctness;
 use nautilus_core::parsing::precision_from_str;
 
 use crate::types::fixed::{f64_to_fixed_u64, fixed_u64_to_f64};
@@ -36,58 +36,61 @@
 }
 
 impl Quantity {
     #[must_use]
     pub fn new(value: f64, precision: u8) -> Self {
         correctness::f64_in_range_inclusive(value, QUANTITY_MIN, QUANTITY_MAX, "`Quantity` value");
 
-        Quantity {
+        Self {
             raw: f64_to_fixed_u64(value, precision),
             precision,
         }
     }
 
+    #[must_use]
     pub fn from_raw(raw: u64, precision: u8) -> Self {
-        Quantity { raw, precision }
+        Self { raw, precision }
     }
 
+    #[must_use]
     pub fn is_zero(&self) -> bool {
         self.raw == 0
     }
+    #[must_use]
     pub fn as_f64(&self) -> f64 {
         fixed_u64_to_f64(self.raw)
     }
 }
 
 impl From<Quantity> for f64 {
-    fn from(value: Quantity) -> f64 {
+    fn from(value: Quantity) -> Self {
         value.as_f64()
     }
 }
 
 impl From<&Quantity> for f64 {
-    fn from(value: &Quantity) -> f64 {
+    fn from(value: &Quantity) -> Self {
         value.as_f64()
     }
 }
 
 impl From<&str> for Quantity {
     fn from(input: &str) -> Self {
         let float_from_input = input.parse::<f64>();
         let float_res = match float_from_input {
             Ok(number) => number,
             Err(err) => panic!("cannot parse `input` string '{input}' as f64, {err}"),
         };
-        Quantity::new(float_res, precision_from_str(input))
+        Self::new(float_res, precision_from_str(input))
     }
 }
 
 impl From<i64> for Quantity {
     fn from(input: i64) -> Self {
-        Quantity::new(input as f64, 0)
+        Self::new(input as f64, 0)
     }
 }
 
 impl Hash for Quantity {
     fn hash<H: Hasher>(&self, state: &mut H) {
         self.raw.hash(state)
     }
@@ -134,49 +137,49 @@
         &self.raw
     }
 }
 
 impl Add for Quantity {
     type Output = Self;
     fn add(self, rhs: Self) -> Self::Output {
-        Quantity {
+        Self {
             raw: self.raw + rhs.raw,
             precision: self.precision,
         }
     }
 }
 
 impl Sub for Quantity {
     type Output = Self;
     fn sub(self, rhs: Self) -> Self::Output {
-        Quantity {
+        Self {
             raw: self.raw - rhs.raw,
             precision: self.precision,
         }
     }
 }
 
 impl Mul for Quantity {
     type Output = Self;
     fn mul(self, rhs: Self) -> Self::Output {
-        Quantity {
+        Self {
             raw: (self.raw * rhs.raw) / (FIXED_SCALAR as u64),
             precision: self.precision,
         }
     }
 }
 
 impl From<Quantity> for u64 {
-    fn from(value: Quantity) -> u64 {
+    fn from(value: Quantity) -> Self {
         value.raw
     }
 }
 
 impl From<&Quantity> for u64 {
-    fn from(value: &Quantity) -> u64 {
+    fn from(value: &Quantity) -> Self {
         value.raw
     }
 }
 
 impl<T: Into<u64>> AddAssign<T> for Quantity {
     fn add_assign(&mut self, other: T) {
         self.raw += other.into();
@@ -192,21 +195,21 @@
 impl<T: Into<u64>> MulAssign<T> for Quantity {
     fn mul_assign(&mut self, other: T) {
         self.raw *= other.into();
     }
 }
 
 impl Debug for Quantity {
-    fn fmt(&self, f: &mut Formatter<'_>) -> Result {
+    fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         write!(f, "{:.*}", self.precision as usize, self.as_f64())
     }
 }
 
 impl Display for Quantity {
-    fn fmt(&self, f: &mut Formatter<'_>) -> Result {
+    fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         write!(f, "{:.*}", self.precision as usize, self.as_f64())
     }
 }
 
 ////////////////////////////////////////////////////////////////////////////////
 // C API
 ////////////////////////////////////////////////////////////////////////////////
@@ -268,15 +271,15 @@
         assert_eq!(qty, qty);
         assert_eq!(qty.raw, 100_000_000_000_000);
         assert_eq!(qty.precision, 0);
     }
 
     #[test]
     fn test_qty_minimum() {
-        let qty = Quantity::new(0.000000001, 9);
+        let qty = Quantity::new(0.000_000_001, 9);
         assert_eq!(qty.raw, 1);
         assert_eq!(qty.to_string(), "0.000000001");
     }
 
     #[test]
     fn test_qty_is_zero() {
         let qty = Quantity::new(0.0, 8);
@@ -306,47 +309,47 @@
     }
 
     #[test]
     fn test_add() {
         let quantity1 = Quantity::new(1.0, 0);
         let quantity2 = Quantity::new(2.0, 0);
         let quantity3 = quantity1 + quantity2;
-        assert_eq!(quantity3.raw, 3000000000);
+        assert_eq!(quantity3.raw, 3_000_000_000);
     }
 
     #[test]
     fn test_sub() {
         let quantity1 = Quantity::new(3.0, 0);
         let quantity2 = Quantity::new(2.0, 0);
         let quantity3 = quantity1 - quantity2;
-        assert_eq!(quantity3.raw, 1000000000);
+        assert_eq!(quantity3.raw, 1_000_000_000);
     }
 
     #[test]
     fn test_add_assign() {
         let mut quantity1 = Quantity::new(1.0, 0);
         let quantity2 = Quantity::new(2.0, 0);
         quantity1 += quantity2;
-        assert_eq!(quantity1.raw, 3000000000);
+        assert_eq!(quantity1.raw, 3_000_000_000);
     }
 
     #[test]
     fn test_sub_assign() {
         let mut quantity1 = Quantity::new(3.0, 0);
         let quantity2 = Quantity::new(2.0, 0);
         quantity1 -= quantity2;
-        assert_eq!(quantity1.raw, 1000000000);
+        assert_eq!(quantity1.raw, 1_000_000_000);
     }
 
     #[test]
     fn test_mul() {
         let quantity1 = Quantity::new(2.0, 1);
         let quantity2 = Quantity::new(2.0, 1);
         let quantity3 = quantity1 * quantity2;
-        assert_eq!(quantity3.raw, 4000000000);
+        assert_eq!(quantity3.raw, 4_000_000_000);
     }
 
     #[test]
     fn test_quantity_mul_assign() {
         let mut q = Quantity::from_raw(100, 0);
         q *= 2u64;
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/network/src/lib.rs` & `nautilus_trader-1.174.0/nautilus_core/model/src/orderbook/mod.rs`

 * *Files 6% similar despite different names*

```diff
@@ -8,7 +8,11 @@
 //
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
+
+pub mod book;
+pub mod ladder;
+pub mod level;
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/persistence/Cargo.toml` & `nautilus_trader-1.174.0/nautilus_core/persistence/Cargo.toml`

 * *Files 17% similar despite different names*

```diff
@@ -16,14 +16,21 @@
 pyo3.workspace = true
 pyo3-asyncio.workspace = true
 rand.workspace = true
 tokio.workspace = true
 binary-heap-plus = "0.5.0"
 compare = "0.1.0"
 # FIX: default feature "crypto_expressions" using using blake3 fails build on windows: https://github.com/BLAKE3-team/BLAKE3/issues/298
-datafusion = { version = "23.0.0", default-features = false, features = ["compression", "regex_expressions", "unicode_expressions"] }
+datafusion = { version = "24.0.0", default-features = false, features = ["compression", "regex_expressions", "unicode_expressions"] }
 futures = "0.3.28"
 pin-project-lite = "0.2.9"
 
 [features]
 extension-module = ["pyo3/extension-module", "nautilus_core/extension-module", "nautilus_model/extension-module"]
 default = []
+
+[dev-dependencies]
+criterion.workspace = true
+
+[[bench]]
+name = "persistence_benchmark"
+harness = false
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/persistence/src/kmerge_batch.rs` & `nautilus_trader-1.174.0/nautilus_core/persistence/src/kmerge_batch.rs`

 * *Files 6% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     async fn new_from_stream(mut stream: S) -> Option<Self> {
         // Poll next batch from stream and get next item from the batch
         // and add the new element to the heap. No new element is added
         // to the heap if the stream is empty. Keep polling the stream
         // for a batch that is non-empty.
         let next_batch = stream.next().await;
         if let Some(mut batch) = next_batch {
-            batch.next().map(|next_item| PeekElementBatchStream {
+            batch.next().map(|next_item| Self {
                 item: next_item,
                 batch,
                 stream,
             })
         } else {
             // Stream is empty, no new batch
             None
@@ -115,14 +115,17 @@
         } else {
             // Heap is empty
             Poll::Ready(None)
         }
     }
 }
 
+////////////////////////////////////////////////////////////////////////////////
+// Tests
+////////////////////////////////////////////////////////////////////////////////
 #[cfg(test)]
 mod tests {
     use super::*;
     use futures::stream::iter;
 
     struct OrdComparator;
     impl<S> Compare<PeekElementBatchStream<S, i32>> for OrdComparator
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/persistence/src/lib.rs` & `nautilus_trader-1.174.0/nautilus_core/persistence/src/lib.rs`

 * *Files 20% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 
 mod kmerge_batch;
 pub mod parquet;
 pub mod session;
 
 use parquet::ParquetType;
 use pyo3::prelude::*;
-use session::{PythonCatalog, PythonQueryResult};
+use session::{DataBackendSession, DataQueryResult};
 
 /// Loaded as nautilus_pyo3.persistence
 #[pymodule]
 pub fn persistence(_: Python<'_>, m: &PyModule) -> PyResult<()> {
     m.add_class::<ParquetType>()?;
-    m.add_class::<PythonCatalog>()?;
-    m.add_class::<PythonQueryResult>()?;
+    m.add_class::<DataBackendSession>()?;
+    m.add_class::<DataQueryResult>()?;
     Ok(())
 }
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/persistence/src/parquet/implementations/mod.rs` & `nautilus_trader-1.174.0/nautilus_trader/model/events/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-// -------------------------------------------------------------------------------------------------
-//  Copyright (C) 2015-2023 Nautech Systems Pty Ltd. All rights reserved.
-//  https://nautechsystems.io
-//
-//  Licensed under the GNU Lesser General Public License Version 3.0 (the "License");
-//  You may not use this file except in compliance with the License.
-//  You may obtain a copy of the License at https://www.gnu.org/licenses/lgpl-3.0.en.html
-//
-//  Unless required by applicable law or agreed to in writing, software
-//  distributed under the License is distributed on an "AS IS" BASIS,
-//  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-//  See the License for the specific language governing permissions and
-//  limitations under the License.
-// -------------------------------------------------------------------------------------------------
+# -------------------------------------------------------------------------------------------------
+#  Copyright (C) 2015-2023 Nautech Systems Pty Ltd. All rights reserved.
+#  https://nautechsystems.io
+#
+#  Licensed under the GNU Lesser General Public License Version 3.0 (the "License");
+#  You may not use this file except in compliance with the License.
+#  You may obtain a copy of the License at https://www.gnu.org/licenses/lgpl-3.0.en.html
+#
+#  Unless required by applicable law or agreed to in writing, software
+#  distributed under the License is distributed on an "AS IS" BASIS,
+#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#  See the License for the specific language governing permissions and
+#  limitations under the License.
+# -------------------------------------------------------------------------------------------------
 
-mod quote_tick;
-mod trade_tick;
+"""Defines the fundamental event types represented within the trading domain."""
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/persistence/src/parquet/mod.rs` & `nautilus_trader-1.174.0/nautilus_core/persistence/src/parquet/mod.rs`

 * *Files 8% similar despite different names*

```diff
@@ -15,23 +15,27 @@
 
 mod implementations;
 
 use std::collections::HashMap;
 
 use datafusion::arrow::datatypes::SchemaRef;
 use datafusion::arrow::record_batch::RecordBatch;
-use nautilus_model::data::tick::Data;
+use nautilus_model::data::Data;
 use pyo3::prelude::*;
 
 #[repr(C)]
 #[pyclass]
 #[derive(Debug, Clone, Copy)]
 pub enum ParquetType {
-    QuoteTick = 0,
-    TradeTick = 1,
+    // Custom = 0,  # First slot reserved for custom data
+    OrderBookSnapshot = 1,
+    OrderBookDelta = 2,
+    QuoteTick = 3,
+    TradeTick = 4,
+    Bar = 5,
 }
 
 #[repr(C)]
 #[pyclass]
 #[derive(Debug, Clone, Copy)]
 pub enum ParquetReaderType {
     File = 0,
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/persistence/src/session.rs` & `nautilus_trader-1.174.0/nautilus_core/persistence/src/session.rs`

 * *Files 18% similar despite different names*

```diff
@@ -18,15 +18,18 @@
 use compare::Compare;
 use datafusion::error::Result;
 use datafusion::physical_plan::SendableRecordBatchStream;
 use datafusion::prelude::*;
 use futures::executor::block_on;
 use futures::{Stream, StreamExt};
 use nautilus_core::cvec::CVec;
-use nautilus_model::data::tick::{Data, QuoteTick, TradeTick};
+use nautilus_model::data::bar::Bar;
+use nautilus_model::data::book::{OrderBookDelta, OrderBookSnapshot};
+use nautilus_model::data::tick::{QuoteTick, TradeTick};
+use nautilus_model::data::Data;
 use pyo3::prelude::*;
 use pyo3::types::PyCapsule;
 use pyo3_asyncio::tokio::get_runtime;
 
 use crate::kmerge_batch::{KMerge, PeekElementBatchStream};
 use crate::parquet::{DecodeDataFromRecordBatch, ParquetType};
 
@@ -43,37 +46,43 @@
         r: &PeekElementBatchStream<S, Data>,
     ) -> std::cmp::Ordering {
         // Max heap ordering must be reversed
         l.item.get_ts_init().cmp(&r.item.get_ts_init()).reverse()
     }
 }
 
-/// Catalog is a data fusion session and registers data fusion queries.
+/// Provides a DataFusion session and registers DataFusion queries.
 ///
 /// The session is used to register data sources and make queries on them. A
 /// query returns a Chunk of Arrow records. It is decoded and converted into
-/// a Vec of data by types that implement [DecodeDataFromRecordBatch].
-pub struct PersistenceCatalog {
+/// a Vec of data by types that implement [`DecodeDataFromRecordBatch`].
+#[pyclass]
+pub struct DataBackendSession {
     session_ctx: SessionContext,
     batch_streams: Vec<Box<dyn Stream<Item = IntoIter<Data>> + Unpin>>,
     chunk_size: usize,
 }
 
-impl PersistenceCatalog {
+impl DataBackendSession {
+    #[must_use]
     pub fn new(chunk_size: usize) -> Self {
         Self {
             session_ctx: SessionContext::default(),
             batch_streams: Vec::default(),
             chunk_size,
         }
     }
 
     // Query a file for all it's records. the caller must specify `T` to indicate
     // the kind of data expected from this query.
-    pub async fn add_file<T>(&mut self, table_name: &str, file_path: &str) -> Result<()>
+    pub async fn add_file_default_query<T>(
+        &mut self,
+        table_name: &str,
+        file_path: &str,
+    ) -> Result<()>
     where
         T: DecodeDataFromRecordBatch + Into<Data>,
     {
         let parquet_options = ParquetReadOptions::<'_> {
             skip_metadata: Some(false),
             ..Default::default()
         };
@@ -94,15 +103,15 @@
 
     // Query a file for all it's records with a custom query. The caller must
     // specify `T` to indicate what kind of data is expected from this query.
     //
     // #Safety
     // They query should ensure the records are ordered by the `ts_init` field
     // in ascending order.
-    pub async fn add_file_with_query<T>(
+    pub async fn add_file_with_custom_query<T>(
         &mut self,
         table_name: &str,
         file_path: &str,
         sql_query: &str,
     ) -> Result<()>
     where
         T: DecodeDataFromRecordBatch + Into<Data>,
@@ -138,15 +147,15 @@
         self.batch_streams.push(Box::new(transform));
     }
 
     // Consumes the registered queries and returns a [QueryResult].
     // Passes the output of the query though the a KMerge which sorts the
     // queries in ascending order of `ts_init`.
     // QueryResult is an iterator that return Vec<Data>.
-    pub fn to_query_result(&mut self) -> QueryResult<Data> {
+    pub fn get_query_result(&mut self) -> QueryResult<Data> {
         // TODO: No need to kmerge if there is only one batch stream
         let mut kmerge: KMerge<_, _, _> = KMerge::new(TsInitComparator);
 
         Iterator::for_each(self.batch_streams.drain(..), |batch_stream| {
             block_on(kmerge.push_stream(batch_stream));
         });
 
@@ -164,55 +173,73 @@
     type Item = Vec<Data>;
 
     fn next(&mut self) -> Option<Self::Item> {
         block_on(self.data.next())
     }
 }
 
-//////////////////////////////////////////
+////////////////////////////////////////////////////////////////////////////////
 /// Python API
-//////////////////////////////////////////
-
-/// Store the data fusion session context
-#[pyclass]
-pub struct PythonCatalog(PersistenceCatalog);
+////////////////////////////////////////////////////////////////////////////////
 
 // Note: Intended to be used on a single python thread
-unsafe impl Send for PersistenceCatalog {}
+unsafe impl Send for DataBackendSession {}
 
 #[pymethods]
-impl PythonCatalog {
+impl DataBackendSession {
     #[new]
     #[pyo3(signature=(chunk_size=5000))]
+    #[must_use]
     pub fn new_session(chunk_size: usize) -> Self {
         // Initialize runtime here
         get_runtime();
-        PythonCatalog(PersistenceCatalog::new(chunk_size))
+        Self::new(chunk_size)
     }
 
     pub fn add_file(
         mut slf: PyRefMut<'_, Self>,
         table_name: &str,
         file_path: &str,
         parquet_type: ParquetType,
     ) {
         let rt = get_runtime();
         let _guard = rt.enter();
 
         match parquet_type {
+            ParquetType::OrderBookSnapshot => {
+                match block_on(
+                    slf.add_file_default_query::<OrderBookSnapshot>(table_name, file_path),
+                ) {
+                    Ok(_) => (),
+                    Err(err) => panic!("Failed new_query with error {err}"),
+                }
+            }
+            ParquetType::OrderBookDelta => {
+                match block_on(slf.add_file_default_query::<OrderBookDelta>(table_name, file_path))
+                {
+                    Ok(_) => (),
+                    Err(err) => panic!("Failed new_query with error {err}"),
+                }
+            }
             ParquetType::QuoteTick => {
-                match block_on(slf.0.add_file::<QuoteTick>(table_name, file_path)) {
+                match block_on(slf.add_file_default_query::<QuoteTick>(table_name, file_path)) {
                     Ok(_) => (),
-                    Err(err) => panic!("failed new_query with error {}", err),
+                    Err(err) => panic!("Failed new_query with error {err}"),
                 }
             }
             ParquetType::TradeTick => {
-                match block_on(slf.0.add_file::<TradeTick>(table_name, file_path)) {
+                match block_on(slf.add_file_default_query::<TradeTick>(table_name, file_path)) {
                     Ok(_) => (),
-                    Err(err) => panic!("failed new_query with error {}", err),
+                    Err(err) => panic!("Failed new_query with error {err}"),
+                }
+            }
+            ParquetType::Bar => {
+                match block_on(slf.add_file_default_query::<Bar>(table_name, file_path)) {
+                    Ok(_) => (),
+                    Err(err) => panic!("Failed new_query with error {err}"),
                 }
             }
         }
     }
 
     pub fn add_file_with_query(
         mut slf: PyRefMut<'_, Self>,
@@ -221,52 +248,77 @@
         sql_query: &str,
         parquet_type: ParquetType,
     ) {
         let rt = get_runtime();
         let _guard = rt.enter();
 
         match parquet_type {
+            ParquetType::OrderBookSnapshot => {
+                match block_on(slf.add_file_with_custom_query::<OrderBookSnapshot>(
+                    table_name, file_path, sql_query,
+                )) {
+                    Ok(_) => (),
+                    Err(err) => panic!("Failed new_query with error {err}"),
+                }
+            }
+            ParquetType::OrderBookDelta => {
+                match block_on(
+                    slf.add_file_with_custom_query::<OrderBookDelta>(
+                        table_name, file_path, sql_query,
+                    ),
+                ) {
+                    Ok(_) => (),
+                    Err(err) => panic!("Failed new_query with error {err}"),
+                }
+            }
             ParquetType::QuoteTick => {
                 match block_on(
-                    slf.0
-                        .add_file_with_query::<QuoteTick>(table_name, file_path, sql_query),
+                    slf.add_file_with_custom_query::<QuoteTick>(table_name, file_path, sql_query),
                 ) {
                     Ok(_) => (),
-                    Err(err) => panic!("failed new_query with error {}", err),
+                    Err(err) => panic!("Failed new_query with error {err}"),
                 }
             }
             ParquetType::TradeTick => {
                 match block_on(
-                    slf.0
-                        .add_file_with_query::<TradeTick>(table_name, file_path, sql_query),
+                    slf.add_file_with_custom_query::<TradeTick>(table_name, file_path, sql_query),
+                ) {
+                    Ok(_) => (),
+                    Err(err) => panic!("Failed new_query with error {err}"),
+                }
+            }
+            ParquetType::Bar => {
+                match block_on(
+                    slf.add_file_with_custom_query::<Bar>(table_name, file_path, sql_query),
                 ) {
                     Ok(_) => (),
-                    Err(err) => panic!("failed new_query with error {}", err),
+                    Err(err) => panic!("Failed new_query with error {err}"),
                 }
             }
         }
     }
 
-    pub fn to_query_result(mut slf: PyRefMut<'_, Self>) -> PythonQueryResult {
+    #[must_use]
+    pub fn to_query_result(mut slf: PyRefMut<'_, Self>) -> DataQueryResult {
         let rt = get_runtime();
         let _guard = rt.enter();
 
-        let query_result = slf.0.to_query_result();
-        PythonQueryResult::new(query_result)
+        let query_result = slf.get_query_result();
+        DataQueryResult::new(query_result)
     }
 }
 
 #[pyclass]
-pub struct PythonQueryResult {
+pub struct DataQueryResult {
     result: QueryResult<Data>,
     chunk: Option<CVec>,
 }
 
 #[pymethods]
-impl PythonQueryResult {
+impl DataQueryResult {
     /// The reader implements an iterator.
     fn __iter__(slf: PyRef<'_, Self>) -> PyRef<'_, Self> {
         slf
     }
 
     /// Each iteration returns a chunk of values read from the parquet file.
     fn __next__(mut slf: PyRefMut<'_, Self>) -> Option<PyObject> {
@@ -279,32 +331,33 @@
             let cvec = chunk.into();
             Python::with_gil(|py| PyCapsule::new::<CVec>(py, cvec, None).unwrap().into_py(py))
         })
     }
 }
 
 // Note: Intended to be used on a single python thread
-unsafe impl Send for PythonQueryResult {}
+unsafe impl Send for DataQueryResult {}
 
-impl PythonQueryResult {
+impl DataQueryResult {
     fn new(result: QueryResult<Data>) -> Self {
         Self {
             result,
             chunk: None,
         }
     }
     /// Chunks generated by iteration must be dropped after use, otherwise
     /// it will leak memory. Current chunk is held by the reader,
     /// drop if exists and reset the field.
     fn drop_chunk(&mut self) {
         if let Some(CVec { ptr, len, cap }) = self.chunk.take() {
-            let data: Vec<Data> = unsafe { Vec::from_raw_parts(ptr as *mut Data, len, cap) };
+            let data: Vec<Data> =
+                unsafe { Vec::from_raw_parts(ptr.cast::<nautilus_model::data::Data>(), len, cap) };
             drop(data);
         }
     }
 }
 
-impl Drop for PythonQueryResult {
+impl Drop for DataQueryResult {
     fn drop(&mut self) {
         self.drop_chunk();
     }
 }
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/persistence/tests/test_catalog.rs` & `nautilus_trader-1.174.0/nautilus_core/persistence/tests/test_catalog.rs`

 * *Files 10% similar despite different names*

```diff
@@ -9,36 +9,29 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
-use nautilus_model::data::tick::{Data, QuoteTick, TradeTick};
-use nautilus_persistence::session::{PersistenceCatalog, QueryResult};
+use nautilus_model::data::tick::{QuoteTick, TradeTick};
+use nautilus_model::data::Data;
+use nautilus_persistence::session::{DataBackendSession, QueryResult};
 
-// Note: "current_thread" hangs up for some reason
+// Note: "current_thread" configuration hangs up for some reason
 #[tokio::test(flavor = "multi_thread")]
 async fn test_quote_ticks() {
-    let mut catalog = PersistenceCatalog::new(5000);
+    let file_path = "../../tests/test_data/quote_tick_data.parquet";
+    let length = 9500;
+    let mut catalog = DataBackendSession::new(10000);
     catalog
-        .add_file::<QuoteTick>(
-            "quote_tick",
-            "../../tests/test_data/quote_tick_data.parquet",
-        )
+        .add_file_default_query::<QuoteTick>("quotes_0005", file_path)
         .await
         .unwrap();
-    catalog
-        .add_file::<QuoteTick>(
-            "quote_tick_2",
-            "../../tests/test_data/quote_tick_data.parquet",
-        )
-        .await
-        .unwrap();
-    let query_result: QueryResult = catalog.to_query_result();
+    let query_result: QueryResult = catalog.get_query_result();
     let ticks: Vec<Data> = query_result.flatten().collect();
 
     // NOTE: is_sorted_by_key is unstable otherwise use
     // ticks.is_sorted_by_key(|tick| tick.ts_init)
     // https://github.com/rust-lang/rust/issues/53485
     let is_ascending_by_init = |ticks: &Vec<Data>| {
         for i in 1..ticks.len() {
@@ -47,41 +40,43 @@
             if ticks[i - 1].get_ts_init() > ticks[i].get_ts_init() {
                 return false;
             }
         }
         true
     };
 
-    match &ticks[0] {
-        Data::Trade(_) => assert!(false),
-        Data::Quote(q) => assert_eq!("EUR/USD.SIM", q.instrument_id.to_string()),
+    if let Data::Quote(q) = &ticks[0] {
+        assert_eq!("EUR/USD.SIM", q.instrument_id.to_string())
+    } else {
+        assert!(false)
     }
-    assert_eq!(ticks.len(), 19000);
+
+    assert_eq!(ticks.len(), length);
     assert!(is_ascending_by_init(&ticks));
 }
 
 // Note: "current_thread" hangs up for some reason
 #[tokio::test(flavor = "multi_thread")]
 async fn test_data_ticks() {
-    let mut catalog = PersistenceCatalog::new(5000);
+    let mut catalog = DataBackendSession::new(5000);
     catalog
-        .add_file::<QuoteTick>(
+        .add_file_default_query::<QuoteTick>(
             "quote_tick",
             "../../tests/test_data/quote_tick_data.parquet",
         )
         .await
         .unwrap();
     catalog
-        .add_file::<TradeTick>(
+        .add_file_default_query::<TradeTick>(
             "quote_tick_2",
             "../../tests/test_data/trade_tick_data.parquet",
         )
         .await
         .unwrap();
-    let query_result: QueryResult = catalog.to_query_result();
+    let query_result: QueryResult = catalog.get_query_result();
     let ticks: Vec<Data> = query_result.flatten().collect();
 
     // NOTE: is_sorted_by_key is unstable otherwise use
     // ticks.is_sorted_by_key(|tick| tick.ts_init)
     // https://github.com/rust-lang/rust/issues/53485
     let is_ascending_by_init = |ticks: &Vec<Data>| {
         for i in 1..ticks.len() {
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/persistence/tests/test_persistence_module.py` & `nautilus_trader-1.174.0/nautilus_core/persistence/tests/test_persistence_module.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,23 +12,23 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 # -------------------------------------------------------------------------------------------------
 
 import os
 
 from nautilus_trader import PACKAGE_ROOT
+from nautilus_trader.core.nautilus_pyo3.persistence import DataBackendSession
 from nautilus_trader.core.nautilus_pyo3.persistence import ParquetType
-from nautilus_trader.core.nautilus_pyo3.persistence import PythonCatalog
 from nautilus_trader.persistence.wranglers import list_from_capsule
 
 
 def test_python_catalog_data():
     trades_path = os.path.join(PACKAGE_ROOT, "tests/test_data/trade_tick_data.parquet")
     quotes_path = os.path.join(PACKAGE_ROOT, "tests/test_data/quote_tick_data.parquet")
-    session = PythonCatalog()
+    session = DataBackendSession()
     session.add_file("trade_ticks", trades_path, ParquetType.TradeTick)
     session.add_file("quote_ticks", quotes_path, ParquetType.QuoteTick)
     result = session.to_query_result()
 
     ticks = []
     for chunk in result:
         ticks.extend(list_from_capsule(chunk))
@@ -36,30 +36,30 @@
     assert len(ticks) == 9600
     is_ascending = all(ticks[i].ts_init <= ticks[i].ts_init for i in range(len(ticks) - 1))
     assert is_ascending
 
 
 def test_python_catalog_trades():
     trades_path = os.path.join(PACKAGE_ROOT, "tests/test_data/trade_tick_data.parquet")
-    session = PythonCatalog()
+    session = DataBackendSession()
     session.add_file("trade_ticks", trades_path, ParquetType.TradeTick)
     result = session.to_query_result()
 
     ticks = []
     for chunk in result:
         ticks.extend(list_from_capsule(chunk))
 
     assert len(ticks) == 100
     is_ascending = all(ticks[i].ts_init <= ticks[i].ts_init for i in range(len(ticks) - 1))
     assert is_ascending
 
 
 def test_python_catalog_quotes():
     parquet_data_path = os.path.join(PACKAGE_ROOT, "tests/test_data/quote_tick_data.parquet")
-    session = PythonCatalog()
+    session = DataBackendSession()
     session.add_file("quote_ticks", parquet_data_path, ParquetType.QuoteTick)
     result = session.to_query_result()
 
     ticks = []
     for chunk in result:
         ticks.extend(list_from_capsule(chunk))
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/persistence/tests/test_util.rs` & `nautilus_trader-1.174.0/nautilus_core/persistence/tests/test_util.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_core/pyo3/Cargo.toml` & `nautilus_trader-1.174.0/nautilus_core/pyo3/Cargo.toml`

 * *Files 18% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 name = "nautilus_pyo3"
 crate-type = ["cdylib"]
 
 [dependencies]
 nautilus_indicators = { path = "../indicators" }
 nautilus_model = { path = "../model" }
 nautilus_persistence = { path = "../persistence" }
+nautilus_network = { path = "../network" }
 pyo3.workspace = true
 
 [features]
 extension-module = [
     "pyo3/extension-module",
     "nautilus_indicators/extension-module",
     "nautilus_model/extension-module",
```

### Comparing `nautilus_trader-1.173.0/nautilus_core/pyo3/src/lib.rs` & `nautilus_trader-1.174.0/nautilus_core/pyo3/src/lib.rs`

 * *Files 18% similar despite different names*

```diff
@@ -38,9 +38,20 @@
     m.add_wrapped(submodule)?;
     let sys = PyModule::import(py, "sys")?;
     let sys_modules: &PyDict = sys.getattr("modules")?.downcast()?;
     sys_modules.set_item(
         "nautilus_trader.core.nautilus_pyo3.model",
         m.getattr("model")?,
     )?;
+
+    // Network
+    let submodule = pyo3::wrap_pymodule!(nautilus_network::nautilus_network);
+    m.add_wrapped(submodule)?;
+    let sys = PyModule::import(py, "sys")?;
+    let sys_modules: &PyDict = sys.getattr("modules")?.downcast()?;
+    sys_modules.set_item(
+        "nautilus_trader.core.nautilus_pyo3.network",
+        m.getattr("nautilus_network")?,
+    )?;
+
     Ok(())
 }
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/__init__.pxd` & `nautilus_trader-1.174.0/nautilus_trader/accounting/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/accounting/__init__.pxd` & `nautilus_trader-1.174.0/nautilus_trader/accounting/accounts/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/accounting/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/accounting/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/accounting/accounts/__init__.pxd` & `nautilus_trader-1.174.0/nautilus_trader/accounting/accounts/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/accounting/accounts/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/_template/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/accounting/accounts/base.pxd` & `nautilus_trader-1.174.0/nautilus_trader/accounting/accounts/base.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/accounting/accounts/base.pyx` & `nautilus_trader-1.174.0/nautilus_trader/accounting/accounts/base.pyx`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 # -------------------------------------------------------------------------------------------------
 
 from typing import Optional
 
+from nautilus_trader.accounting.error import AccountBalanceNegative
+
 from nautilus_trader.core.correctness cimport Condition
 from nautilus_trader.model.enums_c cimport AccountType
 from nautilus_trader.model.enums_c cimport account_type_to_str
 from nautilus_trader.model.events.account cimport AccountState
 from nautilus_trader.model.instruments.base cimport Instrument
 from nautilus_trader.model.objects cimport AccountBalance
 
@@ -401,21 +403,17 @@
         """
         Condition.not_empty(balances, "balances")
 
         cdef AccountBalance balance
         for balance in balances:
             if not balance.total._mem.raw > 0:
                 if balance.total._mem.raw < 0:
-                    raise RuntimeError(
-                        f"account blow up (balance was {balance.total}).",
-                    )
+                    raise AccountBalanceNegative(balance.total.as_decimal(), balance.currency)
                 if balance.total.is_zero() and not allow_zero:
-                    raise RuntimeError(
-                        f"account blow up (balance was {balance.total}).",
-                    )
+                    raise AccountBalanceNegative(balance.total.as_decimal(), balance.currency)
                 else:
                     # Clear asset balance
                     self._balances.pop(balance.currency, None)
             self._balances[balance.currency] = balance
 
     cpdef void update_commissions(self, Money commission):
         """
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/accounting/accounts/betting.pxd` & `nautilus_trader-1.174.0/nautilus_trader/accounting/accounts/betting.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/accounting/accounts/betting.pyx` & `nautilus_trader-1.174.0/nautilus_trader/accounting/accounts/betting.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/accounting/accounts/cash.pxd` & `nautilus_trader-1.174.0/nautilus_trader/accounting/accounts/cash.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/accounting/accounts/cash.pyx` & `nautilus_trader-1.174.0/nautilus_trader/accounting/accounts/cash.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -287,15 +287,15 @@
         fill : OrderFilled
             The fill for the calculation.
         position : Position, optional
             The position for the calculation (can be None).
 
         Returns
         -------
-        list[Money] or ``None``
+        list[Money]
 
         """
         Condition.not_none(instrument, "instrument")
         Condition.not_none(fill, "fill")
 
         cdef dict pnls = {}  # type: dict[Currency, Money]
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/accounting/accounts/margin.pxd` & `nautilus_trader-1.174.0/nautilus_trader/accounting/accounts/margin.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/accounting/accounts/margin.pyx` & `nautilus_trader-1.174.0/nautilus_trader/accounting/accounts/margin.pyx`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 # -------------------------------------------------------------------------------------------------
 
 from decimal import Decimal
 from typing import Optional
 
+from nautilus_trader.accounting.error import AccountMarginExceeded
+
 from nautilus_trader.core.correctness cimport Condition
 from nautilus_trader.model.currency cimport Currency
 from nautilus_trader.model.enums_c cimport AccountType
 from nautilus_trader.model.enums_c cimport LiquiditySide
 from nautilus_trader.model.enums_c cimport liquidity_side_to_str
 from nautilus_trader.model.events.account cimport AccountState
 from nautilus_trader.model.events.order cimport OrderFilled
@@ -411,31 +413,38 @@
     cpdef bint is_unleveraged(self, InstrumentId instrument_id):
         Condition.not_none(instrument_id, "instrument_id")
         return self._leverages.get(instrument_id, self.default_leverage) == 1
 
     cdef void _recalculate_balance(self, Currency currency):
         cdef AccountBalance current_balance = self._balances.get(currency)
         if current_balance is None:
-            # TODO(cs): Temporary pending reimplementation of accounting
-            print("Cannot recalculate balance when no current balance")
-            return
+            raise RuntimeError("cannot recalculate balance when no current balance")
 
         cdef double total_margin = 0.0
 
         cdef MarginBalance margin
         for margin in self._margins.values():
             if margin.currency != currency:
                 continue
             total_margin += margin.initial.as_f64_c()
             total_margin += margin.maintenance.as_f64_c()
 
+        cdef double total_free = current_balance.total.as_f64_c() - total_margin
+
+        if total_free <= 0.0:
+            raise AccountMarginExceeded(
+                balance=current_balance.total.as_decimal(),
+                margin=Money(total_margin, currency).as_decimal(),
+                currency=currency,
+            )
+
         cdef AccountBalance new_balance = AccountBalance(
             current_balance.total,
             Money(total_margin, currency),
-            Money(current_balance.total.as_f64_c() - total_margin, currency),
+            Money(total_free, currency),
         )
 
         self._balances[currency] = new_balance
 
     cpdef Money calculate_commission(
         self,
         Instrument instrument,
@@ -626,15 +635,15 @@
         fill : OrderFilled
             The fill for the calculation.
         position : Position, optional
             The position for the calculation.
 
         Returns
         -------
-        list[Money] or ``None``
+        list[Money]
 
         """
         Condition.not_none(instrument, "instrument")
         Condition.not_none(fill, "fill")
 
         cdef dict pnls = {}  # type: dict[Currency, Money]
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/accounting/calculators.pxd` & `nautilus_trader-1.174.0/nautilus_trader/accounting/calculators.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/accounting/calculators.pyx` & `nautilus_trader-1.174.0/nautilus_trader/accounting/calculators.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/accounting/error.py` & `nautilus_trader-1.174.0/nautilus_trader/model/orderbook/error.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,22 +9,12 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 # -------------------------------------------------------------------------------------------------
 
-from decimal import Decimal
 
-
-class AccountBalanceNegative(Exception):
+class BookIntegrityError(Exception):
     """
-    Represents a negative account balance error.
+    Represents an error condition where the order books integrity has been lost.
     """
-
-    def __init__(self, balance: Decimal):
-        super().__init__()
-
-        self.balance = balance
-
-    def __str__(self) -> str:
-        return f"AccountBalanceNegative(balance={self.balance}"
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/accounting/factory.pxd` & `nautilus_trader-1.174.0/nautilus_trader/accounting/factory.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/accounting/factory.pyx` & `nautilus_trader-1.174.0/nautilus_trader/accounting/factory.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/accounting/manager.pxd` & `nautilus_trader-1.174.0/nautilus_trader/accounting/manager.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/accounting/manager.pyx` & `nautilus_trader-1.174.0/nautilus_trader/accounting/manager.pyx`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 # -------------------------------------------------------------------------------------------------
 
 from libc.stdint cimport uint64_t
 
+from nautilus_trader.accounting.error import AccountBalanceNegative
+from nautilus_trader.accounting.error import AccountMarginExceeded
+
 from nautilus_trader.accounting.accounts.base cimport Account
 from nautilus_trader.accounting.accounts.cash cimport CashAccount
 from nautilus_trader.accounting.accounts.margin cimport MarginAccount
 from nautilus_trader.cache.base cimport CacheFacade
 from nautilus_trader.common.clock cimport Clock
 from nautilus_trader.common.logging cimport LoggerAdapter
 from nautilus_trader.core.correctness cimport Condition
@@ -510,14 +513,16 @@
         cdef Money commission = fill.commission
         cdef AccountBalance balance = None
         cdef AccountBalance new_balance = None
         cdef:
             Money pnl
             double new_total
             double new_free
+            Money total
+            Money free
         for pnl in pnls:
             currency = pnl.currency
             if commission.currency != currency and commission._mem.raw != 0:
                 balance = account.balance(commission.currency)
                 if balance is None:
                     if commission._mem.raw > 0:
                         self._log.error(
@@ -552,33 +557,33 @@
                     total=pnl,
                     locked=Money(0, pnl.currency),
                     free=pnl,
                 )
             else:
                 new_total = balance.total.as_f64_c() + pnl.as_f64_c()
                 new_free = balance.free.as_f64_c() + pnl.as_f64_c()
+                total = Money(new_total, pnl.currency)
+                free = Money(new_free, pnl.currency)
                 if new_total < 0:
-                    self._log.error(
-                        "Cannot complete transaction: "
-                        f"{balance.total.to_str()} total balance is insufficient to deduct a "
-                        f"{pnl.to_str()} realized PnL from."
+                    raise AccountBalanceNegative(
+                        balance=total.as_decimal(),
+                        currency=pnl.currency,
                     )
-                    return
-                if new_free < 0:
-                    self._log.error(
-                        "Cannot complete transaction: "
-                        f"{balance.free.to_str()} free balance is insufficient to deduct a "
-                        f"{pnl.to_str()} realized PnL from."
+                if new_free <= 0:
+                    raise AccountMarginExceeded(
+                        balance=total.as_decimal(),
+                        margin=balance.locked.as_decimal(),
+                        currency=pnl.currency,
                     )
-                    return
+
                 # Calculate new balance
                 new_balance = AccountBalance(
-                    total=Money(new_total, pnl.currency),
+                    total=total,
                     locked=balance.locked,
-                    free=Money(new_free, pnl.currency),
+                    free=free,
                 )
 
             balances.append(new_balance)
 
         # TODO(cs): Refactor and consolidate
         if not pnls and commission._mem.raw != 0:
             currency = commission.currency
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/_template/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/betfair/client/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/_template/core.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/_template/core.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/_template/data.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/_template/data.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/_template/execution.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/_template/execution.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/_template/providers.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/_template/providers.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/betfair/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/betfair/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/betfair/client/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/betfair/parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/betfair/client/core.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/betfair/client/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,15 +111,15 @@
                 return data["result"]
             else:
                 raise TypeError("Unexpected type:" + str(resp))
         except BetfairError as e:
             self._log.error(str(e))
             raise e
         except ClientResponseError as e:
-            self._log.error(f"Err on {method} status={e.status}, message={str(e)}")
+            self._log.error(f"Err on {method} status={e.status}, message={e!s}")
             raise e
 
     async def connect(self):
         await super().connect()
         await self.login()
 
     async def disconnect(self):
@@ -131,18 +131,16 @@
     async def login(self):
         self._log.debug("BetfairClient login")
         if self.session_token is not None:
             self._log.warning("Already logged in, returning")
             return
         url = self.IDENTITY_URL + "certlogin"
         data = {"username": self.username, "password": self.password}
-        headers = {
-            **{k: v for k, v in self.headers.items() if k not in ("content-type",)},
-            **{"Content-Type": "application/x-www-form-urlencoded"},
-        }
+        headers = {k: v for k, v in self.headers.items() if k.lower() != "content-type"}
+        headers["Content-Type"] = "application/x-www-form-urlencoded"
         resp = await self.post(url=url, data=data, headers=headers)
         data = msgspec.json.decode(resp.data)
         if data["loginStatus"] == "SUCCESS":
             self.session_token = data["sessionToken"]
         else:
             raise BetfairError(f"Login failed: {resp.data}")
 
@@ -165,15 +163,15 @@
         Return specific data about markets.
         """
         assert 0 < max_results <= 1000
 
         params = parse_params(**locals())
 
         if "marketProjection" in params:
-            assert all([isinstance(m, MarketProjection) for m in params["marketProjection"]])
+            assert all(isinstance(m, MarketProjection) for m in params["marketProjection"])
             params["marketProjection"] = [m.value for m in params["marketProjection"]]
         if "sort" in params:
             assert isinstance(sort, MarketSort)
         resp = await self.rpc_post(
             url=self.BETTING_URL,
             method="SportsAPING/v1.0/listMarketCatalogue",
             params=params,
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/betfair/client/enums.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/betfair/client/enums.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/betfair/client/exceptions.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/betfair/client/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,16 +15,14 @@
 
 
 class BetfairError(Exception):
     """
     The base class for all `Betfair` specific errors.
     """
 
-    pass
-
 
 class BetfairAPIError(BetfairError):
     """
     Represents a `Betfair` API specific error.
     """
 
     def __init__(self, code: str, message: str):
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/betfair/client/spec.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/betfair/client/spec.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/betfair/client/util.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/betfair/client/util.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/betfair/common.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/betfair/common.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/betfair/config.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/betfair/config.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/betfair/constants.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/betfair/constants.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/betfair/data.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/betfair/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,15 +171,15 @@
     async def _subscribe_order_book_deltas(
         self,
         instrument_id: InstrumentId,
         book_type: BookType,
         depth: Optional[int] = None,
         kwargs: Optional[dict] = None,
     ):
-        PyCondition.not_none(instrument_id, "instrument_id")  # noqa
+        PyCondition.not_none(instrument_id, "instrument_id")
 
         instrument: BettingInstrument = self._instrument_provider.find(instrument_id)
 
         if instrument.market_id in self._subscribed_market_ids:
             self._log.warning(
                 f"Already subscribed to market_id: {instrument.market_id} "
                 f"[Instrument: {instrument_id.symbol}] <OrderBook> data.",
@@ -204,15 +204,15 @@
         )
 
     async def delayed_subscribe(self, delay=0):
         self._log.debug(f"Scheduling subscribe for delay={delay}")
         await asyncio.sleep(delay)
         self._log.info(f"Sending subscribe for market_ids {self._subscribed_market_ids}")
         await self._stream.send_subscription_message(market_ids=list(self._subscribed_market_ids))
-        self._log.info(f"Added market_ids {self._subscribed_market_ids} for <OrderBookData> data.")
+        self._log.info(f"Added market_ids {self._subscribed_market_ids} for <OrderBook> data.")
 
     async def _subscribe_ticker(self, instrument_id: InstrumentId) -> None:
         pass  # Subscribed as part of orderbook
 
     async def _subscribe_trade_ticks(self, instrument_id: InstrumentId) -> None:
         pass  # Subscribed as part of orderbook
 
@@ -264,22 +264,21 @@
                 # Not a regular data type
                 generic_data = GenericData(
                     DataType(data.__class__, {"instrument_id": data.instrument_id}),
                     data,
                 )
                 self._handle_data(generic_data)
             elif isinstance(data, Data):
-                if self._strict_handling:
-                    if (
-                        hasattr(data, "instrument_id")
-                        and data.instrument_id not in self._subscribed_instrument_ids
-                    ):
-                        # We receive data for multiple instruments within a subscription, don't emit data if we're not
-                        # subscribed to this particular instrument as this will trigger a bunch of error logs
-                        continue
+                if self._strict_handling and (
+                    hasattr(data, "instrument_id")
+                    and data.instrument_id not in self._subscribed_instrument_ids
+                ):
+                    # We receive data for multiple instruments within a subscription, don't emit data if we're not
+                    # subscribed to this particular instrument as this will trigger a bunch of error logs
+                    continue
                 self._handle_data(data)
             elif isinstance(data, Event):
                 self._log.warning(
                     f"Received event: {data}, DataEngine not yet setup to send events",
                 )
             else:
                 raise RuntimeError
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/betfair/data_types.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/betfair/data_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,39 +11,38 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 # -------------------------------------------------------------------------------------------------
 
 import copy
 from enum import Enum
+from typing import Optional
 
 import pyarrow as pa
 
+# fmt: off
 from nautilus_trader.core.correctness import PyCondition
 from nautilus_trader.core.data import Data
+from nautilus_trader.model.data.book import BookOrder
+from nautilus_trader.model.data.book import OrderBookDelta
+from nautilus_trader.model.data.book import OrderBookDeltas
 from nautilus_trader.model.data.ticker import Ticker
 from nautilus_trader.model.enums import BookAction
 from nautilus_trader.model.enums import book_action_from_str
-from nautilus_trader.model.enums import book_type_from_str
 from nautilus_trader.model.identifiers import InstrumentId
-from nautilus_trader.model.orderbook.data import BookOrder
-from nautilus_trader.model.orderbook.data import OrderBookData
-from nautilus_trader.model.orderbook.data import OrderBookDelta
-from nautilus_trader.model.orderbook.data import OrderBookDeltas
-from nautilus_trader.serialization.arrow.implementations.order_book import (
-    deserialize as deserialize_orderbook,
-)
-from nautilus_trader.serialization.arrow.implementations.order_book import (
-    serialize as serialize_orderbook,
-)
+from nautilus_trader.serialization.arrow.implementations.order_book import deserialize as deserialize_orderbook
+from nautilus_trader.serialization.arrow.implementations.order_book import serialize as serialize_orderbook
 from nautilus_trader.serialization.arrow.schema import NAUTILUS_PARQUET_SCHEMA
 from nautilus_trader.serialization.arrow.serializer import register_parquet
 from nautilus_trader.serialization.base import register_serializable_object
 
 
+# fmt: on
+
+
 class SubscriptionStatus(Enum):
     """
     Represents a `Betfair` subscription status.
     """
 
     UNSUBSCRIBED = 0
     PENDING_STARTUP = 1
@@ -75,15 +74,14 @@
                 },
             )
             if values["action"] != "CLEAR"
             else None
         )
         return BSPOrderBookDelta(
             instrument_id=InstrumentId.from_str(values["instrument_id"]),
-            book_type=book_type_from_str(values["book_type"]),
             action=action,
             order=order,
             ts_event=values["ts_event"],
             ts_init=values["ts_init"],
         )
 
     @staticmethod
@@ -99,18 +97,18 @@
     """
 
     def __init__(
         self,
         instrument_id: InstrumentId,
         ts_event: int,
         ts_init: int,
-        last_traded_price: float = None,
-        traded_volume: float = None,
-        starting_price_near: float = None,
-        starting_price_far: float = None,
+        last_traded_price: Optional[float] = None,
+        traded_volume: Optional[float] = None,
+        starting_price_near: Optional[float] = None,
+        starting_price_far: Optional[float] = None,
     ):
         super().__init__(instrument_id=instrument_id, ts_event=ts_event, ts_init=ts_init)
         self.last_traded_price = last_traded_price
         self.traded_volume = traded_volume
         self.starting_price_near = starting_price_near
         self.starting_price_far = starting_price_far
 
@@ -214,15 +212,15 @@
     BetfairStartingPrice,
     BetfairStartingPrice.to_dict,
     BetfairStartingPrice.from_dict,
 )
 register_parquet(cls=BetfairStartingPrice, schema=BetfairStartingPrice.schema())
 
 # Register serialization/parquet BSPOrderBookDeltas
-BSP_ORDERBOOK_SCHEMA: pa.Schema = copy.copy(NAUTILUS_PARQUET_SCHEMA[OrderBookData])
+BSP_ORDERBOOK_SCHEMA: pa.Schema = copy.copy(NAUTILUS_PARQUET_SCHEMA[OrderBookDelta])
 BSP_ORDERBOOK_SCHEMA = BSP_ORDERBOOK_SCHEMA.with_metadata({"type": "BSPOrderBookDelta"})
 
 register_serializable_object(
     BSPOrderBookDeltas,
     BSPOrderBookDeltas.to_dict,
     BSPOrderBookDeltas.from_dict,
 )
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/betfair/execution.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/betfair/execution.py`

 * *Files 0% similar despite different names*

```diff
@@ -648,15 +648,15 @@
                         )
                     else:
                         self._log.warning(f"Unknown order state: {unmatched_order}")
                 if selection.fullImage:
                     self.check_cache_against_order_image(order_change_message)
                     continue
 
-    def check_cache_against_order_image(self, order_change_message: OCM) -> None:  # noqa
+    def check_cache_against_order_image(self, order_change_message: OCM) -> None:
         for market in order_change_message.oc:
             for selection in market.orc:
                 instrument_id = betfair_instrument_id(
                     market_id=market.id,
                     selection_id=str(selection.id),
                     selection_handicap=selection.hc,
                 )
@@ -675,21 +675,20 @@
                 for side, matched_order in matched_orders:
                     # We don't get much information from Betfair here, try our best to match order
                     price = betfair_float_to_price(matched_order.price)
                     quantity = betfair_float_to_quantity(matched_order.size)
                     matched = False
                     for order in orders:
                         for event in order.events:
-                            if isinstance(event, OrderFilled):
-                                if (
-                                    order.side == side
-                                    and order.price == price
-                                    and quantity <= order.quantity
-                                ):
-                                    matched = True
+                            if isinstance(event, OrderFilled) and (
+                                order.side == side
+                                and order.price == price
+                                and quantity <= order.quantity
+                            ):
+                                matched = True
                     if not matched:
                         self._log.error(f"UNKNOWN FILL: {instrument_id=} {matched_order}")
                         raise RuntimeError(f"UNKNOWN FILL: {instrument_id=} {matched_order}")
 
     async def _check_order_update(self, unmatched_order: UnmatchedOrder) -> None:
         """
         Ensure we have a client_order_id, instrument and order for this venue order update
@@ -840,18 +839,19 @@
             key = (client_order_id, venue_order_id)
             self._log.debug(
                 f"cancel key: {key}, pending_update_order_client_ids: {self.pending_update_order_client_ids}",
             )
             if key not in self.pending_update_order_client_ids:
                 # The remainder of this order has been canceled
                 cancelled_ts = unmatched_order.cd or unmatched_order.ld or unmatched_order.md
-                if cancelled_ts is not None:
-                    cancelled_ts = millis_to_nanos(cancelled_ts)
-                else:
-                    cancelled_ts = self._clock.timestamp_ns()
+                cancelled_ts = (
+                    millis_to_nanos(cancelled_ts)
+                    if cancelled_ts is not None
+                    else self._clock.timestamp_ns()
+                )
                 self.generate_order_canceled(
                     strategy_id=order.strategy_id,
                     instrument_id=instrument.id,
                     client_order_id=client_order_id,
                     venue_order_id=venue_order_id,
                     ts_event=cancelled_ts,
                 )
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/betfair/factories.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/betfair/factories.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/betfair/historic.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/betfair/historic.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/betfair/orderbook.pxd` & `nautilus_trader-1.174.0/nautilus_trader/adapters/betfair/orderbook.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/betfair/orderbook.pyx` & `nautilus_trader-1.174.0/nautilus_trader/adapters/betfair/orderbook.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/betfair/parsing/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/binance/common/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/betfair/parsing/common.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/betfair/parsing/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from nautilus_trader.adapters.betfair.common import BETFAIR_VENUE
 from nautilus_trader.core.correctness import PyCondition
 from nautilus_trader.model.identifiers import InstrumentId
 from nautilus_trader.model.identifiers import Symbol
 
 
 def hash_market_trade(timestamp: int, price: float, volume: float):
-    return f"{str(timestamp)[:-6]}{price}{str(volume)}"
+    return f"{str(timestamp)[:-6]}{price}{volume!s}"
 
 
 def make_symbol(
     market_id: str,
     selection_id: str,
     selection_handicap: Optional[str],
 ) -> Symbol:
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/betfair/parsing/core.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/betfair/parsing/core.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/betfair/parsing/requests.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/betfair/parsing/requests.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/betfair/parsing/streaming.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/betfair/parsing/streaming.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 from betfair_parser.spec.streaming.mcm import MarketDefinition
 from betfair_parser.spec.streaming.mcm import Runner
 from betfair_parser.spec.streaming.mcm import RunnerChange
 from betfair_parser.spec.streaming.mcm import RunnerStatus
 
 from nautilus_trader.adapters.betfair.client.spec import ClearedOrder
 from nautilus_trader.adapters.betfair.common import B2N_MARKET_STREAM_SIDE
-from nautilus_trader.adapters.betfair.constants import BETFAIR_BOOK_TYPE
 from nautilus_trader.adapters.betfair.constants import CLOSE_PRICE_LOSER
 from nautilus_trader.adapters.betfair.constants import CLOSE_PRICE_WINNER
 from nautilus_trader.adapters.betfair.constants import MARKET_STATUS_MAPPING
 from nautilus_trader.adapters.betfair.constants import STRICT_MARKET_DATA_HANDLING
 from nautilus_trader.adapters.betfair.constants import MarketDataKind
 from nautilus_trader.adapters.betfair.data_types import BetfairStartingPrice
 from nautilus_trader.adapters.betfair.data_types import BetfairTicker
@@ -39,33 +38,32 @@
 from nautilus_trader.adapters.betfair.orderbook import betfair_float_to_price
 from nautilus_trader.adapters.betfair.orderbook import betfair_float_to_quantity
 from nautilus_trader.adapters.betfair.parsing.common import betfair_instrument_id
 from nautilus_trader.adapters.betfair.parsing.common import hash_market_trade
 from nautilus_trader.adapters.betfair.parsing.requests import parse_handicap
 from nautilus_trader.common.functions import one
 from nautilus_trader.execution.reports import TradeReport
+from nautilus_trader.model.data.book import BookOrder
+from nautilus_trader.model.data.book import OrderBookDelta
+from nautilus_trader.model.data.book import OrderBookDeltas
+from nautilus_trader.model.data.book import OrderBookSnapshot
 from nautilus_trader.model.data.tick import TradeTick
 from nautilus_trader.model.data.venue import InstrumentClose
 from nautilus_trader.model.data.venue import InstrumentStatusUpdate
 from nautilus_trader.model.enums import AggressorSide
 from nautilus_trader.model.enums import BookAction
-from nautilus_trader.model.enums import BookType
 from nautilus_trader.model.enums import InstrumentCloseType
 from nautilus_trader.model.enums import LiquiditySide
 from nautilus_trader.model.enums import MarketStatus
 from nautilus_trader.model.enums import OrderSide
 from nautilus_trader.model.identifiers import AccountId
 from nautilus_trader.model.identifiers import InstrumentId
 from nautilus_trader.model.identifiers import Symbol
 from nautilus_trader.model.identifiers import TradeId
 from nautilus_trader.model.identifiers import VenueOrderId
-from nautilus_trader.model.orderbook.data import BookOrder
-from nautilus_trader.model.orderbook.data import OrderBookDelta
-from nautilus_trader.model.orderbook.data import OrderBookDeltas
-from nautilus_trader.model.orderbook.data import OrderBookSnapshot
 
 
 PARSE_TYPES = Union[
     InstrumentStatusUpdate,
     InstrumentClose,
     OrderBookSnapshot,
     OrderBookDeltas,
@@ -322,30 +320,28 @@
 def runner_change_all_depth_to_order_book_snapshot(
     rc: RunnerChange,
     instrument_id: InstrumentId,
     ts_event: int,
     ts_init: int,
 ) -> Optional[OrderBookSnapshot]:
     # ATL = Available To Lay = Back orders
-    if rc.atl:
-        asks = [
-            (betfair_float_to_price(order.price), order.volume) for order in rc.atl if order.price
-        ]
-    else:
-        asks = []
+    asks = (
+        [(betfair_float_to_price(order.price), order.volume) for order in rc.atl if order.price]
+        if rc.atl
+        else []
+    )
     # Asks are available to back (atb)
     if rc.atb:
         bids: list = [
             (betfair_float_to_price(order.price), order.volume) for order in rc.atb if order.price
         ]
     else:
         bids = []
 
     return OrderBookSnapshot(
-        book_type=BookType.L2_MBP,
         instrument_id=instrument_id,
         bids=bids,
         asks=asks,
         ts_event=ts_event,
         ts_init=ts_init,
     )
 
@@ -368,15 +364,14 @@
     if rc.batb:
         bids: list = [
             (betfair_float_to_price(order.price), order.volume) for order in rc.batb if order.price
         ]
     else:
         bids = []
     return OrderBookSnapshot(
-        book_type=BookType.L2_MBP,
         instrument_id=instrument_id,
         bids=bids,
         asks=asks,
         ts_event=ts_event,
         ts_init=ts_init,
     )
 
@@ -384,29 +379,27 @@
 def runner_change_display_depth_to_order_book_snapshot(
     rc: RunnerChange,
     instrument_id: InstrumentId,
     ts_event: int,
     ts_init: int,
 ) -> Optional[OrderBookSnapshot]:
     # Bids are best display available to lay (bdatl)
-    if rc.bdatl:
-        asks = [
-            (betfair_float_to_price(order.price), order.volume) for order in rc.bdatl if order.price
-        ]
-    else:
-        asks = []
+    asks = (
+        [(betfair_float_to_price(order.price), order.volume) for order in rc.bdatl if order.price]
+        if rc.bdatl
+        else []
+    )
     # Asks are best display available to back (bdatb)
     if rc.bdatb:
         bids: list = [
             (betfair_float_to_price(order.price), order.volume) for order in rc.bdatb if order.price
         ]
     else:
         bids = []
     return OrderBookSnapshot(
-        book_type=BookType.L2_MBP,
         instrument_id=instrument_id,
         bids=bids,
         asks=asks,
         ts_event=ts_event,
         ts_init=ts_init,
     )
 
@@ -446,15 +439,14 @@
 
     # Bids are available to lay (atl)
     if rc.atl:
         deltas.extend(
             [
                 OrderBookDelta(
                     instrument_id,
-                    BETFAIR_BOOK_TYPE,
                     BookAction.UPDATE if back.volume != 0.0 else BookAction.DELETE,
                     BookOrder(back.price, back.volume, OrderSide.SELL),
                     ts_event,
                     ts_init,
                 )
                 for back in rc.atl
             ],
@@ -462,27 +454,25 @@
 
     # Asks are available to back (atb)
     if rc.atb:
         deltas.extend(
             [
                 OrderBookDelta(
                     instrument_id,
-                    BETFAIR_BOOK_TYPE,
                     BookAction.UPDATE if lay.volume != 0.0 else BookAction.DELETE,
                     BookOrder(lay.price, lay.volume, OrderSide.BUY),
                     ts_event,
                     ts_init,
                 )
                 for lay in rc.atb
             ],
         )
     if not deltas:
         return None
     return OrderBookDeltas(
-        book_type=BookType.L2_MBP,
         instrument_id=instrument_id,
         deltas=deltas,
         ts_event=ts_event,
         ts_init=ts_init,
     )
 
 
@@ -496,15 +486,14 @@
 
     # Bids are best available to lay (batl)
     if rc.batl:
         deltas.extend(
             [
                 OrderBookDelta(
                     instrument_id,
-                    BETFAIR_BOOK_TYPE,
                     BookAction.UPDATE if back.volume != 0.0 else BookAction.DELETE,
                     BookOrder(back.price, back.volume, OrderSide.SELL),
                     ts_event,
                     ts_init,
                 )
                 for back in rc.batl
             ],
@@ -512,27 +501,25 @@
 
     # Asks are best available to back (batb)
     if rc.batb:
         deltas.extend(
             [
                 OrderBookDelta(
                     instrument_id,
-                    BETFAIR_BOOK_TYPE,
                     BookAction.UPDATE if lay.volume != 0.0 else BookAction.DELETE,
                     BookOrder(lay.price, lay.volume, OrderSide.BUY),
                     ts_event,
                     ts_init,
                 )
                 for lay in rc.batb
             ],
         )
     if not deltas:
         return None
     return OrderBookDeltas(
-        book_type=BookType.L2_MBP,
         instrument_id=instrument_id,
         deltas=deltas,
         ts_event=ts_event,
         ts_init=ts_init,
     )
 
 
@@ -546,15 +533,14 @@
 
     # Bids are best display available to lay (bdatl)
     if rc.bdatl:
         deltas.extend(
             [
                 OrderBookDelta(
                     instrument_id,
-                    BETFAIR_BOOK_TYPE,
                     BookAction.UPDATE if back.volume != 0.0 else BookAction.DELETE,
                     BookOrder(back.price, back.volume, OrderSide.SELL),
                     ts_event,
                     ts_init,
                 )
                 for back in rc.bdatl
             ],
@@ -562,27 +548,25 @@
 
     # Asks are best display available to back (bdatb)
     if rc.bdatb:
         deltas.extend(
             [
                 OrderBookDelta(
                     instrument_id,
-                    BETFAIR_BOOK_TYPE,
                     BookAction.UPDATE if lay.volume != 0.0 else BookAction.DELETE,
                     BookOrder(lay.price, lay.volume, OrderSide.BUY),
                     ts_event,
                     ts_init,
                 )
                 for lay in rc.bdatb
             ],
         )
     if not deltas:
         return None
     return OrderBookDeltas(
-        book_type=BookType.L2_MBP,
         instrument_id=instrument_id,
         deltas=deltas,
         ts_event=ts_event,
         ts_init=ts_init,
     )
 
 
@@ -647,15 +631,14 @@
     price: float,
     volume: float,
     ts_event: int,
     ts_init: int,
 ) -> BSPOrderBookDelta:
     return BSPOrderBookDelta(
         instrument_id=bsp_instrument_id,
-        book_type=BookType.L2_MBP,
         action=BookAction.DELETE if volume == 0 else BookAction.UPDATE,
         order=BookOrder(
             price=betfair_float_to_price(price),
             size=betfair_float_to_quantity(volume),
             side=B2N_MARKET_STREAM_SIDE[side],
         ),
         ts_event=ts_event,
@@ -694,35 +677,32 @@
                 ts_event,
                 ts_init,
             ),
         )
 
     return BSPOrderBookDeltas(
         instrument_id=bsp_instrument_id,
-        book_type=BookType.L2_MBP,
         deltas=deltas,
         ts_event=ts_event,
         ts_init=ts_init,
     )
 
 
 def _merge_order_book_deltas(all_deltas: list[OrderBookDeltas]):
     cls = type(all_deltas[0])
     per_instrument_deltas = defaultdict(list)
-    book_type = one({deltas.book_type for deltas in all_deltas})
     ts_event = one({deltas.ts_event for deltas in all_deltas})
     ts_init = one({deltas.ts_init for deltas in all_deltas})
 
     for deltas in all_deltas:
         per_instrument_deltas[deltas.instrument_id].extend(deltas.deltas)
     return [
         cls(
             instrument_id=instrument_id,
             deltas=deltas,
-            book_type=book_type,
             ts_event=ts_event,
             ts_init=ts_init,
         )
         for instrument_id, deltas in per_instrument_deltas.items()
     ]
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/betfair/providers.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/betfair/providers.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
     def search_instruments(self, instrument_filter: Optional[dict] = None):
         """Search for instruments within the cache. Useful for debugging / interactive use"""
         instruments = self.list_all()
         if instrument_filter:
             instruments = [
                 ins
                 for ins in instruments
-                if all([getattr(ins, k) == v for k, v in instrument_filter.items()])
+                if all(getattr(ins, k) == v for k, v in instrument_filter.items())
             ]
         return instruments
 
     def get_betting_instrument(
         self,
         market_id: str,
         selection_id: str,
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/betfair/sockets.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/betfair/sockets.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/binance/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/binance/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/binance/common/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/binance/common/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/binance/common/constants.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/binance/common/constants.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/binance/common/data.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/binance/common/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 # -------------------------------------------------------------------------------------------------
 
 import asyncio
-from typing import Optional
+from typing import Optional, Union
 
 import msgspec
 import pandas as pd
 
 from nautilus_trader.adapters.binance.common.constants import BINANCE_VENUE
 from nautilus_trader.adapters.binance.common.enums import BinanceAccountType
 from nautilus_trader.adapters.binance.common.enums import BinanceEnumParser
@@ -42,25 +42,25 @@
 from nautilus_trader.common.providers import InstrumentProvider
 from nautilus_trader.core.correctness import PyCondition
 from nautilus_trader.core.datetime import secs_to_millis
 from nautilus_trader.core.uuid import UUID4
 from nautilus_trader.live.data_client import LiveMarketDataClient
 from nautilus_trader.model.data.bar import BarType
 from nautilus_trader.model.data.base import DataType
+from nautilus_trader.model.data.book import OrderBookDelta
+from nautilus_trader.model.data.book import OrderBookDeltas
+from nautilus_trader.model.data.book import OrderBookSnapshot
 from nautilus_trader.model.data.tick import QuoteTick
 from nautilus_trader.model.data.tick import TradeTick
 from nautilus_trader.model.enums import BookType
 from nautilus_trader.model.enums import PriceType
 from nautilus_trader.model.identifiers import ClientId
 from nautilus_trader.model.identifiers import InstrumentId
 from nautilus_trader.model.identifiers import Symbol
 from nautilus_trader.model.instruments import Instrument
-from nautilus_trader.model.orderbook.data import OrderBookData
-from nautilus_trader.model.orderbook.data import OrderBookDeltas
-from nautilus_trader.model.orderbook.data import OrderBookSnapshot
 from nautilus_trader.msgbus.bus import MessageBus
 
 
 class BinanceCommonDataClient(LiveMarketDataClient):
     """
     Provides a data client of common methods for the `Binance` exchange.
 
@@ -147,15 +147,18 @@
             logger=logger,
             handler=self._handle_ws_message,
             base_url=base_url_ws,
         )
 
         # Hot caches
         self._instrument_ids: dict[str, InstrumentId] = {}
-        self._book_buffer: dict[InstrumentId, list[OrderBookData]] = {}
+        self._book_buffer: dict[
+            InstrumentId,
+            list[Union[OrderBookDelta, OrderBookDeltas, OrderBookSnapshot]],
+        ] = {}
 
         self._log.info(f"Base URL HTTP {self._http_client.base_url}.", LogColor.BLUE)
         self._log.info(f"Base URL WebSocket {base_url_ws}.", LogColor.BLUE)
 
         # Register common WebSocket message handlers
         self._ws_handlers = {
             "@bookTicker": self._handle_book_ticker,
@@ -444,19 +447,19 @@
             data_type=data_type,
             data=[instrument],  # Data engine handles lists of instruments
             correlation_id=correlation_id,
         )
 
     async def _request_quote_ticks(
         self,
-        instrument_id: InstrumentId,  # noqa
-        limit: int,  # noqa
-        correlation_id: UUID4,  # noqa
-        start: Optional[pd.Timestamp] = None,  # noqa
-        end: Optional[pd.Timestamp] = None,  # noqa
+        instrument_id: InstrumentId,
+        limit: int,
+        correlation_id: UUID4,
+        start: Optional[pd.Timestamp] = None,
+        end: Optional[pd.Timestamp] = None,
     ) -> None:
         self._log.error(
             "Cannot request historical quote ticks: not published by Binance.",
         )
 
     async def _request_trade_ticks(
         self,
@@ -495,15 +498,15 @@
                 start_time=start_time_ms,
                 end_time=end_time_ms,
                 ts_init=self._clock.timestamp_ns(),
             )
 
         self._handle_trade_ticks(instrument_id, ticks, correlation_id)
 
-    async def _request_bars(  # noqa (too complex)
+    async def _request_bars(  # (too complex)
         self,
         bar_type: BarType,
         limit: int,
         correlation_id: UUID4,
         start: Optional[pd.Timestamp] = None,
         end: Optional[pd.Timestamp] = None,
     ) -> None:
@@ -608,15 +611,17 @@
     def _handle_book_diff_update(self, raw: bytes) -> None:
         msg = self._decoder_order_book_msg.decode(raw)
         instrument_id: InstrumentId = self._get_cached_instrument_id(msg.data.s)
         book_deltas: OrderBookDeltas = msg.data.parse_to_order_book_deltas(
             instrument_id=instrument_id,
             ts_init=self._clock.timestamp_ns(),
         )
-        book_buffer: Optional[list[OrderBookData]] = self._book_buffer.get(instrument_id)
+        book_buffer: Optional[
+            list[Union[OrderBookDelta, OrderBookDeltas, OrderBookSnapshot]]
+        ] = self._book_buffer.get(instrument_id)
         if book_buffer is not None:
             book_buffer.append(book_deltas)
         else:
             self._handle_data(book_deltas)
 
     def _handle_book_ticker(self, raw: bytes) -> None:
         msg = self._decoder_quote_msg.decode(raw)
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/binance/common/enums.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/binance/common/enums.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/binance/common/execution.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/binance/common/execution.py`

 * *Files 0% similar despite different names*

```diff
@@ -297,20 +297,20 @@
                     symbol=instrument_id.symbol.value,
                     orig_client_order_id=client_order_id.value
                     if client_order_id is not None
                     else None,
                 )
         except BinanceError as e:
             self._log.error(
-                f"Cannot generate order status report for {repr(client_order_id)}: {e.message}. Retry {retries}/3",
+                f"Cannot generate order status report for {client_order_id!r}: {e.message}. Retry {retries}/3",
             )
             retries += 1
             self._generate_order_status_retries[client_order_id] = retries
             if not client_order_id:
-                self.log.warning("Cannot retry without a client order ID.")
+                self._log.warning("Cannot retry without a client order ID.")
             else:
                 order: Optional[Order] = self._cache.order(client_order_id)
                 if order is None:
                     self._log.warning("Order not found in cache.")
                     return None
                 elif order.is_closed:
                     return None  # Nothing else to do
@@ -457,15 +457,15 @@
             # TODO(cs): Time filter is WIP
             # timestamp = pd.to_datetime(data["time"], utc=True)
             # if start is not None and timestamp < start:
             #     continue
             # if end is not None and timestamp > end:
             #     continue
             if trade.symbol is None:
-                self.log.warning(f"No symbol for trade {trade}.")
+                self._log.warning(f"No symbol for trade {trade}.")
                 continue
             report = trade.parse_to_trade_report(
                 account_id=self.account_id,
                 instrument_id=self._get_cached_instrument_id(trade.symbol),
                 report_id=UUID4(),
                 ts_init=self._clock.timestamp_ns(),
             )
@@ -504,15 +504,15 @@
 
     # -- COMMAND HANDLERS -------------------------------------------------------------------------
 
     async def _submit_order(self, command: SubmitOrder) -> None:
         order: Order = command.order
 
         if order.is_closed:
-            self.log.warning(f"Cannot submit already closed order {command.order}.")
+            self._log.warning(f"Cannot submit already closed order {order}.")
             return
 
         # Check validity
         self._check_order_validity(order)
         self._log.debug(f"Submitting {order}.")
 
         # Generate event here to ensure correct ordering of events
@@ -547,17 +547,20 @@
             quantity=str(order.quantity),
             new_client_order_id=order.client_order_id.value,
             recv_window=str(5000),
         )
 
     async def _submit_limit_order(self, order: LimitOrder) -> None:
         time_in_force = self._enum_parser.parse_internal_time_in_force(order.time_in_force)
-        if order.time_in_force == TimeInForce.GTD and time_in_force == BinanceTimeInForce.GTC:
-            if self._warn_gtd_to_gtc:
-                self._log.warning("Converted GTD `time_in_force` to GTC.")
+        if (
+            order.time_in_force == TimeInForce.GTD
+            and time_in_force == BinanceTimeInForce.GTC
+            and self._warn_gtd_to_gtc
+        ):
+            self._log.warning("Converted GTD `time_in_force` to GTC.")
         if order.is_post_only and self._binance_account_type.is_spot_or_margin:
             time_in_force = None
         elif order.is_post_only and self._binance_account_type.is_futures:
             time_in_force = BinanceTimeInForce.GTX
 
         await self._http_account.new_order(
             symbol=order.instrument_id.symbol.value,
@@ -790,15 +793,21 @@
                 for order in open_orders_strategy:
                     await self._cancel_order_single(
                         instrument_id=order.instrument_id,
                         client_order_id=order.client_order_id,
                         venue_order_id=order.venue_order_id,
                     )
         except BinanceError as e:
-            self._log.exception(f"Cannot cancel open orders: {e.message}", e)
+            if "Unknown order sent" in e.message:
+                self._log.info(
+                    "No open orders to cancel according to Binance.",
+                    LogColor.GREEN,
+                )
+            else:
+                self._log.exception(f"Cannot cancel open orders: {e.message}", e)
 
     async def _cancel_order_single(
         self,
         instrument_id: InstrumentId,
         client_order_id: ClientOrderId,
         venue_order_id: Optional[VenueOrderId],
     ) -> None:
@@ -812,16 +821,16 @@
                 await self._http_account.cancel_order(
                     symbol=instrument_id.symbol.value,
                     orig_client_order_id=client_order_id.value,
                 )
         except BinanceError as e:
             self._log.exception(
                 f"Cannot cancel order "
-                f"{repr(client_order_id)}, "
-                f"{repr(venue_order_id)}: "
+                f"{client_order_id!r}, "
+                f"{venue_order_id!r}: "
                 f"{e.message}",
                 e,
             )
 
     # -- WEBSOCKET EVENT HANDLERS --------------------------------------------------------------------
 
     def _handle_user_ws_message(self, raw: bytes) -> None:
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/binance/common/schemas/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/binance/futures/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/binance/common/schemas/account.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/binance/common/schemas/account.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/binance/common/schemas/market.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/binance/common/schemas/market.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,29 +24,28 @@
 from nautilus_trader.adapters.binance.common.enums import BinanceRateLimitInterval
 from nautilus_trader.adapters.binance.common.enums import BinanceRateLimitType
 from nautilus_trader.adapters.binance.common.enums import BinanceSymbolFilterType
 from nautilus_trader.adapters.binance.common.types import BinanceBar
 from nautilus_trader.adapters.binance.common.types import BinanceTicker
 from nautilus_trader.core.datetime import millis_to_nanos
 from nautilus_trader.model.data.bar import BarType
+from nautilus_trader.model.data.book import BookOrder
+from nautilus_trader.model.data.book import OrderBookDelta
+from nautilus_trader.model.data.book import OrderBookDeltas
+from nautilus_trader.model.data.book import OrderBookSnapshot
 from nautilus_trader.model.data.tick import QuoteTick
 from nautilus_trader.model.data.tick import TradeTick
 from nautilus_trader.model.enums import AggregationSource
 from nautilus_trader.model.enums import AggressorSide
 from nautilus_trader.model.enums import BookAction
-from nautilus_trader.model.enums import BookType
 from nautilus_trader.model.enums import OrderSide
 from nautilus_trader.model.identifiers import InstrumentId
 from nautilus_trader.model.identifiers import TradeId
 from nautilus_trader.model.objects import Price
 from nautilus_trader.model.objects import Quantity
-from nautilus_trader.model.orderbook.data import BookOrder
-from nautilus_trader.model.orderbook.data import OrderBookDelta
-from nautilus_trader.model.orderbook.data import OrderBookDeltas
-from nautilus_trader.model.orderbook.data import OrderBookSnapshot
 
 
 ################################################################################
 # HTTP responses
 ################################################################################
 
 
@@ -139,15 +138,14 @@
     def parse_to_order_book_snapshot(
         self,
         instrument_id: InstrumentId,
         ts_init: int,
     ) -> OrderBookSnapshot:
         return OrderBookSnapshot(
             instrument_id=instrument_id,
-            book_type=BookType.L2_MBP,
             bids=[[float(o[0]), float(o[1])] for o in self.bids or []],
             asks=[[float(o[0]), float(o[1])] for o in self.asks or []],
             ts_event=ts_init,
             ts_init=ts_init,
             sequence=self.lastUpdateId or 0,
         )
 
@@ -334,15 +332,14 @@
             price=price,
             size=size,
             side=side,
         )
 
         return OrderBookDelta(
             instrument_id=instrument_id,
-            book_type=BookType.L2_MBP,
             action=BookAction.UPDATE if size > 0.0 else BookAction.DELETE,
             order=order,
             ts_event=ts_event,
             ts_init=ts_init,
             sequence=update_id,
         )
 
@@ -383,29 +380,27 @@
                 self.u,
             )
             for delta in self.a
         ]
 
         return OrderBookDeltas(
             instrument_id=instrument_id,
-            book_type=BookType.L2_MBP,
             deltas=bid_deltas + ask_deltas,
             ts_event=ts_event,
             ts_init=ts_init,
             sequence=self.u,
         )
 
     def parse_to_order_book_snapshot(
         self,
         instrument_id: InstrumentId,
         ts_init: int,
     ) -> OrderBookSnapshot:
         return OrderBookSnapshot(
             instrument_id=instrument_id,
-            book_type=BookType.L2_MBP,
             bids=[[float(o.price), float(o.size)] for o in self.b],
             asks=[[float(o.price), float(o.size)] for o in self.a],
             ts_event=millis_to_nanos(self.T),
             ts_init=ts_init,
             sequence=self.u,
         )
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/binance/common/schemas/symbol.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/binance/common/schemas/symbol.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/binance/common/schemas/user.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/binance/common/schemas/user.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/binance/common/types.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/binance/common/types.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/binance/config.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/binance/config.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/binance/factories.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/binance/factories.py`

 * *Files 0% similar despite different names*

```diff
@@ -486,8 +486,8 @@
     elif account_type == BinanceAccountType.FUTURES_USDT:
         return f"wss://fstream.binance.{top_level_domain}"
     elif account_type == BinanceAccountType.FUTURES_COIN:
         return f"wss://dstream.binance.{top_level_domain}"
     else:
         raise RuntimeError(
             f"invalid `BinanceAccountType`, was {account_type}",
-        )  # pragma: no cover (design-time error)  # noqa
+        )  # pragma: no cover (design-time error)
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/binance/futures/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/binance/futures/http/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/binance/futures/data.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/binance/futures/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 # -------------------------------------------------------------------------------------------------
 
 import asyncio
-from typing import Optional
+from typing import Optional, Union
 
 import msgspec
 
 from nautilus_trader.adapters.binance.common.data import BinanceCommonDataClient
 from nautilus_trader.adapters.binance.common.enums import BinanceAccountType
 from nautilus_trader.adapters.binance.futures.enums import BinanceFuturesEnumParser
 from nautilus_trader.adapters.binance.futures.http.market import BinanceFuturesMarketHttpAPI
@@ -29,18 +29,19 @@
 from nautilus_trader.cache.cache import Cache
 from nautilus_trader.common.clock import LiveClock
 from nautilus_trader.common.logging import Logger
 from nautilus_trader.common.providers import InstrumentProvider
 from nautilus_trader.core.correctness import PyCondition
 from nautilus_trader.model.data.base import DataType
 from nautilus_trader.model.data.base import GenericData
+from nautilus_trader.model.data.book import OrderBookDelta
+from nautilus_trader.model.data.book import OrderBookDeltas
+from nautilus_trader.model.data.book import OrderBookSnapshot
 from nautilus_trader.model.data.tick import TradeTick
 from nautilus_trader.model.identifiers import InstrumentId
-from nautilus_trader.model.orderbook.data import OrderBookData
-from nautilus_trader.model.orderbook.data import OrderBookSnapshot
 from nautilus_trader.msgbus.bus import MessageBus
 
 
 class BinanceFuturesDataClient(BinanceCommonDataClient):
     """
     Provides a data client for the `Binance Futures` exchange.
 
@@ -164,15 +165,17 @@
         msg = self._decoder_order_book_msg.decode(raw)
         instrument_id: InstrumentId = self._get_cached_instrument_id(msg.data.s)
         book_snapshot: OrderBookSnapshot = msg.data.parse_to_order_book_snapshot(
             instrument_id=instrument_id,
             ts_init=self._clock.timestamp_ns(),
         )
         # Check if book buffer active
-        book_buffer: Optional[list[OrderBookData]] = self._book_buffer.get(instrument_id)
+        book_buffer: Optional[
+            list[Union[OrderBookDelta, OrderBookDeltas, OrderBookSnapshot]]
+        ] = self._book_buffer.get(instrument_id)
         if book_buffer is not None:
             book_buffer.append(book_snapshot)
         else:
             self._handle_data(book_snapshot)
 
     def _handle_trade(self, raw: bytes) -> None:
         # NOTE @trade is an undocumented endpoint for Futures exchanges
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/binance/futures/enums.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/binance/futures/enums.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/binance/futures/execution.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/binance/futures/execution.py`

 * *Files 0% similar despite different names*

```diff
@@ -238,15 +238,15 @@
     def _handle_user_ws_message(self, raw: bytes) -> None:
         # TODO(cs): Uncomment for development
         # self._log.info(str(json.dumps(msgspec.json.decode(raw), indent=4)), color=LogColor.MAGENTA)
         wrapper = self._decoder_futures_user_msg_wrapper.decode(raw)
         try:
             self._futures_user_ws_handlers[wrapper.data.e](raw)
         except Exception as e:
-            self._log.exception(f"Error on handling {repr(raw)}", e)
+            self._log.exception(f"Error on handling {raw!r}", e)
 
     def _handle_account_update(self, raw: bytes) -> None:
         account_update = self._decoder_futures_account_update_wrapper.decode(raw)
         account_update.data.handle_account_update(self)
 
     def _handle_order_trade_update(self, raw: bytes) -> None:
         order_update = self._decoder_futures_order_update_wrapper.decode(raw)
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/binance/futures/http/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/binance/futures/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/binance/futures/http/account.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/binance/futures/http/account.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/binance/futures/http/market.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/binance/futures/http/market.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/binance/futures/http/user.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/binance/futures/http/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,9 +39,9 @@
         super().__init__(
             client=client,
             account_type=account_type,
         )
 
         if not account_type.is_futures:
             raise RuntimeError(  # pragma: no cover (design-time error)
-                f"`BinanceAccountType` not FUTURES_USDT or FUTURES_COIN, was {account_type}",  # pragma: no cover (design-time error)  # noqa
+                f"`BinanceAccountType` not FUTURES_USDT or FUTURES_COIN, was {account_type}",  # pragma: no cover (design-time error)
             )
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/binance/futures/http/wallet.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/binance/futures/http/wallet.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/binance/futures/providers.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/binance/futures/providers.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,15 +205,15 @@
 
         self._parse_instrument(
             symbol_info=symbol_info_dict[symbol],
             ts_event=millis_to_nanos(exchange_info.serverTime),
             fee=fee,
         )
 
-    def _parse_instrument(  # noqa (C901 too complex)
+    def _parse_instrument(
         self,
         symbol_info: BinanceFuturesSymbolInfo,
         ts_event: int,
         fee: Optional[BinanceFuturesCommissionRate] = None,
     ) -> None:
         contract_type_str = symbol_info.contractType
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/binance/futures/schemas/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/binance/http/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/binance/futures/schemas/account.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/binance/futures/schemas/account.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/binance/futures/schemas/market.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/binance/futures/schemas/market.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/binance/futures/schemas/user.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/binance/futures/schemas/user.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/binance/futures/schemas/wallet.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/binance/futures/schemas/wallet.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/binance/futures/types.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/binance/futures/types.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/binance/http/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/binance/spot/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/binance/http/account.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/binance/http/account.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/binance/http/client.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/binance/http/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,21 +156,17 @@
             return b""
         except aiohttp.ClientResponseError as e:
             await self._handle_exception(e)
             return
 
         if self._show_limit_usage:
             limit_usage = {}
-            for key in resp.headers.keys():
+            for key in resp.headers:
                 key = key.lower()
-                if (
-                    key.startswith("x-mbx-used-weight")
-                    or key.startswith("x-mbx-order-count")
-                    or key.startswith("x-sapi-used")
-                ):
+                if key.startswith(("x-mbx-used-weight", "x-mbx-order-count", "x-sapi-used")):
                     limit_usage[key] = resp.headers[key]
 
         try:
             return resp.data
         except msgspec.MsgspecError:
             self._log.error(f"Could not decode data to JSON: {resp.data}.")
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/binance/http/endpoint.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/binance/http/endpoint.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/binance/http/error.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/binance/http/error.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # -------------------------------------------------------------------------------------------------
 
 
 class BinanceError(Exception):
     """The base class for all `Binance` specific errors."""
 
     def __init__(self, status, message, headers):
+        super().__init__(message)
         self.status = status
         self.message = message
         self.headers = headers
 
 
 class BinanceServerError(BinanceError):
     """Represents an `Binance` specific 500 series HTTP error."""
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/binance/http/market.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/binance/http/market.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,17 +32,17 @@
 from nautilus_trader.adapters.binance.common.schemas.symbol import BinanceSymbol
 from nautilus_trader.adapters.binance.common.schemas.symbol import BinanceSymbols
 from nautilus_trader.adapters.binance.common.types import BinanceBar
 from nautilus_trader.adapters.binance.http.client import BinanceHttpClient
 from nautilus_trader.adapters.binance.http.endpoint import BinanceHttpEndpoint
 from nautilus_trader.core.correctness import PyCondition
 from nautilus_trader.model.data.bar import BarType
+from nautilus_trader.model.data.book import OrderBookSnapshot
 from nautilus_trader.model.data.tick import TradeTick
 from nautilus_trader.model.identifiers import InstrumentId
-from nautilus_trader.model.orderbook.data import OrderBookSnapshot
 
 
 class BinancePingHttp(BinanceHttpEndpoint):
     """
     Endpoint for testing connectivity to the REST API.
 
     `GET /api/v3/ping`
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/binance/http/user.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/binance/http/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,15 +157,15 @@
             self.base_endpoint = "/fapi/v1/"
             listen_key_url = self.base_endpoint + "listenKey"
         elif account_type == BinanceAccountType.FUTURES_COIN:
             self.base_endpoint = "/dapi/v1/"
             listen_key_url = self.base_endpoint + "listenKey"
         else:
             raise RuntimeError(  # pragma: no cover (design-time error)
-                f"invalid `BinanceAccountType`, was {account_type}",  # pragma: no cover (design-time error)  # noqa
+                f"invalid `BinanceAccountType`, was {account_type}",  # pragma: no cover (design-time error)
             )
 
         self._endpoint_listenkey = BinanceListenKeyHttp(client, listen_key_url)
 
     async def create_listen_key(
         self,
         symbol: Optional[str] = None,
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/binance/spot/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/binance/spot/http/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/binance/spot/data.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/binance/spot/data.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 # -------------------------------------------------------------------------------------------------
 
 import asyncio
-from typing import Optional
+from typing import Optional, Union
 
 import msgspec
 
 from nautilus_trader.adapters.binance.common.data import BinanceCommonDataClient
 from nautilus_trader.adapters.binance.common.enums import BinanceAccountType
 from nautilus_trader.adapters.binance.http.client import BinanceHttpClient
 from nautilus_trader.adapters.binance.spot.enums import BinanceSpotEnumParser
@@ -26,18 +26,19 @@
 from nautilus_trader.adapters.binance.spot.schemas.market import BinanceSpotOrderBookPartialDepthMsg
 from nautilus_trader.adapters.binance.spot.schemas.market import BinanceSpotTradeMsg
 from nautilus_trader.cache.cache import Cache
 from nautilus_trader.common.clock import LiveClock
 from nautilus_trader.common.logging import Logger
 from nautilus_trader.common.providers import InstrumentProvider
 from nautilus_trader.core.correctness import PyCondition
+from nautilus_trader.model.data.book import OrderBookDelta
+from nautilus_trader.model.data.book import OrderBookDeltas
+from nautilus_trader.model.data.book import OrderBookSnapshot
 from nautilus_trader.model.data.tick import TradeTick
 from nautilus_trader.model.identifiers import InstrumentId
-from nautilus_trader.model.orderbook.data import OrderBookData
-from nautilus_trader.model.orderbook.data import OrderBookSnapshot
 from nautilus_trader.msgbus.bus import MessageBus
 
 
 class BinanceSpotDataClient(BinanceCommonDataClient):
     """
     Provides a data client for the `Binance Spot/Margin` exchange.
 
@@ -119,15 +120,17 @@
             msg.stream.partition("@")[0],
         )
         book_snapshot: OrderBookSnapshot = msg.data.parse_to_order_book_snapshot(
             instrument_id=instrument_id,
             ts_init=self._clock.timestamp_ns(),
         )
         # Check if book buffer active
-        book_buffer: Optional[list[OrderBookData]] = self._book_buffer.get(instrument_id)
+        book_buffer: Optional[
+            list[Union[OrderBookDelta, OrderBookDeltas, OrderBookSnapshot]]
+        ] = self._book_buffer.get(instrument_id)
         if book_buffer is not None:
             book_buffer.append(book_snapshot)
         else:
             self._handle_data(book_snapshot)
 
     def _handle_trade(self, raw: bytes) -> None:
         msg = self._decoder_spot_trade.decode(raw)
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/binance/spot/enums.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/binance/spot/enums.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/binance/spot/execution.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/binance/spot/execution.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,15 +204,15 @@
     def _handle_user_ws_message(self, raw: bytes) -> None:
         # TODO(cs): Uncomment for development
         # self._log.info(str(json.dumps(msgspec.json.decode(raw), indent=4)), color=LogColor.MAGENTA)
         wrapper = self._decoder_spot_user_msg_wrapper.decode(raw)
         try:
             self._spot_user_ws_handlers[wrapper.data.e](raw)
         except Exception as e:
-            self._log.exception(f"Error on handling {repr(raw)}", e)
+            self._log.exception(f"Error on handling {raw!r}", e)
 
     def _handle_account_update(self, raw: bytes) -> None:
         account_msg = self._decoder_spot_account_update_wrapper.decode(raw)
         account_msg.data.handle_account_update(self)
 
     def _handle_execution_report(self, raw: bytes) -> None:
         order_msg = self._decoder_spot_order_update_wrapper.decode(raw)
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/binance/spot/http/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/binance/spot/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/binance/spot/http/account.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/binance/spot/http/account.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/binance/spot/http/market.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/binance/spot/http/market.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/binance/spot/http/user.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/binance/spot/http/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,9 +39,9 @@
         super().__init__(
             client=client,
             account_type=account_type,
         )
 
         if not account_type.is_spot_or_margin:
             raise RuntimeError(  # pragma: no cover (design-time error)
-                f"`BinanceAccountType` not SPOT, MARGIN_CROSS or MARGIN_ISOLATED, was {account_type}",  # pragma: no cover (design-time error)  # noqa
+                f"`BinanceAccountType` not SPOT, MARGIN_CROSS or MARGIN_ISOLATED, was {account_type}",  # pragma: no cover (design-time error)
             )
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/binance/spot/http/wallet.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/binance/spot/http/wallet.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/binance/spot/providers.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/binance/spot/providers.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/binance/spot/schemas/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/binance/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/binance/spot/schemas/account.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/binance/spot/schemas/account.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/binance/spot/schemas/market.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/binance/spot/schemas/market.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,23 +19,22 @@
 from nautilus_trader.adapters.binance.common.schemas.market import BinanceExchangeFilter
 from nautilus_trader.adapters.binance.common.schemas.market import BinanceOrderBookDelta
 from nautilus_trader.adapters.binance.common.schemas.market import BinanceRateLimit
 from nautilus_trader.adapters.binance.common.schemas.market import BinanceSymbolFilter
 from nautilus_trader.adapters.binance.spot.enums import BinanceSpotPermissions
 from nautilus_trader.core.datetime import millis_to_nanos
 from nautilus_trader.model.currency import Currency
+from nautilus_trader.model.data.book import OrderBookSnapshot
 from nautilus_trader.model.data.tick import TradeTick
 from nautilus_trader.model.enums import AggressorSide
-from nautilus_trader.model.enums import BookType
 from nautilus_trader.model.enums import CurrencyType
 from nautilus_trader.model.identifiers import InstrumentId
 from nautilus_trader.model.identifiers import TradeId
 from nautilus_trader.model.objects import Price
 from nautilus_trader.model.objects import Quantity
-from nautilus_trader.model.orderbook.data import OrderBookSnapshot
 
 
 ################################################################################
 # HTTP responses
 ################################################################################
 
 
@@ -110,15 +109,14 @@
     def parse_to_order_book_snapshot(
         self,
         instrument_id: InstrumentId,
         ts_init: int,
     ) -> OrderBookSnapshot:
         return OrderBookSnapshot(
             instrument_id=instrument_id,
-            book_type=BookType.L2_MBP,
             bids=[[float(o.price), float(o.size)] for o in self.bids],
             asks=[[float(o.price), float(o.size)] for o in self.asks],
             ts_event=ts_init,
             ts_init=ts_init,
             sequence=self.lastUpdateId,
         )
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/binance/spot/schemas/user.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/binance/spot/schemas/user.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/binance/spot/schemas/wallet.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/binance/spot/schemas/wallet.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/binance/websocket/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/deribit/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/binance/websocket/client.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/binance/websocket/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,18 +53,15 @@
 
     @property
     def subscriptions(self) -> list[str]:
         return self._streams.copy()
 
     @property
     def has_subscriptions(self) -> bool:
-        if self._streams:
-            return True
-        else:
-            return False
+        return bool(self._streams)
 
     async def connect(
         self,
         key: Optional[str] = None,
         start: bool = True,
         **ws_kwargs: dict[str, Any],
     ) -> None:
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/deribit/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/deribit/http/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/deribit/http/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/interactive_brokers/parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/deribit/http/client.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/deribit/http/client.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/deribit/http/error.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/deribit/http/error.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/interactive_brokers/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/interactive_brokers/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/interactive_brokers/common.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/interactive_brokers/common.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/interactive_brokers/config.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/interactive_brokers/config.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/interactive_brokers/data.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/interactive_brokers/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,43 +24,45 @@
 from ib_insync import Contract
 from ib_insync import ContractDetails
 from ib_insync import RealTimeBar
 from ib_insync import RealTimeBarList
 from ib_insync import Ticker
 from ib_insync.ticker import nan
 
+# fmt: off
 from nautilus_trader.adapters.interactive_brokers.common import IB_VENUE
 from nautilus_trader.adapters.interactive_brokers.common import ContractId
 from nautilus_trader.adapters.interactive_brokers.parsing.data import bar_spec_to_bar_size
 from nautilus_trader.adapters.interactive_brokers.parsing.data import generate_trade_id
 from nautilus_trader.adapters.interactive_brokers.parsing.data import parse_bar_data
 from nautilus_trader.adapters.interactive_brokers.parsing.data import timedelta_to_duration_str
-from nautilus_trader.adapters.interactive_brokers.providers import (
-    InteractiveBrokersInstrumentProvider,
-)
+from nautilus_trader.adapters.interactive_brokers.providers import InteractiveBrokersInstrumentProvider
 from nautilus_trader.cache.cache import Cache
 from nautilus_trader.common.clock import LiveClock
 from nautilus_trader.common.logging import Logger
 from nautilus_trader.core.datetime import dt_to_unix_nanos
 from nautilus_trader.live.data_client import LiveMarketDataClient
 from nautilus_trader.model.data.bar import Bar
 from nautilus_trader.model.data.bar import BarType
+from nautilus_trader.model.data.book import OrderBookSnapshot
 from nautilus_trader.model.data.tick import QuoteTick
 from nautilus_trader.model.data.tick import TradeTick
 from nautilus_trader.model.enums import AggressorSide
 from nautilus_trader.model.enums import BookType
 from nautilus_trader.model.enums import PriceType
 from nautilus_trader.model.identifiers import ClientId
 from nautilus_trader.model.identifiers import InstrumentId
 from nautilus_trader.model.objects import Price
 from nautilus_trader.model.objects import Quantity
-from nautilus_trader.model.orderbook.data import OrderBookSnapshot
 from nautilus_trader.msgbus.bus import MessageBus
 
 
+# fmt: on
+
+
 class InteractiveBrokersDataClient(LiveMarketDataClient):
     """
     Provides a data client for the InteractiveBrokers exchange.
 
     Parameters
     ----------
     loop : asyncio.AbstractEventLoop
@@ -158,15 +160,15 @@
                             host=self._client.client.host,
                             port=self._client.client.port,
                             clientId=self._client.client.clientId,
                             timeout=30,
                         )
                         self._resubscribe_on_reset()
                     except Exception as e:
-                        self._log.info(f"{repr(e)}")
+                        self._log.info(f"{e!r}")
         except asyncio.CancelledError:
             self._log.debug("`watch_dog` task was canceled.")
 
     async def _subscribe_order_book_snapshots(
         self,
         instrument_id: InstrumentId,
         book_type: BookType,
@@ -257,15 +259,15 @@
                 )
             bar_data_list: BarDataList = await self._client.reqHistoricalDataAsync(
                 contract=contract_details.contract,
                 endDateTime="",
                 durationStr=timedelta_to_duration_str(duration),
                 barSizeSetting=bar_size_setting,
                 whatToShow=what_to_show[bar_type.spec.price_type],
-                useRTH=True if contract_details.contract.secType == "STK" else False,
+                useRTH=contract_details.contract.secType == "STK",
                 formatDate=2,
                 keepUpToDate=True,
             )
             bar_data_list.bar_type = bar_type
             bar_data_list.instrument = self.instrument_provider.find(bar_type.instrument_id)
 
             self._on_historical_bar_update(
@@ -322,15 +324,14 @@
     # def _on_order_book_delta(self, ticker: Ticker):
     #     instrument_id = self.instrument_provider.contract_id_to_instrument_id[
     #         ticker.contract.conId
     #     ]
     #     for depth in ticker.domTicks:
     #         update = OrderBookDelta(
     #             instrument_id=instrument_id,
-    #             book_type=BookType.L2_MBP,
     #             action=MKT_DEPTH_OPERATIONS[depth.operation],
     #             order=Order(
     #                 price=Price.from_str(str(depth.price)),
     #                 size=Quantity.from_str(str(depth.size)),
     #                 side=IB_SIDE[depth.side],
     #             ),
     #             ts_event=dt_to_unix_nanos(depth.time),
@@ -367,15 +368,14 @@
         self._handle_data(quote_tick)
 
     def _on_top_level_snapshot(self, ticker: Ticker):
         instrument_id = self.instrument_provider.contract_id_to_instrument_id[ticker.contract.conId]
         ts_init = self._clock.timestamp_ns()
         ts_event = min(dt_to_unix_nanos(ticker.time), ts_init)
         snapshot = OrderBookSnapshot(
-            book_type=BookType.L1_TBBO,
             instrument_id=instrument_id,
             bids=[(ticker.bid, ticker.bidSize)],
             asks=[(ticker.ask, ticker.askSize)],
             ts_event=ts_event,
             ts_init=ts_init,
         )
         self._handle_data(snapshot)
@@ -383,15 +383,14 @@
     def _on_order_book_snapshot(self, ticker: Ticker, book_type: BookType = BookType.L2_MBP):
         instrument_id = self.instrument_provider.contract_id_to_instrument_id[ticker.contract.conId]
         ts_init = self._clock.timestamp_ns()
         ts_event = min(dt_to_unix_nanos(ticker.time), ts_init)
         if not (ticker.domBids or ticker.domAsks):
             return
         snapshot = OrderBookSnapshot(
-            book_type=book_type,
             instrument_id=instrument_id,
             bids=[(level.price, level.size) for level in ticker.domBids],
             asks=[(level.price, level.size) for level in ticker.domAsks],
             ts_event=ts_event,
             ts_init=ts_init,
         )
         self._handle_data(snapshot)
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/interactive_brokers/execution.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/interactive_brokers/execution.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,27 +20,20 @@
 import pandas as pd
 from ib_insync import AccountValue
 from ib_insync import Fill as IBFill
 from ib_insync import Order as IBOrder
 from ib_insync import OrderStatus as IBOrderStatus
 from ib_insync import Trade as IBTrade
 
+# fmt: off
 from nautilus_trader.adapters.interactive_brokers.common import IB_VENUE
-from nautilus_trader.adapters.interactive_brokers.parsing.execution import (
-    account_values_to_nautilus_account_info,
-)
-from nautilus_trader.adapters.interactive_brokers.parsing.execution import (
-    ib_order_to_nautilus_order_type,
-)
-from nautilus_trader.adapters.interactive_brokers.parsing.execution import (
-    nautilus_order_to_ib_order,
-)
-from nautilus_trader.adapters.interactive_brokers.providers import (
-    InteractiveBrokersInstrumentProvider,
-)
+from nautilus_trader.adapters.interactive_brokers.parsing.execution import account_values_to_nautilus_account_info
+from nautilus_trader.adapters.interactive_brokers.parsing.execution import ib_order_to_nautilus_order_type
+from nautilus_trader.adapters.interactive_brokers.parsing.execution import nautilus_order_to_ib_order
+from nautilus_trader.adapters.interactive_brokers.providers import InteractiveBrokersInstrumentProvider
 from nautilus_trader.cache.cache import Cache
 from nautilus_trader.common.clock import LiveClock
 from nautilus_trader.common.logging import Logger
 from nautilus_trader.core.correctness import PyCondition
 from nautilus_trader.core.datetime import dt_to_unix_nanos
 from nautilus_trader.execution.messages import CancelOrder
 from nautilus_trader.execution.messages import ModifyOrder
@@ -65,14 +58,17 @@
 from nautilus_trader.model.objects import Money
 from nautilus_trader.model.objects import Price
 from nautilus_trader.model.objects import Quantity
 from nautilus_trader.model.orders import Order
 from nautilus_trader.msgbus.bus import MessageBus
 
 
+# fmt: on
+
+
 class InteractiveBrokersExecutionClient(LiveExecutionClient):
     """
     Provides an execution client for Interactive Brokers TWS API.
 
     Parameters
     ----------
     loop : asyncio.AbstractEventLoop
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/interactive_brokers/factories.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/interactive_brokers/factories.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,33 +16,34 @@
 import asyncio
 import os
 from functools import lru_cache
 from typing import Literal, Optional
 
 import ib_insync
 
+# fmt: off
 from nautilus_trader.adapters.interactive_brokers.common import IB_VENUE
 from nautilus_trader.adapters.interactive_brokers.config import InteractiveBrokersDataClientConfig
 from nautilus_trader.adapters.interactive_brokers.config import InteractiveBrokersExecClientConfig
 from nautilus_trader.adapters.interactive_brokers.data import InteractiveBrokersDataClient
 from nautilus_trader.adapters.interactive_brokers.execution import InteractiveBrokersExecutionClient
 from nautilus_trader.adapters.interactive_brokers.gateway import InteractiveBrokersGateway
-from nautilus_trader.adapters.interactive_brokers.providers import (
-    InteractiveBrokersInstrumentProvider,
-)
+from nautilus_trader.adapters.interactive_brokers.providers import InteractiveBrokersInstrumentProvider
 from nautilus_trader.cache.cache import Cache
 from nautilus_trader.common.clock import LiveClock
 from nautilus_trader.common.logging import Logger
 from nautilus_trader.config import InstrumentProviderConfig
 from nautilus_trader.live.factories import LiveDataClientFactory
 from nautilus_trader.live.factories import LiveExecClientFactory
 from nautilus_trader.model.identifiers import AccountId
 from nautilus_trader.msgbus.bus import MessageBus
 
 
+# fmt: on
+
 GATEWAY = None
 IB_INSYNC_CLIENTS: dict[tuple, ib_insync.IB] = {}
 
 
 def get_cached_ib_client(
     username: str,
     password: str,
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/interactive_brokers/gateway.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/interactive_brokers/gateway.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         self.log = logger or logging.getLogger("nautilus_trader")
         if start:
             self.start()
 
     @classmethod
     def from_container(cls, **kwargs):
         """Connect to an already running container - don't stop/start"""
-        self = cls(username="", password="", **kwargs)  # noqa: S106
+        self = cls(username="", password="", **kwargs)
         assert self.container, "Container does not exist"
         return self
 
     @property
     def container_status(self) -> ContainerStatus:
         container = self.container
         if container is None:
@@ -115,15 +115,15 @@
 
     @staticmethod
     def is_logged_in(container) -> bool:
         try:
             logs = container.logs()
         except NoContainer:
             return False
-        return any([b"Forking :::" in line for line in logs.split(b"\n")])
+        return any(b"Forking :::" in line for line in logs.split(b"\n"))
 
     def start(self, wait: Optional[int] = 90):
         """
         Start the gateway.
 
         Parameters
         ----------
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/interactive_brokers/historic.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/interactive_brokers/historic.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/interactive_brokers/parsing/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/sandbox/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/interactive_brokers/parsing/data.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/interactive_brokers/parsing/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
         return False, f"{step} hour{'' if step == 1 else 's'}"
     elif aggregation == BarAggregation.DAY and step == 1:
         return False, f"{step} day"
     elif aggregation == BarAggregation.WEEK and step == 1:
         return False, f"{step} week"
     else:
         raise ValueError(
-            f"InteractiveBrokers doesn't support subscription for {repr(bar_spec)}",
+            f"InteractiveBrokers doesn't support subscription for {bar_spec!r}",
         )
 
 
 def timedelta_to_duration_str(duration: datetime.timedelta) -> str:
     if duration.days >= 365:
         return f"{duration.days / 365:.0f} Y"
     elif duration.days >= 30:
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/interactive_brokers/parsing/execution.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/interactive_brokers/parsing/execution.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 
     balances = []
     margin_balances = []
     for (account, currency), fields in groupby(
         sorted(account_values, key=group_key),
         key=group_key,
     ):
-        if not (account == account_id):
+        if account != account_id:
             continue
         if currency in ("", "BASE"):
             # Only report in base currency
             continue
         account_fields = {f.tag: f.value for f in fields}
         if "FullAvailableFunds" in account_fields:
             total_cash = float(account_fields["NetLiquidation"])
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/interactive_brokers/parsing/instruments.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/interactive_brokers/parsing/instruments.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/interactive_brokers/providers.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/interactive_brokers/providers.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
         build_options_chain=False,
         option_kwargs: Optional[str] = None,
     ) -> list[ContractDetails]:
         if build_futures_chain:
             return await self.get_future_chain_details(contract)
         elif build_options_chain:
             return await self.get_option_chain_details(
-                underlying=contract, **(json.loads(option_kwargs or "{}"))  # noqa: P103
+                underlying=contract, **(json.loads(option_kwargs or "{}"))
             )
         else:
             # Regular contract
             return await self._client.reqContractDetailsAsync(contract=contract)
 
     async def get_future_chain_details(
         self,
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/interactive_brokers/web.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/interactive_brokers/web.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #  limitations under the License.
 # -------------------------------------------------------------------------------------------------
 
 import enum
 from collections import namedtuple
 
 import requests
-from lxml.html import fromstring  # noqa: S410
+from lxml.html import fromstring
 
 
 class ProductClass(enum.Enum):
     """
     Interactive Brokers Web ProductClass
     """
 
@@ -122,16 +122,14 @@
 
 
 class Product(namedtuple("Product", "ib_symbol, description, native_symbol, currency")):
     """
     Interactive Brokers Web Product
     """
 
-    pass
-
 
 def _parse_products(table):
     for row in table.xpath(".//tr")[1:]:
         ib_symbol, desc, symbol, currency = list(
             filter(None, map(str.strip, row.xpath(".//text()"))),
         )
         yield Product(
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/sandbox/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/backtest/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/sandbox/config.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/sandbox/config.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/sandbox/execution.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/sandbox/execution.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,27 +31,29 @@
 from nautilus_trader.core.data import Data
 from nautilus_trader.execution.reports import OrderStatusReport
 from nautilus_trader.execution.reports import PositionStatusReport
 from nautilus_trader.execution.reports import TradeReport
 from nautilus_trader.live.execution_client import LiveExecutionClient
 from nautilus_trader.model.currency import Currency
 from nautilus_trader.model.data.bar import Bar
+from nautilus_trader.model.data.book import OrderBookDelta
+from nautilus_trader.model.data.book import OrderBookDeltas
+from nautilus_trader.model.data.book import OrderBookSnapshot
 from nautilus_trader.model.data.tick import QuoteTick
 from nautilus_trader.model.data.tick import TradeTick
 from nautilus_trader.model.enums import AccountType
 from nautilus_trader.model.enums import OmsType
 from nautilus_trader.model.identifiers import ClientId
 from nautilus_trader.model.identifiers import ClientOrderId
 from nautilus_trader.model.identifiers import InstrumentId
 from nautilus_trader.model.identifiers import Venue
 from nautilus_trader.model.identifiers import VenueOrderId
 from nautilus_trader.model.instruments import Instrument
 from nautilus_trader.model.objects import AccountBalance
 from nautilus_trader.model.objects import Money
-from nautilus_trader.model.orderbook.data import OrderBookData
 from nautilus_trader.msgbus.bus import MessageBus
 
 
 class SandboxExecutionClient(LiveExecutionClient):
     """
     Provides a sandboxed execution client for testing against.
 
@@ -193,15 +195,15 @@
         return self._client.cancel_order(command)
 
     def cancel_all_orders(self, command):
         return self._client.cancel_all_orders(command)
 
     def on_data(self, data: Data):
         # Taken from main backtest loop of BacktestEngine
-        if isinstance(data, OrderBookData):
+        if isinstance(data, (OrderBookDelta, OrderBookDeltas, OrderBookSnapshot)):
             self.exchange.process_order_book(data)
         elif isinstance(data, QuoteTick):
             self.exchange.process_quote_tick(data)
         elif isinstance(data, TradeTick):
             self.exchange.process_trade_tick(data)
         elif isinstance(data, Bar):
             self.exchange.process_bar(data)
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/adapters/sandbox/factory.py` & `nautilus_trader-1.174.0/nautilus_trader/adapters/sandbox/factory.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/analysis/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/analysis/analyzer.py` & `nautilus_trader-1.174.0/nautilus_trader/analysis/analyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -480,14 +480,11 @@
         """
         max_length: int = self._get_max_length_name()
         stats = self.get_performance_stats_general()
 
         output = []
         for k, v in stats.items():
             padding = max_length - len(k) + 1
-            if isinstance(v, (int, float, Decimal)):
-                v_formatted = f"{v:_}"
-            else:
-                v_formatted = str(v)
+            v_formatted = f"{v:_}" if isinstance(v, (int, float, Decimal)) else str(v)
             output.append(f"{k}: {' ' * padding}{v_formatted}")
 
         return output
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/analysis/reporter.py` & `nautilus_trader-1.174.0/nautilus_trader/analysis/reporter.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/analysis/statistic.py` & `nautilus_trader-1.174.0/nautilus_trader/analysis/statistic.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/analysis/statistics/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/analysis/statistics/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/analysis/statistics/expectancy.py` & `nautilus_trader-1.174.0/nautilus_trader/analysis/statistics/expectancy.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/analysis/statistics/long_ratio.py` & `nautilus_trader-1.174.0/nautilus_trader/analysis/statistics/long_ratio.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/analysis/statistics/loser_avg.py` & `nautilus_trader-1.174.0/nautilus_trader/analysis/statistics/loser_avg.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/analysis/statistics/loser_max.py` & `nautilus_trader-1.174.0/nautilus_trader/analysis/statistics/loser_max.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/analysis/statistics/loser_min.py` & `nautilus_trader-1.174.0/nautilus_trader/analysis/statistics/loser_min.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/analysis/statistics/profit_factor.py` & `nautilus_trader-1.174.0/nautilus_trader/analysis/statistics/profit_factor.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/analysis/statistics/returns_avg.py` & `nautilus_trader-1.174.0/nautilus_trader/analysis/statistics/returns_avg.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/analysis/statistics/returns_avg_loss.py` & `nautilus_trader-1.174.0/nautilus_trader/analysis/statistics/returns_avg_loss.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/analysis/statistics/returns_avg_win.py` & `nautilus_trader-1.174.0/nautilus_trader/analysis/statistics/returns_avg_win.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/analysis/statistics/returns_volatility.py` & `nautilus_trader-1.174.0/nautilus_trader/analysis/statistics/returns_volatility.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/analysis/statistics/risk_return_ratio.py` & `nautilus_trader-1.174.0/nautilus_trader/analysis/statistics/risk_return_ratio.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/analysis/statistics/sharpe_ratio.py` & `nautilus_trader-1.174.0/nautilus_trader/analysis/statistics/sharpe_ratio.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/analysis/statistics/sortino_ratio.py` & `nautilus_trader-1.174.0/nautilus_trader/analysis/statistics/sortino_ratio.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/analysis/statistics/win_rate.py` & `nautilus_trader-1.174.0/nautilus_trader/analysis/statistics/win_rate.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/analysis/statistics/winner_avg.py` & `nautilus_trader-1.174.0/nautilus_trader/analysis/statistics/winner_avg.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/analysis/statistics/winner_max.py` & `nautilus_trader-1.174.0/nautilus_trader/analysis/statistics/winner_max.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/analysis/statistics/winner_min.py` & `nautilus_trader-1.174.0/nautilus_trader/analysis/statistics/winner_min.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/backtest/__init__.pxd` & `nautilus_trader-1.174.0/nautilus_trader/cache/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/backtest/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/backtest/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/backtest/__main__.py` & `nautilus_trader-1.174.0/nautilus_trader/backtest/__main__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/backtest/auction.py` & `nautilus_trader-1.174.0/nautilus_trader/backtest/auction.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 # -------------------------------------------------------------------------------------------------
 
+from nautilus_trader.model.data.book import BookOrder
 from nautilus_trader.model.enums import OrderSide
-from nautilus_trader.model.orderbook.data import BookOrder
 from nautilus_trader.model.orderbook.ladder import Ladder
 
 
 def default_auction_match(left: Ladder, right: Ladder) -> tuple[list, list]:
     """Match bid/ask Ladders as default auction match function."""
     if not (left.top() and right.top()):
         return [], []
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/backtest/data_client.pxd` & `nautilus_trader-1.174.0/nautilus_trader/backtest/data_client.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/backtest/data_client.pyx` & `nautilus_trader-1.174.0/nautilus_trader/backtest/data_client.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/backtest/engine.pxd` & `nautilus_trader-1.174.0/nautilus_trader/backtest/engine.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/backtest/engine.pyx` & `nautilus_trader-1.174.0/nautilus_trader/backtest/engine.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 import pickle
 from decimal import Decimal
 from typing import Optional, Union
 
 import pandas as pd
 
+from nautilus_trader.accounting.error import AccountError
 from nautilus_trader.backtest.results import BacktestResult
 from nautilus_trader.common import Environment
 from nautilus_trader.config import BacktestEngineConfig
 from nautilus_trader.config import CacheConfig
 from nautilus_trader.config import CacheDatabaseConfig
 from nautilus_trader.config import DataEngineConfig
 from nautilus_trader.config import ExecEngineConfig
@@ -62,14 +63,15 @@
 from nautilus_trader.core.rust.common cimport TimeEventHandler_t
 from nautilus_trader.core.rust.common cimport vec_time_event_handlers_drop
 from nautilus_trader.core.rust.core cimport CVec
 from nautilus_trader.core.uuid cimport UUID4
 from nautilus_trader.execution.algorithm cimport ExecAlgorithm
 from nautilus_trader.model.data.bar cimport Bar
 from nautilus_trader.model.data.base cimport GenericData
+from nautilus_trader.model.data.book cimport ORDER_BOOK_DATA
 from nautilus_trader.model.data.tick cimport QuoteTick
 from nautilus_trader.model.data.tick cimport TradeTick
 from nautilus_trader.model.data.venue cimport InstrumentStatusUpdate
 from nautilus_trader.model.data.venue cimport VenueStatusUpdate
 from nautilus_trader.model.enums_c cimport AccountType
 from nautilus_trader.model.enums_c cimport AggregationSource
 from nautilus_trader.model.enums_c cimport BookType
@@ -78,15 +80,14 @@
 from nautilus_trader.model.identifiers cimport InstrumentId
 from nautilus_trader.model.identifiers cimport TraderId
 from nautilus_trader.model.identifiers cimport Venue
 from nautilus_trader.model.instruments.base cimport Instrument
 from nautilus_trader.model.instruments.currency_pair cimport CurrencyPair
 from nautilus_trader.model.objects cimport Currency
 from nautilus_trader.model.objects cimport Money
-from nautilus_trader.model.orderbook.data cimport OrderBookData
 from nautilus_trader.portfolio.base cimport PortfolioFacade
 from nautilus_trader.trading.strategy cimport Strategy
 from nautilus_trader.trading.trader cimport Trader
 
 
 cdef class BacktestEngine:
     """
@@ -853,17 +854,20 @@
         if self.kernel.risk_engine.is_running:
             self.kernel.risk_engine.stop()
         if self.kernel.exec_engine.is_running:
             self.kernel.exec_engine.stop()
         if self.kernel.emulator.is_running:
             self.kernel.emulator.stop()
 
-        # Process remaining messages
-        for exchange in self._venues.values():
-            exchange.process(self.kernel.clock.timestamp_ns())
+        try:
+            # Process remaining messages
+            for exchange in self._venues.values():
+                exchange.process(self.kernel.clock.timestamp_ns())
+        except AccountError:
+            pass
 
         self._run_finished = self._clock.utc_now()
         self._backtest_end = self.kernel.clock.utc_now()
         self._kernel.logger.change_clock(self._clock)
 
         self._log_post_run()
 
@@ -964,65 +968,73 @@
         cdef uint64_t i
         for i in range(self._data_len):
             if start_ns <= self._data[i].ts_init:
                 self._index = i
                 break
 
         # -- MAIN BACKTEST LOOP -----------------------------------------------#
+        cdef bint force_stop = False
         cdef uint64_t last_ns = 0
         cdef uint64_t raw_handlers_count = 0
         cdef Data data = self._next()
         cdef CVec raw_handlers
-        while data is not None:
-            if data.ts_init > end_ns:
-                # End of backtest
-                break
-            if data.ts_init > last_ns:
-                # Advance clocks to the next data time
-                raw_handlers = self._advance_time(data.ts_init, clocks)
-                raw_handlers_count = raw_handlers.len
-
-            # Process data through venue
-            if isinstance(data, OrderBookData):
-                self._venues[data.instrument_id.venue].process_order_book(data)
-            elif isinstance(data, QuoteTick):
-                self._venues[data.instrument_id.venue].process_quote_tick(data)
-            elif isinstance(data, TradeTick):
-                self._venues[data.instrument_id.venue].process_trade_tick(data)
-            elif isinstance(data, Bar):
-                self._venues[data.bar_type.instrument_id.venue].process_bar(data)
-            elif isinstance(data, VenueStatusUpdate):
-                self._venues[data.venue].process_venue_status(data)
-            elif isinstance(data, InstrumentStatusUpdate):
-                self._venues[data.instrument_id.venue].process_instrument_status(data)
-
-            self._data_engine.process(data)
-
-            # Process all exchange messages
-            for exchange in self._venues.values():
-                exchange.process(data.ts_init)
-
-            last_ns = data.ts_init
-            data = self._next()
-            if data is None or data.ts_init > last_ns:
-                # Finally process the time events
-                self._process_raw_time_event_handlers(
-                    raw_handlers,
-                    clocks,
-                    last_ns,
-                    only_now=True,
-                )
-
-                # Drop processed event handlers
-                vec_time_event_handlers_drop(raw_handlers)
-                raw_handlers_count = 0
-
-            self._iteration += 1
+        try:
+            while data is not None:
+                if data.ts_init > end_ns:
+                    # End of backtest
+                    break
+                if data.ts_init > last_ns:
+                    # Advance clocks to the next data time
+                    raw_handlers = self._advance_time(data.ts_init, clocks)
+                    raw_handlers_count = raw_handlers.len
+
+                # Process data through venue
+                if isinstance(data, ORDER_BOOK_DATA):
+                    self._venues[data.instrument_id.venue].process_order_book(data)
+                elif isinstance(data, QuoteTick):
+                    self._venues[data.instrument_id.venue].process_quote_tick(data)
+                elif isinstance(data, TradeTick):
+                    self._venues[data.instrument_id.venue].process_trade_tick(data)
+                elif isinstance(data, Bar):
+                    self._venues[data.bar_type.instrument_id.venue].process_bar(data)
+                elif isinstance(data, VenueStatusUpdate):
+                    self._venues[data.venue].process_venue_status(data)
+                elif isinstance(data, InstrumentStatusUpdate):
+                    self._venues[data.instrument_id.venue].process_instrument_status(data)
+
+                self._data_engine.process(data)
+
+                # Process all exchange messages
+                for exchange in self._venues.values():
+                    exchange.process(data.ts_init)
+
+                last_ns = data.ts_init
+                data = self._next()
+                if data is None or data.ts_init > last_ns:
+                    # Finally process the time events
+                    self._process_raw_time_event_handlers(
+                        raw_handlers,
+                        clocks,
+                        last_ns,
+                        only_now=True,
+                    )
+
+                    # Drop processed event handlers
+                    vec_time_event_handlers_drop(raw_handlers)
+                    raw_handlers_count = 0
+
+                self._iteration += 1
+        except AccountError as e:
+            force_stop = True
+            self._log.error(f"Stopping backtest from {e}.")
         # ---------------------------------------------------------------------#
 
+        if force_stop:
+            return
+
         # Process remaining messages
         for exchange in self._venues.values():
             exchange.process(self.kernel.clock.timestamp_ns())
 
         # Process remaining time events
         if raw_handlers_count > 0:
             self._process_raw_time_event_handlers(
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/backtest/exchange.pxd` & `nautilus_trader-1.174.0/nautilus_trader/backtest/exchange.pxd`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from nautilus_trader.backtest.matching_engine cimport OrderMatchingEngine
 from nautilus_trader.backtest.models cimport FillModel
 from nautilus_trader.backtest.models cimport LatencyModel
 from nautilus_trader.cache.cache cimport Cache
 from nautilus_trader.common.clock cimport Clock
 from nautilus_trader.common.logging cimport LoggerAdapter
 from nautilus_trader.common.queue cimport Queue
+from nautilus_trader.core.data cimport Data
 from nautilus_trader.execution.messages cimport TradingCommand
 from nautilus_trader.model.currency cimport Currency
 from nautilus_trader.model.data.bar cimport Bar
 from nautilus_trader.model.data.tick cimport QuoteTick
 from nautilus_trader.model.data.tick cimport TradeTick
 from nautilus_trader.model.data.venue cimport InstrumentStatusUpdate
 from nautilus_trader.model.data.venue cimport VenueStatusUpdate
@@ -36,15 +37,14 @@
 from nautilus_trader.model.enums_c cimport OmsType
 from nautilus_trader.model.identifiers cimport InstrumentId
 from nautilus_trader.model.identifiers cimport Venue
 from nautilus_trader.model.instruments.base cimport Instrument
 from nautilus_trader.model.objects cimport Money
 from nautilus_trader.model.objects cimport Price
 from nautilus_trader.model.orderbook.book cimport OrderBook
-from nautilus_trader.model.orderbook.data cimport OrderBookData
 from nautilus_trader.msgbus.bus cimport MessageBus
 
 
 cdef class SimulatedExchange:
     cdef Clock _clock
     cdef LoggerAdapter _log
 
@@ -115,15 +115,15 @@
     cpdef Account get_account(self)
 
 # -- COMMANDS -------------------------------------------------------------------------------------
 
     cpdef void adjust_account(self, Money adjustment)
     cdef tuple generate_inflight_command(self, TradingCommand command)
     cpdef void send(self, TradingCommand command)
-    cpdef void process_order_book(self, OrderBookData data)
+    cpdef void process_order_book(self, Data data)
     cpdef void process_quote_tick(self, QuoteTick tick)
     cpdef void process_trade_tick(self, TradeTick tick)
     cpdef void process_bar(self, Bar bar)
     cpdef void process_venue_status(self, VenueStatusUpdate update)
     cpdef void process_instrument_status(self, InstrumentStatusUpdate update)
     cpdef void process(self, uint64_t ts_now)
     cpdef void reset(self)
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/backtest/exchange.pyx` & `nautilus_trader-1.174.0/nautilus_trader/backtest/exchange.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -614,21 +614,21 @@
             raise ValueError(f"invalid `TradingCommand`, was {command}")  # pragma: no cover (design-time error)
         if ts not in self._inflight_counter:
             self._inflight_counter[ts] = 0
         self._inflight_counter[ts] += 1
         cdef (uint64_t, uint64_t) key = (ts, self._inflight_counter[ts])
         return key, command
 
-    cpdef void process_order_book(self, OrderBookData data):
+    cpdef void process_order_book(self, Data data):
         """
         Process the exchanges market for the given order book data.
 
         Parameters
         ----------
-        data : OrderBookData
+        data : OrderBookDelta, OrderBookDeltas, OrderBookSnapshot
             The order book data to process.
 
         """
         Condition.not_none(data, "data")
 
         cdef OrderMatchingEngine matching_engine = self._matching_engines.get(data.instrument_id)
         if matching_engine is None:
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/backtest/execution_client.pxd` & `nautilus_trader-1.174.0/nautilus_trader/backtest/execution_client.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/backtest/execution_client.pyx` & `nautilus_trader-1.174.0/nautilus_trader/backtest/execution_client.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/backtest/matching_engine.pxd` & `nautilus_trader-1.174.0/nautilus_trader/backtest/matching_engine.pxd`

 * *Files 2% similar despite different names*

```diff
@@ -16,20 +16,22 @@
 from libc.stdint cimport int64_t
 from libc.stdint cimport uint64_t
 
 from nautilus_trader.backtest.models cimport FillModel
 from nautilus_trader.cache.base cimport CacheFacade
 from nautilus_trader.common.clock cimport Clock
 from nautilus_trader.common.logging cimport LoggerAdapter
+from nautilus_trader.core.data cimport Data
 from nautilus_trader.execution.matching_core cimport MatchingCore
 from nautilus_trader.execution.messages cimport CancelAllOrders
 from nautilus_trader.execution.messages cimport CancelOrder
 from nautilus_trader.execution.messages cimport ModifyOrder
 from nautilus_trader.model.currency cimport Currency
 from nautilus_trader.model.data.bar cimport Bar
+from nautilus_trader.model.data.book cimport BookOrder
 from nautilus_trader.model.data.tick cimport QuoteTick
 from nautilus_trader.model.data.tick cimport TradeTick
 from nautilus_trader.model.enums_c cimport BookType
 from nautilus_trader.model.enums_c cimport LiquiditySide
 from nautilus_trader.model.enums_c cimport MarketStatus
 from nautilus_trader.model.enums_c cimport OmsType
 from nautilus_trader.model.enums_c cimport TimeInForce
@@ -43,16 +45,14 @@
 from nautilus_trader.model.identifiers cimport Venue
 from nautilus_trader.model.identifiers cimport VenueOrderId
 from nautilus_trader.model.instruments.base cimport Instrument
 from nautilus_trader.model.objects cimport Money
 from nautilus_trader.model.objects cimport Price
 from nautilus_trader.model.objects cimport Quantity
 from nautilus_trader.model.orderbook.book cimport OrderBook
-from nautilus_trader.model.orderbook.data cimport BookOrder
-from nautilus_trader.model.orderbook.data cimport OrderBookData
 from nautilus_trader.model.orders.base cimport Order
 from nautilus_trader.model.orders.limit cimport LimitOrder
 from nautilus_trader.model.orders.limit_if_touched cimport LimitIfTouchedOrder
 from nautilus_trader.model.orders.market cimport MarketOrder
 from nautilus_trader.model.orders.market_if_touched cimport MarketIfTouchedOrder
 from nautilus_trader.model.orders.market_to_limit cimport MarketToLimitOrder
 from nautilus_trader.model.orders.stop_limit cimport StopLimitOrder
@@ -117,15 +117,15 @@
     cpdef list get_open_orders(self)
     cpdef list get_open_bid_orders(self)
     cpdef list get_open_ask_orders(self)
     cpdef bint order_exists(self, ClientOrderId client_order_id)
 
 # -- DATA PROCESSING ------------------------------------------------------------------------------
 
-    cpdef void process_order_book(self, OrderBookData data)
+    cpdef void process_order_book(self, Data data)
     cpdef void process_quote_tick(self, QuoteTick tick)
     cpdef void process_trade_tick(self, TradeTick tick)
     cpdef void process_bar(self, Bar bar)
     cpdef void process_status(self, MarketStatus status)
     cpdef void process_auction_book(self, OrderBook book)
     cdef void _process_trade_ticks_from_bar(self, Bar bar)
     cdef void _process_quote_ticks_from_bar(self)
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/backtest/matching_engine.pyx` & `nautilus_trader-1.174.0/nautilus_trader/backtest/matching_engine.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -23,21 +23,23 @@
 
 from nautilus_trader.backtest.models cimport FillModel
 from nautilus_trader.cache.base cimport CacheFacade
 from nautilus_trader.common.clock cimport TestClock
 from nautilus_trader.common.logging cimport LogColor
 from nautilus_trader.common.logging cimport Logger
 from nautilus_trader.core.correctness cimport Condition
+from nautilus_trader.core.data cimport Data
 from nautilus_trader.core.rust.model cimport Price_t
 from nautilus_trader.core.rust.model cimport price_new
 from nautilus_trader.core.rust.model cimport trade_id_new
 from nautilus_trader.core.string cimport pystr_to_cstr
 from nautilus_trader.core.uuid cimport UUID4
 from nautilus_trader.execution.matching_core cimport MatchingCore
 from nautilus_trader.execution.trailing cimport TrailingStopCalculator
+from nautilus_trader.model.data.book cimport BookOrder
 from nautilus_trader.model.data.tick cimport QuoteTick
 from nautilus_trader.model.data.tick cimport TradeTick
 from nautilus_trader.model.enums_c cimport AggressorSide
 from nautilus_trader.model.enums_c cimport BookType
 from nautilus_trader.model.enums_c cimport ContingencyType
 from nautilus_trader.model.enums_c cimport DepthType
 from nautilus_trader.model.enums_c cimport LiquiditySide
@@ -67,15 +69,14 @@
 from nautilus_trader.model.identifiers cimport TraderId
 from nautilus_trader.model.identifiers cimport VenueOrderId
 from nautilus_trader.model.instruments.base cimport Instrument
 from nautilus_trader.model.objects cimport Money
 from nautilus_trader.model.objects cimport Price
 from nautilus_trader.model.objects cimport Quantity
 from nautilus_trader.model.orderbook.book cimport OrderBook
-from nautilus_trader.model.orderbook.data cimport BookOrder
 from nautilus_trader.model.orders.base cimport Order
 from nautilus_trader.model.orders.limit cimport LimitOrder
 from nautilus_trader.model.orders.limit_if_touched cimport LimitIfTouchedOrder
 from nautilus_trader.model.orders.market cimport MarketOrder
 from nautilus_trader.model.orders.market_if_touched cimport MarketIfTouchedOrder
 from nautilus_trader.model.orders.market_to_limit cimport MarketToLimitOrder
 from nautilus_trader.model.orders.stop_limit cimport StopLimitOrder
@@ -312,37 +313,40 @@
         return self._core.get_orders_ask()
 
     cpdef bint order_exists(self, ClientOrderId client_order_id):
         return self._core.order_exists(client_order_id)
 
 # -- DATA PROCESSING ------------------------------------------------------------------------------
 
-    cpdef void process_order_book(self, OrderBookData data):
+    cpdef void process_order_book(self, Data data):
         """
         Process the exchanges market for the given order book data.
 
         Parameters
         ----------
-        data : OrderBookData
+        data : OrderBookDelta, OrderBookDeltas, OrderBookSnapshot
             The order book data to process.
 
         """
         Condition.not_none(data, "data")
 
         if not self._log.is_bypassed:
             self._log.debug(f"Processing {repr(data)}...")
 
-        if data.time_in_force == TimeInForce.GTC:
-            self._book.apply(data)
-        elif data.time_in_force == TimeInForce.AT_THE_OPEN:
-            self._opening_auction_book.apply(data)
-        elif data.time_in_force == TimeInForce.AT_THE_CLOSE:
-            self._closing_auction_book.apply(data)
-        else:
-            raise RuntimeError(data.time_in_force)
+        self._book.apply(data)
+
+        # TODO(cs): WIP to introduce flags
+        # if data.flags == TimeInForce.GTC:
+        #     self._book.apply(data)
+        # elif data.flags == TimeInForce.AT_THE_OPEN:
+        #     self._opening_auction_book.apply(data)
+        # elif data.flags == TimeInForce.AT_THE_CLOSE:
+        #     self._closing_auction_book.apply(data)
+        # else:
+        #     raise RuntimeError(data.time_in_force)
 
         self.iterate(data.ts_init)
 
     cpdef void process_quote_tick(self, QuoteTick tick) :
         """
         Process the exchanges market for the given quote tick.
 
@@ -599,15 +603,15 @@
                 return  # Order rejected
             elif parent.status_c() == OrderStatus.ACCEPTED or parent.status_c() == OrderStatus.TRIGGERED:
                 self._log.info(f"Pending OTO {order.client_order_id} triggers from {parent.client_order_id}")
                 return  # Pending trigger
 
         # Check reduce-only instruction
         cdef Position position
-        if order.is_reduce_only:
+        if order.is_reduce_only and not order.is_closed_c():
             position = self.cache.position_for_order(order.client_order_id)
             if (
                 not position
                 or position.is_closed_c()
                 or (order.is_buy_c() and position.is_long_c())
                 or (order.is_sell_c() and position.is_short_c())
             ):
@@ -1628,15 +1632,15 @@
         # Check contingency orders
         cdef ClientOrderId client_order_id
         cdef Order child_order
         if order.contingency_type == ContingencyType.OTO:
             for client_order_id in order.linked_order_ids:
                 child_order = self.cache.order(client_order_id)
                 assert child_order is not None, "OTO child order not found"
-                if child_order.position_id is None:
+                if child_order.position_id is None and order.position_id is not None:
                     self.cache.add_position_id(
                         position_id=order.position_id,
                         venue=self.venue,
                         client_order_id=client_order_id,
                         strategy_id=child_order.strategy_id,
                     )
                     self._log.debug(
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/backtest/models.pxd` & `nautilus_trader-1.174.0/nautilus_trader/backtest/models.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/backtest/models.pyx` & `nautilus_trader-1.174.0/nautilus_trader/backtest/models.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/backtest/modules.pxd` & `nautilus_trader-1.174.0/nautilus_trader/backtest/modules.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/backtest/modules.pyx` & `nautilus_trader-1.174.0/nautilus_trader/backtest/modules.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/backtest/node.py` & `nautilus_trader-1.174.0/nautilus_trader/backtest/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         If `configs` contains a type other than `BacktestRunConfig`.
     """
 
     def __init__(self, configs: list[BacktestRunConfig]):
         PyCondition.not_none(configs, "configs")
         PyCondition.not_empty(configs, "configs")
         PyCondition.true(
-            all([isinstance(config, BacktestRunConfig) for config in configs]),
+            all(isinstance(config, BacktestRunConfig) for config in configs),
             "configs",
         )
 
         self._validate_configs(configs)
 
         # Configuration
         self._configs: list[BacktestRunConfig] = configs
@@ -109,15 +109,15 @@
         Returns
         -------
         list[BacktestEngine]
 
         """
         return list(self._engines.values())
 
-    def run(self) -> list[BacktestResult]:  # noqa (kwargs for extensibility)
+    def run(self) -> list[BacktestResult]:
         """
         Execute a group of backtest run configs synchronously.
 
         Returns
         -------
         list[BacktestResult]
             The results of the backtest runs.
@@ -162,20 +162,19 @@
         # Build the backtest engine
         engine = BacktestEngine(config=config)
         self._engines[run_config_id] = engine
 
         # Add venues (must be added prior to instruments)
         for config in venue_configs:
             base_currency: Optional[str] = config.base_currency
-            if config.leverages:
-                leverages = {
-                    InstrumentId.from_str(i): Decimal(v) for i, v in config.leverages.items()
-                }
-            else:
-                leverages = {}
+            leverages = (
+                {InstrumentId.from_str(i): Decimal(v) for i, v in config.leverages.items()}
+                if config.leverages
+                else {}
+            )
             engine.add_venue(
                 venue=Venue(config.name),
                 oms_type=OmsType[config.oms_type],
                 account_type=AccountType[config.account_type],
                 base_currency=Currency.from_str(base_currency) if base_currency else None,
                 starting_balances=[Money.from_str(m) for m in config.starting_balances],
                 default_leverage=Decimal(config.default_leverage),
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/backtest/results.py` & `nautilus_trader-1.174.0/nautilus_trader/backtest/results.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/cache/__init__.pxd` & `nautilus_trader-1.174.0/nautilus_trader/common/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/cache/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/cache/base.pxd` & `nautilus_trader-1.174.0/nautilus_trader/cache/base.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/cache/base.pyx` & `nautilus_trader-1.174.0/nautilus_trader/cache/base.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/cache/cache.pxd` & `nautilus_trader-1.174.0/nautilus_trader/cache/cache.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/cache/cache.pyx` & `nautilus_trader-1.174.0/nautilus_trader/cache/cache.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/cache/database.pxd` & `nautilus_trader-1.174.0/nautilus_trader/cache/database.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/cache/database.pyx` & `nautilus_trader-1.174.0/nautilus_trader/cache/database.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/common/__init__.pxd` & `nautilus_trader-1.174.0/nautilus_trader/core/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/common/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/common/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/common/actor.pxd` & `nautilus_trader-1.174.0/nautilus_trader/common/actor.pxd`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 from nautilus_trader.model.data.venue cimport VenueStatusUpdate
 from nautilus_trader.model.enums_c cimport BookType
 from nautilus_trader.model.identifiers cimport ClientId
 from nautilus_trader.model.identifiers cimport InstrumentId
 from nautilus_trader.model.identifiers cimport Venue
 from nautilus_trader.model.instruments.base cimport Instrument
 from nautilus_trader.model.orderbook.book cimport OrderBook
-from nautilus_trader.model.orderbook.data cimport OrderBookData
 from nautilus_trader.msgbus.bus cimport MessageBus
 
 
 cdef class Actor(Component):
     cdef set _warning_events
     cdef dict _signal_classes
 
@@ -72,15 +71,15 @@
     cpdef void on_dispose(self)
     cpdef void on_degrade(self)
     cpdef void on_fault(self)
     cpdef void on_venue_status_update(self, VenueStatusUpdate update)
     cpdef void on_instrument_status_update(self, InstrumentStatusUpdate update)
     cpdef void on_instrument_close(self, InstrumentClose update)
     cpdef void on_instrument(self, Instrument instrument)
-    cpdef void on_order_book_delta(self, OrderBookData delta)
+    cpdef void on_order_book_delta(self, Data data)
     cpdef void on_order_book(self, OrderBook order_book)
     cpdef void on_ticker(self, Ticker ticker)
     cpdef void on_quote_tick(self, QuoteTick tick)
     cpdef void on_trade_tick(self, TradeTick tick)
     cpdef void on_bar(self, Bar bar)
     cpdef void on_data(self, Data data)
     cpdef void on_historical_data(self, Data data)
@@ -178,15 +177,15 @@
     )
 
 # -- HANDLERS -------------------------------------------------------------------------------------
 
     cpdef void handle_instrument(self, Instrument instrument)
     cpdef void handle_instruments(self, list instruments)
     cpdef void handle_order_book(self, OrderBook order_book)
-    cpdef void handle_order_book_delta(self, OrderBookData data)
+    cpdef void handle_order_book_delta(self, Data data)
     cpdef void handle_ticker(self, Ticker ticker)
     cpdef void handle_quote_tick(self, QuoteTick tick)
     cpdef void handle_quote_ticks(self, list ticks)
     cpdef void handle_trade_tick(self, TradeTick tick)
     cpdef void handle_trade_ticks(self, list ticks)
     cpdef void handle_bar(self, Bar bar)
     cpdef void handle_bars(self, list bars)
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/common/actor.pyx` & `nautilus_trader-1.174.0/nautilus_trader/common/actor.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -52,28 +52,28 @@
 from nautilus_trader.data.messages cimport DataRequest
 from nautilus_trader.data.messages cimport DataResponse
 from nautilus_trader.data.messages cimport Subscribe
 from nautilus_trader.data.messages cimport Unsubscribe
 from nautilus_trader.model.data.bar cimport Bar
 from nautilus_trader.model.data.bar cimport BarType
 from nautilus_trader.model.data.base cimport DataType
+from nautilus_trader.model.data.book cimport OrderBookDelta
+from nautilus_trader.model.data.book cimport OrderBookSnapshot
 from nautilus_trader.model.data.tick cimport QuoteTick
 from nautilus_trader.model.data.tick cimport TradeTick
 from nautilus_trader.model.data.ticker cimport Ticker
 from nautilus_trader.model.data.venue cimport InstrumentClose
 from nautilus_trader.model.data.venue cimport InstrumentStatusUpdate
 from nautilus_trader.model.data.venue cimport VenueStatusUpdate
 from nautilus_trader.model.enums_c cimport BookType
 from nautilus_trader.model.identifiers cimport ClientId
 from nautilus_trader.model.identifiers cimport ComponentId
 from nautilus_trader.model.identifiers cimport InstrumentId
 from nautilus_trader.model.identifiers cimport Venue
 from nautilus_trader.model.instruments.base cimport Instrument
-from nautilus_trader.model.orderbook.data cimport OrderBookData
-from nautilus_trader.model.orderbook.data cimport OrderBookSnapshot
 from nautilus_trader.msgbus.bus cimport MessageBus
 
 
 cdef class Actor(Component):
     """
     The base class for all actor components.
 
@@ -366,22 +366,22 @@
         Warnings
         --------
         System method (not intended to be called by user code).
 
         """
         # Optionally override in subclass
 
-    cpdef void on_order_book_delta(self, OrderBookData delta):
+    cpdef void on_order_book_delta(self, Data data):
         """
-        Actions to be performed when running and receives an order book delta.
+        Actions to be performed when running and receives order book data.
 
         Parameters
         ----------
         delta : OrderBookDelta, OrderBookDeltas, OrderBookSnapshot
-            The order book delta received.
+            The order book data received.
 
         Warnings
         --------
         System method (not intended to be called by user code).
 
         """
         # Optionally override in subclass
@@ -779,16 +779,16 @@
         InstrumentId instrument_id,
         BookType book_type=BookType.L2_MBP,
         int depth = 0,
         dict kwargs = None,
         ClientId client_id = None,
     ):
         """
-        Subscribe to the order book deltas stream, being a snapshot then deltas
-        `OrderBookData` for the given instrument ID.
+        Subscribe to the order book data stream, being a snapshot then deltas
+        for the given instrument ID.
 
         Parameters
         ----------
         instrument_id : InstrumentId
             The order book instrument ID to subscribe to.
         book_type : BookType {``L1_TBBO``, ``L2_MBP``, ``L3_MBO``}
             The order book type.
@@ -810,15 +810,15 @@
                   f".{instrument_id.symbol}",
             handler=self.handle_order_book_delta,
         )
 
         cdef Subscribe command = Subscribe(
             client_id=client_id,
             venue=instrument_id.venue,
-            data_type=DataType(OrderBookData, metadata={
+            data_type=DataType(OrderBookDelta, metadata={
                 "instrument_id": instrument_id,
                 "book_type": book_type,
                 "depth": depth,
                 "kwargs": kwargs,
             }),
             command_id=UUID4(),
             ts_init=self._clock.timestamp_ns(),
@@ -1246,15 +1246,15 @@
                   f".{instrument_id.symbol}",
             handler=self.handle_order_book_delta,
         )
 
         cdef Unsubscribe command = Unsubscribe(
             client_id=client_id,
             venue=instrument_id.venue,
-            data_type=DataType(OrderBookData, metadata={"instrument_id": instrument_id}),
+            data_type=DataType(OrderBookDelta, metadata={"instrument_id": instrument_id}),
             command_id=UUID4(),
             ts_init=self._clock.timestamp_ns(),
         )
 
         self._send_data_cmd(command)
 
     cpdef void unsubscribe_order_book_snapshots(
@@ -1862,15 +1862,15 @@
         else:
             self._log.warning("Received <Instrument[]> data with no instruments.")
 
         cdef int i
         for i in range(length):
             self.handle_instrument(instruments[i])
 
-    cpdef void handle_order_book_delta(self, OrderBookData delta):
+    cpdef void handle_order_book_delta(self, Data data):
         """
         Handle the given order book data.
 
         Passes to `on_order_book_delta` if state is ``RUNNING``.
 
         Parameters
         ----------
@@ -1878,21 +1878,21 @@
             The order book delta received.
 
         Warnings
         --------
         System method (not intended to be called by user code).
 
         """
-        Condition.not_none(delta, "data")
+        Condition.not_none(data, "data")
 
         if self._fsm.state == ComponentState.RUNNING:
             try:
-                self.on_order_book_delta(delta)
+                self.on_order_book_delta(data)
             except Exception as e:
-                self._log.exception(f"Error on handling {repr(delta)}", e)
+                self._log.exception(f"Error on handling {repr(data)}", e)
                 raise
 
     cpdef void handle_order_book(self, OrderBook order_book):
         """
         Handle the given order book snapshot.
 
         Passes to `on_order_book` if state is ``RUNNING``.
@@ -2213,34 +2213,31 @@
                 self._log.exception(f"Error on handling {repr(data)}", e)
                 raise
 
     cpdef void handle_historical_data(self, Data data):
         """
         Handle the given historical data.
 
-        If state is ``RUNNING`` then passes to `on_historical_data`.
-
         Parameters
         ----------
         data : Data
             The historical data received.
 
         Warnings
         --------
         System method (not intended to be called by user code).
 
         """
         Condition.not_none(data, "data")
 
-        if self._fsm.state == ComponentState.RUNNING:
-            try:
-                self.on_historical_data(data)
-            except Exception as e:
-                self._log.exception(f"Error on handling {repr(data)}", e)
-                raise
+        try:
+            self.on_historical_data(data)
+        except Exception as e:
+            self._log.exception(f"Error on handling {repr(data)}", e)
+            raise
 
     cpdef void handle_event(self, Event event):
         """
         Handle the given event.
 
         If state is ``RUNNING`` then passes to `on_event`.
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/common/clock.pxd` & `nautilus_trader-1.174.0/nautilus_trader/common/clock.pxd`

 * *Files 1% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 from cpython.datetime cimport timedelta
 from cpython.datetime cimport tzinfo
 from libc.stdint cimport int64_t
 from libc.stdint cimport uint64_t
 
 from nautilus_trader.common.timer cimport LiveTimer
 from nautilus_trader.common.timer cimport TimeEvent
-from nautilus_trader.core.rust.common cimport LiveClockAPI
-from nautilus_trader.core.rust.common cimport TestClockAPI
+from nautilus_trader.core.rust.common cimport LiveClock_API
+from nautilus_trader.core.rust.common cimport TestClock_API
 from nautilus_trader.core.rust.core cimport CVec
 
 
 cdef class Clock:
     cpdef double timestamp(self)
     cpdef uint64_t timestamp_ms(self)
     cpdef uint64_t timestamp_ns(self)
@@ -65,23 +65,23 @@
         callback: Callable[[TimeEvent], None]=*,
     )
     cpdef void cancel_timer(self, str name)
     cpdef void cancel_timers(self)
 
 
 cdef class TestClock(Clock):
-    cdef TestClockAPI _mem
+    cdef TestClock_API _mem
 
     cpdef void set_time(self, uint64_t to_time_ns)
     cdef CVec advance_time_c(self, uint64_t to_time_ns, bint set_time=*)
     cpdef list advance_time(self, uint64_t to_time_ns, bint set_time=*)
 
 
 cdef class LiveClock(Clock):
-    cdef LiveClockAPI _mem
+    cdef LiveClock_API _mem
     cdef object _default_handler
     cdef dict _handlers
 
     cdef object _loop
     cdef int _timer_count
     cdef dict _timers
     cdef LiveTimer[:] _stack
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/common/clock.pyx` & `nautilus_trader-1.174.0/nautilus_trader/common/clock.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/common/component.pxd` & `nautilus_trader-1.174.0/nautilus_trader/common/component.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/common/component.pyx` & `nautilus_trader-1.174.0/nautilus_trader/common/component.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/common/enums.pyx` & `nautilus_trader-1.174.0/nautilus_trader/common/enums.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/common/enums_c.pxd` & `nautilus_trader-1.174.0/nautilus_trader/common/enums_c.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/common/enums_c.pyx` & `nautilus_trader-1.174.0/nautilus_trader/common/enums_c.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/common/factories.pxd` & `nautilus_trader-1.174.0/nautilus_trader/common/factories.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/common/factories.pyx` & `nautilus_trader-1.174.0/nautilus_trader/common/factories.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/common/functions.py` & `nautilus_trader-1.174.0/nautilus_trader/common/functions.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/common/generators.pxd` & `nautilus_trader-1.174.0/nautilus_trader/common/generators.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/common/generators.pyx` & `nautilus_trader-1.174.0/nautilus_trader/common/generators.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/common/logging.pxd` & `nautilus_trader-1.174.0/nautilus_trader/common/logging.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/common/logging.pyx` & `nautilus_trader-1.174.0/nautilus_trader/common/logging.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/common/messages.pxd` & `nautilus_trader-1.174.0/nautilus_trader/common/messages.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/common/messages.pyx` & `nautilus_trader-1.174.0/nautilus_trader/common/messages.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/common/providers.py` & `nautilus_trader-1.174.0/nautilus_trader/common/providers.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/common/queue.pxd` & `nautilus_trader-1.174.0/nautilus_trader/common/queue.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/common/queue.pyx` & `nautilus_trader-1.174.0/nautilus_trader/common/queue.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/common/throttler.pxd` & `nautilus_trader-1.174.0/nautilus_trader/common/throttler.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/common/throttler.pyx` & `nautilus_trader-1.174.0/nautilus_trader/common/throttler.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/common/timer.pxd` & `nautilus_trader-1.174.0/nautilus_trader/common/timer.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/common/timer.pyx` & `nautilus_trader-1.174.0/nautilus_trader/common/timer.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/config/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/config/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/config/backtest.py` & `nautilus_trader-1.174.0/nautilus_trader/config/backtest.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,24 +87,24 @@
     def query(self):
         if self.data_cls is Bar and self.bar_spec:
             bar_type = f"{self.instrument_id}-{self.bar_spec}-EXTERNAL"
             filter_expr = f'field("bar_type") == "{bar_type}"'
         else:
             filter_expr = self.filter_expr
 
-        return dict(
-            cls=self.data_type,
-            instrument_ids=[self.instrument_id] if self.instrument_id else None,
-            start=self.start_time,
-            end=self.end_time,
-            filter_expr=parse_filters_expr(filter_expr),
-            as_nautilus=True,
-            metadata=self.metadata,
-            use_rust=self.use_rust,
-        )
+        return {
+            "cls": self.data_type,
+            "instrument_ids": [self.instrument_id] if self.instrument_id else None,
+            "start": self.start_time,
+            "end": self.end_time,
+            "filter_expr": parse_filters_expr(filter_expr),
+            "as_nautilus": True,
+            "metadata": self.metadata,
+            "use_rust": self.use_rust,
+        }
 
     @property
     def start_time_nanos(self) -> int:
         if self.start_time is None:
             return 0
         return maybe_dt_to_unix_nanos(pd.Timestamp(self.start_time))
 
@@ -252,15 +252,15 @@
 
     def safer_eval(input_string):
         allowed_names = {"field": field}
         code = compile(input_string, "<string>", "eval")
         for name in code.co_names:
             if name not in allowed_names:
                 raise NameError(f"Use of {name} not allowed")
-        return eval(code, {}, allowed_names)  # noqa: S307
+        return eval(code, {}, allowed_names)
 
     return safer_eval(s)  # Only allow use of the field object
 
 
 CUSTOM_ENCODINGS: dict[type, Callable] = {
     pd.DataFrame: lambda x: x.to_json(),
 }
@@ -276,13 +276,12 @@
         return func(x)
     raise TypeError(f"Objects of type {type(x)} are not supported")
 
 
 def register_json_encoding(type_: type, encoder: Callable) -> None:
     global CUSTOM_ENCODINGS
     CUSTOM_ENCODINGS[type_] = encoder
-    return None
 
 
 def tokenize_config(obj: dict) -> str:
     value: bytes = msgspec.json.encode(obj, enc_hook=json_encoder)
     return hashlib.sha256(value).hexdigest()
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/config/common.py` & `nautilus_trader-1.174.0/nautilus_trader/config/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
 
         """
         return bool(msgspec.json.decode(self.json(), type=self.__class__))
 
 
 class CacheConfig(NautilusConfig, frozen=True):
     """
-    Configuration for a ``Cache`` instance.
+    Configuration for ``Cache`` instances.
 
     Parameters
     ----------
     tick_capacity : PositiveInt
         The maximum length for internal tick dequeues.
     bar_capacity : PositiveInt
         The maximum length for internal bar dequeues.
@@ -121,15 +121,15 @@
 
     tick_capacity: PositiveInt = 1000
     bar_capacity: PositiveInt = 1000
 
 
 class CacheDatabaseConfig(NautilusConfig, frozen=True):
     """
-    Configuration for a ``CacheDatabase`` instance.
+    Configuration for ``CacheDatabase`` instances.
 
     Parameters
     ----------
     type : str, {'in-memory', 'redis'}, default 'in-memory'
         The database type.
     host : str, default 'localhost'
         The database host address.
@@ -152,15 +152,15 @@
     password: Optional[str] = None
     ssl: bool = False
     flush: bool = False
 
 
 class InstrumentProviderConfig(NautilusConfig, frozen=True):
     """
-    Configuration for an ``InstrumentProvider`` instance.
+    Configuration for ``InstrumentProvider`` instances.
 
     Parameters
     ----------
     load_all : bool, default False
         If all venue instruments should be loaded on start.
     load_ids : FrozenSet[str], optional
         The list of instrument IDs to be loaded on start (if `load_all_instruments` is False).
@@ -188,15 +188,15 @@
     filters: Optional[dict[str, Any]] = None
     filter_callable: Optional[str] = None
     log_warnings: bool = True
 
 
 class DataEngineConfig(NautilusConfig, frozen=True):
     """
-    Configuration for a ``DataEngine`` instance.
+    Configuration for ``DataEngine`` instances.
 
     Parameters
     ----------
     time_bars_build_with_no_updates : bool, default True
         If time bar aggregators will build and emit bars with no new market updates.
     time_bars_timestamp_on_close : bool, default True
         If time bar aggregators will timestamp `ts_event` on bar close.
@@ -211,15 +211,15 @@
     time_bars_timestamp_on_close: bool = True
     validate_data_sequence: bool = False
     debug: bool = False
 
 
 class RiskEngineConfig(NautilusConfig, frozen=True):
     """
-    Configuration for a ``RiskEngine`` instance.
+    Configuration for ``RiskEngine`` instances.
 
     Parameters
     ----------
     bypass : bool, default False
         If True then will bypass all pre-trade risk checks and rate limits (will still check for duplicate IDs).
     max_order_submit_rate : str, default 100/00:00:01
         The maximum rate of submit order commands per timedelta.
@@ -237,15 +237,15 @@
     max_order_modify_rate: str = "100/00:00:01"
     max_notional_per_order: dict[str, int] = {}
     debug: bool = False
 
 
 class ExecEngineConfig(NautilusConfig, frozen=True):
     """
-    Configuration for an ``ExecutionEngine`` instance.
+    Configuration for ``ExecutionEngine`` instances.
 
     Parameters
     ----------
     load_cache : bool, default True
         If the cache should be loaded on initialization.
     allow_cash_positions : bool, default True
         If unleveraged spot/cash assets should generate positions.
@@ -256,15 +256,15 @@
     load_cache: bool = True
     allow_cash_positions: bool = True
     debug: bool = False
 
 
 class OrderEmulatorConfig(NautilusConfig, frozen=True):
     """
-    Configuration for an ``OrderEmulator`` instance.
+    Configuration for ``OrderEmulator`` instances.
     """
 
 
 class StreamingConfig(NautilusConfig, frozen=True):
     """
     Configuration for streaming live or backtest runs to the catalog in feather format.
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/config/error.py` & `nautilus_trader-1.174.0/nautilus_trader/config/error.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/config/live.py` & `nautilus_trader-1.174.0/nautilus_trader/config/live.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/config/validation.py` & `nautilus_trader-1.174.0/nautilus_trader/config/validation.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/core/__init__.pxd` & `nautilus_trader-1.174.0/nautilus_trader/core/rust/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/core/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/core/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/core/asynchronous.py` & `nautilus_trader-1.174.0/nautilus_trader/core/asynchronous.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/core/correctness.pxd` & `nautilus_trader-1.174.0/nautilus_trader/core/correctness.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/core/correctness.pyx` & `nautilus_trader-1.174.0/nautilus_trader/core/correctness.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/core/data.pxd` & `nautilus_trader-1.174.0/nautilus_trader/core/data.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/core/data.pyx` & `nautilus_trader-1.174.0/nautilus_trader/core/data.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/core/datetime.pxd` & `nautilus_trader-1.174.0/nautilus_trader/core/datetime.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/core/datetime.pyx` & `nautilus_trader-1.174.0/nautilus_trader/core/datetime.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/core/fsm.pxd` & `nautilus_trader-1.174.0/nautilus_trader/core/fsm.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/core/fsm.pyx` & `nautilus_trader-1.174.0/nautilus_trader/core/fsm.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/core/includes/backtest.h` & `nautilus_trader-1.174.0/nautilus_trader/core/includes/backtest.h`

 * *Files 0% similar despite different names*

```diff
@@ -15,12 +15,12 @@
 } TimeEventAccumulatorAPI;
 
 struct TimeEventAccumulatorAPI time_event_accumulator_new(void);
 
 void time_event_accumulator_drop(struct TimeEventAccumulatorAPI accumulator);
 
 void time_event_accumulator_advance_clock(struct TimeEventAccumulatorAPI *accumulator,
-                                          TestClockAPI *clock,
+                                          TestClock_API *clock,
                                           uint64_t to_time_ns,
                                           uint8_t set_time);
 
 CVec time_event_accumulator_drain(struct TimeEventAccumulatorAPI *accumulator);
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/core/includes/common.h` & `nautilus_trader-1.174.0/nautilus_trader/core/includes/common.h`

 * *Files 6% similar despite different names*

```diff
@@ -62,21 +62,21 @@
 
 typedef struct Logger_t Logger_t;
 
 typedef struct Rc_String Rc_String;
 
 typedef struct TestClock TestClock;
 
-typedef struct TestClockAPI {
+typedef struct TestClock_API {
     struct TestClock *_0;
-} TestClockAPI;
+} TestClock_API;
 
-typedef struct LiveClockAPI {
+typedef struct LiveClock_API {
     struct LiveClock *_0;
-} LiveClockAPI;
+} LiveClock_API;
 
 /**
  * Logger is not C FFI safe, so we box and pass it as an opaque pointer.
  * This works because Logger fields don't need to be accessed, only functions
  * are called.
  */
 typedef struct CLogger {
@@ -115,93 +115,93 @@
     struct TimeEvent_t event;
     /**
      * The event ID.
      */
     PyObject *callback_ptr;
 } TimeEventHandler_t;
 
-struct TestClockAPI test_clock_new(void);
+struct TestClock_API test_clock_new(void);
 
-void test_clock_drop(struct TestClockAPI clock);
+void test_clock_drop(struct TestClock_API clock);
 
 /**
  * # Safety
  * - Assumes `callback_ptr` is a valid PyCallable pointer.
  */
-void test_clock_register_default_handler(struct TestClockAPI *clock, PyObject *callback_ptr);
+void test_clock_register_default_handler(struct TestClock_API *clock, PyObject *callback_ptr);
 
-void test_clock_set_time(struct TestClockAPI *clock, uint64_t to_time_ns);
+void test_clock_set_time(struct TestClock_API *clock, uint64_t to_time_ns);
 
-double test_clock_timestamp(struct TestClockAPI *clock);
+double test_clock_timestamp(struct TestClock_API *clock);
 
-uint64_t test_clock_timestamp_ms(struct TestClockAPI *clock);
+uint64_t test_clock_timestamp_ms(struct TestClock_API *clock);
 
-uint64_t test_clock_timestamp_us(struct TestClockAPI *clock);
+uint64_t test_clock_timestamp_us(struct TestClock_API *clock);
 
-uint64_t test_clock_timestamp_ns(struct TestClockAPI *clock);
+uint64_t test_clock_timestamp_ns(struct TestClock_API *clock);
 
-PyObject *test_clock_timer_names(const struct TestClockAPI *clock);
+PyObject *test_clock_timer_names(const struct TestClock_API *clock);
 
-uintptr_t test_clock_timer_count(struct TestClockAPI *clock);
+uintptr_t test_clock_timer_count(struct TestClock_API *clock);
 
 /**
  * # Safety
  * - Assumes `name_ptr` is a valid C string pointer.
  * - Assumes `callback_ptr` is a valid PyCallable pointer.
  */
-void test_clock_set_time_alert_ns(struct TestClockAPI *clock,
+void test_clock_set_time_alert_ns(struct TestClock_API *clock,
                                   const char *name_ptr,
                                   uint64_t alert_time_ns,
                                   PyObject *callback_ptr);
 
 /**
  * # Safety
  * - Assumes `name_ptr` is a valid C string pointer.
  * - Assumes `callback_ptr` is a valid PyCallable pointer.
  */
-void test_clock_set_timer_ns(struct TestClockAPI *clock,
+void test_clock_set_timer_ns(struct TestClock_API *clock,
                              const char *name_ptr,
                              uint64_t interval_ns,
                              uint64_t start_time_ns,
                              uint64_t stop_time_ns,
                              PyObject *callback_ptr);
 
 /**
  * # Safety
  * - Assumes `set_time` is a correct `uint8_t` of either 0 or 1.
  */
-CVec test_clock_advance_time(struct TestClockAPI *clock, uint64_t to_time_ns, uint8_t set_time);
+CVec test_clock_advance_time(struct TestClock_API *clock, uint64_t to_time_ns, uint8_t set_time);
 
 void vec_time_event_handlers_drop(CVec v);
 
 /**
  * # Safety
  * - Assumes `name_ptr` is a valid C string pointer.
  */
-uint64_t test_clock_next_time_ns(struct TestClockAPI *clock, const char *name_ptr);
+uint64_t test_clock_next_time_ns(struct TestClock_API *clock, const char *name_ptr);
 
 /**
  * # Safety
  * - Assumes `name_ptr` is a valid C string pointer.
  */
-void test_clock_cancel_timer(struct TestClockAPI *clock, const char *name_ptr);
+void test_clock_cancel_timer(struct TestClock_API *clock, const char *name_ptr);
 
-void test_clock_cancel_timers(struct TestClockAPI *clock);
+void test_clock_cancel_timers(struct TestClock_API *clock);
 
-struct LiveClockAPI live_clock_new(void);
+struct LiveClock_API live_clock_new(void);
 
-void live_clock_drop(struct LiveClockAPI clock);
+void live_clock_drop(struct LiveClock_API clock);
 
-double live_clock_timestamp(struct LiveClockAPI *clock);
+double live_clock_timestamp(struct LiveClock_API *clock);
 
-uint64_t live_clock_timestamp_ms(struct LiveClockAPI *clock);
+uint64_t live_clock_timestamp_ms(struct LiveClock_API *clock);
 
-uint64_t live_clock_timestamp_us(struct LiveClockAPI *clock);
+uint64_t live_clock_timestamp_us(struct LiveClock_API *clock);
 
-uint64_t live_clock_timestamp_ns(struct LiveClockAPI *clock);
+uint64_t live_clock_timestamp_ns(struct LiveClock_API *clock);
 
 const char *component_state_to_cstr(enum ComponentState value);
 
 /**
  * Returns an enum from a Python string.
  *
  * # Safety
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/core/includes/core.h` & `nautilus_trader-1.174.0/nautilus_trader/core/includes/core.h`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/core/includes/model.h` & `nautilus_trader-1.174.0/nautilus_trader/core/includes/model.h`

 * *Files 3% similar despite different names*

```diff
@@ -211,17 +211,15 @@
     MID_POINT = 7,
     MARK_PRICE = 8,
     INDEX_PRICE = 9,
 } TriggerType;
 
 typedef struct Arc_String Arc_String;
 
-typedef struct BTreeMap_BookPrice__Level BTreeMap_BookPrice__Level;
-
-typedef struct HashMap_u64__BookPrice HashMap_u64__BookPrice;
+typedef struct OrderBook OrderBook;
 
 typedef struct Rc_String Rc_String;
 
 typedef struct BarSpecification_t {
     uint64_t step;
     uint8_t aggregation;
     enum PriceType price_type;
@@ -264,14 +262,46 @@
     struct Price_t close;
     struct Quantity_t volume;
     uint64_t ts_event;
     uint64_t ts_init;
 } Bar_t;
 
 /**
+ * Represents an order in a book.
+ */
+typedef struct BookOrder {
+    enum OrderSide side;
+    struct Price_t price;
+    struct Quantity_t size;
+    uint64_t order_id;
+} BookOrder;
+
+/**
+ * Represents a single change/delta in an order book.
+ */
+typedef struct OrderBookDelta {
+    struct InstrumentId_t instrument_id;
+    enum BookAction action;
+    struct BookOrder order;
+    uint8_t flags;
+    uint64_t sequence;
+    uint64_t ts_event;
+    uint64_t ts_init;
+} OrderBookDelta;
+
+typedef struct OrderBookSnapshot {
+    struct InstrumentId_t instrument_id;
+    CVec bids;
+    CVec asks;
+    uint64_t sequence;
+    uint64_t ts_event;
+    uint64_t ts_init;
+} OrderBookSnapshot;
+
+/**
  * Represents a single quote tick in a financial market.
  */
 typedef struct QuoteTick_t {
     struct InstrumentId_t instrument_id;
     struct Price_t bid;
     struct Price_t ask;
     struct Quantity_t bid_size;
@@ -294,27 +324,39 @@
     enum AggressorSide aggressor_side;
     struct TradeId_t trade_id;
     uint64_t ts_event;
     uint64_t ts_init;
 } TradeTick_t;
 
 typedef enum Data_t_Tag {
-    TRADE,
+    SNAPSHOT,
+    DELTA,
     QUOTE,
+    TRADE,
+    BAR,
 } Data_t_Tag;
 
 typedef struct Data_t {
     Data_t_Tag tag;
     union {
         struct {
-            struct TradeTick_t trade;
+            struct OrderBookSnapshot snapshot;
+        };
+        struct {
+            struct OrderBookDelta delta;
         };
         struct {
             struct QuoteTick_t quote;
         };
+        struct {
+            struct TradeTick_t trade;
+        };
+        struct {
+            struct Bar_t bar;
+        };
     };
 } Data_t;
 
 typedef struct AccountId_t {
     struct Rc_String *value;
 } AccountId_t;
 
@@ -350,28 +392,17 @@
     struct Rc_String *value;
 } TraderId_t;
 
 typedef struct VenueOrderId_t {
     struct Rc_String *value;
 } VenueOrderId_t;
 
-typedef struct Ladder {
-    enum OrderSide side;
-    struct BTreeMap_BookPrice__Level *levels;
-    struct HashMap_u64__BookPrice *cache;
-} Ladder;
-
-typedef struct OrderBook {
-    struct Ladder bids;
-    struct Ladder asks;
-    struct InstrumentId_t instrument_id;
-    enum BookType book_level;
-    enum OrderSide last_side;
-    uint64_t ts_last;
-} OrderBook;
+typedef struct OrderBook_API {
+    struct OrderBook *_0;
+} OrderBook_API;
 
 typedef struct Currency_t {
     struct Arc_String *code;
     uint8_t precision;
     uint16_t iso4217;
     struct Arc_String *name;
     enum CurrencyType currency_type;
@@ -462,14 +493,65 @@
 
 void bar_drop(struct Bar_t bar);
 
 uint8_t bar_eq(const struct Bar_t *lhs, const struct Bar_t *rhs);
 
 uint64_t bar_hash(const struct Bar_t *bar);
 
+void book_order_drop(struct BookOrder order);
+
+struct BookOrder book_order_clone(const struct BookOrder *order);
+
+uint64_t book_order_hash(const struct BookOrder *order);
+
+struct BookOrder book_order_new(enum OrderSide order_side,
+                                struct Price_t price,
+                                struct Quantity_t quantity,
+                                uint64_t order_id);
+
+void orderbook_delta_drop(struct OrderBookDelta delta);
+
+struct OrderBookDelta orderbook_delta_clone(const struct OrderBookDelta *delta);
+
+struct OrderBookDelta orderbook_delta_new(struct InstrumentId_t instrument_id,
+                                          enum BookAction action,
+                                          struct BookOrder order,
+                                          uint8_t flags,
+                                          uint64_t sequence,
+                                          uint64_t ts_event,
+                                          uint64_t ts_init);
+
+void orderbook_snapshot_drop(struct OrderBookSnapshot snapshot);
+
+/**
+ * Creates a new `OrderBookSnapshot` from the provided data.
+ *
+ * # Safety
+ *
+ * This function is marked as `unsafe` because it relies on the assumption that the `CVec`
+ * objects were correctly initialized and point to valid memory regions with a valid layout.
+ * Improper use of this function with incorrect or uninitialized `CVec` objects can lead
+ * to undefined behavior, including memory unsafety and crashes.
+ *
+ * It is the responsibility of the caller to ensure that the `CVec` objects are valid and
+ * have the correct layout matching the expected `Vec` types (`BookOrder` in this case).
+ * Failure to do so can result in memory corruption or access violations.
+ *
+ * Additionally, the ownership of the provided memory is transferred to the returned
+ * `OrderBookSnapshot` object. It is crucial to ensure proper memory management and
+ * deallocation of the `OrderBookSnapshot` object to prevent memory leaks by calling
+ * `orderbook_snapshot_drop(...).
+ */
+struct OrderBookSnapshot orderbook_snapshot_new(struct InstrumentId_t instrument_id,
+                                                CVec bids,
+                                                CVec asks,
+                                                uint64_t sequence,
+                                                uint64_t ts_event,
+                                                uint64_t ts_init);
+
 void quote_tick_drop(struct QuoteTick_t tick);
 
 struct QuoteTick_t quote_tick_clone(const struct QuoteTick_t *tick);
 
 struct QuoteTick_t quote_tick_new(struct InstrumentId_t instrument_id,
                                   struct Price_t bid,
                                   struct Price_t ask,
@@ -1019,15 +1101,15 @@
 
 /**
  * Frees the memory for the given `trade_id` by dropping.
  */
 void trade_id_drop(struct TradeId_t trade_id);
 
 /**
- * Returns [TradeId] as a C string pointer.
+ * Returns [`TradeId`] as a C string pointer.
  */
 const char *trade_id_to_cstr(const struct TradeId_t *trade_id);
 
 uint8_t trade_id_eq(const struct TradeId_t *lhs, const struct TradeId_t *rhs);
 
 uint64_t trade_id_hash(const struct TradeId_t *trade_id);
 
@@ -1092,15 +1174,15 @@
 
 const char *venue_order_id_to_cstr(const struct VenueOrderId_t *venue_order_id);
 
 uint8_t venue_order_id_eq(const struct VenueOrderId_t *lhs, const struct VenueOrderId_t *rhs);
 
 uint64_t venue_order_id_hash(const struct VenueOrderId_t *venue_order_id);
 
-struct OrderBook order_book_new(struct InstrumentId_t instrument_id, enum BookType book_level);
+struct OrderBook_API order_book_new(struct InstrumentId_t instrument_id, enum BookType book_type);
 
 /**
  * Returns a [`Currency`] from pointers and primitives.
  *
  * # Safety
  * - Assumes `code_ptr` is a valid C string pointer.
  * - Assumes `name_ptr` is a valid C string pointer.
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/core/inspect.py` & `nautilus_trader-1.174.0/nautilus_trader/core/inspect.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,18 +21,15 @@
     """
     Determine whether a class is a builtin nautilus type.
     """
     if cls.__module__.startswith("nautilus_trader.model"):
         return True
     elif cls.__module__.startswith("nautilus_trader.test_kit"):
         return False
-    elif any(base.__module__.startswith("nautilus_trader.model") for base in cls.__bases__):
-        return True
-    else:
-        return False
+    return bool(any(base.__module__.startswith("nautilus_trader.model") for base in cls.__bases__))
 
 
 def get_size_of(obj) -> int:
     """
     Return the bytes size in memory of the given object.
 
     Parameters
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/core/message.pxd` & `nautilus_trader-1.174.0/nautilus_trader/core/message.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/core/message.pyx` & `nautilus_trader-1.174.0/nautilus_trader/core/message.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/core/rust/__init__.pxd` & `nautilus_trader-1.174.0/nautilus_trader/data/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/core/rust/backtest.pxd` & `nautilus_trader-1.174.0/nautilus_trader/core/rust/backtest.pxd`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Warning, this file is autogenerated by cbindgen. Don't modify this manually. */
 
 from cpython.object cimport PyObject
 from libc.stdint cimport uint8_t, uint64_t, uintptr_t
-from nautilus_trader.core.rust.common cimport TestClockAPI
+from nautilus_trader.core.rust.common cimport TestClock_API, LiveClock_API
 from nautilus_trader.core.rust.core cimport CVec, UUID4_t
 
 cdef extern from "../includes/backtest.h":
 
     # Provides a means of accumulating and draining time event handlers.
     cdef struct TimeEventAccumulator:
         pass
@@ -15,12 +15,12 @@
         TimeEventAccumulator *_0;
 
     TimeEventAccumulatorAPI time_event_accumulator_new();
 
     void time_event_accumulator_drop(TimeEventAccumulatorAPI accumulator);
 
     void time_event_accumulator_advance_clock(TimeEventAccumulatorAPI *accumulator,
-                                              TestClockAPI *clock,
+                                              TestClock_API *clock,
                                               uint64_t to_time_ns,
                                               uint8_t set_time);
 
     CVec time_event_accumulator_drain(TimeEventAccumulatorAPI *accumulator);
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/core/rust/common.pxd` & `nautilus_trader-1.174.0/nautilus_trader/core/rust/common.pxd`

 * *Files 4% similar despite different names*

```diff
@@ -63,18 +63,18 @@
 
     cdef struct Rc_String:
         pass
 
     cdef struct TestClock:
         pass
 
-    cdef struct TestClockAPI:
+    cdef struct TestClock_API:
         TestClock *_0;
 
-    cdef struct LiveClockAPI:
+    cdef struct LiveClock_API:
         LiveClock *_0;
 
     # Logger is not C FFI safe, so we box and pass it as an opaque pointer.
     # This works because Logger fields don't need to be accessed, only functions
     # are called.
     cdef struct CLogger:
         Logger_t *_0;
@@ -93,81 +93,81 @@
     # Represents a time event and its associated handler.
     cdef struct TimeEventHandler_t:
         # The event.
         TimeEvent_t event;
         # The event ID.
         PyObject *callback_ptr;
 
-    TestClockAPI test_clock_new();
+    TestClock_API test_clock_new();
 
-    void test_clock_drop(TestClockAPI clock);
+    void test_clock_drop(TestClock_API clock);
 
     # # Safety
     # - Assumes `callback_ptr` is a valid PyCallable pointer.
-    void test_clock_register_default_handler(TestClockAPI *clock, PyObject *callback_ptr);
+    void test_clock_register_default_handler(TestClock_API *clock, PyObject *callback_ptr);
 
-    void test_clock_set_time(TestClockAPI *clock, uint64_t to_time_ns);
+    void test_clock_set_time(TestClock_API *clock, uint64_t to_time_ns);
 
-    double test_clock_timestamp(TestClockAPI *clock);
+    double test_clock_timestamp(TestClock_API *clock);
 
-    uint64_t test_clock_timestamp_ms(TestClockAPI *clock);
+    uint64_t test_clock_timestamp_ms(TestClock_API *clock);
 
-    uint64_t test_clock_timestamp_us(TestClockAPI *clock);
+    uint64_t test_clock_timestamp_us(TestClock_API *clock);
 
-    uint64_t test_clock_timestamp_ns(TestClockAPI *clock);
+    uint64_t test_clock_timestamp_ns(TestClock_API *clock);
 
-    PyObject *test_clock_timer_names(const TestClockAPI *clock);
+    PyObject *test_clock_timer_names(const TestClock_API *clock);
 
-    uintptr_t test_clock_timer_count(TestClockAPI *clock);
+    uintptr_t test_clock_timer_count(TestClock_API *clock);
 
     # # Safety
     # - Assumes `name_ptr` is a valid C string pointer.
     # - Assumes `callback_ptr` is a valid PyCallable pointer.
-    void test_clock_set_time_alert_ns(TestClockAPI *clock,
+    void test_clock_set_time_alert_ns(TestClock_API *clock,
                                       const char *name_ptr,
                                       uint64_t alert_time_ns,
                                       PyObject *callback_ptr);
 
     # # Safety
     # - Assumes `name_ptr` is a valid C string pointer.
     # - Assumes `callback_ptr` is a valid PyCallable pointer.
-    void test_clock_set_timer_ns(TestClockAPI *clock,
+    void test_clock_set_timer_ns(TestClock_API *clock,
                                  const char *name_ptr,
                                  uint64_t interval_ns,
                                  uint64_t start_time_ns,
                                  uint64_t stop_time_ns,
                                  PyObject *callback_ptr);
 
     # # Safety
     # - Assumes `set_time` is a correct `uint8_t` of either 0 or 1.
-    CVec test_clock_advance_time(TestClockAPI *clock, uint64_t to_time_ns, uint8_t set_time);
+    CVec test_clock_advance_time(TestClock_API *clock, uint64_t to_time_ns, uint8_t set_time);
 
     void vec_time_event_handlers_drop(CVec v);
 
     # # Safety
     # - Assumes `name_ptr` is a valid C string pointer.
-    uint64_t test_clock_next_time_ns(TestClockAPI *clock, const char *name_ptr);
+    uint64_t test_clock_next_time_ns(TestClock_API *clock, const char *name_ptr);
 
     # # Safety
     # - Assumes `name_ptr` is a valid C string pointer.
-    void test_clock_cancel_timer(TestClockAPI *clock, const char *name_ptr);
+    void test_clock_cancel_timer(TestClock_API *clock, const char *name_ptr);
 
-    void test_clock_cancel_timers(TestClockAPI *clock);
+    void test_clock_cancel_timers(TestClock_API *clock);
 
-    LiveClockAPI live_clock_new();
+    LiveClock_API live_clock_new();
 
-    void live_clock_drop(LiveClockAPI clock);
+    void live_clock_drop(LiveClock_API clock);
 
-    double live_clock_timestamp(LiveClockAPI *clock);
+    double live_clock_timestamp(LiveClock_API *clock);
 
-    uint64_t live_clock_timestamp_ms(LiveClockAPI *clock);
+    uint64_t live_clock_timestamp_ms(LiveClock_API *clock);
 
-    uint64_t live_clock_timestamp_us(LiveClockAPI *clock);
+    uint64_t live_clock_timestamp_us(LiveClock_API *clock);
 
-    uint64_t live_clock_timestamp_ns(LiveClockAPI *clock);
+    uint64_t live_clock_timestamp_ns(LiveClock_API *clock);
 
     const char *component_state_to_cstr(ComponentState value);
 
     # Returns an enum from a Python string.
     #
     # # Safety
     # - Assumes `ptr` is a valid C string pointer.
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/core/rust/common.pyx` & `nautilus_trader-1.174.0/nautilus_trader/core/rust/common.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/core/rust/core.pxd` & `nautilus_trader-1.174.0/nautilus_trader/core/rust/core.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/core/rust/model.pxd` & `nautilus_trader-1.174.0/nautilus_trader/core/rust/model.pxd`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Warning, this file is autogenerated by cbindgen. Don't modify this manually. */
 
 from libc.stdint cimport uint8_t, uint16_t, uint64_t, int64_t
+from nautilus_trader.core.rust.core cimport CVec, UUID4_t
 
 cdef extern from "../includes/model.h":
 
     const uint8_t FIXED_PRECISION # = 9
 
     const double FIXED_SCALAR # = 1000000000.0
 
@@ -181,18 +182,15 @@
         MID_POINT # = 7,
         MARK_PRICE # = 8,
         INDEX_PRICE # = 9,
 
     cdef struct Arc_String:
         pass
 
-    cdef struct BTreeMap_BookPrice__Level:
-        pass
-
-    cdef struct HashMap_u64__BookPrice:
+    cdef struct OrderBook:
         pass
 
     cdef struct Rc_String:
         pass
 
     cdef struct BarSpecification_t:
         uint64_t step;
@@ -228,14 +226,39 @@
         Price_t high;
         Price_t low;
         Price_t close;
         Quantity_t volume;
         uint64_t ts_event;
         uint64_t ts_init;
 
+    # Represents an order in a book.
+    cdef struct BookOrder:
+        OrderSide side;
+        Price_t price;
+        Quantity_t size;
+        uint64_t order_id;
+
+    # Represents a single change/delta in an order book.
+    cdef struct OrderBookDelta:
+        InstrumentId_t instrument_id;
+        BookAction action;
+        BookOrder order;
+        uint8_t flags;
+        uint64_t sequence;
+        uint64_t ts_event;
+        uint64_t ts_init;
+
+    cdef struct OrderBookSnapshot:
+        InstrumentId_t instrument_id;
+        CVec bids;
+        CVec asks;
+        uint64_t sequence;
+        uint64_t ts_event;
+        uint64_t ts_init;
+
     # Represents a single quote tick in a financial market.
     cdef struct QuoteTick_t:
         InstrumentId_t instrument_id;
         Price_t bid;
         Price_t ask;
         Quantity_t bid_size;
         Quantity_t ask_size;
@@ -252,21 +275,27 @@
         Quantity_t size;
         AggressorSide aggressor_side;
         TradeId_t trade_id;
         uint64_t ts_event;
         uint64_t ts_init;
 
     cpdef enum Data_t_Tag:
-        TRADE,
+        SNAPSHOT,
+        DELTA,
         QUOTE,
+        TRADE,
+        BAR,
 
     cdef struct Data_t:
         Data_t_Tag tag;
-        TradeTick_t trade;
+        OrderBookSnapshot snapshot;
+        OrderBookDelta delta;
         QuoteTick_t quote;
+        TradeTick_t trade;
+        Bar_t bar;
 
     cdef struct AccountId_t:
         Rc_String *value;
 
     cdef struct ClientId_t:
         Rc_String *value;
 
@@ -290,26 +319,16 @@
 
     cdef struct TraderId_t:
         Rc_String *value;
 
     cdef struct VenueOrderId_t:
         Rc_String *value;
 
-    cdef struct Ladder:
-        OrderSide side;
-        BTreeMap_BookPrice__Level *levels;
-        HashMap_u64__BookPrice *cache;
-
-    cdef struct OrderBook:
-        Ladder bids;
-        Ladder asks;
-        InstrumentId_t instrument_id;
-        BookType book_level;
-        OrderSide last_side;
-        uint64_t ts_last;
+    cdef struct OrderBook_API:
+        OrderBook *_0;
 
     cdef struct Currency_t:
         Arc_String *code;
         uint8_t precision;
         uint16_t iso4217;
         Arc_String *name;
         CurrencyType currency_type;
@@ -387,14 +406,63 @@
 
     void bar_drop(Bar_t bar);
 
     uint8_t bar_eq(const Bar_t *lhs, const Bar_t *rhs);
 
     uint64_t bar_hash(const Bar_t *bar);
 
+    void book_order_drop(BookOrder order);
+
+    BookOrder book_order_clone(const BookOrder *order);
+
+    uint64_t book_order_hash(const BookOrder *order);
+
+    BookOrder book_order_new(OrderSide order_side,
+                             Price_t price,
+                             Quantity_t quantity,
+                             uint64_t order_id);
+
+    void orderbook_delta_drop(OrderBookDelta delta);
+
+    OrderBookDelta orderbook_delta_clone(const OrderBookDelta *delta);
+
+    OrderBookDelta orderbook_delta_new(InstrumentId_t instrument_id,
+                                       BookAction action,
+                                       BookOrder order,
+                                       uint8_t flags,
+                                       uint64_t sequence,
+                                       uint64_t ts_event,
+                                       uint64_t ts_init);
+
+    void orderbook_snapshot_drop(OrderBookSnapshot snapshot);
+
+    # Creates a new `OrderBookSnapshot` from the provided data.
+    #
+    # # Safety
+    #
+    # This function is marked as `unsafe` because it relies on the assumption that the `CVec`
+    # objects were correctly initialized and point to valid memory regions with a valid layout.
+    # Improper use of this function with incorrect or uninitialized `CVec` objects can lead
+    # to undefined behavior, including memory unsafety and crashes.
+    #
+    # It is the responsibility of the caller to ensure that the `CVec` objects are valid and
+    # have the correct layout matching the expected `Vec` types (`BookOrder` in this case).
+    # Failure to do so can result in memory corruption or access violations.
+    #
+    # Additionally, the ownership of the provided memory is transferred to the returned
+    # `OrderBookSnapshot` object. It is crucial to ensure proper memory management and
+    # deallocation of the `OrderBookSnapshot` object to prevent memory leaks by calling
+    # `orderbook_snapshot_drop(...).
+    OrderBookSnapshot orderbook_snapshot_new(InstrumentId_t instrument_id,
+                                             CVec bids,
+                                             CVec asks,
+                                             uint64_t sequence,
+                                             uint64_t ts_event,
+                                             uint64_t ts_init);
+
     void quote_tick_drop(QuoteTick_t tick);
 
     QuoteTick_t quote_tick_clone(const QuoteTick_t *tick);
 
     QuoteTick_t quote_tick_new(InstrumentId_t instrument_id,
                                Price_t bid,
                                Price_t ask,
@@ -824,15 +892,15 @@
     TradeId_t trade_id_new(const char *ptr);
 
     TradeId_t trade_id_clone(const TradeId_t *trade_id);
 
     # Frees the memory for the given `trade_id` by dropping.
     void trade_id_drop(TradeId_t trade_id);
 
-    # Returns [TradeId] as a C string pointer.
+    # Returns [`TradeId`] as a C string pointer.
     const char *trade_id_to_cstr(const TradeId_t *trade_id);
 
     uint8_t trade_id_eq(const TradeId_t *lhs, const TradeId_t *rhs);
 
     uint64_t trade_id_hash(const TradeId_t *trade_id);
 
     # Returns a Nautilus identifier from a C string pointer.
@@ -880,15 +948,15 @@
 
     const char *venue_order_id_to_cstr(const VenueOrderId_t *venue_order_id);
 
     uint8_t venue_order_id_eq(const VenueOrderId_t *lhs, const VenueOrderId_t *rhs);
 
     uint64_t venue_order_id_hash(const VenueOrderId_t *venue_order_id);
 
-    OrderBook order_book_new(InstrumentId_t instrument_id, BookType book_level);
+    OrderBook_API order_book_new(InstrumentId_t instrument_id, BookType book_type);
 
     # Returns a [`Currency`] from pointers and primitives.
     #
     # # Safety
     # - Assumes `code_ptr` is a valid C string pointer.
     # - Assumes `name_ptr` is a valid C string pointer.
     Currency_t currency_from_py(const char *code_ptr,
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/core/rust/model.pyx` & `nautilus_trader-1.174.0/nautilus_trader/core/rust/model.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/core/stats.pxd` & `nautilus_trader-1.174.0/nautilus_trader/core/stats.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/core/stats.pyx` & `nautilus_trader-1.174.0/nautilus_trader/core/stats.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/core/string.pxd` & `nautilus_trader-1.174.0/nautilus_trader/core/string.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/core/uuid.pxd` & `nautilus_trader-1.174.0/nautilus_trader/core/uuid.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/core/uuid.pyx` & `nautilus_trader-1.174.0/nautilus_trader/core/uuid.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/data/__init__.pxd` & `nautilus_trader-1.174.0/nautilus_trader/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/data/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/data/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/data/aggregation.pxd` & `nautilus_trader-1.174.0/nautilus_trader/data/aggregation.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/data/aggregation.pyx` & `nautilus_trader-1.174.0/nautilus_trader/data/aggregation.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/data/client.pxd` & `nautilus_trader-1.174.0/nautilus_trader/data/client.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/data/client.pyx` & `nautilus_trader-1.174.0/nautilus_trader/data/client.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/data/engine.pxd` & `nautilus_trader-1.174.0/nautilus_trader/data/engine.pxd`

 * *Files 1% similar despite different names*

```diff
@@ -24,24 +24,24 @@
 from nautilus_trader.data.messages cimport DataResponse
 from nautilus_trader.data.messages cimport Subscribe
 from nautilus_trader.data.messages cimport Unsubscribe
 from nautilus_trader.model.data.bar cimport Bar
 from nautilus_trader.model.data.bar cimport BarType
 from nautilus_trader.model.data.base cimport DataType
 from nautilus_trader.model.data.base cimport GenericData
+from nautilus_trader.model.data.book cimport OrderBookDelta
 from nautilus_trader.model.data.tick cimport QuoteTick
 from nautilus_trader.model.data.tick cimport TradeTick
 from nautilus_trader.model.data.ticker cimport Ticker
 from nautilus_trader.model.data.venue cimport InstrumentClose
 from nautilus_trader.model.data.venue cimport InstrumentStatusUpdate
 from nautilus_trader.model.data.venue cimport VenueStatusUpdate
 from nautilus_trader.model.identifiers cimport InstrumentId
 from nautilus_trader.model.identifiers cimport Venue
 from nautilus_trader.model.instruments.base cimport Instrument
-from nautilus_trader.model.orderbook.data cimport OrderBookData
 
 
 cdef class DataEngine(Component):
     cdef readonly Cache _cache
     cdef readonly DataClient _default_client
     cdef readonly object _catalog
     cdef readonly bint _use_rust
@@ -104,14 +104,15 @@
 
     cpdef void _execute_command(self, DataCommand command)
     cpdef void _handle_subscribe(self, DataClient client, Subscribe command)
     cpdef void _handle_unsubscribe(self, DataClient client, Unsubscribe command)
     cpdef void _handle_subscribe_instrument(self, MarketDataClient client, InstrumentId instrument_id)
     cpdef void _handle_subscribe_order_book_deltas(self, MarketDataClient client, InstrumentId instrument_id, dict metadata)  # noqa
     cpdef void _handle_subscribe_order_book_snapshots(self, MarketDataClient client, InstrumentId instrument_id, dict metadata)  # noqa
+    cpdef void _setup_order_book(self, MarketDataClient client, InstrumentId instrument_id, dict metadata, bint only_deltas)  # noqa
     cpdef void _handle_subscribe_ticker(self, MarketDataClient client, InstrumentId instrument_id)
     cpdef void _handle_subscribe_quote_ticks(self, MarketDataClient client, InstrumentId instrument_id)
     cpdef void _handle_subscribe_trade_ticks(self, MarketDataClient client, InstrumentId instrument_id)
     cpdef void _handle_subscribe_bars(self, MarketDataClient client, BarType bar_type)
     cpdef void _handle_subscribe_data(self, DataClient client, DataType data_type)
     cpdef void _handle_subscribe_venue_status_updates(self, MarketDataClient client, Venue venue)
     cpdef void _handle_subscribe_instrument_status_updates(self, MarketDataClient client, InstrumentId instrument_id)
@@ -127,15 +128,15 @@
     cpdef void _handle_request(self, DataRequest request)
     cpdef void _query_data_catalog(self, DataRequest request)
 
 # -- DATA HANDLERS --------------------------------------------------------------------------------
 
     cpdef void _handle_data(self, Data data)
     cpdef void _handle_instrument(self, Instrument instrument)
-    cpdef void _handle_order_book_data(self, OrderBookData data)
+    cpdef void _handle_order_book_data(self, Data data)
     cpdef void _handle_ticker(self, Ticker ticker)
     cpdef void _handle_quote_tick(self, QuoteTick tick)
     cpdef void _handle_trade_tick(self, TradeTick tick)
     cpdef void _handle_bar(self, Bar bar)
     cpdef void _handle_generic_data(self, GenericData data)
     cpdef void _handle_venue_status_update(self, VenueStatusUpdate data)
     cpdef void _handle_instrument_status_update(self, InstrumentStatusUpdate data)
@@ -148,11 +149,11 @@
     cpdef void _handle_quote_ticks(self, list ticks)
     cpdef void _handle_trade_ticks(self, list ticks)
     cpdef void _handle_bars(self, list bars, Bar partial)
 
 # -- INTERNAL -------------------------------------------------------------------------------------
 
     cpdef void _internal_update_instruments(self, list instruments)
-    cpdef void _maintain_order_book(self, OrderBookData data)
+    cpdef void _update_order_book(self, Data data)
     cpdef void _snapshot_order_book(self, TimeEvent snap_event)
     cpdef void _start_bar_aggregator(self, MarketDataClient client, BarType bar_type)
     cpdef void _stop_bar_aggregator(self, MarketDataClient client, BarType bar_type)
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/data/engine.pyx` & `nautilus_trader-1.174.0/nautilus_trader/data/engine.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -63,28 +63,30 @@
 from nautilus_trader.data.messages cimport DataRequest
 from nautilus_trader.data.messages cimport DataResponse
 from nautilus_trader.data.messages cimport Subscribe
 from nautilus_trader.data.messages cimport Unsubscribe
 from nautilus_trader.model.data.bar cimport Bar
 from nautilus_trader.model.data.bar cimport BarType
 from nautilus_trader.model.data.base cimport DataType
+from nautilus_trader.model.data.book cimport ORDER_BOOK_DATA
+from nautilus_trader.model.data.book cimport OrderBookDelta
+from nautilus_trader.model.data.book cimport OrderBookDeltas
+from nautilus_trader.model.data.book cimport OrderBookSnapshot
 from nautilus_trader.model.data.tick cimport QuoteTick
 from nautilus_trader.model.data.tick cimport TradeTick
 from nautilus_trader.model.data.venue cimport InstrumentClose
 from nautilus_trader.model.data.venue cimport InstrumentStatusUpdate
 from nautilus_trader.model.data.venue cimport VenueStatusUpdate
 from nautilus_trader.model.enums_c cimport BarAggregation
 from nautilus_trader.model.enums_c cimport PriceType
 from nautilus_trader.model.identifiers cimport ClientId
 from nautilus_trader.model.identifiers cimport ComponentId
 from nautilus_trader.model.identifiers cimport InstrumentId
 from nautilus_trader.model.instruments.base cimport Instrument
 from nautilus_trader.model.orderbook.book cimport OrderBook
-from nautilus_trader.model.orderbook.data cimport OrderBookData
-from nautilus_trader.model.orderbook.data cimport OrderBookSnapshot
 from nautilus_trader.msgbus.bus cimport MessageBus
 
 
 cdef class DataEngine(Component):
     """
     Provides a high-performance data engine for managing many `DataClient`
     instances, for the asynchronous ingest of data.
@@ -605,15 +607,15 @@
             )
         elif command.data_type.type == OrderBookSnapshot:
             self._handle_subscribe_order_book_snapshots(
                 client,
                 command.data_type.metadata.get("instrument_id"),
                 command.data_type.metadata,
             )
-        elif command.data_type.type == OrderBookData:
+        elif command.data_type.type == OrderBookDelta:
             self._handle_subscribe_order_book_deltas(
                 client,
                 command.data_type.metadata.get("instrument_id"),
                 command.data_type.metadata,
             )
         elif command.data_type.type == Ticker:
             self._handle_subscribe_ticker(
@@ -661,15 +663,15 @@
             )
         elif command.data_type.type == OrderBookSnapshot:
             self._handle_unsubscribe_order_book_snapshots(
                 client,
                 command.data_type.metadata.get("instrument_id"),
                 command.data_type.metadata,
             )
-        elif command.data_type.type == OrderBookData:
+        elif command.data_type.type == OrderBookDelta:
             self._handle_unsubscribe_order_book_deltas(
                 client,
                 command.data_type.metadata.get("instrument_id"),
                 command.data_type.metadata,
             )
         elif command.data_type.type == Ticker:
             self._handle_unsubscribe_ticker(
@@ -714,51 +716,19 @@
         InstrumentId instrument_id,
         dict metadata,
     ):
         Condition.not_none(client, "client")
         Condition.not_none(instrument_id, "instrument_id")
         Condition.not_none(metadata, "metadata")
 
-        # Create order book
-        if not self._cache.has_order_book(instrument_id):
-            instrument = self._cache.instrument(instrument_id)
-            if instrument is None:
-                self._log.error(
-                    f"Cannot subscribe to {instrument_id} <OrderBook> data: "
-                    f"no instrument found in the cache.",
-                )
-                return
-            order_book = OrderBook.create(
-                instrument=instrument,
-                book_type=metadata["book_type"],
-            )
-
-            self._cache.add_order_book(order_book)
-            self._log.debug(f"Created {type(order_book).__name__}.")
-
-        # Always re-subscribe to override previous settings
-        client.subscribe_order_book_deltas(
-            instrument_id=instrument_id,
-            book_type=metadata["book_type"],
-            depth=metadata["depth"],
-            kwargs=metadata.get("kwargs"),
-        )
-
-        cdef str topic = f"data.book.deltas.{instrument_id.venue}.{instrument_id.symbol}"
-
-        if self._msgbus.is_subscribed(
-            topic=topic,
-            handler=self._maintain_order_book,
-        ):
-            return  # Already subscribed
-
-        self._msgbus.subscribe(
-            topic=topic,
-            handler=self._maintain_order_book,
-            priority=10,
+        self._setup_order_book(
+            client,
+            instrument_id,
+            metadata,
+            only_deltas=True,
         )
 
     cpdef void _handle_subscribe_order_book_snapshots(
         self,
         MarketDataClient client,
         InstrumentId instrument_id,
         dict metadata,
@@ -779,14 +749,32 @@
                 interval=timedelta(milliseconds=interval_ms),
                 start_time=start_time,
                 stop_time=None,
                 callback=self._snapshot_order_book,
             )
             self._log.debug(f"Set timer {timer_name}.")
 
+        self._setup_order_book(
+            client,
+            instrument_id,
+            metadata,
+            only_deltas=False,
+        )
+
+    cpdef void _setup_order_book(
+        self,
+        MarketDataClient client,
+        InstrumentId instrument_id,
+        dict metadata,
+        bint only_deltas,
+    ):
+        Condition.not_none(client, "client")
+        Condition.not_none(instrument_id, "instrument_id")
+        Condition.not_none(metadata, "metadata")
+
         # Create order book
         if not self._cache.has_order_book(instrument_id):
             instrument = self._cache.instrument(instrument_id)
             if instrument is None:
                 self._log.error(
                     f"Cannot subscribe to {instrument_id} <OrderBook> data: "
                     f"no instrument found in the cache.",
@@ -805,38 +793,37 @@
             if instrument_id not in client.subscribed_order_book_deltas():
                 client.subscribe_order_book_deltas(
                     instrument_id=instrument_id,
                     book_type=metadata["book_type"],
                     depth=metadata["depth"],
                     kwargs=metadata.get("kwargs"),
                 )
-        except NotImplementedError:
+        except NotImplementedError as ex:
+            if only_deltas:
+                raise
             if instrument_id not in client.subscribed_order_book_snapshots():
                 client.subscribe_order_book_snapshots(
                     instrument_id=instrument_id,
                     book_type=metadata["book_type"],
                     depth=metadata["depth"],
                     kwargs=metadata.get("kwargs"),
                 )
 
+        # Setup subscriptions
         cdef str topic = f"data.book.deltas.{instrument_id.venue}.{instrument_id.symbol}"
 
-        if self._msgbus.is_subscribed(
+        if not self._msgbus.is_subscribed(
             topic=topic,
-            handler=self._maintain_order_book,
+            handler=self._update_order_book,
         ):
-            return  # Already subscribed
-
-        self._msgbus.subscribe(
-            topic=f"data.book.deltas"
-                  f".{instrument_id.venue}"
-                  f".{instrument_id.symbol}",
-            handler=self._maintain_order_book,
-            priority=10,
-        )
+            self._msgbus.subscribe(
+                topic=topic,
+                handler=self._update_order_book,
+                priority=10,
+            )
 
     cpdef void _handle_subscribe_ticker(
         self,
         MarketDataClient client,
         InstrumentId instrument_id,
     ):
         Condition.not_none(client, "client")
@@ -1229,15 +1216,15 @@
         self._handle_response(response)
 
 # -- DATA HANDLERS --------------------------------------------------------------------------------
 
     cpdef void _handle_data(self, Data data):
         self.data_count += 1
 
-        if isinstance(data, OrderBookData):
+        if isinstance(data, ORDER_BOOK_DATA):
             self._handle_order_book_data(data)
         elif isinstance(data, Ticker):
             self._handle_ticker(data)
         elif isinstance(data, QuoteTick):
             self._handle_quote_tick(data)
         elif isinstance(data, TradeTick):
             self._handle_trade_tick(data)
@@ -1261,15 +1248,15 @@
         self._msgbus.publish_c(
             topic=f"data.instrument"
                   f".{instrument.id.venue}"
                   f".{instrument.id.symbol}",
             msg=instrument,
         )
 
-    cpdef void _handle_order_book_data(self, OrderBookData data):
+    cpdef void _handle_order_book_data(self, Data data):
         self._msgbus.publish_c(
             topic=f"data.book.deltas"
                   f".{data.instrument_id.venue}"
                   f".{data.instrument_id.symbol}",
             msg=data,
         )
 
@@ -1405,19 +1392,19 @@
     # Python wrapper to enable callbacks
     cpdef void _internal_update_instruments(self, list instruments: [Instrument]):
         # Handle all instruments individually
         cdef Instrument instrument
         for instrument in instruments:
             self._handle_instrument(instrument)
 
-    cpdef void _maintain_order_book(self, OrderBookData data):
+    cpdef void _update_order_book(self, Data data):
         cdef OrderBook order_book = self._cache.order_book(data.instrument_id)
         if order_book is None:
             self._log.error(
-                f"Cannot maintain order book: "
+                "Cannot update order book: "
                 f"no book found for {data.instrument_id}.",
             )
             return
 
         order_book.apply(data)
 
     cpdef void _snapshot_order_book(self, TimeEvent snap_event):
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/data/messages.pxd` & `nautilus_trader-1.174.0/nautilus_trader/data/messages.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/data/messages.pyx` & `nautilus_trader-1.174.0/nautilus_trader/data/messages.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/examples/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/examples/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/examples/algorithms/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/examples/strategies/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/examples/algorithms/blank.py` & `nautilus_trader-1.174.0/nautilus_trader/examples/algorithms/blank.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/examples/algorithms/twap.py` & `nautilus_trader-1.174.0/nautilus_trader/examples/algorithms/twap.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,15 +156,15 @@
             return
 
         # Validate execution parameters
         exec_params = order.exec_algorithm_params
         if not exec_params:
             self.log.error(
                 f"Cannot execute order: "
-                f"`exec_algorithm_params` not found for primary order {repr(order)}.",
+                f"`exec_algorithm_params` not found for primary order {order!r}.",
             )
             return
 
         horizon_secs = exec_params.get("horizon_secs")
         if not horizon_secs:
             self.log.error(
                 f"Cannot execute order: "
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/examples/strategies/__init__.pxd` & `nautilus_trader-1.174.0/nautilus_trader/examples/strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/examples/strategies/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/execution/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/examples/strategies/blank.py` & `nautilus_trader-1.174.0/nautilus_trader/examples/strategies/blank.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,32 +57,32 @@
         super().__init__(config)
 
         # Configuration
         self.instrument_id = InstrumentId.from_str(config.instrument_id)
 
     def on_start(self) -> None:
         """Actions to be performed when the strategy is started."""
-        pass  # Optionally implement
+        # Optionally implement
 
     def on_stop(self) -> None:
         """Actions to be performed when the strategy is stopped."""
-        pass  # Optionally implement
+        # Optionally implement
 
     def on_reset(self) -> None:
         """Actions to be performed when the strategy is reset."""
-        pass  # Optionally implement
+        # Optionally implement
 
     def on_dispose(self) -> None:
         """
         Actions to be performed when the strategy is disposed.
 
         Cleanup any resources used by the strategy here.
 
         """
-        pass  # Optionally implement
+        # Optionally implement
 
     def on_save(self) -> dict[str, bytes]:
         """
         Actions to be performed when the strategy is saved.
 
         Create and return a state dictionary of values to be saved.
 
@@ -102,93 +102,93 @@
 
         Parameters
         ----------
         state : dict[str, bytes]
             The strategy state dictionary.
 
         """
-        pass  # Optionally implement
+        # Optionally implement
 
     def on_instrument(self, instrument: Instrument) -> None:
         """
         Actions to be performed when the strategy is running and receives an
         instrument.
 
         Parameters
         ----------
         instrument : Instrument
             The instrument received.
 
         """
-        pass  # Optionally implement
+        # Optionally implement
 
     def on_quote_tick(self, tick: QuoteTick) -> None:
         """
         Actions to be performed when the strategy is running and receives a quote tick.
 
         Parameters
         ----------
         tick : QuoteTick
             The tick received.
 
         """
-        pass  # Optionally implement
+        # Optionally implement
 
     def on_trade_tick(self, tick: TradeTick) -> None:
         """
         Actions to be performed when the strategy is running and receives a trade tick.
 
         Parameters
         ----------
         tick : TradeTick
             The tick received.
 
         """
-        pass  # Optionally implement
+        # Optionally implement
 
     def on_bar(self, bar: Bar) -> None:
         """
         Actions to be performed when the strategy is running and receives a bar.
 
         Parameters
         ----------
         bar : Bar
             The bar received.
 
         """
-        pass  # Optionally implement
+        # Optionally implement
 
     def buy(self) -> None:
         """
         Users simple buy method (example).
         """
-        pass  # Optionally implement
+        # Optionally implement
 
     def sell(self) -> None:
         """
         Users simple sell method (example).
         """
-        pass  # Optionally implement
+        # Optionally implement
 
     def on_data(self, data: Data) -> None:
         """
         Actions to be performed when the strategy is running and receives generic data.
 
         Parameters
         ----------
         data : Data
             The data received.
 
         """
-        pass  # Optionally implement
+        # Optionally implement
 
     def on_event(self, event: Event) -> None:
         """
         Actions to be performed when the strategy is running and receives an event.
 
         Parameters
         ----------
         event : Event
             The event received.
 
         """
-        pass  # Optionally implement
+        # Optionally implement
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/examples/strategies/ema_cross.py` & `nautilus_trader-1.174.0/nautilus_trader/examples/strategies/ema_cross.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,31 +10,34 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 # -------------------------------------------------------------------------------------------------
 
 from decimal import Decimal
+from typing import Union
 
 from nautilus_trader.common.enums import LogColor
 from nautilus_trader.config import StrategyConfig
 from nautilus_trader.core.correctness import PyCondition
 from nautilus_trader.core.data import Data
 from nautilus_trader.core.message import Event
 from nautilus_trader.indicators.average.ema import ExponentialMovingAverage
 from nautilus_trader.model.data.bar import Bar
 from nautilus_trader.model.data.bar import BarType
+from nautilus_trader.model.data.book import OrderBookDelta
+from nautilus_trader.model.data.book import OrderBookDeltas
+from nautilus_trader.model.data.book import OrderBookSnapshot
 from nautilus_trader.model.data.tick import QuoteTick
 from nautilus_trader.model.data.tick import TradeTick
 from nautilus_trader.model.data.ticker import Ticker
 from nautilus_trader.model.enums import OrderSide
 from nautilus_trader.model.identifiers import InstrumentId
 from nautilus_trader.model.instruments import Instrument
 from nautilus_trader.model.orderbook import OrderBook
-from nautilus_trader.model.orderbook import OrderBookData
 from nautilus_trader.model.orders import MarketOrder
 from nautilus_trader.trading.strategy import Strategy
 
 
 # *** THIS IS A TEST STRATEGY WITH NO ALPHA ADVANTAGE WHATSOEVER. ***
 # *** IT IS NOT INTENDED TO BE USED TO TRADE LIVE WITH REAL MONEY. ***
 
@@ -146,85 +149,82 @@
         ----------
         instrument : Instrument
             The instrument received.
 
         """
         # For debugging (must add a subscription)
         # self.log.info(repr(instrument), LogColor.CYAN)
-        pass
 
-    def on_order_book_delta(self, data: OrderBookData) -> None:
+    def on_order_book_delta(
+        self,
+        data: Union[OrderBookDelta, OrderBookDeltas, OrderBookSnapshot],
+    ) -> None:
         """
         Actions to be performed when the strategy is running and receives order data.
 
         Parameters
         ----------
-        data : OrderBookData
+        data : OrderBookDelta, OrderBookDeltas, OrderBookSnapshot
             The order book data received.
 
         """
         # For debugging (must add a subscription)
         # self.log.info(repr(data), LogColor.CYAN)
-        pass
 
     def on_order_book(self, order_book: OrderBook) -> None:
         """
         Actions to be performed when the strategy is running and receives an order book.
 
         Parameters
         ----------
         order_book : OrderBook
             The order book received.
 
         """
         # For debugging (must add a subscription)
         # self.log.info(repr(order_book), LogColor.CYAN)
-        pass
 
     def on_ticker(self, ticker: Ticker) -> None:
         """
         Actions to be performed when the strategy is running and receives a ticker.
 
         Parameters
         ----------
         ticker : Ticker
             The ticker received.
 
         """
         # For debugging (must add a subscription)
         # self.log.info(repr(ticker), LogColor.CYAN)
-        pass
 
     def on_quote_tick(self, tick: QuoteTick) -> None:
         """
         Actions to be performed when the strategy is running and receives a quote tick.
 
         Parameters
         ----------
         tick : QuoteTick
             The tick received.
 
         """
         # For debugging (must add a subscription)
         # self.log.info(repr(tick), LogColor.CYAN)
-        pass
 
     def on_trade_tick(self, tick: TradeTick) -> None:
         """
         Actions to be performed when the strategy is running and receives a trade tick.
 
         Parameters
         ----------
         tick : TradeTick
             The tick received.
 
         """
         # For debugging (must add a subscription)
         # self.log.info(repr(tick), LogColor.CYAN)
-        pass
 
     def on_bar(self, bar: Bar) -> None:
         """
         Actions to be performed when the strategy is running and receives a bar.
 
         Parameters
         ----------
@@ -293,27 +293,25 @@
 
         Parameters
         ----------
         data : Data
             The data received.
 
         """
-        pass
 
     def on_event(self, event: Event) -> None:
         """
         Actions to be performed when the strategy is running and receives an event.
 
         Parameters
         ----------
         event : Event
             The event received.
 
         """
-        pass
 
     def on_stop(self) -> None:
         """
         Actions to be performed when the strategy is stopped.
         """
         self.cancel_all_orders(self.instrument_id)
         if self.close_positions_on_stop:
@@ -357,17 +355,15 @@
 
         Parameters
         ----------
         state : dict[str, bytes]
             The strategy state dictionary.
 
         """
-        pass
 
     def on_dispose(self) -> None:
         """
         Actions to be performed when the strategy is disposed.
 
         Cleanup any resources used by the strategy here.
 
         """
-        pass
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/examples/strategies/ema_cross_bracket.py` & `nautilus_trader-1.174.0/nautilus_trader/examples/strategies/ema_cross_bracket.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,14 @@
         ----------
         tick : QuoteTick
             The tick received.
 
         """
         # For debugging (must add a subscription)
         # self.log.info(repr(tick), LogColor.CYAN)
-        pass
 
     def on_bar(self, bar: Bar) -> None:
         """
         Actions to be performed when the strategy is running and receives a bar.
 
         Parameters
         ----------
@@ -259,27 +258,25 @@
 
         Parameters
         ----------
         data : Data
             The data received.
 
         """
-        pass
 
     def on_event(self, event: Event) -> None:
         """
         Actions to be performed when the strategy is running and receives an event.
 
         Parameters
         ----------
         event : Event
             The event received.
 
         """
-        pass
 
     def on_stop(self) -> None:
         """
         Actions to be performed when the strategy is stopped.
         """
         self.cancel_all_orders(self.instrument_id)
         self.close_all_positions(self.instrument_id)
@@ -318,17 +315,15 @@
 
         Parameters
         ----------
         state : dict[str, bytes]
             The strategy state dictionary.
 
         """
-        pass
 
     def on_dispose(self) -> None:
         """
         Actions to be performed when the strategy is disposed.
 
         Cleanup any resources used by the strategy here.
 
         """
-        pass
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/examples/strategies/ema_cross_bracket_algo.py` & `nautilus_trader-1.174.0/nautilus_trader/examples/strategies/ema_cross_bracket_algo.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,27 +29,27 @@
 from nautilus_trader.model.data.tick import QuoteTick
 from nautilus_trader.model.enums import OrderSide
 from nautilus_trader.model.enums import OrderType
 from nautilus_trader.model.enums import TimeInForce
 from nautilus_trader.model.enums import TriggerType
 from nautilus_trader.model.identifiers import ExecAlgorithmId
 from nautilus_trader.model.identifiers import InstrumentId
-from nautilus_trader.model.instruments.base import Instrument
+from nautilus_trader.model.instruments import Instrument
 from nautilus_trader.model.objects import Price
-from nautilus_trader.model.orders.list import OrderList
+from nautilus_trader.model.orders import OrderList
 from nautilus_trader.trading.strategy import Strategy
 
 
 # *** THIS IS A TEST STRATEGY WITH NO ALPHA ADVANTAGE WHATSOEVER. ***
 # *** IT IS NOT INTENDED TO BE USED TO TRADE LIVE WITH REAL MONEY. ***
 
 
 class EMACrossBracketAlgoConfig(StrategyConfig, frozen=True):
     """
-    Configuration for ``EMACrossBracketTWAP`` instances.
+    Configuration for ``EMACrossBracketAlgo`` instances.
 
     Parameters
     ----------
     instrument_id : InstrumentId
         The instrument ID for the strategy.
     bar_type : BarType
         The bar type for the strategy.
@@ -200,15 +200,14 @@
         ----------
         tick : QuoteTick
             The tick received.
 
         """
         # For debugging (must add a subscription)
         # self.log.info(repr(tick), LogColor.CYAN)
-        pass
 
     def on_bar(self, bar: Bar) -> None:
         """
         Actions to be performed when the strategy is running and receives a bar.
 
         Parameters
         ----------
@@ -319,27 +318,25 @@
 
         Parameters
         ----------
         data : Data
             The data received.
 
         """
-        pass
 
     def on_event(self, event: Event) -> None:
         """
         Actions to be performed when the strategy is running and receives an event.
 
         Parameters
         ----------
         event : Event
             The event received.
 
         """
-        pass
 
     def on_stop(self) -> None:
         """
         Actions to be performed when the strategy is stopped.
         """
         self.cancel_all_orders(self.instrument_id)
         self.close_all_positions(self.instrument_id)
@@ -378,17 +375,15 @@
 
         Parameters
         ----------
         state : dict[str, bytes]
             The strategy state dictionary.
 
         """
-        pass
 
     def on_dispose(self) -> None:
         """
         Actions to be performed when the strategy is disposed.
 
         Cleanup any resources used by the strategy here.
 
         """
-        pass
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/examples/strategies/ema_cross_cython.pyx` & `nautilus_trader-1.174.0/nautilus_trader/examples/strategies/ema_cross_cython.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/examples/strategies/ema_cross_stop_entry.py` & `nautilus_trader-1.174.0/nautilus_trader/examples/strategies/ema_cross_stop_entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,15 +178,14 @@
 
         Parameters
         ----------
         instrument : Instrument
             The instrument received.
 
         """
-        pass
 
     def on_order_book(self, order_book: OrderBook) -> None:
         """
         Actions to be performed when the strategy is running and receives an order book.
 
         Parameters
         ----------
@@ -202,39 +201,37 @@
 
         Parameters
         ----------
         tick : QuoteTick
             The tick received.
 
         """
-        pass
 
     def on_trade_tick(self, tick: TradeTick) -> None:
         """
         Actions to be performed when the strategy is running and receives a trade tick.
 
         Parameters
         ----------
         tick : TradeTick
             The tick received.
 
         """
-        pass
 
     def on_bar(self, bar: Bar) -> None:
         """
         Actions to be performed when the strategy is running and receives a bar.
 
         Parameters
         ----------
         bar : Bar
             The bar received.
 
         """
-        self.log.info(f"Received {repr(bar)}")
+        self.log.info(f"Received {bar!r}")
 
         # Check if indicators ready
         if not self.indicators_initialized():
             self.log.info(
                 f"Waiting for indicators to warm up " f"[{self.cache.bar_count(self.bar_type)}]...",
                 color=LogColor.BLUE,
             )
@@ -373,36 +370,33 @@
 
         Parameters
         ----------
         data : Data
             The data received.
 
         """
-        pass
 
     def on_event(self, event: Event) -> None:
         """
         Actions to be performed when the strategy is running and receives an event.
 
         Parameters
         ----------
         event : Event
             The event received.
 
         """
         if isinstance(event, OrderFilled):
-            if self.entry:
-                if event.client_order_id == self.entry.client_order_id:
-                    if event.order_side == OrderSide.BUY:
-                        self.trailing_stop_sell()
-                    elif event.order_side == OrderSide.SELL:
-                        self.trailing_stop_buy()
-            if self.trailing_stop:
-                if event.client_order_id == self.trailing_stop.client_order_id:
-                    self.trailing_stop = None
+            if self.entry and event.client_order_id == self.entry.client_order_id:
+                if event.order_side == OrderSide.BUY:
+                    self.trailing_stop_sell()
+                elif event.order_side == OrderSide.SELL:
+                    self.trailing_stop_buy()
+            if self.trailing_stop and event.client_order_id == self.trailing_stop.client_order_id:
+                self.trailing_stop = None
 
     def on_stop(self) -> None:
         """
         Actions to be performed when the strategy is stopped.
         """
         self.cancel_all_orders(self.instrument_id)
         self.close_all_positions(self.instrument_id)
@@ -443,17 +437,15 @@
 
         Parameters
         ----------
         state : dict[str, bytes]
             The strategy state dictionary.
 
         """
-        pass
 
     def on_dispose(self) -> None:
         """
         Actions to be performed when the strategy is disposed.
 
         Cleanup any resources used by the strategy here.
 
         """
-        pass
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/examples/strategies/ema_cross_trailing_stop.py` & `nautilus_trader-1.174.0/nautilus_trader/examples/strategies/ema_cross_trailing_stop.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,15 +196,14 @@
 
         Parameters
         ----------
         instrument : Instrument
             The instrument received.
 
         """
-        pass
 
     def on_order_book(self, order_book: OrderBook) -> None:
         """
         Actions to be performed when the strategy is running and receives an order book.
 
         Parameters
         ----------
@@ -220,39 +219,37 @@
 
         Parameters
         ----------
         tick : QuoteTick
             The tick received.
 
         """
-        pass
 
     def on_trade_tick(self, tick: TradeTick) -> None:
         """
         Actions to be performed when the strategy is running and receives a trade tick.
 
         Parameters
         ----------
         tick : TradeTick
             The tick received.
 
         """
-        pass
 
     def on_bar(self, bar: Bar) -> None:
         """
         Actions to be performed when the strategy is running and receives a bar.
 
         Parameters
         ----------
         bar : Bar
             The bar received.
 
         """
-        self.log.info(f"Received {repr(bar)}")
+        self.log.info(f"Received {bar!r}")
 
         # Check if indicators ready
         if not self.indicators_initialized():
             self.log.info(
                 f"Waiting for indicators to warm up " f"[{self.cache.bar_count(self.bar_type)}]...",
                 color=LogColor.BLUE,
             )
@@ -352,39 +349,36 @@
 
         Parameters
         ----------
         data : Data
             The data received.
 
         """
-        pass
 
     def on_event(self, event: Event) -> None:
         """
         Actions to be performed when the strategy is running and receives an event.
 
         Parameters
         ----------
         event : Event
             The event received.
 
         """
         if isinstance(event, OrderFilled):
-            if self.trailing_stop:
-                if event.client_order_id == self.trailing_stop.client_order_id:
-                    self.trailing_stop = None
+            if self.trailing_stop and event.client_order_id == self.trailing_stop.client_order_id:
+                self.trailing_stop = None
         elif isinstance(event, (PositionOpened, PositionChanged)):
-            if self.entry:
-                if event.opening_order_id == self.entry.client_order_id:
-                    if event.entry == OrderSide.BUY:
-                        self.position_id = event.position_id
-                        self.trailing_stop_sell()
-                    elif event.entry == OrderSide.SELL:
-                        self.position_id = event.position_id
-                        self.trailing_stop_buy()
+            if self.entry and event.opening_order_id == self.entry.client_order_id:
+                if event.entry == OrderSide.BUY:
+                    self.position_id = event.position_id
+                    self.trailing_stop_sell()
+                elif event.entry == OrderSide.SELL:
+                    self.position_id = event.position_id
+                    self.trailing_stop_buy()
         elif isinstance(event, PositionClosed):
             self.position_id = None
 
     def on_save(self) -> dict[str, bytes]:
         """
         Actions to be performed when the strategy is saved.
 
@@ -406,17 +400,15 @@
 
         Parameters
         ----------
         state : dict[str, bytes]
             The strategy state dictionary.
 
         """
-        pass
 
     def on_dispose(self) -> None:
         """
         Actions to be performed when the strategy is disposed.
 
         Cleanup any resources used by the strategy here.
 
         """
-        pass
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/examples/strategies/ema_cross_twap.py` & `nautilus_trader-1.174.0/nautilus_trader/examples/strategies/ema_cross_twap.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,46 +10,48 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 # -------------------------------------------------------------------------------------------------
 
 from decimal import Decimal
-from typing import Any
+from typing import Any, Union
 
 from nautilus_trader.common.enums import LogColor
 from nautilus_trader.config import StrategyConfig
 from nautilus_trader.config.validation import PositiveFloat
 from nautilus_trader.core.correctness import PyCondition
 from nautilus_trader.core.data import Data
 from nautilus_trader.core.message import Event
 from nautilus_trader.indicators.average.ema import ExponentialMovingAverage
 from nautilus_trader.model.data.bar import Bar
 from nautilus_trader.model.data.bar import BarType
+from nautilus_trader.model.data.book import OrderBookDelta
+from nautilus_trader.model.data.book import OrderBookDeltas
+from nautilus_trader.model.data.book import OrderBookSnapshot
 from nautilus_trader.model.data.tick import QuoteTick
 from nautilus_trader.model.data.tick import TradeTick
 from nautilus_trader.model.data.ticker import Ticker
 from nautilus_trader.model.enums import OrderSide
 from nautilus_trader.model.enums import TimeInForce
 from nautilus_trader.model.identifiers import ExecAlgorithmId
 from nautilus_trader.model.identifiers import InstrumentId
 from nautilus_trader.model.instruments import Instrument
 from nautilus_trader.model.orderbook import OrderBook
-from nautilus_trader.model.orderbook import OrderBookData
 from nautilus_trader.model.orders import MarketOrder
 from nautilus_trader.trading.strategy import Strategy
 
 
 # *** THIS IS A TEST STRATEGY WITH NO ALPHA ADVANTAGE WHATSOEVER. ***
 # *** IT IS NOT INTENDED TO BE USED TO TRADE LIVE WITH REAL MONEY. ***
 
 
 class EMACrossTWAPConfig(StrategyConfig, frozen=True):
     """
-    Configuration for ``EMACross`` instances.
+    Configuration for ``EMACrossTWAP`` instances.
 
     Parameters
     ----------
     instrument_id : InstrumentId
         The instrument ID for the strategy.
     bar_type : BarType
         The bar type for the strategy.
@@ -163,85 +165,82 @@
         ----------
         instrument : Instrument
             The instrument received.
 
         """
         # For debugging (must add a subscription)
         # self.log.info(repr(instrument), LogColor.CYAN)
-        pass
 
-    def on_order_book_delta(self, data: OrderBookData) -> None:
+    def on_order_book_delta(
+        self,
+        data: Union[OrderBookDelta, OrderBookDeltas, OrderBookSnapshot],
+    ) -> None:
         """
         Actions to be performed when the strategy is running and receives order data.
 
         Parameters
         ----------
-        data : OrderBookData
+        data : OrderBookDelta, OrderBookDeltas, OrderBookSnapshot
             The order book data received.
 
         """
         # For debugging (must add a subscription)
         # self.log.info(repr(data), LogColor.CYAN)
-        pass
 
     def on_order_book(self, order_book: OrderBook) -> None:
         """
         Actions to be performed when the strategy is running and receives an order book.
 
         Parameters
         ----------
         order_book : OrderBook
             The order book received.
 
         """
         # For debugging (must add a subscription)
         # self.log.info(repr(order_book), LogColor.CYAN)
-        pass
 
     def on_ticker(self, ticker: Ticker) -> None:
         """
         Actions to be performed when the strategy is running and receives a ticker.
 
         Parameters
         ----------
         ticker : Ticker
             The ticker received.
 
         """
         # For debugging (must add a subscription)
         # self.log.info(repr(ticker), LogColor.CYAN)
-        pass
 
     def on_quote_tick(self, tick: QuoteTick) -> None:
         """
         Actions to be performed when the strategy is running and receives a quote tick.
 
         Parameters
         ----------
         tick : QuoteTick
             The tick received.
 
         """
         # For debugging (must add a subscription)
         # self.log.info(repr(tick), LogColor.CYAN)
-        pass
 
     def on_trade_tick(self, tick: TradeTick) -> None:
         """
         Actions to be performed when the strategy is running and receives a trade tick.
 
         Parameters
         ----------
         tick : TradeTick
             The tick received.
 
         """
         # For debugging (must add a subscription)
         # self.log.info(repr(tick), LogColor.CYAN)
-        pass
 
     def on_bar(self, bar: Bar) -> None:
         """
         Actions to be performed when the strategy is running and receives a bar.
 
         Parameters
         ----------
@@ -314,27 +313,25 @@
 
         Parameters
         ----------
         data : Data
             The data received.
 
         """
-        pass
 
     def on_event(self, event: Event) -> None:
         """
         Actions to be performed when the strategy is running and receives an event.
 
         Parameters
         ----------
         event : Event
             The event received.
 
         """
-        pass
 
     def on_stop(self) -> None:
         """
         Actions to be performed when the strategy is stopped.
         """
         self.cancel_all_orders(self.instrument_id)
         if self.close_positions_on_stop:
@@ -373,17 +370,15 @@
 
         Parameters
         ----------
         state : dict[str, bytes]
             The strategy state dictionary.
 
         """
-        pass
 
     def on_dispose(self) -> None:
         """
         Actions to be performed when the strategy is disposed.
 
         Cleanup any resources used by the strategy here.
 
         """
-        pass
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/examples/strategies/market_maker.py` & `nautilus_trader-1.174.0/nautilus_trader/examples/strategies/market_maker.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,28 +10,30 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 # -------------------------------------------------------------------------------------------------
 
 from decimal import Decimal
-from typing import Optional
+from typing import Optional, Union
 
 from nautilus_trader.core.message import Event
+from nautilus_trader.model.data.book import OrderBookDelta
+from nautilus_trader.model.data.book import OrderBookDeltas
+from nautilus_trader.model.data.book import OrderBookSnapshot
 from nautilus_trader.model.enums import BookType
 from nautilus_trader.model.enums import OrderSide
 from nautilus_trader.model.enums import PositionSide
 from nautilus_trader.model.events.position import PositionChanged
 from nautilus_trader.model.events.position import PositionClosed
 from nautilus_trader.model.events.position import PositionOpened
 from nautilus_trader.model.identifiers import InstrumentId
 from nautilus_trader.model.instruments import Instrument
 from nautilus_trader.model.objects import Price
 from nautilus_trader.model.orderbook import OrderBook
-from nautilus_trader.model.orderbook import OrderBookData
 from nautilus_trader.trading.strategy import Strategy
 
 
 class MarketMaker(Strategy):
     """
     Provides a market making strategy for testing.
 
@@ -72,15 +74,18 @@
 
         # Create orderbook
         self._book = OrderBook.create(instrument=self.instrument, book_type=BookType.L2_MBP)
 
         # Subscribe to live data
         self.subscribe_order_book_deltas(self.instrument_id)
 
-    def on_order_book_delta(self, delta: OrderBookData) -> None:
+    def on_order_book_delta(
+        self,
+        delta: Union[OrderBookDelta, OrderBookDeltas, OrderBookSnapshot],
+    ) -> None:
         if not self._book:
             self.log.error("No book being maintained.")
             return
 
         self._book.apply(delta)
         bid_price = self._book.best_bid_price()
         ask_price = self._book.best_ask_price()
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/examples/strategies/orderbook_imbalance.py` & `nautilus_trader-1.174.0/nautilus_trader/examples/strategies/orderbook_imbalance.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,27 +10,29 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 # -------------------------------------------------------------------------------------------------
 
 from decimal import Decimal
-from typing import Optional
+from typing import Optional, Union
 
 from nautilus_trader.config import StrategyConfig
+from nautilus_trader.model.data.book import BookOrder
+from nautilus_trader.model.data.book import OrderBookDelta
+from nautilus_trader.model.data.book import OrderBookDeltas
+from nautilus_trader.model.data.book import OrderBookSnapshot
 from nautilus_trader.model.data.tick import QuoteTick
 from nautilus_trader.model.enums import BookType
 from nautilus_trader.model.enums import OrderSide
 from nautilus_trader.model.enums import TimeInForce
 from nautilus_trader.model.enums import book_type_from_str
 from nautilus_trader.model.identifiers import InstrumentId
 from nautilus_trader.model.instruments import Instrument
 from nautilus_trader.model.orderbook import OrderBook
-from nautilus_trader.model.orderbook import OrderBookData
-from nautilus_trader.model.orderbook.data import BookOrder
 from nautilus_trader.trading.strategy import Strategy
 
 
 # *** THIS IS A TEST STRATEGY WITH NO ALPHA ADVANTAGE WHATSOEVER. ***
 # *** IT IS NOT INTENDED TO BE USED TO TRADE LIVE WITH REAL MONEY. ***
 
 
@@ -110,15 +112,18 @@
         else:
             book_type = book_type_from_str(self.config.book_type)
             self.subscribe_order_book_deltas(self.instrument.id, book_type)
         if self.config.subscribe_ticker:
             self.subscribe_ticker(self.instrument.id)
         self._book = OrderBook.create(instrument=self.instrument, book_type=book_type)
 
-    def on_order_book_delta(self, data: OrderBookData) -> None:
+    def on_order_book_delta(
+        self,
+        data: Union[OrderBookDelta, OrderBookDeltas, OrderBookSnapshot],
+    ) -> None:
         """Actions to be performed when a delta is received."""
         if not self._book:
             self.log.error("No book being maintained.")
             return
 
         self._book.apply(data)
         if self._book.spread():
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/examples/strategies/signal_strategy.py` & `nautilus_trader-1.174.0/nautilus_trader/examples/strategies/signal_strategy.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/examples/strategies/subscribe.py` & `nautilus_trader-1.174.0/nautilus_trader/examples/strategies/subscribe.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,26 +12,26 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 # -------------------------------------------------------------------------------------------------
 
 from typing import Optional
 
 from nautilus_trader.config import StrategyConfig
+from nautilus_trader.core.data import Data
 from nautilus_trader.model.data.bar import Bar
 from nautilus_trader.model.data.bar import BarSpecification
 from nautilus_trader.model.data.bar import BarType
 from nautilus_trader.model.data.tick import QuoteTick
 from nautilus_trader.model.data.tick import TradeTick
 from nautilus_trader.model.enums import AggregationSource
 from nautilus_trader.model.enums import BarAggregation
 from nautilus_trader.model.enums import BookType
 from nautilus_trader.model.enums import PriceType
 from nautilus_trader.model.identifiers import InstrumentId
 from nautilus_trader.model.orderbook import OrderBook
-from nautilus_trader.model.orderbook import OrderBookData
 from nautilus_trader.trading.strategy import Strategy
 
 
 # *** THIS IS A TEST STRATEGY ***
 
 
 class SubscribeStrategyConfig(StrategyConfig, frozen=True):
@@ -98,15 +98,15 @@
                     aggregation=BarAggregation.SECOND,
                     price_type=PriceType.LAST,
                 ),
                 aggregation_source=AggregationSource.EXTERNAL,
             )
             self.subscribe_bars(bar_type)
 
-    def on_order_book_delta(self, data: OrderBookData) -> None:
+    def on_order_book_delta(self, data: Data) -> None:
         if not self.book:
             self.log.error("No book being maintained.")
             return
 
         self.book.apply(data)
         self.log.info(str(self.book))
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/examples/strategies/volatility_market_maker.py` & `nautilus_trader-1.174.0/nautilus_trader/examples/strategies/volatility_market_maker.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,25 +19,25 @@
 from nautilus_trader.common.enums import LogColor
 from nautilus_trader.config import StrategyConfig
 from nautilus_trader.core.data import Data
 from nautilus_trader.core.message import Event
 from nautilus_trader.indicators.atr import AverageTrueRange
 from nautilus_trader.model.data.bar import Bar
 from nautilus_trader.model.data.bar import BarType
+from nautilus_trader.model.data.book import OrderBookDelta
 from nautilus_trader.model.data.tick import QuoteTick
 from nautilus_trader.model.data.tick import TradeTick
 from nautilus_trader.model.data.ticker import Ticker
 from nautilus_trader.model.enums import OrderSide
 from nautilus_trader.model.enums import TimeInForce
 from nautilus_trader.model.enums import TriggerType
 from nautilus_trader.model.events.order import OrderFilled
 from nautilus_trader.model.identifiers import InstrumentId
 from nautilus_trader.model.instruments import Instrument
 from nautilus_trader.model.orderbook import OrderBook
-from nautilus_trader.model.orderbook import OrderBookDelta
 from nautilus_trader.model.orders import LimitOrder
 from nautilus_trader.trading.strategy import Strategy
 
 
 # *** THIS IS A TEST STRATEGY WITH NO ALPHA ADVANTAGE WHATSOEVER. ***
 # *** IT IS NOT INTENDED TO BE USED TO TRADE LIVE WITH REAL MONEY. ***
 
@@ -331,17 +331,18 @@
             return
 
         # If order filled then replace order at atr multiple distance from the market
         if isinstance(event, OrderFilled):
             if self.buy_order and event.order_side == OrderSide.BUY:
                 if self.buy_order.is_closed:
                     self.create_buy_order(last)
-            elif self.sell_order and event.order_side == OrderSide.SELL:
-                if self.sell_order.is_closed:
-                    self.create_sell_order(last)
+            elif (
+                self.sell_order and event.order_side == OrderSide.SELL and self.sell_order.is_closed
+            ):
+                self.create_sell_order(last)
 
     def on_stop(self) -> None:
         """
         Actions to be performed when the strategy is stopped.
         """
         self.cancel_all_orders(self.instrument_id)
         self.close_all_positions(self.instrument_id)
@@ -379,17 +380,15 @@
 
         Parameters
         ----------
         state : dict[str, bytes]
             The strategy state dictionary.
 
         """
-        pass
 
     def on_dispose(self) -> None:
         """
         Actions to be performed when the strategy is disposed.
 
         Cleanup any resources used by the strategy here.
 
         """
-        pass
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/execution/__init__.pxd` & `nautilus_trader-1.174.0/nautilus_trader/indicators/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/execution/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/execution/algorithm.pxd` & `nautilus_trader-1.174.0/nautilus_trader/execution/algorithm.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/execution/algorithm.pyx` & `nautilus_trader-1.174.0/nautilus_trader/execution/algorithm.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/execution/client.pxd` & `nautilus_trader-1.174.0/nautilus_trader/execution/client.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/execution/client.pyx` & `nautilus_trader-1.174.0/nautilus_trader/execution/client.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/execution/emulator.pxd` & `nautilus_trader-1.174.0/nautilus_trader/execution/emulator.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/execution/emulator.pyx` & `nautilus_trader-1.174.0/nautilus_trader/execution/emulator.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -589,40 +589,52 @@
 
         cdef dict exec_algorithm_index = {}
         cdef:
             ClientOrderId client_order_id
             SubmitOrderList submit_order_list
             Order contingent_order
             Order spawned_order
+            Order primary_order
             list exec_spawn_orders
             uint64_t raw_filled_qty
             Quantity filled_qty
         if order.contingency_type == ContingencyType.OTO:
             assert order.linked_order_ids
             submit_order_list = self._commands_submit_order_list.get(order.order_list_id)
             assert submit_order_list
             for client_order_id in order.linked_order_ids:
                 child_order = self.cache.order(client_order_id)
                 assert child_order, f"Cannot find child order for {repr(client_order_id)}"
+                if child_order.is_closed_c():
+                    continue
                 if not self.cache.load_submit_order_command(child_order.client_order_id):
                     self._create_new_submit_order(
                         order=child_order,
                         position_id=submit_order_list.position_id,
                         client_id=submit_order_list.client_id,
                     )
                     continue
 
-                # Check if execution algorithm spawned order
+                # Check if execution algorithm spawned order (only update based on primary)
                 if order.exec_spawn_id is None:
                     return
 
+                primary_order = self.cache.order(order.exec_spawn_id)
+                if primary_order is None:
+                    self._log.error(f"Cannot find primary order {repr(order.exec_spawn_id)}.")
+                    return
+
+                # Check if primary already pending cancel or completed (no need to update)
+                if primary_order.status == OrderStatus.PENDING_CANCEL or primary_order.is_closed_c():
+                    return
+
                 raw_filled_qty = 0
                 filled_qty = None
 
-                # Get primary order for execution spawn sequence
+                # Check total size of execution spawn sequence
                 exec_spawn_orders = self.cache.orders_for_exec_spawn(order.exec_spawn_id)
                 for spawned_order in exec_spawn_orders:
                     raw_filled_qty += spawned_order.filled_qty._mem.raw
                 raw_filled_qty += order.filled_qty._mem.raw
                 if raw_filled_qty != child_order.quantity._mem.raw:
                     filled_qty = Quantity.from_raw_c(raw_filled_qty, order.filled_qty._mem.precision)
                     self._log.info(
@@ -648,14 +660,18 @@
 
         cdef MatchingCore matching_core = None
         if order.is_closed_c():
             matching_core = self._matching_cores.get(order.instrument_id)
             if matching_core is not None:
                 matching_core.delete_order(order)
 
+        if order.exec_spawn_id is not None:
+            # Do not handle contingencies based on spawned execution algorithm orders
+            return
+
         cdef ClientOrderId client_order_id
         cdef Order contingent_order
         for client_order_id in order.linked_order_ids:
             contingent_order = self.cache.order(client_order_id)
             assert contingent_order
             if client_order_id == order.client_order_id:
                 continue  # Already being handled
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/execution/engine.pxd` & `nautilus_trader-1.174.0/nautilus_trader/execution/engine.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/execution/engine.pyx` & `nautilus_trader-1.174.0/nautilus_trader/execution/engine.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/execution/matching_core.pxd` & `nautilus_trader-1.174.0/nautilus_trader/execution/matching_core.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/execution/matching_core.pyx` & `nautilus_trader-1.174.0/nautilus_trader/execution/matching_core.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/execution/messages.pxd` & `nautilus_trader-1.174.0/nautilus_trader/execution/messages.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/execution/messages.pyx` & `nautilus_trader-1.174.0/nautilus_trader/execution/messages.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/execution/reports.pxd` & `nautilus_trader-1.174.0/nautilus_trader/execution/reports.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/execution/reports.pyx` & `nautilus_trader-1.174.0/nautilus_trader/execution/reports.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/execution/trailing.pxd` & `nautilus_trader-1.174.0/nautilus_trader/execution/trailing.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/execution/trailing.pyx` & `nautilus_trader-1.174.0/nautilus_trader/execution/trailing.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/__init__.pxd` & `nautilus_trader-1.174.0/nautilus_trader/indicators/average/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/indicators/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/amat.pxd` & `nautilus_trader-1.174.0/nautilus_trader/indicators/amat.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/amat.pyx` & `nautilus_trader-1.174.0/nautilus_trader/indicators/amat.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/aroon.pxd` & `nautilus_trader-1.174.0/nautilus_trader/indicators/aroon.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/aroon.pyx` & `nautilus_trader-1.174.0/nautilus_trader/indicators/aroon.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/atr.pxd` & `nautilus_trader-1.174.0/nautilus_trader/indicators/atr.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/atr.pyx` & `nautilus_trader-1.174.0/nautilus_trader/indicators/atr.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/average/__init__.pxd` & `nautilus_trader-1.174.0/nautilus_trader/indicators/average/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/average/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/indicators/base/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/average/ama.pxd` & `nautilus_trader-1.174.0/nautilus_trader/indicators/average/ama.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/average/ama.pyx` & `nautilus_trader-1.174.0/nautilus_trader/indicators/average/ama.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/average/dema.pxd` & `nautilus_trader-1.174.0/nautilus_trader/indicators/average/dema.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/average/dema.pyx` & `nautilus_trader-1.174.0/nautilus_trader/indicators/average/dema.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/average/ema.pxd` & `nautilus_trader-1.174.0/nautilus_trader/indicators/average/ema.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/average/ema.pyx` & `nautilus_trader-1.174.0/nautilus_trader/indicators/average/ema.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/average/hma.pxd` & `nautilus_trader-1.174.0/nautilus_trader/indicators/average/hma.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/average/hma.pyx` & `nautilus_trader-1.174.0/nautilus_trader/indicators/average/hma.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/average/ma_factory.pyx` & `nautilus_trader-1.174.0/nautilus_trader/indicators/average/ma_factory.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/average/moving_average.pxd` & `nautilus_trader-1.174.0/nautilus_trader/indicators/average/moving_average.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/average/moving_average.pyx` & `nautilus_trader-1.174.0/nautilus_trader/indicators/average/moving_average.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/average/rma.pxd` & `nautilus_trader-1.174.0/nautilus_trader/indicators/average/rma.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/average/rma.pyx` & `nautilus_trader-1.174.0/nautilus_trader/indicators/average/rma.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/average/sma.pxd` & `nautilus_trader-1.174.0/nautilus_trader/indicators/average/sma.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/average/sma.pyx` & `nautilus_trader-1.174.0/nautilus_trader/indicators/average/sma.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/average/vidya.pxd` & `nautilus_trader-1.174.0/nautilus_trader/indicators/average/vidya.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/average/vidya.pyx` & `nautilus_trader-1.174.0/nautilus_trader/indicators/average/vidya.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/average/wma.pxd` & `nautilus_trader-1.174.0/nautilus_trader/indicators/average/wma.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/average/wma.pyx` & `nautilus_trader-1.174.0/nautilus_trader/indicators/average/wma.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/base/__init__.pxd` & `nautilus_trader-1.174.0/nautilus_trader/indicators/base/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/base/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/indicators/fuzzy_enums/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/base/indicator.pxd` & `nautilus_trader-1.174.0/nautilus_trader/indicators/base/indicator.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/base/indicator.pyx` & `nautilus_trader-1.174.0/nautilus_trader/indicators/base/indicator.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/bias.pxd` & `nautilus_trader-1.174.0/nautilus_trader/indicators/bias.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/bias.pyx` & `nautilus_trader-1.174.0/nautilus_trader/indicators/bias.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/bollinger_bands.pxd` & `nautilus_trader-1.174.0/nautilus_trader/indicators/bollinger_bands.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/bollinger_bands.pyx` & `nautilus_trader-1.174.0/nautilus_trader/indicators/bollinger_bands.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/cci.pxd` & `nautilus_trader-1.174.0/nautilus_trader/indicators/cci.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/cci.pyx` & `nautilus_trader-1.174.0/nautilus_trader/indicators/cci.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/cmo.pxd` & `nautilus_trader-1.174.0/nautilus_trader/indicators/cmo.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/cmo.pyx` & `nautilus_trader-1.174.0/nautilus_trader/indicators/cmo.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/dm.pxd` & `nautilus_trader-1.174.0/nautilus_trader/indicators/dm.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/dm.pyx` & `nautilus_trader-1.174.0/nautilus_trader/indicators/dm.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/donchian_channel.pxd` & `nautilus_trader-1.174.0/nautilus_trader/indicators/donchian_channel.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/donchian_channel.pyx` & `nautilus_trader-1.174.0/nautilus_trader/indicators/donchian_channel.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/efficiency_ratio.pxd` & `nautilus_trader-1.174.0/nautilus_trader/indicators/efficiency_ratio.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/efficiency_ratio.pyx` & `nautilus_trader-1.174.0/nautilus_trader/indicators/efficiency_ratio.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/fuzzy_candlesticks.pxd` & `nautilus_trader-1.174.0/nautilus_trader/indicators/fuzzy_candlesticks.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/fuzzy_candlesticks.pyx` & `nautilus_trader-1.174.0/nautilus_trader/indicators/fuzzy_candlesticks.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/fuzzy_enum.pyx` & `nautilus_trader-1.174.0/nautilus_trader/indicators/fuzzy_enum.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/fuzzy_enums/__init__.pxd` & `nautilus_trader-1.174.0/nautilus_trader/indicators/fuzzy_enums/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/fuzzy_enums/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/infrastructure/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/fuzzy_enums/candle_body.pxd` & `nautilus_trader-1.174.0/nautilus_trader/indicators/fuzzy_enums/candle_body.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/fuzzy_enums/candle_body.pyx` & `nautilus_trader-1.174.0/nautilus_trader/indicators/fuzzy_enums/candle_body.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/fuzzy_enums/candle_direction.pxd` & `nautilus_trader-1.174.0/nautilus_trader/indicators/fuzzy_enums/candle_direction.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/fuzzy_enums/candle_direction.pyx` & `nautilus_trader-1.174.0/nautilus_trader/indicators/fuzzy_enums/candle_direction.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/fuzzy_enums/candle_size.pxd` & `nautilus_trader-1.174.0/nautilus_trader/indicators/fuzzy_enums/candle_size.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/fuzzy_enums/candle_size.pyx` & `nautilus_trader-1.174.0/nautilus_trader/indicators/fuzzy_enums/candle_size.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/fuzzy_enums/candle_wick.pxd` & `nautilus_trader-1.174.0/nautilus_trader/indicators/fuzzy_enums/candle_wick.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/fuzzy_enums/candle_wick.pyx` & `nautilus_trader-1.174.0/nautilus_trader/indicators/fuzzy_enums/candle_wick.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/keltner_channel.pxd` & `nautilus_trader-1.174.0/nautilus_trader/indicators/keltner_channel.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/keltner_channel.pyx` & `nautilus_trader-1.174.0/nautilus_trader/indicators/keltner_channel.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/keltner_position.pxd` & `nautilus_trader-1.174.0/nautilus_trader/indicators/keltner_position.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/keltner_position.pyx` & `nautilus_trader-1.174.0/nautilus_trader/indicators/keltner_position.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/kvo.pxd` & `nautilus_trader-1.174.0/nautilus_trader/indicators/kvo.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/kvo.pyx` & `nautilus_trader-1.174.0/nautilus_trader/indicators/kvo.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/linear_regression.pxd` & `nautilus_trader-1.174.0/nautilus_trader/indicators/linear_regression.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/linear_regression.pyx` & `nautilus_trader-1.174.0/nautilus_trader/indicators/linear_regression.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/macd.pxd` & `nautilus_trader-1.174.0/nautilus_trader/indicators/macd.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/macd.pyx` & `nautilus_trader-1.174.0/nautilus_trader/indicators/macd.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/obv.pxd` & `nautilus_trader-1.174.0/nautilus_trader/indicators/obv.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/obv.pyx` & `nautilus_trader-1.174.0/nautilus_trader/indicators/obv.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/pressure.pxd` & `nautilus_trader-1.174.0/nautilus_trader/indicators/pressure.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/pressure.pyx` & `nautilus_trader-1.174.0/nautilus_trader/indicators/pressure.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/psl.pxd` & `nautilus_trader-1.174.0/nautilus_trader/indicators/psl.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/psl.pyx` & `nautilus_trader-1.174.0/nautilus_trader/indicators/psl.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/roc.pxd` & `nautilus_trader-1.174.0/nautilus_trader/indicators/roc.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/roc.pyx` & `nautilus_trader-1.174.0/nautilus_trader/indicators/roc.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/rsi.pxd` & `nautilus_trader-1.174.0/nautilus_trader/indicators/rsi.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/rsi.pyx` & `nautilus_trader-1.174.0/nautilus_trader/indicators/rsi.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/rvi.pxd` & `nautilus_trader-1.174.0/nautilus_trader/indicators/rvi.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/rvi.pyx` & `nautilus_trader-1.174.0/nautilus_trader/indicators/rvi.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/spread_analyzer.pxd` & `nautilus_trader-1.174.0/nautilus_trader/indicators/spread_analyzer.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/spread_analyzer.pyx` & `nautilus_trader-1.174.0/nautilus_trader/indicators/spread_analyzer.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/stochastics.pxd` & `nautilus_trader-1.174.0/nautilus_trader/indicators/stochastics.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/stochastics.pyx` & `nautilus_trader-1.174.0/nautilus_trader/indicators/stochastics.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/swings.pxd` & `nautilus_trader-1.174.0/nautilus_trader/indicators/swings.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/swings.pyx` & `nautilus_trader-1.174.0/nautilus_trader/indicators/swings.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/vhf.pxd` & `nautilus_trader-1.174.0/nautilus_trader/indicators/vhf.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/vhf.pyx` & `nautilus_trader-1.174.0/nautilus_trader/indicators/vhf.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/volatility_ratio.pxd` & `nautilus_trader-1.174.0/nautilus_trader/indicators/volatility_ratio.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/volatility_ratio.pyx` & `nautilus_trader-1.174.0/nautilus_trader/indicators/volatility_ratio.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/vwap.pxd` & `nautilus_trader-1.174.0/nautilus_trader/indicators/vwap.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/indicators/vwap.pyx` & `nautilus_trader-1.174.0/nautilus_trader/indicators/vwap.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/infrastructure/__init__.pxd` & `nautilus_trader-1.174.0/nautilus_trader/model/data/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/infrastructure/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/infrastructure/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/infrastructure/cache.pxd` & `nautilus_trader-1.174.0/nautilus_trader/infrastructure/cache.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/infrastructure/cache.pyx` & `nautilus_trader-1.174.0/nautilus_trader/infrastructure/cache.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/live/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/live/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/live/__main__.py` & `nautilus_trader-1.174.0/nautilus_trader/live/__main__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/live/data_client.py` & `nautilus_trader-1.174.0/nautilus_trader/live/data_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,24 +161,24 @@
         self,
         actions: Optional[Callable],
         success: Optional[str],
         task: Task,
     ) -> None:
         if task.exception():
             self._log.error(
-                f"Error on `{task.get_name()}`: " f"{repr(task.exception())}",
+                f"Error on `{task.get_name()}`: " f"{task.exception()!r}",
             )
         else:
             if actions:
                 try:
                     actions()
                 except Exception as e:
                     self._log.error(
                         f"Failed triggering action {actions.__name__} on `{task.get_name()}`: "
-                        f"{repr(e)}",
+                        f"{e!r}",
                     )
             if success:
                 self._log.info(success, LogColor.GREEN)
 
     def connect(self) -> None:
         """
         Connect the client.
@@ -377,24 +377,24 @@
         self,
         actions: Optional[Callable],
         success: Optional[str],
         task: Task,
     ) -> None:
         if task.exception():
             self._log.error(
-                f"Error on `{task.get_name()}`: " f"{repr(task.exception())}",
+                f"Error on `{task.get_name()}`: " f"{task.exception()!r}",
             )
         else:
             if actions:
                 try:
                     actions()
                 except Exception as e:
                     self._log.error(
                         f"Failed triggering action {actions.__name__} on `{task.get_name()}`: "
-                        f"{repr(e)}",
+                        f"{e!r}",
                     )
             if success:
                 self._log.info(success, LogColor.GREEN)
 
     def connect(self) -> None:
         """
         Connect the client.
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/live/data_engine.py` & `nautilus_trader-1.174.0/nautilus_trader/live/data_engine.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/live/execution_client.py` & `nautilus_trader-1.174.0/nautilus_trader/live/execution_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,24 +195,24 @@
         self,
         actions: Optional[Callable],
         success: Optional[str],
         task: Task,
     ) -> None:
         if task.exception():
             self._log.error(
-                f"Error on `{task.get_name()}`: " f"{repr(task.exception())}",
+                f"Error on `{task.get_name()}`: " f"{task.exception()!r}",
             )
         else:
             if actions:
                 try:
                     actions()
                 except Exception as e:
                     self._log.error(
                         f"Failed triggering action {actions.__name__} on `{task.get_name()}`: "
-                        f"{repr(e)}",
+                        f"{e!r}",
                     )
             if success:
                 self._log.info(success, LogColor.GREEN)
 
     def connect(self) -> None:
         """
         Connect the client.
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/live/execution_engine.py` & `nautilus_trader-1.174.0/nautilus_trader/live/execution_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -747,15 +747,15 @@
         )
 
         self._log.warning(f"Generated inferred {filled}.")
         return filled
 
     def _generate_external_order(self, report: OrderStatusReport) -> Order:
         self._log.info(
-            f"Generating external order {repr(report.client_order_id)}",
+            f"Generating external order {report.client_order_id!r}",
             color=LogColor.BLUE,
         )
 
         # Prepare order options
         options: dict[str, Any] = {}
         if report.price is not None:
             options["price"] = str(report.price)
@@ -957,11 +957,10 @@
             or order.order_type == OrderType.TRAILING_STOP_MARKET
         ):
             if report.trigger_price != order.trigger_price:
                 return True
         elif (
             order.order_type == OrderType.STOP_LIMIT
             or order.order_type == OrderType.TRAILING_STOP_LIMIT
-        ):
-            if report.trigger_price != order.trigger_price or report.price != order.price:
-                return True
+        ) and (report.trigger_price != order.trigger_price or report.price != order.price):
+            return True
         return False
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/live/factories.py` & `nautilus_trader-1.174.0/nautilus_trader/live/factories.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/live/node.py` & `nautilus_trader-1.174.0/nautilus_trader/live/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -274,15 +274,15 @@
             if self.kernel.loop.is_running():
                 self.kernel.loop.create_task(self.stop_async())
             else:
                 self.kernel.loop.run_until_complete(self.stop_async())
         except RuntimeError as e:
             self.kernel.log.exception("Error on stop", e)
 
-    def dispose(self) -> None:  # noqa C901 'TradingNode.dispose' is too complex (11)
+    def dispose(self) -> None:  # noqa: C901
         """
         Dispose of the trading node.
 
         Gracefully shuts down the executor and event loop.
         """
         try:
             timeout = self.kernel.clock.utc_now() + timedelta(
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/live/node_builder.py` & `nautilus_trader-1.174.0/nautilus_trader/live/node_builder.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/live/risk_engine.py` & `nautilus_trader-1.174.0/nautilus_trader/live/risk_engine.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/__init__.pxd` & `nautilus_trader-1.174.0/nautilus_trader/model/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/model/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/currencies.pxd` & `nautilus_trader-1.174.0/nautilus_trader/model/currencies.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/currencies.pyx` & `nautilus_trader-1.174.0/nautilus_trader/model/currencies.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/currency.pxd` & `nautilus_trader-1.174.0/nautilus_trader/model/currency.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/currency.pyx` & `nautilus_trader-1.174.0/nautilus_trader/model/currency.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/data/__init__.pxd` & `nautilus_trader-1.174.0/nautilus_trader/model/events/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/data/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/model/data/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/data/bar.pxd` & `nautilus_trader-1.174.0/nautilus_trader/model/data/bar.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/data/bar.pyx` & `nautilus_trader-1.174.0/nautilus_trader/model/data/bar.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/data/bar_aggregation.pxd` & `nautilus_trader-1.174.0/nautilus_trader/model/data/bar_aggregation.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/data/bar_aggregation.pyx` & `nautilus_trader-1.174.0/nautilus_trader/model/data/bar_aggregation.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/data/base.pxd` & `nautilus_trader-1.174.0/nautilus_trader/model/data/base.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/data/base.pyx` & `nautilus_trader-1.174.0/nautilus_trader/model/data/base.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/data/bet.pxd` & `nautilus_trader-1.174.0/nautilus_trader/model/data/bet.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/data/bet.pyx` & `nautilus_trader-1.174.0/nautilus_trader/model/data/bet.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/data/tick.pxd` & `nautilus_trader-1.174.0/nautilus_trader/model/data/tick.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/data/tick.pyx` & `nautilus_trader-1.174.0/nautilus_trader/model/data/tick.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/data/ticker.pxd` & `nautilus_trader-1.174.0/nautilus_trader/model/data/ticker.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/data/ticker.pyx` & `nautilus_trader-1.174.0/nautilus_trader/model/data/ticker.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/data/venue.pxd` & `nautilus_trader-1.174.0/nautilus_trader/model/data/venue.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/data/venue.pyx` & `nautilus_trader-1.174.0/nautilus_trader/model/data/venue.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/enums.pyx` & `nautilus_trader-1.174.0/nautilus_trader/model/enums.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/enums_c.pxd` & `nautilus_trader-1.174.0/nautilus_trader/model/enums_c.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/enums_c.pyx` & `nautilus_trader-1.174.0/nautilus_trader/model/enums_c.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/events/__init__.pxd` & `nautilus_trader-1.174.0/nautilus_trader/model/orderbook/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/events/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/persistence/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 # -------------------------------------------------------------------------------------------------
 
-"""Defines the fundamental event types represented within the trading domain."""
+"""The `persistence` subpackage handles data storage and retrieval, mainly to support backtesting."""
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/events/account.pxd` & `nautilus_trader-1.174.0/nautilus_trader/model/events/account.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/events/account.pyx` & `nautilus_trader-1.174.0/nautilus_trader/model/events/account.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/events/order.pxd` & `nautilus_trader-1.174.0/nautilus_trader/model/events/order.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/events/order.pyx` & `nautilus_trader-1.174.0/nautilus_trader/model/events/order.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/events/position.pxd` & `nautilus_trader-1.174.0/nautilus_trader/model/events/position.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/events/position.pyx` & `nautilus_trader-1.174.0/nautilus_trader/model/events/position.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/identifiers.pxd` & `nautilus_trader-1.174.0/nautilus_trader/model/identifiers.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/identifiers.pyx` & `nautilus_trader-1.174.0/nautilus_trader/model/identifiers.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/instruments/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/model/instruments/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/instruments/base.pxd` & `nautilus_trader-1.174.0/nautilus_trader/model/instruments/base.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/instruments/base.pyx` & `nautilus_trader-1.174.0/nautilus_trader/model/instruments/base.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/instruments/betting.pxd` & `nautilus_trader-1.174.0/nautilus_trader/model/instruments/betting.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/instruments/betting.pyx` & `nautilus_trader-1.174.0/nautilus_trader/model/instruments/betting.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/instruments/crypto_future.pxd` & `nautilus_trader-1.174.0/nautilus_trader/model/instruments/crypto_future.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/instruments/crypto_future.pyx` & `nautilus_trader-1.174.0/nautilus_trader/model/instruments/crypto_future.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/instruments/crypto_perpetual.pxd` & `nautilus_trader-1.174.0/nautilus_trader/model/instruments/crypto_perpetual.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/instruments/crypto_perpetual.pyx` & `nautilus_trader-1.174.0/nautilus_trader/model/instruments/crypto_perpetual.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/instruments/currency_pair.pxd` & `nautilus_trader-1.174.0/nautilus_trader/model/instruments/currency_pair.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/instruments/currency_pair.pyx` & `nautilus_trader-1.174.0/nautilus_trader/model/instruments/currency_pair.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/instruments/equity.pxd` & `nautilus_trader-1.174.0/nautilus_trader/model/instruments/equity.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/instruments/equity.pyx` & `nautilus_trader-1.174.0/nautilus_trader/model/instruments/equity.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/instruments/futures_contract.pxd` & `nautilus_trader-1.174.0/nautilus_trader/model/instruments/futures_contract.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/instruments/futures_contract.pyx` & `nautilus_trader-1.174.0/nautilus_trader/model/instruments/futures_contract.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/instruments/options_contract.pxd` & `nautilus_trader-1.174.0/nautilus_trader/model/instruments/options_contract.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/instruments/options_contract.pyx` & `nautilus_trader-1.174.0/nautilus_trader/model/instruments/options_contract.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/objects.pxd` & `nautilus_trader-1.174.0/nautilus_trader/model/objects.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/objects.pyx` & `nautilus_trader-1.174.0/nautilus_trader/model/objects.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/orderbook/__init__.pxd` & `nautilus_trader-1.174.0/nautilus_trader/model/orders/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/orderbook/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/model/orderbook/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,27 +13,27 @@
 #  limitations under the License.
 # -------------------------------------------------------------------------------------------------
 
 """
 Defines real-time and simulated order book components and data.
 """
 
+from nautilus_trader.model.data.book import BookOrder
+from nautilus_trader.model.data.book import OrderBookDelta
+from nautilus_trader.model.data.book import OrderBookDeltas
+from nautilus_trader.model.data.book import OrderBookSnapshot
 from nautilus_trader.model.orderbook.book import L1OrderBook
 from nautilus_trader.model.orderbook.book import L2OrderBook
 from nautilus_trader.model.orderbook.book import L3OrderBook
 from nautilus_trader.model.orderbook.book import OrderBook
-from nautilus_trader.model.orderbook.data import OrderBookData
-from nautilus_trader.model.orderbook.data import OrderBookDelta
-from nautilus_trader.model.orderbook.data import OrderBookDeltas
-from nautilus_trader.model.orderbook.data import OrderBookSnapshot
 
 
 __all__ = [
+    "BookOrder",
+    "OrderBookDelta",
+    "OrderBookDeltas",
+    "OrderBookSnapshot",
     "L1OrderBook",
     "L2OrderBook",
     "L3OrderBook",
     "OrderBook",
-    "OrderBookData",
-    "OrderBookDelta",
-    "OrderBookDeltas",
-    "OrderBookSnapshot",
 ]
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/orderbook/book.pxd` & `nautilus_trader-1.174.0/nautilus_trader/model/orderbook/book.pxd`

 * *Files 9% similar despite different names*

```diff
@@ -12,23 +12,23 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 # -------------------------------------------------------------------------------------------------
 
 from libc.stdint cimport uint8_t
 from libc.stdint cimport uint64_t
 
+from nautilus_trader.core.data cimport Data
+from nautilus_trader.model.data.book cimport BookOrder
+from nautilus_trader.model.data.book cimport OrderBookDelta
+from nautilus_trader.model.data.book cimport OrderBookDeltas
+from nautilus_trader.model.data.book cimport OrderBookSnapshot
 from nautilus_trader.model.data.tick cimport QuoteTick
 from nautilus_trader.model.data.tick cimport TradeTick
 from nautilus_trader.model.enums_c cimport BookType
 from nautilus_trader.model.identifiers cimport InstrumentId
-from nautilus_trader.model.orderbook.data cimport BookOrder
-from nautilus_trader.model.orderbook.data cimport OrderBookData
-from nautilus_trader.model.orderbook.data cimport OrderBookDelta
-from nautilus_trader.model.orderbook.data cimport OrderBookDeltas
-from nautilus_trader.model.orderbook.data cimport OrderBookSnapshot
 from nautilus_trader.model.orderbook.ladder cimport Ladder
 from nautilus_trader.model.orderbook.level cimport Level
 
 
 cdef class OrderBook:
     cdef readonly InstrumentId instrument_id
     """The order book instrument ID.\n\n:returns: `InstrumentId`"""
@@ -51,15 +51,15 @@
 
     cpdef void add(self, BookOrder order, uint64_t sequence=*)
     cpdef void update(self, BookOrder order, uint64_t sequence=*)
     cpdef void delete(self, BookOrder order, uint64_t sequence=*)
     cpdef void apply_delta(self, OrderBookDelta delta)
     cpdef void apply_deltas(self, OrderBookDeltas deltas)
     cpdef void apply_snapshot(self, OrderBookSnapshot snapshot)
-    cpdef void apply(self, OrderBookData data)
+    cpdef void apply(self, Data data)
     cpdef void clear_bids(self)
     cpdef void clear_asks(self)
     cpdef void clear(self)
     cpdef void check_integrity(self)
     cdef void _add(self, BookOrder order, uint64_t sequence)
     cdef void _update(self, BookOrder order, uint64_t sequence)
     cdef void _delete(self, BookOrder order, uint64_t sequence)
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/orderbook/book.pyx` & `nautilus_trader-1.174.0/nautilus_trader/model/orderbook/book.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -20,23 +20,23 @@
 
 from nautilus_trader.model.orderbook.error import BookIntegrityError
 
 from libc.stdint cimport uint8_t
 from libc.stdint cimport uint64_t
 
 from nautilus_trader.core.correctness cimport Condition
+from nautilus_trader.model.data.book cimport BookOrder
+from nautilus_trader.model.data.book cimport OrderBookSnapshot
 from nautilus_trader.model.data.tick cimport TradeTick
 from nautilus_trader.model.enums_c cimport BookAction
 from nautilus_trader.model.enums_c cimport BookType
 from nautilus_trader.model.enums_c cimport OrderSide
 from nautilus_trader.model.enums_c cimport order_side_to_str
 from nautilus_trader.model.identifiers cimport InstrumentId
 from nautilus_trader.model.instruments.base cimport Instrument
-from nautilus_trader.model.orderbook.data cimport BookOrder
-from nautilus_trader.model.orderbook.data cimport OrderBookSnapshot
 from nautilus_trader.model.orderbook.ladder cimport Ladder
 from nautilus_trader.model.orderbook.level cimport Level
 from nautilus_trader.model.orderbook.simulated cimport SimulatedL1OrderBook
 from nautilus_trader.model.orderbook.simulated cimport SimulatedL2OrderBook
 from nautilus_trader.model.orderbook.simulated cimport SimulatedL3OrderBook
 
 
@@ -202,57 +202,44 @@
         Raises
         ------
         ValueError
             If `delta.book_type` is not equal to `self.type`.
 
         """
         Condition.not_none(delta, "delta")
-        Condition.equal(delta.book_type, self.type, "delta.book_type", "self.type")
 
         self._apply_delta(delta)
 
     cpdef void apply_deltas(self, OrderBookDeltas deltas):
         """
         Apply the bulk deltas to the order book.
 
         Parameters
         ----------
         deltas : OrderBookDeltas
             The deltas to apply.
 
-        Raises
-        ------
-        ValueError
-            If `snapshot.book_type` is not equal to `self.type`.
-
         """
         Condition.not_none(deltas, "deltas")
-        Condition.equal(deltas.book_type, self.type, "deltas.book_type", "self.type")
 
         cdef OrderBookDelta delta
         for delta in deltas.deltas:
             self._apply_delta(delta)
 
     cpdef void apply_snapshot(self, OrderBookSnapshot snapshot):
         """
         Apply the bulk snapshot to the order book.
 
         Parameters
         ----------
         snapshot : OrderBookSnapshot
             The snapshot to apply.
 
-        Raises
-        ------
-        ValueError
-            If `snapshot.book_type` is not equal to `self.type`.
-
         """
         Condition.not_none(snapshot, "snapshot")
-        Condition.equal(snapshot.book_type, self.type, "snapshot.book_type", "self.type")
 
         self.clear()
         # Use `update` instead of `add` (when book has been cleared they're
         # equivalent) to make work for L1_TBBO Orderbook.
         cdef BookOrder order
         for bid in snapshot.bids:
             order = BookOrder(
@@ -267,37 +254,32 @@
                 size=ask[1],
                 side=OrderSide.SELL
             )
             self.update(order=order, sequence=snapshot.sequence)
 
         self.ts_last = snapshot.ts_init
 
-    cpdef void apply(self, OrderBookData data):
+    cpdef void apply(self, Data data):
         """
-        Apply the data to the order book.
+        Apply the given data to the order book.
 
         Parameters
         ----------
-        data : OrderBookData
+        delta : OrderBookDelta, OrderBookDeltas, OrderBookSnapshot
             The data to apply.
 
-        Raises
-        ------
-        ValueError
-            If `data.level` is not equal to `self.type`.
-
         """
-        Condition(data.book_type, self.type, "data.book_type", "self.type")
-
         if isinstance(data, OrderBookSnapshot):
             self.apply_snapshot(snapshot=data)
         elif isinstance(data, OrderBookDeltas):
             self.apply_deltas(deltas=data)
         elif isinstance(data, OrderBookDelta):
             self._apply_delta(delta=data)
+        else:  # pragma: no-cover (design time error)
+            raise RuntimeError(f"invalid order book data type, was {type(data)}")  # pragma: no-cover (design time error)
 
     cpdef void check_integrity(self):
         """
         Check order book integrity.
 
         For all order books:
         - The bid side price should not be greater than the ask side price.
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/orderbook/data.pxd` & `nautilus_trader-1.174.0/nautilus_trader/model/data/book.pxd`

 * *Files 20% similar despite different names*

```diff
@@ -12,83 +12,90 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 # -------------------------------------------------------------------------------------------------
 
 from libc.stdint cimport uint64_t
 
 from nautilus_trader.core.data cimport Data
+from nautilus_trader.model.data.book cimport OrderBookDelta
+from nautilus_trader.model.data.book cimport OrderBookDeltas
+from nautilus_trader.model.data.book cimport OrderBookSnapshot
 from nautilus_trader.model.enums_c cimport BookAction
 from nautilus_trader.model.enums_c cimport BookType
 from nautilus_trader.model.enums_c cimport OrderSide
 from nautilus_trader.model.enums_c cimport TimeInForce
 from nautilus_trader.model.identifiers cimport InstrumentId
 
 
-cdef class OrderBookData(Data):
-    cdef readonly InstrumentId instrument_id
-    """The instrument ID for the order book.\n\n:returns: `InstrumentId`"""
-    cdef readonly BookType book_type
-    """The order book type (L1_TBBO, L2_MBP, L3_MBO).\n\n:returns: `BookType`"""
-    cdef readonly TimeInForce time_in_force
-    """The time in force for this update.\n\n:returns: `TimeInForce`"""
-    cdef readonly uint64_t sequence
-    """The unique sequence number.\n\n:returns: `uint64`"""
-
-
-cdef class OrderBookSnapshot(OrderBookData):
-    cdef readonly list bids
-    """The snapshot bids.\n\n:returns: `list`"""
-    cdef readonly list asks
-    """The snapshot asks.\n\n:returns: `list`"""
+cdef tuple ORDER_BOOK_DATA
 
-    @staticmethod
-    cdef OrderBookSnapshot from_dict_c(dict values)
-
-    @staticmethod
-    cdef dict to_dict_c(OrderBookSnapshot obj)
 
+cdef class BookOrder:
+    cdef readonly double price
+    """The orders price.\n\n:returns: `double`"""
+    cdef readonly double size
+    """The orders size.\n\n:returns: `double`"""
+    cdef readonly OrderSide side
+    """The orders side.\n\n:returns: `OrderSide`"""
+    cdef readonly str order_id
+    """The orders ID.\n\n:returns: `str`"""
 
-cdef class OrderBookDeltas(OrderBookData):
-    cdef readonly list deltas
-    """The order book deltas.\n\n:returns: `list[OrderBookDelta]`"""
+    cpdef void update_price(self, double price)
+    cpdef void update_size(self, double size)
+    cpdef void update_order_id(self, str value)
+    cpdef double exposure(self)
+    cpdef double signed_size(self)
 
     @staticmethod
-    cdef OrderBookDeltas from_dict_c(dict values)
+    cdef BookOrder from_dict_c(dict values)
 
     @staticmethod
-    cdef dict to_dict_c(OrderBookDeltas obj)
+    cdef dict to_dict_c(BookOrder obj)
 
 
-cdef class OrderBookDelta(OrderBookData):
+cdef class OrderBookDelta(Data):
+    cdef readonly InstrumentId instrument_id
+    """The instrument ID for the order book.\n\n:returns: `InstrumentId`"""
     cdef readonly BookAction action
     """The order book delta action {``ADD``, ``UPDATED``, ``DELETE``, ``CLEAR``}.\n\n:returns: `BookAction`"""
     cdef readonly BookOrder order
     """The order to apply.\n\n:returns: `Order`"""
+    cdef readonly uint64_t sequence
+    """The unique sequence number.\n\n:returns: `uint64`"""
 
     @staticmethod
     cdef OrderBookDelta from_dict_c(dict values)
 
     @staticmethod
     cdef dict to_dict_c(OrderBookDelta obj)
 
 
-cdef class BookOrder:
-    cdef readonly double price
-    """The orders price.\n\n:returns: `double`"""
-    cdef readonly double size
-    """The orders size.\n\n:returns: `double`"""
-    cdef readonly OrderSide side
-    """The orders side.\n\n:returns: `OrderSide`"""
-    cdef readonly str order_id
-    """The orders ID.\n\n:returns: `str`"""
+cdef class OrderBookDeltas(Data):
+    cdef readonly InstrumentId instrument_id
+    """The instrument ID for the order book.\n\n:returns: `InstrumentId`"""
+    cdef readonly uint64_t sequence
+    """The unique sequence number.\n\n:returns: `uint64`"""
+    cdef readonly list deltas
+    """The order book deltas.\n\n:returns: `list[OrderBookDelta]`"""
 
-    cpdef void update_price(self, double price)
-    cpdef void update_size(self, double size)
-    cpdef void update_order_id(self, str value)
-    cpdef double exposure(self)
-    cpdef double signed_size(self)
+    @staticmethod
+    cdef OrderBookDeltas from_dict_c(dict values)
 
     @staticmethod
-    cdef BookOrder from_dict_c(dict values)
+    cdef dict to_dict_c(OrderBookDeltas obj)
+
+
+cdef class OrderBookSnapshot(Data):
+    cdef readonly InstrumentId instrument_id
+    """The instrument ID for the order book.\n\n:returns: `InstrumentId`"""
+    cdef readonly uint64_t sequence
+    """The unique sequence number.\n\n:returns: `uint64`"""
+    cdef readonly list bids
+    """The snapshot bids.\n\n:returns: `list`"""
+    cdef readonly list asks
+    """The snapshot asks.\n\n:returns: `list`"""
 
     @staticmethod
-    cdef dict to_dict_c(BookOrder obj)
+    cdef OrderBookSnapshot from_dict_c(dict values)
+
+    @staticmethod
+    cdef dict to_dict_c(OrderBookSnapshot obj)
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/orderbook/data.pyx` & `nautilus_trader-1.174.0/nautilus_trader/model/data/book.pyx`

 * *Files 8% similar despite different names*

```diff
@@ -28,254 +28,347 @@
 from nautilus_trader.model.enums_c cimport book_action_to_str
 from nautilus_trader.model.enums_c cimport book_type_from_str
 from nautilus_trader.model.enums_c cimport book_type_to_str
 from nautilus_trader.model.enums_c cimport order_side_from_str
 from nautilus_trader.model.enums_c cimport order_side_to_str
 
 
-cdef class OrderBookData(Data):
+ORDER_BOOK_DATA = (OrderBookSnapshot, OrderBookDeltas, OrderBookDelta)
+
+
+cdef class BookOrder:
     """
-    The base class for all `OrderBook` data.
+    Represents an order in a book.
 
     Parameters
     ----------
-    instrument_id : InstrumentId
-        The instrument ID for the book.
-    book_type : BookType {``L1_TBBO``, ``L2_MBP``, ``L3_MBO``}
-        The order book type.
-    sequence : uint64, default 0
-        The unique sequence number for the update. If default 0 then will increment the `sequence`.
-    ts_event : uint64_t
-        The UNIX timestamp (nanoseconds) when the data event occurred.
-    ts_init : uint64_t
-        The UNIX timestamp (nanoseconds) when the data object was initialized.
-    time_in_force : TimeInForce, default ``GTC``
-        The order time in force for this update.
-
-    Warnings
-    --------
-    This class should not be used directly, but through a concrete subclass.
+    price : double
+        The order price.
+    size : double
+        The order size.
+    side : OrderSide {``BUY``, ``SELL``}
+        The order side.
+    id : str
+        The order ID.
     """
 
     def __init__(
         self,
-        InstrumentId instrument_id not None,
-        BookType book_type,
-        uint64_t sequence,
-        uint64_t ts_event,
-        uint64_t ts_init,
-        TimeInForce time_in_force = TimeInForce.GTC,
+        double price,
+        double size,
+        OrderSide side,
+        str order_id = None,
     ):
-        super().__init__(ts_event, ts_init)
+        self.price = price
+        self.size = size
+        self.side = side
+        self.order_id = order_id or str(uuid.uuid4())
 
-        self.instrument_id = instrument_id
-        self.book_type = book_type
-        self.time_in_force = time_in_force
-        self.sequence = sequence
+    def __eq__(self, BookOrder other) -> bool:
+        return self.order_id == other.order_id
+
+    def __hash__(self) -> int:
+        return hash(frozenset(BookOrder.to_dict_c(self)))
+
+    def __repr__(self) -> str:
+        return f"{BookOrder.__name__}({self.price}, {self.size}, {order_side_to_str(self.side)}, {self.order_id})"
+
+    cpdef void update_price(self, double price):
+        """
+        Update the orders price.
+
+        Parameters
+        ----------
+        price : double
+            The updated price.
+
+        """
+        self.price = price
+
+    cpdef void update_size(self, double size):
+        """
+        Update the orders size.
+
+        Parameters
+        ----------
+        size : double
+            The updated size.
+
+        """
+        self.size = size
+
+    cpdef void update_order_id(self, str value):
+        """
+        Update the orders ID.
+
+        Parameters
+        ----------
+        value : str
+            The updated order ID.
+
+        """
+        self.order_id = value
+
+    cpdef double exposure(self):
+        """
+        Return the total exposure for this order (price * size).
+
+        Returns
+        -------
+        double
+
+        """
+        return self.price * self.size
+
+    cpdef double signed_size(self):
+        """
+        Return the signed size of the order (negative for ``SELL``).
+
+        Returns
+        -------
+        double
+
+        """
+        if self.side == OrderSide.BUY:
+            return self.size * 1.0
+        else:
+            return self.size * -1.0
+
+    @staticmethod
+    cdef BookOrder from_dict_c(dict values):
+        Condition.not_none(values, "values")
+        return BookOrder(
+            price=values["price"],
+            size=values["size"],
+            side=order_side_from_str(values["side"]),
+            order_id=values["order_id"],
+        )
 
+    @staticmethod
+    cdef dict to_dict_c(BookOrder obj):
+        Condition.not_none(obj, "obj")
+        return {
+            "type": "BookOrder",
+            "price": obj.price,
+            "size": obj.size,
+            "side": order_side_to_str(obj.side),
+            "order_id": str(obj.order_id),
+        }
 
-cdef class OrderBookSnapshot(OrderBookData):
+    @staticmethod
+    def from_dict(dict values) -> BookOrder:
+        """
+        Return an order from the given dict values.
+
+        Parameters
+        ----------
+        values : dict[str, object]
+            The values for initialization.
+
+        Returns
+        -------
+        BookOrder
+
+        """
+        return BookOrder.from_dict_c(values)
+
+    @staticmethod
+    def to_dict(BookOrder obj):
+        """
+        Return a dictionary representation of this object.
+
+        Returns
+        -------
+        dict[str, object]
+
+        """
+        return BookOrder.to_dict_c(obj)
+
+
+cdef class OrderBookDelta(Data):
     """
-    Represents a snapshot in time for an `OrderBook`.
+    Represents a single difference on an `OrderBook`.
 
     Parameters
     ----------
     instrument_id : InstrumentId
         The instrument ID for the book.
-    book_type : BookType {``L1_TBBO``, ``L2_MBP``, ``L3_MBO``}
-        The order book type.
-    bids : list
-        The bids for the snapshot.
-    asks : list
-        The asks for the snapshot.
+    action : BookAction {``ADD``, ``UPDATED``, ``DELETE``, ``CLEAR``}
+        The order book delta action.
+    order : Order
+        The order to apply.
     ts_event : uint64_t
         The UNIX timestamp (nanoseconds) when the data event occurred.
     ts_init : uint64_t
         The UNIX timestamp (nanoseconds) when the data object was initialized.
     sequence : uint64, default 0
         The unique sequence number for the update. If default 0 then will increment the `sequence`.
-    time_in_force : TimeInForce, default ``GTC``
-        The order time in force for this update.
     """
 
     def __init__(
         self,
         InstrumentId instrument_id not None,
-        BookType book_type,
-        list bids not None,
-        list asks not None,
+        BookAction action,
+        BookOrder order,
         uint64_t ts_event,
         uint64_t ts_init,
         uint64_t sequence=0,
-        TimeInForce time_in_force = TimeInForce.GTC,
     ):
-        super().__init__(
-            instrument_id,
-            book_type,
-            sequence,
-            ts_event,
-            ts_init,
-            time_in_force,
-        )
+        super().__init__(ts_event, ts_init)
 
-        self.bids = bids
-        self.asks = asks
+        self.instrument_id = instrument_id
+        self.action = action
+        self.order = order
+        self.sequence = sequence
 
-    def __eq__(self, OrderBookSnapshot other) -> bool:
-        return OrderBookSnapshot.to_dict_c(self) == OrderBookSnapshot.to_dict_c(other)
+    def __eq__(self, OrderBookDelta other) -> bool:
+        return OrderBookDelta.to_dict_c(self) == OrderBookDelta.to_dict_c(other)
 
     def __hash__(self) -> int:
-        return hash(frozenset(OrderBookSnapshot.to_dict_c(self)))
+        return hash(frozenset(OrderBookDelta.to_dict_c(self)))
 
     def __repr__(self) -> str:
         return (
             f"{type(self).__name__}("
-            f"'{self.instrument_id}', "
-            f"book_type={book_type_to_str(self.book_type)}, "
-            f"bids={self.bids}, "
-            f"asks={self.asks}, "
+            f"instrument_id={self.instrument_id}, "
+            f"action={book_action_to_str(self.action)}, "
+            f"order={self.order}, "
             f"sequence={self.sequence}, "
             f"ts_event={self.ts_event}, "
             f"ts_init={self.ts_init})"
         )
 
     @staticmethod
-    cdef OrderBookSnapshot from_dict_c(dict values):
+    cdef OrderBookDelta from_dict_c(dict values):
         Condition.not_none(values, "values")
-        return OrderBookSnapshot(
+        cdef BookAction action = book_action_from_str(values["action"])
+        cdef BookOrder order = BookOrder.from_dict_c({
+            "price": values["price"],
+            "size": values["size"],
+            "side": values["side"],
+            "order_id": values["order_id"],
+        }) if values['action'] != "CLEAR" else None
+        return OrderBookDelta(
             instrument_id=InstrumentId.from_str_c(values["instrument_id"]),
-            book_type=book_type_from_str(values["book_type"]),
-            bids=msgspec.json.decode(values["bids"]),
-            asks=msgspec.json.decode(values["asks"]),
+            action=action,
+            order=order,
+            sequence=values.get("update_id", 0),
             ts_event=values["ts_event"],
             ts_init=values["ts_init"],
-            sequence=values.get("sequence", 0),
         )
 
     @staticmethod
-    cdef dict to_dict_c(OrderBookSnapshot obj):
+    cdef dict to_dict_c(OrderBookDelta obj):
         Condition.not_none(obj, "obj")
         return {
-            "type": "OrderBookSnapshot",
+            "type": "OrderBookDelta",
             "instrument_id": obj.instrument_id.to_str(),
-            "book_type": book_type_to_str(obj.book_type),
+            "action": book_action_to_str(obj.action),
+            "price": obj.order.price if obj.order else None,
+            "size": obj.order.size if obj.order else None,
+            "side": order_side_to_str(obj.order.side) if obj.order else None,
+            "order_id": obj.order.order_id if obj.order else None,
             "sequence": obj.sequence,
-            "bids": msgspec.json.encode(obj.bids),
-            "asks": msgspec.json.encode(obj.asks),
             "ts_event": obj.ts_event,
             "ts_init": obj.ts_init,
         }
 
     @staticmethod
-    def from_dict(dict values) -> OrderBookSnapshot:
+    def from_dict(dict values) -> OrderBookDelta:
         """
-        Return an order book snapshot from the given dict values.
+        Return an order book delta from the given dict values.
 
         Parameters
         ----------
         values : dict[str, object]
             The values for initialization.
 
         Returns
         -------
-        OrderBookSnapshot
+        OrderBookDelta
 
         """
-        return OrderBookSnapshot.from_dict_c(values)
+        return OrderBookDelta.from_dict_c(values)
 
     @staticmethod
-    def to_dict(OrderBookSnapshot obj):
+    def to_dict(OrderBookDelta obj):
         """
         Return a dictionary representation of this object.
 
         Returns
         -------
         dict[str, object]
 
         """
-        return OrderBookSnapshot.to_dict_c(obj)
+        return OrderBookDelta.to_dict_c(obj)
 
 
-cdef class OrderBookDeltas(OrderBookData):
+cdef class OrderBookDeltas(Data):
     """
-    Represents bulk changes for an `OrderBook`.
+    Represents bulk `OrderBookDelta` updates for an `OrderBook`.
 
     Parameters
     ----------
     instrument_id : InstrumentId
         The instrument ID for the book.
-    book_type : BookType {``L1_TBBO``, ``L2_MBP``, ``L3_MBO``}
-        The order book type.
     deltas : list[OrderBookDelta]
         The list of order book changes.
     ts_event : uint64_t
         The UNIX timestamp (nanoseconds) when the data event occurred.
     ts_init : uint64_t
         The UNIX timestamp (nanoseconds) when the data object was initialized.
-    time_in_force : TimeInForce, default ``GTC``
-        The order time in force for this update.
     """
 
     def __init__(
         self,
         InstrumentId instrument_id not None,
-        BookType book_type,
         list deltas not None,
         uint64_t ts_event,
         uint64_t ts_init,
         uint64_t sequence=0,
-        TimeInForce time_in_force = TimeInForce.GTC,
     ):
-        super().__init__(
-            instrument_id,
-            book_type,
-            sequence,
-            ts_event,
-            ts_init,
-            time_in_force,
-        )
+        super().__init__(ts_event, ts_init)
 
+        self.instrument_id = instrument_id
         self.deltas = deltas
+        self.sequence = sequence
 
     def __eq__(self, OrderBookDeltas other) -> bool:
         return OrderBookDeltas.to_dict_c(self) == OrderBookDeltas.to_dict_c(other)
 
     def __hash__(self) -> int:
         return hash(frozenset(OrderBookDeltas.to_dict_c(self)))
 
     def __repr__(self) -> str:
         return (
             f"{type(self).__name__}("
-            f"'{self.instrument_id}', "
-            f"book_type={book_type_to_str(self.book_type)}, "
+            f"instrument_id={self.instrument_id}, "
             f"{self.deltas}, "
             f"sequence={self.sequence}, "
             f"ts_event={self.ts_event}, "
             f"ts_init={self.ts_init})"
         )
 
     @staticmethod
     cdef OrderBookDeltas from_dict_c(dict values):
         Condition.not_none(values, "values")
         return OrderBookDeltas(
             instrument_id=InstrumentId.from_str_c(values["instrument_id"]),
-            book_type=book_type_from_str(values["book_type"]),
             deltas=[OrderBookDelta.from_dict_c(d) for d in msgspec.json.decode(values["deltas"])],
             ts_event=values["ts_event"],
             ts_init=values["ts_init"],
             sequence=values.get("update_id", 0),
         )
 
     @staticmethod
     cdef dict to_dict_c(OrderBookDeltas obj):
         Condition.not_none(obj, "obj")
         return {
             "type": "OrderBookDeltas",
             "instrument_id": obj.instrument_id.to_str(),
-            "book_type": book_type_to_str(obj.book_type),
             "deltas": msgspec.json.encode([OrderBookDelta.to_dict_c(d) for d in obj.deltas]),
             "sequence": obj.sequence,
             "ts_event": obj.ts_event,
             "ts_init": obj.ts_init,
         }
 
     @staticmethod
@@ -304,286 +397,113 @@
         -------
         dict[str, object]
 
         """
         return OrderBookDeltas.to_dict_c(obj)
 
 
-cdef class OrderBookDelta(OrderBookData):
+cdef class OrderBookSnapshot(Data):
     """
-    Represents a single difference on an `OrderBook`.
+    Represents a snapshot in time for an `OrderBook`.
 
     Parameters
     ----------
     instrument_id : InstrumentId
         The instrument ID for the book.
-    book_type : BookType {``L1_TBBO``, ``L2_MBP``, ``L3_MBO``}
-        The order book type.
-    action : BookAction {``ADD``, ``UPDATED``, ``DELETE``, ``CLEAR``}
-        The order book delta action.
-    order : Order
-        The order to apply.
+    bids : list
+        The bids for the snapshot.
+    asks : list
+        The asks for the snapshot.
     ts_event : uint64_t
         The UNIX timestamp (nanoseconds) when the data event occurred.
     ts_init : uint64_t
         The UNIX timestamp (nanoseconds) when the data object was initialized.
     sequence : uint64, default 0
         The unique sequence number for the update. If default 0 then will increment the `sequence`.
-    time_in_force : TimeInForce, default ``GTC``
-        The order time in force for this update.
     """
 
     def __init__(
         self,
         InstrumentId instrument_id not None,
-        BookType book_type,
-        BookAction action,
-        BookOrder order,
+        list bids not None,
+        list asks not None,
         uint64_t ts_event,
         uint64_t ts_init,
         uint64_t sequence=0,
-        TimeInForce time_in_force = TimeInForce.GTC,
     ):
-        super().__init__(
-            instrument_id,
-            book_type,
-            sequence,
-            ts_event,
-            ts_init,
-            time_in_force,
-        )
+        super().__init__(ts_event, ts_init)
 
-        self.action = action
-        self.order = order
+        self.instrument_id = instrument_id
+        self.bids = bids
+        self.asks = asks
+        self.sequence = sequence
 
-    def __eq__(self, OrderBookDelta other) -> bool:
-        return OrderBookDelta.to_dict_c(self) == OrderBookDelta.to_dict_c(other)
+    def __eq__(self, OrderBookSnapshot other) -> bool:
+        return OrderBookSnapshot.to_dict_c(self) == OrderBookSnapshot.to_dict_c(other)
 
     def __hash__(self) -> int:
-        return hash(frozenset(OrderBookDelta.to_dict_c(self)))
+        return hash(frozenset(OrderBookSnapshot.to_dict_c(self)))
 
     def __repr__(self) -> str:
         return (
             f"{type(self).__name__}("
-            f"'{self.instrument_id}', "
-            f"book_type={book_type_to_str(self.book_type)}, "
-            f"action={book_action_to_str(self.action)}, "
-            f"order={self.order}, "
+            f"instrument_id={self.instrument_id}, "
+            f"bids={self.bids}, "
+            f"asks={self.asks}, "
             f"sequence={self.sequence}, "
             f"ts_event={self.ts_event}, "
             f"ts_init={self.ts_init})"
         )
 
     @staticmethod
-    cdef OrderBookDelta from_dict_c(dict values):
+    cdef OrderBookSnapshot from_dict_c(dict values):
         Condition.not_none(values, "values")
-        cdef BookAction action = book_action_from_str(values["action"])
-        cdef BookOrder order = BookOrder.from_dict_c({
-            "price": values["price"],
-            "size": values["size"],
-            "side": values["side"],
-            "order_id": values["order_id"],
-        }) if values['action'] != "CLEAR" else None
-        return OrderBookDelta(
+        return OrderBookSnapshot(
             instrument_id=InstrumentId.from_str_c(values["instrument_id"]),
-            book_type=book_type_from_str(values["book_type"]),
-            action=action,
-            order=order,
+            bids=msgspec.json.decode(values["bids"]),
+            asks=msgspec.json.decode(values["asks"]),
             ts_event=values["ts_event"],
             ts_init=values["ts_init"],
-            sequence=values.get("update_id", 0),
+            sequence=values.get("sequence", 0),
         )
 
     @staticmethod
-    cdef dict to_dict_c(OrderBookDelta obj):
+    cdef dict to_dict_c(OrderBookSnapshot obj):
         Condition.not_none(obj, "obj")
         return {
-            "type": "OrderBookDelta",
+            "type": "OrderBookSnapshot",
             "instrument_id": obj.instrument_id.to_str(),
-            "book_type": book_type_to_str(obj.book_type),
-            "action": book_action_to_str(obj.action),
-            "price": obj.order.price if obj.order else None,
-            "size": obj.order.size if obj.order else None,
-            "side": order_side_to_str(obj.order.side) if obj.order else None,
-            "order_id": obj.order.order_id if obj.order else None,
             "sequence": obj.sequence,
+            "bids": msgspec.json.encode(obj.bids),
+            "asks": msgspec.json.encode(obj.asks),
             "ts_event": obj.ts_event,
             "ts_init": obj.ts_init,
         }
 
     @staticmethod
-    def from_dict(dict values) -> OrderBookDelta:
-        """
-        Return an order book delta from the given dict values.
-
-        Parameters
-        ----------
-        values : dict[str, object]
-            The values for initialization.
-
-        Returns
-        -------
-        OrderBookDelta
-
-        """
-        return OrderBookDelta.from_dict_c(values)
-
-    @staticmethod
-    def to_dict(OrderBookDelta obj):
-        """
-        Return a dictionary representation of this object.
-
-        Returns
-        -------
-        dict[str, object]
-
-        """
-        return OrderBookDelta.to_dict_c(obj)
-
-
-cdef class BookOrder:
-    """
-    Represents an order in a book.
-
-    Parameters
-    ----------
-    price : double
-        The order price.
-    size : double
-        The order size.
-    side : OrderSide {``BUY``, ``SELL``}
-        The order side.
-    id : str
-        The order ID.
-    """
-
-    def __init__(
-        self,
-        double price,
-        double size,
-        OrderSide side,
-        str order_id = None,
-    ):
-        self.price = price
-        self.size = size
-        self.side = side
-        self.order_id = order_id or str(uuid.uuid4())
-
-    def __eq__(self, BookOrder other) -> bool:
-        return self.order_id == other.order_id
-
-    def __hash__(self) -> int:
-        return hash(frozenset(BookOrder.to_dict_c(self)))
-
-    def __repr__(self) -> str:
-        return f"{BookOrder.__name__}({self.price}, {self.size}, {order_side_to_str(self.side)}, {self.order_id})"
-
-    cpdef void update_price(self, double price):
-        """
-        Update the orders price.
-
-        Parameters
-        ----------
-        price : double
-            The updated price.
-
-        """
-        self.price = price
-
-    cpdef void update_size(self, double size):
-        """
-        Update the orders size.
-
-        Parameters
-        ----------
-        size : double
-            The updated size.
-
-        """
-        self.size = size
-
-    cpdef void update_order_id(self, str value):
-        """
-        Update the orders ID.
-
-        Parameters
-        ----------
-        value : str
-            The updated order ID.
-
-        """
-        self.order_id = value
-
-    cpdef double exposure(self):
-        """
-        Return the total exposure for this order (price * size).
-
-        Returns
-        -------
-        double
-
-        """
-        return self.price * self.size
-
-    cpdef double signed_size(self):
-        """
-        Return the signed size of the order (negative for ``SELL``).
-
-        Returns
-        -------
-        double
-
-        """
-        if self.side == OrderSide.BUY:
-            return self.size * 1.0
-        else:
-            return self.size * -1.0
-
-    @staticmethod
-    cdef BookOrder from_dict_c(dict values):
-        Condition.not_none(values, "values")
-        return BookOrder(
-            price=values["price"],
-            size=values["size"],
-            side=order_side_from_str(values["side"]),
-            order_id=values["order_id"],
-        )
-
-    @staticmethod
-    cdef dict to_dict_c(BookOrder obj):
-        Condition.not_none(obj, "obj")
-        return {
-            "type": "BookOrder",
-            "price": obj.price,
-            "size": obj.size,
-            "side": order_side_to_str(obj.side),
-            "order_id": str(obj.order_id),
-        }
-
-    @staticmethod
-    def from_dict(dict values) -> BookOrder:
+    def from_dict(dict values) -> OrderBookSnapshot:
         """
-        Return an order from the given dict values.
+        Return an order book snapshot from the given dict values.
 
         Parameters
         ----------
         values : dict[str, object]
             The values for initialization.
 
         Returns
         -------
-        BookOrder
+        OrderBookSnapshot
 
         """
-        return BookOrder.from_dict_c(values)
+        return OrderBookSnapshot.from_dict_c(values)
 
     @staticmethod
-    def to_dict(BookOrder obj):
+    def to_dict(OrderBookSnapshot obj):
         """
         Return a dictionary representation of this object.
 
         Returns
         -------
         dict[str, object]
 
         """
-        return BookOrder.to_dict_c(obj)
+        return OrderBookSnapshot.to_dict_c(obj)
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/orderbook/error.py` & `nautilus_trader-1.174.0/nautilus_trader/network/error.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,13 +10,11 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 # -------------------------------------------------------------------------------------------------
 
 
-class BookIntegrityError(Exception):
+class MaxRetriesExceeded(ConnectionError):
     """
-    Represents an error condition where the order books integrity has been lost.
+    Represents an error where the maximum number of connection retries has been exceeded.
     """
-
-    pass
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/orderbook/ladder.pxd` & `nautilus_trader-1.174.0/nautilus_trader/model/orderbook/ladder.pxd`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 #  limitations under the License.
 # -------------------------------------------------------------------------------------------------
 
 import cython
 
 from libc.stdint cimport uint8_t
 
+from nautilus_trader.model.data.book cimport BookOrder
 from nautilus_trader.model.enums_c cimport DepthType
-from nautilus_trader.model.orderbook.data cimport BookOrder
 from nautilus_trader.model.orderbook.level cimport Level
 
 
 cdef class Ladder:
     cdef dict _order_id_level_index
 
     cdef readonly list levels
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/orderbook/ladder.pyx` & `nautilus_trader-1.174.0/nautilus_trader/model/orderbook/ladder.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 # -------------------------------------------------------------------------------------------------
 
 from libc.stdint cimport uint8_t
 
 from nautilus_trader.core.correctness cimport Condition
+from nautilus_trader.model.data.book cimport BookOrder
 from nautilus_trader.model.enums_c cimport DepthType
 from nautilus_trader.model.objects cimport Price
 from nautilus_trader.model.objects cimport Quantity
-from nautilus_trader.model.orderbook.data cimport BookOrder
 from nautilus_trader.model.orderbook.level cimport Level
 
 
 cdef class Ladder:
     """
     Represents a ladder of price levels in a book.
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/orderbook/level.pxd` & `nautilus_trader-1.174.0/nautilus_trader/model/orderbook/level.pxd`

 * *Files 15% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 # -------------------------------------------------------------------------------------------------
 
-from nautilus_trader.model.orderbook.data cimport BookOrder
+from nautilus_trader.model.data.book cimport BookOrder
 
 
 cdef class Level:
     cdef readonly double price
     """The levels price.\n\n:returns: `double`"""
     cdef readonly list orders
     """The orders at the level.\n\n:returns: `list[Order]`"""
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/orderbook/level.pyx` & `nautilus_trader-1.174.0/nautilus_trader/model/orderbook/level.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 # -------------------------------------------------------------------------------------------------
 
 from nautilus_trader.core.correctness cimport Condition
-from nautilus_trader.model.orderbook.data cimport BookOrder
+from nautilus_trader.model.data.book cimport BookOrder
 
 
 cdef class Level:
     """
     Represents an `OrderBook` level.
 
     A price level on one side of the `OrderBook` with one or more individual orders.
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/orderbook/simulated.pxd` & `nautilus_trader-1.174.0/nautilus_trader/model/orderbook/simulated.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/orderbook/simulated.pyx` & `nautilus_trader-1.174.0/nautilus_trader/model/orderbook/simulated.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -13,22 +13,22 @@
 #  limitations under the License.
 # -------------------------------------------------------------------------------------------------
 
 from libc.stdint cimport uint8_t
 from libc.stdint cimport uint64_t
 
 from nautilus_trader.core.rust.model cimport FIXED_SCALAR
+from nautilus_trader.model.data.book cimport BookOrder
 from nautilus_trader.model.data.tick cimport QuoteTick
 from nautilus_trader.model.data.tick cimport TradeTick
 from nautilus_trader.model.enums_c cimport OrderSide
 from nautilus_trader.model.identifiers cimport InstrumentId
 from nautilus_trader.model.orderbook.book cimport L1OrderBook
 from nautilus_trader.model.orderbook.book cimport L2OrderBook
 from nautilus_trader.model.orderbook.book cimport L3OrderBook
-from nautilus_trader.model.orderbook.data cimport BookOrder
 
 
 cdef class SimulatedL1OrderBook(L1OrderBook):
     """
     Provides a simulated level 1 order book for backtesting.
 
     Parameters
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/orders/__init__.pxd` & `nautilus_trader-1.174.0/nautilus_trader/model/tick_scheme/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/orders/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/model/orders/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/orders/base.pxd` & `nautilus_trader-1.174.0/nautilus_trader/model/orders/base.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/orders/base.pyx` & `nautilus_trader-1.174.0/nautilus_trader/model/orders/base.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/orders/limit.pxd` & `nautilus_trader-1.174.0/nautilus_trader/model/orders/limit.pxd`

 * *Files 2% similar despite different names*

```diff
@@ -29,8 +29,8 @@
     cdef readonly Quantity display_qty
     """The quantity of the order to display on the public book (iceberg).\n\n:returns: `Quantity` or ``None``"""
 
     @staticmethod
     cdef LimitOrder create(OrderInitialized init)
 
     @staticmethod
-    cdef LimitOrder transform(Order order, uint64_t ts_init)
+    cdef LimitOrder transform(Order order, uint64_t ts_init, Price price=*)
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/orders/limit.pyx` & `nautilus_trader-1.174.0/nautilus_trader/model/orders/limit.pyx`

 * *Files 3% similar despite different names*

```diff
@@ -343,50 +343,58 @@
             exec_algorithm_id=init.exec_algorithm_id,
             exec_algorithm_params=init.exec_algorithm_params,
             exec_spawn_id=init.exec_spawn_id,
             tags=init.tags,
         )
 
     @staticmethod
-    cdef LimitOrder transform(Order order, uint64_t ts_init):
+    cdef LimitOrder transform(Order order, uint64_t ts_init, Price price = None):
         """
         Transform the given order to a `limit` order.
 
         All existing events will be prepended to the orders internal events
         prior to the new `OrderInitialized` event.
 
         Parameters
         ----------
         order : Order
             The order to transform from.
         ts_init : uint64_t
             The UNIX timestamp (nanoseconds) when the object was initialized.
+        price : Price, optional
+            The price to assign to the order (will override any existing price on `order`).
 
         Returns
         -------
         LimitOrder
 
+        Raises
+        ------
+        ValueError
+            If `price` is ``None`` and `order` does not have a `price` attribute.
+
         """
         Condition.not_none(order, "order")
+        Condition.true(price or hasattr(order, "price"), "`order` has no price")
 
         cdef LimitOrder transformed = LimitOrder(
             trader_id=order.trader_id,
             strategy_id=order.strategy_id,
             instrument_id=order.instrument_id,
             client_order_id=order.client_order_id,
             order_side=order.side,
             quantity=order.quantity,
-            price=order.price,
+            price=price or order.price,
             time_in_force=order.time_in_force,
-            expire_time_ns=order.expire_time_ns,
+            expire_time_ns=order.expire_time_ns if hasattr(order, "expire_time_ns") else 0,
             init_id=UUID4(),
             ts_init=ts_init,
-            post_only=order.is_post_only,
+            post_only=order.is_post_only if hasattr(order, "is_post_only") else False,
             reduce_only=order.is_reduce_only,
-            display_qty=order.display_qty,
+            display_qty=order.display_qty if hasattr(order, "display_qty") else None,
             contingency_type=order.contingency_type,
             order_list_id=order.order_list_id,
             linked_order_ids=order.linked_order_ids,
             parent_order_id=order.parent_order_id,
             exec_algorithm_id=order.exec_algorithm_id,
             exec_algorithm_params=order.exec_algorithm_params,
             exec_spawn_id=order.exec_spawn_id,
@@ -398,9 +406,9 @@
             transformed.set_triggered_price_c(triggered_price)
 
         Order._hydrate_initial_events(original=order, transformed=transformed)
 
         return transformed
 
     @staticmethod
-    def transform_py(Order order, uint64_t ts_init) -> LimitOrder:
-        return LimitOrder.transform(order, ts_init)
+    def transform_py(Order order, uint64_t ts_init, Price price = None) -> LimitOrder:
+        return LimitOrder.transform(order, ts_init, price)
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/orders/limit_if_touched.pxd` & `nautilus_trader-1.174.0/nautilus_trader/model/orders/limit_if_touched.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/orders/limit_if_touched.pyx` & `nautilus_trader-1.174.0/nautilus_trader/model/orders/limit_if_touched.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/orders/list.pxd` & `nautilus_trader-1.174.0/nautilus_trader/model/orders/list.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/orders/list.pyx` & `nautilus_trader-1.174.0/nautilus_trader/model/orders/list.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/orders/market.pxd` & `nautilus_trader-1.174.0/nautilus_trader/model/orders/market.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/orders/market.pyx` & `nautilus_trader-1.174.0/nautilus_trader/model/orders/market.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/orders/market_if_touched.pxd` & `nautilus_trader-1.174.0/nautilus_trader/model/orders/market_if_touched.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/orders/market_if_touched.pyx` & `nautilus_trader-1.174.0/nautilus_trader/model/orders/market_if_touched.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/orders/market_to_limit.pxd` & `nautilus_trader-1.174.0/nautilus_trader/model/orders/market_to_limit.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/orders/market_to_limit.pyx` & `nautilus_trader-1.174.0/nautilus_trader/model/orders/market_to_limit.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/orders/stop_limit.pxd` & `nautilus_trader-1.174.0/nautilus_trader/model/orders/stop_limit.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/orders/stop_limit.pyx` & `nautilus_trader-1.174.0/nautilus_trader/model/orders/stop_limit.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/orders/stop_market.pxd` & `nautilus_trader-1.174.0/nautilus_trader/model/orders/stop_market.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/orders/stop_market.pyx` & `nautilus_trader-1.174.0/nautilus_trader/model/orders/stop_market.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/orders/trailing_stop_limit.pxd` & `nautilus_trader-1.174.0/nautilus_trader/model/orders/trailing_stop_limit.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/orders/trailing_stop_limit.pyx` & `nautilus_trader-1.174.0/nautilus_trader/model/orders/trailing_stop_limit.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/orders/trailing_stop_market.pxd` & `nautilus_trader-1.174.0/nautilus_trader/model/orders/trailing_stop_market.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/orders/trailing_stop_market.pyx` & `nautilus_trader-1.174.0/nautilus_trader/model/orders/trailing_stop_market.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/orders/unpacker.pxd` & `nautilus_trader-1.174.0/nautilus_trader/model/orders/unpacker.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/orders/unpacker.pyx` & `nautilus_trader-1.174.0/nautilus_trader/model/orders/unpacker.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/position.pxd` & `nautilus_trader-1.174.0/nautilus_trader/model/position.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/position.pyx` & `nautilus_trader-1.174.0/nautilus_trader/model/position.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/tick_scheme/__init__.pxd` & `nautilus_trader-1.174.0/nautilus_trader/msgbus/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/tick_scheme/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/model/tick_scheme/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,11 +12,11 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 # -------------------------------------------------------------------------------------------------
 
 """Defines a scheme for modeling the tick space for various instruments."""
 
 # Required to register tick schemes
-from nautilus_trader.model.tick_scheme.base import get_tick_scheme  # noqa: F401, F403
-from nautilus_trader.model.tick_scheme.base import list_tick_schemes  # noqa: F401, F403
-from nautilus_trader.model.tick_scheme.base import register_tick_scheme  # noqa: F401, F403
-from nautilus_trader.model.tick_scheme.implementations import *  # noqa: F401, F403
+from nautilus_trader.model.tick_scheme.base import get_tick_scheme  # noqa: F401
+from nautilus_trader.model.tick_scheme.base import list_tick_schemes  # noqa: F401
+from nautilus_trader.model.tick_scheme.base import register_tick_scheme  # noqa: F401
+from nautilus_trader.model.tick_scheme.implementations import *  # noqa: F403
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/tick_scheme/base.pxd` & `nautilus_trader-1.174.0/nautilus_trader/model/tick_scheme/base.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/tick_scheme/base.pyx` & `nautilus_trader-1.174.0/nautilus_trader/model/tick_scheme/base.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/tick_scheme/implementations/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/test_kit/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,14 +9,11 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 # -------------------------------------------------------------------------------------------------
 
-# Required to register tick schemes
-from nautilus_trader.model.tick_scheme.implementations.fixed import (  # noqa: F401
-    FOREX_3DECIMAL_TICK_SCHEME,
-)
-from nautilus_trader.model.tick_scheme.implementations.fixed import (  # noqa: F401
-    FOREX_5DECIMAL_TICK_SCHEME,
-)
+"""
+The test kit contains test doubles and helpers to support the NautilusTrader
+test suite, as well as supporting testing for downstream projects and packages.
+"""
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/tick_scheme/implementations/fixed.pxd` & `nautilus_trader-1.174.0/nautilus_trader/model/tick_scheme/implementations/fixed.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/tick_scheme/implementations/fixed.pyx` & `nautilus_trader-1.174.0/nautilus_trader/model/tick_scheme/implementations/fixed.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/tick_scheme/implementations/tiered.pxd` & `nautilus_trader-1.174.0/nautilus_trader/model/tick_scheme/implementations/tiered.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/model/tick_scheme/implementations/tiered.pyx` & `nautilus_trader-1.174.0/nautilus_trader/model/tick_scheme/implementations/tiered.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/msgbus/__init__.pxd` & `nautilus_trader-1.174.0/nautilus_trader/network/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/msgbus/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/msgbus/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/msgbus/bus.pxd` & `nautilus_trader-1.174.0/nautilus_trader/msgbus/bus.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/msgbus/bus.pyx` & `nautilus_trader-1.174.0/nautilus_trader/msgbus/bus.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/msgbus/subscription.pxd` & `nautilus_trader-1.174.0/nautilus_trader/msgbus/subscription.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/msgbus/subscription.pyx` & `nautilus_trader-1.174.0/nautilus_trader/msgbus/subscription.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/network/__init__.pxd` & `nautilus_trader-1.174.0/nautilus_trader/persistence/external/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/network/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/network/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/network/error.py` & `nautilus_trader-1.174.0/nautilus_trader/persistence/catalog/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,12 +9,15 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 # -------------------------------------------------------------------------------------------------
 
+from nautilus_trader.persistence.catalog.base import BaseDataCatalog
+from nautilus_trader.persistence.catalog.parquet import ParquetDataCatalog
 
-class MaxRetriesExceeded(ConnectionError):
-    """
-    Represents an error where the maximum number of connection retries has been exceeded.
-    """
+
+__all__ = (
+    "BaseDataCatalog",
+    "ParquetDataCatalog",
+)
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/network/http.pxd` & `nautilus_trader-1.174.0/nautilus_trader/network/http.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/network/http.pyx` & `nautilus_trader-1.174.0/nautilus_trader/network/http.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/network/socket.pxd` & `nautilus_trader-1.174.0/nautilus_trader/network/socket.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/network/socket.pyx` & `nautilus_trader-1.174.0/nautilus_trader/network/socket.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/network/websocket.pxd` & `nautilus_trader-1.174.0/nautilus_trader/network/websocket.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/network/websocket.pyx` & `nautilus_trader-1.174.0/nautilus_trader/network/websocket.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/persistence/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/portfolio/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 # -------------------------------------------------------------------------------------------------
 
-"""The `persistence` subpackage handles data storage and retrieval, mainly to support backtesting."""  # noqa
+"""The `portfolio` subpackage provides portfolio management functionality."""
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/persistence/catalog/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/serialization/arrow/implementations/instruments.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,15 +9,13 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 # -------------------------------------------------------------------------------------------------
 
-from nautilus_trader.persistence.catalog.base import BaseDataCatalog
-from nautilus_trader.persistence.catalog.parquet import ParquetDataCatalog
+from nautilus_trader.model.instruments import Instrument
+from nautilus_trader.serialization.arrow.serializer import register_parquet
 
 
-__all__ = (
-    "BaseDataCatalog",
-    "ParquetDataCatalog",
-)
+for cls in Instrument.__subclasses__():
+    register_parquet(cls, partition_keys=())
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/persistence/catalog/base.py` & `nautilus_trader-1.174.0/nautilus_trader/persistence/catalog/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,26 +17,26 @@
 from abc import ABCMeta
 from abc import abstractmethod
 from typing import Optional
 
 from nautilus_trader.model.data.bar import Bar
 from nautilus_trader.model.data.base import DataType
 from nautilus_trader.model.data.base import GenericData
+from nautilus_trader.model.data.book import OrderBookDelta
 from nautilus_trader.model.data.tick import QuoteTick
 from nautilus_trader.model.data.tick import TradeTick
 from nautilus_trader.model.data.ticker import Ticker
 from nautilus_trader.model.data.venue import InstrumentClose
 from nautilus_trader.model.data.venue import InstrumentStatusUpdate
 from nautilus_trader.model.instruments import Instrument
-from nautilus_trader.model.orderbook.data import OrderBookData
 from nautilus_trader.persistence.external.util import Singleton
 from nautilus_trader.serialization.arrow.util import GENERIC_DATA_PREFIX
 
 
-class _CombinedMeta(Singleton, ABCMeta):  # noqa
+class _CombinedMeta(Singleton, ABCMeta):
     pass
 
 
 class BaseDataCatalog(ABC, metaclass=_CombinedMeta):
     """
     Provides a abstract base class for a queryable data catalog.
     """
@@ -161,15 +161,15 @@
 
     def order_book_deltas(
         self,
         instrument_ids: Optional[list[str]] = None,
         **kwargs,
     ):
         return self.query(
-            cls=OrderBookData,
+            cls=OrderBookDelta,
             instrument_ids=instrument_ids,
             **kwargs,
         )
 
     def generic_data(
         self,
         cls: type,
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/persistence/catalog/parquet.py` & `nautilus_trader-1.174.0/nautilus_trader/persistence/catalog/parquet.py`

 * *Files 2% similar despite different names*

```diff
@@ -283,18 +283,19 @@
     def _get_files(
         self,
         cls: type,
         instrument_id: Optional[str] = None,
         start_nanos: Optional[int] = None,
         end_nanos: Optional[int] = None,
     ) -> list[str]:
-        if instrument_id is None:
-            folder = self.path
-        else:
-            folder = self.make_path(cls=cls, instrument_id=instrument_id)
+        folder = (
+            self.path
+            if instrument_id is None
+            else self.make_path(cls=cls, instrument_id=instrument_id)
+        )
 
         if not os.path.exists(folder):
             return []
 
         paths = self.fs.glob(f"{folder}/**")
 
         files = []
@@ -361,15 +362,15 @@
         self,
         base_cls: type,
         instrument_ids: Optional[list[str]] = None,
         filter_expr: Optional[Callable] = None,
         as_nautilus: bool = False,
         **kwargs,
     ):
-        subclasses = [base_cls] + base_cls.__subclasses__()
+        subclasses = [base_cls, *base_cls.__subclasses__()]
 
         dfs = []
         for cls in subclasses:
             try:
                 df = self.query(
                     cls=cls,
                     filter_expr=filter_expr,
@@ -435,18 +436,19 @@
     def list_partitions(self, cls_type: type):
         assert isinstance(cls_type, type), "`cls_type` should be type, i.e. TradeTick"
         name = class_to_filename(cls_type)
         dataset = pq.ParquetDataset(
             f"{self.path}/data/{name}.parquet",
             filesystem=self.fs,
         )
-        partitions = {}
-        for level in dataset.partitions.levels:
-            partitions[level.name] = level.keys
-        return partitions
+        # TODO(cs): Catalog v1 impl below
+        # partitions = {}
+        # for level in dataset.partitioning:
+        #     partitions[level.name] = level.keys
+        return dataset.partitioning
 
     def list_backtests(self) -> list[str]:
         glob_path = f"{self.path}/backtest/*.feather"
         return [p.stem for p in map(Path, self.fs.glob(glob_path))]
 
     def list_live_runs(self) -> list[str]:
         glob_path = f"{self.path}/live/*.feather"
@@ -459,15 +461,15 @@
         return self._read_feather(kind="backtest", run_id=backtest_run_id, **kwargs)
 
     def _read_feather(self, kind: str, run_id: str, raise_on_failed_deserialize: bool = False):
         class_mapping: dict[str, type] = {class_to_filename(cls): cls for cls in list_schemas()}
         data = {}
         glob_path = f"{self.path}/{kind}/{run_id}.feather/*.feather"
 
-        for path in [p for p in self.fs.glob(glob_path)]:
+        for path in list(self.fs.glob(glob_path)):
             cls_name = camel_to_snake_case(pathlib.Path(path).stem).replace("__", "_")
             df = read_feather_file(path=path, fs=self.fs)
 
             if df is None:
                 print(f"No data for {cls_name}")
                 continue
             # Apply post read fixes
@@ -478,15 +480,15 @@
                     mappings={},
                 )
                 data[cls_name] = objs
             except Exception as e:
                 if raise_on_failed_deserialize:
                     raise
                 print(f"Failed to deserialize {cls_name}: {e}")
-        return sorted(sum(data.values(), list()), key=lambda x: x.ts_init)
+        return sorted(sum(data.values(), []), key=lambda x: x.ts_init)
 
 
 def read_feather_file(path: str, fs: fsspec.AbstractFileSystem = None):
     fs = fs or fsspec.filesystem("file")
     if not fs.exists(path):
         return
     try:
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/persistence/external/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/persistence/streaming/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/persistence/external/core.py` & `nautilus_trader-1.174.0/nautilus_trader/persistence/external/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,15 @@
 def make_raw_files(glob_path, block_size="128mb", compression="infer", **kw) -> list[RawFile]:
     files = scan_files(glob_path, compression=compression, **kw)
     return [RawFile(open_file=f, block_size=parse_bytes(block_size)) for f in files]
 
 
 def scan_files(glob_path, compression="infer", **kw) -> list[OpenFile]:
     open_files = fsspec.open_files(glob_path, compression=compression, **kw)
-    return [of for of in open_files]
+    return list(open_files)
 
 
 def split_and_serialize(objs: list) -> dict[type, dict[Optional[str], list]]:
     """
     Given a list of Nautilus `objs`; serialize and split into dictionaries per type / instrument ID.
     """
     # Split objects into their respective tables
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/persistence/external/metadata.py` & `nautilus_trader-1.174.0/nautilus_trader/persistence/external/metadata.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/persistence/external/readers.py` & `nautilus_trader-1.174.0/nautilus_trader/persistence/external/readers.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/persistence/external/util.py` & `nautilus_trader-1.174.0/nautilus_trader/persistence/external/util.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/persistence/funcs.py` & `nautilus_trader-1.174.0/nautilus_trader/persistence/funcs.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/persistence/loaders.py` & `nautilus_trader-1.174.0/nautilus_trader/persistence/loaders.py`

 * *Files 3% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         """
         df = pd.read_csv(
             file_path,
             index_col="local_timestamp",
             date_parser=_ts_parser,
             parse_dates=True,
         )
-        df.rename(columns={"id": "trade_id", "amount": "quantity"}, inplace=True)
+        df = df.rename(columns={"id": "trade_id", "amount": "quantity"})
         df["side"] = df.side.str.upper()
         df = df[["symbol", "trade_id", "price", "quantity", "side"]]
 
         return df
 
 
 class TardisQuoteDataLoader:
@@ -131,22 +131,21 @@
         """
         df = pd.read_csv(
             file_path,
             index_col="local_timestamp",
             date_parser=_ts_parser,
             parse_dates=True,
         )
-        df.rename(
+        df = df.rename(
             columns={
                 "ask_amount": "ask_size",
                 "ask_price": "ask",
                 "bid_price": "bid",
                 "bid_amount": "bid_size",
             },
-            inplace=True,
         )
 
         return df[["bid", "ask", "bid_size", "ask_size"]]
 
 
 class ParquetTickDataLoader:
     """
@@ -166,15 +165,15 @@
             Name of the timestamp column in the parquet data
         Returns
         -------
         pd.DataFrame
 
         """
         df = pd.read_parquet(file_path)
-        df.set_index(timestamp_column, inplace=True)
+        df = df.set_index(timestamp_column)
         return df
 
 
 class ParquetBarDataLoader:
     """
     Provides a means of loading bar data pandas DataFrames from parquet files.
     """
@@ -191,9 +190,9 @@
 
         Returns
         -------
         pd.DataFrame
 
         """
         df = pd.read_parquet(file_path)
-        df.set_index("timestamp", inplace=True)
+        df = df.set_index("timestamp")
         return df
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/persistence/migrate.py` & `nautilus_trader-1.174.0/nautilus_trader/persistence/migrate.py`

 * *Files 11% similar despite different names*

```diff
@@ -34,8 +34,7 @@
 
 
 write_objects = create_temp_table(write_objects)
 
 
 def migrate(catalog: BaseDataCatalog, version_from: str, version_to: str):
     """Migrate the `catalog` between versions `version_from` and `version_to`"""
-    pass
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/persistence/streaming/batching.py` & `nautilus_trader-1.174.0/nautilus_trader/persistence/streaming/batching.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/persistence/streaming/engine.py` & `nautilus_trader-1.174.0/nautilus_trader/persistence/streaming/engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
     """
     Streams merged batches of nautilus objects from _StreamingBuffer objects.
     """
 
     def __init__(
         self,
         buffers: list[_StreamingBuffer],
-        target_batch_size_bytes: int = parse_bytes("100mb"),  # noqa: B008,
+        target_batch_size_bytes: int = parse_bytes("100mb"),  # ,
     ):
         self._buffers = buffers
         self._target_batch_size_bytes = target_batch_size_bytes
 
     def __iter__(self) -> Generator[list[Data], None, None]:
         yield from self._iterate_batches_to_target_memory()
 
@@ -141,26 +141,26 @@
 
     def _remove_completed(self) -> None:
         self._buffers = [b for b in self._buffers if not b.is_complete]
 
 
 class StreamingEngine(_BufferIterator):
     """
-    Streams merged batches of nautilus objects from BacktestDataConfig objects.
+    Streams merged batches of Nautilus objects from `BacktestDataConfig` objects.
     """
 
     def __init__(
         self,
         data_configs: list[BacktestDataConfig],
-        target_batch_size_bytes: int = parse_bytes("100mb"),  # noqa: B008,
+        target_batch_size_bytes: int = parse_bytes("512mb"),  # ,
     ):
         # Sort configs (larger time_aggregated bar specifications first)
         # Define the order of objects with the same timestamp.
         # Larger bar aggregations first. H4 > H1
-        def _sort_larger_specifications_first(config) -> tuple[int, int]:
+        def _sort_larger_specifications_first(config: BacktestDataConfig) -> tuple[int, int]:
             if config.bar_spec is None:
                 return sys.maxsize, sys.maxsize  # last
             else:
                 spec = BarSpecification.from_str(config.bar_spec)
                 return spec.aggregation * -1, spec.step * -1
 
         self._configs = sorted(data_configs, key=_sort_larger_specifications_first)
@@ -180,15 +180,18 @@
         files = config.catalog().get_files(
             cls=config.data_type,
             instrument_id=config.instrument_id,
             start_nanos=config.start_time_nanos,
             end_nanos=config.end_time_nanos,
             bar_spec=BarSpecification.from_str(config.bar_spec) if config.bar_spec else None,
         )
+
         assert files, f"No files found for {config}"
+        assert config.batch_size is not None
+
         if config.use_rust:
             batches = generate_batches_rust(
                 files=files,
                 cls=config.data_type,
                 batch_size=config.batch_size,
                 start_nanos=config.start_time_nanos,
                 end_nanos=config.end_time_nanos,
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/persistence/streaming/writer.py` & `nautilus_trader-1.174.0/nautilus_trader/persistence/streaming/writer.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,18 +6,17 @@
 from pyarrow import RecordBatchStreamWriter
 
 from nautilus_trader.common.logging import LoggerAdapter
 from nautilus_trader.core.correctness import PyCondition
 from nautilus_trader.core.data import Data
 from nautilus_trader.core.inspect import is_nautilus_class
 from nautilus_trader.model.data.base import GenericData
-from nautilus_trader.model.orderbook.data import OrderBookData
-from nautilus_trader.model.orderbook.data import OrderBookDelta
-from nautilus_trader.model.orderbook.data import OrderBookDeltas
-from nautilus_trader.model.orderbook.data import OrderBookSnapshot
+from nautilus_trader.model.data.book import OrderBookDelta
+from nautilus_trader.model.data.book import OrderBookDeltas
+from nautilus_trader.model.data.book import OrderBookSnapshot
 from nautilus_trader.serialization.arrow.serializer import ParquetSerializer
 from nautilus_trader.serialization.arrow.serializer import get_cls_table
 from nautilus_trader.serialization.arrow.serializer import list_schemas
 from nautilus_trader.serialization.arrow.serializer import register_parquet
 from nautilus_trader.serialization.arrow.util import GENERIC_DATA_PREFIX
 from nautilus_trader.serialization.arrow.util import list_dicts_to_dict_lists
 
@@ -65,17 +64,17 @@
             self.fs.rmdir(self.path)
 
         self.fs.makedirs(self.fs._parent(self.path), exist_ok=True)
 
         self._schemas = list_schemas()
         self._schemas.update(
             {
-                OrderBookDelta: self._schemas[OrderBookData],
-                OrderBookDeltas: self._schemas[OrderBookData],
-                OrderBookSnapshot: self._schemas[OrderBookData],
+                OrderBookDelta: self._schemas[OrderBookDelta],
+                OrderBookDeltas: self._schemas[OrderBookDelta],
+                OrderBookSnapshot: self._schemas[OrderBookDelta],
             },
         )
         self.logger = logger
         self._files: dict[type, BinaryIO] = {}
         self._writers: dict[type, RecordBatchStreamWriter] = {}
         self._create_writers()
 
@@ -101,19 +100,15 @@
 
     def _create_writers(self):
         for cls in self._schemas:
             self._create_writer(cls=cls)
 
     @property
     def closed(self) -> bool:
-        for cls in self._files:
-            if not self._files[cls].closed:
-                return False
-
-        return True
+        return all(self._files[cls].closed for cls in self._files)
 
     def write(self, obj: object) -> None:
         """
         Write the object to the stream.
 
         Parameters
         ----------
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/persistence/wranglers.pxd` & `nautilus_trader-1.174.0/nautilus_trader/persistence/wranglers.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/persistence/wranglers.pyx` & `nautilus_trader-1.174.0/nautilus_trader/persistence/wranglers.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -53,18 +53,20 @@
         if ptr[i].tag == Data_t_Tag.TRADE:
             ticks.append(TradeTick.from_mem_c(ptr[i].trade))
         elif ptr[i].tag == Data_t_Tag.QUOTE:
             ticks.append(QuoteTick.from_mem_c(ptr[i].quote))
 
     return ticks
 
+
 @staticmethod
 def list_from_capsule(capsule) -> list[Data]:
     return capsule_to_data_list(capsule)
 
+
 cdef class QuoteTickDataWrangler:
     """
     Provides a means of building lists of Nautilus `QuoteTick` objects.
 
     Parameters
     ----------
     instrument : Instrument
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/portfolio/__init__.pxd` & `nautilus_trader-1.174.0/nautilus_trader/portfolio/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/portfolio/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/risk/__init__.pxd`

 * *Files 9% similar despite different names*

```diff
@@ -8,9 +8,7 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 # -------------------------------------------------------------------------------------------------
-
-"""The `portfolio` subpackage provides portfolio management functionality."""
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/portfolio/base.pxd` & `nautilus_trader-1.174.0/nautilus_trader/portfolio/base.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/portfolio/base.pyx` & `nautilus_trader-1.174.0/nautilus_trader/portfolio/base.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/portfolio/portfolio.pxd` & `nautilus_trader-1.174.0/nautilus_trader/portfolio/portfolio.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/portfolio/portfolio.pyx` & `nautilus_trader-1.174.0/nautilus_trader/portfolio/portfolio.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/risk/__init__.pxd` & `nautilus_trader-1.174.0/nautilus_trader/serialization/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/risk/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/risk/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/risk/engine.pxd` & `nautilus_trader-1.174.0/nautilus_trader/risk/engine.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/risk/engine.pyx` & `nautilus_trader-1.174.0/nautilus_trader/risk/engine.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/risk/sizing.pxd` & `nautilus_trader-1.174.0/nautilus_trader/risk/sizing.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/risk/sizing.pyx` & `nautilus_trader-1.174.0/nautilus_trader/risk/sizing.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/serialization/__init__.pxd` & `nautilus_trader-1.174.0/nautilus_trader/serialization/arrow/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/serialization/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/serialization/arrow/__init__.pxd` & `nautilus_trader-1.174.0/nautilus_trader/serialization/msgpack/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/serialization/arrow/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/serialization/arrow/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/serialization/arrow/implementations/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/serialization/arrow/implementations/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/serialization/arrow/implementations/account_state.py` & `nautilus_trader-1.174.0/nautilus_trader/serialization/arrow/implementations/account_state.py`

 * *Files 10% similar despite different names*

```diff
@@ -76,34 +76,34 @@
 def _deserialize(values):
     balances = []
     for v in values:
         total = v.get("balance_total")
         if total is None:
             continue
         balances.append(
-            dict(
-                total=total,
-                locked=v["balance_locked"],
-                free=v["balance_free"],
-                currency=v["balance_currency"],
-            ),
+            {
+                "total": total,
+                "locked": v["balance_locked"],
+                "free": v["balance_free"],
+                "currency": v["balance_currency"],
+            },
         )
 
     margins = []
     for v in values:
         initial = v.get("margin_initial")
         if pd.isnull(initial):
             continue
         margins.append(
-            dict(
-                initial=initial,
-                maintenance=v["margin_maintenance"],
-                currency=v["margin_currency"],
-                instrument_id=v["margin_instrument_id"],
-            ),
+            {
+                "initial": initial,
+                "maintenance": v["margin_maintenance"],
+                "currency": v["margin_currency"],
+                "instrument_id": v["margin_instrument_id"],
+            },
         )
 
     state = {
         k: v
         for k, v in values[0].items()
         if not k.startswith("balance_") and not k.startswith("margin_")
     }
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/serialization/arrow/implementations/bar.py` & `nautilus_trader-1.174.0/nautilus_trader/serialization/arrow/implementations/bar.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/serialization/arrow/implementations/instruments.py` & `nautilus_trader-1.174.0/nautilus_trader/trading/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,13 +9,14 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 # -------------------------------------------------------------------------------------------------
 
-from nautilus_trader.model.instruments import Instrument
-from nautilus_trader.serialization.arrow.serializer import register_parquet
+"""
+The `trading` subpackage groups all trading domain specific components and tooling.
 
-
-for cls in Instrument.__subclasses__():
-    register_parquet(cls, partition_keys=tuple())
+This is a top-level package where the majority of users will interface with the
+framework. Custom trading strategies can be implemented by inheriting from the
+`Strategy` base class.
+"""
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/serialization/arrow/implementations/order_book.py` & `nautilus_trader-1.174.0/nautilus_trader/serialization/arrow/implementations/orderbook_v2.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,43 +11,42 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 # -------------------------------------------------------------------------------------------------
 
 import itertools
 from itertools import repeat
+from typing import Union
 
+from nautilus_trader.model.data.book import BookOrder
+from nautilus_trader.model.data.book import OrderBookDelta
+from nautilus_trader.model.data.book import OrderBookDeltas
+from nautilus_trader.model.data.book import OrderBookSnapshot
 from nautilus_trader.model.enums import BookAction
 from nautilus_trader.model.enums import OrderSide
 from nautilus_trader.model.enums import book_type_from_str
 from nautilus_trader.model.identifiers import InstrumentId
-from nautilus_trader.model.orderbook.data import BookOrder
-from nautilus_trader.model.orderbook.data import OrderBookData
-from nautilus_trader.model.orderbook.data import OrderBookDelta
-from nautilus_trader.model.orderbook.data import OrderBookDeltas
-from nautilus_trader.model.orderbook.data import OrderBookSnapshot
 from nautilus_trader.serialization.arrow.serializer import register_parquet
 
 
-def _parse_delta(delta: OrderBookDelta, cls):
+def _parse_delta(delta: Union[OrderBookDelta, OrderBookDeltas, OrderBookSnapshot], cls):
     return dict(**OrderBookDelta.to_dict(delta), _type=cls.__name__)
 
 
-def serialize(data: OrderBookData):
+def serialize(data: Union[OrderBookDelta, OrderBookDeltas, OrderBookSnapshot]):
     if isinstance(data, OrderBookDelta):
         result = [_parse_delta(delta=data, cls=OrderBookDelta)]
     elif isinstance(data, OrderBookDeltas):
         result = [_parse_delta(delta=delta, cls=OrderBookDeltas) for delta in data.deltas]
     elif isinstance(data, OrderBookSnapshot):
         # For a snapshot, we store the individual deltas required to rebuild, namely a CLEAR, followed by ADDs
         result = [
             _parse_delta(
                 OrderBookDelta(
                     instrument_id=data.instrument_id,
-                    book_type=data.book_type,
                     order=None,
                     action=BookAction.CLEAR,
                     ts_event=data.ts_event,
                     ts_init=data.ts_init,
                 ),
                 cls=OrderBookSnapshot,
             ),
@@ -56,27 +55,26 @@
             zip(repeat(OrderSide.SELL), data.asks),
         )
         result.extend(
             [
                 _parse_delta(
                     OrderBookDelta(
                         instrument_id=data.instrument_id,
-                        book_type=data.book_type,
                         ts_event=data.ts_event,
                         ts_init=data.ts_init,
                         order=BookOrder(price=price, size=volume, side=side),
                         action=BookAction.ADD,
                     ),
                     cls=OrderBookSnapshot,
                 )
                 for side, (price, volume) in orders
             ],
         )
     else:  # pragma: no cover (design-time error)
-        raise TypeError(f"invalid `OrderBookData`, was {type(data)}")
+        raise TypeError(f"invalid order book data, was {type(data)}")
     # Add a "last" message to let downstream consumers know the end of this group of messages
     if result:
         result[-1]["_last"] = True
     return result
 
 
 def _is_orderbook_snapshot(values: list):
@@ -119,15 +117,15 @@
         if _is_orderbook_snapshot(values=chunk):  # type: ignore
             results.append(_build_order_book_snapshot(values=chunk))
         elif len(chunk) >= 1:  # type: ignore
             results.append(_build_order_book_deltas(values=chunk))
     return sorted(results, key=lambda x: x.ts_event)
 
 
-for cls in [OrderBookData] + OrderBookData.__subclasses__():
+for cls in [OrderBookDelta, OrderBookDeltas, OrderBookSnapshot]:
     register_parquet(
         cls=cls,
         serializer=serialize,
         deserializer=deserialize,
-        table=OrderBookData,
+        table=OrderBookDelta,
         chunk=True,
     )
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/serialization/arrow/implementations/order_events.py` & `nautilus_trader-1.174.0/nautilus_trader/serialization/arrow/implementations/order_events.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 def serialize_order_initialized(event: OrderInitialized):
     caster = {
         "quantity": float,
         "price": float,
     }
     data = event.to_dict(event)
-    data.update(json.loads(data.pop("options", "{}")))  # noqa: P103
+    data.update(json.loads(data.pop("options", "{}")))
     data = {k: caster[k](v) if (k in caster and v is not None) else v for k, v in data.items()}
     return data
 
 
 def deserialize_order_filled(data: dict) -> OrderFilled:
     for k in ("last_px", "last_qty"):
         data[k] = str(data[k])
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/serialization/arrow/implementations/position_events.py` & `nautilus_trader-1.174.0/nautilus_trader/serialization/arrow/implementations/position_events.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/serialization/arrow/schema.py` & `nautilus_trader-1.174.0/nautilus_trader/serialization/arrow/schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import msgspec
 import pyarrow as pa
 
 from nautilus_trader.adapters.binance.common.types import BinanceBar
 from nautilus_trader.common.messages import ComponentStateChanged
 from nautilus_trader.common.messages import TradingStateChanged
 from nautilus_trader.model.data.bar import Bar
+from nautilus_trader.model.data.book import OrderBookDelta
 from nautilus_trader.model.data.tick import QuoteTick
 from nautilus_trader.model.data.tick import TradeTick
 from nautilus_trader.model.data.ticker import Ticker
 from nautilus_trader.model.data.venue import InstrumentClose
 from nautilus_trader.model.data.venue import InstrumentStatusUpdate
 from nautilus_trader.model.data.venue import VenueStatusUpdate
 from nautilus_trader.model.events.account import AccountState
@@ -47,30 +48,28 @@
 from nautilus_trader.model.instruments import BettingInstrument
 from nautilus_trader.model.instruments import CryptoFuture
 from nautilus_trader.model.instruments import CryptoPerpetual
 from nautilus_trader.model.instruments import CurrencyPair
 from nautilus_trader.model.instruments import Equity
 from nautilus_trader.model.instruments import FuturesContract
 from nautilus_trader.model.instruments import OptionsContract
-from nautilus_trader.model.orderbook.data import OrderBookData
 from nautilus_trader.serialization.arrow.serializer import register_parquet
 
 
 NAUTILUS_PARQUET_SCHEMA = {
-    OrderBookData: pa.schema(
+    OrderBookDelta: pa.schema(
         {
             "instrument_id": pa.dictionary(pa.int64(), pa.string()),
             "ts_event": pa.uint64(),
             "ts_init": pa.uint64(),
             "action": pa.string(),
             "side": pa.string(),
             "price": pa.float64(),
             "size": pa.float64(),
             "order_id": pa.string(),
-            "book_type": pa.string(),
             # Track grouped OrderBookDeltas
             "_type": pa.dictionary(pa.int8(), pa.string()),
             "_last": pa.bool_(),
         },
         metadata={"type": "OrderBookDelta"},
     ),
     Ticker: pa.schema(
@@ -103,28 +102,28 @@
             "ts_event": pa.uint64(),
             "ts_init": pa.uint64(),
         },
         metadata={"type": "TradeTick"},
     ),
     Bar: pa.schema(
         {
-            "bar_type": pa.dictionary(pa.int8(), pa.string()),
+            "bar_type": pa.dictionary(pa.int16(), pa.string()),
             "instrument_id": pa.dictionary(pa.int64(), pa.string()),
             "open": pa.string(),
             "high": pa.string(),
             "low": pa.string(),
             "close": pa.string(),
             "volume": pa.string(),
             "ts_event": pa.uint64(),
             "ts_init": pa.uint64(),
         },
     ),
     VenueStatusUpdate: pa.schema(
         {
-            "venue": pa.dictionary(pa.int8(), pa.string()),
+            "venue": pa.dictionary(pa.int16(), pa.string()),
             "status": pa.dictionary(pa.int8(), pa.string()),
             "ts_event": pa.uint64(),
             "ts_init": pa.uint64(),
         },
         metadata={"type": "InstrumentStatusUpdate"},
     ),
     InstrumentClose: pa.schema(
@@ -144,39 +143,39 @@
             "ts_event": pa.uint64(),
             "ts_init": pa.uint64(),
         },
         metadata={"type": "InstrumentStatusUpdate"},
     ),
     ComponentStateChanged: pa.schema(
         {
-            "trader_id": pa.dictionary(pa.int8(), pa.string()),
-            "component_id": pa.dictionary(pa.int8(), pa.string()),
+            "trader_id": pa.dictionary(pa.int16(), pa.string()),
+            "component_id": pa.dictionary(pa.int16(), pa.string()),
             "component_type": pa.dictionary(pa.int8(), pa.string()),
             "state": pa.string(),
             "config": pa.string(),
             "event_id": pa.string(),
             "ts_event": pa.uint64(),
             "ts_init": pa.uint64(),
         },
         metadata={"type": "ComponentStateChanged"},
     ),
     TradingStateChanged: pa.schema(
         {
-            "trader_id": pa.dictionary(pa.int8(), pa.string()),
+            "trader_id": pa.dictionary(pa.int16(), pa.string()),
             "state": pa.string(),
             "config": pa.binary(),
             "event_id": pa.string(),
             "ts_event": pa.uint64(),
             "ts_init": pa.uint64(),
         },
         metadata={"type": "TradingStateChanged"},
     ),
     AccountState: pa.schema(
         {
-            "account_id": pa.dictionary(pa.int8(), pa.string()),
+            "account_id": pa.dictionary(pa.int16(), pa.string()),
             "account_type": pa.dictionary(pa.int8(), pa.string()),
             "base_currency": pa.dictionary(pa.int16(), pa.string()),
             "balance_total": pa.float64(),
             "balance_locked": pa.float64(),
             "balance_free": pa.float64(),
             "balance_currency": pa.dictionary(pa.int16(), pa.string()),
             "margin_initial": pa.float64(),
@@ -189,15 +188,15 @@
             "ts_event": pa.uint64(),
             "ts_init": pa.uint64(),
         },
         metadata={"type": "AccountState"},
     ),
     OrderInitialized: pa.schema(
         {
-            "trader_id": pa.dictionary(pa.int8(), pa.string()),
+            "trader_id": pa.dictionary(pa.int16(), pa.string()),
             "strategy_id": pa.dictionary(pa.int16(), pa.string()),
             "instrument_id": pa.dictionary(pa.int64(), pa.string()),
             "client_order_id": pa.string(),
             "order_side": pa.dictionary(pa.int8(), pa.string()),
             "order_type": pa.dictionary(pa.int8(), pa.string()),
             "quantity": pa.float64(),
             "time_in_force": pa.dictionary(pa.int8(), pa.string()),
@@ -239,185 +238,185 @@
                     "expire_time_ns",
                 ],
             ),
         },
     ),
     OrderDenied: pa.schema(
         {
-            "trader_id": pa.dictionary(pa.int8(), pa.string()),
-            "strategy_id": pa.dictionary(pa.int8(), pa.string()),
+            "trader_id": pa.dictionary(pa.int16(), pa.string()),
+            "strategy_id": pa.dictionary(pa.int16(), pa.string()),
             "instrument_id": pa.dictionary(pa.int64(), pa.string()),
             "client_order_id": pa.string(),
-            "reason": pa.dictionary(pa.int8(), pa.string()),
+            "reason": pa.dictionary(pa.int16(), pa.string()),
             "event_id": pa.string(),
             "ts_init": pa.uint64(),
         },
     ),
     OrderSubmitted: pa.schema(
         {
-            "trader_id": pa.dictionary(pa.int8(), pa.string()),
+            "trader_id": pa.dictionary(pa.int16(), pa.string()),
             "strategy_id": pa.dictionary(pa.int16(), pa.string()),
-            "account_id": pa.dictionary(pa.int8(), pa.string()),
+            "account_id": pa.dictionary(pa.int16(), pa.string()),
             "instrument_id": pa.dictionary(pa.int64(), pa.string()),
             "client_order_id": pa.string(),
             "event_id": pa.string(),
             "ts_event": pa.uint64(),
             "ts_init": pa.uint64(),
         },
     ),
     OrderAccepted: pa.schema(
         {
-            "trader_id": pa.dictionary(pa.int8(), pa.string()),
+            "trader_id": pa.dictionary(pa.int16(), pa.string()),
             "strategy_id": pa.dictionary(pa.int16(), pa.string()),
-            "account_id": pa.dictionary(pa.int8(), pa.string()),
+            "account_id": pa.dictionary(pa.int16(), pa.string()),
             "instrument_id": pa.dictionary(pa.int64(), pa.string()),
             "client_order_id": pa.string(),
             "venue_order_id": pa.string(),
             "event_id": pa.string(),
             "ts_event": pa.uint64(),
             "ts_init": pa.uint64(),
             "reconciliation": pa.bool_(),
         },
     ),
     OrderRejected: pa.schema(
         {
-            "trader_id": pa.dictionary(pa.int8(), pa.string()),
+            "trader_id": pa.dictionary(pa.int16(), pa.string()),
             "strategy_id": pa.dictionary(pa.int16(), pa.string()),
-            "account_id": pa.dictionary(pa.int8(), pa.string()),
+            "account_id": pa.dictionary(pa.int16(), pa.string()),
             "instrument_id": pa.dictionary(pa.int64(), pa.string()),
             "client_order_id": pa.string(),
-            "reason": pa.dictionary(pa.int8(), pa.string()),
+            "reason": pa.dictionary(pa.int16(), pa.string()),
             "event_id": pa.string(),
             "ts_event": pa.uint64(),
             "ts_init": pa.uint64(),
             "reconciliation": pa.bool_(),
         },
     ),
     OrderPendingCancel: pa.schema(
         {
-            "trader_id": pa.dictionary(pa.int8(), pa.string()),
+            "trader_id": pa.dictionary(pa.int16(), pa.string()),
             "strategy_id": pa.dictionary(pa.int16(), pa.string()),
-            "account_id": pa.dictionary(pa.int8(), pa.string()),
+            "account_id": pa.dictionary(pa.int16(), pa.string()),
             "instrument_id": pa.dictionary(pa.int64(), pa.string()),
             "client_order_id": pa.string(),
             "venue_order_id": pa.string(),
             "event_id": pa.string(),
             "ts_event": pa.uint64(),
             "ts_init": pa.uint64(),
             "reconciliation": pa.bool_(),
         },
     ),
     OrderCanceled: pa.schema(
         {
-            "trader_id": pa.dictionary(pa.int8(), pa.string()),
+            "trader_id": pa.dictionary(pa.int16(), pa.string()),
             "strategy_id": pa.dictionary(pa.int16(), pa.string()),
-            "account_id": pa.dictionary(pa.int8(), pa.string()),
+            "account_id": pa.dictionary(pa.int16(), pa.string()),
             "instrument_id": pa.dictionary(pa.int64(), pa.string()),
             "client_order_id": pa.string(),
             "venue_order_id": pa.string(),
             "event_id": pa.string(),
             "ts_event": pa.uint64(),
             "ts_init": pa.uint64(),
             "reconciliation": pa.bool_(),
         },
     ),
     OrderCancelRejected: pa.schema(
         {
-            "trader_id": pa.dictionary(pa.int8(), pa.string()),
+            "trader_id": pa.dictionary(pa.int16(), pa.string()),
             "strategy_id": pa.dictionary(pa.int16(), pa.string()),
-            "account_id": pa.dictionary(pa.int8(), pa.string()),
+            "account_id": pa.dictionary(pa.int16(), pa.string()),
             "instrument_id": pa.dictionary(pa.int64(), pa.string()),
             "client_order_id": pa.string(),
             "venue_order_id": pa.string(),
             "reason": pa.string(),
             "event_id": pa.string(),
             "ts_event": pa.uint64(),
             "ts_init": pa.uint64(),
             "reconciliation": pa.bool_(),
         },
     ),
     OrderExpired: pa.schema(
         {
-            "trader_id": pa.dictionary(pa.int8(), pa.string()),
+            "trader_id": pa.dictionary(pa.int16(), pa.string()),
             "strategy_id": pa.dictionary(pa.int16(), pa.string()),
-            "account_id": pa.dictionary(pa.int8(), pa.string()),
+            "account_id": pa.dictionary(pa.int16(), pa.string()),
             "instrument_id": pa.dictionary(pa.int64(), pa.string()),
             "client_order_id": pa.string(),
             "venue_order_id": pa.string(),
             "event_id": pa.string(),
             "ts_event": pa.uint64(),
             "ts_init": pa.uint64(),
             "reconciliation": pa.bool_(),
         },
     ),
     OrderTriggered: pa.schema(
         {
-            "trader_id": pa.dictionary(pa.int8(), pa.string()),
+            "trader_id": pa.dictionary(pa.int16(), pa.string()),
             "strategy_id": pa.dictionary(pa.int16(), pa.string()),
-            "account_id": pa.dictionary(pa.int8(), pa.string()),
+            "account_id": pa.dictionary(pa.int16(), pa.string()),
             "instrument_id": pa.dictionary(pa.int64(), pa.string()),
             "client_order_id": pa.string(),
             "venue_order_id": pa.string(),
             "event_id": pa.string(),
             "ts_event": pa.uint64(),
             "ts_init": pa.uint64(),
             "reconciliation": pa.bool_(),
         },
     ),
     OrderPendingUpdate: pa.schema(
         {
-            "trader_id": pa.dictionary(pa.int8(), pa.string()),
+            "trader_id": pa.dictionary(pa.int16(), pa.string()),
             "strategy_id": pa.dictionary(pa.int16(), pa.string()),
-            "account_id": pa.dictionary(pa.int8(), pa.string()),
+            "account_id": pa.dictionary(pa.int16(), pa.string()),
             "instrument_id": pa.dictionary(pa.int64(), pa.string()),
             "client_order_id": pa.string(),
             "venue_order_id": pa.string(),
             "event_id": pa.string(),
             "ts_event": pa.uint64(),
             "ts_init": pa.uint64(),
             "reconciliation": pa.bool_(),
         },
     ),
     OrderModifyRejected: pa.schema(
         {
-            "trader_id": pa.dictionary(pa.int8(), pa.string()),
+            "trader_id": pa.dictionary(pa.int16(), pa.string()),
             "strategy_id": pa.dictionary(pa.int16(), pa.string()),
-            "account_id": pa.dictionary(pa.int8(), pa.string()),
+            "account_id": pa.dictionary(pa.int16(), pa.string()),
             "instrument_id": pa.dictionary(pa.int64(), pa.string()),
             "client_order_id": pa.string(),
             "venue_order_id": pa.string(),
-            "reason": pa.dictionary(pa.int8(), pa.string()),
+            "reason": pa.dictionary(pa.int16(), pa.string()),
             "event_id": pa.string(),
             "ts_event": pa.uint64(),
             "ts_init": pa.uint64(),
             "reconciliation": pa.bool_(),
         },
     ),
     OrderUpdated: pa.schema(
         {
-            "trader_id": pa.dictionary(pa.int8(), pa.string()),
+            "trader_id": pa.dictionary(pa.int16(), pa.string()),
             "strategy_id": pa.dictionary(pa.int16(), pa.string()),
-            "account_id": pa.dictionary(pa.int8(), pa.string()),
+            "account_id": pa.dictionary(pa.int16(), pa.string()),
             "instrument_id": pa.dictionary(pa.int64(), pa.string()),
             "client_order_id": pa.string(),
             "venue_order_id": pa.string(),
             "price": pa.float64(),
             "quantity": pa.float64(),
             "trigger_price": pa.float64(),
             "event_id": pa.string(),
             "ts_event": pa.uint64(),
             "ts_init": pa.uint64(),
             "reconciliation": pa.bool_(),
         },
     ),
     OrderFilled: pa.schema(
         {
-            "trader_id": pa.dictionary(pa.int8(), pa.string()),
+            "trader_id": pa.dictionary(pa.int16(), pa.string()),
             "strategy_id": pa.dictionary(pa.int16(), pa.string()),
-            "account_id": pa.dictionary(pa.int8(), pa.string()),
+            "account_id": pa.dictionary(pa.int16(), pa.string()),
             "instrument_id": pa.dictionary(pa.int64(), pa.string()),
             "client_order_id": pa.string(),
             "venue_order_id": pa.string(),
             "trade_id": pa.string(),
             "position_id": pa.string(),
             "order_side": pa.dictionary(pa.int8(), pa.string()),
             "order_type": pa.dictionary(pa.int8(), pa.string()),
@@ -431,18 +430,18 @@
             "ts_init": pa.uint64(),
             "info": pa.binary(),
             "reconciliation": pa.bool_(),
         },
     ),
     PositionOpened: pa.schema(
         {
-            "trader_id": pa.dictionary(pa.int8(), pa.string()),
+            "trader_id": pa.dictionary(pa.int16(), pa.string()),
             "strategy_id": pa.dictionary(pa.int16(), pa.string()),
             "instrument_id": pa.dictionary(pa.int64(), pa.string()),
-            "account_id": pa.dictionary(pa.int8(), pa.string()),
+            "account_id": pa.dictionary(pa.int16(), pa.string()),
             "position_id": pa.string(),
             "opening_order_id": pa.string(),
             "entry": pa.string(),
             "side": pa.string(),
             "signed_qty": pa.float64(),
             "quantity": pa.float64(),
             "peak_qty": pa.float64(),
@@ -455,18 +454,18 @@
             "duration_ns": pa.uint64(),
             "ts_event": pa.uint64(),
             "ts_init": pa.uint64(),
         },
     ),
     PositionChanged: pa.schema(
         {
-            "trader_id": pa.dictionary(pa.int8(), pa.string()),
+            "trader_id": pa.dictionary(pa.int16(), pa.string()),
             "strategy_id": pa.dictionary(pa.int16(), pa.string()),
             "instrument_id": pa.dictionary(pa.int64(), pa.string()),
-            "account_id": pa.dictionary(pa.int8(), pa.string()),
+            "account_id": pa.dictionary(pa.int16(), pa.string()),
             "position_id": pa.string(),
             "opening_order_id": pa.string(),
             "entry": pa.string(),
             "side": pa.string(),
             "signed_qty": pa.float64(),
             "quantity": pa.float64(),
             "peak_qty": pa.float64(),
@@ -482,16 +481,16 @@
             "ts_opened": pa.uint64(),
             "ts_event": pa.uint64(),
             "ts_init": pa.uint64(),
         },
     ),
     PositionClosed: pa.schema(
         {
-            "trader_id": pa.dictionary(pa.int8(), pa.string()),
-            "account_id": pa.dictionary(pa.int8(), pa.string()),
+            "trader_id": pa.dictionary(pa.int16(), pa.string()),
+            "account_id": pa.dictionary(pa.int16(), pa.string()),
             "strategy_id": pa.dictionary(pa.int16(), pa.string()),
             "instrument_id": pa.dictionary(pa.int64(), pa.string()),
             "position_id": pa.string(),
             "opening_order_id": pa.string(),
             "closing_order_id": pa.string(),
             "entry": pa.string(),
             "side": pa.string(),
@@ -542,17 +541,17 @@
         {
             "id": pa.dictionary(pa.int64(), pa.string()),
             "native_symbol": pa.string(),
             "base_currency": pa.dictionary(pa.int16(), pa.string()),
             "quote_currency": pa.dictionary(pa.int16(), pa.string()),
             "price_precision": pa.uint8(),
             "size_precision": pa.uint8(),
-            "price_increment": pa.dictionary(pa.int8(), pa.string()),
-            "size_increment": pa.dictionary(pa.int8(), pa.string()),
-            "lot_size": pa.dictionary(pa.int8(), pa.string()),
+            "price_increment": pa.dictionary(pa.int16(), pa.string()),
+            "size_increment": pa.dictionary(pa.int16(), pa.string()),
+            "lot_size": pa.dictionary(pa.int16(), pa.string()),
             "max_quantity": pa.dictionary(pa.int16(), pa.string()),
             "min_quantity": pa.dictionary(pa.int16(), pa.string()),
             "max_notional": pa.dictionary(pa.int16(), pa.string()),
             "min_notional": pa.dictionary(pa.int16(), pa.string()),
             "max_price": pa.dictionary(pa.int16(), pa.string()),
             "min_price": pa.dictionary(pa.int16(), pa.string()),
             "margin_init": pa.string(),
@@ -570,16 +569,16 @@
             "native_symbol": pa.string(),
             "base_currency": pa.dictionary(pa.int16(), pa.string()),
             "quote_currency": pa.dictionary(pa.int16(), pa.string()),
             "settlement_currency": pa.dictionary(pa.int16(), pa.string()),
             "is_inverse": pa.bool_(),
             "price_precision": pa.uint8(),
             "size_precision": pa.uint8(),
-            "price_increment": pa.dictionary(pa.int8(), pa.string()),
-            "size_increment": pa.dictionary(pa.int8(), pa.string()),
+            "price_increment": pa.dictionary(pa.int16(), pa.string()),
+            "size_increment": pa.dictionary(pa.int16(), pa.string()),
             "max_quantity": pa.dictionary(pa.int16(), pa.string()),
             "min_quantity": pa.dictionary(pa.int16(), pa.string()),
             "max_notional": pa.dictionary(pa.int16(), pa.string()),
             "min_notional": pa.dictionary(pa.int16(), pa.string()),
             "max_price": pa.dictionary(pa.int16(), pa.string()),
             "min_price": pa.dictionary(pa.int16(), pa.string()),
             "margin_init": pa.string(),
@@ -594,25 +593,25 @@
     CryptoFuture: pa.schema(
         {
             "id": pa.dictionary(pa.int64(), pa.string()),
             "native_symbol": pa.string(),
             "underlying": pa.dictionary(pa.int16(), pa.string()),
             "quote_currency": pa.dictionary(pa.int16(), pa.string()),
             "settlement_currency": pa.dictionary(pa.int16(), pa.string()),
-            "expiry_date": pa.dictionary(pa.int8(), pa.string()),
+            "expiry_date": pa.dictionary(pa.int16(), pa.string()),
             "price_precision": pa.uint8(),
             "size_precision": pa.uint8(),
-            "price_increment": pa.dictionary(pa.int8(), pa.string()),
-            "size_increment": pa.dictionary(pa.int8(), pa.string()),
+            "price_increment": pa.dictionary(pa.int16(), pa.string()),
+            "size_increment": pa.dictionary(pa.int16(), pa.string()),
             "max_quantity": pa.dictionary(pa.int16(), pa.string()),
             "min_quantity": pa.dictionary(pa.int16(), pa.string()),
             "max_notional": pa.dictionary(pa.int16(), pa.string()),
             "min_notional": pa.dictionary(pa.int16(), pa.string()),
-            "max_price": pa.dictionary(pa.int8(), pa.string()),
-            "min_price": pa.dictionary(pa.int8(), pa.string()),
+            "max_price": pa.dictionary(pa.int16(), pa.string()),
+            "min_price": pa.dictionary(pa.int16(), pa.string()),
             "margin_init": pa.string(),
             "margin_maint": pa.string(),
             "maker_fee": pa.string(),
             "taker_fee": pa.string(),
             "info": pa.binary(),
             "ts_event": pa.uint64(),
             "ts_init": pa.uint64(),
@@ -621,18 +620,18 @@
     Equity: pa.schema(
         {
             "id": pa.dictionary(pa.int64(), pa.string()),
             "native_symbol": pa.string(),
             "currency": pa.dictionary(pa.int16(), pa.string()),
             "price_precision": pa.uint8(),
             "size_precision": pa.uint8(),
-            "price_increment": pa.dictionary(pa.int8(), pa.string()),
-            "size_increment": pa.dictionary(pa.int8(), pa.string()),
-            "multiplier": pa.dictionary(pa.int8(), pa.string()),
-            "lot_size": pa.dictionary(pa.int8(), pa.string()),
+            "price_increment": pa.dictionary(pa.int16(), pa.string()),
+            "size_increment": pa.dictionary(pa.int16(), pa.string()),
+            "multiplier": pa.dictionary(pa.int16(), pa.string()),
+            "lot_size": pa.dictionary(pa.int16(), pa.string()),
             "isin": pa.string(),
             "margin_init": pa.string(),
             "margin_maint": pa.string(),
             "maker_fee": pa.string(),
             "taker_fee": pa.string(),
             "ts_event": pa.uint64(),
             "ts_init": pa.uint64(),
@@ -643,36 +642,36 @@
             "id": pa.dictionary(pa.int64(), pa.string()),
             "native_symbol": pa.string(),
             "underlying": pa.dictionary(pa.int16(), pa.string()),
             "asset_class": pa.dictionary(pa.int8(), pa.string()),
             "currency": pa.dictionary(pa.int16(), pa.string()),
             "price_precision": pa.uint8(),
             "size_precision": pa.uint8(),
-            "price_increment": pa.dictionary(pa.int8(), pa.string()),
-            "size_increment": pa.dictionary(pa.int8(), pa.string()),
-            "multiplier": pa.dictionary(pa.int8(), pa.string()),
-            "lot_size": pa.dictionary(pa.int8(), pa.string()),
-            "expiry_date": pa.dictionary(pa.int8(), pa.string()),
+            "price_increment": pa.dictionary(pa.int16(), pa.string()),
+            "size_increment": pa.dictionary(pa.int16(), pa.string()),
+            "multiplier": pa.dictionary(pa.int16(), pa.string()),
+            "lot_size": pa.dictionary(pa.int16(), pa.string()),
+            "expiry_date": pa.dictionary(pa.int16(), pa.string()),
             "ts_event": pa.uint64(),
             "ts_init": pa.uint64(),
         },
     ),
     OptionsContract: pa.schema(
         {
             "id": pa.dictionary(pa.int64(), pa.string()),
             "native_symbol": pa.string(),
             "underlying": pa.dictionary(pa.int16(), pa.string()),
             "asset_class": pa.dictionary(pa.int8(), pa.string()),
             "currency": pa.dictionary(pa.int16(), pa.string()),
             "price_precision": pa.uint8(),
             "size_precision": pa.uint8(),
-            "price_increment": pa.dictionary(pa.int8(), pa.string()),
-            "size_increment": pa.dictionary(pa.int8(), pa.string()),
-            "multiplier": pa.dictionary(pa.int8(), pa.string()),
-            "lot_size": pa.dictionary(pa.int8(), pa.string()),
+            "price_increment": pa.dictionary(pa.int16(), pa.string()),
+            "size_increment": pa.dictionary(pa.int16(), pa.string()),
+            "multiplier": pa.dictionary(pa.int16(), pa.string()),
+            "lot_size": pa.dictionary(pa.int16(), pa.string()),
             "expiry_date": pa.dictionary(pa.int64(), pa.string()),
             "strike_price": pa.dictionary(pa.int64(), pa.string()),
             "kind": pa.dictionary(pa.int8(), pa.string()),
             "ts_event": pa.uint64(),
             "ts_init": pa.uint64(),
         },
     ),
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/serialization/arrow/serializer.pxd` & `nautilus_trader-1.174.0/nautilus_trader/serialization/arrow/serializer.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/serialization/arrow/serializer.pyx` & `nautilus_trader-1.174.0/nautilus_trader/serialization/arrow/serializer.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/serialization/arrow/util.py` & `nautilus_trader-1.174.0/nautilus_trader/serialization/arrow/util.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/serialization/base.pxd` & `nautilus_trader-1.174.0/nautilus_trader/serialization/base.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/serialization/base.pyx` & `nautilus_trader-1.174.0/nautilus_trader/serialization/base.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/serialization/msgpack/__init__.pxd` & `nautilus_trader-1.174.0/nautilus_trader/serialization/msgpack/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/serialization/msgpack/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/system/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/serialization/msgpack/serializer.pxd` & `nautilus_trader-1.174.0/nautilus_trader/serialization/msgpack/serializer.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/serialization/msgpack/serializer.pyx` & `nautilus_trader-1.174.0/nautilus_trader/serialization/msgpack/serializer.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/system/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/test_kit/mocks/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/system/kernel.py` & `nautilus_trader-1.174.0/nautilus_trader/system/kernel.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,15 @@
             trader_id=self._trader_id,
             machine_id=self._machine_id,
             instance_id=self._instance_id,
             level_stdout=log_level_from_str(logging.log_level),
             level_file=log_level_from_str(logging.log_level_file)
             if logging.log_level_file is not None
             else LogLevel.DEBUG,
-            file_logging=True if logging.log_level_file is not None else False,
+            file_logging=logging.log_level_file is not None,
             directory=logging.log_directory,
             file_name=logging.log_file_name,
             file_format=logging.log_file_format,
             component_levels=logging.log_component_levels,
             bypass=False if self._environment == Environment.LIVE else logging.bypass_logging,
         )
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/test_kit/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/trading/__init__.pxd`

 * *Files 21% similar despite different names*

```diff
@@ -8,12 +8,7 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 # -------------------------------------------------------------------------------------------------
-
-"""
-The test kit contains test doubles and helpers to support the NautilusTrader
-test suite, as well as supporting testing for downstream projects and packages.
-"""
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/test_kit/mocks/__init__.py` & `nautilus_trader-1.174.0/nautilus_trader/test_kit/stubs/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,7 +8,31 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 # -------------------------------------------------------------------------------------------------
+
+from datetime import datetime
+
+import pytz
+
+from nautilus_trader.core.data import Data
+
+
+UNIX_EPOCH = datetime(1970, 1, 1, 0, 0, 0, 0, tzinfo=pytz.utc)
+
+
+class MyData(Data):
+    """
+    Represents an example user defined data class.
+    """
+
+    def __init__(
+        self,
+        value,
+        ts_event=0,
+        ts_init=0,
+    ):
+        super().__init__(ts_event, ts_init)
+        self.value = value
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/test_kit/mocks/actors.py` & `nautilus_trader-1.174.0/nautilus_trader/test_kit/mocks/actors.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/test_kit/mocks/cache_database.py` & `nautilus_trader-1.174.0/nautilus_trader/test_kit/mocks/cache_database.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/test_kit/mocks/data.py` & `nautilus_trader-1.174.0/nautilus_trader/test_kit/mocks/data.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,27 +38,22 @@
     def parse(self, block: bytes) -> Generator:
         yield block
 
 
 class NewsEventData(NewsEvent):
     """Generic data NewsEvent"""
 
-    pass
-
 
 def data_catalog_setup(protocol, path=None) -> ParquetDataCatalog:
     if protocol not in ("memory", "file"):
         raise ValueError("`protocol` should only be one of `memory` or `file` for testing")
 
     clear_singleton_instances(ParquetDataCatalog)
 
-    if path is None:
-        path = Path.cwd() / "data_catalog"
-    else:
-        path = Path(path).resolve()
+    path = Path.cwd() / "data_catalog" if path is None else Path(path).resolve()
 
     path = str(path)
     catalog = ParquetDataCatalog(path=path, fs_protocol=protocol)
 
     if catalog.fs.exists(path):
         catalog.fs.rm(path, recursive=True)
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/test_kit/mocks/engines.py` & `nautilus_trader-1.174.0/nautilus_trader/test_kit/mocks/engines.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/test_kit/mocks/exec_clients.py` & `nautilus_trader-1.174.0/nautilus_trader/test_kit/mocks/exec_clients.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/test_kit/mocks/strategies.py` & `nautilus_trader-1.174.0/nautilus_trader/test_kit/mocks/strategies.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/test_kit/performance.py` & `nautilus_trader-1.174.0/nautilus_trader/test_kit/performance.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         results = timeit.Timer(target).repeat(repeat=runs, number=iterations)
         minimum = min(results)  # In seconds
 
         if print_output:
             result_milli = minimum * 1_000  # 1,000ms in 1 second
             result_micro = minimum * 1_000_000  # 1,000,000μs in 1 second
             result_nano = minimum * 1_000_000_000  # 1,000,000,000ns in 1 second
-            print(f"\nPerformance test: {str(inspect.getmembers(target)[4][1])} ")
+            print(f"\nPerformance test: {inspect.getmembers(target)[4][1]!s} ")
             print(
                 f"# ~{result_milli:.1f}ms "
                 f"/ ~{result_micro:.1f}μs "
                 f"/ {result_nano:.0f}ns "
                 f"minimum of {runs:,} runs @ {iterations:,} "
                 f"iteration{'s' if iterations > 1 else ''} each run.",
             )
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/test_kit/providers.py` & `nautilus_trader-1.174.0/nautilus_trader/test_kit/providers.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/test_kit/stubs/commands.py` & `nautilus_trader-1.174.0/nautilus_trader/test_kit/stubs/commands.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/test_kit/stubs/component.py` & `nautilus_trader-1.174.0/nautilus_trader/test_kit/stubs/component.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/test_kit/stubs/config.py` & `nautilus_trader-1.174.0/nautilus_trader/test_kit/stubs/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,18 +56,18 @@
         )
 
     @staticmethod
     def order_book_imbalance(instrument_id=None) -> ImportableStrategyConfig:
         return ImportableStrategyConfig(
             strategy_path="nautilus_trader.examples.strategies.orderbook_imbalance:OrderBookImbalance",
             config_path="nautilus_trader.examples.strategies.orderbook_imbalance:OrderBookImbalanceConfig",
-            config=dict(
-                instrument_id=instrument_id or AAPL_US,
-                max_trade_size=50,
-            ),
+            config={
+                "instrument_id": instrument_id or AAPL_US,
+                "max_trade_size": 50,
+            },
         )
 
     @staticmethod
     def exec_engine_config() -> ExecEngineConfig:
         return ExecEngineConfig(allow_cash_positions=True, debug=True)
 
     @staticmethod
@@ -81,18 +81,18 @@
 
     @staticmethod
     def strategies_config() -> list[ImportableStrategyConfig]:
         return [
             ImportableStrategyConfig(
                 strategy_path="nautilus_trader.examples.strategies.orderbook_imbalance:OrderBookImbalance",
                 config_path="nautilus_trader.examples.strategies.orderbook_imbalance:OrderBookImbalanceConfig",
-                config=dict(
-                    instrument_id=AAPL_US.id.value,
-                    max_trade_size=50,
-                ),
+                config={
+                    "instrument_id": AAPL_US.id.value,
+                    "max_trade_size": 50,
+                },
             ),
         ]
 
     @staticmethod
     def backtest_engine_config(
         log_level="INFO",
         bypass_logging=True,
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/test_kit/stubs/data.py` & `nautilus_trader-1.174.0/nautilus_trader/test_kit/stubs/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,41 +18,40 @@
 
 import pandas as pd
 
 from nautilus_trader.core.datetime import millis_to_nanos
 from nautilus_trader.model.data.bar import Bar
 from nautilus_trader.model.data.bar import BarSpecification
 from nautilus_trader.model.data.bar import BarType
+from nautilus_trader.model.data.book import BookOrder
+from nautilus_trader.model.data.book import OrderBookDelta
+from nautilus_trader.model.data.book import OrderBookDeltas
+from nautilus_trader.model.data.book import OrderBookSnapshot
 from nautilus_trader.model.data.tick import QuoteTick
 from nautilus_trader.model.data.tick import TradeTick
 from nautilus_trader.model.data.ticker import Ticker
 from nautilus_trader.model.data.venue import InstrumentClose
 from nautilus_trader.model.data.venue import InstrumentStatusUpdate
 from nautilus_trader.model.data.venue import VenueStatusUpdate
 from nautilus_trader.model.enums import AggressorSide
 from nautilus_trader.model.enums import BarAggregation
 from nautilus_trader.model.enums import BookAction
 from nautilus_trader.model.enums import BookType
 from nautilus_trader.model.enums import InstrumentCloseType
 from nautilus_trader.model.enums import MarketStatus
 from nautilus_trader.model.enums import OrderSide
 from nautilus_trader.model.enums import PriceType
-from nautilus_trader.model.enums import TimeInForce
 from nautilus_trader.model.identifiers import InstrumentId
 from nautilus_trader.model.identifiers import Symbol
 from nautilus_trader.model.identifiers import TradeId
 from nautilus_trader.model.identifiers import Venue
 from nautilus_trader.model.instruments import Instrument
 from nautilus_trader.model.objects import Price
 from nautilus_trader.model.objects import Quantity
 from nautilus_trader.model.orderbook import OrderBook
-from nautilus_trader.model.orderbook import OrderBookDelta
-from nautilus_trader.model.orderbook import OrderBookDeltas
-from nautilus_trader.model.orderbook import OrderBookSnapshot
-from nautilus_trader.model.orderbook.data import BookOrder
 from nautilus_trader.model.orderbook.ladder import Ladder
 from nautilus_trader.persistence.wranglers import QuoteTickDataWrangler
 from nautilus_trader.test_kit.providers import TestDataProvider
 from nautilus_trader.test_kit.providers import TestInstrumentProvider
 from nautilus_trader.test_kit.stubs.identifiers import TestIdStubs
 
 
@@ -304,46 +303,40 @@
         instrument_id=None,
         bid_price=10,
         ask_price=15,
         bid_levels=3,
         ask_levels=3,
         bid_size=10,
         ask_size=10,
-        book_type=BookType.L2_MBP,
-        time_in_force=TimeInForce.GTC,
     ) -> OrderBookSnapshot:
         err = "Too many levels generated; orders will be in cross. Increase bid/ask spread or reduce number of levels"
         assert bid_price < ask_price, err
 
         return OrderBookSnapshot(
             instrument_id=instrument_id or TestIdStubs.audusd_id(),
-            book_type=book_type,
             bids=[(float(bid_price - i), float(bid_size * (1 + i))) for i in range(bid_levels)],
             asks=[(float(ask_price + i), float(ask_size * (1 + i))) for i in range(ask_levels)],
             ts_event=0,
             ts_init=0,
-            time_in_force=time_in_force,
         )
 
     @staticmethod
     def order_book_delta(instrument_id: Optional[InstrumentId] = None, order=None):
         return OrderBookDelta(
             instrument_id=instrument_id or TestIdStubs.audusd_id(),
-            book_type=BookType.L2_MBP,
             action=BookAction.ADD,
             order=order or TestDataStubs.order(),
             ts_event=0,
             ts_init=0,
         )
 
     @staticmethod
     def order_book_deltas(deltas=None):
         return OrderBookDeltas(
             instrument_id=TestIdStubs.audusd_id(),
-            book_type=BookType.L2_MBP,
             deltas=deltas or [TestDataStubs.order_book_delta()],
             ts_event=0,
             ts_init=0,
         )
 
     @staticmethod
     def make_book(
@@ -466,28 +459,28 @@
                 print("Err", updates)
                 return
             for values in updates:
                 keys = ("order_id", "price", "size")
                 data = dict(zip(keys, values))
                 side = OrderSide.BUY if data["size"] >= 0 else OrderSide.SELL
                 if data["price"] == 0:
-                    yield dict(
-                        op="delete",
-                        order=BookOrder(
+                    yield {
+                        "op": "delete",
+                        "order": BookOrder(
                             price=Price(data["price"], precision=9),
                             size=Quantity(abs(data["size"]), precision=9),
                             side=side,
                             order_id=str(data["order_id"]),
                         ),
-                    )
+                    }
                 else:
-                    yield dict(
-                        op="update",
-                        order=BookOrder(
+                    yield {
+                        "op": "update",
+                        "order": BookOrder(
                             price=Price(data["price"], precision=9),
                             size=Quantity(abs(data["size"]), precision=9),
                             side=side,
                             order_id=str(data["order_id"]),
                         ),
-                    )
+                    }
 
         return [msg for data in json.loads(open(filename).read()) for msg in parser(data)]
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/test_kit/stubs/events.py` & `nautilus_trader-1.174.0/nautilus_trader/test_kit/stubs/events.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/test_kit/stubs/execution.py` & `nautilus_trader-1.174.0/nautilus_trader/test_kit/stubs/execution.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from nautilus_trader.model.enums import TimeInForce
 from nautilus_trader.model.identifiers import AccountId
 from nautilus_trader.model.identifiers import ClientOrderId
 from nautilus_trader.model.identifiers import InstrumentId
 from nautilus_trader.model.identifiers import StrategyId
 from nautilus_trader.model.identifiers import TradeId
 from nautilus_trader.model.identifiers import VenueOrderId
+from nautilus_trader.model.instruments import Instrument
 from nautilus_trader.model.objects import Price
 from nautilus_trader.model.objects import Quantity
 from nautilus_trader.model.orders import LimitOrder
 from nautilus_trader.model.orders import MarketOrder
 from nautilus_trader.model.orders import Order
 from nautilus_trader.test_kit.stubs.events import TestEventStubs
 from nautilus_trader.test_kit.stubs.identifiers import TestIdStubs
@@ -48,15 +49,15 @@
     @staticmethod
     def margin_account(account_id: Optional[AccountId] = None) -> MarginAccount:
         return AccountFactory.create(
             TestEventStubs.margin_account_state(account_id=account_id or TestIdStubs.account_id()),
         )
 
     @staticmethod
-    def betting_account(account_id=None) -> BettingAccount:
+    def betting_account(account_id: Optional[AccountId] = None) -> BettingAccount:
         return AccountFactory.create(
             TestEventStubs.betting_account_state(account_id=account_id or TestIdStubs.account_id()),
         )
 
     @staticmethod
     def limit_order(
         instrument_id=None,
@@ -147,12 +148,12 @@
             venue_order_id=venue_order_id,
         )
         assert order
         order.apply(accepted)
         return order
 
     @staticmethod
-    def make_filled_order(instrument, **kwargs) -> Order:
+    def make_filled_order(instrument: Instrument, **kwargs) -> Order:
         order = TestExecStubs.make_accepted_order(instrument_id=instrument.id, **kwargs)
         fill = TestEventStubs.order_filled(order=order, instrument=instrument)
         order.apply(fill)
         return order
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/test_kit/stubs/identifiers.py` & `nautilus_trader-1.174.0/nautilus_trader/test_kit/stubs/identifiers.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/test_kit/stubs/persistence.py` & `nautilus_trader-1.174.0/nautilus_trader/test_kit/stubs/persistence.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/trading/filters.pxd` & `nautilus_trader-1.174.0/nautilus_trader/trading/filters.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/trading/filters.pyx` & `nautilus_trader-1.174.0/nautilus_trader/trading/filters.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/trading/strategy.pxd` & `nautilus_trader-1.174.0/nautilus_trader/trading/strategy.pxd`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 from nautilus_trader.model.enums_c cimport PositionSide
 from nautilus_trader.model.events.order cimport OrderCanceled
 from nautilus_trader.model.events.order cimport OrderDenied
 from nautilus_trader.model.events.order cimport OrderPendingCancel
 from nautilus_trader.model.events.order cimport OrderPendingUpdate
 from nautilus_trader.model.identifiers cimport ClientId
 from nautilus_trader.model.identifiers cimport ClientOrderId
+from nautilus_trader.model.identifiers cimport ExecAlgorithmId
 from nautilus_trader.model.identifiers cimport InstrumentId
 from nautilus_trader.model.identifiers cimport PositionId
 from nautilus_trader.model.identifiers cimport TraderId
 from nautilus_trader.model.objects cimport Price
 from nautilus_trader.model.objects cimport Quantity
 from nautilus_trader.model.orders.base cimport Order
 from nautilus_trader.model.orders.list cimport OrderList
@@ -131,10 +132,10 @@
     cdef void _deny_order(self, Order order, str reason)
     cdef void _deny_order_list(self, OrderList order_list, str reason)
     cdef void _cancel_algo_order(self, Order order)
 
 # -- EGRESS ---------------------------------------------------------------------------------------
 
     cdef void _send_emulator_command(self, TradingCommand command)
-    cdef void _send_algo_command(self, TradingCommand command)
+    cdef void _send_algo_command(self, TradingCommand command, ExecAlgorithmId exec_algorithm_id)
     cdef void _send_risk_command(self, TradingCommand command)
     cdef void _send_exec_command(self, TradingCommand command)
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/trading/strategy.pyx` & `nautilus_trader-1.174.0/nautilus_trader/trading/strategy.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -501,15 +501,15 @@
         if manage_gtd_expiry and order.time_in_force == TimeInForce.GTD:
             self._set_gtd_expiry(order)
 
         # Route order
         if order.is_emulated_c():
             self._send_emulator_command(command)
         elif order.exec_algorithm_id is not None:
-            self._send_algo_command(command)
+            self._send_algo_command(command, order.exec_algorithm_id)
         else:
             self._send_risk_command(command)
 
     cpdef void submit_order_list(
         self,
         OrderList order_list,
         PositionId position_id = None,
@@ -603,15 +603,15 @@
                 if order.time_in_force == TimeInForce.GTD:
                     self._set_gtd_expiry(order)
 
         # Route order
         if command.has_emulated_order:
             self._send_emulator_command(command)
         elif order_list.first.exec_algorithm_id is not None:
-            self._send_algo_command(command)
+            self._send_algo_command(command, order_list.first.exec_algorithm_id)
         else:
             self._send_risk_command(command)
 
     cpdef void modify_order(
         self,
         Order order,
         Quantity quantity = None,
@@ -790,15 +790,15 @@
             venue_order_id=order.venue_order_id,
             command_id=UUID4(),
             ts_init=self.clock.timestamp_ns(),
             client_id=client_id,
         )
 
         if order.exec_algorithm_id is not None:
-            self._send_algo_command(command)
+            self._send_algo_command(command, order.exec_algorithm_id)
 
         if order.is_emulated_c():
             self._send_emulator_command(command)
         else:
             self._send_risk_command(command)
 
     cpdef void cancel_all_orders(
@@ -1444,18 +1444,18 @@
         )
 
 # -- EGRESS ---------------------------------------------------------------------------------------
 
     cdef void _send_emulator_command(self, TradingCommand command):
         self._msgbus.send(endpoint="OrderEmulator.execute", msg=command)
 
-    cdef void _send_algo_command(self, TradingCommand command):
+    cdef void _send_algo_command(self, TradingCommand command, ExecAlgorithmId exec_algorithm_id):
         if not self.log.is_bypassed:
             self.log.info(f"{CMD}{SENT} {command}.")
-        self._msgbus.send(endpoint=f"{command.exec_algorithm_id}.execute", msg=command)
+        self._msgbus.send(endpoint=f"{exec_algorithm_id}.execute", msg=command)
 
     cdef void _send_risk_command(self, TradingCommand command):
         if not self.log.is_bypassed:
             self.log.info(f"{CMD}{SENT} {command}.")
         self._msgbus.send(endpoint="RiskEngine.execute", msg=command)
 
     cdef void _send_exec_command(self, TradingCommand command):
```

### Comparing `nautilus_trader-1.173.0/nautilus_trader/trading/trader.pxd` & `nautilus_trader-1.174.0/nautilus_trader/trading/trader.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/nautilus_trader/trading/trader.pyx` & `nautilus_trader-1.174.0/nautilus_trader/trading/trader.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.173.0/pyproject.toml` & `nautilus_trader-1.174.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 [tool.poetry]
 name = "nautilus_trader"
-version = "1.173.0"
+version = "1.174.0"
 description = "A high-performance algorithmic trading platform and event-driven backtester"
 authors = ["Nautech Systems <info@nautechsystems.io>"]
 license = "LGPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://nautilustrader.io"
 repository = "https://github.com/nautechsystems/nautilus_trader"
 classifiers = [
     "License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)",
     "Operating System :: OS Independent",
     "Development Status :: 4 - Beta",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Scientific/Engineering",
     "Topic :: Office/Business :: Financial",
     "Topic :: Office/Business :: Financial :: Investment",
     "Intended Audience :: Developers",
     "Intended Audience :: Financial and Insurance Industry",
@@ -53,58 +50,57 @@
 click = "^8.1.3"
 frozendict = "^2.3.8"
 fsspec = ">=2022.5.0"
 msgspec = "^0.14.2"
 numpy = "^1.24.3"
 pandas = "^1.5.3"
 psutil = "^5.9.5"
-pyarrow = "^10.0.1"
+pyarrow = "^12.0.0"
 pytz = "^2023.3.0"
 tabulate = "^0.9.0"
 toml = "^0.10.2"
 tqdm = "^4.65.0"
 uvloop = {version = "^0.17.0", markers = "sys_platform != 'win32'"}
 hiredis = {version = "^2.2.3", optional = true}
-ib_insync = {version = "^0.9.83", optional = true}
-redis = {version = "^4.5.4", optional = true}
-docker = {version = "^6.0.1", optional = true}
+ib_insync = {version = "^0.9.85", optional = true}
+redis = {version = "^4.5.5", optional = true}
+docker = {version = "^6.1.2", optional = true}
 betfair_parser = {version = "==0.1.21", optional = true}
 
 [tool.poetry.extras]
 betfair = ["betfair_parser"]
 docker = ["docker"]
 ib = ["ib_insync"]
 redis = ["hiredis", "redis"]
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
-isort = "^5.12.0"
-mypy = "^1.2.0"
-pre-commit = "^3.3.1"
-ruff = "^0.0.264"
+mypy = "^1.3.0"
+pre-commit = "^3.3.2"
+ruff = "^0.0.269"
 types-pytz = "^2022.3.0"
-types-redis = "^4.5.4"
+types-redis = "^4.5.5"
 types-requests = "^2.29.0"
 types-toml = "^0.10.2"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 coverage = "^7.2.5"
 pytest = "^7.3.1"
 pytest-aiohttp = "^1.0.4"
 pytest-asyncio = "^0.21.0"
 pytest-benchmark = "^4.0.0"
 pytest-cov = "4.0.0"
 pytest-mock = "^3.10.0"
-pytest-xdist = { version = "^3.2.1", extras = ["psutil"] }
+pytest-xdist = { version = "^3.3.1", extras = ["psutil"] }
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 numpydoc = "^1.5.0"
 linkify-it-py = "^2.0.0"
@@ -136,36 +132,43 @@
 target_version = ["py39", "py310", "py311"]
 line_length = 100
 
 ##########################################################
 # Linter configs                                         #
 ##########################################################
 [tool.ruff]
+target-version = "py39"
+line-length = 150  # Reduce to 100
 select = [
+    "C4",
     "E",
     "F",
     "W",
     "C90",
     "D",
+    # "DTZ",
     "UP",
     "S",
     "T10",
     "ICN",
+    "PIE",
+    # "PT",
     "PYI",
     "Q",
-    # "I",
+    "I",
     "RSE",
     "TID",
+    # "SIM",
     # "ARG",
     # "ERA",
     # "PD",
     # "PGH",
     # "PLW",
     "NPY",
-    # "RUF",
+    "RUF",
 ]
 
 ignore = [
     "E741",  # Ambiguous variable name (single char)
     "D100",  # Missing docstring in public module  **fix**
     "D101",
     "D102",  # Missing docstring in public method  **fix**
@@ -184,15 +187,40 @@
     "S101",  # Use of assert detected (OK in test suite)
     "S105",  # Use of hardcoded password (spurious)
     "S106",  # Use of hardcoded password (spurious)
     "S113",  # Probable use of requests call without timeout **fix**
 ]
 
 # Allow autofix for all enabled rules (when `--fix`) is provided
-fixable = ["A", "B", "C", "D", "E", "F"]
+fixable = [
+    "A",
+    "B",
+    "C",
+    "C4",
+    "D",
+    "DTZ",
+    "E",
+    "F",
+    "UP",
+    "S",
+    "W",
+    "I",
+    "PIE",
+    "PT",
+    "PYI",
+    "RSE",
+    "TID",
+    "ARG",
+    "PD",
+    "SIM",
+    # "PGH",
+    "NPY",
+    "RUF",
+]
+
 unfixable = []
 
 exclude = [
     ".benchmarks",
     ".eggs",
     ".git",
     ".mypy_cache",
@@ -200,21 +228,17 @@
     ".ruff_cache",
     ".venv",
     "build",
     "dist",
     "venv",
 ]
 
-line-length = 150  # Reduce to 100
-
 # Allow unused variables when underscore-prefixed.
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 
-target-version = "py39"
-
 [tool.ruff.isort]
 combine-as-imports = true
 force-single-line = true
 single-line-exclusions = ["typing"]
 lines-after-imports = 2
 split-on-trailing-comma = true
```

### Comparing `nautilus_trader-1.173.0/PKG-INFO` & `nautilus_trader-1.174.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nautilus-trader
-Version: 1.173.0
+Version: 1.174.0
 Summary: A high-performance algorithmic trading platform and event-driven backtester
 Home-page: https://nautilustrader.io
 License: LGPL-3.0-or-later
 Author: Nautech Systems
 Author-email: info@nautechsystems.io
 Requires-Python: >=3.9,<3.12
 Classifier: Development Status :: 4 - Beta
@@ -13,43 +13,40 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: betfair
 Provides-Extra: docker
 Provides-Extra: ib
 Provides-Extra: redis
 Requires-Dist: aiodns (>=3.0.0,<4.0.0)
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: betfair_parser (==0.1.21) ; extra == "betfair"
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: cython (==3.0.0b2)
-Requires-Dist: docker (>=6.0.1,<7.0.0) ; extra == "docker"
+Requires-Dist: docker (>=6.1.2,<7.0.0) ; extra == "docker"
 Requires-Dist: frozendict (>=2.3.8,<3.0.0)
 Requires-Dist: fsspec (>=2022.5.0)
 Requires-Dist: hiredis (>=2.2.3,<3.0.0) ; extra == "redis"
-Requires-Dist: ib_insync (>=0.9.83,<0.10.0) ; extra == "ib"
+Requires-Dist: ib_insync (>=0.9.85,<0.10.0) ; extra == "ib"
 Requires-Dist: msgspec (>=0.14.2,<0.15.0)
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: psutil (>=5.9.5,<6.0.0)
-Requires-Dist: pyarrow (>=10.0.1,<11.0.0)
+Requires-Dist: pyarrow (>=12.0.0,<13.0.0)
 Requires-Dist: pytz (>=2023.3.0,<2024.0.0)
-Requires-Dist: redis (>=4.5.4,<5.0.0) ; extra == "redis"
+Requires-Dist: redis (>=4.5.5,<5.0.0) ; extra == "redis"
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: uvloop (>=0.17.0,<0.18.0) ; sys_platform != "win32"
 Project-URL: Repository, https://github.com/nautechsystems/nautilus_trader
 Description-Content-Type: text/markdown
```

