# Comparing `tmp/insulaclient-0.6.1-py3-none-any.whl.zip` & `tmp/insulaclient-0.6.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 23256 bytes, number of entries: 29
+Zip file size: 23314 bytes, number of entries: 29
 -rw-r--r--  2.0 fat     2765 b- defN 20-Feb-02 00:00 insulaClient/InsulaApiConfig.py
 -rw-r--r--  2.0 fat      565 b- defN 20-Feb-02 00:00 insulaClient/InsulaClient.py
 -rw-r--r--  2.0 fat      625 b- defN 20-Feb-02 00:00 insulaClient/InsulaQuery.py
 -rw-r--r--  2.0 fat     1365 b- defN 20-Feb-02 00:00 insulaClient/InsulaSearch.py
 -rw-r--r--  2.0 fat     1389 b- defN 20-Feb-02 00:00 insulaClient/SingletonMemoryManager.py
 -rw-r--r--  2.0 fat     1667 b- defN 20-Feb-02 00:00 insulaClient/WorkflowDataManager.py
 -rw-r--r--  2.0 fat      390 b- defN 20-Feb-02 00:00 insulaClient/__init__.py
@@ -15,17 +15,17 @@
 -rw-r--r--  2.0 fat     3153 b- defN 20-Feb-02 00:00 insulaClient/job_status.py
 -rw-r--r--  2.0 fat      262 b- defN 20-Feb-02 00:00 insulaClient/logger.py
 -rw-r--r--  2.0 fat     4617 b- defN 20-Feb-02 00:00 insulaClient/placeholders.py
 -rw-r--r--  2.0 fat     1341 b- defN 20-Feb-02 00:00 insulaClient/results_manager.py
 -rw-r--r--  2.0 fat     1894 b- defN 20-Feb-02 00:00 insulaClient/s3.py
 -rw-r--r--  2.0 fat      725 b- defN 20-Feb-02 00:00 insulaClient/step_result.py
 -rw-r--r--  2.0 fat      929 b- defN 20-Feb-02 00:00 insulaClient/utils.py
--rw-r--r--  2.0 fat     4630 b- defN 20-Feb-02 00:00 insulaClient/workflow.py
+-rw-r--r--  2.0 fat     4966 b- defN 20-Feb-02 00:00 insulaClient/workflow.py
 -rw-r--r--  2.0 fat     6449 b- defN 20-Feb-02 00:00 insulaClient/workflow_manager.py
 -rw-r--r--  2.0 fat      818 b- defN 20-Feb-02 00:00 insulaClient/workflow_step.py
 -rw-r--r--  2.0 fat    14627 b- defN 20-Feb-02 00:00 insulaClient/workflow_step_runner.py
-?rw-r--r--  2.0 fat     9984 b- defN 20-Feb-02 00:00 insulaclient-0.6.1.dist-info/METADATA
-?rw-r--r--  2.0 fat       87 b- defN 20-Feb-02 00:00 insulaclient-0.6.1.dist-info/WHEEL
-?rw-r--r--  2.0 fat       58 b- defN 20-Feb-02 00:00 insulaclient-0.6.1.dist-info/entry_points.txt
-?rw-r--r--  2.0 fat        0 b- defN 20-Feb-02 00:00 insulaclient-0.6.1.dist-info/licenses/LICENSE.txt
-?rw-r--r--  2.0 fat     2453 b- defN 20-Feb-02 00:00 insulaclient-0.6.1.dist-info/RECORD
-29 files, 70373 bytes uncompressed, 19290 bytes compressed:  72.6%
+?rw-r--r--  2.0 fat     9984 b- defN 20-Feb-02 00:00 insulaclient-0.6.2.dist-info/METADATA
+?rw-r--r--  2.0 fat       87 b- defN 20-Feb-02 00:00 insulaclient-0.6.2.dist-info/WHEEL
+?rw-r--r--  2.0 fat       58 b- defN 20-Feb-02 00:00 insulaclient-0.6.2.dist-info/entry_points.txt
+?rw-r--r--  2.0 fat        0 b- defN 20-Feb-02 00:00 insulaclient-0.6.2.dist-info/licenses/LICENSE.txt
+?rw-r--r--  2.0 fat     2453 b- defN 20-Feb-02 00:00 insulaclient-0.6.2.dist-info/RECORD
+29 files, 70709 bytes uncompressed, 19348 bytes compressed:  72.6%
```

## zipnote {}

```diff
@@ -66,23 +66,23 @@
 
 Filename: insulaClient/workflow_step.py
 Comment: 
 
 Filename: insulaClient/workflow_step_runner.py
 Comment: 
 
-Filename: insulaclient-0.6.1.dist-info/METADATA
+Filename: insulaclient-0.6.2.dist-info/METADATA
 Comment: 
 
-Filename: insulaclient-0.6.1.dist-info/WHEEL
+Filename: insulaclient-0.6.2.dist-info/WHEEL
 Comment: 
 
