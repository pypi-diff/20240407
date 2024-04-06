# Comparing `tmp/streamjoy-0.0.4.tar.gz` & `tmp/streamjoy-0.0.6.tar.gz`

## Comparing `streamjoy-0.0.4.tar` & `streamjoy-0.0.6.tar`

### file list

```diff
@@ -1,78 +1,81 @@
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 streamjoy-0.0.4/.editorconfig
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 streamjoy-0.0.4/CONTRIBUTING.md
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 streamjoy-0.0.4/HOWTOCONTRIBUTE.md
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 streamjoy-0.0.4/HOWTORELEASE.md
--rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 streamjoy-0.0.4/mkdocs.yml
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 streamjoy-0.0.4/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 streamjoy-0.0.4/.github/workflows/build.yml
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 streamjoy-0.0.4/.github/workflows/documentation.yml
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 streamjoy-0.0.4/.github/workflows/release.yml
--rw-r--r--   0        0        0     5502 2020-02-02 00:00:00.000000 streamjoy-0.0.4/docs/best_practices.md
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 streamjoy-0.0.4/docs/index.md
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 streamjoy-0.0.4/docs/package_design.md
--rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 streamjoy-0.0.4/docs/supported_formats.md
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 streamjoy-0.0.4/docs/api_reference/core.md
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 streamjoy-0.0.4/docs/api_reference/models.md
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 streamjoy-0.0.4/docs/api_reference/renderers.md
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 streamjoy-0.0.4/docs/api_reference/settings.md
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 streamjoy-0.0.4/docs/api_reference/streams.md
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 streamjoy-0.0.4/docs/api_reference/wrappers.md
--rw-r--r--   0        0        0    32485 2020-02-02 00:00:00.000000 streamjoy-0.0.4/docs/assets/design.svg
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 streamjoy-0.0.4/docs/example_recipes/air_temperature.md
--rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 streamjoy-0.0.4/docs/example_recipes/co2_timeseries.md
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 streamjoy-0.0.4/docs/example_recipes/gender_gapminder.md
--rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 streamjoy-0.0.4/docs/example_recipes/nice_orbit.md
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 streamjoy-0.0.4/docs/example_recipes/oisst_globe.md
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 streamjoy-0.0.4/docs/example_recipes/sea_ice.md
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 streamjoy-0.0.4/docs/example_recipes/sine_wave.md
--rw-r--r--   0        0        0     3579 2020-02-02 00:00:00.000000 streamjoy-0.0.4/docs/example_recipes/stream_code.md
--rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 streamjoy-0.0.4/docs/example_recipes/temperature_anomaly.md
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 streamjoy-0.0.4/docs/stylesheets/extra.css
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 streamjoy-0.0.4/streamjoy/.gitignore
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 streamjoy-0.0.4/streamjoy/__init__.py
--rw-r--r--   0        0        0    10055 2020-02-02 00:00:00.000000 streamjoy-0.0.4/streamjoy/_utils.py
--rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 streamjoy-0.0.4/streamjoy/core.py
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 streamjoy-0.0.4/streamjoy/models.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 streamjoy-0.0.4/streamjoy/pandas.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 streamjoy-0.0.4/streamjoy/polars.py
--rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 streamjoy-0.0.4/streamjoy/renderers.py
--rw-r--r--   0        0        0    20613 2020-02-02 00:00:00.000000 streamjoy-0.0.4/streamjoy/serializers.py
--rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 streamjoy-0.0.4/streamjoy/settings.py
--rw-r--r--   0        0        0    36573 2020-02-02 00:00:00.000000 streamjoy-0.0.4/streamjoy/streams.py
--rw-r--r--   0        0        0     4710 2020-02-02 00:00:00.000000 streamjoy-0.0.4/streamjoy/wrappers.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 streamjoy-0.0.4/streamjoy/xarray.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 streamjoy-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 streamjoy-0.0.4/tests/conftest.py
--rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 streamjoy-0.0.4/tests/test_core.py
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 streamjoy-0.0.4/tests/test_models.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 streamjoy-0.0.4/tests/test_pandas.py
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 streamjoy-0.0.4/tests/test_renderers.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 streamjoy-0.0.4/tests/test_settings.py
--rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 streamjoy-0.0.4/tests/test_streams.py
--rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 streamjoy-0.0.4/tests/test_wrappers.py
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 streamjoy-0.0.4/tests/test_xarray.py
--rw-r--r--   0        0        0    77959 2020-02-02 00:00:00.000000 streamjoy-0.0.4/tests/data/1978_10_Oct_N_19781026_conc_v3.0.png
--rw-r--r--   0        0        0    67272 2020-02-02 00:00:00.000000 streamjoy-0.0.4/tests/data/1978_10_Oct_N_19781027_conc_v3.0.png
--rw-r--r--   0        0        0    71503 2020-02-02 00:00:00.000000 streamjoy-0.0.4/tests/data/air.nc
--rw-r--r--   0        0        0     3685 2020-02-02 00:00:00.000000 streamjoy-0.0.4/tests/data/gapminder.csv
--rw-r--r--   0        0        0     8986 2020-02-02 00:00:00.000000 streamjoy-0.0.4/tests/data/gapminder.parquet
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 streamjoy-0.0.4/tests/data/air.zarr/.zattrs
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 streamjoy-0.0.4/tests/data/air.zarr/.zgroup
--rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 streamjoy-0.0.4/tests/data/air.zarr/.zmetadata
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 streamjoy-0.0.4/tests/data/air.zarr/air/.zarray
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 streamjoy-0.0.4/tests/data/air.zarr/air/.zattrs
--rw-r--r--   0        0        0    43023 2020-02-02 00:00:00.000000 streamjoy-0.0.4/tests/data/air.zarr/air/0.0.0
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 streamjoy-0.0.4/tests/data/air.zarr/lat/.zarray
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 streamjoy-0.0.4/tests/data/air.zarr/lat/.zattrs
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 streamjoy-0.0.4/tests/data/air.zarr/lat/0
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 streamjoy-0.0.4/tests/data/air.zarr/lon/.zarray
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 streamjoy-0.0.4/tests/data/air.zarr/lon/.zattrs
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 streamjoy-0.0.4/tests/data/air.zarr/lon/0
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 streamjoy-0.0.4/tests/data/air.zarr/time/.zarray
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 streamjoy-0.0.4/tests/data/air.zarr/time/.zattrs
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 streamjoy-0.0.4/tests/data/air.zarr/time/0
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 streamjoy-0.0.4/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 streamjoy-0.0.4/LICENSE
--rw-r--r--   0        0        0     6471 2020-02-02 00:00:00.000000 streamjoy-0.0.4/README.md
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 streamjoy-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     7077 2020-02-02 00:00:00.000000 streamjoy-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 streamjoy-0.0.6/.editorconfig
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 streamjoy-0.0.6/CONTRIBUTING.md
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 streamjoy-0.0.6/HOWTOCONTRIBUTE.md
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 streamjoy-0.0.6/HOWTORELEASE.md
+-rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 streamjoy-0.0.6/mkdocs.yml
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 streamjoy-0.0.6/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 streamjoy-0.0.6/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 streamjoy-0.0.6/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 streamjoy-0.0.6/.github/workflows/release.yml
+-rw-r--r--   0        0        0     7033 2020-02-02 00:00:00.000000 streamjoy-0.0.6/docs/how_do_i.md
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 streamjoy-0.0.6/docs/index.md
+-rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 streamjoy-0.0.6/docs/package_design.md
+-rw-r--r--   0        0        0     4954 2020-02-02 00:00:00.000000 streamjoy-0.0.6/docs/supported_formats.md
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 streamjoy-0.0.6/docs/api_reference/core.md
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 streamjoy-0.0.6/docs/api_reference/models.md
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 streamjoy-0.0.6/docs/api_reference/renderers.md
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 streamjoy-0.0.6/docs/api_reference/settings.md
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 streamjoy-0.0.6/docs/api_reference/streams.md
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 streamjoy-0.0.6/docs/api_reference/wrappers.md
+-rw-r--r--   0        0        0   282236 2020-02-02 00:00:00.000000 streamjoy-0.0.6/docs/assets/logo.png
+-rw-r--r--   0        0        0   301011 2020-02-02 00:00:00.000000 streamjoy-0.0.6/docs/assets/logo_bw.png
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 streamjoy-0.0.6/docs/example_recipes/air_temperature.md
+-rw-r--r--   0        0        0     4038 2020-02-02 00:00:00.000000 streamjoy-0.0.6/docs/example_recipes/co2_timeseries.md
+-rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 streamjoy-0.0.6/docs/example_recipes/gender_gapminder.md
+-rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 streamjoy-0.0.6/docs/example_recipes/nice_orbit.md
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 streamjoy-0.0.6/docs/example_recipes/oisst_globe.md
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 streamjoy-0.0.6/docs/example_recipes/sea_ice.md
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 streamjoy-0.0.6/docs/example_recipes/sine_wave.md
+-rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 streamjoy-0.0.6/docs/example_recipes/stream_code.md
+-rw-r--r--   0        0        0     4128 2020-02-02 00:00:00.000000 streamjoy-0.0.6/docs/example_recipes/temperature_anomaly.md
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 streamjoy-0.0.6/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 streamjoy-0.0.6/streamjoy/.gitignore
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 streamjoy-0.0.6/streamjoy/__init__.py
+-rw-r--r--   0        0        0    11516 2020-02-02 00:00:00.000000 streamjoy-0.0.6/streamjoy/_utils.py
+-rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 streamjoy-0.0.6/streamjoy/core.py
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 streamjoy-0.0.6/streamjoy/models.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 streamjoy-0.0.6/streamjoy/pandas.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 streamjoy-0.0.6/streamjoy/polars.py
+-rw-r--r--   0        0        0     4323 2020-02-02 00:00:00.000000 streamjoy-0.0.6/streamjoy/renderers.py
+-rw-r--r--   0        0        0    22305 2020-02-02 00:00:00.000000 streamjoy-0.0.6/streamjoy/serializers.py
+-rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 streamjoy-0.0.6/streamjoy/settings.py
+-rw-r--r--   0        0        0    37493 2020-02-02 00:00:00.000000 streamjoy-0.0.6/streamjoy/streams.py
+-rw-r--r--   0        0        0     4692 2020-02-02 00:00:00.000000 streamjoy-0.0.6/streamjoy/wrappers.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 streamjoy-0.0.6/streamjoy/xarray.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 streamjoy-0.0.6/tests/__init__.py
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 streamjoy-0.0.6/tests/conftest.py
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 streamjoy-0.0.6/tests/test_core.py
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 streamjoy-0.0.6/tests/test_models.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 streamjoy-0.0.6/tests/test_pandas.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 streamjoy-0.0.6/tests/test_polars.py
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 streamjoy-0.0.6/tests/test_renderers.py
+-rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 streamjoy-0.0.6/tests/test_serializers.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 streamjoy-0.0.6/tests/test_settings.py
+-rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 streamjoy-0.0.6/tests/test_streams.py
+-rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 streamjoy-0.0.6/tests/test_wrappers.py
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 streamjoy-0.0.6/tests/test_xarray.py
+-rw-r--r--   0        0        0    77959 2020-02-02 00:00:00.000000 streamjoy-0.0.6/tests/data/1978_10_Oct_N_19781026_conc_v3.0.png
+-rw-r--r--   0        0        0    67272 2020-02-02 00:00:00.000000 streamjoy-0.0.6/tests/data/1978_10_Oct_N_19781027_conc_v3.0.png
+-rw-r--r--   0        0        0    71503 2020-02-02 00:00:00.000000 streamjoy-0.0.6/tests/data/air.nc
+-rw-r--r--   0        0        0     3685 2020-02-02 00:00:00.000000 streamjoy-0.0.6/tests/data/gapminder.csv
+-rw-r--r--   0        0        0     8986 2020-02-02 00:00:00.000000 streamjoy-0.0.6/tests/data/gapminder.parquet
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 streamjoy-0.0.6/tests/data/air.zarr/.zattrs
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 streamjoy-0.0.6/tests/data/air.zarr/.zgroup
+-rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 streamjoy-0.0.6/tests/data/air.zarr/.zmetadata
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 streamjoy-0.0.6/tests/data/air.zarr/air/.zarray
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 streamjoy-0.0.6/tests/data/air.zarr/air/.zattrs
+-rw-r--r--   0        0        0    43023 2020-02-02 00:00:00.000000 streamjoy-0.0.6/tests/data/air.zarr/air/0.0.0
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 streamjoy-0.0.6/tests/data/air.zarr/lat/.zarray
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 streamjoy-0.0.6/tests/data/air.zarr/lat/.zattrs
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 streamjoy-0.0.6/tests/data/air.zarr/lat/0
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 streamjoy-0.0.6/tests/data/air.zarr/lon/.zarray
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 streamjoy-0.0.6/tests/data/air.zarr/lon/.zattrs
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 streamjoy-0.0.6/tests/data/air.zarr/lon/0
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 streamjoy-0.0.6/tests/data/air.zarr/time/.zarray
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 streamjoy-0.0.6/tests/data/air.zarr/time/.zattrs
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 streamjoy-0.0.6/tests/data/air.zarr/time/0
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 streamjoy-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 streamjoy-0.0.6/LICENSE
+-rw-r--r--   0        0        0     6589 2020-02-02 00:00:00.000000 streamjoy-0.0.6/README.md
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 streamjoy-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     7174 2020-02-02 00:00:00.000000 streamjoy-0.0.6/PKG-INFO
```

