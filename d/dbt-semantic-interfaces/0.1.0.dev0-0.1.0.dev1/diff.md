# Comparing `tmp/dbt_semantic_interfaces-0.1.0.dev0.tar.gz` & `tmp/dbt_semantic_interfaces-0.1.0.dev1.tar.gz`

## Comparing `dbt_semantic_interfaces-0.1.0.dev0.tar` & `dbt_semantic_interfaces-0.1.0.dev1.tar`

### file list

```diff
@@ -1,150 +1,168 @@
--rw-r--r--   0        0        0     5669 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/.changie.yaml
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/.tool-versions
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/CHANGELOG.md
--rw-r--r--   0        0        0     4067 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/CONTRIBUTING.md
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/Makefile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/.changes/0.0.0.md
--rw-r--r--   0        0        0     3726 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/.changes/README.md
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/.changes/header.tpl.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/.changes/unreleased/.gitkeep
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/.changes/unreleased/Features-20230515-155013.yaml
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/.changes/unreleased/Under the Hood-20230424-152251.yaml
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/.changes/unreleased/Under the Hood-20230501-154838.yaml
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/.changes/unreleased/Under the Hood-20230501-162818.yaml
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/.changes/unreleased/Under the Hood-20230501-164142.yaml
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/.changes/unreleased/Under the Hood-20230505-120359.yaml
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/.changes/unreleased/Under the Hood-20230515-124059.yaml
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/.changes/unreleased/Under the Hood-20230515-125335.yaml
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/.github/pull_request_template.md
--rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/.github/ISSUE_TEMPLATE/feature-request.yml
--rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/.github/ISSUE_TEMPLATE/regression-report.yml
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/.github/actions/setup-python-env/action.yml
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/.github/workflows/bot-changelog.yml
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/.github/workflows/changelog-existence.yml
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/.github/workflows/ci-pre-commit.yaml
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/.github/workflows/ci-pytest.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/__init__.py
--rw-r--r--   0        0        0    17431 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/dataclass_serialization.py
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/enum_extension.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/errors.py
--rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/model_transformer.py
--rw-r--r--   0        0        0     4016 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/model_validator.py
--rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/pretty_print.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/py.typed
--rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/references.py
--rw-r--r--   0        0        0     5744 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/objects/__init__.py
--rw-r--r--   0        0        0     7229 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/objects/base.py
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/objects/metadata.py
--rw-r--r--   0        0        0     7514 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/objects/metric.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/objects/semantic_manifest.py
--rw-r--r--   0        0        0     5899 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/objects/semantic_model.py
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/objects/time_granularity.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/objects/elements/__init__.py
--rw-r--r--   0        0        0     2711 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/objects/elements/dimension.py
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/objects/elements/entity.py
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/objects/elements/measure.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/objects/filters/__init__.py
--rw-r--r--   0        0        0     5440 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/objects/filters/call_parameter_sets.py
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/objects/filters/where_filter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/parsing/__init__.py
--rw-r--r--   0        0        0    13546 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/parsing/dir_to_model.py
--rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/parsing/explicit_schema.py
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/parsing/objects.py
--rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/parsing/schema_validator.py
--rw-r--r--   0        0        0     9300 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/parsing/schemas.py
--rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/parsing/yaml_loader.py
--rw-r--r--   0        0        0    14653 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/parsing/schemas/metricflow.json
--rw-r--r--   0        0        0     2385 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/protocols/measure.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/transformations/__init__.py
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/transformations/add_input_metric_measures.py
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/transformations/agg_time_dimension.py
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/transformations/boolean_measure.py
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/transformations/convert_count.py
--rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/transformations/convert_median.py
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/transformations/names.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/transformations/proxy_measure.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/transformations/transform_rule.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/type_enums/aggregation_type.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/type_enums/dimension_type.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/validations/__init__.py
--rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/validations/agg_time_dimension.py
--rw-r--r--   0        0        0     3757 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/validations/common_entities.py
--rw-r--r--   0        0        0     7729 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/validations/dimension_const.py
--rw-r--r--   0        0        0     3889 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/validations/element_const.py
--rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/validations/entities.py
--rw-r--r--   0        0        0    27760 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/validations/measures.py
--rw-r--r--   0        0        0     6942 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/validations/metrics.py
--rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/validations/non_empty.py
--rw-r--r--   0        0        0     6649 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/validations/reserved_keywords.py
--rw-r--r--   0        0        0    10061 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/validations/semantic_models.py
--rw-r--r--   0        0        0     9808 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/validations/unique_valid_name.py
--rw-r--r--   0        0        0    13769 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/validations/validator_helpers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/tests/__init__.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/tests/conftest.py
--rw-r--r--   0        0        0     7796 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/tests/test_dataclass_serialization.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/tests/test_pretty_print.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/tests/fixtures/__init__.py
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/tests/fixtures/model_fixtures.py
--rw-r--r--   0        0        0    13041 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/tests/fixtures/model_yamls/simple_model/metrics.yaml
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/tests/fixtures/model_yamls/simple_model/semantic_models/accounts_source.yaml
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/tests/fixtures/model_yamls/simple_model/semantic_models/bookings_source.yaml
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/tests/fixtures/model_yamls/simple_model/semantic_models/companies.yaml
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/tests/fixtures/model_yamls/simple_model/semantic_models/id_verifications.yaml
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/tests/fixtures/model_yamls/simple_model/semantic_models/listings_latest.yaml
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/tests/fixtures/model_yamls/simple_model/semantic_models/lux_listing_mapping.yaml
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/tests/fixtures/model_yamls/simple_model/semantic_models/revenue.yaml
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/tests/fixtures/model_yamls/simple_model/semantic_models/user_sm_source.yaml
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/tests/fixtures/model_yamls/simple_model/semantic_models/users_latest.yaml
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/tests/fixtures/model_yamls/simple_model/semantic_models/views_source.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/tests/objects/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/tests/objects/where_filter/__init__.py
--rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/tests/objects/where_filter/test_parse_calls.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/tests/parsing/__init__.py
--rw-r--r--   0        0        0     6019 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/tests/parsing/test_metadata_parsing.py
--rw-r--r--   0        0        0    16595 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/tests/parsing/test_metric_parsing.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/tests/parsing/test_model_deserialization.py
--rw-r--r--   0        0        0    14867 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/tests/parsing/test_semantic_model_parsing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/tests/transformations/__init__.py
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/tests/transformations/test_configurable_transform_rules.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/tests/validations/__init__.py
--rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/tests/validations/test_agg_time_dimension.py
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/tests/validations/test_common_entities.py
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/tests/validations/test_configurable_rules.py
--rw-r--r--   0        0        0     7404 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/tests/validations/test_dimension_const.py
--rw-r--r--   0        0        0     3655 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/tests/validations/test_element_const.py
--rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/tests/validations/test_entities.py
--rw-r--r--   0        0        0    25297 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/tests/validations/test_measures.py
--rw-r--r--   0        0        0    10958 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/tests/validations/test_metrics.py
--rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/tests/validations/test_reserved_keywords.py
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/tests/validations/test_semantic_models.py
--rw-r--r--   0        0        0     7603 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/tests/validations/test_unique_valid_name.py
--rw-r--r--   0        0        0     5818 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/tests/validations/test_validator_helpers.py
--rw-r--r--   0        0        0    14533 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/tests/validations/test_validity_param_definitions.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/venv-3.9.16/pyvenv.cfg
--rw-r--r--   0        0        0     8834 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/venv-3.9.16/bin/Activate.ps1
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/venv-3.9.16/bin/activate
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/venv-3.9.16/bin/activate.csh
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/venv-3.9.16/bin/activate.fish
--rwxr-xr-x   0        0        0      279 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/venv-3.9.16/bin/hatch
--rwxr-xr-x   0        0        0      293 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/venv-3.9.16/bin/hatchling
--rwxr-xr-x   0        0        0      275 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/venv-3.9.16/bin/httpx
--rwxr-xr-x   0        0        0      281 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/venv-3.9.16/bin/keyring
--rwxr-xr-x   0        0        0      291 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/venv-3.9.16/bin/markdown-it
--rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/venv-3.9.16/bin/pip
--rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/venv-3.9.16/bin/pip3
--rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/venv-3.9.16/bin/pip3.9
--rwxr-xr-x   0        0        0      286 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/venv-3.9.16/bin/pygmentize
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/venv-3.9.16/bin/python -> /Users/quigleymalcolm/.asdf/installs/python/3.9.16/bin/python
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/venv-3.9.16/bin/python3 -> python
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/venv-3.9.16/bin/python3.9 -> python
--rwxr-xr-x   0        0        0      290 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/venv-3.9.16/bin/userpath
--rwxr-xr-x   0        0        0      309 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/venv-3.9.16/bin/virtualenv
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/LICENSE
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/README.md
--rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/pyproject.toml
--rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev0/PKG-INFO
+-rw-r--r--   0        0        0     5669 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.changie.yaml
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.tool-versions
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/CHANGELOG.md
+-rw-r--r--   0        0        0     4067 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/Makefile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.changes/0.0.0.md
+-rw-r--r--   0        0        0     3726 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.changes/README.md
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.changes/header.tpl.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.changes/unreleased/.gitkeep
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.changes/unreleased/Features-20230515-155013.yaml
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.changes/unreleased/Features-20230515-161320.yaml
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.changes/unreleased/Features-20230516-100539.yaml
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.changes/unreleased/Features-20230516-112250.yaml
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.changes/unreleased/Features-20230516-150352.yaml
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.changes/unreleased/Features-20230516-162909.yaml
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.changes/unreleased/Fixes-20230516-172635.yaml
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.changes/unreleased/Fixes-20230516-175643.yaml
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.changes/unreleased/Under the Hood-20230424-152251.yaml
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.changes/unreleased/Under the Hood-20230501-154838.yaml
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.changes/unreleased/Under the Hood-20230501-162818.yaml
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.changes/unreleased/Under the Hood-20230501-164142.yaml
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.changes/unreleased/Under the Hood-20230505-120359.yaml
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.changes/unreleased/Under the Hood-20230515-124059.yaml
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.changes/unreleased/Under the Hood-20230515-125335.yaml
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.github/pull_request_template.md
+-rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.github/ISSUE_TEMPLATE/feature-request.yml
+-rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.github/ISSUE_TEMPLATE/regression-report.yml
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.github/actions/setup-python-env/action.yml
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.github/workflows/bot-changelog.yml
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.github/workflows/changelog-existence.yml
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.github/workflows/ci-pre-commit.yaml
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.github/workflows/ci-pytest.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/__init__.py
+-rw-r--r--   0        0        0    17431 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/dataclass_serialization.py
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/enum_extension.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/errors.py
+-rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/model_transformer.py
+-rw-r--r--   0        0        0     4016 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/model_validator.py
+-rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/pretty_print.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/py.typed
+-rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/references.py
+-rw-r--r--   0        0        0     5744 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/objects/__init__.py
+-rw-r--r--   0        0        0     7229 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/objects/base.py
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/objects/metadata.py
+-rw-r--r--   0        0        0     7399 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/objects/metric.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/objects/semantic_manifest.py
+-rw-r--r--   0        0        0     5699 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/objects/semantic_model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/objects/elements/__init__.py
+-rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/objects/elements/dimension.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/objects/elements/entity.py
+-rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/objects/elements/measure.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/objects/filters/__init__.py
+-rw-r--r--   0        0        0     5443 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/objects/filters/call_parameter_sets.py
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/objects/filters/where_filter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/parsing/__init__.py
+-rw-r--r--   0        0        0    13546 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/parsing/dir_to_model.py
+-rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/parsing/explicit_schema.py
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/parsing/objects.py
+-rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/parsing/schema_validator.py
+-rw-r--r--   0        0        0     9300 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/parsing/schemas.py
+-rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/parsing/yaml_loader.py
+-rw-r--r--   0        0        0    14653 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/parsing/schemas/metricflow.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/protocols/__init__.py
+-rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/protocols/dimension.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/protocols/entity.py
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/protocols/measure.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/protocols/metadata.py
+-rw-r--r--   0        0        0     3598 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/protocols/metric.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/protocols/semantic_manifest.py
+-rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/protocols/semantic_model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/transformations/__init__.py
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/transformations/add_input_metric_measures.py
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/transformations/agg_time_dimension.py
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/transformations/boolean_measure.py
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/transformations/convert_count.py
+-rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/transformations/convert_median.py
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/transformations/names.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/transformations/proxy_measure.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/transformations/transform_rule.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/type_enums/__init__.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/type_enums/aggregation_type.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/type_enums/dimension_type.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/type_enums/entity_type.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/type_enums/metric_type.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/type_enums/time_granularity.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/validations/__init__.py
+-rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/validations/agg_time_dimension.py
+-rw-r--r--   0        0        0     3757 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/validations/common_entities.py
+-rw-r--r--   0        0        0     7732 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/validations/dimension_const.py
+-rw-r--r--   0        0        0     3889 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/validations/element_const.py
+-rw-r--r--   0        0        0     4886 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/validations/entities.py
+-rw-r--r--   0        0        0    27760 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/validations/measures.py
+-rw-r--r--   0        0        0     6942 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/validations/metrics.py
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/validations/non_empty.py
+-rw-r--r--   0        0        0     6649 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/validations/reserved_keywords.py
+-rw-r--r--   0        0        0    10060 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/validations/semantic_models.py
+-rw-r--r--   0        0        0     9811 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/validations/unique_valid_name.py
+-rw-r--r--   0        0        0    13769 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/validations/validator_helpers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/__init__.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/conftest.py
+-rw-r--r--   0        0        0     7796 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/test_dataclass_serialization.py
+-rw-r--r--   0        0        0     6128 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/test_implements_satisfy_protocols.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/test_pretty_print.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/fixtures/model_fixtures.py
+-rw-r--r--   0        0        0    13041 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/fixtures/model_yamls/simple_model/metrics.yaml
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/fixtures/model_yamls/simple_model/semantic_models/accounts_source.yaml
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/fixtures/model_yamls/simple_model/semantic_models/bookings_source.yaml
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/fixtures/model_yamls/simple_model/semantic_models/companies.yaml
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/fixtures/model_yamls/simple_model/semantic_models/id_verifications.yaml
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/fixtures/model_yamls/simple_model/semantic_models/listings_latest.yaml
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/fixtures/model_yamls/simple_model/semantic_models/lux_listing_mapping.yaml
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/fixtures/model_yamls/simple_model/semantic_models/revenue.yaml
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/fixtures/model_yamls/simple_model/semantic_models/user_sm_source.yaml
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/fixtures/model_yamls/simple_model/semantic_models/users_latest.yaml
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/fixtures/model_yamls/simple_model/semantic_models/views_source.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/objects/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/objects/where_filter/__init__.py
+-rw-r--r--   0        0        0     2801 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/objects/where_filter/test_parse_calls.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/parsing/__init__.py
+-rw-r--r--   0        0        0     6019 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/parsing/test_metadata_parsing.py
+-rw-r--r--   0        0        0    16598 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/parsing/test_metric_parsing.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/parsing/test_model_deserialization.py
+-rw-r--r--   0        0        0    14869 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/parsing/test_semantic_model_parsing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/transformations/__init__.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/transformations/test_configurable_transform_rules.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/validations/__init__.py
+-rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/validations/test_agg_time_dimension.py
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/validations/test_common_entities.py
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/validations/test_configurable_rules.py
+-rw-r--r--   0        0        0     7407 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/validations/test_dimension_const.py
+-rw-r--r--   0        0        0     3655 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/validations/test_element_const.py
+-rw-r--r--   0        0        0     4436 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/validations/test_entities.py
+-rw-r--r--   0        0        0    25297 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/validations/test_measures.py
+-rw-r--r--   0        0        0    11019 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/validations/test_metrics.py
+-rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/validations/test_reserved_keywords.py
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/validations/test_semantic_models.py
+-rw-r--r--   0        0        0     7603 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/validations/test_unique_valid_name.py
+-rw-r--r--   0        0        0     5818 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/validations/test_validator_helpers.py
+-rw-r--r--   0        0        0    14533 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/tests/validations/test_validity_param_definitions.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/venv-3.9.16/pyvenv.cfg
+-rw-r--r--   0        0        0     8834 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/venv-3.9.16/bin/Activate.ps1
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/venv-3.9.16/bin/activate
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/venv-3.9.16/bin/activate.csh
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/venv-3.9.16/bin/activate.fish
+-rwxr-xr-x   0        0        0      279 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/venv-3.9.16/bin/hatch
+-rwxr-xr-x   0        0        0      293 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/venv-3.9.16/bin/hatchling
+-rwxr-xr-x   0        0        0      275 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/venv-3.9.16/bin/httpx
+-rwxr-xr-x   0        0        0      281 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/venv-3.9.16/bin/keyring
+-rwxr-xr-x   0        0        0      291 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/venv-3.9.16/bin/markdown-it
+-rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/venv-3.9.16/bin/pip
+-rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/venv-3.9.16/bin/pip3
+-rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/venv-3.9.16/bin/pip3.9
+-rwxr-xr-x   0        0        0      286 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/venv-3.9.16/bin/pygmentize
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/venv-3.9.16/bin/python -> /Users/quigleymalcolm/.asdf/installs/python/3.9.16/bin/python
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/venv-3.9.16/bin/python3 -> python
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/venv-3.9.16/bin/python3.9 -> python
+-rwxr-xr-x   0        0        0      290 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/venv-3.9.16/bin/userpath
+-rwxr-xr-x   0        0        0      309 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/venv-3.9.16/bin/virtualenv
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/LICENSE
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/README.md
+-rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/pyproject.toml
+-rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 dbt_semantic_interfaces-0.1.0.dev1/PKG-INFO
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/.changie.yaml` & `dbt_semantic_interfaces-0.1.0.dev1/.changie.yaml`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/.pre-commit-config.yaml` & `dbt_semantic_interfaces-0.1.0.dev1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/CONTRIBUTING.md` & `dbt_semantic_interfaces-0.1.0.dev1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/Makefile` & `dbt_semantic_interfaces-0.1.0.dev1/Makefile`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/.changes/README.md` & `dbt_semantic_interfaces-0.1.0.dev1/.changes/README.md`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/.changes/header.tpl.md` & `dbt_semantic_interfaces-0.1.0.dev1/.changes/header.tpl.md`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/.github/pull_request_template.md` & `dbt_semantic_interfaces-0.1.0.dev1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/.github/ISSUE_TEMPLATE/bug-report.yml` & `dbt_semantic_interfaces-0.1.0.dev1/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/.github/ISSUE_TEMPLATE/feature-request.yml` & `dbt_semantic_interfaces-0.1.0.dev1/.github/ISSUE_TEMPLATE/feature-request.yml`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/.github/ISSUE_TEMPLATE/regression-report.yml` & `dbt_semantic_interfaces-0.1.0.dev1/.github/ISSUE_TEMPLATE/regression-report.yml`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/.github/workflows/bot-changelog.yml` & `dbt_semantic_interfaces-0.1.0.dev1/.github/workflows/bot-changelog.yml`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/.github/workflows/changelog-existence.yml` & `dbt_semantic_interfaces-0.1.0.dev1/.github/workflows/changelog-existence.yml`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/dataclass_serialization.py` & `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/dataclass_serialization.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/enum_extension.py` & `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/enum_extension.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/errors.py` & `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/errors.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/model_transformer.py` & `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/model_transformer.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/model_validator.py` & `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/model_validator.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/pretty_print.py` & `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/pretty_print.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/references.py` & `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/references.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/test_utils.py` & `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/test_utils.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/objects/base.py` & `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/objects/base.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/objects/metric.py` & `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/objects/metric.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,26 @@
 from __future__ import annotations
 
 from typing import List, Optional
 
-from dbt_semantic_interfaces.enum_extension import ExtendedEnum
 from dbt_semantic_interfaces.errors import ParsingException
 from dbt_semantic_interfaces.objects.base import (
     HashableBaseModel,
     ModelWithMetadataParsing,
     PydanticCustomInputParser,
     PydanticParseableValueType,
 )
 from dbt_semantic_interfaces.objects.filters.where_filter import WhereFilter
 from dbt_semantic_interfaces.objects.metadata import Metadata
-from dbt_semantic_interfaces.objects.time_granularity import (
+from dbt_semantic_interfaces.references import MeasureReference, MetricReference
+from dbt_semantic_interfaces.type_enums.metric_type import MetricType
+from dbt_semantic_interfaces.type_enums.time_granularity import (
     TimeGranularity,
     string_to_time_granularity,
 )
-from dbt_semantic_interfaces.references import MeasureReference, MetricReference
-
-
-class MetricType(ExtendedEnum):
-    """Currently supported metric types."""
-
-    MEASURE_PROXY = "measure_proxy"
-    RATIO = "ratio"
-    EXPR = "expr"
-    CUMULATIVE = "cumulative"
-    DERIVED = "derived"
 
 
 class MetricInputMeasure(PydanticCustomInputParser, HashableBaseModel):
     """Provides a pointer to a measure along with metric-specific processing directives.
 
     If an alias is set, this will be used as the string name reference for this measure after the aggregation
     phase in the SQL plan.
@@ -130,15 +120,16 @@
     name: str
     filter: Optional[WhereFilter]
     alias: Optional[str]
     offset_window: Optional[MetricTimeWindow]
     offset_to_grain: Optional[TimeGranularity]
 
     @property
-    def as_reference(self) -> MetricReference:  # noqa: D
+    def as_reference(self) -> MetricReference:
+        """Property accessor to get the MetricReference associated with this metric input."""
         return MetricReference(element_name=self.name)
 
 
 class MetricTypeParams(HashableBaseModel):
     """Type params add additional context to certain metric types (the context depends on the metric type)."""
 
     measure: Optional[MetricInputMeasure]
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/objects/semantic_model.py` & `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/objects/semantic_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,56 +81,30 @@
     def dimension_references(self) -> List[LinkableElementReference]:  # noqa: D
         return [i.reference for i in self.dimensions]
 
     @property
     def measure_references(self) -> List[MeasureReference]:  # noqa: D
         return [i.reference for i in self.measures]
 
-    def get_measure(self, measure_reference: MeasureReference) -> Measure:  # noqa: D
-        for measure in self.measures:
-            if measure.reference == measure_reference:
-                return measure
-
-        raise ValueError(
-            f"No dimension with name ({measure_reference.element_name}) in semantic_model with name ({self.name})"
-        )
-
-    def get_dimension(self, dimension_reference: LinkableElementReference) -> Dimension:  # noqa: D
-        for dim in self.dimensions:
-            if dim.reference == dimension_reference:
-                return dim
-
-        raise ValueError(f"No dimension with name ({dimension_reference}) in semantic_model with name ({self.name})")
-
-    def get_entity(self, entity_reference: LinkableElementReference) -> Entity:  # noqa: D
-        for entity in self.entities:
-            if entity.reference == entity_reference:
-                return entity
-
-        raise ValueError(f"No entity with name ({entity_reference}) in semantic_model with name ({self.name})")
-
     @property
-    def has_validity_dimensions(self) -> bool:
-        """Returns True if there are validity params set on one or more dimensions."""
+    def has_validity_dimensions(self) -> bool:  # noqa: D
         return any([dim.validity_params is not None for dim in self.dimensions])
 
     @property
-    def validity_start_dimension(self) -> Optional[Dimension]:
-        """Returns the validity window start dimension, if one is set."""
+    def validity_start_dimension(self) -> Optional[Dimension]:  # noqa: D
         validity_start_dims = [dim for dim in self.dimensions if dim.validity_params and dim.validity_params.is_start]
         if not validity_start_dims:
             return None
         assert (
             len(validity_start_dims) == 1
         ), "Found more than one validity start dimension. This should have been blocked in validation!"
         return validity_start_dims[0]
 
     @property
-    def validity_end_dimension(self) -> Optional[Dimension]:
-        """Returns the validity window end dimension, if one is set."""
+    def validity_end_dimension(self) -> Optional[Dimension]:  # noqa: D
         validity_end_dims = [dim for dim in self.dimensions if dim.validity_params and dim.validity_params.is_end]
         if not validity_end_dims:
             return None
         assert (
             len(validity_end_dims) == 1
         ), "Found more than one validity end dimension. This should have been blocked in validation!"
         return validity_end_dims[0]
@@ -147,7 +121,30 @@
         if len(partitions) > 1:
             raise ValueError(f"too many partitions for semantic_model {self.name}")
         return partitions[0]
 
     @property
     def reference(self) -> SemanticModelReference:  # noqa: D
         return SemanticModelReference(semantic_model_name=self.name)
+
+    def get_measure(self, measure_reference: MeasureReference) -> Measure:  # noqa: D
+        for measure in self.measures:
+            if measure.reference == measure_reference:
+                return measure
+
+        raise ValueError(
+            f"No dimension with name ({measure_reference.element_name}) in semantic_model with name ({self.name})"
+        )
+
+    def get_dimension(self, dimension_reference: LinkableElementReference) -> Dimension:  # noqa: D
+        for dim in self.dimensions:
+            if dim.reference == dimension_reference:
+                return dim
+
+        raise ValueError(f"No dimension with name ({dimension_reference}) in semantic_model with name ({self.name})")
+
+    def get_entity(self, entity_reference: LinkableElementReference) -> Entity:  # noqa: D
+        for entity in self.entities:
+            if entity.reference == entity_reference:
+                return entity
+
+        raise ValueError(f"No entity with name ({entity_reference}) in semantic_model with name ({self.name})")
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/objects/time_granularity.py` & `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/type_enums/time_granularity.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/objects/elements/dimension.py` & `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/objects/elements/dimension.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 from typing import Optional
 
 from dbt_semantic_interfaces.objects.base import (
     HashableBaseModel,
     ModelWithMetadataParsing,
 )
 from dbt_semantic_interfaces.objects.metadata import Metadata
-from dbt_semantic_interfaces.objects.time_granularity import TimeGranularity
 from dbt_semantic_interfaces.references import (
     DimensionReference,
     TimeDimensionReference,
 )
 from dbt_semantic_interfaces.type_enums.dimension_type import DimensionType
+from dbt_semantic_interfaces.type_enums.time_granularity import TimeGranularity
 
 ISO8601_FMT = "YYYY-MM-DD"
 
 
 class DimensionValidityParams(HashableBaseModel):
     """Parameters identifying a given dimension as an entity for validity state.
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/objects/elements/measure.py` & `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/protocols/measure.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,46 +1,52 @@
 from __future__ import annotations
 
-from typing import List, Optional
+from abc import abstractmethod
+from typing import List, Optional, Protocol
 
-from dbt_semantic_interfaces.objects.base import (
-    HashableBaseModel,
-    ModelWithMetadataParsing,
-)
-from dbt_semantic_interfaces.objects.metadata import Metadata
-from dbt_semantic_interfaces.protocols.measure import _MeasureMixin
+from dbt_semantic_interfaces.references import MeasureReference, TimeDimensionReference
 from dbt_semantic_interfaces.type_enums.aggregation_type import AggregationType
 
 
-class NonAdditiveDimensionParameters(HashableBaseModel):
-    """Describes the params for specifying non-additive dimensions in a measure.
-
-    NOTE: Currently, only TimeDimensions are supported for this filter
-    """
+class NonAdditiveDimensionParameters(Protocol):
+    """Describes the params for specifying non-additive dimensions in a measure."""
 
     name: str
-
-    # Optional Fields
-    window_choice: AggregationType = AggregationType.MIN
-    window_groupings: List[str] = []
+    window_choice: AggregationType
+    window_groupings: List[str]
 
 
-class MeasureAggregationParameters(HashableBaseModel):
+class MeasureAggregationParameters(Protocol):
     """Describes parameters for aggregations."""
 
-    percentile: Optional[float] = None
-    use_discrete_percentile: bool = False
-    use_approximate_percentile: bool = False
+    percentile: Optional[float]
+    use_discrete_percentile: bool
+    use_approximate_percentile: bool
 
 
-class Measure(_MeasureMixin, HashableBaseModel, ModelWithMetadataParsing):
-    """Describes a measure."""
+class Measure(Protocol):
+    """Describes a measure.
+
+    Measure is a field in the underlying semantic model that can be aggregated
+    in a specific way.
+    """
 
     name: str
     agg: AggregationType
     description: Optional[str]
     create_metric: Optional[bool]
-    expr: Optional[str] = None
+    expr: Optional[str]
     agg_params: Optional[MeasureAggregationParameters]
-    metadata: Optional[Metadata]
-    non_additive_dimension: Optional[NonAdditiveDimensionParameters] = None
-    agg_time_dimension: Optional[str] = None
+    non_additive_dimension: Optional[NonAdditiveDimensionParameters]
+    agg_time_dimension: Optional[str]
+
+    @property
+    @abstractmethod
+    def checked_agg_time_dimension(self) -> TimeDimensionReference:
+        """Returns the aggregation time dimension, throwing an exception if it's not set."""
+        ...
+
+    @property
+    @abstractmethod
+    def reference(self) -> MeasureReference:
+        """Returns a reference to this measure."""
+        ...
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/objects/filters/call_parameter_sets.py` & `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/objects/filters/call_parameter_sets.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 
 import jinja2
 
 from dbt_semantic_interfaces.objects.filters.where_filter import (
     WhereFilter,
     WhereFilterTransform,
 )
-from dbt_semantic_interfaces.objects.time_granularity import TimeGranularity
 from dbt_semantic_interfaces.references import (
     DimensionReference,
     EntityReference,
     TimeDimensionReference,
 )
+from dbt_semantic_interfaces.type_enums.time_granularity import TimeGranularity
 
 
 @dataclass(frozen=True)
 class DimensionCallParameterSet:
     """When 'dimension(...)' is used in the Jinja template of the where filter, the parameters to that call."""
 
     entity_path: Tuple[EntityReference, ...]
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/objects/filters/where_filter.py` & `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/objects/filters/where_filter.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/parsing/dir_to_model.py` & `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/parsing/dir_to_model.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/parsing/explicit_schema.py` & `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/parsing/explicit_schema.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/parsing/objects.py` & `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/parsing/objects.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/parsing/schema_validator.py` & `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/parsing/schema_validator.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/parsing/schemas.py` & `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/parsing/schemas.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/parsing/yaml_loader.py` & `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/parsing/yaml_loader.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/parsing/schemas/metricflow.json` & `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/parsing/schemas/metricflow.json`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/protocols/measure.py` & `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/protocols/dimension.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,74 +1,70 @@
 from __future__ import annotations
 
 from abc import abstractmethod
