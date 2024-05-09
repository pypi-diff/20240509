# Comparing `tmp/backup_helper-0.2.1-py3-none-any.whl.zip` & `tmp/backup_helper-0.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 22632 bytes, number of entries: 17
+Zip file size: 22787 bytes, number of entries: 17
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-28 21:19 backup_helper/__init__.py
 -rw-rw-rw-  2.0 fat      134 b- defN 24-May-07 23:46 backup_helper/__main__.py
--rw-rw-rw-  2.0 fat     6243 b- defN 24-May-08 17:56 backup_helper/backup_helper.py
+-rw-rw-rw-  2.0 fat     6274 b- defN 24-May-09 00:33 backup_helper/backup_helper.py
 -rw-rw-rw-  2.0 fat    14150 b- defN 24-May-07 23:46 backup_helper/cli.py
--rw-rw-rw-  2.0 fat    10726 b- defN 24-May-08 19:04 backup_helper/disk_work_queue.py
+-rw-rw-rw-  2.0 fat    10819 b- defN 24-May-09 00:58 backup_helper/disk_work_queue.py
 -rw-rw-rw-  2.0 fat     1378 b- defN 23-Aug-07 19:34 backup_helper/exceptions.py
 -rw-rw-rw-  2.0 fat     2632 b- defN 23-Aug-05 15:57 backup_helper/helpers.py
 -rw-rw-rw-  2.0 fat     6413 b- defN 24-May-07 23:46 backup_helper/interactive.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-28 21:21 backup_helper/py.typed
--rw-rw-rw-  2.0 fat    11994 b- defN 23-Sep-03 20:03 backup_helper/source.py
+-rw-rw-rw-  2.0 fat    12285 b- defN 24-May-09 00:43 backup_helper/source.py
 -rw-rw-rw-  2.0 fat     4216 b- defN 24-May-07 23:50 backup_helper/target.py
--rw-rw-rw-  2.0 fat     4593 b- defN 24-May-08 19:10 backup_helper/work.py
--rw-rw-rw-  2.0 fat     4588 b- defN 24-May-08 19:20 backup_helper-0.2.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-08 19:20 backup_helper-0.2.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       62 b- defN 24-May-08 19:20 backup_helper-0.2.1.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       14 b- defN 24-May-08 19:20 backup_helper-0.2.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1403 b- defN 24-May-08 19:20 backup_helper-0.2.1.dist-info/RECORD
-17 files, 68638 bytes uncompressed, 20322 bytes compressed:  70.4%
+-rw-rw-rw-  2.0 fat     4745 b- defN 24-May-09 01:07 backup_helper/work.py
+-rw-rw-rw-  2.0 fat     4588 b- defN 24-May-09 01:40 backup_helper-0.2.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-09 01:40 backup_helper-0.2.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       62 b- defN 24-May-09 01:40 backup_helper-0.2.2.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       14 b- defN 24-May-09 01:40 backup_helper-0.2.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1403 b- defN 24-May-09 01:40 backup_helper-0.2.2.dist-info/RECORD
+17 files, 69205 bytes uncompressed, 20477 bytes compressed:  70.4%
```

## zipnote {}

```diff
@@ -30,23 +30,23 @@
 
 Filename: backup_helper/target.py
 Comment: 
 
 Filename: backup_helper/work.py
 Comment: 
 
-Filename: backup_helper-0.2.1.dist-info/METADATA
+Filename: backup_helper-0.2.2.dist-info/METADATA
 Comment: 
 
-Filename: backup_helper-0.2.1.dist-info/WHEEL
+Filename: backup_helper-0.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: backup_helper-0.2.1.dist-info/entry_points.txt
+Filename: backup_helper-0.2.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: backup_helper-0.2.1.dist-info/top_level.txt
+Filename: backup_helper-0.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: backup_helper-0.2.1.dist-info/RECORD
+Filename: backup_helper-0.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## backup_helper/backup_helper.py

