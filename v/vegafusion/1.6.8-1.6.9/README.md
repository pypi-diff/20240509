# Comparing `tmp/vegafusion-1.6.8.tar.gz` & `tmp/vegafusion-1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vegafusion-1.6.8.tar", last modified: Tue May  7 14:03:45 2024, max compression
+gzip compressed data, was "vegafusion-1.6.9.tar", last modified: Thu May  9 17:39:41 2024, max compression
```

## Comparing `vegafusion-1.6.8.tar` & `vegafusion-1.6.9.tar`

### file list

```diff
@@ -1,403 +1,406 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.500220 vegafusion-1.6.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-07 14:03:06.000000 vegafusion-1.6.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-07 14:03:45.500220 vegafusion-1.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-07 14:03:06.000000 vegafusion-1.6.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.472220 vegafusion-1.6.8/proto/
--rw-r--r--   0 runner    (1001) docker     (127)    38178 2024-05-07 14:03:06.000000 vegafusion-1.6.8/proto/datafusion.proto
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-07 14:03:06.000000 vegafusion-1.6.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-07 14:03:06.000000 vegafusion-1.6.8/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-07 14:03:45.500220 vegafusion-1.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 14:03:06.000000 vegafusion-1.6.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.472220 vegafusion-1.6.8/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.468220 vegafusion-1.6.8/tests/altair_mocks/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.456219 vegafusion-1.6.8/tests/altair_mocks/area/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.472220 vegafusion-1.6.8/tests/altair_mocks/area/cumulative_count/
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/area/cumulative_count/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.472220 vegafusion-1.6.8/tests/altair_mocks/area/density_facet/
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/area/density_facet/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.472220 vegafusion-1.6.8/tests/altair_mocks/area/density_stack/
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/area/density_stack/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.472220 vegafusion-1.6.8/tests/altair_mocks/area/gradient/
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/area/gradient/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.472220 vegafusion-1.6.8/tests/altair_mocks/area/horizon_graph/
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/area/horizon_graph/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.472220 vegafusion-1.6.8/tests/altair_mocks/area/layered/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/area/layered/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.472220 vegafusion-1.6.8/tests/altair_mocks/area/normalized_stacked/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/area/normalized_stacked/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.472220 vegafusion-1.6.8/tests/altair_mocks/area/streamgraph/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/area/streamgraph/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.472220 vegafusion-1.6.8/tests/altair_mocks/area/trellis/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/area/trellis/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.472220 vegafusion-1.6.8/tests/altair_mocks/area/trellis_sort_array/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/area/trellis_sort_array/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.456219 vegafusion-1.6.8/tests/altair_mocks/bar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.472220 vegafusion-1.6.8/tests/altair_mocks/bar/and_tick_chart/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/bar/and_tick_chart/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/bar/diverging_stacked/
--rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/bar/diverging_stacked/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/bar/grouped/
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/bar/grouped/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/bar/horizontal/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/bar/horizontal/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/bar/horizontal_grouped/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/bar/horizontal_grouped/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/bar/horizontal_stacked/
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/bar/horizontal_stacked/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/bar/layered/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/bar/layered/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/bar/normalized_stacked/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/bar/normalized_stacked/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/bar/percentage_of_total/
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/bar/percentage_of_total/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/bar/sorted/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/bar/sorted/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/bar/stacked/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/bar/stacked/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/bar/stacked_with_sorted_segments/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/bar/stacked_with_sorted_segments/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/bar/stacked_with_text_overlay/
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/bar/stacked_with_text_overlay/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/bar/trellis_compact/
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/bar/trellis_compact/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/bar/trellis_stacked/
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/bar/trellis_stacked/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/bar/with_error_bars/
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/bar/with_error_bars/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/bar/with_highlighted_bar/
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/bar/with_highlighted_bar/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/bar/with_labels/
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/bar/with_labels/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/bar/with_line_at_mean/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/bar/with_line_at_mean/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/bar/with_line_on_dual_axis/
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/bar/with_line_on_dual_axis/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/bar/with_negative_values/
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/bar/with_negative_values/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/bar/with_rolling_mean/
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/bar/with_rolling_mean/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/bar/with_rounded_edges/
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/bar/with_rounded_edges/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.460219 vegafusion-1.6.8/tests/altair_mocks/casestudy/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/casestudy/airports/
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/casestudy/airports/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/casestudy/anscombe_plot/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/casestudy/anscombe_plot/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/casestudy/beckers_barley_trellis_plot/
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/casestudy/beckers_barley_trellis_plot/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/casestudy/co2_concentration/
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/casestudy/co2_concentration/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/casestudy/falkensee/
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/casestudy/falkensee/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/casestudy/gapminder_bubble_plot/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/casestudy/gapminder_bubble_plot/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/casestudy/iowa_electricity/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/casestudy/iowa_electricity/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/casestudy/isotype/
--rw-r--r--   0 runner    (1001) docker     (127)     5881 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/casestudy/isotype/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.476220 vegafusion-1.6.8/tests/altair_mocks/casestudy/isotype_emoji/
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/casestudy/isotype_emoji/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.480220 vegafusion-1.6.8/tests/altair_mocks/casestudy/london_tube/
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/casestudy/london_tube/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.480220 vegafusion-1.6.8/tests/altair_mocks/casestudy/natural_disasters/
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/casestudy/natural_disasters/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.480220 vegafusion-1.6.8/tests/altair_mocks/casestudy/one_dot_per_zipcode/
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/casestudy/one_dot_per_zipcode/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.480220 vegafusion-1.6.8/tests/altair_mocks/casestudy/top_k_items/
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/casestudy/top_k_items/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.480220 vegafusion-1.6.8/tests/altair_mocks/casestudy/top_k_letters/
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/casestudy/top_k_letters/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.480220 vegafusion-1.6.8/tests/altair_mocks/casestudy/top_k_with_others/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/casestudy/top_k_with_others/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.480220 vegafusion-1.6.8/tests/altair_mocks/casestudy/us_employment/
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/casestudy/us_employment/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.480220 vegafusion-1.6.8/tests/altair_mocks/casestudy/us_population_over_time_facet/
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/casestudy/us_population_over_time_facet/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.480220 vegafusion-1.6.8/tests/altair_mocks/casestudy/us_state_capitals/
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/casestudy/us_state_capitals/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.480220 vegafusion-1.6.8/tests/altair_mocks/casestudy/wheat_wages/
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/casestudy/wheat_wages/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.480220 vegafusion-1.6.8/tests/altair_mocks/casestudy/window_rank/
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/casestudy/window_rank/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.460219 vegafusion-1.6.8/tests/altair_mocks/circular/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.480220 vegafusion-1.6.8/tests/altair_mocks/circular/donut/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/circular/donut/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.480220 vegafusion-1.6.8/tests/altair_mocks/circular/pacman/
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/circular/pacman/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.480220 vegafusion-1.6.8/tests/altair_mocks/circular/pie/
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/circular/pie/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.480220 vegafusion-1.6.8/tests/altair_mocks/circular/pie_with_labels/
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/circular/pie_with_labels/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.480220 vegafusion-1.6.8/tests/altair_mocks/circular/radial/
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/circular/radial/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.460219 vegafusion-1.6.8/tests/altair_mocks/histogram/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.480220 vegafusion-1.6.8/tests/altair_mocks/histogram/layered/
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/histogram/layered/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.480220 vegafusion-1.6.8/tests/altair_mocks/histogram/trellis/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/histogram/trellis/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.480220 vegafusion-1.6.8/tests/altair_mocks/histogram/with_a_global_mean_overlay/
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/histogram/with_a_global_mean_overlay/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.464219 vegafusion-1.6.8/tests/altair_mocks/interactive/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.480220 vegafusion-1.6.8/tests/altair_mocks/interactive/area-interval_selection/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/area-interval_selection/actions.json
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/area-interval_selection/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.480220 vegafusion-1.6.8/tests/altair_mocks/interactive/brush/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/brush/actions.json
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/brush/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.480220 vegafusion-1.6.8/tests/altair_mocks/interactive/casestudy-airport_connections/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/casestudy-airport_connections/actions.json
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/casestudy-airport_connections/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.480220 vegafusion-1.6.8/tests/altair_mocks/interactive/casestudy-seattle_weather_interactive/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/casestudy-seattle_weather_interactive/actions.json
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/casestudy-seattle_weather_interactive/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.480220 vegafusion-1.6.8/tests/altair_mocks/interactive/casestudy-us_population_over_time/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/casestudy-us_population_over_time/actions.json
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/casestudy-us_population_over_time/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.480220 vegafusion-1.6.8/tests/altair_mocks/interactive/casestudy-us_population_pyramid_over_time/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/casestudy-us_population_pyramid_over_time/actions.json
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/casestudy-us_population_pyramid_over_time/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.480220 vegafusion-1.6.8/tests/altair_mocks/interactive/casestudy-weather_heatmap/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/casestudy-weather_heatmap/actions.json
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/casestudy-weather_heatmap/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.484220 vegafusion-1.6.8/tests/altair_mocks/interactive/cross_highlight/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/cross_highlight/actions.json
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/cross_highlight/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.484220 vegafusion-1.6.8/tests/altair_mocks/interactive/histogram-responsive/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/histogram-responsive/actions.json
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/histogram-responsive/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.484220 vegafusion-1.6.8/tests/altair_mocks/interactive/layered_crossfilter/
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/layered_crossfilter/actions.json
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/layered_crossfilter/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.484220 vegafusion-1.6.8/tests/altair_mocks/interactive/legend/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/legend/actions.json
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/legend/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.484220 vegafusion-1.6.8/tests/altair_mocks/interactive/multiline_highlight/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/multiline_highlight/actions.json
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/multiline_highlight/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.484220 vegafusion-1.6.8/tests/altair_mocks/interactive/multiline_tooltip/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/multiline_tooltip/actions.json
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/multiline_tooltip/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.484220 vegafusion-1.6.8/tests/altair_mocks/interactive/other-image_tooltip/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/other-image_tooltip/actions.json
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/other-image_tooltip/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.484220 vegafusion-1.6.8/tests/altair_mocks/interactive/scatter-href/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/scatter-href/actions.json
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/scatter-href/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.484220 vegafusion-1.6.8/tests/altair_mocks/interactive/scatter-with_linked_table/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/scatter-with_linked_table/actions.json
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/scatter-with_linked_table/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.484220 vegafusion-1.6.8/tests/altair_mocks/interactive/scatter-with_minimap/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/scatter-with_minimap/actions.json
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/scatter-with_minimap/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.484220 vegafusion-1.6.8/tests/altair_mocks/interactive/scatter_linked_brush/
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/scatter_linked_brush/actions.json
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/scatter_linked_brush/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.484220 vegafusion-1.6.8/tests/altair_mocks/interactive/scatter_plot/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/scatter_plot/actions.json
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/scatter_plot/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.484220 vegafusion-1.6.8/tests/altair_mocks/interactive/scatter_with_histogram/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/scatter_with_histogram/actions.json
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/scatter_with_histogram/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.484220 vegafusion-1.6.8/tests/altair_mocks/interactive/scatter_with_layered_histogram/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/scatter_with_layered_histogram/actions.json
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/scatter_with_layered_histogram/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.484220 vegafusion-1.6.8/tests/altair_mocks/interactive/select_detail/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/select_detail/actions.json
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/select_detail/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.484220 vegafusion-1.6.8/tests/altair_mocks/interactive/select_mark_area/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/select_mark_area/actions.json
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/select_mark_area/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.488220 vegafusion-1.6.8/tests/altair_mocks/interactive/selection_histogram/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/selection_histogram/actions.json
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/selection_histogram/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.488220 vegafusion-1.6.8/tests/altair_mocks/interactive/selection_layer_bar_month/
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/selection_layer_bar_month/actions.json
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/interactive/selection_layer_bar_month/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.464219 vegafusion-1.6.8/tests/altair_mocks/line/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.488220 vegafusion-1.6.8/tests/altair_mocks/line/bump_chart/
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/line/bump_chart/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.488220 vegafusion-1.6.8/tests/altair_mocks/line/filled_step_chart/
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/line/filled_step_chart/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.488220 vegafusion-1.6.8/tests/altair_mocks/line/layer_line_color_rule/
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/line/layer_line_color_rule/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.488220 vegafusion-1.6.8/tests/altair_mocks/line/multi_series/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/line/multi_series/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.488220 vegafusion-1.6.8/tests/altair_mocks/line/percent_axis/
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/line/percent_axis/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.488220 vegafusion-1.6.8/tests/altair_mocks/line/slope_graph/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/line/slope_graph/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.488220 vegafusion-1.6.8/tests/altair_mocks/line/slope_graph2/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/line/slope_graph2/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.488220 vegafusion-1.6.8/tests/altair_mocks/line/step_chart/
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/line/step_chart/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.488220 vegafusion-1.6.8/tests/altair_mocks/line/trail_marker/
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/line/trail_marker/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.488220 vegafusion-1.6.8/tests/altair_mocks/line/with_ci/
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/line/with_ci/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.488220 vegafusion-1.6.8/tests/altair_mocks/line/with_color_datum/
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/line/with_color_datum/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.488220 vegafusion-1.6.8/tests/altair_mocks/line/with_cumsum/
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/line/with_cumsum/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.488220 vegafusion-1.6.8/tests/altair_mocks/line/with_datum/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/line/with_datum/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.488220 vegafusion-1.6.8/tests/altair_mocks/line/with_generator/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/line/with_generator/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.488220 vegafusion-1.6.8/tests/altair_mocks/line/with_logarithmic_scale/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/line/with_logarithmic_scale/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.488220 vegafusion-1.6.8/tests/altair_mocks/line/with_points/
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/line/with_points/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.464219 vegafusion-1.6.8/tests/altair_mocks/maps/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.488220 vegafusion-1.6.8/tests/altair_mocks/maps/airports_count/
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/maps/airports_count/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.488220 vegafusion-1.6.8/tests/altair_mocks/maps/choropleth/
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/maps/choropleth/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.488220 vegafusion-1.6.8/tests/altair_mocks/maps/choropleth_repeat/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/maps/choropleth_repeat/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.488220 vegafusion-1.6.8/tests/altair_mocks/maps/us_incomebrackets_by_state_facet/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/maps/us_incomebrackets_by_state_facet/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.488220 vegafusion-1.6.8/tests/altair_mocks/maps/world/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/maps/world/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.488220 vegafusion-1.6.8/tests/altair_mocks/maps/world_projections/
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/maps/world_projections/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.468220 vegafusion-1.6.8/tests/altair_mocks/other/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.488220 vegafusion-1.6.8/tests/altair_mocks/other/bar_chart_with_highlighted_segment/
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/other/bar_chart_with_highlighted_segment/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.488220 vegafusion-1.6.8/tests/altair_mocks/other/beckers_barley_wrapped_facet/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/other/beckers_barley_wrapped_facet/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.488220 vegafusion-1.6.8/tests/altair_mocks/other/binned_heatmap/
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/other/binned_heatmap/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.488220 vegafusion-1.6.8/tests/altair_mocks/other/boxplot/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/other/boxplot/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.488220 vegafusion-1.6.8/tests/altair_mocks/other/candlestick_chart/
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/other/candlestick_chart/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/other/comet_chart/
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/other/comet_chart/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/other/errorbars_with_ci/
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/other/errorbars_with_ci/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/other/errorbars_with_std/
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/other/errorbars_with_std/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/other/gantt_chart/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/other/gantt_chart/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/other/hexbins/
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/other/hexbins/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/other/isotype_grid/
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/other/isotype_grid/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/other/layered_chart_with_dual_axis/
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/other/layered_chart_with_dual_axis/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/other/layered_heatmap_text/
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/other/layered_heatmap_text/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/other/multiple_marks/
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/other/multiple_marks/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/other/normed_parallel_coordinates/
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/other/normed_parallel_coordinates/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/other/parallel_coordinates/
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/other/parallel_coordinates/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/other/ranged_dot_plot/
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/other/ranged_dot_plot/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/other/ridgeline_plot/
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/other/ridgeline_plot/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/other/scatter_marginal_hist/
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/other/scatter_marginal_hist/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/other/sorted_error_bars_with_ci/
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/other/sorted_error_bars_with_ci/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/other/stem_and_leaf/
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/other/stem_and_leaf/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/other/violin_plot/
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/other/violin_plot/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/other/wilkinson_dot_plot/
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/other/wilkinson_dot_plot/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.468220 vegafusion-1.6.8/tests/altair_mocks/scatter/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/scatter/binned/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/scatter/binned/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/scatter/bubble_plot/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/scatter/bubble_plot/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/scatter/connected/
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/scatter/connected/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/scatter/dot_dash_plot/
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/scatter/dot_dash_plot/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/scatter/matrix/
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/scatter/matrix/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/scatter/multifeature/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/scatter/multifeature/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/scatter/poly_fit_regression/
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/scatter/poly_fit_regression/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/scatter/qq/
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/scatter/qq/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/scatter/stripplot/
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/scatter/stripplot/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/scatter/table_bubble_plot_github/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/scatter/table_bubble_plot_github/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/scatter/trellis/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/scatter/trellis/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/scatter/wind_vector_map/
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/scatter/wind_vector_map/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/scatter/with_errorbars/
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/scatter/with_errorbars/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.492220 vegafusion-1.6.8/tests/altair_mocks/scatter/with_labels/
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/scatter/with_labels/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.496220 vegafusion-1.6.8/tests/altair_mocks/scatter/with_lowess/
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/scatter/with_lowess/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.496220 vegafusion-1.6.8/tests/altair_mocks/scatter/with_rolling_mean/
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/scatter/with_rolling_mean/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.468220 vegafusion-1.6.8/tests/altair_mocks/simple/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.496220 vegafusion-1.6.8/tests/altair_mocks/simple/bar_chart/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/simple/bar_chart/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.496220 vegafusion-1.6.8/tests/altair_mocks/simple/heatmap/
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/simple/heatmap/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.496220 vegafusion-1.6.8/tests/altair_mocks/simple/line_chart/
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/simple/line_chart/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.496220 vegafusion-1.6.8/tests/altair_mocks/simple/scatter_tooltips/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/simple/scatter_tooltips/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.496220 vegafusion-1.6.8/tests/altair_mocks/simple/stacked_bar_chart/
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/simple/stacked_bar_chart/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.496220 vegafusion-1.6.8/tests/altair_mocks/simple/strip_chart/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/altair_mocks/simple/strip_chart/mock.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/test_conext_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/test_datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)    16868 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/test_input_utc.py
--rw-r--r--   0 runner    (1001) docker     (127)    50706 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/test_pretransform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/test_pretransform_specs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/test_row_limit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/test_save.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/test_sql_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    14052 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/test_transformed_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-07 14:03:06.000000 vegafusion-1.6.8/tests/test_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.496220 vegafusion-1.6.8/vegafusion/
--rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-05-07 14:03:06.000000 vegafusion-1.6.8/vegafusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-07 14:03:06.000000 vegafusion-1.6.8/vegafusion/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-07 14:03:06.000000 vegafusion-1.6.8/vegafusion/compilers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.496220 vegafusion-1.6.8/vegafusion/connection/
--rw-r--r--   0 runner    (1001) docker     (127)     5518 2024-05-07 14:03:06.000000 vegafusion-1.6.8/vegafusion/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13181 2024-05-07 14:03:06.000000 vegafusion-1.6.8/vegafusion/connection/duckdb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.500220 vegafusion-1.6.8/vegafusion/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-07 14:03:06.000000 vegafusion-1.6.8/vegafusion/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6071 2024-05-07 14:03:06.000000 vegafusion-1.6.8/vegafusion/dataset/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     5326 2024-05-07 14:03:06.000000 vegafusion-1.6.8/vegafusion/dataset/dfi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-07 14:03:06.000000 vegafusion-1.6.8/vegafusion/dataset/duckdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-07 14:03:06.000000 vegafusion-1.6.8/vegafusion/dataset/snowpark.py
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-07 14:03:06.000000 vegafusion-1.6.8/vegafusion/dataset/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.500220 vegafusion-1.6.8/vegafusion/datasource/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-07 14:03:06.000000 vegafusion-1.6.8/vegafusion/datasource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17414 2024-05-07 14:03:06.000000 vegafusion-1.6.8/vegafusion/datasource/_dfi_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-07 14:03:06.000000 vegafusion-1.6.8/vegafusion/datasource/datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-05-07 14:03:06.000000 vegafusion-1.6.8/vegafusion/datasource/dfi_datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-05-07 14:03:06.000000 vegafusion-1.6.8/vegafusion/datasource/pandas_datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-07 14:03:06.000000 vegafusion-1.6.8/vegafusion/datasource/pyarrow_datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-07 14:03:06.000000 vegafusion-1.6.8/vegafusion/embed.py
--rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-05-07 14:03:06.000000 vegafusion-1.6.8/vegafusion/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-07 14:03:06.000000 vegafusion-1.6.8/vegafusion/jupyter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-07 14:03:06.000000 vegafusion-1.6.8/vegafusion/local_tz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.500220 vegafusion-1.6.8/vegafusion/proto/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:06.000000 vegafusion-1.6.8/vegafusion/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    85200 2024-05-07 14:03:06.000000 vegafusion-1.6.8/vegafusion/proto/datafusion_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-05-07 14:03:06.000000 vegafusion-1.6.8/vegafusion/renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)    33884 2024-05-07 14:03:06.000000 vegafusion-1.6.8/vegafusion/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-05-07 14:03:06.000000 vegafusion-1.6.8/vegafusion/save.py
--rw-r--r--   0 runner    (1001) docker     (127)     8401 2024-05-07 14:03:06.000000 vegafusion-1.6.8/vegafusion/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-07 14:03:06.000000 vegafusion-1.6.8/vegafusion/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:03:45.500220 vegafusion-1.6.8/vegafusion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-07 14:03:45.000000 vegafusion-1.6.8/vegafusion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10742 2024-05-07 14:03:45.000000 vegafusion-1.6.8/vegafusion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 14:03:45.000000 vegafusion-1.6.8/vegafusion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-07 14:03:45.000000 vegafusion-1.6.8/vegafusion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-07 14:03:45.000000 vegafusion-1.6.8/vegafusion.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.334944 vegafusion-1.6.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-09 17:38:59.000000 vegafusion-1.6.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-09 17:39:41.334944 vegafusion-1.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-09 17:38:59.000000 vegafusion-1.6.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.298944 vegafusion-1.6.9/checks/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-09 17:38:59.000000 vegafusion-1.6.9/checks/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-09 17:38:59.000000 vegafusion-1.6.9/checks/check_lazy_imports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.298944 vegafusion-1.6.9/proto/
+-rw-r--r--   0 runner    (1001) docker     (127)    38178 2024-05-09 17:38:59.000000 vegafusion-1.6.9/proto/datafusion.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-09 17:38:59.000000 vegafusion-1.6.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-09 17:38:59.000000 vegafusion-1.6.9/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-09 17:39:41.334944 vegafusion-1.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 17:38:59.000000 vegafusion-1.6.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.302944 vegafusion-1.6.9/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.298944 vegafusion-1.6.9/tests/altair_mocks/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.282944 vegafusion-1.6.9/tests/altair_mocks/area/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.302944 vegafusion-1.6.9/tests/altair_mocks/area/cumulative_count/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/area/cumulative_count/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.302944 vegafusion-1.6.9/tests/altair_mocks/area/density_facet/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/area/density_facet/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.302944 vegafusion-1.6.9/tests/altair_mocks/area/density_stack/
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/area/density_stack/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.302944 vegafusion-1.6.9/tests/altair_mocks/area/gradient/
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/area/gradient/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.302944 vegafusion-1.6.9/tests/altair_mocks/area/horizon_graph/
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/area/horizon_graph/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.302944 vegafusion-1.6.9/tests/altair_mocks/area/layered/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/area/layered/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.302944 vegafusion-1.6.9/tests/altair_mocks/area/normalized_stacked/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/area/normalized_stacked/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.302944 vegafusion-1.6.9/tests/altair_mocks/area/streamgraph/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/area/streamgraph/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.302944 vegafusion-1.6.9/tests/altair_mocks/area/trellis/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/area/trellis/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.302944 vegafusion-1.6.9/tests/altair_mocks/area/trellis_sort_array/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/area/trellis_sort_array/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.286944 vegafusion-1.6.9/tests/altair_mocks/bar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.302944 vegafusion-1.6.9/tests/altair_mocks/bar/and_tick_chart/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/bar/and_tick_chart/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.302944 vegafusion-1.6.9/tests/altair_mocks/bar/diverging_stacked/
+-rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/bar/diverging_stacked/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.302944 vegafusion-1.6.9/tests/altair_mocks/bar/grouped/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/bar/grouped/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.302944 vegafusion-1.6.9/tests/altair_mocks/bar/horizontal/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/bar/horizontal/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.302944 vegafusion-1.6.9/tests/altair_mocks/bar/horizontal_grouped/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/bar/horizontal_grouped/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.302944 vegafusion-1.6.9/tests/altair_mocks/bar/horizontal_stacked/
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/bar/horizontal_stacked/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.302944 vegafusion-1.6.9/tests/altair_mocks/bar/layered/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/bar/layered/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.302944 vegafusion-1.6.9/tests/altair_mocks/bar/normalized_stacked/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/bar/normalized_stacked/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.306944 vegafusion-1.6.9/tests/altair_mocks/bar/percentage_of_total/
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/bar/percentage_of_total/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.306944 vegafusion-1.6.9/tests/altair_mocks/bar/sorted/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/bar/sorted/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.306944 vegafusion-1.6.9/tests/altair_mocks/bar/stacked/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/bar/stacked/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.306944 vegafusion-1.6.9/tests/altair_mocks/bar/stacked_with_sorted_segments/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/bar/stacked_with_sorted_segments/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.306944 vegafusion-1.6.9/tests/altair_mocks/bar/stacked_with_text_overlay/
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/bar/stacked_with_text_overlay/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.306944 vegafusion-1.6.9/tests/altair_mocks/bar/trellis_compact/
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/bar/trellis_compact/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.306944 vegafusion-1.6.9/tests/altair_mocks/bar/trellis_stacked/
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/bar/trellis_stacked/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.306944 vegafusion-1.6.9/tests/altair_mocks/bar/with_error_bars/
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/bar/with_error_bars/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.306944 vegafusion-1.6.9/tests/altair_mocks/bar/with_highlighted_bar/
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/bar/with_highlighted_bar/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.306944 vegafusion-1.6.9/tests/altair_mocks/bar/with_labels/
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/bar/with_labels/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.306944 vegafusion-1.6.9/tests/altair_mocks/bar/with_line_at_mean/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/bar/with_line_at_mean/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.306944 vegafusion-1.6.9/tests/altair_mocks/bar/with_line_on_dual_axis/
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/bar/with_line_on_dual_axis/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.306944 vegafusion-1.6.9/tests/altair_mocks/bar/with_negative_values/
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/bar/with_negative_values/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.306944 vegafusion-1.6.9/tests/altair_mocks/bar/with_rolling_mean/
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/bar/with_rolling_mean/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.306944 vegafusion-1.6.9/tests/altair_mocks/bar/with_rounded_edges/
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/bar/with_rounded_edges/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.286944 vegafusion-1.6.9/tests/altair_mocks/casestudy/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.306944 vegafusion-1.6.9/tests/altair_mocks/casestudy/airports/
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/casestudy/airports/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.306944 vegafusion-1.6.9/tests/altair_mocks/casestudy/anscombe_plot/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/casestudy/anscombe_plot/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.306944 vegafusion-1.6.9/tests/altair_mocks/casestudy/beckers_barley_trellis_plot/
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/casestudy/beckers_barley_trellis_plot/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.306944 vegafusion-1.6.9/tests/altair_mocks/casestudy/co2_concentration/
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/casestudy/co2_concentration/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.306944 vegafusion-1.6.9/tests/altair_mocks/casestudy/falkensee/
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/casestudy/falkensee/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.306944 vegafusion-1.6.9/tests/altair_mocks/casestudy/gapminder_bubble_plot/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/casestudy/gapminder_bubble_plot/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.306944 vegafusion-1.6.9/tests/altair_mocks/casestudy/iowa_electricity/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/casestudy/iowa_electricity/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.306944 vegafusion-1.6.9/tests/altair_mocks/casestudy/isotype/
+-rw-r--r--   0 runner    (1001) docker     (127)     5881 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/casestudy/isotype/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.306944 vegafusion-1.6.9/tests/altair_mocks/casestudy/isotype_emoji/
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/casestudy/isotype_emoji/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.306944 vegafusion-1.6.9/tests/altair_mocks/casestudy/london_tube/
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/casestudy/london_tube/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.306944 vegafusion-1.6.9/tests/altair_mocks/casestudy/natural_disasters/
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/casestudy/natural_disasters/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.306944 vegafusion-1.6.9/tests/altair_mocks/casestudy/one_dot_per_zipcode/
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/casestudy/one_dot_per_zipcode/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.306944 vegafusion-1.6.9/tests/altair_mocks/casestudy/top_k_items/
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/casestudy/top_k_items/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.310944 vegafusion-1.6.9/tests/altair_mocks/casestudy/top_k_letters/
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/casestudy/top_k_letters/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.310944 vegafusion-1.6.9/tests/altair_mocks/casestudy/top_k_with_others/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/casestudy/top_k_with_others/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.310944 vegafusion-1.6.9/tests/altair_mocks/casestudy/us_employment/
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/casestudy/us_employment/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.310944 vegafusion-1.6.9/tests/altair_mocks/casestudy/us_population_over_time_facet/
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/casestudy/us_population_over_time_facet/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.310944 vegafusion-1.6.9/tests/altair_mocks/casestudy/us_state_capitals/
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/casestudy/us_state_capitals/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.310944 vegafusion-1.6.9/tests/altair_mocks/casestudy/wheat_wages/
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/casestudy/wheat_wages/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.310944 vegafusion-1.6.9/tests/altair_mocks/casestudy/window_rank/
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/casestudy/window_rank/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.286944 vegafusion-1.6.9/tests/altair_mocks/circular/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.310944 vegafusion-1.6.9/tests/altair_mocks/circular/donut/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/circular/donut/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.310944 vegafusion-1.6.9/tests/altair_mocks/circular/pacman/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/circular/pacman/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.310944 vegafusion-1.6.9/tests/altair_mocks/circular/pie/
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/circular/pie/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.310944 vegafusion-1.6.9/tests/altair_mocks/circular/pie_with_labels/
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/circular/pie_with_labels/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.310944 vegafusion-1.6.9/tests/altair_mocks/circular/radial/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/circular/radial/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.286944 vegafusion-1.6.9/tests/altair_mocks/histogram/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.310944 vegafusion-1.6.9/tests/altair_mocks/histogram/layered/
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/histogram/layered/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.310944 vegafusion-1.6.9/tests/altair_mocks/histogram/trellis/
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/histogram/trellis/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.310944 vegafusion-1.6.9/tests/altair_mocks/histogram/with_a_global_mean_overlay/
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/histogram/with_a_global_mean_overlay/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.290944 vegafusion-1.6.9/tests/altair_mocks/interactive/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.310944 vegafusion-1.6.9/tests/altair_mocks/interactive/area-interval_selection/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/interactive/area-interval_selection/actions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/interactive/area-interval_selection/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.310944 vegafusion-1.6.9/tests/altair_mocks/interactive/brush/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/interactive/brush/actions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/interactive/brush/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.310944 vegafusion-1.6.9/tests/altair_mocks/interactive/casestudy-airport_connections/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/interactive/casestudy-airport_connections/actions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/interactive/casestudy-airport_connections/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.310944 vegafusion-1.6.9/tests/altair_mocks/interactive/casestudy-seattle_weather_interactive/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/interactive/casestudy-seattle_weather_interactive/actions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/interactive/casestudy-seattle_weather_interactive/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.310944 vegafusion-1.6.9/tests/altair_mocks/interactive/casestudy-us_population_over_time/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/interactive/casestudy-us_population_over_time/actions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/interactive/casestudy-us_population_over_time/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.310944 vegafusion-1.6.9/tests/altair_mocks/interactive/casestudy-us_population_pyramid_over_time/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/interactive/casestudy-us_population_pyramid_over_time/actions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/interactive/casestudy-us_population_pyramid_over_time/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.314944 vegafusion-1.6.9/tests/altair_mocks/interactive/casestudy-weather_heatmap/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/interactive/casestudy-weather_heatmap/actions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/interactive/casestudy-weather_heatmap/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.314944 vegafusion-1.6.9/tests/altair_mocks/interactive/cross_highlight/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/interactive/cross_highlight/actions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/interactive/cross_highlight/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.314944 vegafusion-1.6.9/tests/altair_mocks/interactive/histogram-responsive/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/interactive/histogram-responsive/actions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/interactive/histogram-responsive/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.314944 vegafusion-1.6.9/tests/altair_mocks/interactive/layered_crossfilter/
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/interactive/layered_crossfilter/actions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/interactive/layered_crossfilter/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.314944 vegafusion-1.6.9/tests/altair_mocks/interactive/legend/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/interactive/legend/actions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/interactive/legend/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.314944 vegafusion-1.6.9/tests/altair_mocks/interactive/multiline_highlight/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/interactive/multiline_highlight/actions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/interactive/multiline_highlight/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.314944 vegafusion-1.6.9/tests/altair_mocks/interactive/multiline_tooltip/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/interactive/multiline_tooltip/actions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/interactive/multiline_tooltip/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.314944 vegafusion-1.6.9/tests/altair_mocks/interactive/other-image_tooltip/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/interactive/other-image_tooltip/actions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/interactive/other-image_tooltip/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.314944 vegafusion-1.6.9/tests/altair_mocks/interactive/scatter-href/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/interactive/scatter-href/actions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/interactive/scatter-href/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.314944 vegafusion-1.6.9/tests/altair_mocks/interactive/scatter-with_linked_table/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/interactive/scatter-with_linked_table/actions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/interactive/scatter-with_linked_table/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.314944 vegafusion-1.6.9/tests/altair_mocks/interactive/scatter-with_minimap/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/interactive/scatter-with_minimap/actions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/interactive/scatter-with_minimap/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.314944 vegafusion-1.6.9/tests/altair_mocks/interactive/scatter_linked_brush/
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/interactive/scatter_linked_brush/actions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/interactive/scatter_linked_brush/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.314944 vegafusion-1.6.9/tests/altair_mocks/interactive/scatter_plot/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/interactive/scatter_plot/actions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/interactive/scatter_plot/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.314944 vegafusion-1.6.9/tests/altair_mocks/interactive/scatter_with_histogram/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/interactive/scatter_with_histogram/actions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/interactive/scatter_with_histogram/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.318944 vegafusion-1.6.9/tests/altair_mocks/interactive/scatter_with_layered_histogram/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/interactive/scatter_with_layered_histogram/actions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/interactive/scatter_with_layered_histogram/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.318944 vegafusion-1.6.9/tests/altair_mocks/interactive/select_detail/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/interactive/select_detail/actions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/interactive/select_detail/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.318944 vegafusion-1.6.9/tests/altair_mocks/interactive/select_mark_area/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/interactive/select_mark_area/actions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/interactive/select_mark_area/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.318944 vegafusion-1.6.9/tests/altair_mocks/interactive/selection_histogram/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/interactive/selection_histogram/actions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/interactive/selection_histogram/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.318944 vegafusion-1.6.9/tests/altair_mocks/interactive/selection_layer_bar_month/
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/interactive/selection_layer_bar_month/actions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/interactive/selection_layer_bar_month/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.290944 vegafusion-1.6.9/tests/altair_mocks/line/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.318944 vegafusion-1.6.9/tests/altair_mocks/line/bump_chart/
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/line/bump_chart/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.318944 vegafusion-1.6.9/tests/altair_mocks/line/filled_step_chart/
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/line/filled_step_chart/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.318944 vegafusion-1.6.9/tests/altair_mocks/line/layer_line_color_rule/
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/line/layer_line_color_rule/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.318944 vegafusion-1.6.9/tests/altair_mocks/line/multi_series/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/line/multi_series/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.318944 vegafusion-1.6.9/tests/altair_mocks/line/percent_axis/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/line/percent_axis/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.318944 vegafusion-1.6.9/tests/altair_mocks/line/slope_graph/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/line/slope_graph/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.318944 vegafusion-1.6.9/tests/altair_mocks/line/slope_graph2/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/line/slope_graph2/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.318944 vegafusion-1.6.9/tests/altair_mocks/line/step_chart/
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/line/step_chart/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.318944 vegafusion-1.6.9/tests/altair_mocks/line/trail_marker/
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/line/trail_marker/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.318944 vegafusion-1.6.9/tests/altair_mocks/line/with_ci/
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/line/with_ci/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.318944 vegafusion-1.6.9/tests/altair_mocks/line/with_color_datum/
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/line/with_color_datum/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.318944 vegafusion-1.6.9/tests/altair_mocks/line/with_cumsum/
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/line/with_cumsum/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.318944 vegafusion-1.6.9/tests/altair_mocks/line/with_datum/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/line/with_datum/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.318944 vegafusion-1.6.9/tests/altair_mocks/line/with_generator/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/line/with_generator/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.318944 vegafusion-1.6.9/tests/altair_mocks/line/with_logarithmic_scale/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/line/with_logarithmic_scale/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.318944 vegafusion-1.6.9/tests/altair_mocks/line/with_points/
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/line/with_points/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.294944 vegafusion-1.6.9/tests/altair_mocks/maps/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.318944 vegafusion-1.6.9/tests/altair_mocks/maps/airports_count/
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/maps/airports_count/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.318944 vegafusion-1.6.9/tests/altair_mocks/maps/choropleth/
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/maps/choropleth/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.318944 vegafusion-1.6.9/tests/altair_mocks/maps/choropleth_repeat/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/maps/choropleth_repeat/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.322944 vegafusion-1.6.9/tests/altair_mocks/maps/us_incomebrackets_by_state_facet/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/maps/us_incomebrackets_by_state_facet/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.322944 vegafusion-1.6.9/tests/altair_mocks/maps/world/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/maps/world/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.322944 vegafusion-1.6.9/tests/altair_mocks/maps/world_projections/
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/maps/world_projections/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.294944 vegafusion-1.6.9/tests/altair_mocks/other/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.322944 vegafusion-1.6.9/tests/altair_mocks/other/bar_chart_with_highlighted_segment/
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/other/bar_chart_with_highlighted_segment/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.322944 vegafusion-1.6.9/tests/altair_mocks/other/beckers_barley_wrapped_facet/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/other/beckers_barley_wrapped_facet/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.322944 vegafusion-1.6.9/tests/altair_mocks/other/binned_heatmap/
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/other/binned_heatmap/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.322944 vegafusion-1.6.9/tests/altair_mocks/other/boxplot/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/other/boxplot/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.322944 vegafusion-1.6.9/tests/altair_mocks/other/candlestick_chart/
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/other/candlestick_chart/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.322944 vegafusion-1.6.9/tests/altair_mocks/other/comet_chart/
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/other/comet_chart/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.322944 vegafusion-1.6.9/tests/altair_mocks/other/errorbars_with_ci/
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/other/errorbars_with_ci/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.322944 vegafusion-1.6.9/tests/altair_mocks/other/errorbars_with_std/
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/other/errorbars_with_std/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.322944 vegafusion-1.6.9/tests/altair_mocks/other/gantt_chart/
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/other/gantt_chart/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.322944 vegafusion-1.6.9/tests/altair_mocks/other/hexbins/
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/other/hexbins/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.322944 vegafusion-1.6.9/tests/altair_mocks/other/isotype_grid/
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/other/isotype_grid/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.322944 vegafusion-1.6.9/tests/altair_mocks/other/layered_chart_with_dual_axis/
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/other/layered_chart_with_dual_axis/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.322944 vegafusion-1.6.9/tests/altair_mocks/other/layered_heatmap_text/
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/other/layered_heatmap_text/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.322944 vegafusion-1.6.9/tests/altair_mocks/other/multiple_marks/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/other/multiple_marks/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.322944 vegafusion-1.6.9/tests/altair_mocks/other/normed_parallel_coordinates/
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/other/normed_parallel_coordinates/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.322944 vegafusion-1.6.9/tests/altair_mocks/other/parallel_coordinates/
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/other/parallel_coordinates/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.322944 vegafusion-1.6.9/tests/altair_mocks/other/ranged_dot_plot/
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/other/ranged_dot_plot/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.322944 vegafusion-1.6.9/tests/altair_mocks/other/ridgeline_plot/
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/other/ridgeline_plot/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.322944 vegafusion-1.6.9/tests/altair_mocks/other/scatter_marginal_hist/
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/other/scatter_marginal_hist/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.322944 vegafusion-1.6.9/tests/altair_mocks/other/sorted_error_bars_with_ci/
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/other/sorted_error_bars_with_ci/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.322944 vegafusion-1.6.9/tests/altair_mocks/other/stem_and_leaf/
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/other/stem_and_leaf/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.322944 vegafusion-1.6.9/tests/altair_mocks/other/violin_plot/
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/other/violin_plot/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.322944 vegafusion-1.6.9/tests/altair_mocks/other/wilkinson_dot_plot/
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/other/wilkinson_dot_plot/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.298944 vegafusion-1.6.9/tests/altair_mocks/scatter/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.322944 vegafusion-1.6.9/tests/altair_mocks/scatter/binned/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/scatter/binned/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.326944 vegafusion-1.6.9/tests/altair_mocks/scatter/bubble_plot/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/scatter/bubble_plot/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.326944 vegafusion-1.6.9/tests/altair_mocks/scatter/connected/
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/scatter/connected/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.326944 vegafusion-1.6.9/tests/altair_mocks/scatter/dot_dash_plot/
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/scatter/dot_dash_plot/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.326944 vegafusion-1.6.9/tests/altair_mocks/scatter/matrix/
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/scatter/matrix/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.326944 vegafusion-1.6.9/tests/altair_mocks/scatter/multifeature/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/scatter/multifeature/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.326944 vegafusion-1.6.9/tests/altair_mocks/scatter/poly_fit_regression/
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/scatter/poly_fit_regression/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.326944 vegafusion-1.6.9/tests/altair_mocks/scatter/qq/
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/scatter/qq/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.326944 vegafusion-1.6.9/tests/altair_mocks/scatter/stripplot/
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/scatter/stripplot/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.326944 vegafusion-1.6.9/tests/altair_mocks/scatter/table_bubble_plot_github/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/scatter/table_bubble_plot_github/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.326944 vegafusion-1.6.9/tests/altair_mocks/scatter/trellis/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/scatter/trellis/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.326944 vegafusion-1.6.9/tests/altair_mocks/scatter/wind_vector_map/
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/scatter/wind_vector_map/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.326944 vegafusion-1.6.9/tests/altair_mocks/scatter/with_errorbars/
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/scatter/with_errorbars/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.326944 vegafusion-1.6.9/tests/altair_mocks/scatter/with_labels/
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/scatter/with_labels/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.326944 vegafusion-1.6.9/tests/altair_mocks/scatter/with_lowess/
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/scatter/with_lowess/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.326944 vegafusion-1.6.9/tests/altair_mocks/scatter/with_rolling_mean/
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/scatter/with_rolling_mean/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.298944 vegafusion-1.6.9/tests/altair_mocks/simple/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.326944 vegafusion-1.6.9/tests/altair_mocks/simple/bar_chart/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/simple/bar_chart/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.326944 vegafusion-1.6.9/tests/altair_mocks/simple/heatmap/
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/simple/heatmap/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.326944 vegafusion-1.6.9/tests/altair_mocks/simple/line_chart/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/simple/line_chart/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.326944 vegafusion-1.6.9/tests/altair_mocks/simple/scatter_tooltips/
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/simple/scatter_tooltips/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.326944 vegafusion-1.6.9/tests/altair_mocks/simple/stacked_bar_chart/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/simple/stacked_bar_chart/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.326944 vegafusion-1.6.9/tests/altair_mocks/simple/strip_chart/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/altair_mocks/simple/strip_chart/mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/test_conext_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/test_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16868 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/test_input_utc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50706 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/test_pretransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/test_pretransform_specs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/test_row_limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/test_save.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/test_sql_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14052 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/test_transformed_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-09 17:38:59.000000 vegafusion-1.6.9/tests/test_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.330944 vegafusion-1.6.9/vegafusion/
+-rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-05-09 17:38:59.000000 vegafusion-1.6.9/vegafusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-09 17:38:59.000000 vegafusion-1.6.9/vegafusion/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.330944 vegafusion-1.6.9/vegafusion/connection/
+-rw-r--r--   0 runner    (1001) docker     (127)     5574 2024-05-09 17:38:59.000000 vegafusion-1.6.9/vegafusion/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13181 2024-05-09 17:38:59.000000 vegafusion-1.6.9/vegafusion/connection/duckdb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.330944 vegafusion-1.6.9/vegafusion/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-09 17:38:59.000000 vegafusion-1.6.9/vegafusion/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6139 2024-05-09 17:38:59.000000 vegafusion-1.6.9/vegafusion/dataset/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-05-09 17:38:59.000000 vegafusion-1.6.9/vegafusion/dataset/dfi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-09 17:38:59.000000 vegafusion-1.6.9/vegafusion/dataset/duckdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-09 17:38:59.000000 vegafusion-1.6.9/vegafusion/dataset/snowpark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-09 17:38:59.000000 vegafusion-1.6.9/vegafusion/dataset/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.330944 vegafusion-1.6.9/vegafusion/datasource/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-09 17:38:59.000000 vegafusion-1.6.9/vegafusion/datasource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17414 2024-05-09 17:38:59.000000 vegafusion-1.6.9/vegafusion/datasource/_dfi_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-09 17:38:59.000000 vegafusion-1.6.9/vegafusion/datasource/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-05-09 17:38:59.000000 vegafusion-1.6.9/vegafusion/datasource/dfi_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-05-09 17:38:59.000000 vegafusion-1.6.9/vegafusion/datasource/pandas_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-09 17:38:59.000000 vegafusion-1.6.9/vegafusion/datasource/pyarrow_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-09 17:38:59.000000 vegafusion-1.6.9/vegafusion/embed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-09 17:38:59.000000 vegafusion-1.6.9/vegafusion/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-09 17:38:59.000000 vegafusion-1.6.9/vegafusion/jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-09 17:38:59.000000 vegafusion-1.6.9/vegafusion/local_tz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.330944 vegafusion-1.6.9/vegafusion/proto/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 17:38:59.000000 vegafusion-1.6.9/vegafusion/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85200 2024-05-09 17:38:59.000000 vegafusion-1.6.9/vegafusion/proto/datafusion_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-05-09 17:38:59.000000 vegafusion-1.6.9/vegafusion/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34609 2024-05-09 17:38:59.000000 vegafusion-1.6.9/vegafusion/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-05-09 17:38:59.000000 vegafusion-1.6.9/vegafusion/save.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8638 2024-05-09 17:38:59.000000 vegafusion-1.6.9/vegafusion/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-09 17:38:59.000000 vegafusion-1.6.9/vegafusion/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:39:41.330944 vegafusion-1.6.9/vegafusion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-09 17:39:40.000000 vegafusion-1.6.9/vegafusion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10801 2024-05-09 17:39:41.000000 vegafusion-1.6.9/vegafusion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 17:39:40.000000 vegafusion-1.6.9/vegafusion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-09 17:39:40.000000 vegafusion-1.6.9/vegafusion.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-09 17:39:40.000000 vegafusion-1.6.9/vegafusion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-09 17:39:40.000000 vegafusion-1.6.9/vegafusion.egg-info/top_level.txt
```

### Comparing `vegafusion-1.6.8/LICENSE.txt` & `vegafusion-1.6.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/PKG-INFO` & `vegafusion-1.6.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: vegafusion
-Version: 1.6.8
+Version: 1.6.9
 Summary: Core tools for using VegaFusion from Python
 License: BSD-3-Clause
 Keywords: vega,altair,vegafusion,arrow
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Requires-Dist: altair>=4.2.0
+Requires-Dist: altair>=5.2.0
 Requires-Dist: pyarrow>=5
 Requires-Dist: pandas
 Requires-Dist: psutil
 Requires-Dist: protobuf
 Provides-Extra: embed
