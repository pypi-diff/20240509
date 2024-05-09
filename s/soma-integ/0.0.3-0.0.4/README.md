# Comparing `tmp/soma_integ-0.0.3.tar.gz` & `tmp/soma_integ-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soma_integ-0.0.3.tar", last modified: Wed Apr 17 06:59:25 2024, max compression
+gzip compressed data, was "soma_integ-0.0.4.tar", last modified: Thu May  9 11:19:45 2024, max compression
```

## Comparing `soma_integ-0.0.3.tar` & `soma_integ-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-04-17 06:59:25.561210 soma_integ-0.0.3/
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     1073 2024-04-15 11:21:18.000000 soma_integ-0.0.3/LICENSE
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      750 2024-04-17 06:59:25.560994 soma_integ-0.0.3/PKG-INFO
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-04-15 11:15:15.000000 soma_integ-0.0.3/README.md
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      838 2024-04-17 06:58:36.000000 soma_integ-0.0.3/pyproject.toml
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)       38 2024-04-17 06:59:25.561251 soma_integ-0.0.3/setup.cfg
-drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-04-17 06:59:25.556439 soma_integ-0.0.3/src/
-drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-04-17 06:59:25.559332 soma_integ-0.0.3/src/soma_integ/
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      469 2024-03-09 18:26:42.000000 soma_integ-0.0.3/src/soma_integ/__init__.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      681 2024-03-04 18:10:58.000000 soma_integ-0.0.3/src/soma_integ/basemodel.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     1841 2024-03-04 18:10:58.000000 soma_integ-0.0.3/src/soma_integ/config.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     2298 2024-03-09 19:19:18.000000 soma_integ-0.0.3/src/soma_integ/data.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     2038 2024-03-04 18:10:58.000000 soma_integ-0.0.3/src/soma_integ/evaluation.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      272 2024-03-04 18:10:58.000000 soma_integ-0.0.3/src/soma_integ/methods.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     4851 2024-03-09 18:31:58.000000 soma_integ-0.0.3/src/soma_integ/optimization.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      197 2024-03-04 18:10:58.000000 soma_integ-0.0.3/src/soma_integ/utils.py
-drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-04-17 06:59:25.560654 soma_integ-0.0.3/src/soma_integ.egg-info/
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      750 2024-04-17 06:59:25.000000 soma_integ-0.0.3/src/soma_integ.egg-info/PKG-INFO
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      448 2024-04-17 06:59:25.000000 soma_integ-0.0.3/src/soma_integ.egg-info/SOURCES.txt
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)        1 2024-04-17 06:59:25.000000 soma_integ-0.0.3/src/soma_integ.egg-info/dependency_links.txt
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)       31 2024-04-17 06:59:25.000000 soma_integ-0.0.3/src/soma_integ.egg-info/requires.txt
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)       11 2024-04-17 06:59:25.000000 soma_integ-0.0.3/src/soma_integ.egg-info/top_level.txt
-drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-04-17 06:59:25.560461 soma_integ-0.0.3/tests/
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-04-15 11:14:17.000000 soma_integ-0.0.3/tests/test.py
+drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-09 11:19:45.855854 soma_integ-0.0.4/
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     1073 2024-04-15 11:21:18.000000 soma_integ-0.0.4/LICENSE
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      750 2024-05-09 11:19:45.855612 soma_integ-0.0.4/PKG-INFO
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-04-15 11:15:15.000000 soma_integ-0.0.4/README.md
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      838 2024-05-09 11:18:22.000000 soma_integ-0.0.4/pyproject.toml
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)       38 2024-05-09 11:19:45.855902 soma_integ-0.0.4/setup.cfg
+drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-09 11:19:45.851376 soma_integ-0.0.4/src/
+drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-09 11:19:45.854000 soma_integ-0.0.4/src/soma_integ/
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      472 2024-05-09 11:16:18.000000 soma_integ-0.0.4/src/soma_integ/__init__.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     1841 2024-03-04 18:10:58.000000 soma_integ-0.0.4/src/soma_integ/config.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     2335 2024-05-09 11:14:23.000000 soma_integ-0.0.4/src/soma_integ/data.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     2038 2024-03-04 18:10:58.000000 soma_integ-0.0.4/src/soma_integ/evaluation.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      272 2024-03-04 18:10:58.000000 soma_integ-0.0.4/src/soma_integ/methods.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      689 2024-05-09 11:12:43.000000 soma_integ-0.0.4/src/soma_integ/model.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     5015 2024-05-09 11:16:18.000000 soma_integ-0.0.4/src/soma_integ/optimization.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      197 2024-03-04 18:10:58.000000 soma_integ-0.0.4/src/soma_integ/utils.py
+drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-09 11:19:45.855238 soma_integ-0.0.4/src/soma_integ.egg-info/
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      750 2024-05-09 11:19:45.000000 soma_integ-0.0.4/src/soma_integ.egg-info/PKG-INFO
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      444 2024-05-09 11:19:45.000000 soma_integ-0.0.4/src/soma_integ.egg-info/SOURCES.txt
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)        1 2024-05-09 11:19:45.000000 soma_integ-0.0.4/src/soma_integ.egg-info/dependency_links.txt
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)       31 2024-05-09 11:19:45.000000 soma_integ-0.0.4/src/soma_integ.egg-info/requires.txt
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)       11 2024-05-09 11:19:45.000000 soma_integ-0.0.4/src/soma_integ.egg-info/top_level.txt
+drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-09 11:19:45.855069 soma_integ-0.0.4/tests/
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-04-15 11:14:17.000000 soma_integ-0.0.4/tests/test.py
```

### Comparing `soma_integ-0.0.3/LICENSE` & `soma_integ-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `soma_integ-0.0.3/PKG-INFO` & `soma_integ-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soma_integ
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package for integrating implementation and evaluation of machine learning platforms
 Author-email: Sobhan Ahmadian Moghadam <sobhan.ahmadian.moghadam@gmail.com>, Arman Rezaei <arman.x.rezaei@gmail.com>
 Project-URL: Homepage, https://github.com/sobhanAhmadian/soma_integrate
 Project-URL: Issues, https://github.com/sobhanAhmadian/soma_integrate/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `soma_integ-0.0.3/pyproject.toml` & `soma_integ-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "soma_integ"