```diff
@@ -137,14 +137,15 @@
 
     def start_all(self) -> None:
         for src in self.unique_sources():
             src.hash_queue(self._queue, log_dir=self._working_dir)
             src.transfer_queue_all(self._queue)
             src.verify_target_queue_all(self._queue)
 
+        # TODO errors missing?
         success, errors = self._queue.start_and_join_all()
         work.report_results(success, errors)
 
     def workers_running(self) -> bool:
         return self._queue.workers_running()
 
     def join(self) -> None:
```

## backup_helper/disk_work_queue.py

```diff
@@ -178,15 +178,16 @@
 
         now = time.time()
         if now - self._last_report < self._report_progress_timestep_seconds:
             return
         self._last_report = now
 
         for work in self._work:
-            if work.started:
+            if work.started and not any(
+                    work_result.work is work for work_result in self._finished):
                 print("Active job:", work.work)
 
     def _wait_till_one_thread_finished_and_update(self):
         """
         Blocks until at least one item is retrieved from the Queue.
         Then updates it.
         """
```

## backup_helper/source.py

```diff
@@ -101,21 +101,23 @@
         # targets contain both path as well as alias as keys, so we have to
         # deduplicate them
         yield from helpers.unique_iterator(self.targets.values())
 
     def add_target(self, target: Target):
         if target.path in self.targets:
             raise TargetAlreadyExists(
-                f"Target '{target.path}' already exists on source '{self.path}'!",
+                f"Target '{target.path}' already exists on source '{
+                    self.path}'!",
                 self.path, target.path)
         self.targets[target.path] = target
         if target.alias:
             if target.alias in self.targets:
                 raise AliasAlreadyExists(
-                    f"Alias '{target.alias}' already exists on source '{self.path}'!",
+                    f"Alias '{target.alias}' already exists on source '{
+                        self.path}'!",
                     target.alias)
             self.targets[target.alias] = target
 
     def get_target(self, target_key: str) -> Target:
         try:
             return self.targets[target_key]
         except KeyError:
@@ -215,19 +217,24 @@
         # or you get interrupted by antivirus
         # -> return list of skipped files
         # -> already handled by copytree, where all errors get raised at the
         #    end as part of shutil.Error
         logger.info("Tranferring %s to %s on thread %d ...",
                     self.path, target.path, threading.get_ident())
 
+        # TODO: support path > 256 on windows?
         try:
             shutil.copytree(self.path, target.path, dirs_exist_ok=True,
                             ignore=self._create_fnmatch_ignore())
         except shutil.Error as e:
             # e.args[0] contains a list of 3-tuples with (src, dst, error)
+            # TODO: retry?
+            # TODO: return errors so they can be reported/logged
+            # TODO: separate log for transfers as well?
+            #       OR TODO no limit on log files
             logger.warning(
                 "Failed to copy the following files when transferring '%s' "
                 "to '%s':\n%s",
                 self.path, target.path,
                 "\n".join(f"{err}: {src} -> {dst}" for src,
                           dst, err in e.args[0]))
         else:
```

## backup_helper/work.py

 * *Ordering differences only*

