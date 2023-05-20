# Comparing `tmp/pyvrp-0.2.1.tar.gz` & `tmp/pyvrp-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvrp-0.2.1.tar", max compression
+gzip compressed data, was "pyvrp-0.3.0.tar", max compression
```

## Comparing `pyvrp-0.2.1.tar` & `pyvrp-0.3.0.tar`

### file list

```diff
@@ -1,162 +1,160 @@
--rw-r--r--   0        0        0     1082 2023-05-13 19:41:45.381572 pyvrp-0.2.1/LICENSE
--rw-r--r--   0        0        0     2102 2023-05-13 19:41:45.381572 pyvrp-0.2.1/README.md
--rw-r--r--   0        0        0     3248 2023-05-13 19:41:45.381572 pyvrp-0.2.1/build_extensions.py
--rw-r--r--   0        0        0     4855 2023-05-13 19:41:45.405573 pyvrp-0.2.1/meson.build
--rw-r--r--   0        0        0      150 2023-05-13 19:41:45.405573 pyvrp-0.2.1/meson_options.txt
--rw-r--r--   0        0        0     3502 2023-05-13 19:41:45.405573 pyvrp-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     7123 2023-05-13 19:41:45.405573 pyvrp-0.2.1/pyvrp/GeneticAlgorithm.py
--rw-r--r--   0        0        0     8810 2023-05-13 19:41:45.405573 pyvrp-0.2.1/pyvrp/PenaltyManager.py
--rw-r--r--   0        0        0     6144 2023-05-13 19:41:45.405573 pyvrp-0.2.1/pyvrp/Population.py
--rw-r--r--   0        0        0     2872 2023-05-13 19:41:45.405573 pyvrp-0.2.1/pyvrp/Result.py
--rw-r--r--   0        0        0     6197 2023-05-13 19:41:45.405573 pyvrp-0.2.1/pyvrp/Statistics.py
--rw-r--r--   0        0        0      799 2023-05-13 19:41:45.405573 pyvrp-0.2.1/pyvrp/_CostEvaluator.pyi
--rw-r--r--   0        0        0     4129 2023-05-13 19:41:45.405573 pyvrp-0.2.1/pyvrp/_Individual.pyi
--rw-r--r--   0        0        0      465 2023-05-13 19:41:45.405573 pyvrp-0.2.1/pyvrp/_Matrix.pyi
--rw-r--r--   0        0        0     4877 2023-05-13 19:41:45.405573 pyvrp-0.2.1/pyvrp/_ProblemData.pyi
--rw-r--r--   0        0        0     4021 2023-05-13 19:41:45.405573 pyvrp-0.2.1/pyvrp/_SubPopulation.pyi
--rw-r--r--   0        0        0     1885 2023-05-13 19:41:45.405573 pyvrp-0.2.1/pyvrp/_TimeWindowSegment.pyi
--rw-r--r--   0        0        0      267 2023-05-13 19:41:45.405573 pyvrp-0.2.1/pyvrp/_XorShift128.pyi
--rw-r--r--   0        0        0      513 2023-05-13 19:41:45.405573 pyvrp-0.2.1/pyvrp/__init__.py
--rw-r--r--   0        0        0     8916 2023-05-13 19:41:45.405573 pyvrp-0.2.1/pyvrp/cli.py
--rw-r--r--   0        0        0      715 2023-05-13 19:41:45.405573 pyvrp-0.2.1/pyvrp/cpp/CostEvaluator.cpp
--rw-r--r--   0        0        0     2194 2023-05-13 19:41:45.405573 pyvrp-0.2.1/pyvrp/cpp/CostEvaluator.h
--rw-r--r--   0        0        0      711 2023-05-13 19:41:45.405573 pyvrp-0.2.1/pyvrp/cpp/CostEvaluator_bindings.cpp
--rw-r--r--   0        0        0     6093 2023-05-13 19:41:45.405573 pyvrp-0.2.1/pyvrp/cpp/Individual.cpp
--rw-r--r--   0        0        0     3819 2023-05-13 19:41:45.405573 pyvrp-0.2.1/pyvrp/cpp/Individual.h
--rw-r--r--   0        0        0     2291 2023-05-13 19:41:45.405573 pyvrp-0.2.1/pyvrp/cpp/Individual_bindings.cpp
--rw-r--r--   0        0        0     2484 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/cpp/Matrix.h
--rw-r--r--   0        0        0      909 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/cpp/Matrix_bindings.cpp
--rw-r--r--   0        0        0     1565 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/cpp/ProblemData.cpp
--rw-r--r--   0        0        0     3605 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/cpp/ProblemData.h
--rw-r--r--   0        0        0     2246 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/cpp/ProblemData_bindings.cpp
--rw-r--r--   0        0        0      574 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/cpp/README.md
--rw-r--r--   0        0        0     4784 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/cpp/SubPopulation.cpp
--rw-r--r--   0        0        0     3115 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/cpp/SubPopulation.h
--rw-r--r--   0        0        0     2750 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/cpp/SubPopulation_bindings.cpp
--rw-r--r--   0        0        0     3349 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/cpp/TimeWindowSegment.h
--rw-r--r--   0        0        0     1215 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/cpp/TimeWindowSegment_bindings.cpp
--rw-r--r--   0        0        0      581 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/cpp/XorShift128.cpp
--rw-r--r--   0        0        0     2017 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/cpp/XorShift128.h
--rw-r--r--   0        0        0      467 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/cpp/XorShift128_bindings.cpp
--rw-r--r--   0        0        0     2822 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/cpp/crossover/crossover.cpp
--rw-r--r--   0        0        0     1925 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/cpp/crossover/crossover.h
--rw-r--r--   0        0        0     8549 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/cpp/crossover/selective_route_exchange.cpp
--rw-r--r--   0        0        0      375 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/cpp/crossover/selective_route_exchange_bindings.cpp
--rw-r--r--   0        0        0     1007 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/cpp/diversity/broken_pairs_distance.cpp
--rw-r--r--   0        0        0      254 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/cpp/diversity/broken_pairs_distance_bindings.cpp
--rw-r--r--   0        0        0      659 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/cpp/diversity/diversity.h
--rw-r--r--   0        0        0     3011 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/cpp/educate/CircleSector.h
--rw-r--r--   0        0        0    11332 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/cpp/educate/Exchange.h
--rw-r--r--   0        0        0     2173 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/cpp/educate/Exchange_bindings.cpp
--rw-r--r--   0        0        0    10040 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/cpp/educate/LocalSearch.cpp
--rw-r--r--   0        0        0     3281 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/cpp/educate/LocalSearch.h
--rw-r--r--   0        0        0     2513 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/cpp/educate/LocalSearchOperator.h
--rw-r--r--   0        0        0     1420 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/cpp/educate/LocalSearch_bindings.cpp
--rw-r--r--   0        0        0     3633 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/cpp/educate/MoveTwoClientsReversed.cpp
--rw-r--r--   0        0        0      481 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/cpp/educate/MoveTwoClientsReversed.h
--rw-r--r--   0        0        0      482 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/cpp/educate/MoveTwoClientsReversed_bindings.cpp
--rw-r--r--   0        0        0      669 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/cpp/educate/Node.cpp
--rw-r--r--   0        0        0     1561 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/cpp/educate/Node.h
--rw-r--r--   0        0        0     1112 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/cpp/educate/RelocateStar.cpp
--rw-r--r--   0        0        0      735 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/cpp/educate/RelocateStar.h
--rw-r--r--   0        0        0      436 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/cpp/educate/RelocateStar_bindings.cpp
--rw-r--r--   0        0        0     3651 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/cpp/educate/Route.cpp
--rw-r--r--   0        0        0     4897 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/cpp/educate/Route.h
--rw-r--r--   0        0        0    10591 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/cpp/educate/SwapStar.cpp
--rw-r--r--   0        0        0     3186 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/cpp/educate/SwapStar.h
--rw-r--r--   0        0        0      420 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/cpp/educate/SwapStar_bindings.cpp
--rw-r--r--   0        0        0     4113 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/cpp/educate/TwoOpt.cpp
--rw-r--r--   0        0        0      895 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/cpp/educate/TwoOpt.h
--rw-r--r--   0        0        0      409 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/cpp/educate/TwoOpt_bindings.cpp
--rw-r--r--   0        0        0       63 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/crossover/__init__.py
--rw-r--r--   0        0        0      374 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/crossover/_selective_route_exchange.pyi
--rw-r--r--   0        0        0     1853 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/crossover/selective_route_exchange.py
--rw-r--r--   0        0        0     8425 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/crossover/tests/test_selective_route_exchange.py
--rw-r--r--   0        0        0      115 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/diagnostics/__init__.py
--rw-r--r--   0        0        0     3825 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/diagnostics/get_route_statistics.py
--rw-r--r--   0        0        0        0 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/diagnostics/tests/__init__.py
--rw-r--r--   0        0        0        7 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/diagnostics/tests/test_get_route_statistics.py
--rw-r--r--   0        0        0       58 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/diversity/__init__.py
--rw-r--r--   0        0        0     1462 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/diversity/_broken_pairs_distance.pyi
--rw-r--r--   0        0        0     1305 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/diversity/tests/test_broken_pairs_distance.py
--rw-r--r--   0        0        0     6601 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/educate/LocalSearch.py
--rw-r--r--   0        0        0      896 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/educate/_Exchange.pyi
--rw-r--r--   0        0        0      880 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/educate/_LocalSearch.pyi
--rw-r--r--   0        0        0      204 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/educate/_MoveTwoClientsReversed.pyi
--rw-r--r--   0        0        0      196 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/educate/_RelocateStar.pyi
--rw-r--r--   0        0        0      192 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/educate/_SwapStar.pyi
--rw-r--r--   0        0        0      188 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/educate/_TwoOpt.pyi
--rw-r--r--   0        0        0      708 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/educate/__init__.py
--rw-r--r--   0        0        0     5045 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/educate/neighbourhood.py
--rw-r--r--   0        0        0        0 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/educate/tests/__init__.py
--rw-r--r--   0        0        0     9129 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/educate/tests/test_Exchange.py
--rw-r--r--   0        0        0     5461 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/educate/tests/test_LocalSearch.py
--rw-r--r--   0        0        0     2714 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/educate/tests/test_MoveTwoClientsReversed.py
--rw-r--r--   0        0        0     3145 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/educate/tests/test_RelocateStar.py
--rw-r--r--   0        0        0     3027 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/educate/tests/test_SwapStar.py
--rw-r--r--   0        0        0     2141 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/educate/tests/test_TwoOpt.py
--rw-r--r--   0        0        0     5350 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/educate/tests/test_neighbourhood.py
--rw-r--r--   0        0        0      206 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/exceptions.py
--rw-r--r--   0        0        0      436 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/plotting/__init__.py
--rw-r--r--   0        0        0     1106 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/plotting/plot_coordinates.py
--rw-r--r--   0        0        0     1046 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/plotting/plot_demands.py
--rw-r--r--   0        0        0     1199 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/plotting/plot_diversity.py
--rw-r--r--   0        0        0     1129 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/plotting/plot_instance.py
--rw-r--r--   0        0        0     2344 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/plotting/plot_objectives.py
--rw-r--r--   0        0        0     1608 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/plotting/plot_result.py
--rw-r--r--   0        0        0     4732 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/plotting/plot_route_schedule.py
--rw-r--r--   0        0        0     1136 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/plotting/plot_runtimes.py
--rw-r--r--   0        0        0     1844 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/plotting/plot_solution.py
--rw-r--r--   0        0        0     1226 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/plotting/plot_time_windows.py
--rw-r--r--   0        0        0        0 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/plotting/tests/__init__.py
--rw-r--r--   0        0        0    47981 2023-05-13 19:41:45.409572 pyvrp-0.2.1/pyvrp/plotting/tests/baseline_images/test_plotting/plot_instance.png
--rw-r--r--   0        0        0   141297 2023-05-13 19:41:45.413573 pyvrp-0.2.1/pyvrp/plotting/tests/baseline_images/test_plotting/plot_result.png
--rw-r--r--   0        0        0    35194 2023-05-13 19:41:45.413573 pyvrp-0.2.1/pyvrp/plotting/tests/baseline_images/test_plotting/plot_route_schedule.png
--rw-r--r--   0        0        0    25609 2023-05-13 19:41:45.413573 pyvrp-0.2.1/pyvrp/plotting/tests/baseline_images/test_plotting/plot_solution.png
--rw-r--r--   0        0        0    43058 2023-05-13 19:41:45.413573 pyvrp-0.2.1/pyvrp/plotting/tests/baseline_images/test_plotting/plot_solution_with_customers.png
--rw-r--r--   0        0        0     3108 2023-05-13 19:41:45.413573 pyvrp-0.2.1/pyvrp/plotting/tests/test_plotting.py
--rw-r--r--   0        0        0     5543 2023-05-13 19:41:45.413573 pyvrp-0.2.1/pyvrp/read.py
--rw-r--r--   0        0        0     1048 2023-05-13 19:41:45.413573 pyvrp-0.2.1/pyvrp/show_versions.py
--rw-r--r--   0        0        0      444 2023-05-13 19:41:45.413573 pyvrp-0.2.1/pyvrp/stop/MaxIterations.py
--rw-r--r--   0        0        0      589 2023-05-13 19:41:45.413573 pyvrp-0.2.1/pyvrp/stop/MaxRuntime.py
--rw-r--r--   0        0        0      819 2023-05-13 19:41:45.413573 pyvrp-0.2.1/pyvrp/stop/NoImprovement.py
--rw-r--r--   0        0        0      573 2023-05-13 19:41:45.413573 pyvrp-0.2.1/pyvrp/stop/StoppingCriterion.py
--rw-r--r--   0        0        0      575 2023-05-13 19:41:45.413573 pyvrp-0.2.1/pyvrp/stop/TimedNoImprovement.py
--rw-r--r--   0        0        0      217 2023-05-13 19:41:45.413573 pyvrp-0.2.1/pyvrp/stop/__init__.py
--rw-r--r--   0        0        0        0 2023-05-13 19:41:45.413573 pyvrp-0.2.1/pyvrp/stop/tests/__init__.py
--rw-r--r--   0        0        0      839 2023-05-13 19:41:45.413573 pyvrp-0.2.1/pyvrp/stop/tests/test_MaxIterations.py
--rw-r--r--   0        0        0     1031 2023-05-13 19:41:45.413573 pyvrp-0.2.1/pyvrp/stop/tests/test_MaxRuntime.py
--rw-r--r--   0        0        0     1777 2023-05-13 19:41:45.413573 pyvrp-0.2.1/pyvrp/stop/tests/test_NoImprovement.py
--rw-r--r--   0        0        0     1292 2023-05-13 19:41:45.413573 pyvrp-0.2.1/pyvrp/stop/tests/test_TimedNoImprovement.py
--rw-r--r--   0        0        0        0 2023-05-13 19:41:45.413573 pyvrp-0.2.1/pyvrp/tests/__init__.py
--rw-r--r--   0        0        0      189 2023-05-13 19:41:45.413573 pyvrp-0.2.1/pyvrp/tests/data/DepotNotOne.txt
--rw-r--r--   0        0        0      607 2023-05-13 19:41:45.413573 pyvrp-0.2.1/pyvrp/tests/data/E-n22-k4.txt
--rw-r--r--   0        0        0      671 2023-05-13 19:41:45.413573 pyvrp-0.2.1/pyvrp/tests/data/EdgeWeightsNoExplicit.txt
--rw-r--r--   0        0        0      668 2023-05-13 19:41:45.413573 pyvrp-0.2.1/pyvrp/tests/data/EdgeWeightsNotFullMatrix.txt
--rw-r--r--   0        0        0      389 2023-05-13 19:41:45.413573 pyvrp-0.2.1/pyvrp/tests/data/FileWithUnknownSection.txt
--rw-r--r--   0        0        0      191 2023-05-13 19:41:45.413573 pyvrp-0.2.1/pyvrp/tests/data/MoreThanOneDepot.txt
--rw-r--r--   0        0        0      371 2023-05-13 19:41:45.413573 pyvrp-0.2.1/pyvrp/tests/data/NonZeroDepotDemand.txt
--rw-r--r--   0        0        0      371 2023-05-13 19:41:45.413573 pyvrp-0.2.1/pyvrp/tests/data/NonZeroDepotOpenTimeWindow.txt
--rw-r--r--   0        0        0      371 2023-05-13 19:41:45.413573 pyvrp-0.2.1/pyvrp/tests/data/NonZeroDepotServiceDuration.txt
--rw-r--r--   0        0        0      675 2023-05-13 19:41:45.413573 pyvrp-0.2.1/pyvrp/tests/data/OkSmall.txt
--rw-r--r--   0        0        0      697 2023-05-13 19:41:45.413573 pyvrp-0.2.1/pyvrp/tests/data/OkSmallGreedyRepair.txt
--rw-r--r--   0        0        0      347 2023-05-13 19:41:45.413573 pyvrp-0.2.1/pyvrp/tests/data/RC208.sol
--rw-r--r--   0        0        0     7524 2023-05-13 19:41:45.413573 pyvrp-0.2.1/pyvrp/tests/data/RC208.txt
--rw-r--r--   0        0        0      369 2023-05-13 19:41:45.413573 pyvrp-0.2.1/pyvrp/tests/data/TimeWindowOpenLargerThanClose.txt
--rw-r--r--   0        0        0      187 2023-05-13 19:41:45.413573 pyvrp-0.2.1/pyvrp/tests/data/UnknownEdgeWeightFmt.txt
--rw-r--r--   0        0        0      154 2023-05-13 19:41:45.413573 pyvrp-0.2.1/pyvrp/tests/data/UnknownEdgeWeightType.txt
--rw-r--r--   0        0        0     1256 2023-05-13 19:41:45.413573 pyvrp-0.2.1/pyvrp/tests/helpers.py
--rw-r--r--   0        0        0     3914 2023-05-13 19:41:45.413573 pyvrp-0.2.1/pyvrp/tests/test_CostEvaluator.py
--rw-r--r--   0        0        0     7641 2023-05-13 19:41:45.413573 pyvrp-0.2.1/pyvrp/tests/test_GeneticAlgorithm.py
--rw-r--r--   0        0        0     8829 2023-05-13 19:41:45.413573 pyvrp-0.2.1/pyvrp/tests/test_Individual.py
--rw-r--r--   0        0        0     1190 2023-05-13 19:41:45.413573 pyvrp-0.2.1/pyvrp/tests/test_Matrix.py
--rw-r--r--   0        0        0     9864 2023-05-13 19:41:45.413573 pyvrp-0.2.1/pyvrp/tests/test_PenaltyManager.py
--rw-r--r--   0        0        0    12487 2023-05-13 19:41:45.413573 pyvrp-0.2.1/pyvrp/tests/test_Population.py
--rw-r--r--   0        0        0     3000 2023-05-13 19:41:45.413573 pyvrp-0.2.1/pyvrp/tests/test_ProblemData.py
--rw-r--r--   0        0        0     2743 2023-05-13 19:41:45.413573 pyvrp-0.2.1/pyvrp/tests/test_Result.py
--rw-r--r--   0        0        0     1148 2023-05-13 19:41:45.413573 pyvrp-0.2.1/pyvrp/tests/test_Statistics.py
--rw-r--r--   0        0        0     5918 2023-05-13 19:41:45.413573 pyvrp-0.2.1/pyvrp/tests/test_SubPopulation.py
--rw-r--r--   0        0        0     1913 2023-05-13 19:41:45.413573 pyvrp-0.2.1/pyvrp/tests/test_TimeWindowSegment.py
--rw-r--r--   0        0        0     1101 2023-05-13 19:41:45.413573 pyvrp-0.2.1/pyvrp/tests/test_XorShift128.py
--rw-r--r--   0        0        0     6306 2023-05-13 19:41:45.413573 pyvrp-0.2.1/pyvrp/tests/test_read.py
--rw-r--r--   0        0        0     3477 1970-01-01 00:00:00.000000 pyvrp-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-05-20 09:32:34.248392 pyvrp-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2102 2023-05-20 09:32:34.248392 pyvrp-0.3.0/README.md
+-rw-r--r--   0        0        0     3248 2023-05-20 09:32:34.248392 pyvrp-0.3.0/build_extensions.py
+-rw-r--r--   0        0        0     4855 2023-05-20 09:32:34.272393 pyvrp-0.3.0/meson.build
+-rw-r--r--   0        0        0      150 2023-05-20 09:32:34.272393 pyvrp-0.3.0/meson_options.txt
+-rw-r--r--   0        0        0     3503 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     7123 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/GeneticAlgorithm.py
+-rw-r--r--   0        0        0     8810 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/PenaltyManager.py
+-rw-r--r--   0        0        0     6686 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/Population.py
+-rw-r--r--   0        0        0     2928 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/Result.py
+-rw-r--r--   0        0        0     6197 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/Statistics.py
+-rw-r--r--   0        0        0     1391 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/_CostEvaluator.pyi
+-rw-r--r--   0        0        0     6101 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/_Individual.pyi
+-rw-r--r--   0        0        0      465 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/_Matrix.pyi
+-rw-r--r--   0        0        0     5128 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/_ProblemData.pyi
+-rw-r--r--   0        0        0     4086 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/_SubPopulation.pyi
+-rw-r--r--   0        0        0     1885 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/_TimeWindowSegment.pyi
+-rw-r--r--   0        0        0      267 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/_XorShift128.pyi
+-rw-r--r--   0        0        0      520 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/__init__.py
+-rw-r--r--   0        0        0     8916 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/cli.py
+-rw-r--r--   0        0        0      834 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/cpp/CostEvaluator.cpp
+-rw-r--r--   0        0        0     2201 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/cpp/CostEvaluator.h
+-rw-r--r--   0        0        0      711 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/cpp/CostEvaluator_bindings.cpp
+-rw-r--r--   0        0        0     8608 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/cpp/Individual.cpp
+-rw-r--r--   0        0        0     6297 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/cpp/Individual.h
+-rw-r--r--   0        0        0     4312 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/cpp/Individual_bindings.cpp
+-rw-r--r--   0        0        0     2484 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/cpp/Matrix.h
+-rw-r--r--   0        0        0      909 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/cpp/Matrix_bindings.cpp
+-rw-r--r--   0        0        0     1907 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/cpp/ProblemData.cpp
+-rw-r--r--   0        0        0     3828 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/cpp/ProblemData.h
+-rw-r--r--   0        0        0     2459 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/cpp/ProblemData_bindings.cpp
+-rw-r--r--   0        0        0      574 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/cpp/README.md
+-rw-r--r--   0        0        0     4784 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/cpp/SubPopulation.cpp
+-rw-r--r--   0        0        0     3115 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/cpp/SubPopulation.h
+-rw-r--r--   0        0        0     2750 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/cpp/SubPopulation_bindings.cpp
+-rw-r--r--   0        0        0     3349 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/cpp/TimeWindowSegment.h
+-rw-r--r--   0        0        0     1215 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/cpp/TimeWindowSegment_bindings.cpp
+-rw-r--r--   0        0        0      581 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/cpp/XorShift128.cpp
+-rw-r--r--   0        0        0     2017 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/cpp/XorShift128.h
+-rw-r--r--   0        0        0      467 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/cpp/XorShift128_bindings.cpp
+-rw-r--r--   0        0        0     2822 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/cpp/crossover/crossover.cpp
+-rw-r--r--   0        0        0     1925 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/cpp/crossover/crossover.h
+-rw-r--r--   0        0        0     8599 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/cpp/crossover/selective_route_exchange.cpp
+-rw-r--r--   0        0        0      375 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/cpp/crossover/selective_route_exchange_bindings.cpp
+-rw-r--r--   0        0        0     1007 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/cpp/diversity/broken_pairs_distance.cpp
+-rw-r--r--   0        0        0      254 2023-05-20 09:32:34.272393 pyvrp-0.3.0/pyvrp/cpp/diversity/broken_pairs_distance_bindings.cpp
+-rw-r--r--   0        0        0      659 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/cpp/diversity/diversity.h
+-rw-r--r--   0        0        0     3011 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/cpp/educate/CircleSector.h
+-rw-r--r--   0        0        0    11368 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/cpp/educate/Exchange.h
+-rw-r--r--   0        0        0     2173 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/cpp/educate/Exchange_bindings.cpp
+-rw-r--r--   0        0        0    13068 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/cpp/educate/LocalSearch.cpp
+-rw-r--r--   0        0        0     3613 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/cpp/educate/LocalSearch.h
+-rw-r--r--   0        0        0     2513 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/cpp/educate/LocalSearchOperator.h
+-rw-r--r--   0        0        0     1420 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/cpp/educate/LocalSearch_bindings.cpp
+-rw-r--r--   0        0        0     3688 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/cpp/educate/MoveTwoClientsReversed.cpp
+-rw-r--r--   0        0        0      481 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/cpp/educate/MoveTwoClientsReversed.h
+-rw-r--r--   0        0        0      482 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/cpp/educate/MoveTwoClientsReversed_bindings.cpp
+-rw-r--r--   0        0        0      970 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/cpp/educate/Node.cpp
+-rw-r--r--   0        0        0     1617 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/cpp/educate/Node.h
+-rw-r--r--   0        0        0     1112 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/cpp/educate/RelocateStar.cpp
+-rw-r--r--   0        0        0      735 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/cpp/educate/RelocateStar.h
+-rw-r--r--   0        0        0      436 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/cpp/educate/RelocateStar_bindings.cpp
+-rw-r--r--   0        0        0     3651 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/cpp/educate/Route.cpp
+-rw-r--r--   0        0        0     4933 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/cpp/educate/Route.h
+-rw-r--r--   0        0        0    10591 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/cpp/educate/SwapStar.cpp
+-rw-r--r--   0        0        0     3186 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/cpp/educate/SwapStar.h
+-rw-r--r--   0        0        0      420 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/cpp/educate/SwapStar_bindings.cpp
+-rw-r--r--   0        0        0     4113 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/cpp/educate/TwoOpt.cpp
+-rw-r--r--   0        0        0      895 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/cpp/educate/TwoOpt.h
+-rw-r--r--   0        0        0      409 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/cpp/educate/TwoOpt_bindings.cpp
+-rw-r--r--   0        0        0       63 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/crossover/__init__.py
+-rw-r--r--   0        0        0      374 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/crossover/_selective_route_exchange.pyi
+-rw-r--r--   0        0        0     1961 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/crossover/selective_route_exchange.py
+-rw-r--r--   0        0        0     8585 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/crossover/tests/test_selective_route_exchange.py
+-rw-r--r--   0        0        0       58 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/diversity/__init__.py
+-rw-r--r--   0        0        0     1462 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/diversity/_broken_pairs_distance.pyi
+-rw-r--r--   0        0        0     1305 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/diversity/tests/test_broken_pairs_distance.py
+-rw-r--r--   0        0        0     6601 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/educate/LocalSearch.py
+-rw-r--r--   0        0        0      896 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/educate/_Exchange.pyi
+-rw-r--r--   0        0        0      880 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/educate/_LocalSearch.pyi
+-rw-r--r--   0        0        0      204 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/educate/_MoveTwoClientsReversed.pyi
+-rw-r--r--   0        0        0      196 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/educate/_RelocateStar.pyi
+-rw-r--r--   0        0        0      192 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/educate/_SwapStar.pyi
+-rw-r--r--   0        0        0      188 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/educate/_TwoOpt.pyi
+-rw-r--r--   0        0        0      708 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/educate/__init__.py
+-rw-r--r--   0        0        0     5149 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/educate/neighbourhood.py
+-rw-r--r--   0        0        0        0 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/educate/tests/__init__.py
+-rw-r--r--   0        0        0     9154 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/educate/tests/test_Exchange.py
+-rw-r--r--   0        0        0     6376 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/educate/tests/test_LocalSearch.py
+-rw-r--r--   0        0        0     2735 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/educate/tests/test_MoveTwoClientsReversed.py
+-rw-r--r--   0        0        0     3145 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/educate/tests/test_RelocateStar.py
+-rw-r--r--   0        0        0     3027 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/educate/tests/test_SwapStar.py
+-rw-r--r--   0        0        0     2166 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/educate/tests/test_TwoOpt.py
+-rw-r--r--   0        0        0     6092 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/educate/tests/test_neighbourhood.py
+-rw-r--r--   0        0        0      392 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/exceptions.py
+-rw-r--r--   0        0        0      436 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/plotting/__init__.py
+-rw-r--r--   0        0        0     1106 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/plotting/plot_coordinates.py
+-rw-r--r--   0        0        0     1046 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/plotting/plot_demands.py
+-rw-r--r--   0        0        0     1199 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/plotting/plot_diversity.py
+-rw-r--r--   0        0        0     1129 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/plotting/plot_instance.py
+-rw-r--r--   0        0        0     2344 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/plotting/plot_objectives.py
+-rw-r--r--   0        0        0     1608 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/plotting/plot_result.py
+-rw-r--r--   0        0        0     4729 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/plotting/plot_route_schedule.py
+-rw-r--r--   0        0        0     1136 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/plotting/plot_runtimes.py
+-rw-r--r--   0        0        0     1844 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/plotting/plot_solution.py
+-rw-r--r--   0        0        0     1226 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/plotting/plot_time_windows.py
+-rw-r--r--   0        0        0        0 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/plotting/tests/__init__.py
+-rw-r--r--   0        0        0    47981 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/plotting/tests/baseline_images/test_plotting/plot_instance.png
+-rw-r--r--   0        0        0   141297 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/plotting/tests/baseline_images/test_plotting/plot_result.png
+-rw-r--r--   0        0        0    35194 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/plotting/tests/baseline_images/test_plotting/plot_route_schedule.png
+-rw-r--r--   0        0        0    25609 2023-05-20 09:32:34.276393 pyvrp-0.3.0/pyvrp/plotting/tests/baseline_images/test_plotting/plot_solution.png
+-rw-r--r--   0        0        0    43058 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/plotting/tests/baseline_images/test_plotting/plot_solution_with_customers.png
+-rw-r--r--   0        0        0     3108 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/plotting/tests/test_plotting.py
+-rw-r--r--   0        0        0     6047 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/read.py
+-rw-r--r--   0        0        0     1048 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/show_versions.py
+-rw-r--r--   0        0        0      444 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/stop/MaxIterations.py
+-rw-r--r--   0        0        0      589 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/stop/MaxRuntime.py
+-rw-r--r--   0        0        0      819 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/stop/NoImprovement.py
+-rw-r--r--   0        0        0      573 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/stop/StoppingCriterion.py
+-rw-r--r--   0        0        0      575 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/stop/TimedNoImprovement.py
+-rw-r--r--   0        0        0      217 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/stop/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/stop/tests/__init__.py
+-rw-r--r--   0        0        0      839 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/stop/tests/test_MaxIterations.py
+-rw-r--r--   0        0        0     1031 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/stop/tests/test_MaxRuntime.py
+-rw-r--r--   0        0        0     1777 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/stop/tests/test_NoImprovement.py
+-rw-r--r--   0        0        0     1292 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/stop/tests/test_TimedNoImprovement.py
+-rw-r--r--   0        0        0        0 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/__init__.py
+-rw-r--r--   0        0        0      189 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/data/DepotNotOne.txt
+-rw-r--r--   0        0        0      607 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/data/E-n22-k4.txt
+-rw-r--r--   0        0        0      671 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/data/EdgeWeightsNoExplicit.txt
+-rw-r--r--   0        0        0      668 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/data/EdgeWeightsNotFullMatrix.txt
+-rw-r--r--   0        0        0      389 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/data/FileWithUnknownSection.txt
+-rw-r--r--   0        0        0      191 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/data/MoreThanOneDepot.txt
+-rw-r--r--   0        0        0      371 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/data/NonZeroDepotDemand.txt
+-rw-r--r--   0        0        0      371 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/data/NonZeroDepotOpenTimeWindow.txt
+-rw-r--r--   0        0        0      371 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/data/NonZeroDepotServiceDuration.txt
+-rw-r--r--   0        0        0      675 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/data/OkSmall.txt
+-rw-r--r--   0        0        0      697 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/data/OkSmallGreedyRepair.txt
+-rw-r--r--   0        0        0      754 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/data/OkSmallPrizes.txt
+-rw-r--r--   0        0        0      347 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/data/RC208.sol
+-rw-r--r--   0        0        0     7524 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/data/RC208.txt
+-rw-r--r--   0        0        0      369 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/data/TimeWindowOpenLargerThanClose.txt
+-rw-r--r--   0        0        0      187 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/data/UnknownEdgeWeightFmt.txt
+-rw-r--r--   0        0        0      154 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/data/UnknownEdgeWeightType.txt
+-rw-r--r--   0        0        0     2005 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/data/p06-2-50.vrp
+-rw-r--r--   0        0        0     1256 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/helpers.py
+-rw-r--r--   0        0        0     4538 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/test_CostEvaluator.py
+-rw-r--r--   0        0        0     7641 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/test_GeneticAlgorithm.py
+-rw-r--r--   0        0        0    12058 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/test_Individual.py
+-rw-r--r--   0        0        0     1190 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/test_Matrix.py
+-rw-r--r--   0        0        0     9864 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/test_PenaltyManager.py
+-rw-r--r--   0        0        0    12857 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/test_Population.py
+-rw-r--r--   0        0        0     3222 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/test_ProblemData.py
+-rw-r--r--   0        0        0     2743 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/test_Result.py
+-rw-r--r--   0        0        0     1148 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/test_Statistics.py
+-rw-r--r--   0        0        0     5918 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/test_SubPopulation.py
+-rw-r--r--   0        0        0     1913 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/test_TimeWindowSegment.py
+-rw-r--r--   0        0        0     1101 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/test_XorShift128.py
+-rw-r--r--   0        0        0     6306 2023-05-20 09:32:34.280393 pyvrp-0.3.0/pyvrp/tests/test_read.py
+-rw-r--r--   0        0        0     3227 1970-01-01 00:00:00.000000 pyvrp-0.3.0/PKG-INFO
```

### Comparing `pyvrp-0.2.1/LICENSE` & `pyvrp-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/README.md` & `pyvrp-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/build_extensions.py` & `pyvrp-0.3.0/build_extensions.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/meson.build` & `pyvrp-0.3.0/meson.build`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyproject.toml` & `pyvrp-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyvrp"
-version = "0.2.1"
+version = "0.3.0"
 description = "A state-of-the-art vehicle routing problem solver."
 authors = [
     "Niels Wouda <nielswouda@gmail.com>",
     "Leon Lan <leon.lanyidong@gmail.com>",
     "Wouter Kool <wouter.kool@ortec.com>",
 ]
 license = "MIT"
@@ -65,15 +65,15 @@
 
 [tool.poetry.group.examples]
 optional = true
 
 
 [tool.poetry.group.examples.dependencies]
 jupyter = ">=1.0.0"
-pandas = ">=1.5.0"
+tabulate = "^0.9.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^2.20.0"
 pytest = ">=6.0.0"
 pytest-cov = ">=2.6.1"
 codecov = "*"
```

