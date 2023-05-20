# Comparing `tmp/spatialdata-0.0.6.tar.gz` & `tmp/spatialdata-0.0.7.tar.gz`

## Comparing `spatialdata-0.0.6.tar` & `spatialdata-0.0.7.tar`

### file list

```diff
@@ -1,105 +1,107 @@
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 spatialdata-0.0.6/.bumpversion.cfg
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 spatialdata-0.0.6/.editorconfig
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 spatialdata-0.0.6/.gitmodules
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 spatialdata-0.0.6/.mypy.ini
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 spatialdata-0.0.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 spatialdata-0.0.6/.readthedocs.yaml
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 spatialdata-0.0.6/CHANGELOG.md
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 spatialdata-0.0.6/_version.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 spatialdata-0.0.6/.github/codecov.yml
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 spatialdata-0.0.6/.github/workflows/build.yaml
--rw-r--r--   0        0        0     2890 2020-02-02 00:00:00.000000 spatialdata-0.0.6/.github/workflows/test_and_deploy.yaml
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 spatialdata-0.0.6/docs/Makefile
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 spatialdata-0.0.6/docs/api.md
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 spatialdata-0.0.6/docs/changelog.md
--rw-r--r--   0        0        0     4823 2020-02-02 00:00:00.000000 spatialdata-0.0.6/docs/conf.py
--rw-r--r--   0        0        0     7691 2020-02-02 00:00:00.000000 spatialdata-0.0.6/docs/contributing.md
--rw-r--r--   0        0        0    33373 2020-02-02 00:00:00.000000 spatialdata-0.0.6/docs/design_doc.md
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 spatialdata-0.0.6/docs/index.md
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 spatialdata-0.0.6/docs/installation.md
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 spatialdata-0.0.6/docs/references.bib
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 spatialdata-0.0.6/docs/references.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.6/docs/_static/.gitkeep
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 spatialdata-0.0.6/docs/_static/css/custom.css
--rw-r--r--   0        0        0    82458 2020-02-02 00:00:00.000000 spatialdata-0.0.6/docs/_static/img/spatialdata_horizontal.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.6/docs/_templates/.gitkeep
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 spatialdata-0.0.6/docs/_templates/autosummary/base.rst
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 spatialdata-0.0.6/docs/_templates/autosummary/class.rst
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 spatialdata-0.0.6/docs/_templates/autosummary/function.rst
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 spatialdata-0.0.6/docs/extensions/typed_returns.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/__init__.py
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/__main__.py
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/_compat.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/_logging.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/_types.py
--rw-r--r--   0        0        0     6823 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/_utils.py
--rw-r--r--   0        0        0     7375 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/datasets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/_core/__init__.py
--rw-r--r--   0        0        0     5171 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/_core/concatenate.py
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/_core/data_extent.py
--rw-r--r--   0        0        0    62204 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/_core/spatialdata.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/_core/operations/__init__.py
--rw-r--r--   0        0        0     9604 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/_core/operations/aggregate.py
--rw-r--r--   0        0        0    21113 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/_core/operations/rasterize.py
--rw-r--r--   0        0        0    17392 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/_core/operations/transform.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/_core/query/__init__.py
--rw-r--r--   0        0        0    30057 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/_core/query/spatial_query.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/_io/__init__.py
--rw-r--r--   0        0        0    10215 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/_io/_utils.py
--rw-r--r--   0        0        0     7267 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/_io/format.py
--rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/_io/io_points.py
--rw-r--r--   0        0        0     9703 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/_io/io_raster.py
--rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/_io/io_shapes.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/_io/io_table.py
--rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/_io/io_zarr.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/dataloader/__init__.py
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/dataloader/_utils.py
--rw-r--r--   0        0        0     7066 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/dataloader/datasets.py
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/models/__init__.py
--rw-r--r--   0        0        0     8150 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/models/_utils.py
--rw-r--r--   0        0        0    28610 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/models/models.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/transformations/__init__.py
--rw-r--r--   0        0        0     8317 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/transformations/_utils.py
--rw-r--r--   0        0        0    19686 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/transformations/operations.py
--rw-r--r--   0        0        0    35159 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/transformations/transformations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/transformations/ngff/__init__.py
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/transformations/ngff/_utils.py
--rw-r--r--   0        0        0    10276 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/transformations/ngff/ngff_coordinate_system.py
--rw-r--r--   0        0        0    48237 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/transformations/ngff/ngff_transformations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/__init__.py
--rw-r--r--   0        0        0     9295 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/conftest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/core/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/core/operations/__init__.py
--rw-r--r--   0        0        0     4977 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/core/operations/test_aggregations.py
--rw-r--r--   0        0        0     3441 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/core/operations/test_rasterize.py
--rw-r--r--   0        0        0    10928 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/core/operations/test_spatialdata_operations.py
--rw-r--r--   0        0        0    19768 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/core/operations/test_transform.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/core/query/__init__.py
--rw-r--r--   0        0        0    14078 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/core/query/test_spatial_query.py
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/data/multipolygon.json
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/data/points.json
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/data/polygon.json
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/dataloader/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/dataloader/test_datasets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/dataloader/test_transforms.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/datasets/__init__.py
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/datasets/test_datasets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/io/__init__.py
--rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/io/test_format.py
--rw-r--r--   0        0        0    14718 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/io/test_readwrite.py
--rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/io/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/models/__init__.py
--rw-r--r--   0        0        0    14805 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/models/test_models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/transformations/__init__.py
--rw-r--r--   0        0        0    28221 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/transformations/test_transformations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/transformations/ngff/__init__.py
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/transformations/ngff/conftest.py
--rw-r--r--   0        0        0     5755 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/transformations/ngff/test_ngff_coordinate_system.py
--rw-r--r--   0        0        0    15405 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/transformations/ngff/test_ngff_transformations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/utils/__init__.py
--rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/utils/test_element_utils.py
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 spatialdata-0.0.6/.gitignore
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 spatialdata-0.0.6/LICENSE
--rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 spatialdata-0.0.6/README.md
--rw-r--r--   0        0        0     4749 2020-02-02 00:00:00.000000 spatialdata-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     6358 2020-02-02 00:00:00.000000 spatialdata-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 spatialdata-0.0.7/.bumpversion.cfg
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 spatialdata-0.0.7/.editorconfig
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 spatialdata-0.0.7/.gitmodules
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 spatialdata-0.0.7/.mypy.ini
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 spatialdata-0.0.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 spatialdata-0.0.7/.readthedocs.yaml
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 spatialdata-0.0.7/CHANGELOG.md
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 spatialdata-0.0.7/_version.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 spatialdata-0.0.7/.github/codecov.yml
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 spatialdata-0.0.7/.github/workflows/build.yaml
+-rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 spatialdata-0.0.7/.github/workflows/test_and_deploy.yaml
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 spatialdata-0.0.7/docs/Makefile
+-rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 spatialdata-0.0.7/docs/api.md
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 spatialdata-0.0.7/docs/changelog.md
+-rw-r--r--   0        0        0     4823 2020-02-02 00:00:00.000000 spatialdata-0.0.7/docs/conf.py
+-rw-r--r--   0        0        0     7691 2020-02-02 00:00:00.000000 spatialdata-0.0.7/docs/contributing.md
+-rw-r--r--   0        0        0    33373 2020-02-02 00:00:00.000000 spatialdata-0.0.7/docs/design_doc.md
+-rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 spatialdata-0.0.7/docs/index.md
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 spatialdata-0.0.7/docs/installation.md
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 spatialdata-0.0.7/docs/references.bib
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 spatialdata-0.0.7/docs/references.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.7/docs/_static/.gitkeep
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 spatialdata-0.0.7/docs/_static/css/custom.css
+-rw-r--r--   0        0        0    51748 2020-02-02 00:00:00.000000 spatialdata-0.0.7/docs/_static/img/spatialdata_horizontal.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.7/docs/_templates/.gitkeep
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 spatialdata-0.0.7/docs/_templates/autosummary/base.rst
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 spatialdata-0.0.7/docs/_templates/autosummary/class.rst
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 spatialdata-0.0.7/docs/_templates/autosummary/function.rst
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 spatialdata-0.0.7/docs/extensions/typed_returns.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/__init__.py
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/__main__.py
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/_compat.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/_logging.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/_types.py
+-rw-r--r--   0        0        0     6823 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/_utils.py
+-rw-r--r--   0        0        0     9796 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/datasets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/_core/__init__.py
+-rw-r--r--   0        0        0     5171 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/_core/concatenate.py
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/_core/data_extent.py
+-rw-r--r--   0        0        0    62038 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/_core/spatialdata.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/_core/operations/__init__.py
+-rw-r--r--   0        0        0     9386 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/_core/operations/aggregate.py
+-rw-r--r--   0        0        0    21113 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/_core/operations/rasterize.py
+-rw-r--r--   0        0        0    17348 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/_core/operations/transform.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/_core/query/__init__.py
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/_core/query/_utils.py
+-rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/_core/query/relational_query.py
+-rw-r--r--   0        0        0    29788 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/_core/query/spatial_query.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/_io/__init__.py
+-rw-r--r--   0        0        0    10215 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/_io/_utils.py
+-rw-r--r--   0        0        0     7265 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/_io/format.py
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/_io/io_points.py
+-rw-r--r--   0        0        0     9703 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/_io/io_raster.py
+-rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/_io/io_shapes.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/_io/io_table.py
+-rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/_io/io_zarr.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/dataloader/__init__.py
+-rw-r--r--   0        0        0     8606 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/dataloader/datasets.py
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/models/__init__.py
+-rw-r--r--   0        0        0     8150 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/models/_utils.py
+-rw-r--r--   0        0        0    28610 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/models/models.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/transformations/__init__.py
+-rw-r--r--   0        0        0     8317 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/transformations/_utils.py
+-rw-r--r--   0        0        0    19686 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/transformations/operations.py
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/transformations/transformations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/transformations/ngff/__init__.py
+-rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/transformations/ngff/_utils.py
+-rw-r--r--   0        0        0    10276 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/transformations/ngff/ngff_coordinate_system.py
+-rw-r--r--   0        0        0    48233 2020-02-02 00:00:00.000000 spatialdata-0.0.7/src/spatialdata/transformations/ngff/ngff_transformations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/__init__.py
+-rw-r--r--   0        0        0     9669 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/conftest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/core/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/core/operations/__init__.py
+-rw-r--r--   0        0        0     4981 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/core/operations/test_aggregations.py
+-rw-r--r--   0        0        0     3441 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/core/operations/test_rasterize.py
+-rw-r--r--   0        0        0    10928 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/core/operations/test_spatialdata_operations.py
+-rw-r--r--   0        0        0    19768 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/core/operations/test_transform.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/core/query/__init__.py
+-rw-r--r--   0        0        0    21090 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/core/query/test_spatial_query.py
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/data/multipolygon.json
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/data/points.json
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/data/polygon.json
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/dataloader/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/dataloader/test_datasets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/dataloader/test_transforms.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/datasets/__init__.py
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/datasets/test_datasets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/io/__init__.py
+-rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/io/test_format.py
+-rw-r--r--   0        0        0    14718 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/io/test_readwrite.py
+-rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/io/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/models/__init__.py
+-rw-r--r--   0        0        0    14739 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/models/test_models.py
+-rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/test_dataloader/test_datasets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/transformations/__init__.py
+-rw-r--r--   0        0        0    28221 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/transformations/test_transformations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/transformations/ngff/__init__.py
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/transformations/ngff/conftest.py
+-rw-r--r--   0        0        0     5755 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/transformations/ngff/test_ngff_coordinate_system.py
+-rw-r--r--   0        0        0    15405 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/transformations/ngff/test_ngff_transformations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/utils/__init__.py
+-rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 spatialdata-0.0.7/tests/utils/test_element_utils.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 spatialdata-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 spatialdata-0.0.7/LICENSE
+-rw-r--r--   0        0        0     3754 2020-02-02 00:00:00.000000 spatialdata-0.0.7/README.md
+-rw-r--r--   0        0        0     4756 2020-02-02 00:00:00.000000 spatialdata-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     7313 2020-02-02 00:00:00.000000 spatialdata-0.0.7/PKG-INFO
```