-version = "0.0.3"
+version = "0.0.4"
 dependencies = ["numpy", "scikit-learn"]
 authors = [
     { name = "Sobhan Ahmadian Moghadam", email = "sobhan.ahmadian.moghadam@gmail.com" },
     { name = "Arman Rezaei", email = "arman.x.rezaei@gmail.com" },
 ]
 description = "A package for integrating implementation and evaluation of machine learning platforms"
 readme = "README.md"
```

### Comparing `soma_integ-0.0.3/src/soma_integ/basemodel.py` & `soma_integ-0.0.4/src/soma_integ/model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import abc
 
 from .utils import logging as base_logger
 
 logger = base_logger.getLogger(__name__)
 
 
-class BaseModel(abc.ABC):
+class ModelHandler(abc.ABC):
     def __init__(self, model_config) -> None:
         self.model_config = model_config
         self.model = None
 
     @abc.abstractmethod
     def destroy(self):
         logger.info(f'Model {self.model} has been deleted')
@@ -20,11 +20,11 @@
         raise NotImplementedError
 
     @abc.abstractmethod
     def summary(self):
         raise NotImplementedError
 
 
-class ModelFactory(abc.ABC):
+class HandlerFactory(abc.ABC):
     @abc.abstractmethod
-    def make_model(self) -> BaseModel:
+    def make_model(self) -> ModelHandler:
         raise NotImplementedError
```

### Comparing `soma_integ-0.0.3/src/soma_integ/config.py` & `soma_integ-0.0.4/src/soma_integ/config.py`

 * *Files identical despite different names*

### Comparing `soma_integ-0.0.3/src/soma_integ/data.py` & `soma_integ-0.0.4/src/soma_integ/data.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import abc
+import random
+
 import torch
 
 from .utils import logging as base_logger
 
 logger = base_logger.getLogger(__name__)
 
 
@@ -22,22 +24,24 @@
 class TrainTestSpliter(abc.ABC):
 
     def __init__(self, k):
         self.k = k
 
     @abc.abstractmethod
     def split(self, i):  # Return Train and Test Data
-        logger.info(f'splitting {i}th fold')
+        logger.info(f"splitting {i}th fold")
         raise NotImplementedError
 
 
 class SimplePytorchData(Data):
     def __init__(self, X: torch.Tensor, y: torch.Tensor, **kwargs) -> None:
         super().__init__(**kwargs)
-        logger.info(f'Initializing SimplePytorchData with X shape : {X.shape} and y shape : {y.shape}')
+        logger.info(
+            f"Initializing SimplePytorchData with X shape : {X.shape} and y shape : {y.shape}"
+        )
         self.X = X
         self.y = y
 
     def extend(self, X: torch.Tensor, y: torch.Tensor):
         if self.X is None or self.y is None:
             self.X = X
             self.y = y