-from typing import List, Optional, Protocol
+from typing import Optional, Protocol
 
-from dbt_semantic_interfaces.references import MeasureReference, TimeDimensionReference
-from dbt_semantic_interfaces.type_enums.aggregation_type import AggregationType
-
-
-class NonAdditiveDimensionParameters(Protocol):
-    """Describes the params for specifying non-additive dimensions in a measure."""
-
-    name: str
-    window_choice: AggregationType
-    window_groupings: List[str]
+from dbt_semantic_interfaces.protocols.metadata import Metadata
+from dbt_semantic_interfaces.references import (
+    DimensionReference,
+    TimeDimensionReference,
+)
+from dbt_semantic_interfaces.type_enums.dimension_type import DimensionType
+from dbt_semantic_interfaces.type_enums.time_granularity import TimeGranularity
+
+
+class DimensionValidityParams(Protocol):
+    """Parameters identifying a given dimension as an entity for validity state.
+
+    This construct is used for supporting SCD Type II tables, such as might be
+    created via dbt's snapshot feature, or generated via periodic loads from external
+    dimension data sources. In either of those cases, there is typically a time dimension
+    associated with the SCD data source that indicates the start and end times of a
+    validity window, where the dimension value is valid for any time within that range.
+    """
 
+    is_start: bool
+    is_end: bool
 
