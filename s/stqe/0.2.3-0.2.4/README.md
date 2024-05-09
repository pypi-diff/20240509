# Comparing `tmp/stqe-0.2.3.tar.gz` & `tmp/stqe-0.2.4.tar.gz`

## Comparing `stqe-0.2.3.tar` & `stqe-0.2.4.tar`

### file list

```diff
@@ -1,349 +1,349 @@
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 stqe-0.2.3/.gitlab-ci.yml
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 stqe-0.2.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 stqe-0.2.3/noxfile.py
--rwxr-xr-x   0        0        0      901 2020-02-02 00:00:00.000000 stqe-0.2.3/release.sh
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 stqe-0.2.3/requirements-stable.txt
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/__init__.py
--rw-r--r--   0        0        0    31943 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/stqe_test.py
--rwxr-xr-x   0        0        0     2628 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/stqe_tool.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/conf/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/conf/lvm/__init__.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/conf/lvm/lvm-thinp-basic.conf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/host/__init__.py
--rwxr-xr-x   0        0        0     5759 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/host/atomic_run.py
--rw-r--r--   0        0        0     4902 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/host/beaker.py
--rw-r--r--   0        0        0    21048 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/host/fmf_tools.py
--rw-r--r--   0        0        0     9424 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/host/iscsi.py
--rw-r--r--   0        0        0    12503 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/host/logchecker.py
--rw-r--r--   0        0        0     5007 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/host/lsm.py
--rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/host/lvm.py
--rw-r--r--   0        0        0    41736 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/host/nfs_lock.py
--rw-r--r--   0        0        0     9088 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/host/persistent_vars.py
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/host/restraint.py
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/host/stratis.py
--rw-r--r--   0        0        0    10173 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/host/tc.py
--rw-r--r--   0        0        0     7014 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/host/vdo.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/__init__.py
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/.fmf/version
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/dm/__init__.py
--rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/dm/block_boundary_obedience.py
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/dm/error_block_alignment.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/dm/main.fmf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/hba/__init__.py
--rwxr-xr-x   0        0        0    11145 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/hba/add_new_lun.py
--rwxr-xr-x   0        0        0    13817 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/hba/dev_loss_tmo.py
--rwxr-xr-x   0        0        0     4590 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/hba/io-failover-alternate-interface.py
--rwxr-xr-x   0        0        0     9440 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/hba/io-remove-lun.py
--rwxr-xr-x   0        0        0    34651 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/hba/mp_failover.py
--rwxr-xr-x   0        0        0     8166 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/hba/online_offline.py
--rwxr-xr-x   0        0        0    16563 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/hba/oscilate_port.py
--rwxr-xr-x   0        0        0     3930 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/hba/show_driver_info.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/iscsi/__init__.py
--rwxr-xr-x   0        0        0     8759 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/iscsi/iscsi_params.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/iscsi/main.fmf
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/iscsi/cli/__init__.py
--rwxr-xr-x   0        0        0     1970 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/iscsi/cli/iscsi_local_target.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/iscsi/cli/main.fmf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/iscsi/setup/__init__.py
--rwxr-xr-x   0        0        0     2238 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/iscsi/setup/create_backstore.py
--rwxr-xr-x   0        0        0     2134 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/iscsi/setup/create_fileio_target.py
--rwxr-xr-x   0        0        0     1196 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/iscsi/setup/delete_backstore.py
--rwxr-xr-x   0        0        0      528 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/iscsi/setup/delete_iscsi_target.py
--rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/iscsi/setup/main.fmf
--rwxr-xr-x   0        0        0     2123 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/iscsi/setup/start_multipath.py
--rwxr-xr-x   0        0        0     1782 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/iscsi/setup/stop_multipath.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/__init__.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/main.fmf
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/__init__.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/main.fmf
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/access_group/__init__.py
--rwxr-xr-x   0        0        0     5491 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/access_group/access_group_add.py
--rwxr-xr-x   0        0        0     4290 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/access_group/access_group_create.py
--rwxr-xr-x   0        0        0     1749 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/access_group/access_group_delete.py
--rwxr-xr-x   0        0        0     3355 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/access_group/access_group_remove.py
--rwxr-xr-x   0        0        0     2021 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/access_group/access_group_volumes.py
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/access_group/main.fmf
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/fs/__init__.py
--rwxr-xr-x   0        0        0     4637 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/fs/fs_clone.py
--rwxr-xr-x   0        0        0     4788 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/fs/fs_create.py
--rwxr-xr-x   0        0        0     1396 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/fs/fs_delete.py
--rwxr-xr-x   0        0        0     2815 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/fs/fs_dependants.py
--rwxr-xr-x   0        0        0     4618 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/fs/fs_dependants_rm.py
--rwxr-xr-x   0        0        0     2444 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/fs/fs_export.py
--rwxr-xr-x   0        0        0     4125 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/fs/fs_resize.py
--rwxr-xr-x   0        0        0     4334 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/fs/fs_snap_create.py
--rwxr-xr-x   0        0        0     2123 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/fs/fs_snap_delete.py
--rwxr-xr-x   0        0        0     3031 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/fs/fs_snap_restore.py
--rwxr-xr-x   0        0        0     1425 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/fs/fs_unexport.py
--rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/fs/main.fmf
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/list/__init__.py
--rwxr-xr-x   0        0        0     1902 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/list/access_groups.py
--rwxr-xr-x   0        0        0     1854 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/list/batteries.py
--rwxr-xr-x   0        0        0     1783 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/list/disks.py
--rwxr-xr-x   0        0        0     1803 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/list/exports.py
--rwxr-xr-x   0        0        0     1725 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/list/fs.py
--rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/list/main.fmf
--rwxr-xr-x   0        0        0     1577 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/list/nsf_client_auth.py
--rwxr-xr-x   0        0        0     1513 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/list/plugins.py
--rwxr-xr-x   0        0        0     1783 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/list/pools.py
--rwxr-xr-x   0        0        0     1116 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/list/snapshots.py
--rwxr-xr-x   0        0        0     1513 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/list/systems.py
--rwxr-xr-x   0        0        0     1853 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/list/target_ports.py
--rwxr-xr-x   0        0        0     1846 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/list/volumes.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/local_disk/__init__.py
--rwxr-xr-x   0        0        0     3366 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/local_disk/local_disk_fault_led.py
--rwxr-xr-x   0        0        0     3384 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/local_disk/local_disk_ident_led.py
--rwxr-xr-x   0        0        0      665 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/local_disk/local_disk_list.py
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/local_disk/main.fmf
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/various_commands/__init__.py
--rwxr-xr-x   0        0        0     1622 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/various_commands/capabilities.py
--rwxr-xr-x   0        0        0       18 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/various_commands/file_clone.py
--rwxr-xr-x   0        0        0     1825 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/various_commands/iscsi_chap.py
--rwxr-xr-x   0        0        0       18 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/various_commands/job_status.py
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/various_commands/main.fmf
--rwxr-xr-x   0        0        0      652 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/various_commands/plugin_info.py
--rwxr-xr-x   0        0        0     1660 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/various_commands/pool_member_info.py
--rwxr-xr-x   0        0        0     2940 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/various_commands/system_read_cache_pct_update.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/volume/__init__.py
--rw-r--r--   0        0        0     6376 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/volume/main.fmf
--rwxr-xr-x   0        0        0     1749 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/volume/volume_access_group.py
--rwxr-xr-x   0        0        0     1802 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/volume/volume_cache_info.py
--rwxr-xr-x   0        0        0     5266 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/volume/volume_create.py
--rwxr-xr-x   0        0        0     1599 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/volume/volume_delete.py
--rwxr-xr-x   0        0        0     3287 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/volume/volume_dependants.py
--rwxr-xr-x   0        0        0     3306 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/volume/volume_dependants_rm.py
--rwxr-xr-x   0        0        0     2275 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/volume/volume_disable.py
--rwxr-xr-x   0        0        0     2435 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/volume/volume_enable.py
--rwxr-xr-x   0        0        0     4182 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/volume/volume_ident_led.py
--rwxr-xr-x   0        0        0     4289 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/volume/volume_mask.py
--rwxr-xr-x   0        0        0     3172 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/volume/volume_phy_disk_cache_update.py
--rwxr-xr-x   0        0        0       18 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/volume/volume_raid_create.py
--rwxr-xr-x   0        0        0       18 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/volume/volume_raid_create_cap.py
--rwxr-xr-x   0        0        0       18 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/volume/volume_raid_info.py
--rwxr-xr-x   0        0        0     3204 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/volume/volume_read_cache_policy_update.py
--rwxr-xr-x   0        0        0     5027 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/volume/volume_replicate.py
--rwxr-xr-x   0        0        0     8443 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/volume/volume_replicate_range.py
--rwxr-xr-x   0        0        0     1778 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/volume/volume_replicate_range_block_size.py
--rwxr-xr-x   0        0        0       18 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/volume/volume_resize.py
--rwxr-xr-x   0        0        0     2780 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/volume/volume_unmask.py
--rwxr-xr-x   0        0        0     3195 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/lsmcli/volume/volume_write_cache_policy_update.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/setup/__init__.py
--rwxr-xr-x   0        0        0      840 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/setup/cleanup_configure.py
--rwxr-xr-x   0        0        0     1810 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/setup/cleanup_storage.py
--rwxr-xr-x   0        0        0     1088 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/setup/clone_fs.py
--rwxr-xr-x   0        0        0     3300 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/setup/configure_lsm.py
--rwxr-xr-x   0        0        0     1418 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/setup/create_access_group.py
--rwxr-xr-x   0        0        0     1244 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/setup/create_fs.py
--rwxr-xr-x   0        0        0     1098 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/setup/create_fs_snap.py
--rwxr-xr-x   0        0        0     1402 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/setup/create_volume.py
--rwxr-xr-x   0        0        0     1160 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/setup/export_fs.py
--rw-r--r--   0        0        0     3957 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/setup/main.fmf
--rwxr-xr-x   0        0        0      704 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/setup/mask_volume.py
--rwxr-xr-x   0        0        0      818 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/setup/remove_access_group.py
--rwxr-xr-x   0        0        0      805 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/setup/remove_fs.py
--rwxr-xr-x   0        0        0      996 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/setup/remove_fs_snap.py
--rwxr-xr-x   0        0        0      986 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/setup/remove_volume.py
--rwxr-xr-x   0        0        0      857 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/setup/unexport_fs.py
--rwxr-xr-x   0        0        0      714 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lsm/setup/unmask_volume.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lvm/__init__.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lvm/main.fmf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lvm/cache/__init__.py
--rwxr-xr-x   0        0        0     5544 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lvm/cache/cache_basic.py
--rwxr-xr-x   0        0        0     2878 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lvm/device_mapper_persistent_data/BZ1456019.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lvm/device_mapper_persistent_data/__init__.py
--rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lvm/device_mapper_persistent_data/cache.fmf
--rwxr-xr-x   0        0        0    16806 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lvm/device_mapper_persistent_data/cache.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lvm/device_mapper_persistent_data/cli.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lvm/device_mapper_persistent_data/main.fmf
--rwxr-xr-x   0        0        0    17764 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lvm/device_mapper_persistent_data/restore_corrupting_metadata.py
--rw-r--r--   0        0        0     8444 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lvm/device_mapper_persistent_data/thin.fmf
--rwxr-xr-x   0        0        0    26777 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lvm/device_mapper_persistent_data/thin.py
--rwxr-xr-x   0        0        0     1695 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lvm/device_mapper_persistent_data/tools_not_linked_usr.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lvm/setup/__init__.py
--rw-r--r--   0        0        0    11721 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lvm/setup/main.fmf
--rw-r--r--   0        0        0     9028 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lvm/setup/setup.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lvm/setup/storage/__init__.py
--rwxr-xr-x   0        0        0      999 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lvm/setup/storage/cleanup_crypt.py
--rwxr-xr-x   0        0        0      641 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lvm/setup/storage/cleanup_fcoe.py
--rwxr-xr-x   0        0        0     1301 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lvm/setup/storage/cleanup_iscsi.py
--rwxr-xr-x   0        0        0      863 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lvm/setup/storage/cleanup_multipath.py
--rwxr-xr-x   0        0        0      856 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lvm/setup/storage/cleanup_raid.py
--rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lvm/setup/storage/main.fmf
--rwxr-xr-x   0        0        0     1198 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lvm/setup/storage/setup_crypt.py
--rwxr-xr-x   0        0        0     1262 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lvm/setup/storage/setup_fcoe.py
--rwxr-xr-x   0        0        0     3781 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lvm/setup/storage/setup_iscsi.py
--rwxr-xr-x   0        0        0      544 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lvm/setup/storage/setup_manual.py
--rwxr-xr-x   0        0        0     1094 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lvm/setup/storage/setup_multipath.py
--rwxr-xr-x   0        0        0     3999 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lvm/setup/storage/setup_raid.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lvm/snapper/__init__.py
--rwxr-xr-x   0        0        0    11053 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lvm/snapper/snapper_basic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lvm/thinp/__init__.py
--rwxr-xr-x   0        0        0     3878 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lvm/thinp/discard-perf.py
--rwxr-xr-x   0        0        0     6585 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lvm/thinp/exceed_pool_capacity.py
--rwxr-xr-x   0        0        0    12476 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lvm/thinp/lvchange-thin.py
--rwxr-xr-x   0        0        0     4705 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lvm/thinp/lvconf-thinp.py
--rwxr-xr-x   0        0        0     6201 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lvm/thinp/lvconvert-thin-lv.py
--rwxr-xr-x   0        0        0     4155 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lvm/thinp/lvconvert-thinpool.py
--rwxr-xr-x   0        0        0     9982 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lvm/thinp/lvcreate-liner.py
--rwxr-xr-x   0        0        0     4929 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lvm/thinp/lvcreate-mirror.py
--rwxr-xr-x   0        0        0     4474 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lvm/thinp/lvcreate-poolmetadataspare.py
--rwxr-xr-x   0        0        0     7806 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lvm/thinp/lvcreate-stripe.py
--rwxr-xr-x   0        0        0     9888 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lvm/thinp/lvextend-thinp.py
--rwxr-xr-x   0        0        0     1665 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lvm/thinp/lvm-thinp-misc.py
--rwxr-xr-x   0        0        0     6065 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lvm/thinp/lvm-thinp-modules.py
--rwxr-xr-x   0        0        0     6754 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lvm/thinp/lvreduce-thinp.py
--rwxr-xr-x   0        0        0     4148 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lvm/thinp/lvremove-thinp.py
--rwxr-xr-x   0        0        0     3355 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lvm/thinp/lvrename-thinp.py
--rwxr-xr-x   0        0        0    13362 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lvm/thinp/lvresize-thinp.py
--rwxr-xr-x   0        0        0     8572 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lvm/thinp/lvs-thinp.py
--rwxr-xr-x   0        0        0     4200 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lvm/thinp/lvscan-thinp.py
--rwxr-xr-x   0        0        0     6149 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lvm/thinp/thin-perf.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lvm/thinp/bugs/__init__.py
--rwxr-xr-x   0        0        0     6568 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lvm/thinp/bugs/corrupt_metadata_bz1319937.py
--rwxr-xr-x   0        0        0     6977 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lvm/thinp/bugs/discard_corruption_BZ_918647.py
--rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lvm/thinp/bugs/stripe-blkdiscard.py
--rwxr-xr-x   0        0        0     3504 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/lvm/thinp/bugs/thinpool_with_error_target_meta_bz1305983.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/stratis/__init__.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/stratis/main.fmf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/stratis/common/__init__.py
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/stratis/common/bz1754649_stratis_pid.py
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/stratis/common/main.fmf
--rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/stratis/common/stratis_fs_limit.py
--rw-r--r--   0        0        0     3425 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/stratis/common/stratis_pool_out_of_space.py
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/stratis/common/stratis_repeat_create_destroy.py
--rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/stratis/common/verify_data_in_restarted_pool.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/stratis/data/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/stratis/data/fio/__init__.py
--rwxr-xr-x   0        0        0     3018 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/stratis/data/fio/basic_stress.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/stratis/data/fio/main.fmf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/stratis/setup/__init__.py
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/stratis/setup/cache_disk.py
--rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/stratis/setup/key_set.py
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/stratis/setup/key_unset.py
--rw-r--r--   0        0        0     9073 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/stratis/setup/main.fmf
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/stratis/setup/pool_bind.py
--rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/stratis/setup/pool_create.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/stratis/setup/pool_destroy.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/stratis/setup/pool_restart.py
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/stratis/setup/pool_unbind.py
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/stratis/setup/setup.py
--rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/stratis/setup/tang_server.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/stratis/setup/storage/__init__.py
--rwxr-xr-x   0        0        0      873 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/stratis/setup/storage/cleanup_crypt.py
--rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/stratis/setup/storage/cleanup_free_disks.py
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/stratis/setup/storage/cleanup_iscsi.py
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/stratis/setup/storage/cleanup_loopdev.py
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/stratis/setup/storage/cleanup_lvm.py
--rwxr-xr-x   0        0        0      972 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/stratis/setup/storage/cleanup_raid.py
--rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/stratis/setup/storage/main.fmf
--rwxr-xr-x   0        0        0     2533 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/stratis/setup/storage/setup_crypt.py
--rw-r--r--   0        0        0     7167 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/stratis/setup/storage/setup_free_disks.py
--rwxr-xr-x   0        0        0     4852 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/stratis/setup/storage/setup_iscsi.py
--rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/stratis/setup/storage/setup_loopdev.py
--rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/stratis/setup/storage/setup_lvm.py
--rwxr-xr-x   0        0        0      557 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/stratis/setup/storage/setup_manual.py
--rwxr-xr-x   0        0        0     4314 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/stratis/setup/storage/setup_raid.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/stratis/stratis_cli/__init__.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/stratis/stratis_cli/blockdev.fmf
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/stratis/stratis_cli/daemon.fmf
--rw-r--r--   0        0        0    12956 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/stratis/stratis_cli/fs.fmf
--rw-r--r--   0        0        0    29144 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/stratis/stratis_cli/key.fmf
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/stratis/stratis_cli/main.fmf
--rw-r--r--   0        0        0    36276 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/stratis/stratis_cli/pool.fmf
--rwxr-xr-x   0        0        0     4742 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/stratis/stratis_cli/stratis_cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/targetcli/__init__.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/targetcli/main.fmf
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/targetcli/python-kmod.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/targetcli/cli/__init__.py
--rwxr-xr-x   0        0        0     2975 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/targetcli/cli/block_attributes.py
--rwxr-xr-x   0        0        0      755 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/targetcli/cli/create_pscsi.py
--rwxr-xr-x   0        0        0     2918 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/targetcli/cli/fileio_attributes.py
--rwxr-xr-x   0        0        0     2252 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/targetcli/cli/iscsi_chap.py
--rwxr-xr-x   0        0        0     2444 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/targetcli/cli/iscsi_chap_2ways.py
--rwxr-xr-x   0        0        0     1963 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/targetcli/cli/iscsi_local_target.py
--rw-r--r--   0        0        0     5245 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/targetcli/cli/main.fmf
--rwxr-xr-x   0        0        0     2921 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/targetcli/cli/ramdisk_attributes.py
--rwxr-xr-x   0        0        0     4163 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/targetcli/cli/saveconfig_backup.py
--rwxr-xr-x   0        0        0     1801 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/targetcli/cli/saveconfig_compare.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/targetcli/setup/__init__.py
--rwxr-xr-x   0        0        0     3746 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/targetcli/setup/configure_chap.py
--rwxr-xr-x   0        0        0     2238 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/targetcli/setup/create_backstore.py
--rwxr-xr-x   0        0        0     2134 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/targetcli/setup/create_fileio_target.py
--rwxr-xr-x   0        0        0     1599 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/targetcli/setup/create_loopback.py
--rwxr-xr-x   0        0        0      940 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/targetcli/setup/create_loopdev.py
--rwxr-xr-x   0        0        0     1236 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/targetcli/setup/create_qcow.py
--rwxr-xr-x   0        0        0     2140 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/targetcli/setup/create_qcow_target.py
--rwxr-xr-x   0        0        0      558 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/targetcli/setup/create_saveconfig.py
--rwxr-xr-x   0        0        0     1196 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/targetcli/setup/delete_backstore.py
--rwxr-xr-x   0        0        0      528 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/targetcli/setup/delete_iscsi_target.py
--rwxr-xr-x   0        0        0      659 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/targetcli/setup/delete_loopback.py
--rwxr-xr-x   0        0        0      455 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/targetcli/setup/delete_loopdev.py
--rwxr-xr-x   0        0        0      535 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/targetcli/setup/delete_qcow.py
--rwxr-xr-x   0        0        0     1156 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/targetcli/setup/disable_chap.py
--rwxr-xr-x   0        0        0     2142 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/targetcli/setup/install_tcmu_runner.py
--rw-r--r--   0        0        0     6644 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/targetcli/setup/main.fmf
--rwxr-xr-x   0        0        0     2123 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/targetcli/setup/start_multipath.py
--rwxr-xr-x   0        0        0     1782 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/targetcli/setup/stop_multipath.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/targetd/__init__.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/targetd/main.fmf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/targetd/setup/__init__.py
--rwxr-xr-x   0        0        0      863 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/targetd/setup/create_loopdev.py
--rwxr-xr-x   0        0        0      453 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/targetd/setup/delete_loopdev.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/targetd/setup/main.fmf
--rwxr-xr-x   0        0        0     1111 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/targetd/setup/prepare_conf.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/targetd/targetd_basic/__init__.py
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/targetd/targetd_basic/main.fmf
--rwxr-xr-x   0        0        0     1189 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/targetd/targetd_basic/targetd_basic.py
--rwxr-xr-x   0        0        0     1437 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/targetd/targetd_basic/targetd_no_passwd.py
--rwxr-xr-x   0        0        0     1641 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/targetd/targetd_basic/targetd_no_vg.py
--rwxr-xr-x   0        0        0     2126 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/targetd/targetd_basic/targetd_ssl.py
--rwxr-xr-x   0        0        0     2199 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/targetd/targetd_basic/targetd_ssl_no_cert.py
--rwxr-xr-x   0        0        0     1797 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/targetd/targetd_basic/targetd_ssl_no_key.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/vdo/__init__.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/vdo/main.fmf
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/vdo/data/__init__.py
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/vdo/data/main.fmf
--rwxr-xr-x   0        0        0     3869 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/vdo/data/repeated_copy.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/vdo/data/fio/__init__.py
--rwxr-xr-x   0        0        0     1875 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/vdo/data/fio/basic_stress.py
--rwxr-xr-x   0        0        0     1874 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/vdo/data/fio/fs.py
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/vdo/data/fio/main.fmf
--rwxr-xr-x   0        0        0     2365 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/vdo/data/fio/vdo_on_vdo.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/vdo/kernel_modules/__init__.py
--rwxr-xr-x   0        0        0     1680 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/vdo/kernel_modules/kvdo.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/vdo/kernel_modules/main.fmf
--rwxr-xr-x   0        0        0     1515 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/vdo/kernel_modules/signatures.py
--rwxr-xr-x   0        0        0     1348 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/vdo/kernel_modules/uds.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/vdo/setup/__init__.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/vdo/setup/data.fmf
--rw-r--r--   0        0        0     5346 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/vdo/setup/main.fmf
--rw-r--r--   0        0        0     8021 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/vdo/setup/setup.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/vdo/setup/storage/__init__.py
--rwxr-xr-x   0        0        0     1103 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/vdo/setup/storage/cleanup_crypt.py
--rwxr-xr-x   0        0        0      642 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/vdo/setup/storage/cleanup_fcoe.py
--rwxr-xr-x   0        0        0     1398 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/vdo/setup/storage/cleanup_iscsi.py
--rwxr-xr-x   0        0        0      932 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/vdo/setup/storage/cleanup_multipath.py
--rwxr-xr-x   0        0        0      921 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/vdo/setup/storage/cleanup_raid.py
--rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/vdo/setup/storage/main.fmf
--rwxr-xr-x   0        0        0     1341 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/vdo/setup/storage/setup_crypt.py
--rwxr-xr-x   0        0        0     1302 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/vdo/setup/storage/setup_fcoe.py
--rwxr-xr-x   0        0        0     3975 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/vdo/setup/storage/setup_iscsi.py
--rwxr-xr-x   0        0        0      545 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/vdo/setup/storage/setup_manual.py
--rwxr-xr-x   0        0        0     1167 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/vdo/setup/storage/setup_multipath.py
--rwxr-xr-x   0        0        0     4111 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/vdo/setup/storage/setup_raid.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/vdo/vdo_cli/__init__.py
--rw-r--r--   0        0        0    27559 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/vdo/vdo_cli/create.fmf
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/vdo/vdo_cli/main.fmf
--rw-r--r--   0        0        0     9281 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/vdo/vdo_cli/modify.fmf
--rw-r--r--   0        0        0    15976 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/vdo/vdo_cli/various_commands.fmf
--rwxr-xr-x   0        0        0     9791 2020-02-02 00:00:00.000000 stqe-0.2.3/stqe/tests/vdo/vdo_cli/vdo_cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.3/tests/__init__.py
--rwxr-xr-x   0        0        0      677 2020-02-02 00:00:00.000000 stqe-0.2.3/tests/augeas_test.py
--rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 stqe-0.2.3/tests/logchecker_test.py
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 stqe-0.2.3/tests/persistent_vars_test.py
--rw-r--r--   0        0        0     3744 2020-02-02 00:00:00.000000 stqe-0.2.3/tests/tc_test.py
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 stqe-0.2.3/LICENSE
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 stqe-0.2.3/README.md
--rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 stqe-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 stqe-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 stqe-0.2.4/.gitlab-ci.yml
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 stqe-0.2.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 stqe-0.2.4/noxfile.py
+-rwxr-xr-x   0        0        0      901 2020-02-02 00:00:00.000000 stqe-0.2.4/release.sh
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 stqe-0.2.4/requirements-stable.txt
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/__init__.py
+-rw-r--r--   0        0        0    31943 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/stqe_test.py
+-rwxr-xr-x   0        0        0     2628 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/stqe_tool.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/conf/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/conf/lvm/__init__.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/conf/lvm/lvm-thinp-basic.conf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/host/__init__.py
+-rwxr-xr-x   0        0        0     5759 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/host/atomic_run.py
+-rw-r--r--   0        0        0     4902 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/host/beaker.py
+-rw-r--r--   0        0        0    21048 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/host/fmf_tools.py
+-rw-r--r--   0        0        0     9424 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/host/iscsi.py
+-rw-r--r--   0        0        0    12203 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/host/logchecker.py
+-rw-r--r--   0        0        0     5007 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/host/lsm.py
+-rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/host/lvm.py
+-rw-r--r--   0        0        0    41736 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/host/nfs_lock.py
+-rw-r--r--   0        0        0     9088 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/host/persistent_vars.py
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/host/restraint.py
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/host/stratis.py
+-rw-r--r--   0        0        0    10173 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/host/tc.py
+-rw-r--r--   0        0        0     7014 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/host/vdo.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/__init__.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/.fmf/version
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/dm/__init__.py
+-rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/dm/block_boundary_obedience.py
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/dm/error_block_alignment.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/dm/main.fmf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/hba/__init__.py
+-rwxr-xr-x   0        0        0    11145 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/hba/add_new_lun.py
+-rwxr-xr-x   0        0        0    13817 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/hba/dev_loss_tmo.py
+-rwxr-xr-x   0        0        0     4590 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/hba/io-failover-alternate-interface.py
+-rwxr-xr-x   0        0        0     9440 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/hba/io-remove-lun.py
+-rwxr-xr-x   0        0        0    34651 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/hba/mp_failover.py
+-rwxr-xr-x   0        0        0     8166 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/hba/online_offline.py
+-rwxr-xr-x   0        0        0    16563 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/hba/oscilate_port.py
+-rwxr-xr-x   0        0        0     3930 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/hba/show_driver_info.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/iscsi/__init__.py
+-rwxr-xr-x   0        0        0     8759 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/iscsi/iscsi_params.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/iscsi/main.fmf
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/iscsi/cli/__init__.py
+-rwxr-xr-x   0        0        0     1970 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/iscsi/cli/iscsi_local_target.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/iscsi/cli/main.fmf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/iscsi/setup/__init__.py
+-rwxr-xr-x   0        0        0     2238 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/iscsi/setup/create_backstore.py
+-rwxr-xr-x   0        0        0     2134 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/iscsi/setup/create_fileio_target.py
+-rwxr-xr-x   0        0        0     1196 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/iscsi/setup/delete_backstore.py
+-rwxr-xr-x   0        0        0      528 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/iscsi/setup/delete_iscsi_target.py
+-rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/iscsi/setup/main.fmf
+-rwxr-xr-x   0        0        0     2123 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/iscsi/setup/start_multipath.py
+-rwxr-xr-x   0        0        0     1782 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/iscsi/setup/stop_multipath.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/__init__.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/main.fmf
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/__init__.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/main.fmf
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/access_group/__init__.py
+-rwxr-xr-x   0        0        0     5491 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/access_group/access_group_add.py
+-rwxr-xr-x   0        0        0     4290 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/access_group/access_group_create.py
+-rwxr-xr-x   0        0        0     1749 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/access_group/access_group_delete.py
+-rwxr-xr-x   0        0        0     3355 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/access_group/access_group_remove.py
+-rwxr-xr-x   0        0        0     2021 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/access_group/access_group_volumes.py
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/access_group/main.fmf
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/fs/__init__.py
+-rwxr-xr-x   0        0        0     4637 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/fs/fs_clone.py
+-rwxr-xr-x   0        0        0     4788 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/fs/fs_create.py
+-rwxr-xr-x   0        0        0     1396 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/fs/fs_delete.py
+-rwxr-xr-x   0        0        0     2815 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/fs/fs_dependants.py
+-rwxr-xr-x   0        0        0     4618 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/fs/fs_dependants_rm.py
+-rwxr-xr-x   0        0        0     2444 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/fs/fs_export.py
+-rwxr-xr-x   0        0        0     4125 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/fs/fs_resize.py
+-rwxr-xr-x   0        0        0     4334 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/fs/fs_snap_create.py
+-rwxr-xr-x   0        0        0     2123 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/fs/fs_snap_delete.py
+-rwxr-xr-x   0        0        0     3031 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/fs/fs_snap_restore.py
+-rwxr-xr-x   0        0        0     1425 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/fs/fs_unexport.py
+-rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/fs/main.fmf
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/list/__init__.py
+-rwxr-xr-x   0        0        0     1902 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/list/access_groups.py
+-rwxr-xr-x   0        0        0     1854 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/list/batteries.py
+-rwxr-xr-x   0        0        0     1783 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/list/disks.py
+-rwxr-xr-x   0        0        0     1803 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/list/exports.py
+-rwxr-xr-x   0        0        0     1725 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/list/fs.py
+-rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/list/main.fmf
+-rwxr-xr-x   0        0        0     1577 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/list/nsf_client_auth.py
+-rwxr-xr-x   0        0        0     1513 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/list/plugins.py
+-rwxr-xr-x   0        0        0     1783 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/list/pools.py
+-rwxr-xr-x   0        0        0     1116 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/list/snapshots.py
+-rwxr-xr-x   0        0        0     1513 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/list/systems.py
+-rwxr-xr-x   0        0        0     1853 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/list/target_ports.py
+-rwxr-xr-x   0        0        0     1846 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/list/volumes.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/local_disk/__init__.py
+-rwxr-xr-x   0        0        0     3366 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/local_disk/local_disk_fault_led.py
+-rwxr-xr-x   0        0        0     3384 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/local_disk/local_disk_ident_led.py
+-rwxr-xr-x   0        0        0      665 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/local_disk/local_disk_list.py
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/local_disk/main.fmf
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/various_commands/__init__.py
+-rwxr-xr-x   0        0        0     1622 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/various_commands/capabilities.py
+-rwxr-xr-x   0        0        0       18 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/various_commands/file_clone.py
+-rwxr-xr-x   0        0        0     1825 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/various_commands/iscsi_chap.py
+-rwxr-xr-x   0        0        0       18 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/various_commands/job_status.py
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/various_commands/main.fmf
+-rwxr-xr-x   0        0        0      652 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/various_commands/plugin_info.py
+-rwxr-xr-x   0        0        0     1660 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/various_commands/pool_member_info.py
+-rwxr-xr-x   0        0        0     2940 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/various_commands/system_read_cache_pct_update.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/volume/__init__.py
+-rw-r--r--   0        0        0     6376 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/volume/main.fmf
+-rwxr-xr-x   0        0        0     1749 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/volume/volume_access_group.py
+-rwxr-xr-x   0        0        0     1802 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/volume/volume_cache_info.py
+-rwxr-xr-x   0        0        0     5266 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/volume/volume_create.py
+-rwxr-xr-x   0        0        0     1599 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/volume/volume_delete.py
+-rwxr-xr-x   0        0        0     3287 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/volume/volume_dependants.py
+-rwxr-xr-x   0        0        0     3306 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/volume/volume_dependants_rm.py
+-rwxr-xr-x   0        0        0     2275 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/volume/volume_disable.py
+-rwxr-xr-x   0        0        0     2435 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/volume/volume_enable.py
+-rwxr-xr-x   0        0        0     4182 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/volume/volume_ident_led.py
+-rwxr-xr-x   0        0        0     4289 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/volume/volume_mask.py
+-rwxr-xr-x   0        0        0     3172 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/volume/volume_phy_disk_cache_update.py
+-rwxr-xr-x   0        0        0       18 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/volume/volume_raid_create.py
+-rwxr-xr-x   0        0        0       18 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/volume/volume_raid_create_cap.py
+-rwxr-xr-x   0        0        0       18 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/volume/volume_raid_info.py
+-rwxr-xr-x   0        0        0     3204 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/volume/volume_read_cache_policy_update.py
+-rwxr-xr-x   0        0        0     5027 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/volume/volume_replicate.py
+-rwxr-xr-x   0        0        0     8443 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/volume/volume_replicate_range.py
+-rwxr-xr-x   0        0        0     1778 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/volume/volume_replicate_range_block_size.py
+-rwxr-xr-x   0        0        0       18 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/volume/volume_resize.py
+-rwxr-xr-x   0        0        0     2780 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/volume/volume_unmask.py
+-rwxr-xr-x   0        0        0     3195 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/lsmcli/volume/volume_write_cache_policy_update.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/setup/__init__.py
+-rwxr-xr-x   0        0        0      840 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/setup/cleanup_configure.py
+-rwxr-xr-x   0        0        0     1810 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/setup/cleanup_storage.py
+-rwxr-xr-x   0        0        0     1088 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/setup/clone_fs.py
+-rwxr-xr-x   0        0        0     3300 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/setup/configure_lsm.py
+-rwxr-xr-x   0        0        0     1418 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/setup/create_access_group.py
+-rwxr-xr-x   0        0        0     1244 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/setup/create_fs.py
+-rwxr-xr-x   0        0        0     1098 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/setup/create_fs_snap.py
+-rwxr-xr-x   0        0        0     1402 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/setup/create_volume.py
+-rwxr-xr-x   0        0        0     1160 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/setup/export_fs.py
+-rw-r--r--   0        0        0     3957 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/setup/main.fmf
+-rwxr-xr-x   0        0        0      704 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/setup/mask_volume.py
+-rwxr-xr-x   0        0        0      818 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/setup/remove_access_group.py
+-rwxr-xr-x   0        0        0      805 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/setup/remove_fs.py
+-rwxr-xr-x   0        0        0      996 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/setup/remove_fs_snap.py
+-rwxr-xr-x   0        0        0      986 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/setup/remove_volume.py
+-rwxr-xr-x   0        0        0      857 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/setup/unexport_fs.py
+-rwxr-xr-x   0        0        0      714 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lsm/setup/unmask_volume.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lvm/__init__.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lvm/main.fmf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lvm/cache/__init__.py
+-rwxr-xr-x   0        0        0     5544 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lvm/cache/cache_basic.py
+-rwxr-xr-x   0        0        0     2878 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lvm/device_mapper_persistent_data/BZ1456019.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lvm/device_mapper_persistent_data/__init__.py
+-rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lvm/device_mapper_persistent_data/cache.fmf
+-rwxr-xr-x   0        0        0    16806 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lvm/device_mapper_persistent_data/cache.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lvm/device_mapper_persistent_data/cli.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lvm/device_mapper_persistent_data/main.fmf
+-rwxr-xr-x   0        0        0    17764 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lvm/device_mapper_persistent_data/restore_corrupting_metadata.py
+-rw-r--r--   0        0        0     8444 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lvm/device_mapper_persistent_data/thin.fmf
+-rwxr-xr-x   0        0        0    26777 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lvm/device_mapper_persistent_data/thin.py
+-rwxr-xr-x   0        0        0     1695 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lvm/device_mapper_persistent_data/tools_not_linked_usr.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lvm/setup/__init__.py
+-rw-r--r--   0        0        0    11721 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lvm/setup/main.fmf
+-rw-r--r--   0        0        0     9028 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lvm/setup/setup.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lvm/setup/storage/__init__.py
+-rwxr-xr-x   0        0        0      999 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lvm/setup/storage/cleanup_crypt.py
+-rwxr-xr-x   0        0        0      641 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lvm/setup/storage/cleanup_fcoe.py
+-rwxr-xr-x   0        0        0     1301 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lvm/setup/storage/cleanup_iscsi.py
+-rwxr-xr-x   0        0        0      863 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lvm/setup/storage/cleanup_multipath.py
+-rwxr-xr-x   0        0        0      856 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lvm/setup/storage/cleanup_raid.py
+-rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lvm/setup/storage/main.fmf
+-rwxr-xr-x   0        0        0     1198 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lvm/setup/storage/setup_crypt.py
+-rwxr-xr-x   0        0        0     1262 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lvm/setup/storage/setup_fcoe.py
+-rwxr-xr-x   0        0        0     3781 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lvm/setup/storage/setup_iscsi.py
+-rwxr-xr-x   0        0        0      544 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lvm/setup/storage/setup_manual.py
+-rwxr-xr-x   0        0        0     1094 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lvm/setup/storage/setup_multipath.py
+-rwxr-xr-x   0        0        0     3999 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lvm/setup/storage/setup_raid.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lvm/snapper/__init__.py
+-rwxr-xr-x   0        0        0    11053 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lvm/snapper/snapper_basic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lvm/thinp/__init__.py
+-rwxr-xr-x   0        0        0     3878 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lvm/thinp/discard-perf.py
+-rwxr-xr-x   0        0        0     6585 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lvm/thinp/exceed_pool_capacity.py
+-rwxr-xr-x   0        0        0    12476 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lvm/thinp/lvchange-thin.py
+-rwxr-xr-x   0        0        0     4705 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lvm/thinp/lvconf-thinp.py
+-rwxr-xr-x   0        0        0     6201 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lvm/thinp/lvconvert-thin-lv.py
+-rwxr-xr-x   0        0        0     4155 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lvm/thinp/lvconvert-thinpool.py
+-rwxr-xr-x   0        0        0     9982 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lvm/thinp/lvcreate-liner.py
+-rwxr-xr-x   0        0        0     4929 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lvm/thinp/lvcreate-mirror.py
+-rwxr-xr-x   0        0        0     4474 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lvm/thinp/lvcreate-poolmetadataspare.py
+-rwxr-xr-x   0        0        0     7806 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lvm/thinp/lvcreate-stripe.py
+-rwxr-xr-x   0        0        0     9888 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lvm/thinp/lvextend-thinp.py
+-rwxr-xr-x   0        0        0     1665 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lvm/thinp/lvm-thinp-misc.py
+-rwxr-xr-x   0        0        0     6065 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lvm/thinp/lvm-thinp-modules.py
+-rwxr-xr-x   0        0        0     6754 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lvm/thinp/lvreduce-thinp.py
+-rwxr-xr-x   0        0        0     4148 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lvm/thinp/lvremove-thinp.py
+-rwxr-xr-x   0        0        0     3355 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lvm/thinp/lvrename-thinp.py
+-rwxr-xr-x   0        0        0    13362 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lvm/thinp/lvresize-thinp.py
+-rwxr-xr-x   0        0        0     8572 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lvm/thinp/lvs-thinp.py
+-rwxr-xr-x   0        0        0     4200 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lvm/thinp/lvscan-thinp.py
+-rwxr-xr-x   0        0        0     6149 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lvm/thinp/thin-perf.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lvm/thinp/bugs/__init__.py
+-rwxr-xr-x   0        0        0     6568 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lvm/thinp/bugs/corrupt_metadata_bz1319937.py
+-rwxr-xr-x   0        0        0     6977 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lvm/thinp/bugs/discard_corruption_BZ_918647.py
+-rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lvm/thinp/bugs/stripe-blkdiscard.py
+-rwxr-xr-x   0        0        0     3504 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/lvm/thinp/bugs/thinpool_with_error_target_meta_bz1305983.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/stratis/__init__.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/stratis/main.fmf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/stratis/common/__init__.py
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/stratis/common/bz1754649_stratis_pid.py
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/stratis/common/main.fmf
+-rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/stratis/common/stratis_fs_limit.py
+-rw-r--r--   0        0        0     3425 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/stratis/common/stratis_pool_out_of_space.py
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/stratis/common/stratis_repeat_create_destroy.py
+-rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/stratis/common/verify_data_in_restarted_pool.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/stratis/data/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/stratis/data/fio/__init__.py
+-rwxr-xr-x   0        0        0     3018 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/stratis/data/fio/basic_stress.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/stratis/data/fio/main.fmf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/stratis/setup/__init__.py
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/stratis/setup/cache_disk.py
+-rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/stratis/setup/key_set.py
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/stratis/setup/key_unset.py
+-rw-r--r--   0        0        0     9073 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/stratis/setup/main.fmf
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/stratis/setup/pool_bind.py
+-rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/stratis/setup/pool_create.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/stratis/setup/pool_destroy.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/stratis/setup/pool_restart.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/stratis/setup/pool_unbind.py
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/stratis/setup/setup.py
+-rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/stratis/setup/tang_server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/stratis/setup/storage/__init__.py
+-rwxr-xr-x   0        0        0      873 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/stratis/setup/storage/cleanup_crypt.py
+-rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/stratis/setup/storage/cleanup_free_disks.py
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/stratis/setup/storage/cleanup_iscsi.py
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/stratis/setup/storage/cleanup_loopdev.py
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/stratis/setup/storage/cleanup_lvm.py
+-rwxr-xr-x   0        0        0      972 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/stratis/setup/storage/cleanup_raid.py
+-rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/stratis/setup/storage/main.fmf
+-rwxr-xr-x   0        0        0     2533 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/stratis/setup/storage/setup_crypt.py
+-rw-r--r--   0        0        0     7167 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/stratis/setup/storage/setup_free_disks.py
+-rwxr-xr-x   0        0        0     4852 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/stratis/setup/storage/setup_iscsi.py
+-rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/stratis/setup/storage/setup_loopdev.py
+-rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/stratis/setup/storage/setup_lvm.py
+-rwxr-xr-x   0        0        0      557 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/stratis/setup/storage/setup_manual.py
+-rwxr-xr-x   0        0        0     4314 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/stratis/setup/storage/setup_raid.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/stratis/stratis_cli/__init__.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/stratis/stratis_cli/blockdev.fmf
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/stratis/stratis_cli/daemon.fmf
+-rw-r--r--   0        0        0    12956 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/stratis/stratis_cli/fs.fmf
+-rw-r--r--   0        0        0    29144 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/stratis/stratis_cli/key.fmf
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/stratis/stratis_cli/main.fmf
+-rw-r--r--   0        0        0    36276 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/stratis/stratis_cli/pool.fmf
+-rwxr-xr-x   0        0        0     4742 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/stratis/stratis_cli/stratis_cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/targetcli/__init__.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/targetcli/main.fmf
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/targetcli/python-kmod.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/targetcli/cli/__init__.py
+-rwxr-xr-x   0        0        0     2975 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/targetcli/cli/block_attributes.py
+-rwxr-xr-x   0        0        0      755 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/targetcli/cli/create_pscsi.py
+-rwxr-xr-x   0        0        0     2918 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/targetcli/cli/fileio_attributes.py
+-rwxr-xr-x   0        0        0     2252 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/targetcli/cli/iscsi_chap.py
+-rwxr-xr-x   0        0        0     2444 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/targetcli/cli/iscsi_chap_2ways.py
+-rwxr-xr-x   0        0        0     1963 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/targetcli/cli/iscsi_local_target.py
+-rw-r--r--   0        0        0     5245 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/targetcli/cli/main.fmf
+-rwxr-xr-x   0        0        0     2921 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/targetcli/cli/ramdisk_attributes.py
+-rwxr-xr-x   0        0        0     4163 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/targetcli/cli/saveconfig_backup.py
+-rwxr-xr-x   0        0        0     1801 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/targetcli/cli/saveconfig_compare.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/targetcli/setup/__init__.py
+-rwxr-xr-x   0        0        0     3746 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/targetcli/setup/configure_chap.py
+-rwxr-xr-x   0        0        0     2238 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/targetcli/setup/create_backstore.py
+-rwxr-xr-x   0        0        0     2134 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/targetcli/setup/create_fileio_target.py
+-rwxr-xr-x   0        0        0     1599 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/targetcli/setup/create_loopback.py
+-rwxr-xr-x   0        0        0      940 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/targetcli/setup/create_loopdev.py
+-rwxr-xr-x   0        0        0     1236 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/targetcli/setup/create_qcow.py
+-rwxr-xr-x   0        0        0     2140 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/targetcli/setup/create_qcow_target.py
+-rwxr-xr-x   0        0        0      558 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/targetcli/setup/create_saveconfig.py
+-rwxr-xr-x   0        0        0     1196 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/targetcli/setup/delete_backstore.py
+-rwxr-xr-x   0        0        0      528 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/targetcli/setup/delete_iscsi_target.py
+-rwxr-xr-x   0        0        0      659 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/targetcli/setup/delete_loopback.py
+-rwxr-xr-x   0        0        0      455 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/targetcli/setup/delete_loopdev.py
+-rwxr-xr-x   0        0        0      535 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/targetcli/setup/delete_qcow.py
+-rwxr-xr-x   0        0        0     1156 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/targetcli/setup/disable_chap.py
+-rwxr-xr-x   0        0        0     2142 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/targetcli/setup/install_tcmu_runner.py
+-rw-r--r--   0        0        0     6644 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/targetcli/setup/main.fmf
+-rwxr-xr-x   0        0        0     2123 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/targetcli/setup/start_multipath.py
+-rwxr-xr-x   0        0        0     1782 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/targetcli/setup/stop_multipath.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/targetd/__init__.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/targetd/main.fmf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/targetd/setup/__init__.py
+-rwxr-xr-x   0        0        0      863 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/targetd/setup/create_loopdev.py
+-rwxr-xr-x   0        0        0      453 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/targetd/setup/delete_loopdev.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/targetd/setup/main.fmf
+-rwxr-xr-x   0        0        0     1111 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/targetd/setup/prepare_conf.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/targetd/targetd_basic/__init__.py
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/targetd/targetd_basic/main.fmf
+-rwxr-xr-x   0        0        0     1189 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/targetd/targetd_basic/targetd_basic.py
+-rwxr-xr-x   0        0        0     1437 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/targetd/targetd_basic/targetd_no_passwd.py
+-rwxr-xr-x   0        0        0     1641 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/targetd/targetd_basic/targetd_no_vg.py
+-rwxr-xr-x   0        0        0     2126 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/targetd/targetd_basic/targetd_ssl.py
+-rwxr-xr-x   0        0        0     2199 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/targetd/targetd_basic/targetd_ssl_no_cert.py
+-rwxr-xr-x   0        0        0     1797 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/targetd/targetd_basic/targetd_ssl_no_key.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/vdo/__init__.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/vdo/main.fmf
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/vdo/data/__init__.py
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/vdo/data/main.fmf
+-rwxr-xr-x   0        0        0     3869 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/vdo/data/repeated_copy.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/vdo/data/fio/__init__.py
+-rwxr-xr-x   0        0        0     1875 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/vdo/data/fio/basic_stress.py
+-rwxr-xr-x   0        0        0     1874 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/vdo/data/fio/fs.py
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/vdo/data/fio/main.fmf
+-rwxr-xr-x   0        0        0     2365 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/vdo/data/fio/vdo_on_vdo.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/vdo/kernel_modules/__init__.py
+-rwxr-xr-x   0        0        0     1680 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/vdo/kernel_modules/kvdo.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/vdo/kernel_modules/main.fmf
+-rwxr-xr-x   0        0        0     1515 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/vdo/kernel_modules/signatures.py
+-rwxr-xr-x   0        0        0     1348 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/vdo/kernel_modules/uds.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/vdo/setup/__init__.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/vdo/setup/data.fmf
+-rw-r--r--   0        0        0     5346 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/vdo/setup/main.fmf
+-rw-r--r--   0        0        0     8021 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/vdo/setup/setup.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/vdo/setup/storage/__init__.py
+-rwxr-xr-x   0        0        0     1103 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/vdo/setup/storage/cleanup_crypt.py
+-rwxr-xr-x   0        0        0      642 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/vdo/setup/storage/cleanup_fcoe.py
+-rwxr-xr-x   0        0        0     1398 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/vdo/setup/storage/cleanup_iscsi.py
+-rwxr-xr-x   0        0        0      932 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/vdo/setup/storage/cleanup_multipath.py
+-rwxr-xr-x   0        0        0      921 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/vdo/setup/storage/cleanup_raid.py
+-rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/vdo/setup/storage/main.fmf
+-rwxr-xr-x   0        0        0     1341 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/vdo/setup/storage/setup_crypt.py
+-rwxr-xr-x   0        0        0     1302 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/vdo/setup/storage/setup_fcoe.py
+-rwxr-xr-x   0        0        0     3975 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/vdo/setup/storage/setup_iscsi.py
+-rwxr-xr-x   0        0        0      545 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/vdo/setup/storage/setup_manual.py
+-rwxr-xr-x   0        0        0     1167 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/vdo/setup/storage/setup_multipath.py
+-rwxr-xr-x   0        0        0     4111 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/vdo/setup/storage/setup_raid.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/vdo/vdo_cli/__init__.py
+-rw-r--r--   0        0        0    27559 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/vdo/vdo_cli/create.fmf
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/vdo/vdo_cli/main.fmf
+-rw-r--r--   0        0        0     9281 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/vdo/vdo_cli/modify.fmf
+-rw-r--r--   0        0        0    15976 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/vdo/vdo_cli/various_commands.fmf
+-rwxr-xr-x   0        0        0     9791 2020-02-02 00:00:00.000000 stqe-0.2.4/stqe/tests/vdo/vdo_cli/vdo_cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stqe-0.2.4/tests/__init__.py
+-rwxr-xr-x   0        0        0      677 2020-02-02 00:00:00.000000 stqe-0.2.4/tests/augeas_test.py
+-rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 stqe-0.2.4/tests/logchecker_test.py
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 stqe-0.2.4/tests/persistent_vars_test.py
+-rw-r--r--   0        0        0     3744 2020-02-02 00:00:00.000000 stqe-0.2.4/tests/tc_test.py
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 stqe-0.2.4/LICENSE
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 stqe-0.2.4/README.md
+-rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 stqe-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 stqe-0.2.4/PKG-INFO
```

