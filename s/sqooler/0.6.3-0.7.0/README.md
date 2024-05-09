# Comparing `tmp/sqooler-0.6.3.tar.gz` & `tmp/sqooler-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqooler-0.6.3.tar", max compression
+gzip compressed data, was "sqooler-0.7.0.tar", max compression
```

## Comparing `sqooler-0.6.3.tar` & `sqooler-0.7.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1211 2024-03-18 17:38:21.370303 sqooler-0.6.3/LICENSE
--rw-r--r--   0        0        0     3928 2024-03-21 16:38:07.651464 sqooler-0.6.3/README.md
--rw-r--r--   0        0        0     1057 2024-04-16 20:23:10.386599 sqooler-0.6.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-18 17:38:21.374962 sqooler-0.6.3/src/sqooler/__init__.py
--rw-r--r--   0        0        0    12140 2024-04-03 16:25:44.628605 sqooler-0.6.3/src/sqooler/schemes.py
--rw-r--r--   0        0        0     8775 2024-03-29 14:08:39.014572 sqooler-0.6.3/src/sqooler/security.py
--rw-r--r--   0        0        0    27245 2024-04-16 20:23:01.954085 sqooler-0.6.3/src/sqooler/spoolers.py
--rw-r--r--   0        0        0        0 2024-03-21 16:38:07.659018 sqooler-0.6.3/src/sqooler/storage_providers/__init__.py
--rw-r--r--   0        0        0    22085 2024-04-16 20:11:29.601741 sqooler-0.6.3/src/sqooler/storage_providers/base.py
--rw-r--r--   0        0        0    25716 2024-04-16 20:11:29.602180 sqooler-0.6.3/src/sqooler/storage_providers/dropbox.py
--rw-r--r--   0        0        0    21513 2024-04-16 20:11:29.602485 sqooler-0.6.3/src/sqooler/storage_providers/local.py
--rw-r--r--   0        0        0    26090 2024-04-16 20:11:29.602903 sqooler-0.6.3/src/sqooler/storage_providers/mongodb.py
--rw-r--r--   0        0        0     6472 2024-04-14 14:40:46.943889 sqooler-0.6.3/src/sqooler/utils.py
--rw-r--r--   0        0        0     4927 1970-01-01 00:00:00.000000 sqooler-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-04-18 18:44:41.208787 sqooler-0.7.0/LICENSE
+-rw-r--r--   0        0        0     3928 2024-04-18 18:44:41.212121 sqooler-0.7.0/README.md
+-rw-r--r--   0        0        0     1282 2024-05-09 11:09:37.943063 sqooler-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-18 18:44:41.212209 sqooler-0.7.0/src/sqooler/__init__.py
+-rw-r--r--   0        0        0      810 2024-05-05 09:53:38.382220 sqooler-0.7.0/src/sqooler/cli.py
+-rw-r--r--   0        0        0    12206 2024-05-09 11:09:37.944438 sqooler-0.7.0/src/sqooler/schemes.py
+-rw-r--r--   0        0        0     8775 2024-04-18 18:44:42.470722 sqooler-0.7.0/src/sqooler/security.py
+-rw-r--r--   0        0        0    27991 2024-04-19 14:40:24.524812 sqooler-0.7.0/src/sqooler/spoolers.py
+-rw-r--r--   0        0        0        0 2024-04-18 18:44:42.471937 sqooler-0.7.0/src/sqooler/storage_providers/__init__.py
+-rw-r--r--   0        0        0    30402 2024-05-09 11:09:37.945823 sqooler-0.7.0/src/sqooler/storage_providers/base.py
+-rw-r--r--   0        0        0    30431 2024-05-09 11:09:37.946668 sqooler-0.7.0/src/sqooler/storage_providers/dropbox.py
+-rw-r--r--   0        0        0    25852 2024-05-04 06:42:01.258236 sqooler-0.7.0/src/sqooler/storage_providers/local.py
+-rw-r--r--   0        0        0    31201 2024-05-04 06:41:56.453899 sqooler-0.7.0/src/sqooler/storage_providers/mongodb.py
+-rw-r--r--   0        0        0     6672 2024-05-03 19:00:26.771893 sqooler-0.7.0/src/sqooler/utils.py
+-rw-r--r--   0        0        0     4965 1970-01-01 00:00:00.000000 sqooler-0.7.0/PKG-INFO
```

### Comparing `sqooler-0.6.3/LICENSE` & `sqooler-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqooler-0.6.3/README.md` & `sqooler-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `sqooler-0.6.3/pyproject.toml` & `sqooler-0.7.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sqooler"
-version = "0.6.3"
+version = "0.7.0"
 description = "Code that enables validated cloud access to quantum hardware (simulators)"
 authors = ["fretchen <fred.jendrzejewski@gmail.com>"]
 repository = "https://github.com/Alqor-UG/sqooler"
 documentation = "https://alqor-ug.github.io/sqooler"
 license = "Unlicense"
 readme = "README.md"
 packages = [{include = "sqooler", from = "src"}]
@@ -14,30 +14,42 @@
 python = "^3.10"
 pydantic = "^2.3.0"
 dropbox = "^11.36.2"
 setuptools = "^69.0.3"
 pymongo = "^4.3.3"
 regex = "^2023.6.3"
 cryptography = "^42.0.5"
+click = "^8.1.7"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.1.1"
 pytest = "^8.0.2"
 pylint = "^3.0.3"
 mypy = "^1.8.0"
 python-decouple = "^3.6"
 ipykernel = "^6.28.0"
 icecream = "^2.1.3"
 pytest-cov = "^5.0.0"
+isort = "^5.13.2"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 mike = "^2.0.0"
 mkdocs-material = "^9.1.5"
 mkdocstrings-python = "^1.3.0"
 
+[tool.poetry.scripts]
+sqoolerkey = "sqooler.cli:cli_private_key_str"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.isort]
+multi_line_output = 3
+include_trailing_comma = true
+force_grid_wrap = 0
+line_length = 88
+profile = "black"
```

### Comparing `sqooler-0.6.3/src/sqooler/schemes.py` & `sqooler-0.7.0/src/sqooler/schemes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 The module that contains common logic for schemes, validation etc.
 There is no obvious need, why this code should be touch in a new back-end.
 """
 
-from typing import Optional, Literal, Annotated
 from datetime import datetime
+from typing import Annotated, Literal, Optional
 
 from pydantic import BaseModel, Field, field_validator
 
 # the strings that are allowed for the status
 StatusStr = Annotated[
     Literal["INITIALIZING", "QUEUED", "DONE", "ERROR"],
     Field(description="status of job execution."),
@@ -138,28 +138,32 @@
     simulator: bool = Field(description="True if the backend is a simulator")
     supported_instructions: list[str] = Field(
         description="Instructions supported by the backend."
     )
     num_wires: int = Field(description="The number of qubits / wires for the backend")
     wire_order: WireOrderStr
     num_species: int = Field(description="The number of species in the system.")
-    operational: bool = Field(description="True if the backend is operational")
+
     pending_jobs: Optional[int] = Field(
         default=None, description="The number of pending jobs on the backend"
     )
     status_msg: Optional[str] = Field(
         default=None, description="The status message for the backend"
     )
     last_queue_check: Optional[datetime] = Field(
         default=None, description="The last time the queue was checked."
     )
     sign: bool = Field(
         default=False,
         description="True if the results are signed by the backend provider.",
     )
+    kid: Optional[str] = Field(
+        default=None,
+        description="The identifier for the public and private key of the backend.",
+    )
 
 
 class BackendConfigSchemaOut(BaseModel, validate_assignment=True):
     """
     The schema send out to detail the configuration of the backend. We follow the
     conventions of the qiskit configuration dictionary here.
```

### Comparing `sqooler-0.6.3/src/sqooler/security.py` & `sqooler-0.7.0/src/sqooler/security.py`

 * *Files identical despite different names*

### Comparing `sqooler-0.6.3/src/sqooler/spoolers.py` & `sqooler-0.7.0/src/sqooler/spoolers.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,42 +3,37 @@
 on the back-end side for people that would like to perform calculations and work through the job queue.
 
 The main class is the `Spooler` class. It is the class that is used for the simulators. 
 The `LabscriptSpooler` class is a specialized version of the `Spooler` class that allows us to execute 
 jobs in labscript directly.
 """
 
+import logging
 import os
-from collections.abc import Callable
-from typing import Type, Any, Optional
-from time import sleep
 from abc import ABC
-import logging
+from binascii import Error as BinasciiError
+from time import sleep
+from typing import Any, Callable, Optional, Type
 
 from decouple import config
-
-from pydantic import ValidationError, BaseModel
-
-from .security import (
-    JWK,
-    jwk_from_config_str,
-)
+from pydantic import BaseModel, ValidationError
 
 from .schemes import (
     BackendConfigSchemaIn,
-    ExperimentDict,
+    ColdAtomStr,
     ExperimentalInputDict,
-    ResultDict,
-    StatusMsgDict,
+    ExperimentDict,
     GateDict,
     LabscriptParams,
+    ResultDict,
+    StatusMsgDict,
     WireOrderStr,
-    ColdAtomStr,
     get_init_status,
 )
+from .security import JWK, jwk_from_config_str
 
 
 class BaseSpooler(ABC):
     """
     Abstract base class for spoolers. They are the main logic of the back-end.
 
     Attributes:
@@ -47,15 +42,14 @@
         n_wires: maximum number of wires for the spooler
         n_max_shots: the maximum number of shots for the spooler
         version: the version of the backend
         cold_atom_type: the type of cold atom that is used in the experiment
         n_max_experiments: the maximum number of experiments that can be executed
         wire_order: the order of the wires
         num_species: the number of atomic species in the experiment
-        operational: is the backend ready for access by remote users ?
         sign: sign the results of the job
     """
 
     def __init__(
         self,
         ins_schema_dict: dict,
         device_config: Type[BaseModel],
@@ -63,15 +57,14 @@
         description: str = "",
         n_max_shots: int = 1000,
         version: str = "0.0.1",
         cold_atom_type: ColdAtomStr = "spin",
         n_max_experiments: int = 15,
         wire_order: WireOrderStr = "interleaved",
         num_species: int = 1,
-        operational: bool = True,
         sign: bool = False,
     ):
         """
         The constructor of the class.
         """
         self.ins_schema_dict = ins_schema_dict
         self.device_config = device_config
@@ -80,15 +73,14 @@
         self.description = description
         self.version = version
         self.cold_atom_type = cold_atom_type
         self.n_max_experiments = n_max_experiments
         self.wire_order = wire_order
         self.num_species = num_species
         self._display_name: str = ""
-        self.operational = operational
         self.sign = sign
 
     def check_experiment(self, exper_dict: dict) -> tuple[str, bool]:
         """
         Check the validity of the experiment. It checks if the the instructions are valid
         based on the device configuration of the spooler.
 
@@ -106,14 +98,20 @@
         except ValidationError as err:
             return str(err), False
 
     def get_configuration(self) -> BackendConfigSchemaIn:
         """
         Sends back the configuration dictionary of the spooler.
 
+        This creates the configuration of the Spooler. However, it does not contain
+        any information about the operational status. This is not really connected to
+        the machine but much rather to the queue etc. So items of the `BackendConfigSchemaIn`
+        like `operational` or `last_queue_check` are not set here at just the default values.
+        ``
+
         Returns:
             The configuration dictionary of the spooler.
         """
         gate_list = []
         for _, ins_obj in self.ins_schema_dict.items():
             if "is_gate" in ins_obj.model_fields:
                 gate_list.append(ins_obj.config_dict())
@@ -125,15 +123,14 @@
             "max_experiments": self.n_max_experiments,
             "max_shots": self.n_max_shots,
             "simulator": True,
             "supported_instructions": list(self.ins_schema_dict.keys()),
             "num_wires": self.n_wires,
             "wire_order": self.wire_order,
             "num_species": self.num_species,
-            "operational": self.operational,
             "display_name": self.display_name,
             "sign": self.sign,
         }
         return BackendConfigSchemaIn(**backend_config_dict)
 
     def check_instructions(self, ins_list: list) -> tuple[str, bool]:
         """
@@ -348,17 +345,32 @@
 
     def get_private_jwk(self) -> JWK:
         """
         Get the private JWK for the spooler.
 
         Returns:
             The private JWK for the spooler.
+
+        Raises:
+            ValueError: If the private JWK is not set.
         """
-        private_jwk_str = config("PRIVATE_JWK_STR")
-        return jwk_from_config_str(private_jwk_str)
+        private_jwk_str = config("PRIVATE_JWK_STR", default=None)
+        if private_jwk_str == "":
+            logging.error("PRIVATE_JWK_STR must not be empty.")
+
+            raise ValueError("PRIVATE_JWK_STR must not be empty.")
+
+        if private_jwk_str is None:
+            logging.error("PRIVATE_JWK_STR is not set and available.")
+            raise ValueError("PRIVATE_JWK_STR is not set and available.")
+        try:
+            return jwk_from_config_str(private_jwk_str)
+        except BinasciiError as bin_err:
+            logging.error("PRIVATE_JWK_STR is invalid.")
+            raise ValueError("PRIVATE_JWK_STR is invalid.") from bin_err
 
 
 class Spooler(BaseSpooler):
     """
     The class for the spooler as it can be used for simulators.
     """
 
@@ -456,15 +468,14 @@
         description: str = "",
         n_max_shots: int = 1000,
         version: str = "0.0.1",
         cold_atom_type: ColdAtomStr = "spin",
         n_max_experiments: int = 15,
         wire_order: WireOrderStr = "interleaved",
         num_species: int = 1,
-        operational: bool = True,
         sign: bool = False,
     ):
         """
         The constructor of the class. The  arguments are the same as for the Spooler
         class with two additions.
 
 
@@ -476,15 +487,14 @@
             description,
             n_max_shots,
             version,
             cold_atom_type,
             n_max_experiments,
             wire_order,
             num_species,