### Comparing `spatialdata-0.0.6/.mypy.ini` & `spatialdata-0.0.7/.mypy.ini`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.6/.pre-commit-config.yaml` & `spatialdata-0.0.7/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -9,25 +9,25 @@
     skip: []
 repos:
     - repo: https://github.com/psf/black
       rev: 23.3.0
       hooks:
           - id: black
     - repo: https://github.com/pre-commit/mirrors-prettier
-      rev: v3.0.0-alpha.6
+      rev: v3.0.0-alpha.9-for-vscode
       hooks:
           - id: prettier
     - repo: https://github.com/asottile/blacken-docs
       rev: 1.13.0
       hooks:
           - id: blacken-docs
     - repo: https://github.com/pre-commit/mirrors-mypy
-      rev: v1.2.0
+      rev: v1.3.0
       hooks:
           - id: mypy
             additional_dependencies: [numpy, types-requests]
             exclude: tests/|docs/
     - repo: https://github.com/charliermarsh/ruff-pre-commit
-      rev: v0.0.261
+      rev: v0.0.267
       hooks:
           - id: ruff
             args: [--fix, --exit-non-zero-on-fix]
```

### Comparing `spatialdata-0.0.6/.github/workflows/build.yaml` & `spatialdata-0.0.7/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.6/.github/workflows/test_and_deploy.yaml` & `spatialdata-0.0.7/.github/workflows/test_and_deploy.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -45,15 +45,15 @@
                       pip-${{ runner.os }}-${{ env.pythonLocation }}-
             - name: Install test dependencies
               run: |
                   python -m pip install --upgrade pip wheel
                   pip install pytest-cov
             - name: Install dependencies
               run: |
-                  pip install -e ".[dev,test]"
+                  pip install -e ".[dev,test,torch]"
             - name: Test
               env:
                   MPLBACKEND: agg
                   PLATFORM: ${{ matrix.os }}
                   DISPLAY: :42
               run: |
                   pytest -v --cov --color=yes --cov-report=xml