-Requires-Dist: vegafusion-python-embed==1.6.8; extra == "embed"
+Requires-Dist: vegafusion-python-embed==1.6.9; extra == "embed"
 Requires-Dist: vl-convert-python>=0.7.0; extra == "embed"
 
 ## VegaFusion
 This package is part of the VegaFusion project: https://vegafusion.io.
 
 In particular, the `vegafusion` package provides a pure Python interface to a VegaFusion Runtime. Initially, the only runtime available is provided by the `vegafusion-python-embed` package. Eventually, the VegaFusion runtime will be available as a standalone gRPC server and this package will be updated to support communication with a VegaFusion Runtime over gRPC as an alternative to the Runtime provided by `vegafusion-python-embed`.
```

### Comparing `vegafusion-1.6.8/README.md` & `vegafusion-1.6.9/README.md`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/proto/datafusion.proto` & `vegafusion-1.6.9/proto/datafusion.proto`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/area/density_facet/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/area/density_facet/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/area/density_stack/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/area/density_stack/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/area/gradient/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/area/gradient/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/area/horizon_graph/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/area/horizon_graph/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/bar/and_tick_chart/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/bar/and_tick_chart/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/bar/diverging_stacked/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/bar/diverging_stacked/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/bar/stacked_with_text_overlay/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/bar/stacked_with_text_overlay/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/bar/trellis_compact/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/bar/trellis_compact/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/bar/with_highlighted_bar/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/bar/with_highlighted_bar/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/bar/with_rolling_mean/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/bar/with_rolling_mean/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/casestudy/airports/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/casestudy/airports/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/casestudy/beckers_barley_trellis_plot/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/casestudy/beckers_barley_trellis_plot/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/casestudy/co2_concentration/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/casestudy/co2_concentration/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/casestudy/falkensee/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/casestudy/falkensee/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/casestudy/iowa_electricity/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/casestudy/iowa_electricity/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/casestudy/isotype/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/casestudy/isotype/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/casestudy/isotype_emoji/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/casestudy/isotype_emoji/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/casestudy/london_tube/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/casestudy/london_tube/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/casestudy/natural_disasters/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/casestudy/natural_disasters/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/casestudy/one_dot_per_zipcode/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/casestudy/one_dot_per_zipcode/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/casestudy/top_k_items/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/casestudy/top_k_items/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/casestudy/top_k_letters/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/casestudy/top_k_letters/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/casestudy/top_k_with_others/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/casestudy/top_k_with_others/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/casestudy/us_employment/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/casestudy/us_employment/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/casestudy/us_state_capitals/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/casestudy/us_state_capitals/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/casestudy/wheat_wages/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/casestudy/wheat_wages/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/casestudy/window_rank/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/casestudy/window_rank/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/histogram/layered/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/histogram/layered/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/interactive/casestudy-airport_connections/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/interactive/casestudy-airport_connections/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/interactive/casestudy-seattle_weather_interactive/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/interactive/casestudy-seattle_weather_interactive/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/interactive/casestudy-us_population_over_time/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/interactive/casestudy-us_population_over_time/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/interactive/casestudy-us_population_pyramid_over_time/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/interactive/casestudy-us_population_pyramid_over_time/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/interactive/casestudy-weather_heatmap/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/interactive/casestudy-weather_heatmap/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/interactive/cross_highlight/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/interactive/cross_highlight/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/interactive/histogram-responsive/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/interactive/histogram-responsive/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/interactive/layered_crossfilter/actions.json` & `vegafusion-1.6.9/tests/altair_mocks/interactive/layered_crossfilter/actions.json`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/interactive/layered_crossfilter/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/interactive/layered_crossfilter/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/interactive/legend/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/interactive/legend/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/interactive/multiline_highlight/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/interactive/multiline_highlight/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/interactive/multiline_tooltip/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/interactive/multiline_tooltip/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/interactive/scatter-with_linked_table/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/interactive/scatter-with_linked_table/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/interactive/scatter-with_minimap/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/interactive/scatter-with_minimap/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/interactive/scatter_with_histogram/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/interactive/scatter_with_histogram/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/interactive/scatter_with_layered_histogram/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/interactive/scatter_with_layered_histogram/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/interactive/select_detail/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/interactive/select_detail/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/interactive/selection_layer_bar_month/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/interactive/selection_layer_bar_month/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/line/bump_chart/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/line/bump_chart/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/line/with_cumsum/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/line/with_cumsum/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/line/with_datum/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/line/with_datum/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/maps/airports_count/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/maps/airports_count/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/maps/choropleth_repeat/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/maps/choropleth_repeat/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/maps/us_incomebrackets_by_state_facet/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/maps/us_incomebrackets_by_state_facet/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/maps/world/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/maps/world/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/other/bar_chart_with_highlighted_segment/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/other/bar_chart_with_highlighted_segment/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/other/candlestick_chart/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/other/candlestick_chart/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/other/comet_chart/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/other/comet_chart/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/other/errorbars_with_ci/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/other/errorbars_with_ci/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/other/hexbins/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/other/hexbins/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/other/isotype_grid/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/other/isotype_grid/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/other/layered_chart_with_dual_axis/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/other/layered_chart_with_dual_axis/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/other/layered_heatmap_text/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/other/layered_heatmap_text/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/other/normed_parallel_coordinates/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/other/normed_parallel_coordinates/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/other/ranged_dot_plot/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/other/ranged_dot_plot/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/other/ridgeline_plot/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/other/ridgeline_plot/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/other/scatter_marginal_hist/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/other/scatter_marginal_hist/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/other/sorted_error_bars_with_ci/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/other/sorted_error_bars_with_ci/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/other/stem_and_leaf/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/other/stem_and_leaf/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/other/violin_plot/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/other/violin_plot/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/scatter/dot_dash_plot/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/scatter/dot_dash_plot/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/scatter/poly_fit_regression/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/scatter/poly_fit_regression/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/scatter/stripplot/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/scatter/stripplot/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/scatter/wind_vector_map/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/scatter/wind_vector_map/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/scatter/with_errorbars/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/scatter/with_errorbars/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/scatter/with_lowess/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/scatter/with_lowess/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/altair_mocks/scatter/with_rolling_mean/mock.py` & `vegafusion-1.6.9/tests/altair_mocks/scatter/with_rolling_mean/mock.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/test_conext_manager.py` & `vegafusion-1.6.9/tests/test_conext_manager.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/test_datasource.py` & `vegafusion-1.6.9/tests/test_datasource.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/test_input_utc.py` & `vegafusion-1.6.9/tests/test_input_utc.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/test_pretransform.py` & `vegafusion-1.6.9/tests/test_pretransform.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/test_pretransform_specs.py` & `vegafusion-1.6.9/tests/test_pretransform_specs.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/test_row_limit.py` & `vegafusion-1.6.9/tests/test_row_limit.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/test_save.py` & `vegafusion-1.6.9/tests/test_save.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/test_transformed_data.py` & `vegafusion-1.6.9/tests/test_transformed_data.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/tests/test_transformer.py` & `vegafusion-1.6.9/tests/test_transformer.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/vegafusion/__init__.py` & `vegafusion-1.6.9/vegafusion/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from .runtime import runtime
 from .transformer import to_feather, get_inline_datasets_for_spec
 from .renderer import RowLimitError
 from .local_tz import set_local_tz, get_local_tz
 from .evaluation import transformed_data
 from .save import save_html, save_vega, save_png, save_svg
 from . import renderer
-from .compilers import vegalite_compilers
-import altair as alt
+
 
 from ._version import __version__
 from .utils import RendererTransformerEnabler
 
 # Import optional subpackages
 try:
     import vegafusion.jupyter
@@ -55,14 +54,15 @@
     :param row_limit: Maximum number of rows (after transforms are applied) that may be
         included in the Vega specifications that will be displayed. An error will
         be raised if the limit is exceeded. None for unlimited.
     :param embed_options: dict (optional)
         Dictionary of options to pass to the vega-embed. Default
         entry is {'mode': 'vega'}.
     """
+    import altair as alt
     embed_options = embed_options if embed_options is not None else {}
     return RendererTransformerEnabler(
         renderer_ctx=alt.renderers.enable(
             'vegafusion-mime', mimetype=mimetype, row_limit=row_limit, embed_options=embed_options
         ),
         data_transformer_ctx=alt.data_transformers.enable('vegafusion-inline'),
         repr_str=(
@@ -111,12 +111,13 @@
     import altair as alt
     alt.renderers.enable('default')
     alt.data_transformers.enable('default')
     ```
 
     This does not affect the behavior of VegaFusionWidget
     """
+    import altair as alt
     return RendererTransformerEnabler(
         renderer_ctx=alt.renderers.enable('default'),
         data_transformer_ctx=alt.data_transformers.enable('default'),
         repr_str="vegafusion.disable()"
     )
```

### Comparing `vegafusion-1.6.8/vegafusion/connection/__init__.py` & `vegafusion-1.6.9/vegafusion/connection/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from typing import Dict, Optional
-
-import pandas as pd
-import pyarrow as pa
-
+from typing import Dict, Optional, TYPE_CHECKING
 from dataclasses import dataclass
 from abc import ABC, abstractmethod
 
+if TYPE_CHECKING:
+    from pyarrow import Schema, Table
+    from pandas import DataFrame
+
 
 @dataclass
 class CsvReadOptions:
     """
     CSV Read configuration options
     """
     has_header: bool
     delimeter: str
     file_extension: str
-    schema: Optional[pa.Schema]
+    schema: Optional["Schema"]
 
 
 class RegistrationNotSupportedError(RuntimeError):
     pass
 
 
 class SqlConnection(ABC):
@@ -42,26 +42,26 @@
          - "postgres"
          - "redshift"
          - "snowflake"
         """
         raise NotImplementedError()
 
     @abstractmethod