### Comparing `stqe-0.2.3/.gitlab-ci.yml` & `stqe-0.2.4/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/.pre-commit-config.yaml` & `stqe-0.2.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/noxfile.py` & `stqe-0.2.4/noxfile.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/release.sh` & `stqe-0.2.4/release.sh`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/requirements-stable.txt` & `stqe-0.2.4/requirements-stable.txt`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/stqe_test.py` & `stqe-0.2.4/stqe/stqe_test.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/stqe_tool.py` & `stqe-0.2.4/stqe/stqe_tool.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/host/atomic_run.py` & `stqe-0.2.4/stqe/host/atomic_run.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/host/beaker.py` & `stqe-0.2.4/stqe/host/beaker.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/host/fmf_tools.py` & `stqe-0.2.4/stqe/host/fmf_tools.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/host/iscsi.py` & `stqe-0.2.4/stqe/host/iscsi.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/host/logchecker.py` & `stqe-0.2.4/stqe/host/logchecker.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,16 +46,14 @@
         error += 1
     if not abrt_check():
         error += 1
     if not messages_dump_check():
         error += 1
     if not dmesg_check():
         error += 1
-    if not console_log_check():
-        error += 1
     if not kdump_check():
         error += 1
 
     if error:
         log_messages = "/var/log/messages"
         if os.path.isfile(log_messages):
             print("submit %s, named messages.log" % log_messages)