@@ -49,15 +53,15 @@
         return self.y[indices], self.y[indices]
 
 
 class SimplePytorchDataTrainTestSpliter(TrainTestSpliter):
 
     def __init__(self, k, simple_data):
         super().__init__(k)
-        logger.info(f'Initializing SimplePytorchDataTrainTestSpliter')
+        logger.info(f"Initializing SimplePytorchDataTrainTestSpliter")
         self.X = simple_data.X
         self.y = simple_data.y
 
         self.data_size = simple_data.X.shape[0]
 
         subsets = dict()
         subset_size = int(self.data_size / self.k)
```

### Comparing `soma_integ-0.0.3/src/soma_integ/evaluation.py` & `soma_integ-0.0.4/src/soma_integ/evaluation.py`

 * *Files identical despite different names*

### Comparing `soma_integ-0.0.3/src/soma_integ/optimization.py` & `soma_integ-0.0.4/src/soma_integ/optimization.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,98 +1,113 @@
 import abc
 import os.path
 import random
+
 import torch
-from torch.utils.data import TensorDataset, DataLoader
+from torch.utils.data import DataLoader, TensorDataset
 
-from .basemodel import BaseModel, ModelFactory
 from .config import OptimizerConfig
-from .data import Data, TrainTestSpliter, SimplePytorchData
+from .data import Data, SimplePytorchData, TrainTestSpliter
 from .evaluation import Result, get_prediction_results
+from .model import HandlerFactory, ModelHandler
 from .utils import logging as base_logger
 
 logger = base_logger.getLogger(__name__)
 
 
 class Trainer(abc.ABC):
     @abc.abstractmethod
-    def train(self, model: BaseModel, data: Data, config: OptimizerConfig) -> Result:
+    def train(self, model: ModelHandler, data: Data, config: OptimizerConfig) -> Result:
         raise NotImplementedError
 
 
 class Tester(abc.ABC):
     @abc.abstractmethod
-    def test(self, model: BaseModel, data: Data, config: OptimizerConfig) -> Result:
+    def test(self, model: ModelHandler, data: Data, config: OptimizerConfig) -> Result:
         raise NotImplementedError
 
 
-def cross_validation(train_test_spliter: TrainTestSpliter, model_factory: ModelFactory, trainer: Trainer,
-                     tester: Tester, config: OptimizerConfig) -> Result:
+def cross_validation(
+    train_test_spliter: TrainTestSpliter,
+    model_factory: HandlerFactory,
+    trainer: Trainer,
+    tester: Tester,
+    config: OptimizerConfig,
+) -> Result:
     k = train_test_spliter.k
-    logger.info(f'Start {k}-fold Cross Validation with config : {config.exp_name}')
+    logger.info(f"Start {k}-fold Cross Validation with config : {config.exp_name}")
 
     result = Result()
     for i in range(k):
         logger.info(f"---- Fold {i + 1} ----")
 
         train_data, test_data = train_test_spliter.split(i)
 
         model = model_factory.make_model()
         trainer.train(model=model, data=train_data, config=config)
         test_result = tester.test(model=model, data=test_data, config=config)
-        logger.info(f'Result of fold {i + 1} : {test_result.get_result()}')
+        logger.info(f"Result of fold {i + 1} : {test_result.get_result()}")
         model.destroy()
 
         result.add(test_result)
 
     result.divide(k=k)
 
     logger.info(
-        f'{k}-fold result: avg_auc: {result.auc}, avg_acc: {result.acc}, avg_f1: {result.f1}, avg_aupr: {result.aupr}')
+        f"{k}-fold result: avg_auc: {result.auc}, avg_acc: {result.acc}, avg_f1: {result.f1}, avg_aupr: {result.aupr}"
+    )
 
     return result
 
 
-def _batch_optimize(loader, model, config: OptimizerConfig, ):
+def _batch_optimize(
+    loader,
+    model,
+    config: OptimizerConfig,
+):
     model.classifier.train()
     optimizer = config.optimizer(model.classifier.parameters(), lr=config.lr)
 
     for epoch in range(config.n_epoch):
         running_loss = 0.0
         for j, data in enumerate(loader, 0):
             X, y = data
 