-Filename: insulaclient-0.6.1.dist-info/entry_points.txt
+Filename: insulaclient-0.6.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: insulaclient-0.6.1.dist-info/licenses/LICENSE.txt
+Filename: insulaclient-0.6.2.dist-info/licenses/LICENSE.txt
 Comment: 
 
-Filename: insulaclient-0.6.1.dist-info/RECORD
+Filename: insulaclient-0.6.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## insulaClient/workflow.py

```diff
@@ -1,34 +1,80 @@
+from threading import Lock
 from snakenest import Poisoned
 from .InsulaApiConfig import InsulaApiConfig
 from .workflow_step import InsulaWorkflowStep
 from .job_status import InsulaJobStatus
 from .files_job_result import InsulaFilesJobResult
 from .workflow_step_runner import InsulaWorkflowStepRunner
-from .results_manager import ResultsManager
+from .results_manager import ResultManager
 from .workflow_manager import WorkflowManager
+from .logger import logger
 
 
 class InsulaWorkflow(object):
-    @Poisoned(workflow_manager='native_workflow_manager', result_manager='memory_results_manager')
+    @Poisoned()
     def __init__(self, insula_config: InsulaApiConfig, workflow: str, parameters: dict, external_name,
-                 workflow_manager: WorkflowManager, result_manager: ResultsManager):
+                 workflow_manager: WorkflowManager, result_manager: ResultManager):
 
         self.__workflow_data = workflow_manager.parse(workflow, parameters)
         self.__result_manager = result_manager
 
         self.__external_name = external_name
         self.__insula_api_config = insula_config
         self.__steps_order = []
         self.__get_workflow_info()
         self.__validate_version()
         self.__get_workflow_steps_order()
         self.__init_job_requirements()
         self.__check_parameters(parameters)
 
+        self.__lock: Lock = Lock()
+        self.__can_continue: bool = True
+
+    def stop(self):
+        with self.__lock:
+            self.__can_continue = False
+
+    def run(self):
+        logger.info('Running WORKFLOW\n')
+        insula_job_status = InsulaJobStatus()
+        insula_job_status.set_job_id(f'wf_{self.__name}')
+        insula_job_status.set_properties(self.__filter_log_properties()).save()
+
+        try:
+            for step in self.__steps_order:
+
+                with self.__lock:
+                    if not self.__can_continue:
+                        break
+
+                logger.info(f'running:\n\tstep: Step: {step}')
+                workflow_step_runner = InsulaWorkflowStepRunner(
+                    self.__insula_api_config,
+                    step,
+                    self.__workflow_data
+                )
+                results = workflow_step_runner.run()
+                for result in results['results']:
+                    self.__result_manager.add_result_step(self.__workflow_data.identifier, result['run'])
+                insula_job_status.set_properties(self.__filter_log_properties()).save()
+
+                if results['error']:
+                    if not self.__workflow_data.config['continue_on_error']:
+                        raise Exception('there is an error, check the pid file')
+
+            if self.__workflow_data.config['delete_workflow_log']:
+                insula_job_status.remove()
+
+            return self.__result_manager.get_result_steps(self.__workflow_data.identifier)
+
+        except Exception as error:
+            insula_job_status.set_job_error('ERROR', error).save()
+            raise Exception(error)
+
     # TODO: remove from here and move in WorkflowDataManager
     def __check_parameters(self, parameters):
         for key, value in self.__workflow_data.parameters.items():
             if isinstance(value, str):
                 pass
             elif isinstance(value, list):
                 for v in value:
@@ -40,23 +86,24 @@
     def __get_workflow_info(self):
         self.__name = self.__workflow_data.name
         self.__type = self.__workflow_data.type
 
         if self.__external_name:
             self.__name = self.__external_name
 
+    # TODO: remove from here and move in WorkflowDataManager
     def __validate_version(self):
         self.__version = self.__workflow_data.version
 
         if not self.__version:
-            print('This workflow requires insulaClient version 0.0.1')
+            logger.info('This workflow requires insulaClient version 0.0.1')
             exit(1)
 
         if self.__version != 'beta/1':
-            print('Version not compatible with beta/1')
+            logger.info('Version not compatible with beta/1')
             exit(1)
 
     def __get_workflow_steps_order(self):
         for step in self.__workflow_data.steps:
             self.__steps_order.append(InsulaWorkflowStep(step))
 
     def __init_job_requirements(self):
@@ -79,39 +126,7 @@
             self.__result_manager.add_result_step(self.__workflow_data.identifier, run)
 
     def __filter_log_properties(self):
         to_save = {
             'steps': self.__result_manager.get_result_steps(self.__workflow_data.identifier)
         }
         return to_save
-
-    def run(self):
-        print('Running WORKFLOW\n')
-        insula_job_status = InsulaJobStatus()
-        insula_job_status.set_job_id(f'wf_{self.__name}')
-        insula_job_status.set_properties(self.__filter_log_properties()).save()
-
-        try:
-            for step in self.__steps_order:
-                print(f'running:\n\tstep: Step: {step}')
-                _ = InsulaWorkflowStepRunner(
-                    self.__insula_api_config,
-                    step,
-                    self.__workflow_data
-                )
-                results = _.run()
-                for result in results['results']:
-                    self.__result_manager.add_result_step(self.__workflow_data.identifier, result['run'])
-                insula_job_status.set_properties(self.__filter_log_properties()).save()
-
-                if results['error']:
-                    print(results)
-                    if not self.__workflow_data.config['continue_on_error']:
-                        raise Exception('there is an error, check the pid file')
-
-            if self.__workflow_data.config['delete_workflow_log']:
-                insula_job_status.remove()
-            return self.__result_manager.get_result_steps(self.__workflow_data.identifier)
-
-        except Exception as error:
-            insula_job_status.set_job_error('ERROR', error).save()
-            raise Exception(error)
```