-class MeasureAggregationParameters(Protocol):
-    """Describes parameters for aggregations."""
 
-    percentile: Optional[float]
-    use_discrete_percentile: bool
-    use_approximate_percentile: bool
+class DimensionTypeParams(Protocol):
+    """Dimension type params add context to some types of dimensions (like time)."""
 
+    is_primary: bool
+    time_granularity: TimeGranularity
+    validity_params: Optional[DimensionValidityParams]
 
-class Measure(Protocol):
-    """Describes a measure.
 
-    Measure is a field in the underlying semantic model that can be aggregated
-    in a specific way.
-    """
+class Dimension(Protocol):
+    """Describes a dimension."""
 
     name: str
-    agg: AggregationType
     description: Optional[str]
-    create_metric: Optional[bool]
+    type: DimensionType
+    is_partition: bool
+    type_params: Optional[DimensionTypeParams]
     expr: Optional[str]
-    agg_params: Optional[MeasureAggregationParameters]
-    non_additive_dimension: Optional[NonAdditiveDimensionParameters]
-    agg_time_dimension: Optional[str]
+    metadata: Optional[Metadata]
 
     @property
     @abstractmethod
-    def checked_agg_time_dimension(self) -> TimeDimensionReference:
-        """Returns the aggregation time dimension, throwing an exception if it's not set."""
+    def is_primary_time(self) -> bool:
+        """Returns boolean of whether the dimension is a the primary time dimension."""
         ...
 
     @property
     @abstractmethod