-    def tables(self) -> Dict[str, pa.Schema]:
+    def tables(self) -> Dict[str, "Schema"]:
         """
         Returns the names and schema for the tables that are provided by the connection.
         These are the tables that may be referenced by SQL queries passed to the
         fetch_query method
 
         :return: dict from table name to pa.Schema
         """
         raise NotImplementedError()
 
     @abstractmethod
-    def fetch_query(self, query: str, schema: pa.Schema) -> pa.Table:
+    def fetch_query(self, query: str, schema: "Schema") -> "Table":
         """
         Returns the result of evaluating the requested query. The resulting pa.Table
         should have a schema matching the provided schema
 
         :param query: SQL query string
         :param schema: expected pyarrow Schema of resulting pyarrow Table
         :return: pyarrow Table with query results
@@ -73,26 +73,26 @@
         Whether VegaFusion should fall back to the built-in DataFusion connection
         when SQL is encountered that is not supported by this connection's SQL dialect
 
         :return: bool
         """
         return True
 
-    def register_pandas(self, name: str, df: pd.DataFrame, temporary: bool = False):
+    def register_pandas(self, name: str, df: "DataFrame", temporary: bool = False):
         """
         Register the provided pandas DataFrame as a table with the provided name
 
         :param name: Table name
         :param df: pandas DataFrame
         :param temporary: Whether table is considered temporary,
             and should be removed by unregister_temporary_tables
         """
         raise RegistrationNotSupportedError("Connection does not support registration of pandas datasets")
 