### Comparing `streamjoy-0.0.4/CONTRIBUTING.md` & `streamjoy-0.0.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.4/HOWTOCONTRIBUTE.md` & `streamjoy-0.0.6/HOWTOCONTRIBUTE.md`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.4/mkdocs.yml` & `streamjoy-0.0.6/mkdocs.yml`

 * *Files 8% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 repo_url: https://github.com/ahuang11/streamjoy
 repo_name: ahuang11/streamjoy
 
 theme:
     name: material
     features:
         - content.code.copy
-    icon:
-        logo: material/library
+    logo: assets/logo.png
     palette:
         # Palette toggle for automatic mode
         - media: "(prefers-color-scheme)"
           toggle:
             icon: material/brightness-auto
             name: Switch to light mode
 
@@ -38,17 +37,25 @@
 markdown_extensions:
     - toc:
         permalink: true
     - pymdownx.highlight:
         anchor_linenums: true
     - pymdownx.tasklist:
         custom_checkbox: true
+    - admonition
+    - pymdownx.details
+    - pymdownx.tabbed
+    - pymdownx.magiclink
     - pymdownx.inlinehilite
     - pymdownx.snippets
-    - pymdownx.superfences
+    - pymdownx.superfences:
+        custom_fences:
+        - name: mermaid
+          class: mermaid
+          format: !!python/name:pymdownx.superfences.fence_code_format
 
 plugins:
     - search
     - mkdocstrings:
         handlers:
             python:
                 options:
@@ -58,15 +65,15 @@
 watch:
     - docs
     - streamjoy
 
 nav:
     - Read me!: index.md
     - Supported formats: supported_formats.md
-    - Best practices: best_practices.md
+    - How do I...: how_do_i.md
     - Package design: package_design.md
     - Example recipes:
         - Air temperature: example_recipes/air_temperature.md
         - Sine wave: example_recipes/sine_wave.md
         - CO2 timeseries: example_recipes/co2_timeseries.md
         - Temperature anomaly: example_recipes/temperature_anomaly.md
         - Sea ice: example_recipes/sea_ice.md
```

### Comparing `streamjoy-0.0.4/.github/workflows/build.yml` & `streamjoy-0.0.6/.github/workflows/build.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 name: Build
 
-on: [push, pull_request]
+on: [pull_request]
 
 jobs:
   test:
 
     runs-on: ubuntu-latest
     strategy:
       matrix:
```

### Comparing `streamjoy-0.0.4/.github/workflows/documentation.yml` & `streamjoy-0.0.6/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.4/.github/workflows/release.yml` & `streamjoy-0.0.6/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.4/docs/best_practices.md` & `streamjoy-0.0.6/docs/how_do_i.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,22 @@
-# Best practices
+# How do I...
 
-## ⏸️ Take advantage of `Paused`, `intro_pause`, `ending_pause`
+## 🖼️ Use all resources with `max_frames=-1`
+
+By default, StreamJoy only renders the first 50 frames to prevent accidentally rendering a large dataset.
+
+To render all frames, set `max_frames=-1`.
+
+```python
+from streamjoy import stream
+
+stream(..., max_frames=-1)
+```
+
+## ⏸️ How to pause animations with `Paused`, `intro_pause`, `ending_pause`
 
 Animations can be good, but sometimes you want to pause at various points of the animation to provide context or to emphasize a point.
 
 To pause at a given frame using a custom `renderer`, wrap `Paused` around the output:
 
 ```python
 from streamjoy import stream
@@ -17,15 +29,15 @@
         return fig
 
 stream(..., renderer=plot_frame)
 ```
 
 Don't forget there's also `intro_pause` and `ending_pause` to pause at the beginning and end of the animation!
 
-## 📊 Decorate custom `renderer` with `wrap_*` decorators
+## 📊 Reduce boilerplate code with `wrap_*` decorators
 
 If you're using a custom `renderer`, you can use `wrap_matplotlib` and `wrap_holoviews` to automatically handle saving and closing the figure.
 
 ```python
 from streamjoy import stream, wrap_matplotlib
 
 @wrap_matplotlib()
@@ -41,53 +53,55 @@
 
 ```python
 from streamjoy import stream
 
 stream(..., intro_title="Himawari Visible", intro_subtitle="10 Hours Loop")
 ```
 
-## 💾 Save to memory for testing purposes
+## 💾 Write animation to memory instead of file
 
 If you're just testing out the animation, you can save it to memory instead of to disk by calling write without specifying a uri.
 
 ```python
 from streamjoy import stream
 
 stream(...).write()
 ```
 
-## 🚪 Use accessors for `pandas` and `xarray` objects
+## 🚪 Use as a method of `pandas` and `xarray` objects
+
+StreamJoy can be used directly from `pandas` and `xarray` objects as an accessor.
 
 ```python
 import pandas as pd
 import streamjoy.pandas
 
 df = pd.DataFrame(...)
 
 # equivalent to streamjoy.stream(df)
-df.stream(...)
+df.streamjoy(...)
 
 # series also works!
-df["col"].stream(...)
+df["col"].streamjoy(...)
 ```
 
 ```python
 import xarray as xr
 import streamjoy.xarray
 
 ds = xr.Dataset(...)
 
 # equivalent to streamjoy.stream(ds)
-ds.stream(...)
+ds.streamjoy(...)
 
 # dataarray also works!
-ds["var"].stream(...)
+ds["var"].streamjoy(...)
 ```
 
-## ⛓️ Use `sum` to join homogeneous streams and `connect` for hetereogenous
+## ⛓️ Join streams with `sum` and `connect`
 
 Use `sum` to join homogeneous streams, i.e. streams that have the same keyword arguments.
 
 ```python
 from streamjoy import stream, sum
 
 sum([stream(..., **same_kwargs) for i in range(10)])
@@ -97,21 +111,21 @@
 
 ```python
 from streamjoy import stream, connect
 
 connect([stream(..., **kwargs1), stream(..., **kwargs2)])
 ```
 
-## 🎥 When to use `.mp4` vs `.gif`
+## 🎥 Decide between writing as `.mp4` vs `.gif`
 
 If you need a comprehensive color palette, use `.mp4` as it supports more colors.
 
 For automatic playing and looping, use `.gif`. To reduce the file size of the `.gif`, set `optimize=True`, which uses `pygifsicle` to reduce the file size.
 
-## 📦 Wrap `streamjoy` functionality under `__name__ == "__main__"`
+## 📦 Prevent `RuntimeError` by using `__name__ == "__main__"`
 
 If you run a `.py` script without it, you might encounter the following `RuntimeError`:
 
 ```python
 RuntimeError:
 An attempt has been made to start a new process before the
 current process has finished its bootstrapping phase.
@@ -124,17 +138,24 @@
         freeze_support()
         ...
 
 The "freeze_support()" line can be omitted if the program
 is not going to be frozen to produce an executable.
 ```
 
+To patch, simply wrap your `stream` call in `if __name__ == "__main__":`.
+
+```python
+if __name__ == "__main__":
+    stream(...)
+```
+
 It's fine without it in notebooks though.
 
-## ⚙️ Change the default `config` settings
+## ⚙️ Set your own default settings with `config`
 
 StreamJoy uses a simple `config` dict to store settings. You can change the default settings by modifying the `streamjoy.config` object.
 
 To see the available options:
 ```python
 import streamjoy
 
@@ -151,50 +172,80 @@
 Be wary of completely overwriting the `config` object, as it might break the functionality; do not do this!
 ```python
 import streamjoy
 
 streamjoy.config = {"max_frames": -1}
 ```
 
-## 🔧 Explicitly set keyword arguments
+## 🔧 Use custom values instead of the defaults
 
 Much of StreamJoy is based on sensible defaults to get you started quickly, but you should override them.
 
 For example, `max_frames` is set to 50 by default so you can quickly preview the animation. If you want to render the entire animation, set `max_frames=-1`.
 
 StreamJoy will warn you on some settings if you don't override them:
 
 ```python
 No 'max_frames' specified; using the default 50 / 100 frames. Pass `-1` to use all frames. Suppress this by passing 'max_frames'.
 ```
 
-## 🧩 Use `processes=False` for rendering HoloViews objects
+## 🧩 Render HoloViews objects with `processes=False`
 
 This is done automatically! However, in case there's an edge case, note that the kdims/vdims don't seem to carry over properly to the subprocesses when rendering HoloViews objects. It might complain that it can't find the desired dimensions.
 
-## 📚 Use `threads_per_worker` if flickering
+## 📚 Prevent flickering by setting `threads_per_worker`
 
 Matplotlib is not always thread-safe, so if you're seeing flickering, set `threads_per_worker=1`.
 
 ```python
 from streamjoy import stream
 
 stream(..., threads_per_worker=1)
 ```
 
-## 🖥️ Specify `client` if using a remote cluster
+## 🖥️ Provide `client` if using a remote cluster
 
 If you're using a remote cluster, specify the `client` argument to use the Dask client.
 
 ```python
 from dask.distributed import Client
 
 client = Client()
 stream(..., client=client)
 ```
 
-## 🪣 Use `fsspec` to read/write intermediate files on a remote filesystem
+## 🪣 Read & write files on a remote filesystem with `fsspec_fs`
+
+To read and write files on a remote filesystem, use `fsspec_fs` to specify the filesystem.
+
+A scratch directory must be provided; be sure to prefix the bucket name.
 
 ```python
 fs = fsspec.filesystem('s3', anon=False)
 stream(..., fsspec_fs=fs, scratch_dir="bucket-name/streamjoy_scratch")
 ```
+
+## 🚗 Use a custom webdriver to render HoloViews
+
+By default, StreamJoy uses Firefox as the default headless webdriver to render HoloViews objects into images.
+
+If you want to use Chrome instead, you can pass `webdriver="chrome"`.
+
+If you want to use a different webdriver, you can pass a custom function to `webdriver`.
+
+```python
+def get_webdriver():
+    from selenium.webdriver.firefox.options import Options
+    from selenium.webdriver.firefox.webdriver import Service, WebDriver
+    from webdriver_manager.firefox import GeckoDriverManager
+
+    options = Options()
+    options.add_argument("--headless")
+    options.add_argument("--disable-extensions")
+    executable_path = GeckoDriverManager().install()
+    driver = WebDriver(
+        service=Service(executable_path), options=options
+    )
+    return driver
+
+stream(..., webdriver=get_webdriver)
+```
```