```diff
@@ -1,152 +1,152 @@
-import dataclasses
-import enum
-import logging
-import os
-
-from typing import Optional, TYPE_CHECKING, Final, List, Union, Tuple, cast
-
-if TYPE_CHECKING:
-    from backup_helper.source import Source
-    from backup_helper.target import Target, VerifiedInfo
-
-from backup_helper.disk_work_queue import DiskWorkQueue
-
-
-logger = logging.getLogger(__name__)
-
-
-@dataclasses.dataclass
-class WorkHash:
-    source: 'Source'
-    log_dir: str
-
-    # whether it's dependencies have completed
-    def is_ready(self) -> bool:
-        return True
-
-    def get_involved_paths(self) -> List[str]:
-        return [self.source.path]
-
-    def do_work(self):
-        self.source.hash(log_directory=self.log_dir)
-        return self
-
-    def report_success(self) -> str:
-        return (f"Hashed '{self.source.path}':\n"
-                f"  Hash file: {self.source.hash_file}")
-
-    def report_error(self) -> str:
-        return f"Error hashing '{self.source.path}'!"
-
-    def __str__(self) -> str:
-        return f"Hashing '{self.source.path}'"
-
-
-@dataclasses.dataclass
-class WorkTransfer:
-    source: 'Source'
-    target: 'Target'
-
-    # whether it's dependencies have completed
-    def is_ready(self) -> bool:
-        # we don't need a hash file on source if the target should not be
-        # verified
-        return not self.target.verify or bool(self.source.hash_file)
-
-    def get_involved_paths(self) -> List[str]:
-        return [self.source.path, self.target.path]
-
-    def do_work(self):
-        self.source.transfer(self.target)
-        return self
-
-    def report_success(self) -> str:
-        return (f"Transfer successful:\n"
-                f"  From: {self.source.path}\n"
-                f"  To: {self.target.path}")
-
-    def report_error(self) -> str:
-        return ("Error transfering:\n"
-                f"  From: {self.source.path}\n"
-                f"  To: {self.target.path}")
-
-    def __str__(self) -> str:
-        return f"Transferring\n\t'{self.source.path}'\n\t-> '{self.target.path}'"
-
-
-@dataclasses.dataclass
-class WorkVerifyTransfer:
-    source: 'Source'
-    target: 'Target'
-
-    # whether it's dependencies have completed
-    def is_ready(self) -> bool:
-        # we don't need a hash file on source if the target should not be verified
-        return self.target.transfered and (
-            not self.target.verify or bool(self.source.hash_file))
-
-    def get_involved_paths(self) -> List[str]:
-        return [self.target.path]
-
-    def do_work(self):
-        self.target.verify_from(self.source.hash_file)
-        return self
-
-    def report_success(self) -> str:
-        cast('VerifiedInfo', self.target.verified)
-        return (f"Verified transfer '{self.target.path}':\n"
-                f"  Checked: {self.target.verified.checked}\n"
-                f"  CRC Errors: {self.target.verified.crc_errors}\n"
-                f"  Missing: {self.target.verified.missing}")
-
-    def report_error(self) -> str:
-        return f"Error verifying '{self.target.path}'!"
-
-    def __str__(self) -> str:
-        if not self.source.hash_file:
-            return f"Waiting for source hash file in {self.source.path}"
-
-        hash_file = os.path.join(
-            self.target.path, os.path.basename(self.source.hash_file))
-        return f"Verifying '{hash_file}'"
-
-
-WorkType = Union[WorkHash, WorkTransfer, WorkVerifyTransfer]
-WorkResult = WorkType
-WorkQueue = DiskWorkQueue[WorkType, WorkResult]
-
-
-def get_involved_paths(work: WorkType) -> List[str]:
-    return work.get_involved_paths()
-
-
-def do_work(work: WorkType) -> WorkResult:
-    return work.do_work()
-
-
-def is_ready(work: WorkType) -> bool:
-    return work.is_ready()
-
-
-def setup_work_queue(work_items: List[WorkType]) -> WorkQueue:
-    return WorkQueue(get_involved_paths, do_work, is_ready,
-                     report_progress_timestep_seconds=60,
-                     work=work_items)
-
-
-def report_results(success: List[WorkType], errors: List[Tuple[WorkType, str]]):
-    if success:
-        logger.info(
-            "Successfully completed the following %d operation(s):\n%s",
-            len(success),
-            "\n".join(w.report_success() for w in success))
-    if errors:
-        logger.warning(
-            "Failed to complete the following %d operation(s):\n%s",
-            len(errors), "\n".join(f"{w.report_error()}:\n Error: {err}"
-                                   for w, err in errors))
-
-    if not success and not errors:
-        logger.info("No operations were run maybe you forgot to run a "
-                    "previous step, e.g. sources cannot be transfered until "
-                    "they were hashed!")
+import dataclasses
+import enum
+import logging
+import os
+
+from typing import Optional, TYPE_CHECKING, Final, List, Union, Tuple, cast
+
+if TYPE_CHECKING:
+    from backup_helper.source import Source
+    from backup_helper.target import Target, VerifiedInfo
+
+from backup_helper.disk_work_queue import DiskWorkQueue
+
+
+logger = logging.getLogger(__name__)
+
+
+@dataclasses.dataclass
+class WorkHash:
+    source: 'Source'
+    log_dir: str
+
+    # whether it's dependencies have completed
+    def is_ready(self) -> bool:
+        return True
+
+    def get_involved_paths(self) -> List[str]:
+        return [self.source.path]
+
+    def do_work(self):
+        self.source.hash(log_directory=self.log_dir)
+        return self
+
+    def report_success(self) -> str:
+        return (f"Hashed '{self.source.path}':\n"
+                f"  Hash file: {self.source.hash_file}")
+
+    def report_error(self) -> str:
+        return f"Error hashing '{self.source.path}'!"
+
+    def __str__(self) -> str:
+        return f"Hashing '{self.source.path}'"
+
+
+@dataclasses.dataclass
+class WorkTransfer:
+    source: 'Source'
+    target: 'Target'
+
+    # whether it's dependencies have completed
+    def is_ready(self) -> bool:
+        # we don't need a hash file on source if the target should not be
+        # verified
+        return not self.target.verify or bool(self.source.hash_file)
+
+    def get_involved_paths(self) -> List[str]:
+        return [self.source.path, self.target.path]
+
+    def do_work(self):
+        self.source.transfer(self.target)
+        return self
+
+    def report_success(self) -> str:
+        return (f"Transfer successful:\n"
+                f"  From: {self.source.path}\n"
+                f"  To: {self.target.path}")
+
+    def report_error(self) -> str:
+        return ("Error transfering:\n"
+                f"  From: {self.source.path}\n"
+                f"  To: {self.target.path}")
+
+    def __str__(self) -> str:
+        return f"Transferring\n\t'{self.source.path}'\n\t-> '{self.target.path}'"
+
+
+@dataclasses.dataclass
+class WorkVerifyTransfer:
+    source: 'Source'
+    target: 'Target'
+
+    # whether it's dependencies have completed
+    def is_ready(self) -> bool:
+        # we don't need a hash file on source if the target should not be verified
+        return self.target.transfered and (
+            not self.target.verify or bool(self.source.hash_file))
+
+    def get_involved_paths(self) -> List[str]:
+        return [self.target.path]
+
+    def do_work(self):
+        self.target.verify_from(self.source.hash_file)
+        return self
+
+    def report_success(self) -> str:
+        cast('VerifiedInfo', self.target.verified)
+        return (f"Verified transfer '{self.target.path}':\n"
+                f"  Checked: {self.target.verified.checked}\n"
+                f"  CRC Errors: {self.target.verified.crc_errors}\n"
+                f"  Missing: {self.target.verified.missing}")
+
+    def report_error(self) -> str:
+        return f"Error verifying '{self.target.path}'!"
+
+    def __str__(self) -> str:
+        if not self.source.hash_file:
+            return f"Waiting for source hash file in {self.source.path}"
+
+        hash_file = os.path.join(
+            self.target.path, os.path.basename(self.source.hash_file))
+        return f"Verifying '{hash_file}'"
+
+
+WorkType = Union[WorkHash, WorkTransfer, WorkVerifyTransfer]
+WorkResult = WorkType
+WorkQueue = DiskWorkQueue[WorkType, WorkResult]
+
+
+def get_involved_paths(work: WorkType) -> List[str]:
+    return work.get_involved_paths()
+
+
+def do_work(work: WorkType) -> WorkResult:
+    return work.do_work()
+
+
+def is_ready(work: WorkType) -> bool:
+    return work.is_ready()
+
+
+def setup_work_queue(work_items: List[WorkType]) -> WorkQueue:
+    return WorkQueue(get_involved_paths, do_work, is_ready,
+                     report_progress_timestep_seconds=60,
+                     work=work_items)
+
+
+def report_results(success: List[WorkType], errors: List[Tuple[WorkType, str]]):
+    if success:
+        logger.info(
+            "Successfully completed the following %d operation(s):\n%s",
+            len(success),
+            "\n".join(w.report_success() for w in success))
+    if errors:
+        logger.warning(
+            "Failed to complete the following %d operation(s):\n%s",
+            len(errors), "\n".join(f"{w.report_error()}:\n Error: {err}"
+                                   for w, err in errors))
+
+    if not success and not errors:
+        logger.info("No operations were run maybe you forgot to run a "
+                    "previous step, e.g. sources cannot be transfered until "
+                    "they were hashed!")
```

