# Comparing `tmp/spond_classes-0.8.1.tar.gz` & `tmp/spond_classes-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spond_classes-0.8.1.tar", max compression
+gzip compressed data, was "spond_classes-0.9.0.tar", max compression
```

## Comparing `spond_classes-0.8.1.tar` & `spond_classes-0.9.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1742 2024-05-03 18:25:13.871587 spond_classes-0.8.1/CHANGELOG.md
--rw-r--r--   0        0        0    35823 2023-12-24 18:39:51.814809 spond_classes-0.8.1/LICENSE
--rw-r--r--   0        0        0     1633 2024-05-03 18:25:13.869583 spond_classes-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     2762 2024-05-03 18:25:14.842922 spond_classes-0.8.1/README.md
--rw-r--r--   0        0        0      336 2024-03-31 18:32:28.304420 spond_classes-0.8.1/spond_classes/__init__.py
--rw-r--r--   0        0        0     3298 2024-05-03 18:18:33.548165 spond_classes-0.8.1/spond_classes/event.py
--rw-r--r--   0        0        0     5186 2024-05-03 18:18:33.549165 spond_classes-0.8.1/spond_classes/group.py
--rw-r--r--   0        0        0     3331 2024-05-03 18:18:33.549165 spond_classes-0.8.1/spond_classes/member.py
--rw-r--r--   0        0        0        0 2023-12-24 18:39:51.816809 spond_classes-0.8.1/spond_classes/py.typed
--rw-r--r--   0        0        0     1492 2024-05-03 18:18:33.549165 spond_classes-0.8.1/spond_classes/role.py
--rw-r--r--   0        0        0     1476 2024-05-03 18:18:33.550165 spond_classes-0.8.1/spond_classes/subgroup.py
--rw-r--r--   0        0        0     3499 1970-01-01 00:00:00.000000 spond_classes-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     2065 2024-05-09 11:23:48.247557 spond_classes-0.9.0/CHANGELOG.md
+-rw-r--r--   0        0        0    35823 2023-12-24 18:39:51.814809 spond_classes-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1958 2024-05-09 11:23:48.252828 spond_classes-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     3005 2024-05-09 11:09:44.224321 spond_classes-0.9.0/README.md
+-rw-r--r--   0        0        0      222 2024-05-09 11:09:45.384084 spond_classes-0.9.0/spond_classes/__init__.py
+-rw-r--r--   0        0        0     1795 2024-05-09 10:55:24.781772 spond_classes-0.9.0/spond_classes/event.py
+-rw-r--r--   0        0        0     3402 2024-05-09 10:55:24.905214 spond_classes-0.9.0/spond_classes/group.py
+-rw-r--r--   0        0        0     2258 2024-05-09 10:55:24.880009 spond_classes-0.9.0/spond_classes/member.py
+-rw-r--r--   0        0        0      192 2024-05-09 10:54:57.747925 spond_classes-0.9.0/spond_classes/profile.py
+-rw-r--r--   0        0        0        0 2023-12-24 18:39:51.816809 spond_classes-0.9.0/spond_classes/py.typed
+-rw-r--r--   0        0        0      586 2024-05-09 10:55:24.805315 spond_classes-0.9.0/spond_classes/role.py
+-rw-r--r--   0        0        0      619 2024-05-09 10:55:24.829755 spond_classes-0.9.0/spond_classes/subgroup.py
+-rw-r--r--   0        0        0     3678 1970-01-01 00:00:00.000000 spond_classes-0.9.0/PKG-INFO
```

### Comparing `spond_classes-0.8.1/CHANGELOG.md` & `spond_classes-0.9.0/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,27 @@
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
 and this project tries to adhere to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 Historic and pre-release versions aren't necessarily included.
 
 
+## [0.9.0] - 2024-05-09
+
+### Changed
+
+- BREAKING CHANGES: Significantly revised API - see README for details.
+
+- Rewritten from scratch using Pydantic; much closer to API data structure
+
+### Removed
+
+- Support for Python 3.8, 3.9
+
+
 ## [0.8.1] - 2024-05-03
 
 ### Added
 
 - Support for Python 3.12 in GitHub CI
 
 ### Changed
@@ -66,11 +79,12 @@
 - Enforce linting with isort, black and ruff in CI using GitHub Actions
 
 ### Changed
 
 - Update dev/test dependencies: ruff
 
 
+[0.9.0]: https://github.com/elliot-100/Spond-classes/compare/v0.8.1...v0.9.0
 [0.8.1]: https://github.com/elliot-100/Spond-classes/compare/v0.8.0...v0.8.1
 [0.8.0]: https://github.com/elliot-100/Spond-classes/compare/v0.7.3...v0.8.0
 [0.7.3]: https://github.com/elliot-100/Spond-classes/compare/v0.7.2...v0.7.3
 [0.7.2]: https://github.com/elliot-100/Spond-classes/compare/v0.7.1...v0.7.2