### Comparing `streamjoy-0.0.4/docs/package_design.md` & `streamjoy-0.0.6/docs/package_design.md`

 * *Files 4% similar despite different names*

```diff
@@ -12,19 +12,14 @@
 
 I also was thinking of naming this `streamio` and `streamit`, but the former was already taken and the latter too close to `streamlit`.
 
 ## 📶 Diagram
 
 Below is a diagram of the package design. The animation part is actually quite simple--most of the complexity comes with handling various input types, e.g. URLs, files, and datasets.
 
-<figure>
-    <img src="https://github.com/ahuang11/streamjoy/raw/main/docs/assets/design.svg" alt="StreamJoy package design" style="width:100%">
-    <figcaption>StreamJoy package design</figcaption>
-</figure>
-
 ```mermaid
 graph TD
     A[Start] --> Z{Input Type}
     Z -->|URL| U[Download and Assess Content]
     Z -->|Direct Input| V{Determine Content Type}
     U --> V
     V -->|DataFrame| B[Split pandas DataFrame]
```

### Comparing `streamjoy-0.0.4/docs/api_reference/settings.md` & `streamjoy-0.0.6/docs/api_reference/settings.md`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.4/docs/example_recipes/co2_timeseries.md` & `streamjoy-0.0.6/docs/example_recipes/co2_timeseries.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 Highlights:
 
 - Uses `wrap_matplotlib` to automatically handle saving and closing the figure.
 - Uses a custom `renderer` function to create each frame of the animation.
 - Uses `Paused` to pause the animation at notable dates.
 
-```python
+```python hl_lines="4 19 114"
 import pandas as pd
 import matplotlib.pyplot as plt
 from matplotlib.ticker import AutoMinorLocator
 from streamjoy import stream, wrap_matplotlib, Paused
 
 URL = "https://raw.githubusercontent.com/datasets/co2-ppm-daily/master/data/co2-ppm-daily.csv"
 NOTABLE_YEARS = {
```

### Comparing `streamjoy-0.0.4/docs/example_recipes/gender_gapminder.md` & `streamjoy-0.0.6/docs/example_recipes/gender_gapminder.md`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 Highlights:
 
 - Uses `intro_title` and `intro_subtitle` to set the title and subtitle of the video.
 - Uses `renderer_kwargs` to pass keyword arguments to the custom `renderer` function.
 - Updates `fps` to 30 to create a smoother animation.
 - Uses `connect` to concatenate the two heterogeneous streams (different keyword arguments with different titles) together.
 
