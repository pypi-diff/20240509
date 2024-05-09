# Comparing `tmp/pyaimopt-0.7.4.tar.gz` & `tmp/pyaimopt-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaimopt-0.7.4.tar", max compression
+gzip compressed data, was "pyaimopt-0.7.5.tar", max compression
```

## Comparing `pyaimopt-0.7.4.tar` & `pyaimopt-0.7.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    11631 2024-03-25 17:21:04.293085 pyaimopt-0.7.4/LICENSE
--rw-r--r--   0        0        0   232878 2024-03-25 17:21:04.308710 pyaimopt-0.7.4/NOTICE.html
--rw-r--r--   0        0        0      377 2024-03-25 17:21:04.308710 pyaimopt-0.7.4/pyaimopt/__init__.py
--rw-r--r--   0        0        0    11859 2024-03-25 17:21:04.308710 pyaimopt-0.7.4/pyaimopt/aim_credentials.py
--rw-r--r--   0        0        0     6511 2024-03-25 17:21:04.308710 pyaimopt-0.7.4/pyaimopt/azure_test.py
--rw-r--r--   0        0        0    32951 2024-03-25 17:21:04.308710 pyaimopt-0.7.4/pyaimopt/azure_workspace.py
--rw-r--r--   0        0        0     9797 2024-03-25 17:21:04.308710 pyaimopt-0.7.4/pyaimopt/builder.py
--rw-r--r--   0        0        0     1407 2024-03-25 17:21:04.308710 pyaimopt-0.7.4/pyaimopt/constants.py
--rw-r--r--   0        0        0     2399 2024-03-25 17:21:04.308710 pyaimopt-0.7.4/pyaimopt/description.py
--rw-r--r--   0        0        0    11631 2024-03-25 17:21:04.308710 pyaimopt-0.7.4/pyaimopt/LICENSE
--rw-r--r--   0        0        0     1853 2024-03-25 17:21:04.308710 pyaimopt-0.7.4/pyaimopt/platform.py
--rw-r--r--   0        0        0    27535 2024-03-25 17:21:04.308710 pyaimopt-0.7.4/pyaimopt/problem.py
--rw-r--r--   0        0        0     7052 2024-03-25 17:21:04.308710 pyaimopt-0.7.4/pyaimopt/serialization.py
--rw-r--r--   0        0        0     4154 2024-03-25 17:21:04.308710 pyaimopt-0.7.4/pyaimopt/solver.py
--rw-r--r--   0        0        0    11644 2024-03-25 17:21:04.308710 pyaimopt-0.7.4/pyaimopt/use.txt
--rw-r--r--   0        0        0    10113 2024-03-25 17:21:04.324335 pyaimopt-0.7.4/pyaimopt/workspace.py
--rw-r--r--   0        0        0     1400 2024-03-25 17:21:04.324335 pyaimopt-0.7.4/pyproject.toml
--rw-r--r--   0        0        0     4388 2024-03-25 17:21:04.308710 pyaimopt-0.7.4/README.md
--rw-r--r--   0        0        0     5505 1970-01-01 00:00:00.000000 pyaimopt-0.7.4/setup.py
--rw-r--r--   0        0        0     5319 1970-01-01 00:00:00.000000 pyaimopt-0.7.4/PKG-INFO
+-rw-r--r--   0        0        0    11631 2024-05-09 09:33:01.588844 pyaimopt-0.7.5/LICENSE
+-rw-r--r--   0        0        0   232878 2024-05-09 09:33:01.588844 pyaimopt-0.7.5/NOTICE.html
+-rw-r--r--   0        0        0      377 2024-05-09 09:33:01.604471 pyaimopt-0.7.5/pyaimopt/__init__.py
+-rw-r--r--   0        0        0    11859 2024-05-09 09:33:01.604471 pyaimopt-0.7.5/pyaimopt/aim_credentials.py
+-rw-r--r--   0        0        0     6511 2024-05-09 09:33:01.604471 pyaimopt-0.7.5/pyaimopt/azure_test.py
+-rw-r--r--   0        0        0    32951 2024-05-09 09:33:01.604471 pyaimopt-0.7.5/pyaimopt/azure_workspace.py
+-rw-r--r--   0        0        0     9797 2024-05-09 09:33:01.604471 pyaimopt-0.7.5/pyaimopt/builder.py
+-rw-r--r--   0        0        0     1407 2024-05-09 09:33:01.604471 pyaimopt-0.7.5/pyaimopt/constants.py
+-rw-r--r--   0        0        0     2399 2024-05-09 09:33:01.604471 pyaimopt-0.7.5/pyaimopt/description.py
+-rw-r--r--   0        0        0    11631 2024-05-09 09:33:01.604471 pyaimopt-0.7.5/pyaimopt/LICENSE
+-rw-r--r--   0        0        0     1853 2024-05-09 09:33:01.604471 pyaimopt-0.7.5/pyaimopt/platform.py
+-rw-r--r--   0        0        0    27535 2024-05-09 09:33:01.604471 pyaimopt-0.7.5/pyaimopt/problem.py
+-rw-r--r--   0        0        0     7052 2024-05-09 09:33:01.604471 pyaimopt-0.7.5/pyaimopt/serialization.py
+-rw-r--r--   0        0        0     4154 2024-05-09 09:33:01.604471 pyaimopt-0.7.5/pyaimopt/solver.py
+-rw-r--r--   0        0        0    11644 2024-05-09 09:33:01.604471 pyaimopt-0.7.5/pyaimopt/use.txt
+-rw-r--r--   0        0        0    10113 2024-05-09 09:33:01.604471 pyaimopt-0.7.5/pyaimopt/workspace.py
+-rw-r--r--   0        0        0     1400 2024-05-09 09:33:01.604471 pyaimopt-0.7.5/pyproject.toml
+-rw-r--r--   0        0        0     4388 2024-05-09 09:33:01.588844 pyaimopt-0.7.5/README.md
+-rw-r--r--   0        0        0     5505 1970-01-01 00:00:00.000000 pyaimopt-0.7.5/setup.py
+-rw-r--r--   0        0        0     5319 1970-01-01 00:00:00.000000 pyaimopt-0.7.5/PKG-INFO
```

### Comparing `pyaimopt-0.7.4/LICENSE` & `pyaimopt-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaimopt-0.7.4/NOTICE.html` & `pyaimopt-0.7.5/NOTICE.html`

 * *Files identical despite different names*

### Comparing `pyaimopt-0.7.4/pyaimopt/aim_credentials.py` & `pyaimopt-0.7.5/pyaimopt/aim_credentials.py`

 * *Files identical despite different names*

### Comparing `pyaimopt-0.7.4/pyaimopt/azure_test.py` & `pyaimopt-0.7.5/pyaimopt/azure_test.py`

 * *Files identical despite different names*

### Comparing `pyaimopt-0.7.4/pyaimopt/azure_workspace.py` & `pyaimopt-0.7.5/pyaimopt/azure_workspace.py`

 * *Files identical despite different names*

### Comparing `pyaimopt-0.7.4/pyaimopt/builder.py` & `pyaimopt-0.7.5/pyaimopt/builder.py`

 * *Files identical despite different names*

### Comparing `pyaimopt-0.7.4/pyaimopt/constants.py` & `pyaimopt-0.7.5/pyaimopt/constants.py`

 * *Files identical despite different names*

### Comparing `pyaimopt-0.7.4/pyaimopt/description.py` & `pyaimopt-0.7.5/pyaimopt/description.py`

 * *Files identical despite different names*

### Comparing `pyaimopt-0.7.4/pyaimopt/LICENSE` & `pyaimopt-0.7.5/pyaimopt/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaimopt-0.7.4/pyaimopt/platform.py` & `pyaimopt-0.7.5/pyaimopt/platform.py`

 * *Files identical despite different names*

### Comparing `pyaimopt-0.7.4/pyaimopt/problem.py` & `pyaimopt-0.7.5/pyaimopt/problem.py`

 * *Files identical despite different names*

### Comparing `pyaimopt-0.7.4/pyaimopt/serialization.py` & `pyaimopt-0.7.5/pyaimopt/serialization.py`

 * *Files identical despite different names*

### Comparing `pyaimopt-0.7.4/pyaimopt/solver.py` & `pyaimopt-0.7.5/pyaimopt/solver.py`

 * *Files identical despite different names*

### Comparing `pyaimopt-0.7.4/pyaimopt/use.txt` & `pyaimopt-0.7.5/pyaimopt/use.txt`

 * *Files identical despite different names*

### Comparing `pyaimopt-0.7.4/pyaimopt/workspace.py` & `pyaimopt-0.7.5/pyaimopt/workspace.py`

 * *Files identical despite different names*

### Comparing `pyaimopt-0.7.4/pyproject.toml` & `pyaimopt-0.7.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyaimopt"
-version = "0.7.4"
+version = "0.7.5"
 description = ""
 authors = ["Project AIM <project-aim-contact@microsoft.com>",
            "Christos Gkantsidis",
            "Greg O'Shea"]
 readme = "README.md"
 license = "Proprietary"
 include = [ "NOTICE.html" ]