-    def register_arrow(self, name: str, table: pa.Table, temporary: bool = False):
+    def register_arrow(self, name: str, table: "Table", temporary: bool = False):
         """
         Register the provided pyarrow Table as a table with the provided name
         :param name: Table name
         :param table: pyarrow Table
         :param temporary: Whether table is considered temporary,
             and should be removed by unregister_temporary_tables
         """
```

### Comparing `vegafusion-1.6.8/vegafusion/connection/duckdb.py` & `vegafusion-1.6.9/vegafusion/connection/duckdb.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/vegafusion/dataset/dataframe.py` & `vegafusion-1.6.9/vegafusion/dataset/dataframe.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from abc import ABC, abstractmethod
-import pyarrow as pa
-from vegafusion.proto.datafusion_pb2 import LogicalExprNode
+from typing import Optional, List, Literal, Union, Any, TYPE_CHECKING
 
-from typing import Optional, List, Literal, Union, Any
+if TYPE_CHECKING:
+    from pyarrow import Schema, Table
+    from vegafusion.proto.datafusion_pb2 import LogicalExprNode
 
 
 class DataFrameOperationNotSupportedError(RuntimeError):
     """
     Exception raised when a DataFrame transform method is not
     supported
     """
@@ -15,20 +16,20 @@
 
 class DataFrameDataset(ABC):
     """
     Python interface for VegaFusion DataFrame
     """
 
     @abstractmethod
