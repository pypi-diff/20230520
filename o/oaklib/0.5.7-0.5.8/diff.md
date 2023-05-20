# Comparing `tmp/oaklib-0.5.7.tar.gz` & `tmp/oaklib-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oaklib-0.5.7.tar", max compression
+gzip compressed data, was "oaklib-0.5.8.tar", max compression
```

## Comparing `oaklib-0.5.7.tar` & `oaklib-0.5.8.tar`

### file list

```diff
@@ -1,274 +1,274 @@
--rw-r--r--   0        0        0    11357 2023-05-19 00:06:17.004512 oaklib-0.5.7/LICENSE
--rw-r--r--   0        0        0     7241 2023-05-19 00:06:17.004512 oaklib-0.5.7/README.md
--rw-r--r--   0        0        0     1880 2023-05-19 00:07:13.982994 oaklib-0.5.7/pyproject.toml
--rw-r--r--   0        0        0      271 2023-05-19 00:06:17.148518 oaklib-0.5.7/src/oaklib/__init__.py
--rw-r--r--   0        0        0   194032 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/cli.py
--rw-r--r--   0        0        0       64 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/conf/__init__.py
--rw-r--r--   0        0        0      372 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/conf/go-human-input-spec.yaml
--rw-r--r--   0        0        0      162 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/conf/go-pombase-input-spec.yaml
--rw-r--r--   0        0        0      109 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/conf/hpoa-g2p-input-spec.yaml
--rw-r--r--   0        0        0      106 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/conf/hpoa-input-spec.yaml
--rw-r--r--   0        0        0     1903 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/conf/lexmatch-rules-oboinowl-default.yaml
--rw-r--r--   0        0        0      562 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/conf/mondo-g2d-input-spec.yaml
--rw-r--r--   0        0        0      109 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/conf/mondo-gencc-input-spec.yaml
--rw-r--r--   0        0        0      118 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/conf/mondo-medgen-g2d-input-spec.yaml
--rw-r--r--   0        0        0     4537 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/conf/obograph-style.json
--rw-r--r--   0        0        0      256 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/conf/omo-to-skos.sssom.tsv
--rw-r--r--   0        0        0      131 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/conf/value-set-expander.conf.yaml
--rw-r--r--   0        0        0      128 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/constants.py
--rw-r--r--   0        0        0        0 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/converters/__init__.py
--rw-r--r--   0        0        0     1456 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/converters/data_model_converter.py
--rw-r--r--   0        0        0     2561 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/converters/logical_definition_flattener.py
--rw-r--r--   0        0        0     2371 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/converters/obo_graph_to_cx_converter.py
--rw-r--r--   0        0        0    12159 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/converters/obo_graph_to_fhir_converter.py
--rw-r--r--   0        0        0     5713 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/converters/obo_graph_to_obo_format_converter.py
--rw-r--r--   0        0        0     5789 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/converters/obo_graph_to_rdf_owl_converter.py
--rw-r--r--   0        0        0       60 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/datamodels/__init__.py
--rw-r--r--   0        0        0     4034 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/datamodels/association.owl.ttl
--rw-r--r--   0        0        0    36266 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/datamodels/association.py
--rw-r--r--   0        0        0    11740 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/datamodels/association.yaml
--rw-r--r--   0        0        0     6165 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/datamodels/class_enrichment.owl.ttl
--rw-r--r--   0        0        0    13328 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/datamodels/class_enrichment.py
--rw-r--r--   0        0        0     3192 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/datamodels/class_enrichment.yaml
--rw-r--r--   0        0        0    19083 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/datamodels/cross_ontology_diff.owl.ttl
--rw-r--r--   0        0        0    24246 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/datamodels/cross_ontology_diff.py
--rw-r--r--   0        0        0    10687 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/datamodels/cross_ontology_diff.yaml
--rw-r--r--   0        0        0    29418 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/datamodels/cx.py
--rw-r--r--   0        0        0     6314 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/datamodels/cx.yaml
--rw-r--r--   0        0        0    15826 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/datamodels/fhir.owl.ttl
--rw-r--r--   0        0        0    35744 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/datamodels/fhir.py
--rw-r--r--   0        0        0     5064 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/datamodels/fhir.yaml
--rw-r--r--   0        0        0    14564 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/datamodels/input_specification.py
--rw-r--r--   0        0        0     3560 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/datamodels/input_specification.yaml
--rw-r--r--   0        0        0    15768 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/datamodels/item_list.py
--rw-r--r--   0        0        0     6339 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/datamodels/item_list.yaml
--rw-r--r--   0        0        0     8984 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/datamodels/lexical_index.owl.ttl
--rw-r--r--   0        0        0    17256 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/datamodels/lexical_index.py
--rw-r--r--   0        0        0     6429 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/datamodels/lexical_index.schema.json
--rw-r--r--   0        0        0     4016 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/datamodels/lexical_index.yaml
--rw-r--r--   0        0        0    26434 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/datamodels/mapping_cluster_datamodel.py
--rw-r--r--   0        0        0     7317 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/datamodels/mapping_cluster_datamodel.yaml
--rw-r--r--   0        0        0   226115 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/datamodels/mapping_rules_datamodel.owl.ttl
--rw-r--r--   0        0        0    32727 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/datamodels/mapping_rules_datamodel.py
--rw-r--r--   0        0        0    12889 2023-05-19 00:06:17.152518 oaklib-0.5.7/src/oaklib/datamodels/mapping_rules_datamodel.schema.json
--rw-r--r--   0        0        0     3607 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/mapping_rules_datamodel.yaml
--rw-r--r--   0        0        0    25354 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/obograph.owl.ttl
--rw-r--r--   0        0        0    46876 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/obograph.py
--rw-r--r--   0        0        0    22375 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/obograph.schema.json
--rw-r--r--   0        0        0    18191 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/obograph.yaml
--rw-r--r--   0        0        0    59793 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/ontology_metadata.owl.ttl
--rw-r--r--   0        0        0   117175 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/ontology_metadata.py
--rw-r--r--   0        0        0    95288 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/ontology_metadata.schema.json
--rw-r--r--   0        0        0    30433 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/ontology_metadata.yaml
--rw-r--r--   0        0        0    14759 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/oxo.owl.ttl
--rw-r--r--   0        0        0    21914 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/oxo.py
--rw-r--r--   0        0        0     4392 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/oxo.yaml
--rw-r--r--   0        0        0     3240 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/search.py
--rw-r--r--   0        0        0    16948 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/search_datamodel.owl.ttl
--rw-r--r--   0        0        0    25145 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/search_datamodel.py
--rw-r--r--   0        0        0     6683 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/search_datamodel.yaml
--rw-r--r--   0        0        0      287 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/settings.py
--rw-r--r--   0        0        0    12767 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/similarity.owl.ttl
--rw-r--r--   0        0        0    22226 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/similarity.py
--rw-r--r--   0        0        0     5511 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/similarity.yaml
--rw-r--r--   0        0        0    31217 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/summary_statistics_datamodel.owl.ttl
--rw-r--r--   0        0        0    50743 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/summary_statistics_datamodel.py
--rw-r--r--   0        0        0    21176 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/summary_statistics_datamodel.schema.json
--rw-r--r--   0        0        0    16246 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/summary_statistics_datamodel.yaml
--rw-r--r--   0        0        0     9909 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/taxon_constraints.owl.ttl
--rw-r--r--   0        0        0    18430 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/taxon_constraints.py
--rw-r--r--   0        0        0     5879 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/taxon_constraints.yaml
--rw-r--r--   0        0        0    11599 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/text_annotator.owl.ttl
--rw-r--r--   0        0        0    20418 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/text_annotator.py
--rw-r--r--   0        0        0     2464 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/text_annotator.schema.json
--rw-r--r--   0        0        0     4219 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/text_annotator.yaml
--rw-r--r--   0        0        0    13670 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/validation_datamodel.owl.ttl
--rw-r--r--   0        0        0    25351 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/validation_datamodel.py
--rw-r--r--   0        0        0    10783 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/validation_datamodel.schema.json
--rw-r--r--   0        0        0     7510 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/validation_datamodel.yaml
--rw-r--r--   0        0        0     6640 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/value_set_configuration.owl.ttl
--rw-r--r--   0        0        0     8458 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/value_set_configuration.py
--rw-r--r--   0        0        0     2276 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/value_set_configuration.yaml
--rw-r--r--   0        0        0     5614 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/datamodels/vocabulary.py
--rw-r--r--   0        0        0     5849 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/implementations/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/implementations/aggregator/__init__.py
--rw-r--r--   0        0        0     5996 2023-05-19 00:06:17.156519 oaklib-0.5.7/src/oaklib/implementations/aggregator/aggregator_implementation.py
--rw-r--r--   0        0        0        0 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/agrkb/__init__.py
--rw-r--r--   0        0        0     8126 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/agrkb/agrkb_implementation.py
--rw-r--r--   0        0        0        0 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/amigo/__init__.py
--rw-r--r--   0        0        0     4601 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/amigo/amigo_implementation.py
--rw-r--r--   0        0        0        0 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/cx/__init__.py
--rw-r--r--   0        0        0     1985 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/cx/cx_implementation.py
--rw-r--r--   0        0        0        0 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/eutils/__init__.py
--rw-r--r--   0        0        0     2179 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/eutils/eutils_implementation.py
--rw-r--r--   0        0        0     1053 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/eutils/pubmed_implementation.py
--rw-r--r--   0        0        0        0 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/fhir/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/funowl/__init__.py
--rw-r--r--   0        0        0     8473 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/funowl/funowl_implementation.py
--rw-r--r--   0        0        0     2313 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/gilda.py
--rw-r--r--   0        0        0        0 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/kgx/__init__.py
--rw-r--r--   0        0        0    30434 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/kgx/kgx_implementation.py
--rw-r--r--   0        0        0        0 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/monarch/__init__.py
--rw-r--r--   0        0        0     7009 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/monarch/monarch_implementation.py
--rw-r--r--   0        0        0        0 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/neo4j/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/obograph/__init__.py
--rw-r--r--   0        0        0    16240 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/obograph/obograph_implementation.py
--rw-r--r--   0        0        0      267 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/ols/__init__.py
--rw-r--r--   0        0        0      132 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/ols/constants.py
--rw-r--r--   0        0        0     7942 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/ols/ols_implementation.py
--rw-r--r--   0        0        0      686 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/ols/oxo_utils.py
--rw-r--r--   0        0        0        0 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/ontobee/__init__.py
--rw-r--r--   0        0        0     2532 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/ontobee/ontobee_implementation.py
--rw-r--r--   0        0        0        0 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/ontoportal/__init__.py
--rw-r--r--   0        0        0      382 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/ontoportal/agroportal_implementation.py
--rw-r--r--   0        0        0     1238 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/ontoportal/bioportal_implementation.py
--rw-r--r--   0        0        0      378 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/ontoportal/ecoportal_implementation.py
--rw-r--r--   0        0        0      378 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/ontoportal/matportal_implementation.py
--rw-r--r--   0        0        0    12106 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/ontoportal/ontoportal_implementation_base.py
--rw-r--r--   0        0        0        0 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/owlery/__init__.py
--rw-r--r--   0        0        0      427 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/owlery/owlery_implementation.py
--rw-r--r--   0        0        0        0 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/pronto/__init__.py
--rw-r--r--   0        0        0    35620 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/pronto/pronto_implementation.py
--rw-r--r--   0        0        0        0 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/robot/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/scigraph/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/semsimian/__init__.py
--rw-r--r--   0        0        0      246 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/semsimian/profiler.py
--rw-r--r--   0        0        0     4110 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/semsimian/semsimian_implementation.py
--rw-r--r--   0        0        0        0 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/simpleobo/__init__.py
--rw-r--r--   0        0        0    34382 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/simpleobo/simple_obo_implementation.py
--rw-r--r--   0        0        0    21451 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/simpleobo/simple_obo_parser.py
--rw-r--r--   0        0        0        0 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/skos/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/solor/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/solr/__init__.py
--rw-r--r--   0        0        0       96 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/sparql/__init__.py
--rw-r--r--   0        0        0    36699 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/sparql/abstract_sparql_implementation.py
--rw-r--r--   0        0        0      885 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/sparql/lov_implementation.py
--rw-r--r--   0        0        0     1721 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/sparql/oak_metamodel_implementation.py
--rw-r--r--   0        0        0     2658 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/sparql/sparql_implementation.py
--rw-r--r--   0        0        0     2326 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/sparql/sparql_query.py
--rw-r--r--   0        0        0       96 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/sqldb/__init__.py
--rw-r--r--   0        0        0   106362 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/sqldb/sql_implementation.py
--rw-r--r--   0        0        0     1903 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/sqldb/sqlite_utils.py
--rw-r--r--   0        0        0        0 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/tccm/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/translator/__init__.py
--rw-r--r--   0        0        0     3283 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/translator/translator_implementation.py
--rw-r--r--   0        0        0      108 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/ubergraph/__init__.py
--rw-r--r--   0        0        0    19393 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/ubergraph/ubergraph_implementation.py
--rw-r--r--   0        0        0        0 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/umls/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 00:06:17.160519 oaklib-0.5.7/src/oaklib/implementations/uniprot/__init__.py
--rw-r--r--   0        0        0     9603 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/implementations/uniprot/uniprot_implementation.py
--rw-r--r--   0        0        0       96 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/implementations/wikidata/__init__.py
--rw-r--r--   0        0        0    17121 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/implementations/wikidata/wikidata_implementation.py
--rw-r--r--   0        0        0      913 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/interfaces/__init__.py
--rw-r--r--   0        0        0    20557 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/interfaces/association_provider_interface.py
--rw-r--r--   0        0        0    50981 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/interfaces/basic_ontology_interface.py
--rw-r--r--   0        0        0     8830 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/interfaces/class_enrichment_calculation_interface.py
--rw-r--r--   0        0        0    11720 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/interfaces/differ_interface.py
--rw-r--r--   0        0        0     2649 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/interfaces/dumper_interface.py
--rw-r--r--   0        0        0      977 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/interfaces/embedding_provider_interface.py
--rw-r--r--   0        0        0    13681 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/interfaces/mapping_provider_interface.py
--rw-r--r--   0        0        0     3262 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/interfaces/merge_interface.py
--rw-r--r--   0        0        0     3103 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/interfaces/metadata_interface.py
--rw-r--r--   0        0        0    18964 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/interfaces/obograph_interface.py
--rw-r--r--   0        0        0     1003 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/interfaces/obolegacy_interface.py
--rw-r--r--   0        0        0      784 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/interfaces/ontology_interface.py
--rw-r--r--   0        0        0    10988 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/interfaces/owl_interface.py
--rw-r--r--   0        0        0     8236 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/interfaces/patcher_interface.py
--rw-r--r--   0        0        0     1955 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/interfaces/rdf_interface.py
--rw-r--r--   0        0        0     2459 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/interfaces/relation_graph_interface.py
--rw-r--r--   0        0        0     3759 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/interfaces/search_interface.py
--rw-r--r--   0        0        0    12778 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/interfaces/semsim_interface.py
--rw-r--r--   0        0        0     1063 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/interfaces/skos_interface.py
--rw-r--r--   0        0        0     2112 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/interfaces/subsetter_interface.py
--rw-r--r--   0        0        0    10140 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/interfaces/summary_statistics_interface.py
--rw-r--r--   0        0        0    18296 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/interfaces/taxon_constraint_interface.py
--rw-r--r--   0        0        0     7511 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/interfaces/text_annotator_interface.py
--rw-r--r--   0        0        0     3033 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/interfaces/validator_interface.py
--rw-r--r--   0        0        0        0 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/io/__init__.py
--rw-r--r--   0        0        0     2087 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/io/heatmap_writer.py
--rw-r--r--   0        0        0     1698 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/io/html_writer.py
--rw-r--r--   0        0        0     1379 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/io/obograph_writer.py
--rw-r--r--   0        0        0     3444 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/io/rollup_report_writer.py
--rw-r--r--   0        0        0      739 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/io/streaming_axiom_writer.py
--rw-r--r--   0        0        0     7906 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/io/streaming_csv_writer.py
--rw-r--r--   0        0        0     1284 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/io/streaming_fhir_writer.py
--rw-r--r--   0        0        0     2524 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/io/streaming_info_writer.py
--rw-r--r--   0        0        0     1231 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/io/streaming_json_lines_writer.py
--rw-r--r--   0        0        0     1806 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/io/streaming_json_writer.py
--rw-r--r--   0        0        0      741 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/io/streaming_kgcl_writer.py
--rw-r--r--   0        0        0     2088 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/io/streaming_markdown_writer.py
--rw-r--r--   0        0        0     1152 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/io/streaming_nl_writer.py
--rw-r--r--   0        0        0     1117 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/io/streaming_obo_json_writer.py
--rw-r--r--   0        0        0     3496 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/io/streaming_obo_writer.py
--rw-r--r--   0        0        0     1270 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/io/streaming_owl_functional_writer.py
--rw-r--r--   0        0        0     2244 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/io/streaming_rdf_writer.py
--rw-r--r--   0        0        0     5129 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/io/streaming_writer.py
--rw-r--r--   0        0        0     1318 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/io/streaming_yaml_writer.py
--rw-r--r--   0        0        0      113 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/mappers/__init__.py
--rw-r--r--   0        0        0     3717 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/mappers/base_mapper.py
--rw-r--r--   0        0        0     1849 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/mappers/ontology_metadata_mapper.py
--rw-r--r--   0        0        0     2179 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/parsers/__init__.py
--rw-r--r--   0        0        0     1524 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/parsers/association_parser.py
--rw-r--r--   0        0        0      522 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/parsers/association_parser_factory.py
--rw-r--r--   0        0        0     4731 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/parsers/boomer_parser.py
--rw-r--r--   0        0        0     2208 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/parsers/gaf_association_parser.py
--rw-r--r--   0        0        0     1090 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/parsers/gencc_association_parser.py
--rw-r--r--   0        0        0     1130 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/parsers/hpoa_association_parser.py
--rw-r--r--   0        0        0      602 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/parsers/hpoa_g2p_association_parser.py
--rw-r--r--   0        0        0      653 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/parsers/kgx_association_parser.py
--rw-r--r--   0        0        0     1666 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/parsers/mim2gene_association_parser.py
--rw-r--r--   0        0        0      525 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/parsers/pairwise_association_parser.py
--rw-r--r--   0        0        0     1432 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/parsers/parser_base.py
--rw-r--r--   0        0        0      707 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/parsers/phaf_association_parser.py
--rw-r--r--   0        0        0     8084 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/parsers/xaf_association_parser.py
--rw-r--r--   0        0        0     2210 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/resource.py
--rw-r--r--   0        0        0    14702 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/selector.py
--rw-r--r--   0        0        0      177 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/types.py
--rw-r--r--   0        0        0        0 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/utilities/__init__.py
--rw-r--r--   0        0        0     1613 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/utilities/apikey_manager.py
--rw-r--r--   0        0        0        0 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/utilities/associations/__init__.py
--rw-r--r--   0        0        0    13441 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/utilities/associations/association_differ.py
--rw-r--r--   0        0        0     3419 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/utilities/associations/association_index.py
--rw-r--r--   0        0        0     1540 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/utilities/basic_utils.py
--rw-r--r--   0        0        0        0 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/utilities/graph/__init__.py
--rw-r--r--   0        0        0     2490 2023-05-19 00:06:17.164519 oaklib-0.5.7/src/oaklib/utilities/graph/networkx_bridge.py
--rw-r--r--   0        0        0     2918 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/graph/relationship_walker.py
--rw-r--r--   0        0        0      993 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/identifier_utils.py
--rw-r--r--   0        0        0      999 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/iterator_utils.py
--rw-r--r--   0        0        0     3345 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/kgcl_utilities.py
--rw-r--r--   0        0        0      850 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/label_utilities.py
--rw-r--r--   0        0        0        0 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/lexical/__init__.py
--rw-r--r--   0        0        0    19516 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/lexical/lexical_indexer.py
--rw-r--r--   0        0        0        0 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/mapping/__init__.py
--rw-r--r--   0        0        0    14467 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/mapping/boomer_utils.py
--rw-r--r--   0        0        0    15328 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/mapping/cross_ontology_diffs.py
--rw-r--r--   0        0        0      751 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/mapping/mapping_propagator.py
--rw-r--r--   0        0        0     2270 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/mapping/mapping_validation.py
--rw-r--r--   0        0        0     2694 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/mapping/sssom_utils.py
--rw-r--r--   0        0        0      684 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/ner_utilities.py
--rw-r--r--   0        0        0        0 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/nlp/__init__.py
--rw-r--r--   0        0        0     3358 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/nlp/natual_language_generation.py
--rw-r--r--   0        0        0      136 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/oboformat_utils.py
--rw-r--r--   0        0        0    22646 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/obograph_utils.py
--rw-r--r--   0        0        0     2275 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/ontology_builder.py
--rw-r--r--   0        0        0      379 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/rate_limiter.py
--rw-r--r--   0        0        0        0 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/reasoning/__init__.py
--rw-r--r--   0        0        0      569 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/reasoning/relation_graph.py
--rw-r--r--   0        0        0        0 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/semsim/__init__.py
--rw-r--r--   0        0        0     1739 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/semsim/similarity_utils.py
--rw-r--r--   0        0        0        0 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/stats/__init__.py
--rw-r--r--   0        0        0     1511 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/stats/hypergeometric.py
--rw-r--r--   0        0        0        0 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/subsets/__init__.py
--rw-r--r--   0        0        0     2819 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/subsets/slimmer_utils.py
--rw-r--r--   0        0        0     4701 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/subsets/subset_analysis.py
--rw-r--r--   0        0        0    11592 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/subsets/value_set_expander.py
--rw-r--r--   0        0        0    13212 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/table_filler.py
--rw-r--r--   0        0        0        0 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/taxon/__init__.py
--rw-r--r--   0        0        0     1743 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/taxon/taxon_constraint_utils.py
--rw-r--r--   0        0        0        0 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/validation/__init__.py
--rw-r--r--   0        0        0    10097 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/validation/definition_ontology_rule.py
--rw-r--r--   0        0        0     7492 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/validation/disjointness_rule.py
--rw-r--r--   0        0        0     1729 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/validation/lint_utils.py
--rw-r--r--   0        0        0     1402 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/validation/ontology_rule.py
--rw-r--r--   0        0        0     1313 2023-05-19 00:06:17.168519 oaklib-0.5.7/src/oaklib/utilities/validation/rule_runner.py
--rw-r--r--   0        0        0     8866 1970-01-01 00:00:00.000000 oaklib-0.5.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-20 02:24:55.498869 oaklib-0.5.8/LICENSE
+-rw-r--r--   0        0        0     7241 2023-05-20 02:24:55.498869 oaklib-0.5.8/README.md
+-rw-r--r--   0        0        0     1880 2023-05-20 02:25:41.823500 oaklib-0.5.8/pyproject.toml
+-rw-r--r--   0        0        0      271 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/__init__.py
+-rw-r--r--   0        0        0   194032 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/cli.py
+-rw-r--r--   0        0        0       64 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/conf/__init__.py
+-rw-r--r--   0        0        0      372 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/conf/go-human-input-spec.yaml
+-rw-r--r--   0        0        0      162 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/conf/go-pombase-input-spec.yaml
+-rw-r--r--   0        0        0      109 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/conf/hpoa-g2p-input-spec.yaml
+-rw-r--r--   0        0        0      106 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/conf/hpoa-input-spec.yaml
+-rw-r--r--   0        0        0     1903 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/conf/lexmatch-rules-oboinowl-default.yaml
+-rw-r--r--   0        0        0      562 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/conf/mondo-g2d-input-spec.yaml
+-rw-r--r--   0        0        0      109 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/conf/mondo-gencc-input-spec.yaml
+-rw-r--r--   0        0        0      118 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/conf/mondo-medgen-g2d-input-spec.yaml
+-rw-r--r--   0        0        0     4537 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/conf/obograph-style.json
+-rw-r--r--   0        0        0      256 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/conf/omo-to-skos.sssom.tsv
+-rw-r--r--   0        0        0      131 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/conf/value-set-expander.conf.yaml
+-rw-r--r--   0        0        0      128 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/constants.py
+-rw-r--r--   0        0        0        0 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/converters/__init__.py
+-rw-r--r--   0        0        0     1456 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/converters/data_model_converter.py
+-rw-r--r--   0        0        0     2561 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/converters/logical_definition_flattener.py
+-rw-r--r--   0        0        0     2371 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/converters/obo_graph_to_cx_converter.py
+-rw-r--r--   0        0        0    12159 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/converters/obo_graph_to_fhir_converter.py
+-rw-r--r--   0        0        0     5713 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/converters/obo_graph_to_obo_format_converter.py
+-rw-r--r--   0        0        0     5789 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/converters/obo_graph_to_rdf_owl_converter.py
+-rw-r--r--   0        0        0       60 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/datamodels/__init__.py
+-rw-r--r--   0        0        0     4034 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/datamodels/association.owl.ttl
+-rw-r--r--   0        0        0    36266 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/datamodels/association.py
+-rw-r--r--   0        0        0    11740 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/datamodels/association.yaml
+-rw-r--r--   0        0        0     6165 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/datamodels/class_enrichment.owl.ttl
+-rw-r--r--   0        0        0    13328 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/datamodels/class_enrichment.py
+-rw-r--r--   0        0        0     3192 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/datamodels/class_enrichment.yaml
+-rw-r--r--   0        0        0    19083 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/datamodels/cross_ontology_diff.owl.ttl
+-rw-r--r--   0        0        0    24246 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/datamodels/cross_ontology_diff.py
+-rw-r--r--   0        0        0    10687 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/datamodels/cross_ontology_diff.yaml
+-rw-r--r--   0        0        0    29418 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/datamodels/cx.py
+-rw-r--r--   0        0        0     6314 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/datamodels/cx.yaml
+-rw-r--r--   0        0        0    15826 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/datamodels/fhir.owl.ttl
+-rw-r--r--   0        0        0    35744 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/datamodels/fhir.py
+-rw-r--r--   0        0        0     5064 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/datamodels/fhir.yaml
+-rw-r--r--   0        0        0    14564 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/datamodels/input_specification.py
+-rw-r--r--   0        0        0     3560 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/datamodels/input_specification.yaml
+-rw-r--r--   0        0        0    15768 2023-05-20 02:24:55.630870 oaklib-0.5.8/src/oaklib/datamodels/item_list.py
+-rw-r--r--   0        0        0     6339 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/item_list.yaml
+-rw-r--r--   0        0        0     8984 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/lexical_index.owl.ttl
+-rw-r--r--   0        0        0    17256 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/lexical_index.py
+-rw-r--r--   0        0        0     6429 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/lexical_index.schema.json
+-rw-r--r--   0        0        0     4016 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/lexical_index.yaml
+-rw-r--r--   0        0        0    26434 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/mapping_cluster_datamodel.py
+-rw-r--r--   0        0        0     7317 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/mapping_cluster_datamodel.yaml
+-rw-r--r--   0        0        0   226115 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/mapping_rules_datamodel.owl.ttl
+-rw-r--r--   0        0        0    32727 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/mapping_rules_datamodel.py
+-rw-r--r--   0        0        0    12889 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/mapping_rules_datamodel.schema.json
+-rw-r--r--   0        0        0     3607 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/mapping_rules_datamodel.yaml
+-rw-r--r--   0        0        0    25354 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/obograph.owl.ttl
+-rw-r--r--   0        0        0    46876 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/obograph.py
+-rw-r--r--   0        0        0    22375 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/obograph.schema.json
+-rw-r--r--   0        0        0    18191 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/obograph.yaml
+-rw-r--r--   0        0        0    59793 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/ontology_metadata.owl.ttl
+-rw-r--r--   0        0        0   117175 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/ontology_metadata.py
+-rw-r--r--   0        0        0    95288 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/ontology_metadata.schema.json
+-rw-r--r--   0        0        0    30433 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/ontology_metadata.yaml
+-rw-r--r--   0        0        0    14759 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/oxo.owl.ttl
+-rw-r--r--   0        0        0    21914 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/oxo.py
+-rw-r--r--   0        0        0     4392 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/oxo.yaml
+-rw-r--r--   0        0        0     3240 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/search.py
+-rw-r--r--   0        0        0    16948 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/search_datamodel.owl.ttl
+-rw-r--r--   0        0        0    25145 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/search_datamodel.py
+-rw-r--r--   0        0        0     6683 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/search_datamodel.yaml
+-rw-r--r--   0        0        0      287 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/settings.py
+-rw-r--r--   0        0        0    12767 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/similarity.owl.ttl
+-rw-r--r--   0        0        0    22226 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/similarity.py
+-rw-r--r--   0        0        0     5511 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/similarity.yaml
+-rw-r--r--   0        0        0    31217 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/summary_statistics_datamodel.owl.ttl
+-rw-r--r--   0        0        0    50743 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/summary_statistics_datamodel.py
+-rw-r--r--   0        0        0    21176 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/summary_statistics_datamodel.schema.json
+-rw-r--r--   0        0        0    16246 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/summary_statistics_datamodel.yaml
+-rw-r--r--   0        0        0     9909 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/taxon_constraints.owl.ttl
+-rw-r--r--   0        0        0    18430 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/taxon_constraints.py
+-rw-r--r--   0        0        0     5879 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/taxon_constraints.yaml
+-rw-r--r--   0        0        0    11599 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/text_annotator.owl.ttl
+-rw-r--r--   0        0        0    20418 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/text_annotator.py
+-rw-r--r--   0        0        0     2464 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/text_annotator.schema.json
+-rw-r--r--   0        0        0     4219 2023-05-20 02:24:55.634870 oaklib-0.5.8/src/oaklib/datamodels/text_annotator.yaml
+-rw-r--r--   0        0        0    13670 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/datamodels/validation_datamodel.owl.ttl
+-rw-r--r--   0        0        0    25351 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/datamodels/validation_datamodel.py
+-rw-r--r--   0        0        0    10783 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/datamodels/validation_datamodel.schema.json
+-rw-r--r--   0        0        0     7510 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/datamodels/validation_datamodel.yaml
+-rw-r--r--   0        0        0     6640 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/datamodels/value_set_configuration.owl.ttl
+-rw-r--r--   0        0        0     8458 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/datamodels/value_set_configuration.py
+-rw-r--r--   0        0        0     2276 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/datamodels/value_set_configuration.yaml
+-rw-r--r--   0        0        0     5614 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/datamodels/vocabulary.py
+-rw-r--r--   0        0        0     5849 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/aggregator/__init__.py
+-rw-r--r--   0        0        0     5996 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/aggregator/aggregator_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/agrkb/__init__.py
+-rw-r--r--   0        0        0     8126 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/agrkb/agrkb_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/amigo/__init__.py
+-rw-r--r--   0        0        0     4601 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/amigo/amigo_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/cx/__init__.py
+-rw-r--r--   0        0        0     1985 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/cx/cx_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/eutils/__init__.py
+-rw-r--r--   0        0        0     2179 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/eutils/eutils_implementation.py
+-rw-r--r--   0        0        0     1053 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/eutils/pubmed_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/fhir/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/funowl/__init__.py
+-rw-r--r--   0        0        0     8473 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/funowl/funowl_implementation.py
+-rw-r--r--   0        0        0     2313 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/gilda.py
+-rw-r--r--   0        0        0        0 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/kgx/__init__.py
+-rw-r--r--   0        0        0    30434 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/kgx/kgx_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/monarch/__init__.py
+-rw-r--r--   0        0        0     7009 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/monarch/monarch_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/neo4j/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/obograph/__init__.py
+-rw-r--r--   0        0        0    16240 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/obograph/obograph_implementation.py
+-rw-r--r--   0        0        0      267 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/ols/__init__.py
+-rw-r--r--   0        0        0      132 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/ols/constants.py
+-rw-r--r--   0        0        0     7942 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/ols/ols_implementation.py
+-rw-r--r--   0        0        0      686 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/ols/oxo_utils.py
+-rw-r--r--   0        0        0        0 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/ontobee/__init__.py
+-rw-r--r--   0        0        0     2532 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/ontobee/ontobee_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/ontoportal/__init__.py
+-rw-r--r--   0        0        0      382 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/ontoportal/agroportal_implementation.py
+-rw-r--r--   0        0        0     1238 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/ontoportal/bioportal_implementation.py
+-rw-r--r--   0        0        0      378 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/ontoportal/ecoportal_implementation.py
+-rw-r--r--   0        0        0      378 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/ontoportal/matportal_implementation.py
+-rw-r--r--   0        0        0    12106 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/ontoportal/ontoportal_implementation_base.py
+-rw-r--r--   0        0        0        0 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/owlery/__init__.py
+-rw-r--r--   0        0        0      427 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/owlery/owlery_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/pronto/__init__.py
+-rw-r--r--   0        0        0    35620 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/pronto/pronto_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/robot/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/scigraph/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/semsimian/__init__.py
+-rw-r--r--   0        0        0      246 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/semsimian/profiler.py
+-rw-r--r--   0        0        0     4110 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/semsimian/semsimian_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/simpleobo/__init__.py
+-rw-r--r--   0        0        0    34382 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/simpleobo/simple_obo_implementation.py
+-rw-r--r--   0        0        0    21451 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/simpleobo/simple_obo_parser.py
+-rw-r--r--   0        0        0        0 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/skos/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/solor/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/solr/__init__.py
+-rw-r--r--   0        0        0       96 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/sparql/__init__.py
+-rw-r--r--   0        0        0    36699 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/sparql/abstract_sparql_implementation.py
+-rw-r--r--   0        0        0      885 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/sparql/lov_implementation.py
+-rw-r--r--   0        0        0     1721 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/sparql/oak_metamodel_implementation.py
+-rw-r--r--   0        0        0     2658 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/sparql/sparql_implementation.py
+-rw-r--r--   0        0        0     2326 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/sparql/sparql_query.py
+-rw-r--r--   0        0        0       96 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/sqldb/__init__.py
+-rw-r--r--   0        0        0   106362 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/sqldb/sql_implementation.py
+-rw-r--r--   0        0        0     1903 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/sqldb/sqlite_utils.py
+-rw-r--r--   0        0        0        0 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/tccm/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/translator/__init__.py
+-rw-r--r--   0        0        0     3283 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/translator/translator_implementation.py
+-rw-r--r--   0        0        0      108 2023-05-20 02:24:55.638870 oaklib-0.5.8/src/oaklib/implementations/ubergraph/__init__.py
+-rw-r--r--   0        0        0    19393 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/implementations/ubergraph/ubergraph_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/implementations/umls/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/implementations/uniprot/__init__.py
+-rw-r--r--   0        0        0     9603 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/implementations/uniprot/uniprot_implementation.py
+-rw-r--r--   0        0        0       96 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/implementations/wikidata/__init__.py
+-rw-r--r--   0        0        0    17121 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/implementations/wikidata/wikidata_implementation.py
+-rw-r--r--   0        0        0      913 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/interfaces/__init__.py
+-rw-r--r--   0        0        0    20557 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/interfaces/association_provider_interface.py
+-rw-r--r--   0        0        0    50981 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/interfaces/basic_ontology_interface.py
+-rw-r--r--   0        0        0     8830 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/interfaces/class_enrichment_calculation_interface.py
+-rw-r--r--   0        0        0    11720 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/interfaces/differ_interface.py
+-rw-r--r--   0        0        0     2649 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/interfaces/dumper_interface.py
+-rw-r--r--   0        0        0      977 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/interfaces/embedding_provider_interface.py
+-rw-r--r--   0        0        0    13681 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/interfaces/mapping_provider_interface.py
+-rw-r--r--   0        0        0     3262 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/interfaces/merge_interface.py
+-rw-r--r--   0        0        0     3103 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/interfaces/metadata_interface.py
+-rw-r--r--   0        0        0    18964 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/interfaces/obograph_interface.py
+-rw-r--r--   0        0        0     1003 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/interfaces/obolegacy_interface.py
+-rw-r--r--   0        0        0      784 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/interfaces/ontology_interface.py
+-rw-r--r--   0        0        0    10988 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/interfaces/owl_interface.py
+-rw-r--r--   0        0        0     8236 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/interfaces/patcher_interface.py
+-rw-r--r--   0        0        0     1955 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/interfaces/rdf_interface.py
+-rw-r--r--   0        0        0     2459 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/interfaces/relation_graph_interface.py
+-rw-r--r--   0        0        0     3759 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/interfaces/search_interface.py
+-rw-r--r--   0        0        0    12778 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/interfaces/semsim_interface.py
+-rw-r--r--   0        0        0     1063 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/interfaces/skos_interface.py
+-rw-r--r--   0        0        0     2112 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/interfaces/subsetter_interface.py
+-rw-r--r--   0        0        0    10140 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/interfaces/summary_statistics_interface.py
+-rw-r--r--   0        0        0    18296 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/interfaces/taxon_constraint_interface.py
+-rw-r--r--   0        0        0     7566 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/interfaces/text_annotator_interface.py
+-rw-r--r--   0        0        0     3033 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/interfaces/validator_interface.py
+-rw-r--r--   0        0        0        0 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/io/__init__.py
+-rw-r--r--   0        0        0     2087 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/io/heatmap_writer.py
+-rw-r--r--   0        0        0     1698 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/io/html_writer.py
+-rw-r--r--   0        0        0     1379 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/io/obograph_writer.py
+-rw-r--r--   0        0        0     3444 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/io/rollup_report_writer.py
+-rw-r--r--   0        0        0      739 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/io/streaming_axiom_writer.py
+-rw-r--r--   0        0        0     7906 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/io/streaming_csv_writer.py
+-rw-r--r--   0        0        0     1284 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/io/streaming_fhir_writer.py
+-rw-r--r--   0        0        0     2524 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/io/streaming_info_writer.py
+-rw-r--r--   0        0        0     1231 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/io/streaming_json_lines_writer.py
+-rw-r--r--   0        0        0     1806 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/io/streaming_json_writer.py
+-rw-r--r--   0        0        0      741 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/io/streaming_kgcl_writer.py
+-rw-r--r--   0        0        0     2088 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/io/streaming_markdown_writer.py
+-rw-r--r--   0        0        0     1152 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/io/streaming_nl_writer.py
+-rw-r--r--   0        0        0     1117 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/io/streaming_obo_json_writer.py
+-rw-r--r--   0        0        0     3496 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/io/streaming_obo_writer.py
+-rw-r--r--   0        0        0     1270 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/io/streaming_owl_functional_writer.py
+-rw-r--r--   0        0        0     2244 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/io/streaming_rdf_writer.py
+-rw-r--r--   0        0        0     5129 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/io/streaming_writer.py
+-rw-r--r--   0        0        0     1318 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/io/streaming_yaml_writer.py
+-rw-r--r--   0        0        0      113 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/mappers/__init__.py
+-rw-r--r--   0        0        0     3717 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/mappers/base_mapper.py
+-rw-r--r--   0        0        0     1849 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/mappers/ontology_metadata_mapper.py
+-rw-r--r--   0        0        0     2179 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/parsers/__init__.py
+-rw-r--r--   0        0        0     1524 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/parsers/association_parser.py
+-rw-r--r--   0        0        0      522 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/parsers/association_parser_factory.py
+-rw-r--r--   0        0        0     4731 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/parsers/boomer_parser.py
+-rw-r--r--   0        0        0     2208 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/parsers/gaf_association_parser.py
+-rw-r--r--   0        0        0     1090 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/parsers/gencc_association_parser.py
+-rw-r--r--   0        0        0     1130 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/parsers/hpoa_association_parser.py
+-rw-r--r--   0        0        0      602 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/parsers/hpoa_g2p_association_parser.py
+-rw-r--r--   0        0        0      653 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/parsers/kgx_association_parser.py
+-rw-r--r--   0        0        0     1666 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/parsers/mim2gene_association_parser.py
+-rw-r--r--   0        0        0      525 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/parsers/pairwise_association_parser.py
+-rw-r--r--   0        0        0     1432 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/parsers/parser_base.py
+-rw-r--r--   0        0        0      707 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/parsers/phaf_association_parser.py
+-rw-r--r--   0        0        0     8084 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/parsers/xaf_association_parser.py
+-rw-r--r--   0        0        0     2210 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/resource.py
+-rw-r--r--   0        0        0    14702 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/selector.py
+-rw-r--r--   0        0        0      177 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/types.py
+-rw-r--r--   0        0        0        0 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/utilities/__init__.py
+-rw-r--r--   0        0        0     1613 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/utilities/apikey_manager.py
+-rw-r--r--   0        0        0        0 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/utilities/associations/__init__.py
+-rw-r--r--   0        0        0    13441 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/utilities/associations/association_differ.py
+-rw-r--r--   0        0        0     3419 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/utilities/associations/association_index.py
+-rw-r--r--   0        0        0     1540 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/utilities/basic_utils.py
+-rw-r--r--   0        0        0        0 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/utilities/graph/__init__.py
+-rw-r--r--   0        0        0     2490 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/utilities/graph/networkx_bridge.py
+-rw-r--r--   0        0        0     2918 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/utilities/graph/relationship_walker.py
+-rw-r--r--   0        0        0      993 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/utilities/identifier_utils.py
+-rw-r--r--   0        0        0      999 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/utilities/iterator_utils.py
+-rw-r--r--   0        0        0     3345 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/utilities/kgcl_utilities.py
+-rw-r--r--   0        0        0      850 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/utilities/label_utilities.py
+-rw-r--r--   0        0        0        0 2023-05-20 02:24:55.642870 oaklib-0.5.8/src/oaklib/utilities/lexical/__init__.py
+-rw-r--r--   0        0        0    19516 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/lexical/lexical_indexer.py
+-rw-r--r--   0        0        0        0 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/mapping/__init__.py
+-rw-r--r--   0        0        0    14467 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/mapping/boomer_utils.py
+-rw-r--r--   0        0        0    15328 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/mapping/cross_ontology_diffs.py
+-rw-r--r--   0        0        0      751 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/mapping/mapping_propagator.py
+-rw-r--r--   0        0        0     2270 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/mapping/mapping_validation.py
+-rw-r--r--   0        0        0     2694 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/mapping/sssom_utils.py
+-rw-r--r--   0        0        0      684 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/ner_utilities.py
+-rw-r--r--   0        0        0        0 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/nlp/__init__.py
+-rw-r--r--   0        0        0     3358 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/nlp/natual_language_generation.py
+-rw-r--r--   0        0        0      136 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/oboformat_utils.py
+-rw-r--r--   0        0        0    22646 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/obograph_utils.py
+-rw-r--r--   0        0        0     2275 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/ontology_builder.py
+-rw-r--r--   0        0        0      379 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/rate_limiter.py
+-rw-r--r--   0        0        0        0 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/reasoning/__init__.py
+-rw-r--r--   0        0        0      569 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/reasoning/relation_graph.py
+-rw-r--r--   0        0        0        0 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/semsim/__init__.py
+-rw-r--r--   0        0        0     1739 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/semsim/similarity_utils.py
+-rw-r--r--   0        0        0        0 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/stats/__init__.py
+-rw-r--r--   0        0        0     1511 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/stats/hypergeometric.py
+-rw-r--r--   0        0        0        0 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/subsets/__init__.py
+-rw-r--r--   0        0        0     2819 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/subsets/slimmer_utils.py
+-rw-r--r--   0        0        0     4701 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/subsets/subset_analysis.py
+-rw-r--r--   0        0        0    11592 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/subsets/value_set_expander.py
+-rw-r--r--   0        0        0    13212 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/table_filler.py
+-rw-r--r--   0        0        0        0 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/taxon/__init__.py
+-rw-r--r--   0        0        0     1743 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/taxon/taxon_constraint_utils.py
+-rw-r--r--   0        0        0        0 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/validation/__init__.py
+-rw-r--r--   0        0        0    10097 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/validation/definition_ontology_rule.py
+-rw-r--r--   0        0        0     7492 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/validation/disjointness_rule.py
+-rw-r--r--   0        0        0     1729 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/validation/lint_utils.py
+-rw-r--r--   0        0        0     1402 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/validation/ontology_rule.py
+-rw-r--r--   0        0        0     1313 2023-05-20 02:24:55.646870 oaklib-0.5.8/src/oaklib/utilities/validation/rule_runner.py
+-rw-r--r--   0        0        0     8866 1970-01-01 00:00:00.000000 oaklib-0.5.8/PKG-INFO
```

### Comparing `oaklib-0.5.7/LICENSE` & `oaklib-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/README.md` & `oaklib-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/pyproject.toml` & `oaklib-0.5.8/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oaklib"
-version = "v0.5.7"
+version = "v0.5.8"
 description = "Ontology Access Kit: Python library for common ontology operations over a variety of backends"
 authors = ["cmungall <cjm@berkeleybop.org>"]
 
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0.0"
```

### Comparing `oaklib-0.5.7/src/oaklib/cli.py` & `oaklib-0.5.8/src/oaklib/cli.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/conf/lexmatch-rules-oboinowl-default.yaml` & `oaklib-0.5.8/src/oaklib/conf/lexmatch-rules-oboinowl-default.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/conf/mondo-g2d-input-spec.yaml` & `oaklib-0.5.8/src/oaklib/conf/mondo-g2d-input-spec.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/conf/obograph-style.json` & `oaklib-0.5.8/src/oaklib/conf/obograph-style.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/converters/data_model_converter.py` & `oaklib-0.5.8/src/oaklib/converters/data_model_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/converters/logical_definition_flattener.py` & `oaklib-0.5.8/src/oaklib/converters/logical_definition_flattener.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/converters/obo_graph_to_cx_converter.py` & `oaklib-0.5.8/src/oaklib/converters/obo_graph_to_cx_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/converters/obo_graph_to_fhir_converter.py` & `oaklib-0.5.8/src/oaklib/converters/obo_graph_to_fhir_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/converters/obo_graph_to_obo_format_converter.py` & `oaklib-0.5.8/src/oaklib/converters/obo_graph_to_obo_format_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/converters/obo_graph_to_rdf_owl_converter.py` & `oaklib-0.5.8/src/oaklib/converters/obo_graph_to_rdf_owl_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/association.owl.ttl` & `oaklib-0.5.8/src/oaklib/datamodels/association.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/association.py` & `oaklib-0.5.8/src/oaklib/datamodels/association.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/association.yaml` & `oaklib-0.5.8/src/oaklib/datamodels/association.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/class_enrichment.owl.ttl` & `oaklib-0.5.8/src/oaklib/datamodels/class_enrichment.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/class_enrichment.py` & `oaklib-0.5.8/src/oaklib/datamodels/class_enrichment.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/class_enrichment.yaml` & `oaklib-0.5.8/src/oaklib/datamodels/class_enrichment.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/cross_ontology_diff.owl.ttl` & `oaklib-0.5.8/src/oaklib/datamodels/cross_ontology_diff.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/cross_ontology_diff.py` & `oaklib-0.5.8/src/oaklib/datamodels/cross_ontology_diff.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/cross_ontology_diff.yaml` & `oaklib-0.5.8/src/oaklib/datamodels/cross_ontology_diff.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/cx.py` & `oaklib-0.5.8/src/oaklib/datamodels/cx.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/cx.yaml` & `oaklib-0.5.8/src/oaklib/datamodels/cx.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/fhir.owl.ttl` & `oaklib-0.5.8/src/oaklib/datamodels/fhir.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/fhir.py` & `oaklib-0.5.8/src/oaklib/datamodels/fhir.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/fhir.yaml` & `oaklib-0.5.8/src/oaklib/datamodels/fhir.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/input_specification.py` & `oaklib-0.5.8/src/oaklib/datamodels/input_specification.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/input_specification.yaml` & `oaklib-0.5.8/src/oaklib/datamodels/input_specification.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/item_list.py` & `oaklib-0.5.8/src/oaklib/datamodels/item_list.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/item_list.yaml` & `oaklib-0.5.8/src/oaklib/datamodels/item_list.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/lexical_index.owl.ttl` & `oaklib-0.5.8/src/oaklib/datamodels/lexical_index.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/lexical_index.py` & `oaklib-0.5.8/src/oaklib/datamodels/lexical_index.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/lexical_index.schema.json` & `oaklib-0.5.8/src/oaklib/datamodels/lexical_index.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/lexical_index.yaml` & `oaklib-0.5.8/src/oaklib/datamodels/lexical_index.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/mapping_cluster_datamodel.py` & `oaklib-0.5.8/src/oaklib/datamodels/mapping_cluster_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/mapping_cluster_datamodel.yaml` & `oaklib-0.5.8/src/oaklib/datamodels/mapping_cluster_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/mapping_rules_datamodel.owl.ttl` & `oaklib-0.5.8/src/oaklib/datamodels/mapping_rules_datamodel.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/mapping_rules_datamodel.py` & `oaklib-0.5.8/src/oaklib/datamodels/mapping_rules_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/mapping_rules_datamodel.schema.json` & `oaklib-0.5.8/src/oaklib/datamodels/mapping_rules_datamodel.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/mapping_rules_datamodel.yaml` & `oaklib-0.5.8/src/oaklib/datamodels/mapping_rules_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/obograph.owl.ttl` & `oaklib-0.5.8/src/oaklib/datamodels/obograph.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/obograph.py` & `oaklib-0.5.8/src/oaklib/datamodels/obograph.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/obograph.schema.json` & `oaklib-0.5.8/src/oaklib/datamodels/obograph.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/obograph.yaml` & `oaklib-0.5.8/src/oaklib/datamodels/obograph.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/ontology_metadata.owl.ttl` & `oaklib-0.5.8/src/oaklib/datamodels/ontology_metadata.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/ontology_metadata.py` & `oaklib-0.5.8/src/oaklib/datamodels/ontology_metadata.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/ontology_metadata.schema.json` & `oaklib-0.5.8/src/oaklib/datamodels/ontology_metadata.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/ontology_metadata.yaml` & `oaklib-0.5.8/src/oaklib/datamodels/ontology_metadata.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/oxo.owl.ttl` & `oaklib-0.5.8/src/oaklib/datamodels/oxo.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/oxo.py` & `oaklib-0.5.8/src/oaklib/datamodels/oxo.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/oxo.yaml` & `oaklib-0.5.8/src/oaklib/datamodels/oxo.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/search.py` & `oaklib-0.5.8/src/oaklib/datamodels/search.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/search_datamodel.owl.ttl` & `oaklib-0.5.8/src/oaklib/datamodels/search_datamodel.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/search_datamodel.py` & `oaklib-0.5.8/src/oaklib/datamodels/search_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/search_datamodel.yaml` & `oaklib-0.5.8/src/oaklib/datamodels/search_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/similarity.owl.ttl` & `oaklib-0.5.8/src/oaklib/datamodels/similarity.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/similarity.py` & `oaklib-0.5.8/src/oaklib/datamodels/similarity.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/similarity.yaml` & `oaklib-0.5.8/src/oaklib/datamodels/similarity.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/summary_statistics_datamodel.owl.ttl` & `oaklib-0.5.8/src/oaklib/datamodels/summary_statistics_datamodel.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/summary_statistics_datamodel.py` & `oaklib-0.5.8/src/oaklib/datamodels/summary_statistics_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/summary_statistics_datamodel.schema.json` & `oaklib-0.5.8/src/oaklib/datamodels/summary_statistics_datamodel.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/summary_statistics_datamodel.yaml` & `oaklib-0.5.8/src/oaklib/datamodels/summary_statistics_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/taxon_constraints.owl.ttl` & `oaklib-0.5.8/src/oaklib/datamodels/taxon_constraints.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/taxon_constraints.py` & `oaklib-0.5.8/src/oaklib/datamodels/taxon_constraints.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/taxon_constraints.yaml` & `oaklib-0.5.8/src/oaklib/datamodels/taxon_constraints.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/text_annotator.owl.ttl` & `oaklib-0.5.8/src/oaklib/datamodels/text_annotator.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/text_annotator.py` & `oaklib-0.5.8/src/oaklib/datamodels/text_annotator.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/text_annotator.schema.json` & `oaklib-0.5.8/src/oaklib/datamodels/text_annotator.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/text_annotator.yaml` & `oaklib-0.5.8/src/oaklib/datamodels/text_annotator.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/validation_datamodel.owl.ttl` & `oaklib-0.5.8/src/oaklib/datamodels/validation_datamodel.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/validation_datamodel.py` & `oaklib-0.5.8/src/oaklib/datamodels/validation_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/validation_datamodel.schema.json` & `oaklib-0.5.8/src/oaklib/datamodels/validation_datamodel.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/validation_datamodel.yaml` & `oaklib-0.5.8/src/oaklib/datamodels/validation_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/value_set_configuration.owl.ttl` & `oaklib-0.5.8/src/oaklib/datamodels/value_set_configuration.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/value_set_configuration.py` & `oaklib-0.5.8/src/oaklib/datamodels/value_set_configuration.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/value_set_configuration.yaml` & `oaklib-0.5.8/src/oaklib/datamodels/value_set_configuration.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/datamodels/vocabulary.py` & `oaklib-0.5.8/src/oaklib/datamodels/vocabulary.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/implementations/__init__.py` & `oaklib-0.5.8/src/oaklib/implementations/__init__.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/implementations/aggregator/aggregator_implementation.py` & `oaklib-0.5.8/src/oaklib/implementations/aggregator/aggregator_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/implementations/agrkb/agrkb_implementation.py` & `oaklib-0.5.8/src/oaklib/implementations/agrkb/agrkb_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/implementations/amigo/amigo_implementation.py` & `oaklib-0.5.8/src/oaklib/implementations/amigo/amigo_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/implementations/cx/cx_implementation.py` & `oaklib-0.5.8/src/oaklib/implementations/cx/cx_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/implementations/eutils/eutils_implementation.py` & `oaklib-0.5.8/src/oaklib/implementations/eutils/eutils_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/implementations/eutils/pubmed_implementation.py` & `oaklib-0.5.8/src/oaklib/implementations/eutils/pubmed_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/implementations/funowl/funowl_implementation.py` & `oaklib-0.5.8/src/oaklib/implementations/funowl/funowl_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/implementations/gilda.py` & `oaklib-0.5.8/src/oaklib/implementations/gilda.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/implementations/kgx/kgx_implementation.py` & `oaklib-0.5.8/src/oaklib/implementations/kgx/kgx_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/implementations/monarch/monarch_implementation.py` & `oaklib-0.5.8/src/oaklib/implementations/monarch/monarch_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/implementations/obograph/obograph_implementation.py` & `oaklib-0.5.8/src/oaklib/implementations/obograph/obograph_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/implementations/ols/ols_implementation.py` & `oaklib-0.5.8/src/oaklib/implementations/ols/ols_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/implementations/ols/oxo_utils.py` & `oaklib-0.5.8/src/oaklib/implementations/ols/oxo_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/implementations/ontobee/ontobee_implementation.py` & `oaklib-0.5.8/src/oaklib/implementations/ontobee/ontobee_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/implementations/ontoportal/bioportal_implementation.py` & `oaklib-0.5.8/src/oaklib/implementations/ontoportal/bioportal_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/implementations/ontoportal/ontoportal_implementation_base.py` & `oaklib-0.5.8/src/oaklib/implementations/ontoportal/ontoportal_implementation_base.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/implementations/pronto/pronto_implementation.py` & `oaklib-0.5.8/src/oaklib/implementations/pronto/pronto_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/implementations/semsimian/semsimian_implementation.py` & `oaklib-0.5.8/src/oaklib/implementations/semsimian/semsimian_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/implementations/simpleobo/simple_obo_implementation.py` & `oaklib-0.5.8/src/oaklib/implementations/simpleobo/simple_obo_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/implementations/simpleobo/simple_obo_parser.py` & `oaklib-0.5.8/src/oaklib/implementations/simpleobo/simple_obo_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/implementations/sparql/abstract_sparql_implementation.py` & `oaklib-0.5.8/src/oaklib/implementations/sparql/abstract_sparql_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/implementations/sparql/lov_implementation.py` & `oaklib-0.5.8/src/oaklib/implementations/sparql/lov_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/implementations/sparql/oak_metamodel_implementation.py` & `oaklib-0.5.8/src/oaklib/implementations/sparql/oak_metamodel_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/implementations/sparql/sparql_implementation.py` & `oaklib-0.5.8/src/oaklib/implementations/sparql/sparql_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/implementations/sparql/sparql_query.py` & `oaklib-0.5.8/src/oaklib/implementations/sparql/sparql_query.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/implementations/sqldb/sql_implementation.py` & `oaklib-0.5.8/src/oaklib/implementations/sqldb/sql_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/implementations/sqldb/sqlite_utils.py` & `oaklib-0.5.8/src/oaklib/implementations/sqldb/sqlite_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/implementations/translator/translator_implementation.py` & `oaklib-0.5.8/src/oaklib/implementations/translator/translator_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/implementations/ubergraph/ubergraph_implementation.py` & `oaklib-0.5.8/src/oaklib/implementations/ubergraph/ubergraph_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/implementations/uniprot/uniprot_implementation.py` & `oaklib-0.5.8/src/oaklib/implementations/uniprot/uniprot_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/implementations/wikidata/wikidata_implementation.py` & `oaklib-0.5.8/src/oaklib/implementations/wikidata/wikidata_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/interfaces/__init__.py` & `oaklib-0.5.8/src/oaklib/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/interfaces/association_provider_interface.py` & `oaklib-0.5.8/src/oaklib/interfaces/association_provider_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/interfaces/basic_ontology_interface.py` & `oaklib-0.5.8/src/oaklib/interfaces/basic_ontology_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/interfaces/class_enrichment_calculation_interface.py` & `oaklib-0.5.8/src/oaklib/interfaces/class_enrichment_calculation_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/interfaces/differ_interface.py` & `oaklib-0.5.8/src/oaklib/interfaces/differ_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/interfaces/dumper_interface.py` & `oaklib-0.5.8/src/oaklib/interfaces/dumper_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/interfaces/embedding_provider_interface.py` & `oaklib-0.5.8/src/oaklib/interfaces/embedding_provider_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/interfaces/mapping_provider_interface.py` & `oaklib-0.5.8/src/oaklib/interfaces/mapping_provider_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/interfaces/merge_interface.py` & `oaklib-0.5.8/src/oaklib/interfaces/merge_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/interfaces/metadata_interface.py` & `oaklib-0.5.8/src/oaklib/interfaces/metadata_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/interfaces/obograph_interface.py` & `oaklib-0.5.8/src/oaklib/interfaces/obograph_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/interfaces/obolegacy_interface.py` & `oaklib-0.5.8/src/oaklib/interfaces/obolegacy_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/interfaces/ontology_interface.py` & `oaklib-0.5.8/src/oaklib/interfaces/ontology_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/interfaces/owl_interface.py` & `oaklib-0.5.8/src/oaklib/interfaces/owl_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/interfaces/patcher_interface.py` & `oaklib-0.5.8/src/oaklib/interfaces/patcher_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/interfaces/rdf_interface.py` & `oaklib-0.5.8/src/oaklib/interfaces/rdf_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/interfaces/relation_graph_interface.py` & `oaklib-0.5.8/src/oaklib/interfaces/relation_graph_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/interfaces/search_interface.py` & `oaklib-0.5.8/src/oaklib/interfaces/search_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/interfaces/semsim_interface.py` & `oaklib-0.5.8/src/oaklib/interfaces/semsim_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/interfaces/skos_interface.py` & `oaklib-0.5.8/src/oaklib/interfaces/skos_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/interfaces/subsetter_interface.py` & `oaklib-0.5.8/src/oaklib/interfaces/subsetter_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/interfaces/summary_statistics_interface.py` & `oaklib-0.5.8/src/oaklib/interfaces/summary_statistics_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/interfaces/taxon_constraint_interface.py` & `oaklib-0.5.8/src/oaklib/interfaces/taxon_constraint_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/interfaces/text_annotator_interface.py` & `oaklib-0.5.8/src/oaklib/interfaces/text_annotator_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,24 +126,25 @@
                     label = self.label(object_id)
                     yield nen_annotation(text=text, object_id=object_id, object_label=label)
             else:
                 raise NotImplementedError(
                     f"{self.__class__.__name__} can't be used to match partial text"
                 )
         else:
-            logging.info("Indexing ontology...")
             if self.cache_directory:
                 index_name = f"{self.resource.scheme}-{self.resource.slug}-index.yaml"
                 index_path = str(Path(self.cache_directory) / index_name)
                 logging.info(f"Caching to {index_path}")
             else:
                 index_path = None
-            self.lexical_index = create_or_load_lexical_index(
-                index_path, self, mapping_rule_collection=self.rule_collection
-            )
+            if not self.lexical_index:
+                logging.info("Indexing ontology...")
+                self.lexical_index = create_or_load_lexical_index(
+                    index_path, self, mapping_rule_collection=self.rule_collection
+                )
             logging.info("Performing naive search using lexical index")
             li = self.lexical_index
             text_lower = text.lower()
             for k, grouping in li.groupings.items():
                 if k in text_lower:
                     ix = text_lower.index(k)
                     # TODO: make configurable. Exclude mid-word matches
```

### Comparing `oaklib-0.5.7/src/oaklib/interfaces/validator_interface.py` & `oaklib-0.5.8/src/oaklib/interfaces/validator_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/io/heatmap_writer.py` & `oaklib-0.5.8/src/oaklib/io/heatmap_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/io/html_writer.py` & `oaklib-0.5.8/src/oaklib/io/html_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/io/obograph_writer.py` & `oaklib-0.5.8/src/oaklib/io/obograph_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/io/rollup_report_writer.py` & `oaklib-0.5.8/src/oaklib/io/rollup_report_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/io/streaming_axiom_writer.py` & `oaklib-0.5.8/src/oaklib/io/streaming_axiom_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/io/streaming_csv_writer.py` & `oaklib-0.5.8/src/oaklib/io/streaming_csv_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/io/streaming_fhir_writer.py` & `oaklib-0.5.8/src/oaklib/io/streaming_fhir_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/io/streaming_info_writer.py` & `oaklib-0.5.8/src/oaklib/io/streaming_info_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/io/streaming_json_lines_writer.py` & `oaklib-0.5.8/src/oaklib/io/streaming_json_lines_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/io/streaming_json_writer.py` & `oaklib-0.5.8/src/oaklib/io/streaming_json_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/io/streaming_kgcl_writer.py` & `oaklib-0.5.8/src/oaklib/io/streaming_kgcl_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/io/streaming_markdown_writer.py` & `oaklib-0.5.8/src/oaklib/io/streaming_markdown_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/io/streaming_nl_writer.py` & `oaklib-0.5.8/src/oaklib/io/streaming_nl_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/io/streaming_obo_json_writer.py` & `oaklib-0.5.8/src/oaklib/io/streaming_obo_json_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/io/streaming_obo_writer.py` & `oaklib-0.5.8/src/oaklib/io/streaming_obo_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/io/streaming_owl_functional_writer.py` & `oaklib-0.5.8/src/oaklib/io/streaming_owl_functional_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/io/streaming_rdf_writer.py` & `oaklib-0.5.8/src/oaklib/io/streaming_rdf_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/io/streaming_writer.py` & `oaklib-0.5.8/src/oaklib/io/streaming_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/io/streaming_yaml_writer.py` & `oaklib-0.5.8/src/oaklib/io/streaming_yaml_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/mappers/base_mapper.py` & `oaklib-0.5.8/src/oaklib/mappers/base_mapper.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/mappers/ontology_metadata_mapper.py` & `oaklib-0.5.8/src/oaklib/mappers/ontology_metadata_mapper.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/parsers/__init__.py` & `oaklib-0.5.8/src/oaklib/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/parsers/association_parser.py` & `oaklib-0.5.8/src/oaklib/parsers/association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/parsers/association_parser_factory.py` & `oaklib-0.5.8/src/oaklib/parsers/association_parser_factory.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/parsers/boomer_parser.py` & `oaklib-0.5.8/src/oaklib/parsers/boomer_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/parsers/gaf_association_parser.py` & `oaklib-0.5.8/src/oaklib/parsers/gaf_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/parsers/gencc_association_parser.py` & `oaklib-0.5.8/src/oaklib/parsers/gencc_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/parsers/hpoa_association_parser.py` & `oaklib-0.5.8/src/oaklib/parsers/hpoa_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/parsers/hpoa_g2p_association_parser.py` & `oaklib-0.5.8/src/oaklib/parsers/hpoa_g2p_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/parsers/kgx_association_parser.py` & `oaklib-0.5.8/src/oaklib/parsers/kgx_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/parsers/mim2gene_association_parser.py` & `oaklib-0.5.8/src/oaklib/parsers/mim2gene_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/parsers/pairwise_association_parser.py` & `oaklib-0.5.8/src/oaklib/parsers/pairwise_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/parsers/parser_base.py` & `oaklib-0.5.8/src/oaklib/parsers/parser_base.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/parsers/phaf_association_parser.py` & `oaklib-0.5.8/src/oaklib/parsers/phaf_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/parsers/xaf_association_parser.py` & `oaklib-0.5.8/src/oaklib/parsers/xaf_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/resource.py` & `oaklib-0.5.8/src/oaklib/resource.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/selector.py` & `oaklib-0.5.8/src/oaklib/selector.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/utilities/apikey_manager.py` & `oaklib-0.5.8/src/oaklib/utilities/apikey_manager.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/utilities/associations/association_differ.py` & `oaklib-0.5.8/src/oaklib/utilities/associations/association_differ.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/utilities/associations/association_index.py` & `oaklib-0.5.8/src/oaklib/utilities/associations/association_index.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/utilities/basic_utils.py` & `oaklib-0.5.8/src/oaklib/utilities/basic_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/utilities/graph/networkx_bridge.py` & `oaklib-0.5.8/src/oaklib/utilities/graph/networkx_bridge.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/utilities/graph/relationship_walker.py` & `oaklib-0.5.8/src/oaklib/utilities/graph/relationship_walker.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/utilities/identifier_utils.py` & `oaklib-0.5.8/src/oaklib/utilities/identifier_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/utilities/iterator_utils.py` & `oaklib-0.5.8/src/oaklib/utilities/iterator_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/utilities/kgcl_utilities.py` & `oaklib-0.5.8/src/oaklib/utilities/kgcl_utilities.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/utilities/label_utilities.py` & `oaklib-0.5.8/src/oaklib/utilities/label_utilities.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/utilities/lexical/lexical_indexer.py` & `oaklib-0.5.8/src/oaklib/utilities/lexical/lexical_indexer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/utilities/mapping/boomer_utils.py` & `oaklib-0.5.8/src/oaklib/utilities/mapping/boomer_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/utilities/mapping/cross_ontology_diffs.py` & `oaklib-0.5.8/src/oaklib/utilities/mapping/cross_ontology_diffs.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/utilities/mapping/mapping_propagator.py` & `oaklib-0.5.8/src/oaklib/utilities/mapping/mapping_propagator.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/utilities/mapping/mapping_validation.py` & `oaklib-0.5.8/src/oaklib/utilities/mapping/mapping_validation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/utilities/mapping/sssom_utils.py` & `oaklib-0.5.8/src/oaklib/utilities/mapping/sssom_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/utilities/ner_utilities.py` & `oaklib-0.5.8/src/oaklib/utilities/ner_utilities.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/utilities/nlp/natual_language_generation.py` & `oaklib-0.5.8/src/oaklib/utilities/nlp/natual_language_generation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/utilities/obograph_utils.py` & `oaklib-0.5.8/src/oaklib/utilities/obograph_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/utilities/ontology_builder.py` & `oaklib-0.5.8/src/oaklib/utilities/ontology_builder.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/utilities/reasoning/relation_graph.py` & `oaklib-0.5.8/src/oaklib/utilities/reasoning/relation_graph.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/utilities/semsim/similarity_utils.py` & `oaklib-0.5.8/src/oaklib/utilities/semsim/similarity_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/utilities/stats/hypergeometric.py` & `oaklib-0.5.8/src/oaklib/utilities/stats/hypergeometric.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/utilities/subsets/slimmer_utils.py` & `oaklib-0.5.8/src/oaklib/utilities/subsets/slimmer_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/utilities/subsets/subset_analysis.py` & `oaklib-0.5.8/src/oaklib/utilities/subsets/subset_analysis.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/utilities/subsets/value_set_expander.py` & `oaklib-0.5.8/src/oaklib/utilities/subsets/value_set_expander.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/utilities/table_filler.py` & `oaklib-0.5.8/src/oaklib/utilities/table_filler.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/utilities/taxon/taxon_constraint_utils.py` & `oaklib-0.5.8/src/oaklib/utilities/taxon/taxon_constraint_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/utilities/validation/definition_ontology_rule.py` & `oaklib-0.5.8/src/oaklib/utilities/validation/definition_ontology_rule.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/utilities/validation/disjointness_rule.py` & `oaklib-0.5.8/src/oaklib/utilities/validation/disjointness_rule.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/utilities/validation/lint_utils.py` & `oaklib-0.5.8/src/oaklib/utilities/validation/lint_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/utilities/validation/ontology_rule.py` & `oaklib-0.5.8/src/oaklib/utilities/validation/ontology_rule.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/src/oaklib/utilities/validation/rule_runner.py` & `oaklib-0.5.8/src/oaklib/utilities/validation/rule_runner.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.7/PKG-INFO` & `oaklib-0.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oaklib
-Version: 0.5.7
+Version: 0.5.8
 Summary: Ontology Access Kit: Python library for common ontology operations over a variety of backends
 Author: cmungall
 Author-email: cjm@berkeleybop.org
 Requires-Python: >=3.9,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

