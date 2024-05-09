# Comparing `tmp/t0-4.0.6rc0.tar.gz` & `tmp/t0-4.0.7rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "t0-4.0.6rc0.tar", last modified: Wed May  8 22:57:54 2024, max compression
+gzip compressed data, was "t0-4.0.7rc0.tar", last modified: Wed May  8 23:32:57 2024, max compression
```

## Comparing `t0-4.0.6rc0.tar` & `t0-4.0.7rc0.tar`

### file list

```diff
@@ -1,226 +1,214 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:57:54.017145 t0-4.0.6rc0/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-08 22:57:40.000000 t0-4.0.6rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-08 22:57:40.000000 t0-4.0.6rc0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-08 22:57:40.000000 t0-4.0.6rc0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)    13790 2024-05-08 22:57:54.017145 t0-4.0.6rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 22:57:40.000000 t0-4.0.6rc0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:57:53.985145 t0-4.0.6rc0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)    12588 2024-05-08 22:57:40.000000 t0-4.0.6rc0/bin/00_deploy.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)    13192 2024-05-08 22:57:40.000000 t0-4.0.6rc0/bin/00_deploy_prod.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)    13970 2024-05-08 22:57:40.000000 t0-4.0.6rc0/bin/00_deploy_replay.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     1422 2024-05-08 22:57:40.000000 t0-4.0.6rc0/bin/00_patches.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     2147 2024-05-08 22:57:40.000000 t0-4.0.6rc0/bin/00_software.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     4602 2024-05-08 22:57:40.000000 t0-4.0.6rc0/bin/buildrelease.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     7118 2024-05-08 22:57:40.000000 t0-4.0.6rc0/bin/cmst0_backlog_wma
--rwxr-xr-x   0 runner    (1001) docker     (127)     8335 2024-05-08 22:57:40.000000 t0-4.0.6rc0/bin/cmst0_late_workflows
--rwxr-xr-x   0 runner    (1001) docker     (127)    11425 2024-05-08 22:57:40.000000 t0-4.0.6rc0/bin/cmst0_long_jobs
--rwxr-xr-x   0 runner    (1001) docker     (127)     6694 2024-05-08 22:57:40.000000 t0-4.0.6rc0/bin/cmst0_paused_jobs
--rwxr-xr-x   0 runner    (1001) docker     (127)    11745 2024-05-08 22:57:40.000000 t0-4.0.6rc0/bin/diagnoseActiveRuns
--rwxr-xr-x   0 runner    (1001) docker     (127)     8094 2024-05-08 22:57:40.000000 t0-4.0.6rc0/bin/forceCloseRuns
--rwxr-xr-x   0 runner    (1001) docker     (127)     5211 2024-05-08 22:57:40.000000 t0-4.0.6rc0/bin/tier0-mod-config
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:57:53.989145 t0-4.0.6rc0/etc/
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-08 22:57:40.000000 t0-4.0.6rc0/etc/ContainterConfig.sh
--rw-r--r--   0 runner    (1001) docker     (127)    72655 2024-05-08 22:57:40.000000 t0-4.0.6rc0/etc/HIProdOfflineConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)    65615 2024-05-08 22:57:40.000000 t0-4.0.6rc0/etc/HIReplayOfflineConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)    60169 2024-05-08 22:57:40.000000 t0-4.0.6rc0/etc/ProdOfflineConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)    54268 2024-05-08 22:57:40.000000 t0-4.0.6rc0/etc/ReplayOfflineConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)    18168 2024-05-08 22:57:40.000000 t0-4.0.6rc0/etc/ReplayOfflineConfigurationRun1.py
--rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-05-08 22:57:40.000000 t0-4.0.6rc0/etc/SLSAlarmsConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-08 22:57:40.000000 t0-4.0.6rc0/etc/Tier0Config.py
--rw-r--r--   0 runner    (1001) docker     (127)    77152 2024-05-08 22:57:40.000000 t0-4.0.6rc0/etc/XeXeProdOfflineConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)    70892 2024-05-08 22:57:40.000000 t0-4.0.6rc0/etc/XeXeReplayOfflineConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-08 22:57:51.000000 t0-4.0.6rc0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-08 22:57:40.000000 t0-4.0.6rc0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 22:57:54.017145 t0-4.0.6rc0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:57:53.981145 t0-4.0.6rc0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:57:53.985145 t0-4.0.6rc0/src/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:57:53.989145 t0-4.0.6rc0/src/python/T0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:57:53.989145 t0-4.0.6rc0/src/python/T0/ConditionUpload/
--rw-r--r--   0 runner    (1001) docker     (127)    12463 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/ConditionUpload/ConditionUploadAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/ConditionUpload/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    29389 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/ConditionUpload/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:57:53.993145 t0-4.0.6rc0/src/python/T0/JobSplitting/
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/JobSplitting/AlcaHarvest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/JobSplitting/Condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     6057 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/JobSplitting/Express.py
--rw-r--r--   0 runner    (1001) docker     (127)     6356 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/JobSplitting/ExpressMerge.py
--rw-r--r--   0 runner    (1001) docker     (127)    12570 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/JobSplitting/Repack.py
--rw-r--r--   0 runner    (1001) docker     (127)    12824 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/JobSplitting/RepackMerge.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/JobSplitting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:57:53.993145 t0-4.0.6rc0/src/python/T0/RunConfig/
--rw-r--r--   0 runner    (1001) docker     (127)    61626 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/RunConfig/RunConfigAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)    48913 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/RunConfig/Tier0Config.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/RunConfig/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:57:53.993145 t0-4.0.6rc0/src/python/T0/RunLumiCloseout/
--rw-r--r--   0 runner    (1001) docker     (127)     9035 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/RunLumiCloseout/RunLumiCloseoutAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/RunLumiCloseout/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:57:53.993145 t0-4.0.6rc0/src/python/T0/StorageManager/
--rw-r--r--   0 runner    (1001) docker     (127)     8326 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/StorageManager/StorageManagerAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/StorageManager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:57:53.993145 t0-4.0.6rc0/src/python/T0/WMBS/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:57:53.993145 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:57:53.993145 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/ConditionUpload/
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/ConditionUpload/CompleteFiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/ConditionUpload/FinishPCLforEmptyExpress.py
--rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/ConditionUpload/GetConditions.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/ConditionUpload/GetRunStopTime.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/ConditionUpload/IsPromptCalibrationFinished.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/ConditionUpload/MarkPromptCalibrationFinished.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/ConditionUpload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38733 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Create.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:57:53.993145 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/JobSplitting/
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/JobSplitting/InsertPromptCalibrationFile.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/JobSplitting/InsertSplitLumis.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/JobSplitting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:57:54.001145 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/
--rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/FindRecoRelease.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/FindRecoReleaseDatasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/GetExpressConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/GetHLTConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/GetPhEDExConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/GetRecoConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/GetRepackConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/GetRunInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/GetStreamDatasetTriggers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/GetStreamDatasets.py
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/GetStreamOnlineVersion.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/GetStreamStyle.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertCMSSWVersion.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertDatasetScenario.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertDatasetTrigger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertExpressConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertLumiSection.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertPhEDExConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertPrimaryDataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertPromptCalibration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertRecoConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertRecoReleaseConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertRepackConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertRun.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertRunStreamDone.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertSpecialDataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertStorageNode.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertStream.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertStreamCMSSWVersion.py
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertStreamDataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertStreamFileset.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertStreamStyle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertStreamer.py
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertTrigger.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertWorkflowMonitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/ReleasePromptReco.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/UpdateRun.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:57:54.005145 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/CheckActiveSplitLumis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/CheckClosedLumis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/CheckEndOfRunRecords.py
--rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/CloseRunStreamFilesets.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/CloseRuns.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/DeleteStreamers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/FinalCloseLumi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/FindActiveRuns.py
--rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/FindClosedLumis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/FindClosedRuns.py
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/FindHighContLumi.py
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/FindOpenRuns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/FindStoppedRuns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/ForceCloseLumi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/GetClosedLumisForStream.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/GetFileCountOnOpenLumis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/GetFilesForStreamLumi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/GetOpenRunStreamLumicount.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/InsertClosedLumi.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/StopRuns.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:57:54.005145 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/SMNotification/
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/SMNotification/GetFinishedStreamers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/SMNotification/InsertOfflineFileStatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/SMNotification/MarkStreamersFinished.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/SMNotification/UpdateOfflineFileStatus.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/SMNotification/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:57:54.005145 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/StorageManager/
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/StorageManager/GetNewData.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/StorageManager/GetRunInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/StorageManager/GetRunSetup.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/StorageManager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:57:54.009145 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Subscriptions/
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Subscriptions/GetAllFiles.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Subscriptions/GetAvailableConditionFiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Subscriptions/GetAvailableExpressFiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Subscriptions/GetAvailableExpressMergeFiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Subscriptions/GetAvailableRepackFiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Subscriptions/GetAvailableRepackMergeFiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Subscriptions/GetLumiHolesForRepack.py
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Subscriptions/GetLumiHolesForRepackMerge.py
--rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Subscriptions/GetUsedLumis.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Subscriptions/HaveAvailableFile.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Subscriptions/HaveJobGroup.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Subscriptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:57:54.013145 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/T0DataSvc/
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/T0DataSvc/GetDatasetLocked.py
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/T0DataSvc/GetExpressConfigs.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/T0DataSvc/GetNewRun.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/T0DataSvc/GetPromptRecoStatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/T0DataSvc/GetRecoConfigs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/T0DataSvc/GetRunStreamDone.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/T0DataSvc/GetSkippedStreamers.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/T0DataSvc/InsertDatasetLocked.py
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/T0DataSvc/InsertExpressConfigs.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/T0DataSvc/InsertNewRun.py
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/T0DataSvc/InsertRecoConfigs.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/T0DataSvc/InsertRecoLocked.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/T0DataSvc/InsertRunDatasetDone.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/T0DataSvc/InsertRunStreamDone.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/T0DataSvc/InsertSkippedStreamers.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateDatasetLocked.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateExpressConfigs.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateNewRun.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateRecoConfigs.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateRecoLocked.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateRunDatasetDone.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateRunStreamDone.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateSkippedStreamers.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/T0DataSvc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:57:54.017145 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/
--rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/FeedStreamers.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/FindNewExpressRuns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/FindNewRunStreams.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/FindNewRuns.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/GetDeploymentID.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/GetExpressReadyRuns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/GetNotClosedOutWorkflows.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/GetPromptRecoWorkflowsForMonitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/GetRunDatasetDone.py
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/GetRunDatasetNew.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/GetRunDatasetReleased.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/GetStreamerWorkflowsForMonitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/MarkCloseoutWorkflowMonitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/MarkTrackedWorkflowMonitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     6700 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/MarkWorkflowsInjected.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/ReleaseExpress.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/SetDeploymentID.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/UpdateRecoReleaseConfigs.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/Oracle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMBS/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:57:54.017145 t0-4.0.6rc0/src/python/T0/WMSpec/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:57:54.017145 t0-4.0.6rc0/src/python/T0/WMSpec/StdSpecs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMSpec/StdSpecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/WMSpec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:57:54.017145 t0-4.0.6rc0/src/python/T0.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13790 2024-05-08 22:57:53.000000 t0-4.0.6rc0/src/python/T0.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10026 2024-05-08 22:57:53.000000 t0-4.0.6rc0/src/python/T0.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 22:57:53.000000 t0-4.0.6rc0/src/python/T0.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-08 22:57:53.000000 t0-4.0.6rc0/src/python/T0.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:57:54.017145 t0-4.0.6rc0/src/python/T0Component/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:57:54.017145 t0-4.0.6rc0/src/python/T0Component/Tier0Auditor/
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0Component/Tier0Auditor/Tier0Auditor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0Component/Tier0Auditor/Tier0AuditorPoller.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0Component/Tier0Auditor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:57:54.017145 t0-4.0.6rc0/src/python/T0Component/Tier0Feeder/
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0Component/Tier0Feeder/Tier0Feeder.py
--rw-r--r--   0 runner    (1001) docker     (127)    31635 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0Component/Tier0Feeder/Tier0FeederPoller.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0Component/Tier0Feeder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 22:57:40.000000 t0-4.0.6rc0/src/python/T0Component/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:32:57.617895 t0-4.0.7rc0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-08 23:32:45.000000 t0-4.0.7rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-08 23:32:45.000000 t0-4.0.7rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-08 23:32:45.000000 t0-4.0.7rc0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)    13790 2024-05-08 23:32:57.617895 t0-4.0.7rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 23:32:45.000000 t0-4.0.7rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-08 23:32:55.000000 t0-4.0.7rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-08 23:32:45.000000 t0-4.0.7rc0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 23:32:57.617895 t0-4.0.7rc0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:32:57.585894 t0-4.0.7rc0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:32:57.589894 t0-4.0.7rc0/src/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:32:57.589894 t0-4.0.7rc0/src/python/T0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:32:57.589894 t0-4.0.7rc0/src/python/T0/ConditionUpload/
+-rw-r--r--   0 runner    (1001) docker     (127)    12463 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/ConditionUpload/ConditionUploadAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/ConditionUpload/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29389 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/ConditionUpload/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:32:57.589894 t0-4.0.7rc0/src/python/T0/JobSplitting/
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/JobSplitting/AlcaHarvest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/JobSplitting/Condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6057 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/JobSplitting/Express.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6356 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/JobSplitting/ExpressMerge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12570 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/JobSplitting/Repack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12824 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/JobSplitting/RepackMerge.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/JobSplitting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:32:57.593894 t0-4.0.7rc0/src/python/T0/RunConfig/
+-rw-r--r--   0 runner    (1001) docker     (127)    61626 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/RunConfig/RunConfigAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48913 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/RunConfig/Tier0Config.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/RunConfig/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:32:57.593894 t0-4.0.7rc0/src/python/T0/RunLumiCloseout/
+-rw-r--r--   0 runner    (1001) docker     (127)     9035 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/RunLumiCloseout/RunLumiCloseoutAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/RunLumiCloseout/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:32:57.593894 t0-4.0.7rc0/src/python/T0/StorageManager/
+-rw-r--r--   0 runner    (1001) docker     (127)     8326 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/StorageManager/StorageManagerAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/StorageManager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:32:57.593894 t0-4.0.7rc0/src/python/T0/WMBS/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:32:57.593894 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:32:57.593894 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/ConditionUpload/
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/ConditionUpload/CompleteFiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/ConditionUpload/FinishPCLforEmptyExpress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/ConditionUpload/GetConditions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/ConditionUpload/GetRunStopTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/ConditionUpload/IsPromptCalibrationFinished.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/ConditionUpload/MarkPromptCalibrationFinished.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/ConditionUpload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38733 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Create.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:32:57.593894 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/JobSplitting/
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/JobSplitting/InsertPromptCalibrationFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/JobSplitting/InsertSplitLumis.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/JobSplitting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:32:57.601894 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/
+-rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/FindRecoRelease.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/FindRecoReleaseDatasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/GetExpressConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/GetHLTConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/GetPhEDExConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/GetRecoConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/GetRepackConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/GetRunInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/GetStreamDatasetTriggers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/GetStreamDatasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/GetStreamOnlineVersion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/GetStreamStyle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertCMSSWVersion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertDatasetScenario.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertDatasetTrigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertExpressConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertLumiSection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertPhEDExConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertPrimaryDataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertPromptCalibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertRecoConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertRecoReleaseConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertRepackConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertRun.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertRunStreamDone.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertSpecialDataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertStorageNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertStream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertStreamCMSSWVersion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertStreamDataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertStreamFileset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertStreamStyle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertStreamer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertTrigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertWorkflowMonitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/ReleasePromptReco.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/UpdateRun.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:32:57.601894 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/CheckActiveSplitLumis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/CheckClosedLumis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/CheckEndOfRunRecords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/CloseRunStreamFilesets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/CloseRuns.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/DeleteStreamers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/FinalCloseLumi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/FindActiveRuns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/FindClosedLumis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/FindClosedRuns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/FindHighContLumi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/FindOpenRuns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/FindStoppedRuns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/ForceCloseLumi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/GetClosedLumisForStream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/GetFileCountOnOpenLumis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/GetFilesForStreamLumi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/GetOpenRunStreamLumicount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/InsertClosedLumi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/StopRuns.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:32:57.605894 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/SMNotification/
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/SMNotification/GetFinishedStreamers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/SMNotification/InsertOfflineFileStatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/SMNotification/MarkStreamersFinished.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/SMNotification/UpdateOfflineFileStatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/SMNotification/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:32:57.605894 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/StorageManager/
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/StorageManager/GetNewData.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/StorageManager/GetRunInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/StorageManager/GetRunSetup.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/StorageManager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:32:57.605894 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Subscriptions/GetAllFiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Subscriptions/GetAvailableConditionFiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Subscriptions/GetAvailableExpressFiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Subscriptions/GetAvailableExpressMergeFiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Subscriptions/GetAvailableRepackFiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Subscriptions/GetAvailableRepackMergeFiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Subscriptions/GetLumiHolesForRepack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Subscriptions/GetLumiHolesForRepackMerge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Subscriptions/GetUsedLumis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Subscriptions/HaveAvailableFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Subscriptions/HaveJobGroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Subscriptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:32:57.609894 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/T0DataSvc/
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/T0DataSvc/GetDatasetLocked.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/T0DataSvc/GetExpressConfigs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/T0DataSvc/GetNewRun.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/T0DataSvc/GetPromptRecoStatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/T0DataSvc/GetRecoConfigs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/T0DataSvc/GetRunStreamDone.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/T0DataSvc/GetSkippedStreamers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/T0DataSvc/InsertDatasetLocked.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/T0DataSvc/InsertExpressConfigs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/T0DataSvc/InsertNewRun.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/T0DataSvc/InsertRecoConfigs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/T0DataSvc/InsertRecoLocked.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/T0DataSvc/InsertRunDatasetDone.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/T0DataSvc/InsertRunStreamDone.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/T0DataSvc/InsertSkippedStreamers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateDatasetLocked.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateExpressConfigs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateNewRun.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateRecoConfigs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateRecoLocked.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateRunDatasetDone.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateRunStreamDone.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateSkippedStreamers.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/T0DataSvc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:32:57.613894 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/FeedStreamers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/FindNewExpressRuns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/FindNewRunStreams.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/FindNewRuns.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/GetDeploymentID.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/GetExpressReadyRuns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/GetNotClosedOutWorkflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/GetPromptRecoWorkflowsForMonitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/GetRunDatasetDone.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/GetRunDatasetNew.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/GetRunDatasetReleased.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/GetStreamerWorkflowsForMonitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/MarkCloseoutWorkflowMonitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/MarkTrackedWorkflowMonitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6700 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/MarkWorkflowsInjected.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/ReleaseExpress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/SetDeploymentID.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/UpdateRecoReleaseConfigs.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/Oracle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMBS/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:32:57.613894 t0-4.0.7rc0/src/python/T0/WMSpec/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:32:57.613894 t0-4.0.7rc0/src/python/T0/WMSpec/StdSpecs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMSpec/StdSpecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/WMSpec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:32:57.617895 t0-4.0.7rc0/src/python/T0.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13790 2024-05-08 23:32:57.000000 t0-4.0.7rc0/src/python/T0.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9867 2024-05-08 23:32:57.000000 t0-4.0.7rc0/src/python/T0.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 23:32:57.000000 t0-4.0.7rc0/src/python/T0.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-08 23:32:57.000000 t0-4.0.7rc0/src/python/T0.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:32:57.613894 t0-4.0.7rc0/src/python/T0Component/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:32:57.613894 t0-4.0.7rc0/src/python/T0Component/Tier0Auditor/
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0Component/Tier0Auditor/Tier0Auditor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0Component/Tier0Auditor/Tier0AuditorPoller.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0Component/Tier0Auditor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:32:57.613894 t0-4.0.7rc0/src/python/T0Component/Tier0Feeder/
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0Component/Tier0Feeder/Tier0Feeder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31635 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0Component/Tier0Feeder/Tier0FeederPoller.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0Component/Tier0Feeder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0Component/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:32:57.589894 t0-4.0.7rc0/src/python/T0Tools/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:32:57.617895 t0-4.0.7rc0/src/python/T0Tools/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7118 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0Tools/bin/cmst0_backlog_wma
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8335 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0Tools/bin/cmst0_late_workflows
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11425 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0Tools/bin/cmst0_long_jobs
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6694 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0Tools/bin/cmst0_paused_jobs
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11745 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0Tools/bin/diagnoseActiveRuns
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8094 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0Tools/bin/forceCloseRuns
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5211 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0Tools/bin/tier0-mod-config
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:32:57.617895 t0-4.0.7rc0/src/python/T0Tools/etc/
+-rw-r--r--   0 runner    (1001) docker     (127)    60169 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0Tools/etc/ProdOfflineConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54268 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0Tools/etc/ReplayOfflineConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-08 23:32:45.000000 t0-4.0.7rc0/src/python/T0Tools/etc/Tier0Config.py
```

### Comparing `t0-4.0.6rc0/LICENSE` & `t0-4.0.7rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/NOTICE` & `t0-4.0.7rc0/NOTICE`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/PKG-INFO` & `t0-4.0.7rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: T0
-Version: 4.0.6rc0
+Version: 4.0.7rc0
 Summary: This package contains the code that is involved in the Tier 0 agent when its deployed
 Author: Dirk Hufnagel
 Author-email: Dirk.Hufnagel@cern.ch
 Maintainer-email: WMCore <ms.unmerged@cern.ch>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
```