## Comparing `backup_helper-0.2.1.dist-info/METADATA` & `backup_helper-0.2.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backup-helper
-Version: 0.2.1
+Version: 0.2.2
 Summary: Helper tool for creating plain-file cold-storage archives including checksum files
 Author-email: omgitsmoe <60219950+omgitsmoe@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/omgitsmoe/backup_helper
 Project-URL: Bug Tracker, https://github.com/omgitsmoe/backup_helper/issues
 Keywords: script,verify,backup,archival,bit-rot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `backup_helper-0.2.1.dist-info/RECORD` & `backup_helper-0.2.2.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 backup_helper/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 backup_helper/__main__.py,sha256=veMU3c-ZYmOGEs0FzOQoN7YVRd8iTwtu5u79lwe3R2U,134
-backup_helper/backup_helper.py,sha256=u8aS-ZUnBKIbV2Rk4SIUFXLBMPpcM4cL9cRpxsv0ZTg,6243
+backup_helper/backup_helper.py,sha256=g7RSgbwit2VWF6pHNhZSdS9IFklX1udNg_22UNbf1nk,6274
 backup_helper/cli.py,sha256=EBiCtr5c5818-UjbNhPGx1xPes_E8LthqNRoTU7yU24,14150
-backup_helper/disk_work_queue.py,sha256=ytUIiqhFdtqpXLmHjm-yonDCC6w_wOKiqdrZwIYxYeA,10726
+backup_helper/disk_work_queue.py,sha256=Ir1gsZscX6af5pu4AcKpvtBZkUznU4Ec3bOOUjyN4CA,10819
 backup_helper/exceptions.py,sha256=ZNPNxKg_U6HPD9omcuLbXXXBvYixh03Ew7ztFAlU5lE,1378
 backup_helper/helpers.py,sha256=F0A1-16fEy4QdYJIhKKVY9-sx_DZlSp6VhWsm6_VfTQ,2632
 backup_helper/interactive.py,sha256=NoUOYyouoQH7DbKW1NyB6WaYvKMcVOujgPk76LwadDU,6413
 backup_helper/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-backup_helper/source.py,sha256=AiizlDGRXZtpNEDQU3s2uZm832E6cn0Kf0iltlM3NFQ,11994
+backup_helper/source.py,sha256=FH8-J4a4kuVi8whgObMwVmlfhFwsPa3RopUxdsW6PWc,12285
 backup_helper/target.py,sha256=2K-SCROo5g82gppZZ_NzieTX02o1LU3OvZP5bFyt6Jo,4216
-backup_helper/work.py,sha256=KeOlzI_9i98s1CftZVZdtQzb3bnpQKc0fa6cJLB2Rfo,4593
-backup_helper-0.2.1.dist-info/METADATA,sha256=Ior-vW2b-Y4JFHNzGJ6BVPJ28KhxU2x37fmb9bCbisU,4588
-backup_helper-0.2.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-backup_helper-0.2.1.dist-info/entry_points.txt,sha256=XdFN-87n-MWUOVPAdpcJOkoU97dKaMAgS5rmmB_8D1Y,62
-backup_helper-0.2.1.dist-info/top_level.txt,sha256=XgSeNwprE6QO8VplFlrUfL-W8F3ujfSxm5ku60w3_xY,14
-backup_helper-0.2.1.dist-info/RECORD,,
+backup_helper/work.py,sha256=6-lSPnNP7rk7RcPcS0eJM7AmgR0ZUFE75uapkiojeMg,4745
+backup_helper-0.2.2.dist-info/METADATA,sha256=hAdgTYQEaHdTVle8niokEd4PuqLUqnt5VcyU4fYqCNQ,4588
+backup_helper-0.2.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+backup_helper-0.2.2.dist-info/entry_points.txt,sha256=XdFN-87n-MWUOVPAdpcJOkoU97dKaMAgS5rmmB_8D1Y,62
+backup_helper-0.2.2.dist-info/top_level.txt,sha256=XgSeNwprE6QO8VplFlrUfL-W8F3ujfSxm5ku60w3_xY,14
+backup_helper-0.2.2.dist-info/RECORD,,
```