-            loss, running_loss = predict_error(X, config.criterion, model, running_loss, y)
-            backpropagation(loss, optimizer)
+            loss, running_loss = _predict_error(
+                X, config.criterion, model, running_loss, y
+            )
+            _backpropagation(loss, optimizer)
 
             if j % config.report_size == config.report_size - 1:
                 loss = running_loss / (config.report_size * config.batch_size)
-                logger.info(f'loss: {loss:.4f}    [{epoch + 1}, {j + 1:5d}]')
+                logger.info(f"loss: {loss:.4f}    [{epoch + 1}, {j + 1:5d}]")
                 running_loss = 0
 
         if config.save:
             if epoch % 5 == 0 or epoch == config.n_epoch - 1:
-                m = os.path.join(config.save_path, model.model_config.model_name + ".pth")
+                m = os.path.join(
+                    config.save_path, model.model_config.model_name + ".pth"
+                )
                 torch.save(model.classifier.state_dict(), m)
 
 
-def predict_error(X, loss_function, model, running_loss, y):
+def _predict_error(X, loss_function, model, running_loss, y):
     pred = model.classifier(X)
     loss = loss_function(pred, y)
     running_loss += loss.item()
     return loss, running_loss
 
 
-def backpropagation(loss, optimizer):
+def _backpropagation(loss, optimizer):
     optimizer.zero_grad()
     loss.backward()
     optimizer.step()
 
 
-def _evaluate(model: BaseModel, loader, config: OptimizerConfig):
+def _evaluate(model: ModelHandler, loader, config: OptimizerConfig):
     model.classifier.eval()
     total_labels = []
     total_predictions = []
     total_loss = 0.0
     for data in loader:
         inputs, labels = data
         outputs = model.predict(inputs)
@@ -101,34 +116,41 @@
         total_predictions.extend(torch.sigmoid(outputs).cpu().numpy())
     result = get_prediction_results(total_labels, total_predictions, config.threshold)
     result.loss = total_loss / len(loader)
     return result
 
 
 class SimpleTrainer(Trainer):
-    def train(self, model: BaseModel, data: SimplePytorchData, config: OptimizerConfig) -> Result:
-        logger.info(f'Running Simple Trainer with config : {config.exp_name}')
+    def train(
+        self, model: ModelHandler, data: SimplePytorchData, config: OptimizerConfig
+    ) -> Result:
+        logger.info(f"Running Simple Trainer with config : {config.exp_name}")
 
-        logger.info(f'moving data and model to {config.device}')
+        logger.info(f"moving data and model to {config.device}")
         model.classifier = model.classifier.to(config.device)
         dataset = TensorDataset(data.X.to(config.device), data.y.to(config.device))
         loader = DataLoader(dataset, batch_size=config.batch_size, shuffle=True)
 
         _batch_optimize(loader, model, config)
         result = _evaluate(model, loader, config)
 
-        logger.info(f'Result on Train Data : {result.get_result()}')
+        logger.info(f"Result on Train Data : {result.get_result()}")
         return result
 
 
 class SimpleTester(Tester):
-    def test(self, model: BaseModel, data: SimplePytorchData, config: OptimizerConfig = None) -> Result:
-        logger.info(f'Running Simple Tester with config : {config.exp_name}')
+    def test(
+        self,
+        model: ModelHandler,
+        data: SimplePytorchData,
+        config: OptimizerConfig = None,
+    ) -> Result:
+        logger.info(f"Running Simple Tester with config : {config.exp_name}")
 
-        logger.info(f'moving data and model to {config.device}')
+        logger.info(f"moving data and model to {config.device}")
         model.classifier = model.classifier.to(config.device)
         dataset = TensorDataset(data.X.to(config.device), data.y.to(config.device))
         loader = DataLoader(dataset, batch_size=config.batch_size, shuffle=True)
         result = _evaluate(model, loader, config)
 
-        logger.info(f'Result on Test Data : {result.get_result()}')
+        logger.info(f"Result on Test Data : {result.get_result()}")
         return result
```

### Comparing `soma_integ-0.0.3/src/soma_integ.egg-info/PKG-INFO` & `soma_integ-0.0.4/src/soma_integ.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soma_integ
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package for integrating implementation and evaluation of machine learning platforms
 Author-email: Sobhan Ahmadian Moghadam <sobhan.ahmadian.moghadam@gmail.com>, Arman Rezaei <arman.x.rezaei@gmail.com>
 Project-URL: Homepage, https://github.com/sobhanAhmadian/soma_integrate
 Project-URL: Issues, https://github.com/sobhanAhmadian/soma_integrate/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