### Comparing `pyvrp-0.2.1/pyvrp/GeneticAlgorithm.py` & `pyvrp-0.3.0/pyvrp/GeneticAlgorithm.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/PenaltyManager.py` & `pyvrp-0.3.0/pyvrp/PenaltyManager.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/Population.py` & `pyvrp-0.3.0/pyvrp/Population.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from __future__ import annotations
 
 from typing import Callable, Generator, Tuple
+from warnings import warn
 
 from ._CostEvaluator import CostEvaluator
 from ._Individual import Individual
 from ._SubPopulation import PopulationParams, SubPopulation
 from ._XorShift128 import XorShift128
+from .exceptions import EmptySolutionWarning
 
 
 class Population:
     """
     Creates a Population instance.
 
     Parameters
@@ -100,15 +102,25 @@
         Parameters
         ----------
         individual
             Individual to add to the population.
         cost_evaluator
             CostEvaluator to use to compute the cost.
         """
-        # Note: the PenaltyManager is required here since adding an individual
+        if individual.num_clients() == 0:
+            msg = """
+            An empty solution is being added to the population. This typically
+            indicates that there is a significant difference between the values
+            of the prizes and the other objective terms, which hints at a data
+            problem. Note that not every part of PyVRP can work gracefully with
+            empty solutions.
+            """
+            warn(msg, EmptySolutionWarning)
+
+        # Note: the CostEvaluator is required here since adding an individual
         # may trigger a purge which needs to compute the biased fitness which
         # requires computing the cost.
         if individual.is_feasible():
             # Note: the feasible subpopulation actually doet not depend
             # on the penalty values but we use the same implementation.
             self._feas.add(individual, cost_evaluator)
         else:
```

### Comparing `pyvrp-0.2.1/pyvrp/Result.py` & `pyvrp-0.3.0/pyvrp/Result.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,14 +84,15 @@
 
     def __str__(self) -> str:
         obj_str = f"{self.cost():.2f}" if self.is_feasible() else "INFEASIBLE"
         summary = [
             "Solution results",
             "================",
             f"    # routes: {self.best.num_routes()}",
+            f"   # clients: {self.best.num_clients()}",
             f"   objective: {obj_str}",
             f"# iterations: {self.num_iterations}",
             f"    run-time: {self.runtime:.2f} seconds",
             "",
             "Routes",
             "------",
         ]
```

### Comparing `pyvrp-0.2.1/pyvrp/Statistics.py` & `pyvrp-0.3.0/pyvrp/Statistics.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/_Individual.pyi` & `pyvrp-0.3.0/pyvrp/_Individual.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,61 @@
-from typing import Any, Dict, List, Tuple
+from typing import Any, Dict, Iterator, List, Tuple
 
 from ._ProblemData import ProblemData
 from ._XorShift128 import XorShift128
 
+class Route:
+    """
+    A simple class that stores the route plan and some statistics.
+    """
+
+    def __init__(self, data: ProblemData, visits: List[int]) -> None: ...
+    def __getitem__(self, idx: int) -> int: ...
+    def __iter__(self) -> Iterator[int]: ...
+    def __len__(self) -> int: ...
+    def is_feasible(self) -> bool: ...
+    def has_excess_load(self) -> bool: ...
+    def has_time_warp(self) -> bool: ...
+    def demand(self) -> int:
+        """
+        Total client demand on this route.
+        """
+    def excess_load(self) -> int:
+        """
+        Demand in excess of the vehicle's capacity.
+        """
+    def distance(self) -> int:
+        """
+        Total distance travelled on this route.
+        """
+    def duration(self) -> int:
+        """
+        Total route duration, including waiting time.
+        """
+    def visits(self) -> List[int]:
+        """
+        Route visits, as a list of clients.
+        """
+    def service_duration(self) -> int:
+        """
+        Total duration of service on the route.
+        """
+    def time_warp(self) -> int:
+        """
+        Any time warp incurred along the route.
+        """
+    def wait_duration(self) -> int:
+        """
+        Total waiting duration on this route.
+        """
+    def prizes(self) -> int:
+        """
+        Total prize value collected on this route.
+        """
+
 class Individual:
     """
     The Individual class encodes VRP solutions.
 
     Parameters
     ----------
     data
@@ -54,32 +103,32 @@
 
         Returns
         -------
         list
             A list of ``(pred, succ)`` tuples that encode for each client their
             predecessor and successors in this individual's routes.
         """
-    def get_routes(self) -> List[List[int]]:
+    def get_routes(self) -> List[Route]:
         """
         The solution this individual encodes, as a list of routes.
 
         .. note::
 
            This list is of length
            :py:attr:`~pyvrp._ProblemData.ProblemData.num_vehicles`, but there
            could be a number of empty routes. These empty routes are all in the
            higher indices (guarantee). Use :meth:`~num_routes` to determine
            which of the lower indices contain non-empty routes.
 
         Returns
         -------
         list
-            A list of routes, where each route is a list of client numbers. The
-            routes each start and end at the depot (0), but that is implicit:
-            the depot is not part of the returned routes.
+            A list of routes. Each :class:`~pyvrp._Individual.Route` starts and
+            ends at the depot (0), but that is implicit: the depot is not part
+            of the returned routes.
         """
     def has_excess_load(self) -> bool:
         """
         Returns whether this individual violates capacity constraints.
 
         Returns
         -------
@@ -119,14 +168,32 @@
         Returns the total time warp load over all routes.
 
         Returns
         -------
         int
             Total time warp over all routes.
         """