```

### Comparing `spatialdata-0.0.6/docs/Makefile` & `spatialdata-0.0.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.6/docs/api.md` & `spatialdata-0.0.7/docs/api.md`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,19 @@
 Operations on `SpatialData` objects.
 
 ```{eval-rst}
 .. autosummary::
     :toctree: generated
 
     bounding_box_query
+    polygon_query
     concatenate
     rasterize
     transform
+    aggregate
 ```
 
 ### Utilities
 
 ```{eval-rst}
 .. autosummary::
     :toctree: generated
```

### Comparing `spatialdata-0.0.6/docs/conf.py` & `spatialdata-0.0.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.6/docs/contributing.md` & `spatialdata-0.0.7/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.6/docs/design_doc.md` & `spatialdata-0.0.7/docs/design_doc.md`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.6/docs/references.bib` & `spatialdata-0.0.7/docs/references.bib`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.6/docs/_static/css/custom.css` & `spatialdata-0.0.7/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.6/docs/_templates/autosummary/class.rst` & `spatialdata-0.0.7/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.6/docs/extensions/typed_returns.py` & `spatialdata-0.0.7/docs/extensions/typed_returns.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.6/src/spatialdata/__init__.py` & `spatialdata-0.0.7/src/spatialdata/__init__.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.6/src/spatialdata/__main__.py` & `spatialdata-0.0.7/src/spatialdata/__main__.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.6/src/spatialdata/_compat.py` & `spatialdata-0.0.7/src/spatialdata/_compat.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.6/src/spatialdata/_logging.py` & `spatialdata-0.0.7/src/spatialdata/_logging.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.6/src/spatialdata/_utils.py` & `spatialdata-0.0.7/src/spatialdata/_utils.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.6/src/spatialdata/_core/concatenate.py` & `spatialdata-0.0.7/src/spatialdata/_core/concatenate.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.6/src/spatialdata/_core/data_extent.py` & `spatialdata-0.0.7/src/spatialdata/_core/data_extent.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.6/src/spatialdata/_core/spatialdata.py` & `spatialdata-0.0.7/src/spatialdata/_core/spatialdata.py`

 * *Files 2% similar despite different names*

```diff
@@ -583,14 +583,15 @@
             If True (default), the table will be filtered to only contain regions
             of an element belonging to the specified coordinate system(s).
 
         Returns
         -------
         The filtered SpatialData.
         """
+        from spatialdata._core.query.relational_query import _filter_table_by_coordinate_system
         from spatialdata.transformations.operations import get_transformation
 
         elements: dict[str, dict[str, SpatialElement]] = {}
         element_paths_in_coordinate_system = []
         if isinstance(coordinate_system, str):
             coordinate_system = [coordinate_system]
         for element_type, element_name, element in self._gen_elements():
@@ -600,18 +601,15 @@
                 if cs in transformations:
                     if element_type not in elements:
                         elements[element_type] = {}
                     elements[element_type][element_name] = element
                     element_paths_in_coordinate_system.append(element_name)
 
         if filter_table:
-            table_mapping_metadata = self.table.uns[TableModel.ATTRS_KEY]
-            region_key = table_mapping_metadata[TableModel.REGION_KEY_KEY]
-            table = self.table[self.table.obs[region_key].isin(element_paths_in_coordinate_system)].copy()
-            table.uns[TableModel.ATTRS_KEY][TableModel.REGION_KEY] = table.obs[region_key].unique().tolist()
+            table = _filter_table_by_coordinate_system(self.table, element_paths_in_coordinate_system)
         else:
             table = self.table
 
         return SpatialData(**elements, table=table)
 
     def transform_element_to_coordinate_system(
         self, element: SpatialElement, target_coordinate_system: str
```

### Comparing `spatialdata-0.0.6/src/spatialdata/_core/operations/aggregate.py` & `spatialdata-0.0.7/src/spatialdata/_core/operations/aggregate.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import pandas as pd
 from multiscale_spatial_image import MultiscaleSpatialImage
 from scipy import sparse
 from spatial_image import SpatialImage
 from xrspatial import zonal_stats
 
 from spatialdata._core.operations.transform import transform
+from spatialdata._core.query._utils import circles_to_polygons
 from spatialdata._types import ArrayLike
 from spatialdata.models import (
     Image2DModel,
     Labels2DModel,
     PointsModel,
     ShapesModel,
     get_model,
@@ -66,14 +67,17 @@
 
     Returns
     -------
     AnnData of shape (by.shape[0], values[id_key].nunique())])
 
     Notes
     -----
+    This function returns an AnnData object. Use :func:`spatialdata.SpatialData.aggregate` to return a `SpatialData`
+    object instead (with the table already referring to the regions passed in `by`).
+
     When aggregation points by shapes, the current implementation loads all the points into
     memory and thus could lead to a large memory usage. This Github issue
     https://github.com/scverse/spatialdata/issues/210 keeps track of the changes required to
     address this behavior.
     """
     # get schema
     by_type = get_model(by)
@@ -130,23 +134,14 @@
     values: gpd.GeoDataFrame,
     by: gpd.GeoDataFrame,
     id_key: str | None,
     *,
     value_key: str | None = None,
     agg_func: str | list[str] = "count",
 ) -> ad.AnnData:
-    def circles_to_polygons(df: gpd.GeoDataFrame) -> gpd.GeoDataFrame:
-        # We should only be buffering points, not polygons. Unfortunately this is an expensive check.
-        values_geotypes = list(values.geom_type.unique())
-        if values_geotypes == ["Point"]:
-            df = df.set_geometry(df.geometry.buffer(df[ShapesModel.RADIUS_KEY]))
-        elif "Point" in values_geotypes:
-            raise TypeError("Geometry contained shapes and polygons.")
-        return df
-
     if id_key is None:
         raise ValueError("Must pass id_key for shapes.")
 
     values = circles_to_polygons(values)
     by = circles_to_polygons(by)
 
     return _aggregate_shapes(values, by, id_key, value_key, agg_func)
```

### Comparing `spatialdata-0.0.6/src/spatialdata/_core/operations/rasterize.py` & `spatialdata-0.0.7/src/spatialdata/_core/operations/rasterize.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.6/src/spatialdata/_core/operations/transform.py` & `spatialdata-0.0.7/src/spatialdata/_core/operations/transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,14 @@
     new_v = (matrix @ v.T).T
     c_shape: tuple[int, ...]
     c_shape = (data.shape[0],) if "c" in axes else ()
     new_spatial_shape = tuple(
         int(np.max(new_v[:, i]) - np.min(new_v[:, i])) for i in range(len(c_shape), n_spatial_dims + len(c_shape))
     )
     output_shape = c_shape + new_spatial_shape
-    ##
     translation_vector = np.min(new_v[:, :-1], axis=0)
     translation = Translation(translation_vector, axes=axes)
     inverse_matrix_adjusted = Sequence(
         [
             translation,
             transformation.inverse(),
         ]
@@ -71,19 +70,17 @@
         data,
         matrix=inverse_matrix_adjusted,
         output_shape=output_shape,
         **kwargs,
         # , output_chunks=output_chunks
     )
     assert isinstance(transformed_dask, DaskArray)