-    def reference(self) -> MeasureReference:
-        """Returns a reference to this measure."""
+    def reference(self) -> DimensionReference:
+        """Returns a DimensionReference object for the dimension implementation."""
         ...
 
-
-class _MeasureMixin:
-    """Some useful default implementation details of MeasureProtocol."""
-
-    name: str
-    expr: Optional[str] = None
-    non_additive_dimension: Optional[NonAdditiveDimensionParameters] = None
-    agg_time_dimension: Optional[str] = None
-
     @property
-    def checked_agg_time_dimension(self) -> TimeDimensionReference:
-        assert self.agg_time_dimension, (
-            f"Aggregation time dimension for measure {self.name} is not set! This should either be set directly on "
-            f"the measure specification in the model, or else defaulted to the primary time dimension in the data "
-            f"source containing the measure."
-        )
-        return TimeDimensionReference(element_name=self.agg_time_dimension)
+    @abstractmethod
+    def time_dimension_reference(self) -> Optional[TimeDimensionReference]:
+        """Returns a TimeDimensionReference if the dimension implementation is a time dimension."""
+        ...
 
     @property
-    def reference(self) -> MeasureReference:  # noqa: D
-        return MeasureReference(element_name=self.name)
+    @abstractmethod
+    def validity_params(self) -> Optional[DimensionValidityParams]:
+        """Returns the DimensionValidityParams if they exist for the dimension implementation."""
+        ...
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/transformations/add_input_metric_measures.py` & `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/transformations/add_input_metric_measures.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/transformations/agg_time_dimension.py` & `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/transformations/agg_time_dimension.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/transformations/boolean_measure.py` & `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/transformations/boolean_measure.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/transformations/convert_count.py` & `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/transformations/convert_count.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/transformations/convert_median.py` & `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/transformations/convert_median.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/transformations/names.py` & `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/transformations/names.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/transformations/proxy_measure.py` & `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/transformations/proxy_measure.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/validations/agg_time_dimension.py` & `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/validations/agg_time_dimension.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/validations/common_entities.py` & `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/validations/common_entities.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/validations/dimension_const.py` & `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/validations/dimension_const.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Dict, List
 
 from dbt_semantic_interfaces.objects.elements.dimension import Dimension
 from dbt_semantic_interfaces.objects.semantic_manifest import SemanticManifest
 from dbt_semantic_interfaces.objects.semantic_model import SemanticModel