+    def prizes(self) -> int:
+        """
+        Returns the total collected prize value over all routes.
+
+        Returns
+        -------
+        int
+            Value of collected prizes.
+        """
+    def uncollected_prizes(self) -> int:
+        """
+        Total prize value of all clients not visited in this solution.
+
+        Returns
+        -------
+        int
+            Value of uncollected prizes.
+        """
     def is_feasible(self) -> bool:
         """
         Whether this individual is feasible. This is a shorthand for checking
         :meth:`~has_excess_load` and :meth:`~has_time_warp` both return
         false.
 
         Returns
@@ -140,12 +207,21 @@
         Number of non-empty routes in this solution.
 
         Returns
         -------
         int
             Number of non-empty routes.
         """
+    def num_clients(self) -> int:
+        """
+        Number of clients in this solution.
+
+        Returns
+        -------
+        int
+            Number of clients in this solution.
+        """
     def __copy__(self) -> Individual: ...
     def __deepcopy__(self, memo: Dict) -> Individual: ...
     def __hash__(self) -> int: ...
     def __eq__(self, other: Any) -> bool: ...
     def __str__(self) -> str: ...
```

### Comparing `pyvrp-0.2.1/pyvrp/_ProblemData.pyi` & `pyvrp-0.3.0/pyvrp/_ProblemData.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -21,31 +21,39 @@
         visit the client for. Service should start (but not necessarily end)
         within the [:py:attr:`~tw_early`, :py:attr:`~tw_late`] interval.
         Default 0.
     tw_early
         Earliest time at which we can visit this client. Default 0.
     tw_late
         Latest time at which we can visit this client. Default 0.
+    prize
+        Prize collected by visiting this client. Default 0.
+    required
+        Whether this client must be part of a feasible solution. Default True.
     """
 
     x: int
     y: int
     demand: int
     service_duration: int
     tw_early: int
     tw_late: int
+    prize: int
+    required: bool
 
     def __init__(
         self,
         x: int,
         y: int,
         demand: int = 0,
         service_duration: int = 0,
         tw_early: int = 0,
         tw_late: int = 0,
+        prize: int = 0,
+        required: bool = True,
     ) -> None: ...
 
 class ProblemData:
     """
     Creates a problem data instance. This instance contains all information
     needed to solve the vehicle routing problem.
```

### Comparing `pyvrp-0.2.1/pyvrp/_SubPopulation.pyi` & `pyvrp-0.3.0/pyvrp/_SubPopulation.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-from typing import Iterator, List, Tuple
+from typing import Callable, Iterator
 
 from pyvrp._CostEvaluator import CostEvaluator
 from pyvrp._Individual import Individual
 
 class PopulationParams:
     generation_size: int
     lb_diversity: float
     min_pop_size: int
     nb_close: int
     nb_elite: int
     ub_diversity: float
     def __init__(
         self,
-        min_pop_size: int = ...,
-        generation_size: int = ...,
-        nb_elite: int = ...,
-        nb_close: int = ...,
-        lb_diversity: float = ...,
-        ub_diversity: float = ...,
+        min_pop_size: int = 25,
+        generation_size: int = 40,
+        nb_elite: int = 4,
+        nb_close: int = 5,
+        lb_diversity: float = 0.1,
+        ub_diversity: float = 0.5,
     ) -> None: ...
     @property
     def max_pop_size(self) -> int: ...
 
 class SubPopulation:
-    def __init__(self, diversity_op, params: PopulationParams) -> None:
+    def __init__(
+        self,
+        diversity_op: Callable[[Individual, Individual], float],
+        params: PopulationParams,
+    ) -> None:
         """
         Creates a SubPopulation instance.
 
         This subpopulation manages a number individuals, and initiates survivor
         selection (purging) when their number grows large. A subpopulation's
         individuals (and metadata) can be accessed via indexing and iteration.
         Each individual is stored as a tuple of type ``_Item``, which stores
```

### Comparing `pyvrp-0.2.1/pyvrp/_TimeWindowSegment.pyi` & `pyvrp-0.3.0/pyvrp/_TimeWindowSegment.pyi`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/__init__.py` & `pyvrp-0.3.0/pyvrp/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from .GeneticAlgorithm import GeneticAlgorithm, GeneticAlgorithmParams
 from .PenaltyManager import PenaltyManager, PenaltyParams
 from .Population import Population, PopulationParams
 from .Result import Result
 from .Statistics import Statistics
 from ._CostEvaluator import CostEvaluator
-from ._Individual import Individual
+from ._Individual import Individual, Route
 from ._Matrix import Matrix
 from ._ProblemData import Client, ProblemData
 from ._XorShift128 import XorShift128
 from .read import read, read_solution
 from .show_versions import show_versions
```

### Comparing `pyvrp-0.2.1/pyvrp/cli.py` & `pyvrp-0.3.0/pyvrp/cli.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/cpp/CostEvaluator.h` & `pyvrp-0.3.0/pyvrp/cpp/CostEvaluator.h`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
     /**
      * Computes the time warp penalty for the given time warp.
      */
     [[nodiscard]] inline unsigned int twPenalty(unsigned int timeWarp) const;
 
     /**
-     * Computes the objective (penalised cost) for a given individual.
+     * Computes a smoothed objective (penalised cost) for a given individual.
      */
     [[nodiscard]] unsigned int
     penalisedCost(Individual const &individual) const;
 
     /**
      * Computes the objective for a given individual. Returns the largest
      * representable cost value if the individual is infeasible.
```

### Comparing `pyvrp-0.2.1/pyvrp/cpp/CostEvaluator_bindings.cpp` & `pyvrp-0.3.0/pyvrp/cpp/CostEvaluator_bindings.cpp`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/cpp/Matrix.h` & `pyvrp-0.3.0/pyvrp/cpp/Matrix.h`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/cpp/Matrix_bindings.cpp` & `pyvrp-0.3.0/pyvrp/cpp/Matrix_bindings.cpp`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/cpp/ProblemData.cpp` & `pyvrp-0.3.0/pyvrp/cpp/ProblemData.cpp`

 * *Files 9% similar despite different names*

```diff
@@ -2,31 +2,42 @@
 
 #include <cmath>
 #include <fstream>
 #include <sstream>
 #include <string>
 #include <vector>
 
-ProblemData::Client::Client(
-    int x, int y, int demand, int serviceDuration, int twEarly, int twLate)
+ProblemData::Client::Client(int x,
+                            int y,
+                            int demand,
+                            int serviceDuration,
+                            int twEarly,
+                            int twLate,
+                            int prize,
+                            bool required)
     : x(x),
       y(y),
       demand(demand),
       serviceDuration(serviceDuration),
       twEarly(twEarly),
-      twLate(twLate)
+      twLate(twLate),
+      prize(prize),
+      required(required)
 {
     if (demand < 0)
         throw std::invalid_argument("demand must be >= 0");
 
     if (serviceDuration < 0)
         throw std::invalid_argument("service_duration must be >= 0");
 
     if (twEarly > twLate)
         throw std::invalid_argument("tw_early must be <= tw_late");
+
+    if (prize < 0)
+        throw std::invalid_argument("prize must be >= 0");
 }
 
 ProblemData::Client const &ProblemData::depot() const { return client(0); }
 
 Matrix<int> const &ProblemData::distanceMatrix() const { return dist_; }
 
 Matrix<int> const &ProblemData::durationMatrix() const { return dur_; }
```

### Comparing `pyvrp-0.2.1/pyvrp/cpp/ProblemData.h` & `pyvrp-0.3.0/pyvrp/cpp/ProblemData.h`

 * *Files 10% similar despite different names*

```diff
@@ -8,27 +8,31 @@
 #include <vector>
 
 class ProblemData
 {
 public:
     struct Client
     {
-        int x;                // Coordinate X
-        int y;                // Coordinate Y
-        int demand;           // Demand
-        int serviceDuration;  // Service duration
-        int twEarly;          // Earliest arrival (when using time windows)
-        int twLate;           // Latest arrival (when using time windows)
+        int x;                 // Coordinate X
+        int y;                 // Coordinate Y
+        int demand;            // Demand
+        int serviceDuration;   // Service duration
+        int twEarly;           // Earliest arrival (when using time windows)
+        int twLate;            // Latest arrival (when using time windows)
+        int prize = 0;         // Prize collected when visiting this client
+        bool required = true;  // Must this client be part of a solution?
 
         Client(int x,
                int y,
                int demand = 0,
                int serviceDuration = 0,
                int twEarly = 0,
-               int twLate = 0);
+               int twLate = 0,
+               int prize = 0,
+               bool required = true);
     };
 
 private:
     Matrix<int> const dist_;       // Distance matrix (+depot)
     Matrix<int> const dur_;        // Duration matrix (+depot)
     std::vector<Client> clients_;  // Client (+depot) information
```

### Comparing `pyvrp-0.2.1/pyvrp/cpp/ProblemData_bindings.cpp` & `pyvrp-0.3.0/pyvrp/cpp/ProblemData_bindings.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -4,27 +4,31 @@
 #include <pybind11/stl.h>
 
 namespace py = pybind11;
 
 PYBIND11_MODULE(_ProblemData, m)
 {
     py::class_<ProblemData::Client>(m, "Client")
-        .def(py::init<int, int, int, int, int, int>(),
+        .def(py::init<int, int, int, int, int, int, int, bool>(),
              py::arg("x"),
              py::arg("y"),
              py::arg("demand") = 0,
              py::arg("service_duration") = 0,
              py::arg("tw_early") = 0,
-             py::arg("tw_late") = 0)
+             py::arg("tw_late") = 0,
+             py::arg("prize") = 0,
+             py::arg("required") = true)
         .def_readonly("x", &ProblemData::Client::x)
         .def_readonly("y", &ProblemData::Client::y)
         .def_readonly("service_duration", &ProblemData::Client::serviceDuration)
         .def_readonly("demand", &ProblemData::Client::demand)
         .def_readonly("tw_early", &ProblemData::Client::twEarly)
-        .def_readonly("tw_late", &ProblemData::Client::twLate);
+        .def_readonly("tw_late", &ProblemData::Client::twLate)
+        .def_readonly("prize", &ProblemData::Client::prize)
+        .def_readonly("required", &ProblemData::Client::required);
 
     py::class_<ProblemData>(m, "ProblemData")
         .def(py::init<std::vector<ProblemData::Client> const &,
                       int,
                       int,
                       std::vector<std::vector<int>> const &,
                       std::vector<std::vector<int>> const &>(),
```

### Comparing `pyvrp-0.2.1/pyvrp/cpp/README.md` & `pyvrp-0.3.0/pyvrp/cpp/README.md`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/cpp/SubPopulation.cpp` & `pyvrp-0.3.0/pyvrp/cpp/SubPopulation.cpp`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/cpp/SubPopulation.h` & `pyvrp-0.3.0/pyvrp/cpp/SubPopulation.h`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/cpp/SubPopulation_bindings.cpp` & `pyvrp-0.3.0/pyvrp/cpp/SubPopulation_bindings.cpp`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/cpp/TimeWindowSegment.h` & `pyvrp-0.3.0/pyvrp/cpp/TimeWindowSegment.h`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/cpp/TimeWindowSegment_bindings.cpp` & `pyvrp-0.3.0/pyvrp/cpp/TimeWindowSegment_bindings.cpp`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/cpp/XorShift128.cpp` & `pyvrp-0.3.0/pyvrp/cpp/XorShift128.cpp`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/cpp/XorShift128.h` & `pyvrp-0.3.0/pyvrp/cpp/XorShift128.h`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/cpp/crossover/crossover.cpp` & `pyvrp-0.3.0/pyvrp/cpp/crossover/crossover.cpp`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/cpp/crossover/crossover.h` & `pyvrp-0.3.0/pyvrp/cpp/crossover/crossover.h`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/cpp/crossover/selective_route_exchange.cpp` & `pyvrp-0.3.0/pyvrp/cpp/crossover/selective_route_exchange.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 #include <cmath>
 #include <unordered_set>
 
 using Client = int;
 using Clients = std::vector<Client>;
 using ClientSet = std::unordered_set<Client>;
-using Route = std::vector<Client>;
+using Route = Individual::Route;
 using Routes = std::vector<Route>;
 
 namespace
 {
 double routeAngle(ProblemData const &data, Route const &route)
 {
     // Computes the route angle center. Assumes that the route is non-empty.
@@ -198,16 +198,16 @@
 
     // Identify differences between route sets
     ClientSet clientsInSelectedBNotA;
     for (Client c : selectedB)
         if (!selectedA.contains(c))
             clientsInSelectedBNotA.insert(c);
 
-    Routes routes1(data.numVehicles());
-    Routes routes2(data.numVehicles());
+    std::vector<std::vector<Client>> routes1(data.numVehicles());
+    std::vector<std::vector<Client>> routes2(data.numVehicles());
 
     // Replace selected routes from parent A with routes from parent B
     for (size_t r = 0; r < numMovedRoutes; r++)
     {
         size_t indexA = (startA + r) % nRoutesA;
         size_t indexB = (startB + r) % nRoutesB;
```

### Comparing `pyvrp-0.2.1/pyvrp/cpp/diversity/broken_pairs_distance.cpp` & `pyvrp-0.3.0/pyvrp/cpp/diversity/broken_pairs_distance.cpp`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/cpp/diversity/diversity.h` & `pyvrp-0.3.0/pyvrp/cpp/diversity/diversity.h`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/cpp/educate/CircleSector.h` & `pyvrp-0.3.0/pyvrp/cpp/educate/CircleSector.h`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/cpp/educate/Exchange.h` & `pyvrp-0.3.0/pyvrp/cpp/educate/Exchange.h`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
 
         deltaCost += costEvaluator.loadPenalty(U->route->load() - loadDiff,
                                                data.vehicleCapacity());
         deltaCost -= costEvaluator.loadPenalty(U->route->load(),
                                                data.vehicleCapacity());
 
         if (deltaCost >= 0)    // if delta cost of just U's route is not enough
-            return deltaCost;  // even without V, the move will never be good
+            return deltaCost;  // even without V, the move will never be good.
 
         deltaCost += costEvaluator.loadPenalty(V->route->load() + loadDiff,
                                                data.vehicleCapacity());
         deltaCost -= costEvaluator.loadPenalty(V->route->load(),
                                                data.vehicleCapacity());
 
         auto vTWS = TWS::merge(data.durationMatrix(),
@@ -173,14 +173,16 @@
     auto const posU = U->position;
     auto const posV = V->position;
 
     assert(posU > 0 && posV > 0);
     auto *endU = N == 1 ? U : (*U->route)[posU + N - 1];
     auto *endV = M == 1 ? V : (*V->route)[posV + M - 1];
 
+    assert(U->route && V->route);
+
     int const current = U->route->distBetween(posU - 1, posU + N)
                         + V->route->distBetween(posV - 1, posV + M);
 
     int const proposed
         //   p(U) -> V -> ... -> endV -> n(endU)
         // + p(V) -> U -> ... -> endU -> n(endV)
         = data.dist(p(U)->client, V->client)
@@ -201,31 +203,31 @@
                                p(U)->twBefore,
                                V->route->twBetween(posV, posV + M - 1),
                                n(endU)->twAfter);
 
         deltaCost += costEvaluator.twPenalty(uTWS.totalTimeWarp());
         deltaCost -= costEvaluator.twPenalty(U->route->timeWarp());
 
-        auto vTWS = TWS::merge(data.durationMatrix(),
-                               p(V)->twBefore,
-                               U->route->twBetween(posU, posU + N - 1),
-                               n(endV)->twAfter);
-
-        deltaCost += costEvaluator.twPenalty(vTWS.totalTimeWarp());
-        deltaCost -= costEvaluator.twPenalty(V->route->timeWarp());
-
         auto const loadU = U->route->loadBetween(posU, posU + N - 1);
         auto const loadV = V->route->loadBetween(posV, posV + M - 1);
         auto const loadDiff = loadU - loadV;
 
         deltaCost += costEvaluator.loadPenalty(U->route->load() - loadDiff,
                                                data.vehicleCapacity());
         deltaCost -= costEvaluator.loadPenalty(U->route->load(),
                                                data.vehicleCapacity());
 
+        auto vTWS = TWS::merge(data.durationMatrix(),
+                               p(V)->twBefore,
+                               U->route->twBetween(posU, posU + N - 1),
+                               n(endV)->twAfter);
+
+        deltaCost += costEvaluator.twPenalty(vTWS.totalTimeWarp());
+        deltaCost -= costEvaluator.twPenalty(V->route->timeWarp());
+
         deltaCost += costEvaluator.loadPenalty(V->route->load() + loadDiff,
                                                data.vehicleCapacity());
         deltaCost -= costEvaluator.loadPenalty(V->route->load(),
                                                data.vehicleCapacity());
     }
     else  // within same route
     {
```

### Comparing `pyvrp-0.2.1/pyvrp/cpp/educate/Exchange_bindings.cpp` & `pyvrp-0.3.0/pyvrp/cpp/educate/Exchange_bindings.cpp`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/cpp/educate/LocalSearch.cpp` & `pyvrp-0.3.0/pyvrp/cpp/educate/LocalSearch.cpp`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 #include "LocalSearch.h"
+#include "TimeWindowSegment.h"
 
 #include <algorithm>
+#include <cassert>
 #include <numeric>
 #include <set>
 #include <stdexcept>
 #include <vector>
 
+using TWS = TimeWindowSegment;
+
 Individual LocalSearch::search(Individual &individual,
                                CostEvaluator const &costEvaluator)
 {
     loadIndividual(individual);
 
     // Shuffling the order beforehand adds diversity to the search
     std::shuffle(orderNodes.begin(), orderNodes.end(), rng);
@@ -31,46 +35,56 @@
     {
         searchCompleted = true;
 
         // Node operators are evaluated at neighbouring (U, V) pairs.
         for (auto const uClient : orderNodes)
         {
             auto *U = &clients[uClient];
+
             auto const lastTestedNode = lastTestedNodes[uClient];
             lastTestedNodes[uClient] = numMoves;
 
+            if (U->route && !data.client(uClient).required)  // test removing U
+                maybeRemove(U, costEvaluator);
+
             // Shuffling the neighbours in this loop should not matter much as
             // we are already randomizing the nodes U.
             for (auto const vClient : neighbours[uClient])
             {
                 auto *V = &clients[vClient];
 
+                if (!U->route && V->route)             // U might be inserted
+                    maybeInsert(U, V, costEvaluator);  // into V's route
+
+                if (!U->route || !V->route)  // we already tested inserting U,
+                    continue;                // so we can skip this move
+
                 if (lastModified[U->route->idx] > lastTestedNode
                     || lastModified[V->route->idx] > lastTestedNode)
                 {
                     if (applyNodeOps(U, V, costEvaluator))
                         continue;
 
                     if (p(V)->isDepot() && applyNodeOps(U, p(V), costEvaluator))
                         continue;
                 }
             }
 
-            // Empty route moves are not tested in the first iteration to avoid
-            // increasing the fleet size too much.
-            if (step > 0)
-            {
+            if (step > 0)  // empty moves are not tested initially to avoid
+            {              // using too many routes.
                 auto pred = [](auto const &route) { return route.empty(); };
                 auto empty = std::find_if(routes.begin(), routes.end(), pred);
 
                 if (empty == routes.end())
                     continue;
 
-                if (applyNodeOps(U, empty->depot, costEvaluator))
-                    continue;
+                if (U->route)  // try inserting U into the empty route.
+                    applyNodeOps(U, empty->depot, costEvaluator);
+                else  // U is not in the solution, so again try inserting.
+                    maybeInsert(U, empty->depot, costEvaluator);
             }
         }
     }
 
     return exportIndividual();
 }
 
@@ -168,14 +182,81 @@
 
             return true;
         }
 
     return false;
 }
 
+void LocalSearch::maybeInsert(Node *U,
+                              Node *V,
+                              CostEvaluator const &costEvaluator)
+{
+    assert(!U->route && V->route);
+
+    auto const &uClient = data.client(U->client);
+
+    int const current = data.dist(V->client, n(V)->client);
+    int const proposed = data.dist(V->client, U->client)
+                         + data.dist(U->client, n(V)->client) - uClient.prize;
+
+    int deltaCost = proposed - current;
+
+    deltaCost += costEvaluator.loadPenalty(V->route->load() + uClient.demand,
+                                           data.vehicleCapacity());
+    deltaCost
+        -= costEvaluator.loadPenalty(V->route->load(), data.vehicleCapacity());
+
+    if (deltaCost >= V->route->timeWarp())  // adding U will likely not lower
+        return;                             // time warp, so we can stop here.
+
+    auto vTWS
+        = TWS::merge(data.durationMatrix(), V->twBefore, U->tw, n(V)->twAfter);
+
+    deltaCost += costEvaluator.twPenalty(vTWS.totalTimeWarp());
+    deltaCost -= costEvaluator.twPenalty(V->route->timeWarp());
+
+    if (deltaCost < 0)
+    {
+        U->insertAfter(V);           // U has no route, so there's nothing to
+        update(V->route, V->route);  // update there.
+    }
+}
+
+void LocalSearch::maybeRemove(Node *U, CostEvaluator const &costEvaluator)
+{
+    assert(U->route);
+
+    auto const &uClient = data.client(U->client);
+
+    int const current = data.dist(p(U)->client, U->client)
+                        + data.dist(U->client, n(U)->client) - uClient.prize;
+
+    int const proposed = data.dist(p(U)->client, n(U)->client);
+
+    int deltaCost = proposed - current;
+
+    deltaCost += costEvaluator.loadPenalty(U->route->load() - uClient.demand,
+                                           data.vehicleCapacity());
+    deltaCost
+        -= costEvaluator.loadPenalty(U->route->load(), data.vehicleCapacity());
+
+    auto uTWS
+        = TWS::merge(data.durationMatrix(), p(U)->twBefore, n(U)->twAfter);
+
+    deltaCost += costEvaluator.twPenalty(uTWS.totalTimeWarp());
+    deltaCost -= costEvaluator.twPenalty(U->route->timeWarp());
+
+    if (deltaCost < 0)
+    {
+        auto *route = U->route;  // after U->remove(), U->route is a nullptr
+        U->remove();
+        update(route, route);
+    }
+}
+
 void LocalSearch::update(Route *U, Route *V)
 {
     numMoves++;
     searchCompleted = false;
 
     U->update();
     lastModified[U->idx] = numMoves;
@@ -186,24 +267,28 @@
         lastModified[V->idx] = numMoves;
     }
 }
 
 void LocalSearch::loadIndividual(Individual const &individual)
 {
     for (size_t client = 0; client <= data.numClients(); client++)
+    {
         clients[client].tw = {static_cast<int>(client),  // TODO cast
                               static_cast<int>(client),  // TODO cast
                               data.client(client).serviceDuration,
                               0,
                               data.client(client).twEarly,
                               data.client(client).twLate};
 
+        clients[client].route = nullptr;  // nullptr implies "not in solution"
+    }
+
     auto const &routesIndiv = individual.getRoutes();
 
-    for (size_t r = 0; r < data.numVehicles(); r++)
+    for (size_t r = 0; r != data.numVehicles(); r++)
     {
         Node *startDepot = &startDepots[r];
         Node *endDepot = &endDepots[r];
 
         startDepot->prev = endDepot;
         startDepot->next = endDepot;
 
@@ -222,19 +307,19 @@
         {
             Node *client = &clients[routesIndiv[r][0]];
             client->route = route;
 
             client->prev = startDepot;
             startDepot->next = client;
 
-            for (int i = 1; i < static_cast<int>(routesIndiv[r].size()); i++)
+            for (size_t idx = 1; idx < routesIndiv[r].size(); idx++)
             {
                 Node *prev = client;
 
-                client = &clients[routesIndiv[r][i]];
+                client = &clients[routesIndiv[r][idx]];
                 client->route = route;
 
                 client->prev = prev;
                 prev->next = client;
             }
 
             client->next = endDepot;
```

### Comparing `pyvrp-0.2.1/pyvrp/cpp/educate/LocalSearch.h` & `pyvrp-0.3.0/pyvrp/cpp/educate/LocalSearch.h`

 * *Files 6% similar despite different names*

```diff
@@ -44,23 +44,29 @@
 
     // Load an initial solution that we will attempt to improve
     void loadIndividual(Individual const &individual);
 
     // Export the LS solution back into an individual
     Individual exportIndividual();
 
-    [[nodiscard]] bool
-    applyNodeOps(Node *U, Node *V, CostEvaluator const &costEvaluator);
+    // Tests the node pair (U, V).
+    bool applyNodeOps(Node *U, Node *V, CostEvaluator const &costEvaluator);
 
-    [[nodiscard]] bool
-    applyRouteOps(Route *U, Route *V, CostEvaluator const &costEvaluator);
+    // Tests the route pair (U, V).
+    bool applyRouteOps(Route *U, Route *V, CostEvaluator const &costEvaluator);
 
-    // Updates solution state after an improving local search move
+    // Updates solution state after an improving local search move.
     void update(Route *U, Route *V);
 
+    // Test inserting U after V. Called if U is not currently in the solution.
+    void maybeInsert(Node *U, Node *V, CostEvaluator const &costEvaluator);
+
+    // Test removing U from the solution. Called when U can be removed.
+    void maybeRemove(Node *U, CostEvaluator const &costEvaluator);
+
 public:
     /**
      * Adds a local search operator that works on node/client pairs U and V.
      */
     void addNodeOperator(NodeOp &op);
 
     /**
```

### Comparing `pyvrp-0.2.1/pyvrp/cpp/educate/LocalSearchOperator.h` & `pyvrp-0.3.0/pyvrp/cpp/educate/LocalSearchOperator.h`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/cpp/educate/LocalSearch_bindings.cpp` & `pyvrp-0.3.0/pyvrp/cpp/educate/LocalSearch_bindings.cpp`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/cpp/educate/MoveTwoClientsReversed.cpp` & `pyvrp-0.3.0/pyvrp/cpp/educate/MoveTwoClientsReversed.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 #include "MoveTwoClientsReversed.h"
 #include "Route.h"
 #include "TimeWindowSegment.h"
 
+#include <cassert>
+
 using TWS = TimeWindowSegment;
 
 int MoveTwoClientsReversed::evaluate(Node *U,
                                      Node *V,
                                      CostEvaluator const &costEvaluator)
 {
     if (U == n(V) || n(U) == V || n(U)->isDepot())
         return 0;
 
     auto const posU = U->position;
     auto const posV = V->position;
 
+    assert(U->route && V->route);
+
     int const current = U->route->distBetween(posU - 1, posU + 2)
                         + data.dist(V->client, n(V)->client);
     int const proposed = data.dist(p(U)->client, n(n(U))->client)
                          + data.dist(V->client, n(U)->client)
                          + data.dist(n(U)->client, U->client)
                          + data.dist(U->client, n(V)->client);
```

### Comparing `pyvrp-0.2.1/pyvrp/cpp/educate/Node.h` & `pyvrp-0.3.0/pyvrp/cpp/educate/Node.h`

 * *Files 16% similar despite different names*

```diff
@@ -2,17 +2,16 @@
 #define NODE_H
 
 #include "ProblemData.h"
 #include "TimeWindowSegment.h"
 
 class Route;
 
-class Node
+struct Node
 {
-public:               // TODO make fields private
     int client;       // Client represented with this node
     size_t position;  // Position in the route
     Node *next;       // Next node in the route order
     Node *prev;       // Previous node in the route order
     Route *route;     // Pointer towards the associated route
 
     // TODO can these data fields be moved to Route?
@@ -23,22 +22,27 @@
     TimeWindowSegment tw;        // TWS for individual node (client)
     TimeWindowSegment twBefore;  // TWS for (0...client) including self
     TimeWindowSegment twAfter;   // TWS for (client...0) including self
 
     [[nodiscard]] inline bool isDepot() const;
 
     /**
-     * Inserts this node after the other and updates the solution.
+     * Inserts this node after the other and updates the relevant links.
      */
     void insertAfter(Node *other);
 
     /**
-     * Swaps this node with the other and updates the solution.
+     * Swaps this node with the other and updates the relevant links.
      */
     void swapWith(Node *other);
+
+    /**
+     * Removes this node and updates the relevant links.
+     */
+    void remove();
 };
 
 bool Node::isDepot() const { return client == 0; }
 
 /**
  * Convenience method accessing the node directly before the argument.
  */
```

### Comparing `pyvrp-0.2.1/pyvrp/cpp/educate/RelocateStar.cpp` & `pyvrp-0.3.0/pyvrp/cpp/educate/RelocateStar.cpp`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/cpp/educate/RelocateStar.h` & `pyvrp-0.3.0/pyvrp/cpp/educate/RelocateStar.h`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/cpp/educate/Route.cpp` & `pyvrp-0.3.0/pyvrp/cpp/educate/Route.cpp`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/cpp/educate/Route.h` & `pyvrp-0.3.0/pyvrp/cpp/educate/Route.h`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,15 @@
 size_t Route::size() const
 {
     return nodes.size() - 1;  // exclude end depot
 }
 
 TimeWindowSegment Route::twBetween(size_t start, size_t end) const
 {
-    assert(start <= end);
+    assert(0 < start && start <= end && end <= nodes.size());
 
     auto tws = nodes[start - 1]->tw;
 
     for (size_t step = start; step != end; ++step)
         tws = TimeWindowSegment::merge(
             data.durationMatrix(), tws, nodes[step]->tw);
```

### Comparing `pyvrp-0.2.1/pyvrp/cpp/educate/SwapStar.cpp` & `pyvrp-0.3.0/pyvrp/cpp/educate/SwapStar.cpp`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/cpp/educate/SwapStar.h` & `pyvrp-0.3.0/pyvrp/cpp/educate/SwapStar.h`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/cpp/educate/TwoOpt.cpp` & `pyvrp-0.3.0/pyvrp/cpp/educate/TwoOpt.cpp`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/cpp/educate/TwoOpt.h` & `pyvrp-0.3.0/pyvrp/cpp/educate/TwoOpt.h`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/crossover/selective_route_exchange.py` & `pyvrp-0.3.0/pyvrp/crossover/selective_route_exchange.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,14 +44,17 @@
            Exchange Crossover. *Parallel Problem Solving from Nature*, PPSN XI,
            536 - 545.
     """
     first, second = parents
 
     idx1 = rng.randint(first.num_routes())
     idx2 = idx1 if idx1 < second.num_routes() else 0