@@ -295,22 +293,14 @@
     if error:
         return False
 
     print("PASS: No errors on dmesg have been found.")
     return True
 
 
-def console_log_check():
-    """Checks for error messages on console log ("Call Trace and segfault")"""
-    if not stqe.host.beaker.is_beaker_job():
-        # skip check
-        return True
-    return stqe.host.beaker.console_log_check(error_mgs)
-
-
 def kdump_check():
     """
     Check for kdump error messages.
     It assumes kdump is configured on /var/crash
     """
     error = 0
```

### Comparing `stqe-0.2.3/stqe/host/lsm.py` & `stqe-0.2.4/stqe/host/lsm.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/host/lvm.py` & `stqe-0.2.4/stqe/host/lvm.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/host/nfs_lock.py` & `stqe-0.2.4/stqe/host/nfs_lock.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/host/persistent_vars.py` & `stqe-0.2.4/stqe/host/persistent_vars.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/host/restraint.py` & `stqe-0.2.4/stqe/host/restraint.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/host/stratis.py` & `stqe-0.2.4/stqe/host/stratis.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/host/tc.py` & `stqe-0.2.4/stqe/host/tc.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/host/vdo.py` & `stqe-0.2.4/stqe/host/vdo.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/dm/block_boundary_obedience.py` & `stqe-0.2.4/stqe/tests/dm/block_boundary_obedience.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/dm/error_block_alignment.py` & `stqe-0.2.4/stqe/tests/dm/error_block_alignment.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/hba/add_new_lun.py` & `stqe-0.2.4/stqe/tests/hba/add_new_lun.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/hba/dev_loss_tmo.py` & `stqe-0.2.4/stqe/tests/hba/dev_loss_tmo.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/hba/io-failover-alternate-interface.py` & `stqe-0.2.4/stqe/tests/hba/io-failover-alternate-interface.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/hba/io-remove-lun.py` & `stqe-0.2.4/stqe/tests/hba/io-remove-lun.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/hba/mp_failover.py` & `stqe-0.2.4/stqe/tests/hba/mp_failover.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/hba/online_offline.py` & `stqe-0.2.4/stqe/tests/hba/online_offline.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/hba/oscilate_port.py` & `stqe-0.2.4/stqe/tests/hba/oscilate_port.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/hba/show_driver_info.py` & `stqe-0.2.4/stqe/tests/hba/show_driver_info.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/iscsi/iscsi_params.py` & `stqe-0.2.4/stqe/tests/iscsi/iscsi_params.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/iscsi/cli/iscsi_local_target.py` & `stqe-0.2.4/stqe/tests/iscsi/cli/iscsi_local_target.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/iscsi/setup/create_backstore.py` & `stqe-0.2.4/stqe/tests/iscsi/setup/create_backstore.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/iscsi/setup/create_fileio_target.py` & `stqe-0.2.4/stqe/tests/iscsi/setup/create_fileio_target.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/iscsi/setup/delete_backstore.py` & `stqe-0.2.4/stqe/tests/iscsi/setup/delete_backstore.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/iscsi/setup/delete_iscsi_target.py` & `stqe-0.2.4/stqe/tests/iscsi/setup/delete_iscsi_target.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/iscsi/setup/main.fmf` & `stqe-0.2.4/stqe/tests/iscsi/setup/main.fmf`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/iscsi/setup/start_multipath.py` & `stqe-0.2.4/stqe/tests/iscsi/setup/start_multipath.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/iscsi/setup/stop_multipath.py` & `stqe-0.2.4/stqe/tests/iscsi/setup/stop_multipath.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/access_group/access_group_add.py` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/access_group/access_group_add.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/access_group/access_group_create.py` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/access_group/access_group_create.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/access_group/access_group_delete.py` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/access_group/access_group_delete.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/access_group/access_group_remove.py` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/access_group/access_group_remove.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/access_group/access_group_volumes.py` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/access_group/access_group_volumes.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/access_group/main.fmf` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/access_group/main.fmf`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/fs/fs_clone.py` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/fs/fs_clone.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/fs/fs_create.py` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/fs/fs_create.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/fs/fs_delete.py` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/fs/fs_delete.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/fs/fs_dependants.py` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/fs/fs_dependants.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/fs/fs_dependants_rm.py` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/fs/fs_dependants_rm.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/fs/fs_export.py` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/fs/fs_export.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/fs/fs_resize.py` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/fs/fs_resize.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/fs/fs_snap_create.py` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/fs/fs_snap_create.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/fs/fs_snap_delete.py` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/fs/fs_snap_delete.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/fs/fs_snap_restore.py` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/fs/fs_snap_restore.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/fs/fs_unexport.py` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/fs/fs_unexport.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/fs/main.fmf` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/fs/main.fmf`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/list/access_groups.py` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/list/access_groups.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/list/batteries.py` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/list/batteries.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/list/disks.py` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/list/disks.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/list/exports.py` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/list/exports.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/list/fs.py` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/list/fs.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/list/main.fmf` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/list/main.fmf`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/list/nsf_client_auth.py` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/list/nsf_client_auth.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/list/plugins.py` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/list/plugins.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/list/pools.py` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/list/pools.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/list/snapshots.py` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/list/snapshots.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/list/systems.py` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/list/systems.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/list/target_ports.py` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/list/target_ports.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/list/volumes.py` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/list/volumes.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/local_disk/local_disk_fault_led.py` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/local_disk/local_disk_fault_led.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/local_disk/local_disk_ident_led.py` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/local_disk/local_disk_ident_led.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/local_disk/local_disk_list.py` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/local_disk/local_disk_list.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/local_disk/main.fmf` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/local_disk/main.fmf`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/various_commands/capabilities.py` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/various_commands/capabilities.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/various_commands/iscsi_chap.py` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/various_commands/iscsi_chap.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/various_commands/main.fmf` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/various_commands/main.fmf`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/various_commands/plugin_info.py` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/various_commands/plugin_info.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/various_commands/pool_member_info.py` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/various_commands/pool_member_info.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/various_commands/system_read_cache_pct_update.py` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/various_commands/system_read_cache_pct_update.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/volume/main.fmf` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/volume/main.fmf`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/volume/volume_access_group.py` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/volume/volume_access_group.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/volume/volume_cache_info.py` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/volume/volume_cache_info.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/volume/volume_create.py` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/volume/volume_create.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/volume/volume_delete.py` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/volume/volume_delete.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/volume/volume_dependants.py` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/volume/volume_dependants.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/volume/volume_dependants_rm.py` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/volume/volume_dependants_rm.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/volume/volume_disable.py` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/volume/volume_disable.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/volume/volume_enable.py` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/volume/volume_enable.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/volume/volume_ident_led.py` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/volume/volume_ident_led.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/volume/volume_mask.py` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/volume/volume_mask.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/volume/volume_phy_disk_cache_update.py` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/volume/volume_phy_disk_cache_update.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/volume/volume_read_cache_policy_update.py` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/volume/volume_read_cache_policy_update.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/volume/volume_replicate.py` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/volume/volume_replicate.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/volume/volume_replicate_range.py` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/volume/volume_replicate_range.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/volume/volume_replicate_range_block_size.py` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/volume/volume_replicate_range_block_size.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/volume/volume_unmask.py` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/volume/volume_unmask.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/lsmcli/volume/volume_write_cache_policy_update.py` & `stqe-0.2.4/stqe/tests/lsm/lsmcli/volume/volume_write_cache_policy_update.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/setup/cleanup_configure.py` & `stqe-0.2.4/stqe/tests/lsm/setup/cleanup_configure.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/setup/cleanup_storage.py` & `stqe-0.2.4/stqe/tests/lsm/setup/cleanup_storage.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/setup/clone_fs.py` & `stqe-0.2.4/stqe/tests/lsm/setup/clone_fs.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/setup/configure_lsm.py` & `stqe-0.2.4/stqe/tests/lsm/setup/configure_lsm.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/setup/create_access_group.py` & `stqe-0.2.4/stqe/tests/lsm/setup/create_access_group.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/setup/create_fs.py` & `stqe-0.2.4/stqe/tests/lsm/setup/create_fs.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/setup/create_fs_snap.py` & `stqe-0.2.4/stqe/tests/lsm/setup/create_fs_snap.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/setup/create_volume.py` & `stqe-0.2.4/stqe/tests/lsm/setup/create_volume.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/setup/export_fs.py` & `stqe-0.2.4/stqe/tests/lsm/setup/export_fs.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/setup/main.fmf` & `stqe-0.2.4/stqe/tests/lsm/setup/main.fmf`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/setup/mask_volume.py` & `stqe-0.2.4/stqe/tests/lsm/setup/mask_volume.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/setup/remove_access_group.py` & `stqe-0.2.4/stqe/tests/lsm/setup/remove_access_group.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/setup/remove_fs.py` & `stqe-0.2.4/stqe/tests/lsm/setup/remove_fs.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/setup/remove_fs_snap.py` & `stqe-0.2.4/stqe/tests/lsm/setup/remove_fs_snap.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/setup/remove_volume.py` & `stqe-0.2.4/stqe/tests/lsm/setup/remove_volume.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/setup/unexport_fs.py` & `stqe-0.2.4/stqe/tests/lsm/setup/unexport_fs.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lsm/setup/unmask_volume.py` & `stqe-0.2.4/stqe/tests/lsm/setup/unmask_volume.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lvm/cache/cache_basic.py` & `stqe-0.2.4/stqe/tests/lvm/cache/cache_basic.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lvm/device_mapper_persistent_data/BZ1456019.py` & `stqe-0.2.4/stqe/tests/lvm/device_mapper_persistent_data/BZ1456019.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lvm/device_mapper_persistent_data/cache.fmf` & `stqe-0.2.4/stqe/tests/lvm/device_mapper_persistent_data/cache.fmf`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lvm/device_mapper_persistent_data/cache.py` & `stqe-0.2.4/stqe/tests/lvm/device_mapper_persistent_data/cache.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lvm/device_mapper_persistent_data/cli.py` & `stqe-0.2.4/stqe/tests/lvm/device_mapper_persistent_data/cli.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lvm/device_mapper_persistent_data/restore_corrupting_metadata.py` & `stqe-0.2.4/stqe/tests/lvm/device_mapper_persistent_data/restore_corrupting_metadata.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lvm/device_mapper_persistent_data/thin.fmf` & `stqe-0.2.4/stqe/tests/lvm/device_mapper_persistent_data/thin.fmf`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lvm/device_mapper_persistent_data/thin.py` & `stqe-0.2.4/stqe/tests/lvm/device_mapper_persistent_data/thin.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lvm/device_mapper_persistent_data/tools_not_linked_usr.py` & `stqe-0.2.4/stqe/tests/lvm/device_mapper_persistent_data/tools_not_linked_usr.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lvm/setup/main.fmf` & `stqe-0.2.4/stqe/tests/lvm/setup/main.fmf`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lvm/setup/setup.py` & `stqe-0.2.4/stqe/tests/lvm/setup/setup.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lvm/setup/storage/cleanup_crypt.py` & `stqe-0.2.4/stqe/tests/lvm/setup/storage/cleanup_crypt.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lvm/setup/storage/cleanup_fcoe.py` & `stqe-0.2.4/stqe/tests/lvm/setup/storage/cleanup_fcoe.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lvm/setup/storage/cleanup_iscsi.py` & `stqe-0.2.4/stqe/tests/lvm/setup/storage/cleanup_iscsi.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lvm/setup/storage/cleanup_multipath.py` & `stqe-0.2.4/stqe/tests/lvm/setup/storage/cleanup_multipath.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lvm/setup/storage/cleanup_raid.py` & `stqe-0.2.4/stqe/tests/lvm/setup/storage/cleanup_raid.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lvm/setup/storage/main.fmf` & `stqe-0.2.4/stqe/tests/lvm/setup/storage/main.fmf`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lvm/setup/storage/setup_crypt.py` & `stqe-0.2.4/stqe/tests/lvm/setup/storage/setup_crypt.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lvm/setup/storage/setup_fcoe.py` & `stqe-0.2.4/stqe/tests/lvm/setup/storage/setup_fcoe.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lvm/setup/storage/setup_iscsi.py` & `stqe-0.2.4/stqe/tests/lvm/setup/storage/setup_iscsi.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lvm/setup/storage/setup_manual.py` & `stqe-0.2.4/stqe/tests/lvm/setup/storage/setup_manual.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lvm/setup/storage/setup_multipath.py` & `stqe-0.2.4/stqe/tests/lvm/setup/storage/setup_multipath.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lvm/setup/storage/setup_raid.py` & `stqe-0.2.4/stqe/tests/lvm/setup/storage/setup_raid.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lvm/snapper/snapper_basic.py` & `stqe-0.2.4/stqe/tests/lvm/snapper/snapper_basic.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lvm/thinp/discard-perf.py` & `stqe-0.2.4/stqe/tests/lvm/thinp/discard-perf.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lvm/thinp/exceed_pool_capacity.py` & `stqe-0.2.4/stqe/tests/lvm/thinp/exceed_pool_capacity.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lvm/thinp/lvchange-thin.py` & `stqe-0.2.4/stqe/tests/lvm/thinp/lvchange-thin.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lvm/thinp/lvconf-thinp.py` & `stqe-0.2.4/stqe/tests/lvm/thinp/lvconf-thinp.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lvm/thinp/lvconvert-thin-lv.py` & `stqe-0.2.4/stqe/tests/lvm/thinp/lvconvert-thin-lv.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lvm/thinp/lvconvert-thinpool.py` & `stqe-0.2.4/stqe/tests/lvm/thinp/lvconvert-thinpool.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lvm/thinp/lvcreate-liner.py` & `stqe-0.2.4/stqe/tests/lvm/thinp/lvcreate-liner.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lvm/thinp/lvcreate-mirror.py` & `stqe-0.2.4/stqe/tests/lvm/thinp/lvcreate-mirror.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lvm/thinp/lvcreate-poolmetadataspare.py` & `stqe-0.2.4/stqe/tests/lvm/thinp/lvcreate-poolmetadataspare.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lvm/thinp/lvcreate-stripe.py` & `stqe-0.2.4/stqe/tests/lvm/thinp/lvcreate-stripe.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lvm/thinp/lvextend-thinp.py` & `stqe-0.2.4/stqe/tests/lvm/thinp/lvextend-thinp.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lvm/thinp/lvm-thinp-misc.py` & `stqe-0.2.4/stqe/tests/lvm/thinp/lvm-thinp-misc.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lvm/thinp/lvm-thinp-modules.py` & `stqe-0.2.4/stqe/tests/lvm/thinp/lvm-thinp-modules.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lvm/thinp/lvreduce-thinp.py` & `stqe-0.2.4/stqe/tests/lvm/thinp/lvreduce-thinp.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lvm/thinp/lvremove-thinp.py` & `stqe-0.2.4/stqe/tests/lvm/thinp/lvremove-thinp.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lvm/thinp/lvrename-thinp.py` & `stqe-0.2.4/stqe/tests/lvm/thinp/lvrename-thinp.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lvm/thinp/lvresize-thinp.py` & `stqe-0.2.4/stqe/tests/lvm/thinp/lvresize-thinp.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lvm/thinp/lvs-thinp.py` & `stqe-0.2.4/stqe/tests/lvm/thinp/lvs-thinp.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lvm/thinp/lvscan-thinp.py` & `stqe-0.2.4/stqe/tests/lvm/thinp/lvscan-thinp.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lvm/thinp/thin-perf.py` & `stqe-0.2.4/stqe/tests/lvm/thinp/thin-perf.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lvm/thinp/bugs/corrupt_metadata_bz1319937.py` & `stqe-0.2.4/stqe/tests/lvm/thinp/bugs/corrupt_metadata_bz1319937.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lvm/thinp/bugs/discard_corruption_BZ_918647.py` & `stqe-0.2.4/stqe/tests/lvm/thinp/bugs/discard_corruption_BZ_918647.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lvm/thinp/bugs/stripe-blkdiscard.py` & `stqe-0.2.4/stqe/tests/lvm/thinp/bugs/stripe-blkdiscard.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/lvm/thinp/bugs/thinpool_with_error_target_meta_bz1305983.py` & `stqe-0.2.4/stqe/tests/lvm/thinp/bugs/thinpool_with_error_target_meta_bz1305983.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/stratis/common/bz1754649_stratis_pid.py` & `stqe-0.2.4/stqe/tests/stratis/common/bz1754649_stratis_pid.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/stratis/common/main.fmf` & `stqe-0.2.4/stqe/tests/stratis/common/main.fmf`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/stratis/common/stratis_fs_limit.py` & `stqe-0.2.4/stqe/tests/stratis/common/stratis_fs_limit.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/stratis/common/stratis_pool_out_of_space.py` & `stqe-0.2.4/stqe/tests/stratis/common/stratis_pool_out_of_space.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/stratis/common/stratis_repeat_create_destroy.py` & `stqe-0.2.4/stqe/tests/stratis/common/stratis_repeat_create_destroy.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/stratis/common/verify_data_in_restarted_pool.py` & `stqe-0.2.4/stqe/tests/stratis/common/verify_data_in_restarted_pool.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/stratis/data/fio/basic_stress.py` & `stqe-0.2.4/stqe/tests/stratis/data/fio/basic_stress.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/stratis/setup/cache_disk.py` & `stqe-0.2.4/stqe/tests/stratis/setup/cache_disk.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/stratis/setup/key_set.py` & `stqe-0.2.4/stqe/tests/stratis/setup/key_set.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/stratis/setup/key_unset.py` & `stqe-0.2.4/stqe/tests/stratis/setup/key_unset.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/stratis/setup/main.fmf` & `stqe-0.2.4/stqe/tests/stratis/setup/main.fmf`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/stratis/setup/pool_bind.py` & `stqe-0.2.4/stqe/tests/stratis/setup/pool_bind.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/stratis/setup/pool_create.py` & `stqe-0.2.4/stqe/tests/stratis/setup/pool_create.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/stratis/setup/pool_destroy.py` & `stqe-0.2.4/stqe/tests/stratis/setup/pool_destroy.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/stratis/setup/pool_restart.py` & `stqe-0.2.4/stqe/tests/stratis/setup/pool_restart.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/stratis/setup/pool_unbind.py` & `stqe-0.2.4/stqe/tests/stratis/setup/pool_unbind.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/stratis/setup/setup.py` & `stqe-0.2.4/stqe/tests/stratis/setup/setup.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/stratis/setup/tang_server.py` & `stqe-0.2.4/stqe/tests/stratis/setup/tang_server.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/stratis/setup/storage/cleanup_crypt.py` & `stqe-0.2.4/stqe/tests/stratis/setup/storage/cleanup_crypt.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/stratis/setup/storage/cleanup_free_disks.py` & `stqe-0.2.4/stqe/tests/stratis/setup/storage/cleanup_free_disks.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/stratis/setup/storage/cleanup_iscsi.py` & `stqe-0.2.4/stqe/tests/stratis/setup/storage/cleanup_iscsi.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/stratis/setup/storage/cleanup_loopdev.py` & `stqe-0.2.4/stqe/tests/stratis/setup/storage/cleanup_loopdev.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/stratis/setup/storage/cleanup_lvm.py` & `stqe-0.2.4/stqe/tests/stratis/setup/storage/cleanup_lvm.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/stratis/setup/storage/cleanup_raid.py` & `stqe-0.2.4/stqe/tests/stratis/setup/storage/cleanup_raid.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/stratis/setup/storage/main.fmf` & `stqe-0.2.4/stqe/tests/stratis/setup/storage/main.fmf`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/stratis/setup/storage/setup_crypt.py` & `stqe-0.2.4/stqe/tests/stratis/setup/storage/setup_crypt.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/stratis/setup/storage/setup_free_disks.py` & `stqe-0.2.4/stqe/tests/stratis/setup/storage/setup_free_disks.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/stratis/setup/storage/setup_iscsi.py` & `stqe-0.2.4/stqe/tests/stratis/setup/storage/setup_iscsi.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/stratis/setup/storage/setup_loopdev.py` & `stqe-0.2.4/stqe/tests/stratis/setup/storage/setup_loopdev.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/stratis/setup/storage/setup_lvm.py` & `stqe-0.2.4/stqe/tests/stratis/setup/storage/setup_lvm.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/stratis/setup/storage/setup_manual.py` & `stqe-0.2.4/stqe/tests/stratis/setup/storage/setup_manual.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/stratis/setup/storage/setup_raid.py` & `stqe-0.2.4/stqe/tests/stratis/setup/storage/setup_raid.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/stratis/stratis_cli/blockdev.fmf` & `stqe-0.2.4/stqe/tests/stratis/stratis_cli/blockdev.fmf`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/stratis/stratis_cli/fs.fmf` & `stqe-0.2.4/stqe/tests/stratis/stratis_cli/fs.fmf`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/stratis/stratis_cli/key.fmf` & `stqe-0.2.4/stqe/tests/stratis/stratis_cli/key.fmf`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/stratis/stratis_cli/pool.fmf` & `stqe-0.2.4/stqe/tests/stratis/stratis_cli/pool.fmf`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/stratis/stratis_cli/stratis_cli.py` & `stqe-0.2.4/stqe/tests/stratis/stratis_cli/stratis_cli.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/targetcli/python-kmod.py` & `stqe-0.2.4/stqe/tests/targetcli/python-kmod.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/targetcli/cli/block_attributes.py` & `stqe-0.2.4/stqe/tests/targetcli/cli/block_attributes.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/targetcli/cli/create_pscsi.py` & `stqe-0.2.4/stqe/tests/targetcli/cli/create_pscsi.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/targetcli/cli/fileio_attributes.py` & `stqe-0.2.4/stqe/tests/targetcli/cli/fileio_attributes.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/targetcli/cli/iscsi_chap.py` & `stqe-0.2.4/stqe/tests/targetcli/cli/iscsi_chap.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/targetcli/cli/iscsi_chap_2ways.py` & `stqe-0.2.4/stqe/tests/targetcli/cli/iscsi_chap_2ways.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/targetcli/cli/iscsi_local_target.py` & `stqe-0.2.4/stqe/tests/targetcli/cli/iscsi_local_target.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/targetcli/cli/main.fmf` & `stqe-0.2.4/stqe/tests/targetcli/cli/main.fmf`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/targetcli/cli/ramdisk_attributes.py` & `stqe-0.2.4/stqe/tests/targetcli/cli/ramdisk_attributes.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/targetcli/cli/saveconfig_backup.py` & `stqe-0.2.4/stqe/tests/targetcli/cli/saveconfig_backup.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/targetcli/cli/saveconfig_compare.py` & `stqe-0.2.4/stqe/tests/targetcli/cli/saveconfig_compare.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/targetcli/setup/configure_chap.py` & `stqe-0.2.4/stqe/tests/targetcli/setup/configure_chap.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/targetcli/setup/create_backstore.py` & `stqe-0.2.4/stqe/tests/targetcli/setup/create_backstore.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/targetcli/setup/create_fileio_target.py` & `stqe-0.2.4/stqe/tests/targetcli/setup/create_fileio_target.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/targetcli/setup/create_loopback.py` & `stqe-0.2.4/stqe/tests/targetcli/setup/create_loopback.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/targetcli/setup/create_loopdev.py` & `stqe-0.2.4/stqe/tests/targetcli/setup/create_loopdev.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/targetcli/setup/create_qcow.py` & `stqe-0.2.4/stqe/tests/targetcli/setup/create_qcow.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/targetcli/setup/create_qcow_target.py` & `stqe-0.2.4/stqe/tests/targetcli/setup/create_qcow_target.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/targetcli/setup/create_saveconfig.py` & `stqe-0.2.4/stqe/tests/targetcli/setup/create_saveconfig.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/targetcli/setup/delete_backstore.py` & `stqe-0.2.4/stqe/tests/targetcli/setup/delete_backstore.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/targetcli/setup/delete_iscsi_target.py` & `stqe-0.2.4/stqe/tests/targetcli/setup/delete_iscsi_target.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/targetcli/setup/delete_loopback.py` & `stqe-0.2.4/stqe/tests/targetcli/setup/delete_loopback.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/targetcli/setup/delete_qcow.py` & `stqe-0.2.4/stqe/tests/targetcli/setup/delete_qcow.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/targetcli/setup/disable_chap.py` & `stqe-0.2.4/stqe/tests/targetcli/setup/disable_chap.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/targetcli/setup/install_tcmu_runner.py` & `stqe-0.2.4/stqe/tests/targetcli/setup/install_tcmu_runner.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/targetcli/setup/main.fmf` & `stqe-0.2.4/stqe/tests/targetcli/setup/main.fmf`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/targetcli/setup/start_multipath.py` & `stqe-0.2.4/stqe/tests/targetcli/setup/start_multipath.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/targetcli/setup/stop_multipath.py` & `stqe-0.2.4/stqe/tests/targetcli/setup/stop_multipath.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/targetd/setup/create_loopdev.py` & `stqe-0.2.4/stqe/tests/targetd/setup/create_loopdev.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/targetd/setup/prepare_conf.py` & `stqe-0.2.4/stqe/tests/targetd/setup/prepare_conf.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/targetd/targetd_basic/main.fmf` & `stqe-0.2.4/stqe/tests/targetd/targetd_basic/main.fmf`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/targetd/targetd_basic/targetd_basic.py` & `stqe-0.2.4/stqe/tests/targetd/targetd_basic/targetd_basic.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/targetd/targetd_basic/targetd_no_passwd.py` & `stqe-0.2.4/stqe/tests/targetd/targetd_basic/targetd_no_passwd.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/targetd/targetd_basic/targetd_no_vg.py` & `stqe-0.2.4/stqe/tests/targetd/targetd_basic/targetd_no_vg.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/targetd/targetd_basic/targetd_ssl.py` & `stqe-0.2.4/stqe/tests/targetd/targetd_basic/targetd_ssl.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/targetd/targetd_basic/targetd_ssl_no_cert.py` & `stqe-0.2.4/stqe/tests/targetd/targetd_basic/targetd_ssl_no_cert.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/targetd/targetd_basic/targetd_ssl_no_key.py` & `stqe-0.2.4/stqe/tests/targetd/targetd_basic/targetd_ssl_no_key.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/vdo/data/main.fmf` & `stqe-0.2.4/stqe/tests/vdo/data/main.fmf`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/vdo/data/repeated_copy.py` & `stqe-0.2.4/stqe/tests/vdo/data/repeated_copy.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/vdo/data/fio/basic_stress.py` & `stqe-0.2.4/stqe/tests/vdo/data/fio/basic_stress.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/vdo/data/fio/fs.py` & `stqe-0.2.4/stqe/tests/vdo/data/fio/fs.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/vdo/data/fio/main.fmf` & `stqe-0.2.4/stqe/tests/vdo/data/fio/main.fmf`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/vdo/data/fio/vdo_on_vdo.py` & `stqe-0.2.4/stqe/tests/vdo/data/fio/vdo_on_vdo.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/vdo/kernel_modules/kvdo.py` & `stqe-0.2.4/stqe/tests/vdo/kernel_modules/kvdo.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/vdo/kernel_modules/signatures.py` & `stqe-0.2.4/stqe/tests/vdo/kernel_modules/signatures.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/vdo/kernel_modules/uds.py` & `stqe-0.2.4/stqe/tests/vdo/kernel_modules/uds.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/vdo/setup/data.fmf` & `stqe-0.2.4/stqe/tests/vdo/setup/data.fmf`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/vdo/setup/main.fmf` & `stqe-0.2.4/stqe/tests/vdo/setup/main.fmf`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/vdo/setup/setup.py` & `stqe-0.2.4/stqe/tests/vdo/setup/setup.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/vdo/setup/storage/cleanup_crypt.py` & `stqe-0.2.4/stqe/tests/vdo/setup/storage/cleanup_crypt.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/vdo/setup/storage/cleanup_fcoe.py` & `stqe-0.2.4/stqe/tests/vdo/setup/storage/cleanup_fcoe.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/vdo/setup/storage/cleanup_iscsi.py` & `stqe-0.2.4/stqe/tests/vdo/setup/storage/cleanup_iscsi.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/vdo/setup/storage/cleanup_multipath.py` & `stqe-0.2.4/stqe/tests/vdo/setup/storage/cleanup_multipath.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/vdo/setup/storage/cleanup_raid.py` & `stqe-0.2.4/stqe/tests/vdo/setup/storage/cleanup_raid.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/vdo/setup/storage/main.fmf` & `stqe-0.2.4/stqe/tests/vdo/setup/storage/main.fmf`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/vdo/setup/storage/setup_crypt.py` & `stqe-0.2.4/stqe/tests/vdo/setup/storage/setup_crypt.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/vdo/setup/storage/setup_fcoe.py` & `stqe-0.2.4/stqe/tests/vdo/setup/storage/setup_fcoe.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/vdo/setup/storage/setup_iscsi.py` & `stqe-0.2.4/stqe/tests/vdo/setup/storage/setup_iscsi.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/vdo/setup/storage/setup_manual.py` & `stqe-0.2.4/stqe/tests/vdo/setup/storage/setup_manual.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/vdo/setup/storage/setup_multipath.py` & `stqe-0.2.4/stqe/tests/vdo/setup/storage/setup_multipath.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/vdo/setup/storage/setup_raid.py` & `stqe-0.2.4/stqe/tests/vdo/setup/storage/setup_raid.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/vdo/vdo_cli/create.fmf` & `stqe-0.2.4/stqe/tests/vdo/vdo_cli/create.fmf`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/vdo/vdo_cli/modify.fmf` & `stqe-0.2.4/stqe/tests/vdo/vdo_cli/modify.fmf`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/vdo/vdo_cli/various_commands.fmf` & `stqe-0.2.4/stqe/tests/vdo/vdo_cli/various_commands.fmf`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/stqe/tests/vdo/vdo_cli/vdo_cli.py` & `stqe-0.2.4/stqe/tests/vdo/vdo_cli/vdo_cli.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/tests/augeas_test.py` & `stqe-0.2.4/tests/augeas_test.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/tests/logchecker_test.py` & `stqe-0.2.4/tests/logchecker_test.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/tests/persistent_vars_test.py` & `stqe-0.2.4/tests/persistent_vars_test.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/tests/tc_test.py` & `stqe-0.2.4/tests/tc_test.py`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/LICENSE` & `stqe-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/pyproject.toml` & `stqe-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `stqe-0.2.3/PKG-INFO` & `stqe-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: stqe
-Version: 0.2.3
+Version: 0.2.4
 Summary: Python modules to manage SAN devices
 Project-URL: Repository, https://gitlab.com/rh-kernel-stqe/python-stqe
 Author: Jakub Krysl
 Author-email: Bruno Goncalves <bgoncalv@redhat.com>
 Maintainer-email: Bruno Goncalves <bgoncalv@redhat.com>, Martin Hoyer <mhoyer@redhat.com>, Filip Suba <fsuba@redhat.com>
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE
```