### Comparing `t0-4.0.6rc0/bin/cmst0_backlog_wma` & `t0-4.0.7rc0/src/python/T0Tools/bin/cmst0_backlog_wma`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/bin/cmst0_late_workflows` & `t0-4.0.7rc0/src/python/T0Tools/bin/cmst0_late_workflows`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/bin/cmst0_long_jobs` & `t0-4.0.7rc0/src/python/T0Tools/bin/cmst0_long_jobs`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/bin/cmst0_paused_jobs` & `t0-4.0.7rc0/src/python/T0Tools/bin/cmst0_paused_jobs`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/bin/diagnoseActiveRuns` & `t0-4.0.7rc0/src/python/T0Tools/bin/diagnoseActiveRuns`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/bin/forceCloseRuns` & `t0-4.0.7rc0/src/python/T0Tools/bin/forceCloseRuns`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/bin/tier0-mod-config` & `t0-4.0.7rc0/src/python/T0Tools/bin/tier0-mod-config`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/etc/HIProdOfflineConfiguration.py` & `t0-4.0.7rc0/src/python/T0Tools/etc/ProdOfflineConfiguration.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 Processing configuration for the Tier0 - Production version
 """
 from __future__ import print_function
 
 from T0.RunConfig.Tier0Config import addDataset
 from T0.RunConfig.Tier0Config import createTier0Config
 from T0.RunConfig.Tier0Config import setAcquisitionEra
+from T0.RunConfig.Tier0Config import setEmulationAcquisitionEra
 from T0.RunConfig.Tier0Config import setDefaultScramArch
+from T0.RunConfig.Tier0Config import setScramArch
 from T0.RunConfig.Tier0Config import setBaseRequestPriority
 from T0.RunConfig.Tier0Config import setBackfill
 from T0.RunConfig.Tier0Config import setBulkDataType
 from T0.RunConfig.Tier0Config import setProcessingSite
 from T0.RunConfig.Tier0Config import setDQMDataTier
 from T0.RunConfig.Tier0Config import setDQMUploadUrl
 from T0.RunConfig.Tier0Config import setPromptCalibrationConfig
@@ -21,20 +23,22 @@
 from T0.RunConfig.Tier0Config import addRepackConfig
 from T0.RunConfig.Tier0Config import addExpressConfig
 from T0.RunConfig.Tier0Config import setInjectMinRun
 from T0.RunConfig.Tier0Config import setInjectMaxRun
 from T0.RunConfig.Tier0Config import setStreamerPNN
 from T0.RunConfig.Tier0Config import addSiteConfig
 from T0.RunConfig.Tier0Config import setStorageSite
+from T0.RunConfig.Tier0Config import setExtraStreamDatasetMap
+
 
 # Create the Tier0 configuration object
 tier0Config = createTier0Config()
 
 # Set the verstion configuration (not used at the moment)
-setConfigVersion(tier0Config, "replace with real version")
+setConfigVersion(tier0Config, "3.1.5")
 
 # Set the min run number:
 setInjectMinRun(tier0Config, 9999999)
 
 # Set the max run number:
 setInjectMaxRun(tier0Config, 9999999)
 
@@ -43,37 +47,39 @@
 storageSite = "T0_CH_CERN_Disk"
 streamerPNN = "T0_CH_CERN_Disk"
 
 addSiteConfig(tier0Config, "T0_CH_CERN_Disk",
                 siteLocalConfig="/cvmfs/cms.cern.ch/SITECONF/T0_CH_CERN/JobConfig/site-local-config.xml",
                 overrideCatalog="T2_CH_CERN,,T0_CH_CERN,CERN_EOS_T0,XRootD"
                 )
+
 # Set global parameters:
 #  Acquisition era
 #  BaseRequestPriority
 #  Backfill mode
 #  Data type
 #  Processing site (where jobs run)
 #  PhEDEx locations
-setAcquisitionEra(tier0Config, "HIRun2023A")
+setAcquisitionEra(tier0Config, "Run2024D")
+setEmulationAcquisitionEra(tier0Config, "Emulation2024")
 setBaseRequestPriority(tier0Config, 251000)
 setBackfill(tier0Config, None)
-setBulkDataType(tier0Config, "hidata")
+setBulkDataType(tier0Config, "data")
 setProcessingSite(tier0Config, processingSite)
 setStreamerPNN(tier0Config, streamerPNN)
 setStorageSite(tier0Config, storageSite)
 
 # Override for DQM data tier
 setDQMDataTier(tier0Config, "DQMIO")
 
 # Define the two default timeouts for reco release
 # First timeout is used directly for reco release
 # Second timeout is used for the data service PromptReco start check
 # (to basically say we started PromptReco even though we haven't)
-defaultRecoTimeout = 154 * 3600
+defaultRecoTimeout = 48 * 3600
 defaultRecoLockTimeout = 1800
 
 # DQM Server
 setDQMUploadUrl(tier0Config, "https://cmsweb.cern.ch/dqm/offline")
 
 # PCL parameters
 setPromptCalibrationConfig(tier0Config,
@@ -87,76 +93,95 @@
 # Special syntax supported for cmssw version, processing version, global tag and processing scenario
 # https://github.com/dmwm/T0/blob/master/src/python/T0/RunConfig/RunConfigAPI.py#L828
 #
 # { 'acqEra': {'Era1': Value1, 'Era2': Value2},
 #   'maxRun': {100000: Value3, 200000: Value4},
 #   'default': Value5 }
 
+# maxRunPreviousConfig = 999999 # Last run before era change 08/09/23
 # Defaults for CMSSW version
 defaultCMSSWVersion = {
-    'default': "CMSSW_13_2_6",
+    'default': "CMSSW_14_0_6_patch1",
+    #'acqEra': {'Run2024B': "CMSSW_14_0_4"}
+    #'maxRun': {maxRunPreviousConfig: "CMSSW_13_2_2"}
 }
 
 # Configure ScramArch
-setDefaultScramArch(tier0Config, "el8_amd64_gcc11")
+setDefaultScramArch(tier0Config, "el8_amd64_gcc12")
+#setScramArch(tier0Config, "CMSSW_13_3_2_patch1", "el8_amd64_gcc12")
+#setScramArch(tier0Config, "CMSSW_13_3_2", "el8_amd64_gcc12")
+#setScramArch(tier0Config, "CMSSW_13_3_0", "el8_amd64_gcc12")
 
 # Configure scenarios
-ppScenario = "ppEra_Run3_2023"
+ppScenario = "ppEra_Run3"
+ppScenarioB0T = "ppEra_Run3"
 cosmicsScenario = "cosmicsEra_Run3"
 hcalnzsScenario = "hcalnzsEra_Run3"
-HIhcalnzsScenario = "hcalnzsEra_Run3_pp_on_PbPb"
-hiScenario = "ppEra_Run3_pp_on_PbPb_2023"
 alcaTrackingOnlyScenario = "trackingOnlyEra_Run3"
-HIalcaTrackingOnlyScenario = "trackingOnlyEra_Run3_pp_on_PbPb"
 alcaTestEnableScenario = "AlCaTestEnable"
 alcaLumiPixelsScenario = "AlCaLumiPixels_Run3"
 alcaPPSScenario = "AlCaPPS_Run3"
 hiTestppScenario = "ppEra_Run3_pp_on_PbPb_2023"
 hiRawPrimeScenario = "ppEra_Run3_pp_on_PbPb_approxSiStripClusters_2023"
-hiForwardScenario = "ppEra_Run3_2023_repacked"
 
 # Defaults for processing version
 alcarawProcVersion = {
-    'default': "2",
+    'default': 1
 }
 
 defaultProcVersionReco = {
-    'default': "2",
+    'default': 1
 }
 
 expressProcVersion = {
-    'default': "2",
+    'default': 1
 }
 
 # Defaults for GlobalTag
-expressGlobalTag = "132X_dataRun3_Express_v4"
-promptrecoGlobalTag = "132X_dataRun3_Prompt_v4"
+expressGlobalTag = {
+    'default': "140X_dataRun3_Express_v3",
+    'acqEra': {'Run2024B': "140X_dataRun3_Express_v2"}
+    #'maxRun': {maxRunPreviousConfig: "132X_dataRun3_Express_v3"}
+}
+promptrecoGlobalTag = {
+    'default': "140X_dataRun3_Prompt_v2",
+    #'acqEra': {'Run2023E': "132X_dataRun3_Prompt_v2"},
+    #'maxRun': {maxRunPreviousConfig: "132X_dataRun3_Prompt_v2"}
+}
 
 # Mandatory for CondDBv2
 globalTagConnect = "frontier://PromptProd/CMS_CONDITIONS"
 
 # Multicore settings
 numberOfCores = 8
 
 # Splitting parameters for PromptReco
-defaultRecoSplitting = 750 * numberOfCores # reduced from 3000
+defaultRecoSplitting = 750 * numberOfCores
 hiRecoSplitting = 200 * numberOfCores
 alcarawSplitting = 20000 * numberOfCores
 
 #
 # Setup repack and express mappings
 #
 repackVersionOverride = {
     "CMSSW_12_6_3" : "CMSSW_12_6_4"
 }
 
 expressVersionOverride = {
     "CMSSW_12_6_3" : "CMSSW_12_6_4"
 }
 
+
+# Additional Repack mappings
+#    L1Scouting stream
+setExtraStreamDatasetMap(tier0Config,{
+                                        "L1Scouting": {"Dataset":"L1Scouting"}
+                                    }
+                         )
+
 #set default repack settings for bulk streams
 addRepackConfig(tier0Config, "Default",
                 proc_ver=1, # Should remain 1. Changing it can cause several issues.
                 maxSizeSingleLumi=24 * 1024 * 1024 * 1024,
                 maxSizeMultiLumi=8 * 1024 * 1024 * 1024,
                 minInputSize=2.1 * 1024 * 1024 * 1024,
                 maxInputSize=4 * 1024 * 1024 * 1024,
@@ -165,31 +190,42 @@
                 maxInputEvents=3 * 1000 * 1000,
                 maxInputFiles=1000,
                 maxLatency=24 * 3600,
                 blockCloseDelay=24 * 3600,
                 maxMemory=2000,
                 versionOverride=repackVersionOverride)
 
+addRepackConfig(tier0Config, "ScoutingPF",
+                proc_ver=1, # Should remain 1. Changing it can cause several issues.
+                dataTier="HLTSCOUT",
+                versionOverride=repackVersionOverride)
+
+addRepackConfig(tier0Config, "L1Scouting",
+                proc_ver=1, # Should remain 1. Changing it can cause several issues.
+                dataTier="L1SCOUT",
+                versionOverride=repackVersionOverride)
+
+
 addDataset(tier0Config, "Default",
            do_reco=False,
-           write_reco=False, write_aod=True, write_miniaod=True, write_nanoaod=False, write_dqm=False,
+           write_reco=False, write_aod=True, write_miniaod=True, write_nanoaod=True, write_dqm=False,
            reco_delay=defaultRecoTimeout,
            reco_delay_offset=defaultRecoLockTimeout,
            reco_split=defaultRecoSplitting,
            proc_version=defaultProcVersionReco,
            cmssw_version=defaultCMSSWVersion,
            multicore=numberOfCores,
            global_tag=promptrecoGlobalTag,
            global_tag_connect=globalTagConnect,
            archival_node="T0_CH_CERN_MSS",
-           tape_node="T0_CH_CERN_MSS",
-           disk_node="T2_CH_CERN",
-           siteWhitelist = ["T2_CH_CERN_P5", "T2_CH_CERN", "T1_IT_CNAF", "T1_DE_KIT", "T1_FR_CCIN2P3", "T1_UK_RAL"],
+           tape_node="T1_US_FNAL_MSS",
+           disk_node="T1_US_FNAL_Disk",
+           siteWhitelist = ["T2_CH_CERN_P5", "T2_CH_CERN"],
            raw_to_disk=False,
-           aod_to_disk=False,
+           aod_to_disk=True,
            blockCloseDelay=24 * 3600,
            timePerEvent=5,
            sizePerEvent=1500,
            maxMemoryperCore=2000,
            dataset_lifetime=3*30*24*3600,#lifetime for container rules. Default 3 months
            scenario=ppScenario)
 
@@ -200,17 +236,19 @@
 addExpressConfig(tier0Config, "Express",
                  scenario=ppScenario,
                  diskNode="T2_CH_CERN",
                  data_tiers=["FEVT"],
                  write_dqm=True,
                  alca_producers=["SiStripPCLHistos", "SiStripCalZeroBias", "SiStripCalMinBias", "SiStripCalMinBiasAAG",
                                  "TkAlMinBias", "SiPixelCalZeroBias", "SiPixelCalSingleMuon", "SiPixelCalSingleMuonTight",
+                                 "TkAlZMuMu",
                                  "PromptCalibProd", "PromptCalibProdSiStrip", "PromptCalibProdSiPixelAli",
                                  "PromptCalibProdSiStripGains", "PromptCalibProdSiStripGainsAAG", "PromptCalibProdSiPixel",
-                                 "PromptCalibProdSiPixelLA", "PromptCalibProdSiStripHitEff", "PromptCalibProdSiPixelAliHG"
+                                 "PromptCalibProdSiPixelLA", "PromptCalibProdSiStripHitEff", "PromptCalibProdSiPixelAliHG",
+                                 "PromptCalibProdSiPixelAliHGComb"
                                 ],
                  dqm_sequences=["@standardDQMExpress"],
                  reco_version=defaultCMSSWVersion,
                  multicore=numberOfCores,
                  global_tag_connect=globalTagConnect,
                  global_tag=expressGlobalTag,
                  proc_ver=expressProcVersion,
@@ -297,15 +335,15 @@
                  periodicHarvestInterval=24 * 3600,
                  blockCloseDelay=2 * 3600,
                  timePerEvent=4,
                  sizePerEvent=1700,
                  versionOverride=expressVersionOverride,
                  maxMemoryperCore=2000,
                  archivalNode="T0_CH_CERN_MSS",
-                 dataType="hidata",
+                 dataType="data",
                  dataset_lifetime=3*30*24*3600,#lifetime for container rules. Default 3 months
                  tape_node="T1_US_FNAL_MSS")
 
 addExpressConfig(tier0Config, "ExpressAlignment",
                  scenario=alcaTrackingOnlyScenario,
                  data_tiers=["ALCARECO"],
                  write_dqm=True,
@@ -380,28 +418,26 @@
                  sizePerEvent=1700,
                  maxMemoryperCore=2000,
                  dataset_lifetime=12*30*24*3600,#lifetime for container rules. Default 12 months
                  diskNode="T2_CH_CERN",
                  versionOverride=expressVersionOverride)
 
 #####################
-### HI Tests 2022 ###
+### HI Tests 2018 ###
 #####################
 
 addExpressConfig(tier0Config, "HIExpress",
                  scenario=hiTestppScenario,
                  diskNode="T2_CH_CERN",
                  data_tiers=["FEVT"],
                  write_dqm=True,
                  alca_producers=["SiStripPCLHistos", "SiStripCalZeroBias", "SiStripCalMinBias", "SiStripCalMinBiasAAG",
-                                 "TkAlMinBias", "SiPixelCalZeroBias","SiPixelCalSingleMuon", "SiPixelCalSingleMuonTight",
-                                 "SiPixelCalSingleMuonLoose",
+                                 "TkAlMinBias", "LumiPixelsMinBias", "SiPixelCalZeroBias",
                                  "PromptCalibProd", "PromptCalibProdSiStrip", "PromptCalibProdSiPixelAli",
-                                 "PromptCalibProdSiStripGains", "PromptCalibProdSiStripGainsAAG", "PromptCalibProdSiPixel",
-                                 "PromptCalibProdSiPixelLA", "PromptCalibProdSiStripHitEff", "PromptCalibProdSiPixelAliHG"
+                                 "PromptCalibProdSiStripGains", "PromptCalibProdSiStripGainsAAG", "PromptCalibProdSiPixel"
                                 ],
                  reco_version=defaultCMSSWVersion,
                  multicore=numberOfCores,
                  global_tag_connect=globalTagConnect,
                  global_tag=expressGlobalTag,
                  proc_ver=expressProcVersion,
                  maxInputRate=23 * 1000,
@@ -413,43 +449,19 @@
                  blockCloseDelay=1200,
                  timePerEvent=4,
                  sizePerEvent=1700,
                  maxMemoryperCore=2000,
                  dataset_lifetime=3*30*24*3600,#lifetime for container rules. Default 3 months
                  versionOverride=expressVersionOverride)
 
-addExpressConfig(tier0Config, "HIExpressRawPrime",
-                 scenario=hiRawPrimeScenario,
-                 diskNode="T2_CH_CERN",
-                 data_tiers=["FEVT"],
-                 write_dqm=True,
-                 alca_producers=["SiStripCalMinBias", "SiStripCalMinBiasAAG"],
-                 reco_version=defaultCMSSWVersion,
-                 multicore=numberOfCores,
-                 global_tag_connect=globalTagConnect,
-                 global_tag=expressGlobalTag,
-                 proc_ver=expressProcVersion,
-                 maxInputRate=23 * 1000,
-                 maxInputEvents=400,
-                 maxInputSize=2 * 1024 * 1024 * 1024,
-                 maxInputFiles=15,
-                 maxLatency=15 * 23,
-                 periodicHarvestInterval=20 * 60,
-                 blockCloseDelay=1200,
-                 timePerEvent=4,
-                 sizePerEvent=1700,
-                 maxMemoryperCore=2000,
-                 dataset_lifetime=3*30*24*3600,#lifetime for container rules. Default 3 months
-                 versionOverride=expressVersionOverride)
-
 addExpressConfig(tier0Config, "HIExpressAlignment",
-                 scenario=HIalcaTrackingOnlyScenario,
+                 scenario=hiTestppScenario,
                  data_tiers=["ALCARECO", "RAW"],
                  write_dqm=True,
-                 alca_producers=["TkAlMinBias", "PromptCalibProdBeamSpotHP"],
+                 alca_producers=["TkAlMinBias"],
                  dqm_sequences=["@trackingOnlyDQM"],
                  reco_version=defaultCMSSWVersion,
                  raw_to_disk=True,
                  multicore=numberOfCores,
                  global_tag_connect=globalTagConnect,
                  global_tag=expressGlobalTag,
                  proc_ver=expressProcVersion,
@@ -463,38 +475,14 @@
                  timePerEvent=4,
                  sizePerEvent=1700,
                  versionOverride=expressVersionOverride,
                  maxMemoryperCore=2000,
                  dataset_lifetime=3*30*24*3600,#lifetime for container rules. Default 3 months
                  diskNode="T2_CH_CERN")
 
-addExpressConfig(tier0Config, "HIHLTMonitor",
-                 scenario=hiTestppScenario,
-                 diskNode="T2_CH_CERN",
-                 data_tiers=["FEVTHLTALL"],
-                 write_dqm=True,
-                 alca_producers=[],
-                 dqm_sequences=["@HLTMon"],
-                 reco_version=defaultCMSSWVersion,
-                 multicore=numberOfCores,
-                 global_tag_connect=globalTagConnect,
-                 global_tag=expressGlobalTag,
-                 proc_ver=expressProcVersion,
-                 maxInputRate=23 * 1000,
-                 maxInputEvents=400,
-                 maxInputSize=2 * 1024 * 1024 * 1024,
-                 maxInputFiles=15,
-                 maxLatency=15 * 23,
-                 periodicHarvestInterval=20 * 60,
-                 blockCloseDelay=1200,
-                 timePerEvent=4,
-                 sizePerEvent=1700,
-                 versionOverride=expressVersionOverride,
-                 dataset_lifetime=3*30*24*3600)#lifetime for container rules. Default 3 months
-
 ###################################
 ### Standard Physics PDs (2022) ###
 ###################################
 
 DATASETS = ["BTagMu"]
 
 for dataset in DATASETS:
@@ -511,14 +499,15 @@
 
 for dataset in DATASETS:
     addDataset(tier0Config, dataset,
                do_reco=True,
                write_reco=False,
                write_aod=True,
                write_miniaod=False,
+               write_nanoaod=False,
                write_dqm=True,
                alca_producers=["SiStripCalCosmics", "SiPixelCalCosmics", "TkAlCosmics0T", "MuAlGlobalCosmics", "SiStripCalCosmicsNano"],
                physics_skims=["CosmicSP", "CosmicTP", "LogError", "LogErrorMonitor"],
                timePerEvent=0.5,
                sizePerEvent=155,
                scenario=cosmicsScenario)
 
@@ -559,35 +548,26 @@
                disk_node="T1_DE_KIT_Disk",
                alca_producers=["TkAlZMuMu", "MuAlCalIsolatedMu", "MuAlOverlaps", "MuAlZMuMu"],
                dqm_sequences=["@common", "@muon", "@lumi", "@L1TMuon"],
                physics_skims=["LogError", "LogErrorMonitor"],
                timePerEvent=1,
                scenario=ppScenario)
 
-DATASETS = ["ReservedDoubleMuonLowMass"]
-
-for dataset in DATASETS:
-    addDataset(tier0Config, dataset,
-               do_reco=False,
-               tape_node="T1_IT_CNAF_MSS",
-               disk_node="T1_IT_CNAF_Disk",
-               scenario=ppScenario)
-
 DATASETS = ["ParkingSingleMuon","ParkingSingleMuon0"]
 
 for dataset in DATASETS:
     addDataset(tier0Config, dataset,
                do_reco=True,
                siteWhitelist = ["T2_CH_CERN_P5", "T2_CH_CERN"],
                archival_node=None,
                tape_node="T0_CH_CERN_MSS",
                disk_node="T2_CH_CERN",
                scenario=ppScenario)
 
-DATASETS = ["ParkingSingleMuon1","ParkingSingleMuon2"]
+DATASETS = ["ParkingSingleMuon1","ParkingSingleMuon2","ParkingSingleMuon3","ParkingSingleMuon4","ParkingSingleMuon5","ParkingSingleMuon6","ParkingSingleMuon7"]
 
 for dataset in DATASETS:
     addDataset(tier0Config, dataset,
                do_reco=True,
                aod_to_disk=False,
                siteWhitelist = ["T2_CH_CERN_P5", "T2_CH_CERN"],
                archival_node=None,
@@ -703,15 +683,15 @@
     addDataset(tier0Config, dataset,
                do_reco=True,
                write_dqm=True,
                tape_node="T1_US_FNAL_MSS",  # JetHT was in "T1_UK_RAL_MSS" , MET was in "T1_DE_KIT_MSS"
                disk_node="T1_US_FNAL_Disk", # JetHT was in "T1_UK_RAL_Disk", MET was in "T1_DE_KIT_Disk"
                alca_producers=["HcalCalIsoTrkProducerFilter", "TkAlJetHT", "HcalCalNoise"],
                dqm_sequences=["@common", "@jetmet", "@L1TMon", "@hcal"],
-               physics_skims=["EXOHighMET", "EXODelayedJetMET", "JetHTJetPlusHOFilter", "EXODisappTrk", "LogError", "LogErrorMonitor"],
+               physics_skims=["EXOHighMET", "EXODelayedJetMET", "JetHTJetPlusHOFilter", "EXODisappTrk", "EXOSoftDisplacedVertices", "TeVJet", "LogError", "LogErrorMonitor"],
                timePerEvent=5.7,  # copied from JetHT - should be checked
                sizePerEvent=2250, # copied from JetHT - should be checked
                scenario=ppScenario)
 
 DATASETS = ["PPRefHardProbes0", "PPRefHardProbes1", "PPRefHardProbes2"]
 
 for dataset in DATASETS:
@@ -775,15 +755,15 @@
                tape_node="T1_FR_CCIN2P3_MSS",  # SingleMon was in "T1_US_FNAL_MSS" , DoubleMuon was in "T1_DE_KIT_MSS"
                disk_node="T1_FR_CCIN2P3_Disk", # SingleMon was in "T1_US_FNAL_Disk", DoubleMuon was in "T1_DE_KIT_Disk"
                alca_producers=["TkAlMuonIsolated", "HcalCalIterativePhiSym", "MuAlCalIsolatedMu",
                                "HcalCalHO", "HcalCalHBHEMuonProducerFilter",
                                "SiPixelCalSingleMuonLoose", "SiPixelCalSingleMuonTight",
                                "TkAlZMuMu", "TkAlDiMuonAndVertex"],
                dqm_sequences=["@common", "@muon", "@lumi", "@L1TMuon", "@jetmet"],
-               physics_skims=["ZMu", "EXODisappTrk", "LogError", "LogErrorMonitor", "EXOCSCCluster", "EXODisappMuon"],
+               physics_skims=["MUOJME", "ZMu", "EXODisappTrk", "LogError", "LogErrorMonitor", "EXOCSCCluster", "EXODisappMuon"],
                scenario=ppScenario)
 
 DATASETS = ["Muon1"]
 DATASETS += ["PPRefSingleMuon0", "PPRefSingleMuon1", "PPRefSingleMuon2"]
 
 for dataset in DATASETS:
     addDataset(tier0Config, dataset,
@@ -793,15 +773,15 @@
                tape_node="T1_US_FNAL_MSS",
                disk_node="T1_US_FNAL_Disk",
                alca_producers=["TkAlMuonIsolated", "HcalCalIterativePhiSym", "MuAlCalIsolatedMu",
                                "HcalCalHO", "HcalCalHBHEMuonProducerFilter",
                                "SiPixelCalSingleMuonLoose", "SiPixelCalSingleMuonTight",
                                "TkAlZMuMu", "TkAlDiMuonAndVertex"],
                dqm_sequences=["@common", "@muon", "@lumi", "@L1TMuon", "@jetmet"],
-               physics_skims=["ZMu", "EXODisappTrk", "LogError", "LogErrorMonitor", "EXOCSCCluster", "EXODisappMuon"],
+               physics_skims=["MUOJME", "ZMu", "EXODisappTrk", "LogError", "LogErrorMonitor", "EXOCSCCluster", "EXODisappMuon"],
                scenario=ppScenario)
 
 DATASETS = ["PPRefDoubleMuon0", "PPRefDoubleMuon1", "PPRefDoubleMuon2", "PPRefDoubleMuon3"]
 
 for dataset in DATASETS:
     addDataset(tier0Config, dataset,
                do_reco=True,
@@ -824,15 +804,14 @@
                alca_producers=["TkAlCosmicsInCollisions"],
                dqm_sequences=["@common"],
                physics_skims=["EXONoBPTXSkim", "LogError", "LogErrorMonitor"],
                tape_node="T1_UK_RAL_MSS",
                disk_node="T1_UK_RAL_Disk",
                scenario=ppScenario)
 
-
 DATASETS = ["SingleMuon"]
 
 for dataset in DATASETS:
     addDataset(tier0Config, dataset,
                do_reco=True,
                write_dqm=True,
                tape_node="T1_US_FNAL_MSS", # "T1_IT_CNAF_MSS", CNAF is underwater
@@ -851,15 +830,15 @@
                do_reco=True,
                write_dqm=True,
                tape_node="T1_US_FNAL_MSS",
                disk_node="T1_US_FNAL_Disk",
                alca_producers=["EcalUncalZElectron", "EcalUncalWElectron", "HcalCalIterativePhiSym",
                                "HcalCalIsoTrkProducerFilter", "EcalESAlign"],
                dqm_sequences=["@common", "@ecal", "@egamma", "@L1TEgamma"],
-               physics_skims=["ZElectron","WElectron", "EXOMONOPOLE", "EXODisappTrk", "IsoPhotonEB", "LogError", "LogErrorMonitor"],
+               physics_skims=["ZElectron", "WElectron", "EGMJME", "EXOMONOPOLE", "EXODisappTrk", "IsoPhotonEB", "LogError", "LogErrorMonitor"],
                scenario=ppScenario)
 
 DATASETS = ["Tau"]
 
 for dataset in DATASETS:
     addDataset(tier0Config, dataset,
                do_reco=True,
@@ -923,23 +902,14 @@
 
 for dataset in DATASETS:
     addDataset(tier0Config, dataset,
                do_reco=False,
                raw_to_disk=False,
                scenario=ppScenario)
 
-DATASETS = ["CosmicsForEventDisplay"]
-
-for dataset in DATASETS:
-    addDataset(tier0Config, dataset,
-               do_reco=False,
-               raw_to_disk=False,
-               write_miniaod=False,
-               scenario=cosmicsScenario)
-
 DATASETS = ["L1Accept", "L1Accepts"]
 
 for dataset in DATASETS:
     addDataset(tier0Config, dataset,
                do_reco=False,
                write_dqm=False,
                write_aod=True,
@@ -1099,15 +1069,15 @@
                do_reco=True,
                raw_to_disk=True,
                write_reco=False,
                write_dqm=True,
                write_miniaod=True,
                write_aod=True,
                dqm_sequences=["@common", "@ecal", "@jetmet", "@L1TMon", "@hcal", "@L1TEgamma"],
-               alca_producers=["TkAlMinBias"],
+               alca_producers=["TkAlMinBias", "TkAlV0s"],
                physics_skims=["LogError", "LogErrorMonitor"],
                disk_node="T1_IT_CNAF_Disk",
                tape_node="T1_IT_CNAF_MSS",
                scenario=ppScenario)
 
 DATASETS = ["SpecialHLTPhysics", "SpecialHLTPhysics0", "SpecialHLTPhysics1",
             "SpecialHLTPhysics2", "SpecialHLTPhysics3", "SpecialHLTPhysics4",
@@ -1250,15 +1220,19 @@
 
 DATASETS += ["SpecialZeroBias", "SpecialZeroBias0", "SpecialZeroBias1", 
 	     "SpecialZeroBias2", "SpecialZeroBias3", "SpecialZeroBias4", 
 	     "SpecialZeroBias5", "SpecialZeroBias6", "SpecialZeroBias7",
 	     "SpecialZeroBias8", "SpecialZeroBias9", "SpecialZeroBias10",
 	     "SpecialZeroBias11", "SpecialZeroBias12", "SpecialZeroBias13",
 	     "SpecialZeroBias14", "SpecialZeroBias15", "SpecialZeroBias16",
-	     "SpecialZeroBias17", "SpecialZeroBias18", "SpecialZeroBias19"]
+	     "SpecialZeroBias17", "SpecialZeroBias18", "SpecialZeroBias19",
+	     "SpecialZeroBias20", "SpecialZeroBias21", "SpecialZeroBias22",
+	     "SpecialZeroBias23", "SpecialZeroBias24", "SpecialZeroBias25",
+	     "SpecialZeroBias26", "SpecialZeroBias27", "SpecialZeroBias28",
+	     "SpecialZeroBias29", "SpecialZeroBias30", "SpecialZeroBias31"]
 
 DATASETS += ["PPRefZeroBias0", "PPRefZeroBias1", "PPRefZeroBias2",
              "PPRefZeroBias3", "PPRefZeroBias4", "PPRefZeroBias5", "PPRefZeroBias6",
              "PPRefZeroBias7", "PPRefZeroBias8", "PPRefZeroBias9", "PPRefZeroBias10",
              "PPRefZeroBias11", "PPRefZeroBias12", "PPRefZeroBias13", "PPRefZeroBias14",
              "PPRefZeroBias15", "PPRefZeroBias16", "PPRefZeroBias17", "PPRefZeroBias18",
              "PPRefZeroBias19"]
@@ -1266,15 +1240,16 @@
 for dataset in DATASETS:
     addDataset(tier0Config, dataset,
                do_reco=True,
                raw_to_disk=True,
                write_reco=False,
                write_dqm=True,
                dqm_sequences=["@commonSiStripZeroBias", "@ecal", "@hcal", "@muon", "@jetmet", "@ctpps"],
-               alca_producers=["SiStripCalZeroBias", "TkAlMinBias", "SiStripCalMinBias", "HcalCalIsolatedBunchSelector"],
+               alca_producers=["SiStripCalZeroBias", "TkAlMinBias", "SiStripCalMinBias", "LumiPixelsMinBias",
+                               "HcalCalIsolatedBunchSelector"],
                physics_skims=["LogError", "LogErrorMonitor"],
                siteWhitelist = ["T2_CH_CERN_P5", "T2_CH_CERN"],
                timePerEvent=3.5,
                sizePerEvent=1500,
                tape_node="T1_ES_PIC_MSS",
                disk_node="T1_ES_PIC_Disk",
                scenario=ppScenario)
@@ -1298,20 +1273,25 @@
                disk_node="T2_CH_CERN",
                scenario=ppScenario)
 
 ########################################################
 ### Parking and Scouting PDs                         ###
 ########################################################
 
+DATASETS = ["L1Scouting"]
+for dataset in DATASETS:
+    addDataset(tier0Config, dataset,
+               do_reco=False)
+
 DATASETS = ["ScoutingPFRun3"]
 for dataset in DATASETS:
     addDataset(tier0Config, dataset,
                do_reco=False,
-               tape_node="T1_UK_RAL_MSS",
-               disk_node="T1_UK_RAL_Disk",
+               tape_node="T1_US_FNAL_MSS",
+               disk_node="T1_US_FNAL_Disk",
                scenario=ppScenario)
 
 DATASETS = ["ParkingDoubleElectronLowMass","ParkingDoubleElectronLowMass0"]
 for dataset in DATASETS:
     addDataset(tier0Config, dataset,
                do_reco=True,
                write_dqm=True,
@@ -1393,299 +1373,67 @@
                write_reco=False, write_aod=False, write_miniaod=False,
                write_nanoaod=False,
                write_dqm=True,
                alca_producers=["PPSCalMaxTracks"],
                dqm_sequences=["@none"],
                scenario=alcaPPSScenario)
 
-#####################
-### HI TESTS 2022 ###
-#####################
+######################
+### RAW' TEST 2023 ###
+######################
 
-DATASETS = ["HIHcalNZS"]
+DATASETS = ["CommissioningRawPrime"]
 
 for dataset in DATASETS:
     addDataset(tier0Config, dataset,
                do_reco=True,
-               raw_to_disk=False,
-               aod_to_disk=False,
                write_dqm=True,
-               disk_node="T2_US_Vanderbilt",
-               alca_producers=["HcalCalMinBias"],
+	       write_nanoaod=False,
+               alca_producers=["TkAlMinBias", "SiStripCalMinBias", "HcalCalIsoTrk"],
                dqm_sequences=["@common", "@L1TMon", "@hcal"],
-               scenario=HIhcalnzsScenario)
-
-DATASETS = ["HIHLTPhysics"]
-
-for dataset in DATASETS:
-    addDataset(tier0Config, dataset,
-               do_reco=True,
-               raw_to_disk=False,
-               aod_to_disk=False,
-               write_dqm=True,
-               disk_node="T2_US_Vanderbilt",
-               alca_producers=["TkAlMinBias"],
-               dqm_sequences=["@common"],
-               scenario=hiTestppScenario)
-
-DATASETS = ["HIOnlineMonitor", "HITrackerNZS"]
-
-for dataset in DATASETS:
-    addDataset(tier0Config, dataset,
-               do_reco=False,
-               aod_to_disk=False,
-               raw_to_disk=False,
-               disk_node="T2_US_Vanderbilt",
-               scenario=hiTestppScenario)
-
-DATASETS = ["HIEmptyBX"]
-
-for dataset in DATASETS:
-    addDataset(tier0Config, dataset,
-               do_reco=True,
-               write_dqm=True,
-               raw_to_disk=False,
-               aod_to_disk=False,
-               disk_node="T2_US_Vanderbilt",
-               dqm_sequences=["@common"],
-               scenario=hiTestppScenario)
-
-DATASETS = ["HITestRaw0", "HITestRaw1", "HITestRaw2", "HITestRaw3", "HITestRaw4", "HITestRaw5",
-            "HITestRaw6", "HITestRaw7", "HITestRaw8", "HITestRaw9", "HITestRaw10", "HITestRaw11",
-            "HITestRaw12", "HITestRaw13", "HITestRaw14", "HITestRaw15", "HITestRaw16", "HITestRaw17",
-            "HITestRaw18", "HITestRaw19", "HITestRaw20", "HITestRaw21", "HITestRaw22", "HITestRaw23"]
-
-for dataset in DATASETS:
-    addDataset(tier0Config, dataset,
-               do_reco=True,
-               raw_to_disk=False,
-               aod_to_disk=False,
-               write_dqm=True,
-               disk_node="T2_US_Vanderbilt",
-               alca_producers=["SiStripCalZeroBias", "SiStripCalMinBias","TkAlMinBias",
-                               "HcalCalIsolatedBunchSelector", "HcalCalIterativePhiSym","HcalCalMinBias",
-                               "TkAlJpsiMuMu", "TkAlUpsilonMuMu","TkAlZMuMu","TkAlMuonIsolated"],
-               dqm_sequences=["@commonSiStripZeroBias", "@ecal", "@hcal", "@muon", "@jetmet"],
-               scenario=hiTestppScenario)
-
-
-DATASETS = ["HIForward0"]
-
-for dataset in DATASETS:
-    addDataset(tier0Config, dataset,
-               do_reco=True,
-               #reco_delay=defaultRecoTimeout*100,
-               timePerEvent=1,
-               raw_to_disk=False,
-               aod_to_disk=True,
-               write_dqm=True,
-               disk_node="T2_US_Vanderbilt",
-               alca_producers=["EcalUncalZElectron", "EcalUncalWElectron", "EcalESAlign", "MuAlCalIsolatedMu", 
-                               "TkAlDiMuonAndVertex", "HcalCalHO", "HcalCalIsoTrkProducerFilter", "HcalCalHBHEMuonProducerFilter",
-                               "SiStripCalZeroBias", "SiStripCalMinBias","TkAlMinBias",
-                               "HcalCalIsolatedBunchSelector", "HcalCalIterativePhiSym","HcalCalMinBias",
-                               "TkAlJpsiMuMu", "TkAlUpsilonMuMu","TkAlZMuMu","TkAlMuonIsolated"],
-               dqm_sequences=["@commonSiStripZeroBias", "@ecal", "@hcal", "@muon", "@jetmet", "@egamma"],
-               scenario=hiForwardScenario)
-    
-
-DATASETS = ["HIForward1", "HIForward2",
-            "HIForward3", "HIForward4", "HIForward5",
-            "HIForward6", "HIForward7", "HIForward8",
-            "HIForward9", "HIForward10", "HIForward11",
-            "HIForward12", "HIForward13", "HIForward14",
-            "HIForward15", "HIForward16", "HIForward17",
-            "HIForward18", "HIForward19"]
-
-for dataset in DATASETS:
-    addDataset(tier0Config, dataset,
-               do_reco=True,
-               #reco_delay=defaultRecoTimeout*100,
-               timePerEvent=1,
-               raw_to_disk=False,
-               aod_to_disk=True,
-               write_dqm=True,
-               disk_node="T2_US_Vanderbilt",
-               alca_producers=["EcalUncalZElectron", "EcalUncalWElectron", "EcalESAlign", "MuAlCalIsolatedMu", 
-                               "TkAlDiMuonAndVertex", "HcalCalHO", "HcalCalIsoTrkProducerFilter", "HcalCalHBHEMuonProducerFilter",
-                               "SiStripCalZeroBias", "HcalCalIsolatedBunchSelector", "HcalCalIterativePhiSym","HcalCalMinBias",
-                               "TkAlJpsiMuMu", "TkAlUpsilonMuMu","TkAlZMuMu","TkAlMuonIsolated"],
-               dqm_sequences=["@commonSiStripZeroBias", "@ecal", "@hcal", "@muon", "@jetmet", "@egamma"],
-               scenario=hiForwardScenario)
-
-DATASETS = ["HIMinimumBias0"]
-
-for dataset in DATASETS:
-    addDataset(tier0Config, dataset,
-               do_reco=True,
-               raw_to_disk=False,
-               write_dqm=True,
-               disk_node="T2_US_Vanderbilt",
-               alca_producers=["SiStripCalZeroBias", "SiStripCalMinBias", "TkAlMinBias"],
-               dqm_sequences=["@commonSiStripZeroBias"],
-               scenario=hiTestppScenario)
-    
-DATASETS = ["HIMinimumBias1", "HIMinimumBias2", "HIMinimumBias3", 
-            "HIMinimumBias4", "HIMinimumBias5", "HIMinimumBias6", "HIMinimumBias7",
-            "HIMinimumBias8", "HIMinimumBias9", "HIMinimumBias10", "HIMinimumBias11",
-            "HIMinimumBias12", "HIMinimumBias13", "HIMinimumBias14", "HIMinimumBias15",
-            "HIMinimumBias16", "HIMinimumBias17", "HIMinimumBias18", "HIMinimumBias19"]
-
-for dataset in DATASETS:
-    addDataset(tier0Config, dataset,
-               do_reco=True,
-               raw_to_disk=False,
-               write_dqm=True,
-               disk_node="T2_US_Vanderbilt",
-               alca_producers=["SiStripCalZeroBias"],
-               dqm_sequences=["@commonSiStripZeroBias"],
-               scenario=hiTestppScenario)
-
-DATASETS = ["HIEphemeralHLTPhysics"]
-
-for dataset in DATASETS:
-    addDataset(tier0Config, dataset,
-               do_reco=True,
-               raw_to_disk=False,
-               write_dqm=True,
-               disk_node="T2_US_Vanderbilt",
-               dqm_sequences=["@commonSiStripZeroBias"],
-               scenario=hiTestppScenario)
-
-DATASETS = ["HIEphemeralZeroBias0", "HIEphemeralZeroBias1"]
-
-for dataset in DATASETS:
-    addDataset(tier0Config, dataset,
-               do_reco=True,
-               raw_to_disk=False,
-               write_dqm=True,
-               timePerEvent=1,
-               disk_node="T2_US_Vanderbilt",
-               dqm_sequences=["@commonSiStripZeroBias"],
-               scenario=hiTestppScenario)
-
-DATASETS = ["HITestRawPrime0", "HITestRawPrime1", "HITestRawPrime2", "HITestRawPrime3", "HITestRawPrime4",
-            "HITestRawPrime5", "HITestRawPrime6", "HITestRawPrime7", "HITestRawPrime8", "HITestRawPrime9",
-            "HITestRawPrime10", "HITestRawPrime11", "HITestRawPrime12", "HITestRawPrime13", "HITestRawPrime14",
-            "HITestRawPrime15", "HITestRawPrime16", "HITestRawPrime17", "HITestRawPrime18", "HITestRawPrime19",
-            "HITestRawPrime20", "HITestRawPrime21", "HITestRawPrime22", "HITestRawPrime23"]
-
-
-for dataset in DATASETS:
-    addDataset(tier0Config, dataset,
-               do_reco=True,
-               raw_to_disk=False,
-               aod_to_disk=True,
-               write_dqm=True,
-               siteWhitelist = ["T2_CH_CERN"],
-               maxMemoryperCore=2500,
-               disk_node="T2_US_Vanderbilt",
-               alca_producers=["EcalUncalZElectron", "EcalUncalWElectron", "EcalESAlign", "MuAlCalIsolatedMu", 
-                               "TkAlDiMuonAndVertex", "HcalCalHO", "HcalCalIsoTrkProducerFilter", "HcalCalHBHEMuonProducerFilter",
-                               "SiStripCalZeroBias", "SiStripCalMinBias","TkAlMinBias",
-                               "HcalCalIsolatedBunchSelector", "HcalCalIterativePhiSym","HcalCalMinBias",
-                               "TkAlJpsiMuMu", "TkAlUpsilonMuMu","TkAlZMuMu","TkAlMuonIsolated"],
-               dqm_sequences=["@commonSiStripZeroBias", "@ecal", "@hcal", "@muon", "@jetmet", "@egamma"],
-               physics_skims=["PbPbEMu", "PbPbZEE", "PbPbZMM", "LogError", "LogErrorMonitor"],
-               scenario=hiRawPrimeScenario)
-    
-DATASETS = ["HIPhysicsRawPrime0"]
-
-for dataset in DATASETS:
-    addDataset(tier0Config, dataset,
-               do_reco=True,
-               raw_to_disk=False,
-               aod_to_disk=True,
-               write_dqm=True,
-               timePerEvent=3,
-               siteWhitelist = ["T2_CH_CERN"],
-               maxMemoryperCore=2500,
-               disk_node="T2_US_Vanderbilt",
-               alca_producers=["EcalUncalZElectron", "EcalUncalWElectron", "EcalESAlign", "MuAlCalIsolatedMu", 
-                               "TkAlDiMuonAndVertex", "HcalCalHO", "HcalCalIsoTrkProducerFilter", "HcalCalHBHEMuonProducerFilter",
-                               "SiStripCalZeroBias", "SiStripCalMinBias","TkAlMinBias", "HcalCalIsolatedBunchSelector", "HcalCalIterativePhiSym","HcalCalMinBias",
-                               "TkAlJpsiMuMu", "TkAlUpsilonMuMu","TkAlZMuMu","TkAlMuonIsolated"],
-               dqm_sequences=["@commonSiStripZeroBias", "@ecal", "@hcal", "@muon", "@jetmet", "@egamma"],
-               physics_skims=["PbPbEMu", "PbPbZEE", "PbPbZMM", "LogError", "LogErrorMonitor"],
-               scenario=hiRawPrimeScenario)
-
-DATASETS = ["HIPhysicsRawPrime1"]
-
-for dataset in DATASETS:
-    addDataset(tier0Config, dataset,
-               do_reco=True,
-               raw_to_disk=False,
-               aod_to_disk=True,
-               write_dqm=True,
-               timePerEvent=3,
-               siteWhitelist = ["T2_CH_CERN"],
-               maxMemoryperCore=2500,
-               disk_node="T2_US_Vanderbilt",
-               alca_producers=["EcalUncalZElectron", "EcalUncalWElectron", "EcalESAlign", "MuAlCalIsolatedMu", 
-                               "TkAlDiMuonAndVertex", "HcalCalHO", "HcalCalIsoTrkProducerFilter", "HcalCalHBHEMuonProducerFilter",
-                               "SiStripCalZeroBias", "HcalCalIsolatedBunchSelector", "HcalCalIterativePhiSym","HcalCalMinBias",
-                               "TkAlJpsiMuMu", "TkAlUpsilonMuMu","TkAlZMuMu","TkAlMuonIsolated"],
-               dqm_sequences=["@commonSiStripZeroBias", "@ecal", "@hcal", "@muon", "@jetmet", "@egamma"],
-               physics_skims=["PbPbEMu", "PbPbZEE", "PbPbZMM", "LogError", "LogErrorMonitor"],
-               scenario=hiRawPrimeScenario)
-    
-
-DATASETS = ["HIPhysicsRawPrime2", "HIPhysicsRawPrime3", "HIPhysicsRawPrime4",
-            "HIPhysicsRawPrime5", "HIPhysicsRawPrime6", "HIPhysicsRawPrime7", "HIPhysicsRawPrime8", "HIPhysicsRawPrime9",
-            "HIPhysicsRawPrime10", "HIPhysicsRawPrime11", "HIPhysicsRawPrime12", "HIPhysicsRawPrime13", "HIPhysicsRawPrime14",
-            "HIPhysicsRawPrime15", "HIPhysicsRawPrime16", "HIPhysicsRawPrime17", "HIPhysicsRawPrime18", "HIPhysicsRawPrime19",
-            "HIPhysicsRawPrime20", "HIPhysicsRawPrime21", "HIPhysicsRawPrime22", "HIPhysicsRawPrime23", "HIPhysicsRawPrime24",
-            "HIPhysicsRawPrime25", "HIPhysicsRawPrime26", "HIPhysicsRawPrime27", "HIPhysicsRawPrime28", "HIPhysicsRawPrime29",
-            "HIPhysicsRawPrime30", "HIPhysicsRawPrime31"]
-
-for dataset in DATASETS:
-    addDataset(tier0Config, dataset,
-               do_reco=True,
-               raw_to_disk=False,
-               aod_to_disk=False,
-               timePerEvent=3,
-               write_dqm=False,
-               disk_node="T2_US_Vanderbilt",
-               alca_producers=["EcalUncalZElectron", "EcalUncalWElectron", "EcalESAlign", "MuAlCalIsolatedMu", 
-                               "TkAlDiMuonAndVertex", "HcalCalHO", "HcalCalIsoTrkProducerFilter", "HcalCalHBHEMuonProducerFilter",
-                               "SiStripCalZeroBias", "HcalCalIsolatedBunchSelector", "HcalCalIterativePhiSym","HcalCalMinBias",
-                               "TkAlJpsiMuMu", "TkAlUpsilonMuMu","TkAlZMuMu","TkAlMuonIsolated"],
-               dqm_sequences=["@none"],
-               physics_skims=["PbPbEMu", "PbPbZEE", "PbPbZMM", "LogError", "LogErrorMonitor"],
+               physics_skims=["EcalActivity", "LogError", "LogErrorMonitor"],
+               timePerEvent=12,
+               sizePerEvent=4000,
                scenario=hiRawPrimeScenario)
 
-DATASETS = ["HIZeroBias0", "HIZeroBias1", "HIZeroBias2"]
+######################
+###    DAQ TEST    ###
+######################
+
+DATASETS = ["D01", "D02", "D03", "D04", "D05", "D06", "D07", "D08", "D09", "D10",
+	   "D11", "D12", "D13", "D14", "D15", "D16", "D17", "D18", "D19", "D20",
+	   "D21", "D22", "D23", "D24", "D25", "D26", "D27", "D28", "D29", "D30",
+	   "D31", "D32", "D33", "D34", "D35", "D36", "D37", "D38", "Parking"]
 
 for dataset in DATASETS:
     addDataset(tier0Config, dataset,
-               do_reco=True,
-               write_dqm=True,
-               raw_to_disk=False,
-               aod_to_disk=True,
-               disk_node="T2_US_Vanderbilt",
-               dqm_sequences=["@commonSiStripZeroBias", "@ecal", "@hcal", "@muon", "@jetmet", "@egamma"],
-               alca_producers=["SiStripCalZeroBias", "TkAlMinBias", "SiStripCalMinBias"],
-               timePerEvent=1,
-               scenario=hiForwardScenario)
+               do_reco=False,
+               archival_node=None,
+               tape_node=None,
+               disk_node="T0_CH_CERN_Disk",
+               dataset_lifetime=15*24*3600,
+               scenario=ppScenario)
 
 #######################
 ### ignored streams ###
 #######################
 
 ignoreStream(tier0Config, "Error")
 ignoreStream(tier0Config, "HLTMON")
 ignoreStream(tier0Config, "EventDisplay")
-ignoreStream(tier0Config, "HIEventDisplay")
 ignoreStream(tier0Config, "DQM")
 ignoreStream(tier0Config, "DQMEventDisplay")
 ignoreStream(tier0Config, "LookArea")
 ignoreStream(tier0Config, "DQMOffline")
 ignoreStream(tier0Config, "streamHLTRates")
 ignoreStream(tier0Config, "streamL1Rates")
 ignoreStream(tier0Config, "streamDQMRates")
+ignoreStream(tier0Config, "DQMPPSRandom")
+ignoreStream(tier0Config, "L1ScoutingSelection")
+
 
 ###################################
 ### currently inactive settings ###
 ###################################
 
 ##ignoreStream(tier0Config, "Express")
 ##addRegistrationConfig(tier0Config, "UserStreamExample1",
```

### Comparing `t0-4.0.6rc0/etc/HIReplayOfflineConfiguration.py` & `t0-4.0.7rc0/src/python/T0Tools/etc/ReplayOfflineConfiguration.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,46 +4,50 @@
 """
 from __future__ import print_function
 
 from T0.RunConfig.Tier0Config import addDataset
 from T0.RunConfig.Tier0Config import createTier0Config
 from T0.RunConfig.Tier0Config import setAcquisitionEra
 from T0.RunConfig.Tier0Config import setDefaultScramArch