-
     max_routes_to_move = min(first.num_routes(), second.num_routes())
-    num_routes_to_move = rng.randint(max_routes_to_move) + 1  # at least one
+
+    if max_routes_to_move == 0:  # rng.randint() cannot be called in this case
+        num_routes_to_move = 1
+    else:
+        num_routes_to_move = rng.randint(max_routes_to_move) + 1
 
     return _srex(
         parents, data, cost_evaluator, (idx1, idx2), num_routes_to_move
     )
```

### Comparing `pyvrp-0.2.1/pyvrp/crossover/tests/test_selective_route_exchange.py` & `pyvrp-0.3.0/pyvrp/crossover/tests/test_selective_route_exchange.py`

 * *Files 8% similar despite different names*

```diff
@@ -111,16 +111,16 @@
     # The start indices do not change because there are no improving moves.
     # So, indiv1's route [3, 4] will be replaced by indiv2's route [2, 3].
     # This results in two incomplete offspring [[2, 3], [1]] and [[3], [1, 2]],
     # which are both repaired using greedy repair. After repair, we obtain the
     # offspring [[2, 3, 4], [1]] with cost 8188, and [[3, 4], [1, 2]] with
     # cost 9725. The first one is returned since it has the lowest cost.
     offspring = cpp_srex((indiv1, indiv2), data, cost_evaluator, (0, 0), 1)
-
-    assert_equal(offspring.get_routes(), [[2, 3, 4], [1], []])
+    expected = Individual(data, [[2, 3, 4], [1]])
+    assert_equal(offspring, expected)
 
 
 def test_srex_changed_start_indices():
     """
     Tests the case where the initial start indices are changed in SREX.
     """
     data = read("data/OkSmall.txt")
@@ -137,16 +137,16 @@
     # idx2 = 1. There are no improving moves in this position since the
     # difference for A to move is 1 and difference for B to move is 1.
     # So, indiv1's route [4] will be replaced by indiv2's route [1, 2, 4].
     # This results in two candidate offspring, [[1, 2, 4], [3]] with cost
     # 10195, and [[4], [1, 2, 3]] with cost 31029. The first candidate is
     # returned since it has the lowest cost.
     offspring = cpp_srex((indiv1, indiv2), data, cost_evaluator, (1, 1), 1)
-
-    assert_equal(offspring.get_routes(), [[1, 2, 4], [3], []])
+    expected = Individual(data, [[1, 2, 4], [3]])
+    assert_equal(offspring, expected)
 
 
 def test_srex_a_right_move():
     """
     Tests the case where the initial start indices are changed by moving the
     A index to the right.
     """
@@ -184,16 +184,16 @@
     #
     # No more improving moves.
     #
     # Candidate offspring
     # [4, 1] [2] [3] - cost: 12699 <-- selected as new offspring
     # [4] [2] [1, 3] - cost: 24416
     offspring = cpp_srex((indiv1, indiv2), data, cost_evaluator, (2, 2), 1)
-
-    assert_equal(offspring.get_routes(), [[4, 1], [2], [3]])
+    expected = Individual(data, [[4, 1], [2], [3]])
+    assert_equal(offspring, expected)
 
 
 def test_srex_a_left_move():
     """
     Tests the case where the initial start indices are changed by moving to
     A index to the left.
     """
@@ -201,16 +201,16 @@
     cost_evaluator = CostEvaluator(20, 6)
 
     # We create the routes sorted by angle such that SREX sorting doesn't
     # affect them
     indiv1 = Individual(data, [[4], [2], [1, 3]])
     indiv2 = Individual(data, [[3], [4], [2, 1]])
     offspring = cpp_srex((indiv1, indiv2), data, cost_evaluator, (2, 2), 1)
-
-    assert_equal(offspring.get_routes(), [[4], [2, 1], [3]])
+    expected = Individual(data, [[4], [2, 1], [3]])
+    assert_equal(offspring, expected)
 
 
 def test_srex_b_left_move():
     """
     Tests the case where the initial start indices are changed by moving the
     B index to the left.
     """
@@ -218,16 +218,16 @@
     cost_evaluator = CostEvaluator(20, 6)
 
     # We create the routes sorted by angle such that SREX sorting doesn't
     # affect them
     indiv1 = Individual(data, [[4], [2], [1, 3]])
     indiv2 = Individual(data, [[3], [2], [4, 1]])
     offspring = cpp_srex((indiv1, indiv2), data, cost_evaluator, (0, 0), 1)
-
-    assert_equal(offspring.get_routes(), [[4, 1], [2], [3]])
+    expected = Individual(data, [[4, 1], [2], [3]])
+    assert_equal(offspring, expected)
 
 
 def test_srex_b_right_move():
     """
     Tests the case where the initial start indices are changed by moving the
     B index to the right.
     """
@@ -235,9 +235,9 @@
     cost_evaluator = CostEvaluator(20, 6)
 
     # We create the routes sorted by angle such that SREX sorting doesn't
     # affect them
     indiv1 = Individual(data, [[4], [2], [1, 3]])
     indiv2 = Individual(data, [[3], [4], [2, 1]])
     offspring = cpp_srex((indiv1, indiv2), data, cost_evaluator, (0, 0), 1)
-
-    assert_equal(offspring.get_routes(), [[4], [2], [1, 3]])
+    expected = Individual(data, [[4], [2], [1, 3]])
+    assert_equal(offspring, expected)
```

### Comparing `pyvrp-0.2.1/pyvrp/diversity/_broken_pairs_distance.pyi` & `pyvrp-0.3.0/pyvrp/diversity/_broken_pairs_distance.pyi`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/diversity/tests/test_broken_pairs_distance.py` & `pyvrp-0.3.0/pyvrp/diversity/tests/test_broken_pairs_distance.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/educate/LocalSearch.py` & `pyvrp-0.3.0/pyvrp/educate/LocalSearch.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/educate/_Exchange.pyi` & `pyvrp-0.3.0/pyvrp/educate/_Exchange.pyi`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/educate/_LocalSearch.pyi` & `pyvrp-0.3.0/pyvrp/educate/_LocalSearch.pyi`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/educate/__init__.py` & `pyvrp-0.3.0/pyvrp/educate/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/educate/neighbourhood.py` & `pyvrp-0.3.0/pyvrp/educate/neighbourhood.py`

 * *Files 6% similar despite different names*

```diff
@@ -130,17 +130,18 @@
            hybrid genetic algorithm with adaptive diversity management for a
            large class of vehicle routing problems with time-windows.
            *Computers & Operations Research*, 40(1), 475 - 489.
     """
     dim = data.num_clients + 1
     clients = [data.client(idx) for idx in range(dim)]
 
-    earliest = np.array([cli.tw_early for cli in clients])
-    latest = np.array([cli.tw_late for cli in clients])
-    service = np.array([cli.service_duration for cli in clients])
+    earliest = np.array([client.tw_early for client in clients])
+    latest = np.array([client.tw_late for client in clients])
+    service = np.array([client.service_duration for client in clients])
+    prizes = np.array([client.prize for client in clients])
     durations = np.array(
         [[data.duration(i, j) for j in range(dim)] for i in range(dim)],
         dtype=float,
     )
 
     min_wait_time = np.maximum(
         earliest[None, :] - durations - service[:, None] - latest[:, None], 0
@@ -156,8 +157,9 @@
         dtype=float,
     )
 
     return (
         distances
         + weight_wait_time * min_wait_time
         + weight_time_warp * min_time_warp
+        - prizes[None, :]
     )
```

### Comparing `pyvrp-0.2.1/pyvrp/educate/tests/test_Exchange.py` & `pyvrp-0.3.0/pyvrp/educate/tests/test_Exchange.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,16 +170,17 @@
 
     nb_params = NeighbourhoodParams(nb_granular=data.num_clients)
     ls = LocalSearch(data, rng, compute_neighbours(data, nb_params))
     ls.add_node_operator(Exchange21(data))
 
     individual = Individual(data, [[1, 2], [3, 4]])
     improved_individual = ls.search(individual, cost_evaluator)
+    expected = Individual(data, [[3, 4, 2], [1]])
+    assert_equal(improved_individual, expected)
 