```

### Comparing `pyaimopt-0.7.4/README.md` & `pyaimopt-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `pyaimopt-0.7.4/setup.py` & `pyaimopt-0.7.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 {':python_version >= "3.8" and python_version < "3.12"': ['scipy>=1.10.1,<2.0.0']}
 
 entry_points = \
 {'console_scripts': ['aim = pyaimopt.azure_test:main']}
 
 setup_kwargs = {
     'name': 'pyaimopt',
-    'version': '0.7.4',
+    'version': '0.7.5',
     'description': '',
     'long_description': '# `pyaimopt`: Python Wrapper for the AIM optimization service\n\n`pyaimopt` is a package that provides access to the Analog Iterative Machine (`AIM`) optimization service.\nThe `AIM` optimizer accepts problems in the quadratic unconstrained mixed optimization (`QUMO`) format.\nThe `QUMO` format is a generalization of the quadratic unconstrained binary optimization (`QUBO`) format,\nand allows for the optimization of continuous variables in addition to binary variables.\nThe `AIM` optimizer is a stochastic optimization algorithm that uses a combination of gradient descent and\nannealing to find the global minimum of a given objective function.\nIn addition to `QUMO` and `QUBO` problems, the `AIM` optimizer can also be used to solve `MaxCut` and `Ising`\nproblems.\n\n[![Build Status](https://img.shields.io/travis/username/pyaimopt.svg)](https://travis-ci.org/username/pyaimopt)\n[![Coverage Status](https://img.shields.io/coveralls/github/username/pyaimopt.svg)](https://coveralls.io/github/username/pyaimopt)\n[![License: MS-PL](https://img.shields.io/badge/License-MSPL-green.svg)](https://opensource.org/licenses/MS-PL)\n[![PyPI version](https://badge.fury.io/py/pyaimopt.svg)](https://pypi.org/project/pyaimopt/)\n\n## Table of Contents\n\n- [`pyaimopt`: Python Wrapper for the AIM optimization service](#pyaimopt-python-wrapper-for-the-aim-optimization-service)\n  - [Table of Contents](#table-of-contents)\n  - [Prerequisites](#prerequisites)\n  - [Installation](#installation)\n  - [Authentication and API Keys](#authentication-and-api-keys)\n  - [Usage Examples](#usage-examples)\n  - [Documentation](#documentation)\n  - [Contributing](#contributing)\n  - [License](#license)\n  - [Contact Information](#contact-information)\n\n## Prerequisites\n\nThe package requires Python 3.10 or higher. It is recommended to use a virtual environment to install the package.\n\n\n## Installation\n\nTo install pyaimopt, simply use pip:\n\n```bash\npip install pyaimopt -i https://msr-optics.pkgs.visualstudio.com/OpticalCompute/_packaging/OpticalCompute/pypi/simple/\n```\n\nYou can check successful installation by running the following command:\n\n```bash\naim status\n```\n\nIt should return the version of the installed package and the status of the AIM service.\n\n_TODO_: Example with passing the API key.\n\n## Authentication and API Keys\n\n_TODO_: Add instructions on how to get an API key. This should be done by the AIM team.\n\n_TODO_: Explain how to pass the API key to the package.\n\n_TODO_: Explain alternative authentication methods.\n\n## Usage Examples\n\nTo get started, you can use the following commands to submit a simple `QUMO` problem to the `AIM` optimizer,\ncheck the status of the submitted problem, and retrieve the results.\n\n```bash\naim submit\n# This returns: "Submitted job <job_id>"\naim list\n# The output should contain the <job_id> of the submitted job and its status\n# Upon completion, the status should be "Completed"\naim retrieve <job_id>\n# This returns the results of the optimization\n```\n\n_TODO_: Add example of submitting a simple `QUMO` problem using the synchronous interface.\n\n_TODO_: Add example of using the asynchronous interface.\n\n_TODO_: Mention the `GitHub` repository that contains examples.\n\n## Documentation\n\n_TODO_: Add a link to the documentation.\n\n## Contributing\n\nContributions are welcome!\n\n_TODO_: Add instructions on how to contribute examples.\n\n_TODO_: Add instructions on how to report bugs, and propose new features.\n\n_TODO_: Add instructions on how to suggest changes to the solver.\n\n## License\n\nThis package is released under the `MS-PL` License. See the [LICENSE](LICENSE) file for more information.\n\nThe package depends on a number of external packages.\nThe list of those packages and their corresponding licences can be found in the [NOTICE.html](file:///NOTICE.html) file.\n\n## Contact Information\n\nFor questions or comments related to the functionality or features of the `AIM` optimizer,\nplease raise an issue on the [AIM GitHub repository]().\n\nTo get access to the service, please contact the [AIM Team](mailto:project-aim-contant@microsoft.com).\nAt this point, the service is available to selected users only.\n\nFor further questions or comments, please contact the [AIM Team](mailto:project-aim-service@microsoft.com).\n\n_TODO_: Add a link to the *Issues* page.\n',
     'author': 'Project AIM',
     'author_email': 'project-aim-contact@microsoft.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pyaimopt-0.7.4/PKG-INFO` & `pyaimopt-0.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaimopt
-Version: 0.7.4
+Version: 0.7.5
 Summary: 
 License: Proprietary
 Author: Project AIM
 Author-email: project-aim-contact@microsoft.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