+from T0.RunConfig.Tier0Config import setScramArch
 from T0.RunConfig.Tier0Config import setBaseRequestPriority
 from T0.RunConfig.Tier0Config import setBackfill
 from T0.RunConfig.Tier0Config import setBulkDataType
 from T0.RunConfig.Tier0Config import setProcessingSite
 from T0.RunConfig.Tier0Config import setDQMDataTier
 from T0.RunConfig.Tier0Config import setDQMUploadUrl
 from T0.RunConfig.Tier0Config import setPromptCalibrationConfig
 from T0.RunConfig.Tier0Config import setConfigVersion
 from T0.RunConfig.Tier0Config import ignoreStream
 from T0.RunConfig.Tier0Config import specifyStreams
 from T0.RunConfig.Tier0Config import addRepackConfig
 from T0.RunConfig.Tier0Config import addExpressConfig
 from T0.RunConfig.Tier0Config import setInjectRuns
+from T0.RunConfig.Tier0Config import setInjectLimit
 from T0.RunConfig.Tier0Config import setStreamerPNN
 from T0.RunConfig.Tier0Config import setEnableUniqueWorkflowName
 from T0.RunConfig.Tier0Config import addSiteConfig
 from T0.RunConfig.Tier0Config import setStorageSite
+from T0.RunConfig.Tier0Config import setExtraStreamDatasetMap
 
 # Create the Tier0 configuration object
 tier0Config = createTier0Config()
 
 # Set the verstion configuration (not used at the moment)
 setConfigVersion(tier0Config, "replace with real version")
 
 # Set run number to replay