-    def schema(self) -> pa.Schema:
+    def schema(self) -> "Schema":
         """DataFrame's pyarrow schema"""
         raise NotImplementedError()
 
     @abstractmethod
-    def collect(self) -> pa.Table:
+    def collect(self) -> "Table":
         """Return DataFrame's value as a pyarrow Table"""
         raise NotImplementedError()
 
     def fallback(self) -> bool:
         """
         Whether VegaFusion should fall back to the built-in DataFusion connection
         when DataFrame operations are encountered that are not supported
@@ -43,63 +44,63 @@
         This blocks multithreaded parallelization, but is sometimes required
 
         :return: bool
         """
         return True
 
     def sort(
-        self, exprs: List[LogicalExprNode], limit: Optional[int]
+        self, exprs: List["LogicalExprNode"], limit: Optional[int]
     ) -> "DataFrameDataset":
         """
         Sort and optionally limit dataset
 
         :param exprs: Sort expressions
         :param limit: Max number of rows to return
         :return: DataFrameDataset
         """
         raise DataFrameOperationNotSupportedError()
 
-    def select(self, exprs: List[LogicalExprNode]) -> "DataFrameDataset":
+    def select(self, exprs: List["LogicalExprNode"]) -> "DataFrameDataset":
         """
         Select columns from Dataset. Selection expressions may include column names,
         column expressions, or window expressions
 
         :param exprs: Selection expressions
         :return: DataFrameDataset
         """
         raise DataFrameOperationNotSupportedError()
 
     def aggregate(
-        self, group_exprs: List[LogicalExprNode], agg_exprs: List[LogicalExprNode]
+        self, group_exprs: List["LogicalExprNode"], agg_exprs: List["LogicalExprNode"]
     ) -> "DataFrameDataset":
         """
         Perform dataset aggregation. Resulting dataset includes grouping
         columns and aggregate expressions
 
         :param group_exprs: Expressions to group by
         :param agg_exprs: Aggregate expressions
         :return: DataFrameDataset
         """
         raise DataFrameOperationNotSupportedError()
 
     def joinaggregate(
-        self, group_exprs: List[LogicalExprNode], agg_exprs: List[LogicalExprNode]
+        self, group_exprs: List["LogicalExprNode"], agg_exprs: List["LogicalExprNode"]
     ) -> "DataFrameDataset":
         """
         Perform joinaggregate dataset operation.
 
         See: https://vega.github.io/vega/docs/transforms/joinaggregate/
 
         :param group_exprs: Expressions to group by
         :param agg_exprs: Aggregate expressions
         :return: DataFrameDataset
         """
         raise DataFrameOperationNotSupportedError()
 
