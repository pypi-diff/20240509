# Comparing `tmp/pycollimator-2.0.3-py3-none-any.whl.zip` & `tmp/pycollimator-2.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,133 +1,170 @@
-Zip file size: 385190 bytes, number of entries: 131
--rw-r--r--  2.0 unx     1905 b- defN 24-Apr-01 02:40 collimator/__init__.py
+Zip file size: 490848 bytes, number of entries: 168
+-rw-r--r--  2.0 unx     1985 b- defN 24-May-09 06:03 collimator/__init__.py
 -rw-r--r--  2.0 unx     4049 b- defN 20-Apr-16 12:00 collimator/lazy_loader.py
--rw-r--r--  2.0 unx     2913 b- defN 24-Apr-01 02:40 collimator/logging.py
--rw-r--r--  2.0 unx     5913 b- defN 24-Apr-01 02:40 collimator/profiling.py
--rw-r--r--  2.0 unx      939 b- defN 24-Apr-01 02:40 collimator/version.py
--rw-r--r--  2.0 unx     1478 b- defN 24-Apr-01 02:40 collimator/backend/__init__.py
--rw-r--r--  2.0 unx     1284 b- defN 24-Apr-01 02:40 collimator/backend/_torch.py
--rw-r--r--  2.0 unx     5335 b- defN 24-Apr-01 02:40 collimator/backend/backend.py
--rw-r--r--  2.0 unx     5800 b- defN 24-Apr-01 02:40 collimator/backend/ode_solver.py
--rw-r--r--  2.0 unx     5835 b- defN 24-Apr-01 02:40 collimator/backend/results_data.py
--rw-r--r--  2.0 unx     1071 b- defN 24-Apr-01 02:40 collimator/backend/typing.py
--rw-r--r--  2.0 unx     1675 b- defN 24-Apr-01 02:40 collimator/backend/utils.py
--rw-r--r--  2.0 unx     1269 b- defN 24-Apr-01 02:40 collimator/backend/_jax/__init__.py
--rw-r--r--  2.0 unx    15508 b- defN 24-Apr-01 02:40 collimator/backend/_jax/dopri5.py
--rw-r--r--  2.0 unx     1863 b- defN 24-Apr-01 02:40 collimator/backend/_jax/ode_solver.py
--rw-r--r--  2.0 unx     9276 b- defN 24-Apr-01 02:40 collimator/backend/_jax/results_data.py
--rw-r--r--  2.0 unx     3647 b- defN 24-Apr-01 02:40 collimator/backend/_jax/rk4.py
--rw-r--r--  2.0 unx     1270 b- defN 24-Apr-01 02:40 collimator/backend/_numpy/__init__.py
--rw-r--r--  2.0 unx     7108 b- defN 24-Apr-01 02:40 collimator/backend/_numpy/ode_solver.py
--rw-r--r--  2.0 unx     1807 b- defN 24-Apr-01 02:40 collimator/backend/_numpy/python_functions.py
--rw-r--r--  2.0 unx     3093 b- defN 24-Apr-01 02:40 collimator/backend/_numpy/results_data.py
--rw-r--r--  2.0 unx      781 b- defN 24-Apr-01 02:40 collimator/cli/__init__.py
--rw-r--r--  2.0 unx     4155 b- defN 24-Apr-01 02:40 collimator/cli/cli_run.py
--rw-r--r--  2.0 unx      831 b- defN 24-Apr-01 02:40 collimator/cli/collimator_cli.py
--rw-r--r--  2.0 unx    13057 b- defN 24-Apr-01 02:40 collimator/cli/model_interface.py
--rw-r--r--  2.0 unx      760 b- defN 24-Apr-01 02:40 collimator/dashboard/__init__.py
--rw-r--r--  2.0 unx     5539 b- defN 24-Apr-01 02:40 collimator/dashboard/api.py
--rw-r--r--  2.0 unx     6191 b- defN 24-Apr-01 02:40 collimator/dashboard/model.py
--rw-r--r--  2.0 unx    26196 b- defN 24-Apr-01 02:40 collimator/dashboard/project.py
--rw-r--r--  2.0 unx     1632 b- defN 24-Apr-01 02:40 collimator/dashboard/results.py
--rw-r--r--  2.0 unx     1313 b- defN 24-Apr-01 02:40 collimator/dashboard/schemas.py
--rw-r--r--  2.0 unx     2449 b- defN 24-Apr-01 02:40 collimator/dashboard/uiprops.py
--rw-r--r--  2.0 unx      872 b- defN 24-Apr-01 02:40 collimator/dashboard/serialization/__init__.py
--rw-r--r--  2.0 unx    21080 b- defN 24-Apr-01 02:40 collimator/dashboard/serialization/block_interface.py
--rw-r--r--  2.0 unx    42872 b- defN 24-Apr-01 02:40 collimator/dashboard/serialization/from_model_json.py
--rw-r--r--  2.0 unx     8449 b- defN 24-Apr-01 02:40 collimator/dashboard/serialization/model_json.py
--rw-r--r--  2.0 unx     4871 b- defN 24-Apr-01 02:40 collimator/dashboard/serialization/time_mode.py
--rw-r--r--  2.0 unx    14745 b- defN 24-Apr-01 02:40 collimator/dashboard/serialization/to_model_json.py
--rw-r--r--  2.0 unx     3793 b- defN 24-Apr-01 02:40 collimator/dashboard/serialization/ui_types.py
--rw-r--r--  2.0 unx      672 b- defN 24-Apr-01 02:40 collimator/experimental/__init__.py
--rw-r--r--  2.0 unx      786 b- defN 24-Apr-01 02:40 collimator/experimental/acausal/__init__.py
--rw-r--r--  2.0 unx    38410 b- defN 24-Apr-01 02:40 collimator/experimental/acausal/compiler.py
--rw-r--r--  2.0 unx     2733 b- defN 24-Apr-01 02:40 collimator/experimental/acausal/network_builder.py
--rw-r--r--  2.0 unx     1413 b- defN 24-Apr-01 02:40 collimator/experimental/acausal/component_library/__init__.py
--rw-r--r--  2.0 unx     4723 b- defN 24-Apr-01 02:40 collimator/experimental/acausal/component_library/base.py
--rw-r--r--  2.0 unx     8850 b- defN 24-Apr-01 02:40 collimator/experimental/acausal/component_library/elec.py
--rw-r--r--  2.0 unx    13410 b- defN 24-Apr-01 02:40 collimator/experimental/acausal/component_library/mech.py
--rw-r--r--  2.0 unx     2342 b- defN 24-Apr-01 02:40 collimator/framework/__init__.py
--rw-r--r--  2.0 unx     6637 b- defN 24-Apr-01 02:40 collimator/framework/cache.py
--rw-r--r--  2.0 unx    18536 b- defN 24-Apr-01 02:40 collimator/framework/context.py
--rw-r--r--  2.0 unx     9049 b- defN 24-Apr-01 02:40 collimator/framework/context_factory.py
--rw-r--r--  2.0 unx    20243 b- defN 24-Apr-01 02:40 collimator/framework/dependency_graph.py
--rw-r--r--  2.0 unx    21169 b- defN 24-Apr-01 02:40 collimator/framework/diagram.py
--rw-r--r--  2.0 unx    21320 b- defN 24-Apr-01 02:40 collimator/framework/diagram_builder.py
--rw-r--r--  2.0 unx    12769 b- defN 24-Apr-01 02:40 collimator/framework/error.py
--rw-r--r--  2.0 unx    25404 b- defN 24-Apr-01 02:40 collimator/framework/event.py
--rw-r--r--  2.0 unx    52536 b- defN 24-Apr-01 02:40 collimator/framework/leaf_system.py
--rw-r--r--  2.0 unx    14946 b- defN 24-Apr-01 02:40 collimator/framework/parameter.py
--rw-r--r--  2.0 unx     6790 b- defN 24-Apr-01 02:40 collimator/framework/port.py
--rw-r--r--  2.0 unx     8853 b- defN 24-Apr-01 02:40 collimator/framework/state.py
--rw-r--r--  2.0 unx    40677 b- defN 24-Apr-01 02:40 collimator/framework/system_base.py
--rw-r--r--  2.0 unx     5226 b- defN 24-Apr-01 02:40 collimator/library/__init__.py
--rw-r--r--  2.0 unx     3441 b- defN 24-Apr-01 02:40 collimator/library/ansys.py
--rw-r--r--  2.0 unx     6331 b- defN 24-Apr-01 02:40 collimator/library/battery_cell.py
--rw-r--r--  2.0 unx    31129 b- defN 24-Apr-01 02:40 collimator/library/custom.py
--rw-r--r--  2.0 unx    14150 b- defN 24-Apr-01 02:40 collimator/library/data_source.py
--rw-r--r--  2.0 unx    13209 b- defN 24-Apr-01 02:40 collimator/library/fmu_import.py
--rw-r--r--  2.0 unx     3571 b- defN 24-Apr-01 02:40 collimator/library/generic.py
--rw-r--r--  2.0 unx    18862 b- defN 24-Apr-01 02:40 collimator/library/linear_system.py
--rw-r--r--  2.0 unx     9733 b- defN 24-Apr-01 02:40 collimator/library/lqr.py
--rw-r--r--  2.0 unx    10341 b- defN 24-Apr-01 02:40 collimator/library/mpc.py
--rw-r--r--  2.0 unx     5727 b- defN 24-Apr-01 02:40 collimator/library/nn.py
--rw-r--r--  2.0 unx    12210 b- defN 24-Apr-01 02:40 collimator/library/predictor.py
--rw-r--r--  2.0 unx   126394 b- defN 24-Apr-01 02:40 collimator/library/primitives.py
--rw-r--r--  2.0 unx     9982 b- defN 24-Apr-01 02:40 collimator/library/random.py
--rw-r--r--  2.0 unx     4587 b- defN 24-Apr-01 02:40 collimator/library/reference_subdiagram.py
--rw-r--r--  2.0 unx    36143 b- defN 24-Apr-01 02:40 collimator/library/rotations.py
--rw-r--r--  2.0 unx    12610 b- defN 24-Apr-01 02:40 collimator/library/sindy.py
--rw-r--r--  2.0 unx    21027 b- defN 24-Apr-01 02:40 collimator/library/state_machine.py
--rw-r--r--  2.0 unx     1521 b- defN 24-Apr-01 02:40 collimator/library/wrappers.py
--rw-r--r--  2.0 unx     1307 b- defN 24-Apr-01 02:40 collimator/library/nmpc/__init__.py
--rw-r--r--  2.0 unx     5425 b- defN 24-Apr-01 02:40 collimator/library/nmpc/direct_shooting_ipopt_nmpc.py
--rw-r--r--  2.0 unx     6827 b- defN 24-Apr-01 02:40 collimator/library/nmpc/direct_transcription_ipopt_nmpc.py
--rw-r--r--  2.0 unx     8507 b- defN 24-Apr-01 02:40 collimator/library/nmpc/hermite_simpson_ipopt_nmpc.py
--rw-r--r--  2.0 unx     2732 b- defN 24-Apr-01 02:40 collimator/library/nmpc/trajectory_optimization.py
--rw-r--r--  2.0 unx      889 b- defN 24-Apr-01 02:40 collimator/library/nmpc/base/__init__.py
--rw-r--r--  2.0 unx     9256 b- defN 24-Apr-01 02:40 collimator/library/nmpc/base/nlp_ipopt_base.py
--rw-r--r--  2.0 unx     4091 b- defN 24-Apr-01 02:40 collimator/library/nmpc/base/nmpc_base.py
--rw-r--r--  2.0 unx     7490 b- defN 24-Apr-01 02:40 collimator/library/nmpc/base/nmpc_ipopt_base.py
--rw-r--r--  2.0 unx     1227 b- defN 24-Apr-01 02:40 collimator/library/state_estimators/__init__.py
--rw-r--r--  2.0 unx     6865 b- defN 24-Apr-01 02:40 collimator/library/state_estimators/continuous_time_infinite_horizon_kalman_filter.py
--rw-r--r--  2.0 unx    11723 b- defN 24-Apr-01 02:40 collimator/library/state_estimators/extended_kalman_filter.py
--rw-r--r--  2.0 unx     8868 b- defN 24-Apr-01 02:40 collimator/library/state_estimators/infinite_horizon_kalman_filter.py
--rw-r--r--  2.0 unx     8751 b- defN 24-Apr-01 02:40 collimator/library/state_estimators/kalman_filter.py
--rw-r--r--  2.0 unx     7055 b- defN 24-Apr-01 02:40 collimator/library/state_estimators/kalman_filter_base.py
--rw-r--r--  2.0 unx    16059 b- defN 24-Apr-01 02:40 collimator/library/state_estimators/unscented_kalman_filter.py
--rw-r--r--  2.0 unx     8889 b- defN 24-Apr-01 02:40 collimator/library/state_estimators/utils.py
--rw-r--r--  2.0 unx      948 b- defN 24-Apr-01 02:40 collimator/library/utils/__init__.py
--rw-r--r--  2.0 unx     2509 b- defN 24-Apr-01 02:40 collimator/library/utils/plant_utils.py
--rw-r--r--  2.0 unx     3320 b- defN 24-Apr-01 02:40 collimator/library/utils/rk4_utils.py
--rw-r--r--  2.0 unx     1767 b- defN 24-Apr-01 02:40 collimator/models/__init__.py
--rw-r--r--  2.0 unx     5083 b- defN 24-Apr-01 02:40 collimator/models/acrobot.py
--rw-r--r--  2.0 unx     3713 b- defN 24-Apr-01 02:40 collimator/models/battery_ecm.py
--rw-r--r--  2.0 unx     2509 b- defN 24-Apr-01 02:40 collimator/models/bouncing_ball.py
--rw-r--r--  2.0 unx     4319 b- defN 24-Apr-01 02:40 collimator/models/cartpole.py
--rw-r--r--  2.0 unx    21940 b- defN 24-Apr-01 02:40 collimator/models/compact_ev.py
--rw-r--r--  2.0 unx     9644 b- defN 24-Apr-01 02:40 collimator/models/compass_gait.py
--rw-r--r--  2.0 unx     1565 b- defN 24-Apr-01 02:40 collimator/models/fitzhugh_nagumo.py
--rw-r--r--  2.0 unx     4868 b- defN 24-Apr-01 02:40 collimator/models/hairer.py
--rw-r--r--  2.0 unx     1515 b- defN 24-Apr-01 02:40 collimator/models/lotka_volterra.py
--rw-r--r--  2.0 unx     7998 b- defN 24-Apr-01 02:40 collimator/models/pendulum.py
--rw-r--r--  2.0 unx     6818 b- defN 24-Apr-01 02:40 collimator/models/planar_quadrotor.py
--rw-r--r--  2.0 unx     6970 b- defN 24-Apr-01 02:40 collimator/models/rimless_wheel.py
--rw-r--r--  2.0 unx     1188 b- defN 24-Apr-01 02:40 collimator/models/van_der_pol.py
--rw-r--r--  2.0 unx     1071 b- defN 24-Apr-01 02:40 collimator/models/quadcopter/__init__.py
--rw-r--r--  2.0 unx     4544 b- defN 24-Apr-01 02:40 collimator/models/quadcopter/plot_utils.py
--rw-r--r--  2.0 unx     4113 b- defN 24-Apr-01 02:40 collimator/models/quadcopter/quadcopter.py
--rw-r--r--  2.0 unx     4396 b- defN 24-Apr-01 02:40 collimator/models/quadcopter/trajectory_generation.py
--rw-r--r--  2.0 unx     2732 b- defN 24-Apr-01 02:40 collimator/models/quadcopter/transformations.py
--rw-r--r--  2.0 unx      725 b- defN 24-Apr-01 02:40 collimator/optimization/__init__.py
--rw-r--r--  2.0 unx     6246 b- defN 24-Apr-01 02:40 collimator/optimization/training.py
--rw-r--r--  2.0 unx     1059 b- defN 24-Apr-01 02:40 collimator/simulation/__init__.py
--rw-r--r--  2.0 unx    67307 b- defN 24-Apr-01 02:40 collimator/simulation/simulator.py
--rw-r--r--  2.0 unx     9891 b- defN 24-Apr-01 02:40 collimator/simulation/types.py
--rw-r--r--  2.0 unx      650 b- defN 24-Apr-01 02:40 pycollimator-2.0.3.dist-info/LICENSE.header.txt
--rw-r--r--  2.0 unx    34120 b- defN 24-Apr-01 02:40 pycollimator-2.0.3.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     3794 b- defN 24-Apr-01 02:40 pycollimator-2.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-01 02:40 pycollimator-2.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       69 b- defN 24-Apr-01 02:40 pycollimator-2.0.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 24-Apr-01 02:40 pycollimator-2.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    12325 b- defN 24-Apr-01 02:40 pycollimator-2.0.3.dist-info/RECORD
-131 files, 1276866 bytes uncompressed, 365420 bytes compressed:  71.4%
+-rw-r--r--  2.0 unx     2913 b- defN 24-May-09 06:03 collimator/logging.py
+-rw-r--r--  2.0 unx     5913 b- defN 24-May-09 06:03 collimator/profiling.py
+-rw-r--r--  2.0 unx      939 b- defN 24-May-09 06:03 collimator/version.py
+-rw-r--r--  2.0 unx     1478 b- defN 24-May-09 06:03 collimator/backend/__init__.py
+-rw-r--r--  2.0 unx     1284 b- defN 24-May-09 06:03 collimator/backend/_torch.py
+-rw-r--r--  2.0 unx     5424 b- defN 24-May-09 06:03 collimator/backend/backend.py
+-rw-r--r--  2.0 unx     5867 b- defN 24-May-09 06:03 collimator/backend/ode_solver.py
+-rw-r--r--  2.0 unx     5835 b- defN 24-May-09 06:03 collimator/backend/results_data.py
+-rw-r--r--  2.0 unx     1071 b- defN 24-May-09 06:03 collimator/backend/typing.py
+-rw-r--r--  2.0 unx     1681 b- defN 24-May-09 06:03 collimator/backend/utils.py
+-rw-r--r--  2.0 unx     1269 b- defN 24-May-09 06:03 collimator/backend/_jax/__init__.py
+-rw-r--r--  2.0 unx    19246 b- defN 24-May-09 06:03 collimator/backend/_jax/bdf.py
+-rw-r--r--  2.0 unx     9956 b- defN 24-May-09 06:03 collimator/backend/_jax/dopri5.py
+-rw-r--r--  2.0 unx     2152 b- defN 24-May-09 06:03 collimator/backend/_jax/ode_solver.py
+-rw-r--r--  2.0 unx     6178 b- defN 24-May-09 06:03 collimator/backend/_jax/ode_solver_impl.py
+-rw-r--r--  2.0 unx     9365 b- defN 24-May-09 06:03 collimator/backend/_jax/results_data.py
+-rw-r--r--  2.0 unx     3647 b- defN 24-May-09 06:03 collimator/backend/_jax/rk4.py
+-rw-r--r--  2.0 unx     1270 b- defN 24-May-09 06:03 collimator/backend/_numpy/__init__.py
+-rw-r--r--  2.0 unx     7108 b- defN 24-May-09 06:03 collimator/backend/_numpy/ode_solver.py
+-rw-r--r--  2.0 unx     1807 b- defN 24-May-09 06:03 collimator/backend/_numpy/python_functions.py
+-rw-r--r--  2.0 unx     3093 b- defN 24-May-09 06:03 collimator/backend/_numpy/results_data.py
+-rw-r--r--  2.0 unx      829 b- defN 24-May-09 06:03 collimator/cli/__init__.py
+-rw-r--r--  2.0 unx     4155 b- defN 24-May-09 06:03 collimator/cli/cli_run.py
+-rw-r--r--  2.0 unx      831 b- defN 24-May-09 06:03 collimator/cli/collimator_cli.py
+-rw-r--r--  2.0 unx    16715 b- defN 24-May-09 06:03 collimator/cli/model_interface.py
+-rw-r--r--  2.0 unx      760 b- defN 24-May-09 06:03 collimator/dashboard/__init__.py
+-rw-r--r--  2.0 unx     5539 b- defN 24-May-09 06:03 collimator/dashboard/api.py
+-rw-r--r--  2.0 unx     6191 b- defN 24-May-09 06:03 collimator/dashboard/model.py
+-rw-r--r--  2.0 unx    26209 b- defN 24-May-09 06:03 collimator/dashboard/project.py
+-rw-r--r--  2.0 unx     1632 b- defN 24-May-09 06:03 collimator/dashboard/results.py
+-rw-r--r--  2.0 unx     1313 b- defN 24-May-09 06:03 collimator/dashboard/schemas.py
+-rw-r--r--  2.0 unx     2449 b- defN 24-May-09 06:03 collimator/dashboard/uiprops.py
+-rw-r--r--  2.0 unx      872 b- defN 24-May-09 06:03 collimator/dashboard/serialization/__init__.py
+-rw-r--r--  2.0 unx    27999 b- defN 24-May-09 06:03 collimator/dashboard/serialization/block_interface.py
+-rw-r--r--  2.0 unx    46633 b- defN 24-May-09 06:03 collimator/dashboard/serialization/from_model_json.py
+-rw-r--r--  2.0 unx     8485 b- defN 24-May-09 06:03 collimator/dashboard/serialization/model_json.py
+-rw-r--r--  2.0 unx     4865 b- defN 24-May-09 06:03 collimator/dashboard/serialization/time_mode.py
+-rw-r--r--  2.0 unx    15095 b- defN 24-May-09 06:03 collimator/dashboard/serialization/to_model_json.py
+-rw-r--r--  2.0 unx     3793 b- defN 24-May-09 06:03 collimator/dashboard/serialization/ui_types.py
+-rw-r--r--  2.0 unx      672 b- defN 24-May-09 06:03 collimator/experimental/__init__.py
+-rw-r--r--  2.0 unx      822 b- defN 24-May-09 06:03 collimator/experimental/acausal/__init__.py
+-rw-r--r--  2.0 unx    39125 b- defN 24-May-09 06:03 collimator/experimental/acausal/compiler.py
+-rw-r--r--  2.0 unx     3211 b- defN 24-May-09 06:03 collimator/experimental/acausal/network_builder.py
+-rw-r--r--  2.0 unx      672 b- defN 24-May-09 06:03 collimator/experimental/acausal/component_library/__init__.py
+-rw-r--r--  2.0 unx     4723 b- defN 24-May-09 06:03 collimator/experimental/acausal/component_library/base.py
+-rw-r--r--  2.0 unx     6889 b- defN 24-May-09 06:03 collimator/experimental/acausal/component_library/elec.py
+-rw-r--r--  2.0 unx     7042 b- defN 24-May-09 06:03 collimator/experimental/acausal/component_library/rotational.py
+-rw-r--r--  2.0 unx     6935 b- defN 24-May-09 06:03 collimator/experimental/acausal/component_library/translational.py
+-rw-r--r--  2.0 unx      901 b- defN 24-May-09 06:03 collimator/experimental/acausal2/__init__.py
+-rw-r--r--  2.0 unx     5995 b- defN 24-May-09 06:03 collimator/experimental/acausal2/acausal_compiler.py
+-rw-r--r--  2.0 unx     1047 b- defN 24-May-09 06:03 collimator/experimental/acausal2/acausal_system.py
+-rw-r--r--  2.0 unx    40984 b- defN 24-May-09 06:03 collimator/experimental/acausal2/diagram_processing.py
+-rw-r--r--  2.0 unx     4603 b- defN 24-May-09 06:03 collimator/experimental/acausal2/phleaf_generator.py
+-rw-r--r--  2.0 unx    11004 b- defN 24-May-09 06:03 collimator/experimental/acausal2/run_examples.py
+-rw-r--r--  2.0 unx     1841 b- defN 24-May-09 06:03 collimator/experimental/acausal2/run_index_reduction_examples.py
+-rw-r--r--  2.0 unx     4923 b- defN 24-May-09 06:03 collimator/experimental/acausal2/run_regression.py
+-rw-r--r--  2.0 unx     7341 b- defN 24-May-09 06:03 collimator/experimental/acausal2/sandbox.py
+-rw-r--r--  2.0 unx      672 b- defN 24-May-09 06:03 collimator/experimental/acausal2/component_library/__init__.py
+-rw-r--r--  2.0 unx     7587 b- defN 24-May-09 06:03 collimator/experimental/acausal2/component_library/base.py
+-rw-r--r--  2.0 unx    15659 b- defN 24-May-09 06:03 collimator/experimental/acausal2/component_library/cross_domain.py
+-rw-r--r--  2.0 unx     8404 b- defN 24-May-09 06:03 collimator/experimental/acausal2/component_library/elec.py
+-rw-r--r--  2.0 unx    10915 b- defN 24-May-09 06:03 collimator/experimental/acausal2/component_library/fluid_i.py
+-rw-r--r--  2.0 unx     8237 b- defN 24-May-09 06:03 collimator/experimental/acausal2/component_library/rotational.py
+-rw-r--r--  2.0 unx     5489 b- defN 24-May-09 06:03 collimator/experimental/acausal2/component_library/thermal.py
+-rw-r--r--  2.0 unx     9185 b- defN 24-May-09 06:03 collimator/experimental/acausal2/component_library/translational.py
+-rw-r--r--  2.0 unx     1227 b- defN 24-May-09 06:03 collimator/experimental/acausal2/index_reduction/__init__.py
+-rw-r--r--  2.0 unx     5774 b- defN 24-May-09 06:03 collimator/experimental/acausal2/index_reduction/equation_utils.py
+-rw-r--r--  2.0 unx     2102 b- defN 24-May-09 06:03 collimator/experimental/acausal2/index_reduction/ex_Mattson.py
+-rw-r--r--  2.0 unx     1626 b- defN 24-May-09 06:03 collimator/experimental/acausal2/index_reduction/ex_exothermic_reactor.py
+-rw-r--r--  2.0 unx     1424 b- defN 24-May-09 06:03 collimator/experimental/acausal2/index_reduction/ex_pendulum.py
+-rw-r--r--  2.0 unx     4395 b- defN 24-May-09 06:03 collimator/experimental/acausal2/index_reduction/ex_pendulum_solve.py
+-rw-r--r--  2.0 unx     5291 b- defN 24-May-09 06:03 collimator/experimental/acausal2/index_reduction/graph_utils.py
+-rw-r--r--  2.0 unx    27551 b- defN 24-May-09 06:03 collimator/experimental/acausal2/index_reduction/index_reduction.py
+-rw-r--r--  2.0 unx      753 b- defN 24-May-09 06:03 collimator/experimental/acausal2/index_reduction/archive/__init__.py
+-rw-r--r--  2.0 unx     1697 b- defN 24-May-09 06:03 collimator/experimental/acausal2/index_reduction/archive/dummy_derivative_Mattsson.py
+-rw-r--r--  2.0 unx    22559 b- defN 24-May-09 06:03 collimator/experimental/acausal2/index_reduction/archive/index_reduction.py
+-rw-r--r--  2.0 unx     1353 b- defN 24-May-09 06:03 collimator/experimental/acausal2/index_reduction/archive/mech_oscillator.py
+-rw-r--r--  2.0 unx     1426 b- defN 24-May-09 06:03 collimator/experimental/acausal2/index_reduction/archive/pendulum.py
+-rw-r--r--  2.0 unx     2372 b- defN 24-May-09 06:03 collimator/framework/__init__.py
+-rw-r--r--  2.0 unx     6637 b- defN 24-May-09 06:03 collimator/framework/cache.py
+-rw-r--r--  2.0 unx    18493 b- defN 24-May-09 06:03 collimator/framework/context.py
+-rw-r--r--  2.0 unx     9541 b- defN 24-May-09 06:03 collimator/framework/context_factory.py
+-rw-r--r--  2.0 unx    20243 b- defN 24-May-09 06:03 collimator/framework/dependency_graph.py
+-rw-r--r--  2.0 unx    26689 b- defN 24-May-09 06:03 collimator/framework/diagram.py
+-rw-r--r--  2.0 unx    15697 b- defN 24-May-09 06:03 collimator/framework/diagram_builder.py
+-rw-r--r--  2.0 unx    12769 b- defN 24-May-09 06:03 collimator/framework/error.py
+-rw-r--r--  2.0 unx    25404 b- defN 24-May-09 06:03 collimator/framework/event.py
+-rw-r--r--  2.0 unx    56453 b- defN 24-May-09 06:03 collimator/framework/leaf_system.py
+-rw-r--r--  2.0 unx    17329 b- defN 24-May-09 06:03 collimator/framework/parameter.py
+-rw-r--r--  2.0 unx     6782 b- defN 24-May-09 06:03 collimator/framework/port.py
+-rw-r--r--  2.0 unx     8853 b- defN 24-May-09 06:03 collimator/framework/state.py
+-rw-r--r--  2.0 unx    47674 b- defN 24-May-09 06:03 collimator/framework/system_base.py
+-rw-r--r--  2.0 unx     5405 b- defN 24-May-09 06:03 collimator/library/__init__.py
+-rw-r--r--  2.0 unx     3409 b- defN 24-May-09 06:03 collimator/library/ansys.py
+-rw-r--r--  2.0 unx     6208 b- defN 24-May-09 06:03 collimator/library/battery_cell.py
+-rw-r--r--  2.0 unx     1423 b- defN 24-May-09 06:03 collimator/library/costs_and_losses.py
+-rw-r--r--  2.0 unx    31466 b- defN 24-May-09 06:03 collimator/library/custom.py
+-rw-r--r--  2.0 unx    14069 b- defN 24-May-09 06:03 collimator/library/data_source.py
+-rw-r--r--  2.0 unx    13212 b- defN 24-May-09 06:03 collimator/library/fmu_import.py
+-rw-r--r--  2.0 unx     3636 b- defN 24-May-09 06:03 collimator/library/generic.py
+-rw-r--r--  2.0 unx    20111 b- defN 24-May-09 06:03 collimator/library/linear_system.py
+-rw-r--r--  2.0 unx     9989 b- defN 24-May-09 06:03 collimator/library/lqr.py
+-rw-r--r--  2.0 unx    10341 b- defN 24-May-09 06:03 collimator/library/mpc.py
+-rw-r--r--  2.0 unx     9381 b- defN 24-May-09 06:03 collimator/library/nn.py
+-rw-r--r--  2.0 unx    13715 b- defN 24-May-09 06:03 collimator/library/predictor.py
+-rw-r--r--  2.0 unx   133203 b- defN 24-May-09 06:03 collimator/library/primitives.py
+-rw-r--r--  2.0 unx    14143 b- defN 24-May-09 06:03 collimator/library/quanser.py
+-rw-r--r--  2.0 unx    10312 b- defN 24-May-09 06:03 collimator/library/random.py
+-rw-r--r--  2.0 unx     4520 b- defN 24-May-09 06:03 collimator/library/reference_subdiagram.py
+-rw-r--r--  2.0 unx    12521 b- defN 24-May-09 06:03 collimator/library/ros2.py
+-rw-r--r--  2.0 unx    39750 b- defN 24-May-09 06:03 collimator/library/rotations.py
+-rw-r--r--  2.0 unx    22536 b- defN 24-May-09 06:03 collimator/library/sindy.py
+-rw-r--r--  2.0 unx    21027 b- defN 24-May-09 06:03 collimator/library/state_machine.py
+-rw-r--r--  2.0 unx     1521 b- defN 24-May-09 06:03 collimator/library/wrappers.py
+-rw-r--r--  2.0 unx     1307 b- defN 24-May-09 06:03 collimator/library/nmpc/__init__.py
+-rw-r--r--  2.0 unx     5425 b- defN 24-May-09 06:03 collimator/library/nmpc/direct_shooting_ipopt_nmpc.py
+-rw-r--r--  2.0 unx     6827 b- defN 24-May-09 06:03 collimator/library/nmpc/direct_transcription_ipopt_nmpc.py
+-rw-r--r--  2.0 unx     8507 b- defN 24-May-09 06:03 collimator/library/nmpc/hermite_simpson_ipopt_nmpc.py
+-rw-r--r--  2.0 unx     2676 b- defN 24-May-09 06:03 collimator/library/nmpc/trajectory_optimization.py
+-rw-r--r--  2.0 unx      887 b- defN 24-May-09 06:03 collimator/library/nmpc/base/__init__.py
+-rw-r--r--  2.0 unx     9254 b- defN 24-May-09 06:03 collimator/library/nmpc/base/nlp_ipopt_base.py
+-rw-r--r--  2.0 unx     4089 b- defN 24-May-09 06:03 collimator/library/nmpc/base/nmpc_base.py
+-rw-r--r--  2.0 unx     7488 b- defN 24-May-09 06:03 collimator/library/nmpc/base/nmpc_ipopt_base.py
+-rw-r--r--  2.0 unx     1227 b- defN 24-May-09 06:03 collimator/library/state_estimators/__init__.py
+-rw-r--r--  2.0 unx     6863 b- defN 24-May-09 06:03 collimator/library/state_estimators/continuous_time_infinite_horizon_kalman_filter.py
+-rw-r--r--  2.0 unx    11721 b- defN 24-May-09 06:03 collimator/library/state_estimators/extended_kalman_filter.py
+-rw-r--r--  2.0 unx    10690 b- defN 24-May-09 06:03 collimator/library/state_estimators/infinite_horizon_kalman_filter.py
+-rw-r--r--  2.0 unx    10782 b- defN 24-May-09 06:03 collimator/library/state_estimators/kalman_filter.py
+-rw-r--r--  2.0 unx     7081 b- defN 24-May-09 06:03 collimator/library/state_estimators/kalman_filter_base.py
+-rw-r--r--  2.0 unx    16057 b- defN 24-May-09 06:03 collimator/library/state_estimators/unscented_kalman_filter.py
+-rw-r--r--  2.0 unx    10783 b- defN 24-May-09 06:03 collimator/library/state_estimators/utils.py
+-rw-r--r--  2.0 unx     1082 b- defN 24-May-09 06:03 collimator/library/utils/__init__.py
+-rw-r--r--  2.0 unx     3151 b- defN 24-May-09 06:03 collimator/library/utils/csv_utils.py
+-rw-r--r--  2.0 unx     2507 b- defN 24-May-09 06:03 collimator/library/utils/plant_utils.py
+-rw-r--r--  2.0 unx     3318 b- defN 24-May-09 06:03 collimator/library/utils/rk4_utils.py
+-rw-r--r--  2.0 unx     1767 b- defN 24-May-09 06:03 collimator/models/__init__.py
+-rw-r--r--  2.0 unx     5147 b- defN 24-May-09 06:03 collimator/models/acrobot.py
+-rw-r--r--  2.0 unx     3745 b- defN 24-May-09 06:03 collimator/models/battery_ecm.py
+-rw-r--r--  2.0 unx     2571 b- defN 24-May-09 06:03 collimator/models/bouncing_ball.py
+-rw-r--r--  2.0 unx     4351 b- defN 24-May-09 06:03 collimator/models/cartpole.py
+-rw-r--r--  2.0 unx    21972 b- defN 24-May-09 06:03 collimator/models/compact_ev.py
+-rw-r--r--  2.0 unx     9700 b- defN 24-May-09 06:03 collimator/models/compass_gait.py
+-rw-r--r--  2.0 unx     1605 b- defN 24-May-09 06:03 collimator/models/fitzhugh_nagumo.py
+-rw-r--r--  2.0 unx     4954 b- defN 24-May-09 06:03 collimator/models/hairer.py
+-rw-r--r--  2.0 unx     1547 b- defN 24-May-09 06:03 collimator/models/lotka_volterra.py
+-rw-r--r--  2.0 unx     8030 b- defN 24-May-09 06:03 collimator/models/pendulum.py
+-rw-r--r--  2.0 unx     6850 b- defN 24-May-09 06:03 collimator/models/planar_quadrotor.py
+-rw-r--r--  2.0 unx     7024 b- defN 24-May-09 06:03 collimator/models/rimless_wheel.py
+-rw-r--r--  2.0 unx     1393 b- defN 24-May-09 06:03 collimator/models/van_der_pol.py
+-rw-r--r--  2.0 unx     1071 b- defN 24-May-09 06:03 collimator/models/quadcopter/__init__.py
+-rw-r--r--  2.0 unx     4544 b- defN 24-May-09 06:03 collimator/models/quadcopter/plot_utils.py
+-rw-r--r--  2.0 unx     4177 b- defN 24-May-09 06:03 collimator/models/quadcopter/quadcopter.py
+-rw-r--r--  2.0 unx     4396 b- defN 24-May-09 06:03 collimator/models/quadcopter/trajectory_generation.py
+-rw-r--r--  2.0 unx     2732 b- defN 24-May-09 06:03 collimator/models/quadcopter/transformations.py
+-rw-r--r--  2.0 unx      725 b- defN 24-May-09 06:03 collimator/optimization/__init__.py
+-rw-r--r--  2.0 unx     6743 b- defN 24-May-09 06:03 collimator/optimization/training.py
+-rw-r--r--  2.0 unx     1059 b- defN 24-May-09 06:03 collimator/simulation/__init__.py
+-rw-r--r--  2.0 unx    68337 b- defN 24-May-09 06:03 collimator/simulation/simulator.py
+-rw-r--r--  2.0 unx    10171 b- defN 24-May-09 06:03 collimator/simulation/types.py
+-rw-r--r--  2.0 unx      650 b- defN 24-May-09 06:03 pycollimator-2.0.4.dist-info/LICENSE.header.txt
+-rw-r--r--  2.0 unx    34120 b- defN 24-May-09 06:03 pycollimator-2.0.4.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     3812 b- defN 24-May-09 06:03 pycollimator-2.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-09 06:03 pycollimator-2.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       69 b- defN 24-May-09 06:03 pycollimator-2.0.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 24-May-09 06:03 pycollimator-2.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    16565 b- defN 24-May-09 06:03 pycollimator-2.0.4.dist-info/RECORD
+168 files, 1618437 bytes uncompressed, 464022 bytes compressed:  71.3%
```

## zipnote {}

```diff
@@ -33,20 +33,26 @@
 
 Filename: collimator/backend/utils.py
 Comment: 
 
 Filename: collimator/backend/_jax/__init__.py
 Comment: 
 
+Filename: collimator/backend/_jax/bdf.py
+Comment: 
+
 Filename: collimator/backend/_jax/dopri5.py
 Comment: 
 
 Filename: collimator/backend/_jax/ode_solver.py
 Comment: 
 
+Filename: collimator/backend/_jax/ode_solver_impl.py
+Comment: 
+
 Filename: collimator/backend/_jax/results_data.py
 Comment: 
 
 Filename: collimator/backend/_jax/rk4.py
 Comment: 
 
 Filename: collimator/backend/_numpy/__init__.py
@@ -132,15 +138,108 @@
 
 Filename: collimator/experimental/acausal/component_library/base.py
 Comment: 
 
 Filename: collimator/experimental/acausal/component_library/elec.py
 Comment: 
 
-Filename: collimator/experimental/acausal/component_library/mech.py
+Filename: collimator/experimental/acausal/component_library/rotational.py
+Comment: 
+
+Filename: collimator/experimental/acausal/component_library/translational.py
+Comment: 
+
+Filename: collimator/experimental/acausal2/__init__.py
+Comment: 
+
+Filename: collimator/experimental/acausal2/acausal_compiler.py
+Comment: 
+
+Filename: collimator/experimental/acausal2/acausal_system.py
+Comment: 
+
+Filename: collimator/experimental/acausal2/diagram_processing.py
+Comment: 
+
+Filename: collimator/experimental/acausal2/phleaf_generator.py
+Comment: 
+
+Filename: collimator/experimental/acausal2/run_examples.py
+Comment: 
+
+Filename: collimator/experimental/acausal2/run_index_reduction_examples.py
+Comment: 
+
+Filename: collimator/experimental/acausal2/run_regression.py
+Comment: 
+
+Filename: collimator/experimental/acausal2/sandbox.py
+Comment: 
+
+Filename: collimator/experimental/acausal2/component_library/__init__.py
+Comment: 
+
+Filename: collimator/experimental/acausal2/component_library/base.py
+Comment: 
+
+Filename: collimator/experimental/acausal2/component_library/cross_domain.py
+Comment: 
+
+Filename: collimator/experimental/acausal2/component_library/elec.py
+Comment: 
+
+Filename: collimator/experimental/acausal2/component_library/fluid_i.py
+Comment: 
+
+Filename: collimator/experimental/acausal2/component_library/rotational.py
+Comment: 
+
+Filename: collimator/experimental/acausal2/component_library/thermal.py
+Comment: 
+
+Filename: collimator/experimental/acausal2/component_library/translational.py
+Comment: 
+
+Filename: collimator/experimental/acausal2/index_reduction/__init__.py
+Comment: 
+
+Filename: collimator/experimental/acausal2/index_reduction/equation_utils.py
+Comment: 
+
+Filename: collimator/experimental/acausal2/index_reduction/ex_Mattson.py
+Comment: 
+
+Filename: collimator/experimental/acausal2/index_reduction/ex_exothermic_reactor.py
+Comment: 
+
+Filename: collimator/experimental/acausal2/index_reduction/ex_pendulum.py
+Comment: 
+
+Filename: collimator/experimental/acausal2/index_reduction/ex_pendulum_solve.py
+Comment: 
+
+Filename: collimator/experimental/acausal2/index_reduction/graph_utils.py
+Comment: 
+
+Filename: collimator/experimental/acausal2/index_reduction/index_reduction.py
+Comment: 
+
+Filename: collimator/experimental/acausal2/index_reduction/archive/__init__.py
+Comment: 
+
+Filename: collimator/experimental/acausal2/index_reduction/archive/dummy_derivative_Mattsson.py
+Comment: 
+
+Filename: collimator/experimental/acausal2/index_reduction/archive/index_reduction.py
+Comment: 
+
+Filename: collimator/experimental/acausal2/index_reduction/archive/mech_oscillator.py
+Comment: 
+
+Filename: collimator/experimental/acausal2/index_reduction/archive/pendulum.py
 Comment: 
 
 Filename: collimator/framework/__init__.py
 Comment: 
 
 Filename: collimator/framework/cache.py
 Comment: 
@@ -186,14 +285,17 @@
 
 Filename: collimator/library/ansys.py
 Comment: 
 
 Filename: collimator/library/battery_cell.py
 Comment: 
 
+Filename: collimator/library/costs_and_losses.py
+Comment: 
+
 Filename: collimator/library/custom.py
 Comment: 
 
 Filename: collimator/library/data_source.py
 Comment: 
 
 Filename: collimator/library/fmu_import.py
@@ -216,20 +318,26 @@
 
 Filename: collimator/library/predictor.py
 Comment: 
 
 Filename: collimator/library/primitives.py
 Comment: 
 
+Filename: collimator/library/quanser.py
+Comment: 
+
 Filename: collimator/library/random.py
 Comment: 
 
 Filename: collimator/library/reference_subdiagram.py
 Comment: 
 
+Filename: collimator/library/ros2.py
+Comment: 
+
 Filename: collimator/library/rotations.py
 Comment: 
 
 Filename: collimator/library/sindy.py
 Comment: 
 
 Filename: collimator/library/state_machine.py
@@ -288,14 +396,17 @@
 
 Filename: collimator/library/state_estimators/utils.py
 Comment: 
 
 Filename: collimator/library/utils/__init__.py
 Comment: 
 
+Filename: collimator/library/utils/csv_utils.py
+Comment: 
+
 Filename: collimator/library/utils/plant_utils.py
 Comment: 
 
 Filename: collimator/library/utils/rk4_utils.py
 Comment: 
 
 Filename: collimator/models/__init__.py
@@ -366,29 +477,29 @@
 
 Filename: collimator/simulation/simulator.py
 Comment: 
 
 Filename: collimator/simulation/types.py
 Comment: 
 
-Filename: pycollimator-2.0.3.dist-info/LICENSE.header.txt
+Filename: pycollimator-2.0.4.dist-info/LICENSE.header.txt
 Comment: 
 
-Filename: pycollimator-2.0.3.dist-info/LICENSE.md
+Filename: pycollimator-2.0.4.dist-info/LICENSE.md
 Comment: 
 
-Filename: pycollimator-2.0.3.dist-info/METADATA
+Filename: pycollimator-2.0.4.dist-info/METADATA
 Comment: 
 
-Filename: pycollimator-2.0.3.dist-info/WHEEL
+Filename: pycollimator-2.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: pycollimator-2.0.3.dist-info/entry_points.txt
+Filename: pycollimator-2.0.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: pycollimator-2.0.3.dist-info/top_level.txt
+Filename: pycollimator-2.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: pycollimator-2.0.3.dist-info/RECORD
+Filename: pycollimator-2.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## collimator/__init__.py

```diff
@@ -12,29 +12,30 @@
 
 import os
 
 from . import logging
 from .framework import (
     LeafSystem,
     DiagramBuilder,
+    Parameter,
 )
 from .backend import dispatcher as backend
 
 from .library.nmpc import trajopt
 from .library.linear_system import linearize
 
 from .simulation import (
     Simulator,
     simulate,
     estimate_max_major_steps,
     ODESolver,
     ODESolverOptions,
     SimulatorOptions,
 )
-from .cli import load_model
+from .cli import load_model, load_model_from_dir
 from .version import __version__
 
 _log_level = os.environ.get("LOG_LEVEL", "INFO")
 logging.set_log_level(_log_level)
 logging.set_stream_handler()
 
 _per_package_log_levels = os.environ.get("LOG_LEVELS", None)
@@ -45,21 +46,23 @@
         logging.set_log_level(level, pkg=pkg)
 
 set_backend = backend.set_backend
 
 __all__ = [
     "__version__",
     "load_model",
+    "load_model_from_dir",
     "linearize",
     "LeafSystem",
     "DiagramBuilder",
     "Simulator",
     "SimulatorOptions",
     "simulate",
     "trajopt",
     "estimate_max_major_steps",
     "ODESolver",
     "SimulatorOptions",
     "ODESolverOptions",
     "backend",
     "set_backend",
+    "Parameter",
 ]
```

## collimator/version.py

```diff
@@ -13,8 +13,8 @@
 """collimator version information."""
 
 # Keep in sync with pyproject.toml
 # Carefully bump version number based on changes:
 # add .alphaN to prepublish alpha releases
 # minor update for major new features
 # major update shouldn't happen for now
-__version__ = "2.0.3"
+__version__ = "2.0.4"
```

## collimator/backend/backend.py

```diff
@@ -45,15 +45,15 @@
         "jax": _make_backend("JaxBackend", jax_functions, jax_constants),
         "torch": _make_backend("TorchBackend", torch_functions, torch_constants),
         "numpy": _make_backend("NumpyBackend", numpy_functions, numpy_constants),
     }
 
     def __init__(self) -> None:
         # FIXME can't switch to 32 bits after init
-        enable_x64 = os.environ.get('JAX_ENABLE_X64', 'true').lower() != 'false'
+        enable_x64 = os.environ.get("JAX_ENABLE_X64", "true").lower() != "false"
         jax.config.update("jax_enable_x64", enable_x64)
         self._disable_x64 = not enable_x64
 
     @property
     def active_backend(self) -> str:
         return self._active_backend
 
@@ -118,20 +118,27 @@
 io_callback = dispatcher.function("io_callback")
 pure_callback = dispatcher.function("pure_callback")
 Rotation = dispatcher.Rotation
 
 ODESolver = dispatcher.function("ODESolver")
 
 
-# Inherits docstring from AbstractResultsData
 @register_pytree_node_class
-class ResultsData(AbstractResultsData):
+class ResultsData:
     def __init__(self, solution_data: AbstractResultsData):
         self._solution_data = solution_data
 
+    @property
+    def time(self):
+        return self._solution_data.time
+
+    @property
+    def outputs(self):
+        return self._solution_data.outputs
+
     @staticmethod
     def initialize(*args, **kwargs) -> ResultsData:
         solution = dispatcher.ResultsDataImpl.initialize(*args, **kwargs)
         return ResultsData(solution)
 
     def update(self, *args, **kwargs) -> ResultsData:
         solution = self._solution_data.update(*args, **kwargs)
```

## collimator/backend/ode_solver.py

```diff
@@ -43,15 +43,15 @@
 
 
 @dataclasses.dataclass
 class ODESolverState(metaclass=abc.ABCMeta):
     y: Array  # The current state of the system.
     t: float
     # `f` is the time derivative of `y` at `(y,, t)`.
-    f: Array
+    f: Array  # FIXME: Not needed for BDF... so this isn't a general interface.
     # The current step size.  The next step will `dt`, clipped to the interval
     # [0, tf - t].
     dt: float
     # The previous step time.  The interpolant is valid between (t_prev, t).
     t_prev: float = None
 
     @abc.abstractmethod
```

## collimator/backend/utils.py

```diff
@@ -14,15 +14,17 @@
 from .typing import (
     Array,
     DTypeLike,
     ShapeLike,
 )
 
 
-def make_array(default_value: Array, dtype: DTypeLike = None, shape: ShapeLike = None) -> Array:
+def make_array(
+    default_value: Array, dtype: DTypeLike = None, shape: ShapeLike = None
+) -> Array:
     assert not (
         shape is None and default_value is None
     ), "Must provide either shape or default_value"
 
     if default_value is not None:
         default_value = cnp.array(default_value, dtype=dtype)
     else:
```

## collimator/backend/_jax/dopri5.py

```diff
@@ -13,32 +13,28 @@
 """JAX-based Dormand-Prince ODE integration with adaptive stepsize.
 
 Modified from the built-in JAX `odeint` function:
 https://github.com/google/jax/blob/main/jax/experimental/ode.py
 
 This version is modified to return a dense interpolant as well as the time points.
 """
+
 from __future__ import annotations
 import dataclasses
 from typing import TYPE_CHECKING, Callable
 from functools import partial
 
 import jax
 import jax.numpy as jnp
 from jax import lax
-from jax._src.numpy.util import promote_dtypes_inexact
-from jax.flatten_util import ravel_pytree
-from jax.experimental.ode import map, ravel_first_arg
-import equinox as eqx
 
-from ..ode_solver import ODESolverBase, ODESolverState
+from .ode_solver_impl import ODESolverImpl, ODESolverState
 from ..typing import Array
 
 if TYPE_CHECKING:
-    from ...framework import ContextBase
     from ...framework.state import StateComponent
 
 __all__ = [
     "Dopri5State",
     "Dopri5Solver",
 ]
 
@@ -126,46 +122,14 @@
 
     y1 = dt.astype(f0.dtype) * jnp.dot(c_sol, k) + y0
     y1_error = dt.astype(f0.dtype) * jnp.dot(c_error, k)
     f1 = k[-1]
     return y1, f1, y1_error, k
 
 
-def abs2(x):
-    if jnp.iscomplexobj(x):
-        return x.real**2 + x.imag**2
-    else:
-        return x**2
-
-
-@jax.tree_util.register_pytree_node_class
-@dataclasses.dataclass
-class Interpolant:
-    ts: jnp.ndarray
-    coeffs: jnp.ndarray
-    unravel: Callable
-    max_idx: int
-
-    def evaluate(self, t):
-        idx = jnp.maximum(1, jnp.searchsorted(self.ts, t))
-        idx = jnp.minimum(idx, self.max_idx)
-        last_t = self.ts[idx - 1]
-        relative_output_time = (t - last_t) / (self.ts[idx] - last_t)
-        return self.unravel(jnp.polyval(self.coeffs[idx], relative_output_time))
-
-    def tree_flatten(self):
-        return (self.ts, self.coeffs, self.max_idx), (self.unravel)
-
-    @classmethod
-    def tree_unflatten(cls, aux_data, children):
-        ts, coeffs, max_idx = children
-        unravel = aux_data
-        return cls(ts, coeffs, unravel=unravel, max_idx=max_idx)
-
-
 @dataclasses.dataclass
 class Dopri5State(ODESolverState):
     # `t_return` is the time value to return in time series.  Will be inf when
     # the end time is reached.  Otherwise it should match `t`.
     t_return: float = None
     interp_coeff: Array = None  # Current dense interpolation coefficients
     n_acc: int = 0  # Number of accepted steps
@@ -223,19 +187,20 @@
             self.t,
             self.interp_coeff,
             self.n_acc,
             self.n_rej + 1,
             False,
         ]
         return Dopri5State(
-            *map(partial(jnp.where, (error_ratio <= 1.0)), new, old), self.unravel
+            *jax.tree.map(partial(jnp.where, (error_ratio <= 1.0)), new, old),
+            self.unravel,
         )
 
     @property
-    def rk_step_variables(self):
+    def step_variables(self):
         return self.y, self.f, self.t, self.dt
 
     @property
     def return_variables(self):
         return self.t_return, self.y, self.interp_coeff
 
     def tree_flatten(self):
@@ -263,136 +228,37 @@
 jax.tree_util.register_pytree_node(
     Dopri5State,
     lambda state: state.tree_flatten(),
     Dopri5State.tree_unflatten,
 )
 
 
-class Dopri5Solver(ODESolverBase):
+class Dopri5Solver(ODESolverImpl):
     """JAX-based Dormand-Prince (4)5 ODE integration with adaptive stepsize.
 
     Modified from the built-in JAX `odeint` function:
     https://github.com/google/jax/blob/main/jax/experimental/ode.py
 
     This version is modified to return a dense interpolant as well as the time points.
     It is also modified to work with `SystemBase` and `ContextBase` objects instead of
     raw arrays and functions.
     """
 
-    def _finalize(self):
-        self.hmin = self.min_step_size or 0.0
-        self.hmax = self.max_step_size or jnp.inf
-        self.initialize = self._override_initialize_vjp()
-
-    def initialize(self, context: ContextBase, dt: float = None) -> Dopri5State:
-        # The abstract base class requires an implementation of this method.
-        # However, in order to provide a custom VJP definition, the class will
-        # override this method with a custom VJP definition in `_override_initialize_vjp`.
-        # Hence, this is a dummy implementation that should never actually be called.
-        raise RuntimeError(
-            "Default method should have been overridden in __post_init__"
-        )
-
-    # Inherits docstring from `ODESolverBase`
-    def _initialize(self, context: ContextBase, dt: float = None) -> Dopri5State:
-        xc0 = context.continuous_state
-        t0 = context.time
-        xc0, unravel = ravel_pytree(xc0)
-        self.flat_ode_rhs = ravel_first_arg(self.ode_rhs, unravel)
-
+    def _initialize_state(self, func, t0, xc0, unravel, *args, dt=None):
         # Initialize the solver state.
-        f0 = self.flat_ode_rhs(xc0, t0, context)
+        order = 4
+        f0 = func(xc0, t0, *args)
         if dt is None:
-            dt = self.initial_step_size(self.flat_ode_rhs, xc0, t0, 4, f0, context)
+            dt = self.initial_step_size(func, xc0, t0, order, f0, *args)
         return Dopri5State(xc0, t0, f0, dt, unravel=unravel)
 
-    def _override_initialize_vjp(self):
-        if not self.enable_autodiff:
-            return self._initialize
-
-        def _wrapped_initialize(self: Dopri5Solver, context, dt=None):
-            return self._initialize(context, dt=dt)
-
-        def _wrapped_initialize_fwd(self: Dopri5Solver, context, dt):
-            # Need to correctly initialize the time step if it is not
-            # provided.  This is probably not the most efficient
-            # implementation, since it results in multiple call sites
-            # to the RHS evaluation.  However, it will not typically end
-            # up in the JIT computation graph unless differentiating through
-            # reset maps. From some simple timing, the overhead seems to be pretty
-            # minimal, at least.
-
-            if dt is None:
-                state = self._initialize(context, dt)
-                dt = state.dt
-
-            primals, vjp_fun = jax.vjp(partial(self._initialize, dt=dt), context)
-            residuals = (vjp_fun,)
-            return primals, residuals
-
-        def _wrapped_initialize_adj(self, dt, residuals, adjoints):
-            (vjp_fun,) = residuals
-            (context_adj,) = vjp_fun(adjoints)
-            return (context_adj,)
-
-        initialize = jax.custom_vjp(_wrapped_initialize, nondiff_argnums=(0, 2))
-        initialize.defvjp(_wrapped_initialize_fwd, _wrapped_initialize_adj)
-
-        # Copy docstring and type hints
-        initialize.__doc__ = super().initialize.__doc__
-        initialize.__annotations__ = self._initialize.__annotations__
-
-        return partial(initialize, self)
-
-    def initialize_adjoint(self, func, init_adj_state, tf, context):
-        """Initialize the solver configured for the adjoint reverse-time solve."""
-
-        def adj_dynamics(aug_state, neg_t, context):
-            """Original system augmented with vjp_y, vjp_t and vjp_args."""
-            y, y_bar, *_ = aug_state
-            # `neg_t` here is negative time, so we need to negate again to get back to
-            # normal time.  The VJP is filtered to only differentiable arguments
-            y_dot, vjpfun = eqx.filter_vjp(func, y, -neg_t, context)
-            return (-y_dot, *vjpfun(y_bar))
-
-        init_adj_state, unravel = ravel_pytree(init_adj_state)
-        adj_dynamics = ravel_first_arg(adj_dynamics, unravel)
-        f0 = adj_dynamics(init_adj_state, -tf, context)
-        dt = self.initial_step_size(adj_dynamics, init_adj_state, -tf, 4, f0, context)
-        return Dopri5State(init_adj_state, -tf, f0, dt, unravel=unravel), adj_dynamics
-
-    def initial_step_size(self, fun, y0, t0, order, f0, *args):
-        # Algorithm from:
-        # E. Hairer, S. P. Norsett G. Wanner,
-        # Solving Ordinary Differential Equations I: Nonstiff Problems, Sec. II.4.
-        y0, f0 = promote_dtypes_inexact(y0, f0)
-        dtype = y0.dtype
-
-        scale = self.atol + jnp.abs(y0) * self.rtol
-        d0 = jnp.linalg.norm(y0 / scale.astype(dtype))
-        d1 = jnp.linalg.norm(f0 / scale.astype(dtype))
-
-        h0 = jnp.where((d0 < 1e-5) | (d1 < 1e-5), 1e-6, 0.01 * d0 / d1)
-        y1 = y0 + h0.astype(dtype) * f0
-        f1 = fun(y1, t0 + h0, *args)
-        d2 = jnp.linalg.norm((f1 - f0) / scale.astype(dtype)) / h0
-
-        h1 = jnp.where(
-            (d1 <= 1e-15) & (d2 <= 1e-15),
-            jnp.maximum(1e-6, h0 * 1e-3),
-            (0.01 / jnp.maximum(d1, d2)) ** (1.0 / (order + 1.0)),
-        )
-
-        dt = jnp.minimum(100.0 * h0, h1)
-        return jnp.clip(dt, a_min=self.hmin, a_max=self.hmax)
-
     def mean_error_ratio(self, error_estimate, y0, y1):
         err_tol = self.atol + self.rtol * jnp.maximum(jnp.abs(y0), jnp.abs(y1))
         err_ratio = error_estimate / err_tol.astype(error_estimate.dtype)
-        return jnp.sqrt(jnp.mean(abs2(err_ratio)))
+        return jnp.sqrt(jnp.mean(err_ratio**2))
 
     def optimal_step_size(
         self,
         last_step,
         mean_error_ratio,
         safety=0.9,
         ifactor=10.0,
@@ -407,15 +273,15 @@
         )
         next_step = jnp.where(
             mean_error_ratio == 0, last_step * ifactor, last_step * factor
         )
         return jnp.clip(next_step, a_min=self.hmin, a_max=self.hmax)
 
     def attempt_rk_step(self, func, boundary_time, solver_state):
-        y, f, t, dt = solver_state.rk_step_variables
+        y, f, t, dt = solver_state.step_variables
         dt = jnp.clip(dt, a_min=self.hmin, a_max=(boundary_time - t))
         next_y, next_f, next_y_error, k = runge_kutta_step(func, y, f, t, dt)
         next_t = t + dt
         error_ratio = self.mean_error_ratio(next_y_error, y, next_y)
         new_interp_coeff = interp_fit_dopri(y, next_y, k, dt)
         dt = self.optimal_step_size(dt, error_ratio)
         return solver_state.update(
```

## collimator/backend/_jax/ode_solver.py

```diff
@@ -6,23 +6,23 @@
 # Software Foundation, version 3. This program is distributed in the hope that it
 # will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Affero General
 # Public License for more details.  You should have received a copy of the GNU
 # Affero General Public License along with this program. If not, see
 # <https://www.gnu.org/licenses/>.
 
-"""JAX-backend ODE solvers for continuous-time simulation.
-"""
+"""JAX-backend ODE solvers for continuous-time simulation."""
 
 from __future__ import annotations
 
 import dataclasses
 from typing import TYPE_CHECKING
 
 from .dopri5 import Dopri5Solver
+from .bdf import BDFSolver
 
 from ..ode_solver import ODESolverBase, ODESolverOptions
 
 if TYPE_CHECKING:
     from collimator.framework import SystemBase
 
 __all__ = ["ODESolver"]
@@ -49,8 +49,19 @@
             The specific class will depend on the system and options.
     """
 
     if options is None:
         options = ODESolverOptions()
     options = dataclasses.asdict(options)
 
-    return Dopri5Solver(system, **options)
+    method = options.pop("method", "default")
+
+    Solver = {
+        "default": Dopri5Solver,
+        "stiff": BDFSolver,
+        "non-stiff": Dopri5Solver,
+        "rk45": Dopri5Solver,
+        "dopri5": Dopri5Solver,
+        "bdf": BDFSolver,
+    }[method.lower()]
+
+    return Solver(system, **options)
```

## collimator/backend/_jax/results_data.py

```diff
@@ -94,14 +94,15 @@
     outputs = {}
     for key, y in solution.outputs.items():
         outputs[key] = np.array(y[valid_idx])
 
     # If there is stored NumPy data in the solution, add the buffer data to it.
     if solution.np_data.time is not None:
         time = np.append(solution.np_data.time, time, axis=0)
+        solution.np_data.time = None
         for key, value in outputs.items():
             outputs[key] = np.append(solution.np_data.outputs[key], value, axis=0)
 
     return time, outputs
 
 
 @dataclasses.dataclass
@@ -167,14 +168,17 @@
         Returns:
             JaxResultsData: The updated simulation solution data.
         """
 
         # Index of the current major step in the solution data buffer.
         index = self.buffer_index
 
+        # initialize the time buffer
+        self.time = jnp.where(index == 0, jnp.full_like(self.time, jnp.inf), self.time)
+
         # In this case we only need to get the signal at the current step,
         # since there are no intermediate steps from the ODE solver.
         y = self.eval_sources(context)
 
         outputs = {
             key: self.outputs[key].at[index].set(y[key]) for key in self.source_dict
         }
@@ -187,15 +191,14 @@
 
         # If the buffer is full:
         # - dump the buffer to NumPy arrays
         # - reset the time buffer array to `inf`.  This will signal unused buffer entries.
         # - reset the buffer index
         buffer_full = buffer_index >= self.buffer_length
         io_callback(self.np_data.dump_buffer, None, buffer_full, time, outputs)
-        time = jnp.where(buffer_full, jnp.full_like(time, jnp.inf), time)
         buffer_index = jnp.where(buffer_full, 0, buffer_index)
 
         return dataclasses.replace(
             self,
             outputs=outputs,
             time=time,
             n_steps=self.n_steps + 1,
```

## collimator/cli/__init__.py

```diff
@@ -6,14 +6,15 @@
 # Software Foundation, version 3. This program is distributed in the hope that it
 # will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Affero General
 # Public License for more details.  You should have received a copy of the GNU
 # Affero General Public License along with this program. If not, see
 # <https://www.gnu.org/licenses/>.
 
-from .model_interface import load_model
+from .model_interface import load_model, load_model_from_dir
 from .cli_run import run
 
 __all__ = [
     "load_model",
+    "load_model_from_dir",
     "run",
 ]
```

## collimator/cli/model_interface.py

```diff
@@ -11,72 +11,156 @@
 # <https://www.gnu.org/licenses/>.
 
 from __future__ import annotations
 
 import glob
 import json
 import os
+import traceback
+from typing import TYPE_CHECKING, Any
 import warnings
-from typing import TYPE_CHECKING
 
 import numpy as np
 
 from collimator import logging
 from collimator.dashboard.serialization import (
     model_json,
     from_model_json,
     ui_types,
 )
 from collimator.dashboard.serialization.time_mode import (
     time_mode_node,
     time_mode_port,
     time_mode_node_with_ports,
 )
-from ..framework import Diagram, IntegerTime, SystemBase, ErrorCollector
+from ..experimental.acausal.compiler import AcausalSystem
+from ..framework import Diagram, IntegerTime, SystemBase, ErrorCollector, Parameter
 from ..simulation import SimulatorOptions, simulate
 
 if TYPE_CHECKING:
     from ..framework import ContextBase
     from ..backend.typing import Array
 
 __all__ = [
     "load_model",
+    "load_model_from_dir",
 ]
 
 
-def load_model(
-    modeldir: str = ".",
-    model: str = "model.json",
-    logsdir: str = None,
-    npydir: str = None,
-    block_overrides=None,
-    parameters: dict[str, model_json.Parameter] = None,
-) -> AppInterface:
+def load_model_from_dir(modeldir: str, model: str = "model.json"):
     # register reference submodels
     file_pattern = os.path.join(modeldir, "submodel-*-latest.json")
     submodel_files = glob.glob(file_pattern)
     for submodel_file in submodel_files:
         ref_id = os.path.basename(submodel_file).split("-")[1:-1]
         ref_id = "-".join(ref_id)
         with open(submodel_file, "r", encoding="utf-8") as f:
             submodel = model_json.Model.from_json(f.read())
             from_model_json.register_reference_submodel(ref_id, submodel)
 
     with open(os.path.join(modeldir, model), "r", encoding="utf-8") as f:
         model = model_json.Model.from_json(f.read())
 
+    return model
+
+
+def load_model(
+    modeldir: str = ".",
+    model: str = "model.json",
+    logsdir: str = None,
+    npydir: str = None,
+    block_overrides=None,
+    parameters: dict[str, model_json.Parameter] = None,
+) -> AppInterface:
+    model = load_model_from_dir(modeldir, model=model)
+
     return AppInterface(
         model,
         logsdir=logsdir,
         npydir=npydir,
         block_overrides=block_overrides,
         parameters=parameters,
     )
 
 
+def get_acausal_signal_types(
+    namepath: list[str],
+    uuidpath: list[str],
+    node: AcausalSystem,
+    context: ContextBase,
+):
+    signal_types: list[ui_types.Node] = []
+
+    # FIXME these two are quite the hack
+    cmp_to_phleaf_outport_map = node.cmp_to_phleaf_outport_map
+    acausal_diagram: from_model_json.AcausalDiagram = node.acausal_diagram
+
+    phleaf_outport_to_block_port: dict[int, tuple[str, int]] = {}
+    for block_id, outport_map in cmp_to_phleaf_outport_map.items():
+        for block_port_index, phleaf_outport_index in outport_map.items():
+            phleaf_outport_to_block_port[phleaf_outport_index] = (
+                block_id,
+                block_port_index,
+            )
+
+    phleaf_outport_values: dict[int, Any] = {}
+    phleaf_outport_tms: dict[int, ui_types.TimeMode] = {}
+    for phleaf_outport_idx, phleaf_outport in enumerate(node.output_ports):
+        val = phleaf_outport.eval(context)
+        phleaf_outport_values[phleaf_outport_idx] = val
+        phleaf_outport_tms[phleaf_outport_idx] = time_mode_port(phleaf_outport, None)
+
+    all_ports_tms = []
+    for block_id, phleaf_outport_map in cmp_to_phleaf_outport_map.items():
+        block_spec = next(
+            (blk for blk in acausal_diagram.blocks.values() if blk.uuid == block_id),
+            None,
+        )
+
+        if block_spec is None:
+            logging.error("Block with id %s not found in acausal diagram.", block_id)
+            continue
+
+        blk_namepath = namepath + [block_spec.name]
+        blk_uuidpath = uuidpath + [block_spec.uuid]
+        blk_outports = []
+        blk_port_tms = []
+
+        for block_port_index, phleaf_outport_index in phleaf_outport_map.items():
+            outport_spec: model_json.IOPort = block_spec.outputs[block_port_index]
+            val = phleaf_outport_values[phleaf_outport_index]
+
+            port_tm = phleaf_outport_tms[phleaf_outport_index]
+            all_ports_tms.append(port_tm)
+            blk_port_tms.append(port_tm)
+
+            blk_outport = ui_types.Port(
+                index=block_port_index,
+                dtype=str(np.array(val).dtype),
+                dimension=np.shape(val),
+                time_mode=port_tm,
+                discrete_interval=None,
+                name=outport_spec.name,
+            )
+            blk_outports.append(blk_outport)
+
+        blk_tm = time_mode_node_with_ports(blk_port_tms)
+        nd = ui_types.Node(
+            namepath=blk_namepath,
+            uuidpath=blk_uuidpath,
+            outports=blk_outports,
+            time_mode=blk_tm,
+            discrete_interval=None,
+        )
+        signal_types.append(nd)
+
+    tm = time_mode_node_with_ports(all_ports_tms)
+    return signal_types, tm
+
+
 def get_signal_types(
     namepath: list[str],
     uuidpath: list[str],
     signal_type_nodes: list[ui_types.Node],
     nodes: list[SystemBase],
     context: ContextBase,
     dep_graph,
@@ -84,14 +168,35 @@
     # iterate over the nested diagram and:
     #   1] determine each signal's dtype and dimension
     #   2] determine time_mode of nodes and signals
     #   3] generate the signal_types.json given to the frontend
 
     nodes_tm = []
     for node in nodes:
+        if isinstance(node, AcausalSystem):
+            try:
+                acausal_signal_types, acausal_tm = get_acausal_signal_types(
+                    namepath,
+                    uuidpath,
+                    node,
+                    context,
+                )
+                nodes_tm.append(acausal_tm)
+                signal_type_nodes.extend(acausal_signal_types)
+            except Exception as exc:
+                # Not raising an exception because this is very experimental
+                logging.error(
+                    "Failed to extract signal type information for acausal blocks in "
+                    "'%s' due to exception: %s. Signals may not be visualized and the "
+                    "coloring of the diagram may be incorrect.",
+                    ".".join(namepath) or "root",
+                    exc,
+                )
+            continue
+
         node_cls_tm = time_mode_node(node)
         blk_namepath = namepath + [node.name]
         blk_uuidpath = uuidpath + [node.ui_id]
         ports = []
 
         if isinstance(node, Diagram):
             signal_type_nodes, subdiagram_tm = get_signal_types(
@@ -106,19 +211,14 @@
         ports_tm = []
         for port_idx, out_port in enumerate(node.output_ports):
             val = out_port.eval(context)
 
             tm = time_mode_port(out_port, node_cls_tm)
             ports_tm.append(tm)
 
-            # jp's trick. 'val' may have a Python type (int or float) in which
-            # case it doesn't have a dtype. So turn it into an array and then
-            # retrive the dtype. While a Python type doesn't have a dtype,
-            # for some reason one can apply np.shape(..) to it. Go figure.
-
             # this data is returned to the UI
             port = ui_types.Port(
                 index=port_idx,
                 dtype=str(np.array(val).dtype),
                 dimension=np.shape(val),
                 time_mode=tm,
                 discrete_interval=None,
@@ -126,30 +226,30 @@
             )
             ports.append(port.__dict__)
 
         # node time mode
         if isinstance(node, Diagram):
             node_tm = subdiagram_tm
         else:
-            node_tm = time_mode_node_with_ports(node, ports_tm)
+            node_tm = time_mode_node_with_ports(ports_tm)
 
         nodes_tm.append(node_tm)
 
         # this data is returned to the UI
         nd = ui_types.Node(
             namepath=blk_namepath,
             uuidpath=blk_uuidpath,
             outports=ports,
             time_mode=node_tm,
             discrete_interval=None,
         )
         signal_type_nodes.append(nd.__dict__)
 
     # diagram time mode
-    diagram_tm = time_mode_node_with_ports(node, nodes_tm)
+    diagram_tm = time_mode_node_with_ports(nodes_tm)
 
     return signal_type_nodes, diagram_tm
 
 
 class AppInterface:
     def __init__(
         self,
@@ -230,16 +330,15 @@
             ui_id=root_id,
         )
 
         # build the model.
         # this step runs checks for:
         #   1] all inports connected
         #   2] no inports connected to multiple sources
-        #   3] no algebraic loops
-        #   4] all block "validate" functions
+        #   3] all block "validate" functions
         self.diagram = from_model_json.make_subdiagram(
             root_id,
             self.model.diagram,
             self.model.subdiagrams,
             self.model.state_machines,
             acausal_diagrams,
             ui_id=self.model.uuid,
@@ -247,14 +346,18 @@
             parent_ui_id_path=[],
             namespace_params=model_parameters,
             block_overrides=self.block_overrides,
             global_discrete_interval=self.model.configuration.sample_time,
             record_mode=self.model.configuration.record_mode,
             recorded_signals=recorded_signals,
             start_time=float(self.model.configuration.start_time),
+            model_parameters={
+                k: Parameter(name=k, value=model_parameters[k])
+                for k in self.model.parameters.keys()
+            },
         )
 
         # TODO: ensure no top level inports/outports
 
         # initialized context and verify internal consistency
         try:
             error_collector = ErrorCollector()
@@ -290,14 +393,15 @@
                 signal_types_file = os.path.join(self.logsdir, "signal_types.json")
                 signal_types = ui_types.SignalTypes(nodes=signal_type_nodes)
                 signal_types_dict = signal_types.to_api(omit_none=True)
                 with open(signal_types_file, "w", encoding="utf-8") as outfile:
                     json.dump(signal_types_dict, outfile, indent=2, sort_keys=False)
 
             except Exception as exc:
+                traceback.print_exc()
                 warnings.warn(
                     f"Failed to generate signal_types.json due to exception: {exc}."
                 )
 
         if error_collector.errors:
             # log all errors
             logging.debug("Type Errors collected during context creation:")
@@ -333,16 +437,14 @@
         while stop_time > IntegerTime.max_float_time:
             IntegerTime.set_scale(1000 * IntegerTime.time_scale)
             logging.info(
                 "Increasing integer time scale by a factor of 1000x to allow for "
                 "representation of the specified end time."
             )
 
-        print("Beginning simulation")
-
         results = simulate(
             self.diagram,
             self.context,
             (start_time, stop_time),
             options=options,
             results_options=self.results_options,
             recorded_signals=options.recorded_signals,
```

## collimator/dashboard/project.py

```diff
@@ -749,15 +749,16 @@
     body = {"ignore_cache": ignore_cache}
     if parameters:
         body["parameters"] = {}
         for p in parameters:
             if p.name is None:
                 raise ValueError("Parameter name cannot be None")
             json_param = model_json.Parameter(
-                value=p.value_as_str(), is_string=isinstance(p.value, str))
+                value=p.value_as_str(), is_string=isinstance(p.value, str)
+            )
             body["parameters"][p.name] = json_param.to_dict()
 
     summary = api.post(f"/models/{model_uuid}/simulations", body=body)
 
     # wait for simulation completion
     while summary["status"] not in ("completed", "failed"):
         await asyncio.sleep(1)
```

## collimator/dashboard/serialization/block_interface.py

```diff
@@ -6,23 +6,29 @@
 # Software Foundation, version 3. This program is distributed in the hope that it
 # will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Affero General
 # Public License for more details.  You should have received a copy of the GNU
 # Affero General Public License along with this program. If not, see
 # <https://www.gnu.org/licenses/>.
 
+import importlib
+from importlib.util import find_spec as try_import
 import inspect
 
 import numpy as np
 
 from collimator import library
 from collimator.dashboard.serialization import model_json
 import collimator.library.state_machine as sm_lib
 from collimator.logging import logger
-from collimator.experimental.acausal import component_library as phys
+from collimator.experimental.acausal.component_library import (
+    elec,
+    rotational,
+    translational,
+)
 
 """
 All of the <BlahBlock> functions should eventually be ported to
 their respective blocks class definition, e.g. in library.primitives.py
 """
 
 
@@ -182,21 +188,14 @@
         ki=Ki,
         kd=Kd,
         n=N,
         **kwargs,
     )
 
 
-def MLPBlock(file_name, model_format, **kwargs):
-    return _wrap(library.MLP)(
-        filename=file_name,
-        **kwargs,
-    )
-
-
 def DiscreteInitializerBlock(discrete_interval, initial_state, **kwargs):
     dt = kwargs.pop("dt", None)
     return _wrap(library.DiscreteInitializer)(
         initial_state=initial_state,
         dt=dt if dt is not None else discrete_interval,
         **kwargs,
     )
@@ -234,41 +233,218 @@
         seed=seed,
         shape=shape,
         dtype=dtype,
         **kwargs,
     )
 
 
+def _wrap_ros2_block(cls: type, io_ports: model_json.IOPort, **kwargs):
+    # The ROS2 blocks are very experimental and require a complex setup before use.
+    # This glue code is super hacky and intended for quick demos. We can absolutely
+    # release this and example notebooks (using the dashboard API) but we need to
+    # make it clear this is an unstable feature.
+
+    topic = kwargs.pop("topic", None)
+    msg_type = kwargs.pop("msg_type", None)
+    message_class: type = None
+
+    rclpy = try_import("rclpy")
+    geometry_msgs = try_import("geometry_msgs")
+    std_msgs = try_import("std_msgs")
+    if rclpy is None or geometry_msgs is None or std_msgs is None:
+        raise ImportError("ROS2 blocks require rclpy, geometry_msgs and std_msgs")
+
+    # FIXME/TODO: primitive types are not actually supported...
+    # if msg_type == "std_msgs/Float64":
+    #     message_class = std_msgs.msg.Float64
+    # elif msg_type == "std_msgs/Int32":
+    #     message_class = std_msgs.msg.Int32
+    # elif msg_type == "std_msgs/String":
+    #     message_class = std_msgs.msg.String
+
+    ns = ".".join(msg_type.split("/")[:-1])
+    classname = msg_type.split("/")[-1]
+    try:
+        module = importlib.import_module(ns)
+        message_class = getattr(module, classname)
+    except ImportError as e:
+        raise ImportError(f"Could not import message class {msg_type}") from e
+    except AttributeError as e:
+        raise AttributeError(f"Could not find class {msg_type} in module {ns}") from e
+
+    # FIXME: abusing port parameters to carry ros2 message field/type info
+    # A proper fix would be not to set these awkward definitions on this block
+    # but rather on a bus creator block. Note: the implementation requires
+    # use of ordered dicts where the order matches that of the I/O ports.
+    fields: dict[str, str] = {}
+    for io_port in io_ports:
+        field = io_port.parameters.get("field_name", None)
+        dtype = io_port.parameters.get("dtype", None)
+        if field is None or dtype is None:
+            raise ValueError("Field name and data type must be provided for all inputs")
+        fields[field.value] = dtype.value
+
+    return _wrap_discrete(cls)(
+        topic=topic, msg_type=message_class, fields=fields, **kwargs
+    )
+
+
+def Ros2PublisherBlock(block_spec: model_json.Node, **kwargs):
+    return _wrap_ros2_block(library.Ros2Publisher, block_spec.inputs, **kwargs)
+
+
+def Ros2SubscriberBlock(block_spec: model_json.Node, **kwargs):
+    return _wrap_ros2_block(library.Ros2Subscriber, block_spec.outputs, **kwargs)
+
+
 def WhiteNoiseBlock(discrete_interval, **kwargs):
     # Custom wrapper for some deserialization and type conversions
     corr_time = kwargs.pop("correlation_time", None)
-    noise_power = float(kwargs.pop("noise_power", 1.0))
+    noise_power = kwargs.pop("noise_power", 1.0)
     num_samples = int(kwargs.pop("num_samples", 10))
     seed = kwargs.pop("seed", None)
     shape = kwargs.pop("shape", ())
     dtype = kwargs.pop("dtype", None)
 
-    if seed is not None:
-        seed = int(seed)
-    if shape is not None:
-        shape = tuple(map(int, shape))
     if dtype is not None:
         dtype = np.dtype(dtype)
 
     return _wrap(library.WhiteNoise)(
         correlation_time=(corr_time if corr_time is not None else discrete_interval),
         noise_power=noise_power,
         num_samples=num_samples,
         seed=seed,
         shape=shape,
         dtype=dtype,
         **kwargs,
     )
 
 
+def KalmanFilterBlock(discrete_interval, **kwargs):
+    # Custom wrapper for some deserialization and type conversions
+
+    dt = kwargs.pop("dt", None)  # needed for all
+    if dt is None:
+        dt = discrete_interval
+
+    matrices_provided = kwargs.pop("matrices_provided", True)
+    use_ihkf = kwargs.pop("use_ihkf", False)
+
+    # For continuous-time plant
+    plant_submodel_uuid = kwargs.pop("plant_submodel_uuid", None)
+    discretization_method = kwargs.pop("discretization_method", "zoh")
+    x_eq = kwargs.pop("x_eq", None)
+    u_eq = kwargs.pop("u_eq", None)
+
+    # For input matrices
+    A = kwargs.pop("A")
+    B = kwargs.pop("B")
+    C = kwargs.pop("C", None)
+    D = kwargs.pop("D", None)
+
+    # For both continuous-time plant and input matrices
+    G = kwargs.pop("G", None)
+    Q = kwargs.pop("Q", None)
+    R = kwargs.pop("R", None)
+    x_hat_0 = kwargs.pop("x_hat_0", None)
+
+    # only needed if use_ihkf is False
+    P_hat_0 = kwargs.pop("P_hat_0", None)
+
+    # Convert list inputs to numpy arrays
+    if x_eq is not None:
+        x_eq = np.array(x_eq)
+    if u_eq is not None:
+        u_eq = np.array(u_eq)
+    if A is not None:
+        A = np.array(A)
+    if B is not None:
+        B = np.array(B)
+    if C is not None:
+        C = np.array(C)
+    if D is not None:
+        D = np.array(D)
+    if G is not None:
+        G = np.array(G)
+    if Q is not None:
+        Q = np.array(Q)
+    if R is not None:
+        R = np.array(R)
+    if x_hat_0 is not None:
+        x_hat_0 = np.array(x_hat_0)
+    if P_hat_0 is not None:
+        P_hat_0 = np.array(P_hat_0)
+
+    if matrices_provided:
+        if use_ihkf:
+            return _wrap(library.InfiniteHorizonKalmanFilter)(
+                dt=dt,
+                A=A,
+                B=B,
+                C=C,
+                D=D,
+                G=G,
+                Q=Q,
+                R=R,
+                x_hat_0=x_hat_0,
+                **kwargs,
+            )
+        else:
+            return _wrap(library.KalmanFilter)(
+                dt=dt,
+                A=A,
+                B=B,
+                C=C,
+                D=D,
+                G=G,
+                Q=Q,
+                R=R,
+                x_hat_0=x_hat_0,
+                P_hat_0=P_hat_0,
+                **kwargs,
+            )
+    else:
+        # NOTE: there is no way to specify custom parameters or re-run the
+        # submodel init script at this point.
+        plant = library.ReferenceSubdiagram.create_diagram(
+            plant_submodel_uuid,
+            instance_parameters={},
+            instance_name="ct_plant_for_kf",
+        )
+        if use_ihkf:
+            y_eq, kf = _wrap(library.InfiniteHorizonKalmanFilter.for_continuous_plant)(
+                plant,
+                x_eq,
+                u_eq,
+                dt,
+                G=G,
+                Q=Q,
+                R=R,
+                x_hat_bar_0=x_hat_0,
+                **kwargs,
+            )
+        else:
+            y_eq, kf = _wrap(library.KalmanFilter.for_continuous_plant)(
+                plant,
+                x_eq,
+                u_eq,
+                dt,
+                G=G,
+                Q=Q,
+                R=R,
+                x_hat_bar_0=x_hat_0,
+                P_hat_bar_0=P_hat_0,
+                discretization_method=discretization_method,
+                **kwargs,
+            )
+
+        logger.info("Kalman filter created with equilibrium state y_eq: %s", y_eq)
+        return kf
+
+
 def IOPortBlock(**kwargs):
     if "description" in kwargs:
         kwargs.pop("description")
     if "port_id" in kwargs:
         kwargs.pop("port_id")
     if "default_value" in kwargs:
         kwargs.pop("default_value")
@@ -448,15 +624,16 @@
 
 
 def _filter_init_kwargs(cls: type, kwargs: dict):
     # Filters the parameters actually accepted by __init__ of the given block
     # class. This prevents failing simulations in case of a slightly invalid
     # JSON model.
 
-    cls_init_param_defs = inspect.signature(cls.__init__).parameters
+    fn = cls.__init__ if isinstance(cls, type) else cls
+    cls_init_param_defs = inspect.signature(fn).parameters
 
     allowed_kwargs = set(["ui_id", "name"])
     cls_init_param_names = set(cls_init_param_defs.keys())
     allowed_param_names = cls_init_param_names | allowed_kwargs
 
     unsupported_kwargs = []
     new_kwargs = {}
@@ -537,14 +714,17 @@
         # image segmentation
         # image source
         "core.Inport": IOPortBlock,
         "core.Integrator": IntegratorBlock,
         "core.IntegratorDiscrete": IntegratorDiscreteBlock,
         # iterator [and its loop control blocks]
         # linearized sysyem
+        # State estimators from Kalman filter family
+        "core.KalmanFilter": KalmanFilterBlock,
+        "core.InfiniteHorizonKalmanFilter": _wrap(library.InfiniteHorizonKalmanFilter),
         "core.Log": _wrap(library.Logarithm),
         "core.LogicalOperator": _wrap(library.LogicalOperator),
         "core.LogicalReduce": _wrap(library.LogicalReduce),
         "core.LookupTable1d": _wrap(library.LookupTable1d),
         "core.LookupTable2d": _wrap(library.LookupTable2d),
         # loop blah, iterator blocks
         "core.MatrixConcatenation": _wrap_reducer(library.MatrixConcatenation),
@@ -558,35 +738,37 @@
         "core.Offset": _wrap(library.Offset),
         "core.Outport": IOPortBlock,
         "core.PID": PIDBlock,
         "core.PID_Discrete": PIDDiscreteBlock,
         "core.Power": _wrap(library.Power),
         "core.PyTorch": PyTorchBlock,
         "core.TensorFlow": TensorFlowBlock,
-        "core.MLP": MLPBlock,
+        "core.MLP": _wrap(library.MLP),
         "core.Product": _wrap_reducer(library.Product),
         "core.ProductOfElements": _wrap(library.ProductOfElements),
         "core.Pulse": _wrap(library.Pulse),
         "core.PythonScript": PythonScriptBlock,
         "core.PyTwin": PyTwinBlock,
         "core.Quantizer": _wrap(library.Quantizer),
         "core.Ramp": _wrap(library.Ramp),
         "core.RandomNumber": RandomNumberBlock,
         "core.RateLimiter": _wrap_discrete(library.RateLimiter),
         "core.Reciprocal": _wrap(library.Reciprocal),
         # "core.ReferenceSubmodel": implemented in model_interface.py
         "core.Relay": _wrap(library.Relay),
         # replicator
         "core.RigidBody": _wrap(library.RigidBody),
+        "core.Ros2Publisher": Ros2PublisherBlock,
+        "core.Ros2Subscriber": Ros2SubscriberBlock,
         "core.Saturate": _wrap(library.Saturate),
         "core.Sawtooth": _wrap(library.Sawtooth),
         "core.ScalarBroadcast": _wrap(library.ScalarBroadcast),
         "core.SignalDatatypeConversion": _wrap(library.SignalDatatypeConversion),
         "core.SineWave": _wrap(library.Sine),
-        "core.SINDy": _wrap(library.ContinuousTimeSindyWithControl),
+        "core.SINDy": _wrap(library.Sindy),
         "core.Slice": _wrap(library.Slice),
         "core.SquareRoot": _wrap(library.SquareRoot),
         "core.Stack": StackBlock,
         "core.StateMachine": StateMachineBlock,
         "core.StateSpace": StateSpaceBlock,
         "core.Step": _wrap(library.Step),
         "core.Stop": _wrap(library.Stop),
@@ -595,28 +777,40 @@
         "core.TransferFunctionDiscrete": TransferFunctionDiscreteBlock,
         "core.Trigonometric": _wrap(library.Trigonometric),
         "core.UnitDelay": _wrap_discrete(library.UnitDelay),
         # video sink
         # video source
         "core.WhiteNoise": WhiteNoiseBlock,
         "core.ZeroOrderHold": _wrap_discrete(library.ZeroOrderHold),
-        # Acausal blocks
-        "phys.elec.Capacitor": _wrap(phys.elec.ElecCapacitor),
-        "phys.elec.ConstantVoltage": _wrap(phys.elec.ElecVoltageSource),
-        "phys.elec.Reference": _wrap(phys.elec.ElecRef),
-        "phys.elec.Resistor": _wrap(phys.elec.ElecResistor),
-        "phys.elec.IdealCurrentSensor": _wrap(phys.elec.ElecCurrentSensor),
-        "phys.elec.IdealVoltageSensor": _wrap(phys.elec.ElecVoltageSensor),
-        "phys.elec.SignalVoltage": _wrap(phys.elec.ElecVoltageSourceControlled),
-        "phys.mech.rotational.ConstantTorque": _wrap(phys.mech.MechRotTorque),
-        "phys.mech.rotational.Damper": _wrap(phys.mech.MechRotDamper),
-        "phys.mech.rotational.Reference": _wrap(phys.mech.MechRotRef),
-        "phys.mech.rotational.Inertia": _wrap(phys.mech.MechRotInertia),
-        "phys.mech.rotational.Spring": _wrap(phys.mech.MechRotSpring),
-        "phys.mech.translational.ConstantForce": _wrap(phys.mech.MechTransForce),
-        "phys.mech.translational.Damper": _wrap(phys.mech.MechTransDamper),
-        "phys.mech.translational.Reference": _wrap(phys.mech.MechTransRef),
-        "phys.mech.translational.Mass": _wrap(phys.mech.MechTransMass),
-        "phys.mech.translational.Spring": _wrap(phys.mech.MechTransSpring),
+        # Acausal elec blocks
+        "acausal.elec.Capacitor": _wrap(elec.Capacitor),
+        "acausal.elec.Ground": _wrap(elec.Ground),
+        "acausal.elec.Resistor": _wrap(elec.Resistor),
+        # "acausal.elec.Inductor": _wrap(elec.Inductor),
+        "acausal.elec.CurrentSensor": _wrap(elec.CurrentSensor),
+        "acausal.elec.VoltageSensor": _wrap(elec.VoltageSensor),
+        "acausal.elec.VoltageSource": _wrap(elec.VoltageSource),
+        # "acausal.elec.CurrentSource": _wrap(elec.CurrentSource),
+        # Acausal mechRot blocks
+        "acausal.rotational.TorqueSource": _wrap(rotational.TorqueSource),
+        # "acausal.rotational.RotationalSpeedSource": _wrap(rotational.RotationalSpeedSource),
+        "acausal.rotational.Damper": _wrap(rotational.Damper),
+        "acausal.rotational.FixedAngle": _wrap(rotational.FixedAngle),
+        "acausal.rotational.Inertia": _wrap(rotational.Inertia),
+        "acausal.rotational.Spring": _wrap(rotational.Spring),
+        # "acausal.rotational.TorqueSensor": _wrap(rotational.TorqueSensor),
+        # "acausal.rotational.RotationalSpeedSensor": _wrap(rotational.RotationalSpeedSensor),
+        # Acausal mechTrans blocks
+        "acausal.translational.ForceSource": _wrap(translational.ForceSource),
+        # "acausal.translational.TranslationalSpeedSource": _wrap(translational.TranslationalSpeedSource),
+        "acausal.translational.Damper": _wrap(translational.Damper),
+        "acausal.translational.FixedPosition": _wrap(translational.FixedPosition),
+        "acausal.translational.Mass": _wrap(translational.Mass),
+        "acausal.translational.Spring": _wrap(translational.Spring),
+        # "acausal.rotational.ForceSensor": _wrap(translational.ForceSensor),
+        # "acausal.translational.TranslationalSpeedSensor": _wrap(translational.TranslationalSpeedSensor),
+        # Quanser blocks
+        "quanser.QubeServoModel": _wrap(library.quanser.QubeServoModel),
+        "quanser.QuanserHAL": _wrap_discrete(library.quanser.QuanserHAL),
     }
 
     return fcn_map[node_type]
```

## collimator/dashboard/serialization/from_model_json.py

```diff
@@ -16,18 +16,20 @@
 import traceback
 from uuid import uuid4
 
 from collimator.framework import (
     Diagram,
     DiagramBuilder,
     Parameter,
+    ParameterCache,
     SystemBase,
     SystemCallback,
     LeafSystem,
 )
+from collimator.framework.parameter import resolve_parameters
 from collimator.library import ReferenceSubdiagram
 from collimator.simulation import (
     ResultsMode,
     ResultsOptions,
     SimulatorOptions,
 )
 from collimator.experimental.acausal import Network, Compiler
@@ -37,15 +39,15 @@
 import dataclasses
 import math
 from typing import Any
 
 import jax.numpy as jnp
 import numpy as np
 
-from collimator import logging
+from collimator import backend, logging
 from collimator.framework.error import (
     BlockInitializationError,
     BlockParameterError,
     CollimatorError,
     LegacyBlockConfigurationError,
     ModelInitializationError,
     StaticError,
@@ -82,15 +84,15 @@
     results_options: ResultsOptions
     recorded_signals: dict[str, SystemCallback]
     simulator_options: SimulatorOptions = None
 
 
 @dataclasses.dataclass
 class AcausalDiagram:
-    blocks: dict[str, dict]
+    blocks: dict[str, model_json.Node]
     acausal_links: dict[str, model_json.Link]
     causal_inlinks: dict[str, model_json.Link]
     causal_outlinks: dict[str, model_json.Link]
 
 
 def loads_model(
     model_json_str: str,
@@ -113,15 +115,14 @@
     Reference submodels must be registered before calling this function.
     """
     if namespace is None:
         namespace = {}
 
     model = model_json.Model.from_dict(model_json_obj)
 
-
     model_parameters = {}
     for param_name, param in model.parameters.items():
         if param.is_string:
             model_parameters[param_name] = param.value
         else:
             value = eval_parameter(param.value, namespace, namespace)
             model_parameters[param_name] = Parameter(name=param_name, value=value)
@@ -179,15 +180,48 @@
     )
 
 
 def eval_parameter(value: str, _globals: dict, _locals: dict):
     # Block parameters can be left empty, but JSON may contain null or "None"
     if not value or value == "None":
         return None
-    p = eval(str(value), _globals, _locals)
+
+    # FIXME: These are passed correctly when called from `eval_parameters`, but
+    # not when called directly from `load_model`, so when pulling a model from the
+    # dashboard anything with `np` or `jnp` will fail.  Is there a better way to
+    # ensure these are always available in both cases?
+    _locals = {
+        **_locals,
+        "np": np,
+        "jnp": jnp,
+        "math": math,
+        "false": False,
+        "true": True,
+    }
+
+    # Resolve parameters used in the expression
+    params_in_global, _ = resolve_parameters(value, _globals)
+    params_in_local, _ = resolve_parameters(value, _locals)
+
+    parameters = params_in_global | params_in_local
+
+    # Value is a python expression that depends on parameters.
+    # We should wrap it in a Parameter object to track dependencies.
+    if len(parameters) > 0:
+        p = Parameter(
+            value=value,
+            is_python_expr=True,
+            globals_=_globals.copy(),
+            locals_=_locals.copy(),
+        )
+        for param in parameters:
+            ParameterCache.add_dependent(param, p)
+        return p
+
+    p = eval(value, _globals, _locals)
     # Rules for user-input parameters:
     # - if explicitly given as an array with dtype, use that dtype
     # - if boolean, use as given
     # - otherwise, convert to a numpy array
     if not hasattr(p, "dtype") and not isinstance(p, bool):
         p = np.array(p)
         # if the array has integer dtype convert to float. Note that
@@ -204,15 +238,15 @@
     instance_parameters: dict[str, model_json.Parameter] = None,
     call_site_namespace: dict[str, Any] = None,
     name_path: list[str] = None,
     ui_id_path: list[str] = None,
 ):
     # parameter handling.
     # at this point we have the following:
-    # 1] diagrams[block_id].default_parameters
+    # 1] diagrams[block_id].dynamic_parameters
     #   these are from the submodel-uuid-ver.json[parameter_definitions].
     #   these are the definitions and defaults for all parameters in the name space of the submodel
     # 2] instance_parameters
     #   these are the parameter values from the instance of the submodel. this must be a subset of 1]
     #   this dict is typically limited to those params which have been modified from their default value.
     #   the values of these should have been evaluated in the context of the parent of the instance.
     # 3] call_site_namespace
@@ -415,15 +449,17 @@
         logging.debug("Converting instantiated parameters to parameter definitions.")
         parameter_definitions = [
             model_json.ParameterDefinition(name=k, default_value=v.value)
             for k, v in model.parameters.items()
         ]
 
     parameters = eval_parameters(default_parameters=parameter_definitions)
-    parameters = [Parameter(name=name, value=value) for name, value in parameters.items()]
+    parameters = [
+        Parameter(name=name, value=value) for name, value in parameters.items()
+    ]
 
     ReferenceSubdiagram.register(
         _make_subdiagram_instance,
         parameter_definitions=parameters,
         ref_id=ref_id,
     )
 
@@ -442,15 +478,15 @@
     ui_id: str = None,
     namespace_params=None,
     block_overrides: dict[str, SystemBase] = None,
     record_mode: str = "selected",
     recorded_signals: dict[str, SystemCallback] = None,
     global_discrete_interval: float = 0.1,
     start_time: float = 0.0,
-    model_parameters: dict[str, model_json.Parameter] = None,
+    model_parameters: dict[str, Parameter] = None,
 ) -> Diagram:
     if namespace_params is None:
         namespace_params = {}
 
     if parent_path is None:
         parent_path = []
 
@@ -486,15 +522,20 @@
         # string as id.
         acausal_diagram_key = ".".join(["root"] + parent_ui_id_path)
         acausal_diagram = acausal_diagrams.get(acausal_diagram_key, None)
     else:
         acausal_diagram = None
     # if this canavas has an acausal diagram, produce the equivalent phleaf
     if acausal_diagram is not None:
-        phleaf, inlinks_map, outlinks_map = build_acausal_network(
+        (
+            phleaf,
+            inlinks_map,
+            outlinks_map,
+            cmp_to_phleaf_outport_map,
+        ) = build_acausal_network(
             acausal_diagram,
             namespace_params,
             name=".".join(["root"] + parent_path + ["phleaf"]),
             parent_path=parent_path,
             parent_ui_id_path=parent_ui_id_path,
         )
         blocks[phleaf.name] = phleaf
@@ -504,14 +545,15 @@
         causal_outlinks = acausal_diagram.causal_outlinks
     else:
         acausal_links = {}
         causal_inlinks = {}
         causal_outlinks = {}
         inlinks_map = {}
         outlinks_map = {}
+        cmp_to_phleaf_outport_map = {}
 
     # process causal blocks
     for block_spec in diagram.nodes:
         block: SystemBase | Diagram = None
 
         # block names are used as locally (in this canvas) unique identifiers
         block_name = block_spec.name
@@ -610,15 +652,15 @@
                     block = block_interface.get_block_fcn(block_spec.type)(
                         block_spec=block_spec,
                         discrete_interval=global_discrete_interval,
                         start_time=start_time,
                         **common_kwargs,
                         **parameters,
                     )
-                elif block_spec.type[0:5] == "phys.":
+                elif block_spec.type.startswith("acausal."):
                     # FIXME: the above condition is terrible
                     # NOTE: acausal blocks were already isolated and processed, nothing to do here.
                     # NOTE: we need to flag that the 'block' being processed is not a 'LeafSystem'
                     # to avoid further processing (only applicable to LeafSystems) being applied to it.
                     is_phealf_block = True
                 else:
                     block = block_interface.get_block_fcn(block_spec.type)(
@@ -640,19 +682,19 @@
 
             # NOTE: Here we assume that the port order is the same in the frontend and wildcat
             # Log anything with record=True
             if block_spec.outputs and recorded_signals is not None:
                 for i, port in enumerate(block_spec.outputs):
                     if port.record or record_mode == "all":
                         if is_phealf_block:
-                            if block_ui_id in outlinks_map.keys():
-                                if i in outlinks_map[block_ui_id].keys():
+                            if block_ui_id in cmp_to_phleaf_outport_map.keys():
+                                if i in cmp_to_phleaf_outport_map[block_ui_id].keys():
                                     # when the block is part of a phleaf, we map its 'recorded'
                                     # ports to the corresponding phleaf port.
-                                    port_id = outlinks_map[block_ui_id][i]
+                                    port_id = cmp_to_phleaf_outport_map[block_ui_id][i]
                                     port_path = parent_path + [block_name, port.name]
                                     port_path = ".".join(port_path)
                                     logging.debug("Recording %s", port_path)
                                     recorded_signals[port_path] = phleaf.output_ports[
                                         port_id
                                     ]
                             else:
@@ -720,15 +762,14 @@
 
         src_block_name = block_uuid_to_name[link.src.node]
         dst_block_name = block_uuid_to_name[link.dst.node]
         src_port_index = int(link.src.port)
         dst_port_index = int(link.dst.port)
 
         if acausal_diagram is not None:
-
             if link.uuid in causal_inlinks.keys():
                 dst_block_name = phleaf.name
                 dst_port_index = inlinks_map[link.dst.node][dst_port_index]
             elif link.uuid in causal_outlinks.keys():
                 src_block_name = phleaf.name
                 src_port_index = outlinks_map[link.src.node][src_port_index]
         else:
@@ -839,29 +880,29 @@
                 parent_path=block_name_path,
                 parent_ui_id_path=block_ui_id_path,
                 ui_id=block_ui_id,
                 acausal_diagrams=acausal_diagrams,
             )
 
         # branch for identifying acausal component blocks
-        elif block_spec.type[0:5] == "phys.":
+        elif block_spec.type.startswith("acausal."):
             # FIXME: the above condition is terrible
             blocks[block_ui_id] = block_spec
-            # print(f"phys block inputs: {block_spec.inputs}")
+            # print(f"acausal block inputs: {block_spec.inputs}")
             if block_spec.inputs:
                 for idx, ioport in enumerate(block_spec.inputs):
                     # FIXME, we need a more explicit way to identify explicit ports of acausal blocks
                     if ioport.variant.variant_kind is None:
                         if block_ui_id not in phleaf_input_ui_ids.keys():
                             phleaf_input_ui_ids[block_ui_id] = []
                         port_ids = phleaf_input_ui_ids[block_ui_id]
                         port_ids.append(idx)
                         phleaf_input_ui_ids[block_ui_id] = port_ids
 
-            # print(f"phys block outputs: {block_spec.outputs}")
+            # print(f"acausal block outputs: {block_spec.outputs}")
             if block_spec.outputs:
                 for idx, ioport in enumerate(block_spec.outputs):
                     # FIXME, we need a more explicit way to identify explicit ports of acausal blocks
                     if ioport.variant.variant_kind is None:
                         if block_ui_id not in phleaf_output_ui_ids.keys():
                             phleaf_output_ui_ids[block_ui_id] = []
                         port_ids = phleaf_output_ui_ids[block_ui_id]
@@ -907,19 +948,19 @@
             and not is_phleaf_output
         ):
             # when both src and dst blocks are blocks in the physical network, and neither
             # has been identified as an explicit connection to the physical network, this
             # means this link is between two acausal ports.
             acausal_links[link.uuid] = link
         elif is_phleaf_input and link.src.node not in blocks.keys():
-            # dst node is a phleaf actuator block, and the other is not an acasual block.
+            # dst node is a phleaf actuator block, and the other is not an acausal block.
             # this case can only be a causal input to the phleaf.
             causal_inlinks[link.uuid] = link
         elif is_phleaf_output and link.dst.node not in blocks.keys():
-            # src node is a phleaf sensor block, and the other is not an acasual block.
+            # src node is a phleaf sensor block, and the other is not an acausal block.
             # this case can only be a causal output from the phleaf.
             causal_outlinks[link.uuid] = link
 
     if blocks:
         acausal_diagram = AcausalDiagram(
             blocks=blocks,
             acausal_links=acausal_links,
@@ -946,14 +987,15 @@
     blocks = acausal_diagram.blocks
     links = acausal_diagram.acausal_links
     causal_inlinks = acausal_diagram.causal_inlinks
     causal_outlinks = acausal_diagram.causal_outlinks
 
     # create acausal component objects from block_specs
     uuid_to_comp = {}
+    comp_to_uuid = {}
     for block_spec in blocks.values():
         block_name_path = parent_path + [block_spec.name]
         block_ui_id_path = parent_ui_id_path + [block_spec.uuid]
         common_kwargs = {"name": block_spec.name}
         parameters = eval_parameters(
             instance_parameters=block_spec.parameters,
             call_site_namespace=namespace_params,
@@ -962,43 +1004,61 @@
         )
         comp = block_interface.get_block_fcn(block_spec.type)(
             block_spec=block_spec,
             **common_kwargs,
             **parameters,
         )
         uuid_to_comp[block_spec.uuid] = comp
+        comp_to_uuid[comp] = block_spec.uuid
 
     # create acausal Network object
     nw = Network(name=name, comp_list=uuid_to_comp.values())
 
-    # define connections in the acasual network
+    # define connections in the acausal network
     for link_uuid, link in links.items():
         cmp_a = uuid_to_comp[link.src.node]
         cmp_b = uuid_to_comp[link.dst.node]
 
         src_port_index = int(link.src.port)
         dst_port_index = int(link.dst.port)
 
+        # FIXME: this is a garnly nasty hack on top of the one below.
+        # the UI has peculiar way of recording how links are connected when
+        # they are between acausal ports (in order to deal with the any to any freedom).
+        # normally, 'src' means the round exit port, and 'dst' means the triangle
+        # entry port. but for acausal connections, this doesn't necessarily hold.
+        # there is an optional qualifier in end point (e.g. 'src') called 'port_side'.
+        # port_side overrides the src->round and dst->triangle rule, so that it becomes
+        # port_side='outputs'->round, port_side='inputs'->triangle.
+        # this means that the 'sign' of the hacky +/- index used below is controlled
+        # by the port_side field when it is present.
+        cmp_a_port_index_sign = 1
+        if link.src.port_side == "inputs":
+            cmp_a_port_index_sign = -1
+        cmp_b_port_index_sign = -1
+        if link.dst.port_side == "outputs":
+            cmp_b_port_index_sign = 1
+
         # FIXME: this is a wicked nasty hack
         # acausal components ports should really be referred to by name, but json
         # links refer to ports by src/dst+index. acausal components do not have src/dst,
         # so to differentiate here we make dst index negative, that way components can
         # use the index only to know which port is connected.
         # as such, we have to index starting at one because we cant differentiate between
         # 0 and -0.
-        cmp_a_port_idx = src_port_index + 1
-        cmp_b_port_idx = (dst_port_index + 1) * -1
+        cmp_a_port_idx = (src_port_index + 1) * cmp_a_port_index_sign
+        cmp_b_port_idx = (dst_port_index + 1) * cmp_b_port_index_sign
         port_a = cmp_a.port_idx_to_name[cmp_a_port_idx]
         port_b = cmp_b.port_idx_to_name[cmp_b_port_idx]
         nw.connect(cmp_a, port_a, cmp_b, port_b)
 
     # create an acausal compiler object, and generate the phleaf
-    AcausalCompiler = Compiler(nw)
-    phleaf, insym_to_portid, outsym_to_portid = AcausalCompiler.generate_phleaf(
-        name=name
+    compiler = Compiler(nw)
+    phleaf, insym_to_portid, outsym_to_portid = compiler.generate_phleaf(
+        name=name,
     )
 
     # create link end point remapping data so that when back in the causal diagram assembly,
     # we can remap link end points to phleaf ports instead of the acausal block ports.
     inlinks_map = {}
     for link_uuid, link in causal_inlinks.items():
         cmp = uuid_to_comp[link.dst.node]
@@ -1009,15 +1069,35 @@
     outlinks_map = {}
     for link_uuid, link in causal_outlinks.items():
         cmp = uuid_to_comp[link.src.node]
         sym = cmp.get_out_sym()
         phleaf_portid = outsym_to_portid[sym]
         outlinks_map[link.src.node] = {int(link.src.port): phleaf_portid}
 
-    return phleaf, inlinks_map, outlinks_map
+    # NOTE: not ideal, but this is only for mapping phleaf ports to the original component
+    # ports since the components or sim request would know if a port should be 'recorded'.
+
+    # {cmp_ui_id: {cmp_port_id: phleaf_port_id}}
+    cmp_to_phleaf_outport_map: dict[str, dict[int, int]] = {}
+    if outsym_to_portid is not None:
+        for sym, phleaf_port_id in outsym_to_portid.items():
+            cmp = nw.sym_to_cmp[sym]
+            cmp_ui_id = comp_to_uuid[cmp]
+            # FIXME: hardcoding '1' below means we can only handle sensor blocks
+            # with one causal output, and it must be port_id 1.
+            cmp_port_map = cmp_to_phleaf_outport_map.get(cmp_ui_id, {})
+            cmp_port_map[1] = phleaf_port_id
+            cmp_to_phleaf_outport_map[cmp_ui_id] = cmp_port_map
+
+    # save these maps for later lookups when writing signal_types.json
+    # FIXME: saving in the object is pretty hacky but way simpler than passing around
+    phleaf.acausal_diagram = acausal_diagram
+    phleaf.cmp_to_phleaf_outport_map = cmp_to_phleaf_outport_map
+
+    return phleaf, inlinks_map, outlinks_map, cmp_to_phleaf_outport_map
 
 
 def simulation_settings(
     config: model_json.Configuration, recorded_signals: dict[str, SystemCallback] = None
 ):
     sim_output_mode_lookup = {
         "auto": ResultsMode.auto,
@@ -1037,14 +1117,16 @@
         method = "stiff"
     else:
         raise ValueError(f"Unsupported solver method: {config.solver.method}")
 
     numerical_backend = config.numerical_backend or "auto"
     if numerical_backend not in ["auto", "numpy", "jax"]:
         raise ValueError(f"Unsupported numerical backend: {config.numerical_backend}")
+    if numerical_backend == "auto":
+        numerical_backend = backend.active_backend
 
     results_options = ResultsOptions(
         mode=sim_output_mode,
         max_results_interval=config.max_results_interval,
         fixed_results_interval=config.fixed_results_interval,
     )
 
@@ -1055,13 +1137,14 @@
         min_minor_step_size=config.solver.min_step,
         max_minor_step_size=config.solver.max_step,
         atol=config.solver.absolute_tolerance,
         rtol=config.solver.relative_tolerance,
         ode_solver_method=method,
         return_context=False,
         recorded_signals=recorded_signals,
+        save_time_series=recorded_signals is not None and len(recorded_signals) > 0,
     )
 
     logging.info("Simulation settings: %s", simulator_options)
     logging.info("Results settings: %s", results_options)
 
     return results_options, simulator_options
```

## collimator/dashboard/serialization/model_json.py

```diff
@@ -28,14 +28,15 @@
 
 
 @dataclass_json
 @dataclasses.dataclass
 class Port:
     node: UUID
     port: int
+    port_side: Optional[str] = None
 
 
 @dataclass_json
 @dataclasses.dataclass
 class Link:
     uuid: Optional[UUID] = None
     src: Optional[Port] = None
```

## collimator/dashboard/serialization/time_mode.py

```diff
@@ -78,15 +78,15 @@
         return TimeMode.CONTINUOUS
     elif node.__class__.__name__ in continuous_blocks:
         return TimeMode.CONTINUOUS
 
     return None
 
 
-def time_mode_node_with_ports(node, ports_tm: list[TimeMode]) -> TimeMode:
+def time_mode_node_with_ports(ports_tm: list[TimeMode]) -> TimeMode:
     # node time_mode rules for block which do not have time mode assigned based on their
     # class.
     if TimeMode.CONTINUOUS in ports_tm and TimeMode.DISCRETE in ports_tm:
         # this case is actually used for subdiagrams, and ports_tm is actaully
         # a list of the subdiagams' nodes time_modes.
         return TimeMode.HYBRID
     elif TimeMode.CONTINUOUS in ports_tm:
```

## collimator/dashboard/serialization/to_model_json.py

```diff
@@ -30,15 +30,15 @@
 )
 from collimator.framework import (
     Diagram as WildcatDiagram,
     SystemBase,
     SystemCallback,
 )
 from collimator.library import (
-    ContinuousTimeSindyWithControl,
+    Sindy,
     CustomJaxBlock,
     CustomPythonBlock,
     Demultiplexer,
     DiscreteClock,
     PIDDiscrete,
     PyTorch,
     TensorFlow,
@@ -79,24 +79,27 @@
     "Exponent",
     "FilterDiscrete",
     "Gain",
     "IfThenElse",
     "Inport",
     "Integrator",
     "IntegratorDiscrete",
+    "KalmanFilter",
+    "InfiniteHorizonKalmanFilter",
     "LogicalOperator",
     "LogicalReduce",
     "LookupTable1d",
     "LookupTable2d",
     "Log",
     "MatrixConcatenation",
     "MatrixInversion",
     "MatrixMultiplication",
     "MatrixTransposition",
     "MinMax",
+    "MLP",
     "ModelicaFMU",
     "Mux",
     "Offset",
     "Outport",
     "PID",
     "PID_Discrete",
     "Power",
@@ -167,46 +170,56 @@
 
 
 def _wc_to_cl_parameters(block: SystemBase) -> dict[str, Parameter]:
     """Parse parameters of a wildcat block to a Collimator-compatible format"""
     # Following blocks are instances of LTISystem so we want to ignore A, B, C, D
     # TFDiscrete is not an instance of LTISystem, but needs the same treatment as TF.
     if isinstance(block, PID):
-        kp = str(block.instance_parameters["kp"])
-        ki = str(block.instance_parameters["ki"])
-        kd = str(block.instance_parameters["kd"])
-        n = str(block.instance_parameters["n"])
-        initial_state = str(block.instance_parameters["initial_state"])
+        kp = str(block.dynamic_parameters["kp"])
+        ki = str(block.dynamic_parameters["ki"])
+        kd = str(block.dynamic_parameters["kd"])
+        n = str(block.dynamic_parameters["n"])
+        initial_state = str(block.dynamic_parameters["initial_state"])
         return {
             "Kp": Parameter(value=kp),
             "Ki": Parameter(value=ki),
             "Kd": Parameter(value=kd),
             "N": Parameter(value=n),
             "initial_state": Parameter(value=initial_state),
         }
     elif isinstance(block, TransferFunction) or isinstance(
         block, TransferFunctionDiscrete
     ):
-        num = str(block.instance_parameters["num"])
-        den = str(block.instance_parameters["den"])
+        num = str(block.parameters["num"])
+        den = str(block.parameters["den"])
         return {
             "numerator_coefficients": Parameter(value=num),
             "denominator_coefficients": Parameter(value=den),
         }
 
-    params = {}
+    all_parameters = []
+    if isinstance(block, WildcatDiagram):
+        if block.instance_parameters:
+            all_parameters = {
+                param_name: block.parameters[param_name]
+                for param_name in block.instance_parameters
+            }
+    else:
+        all_parameters = {**block.dynamic_parameters, **block.static_parameters}
 
-    if block.instance_parameters:
-        for k, p in block.instance_parameters.items():
+    params = {}
+    if all_parameters:
+        for k, p in all_parameters.items():
             pname = _param_name(block, k)
+            is_string = isinstance(p.value, str) and not p.is_python_expr
             # for model parameters we want to always show the value of the parameter, not its name.
             if isinstance(block, WildcatDiagram):
-                params[pname] = Parameter(value=p.value_as_str(), is_string=isinstance(p.value, str))
+                params[pname] = Parameter(value=p.value_as_str(), is_string=is_string)
             else:
-                params[pname] = Parameter(value=str(p), is_string=isinstance(p.value, str))
+                params[pname] = Parameter(value=str(p), is_string=is_string)
 
     return params
 
 
 def _wc_to_cl_ports(
     ports: list[SystemCallback], kind, params: dict = None
 ) -> list[dict]:
@@ -253,18 +266,18 @@
     elif type(node) is LTISystem:
         return "core.StateSpace"
     elif isinstance(node, WildcatDiagram):
         if node.ref_id is not None:
             return "core.ReferenceSubmodel"
         else:
             return "core.Group"
+    elif isinstance(node, Sindy):
+        return "core.SINDy"
     elif isinstance(node, CustomPythonBlock):
         return "core.PythonScript"
-    elif isinstance(node, ContinuousTimeSindyWithControl):
-        return "core.SINDy"
     elif isinstance(node, CustomJaxBlock):
         return "core.PythonScript"
     elif node.__class__.__name__ in _CL_LIBRARY:
         return f"core.{node.__class__.__name__}"
 
     return None
 
@@ -464,17 +477,15 @@
         uuid=str(uuid4()),
         links=_wc_to_cl_links(diagram, nodes) + ioports_links,
         nodes=list(nodes.values()) + ioports,
         annotations=None,
     )
     parameter_definitions = None
     if diagram.ref_id is not None:
-        params = ReferenceSubdiagram.get_parameter_definitions(
-            diagram.ref_id
-        )
+        params = ReferenceSubdiagram.get_parameter_definitions(diagram.ref_id)
         parameter_definitions = [
             ParameterDefinition(name=param.name, default_value=str(param.value))
             for param in params
         ]
 
     parameters = _wc_to_cl_parameters(diagram)
```

## collimator/experimental/acausal/__init__.py

```diff
@@ -6,14 +6,15 @@
 # Software Foundation, version 3. This program is distributed in the hope that it
 # will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Affero General
 # Public License for more details.  You should have received a copy of the GNU
 # Affero General Public License along with this program. If not, see
 # <https://www.gnu.org/licenses/>.
 
-from .compiler import Compiler
+from .compiler import Compiler, AcausalSystem
 from .network_builder import Network
 
 __all__ = [
+    "AcausalSystem",
     "Compiler",
     "Network",
 ]
```

## collimator/experimental/acausal/compiler.py

```diff
@@ -11,22 +11,34 @@
 # <https://www.gnu.org/licenses/>.
 
 import numpy as np
 from scipy.integrate import solve_ivp
 import copy
 import sympy
 from sympy import lambdify, solve, Symbol, Eq
+from typing import TYPE_CHECKING
+
 from .component_library.base import eqn
 
 # collimator imports
 # from collimator.library import *
 from collimator.framework import LeafSystem, DependencyTicket
 from collimator.backend import numpy_api as cnp
 
 
+if TYPE_CHECKING:
+    from collimator.dashboard.serialization.from_model_json import AcausalDiagram
+
+
+class AcausalSystem(LeafSystem):
+    # FIXME these two are quite the hack
+    acausal_diagram: "AcausalDiagram" = None
+    cmp_to_phleaf_outport_map: dict[str, dict[int, int]] = None
+
+
 class Compiler:
     # FIXME: needs a better name
     """
     this class does the equation solving to produce the RHS for the system.
     this class also has a *solve* method for systems resulting in ODEs.
     this is not scalable. only the make_node_sets() and add_node_eqs() can
     be used going forward.
@@ -278,15 +290,15 @@
                     eq_syms_ = eq.e.atoms()
                     if s.s in eq_syms_:
                         replace_cnt = replace_cnt + 1
                 if replace_cnt > 0:
                     self.eqs_rhs = set([eq.subs(s.s, sub_expr) for eq in self.eqs_rhs])
                 else:
                     print(
-                        f'f"no substitution options for flow var {s} with sub_expr {sub_expr}"'
+                        f"no substitution options for flow var {s} with sub_expr {sub_expr}"
                     )
                     # raise RuntimeError(
                     #     f"no substitution options for flow var {s} with sub_expr {sub_expr}"
                     # )
                     disconnected_flow_vars.add(s)
 
                 # print(f"eqs after replace flow var {s.s} with sub_expr {sub_expr}:")
@@ -809,59 +821,66 @@
         if not self.preamble_done:
             self.preamble()
 
         # INITIAL STATE AND PARAMETERS
         x0, ps = self.get_x0_ps()
 
         # LEAF SYSTEM
-        phleaf = LeafSystem(name=name)
+        phleaf = AcausalSystem(name=name)
 
         # INPUT PORTS
         # this ensure that inports of the phleaf are in the same order as
         # the 'inputs' portion of the lambdify args
         insym_to_portid = {}
         for sym in self.model.input_syms:
             idx = phleaf.declare_input_port(name=sym.name)
             insym_to_portid[sym] = idx
 
         # COMMON TO ODE AND OUTPUTS
-        # create the lambda functions input args vector.
-        # [time, states, inputs, params]
-        lambda_args = (
-            [self.t_sym.s]
-            + list(s.s for s in self.rhs_exprs.keys())
-            + self.model.input_syms
-            + list(s.s for s in self.params.keys())
-        )
+        # create the lambda functions input args tuple.
+        # (time, states, inputs, params)
+        time = self.t_sym.s
+        state = list(s.s for s in self.rhs_exprs.keys())
+        inputs = self.model.input_syms
+        params = list(s.s for s in self.params.keys())
+        lambda_args = (time, state, *inputs, *params)
 
         # CONTINUOUS STATE AND DYNAMICS
         lambdify_rhs = lambdify(
             lambda_args, list(self.rhs_exprs.values()), leaf_backend
         )
 
-        def _ode(time, state, *inputs):
+        # PARAMETERS IN CONTEXT
+        for k, v in self.params.items():
+            phleaf.declare_dynamic_parameter(str(k), v)
+
+        def _ode(time, state, *inputs, **params):
             cstate = state.continuous_state
-            return cnp.array(lambdify_rhs(time, *cstate, *inputs, *ps))
+            param_values = [params[str(k)] for k in self.params.keys()]
+            return cnp.array(lambdify_rhs(time, cstate, *inputs, *param_values))
 
         phleaf.declare_continuous_state(default_value=x0, ode=_ode)
 
         # OUTPUT PORTS
         outsym_to_portid = {}
         if self.model.num_outputs == 0:
             # if not output, output the state vector
             phleaf.declare_continuous_state_output(name=f"{phleaf.name}:output")
             outsym_to_portid = None
         else:
 
             def _make_outp_callback2(outp_expr):
                 lambdify_output = lambdify(lambda_args, outp_expr, leaf_backend)
 
-                def _output_fun(time, state, *inputs):
+                def _output_fun(time, state, *inputs, **params):
                     cstate = state.continuous_state
-                    return cnp.array(lambdify_output(time, *cstate, *inputs, *ps))
+                    param_values = [params[str(k)] for k in self.params.keys()]
+                    return cnp.array(
+                        lambdify_output(time, cstate, *inputs, *param_values)
+                    )
 
                 return _output_fun
 
             # declaring phleaf output ports in this order means that the ordering
             # 'source of truth' is self.model.output_syms which can be used to link
             # back to the acausal sensors causal port for diagram link src point remapping.
             for sym in self.model.output_syms:
```

## collimator/experimental/acausal/network_builder.py

```diff
@@ -22,35 +22,47 @@
     def __init__(self, name=None, comp_list=None, cnctn_list=None):
         self.name = "sys" if name is None else name
         self.comps = set() if comp_list is None else set(comp_list)
         self.connections = [] if cnctn_list is None else cnctn_list
         self.t_sym = sym("t", kind="var")  # symbol for time (independent variable)
         self.syms = set()
         self.eqs = set()  # accumulate equations, and remove
+        # dict[sym:cmp] needed to dereference syms to their source compnent
+        self.sym_to_cmp = {}
+        if comp_list is not None:
+            for cmp in comp_list:
+                self.add_cmp_syms(cmp)
 
     # TODO:
-    # 1] verify that each connection is between 2 ports of the same domain
+    # 1] verify that each connection is between 2 ports of the same domain. done in acausal2
     # 2] find a way to spread not-None IC of node state to other equivalent states of
-    # same node whose ICs are None
+    # same node whose ICs are None. done in acausal2
 
     def connect(self, cmp_a, port_a, cmp_b, port_b):
         # add the components
         self.comps.update(set([cmp_a, cmp_b]))
+        self.add_cmp_syms(cmp_a)
+        self.add_cmp_syms(cmp_b)
 
         # add the symbols from each component
         self.syms.update(cmp_a.syms)
         self.syms.update(cmp_b.syms)
 
         # add the equations from the components
         self.eqs.update(cmp_a.eqs)
         self.eqs.update(cmp_b.eqs)
 
         # add the connection between the components
         self.connections.append(((cmp_a, port_a), (cmp_b, port_b)))
 
+    def add_cmp_syms(self, cmp):
+        if cmp not in self.sym_to_cmp.keys():
+            for sym_ in list(cmp.syms):
+                self.sym_to_cmp[sym_] = cmp
+
     @property
     def input_syms(self):
         syms = []
         for comp in self.comps:
             sym = comp.get_in_sym()
             if sym is not None:
                 syms.append(sym)
```

## collimator/experimental/acausal/component_library/__init__.py

```diff
@@ -6,46 +6,7 @@
 # Software Foundation, version 3. This program is distributed in the hope that it
 # will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Affero General
 # Public License for more details.  You should have received a copy of the GNU
 # Affero General Public License along with this program. If not, see
 # <https://www.gnu.org/licenses/>.
 
-from .elec import (
-    ElecVoltageSource,
-    ElecResistor,
-    ElecCapacitor,
-    ElecRef,
-    ElecVoltageSourceControlled,
-    ElecVoltageSensor,
-    ElecCurrentSensor,
-)
-from .mech import (
-    MechTransMass,
-    MechTransSpring,
-    MechTransRef,
-    MechTransForce,
-    MechTransDamper,
-    MechRotTorque,
-    MechRotInertia,
-    MechRotDamper,
-    MechRotRef,
-)
-
-__all__ = [
-    "ElecVoltageSource",
-    "ElecResistor",
-    "ElecCapacitor",
-    "ElecRef",
-    "ElecVoltageSourceControlled",
-    "ElecVoltageSensor",
-    "ElecCurrentSensor",
-    "MechTransMass",
-    "MechTransSpring",
-    "MechTransRef",
-    "MechTransForce",
-    "MechTransDamper",
-    "MechRotTorque",
-    "MechRotInertia",
-    "MechRotDamper",
-    "MechRotRef",
-]
```

## collimator/experimental/acausal/component_library/elec.py

```diff
@@ -18,18 +18,27 @@
 
 MSL Pin.mo defines the I(flow), and V. We do the similar in ElecPort, but the symbols are passed in from
 the component, so we get I1, I2, V1, V2.
 
 MSL TwoPin.mo and OnePort.mo define the component I and V symbols. We do similar, but define V in Elec2Pin,
 and use the I1 from component for I.
 
-In this way, the ElecResistor and ElecCapacitor end up with essetially an analogous set of symbols, and
+In this way, the Resistor and Capacitor end up with essetially an analogous set of symbols, and
 an equivalent set of equations relative to the MSL components.
 """
 
+__all__ = [
+    "Resistor",
+    "Capacitor",
+    "Ground",
+    "VoltageSource",
+    "VoltageSensor",
+    "CurrentSensor",
+]
+
 
 class ElecPort(PortBase):
     """
     port for a electrical component to interface with others.
     """
 
     def __init__(self, name=None, V_sym=None, I_sym=None):
@@ -40,15 +49,15 @@
 
 class Elec2Pin(ComponentBase):
     """
     electrical domain component with 2 pins.
     Incomplete component.
     """
 
-    def __init__(self, name, v_der_sym=None, V_ic=None, p1="plus", p2="minus"):
+    def __init__(self, name, v_der_sym=None, V_ic=None, p1="p", p2="n"):
         self.V = sym(name + "_V", kind="var", der_sym=v_der_sym, ic=V_ic)
         self.V1 = sym(name + "_V1", kind="pot")
         self.V2 = sym(name + "_V2", kind="pot")
         self.I1 = sym(name + "_I1", kind="flow")
         self.I2 = sym(name + "_I2", kind="flow")
 
         self.ports = {
@@ -63,104 +72,94 @@
                 eqn(e=Eq(0, self.I1.s + self.I2.s)),
             ]
         )
 
         self.port_idx_to_name = {-1: p1, 1: p2}
 
 
-class ElecVoltageSource(Elec2Pin):
-    """
-    ideal constant voltage source in electrical domain
-    """
-
-    def __init__(self, name=None, voltage=1.0):
-        self.name = "ecv" if name is None else name
-        super().__init__(self.name)
-
-        self.Vparam = sym(self.name + "_Vparam", kind="param", val=voltage)
-        self.syms.add(self.Vparam)
-        self.eqs.add(eqn(e=Eq(self.V.s, self.Vparam.s)))
-
-
-class ElecVoltageSourceControlled(Elec2Pin):
+class VoltageSource(Elec2Pin):
     """
     ideal controlled voltage source in electrical domain
     """
 
-    def __init__(self, name=None):
+    def __init__(self, name=None, V=1.0, enable_voltage_port=False, **kwargs):
         self.name = "ecvc" if name is None else name
         super().__init__(self.name)
 
-        self.Vin = sym(self.name + "_Vin", kind="in")
+        if enable_voltage_port:
+            self.Vin = sym(self.name + "_Vin", kind="in")
+        else:
+            self.Vin = sym(self.name + "_Vin", kind="param", val=V)
+
         self.syms.add(self.Vin)
         self.eqs.add(eqn(e=Eq(self.V.s, self.Vin.s)))
 
 
-class ElecRef(ComponentBase):
+class Ground(ComponentBase):
     """
     *ground* reference in electrical domain
     """
 
     def __init__(self, name=None):
         self.name = "er" if name is None else name
 
         self.I = sym(self.name + "_I", kind="flow")  # noqa
         self.dV = sym(self.name + "_dV", kind="var")
         self.V = sym(self.name + "_V", kind="pot", der_sym=self.dV.s)
 
-        self.ports = {"minus": ElecPort(V_sym=self.V, I_sym=self.I)}
+        self.ports = {"p": ElecPort(V_sym=self.V, I_sym=self.I)}
         self.syms = set([self.I, self.dV, self.V])
         self.eqs = set(
             [eqn(e=Eq(0, self.dV.s)), eqn(e=Eq(0, self.V.s)), eqn(e=Eq(0, self.I.s))]
         )
 
-        self.port_idx_to_name = {-1: "minus"}
+        self.port_idx_to_name = {-1: "p"}
 
 
-class ElecResistor(Elec2Pin):
+class Resistor(Elec2Pin):
     """
     ideal resistor in electrical domain
     """
 
     def __init__(self, name=None, R=1.0):
         self.name = "er" if name is None else name
         super().__init__(self.name)
 
         if R <= 0.0:
-            raise ValueError(f"Component ElecResistor {self.name} must have R>0")
+            raise ValueError(f"Component Resistor {self.name} must have R>0")
 
         self.R = sym(self.name + "_R", kind="param", val=R)
         self.syms.add(self.R)
         self.eqs.add(eqn(e=Eq(self.V.s, self.I1.s * self.R.s)))
 
 
-class ElecCapacitor(Elec2Pin):
+class Capacitor(Elec2Pin):
     """
     ideal capacitor in electrical domain
     """
 
-    def __init__(self, name=None, C=1.0, V_ic=0.0):
+    def __init__(self, name=None, C=1.0, initial_voltage=0.0):
         self.name = "ec" if name is None else name
 
         if C <= 0.0:
-            raise ValueError(f"Component ElecCapacitor {self.name} must have C>0")
+            raise ValueError(f"Component Capacitor {self.name} must have C>0")
 
         self.dV = sym(self.name + "_dV", kind="var")
-        super().__init__(self.name, v_der_sym=self.dV.s, V_ic=V_ic)
+        super().__init__(self.name, v_der_sym=self.dV.s, V_ic=initial_voltage)
         self.C = sym(self.name + "_C", kind="param", val=C)
         self.syms.update(set([self.C, self.dV]))
         self.eqs.add(eqn(e=Eq(self.I1.s, self.C.s * self.dV.s)))
 
 
-class ElecVoltageSensor(ComponentBase):
+class VoltageSensor(ComponentBase):
     """
     ideal voltage sensor in electrical domain
     """
 
-    def __init__(self, name=None, p1="plus", p2="minus"):
+    def __init__(self, name=None, p1="p", p2="n"):
         self.name = "evs" if name is None else name
         self.Vout = sym(self.name + "_Vout", kind="out")
         self.V1 = sym(self.name + "_V1", kind="pot")
         self.V2 = sym(self.name + "_V2", kind="pot")
 
         self.ports = {
             p1: ElecPort(V_sym=self.V1),
@@ -177,22 +176,22 @@
         # although the UI shows this block with 2 ports on the left side
         # here the causal port (the voltage input) is defined using the
         # Vout variable and its corresponding equation. So this map only
         # needs toie two acaual ports.
         self.port_idx_to_name = {-1: p1, 1: p2}
 
 
-class ElecCurrentSensor(ComponentBase):
+class CurrentSensor(ComponentBase):
     """
     ideal current sensor in electrical domain
     """
 
     # FIXME: this may need potential variables V1 and V2.
 
-    def __init__(self, name=None, p1="plus", p2="minus"):
+    def __init__(self, name=None, p1="p", p2="n"):
         self.name = "evs" if name is None else name
         self.Iout = sym(self.name + "_Iout", kind="out")
         self.I1 = sym(self.name + "_I1", kind="pot")
         self.I2 = sym(self.name + "_I2", kind="pot")
 
         self.ports = {
             p1: ElecPort(I_sym=self.I1),
@@ -208,59 +207,7 @@
         )
 
         # although the UI shows this block with 2 ports on the left side
         # here the causal port (the voltage input) is defined using the
         # Vout variable and its corresponding equation. So this map only
         # needs toie two acaual ports.
         self.port_idx_to_name = {-1: p1, 1: p2}
-
-
-# class ElecMotor(MechRotOnePort, Elec2Pin):
-class ElecMotor:
-    """
-    ideal DC electric motor
-    """
-
-    # FIXME how do properly inherit from 2 classes?
-
-    def __init__(self, name=None, Kt=1.0, Kv=1e-3, R=0.1):
-        self.name = "motor" if name is None else name
-        # MechRotOnePort.__init__(self, self.name, p="pm")
-        # print(f"self.ports={self.ports}")
-        # Elec2Pin.__init__(self, self.name, p1="pe1", p2="pe2")
-        # # super(ElecMotor, self).__init__()
-        # print(f"self.ports={self.ports}")
-        # print(f"self.syms={self.syms}")
-        # print(f"self.eqs={self.eqs}")
-
-        # self.Kt = sym(name + "_Kt", kind="param", val=Kt)
-        # self.Kv = sym(name + "_Kv", kind="param", val=Kv)
-        # self.R = sym(name + "_R", kind="param", val=R)
-
-        # self.t = sym(name + "_t", kind="flow")
-        # self.alpha = sym(name + "_alpha", kind="var")
-        # self.w = sym(name + "_w", kind="pot", der_sym=self.alpha.s, ic=0)
-        # self.ang = sym(name + "_ang", kind="var", der_sym=self.w.s, ic=0)
-
-        # self.ports["pm"] = MechRotPort(w_sym=self.w, t_sym=self.t)
-
-        # self.syms.update(
-        #     [self.t, self.alpha, self.w, self.ang, self.Kt, self.Kv, self.R]
-        # )
-
-        # print(f"\nself.ports={self.ports}")
-        # print(f"self.syms={self.syms}")
-        # print(f"self.eqs={self.eqs}")
-
-        # # toqrue = Kt*current
-        # self.eqs.add(eqn(e=Eq(self.t.s, self.Kt.s * self.I1.s)))
-        # # backEMF = v1-v2 = Kv*speed
-        # self.eqs.add(
-        #     eqn(
-        #         e=Eq(
-        #             (self.V1.s - self.V2.s) - (self.Kv.s * self.w.s),
-        #             self.I1.s * self.R.s,
-        #         )
-        #     )
-        # )
-
-        # print(f"self.eqs={self.eqs}")
```

## collimator/framework/__init__.py

```diff
@@ -29,15 +29,15 @@
     is_event_data,
 )
 
 from .cache import (
     SystemCallback,
 )
 
-from .system_base import SystemBase
+from .system_base import SystemBase, parameters
 from .leaf_system import LeafSystem
 from .diagram_builder import DiagramBuilder
 from .diagram import Diagram
 from .parameter import Parameter, ParameterCache
 from .error import (
     CollimatorError,
     StaticError,
@@ -85,8 +85,9 @@
     "BlockParameterError",
     "BlockRuntimeError",
     "ErrorCollector",
     "Parameter",
     "ParameterCache",
     "DependencyTicket",
     "next_dependency_ticket",
+    "parameters",
 ]
```

## collimator/framework/context.py

```diff
@@ -82,14 +82,15 @@
     "DiagramContext",
 ]
 
 
 def _make_globals(env):
     import numpy as np
     import jax.numpy as jnp
+
     _globals = {
         "np": np,
         "jnp": jnp,
     }
 
     if env is not None:
         _globals.update(env)
@@ -208,20 +209,22 @@
 
     @abc.abstractmethod
     def with_parameter(self, name: str, value: Parameter | ArrayLike) -> ContextBase:
         """Create a copy of this context, replacing the specified parameter."""
         pass
 
     @abc.abstractmethod
-    def with_parameters(self, new_parameters: Mapping[str, Parameter | ArrayLike]) -> ContextBase:
+    def with_parameters(
+        self, new_parameters: Mapping[str, Parameter | ArrayLike]
+    ) -> ContextBase:
         """Create a copy of this context, replacing only the specified parameters."""
         pass
 
     def _replace_param(self, name: str, value: ArrayLike):
-        param = self.owning_system.default_parameters[name]
+        param = self.owning_system.dynamic_parameters[name]
         param.set(value)
         self.parameters[name] = param.get()
 
 
 @dataclasses.dataclass(frozen=True)
 class LeafContext(ContextBase):
     state: LeafState = None
@@ -444,33 +447,34 @@
             )
         return dataclasses.replace(self, subcontexts=new_subcontexts)
 
     def _compute_params(self):
         new_subcontexts = self.subcontexts.copy()
         for system_id, subctx in self.subcontexts.items():
             parameters = subctx.parameters
-            for name, param in subctx.owning_system.default_parameters.items():
+            for name, param in subctx.owning_system.dynamic_parameters.items():
                 parameters[name] = param.get()
-            new_subcontexts[system_id] = subctx.with_parameters(parameters)
         return new_subcontexts
 
     def with_parameter(self, name: str, value: ArrayLike) -> ContextBase:
         """Create a copy of this context, replacing the specified parameter."""
         self._replace_param(name, value)
         new_subcontexts = self._compute_params()
         return dataclasses.replace(
-            self, parameters=self.parameters, subcontexts=new_subcontexts)
+            self, parameters=self.parameters, subcontexts=new_subcontexts
+        )
 
     def with_parameters(self, new_parameters: Mapping[str, ArrayLike]) -> ContextBase:
         """Create a copy of this context, replacing only the specified parameters."""
         for name, value in new_parameters.items():
             self._replace_param(name, value)
         new_subcontexts = self._compute_params()
         return dataclasses.replace(
-            self, parameters=self.parameters, subcontexts=new_subcontexts)
+            self, parameters=self.parameters, subcontexts=new_subcontexts
+        )
 
 
 #
 # Register as custom pytree nodes
 #    https://jax.readthedocs.io/en/latest/pytrees.html#extending-pytrees
 #
 # Even though this is a JAX utility, it can also be useful for generally working
```

## collimator/framework/context_factory.py

```diff
@@ -88,15 +88,15 @@
         if check_types:
             self.check_types(ctx, error_collector=error_collector)
 
         ctx = ctx.mark_initialized()
         return ctx
 
     @abc.abstractmethod
-    def create_node_context(self, env: dict = None) -> ContextBase:
+    def create_node_context(self) -> ContextBase:
         """Create a generic context for this system
 
         This will not perform any type checking or static analysis, but does initialize
         state and parameters, cache, etc.
 
         Returns:
             The created node context.
@@ -163,53 +163,68 @@
 class LeafContextFactory(ContextFactory):
     """ContextFactory for leaf systems."""
 
     # Inherit docstring from ContextFactory
     def create_node_context(self) -> LeafContext:
         system: LeafSystem = self.system
 
-        logger.debug(f"Creating cache entries for {system.callbacks}")
-
-        parameters = {}
-        for name, param in system.default_parameters.items():
-            parameters[name] = param.get()
+        try:
+            system.initialize(**system.parameters)
+        except BaseException as exc:
+            raise StaticError(system=system) from exc
+
+        # Make sure the child system has a dependency graph so that we can
+        # subscribe trackers to its ports and callbacks.  If the system already
+        # has a dependency graph, this will do nothing.
+        system.create_dependency_graph()
+
+        dynamic_parameters = {}
+        for name, param in system.dynamic_parameters.items():
+            dynamic_parameters[name] = param.get()
 
         state = system.create_state()
-        logger.debug(f"Created state {state} and parameters {parameters} for {system.name}")
+
+        logger.debug(
+            f"Created state {state} and parameters {system.parameters} for {system.name}"
+        )
 
         return LeafContext(
             owning_system=system,
             state=state,
-            parameters=parameters,
+            parameters=dynamic_parameters,
         )
 
 
 class DiagramContextFactory(ContextFactory):
     """ContextFactory for diagram systems."""
 
     # Inherit docstring from ContextFactory
     def create_node_context(self) -> DiagramContext:
         system: Diagram = self.system
 
-        parameters = {}
-        for name, param in system.default_parameters.items():
-            parameters[name] = param.get()
-
         subcontext_nodes = [
-            sys.context_factory.create_node_context()
-            for sys in system.nodes
+            sys.context_factory.create_node_context() for sys in system.nodes
         ]
 
+        system.check_no_algebraic_loops()
+
+        # Create the dependency graph for the diagram
+        system.create_dependency_graph()
+
         subcontexts = OrderedDict()
         for ctx in subcontext_nodes:
             if isinstance(ctx, DiagramContext):
                 subcontexts.update(ctx.subcontexts)
             else:
                 subcontexts[ctx.owning_system.system_id] = ctx
 
+        parameters = {}
+        for name, param in system.parameters.items():
+            parameters[name] = param.get()
+
         return DiagramContext(
             owning_system=system,
             subcontexts=subcontexts,
             parameters=parameters,
         )
 
     # Inherit docstring from ContextFactory
```

## collimator/framework/diagram.py

```diff
@@ -32,37 +32,57 @@
     Hashable,
     Iterator,
 )
 from collections import OrderedDict
 
 from ..logging import logger
 from .event import DiagramEventCollection, FlatEventCollection
-from .error import InputNotConnectedError
+from .error import InputNotConnectedError, StaticError
 from .system_base import SystemBase, UpstreamEvalError, next_system_id
 from .context_factory import DiagramContextFactory
 from .dependency_graph import DependencyTicket, DiagramDependencyGraphFactory
 from .parameter import Parameter
 
 if TYPE_CHECKING:
     from .error import ErrorCollector
-
+    from .port import (
+        PortBase,
+        InputPortLocator,
+        OutputPortLocator,
+        DirectedPortLocator,
+    )
 
 __all__ = [
+    "AlgebraicLoopError",
     "Diagram",
 ]
 
 if TYPE_CHECKING:
     from .cache import SystemCallback
     from .port import InputPortLocator, OutputPortLocator
     from .state import LeafState
     from .leaf_system import LeafSystem
     from .context import DiagramContext
     from ..backend.typing import Array
 
 
+class AlgebraicLoopError(StaticError):
+    def __init__(self, name: str, loop: list[DirectedPortLocator]):
+        # `loop` is a list of ports that form a cycle. From there, we can recover
+        # system, direction and index as port[0], port[1], port[2] respectively.
+        str_loop = " \u2192 ".join(
+            f"{port[0].name_path_str}.{port[1]}[{port[2]}]" for port in loop
+        )
+        super().__init__(
+            f"Algebraic loop detected in {name}: {str_loop}",
+            loop=loop,
+            system=None,  # Not applicable since this involves multiple systems
+        )
+
+
 @dataclasses.dataclass
 class Diagram(SystemBase):
     """Composite block-diagram representation of a dynamical system.
 
     A Diagram is a collection of Systems connected together to form a larger hybrid
     dynamical system. Diagrams can be nested to any depth, creating a tree-structured
     block diagram.
@@ -87,14 +107,17 @@
     connection_map: Mapping[InputPortLocator, OutputPortLocator] = dataclasses.field(
         default_factory=dict,
     )
 
     # Optional identifier for "reference diagrams"
     ref_id: str = None
 
+    # for serialization
+    instance_parameters: set[str] = dataclasses.field(default_factory=set)
+
     def __repr__(self) -> str:
         return f"{type(self).__name__}({self.name}, {len(self.nodes)} nodes)"
 
     def _pprint(self, prefix="") -> str:
         return f"{prefix}|-- {self.name}\n"
 
     def _pprint_helper(self, prefix="") -> str:
@@ -137,14 +160,19 @@
                 self.leaf_systems.extend(sys.leaf_systems)
                 # No longer need the child leaf systems, since methods using this
                 # should only be called from the top level.
                 sys.leaf_systems = None
             else:
                 self.leaf_systems.append(sys)
 
+    def post_simulation_finalize(self) -> None:
+        """Perform any post-simulation cleanup for this system."""
+        for system in self.nodes:
+            system.post_simulation_finalize()
+
     # Inherits docstrings from SystemBase
     @property
     def has_feedthrough_side_effects(self) -> bool:
         # See explanation in `SystemBase.has_feedthrough_side_effects`.
         return any(sys.has_feedthrough_side_effects for sys in self.nodes)
 
     # Inherits docstrings from SystemBase
@@ -534,18 +562,113 @@
             return _find_in_children()
 
         if self.name == path[0] and len(path) == 1:
             return self
 
         return _find_in_children()
 
-    def declare_parameter(self, name: str, parameter: Parameter) -> None:
+    def declare_dynamic_parameter(self, name: str, parameter: Parameter) -> None:
         """Declare a parameter for this system.
 
         Parameters:
             name (str): The name of the parameter.
             parameter (Parameter): The parameter object.
         """
         # Force the parameter to have the correct name, all diagram parameters
         # should be named.
         parameter.name = name
-        super().declare_parameter(name, parameter)
+        super().declare_dynamic_parameter(name, parameter)
+
+    def check_no_algebraic_loops(self):
+        """Check for algebraic loops in the diagram.
+
+        This is a more or less direct port of the Drake method
+        DiagramBuilder::ThrowIfAlgebraicLoopExists. Some comments are verbatim
+        explanations of the algorithm implemented there.
+        """
+
+        # The nodes in the graph are the input/output ports defined as part of
+        # the diagram's internal connections.  Ports that are not internally
+        # connected cannot participate in a cycle at this level, so we don't include them
+        # in the nodes set.
+        nodes: Set[PortBase] = set()
+
+        # For each `value` in `edges[key]`, the `key` directly influences `value`.
+        edges: Mapping[PortBase, Set[PortBase]] = {}
+
+        # Add the diagram's internal connections to the digraph nodes and edges
+        for input_port_locator, output_port_locator in self.connection_map.items():
+            # Directly using the port locator does not result in a unique identifier
+            # since (sys, 0) represents both input port 0 and output port 0.  Instead,
+            # use the port directly as a key, since it is a unique hashable object.
+            input_system, input_index = input_port_locator
+            input_port = input_system.input_ports[input_index]
+            logger.debug(f"Adding locator {input_port} to nodes")
+            nodes.add(input_port)
+
+            output_system, output_index = output_port_locator
+            output_port = output_system.output_ports[output_index]
+            logger.debug(f"Adding locator {output_port} to nodes")
+            nodes.add(output_port)
+
+            if output_port not in edges:
+                edges[output_port] = set()
+
+            logger.debug(f"Adding edge[{output_port}] = {input_port}")
+            edges[output_port].add(input_port)
+
+        # Add more edges based on each System's direct feedthrough.
+        # input -> output port iff there is direct feedthrough from input -> output
+        # If a feedthrough edge refers to a port not in `nodes`, omit it because ports
+        # that are not connected inside the diagram cannot participate in a cycle at
+        # the level of this diagram (higher-level diagrams will test for cycles at
+        # their level).
+        for system in self.nodes:
+            logger.debug(f"Checking feedthrough for system {system.name}")
+            for input_index, output_index in system.get_feedthrough():
+                input_port = system.input_ports[input_index]
+                output_port = system.output_ports[output_index]
+                logger.debug(f"Feedthrough from {input_port} to {output_port}")
+                if input_port in nodes and output_port in nodes:
+                    if input_port not in edges:
+                        edges[input_port] = set()
+                    edges[input_port].add(output_port)
+
+        def _graph_has_cycle(
+            node: PortBase,
+            visited: Set[DirectedPortLocator],
+            stack: List[DirectedPortLocator],
+        ) -> bool:
+            # Helper to do the algebraic loop test by depth-first search on the graph
+            # to find cycles. Modifies `visited` and `stack` in place.
+
+            logger.debug(f"Checking node {node}")
+
+            assert node.directed_locator not in visited
+            visited.add(node.directed_locator)
+
+            if node in edges:
+                assert node not in stack
+                stack.append(node.directed_locator)
+                edge_iter = edges[node]
+                for target in edge_iter:
+                    if target.directed_locator not in visited and _graph_has_cycle(
+                        target, visited, stack
+                    ):
+                        logger.debug(f"Found cycle at {target}")
+                        return True
+                    elif target.directed_locator in stack:
+                        logger.debug(f"Found target {target} in stack {stack}")
+                        return True
+                stack.pop()
+
+            # If we get this far there is no cycle
+            return False
+
+        # Evaluate the graph for cycles
+        visited: Set[DirectedPortLocator] = set()
+        stack: List[DirectedPortLocator] = []
+        for node in nodes:
+            if node.directed_locator in visited:
+                continue
+            if _graph_has_cycle(node, visited, stack):
+                raise AlgebraicLoopError(self.name, stack)
```

## collimator/framework/diagram_builder.py

```diff
@@ -10,31 +10,29 @@
 # Affero General Public License along with this program. If not, see
 # <https://www.gnu.org/licenses/>.
 
 """Builder class for constructing block diagrams."""
 
 from __future__ import annotations
 
-from typing import Tuple, List, Mapping, Set, TYPE_CHECKING
+from typing import Tuple, List, Mapping, TYPE_CHECKING
 
 from ..logging import logger
 
 from .system_base import SystemBase
 from .diagram import Diagram
 from .error import InputNotConnectedError, StaticError
 from .parameter import Parameter
 
 if TYPE_CHECKING:
     from .port import (
-        PortBase,
         InputPort,
         OutputPort,
         InputPortLocator,
         OutputPortLocator,
-        DirectedPortLocator,
     )
 
     ExportedInputData = Tuple[InputPortLocator, str]  # (locator, port_name)
 
 __all__ = [
     "DiagramBuilder",
 ]
@@ -58,28 +56,14 @@
             f"Input port {system.name}[{port_index}] is not connected",
             system=system,
             port_index=port_index,
             port_direction="in",
         )
 
 
-class AlgebraicLoopError(BuilderError):
-    def __init__(self, name: str, loop: list[DirectedPortLocator]):
-        # `loop` is a list of ports that form a cycle. From there, we can recover
-        # system, direction and index as port[0], port[1], port[2] respectively.
-        str_loop = " \u2192 ".join(
-            f"{port[0].name_path_str}.{port[1]}[{port[2]}]" for port in loop
-        )
-        super().__init__(
-            f"Algebraic loop detected in {name}: {str_loop}",
-            loop=loop,
-            system=None,  # Not applicable since this involves multiple systems
-        )
-
-
 class EmptyDiagramError(BuilderError):
     def __init__(self, name: str):
         super().__init__(f"Cannot compile an empty diagram: {name}")
 
 
 class DiagramBuilder:
     """Class for constructing block diagram systems.
@@ -135,19 +119,14 @@
         """
         for system in systems:
             self._check_not_already_built()
             self._check_system_not_registered(system)
             self._check_system_name_is_unique(system)
             self._registered_systems.append(system)
 
-            # Make sure the child system has a dependency graph so that we can
-            # subscribe trackers to its ports and callbacks.  If the system already
-            # has a dependency graph, this will do nothing.
-            system.create_dependency_graph()
-
             # Add the system's input ports to the list of all input ports
             # So that we can make sure they're all connected before building.
             self._all_input_ports.extend([port.locator for port in system.input_ports])
 
             logger.debug(f"Added system {system.name} to DiagramBuilder")
             logger.debug(
                 f"    Registered systems: {[s.name for s in self._registered_systems]}"
@@ -319,109 +298,14 @@
     def _check_input_is_connected(self, input_port_locator: InputPortLocator):
         if not (
             (input_port_locator in self._input_port_ids)
             or (input_port_locator in self._connection_map)
         ):
             raise DisconnectedInputError(input_port_locator)
 
-    def _check_no_algebraic_loops(self, name: str):
-        """Check for algebraic loops in the diagram.
-
-        This is a more or less direct port of the Drake method
-        DiagramBuilder::ThrowIfAlgebraicLoopExists. Some comments are verbatim
-        explanations of the algorithm implemented there.
-        """
-
-        # The nodes in the graph are the input/output ports defined as part of
-        # the diagram's internal connections.  Ports that are not internally
-        # connected cannot participate in a cycle at this level, so we don't include them
-        # in the nodes set.
-        nodes: Set[PortBase] = set()
-
-        # For each `value` in `edges[key]`, the `key` directly influences `value`.
-        edges: Mapping[PortBase, Set[PortBase]] = {}
-
-        # Add the diagram's internal connections to the digraph nodes and edges
-        for input_port_locator, output_port_locator in self._connection_map.items():
-            # Directly using the port locator does not result in a unique identifier
-            # since (sys, 0) represents both input port 0 and output port 0.  Instead,
-            # use the port directly as a key, since it is a unique hashable object.
-            input_system, input_index = input_port_locator
-            input_port = input_system.input_ports[input_index]
-            logger.debug(f"Adding locator {input_port} to nodes")
-            nodes.add(input_port)
-
-            output_system, output_index = output_port_locator
-            output_port = output_system.output_ports[output_index]
-            logger.debug(f"Adding locator {output_port} to nodes")
-            nodes.add(output_port)
-
-            if output_port not in edges:
-                edges[output_port] = set()
-
-            logger.debug(f"Adding edge[{output_port}] = {input_port}")
-            edges[output_port].add(input_port)
-
-        # Add more edges based on each System's direct feedthrough.
-        # input -> output port iff there is direct feedthrough from input -> output
-        # If a feedthrough edge refers to a port not in `nodes`, omit it because ports
-        # that are not connected inside the diagram cannot participate in a cycle at
-        # the level of this diagram (higher-level diagrams will test for cycles at
-        # their level).
-        for system in self._registered_systems:
-            logger.debug(f"Checking feedthrough for system {system.name}")
-            for input_index, output_index in system.get_feedthrough():
-                input_port = system.input_ports[input_index]
-                output_port = system.output_ports[output_index]
-                logger.debug(f"Feedthrough from {input_port} to {output_port}")
-                if input_port in nodes and output_port in nodes:
-                    if input_port not in edges:
-                        edges[input_port] = set()
-                    edges[input_port].add(output_port)
-
-        def _graph_has_cycle(
-            node: PortBase,
-            visited: Set[DirectedPortLocator],
-            stack: List[DirectedPortLocator],
-        ) -> bool:
-            # Helper to do the algebraic loop test by depth-first search on the graph
-            # to find cycles. Modifies `visited` and `stack` in place.
-
-            logger.debug(f"Checking node {node}")
-
-            assert node.directed_locator not in visited
-            visited.add(node.directed_locator)
-
-            if node in edges:
-                assert node not in stack
-                stack.append(node.directed_locator)
-                edge_iter = edges[node]
-                for target in edge_iter:
-                    if target.directed_locator not in visited and _graph_has_cycle(
-                        target, visited, stack
-                    ):
-                        logger.debug(f"Found cycle at {target}")
-                        return True
-                    elif target.directed_locator in stack:
-                        logger.debug(f"Found target {target} in stack {stack}")
-                        return True
-                stack.pop()
-
-            # If we get this far there is no cycle
-            return False
-
-        # Evaluate the graph for cycles
-        visited: Set[DirectedPortLocator] = set()
-        stack: List[DirectedPortLocator] = []
-        for node in nodes:
-            if node.directed_locator in visited:
-                continue
-            if _graph_has_cycle(node, visited, stack):
-                raise AlgebraicLoopError(name, stack)
-
     def _check_contents_are_complete(self):
         # Make sure all the systems referenced in the builder attributes are registered
 
         # Check that systems and registered_systems have the same elements
         for system in self._registered_systems:
             self._check_system_is_registered(system)
 
@@ -452,15 +336,15 @@
                     system=src_sys,
                 )
 
     def build(
         self,
         name: str = "root",
         ui_id: str = None,
-        parameters: dict[str, Parameter] = None
+        parameters: dict[str, Parameter] = None,
     ) -> Diagram:
         """Builds a Diagram system with the specified name and system ID.
 
         Args:
             name (str, optional): The name of the diagram. Defaults to "root".
             system_id (Hashable, optional):
                 The system ID of the diagram. Defaults to None, which
@@ -479,39 +363,33 @@
         self._check_contents_are_complete()
         self._check_ports_are_valid()
 
         # Check that all internal input ports are connected
         for input_port_locator in self._input_port_ids:
             self._check_input_is_connected(input_port_locator)
 
-        logger.debug(f"DiagramBuilder: checking for algebraic loops in {name}")
-        self._check_no_algebraic_loops(name)
-        logger.debug(f"DiagramBuilder: no algebraic loops detected in {name}")
-
         if len(self._registered_systems) == 0:
             raise EmptyDiagramError(name)
 
         diagram = Diagram(
             nodes=self._registered_systems,
             name=name,
             connection_map=self._connection_map,
             ui_id=ui_id,
         )
 
         if parameters:
             for name, parameter in parameters.items():
-                diagram.declare_parameter(name, parameter)
+                diagram.declare_dynamic_parameter(name, parameter)
+                diagram.instance_parameters.add(name)
 
         # Export diagram-level inputs
         for locator, port_name in zip(self._input_port_ids, self._input_port_names):
             diagram.export_input(locator, port_name)
 
         # Export diagram-level outputs
         assert len(self._output_port_ids) == len(self._output_port_names)
         for locator, port_name in zip(self._output_port_ids, self._output_port_names):
             diagram.export_output(locator, port_name)
 
-        # Create the dependency graph for the diagram
-        diagram.create_dependency_graph()
-
         self._already_built = True  # Prevent further use of this builder
         return diagram
```

## collimator/framework/leaf_system.py

```diff
@@ -25,25 +25,26 @@
 
 After declaring states, parameters, ODE, updates, etc., the LeafSystem comprises a set
 of pure functions that can be evaluated given a Context, which contains the actual
 numeric values for the states, parameters, etc.
 """
 
 from __future__ import annotations
+from abc import ABCMeta
 from functools import partial
 from typing import List, Set, Tuple, Callable, TYPE_CHECKING
 
 import jax
 import jax.numpy as jnp
 from jax import tree_util
-import numpy as np
 
 from ..logging import logger
 
 from collimator.backend import utils
+
 # Import the switchable backend dispatcher as "collimator.numpy" or "cnp"
 from ..backend import cond, numpy_api as cnp
 
 from .cache import SystemCallback, CallbackTracer
 from .state import LeafState
 from .port import OutputPort
 
@@ -79,15 +80,41 @@
 
 
 # Helper functons used in feedthrough determination
 _mark_up_to_date = partial(mark_cache, is_out_of_date=False)
 _mark_out_of_date = partial(mark_cache, is_out_of_date=True)
 
 
-class LeafSystem(SystemBase):
+def _resolve_params(func):
+    def wrapper(*args, **kwargs):
+        args = [arg.get() if isinstance(arg, Parameter) else arg for arg in args]
+        kwargs = {
+            k: v.get() if isinstance(v, Parameter) else v for k, v in kwargs.items()
+        }
+        result = func(*args, **kwargs)
+        return result
+
+    return wrapper
+
+
+class InitializeParameterResolver(ABCMeta):
+    """Wrapper around the initialize() method to resolve Parameters.
+
+    All LeafSystem which implement the initialize() method will have their
+    parameters resolved before the method is called.
+    """
+
+    def __new__(cls, name, bases, dct):
+        if "initialize" in dct:
+            orig_initialize = dct["initialize"]
+            dct["initialize"] = _resolve_params(orig_initialize)
+        return super().__new__(cls, name, bases, dct)
+
+
+class LeafSystem(SystemBase, metaclass=InitializeParameterResolver):
     """Basic building block for dynamical systems.
 
     A LeafSystem is a minimal component of a system model in collimator, containing no
     subsystems.  Inputs, outputs, state, parameters, updates, etc. can be added to the
     block using the various `declare_*` methods.  The built-in blocks in
     collimator.library are all subclasses of LeafSystem, as are any custom blocks defined
     by the user."""
@@ -100,14 +127,15 @@
         # If not None, this defines the shape and data type of the continuous state
         # component.  This value will be used to initialize the context, so it will
         # also serve as the initial value unless explicitly overridden. It will
         # typically be an array, but it can be any PyTree-structured object (list,
         # dict, namedtuple, etc.), provided that the ODE function returns a PyTree
         # of the same structure.
         self._default_continuous_state: LeafStateComponent = None
+        self._continuous_state_output_port_idx: int = None
 
         # The SystemCallback associated with time derivatives of the continuous state.
         # This is initialized in the `declare_continuous_state` method.
         self.ode_callback: SystemCallback = None
 
         # If not empty, this defines the shape and data type of the discrete state.
         # This value will be used to initialize the context, so it will also serve
@@ -142,14 +170,25 @@
         self._state_update_events: List[DiscreteUpdateEvent] = []
 
         # Set of events that update when a zero-crossing occurs.  Each event has its
         # own guard function and, optionally, reset map, start mode, and end mode.
         # These can be created using the `declare_zero_crossing` method.
         self._zero_crossing_events: List[ZeroCrossingEvent] = []
 
+    def initialize(self, **parameters):
+        """Hook for initializing a system. Called during context creation.
+
+        If the parameters are instances of Parameter, they will be resolved.
+        If implemented, the function signature should contain all the declared
+        parameters.
+
+        This function should not be called directly.
+        """
+        pass
+
     @property
     def has_feedthrough_side_effects(self) -> bool:
         # See explanation in `SystemBase.has_feedthrough_side_effects`.  This will
         # almost always be False, but can be overridden in special cases where a
         # feedthrough output is computed via use of `io_callback`.
         return False
 
@@ -345,20 +384,14 @@
                 case the default is to assume dependency on either (inputs) if
                 `requires_inputs` is True, or (nothing) otherwise.
 
         Returns:
             int: The index of the callback in `system.callbacks`.  The cache index can
                 recovered from `system.callbacks[callback_index].cache_index`.
         """
-
-        if isinstance(period, Parameter):
-            period = period.get()
-        if isinstance(offset, Parameter):
-            offset = offset.get()
-
         # The index in the list of system callbacks
         callback_index = len(self.callbacks)
 
         # This is the index that this cached value will have in state.cache
         cache_index = len(self._default_cache)
         self._default_cache.append(default_value)
 
@@ -418,22 +451,64 @@
         default_value: Array = None,
         dtype: DTypeLike = None,
         ode: Callable = None,
         as_array: bool = True,
         requires_inputs: bool = True,
         prerequisites_of_calc: List[DependencyTicket] = None,
     ):
-        """Declare a continuous state component for the system.
+        """Declare a continuous state component for the system."""
+
+        self.ode_callback = SystemCallback(
+            callback=None,
+            system=self,
+            callback_index=len(self.callbacks),
+            name=f"{self.name}_ode",
+            prerequisites_of_calc=prerequisites_of_calc,
+        )
+        self.callbacks.append(self.ode_callback)
+        callback_idx = len(self.callbacks) - 1
+
+        # FIXME: this is to preserve some backward compatibility while we decouple
+        # declaration from configuration. Declaration should not have to call
+        # configuration.
+        if default_value is not None or shape is not None:
+            self.configure_continuous_state(
+                callback_idx,
+                shape=shape,
+                default_value=default_value,
+                dtype=dtype,
+                ode=ode,
+                as_array=as_array,
+                requires_inputs=requires_inputs,
+                prerequisites_of_calc=prerequisites_of_calc,
+            )
+
+        return callback_idx
+
+    def configure_continuous_state(
+        self,
+        callback_idx: int,
+        shape: ShapeLike = None,
+        default_value: Array = None,
+        dtype: DTypeLike = None,
+        ode: Callable = None,
+        as_array: bool = True,
+        requires_inputs: bool = True,
+        prerequisites_of_calc: List[DependencyTicket] = None,
+    ):
+        """Configure a continuous state component for the system.
 
         The `ode` callback computes the time derivative of the continuous state based on the
         current time, state, and any additional inputs. If `ode` is not provided, a default
         zero vector of the same size as the continuous state is used. If provided, the `ode`
         callback should have the signature `ode(time, state, *inputs, **params) -> xcdot`.
 
         Args:
+            callback_idx (int):
+                The index of the callback in the system's callback list.
             shape (ShapeLike, optional):
                 The shape of the continuous state vector. Defaults to None.
             default_value (Array, optional):
                 The initial value of the continuous state vector. Defaults to None.
             dtype (DTypeLike, optional):
                 The data type of the continuous state vector. Defaults to None.
             ode (Callable, optional):
@@ -465,26 +540,28 @@
 
         if prerequisites_of_calc is None:
             prerequisites_of_calc = [DependencyTicket.time, DependencyTicket.xc]
             if requires_inputs:
                 prerequisites_of_calc.append(DependencyTicket.u)
 
         if as_array:
-            default_value = utils.make_array(
-                default_value, dtype=dtype, shape=shape
-            )
+            default_value = utils.make_array(default_value, dtype=dtype, shape=shape)
 
         logger.debug(f"In block {self.name} [{self.system_id}]: {default_value=}")
 
         # Tree-map the default value to ensure that it is an array-like with the
         # correct shape and dtype. This is necessary because the default value
         # may be a list, tuple, or other PyTree-structured object.
         default_value = tree_util.tree_map(cnp.asarray, default_value)
 
         self._default_continuous_state = default_value
+        if self._continuous_state_output_port_idx is not None:
+            port = self.output_ports[self._continuous_state_output_port_idx]
+            port.default_value = default_value
+            self._default_cache[port.cache_index] = default_value
 
         if ode is None:
             # If no ODE is specified, return a zero vector of the same size as the
             # continuous state. This will break if the continuous state is
             # a named tuple, in which case a custom ODE must be provided.
             assert as_array, "Must provide custom ODE for non-array continuous state"
 
@@ -492,23 +569,16 @@
                 return cnp.zeros_like(default_value)
 
         # Wrap the ode function to accept a context and return the time derivatives.
         ode = self.wrap_callback(ode)
 
         # Declare the time derivative function as a system callback so that its
         # dependencies can be tracked in the system dependency graph
-        self.ode_callback = SystemCallback(
-            callback=ode,
-            system=self,
-            callback_index=len(self.callbacks),
-            name=f"{self.name}_ode",
-            prerequisites_of_calc=prerequisites_of_calc,
-        )
-
-        self.callbacks.append(self.ode_callback)
+        self.ode_callback._callback = ode
+        self.ode_callback.prerequisites_of_calc = prerequisites_of_calc
 
         # Override the default `eval_time_derivatives` to use the wrapped ODE function
         self.eval_time_derivatives = self.ode_callback.eval
 
     def declare_discrete_state(
         self,
         shape: ShapeLike = None,
@@ -547,63 +617,30 @@
             `default_value` is provided, it will be used as the initial value of the
             continuous state. If `shape` is provided, the initial value will be a
             zero vector of the given shape and specified dtype.
 
             (2) Use `declare_periodic_update` to declare an update event that
             modifies the discrete state at a recurring interval.
         """
-
-        if isinstance(default_value, Parameter):
-            default_value = default_value.get()
-
         if as_array:
-            default_value = utils.make_array(
-                default_value, dtype=dtype, shape=shape
-            )
+            default_value = utils.make_array(default_value, dtype=dtype, shape=shape)
 
         # Tree-map the default value to ensure that it is an array-like with the
         # correct shape and dtype. This is necessary because the default value
         # may be a list, tuple, or other PyTree-structured object.
         default_value = tree_util.tree_map(cnp.asarray, default_value)
 
         self._default_discrete_state = default_value
 
-    def declare_configuration_parameters(self, **params):
-        """Declare a set of "configuration" parameters for the system.
-
-        These parameters are non-numeric parameters used for block configuration.
-        Their declaration as parameters rather than object attributes is mainly
-        for the purpose of serialization - blocks that take boolean or string
-        parameters can register them as configuration parameters and they will be
-        properly serialized.
-
-        The args should be a dict of name-value pairs, where the values are either
-        strings, bool, arrays, or Parameters.
-
-        Typical usage:
-
-        ```python
-        class MyBlock(LeafSystem):
-            def __init__(self, param1=True, param2=1.0):
-                super().__init__()
-                self.declare_configuration_parameters(param1=param1, param2=param2)
-        ```
-        """
-        for name, value in params.items():
-            if isinstance(value, list):
-                self._instance_parameters[name] = Parameter(value=np.array(value))
-            else:
-                self._instance_parameters[name] = Parameter(value=value)
-
     #
     # I/O declaration
     #
     def declare_output_port(
         self,
-        callback: Callable,
+        callback: Callable = None,
         period: float | Parameter = None,
         offset: float | Parameter = 0.0,
         name: str = None,
         prerequisites_of_calc: List[DependencyTicket] = None,
         default_value: Array | Parameter = None,
         requires_inputs: bool = True,
     ) -> int:
@@ -639,21 +676,64 @@
                 None, in which case the assumption is a dependency on either (nothing)
                 if `requires_inputs` is False otherwise (inputs).
 
         Returns:
             int: The index of the declared output port.
         """
 
-        if isinstance(default_value, Parameter):
-            default_value = default_value.get()
-        if isinstance(period, Parameter):
-            period = period.get()
-        if isinstance(offset, Parameter):
-            offset = offset.get()
+        if default_value is not None:
+            default_value = cnp.array(default_value)
+
+        cache_index = None
+        if period is not None:
+            # The output port will be of "sample-and-hold" type, so we have to declare a
+            # periodic event to update the value.  The callback will be used to define the
+            # update event, and the output callback will simply return the stored value.
+
+            # This is the index that this port value will have in state.cache
+            cache_index = len(self._default_cache)
+            self._default_cache.append(default_value)
+
+        output_port_idx = super().declare_output_port(
+            callback, name=name, cache_index=cache_index
+        )
+
+        self.configure_output_port(
+            output_port_idx,
+            callback,
+            period=period,
+            offset=offset,
+            prerequisites_of_calc=prerequisites_of_calc,
+            default_value=default_value,
+            requires_inputs=requires_inputs,
+        )
+
+        return output_port_idx
+
+    def configure_output_port(
+        self,
+        port_index: int,
+        callback: Callable,
+        period: float | Parameter = None,
+        offset: float | Parameter = 0.0,
+        prerequisites_of_calc: List[DependencyTicket] = None,
+        default_value: Array | Parameter = None,
+        requires_inputs: bool = True,
+    ):
+        """Configure an output port in the LeafSystem.
+
+        See `declare_output_port` for a description of the arguments.
 
+        Args:
+            port_index (int):
+                The index of the output port to configure.
+
+        Returns:
+            None
+        """
         if default_value is not None:
             default_value = cnp.array(default_value)
 
         # To help avoid unnecessary flagging of algebraic loops, trim the inputs as a
         # default prereq if the output callback doesn't use them
         if prerequisites_of_calc is None:
             if requires_inputs:
@@ -670,15 +750,18 @@
 
         else:
             # The output port will be of "sample-and-hold" type, so we have to declare a
             # periodic event to update the value.  The callback will be used to define the
             # update event, and the output callback will simply return the stored value.
 
             # This is the index that this port value will have in state.cache
-            cache_index = len(self._default_cache)
+            cache_index = self.output_ports[port_index].cache_index
+            if cache_index is None:
+                cache_index = len(self._default_cache)
+                self._default_cache.append(default_value)
 
             def _output_callback(context: ContextBase) -> Array:
                 state = context[self.system_id].state
                 return state.cache[cache_index]
 
             def _update_callback(
                 time: Scalar, state: LeafState, *inputs, **parameters
@@ -697,24 +780,22 @@
                     period=period, offset=offset, active=False
                 ),
                 name=f"{self.name}:output_{cache_index}",
                 callback=_update_callback,
                 passthrough=self._passthrough,
             )
 
-            self._default_cache.append(default_value)
-
             # Note that in this case the "prerequisites of calc" will correspond to the
             # prerequisites of the update event, not the literal output callback itself.
             # However, these can be used to determine dependencies for the update event
             # via the output port.
 
-        return super().declare_output_port(
+        super().configure_output_port(
+            port_index,
             _output_callback,
-            name=name,
             prerequisites_of_calc=prerequisites_of_calc,
             default_value=default_value,
             event=event,
             cache_index=cache_index,
         )
 
     def declare_continuous_state_output(
@@ -729,25 +810,28 @@
         Args:
             name (str, optional):
                 The name of the output port. Defaults to None (autogenerate name).
 
         Returns:
             int: The index of the new output port.
         """
+        if self._continuous_state_output_port_idx is not None:
+            raise ValueError("Continuous state output port already declared")
 
         def _callback(time: Scalar, state: LeafState, *inputs, **parameters):
             return state.continuous_state
 
-        return self.declare_output_port(
+        self._continuous_state_output_port_idx = self.declare_output_port(
             _callback,
             name=name,
             prerequisites_of_calc=[DependencyTicket.xc],
             default_value=self._default_continuous_state,
             requires_inputs=False,
         )
+        return self._continuous_state_output_port_idx
 
     def declare_mode_output(self, name: str = None) -> int:
         """Declare a mode output port in the system.
 
         This method creates a new block-level output port which returns the component
         of the system's state corresponding to the discrete "mode" or "stage".
 
@@ -772,45 +856,65 @@
         )
 
     #
     # Event declaration
     #
     def declare_periodic_update(
         self,
+        callback: Callable = None,
+        period: Scalar | Parameter = None,
+        offset: Scalar | Parameter = None,
+        enable_tracing: bool = None,
+    ):
+        self._state_update_events.append(None)
+        event_idx = len(self._state_update_events) - 1
+
+        # FIXME: this is to preserve some backward compatibility while we decouple
+        # declaration from configuration. Declaration should not have to call
+        # configuration.
+        if callback is not None:
+            self.configure_periodic_update(
+                event_idx,
+                callback,
+                period,
+                offset,
+                enable_tracing=enable_tracing,
+            )
+        return event_idx
+
+    def configure_periodic_update(
+        self,
+        event_index: int,
         callback: Callable,
         period: Scalar | Parameter,
         offset: Scalar | Parameter,
         enable_tracing: bool = None,
     ):
-        """Declare a periodic discrete update event.
+        """Configure an existing periodic update event.
 
         The event will be triggered at regular intervals defined by the period and
         offset parameters. The callback should have the signature
         `callback(time, state, *inputs, **params) -> xd_plus`, where `xd_plus` is the
         updated value of the discrete state.
 
         This callback should be written to compute the "plus" value of the discrete
         state component given the "minus" values of all state components and inputs.
 
         Args:
+            event_index (int):
+                The index of the event to configure.
             callback (Callable):
                 The callback function defining the update.
             period (Scalar):
                 The period at which the update event occurs.
             offset (Scalar):
                 The offset at which the first occurrence of the event is triggered.
             enable_tracing (bool, optional):
                 If True, enable tracing for this event. Defaults to None.
         """
-
-        if isinstance(period, Parameter):
-            period = period.get()
-        if isinstance(offset, Parameter):
-            offset = offset.get()
-
         _wrapped_callback = self.wrap_callback(callback)
 
         def _callback(context: ContextBase) -> LeafState:
             xd = _wrapped_callback(context)
             return context[self.system_id].state.with_discrete_state(xd)
 
         if enable_tracing is None:
@@ -820,15 +924,15 @@
             system_id=self.system_id,
             name=f"{self.name}:periodic_update",
             event_data=PeriodicEventData(period=period, offset=offset, active=False),
             callback=_callback,
             passthrough=self._passthrough,
             enable_tracing=enable_tracing,
         )
-        self._state_update_events.append(event)
+        self._state_update_events[event_index] = event
 
     def declare_default_mode(self, mode: int):
         self._default_mode = mode
 
     def declare_zero_crossing(
         self,
         guard: Callable,
@@ -971,15 +1075,14 @@
             name=self.name,
             continuous_state=self._default_continuous_state,
             discrete_state=self._default_discrete_state,
             mode=self._default_mode,
             cache=tuple(self._default_cache),
         )
 
-
     def initialize_static_data(self, context: ContextBase):
         # Try to infer any missing default values for "sample-and-hold" output ports
         # and any other cached computations.
         cached_callbacks: list(SystemCallback) = [
             cb for cb in self.callbacks if cb.cache_index is not None
         ]
```

## collimator/framework/parameter.py

```diff
@@ -6,31 +6,30 @@
 # Software Foundation, version 3. This program is distributed in the hope that it
 # will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Affero General
 # Public License for more details.  You should have received a copy of the GNU
 # Affero General Public License along with this program. If not, see
 # <https://www.gnu.org/licenses/>.
 
+import ast
 from collections import defaultdict
 import dataclasses
 import enum
 from typing import Union
 
 from jax import Array
+from jax.flatten_util import ravel_pytree
 import jax.numpy as jnp
 import numpy as np
 
 from .error import ParameterError
 
 
-from ..backend.typing import (
-    ArrayLike,
-    ShapeLike,
-    DTypeLike,
-)
+from ..backend.typing import ArrayLike, DTypeLike, ShapeLike
+
 
 class ParameterExpr(list):
     pass
 
 
 class Ops(enum.Enum):
     ADD = enum.auto()
@@ -45,33 +44,35 @@
     ABS = enum.auto()
     EQ = enum.auto()
     NE = enum.auto()
     LT = enum.auto()
     LE = enum.auto()
     GT = enum.auto()
     GE = enum.auto()
+    MATMUL = enum.auto()
 
 
 __OPS_FN__ = {
     Ops.ADD: lambda x, y: x + y,
     Ops.SUB: lambda x, y: x - y,
     Ops.MUL: lambda x, y: x * y,
     Ops.DIV: lambda x, y: x / y,
     Ops.FLOORDIV: lambda x, y: x // y,
     Ops.MOD: lambda x, y: x % y,
-    Ops.POW: lambda x, y: x ** y,
+    Ops.POW: lambda x, y: x**y,
     Ops.NEG: lambda x: -x,
     Ops.POS: lambda x: +x,
-    Ops.ABS: lambda x: abs(x),
+    Ops.ABS: abs,
     Ops.EQ: lambda x, y: x == y,
     Ops.NE: lambda x, y: x != y,
     Ops.LT: lambda x, y: x < y,
     Ops.LE: lambda x, y: x <= y,
     Ops.GT: lambda x, y: x > y,
     Ops.GE: lambda x, y: x >= y,
+    Ops.MATMUL: lambda x, y: x @ y,
 }
 
 __OPS_STR__ = {
     Ops.ADD: "+",
     Ops.SUB: "-",
     Ops.MUL: "*",
     Ops.DIV: "/",
@@ -83,34 +84,75 @@
     Ops.ABS: "abs",
     Ops.EQ: "==",
     Ops.NE: "!=",
     Ops.LT: "<",
     Ops.LE: "<=",
     Ops.GT: ">",
     Ops.GE: ">=",
+    Ops.MATMUL: "@",
 }
 
 
+class _VarRecorder(ast.NodeVisitor):
+    """Used to record all variables in a Python expression."""
+
+    def __init__(self):
+        super().__init__()
+        self.vars = set()
+
+    def visit_Name(self, node):
+        self.vars.add(node.id)
+        return node.id
+
+
 ArrayLikeTypes = (
     Array,  # JAX array type
     np.ndarray,  # NumPy array type
-    np.bool_, np.number,  # NumPy scalar types
-    bool, int, float, complex,  # Python scalar types
+    np.bool_,
+    np.number,  # NumPy scalar types
+    bool,
+    int,
+    float,
+    complex,  # Python scalar types
 )
 
 
+def resolve_parameters(python_expr: str, env: dict):
+    # look for variables used in the expression
+    tree = ast.parse(python_expr, mode="eval")
+    var_recorder = _VarRecorder()
+    var_recorder.visit(tree.body)
+
+    # record the parameters and resolve them
+    parameters = set()
+    resolved_params = {}
+    for var in var_recorder.vars:
+        if var in env:
+            if isinstance(env[var], Parameter):
+                parameters.add(env[var])
+                resolved_params[var] = env[var].get()
+
+    return parameters, resolved_params
+
+
 def _resolve_array_like(value: ArrayLike) -> ArrayLike:
     vals = []
     if value.ndim == 0:
         return value
     for val in value:
         if isinstance(val, Parameter):
             vals.append(ParameterCache.__compute__(val))
         else:
             vals.append(_resolve_array_like(val))
+
+    numeric_types = (int, float, complex, np.number, bool)
+    is_numeric = all(isinstance(v, numeric_types) for v in vals)
+    if not is_numeric:
+        return vals
+
     return np.array(vals)
 
 
 def _list_to_str(lst):
     str_repr = []
     for val in lst:
         if isinstance(val, list):
@@ -147,19 +189,98 @@
         return tuple(new_lst)
     return new_lst
 
 
 def _add_dependents(lst, param):
     for val in lst:
         if isinstance(val, Parameter):
-            ParameterCache.__dependents__[val].add(param)
+            ParameterCache.add_dependent(val, param)
         elif isinstance(val, (list, tuple)):
             _add_dependents(val, param)
 
 
+def _array_to_str(arr):
+    if isinstance(arr, Parameter):
+        return str(arr)
+    if isinstance(arr, str):
+        return f'"{arr}"'
+    if arr.ndim == 0:
+        return str(arr.item())
+    arr = [_array_to_str(v) for v in arr]
+    arr = ", ".join(arr)
+    return f"np.array([{arr}])"
+
+
+def _value_as_str(value):
+    if isinstance(value, ArrayLikeTypes):
+        if isinstance(value, (Array, np.ndarray)):
+            return _array_to_str(value)
+        elif isinstance(value, bool):
+            return str(value)
+        elif isinstance(value, np.number):
+            dtype = value.dtype
+            return f"np.{dtype}({value.item()})"
+        return str(value)
+
+    if isinstance(value, ParameterExpr):
+        i = 0
+        str_repr = []
+        while i < len(value):
+            val = value[i]
+            if isinstance(val, Parameter):
+                val_str = val.name if val.name is not None else str(val)
+                if isinstance(val.value, ParameterExpr):
+                    val_str = f"({val_str})"
+                str_repr.append(val_str)
+            elif isinstance(val, Ops):
+                if val in (Ops.NEG, Ops.POS, Ops.ABS):
+                    if i + 1 >= len(value):
+                        raise ValueError()
+                    next_val = value[i + 1]
+                    if val is Ops.ABS:
+                        str_repr.append(f"abs({next_val})")
+                    elif val is Ops.NEG:
+                        str_repr.append(f"-{next_val}")
+                    elif val is Ops.POS:
+                        str_repr.append(f"+{next_val}")
+                    i += 1
+                else:
+                    str_repr.append(__OPS_STR__[val])
+            elif isinstance(val, (Array, np.ndarray)):
+                str_repr.append(f"np.array({val.tolist()})")
+            else:
+                str_repr.append(str(val))
+            i += 1
+
+        t = " ".join(str_repr)
+        return t
+
+    if isinstance(value, list):
+        return _list_to_str(value)
+
+    if isinstance(value, tuple):
+        return _tuple_to_str(value)
+
+    if isinstance(value, str):
+        return value
+
+    if value is None:
+        return ""
+
+    # if is a Pytree
+    try:
+        value, _ = ravel_pytree(value)
+        return _value_as_str(value)
+    except BaseException:
+        # Not a pytree
+        pass
+
+    return str(value)
+
+
 class ParameterCache:
     __dependents__: dict["Parameter", set["Parameter"]] = {}
     __cache__: dict["Parameter", ArrayLike] = {}
     __is_dirty__ = defaultdict(lambda: True)
 
     @classmethod
     def get(cls, param: "Parameter") -> ArrayLike:
@@ -167,14 +288,15 @@
             cls.__cache__[param] = cls.__compute__(param)
             cls.__is_dirty__[param] = False
 
         return cls.__cache__[param]
 
     @classmethod
     def replace(cls, param: "Parameter", value: ArrayLike):
+        # TODO: update dependencies of this parameter
         param.value = value
         cls.__invalidate__(param)
 
     @classmethod
     def remove(cls, param: "Parameter"):
         for dependents in cls.__dependents__.values():
             if param in dependents:
@@ -184,23 +306,26 @@
             del cls.__dependents__[param]
         if param in cls.__cache__:
             del cls.__cache__[param]
         if param in cls.__is_dirty__:
             del cls.__is_dirty__[param]
 
     @classmethod
+    def add_dependent(cls, param: "Parameter", dependent: "Parameter"):
+        cls.__dependents__[param].add(dependent)
+
+    @classmethod
     def __invalidate__(cls, param: "Parameter"):
         cls.__cache__[param] = None
         cls.__is_dirty__[param] = True
         for dependent in cls.__dependents__[param]:
             cls.__invalidate__(dependent)
 
     @classmethod
     def __compute__(cls, param: "Parameter"):
-
         if isinstance(param.value, ParameterExpr):
             acc = None
             right_value = None
             op = None
             i = 0
 
             while i < len(param.value):
@@ -209,31 +334,33 @@
                 if isinstance(val, Parameter):
                     right_value = val.get()
                 elif isinstance(val, ArrayLikeTypes):
                     right_value = val
                 elif isinstance(val, Ops):
                     if val in (Ops.NEG, Ops.POS, Ops.ABS):
                         if i + 1 >= len(param.value):
-                            raise ParameterError(param, message="Invalid parameter value")
+                            raise ParameterError(
+                                param, message="Invalid parameter value"
+                            )
                         if isinstance(param.value[i + 1], Parameter):
                             right_value = __OPS_FN__[val](param.value[i + 1].get())
                         elif isinstance(param.value[i + 1], ArrayLikeTypes):
                             right_value = __OPS_FN__[val](param.value[i + 1])
                         else:
                             raise ParameterError(
                                 param,
-                                message=f"Invalid value in parameter list: {param.value[i + 1]} of type {type(param.value[i + 1])}"
+                                message=f"Invalid value in parameter list: {param.value[i + 1]} of type {type(param.value[i + 1])}",
                             )
                         i += 1
                     else:
                         op = val
                 else:
                     raise ParameterError(
                         param,
-                        message=f"Invalid value in parameter list: {val} of type {type(val)}"
+                        message=f"Invalid value in parameter list: {val} of type {type(val)}",
                     )
 
                 if acc is not None and right_value is not None and op is not None:
                     acc = __OPS_FN__[op](acc, right_value)
                     op = None
                     right_value = None
                 elif right_value is not None:
@@ -241,18 +368,15 @@
                     right_value = None
                 i += 1
 
             if acc is not None:
                 return acc
             if right_value is not None:
                 return right_value
-            raise ParameterError(
-                param,
-                message="Invalid parameter value"
-            )
+            raise ParameterError(param, message="Invalid parameter value")
 
         if isinstance(param.value, Parameter):
             return cls.__compute__(param.value)
 
         if isinstance(param.value, tuple):
             t = _compute_list(param.value, is_tuple=True)
             return t
@@ -272,53 +396,71 @@
             return jnp.array(vals, dtype=param.value.dtype)
 
         if isinstance(param.value, np.number):
             if isinstance(param.value.item(), Parameter):
                 return type(param.value)(cls.__compute__(param.value.item()))
             return param.value
 
+        if isinstance(param.value, str) and param.is_python_expr:
+            _, params_in_global_resolved = resolve_parameters(
+                param.value, param.globals_
+            )
+            _, params_in_local_resolved = resolve_parameters(param.value, param.locals_)
+            resolved_parameters = {
+                **params_in_global_resolved,
+                **params_in_local_resolved,
+            }
+            return eval(
+                param.value, param.globals_, {**param.locals_, **resolved_parameters}
+            )
+
         return param.value
 
 
 def _op(op: Ops, left, right):
     param = Parameter(
         value=ParameterExpr([left, op, right]),
     )
     if isinstance(left, Parameter):
-        ParameterCache.__dependents__[left].add(param)
+        ParameterCache.add_dependent(left, param)
     if isinstance(right, Parameter):
-        ParameterCache.__dependents__[right].add(param)
+        ParameterCache.add_dependent(right, param)
     return param
 
 
 @dataclasses.dataclass
 class Parameter:
-
     value: Union[ParameterExpr, "Parameter", ArrayLike, str, tuple]
     dtype: DTypeLike = None
     shape: ShapeLike = None
 
     # name is used by reference submodels, model parameters and init script
     # variables so that they can be referred to in other fields
     # (we need this for serialization).
     name: str = None
 
+    # For complex parameter values, we can specify a Python expression as string
+    # This is useful for expressions like "np.eye(p)" where p is a parameter.
+    is_python_expr: bool = False
+    globals_: dict = None
+    locals_: dict = None
+
     def get(self):
         return ParameterCache.get(self)
 
     def set(self, value: Union["Parameter", ArrayLike, str, tuple]):
         ParameterCache.replace(self, value)
 
     def __post_init__(self):
         if isinstance(self.value, Parameter):
-            ParameterCache.__dependents__[self.value].add(self)
+            ParameterCache.add_dependent(self.value, self)
         if isinstance(self.value, ParameterExpr):
             for val in self.value:
                 if isinstance(val, Parameter):
-                    ParameterCache.__dependents__[val].add(self)
+                    ParameterCache.add_dependent(val, self)
         if isinstance(self.value, (list, tuple)):
             _add_dependents(self.value, self)
 
         ParameterCache.__dependents__[self] = set()
 
     def __add__(self, other):
         return _op(Ops.ADD, self, other)
@@ -360,25 +502,25 @@
         return _op(Ops.POW, self, other)
 
     def __rpow__(self, other):
         return _op(Ops.POW, other, self)
 
     def __neg__(self):
         p = Parameter(value=ParameterExpr([Ops.NEG, self]))
-        ParameterCache.__dependents__[self].add(p)
+        ParameterCache.add_dependent(self, p)
         return p
 
     def __pos__(self):
         p = Parameter(value=ParameterExpr([Ops.POS, self]))
-        ParameterCache.__dependents__[self].add(p)
+        ParameterCache.add_dependent(self, p)
         return p
 
     def __abs__(self):
         p = Parameter(value=ParameterExpr([Ops.ABS, self]))
-        ParameterCache.__dependents__[self].add(p)
+        ParameterCache.add_dependent(self, p)
         return p
 
     def __eq__(self, other):
         return _op(Ops.EQ, self, other)
 
     def __ne__(self, other):
         return _op(Ops.NE, self, other)
@@ -398,20 +540,22 @@
     def __del__(self):
         ParameterCache.remove(self)
 
     def __hash__(self):
         return id(self)
 
     def __str__(self):
-
         if self.name is not None:
             return self.name
 
         return self.value_as_str()
 
+    def __matmul__(self, other):
+        return _op(Ops.MATMUL, self, other)
+
     def __int__(self):
         if self.dtype is not None:
             return self.dtype(self.get())
         return int(self.get())
 
     def __float__(self):
         if self.dtype is not None:
@@ -422,75 +566,18 @@
     # def __bool__(self):
     #     return bool(self.get())
 
     def __complex__(self):
         return complex(self.get())
 
     def value_as_str(self):
+        """Used for serialization of parameters. This string is displayed in the
+        UI text fields for the parameters."""
+        try:
+            return _value_as_str(self.value)
+        except ValueError as e:
+            raise ParameterError(
+                self, message=f"Invalid parameter value: {self.value}"
+            ) from e
 
-        def array_to_str(arr):
-            if isinstance(arr, Parameter):
-                return str(arr)
-            if isinstance(arr, str):
-                return f'"{arr}"'
-            if arr.ndim == 0:
-                return str(arr.item())
-            arr = [array_to_str(v) for v in arr]
-            arr = ", ".join(arr)
-            return f"np.array([{arr}])"
-
-        if isinstance(self.value, ArrayLikeTypes):
-            if isinstance(self.value, (Array, np.ndarray)):
-                return array_to_str(self.value)
-            elif isinstance(self.value, bool):
-                return str(self.value)
-            elif isinstance(self.value, np.number):
-                dtype = self.value.dtype
-                return f"np.{dtype}({self.value.item()})"
-            return str(self.value)
-
-        if isinstance(self.value, ParameterExpr):
-            i = 0
-            str_repr = []
-            while i < len(self.value):
-                val = self.value[i]
-                if isinstance(val, Parameter):
-                    val_str = val.name if val.name is not None else str(val)
-                    if isinstance(val.value, ParameterExpr):
-                        val_str = f"({val_str})"
-                    str_repr.append(val_str)
-                elif isinstance(val, Ops):
-                    if val in (Ops.NEG, Ops.POS, Ops.ABS):
-                        if i + 1 >= len(self.value):
-                            raise ParameterError(self, message="Invalid parameter value")
-                        next_val = self.value[i + 1]
-                        if val is Ops.ABS:
-                            str_repr.append(f"abs({next_val})")
-                        elif val is Ops.NEG:
-                            str_repr.append(f"-{next_val}")
-                        elif val is Ops.POS:
-                            str_repr.append(f"+{next_val}")
-                        i += 1
-                    else:
-                        str_repr.append(__OPS_STR__[val])
-                elif isinstance(val, (Array, np.ndarray)):
-                    str_repr.append(f"np.array({val.tolist()})")
-                else:
-                    str_repr.append(str(val))
-                i += 1
-
-            t = " ".join(str_repr)
-            return t
-
-        if isinstance(self.value, list):
-            return _list_to_str(self.value)
-
-        if isinstance(self.value, tuple):
-            return _tuple_to_str(self.value)
-
-        if isinstance(self.value, str):
-            return self.value
-
-        if self.value is None:
-            return ""
-
-        return str(self.value)
+    def __repr__(self):
+        return f"Parameter(name={self.name}, value={self.value_as_str()}, value_type={type(self.value)})"
```

## collimator/framework/port.py

```diff
@@ -68,16 +68,15 @@
 
     def __post_init__(self, callback):
         super().__post_init__(callback)
         assert self.index is not None, "Port index cannot be None"
 
     @property
     @abstractmethod
-    def direction(self) -> str:
-        ...
+    def direction(self) -> str: ...
 
     @property
     def locator(self) -> EitherPortLocator:
         return (self.system, self.index)
 
     @property
     def directed_locator(self) -> DirectedPortLocator:
```

## collimator/framework/system_base.py

```diff
@@ -24,38 +24,42 @@
 derivatives of the continuous state for the system, given the root context of
 the diagram.
 """
 
 from __future__ import annotations
 
 import abc
+from functools import wraps
+import inspect
 import traceback
 from typing import (
     List,
     Tuple,
     TYPE_CHECKING,
     Hashable,
     Callable,
     Union,
+    ParamSpec,
+    TypeVar,
 )
 import dataclasses
 
+import numpy as np
+
 from collimator.framework.error import BlockParameterError
 from ..backend import utils
 from ..logging import logger
 from .cache import SystemCallback
 from .event import FlatEventCollection
 from .parameter import Parameter
 from .port import InputPort, OutputPort
 from .dependency_graph import DependencyTicket, sort_trackers
 from .error import StaticError
 
-__all__ = [
-    "SystemBase",
-]
+__all__ = ["SystemBase", "parameters"]
 
 if TYPE_CHECKING:
     # Array-like object, e.g. a JAX PyTree or a numpy ndarray.
     from ..backend.typing import (
         Array,
         ShapeLike,
         DTypeLike,
@@ -79,14 +83,103 @@
 
 
 def reset_system_id():
     """Reset the system ID counter."""
     IDGenerator.reset()
 
 
+def _get_arg_names(func):
+    sig = inspect.signature(func)
+    positional_arg_names = []
+    all_args = []
+    for name, param in sig.parameters.items():
+        is_positional_or_keyword = param.kind in (
+            inspect.Parameter.POSITIONAL_OR_KEYWORD,
+            inspect.Parameter.POSITIONAL_ONLY,
+        )
+        if is_positional_or_keyword and param.default == inspect.Parameter.empty:
+            positional_arg_names.append(name)
+        all_args.append(name)
+
+    return all_args, positional_arg_names
+
+
+def _get_default_value(init_func, param_name):
+    sig = inspect.signature(init_func)
+    param = sig.parameters[param_name]
+    if param.default == inspect.Parameter.empty:
+        return None
+    return param.default
+
+
+def _get_params(param_names, init_func, args, kwargs):
+    all_args, args_names = _get_arg_names(init_func)
+    all_args = all_args[1:]  # remove self
+    args_names = args_names[1:]  # remove self
+
+    params = {}
+    for k in param_names:
+        if k in kwargs:
+            params[k] = kwargs[k]
+        elif k in args_names:
+            idx = args_names.index(k)
+            if idx >= len(args):
+                raise ValueError(f"Missing required argument {k}")
+            params[k] = args[idx]
+        elif k in all_args and all_args.index(k) < len(args):
+            params[k] = args[all_args.index(k)]
+        else:
+            # kwarg's default value
+            params[k] = _get_default_value(init_func, k)
+    return params
+
+
+P = ParamSpec("P")
+T = TypeVar("T")
+
+
+def parameters(static: list[str] = None, dynamic: list[str] = None):
+    """Decorator to apply to the __init__ function of a system to declare
+    static or dynamic parameters."""
+
+    if static is None:
+        static = []
+
+    if dynamic is None:
+        dynamic = []
+
+    static_param_names = set(static)
+    dynamic_param_names = set(dynamic)
+
+    def decorator(init_func: Callable[P, T]) -> Callable[P, T]:
+        @wraps(init_func)
+        def wrapped_init(self, *args, **kwargs):
+            resolved_args = [
+                arg.get() if isinstance(arg, Parameter) else arg for arg in args
+            ]
+            resolved_kwargs = {
+                k: kwarg.get() if isinstance(kwarg, Parameter) else kwarg
+                for k, kwarg in kwargs.items()
+            }
+            init_func(self, *resolved_args, **resolved_kwargs)
+
+            static_params = _get_params(static_param_names, init_func, args, kwargs)
+            for param_name, value in static_params.items():
+                self.declare_static_parameter(param_name, value)
+
+            dyn_params = _get_params(dynamic_param_names, init_func, args, kwargs)
+            for param_name, value in dyn_params.items():
+                if value is not None:
+                    self.declare_dynamic_parameter(param_name, value)
+
+        return wrapped_init
+
+    return decorator
+
+
 class IDGenerator:
     """Singleton class for automatically managing unique system IDs.
 
     This can be ignored altogether if using manually determined system IDs,
     for example as determined by "block path" from the UI. In either case, it
     typically does not need to be used directly by either users or developers.
     """
@@ -155,26 +248,26 @@
 
         # A dependency graph for the system, mapping prerequisites of each calculation.
         # `None` indicates that the dependency graph has not been constructed yet.  If
         # accessed via the `dependency_graph` property, it will be constructed
         # automatically as necessary.
         self._dependency_graph: DependencyGraph = None
 
-        # Storage of attributes for system serialization
-        self._instance_parameters: dict[str, Parameter] = {}
+        # Static parameters are not jax-traceable
+        self._static_parameters: dict[str, Parameter] = {}
 
         # If not empty, this defines the shape and data type of the numeric parameters
         # in the LeafSystem. This value will be used to initialize the context, so it
         # will also serve as the initial value unless explicitly overridden. In the
         # simplest cases, parameters could be stored as attributes of the LeafSystem,
         # but declaring them has the advantage of moving the values to the context,
         # allowing them to be traced by JAX rather than stored as static data. This
         # means they can be differentiated, vmapped, or otherwise modified without
         # re-compiling the simulation.
-        self._default_parameters: dict[str, Array] = {}
+        self._dynamic_parameters: dict[str, Array] = {}
 
         # Map from (input_port, output_port) if that pair is feedthrough
         # `None` indicates that the feedthrough is unknown for this system.
         # This will be computed automatically using the dependency graph
         # during algebraic loop detection unless it is set manually.
         # To manually set feedthrough, either declare this explicitly or
         # override `get_feedthrough`.
@@ -190,21 +283,35 @@
 
     def pprint(self, output=print) -> str:
         output(self._pprint_helper().strip())
 
     def _pprint_helper(self, prefix="") -> str:
         return f"{prefix}|-- {self.name}(id={self.system_id})\n"
 
+    def post_simulation_finalize(self) -> None:
+        """Finalize the system after simulation has completed.
+
+        This is only intended for special blocks that need to clean up
+        resources and close files."""
+
     @property
-    def instance_parameters(self) -> dict[str, Parameter]:
-        return self._instance_parameters
+    def static_parameters(self) -> dict[str, Parameter]:
+        return self._static_parameters
 
-    @instance_parameters.setter
-    def instance_parameters(self, value):
-        self._instance_parameters = value
+    @static_parameters.setter
+    def static_parameters(self, value):
+        self._static_parameters = value
+
+    @property
+    def dynamic_parameters(self) -> dict[str, Parameter]:
+        return self._dynamic_parameters
+
+    @property
+    def parameters(self) -> dict[str, Parameter]:
+        return {**self.static_parameters, **self.dynamic_parameters}
 
     #
     # Simulation interface
     #
     @abc.abstractproperty
     def has_feedthrough_side_effects(self) -> bool:
         """Check if the system includes any feedthrough calls to `io_callback`."""
@@ -681,15 +788,15 @@
             the callback function associated with the system-level port
 
         Returns the corresponding index into the system output_port_indices list
         Note that this is different from the callbacks index - typically it
         will make more sense to retrieve via system.output_ports[port_index].
 
         Args:
-            callback (Callable): computes the value of the output port given
+            callback (Callable, optional): computes the value of the output port given
                 the root context.
             name (str, optional): name of the new port. Defaults to None, which will
                 use the default naming scheme for the system (e.g. "y_0")
             prerequisites_of_calc (List[DependencyTicket], optional): list of
                 dependencies for the callback function. Defaults to None, which will
                 use the default dependencies for the system (all sources).  This may
                 conservatively flag the system as having algebraic loops, so it is
@@ -740,41 +847,98 @@
 
         # Check that name is unique
         for p in self.output_ports:
             assert (
                 p.name != port.name
             ), f"System {self.name} already has an output port named {port.name}"
 
-        logger.debug(f"Adding output port {port} to {self.name}")
+        logger.debug("Adding output port %s to %s", port, self.name)
         self.output_port_indices.append(callback_index)
         self.callbacks.append(port)
         logger.debug(
-            f"    ---> {self.name} now has {len(self.output_ports)} output ports: {self.output_ports}"
+            "    ---> %s now has %s output ports: %s",
+            self.name,
+            len(self.output_ports),
+            self.output_ports,
         )
         logger.debug(
-            f"    ---> {self.name} now has {len(self.callbacks)} cache sources: {self.callbacks}"
+            "    ---> %s now has %s cache sources: %s",
+            self.name,
+            len(self.callbacks),
+            self.callbacks,
         )
 
         return port_index
 
+    def configure_output_port(
+        self,
+        port_index: int,
+        callback: Callable,
+        prerequisites_of_calc: List[DependencyTicket] = None,
+        default_value: Array = None,
+        event: DiscreteUpdateEvent = None,
+        cache_index: int = None,
+    ):
+        """Configure an output port of the system.
+
+        See `declare_output_port` for a description of the arguments.
+
+        Args:
+            port_index (int): index of the output port to configure
+
+        Returns:
+            None
+        """
+        old_port = self.output_ports[port_index]
+
+        if prerequisites_of_calc is None:
+            prerequisites_of_calc = [DependencyTicket.all_sources]
+
+        port = OutputPort(
+            callback,
+            system=self,
+            callback_index=old_port.callback_index,
+            name=old_port.name,
+            index=port_index,
+            prerequisites_of_calc=prerequisites_of_calc,
+            default_value=default_value,
+            event=event,
+            cache_index=cache_index,
+            ticket=old_port.ticket,
+        )
+
+        self.callbacks[old_port.callback_index] = port
+        logger.debug(
+            "    ---> %s now has %s output ports: %s",
+            self.name,
+            len(self.output_ports),
+            self.output_ports,
+        )
+        logger.debug(
+            "    ---> %s now has %s cache sources: %s",
+            self.name,
+            len(self.callbacks),
+            self.callbacks,
+        )
+
     @abc.abstractmethod
     def get_feedthrough(self) -> List[Tuple[int, int]]:
         """Determine pairs of direct feedthrough ports for this system.
 
         By default, the algorithm relies on the dependency tracking system to determine
         feedthrough, but this can be overridden by implementing this method directly
         in a subclass, for instance if the automatic dependency tracking is too
         conservative in determining feedthrough.
 
         Returns:
             List[Tuple[int, int]]:
                 A list of tuples (u, v) indicating that output port v has a direct
                 dependency on input port u, resulting in a feedthrough path in the system.
                 The indices u and v correspond to the indices of the input and output
-                ports in the system's input and outpu port lists.
+                ports in the system's input and output port lists.
         """
         pass
 
     #
     # Initialization
     #
     def create_context(self, **kwargs) -> ContextBase:
@@ -871,34 +1035,79 @@
         if self.parent.parent is None:
             return [self.ui_id]  # top-level block
         parent_path = self.parent.ui_id_path
         if parent_path is None:
             return None
         return parent_path + [self.ui_id]
 
-    #
-    # Serialization
-    #
-    @property
-    def default_parameters(self) -> dict[str, Parameter]:
-        return self._default_parameters
+    def declare_static_parameters(self, **params):
+        """Declare a set of static parameters for the system.
 
-    def declare_parameter(
+        These parameters are not JAX-traceable and therefore can't be optimized.
+
+        Examples of static parameters include booleans, strings, parameters
+        used in shapes, etc.
+
+        The args should be a dict of name-value pairs, where the values are either
+        strings, bool, arrays, or Parameters.
+
+        Typical usage:
+
+        ```python
+        class MyBlock(LeafSystem):
+            def __init__(self, param1=True, param2=1.0):
+                super().__init__()
+                self.declare_static_parameters(param1=param1, param2=param2)
+        ```
+        """
+        for name, value in params.items():
+            if name in self.dynamic_parameters:
+                raise BlockParameterError(
+                    "Parameter already declared as dynamic parameter",
+                    system=self,
+                    parameter_name=name,
+                )
+            if isinstance(value, list):
+                self._static_parameters[name] = Parameter(value=np.array(value))
+            else:
+                self._static_parameters[name] = Parameter(value=value)
+
+    def declare_static_parameter(self, name, value):
+        """Declare a single static parameter for the system.
+
+        This is a convenience function for declaring a single static parameter.
+
+        Args:
+            name (str): name of the parameter
+            value (Union[Array, Parameter]): value of the parameter
+        """
+        if name in self.dynamic_parameters:
+            raise BlockParameterError(
+                "Parameter already declared as dynamic parameter",
+                system=self,
+                parameter_name=name,
+            )
+        if isinstance(value, list):
+            self._static_parameters[name] = Parameter(value=np.array(value))
+        else:
+            self._static_parameters[name] = Parameter(value=value)
+
+    def declare_dynamic_parameter(
         self,
         name: str,
         default_value: Array | Parameter = None,
         shape: ShapeLike = None,
         dtype: DTypeLike = None,
         as_array: bool = True,
     ):
         """Declare a numeric parameter for the system.
 
         Parameters are declared in the system and accessed through the context to
         maintain separation of data ownership. This method creates an entry in the
-        system's default_parameters, recording the name, default value, and dependency
+        system's dynamic_parameters, recording the name, default value, and dependency
         ticket for later reference.
 
         The default value will be used to initialize the context, so it
         will also serve as the initial value unless explicitly overridden. In the
         simplest cases, parameters could be stored as attributes of the LeafSystem,
         but declaring them has the advantage of moving the values to the context,
         allowing them to be traced by JAX rather than stored as static data. This
@@ -926,38 +1135,43 @@
 
         Notes:
             (1) Only one of `shape` and `default_value` should be provided. If
             `default_value` is provided, it will be used as the initial value of the
             continuous state. If `shape` is provided, the initial value will be a
             zero vector of the given shape and specified dtype.
         """
-        assert (
-            name not in self._instance_parameters
-        ), f"Parameter {name} already declared"
+        # assert (
+        #     name not in self._dynamic_parameters
+        # ), f"Parameter {name} already declared"
+
+        if name in self.static_parameters:
+            raise BlockParameterError(
+                "Parameter already declared as static parameter",
+                system=self,
+                parameter_name=name,
+            )
 
         try:
             if isinstance(default_value, Parameter):
-                self._instance_parameters[name] = default_value
+                self._dynamic_parameters[name] = default_value
             else:
                 if as_array:
                     default_value = utils.make_array(
                         default_value, dtype=dtype, shape=shape
                     )
-                self._instance_parameters[name] = Parameter(
+                self._dynamic_parameters[name] = Parameter(
                     value=default_value,
                     dtype=dtype,
                     shape=shape,
                 )
 
             logger.debug(
                 f"Adding parameter {name} to {self.name} with default: {default_value}"
             )
 
-            self._default_parameters[name] = self._instance_parameters[name]
-
         except Exception as e:
             traceback.print_exc()
             raise BlockParameterError(
                 "Error declaring parameter",
                 system=self,
                 parameter_name=name,
             ) from e
```

## collimator/library/__init__.py

```diff
@@ -108,14 +108,17 @@
     LinearQuadraticRegulator,
     DiscreteTimeLinearQuadraticRegulator,
     FiniteHorizonLinearQuadraticRegulator,
 )
 
 from .nn import (
     MLP,
+)
+
+from .costs_and_losses import (
     QuadraticCost,
 )
 
 from .fmu_import import (
     ModelicaFMU,
 )
 
@@ -127,28 +130,33 @@
 from .rotations import (
     CoordinateRotation,
     CoordinateRotationConversion,
     RigidBody,
 )
 
 from .sindy import (
-    ContinuousTimeSindyWithControl,
+    Sindy,
 )
 
 from .data_source import (
     DataSource,
 )
 from .state_machine import (
     StateMachine,
 )
 
 from .ansys import (
     PyTwin,
 )
 
+from .ros2 import (
+    Ros2Publisher,
+    Ros2Subscriber,
+)
+
 from .state_estimators import (
     KalmanFilter,
     InfiniteHorizonKalmanFilter,
     ContinuousTimeInfiniteHorizonKalmanFilter,
     ExtendedKalmanFilter,
     UnscentedKalmanFilter,
 )
@@ -156,14 +164,16 @@
 from .predictor import (
     PyTorch,
     TensorFlow,
 )
 
 from .reference_subdiagram import ReferenceSubdiagram
 
+from .quanser import QuanserHAL, QubeServoModel
+
 __all__ = [
     "SourceBlock",
     "FeedthroughBlock",
     "ReduceBlock",
     "Abs",
     "Constant",
     "Sine",
@@ -214,15 +224,15 @@
     "Pulse",
     "Quantizer",
     "RandomNumber",
     "Relay",
     "RigidBody",
     "Sawtooth",
     "ScalarBroadcast",
-    "ContinuousTimeSindyWithControl",
+    "Sindy",
     "SumOfElements",
     "Slice",
     "StateMachine",
     "Stack",
     "Step",
     "Stop",
     "SquareRoot",
@@ -256,9 +266,13 @@
     "UnscentedKalmanFilter",
     "LinearQuadraticRegulator",
     "DiscreteTimeLinearQuadraticRegulator",
     "FiniteHorizonLinearQuadraticRegulator",
     "PyTwin",
     "PyTorch",
     "TensorFlow",
+    "Ros2Publisher",
+    "Ros2Subscriber",
     "SignalDatatypeConversion",
+    "QubeServoModel",
+    "QuanserHAL",
 ]
```

## collimator/library/ansys.py

```diff
@@ -12,40 +12,41 @@
 
 from collections import namedtuple
 
 import jax
 import jax.numpy as jnp
 from jax.experimental import io_callback
 
-from ..framework import LeafSystem
+from ..framework import LeafSystem, parameters
 from ..lazy_loader import LazyLoader
 
 pytwin = LazyLoader("pytwin", globals(), "pytwin")
 
 
 class PyTwin(LeafSystem):
+    @parameters(
+        static=[
+            "pytwin_file",
+            "pytwin_config",
+            "parameters",
+            "inputs",
+        ]
+    )
     def __init__(
         self,
         pytwin_file,
         dt,
         pytwin_config=None,
         parameters=None,
         inputs=None,
         *args,
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
 
-        self.declare_configuration_parameters(
-            pytwin_file=pytwin_file,
-            pytwin_config=pytwin_config,
-            parameters=parameters,
-            inputs=inputs,
-        )
-
         self.dt = dt
 
         self.twin_model = pytwin.TwinModel(pytwin_file)
         if pytwin_config:
             self.twin_model.initialize_evaluation(json_config_filepath=pytwin_config)
         elif parameters or inputs:
             self.twin_model.initialize_evaluation(parameters=parameters, inputs=inputs)
```

## collimator/library/battery_cell.py

```diff
@@ -9,15 +9,15 @@
 # Public License for more details.  You should have received a copy of the GNU
 # Affero General Public License along with this program. If not, see
 # <https://www.gnu.org/licenses/>.
 
 from __future__ import annotations
 from typing import TYPE_CHECKING, NamedTuple
 
-from ..framework import LeafSystem, DependencyTicket
+from ..framework import LeafSystem, DependencyTicket, parameters
 from ..backend import numpy_api as cnp
 
 if TYPE_CHECKING:
     from ..backend.typing import Array
 
 
 __all__ = ["BatteryCell"]
@@ -63,71 +63,66 @@
         i_lb: float
 
     class FirstOrderFilter(NamedTuple):
         A: float
         B: float
         C: float
 
+    @parameters(dynamic=["E0", "K", "Q", "R", "tau", "A", "B", "initial_SOC"])
     def __init__(
         self,
         E0: float = 3.366,
         K: float = 0.0076,
         Q: float = 2.3,
         R: float = 0.01,
         tau: float = 30.0,
         A: float = 0.26422,
         B: float = 26.5487,
         initial_SOC: float = 1.0,
         **kwargs,
     ):
         super().__init__(**kwargs)
 
-        self.declare_parameter("E0", E0)
-        self.declare_parameter("K", K)
-        self.declare_parameter("Q", Q)
-        self.declare_parameter("R", R)
-        self.declare_parameter("tau", tau)
-        self.declare_parameter("A", A)
-        self.declare_parameter("B", B)
-        self.declare_parameter("initial_SOC", initial_SOC)
+        self.declare_input_port()  # Current flowing through the cell
+
+        self.declare_output_port(
+            self._voltage_output,
+            prerequisites_of_calc=[DependencyTicket.xc],
+            requires_inputs=False,
+            name="voltage",
+        )
+
+        self.declare_output_port(
+            self._soc_output,
+            prerequisites_of_calc=[DependencyTicket.xc],
+            requires_inputs=False,
+            name="soc",
+        )
+
+        self.initialize(E0, K, Q, R, tau, A, B, initial_SOC)
 
+    def initialize(self, E0, K, Q, R, tau, A, B, initial_SOC):
         # Filter for input current
         self.current_filter = self.FirstOrderFilter(-0.05, 1.0, 0.05)
 
         # Filter for loop-breaker
         self.lb_filter = self.FirstOrderFilter(-10.0, 1.0, 10.0)
 
         initial_state = self.BatteryStateType(
             soc=initial_SOC,
             i_star=0.0,  # Filtered input current
             i_lb=0.0,  # Filtered current for loop-breaking
         )
 
-        self.declare_input_port()  # Current flowing through the cell
-
         self.declare_continuous_state(
             default_value=initial_state,
             as_array=False,
             ode=self._ode,
         )
 
-        self.declare_output_port(
-            self._voltage_output,
-            prerequisites_of_calc=[DependencyTicket.xc],
-            requires_inputs=False,
-            name="voltage",
-        )
-
-        self.declare_output_port(
-            self._soc_output,
-            prerequisites_of_calc=[DependencyTicket.xc],
-            requires_inputs=False,
-            name="soc",
-        )
-
     def _ode(self, _time, state, *inputs, **parameters) -> BatteryStateType:
         xc = state.continuous_state
         Q = parameters["Q"]
 
         (u,) = inputs
 
         soc_der_unsat = -u / (Q * Ah_to_As)
```

## collimator/library/custom.py

```diff
@@ -18,15 +18,15 @@
 from io import StringIO
 import types
 from typing import TYPE_CHECKING, Any, List, Mapping
 
 import jax
 import jax.numpy as jnp
 
-from ..framework import LeafSystem, LeafState
+from ..framework import LeafSystem, LeafState, parameters
 from ..logging import logger
 from ..framework.error import (
     BlockInitializationError,
     ErrorCollector,
     PythonScriptError,
     PythonScriptTimeNotSupportedError,
 )
@@ -203,22 +203,32 @@
             output ports is the same as the order of the output variables.
         parameters (Mapping[str, Array]): A dictionary mapping parameter names to
             values. Parameters are treated as immutable and cannot be modified in
             the step code. Parameters can be arrays or scalars, but must have static
             shapes and dtypes in order to support JIT compilation.
     """
 
+    @parameters(
+        static=[
+            "dt",
+            "init_script",
+            "user_statements",
+            "finalize_script",
+            "accelerate_with_jax",
+            "time_mode",
+        ]
+    )
     def __init__(
         self,
         dt: float = None,
         init_script: str = "",
         user_statements: str = "",
         finalize_script: str = "",  # presently ignored for JAX block
         accelerate_with_jax: bool = True,
-        time_mode: bool = "discrete",  # [discrete, agnostic]
+        time_mode: str = "discrete",  # [discrete, agnostic]
         inputs: List[str] = None,  # [name]
         outputs: List[str] = None,
         parameters: Mapping[str, Array] = None,
         **kwargs,
     ):
         super().__init__(**kwargs)
         parameters = parameters or {}
@@ -259,15 +269,15 @@
             )
 
         # Declare parameters
         for param_name, value in parameters.items():
             if isinstance(value, list):
                 value = cnp.asarray(value)
             as_array = isinstance(value, cnp.ndarray) or cnp.isscalar(value)
-            self.declare_parameter(param_name, value, as_array=as_array)
+            self.declare_dynamic_parameter(param_name, value, as_array=as_array)
 
         # Run the init_script
         persistent_env = self.exec_init()
 
         # Declare an input port for each of the input variables
         self.input_names = inputs
         for name in inputs:
@@ -277,22 +287,25 @@
         self._create_cache_type(outputs)
 
         if time_mode == "discrete":
             self._configure_discrete(dt, outputs, persistent_env)
         else:
             self._configure_agnostic(outputs, persistent_env)
 
-        self.declare_configuration_parameters(
-            dt=dt,
-            init_script=init_script,
-            user_statements=user_statements,
-            finalize_script=finalize_script,
-            accelerate_with_jax=accelerate_with_jax,
-            time_mode=time_mode,
-        )
+    def initialize(
+        self,
+        dt: float = None,
+        init_script: str = "",
+        user_statements: str = "",
+        finalize_script: str = "",  # presently ignored for JAX block
+        accelerate_with_jax: bool = True,
+        time_mode: str = "discrete",  # [discrete, agnostic]
+        **parameters,
+    ):
+        pass
 
     def _initialize_outputs(self, outputs, persistent_env):
         default_outputs = {name: None for name in outputs}
 
         for name in outputs:
             # If the initial value is set explicitly in the init script,
             # override the default value.  We don't need to do this for
@@ -432,15 +445,15 @@
         }
 
     def exec_init(self) -> dict[str, Array]:
         # Before executing the step code, we have to build up the local environment.
         # This includes specified modules, python block user defined parameters.
 
         default_parameters = {
-            name: param.get() for name, param in self.default_parameters.items()
+            name: param.get() for name, param in self.dynamic_parameters.items()
         }
 
         local_env = {
             **self.local_env_base,
             **default_parameters,
         }
 
@@ -576,14 +589,17 @@
                 "System %s is in agnostic time mode but is not traced with JAX. Be "
                 "advised that the step code will be evaluated once per output port "
                 "evaluation. Any mutation of the local environment should be strictly "
                 "avoided as it will likely lead to unexpected behavior.",
                 self.name_path_str,
             )
 
+    def initialize(self, **kwargs):
+        pass
+
     @property
     def has_feedthrough_side_effects(self) -> bool:
         # See explanation in `SystemBase.has_ode_side_effects`.
         return self.time_mode == "agnostic"
 
     @staticmethod
     def set_exec_fn(exec_fn: callable):
@@ -598,17 +614,16 @@
         return {
             "__main__": {},
             "true": True,
             "false": False,
         }
 
     def exec_init(self) -> None:
-
         default_parameters = {
-            name: param.get() for name, param in self.default_parameters.items()
+            name: param.get() for name, param in self.dynamic_parameters.items()
         }
 
         local_env = {
             **self.local_env_base,
             **self._parameters,
             **default_parameters,
         }
```

## collimator/library/data_source.py

```diff
@@ -11,14 +11,15 @@
 # <https://www.gnu.org/licenses/>.
 
 """DataSource block for loading data into a simulation from a CSV file."""
 
 import numpy as np
 
 from .generic import SourceBlock
+from ..framework import parameters
 from collimator.lazy_loader import LazyLoader
 from collimator.backend import numpy_api as cnp
 
 pd = LazyLoader("pd", globals(), "pandas")
 
 
 __all__ = [
@@ -100,14 +101,26 @@
             the fixed time step value here.
         data_columns:
             Enter name, index, or slice to select columns from the data file.
         extrapolation: the extrapolation method.  One of "hold" or "zero".
         interpolation: the interpolation method.  One of "zero_order_hold" or "linear".
     """
 
+    @parameters(
+        static=[
+            "file_name",
+            "data_columns",
+            "extrapolation",
+            "header_as_first_row",
+            "interpolation",
+            "sampling_interval",
+            "time_column",
+            "time_samples_as_column",
+        ]
+    )
     def __init__(
         self,
         file_name: str,
         data_columns: str = "1",  # slice, e.g. 3:4
         extrapolation: str = "hold",
         header_as_first_row: bool = False,
         interpolation: str = "zero_order_hold",
@@ -261,25 +274,14 @@
         super().__init__(_func, **kwargs)
 
         if data.size == 0:
             raise ValueError(
                 f"DataSource {self.name} did not succeed in getting the requested data columns."
             )
 
-        self.declare_configuration_parameters(
-            file_name=file_name,
-            data_columns=data_columns,
-            extrapolation=extrapolation,
-            header_as_first_row=header_as_first_row,
-            interpolation=interpolation,
-            sampling_interval=sampling_interval,
-            time_column=time_column,
-            time_samples_as_column=time_samples_as_column,
-        )
-
     def make_time_col(self, start, step, n):
         """
         this function computes the time vector from sample
         interval when this is requested by user
         """
         return np.array([i * step + start for i in range(n)])
```

## collimator/library/fmu_import.py

```diff
@@ -20,15 +20,20 @@
 import jax
 
 from fmpy import read_model_description, extract
 from fmpy.fmi2 import FMU2Slave, FMICallException
 from fmpy.model_description import ScalarVariable
 
 from ..framework.error import BlockRuntimeError
-from ..framework import LeafSystem, BlockInitializationError, DependencyTicket
+from ..framework import (
+    LeafSystem,
+    BlockInitializationError,
+    DependencyTicket,
+    parameters,
+)
 from ..logging import logger
 from ..backend import io_callback, numpy_api as cnp
 
 
 ValueReference = int
 
 
@@ -71,26 +76,25 @@
             )
         except Exception as e:
             logger.error(
                 "Failed to initialize FMU block %s (%s): %s", name, self.system_id, e
             )
             raise BlockInitializationError(str(e), system=self)
 
+    @parameters(static=["file_name"])
     def _init(
         self,
         file_name,
         dt,
         name: str,
         input_names: list[str] = None,
         output_names: list[str] = None,
         parameters: dict = None,
         start_time: float = 0.0,
     ):
-        self.declare_configuration_parameters(file_name=file_name)
-
         self.dt = dt
 
         # read the model description
         model_description = read_model_description(file_name)
 
         # extract the FMU
         unzipdir = extract(file_name)
```

## collimator/library/generic.py

```diff
@@ -10,100 +10,100 @@
 # Affero General Public License along with this program. If not, see
 # <https://www.gnu.org/licenses/>.
 
 from __future__ import annotations
 from typing import Callable
 
 from ..framework import LeafSystem, DependencyTicket
-from ..backend import asarray
 
 __all__ = [
     "SourceBlock",
     "FeedthroughBlock",
     "ReduceBlock",
 ]
 
 
-def _add_parameters(sys, parameters):
-    """Add parameters to a system.
-
-    These will appear in created contexts, hence are optimizable via
-    differentiation through simulations.
-    """
-    for key, val in parameters.items():
-        # Check if the parameter is convertible to an array
-        #   If not, it will be stored as an arbitrary object and it's up
-        #   to the user to handle it appropriately.
-        try:
-            asarray(val)
-            param_as_array = True
-        except TypeError:
-            param_as_array = False
-
-        sys.declare_parameter(key, val, as_array=param_as_array)
-
-
 class SourceBlock(LeafSystem):
     """Simple blocks with a single time-dependent output"""
 
-    def __init__(self, func: Callable, parameters={}, **kwargs):
+    def __init__(self, func: Callable, **kwargs):
         """Create a source block with a time-dependent output.
 
         Args:
             func (Callable):
                 A function of time and parameters that returns a single value.
                 Signature should be `func(time, **parameters) -> Array`.
             name (str): Name of the block.
             system_id (int): Unique ID of the block.
             parameters (dict): Dictionary of parameters to add to the block.
         """
         super().__init__(**kwargs)
+        self._output_port_idx = self.declare_output_port(
+            None,
+            name="out_0",
+            prerequisites_of_calc=[DependencyTicket.time],
+            requires_inputs=False,
+        )
+        self.replace_op(func)
 
-        _add_parameters(self, parameters)
-
+    def replace_op(self, func):
         def _callback(time, state, *inputs, **parameters):
             return func(time, **parameters)
 
-        self.declare_output_port(
+        self.configure_output_port(
+            self._output_port_idx,
             _callback,
-            name="out_0",
             prerequisites_of_calc=[DependencyTicket.time],
             requires_inputs=False,
         )
 
 
 class FeedthroughBlock(LeafSystem):
     """Simple feedthrough blocks with a function of a single input"""
 
     def __init__(self, func, parameters={}, **kwargs):
         super().__init__(**kwargs)
         self.declare_input_port()
+        self._output_port_idx = self.declare_output_port(
+            None,
+            prerequisites_of_calc=[self.input_ports[0].ticket],
+            requires_inputs=True,
+        )
+        self.replace_op(func)
 
-        _add_parameters(self, parameters)
-
+    def replace_op(self, func):
         def _callback(time, state, *inputs, **parameters):
             return func(*inputs, **parameters)
 
-        self.declare_output_port(
+        self.configure_output_port(
+            self._output_port_idx,
             _callback,
             prerequisites_of_calc=[self.input_ports[0].ticket],
             requires_inputs=True,
         )
 
 
 class ReduceBlock(LeafSystem):
     def __init__(self, n_in, op, parameters={}, **kwargs):
         super().__init__(**kwargs)
 
-        _add_parameters(self, parameters)
-
         for i in range(n_in):
             self.declare_input_port()
 
+        self._output_port_idx = self.declare_output_port(
+            None,
+            prerequisites_of_calc=[port.ticket for port in self.input_ports],
+            requires_inputs=True,
+        )
+
+        self.replace_op(op)
+
+    def replace_op(self, op):
         def _compute_output(time, state, *inputs, **parameters):
             return op(inputs, **parameters)
 
-        self.declare_output_port(
+        self.configure_output_port(
+            self._output_port_idx,
             _compute_output,
             prerequisites_of_calc=[port.ticket for port in self.input_ports],
             requires_inputs=True,
         )
```

## collimator/library/linear_system.py

```diff
@@ -15,15 +15,15 @@
 from abc import ABC, abstractmethod
 from functools import partial
 
 import jax
 import jax.numpy as jnp
 from scipy import signal
 
-from ..framework import LeafSystem
+from ..framework import LeafSystem, parameters, Parameter
 from ..logging import logger
 from collimator.lazy_loader import LazyLoader
 from collimator.framework.error import StaticError, ErrorCollector
 from collimator.backend import numpy_api as cnp
 
 control = LazyLoader(
     "control", globals(), "control"
@@ -37,89 +37,88 @@
     "linearize",
     "PID",
     "Derivative",
     "derivative_filter",
 ]
 
 
+def _reshape(A, B, C, D):
+    # Size checks. UI allows vectors, but here we need matrices, so reshape as needed.
+    if len(A.shape) == 1:
+        n = 1
+        A = A.reshape((n, n))
+    else:
+        n = A.shape[0]
+    if len(B.shape) == 1:
+        m = 1
+        B = B.reshape((n, m))
+    else:
+        m = B.shape[1]
+    if len(C.shape) == 1:
+        p = 1
+        C = C.reshape((p, n))
+    else:
+        p = C.shape[0]
+    if len(D.shape) == 1:
+        D = D.reshape((p, m))
+
+    assert A.shape == (n, n)
+    assert B.shape == (n, m)
+    assert C.shape == (p, n)
+    assert D.shape == (p, m)
+
+    return A, B, C, D, n, m, p
+
+
 class LTISystemBase(LeafSystem, ABC):
     """Base class for linear time-invariant systems.
 
     Parameters:
         A: State matrix of size n x n
         B: Input matrix of size n x m
         C: Output matrix of size p x n
         D: Feedthrough matrix of size p x m
         initialize_states: Initial state vector of size n (default: 0)
     """
 
+    # A, B, C, D are dynamic parameters but we modify them in the constructor
+    # so they can't be declared in the decorator.
+    @parameters(dynamic=["initialize_states"])
     def __init__(self, A, B, C, D, initialize_states=None, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
-        if initialize_states is not None:
-            self.declare_parameter("initialize_states", initialize_states)
+        [A, B, C, D] = [
+            cnp.array(mat.get() if isinstance(mat, Parameter) else mat)
+            for mat in [A, B, C, D]
+        ]
 
-        A = cnp.array(A)
-        B = cnp.array(B)
-        C = cnp.array(C)
-        D = cnp.array(D)
-
-        # Size checks. UI allows vectors, but here we need matrices, so reshape as needed.
-        if len(A.shape) == 1:
-            n = 1
-            A = A.reshape((n, n))
-        else:
-            n = A.shape[0]
-        if len(B.shape) == 1:
-            m = 1
-            B = B.reshape((n, m))
-        else:
-            m = B.shape[1]
-        if len(C.shape) == 1:
-            p = 1
-            C = C.reshape((p, n))
-        else:
-            p = C.shape[0]
-        if len(D.shape) == 1:
-            D = D.reshape((p, m))
-
-        assert A.shape == (n, n)
-        assert B.shape == (n, m)
-        assert C.shape == (p, n)
-        assert D.shape == (p, m)
+        (self.A, self.B, self.C, self.D, self.n, self.m, self.p) = _reshape(A, B, C, D)
 
         # Store the matrices as parameters for access from the context.
-        self.declare_parameter("A", A)
-        self.declare_parameter("B", B)
-        self.declare_parameter("C", C)
-        self.declare_parameter("D", D)
-
-        # Store `n` and `p` for subclasses to define state and output
-        self.n = n
-        self.p = p
-
-        # Store the matrices for string representation
-        self.A = A
-        self.B = B
-        self.C = C
-        self.D = D
-
-        self.is_feedthrough = not cnp.allclose(D, 0.0)
-        self.scalar_output = p == 1
+        self.declare_dynamic_parameter("A", self.A)
+        self.declare_dynamic_parameter("B", self.B)
+        self.declare_dynamic_parameter("C", self.C)
+        self.declare_dynamic_parameter("D", self.D)
 
         self.declare_input_port()  # Single input port (u)
 
+    def initialize(self, A, B, C, D, initialize_states=None, **kwargs):
+        (self.A, self.B, self.C, self.D, self.n, self.m, self.p) = _reshape(A, B, C, D)
+
+        self.is_feedthrough = not cnp.allclose(D, 0.0)
+        self.scalar_output = self.p == 1
+
         if initialize_states is None:
-            initialize_states = cnp.zeros(n)
+            initialize_states = cnp.zeros(self.n)
         else:
             initialize_states = cnp.array(initialize_states)
         # Broadcast to size (n,) if only a scalar-valued list, numpy array,
         # jax array, or float is provided at initialization
-        if initialize_states.size == 1 and n > 1:
-            initialize_states = cnp.ones(n) * initialize_states.ravel()
+        if initialize_states.size == 1 and self.n > 1:
+            initialize_states = cnp.ones(self.n) * initialize_states.ravel()
 
         self.initialize_states = initialize_states
 
     @abstractmethod
     def _eval_output(self, time, state, *inputs, **params):
         """Evaluate the output of the system. Contonuous and discrete systems have
         different implementations."""
@@ -166,29 +165,38 @@
         C: Output matrix of size p x n
         D: Feedthrough matrix of size p x m
         initialize_states: Initial state vector of size n (default: 0)
     """
 
     def __init__(self, A, B, C, D, initialize_states=None, *args, **kwargs):
         super().__init__(A, B, C, D, initialize_states, *args, **kwargs)
-
-        self.declare_continuous_state(
-            ode=self.ode,
-            default_value=self.initialize_states,
+        self._output_port_idx = self.declare_output_port(
+            self._eval_output
+        )  # Single output port (y)
+        self._continuous_state_id = (
+            self.declare_continuous_state()
         )  # Single continuous state (x)
 
-        default_output = cnp.zeros(self.p) if self.p > 1 else 0.0
-        self.declare_output_port(
+    def initialize(self, **kwargs):
+        super().initialize(**kwargs)
+        self.configure_output_port(
+            self._output_port_idx,
             self._eval_output,
-            default_value=default_output,
+            default_value=cnp.zeros(self.p) if self.p > 1 else 0.0,
             requires_inputs=self.is_feedthrough,
-        )  # Single output port (y)
+        )
+        self.configure_continuous_state(
+            self._continuous_state_id,
+            ode=self.ode,
+            default_value=self.initialize_states,
+        )
 
     def _eval_output(self, time, state, *inputs, **params):
         x = state.continuous_state
+
         C, D = params["C"], params["D"]
         y = cnp.matmul(C, cnp.atleast_1d(x))
 
         if self.is_feedthrough:
             (u,) = inputs
             y += cnp.matmul(D, cnp.atleast_1d(u))
 
@@ -230,19 +238,23 @@
 
     Parameters:
         num: Numerator polynomial coefficients, in descending powers of s
         den: Denominator polynomial coefficients, in descending powers of s
         initialize_states: Initial state vector (default: 0)
     """
 
+    @parameters(static=["num", "den"])
     def __init__(self, num, den, *args, **kwargs):
         A, B, C, D = signal.tf2ss(num, den)
         super().__init__(A, B, C, D, *args, **kwargs)
-        self.declare_parameter("num", num)
-        self.declare_parameter("den", den)
+
+    def initialize(self, num, den, **kwargs):
+        A, B, C, D = signal.tf2ss(num, den)
+        kwargs.update(A=A, B=B, C=C, D=D)
+        super().initialize(**kwargs)
 
 
 class PID(LTISystem):
     """Continuous-time PID controller.
 
     The PID controller is implemented as a state-space system with matrices
     (A, B, C, D), which are then used to create a (second-order) LTISystem.
@@ -276,45 +288,46 @@
         kp: Proportional gain
         ki: Integral gain
         kd: Derivative gain
         n: Derivative filter coefficient
         initial_state: Initial state of the integral term (default: 0)
     """
 
+    @parameters(dynamic=["kp", "ki", "kd", "n", "initial_state"])
     def __init__(
         self,
         kp,
         ki,
         kd,
         n,
         initial_state=0.0,
-        *args,
         enable_external_initial_state=False,
         **kwargs,
     ):
         if enable_external_initial_state:
             raise NotImplementedError(
                 "External initial state not yet implemented for PID"
             )
 
-        # FIXME: kp, ki, kd, n are not optimizable since they are set in __init__
+        A, B, C, D = self._get_abcd(kp, ki, kd, n)
+        initialize_states = cnp.array([initial_state, 0.0])
+        super().__init__(A, B, C, D, initialize_states=initialize_states, **kwargs)
 
+    def _get_abcd(self, kp, ki, kd, n):
         A = cnp.array([[0.0, 1.0], [0.0, -n]])
         B = cnp.array([[0.0], [1.0]])
         C = cnp.array([(ki * n), ((kp * n + ki) - (kp + kd * n) * n)])
         D = cnp.array([(kp + kd * n)])
+        return A, B, C, D
+
+    def initialize(self, kp, ki, kd, n, initial_state, **kwargs):
+        A, B, C, D = self._get_abcd(kp, ki, kd, n)
         initialize_states = cnp.array([initial_state, 0.0])
-        super().__init__(
-            A, B, C, D, initialize_states=initialize_states, *args, **kwargs
-        )
-        self.declare_parameter("kp", kp)
-        self.declare_parameter("ki", ki)
-        self.declare_parameter("kd", kd)
-        self.declare_parameter("n", n)
-        self.declare_parameter("initial_state", initial_state)
+        kwargs.update(A=A, B=B, C=C, D=D, initialize_states=initialize_states)
+        super().initialize(**kwargs)
 
 
 class Derivative(LTISystem):
     """Causal estimate of the derivative of a signal in continuous time.
 
     This is implemented as a state-space system with matrices (A, B, C, D),
     which are then used to create a (first-order) LTISystem.  Note that this
@@ -335,21 +348,30 @@
     Input ports:
         (0) u: Input (scalar)
 
     Output ports:
         (0) y: Output (scalar), estimating the time derivative du/dt
     """
 
+    @parameters(dynamic=["filter_coefficient"])
     def __init__(self, filter_coefficient=100, *args, **kwargs):
         N = filter_coefficient
         num = [N, 0]
         den = [1, N]
         A, B, C, D = signal.tf2ss(num, den)
         super().__init__(A, B, C, D, *args, **kwargs)
-        self.declare_parameter("filter_coefficient", filter_coefficient)
+
+    def initialize(self, filter_coefficient, **kwargs):
+        N = filter_coefficient
+        num = [N, 0]
+        den = [1, N]
+
+        A, B, C, D = signal.tf2ss(num, den)
+        kwargs.update(A=A, B=B, C=C, D=D)
+        super().initialize(**kwargs)
 
     def check_types(
         self,
         context,
         error_collector: ErrorCollector = None,
     ):
         inputs = self.collect_inputs(context)
@@ -512,33 +534,37 @@
         initialize_states: Initial state vector of size n (default: 0)
     """
 
     def __init__(self, A, B, C, D, dt, initialize_states=None, *args, **kwargs):
         super().__init__(A, B, C, D, initialize_states, *args, **kwargs)
 
         self.dt = dt
-
-        self.declare_discrete_state(
-            default_value=self.initialize_states,
-        )  # Single discrete state (x)
-
         self.declare_periodic_update(
             self._update,
             period=dt,
             offset=0.0,
         )
 
-        default_output = jnp.zeros(self.p) if self.p > 1 else 0.0
-        self.declare_output_port(
+        self._output_port_idx = self.declare_output_port(
+            self._eval_output
+        )  # Single output port (y)
+
+    def initialize(self, **kwargs):
+        super().initialize(**kwargs)
+        self.declare_discrete_state(
+            default_value=self.initialize_states,
+        )  # Single discrete state (x)
+        self.configure_output_port(
+            self._output_port_idx,
             self._eval_output,
-            period=dt,
+            period=self.dt,
             offset=0.0,
-            default_value=default_output,
+            default_value=jnp.zeros(self.p) if self.p > 1 else 0.0,
             requires_inputs=self.is_feedthrough,
-        )  # Single output port (y)
+        )
 
     def _eval_output(self, time, state, *inputs, **params):
         x = state.discrete_state
         C, D = params["C"], params["D"]
         y = jnp.matmul(C, jnp.atleast_1d(x))
 
         if self.is_feedthrough:
@@ -587,12 +613,16 @@
             Numerator polynomial coefficients, in descending powers of z
         den:
             Denominator polynomial coefficients, in descending powers of z
         initialize_states:
             Initial state vector (default: 0)
     """
 
+    @parameters(static=["num", "den"])
     def __init__(self, dt, num, den, initialize_states=None, *args, **kwargs):
         A, B, C, D = signal.tf2ss(num, den)
         super().__init__(A, B, C, D, dt, initialize_states, *args, **kwargs)
-        self.declare_parameter("num", num)
-        self.declare_parameter("den", den)
+
+    def initialize(self, num, den, **kwargs):
+        A, B, C, D = signal.tf2ss(num, den)
+        kwargs.update(A=A, B=B, C=C, D=D)
+        super().initialize(**kwargs)
```

## collimator/library/lqr.py

```diff
@@ -165,40 +165,46 @@
             A function that returns the nominal state vector `x0` at time `t`.
             func_x_0(t)->x0
         func_u_0 : Callable
             A function that returns the nominal control vector `u0` at time `t`.
             func_u_0(t)->u0
         func_x_d : Callable
             A function that returns the desired state vector `xd` at time `t`.
-            func_x_d(t)->xd
+            func_x_d(t)->xd.  If None, assumed to be the same as the nominal trajectory.
         func_u_d : Callable
             A function that returns the desired control vector `ud` at time `t`.
-            func_u_d(t)->ud
+            func_u_d(t)->ud.  If None, assumed to be the same as the nominal trajectory.
     """
 
     def __init__(
         self,
         t0,
         tf,
         plant,
         Qf,
         func_Q,
         func_R,
         func_N,
         func_x_0,
         func_u_0,
-        func_x_d,
-        func_u_d,
+        func_x_d=None,
+        func_u_d=None,
         name=None,
     ):
         super().__init__(name=name)
 
         self.t0 = t0
         self.tf = tf
 
+        if func_x_d is None:
+            func_x_d = func_x_0
+
+        if func_u_d is None:
+            func_u_d = func_u_0
+
         self.func_R = func_R
         self.func_N = func_N
         self.func_x_0 = func_x_0
         self.func_u_0 = func_u_0
         self.func_x_d = func_x_d
         self.func_u_d = func_u_d
```

## collimator/library/nn.py

```diff
@@ -12,150 +12,232 @@
 
 """Minimal example of a neural network block.
 
 This uses equinox to start, but we should generalize to support other
 JAX libraries as well as PyTorch, pending switchable backends.
 """
 
-from functools import partial
-
+import warnings
+import numpy as np
 import jax
+from jax import random
 import jax.numpy as jnp
-import equinox as eqx  # JAX neural network library
-import json
-
-from ..library import FeedthroughBlock, ReduceBlock
+import equinox as eqx
 
+from ..framework import parameters
+from ..library import FeedthroughBlock
 
-# This could probably go into some kind of generic control.py file when we
-# have more blocks like this that are useful for control.
-class QuadraticCost(ReduceBlock):
-    """LQR-type quadratic cost function for a state and input.
 
-    Computes the cost as x'Qx + u'Ru, where Q and R are the cost matrices.
-    In order to compute a running cost, combine this with an `Integrator`
-    or `IntegratorDiscrete` block.
+class MLP(FeedthroughBlock):
     """
+    A feedforward neural network block representing an Equinox multi-layer
+    perceptron (MLP). The output `y` of the MLP is computed as
 
-    def __init__(self, Q, R, name=None):
-        super().__init__(2, self._cost, name=name)
-        self.Q = Q
-        self.R = R
-
-    def _cost(self, inputs):
-        x, u = inputs
-        return jnp.dot(x, jnp.dot(self.Q, x)) + jnp.dot(u, jnp.dot(self.R, u))
-
+    ```
+        y = MLP(x, theta)
+    ```
+
+    where `theta` are the parameters of the MLP, and `x` is the input to the MLP.
+    This block is differentialble w.r.t. the MLP parameters `theta`. Note that `theta`,
+    does not include the hyperparameters representing the architecture of the MLP.
+
+    Input ports:
+        (0) The input to the MLP.
+
+    Output ports:
+        (0) The output of the MLP.
+
+    Parameters:
+        in_size (int):
+            The dimension of the input to the MLP.
+        out_size (int):
+            The dimension of the output of the MLP.
+        width_size (int):
+            The width of every hidden layers of the MLP.
+        depth (int):
+            The depth of the MLP. This represents the number of hidden layers,
+            including the output layer.
+        seed (int):
+            The seed for the random number generator for initialization of the
+            MLP parameters (weights and biases of every layer).
+            If None, a random 32-bit seed will be generated.
+        activation_str (str):
+            The activation function to use after each internal layer of the MLP.
+            Possible values are "relu", "sigmoid", "tanh", "elu", "swish", "rbf",
+            and "identity". Default is "relu".
+        final_activation_str (str):
+            The activation function to use for the output layer of the MLP.
+            Possible values are "relu", "sigmoid", "tanh", "elu", "swish", "rbf",
+            and "identity". Default is "identity".
+        use_bias (bool):
+            Whether to add a bias to the internal layers of the MLP.
+            Default is True.
+        use_final_bias (bool):
+            Wheter to add a bias to the output layer of the MLP.
+            Default is True.
+        file_name (str):
+            Optional file name containing the serialized parameters of the MLP.
+            If provided, the parameters are loaded from the file, and set as the
+            parameters of the MLP. Default is None.
+    """
 
-class MLP(FeedthroughBlock):
+    @parameters(
+        static=[
+            "in_size",
+            "out_size",
+            "width_size",
+            "depth",
+            "seed",
+            "activation_str",
+            "final_activation_str",
+            "use_bias",
+            "use_final_bias",
+            "file_name",
+        ]
+    )
     def __init__(
         self,
-        input_size=None,
-        output_size=None,
+        in_size=None,
+        out_size=None,
         width_size=None,
         depth=None,
-        key=None,
+        seed=None,
         activation_str="relu",
-        final_activation_str=None,
+        final_activation_str="identity",
         use_bias=True,
         use_final_bias=True,
-        name=None,
-        filename=None,
+        file_name=None,
         **kwargs,
     ):
+        """
+        see https://docs.kidger.site/equinox/examples/serialisation/ for rationale
+        of implementation here. We can't serialize the activation function, so we
+        serialize a string representing a selection for activation function amongst
+        a finite set of options.
+        """
+        super().__init__(None, **kwargs)
+        self.initialize(
+            in_size=in_size,
+            out_size=out_size,
+            width_size=width_size,
+            depth=depth,
+            seed=seed,
+            activation_str=activation_str,
+            final_activation_str=final_activation_str,
+            use_bias=use_bias,
+            use_final_bias=use_final_bias,
+            file_name=file_name,
+        )
+
+    def initialize(
+        self,
+        in_size=None,
+        out_size=None,
+        width_size=None,
+        depth=None,
+        seed=None,
+        activation_str="relu",
+        final_activation_str="identity",
+        use_bias=True,
+        use_final_bias=True,
+        file_name=None,
+        mlp_params=None,
+    ):
+        # FIXME: mlp_params will always be overwritten so it can't be optimized for now.
+
+        if in_size is None or out_size is None or width_size is None or depth is None:
+            raise ValueError("Must specify in_size, out_size, width_size, and depth.")
+        else:
+            # Cast to int for safety
+            in_size = int(in_size)
+            out_size = int(out_size)
+            width_size = int(width_size)
+            depth = int(depth)
+
+        # file_name may come as an empty string through json parsing
+        if file_name == "":
+            file_name = None
+
+        # dict maping activation string to function
+        # TODO: Add more activation functions from
+        # https://jax.readthedocs.io/en/latest/jax.nn.html and updae schema
         def _match_activation(activation_str):
-            # match activation_str:
-            #     case "relu":
-            #         return jax.nn.relu
-            #     case "tanh":
-            #         return jnp.tanh
-            #     case _:
-            #         return lambda x: x
-            if activation_str == "relu":
-                return jax.nn.relu
-            elif activation_str == "sigmoid":
-                return jax.nn.sigmoid
-            elif activation_str == "tanh":
-                return jnp.tanh
-            else:
-                return lambda x: x
+            activation_mapping = {
+                "relu": jax.nn.relu,
+                "sigmoid": jax.nn.sigmoid,
+                "tanh": jnp.tanh,
+                "elu": jax.nn.elu,
+                "swish": jax.nn.silu,
+                "rbf": lambda x: jnp.exp(-(x**2)),
+                "identity": lambda x: x,
+            }
+            if activation_str not in activation_mapping:
+                warnings.warn(
+                    f"Provided activation function {activation_str} not recognized. "
+                    "Using Identity function as activation."
+                )
+            return activation_mapping.get(activation_str, lambda x: x)
+
+        seed = np.random.randint(0, 2**32) if seed is None else int(seed)
+        self.key = random.PRNGKey(seed)
 
-        def _make(
+        self.mlp = eqx.nn.MLP(
             in_size,
             out_size,
             width_size,
             depth,
-            key=None,
-            activation_str="relu",
-            final_activation_str=None,
-            use_bias=False,
-            use_final_bias=False,
-        ):
-            """
-            see https://docs.kidger.site/equinox/examples/serialisation/ for rationale
-            of implementation here.
-            cant serialize the activation function, so we serialize a string representing
-            a selection for activation function amongst a finite set of options.
-            """
-            return eqx.nn.MLP(
-                in_size,
-                out_size,
-                width_size,
-                depth,
-                key=key,
-                activation=_match_activation(activation_str),
-                final_activation=_match_activation(final_activation_str),
-                use_bias=use_bias,
-                use_final_bias=use_final_bias,
-            )
-
-        if filename is None:
-            self.net = _make(
-                input_size,
-                output_size,
-                width_size,
-                depth,
-                key=key,
-                activation_str=activation_str,
-                final_activation_str=final_activation_str,
-                use_bias=use_bias,
-                use_final_bias=use_final_bias,
-            )
-            self.activation_str = activation_str
-            self.final_activation_str = final_activation_str
-        else:
-            with open(filename, "rb") as f:
-                hyperparams = json.loads(f.readline().decode())
-                model = _make(key=jax.random.PRNGKey(0), **hyperparams)
-                self.net = eqx.tree_deserialise_leaves(f, model)
-
-        # Keep the NN params in the context, but save static data (functions, etc)
-        nn_params, static = eqx.partition(self.net, eqx.is_array)
-
-        # Declare the parameters as block parameters so that they can be
-        # updated in-context during optimization.
-        block_params = {"nn_params": nn_params}
-
-        def _func(static, inputs, **parameters):
-            net = eqx.combine(parameters["nn_params"], static)
-            return net(inputs)
-
-        super().__init__(
-            partial(_func, static), name=name, parameters=block_params, **kwargs
+            key=self.key,
+            activation=_match_activation(activation_str),
+            final_activation=_match_activation(final_activation_str),
+            use_bias=use_bias,
+            use_final_bias=use_final_bias,
         )
 
-    def serialize(self, filename):
-        nn_params, static = eqx.partition(self.net, eqx.is_array)
-        hyperparams = {
-            "in_size": nn_params.in_size,
-            "out_size": nn_params.out_size,
-            "width_size": nn_params.width_size,
-            "depth": nn_params.depth,
-            "activation_str": self.activation_str,
-            "final_activation_str": self.final_activation_str,
-            "use_bias": nn_params.use_bias,
-            "use_final_bias": nn_params.use_final_bias,
-        }
-        with open(filename, "wb") as f:
-            hyperparam_str = json.dumps(hyperparams)
-            f.write((hyperparam_str + "\n").encode())
-            eqx.tree_serialise_leaves(f, self.net)
+        if file_name is not None:
+            with open(file_name, "rb") as fp:
+                self.mlp = eqx.tree_deserialise_leaves(fp, self.mlp)
+
+        # partition into a pytree of params and static components
+        mlp_params, self.mlp_static = eqx.partition(self.mlp, eqx.is_array)
+
+        if "mlp_params" in self.dynamic_parameters:
+            self.dynamic_parameters["mlp_params"].set(mlp_params)
+        else:
+            self.declare_dynamic_parameter("mlp_params", mlp_params, as_array=False)
+
+        def _eval_MLP(inputs, **parameters):
+            mlp_params = parameters["mlp_params"]
+            mlp = eqx.combine(mlp_params, self.mlp_static)
+            return mlp(inputs)
+
+        self.replace_op(_eval_MLP)
+
+    def serialize(self, file_name, mlp_params=None):
+        """
+        Serialize only the parameters of the MLP. Note that the hyperparameters
+        representing the architecture of the MLP are not serialized. This is because
+        of the following use-cases imagined:
+        (i) The user may train the Equinox MLP outside of Collimator. In this case,
+        it seems unnecessary to force the user to serialize the hyperparameters of the
+        MLP in the strict form chosen by Collimator. It would seem much easier
+        for the user to just input these hyperparameters when creating the MLP block
+        in Collimator UI, and upload the naturally produced serialized parameters file
+        by Equinox.
+        (ii) The user may want to train the Equinox MLP within Collimator in a notebook,
+        and then use the block within Colimator UI. In this case, while serialization of
+        the hyperparameters of the MLP would be a litte more convenient compared
+        to manually inputting the hyperparameters in the UI, it seems like a small
+        convenience relative to disadvantages of (i). Ideally the user should be
+        able to use the API to push the learnt parameters.
+        (iii) When we support training in the UI, the hyperparameters are naturally
+        serialzed with `declare_configuraton_parameters`, and thus, in this case too,
+        only serializatio of the MLP parameters is necessary.
+
+        The choice of an optional `mlp_params` is to enable training of the
+        models in a notebook and easily seralizing them for use in the UI.
+        """
+        if mlp_params is None:
+            mlp = self.mlp
+        else:
+            mlp = eqx.combine(mlp_params, self.mlp_static)
+        with open(file_name, "wb") as f:
+            eqx.tree_serialise_leaves(f, mlp)
```

## collimator/library/predictor.py

```diff
@@ -14,15 +14,15 @@
 import zipfile
 import tempfile
 
 import jax
 import jax.numpy as jnp
 import numpy as np
 
-from ..framework import LeafSystem
+from ..framework import LeafSystem, parameters
 from ..framework.system_base import UpstreamEvalError
 from ..lazy_loader import LazyLoader
 from ..logging import logger
 
 torch = LazyLoader("torch", globals(), "torch")
 tf = LazyLoader("tensorflow", globals(), "tensorflow")
 
@@ -67,34 +67,75 @@
 
         add_batch_dim_to_inputs (bool):
             Whether to add a new first dimension to the inputs before evaluating the
             TorchScript or TensorFlow model. This is useful when the model expects a
             batch dimension.
     """
 
+    @parameters(
+        static=[
+            "file_name",
+            "num_inputs",
+            "num_outputs",
+            "cast_outputs_to_dtype",
+            "add_batch_dim_to_inputs",
+        ]
+    )
     def __init__(
         self,
         file_name,
         num_inputs=1,
         num_outputs=1,
         cast_outputs_to_dtype=None,
         add_batch_dim_to_inputs=False,
         *args,
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
 
-        self.declare_configuration_parameters(
-            file_name=file_name,
+        self._num_inputs = num_inputs
+        self._num_outputs = num_outputs
+
+        for _ in range(num_inputs):
+            self.declare_input_port()
+
+        def _make_output_callback(output_index):
+            def _output_callback(time, state, *inputs, **params):
+                outputs = self._evaluate_output(time, state, *inputs, **params)
+                return outputs[output_index]
+
+            return _output_callback
+
+        for output_index in range(num_outputs):
+            self.declare_output_port(
+                _make_output_callback(output_index),
+                requires_inputs=True,
+            )
+
+        self.initialize(
+            file_name,
             num_inputs=num_inputs,
             num_outputs=num_outputs,
             cast_outputs_to_dtype=cast_outputs_to_dtype,
             add_batch_dim_to_inputs=add_batch_dim_to_inputs,
         )
 
+    def initialize(
+        self,
+        file_name,
+        num_inputs=1,
+        num_outputs=1,
+        cast_outputs_to_dtype=None,
+        add_batch_dim_to_inputs=False,
+    ):
+        if num_inputs != self._num_inputs:
+            raise ValueError("num_inputs can't be changed after initialization")
+        if num_outputs != self._num_outputs:
+            raise ValueError("num_outputs can't be changed after initialization")
+
         self.dtype_output = (
             getattr(jnp, cast_outputs_to_dtype)
             if cast_outputs_to_dtype is not None
             else None
         )
 
         self.add_batch_dim_to_inputs = add_batch_dim_to_inputs
@@ -104,30 +145,14 @@
         if ext == ".pt":
             self.model_format = "TorchScript"
             self.model = torch.jit.load(file_name)
             self.model.eval()
         else:
             raise ValueError(f"Expected extension of file is `.pt`, but found {ext}")
 
-        for _ in range(num_inputs):
-            self.declare_input_port()
-
-        def _make_output_callback(output_index):
-            def _output_callback(time, state, *inputs, **params):
-                outputs = self._evaluate_output(time, state, *inputs, **params)
-                return outputs[output_index]
-
-            return _output_callback
-
-        for output_index in range(num_outputs):
-            self.declare_output_port(
-                _make_output_callback(output_index),
-                requires_inputs=True,
-            )
-
     def initialize_static_data(self, context):
         """Infer the output shapes and dtypes of the ML model."""
         # If building as part of a subsystem, this may not be fully connected yet.
         # That's fine, as long as it is connected by root context creation time.
         # This probably isn't a good long-term solution:
         #   see https://collimator.atlassian.net/browse/WC-51
         try:
@@ -203,76 +228,103 @@
 
         add_batch_dim_to_inputs (bool):
             Whether to add a new first dimension to the inputs before evaluating the
             TorchScript or TensorFlow model. This is useful when the model expects a
             batch dimension.
     """
 
+    @parameters(
+        static=[
+            "file_name",
+            "cast_outputs_to_dtype",
+            "add_batch_dim_to_inputs",
+        ]
+    )
     def __init__(
         self,
         file_name,
         cast_outputs_to_dtype=None,
         add_batch_dim_to_inputs=False,
         *args,
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
-
-        self.declare_configuration_parameters(
-            file_name=file_name,
-            cast_outputs_to_dtype=cast_outputs_to_dtype,
-            add_batch_dim_to_inputs=add_batch_dim_to_inputs,
+        model, num_inputs, num_outputs, num_args, kwargs_signature = self._load_model(
+            file_name
         )
 
-        self.dtype_output = (
-            getattr(jnp, cast_outputs_to_dtype)
-            if cast_outputs_to_dtype is not None
-            else None
-        )
+        self.num_inputs = num_inputs
+        self.num_outputs = num_outputs
 
-        self.add_batch_dim_to_inputs = add_batch_dim_to_inputs
+        for _ in range(self.num_inputs):
+            self.declare_input_port()
 
+        def _make_output_callback(output_index):
+            def _output_callback(time, state, *inputs, **params):
+                outputs = self._evaluate_output(time, state, *inputs, **params)
+                return outputs[output_index]
+
+            return _output_callback
+
+        for output_index in range(self.num_outputs):
+            self.declare_output_port(
+                _make_output_callback(output_index),
+                requires_inputs=True,
+            )
+
+    def _load_model(self, file_name):
         _, ext = os.path.splitext(file_name)
 
         if ext == ".zip":
-            self.model_format = "TFSavedModel"
-
             with tempfile.TemporaryDirectory() as model_dir:
                 with zipfile.ZipFile(file_name, "r") as zip_ref:
                     zip_ref.extractall(model_dir)
 
                 model = tf.saved_model.load(model_dir)
 
-            self.model = model.signatures["serving_default"]
-
-            self.num_args = len(self.model.structured_input_signature[0])
-            self.kwargs_signature = self.model.structured_input_signature[1]
-            self.num_kwargs = len(self.kwargs_signature)
+            model = model.signatures["serving_default"]
 
-            self.num_inputs = self.num_args + self.num_kwargs
-            self.num_outputs = len(self.model.structured_outputs)
+            num_args = len(model.structured_input_signature[0])
+            kwargs_signature = model.structured_input_signature[1]
+            num_kwargs = len(kwargs_signature)
 
+            num_inputs = num_args + num_kwargs
+            num_outputs = len(model.structured_outputs)
         else:
             raise ValueError(f"Expected extension of file is `.zip`, but found {ext}")
 
-        for _ in range(self.num_inputs):
-            self.declare_input_port()
+        return model, num_inputs, num_outputs, num_args, kwargs_signature
 
-        def _make_output_callback(output_index):
-            def _output_callback(time, state, *inputs, **params):
-                outputs = self._evaluate_output(time, state, *inputs, **params)
-                return outputs[output_index]
+    def initialize(
+        self,
+        file_name,
+        cast_outputs_to_dtype=None,
+        add_batch_dim_to_inputs=False,
+    ):
+        self.dtype_output = (
+            getattr(jnp, cast_outputs_to_dtype)
+            if cast_outputs_to_dtype is not None
+            else None
+        )
 
-            return _output_callback
+        self.add_batch_dim_to_inputs = add_batch_dim_to_inputs
 
-        for output_index in range(self.num_outputs):
-            self.declare_output_port(
-                _make_output_callback(output_index),
-                requires_inputs=True,
-            )
+        model, num_inputs, num_outputs, num_args, kwargs_signature = self._load_model(
+            file_name
+        )
+
+        if self.num_inputs != num_inputs:
+            raise ValueError("num_inputs can't be changed after initialization")
+        if self.num_outputs != num_outputs:
+            raise ValueError("num_outputs can't be changed after initialization")
+
+        self.model = model
+        self.num_args = num_args
+        self.kwargs_signature = kwargs_signature
+        self.num_kwargs = len(self.kwargs_signature)
 
     def initialize_static_data(self, context):
         """Infer the output shapes and dtypes of the ML model."""
         # If building as part of a subsystem, this may not be fully connected yet.
         # That's fine, as long as it is connected by root context creation time.
         # This probably isn't a good long-term solution:
         #   see https://collimator.atlassian.net/browse/WC-51
```

## collimator/library/primitives.py

```diff
@@ -33,14 +33,15 @@
 from ..framework.system_base import UpstreamEvalError
 from ..framework import (
     LeafSystem,
     ShapeMismatchError,
     DtypeMismatchError,
     DependencyTicket,
     Parameter,
+    parameters,
 )
 from ..backend import cond, numpy_api as cnp
 from .generic import SourceBlock, FeedthroughBlock, ReduceBlock
 from .linear_system import derivative_filter
 
 if TYPE_CHECKING:
     from ..framework.port import OutputPort
@@ -192,34 +193,37 @@
     Input ports:
         (0..n_in-1) The input signals to add/subtract.
 
     Output ports:
         (0) The sum/difference of the input signals.
     """
 
+    @parameters(static=["operators"])
     def __init__(self, n_in, *args, operators=None, **kwargs):
+        super().__init__(n_in, None, *args, **kwargs)
+        self.initialize(operators)
+
+    def initialize(self, operators):
+        if operators is not None and any(char not in {"+", "-"} for char in operators):
+            raise BlockParameterError(
+                message=f"Adder block {self.name} has invalid operators {operators}. Can only contain '+' and '-'",
+                system=self,
+                parameter_name="operators",
+            )
+
         if operators is None:
             _func = sum
-
         else:
             signs = [1 if op == "+" else -1 for op in operators]
 
             def _func(inputs):
                 signed_inputs = [s * u for (s, u) in zip(signs, inputs)]
                 return sum(signed_inputs)
 
-        super().__init__(n_in, _func, *args, **kwargs)
-        if operators is not None and any(char not in {"+", "-"} for char in operators):
-            name = kwargs.get("name", self.__class__.__name__)
-            raise BlockParameterError(
-                message=f"Adder block {name} has invalid operators {operators}. Can only contain '+' and '-'",
-                system=self,
-                parameter_name="operators",
-            )
-        self.declare_configuration_parameters(operators=operators)
+        self.replace_op(_func)
 
 
 class Chirp(SourceBlock):
     """Produces a signal like the linear method of
 
     https://docs.scipy.org/doc/scipy/reference/generated/scipy.signal.chirp.html
 
@@ -232,25 +236,26 @@
     Input ports:
         None
 
     Output ports:
         (0) The chirp signal.
     """
 
+    @parameters(dynamic=["f0", "f1", "stop_time", "phi"])
     def __init__(self, f0, f1, stop_time, phi=0.0, **kwargs):
+        super().__init__(None, **kwargs)
+        self.initialize(f0, f1, stop_time, phi)
+
+    def initialize(self, f0, f1, stop_time, phi):
         # FIXME: There's an extra factor of 2 that doesn't seem like it's in the SciPy version.
         def _func(time, stop_time, f0, f1, phi):
             f = f0 + (f1 - f0) * time / (2 * stop_time)
             return cnp.cos(f * time + phi)
 
-        super().__init__(_func, **kwargs)
-        self.declare_parameter("stop_time", stop_time)
-        self.declare_parameter("f0", f0)
-        self.declare_parameter("f1", f1)
-        self.declare_parameter("phi", phi)
+        self.replace_op(_func)
 
 
 class Clock(SourceBlock):
     """Source block returning simulation time.
 
     Input ports:
         None
@@ -286,58 +291,55 @@
     Output Ports:
         (0) The result of the comparison (boolean signal)
 
     Events:
         An event is triggered when the output changes from true to false or vice versa.
     """
 
+    @parameters(static=["operator", "atol", "rtol"])
     def __init__(self, atol=1e-5, rtol=1e-8, operator=None, **kwargs):
         super().__init__(**kwargs)
+        self.declare_input_port()
+        self.declare_input_port()
+        self._output_port_idx = self.declare_output_port()
+        self.initialize(atol, rtol, operator)
 
+    def initialize(self, atol, rtol, operator):
         func_lookup = {
             ">": cnp.greater,
             ">=": cnp.greater_equal,
             "<": cnp.less,
             "<=": cnp.less_equal,
             "==": self._equal,
             "!=": self._ne,
         }
 
         if operator not in func_lookup:
-            name = kwargs.get("name", self.__class__.__name__)
             message = (
-                f"Comparator block '{name}' has invalid selection "
+                f"Comparator block '{self.name}' has invalid selection "
                 + f"'{operator}' for parameter 'operator'. Valid options: "
                 + ",".join([k for k in func_lookup.keys()])
             )
             raise BlockParameterError(
                 message=message, system=self, parameter_name="operator"
             )
 
-        self.declare_configuration_parameters(
-            operator=operator,
-            rtol=rtol,
-            atol=atol,
-        )
         self.rtol = rtol
         self.atol = atol
 
-        self.declare_input_port()
-        self.declare_input_port()
-
         compare = func_lookup[operator]
 
         def _compute_output(_time, _state, *inputs, **_params):
             return compare(*inputs)
 
-        self.declare_output_port(
+        self.configure_output_port(
+            self._output_port_idx,
             _compute_output,
             prerequisites_of_calc=[port.ticket for port in self.input_ports],
         )
-
         self.evt_direction = self._process_operator(operator)
 
     def _equal(self, x, y):
         if cnp.issubdtype(x.dtype, cnp.floating):
             return cnp.isclose(x, y, self.rtol, self.atol)
         return x == y
 
@@ -377,28 +379,31 @@
     Input ports:
         None
 
     Output ports:
         (0) The constant value.
     """
 
+    @parameters(dynamic=["value"])
     def __init__(self, value, *args, **kwargs):
         super().__init__(**kwargs)
-        self.declare_parameter("value", value)
+        self._output_port_idx = self.declare_output_port(name="out_0")
+        self.initialize(value)
 
-        self.declare_output_port(
-            self._func,
-            name="out_0",
+    def initialize(self, value):
+        def _func(time, state, *inputs, **parameters):
+            return parameters["value"]
+
+        self.configure_output_port(
+            self._output_port_idx,
+            _func,
             prerequisites_of_calc=[DependencyTicket.nothing],
             requires_inputs=False,
         )
 
-    def _func(self, time, state, *inputs, **parameters):
-        return parameters["value"]
-
 
 class CrossProduct(ReduceBlock):
     """Compute the cross product between the inputs.
 
     See NumPy docs for details:
     https://numpy.org/doc/stable/reference/generated/numpy.cross.html
 
@@ -437,26 +442,27 @@
         (0) The input signal modified by the dead zone.
 
     Events:
         An event is triggered when the signal enters or exits the dead zone
         in either direction.
     """
 
+    @parameters(dynamic=["half_range"])
     def __init__(self, half_range=1.0, **kwargs):
-        super().__init__(
-            self._dead_zone, parameters={"half_range": half_range}, **kwargs
-        )
+        super().__init__(self._dead_zone, **kwargs)
         if half_range <= 0:
-            name = kwargs.get("name", self.__class__.__name__)
             raise BlockParameterError(
-                message=f"DeadZone block {name} has invalid half_range {half_range}. Must be > 0.",
+                message=f"DeadZone block {self.name} has invalid half_range {half_range}. Must be > 0.",
                 system=self,
                 parameter_name="half_range",
             )
 
+    def initialize(self, half_range):
+        pass
+
     def _dead_zone(self, x, **params):
         return cnp.where(abs(x) < params["half_range"], x * 0, x)
 
     def _lower_limit_event_value(self, _time, _state, *inputs, **params):
         (u,) = inputs
         return u + params["half_range"]
 
@@ -548,45 +554,53 @@
             type of filter used to approximate the derivative. The default is "none",
             corresponding to a simple backward difference approximation.
         filter_coefficient:
             The coefficient in the filter (`N` in the equations above). This is only
             used if `filter_type` is not "none". The default is 1.0.
     """
 
+    @parameters(static=["filter_type", "filter_coefficient"])
     def __init__(self, dt, filter_type="none", filter_coefficient=1.0, **kwargs):
         super().__init__(**kwargs)
         self.dt = dt
-
-        self.declare_configuration_parameters(
-            filter_type=filter_type,
-            filter_coefficient=filter_coefficient,
+        self.declare_input_port()
+        self._periodic_update_idx = self.declare_periodic_update()
+        self.deriv_output = self.declare_output_port(
+            period=dt,
+            offset=0.0,
+            prerequisites_of_calc=[self.input_ports[0].ticket],
         )
 
+    def initialize(self, filter_type="none", filter_coefficient=1.0):
         # Determine the coefficients of the filter, if applicable
         # The filter is a pair of two-element array and the filter
         # equation is:
         # a0*y[k] + a1*y[k-1] = b0*u[k] + b1*u[k-1]
         self.filter = derivative_filter(
-            N=filter_coefficient, dt=dt, filter_type=filter_type
+            N=filter_coefficient, dt=self.dt, filter_type=filter_type
         )
 
-        self.declare_input_port()
-
         self.declare_discrete_state(default_value=None, as_array=False)
 
-        self.declare_periodic_update(
+        self.configure_periodic_update(
+            self._periodic_update_idx,
             self._update,
-            period=dt,
+            period=self.dt,
             offset=0.0,
         )
 
-        self.deriv_output = self.declare_output_port(
+        # At t=0 we have no prior information, so the output will
+        # be held from its initial value (zero). At t=dt, we have
+        # a previous sample, so there is enough information to estimate
+        # the derivative.
+        self.configure_output_port(
+            self.deriv_output,
             self._output,
-            period=dt,
-            offset=0.0,
+            period=self.dt,
+            offset=self.dt,
             prerequisites_of_calc=[self.input_ports[0].ticket],
         )
 
     def _output(self, _time, state, *inputs, **_params):
         # Compute the filtered derivative estimate
         (u,) = inputs
         b, a = self.filter
@@ -604,17 +618,17 @@
         # If building as part of a subsystem, this may not be fully connected yet.
         # That's fine, as long as it is connected by root context creation time.
         # This probably isn't a good long-term solution:
         #   see https://collimator.atlassian.net/browse/WC-51
         try:
             u = self.eval_input(context)
             self._default_discrete_state = u
-            self._default_cache[self.deriv_output] = u
             local_context = context[self.system_id].with_discrete_state(u)
-            local_context = local_context.with_cached_value(self.deriv_output, u)
+            self._default_cache[self.deriv_output] = 0 * u
+            local_context = local_context.with_cached_value(self.deriv_output, 0 * u)
             context = context.with_subcontext(self.system_id, local_context)
 
         except UpstreamEvalError:
             logger.debug(
                 "DerivativeDiscrete.initialize_static_data: UpstreamEvalError. "
                 "Continuing without default value initialization."
             )
@@ -686,25 +700,29 @@
     Input ports:
         None
 
     Output ports:
         (0) The dot product of the inputs.
     """
 
+    @parameters(dynamic=["initial_state"])
     def __init__(self, dt, initial_state=True, **kwargs):
         super().__init__(**kwargs)
         self.dt = dt
+        self.declare_output_port(self._output)
+        self._periodic_update_idx = self.declare_periodic_update()
+        self.initialize(initial_state)
 
+    def initialize(self, initial_state):
         self.declare_discrete_state(default_value=initial_state, dtype=cnp.bool_)
-        self.declare_output_port(self._output)
-        self.declare_parameter("initial_state", initial_state)
-        self.declare_periodic_update(
+        self.configure_periodic_update(
+            self._periodic_update_idx,
             self._update,
             period=cnp.inf,
-            offset=dt,
+            offset=self.dt,
         )
 
     def _update(self, time, state, *_inputs, **_params):
         return cnp.logical_not(state.discrete_state)
 
     def _output(self, _time, state, *_inputs, **_params):
         return state.discrete_state
@@ -757,52 +775,62 @@
             The initial value of the output signal.
     """
 
     class DiscreteStateType(NamedTuple):
         prev_input: Array
         output: bool
 
+    @parameters(static=["edge_detection"], dynamic=["initial_state"])
     def __init__(self, dt, edge_detection, initial_state=False, *args, **kwargs):
         super().__init__(*args, **kwargs)
+        self.dt = dt
+        self.declare_input_port()
+
+        # Declare the periodic update
+        self._periodic_update_idx = self.declare_periodic_update()
+
+        # Declare the output port
+        self._output_port_idx = self.declare_output_port(
+            self._output,
+            prerequisites_of_calc=[DependencyTicket.xd, self.input_ports[0].ticket],
+            requires_inputs=False,
+        )
+        self.initialize(edge_detection, initial_state)
 
+    def initialize(self, edge_detection, initial_state):
         # Determine the type of edge detection
         _detection_funcs = {
             "rising": self._detect_rising,
             "falling": self._detect_falling,
             "either": self._detect_either,
         }
         if edge_detection not in _detection_funcs:
             raise ValueError(
                 f"EdgeDetection block {self.name} has invalid selection "
                 f"{edge_detection} for 'edge_detection'"
             )
         self._detect_edge = _detection_funcs[edge_detection]
 
-        self.declare_configuration_parameters(edge_detection=edge_detection)
-        self.declare_parameter("initial_state", initial_state)
-
-        self.declare_input_port()
-
         # The discrete state will contain the previous input value and the output
         self.declare_discrete_state(
             default_value=self.DiscreteStateType(
                 prev_input=initial_state, output=False
             ),
             as_array=False,
         )
-
-        # Declare the periodic update
-        self.declare_periodic_update(
+        self.configure_periodic_update(
+            self._periodic_update_idx,
             self._update,
-            period=dt,
+            period=self.dt,
             offset=0.0,
         )
 
         # Declare the output port
-        self.declare_output_port(
+        self.configure_output_port(
+            self._output_port_idx,
             self._output,
             prerequisites_of_calc=[DependencyTicket.xd, self.input_ports[0].ticket],
             requires_inputs=False,
         )
 
     def _update(self, time, state, *inputs, **params):
         # Update the stored previous state
@@ -854,28 +882,28 @@
         (0) The exponential of the input signal.
 
     Parameters:
         base:
             One of "exp" or "2". Determines the base of the exponential function.
     """
 
+    @parameters(static=["base"])
     def __init__(self, base, **kwargs):
+        super().__init__(None, **kwargs)
+        self.initialize(base)
+
+    def initialize(self, base):
         func_lookup = {"exp": cnp.exp, "2": cnp.exp2}
         if base not in func_lookup:
-            name = kwargs.get("name", self.__class__.__name__)
-            # cannot pass system=self because this error must be raised BEFORE calling super.__init__()
-            # in the case of inheritting from FeedthroughBlock.
-            # if we call super.__init__() first, we get missing key error for func_lookup[base].
             raise BlockParameterError(
-                message=f"Exponent block {name} has invalid selection {base} for 'base'. Valid selections: "
+                message=f"Exponent block {self.name} has invalid selection {base} for 'base'. Valid selections: "
                 + ", ".join([k for k in func_lookup.keys()]),
                 parameter_name="base",
             )
-        super().__init__(func_lookup[base], **kwargs)
-        self.declare_configuration_parameters(base=base)
+        self.replace_op(func_lookup[base])
 
 
 class FilterDiscrete(LeafSystem):
     """Finite Impulse Response (FIR) filter.
 
     Similar to https://docs.scipy.org/doc/scipy/reference/generated/scipy.signal.lfilter.html
     Note: does not implement the IIR filter.
@@ -887,51 +915,54 @@
         (0) The filtered signal.
 
     Parameters:
         b_coefficients:
             Array of filter coefficients.
     """
 
+    @parameters(dynamic=["b_coefficients"])
     def __init__(
         self,
         dt,
         b_coefficients,
         *args,
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
         self.dt = dt
-
         self.declare_input_port()
+        self._periodic_update_idx = self.declare_periodic_update()
+        self._output_port_idx = self.declare_output_port()
+        self.initialize(b_coefficients)
 
+    def initialize(self, b_coefficients):
         initial_state = cnp.zeros(len(b_coefficients) - 1)
         self.declare_discrete_state(default_value=initial_state)
 
         self.is_feedthrough = b_coefficients[0] != 0
-
         prerequisites_of_calc = []
         if self.is_feedthrough:
             prerequisites_of_calc.append(self.input_ports[0].ticket)
 
-        self.declare_periodic_update(
+        self.configure_periodic_update(
+            self._periodic_update_idx,
             self._update,
-            period=dt,
-            offset=dt,
+            period=self.dt,
+            offset=self.dt,
         )
 
-        self.declare_output_port(
+        self.configure_output_port(
+            self._output_port_idx,
             self._output,
-            period=dt,
-            offset=dt,
+            period=self.dt,
+            offset=self.dt,
             requires_inputs=self.is_feedthrough,
             prerequisites_of_calc=prerequisites_of_calc,
         )
 
-        self.declare_parameter("b_coefficients", b_coefficients)
-
     def _update(self, _time, state, u, **_parameters):
         xd = state.discrete_state
         return cnp.concatenate([cnp.atleast_1d(u), xd[:-1]])
 
     def _output(self, time, state, *inputs, **parameters):
         xd = state.discrete_state
         b_coefficients = parameters["b_coefficients"]
@@ -955,17 +986,20 @@
         (0) The input signal multiplied by the gain: `y = gain * u`.
 
     Parameters:
         gain:
             The value to scale the input signal by.
     """
 
+    @parameters(dynamic=["gain"])
     def __init__(self, gain, *args, **kwargs):
         super().__init__(lambda x, gain: gain * x, *args, **kwargs)
-        self.declare_parameter("gain", gain)
+
+    def initialize(self, gain):
+        pass
 
 
 class IfThenElse(LeafSystem):
     """Applies a conditional expression to the input signals.
 
     Given inputs `pred`, `true_val`, and `false_val`, the block computes:
     ```
@@ -1097,14 +1131,24 @@
         An event is triggered when the "hold" port changes.
 
         Another guard is conditionally active when the integrator is in the Zeno
         state, and is triggered when the "reset" port changes from True to False.
         This event is used to exit the Zeno state and resume normal integration.
     """
 
+    @parameters(
+        static=[
+            "enable_reset",
+            "enable_external_reset",
+            "enable_limits",
+            "enable_hold",
+            "reset_on_enter_zeno",
+        ],
+        dynamic=["initial_state", "zeno_tolerance", "lower_limit", "upper_limit"],
+    )
     def __init__(
         self,
         initial_state,
         enable_reset=False,
         enable_limits=False,
         lower_limit=None,
         upper_limit=None,
@@ -1112,55 +1156,31 @@
         enable_external_reset=False,
         zeno_tolerance=1e-6,
         reset_on_enter_zeno=False,
         dtype=None,
         **kwargs,
     ):
         super().__init__(**kwargs)
-
-        self.declare_configuration_parameters(
-            enable_reset=enable_reset,
-            enable_external_reset=enable_external_reset,
-            reset_on_enter_zeno=reset_on_enter_zeno,
-            enable_limits=enable_limits,
-            enable_hold=enable_hold,
-        )
-        self.declare_parameter("initial_state", initial_state)
-        self.declare_parameter("zeno_tolerance", zeno_tolerance)
-
-        # Default initial condition unless modified in context
-        # FIXME: initial_state is not optimizable?
-        if isinstance(initial_state, Parameter):
-            initial_state = initial_state.get()
-        self.x0 = cnp.array(initial_state, dtype=dtype)
-        self.dtype = dtype if dtype is not None else self.x0.dtype
-
-        self.xdot_index = self.declare_input_port(name="in_0")
-        self.declare_continuous_state(
-            default_value=self.x0,
-            ode=self._ode,
-            prerequisites_of_calc=[self.input_ports[self.xdot_index].ticket],
-        )
-
-        # minimum output prereqs
-        prerequisites_of_calc = [DependencyTicket.xc]
-
+        self.dtype = dtype
         self.enable_reset = enable_reset
         self.enable_external_reset = enable_external_reset
-        self.zeno_tolerance = zeno_tolerance
-        self.reset_on_enter_zeno = reset_on_enter_zeno
+        self.enable_hold = enable_hold
         self.discrete_state_type = namedtuple(
             "IntegratorDiscreteState", ["zeno", "counter", "tprev"]
         )
 
-        self.enable_limits = enable_limits
-        self.has_lower_limit = lower_limit is not None
-        self.has_upper_limit = upper_limit is not None
+        self.xdot_index = self.declare_input_port(name="in_0")
 
-        self.enable_hold = enable_hold
+        self.x0 = cnp.array(initial_state, dtype=self.dtype)
+        self.dtype = self.dtype if self.dtype is not None else self.x0.dtype
+        self._continuous_state_idx = self.declare_continuous_state(
+            default_value=self.x0,
+            ode=self._ode,
+            prerequisites_of_calc=[self.input_ports[self.xdot_index].ticket],
+        )
 
         if enable_reset:
             # Boolean input for triggering reset
             self.reset_trigger_index = self.declare_input_port(name="reset_trigger")
             # prerequisites_of_calc.append(
             #     self.input_ports[self.reset_trigger_index].ticket
             # )
@@ -1200,50 +1220,101 @@
             # Optional: reset value defined by external signal
             if enable_external_reset:
                 self.reset_value_index = self.declare_input_port(name="reset_value")
                 # prerequisites_of_calc.append(
                 #     self.input_ports[self.reset_value_index].ticket
                 # )
 
-        self.declare_output_port(
-            self._output,
-            name="out_0",
-            prerequisites_of_calc=prerequisites_of_calc,
-            requires_inputs=False,
-        )
-
         if enable_hold:
             # Boolean input for triggering hold assert/deassert
             self.hold_trigger_index = self.declare_input_port(name="hold_trigger")
 
             def _hold_guard(_time, _state, *inputs, **_params):
                 trigger = inputs[self.hold_trigger_index]
                 return cnp.where(trigger, 1.0, -1.0)
 
             self.declare_zero_crossing(
                 guard=_hold_guard,
                 name="hold",
                 direction="crosses_zero",
             )
 
+        self._output_port_idx = self.declare_output_port(name="out_0")
+
+        self.initialize(
+            initial_state,
+            enable_reset,
+            enable_limits,
+            lower_limit,
+            upper_limit,
+            enable_hold,
+            enable_external_reset,
+            zeno_tolerance,
+            reset_on_enter_zeno,
+        )
+
+    def initialize(
+        self,
+        initial_state,
+        enable_reset=False,
+        enable_limits=False,
+        lower_limit=None,
+        upper_limit=None,
+        enable_hold=False,
+        enable_external_reset=False,
+        zeno_tolerance=1e-6,
+        reset_on_enter_zeno=False,
+    ):
+        if self.enable_reset != enable_reset:
+            raise ValueError("enable_reset cannot be changed after initialization")
+        if self.enable_external_reset != enable_external_reset:
+            raise ValueError(
+                "enable_external_reset cannot be changed after initialization"
+            )
+        if self.enable_hold != enable_hold:
+            raise ValueError("enable_hold cannot be changed after initialization")
+
+        # Default initial condition unless modified in context
+        self.x0 = cnp.array(initial_state, dtype=self.dtype)
+        self.dtype = self.dtype if self.dtype is not None else self.x0.dtype
+
+        self.configure_continuous_state(
+            self._continuous_state_idx,
+            default_value=self.x0,
+            ode=self._ode,
+            prerequisites_of_calc=[self.input_ports[self.xdot_index].ticket],
+        )
+
+        self.zeno_tolerance = zeno_tolerance
+        self.reset_on_enter_zeno = reset_on_enter_zeno
+
+        self.enable_limits = enable_limits
+        self.has_lower_limit = lower_limit is not None
+        self.has_upper_limit = upper_limit is not None
+
+        self.configure_output_port(
+            self._output_port_idx,
+            self._output,
+            prerequisites_of_calc=[DependencyTicket.xc],
+            requires_inputs=False,
+        )
+
         if enable_limits:
             if lower_limit is not None:
-                self.declare_parameter("lower_limit", lower_limit)
 
                 def _lower_limit_guard(_time, state, *_inputs, **params):
                     return state.continuous_state - params["lower_limit"]
 
                 self.declare_zero_crossing(
                     guard=_lower_limit_guard,
                     name="lower_limit",
                     direction="positive_then_non_positive",
                 )
 
             if upper_limit is not None:
-                self.declare_parameter("upper_limit", upper_limit)
 
                 def _upper_limit_guard(_time, state, *_inputs, **params):
                     return state.continuous_state - params["upper_limit"]
 
                 self.declare_zero_crossing(
                     guard=_upper_limit_guard,
                     name="upper_limit",
@@ -1448,55 +1519,49 @@
             the upper and lower limits. Either limit may be disbale by setting its
             value to None.
         ennable_hold:
             If True, the integrator will hold integration when the hold trigger is
             True.
     """
 
+    @parameters(
+        static=[
+            "enable_reset",
+            "enable_external_reset",
+            "enable_limits",
+            "enable_hold",
+        ],
+        dynamic=["initial_state", "lower_limit", "upper_limit"],
+    )
     def __init__(
         self,
         dt,
         initial_state,
         enable_reset=False,
         enable_hold=False,
         enable_limits=False,
         lower_limit=None,
         upper_limit=None,
         enable_external_reset=False,
         dtype=None,
         **kwargs,
     ):
         super().__init__(**kwargs)
-
-        self.declare_configuration_parameters(
-            enable_reset=enable_reset,
-            enable_external_reset=enable_external_reset,
-            enable_limits=enable_limits,
-            enable_hold=enable_hold,
-        )
-        self.declare_parameter("initial_state", initial_state)
-
-        # Default initial condition unless modified in context
         self.dt = dt
-        self.x0 = cnp.array(initial_state, dtype=dtype)
-        self.dtype = dtype if dtype is not None else self.x0.dtype
+        self.dtype = dtype
 
-        # Since the reset is applied to the output port, having this
-        # active makes the block feedthrough with respect to related
-        # input ports.
-        self.is_feedthrough = enable_reset
+        self.enable_reset = enable_reset
+        self.enable_external_reset = enable_external_reset
 
         self.xdot_index = self.declare_input_port(
             name="in_0"
         )  # One vector-valued input
-        self.declare_discrete_state(default_value=self.x0)
-        self.declare_periodic_update(self._update, period=dt, offset=0.0)
 
-        self.enable_reset = enable_reset
-        self.enable_external_reset = enable_external_reset
+        self._periodic_update_idx = self.declare_periodic_update()
+
         if enable_reset:
             self.reset_trigger_index = self.declare_input_port(
                 name="reset_trigger"
             )  # Boolean input for triggering reset
 
             if enable_external_reset:
                 self.reset_value_index = self.declare_input_port(
@@ -1505,34 +1570,75 @@
 
         self.enable_hold = enable_hold
         if enable_hold:
             self.hold_trigger_index = self.declare_input_port(
                 name="hold_trigger"
             )  # Boolean input for triggering hold
 
+        self.state_output_index = self.declare_output_port(name="out_0")
+
+        self.initialize(
+            initial_state,
+            enable_reset,
+            enable_hold,
+            enable_limits,
+            lower_limit,
+            upper_limit,
+            enable_external_reset,
+        )
+
+    def initialize(
+        self,
+        initial_state,
+        enable_reset=False,
+        enable_hold=False,
+        enable_limits=False,
+        lower_limit=None,
+        upper_limit=None,
+        enable_external_reset=False,
+    ):
+        if self.enable_reset != enable_reset:
+            raise ValueError("enable_reset cannot be changed after initialization")
+        if self.enable_external_reset != enable_external_reset:
+            raise ValueError(
+                "enable_external_reset cannot be changed after initialization"
+            )
+        if self.enable_hold != enable_hold:
+            raise ValueError("enable_hold cannot be changed after initialization")
+
+        # Default initial condition unless modified in context
+        self.x0 = cnp.array(initial_state, dtype=self.dtype)
+        self.dtype = self.dtype if self.dtype is not None else self.x0.dtype
+
+        self.declare_discrete_state(default_value=self.x0)
+        self.configure_periodic_update(
+            self._periodic_update_idx, self._update, period=self.dt, offset=0.0
+        )
+
+        # Since the reset is applied to the output port, having this
+        # active makes the block feedthrough with respect to related
+        # input ports.
+        self.is_feedthrough = enable_reset
+
         self.enable_limits = enable_limits
         self.has_lower_limit = lower_limit is not None
         self.has_upper_limit = upper_limit is not None
-        if self.has_lower_limit:
-            self.declare_parameter("lower_limit", lower_limit)
-        if self.has_upper_limit:
-            self.declare_parameter("upper_limit", upper_limit)
 
         prereqs = [DependencyTicket.xd]
         if enable_reset:
             prereqs.append(self.input_ports[self.reset_trigger_index].ticket)
             if enable_external_reset:
                 prereqs.append(self.input_ports[self.reset_value_index].ticket)
 
-        self.state_output_index = self.declare_output_port(
+        self.configure_output_port(
+            self.state_output_index,
             self._output,
-            period=dt,
+            period=self.dt,
             offset=0.0,
             default_value=self.x0,
-            name="out_0",
             prerequisites_of_calc=prereqs,
         )
 
     def _reset(self, *inputs):
         if self.enable_external_reset:
             return inputs[self.reset_value_index]
         return self.x0
@@ -1628,32 +1734,35 @@
 
     Parameters:
         base:
             One of "natural", "2", or "10". Determines the base of the logarithm.
             The default is "natural".
     """
 
+    @parameters(static=["base"])
     def __init__(self, base="natural", **kwargs):
+        super().__init__(None, **kwargs)
+        self.initialize(base)
+
+    def initialize(self, base="natural"):
         func_lookup = {
             "10": cnp.log10,
             "2": cnp.log2,
             "natural": cnp.log,
         }
         if base not in func_lookup:
-            name = kwargs.get("name", self.__class__.__name__)
             # cannot pass system=self because this error must be raised BEFORE calling super.__init__()
             # in the case of inheritting from FeedthroughBlock.
             # if we call super.__init__() first, we get missing key error for func_lookup[base].
             raise BlockParameterError(
-                message=f"Logarithm block {name} has invalid selection {base} for 'base'. Valid selections: "
+                message=f"Logarithm block {self.name} has invalid selection {base} for 'base'. Valid selections: "
                 + ", ".join([k for k in func_lookup.keys()]),
                 parameter_name="base",
             )
-        super().__init__(func_lookup[base], **kwargs)
-        self.declare_configuration_parameters(base=base)
+        self.replace_op(func_lookup[base])
 
 
 class LogicalOperator(LeafSystem):
     """Apply a boolean function elementwise to the input signals.
 
     This block implements the following boolean functions:
         - "or": same as np.logical_or
@@ -1675,47 +1784,65 @@
             The boolean function to apply. One of "or", "and", "not", "nor", "nand",
             or "xor".
 
     Events:
         An event is triggered when the output changes from True to False or vice versa.
     """
 
+    @parameters(static=["function"])
     def __init__(self, function, **kwargs):
         super().__init__(**kwargs)
+        self.declare_input_port()
+        if not function == "not":
+            self.declare_input_port()
+        self._output_port_idx = self.declare_output_port(
+            None,
+            prerequisites_of_calc=[port.ticket for port in self.input_ports],
+            requires_inputs=True,
+        )
+        self.initialize(function)
+
+    def initialize(self, function):
         self.function = function
         func_lookup = {
             "or": self._or,
             "and": self._and,
             "not": self._not,
             "xor": self._xor,
             "nor": self._nor,
             "nand": self._nand,
         }
-        name = kwargs.get("name", self.__class__.__name__)
         if function not in func_lookup:
             raise BlockParameterError(
-                message=f"LogicalOperator block {name} has invalid selection {function} for 'function'. Valid options: "
+                message=f"LogicalOperator block {self.name} has invalid selection {function} for 'function'. Valid options: "
                 + ", ".join([f for f in func_lookup.keys()]),
                 system=self,
             )
 
-        self.declare_input_port()
-        if not function == "not":
-            self.declare_input_port()
+        if function != "not" and len(self.input_ports) < 2:
+            raise BlockParameterError(
+                message=f"Can't change logical operator from 'not' to {function} for block {self.name}",
+                system=self,
+            )
+
+        if function == "not" and len(self.input_ports) > 1:
+            raise BlockParameterError(
+                message=f"Can't change logical operator from {function} to 'not' for block {self.name}",
+                system=self,
+            )
 
         self._func = func_lookup[function]
 
-        self.declare_output_port(
+        self.configure_output_port(
+            self._output_port_idx,
             self._func,
             prerequisites_of_calc=[port.ticket for port in self.input_ports],
             requires_inputs=True,
         )
 
-        self.declare_configuration_parameters(function=function)
-
     def _edge_detection(self, time, state, *inputs, **params):
         outp = self._func(time, state, *inputs, **params)
         return cnp.where(outp, 1.0, -1.0)
 
     def _or(self, time, state, *inputs, **parameters):
         return cnp.logical_or(cnp.array(inputs[0]), jnp.array(inputs[1]))
 
@@ -1769,33 +1896,34 @@
         axis:
             Axis or axes along which a logical OR/AND reduction is performed.
 
     Events:
         An event is triggered when the output changes from True to False or vice versa.
     """
 
+    @parameters(static=["function", "axis"])
     def __init__(self, function, axis=None, **kwargs):
+        super().__init__(None, **kwargs)
+        self.initialize(function, axis=axis)
+
+    def initialize(self, function, axis=None):
         self.function = function
         self.axis = int(axis) if axis is not None else None
         func_lookup = {
             "any": self._any,
             "all": self._all,
         }
-        name = kwargs.get("name", self.__class__.__name__)
         if function not in func_lookup:
             raise BlockParameterError(
-                message=f"LogicalReduce block {name} has invalid selection {function} for 'function'. Valid options: "
+                message=f"LogicalReduce block {self.name} has invalid selection {function} for 'function'. Valid options: "
                 + ", ".join([f for f in func_lookup.keys()])
             )
 
         self._func = func_lookup[function]
-
-        super().__init__(self._func, **kwargs)
-
-        self.declare_configuration_parameters(function=function, axis=axis)
+        self.replace_op(self._func)
 
     def _edge_detection(self, _time, _state, *inputs, **_params):
         outp = self._func(inputs)
         return cnp.where(outp, 1.0, -1.0)
 
     def _any(self, inputs):
         return cnp.any(cnp.array(inputs), axis=self.axis)
@@ -1840,53 +1968,45 @@
             performed by the block.
 
     Notes:
         Currently restricted to 1D input and output data.  This may be expanded to
         support multi-dimensional output arrays in the future.
     """
 
+    @parameters(static=["input_array", "output_array", "interpolation"])
     def __init__(self, input_array, output_array, interpolation, **kwargs):
-        if isinstance(input_array, Parameter):
-            input_array = input_array.get()
-        if isinstance(output_array, Parameter):
-            output_array = output_array.get()
+        super().__init__(None, **kwargs)
+        self.initialize(input_array, output_array, interpolation)
 
+    def initialize(self, input_array, output_array, interpolation):
         self.input_array = cnp.array(input_array)
         self.output_array = cnp.array(output_array)
-        name = kwargs.get("name", self.__class__.__name__)
         if len(self.input_array.shape) != 1:
             raise ValueError(
-                f"LookupTable1d block {name} input_array must be 1D, got shape "
+                f"LookupTable1d block {self.name} input_array must be 1D, got shape "
                 f"{self.input_array.shape}"
             )
         if len(self.output_array.shape) != 1:
             raise ValueError(
-                f"LookupTable1d block {name} output_array must be 1D, got shape "
+                f"LookupTable1d block {self.name} output_array must be 1D, got shape "
                 f"{self.output_array.shape}"
             )
         self.max_i = len(self.input_array) - 1
 
         func_lookup = {
             "linear": self._lookup_linear,
             "nearest": self._lookup_nearest,
             "flat": self._lookup_flat,
         }
         if interpolation not in func_lookup:
             raise ValueError(
-                f"LookupTable1d block {name} has invalid selection {interpolation} "
+                f"LookupTable1d block {self.name} has invalid selection {interpolation} "
                 "for 'interpolation'"
             )
-
-        super().__init__(func_lookup[interpolation], **kwargs)
-
-        self.declare_configuration_parameters(
-            interpolation=interpolation,
-            input_array=input_array,
-            output_array=output_array,
-        )
+        self.replace_op(func_lookup[interpolation])
 
     def _lookup_linear(self, x):
         return cnp.interp(x, self.input_array, self.output_array)
 
     def _lookup_nearest(self, x):
         i = cnp.argmin(cnp.abs(self.input_array - x))
         i = cnp.clip(i, 0, self.max_i)
@@ -1925,72 +2045,66 @@
         output_table_array:
             The array of output values. Must be 2D with shape `(m, n)`, where
             `m = len(input_x_array)` and `n = len(input_y_array)`.
         interpolation:
             Only "linear" is supported.
     """
 
+    @parameters(
+        static=["input_x_array", "input_y_array", "output_table_array", "interpolation"]
+    )
     def __init__(
         self,
         input_x_array,
         input_y_array,
         output_table_array,
         interpolation="linear",
         **kwargs,
     ):
-        if isinstance(input_x_array, Parameter):
-            input_x_array = input_x_array.get()
-        if isinstance(input_y_array, Parameter):
-            input_y_array = input_y_array.get()
-        if isinstance(output_table_array, Parameter):
-            output_table_array = output_table_array.get()
+        super().__init__(2, None, **kwargs)
+        self.initialize(input_x_array, input_y_array, output_table_array, interpolation)
 
+    def initialize(
+        self, input_x_array, input_y_array, output_table_array, interpolation
+    ):
         xp = cnp.array(input_x_array)
         yp = cnp.array(input_y_array)
         zp = cnp.array(output_table_array)
 
-        name = kwargs.get("name", self.__class__.__name__)
         if len(xp.shape) != 1:
             raise ValueError(
-                f"LookupTable2d block {name} input_x_array must be 1D, got "
+                f"LookupTable2d block {self.name} input_x_array must be 1D, got "
                 f"shape {xp.shape}"
             )
 
         if len(yp.shape) != 1:
             raise ValueError(
-                f"LookupTable2d block {name} input_y_array must be 1D, got "
+                f"LookupTable2d block {self.name} input_y_array must be 1D, got "
                 f"shape {yp.shape}"
             )
 
         if len(zp.shape) != 2:
             raise ValueError(
-                f"LookupTable2d block {name} output_table_array must be 2D, "
+                f"LookupTable2d block {self.name} output_table_array must be 2D, "
                 f"got shape {zp.shape}"
             )
 
         if zp.shape != (len(xp), len(yp)):
             raise ValueError(
-                f"LookupTable2d block {name} output_table_array must have "
+                f"LookupTable2d block {self.name} output_table_array must have "
                 f"shape (len(input_x_array), len(input_y_array)), got shape {zp.shape}"
             )
 
         if interpolation != "linear":
             raise NotImplementedError(
-                f"LookupTable2d block {name} only supports linear interpolation."
+                f"LookupTable2d block {self.name} only supports linear interpolation."
             )
 
         _compute_output = partial(self._interp2d, xp, yp, zp)
-        super().__init__(2, _compute_output, **kwargs)
-
-        self.declare_configuration_parameters(
-            interpolation=interpolation,
-            input_x_array=input_x_array,
-            input_y_array=input_y_array,
-            output_table_array=output_table_array,
-        )
+        self.replace_op(_compute_output)
 
     def _interp2d(self, xp, yp, zp, inputs, fill_value=None):
         """
         Bilinear interpolation on a grid.
 
         Args:
             x, y: 1D arrays of point at which to interpolate. Any out-of-bounds
@@ -2059,25 +2173,28 @@
     Input ports:
         (0, 1) The input matrices `A` and `B`
 
     Output ports:
         (0) The concatenation input matrices: e.g. `[A,B]`.
     """
 
+    @parameters(static=["axis"])
     def __init__(self, n_in=2, axis=0, **kwargs):
-        def _func(inputs):
-            return cnp.concatenate((inputs[0], inputs[1]), axis=int(axis))
-
         if n_in != 2:
             raise ValueError(
                 "MatrixConcatenation block only supports two input matrices."
             )
+        super().__init__(2, None, **kwargs)
+        self.initialize(axis)
 
-        super().__init__(2, _func, **kwargs)
-        self.declare_configuration_parameters(axis=axis)
+    def initialize(self, axis):
+        def _func(inputs):
+            return cnp.concatenate((inputs[0], inputs[1]), axis=int(axis))
+
+        self.replace_op(_func)
 
 
 class MatrixInversion(FeedthroughBlock):
     """Compute the matrix inverse of the input signal.
 
     Dispatches to `jax.numpy.inv`, so see the JAX docs for details:
     https://jax.readthedocs.io/en/latest/_autosummary/jax.numpy.linalg.inv.html
@@ -2155,34 +2272,37 @@
 
     Events:
         An event is triggered when the extreme input signal changes.  For example,
         if the block is configured as a "max" block with two inputs and the second
         signal becomes greater than the first, a zero-crossing event will be triggered.
     """
 
+    @parameters(static=["operator"])
     def __init__(self, n_in, operator, **kwargs):
+        super().__init__(n_in, None, **kwargs)
+        self.initialize(operator)
+
+    def initialize(self, operator):
         func_lookup = {
             "max": self._max,
             "min": self._min,
         }
         if operator not in func_lookup:
-            name = kwargs.get("name", self.__class__.__name__)
             # cannot pass system=self because this error must be raised BEFORE calling super.__init__()
             # in the case of inheritting from FeedthroughBlock.
             # if we call super.__init__() first, we get missing key error for func_lookup[base].
             raise BlockParameterError(
-                message=f"MinMax block {name} has invalid selection {operator} for 'operator'. Valid options: "
+                message=f"MinMax block {self.name} has invalid selection {operator} for 'operator'. Valid options: "
                 + ", ".join([f for f in func_lookup.keys()]),
                 parameter_name="operator",
             )
 
         self.operator = operator
 
-        super().__init__(n_in, func_lookup[operator], **kwargs)
-        self.declare_configuration_parameters(operator=operator)
+        self.replace_op(func_lookup[operator])
 
         guard_lookup = {
             "max": self._max_guard,
             "min": self._min_guard,
         }
 
         self._guard = guard_lookup[operator]
@@ -2238,17 +2358,20 @@
         (0) The input signal plus the offset.
 
     Parameters:
         offset:
             The constant offset to add to the input signal.
     """
 
+    @parameters(dynamic=["offset"])
     def __init__(self, offset, *args, **kwargs):
         super().__init__(lambda x, offset: x + offset, *args, **kwargs)
-        self.declare_parameter("offset", offset)
+
+    def initialize(self, offset):
+        pass
 
 
 class PIDDiscrete(LeafSystem):
     """Discrete-time PID controller.
 
     This block implements a discrete-time PID controller with a first-order
     approximation to the integrated error and an optional derivative filter.
@@ -2295,91 +2418,108 @@
 
     class DiscreteStateType(NamedTuple):
         integral: Array
         # Recursive filter memory for the derivative estimate
         e_prev: Array
         e_dot_prev: Array
 
+    @parameters(
+        static=["filter_type", "filter_coefficient"],
+        dynamic=["kp", "ki", "kd", "initial_state"],
+    )
     def __init__(
         self,
         dt,
         kp=1.0,
         ki=1.0,
         kd=1.0,
         initial_state=0.0,
         enable_external_initial_state=False,
         filter_type="none",
         filter_coefficient=1.0,
         **kwargs,
     ):
         super().__init__(**kwargs)
-
-        self.declare_configuration_parameters(
-            filter_type=filter_type,
-            filter_coefficient=filter_coefficient,
-        )
-
-        # Determine the coefficients of the filter, if applicable
-        # The filter is a pair of two-element array and the filter
-        # equation is:
-        # a0*y[k] + a1*y[k-1] = b0*u[k] + b1*u[k-1]
-        self.filter_type = filter_type
-        self.filter = derivative_filter(
-            N=filter_coefficient, dt=dt, filter_type=filter_type
-        )
-
-        self.declare_parameter("kp", kp)
-        self.declare_parameter("ki", ki)
-        self.declare_parameter("kd", kd)
-        self.declare_parameter("dt", dt)
-        self.declare_parameter("initial_state", initial_state)
-
+        self.dt = dt
         self.input_index = self.declare_input_port()
 
-        enable_external_initial_state = enable_external_initial_state
+        self.enable_external_initial_state = enable_external_initial_state
         self.initial_state_index = None
         if enable_external_initial_state:
             self.initial_state_index = self.declare_input_port()
 
+        # Declare the periodic update
+        self._periodic_update_idx = self.declare_periodic_update()
+
+        # Declare an output port for the control signal
+        self.control_output = self.declare_output_port()
+
+        # NOTE:
+        # An extra output port for the derivative value is not strictly necessary,
+        # but the filtered estimate could be resused elsewhere.  Also, having the
+        # previous value saved in the discrete output component of state would allows
+        # it to be reused in the recursive filter without recomputing it as part of
+        # the update step, a minor efficiency gain.  The tradeoff is an extra event
+        # that has to be handled.  This implementation uses one output event and
+        # re-does the derivative calculation when a recursive filter is used, but
+        # we could always do it the other way in the future.
+
+        self.initialize(
+            kp,
+            ki,
+            kd,
+            initial_state,
+            filter_type,
+            filter_coefficient,
+        )
+
+    def initialize(
+        self,
+        kp,
+        ki,
+        kd,
+        initial_state,
+        filter_type,
+        filter_coefficient,
+    ):
         # Declare an internal discrete state
         self.declare_discrete_state(
             default_value=self.DiscreteStateType(
                 integral=initial_state,
                 e_prev=0.0,
                 e_dot_prev=0.0,
             ),
             as_array=False,
         )
 
-        # Declare the periodic update
-        self.declare_periodic_update(
+        self.configure_periodic_update(
+            self._periodic_update_idx,
             self._update,
-            period=dt,
+            period=self.dt,
             offset=0.0,
         )
 
-        # Declare an output port for the control signal
-        self.control_output = self.declare_output_port(
+        # Determine the coefficients of the filter, if applicable
+        # The filter is a pair of two-element array and the filter
+        # equation is:
+        # a0*y[k] + a1*y[k-1] = b0*u[k] + b1*u[k-1]
+        self.filter_type = filter_type
+        self.filter = derivative_filter(
+            N=filter_coefficient, dt=self.dt, filter_type=filter_type
+        )
+
+        self.configure_output_port(
+            self.control_output,
             self._output,
-            period=dt,
+            period=self.dt,
             offset=0.0,
             default_value=initial_state,
             prerequisites_of_calc=[DependencyTicket.xd, self.input_ports[0].ticket],
         )
 
-        # NOTE:
-        # An extra output port for the derivative value is not strictly necessary,
-        # but the filtered estimate could be resused elsewhere.  Also, having the
-        # previous value saved in the discrete output component of state would allows
-        # it to be reused in the recursive filter without recomputing it as part of
-        # the update step, a minor efficiency gain.  The tradeoff is an extra event
-        # that has to be handled.  This implementation uses one output event and
-        # re-does the derivative calculation when a recursive filter is used, but
-        # we could always do it the other way in the future.
-
     def _eval_derivative(self, _time, state, *inputs, **_params):
         # Filtered derivative estimate
 
         e = inputs[self.input_index]  # Error signal from upstream
         e_prev = state.discrete_state.e_prev
         b, a = self.filter  # IIR filter coefficients
 
@@ -2396,30 +2536,29 @@
             # Standard finite difference approximation - no recursion
             e_dot = (b[0] * e + b[1] * e_prev) / a[0]
 
         return e_dot
 
     def _update(self, time, state, *inputs, **params):
         e = inputs[self.input_index]  # Error signal from upstream
-        dt = params["dt"]
 
         # Integrated error signal
         e_int = state.discrete_state.integral
 
         # Update the derivative estimate if needed for a recursive filter.
         if self.filter_type != "none":
             e_dot = self._eval_derivative(time, state, *inputs, **params)
         else:
             # This state entry isn't used for the finite difference estimator.
             # Can just keep the original value as a placeholder.
             e_dot = state.discrete_state.e_dot_prev
 
         # Update the internal state
         return self.DiscreteStateType(
-            integral=e_int + e * dt, e_prev=e, e_dot_prev=e_dot
+            integral=e_int + e * self.dt, e_prev=e, e_dot_prev=e_dot
         )
 
     def _eval_control(self, e, e_int, e_dot, **params):
         # Calculate the control signal for the PID control law
         kp, ki, kd = params["kp"], params["ki"], params["kd"]
         u = kp * e + ki * e_int + kd * e_dot
         return u
@@ -2486,32 +2625,35 @@
         (0) The input signal raised to the power of the exponent.
 
     Parameters:
         exponent:
             The exponent to which the input signal is raised.
     """
 
+    @parameters(static=["exponent"])
     def __init__(self, exponent, **kwargs):
         super().__init__(self._func, **kwargs)
 
         # Note that the exponent here is declared as a configuration
         # parameter and not a context parameter, making it non-differentiable.
         # This is because the derivative rule for the exponent includes a log
         # of the primal input signal, which can cause NaN values during backprop
         # if the input signal is non-positive. Specifically, for `y = u ** p`, the
         # linearization with respect to `p` is `dy = y * log(u) * dp`. If we
         # eventually want to support backprop through this block, we will need
         # to handle the log of the input signal in a way that avoids NaN values.
         # (e.g. with gradient clipping). Tracked in WC-306
-        self.declare_configuration_parameters(exponent=exponent)
+        self.exponent = exponent
+
+    def initialize(self, exponent):
         self.exponent = exponent
 
     def _func(self, *inputs, **parameters):
         (u,) = inputs
-        return u ** self.exponent
+        return u**self.exponent
 
 
 class Product(ReduceBlock):
     """Compute the product and/or quotient of the input signals.
 
     The block will multiply or divide the input signals, depending on the specified
     operators.  For example, if the block has three inputs `u1`, `u2`, and `u3` and
@@ -2533,55 +2675,59 @@
             The default is "*".
         denominator_limit:
             Currently unsupported
         divide_by_zero_behavior:
             Currently unsupported
     """
 
+    @parameters(static=["operators", "denominator_limit", "divide_by_zero_behavior"])
     def __init__(
         self,
         n_in,
         operators=None,  # Expect "**/*", etc
         denominator_limit=None,
         divide_by_zero_behavior=None,
         **kwargs,
     ):
+        super().__init__(n_in, None, **kwargs)
+        self.initialize(operators, denominator_limit, divide_by_zero_behavior)
+
+    def initialize(
+        self,
+        operators=None,  # Expect "**/*", etc
+        denominator_limit=None,
+        divide_by_zero_behavior=None,
+    ):
+        if operators is not None and any(char not in {"*", "/"} for char in operators):
+            raise BlockParameterError(
+                message=f"Product block {self.name} has invalid operators {operators}. Can only contain '*' and '/'",
+                system=self,
+                parameter_name="operators",
+            )
+
         if operators is not None and "/" in operators:
             num_indices = cnp.array(
                 [idx for idx, op in enumerate(operators) if op == "*"]
             )
             den_indices = cnp.array(
                 [idx for idx, op in enumerate(operators) if op == "/"]
             )
 
             def _func(inputs):
                 ain = cnp.array(inputs)
-                num = cnp.take(ain, num_indices)
-                den = cnp.take(ain, den_indices)
-                return cnp.prod(num) / cnp.prod(den)
+                num = cnp.take(ain, num_indices, axis=0)
+                den = cnp.take(ain, den_indices, axis=0)
+                return cnp.prod(num, axis=0) / cnp.prod(den, axis=0)
 
         else:
 
             def _func(inputs):
-                return cnp.prod(cnp.array(inputs))
-
-        super().__init__(n_in, _func, **kwargs)
-        if operators is not None and any(char not in {"*", "/"} for char in operators):
-            name = kwargs.get("name", self.__class__.__name__)
-            raise BlockParameterError(
-                message=f"Product block {name} has invalid operators {operators}. Can only contain '*' and '/'",
-                system=self,
-                parameter_name="operators",
-            )
+                return cnp.prod(cnp.array(inputs), axis=0)
 
-        self.declare_configuration_parameters(
-            operators=operators,
-            denominator_limit=denominator_limit,
-            divide_by_zero_behavior=divide_by_zero_behavior,
-        )
+        self.replace_op(_func)
 
 
 class ProductOfElements(FeedthroughBlock):
     """Compute the product of the elements of the input signal.
 
     Dispatches to `jax.numpy.prod`, so see the JAX docs for details:
     https://jax.readthedocs.io/en/latest/_autosummary/jax.numpy.prod.html
@@ -2619,39 +2765,48 @@
             The fraction of the period during which the pulse is "high".
         period:
             The period of the pulse signal.
         phase_delay:
             Currently unsupported.
     """
 
+    @parameters(dynamic=["amplitude", "pulse_width", "period", "phase_delay"])
     def __init__(
         self, amplitude=1.0, pulse_width=0.5, period=1.0, phase_delay=0.0, **kwargs
     ):
         super().__init__(self._func, **kwargs)
 
-        self.declare_parameter("amplitude", amplitude)
-        self.declare_parameter("pulse_width", pulse_width)
-        self.declare_parameter("period", period)
-
         # Initialize the floating-point tolerance.  This will be machine epsilon
         # for the floating point type of the time variable (determined in the
         # static initialization step).
         self.eps = 0.0
 
         if abs(phase_delay) > 1e-9:
             warnings.warn("Warning. Pulse block phase_delay not implemented.")
 
         # Add a dummy event so that the ODE solver doesn't try to integrate through
         # the discontinuity.
         # ad 2 events, one for the up jump, and one the down jump
         self.declare_discrete_state(default_value=False)
-        self.declare_periodic_update(
-            lambda *args, **kwargs: True, period=period, offset=period
+        self._dummy_periodic_update_idx = self.declare_periodic_update()
+        self._periodic_update_idx = self.declare_periodic_update()
+
+    def initialize(self, amplitude, pulse_width, period, phase_delay):
+        if abs(phase_delay) > 1e-9:
+            warnings.warn("Warning. Pulse block phase_delay not implemented.")
+
+        self.configure_periodic_update(
+            self._dummy_periodic_update_idx,
+            lambda *args, **kwargs: True,
+            period=period,
+            offset=period,
         )
-        self.declare_periodic_update(
+
+        self.configure_periodic_update(
+            self._periodic_update_idx,
             lambda *args, **kwargs: True,
             period=period,
             offset=period + period * pulse_width,
         )
 
     def _func(self, time, **parameters):
         # Add a floating-point tolerance to the modulo operation to avoid
@@ -2686,19 +2841,22 @@
         (0) The quantized output signal, on the same scale as the input signal.
 
     Parameters:
         intervals:
             The number of discrete values into which the input signal is quantized.
     """
 
+    @parameters(dynamic=["interval"])
     def __init__(self, interval, *args, **kwargs):
         super().__init__(
             lambda x, interval: interval * cnp.round(x / interval), *args, **kwargs
         )
-        self.declare_parameter("interval", interval)
+
+    def initialize(self, interval):
+        pass
 
 
 class Relay(LeafSystem):
     """Simple state machine implementing hysteresis behavior.
 
     The input-output map is as follows:
 
@@ -2753,14 +2911,23 @@
         for the opposite transition from ON->OFF.
     """
 
     class State(IntEnum):
         OFF = 0
         ON = 1
 
+    @parameters(
+        dynamic=[
+            "on_threshold",
+            "off_threshold",
+            "on_value",
+            "off_value",
+            "initial_state",
+        ]
+    )
     def __init__(
         self, on_threshold, off_threshold, on_value, off_value, initial_state, **kwargs
     ):
         super().__init__(**kwargs)
 
         self.declare_default_mode(
             self.State.ON if initial_state == on_value else self.State.OFF
@@ -2791,19 +2958,20 @@
         self.declare_zero_crossing(
             guard=_off_guard,
             direction="positive_then_non_positive",
             start_mode=self.State.ON,
             end_mode=self.State.OFF,
         )
 
-        self.declare_parameter("on_threshold", on_threshold)
-        self.declare_parameter("off_threshold", off_threshold)
-        self.declare_parameter("on_value", on_value)
-        self.declare_parameter("off_value", off_value)
-        self.declare_parameter("initial_state", initial_state)
+    def initialize(
+        self, on_threshold, off_threshold, on_value, off_value, initial_state
+    ):
+        self.declare_default_mode(
+            self.State.ON if initial_state == on_value else self.State.OFF
+        )
 
     def _output(self, _time, state, **parameters):
         on_value = parameters["on_value"]
         off_value = parameters["off_value"]
         return cnp.where(state.mode == self.State.ON, on_value, off_value)
 
 
@@ -2827,19 +2995,20 @@
             The value of the output signal at the start time.
         slope:
             The slope of the ramp signal.
         start_time:
             The time at which the ramp signal begins.
     """
 
+    @parameters(dynamic=["start_value", "slope", "start_time"])
     def __init__(self, start_value=0.0, slope=1.0, start_time=1.0, **kwargs):
         super().__init__(self._func, **kwargs)
-        self.declare_parameter("start_time", start_time)
-        self.declare_parameter("start_value", start_value)
-        self.declare_parameter("slope", slope)
+
+    def initialize(self, start_value, slope, start_time):
+        pass
 
     def _func(self, time, **parameters):
         m = parameters["slope"]
         t0 = parameters["start_time"]
         y0 = parameters["start_value"]
         return cnp.where(time >= t0, m * (time - t0) + y0, y0)
 
@@ -2893,54 +3062,62 @@
             is False.
     """
 
     class DiscreteStateType(NamedTuple):
         y_prev: Array
         t_prev: float
 
+    @parameters(
+        static=["enable_dynamic_upper_limit", "enable_dynamic_lower_limit"],
+        dynamic=["upper_limit", "lower_limit"],
+    )
     def __init__(
         self,
         dt,
-        upper_limit=None,
+        upper_limit=np.inf,
         enable_dynamic_upper_limit=False,
-        lower_limit=None,
+        lower_limit=-np.inf,
         enable_dynamic_lower_limit=False,
         **kwargs,
     ):
         super().__init__(**kwargs)
         self.primary_input_index = self.declare_input_port()
         self.enable_dynamic_upper_limit = enable_dynamic_upper_limit
         self.enable_dynamic_lower_limit = enable_dynamic_lower_limit
         self.dt = dt
 
         if enable_dynamic_upper_limit:
             # If dynamic limit, simply ignore the static limit
             self.upper_limit_index = self.declare_input_port()
-        else:
-            if upper_limit is None:
-                upper_limit = np.inf
-            self.declare_parameter("upper_limit", upper_limit)
 
         if enable_dynamic_lower_limit:
             # If dynamic limit, simply ignore the static limit
             self.lower_limit_index = self.declare_input_port()
-        else:
-            if lower_limit is None:
-                lower_limit = -np.inf
-            self.declare_parameter("lower_limit", lower_limit)
 
         self.output_index = self.declare_output_port(
             self._output,
             period=dt,
             offset=0.0,
         )
-        self.declare_configuration_parameters(
-            enable_dynamic_upper_limit=enable_dynamic_upper_limit,
-            enable_dynamic_lower_limit=enable_dynamic_lower_limit,
-        )
+
+    def initialize(
+        self,
+        upper_limit=np.inf,
+        enable_dynamic_upper_limit=False,
+        lower_limit=-np.inf,
+        enable_dynamic_lower_limit=False,
+    ):
+        if enable_dynamic_upper_limit != self.enable_dynamic_upper_limit:
+            raise ValueError(
+                "RateLimiter: enable_dynamic_upper_limit cannot be changed after initialization"
+            )
+        if enable_dynamic_lower_limit != self.enable_dynamic_lower_limit:
+            raise ValueError(
+                "RateLimiter: enable_dynamic_lower_limit cannot be changed after initialization"
+            )
 
     def _output(self, time, state, *inputs, **params):
         y_prev = state.cache[self.output_index]
 
         u = inputs[self.primary_input_index]
 
         t_diff = self.dt
@@ -3037,14 +3214,18 @@
     Events:
         The block will trigger an event when the input signal crosses either the upper
         or lower limit.  For example, if the block is configured with static upper and
         lower limits and the input signal crosses the upper limit, then a zero-crossing
         event will be triggered.
     """
 
+    @parameters(
+        static=["enable_dynamic_upper_limit", "enable_dynamic_lower_limit"],
+        dynamic=["upper_limit", "lower_limit"],
+    )
     def __init__(
         self,
         upper_limit=None,
         enable_dynamic_upper_limit=False,
         lower_limit=None,
         enable_dynamic_lower_limit=False,
         **kwargs,
@@ -3061,34 +3242,44 @@
             self.upper_limit_index = self.declare_input_port()
             prerequisites_of_calc.append(
                 self.input_ports[self.upper_limit_index].ticket
             )
         else:
             if upper_limit is None:
                 upper_limit = np.inf
-            self.declare_parameter("upper_limit", upper_limit)
 
         if enable_dynamic_lower_limit:
             # If dynamic limit, simply ignore the static limit
             self.lower_limit_index = self.declare_input_port()
             prerequisites_of_calc.append(
                 self.input_ports[self.lower_limit_index].ticket
             )
         else:
             if lower_limit is None:
                 lower_limit = -np.inf
-            self.declare_parameter("lower_limit", lower_limit)
 
         self.declare_output_port(
             self._compute_output, prerequisites_of_calc=prerequisites_of_calc
         )
-        self.declare_configuration_parameters(
-            enable_dynamic_upper_limit=enable_dynamic_upper_limit,
-            enable_dynamic_lower_limit=enable_dynamic_lower_limit,
-        )
+
+    def initialize(
+        self,
+        upper_limit=None,
+        enable_dynamic_upper_limit=False,
+        lower_limit=None,
+        enable_dynamic_lower_limit=False,
+    ):
+        if enable_dynamic_lower_limit != self.enable_dynamic_lower_limit:
+            raise ValueError(
+                "enable_dynamic_lower_limit must be the same as the value passed to the constructor"
+            )
+        if enable_dynamic_upper_limit != self.enable_dynamic_upper_limit:
+            raise ValueError(
+                "enable_dynamic_upper_limit must be the same as the value passed to the constructor"
+            )
 
     def _lower_limit_event_value(self, _time, _state, *inputs, **params):
         u = inputs[self.primary_input_index]
         if self.enable_dynamic_lower_limit:
             lim = inputs[self.lower_limit_index]
         else:
             lim = params["lower_limit"]
@@ -3120,18 +3311,22 @@
 
     def initialize_static_data(self, context):
         # Add zero-crossing events so ODE solvers can't try to integrate
         # through a discontinuity. For efficiency, only do this if the output
         # is fed to an ODE block
         if not self.has_zero_crossing_events and is_discontinuity(self.output_ports[0]):
             self.declare_zero_crossing(
-                self._lower_limit_event_value, direction="positive_then_non_positive"
+                self._lower_limit_event_value,
+                direction="positive_then_non_positive",
+                name="llim",
             )
             self.declare_zero_crossing(
-                self._upper_limit_event_value, direction="negative_then_non_negative"
+                self._upper_limit_event_value,
+                direction="negative_then_non_negative",
+                name="ulim",
             )
 
         return super().initialize_static_data(context)
 
 
 class Sawtooth(SourceBlock):
     """Produces a modulated linear sawtooth signal.
@@ -3148,32 +3343,35 @@
     Input ports:
         None
 
     Output ports:
         (0) The sawtooth signal.
     """
 
+    @parameters(dynamic=["amplitude", "frequency", "phase_delay"])
     def __init__(self, amplitude=1.0, frequency=0.5, phase_delay=1.0, **kwargs):
         super().__init__(self._func, **kwargs)
 
-        self.declare_parameter("amplitude", amplitude)
-        self.declare_parameter("frequency", frequency)
-        self.declare_parameter("phase_delay", phase_delay)
-
         # Initialize the floating-point tolerance.  This will be machine epsilon
         # for the floating point type of the time variable (determined in the
         # static initialization step).
         self.eps = 0.0
+        self._periodic_update_idx = self.declare_periodic_update()
 
+    def initialize(self, amplitude, frequency, phase_delay):
         # Add a dummy event so that the ODE solver doesn't try to integrate through
         # the discontinuity.
-        period = 1 / frequency
         self.declare_discrete_state(default_value=False)
-        self.declare_periodic_update(
-            lambda *args, **kwargs: True, period=period, offset=phase_delay
+
+        period = 1 / frequency
+        self.configure_periodic_update(
+            self._periodic_update_idx,
+            lambda *args, **kwargs: True,
+            period=period,
+            offset=phase_delay,
         )
 
     def _func(self, time, **parameters):
         # np.mod((t - phase_delay), (1.0 / frequency)) * amplitude
         period = 1 / parameters["frequency"]
         period_fraction = cnp.mod(time - parameters["phase_delay"] + self.eps, period)
         return period_fraction * parameters["amplitude"]
@@ -3203,15 +3401,20 @@
             set `m=1` expliclty.
         n:
             The number of columns in the output matrix.  If `n` is None, then the
             output will be a vector with shape `(m,)`. To get a column vector of size
             `(m,1)`, set `n=1` expliclty.
     """
 
+    @parameters(static=["m", "n"])
     def __init__(self, m, n, **kwargs):
+        super().__init__(None, **kwargs)
+        self.initialize(m, n)
+
+    def initialize(self, m, n):
         if m is not None:
             m = int(m)
         else:
             m = 0
         if n is not None:
             n = int(n)
         else:
@@ -3220,20 +3423,18 @@
         if m > 0 and n > 0:
             ones_ = cnp.ones((m, n))
         elif m > 0:
             ones_ = cnp.ones((m,))
         elif n > 0:
             ones_ = cnp.ones((n,))
         else:
-            name = kwargs.get("name", self.__class__.__name__)
             raise BlockParameterError(
-                message=f"ScalarBroadcast block {name} at least m or n must not be None or Zero"
+                message=f"ScalarBroadcast block {self.name} at least m or n must not be None or Zero"
             )
-        super().__init__(lambda x: ones_ * x, **kwargs)
-        self.declare_configuration_parameters(m=m, n=n)
+        self.replace_op(lambda x: ones_ * x)
 
 
 class Sine(SourceBlock):
     """Generates a sinusoidal signal.
 
     Given amplitude `a`, frequency `f`, phase `phi`, and bias `b`, the output signal is:
     ```
@@ -3253,21 +3454,20 @@
             The frequency of the sinusoidal signal.
         phase:
             The phase of the sinusoidal signal.
         bias:
             The bias of the sinusoidal signal.
     """
 
+    @parameters(dynamic=["amplitude", "frequency", "phase", "bias"])
     def __init__(self, amplitude=1.0, frequency=1.0, phase=0.0, bias=0.0, **kwargs):
         super().__init__(self._eval, **kwargs)
 
-        self.declare_parameter("amplitude", amplitude)
-        self.declare_parameter("frequency", frequency)
-        self.declare_parameter("phase", phase)
-        self.declare_parameter("bias", bias)
+    def initialize(self, amplitude=1.0, frequency=1.0, phase=0.0, bias=0.0):
+        pass
 
     def _eval(self, t, **parameters):
         a = parameters["amplitude"]
         f = parameters["frequency"]
         phi = parameters["phase"]
         b = parameters["bias"]
         return a * cnp.sin(f * t + phi) + b
@@ -3289,14 +3489,17 @@
             `Slice("1:3")`.
 
     Notes:
         Currently only up to 3-dimensional slices are supported.
     """
 
     def __init__(self, slice_, *args, **kwargs):
+        if isinstance(slice_, Parameter):
+            slice_ = slice_.get()
+
         # if slice was provided as numpy slice object, remove this before validating.
         if slice_.startswith("np.s_"):
             slice_ = slice_[len("np.s_") :]
         # if slice is wrapped in [], remove them temporarily.
         if slice_[0] == "[":
             slice_ = slice_[1:]
         if slice_[-1] == "]":
@@ -3317,15 +3520,25 @@
         np_slice = eval(slice_)
 
         def _func(inp):
             return cnp.array(inp)[np_slice]
 
         super().__init__(_func, *args, **kwargs)
         # declare the configuraion parameter as we would expect the user to pass it in.
-        self.declare_configuration_parameters(slice_=slice_config)
+        self.declare_static_parameters(slice_=slice_config)
+
+        # Avoid printing warning from UI
+        self._initialized = False
+
+    def initialize(self, slice_):
+        if self._initialized:
+            logger.warning(
+                "initialize() for Slice block is not implemented. New configuration will be ignored."
+            )
+        self._initialized = True
 
 
 class SquareRoot(FeedthroughBlock):
     """Compute the square root of the input signal.
 
     Dispatches to `jax.numpy.sqrt`, so see the JAX docs for details:
     https://jax.readthedocs.io/en/latest/_autosummary/jax.numpy.sqrt.html
@@ -3354,18 +3567,21 @@
         (0) The stacked output signal.
 
     Parameters:
         axis:
             The axis along which the input signals are stacked.  Default is 0.
     """
 
+    @parameters(static=["axis"])
     def __init__(self, n_in, axis=0, **kwargs):
-        axis = int(axis)
-        super().__init__(n_in, partial(cnp.stack, axis=axis), **kwargs)
-        self.declare_configuration_parameters(axis=axis)
+        super().__init__(n_in, None, **kwargs)
+        self.initialize(axis)
+
+    def initialize(self, axis):
+        self.replace_op(partial(cnp.stack, axis=int(axis)))
 
 
 class Step(SourceBlock):
     """A step signal.
 
     Given start value `y0`, end value `y1`, and step time `t0`, the
     output signal is:
@@ -3384,26 +3600,28 @@
             The value of the output signal before the step time.
         end_value:
             The value of the output signal after the step time.
         step_time:
             The time at which the step occurs.
     """
 
+    @parameters(dynamic=["start_value", "end_value", "step_time"])
     def __init__(self, start_value=0.0, end_value=1.0, step_time=1.0, **kwargs):
         super().__init__(self._func, **kwargs)
+        self._periodic_update_idx = self.declare_periodic_update()
 
-        self.declare_parameter("step_time", step_time)
-        self.declare_parameter("start_value", start_value)
-        self.declare_parameter("end_value", end_value)
-
+    def initialize(self, start_value, end_value, step_time):
         # Add a dummy event so that the ODE solver doesn't try to integrate through
         # the discontinuity.
         self.declare_discrete_state(default_value=False)
-        self.declare_periodic_update(
-            lambda *args, **kwargs: True, period=np.inf, offset=step_time
+        self.configure_periodic_update(
+            self._periodic_update_idx,
+            lambda *args, **kwargs: True,
+            period=np.inf,
+            offset=step_time,
         )
 
     def _func(self, time, **parameters):
         return cnp.where(
             time >= parameters["step_time"],
             parameters["end_value"],
             parameters["start_value"],
@@ -3472,15 +3690,20 @@
     Parameters:
         function:
             The trigonometric function to apply to the input signal.  Must be one of
             "sin", "cos", "tan", "asin", "acos", "atan", "sinh", "cosh", "tanh",
             "asinh", "acosh", "atanh".
     """
 
+    @parameters(static=["function"])
     def __init__(self, function, **kwargs):
+        super().__init__(None, **kwargs)
+        self.initialize(function)
+
+    def initialize(self, function):
         func_lookup = {
             "sin": cnp.sin,
             "cos": cnp.cos,
             "tan": cnp.tan,
             "asin": cnp.arcsin,
             "acos": cnp.arccos,
             "atan": cnp.arctan,
@@ -3488,23 +3711,20 @@
             "cosh": cnp.cosh,
             "tanh": cnp.tanh,
             "asinh": cnp.arcsinh,
             "acosh": cnp.arccosh,
             "atanh": cnp.arctanh,
         }
         if function not in func_lookup:
-            name = kwargs.get("name", self.__class__.__name__)
             raise BlockParameterError(
-                message=f"Trigonometric block {name} has invalid selection {function} for 'function'. Valid options: "
+                message=f"Trigonometric block {self.name} has invalid selection {function} for 'function'. Valid options: "
                 + ", ".join([f for f in func_lookup.keys()]),
                 parameter_name="function",
             )
-
-        super().__init__(func_lookup[function], **kwargs)
-        self.declare_configuration_parameters(function=function)
+        self.replace_op(func_lookup[function])
 
 
 class UnitDelay(LeafSystem):
     """Hold and delay the input signal by one time step.
 
     This block implements a "unit delay" with the following difference equation
     for internal state `x`, input signal `u`, and output signal `y`:
@@ -3540,30 +3760,39 @@
     Parameters:
         dt:
             The time step of the discrete update.
         initial_state:
             The initial state of the block.  Default is 0.0.
     """
 
+    @parameters(dynamic=["initial_state"])
     def __init__(self, dt, initial_state, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.dt = dt
-
         self.declare_input_port()
+        self._periodic_update_idx = self.declare_periodic_update()
+        self._output_port_idx = self.declare_output_port()
+        self.initialize(initial_state)
+
+    def initialize(self, initial_state):
         self.declare_discrete_state(default_value=initial_state)
-        self.declare_periodic_update(self._update, period=dt, offset=dt)
-        self.declare_output_port(
+
+        self.configure_periodic_update(
+            self._periodic_update_idx, self._update, period=self.dt, offset=self.dt
+        )
+
+        self.configure_output_port(
+            self._output_port_idx,
             self._output,
-            period=dt,
+            period=self.dt,
             offset=0.0,
             requires_inputs=False,
             default_value=initial_state,
             prerequisites_of_calc=[DependencyTicket.xd],
         )
-        self.declare_parameter("initial_state", initial_state)
 
     def _update(self, _time, _state, u, **_params):
         # Every dt seconds, update the state to the current input value
         return u
 
     def _output(self, _time, state, **parameters):
         return state.discrete_state
@@ -3639,20 +3868,31 @@
         (0) The input signal converted to the specified data type.
     Parameters:
         dtype:
             The data type to which the input signal is converted.  Must be a valid
             NumPy data type, e.g. "float32", "int64", etc.
     """
 
+    @parameters(static=["convert_to_type"])
     def __init__(self, convert_to_type, *args, **kwargs):
         self.dtype = np.dtype(convert_to_type)
         super().__init__(
             lambda x: cond(
                 isinstance(x, cnp.ndarray),
                 lambda x: cnp.astype(x, self.dtype),
                 lambda x: cnp.array(x, self.dtype),
                 x,
             ),
             *args,
             **kwargs,
         )
-        self.declare_configuration_parameters(convert_to_type=convert_to_type)
+
+    def initialize(self, convert_to_type):
+        self.dtype = np.dtype(convert_to_type)
+        self.replace_op(
+            lambda x: cond(
+                isinstance(x, cnp.ndarray),
+                lambda x: cnp.astype(x, self.dtype),
+                lambda x: cnp.array(x, self.dtype),
+                x,
+            )
+        )
```

## collimator/library/random.py

```diff
@@ -16,15 +16,15 @@
 from functools import partial
 from typing import TYPE_CHECKING, NamedTuple
 
 from jax import random
 import jax.numpy as jnp
 import numpy as np
 
-from ..framework import LeafSystem
+from ..framework import LeafSystem, parameters
 
 if TYPE_CHECKING:
     from ..backend.typing import Array, DTypeLike, ShapeLike
 
 
 __all__ = [
     "RandomNumber",
@@ -72,41 +72,57 @@
             distribution function.
     """
 
     class RNGState(NamedTuple):
         key: Array
         val: Array
 
+    @parameters(static=["distribution", "seed", "shape"])
     def __init__(
         self,
         dt: float,
         distribution: str = "normal",  # UI only exposes 'normal' for now
         seed: int = None,
         dtype: DTypeLike = None,
         shape: ShapeLike = (),
         name: str = None,
         ui_id: str = None,
         **distribution_parameters,
     ):
         super().__init__(name=name, ui_id=ui_id)
 
         # Declare config parameters for serialization
-        self.declare_configuration_parameters(
-            distribution=distribution,
-            seed=seed,
-            shape=shape,
-            **distribution_parameters,
-        )
+        self.declare_static_parameters(**distribution_parameters)
 
         # Add to the data type if specified.  Since not all distributions
         # support this parameter (though most do), we don't want to do this
         # unconditionally.
         if dtype is not None:
             distribution_parameters["dtype"] = dtype
 
+        self.declare_output_port(
+            self._output,
+            period=dt,
+            offset=0.0,
+        )
+
+        self.declare_periodic_update(
+            self._update,
+            period=dt,
+            offset=0.0,
+        )
+        self.initialize(distribution, seed, shape, **distribution_parameters)
+
+    def initialize(
+        self,
+        distribution: str = "normal",  # UI only exposes 'normal' for now
+        seed: int = None,
+        shape: ShapeLike = (),
+        **distribution_parameters,
+    ):
         # Supposedly all distributions support the shape parameter
         if shape is not None and shape != ():
             distribution_parameters["shape"] = shape
 
         self.rng = partial(getattr(random, distribution), **distribution_parameters)
 
         key = random.PRNGKey(np.random.randint(0, 2**32) if seed is None else seed)
@@ -115,29 +131,16 @@
         # JAX maintains RNG state, we need to keep track of the key as well as the
         # most recently generated value.
         key, subkey = random.split(key)
         default_state = self.RNGState(
             key=key,
             val=self.rng(subkey),  # Initial random number with the right data type
         )
-
         self.declare_discrete_state(default_value=default_state, as_array=False)
 
-        self.declare_output_port(
-            self._output,
-            period=dt,
-            offset=0.0,
-        )
-
-        self.declare_periodic_update(
-            self._update,
-            period=dt,
-            offset=0.0,
-        )
-
     def _output(self, _time, state, *_inputs, **_parameters):
         return state.discrete_state.val
 
     def _update(self, _time, state, *_inputs, **_parameters):
         key, subkey = random.split(state.discrete_state.key)
         return self.RNGState(
             key=key,
@@ -188,60 +191,66 @@
     """
 
     class RNGState(NamedTuple):
         key: Array
         samples: Array
         t_last: float = 0.0
 
+    @parameters(
+        static=["num_samples", "shape", "seed"],
+        dynamic=["correlation_time", "noise_power"],
+    )
     def __init__(
         self,
         correlation_time,
         noise_power: float = 1.0,
         num_samples: int = 10,
         seed: int = None,
         dtype: DTypeLike = None,
         shape: ShapeLike = (),
-        name: str = None,
-        ui_id: str = None,
+        **kwargs,
     ):
-        super().__init__(name=name, ui_id=ui_id)
+        super().__init__(**kwargs)
 
-        self.declare_configuration_parameters(
-            noise_power=noise_power,
-            seed=seed,
-            shape=shape,
-            num_samples=num_samples,
+        self.dtype = dtype
+
+        self.declare_output_port(self._output)
+        self.declare_periodic_update(
+            self._update,
+            period=correlation_time,
+            offset=0.0,
         )
-        self.declare_parameter("correlation_time", correlation_time)
 
-        self.shape = shape
+    def initialize(
+        self,
+        correlation_time,
+        noise_power: float = 1.0,
+        num_samples: int = 10,
+        seed: int = None,
+        shape: ShapeLike = (),
+    ):
+        self.shape = tuple(map(int, shape))
         self.N = num_samples
+
         self.noise_power = noise_power
         self.shift = np.arange(self.N) - (self.N - 1) / 2
-
-        self.rng = partial(random.normal, dtype=dtype)
-        key = random.PRNGKey(np.random.randint(0, 2**32) if seed is None else seed)
+        self.rng = partial(random.normal, dtype=self.dtype)
 
         # The default state is a tuple of (key, samples) pairs.  The continuous-time
         # output signal is reconstructed from the samples using a sinc interpolation.
+        seed = np.random.randint(0, 2**32) if seed is None else int(seed)
+        key = random.PRNGKey(int(seed))
         key, subkey = random.split(key)
         default_state = self.RNGState(
             key=key,
-            samples=self._sample(subkey, shape=(self.N, *self.shape)),
+            samples=self.sample(subkey, shape=(self.N, *self.shape)),
         )
-
         self.declare_discrete_state(default_value=default_state, as_array=False)
-        self.declare_output_port(self._output)
-        self.declare_periodic_update(
-            self._update,
-            period=correlation_time,
-            offset=0.0,
-        )
 
-    def _sample(self, key, shape):
+    def sample(self, key, shape):
         return jnp.sqrt(self.noise_power) * self.rng(key, shape)
 
     def _output(self, time, state, *_inputs, **parameters):
         t_last = state.discrete_state.t_last
 
         # Time relative to the last discrete sample, in units of
         # samples.  This is the argument to the sinc function.
@@ -256,15 +265,15 @@
         samples = jnp.moveaxis(state.discrete_state.samples, 0, -1)
 
         return jnp.sum(samples * jnp.sinc(w), axis=-1)
 
     def _update(self, time, state, *_inputs, **_parameters):
         key, subkey = random.split(state.discrete_state.key)
 
-        new_sample = self._sample(subkey, (1, *self.shape))
+        new_sample = self.sample(subkey, (1, *self.shape))
         samples = jnp.concatenate((state.discrete_state.samples[1:], new_sample))
 
         return self.RNGState(
             key=key,
             samples=samples,
             t_last=time,
         )
```

## collimator/library/reference_subdiagram.py

```diff
@@ -65,37 +65,36 @@
         new_instance_parameters = {}
         if instance_parameters:
             for param_name, param in instance_parameters.items():
                 if param_name not in default_params:
                     raise ValueError(
                         f"Parameter {param_name} not found in parameter definitions."
                     )
-                if isinstance(param, Parameter):
-                    new_instance_parameters[param_name] = Parameter(name=param_name, value=param.value)
-                else:
-                    new_instance_parameters[param_name] = Parameter(name=param_name, value=param)
-
+                new_instance_parameters[param_name] = Parameter(
+                    name=param_name, value=param
+                )
 
         all_params = {**default_params, **new_instance_parameters}
-
         diagram = ReferenceSubdiagram._registry[ref_id](
             *args,
             instance_name=instance_name,
             parameters=all_params,
             **kwargs,
         )
 
         diagram.ref_id = ref_id
+        diagram.instance_parameters = set(new_instance_parameters.keys())
 
         for param in params_def:
-            diagram.declare_parameter(param.name, param)
-
-        # declare_parameter adds all parameters to the instance_parameters
-        # so we need to remove the default parameters and only add the new ones.
-        diagram.instance_parameters = new_instance_parameters
+            if param.name in new_instance_parameters:
+                diagram.declare_dynamic_parameter(
+                    param.name, new_instance_parameters[param.name]
+                )
+            else:
+                diagram.declare_dynamic_parameter(param.name, param)
 
         return diagram
 
     @staticmethod
     def register(
         constructor: Callable[[Any], "Diagram"],
         # FIXME: rename parameter_definitions to default_parameters
```

## collimator/library/rotations.py

```diff
@@ -12,15 +12,20 @@
 
 from __future__ import annotations
 from typing import TYPE_CHECKING, NamedTuple
 from functools import partial
 
 from ..backend import Rotation, numpy_api as cnp
 
-from ..framework import LeafSystem, DependencyTicket, ShapeMismatchError
+from ..framework import (
+    LeafSystem,
+    DependencyTicket,
+    ShapeMismatchError,
+    parameters,
+)
 from ..framework.error import BlockParameterError, ErrorCollector
 
 if TYPE_CHECKING:
     from ..backend.typing import Array
 
 __all__ = [
     "CoordinateRotation",
@@ -176,29 +181,39 @@
             `enable_external_rotation_definition=False`.  Must not be None in that case
         inverse: If `True`, the block will compute the inverse transformation, i.e.
             if the matrix representation of the rotation is `C_AB` from frame `B` to
             frame `A`, the block will compute the inverse transformation
             `C_BA = C_AB⁻¹ = C_AB.T`
     """
 
+    @parameters(
+        static=[
+            "quaternion",
+            "roll_pitch_yaw",
+            "direction_cosine_matrix",
+            "rotation_type",
+            "enable_external_rotation_definition",
+            "inverse",
+        ]
+    )
     def __init__(
         self,
         rotation_type,
         enable_external_rotation_definition=True,
         quaternion=None,
         roll_pitch_yaw=None,
         direction_cosine_matrix=None,
         inverse=False,
         **kwargs,
     ):
         super().__init__(**kwargs)
 
-        self.rotation_type = rotation_type
         self.external_rotation = enable_external_rotation_definition
-        self.inverse = inverse
+
+        self.vector_input_index = self.declare_input_port()
 
         # Note: all of the possible rotation specifications are passed as parameters
         # to make the serialization work, but only one is valid at a time. This makes
         # sense from the UI, but is a bit strange when working directly with the code.
         # In any case, the typical use case is to have the external rotation port
         # enabled, so all of these should usually be None.  If more than one is
         # provided (which can happen for instance via hidden parameters in the JSON)
@@ -207,37 +222,72 @@
         rotation = self._check_config(
             rotation_type,
             quaternion,
             roll_pitch_yaw,
             direction_cosine_matrix,
         )
 
-        self.vector_input_index = self.declare_input_port()
-
         if enable_external_rotation_definition:
             self.rotation_input_index = self.declare_input_port()
 
         else:
             # Store the static rotation as a parameter (will be None if external
             # rotation is enabled)
-            self.declare_parameter("rotation", rotation)
+            self.declare_dynamic_parameter("rotation", rotation)
 
-        self.declare_output_port(
-            self._output_func,
+        self._output_port_idx = self.declare_output_port(
             prerequisites_of_calc=[port.ticket for port in self.input_ports],
         )
+        self.initialize(
+            rotation_type,
+            enable_external_rotation_definition,
+            quaternion,
+            roll_pitch_yaw,
+            direction_cosine_matrix,
+            inverse,
+        )
 
-        # Serialization
-        self.declare_configuration_parameters(
-            quaternion=quaternion,
-            roll_pitch_yaw=roll_pitch_yaw,
-            direction_cosine_matrix=direction_cosine_matrix,
-            rotation_type=rotation_type,
-            enable_external_rotation_definition=enable_external_rotation_definition,
-            inverse=inverse,
+    def initialize(
+        self,
+        rotation_type,
+        enable_external_rotation_definition,
+        quaternion,
+        roll_pitch_yaw,
+        direction_cosine_matrix,
+        inverse,
+        rotation=None,
+    ):
+        if enable_external_rotation_definition != self.external_rotation:
+            raise ValueError("Cannot change external rotation definition.")
+
+        self.rotation_type = rotation_type
+        self.inverse = inverse
+        if not self.external_rotation:
+            rotation = self._check_config(
+                rotation_type,
+                quaternion,
+                roll_pitch_yaw,
+                direction_cosine_matrix,
+            )
+
+            def _output_func(_time, _state, *inputs, **parameters):
+                vector = inputs[self.vector_input_index]
+                return self._apply(rotation, vector)
+
+        else:
+
+            def _output_func(_time, _state, *inputs, **parameters):
+                vector = inputs[self.vector_input_index]
+                rotation = inputs[self.rotation_input_index]
+                return self._apply(rotation, vector)
+
+        self.configure_output_port(
+            self._output_port_idx,
+            _output_func,
+            prerequisites_of_calc=[port.ticket for port in self.input_ports],
         )
 
     def _check_config(
         self, rotation_type, quaternion, roll_pitch_yaw, direction_cosine_matrix
     ):
         if rotation_type not in ("quaternion", "roll_pitch_yaw", "DCM"):
             message = f"Invalid rotation type: {rotation_type}."
@@ -320,22 +370,14 @@
         }[self.rotation_type](rotation)
 
         if self.inverse:
             rot = rot.inv()
 
         return rot.apply(vector)
 
-    def _output_func(self, _time, _state, *inputs, **parameters):
-        vector = inputs[self.vector_input_index]
-        if self.external_rotation:
-            rotation = inputs[self.rotation_input_index]
-        else:
-            rotation = parameters["rotation"]
-        return self._apply(rotation, vector)
-
     def check_types(
         self,
         context,
         error_collector: ErrorCollector = None,
     ):
         vec = self.input_ports[self.vector_input_index].eval(context)
 
@@ -390,53 +432,56 @@
 
     Parameters:
         conversion_type (str): The type of rotation conversion to perform.
             Must be one of ("quaternion_to_euler", "quaternion_to_dcm",
             "euler_to_quaternion", "euler_to_dcm", "dcm_to_quaternion", "dcm_to_euler")
     """
 
+    @parameters(static=["conversion_type"])
     def __init__(self, conversion_type, **kwargs):
         super().__init__(**kwargs)
+        self.declare_input_port()
+        self._output_port_idx = self.declare_output_port(requires_inputs=True)
+        self.initialize(conversion_type)
 
+    def initialize(self, conversion_type):
         if conversion_type not in (
             "quaternion_to_RPY",
             "quaternion_to_DCM",
             "RPY_to_quaternion",
             "RPY_to_DCM",
             "DCM_to_quaternion",
             "DCM_to_RPY",
         ):
             message = f"Invalid rotation conversion type: {conversion_type}."
             raise BlockParameterError(
                 message=message, system=self, parameter_name="conversion_type"
             )
 
-        self.declare_input_port()
-
         _func = {
             "quaternion_to_RPY": quat_to_euler,
             "quaternion_to_DCM": quat_to_dcm,
             "RPY_to_quaternion": euler_to_quat,
             "RPY_to_DCM": euler_to_dcm,
             "DCM_to_quaternion": dcm_to_quat,
             "DCM_to_RPY": dcm_to_euler,
         }[conversion_type]
 
         def _output(_time, _state, *inputs, **_parameters):
             (u,) = inputs
             return _func(u)
 
-        self.declare_output_port(
+        self.configure_output_port(
+            self._output_port_idx,
             _output,
             requires_inputs=True,
         )
 
         # Serialization
         self.conversion_type = conversion_type
-        self.declare_configuration_parameters(conversion_type=conversion_type)
 
     def check_types(
         self,
         context,
         error_collector: ErrorCollector = None,
     ):
         rot = self.input_ports[0].eval(context)
@@ -575,14 +620,25 @@
         angular_velocity: Array
 
         def asarray(self):
             return cnp.concatenate(
                 [self.position, self.orientation, self.velocity, self.angular_velocity]
             )
 
+    @parameters(
+        static=[
+            "initial_position",
+            "initial_orientation",
+            "initial_velocity",
+            "initial_angular_velocity",
+            "enable_external_mass",
+            "enable_external_inertia_matrix",
+            "enable_output_state_derivatives",
+        ],
+    )
     def __init__(
         self,
         initial_position,
         initial_orientation,
         initial_velocity,
         initial_angular_velocity,
         enable_external_mass=False,
@@ -591,24 +647,32 @@
         inertia_matrix=None,
         enable_output_state_derivatives=False,
         gravity_vector=None,
         **kwargs,
     ):
         super().__init__(**kwargs)
 
+        self._enable_external_mass = enable_external_mass
+        self._enable_external_inertia_matrix = enable_external_inertia_matrix
+        self._enable_output_state_derivatives = enable_output_state_derivatives
+
         # Process mass and intertia matrices
         if not enable_external_mass:
             if mass is None:
                 mass = 1.0
-            self.declare_parameter("mass", mass)
+            self.declare_dynamic_parameter("mass", mass)
+        else:
+            self.declare_static_parameters(mass=mass)
 
         if not enable_external_inertia_matrix:
             if inertia_matrix is None:
                 inertia_matrix = cnp.eye(3)
-            self.declare_parameter("inertia_matrix", inertia_matrix)
+            self.declare_dynamic_parameter("inertia_matrix", inertia_matrix)
+        else:
+            self.declare_static_parameters(inertia_matrix=inertia_matrix)
 
         # Process gravity vector
         if gravity_vector is None:
             gravity_vector = cnp.zeros(3)
         else:
             gravity_vector = cnp.asarray(gravity_vector)
             if gravity_vector.shape != (3,):
@@ -616,47 +680,100 @@
                     "Gravity vector must have shape (3,), but has shape "
                     + f"{gravity_vector.shape}."
                 )
                 raise BlockParameterError(
                     message=message, system=self, parameter_name="gravity_vector"
                 )
 
-        self.declare_parameter("gravity_vector", gravity_vector)
+        self.declare_dynamic_parameter("gravity_vector", gravity_vector)
 
         initial_state = self._make_initial_state(
             initial_position,
             initial_orientation,
             initial_velocity,
             initial_angular_velocity,
         )
 
-        self.declare_continuous_state(
+        self._continuous_state_idx = self.declare_continuous_state(
             default_value=initial_state,
             as_array=False,
             ode=self._state_derivative,
         )
 
         self._configure_ports(
             initial_state,
             enable_external_mass,
             enable_external_inertia_matrix,
             enable_output_state_derivatives,
         )
 
-        self.declare_configuration_parameters(
-            initial_position=initial_position,
-            initial_orientation=initial_orientation,
-            initial_velocity=initial_velocity,
-            initial_angular_velocity=initial_angular_velocity,
-            enable_external_mass=enable_external_mass,
-            mass=mass,
-            enable_external_inertia_matrix=enable_external_inertia_matrix,
-            inertia_matrix=inertia_matrix,
-            enable_output_state_derivatives=enable_output_state_derivatives,
-            gravity_vector=gravity_vector,
+    def initialize(
+        self,
+        initial_position,
+        initial_orientation,
+        initial_velocity,
+        initial_angular_velocity,
+        enable_external_mass,
+        enable_external_inertia_matrix,
+        enable_output_state_derivatives,
+        mass,
+        inertia_matrix,
+        gravity_vector,
+    ):
+        if enable_external_mass != self._enable_external_mass:
+            raise ValueError("Cannot change external mass definition.")
+        if enable_external_inertia_matrix != self._enable_external_inertia_matrix:
+            raise ValueError("Cannot change external inertia matrix definition.")
+        if enable_output_state_derivatives != self._enable_output_state_derivatives:
+            raise ValueError("Cannot change output state derivatives definition.")
+
+        initial_state = self._make_initial_state(
+            initial_position,
+            initial_orientation,
+            initial_velocity,
+            initial_angular_velocity,
+        )
+
+        self.configure_continuous_state(
+            self._continuous_state_idx,
+            default_value=initial_state,
+            as_array=False,
+            ode=self._state_derivative,
+        )
+
+        self.configure_output_port(
+            self.pos_output_index,
+            self._pos_output,
+            prerequisites_of_calc=[DependencyTicket.xc],
+            requires_inputs=False,
+            default_value=initial_state.position,
+        )
+
+        self.configure_output_port(
+            self.orientation_output_index,
+            self._orientation_output,
+            prerequisites_of_calc=[DependencyTicket.xc],
+            requires_inputs=False,
+            default_value=initial_state.orientation,
+        )
+
+        self.configure_output_port(
+            self.vel_output_index,
+            self._vel_output,
+            prerequisites_of_calc=[DependencyTicket.xc],
+            requires_inputs=False,
+            default_value=initial_state.velocity,
+        )
+
+        self.configure_output_port(
+            self.ang_vel_output_index,
+            self._ang_vel_output,
+            prerequisites_of_calc=[DependencyTicket.xc],
+            requires_inputs=False,
+            default_value=initial_state.angular_velocity,
         )
 
     def _make_initial_state(
         self,
         initial_position,
         initial_orientation,
         initial_velocity,
```

## collimator/library/sindy.py

```diff
@@ -10,292 +10,553 @@
 # Affero General Public License along with this program. If not, see
 # <https://www.gnu.org/licenses/>.
 
 """
 Wrappers for PySINDy
 """
 
+import warnings
 import numpy as np
 import json
-import jax.numpy as jnp
 
-from collimator.framework import LeafSystem
+from ..backend import numpy_api as cnp
+from ..logging import logger
+
+from collimator.framework import LeafSystem, parameters
 from collimator.lazy_loader import LazyLoader
 
-pd = LazyLoader("pd", globals(), "pandas")
+from .utils import read_csv, extract_columns
+
 ps = LazyLoader("ps", globals(), "pysindy")
 sp = LazyLoader("sp", globals(), "sympy")
 
 
 __all__ = [
-    "ContinuousTimeSindyWithControl",
+    "Sindy",
 ]
 
 
-def _read_csv(file_path):
-    """Reads a CSV file and returns a DataFrame."""
-    try:
-        return pd.read_csv(file_path)
-    except Exception as e:
-        raise IOError(f"Error reading {file_path}: {e}")
-
-
-def _extract_columns(data, cols):
-    """Extracts columns from the DataFrame based on names or indices."""
-    if cols is None:
-        return None
-
-    if isinstance(cols, (str, int)):
-        cols = [cols]  # convert to list if a single column name/index is provided
-
-    if isinstance(cols, (list, tuple)):
-        extracted_cols = []
-        for col in cols:
-            if isinstance(col, str) and col in data.columns:
-                extracted_cols.append(data[col])
-            elif isinstance(col, int) and col in range(data.shape[1]):
-                extracted_cols.append(data.iloc[:, col])
-            else:
-                raise ValueError(f"Column {col} not found in data")
-
-        return np.column_stack(extracted_cols)
-    else:
-        raise ValueError(
-            "Columns must be specified as strings, integers, "
-            "or a list/tuple of strings/integers"
-        )
-
-
-def _reduce(feature_names, coefficients):
+def _reduce(base_feature_names, feature_names, coefficients):
     """
-    Reduce the sparse SINDyc coefficients
+    Reduce the sparse SINDy coefficients
     by removing columns with all zeros
     """
+    nx, _ = coefficients.shape
+    nxu = len(base_feature_names)
+
     # Identify zero columns
-    zero_columns = jnp.all(coefficients == 0, axis=0)
+    zero_columns = cnp.all(coefficients == 0, axis=0)
 
     # Filter out zero columns from coefficients
     coefficients_filtered = coefficients[:, ~zero_columns]
 
     # Filter out corresponding feature names
     feature_names_filtered = [
         name for name, is_zero in zip(feature_names, zero_columns) if not is_zero
     ]
 
+    # Handle the case where all coefficients are zero
+    if len(feature_names_filtered) == 0:
+        feature_names_filtered = base_feature_names
+        coefficients_filtered = cnp.zeros((nx, nxu))
+
     return feature_names_filtered, coefficients_filtered
 
 
 def train(
     x_train,
-    u_train,
-    x_dot_train,
-    time,
+    u_train=None,
+    x_dot_train=None,
+    time=None,
+    discrete_time=False,
+    differentiation_method=None,
     poly_order=None,
     fourier_n_frequencies=None,
     threshold=0.1,
+    alpha=0.05,
+    max_iter=20,
+    normalize_columns=False,
 ):
-    """Train the SINDyc model"""
+    """Train the SINDy model"""
     library = []
 
     if poly_order is not None:
         library.append(ps.PolynomialLibrary(degree=poly_order))
 
     if fourier_n_frequencies is not None:
         library.append(ps.FourierLibrary(n_frequencies=fourier_n_frequencies))
 
     optimizer = ps.STLSQ(
-        threshold=threshold, alpha=0.05, max_iter=50, normalize_columns=False
+        threshold=threshold,
+        alpha=alpha,
+        max_iter=max_iter,
+        normalize_columns=normalize_columns,
     )
 
+    if differentiation_method is None:
+        differentiation_method = "centered difference"
+
+    ## TODO: Add support for other differentiation methods. Accept strings as input
+    ## and convert them to appropriate differentiation objects.
+    differentiation_objects_map = {
+        "centered difference": ps.differentiation.FiniteDifference(order=2, axis=0),
+    }
+
     model = ps.SINDy(
         optimizer=optimizer,
         feature_library=ps.feature_library.GeneralizedLibrary(library),
+        differentiation_method=differentiation_objects_map[differentiation_method],
+        discrete_time=discrete_time,
     )
 
+    # Convert cnp arrays to numpy arrays explicitly for Sindy fit
+    x_train = np.array(x_train)
+
+    if u_train is not None:
+        u_train = np.array(u_train)
+
+    if x_dot_train is not None:
+        x_dot_train = np.array(x_dot_train)
+
+    time = np.array(time) if isinstance(time, cnp.ndarray) else time
+
     model.fit(x_train, u=u_train, x_dot=x_dot_train, t=time, quiet=True)
 
     base_feature_names = model.feature_names
+
     feature_names, coefficients = _reduce(
-        model.get_feature_names(), model.coefficients()
+        base_feature_names, model.get_feature_names(), model.coefficients()
     )
 
     equations = model.equations()
 
-    return equations, base_feature_names, feature_names, jnp.array(coefficients)
+    return equations, base_feature_names, feature_names, cnp.array(coefficients)
+
+
+def train_from_csv(
+    file_name,
+    header_as_first_row=False,
+    state_columns=1,
+    control_input_columns=None,
+    dt=None,
+    time_column=None,
+    state_derivatives_columns=None,
+    discrete_time=False,
+    differentiation_method="centered difference",
+    # optimizer parameters
+    threshold=0.1,
+    alpha=0.05,
+    max_iter=20,
+    normalize_columns=False,
+    # Library parameters
+    poly_order=2,
+    fourier_n_frequencies=None,
+):
+    df = read_csv(file_name, header_as_first_row=header_as_first_row)
+
+    if time_column is not None:
+        time_column_name = (
+            time_column if isinstance(time_column, str) else df.columns[time_column]
+        )
+        df = df.drop_duplicates(subset=[time_column_name], keep="first")
+        time = extract_columns(df, time_column)
+    elif dt:
+        time = dt
+    else:
+        time = None
+
+    has_control_input = control_input_columns is not None
+
+    u_train = extract_columns(df, control_input_columns) if has_control_input else None
+
+    x_dot_train = (
+        extract_columns(df, state_derivatives_columns)
+        if state_derivatives_columns
+        else None
+    )
+
+    x_train = extract_columns(df, state_columns)
+
+    (
+        equations,
+        base_feature_names,
+        feature_names,
+        coefficients,
+    ) = train(
+        x_train,
+        u_train,
+        x_dot_train,
+        time,
+        discrete_time=discrete_time,
+        differentiation_method=differentiation_method,
+        poly_order=poly_order,
+        fourier_n_frequencies=fourier_n_frequencies,
+        threshold=threshold,
+        alpha=alpha,
+        max_iter=max_iter,
+        normalize_columns=normalize_columns,
+    )
+
+    return equations, base_feature_names, feature_names, coefficients, has_control_input
+
+
+def _validate_leafsystem_inputs(
+    pretrained, pretrained_file_path, dt, time_column, poly_order, fourier_n_frequencies
+):
+    if (pretrained is True) and (pretrained_file_path is None):
+        raise ValueError(
+            "Please provide `pretrained_file_path` as boolean "
+            "`pretrained` is set to True"
+        )
+
+    if (pretrained is False) and (pretrained_file_path is not None):
+        raise ValueError(
+            "Boolean `pretrained` is False but `pretrained_file_path` " "is provided."
+        )
+
+    if pretrained is False:
+        if (dt is None) and (time_column is None):
+            warnings.warn(
+                "Neither fixed dt nor column for time data are provided. "
+                "Default dt=1.0 will be used for SINDy training"
+            )
+
+    if (poly_order is None) and (fourier_n_frequencies is None):
+        raise ValueError(
+            "Please use atleast one of the Polynomial or Fourier libraries "
+            "by setting `poly_order` and/or `fourier_n_frequencies` "
+        )
+
 
+def _validate_ui_pretrained_data(coefficients, feature_names, base_feature_names, name):
+    ui_pretrained_data = [coefficients, feature_names, base_feature_names]
+    all_ui_pretrained_data_is_none = all(v is None for v in ui_pretrained_data)
+    all_ui_pretrained_data_is_not_none = all(v is not None for v in ui_pretrained_data)
 
-class ContinuousTimeSindyWithControl(LeafSystem):
+    if not (all_ui_pretrained_data_is_none or all_ui_pretrained_data_is_not_none):
+        raise ValueError(
+            f"Only some pretrained data from UI was provided for SINDY block: {name}. "
+            f"{ui_pretrained_data}"
+        )
+    return all_ui_pretrained_data_is_not_none
+
+
+class Sindy(LeafSystem):
     """
-    Sindy with control (SINDyc) block: Continuous-time.
+    This class implements System Identification (SINDy) algorithm with or without
+    control inputs for contiuous-time and discrete-time systems.
 
-    This class implements System Identification (SINDy) algorithm with control inputs.
+    The learned continuous-time dynamical system model will be of the form:
 
-    Attributes:
-        equations (list of strings): The identified system equations.
-        base_feature_names (list of strings): features x_i and u_i.
-        feature_names (list of strings): Composed features with basis libraries.
-        coefficients (ndarray): Coefficients of the identified model.
-        nx (int): Number of states in the model.
+    ```
+    dx/dt = f(x, u)
+    ```
+    where `x` is the state vector and `u` is the optional control input vector. The
+    block will output the full state vector `x` of the system.
+
+    The learned discrete-time dynamical system model will be of the form:
+
+    ```
+    x_{k+1} = f(x_k, u_k)
+    ```
+
+    where `x_k` is the state vector at time step `k` and `u_k` is the optional control
+    vector. The block will update the output to `x_k` at an interval provided by the
+    parameter `discrete_time_update_interval`.
+
+    Input ports:
+        (0) u: control vector for the system. This port is only available if the Sindy
+            model is trained with control inputs, i.e. `control_input_columns` is not
+            `None` during training.
+
+    Output ports:
+        (0) x: full state output of the system.
+
+    Parameters:
+        file_name (str):
+            Path to the CSV file containing training data.
+
+        header_as_first_row (bool):
+            If True, the first row of the CSV file is treated as the header.
+
+        state_columns (int | str | list[int] | list[str]):
+            For training, either one of the following for CSV columns representing
+            state variables `x`:
+                - a string or integer (for a single column)
+                - a list of strings or integers (for multiple columns)
+                - a string representing a slice of columns, e.g. '0:3'
+
+
+        control_input_columns (int | str | list[int] | list[str]):
+            For training, either one of the following for CSV columns representing
+            control inputs `u`:
+                - a string or integer (for a single column)
+                - a list of strings or integers (for multiple columns)
+                - a string representing a slice of columns, e.g. '0:3'
+            If None, then the SINDy model will be trained without control inputs.
+
+        dt (float):
+            Fixed value of dt if rows of the CSV file represent equidistant time steps.
+
+        time_column (str, int):
+            Column name (str) for column index (int) for time data `t`.
+            If `time_column` is provided, then fixed `dt` above will be ignored.
+            If neither `dt` nor `time_column` is provided, then the SINDy model will
+            use a fixed detault time step of `dt=1`.
+
+        state_derivatives_columns (int | str | list[int] | list[str]):
+            For training, either one of the following for csv columns representing
+            state derivatives `x_dot`:
+                - a string or integer (for a single column)
+                - a list of strings or integers (for multiple columns)
+                - a string representing a slice of columns, e.g. '0:3'
+            This field is optional. If provided, the SINDy model will estimate directly
+            use these state derivatives for training. If not provided, the SINDy model
+            will approximate the state derivatives `dot_x = dx/dt` from `x` by using
+            the specified `differentiation_method`.
+
+        discrete_time (bool):
+            If True, the SINDy model will be trained for discrete-time systems. In
+            this case, the dynamical system is treated as a map. Rather than
+            predicting derivatives, the right hand side functions step the system
+            forward by one time step. If False, dynamical system is assumed to be a
+            flow (right-hand side functions predict continuous time derivatives).
+            See documentation for `pysindy`.
+
+        differentiation_method (str):
+            Method to use for differentiating the state data `x` to obtain state
+            derivatives `dot_x = dx/dt`. Available options are:
+                'centered difference' (default)
+
+        threshold (float):
+            Threshold for the Sequentially thresholded least squares (STLSQ) algorithm
+            used for training SINDy model.
+
+        alpha (float):
+            Regularization strength for the STLSQ algorithm.
+
+        max_iter (int):
+            Maximum number of iterations for the STLSQ algorithm.
+
+        normalize_columns (bool):
+            If True, normalize the columns of the data matrix before regression.
+
+        poly_order (int):
+            Degree of polynomial features. Set to `None` to omit this library.
+
+        fourier_n_frequencies (int):
+            Number of Fourier frequencies. Set to `None` to omit this library.
+
+        pretrained (bool):
+            If True, use a pretrained model specified by the `pretrained_file_path`
+            argument.
+
+        pretrained_file_path (str, optional): Path to the pretrained model file.
+
+        initial_state (ndarray):
+                Initial state of the system for propagating the continuous-time
+                or discrete-time system forward duiring simulation.
+
+        discrete_time_update_interval (float):
+            Interval at which the discrete-time model should be updated. Default
+            is 1.0.
+
+        equations (list of strings):
+            (For internal UI use only) The identified system equations.
+
+        base_feature_names (list of strings):
+            (For internal UI use only) Features x_i and u_i.
+
+        feature_names (list of strings):
+            (For internal UI use only) Composed features with basis libraries.
+
+        coefficients (ndarray):
+            (For internal UI use only) Coefficients of the identified model.
+
+        has_control_input (bool):
+            (For internal UI use only) If True, the model was trained with control.
+            For standard training from CSV file, this is inferred from the
+            parameter `control_input_columns`.
     """
 
+    @parameters(
+        static=[
+            "file_name",
+            "header_as_first_row",
+            "state_columns",
+            "control_input_columns",
+            "discrete_time",
+            "dt",
+            "time_column",
+            "state_derivatives_columns",
+            "differentiation_method",
+            "threshold",
+            "alpha",
+            "max_iter",
+            "normalize_columns",
+            "poly_order",
+            "fourier_n_frequencies",
+            "pretrained",
+            "equations",
+            "discrete_time_update_interval",
+            "pretrained_file_path",
+        ]
+    )
     def __init__(
         self,
-        file_name,
-        state_columns,
-        control_input_columns,
-        *args,
+        file_name=None,
+        header_as_first_row=False,
+        state_columns=1,
+        control_input_columns=None,
         dt=None,
         time_column=None,
         state_derivatives_columns=None,
+        discrete_time=False,
+        differentiation_method="centered difference",
+        # optimizer parameters
         threshold=0.1,
+        alpha=0.05,
+        max_iter=20,
+        normalize_columns=False,
+        # Library parameters
         poly_order=2,
         fourier_n_frequencies=None,
         pretrained=False,
         pretrained_file_path=None,
-        coefficients=None,
-        feature_names=None,
-        base_feature_names=None,
+        # for parameters obtained from UI training
         equations=None,
+        base_feature_names=None,
+        feature_names=None,
+        coefficients=None,
+        has_control_input=True,
+        # Simulation parameters
         initial_state=None,
+        discrete_time_update_interval=1.0,
         **kwargs,
     ):
-        """Initializes the LeafSystem.
-
-        Args:
-            file_name (str): Path to the CSV file containing the training data.
-
-            state_columns: Column names (str or list[str])
-                          or column indices (int or list[int]) for x_train.
-
-            control_input_columns: Column names (str or list[str])
-                          or column indices (int or list[int]) for u_train.
-
-            dt: fixed dt (float)
+        super().__init__(**kwargs)
 
-            time_column : Column name (str) for column index (int) for time data.
-                       If time_column is provided, then fixed `dt` above will be ignored.
-
-            state_derivatives_columns (optional): Column names (str or list[str]) or column
-                                         indices (int or list[int]) for x_dot_train.
-
-            poly_order (int): Degree of polynomial features. Set to `None` to
-                                     omit this library.
-
-            fourier_n_frequencies (int): Number of Fourier frequencies. Set to `None`
-                                         to omit this library.
-
-            pretrained (bool): If True, use a pretrained model specified by the
-                               `pretrained_file_path` argument.
-
-            pretrained_file_path (str, optional): Path to the pretrained model file.
-
-            initial_state: Initial state of the system for propagating the ODE forward
-                           during inference.
-        """
-        super().__init__(*args, **kwargs)
-
-        if (pretrained is True) and (pretrained_file_path is None):
-            raise ValueError(
-                "Please provide `pretrained_file_path` as boolean "
-                "`pretrained` is set to True"
-            )
-
-        if (pretrained is False) and (pretrained_file_path is not None):
-            raise ValueError(
-                "Boolean `pretrained` is False but `pretrained_file_path` "
-                "is provided."
-            )
-
-        if pretrained is False:
-            if (dt is None) and (time_column is None):
-                raise ValueError(
-                    "Neither fixed dt nor column for time data are provided."
-                )
-
-        if (poly_order is None) and (fourier_n_frequencies is None):
-            raise ValueError(
-                "Please use atleast one of the Polynomial or Fourier libraries "
-                "by setting `poly_order` and/or `fourier_n_frequencies` "
-            )
-
-        # validate training data from UI
-        ui_pretrained_data = [coefficients, feature_names, base_feature_names]
-        all_ui_pretrained_data_is_none = all(v is None for v in ui_pretrained_data)
-        all_ui_pretrained_data_is_not_none = all(
-            v is not None for v in ui_pretrained_data
+        _validate_leafsystem_inputs(
+            pretrained,
+            pretrained_file_path,
+            dt,
+            time_column,
+            poly_order,
+            fourier_n_frequencies,
         )
 
-        if not (all_ui_pretrained_data_is_none or all_ui_pretrained_data_is_not_none):
-            raise ValueError(
-                f"Only some pretrained data from UI was provided for SINDY block: {self.name}. "
-                f"{ui_pretrained_data}"
-            )
+        ui_is_providing_pretrained_data = _validate_ui_pretrained_data(
+            coefficients, feature_names, base_feature_names, self.name
+        )
 
-        if all_ui_pretrained_data_is_not_none:
+        if ui_is_providing_pretrained_data:
+            self.equations = equations
             self.base_feature_names = base_feature_names.tolist()
             self.feature_names = feature_names.tolist()
-            self.coefficients = jnp.array(coefficients)
+            self.coefficients = cnp.array(coefficients)
+            self.has_control_input = has_control_input
 
         elif pretrained:
             with open(pretrained_file_path, "r") as f:
                 deserialized_model = json.load(f)
 
             self.equations = deserialized_model["equations"]
             self.base_feature_names = deserialized_model["base_feature_names"]
             self.feature_names = deserialized_model["feature_names"]
-            self.coefficients = jnp.array(deserialized_model["coefficients"])
-        else:
-            df = _read_csv(file_name)
-
-            if time_column:
-                time_column_name = (
-                    df.columns[time_column]
-                    if isinstance(time_column, int)
-                    else time_column
-                )
-                df = df.drop_duplicates(subset=time_column_name, keep="first")
-                time = np.array(_extract_columns(df, time_column_name)[:, 0])
-            else:
-                time = dt
-
-            x_train = _extract_columns(df, state_columns)
-            u_train = _extract_columns(df, control_input_columns)
-            x_dot_train = (
-                _extract_columns(df, state_derivatives_columns)
-                if state_derivatives_columns
-                else None
-            )
+            self.coefficients = cnp.array(deserialized_model["coefficients"])
+            self.has_control_input = deserialized_model["has_control_input"]
 
+        else:
             (
                 self.equations,
                 self.base_feature_names,
                 self.feature_names,
                 self.coefficients,
-            ) = train(
-                x_train,
-                u_train,
-                x_dot_train,
-                time,
+                self.has_control_input,
+            ) = train_from_csv(
+                file_name,
+                header_as_first_row=header_as_first_row,
+                state_columns=state_columns,
+                control_input_columns=control_input_columns,
+                dt=dt,
+                time_column=time_column,
+                state_derivatives_columns=state_derivatives_columns,
+                discrete_time=discrete_time,
+                differentiation_method=differentiation_method,
+                threshold=threshold,
+                alpha=alpha,
+                max_iter=max_iter,
+                normalize_columns=normalize_columns,
                 poly_order=poly_order,
                 fourier_n_frequencies=fourier_n_frequencies,
-                threshold=threshold,
             )
 
-        _, self.nx = self.coefficients.shape
-        self.declare_input_port()  # one vector valued input port for u
+        self.nx, _ = self.coefficients.shape
 
-        if initial_state is None:
-            initial_state = jnp.zeros(self.nx)
+        if cnp.all(self.coefficients == 0):
+            warnings.warn(
+                "No features were selected for the SINDy model. "
+                "Please check the training data and the feature selection "
+                "parameters."
+            )
 
-        self.declare_continuous_state(
-            shape=(self.nx,), ode=self.ode, default_value=jnp.array(initial_state)
-        )
-        self.declare_continuous_state_output()  # output of the state in ODE
+        if initial_state is not None:
+            if len(initial_state) != self.nx:
+                raise ValueError(
+                    f"Provided initial state has {len(initial_state)} elements. "
+                    f"Expected {self.nx} elements."
+                )
+        else:
+            initial_state = cnp.zeros(self.nx)
 
-        # SymPy parsing to compute $\dot{x} = f(x,u)$
+        if self.has_control_input:
+            self.declare_input_port()  # one vector valued input port for u
+
+        if discrete_time:
+            self.declare_discrete_state(
+                shape=(self.nx,),
+                default_value=initial_state,
+                as_array=True,
+            )
+            self.declare_periodic_update(
+                (
+                    self._discrete_update
+                    if self.has_control_input
+                    else lambda time, state, **params: self._discrete_update(
+                        time, state, (), **params
+                    )
+                ),
+                period=discrete_time_update_interval,
+                offset=0.0,
+            )
+            self.declare_output_port(
+                self._full_discrete_state_output,
+                period=discrete_time_update_interval,
+                offset=0.0,
+                default_value=initial_state,
+                requires_inputs=False,
+            )
+
+        else:
+            self.declare_continuous_state(
+                ode=(
+                    self._ode
+                    if self.has_control_input
+                    else lambda time, state, **params: self._ode(
+                        time, state, (), **params
+                    )
+                ),
+                shape=(self.nx,),
+                default_value=cnp.array(initial_state),
+            )
+            self.declare_continuous_state_output()  # output of the state in ODE
+
+        # SymPy parsing to compute $f(x,u)$
+        # For continuous-time systems $\dot{x} = f(x,u)$
+        # For discrete-time systems $x_{k+1} = f(x_k, u_k)$
         sympy_base_features = sp.symbols(self.base_feature_names)
 
         # Convert feature names to sympy expressions
         sympy_feature_expressions = []
         for name in self.feature_names:
             # Replace spaces with multiplication
             name = name.replace(" ", "*")
@@ -303,61 +564,81 @@
             sympy_feature_expressions.append(expr)
 
         x_and_u_vec = sp.Matrix(sympy_base_features)
         self.features_func = sp.lambdify(
             (x_and_u_vec,), sympy_feature_expressions, modules="jax"
         )  # feature functions
 
-        self.declare_continuous_state(
-            shape=(self.nx,),
-            ode=self.ode,
-            default_value=jnp.array(initial_state),
-        )
-
-        self.declare_configuration_parameters(
-            file_name=file_name,
-            state_columns=state_columns,
-            control_input_columns=control_input_columns,
-            dt=dt,
-            time_column=time_column,
-            state_derivatives_columns=state_derivatives_columns,
-            threshold=threshold,
-            poly_order=poly_order,
-            fourier_n_frequencies=fourier_n_frequencies,
-            pretrained=pretrained,
-            coefficients=self.coefficients.tolist(),
-            feature_names=self.feature_names,
+        self.declare_static_parameters(
             base_feature_names=self.base_feature_names,
-            equations=equations,
+            feature_names=self.feature_names,
+            coefficients=self.coefficients.tolist(),
+            has_control_input=self.has_control_input,
             initial_state=initial_state,
         )
 
-        if pretrained_file_path:
-            self.declare_configuration_parameters(
-                pretrained_file_path=pretrained_file_path
-            )
+    def initialize(self, **kwargs):
+        logger.warning("SINDy block does not support re-initialization yet.")
 
-    def ode(self, time, state, inputs, **params):
+    def _ode(self, _time, state, inputs, **_params):
         """
-        The ODE system RHS. The RHS is given by
-        coefficients @ features
+        The ODE system RHS. The RHS is given by `coefficients @ features`
         """
         x = state.continuous_state
         u = inputs
-        x_and_u = jnp.hstack([x, u])
+        x_and_u = cnp.hstack([x, u])
         features_evaluated = self.features_func(x_and_u)
-        x_dot = jnp.matmul(self.coefficients, jnp.atleast_1d(features_evaluated))
+        x_dot = cnp.matmul(self.coefficients, cnp.atleast_1d(features_evaluated))
         return x_dot
 
+    def _discrete_update(self, _time, state, inputs, **_params):
+        """
+        Update map is given by `coefficients @ features`
+        """
+        x = state.discrete_state
+        u = inputs
+        x_and_u = cnp.hstack([x, u])
+        features_evaluated = self.features_func(x_and_u)
+        x_plus = cnp.matmul(self.coefficients, cnp.atleast_1d(features_evaluated))
+        return x_plus
+
+    def _full_discrete_state_output(self, _time, state, *_inputs, **_params):
+        return state.discrete_state
+
     def serialize(self, filename):
         """
         Save the relevant class attributes post training
         so that model state can be restored
         """
-        sindy_model = {
+        sindy_data = {
             "equations": self.equations,
             "base_feature_names": self.base_feature_names,
             "feature_names": self.feature_names,
             "coefficients": self.coefficients.tolist(),  # Can't serialize numpy arrays
+            "has_control_input": self.has_control_input,
         }
         with open(filename, "w") as f:
-            json.dump(sindy_model, f)
+            json.dump(sindy_data, f)
+
+    @staticmethod
+    def serialize_trained_pysindy_model(model, filename):
+        """
+        Serialize a PySindy model trained outside of Collimator.
+        The saved file can be used as a pretrained model in Collimator.
+        """
+
+        feature_names, coefficients = _reduce(
+            model.feature_names, model.get_feature_names(), model.coefficients()
+        )
+
+        has_control_input = model.model.n_input_features_ > 0
+
+        sindy_data = {
+            "equations": model.equations,
+            "base_feature_names": model.feature_names,
+            "feature_names": feature_names,
+            "coefficients": coefficients.tolist(),  # Can't serialize numpy arrays
+            "has_control_input": has_control_input,
+        }
+
+        with open(filename, "w") as f:
+            json.dump(sindy_data, f)
```

## collimator/library/nmpc/trajectory_optimization.py

```diff
@@ -75,19 +75,18 @@
         # Only the final point is constrained in this case
         if xf is not None:
             x_ref[-1, :] = xf
     if u_ref is None:
         u_ref = np.zeros((N + 1, nu))
 
     if x_guess is None:
-        x_guess = np.zeros((N + 1, nx))
         if xf is not None:
-            # Linearly interpolate between x0 and xf
-            for i in range(N + 1):
-                x_guess[i, :] = x0 + (i / N) * (xf - x0)
+            x_guess = x0 + (np.arange(N + 1) / N)[:, None] * (xf - x0)
+        else:
+            x_guess = np.zeros((N + 1, nx))
     if u_guess is None:
         u_guess = np.zeros((N + 1, nu))
 
     optvars_sol = mpc.solve_trajectory_optimzation(
         t0, x0, x_ref, u_ref, x_guess, u_guess
     )
```

## collimator/library/nmpc/base/__init__.py

```diff
@@ -6,15 +6,15 @@
 # Software Foundation, version 3. This program is distributed in the hope that it
 # will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Affero General
 # Public License for more details.  You should have received a copy of the GNU
 # Affero General Public License along with this program. If not, see
 # <https://www.gnu.org/licenses/>.
 
-""" Base classes for nonlinear MPCs with Ipopt """
+"""Base classes for nonlinear MPCs with Ipopt"""
 
 from .nmpc_ipopt_base import NonlinearMPCIpopt
 from .nlp_ipopt_base import NMPCProblemStructure
 
 
 __all__ = [
     "NonlinearMPCIpopt",
```

## collimator/library/nmpc/base/nlp_ipopt_base.py

```diff
@@ -6,15 +6,15 @@
 # Software Foundation, version 3. This program is distributed in the hope that it
 # will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Affero General
 # Public License for more details.  You should have received a copy of the GNU
 # Affero General Public License along with this program. If not, see
 # <https://www.gnu.org/licenses/>.
 
-""" Base classes for Ipopt NLP structures """
+"""Base classes for Ipopt NLP structures"""
 
 from abc import ABC, abstractmethod
 from functools import partial
 
 from typing import Tuple
 
 import jax
```

## collimator/library/nmpc/base/nmpc_base.py

```diff
@@ -6,15 +6,15 @@
 # Software Foundation, version 3. This program is distributed in the hope that it
 # will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Affero General
 # Public License for more details.  You should have received a copy of the GNU
 # Affero General Public License along with this program. If not, see
 # <https://www.gnu.org/licenses/>.
 
-""" Base class for nonlinear MPCs """
+"""Base class for nonlinear MPCs"""
 
 from abc import ABC, abstractmethod
 
 import jax.numpy as jnp
 
 from ....framework import LeafSystem
```

## collimator/library/nmpc/base/nmpc_ipopt_base.py

```diff
@@ -6,15 +6,15 @@
 # Software Foundation, version 3. This program is distributed in the hope that it
 # will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Affero General
 # Public License for more details.  You should have received a copy of the GNU
 # Affero General Public License along with this program. If not, see
 # <https://www.gnu.org/licenses/>.
 
-""" Base class for nonlinear MPCs utilizing Ipopt """
+"""Base class for nonlinear MPCs utilizing Ipopt"""
 
 from abc import abstractmethod
 from typing import Tuple
 from functools import partial
 
 import jax
 import jax.numpy as jnp
```

## collimator/library/state_estimators/continuous_time_infinite_horizon_kalman_filter.py

```diff
@@ -6,15 +6,15 @@
 # Software Foundation, version 3. This program is distributed in the hope that it
 # will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Affero General
 # Public License for more details.  You should have received a copy of the GNU
 # Affero General Public License along with this program. If not, see
 # <https://www.gnu.org/licenses/>.
 
-""" Implements Continuous-time Infinite Horizon Kalman Filter LeafSystem """
+"""Implements Continuous-time Infinite Horizon Kalman Filter LeafSystem"""
 
 from ...backend import numpy_api as cnp
 
 from .utils import linearize_plant
 
 from ...framework import LeafSystem
```

## collimator/library/state_estimators/extended_kalman_filter.py

```diff
@@ -6,15 +6,15 @@
 # Software Foundation, version 3. This program is distributed in the hope that it
 # will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Affero General
 # Public License for more details.  You should have received a copy of the GNU
 # Affero General Public License along with this program. If not, see
 # <https://www.gnu.org/licenses/>.
 
-""" Implements Extended Kalman Filter LeafSystem """
+"""Implements Extended Kalman Filter LeafSystem"""
 
 import jax
 import jax.numpy as jnp
 
 from .utils import prepare_continuous_plant_for_nonlinear_kalman_filter
 
 from .kalman_filter_base import KalmanFilterBase
```

## collimator/library/state_estimators/infinite_horizon_kalman_filter.py

```diff
@@ -6,30 +6,39 @@
 # Software Foundation, version 3. This program is distributed in the hope that it
 # will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Affero General
 # Public License for more details.  You should have received a copy of the GNU
 # Affero General Public License along with this program. If not, see
 # <https://www.gnu.org/licenses/>.
 
-""" Implements Discrete-time Infinite Horizon Kalman Filter LeafSystem """
+"""Implements Discrete-time Infinite Horizon Kalman Filter LeafSystem"""
 
 import numpy as np
+
+from collimator.framework.system_base import parameters
+
 from ...backend import numpy_api as cnp
 
-from .utils import linearize_and_discretize_continuous_plant
+from .utils import (
+    check_shape_compatibilities,
+    linearize_and_discretize_continuous_plant,
+)
 
 from .kalman_filter_base import KalmanFilterBase
 
 from ...lazy_loader import LazyLoader
 
 control = LazyLoader(
     "control", globals(), "control"
 )  # For formatting state-space systems
 
 
+# noqa: C0103
+
+
 class InfiniteHorizonKalmanFilter(KalmanFilterBase):
     """
     Infinite Horizon Kalman Filter for the following system:
 
     ```
     x[n+1] = A x[n] + B u[n] + G w[n]
     y[n]   = C x[n] + D u[n] + v[n]
@@ -51,59 +60,107 @@
         dt: float
             Time step of the discrete-time system
         A: ndarray
             State transition matrix
         B: ndarray
             Input matrix
         C: ndarray
-            Output matrix
+            Output matrix. If `None`, full state output is assumed.
         D: ndarray
-            Feedthrough matrix
+            Feedthrough matrix. If `None`, no feedthrough is assumed.
         G: ndarray
-            Process noise matrix
+            Process noise matrix. If `None`, `G=B` is assumed.
         Q: ndarray
-            Process noise covariance matrix
+            Process noise covariance matrix. If `None`, Identity matrix of size
+            compatible with `G` and `A` is assumed.
         R: ndarray
-            Measurement noise covariance matrix
+            Measurement noise covariance matrix. If `None`, Identity matrix of size
+            compatible with `C` and `A` is assumed.
         x_hat_0: ndarray
-            Initial state estimate
+            Initial state estimate. If `None`, an array of zeros is assumed.
     """
 
+    @parameters(
+        static=["dt", "A", "B", "C", "D", "G", "Q", "R", "x_hat_0"],
+    )
     def __init__(
         self,
         dt,
         A,
         B,
-        C,
-        D,
-        G,
-        Q,
-        R,
-        x_hat_0,
+        C=None,
+        D=None,
+        G=None,
+        Q=None,
+        R=None,
+        x_hat_0=None,
         name=None,
+        **kwargs,
     ):
+        self.nx = 0
+        self.nu = 0
+        self.ny = 0
+        self.nd = 0
+        self.A = None
+        self.B = None
+        self.C = None
+        self.D = None
+        self.G = None
+        self.Q = None
+        self.R = None
+        self.K = None
+        self.A_minus_LC = None
+        self.B_minus_LD = None
+        self.L = None
+
         # Note: This class inherits from KalmanFilterBase. Since the infinite horizon
         # kalman filter does not need P_hat and track it, a dummy_P_hat_0 is set as
         # Identity matrix of size 1, and used wherever KalmanFilterBase demands
         # P_hat-like matrices
-
         self.dummy_P_hat_0 = cnp.eye(1)
-        super().__init__(dt, x_hat_0, self.dummy_P_hat_0, name)
+        super().__init__(dt, x_hat_0, self.dummy_P_hat_0, name, **kwargs)
+
+    def initialize(
+        self, dt, A, B, C=None, D=None, G=None, Q=None, R=None, x_hat_0=None
+    ):
+        self.nx, self.nu = B.shape
+
+        if C is None:
+            C = cnp.eye(self.nx)
+            self.ny = self.nx
+        else:
+            self.ny = C.shape[0]
+
+        if D is None:
+            D = cnp.zeros((self.ny, self.nu))
+
+        if G is None:
+            G = B
+
+        _, self.nd = G.shape
+
+        if Q is None:
+            Q = cnp.eye(self.nd)
+
+        if R is None:
+            R = cnp.eye(self.ny)
+
+        if x_hat_0 is None:
+            x_hat_0 = cnp.zeros(self.nx)
+
+        check_shape_compatibilities(A, B, C, D, G, Q, R)
 
         self.A = A
         self.B = B
         self.C = C
         self.D = D
         self.G = G
         self.Q = Q
         self.R = R
 
-        self.nx, self.nu = B.shape
-        self.ny = C.shape[0]
-
         L, P, E = control.dlqe(A, G, C, Q, R)
 
         self.K = np.linalg.solve(A, L)
 
         self.A_minus_LC = A - np.matmul(L, C)
         self.B_minus_LD = B - np.matmul(L, D)
         self.L = L
@@ -139,16 +196,16 @@
 
     @staticmethod
     def for_continuous_plant(
         plant,
         x_eq,
         u_eq,
         dt,
-        Q,
-        R,
+        Q=None,
+        R=None,
         G=None,
         x_hat_bar_0=None,
         discretization_method="zoh",
         discretized_noise=False,
         name=None,
     ):
         """
@@ -243,17 +300,19 @@
             x_eq: ndarray
                 Equilibrium state vector for discretization
             u_eq: ndarray
                 Equilibrium control vector for discretization
             dt: float
                 Time step for the discretization.
             Q: ndarray
-                Process noise covariance matrix.
+                Process noise covariance matrix. If `None`, Identity matrix of size
+                compatible with `G` and and linearized system's `A` is assumed.
             R: ndarray
-                Measurement noise covariance matrix.
+                Measurement noise covariance matrix. If `None`, Identity matrix of size
+                compatible with linearized system's `C` and `A` is assumed.
             G: ndarray
                 Process noise matrix. If `None`, `G=B` is assumed making disrurbances
                 additive to control vector `u`, i.e. `u_disturbed = u_orig + w`.
             x_hat_bar_0: ndarray
                 Initial state estimate relative to equilibrium.
                 If None, an identity matrix is assumed.
             discretization_method: str ("euler" or "zoh")
@@ -272,14 +331,16 @@
             Gd,
             Qd,
             Rd,
         ) = linearize_and_discretize_continuous_plant(
             plant, x_eq, u_eq, dt, Q, R, G, discretization_method, discretized_noise
         )
 
+        check_shape_compatibilities(Ad, Bd, Cd, Dd, Gd, Qd, Rd)
+
         nx = x_eq.size
 
         if x_hat_bar_0 is None:
             x_hat_bar_0 = cnp.zeros(nx)
 
         # Instantiate an Infinite Horizon Kalman Filter for the linearized plant
         kf = InfiniteHorizonKalmanFilter(
```

## collimator/library/state_estimators/kalman_filter.py

```diff
@@ -6,19 +6,23 @@
 # Software Foundation, version 3. This program is distributed in the hope that it
 # will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Affero General
 # Public License for more details.  You should have received a copy of the GNU
 # Affero General Public License along with this program. If not, see
 # <https://www.gnu.org/licenses/>.
 
-""" Implements time-varying Kalman Filter LeafSystem """
+"""Implements time-varying Kalman Filter LeafSystem"""
 
 import jax.numpy as jnp
 
-from .utils import linearize_and_discretize_continuous_plant
+from ...framework import parameters
+from .utils import (
+    check_shape_compatibilities,
+    linearize_and_discretize_continuous_plant,
+)
 
 from .kalman_filter_base import KalmanFilterBase
 
 
 class KalmanFilter(KalmanFilterBase):
     """
     Kalman Filter for the following system:
@@ -44,56 +48,117 @@
         dt: float
             Time step of the discrete-time system
         A: ndarray
             State transition matrix
         B: ndarray
             Input matrix
         C: ndarray
-            Output matrix
+            Output matrix. If `None`, full state output is assumed.
         D: ndarray
-            Feedthrough matrix
+            Feedthrough matrix. If `None`, no feedthrough is assumed.
         G: ndarray
-            Process noise matrix
+            Process noise matrix. If `None`, `G=B` is assumed.
         Q: ndarray
-            Process noise covariance matrix
+            Process noise covariance matrix. If `None`, Identity matrix of size
+            compatible with `G` and `A` is assumed.
         R: ndarray
-            Measurement noise covariance matrix
+            Measurement noise covariance matrix. If `None`, Identity matrix of size
+            compatible with `C` and `A` is assumed.
         x_hat_0: ndarray
-            Initial state estimate
+            Initial state estimate. If `None`, an array of zeros is assumed.
         P_hat_0: ndarray
-            Initial state covariance matrix estimate
+            Initial state covariance matrix estimate. If `None`, Identity matrix of size
+            identical to `A` is assumed.
     """
 
+    @parameters(
+        static=["dt", "A", "B", "C", "D", "G", "Q", "R", "x_hat_0", "P_hat_0"],
+    )
     def __init__(
         self,
         dt,
         A,
         B,
-        C,
-        D,
-        G,
-        Q,
-        R,
-        x_hat_0,
-        P_hat_0,
+        C=None,
+        D=None,
+        G=None,
+        Q=None,
+        R=None,
+        x_hat_0=None,
+        P_hat_0=None,
         name=None,
+        **kwargs,
     ):
-        super().__init__(dt, x_hat_0, P_hat_0, name)
+        super().__init__(dt, x_hat_0, P_hat_0, name, **kwargs)
+
+        self.nx = 0
+        self.nu = 0
+        self.ny = 0
+        self.nd = 0
+        self.A = None
+        self.B = None
+        self.C = None
+        self.D = None
+        self.G = None
+        self.Q = None
+        self.R = None
+        self.eye_x = None
+        self.GQGT = None
+
+    def initialize(
+        self,
+        dt,
+        A,
+        B,
+        C=None,
+        D=None,
+        G=None,
+        Q=None,
+        R=None,
+        x_hat_0=None,
+        P_hat_0=None,
+    ):
+        self.nx, self.nu = B.shape
+
+        if C is None:
+            C = jnp.eye(self.nx)
+            self.ny = self.nx
+        else:
+            self.ny = C.shape[0]
+
+        if D is None:
+            D = jnp.zeros((self.ny, self.nu))
+
+        if G is None:
+            G = B
+
+        _, self.nd = G.shape
+
+        if Q is None:
+            Q = jnp.eye(self.nd)
+
+        if R is None:
+            R = jnp.eye(self.ny)
+
+        if x_hat_0 is None:
+            x_hat_0 = jnp.zeros(self.nx)
+
+        if P_hat_0 is None:
+            P_hat_0 = jnp.eye(self.nx)
+
+        check_shape_compatibilities(A, B, C, D, G, Q, R)
 
         self.A = A
         self.B = B
         self.C = C
         self.D = D
         self.G = G
         self.Q = Q
         self.R = R
 
-        self.nx, self.nu = B.shape
-        self.ny = C.shape[0]
-
         self.eye_x = jnp.eye(self.nx)
         self.GQGT = G @ Q @ G.T
 
     def _correct(self, time, x_hat_minus, P_hat_minus, *inputs):
         u, y = inputs
         u = jnp.atleast_1d(u)
         y = jnp.atleast_1d(y)
@@ -132,22 +197,23 @@
 
     @staticmethod
     def for_continuous_plant(
         plant,
         x_eq,
         u_eq,
         dt,
-        Q,
-        R,
+        Q=None,
+        R=None,
         G=None,
         x_hat_bar_0=None,
         P_hat_bar_0=None,
         discretization_method="euler",
         discretized_noise=False,
         name=None,
+        ui_id=None,
     ):
         """
         Obtain a Kalman Filter system for a continuous-time plant after linearization
         at equilibrium point (x_eq, u_eq)
 
         The input plant contains the deterministic forms of the forward and observation
         operators:
@@ -235,17 +301,19 @@
             x_eq: ndarray
                 Equilibrium state vector for discretization
             u_eq: ndarray
                 Equilibrium control vector for discretization
             dt: float
                 Time step for the discretization.
             Q: ndarray
-                Process noise covariance matrix.
+                Process noise covariance matrix. If `None`, Identity matrix of size
+                compatible with `G` and and linearized system's `A` is assumed.
             R: ndarray
-                Measurement noise covariance matrix.
+                Measurement noise covariance matrix. If `None`, Identity matrix of size
+                compatible with linearized system's `C` and `A` is assumed.
             G: ndarray
                 Process noise matrix. If `None`, `G=B` is assumed making disrurbances
                 additive to control vector `u`, i.e. `u_disturbed = u_orig + w`.
             x_hat_bar_0: ndarray
                 Initial state estimate, relative to equilirium.
                 If None, an identity matrix is assumed.
             P_hat_bar_0: ndarray
@@ -267,14 +335,16 @@
             Gd,
             Qd,
             Rd,
         ) = linearize_and_discretize_continuous_plant(
             plant, x_eq, u_eq, dt, Q, R, G, discretization_method, discretized_noise
         )
 
+        check_shape_compatibilities(Ad, Bd, Cd, Dd, Gd, Qd, Rd)
+
         nx = x_eq.size
 
         if x_hat_bar_0 is None:
             x_hat_bar_0 = jnp.zeros(nx)
 
         if P_hat_bar_0 is None:
             P_hat_bar_0 = jnp.eye(nx)
@@ -288,10 +358,11 @@
             Dd,
             Gd,
             Qd,
             Rd,
             x_hat_bar_0,
             P_hat_bar_0,
             name=name,
+            ui_id=ui_id,
         )
 
         return y_eq, kf
```

## collimator/library/state_estimators/kalman_filter_base.py

```diff
@@ -6,15 +6,15 @@
 # Software Foundation, version 3. This program is distributed in the hope that it
 # will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Affero General
 # Public License for more details.  You should have received a copy of the GNU
 # Affero General Public License along with this program. If not, see
 # <https://www.gnu.org/licenses/>.
 
-""" Base class for discrete-time Kalman Filters and its variants """
+"""Base class for discrete-time Kalman Filters and its variants"""
 
 from abc import ABC, abstractmethod
 from typing import NamedTuple
 
 from collimator.backend import numpy_api as cnp
 
 from ...framework import LeafSystem
@@ -98,16 +98,17 @@
 
     def __init__(
         self,
         dt,
         x_hat_0,
         P_hat_0,
         name=None,
+        **kwargs,
     ):
-        super().__init__(name=name)
+        super().__init__(name=name, **kwargs)
 
         self.dt = dt
 
         self.declare_input_port()  # u
         self.declare_input_port()  # y
 
         self.declare_discrete_state(
```

## collimator/library/state_estimators/unscented_kalman_filter.py

```diff
@@ -6,15 +6,15 @@
 # Software Foundation, version 3. This program is distributed in the hope that it
 # will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Affero General
 # Public License for more details.  You should have received a copy of the GNU
 # Affero General Public License along with this program. If not, see
 # <https://www.gnu.org/licenses/>.
 
-""" Implements Unscented Kalman Filter LeafSystem """
+"""Implements Unscented Kalman Filter LeafSystem"""
 
 import jax
 import jax.numpy as jnp
 import jax.scipy as jsp
 
 from .utils import prepare_continuous_plant_for_nonlinear_kalman_filter
```

## collimator/library/state_estimators/utils.py

```diff
@@ -6,26 +6,84 @@
 # Software Foundation, version 3. This program is distributed in the hope that it
 # will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Affero General
 # Public License for more details.  You should have received a copy of the GNU
 # Affero General Public License along with this program. If not, see
 # <https://www.gnu.org/licenses/>.
 
-""" Utilities for state estimators """
+"""Utilities for state estimators"""
 
 import jax
 import jax.numpy as jnp
 import jax.scipy as jsp
 
 from jax.flatten_util import ravel_pytree
 
 from .. import linearize
 from ..utils import make_ode_rhs
 
 
+def check_shape_compatibilities(A, B, C, D, G, Q, R):
+    """
+    Check shape compatibilities of matrices in a linear system.
+
+    ```
+    x[n+1] = A x[n] + B u[n] + G w[n]
+    y[n]   = C x[n] + D u[n] + v[n]
+
+    E(w[n]) = E(v[n]) = 0
+    E(w[n]w'[n]) = Q
+    E(v[n]v'[n] = R
+    E(w[n]v'[n] = N = 0
+    ```
+    """
+
+    # Retrieve the expected shapes from matrices B and C
+    nx, nu = B.shape
+    _, nd = G.shape
+    ny = C.shape[0]
+
+    # Define expected shapes based on system dynamics
+    expected_shapes = {
+        "A": (nx, nx),
+        "C": (ny, nx),
+        "D": (ny, nu),
+        "G": (nx, nd),
+        "Q": (nd, nd),
+        "R": (ny, ny),
+    }
+
+    # Dictionary to hold the actual shapes for comparison
+    actual_shapes = {
+        "A": A.shape,
+        "C": C.shape,
+        "D": D.shape,
+        "G": G.shape,
+        "Q": Q.shape,
+        "R": R.shape,
+    }
+
+    # Iterate through the expected shapes to verify each one
+    for matrix_name, expected_shape in expected_shapes.items():
+        actual_shape = actual_shapes[matrix_name]
+        if actual_shape != expected_shape:
+            error_message = (
+                f"Shape mismatch for matrix '{matrix_name}': "
+                f"expected {expected_shape}, got {actual_shape}."
+                "\nThe above was extracted from the shapes of B and C as follows:"
+                f"\n- B should have shape (nx, nu) = {B.shape}"
+                f"\n- C should have shape (ny, nx) = {C.shape}"
+                f"\n- 'nx' is the number of state variables "
+                f"\n- 'nu' is the number of control inputs."
+                f"\n- 'ny' is the number of measurement outputs."
+                f"\n- and 'nd' is the number of disturbances."
+            )
+            raise ValueError(error_message)
+
+
 def discretize_forward_zoh(A, B, dt):
     """
     Discretize a continuous-time forward model `dot_x = A x + B u` using zero-order
     hold (ZOH) discretization.
 
     Parameters:
     A : jnp.ndarray
@@ -146,16 +204,16 @@
 
 @staticmethod
 def linearize_and_discretize_continuous_plant(
     plant,
     x_eq,
     u_eq,
     dt,
-    Q,
-    R,
+    Q=None,
+    R=None,
     G=None,  # if None, assume u = u+w, so G = B
     discretization_method="zoh",
     discretized_noise=False,
 ):
     """
     Utility to linearize and discretize a continuous plant.
     See documentation for methods calling this for more information; for example,
@@ -168,14 +226,22 @@
 
     nx, nu = B.shape
     ny, _ = D.shape
 
     if G is None:
         G = B
 
+    _, nd = G.shape
+
+    if Q is None:
+        Q = jnp.eye(nd)
+
+    if R is None:
+        R = jnp.eye(ny)
+
     # Convert to discrete-time
     Cd, Dd = C, D
 
     if discretization_method == "euler":
         Ad, Bd = discretize_forward_euler(A, B, dt)
         if discretized_noise:
             Gd = G
```

## collimator/library/utils/__init__.py

```diff
@@ -6,17 +6,20 @@
 # Software Foundation, version 3. This program is distributed in the hope that it
 # will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Affero General
 # Public License for more details.  You should have received a copy of the GNU
 # Affero General Public License along with this program. If not, see
 # <https://www.gnu.org/licenses/>.
 
-""" Variour utilities for nonlinear plants """
+"""Variour utilities for nonlinear plants"""
 
 from .plant_utils import make_ode_rhs
 from .rk4_utils import rk4_major_step_constant_u
+from .csv_utils import read_csv, extract_columns
 
 
 __all__ = [
     "make_ode_rhs",  # used by finite horizon LQR and nmmpc classes
     "rk4_major_step_constant_u",  # used by nmpc classes
+    "read_csv",  # Sindy and DataSource
+    "extract_columns",  # Sindy and DataSource
 ]
```

## collimator/library/utils/plant_utils.py

```diff
@@ -6,15 +6,15 @@
 # Software Foundation, version 3. This program is distributed in the hope that it
 # will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Affero General
 # Public License for more details.  You should have received a copy of the GNU
 # Affero General Public License along with this program. If not, see
 # <https://www.gnu.org/licenses/>.
 
-""" Utilities to generate a function that evaluates ODE RHS for a plant """
+"""Utilities to generate a function that evaluates ODE RHS for a plant"""
 
 import jax
 import jax.numpy as jnp
 
 from jax.flatten_util import ravel_pytree
```

## collimator/library/utils/rk4_utils.py

```diff
@@ -6,15 +6,15 @@
 # Software Foundation, version 3. This program is distributed in the hope that it
 # will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Affero General
 # Public License for more details.  You should have received a copy of the GNU
 # Affero General Public License along with this program. If not, see
 # <https://www.gnu.org/licenses/>.
 
-""" RK4 integration utilities """
+"""RK4 integration utilities"""
 
 # TODO: Integrate with utilities present in the simulator
 
 from functools import partial
 import jax
```

## collimator/models/acrobot.py

```diff
@@ -28,22 +28,22 @@
         I2=-1.0068,
         g=9.81,
         *args,
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
 
-        self.declare_parameter("m1", m1)
-        self.declare_parameter("m2", m2)
-        self.declare_parameter("l1", l1)
-        self.declare_parameter("lc1", lc1)
-        self.declare_parameter("lc2", lc2)
-        self.declare_parameter("I1", I1)
-        self.declare_parameter("I2", I2)
-        self.declare_parameter("g", g)
+        self.declare_dynamic_parameter("m1", m1)
+        self.declare_dynamic_parameter("m2", m2)
+        self.declare_dynamic_parameter("l1", l1)
+        self.declare_dynamic_parameter("lc1", lc1)
+        self.declare_dynamic_parameter("lc2", lc2)
+        self.declare_dynamic_parameter("I1", I1)
+        self.declare_dynamic_parameter("I2", I2)
+        self.declare_dynamic_parameter("g", g)
 
         self.declare_input_port(name="tau")
 
         self.declare_continuous_state(shape=(4,), ode=self.ode, default_value=x0)
 
         self.declare_continuous_state_output()
```

## collimator/models/battery_ecm.py

```diff
@@ -40,20 +40,20 @@
         super().__init__(*args, **kwargs)
 
         self.soc_0 = soc_0
         self.vc1_0 = vc1_0
         self.Q = Q
 
         self.soc_points = soc_points
-        self.declare_parameter(
+        self.declare_dynamic_parameter(
             "v0_points", v0_points
         )  # declare as parameters so that these can be changed in the context
-        self.declare_parameter("Rs_points", Rs_points)
-        self.declare_parameter("R1_points", R1_points)
-        self.declare_parameter("C1_points", C1_points)
+        self.declare_dynamic_parameter("Rs_points", Rs_points)
+        self.declare_dynamic_parameter("R1_points", R1_points)
+        self.declare_dynamic_parameter("C1_points", C1_points)
 
         self.declare_input_port()  # input port for the discharge current
 
         self.declare_continuous_state(
             shape=(2,),  # Two continuous states: soc and vc1
             ode=self.ode,
             default_value=jnp.array([self.soc_0, self.vc1_0]),
```

## collimator/models/bouncing_ball.py

```diff
@@ -19,19 +19,21 @@
     def __init__(
         self, *args, g=9.81, e=1.0, b=0.0, h0=0.0, hdot=0.0, name="ball", **kwargs
     ):
         super().__init__(*args, name=name, **kwargs)
 
         self.declare_continuous_state(2, ode=self.ode)  # Two state variables.
         self.declare_continuous_state_output(name=f"{name}:y")
-        self.declare_parameter("g", g)
-        self.declare_parameter("e", e)  # Resitiution coefficent (0.0 <= e <= 1.0)
-        self.declare_parameter("b", b)  # Quadratic drag coefficient
-        self.declare_parameter("hdot", hdot)  # Speed of floor
-        self.declare_parameter("h0", h0)  # Initial floor height
+        self.declare_dynamic_parameter("g", g)
+        self.declare_dynamic_parameter(
+            "e", e
+        )  # Resitiution coefficent (0.0 <= e <= 1.0)
+        self.declare_dynamic_parameter("b", b)  # Quadratic drag coefficient
+        self.declare_dynamic_parameter("hdot", hdot)  # Speed of floor
+        self.declare_dynamic_parameter("h0", h0)  # Initial floor height
 
         self.declare_zero_crossing(
             guard=self._signed_distance,
             reset_map=self._reset,
             name="time_reset",
             direction="positive_then_non_positive",
         )
```

## collimator/models/cartpole.py

```diff
@@ -24,18 +24,18 @@
         m_p=1.0,
         L=2.0,
         g=9.81,
         full_state_output=False,
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
-        self.declare_parameter("m_c", m_c)
-        self.declare_parameter("m_p", m_p)
-        self.declare_parameter("L", L)
-        self.declare_parameter("g", g)
+        self.declare_dynamic_parameter("m_c", m_c)
+        self.declare_dynamic_parameter("m_p", m_p)
+        self.declare_dynamic_parameter("L", L)
+        self.declare_dynamic_parameter("g", g)
 
         self.declare_input_port(name="fx")
 
         self.declare_continuous_state(shape=(4,), ode=self.ode, default_value=x0)
 
         if full_state_output:
             self.declare_continuous_state_output()
```

## collimator/models/compact_ev.py

```diff
@@ -19,15 +19,15 @@
 
 class DummyBlock(LeafSystem):
     def __init__(
         self,
         name="dummy",
     ):
         super().__init__(name=name)
-        self.declare_parameter("dummy_param", 1.0)
+        self.declare_dynamic_parameter("dummy_param", 1.0)
 
 
 class CompactEV(LeafSystem):
     """
     Leaf equivalent of the UI model.
     """
 
@@ -45,18 +45,18 @@
         self,
         *args,
         dt=0.01,  # 0.01 matches the UI model
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
 
-        self.declare_parameter("mass", 2e3)
+        self.declare_dynamic_parameter("mass", 2e3)
         for i in range(100):
-            self.declare_parameter(f"dummy{str(i)}", float(i))
-        # self.declare_parameter("m2km", 0.001)
+            self.declare_dynamic_parameter(f"dummy{str(i)}", float(i))
+        # self.declare_dynamic_parameter("m2km", 0.001)
 
         # Continuous states:
         self.velocity_state_idx = 0
         self.position_state_idx = 1
         self.accel_loop_breaker_state_idx = 2
         self.driver_pid_iterm_state_idx = 3
         self.coolant_temp_state_idx = 4
```

## collimator/models/compass_gait.py

```diff
@@ -40,21 +40,21 @@
         center_of_mass_leg=0.5,
         gravity=9.81,
         slope=0.0525,
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
 
-        self.declare_parameter("gamma", slope)  # Ramp angle
-        self.declare_parameter("g", gravity)  # Gravity
-        self.declare_parameter("L", length_leg)  # Leg length
-        self.declare_parameter("mh", mass_hip)  # Hip mass
-        self.declare_parameter("m", mass_leg)  # Leg mass
-        self.declare_parameter("a", length_leg - center_of_mass_leg)
-        self.declare_parameter("b", center_of_mass_leg)
+        self.declare_dynamic_parameter("gamma", slope)  # Ramp angle
+        self.declare_dynamic_parameter("g", gravity)  # Gravity
+        self.declare_dynamic_parameter("L", length_leg)  # Leg length
+        self.declare_dynamic_parameter("mh", mass_hip)  # Hip mass
+        self.declare_dynamic_parameter("m", mass_leg)  # Leg mass
+        self.declare_dynamic_parameter("a", length_leg - center_of_mass_leg)
+        self.declare_dynamic_parameter("b", center_of_mass_leg)
 
         # Continuous state: q = [θ_st, θ_sw], dq = [dθ_st, dθ_sw]
         self.declare_continuous_state(shape=(4,), ode=self.ode)
 
         # # Add a torque input (by default set to zero)
         # self.declare_input_port(name="u")
         # self.input_ports[0].fix_value(0.0)
```

## collimator/models/fitzhugh_nagumo.py

```diff
@@ -14,19 +14,19 @@
 from ..framework import LeafSystem
 
 
 # Define the system.
 class FitzHughNagumo(LeafSystem):
     def __init__(self, x0=[0.0, 0.0], I_ext=1.0, R=1.0, a=0.7, b=0.8, tau=12.5):
         super().__init__(self)
-        self.declare_parameter("I_ext", I_ext)
-        self.declare_parameter("R", R)
-        self.declare_parameter("a", a)
-        self.declare_parameter("b", b)
-        self.declare_parameter("tau", tau)
+        self.declare_dynamic_parameter("I_ext", I_ext)
+        self.declare_dynamic_parameter("R", R)
+        self.declare_dynamic_parameter("a", a)
+        self.declare_dynamic_parameter("b", b)
+        self.declare_dynamic_parameter("tau", tau)
         self.declare_continuous_state(default_value=jnp.array(x0), ode=self.ode)
         self.declare_continuous_state_output()
 
     def ode(self, time, state, *inputs, **parameters):
         v, w = state.continuous_state
         I_ext = parameters["I_ext"]
         R = parameters["R"]
```

## collimator/models/hairer.py

```diff
@@ -23,17 +23,17 @@
 class EulerRigidBody(LeafSystem):
     def __init__(
         self, I1=0.5, I2=2.0, I3=3.0, x0=np.array([1.0, 0.0, 0.9]), name="euler"
     ):
         # Euler's equation of rotation for a rigid body
         super().__init__(name=name)
 
-        self.declare_parameter("I1", I1)
-        self.declare_parameter("I2", I2)
-        self.declare_parameter("I3", I3)
+        self.declare_dynamic_parameter("I1", I1)
+        self.declare_dynamic_parameter("I2", I2)
+        self.declare_dynamic_parameter("I3", I3)
 
         self.declare_continuous_state(default_value=x0, ode=self._ode)
         self.declare_continuous_state_output()
 
     def _ode(self, time, state, *inputs, **parameters):
         I1, I2, I3 = parameters["I1"], parameters["I2"], parameters["I3"]
         x = state.continuous_state
@@ -50,15 +50,15 @@
             ]
         )
 
 
 class ArenstorfOrbit(LeafSystem):
     def __init__(self, name="arenstorf"):
         super().__init__(name=name)
-        self.declare_parameter("mu", 0.012277471)
+        self.declare_dynamic_parameter("mu", 0.012277471)
         y0 = np.array([0.994, 0.0, 0.0, -2.00158510637908252240537862224])
 
         self.declare_continuous_state(default_value=y0, ode=self._ode)
         self.declare_continuous_state_output()
 
     def _ode(self, time, state, *inputs, **parameters):
         mu = parameters["mu"]
@@ -74,17 +74,17 @@
             ]
         )
 
 
 class Lorenz(LeafSystem):
     def __init__(self, name="lorenz"):
         super().__init__(name=name)
-        self.declare_parameter("sigma", 10.0)
-        self.declare_parameter("rho", 28.0)
-        self.declare_parameter("beta", 8.0 / 3.0)
+        self.declare_dynamic_parameter("sigma", 10.0)
+        self.declare_dynamic_parameter("rho", 28.0)
+        self.declare_dynamic_parameter("beta", 8.0 / 3.0)
         y0 = np.array([-8.0, 8.0, 27.0])
         self.declare_continuous_state(default_value=y0, ode=self._ode)
         self.declare_continuous_state_output()
 
     def _ode(self, time, state, *inputs, **parameters):
         sigma = parameters["sigma"]
         rho = parameters["rho"]
@@ -98,15 +98,17 @@
             ]
         )
 
 
 class Pleiades(LeafSystem):
     def __init__(self, name="pleiades"):
         super().__init__(name=name)
-        self.declare_parameter("m", np.array([1.0, 2.0, 3.0, 4.0, 5.0, 6.0, 7.0]))
+        self.declare_dynamic_parameter(
+            "m", np.array([1.0, 2.0, 3.0, 4.0, 5.0, 6.0, 7.0])
+        )
         x0 = np.array([3.0, 3.0, -1.0, -3.0, 2.0, -2.0, 2.0])
         y0 = np.array([3.0, -3.0, 2.0, 0.0, 0.0, -4.0, 4.0])
         dx0 = np.zeros(7)
         dx0[5] = 1.75
         dx0[6] = -1.5
         dy0 = np.zeros(7)
         dy0[3] = -1.25
```

## collimator/models/lotka_volterra.py

```diff
@@ -13,18 +13,18 @@
 import jax.numpy as jnp
 from ..framework import LeafSystem
 
 
 class LotkaVolterra(LeafSystem):
     def __init__(self, x0=[10.0, 10.0], alpha=1.1, beta=0.4, gamma=0.4, delta=0.1):
         super().__init__(self)
-        self.declare_parameter("alpha", alpha)
-        self.declare_parameter("beta", beta)
-        self.declare_parameter("gamma", gamma)
-        self.declare_parameter("delta", delta)
+        self.declare_dynamic_parameter("alpha", alpha)
+        self.declare_dynamic_parameter("beta", beta)
+        self.declare_dynamic_parameter("gamma", gamma)
+        self.declare_dynamic_parameter("delta", delta)
         self.declare_continuous_state(default_value=jnp.array(x0), ode=self.ode)
         self.declare_continuous_state_output()
 
     def ode(self, time, state, *inputs, **parameters):
         x, y = state.continuous_state
         alpha = parameters["alpha"]
         beta = parameters["beta"]
```

## collimator/models/pendulum.py

```diff
@@ -53,18 +53,18 @@
         L=1.0,
         b=0.0,
         input_port=False,
         full_state_output=False,
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
-        self.declare_parameter("m", m)
-        self.declare_parameter("g", g)
-        self.declare_parameter("L", L)
-        self.declare_parameter("b", b)
+        self.declare_dynamic_parameter("m", m)
+        self.declare_dynamic_parameter("g", g)
+        self.declare_dynamic_parameter("L", L)
+        self.declare_dynamic_parameter("b", b)
         self.declare_continuous_state(default_value=jnp.array(x0), ode=self.ode)
 
         if input_port:
             self.declare_input_port(name="u")
 
         if full_state_output:
             self.declare_continuous_state_output(name="x")
```

## collimator/models/planar_quadrotor.py

```diff
@@ -15,18 +15,18 @@
 
 from ..framework import LeafSystem
 
 
 class PlanarQuadrotor(LeafSystem):
     def __init__(self, *args, m=1.0, I_B=1.0, r=0.5, g=9.81, **kwargs):
         super().__init__(*args, **kwargs)
-        self.declare_parameter("m", m)
-        self.declare_parameter("I_B", I_B)
-        self.declare_parameter("r", r)
-        self.declare_parameter("g", g)
+        self.declare_dynamic_parameter("m", m)
+        self.declare_dynamic_parameter("I_B", I_B)
+        self.declare_dynamic_parameter("r", r)
+        self.declare_dynamic_parameter("g", g)
 
         self.declare_input_port(name="u")
 
         self.declare_continuous_state(shape=(6,), ode=self.ode)
         self.declare_continuous_state_output()
 
     def ode(self, time, state, *inputs, **parameters):
```

## collimator/models/rimless_wheel.py

```diff
@@ -24,18 +24,20 @@
     """Highly simplified model of 'walking' on a ramp.
 
     https://underactuated.csail.mit.edu/simple_legs.html#section2
     """
 
     def __init__(self, *args, g=9.81, L=1.0, N_spokes=7, gamma=np.pi / 12, **kwargs):
         super().__init__(*args, **kwargs)
-        self.declare_parameter("alpha", np.pi / N_spokes)  # Half-angle between spokes
-        self.declare_parameter("g", g)  # Gravity
-        self.declare_parameter("L", L)  # Leg length
-        self.declare_parameter("gamma", gamma)  # Ramp angle
+        self.declare_dynamic_parameter(
+            "alpha", np.pi / N_spokes
+        )  # Half-angle between spokes
+        self.declare_dynamic_parameter("g", g)  # Gravity
+        self.declare_dynamic_parameter("L", L)  # Leg length
+        self.declare_dynamic_parameter("gamma", gamma)  # Ramp angle
 
         # For plotting/animation
         self.N_spokes = N_spokes
 
         # theta, theta_dot states
         self.declare_continuous_state(shape=(2,), ode=self.ode)
         self.declare_continuous_state_output()
```

## collimator/models/van_der_pol.py

```diff
@@ -11,17 +11,27 @@
 # <https://www.gnu.org/licenses/>.
 
 import jax.numpy as jnp
 from ..framework import LeafSystem
 
 
 class VanDerPol(LeafSystem):
-    def __init__(self, x0=[0.0, 0.0], mu=1.0):
-        super().__init__(self)
-        self.declare_parameter("mu", mu)
+    def __init__(self, x0=[0.0, 0.0], mu=1.0, input_port=False, name="van_der_pol"):
+        super().__init__(name=name)
+        self.declare_dynamic_parameter("mu", mu)
+
+        if input_port:
+            self.declare_input_port(name="u")
+
         self.declare_continuous_state(default_value=jnp.array(x0), ode=self.ode)
         self.declare_continuous_state_output()
 
     def ode(self, time, state, *inputs, **parameters):
         x, y = state.continuous_state
         mu = parameters["mu"]
-        return jnp.array([y, mu * (1 - x**2) * y - x])
+        dy = mu * (1 - x**2) * y - x
+
+        if inputs:
+            (u,) = inputs
+            dy += u
+
+        return jnp.array([y, dy])
```

## collimator/models/quadcopter/quadcopter.py

```diff
@@ -99,22 +99,22 @@
         g=9.81,
         initial_state=jnp.zeros(12),
         *args,
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
 
-        self.declare_parameter("Ixx", Ixx)
-        self.declare_parameter("Iyy", Iyy)
-        self.declare_parameter("Izz", Izz)
-        self.declare_parameter("k", k)
-        self.declare_parameter("b", b)
-        self.declare_parameter("l", l)
-        self.declare_parameter("m", m)
-        self.declare_parameter("g", g)
+        self.declare_dynamic_parameter("Ixx", Ixx)
+        self.declare_dynamic_parameter("Iyy", Iyy)
+        self.declare_dynamic_parameter("Izz", Izz)
+        self.declare_dynamic_parameter("k", k)
+        self.declare_dynamic_parameter("b", b)
+        self.declare_dynamic_parameter("l", l)
+        self.declare_dynamic_parameter("m", m)
+        self.declare_dynamic_parameter("g", g)
 
         self.nx = 12
 
         self.declare_input_port()  # port for the control input
 
         self.declare_continuous_state(
             shape=(self.nx,), ode=self.ode, default_value=jnp.array(initial_state)
```

## collimator/optimization/training.py

```diff
@@ -15,14 +15,16 @@
 Specifically, for training neural networks and other parameters
 via stochastic gradient descent.
 """
 
 import abc
 from functools import partial
 
+import numpy as np
+
 import jax
 from jax import lax
 from jax.flatten_util import ravel_pytree
 import jax.numpy as jnp
 from collimator.simulation import Simulator, estimate_max_major_steps
 import optax
 
@@ -55,35 +57,36 @@
         self,
         simulator: Simulator,
         context,
         optimizer="adamw",
         lr=1e-3,
         print_every=10,
         clip_range=(-10.0, 10.0),
+        **opt_kwargs,
     ):
         self.simulator = simulator
         self.context = context
 
         # See https://optax.readthedocs.io/en/latest/api.html for supported optimizers
-        self.optimizer = getattr(optax, optimizer)(lr)
+        self.optimizer = getattr(optax, optimizer)(lr, **opt_kwargs)
 
         self.print_every = print_every
         self.clip_range = clip_range
 
     @abc.abstractmethod
     def optimizable_parameters(self, context):
         """Extract optimizable model-specific parameters from the context.
 
         These should be in the form of a PyTree (e.g. tuple, dict, array, etc)
         and should be the first arguments to `prepare_context`.
         """
         pass
 
     @abc.abstractmethod
-    def prepare_context(self, context, *data):
+    def prepare_context(self, context, *data, key=None):
         """Model-specific updates to incorporate the sample data and parameters.
 
         `data` should be the combination of the output of `optimizable_parameters`
         along with all the per-simulation "training data".  Parameters will
         update once per epoch, and training data will update once per sample.
         """
         pass
@@ -93,84 +96,102 @@
         """Model-specific cost function, evaluated on final context"""
         pass
 
     def make_forward(self, start_time, stop_time):
         """Create a generic forward pass through the simulation, returning loss"""
 
         # Take all the data and model parameters, run a simulation, return loss.
-        def _simulate(*data):
+        def _simulate(key, *data):
             context = self.context.with_time(start_time)
-            context = self.prepare_context(context, *data)
+            context = self.prepare_context(context, *data, key=key)
             results = self.simulator.advance_to(stop_time, context)
             return self.evaluate_cost(results.context)
 
         return _simulate
 
     def make_loss_fn(self, forward, params):
         """Create a loss function based on a forward pass of the simulation
 
         `params` here can be any PyTree - it will get flattened to a single array
         """
         # Flatten all optimizable parameters into a single array
         p0, unflatten = ravel_pytree(params)
 
         # Define the loss as the mean cost function over the data set
-        def _loss(p, *batch_data):
+        def _loss(p, key, *batch_data):
             # Map the forward pass over all the data points and return the loss
-            loss = batch_scan(partial(forward, unflatten(p)), *batch_data)
+            loss = batch_scan(partial(forward, key, unflatten(p)), *batch_data)
             return loss
 
         # JIT compile the loss function and return the initial parameter
         # array and unflatten function
         return jax.jit(_loss), p0, unflatten
 
-    def train(self, training_data, sim_start_time, sim_stop_time, epochs=100):
+    def train(
+        self,
+        training_data,
+        sim_start_time,
+        sim_stop_time,
+        epochs=100,
+        key=None,
+        params=None,
+        opt_state=None,
+    ):
         """Run the optimization loop over the training data"""
 
         if (
             self.simulator.max_major_steps is None
             or self.simulator.max_major_steps <= 0
         ):
             self.simulator.max_major_steps = estimate_max_major_steps(
                 self.simulator.system,
                 (sim_start_time, sim_stop_time),
                 self.simulator.max_major_step_length,
             )
 
+        if key is None:
+            key = jax.random.PRNGKey(np.random.randint(0, 2**32))
+
         # Create a function to evaluate the forward pass through the simulation
         forward = self.make_forward(sim_start_time, sim_stop_time)
 
         # Pull out the optimizable parameters from the context
-        params = self.optimizable_parameters(self.context)
+        if params is None:
+            params = self.optimizable_parameters(self.context)
 
         # Initialize the optimizer and create the loss function
         loss, p, unflatten = self.make_loss_fn(forward, params)
-        opt_state = self.optimizer.init(p)
+
+        if opt_state is None:
+            opt_state = self.optimizer.init(p)
+
+        self.opt_state = opt_state
 
         @jax.jit
-        def opt_step(p, opt_state, batch_data):
+        def opt_step(p, opt_state, key, batch_data):
+            key, subkey = jax.random.split(key)
             if batch_data:
-                loss_value, grads = jax.value_and_grad(loss)(p, *batch_data)
+                loss_value, grads = jax.value_and_grad(loss)(p, subkey, *batch_data)
             else:
-                loss_value, grads = jax.value_and_grad(loss)(p)
+                loss_value, grads = jax.value_and_grad(loss)(p, subkey)
 
             grads = jnp.clip(grads, *self.clip_range)
 
             updates, opt_state = self.optimizer.update(grads, opt_state, p)
             p = optax.apply_updates(p, updates)
-            return p, opt_state, loss_value
+            return p, opt_state, key, loss_value
 
         def _scan_fun(carry, batch_data):
-            p, opt_state, loss_value = opt_step(*carry, batch_data)
-            return (p, opt_state), loss_value
+            p, opt_state, key, loss_value = opt_step(*carry, batch_data)
+            return (p, opt_state, key), loss_value
 
         # Run the optimization loop
         for epoch in range(epochs):
-            (p, opt_state), batch_loss = jax.lax.scan(
-                _scan_fun, (p, opt_state), training_data
+            (p, self.opt_state, key), batch_loss = jax.lax.scan(
+                _scan_fun, (p, self.opt_state, key), training_data
             )
 
             if epoch % self.print_every == 0:
                 print(f"Epoch {epoch}, loss={jnp.mean(batch_loss)}")
 
         # Return the optimized parameters
         return unflatten(p)
```

## collimator/simulation/simulator.py

```diff
@@ -418,20 +418,24 @@
     if options.enable_tracing:
         _wrapped_simulate = jax.jit(_wrapped_simulate)
         _wrapped_simulate = Profiler.jaxjit_profiledfunc(
             _wrapped_simulate, "_wrapped_simulate"
         )
 
     # Run the simulation
-    final_context, results_data = _wrapped_simulate()
+    try:
+        final_context, results_data = _wrapped_simulate()
 
-    if postprocess and results_data is not None:
-        time, outputs = results_data.finalize()
-    else:
-        time, outputs = None, None
+        if postprocess and results_data is not None:
+            time, outputs = results_data.finalize()
+        else:
+            time, outputs = None, None
+
+    finally:
+        system.post_simulation_finalize()
 
     # Reset the integer time scale to the default value in case we decreased precision
     # to reach the end time of a long simulation.  Typically this won't do anything.
     if options.int_time_scale is not None:
         IntegerTime.set_default_scale()
 
     return SimulationResults(
@@ -690,41 +694,59 @@
         func = solver.flat_ode_rhs  # Raveled ODE RHS function
 
         # Close over the additional arguments so that the RHS function has the
         # signature `func(y, t)`.
         def _func(y, t):
             return func(y, t, context)
 
-        def _localize_zc_minor(solver_state, context_t0, context_tf, zc_events):
+        def _localize_zc_minor(
+            solver_state, context_t0, context_tf, zc_events, results_data
+        ):
             # Using the ODE solver interpolant, employ bisection to find a 'small' time
             # interval within which the earliest zero crossing occurrs. See
             # _bisection_step_fun for details about how bisection is employed for
             # localizing the zero crossing in time.
             int_t1 = IntegerTime.from_decimal(context_tf.time)
             int_t0 = IntegerTime.from_decimal(context_t0.time)
             _body_fun = partial(_bisection_step_fun, solver_state)
             carry = GuardIsolationData(int_t0, int_t1, zc_events, context_tf)
             search_data = backend.fori_loop(
                 0, self.zc_bisection_loop_count, _body_fun, carry
             )
             context_tf = search_data.context
             zc_events = search_data.guards
 
+            # record results sample for the ZC having 'occurred'
+            minor_step_end_time = IntegerTime.as_decimal(int_t1)
+            minor_step_start_time = IntegerTime.as_decimal(int_t0)
+            zc_occur_time = context_tf.time - (
+                minor_step_end_time - minor_step_start_time
+            ) / (2 ** (self.zc_bisection_loop_count + 1))
+            context_zc_time = context_tf.with_time(zc_occur_time)
+            results_data = self.save_results(results_data, context_zc_time)
+
             # Handle any triggered zero-crossing events
             context_tf = self.system.handle_zero_crossings(zc_events, context_tf)
 
             # Re-initialize the solver, since the state may have been reset
             # Keep the last step size, since there's no reason to assume that the
             # dynamics have changed significantly as a result of the event.  If that is
             # the case, then we're relying on the adaptive stepping to re-calibrate.
-            solver_state = solver_state.with_context(context_tf)
-            return solver_state, context_tf, zc_events
-
-        def _no_events_fun(solver_state, context_t0, context_tf, zc_events):
-            return solver_state, context_tf, zc_events
+            #
+            # NOTE: this previously only updated the state and time of
+            # the solver state, but with multistep solvers (e.g. BDF), the
+            # solver needs to be fully reinitialized because the history
+            # of differences needs to be cleared and rebuilt over the next few steps.
+            solver_state = solver.initialize(context_tf)
+            return solver_state, context_tf, zc_events, results_data
+
+        def _no_events_fun(
+            solver_state, context_t0, context_tf, zc_events, results_data
+        ):
+            return solver_state, context_tf, zc_events, results_data
 
         def _ode_step(carry):
             _, solver_state, context_t0, results_data, zc_events = carry
 
             # Save results at the top of the loop. This will save data at t=t0,
             # but not at t=tf.  This is okay, since we will save the results at
             # the top of the next major step, as well as at the end of the main
@@ -739,16 +761,16 @@
             context = context_t0.with_time(solver_state.t).with_continuous_state(xc)
 
             # Check for zero-crossing events
             zc_events = determine_triggered_guards(zc_events, context)
 
             triggered = zc_events.has_triggered
 
-            args = (solver_state, context_t0, context, zc_events)
-            solver_state, context, zc_events = backend.cond(
+            args = (solver_state, context_t0, context, zc_events, results_data)
+            solver_state, context, zc_events, results_data = backend.cond(
                 triggered, _localize_zc_minor, _no_events_fun, *args
             )
 
             return (triggered, solver_state, context, results_data, zc_events)
 
         def _cond_fun(carry):
             triggered, solver_state, _, _, _ = carry
```

## collimator/simulation/types.py

```diff
@@ -134,14 +134,18 @@
     min_minor_step_size: float = None
     max_minor_step_size: float = None
 
     # This option determines whether the simulator saves any data.  If the
     # simulation is initiated from `simulate` this will be set automatically
     # depending on whether `recorded_signals` is provided.  Hence, this
     # should not need to be manually configured.
+    # FIXME: remove this and use `recorded_signals` instead. There are usecases
+    # where simulate() is not used and we use the Simulator's advance_to function
+    # directly. In those cases, recorded_signals can be set while save_time_series
+    # is False which is confusing.
     save_time_series: bool = False
 
     # Dictionary of ports (or other cache sources) for which the time series should
     # be recorded. Note that if the simulation is initiated from `simulate` and
     # `recorded_signals` is provided as a kwarg to `simulate`, anything set here
     # will be overridden.  Hence, this should not need to be manually configured.
     recorded_signals: dict[str, SystemCallback] = None
```

## Comparing `pycollimator-2.0.3.dist-info/LICENSE.header.txt` & `pycollimator-2.0.4.dist-info/LICENSE.header.txt`

 * *Files identical despite different names*

## Comparing `pycollimator-2.0.3.dist-info/LICENSE.md` & `pycollimator-2.0.4.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `pycollimator-2.0.3.dist-info/METADATA` & `pycollimator-2.0.4.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycollimator
-Version: 2.0.3
+Version: 2.0.4
 Summary: Collimator.ai core simulation engine and API client
 Author-email: Collimator <support@collimator.ai>
 License: AGPLv3+
 Project-URL: Homepage, https://www.collimator.ai
 Project-URL: Documentation, https://py.collimator.ai
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -19,21 +19,21 @@
 License-File: LICENSE.md
 Requires-Dist: click ~=8.1.7
 Requires-Dist: dataclasses-json ~=0.6.4
 Requires-Dist: dataclasses-jsonschema ~=2.16
 Requires-Dist: diffrax ~=0.5.0
 Requires-Dist: equinox ~=0.11.1
 Requires-Dist: fmpy ~=0.3.19
-Requires-Dist: jax ~=0.4.25
-Requires-Dist: jaxlib ~=0.4.25
+Requires-Dist: jax <=0.4.26,~=0.4.25
+Requires-Dist: jaxlib <=0.4.26,~=0.4.25
 Requires-Dist: jaxtyping ~=0.2.25
 Requires-Dist: jaxopt ~=0.8.3
 Requires-Dist: networkx ~=3.1
 Requires-Dist: numpy ~=1.26.0
-Requires-Dist: optax ~=0.1.5
+Requires-Dist: optax ~=0.2.2
 Requires-Dist: requests ~=2.31.0
 Requires-Dist: scipy ~=1.10.1
 Requires-Dist: sympy ~=1.11.1
 Requires-Dist: ts-type ~=0.2.9
 Requires-Dist: StrEnum ~=0.4.15 ; python_version < "3.11"
 Provides-Extra: all
 Requires-Dist: control ~=0.9.4 ; extra == 'all'
```