-# 352929 - 2022 pp at 900 GeV
-# 355189 - 2022 cosmics
-# 355559 - 2022 pp at 13.6 TeV (1h long, 300 bunches)
-# 356005 - 2022 pp at 13.6 TeV (1h long, 600 bunches - ALL detectors included)
-# 359060 - 2022 cosmics - Oberved failures in Express (https://cms-talk.web.cern.ch/t/paused-jobs-for-express-run359045-streamexpress/15232)
-# 361694:361699,361779 - 2022 HI dry-run test runs
-setInjectRuns(tier0Config, [375820])
+# 369998 - Collisions 2023 - 1800b - 1h long - ALL components in
+# 379070 - Cosmics 3.8T 2024 - 3h long - ALL components in
+# 378993 - 2024 13.6TeV Collisions run - 12b - 1h long - ALL components in
+
+setInjectRuns(tier0Config, [369998, 379070, 378993])
+
+# Use this in order to limit the number of lumisections to process
+#setInjectLimit(tier0Config, 10)
 
 # Settings up sites
 processingSite = "T2_CH_CERN"
 storageSite = "T0_CH_CERN_Disk"
 streamerPNN = "T0_CH_CERN_Disk"
 
 addSiteConfig(tier0Config, "T0_CH_CERN_Disk",
@@ -59,18 +63,18 @@
 # Set global parameters:
 #  Acquisition era
 #  BaseRequestPriority
 #  Backfill mode
 #  Data type
 #  Processing site (where jobs run)
 #  PhEDEx locations
-setAcquisitionEra(tier0Config, "Tier0_HIREPLAY_2023")
+setAcquisitionEra(tier0Config, "Tier0_REPLAY_2024")
 setBaseRequestPriority(tier0Config, 260000)
 setBackfill(tier0Config, 1)
-setBulkDataType(tier0Config, "hidata")
+setBulkDataType(tier0Config, "data")
 setProcessingSite(tier0Config, processingSite)
 setStreamerPNN(tier0Config, streamerPNN)
 setStorageSite(tier0Config, storageSite)
 
 # Override for DQM data tier
 setDQMDataTier(tier0Config, "DQMIO")
 
@@ -102,45 +106,45 @@
 #
 # { 'acqEra': {'Era1': Value1, 'Era2': Value2},
 #   'maxRun': {100000: Value3, 200000: Value4},
 #   'default': Value5 }
 
 # Defaults for CMSSW version
 defaultCMSSWVersion = {
-    'default': "CMSSW_13_2_6_patch2"
+    'default': "CMSSW_14_0_6_patch1"
 }
 
 # Configure ScramArch
-setDefaultScramArch(tier0Config, "el8_amd64_gcc11")
+setDefaultScramArch(tier0Config, "el8_amd64_gcc12")
+setScramArch(tier0Config, "CMSSW_12_4_9", "el8_amd64_gcc10")
+setScramArch(tier0Config, "CMSSW_12_3_0", "cs8_amd64_gcc10")
+setScramArch(tier0Config, "CMSSW_13_0_9", "el8_amd64_gcc11")
 
 # Configure scenarios
-ppScenario = "ppEra_Run3_2023"
+ppScenario = "ppEra_Run3"
+ppScenarioB0T = "ppEra_Run3"
 cosmicsScenario = "cosmicsEra_Run3"
 hcalnzsScenario = "hcalnzsEra_Run3"
-HIhcalnzsScenario = "hcalnzsEra_Run3_pp_on_PbPb"
-hiScenario = "ppEra_Run3_pp_on_PbPb_2023"
 alcaTrackingOnlyScenario = "trackingOnlyEra_Run3"
-HIalcaTrackingOnlyScenario = "trackingOnlyEra_Run3_pp_on_PbPb"
 alcaTestEnableScenario = "AlCaTestEnable"
 alcaLumiPixelsScenario = "AlCaLumiPixels_Run3"
 alcaPPSScenario = "AlCaPPS_Run3"
 hiTestppScenario = "ppEra_Run3_pp_on_PbPb_2023"
 hiRawPrimeScenario = "ppEra_Run3_pp_on_PbPb_approxSiStripClusters_2023"
-hiForwardScenario = "ppEra_Run3_2023_repacked"
 
 # Procesing version number replays
 # Taking Replay processing ID from the last 8 digits of the DeploymentID
 dt = int(open("/data/tier0/DeploymentID.txt","r").read()[4:])
 defaultProcVersion = dt
 expressProcVersion = dt
 alcarawProcVersion = dt
 
 # Defaults for GlobalTag
-expressGlobalTag = "132X_dataRun3_Express_v4"
-promptrecoGlobalTag = "132X_dataRun3_Prompt_v4"
+expressGlobalTag = "140X_dataRun3_Express_v3"
+promptrecoGlobalTag = "140X_dataRun3_Prompt_v2"
 
 # Mandatory for CondDBv2
 globalTagConnect = "frontier://PromptProd/CMS_CONDITIONS"
 
 # Multicore settings
 numberOfCores = 8
 
@@ -156,14 +160,20 @@
     "CMSSW_12_6_3" : "CMSSW_12_6_4"
 }
 
 expressVersionOverride = {
     "CMSSW_12_6_3" : "CMSSW_12_6_4"
 }
 