-    def filter(self, predicate: LogicalExprNode) -> "DataFrameDataset":
+    def filter(self, predicate: "LogicalExprNode") -> "DataFrameDataset":
         """
         Filter dataset by predicate expression
 
         :param predicate: Predicate expression
         :return: DataFrameDataset
         """
         raise DataFrameOperationNotSupportedError()
@@ -131,15 +132,15 @@
         :return: DataFrameDataset
         """
         raise DataFrameOperationNotSupportedError()
 
     def stack(
         self,
         field: str,
-        orderby: List[LogicalExprNode],
+        orderby: List["LogicalExprNode"],
         groupby: List[str],
         start_field: str,
         stop_field: str,
         mode: Literal["zero", "center", "normalize"],
     ) -> "DataFrameDataset":
         """
         Computes a layout of stacking groups of values
```

### Comparing `vegafusion-1.6.8/vegafusion/dataset/dfi.py` & `vegafusion-1.6.9/vegafusion/dataset/dfi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-import pyarrow as pa
 from functools import cached_property
-from typing import Sequence, Optional
+from typing import Sequence, Optional, TYPE_CHECKING
 from .sql import SqlDataset
 
+if TYPE_CHECKING:
+    from pyarrow import Table, Schema
 
 class SqlDatasetDataFrame:
     """An implementation of the dataframe interchange protocol.
     Based on https://github.com/ibis-project/ibis/pull/6733
 
     This is a thin shim around the pyarrow implementation to allow for:
      - Accessing a few of the metadata queries without executing the expression.
@@ -18,15 +19,15 @@
     """
 
     def __init__(
         self,
         dataset: SqlDataset,
         nan_as_null: bool = False,
         allow_copy: bool = True,
-        pyarrow_table: Optional[pa.Table] = None,
+        pyarrow_table: Optional["Table"] = None,
     ):
         self._dataset = dataset
         self._nan_as_null = nan_as_null
         self._allow_copy = allow_copy
         self._pyarrow_table = pyarrow_table
 
     @cached_property
@@ -51,15 +52,15 @@
         Used for returning dtype information without executing the backing ibis
         expression.
         """
         schema = self._schema
         return schema.empty_table().__dataframe__()
 
     @property
-    def _schema(self) -> pa.Schema:
+    def _schema(self) -> "Schema":
         return self._dataset.table_schema()
 
     def _get_dtype(self, name):
         """Get the dtype info for a column named `name`."""
         return self._empty_pyarrow_df.get_column_by_name(name).dtype
 
     # These methods may all be handled without executing the query
```

### Comparing `vegafusion-1.6.8/vegafusion/dataset/duckdb.py` & `vegafusion-1.6.9/vegafusion/dataset/duckdb.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/vegafusion/dataset/snowpark.py` & `vegafusion-1.6.9/vegafusion/dataset/snowpark.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/vegafusion/dataset/sql.py` & `vegafusion-1.6.9/vegafusion/dataset/sql.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from abc import ABC, abstractmethod
-import pyarrow as pa
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from .dfi import SqlDatasetDataFrame
+    import pyarrow as pa
 
 
 class SqlDataset(ABC):
     """
     Python interface for VegaFusion Sql Dataset
     """
 
@@ -31,20 +31,20 @@
 
     @abstractmethod
     def table_name(self) -> str:
         """Name of source table for use in queries"""
         raise NotImplementedError()
 
     @abstractmethod
-    def table_schema(self) -> pa.Schema:
+    def table_schema(self) -> "pa.Schema":
         """Schema of source table"""
         raise NotImplementedError()
 
     @abstractmethod
-    def fetch_query(self, query: str, schema: pa.Schema) -> pa.Table:
+    def fetch_query(self, query: str, schema: "pa.Schema") -> "pa.Table":
         """
         Returns the result of evaluating the requested query. The resulting pa.Table
         should have a schema matching the provided schema
 
         :param query: SQL query string
         :param schema: expected pyarrow Schema of resulting pyarrow Table
         :return: pyarrow Table with query results
```

### Comparing `vegafusion-1.6.8/vegafusion/datasource/_dfi_types.py` & `vegafusion-1.6.9/vegafusion/datasource/_dfi_types.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/vegafusion/datasource/dfi_datasource.py` & `vegafusion-1.6.9/vegafusion/datasource/pandas_datasource.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,85 +1,89 @@
-from typing import Iterable
-import re
-import pyarrow as pa
-
-from typing import Any, Dict
-from ._dfi_types import DtypeKind, DataFrame as DfiDataFrame
+from typing import Iterable, TYPE_CHECKING
+from math import floor
 from .datasource import Datasource
 