-            operational,
             sign,
         )
         self.remote_client = remote_client
         self.labscript_params = labscript_params
         self.run = run
 
     def add_job(
```

### Comparing `sqooler-0.6.3/src/sqooler/storage_providers/base.py` & `sqooler-0.7.0/src/sqooler/storage_providers/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 """
 The module that contains all the necessary logic for communication with the external
 storage for the jobs. It creates an abstract API layer for the storage providers.
 """
 
-from abc import ABC, abstractmethod
-import re
-
-from typing import Mapping, Callable, Any, Optional
 import functools
-
+import logging
+import re
+from abc import ABC, abstractmethod
 from datetime import datetime, timezone
+from typing import Any, Callable, Mapping, Optional
+
+from decouple import config
 
 from ..schemes import (
-    ResultDict,
-    StatusMsgDict,
-    BackendStatusSchemaOut,
     BackendConfigSchemaIn,
     BackendConfigSchemaOut,
-    NextJobSchema,
-    DisplayNameStr,
     BackendNameStr,
+    BackendStatusSchemaOut,
+    DisplayNameStr,
+    NextJobSchema,
+    ResultDict,
+    StatusMsgDict,
 )
-
 from ..security import JWK, sign_payload
 
 
 def validate_active(func: Callable) -> Callable:
     """
     Decorator to check if the storage provider is active.
     """
@@ -132,14 +132,18 @@
         Returns:
             The status dict of the backend
 
         Raises:
             FileNotFoundError: If the backend does not exist
         """
         backend_config_info = self.get_config(display_name)
+
+        # now see how long it has been since the last queue check in minutes
+        # if it is more than 5 minutes, we should set the backend to not operational
+
         qiskit_backend_dict = self.backend_dict_to_qiskit_status(backend_config_info)
         return qiskit_backend_dict
 
     @abstractmethod
     def upload_job(
         self, job_dict: dict, display_name: DisplayNameStr, username: str
     ) -> str:
@@ -166,23 +170,28 @@
 
         Returns:
             The content of the job
         """
 
     @abstractmethod
     def upload_status(
-        self, display_name: DisplayNameStr, username: str, job_id: str
+        self,
+        display_name: DisplayNameStr,
+        username: str,
+        job_id: str,
+        private_jwk: Optional[JWK] = None,
     ) -> StatusMsgDict:
         """
         This function uploads a status file to the backend and creates the status dict.
 
         Args:
             display_name: The name of the backend to which we want to upload the job
             username: The username of the user that is uploading the job
             job_id: The job_id of the job that we want to upload the status for
+            private_jwk: The private key of the backend
 
         Returns:
             The status dict of the job
         """
 
     @abstractmethod
     def get_status(
@@ -197,14 +206,71 @@
             job_id: The job_id of the job that we want to upload the status for
 
         Returns:
             The status dict of the job
         """
 
     @abstractmethod
+    def _delete_status(
+        self, display_name: DisplayNameStr, username: str, job_id: str
+    ) -> bool:
+        """
+        Delete a status from the storage. This is only intended for test purposes.
+
+        Args:
+            display_name: The name of the backend to which we want to upload the job
+            username: The username of the user that is uploading the job
+            job_id: The job_id of the job that we want to upload the status for
+
+        Raises:
+            FileNotFoundError: If the status does not exist.
+
+        Returns:
+            Success if the file was deleted successfully
+        """
+
+    @abstractmethod
+    def upload_result(
+        self,
+        result_dict: ResultDict,
+        display_name: DisplayNameStr,
+        job_id: str,
+        private_jwk: Optional[JWK] = None,
+    ) -> bool:
+        """
+        This function allows us to upload the result file .
+
+        Args:
+            result_dict: The result dictionary
+            display_name: The name of the backend to which we want to upload the job
+            job_id: The job_id of the job that we want to upload the status for
+            private_jwk: The private key of the backend
+
+        Returns:
+            The success of the upload process
+        """
+
+    @abstractmethod
+    def _delete_result(self, display_name: DisplayNameStr, job_id: str) -> bool:
+        """
+        Delete a result from the storage. This is only intended for test purposes.
+
+        Args:
+            display_name: The name of the backend to which we want to upload the job
+            username: The username of the user that is uploading the job
+            job_id: The job_id of the job that we want to upload the status for
+
+        Raises:
+            FileNotFoundError: If the result does not exist.
+
+        Returns:
+            Success if the file was deleted successfully
+        """
+
+    @abstractmethod
     def get_result(
         self, display_name: DisplayNameStr, username: str, job_id: str
     ) -> ResultDict:
         """
         This function gets the result file from the backend and returns the result dict.
 
         Args:
@@ -214,14 +280,28 @@
 
         Returns:
             The result dict of the job. If the information is not available, the result dict
             has a status of "ERROR".
         """
 
     @abstractmethod
+    def verify_result(self, display_name: DisplayNameStr, job_id: str) -> bool:
+        """
+        This function verifies the result and returns the success. If the backend does not sign the
+        result, we will reutrn `False` by default, given that we were not able to establish ownership.
+
+        Args:
+            display_name: The name of the backend to which we want to upload the job
+            job_id: The job_id of the job that we want to upload the status for
+
+        Returns:
+            If it was possible to verify the result dict positively.
+        """
+
+    @abstractmethod
     def update_file(self, content_dict: dict, storage_path: str, job_id: str) -> None:
         """
         Update the file content. It replaces the old content with the new content.
 
         Args:
             content_dict: The dictionary containing the new content of the file
             storage_path: The path to the file
@@ -309,14 +389,29 @@
             display_name : The name of the backend
 
         Returns:
             The configuration of the backend in complete form.
         """
 
     @abstractmethod
+    def _delete_config(self, display_name: DisplayNameStr) -> bool:
+        """
+        Delete a config from the storage. This is only intended for test purposes.
+
+        Args:
+            display_name: The name of the backend to which we want to upload the job
+
+        Raises:
+            FileNotFoundError: If the status does not exist.
+
+        Returns:
+            Success if the file was deleted successfully
+        """
+
+    @abstractmethod
     def upload_public_key(self, public_jwk: JWK, display_name: DisplayNameStr) -> None:
         """
         The function that uploads the spooler public JWK to the storage.
 
         Args:
             public_jwk: The JWK that contains the public key
             display_name : The name of the backend
@@ -334,14 +429,29 @@
             display_name : The name of the backend
 
         Returns:
             JWk : The public JWK object
         """
 
     @abstractmethod
+    def _delete_public_key(self, kid: str) -> bool:
+        """
+        Delete a public key from the storage. This is only intended for test purposes.
+
+        Args:
+            kid: The key id of the public key
+
+        Raises:
+            FileNotFoundError: If the status does not exist.
+
+        Returns:
+            Success if the file was deleted successfully
+        """
+
+    @abstractmethod
     def update_in_database(
         self,
         result_dict: ResultDict,
         status_msg_dict: StatusMsgDict,
         job_id: str,
         display_name: DisplayNameStr,
         private_jwk: Optional[JWK] = None,
@@ -385,14 +495,58 @@
             display_name: The name of the backend
             private_jwk: The private JWK to sign the result with
 
         Returns:
             the job dict
         """
 
+    def _common_upload_result(
+        self,
+        result_dict: ResultDict,
+        display_name: DisplayNameStr,
+        job_id: str,
+        result_json_dir: str,
+        result_json_name: str,
+        private_jwk: Optional[JWK] = None,
+    ) -> bool:
+        """
+        Common code for the upload of the results.
+
+        Args:
+            result_dict: The dictionary containing the result of the job
+            display_name: The name of the backend
+            job_id: The name of the job
+            result_json_dir: The directory where the result should be stored
+            result_json_name: The name of the result file
+            private_jwk: The private JWK to sign the result with
+
+        Returns:
+            The success of the upload process
+        """
+        # make sure that the job_id is in the result_dict
+        if not result_dict.job_id == job_id:
+            logging.warning(
+                "Tried to upload an inconsistent result for job_id %s.", job_id
+            )
+            result_dict.job_id = job_id
+        # let us see if we should sign the result
+        backend_config = self.get_config(display_name)
+        if backend_config.sign:
+            # get the private key
+            if private_jwk is None:
+                raise ValueError(
+                    "The private key is not given, but the backend is configured to sign."
+                )
+            # we should sign the result
+            signed_result = sign_payload(result_dict.model_dump(), private_jwk)
+            self.upload(signed_result.model_dump(), result_json_dir, result_json_name)
+        else:
+            self.upload(result_dict.model_dump(), result_json_dir, result_json_name)
+        return True
+
     def _format_config_dict(
         self, config_dict: BackendConfigSchemaIn, private_jwk: Optional[JWK] = None
     ) -> dict:
         """
         Format the config dict to a string that can be written to a file.
 
         Args:
@@ -408,20 +562,61 @@
         if config_dict.sign:
             # get the private key
             if private_jwk is None:
                 raise ValueError(
                     "The private key is not given, but the backend needs to be signed."
                 )
             # we sign the result now
+            config_dict.kid = private_jwk.kid
             signed_config = sign_payload(config_dict.model_dump(), private_jwk)
             upload_dict = signed_config.model_dump()
         else:
             upload_dict = config_dict.model_dump()
         return upload_dict
 
+    def _format_status_dict(
+        self,
+        status_dict: StatusMsgDict,
+        storage_path: str,
+        display_name: DisplayNameStr,
+        job_id: str,
+        private_jwk: Optional[JWK] = None,
+        status_json_name: Optional[str] = None,
+    ) -> None:
+        """
+        Allows us to upload the appropiate status dict to the storage provider.
+        """
+        # get the backend config
+        config_dict = self.get_config(display_name)
+        if config_dict.sign:
+            # get the private key
+            if private_jwk is None:
+                raise ValueError(
+                    "The private key is not given, but the backend needs to be signed."
+                )
+            # we sign the result now
+            signed_status = sign_payload(status_dict.model_dump(), private_jwk)
+            upload_dict = signed_status.model_dump()
+        else:
+            upload_dict = status_dict.model_dump()
+
+        # now upload the status dict
+        if status_json_name is None:
+            self.upload(
+                content_dict=upload_dict,
+                storage_path=storage_path,
+                job_id=job_id,
+            )
+        else:
+            self.upload(
+                content_dict=upload_dict,
+                storage_path=storage_path,
+                job_id=status_json_name,
+            )
+
     def _format_update_config(
         self,
         old_config_jws: dict,
         config_dict: BackendConfigSchemaIn,
         private_jwk: Optional[JWK] = None,
     ) -> dict:
         """
@@ -458,14 +653,15 @@
                 test_signature = sign_payload(old_config_dict.model_dump(), private_jwk)
                 if not test_signature.signature == old_config_jws["signature"]:
                     raise ValueError(
                         "The new private key does not create the same signature as the old one."
                     )
 
             # now that we know that the private key is the same, we can sign the new config
+            config_dict.kid = private_jwk.kid
             signed_config = sign_payload(config_dict.model_dump(), private_jwk)
             upload_dict = signed_config.model_dump()
         else:
             # the old and the new are not signed
             upload_dict = config_dict.model_dump()
         return upload_dict
 
@@ -511,14 +707,33 @@
             result_payload["backend_name"] = backend_config_info.backend_name
             typed_result = ResultDict(**result_payload)
         else:
             result_dict["backend_name"] = backend_config_info.backend_name
             typed_result = ResultDict(**result_dict)
         return typed_result
 
+    def _adapt_status_dict(self, status_dict: dict) -> StatusMsgDict:
+        """
+        This function adapts the status dict to the standard format that we use in the system.
+
+        Args:
+            status_dict: The status dictionary
+            backend_config_info: The configuration of the backend
+
+        Returns:
+            The status dict in the standard format
+        """
+        # done day we should verify the result before we send it out
+        expected_keys_for_jws = {"header", "payload", "signature"}
+        if set(status_dict.keys()) == expected_keys_for_jws:
+            typed_result = StatusMsgDict(**status_dict["payload"])
+        else:
+            typed_result = StatusMsgDict(**status_dict)
+        return typed_result
+
     def timestamp_queue(
         self, display_name: DisplayNameStr, private_jwk: Optional[JWK] = None
     ) -> None:
         """
         Updates the time stamp for when the system last looked into the file queue.
         This allows us to track if the system is actually online or not.
 
@@ -592,14 +807,31 @@
         Returns:
             The long name of the backend
         """
         if simulator:
             return f"{self.name}_{display_name}_simulator"
         return f"{self.name}_{display_name}_hardware"
 
+    def _last_queued_to_operational(self, last_queue_check: datetime | None) -> bool:
+        """
+        Calculate the operational status based on the last time the queue
+        was checked.
+        """
+        # get the timeout from the configuration
+        t_timeout = config("T_TIMEOUT", cast=int, default=300)
+        if not last_queue_check:
+            return False
+
+        last_queue_check = last_queue_check.replace(tzinfo=timezone.utc)
+        current_time = datetime.now(timezone.utc).replace(microsecond=0)
+
+        if (current_time - last_queue_check).total_seconds() > t_timeout:
+            return False
+        return True
+
     def backend_dict_to_qiskit_status(
         self, backend_dict: BackendConfigSchemaIn
     ) -> BackendStatusSchemaOut:
         """
         This function transforms the dictionary that is safed in the storage provider
         into a qiskit backend status dictionnary.
 
@@ -614,28 +846,30 @@
             "backend_version": "",
             "operational": True,
             "pending_jobs": 0,
             "status_msg": "",
         }
 
         display_name = backend_dict.display_name
+        last_queue_check = backend_dict.last_queue_check
 
         # if the name is already in the dict, we should set the backend_name to the name
         # otherwise we calculate it.
         if backend_dict.simulator:
             backend_name = f"{self.name}_{display_name}_simulator"
         else:
             backend_name = f"{self.name}_{display_name}_hardware"
 
         backend_status_dict["backend_name"] = backend_name
         backend_status_dict["backend_version"] = backend_dict.version
 
         # now I also need to obtain the operational status from the backend.
-        backend_status_dict["operational"] = backend_dict.operational
-
+        backend_status_dict["operational"] = self._last_queued_to_operational(
+            last_queue_check
+        )
         # would be nice to attempt to get the pending jobs too, if possible easily.
         if backend_dict.pending_jobs:
             backend_status_dict["pending_jobs"] = backend_dict.pending_jobs
         else:
             backend_status_dict["pending_jobs"] = 0
 
         # and also handle the status message which is currently optional BackendConfigSchemaIn
```

### Comparing `sqooler-0.6.3/src/sqooler/storage_providers/dropbox.py` & `sqooler-0.7.0/src/sqooler/storage_providers/dropbox.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 """
 The module that contains all the necessary logic for communication with the Dropbox providers.
 """
 
+# necessary for the dropbox provider
+import datetime
+import json
 import sys
 import uuid
-import json
-
+from datetime import timezone
 from typing import Mapping, Optional
 
-# necessary for the dropbox provider
-import datetime
-from datetime import timezone
 import dropbox
-from dropbox.files import WriteMode
 from dropbox.exceptions import ApiError, AuthError
+from dropbox.files import WriteMode
 
 from ..schemes import (
-    ResultDict,
-    StatusMsgDict,
-    DropboxLoginInformation,
     BackendConfigSchemaIn,
-    NextJobSchema,
     DisplayNameStr,
+    DropboxLoginInformation,
+    NextJobSchema,
+    ResultDict,
+    StatusMsgDict,
 )
-from ..security import JWK, sign_payload
-from .base import StorageProvider, validate_active, datetime_handler
+from ..security import JWK, JWSDict
+from .base import StorageProvider, datetime_handler, validate_active
 
 
 class DropboxProviderExtended(StorageProvider):
     """
     The class that implements the dropbox storage provider.
     """
 
@@ -303,14 +302,32 @@
             )
         except FileNotFoundError:
             pass
 
         upload_dict = self._format_config_dict(config_dict, private_jwk)
         self.upload(upload_dict, config_path, "config")
 
+    def _delete_config(self, display_name: DisplayNameStr) -> bool:
+        """
+        Delete a config from the storage. This is only intended for test purposes.
+
+        Args:
+            display_name: The name of the backend to which we want to upload the job
+
+        Raises:
+            FileNotFoundError: If the status does not exist.
+
+        Returns:
+            Success if the file was deleted successfully
+        """
+        config_path = "Backend_files/Config/" + display_name
+
+        self.delete_file(storage_path=config_path, job_id="config")
+        return True
+
     def upload_public_key(self, public_jwk: JWK, display_name: DisplayNameStr) -> None:
         """
         The function that uploads the spooler public JWK to the storage.
 
         Args:
             public_jwk: The JWK that contains the public key
             display_name : The name of the backend
@@ -322,34 +339,62 @@
         if not public_jwk.key_ops == "verify":
             raise ValueError("The key is not intended for verification")
 
         # make sure that the key does not contain a private key
         if public_jwk.d is not None:
             raise ValueError("The key contains a private key")
 
+        # make sure that the key has the correct kid
+        config_dict = self.get_config(display_name)
+        if public_jwk.kid != config_dict.kid:
+            raise ValueError("The key does not have the correct kid.")
+
         pk_paths = "Backend_files/public_keys"
 
-        self.upload_string(public_jwk.model_dump_json(), pk_paths, display_name)
+        self.upload_string(public_jwk.model_dump_json(), pk_paths, config_dict.kid)
 
     def get_public_key(self, display_name: DisplayNameStr) -> JWK:
         """
         The function that gets the spooler public JWK for the device.
 
         Args:
             display_name : The name of the backend
 
         Returns:
             JWk : The public JWK object
         """
         pk_paths = "Backend_files/public_keys"
+
+        # now get the appropiate kid
+        config_dict = self.get_config(display_name)
+        if config_dict.kid is None:
+            raise ValueError("The kid is not set in the backend configuration.")
+
         public_jwk_dict = self.get_file_content(
-            storage_path=pk_paths, job_id=display_name
+            storage_path=pk_paths, job_id=config_dict.kid
         )
         return JWK(**public_jwk_dict)
 
+    def _delete_public_key(self, kid: str) -> bool:
+        """
+        Delete a public key from the storage. This is only intended for test purposes.
+
+        Args:
+            kid: The key id of the public key
+
+        Raises:
+            FileNotFoundError: If the status does not exist.
+
+        Returns:
+            Success if the file was deleted successfully
+        """
+        pk_paths = "Backend_files/public_keys"
+        self.delete_file(storage_path=pk_paths, job_id=kid)
+        return True
+
     def update_in_database(
         self,
         result_dict: ResultDict,
         status_msg_dict: StatusMsgDict,
         job_id: str,
         display_name: DisplayNameStr,
         private_jwk: Optional[JWK] = None,
@@ -375,36 +420,20 @@
         )
         status_json_name = "status-" + job_id
 
         job_json_name = "job-" + job_id
         job_json_start_dir = "Backend_files/Running_Jobs"
 
         if status_msg_dict.status == "DONE":
-            # let us create the result json file
-            result_json_dir = (
-                "/Backend_files/Result/" + display_name + "/" + extracted_username + "/"
+            self.upload_result(
+                result_dict,
+                display_name,
+                job_id,
+                private_jwk,
             )
-            result_json_name = "result-" + job_id
-
-            # let us see if we should sign the result
-            backend_config = self.get_config(display_name)
-            if backend_config.sign:
-                # get the private key
-                if private_jwk is None:
-                    raise ValueError(
-                        "The private key is not given, but the backend is configured to sign."
-                    )
-                # we should sign the result
-                signed_result = sign_payload(result_dict.model_dump(), private_jwk)
-                self.upload(
-                    signed_result.model_dump(), result_json_dir, result_json_name
-                )
-            else:
-                self.upload(result_dict.model_dump(), result_json_dir, result_json_name)
-
             # now move the job out of the running jobs into the finished jobs
             job_finished_json_dir = (
                 "/Backend_files/Finished_Jobs/"
                 + display_name
                 + "/"
                 + extracted_username
                 + "/"
@@ -534,40 +563,48 @@
 
         self.upload(
             content_dict=job_dict, storage_path=job_json_dir, job_id=job_json_name
         )
         return job_id
 
     def upload_status(
-        self, display_name: DisplayNameStr, username: str, job_id: str
+        self,
+        display_name: DisplayNameStr,
+        username: str,
+        job_id: str,
+        private_jwk: Optional[JWK] = None,
     ) -> StatusMsgDict:
         """
         This function uploads a status file to the backend and creates the status dict.
 
         Args:
             display_name: The name of the backend to which we want to upload the job
             username: The username of the user that is uploading the job
             job_id: The job_id of the job that we want to upload the status for
+            private_jwk: The private key of the backend
 
         Returns:
             The status dict of the job
         """
         status_json_dir = "Backend_files/Status/" + display_name + "/" + username
         status_json_name = "status-" + job_id
         status_draft = {
             "job_id": job_id,
             "status": "INITIALIZING",
             "detail": "Got your json.",
             "error_message": "None",
         }
         status_dict = StatusMsgDict(**status_draft)
-        self.upload(
-            content_dict=status_dict.model_dump(),
-            storage_path=status_json_dir,
-            job_id=status_json_name,
+        self._format_status_dict(
+            status_dict,
+            status_json_dir,
+            display_name,
+            job_id,
+            private_jwk,
+            status_json_name,
         )
         return status_dict
 
     def get_status(
         self, display_name: DisplayNameStr, username: str, job_id: str
     ) -> StatusMsgDict:
         """
@@ -584,24 +621,82 @@
         status_json_dir = "Backend_files/Status/" + display_name + "/" + username
         status_json_name = "status-" + job_id
 
         try:
             status_dict = self.get_file_content(
                 storage_path=status_json_dir, job_id=status_json_name
             )
-            return StatusMsgDict(**status_dict)
         except FileNotFoundError:
             status_draft = {
                 "job_id": job_id,
                 "status": "ERROR",
                 "detail": "Could not find the status file.",
                 "error_message": f"Missing status file for {job_id}.",
             }
             return StatusMsgDict(**status_draft)
 
+        return self._adapt_status_dict(status_dict)
+
+    def _delete_status(
+        self, display_name: DisplayNameStr, username: str, job_id: str
+    ) -> bool:
+        """
+        Delete a status from the storage. This is only intended for test purposes.
+
+        Args:
+            display_name: The name of the backend to which we want to upload the job
+            username: The username of the user that is uploading the job
+            job_id: The job_id of the job that we want to upload the status for
+
+        Raises:
+            FileNotFoundError: If the status does not exist.
+
+        Returns:
+            Success if the file was deleted successfully
+        """
+        status_json_dir = "Backend_files/Status/" + display_name + "/" + username
+        status_json_name = "status-" + job_id
+
+        self.delete_file(storage_path=status_json_dir, job_id=status_json_name)
+        return True
+
+    def upload_result(
+        self,
+        result_dict: ResultDict,
+        display_name: DisplayNameStr,
+        job_id: str,
+        private_jwk: Optional[JWK] = None,
+    ) -> bool:
+        """
+        This function allows us to upload the result file .
+
+        Args:
+            result_dict: The result dictionary
+            display_name: The name of the backend to which we want to upload the job
+            job_id: The job_id of the job that we want to upload the status for
+            private_jwk: The private key of the backend
+
+        Returns:
+            The success of the upload process
+        """
+        extracted_username = job_id.split("-")[2]
+        result_json_dir = (
+            "/Backend_files/Result/" + display_name + "/" + extracted_username + "/"
+        )
+        result_json_name = "result-" + job_id
+
+        return self._common_upload_result(
+            result_dict,
+            display_name,
+            job_id,
+            result_json_dir,
+            result_json_name=result_json_name,
+            private_jwk=private_jwk,
+        )
+
     def get_result(
         self, display_name: DisplayNameStr, username: str, job_id: str
     ) -> ResultDict:
         """
         This function gets the result file from the backend and returns the result dict.
 
         Args:
@@ -629,14 +724,62 @@
                 status="ERROR",
                 header={},
                 results=[],
             )
         backend_config_info = self.get_backend_dict(display_name)
         return self._adapt_result_dict(result_dict, backend_config_info)
 
+    def verify_result(self, display_name: DisplayNameStr, job_id: str) -> bool:
+        """
+        This function verifies the result and returns the success. If the backend does not sign the
+        result, we will reutrn `False` by default, given that we were not able to establish ownership.
+
+        Args:
+            display_name: The name of the backend to which we want to upload the job
+            job_id: The job_id of the job that we want to upload the status for
+
+        Returns:
+            If it was possible to verify the result dict positively.
+        """
+        username = job_id.split("-")[2]
+        result_json_dir = "Backend_files/Result/" + display_name + "/" + username
+        result_json_name = "result-" + job_id
+
+        result_dict = self.get_file_content(
+            storage_path=result_json_dir, job_id=result_json_name
+        )
+        public_jwk = self.get_public_key(display_name)
+
+        result_jws = JWSDict(**result_dict)
+        return result_jws.verify_signature(public_jwk)
+
+    def _delete_result(self, display_name: DisplayNameStr, job_id: str) -> bool:
+        """
+        Delete a result from the storage. This is only intended for test purposes.
+
+        Args:
+            display_name: The name of the backend to which we want to upload the job
+            username: The username of the user that is uploading the job
+            job_id: The job_id of the job that we want to upload the status for
+
+        Raises:
+            FileNotFoundError: If the result does not exist.
+
+        Returns:
+            Success if the file was deleted successfully
+        """
+        extracted_username = job_id.split("-")[2]
+        result_json_dir = (
+            "Backend_files/Result/" + display_name + "/" + extracted_username
+        )
+        result_json_name = "result-" + job_id
+
+        self.delete_file(storage_path=result_json_dir, job_id=result_json_name)
+        return True
+
     def get_next_job_in_queue(
         self, display_name: DisplayNameStr, private_jwk: Optional[JWK] = None
     ) -> NextJobSchema:
         """
         A function that obtains the next job in the queue.
 
         Args:
```

### Comparing `sqooler-0.6.3/src/sqooler/storage_providers/local.py` & `sqooler-0.7.0/src/sqooler/storage_providers/local.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 """
 The module that contains all the necessary logic for communication with the local storage providers.
 """
 
-import uuid
 import json
-
-from typing import Mapping, Optional
+import os
 
 # necessary for the local provider
 import shutil
-import os
+import uuid
+from typing import Mapping, Optional
 
 from ..schemes import (
-    ResultDict,
-    StatusMsgDict,
-    LocalLoginInformation,
     BackendConfigSchemaIn,
-    NextJobSchema,
     DisplayNameStr,
+    LocalLoginInformation,
+    NextJobSchema,
+    ResultDict,
+    StatusMsgDict,
 )
-
-from .base import StorageProvider, validate_active, datetime_handler
-from ..security import JWK, sign_payload
+from ..security import JWK, JWSDict
+from .base import StorageProvider, datetime_handler, validate_active
 
 
 class LocalProviderExtended(StorageProvider):
     """
     Create a file storage that works on the local machine.
     """
 
@@ -215,42 +213,49 @@
         storage_path = "jobs/queued/" + display_name
         job_id = (uuid.uuid4().hex)[:24]
 
         self.upload(content_dict=job_dict, storage_path=storage_path, job_id=job_id)
         return job_id
 
     def upload_status(
-        self, display_name: DisplayNameStr, username: str, job_id: str
+        self,
+        display_name: DisplayNameStr,
+        username: str,
+        job_id: str,
+        private_jwk: Optional[JWK] = None,
     ) -> StatusMsgDict:
         """
         This function uploads a status file to the backend and creates the status dict.
 
         Args:
             display_name: The name of the backend to which we want to upload the job
             username: The username of the user that is uploading the job
             job_id: The job_id of the job that we want to upload the status for
+            private_jwk: The private key of the backend
 
         Returns:
             The status dict of the job
         """
         storage_path = "status/" + display_name
         status_draft = {
             "job_id": job_id,
             "status": "INITIALIZING",
             "detail": "Got your json.",
             "error_message": "None",
         }
 
         # should we also upload the username into the dict ?
         status_dict = StatusMsgDict(**status_draft)
-        # now upload the status dict
-        self.upload(
-            content_dict=status_dict.model_dump(),
-            storage_path=storage_path,
-            job_id=job_id,
+
+        self._format_status_dict(
+            status_dict,
+            storage_path,
+            display_name,
+            job_id,
+            private_jwk,
         )
         return status_dict
 
     def get_status(
         self, display_name: DisplayNameStr, username: str, job_id: str
     ) -> StatusMsgDict:
         """
@@ -266,24 +271,78 @@
         """
         status_json_dir = "status/" + display_name
 
         try:
             status_dict = self.get_file_content(
                 storage_path=status_json_dir, job_id=job_id
             )
-            return StatusMsgDict(**status_dict)
+            # return StatusMsgDict(**status_dict)
         except FileNotFoundError:
             # if the job_id is not valid, we return an error
             return StatusMsgDict(
                 job_id=job_id,
                 status="ERROR",
                 detail="Cannot get status",
                 error_message=f"Could not find status for {display_name} with job_id {job_id}.",
             )
 
+        return self._adapt_status_dict(status_dict)
+
+    def _delete_status(
+        self, display_name: DisplayNameStr, username: str, job_id: str
+    ) -> bool:
+        """
+        Delete a status from the storage. This is only intended for test purposes.
+
+        Args:
+            display_name: The name of the backend to which we want to upload the job
+            username: The username of the user that is uploading the job
+            job_id: The job_id of the job that we want to upload the status for
+
+        Raises:
+            FileNotFoundError: If the status does not exist.
+
+        Returns:
+            Success if the file was deleted successfully
+        """
+        status_json_dir = "status/" + display_name
+
+        self.delete_file(storage_path=status_json_dir, job_id=job_id)
+        return True
+
+    def upload_result(
+        self,
+        result_dict: ResultDict,
+        display_name: DisplayNameStr,
+        job_id: str,
+        private_jwk: Optional[JWK] = None,
+    ) -> bool:
+        """
+        This function allows us to upload the result file .
+
+        Args:
+            result_dict: The result dictionary
+            display_name: The name of the backend to which we want to upload the job
+            job_id: The job_id of the job that we want to upload the status for
+            private_jwk: The private key of the backend
+
+        Returns:
+            The success of the upload process
+        """
+        result_json_dir = "results/" + display_name
+
+        return self._common_upload_result(
+            result_dict,
+            display_name,
+            job_id,
+            result_json_dir,
+            result_json_name=job_id,
+            private_jwk=private_jwk,
+        )
+
     def get_result(
         self, display_name: DisplayNameStr, username: str, job_id: str
     ) -> ResultDict:
         """
         This function gets the result file from the backend and returns the result dict.
 
         Args:
@@ -326,14 +385,54 @@
                 success=False,
                 status="ERROR",
                 header={},
                 results=[],
             )
         return self._adapt_result_dict(result_dict, backend_config_info)
 
+    def verify_result(self, display_name: DisplayNameStr, job_id: str) -> bool:
+        """
+        This function verifies the result and returns the success. If the backend does not sign the
+        result, we will reutrn `False` by default, given that we were not able to establish ownership.
+
+        Args:
+            display_name: The name of the backend to which we want to upload the job
+            job_id: The job_id of the job that we want to upload the status for
+
+        Returns:
+            If it was possible to verify the result dict positively.
+        """
+        result_json_dir = "results/" + display_name
+        result_dict = self.get_file_content(storage_path=result_json_dir, job_id=job_id)
+        public_jwk = self.get_public_key(display_name)
+
+        result_jws = JWSDict(**result_dict)
+        return result_jws.verify_signature(public_jwk)
+
+    def _delete_result(self, display_name: DisplayNameStr, job_id: str) -> bool:
+        """
+        Delete a result from the storage. This is only intended for test purposes.
+
+        Args:
+            display_name: The name of the backend to which we want to upload the job
+            username: The username of the user that is uploading the job
+            job_id: The job_id of the job that we want to upload the status for
+
+        Raises:
+            FileNotFoundError: If the result does not exist.
+
+        Returns:
+            Success if the file was deleted successfully
+        """
+
+        result_json_dir = "results/" + display_name
+
+        self.delete_file(storage_path=result_json_dir, job_id=job_id)
+        return True
+
     def update_config(
         self,
         config_dict: BackendConfigSchemaIn,
         display_name: DisplayNameStr,
         private_jwk: Optional[JWK] = None,
     ) -> None:
         """
@@ -434,17 +533,36 @@
         """
         # path of the configs
         config_path = "/backends/configs"
         backend_config_dict = self.get_file_content(config_path, job_id=display_name)
         typed_config = self._adapt_get_config(backend_config_dict)
         return typed_config
 
+    def _delete_config(self, display_name: DisplayNameStr) -> bool:
+        """
+        Delete a config from the storage. This is only intended for test purposes.
+
+        Args:
+            display_name: The name of the backend to which we want to upload the job
+
+        Raises:
+            FileNotFoundError: If the status does not exist.
+
+        Returns:
+            Success if the file was deleted successfully
+        """
+        config_path = "/backends/configs"
+
+        self.delete_file(storage_path=config_path, job_id=display_name)
+        return True
+
     def upload_public_key(self, public_jwk: JWK, display_name: DisplayNameStr) -> None:
         """
-        The function that uploads the spooler public JWK to the storage.
+        The function that uploads the spooler public JWK to the storage. It should
+        only be used after `upload_config` as the kid is set there.
 
         Args:
             public_jwk: The JWK that contains the public key
             display_name : The name of the backend
 
         Returns:
             None
@@ -453,23 +571,28 @@
         if not public_jwk.key_ops == "verify":
             raise ValueError("The key is not intended for verification")
 
         # make sure that the key does not contain a private key
         if public_jwk.d is not None:
             raise ValueError("The key contains a private key")
 
+        # make sure that the key has the correct kid
+        config_dict = self.get_config(display_name)
+        if public_jwk.kid != config_dict.kid:
+            raise ValueError("The key does not have the correct kid.")
+
         # path of the public keys
         key_path = os.path.join(self.base_path, "backends/public_keys")
         key_path = os.path.normpath(key_path)
         # test if the config path already exists. If it does not, create it
         if not os.path.exists(key_path):
             os.makedirs(key_path)
 
         # this should most likely depend on the kid at some point
-        file_name = display_name + ".json"
+        file_name = f"{public_jwk.kid}.json"
         full_json_path = os.path.join(key_path, file_name)
         secure_path = os.path.normpath(full_json_path)
         with open(secure_path, "w", encoding="utf-8") as json_file:
             json_file.write(public_jwk.model_dump_json())
 
     def get_public_key(self, display_name: DisplayNameStr) -> JWK:
         """
@@ -478,27 +601,48 @@
         Args:
             display_name : The name of the backend
 
         Returns:
             JWk : The public JWK object
         """
 
+        # first we have to get the kid
+        config_info = self.get_config(display_name)
+
         # path of the configs
         key_path = os.path.join(self.base_path, "backends/public_keys")
-        file_name = display_name + ".json"
+        file_name = f"{config_info.kid}.json"
         full_json_path = os.path.join(key_path, file_name)
         secure_path = os.path.normpath(full_json_path)
         with open(secure_path, "r", encoding="utf-8") as json_file:
             public_key_dict = json.load(json_file)
 
         if not public_key_dict:
             raise FileNotFoundError("The backend does not exist for the given storage.")
 
         return JWK(**public_key_dict)
 
+    def _delete_public_key(self, kid: str) -> bool:
+        """
+        Delete a public key from the storage. This is only intended for test purposes.
+
+        Args:
+            kid: The key id of the public key
+
+        Raises:
+            FileNotFoundError: If the status does not exist.
+
+        Returns:
+            Success if the file was deleted successfully
+        """
+        key_path = "backends/public_keys"
+
+        self.delete_file(storage_path=key_path, job_id=kid)
+        return True
+
     def update_in_database(
         self,
         result_dict: ResultDict,
         status_msg_dict: StatusMsgDict,
         job_id: str,
         display_name: DisplayNameStr,
         private_jwk: Optional[JWK] = None,
@@ -520,30 +664,19 @@
         # check if the job is done or had an error
         if status_msg_dict.status == "DONE":
             # test if the result dict is None
             if result_dict is None:
                 raise ValueError(
                     "The 'result_dict' argument cannot be None if the job is done."
                 )
-            # let us create the result json file
-            result_json_dir = "results/" + display_name
-
-            # let us see if we should sign the result
-            backend_config = self.get_config(display_name)
-            if backend_config.sign:
-                # get the private key
-                if private_jwk is None:
-                    raise ValueError(
-                        "The private key is not given, but the backend is configured to sign."
-                    )
-                # we should sign the result
-                signed_result = sign_payload(result_dict.model_dump(), private_jwk)
-                self.upload(signed_result.model_dump(), result_json_dir, job_id)
-            else:
-                self.upload(result_dict.model_dump(), result_json_dir, job_id)
+            result_uploaded = self.upload_result(
+                result_dict, display_name, job_id, private_jwk
+            )
+            if not result_uploaded:
+                raise ValueError("The result was not uploaded successfully.")
 
             # now move the job out of the running jobs into the finished jobs
             job_finished_json_dir = "jobs/finished/" + display_name
 
             self.move_file(job_json_start_dir, job_finished_json_dir, job_id)
 
         elif status_msg_dict.status == "ERROR":
```

### Comparing `sqooler-0.6.3/src/sqooler/storage_providers/mongodb.py` & `sqooler-0.7.0/src/sqooler/storage_providers/mongodb.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 """
 The module that contains all the necessary logic for communication with the MongoDb storage providers.
 """
 
 import uuid
-from typing import Optional
 from datetime import timezone
+from typing import Optional
+
+from bson.codec_options import CodecOptions
+from bson.errors import InvalidId
+from bson.objectid import ObjectId
 
 # necessary for the mongodb provider
 from pymongo.mongo_client import MongoClient
-from bson.objectid import ObjectId
-from bson.errors import InvalidId
-from bson.codec_options import CodecOptions
 
 from ..schemes import (
-    ResultDict,
-    StatusMsgDict,
-    MongodbLoginInformation,
     BackendConfigSchemaIn,
-    NextJobSchema,
     DisplayNameStr,
+    MongodbLoginInformation,
+    NextJobSchema,
+    ResultDict,
+    StatusMsgDict,
 )
-
+from ..security import JWK, JWSDict
 from .base import StorageProvider, validate_active
-from ..security import JWK, sign_payload
 
 
 class MongodbProviderExtended(StorageProvider):
     """
     The access to the mongodb
     """
 
@@ -394,14 +394,45 @@
         # mypy happy, we have to check if the signed_backend_config_dict is not None
         elif signed_backend_config_dict:
             payload = signed_backend_config_dict["payload"]
             return BackendConfigSchemaIn(**payload)
 
         raise FileNotFoundError("The backend does not exist for the given storage.")
 
+    def _delete_config(self, display_name: DisplayNameStr) -> bool:
+        """
+        Delete a config from the storage. This is only intended for test purposes.
+
+        Args:
+            display_name: The name of the backend to which we want to upload the job
+
+        Raises:
+            FileNotFoundError: If the config does not exist.
+
+        Returns:
+            Success if the file was deleted successfully
+        """
+
+        config_dict = self.get_config(display_name)
+        config_path = "backends/configs"
+        database = self.client["backends"]
+        collection = database["configs"]
+
+        if not config_dict.sign:
+            document_to_find = {"display_name": display_name}
+        else:
+            document_to_find = {"payload.display_name": display_name}
+
+        result_found = collection.find_one(document_to_find)
+        if result_found is None:
+            raise FileNotFoundError(f"the config for {display_name} does not exist.")
+        self.delete_file(config_path, str(result_found["_id"]))
+
+        return True
+
     def upload_job(
         self, job_dict: dict, display_name: DisplayNameStr, username: str
     ) -> str:
         """
         Upload the job to the storage provider.
 
         Args:
@@ -416,42 +447,49 @@
         storage_path = "jobs/queued/" + display_name
         job_id = (uuid.uuid4().hex)[:24]
 
         self.upload(content_dict=job_dict, storage_path=storage_path, job_id=job_id)
         return job_id
 
     def upload_status(
-        self, display_name: DisplayNameStr, username: str, job_id: str
+        self,
+        display_name: DisplayNameStr,
+        username: str,
+        job_id: str,
+        private_jwk: Optional[JWK] = None,
     ) -> StatusMsgDict:
         """
         This function uploads a status file to the backend and creates the status dict.
 
         Args:
             display_name: The name of the backend to which we want to upload the job
             username: The username of the user that is uploading the job
             job_id: The job_id of the job that we want to upload the status for
+            private_jwk: The private key of the backend
 
         Returns:
             The status dict of the job
         """
         storage_path = "status/" + display_name
         status_draft = {
             "job_id": job_id,
             "status": "INITIALIZING",
             "detail": "Got your json.",
             "error_message": "None",
         }
 
         # should we also upload the username into the dict ?
         status_dict = StatusMsgDict(**status_draft)
-        # now upload the status dict
-        self.upload(
-            content_dict=status_dict.model_dump(),
-            storage_path=storage_path,
-            job_id=job_id,
+
+        self._format_status_dict(
+            status_dict,
+            storage_path,
+            display_name,
+            job_id,
+            private_jwk,
         )
         return status_dict
 
     def get_status(
         self, display_name: DisplayNameStr, username: str, job_id: str
     ) -> StatusMsgDict:
         """
@@ -467,24 +505,77 @@
         """
         status_json_dir = "status/" + display_name
 
         try:
             status_dict = self.get_file_content(
                 storage_path=status_json_dir, job_id=job_id
             )
-            return StatusMsgDict(**status_dict)
         except FileNotFoundError as err:
             # if the job_id is not valid, we return an error
             return StatusMsgDict(
                 job_id=job_id,
                 status="ERROR",
                 detail="The job_id is not valid.",
                 error_message=str(err),
             )
 
+        return self._adapt_status_dict(status_dict)
+
+    def _delete_status(
+        self, display_name: DisplayNameStr, username: str, job_id: str
+    ) -> bool:
+        """
+        Delete a status from the storage. This is only intended for test purposes.
+
+        Args:
+            display_name: The name of the backend to which we want to upload the job
+            username: The username of the user that is uploading the job
+            job_id: The job_id of the job that we want to upload the status for
+
+        Raises:
+            FileNotFoundError: If the status does not exist.
+
+        Returns:
+            Success if the file was deleted successfully
+        """
+        status_json_dir = "status/" + display_name
+
+        self.delete_file(storage_path=status_json_dir, job_id=job_id)
+        return True
+
+    def upload_result(
+        self,
+        result_dict: ResultDict,
+        display_name: DisplayNameStr,
+        job_id: str,
+        private_jwk: Optional[JWK] = None,
+    ) -> bool:
+        """
+        This function allows us to upload the result file .
+
+        Args:
+            result_dict: The result dictionary
+            display_name: The name of the backend to which we want to upload the job
+            job_id: The job_id of the job that we want to upload the status for
+            private_jwk: The private key of the backend
+
+        Returns:
+            The success of the upload process
+        """
+        result_json_dir = "results/" + display_name
+
+        return self._common_upload_result(
+            result_dict,
+            display_name,
+            job_id,
+            result_json_dir,
+            result_json_name=job_id,
+            private_jwk=private_jwk,
+        )
+
     def get_result(
         self, display_name: DisplayNameStr, username: str, job_id: str
     ) -> ResultDict:
         """
         This function gets the result file from the backend and returns the result dict.
 
         Args:
@@ -512,14 +603,54 @@
                 status="ERROR",
                 header={},
                 results=[],
             )
         backend_config_info = self.get_backend_dict(display_name)
         return self._adapt_result_dict(result_dict, backend_config_info)
 
+    def verify_result(self, display_name: DisplayNameStr, job_id: str) -> bool:
+        """
+        This function verifies the result and returns the success. If the backend does not sign the
+        result, we will reutrn `False` by default, given that we were not able to establish ownership.
+
+        Args:
+            display_name: The name of the backend to which we want to upload the job
+            job_id: The job_id of the job that we want to upload the status for
+
+        Returns:
+            If it was possible to verify the result dict positively.
+        """
+        result_json_dir = "results/" + display_name
+        result_dict = self.get_file_content(storage_path=result_json_dir, job_id=job_id)
+        public_jwk = self.get_public_key(display_name)
+
+        result_jws = JWSDict(**result_dict)
+        return result_jws.verify_signature(public_jwk)
+
+    def _delete_result(self, display_name: DisplayNameStr, job_id: str) -> bool:
+        """
+        Delete a result from the storage. This is only intended for test purposes.
+
+        Args:
+            display_name: The name of the backend to which we want to upload the job
+            username: The username of the user that is uploading the job
+            job_id: The job_id of the job that we want to upload the status for
+
+        Raises:
+            FileNotFoundError: If the result does not exist.
+
+        Returns:
+            Success if the file was deleted successfully
+        """
+
+        result_json_dir = "results/" + display_name
+
+        self.delete_file(storage_path=result_json_dir, job_id=job_id)
+        return True
+
     def upload_public_key(self, public_jwk: JWK, display_name: DisplayNameStr) -> None:
         """
         The function that uploads the spooler public JWK to the storage.
 
         Args:
             public_jwk: The JWK that contains the public key
             display_name : The name of the backend
@@ -533,17 +664,22 @@
 
         # make sure that the key does not contain a private key
         if public_jwk.d is not None:
             raise ValueError("The key contains a private key")
 
         pk_paths = "backends/public_keys"
 
+        # make sure that the key has the correct kid
+        config_dict = self.get_config(display_name)
+        if public_jwk.kid != config_dict.kid:
+            raise ValueError("The key does not have the correct kid.")
+
         # first we have to check if the device already exists in the database
 
-        document_to_find = {"display_name": display_name}
+        document_to_find = {"kid": config_dict.kid}
 
         # get the database on which we work
         database = self.client["backends"]
 
         # get the collection on which we work
         collection = database["public_keys"]
 
@@ -554,15 +690,14 @@
                 content_dict=public_jwk.model_dump(),
                 storage_path=pk_paths,
                 job_id=result_found["_id"],
             )
             return
 
         # if the device does not exist, we have to create it
-
         config_id = uuid.uuid4().hex[:24]
         self.upload(public_jwk.model_dump(), pk_paths, config_id)
 
     def get_public_key(self, display_name: DisplayNameStr) -> JWK:
         """
         The function that gets the spooler public JWK for the device.
 
@@ -572,24 +707,53 @@
         Returns:
             JWk : The public JWK object
         """
         # get the database on which we work
         database = self.client["backends"]
         collection = database["public_keys"]
 
+        # now get the appropiate kid
+        config_dict = self.get_config(display_name)
+        if config_dict.kid is None:
+            raise ValueError("The kid is not set in the backend configuration.")
+
         # create the filter for the document with display_name that is equal to display_name
-        document_to_find = {"display_name": display_name}
+        document_to_find = {"kid": config_dict.kid}
         public_jwk_dict = collection.find_one(document_to_find)
 
         if not public_jwk_dict:
             raise FileNotFoundError("The backend does not exist for the given storage.")
 
         public_jwk_dict.pop("_id")
         return JWK(**public_jwk_dict)
 
+    def _delete_public_key(self, kid: str) -> bool:
+        """
+        Delete a public key from the storage. This is only intended for test purposes.
+
+        Args:
+            kid: The key id of the public key
+
+        Raises:
+            FileNotFoundError: If the public key does not exist.
+
+        Returns:
+            Success if the file was deleted successfully
+        """
+        key_path = "backends/public_keys"
+        document_to_find = {"kid": kid}
+
+        database = self.client["backends"]
+        collection = database["public_keys"]
+        result_found = collection.find_one(document_to_find)
+        if result_found is None:
+            raise FileNotFoundError(f"The public key with kid {kid} does not exist")
+        self.delete_file(key_path, str(result_found["_id"]))
+        return True
+
     def update_in_database(
         self,
         result_dict: ResultDict | None,
         status_msg_dict: StatusMsgDict,
         job_id: str,
         display_name: DisplayNameStr,
         private_jwk: Optional[JWK] = None,
@@ -619,30 +783,19 @@
         # check if the job is done or had an error
         if status_msg_dict.status == "DONE":
             # test if the result dict is None
             if result_dict is None:
                 raise ValueError(
                     "The 'result_dict' argument cannot be None if the job is done."
                 )
-            # let us create the result json file
-            result_json_dir = "results/" + display_name
-
-            # let us see if we should sign the result
-            backend_config = self.get_config(display_name)
-            if backend_config.sign:
-                # get the private key
-                if private_jwk is None:
-                    raise ValueError(
-                        "The private key is not given, but the backend is configured to sign."
-                    )
-                # we should sign the result
-                signed_result = sign_payload(result_dict.model_dump(), private_jwk)
-                self.upload(signed_result.model_dump(), result_json_dir, job_id)
-            else:
-                self.upload(result_dict.model_dump(), result_json_dir, job_id)
+            result_uploaded = self.upload_result(
+                result_dict, display_name, job_id, private_jwk
+            )
+            if not result_uploaded:
+                raise ValueError("The result was not uploaded successfully.")
 
             # now move the job out of the running jobs into the finished jobs
             job_finished_json_dir = "jobs/finished/" + display_name
             self.move_file(job_json_start_dir, job_finished_json_dir, job_id)
 
         elif status_msg_dict.status == "ERROR":
             # because there was an error, we move the job to the deleted jobs
```

### Comparing `sqooler-0.6.3/src/sqooler/utils.py` & `sqooler-0.7.0/src/sqooler/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """
 This module contains some functions that are especially helpful for deployment of the 
 sqooler package.
 """
 
+import logging
 import time
 import traceback
-import logging
 
 import regex as re
+from decouple import config
 from pydantic import ValidationError
 
-from .schemes import get_init_results, get_init_status, NextJobSchema
+from .schemes import NextJobSchema, get_init_results, get_init_status
+from .security import public_from_private_jwk
 from .spoolers import Spooler
 from .storage_providers.base import StorageProvider
-from .security import public_from_private_jwk
 
 
 def update_backends(
     storage_provider: StorageProvider, backends: dict[str, Spooler]
 ) -> None:
     """
     Update the backends on the storage. Uploads it as a new one if it fails.
@@ -30,42 +31,46 @@
         # the content
         backend_config_dict = spooler.get_configuration()
         # set the display name
         backend_config_dict.display_name = requested_backend
         # upload the public key if the backend has one and is designed to sign
         if spooler.sign:
             private_jwk = spooler.get_private_jwk()
-            public_jwk = public_from_private_jwk(private_jwk)
-            storage_provider.upload_public_key(public_jwk, requested_backend)
         else:
             private_jwk = None
 
         # upload the content through the storage provider
         try:
             storage_provider.update_config(
                 backend_config_dict, requested_backend, private_jwk=private_jwk
             )
+
             logging.info(
                 "Updated the config for %s .",
                 requested_backend,
             )
         except FileNotFoundError:
             # this should become a log
             logging.warning(
                 "Failed to update the configuration for %s . Uploading it as a new one.",
                 requested_backend,
             )
-            if spooler.sign:
-                storage_provider.upload_config(
-                    backend_config_dict, requested_backend, private_jwk
-                )
-            else:
-                storage_provider.upload_config(
-                    backend_config_dict, requested_backend, private_jwk=None
-                )
+            storage_provider.upload_config(
+                backend_config_dict, requested_backend, private_jwk
+            )
+
+        if spooler.sign:
+            # this line is IMHO needless but somehow mypy thinks that it could be a
+            # None (no idea how this could happen)
+            private_jwk = spooler.get_private_jwk()
+
+            # this has to happen after the config was uploaded to be sure
+            # the we know the appropiate kid
+            public_jwk = public_from_private_jwk(private_jwk)
+            storage_provider.upload_public_key(public_jwk, requested_backend)
 
 
 def main(
     storage_provider: StorageProvider,
     backends: dict[str, Spooler],
     num_iter: int = 0,
 ) -> None:
@@ -82,16 +87,18 @@
     # set the appropiate display names for all the back-ends
     for requested_backend, spooler in backends.items():
         # the content
         spooler.display_name = requested_backend
 
     counter = 0
     # loop which is looking for the jobs
+
+    t_wait_main = config("T_WAIT_MAIN", cast=float, default=0.2)
     while num_iter == 0 or counter < num_iter:
-        time.sleep(0.2)
+        time.sleep(t_wait_main)
         # the following a fancy for loop of going through all the back-ends in the list
         requested_backend = backends_list[0]
         backends_list.append(backends_list.pop(0))
 
         spooler = backends[requested_backend]
         # let us first see if jobs are waiting
         logging.info("Looking for jobs in %s", requested_backend)
@@ -143,15 +150,14 @@
             # Update status dict
             status_msg_dict.status = "ERROR"
             status_msg_dict.detail += "; " + slimmed_tb
             status_msg_dict.error_message += "; " + slimmed_tb
             logging.exception("Error in add_job for %s .", requested_backend)
 
         logging.debug("Updating in database.")
-        spooler.get_private_jwk()
         storage_provider.update_in_database(
             result_dict,
             status_msg_dict,
             job_dict.job_id,
             requested_backend,
             private_jwk,
         )
```

### Comparing `sqooler-0.6.3/PKG-INFO` & `sqooler-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: sqooler
-Version: 0.6.3
+Version: 0.7.0
 Summary: Code that enables validated cloud access to quantum hardware (simulators)
 Home-page: https://github.com/Alqor-UG/sqooler
 License: Unlicense
 Keywords: pydantic,quantum-hardware,sdk-python
 Author: fretchen
 Author-email: fred.jendrzejewski@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: cryptography (>=42.0.5,<43.0.0)
 Requires-Dist: dropbox (>=11.36.2,<12.0.0)
 Requires-Dist: pydantic (>=2.3.0,<3.0.0)
 Requires-Dist: pymongo (>=4.3.3,<5.0.0)
 Requires-Dist: regex (>=2023.6.3,<2024.0.0)
 Requires-Dist: setuptools (>=69.0.3,<70.0.0)
 Project-URL: Documentation, https://alqor-ug.github.io/sqooler
```