+# Additional Stream-Dataset mapping
+setExtraStreamDatasetMap(tier0Config,{
+                                        "L1Scouting": {"Dataset":"L1Scouting"}
+                                    }
+                         )
+
 #set default repack settings for bulk streams
 addRepackConfig(tier0Config, "Default",
                 proc_ver=defaultProcVersion,
                 maxSizeSingleLumi=24 * 1024 * 1024 * 1024,
                 maxSizeMultiLumi=8 * 1024 * 1024 * 1024,
                 minInputSize=2.1 * 1024 * 1024 * 1024,
                 maxInputSize=4 * 1024 * 1024 * 1024,
@@ -172,17 +182,22 @@
                 maxInputEvents=3 * 1000 * 1000,
                 maxInputFiles=1000,
                 maxLatency=2 * 3600,
                 blockCloseDelay=1200,
                 maxMemory=2000,
                 versionOverride=repackVersionOverride)
 
+addRepackConfig(tier0Config, "ScoutingPF",
+                proc_ver=1, # Should remain 1. Changing it can cause several issues.
+                dataTier="HLTSCOUT",
+                versionOverride=repackVersionOverride)
+
 addDataset(tier0Config, "Default",
            do_reco=False,
-           write_reco=False, write_aod=True, write_miniaod=True, write_nanoaod=False, write_dqm=False,
+           write_reco=False, write_aod=True, write_miniaod=True, write_nanoaod=True, write_dqm=False,
            reco_delay=defaultRecoTimeout,
            reco_delay_offset=defaultRecoLockTimeout,
            reco_split=defaultRecoSplitting,
            proc_version=defaultProcVersion,
            cmssw_version=defaultCMSSWVersion,
            multicore=numberOfCores,
            global_tag=promptrecoGlobalTag,
@@ -205,17 +220,19 @@
 addExpressConfig(tier0Config, "Express",
                  scenario=ppScenario,
                  diskNode="T0_CH_CERN_Disk",
                  data_tiers=["FEVT"],
                  write_dqm=True,
                  alca_producers=["SiStripPCLHistos", "SiStripCalZeroBias", "SiStripCalMinBias", "SiStripCalMinBiasAAG",
                                  "TkAlMinBias", "SiPixelCalZeroBias", "SiPixelCalSingleMuon", "SiPixelCalSingleMuonTight",
+                                 "TkAlZMuMu",
                                  "PromptCalibProd", "PromptCalibProdSiStrip", "PromptCalibProdSiPixelAli",
                                  "PromptCalibProdSiStripGains", "PromptCalibProdSiStripGainsAAG", "PromptCalibProdSiPixel",
-                                 "PromptCalibProdSiPixelLA", "PromptCalibProdSiStripHitEff", "PromptCalibProdSiPixelAliHG"
+                                 "PromptCalibProdSiPixelLA", "PromptCalibProdSiStripHitEff", "PromptCalibProdSiPixelAliHG",
+                                 "PromptCalibProdSiPixelAliHGComb"
                                 ],
                  dqm_sequences=["@standardDQMExpress"],
                  reco_version=defaultCMSSWVersion,
                  multicore=numberOfCores,
                  global_tag_connect=globalTagConnect,
                  global_tag=expressGlobalTag,
                  proc_ver=expressProcVersion,
@@ -301,15 +318,15 @@
                  maxLatency=1 * 3600,
                  periodicHarvestInterval=24 * 3600,
                  blockCloseDelay=2 * 3600,
                  timePerEvent=4,
                  sizePerEvent=1700,
                  versionOverride=expressVersionOverride,
                  maxMemoryperCore=2000,
-                 dataType="hidata",
+                 dataType="data",
                  dataset_lifetime=14*24*3600,#lifetime for container rules. Default 14 days
                  diskNode="T0_CH_CERN_Disk")
 
 addExpressConfig(tier0Config, "ExpressAlignment",
                  scenario=alcaTrackingOnlyScenario,
                  data_tiers=["ALCARECO"],
                  write_dqm=True,
@@ -382,28 +399,26 @@
                  sizePerEvent=1700,
                  maxMemoryperCore=2000,
                  dataset_lifetime=14*24*3600,#lifetime for container rules. Default 14 days
                  diskNode="T0_CH_CERN_Disk",
                  versionOverride=expressVersionOverride)
 
 #####################
-### HI Tests 2022 ###
+### HI Tests 2018 ###
 #####################
 
 addExpressConfig(tier0Config, "HIExpress",
                  scenario=hiTestppScenario,
                  diskNode="T0_CH_CERN_Disk",
                  data_tiers=["FEVT"],
                  write_dqm=True,
                  alca_producers=["SiStripPCLHistos", "SiStripCalZeroBias", "SiStripCalMinBias", "SiStripCalMinBiasAAG",
-                                 "TkAlMinBias", "SiPixelCalZeroBias","SiPixelCalSingleMuon", "SiPixelCalSingleMuonTight",
-                                 "SiPixelCalSingleMuonLoose",
+                                 "TkAlMinBias", "LumiPixelsMinBias", "SiPixelCalZeroBias",
                                  "PromptCalibProd", "PromptCalibProdSiStrip", "PromptCalibProdSiPixelAli",
-                                 "PromptCalibProdSiStripGains", "PromptCalibProdSiStripGainsAAG", "PromptCalibProdSiPixel",
-                                 "PromptCalibProdSiPixelLA", "PromptCalibProdSiStripHitEff", "PromptCalibProdSiPixelAliHG"
+                                 "PromptCalibProdSiStripGains", "PromptCalibProdSiStripGainsAAG", "PromptCalibProdSiPixel"
                                 ],
                  reco_version=defaultCMSSWVersion,
                  multicore=numberOfCores,
                  global_tag_connect=globalTagConnect,
                  global_tag=expressGlobalTag,
                  proc_ver=expressProcVersion,
                  maxInputRate=23 * 1000,
@@ -415,43 +430,19 @@
                  blockCloseDelay=1200,
                  timePerEvent=4,
                  sizePerEvent=1700,
                  maxMemoryperCore=2000,
                  dataset_lifetime=14*24*3600,#lifetime for container rules. Default 14 days
                  versionOverride=expressVersionOverride)
 
-addExpressConfig(tier0Config, "HIExpressRawPrime",
-                 scenario=hiRawPrimeScenario,
-                 diskNode="T2_CH_CERN",
-                 data_tiers=["FEVT"],
-                 write_dqm=True,
-                 alca_producers=["SiStripCalMinBias", "SiStripCalMinBiasAAG"],
-                 reco_version=defaultCMSSWVersion,
-                 multicore=numberOfCores,
-                 global_tag_connect=globalTagConnect,
-                 global_tag=expressGlobalTag,
-                 proc_ver=expressProcVersion,
-                 maxInputRate=23 * 1000,
-                 maxInputEvents=400,
-                 maxInputSize=2 * 1024 * 1024 * 1024,
-                 maxInputFiles=15,
-                 maxLatency=15 * 23,
-                 periodicHarvestInterval=20 * 60,
-                 blockCloseDelay=1200,
-                 timePerEvent=4,
-                 sizePerEvent=1700,
-                 maxMemoryperCore=2000,
-                 dataset_lifetime=3*30*24*3600,#lifetime for container rules. Default 3 months
-                 versionOverride=expressVersionOverride)
-
 addExpressConfig(tier0Config, "HIExpressAlignment",
-                 scenario=HIalcaTrackingOnlyScenario,
+                 scenario=hiTestppScenario,
                  data_tiers=["ALCARECO", "RAW"],
                  write_dqm=True,
-                 alca_producers=["TkAlMinBias", "PromptCalibProdBeamSpotHP"],
+                 alca_producers=["TkAlMinBias"],
                  dqm_sequences=["@trackingOnlyDQM"],
                  reco_version=defaultCMSSWVersion,
                  raw_to_disk=True,
                  multicore=numberOfCores,
                  global_tag_connect=globalTagConnect,
                  global_tag=expressGlobalTag,
                  proc_ver=expressProcVersion,
@@ -464,39 +455,15 @@
                  blockCloseDelay=2 * 3600,
                  timePerEvent=4,
                  sizePerEvent=1700,
                  versionOverride=expressVersionOverride,
                  maxMemoryperCore=2000,
                  dataset_lifetime=14*24*3600,#lifetime for container rules. Default 14 days
                  diskNode="T0_CH_CERN_Disk")
-
-addExpressConfig(tier0Config, "HIHLTMonitor",
-                 scenario=hiTestppScenario,
-                 diskNode="T2_CH_CERN",
-                 data_tiers=["FEVTHLTALL"],
-                 write_dqm=True,
-                 alca_producers=[],
-                 dqm_sequences=["@HLTMon"],
-                 reco_version=defaultCMSSWVersion,
-                 multicore=numberOfCores,
-                 global_tag_connect=globalTagConnect,
-                 global_tag=expressGlobalTag,
-                 proc_ver=expressProcVersion,
-                 maxInputRate=23 * 1000,
-                 maxInputEvents=400,
-                 maxInputSize=2 * 1024 * 1024 * 1024,
-                 maxInputFiles=15,
-                 maxLatency=15 * 23,
-                 periodicHarvestInterval=20 * 60,
-                 blockCloseDelay=1200,
-                 timePerEvent=4,
-                 sizePerEvent=1700,
-                 dataset_lifetime=14*24*3600,#lifetime for container rules. Default 14 days
-                 versionOverride=expressVersionOverride)
-
+                 
 ###################################
 ### Standard Physics PDs (2022) ###
 ###################################
 
 DATASETS = ["BTagMu"]
 
 for dataset in DATASETS:
@@ -511,14 +478,15 @@
 
 for dataset in DATASETS:
     addDataset(tier0Config, dataset,
                do_reco=True,
                write_reco=False,
                write_aod=True,
                write_miniaod=False,
+               write_nanoaod=False,
                write_dqm=True,
                alca_producers=["SiStripCalCosmics", "SiPixelCalCosmics", "TkAlCosmics0T", "MuAlGlobalCosmics", "SiStripCalCosmicsNano"],
                physics_skims=["CosmicSP", "CosmicTP", "LogError", "LogErrorMonitor"],
                timePerEvent=0.5,
                sizePerEvent=155,
                scenario=cosmicsScenario)
 
@@ -557,56 +525,45 @@
                timePerEvent=1,
                scenario=ppScenario)
 
 DATASETS = ["ReservedDoubleMuonLowMass"]
 
 for dataset in DATASETS:
     addDataset(tier0Config, dataset,
-               do_reco=False,
-               scenario=ppScenario)
-
-DATASETS = ["ParkingSingleMuon","ParkingSingleMuon0"]
-
-for dataset in DATASETS:
-    addDataset(tier0Config, dataset,
                do_reco=True,
                scenario=ppScenario)
 