-# Taken from private pyarrow utilities
-_PYARROW_DTYPES: Dict[DtypeKind, Dict[int, Any]] = {
-    DtypeKind.INT: {8: pa.int8(),
-                    16: pa.int16(),
-                    32: pa.int32(),
-                    64: pa.int64()},
-    DtypeKind.UINT: {8: pa.uint8(),
-                     16: pa.uint16(),
-                     32: pa.uint32(),
-                     64: pa.uint64()},
-    DtypeKind.FLOAT: {16: pa.float16(),
-                      32: pa.float32(),
-                      64: pa.float64()},
-    DtypeKind.BOOL: {1: pa.bool_(),
-                     8: pa.uint8()},
-    DtypeKind.STRING: {8: pa.string()},
-}
-
-
-def parse_datetime_format_str(format_str):
-    """Parse datetime `format_str` to interpret the `data`."""
-
-    # timestamp 'ts{unit}:tz'
-    timestamp_meta = re.match(r"ts([smun]):(.*)", format_str)
-    if timestamp_meta:
-        unit, tz = timestamp_meta.group(1), timestamp_meta.group(2)
-        if unit != "s":
-            # the format string describes only a first letter of the unit, so
-            # add one extra letter to convert the unit to numpy-style:
-            # 'm' -> 'ms', 'u' -> 'us', 'n' -> 'ns'
-            unit += "s"
-
-        return unit, tz
-
-    raise NotImplementedError(f"DateTime kind is not supported: {format_str}")
-
-
-def map_date_type(data_type):
-    """Map column date type to pyarrow date type. """
-    kind, bit_width, f_string, _ = data_type
-
-    if kind == DtypeKind.DATETIME:
-        unit, tz = parse_datetime_format_str(f_string)
-        return pa.timestamp(unit, tz=tz)
-    else:
-        pa_dtype = _PYARROW_DTYPES.get(kind, {}).get(bit_width, None)
-
-        # Error if dtype is not supported
-        if pa_dtype:
-            return pa_dtype
-        else:
-            raise NotImplementedError(
-                f"Conversion for {data_type} is not yet supported.")
+if TYPE_CHECKING:
+    import pandas as pd
+    import pyarrow as pa
 
 
-class DfiDatasource(Datasource):
-    def __init__(self, dataframe: DfiDataFrame):
-        if hasattr(dataframe, "__dataframe__"):
-            dataframe = dataframe.__dataframe__()
+class PandasDatasource(Datasource):
+    def __init__(self, df: "pd.DataFrame", sample_size: int = 1000, batch_size: int = 8096):
+        import pandas as pd
+        import pyarrow as pa
+
         fields = []
-        for col in dataframe.column_names():
-            field = dataframe.get_column_by_name(col)
-            pa_type = map_date_type(field.dtype)
-            fields.append(pa.field(col, pa_type))
+        casts = {}
+        sample_stride = max(1, floor(len(df) / sample_size))
 
-        self._dataframe = dataframe
+        # Shallow copy and add named index levels as columns
+        # (this is faster that df.reset_index, which seems to perform a deep copy)
+        df = df.copy(deep=False)
+        for i, index_name in enumerate(getattr(df.index, "names", [])):
+            if isinstance(index_name, str):
+                df[index_name] = df.index.get_level_values(i)
+        df.reset_index(drop=True, inplace=True)
+
+        for col, pd_type in df.dtypes.items():
+            if not isinstance(col, str):
+                continue
+            try:
+                try:
+                    # We will expand categoricals (not yet supported in VegaFusion)
+                    if isinstance(pd_type, pd.CategoricalDtype):
+                        cat = df[col].cat
+                        field = pa.Schema.from_pandas(pd.DataFrame({col: cat.categories})).field(col)
+                    else:
+                        candidate_schema = pa.Schema.from_pandas(df.iloc[::sample_stride][[col]])
+                        field = candidate_schema.field(col)
+                except (pa.ArrowTypeError, pa.ArrowInvalid):
+                    # If arrow fails to infer the type, fall back to string
+                    casts[col] = "str"
+                    field = pa.field(col, pa.string())
+
+                # Convert Decimal columns to float
+                if isinstance(field.type, (pa.Decimal128Type, pa.Decimal256Type)):
+                    field = pa.field(col, pa.float64())
+                    casts[col] = "float64"
+
+                # Get inferred pyarrow type
+                fields.append(field)
+
+            except pa.ArrowTypeError:
+                if pd_type.kind == "O":
+                    fields.append(pa.field(col, pa.string()))
+                    casts[col] = str
+                else:
+                    raise
+        self._df = df
         self._schema = pa.schema(fields)
+        self._casts = casts
+        self._batch_size = batch_size
 
-    def schema(self) -> pa.Schema:
+    def schema(self) -> "pa.Schema":
         return self._schema
 
-    def fetch(self, columns: Iterable[str]) -> pa.Table:
-        from pyarrow.interchange import from_dataframe
-        columns = list(columns)
-        projected_schema = pa.schema([f for f in self._schema if f.name in columns])
-        table = from_dataframe(self._dataframe.select_columns_by_name(columns))
-        return table.cast(projected_schema, safe=False)
+    def fetch(self, columns: Iterable[str]) -> "pa.Table":
+        import pandas as pd
+        import pyarrow as pa
+        projected = self._df[columns].copy(deep=False)
+
+        for col, pd_type in projected.dtypes.items():
+            # Handle cases that need to happen before conversion to pyarrow
+            if col in self._casts:
+                projected[col] = projected[col].astype(self._casts[col])
+
+            # Handle expanding categoricals
+            if isinstance(pd_type, pd.CategoricalDtype):
+                cat = projected[col].cat
+                projected[col] = cat.categories[cat.codes]
+
+        table = pa.Table.from_pandas(projected, preserve_index=False)
+
+        # Split into batches of desired size
+        if self._batch_size is None:
+            return table
+        else:
+            # Resize batches
+            batches = table.to_batches(self._batch_size)
+            return pa.Table.from_batches(batches, table.schema)
```

### Comparing `vegafusion-1.6.8/vegafusion/local_tz.py` & `vegafusion-1.6.9/vegafusion/local_tz.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/vegafusion/proto/datafusion_pb2.py` & `vegafusion-1.6.9/vegafusion/proto/datafusion_pb2.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/vegafusion/renderer.py` & `vegafusion-1.6.9/vegafusion/renderer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 from uuid import uuid4
-import altair as alt
-from altair.utils.html import spec_to_html
-
 
 class RowLimitError(ValueError):
     def __init__(self, row_limit):
         self.row_limit = row_limit
 
     def __str__(self):
         return (
@@ -29,15 +26,16 @@
         mimetype="html",
         row_limit=None,
         embed_options=None,
         html_template="universal",
         full_html=False,
         scale=1,
 ):