-    assert_equal(improved_individual.get_routes(), [[3, 4, 2], [1], []])
     current_cost = cost_evaluator.penalised_cost(individual)
     improved_cost = cost_evaluator.penalised_cost(improved_individual)
     assert_(improved_cost < current_cost)
 
 
 def test_relocate_after_depot_should_work():
     """
```

### Comparing `pyvrp-0.2.1/pyvrp/educate/tests/test_LocalSearch.py` & `pyvrp-0.3.0/pyvrp/educate/tests/test_LocalSearch.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from numpy.testing import assert_, assert_equal, assert_raises
 from pytest import mark
 
 from pyvrp import CostEvaluator, Individual, XorShift128
 from pyvrp.educate import (
+    Exchange10,
+    Exchange11,
     LocalSearch,
     NeighbourhoodParams,
     Neighbours,
     compute_neighbours,
 )
-from pyvrp.educate._Exchange import Exchange10
 from pyvrp.tests.helpers import read
 
 
 def test_local_search_raises_when_there_are_no_operators():
     data = read("data/OkSmall.txt")
     cost_evaluator = CostEvaluator(20, 6)
     rng = XorShift128(seed=42)
@@ -157,7 +158,33 @@
     # solution
     # (previously this was not the case since due to caching the current TW was
     # computed as being zero, causing the move to be evaluated as worse)
     cost_evaluator_tw = CostEvaluator(0, 1000)
     improved_indiv = ls.search(individual, cost_evaluator_tw)
     improved_cost = cost_evaluator_tw.penalised_cost(improved_indiv)
     assert_(improved_cost < cost_evaluator_tw.penalised_cost(individual))
+
+
+def test_prize_collecting():
+    """
+    Tests that local search works on a small prize-collecting instance.
+    """
+    data = read("data/p06-2-50.vrp", round_func="dimacs")
+    rng = XorShift128(seed=42)
+    cost_evaluator = CostEvaluator(1, 1)
+
+    individual = Individual.make_random(data, rng)
+    individual_cost = cost_evaluator.penalised_cost(individual)
+
+    # Random solutions are complete...
+    assert_equal(individual.num_clients(), data.num_clients)
+
+    ls = LocalSearch(data, rng, compute_neighbours(data))
+    ls.add_node_operator(Exchange10(data))  # relocate
+    ls.add_node_operator(Exchange11(data))  # swap
+
+    improved = ls.search(individual, cost_evaluator)
+    improved_cost = cost_evaluator.penalised_cost(improved)
+
+    # ...but an optimised prize-collecting solution is likely not complete.
+    assert_(improved.num_clients() < individual.num_clients())
+    assert_(improved_cost < individual_cost)
```

### Comparing `pyvrp-0.2.1/pyvrp/educate/tests/test_MoveTwoClientsReversed.py` & `pyvrp-0.3.0/pyvrp/educate/tests/test_MoveTwoClientsReversed.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,16 @@
     assert_equal(improved_individual.num_routes(), 1)
     current_cost = cost_evaluator.penalised_cost(individual)
     improved_cost = cost_evaluator.penalised_cost(improved_individual)
     assert_(improved_cost < current_cost)
 
     # (2, 3) was inserted after 1 as 1 -> 3 -> 2 -> 4. Then (1, 3) got inserted
     # after 4 as 2 -> 4 -> 3 -> 1.
-    assert_equal(improved_individual.get_routes(), [[2, 4, 3, 1], [], []])
+    expected = Individual(data, [[2, 4, 3, 1]])
+    assert_equal(improved_individual, expected)
 
     # These two-route solutions can all be created by MoveTwoClientsReversed
     # from the returned solution. So they must have a cost that's at best equal
     # to the returned solution's cost.
     for routes in ([[3, 1], [4, 2]], [[2, 1], [3, 4]], [[2, 4], [1, 3]]):
         other = Individual(data, routes)
         improved_cost = cost_evaluator.penalised_cost(improved_individual)
```

### Comparing `pyvrp-0.2.1/pyvrp/educate/tests/test_RelocateStar.py` & `pyvrp-0.3.0/pyvrp/educate/tests/test_RelocateStar.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/educate/tests/test_SwapStar.py` & `pyvrp-0.3.0/pyvrp/educate/tests/test_SwapStar.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/educate/tests/test_TwoOpt.py` & `pyvrp-0.3.0/pyvrp/educate/tests/test_TwoOpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,16 @@
     current_cost = cost_evaluator.penalised_cost(individual)
     improved_cost = cost_evaluator.penalised_cost(improved_individual)
     assert_(improved_cost < current_cost)
 
     # First improving (U, V) node pair is (1, 3), which results in the route
     # [1, 3, 2, 4]. The second improving node pair involves the depot of an
     # empty route: (1, 0). This results in routes [1] and [3, 2, 4].
-    assert_equal(improved_individual.get_routes(), [[1], [3, 2, 4], []])
+    expected = Individual(data, [[1], [3, 2, 4]])
+    assert_equal(improved_individual, expected)
 
 
 @mark.parametrize("seed", [2643, 2742, 2941, 3457, 4299, 4497, 6178, 6434])
 def test_RC208_instance(seed: int):
     data = read("data/RC208.txt", "solomon", "dimacs")
     cost_evaluator = CostEvaluator(20, 6)
     rng = XorShift128(seed=seed)
```

### Comparing `pyvrp-0.2.1/pyvrp/plotting/plot_coordinates.py` & `pyvrp-0.3.0/pyvrp/plotting/plot_coordinates.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/plotting/plot_demands.py` & `pyvrp-0.3.0/pyvrp/plotting/plot_demands.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/plotting/plot_diversity.py` & `pyvrp-0.3.0/pyvrp/plotting/plot_diversity.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/plotting/plot_instance.py` & `pyvrp-0.3.0/pyvrp/plotting/plot_instance.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/plotting/plot_objectives.py` & `pyvrp-0.3.0/pyvrp/plotting/plot_objectives.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/plotting/plot_result.py` & `pyvrp-0.3.0/pyvrp/plotting/plot_result.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/plotting/plot_route_schedule.py` & `pyvrp-0.3.0/pyvrp/plotting/plot_route_schedule.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from typing import List, Optional
+from typing import Optional
 
 import matplotlib.pyplot as plt
 import numpy as np
 from matplotlib.collections import LineCollection
 
-from pyvrp import ProblemData
+from pyvrp import ProblemData, Route
 
 
 def plot_route_schedule(
     data: ProblemData,
-    route: List[int],
+    route: Route,
     legend: bool = True,
     title: Optional[str] = None,
     ax: Optional[plt.Axes] = None,
 ):
     """
     Plots a route schedule. This function plots multiple time statistics
     as a function of distance traveled:
```

### Comparing `pyvrp-0.2.1/pyvrp/plotting/plot_runtimes.py` & `pyvrp-0.3.0/pyvrp/plotting/plot_runtimes.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/plotting/plot_solution.py` & `pyvrp-0.3.0/pyvrp/plotting/plot_solution.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/plotting/plot_time_windows.py` & `pyvrp-0.3.0/pyvrp/plotting/plot_time_windows.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/plotting/tests/baseline_images/test_plotting/plot_instance.png` & `pyvrp-0.3.0/pyvrp/plotting/tests/baseline_images/test_plotting/plot_instance.png`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/plotting/tests/baseline_images/test_plotting/plot_result.png` & `pyvrp-0.3.0/pyvrp/plotting/tests/baseline_images/test_plotting/plot_result.png`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/plotting/tests/baseline_images/test_plotting/plot_route_schedule.png` & `pyvrp-0.3.0/pyvrp/plotting/tests/baseline_images/test_plotting/plot_route_schedule.png`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/plotting/tests/baseline_images/test_plotting/plot_solution.png` & `pyvrp-0.3.0/pyvrp/plotting/tests/baseline_images/test_plotting/plot_solution.png`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/plotting/tests/baseline_images/test_plotting/plot_solution_with_customers.png` & `pyvrp-0.3.0/pyvrp/plotting/tests/baseline_images/test_plotting/plot_solution_with_customers.png`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/plotting/tests/test_plotting.py` & `pyvrp-0.3.0/pyvrp/plotting/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/read.py` & `pyvrp-0.3.0/pyvrp/read.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import functools
 import pathlib
+from numbers import Number
 from typing import Callable, Dict, List, Union
 
 import numpy as np
 import vrplib
 
 from ._ProblemData import Client, ProblemData
 
@@ -103,15 +104,21 @@
 
     if "node_coord" in instance:
         coords: np.ndarray = round_func(instance["node_coord"])
     else:
         coords = np.zeros((dimension, 2), dtype=int)
 
     if "service_time" in instance:
-        service_times: np.ndarray = round_func(instance["service_time"])
+        if isinstance(instance["service_time"], Number):
+            # Some instances describe a uniform service time as a single value
+            # that applies to all clients.
+            service_times = np.full(dimension, instance["service_time"], int)
+            service_times[0] = 0
+        else:
+            service_times = round_func(instance["service_time"])
     else:
         service_times = np.zeros(dimension, dtype=int)
 
     if "time_window" in instance:
         # VRPLIB instances typically do not have a duration data field, so we
         # assume duration == distance if the instance has time windows.
         durations = distances
@@ -119,14 +126,16 @@
     else:
         # No time window data. So the time window component is not relevant,
         # and we set all time-related fields to zero.
         durations = np.zeros_like(distances)
         service_times = np.zeros(dimension, dtype=int)
         time_windows = np.zeros((dimension, 2), dtype=int)
 
+    prizes = round_func(instance.get("prize", np.zeros(dimension, dtype=int)))
+
     # Checks
     if len(depots) != 1 or depots[0] != 0:
         raise ValueError(
             "Source file should contain single depot with index 1 "
             + "(depot index should be 0 after subtracting offset 1)"
         )
 
@@ -146,14 +155,16 @@
         Client(
             coords[idx][0],  # x
             coords[idx][1],  # y
             demands[idx],
             service_times[idx],
             time_windows[idx][0],  # TW early
             time_windows[idx][1],  # TW late
+            prizes[idx],
+            np.isclose(prizes[idx], 0),  # required only when prize is zero
         )
         for idx in range(dimension)
     ]
 
     return ProblemData(
         clients,
         num_vehicles,
```

### Comparing `pyvrp-0.2.1/pyvrp/show_versions.py` & `pyvrp-0.3.0/pyvrp/show_versions.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/stop/MaxRuntime.py` & `pyvrp-0.3.0/pyvrp/stop/MaxRuntime.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/stop/NoImprovement.py` & `pyvrp-0.3.0/pyvrp/stop/NoImprovement.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/stop/StoppingCriterion.py` & `pyvrp-0.3.0/pyvrp/stop/StoppingCriterion.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/stop/TimedNoImprovement.py` & `pyvrp-0.3.0/pyvrp/stop/TimedNoImprovement.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/stop/tests/test_MaxIterations.py` & `pyvrp-0.3.0/pyvrp/stop/tests/test_MaxIterations.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/stop/tests/test_MaxRuntime.py` & `pyvrp-0.3.0/pyvrp/stop/tests/test_MaxRuntime.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/stop/tests/test_NoImprovement.py` & `pyvrp-0.3.0/pyvrp/stop/tests/test_NoImprovement.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/stop/tests/test_TimedNoImprovement.py` & `pyvrp-0.3.0/pyvrp/stop/tests/test_TimedNoImprovement.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/tests/data/E-n22-k4.txt` & `pyvrp-0.3.0/pyvrp/tests/data/E-n22-k4.txt`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/tests/data/EdgeWeightsNoExplicit.txt` & `pyvrp-0.3.0/pyvrp/tests/data/EdgeWeightsNoExplicit.txt`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/tests/data/EdgeWeightsNotFullMatrix.txt` & `pyvrp-0.3.0/pyvrp/tests/data/EdgeWeightsNotFullMatrix.txt`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/tests/data/OkSmall.txt` & `pyvrp-0.3.0/pyvrp/tests/data/OkSmall.txt`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/tests/data/OkSmallGreedyRepair.txt` & `pyvrp-0.3.0/pyvrp/tests/data/OkSmallGreedyRepair.txt`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/tests/data/RC208.txt` & `pyvrp-0.3.0/pyvrp/tests/data/RC208.txt`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/tests/helpers.py` & `pyvrp-0.3.0/pyvrp/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/tests/test_CostEvaluator.py` & `pyvrp-0.3.0/pyvrp/tests/test_CostEvaluator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-from numpy.testing import assert_equal
+from numpy.testing import assert_, assert_allclose, assert_equal
 from pytest import mark
 
 from pyvrp import CostEvaluator, Individual
 from pyvrp.tests.helpers import read
 
 
 def test_load_penalty():
@@ -73,20 +73,38 @@
 
     assert_equal(cost_evaluator.cost(feas_indiv), distance)
     assert_equal(default_cost_evaluator.cost(feas_indiv), distance)
 
     # Infeasible individual
     infeas_indiv = Individual(data, [[1, 2, 3, 4]])
 
-    # C++ code represents infinite as max value for unsigned integer
+    # C++ code represents infinity as UINT_MAX
     INFEAS_COST = np.iinfo(np.uint32).max
     assert_equal(cost_evaluator.cost(infeas_indiv), INFEAS_COST)
     assert_equal(default_cost_evaluator.cost(infeas_indiv), INFEAS_COST)
 
 
+def test_cost_with_prizes():
+    data = read("data/p06-2-50.vrp", round_func="dimacs")
+    cost_evaluator = CostEvaluator(1, 1)
+
+    indiv = Individual(data, [[1, 2], [3, 4, 5]])
+    cost = cost_evaluator.cost(indiv)
+    assert_(indiv.is_feasible())
+
+    prizes = [data.client(idx).prize for idx in range(data.num_clients + 1)]
+    collected = sum(prizes[:6])
+    uncollected = sum(prizes) - collected
+
+    assert_allclose(prizes[0], 0)
+    assert_allclose(indiv.prizes(), collected)
+    assert_allclose(indiv.uncollected_prizes(), uncollected)
+    assert_allclose(indiv.distance() + indiv.uncollected_prizes(), cost)
+
+
 def test_penalised_cost():
     data = read("data/OkSmall.txt")
     penalty_capacity = 20
     penalty_tw = 6
     default_cost_evaluator = CostEvaluator()
     cost_evaluator = CostEvaluator(penalty_capacity, penalty_tw)
```

### Comparing `pyvrp-0.2.1/pyvrp/tests/test_GeneticAlgorithm.py` & `pyvrp-0.3.0/pyvrp/tests/test_GeneticAlgorithm.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/tests/test_Individual.py` & `pyvrp-0.3.0/pyvrp/tests/test_Individual.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from copy import copy, deepcopy
 
 import numpy as np
-from numpy.testing import assert_, assert_equal, assert_raises
+from numpy.testing import assert_, assert_allclose, assert_equal, assert_raises
 from pytest import mark
 
 from pyvrp import Client, Individual, ProblemData, XorShift128
 from pyvrp.tests.helpers import read
 
 
 def test_route_constructor_sorts_by_empty():
@@ -22,32 +22,59 @@
     # We expect Individual to sort the routes such that all non-empty routes
     # are in the lower indices.
     assert_equal(len(routes[0]), 2)
     assert_equal(len(routes[1]), 2)
     assert_equal(len(routes[2]), 0)
 
 
-def test_route_constructor_raises():
+def test_random_constructor_cycles_over_routes():
+    # This instance has four clients and three vehicles. Since 1 client per
+    # vehicle would not work (insufficient vehicles), each route is given two
+    # clients (and the last route should be empty).
+    data = read("data/OkSmall.txt")
+    rng = XorShift128(seed=42)
+
+    indiv = Individual.make_random(data, rng)
+    routes = indiv.get_routes()
+
+    assert_equal(indiv.num_routes(), 2)
+    assert_equal(len(routes), 3)
+
+    for idx, size in enumerate([2, 2, 0]):
+        assert_equal(len(routes[idx]), size)
+
+
+def test_route_constructor_raises_too_many_vehicles():
     data = read("data/OkSmall.txt")
 
     assert_equal(data.num_vehicles, 3)
 
     # Only two routes should not raise. But we should always get num_vehicles
     # routes back.