-DATASETS = ["ParkingSingleMuon1","ParkingSingleMuon2"]
+DATASETS = ["ParkingSingleMuon","ParkingSingleMuon0","ParkingSingleMuon1","ParkingSingleMuon2"]
 
 for dataset in DATASETS:
     addDataset(tier0Config, dataset,
                do_reco=True,
-               aod_to_disk=False,
-               archival_node=None,
                scenario=ppScenario)
 
-DATASETS = ["ParkingDoubleMuonLowMass0"]
+DATASETS = ["ParkingDoubleMuonLowMass0","ParkingDoubleMuonLowMass1","ParkingDoubleMuonLowMass2",
+            "ParkingDoubleMuonLowMass3"]
 
 for dataset in DATASETS:
     addDataset(tier0Config, dataset,
                do_reco=True,
                write_dqm=True,
                dqm_sequences=["@common", "@muon", "@heavyFlavor"],
                alca_producers=["TkAlJpsiMuMu", "TkAlUpsilonMuMu"],
-               archival_node=None,
+               tape_node=None,
                scenario=ppScenario)
 
-DATASETS = ["ParkingDoubleMuonLowMass1","ParkingDoubleMuonLowMass2",
-            "ParkingDoubleMuonLowMass3","ParkingDoubleMuonLowMass4","ParkingDoubleMuonLowMass5",
+DATASETS = ["ParkingDoubleMuonLowMass4","ParkingDoubleMuonLowMass5",
             "ParkingDoubleMuonLowMass6","ParkingDoubleMuonLowMass7"]
 
 for dataset in DATASETS:
     addDataset(tier0Config, dataset,
                do_reco=True,
                write_dqm=True,
-               aod_to_disk=False,
                dqm_sequences=["@common", "@muon", "@heavyFlavor"],
                alca_producers=["TkAlJpsiMuMu", "TkAlUpsilonMuMu"],
-               archival_node=None,
                scenario=ppScenario)
 
 DATASETS = ["MuonShower"]
 
 for dataset in DATASETS:
     addDataset(tier0Config, dataset,
                do_reco=True,
@@ -625,39 +582,35 @@
                write_reco=False,
                write_aod=True,
                write_miniaod=True,
                write_nanoaod=True,
                physics_skims=["EXOCSCCluster"],
                scenario=ppScenario)
 
-DATASETS = ["ParkingHH", "ParkingVBF0",
-            "ParkingVBF1", "ParkingVBF2", "ParkingVBF3",
-            "ParkingVBF4", "ParkingVBF5", "ParkingVBF6",
-            "ParkingVBF7"]
-
+DATASETS = [ "ParkingLLP" ]
 for dataset in DATASETS:
     addDataset(tier0Config, dataset,
                do_reco=True,
                write_dqm=True,
                aod_to_disk=False,
-               dqm_sequences=["@common"],
-               archival_node=None,
+               dqm_sequences=["@common", "@jetmet"],
                scenario=ppScenario)
-    
-DATASETS = ["ParkingLLP"]
 
+DATASETS = ["ParkingHH", "ParkingVBF0",
+            "ParkingVBF1", "ParkingVBF2", "ParkingVBF3",
+            "ParkingVBF4", "ParkingVBF5", "ParkingVBF6",
+            "ParkingVBF7"]
 for dataset in DATASETS:
     addDataset(tier0Config, dataset,
                do_reco=True,
                write_dqm=True,
                aod_to_disk=False,
-               dqm_sequences=["@common", "@jetmet"],
-               archival_node=None,
+               dqm_sequences=["@common"],
                scenario=ppScenario)
-    
+
 DATASETS = ["EmptyBX"]
 
 for dataset in DATASETS:
     addDataset(tier0Config, dataset,
                do_reco=True,
                write_dqm=True,
                dqm_sequences=["@common"],
@@ -676,15 +629,15 @@
 
 for dataset in DATASETS:
     addDataset(tier0Config, dataset,
                do_reco=True,
                write_dqm=True,
                alca_producers=["HcalCalIsoTrkProducerFilter", "TkAlJetHT", "HcalCalNoise"],
                dqm_sequences=["@common", "@jetmet", "@L1TMon", "@hcal"],
-               physics_skims=["EXOHighMET", "EXODelayedJetMET", "JetHTJetPlusHOFilter", "EXODisappTrk", "LogError", "LogErrorMonitor"],
+               physics_skims=["EXOHighMET", "EXODelayedJetMET", "JetHTJetPlusHOFilter", "EXODisappTrk", "EXOSoftDisplacedVertices", "TeVJet", "LogError", "LogErrorMonitor"],
                timePerEvent=5.7,  # copied from JetHT - should be checked
                sizePerEvent=2250, # copied from JetHT - should be checked
                scenario=ppScenario)
 
 DATASETS = ["PPRefHardProbes0", "PPRefHardProbes1", "PPRefHardProbes2"]
 
 for dataset in DATASETS:
@@ -728,36 +681,33 @@
     addDataset(tier0Config, dataset,
                do_reco=True,
                write_dqm=True,
                dqm_sequences=["@common"],
                physics_skims=["TopMuEG", "LogError", "LogErrorMonitor"],
                scenario=ppScenario)
 
-DATASETS = ["Muon", "Muon0"]
+DATASETS = ["Muon", "Muon0", "Muon1"]
 
 for dataset in DATASETS:
     addDataset(tier0Config, dataset,
                do_reco=True,
-               write_reco=False,
                write_dqm=True,
                alca_producers=["TkAlMuonIsolated", "HcalCalIterativePhiSym", "MuAlCalIsolatedMu",
                                "HcalCalHO", "HcalCalHBHEMuonProducerFilter",
                                "SiPixelCalSingleMuonLoose", "SiPixelCalSingleMuonTight",
                                "TkAlZMuMu", "TkAlDiMuonAndVertex"],
                dqm_sequences=["@common", "@muon", "@lumi", "@L1TMuon", "@jetmet"],
-               physics_skims=["ZMu", "EXODisappTrk", "LogError", "LogErrorMonitor", "EXOCSCCluster", "EXODisappMuon"],
+               physics_skims=["MUOJME", "ZMu", "EXODisappTrk", "EXOCSCCluster", "EXODisappMuon", "LogError", "LogErrorMonitor"],
                scenario=ppScenario)
 
-DATASETS = ["Muon1"]
-DATASETS += ["PPRefSingleMuon0", "PPRefSingleMuon1", "PPRefSingleMuon2"]
+DATASETS = ["PPRefSingleMuon0", "PPRefSingleMuon1", "PPRefSingleMuon2"]
 
 for dataset in DATASETS:
     addDataset(tier0Config, dataset,
                do_reco=True,
-               write_reco=False,
                write_dqm=True,
                alca_producers=["TkAlMuonIsolated", "HcalCalIterativePhiSym", "MuAlCalIsolatedMu",
                                "HcalCalHO", "HcalCalHBHEMuonProducerFilter",
                                "SiPixelCalSingleMuonLoose", "SiPixelCalSingleMuonTight",
                                "TkAlZMuMu", "TkAlDiMuonAndVertex"],
                dqm_sequences=["@common", "@muon", "@lumi", "@L1TMuon", "@jetmet"],
                physics_skims=["ZMu", "EXODisappTrk", "LogError", "LogErrorMonitor", "EXOCSCCluster", "EXODisappMuon"],
@@ -766,14 +716,16 @@
 DATASETS = ["PPRefDoubleMuon0", "PPRefDoubleMuon1", "PPRefDoubleMuon2", "PPRefDoubleMuon3"]
 
 for dataset in DATASETS:
     addDataset(tier0Config, dataset,
                do_reco=True,
                write_reco=False,
                write_dqm=True,
+               tape_node="T1_US_FNAL_MSS",
+               disk_node="T1_US_FNAL_Disk",
                alca_producers=["TkAlZMuMu", "TkAlDiMuonAndVertex", "TkAlJpsiMuMu", "TkAlUpsilonMuMu"],
                dqm_sequences=["@common", "@muon", "@lumi", "@L1TMuon", "@jetmet"],
                physics_skims=["ZMu", "EXODisappTrk", "LogError", "LogErrorMonitor", "EXOCSCCluster", "EXODisappMuon"],
                scenario=ppScenario)
 
 DATASETS = ["NoBPTX"]
 
@@ -783,15 +735,14 @@
                write_reco=False,
                write_dqm=True,
                alca_producers=["TkAlCosmicsInCollisions"],
                dqm_sequences=["@common"],
                physics_skims=["EXONoBPTXSkim", "LogError", "LogErrorMonitor"],
                scenario=ppScenario)
 
-
 DATASETS = ["SingleMuon"]
 
 for dataset in DATASETS:
     addDataset(tier0Config, dataset,
                do_reco=True,
                write_dqm=True,
                alca_producers=["TkAlMuonIsolated", "HcalCalIterativePhiSym", "MuAlCalIsolatedMu",
@@ -806,15 +757,15 @@
 for dataset in DATASETS:
     addDataset(tier0Config, dataset,
                do_reco=True,
                write_dqm=True,
                alca_producers=["EcalUncalZElectron", "EcalUncalWElectron", "HcalCalIterativePhiSym",
                                "HcalCalIsoTrkProducerFilter", "EcalESAlign"],
                dqm_sequences=["@common", "@ecal", "@egamma", "@L1TEgamma"],
-               physics_skims=["ZElectron","WElectron", "EXOMONOPOLE", "EXODisappTrk", "IsoPhotonEB", "LogError", "LogErrorMonitor"],
+               physics_skims=["ZElectron","WElectron", "EGMJME", "EXOMONOPOLE", "EXODisappTrk", "IsoPhotonEB", "LogError", "LogErrorMonitor"],
                scenario=ppScenario)
 
 DATASETS = ["Tau"]
 
 for dataset in DATASETS:
     addDataset(tier0Config, dataset,
                do_reco=True,
@@ -828,14 +779,16 @@
 #############################################
 
 DATASETS = ["Commissioning"]
 
 DATASETS += ["Commissioning1", "Commissioning2", "Commissioning3", "Commissioning4",
              "CommissioningMuons", "CommissioningEGamma", "CommissioningTaus", "CommissioningSingleJet", "CommissioningDoubleJet"]
 
+DATASETS += ["CommissioningZDC"]
+
 for dataset in DATASETS:
     addDataset(tier0Config, dataset,
                do_reco=True,
                write_dqm=True,
                alca_producers=["TkAlMinBias", "SiStripCalMinBias", "HcalCalIsoTrk"],
                dqm_sequences=["@common", "@L1TMon", "@hcal"],
                physics_skims=["EcalActivity", "LogError", "LogErrorMonitor"],
@@ -872,60 +825,39 @@
 
 for dataset in DATASETS:
     addDataset(tier0Config, dataset,
                do_reco=False,
                raw_to_disk=False,
                scenario=ppScenario)
 
-DATASETS = ["CosmicsForEventDisplay"]
-
-for dataset in DATASETS:
-    addDataset(tier0Config, dataset,
-               do_reco=False,
-               raw_to_disk=False,
-               write_miniaod=False,
-               scenario=cosmicsScenario)
-
 DATASETS = ["L1Accept", "L1Accepts"]
 
 for dataset in DATASETS:
     addDataset(tier0Config, dataset,
                do_reco=False,
                write_dqm=False,
                write_aod=True,
                write_miniaod=True,
                write_reco=False,
                dqm_sequences=["@common"],
                scenario=ppScenario)
 
-#############################################
-### MiniDAQ                               ###
-#############################################
-
-DATASETS = ["MiniDaq"]
-for dataset in DATASETS:
-    addDataset(tier0Config, dataset,
-               raw_to_disk=True,
-               dataset_lifetime=6*30*24*3600)
-
 ###########################
 ### special AlcaRaw PDs ###
 ###########################
 
 DATASETS = ["AlCaLumiPixels", "AlCaLumiPixels0", "AlCaLumiPixels1", "AlCaLumiPixels2", "AlCaLumiPixels3",
             "AlCaLumiPixels4", "AlCaLumiPixels5", "AlCaLumiPixels6", "AlCaLumiPixels7",
             "AlCaLumiPixels8", "AlCaLumiPixels9", "AlCaLumiPixels10", "AlCaLumiPixels11",
             "AlCaLumiPixels12"]
 
 for dataset in DATASETS:
     addDataset(tier0Config, dataset,
                do_reco=True,
                write_reco=False, write_aod=False, write_miniaod=False, write_nanoaod=False, write_dqm=True,
-               disk_node=None,
-               tape_node=None,
                reco_split=alcarawSplitting,
                proc_version=alcarawProcVersion,
                alca_producers=["AlCaPCCZeroBias"],
                dqm_sequences=["@common"],
                timePerEvent=0.02,
                sizePerEvent=38,
                scenario=alcaLumiPixelsScenario)
@@ -962,14 +894,15 @@
             "AlCaLumiPixelsCountsExpress8", "AlCaLumiPixelsCountsExpress9", "AlCaLumiPixelsCountsExpress10", "AlCaLumiPixelsCountsExpress11",
             "AlCaLumiPixelsCountsExpress12", "AlCaLumiPixelsCountsExpress"]
 
 for dataset in DATASETS:
     addDataset(tier0Config, dataset,
                do_reco=False,
                write_reco=False, write_aod=False, write_miniaod=False, write_dqm=False,
+               write_nanoaod=False,
                disk_node=None,
                tape_node=None,
                reco_split=alcarawSplitting,
                proc_version=alcarawProcVersion,
                timePerEvent=0.02,
                sizePerEvent=38,
                scenario=alcaLumiPixelsScenario)
@@ -978,14 +911,15 @@
 
 for dataset in DATASETS:
     addDataset(tier0Config, dataset,
                do_reco=False,
                write_reco=False, write_aod=False, write_miniaod=False, write_dqm=False,
                write_nanoaod=False,
                raw_to_disk=True,
+               disk_node=None,
                tape_node=None,
                reco_split=alcarawSplitting,
                proc_version=alcarawProcVersion,
                timePerEvent=0.02,
                sizePerEvent=38,
                scenario=alcaLumiPixelsScenario)
 
@@ -993,14 +927,15 @@
 
 for dataset in DATASETS:
     addDataset(tier0Config, dataset,
                do_reco=False,
                write_reco=False, write_aod=False, write_miniaod=False, write_dqm=False,
                write_nanoaod=False,
                raw_to_disk=True,
+               disk_node=None,
                tape_node=None,
                reco_split=alcarawSplitting,
                proc_version=alcarawProcVersion,
                timePerEvent=0.02,
                sizePerEvent=38,
                scenario=alcaLumiPixelsScenario)
 
@@ -1013,15 +948,14 @@
                scenario=ppScenario)
 
 DATASETS = ["AlCaP0"]
 
 for dataset in DATASETS:
     addDataset(tier0Config, dataset,
                do_reco=False,
-               raw_to_disk=True,
                alca_producers=["EcalCalPi0Calib", "EcalCalEtaCalib"],
                scenario=ppScenario)
 
 ########################################################
 ### HLTPhysics PDs                                   ###
 ########################################################
 
@@ -1038,15 +972,15 @@
                do_reco=True,
                raw_to_disk=True,
                write_reco=False,
                write_dqm=True,
                write_miniaod=True,
                write_aod=True,
                dqm_sequences=["@common", "@ecal", "@jetmet", "@L1TMon", "@hcal", "@L1TEgamma"],
-               alca_producers=["TkAlMinBias"],
+               alca_producers=["TkAlMinBias", "TkAlV0s"],
                physics_skims=["LogError", "LogErrorMonitor"],
                scenario=ppScenario)
 
 DATASETS = ["SpecialHLTPhysics", "SpecialHLTPhysics0", "SpecialHLTPhysics1",
             "SpecialHLTPhysics2", "SpecialHLTPhysics3", "SpecialHLTPhysics4",
             "SpecialHLTPhysics5", "SpecialHLTPhysics6", "SpecialHLTPhysics7",
             "SpecialHLTPhysics8", "SpecialHLTPhysics9", "SpecialHLTPhysics10",
@@ -1079,21 +1013,18 @@
 
 for dataset in DATASETS:
     addDataset(tier0Config, dataset,
                do_reco=True,
                raw_to_disk=True,
                dqm_sequences=["@none"],
                write_dqm=False,
-               write_aod=False,
-               archival_node=None,
-               siteWhitelist = ["T2_CH_CERN_P5", "T2_CH_CERN"],
                scenario=ppScenario)
 
 ########################################################
-### SpecialRandom PDs                                  ###
+### SpecialRandom PDs                                ###
 ########################################################
 
 DATASETS = ["SpecialRandom0", "SpecialRandom1", "SpecialRandom2",
             "SpecialRandom3", "SpecialRandom4", "SpecialRandom5",
             "SpecialRandom6", "SpecialRandom7", "SpecialRandom8",
             "SpecialRandom9", "SpecialRandom10", "SpecialRandom11",
             "SpecialRandom12", "SpecialRandom13", "SpecialRandom14",
@@ -1183,15 +1114,19 @@
 
 DATASETS += ["SpecialZeroBias", "SpecialZeroBias0", "SpecialZeroBias1", 
 	     "SpecialZeroBias2", "SpecialZeroBias3", "SpecialZeroBias4", 
 	     "SpecialZeroBias5", "SpecialZeroBias6", "SpecialZeroBias7",
 	     "SpecialZeroBias8", "SpecialZeroBias9", "SpecialZeroBias10",
 	     "SpecialZeroBias11", "SpecialZeroBias12", "SpecialZeroBias13",
 	     "SpecialZeroBias14", "SpecialZeroBias15", "SpecialZeroBias16",
-	     "SpecialZeroBias17", "SpecialZeroBias18", "SpecialZeroBias19"]
+	     "SpecialZeroBias17", "SpecialZeroBias18", "SpecialZeroBias19",
+	     "SpecialZeroBias20", "SpecialZeroBias21", "SpecialZeroBias22",
+	     "SpecialZeroBias23", "SpecialZeroBias24", "SpecialZeroBias25",
+	     "SpecialZeroBias26", "SpecialZeroBias27", "SpecialZeroBias28",
+	     "SpecialZeroBias29", "SpecialZeroBias30", "SpecialZeroBias31"]
 
 DATASETS += ["PPRefZeroBias0", "PPRefZeroBias1", "PPRefZeroBias2",
              "PPRefZeroBias3", "PPRefZeroBias4", "PPRefZeroBias5", "PPRefZeroBias6",
              "PPRefZeroBias7", "PPRefZeroBias8", "PPRefZeroBias9", "PPRefZeroBias10",
              "PPRefZeroBias11", "PPRefZeroBias12", "PPRefZeroBias13", "PPRefZeroBias14",
              "PPRefZeroBias15", "PPRefZeroBias16", "PPRefZeroBias17", "PPRefZeroBias18",
              "PPRefZeroBias19"]
@@ -1199,15 +1134,16 @@
 for dataset in DATASETS:
     addDataset(tier0Config, dataset,
                do_reco=True,
                raw_to_disk=True,
                write_reco=False,
                write_dqm=True,
                dqm_sequences=["@commonSiStripZeroBias", "@ecal", "@hcal", "@muon", "@jetmet", "@ctpps"],
-               alca_producers=["SiStripCalZeroBias", "TkAlMinBias", "SiStripCalMinBias", "HcalCalIsolatedBunchSelector"],
+               alca_producers=["SiStripCalZeroBias", "TkAlMinBias", "SiStripCalMinBias", "LumiPixelsMinBias",
+                               "HcalCalIsolatedBunchSelector"],
                physics_skims=["LogError", "LogErrorMonitor"],
                timePerEvent=3.5,
                sizePerEvent=1500,
                scenario=ppScenario)
 
 DATASETS = ["EphemeralZeroBias0", "EphemeralZeroBias1", "EphemeralZeroBias2", "EphemeralZeroBias3",
             "EphemeralZeroBias4", "EphemeralZeroBias5", "EphemeralZeroBias6", "EphemeralZeroBias7",
@@ -1223,39 +1159,35 @@
                write_dqm=False,
                scenario=ppScenario)
 
 ########################################################
 ### Parking and Scouting PDs                         ###
 ########################################################
 
-DATASETS = ["ScoutingPFRun3"]
+DATASETS = ["L1Scouting"]
 for dataset in DATASETS:
     addDataset(tier0Config, dataset,
-               do_reco=False,
-               scenario=ppScenario)
+               do_reco=False)
 
-DATASETS = ["ParkingDoubleElectronLowMass","ParkingDoubleElectronLowMass0"]
+DATASETS = ["ScoutingPFRun3"]
 for dataset in DATASETS:
     addDataset(tier0Config, dataset,
-               do_reco=True,
-               write_dqm=True,
-               dqm_sequences=["@common"],
-               archival_node=None,
+               do_reco=False,
                scenario=ppScenario)
 
-DATASETS = ["ParkingDoubleElectronLowMass1","ParkingDoubleElectronLowMass2",
-            "ParkingDoubleElectronLowMass3","ParkingDoubleElectronLowMass4","ParkingDoubleElectronLowMass5"]
+DATASETS = ["ParkingDoubleElectronLowMass0","ParkingDoubleElectronLowMass1","ParkingDoubleElectronLowMass2",
+            "ParkingDoubleElectronLowMass3","ParkingDoubleElectronLowMass4","ParkingDoubleElectronLowMass5",
+            "ParkingDoubleElectronLowMass"]
 
 for dataset in DATASETS:
     addDataset(tier0Config, dataset,
                do_reco=True,
                write_dqm=True,
                dqm_sequences=["@common"],
-               aod_to_disk=False,
-               siteWhitelist = ["T2_CH_CERN_P5", "T2_CH_CERN"],
+               tape_node=None,
                scenario=ppScenario)
 
 DATASETS = ["RPCMonitor"]
 
 for dataset in DATASETS:
     addDataset(tier0Config, dataset,
                do_reco=False,
@@ -1306,225 +1238,47 @@
                write_reco=False, write_aod=False, write_miniaod=False,
                write_nanoaod=False,
                write_dqm=True,
                alca_producers=["PPSCalMaxTracks"],
                dqm_sequences=["@none"],
                scenario=alcaPPSScenario)
 
-#####################
-### HI TESTS 2022 ###
-#####################
+######################
+### RAW' TEST 2023 ###
+######################
 
-DATASETS = ["HIHcalNZS"]
+DATASETS = ["CommissioningRawPrime"]
 
 for dataset in DATASETS:
     addDataset(tier0Config, dataset,
                do_reco=True,
-               raw_to_disk=False,
-               aod_to_disk=False,
                write_dqm=True,
-               alca_producers=["HcalCalMinBias"],
+	       write_nanoaod=False,
+               alca_producers=["TkAlMinBias", "SiStripCalMinBias", "HcalCalIsoTrk"],
                dqm_sequences=["@common", "@L1TMon", "@hcal"],
-               scenario=HIhcalnzsScenario)
-
-DATASETS = ["HIHLTPhysics"]
-
-for dataset in DATASETS:
-    addDataset(tier0Config, dataset,
-               do_reco=True,
-               raw_to_disk=False,
-               aod_to_disk=False,
-               write_dqm=True,
-               alca_producers=["TkAlMinBias"],
-               dqm_sequences=["@common"],
-               scenario=hiTestppScenario)
-
-DATASETS = ["HIOnlineMonitor", "HITrackerNZS"]
-
-for dataset in DATASETS:
-    addDataset(tier0Config, dataset,
-               do_reco=False,
-               aod_to_disk=False,
-               raw_to_disk=False,
-               scenario=hiTestppScenario)
-
-DATASETS = ["HIEmptyBX"]
-
-for dataset in DATASETS:
-    addDataset(tier0Config, dataset,
-               do_reco=True,
-               write_dqm=True,
-               raw_to_disk=False,
-               aod_to_disk=False,
-               dqm_sequences=["@common"],
-               scenario=hiTestppScenario)
-
-DATASETS = ["HITestRaw0", "HITestRaw1", "HITestRaw2", "HITestRaw3", "HITestRaw4", "HITestRaw5",
-            "HITestRaw6", "HITestRaw7", "HITestRaw8", "HITestRaw9", "HITestRaw10", "HITestRaw11",
-            "HITestRaw12", "HITestRaw13", "HITestRaw14", "HITestRaw15", "HITestRaw16", "HITestRaw17",
-            "HITestRaw18", "HITestRaw19", "HITestRaw20", "HITestRaw21", "HITestRaw22", "HITestRaw23"]
-
-for dataset in DATASETS:
-    addDataset(tier0Config, dataset,
-               do_reco=True,
-               raw_to_disk=False,
-               aod_to_disk=False,
-               write_dqm=True,
-               alca_producers=["SiStripCalZeroBias", "SiStripCalMinBias","TkAlMinBias",
-                               "HcalCalIsolatedBunchSelector", "HcalCalIterativePhiSym","HcalCalMinBias",
-                               "TkAlJpsiMuMu", "TkAlUpsilonMuMu","TkAlZMuMu","TkAlMuonIsolated"],
-               dqm_sequences=["@commonSiStripZeroBias", "@ecal", "@hcal", "@muon", "@jetmet"],
-               scenario=hiTestppScenario)
-DATASETS = ["HIForward0", "HIForward1", "HIForward2",
-	    "HIForward3", "HIForward4", "HIForward5",
-            "HIForward6", "HIForward7", "HIForward8",
-            "HIForward9", "HIForward10", "HIForward11",
-            "HIForward12", "HIForward13", "HIForward14",
-            "HIForward15", "HIForward16", "HIForward17",
-            "HIForward18", "HIForward19"]
-for dataset in DATASETS:
-    addDataset(tier0Config, dataset,
-               do_reco=True,
-               timePerEvent=1,
-               raw_to_disk=False,
-               aod_to_disk=True,
-               write_dqm=True,
-               alca_producers=["EcalUncalZElectron", "EcalUncalWElectron", "EcalESAlign", "MuAlCalIsolatedMu", 
-                               "TkAlDiMuonAndVertex", "HcalCalHO", "HcalCalIsoTrkProducerFilter", "HcalCalHBHEMuonProducerFilter",
-                               "SiStripCalZeroBias", "SiStripCalMinBias","TkAlMinBias",
-                               "HcalCalIsolatedBunchSelector", "HcalCalIterativePhiSym","HcalCalMinBias",
-                               "TkAlJpsiMuMu", "TkAlUpsilonMuMu","TkAlZMuMu","TkAlMuonIsolated"],
-               dqm_sequences=["@commonSiStripZeroBias", "@ecal", "@hcal", "@muon", "@jetmet", "@egamma"],
-               scenario=hiForwardScenario)
-    
-DATASETS = ["HIMinimumBias0", "HIMinimumBias1", "HIMinimumBias2", "HIMinimumBias3", 
-            "HIMinimumBias4", "HIMinimumBias5", "HIMinimumBias6", "HIMinimumBias7",
-            "HIMinimumBias8", "HIMinimumBias9", "HIMinimumBias10", "HIMinimumBias11",
-            "HIMinimumBias12", "HIMinimumBias13", "HIMinimumBias14", "HIMinimumBias15",
-            "HIMinimumBias16", "HIMinimumBias17", "HIMinimumBias18", "HIMinimumBias19"]
-
-for dataset in DATASETS:
-    addDataset(tier0Config, dataset,
-               do_reco=True,
-               raw_to_disk=False,
-               write_dqm=True,
-               alca_producers=["SiStripCalZeroBias", "SiStripCalMinBias", "TkAlMinBias"],
-               dqm_sequences=["@commonSiStripZeroBias"],
-               scenario=hiTestppScenario)
-
-DATASETS = ["HIEphemeralHLTPhysics"]
-
-for dataset in DATASETS:
-    addDataset(tier0Config, dataset,
-               do_reco=True,
-               raw_to_disk=False,
-               write_dqm=True,
-               disk_node="T2_US_Vanderbilt",
-               dqm_sequences=["@commonSiStripZeroBias"],
-               scenario=hiTestppScenario)
-
-DATASETS = ["HIEphemeralZeroBias0", "HIEphemeralZeroBias1"]
-
-for dataset in DATASETS:
-    addDataset(tier0Config, dataset,
-               do_reco=True,
-               raw_to_disk=False,
-               write_dqm=True,
-               timePerEvent=1,
-               disk_node="T2_US_Vanderbilt",
-               dqm_sequences=["@commonSiStripZeroBias"],
-               scenario=hiTestppScenario)
-
-DATASETS = ["HITestRawPrime0", "HITestRawPrime1", "HITestRawPrime2", "HITestRawPrime3", "HITestRawPrime4",
-            "HITestRawPrime5", "HITestRawPrime6", "HITestRawPrime7", "HITestRawPrime8", "HITestRawPrime9",
-            "HITestRawPrime10", "HITestRawPrime11", "HITestRawPrime12", "HITestRawPrime13", "HITestRawPrime14",
-            "HITestRawPrime15", "HITestRawPrime16", "HITestRawPrime17", "HITestRawPrime18", "HITestRawPrime19",
-            "HITestRawPrime20", "HITestRawPrime21", "HITestRawPrime22", "HITestRawPrime23"]
-
-DATASETS += ["HIPhysicsRawPrime0", "HIPhysicsRawPrime1"]
-
-for dataset in DATASETS:
-    addDataset(tier0Config, dataset,
-               do_reco=True,
-               raw_to_disk=False,
-               aod_to_disk=True,
-               write_dqm=True,
-               timePerEvent=3,
-               siteWhitelist = ["T2_CH_CERN"],
-               maxMemoryperCore=2500,
-               disk_node="T2_US_Vanderbilt",
-               alca_producers=["EcalUncalZElectron", "EcalUncalWElectron", "EcalESAlign", "MuAlCalIsolatedMu", 
-                               "TkAlDiMuonAndVertex", "HcalCalHO", "HcalCalIsoTrkProducerFilter", "HcalCalHBHEMuonProducerFilter",
-                               "SiStripCalZeroBias", "SiStripCalMinBias","TkAlMinBias",
-                               "HcalCalIsolatedBunchSelector", "HcalCalIterativePhiSym","HcalCalMinBias",
-                               "TkAlJpsiMuMu", "TkAlUpsilonMuMu","TkAlZMuMu","TkAlMuonIsolated"],
-               dqm_sequences=["@commonSiStripZeroBias", "@ecal", "@hcal", "@muon", "@jetmet", "@egamma"],
-               physics_skims=["PbPbEMu", "PbPbZEE", "PbPbZMM", "LogError", "LogErrorMonitor"],
-               scenario=hiRawPrimeScenario)
-
-DATASETS = ["HIPhysicsRawPrime2", "HIPhysicsRawPrime3", "HIPhysicsRawPrime4",
-            "HIPhysicsRawPrime5", "HIPhysicsRawPrime6", "HIPhysicsRawPrime7", "HIPhysicsRawPrime8", "HIPhysicsRawPrime9",
-            "HIPhysicsRawPrime10", "HIPhysicsRawPrime11", "HIPhysicsRawPrime12", "HIPhysicsRawPrime13", "HIPhysicsRawPrime14",
-            "HIPhysicsRawPrime15", "HIPhysicsRawPrime16", "HIPhysicsRawPrime17", "HIPhysicsRawPrime18", "HIPhysicsRawPrime19",
-            "HIPhysicsRawPrime20", "HIPhysicsRawPrime21", "HIPhysicsRawPrime22", "HIPhysicsRawPrime23", "HIPhysicsRawPrime24",
-            "HIPhysicsRawPrime25", "HIPhysicsRawPrime26", "HIPhysicsRawPrime27", "HIPhysicsRawPrime28", "HIPhysicsRawPrime29",
-            "HIPhysicsRawPrime30", "HIPhysicsRawPrime31"]
-
-for dataset in DATASETS:
-    addDataset(tier0Config, dataset,
-               do_reco=True,
-               raw_to_disk=False,
-               aod_to_disk=False,
-               write_dqm=False,
-               timePerEvent=3,
-               alca_producers=["EcalUncalZElectron", "EcalUncalWElectron", "EcalESAlign", "MuAlCalIsolatedMu", 
-                               "TkAlDiMuonAndVertex", "HcalCalHO", "HcalCalIsoTrkProducerFilter", "HcalCalHBHEMuonProducerFilter",
-                               "SiStripCalZeroBias", "SiStripCalMinBias","TkAlMinBias",
-                               "HcalCalIsolatedBunchSelector", "HcalCalIterativePhiSym","HcalCalMinBias",
-                               "TkAlJpsiMuMu", "TkAlUpsilonMuMu","TkAlZMuMu","TkAlMuonIsolated"],
-               dqm_sequences=["@none"],
-               physics_skims=["PbPbEMu", "PbPbZEE", "PbPbZMM", "LogError", "LogErrorMonitor"],
+               physics_skims=["EcalActivity", "LogError", "LogErrorMonitor"],
+               timePerEvent=12,
+               sizePerEvent=4000,
                scenario=hiRawPrimeScenario)
 
-DATASETS = ["HIZeroBias0", "HIZeroBias1", "HIZeroBias2"]
-
-for dataset in DATASETS:
-    addDataset(tier0Config, dataset,
-               do_reco=True,
-               write_dqm=True,
-               raw_to_disk=False,
-               aod_to_disk=True,
-               dqm_sequences=["@commonSiStripZeroBias", "@ecal", "@hcal", "@muon", "@jetmet", "@egamma"],
-               alca_producers=["SiStripCalZeroBias", "TkAlMinBias", "SiStripCalMinBias"],
-               timePerEvent=1,
-               scenario=hiForwardScenario)
-
 #######################
 ### ignored streams ###
 #######################
-#specifyStreams(tier0Config, ["HIForward0", "HIForward1", "HIForward2",
-#            "HIForward3", "HIForward4", "HIForward5",
-#            "HIForward6", "HIForward7", "HIForward8",
-#            "HIForward9", "HIForward10", "HIForward11",
-#            "HIForward12", "HIForward13", "HIForward14",
-#            "HIForward15", "HIForward16", "HIForward17",
-#            "HIForward18", "HIForward19"])
 
 ignoreStream(tier0Config, "Error")
 ignoreStream(tier0Config, "HLTMON")
 ignoreStream(tier0Config, "EventDisplay")
-ignoreStream(tier0Config, "HIEventDisplay")
 ignoreStream(tier0Config, "DQM")
 ignoreStream(tier0Config, "DQMEventDisplay")
 ignoreStream(tier0Config, "LookArea")
 ignoreStream(tier0Config, "DQMOffline")
 ignoreStream(tier0Config, "streamHLTRates")
 ignoreStream(tier0Config, "streamL1Rates")
 ignoreStream(tier0Config, "streamDQMRates")
-
+ignoreStream(tier0Config, "DQMPPSRandom")
 ###################################
 ### currently inactive settings ###
 ###################################
 
 ##ignoreStream(tier0Config, "Express")
 ##addRegistrationConfig(tier0Config, "UserStreamExample1",
 ##                      primds="ExamplePrimDS1",
```

### Comparing `t0-4.0.6rc0/etc/Tier0Config.py` & `t0-4.0.7rc0/src/python/T0Tools/etc/Tier0Config.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/pyproject.toml` & `t0-4.0.7rc0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "T0"
-version = "4.0.6.pre"
+version = "4.0.7.pre"
 description = "This package contains the code that is involved in the Tier 0 agent when its deployed"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 keywords = ["T0"]
 authors = [
   {email = "Dirk.Hufnagel@cern.ch"},
```

### Comparing `t0-4.0.6rc0/src/python/T0/ConditionUpload/ConditionUploadAPI.py` & `t0-4.0.7rc0/src/python/T0/ConditionUpload/ConditionUploadAPI.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/ConditionUpload/upload.py` & `t0-4.0.7rc0/src/python/T0/ConditionUpload/upload.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/JobSplitting/AlcaHarvest.py` & `t0-4.0.7rc0/src/python/T0/JobSplitting/AlcaHarvest.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/JobSplitting/Condition.py` & `t0-4.0.7rc0/src/python/T0/JobSplitting/Condition.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/JobSplitting/Express.py` & `t0-4.0.7rc0/src/python/T0/JobSplitting/Express.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/JobSplitting/ExpressMerge.py` & `t0-4.0.7rc0/src/python/T0/JobSplitting/ExpressMerge.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/JobSplitting/Repack.py` & `t0-4.0.7rc0/src/python/T0/JobSplitting/Repack.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/JobSplitting/RepackMerge.py` & `t0-4.0.7rc0/src/python/T0/JobSplitting/RepackMerge.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/RunConfig/RunConfigAPI.py` & `t0-4.0.7rc0/src/python/T0/RunConfig/RunConfigAPI.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/RunConfig/Tier0Config.py` & `t0-4.0.7rc0/src/python/T0/RunConfig/Tier0Config.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/RunLumiCloseout/RunLumiCloseoutAPI.py` & `t0-4.0.7rc0/src/python/T0/RunLumiCloseout/RunLumiCloseoutAPI.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/StorageManager/StorageManagerAPI.py` & `t0-4.0.7rc0/src/python/T0/StorageManager/StorageManagerAPI.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/ConditionUpload/CompleteFiles.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/ConditionUpload/CompleteFiles.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/ConditionUpload/FinishPCLforEmptyExpress.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/ConditionUpload/FinishPCLforEmptyExpress.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/ConditionUpload/GetConditions.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/ConditionUpload/GetConditions.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/ConditionUpload/GetRunStopTime.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/ConditionUpload/GetRunStopTime.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/ConditionUpload/IsPromptCalibrationFinished.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/ConditionUpload/IsPromptCalibrationFinished.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/ConditionUpload/MarkPromptCalibrationFinished.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/ConditionUpload/MarkPromptCalibrationFinished.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Create.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Create.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/JobSplitting/InsertPromptCalibrationFile.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/JobSplitting/InsertPromptCalibrationFile.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/JobSplitting/InsertSplitLumis.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/JobSplitting/InsertSplitLumis.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/FindRecoRelease.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/FindRecoRelease.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/FindRecoReleaseDatasets.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/FindRecoReleaseDatasets.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/GetExpressConfig.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/GetExpressConfig.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/GetHLTConfig.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/GetHLTConfig.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/GetPhEDExConfig.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/GetPhEDExConfig.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/GetRecoConfig.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/GetRecoConfig.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/GetRepackConfig.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/GetRepackConfig.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/GetRunInfo.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/GetRunInfo.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/GetStreamDatasetTriggers.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/GetStreamDatasetTriggers.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/GetStreamDatasets.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/GetStreamDatasets.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/GetStreamOnlineVersion.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/GetStreamOnlineVersion.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/GetStreamStyle.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/GetStreamStyle.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertCMSSWVersion.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertCMSSWVersion.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertDatasetScenario.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertDatasetScenario.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertDatasetTrigger.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertDatasetTrigger.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertExpressConfig.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertExpressConfig.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertLumiSection.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertLumiSection.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertPhEDExConfig.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertPhEDExConfig.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertPrimaryDataset.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertPrimaryDataset.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertPromptCalibration.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertPromptCalibration.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertRecoConfig.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertRecoConfig.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertRecoReleaseConfig.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertRecoReleaseConfig.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertRepackConfig.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertRepackConfig.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertRun.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertRun.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertRunStreamDone.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertRunStreamDone.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertSpecialDataset.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertSpecialDataset.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertStorageNode.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertStorageNode.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertStream.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertStream.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertStreamCMSSWVersion.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertStreamCMSSWVersion.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertStreamDataset.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertStreamDataset.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertStreamFileset.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertStreamFileset.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertStreamStyle.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertStreamStyle.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertStreamer.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertStreamer.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertTrigger.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertTrigger.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertWorkflowMonitoring.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/InsertWorkflowMonitoring.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/ReleasePromptReco.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/ReleasePromptReco.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunConfig/UpdateRun.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunConfig/UpdateRun.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/CheckActiveSplitLumis.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/CheckActiveSplitLumis.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/CheckClosedLumis.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/CheckClosedLumis.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/CheckEndOfRunRecords.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/CheckEndOfRunRecords.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/CloseRunStreamFilesets.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/CloseRunStreamFilesets.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/CloseRuns.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/CloseRuns.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/DeleteStreamers.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/DeleteStreamers.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/FinalCloseLumi.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/FinalCloseLumi.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/FindActiveRuns.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/FindActiveRuns.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/FindClosedLumis.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/FindClosedLumis.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/FindClosedRuns.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/FindClosedRuns.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/FindHighContLumi.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/FindHighContLumi.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/FindOpenRuns.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/FindOpenRuns.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/FindStoppedRuns.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/FindStoppedRuns.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/ForceCloseLumi.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/ForceCloseLumi.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/GetClosedLumisForStream.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/GetClosedLumisForStream.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/GetFileCountOnOpenLumis.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/GetFileCountOnOpenLumis.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/GetFilesForStreamLumi.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/GetFilesForStreamLumi.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/GetOpenRunStreamLumicount.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/GetOpenRunStreamLumicount.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/InsertClosedLumi.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/InsertClosedLumi.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/StopRuns.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/RunLumiCloseout/StopRuns.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/SMNotification/GetFinishedStreamers.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/SMNotification/GetFinishedStreamers.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/SMNotification/InsertOfflineFileStatus.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/SMNotification/InsertOfflineFileStatus.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/SMNotification/MarkStreamersFinished.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/SMNotification/MarkStreamersFinished.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/SMNotification/UpdateOfflineFileStatus.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/SMNotification/UpdateOfflineFileStatus.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/StorageManager/GetNewData.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/StorageManager/GetNewData.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/StorageManager/GetRunInfo.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/StorageManager/GetRunInfo.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/StorageManager/GetRunSetup.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/StorageManager/GetRunSetup.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Subscriptions/GetAllFiles.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Subscriptions/GetAllFiles.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Subscriptions/GetAvailableConditionFiles.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Subscriptions/GetAvailableConditionFiles.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Subscriptions/GetAvailableExpressFiles.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Subscriptions/GetAvailableExpressFiles.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Subscriptions/GetAvailableExpressMergeFiles.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Subscriptions/GetAvailableExpressMergeFiles.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Subscriptions/GetAvailableRepackFiles.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Subscriptions/GetAvailableRepackFiles.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Subscriptions/GetAvailableRepackMergeFiles.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Subscriptions/GetAvailableRepackMergeFiles.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Subscriptions/GetLumiHolesForRepack.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Subscriptions/GetLumiHolesForRepack.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Subscriptions/GetLumiHolesForRepackMerge.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Subscriptions/GetLumiHolesForRepackMerge.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Subscriptions/GetUsedLumis.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Subscriptions/GetUsedLumis.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Subscriptions/HaveAvailableFile.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Subscriptions/HaveAvailableFile.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Subscriptions/HaveJobGroup.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Subscriptions/HaveJobGroup.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/T0DataSvc/GetDatasetLocked.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/T0DataSvc/GetDatasetLocked.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/T0DataSvc/GetExpressConfigs.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/T0DataSvc/GetExpressConfigs.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/T0DataSvc/GetNewRun.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/T0DataSvc/GetNewRun.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/T0DataSvc/GetPromptRecoStatus.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/T0DataSvc/GetPromptRecoStatus.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/T0DataSvc/GetRecoConfigs.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/T0DataSvc/GetRecoConfigs.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/T0DataSvc/GetRunStreamDone.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/T0DataSvc/GetRunStreamDone.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/T0DataSvc/GetSkippedStreamers.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/T0DataSvc/GetSkippedStreamers.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/T0DataSvc/InsertDatasetLocked.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/T0DataSvc/InsertDatasetLocked.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/T0DataSvc/InsertExpressConfigs.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/T0DataSvc/InsertExpressConfigs.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/T0DataSvc/InsertNewRun.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/T0DataSvc/InsertNewRun.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/T0DataSvc/InsertRecoConfigs.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/T0DataSvc/InsertRecoConfigs.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/T0DataSvc/InsertRecoLocked.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/T0DataSvc/InsertRecoLocked.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/T0DataSvc/InsertRunDatasetDone.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/T0DataSvc/InsertRunDatasetDone.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/T0DataSvc/InsertRunStreamDone.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/T0DataSvc/InsertRunStreamDone.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/T0DataSvc/InsertSkippedStreamers.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/T0DataSvc/InsertSkippedStreamers.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateDatasetLocked.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateDatasetLocked.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateExpressConfigs.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateExpressConfigs.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateNewRun.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateNewRun.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateRecoConfigs.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateRecoConfigs.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateRecoLocked.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateRecoLocked.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateRunDatasetDone.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateRunDatasetDone.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateRunStreamDone.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateRunStreamDone.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateSkippedStreamers.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/T0DataSvc/UpdateSkippedStreamers.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/FeedStreamers.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/FeedStreamers.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/FindNewExpressRuns.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/FindNewExpressRuns.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/FindNewRunStreams.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/FindNewRunStreams.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/FindNewRuns.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/FindNewRuns.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/GetDeploymentID.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/GetDeploymentID.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/GetExpressReadyRuns.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/GetExpressReadyRuns.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/GetNotClosedOutWorkflows.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/GetNotClosedOutWorkflows.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/GetPromptRecoWorkflowsForMonitoring.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/GetPromptRecoWorkflowsForMonitoring.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/GetRunDatasetDone.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/GetRunDatasetDone.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/GetRunDatasetNew.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/GetRunDatasetNew.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/GetRunDatasetReleased.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/GetRunDatasetReleased.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/GetStreamerWorkflowsForMonitoring.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/GetStreamerWorkflowsForMonitoring.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/MarkCloseoutWorkflowMonitoring.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/MarkCloseoutWorkflowMonitoring.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/MarkTrackedWorkflowMonitoring.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/MarkTrackedWorkflowMonitoring.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/MarkWorkflowsInjected.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/MarkWorkflowsInjected.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/ReleaseExpress.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/ReleaseExpress.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/SetDeploymentID.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/SetDeploymentID.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/UpdateRecoReleaseConfigs.py` & `t0-4.0.7rc0/src/python/T0/WMBS/Oracle/Tier0Feeder/UpdateRecoReleaseConfigs.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0.egg-info/PKG-INFO` & `t0-4.0.7rc0/src/python/T0.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: T0
-Version: 4.0.6rc0
+Version: 4.0.7rc0
 Summary: This package contains the code that is involved in the Tier 0 agent when its deployed
 Author: Dirk Hufnagel
 Author-email: Dirk.Hufnagel@cern.ch
 Maintainer-email: WMCore <ms.unmerged@cern.ch>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
```

### Comparing `t0-4.0.6rc0/src/python/T0.egg-info/SOURCES.txt` & `t0-4.0.7rc0/src/python/T0.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,13 @@
 LICENSE
 MANIFEST.in
 NOTICE
 README.md
 pyproject.toml
 requirements.txt
-bin/00_deploy.sh
-bin/00_deploy_prod.sh
-bin/00_deploy_replay.sh
-bin/00_patches.sh
-bin/00_software.sh
-bin/buildrelease.sh
-bin/cmst0_backlog_wma
-bin/cmst0_late_workflows
-bin/cmst0_long_jobs
-bin/cmst0_paused_jobs
-bin/diagnoseActiveRuns
-bin/forceCloseRuns
-bin/tier0-mod-config
-etc/ContainterConfig.sh
-etc/HIProdOfflineConfiguration.py
-etc/HIReplayOfflineConfiguration.py
-etc/ProdOfflineConfiguration.py
-etc/ReplayOfflineConfiguration.py
-etc/ReplayOfflineConfigurationRun1.py
-etc/SLSAlarmsConfig.py
-etc/Tier0Config.py
-etc/XeXeProdOfflineConfiguration.py
-etc/XeXeReplayOfflineConfiguration.py
 src/python/T0/__init__.py
 src/python/T0.egg-info/PKG-INFO
 src/python/T0.egg-info/SOURCES.txt
 src/python/T0.egg-info/dependency_links.txt
 src/python/T0.egg-info/top_level.txt
 src/python/T0/ConditionUpload/ConditionUploadAPI.py
 src/python/T0/ConditionUpload/__init__.py
@@ -189,8 +166,18 @@
 src/python/T0/WMSpec/StdSpecs/__init__.py
 src/python/T0Component/__init__.py
 src/python/T0Component/Tier0Auditor/Tier0Auditor.py
 src/python/T0Component/Tier0Auditor/Tier0AuditorPoller.py
 src/python/T0Component/Tier0Auditor/__init__.py
 src/python/T0Component/Tier0Feeder/Tier0Feeder.py
 src/python/T0Component/Tier0Feeder/Tier0FeederPoller.py
-src/python/T0Component/Tier0Feeder/__init__.py
+src/python/T0Component/Tier0Feeder/__init__.py
+src/python/T0Tools/bin/cmst0_backlog_wma
+src/python/T0Tools/bin/cmst0_late_workflows
+src/python/T0Tools/bin/cmst0_long_jobs
+src/python/T0Tools/bin/cmst0_paused_jobs
+src/python/T0Tools/bin/diagnoseActiveRuns
+src/python/T0Tools/bin/forceCloseRuns
+src/python/T0Tools/bin/tier0-mod-config
+src/python/T0Tools/etc/ProdOfflineConfiguration.py
+src/python/T0Tools/etc/ReplayOfflineConfiguration.py
+src/python/T0Tools/etc/Tier0Config.py
```

### Comparing `t0-4.0.6rc0/src/python/T0Component/Tier0Auditor/Tier0Auditor.py` & `t0-4.0.7rc0/src/python/T0Component/Tier0Auditor/Tier0Auditor.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0Component/Tier0Auditor/Tier0AuditorPoller.py` & `t0-4.0.7rc0/src/python/T0Component/Tier0Auditor/Tier0AuditorPoller.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0Component/Tier0Feeder/Tier0Feeder.py` & `t0-4.0.7rc0/src/python/T0Component/Tier0Feeder/Tier0Feeder.py`

 * *Files identical despite different names*

### Comparing `t0-4.0.6rc0/src/python/T0Component/Tier0Feeder/Tier0FeederPoller.py` & `t0-4.0.7rc0/src/python/T0Component/Tier0Feeder/Tier0FeederPoller.py`

 * *Files identical despite different names*