-    from . import transformer, runtime, local_tz, vegalite_compilers, altair_vl_version
+    from altair import vegalite_compilers
+    from . import transformer, runtime, local_tz, altair_vl_version
     vega_spec = vegalite_compilers.get()(spec)
 
     inline_datasets = transformer.get_inline_datasets_for_spec(vega_spec)
     tx_vega_spec, warnings = runtime.pre_transform_spec(
         vega_spec,
         local_tz.get_local_tz(),
         row_limit=row_limit,
@@ -55,14 +53,15 @@
     if mimetype == "vega":
         vega_mimetype = "application/vnd.vega.v5+json"
         return (
             {vega_mimetype: tx_vega_spec},
             {vega_mimetype: {"embed_options": embed_options}}
         )
     elif mimetype == "html":
+        from altair.utils.html import spec_to_html
         output_div = f"altair-viz-{uuid4().hex}"
         html = spec_to_html(
             tx_vega_spec,
             mode="vega",
             vega_version="5",
             vegalite_version=altair_vl_version(),
             vegaembed_version="6",
@@ -78,10 +77,7 @@
         return {"image/svg+xml": svg}
     elif mimetype == "png":
         import vl_convert as vlc
         png = vlc.vega_to_png(tx_vega_spec, scale=scale)
         return {"image/png": png}
     else:
         raise ValueError(f"Unsupported mimetype: {mimetype}")
-
-
-alt.renderers.register('vegafusion-mime', vegafusion_mime_renderer)
```

### Comparing `vegafusion-1.6.8/vegafusion/runtime.py` & `vegafusion-1.6.9/vegafusion/runtime.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,19 @@
-import pandas as pd
+import sys
+from typing import TypedDict, List, Literal, Any, Union, TYPE_CHECKING
+
 import psutil
-import pyarrow as pa
-from typing import Union
+
 from .connection import SqlConnection
 from .dataset import SqlDataset, DataFrameDataset
 from .datasource import PandasDatasource, DfiDatasource, PyArrowDatasource
-from .evaluation import get_mark_group_for_scope
-from .transformer import import_pyarrow_interchange, to_arrow_table
 from .local_tz import get_local_tz
 
-try:
+if TYPE_CHECKING:
     from duckdb import DuckDBPyConnection
-except ImportError:
-    DuckDBPyConnection = None
-
-try:
-    import polars as pl
-except ImportError:
-    pl = None
-
-from typing import TypedDict, List, Literal, Any
-
 
 def _all_datasets_have_type(inline_datasets, types):
     if not inline_datasets:
         # If there are no inline datasets, return false
         # (we want the default pandas behavior in this case)
         return False
     else:
@@ -126,15 +115,15 @@
             # Try to initialize an embedded runtime
             from vegafusion_embed import PyVegaFusionRuntime
             self._embedded_runtime = PyVegaFusionRuntime(
                 self.cache_capacity, self.memory_limit, self.worker_threads, connection=self._connection
             )
         return self._embedded_runtime
 
-    def set_connection(self, connection: Union[str, SqlConnection, DuckDBPyConnection] = "datafusion"):
+    def set_connection(self, connection: Union[str, SqlConnection, "DuckDBPyConnection"] = "datafusion"):
         """
         Sets the connection to use to evaluate Vega data transformations.
 
         Named tables returned by the connection's `tables` method may be referenced in Vega/Altair
         chart specifications using special dataset URLs. For example, if the connection's `tables`
         method returns a dictionary that includes "tableA" as a key, then this table may be
         referenced in a chart specification using the URL "table://tableA" or
@@ -143,24 +132,27 @@
         :param connection: One of:
           - An instance of vegafusion.connection.SqlConnection
           - An instance of a duckdb connection
           - A string, one of:
                 - "datafusion" (default)
                 - "duckdb"
         """
+        # Don't import duckdb unless it's already loaded. If it's not loaded,
+        # then the input connection can't be a duckdb connection.
+        duckdb = sys.modules.get("duckdb", None)
         if isinstance(connection, str):
             if connection == "datafusion":
                 # Connection of None uses DataFusion
                 connection = None
             elif connection == "duckdb":
                 from vegafusion.connection.duckdb import DuckDbConnection
                 connection = DuckDbConnection()
             else:
                 raise ValueError(f"Unsupported connection name: {connection}")
-        elif DuckDBPyConnection is not None and isinstance(connection, DuckDBPyConnection):
+        elif duckdb is not None and isinstance(connection, duckdb.DuckDBPyConnection):
             from vegafusion.connection.duckdb import DuckDbConnection
             connection = DuckDbConnection(connection)
         elif not isinstance(connection, SqlConnection):
             raise ValueError(
                 "connection argument must be a string or an instance of SqlConnection\n"
                 f"Received value of type {type(connection).__name__}: {connection}"
             )
@@ -198,42 +190,45 @@
         if self._grpc_channel:
             return self.grpc_query(request)
         else:
             # No grpc channel, get or initialize an embedded runtime
             return self.embedded_runtime.process_request_bytes(request)
 
     def _import_or_register_inline_datasets(self, inline_datasets=None):
+        pl = sys.modules.get("polars", None)
+        pa = sys.modules.get("pyarrow", None)
+        pd = sys.modules.get("pandas", None)
+
         inline_datasets = inline_datasets or dict()
         imported_inline_datasets = dict()
         for name, value in inline_datasets.items():
             if isinstance(value, SqlDataset):
                 imported_inline_datasets[name] = value
             elif isinstance(value, DataFrameDataset):
                 imported_inline_datasets[name] = value
-            elif isinstance(value, pd.DataFrame):
+            elif pd is not None and isinstance(value, pd.DataFrame):
                 if self._connection is not None:
                     try:
                         # Try registering DataFrame if supported
                         self._connection.register_pandas(name, value, temporary=True)
                         continue
                     except ValueError:
                         pass
 
                 imported_inline_datasets[name] = PandasDatasource(value)
             elif hasattr(value, "__dataframe__"):
                 # Let polars convert to pyarrow since it has broader support than the raw dataframe interchange
                 # protocol, and "This operation is mostly zero copy."
                 try:
-                    import polars as pl
-                    if isinstance(value, pl.DataFrame):
+                    if pl is not None and isinstance(value, pl.DataFrame):
                         value = value.to_arrow()
                 except ImportError:
                     pass
 
-                if isinstance(value, pa.Table):
+                if pa is not None and isinstance(value, pa.Table):
                     try:
                         if self._connection is not None:
                             # Try registering Arrow Table if supported
                             self._connection.register_arrow(name, value, temporary=True)
                             continue
                     except ValueError:
                         pass
@@ -498,28 +493,30 @@
                     inline_datasets=inline_arrow_dataset
                 )
             finally:
                 # Clean up registered tables (both inline and internal temporary tables)
                 if self._connection is not None:
                     self._connection.unregister_temporary_tables()
 
+            pl = sys.modules.get("polars", None)
+            pa = sys.modules.get("pyarrow", None)
             if pl is not None and _all_datasets_have_type(inline_datasets, (pl.DataFrame, pl.LazyFrame)):
                 # Deserialize values to Polars tables
                 datasets = [pl.from_arrow(value) for value in values]
 
                 # Localize datetime columns to UTC
                 processed_datasets = []
                 for df in datasets:
                     for name, dtype in zip(df.columns, df.dtypes):
                         if dtype == pl.Datetime:
                             df = df.with_columns(df[name].dt.replace_time_zone("UTC").dt.convert_time_zone(local_tz))
                     processed_datasets.append(df)
 
                 return processed_datasets, warnings
-            elif _all_datasets_have_type(inline_datasets, pa.Table):
+            elif pa is not None and _all_datasets_have_type(inline_datasets, pa.Table):
                 return values, warnings
             else:
                 # Deserialize values to pandas DataFrames
                 datasets = [value.to_pandas() for value in values]
 
                 # Localize datetime columns to UTC
                 for df in datasets:
@@ -749,8 +746,27 @@
             else:
                 raise ValueError(err_msg)
         else:
             raise ValueError(err_msg)
     return pre_tx_vars
 
 
+def get_mark_group_for_scope(vega_spec, scope):
+    group = vega_spec
+
+    # Find group at scope
+    for scope_value in scope:
+        group_index = 0
+        child_group = None
+        for mark in group.get("marks", []):
+            if mark.get("type") == "group":
+                if group_index == scope_value:
+                    child_group = mark
+                    break
+                group_index += 1
+        if child_group is None:
+            return None
+        group = child_group
+
+    return group
+
 runtime = VegaFusionRuntime(64, psutil.virtual_memory().total // 2, psutil.cpu_count())
```

### Comparing `vegafusion-1.6.8/vegafusion/save.py` & `vegafusion-1.6.9/vegafusion/save.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/vegafusion/transformer.py` & `vegafusion-1.6.9/vegafusion/transformer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 import io
 import os
+import sys
 import pathlib
 from hashlib import sha1
 from tempfile import NamedTemporaryFile
 import uuid
-import altair as alt
-import pandas as pd
-import pyarrow as pa
 from weakref import WeakValueDictionary
 
 DATASET_PREFIXES = ("vegafusion+dataset://", "table://")
 BATCH_SIZE = 8096
 
 
 def to_arrow_table(data):
     """
     Helper to convert a Pandas DataFrame to a PyArrow Table
 
     :param data: Pandas DataFrame
     :return: pyarrow.Table
     """
     import pyarrow as pa
+    pd = sys.modules.get("pandas")
 
     # Reset named index(ex) into a column
     if getattr(data.index, "name", None) is not None:
         data = data.reset_index()
 
     # Use pyarrow to infer schema from DataFrame
     for col, pd_type in data.dtypes.items():
@@ -41,15 +40,15 @@
         except pa.ArrowTypeError:
             if pd_type.kind == "O":
                 # Try converting object columns to strings to handle cases where a
                 # column has a mix of numbers and strings
                 data = data.assign(**{col: data[col].astype(str)})
 
         # Expand categoricals (not yet supported in VegaFusion)
-        if isinstance(pd_type, pd.CategoricalDtype):
+        if pd is not None and isinstance(pd_type, pd.CategoricalDtype):
             cat = data[col].cat
             data = data.assign(**{col: cat.categories[cat.codes]})
 
         # Copy un-aligned columns to align them
         # (arrow-rs seems to have trouble with un-aligned arrays)
         values = getattr(data[col], "values", None)
         if values is not None:
@@ -78,17 +77,19 @@
     Helper to convert a DataFrame to the Arrow IPC binary format
 
     :param data: Pandas DataFrame, pyarrow Table, or object that supports
         the DataFrame Interchange Protocol
     :param stream: If True, write IPC Stream format. If False (default), write ipc file format.
     :return: bytes
     """
-    if isinstance(data, pd.DataFrame):
+    pa = sys.modules.get("pyarrow", None)
+    pd = sys.modules.get("pandas", None)
+    if pd is not None and isinstance(data, pd.DataFrame):
         table = to_arrow_table(data)
-    elif isinstance(data, pa.Table):
+    elif pa is not None and isinstance(data, pa.Table):
         table = data
     elif hasattr(data, "__dataframe__"):
         pi = import_pyarrow_interchange()
         table = pi.from_dataframe(data)
     else:
         raise ValueError(f"Unsupported input to to_arrow_ipc_bytes: {type(data)}")
     return arrow_table_to_ipc_bytes(table, stream=stream)
@@ -129,14 +130,15 @@
     else:
         with open(file, "wb") as f:
             f.write(file_bytes)
 
 
 def feather_transformer(data, data_dir="_vegafusion_data"):
     from vegafusion import runtime
+    import altair as alt
 
     if "vegafusion" not in alt.renderers.active:
         # Use default transformer if a vegafusion renderer is not active
         return alt.default_data_transformer(data)
     elif has_geo_interface(data):
         # Use default transformer for geo interface objects
         # (e.g. a geopandas GeoDataFrame)
@@ -213,41 +215,43 @@
         except KeyError:
             # named dataset that was provided by the user
             pass
     return datasets
 
 
 def inline_data_transformer(data):
+    import altair as alt
     if has_geo_interface(data):
         # Use default transformer for geo interface objects
         # # (e.g. a geopandas GeoDataFrame)
         return alt.default_data_transformer(data)
     elif is_dataframe_like(data):
         table_name = f"table_{uuid.uuid4()}".replace("-", "_")
         __inline_tables[table_name] = data
         return {"url": DATASET_PREFIXES[0] + table_name}
     else:
         # Use default transformer if we don't recognize data
         return alt.default_data_transformer(data)
 
 
 def is_dataframe_like(data):
-    return isinstance(data, (pd.DataFrame, pa.Table)) or hasattr(data, "__dataframe__")
+    pa = sys.modules.get("pyarrow")
+    pd = sys.modules.get("pandas")
+    is_pa_table = pa is not None and isinstance(data, pa.Table)
+    is_pd_table = pd is not None and isinstance(data, pd.DataFrame)
+    return is_pa_table or is_pd_table or hasattr(data, "__dataframe__")
 
 
 def has_geo_interface(data):
     return hasattr(data, "__geo_interface__")
 
 
 def import_pyarrow_interchange():
     try:
         import pyarrow.interchange as pi
         return pi
     except ImportError:
+        import pyarrow as pa
         raise ImportError(
             "Use of the DataFrame Interchange Protocol requires at least version 11.0.0 of pyarrow\n"
             f"Found version {pa.__version__}"
         )
-
-
-alt.data_transformers.register("vegafusion-feather", feather_transformer)
-alt.data_transformers.register("vegafusion-inline", inline_data_transformer)
```

### Comparing `vegafusion-1.6.8/vegafusion/utils.py` & `vegafusion-1.6.9/vegafusion/utils.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.6.8/vegafusion.egg-info/PKG-INFO` & `vegafusion-1.6.9/vegafusion.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: vegafusion
-Version: 1.6.8
+Version: 1.6.9
 Summary: Core tools for using VegaFusion from Python
 License: BSD-3-Clause
 Keywords: vega,altair,vegafusion,arrow
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Requires-Dist: altair>=4.2.0
+Requires-Dist: altair>=5.2.0
 Requires-Dist: pyarrow>=5
 Requires-Dist: pandas
 Requires-Dist: psutil
 Requires-Dist: protobuf
 Provides-Extra: embed
-Requires-Dist: vegafusion-python-embed==1.6.8; extra == "embed"
+Requires-Dist: vegafusion-python-embed==1.6.9; extra == "embed"
 Requires-Dist: vl-convert-python>=0.7.0; extra == "embed"
 
 ## VegaFusion
 This package is part of the VegaFusion project: https://vegafusion.io.
 
 In particular, the `vegafusion` package provides a pure Python interface to a VegaFusion Runtime. Initially, the only runtime available is provided by the `vegafusion-python-embed` package. Eventually, the VegaFusion runtime will be available as a standalone gRPC server and this package will be updated to support communication with a VegaFusion Runtime over gRPC as an alternative to the Runtime provided by `vegafusion-python-embed`.
```

### Comparing `vegafusion-1.6.8/vegafusion.egg-info/SOURCES.txt` & `vegafusion-1.6.9/vegafusion.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 LICENSE.txt
 README.md
 pyproject.toml
 pytest.ini
 setup.cfg
 setup.py
+checks/README.md
+checks/check_lazy_imports.py
 proto/datafusion.proto
 tests/test_conext_manager.py
 tests/test_datasource.py
 tests/test_input_utc.py
 tests/test_pretransform.py
 tests/test_pretransform_specs.py
 tests/test_row_limit.py
@@ -191,27 +193,27 @@
 tests/altair_mocks/simple/heatmap/mock.py
 tests/altair_mocks/simple/line_chart/mock.py
 tests/altair_mocks/simple/scatter_tooltips/mock.py
 tests/altair_mocks/simple/stacked_bar_chart/mock.py
 tests/altair_mocks/simple/strip_chart/mock.py
 vegafusion/__init__.py
 vegafusion/_version.py
-vegafusion/compilers.py
 vegafusion/embed.py
 vegafusion/evaluation.py
 vegafusion/jupyter.py
 vegafusion/local_tz.py
 vegafusion/renderer.py
 vegafusion/runtime.py
 vegafusion/save.py
 vegafusion/transformer.py
 vegafusion/utils.py
 vegafusion.egg-info/PKG-INFO
 vegafusion.egg-info/SOURCES.txt
 vegafusion.egg-info/dependency_links.txt
+vegafusion.egg-info/entry_points.txt
 vegafusion.egg-info/requires.txt
 vegafusion.egg-info/top_level.txt
 vegafusion/connection/__init__.py
 vegafusion/connection/duckdb.py
 vegafusion/dataset/__init__.py
 vegafusion/dataset/dataframe.py
 vegafusion/dataset/dfi.py
```