-    individual = Individual(data, [[1, 2], [4, 2]])
+    individual = Individual(data, [[1, 2], [4, 3]])
     assert_equal(len(individual.get_routes()), data.num_vehicles)
 
     # Empty third route should not raise.
-    Individual(data, [[1, 2], [4, 2], []])
+    Individual(data, [[1, 2], [4, 3], []])
 
     # More than three routes should raise, since we only have three vehicles.
     with assert_raises(RuntimeError):
         Individual(data, [[1], [2], [3], [4]])
 
 
+def test_route_constructor_raises_for_invalid_routes():
+    data = read("data/OkSmall.txt")
+    with assert_raises(RuntimeError):
+        Individual(data, [[1, 2], [1, 3, 4]])  # client 1 is visited twice
+
+    data = read("data/OkSmallPrizes.txt")
+    with assert_raises(RuntimeError):
+        Individual(data, [[2], [3, 4]])  # 1 is required but not visited
+
+
 def test_get_neighbours():
     data = read("data/OkSmall.txt")
 
     indiv = Individual(data, [[3, 4], [], [1, 2]])
     neighbours = indiv.get_neighbours()
 
     expected = [
@@ -85,27 +112,34 @@
     assert_(not indiv.has_time_warp())
 
 
 def test_distance_calculation():
     data = read("data/OkSmall.txt")
 
     indiv = Individual(data, [[1, 2], [3], [4]])
+    routes = indiv.get_routes()
+
+    # Solution is feasible, so all its routes should also be feasible.
     assert_(indiv.is_feasible())
+    assert_(all(route.is_feasible() for route in routes))
 
-    # Feasible individual, so cost should equal total distance travelled.
-    dist = (
-        data.dist(0, 1)
-        + data.dist(1, 2)
-        + data.dist(2, 0)
-        + data.dist(0, 3)
-        + data.dist(3, 0)
-        + data.dist(0, 4)
-        + data.dist(4, 0)
+    # Solution distance should be equal to all routes' distances. These we
+    # check separately.
+    assert_allclose(
+        indiv.distance(), sum(route.distance() for route in routes)
     )
-    assert_equal(indiv.distance(), dist)
+
+    expected = data.dist(0, 1) + data.dist(1, 2) + data.dist(2, 0)
+    assert_allclose(routes[0].distance(), expected)
+
+    expected = data.dist(0, 3) + data.dist(3, 0)
+    assert_allclose(routes[1].distance(), expected)
+
+    expected = data.dist(0, 4) + data.dist(4, 0)
+    assert_allclose(routes[2].distance(), expected)
 
 
 def test_excess_load_calculation():
     data = read("data/OkSmall.txt")
 
     indiv = Individual(data, [[4, 3, 1, 2]])
     assert_(indiv.has_excess_load())
@@ -113,29 +147,71 @@
 
     # All clients are visited on the same route/by the same vehicle. The total
     # demand is 18, but the vehicle capacity is only 10. This has a non-zero
     # load penalty
     assert_equal(indiv.excess_load(), 18 - data.vehicle_capacity)
 
 
-def test_time_warp_calculation():
+def test_route_access_methods():
     data = read("data/OkSmall.txt")
-
     indiv = Individual(data, [[1, 3], [2, 4]])
+    routes = indiv.get_routes()
+
+    # Test route access: getting the route plan should return a simple list, as
+    # given to the individual above.
+    assert_equal(routes[0].visits(), [1, 3])
+    assert_equal(routes[1].visits(), [2, 4])
+
+    # There's no excess load, so all excess load should be zero.
     assert_(not indiv.has_excess_load())
-    assert_(indiv.has_time_warp())
+    assert_allclose(routes[0].excess_load(), 0)
+    assert_allclose(routes[1].excess_load(), 0)
+
+    # Total route demand.
+    demands = [data.client(idx).demand for idx in range(data.num_clients + 1)]
+    assert_allclose(routes[0].demand(), demands[1] + demands[3])
+    assert_allclose(routes[1].demand(), demands[2] + demands[4])
+
+    # The first route is not feasible due to time warp, but the second one is.
+    # See also the tests below.
+    assert_(not routes[0].is_feasible())
+    assert_(routes[1].is_feasible())
+
+    # Total service duration.
+    services = [
+        data.client(idx).service_duration
+        for idx in range(data.num_clients + 1)
+    ]
+    assert_allclose(routes[0].service_duration(), services[1] + services[3])
+    assert_allclose(routes[1].service_duration(), services[2] + services[4])
+
+
+def test_route_time_warp_and_wait_duration():
+    data = read("data/OkSmall.txt")
+    indiv = Individual(data, [[1, 3], [2, 4]])
+    routes = indiv.get_routes()
 
     # There's only time warp on the first route: duration(0, 1) = 1'544, so we
     # arrive at 1 before its opening window of 15'600. Service (360) thus
     # starts at 15'600, and completes at 15'600 + 360. Then we drive for
     # duration(1, 3) = 1'427, where we arrive after 15'300 (its closing time
     # window). This is where we incur time warp: we need to 'warp' to 15'300.
-    tw_first_route = 15_600 + 360 + 1_427 - 15_300
-    tw_second_route = 0
-    assert_equal(indiv.time_warp(), tw_first_route + tw_second_route)
+    assert_(indiv.has_time_warp())
+    assert_(routes[0].has_time_warp())
+    assert_(not routes[1].has_time_warp())
+    assert_allclose(routes[0].time_warp(), 15_600 + 360 + 1_427 - 15_300)
+    assert_allclose(routes[1].time_warp(), 0)
+    assert_allclose(indiv.time_warp(), routes[0].time_warp())
+
+    # On the first route, we have to wait at the first client, where we arrive
+    # at 1'544, but cannot start service until 15'600. On the second route, we
+    # also have to wait at the first client, where we arrive at 1'944, but
+    # cannot start service until 12'000.
+    assert_equal(routes[0].wait_duration(), 15_600 - 1_544)
+    assert_equal(routes[1].wait_duration(), 12_000 - 1_944)
 
 
 @mark.parametrize(
     "dist_mat",
     [
         np.full((3, 3), fill_value=100, dtype=int),
         np.full((3, 3), fill_value=1, dtype=int),
@@ -237,26 +313,27 @@
         individual = Individual.make_random(data, rng)
         str_representation = str(individual).splitlines()
 
         routes = individual.get_routes()
         num_routes = individual.num_routes()
 
         # There should be no more than num_routes lines (each detailing a
-        # single route), and a final line containing the distance.
-        assert_equal(len(str_representation), num_routes + 1)
+        # single route), and two final lines containing distance and prizes.
+        assert_equal(len(str_representation), num_routes + 2)
 
         # The first num_routes lines should each contain a route, where each
         # route should contain every client that is in the route as returned
         # by get_routes().
         for route, str_route in zip(routes[:num_routes], str_representation):
             for client in route:
                 assert_(str(client) in str_route)
 
-        # Last line should contain the distance (cost).
-        assert_(str(individual.distance()) in str_representation[-1])
+        # Last lines should contain the travel distance and collected prizes.
+        assert_(str(individual.distance()) in str_representation[-2])
+        assert_(str(individual.prizes()) in str_representation[-1])
 
 
 def test_hash():
     data = read("data/OkSmall.txt")
     rng = XorShift128(seed=2)
 
     indiv1 = Individual.make_random(data, rng)
```

### Comparing `pyvrp-0.2.1/pyvrp/tests/test_Matrix.py` & `pyvrp-0.3.0/pyvrp/tests/test_Matrix.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/tests/test_PenaltyManager.py` & `pyvrp-0.3.0/pyvrp/tests/test_PenaltyManager.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/tests/test_Population.py` & `pyvrp-0.3.0/pyvrp/tests/test_Population.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 import numpy as np
-from numpy.testing import assert_, assert_allclose, assert_equal, assert_raises
+from numpy.testing import (
+    assert_,
+    assert_allclose,
+    assert_equal,
+    assert_raises,
+    assert_warns,
+)
 from pytest import mark
 
 from pyvrp import (
     CostEvaluator,
     Individual,
     Population,
     PopulationParams,
     XorShift128,
 )
 from pyvrp.diversity import broken_pairs_distance as bpd
+from pyvrp.exceptions import EmptySolutionWarning
 from pyvrp.tests.helpers import make_random_solutions, read
 
 
 @mark.parametrize(
     "min_pop_size,"
     "generation_size,"
     "nb_elite,"
@@ -351,7 +358,16 @@
     for individual in make_random_solutions(10, data, rng):
         pop.add(individual, cost_evaluator)
 
     assert_equal(len(pop), 10)
 
     pop.clear()
     assert_equal(len(pop), 0)
+
+
+def test_add_emits_warning_when_solution_is_empty():
+    data = read("data/p06-2-50.vrp", round_func="dimacs")
+    cost_evaluator = CostEvaluator(20, 6)
+    pop = Population(bpd)
+
+    with assert_warns(EmptySolutionWarning):
+        pop.add(Individual(data, []), cost_evaluator)
```

### Comparing `pyvrp-0.2.1/pyvrp/tests/test_ProblemData.py` & `pyvrp-0.3.0/pyvrp/tests/test_ProblemData.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,58 +2,63 @@
 from numpy.testing import assert_, assert_allclose, assert_raises
 from pytest import mark
 
 from pyvrp import Client, ProblemData
 
 
 @mark.parametrize(
-    "x,y,demand,service_duration,tw_early,tw_late",
+    "x,y,demand,service_duration,tw_early,tw_late,prize",
     [
-        (1, 1, 1, 1, 0, 1),  # normal
-        (1, 1, 1, 0, 0, 1),  # zero duration
-        (1, 1, 0, 1, 0, 1),  # zero demand
-        (1, 1, 1, 1, 0, 0),  # zero length time interval
-        (-1, -1, 1, 1, 0, 1),  # negative coordinates
+        (1, 1, 1, 1, 0, 1, 0),  # normal
+        (1, 1, 1, 0, 0, 1, 0),  # zero duration
+        (1, 1, 0, 1, 0, 1, 0),  # zero demand
+        (1, 1, 1, 1, 0, 0, 0),  # zero length time interval
+        (-1, -1, 1, 1, 0, 1, 0),  # negative coordinates
+        (0, 0, 1, 1, 0, 1, 1),  # positive prize
     ],
 )
 def test_client_constructor_initialises_data_fields_correctly(
     x: int,
     y: int,
     demand: int,
     service_duration: int,
     tw_early: int,
     tw_late: int,
+    prize: int,
 ):
-    client = Client(x, y, demand, service_duration, tw_early, tw_late)
+    client = Client(x, y, demand, service_duration, tw_early, tw_late, prize)
     assert_allclose(client.x, x)
     assert_allclose(client.y, y)
     assert_allclose(client.demand, demand)
     assert_allclose(client.service_duration, service_duration)
     assert_allclose(client.tw_early, tw_early)
     assert_allclose(client.tw_late, tw_late)
+    assert_allclose(client.prize, prize)
 
 
 @mark.parametrize(
-    "x,y,demand,service_duration,tw_early,tw_late",
+    "x,y,demand,service_duration,tw_early,tw_late,prize",
     [
-        (1, 1, 1, 1, 1, 0),  # late < early
-        (1, 1, 1, -1, 0, 1),  # negative duration
-        (1, 1, -1, 1, 0, 1),  # negative demand
+        (1, 1, 1, 1, 1, 0, 0),  # late < early
+        (1, 1, 1, -1, 0, 1, 0),  # negative duration
+        (1, 1, -1, 1, 0, 1, 0),  # negative demand
+        (1, 1, 1, 1, 0, 1, -1),  # negative prize
     ],
 )
 def test_raises_for_invalid_client_data(
     x: int,
     y: int,
     demand: int,
     service_duration: int,
     tw_early: int,
     tw_late: int,
+    prize: int,
 ):
     with assert_raises(ValueError):
-        Client(x, y, demand, service_duration, tw_early, tw_late)
+        Client(x, y, demand, service_duration, tw_early, tw_late, prize)
 
 
 def test_depot_is_first_client():
     """
     The ``depot()`` helper should return the first client, that is,
     ``client(0)``.
     """
```

### Comparing `pyvrp-0.2.1/pyvrp/tests/test_Result.py` & `pyvrp-0.3.0/pyvrp/tests/test_Result.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/tests/test_Statistics.py` & `pyvrp-0.3.0/pyvrp/tests/test_Statistics.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/tests/test_SubPopulation.py` & `pyvrp-0.3.0/pyvrp/tests/test_SubPopulation.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/tests/test_TimeWindowSegment.py` & `pyvrp-0.3.0/pyvrp/tests/test_TimeWindowSegment.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/tests/test_XorShift128.py` & `pyvrp-0.3.0/pyvrp/tests/test_XorShift128.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/pyvrp/tests/test_read.py` & `pyvrp-0.3.0/pyvrp/tests/test_read.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.2.1/PKG-INFO` & `pyvrp-0.3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvrp
-Version: 0.2.1
+Version: 0.3.0
 Summary: A state-of-the-art vehicle routing problem solver.
 Home-page: https://github.com/PyVRP/PyVRP
 License: MIT
 Author: Niels Wouda
 Author-email: nielswouda@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,19 +12,14 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Requires-Dist: matplotlib (>=2.2.0)
 Requires-Dist: numpy (>=1.15.2)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
 Requires-Dist: vrplib (>=1.0.0,<2.0.0)
```