```

### Comparing `spond_classes-0.8.1/LICENSE` & `spond_classes-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spond_classes-0.8.1/pyproject.toml` & `spond_classes-0.9.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,59 @@
 [tool.poetry]
 name = "spond-classes"
-version = "0.8.1"
+version = "0.9.0"
 description = "Experimental Python class abstraction layer for `spond` package."
 authors = ["elliot-100 <3186037+elliot-100@users.noreply.github.com>"]
 readme = "README.md"
 homepage = "https://github.com/elliot-100/Spond-classes"
 repository = "https://github.com/elliot-100/Spond-classes"
 packages = [{include = "spond_classes"}]
 include = ["CHANGELOG.md"]
 license = "GPL 3.0"
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.10"
 python-dateutil = "^2.8.2"
 spond = "^0.99.1"
+pydantic = "^2.7.1"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.1.1"
 ruff = "^0.4.2"
 
 [tool.poetry.group.test.dependencies]
 mypy = "^1.8.0"
 pytest = "^8.1.1"
 types-python-dateutil = "^2.8.19.14"
 
 [tool.mypy]
+plugins = ["pydantic.mypy"]
+
+enable_error_code = ["ignore-without-code"]  # Require specific codes for ignores
 warn_unused_configs = true
 strict = true
 disallow_any_generics = false
 
+[tool.ruff]
+target-version = "py310"  # Ruff doesn't respect Python dependency in [tool.poetry.dependencies]
+
 [tool.ruff.lint]
+
 select = ["ALL"]
 
 # Ignore rules that conflict with Ruff formatter:
 #   COM812 Trailing comma missing
+#   ISC001 Implicitly concatenated string literals on one line
 
 # Ignore other rules:
 #   ANN101 Missing type annotation for `self` in method
 #   ANN102 Missing type annotation for `cls` in classmethod
 #   D205 1 blank line required between summary line and description
 
-ignore = ["COM812", "ANN101", "ANN102", "D205"]
+ignore = ["COM812", "ISC001", "ANN101", "ANN102", "D205"]
 
 [tool.ruff.lint.per-file-ignores]
 # Ignore rules that aren't relevant in tests:
 #   S101 Use of assert detected
 "**/{tests}/*" = ["S101"]
 
 # Ignore rules that conflict with Mypy