-```python
+```python hl_lines="21-23 31 34"
 import pandas as pd
 from streamjoy import stream, connect
 
 if __name__ == "__main__":
     url_fmt = (
         "https://raw.githubusercontent.com/open-numbers/ddf--gapminder--systema_globalis/master/"
         "countries-etc-datapoints/ddf--datapoints--{gender}_population_with_projections--by--geo--time.csv"
```

### Comparing `streamjoy-0.0.4/docs/example_recipes/nice_orbit.md` & `streamjoy-0.0.6/docs/example_recipes/nice_orbit.md`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 All credits go to [Simone Conradi](https://github.com/profConradi); the only addition here was wrapping the code into a function and using `streamjoy` to create the animation. Please consider giving the [Python_Simulations](https://github.com/profConradi/Python_Simulations/tree/main) repo a star!
 
 Highlights:
 
 - Uses `wrap_matplotlib` to automatically handle saving and closing the figure.
 - Uses a custom `renderer` function to create each frame of the animation.
 
-```python
+```python hl_lines="45 46"
 import numpy as np
 import matplotlib.pyplot as plt
 from numba import njit
 from streamjoy import stream, wrap_matplotlib
 
 @njit
 def meshgrid(x, y):
```

### Comparing `streamjoy-0.0.4/docs/example_recipes/oisst_globe.md` & `streamjoy-0.0.6/docs/example_recipes/oisst_globe.md`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 Highlights:
 
 - Concatenates multiple homogeneous streams together (same keyword arguments, different resources) by summing them.
 - Uses the built-in `default_xarray_renderer` under the hood
 - Uses `renderer_kwargs` to pass keyword arguments to the underlying `ds.plot` method.
 
-```python
+```python hl_lines="19 32"
 import cartopy.crs as ccrs
 from streamjoy import stream
 
 YEAR = 2023
 URL_FMT = "https://www.ncei.noaa.gov/data/sea-surface-temperature-optimum-interpolation/v2.1/access/avhrr/{year}{month:02}/"
 
 if __name__ == "__main__":
```

### Comparing `streamjoy-0.0.4/docs/example_recipes/sea_ice.md` & `streamjoy-0.0.6/docs/example_recipes/sea_ice.md`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 Highlights:
 
 - Downloads images directly from the NSIDC FTP server.
 - Uses `connect` to concatenate the two homogeneous streams together (same keyword arguments, different resources).
 - Uses `pattern` to filter for only the sea ice concentration images.
 - Uses `intro_title` and `intro_subtitle` to provide context at the beginning of the animation.
 
-```python
+```python hl_lines="3 6-9"
 from streamjoy import stream, connect
 
 connect(
     [
         stream(
             f"https://noaadata.apps.nsidc.org/NOAA/G02135/north/daily/images/{year}/08_Aug/",
             pattern=f"N_*_conc_v3.0.png",
```

### Comparing `streamjoy-0.0.4/docs/example_recipes/sine_wave.md` & `streamjoy-0.0.6/docs/example_recipes/sine_wave.md`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Example of how to use `stream` alongside a custom `renderer` to create a sine wave animation.
 
 Highlights:
 
 - Uses `wrap_matplotlib` to automatically handle saving and closing the figure.
 - Uses a custom `renderer` function to create each frame of the animation.
 
-```python
+```python hl_lines="5-6 14"
 import matplotlib.pyplot as plt
 import numpy as np
 from streamjoy import stream, wrap_matplotlib
 
 @wrap_matplotlib()
 def plot_frame(i):
     x = np.linspace(0, 2, 1000)
```

### Comparing `streamjoy-0.0.4/docs/example_recipes/stream_code.md` & `streamjoy-0.0.6/docs/example_recipes/stream_code.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Generates an animation of a code snippet being written character by character.
 
 Highlights:
 
 - Uses a custom `renderer` function to create each frame of the animation.
 - Propagates `formatter`, `max_line_length`, and `max_line_number` to the custom `renderer` function.
 
-```python
+```python hl_lines="51 102-104"
 from textwrap import dedent
 
 import numpy as np
 from PIL import Image, ImageDraw
 from pygments import lex
 from pygments.formatters import ImageFormatter
 from pygments.lexers import get_lexer_by_name
```

### Comparing `streamjoy-0.0.4/docs/example_recipes/temperature_anomaly.md` & `streamjoy-0.0.6/docs/example_recipes/temperature_anomaly.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 Highlights:
 
 - Uses `wrap_matplotlib` to automatically handle saving and closing the figure.
 - Uses a custom `renderer` function to create each frame of the animation.
 - Uses `Paused` to pause the animation at notable dates.
 
-```python
+```python hl_lines="16 17 112"
 import pandas as pd
 import matplotlib.pyplot as plt
 from streamjoy import stream, wrap_matplotlib, Paused
 
 URL = "https://climexp.knmi.nl/data/ihadcrut5_global.dat"
 NOTABLE_DATES = {
     "1997-12": "Kyoto Protocol adopted",
```

### Comparing `streamjoy-0.0.4/streamjoy/__init__.py` & `streamjoy-0.0.6/streamjoy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     default_pandas_renderer,
     default_xarray_renderer,
 )
 from .settings import config, file_handlers, obj_handlers
 from .streams import GifStream, Mp4Stream
 from .wrappers import wrap_holoviews, wrap_matplotlib
 
-__version__ = "0.0.4"
+__version__ = "0.0.6"
 
 __all__ = [
     "GifStream",
     "ImageText",
     "Mp4Stream",
     "Paused",
     "config",
```

### Comparing `streamjoy-0.0.4/streamjoy/_utils.py` & `streamjoy-0.0.6/streamjoy/_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,14 +18,19 @@
 
 if TYPE_CHECKING:
     try:
         import xarray as xr
     except ImportError:
         xr = None
 
+    try:
+        from selenium.webdriver.remote.webdriver import BaseWebDriver
+    except ImportError:
+        BaseWebDriver = None
+
 
 def update_logger(
     level: str | None = None,
     format: str | None = None,
     datefmt: str | None = None,
 ) -> logging.Logger:
     success_level = config["logging_level"]
@@ -323,20 +328,58 @@
     else:
         return Paused(output=image, seconds=seconds)
 
 
 def subset_resources_renderer_iterables(
     resources: Any, renderer_iterables: list[Any], max_frames: int
 ):
-    if len(resources) > max_frames and max_frames != -1:
-        color = config["logging_warning_color"]
-        reset = config["logging_reset_color"]
-        logging.warning(
-            f"There are a total of {len(resources)} frames, "
-            f"but streaming only {color}{max_frames}{reset}. "
-            f"Set max_frames to -1 to stream all frames."
-        )
     resources = resources[: max_frames or max_frames]
     renderer_iterables = [
         iterable[: len(resources)] for iterable in renderer_iterables or []
     ]
     return resources, renderer_iterables
+
+
+def get_webdriver_path(webdriver: str):
+    if webdriver.lower() == "chrome":
+        from webdriver_manager.chrome import ChromeDriverManager
+
+        webdriver_path = ChromeDriverManager().install()
+    elif webdriver.lower() == "firefox":
+        from webdriver_manager.firefox import GeckoDriverManager
+
+        webdriver_path = GeckoDriverManager().install()
+    return webdriver_path
+
+
+def get_webdriver(webdriver: tuple[str, str] | Callable) -> BaseWebDriver:
+    if isinstance(webdriver, Callable):
+        return webdriver()
+
+    webdriver_key, webdriver_path = webdriver
+    if webdriver_key.lower() == "chrome":
+        from selenium.webdriver.chrome.options import Options
+        from selenium.webdriver.chrome.webdriver import Service, WebDriver
+
+        options = Options()
+        options.add_argument("--headless")
+        options.add_argument("--disable-extensions")
+        webdriver_path = webdriver_path or get_webdriver_path("chrome")
+        driver = WebDriver(service=Service(webdriver_path), options=options)
+
+    elif webdriver_key.lower() == "firefox":
+        from selenium.webdriver.firefox.options import Options
+        from selenium.webdriver.firefox.webdriver import Service, WebDriver
+
+        options = Options()
+        options.add_argument("--headless")
+        options.add_argument("--disable-extensions")
+        webdriver_path = webdriver_path or get_webdriver_path("firefox")
+        driver = WebDriver(service=Service(webdriver_path), options=options)
+
+    else:
+        raise NotImplementedError(
+            f"Webdriver {webdriver_key} not supported; "
+            f"use 'chrome' or 'firefox', or pass a custom callable."
+        )
+
+    return driver
```

### Comparing `streamjoy-0.0.4/streamjoy/core.py` & `streamjoy-0.0.6/streamjoy/core.py`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.4/streamjoy/models.py` & `streamjoy-0.0.6/streamjoy/models.py`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.4/streamjoy/polars.py` & `streamjoy-0.0.6/streamjoy/polars.py`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.4/streamjoy/renderers.py` & `streamjoy-0.0.6/streamjoy/renderers.py`

 * *Files 12% similar despite different names*

```diff
@@ -46,14 +46,15 @@
         A matplotlib figure.
     """
     import matplotlib.pyplot as plt
 
     df_sub = df_sub.reset_index()
 
     fig, ax = plt.subplots()
+
     title = kwargs.get("title")
     if title:
         title = title.format(**df_sub.iloc[-1])
     elif title is None:
         title = df_sub[kwargs["x"]].iloc[-1]
     kwargs["title"] = title
 
@@ -77,19 +78,28 @@
         df_sub: The DataFrame to render.
         *args: Additional positional arguments to pass to the renderer.
         **kwargs: Additional keyword arguments to pass to the renderer.
 
     Returns:
         The rendered HoloViews Element.
     """
+    backend = kwargs.pop("backend", None)
     by = kwargs.pop("groupby", None)
+
+    title = kwargs.get("title")
+    if title:
+        title = title.format(**df_sub.tail(1).to_pandas().to_dict("records")[0])
+    elif title is None:
+        title = df_sub[kwargs["x"]].tail(1)[0]
+    kwargs["title"] = str(title)
+
     if by:
         kwargs["by"] = by
     hv_obj = df_sub.plot(*args, **kwargs)
-    return default_holoviews_renderer(hv_obj)
+    return default_holoviews_renderer(hv_obj, backend=backend)
 
 
 def default_xarray_renderer(
     da_sel: xr.DataArray, *args: tuple[Any], **kwargs: dict[str, Any]
 ) -> plt.Figure:
     """
     Render an xarray DataArray using matplotlib.
@@ -104,18 +114,25 @@
     """
     import matplotlib.pyplot as plt
 
     da_sel = _utils.validate_xarray(da_sel, warn=False)
 
     fig = plt.figure()
     ax = plt.axes(**kwargs.pop("subplot_kws", {}))
+    title = kwargs.pop("title", None)
+
     try:
         da_sel.plot(ax=ax, extend="both", *args, **kwargs)
     except Exception:
         da_sel.plot(ax=ax, *args, **kwargs)
+
+    if title:
+        title_format = {coord: da_sel[coord].values for coord in da_sel.coords}
+        ax.set_title(title.format(**title_format))
+
     return fig
 
 
 def default_holoviews_renderer(
     hv_obj: hv.Element, *args: tuple[Any], **kwargs: dict[str, Any]
 ) -> hv.Element:
     """
@@ -127,24 +144,25 @@
         **kwargs: Additional keyword arguments to pass to the renderer.
 
     Returns:
         The rendered HoloViews Element.
     """
     import holoviews as hv
 
-    backend = kwargs.get("backend", "bokeh")
-    hv.extension(backend)
+    backend = kwargs.get("backend", hv.Store.current_backend)
 
     clims = kwargs.pop("clims", {})
     for hv_el in hv_obj.traverse(full_breadth=False):
         try:
             vdim = hv_el.vdims[0].name
         except IndexError:
             continue
         if vdim in clims:
-            hv_el.opts(clim=clims[vdim])
+            hv_el.opts(clim=clims[vdim], backend=backend)
 
     if backend == "bokeh":
         kwargs["toolbar"] = None
+    elif backend == "matplotlib":
+        kwargs["cbar_extend"] = kwargs.get("cbar_extend", "both")
     hv_obj.opts(**kwargs)
 
     return hv_obj
```

### Comparing `streamjoy-0.0.4/streamjoy/serializers.py` & `streamjoy-0.0.6/streamjoy/serializers.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,29 +44,58 @@
 
 def _select_obj_handler(resources: Any) -> MediaStream:
     if isinstance(resources, str) and "://" in resources:
         return serialize_url
     if isinstance(resources, (Path, str)):
         return serialize_paths
 
+    resources_type = type(resources)
+    module = getattr(resources_type, "__module__").split(".", maxsplit=1)[0]
+    type_ = resources_type.__name__
     for class_or_package_name, function_name in obj_handlers.items():
-        module = getattr(resources, "__module__", "").split(".", maxsplit=1)[0]
-        type_ = type(resources).__name__
         if (
             f"{module}.{type_}" == class_or_package_name
             or module == class_or_package_name
         ):
             return globals()[function_name]
 
     raise ValueError(
-        f"Could not find a method to handle {type(resources)}; "
+        f"Could not find a method to handle {resources_type}; "
         f"supported classes/packages are {list(obj_handlers.keys())}."
     )
 
 
+def serialize_numpy(
+    stream_cls,
+    resources: np.ndarray,
+    renderer: Callable | None = None,
+    renderer_iterables: list[Any] | None = None,
+    renderer_kwargs: dict | None = None,
+    **kwargs,
+) -> Serialized:
+    """
+    Serialize numpy arrays for streaming or rendering.
+
+    Args:
+        stream_cls: The class reference used for logging and utility functions.
+        resources: The numpy array to be serialized.
+        renderer: The rendering function to use on the array.
+        renderer_iterables: Additional iterable arguments to pass to the renderer.
+        renderer_kwargs: Additional keyword arguments to pass to the renderer.
+        **kwargs: Additional keyword arguments, including 'dim' and 'var' for xarray selection.
+
+    Returns:
+        A tuple containing the serialized resources, renderer, renderer_iterables, renderer_kwargs, and any additional keyword arguments.
+    """
+    resources = [resource for resource in resources]
+    renderer_kwargs = renderer_kwargs or {}
+    renderer_kwargs.update(_utils.pop_from_cls(stream_cls, kwargs))
+    return Serialized(resources, renderer, renderer_iterables, renderer_kwargs, kwargs)
+
+
 def serialize_xarray(
     stream_cls,
     resources: xr.Dataset | xr.DataArray,
     renderer: Callable | None = None,
     renderer_iterables: list[Any] | None = None,
     renderer_kwargs: dict | None = None,
     **kwargs,
@@ -104,14 +133,15 @@
     renderer_kwargs = renderer_kwargs or {}
     renderer_kwargs.update(_utils.pop_from_cls(stream_cls, kwargs))
 
     if renderer is None:
         renderer = wrap_matplotlib(
             in_memory=kwargs.get("in_memory"),
             scratch_dir=kwargs.get("scratch_dir"),
+            fsspec_fs=kwargs.get("fsspec_fs"),
         )(default_xarray_renderer)
         ds_0 = resources[0]
         if ds_0.ndim >= 2:
             renderer_kwargs["vmin"] = renderer_kwargs.get(
                 "vmin", _utils.get_result(ds_0.min()).item()
             )
             renderer_kwargs["vmax"] = renderer_kwargs.get(
@@ -165,14 +195,15 @@
     renderer_kwargs = renderer_kwargs or {}
     renderer_kwargs.update(_utils.pop_from_cls(stream_cls, kwargs))
 
     if renderer is None:
         renderer = wrap_matplotlib(
             in_memory=kwargs.get("in_memory"),
             scratch_dir=kwargs.get("scratch_dir"),
+            fsspec_fs=kwargs.get("fsspec_fs"),
         )(default_pandas_renderer)
         if "x" not in renderer_kwargs:
             if df.index.name or isinstance(df, pd.Series):
                 renderer_kwargs["x"] = df.index.name
             else:
                 for col in df.columns:
                     if col != groupby:
@@ -224,16 +255,16 @@
         A tuple containing the serialized resources, renderer, renderer_iterables, renderer_kwargs, and any additional keyword arguments.
     """
     import polars as pl
 
     groupby = kwargs.get("groupby")
 
     if groupby:
-        group_sizes = resources.groupby(groupby).agg(pl.count()).sort(by="count")
-        total_frames = group_sizes.select(pl.col("count").max()).to_numpy()[0, 0]
+        group_sizes = resources.groupby(groupby).agg(pl.len())
+        total_frames = group_sizes.select(pl.col("len").max()).to_numpy()[0, 0]
     else:
         total_frames = len(resources)
 
     max_frames = _utils.get_max_frames(total_frames, kwargs.get("max_frames"))
     resources_expanded = [
         resources.groupby(groupby).head(i) if groupby else resources.head(i)
         for i in range(1, max_frames + 1)
@@ -242,14 +273,16 @@
     renderer_kwargs = renderer_kwargs or {}
     renderer_kwargs.update(_utils.pop_from_cls(stream_cls, kwargs))
 
     if renderer is None:
         renderer = wrap_holoviews(
             in_memory=kwargs.get("in_memory"),
             scratch_dir=kwargs.get("scratch_dir"),
+            fsspec_fs=kwargs.get("fsspec_fs"),
+            webdriver=renderer_kwargs.pop("webdriver", None),
         )(default_polars_renderer)
         numeric_cols = [
             col
             for col in resources.columns
             if resources[col].dtype in [pl.Float64, pl.Int64, pl.Float32, pl.Int32]
         ]
         if "x" not in renderer_kwargs:
@@ -269,14 +302,20 @@
                 "y", renderer_kwargs["y"], suffix="from the dataframe"
             )
         if "xlabel" not in renderer_kwargs:
             renderer_kwargs["xlabel"] = renderer_kwargs["x"].title().replace("_", " ")
         if "ylabel" not in renderer_kwargs:
             renderer_kwargs["ylabel"] = renderer_kwargs["y"].title().replace("_", " ")
 
+    if kwargs.get("processes"):
+        logging.warning(
+            "Polars (HoloViews) rendering does not support processes; "
+            "setting processes=False."
+        )
+    kwargs["processes"] = False
     return Serialized(
         resources_expanded, renderer, renderer_iterables, renderer_kwargs, kwargs
     )
 
 
 def serialize_holoviews(
     stream_cls,
@@ -298,16 +337,15 @@
         **kwargs: Additional keyword arguments for HoloViews object customization.
 
     Returns:
         A tuple containing the serialized resources, renderer, renderer_iterables, renderer_kwargs, and any additional keyword arguments.
     """
     import holoviews as hv
 
-    backend = hv.Store.current_backend
-    hv.extension(backend)
+    backend = kwargs.get("backend", hv.Store.current_backend)
 
     def _select_element(hv_obj, key):
         try:
             resource = hv_obj[key]
         except Exception:
             resource = hv_obj.select(**{kdims[0].name: key})
         return resource
@@ -337,26 +375,29 @@
     renderer_kwargs = renderer_kwargs or {}
     renderer_kwargs.update(_utils.pop_from_cls(stream_cls, kwargs))
 
     if renderer is None:
         renderer = wrap_holoviews(
             in_memory=kwargs.get("in_memory"),
             scratch_dir=kwargs.get("scratch_dir"),
+            fsspec_fs=kwargs.get("fsspec_fs"),
+            webdriver=renderer_kwargs.pop("webdriver", None),
         )(default_holoviews_renderer)
         clims = {}
         for hv_el in hv_obj.traverse(full_breadth=False):
             if isinstance(hv_el, hv.DynamicMap):
                 hv.render(hv_el, backend=backend)
 
             if isinstance(hv_el, hv.Element):
                 if hv_el.ndims > 1:
                     vdim = hv_el.vdims[0].name
                     array = hv_el.dimension_values(vdim)
                     clim = (np.nanmin(array), np.nanmax(array))
                     clims[vdim] = clim
+
         renderer_kwargs.update(
             backend=backend,
             clims=clims,
         )
 
     if kwargs.get("processes"):
         logging.warning(
```

### Comparing `streamjoy-0.0.4/streamjoy/settings.py` & `streamjoy-0.0.6/streamjoy/settings.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,14 +10,16 @@
     "intro_pause": 2,
     "intro_watermark": "made with streamjoy",
     "intro_background": "black",
     # from_url
     "max_files": 2,
     # matplotlib
     "max_open_warning": 100,
+    # holoviews
+    "webdriver": "firefox",
     # output
     "in_memory": False,
     "scratch_dir": "streamjoy_scratch",
     "uri": None,
     # imageio
     "codec": "libx264",
     "loop": 0,
@@ -44,15 +46,15 @@
 obj_handlers = {
     "xarray.Dataset": "serialize_xarray",
     "xarray.DataArray": "serialize_xarray",
     "pandas.DataFrame": "serialize_pandas",
     "pandas.Series": "serialize_pandas",
     "holoviews": "serialize_holoviews",
     "polars.DataFrame": "serialize_polars",
-    "polars.Series": "serialize_polars",
+    "numpy.ndarray": "serialize_numpy",
 }
 
 file_handlers = {
     ".nc": {
         "import_path": "xarray.open_mfdataset",
     },
     ".nc4": {
```

### Comparing `streamjoy-0.0.4/streamjoy/streams.py` & `streamjoy-0.0.6/streamjoy/streams.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,14 +193,33 @@
         for param_key in set(params):
             if param_key not in self.param:
                 params["_tbd_kwargs"][param_key] = params.pop(param_key)
 
         super().__init__(**params)
 
     @classmethod
+    def from_numpy(
+        cls,
+        array: np.ndarray,
+        renderer: Callable | None = None,
+        renderer_iterables: list[Any] | None = None,
+        renderer_kwargs: dict | None = None,
+        **kwargs,
+    ) -> MediaStream:
+        serialized = serialize_appropriately(
+            cls,
+            resources=array,
+            renderer=renderer,
+            renderer_iterables=renderer_iterables,
+            renderer_kwargs=renderer_kwargs,
+            **kwargs,
+        )
+        return cls(**serialized.param.values(), **serialized.kwargs)
+
+    @classmethod
     def from_xarray(
         cls,
         ds: xr.Dataset | xr.DataArray,
         renderer: Callable | None = None,
         renderer_iterables: list[Any] | None = None,
         renderer_kwargs: dict | None = None,
         dim: str | None = None,
@@ -534,14 +553,21 @@
                 setattr(self, key, value)
             else:
                 renderer_kwargs[key] = value
 
         if resources is None:
             resources = self.resources
             renderer_iterables = self.renderer_iterables
+            max_frames = _utils.get_max_frames(
+                len(resources), kwargs.get("max_frames", self.max_frames)
+            )
+            kwargs["max_frames"] = max_frames
+            resources, renderer_iterables = _utils.subset_resources_renderer_iterables(
+                resources, renderer_iterables, max_frames
+            )
         else:
             serialized = serialize_appropriately(
                 self, resources, renderer, renderer_kwargs, **kwargs
             )
             resources = serialized.resources
             renderer = serialized.renderer
             renderer_iterables = serialized.renderer_iterables
```

### Comparing `streamjoy-0.0.4/streamjoy/xarray.py` & `streamjoy-0.0.6/streamjoy/xarray.py`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.4/tests/conftest.py` & `streamjoy-0.0.6/tests/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from pathlib import Path
 
 import hvplot.xarray  # noqa: F401
+import imageio.v3 as iio
 import pandas as pd
 import polars as pl
 import pytest
 import xarray as xr
 
 from streamjoy._utils import get_distributed_client
 from streamjoy.settings import config
@@ -13,14 +14,19 @@
 NC_PATH = DATA_DIR / "air.nc"
 ZARR_PATH = DATA_DIR / "air.zarr"
 CSV_PATH = DATA_DIR / "gapminder.csv"
 PARQUET_PATH = DATA_DIR / "gapminder.parquet"
 
 
 @pytest.fixture
+def array():
+    return iio.imread("imageio:newtonscradle.gif")
+
+
+@pytest.fixture
 def ds():
     return xr.open_zarr(ZARR_PATH)
 
 
 @pytest.fixture
 def df():
     return pd.read_parquet(PARQUET_PATH)
```

### Comparing `streamjoy-0.0.4/tests/test_core.py` & `streamjoy-0.0.6/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.4/tests/test_models.py` & `streamjoy-0.0.6/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.4/tests/test_pandas.py` & `streamjoy-0.0.6/tests/test_pandas.py`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.4/tests/test_settings.py` & `streamjoy-0.0.6/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.4/tests/test_streams.py` & `streamjoy-0.0.6/tests/test_streams.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,14 +8,19 @@
 
 class AbstractTestMediaStream:
     def _assert_stream_and_props(self, sj, stream_cls):
         assert isinstance(sj, stream_cls)
         buf = sj.write()
         props = improps(buf)
         props.n_images == 3
+        return props
+
+    def test_from_numpy(self, stream_cls, array):
+        sj = stream_cls.from_numpy(array)
+        self._assert_stream_and_props(sj, stream_cls)
 
     def test_from_pandas(self, stream_cls, df):
         sj = stream_cls.from_pandas(df)
         self._assert_stream_and_props(sj, stream_cls)
 
     def test_from_polars(self, stream_cls, pl_df):
         sj = stream_cls.from_polars(pl_df)
@@ -50,14 +55,34 @@
         sj = stream_cls.from_directory(data_dir, pattern="*.png")
         self._assert_stream_and_props(sj, stream_cls)
 
     def test_fsspec_fs(self, stream_cls, df, fsspec_fs):
         sj = stream_cls.from_pandas(df, fsspec_fs=fsspec_fs)
         self._assert_stream_and_props(sj, stream_cls)
 
+    def test_holoviews_matplotlib_backend(self, stream_cls, ds):
+        sj = stream_cls.from_holoviews(
+            ds.hvplot("lon", "lat", fig_size=200, backend="matplotlib")
+        )
+        props = self._assert_stream_and_props(sj, stream_cls)
+        assert props.shape[1] == 300
+
+    def test_holoviews_bokeh_backend(self, stream_cls, ds):
+        sj = stream_cls.from_holoviews(
+            ds.hvplot("lon", "lat", width=300, backend="bokeh")
+        )
+        props = self._assert_stream_and_props(sj, stream_cls)
+        assert props.shape[1] == 300
+
+    def test_write_max_frames(self, stream_cls, df):
+        sj = stream_cls.from_pandas(df, max_frames=3)
+        buf = sj.write(max_frames=2)
+        props = improps(buf)
+        assert props.n_images == 2
+
 
 class TestGifStream(AbstractTestMediaStream):
     @pytest.fixture(scope="class")
     def stream_cls(self):
         return GifStream
 
     def test_paused(self, stream_cls, df):
```

### Comparing `streamjoy-0.0.4/tests/test_wrappers.py` & `streamjoy-0.0.6/tests/test_wrappers.py`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.4/tests/test_xarray.py` & `streamjoy-0.0.6/tests/test_xarray.py`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.4/tests/data/1978_10_Oct_N_19781026_conc_v3.0.png` & `streamjoy-0.0.6/tests/data/1978_10_Oct_N_19781026_conc_v3.0.png`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.4/tests/data/1978_10_Oct_N_19781027_conc_v3.0.png` & `streamjoy-0.0.6/tests/data/1978_10_Oct_N_19781027_conc_v3.0.png`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.4/tests/data/air.nc` & `streamjoy-0.0.6/tests/data/air.nc`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.4/tests/data/gapminder.csv` & `streamjoy-0.0.6/tests/data/gapminder.csv`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.4/tests/data/gapminder.parquet` & `streamjoy-0.0.6/tests/data/gapminder.parquet`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.4/tests/data/air.zarr/.zmetadata` & `streamjoy-0.0.6/tests/data/air.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.4/tests/data/air.zarr/air/0.0.0` & `streamjoy-0.0.6/tests/data/air.zarr/air/0.0.0`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.4/.gitignore` & `streamjoy-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.4/LICENSE` & `streamjoy-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.4/README.md` & `streamjoy-0.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -118,19 +118,20 @@
 ### 🖇️ Connect streams
 
 Connect multiple streams together to provide further context.
 
 ```python
 from streamjoy import stream, connect
 
+URL_FMTS = {
+    "visible": "https://www.goes.noaa.gov/dimg/jma/fd/vis/{i}.gif",
+    "infrared": "https://www.goes.noaa.gov/dimg/jma/fd/rbtop/{i}.gif",
+}
+
 if __name__ == "__main__":
-    URL_FMTS = {
-        "visible": "https://www.goes.noaa.gov/dimg/jma/fd/vis/{i}.gif",
-        "infrared": "https://www.goes.noaa.gov/dimg/jma/fd/rbtop/{i}.gif",
-    }
     visible_stream = stream(
         [URL_FMTS["visible"].format(i=i) for i in range(1, 11)],
         intro_title="Himawari Visible",
         intro_subtitle="10 Hours Loop",
     )
     infrared_stream = stream(
         [URL_FMTS["infrared"].format(i=i) for i in range(1, 11)],
@@ -142,14 +143,20 @@
 
 <img src="https://github.com/ahuang11/streamjoy/assets/15331990/5f6e0435-f2c2-4c3e-bcf9-4c84d4d060e9" width="500" height="500">
 
 ### 📷 Render datasets
 
 You can also render images directly from datasets, either through a custom renderer or a built-in one, and they'll also run in parallel!
 
+The following example requires xarray, cartopy, matplotlib, and netcdf4.
+
+```bash
+pip install xarray cartopy matplotlib netcdf4
+```
+
 ```python
 import numpy as np
 import cartopy.crs as ccrs
 import matplotlib.pyplot as plt
 from streamjoy import stream, wrap_matplotlib
 
 @wrap_matplotlib()
```

### Comparing `streamjoy-0.0.4/pyproject.toml` & `streamjoy-0.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,14 @@
 dynamic = ["version"]
 classifiers = [
     "Programming Language :: Python :: 3 :: Only",
 ]
 requires-python = ">=3.9"
 dependencies = [
     "param",
-    "bokeh",
     "dask[distributed]",
     "imageio[pyav]>=2.34.0",
     "pygifsicle==1.0.5",
     "requests",
     "bs4",
 ]
```

### Comparing `streamjoy-0.0.4/PKG-INFO` & `streamjoy-0.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.3
 Name: streamjoy
-Version: 0.0.4
+Version: 0.0.6
 Summary: Enjoy animating images into GIFs and MP4s!
 Project-URL: Documentation, https://ahuang11.github.io/streamjoy/
 Project-URL: Source, https://github.com/ahuang11/streamjoy
 Author-email: streamjoy <hey.at.py@gmail.com>
 License-File: LICENSE
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9
-Requires-Dist: bokeh
 Requires-Dist: bs4
 Requires-Dist: dask[distributed]
 Requires-Dist: imageio[pyav]>=2.34.0
 Requires-Dist: param
 Requires-Dist: pygifsicle==1.0.5
 Requires-Dist: requests
 Description-Content-Type: text/markdown
@@ -137,19 +136,20 @@
 ### 🖇️ Connect streams
 
 Connect multiple streams together to provide further context.
 
 ```python
 from streamjoy import stream, connect
 
+URL_FMTS = {
+    "visible": "https://www.goes.noaa.gov/dimg/jma/fd/vis/{i}.gif",
+    "infrared": "https://www.goes.noaa.gov/dimg/jma/fd/rbtop/{i}.gif",
+}
+
 if __name__ == "__main__":
-    URL_FMTS = {
-        "visible": "https://www.goes.noaa.gov/dimg/jma/fd/vis/{i}.gif",
-        "infrared": "https://www.goes.noaa.gov/dimg/jma/fd/rbtop/{i}.gif",
-    }
     visible_stream = stream(
         [URL_FMTS["visible"].format(i=i) for i in range(1, 11)],
         intro_title="Himawari Visible",
         intro_subtitle="10 Hours Loop",
     )
     infrared_stream = stream(
         [URL_FMTS["infrared"].format(i=i) for i in range(1, 11)],
@@ -161,14 +161,20 @@
 
 <img src="https://github.com/ahuang11/streamjoy/assets/15331990/5f6e0435-f2c2-4c3e-bcf9-4c84d4d060e9" width="500" height="500">
 
 ### 📷 Render datasets
 
 You can also render images directly from datasets, either through a custom renderer or a built-in one, and they'll also run in parallel!
 
+The following example requires xarray, cartopy, matplotlib, and netcdf4.
+
+```bash
+pip install xarray cartopy matplotlib netcdf4
+```
+
 ```python
 import numpy as np
 import cartopy.crs as ccrs
 import matplotlib.pyplot as plt
 from streamjoy import stream, wrap_matplotlib
 
 @wrap_matplotlib()
```