-    ##
 
     if DEBUG_WITH_PLOTS:
         if n_spatial_dims == 2:
-            ##
             import matplotlib.pyplot as plt
 
             plt.figure()
             im = data
             new_v_inverse = (inverse_matrix @ v.T).T
             # min_x_inverse = np.min(new_v_inverse[:, 2])
             # min_y_inverse = np.min(new_v_inverse[:, 1])
@@ -97,15 +94,14 @@
             start_index = 1 if "c" in axes else 0
             plt.scatter(v[:, start_index:-1][:, 1] - 0.5, v[:, start_index:-1][:, 0] - 0.5, c="r")
             plt.scatter(new_v[:, start_index:-1][:, 1] - 0.5, new_v[:, start_index:-1][:, 0] - 0.5, c="g")
             plt.scatter(
                 new_v_inverse[:, start_index:-1][:, 1] - 0.5, new_v_inverse[:, start_index:-1][:, 0] - 0.5, c="k"
             )
             plt.show()
-            ##
         else:
             assert n_spatial_dims == 3
             # raise NotImplementedError()
     return transformed_dask, translation
 
 
 def _prepend_transformation(
```

### Comparing `spatialdata-0.0.6/src/spatialdata/_core/query/spatial_query.py` & `spatialdata-0.0.7/src/spatialdata/_core/query/spatial_query.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,21 +18,16 @@
 from xarray import DataArray
 
 from spatialdata._core.spatialdata import SpatialData
 from spatialdata._logging import logger
 from spatialdata._types import ArrayLike
 from spatialdata._utils import Number, _parse_list_into_array
 from spatialdata.models import (
-    Labels2DModel,
-    Labels3DModel,
-    ShapesModel,
     SpatialElement,
-    TableModel,
     get_axes_names,
-    get_model,
 )
 from spatialdata.models._utils import ValidAxis_t, get_spatial_axes
 from spatialdata.transformations._utils import compute_coordinates
 from spatialdata.transformations.transformations import (
     Affine,
     BaseTransformation,
     Sequence,
@@ -301,14 +296,15 @@
     axes: tuple[str, ...],
     min_coordinate: Union[list[Number], ArrayLike],
     max_coordinate: Union[list[Number], ArrayLike],
     target_coordinate_system: str,
     filter_table: bool = True,
 ) -> SpatialData:
     from spatialdata import SpatialData
+    from spatialdata._core.query.relational_query import _filter_table_by_elements
 
     min_coordinate = _parse_list_into_array(min_coordinate)
     max_coordinate = _parse_list_into_array(max_coordinate)
     new_elements = {}
     for element_type in ["points", "images", "labels", "shapes"]:
         elements = getattr(sdata, element_type)
         queried_elements = _dict_query_dispatcher(
@@ -317,40 +313,15 @@
             axes=axes,
             min_coordinate=min_coordinate,
             max_coordinate=max_coordinate,
             target_coordinate_system=target_coordinate_system,
         )
         new_elements[element_type] = queried_elements
 
-    if filter_table and sdata.table is not None:
-        to_keep = np.array([False] * len(sdata.table))
-        region_key = sdata.table.uns[TableModel.ATTRS_KEY][TableModel.REGION_KEY_KEY]
-        instance_key = sdata.table.uns[TableModel.ATTRS_KEY][TableModel.INSTANCE_KEY]
-        for _, elements in new_elements.items():
-            for name, element in elements.items():
-                if get_model(element) == Labels2DModel or get_model(element) == Labels3DModel:
-                    if isinstance(element, SpatialImage):
-                        # get unique labels value (including 0 if present)
-                        instances = da.unique(element.data).compute()
-                    else:
-                        assert isinstance(element, MultiscaleSpatialImage)
-                        v = element["scale0"].values()
-                        assert len(v) == 1
-                        xdata = next(iter(v))
-                        instances = da.unique(xdata.data).compute()
-                elif get_model(element) == ShapesModel:
-                    instances = element.index.to_numpy()
-                else:
-                    continue
-                indices = (sdata.table.obs[region_key] == name) & (sdata.table.obs[instance_key].isin(instances))
-                to_keep = to_keep | indices
-        table = sdata.table[to_keep, :].copy()
-        table.uns[TableModel.ATTRS_KEY][TableModel.REGION_KEY] = table.obs[region_key].unique().tolist()
-    else:
-        table = sdata.table
+    table = _filter_table_by_elements(sdata.table, new_elements) if filter_table else sdata.table
     return SpatialData(**new_elements, table=table)
 
 
 @bounding_box_query.register(SpatialImage)
 @bounding_box_query.register(MultiscaleSpatialImage)
 def _(
     image: Union[SpatialImage, MultiscaleSpatialImage],
@@ -636,61 +607,79 @@
     queried = polygons[polygons.geometry.within(bounding_box_non_axes_aligned)]
     if len(queried) == 0:
         return None
     return queried
 
 
 def _polygon_query(
-    sdata: SpatialData, polygon: Polygon, target_coordinate_system: str, shapes: bool, points: bool
+    sdata: SpatialData, polygon: Polygon, target_coordinate_system: str, filter_table: bool, shapes: bool, points: bool
 ) -> SpatialData:
-    from spatialdata.models import PointsModel, points_dask_dataframe_to_geopandas, points_geopandas_to_dask_dataframe
+    from spatialdata._core.query._utils import circles_to_polygons
+    from spatialdata._core.query.relational_query import _filter_table_by_elements
+    from spatialdata.models import (
+        PointsModel,
+        ShapesModel,
+        points_dask_dataframe_to_geopandas,
+        points_geopandas_to_dask_dataframe,
+    )
     from spatialdata.transformations import get_transformation, set_transformation
 
     new_shapes = {}
     if shapes:
         for shapes_name, s in sdata.shapes.items():
-            if "__old_index" in s.columns:
-                assert np.all(s["__old_index"] == s.index)
+            buffered = circles_to_polygons(s) if ShapesModel.RADIUS_KEY in s.columns else s
+
+            if "__old_index" in buffered.columns:
+                assert np.all(s["__old_index"] == buffered.index)
             else:
-                s["__old_index"] = s.index
-            indices = s.geometry.apply(lambda x: x.intersects(polygon))
+                buffered["__old_index"] = buffered.index
+            indices = buffered.geometry.apply(lambda x: x.intersects(polygon))
             if np.sum(indices) == 0:
                 raise ValueError("we expect at least one shape")
             queried_shapes = s[indices]
-            queried_shapes.index = queried_shapes["__old_index"]
+            queried_shapes.index = buffered[indices]["__old_index"]
             queried_shapes.index.name = None
-            del s["__old_index"]
-            del queried_shapes["__old_index"]
-            transformation = get_transformation(s, target_coordinate_system)
+            del buffered["__old_index"]
+            if "__old_index" in queried_shapes.columns:
+                del queried_shapes["__old_index"]
+            transformation = get_transformation(buffered, target_coordinate_system)
             queried_shapes = ShapesModel.parse(queried_shapes)
             set_transformation(queried_shapes, transformation, target_coordinate_system)
             new_shapes[shapes_name] = queried_shapes
 
     new_points = {}
     if points:
         for points_name, p in sdata.points.items():
             points_gdf = points_dask_dataframe_to_geopandas(p)
             indices = points_gdf.geometry.intersects(polygon)
             if np.sum(indices) == 0:
                 raise ValueError("we expect at least one point")
             queried_points = points_gdf[indices]
             ddf = points_geopandas_to_dask_dataframe(queried_points)
             transformation = get_transformation(p, target_coordinate_system)
-            ddf = PointsModel.parse(ddf, coordinates={"x": "x", "y": "y", "z": "z"})
+            if "z" in ddf.columns:
+                ddf = PointsModel.parse(ddf, coordinates={"x": "x", "y": "y", "z": "z"})
+            else:
+                ddf = PointsModel.parse(ddf, coordinates={"x": "x", "y": "y"})
             set_transformation(ddf, transformation, target_coordinate_system)
             new_points[points_name] = ddf
 
-    return SpatialData(shapes=new_shapes, points=new_points, table=sdata.table)
+    if filter_table:
+        table = _filter_table_by_elements(sdata.table, {"shapes": new_shapes, "points": new_points})
+    else:
+        table = sdata.table
+    return SpatialData(shapes=new_shapes, points=new_points, table=table)
 
 
 # this function is currently excluded from the API documentation. TODO: add it after the refactoring
 def polygon_query(
     sdata: SpatialData,
     polygons: Union[Polygon, list[Polygon]],
     target_coordinate_system: str,
+    filter_table: bool = True,
     shapes: bool = True,
     points: bool = True,
 ) -> SpatialData:
     """
     Query a spatial data object by a polygon, filtering shapes and points.
 
     Parameters
@@ -712,52 +701,62 @@
     Notes
     -----
     This function will be refactored to be more general.
     The table is not filtered by this function, but is passed as is, this will also changed during the refactoring
     making this function more general and ergonomic.
 
     """
+    from spatialdata._core.query.relational_query import _filter_table_by_elements
+
     if isinstance(polygons, Polygon):
         polygons = [polygons]
 
     if len(polygons) == 1:
         return _polygon_query(
             sdata=sdata,
             polygon=polygons[0],
             target_coordinate_system=target_coordinate_system,
+            filter_table=filter_table,
             shapes=shapes,
             points=points,
         )
     # TODO: the performance for this case can be greatly improved by using the geopandas queries only once, and not
     #  in a loop as done preliminarily here
     if points:
         raise NotImplementedError(
             "points=True is not implemented when querying by multiple polygons. If you encounter this error, please"
             " open an issue on GitHub and we will prioritize the implementation."
         )
     sdatas = []
     for polygon in tqdm(polygons):
         try:
+            # not filtering now, we filter below
             queried_sdata = _polygon_query(
                 sdata=sdata,
                 polygon=polygon,
                 target_coordinate_system=target_coordinate_system,
+                filter_table=False,
                 shapes=shapes,
                 points=points,
             )
             sdatas.append(queried_sdata)
         except ValueError as e:
             if str(e) != "we expect at least one shape":
                 raise e
             # print("skipping", end="")
-    geodataframe_pieces: dict[str, GeoDataFrame] = {}
+    geodataframe_pieces: dict[str, list[GeoDataFrame]] = {}
 
     for sdata in sdatas:
         for shapes_name, shapes in sdata.shapes.items():
             if shapes_name not in geodataframe_pieces:
                 geodataframe_pieces[shapes_name] = []
             geodataframe_pieces[shapes_name].append(shapes)
 
     geodataframes = {}
     for k, v in geodataframe_pieces.items():
-        geodataframes[k] = pd.concat(v)
-    return SpatialData(shapes=geodataframes, table=sdatas[0].table)
+        vv = pd.concat(v)
+        vv = vv[~vv.index.duplicated(keep="first")]
+        geodataframes[k] = vv
+
+    table = _filter_table_by_elements(sdata.table, {"shapes": geodataframes}) if filter_table else sdata.table
+
+    return SpatialData(shapes=geodataframes, table=table)
```

### Comparing `spatialdata-0.0.6/src/spatialdata/_io/_utils.py` & `spatialdata-0.0.7/src/spatialdata/_io/_utils.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.6/src/spatialdata/_io/format.py` & `spatialdata-0.0.7/src/spatialdata/_io/format.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
             raise ValueError("coordinate_transformations must be provided")
         ct_count = len(coordinate_transformations)
         if ct_count != nlevels:
             raise ValueError(f"coordinate_transformations count: {ct_count} must match datasets {nlevels}")
         for transformations in coordinate_transformations:
             assert isinstance(transformations, list)
             types = [t.get("type", None) for t in transformations]
-            if any([t is None for t in types]):
+            if any(t is None for t in types):
                 raise ValueError("Missing type in: %s" % transformations)
 
             # new validation
             import json
 
             json0 = [json.dumps(t) for t in transformations]
             from spatialdata.transformations.ngff.ngff_transformations import (
```

### Comparing `spatialdata-0.0.6/src/spatialdata/_io/io_points.py` & `spatialdata-0.0.7/src/spatialdata/_io/io_points.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.6/src/spatialdata/_io/io_raster.py` & `spatialdata-0.0.7/src/spatialdata/_io/io_raster.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.6/src/spatialdata/_io/io_shapes.py` & `spatialdata-0.0.7/src/spatialdata/_io/io_shapes.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.6/src/spatialdata/_io/io_table.py` & `spatialdata-0.0.7/src/spatialdata/_io/io_table.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.6/src/spatialdata/_io/io_zarr.py` & `spatialdata-0.0.7/src/spatialdata/_io/io_zarr.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.6/src/spatialdata/dataloader/datasets.py` & `spatialdata-0.0.7/src/spatialdata/dataloader/datasets.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Callable, Optional
 
 import numpy as np
 from geopandas import GeoDataFrame
 from multiscale_spatial_image import MultiscaleSpatialImage
+from shapely import MultiPolygon, Point, Polygon
 from spatial_image import SpatialImage
 from torch.utils.data import Dataset
 
 from spatialdata._core.operations.rasterize import rasterize
 from spatialdata._utils import _affine_matrix_multiplication
 from spatialdata.models import (
     Image2DModel,
@@ -31,15 +32,15 @@
         self,
         sdata: SpatialData,
         regions_to_images: dict[str, str],
         tile_dim_in_units: float,
         tile_dim_in_pixels: int,
         target_coordinate_system: str = "global",
         # unused at the moment, see
-        transform: Optional[Callable[[Any], Any]] = None,
+        transform: Optional[Callable[[SpatialData], Any]] = None,
     ):
         """
         Torch Dataset that returns image tiles around regions from a SpatialData object.
 
         Parameters
         ----------
         sdata
@@ -100,27 +101,38 @@
                 return region_key, index - i
             i += n_spots
         raise ValueError(f"index {index} is out of range")
 
     def __len__(self) -> int:
         return self.n_spots
 
-    def __getitem__(self, idx: int) -> tuple[SpatialImage, str, int]:
+    def __getitem__(self, idx: int) -> Any | SpatialData:
+        from spatialdata import SpatialData
+
         if idx >= self.n_spots:
             raise IndexError()
         regions_name, region_index = self._get_region_info_for_index(idx)
         regions = self.sdata[regions_name]
         # TODO: here we just need to compute the centroids,
         #  we probably want to move this functionality to a different file
         if isinstance(regions, GeoDataFrame):
             dims = get_axes_names(regions)
             region = regions.iloc[region_index]
-            # the function coords.xy is just accessing _coords, and wrapping it with extra information, so we access
-            # it directly
-            centroid = np.atleast_2d(region.geometry.coords._coords[0])
+            shape = regions.geometry.iloc[0]
+            if isinstance(shape, Polygon):
+                xy = region.geometry.centroid.coords.xy
+                centroid = np.array([[xy[0][0], xy[1][0]]])
+            elif isinstance(shape, MultiPolygon):
+                raise NotImplementedError("MultiPolygon not supported yet")
+            elif isinstance(shape, Point):
+                xy = region.geometry.coords.xy
+                centroid = np.array([[xy[0][0], xy[1][0]]])
+            else:
+                raise RuntimeError(f"Unsupported type: {type(shape)}")
+
             t = get_transformation(regions, self.target_coordinate_system)
             assert isinstance(t, BaseTransformation)
             aff = t.to_affine_matrix(input_axes=dims, output_axes=dims)
             transformed_centroid = np.squeeze(_affine_matrix_multiplication(aff, centroid), 0)
         elif isinstance(regions, (SpatialImage, MultiscaleSpatialImage)):
             raise NotImplementedError("labels not supported yet")
         else:
@@ -133,23 +145,44 @@
             raster,
             axes=dims,
             min_coordinate=min_coordinate,
             max_coordinate=max_coordinate,
             target_coordinate_system=self.target_coordinate_system,
             target_width=self.tile_dim_in_pixels,
         )
-        if self.transform is not None:
-            tile = self.transform(tile)
-
         # TODO: as explained in the TODO in the __init__(), we want to let the
         #  user also use the bounding box query instaed of the rasterization
         #  the return function of this function would change, so we need to
         #  decide if instead having an extra Tile dataset class
         # from spatialdata._core._spatial_query import BoundingBoxRequest
         # request = BoundingBoxRequest(
         #     target_coordinate_system=self.target_coordinate_system,
         #     axes=dims,
         #     min_coordinate=min_coordinate,
         #     max_coordinate=max_coordinate,
         # )
         # sdata_item = self.sdata.query.bounding_box(**request.to_dict())
-        return tile, regions_name, region_index
+        table = self.sdata.table
+        filter_table = False
+        if table is not None:
+            region = table.uns["spatialdata_attrs"]["region"]
+            region_key = table.uns["spatialdata_attrs"]["region_key"]
+            instance_key = table.uns["spatialdata_attrs"]["instance_key"]
+            if isinstance(region, str):
+                if regions_name == region:
+                    filter_table = True
+            elif isinstance(region, list):
+                if regions_name in region:
+                    filter_table = True
+            else:
+                raise ValueError("region must be a string or a list of strings")
+        # TODO: maybe slow, we should check if there is a better way to do this
+        if filter_table:
+            instance = self.sdata[regions_name].iloc[region_index].name
+            row = table[(table.obs[region_key] == regions_name) & (table.obs[instance_key] == instance)].copy()
+            tile_table = row
+        else:
+            tile_table = None
+        tile_sdata = SpatialData(images={self.regions_to_images[regions_name]: tile}, table=tile_table)
+        if self.transform is not None:
+            return self.transform(tile_sdata)
+        return tile_sdata
```

### Comparing `spatialdata-0.0.6/src/spatialdata/models/__init__.py` & `spatialdata-0.0.7/src/spatialdata/models/__init__.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.6/src/spatialdata/models/_utils.py` & `spatialdata-0.0.7/src/spatialdata/models/_utils.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.6/src/spatialdata/models/models.py` & `spatialdata-0.0.7/src/spatialdata/models/models.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.6/src/spatialdata/transformations/__init__.py` & `spatialdata-0.0.7/src/spatialdata/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.6/src/spatialdata/transformations/_utils.py` & `spatialdata-0.0.7/src/spatialdata/transformations/_utils.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.6/src/spatialdata/transformations/operations.py` & `spatialdata-0.0.7/src/spatialdata/transformations/operations.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.6/src/spatialdata/transformations/transformations.py` & `spatialdata-0.0.7/src/spatialdata/transformations/transformations.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,15 +191,15 @@
         pass
 
 
 class Identity(BaseTransformation):
     def to_affine_matrix(self, input_axes: tuple[ValidAxis_t, ...], output_axes: tuple[ValidAxis_t, ...]) -> ArrayLike:
         self.validate_axes(input_axes)
         self.validate_axes(output_axes)
-        if not all([ax in output_axes for ax in input_axes]):
+        if not all(ax in output_axes for ax in input_axes):
             raise ValueError("Input axes must be a subset of output axes.")
         m = self._empty_affine_matrix(input_axes, output_axes)
         for i_out, ax_out in enumerate(output_axes):
             for i_in, ax_in in enumerate(input_axes):
                 if ax_in == ax_out:
                     m[i_out, i_in] = 1
         return m
@@ -346,15 +346,15 @@
 
     def inverse(self) -> BaseTransformation:
         return Translation(-self.translation, self.axes)
 
     def to_affine_matrix(self, input_axes: tuple[ValidAxis_t, ...], output_axes: tuple[ValidAxis_t, ...]) -> ArrayLike:
         self.validate_axes(input_axes)
         self.validate_axes(output_axes)
-        if not all([ax in output_axes for ax in input_axes]):
+        if not all(ax in output_axes for ax in input_axes):
             raise ValueError("Input axes must be a subset of output axes.")
         m = self._empty_affine_matrix(input_axes, output_axes)
         for i_out, ax_out in enumerate(output_axes):
             for i_in, ax_in in enumerate(input_axes):
                 if ax_in == ax_out:
                     m[i_out, i_in] = 1
                     if ax_out in self.axes:
@@ -433,15 +433,15 @@
 
     def inverse(self) -> BaseTransformation:
         return Scale(1 / self.scale, self.axes)
 
     def to_affine_matrix(self, input_axes: tuple[ValidAxis_t, ...], output_axes: tuple[ValidAxis_t, ...]) -> ArrayLike:
         self.validate_axes(input_axes)
         self.validate_axes(output_axes)
-        if not all([ax in output_axes for ax in input_axes]):
+        if not all(ax in output_axes for ax in input_axes):
             raise ValueError("Input axes must be a subset of output axes.")
         m = self._empty_affine_matrix(input_axes, output_axes)
         for i_out, ax_out in enumerate(output_axes):
             for i_in, ax_in in enumerate(input_axes):
                 if ax_in == ax_out:
                     scale_factor = self.scale[self.axes.index(ax_out)] if ax_out in self.axes else 1
                     m[i_out, i_in] = scale_factor
@@ -629,15 +629,15 @@
     # return two values for the recursive logic to work
     def _to_affine_matrix_wrapper(
         self, input_axes: tuple[ValidAxis_t, ...], output_axes: tuple[ValidAxis_t, ...], _nested_sequence: bool = False
     ) -> tuple[ArrayLike, tuple[ValidAxis_t, ...]]:
         DEBUG_SEQUENCE = False
         self.validate_axes(input_axes)
         self.validate_axes(output_axes)
-        if not all([ax in output_axes for ax in input_axes]):
+        if not all(ax in output_axes for ax in input_axes):
             raise ValueError("Input axes must be a subset of output axes.")
 
         current_input_axes = input_axes
         current_output_axes = _get_current_output_axes(self.transformations[0], current_input_axes)
         m = self.transformations[0].to_affine_matrix(current_input_axes, current_output_axes)
         if DEBUG_SEQUENCE:
             print(f"# 0: current_input_axes = {current_input_axes}, current_output_axes = {current_output_axes}")
@@ -762,15 +762,15 @@
         to_return = []
         for ax in input_axes:
             if ax not in map_axis_input_axes:
                 assert ax not in to_return
                 to_return.append(ax)
             else:
                 mapped = [ax_out for ax_out, ax_in in transformation.map_axis.items() if ax_in == ax]
-                assert all([ax_out not in to_return for ax_out in mapped])
+                assert all(ax_out not in to_return for ax_out in mapped)
                 to_return.extend(mapped)
         return tuple(to_return)
     elif isinstance(transformation, Affine):
         to_return = []
         add_affine_output_axes = False
         for ax in input_axes:
             if ax not in transformation.input_axes:
```

### Comparing `spatialdata-0.0.6/src/spatialdata/transformations/ngff/_utils.py` & `spatialdata-0.0.7/src/spatialdata/transformations/ngff/_utils.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.6/src/spatialdata/transformations/ngff/ngff_coordinate_system.py` & `spatialdata-0.0.7/src/spatialdata/transformations/ngff/ngff_coordinate_system.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.6/src/spatialdata/transformations/ngff/ngff_transformations.py` & `spatialdata-0.0.7/src/spatialdata/transformations/ngff/ngff_transformations.py`

 * *Files 0% similar despite different names*

```diff
@@ -651,16 +651,16 @@
         input_axes
             the input axes.
         output_axes
             the output axes.
         """
         from spatialdata.models import C, X, Y, Z
 
-        assert all([ax in (X, Y, Z, C) for ax in input_axes])
-        assert all([ax in (X, Y, Z, C) for ax in output_axes])
+        assert all(ax in (X, Y, Z, C) for ax in input_axes)
+        assert all(ax in (X, Y, Z, C) for ax in output_axes)
         m = np.zeros((len(output_axes) + 1, len(input_axes) + 1))
         for output_ax in output_axes:
             for input_ax in input_axes:
                 if output_ax == input_ax:
                     m[output_axes.index(output_ax), input_axes.index(input_ax)] = 1
         m[-1, -1] = 1
         return m
```

### Comparing `spatialdata-0.0.6/tests/conftest.py` & `spatialdata-0.0.7/tests/conftest.py`

 * *Files 13% similar despite different names*

```diff
@@ -285,8 +285,17 @@
 
 @pytest.fixture()
 def sdata_blobs() -> SpatialData:
     """Create a 2D labels."""
     from copy import deepcopy
     from spatialdata.datasets import blobs
 
-    return deepcopy(blobs(256, 300, 3))
+    sdata = deepcopy(blobs(256, 300, 3))
+    from spatialdata._utils import multiscale_spatial_image_from_data_tree
+
+    sdata.images["blobs_multiscale_image"] = multiscale_spatial_image_from_data_tree(
+        sdata.images["blobs_multiscale_image"]
+    )
+    sdata.labels["blobs_multiscale_labels"] = multiscale_spatial_image_from_data_tree(
+        sdata.labels["blobs_multiscale_labels"]
+    )
+    return sdata
```

### Comparing `spatialdata-0.0.6/tests/core/operations/test_aggregations.py` & `spatialdata-0.0.7/tests/core/operations/test_aggregations.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,12 +117,12 @@
     assert len(out) + 1 == len(np.unique(labels_blobs))
 
     out = aggregate(image, labels, zone_ids=[1, 2, 3])
     assert len(out) == 3
 
 
 def test_aggregate_spatialdata(sdata_blobs: SpatialData) -> None:
-    sdata = sdata_blobs.aggregate(sdata_blobs.points["blobs_points"], by="blobs_shapes")
+    sdata = sdata_blobs.aggregate(sdata_blobs.points["blobs_points"], by="blobs_polygons")
     assert isinstance(sdata, SpatialData)
-    assert len(sdata.shapes["blobs_shapes"]) == 2
+    assert len(sdata.shapes["blobs_polygons"]) == 2
     assert sdata.table.shape == (2, 2)
     assert len(sdata.points["points"].compute()) == 300
```

### Comparing `spatialdata-0.0.6/tests/core/operations/test_rasterize.py` & `spatialdata-0.0.7/tests/core/operations/test_rasterize.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.6/tests/core/operations/test_spatialdata_operations.py` & `spatialdata-0.0.7/tests/core/operations/test_spatialdata_operations.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.6/tests/core/operations/test_transform.py` & `spatialdata-0.0.7/tests/core/operations/test_transform.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.6/tests/data/multipolygon.json` & `spatialdata-0.0.7/tests/data/multipolygon.json`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.6/tests/data/polygon.json` & `spatialdata-0.0.7/tests/data/polygon.json`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.6/tests/io/test_format.py` & `spatialdata-0.0.7/tests/io/test_format.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.6/tests/io/test_readwrite.py` & `spatialdata-0.0.7/tests/io/test_readwrite.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.6/tests/io/test_utils.py` & `spatialdata-0.0.7/tests/io/test_utils.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.6/tests/models/test_models.py` & `spatialdata-0.0.7/tests/models/test_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     def _parse_transformation_from_multiple_places(self, model: Any, element: Any, **kwargs) -> None:
         # This function seems convoluted but the idea is simple: sometimes the parser creates a whole new object,
         # other times (SpatialImage, DataArray, AnnData, GeoDataFrame) the object is enriched in-place. In such
         # cases we check that if there was already a transformation in the object we consider it then we are not
         # passing it also explicitly in the parser.
         # This function does that for all the models (it's called by the various tests of the models) and it first
         # creates clean copies of the element, and then puts the transformation inside it with various methods
-        if any([isinstance(element, t) for t in (SpatialImage, DataArray, AnnData, GeoDataFrame, DaskDataFrame)]):
+        if any(isinstance(element, t) for t in (SpatialImage, DataArray, AnnData, GeoDataFrame, DaskDataFrame)):
             element_erased = deepcopy(element)
             # we are not respecting the function signature (the transform should be not None); it's fine for testing
             if isinstance(element_erased, DataArray) and not isinstance(element_erased, SpatialImage):
                 # this case is for xarray.DataArray where the user manually updates the transform in attrs,
                 # or when a user takes an image from a MultiscaleSpatialImage
                 _set_transformations_xarray(element_erased, {})
             else:
@@ -104,25 +104,23 @@
                 element_copy3 = deepcopy(element_erased)
                 if isinstance(element_copy3, DataArray) and not isinstance(element_copy3, SpatialImage):
                     _set_transformations_xarray(element_copy3, {"global": t})
                 else:
                     set_transformation(element_copy3, t, "global")
                 model.parse(element_copy3, transformations={"global": t}, **kwargs)
         elif any(
-            [
-                isinstance(element, t)
-                for t in (
-                    MultiscaleSpatialImage,
-                    str,
-                    np.ndarray,
-                    dask.array.core.Array,
-                    pathlib.PosixPath,
-                    pd.DataFrame,
-                )
-            ]
+            isinstance(element, t)
+            for t in (
+                MultiscaleSpatialImage,
+                str,
+                np.ndarray,
+                dask.array.core.Array,
+                pathlib.PosixPath,
+                pd.DataFrame,
+            )
         ):
             # no need to apply this function since the parser always creates a new object and the transformation is not
             # part of the object passed as input
             pass
         else:
             raise ValueError(f"Unknown type {type(element)}")
```

### Comparing `spatialdata-0.0.6/tests/transformations/test_transformations.py` & `spatialdata-0.0.7/tests/transformations/test_transformations.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.6/tests/transformations/ngff/conftest.py` & `spatialdata-0.0.7/tests/transformations/ngff/conftest.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.6/tests/transformations/ngff/test_ngff_coordinate_system.py` & `spatialdata-0.0.7/tests/transformations/ngff/test_ngff_coordinate_system.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.6/tests/transformations/ngff/test_ngff_transformations.py` & `spatialdata-0.0.7/tests/transformations/ngff/test_ngff_transformations.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.6/tests/utils/test_element_utils.py` & `spatialdata-0.0.7/tests/utils/test_element_utils.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.6/LICENSE` & `spatialdata-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.6/pyproject.toml` & `spatialdata-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     "pytest",
     "pytest-cov",
 ]
 torch = [
     "torch"
 ]
 extra  = [
-    "napari-spatialdata",
+    "napari-spatialdata>=0.2.3",
     "spatialdata-plot",
     "spatialdata-io",
 ]
 
 [tool.coverage.run]
 source = ["spatialdata"]
 omit = [
```

### Comparing `spatialdata-0.0.6/PKG-INFO` & `spatialdata-0.0.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spatialdata
-Version: 0.0.6
+Version: 0.0.7
 Summary: Spatial data format.
 Project-URL: Documentation, https://spatialdata.readthedocs.io/
 Project-URL: Source, https://github.com/scverse/spatialdata.git
 Project-URL: Home-page, https://github.com/scverse/spatialdata.git
 Author: scverse
 Maintainer-email: scverse <giov.pll@gmail.com>
 License: BSD 3-Clause License
@@ -65,50 +65,56 @@
 Requires-Dist: sphinx-book-theme>=1.0.0; extra == 'docs'
 Requires-Dist: sphinx-copybutton; extra == 'docs'
 Requires-Dist: sphinx-design; extra == 'docs'
 Requires-Dist: sphinx-rtd-theme; extra == 'docs'
 Requires-Dist: sphinx>=4.5; extra == 'docs'
 Requires-Dist: sphinxcontrib-bibtex>=1.0.0; extra == 'docs'
 Provides-Extra: extra
-Requires-Dist: napari-spatialdata; extra == 'extra'
+Requires-Dist: napari-spatialdata>=0.2.3; extra == 'extra'
 Requires-Dist: spatialdata-io; extra == 'extra'
 Requires-Dist: spatialdata-plot; extra == 'extra'
 Provides-Extra: test
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Provides-Extra: torch
 Requires-Dist: torch; extra == 'torch'
 Description-Content-Type: text/markdown
 
-# In review ⚠
+![SpatialData banner](https://github.com/scverse/spatialdata/blob/main/docs/_static/img/spatialdata_horizontal.png?raw=true)
 
--   **The library is currently under review.** We expect there to be changes as the community provides feedback.
--   To get involved in the discussion you are welcome to join our Zulip workspace and/or our community meetings every second week; [more info here](https://imagesc.zulipchat.com/#narrow/stream/329057-scverse/topic/SpatialData.20meetings).
--   Links to the OME-NGFF specification: [0.4](https://ngff.openmicroscopy.org/latest/), [0.5-dev (tables)](https://github.com/ome/ngff/pull/64), [0.5-dev (transformations and coordinate systems)](https://github.com/ome/ngff/pull/138)
-
-# spatialdata
+# SpatialData: an open and universal framework for processing spatial omics data.
 
 [![Tests][badge-tests]][link-tests]
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/scverse/spatialdata/main.svg)](https://results.pre-commit.ci/latest/github/scverse/spatialdata/main)
 [![codecov](https://codecov.io/gh/scverse/spatialdata/branch/main/graph/badge.svg?token=X19DRSIMCU)](https://codecov.io/gh/scverse/spatialdata)
-[![DOI](https://zenodo.org/badge/487366481.svg)](https://zenodo.org/badge/latestdoi/487366481)
+[![documentation badge](https://readthedocs.org/projects/scverse-spatialdata/badge/?version=latest)](https://spatialdata.scverse.org/en/latest/)
+
+SpatialData is a data framework that comprises a FAIR storage format and a collection of python libraries for performant access, alignment, and processing of uni- and multi-modal spatial omics datasets. This repository contains the core spatialdata library. See the links below to learn more about other packages in the SpatialData ecosystem.
 
-<img src='https://user-images.githubusercontent.com/1120672/236395765-2a4fc420-c7fb-4937-8a54-5036adc87760.png'/>
+-   [spatialdata-io](https://github.com/scverse/spatialdata-io): load data from common spatial omics technologies into spatialdata.
+-   [spatialdata-plot](https://github.com/scverse/spatialdata-plot): Static plotting library for spatialdata.
+-   [napari-spatialdata](https://github.com/scverse/napari-spatialdata): napari plugin for interactive exploration and annotation of spatialdata.
+
+![SpatialDataOverview](https://github.com/scverse/spatialdata/assets/1120672/cb91071f-12a7-4b8e-9430-2b3a0f65e52f)
+
+-   **The library is currently under review.** We expect there to be changes as the community provides feedback.
+-   To get involved in the discussion, or if you need help to get started, you are welcome to join our [`scverse` Zulip chat](https://imagesc.zulipchat.com/#narrow/stream/329057-scverse/topic/segmentation) and our [scverse discourse forum](https://discourse.scverse.org/).
+-   The SpatialData storage format is built on top of the [OME-NGFF](https://ngff.openmicroscopy.org/latest/) specification.
 
 ## Getting started
 
 Please refer to the [documentation][link-docs]. In particular:
 
 -   [API documentation][link-api].
 -   [Design doc][link-design-doc].
 -   [Example notebooks][link-notebooks].
 
 ## Installation
 
-Check out the docs for more complete installation instructions. To get started with the "batteries included" installation, you can install via pip:
+Check out the docs for more complete [installation instructions](https://spatialdata.scverse.org/en/latest/installation.html). To get started with the "batteries included" installation, you can install via pip:
 
 ```bash
 pip install "spatialdata[extra]"
 ```
 
 ## Contact
```