## Comparing `insulaclient-0.6.1.dist-info/METADATA` & `insulaclient-0.6.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: InsulaClient
-Version: 0.6.1
+Version: 0.6.2
 Summary: Insula CLient
 Author-email: Roberto Di Rienzo <roberto.dirienzo@codelithic.com>, roberto.dirienzo@cgi.com
 Maintainer-email: Roberto Di Rienzo <roberto.dirienzo@codelithic.com>
 License-File: LICENSE.txt
 Keywords: Italia,cgi,client,insula
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

## Comparing `insulaclient-0.6.1.dist-info/RECORD` & `insulaclient-0.6.2.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 insulaClient/job_status.py,sha256=2p70J77OjY9XSVXlxlGUgOfD4OUIgcob61hzK5f1uv4,3153
 insulaClient/logger.py,sha256=SyGGFciQATh-JOzBKW_a_WW8ukZkhJimQwgvaL7taRE,262
 insulaClient/placeholders.py,sha256=FZANExqFNVs5SaOqDnflEUcrpOmzWPhKpJCw78E3LaE,4617
 insulaClient/results_manager.py,sha256=jAnnM6fv8S3oP1PT_6A1cPN2db7ExcRPYAOpaSaYHUs,1341
 insulaClient/s3.py,sha256=H5O5NbkWI58Q0KQqyBmiI2gJT8yfe2qTvU67E6-9aOY,1894
 insulaClient/step_result.py,sha256=yX2RINUxlsqxYxfm9sUx69M_YAY0EM2SZBd2SxqXfRo,725
 insulaClient/utils.py,sha256=3iDY90A8vlc52KKLukNHVEg6bhWfiGSKjkRXVueO5W8,929
-insulaClient/workflow.py,sha256=jh5Yu5RioDQHt7Hqv5C7tZCzMFnLiC0jXqTx4VopYPE,4630
+insulaClient/workflow.py,sha256=bes1cbN1yX89vyL6TovI1YOAXZY1eEwYfGv3_DWw5Ao,4966
 insulaClient/workflow_manager.py,sha256=MsCTMBCwrLVorTyooX80ACusQJZ9ky3afx5wUcozKFM,6449
 insulaClient/workflow_step.py,sha256=BllZzKLeOuNbB4aUtyIESqPOpPjDDVo-_YkSSjl27-0,818
 insulaClient/workflow_step_runner.py,sha256=836FXIMLwpsPHWbiWknQVIZl5WAOX4sNugt14lqy9zw,14627
-insulaclient-0.6.1.dist-info/METADATA,sha256=Xf0d7OQZoXLSi1L3xCb1tgnPSXHKYE6zkB2z3H_YKO8,9984
-insulaclient-0.6.1.dist-info/WHEEL,sha256=as-1oFTWSeWBgyzh0O_qF439xqBe6AbBgt4MfYe5zwY,87
-insulaclient-0.6.1.dist-info/entry_points.txt,sha256=XmoJBOq6Rxy9modIBGlEqhdnWgRWiKRZxJOVnoDoW8A,58
-insulaclient-0.6.1.dist-info/licenses/LICENSE.txt,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-insulaclient-0.6.1.dist-info/RECORD,,
+insulaclient-0.6.2.dist-info/METADATA,sha256=nEBfIxFhyXmB7YouBL18Fgy2RP1GXb386MTnZtdaRsY,9984
+insulaclient-0.6.2.dist-info/WHEEL,sha256=as-1oFTWSeWBgyzh0O_qF439xqBe6AbBgt4MfYe5zwY,87
+insulaclient-0.6.2.dist-info/entry_points.txt,sha256=XmoJBOq6Rxy9modIBGlEqhdnWgRWiKRZxJOVnoDoW8A,58
+insulaclient-0.6.2.dist-info/licenses/LICENSE.txt,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+insulaclient-0.6.2.dist-info/RECORD,,
```