```

### Comparing `spond_classes-0.8.1/README.md` & `spond_classes-0.9.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,121 +1,148 @@
-# Spond-classes
-
-## About
-
-[Spond](https://spond.com/welcome) is a team/group-oriented events system.
-
-The unofficial Python [`spond` library package](https://github.com/Olen/Spond/) gets
-data from the Spond API and returns `dict` objects.
-
-This unofficial Python `spond-classes` package parses those `dict` objects to create
-class instances, i.e. provides an object abstraction layer.
-
-Experimental, very partial, read-only implementation.
-
-## Install
-
-Install from PyPI, e.g:
-`
-pip install spond-classes
-`
-Or if you're using Poetry:
-`
-poetry add spond-classes
-`
-
-## Example code
-
-Adapting the example code in [`Spond`](https://github.com/Olen/Spond/) README:
-
-```
-import asyncio
-from spond import spond
-import spond_classes
-
-username = 'my@mail.invalid'
-password = 'Pa55worD'
-group_id = 'C9DC791FFE63D7914D6952BE10D97B46'  # fake
-
-async def main():
-    s = spond.Spond(username=username, password=password)
-    group_data = await s.get_group(group_id)
-    await s.clientsession.close()
-
-    # Now we can create a class instance ...
-    group = spond_classes.Group.from_dict(group_data)
-
-    # ... use class properties instead of dict keys ...
-    print(group.name)
-
-    # ... and access child instances and their properties
-    for member in group.members:
-        print(member.full_name)
-
-asyncio.run(main())
-```
-## Key features
-
-* Create `Group` class instance from the dict returned by the corresponding `spond`
-  method:
-
-```
-spond_classes.Group.from_dict()
-```
-
-* Then access class instance attributes and methods:
-
-```
-Group.uid: str
-Group.name: str
-Group.members: List[Member]
-Group.member_by_id() -> Member
-Group.roles: List[SpondRoles]
-Group.role_by_id() -> Role
-Group.subgroups: List[Subgroup]
-Group.subgroup_by_id() -> Subgroup
-```
-
-* Also provides access to child `Member`, `Role`, `Subgroup` instances:
-
-```
-Member.uid: str
-Member.created_time: datetime
-Member.first_name: str
-Member.last_name: str
-Member.full_name: str
-Member.phone_number: str
-Member.profile_uid: str
-Member.roles: List[Role]
-Member.subgroups: List[Subgroup]
-
-Role.uid: str
-Role.members: List[Member]
-Role.name: str
-
-Subgroup.uid: str
-Subgroup.members: List[Member]
-Subgroup.name: str
-```
-
-* Create `Event` class instance from the dict returned by the corresponding `Spond`
-  method:
-
-```
-spond_classes.Event.from_dict()
-```
-
-* Then access attributes:
-
-```
-Event.uid: str
-Event.heading: str
-Event.start_time: datetime
-Event.accepted_uids: list
-Event.declined_uids: list
-Event.unanswered_uids: list
-Event.waiting_list_uids: list
-Event.unconfirmed_uids: list
-```
-
-It's also possible to create `Member.from_dict()`, `Role.from_dict()`,
-`Subgroup.from_dict()`.
+Metadata-Version: 2.1
+Name: spond-classes
+Version: 0.9.0
+Summary: Experimental Python class abstraction layer for `spond` package.
+Home-page: https://github.com/elliot-100/Spond-classes
+License: GPL 3.0
+Author: elliot-100
+Author-email: 3186037+elliot-100@users.noreply.github.com
+Requires-Python: >=3.10,<4.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: pydantic (>=2.7.1,<3.0.0)
+Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
+Requires-Dist: spond (>=0.99.1,<0.100.0)
+Project-URL: Repository, https://github.com/elliot-100/Spond-classes
+Description-Content-Type: text/markdown
+
+# Spond-classes
+
+## About
+
+[Spond](https://spond.com/welcome) is a team/group-oriented events system.
+
+The unofficial Python [`spond` library package](https://github.com/Olen/Spond/) gets
+data from the Spond API and returns `dict` objects.
+
+This unofficial Python `spond-classes` package parses those `dict` objects to create
+class instances, i.e. provides an object abstraction layer.
+
+Experimental, very partial, read-only implementation.
+
+## Install
+
+Install from PyPI, e.g:
+`
+pip install spond-classes
+`
+Or if you're using Poetry:
+`
+poetry add spond-classes
+`
+
+## Example code
+
+Adapting the example code in [`Spond`](https://github.com/Olen/Spond/) README:
+
+```
+import asyncio
+from spond import spond
+import spond_classes
+
+# fake credentials and ids
+username = 'my@mail.invalid'
+password = 'Pa55worD'
+group_id = 'G1'
+subgroup_id = 'SG1'
+
+async def main():
+    s = spond.Spond(username=username, password=password)
+    group_data = await s.get_group(group_id)
+    await s.clientsession.close()
+
+    # Now we can create a class instance ...
+    group = spond_classes.Group(**group_data)
+
+    # ... use class properties instead of dict keys ...
+    print(group.name)
+
+    # ... access nested instances and their properties ...
+    for member in group.members:
+        print(f"{member.full_name} is in the {group.name} group")
+
+    # ... and use some helper methods
+    for member in group.members_by_subgroup(group.subgroup_by_id(subgroup_id))
+        print(f"{member.full_name} is in the {subgroup.name} subgroup")
+
+asyncio.run(main())
+```
+## Key features
+
+* Create `Group` class instance from the dict returned by the corresponding `spond`
+  method:
+
+```
+spond_classes.Group()
+```
+
+* Then access class instance attributes and methods:
+
+```
+Group.uid: str
+Group.members: list[Member]
+Group.name: str
+Group.roles: list[Role]
+Group.subgroups: list[Subgroup]
+
+Group.member_by_id() -> Member
+Group.role_by_id() -> Role
+Group.subgroup_by_id() -> Subgroup
+
+Group.members_by_subgroup(subgroup: Subgroup) -> list[Member]
+Group.members_by_role(role: Role) -> list[Member]
+```
+
+* Also provides access to nested `Member`, `Role`, `Subgroup` instances:
+
+```
+Member.uid: str
+Member.created_time: datetime
+Member.email: str
+Member.first_name: str
+Member.full_name: str
+Member.last_name: str
+Member.phone_number: str
+Member.Profile.uid: str
+Member.role_uids: list[str]
+Member.subgroup_uids: list[str]
+
+Role.uid: str
+Role.name: str
+
+Subgroup.uid: str
+Subgroup.name: str
+```
+
+* Create `Event` class instance from the dict returned by the corresponding `Spond`
+  method:
+
+```
+spond_classes.Event(**dict)
+```
+
+* Then access attributes:
+
+```
+Event.uid: str
+Event.heading: str
+Event.start_time: datetime
+Event.Responses.accepted_uids: list
+Event.Responses.declined_uids: list
+Event.Responses.unanswered_uids: list
+Event.Responses.waiting_list_uids: list
+Event.Responses.unconfirmed_uids: list
+```
+
```