-from dbt_semantic_interfaces.objects.time_granularity import TimeGranularity
 from dbt_semantic_interfaces.references import (
     DimensionReference,
     SemanticModelElementReference,
 )
 from dbt_semantic_interfaces.type_enums.dimension_type import DimensionType
+from dbt_semantic_interfaces.type_enums.time_granularity import TimeGranularity
 from dbt_semantic_interfaces.validations.validator_helpers import (
     DimensionInvariants,
     FileContext,
     ModelValidationRule,
     SemanticModelElementContext,
     SemanticModelElementType,
     ValidationError,
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/validations/element_const.py` & `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/validations/element_const.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/validations/entities.py` & `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/validations/entities.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 from datetime import date
 from typing import List, MutableSet
 
-from dbt_semantic_interfaces.objects.elements.entity import EntityType
 from dbt_semantic_interfaces.objects.semantic_manifest import SemanticManifest
 from dbt_semantic_interfaces.objects.semantic_model import SemanticModel
 from dbt_semantic_interfaces.references import SemanticModelReference
+from dbt_semantic_interfaces.type_enums.entity_type import EntityType
 from dbt_semantic_interfaces.validations.validator_helpers import (
     FileContext,
     ModelValidationRule,
     SemanticModelContext,
     ValidationError,
     ValidationFutureError,
     ValidationIssue,
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/validations/measures.py` & `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/validations/measures.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/validations/metrics.py` & `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/validations/metrics.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/validations/non_empty.py` & `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/validations/non_empty.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/validations/reserved_keywords.py` & `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/validations/reserved_keywords.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/validations/semantic_models.py` & `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/validations/semantic_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 from typing import List
 
-from dbt_semantic_interfaces.objects.elements.entity import EntityType
 from dbt_semantic_interfaces.objects.semantic_manifest import SemanticManifest
 from dbt_semantic_interfaces.objects.semantic_model import SemanticModel
 from dbt_semantic_interfaces.references import SemanticModelReference
 from dbt_semantic_interfaces.type_enums.dimension_type import DimensionType
+from dbt_semantic_interfaces.type_enums.entity_type import EntityType
 from dbt_semantic_interfaces.validations.validator_helpers import (
     FileContext,
     ModelValidationRule,
     SemanticModelContext,
     ValidationError,
     ValidationIssue,
     validate_safely,
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/validations/unique_valid_name.py` & `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/validations/unique_valid_name.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 import enum
 import re
 from typing import Dict, List, Optional, Tuple
 
 from dbt_semantic_interfaces.enum_extension import assert_values_exhausted
 from dbt_semantic_interfaces.objects.semantic_manifest import SemanticManifest
 from dbt_semantic_interfaces.objects.semantic_model import SemanticModel
-from dbt_semantic_interfaces.objects.time_granularity import TimeGranularity
 from dbt_semantic_interfaces.references import (
     ElementReference,
     MetricModelReference,
     SemanticModelElementReference,
     SemanticModelReference,
 )
+from dbt_semantic_interfaces.type_enums.time_granularity import TimeGranularity
 from dbt_semantic_interfaces.validations.validator_helpers import (
     FileContext,
     MetricContext,
     ModelValidationRule,
     SemanticModelContext,
     SemanticModelElementContext,
     SemanticModelElementType,
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/dbt_semantic_interfaces/validations/validator_helpers.py` & `dbt_semantic_interfaces-0.1.0.dev1/dbt_semantic_interfaces/validations/validator_helpers.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/tests/test_dataclass_serialization.py` & `dbt_semantic_interfaces-0.1.0.dev1/tests/test_dataclass_serialization.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/tests/test_pretty_print.py` & `dbt_semantic_interfaces-0.1.0.dev1/tests/test_pretty_print.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/tests/fixtures/model_fixtures.py` & `dbt_semantic_interfaces-0.1.0.dev1/tests/fixtures/model_fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/tests/fixtures/model_yamls/simple_model/metrics.yaml` & `dbt_semantic_interfaces-0.1.0.dev1/tests/fixtures/model_yamls/simple_model/metrics.yaml`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/tests/fixtures/model_yamls/simple_model/semantic_models/accounts_source.yaml` & `dbt_semantic_interfaces-0.1.0.dev1/tests/fixtures/model_yamls/simple_model/semantic_models/accounts_source.yaml`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/tests/fixtures/model_yamls/simple_model/semantic_models/bookings_source.yaml` & `dbt_semantic_interfaces-0.1.0.dev1/tests/fixtures/model_yamls/simple_model/semantic_models/bookings_source.yaml`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/tests/fixtures/model_yamls/simple_model/semantic_models/id_verifications.yaml` & `dbt_semantic_interfaces-0.1.0.dev1/tests/fixtures/model_yamls/simple_model/semantic_models/id_verifications.yaml`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/tests/fixtures/model_yamls/simple_model/semantic_models/listings_latest.yaml` & `dbt_semantic_interfaces-0.1.0.dev1/tests/fixtures/model_yamls/simple_model/semantic_models/listings_latest.yaml`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/tests/fixtures/model_yamls/simple_model/semantic_models/user_sm_source.yaml` & `dbt_semantic_interfaces-0.1.0.dev1/tests/fixtures/model_yamls/simple_model/semantic_models/user_sm_source.yaml`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/tests/fixtures/model_yamls/simple_model/semantic_models/views_source.yaml` & `dbt_semantic_interfaces-0.1.0.dev1/tests/fixtures/model_yamls/simple_model/semantic_models/views_source.yaml`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/tests/objects/where_filter/test_parse_calls.py` & `dbt_semantic_interfaces-0.1.0.dev1/tests/objects/where_filter/test_parse_calls.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,20 @@
     DimensionCallParameterSet,
     EntityCallParameterSet,
     FilterCallParameterSets,
     ParseToCallParameterSets,
     TimeDimensionCallParameterSet,
 )
 from dbt_semantic_interfaces.objects.filters.where_filter import WhereFilter
-from dbt_semantic_interfaces.objects.time_granularity import TimeGranularity
 from dbt_semantic_interfaces.references import (
     DimensionReference,
     EntityReference,
     TimeDimensionReference,
 )
+from dbt_semantic_interfaces.type_enums.time_granularity import TimeGranularity
 
 logger = logging.getLogger(__name__)
 
 
 def test_extract_dimension_call_parameter_sets() -> None:  # noqa: D
     parse_result = WhereFilter(
         where_sql_template=(
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/tests/parsing/test_metadata_parsing.py` & `dbt_semantic_interfaces-0.1.0.dev1/tests/parsing/test_metadata_parsing.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/tests/parsing/test_metric_parsing.py` & `dbt_semantic_interfaces-0.1.0.dev1/tests/parsing/test_metric_parsing.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from dbt_semantic_interfaces.objects.filters.where_filter import WhereFilter
 from dbt_semantic_interfaces.objects.metric import (
     MetricInput,
     MetricInputMeasure,
     MetricTimeWindow,
     MetricType,
 )
-from dbt_semantic_interfaces.objects.time_granularity import TimeGranularity
 from dbt_semantic_interfaces.parsing.dir_to_model import parse_yaml_files_to_model
 from dbt_semantic_interfaces.parsing.objects import YamlConfigFile
+from dbt_semantic_interfaces.type_enums.time_granularity import TimeGranularity
 from dbt_semantic_interfaces.validations.validator_helpers import (
     ModelValidationException,
 )
 
 
 def test_legacy_measure_metric_parsing() -> None:
     """Test for parsing a simple metric specification with the `measure` parameter instead of `measures`."""
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/tests/parsing/test_model_deserialization.py` & `dbt_semantic_interfaces-0.1.0.dev1/tests/parsing/test_model_deserialization.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/tests/parsing/test_semantic_model_parsing.py` & `dbt_semantic_interfaces-0.1.0.dev1/tests/parsing/test_semantic_model_parsing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import textwrap
 
-from dbt_semantic_interfaces.objects.elements.entity import EntityType
-from dbt_semantic_interfaces.objects.time_granularity import TimeGranularity
 from dbt_semantic_interfaces.parsing.dir_to_model import parse_yaml_files_to_model
 from dbt_semantic_interfaces.parsing.objects import YamlConfigFile
 from dbt_semantic_interfaces.type_enums.aggregation_type import AggregationType
 from dbt_semantic_interfaces.type_enums.dimension_type import DimensionType
+from dbt_semantic_interfaces.type_enums.entity_type import EntityType
+from dbt_semantic_interfaces.type_enums.time_granularity import TimeGranularity
 
 
 def test_semantic_model_metadata_parsing() -> None:
     """Test for asserting that internal metadata is parsed into the SemanticModel object."""
     yaml_contents = textwrap.dedent(
         """\
         semantic_model:
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/tests/transformations/test_configurable_transform_rules.py` & `dbt_semantic_interfaces-0.1.0.dev1/tests/transformations/test_configurable_transform_rules.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/tests/validations/test_agg_time_dimension.py` & `dbt_semantic_interfaces-0.1.0.dev1/tests/validations/test_agg_time_dimension.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/tests/validations/test_common_entities.py` & `dbt_semantic_interfaces-0.1.0.dev1/tests/validations/test_common_entities.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/tests/validations/test_configurable_rules.py` & `dbt_semantic_interfaces-0.1.0.dev1/tests/validations/test_configurable_rules.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/tests/validations/test_dimension_const.py` & `dbt_semantic_interfaces-0.1.0.dev1/tests/validations/test_dimension_const.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,26 +5,26 @@
     Dimension,
     DimensionTypeParams,
 )
 from dbt_semantic_interfaces.objects.elements.measure import Measure
 from dbt_semantic_interfaces.objects.metric import Metric, MetricType, MetricTypeParams
 from dbt_semantic_interfaces.objects.semantic_manifest import SemanticManifest
 from dbt_semantic_interfaces.objects.semantic_model import NodeRelation, SemanticModel
-from dbt_semantic_interfaces.objects.time_granularity import TimeGranularity
 from dbt_semantic_interfaces.references import (
     DimensionReference,
     MeasureReference,
     TimeDimensionReference,
 )
 from dbt_semantic_interfaces.test_utils import (
     metric_with_guaranteed_meta,
     semantic_model_with_guaranteed_meta,
 )
 from dbt_semantic_interfaces.type_enums.aggregation_type import AggregationType
 from dbt_semantic_interfaces.type_enums.dimension_type import DimensionType
+from dbt_semantic_interfaces.type_enums.time_granularity import TimeGranularity
 from dbt_semantic_interfaces.validations.dimension_const import DimensionConsistencyRule
 from dbt_semantic_interfaces.validations.semantic_models import (
     SemanticModelTimeDimensionWarningsRule,
 )
 from dbt_semantic_interfaces.validations.validator_helpers import (
     ModelValidationException,
 )
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/tests/validations/test_element_const.py` & `dbt_semantic_interfaces-0.1.0.dev1/tests/validations/test_element_const.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/tests/validations/test_entities.py` & `dbt_semantic_interfaces-0.1.0.dev1/tests/validations/test_entities.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import copy
 import re
 import textwrap
 
 import pytest
 
 from dbt_semantic_interfaces.model_validator import ModelValidator
-from dbt_semantic_interfaces.objects.elements.entity import EntityType
 from dbt_semantic_interfaces.objects.semantic_manifest import SemanticManifest
 from dbt_semantic_interfaces.objects.semantic_model import SemanticModel
 from dbt_semantic_interfaces.parsing.dir_to_model import (
     parse_yaml_files_to_validation_ready_model,
 )
 from dbt_semantic_interfaces.parsing.objects import YamlConfigFile
 from dbt_semantic_interfaces.test_utils import (
     base_semantic_manifest_file,
     find_semantic_model_with,
 )
+from dbt_semantic_interfaces.type_enums.entity_type import EntityType
 from dbt_semantic_interfaces.validations.entities import (
     NaturalEntityConfigurationRule,
     OnePrimaryEntityPerSemanticModelRule,
 )
 from dbt_semantic_interfaces.validations.validator_helpers import (
     ModelValidationException,
 )
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/tests/validations/test_measures.py` & `dbt_semantic_interfaces-0.1.0.dev1/tests/validations/test_measures.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/tests/validations/test_metrics.py` & `dbt_semantic_interfaces-0.1.0.dev1/tests/validations/test_metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 import pytest
 
 from dbt_semantic_interfaces.model_validator import ModelValidator
 from dbt_semantic_interfaces.objects.elements.dimension import (
     Dimension,
     DimensionTypeParams,
 )
-from dbt_semantic_interfaces.objects.elements.entity import Entity, EntityType
+from dbt_semantic_interfaces.objects.elements.entity import Entity
 from dbt_semantic_interfaces.objects.elements.measure import Measure
 from dbt_semantic_interfaces.objects.metric import (
     MetricInput,
     MetricType,
     MetricTypeParams,
 )
 from dbt_semantic_interfaces.objects.semantic_manifest import SemanticManifest
-from dbt_semantic_interfaces.objects.time_granularity import TimeGranularity
 from dbt_semantic_interfaces.references import (
     DimensionReference,
     EntityReference,
     TimeDimensionReference,
 )
 from dbt_semantic_interfaces.test_utils import (
     metric_with_guaranteed_meta,
     semantic_model_with_guaranteed_meta,
 )
 from dbt_semantic_interfaces.type_enums.aggregation_type import AggregationType
 from dbt_semantic_interfaces.type_enums.dimension_type import DimensionType
+from dbt_semantic_interfaces.type_enums.entity_type import EntityType
+from dbt_semantic_interfaces.type_enums.time_granularity import TimeGranularity
 from dbt_semantic_interfaces.validations.metrics import DerivedMetricRule
 from dbt_semantic_interfaces.validations.validator_helpers import (
     ModelValidationException,
 )
 
 
 def test_metric_no_time_dim_dim_only_source() -> None:  # noqa:D
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/tests/validations/test_reserved_keywords.py` & `dbt_semantic_interfaces-0.1.0.dev1/tests/validations/test_reserved_keywords.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/tests/validations/test_semantic_models.py` & `dbt_semantic_interfaces-0.1.0.dev1/tests/validations/test_semantic_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import pytest
 
 from dbt_semantic_interfaces.objects.elements.dimension import (
     Dimension,
     DimensionTypeParams,
 )
-from dbt_semantic_interfaces.objects.time_granularity import TimeGranularity
 from dbt_semantic_interfaces.test_utils import semantic_model_with_guaranteed_meta
 from dbt_semantic_interfaces.type_enums.dimension_type import DimensionType
+from dbt_semantic_interfaces.type_enums.time_granularity import TimeGranularity
 from dbt_semantic_interfaces.validations.validator_helpers import (
     ModelValidationException,
 )
 
 
 @pytest.mark.skip("TODO: Will convert to validation rule")
 def test_semantic_model_invalid_sql() -> None:  # noqa:D
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/tests/validations/test_unique_valid_name.py` & `dbt_semantic_interfaces-0.1.0.dev1/tests/validations/test_unique_valid_name.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/tests/validations/test_validator_helpers.py` & `dbt_semantic_interfaces-0.1.0.dev1/tests/validations/test_validator_helpers.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/tests/validations/test_validity_param_definitions.py` & `dbt_semantic_interfaces-0.1.0.dev1/tests/validations/test_validity_param_definitions.py`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/venv-3.9.16/bin/Activate.ps1` & `dbt_semantic_interfaces-0.1.0.dev1/venv-3.9.16/bin/Activate.ps1`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/venv-3.9.16/bin/activate` & `dbt_semantic_interfaces-0.1.0.dev1/venv-3.9.16/bin/activate`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/venv-3.9.16/bin/activate.csh` & `dbt_semantic_interfaces-0.1.0.dev1/venv-3.9.16/bin/activate.csh`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/venv-3.9.16/bin/activate.fish` & `dbt_semantic_interfaces-0.1.0.dev1/venv-3.9.16/bin/activate.fish`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/.gitignore` & `dbt_semantic_interfaces-0.1.0.dev1/.gitignore`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/LICENSE` & `dbt_semantic_interfaces-0.1.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/README.md` & `dbt_semantic_interfaces-0.1.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/pyproject.toml` & `dbt_semantic_interfaces-0.1.0.dev1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dbt-semantic-interfaces"
-version = "0.1.0.dev0"
+version = "0.1.0.dev1"
 description = 'The shared semantic layer definitions that dbt-core and MetricFlow use'
 readme = "README.md"
 requires-python = ">=3.8"
 license = "Apache-2.0"
 keywords = []
 authors = [
   { name = "dbt Labs", email = "info@dbtlabs.com" },
```

### Comparing `dbt_semantic_interfaces-0.1.0.dev0/PKG-INFO` & `dbt_semantic_interfaces-0.1.0.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-semantic-interfaces
-Version: 0.1.0.dev0
+Version: 0.1.0.dev1
 Summary: The shared semantic layer definitions that dbt-core and MetricFlow use
 Author-email: dbt Labs <info@dbtlabs.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-semantic-interfaces Version: 0.1.0.dev0
+Metadata-Version: 2.1 Name: dbt-semantic-interfaces Version: 0.1.0.dev1
 Summary: The shared semantic layer definitions that dbt-core and MetricFlow use
 Author-email: dbt Labs
 dbtlabs.com> License-Expression: Apache-2.0 License-File: LICENSE Classifier:
 Development Status :: 4 - Beta Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
```

